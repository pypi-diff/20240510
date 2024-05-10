# Comparing `tmp/aa_discordnotify-1.3.0.tar.gz` & `tmp/aa_discordnotify-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa_discordnotify-1.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aa_discordnotify-2.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aa_discordnotify-1.3.0.tar` & `aa_discordnotify-2.0.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0     1070 2021-03-12 20:32:47.332721 aa_discordnotify-1.3.0/LICENSE
--rw-r--r--   0        0        0     4179 2021-04-16 23:02:23.491958 aa_discordnotify-1.3.0/README.md
--rw-r--r--   0        0        0      211 2023-12-28 13:42:55.875282 aa_discordnotify-1.3.0/discordnotify/__init__.py
--rw-r--r--   0        0        0      706 2023-12-28 13:42:55.875282 aa_discordnotify-1.3.0/discordnotify/app_settings.py
--rw-r--r--   0        0        0      229 2021-03-12 20:32:47.332721 aa_discordnotify-1.3.0/discordnotify/apps.py
--rw-r--r--   0        0        0      212 2021-03-13 20:20:25.313908 aa_discordnotify-1.3.0/discordnotify/auth_hooks.py
--rw-r--r--   0        0        0     2438 2023-10-06 12:29:17.311117 aa_discordnotify-1.3.0/discordnotify/core.py
--rw-r--r--   0        0        0        0 2023-12-28 13:56:04.887510 aa_discordnotify-1.3.0/discordnotify/migrations/__init__.py
--rw-r--r--   0        0        0     1900 2023-10-06 12:29:17.315117 aa_discordnotify-1.3.0/discordnotify/signals.py
--rw-r--r--   0        0        0     1027 2021-12-28 19:35:45.108126 aa_discordnotify-1.3.0/discordnotify/static/discordnotify/discordnotify_logo.png
--rw-r--r--   0        0        0     1328 2023-10-06 12:29:17.315117 aa_discordnotify-1.3.0/discordnotify/tasks.py
--rw-r--r--   0        0        0        0 2023-12-28 13:56:04.891510 aa_discordnotify-1.3.0/discordnotify/tests/__init__.py
--rw-r--r--   0        0        0     9262 2023-10-06 12:29:17.315117 aa_discordnotify-1.3.0/discordnotify/tests/test_integration.py
--rw-r--r--   0        0        0      210 2023-10-06 12:29:17.315117 aa_discordnotify-1.3.0/discordnotify/urls.py
--rw-r--r--   0        0        0      654 2023-10-06 12:29:17.315117 aa_discordnotify-1.3.0/discordnotify/views.py
--rw-r--r--   0        0        0     1961 2023-10-06 12:29:17.315117 aa_discordnotify-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     5457 1970-01-01 00:00:00.000000 aa_discordnotify-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-10 14:16:25.528040 aa_discordnotify-2.0.0/LICENSE
+-rw-r--r--   0        0        0     4249 2024-05-10 14:16:25.528040 aa_discordnotify-2.0.0/README.md
+-rw-r--r--   0        0        0      211 2024-05-10 14:16:25.528040 aa_discordnotify-2.0.0/discordnotify/__init__.py
+-rw-r--r--   0        0        0      796 2024-05-10 14:16:25.528040 aa_discordnotify-2.0.0/discordnotify/app_settings.py
+-rw-r--r--   0        0        0      229 2024-05-10 14:16:25.528040 aa_discordnotify-2.0.0/discordnotify/apps.py
+-rw-r--r--   0        0        0      212 2024-05-10 14:16:25.528040 aa_discordnotify-2.0.0/discordnotify/auth_hooks.py
+-rw-r--r--   0        0        0     2478 2024-05-10 14:16:25.528040 aa_discordnotify-2.0.0/discordnotify/core.py
+-rw-r--r--   0        0        0        0 2024-05-10 14:24:01.398620 aa_discordnotify-2.0.0/discordnotify/migrations/__init__.py
+-rw-r--r--   0        0        0     1900 2024-05-10 14:16:25.528040 aa_discordnotify-2.0.0/discordnotify/signals.py
+-rw-r--r--   0        0        0     1027 2024-05-10 14:16:25.528040 aa_discordnotify-2.0.0/discordnotify/static/discordnotify/discordnotify_logo.png
+-rw-r--r--   0        0        0     1328 2024-05-10 14:16:25.528040 aa_discordnotify-2.0.0/discordnotify/tasks.py
+-rw-r--r--   0        0        0        0 2024-05-10 14:24:01.398620 aa_discordnotify-2.0.0/discordnotify/tests/__init__.py
+-rw-r--r--   0        0        0     1297 2024-05-10 14:16:25.532040 aa_discordnotify-2.0.0/discordnotify/tests/test_core.py
+-rw-r--r--   0        0        0     9262 2024-05-10 14:16:25.532040 aa_discordnotify-2.0.0/discordnotify/tests/test_integration.py
+-rw-r--r--   0        0        0      210 2024-05-10 14:16:25.532040 aa_discordnotify-2.0.0/discordnotify/urls.py
+-rw-r--r--   0        0        0      654 2024-05-10 14:16:25.532040 aa_discordnotify-2.0.0/discordnotify/views.py
+-rw-r--r--   0        0        0     1961 2024-05-10 14:16:25.532040 aa_discordnotify-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5527 1970-01-01 00:00:00.000000 aa_discordnotify-2.0.0/PKG-INFO
```

### Comparing `aa_discordnotify-1.3.0/LICENSE` & `aa_discordnotify-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_discordnotify-1.3.0/README.md` & `aa_discordnotify-2.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -79,10 +79,11 @@
 Here is a list of available settings for this app. They can be configured by adding them to your AA settings file (`local.py`).
 
 Note that all settings are optional and the app will use the documented default settings if they are not used.
 
 Name | Description | Default
 -- | -- | --
 `DISCORDNOTIFY_ENABLED`| Set this to False to disable this app temporarily | `True`
-`DISCORDNOTIFY_DISCORDPROXY_PORT`| Port used to communicate with Discord Proxy. | `50051`
+`DISCORDPROXY_PORT`| Port used to communicate with Discord Proxy. | `50051`
+`DISCORDPROXY_HOST`| Hostname used to communicate with Discord Proxy. | `localhost`
 `DISCORDNOTIFY_MARK_AS_VIEWED`| When enabled will mark all notifications as viewed that have been successfully submitted to Discord | `False`
 `DISCORDNOTIFY_SUPERUSER_ONLY`| When enabled only superusers will be get their notifications forwarded. | `False`
```

### Comparing `aa_discordnotify-1.3.0/discordnotify/app_settings.py` & `aa_discordnotify-2.0.0/discordnotify/app_settings.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Settings for Discord Notify."""
 
 from django.conf import settings
 
-DISCORDNOTIFY_DISCORDPROXY_PORT = getattr(
-    settings, "DISCORDNOTIFY_DISCORDPROXY_PORT", 50051
-)
+DISCORDPROXY_PORT = getattr(settings, "DISCORDPROXY_PORT", 50051)
 """Port used to communicate with Discord Proxy."""
 
+DISCORDPROXY_HOST = getattr(settings, "DISCORDPROXY_HOST", "localhost")
+"""Host used to communicate with Discord Proxy."""
+
 DISCORDNOTIFY_SUPERUSER_ONLY = getattr(settings, "DISCORDNOTIFY_SUPERUSER_ONLY", False)
 """When set to True, only superusers will be get their notifications forwarded."""
 
 DISCORDNOTIFY_ENABLED = getattr(settings, "DISCORDNOTIFY_ENABLED", True)
 """Set to False to disable this app."""
 
 DISCORDNOTIFY_MARK_AS_VIEWED = getattr(settings, "DISCORDNOTIFY_MARK_AS_VIEWED", True)
```

### Comparing `aa_discordnotify-1.3.0/discordnotify/core.py` & `aa_discordnotify-2.0.0/discordnotify/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 """Core logic for Discord Notify."""
 
+from typing import Any
+
 from discordproxy.client import DiscordClient
 from discordproxy.discord_api_pb2 import Embed
 
 from allianceauth.notifications.models import Notification
 from app_utils.urls import reverse_absolute, static_file_absolute_url
 
 from . import __title__
-from .app_settings import DISCORDNOTIFY_DISCORDPROXY_PORT, DISCORDNOTIFY_MARK_AS_VIEWED
+from .app_settings import (
+    DISCORDNOTIFY_MARK_AS_VIEWED,
+    DISCORDPROXY_HOST,
+    DISCORDPROXY_PORT,
+)
 
 # embed colors
 COLOR_INFO = 0x5BC0DE
 COLOR_SUCCESS = 0x5CB85C
 COLOR_WARNING = 0xF0AD4E
 COLOR_DANGER = 0xD9534F
 
@@ -40,23 +46,23 @@
     embed = _build_embed(
         notification_id=notification_id,
         title=title,
         message=message,
         level=level,
         timestamp=timestamp,
     )
-    target = f"localhost:{DISCORDNOTIFY_DISCORDPROXY_PORT}"
+    target = f"{DISCORDPROXY_HOST}:{DISCORDPROXY_PORT}"
     client = DiscordClient(target=target, timeout=DISCORD_PROXY_TIMEOUT)
     client.create_direct_message(user_id=discord_uid, embed=embed)
     _mark_as_viewed(notification_id)
 
 
 def _build_embed(
     notification_id: int, title: str, message: str, level: str, timestamp: str
-) -> Embed:
+) -> Any:
     description = message.strip()
     if len(description) > MAX_LENGTH_DESCRIPTION:
         description = description[: (MAX_LENGTH_DESCRIPTION - 6)] + " [...]"
     author = Embed.Author(
         name="Alliance Auth Notification",
         icon_url=static_file_absolute_url("icons/apple-touch-icon.png"),
     )
```

### Comparing `aa_discordnotify-1.3.0/discordnotify/signals.py` & `aa_discordnotify-2.0.0/discordnotify/signals.py`

 * *Files identical despite different names*

### Comparing `aa_discordnotify-1.3.0/discordnotify/static/discordnotify/discordnotify_logo.png` & `aa_discordnotify-2.0.0/discordnotify/static/discordnotify/discordnotify_logo.png`

 * *Files identical despite different names*

### Comparing `aa_discordnotify-1.3.0/discordnotify/tasks.py` & `aa_discordnotify-2.0.0/discordnotify/tasks.py`

 * *Files identical despite different names*

### Comparing `aa_discordnotify-1.3.0/discordnotify/tests/test_integration.py` & `aa_discordnotify-2.0.0/discordnotify/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `aa_discordnotify-1.3.0/discordnotify/views.py` & `aa_discordnotify-2.0.0/discordnotify/views.py`

 * *Files identical despite different names*

### Comparing `aa_discordnotify-1.3.0/pyproject.toml` & `aa_discordnotify-2.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aa_discordnotify-1.3.0/PKG-INFO` & `aa_discordnotify-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-discordnotify
-Version: 1.3.0
+Version: 2.0.0
 Summary: Forward Alliance Auth notifications to users on Discord.
 Author-email: Erik Kalkoken <kalkoken87@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
@@ -107,11 +107,12 @@
 Here is a list of available settings for this app. They can be configured by adding them to your AA settings file (`local.py`).
 
 Note that all settings are optional and the app will use the documented default settings if they are not used.
 
 Name | Description | Default
 -- | -- | --
 `DISCORDNOTIFY_ENABLED`| Set this to False to disable this app temporarily | `True`
-`DISCORDNOTIFY_DISCORDPROXY_PORT`| Port used to communicate with Discord Proxy. | `50051`
+`DISCORDPROXY_PORT`| Port used to communicate with Discord Proxy. | `50051`
+`DISCORDPROXY_HOST`| Hostname used to communicate with Discord Proxy. | `localhost`
 `DISCORDNOTIFY_MARK_AS_VIEWED`| When enabled will mark all notifications as viewed that have been successfully submitted to Discord | `False`
 `DISCORDNOTIFY_SUPERUSER_ONLY`| When enabled only superusers will be get their notifications forwarded. | `False`
```

