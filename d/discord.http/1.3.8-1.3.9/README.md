# Comparing `tmp/discord.http-1.3.8.tar.gz` & `tmp/discord.http-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord.http-1.3.8.tar", last modified: Fri Mar 22 12:59:46 2024, max compression
+gzip compressed data, was "discord.http-1.3.9.tar", last modified: Mon Mar 25 13:06:10 2024, max compression
```

## Comparing `discord.http-1.3.8.tar` & `discord.http-1.3.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-03-22 12:59:46.289477 discord.http-1.3.8/
--rw-rw-rw-   0        0        0     1082 2023-04-19 13:35:24.000000 discord.http-1.3.8/LICENSE
--rw-rw-rw-   0        0        0     2377 2024-03-22 12:59:46.288429 discord.http-1.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     1498 2023-11-14 19:21:06.000000 discord.http-1.3.8/README.md
-drwxrwxrwx   0        0        0        0 2024-03-22 12:59:46.286878 discord.http-1.3.8/discord.http.egg-info/
--rw-rw-rw-   0        0        0     2377 2024-03-22 12:59:46.000000 discord.http-1.3.8/discord.http.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      954 2024-03-22 12:59:46.000000 discord.http-1.3.8/discord.http.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-22 12:59:46.000000 discord.http-1.3.8/discord.http.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-03-22 12:59:46.000000 discord.http-1.3.8/discord.http.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-03-22 12:59:46.000000 discord.http-1.3.8/discord.http.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-22 12:59:46.285849 discord.http-1.3.8/discord_http/
--rw-rw-rw-   0        0        0      745 2024-03-22 07:51:01.000000 discord.http-1.3.8/discord_http/__init__.py
--rw-rw-rw-   0        0        0     1253 2024-01-19 12:33:13.000000 discord.http-1.3.8/discord_http/__main__.py
--rw-rw-rw-   0        0        0     4593 2024-03-12 11:43:15.000000 discord.http-1.3.8/discord_http/asset.py
--rw-rw-rw-   0        0        0    16468 2024-03-22 10:20:43.000000 discord.http-1.3.8/discord_http/backend.py
--rw-rw-rw-   0        0        0    54720 2024-03-13 13:29:54.000000 discord.http-1.3.8/discord_http/channel.py
--rw-rw-rw-   0        0        0    38434 2024-03-22 07:54:03.000000 discord.http-1.3.8/discord_http/client.py
--rw-rw-rw-   0        0        0     3492 2023-12-15 13:16:47.000000 discord.http-1.3.8/discord_http/colour.py
--rw-rw-rw-   0        0        0    41745 2024-03-22 12:54:23.000000 discord.http-1.3.8/discord_http/commands.py
--rw-rw-rw-   0        0        0    26891 2024-03-15 15:34:56.000000 discord.http-1.3.8/discord_http/context.py
--rw-rw-rw-   0        0        0     8999 2024-03-15 10:24:13.000000 discord.http-1.3.8/discord_http/embeds.py
--rw-rw-rw-   0        0        0     7592 2024-03-06 13:21:30.000000 discord.http-1.3.8/discord_http/emoji.py
--rw-rw-rw-   0        0        0     4864 2024-02-21 10:15:18.000000 discord.http-1.3.8/discord_http/entitlements.py
--rw-rw-rw-   0        0        0     5395 2024-03-12 11:56:05.000000 discord.http-1.3.8/discord_http/enums.py
--rw-rw-rw-   0        0        0     2191 2023-12-15 13:17:01.000000 discord.http-1.3.8/discord_http/errors.py
--rw-rw-rw-   0        0        0     2133 2023-12-07 10:59:15.000000 discord.http-1.3.8/discord_http/file.py
--rw-rw-rw-   0        0        0     8980 2024-02-21 10:16:32.000000 discord.http-1.3.8/discord_http/flag.py
--rw-rw-rw-   0        0        0    59269 2024-03-21 13:35:40.000000 discord.http-1.3.8/discord_http/guild.py
--rw-rw-rw-   0        0        0    15064 2024-02-21 12:28:14.000000 discord.http-1.3.8/discord_http/http.py
--rw-rw-rw-   0        0        0     3455 2024-02-20 15:20:30.000000 discord.http-1.3.8/discord_http/invite.py
--rw-rw-rw-   0        0        0    16242 2024-03-13 14:26:21.000000 discord.http-1.3.8/discord_http/member.py
--rw-rw-rw-   0        0        0     1724 2024-02-21 10:16:01.000000 discord.http-1.3.8/discord_http/mentions.py
--rw-rw-rw-   0        0        0    28106 2024-03-18 13:21:33.000000 discord.http-1.3.8/discord_http/message.py
--rw-rw-rw-   0        0        0     2635 2024-03-13 13:59:28.000000 discord.http-1.3.8/discord_http/multipart.py
--rw-rw-rw-   0        0        0     3190 2024-02-21 12:26:35.000000 discord.http-1.3.8/discord_http/object.py
--rw-rw-rw-   0        0        0     9342 2024-02-21 12:42:36.000000 discord.http-1.3.8/discord_http/response.py
--rw-rw-rw-   0        0        0     9025 2024-02-12 12:58:34.000000 discord.http-1.3.8/discord_http/role.py
--rw-rw-rw-   0        0        0     7435 2024-02-23 13:11:04.000000 discord.http-1.3.8/discord_http/sticker.py
--rw-rw-rw-   0        0        0    16479 2024-02-21 10:01:55.000000 discord.http-1.3.8/discord_http/tasks.py
--rw-rw-rw-   0        0        0     6411 2024-03-15 14:14:41.000000 discord.http-1.3.8/discord_http/user.py
--rw-rw-rw-   0        0        0    15504 2024-03-22 12:42:00.000000 discord.http-1.3.8/discord_http/utils.py
--rw-rw-rw-   0        0        0    25263 2024-03-07 11:25:28.000000 discord.http-1.3.8/discord_http/view.py
--rw-rw-rw-   0        0        0    11221 2024-03-15 11:52:16.000000 discord.http-1.3.8/discord_http/webhook.py
--rw-rw-rw-   0        0        0     1525 2023-12-01 14:35:12.000000 discord.http-1.3.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-22 12:59:46.289996 discord.http-1.3.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-03-25 13:06:10.326331 discord.http-1.3.9/
+-rw-rw-rw-   0        0        0     1082 2023-04-19 13:35:24.000000 discord.http-1.3.9/LICENSE
+-rw-rw-rw-   0        0        0     2377 2024-03-25 13:06:10.325297 discord.http-1.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1498 2023-11-14 19:21:06.000000 discord.http-1.3.9/README.md
+drwxrwxrwx   0        0        0        0 2024-03-25 13:06:10.323754 discord.http-1.3.9/discord.http.egg-info/
+-rw-rw-rw-   0        0        0     2377 2024-03-25 13:06:10.000000 discord.http-1.3.9/discord.http.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      954 2024-03-25 13:06:10.000000 discord.http-1.3.9/discord.http.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-25 13:06:10.000000 discord.http-1.3.9/discord.http.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-03-25 13:06:10.000000 discord.http-1.3.9/discord.http.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-03-25 13:06:10.000000 discord.http-1.3.9/discord.http.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-25 13:06:10.322724 discord.http-1.3.9/discord_http/
+-rw-rw-rw-   0        0        0      745 2024-03-25 11:57:53.000000 discord.http-1.3.9/discord_http/__init__.py
+-rw-rw-rw-   0        0        0     1253 2024-01-19 12:33:13.000000 discord.http-1.3.9/discord_http/__main__.py
+-rw-rw-rw-   0        0        0     4593 2024-03-12 11:43:15.000000 discord.http-1.3.9/discord_http/asset.py
+-rw-rw-rw-   0        0        0    16468 2024-03-22 10:20:43.000000 discord.http-1.3.9/discord_http/backend.py
+-rw-rw-rw-   0        0        0    54720 2024-03-25 12:57:20.000000 discord.http-1.3.9/discord_http/channel.py
+-rw-rw-rw-   0        0        0    38434 2024-03-25 12:29:52.000000 discord.http-1.3.9/discord_http/client.py
+-rw-rw-rw-   0        0        0     3492 2023-12-15 13:16:47.000000 discord.http-1.3.9/discord_http/colour.py
+-rw-rw-rw-   0        0        0    43576 2024-03-25 13:03:57.000000 discord.http-1.3.9/discord_http/commands.py
+-rw-rw-rw-   0        0        0    27122 2024-03-25 12:57:36.000000 discord.http-1.3.9/discord_http/context.py
+-rw-rw-rw-   0        0        0     9001 2024-03-25 12:56:58.000000 discord.http-1.3.9/discord_http/embeds.py
+-rw-rw-rw-   0        0        0     7596 2024-03-25 12:57:41.000000 discord.http-1.3.9/discord_http/emoji.py
+-rw-rw-rw-   0        0        0     4864 2024-02-21 10:15:18.000000 discord.http-1.3.9/discord_http/entitlements.py
+-rw-rw-rw-   0        0        0     5395 2024-03-12 11:56:05.000000 discord.http-1.3.9/discord_http/enums.py
+-rw-rw-rw-   0        0        0     2191 2023-12-15 13:17:01.000000 discord.http-1.3.9/discord_http/errors.py
+-rw-rw-rw-   0        0        0     2133 2023-12-07 10:59:15.000000 discord.http-1.3.9/discord_http/file.py
+-rw-rw-rw-   0        0        0     8980 2024-02-21 10:16:32.000000 discord.http-1.3.9/discord_http/flag.py
+-rw-rw-rw-   0        0        0    59269 2024-03-21 13:35:40.000000 discord.http-1.3.9/discord_http/guild.py
+-rw-rw-rw-   0        0        0    15064 2024-02-21 12:28:14.000000 discord.http-1.3.9/discord_http/http.py
+-rw-rw-rw-   0        0        0     3455 2024-02-20 15:20:30.000000 discord.http-1.3.9/discord_http/invite.py
+-rw-rw-rw-   0        0        0    16242 2024-03-13 14:26:21.000000 discord.http-1.3.9/discord_http/member.py
+-rw-rw-rw-   0        0        0     1724 2024-02-21 10:16:01.000000 discord.http-1.3.9/discord_http/mentions.py
+-rw-rw-rw-   0        0        0    28106 2024-03-18 13:21:33.000000 discord.http-1.3.9/discord_http/message.py
+-rw-rw-rw-   0        0        0     2802 2024-03-25 11:58:20.000000 discord.http-1.3.9/discord_http/multipart.py
+-rw-rw-rw-   0        0        0     3190 2024-02-21 12:26:35.000000 discord.http-1.3.9/discord_http/object.py
+-rw-rw-rw-   0        0        0     9342 2024-02-21 12:42:36.000000 discord.http-1.3.9/discord_http/response.py
+-rw-rw-rw-   0        0        0     9025 2024-02-12 12:58:34.000000 discord.http-1.3.9/discord_http/role.py
+-rw-rw-rw-   0        0        0     7435 2024-02-23 13:11:04.000000 discord.http-1.3.9/discord_http/sticker.py
+-rw-rw-rw-   0        0        0    16479 2024-02-21 10:01:55.000000 discord.http-1.3.9/discord_http/tasks.py
+-rw-rw-rw-   0        0        0     6411 2024-03-15 14:14:41.000000 discord.http-1.3.9/discord_http/user.py
+-rw-rw-rw-   0        0        0    15504 2024-03-22 12:42:00.000000 discord.http-1.3.9/discord_http/utils.py
+-rw-rw-rw-   0        0        0    25364 2024-03-25 13:05:04.000000 discord.http-1.3.9/discord_http/view.py
+-rw-rw-rw-   0        0        0    11221 2024-03-15 11:52:16.000000 discord.http-1.3.9/discord_http/webhook.py
+-rw-rw-rw-   0        0        0     1525 2023-12-01 14:35:12.000000 discord.http-1.3.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-03-25 13:06:10.326331 discord.http-1.3.9/setup.cfg
```

### Comparing `discord.http-1.3.8/LICENSE` & `discord.http-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `discord.http-1.3.8/PKG-INFO` & `discord.http-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord.http
-Version: 1.3.8
+Version: 1.3.9
 Summary: Python library that handles interactions from Discord POST requests.
 Author-email: AlexFlipnote <root@alexflipnote.dev>
 License: MIT
 Keywords: discord,http,api,interaction,quart,webhook,slash
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `discord.http-1.3.8/README.md` & `discord.http-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `discord.http-1.3.8/discord.http.egg-info/PKG-INFO` & `discord.http-1.3.9/discord.http.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord.http
-Version: 1.3.8
+Version: 1.3.9
 Summary: Python library that handles interactions from Discord POST requests.
 Author-email: AlexFlipnote <root@alexflipnote.dev>
 License: MIT
 Keywords: discord,http,api,interaction,quart,webhook,slash
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `discord.http-1.3.8/discord.http.egg-info/SOURCES.txt` & `discord.http-1.3.9/discord.http.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discord.http-1.3.8/discord_http/__init__.py` & `discord.http-1.3.9/discord_http/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.3.8"
+__version__ = "1.3.9"
 
 # flake8: noqa: F401
 from .asset import *
 from .backend import *
 from .channel import *
 from .client import *
 from .colour import *
```

### Comparing `discord.http-1.3.8/discord_http/__main__.py` & `discord.http-1.3.9/discord_http/__main__.py`

 * *Files identical despite different names*

### Comparing `discord.http-1.3.8/discord_http/asset.py` & `discord.http-1.3.9/discord_http/asset.py`

 * *Files identical despite different names*

### Comparing `discord.http-1.3.8/discord_http/backend.py` & `discord.http-1.3.9/discord_http/backend.py`

 * *Files identical despite different names*

### Comparing `discord.http-1.3.8/discord_http/channel.py` & `discord.http-1.3.9/discord_http/channel.py`

 * *Files identical despite different names*

### Comparing `discord.http-1.3.8/discord_http/client.py` & `discord.http-1.3.9/discord_http/client.py`

 * *Files identical despite different names*

### Comparing `discord.http-1.3.8/discord_http/colour.py` & `discord.http-1.3.9/discord_http/colour.py`

 * *Files identical despite different names*

### Comparing `discord.http-1.3.8/discord_http/commands.py` & `discord.http-1.3.9/discord_http/commands.py`

 * *Files 5% similar despite different names*

```diff
@@ -130,14 +130,15 @@
             bot.add_listener(listener)
 
         for interaction in self._cog_interactions.values():
             interaction.cog = self
             bot.add_interaction(interaction)
 
     async def cog_load(self) -> None:
+        """ Called before the cog is loaded """
         pass
 
 
 class PartialCommand(PartialBase):
     def __init__(self, data: dict):
         super().__init__(id=int(data["id"]))
         self.name: str = data["name"]
@@ -176,42 +177,42 @@
         self.id: Optional[int] = None
         self.command = command
         self.cog: Optional["Cog"] = None
         self.type: int = int(type)
         self.name = name
         self.description = description
         self.options = []
-        self.default_member_permissions = None
 
         self.guild_install = guild_install
         self.user_install = user_install
 
-        self.name_localizations: Dict[LocaleTypes, str] = {}
-        self.description_localizations: Dict[LocaleTypes, str] = {}
-
         self.list_autocompletes: Dict[str, Callable] = {}
         self.guild_ids: list[Union[Snowflake, int]] = guild_ids or []
+
         self.__list_choices: list[str] = []
 
         if self.type == ApplicationCommandType.chat_input:
             if self.description is None:
                 self.description = command.__doc__ or "No description provided."
             if self.name != self.name.lower():
                 raise ValueError("Command names must be lowercase.")
             if not 1 <= len(self.description) <= 100:
                 raise ValueError("Command descriptions must be between 1 and 100 characters.")
         else:
             self.description = None
 
-        if self.type is ApplicationCommandType.chat_input.value and not self.options:
+        if (
+            self.type is ApplicationCommandType.chat_input.value and
+            not self.options
+        ):
             sig = inspect.signature(self.command)
             self.options = []
 
             slicer = 1
-            if sig.parameters.get("self"):
+            if sig.parameters.get("self", None):
                 slicer = 2
 
             for parameter in itertools.islice(sig.parameters.values(), slicer, None):
                 origin = getattr(
                     parameter.annotation, "__origin__",
                     parameter.annotation
                 )
@@ -227,55 +228,66 @@
                     origin = parameter.annotation.__args__[0]
 
                     # Recreate GenericAlias if it's something like Choice[str]
                     if getattr(origin, "__origin__", None):
                         parameter.annotation.__args__ = origin.__args__
                         origin = origin.__origin__
 
-                if origin in [Member, User]:
-                    ptype = CommandOptionType.user
-                elif origin in channel_types:
-                    ptype = CommandOptionType.channel
-                    option.update({
-                        "channel_types": [
-                            int(i) for i in channel_types[origin]
-                        ]
-                    })
-                elif origin in [Attachment]:
-                    ptype = CommandOptionType.attachment
-                elif origin in [Role]:
-                    ptype = CommandOptionType.role
-                elif origin in [Choice]:
-                    self.__list_choices.append(parameter.name)
-                    ptype = _type_table.get(
-                        parameter.annotation.__args__[0],
-                        CommandOptionType.string
-                    )
-                elif isinstance(origin, Range):
-                    ptype = origin.type
-                    if origin.type == CommandOptionType.string:
-                        option.update({
-                            "min_length": origin.min,
-                            "max_length": origin.max
-                        })
-                    else:
+                match origin:
+                    case x if x in [Member, User]:
+                        ptype = CommandOptionType.user
+
+                    case x if x in channel_types:
+                        ptype = CommandOptionType.channel
                         option.update({
-                            "min_value": origin.min,
-                            "max_value": origin.max
+                            "channel_types": [
+                                int(i) for i in channel_types[origin]
+                            ]
                         })
-                elif origin == int:
-                    ptype = CommandOptionType.integer
-                elif origin == bool:
-                    ptype = CommandOptionType.boolean
-                elif origin == float:
-                    ptype = CommandOptionType.number
-                elif origin == str:
-                    ptype = CommandOptionType.string
-                else:
-                    ptype = CommandOptionType.string
+
+                    case x if x in [Attachment]:
+                        ptype = CommandOptionType.attachment
+
+                    case x if x in [Role]:
+                        ptype = CommandOptionType.role
+
+                    case x if x in [Choice]:
+                        self.__list_choices.append(parameter.name)
+                        ptype = _type_table.get(
+                            parameter.annotation.__args__[0],
+                            CommandOptionType.string
+                        )
+
+                    case x if isinstance(x, Range):
+                        ptype = origin.type
+                        if origin.type == CommandOptionType.string:
+                            option.update({
+                                "min_length": origin.min,
+                                "max_length": origin.max
+                            })
+                        else:
+                            option.update({
+                                "min_value": origin.min,
+                                "max_value": origin.max
+                            })
+
+                    case x if x == int:
+                        ptype = CommandOptionType.integer
+
+                    case x if x == bool:
+                        ptype = CommandOptionType.boolean
+
+                    case x if x == float:
+                        ptype = CommandOptionType.number
+
+                    case x if x == str:
+                        ptype = CommandOptionType.string
+
+                    case _:
+                        ptype = CommandOptionType.string
 
                 option.update({
                     "name": parameter.name,
                     "description": "…",
                     "type": ptype.value,
                     "required": (parameter.default == parameter.empty),
                     "autocomplete": False,
@@ -388,15 +400,20 @@
                 result = g(ctx)
 
             if result is not True:
                 raise CheckFailed(f"Check {g.__name__} failed.")
 
         return True
 
-    async def run(self, context: "Context", *args, **kwargs) -> BaseResponse:
+    async def run(
+        self,
+        context: "Context",
+        *args,
+        **kwargs
+    ) -> BaseResponse:
         """
         Runs the command.
 
         Parameters
         ----------
         context: `Context`
             The context of the command.
@@ -479,27 +496,25 @@
         -------
         `dict`
             The dict of the command.
         """
         _extra_locale = getattr(self.command, "__locales__", {})
         _extra_params = getattr(self.command, "__describe_params__", {})
         _extra_choices = getattr(self.command, "__choices_params__", {})
-        _default_permissions = getattr(self.command, "__default_permissions__", None)
+        _default_permissions: Optional[Permissions] = getattr(
+            self.command, "__default_permissions__", None
+        )
 
         _integration_types = []
         if self.guild_install:
             _integration_types.append(0)
         if self.user_install:
             _integration_types.append(1)
 
         _integration_contexts = getattr(self.command, "__integration_contexts__", [0, 1, 2])
-        _dm_permission = getattr(self.command, "__dm_permission__", True)
-
-        if not _dm_permission:
-            _integration_contexts = [0]
 
         # Types
         _extra_locale: dict[LocaleTypes, list[LocaleContainer]]
 
         data = {
             "type": self.type,
             "name": self.name,
@@ -529,15 +544,15 @@
                     )
                     continue
 
                 opt["name_localizations"][key] = loc.name
                 opt["description_localizations"][key] = loc.description
 
         if _default_permissions:
-            data["default_member_permissions"] = _default_permissions
+            data["default_member_permissions"] = str(_default_permissions.value)
 
         for key, value in _extra_params.items():
             opt = self._find_option(key)
             if not opt:
                 continue
 
             opt["description"] = value
@@ -584,14 +599,15 @@
             find_option = next((
                 option for option in self.options
                 if option["name"] == name
             ), None)
 
             if not find_option:
                 raise ValueError(f"Option {name} in command {self.name} not found.")
+
             find_option["autocomplete"] = True
             self.list_autocompletes[name] = func
             return func
 
         return wrapper
 
 
@@ -621,22 +637,26 @@
 
 class SubGroup(Command):
     def __init__(
         self,
         *,
         name: str,
         description: Optional[str] = None,
-        guild_ids: Optional[list[Union[Snowflake, int]]] = None
+        guild_ids: Optional[list[Union[Snowflake, int]]] = None,
+        guild_install: bool = True,
+        user_install: bool = False
     ):
         self.name = name
         self.description = description or "..."  # Only used to make Discord happy
         self.guild_ids: list[Union[Snowflake, int]] = guild_ids or []
         self.type = int(ApplicationCommandType.chat_input)
         self.cog: Optional["Cog"] = None
         self.subcommands: Dict[str, Union[SubCommand, SubGroup]] = {}
+        self.guild_install = guild_install
+        self.user_install = user_install
 
     def __repr__(self) -> str:
         _subs = [g for g in self.subcommands.values()]
         return f"<SubGroup name='{self.name}', subcommands={_subs}>"
 
     def command(
         self,
@@ -824,17 +844,17 @@
     Paramaters
     ----------
     key: `str`
         The key of the choice from your dict.
     value: `Union[int, str, float]`
         The value of your choice (the one that is shown to public)
     """
-    def __init__(self, key: str, value: ChoiceT):
-        self.key: str = key
-        self.value: ChoiceT = value
+    def __init__(self, key: ChoiceT, value: Union[str, int, float]):
+        self.key: ChoiceT = key
+        self.value: Union[str, int, float] = value
 
 
 class Range:
     """
     Makes it possible to create a range rule for command arguments
 
     When used in a command, it will only return the value if it's within the range.
@@ -1114,31 +1134,44 @@
         func.__locales__ = container
         return func
 
     return decorator
 
 
 def group(
+    *,
     name: Optional[str] = None,
-    description: Optional[str] = None
+    description: Optional[str] = None,
+    guild_ids: Optional[list[Union[Snowflake, int]]] = None,
+    guild_install: bool = True,
+    user_install: bool = False,
 ):
     """
     Decorator to register a command group.
 
     Parameters
     ----------
     name: `Optional[str]`
         Name of the command group (defaults to the function name)
     description: `Optional[str]`
         Description of the command group (defaults to the function docstring)
+    guild_ids: `Optional[list[Union[Snowflake, int]]]`
+        List of guild IDs to register the command group in
+    user_install: `bool`
+        Whether the command group can be installed by users or not
+    guild_install: `bool`
+        Whether the command group can be installed by guilds or not
     """
     def decorator(func):
         return SubGroup(
             name=name or func.__name__,
-            description=description
+            description=description,
+            guild_ids=guild_ids,
+            guild_install=guild_install,
+            user_install=user_install
         )
 
     return decorator
 
 
 def describe(**kwargs):
     """
@@ -1189,25 +1222,34 @@
         if private_dm:
             func.__integration_contexts__.append(2)
 
         return func
     return decorator
 
 
-def choices(**kwargs):
+def choices(
+    **kwargs: dict[
+        Union[str, int, float],
+        Union[str, int, float]
+    ]
+):
     """
     Decorator to set choices for a command.
 
     Example usage:
 
     .. code-block:: python
 
         @commands.command()
         @commands.choices(
-            options={"opt1": "Choice 1", "opt2": "Choice 2"}
+            options={
+                "opt1": "Choice 1",
+                "opt2": "Choice 2",
+                ...
+            }
         )
         async def ping(ctx, options: Choice[str]):
             await ctx.send(f"You chose {choice.value}")
     """
     def decorator(func):
         for k, v in kwargs.items():
             if not isinstance(v, dict):
@@ -1224,15 +1266,15 @@
 def guild_only():
     """
     Decorator to set a command as guild only.
 
     This is a alias to `commands.allow_contexts(guild=True, bot_dm=False, private_dm=False)`
     """
     def decorator(func):
-        func.__dm_permission__ = False
+        func.__integration_contexts__ = [0]
         return func
 
     return decorator
 
 
 def is_nsfw():
     """ Decorator to set a command as NSFW. """
@@ -1246,68 +1288,96 @@
 def default_permissions(*args: Union[Permissions, str]):
     """ Decorator to set default permissions for a command. """
     def decorator(func):
         if not args:
             return func
 
         if isinstance(args[0], Permissions):
-            func.__default_permissions__ = str(args[0].value)
+            func.__default_permissions__ = args[0]
         else:
-            _store_perms: list[str] = []
-            for arg in args:
-                if not isinstance(arg, str):
-                    raise TypeError(
-                        "Default permissions must be a "
-                        f"string or Permissions, not a {type(arg)}"
-                    )
+            if any(not isinstance(arg, str) for arg in args):
+                raise TypeError(
+                    "All permissions must be strings "
+                    "or only 1 Permissions object"
+                )
 
-            func.__default_permissions__ = str(
-                Permissions.from_names(*_store_perms).value
+            func.__default_permissions__ = Permissions.from_names(
+                *args  # type: ignore
             )
 
         return func
 
     return decorator
 
 
-def has_permissions(*args: str):
+def has_permissions(*args: Union[Permissions, str]):
     """
     Decorator to set permissions for a command.
 
     Example usage:
 
     .. code-block:: python
 
         @commands.command()
         @commands.has_permissions("manage_messages")
         async def ban(ctx, user: Member):
             ...
     """
     def decorator(func):
-        func.__has_permissions__ = Permissions.from_names(*args)
+        if not args:
+            return func
+
+        if isinstance(args[0], Permissions):
+            func.__has_permissions__ = args[0]
+        else:
+            if any(not isinstance(arg, str) for arg in args):
+                raise TypeError(
+                    "All permissions must be strings "
+                    "or only 1 Permissions object"
+                )
+
+            func.__has_permissions__ = Permissions.from_names(
+                *args  # type: ignore
+            )
+
         return func
 
     return decorator
 
 
-def bot_has_permissions(*args: str):
+def bot_has_permissions(*args: Union[Permissions, str]):
     """
     Decorator to set permissions for a command.
 
     Example usage:
 
     .. code-block:: python
 
         @commands.command()
         @commands.bot_has_permissions("embed_links")
         async def cat(ctx):
             ...
     """
     def decorator(func):
-        func.__bot_has_permissions__ = Permissions.from_names(*args)
+        if not args:
+            return func
+
+        if isinstance(args[0], Permissions):
+            func.__bot_has_permissions__ = args[0]
+        else:
+            if any(not isinstance(arg, str) for arg in args):
+                raise TypeError(
+                    "All permissions must be strings "
+                    "or only 1 Permissions object"
+                )
+
+            func.__bot_has_permissions__ = Permissions.from_names(
+                *args  # type: ignore
+            )
+
         return func
 
     return decorator
 
 
 def check(predicate: Union[Callable, Coroutine]):
     """
```

### Comparing `discord.http-1.3.8/discord_http/context.py` & `discord.http-1.3.9/discord_http/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -648,32 +648,46 @@
     def _create_args(self) -> tuple[list[Union[Member, User, Message, None]], dict]:
         match self.command_type:
             case ApplicationCommandType.chat_input:
                 return [], self._create_args_chat_input()
 
             case ApplicationCommandType.user:
                 if self._resolved.get("members", {}):
-                    _first: Optional[dict] = next(iter(self._resolved["members"].values()), None)
+                    _first: Optional[dict] = next(
+                        iter(self._resolved["members"].values()),
+                        None
+                    )
 
                     if not _first:
                         raise ValueError("User command detected members, but was unable to parse it")
                     if not self.guild:
                         raise ValueError("While parsing members, guild was not available")
 
-                    _first["user"] = next(iter(self._resolved["users"].values()), None)
+                    _first["user"] = next(
+                        iter(self._resolved["users"].values()),
+                        None
+                    )
+
                     _target = Member(
                         state=self.bot.state,
                         guild=self.guild,
                         data=_first
                     )
+
                 elif self._resolved.get("users", {}):
-                    _first: Optional[dict] = next(iter(self._resolved["users"].values()), None)
+                    _first: Optional[dict] = next(
+                        iter(self._resolved["users"].values()),
+                        None
+                    )
+
                     if not _first:
                         raise ValueError("User command detected users, but was unable to parse it")
+
                     _target = User(state=self.bot.state, data=_first)
+
                 else:
                     raise ValueError("Neither members nor users were detected while parsing user command")
 
                 return [_target], {}
 
             case ApplicationCommandType.message:
                 return [self.message], {}
@@ -699,15 +713,15 @@
 
                     case CommandOptionType.user:
                         if "members" in resolved:
                             member_data = resolved["members"][option["value"]]
                             member_data["user"] = resolved["users"][option["value"]]
 
                             if not self.guild:
-                                raise ValueError("Guild somehow was not available while parsing user")
+                                raise ValueError("Guild somehow was not available while parsing Member")
 
                             kwargs[option["name"]] = Member(
                                 state=self.bot.state,
                                 guild=self.guild,
                                 data=member_data
                             )
                         else:
@@ -727,15 +741,15 @@
                         kwargs[option["name"]] = Attachment(
                             state=self.bot.state,
                             data=resolved["attachments"][option["value"]]
                         )
 
                     case CommandOptionType.role:
                         if not self.guild:
-                            raise ValueError("Guild somehow was not available while parsing role")
+                            raise ValueError("Guild somehow was not available while parsing Role")
 
                         kwargs[option["name"]] = Role(
                             state=self.bot.state,
                             guild=self.guild,
                             data=resolved["roles"][option["value"]]
                         )
```

### Comparing `discord.http-1.3.8/discord_http/embeds.py` & `discord.http-1.3.9/discord_http/embeds.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         description: Optional[str] = None,
         colour: Optional[Union[Colour, int]] = None,
         color: Optional[Union[Colour, int]] = None,
         url: Optional[str] = None,
         timestamp: Optional[datetime] = None,
     ):
         self.colour: Optional[Colour] = None
+
         if colour is not None:
             self.colour = Colour(int(colour))
         elif color is not None:
             self.colour = Colour(int(color))
 
         self.title: Optional[str] = title
         self.description: Optional[str] = description
```

### Comparing `discord.http-1.3.8/discord_http/emoji.py` & `discord.http-1.3.9/discord_http/emoji.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,18 +44,20 @@
 
         if is_custom:
             _animated, _name, _id = is_custom.groups()
             self.discord_emoji = True
             self.animated = bool(_animated)
             self.name: str = _name
             self.id = int(_id)
+
         elif emoji.isdigit():
             self.discord_emoji = True
             self.id = int(emoji)
             self.name: str = emoji
+
         else:
             self.name: str = emoji
 
     def __repr__(self) -> str:
         if self.discord_emoji:
             return f"<EmojiParser name='{self.name}' id={self.id}>"
         return f"<EmojiParser name='{self.name}'>"
```

### Comparing `discord.http-1.3.8/discord_http/entitlements.py` & `discord.http-1.3.9/discord_http/entitlements.py`

 * *Files identical despite different names*

### Comparing `discord.http-1.3.8/discord_http/enums.py` & `discord.http-1.3.9/discord_http/enums.py`

 * *Files identical despite different names*

### Comparing `discord.http-1.3.8/discord_http/errors.py` & `discord.http-1.3.9/discord_http/errors.py`

 * *Files identical despite different names*

### Comparing `discord.http-1.3.8/discord_http/file.py` & `discord.http-1.3.9/discord_http/file.py`

 * *Files identical despite different names*

### Comparing `discord.http-1.3.8/discord_http/flag.py` & `discord.http-1.3.9/discord_http/flag.py`

 * *Files identical despite different names*

### Comparing `discord.http-1.3.8/discord_http/guild.py` & `discord.http-1.3.9/discord_http/guild.py`

 * *Files identical despite different names*

### Comparing `discord.http-1.3.8/discord_http/http.py` & `discord.http-1.3.9/discord_http/http.py`

 * *Files identical despite different names*

### Comparing `discord.http-1.3.8/discord_http/invite.py` & `discord.http-1.3.9/discord_http/invite.py`

 * *Files identical despite different names*

### Comparing `discord.http-1.3.8/discord_http/member.py` & `discord.http-1.3.9/discord_http/member.py`

 * *Files identical despite different names*

### Comparing `discord.http-1.3.8/discord_http/mentions.py` & `discord.http-1.3.9/discord_http/mentions.py`

 * *Files identical despite different names*

### Comparing `discord.http-1.3.8/discord_http/message.py` & `discord.http-1.3.9/discord_http/message.py`

 * *Files identical despite different names*

### Comparing `discord.http-1.3.8/discord_http/multipart.py` & `discord.http-1.3.9/discord_http/multipart.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,33 +37,38 @@
             Name of the file data
         data: `Union[File, io.BufferedIOBase, dict, str]`
             The data to attach
         filename: `Optional[str]`
             Filename to be sent on Discord
         content_type: `Optional[str]`
             The content type of the file data
+            (Defaults to 'application/octet-stream' if not provided)
         """
         if not data:
             return None
 
         string = f"\r\n--{self.boundary}\r\nContent-Disposition: form-data; name=\"{name}\""
         if filename:
             string += f"; filename=\"{filename}\""
 
-        if isinstance(data, File):
-            string += f"\r\nContent-Type: {content_type or 'application/octet-stream'}\r\n\r\n"
-            data = data.data
-        elif isinstance(data, BufferedIOBase):
-            string += f"\r\nContent-Type: {content_type or 'application/octet-stream'}\r\n\r\n"
-        elif isinstance(data, dict):
-            string += "\r\nContent-Type: application/json\r\n\r\n"
-            data = json.dumps(data)
-        else:
-            string += "\r\n\r\n"
-            data = str(data)
+        match data:
+            case x if isinstance(x, File):
+                string += f"\r\nContent-Type: {content_type or 'application/octet-stream'}\r\n\r\n"
+                data = data.data  # type: ignore
+
+            case x if isinstance(x, BufferedIOBase):
+                string += f"\r\nContent-Type: {content_type or 'application/octet-stream'}\r\n\r\n"
+
+            case x if isinstance(x, dict):
+                string += "\r\nContent-Type: application/json\r\n\r\n"
+                data = json.dumps(data)
+
+            case _:
+                string += "\r\n\r\n"
+                data = str(data)
 
         self.bufs.append(string.encode("utf8"))
 
         if getattr(data, "read", None):
             # Check if the data has a read method
             # If it does, it's a file-like object
             data = data.read()  # type: ignore
```

### Comparing `discord.http-1.3.8/discord_http/object.py` & `discord.http-1.3.9/discord_http/object.py`

 * *Files identical despite different names*

### Comparing `discord.http-1.3.8/discord_http/response.py` & `discord.http-1.3.9/discord_http/response.py`

 * *Files identical despite different names*

### Comparing `discord.http-1.3.8/discord_http/role.py` & `discord.http-1.3.9/discord_http/role.py`

 * *Files identical despite different names*

### Comparing `discord.http-1.3.8/discord_http/sticker.py` & `discord.http-1.3.9/discord_http/sticker.py`

 * *Files identical despite different names*

### Comparing `discord.http-1.3.8/discord_http/tasks.py` & `discord.http-1.3.9/discord_http/tasks.py`

 * *Files identical despite different names*

### Comparing `discord.http-1.3.8/discord_http/user.py` & `discord.http-1.3.9/discord_http/user.py`

 * *Files identical despite different names*

### Comparing `discord.http-1.3.8/discord_http/utils.py` & `discord.http-1.3.9/discord_http/utils.py`

 * *Files identical despite different names*

### Comparing `discord.http-1.3.8/discord_http/view.py` & `discord.http-1.3.9/discord_http/view.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,25 +134,29 @@
         self.emoji: Optional[Union[str, dict]] = emoji
         self.style: Union[ButtonStyles, str, int] = style
         self.custom_id: str = (
             str(custom_id)
             if custom_id else _garbage_id()
         )
 
-        if isinstance(style, ButtonStyles):
-            pass
-        elif isinstance(style, int):
-            self.style = ButtonStyles(style)
-        elif isinstance(style, str):
-            try:
-                self.style = ButtonStyles[style]
-            except KeyError:
+        match style:
+            case x if isinstance(x, ButtonStyles):
+                pass
+
+            case x if isinstance(x, int):
+                self.style = ButtonStyles(style)
+
+            case x if isinstance(x, str):
+                try:
+                    self.style = ButtonStyles[style]  # type: ignore
+                except KeyError:
+                    self.style = ButtonStyles.primary
+
+            case _:
                 self.style = ButtonStyles.primary
-        else:
-            self.style = ButtonStyles.primary
 
     def to_dict(self) -> dict:
         """ `dict`: Returns a dict representation of the button """
         payload = {
             "type": self.type,
             "style": int(self.style),
             "disabled": self.disabled,
@@ -162,18 +166,21 @@
             raise ValueError("Cannot have both custom_id and url")
 
         if self.emoji:
             if isinstance(self.emoji, str):
                 payload["emoji"] = EmojiParser(self.emoji).to_dict()
             elif isinstance(self.emoji, dict):
                 payload["emoji"] = self.emoji
+
         if self.label:
             payload["label"] = self.label
+
         if self.custom_id:
             payload["custom_id"] = self.custom_id
+
         if self.url:
             payload["url"] = self.url
 
         return payload
 
 
 class Link(Button):
```

### Comparing `discord.http-1.3.8/discord_http/webhook.py` & `discord.http-1.3.9/discord_http/webhook.py`

 * *Files identical despite different names*

### Comparing `discord.http-1.3.8/pyproject.toml` & `discord.http-1.3.9/pyproject.toml`

 * *Files identical despite different names*

