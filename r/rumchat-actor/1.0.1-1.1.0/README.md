# Comparing `tmp/rumchat_actor-1.0.1.tar.gz` & `tmp/rumchat_actor-1.1.0.tar.gz`

## Comparing `rumchat_actor-1.0.1.tar` & `rumchat_actor-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 rumchat_actor-1.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0    16023 2020-02-02 00:00:00.000000 rumchat_actor-1.0.1/src/rumchat_actor/__init__.py
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 rumchat_actor-1.0.1/src/rumchat_actor/common_commands.py
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 rumchat_actor-1.0.1/LICENSE.txt
--rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 rumchat_actor-1.0.1/README.md
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 rumchat_actor-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 rumchat_actor-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 rumchat_actor-1.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0    20765 2020-02-02 00:00:00.000000 rumchat_actor-1.1.0/src/rumchat_actor/__init__.py
+-rw-r--r--   0        0        0    20058 2020-02-02 00:00:00.000000 rumchat_actor-1.1.0/src/rumchat_actor/common_commands.py
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 rumchat_actor-1.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 rumchat_actor-1.1.0/README.md
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 rumchat_actor-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 rumchat_actor-1.1.0/PKG-INFO
```

### Comparing `rumchat_actor-1.0.1/.github/workflows/python-publish.yml` & `rumchat_actor-1.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `rumchat_actor-1.0.1/src/rumchat_actor/__init__.py` & `rumchat_actor-1.1.0/src/rumchat_actor/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,29 +2,41 @@
 """Rumble Chat Actor
 
 Automatically interact with your Rumble livestream chats.
 S.D.G."""
 
 import textwrap
 import time
+import threading
 from cocorum import RumbleAPI, utils
 from cocorum.ssechat import SSEChat
 import selenium
 from selenium import webdriver
 from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.common.alert import Alert
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.keys import Keys
+from selenium.webdriver.support import expected_conditions as EC
+from selenium.webdriver.support.ui import WebDriverWait
 
-#How long to wait after performing any browser action, for the webpage to load its response
-BROWSER_ACTION_DELAY = 2
+#How long to wait maximum for a condition to be true in the browser
+BROWSER_WAIT_TIMEOUT = 30
+
+#How long to wait between sending messages
+SEND_MESSAGE_COOLDOWN = 3
 
 #Popout chat url. Format with stream_id_b10
 CHAT_URL = "https://rumble.com/chat/popup/{stream_id_b10}"
 
+#Rumble user URL. Format with username
+USER_URL = "https://rumble.com/user/{username}"
+
+#Rumble channel URL. Format with channel_name
+CHANNEL_URL = "https://rumble.com/c/{channel_name}"
+
 #Maximum chat message length
 MAX_MESSAGE_LEN = 200
 
 #Message split across multiple lines must not be longer than this
 MAX_MULTIMESSAGE_LEN = 1000
 
 #Prefix to all actor messages
@@ -38,42 +50,65 @@
     "5" : "cmi js-btn-mute-current-5",
     "stream" : "cmi js-btn-mute-current",
     "forever" : "cmi js-btn-mute-for-account",
     }
 
 class ChatCommand():
     """A chat command, internal use only"""
-    def __init__(self, name, actor, cooldown = BROWSER_ACTION_DELAY, amount_cents = 0, whitelist_badges = ["moderator"], target = None):
+    def __init__(self, name, actor, cooldown = SEND_MESSAGE_COOLDOWN, amount_cents = 0, exclusive = False, allowed_badges = ["subscriber"], whitelist_badges = ["moderator"], target = None):
         """name: The !name of the command
     actor: The RumleChatActor host object
     amount_cents: The minimum cost of the command. Defaults to free
+    exclusive: If this command can only be run by users with allowed badges. Defaults to False
+    allowed_badges: Badges that are allowed to run this command (if it is exclusive).
+        Defaults to subscribers, admin is added internally.
     whitelist_badges: Badges which if borne give the user free-of-charge command access
-    target: The function(message, actor) to call on successful command usage. Defaults to self.run"""
+    target: The command function(message, actor) to call. Defaults to self.run"""
         assert " " not in name, "Name cannot contain spaces"
         self.name = name
         self.actor = actor
-        assert cooldown >= BROWSER_ACTION_DELAY, f"Cannot set a cooldown shorter than {BROWSER_ACTION_DELAY}"
+        assert cooldown >= SEND_MESSAGE_COOLDOWN, \
+            f"Cannot set a cooldown shorter than {SEND_MESSAGE_COOLDOWN}"
+
         self.cooldown = cooldown
         self.amount_cents = amount_cents #Cost of the command
+        self.exclusive = exclusive
+        self.allowed_badges = ["admin"] + allowed_badges #Admin can always run any command
         self.whitelist_badges = ["admin"] + whitelist_badges #Admin always has free-of-charge usage
         self.last_use_time = 0 #Last time the command was called
         self.target = target
 
     def call(self, message):
         """The command was called"""
+        #this command is exclusive, and the user does not have the required badge
+        if self.exclusive and \
+            not (True in [badge.slug in self.allowed_badges for badge in message.user.badges]):
+
+            self.actor.send_message(f"@{message.user.username} That command is exclusive to: " +
+                                    ", ".join(self.allowed_badges)
+                                    )
+
+            return
 
         #The command is still on cooldown
         if (curtime := time.time()) - self.last_use_time < self.cooldown:
-            self.actor.send_message(f"@{message.user.username} That command is still on cooldown. Try again in {int(self.last_use_time + self.cooldown - curtime + 0.5)} seconds.")
+            self.actor.send_message(
+                f"@{message.user.username} That command is still on cooldown. " +
+                f"Try again in {int(self.last_use_time + self.cooldown - curtime + 0.5)} seconds."
+                )
 
             return
 
         #the user did not pay enough for the command and they do not have a free pass
-        if message.rant_price_cents < self.amount_cents and not (True in [badge.slug in self.whitelist_badges for badge in message.user.badges]):
-            self.actor.send_message(f"@{message.user.username} That command costs ${self.amount_cents/100:.2f}.")
+        if message.rant_price_cents < self.amount_cents and \
+            not (True in [badge.slug in self.whitelist_badges for badge in message.user.badges]):
+
+            self.actor.send_message("@" + message.user.username +
+                                    f"That command costs ${self.amount_cents/100:.2f}."
+                                    )
             return
 
         #the command was called successfully
         self.run(message)
 
         #Mark the last use time for cooldown
         self.last_use_time = time.time()
@@ -81,58 +116,48 @@
     def run(self, message):
         """Dummy run method"""
         if self.target:
             self.target(message, self.actor)
             return
 
         #Run method was never defined
-        self.actor.send_message(f"@{message.user.username} Hello, this command never had a target defined. :-)")
-
-class ExclusiveChatCommand(ChatCommand):
-    """Chat command that only certain badges can use"""
-    def __init__(self, name, actor, cooldown = BROWSER_ACTION_DELAY, amount_cents = 0, allowed_badges = ["subscriber"], whitelist_badges = ["moderator"], target = None):
-        """name: The !name of the command
-    actor: The RumleChatActor host object
-    amount_cents: The minimum cost of the command. Defaults to free
-    allowed_badges: Badges which must be borne to use the command at all
-    whitelist_badges: Badges which if borne give the user free-of-charge command access
-    target: The function(message, actor) to call on successful command usage. Defaults to self.run"""
-        super().__init__(name, actor, cooldown = BROWSER_ACTION_DELAY, amount_cents = 0, whitelist_badges = ["moderator"], target = target)
-        #Admin can always call any command
-        self.allowed_badges = ["admin"] + allowed_badges
-
-    def call(self, message):
-        """The command was called"""
-        #the user does not have the required badge
-        if not (True in [badge.slug in self.allowed_badges for badge in message.user.badges]):
-            self.actor.send_message(f"@{message.user.username} That command is exclusive to: " + ", ".join(self.allowed_badges))
-            return
-
-        #Proceed with normal command processing
-        super().call(message)
+        self.actor.send_message("@" + message.user.username +
+                                "Hello, this command never had a target defined. :-)"
+                                )
 
 class RumbleChatActor():
     """Actor that interacts with Rumble chat"""
-    def __init__(self, stream_id = None, init_message = "Hello, Rumble world!", profile_dir = None, credentials = None, api_url = None):
+    def __init__(self, stream_id = None, init_message = "Hello, Rumble world!", profile_dir = None, username = None, password = None, api_url = None, streamer_username = None, streamer_channel = None, is_channel_stream = None, ignore_users = ["TheRumbleBot"]):
         """stream_id: The stream ID you want to connect to. Defaults to latest livestream
     init_message: What to say when the actor starts up.
     profile_dir: The Firefox profile directory to use. Defaults to temp (sign-in not saved)
-    credentials: The (username, password) to log in with. Defaults to manual log in"""
+    credentials: The (username, password) to log in with. Defaults to manual log in
+    api_url: The Rumble Live Stream API URL with your key
+    streamer_username: The username of the person streaming
+    streamer_channel: The channel doing the livestream
+    is_channel_stream: If the livestream is on a channel or not
+    ignore_users: List of usernames, will ignore all their messages"""
+
+        #The info of the person streaming
+        self.__streamer_username = streamer_username
+        self.__streamer_channel = streamer_channel
+        self.__is_channel_stream = is_channel_stream
 
         #Get Live Stream API
         if api_url:
             self.rum_api = RumbleAPI(api_url)
         else:
             self.rum_api = None
 
         #A stream ID was passed
         if stream_id:
             self.stream_id, self.stream_id_b10 = utils.stream_id_36_and_10(stream_id)
 
-            #It is not our livestream or we have no Live Stream API, LS API functions are not available
+            #It is not our livestream or we have no Live Stream API,
+            #so LS API functions are not available
             if not self.rum_api or self.stream_id not in self.rum_api.livestreams:
                 self.api_stream = None
 
             #It is our livestream, we can use the Live Stream API
             else:
                 self.api_stream = self.rum_api.livestreams[stream_id]
 
@@ -162,61 +187,133 @@
         self.browser.minimize_window()
         self.browser.get(CHAT_URL.format(stream_id_b10 = self.ssechat.stream_id_b10))
         assert "Chat" in self.browser.title
 
         #Sign in to chat, unless we are already. While there is a sign-in button...
         while sign_in_buttn := self.get_sign_in_button():
             #We have credentials
-            if credentials:
+            if username and password:
                 sign_in_buttn.click()
-                time.sleep(BROWSER_ACTION_DELAY)
-                self.browser.find_element(By.ID, "login-username").send_keys(credentials[0] + Keys.RETURN)
-                self.browser.find_element(By.ID, "login-password").send_keys(credentials[1] + Keys.RETURN)
-                break #We only need to do that once
+                WebDriverWait(self.browser, BROWSER_WAIT_TIMEOUT).until(
+                    EC.visibility_of_element_located((By.ID, "login-username")),
+                    "Timed out waiting for sign-in dialouge"
+                    )
+
+                uname_field = self.browser.find_element(By.ID, "login-username")
+                uname_field.send_keys(username + Keys.RETURN)
+                self.browser.find_element(By.ID, "login-password").send_keys(password + Keys.RETURN)
 
             #We do not have credentials, ask for manual sign in
             self.browser.maximize_window()
             input("Please log in at the browser, then press enter here.")
 
-            #Wait for signed in loading to complete
-            time.sleep(BROWSER_ACTION_DELAY)
+        #Wait for signed in loading to complete
+        WebDriverWait(self.browser, BROWSER_WAIT_TIMEOUT).until(
+            EC.element_to_be_clickable((By.ID, "chat-message-text-input")),
+            "Timed out waiting for chat message field to become usable"
+            )
+
 
         #Find our username
-        if credentials:
-            self.username = credentials[0]
+        if username:
+            self.username = username
         elif self.rum_api:
             self.username = self.rum_api.username
         else:
             self.username = None
             while not self.username:
                 self.username = input("Enter the username the actor is using: ")
 
-        #Wait for potential further page load?
-        time.sleep(BROWSER_ACTION_DELAY)
+        #Ignore these users when processing messages
+        self.ignore_users = ignore_users
 
         #History of the bot's messages so they do not get loop processed
         self.sent_messages = []
 
+        #Messages waiting to be sent
+        self.outbox = []
+
+        #Time that the last message we sent was sent
+        self.last_message_send_time = 0
+
+        #Loop condition of the mainloop() and sender_loop() methods
+        self.keep_running = True
+
+        #thread to send messages at timed intervals
+        self.sender_thread = threading.Thread(target = self._sender_loop, daemon = True)
+        self.sender_thread.start()
+
         #Send an initialization message to get wether we are moderator or not
         self.send_message(init_message)
 
         #Wait until we get that message
         while (m := self.ssechat.get_message()).user.username != self.username:
             pass
 
-        assert "moderator" in m.user.badges or "admin" in m.user.badges, "Actor cannot function without being a moderator"
+        assert "moderator" in m.user.badges or "admin" in m.user.badges, \
+            "Actor cannot function without being a moderator"
 
-        #Functions that are to be called on each message, must return False if the message was deleted
+        #Functions that are to be called on each message,
+        #must return False if the message was deleted
         self.message_actions = []
 
         #Instances of RumbleChatCommand, by name
         self.chat_commands = {}
 
-        #Loop condition of the mainloop() method
-        self.keep_running = True
+    @property
+    def streamer_username(self):
+        """The username of the streamer"""
+        if not self.__streamer_username:
+            #We are the ones streaming
+            if self.api_stream:
+                self.__streamer_username = self.rum_api.username
+            else:
+                self.__streamer_username = input("Enter the username of the person streaming: ")
+
+        return self.__streamer_username
+
+    @property
+    def streamer_channel(self):
+        """The channel of the streamer"""
+        #We don't yet have the streamer channel, and this is a channel stream
+        if not self.__streamer_channel and self.is_channel_stream:
+            #We are the ones streaming, and the API URL is under the channel
+            if self.api_stream and self.rum_api.channel_name:
+                self.__streamer_channel = self.rum_api.channel_name
+
+            #We are not the ones streaming,
+            #or the API URL was not under our channel,
+            #and we are sure this is a channel stream
+            else:
+                self.__streamer_channel = input("Enter the channel of the person streaming: ")
+
+        return self.__streamer_channel
+
+    @property
+    def is_channel_stream(self):
+        """Is the stream under a channel?"""
+        #We do not know yet
+        if self.__is_channel_stream is None:
+            #We know that this is a channel stream because it showed up in the channel-specific API
+            if self.api_stream and self.rum_api.channel_name:
+                self.__is_channel_stream = True
+
+            #We will ask the user
+            else:
+                self.__is_channel_stream = "y" in input("Is this a channel stream? y/[N]:")
+
+        return self.__is_channel_stream
+
+    @property
+    def streamer_main_page_url(self):
+        """The URL of the main page of the streamer"""
+        if self.is_channel_stream:
+            return CHANNEL_URL.format(channel_name = self.streamer_channel)
+
+        return USER_URL.format(username = self.streamer_username)
 
     def get_sign_in_button(self):
         """Look for the sign in button"""
         try:
             return self.browser.find_element(By.CLASS_NAME, "chat--sign-in")
         except selenium.common.exceptions.NoSuchElementException:
             print("Could not find sign-in button, already signed in.")
@@ -224,22 +321,32 @@
 
     def send_message(self, text):
         """Send a message in chat (splits across lines if necessary)"""
         text = BOT_MESSAGE_PREFIX + text
         assert "\n" not in text, "Message cannot contain newlines"
         assert len(text) < MAX_MULTIMESSAGE_LEN, "Message is too long"
         for subtext in textwrap.wrap(text, width = MAX_MESSAGE_LEN):
-            self.__send_message(subtext)
+            self.outbox.append(subtext)
+
+    def _sender_loop(self):
+        """Constantly check our outbox and send any messages in it"""
+        while self.keep_running:
+            #We have messages to send and it is time to send one
+            if self.outbox and time.time() - self.last_message_send_time > SEND_MESSAGE_COOLDOWN:
+                self.__send_message(self.outbox.pop(0))
+            time.sleep(0.1)
 
     def __send_message(self, text):
         """Send a message in chat"""
-        assert len(text) < MAX_MESSAGE_LEN, f"Message with prefix cannot be longer than {MAX_MESSAGE_LEN} characters"
+        assert len(text) < MAX_MESSAGE_LEN, \
+            f"Message with prefix cannot be longer than {MAX_MESSAGE_LEN} characters"
+
         self.sent_messages.append(text)
+        self.last_message_send_time = time.time()
         self.browser.find_element(By.ID, "chat-message-text-input").send_keys(text + Keys.RETURN)
-        time.sleep(BROWSER_ACTION_DELAY)
 
     def hover_element(self, element):
         """Hover over a selenium element"""
         ActionChains(self.browser).move_to_element(element).perform()
 
     def open_moderation_menu(self, message):
         """Open the moderation menu of a message"""
@@ -248,74 +355,107 @@
         if isinstance(message, webdriver.remote.webelement.WebElement) and message.tag_name == "li":
             message_li = message
             message_id = message_li.get_attribute("data-message-id")
 
         #Find the message by ID
         elif isinstance(message, int):
             message_id = message
-            message_li = self.browser.find_element(By.XPATH, f"//li[@class='chat-history--row js-chat-history-item'][@data-message-id='{message_id}']")
+            message_li = self.browser.find_element(
+                By.XPATH,
+                "//li[@class='chat-history--row js-chat-history-item']" +
+                f"[@data-message-id='{message_id}']"
+                )
 
         #The message has a message ID attribute
         elif hasattr(message, "message_id"):
             message_id = message.message_id
-            message_li = self.browser.find_element(By.XPATH, f"//li[@class='chat-history--row js-chat-history-item'][@data-message-id='{message_id}']")
+            message_li = self.browser.find_element(
+                By.XPATH,
+                "//li[@class='chat-history--row js-chat-history-item']" +
+                f"[@data-message-id='{message_id}']"
+                )
 
         #Not a valid message type
         else:
             raise TypeError("Message must be ID, li element, or have message_id attribute")
 
         #Hover over the message
         self.hover_element(message_li)
         #Find the moderation menu
-        menu_bttn = self.browser.find_element(By.XPATH, f"//li[@class='chat-history--row js-chat-history-item'][@data-message-id='{message_id}']/button[@class='js-moderate-btn chat-history--kebab-button']")
+        menu_bttn = message_li.find_element(
+            By.XPATH,
+            ".//button[@class='js-moderate-btn chat-history--kebab-button']"
+            )
         #Click the moderation menu button
         menu_bttn.click()
 
         return message_id
 
     def delete_message(self, message):
         """Delete a message in the chat"""
         m_id = self.open_moderation_menu(message)
-        del_bttn = self.browser.find_element(By.XPATH, f"//button[@class='cmi js-btn-delete-current'][@data-message-id='{m_id}']")
+        del_bttn = self.browser.find_element(
+            By.XPATH,
+            f"//button[@class='cmi js-btn-delete-current'][@data-message-id='{m_id}']"
+            )
+
         del_bttn.click()
-        time.sleep(BROWSER_ACTION_DELAY)
+
+        #Wait for the confirmation to appear
+        WebDriverWait(self.browser, BROWSER_WAIT_TIMEOUT).until(
+            EC.alert_is_present(),
+            "Timed out waiting for deletion confirmation dialouge to appear"
+            )
 
         #Confirm the confirmation dialog
         Alert(self.browser).accept()
 
     def mute_by_message(self, message, mute_level = "5"):
         """Mute a user by message"""
         self.open_moderation_menu(message)
-        timeout_bttn = self.browser.find_element(By.XPATH, f"//button[@class='{MUTE_LEVELS[mute_level]}']")
+        timeout_bttn = self.browser.find_element(
+            By.XPATH,
+            f"//button[@class='{MUTE_LEVELS[mute_level]}']"
+            )
+
         timeout_bttn.click()
 
     def mute_by_appearname(self, name, mute_level = "5"):
         """Mute a user by the name they are appearing with"""
         #Find any chat message by this user
-        message_li = self.browser.find_element(By.XPATH, f"//li[@class='chat-history--row js-chat-history-item'][@data-username='{name}']")
+        message_li = self.browser.find_element(
+            By.XPATH,
+            f"//li[@class='chat-history--row js-chat-history-item'][@data-username='{name}']"
+            )
+
         self.mute_by_message(message = message_li, mute_level = mute_level)
 
     def pin_message(self, message):
         """Pin a message by ID or li element"""
         self.open_moderation_menu(message)
         pin_bttn = self.browser.find_element(By.XPATH, "//button[@class='cmi js-btn-pin-current']")
         pin_bttn.click()
 
     def unpin_message(self):
         """Unpin the currently pinned message"""
         try:
-            unpin_bttn = self.browser.find_element(By.XPATH, "//button[@data-js='remove_pinned_message_button']")
+            unpin_bttn = self.browser.find_element(
+                By.XPATH,
+                "//button[@data-js='remove_pinned_message_button']"
+                )
+
         except selenium.common.exceptions.NoSuchElementException:
             return False #No message was pinned
 
         unpin_bttn.click()
         return True
 
     def quit(self):
         """Shut down everything"""
+        self.keep_running = False
         self.browser.quit()
         # TODO how to close an SSEClient?
         # self.ssechat.client.close()
 
     def __run_if_command(self, message):
         """Check if a message is a command, and run it if so"""
         #Not a command
@@ -332,15 +472,16 @@
 
         self.chat_commands[name].call(message)
 
     def register_command(self, command, name = None):
         """Register a command"""
         #Is a ChatCommand instance
         if isinstance(command, ChatCommand):
-            assert not name or name == command.name, "ChatCommand instance has different name than one passed"
+            assert not name or name == command.name, \
+                "ChatCommand instance has different name than one passed"
             self.chat_commands[command.name] = command
 
         #Is a callable
         elif callable(command):
             assert name, "Name cannot be None if command is a callable"
             assert " " not in name, "Name cannot contain spaces"
             self.chat_commands[name] = ChatCommand(name = name, actor = self, target = command)
@@ -351,20 +492,29 @@
     - Action should return True if the message survived the action
     - Action should return False if the message was deleted by the action"""
         assert callable(action), "Action must be a callable"
         self.message_actions.append(action)
 
     def __process_message(self, message):
         """Process a single SSE Chat message"""
-        #Do not do anything with the message if it matches one we sent before
+        #Ignore messages that match ones we sent before
         if message.text in self.sent_messages:
             return
 
+        #If the message is from the same account as us, consider it in message send cooldown
+        if message.user.username == self.username:
+            self.last_message_send_time = max((self.last_message_send_time, message.time))
+
+        #Ignore messages that are in the ignore_users list
+        if message.user.username in self.ignore_users:
+            return
+
         for action in self.message_actions:
-            if message.message_id in self.ssechat.deleted_message_ids or not action(message, self): #The message got deleted, possibly by this action
+            #The message got deleted, possibly by this action
+            if message.message_id in self.ssechat.deleted_message_ids or not action(message, self):
                 return
 
         self.__run_if_command(message)
 
     def mainloop(self):
         """Run the actor forever"""
         while self.keep_running:
```

### Comparing `rumchat_actor-1.0.1/LICENSE.txt` & `rumchat_actor-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rumchat_actor-1.0.1/README.md` & `rumchat_actor-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `rumchat_actor-1.0.1/pyproject.toml` & `rumchat_actor-1.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "rumchat_actor"
-version = "1.0.1"
+version = "1.1.0"
 keywords = ["rumble", "chat", "livestream", "bot"]
 authors = [
   { name="Wilbur Jaywright", email="zargulthewizard@outlook.com" },
 ]
 description = "Automatically interact with your Rumble livestream chats."
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
+  "browsermobproxy",
   "cocorum>=1.0.0",
+  "moviepy",
+  "requests",
   "selenium",
+  "talkey",
   ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Affero General Public License v3",
     "Operating System :: OS Independent",
     "Development Status :: 4 - Beta",
 ]
```

### Comparing `rumchat_actor-1.0.1/PKG-INFO` & `rumchat_actor-1.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.3
 Name: rumchat_actor
-Version: 1.0.1
+Version: 1.1.0
 Summary: Automatically interact with your Rumble livestream chats.
 Project-URL: Homepage, https://github.com/thelabcat/rum-chat-actor
 Project-URL: Issues, https://github.com/thelabcat/rumble-api-wrapper-py/issues
 Author-email: Wilbur Jaywright <zargulthewizard@outlook.com>
 License-File: LICENSE.txt
 Keywords: bot,chat,livestream,rumble
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
+Requires-Dist: browsermobproxy
 Requires-Dist: cocorum>=1.0.0
+Requires-Dist: moviepy
+Requires-Dist: requests
 Requires-Dist: selenium
+Requires-Dist: talkey
 Description-Content-Type: text/markdown
 
 # Rumble Chat Actor
 Automatically interact with your Rumble livestream chats.
 
 This project requires the following python libraries:
 - [Cocorum](https://pypi.org/project/cocorum/)
```

