# Comparing `tmp/discordproxy-1.3.1.tar.gz` & `tmp/discordproxy-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discordproxy-1.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "discordproxy-1.3.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `discordproxy-1.3.1.tar` & `discordproxy-1.3.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1070 2023-08-01 21:31:12.819419 discordproxy-1.3.1/LICENSE
--rw-r--r--   0        0        0     1890 2023-08-01 21:31:12.819419 discordproxy-1.3.1/README.md
--rw-r--r--   0        0        0      110 2023-08-01 21:31:12.819419 discordproxy-1.3.1/discordproxy/__init__.py
--rw-r--r--   0        0        0     6096 2023-08-01 21:31:12.819419 discordproxy-1.3.1/discordproxy/_api.py
--rw-r--r--   0        0        0     2003 2023-08-01 21:31:12.819419 discordproxy-1.3.1/discordproxy/_cli.py
--rw-r--r--   0        0        0     3855 2023-08-01 21:31:12.819419 discordproxy-1.3.1/discordproxy/_config.py
--rw-r--r--   0        0        0       90 2023-08-01 21:31:12.819419 discordproxy-1.3.1/discordproxy/_constants.py
--rw-r--r--   0        0        0     2940 2023-08-01 21:31:12.819419 discordproxy-1.3.1/discordproxy/_decorators.py
--rw-r--r--   0        0        0      630 2023-08-01 21:31:12.819419 discordproxy-1.3.1/discordproxy/_discord_client.py
--rw-r--r--   0        0        0     3637 2023-08-01 21:31:12.819419 discordproxy-1.3.1/discordproxy/_server.py
--rw-r--r--   0        0        0     4087 2023-08-01 21:31:12.819419 discordproxy-1.3.1/discordproxy/client.py
--rw-r--r--   0        0        0    24933 2023-08-01 21:31:12.823420 discordproxy-1.3.1/discordproxy/discord_api_pb2.py
--rw-r--r--   0        0        0     5883 2023-08-01 21:31:12.823420 discordproxy-1.3.1/discordproxy/discord_api_pb2_grpc.py
--rw-r--r--   0        0        0     2780 2023-08-01 21:31:12.823420 discordproxy-1.3.1/discordproxy/exceptions.py
--rw-r--r--   0        0        0      733 2023-08-01 21:31:12.823420 discordproxy-1.3.1/discordproxy/helpers.py
--rw-r--r--   0        0        0        0 2023-08-01 21:49:47.819238 discordproxy-1.3.1/discordproxy/tests/__init__.py
--rw-r--r--   0        0        0      930 2023-08-01 21:31:12.823420 discordproxy-1.3.1/discordproxy/tests/factories.py
--rw-r--r--   0        0        0      841 2023-08-01 21:31:12.823420 discordproxy-1.3.1/discordproxy/tests/helpers.py
--rw-r--r--   0        0        0     8290 2023-08-01 21:31:12.823420 discordproxy-1.3.1/discordproxy/tests/stubs.py
--rw-r--r--   0        0        0     6732 2023-08-01 21:31:12.823420 discordproxy-1.3.1/discordproxy/tests/test_api.py
--rw-r--r--   0        0        0     1551 2023-08-01 21:31:12.823420 discordproxy-1.3.1/discordproxy/tests/test_cli.py
--rw-r--r--   0        0        0     4501 2023-08-01 21:31:12.823420 discordproxy-1.3.1/discordproxy/tests/test_client.py
--rw-r--r--   0        0        0     2018 2023-08-01 21:31:12.823420 discordproxy-1.3.1/discordproxy/tests/test_config.py
--rw-r--r--   0        0        0     1905 2023-08-01 21:31:12.823420 discordproxy-1.3.1/discordproxy/tests/test_end2end.py
--rw-r--r--   0        0        0     2556 2023-08-01 21:31:12.823420 discordproxy-1.3.1/discordproxy/tests/test_exceptions.py
--rw-r--r--   0        0        0     1073 2023-08-01 21:31:12.823420 discordproxy-1.3.1/discordproxy/tests/test_helpers.py
--rw-r--r--   0        0        0     1886 2023-08-01 21:31:12.823420 discordproxy-1.3.1/discordproxy/tests/test_server.py
--rw-r--r--   0        0        0     1411 2023-08-01 21:31:12.827420 discordproxy-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     2743 1970-01-01 00:00:00.000000 discordproxy-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-29 14:16:52.177131 discordproxy-1.3.2/LICENSE
+-rw-r--r--   0        0        0     1890 2021-03-13 18:29:37.317667 discordproxy-1.3.2/README.md
+-rw-r--r--   0        0        0      110 2024-05-10 19:42:59.318707 discordproxy-1.3.2/discordproxy/__init__.py
+-rw-r--r--   0        0        0     6136 2024-05-10 19:42:59.318707 discordproxy-1.3.2/discordproxy/_api.py
+-rw-r--r--   0        0        0     2003 2023-08-01 21:30:13.108525 discordproxy-1.3.2/discordproxy/_cli.py
+-rw-r--r--   0        0        0     3855 2023-08-01 21:30:13.108525 discordproxy-1.3.2/discordproxy/_config.py
+-rw-r--r--   0        0        0       90 2023-08-01 21:30:13.108525 discordproxy-1.3.2/discordproxy/_constants.py
+-rw-r--r--   0        0        0     2940 2023-08-01 21:30:13.108525 discordproxy-1.3.2/discordproxy/_decorators.py
+-rw-r--r--   0        0        0      630 2023-08-01 21:30:13.108525 discordproxy-1.3.2/discordproxy/_discord_client.py
+-rw-r--r--   0        0        0     3637 2023-08-01 21:30:13.108525 discordproxy-1.3.2/discordproxy/_server.py
+-rw-r--r--   0        0        0     4477 2024-05-10 19:58:24.115976 discordproxy-1.3.2/discordproxy/client.py
+-rw-r--r--   0        0        0    24961 2024-05-10 19:42:59.318707 discordproxy-1.3.2/discordproxy/discord_api_pb2.py
+-rw-r--r--   0        0        0     5883 2023-06-22 14:14:27.248149 discordproxy-1.3.2/discordproxy/discord_api_pb2_grpc.py
+-rw-r--r--   0        0        0     2780 2023-08-01 21:30:13.108525 discordproxy-1.3.2/discordproxy/exceptions.py
+-rw-r--r--   0        0        0      733 2023-08-01 21:30:13.108525 discordproxy-1.3.2/discordproxy/helpers.py
+-rw-r--r--   0        0        0        0 2024-05-10 20:23:11.471144 discordproxy-1.3.2/discordproxy/tests/__init__.py
+-rw-r--r--   0        0        0      930 2023-08-01 21:30:13.112526 discordproxy-1.3.2/discordproxy/tests/factories.py
+-rw-r--r--   0        0        0      841 2023-08-01 21:30:13.112526 discordproxy-1.3.2/discordproxy/tests/helpers.py
+-rw-r--r--   0        0        0     8290 2023-08-01 21:30:13.112526 discordproxy-1.3.2/discordproxy/tests/stubs.py
+-rw-r--r--   0        0        0     6732 2023-08-01 21:30:13.112526 discordproxy-1.3.2/discordproxy/tests/test_api.py
+-rw-r--r--   0        0        0     1551 2023-08-01 21:30:13.112526 discordproxy-1.3.2/discordproxy/tests/test_cli.py
+-rw-r--r--   0        0        0     5085 2024-05-10 20:11:58.247032 discordproxy-1.3.2/discordproxy/tests/test_client.py
+-rw-r--r--   0        0        0     2018 2023-08-01 21:30:13.112526 discordproxy-1.3.2/discordproxy/tests/test_config.py
+-rw-r--r--   0        0        0     3763 2023-12-04 20:38:06.859903 discordproxy-1.3.2/discordproxy/tests/test_end2end.py
+-rw-r--r--   0        0        0     2556 2023-08-01 21:30:13.116526 discordproxy-1.3.2/discordproxy/tests/test_exceptions.py
+-rw-r--r--   0        0        0     1073 2023-08-01 21:30:13.116526 discordproxy-1.3.2/discordproxy/tests/test_helpers.py
+-rw-r--r--   0        0        0     1886 2023-08-01 21:30:13.116526 discordproxy-1.3.2/discordproxy/tests/test_server.py
+-rw-r--r--   0        0        0     1411 2023-08-01 21:30:13.116526 discordproxy-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2743 1970-01-01 00:00:00.000000 discordproxy-1.3.2/PKG-INFO
```

### Comparing `discordproxy-1.3.1/LICENSE` & `discordproxy-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `discordproxy-1.3.1/README.md` & `discordproxy-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `discordproxy-1.3.1/discordproxy/_api.py` & `discordproxy-1.3.2/discordproxy/_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,17 +52,19 @@
         system=message.author.system,
     )
     if isinstance(message.author, discord.Member):
         member = discord_api_pb2.GuildMember(
             user=author,
             nick=message.author.nick,
             roles=[obj.id for obj in message.author.roles],
-            joined_at=message.author.joined_at.isoformat()
-            if message.author.joined_at
-            else None,
+            joined_at=(
+                message.author.joined_at.isoformat()
+                if message.author.joined_at
+                else None
+            ),
             # permissions=message.author.permissions.value, TODO
         )
     else:
         member = None
     return discord_api_pb2.Message(
         id=message.id,
         channel_id=message.channel.id if message.channel else None,
```

### Comparing `discordproxy-1.3.1/discordproxy/_cli.py` & `discordproxy-1.3.2/discordproxy/_cli.py`

 * *Files identical despite different names*

### Comparing `discordproxy-1.3.1/discordproxy/_config.py` & `discordproxy-1.3.2/discordproxy/_config.py`

 * *Files identical despite different names*

### Comparing `discordproxy-1.3.1/discordproxy/_decorators.py` & `discordproxy-1.3.2/discordproxy/_decorators.py`

 * *Files identical despite different names*

### Comparing `discordproxy-1.3.1/discordproxy/_discord_client.py` & `discordproxy-1.3.2/discordproxy/_discord_client.py`

 * *Files identical despite different names*

### Comparing `discordproxy-1.3.1/discordproxy/_server.py` & `discordproxy-1.3.2/discordproxy/_server.py`

 * *Files identical despite different names*

### Comparing `discordproxy-1.3.1/discordproxy/client.py` & `discordproxy-1.3.2/discordproxy/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -33,14 +33,29 @@
             timeout: Default timeout for gRPC method invocations in seconds.
                 If not specified the timeout is about 30 minutes.
         """
         self._target = str(target) if target else "localhost:50051"
         self._options = options
         self._timeout = timeout
 
+    @property
+    def target(self) -> str:
+        """Return configured target for this client."""
+        return self._target
+
+    @property
+    def timeout(self) -> str:
+        """Return configured timeout for this client."""
+        return self._timeout
+
+    @property
+    def options(self) -> str:
+        """Return configured options for this client."""
+        return self._options
+
     def get_guild_channels(self, guild_id: int) -> Iterable[Channel]:
         """Get all channels.
 
         Args:
             guild_id: ID of guild to get the channel for
 
         Returns:
```

### Comparing `discordproxy-1.3.1/discordproxy/discord_api_pb2.py` & `discordproxy-1.3.2/discordproxy/discord_api_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,89 +57,89 @@
 _MESSAGE_STICKER_TYPE = _MESSAGE_STICKER.enum_types_by_name["Type"]
 _MESSAGE_TYPE = _MESSAGE.enum_types_by_name["Type"]
 Channel = _reflection.GeneratedProtocolMessageType(
     "Channel",
     (_message.Message,),
     {
         "DESCRIPTOR": _CHANNEL,
-        "__module__": "discord_api_pb2"
+        "__module__": "discord_api_pb2",
         # @@protoc_insertion_point(class_scope:discord_api.Channel)
     },
 )
 _sym_db.RegisterMessage(Channel)
 
 Embed = _reflection.GeneratedProtocolMessageType(
     "Embed",
     (_message.Message,),
     {
         "Footer": _reflection.GeneratedProtocolMessageType(
             "Footer",
             (_message.Message,),
             {
                 "DESCRIPTOR": _EMBED_FOOTER,
-                "__module__": "discord_api_pb2"
+                "__module__": "discord_api_pb2",
                 # @@protoc_insertion_point(class_scope:discord_api.Embed.Footer)
             },
         ),
         "Image": _reflection.GeneratedProtocolMessageType(
             "Image",
             (_message.Message,),
             {
                 "DESCRIPTOR": _EMBED_IMAGE,
-                "__module__": "discord_api_pb2"
+                "__module__": "discord_api_pb2",
                 # @@protoc_insertion_point(class_scope:discord_api.Embed.Image)
             },
         ),
         "Thumbnail": _reflection.GeneratedProtocolMessageType(
             "Thumbnail",
             (_message.Message,),
             {
                 "DESCRIPTOR": _EMBED_THUMBNAIL,
-                "__module__": "discord_api_pb2"
+                "__module__": "discord_api_pb2",
                 # @@protoc_insertion_point(class_scope:discord_api.Embed.Thumbnail)
             },
         ),
         "Video": _reflection.GeneratedProtocolMessageType(
             "Video",
             (_message.Message,),
             {
                 "DESCRIPTOR": _EMBED_VIDEO,
-                "__module__": "discord_api_pb2"
+                "__module__": "discord_api_pb2",
                 # @@protoc_insertion_point(class_scope:discord_api.Embed.Video)
             },
         ),
         "Provider": _reflection.GeneratedProtocolMessageType(
             "Provider",
             (_message.Message,),
             {
                 "DESCRIPTOR": _EMBED_PROVIDER,
-                "__module__": "discord_api_pb2"
+                "__module__": "discord_api_pb2",
                 # @@protoc_insertion_point(class_scope:discord_api.Embed.Provider)
             },
         ),
         "Author": _reflection.GeneratedProtocolMessageType(
             "Author",
             (_message.Message,),
             {
                 "DESCRIPTOR": _EMBED_AUTHOR,
-                "__module__": "discord_api_pb2"
+                "__module__": "discord_api_pb2",
                 # @@protoc_insertion_point(class_scope:discord_api.Embed.Author)
             },
         ),
         "Field": _reflection.GeneratedProtocolMessageType(
             "Field",
             (_message.Message,),
             {
                 "DESCRIPTOR": _EMBED_FIELD,
-                "__module__": "discord_api_pb2"
+                "__module__": "discord_api_pb2",
                 # @@protoc_insertion_point(class_scope:discord_api.Embed.Field)
             },
         ),
         "DESCRIPTOR": _EMBED,
-        "__module__": "discord_api_pb2"
+        "__module__": "discord_api_pb2",
         # @@protoc_insertion_point(class_scope:discord_api.Embed)
     },
 )
 _sym_db.RegisterMessage(Embed)
 _sym_db.RegisterMessage(Embed.Footer)
 _sym_db.RegisterMessage(Embed.Image)
 _sym_db.RegisterMessage(Embed.Thumbnail)
@@ -149,100 +149,100 @@
 _sym_db.RegisterMessage(Embed.Field)
 
 Emoji = _reflection.GeneratedProtocolMessageType(
     "Emoji",
     (_message.Message,),
     {
         "DESCRIPTOR": _EMOJI,
-        "__module__": "discord_api_pb2"
+        "__module__": "discord_api_pb2",
         # @@protoc_insertion_point(class_scope:discord_api.Emoji)
     },
 )
 _sym_db.RegisterMessage(Emoji)
 
 GuildMember = _reflection.GeneratedProtocolMessageType(
     "GuildMember",
     (_message.Message,),
     {
         "DESCRIPTOR": _GUILDMEMBER,
-        "__module__": "discord_api_pb2"
+        "__module__": "discord_api_pb2",
         # @@protoc_insertion_point(class_scope:discord_api.GuildMember)
     },
 )
 _sym_db.RegisterMessage(GuildMember)
 
 Message = _reflection.GeneratedProtocolMessageType(
     "Message",
     (_message.Message,),
     {
         "ChannelMention": _reflection.GeneratedProtocolMessageType(
             "ChannelMention",
             (_message.Message,),
             {
                 "DESCRIPTOR": _MESSAGE_CHANNELMENTION,
-                "__module__": "discord_api_pb2"
+                "__module__": "discord_api_pb2",
                 # @@protoc_insertion_point(class_scope:discord_api.Message.ChannelMention)
             },
         ),
         "Attachment": _reflection.GeneratedProtocolMessageType(
             "Attachment",
             (_message.Message,),
             {
                 "DESCRIPTOR": _MESSAGE_ATTACHMENT,
-                "__module__": "discord_api_pb2"
+                "__module__": "discord_api_pb2",
                 # @@protoc_insertion_point(class_scope:discord_api.Message.Attachment)
             },
         ),
         "Reaction": _reflection.GeneratedProtocolMessageType(
             "Reaction",
             (_message.Message,),
             {
                 "DESCRIPTOR": _MESSAGE_REACTION,
-                "__module__": "discord_api_pb2"
+                "__module__": "discord_api_pb2",
                 # @@protoc_insertion_point(class_scope:discord_api.Message.Reaction)
             },
         ),
         "Activity": _reflection.GeneratedProtocolMessageType(
             "Activity",
             (_message.Message,),
             {
                 "DESCRIPTOR": _MESSAGE_ACTIVITY,
-                "__module__": "discord_api_pb2"
+                "__module__": "discord_api_pb2",
                 # @@protoc_insertion_point(class_scope:discord_api.Message.Activity)
             },
         ),
         "Application": _reflection.GeneratedProtocolMessageType(
             "Application",
             (_message.Message,),
             {
                 "DESCRIPTOR": _MESSAGE_APPLICATION,
-                "__module__": "discord_api_pb2"
+                "__module__": "discord_api_pb2",
                 # @@protoc_insertion_point(class_scope:discord_api.Message.Application)
             },
         ),
         "Reference": _reflection.GeneratedProtocolMessageType(
             "Reference",
             (_message.Message,),
             {
                 "DESCRIPTOR": _MESSAGE_REFERENCE,
-                "__module__": "discord_api_pb2"
+                "__module__": "discord_api_pb2",
                 # @@protoc_insertion_point(class_scope:discord_api.Message.Reference)
             },
         ),
         "Sticker": _reflection.GeneratedProtocolMessageType(
             "Sticker",
             (_message.Message,),
             {
                 "DESCRIPTOR": _MESSAGE_STICKER,
-                "__module__": "discord_api_pb2"
+                "__module__": "discord_api_pb2",
                 # @@protoc_insertion_point(class_scope:discord_api.Message.Sticker)
             },
         ),
         "DESCRIPTOR": _MESSAGE,
-        "__module__": "discord_api_pb2"
+        "__module__": "discord_api_pb2",
         # @@protoc_insertion_point(class_scope:discord_api.Message)
     },
 )
 _sym_db.RegisterMessage(Message)
 _sym_db.RegisterMessage(Message.ChannelMention)
 _sym_db.RegisterMessage(Message.Attachment)
 _sym_db.RegisterMessage(Message.Reaction)
@@ -256,98 +256,98 @@
     (_message.Message,),
     {
         "Tag": _reflection.GeneratedProtocolMessageType(
             "Tag",
             (_message.Message,),
             {
                 "DESCRIPTOR": _ROLE_TAG,
-                "__module__": "discord_api_pb2"
+                "__module__": "discord_api_pb2",
                 # @@protoc_insertion_point(class_scope:discord_api.Role.Tag)
             },
         ),
         "DESCRIPTOR": _ROLE,
-        "__module__": "discord_api_pb2"
+        "__module__": "discord_api_pb2",
         # @@protoc_insertion_point(class_scope:discord_api.Role)
     },
 )
 _sym_db.RegisterMessage(Role)
 _sym_db.RegisterMessage(Role.Tag)
 
 User = _reflection.GeneratedProtocolMessageType(
     "User",
     (_message.Message,),
     {
         "DESCRIPTOR": _USER,
-        "__module__": "discord_api_pb2"
+        "__module__": "discord_api_pb2",
         # @@protoc_insertion_point(class_scope:discord_api.User)
     },
 )
 _sym_db.RegisterMessage(User)
 
 SendChannelMessageRequest = _reflection.GeneratedProtocolMessageType(
     "SendChannelMessageRequest",
     (_message.Message,),
     {
         "DESCRIPTOR": _SENDCHANNELMESSAGEREQUEST,
-        "__module__": "discord_api_pb2"
+        "__module__": "discord_api_pb2",
         # @@protoc_insertion_point(class_scope:discord_api.SendChannelMessageRequest)
     },
 )
 _sym_db.RegisterMessage(SendChannelMessageRequest)
 
 SendChannelMessageResponse = _reflection.GeneratedProtocolMessageType(
     "SendChannelMessageResponse",
     (_message.Message,),
     {
         "DESCRIPTOR": _SENDCHANNELMESSAGERESPONSE,
-        "__module__": "discord_api_pb2"
+        "__module__": "discord_api_pb2",
         # @@protoc_insertion_point(class_scope:discord_api.SendChannelMessageResponse)
     },
 )
 _sym_db.RegisterMessage(SendChannelMessageResponse)
 
 SendDirectMessageRequest = _reflection.GeneratedProtocolMessageType(
     "SendDirectMessageRequest",
     (_message.Message,),
     {
         "DESCRIPTOR": _SENDDIRECTMESSAGEREQUEST,
-        "__module__": "discord_api_pb2"
+        "__module__": "discord_api_pb2",
         # @@protoc_insertion_point(class_scope:discord_api.SendDirectMessageRequest)
     },
 )
 _sym_db.RegisterMessage(SendDirectMessageRequest)
 
 SendDirectMessageResponse = _reflection.GeneratedProtocolMessageType(
     "SendDirectMessageResponse",
     (_message.Message,),
     {
         "DESCRIPTOR": _SENDDIRECTMESSAGERESPONSE,
-        "__module__": "discord_api_pb2"
+        "__module__": "discord_api_pb2",
         # @@protoc_insertion_point(class_scope:discord_api.SendDirectMessageResponse)
     },
 )
 _sym_db.RegisterMessage(SendDirectMessageResponse)
 
 GetGuildChannelsRequest = _reflection.GeneratedProtocolMessageType(
     "GetGuildChannelsRequest",
     (_message.Message,),
     {
         "DESCRIPTOR": _GETGUILDCHANNELSREQUEST,
-        "__module__": "discord_api_pb2"
+        "__module__": "discord_api_pb2",
         # @@protoc_insertion_point(class_scope:discord_api.GetGuildChannelsRequest)
     },
 )
 _sym_db.RegisterMessage(GetGuildChannelsRequest)
 
 GetGuildChannelsResponse = _reflection.GeneratedProtocolMessageType(
     "GetGuildChannelsResponse",
     (_message.Message,),
     {
         "DESCRIPTOR": _GETGUILDCHANNELSRESPONSE,
-        "__module__": "discord_api_pb2"
+        "__module__": "discord_api_pb2",
         # @@protoc_insertion_point(class_scope:discord_api.GetGuildChannelsResponse)
     },
 )
 _sym_db.RegisterMessage(GetGuildChannelsResponse)
 
 _DISCORDAPI = DESCRIPTOR.services_by_name["DiscordApi"]
 if _descriptor._USE_C_DESCRIPTORS == False:
```

### Comparing `discordproxy-1.3.1/discordproxy/discord_api_pb2_grpc.py` & `discordproxy-1.3.2/discordproxy/discord_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `discordproxy-1.3.1/discordproxy/exceptions.py` & `discordproxy-1.3.2/discordproxy/exceptions.py`

 * *Files identical despite different names*

### Comparing `discordproxy-1.3.1/discordproxy/helpers.py` & `discordproxy-1.3.2/discordproxy/helpers.py`

 * *Files identical despite different names*

### Comparing `discordproxy-1.3.1/discordproxy/tests/factories.py` & `discordproxy-1.3.2/discordproxy/tests/factories.py`

 * *Files identical despite different names*

### Comparing `discordproxy-1.3.1/discordproxy/tests/helpers.py` & `discordproxy-1.3.2/discordproxy/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `discordproxy-1.3.1/discordproxy/tests/stubs.py` & `discordproxy-1.3.2/discordproxy/tests/stubs.py`

 * *Files identical despite different names*

### Comparing `discordproxy-1.3.1/discordproxy/tests/test_api.py` & `discordproxy-1.3.2/discordproxy/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `discordproxy-1.3.1/discordproxy/tests/test_cli.py` & `discordproxy-1.3.2/discordproxy/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `discordproxy-1.3.1/discordproxy/tests/test_client.py` & `discordproxy-1.3.2/discordproxy/tests/test_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,32 @@
 
 from .factories import create_discordproxy_channel, create_rpc_error
 from .helpers import NoSocketsTestCase
 
 MODULE_PATH = "discordproxy.client"
 
 
+class TestDiscordClient(NoSocketsTestCase):
+    def test_should_return_new_config(self):
+        # when
+        c = DiscordClient(target="1.2.3.4:56789", options={"alpha": "one"}, timeout=42)
+        # then
+        self.assertEqual(c.target, "1.2.3.4:56789")
+        self.assertEqual(c.options, {"alpha": "one"})
+        self.assertEqual(c.timeout, 42)
+
+    def test_should_return_default(self):
+        # when
+        c = DiscordClient()
+        # then
+        self.assertEqual(c.target, "localhost:50051")
+        self.assertIsNone(c.options)
+        self.assertIsNone(c.timeout)
+
+
 @patch(MODULE_PATH + ".DiscordApiStub")
 @patch(MODULE_PATH + ".grpc.insecure_channel", spec=True)
 class TestFetchChannels(NoSocketsTestCase):
     def test_should_return_text_channels(
         self, mock_insecure_channel, mock_DiscordApiStub
     ):
         # given
```

### Comparing `discordproxy-1.3.1/discordproxy/tests/test_config.py` & `discordproxy-1.3.2/discordproxy/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `discordproxy-1.3.1/discordproxy/tests/test_end2end.py` & `discordproxy-1.3.2/discordproxy/tests/test_end2end.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,16 +3,20 @@
 from collections import namedtuple
 from pathlib import Path
 from unittest import IsolatedAsyncioTestCase
 
 import grpc
 
 from discordproxy._server import _shutdown_server, run_server
-from discordproxy.discord_api_pb2 import SendDirectMessageRequest
+from discordproxy.discord_api_pb2 import (
+    SendChannelMessageRequest,
+    SendDirectMessageRequest,
+)
 from discordproxy.discord_api_pb2_grpc import DiscordApiStub
+from discordproxy.exceptions import DiscordProxyHttpError, to_discord_proxy_exception
 
 from .stubs import DiscordClientStub
 
 MyArgsStub = namedtuple("MyArgsStub", ["host", "port"])
 
 logging.basicConfig(
     filename=Path(__file__).with_suffix(".log"),
@@ -23,14 +27,15 @@
 logger.setLevel(logging.DEBUG)
 
 
 class TestEnd2End(IsolatedAsyncioTestCase):
     async def asyncSetUp(self) -> None:
         self.host = "localhost"
         self.port = 50051
+        self.target = f"{self.host}:{self.port}"
         token = "dummy"
         my_args = MyArgsStub(host=self.host, port=self.port)
         self.grpc_server = grpc.aio.server()
         self.discord_client = DiscordClientStub()
         asyncio.create_task(
             run_server(
                 token=token,
@@ -42,17 +47,52 @@
         await asyncio.sleep(1)
 
     async def asyncTearDown(self) -> None:
         await _shutdown_server(
             grpc_server=self.grpc_server, discord_client=self.discord_client
         )
 
-    async def test_should_send_message_to_server(self):
+    async def test_should_send_direct_message_to_server(self):
         # given
-        channel = grpc.aio.insecure_channel(f"{self.host}:{self.port}")
-        client = DiscordApiStub(channel)
-        request = SendDirectMessageRequest(user_id=1001, content="content")
-        # when
-        response = await client.SendDirectMessage(request, timeout=5)
+        async with grpc.aio.insecure_channel(self.target) as grpc_channel:
+            client = DiscordApiStub(grpc_channel)
+            request = SendDirectMessageRequest(user_id=1001, content="content")
+            # when
+            response = await client.SendDirectMessage(request, timeout=5)
         # then
         self.assertEqual(response.message.channel_id, 2010)
         self.assertEqual(response.message.content, "content")
+
+    async def test_should_send_direct_message_to_channel(self):
+        # given
+        async with grpc.aio.insecure_channel(self.target) as grpc_channel:
+            client = DiscordApiStub(grpc_channel)
+            request = SendChannelMessageRequest(channel_id=2001, content="content")
+            # when
+            response = await client.SendChannelMessage(request, timeout=5)
+        # then
+        self.assertEqual(response.message.channel_id, 2001)
+        self.assertEqual(response.message.content, "content")
+
+    async def test_should_raise_http_exception_when_not_found(self):
+        # given
+        async with grpc.aio.insecure_channel(self.target) as grpc_channel:
+            client = DiscordApiStub(grpc_channel)
+            request = SendDirectMessageRequest(user_id=1234, content="content")
+            # when/then
+            try:
+                await client.SendDirectMessage(request, timeout=5)
+            except Exception as ex:
+                with self.assertRaises(DiscordProxyHttpError):
+                    raise to_discord_proxy_exception(ex) from ex
+
+    async def test_should_raise_http_exception_when_forbidden(self):
+        # given
+        async with grpc.aio.insecure_channel(self.target) as grpc_channel:
+            client = DiscordApiStub(grpc_channel)
+            request = SendChannelMessageRequest(channel_id=2100, content="content")
+            # when/then
+            try:
+                await client.SendChannelMessage(request, timeout=5)
+            except Exception as ex:
+                with self.assertRaises(DiscordProxyHttpError):
+                    raise to_discord_proxy_exception(ex) from ex
```

### Comparing `discordproxy-1.3.1/discordproxy/tests/test_exceptions.py` & `discordproxy-1.3.2/discordproxy/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `discordproxy-1.3.1/discordproxy/tests/test_helpers.py` & `discordproxy-1.3.2/discordproxy/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `discordproxy-1.3.1/discordproxy/tests/test_server.py` & `discordproxy-1.3.2/discordproxy/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `discordproxy-1.3.1/pyproject.toml` & `discordproxy-1.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `discordproxy-1.3.1/PKG-INFO` & `discordproxy-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discordproxy
-Version: 1.3.1
+Version: 1.3.2
 Summary: Proxy server for accessing the Discord API via gRPC.
 Author-email: Erik Kalkoken <kalkoken87@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

