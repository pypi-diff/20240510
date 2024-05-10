# Comparing `tmp/aa_mailrelay-1.3.0.tar.gz` & `tmp/aa_mailrelay-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa_mailrelay-1.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aa_mailrelay-1.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aa_mailrelay-1.3.0.tar` & `aa_mailrelay-1.4.0.tar`

### file list

```diff
@@ -1,34 +1,36 @@
--rw-r--r--   0        0        0     1070 2024-01-18 14:03:57.975129 aa_mailrelay-1.3.0/LICENSE
--rw-r--r--   0        0        0     4179 2024-01-18 14:03:57.975129 aa_mailrelay-1.3.0/README.md
--rw-r--r--   0        0        0      182 2024-01-18 14:03:57.979128 aa_mailrelay-1.3.0/mailrelay/__init__.py
--rw-r--r--   0        0        0     5924 2024-01-18 14:03:57.979128 aa_mailrelay-1.3.0/mailrelay/admin.py
--rw-r--r--   0        0        0      690 2024-01-18 14:03:57.979128 aa_mailrelay-1.3.0/mailrelay/app_settings.py
--rw-r--r--   0        0        0      192 2024-01-18 14:03:57.979128 aa_mailrelay-1.3.0/mailrelay/apps.py
--rw-r--r--   0        0        0      204 2024-01-18 14:03:57.979128 aa_mailrelay-1.3.0/mailrelay/auth_hooks.py
--rw-r--r--   0        0        0        0 2024-01-18 14:53:21.020375 aa_mailrelay-1.3.0/mailrelay/core/__init__.py
--rw-r--r--   0        0        0     1287 2024-01-18 14:03:57.979128 aa_mailrelay-1.3.0/mailrelay/core/xml_converter.py
--rw-r--r--   0        0        0     1998 2024-01-18 14:03:57.979128 aa_mailrelay-1.3.0/mailrelay/managers.py
--rw-r--r--   0        0        0     4328 2024-01-18 14:03:57.979128 aa_mailrelay-1.3.0/mailrelay/migrations/0001_initial.py
--rw-r--r--   0        0        0      632 2024-01-18 14:03:57.979128 aa_mailrelay-1.3.0/mailrelay/migrations/0002_django4_update.py
--rw-r--r--   0        0        0      805 2024-01-18 14:03:57.979128 aa_mailrelay-1.3.0/mailrelay/migrations/0003_alter_discordcategory_options_and_more.py
--rw-r--r--   0        0        0        0 2024-01-18 14:53:21.024375 aa_mailrelay-1.3.0/mailrelay/migrations/__init__.py
--rw-r--r--   0        0        0     7959 2024-01-18 14:03:57.979128 aa_mailrelay-1.3.0/mailrelay/models.py
--rw-r--r--   0        0        0     1137 2024-01-18 14:03:57.979128 aa_mailrelay-1.3.0/mailrelay/static/mailrelay/mailrelay_logo.png
--rw-r--r--   0        0        0     2682 2024-01-18 14:03:57.979128 aa_mailrelay-1.3.0/mailrelay/tasks.py
--rw-r--r--   0        0        0      296 2024-01-18 14:03:57.979128 aa_mailrelay-1.3.0/mailrelay/templates/admin/mailrelay/relayconfig/change_list.html
--rw-r--r--   0        0        0      335 2024-01-18 14:03:57.979128 aa_mailrelay-1.3.0/mailrelay/templates/mailrelay/base.html
--rw-r--r--   0        0        0      478 2024-01-18 14:03:57.979128 aa_mailrelay-1.3.0/mailrelay/templates/mailrelay/index.html
--rw-r--r--   0        0        0        0 2024-01-18 14:53:21.024375 aa_mailrelay-1.3.0/mailrelay/tests/__init__.py
--rw-r--r--   0        0        0     3320 2024-01-18 14:03:57.979128 aa_mailrelay-1.3.0/mailrelay/tests/factories.py
--rw-r--r--   0        0        0     5665 2024-01-18 14:03:57.979128 aa_mailrelay-1.3.0/mailrelay/tests/test_admin.py
--rw-r--r--   0        0        0     1380 2024-01-18 14:03:57.979128 aa_mailrelay-1.3.0/mailrelay/tests/test_core_xml_converter.py
--rw-r--r--   0        0        0     3072 2024-01-18 14:03:57.979128 aa_mailrelay-1.3.0/mailrelay/tests/test_integration.py
--rw-r--r--   0        0        0    13609 2024-01-18 14:03:57.979128 aa_mailrelay-1.3.0/mailrelay/tests/test_models.py
--rw-r--r--   0        0        0     6119 2024-01-18 14:03:57.979128 aa_mailrelay-1.3.0/mailrelay/tests/test_tasks.py
--rw-r--r--   0        0        0      370 2024-01-18 14:03:57.979128 aa_mailrelay-1.3.0/mailrelay/tests/test_utils.py
--rw-r--r--   0        0        0     1439 2024-01-18 14:03:57.979128 aa_mailrelay-1.3.0/mailrelay/tests/test_views.py
--rw-r--r--   0        0        0      272 2024-01-18 14:03:57.979128 aa_mailrelay-1.3.0/mailrelay/urls.py
--rw-r--r--   0        0        0      531 2024-01-18 14:03:57.979128 aa_mailrelay-1.3.0/mailrelay/utils.py
--rw-r--r--   0        0        0     1218 2024-01-18 14:03:57.979128 aa_mailrelay-1.3.0/mailrelay/views.py
--rw-r--r--   0        0        0     1831 2024-01-18 14:03:57.979128 aa_mailrelay-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     5293 1970-01-01 00:00:00.000000 aa_mailrelay-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-10 20:25:48.101287 aa_mailrelay-1.4.0/LICENSE
+-rw-r--r--   0        0        0     4240 2024-05-10 20:25:48.101287 aa_mailrelay-1.4.0/README.md
+-rw-r--r--   0        0        0      182 2024-05-10 20:25:48.101287 aa_mailrelay-1.4.0/mailrelay/__init__.py
+-rw-r--r--   0        0        0     5845 2024-05-10 20:25:48.101287 aa_mailrelay-1.4.0/mailrelay/admin.py
+-rw-r--r--   0        0        0      781 2024-05-10 20:25:48.101287 aa_mailrelay-1.4.0/mailrelay/app_settings.py
+-rw-r--r--   0        0        0      192 2024-05-10 20:25:48.101287 aa_mailrelay-1.4.0/mailrelay/apps.py
+-rw-r--r--   0        0        0      204 2024-05-10 20:25:48.101287 aa_mailrelay-1.4.0/mailrelay/auth_hooks.py
+-rw-r--r--   0        0        0        0 2024-05-10 20:49:45.010964 aa_mailrelay-1.4.0/mailrelay/core/__init__.py
+-rw-r--r--   0        0        0     1287 2024-05-10 20:25:48.101287 aa_mailrelay-1.4.0/mailrelay/core/xml_converter.py
+-rw-r--r--   0        0        0     1972 2024-05-10 20:25:48.101287 aa_mailrelay-1.4.0/mailrelay/managers.py
+-rw-r--r--   0        0        0     4328 2024-05-10 20:25:48.101287 aa_mailrelay-1.4.0/mailrelay/migrations/0001_initial.py
+-rw-r--r--   0        0        0      632 2024-05-10 20:25:48.101287 aa_mailrelay-1.4.0/mailrelay/migrations/0002_django4_update.py
+-rw-r--r--   0        0        0      805 2024-05-10 20:25:48.101287 aa_mailrelay-1.4.0/mailrelay/migrations/0003_alter_discordcategory_options_and_more.py
+-rw-r--r--   0        0        0        0 2024-05-10 20:49:45.010964 aa_mailrelay-1.4.0/mailrelay/migrations/__init__.py
+-rw-r--r--   0        0        0     7917 2024-05-10 20:25:48.105287 aa_mailrelay-1.4.0/mailrelay/models.py
+-rw-r--r--   0        0        0      453 2024-05-10 20:25:48.105287 aa_mailrelay-1.4.0/mailrelay/providers.py
+-rw-r--r--   0        0        0     1137 2024-05-10 20:25:48.105287 aa_mailrelay-1.4.0/mailrelay/static/mailrelay/mailrelay_logo.png
+-rw-r--r--   0        0        0     2585 2024-05-10 20:25:48.105287 aa_mailrelay-1.4.0/mailrelay/tasks.py
+-rw-r--r--   0        0        0      296 2024-05-10 20:25:48.105287 aa_mailrelay-1.4.0/mailrelay/templates/admin/mailrelay/relayconfig/change_list.html
+-rw-r--r--   0        0        0      335 2024-05-10 20:25:48.105287 aa_mailrelay-1.4.0/mailrelay/templates/mailrelay/base.html
+-rw-r--r--   0        0        0      478 2024-05-10 20:25:48.105287 aa_mailrelay-1.4.0/mailrelay/templates/mailrelay/index.html
+-rw-r--r--   0        0        0        0 2024-05-10 20:49:45.010964 aa_mailrelay-1.4.0/mailrelay/tests/__init__.py
+-rw-r--r--   0        0        0     3320 2024-05-10 20:25:48.105287 aa_mailrelay-1.4.0/mailrelay/tests/factories.py
+-rw-r--r--   0        0        0     5771 2024-05-10 20:25:48.105287 aa_mailrelay-1.4.0/mailrelay/tests/test_admin.py
+-rw-r--r--   0        0        0     1380 2024-05-10 20:25:48.105287 aa_mailrelay-1.4.0/mailrelay/tests/test_core_xml_converter.py
+-rw-r--r--   0        0        0     3131 2024-05-10 20:25:48.105287 aa_mailrelay-1.4.0/mailrelay/tests/test_integration.py
+-rw-r--r--   0        0        0    13981 2024-05-10 20:25:48.105287 aa_mailrelay-1.4.0/mailrelay/tests/test_models.py
+-rw-r--r--   0        0        0      624 2024-05-10 20:25:48.105287 aa_mailrelay-1.4.0/mailrelay/tests/test_providers.py
+-rw-r--r--   0        0        0     6119 2024-05-10 20:25:48.105287 aa_mailrelay-1.4.0/mailrelay/tests/test_tasks.py
+-rw-r--r--   0        0        0      370 2024-05-10 20:25:48.105287 aa_mailrelay-1.4.0/mailrelay/tests/test_utils.py
+-rw-r--r--   0        0        0     1439 2024-05-10 20:25:48.105287 aa_mailrelay-1.4.0/mailrelay/tests/test_views.py
+-rw-r--r--   0        0        0      272 2024-05-10 20:25:48.105287 aa_mailrelay-1.4.0/mailrelay/urls.py
+-rw-r--r--   0        0        0      531 2024-05-10 20:25:48.105287 aa_mailrelay-1.4.0/mailrelay/utils.py
+-rw-r--r--   0        0        0     1101 2024-05-10 20:25:48.105287 aa_mailrelay-1.4.0/mailrelay/views.py
+-rw-r--r--   0        0        0     1835 2024-05-10 20:25:48.105287 aa_mailrelay-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5358 1970-01-01 00:00:00.000000 aa_mailrelay-1.4.0/PKG-INFO
```

### Comparing `aa_mailrelay-1.3.0/LICENSE` & `aa_mailrelay-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_mailrelay-1.3.0/README.md` & `aa_mailrelay-1.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -87,11 +87,12 @@
 
 Here is a list of available settings for this app. They can be configured by adding them to your AA settings file (`local.py`).
 
 Note that all settings are optional and the app will use the documented default settings if they are not used.
 
 Name|Description|Default
 --|--|--
-`MAILRELAY_DISCORD_TASK_TIMEOUT`|Timeout for asynchronous Discord requests in seconds.|`60`
-`MAILRELAY_DISCORD_USER_TIMEOUT`|Timeout for user facing Discord requests in seconds.|`30`
+`DISCORDPROXY_HOST`|Port used to communicate with Discord Proxy.|`localhost`
+`DISCORDPROXY_PORT`|Host used to communicate with Discord Proxy.|`50051`
+`MAILRELAY_DISCORDPROXY_TIMEOUT`|Timeout for sending request to DISCORDPROXY in seconds.|`30`
 `MAILRELAY_OLDEST_MAIL_HOURS`|Oldest mail to be forwarded in hours. Set to 0 to disable.|`2`
 `MAILRELAY_RELAY_GRACE_MINUTES`|Max time in minutes since last successful relay before service is reported as down.|`30`
```

### Comparing `aa_mailrelay-1.3.0/mailrelay/admin.py` & `aa_mailrelay-1.4.0/mailrelay/admin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """Admin site for Mail Relay."""
+
 # pylint: disable=missing-class-docstring,missing-function-docstring
 
 from collections import defaultdict
 
-from discordproxy.client import DiscordClient
 from discordproxy.exceptions import DiscordProxyException
 
 from django.conf import settings
 from django.contrib import admin
 from django.forms import ModelForm
 from django.utils.html import format_html
 
 from allianceauth.services.hooks import get_extension_logger
 from app_utils.logging import LoggerAddTag
 
 from . import __title__
-from .app_settings import MAILRELAY_DISCORD_USER_TIMEOUT
 from .models import DiscordCategory, DiscordChannel, RelayConfig
+from .providers import create_discordproxy_client
 
 logger = LoggerAddTag(get_extension_logger(__name__), __title__)
 
 
 class RelayConfigForm(ModelForm):
     """Form for RelayConfig objects."""
 
@@ -93,15 +93,15 @@
             eve_character.corporation_name,
             eve_character.alliance_name if eve_character.alliance_name else "",
         )
 
     @admin.action(description="Send test message for selected configurations")
     def send_test_message(self, request, queryset):
         items_count = 0
-        client = DiscordClient()
+        client = create_discordproxy_client()
         for obj in queryset:
             try:
                 client.create_channel_message(
                     channel_id=obj.discord_channel.id,
                     content=f"Test message from {__title__}",
                 )
             except DiscordProxyException as ex:
@@ -124,15 +124,15 @@
         mails_count = 0
         for obj in queryset:
             obj.mails_sent.clear()
             new_mails_qs = obj.new_mails_queryset()
             mails_sent = 0
             for mail in new_mails_qs:
                 try:
-                    obj.send_mail(mail, timeout=MAILRELAY_DISCORD_USER_TIMEOUT)
+                    obj.send_mail(mail)
                 except DiscordProxyException as ex:
                     logger.error(
                         "%s: Failed to send test message for", obj, exc_info=True
                     )
                     self.message_user(
                         request,
                         f"{obj}: Failed to send test message: {ex}",
```

### Comparing `aa_mailrelay-1.3.0/mailrelay/core/xml_converter.py` & `aa_mailrelay-1.4.0/mailrelay/core/xml_converter.py`

 * *Files identical despite different names*

### Comparing `aa_mailrelay-1.3.0/mailrelay/managers.py` & `aa_mailrelay-1.4.0/mailrelay/managers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Managers for Mail Relay."""
 
-from typing import Optional
-
-from discordproxy.client import Channel, DiscordClient
+from discordproxy.client import Channel
 
 from django.conf import settings
 from django.db import models
 
+from .providers import create_discordproxy_client
+
 
 class DiscordChannelManager(models.Manager):
     """Manager for DiscordChannel."""
 
-    def sync(self, timeout: Optional[int] = None) -> int:
+    def sync(self) -> int:
         """Synchronize list of guild channels objects with the Discord server.
 
         Args:
         - timeout: timeout for request to Discord in seconds
 
         Returns:
         number of channels
@@ -25,15 +25,15 @@
         try:
             guild_id = int(settings.DISCORD_GUILD_ID)
         except AttributeError:
             raise ValueError(
                 "Can not find Discord guild ID in settings. "
                 "Is the Discord service configured?"
             ) from None
-        client = DiscordClient(timeout=timeout)
+        client = create_discordproxy_client()
         channels = client.get_guild_channels(guild_id)
         # pylint: disable=no-member
         categories = {
             obj.id: obj for obj in channels if obj.type == Channel.Type.GUILD_CATEGORY
         }
         for category in categories.values():
             DiscordCategory.objects.update_or_create(
```

### Comparing `aa_mailrelay-1.3.0/mailrelay/migrations/0001_initial.py` & `aa_mailrelay-1.4.0/mailrelay/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_mailrelay-1.3.0/mailrelay/migrations/0002_django4_update.py` & `aa_mailrelay-1.4.0/mailrelay/migrations/0002_django4_update.py`

 * *Files identical despite different names*

### Comparing `aa_mailrelay-1.3.0/mailrelay/migrations/0003_alter_discordcategory_options_and_more.py` & `aa_mailrelay-1.4.0/mailrelay/migrations/0003_alter_discordcategory_options_and_more.py`

 * *Files identical despite different names*

### Comparing `aa_mailrelay-1.3.0/mailrelay/models.py` & `aa_mailrelay-1.4.0/mailrelay/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Models for Mail Relay."""
 
 import datetime as dt
-from typing import List, Optional
+from typing import Optional
 
-from discordproxy.client import DiscordClient
 from discordproxy.discord_api_pb2 import Embed
 from memberaudit.models import Character, CharacterMail
 
 from django.db import models
 from django.utils.timezone import now
 
 from allianceauth.services.hooks import get_extension_logger
@@ -15,14 +14,15 @@
 from app_utils.logging import LoggerAddTag
 from app_utils.urls import static_file_absolute_url
 
 from . import __title__
 from .app_settings import MAILRELAY_OLDEST_MAIL_HOURS, MAILRELAY_RELAY_GRACE_MINUTES
 from .core.xml_converter import eve_xml_to_discord_markup
 from .managers import DiscordChannelManager
+from .providers import create_discordproxy_client
 from .utils import chunks_by_lines
 
 logger = LoggerAddTag(get_extension_logger(__name__), __title__)
 
 
 class RelayConfig(models.Model):
     """A configuration for mail relay."""
@@ -118,28 +118,28 @@
             new_mails_qs = new_mails_qs.filter(recipients__id=corporation_id)
 
         else:
             raise NotImplementedError(f"Unknown mail category: {self.mail_category}")
 
         return new_mails_qs
 
-    def send_mail(self, mail: CharacterMail, timeout: Optional[int] = None) -> None:
+    def send_mail(self, mail: CharacterMail) -> None:
         """Send one mail to channel.
 
         Args:
         - mail: mail to be sent
         - timeout: timeout for request to Discord in seconds
         """
         if not mail.body:
             return
 
         if not self.discord_channel:
             raise ValueError(f"No channel configured for config {self}")
 
-        client = DiscordClient(timeout=timeout)
+        client = create_discordproxy_client()
         embeds = self._generate_embeds(mail)
         for num, embed in enumerate(embeds, start=1):
             content = self._content_with_mentions() if num == 1 else ""
             client.create_channel_message(
                 channel_id=self.discord_channel.id, content=content, embed=embed
             )
         self.mails_sent.add(mail)
@@ -155,15 +155,15 @@
             title = "Alliance"
         elif self.mail_category == self.MailCategory.CORPORATION:
             title = "Corporation"
         else:
             title = "Eve"
         return f"{mention}**New {title} Mail**"
 
-    def _generate_embeds(self, mail: CharacterMail) -> List[Embed]:
+    def _generate_embeds(self, mail: CharacterMail) -> list:
         recipients = ", ".join(
             [obj.name_plus for obj in mail.recipients.order_by("name")]
         )
         from_name = mail.sender.name_plus if mail.sender else "?"
         sent_text = mail.timestamp.strftime(DATETIME_FORMAT) if mail.timestamp else "?"
         full_description = (
             f"**From**: {from_name}\n"
```

### Comparing `aa_mailrelay-1.3.0/mailrelay/static/mailrelay/mailrelay_logo.png` & `aa_mailrelay-1.4.0/mailrelay/static/mailrelay/mailrelay_logo.png`

 * *Files identical despite different names*

### Comparing `aa_mailrelay-1.3.0/mailrelay/tasks.py` & `aa_mailrelay-1.4.0/mailrelay/tasks.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from memberaudit.models import CharacterMail
 from memberaudit.tasks import update_character_mails
 
 from allianceauth.services.hooks import get_extension_logger
 from app_utils.logging import LoggerAddTag
 
 from . import __title__
-from .app_settings import MAILRELAY_DISCORD_TASK_TIMEOUT
 from .models import RelayConfig
 
 logger = LoggerAddTag(get_extension_logger(__name__), __title__)
 
 WAIT_FOR_MAIL_UPDATE_TO_COMPLETE = 60
 
 
@@ -55,15 +54,15 @@
 def forward_mail_to_discord(config_pk, mail_pk):
     """Forward one mail to Discord."""
     config: RelayConfig = RelayConfig.objects.select_related(
         "character", "discord_channel"
     ).get(pk=config_pk)
     mail: CharacterMail = config.character.mails.get(pk=mail_pk)  # type: ignore
     try:
-        config.send_mail(mail=mail, timeout=MAILRELAY_DISCORD_TASK_TIMEOUT)
+        config.send_mail(mail=mail)
     except DiscordProxyException as ex:
         logger.error(
             "%s: Failed to send mail %s to channel %s due to error from Discord Proxy. "
             "Will try again later: %s",
             config,
             mail,
             config.discord_channel,
```

### Comparing `aa_mailrelay-1.3.0/mailrelay/tests/factories.py` & `aa_mailrelay-1.4.0/mailrelay/tests/factories.py`

 * *Files identical despite different names*

### Comparing `aa_mailrelay-1.3.0/mailrelay/tests/test_admin.py` & `aa_mailrelay-1.4.0/mailrelay/tests/test_admin.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,38 +60,41 @@
         config = create_relay_config(character=self.character)
         # when
         result = self.modeladmin._organization(config)
         # then
         self.assertEqual(result, "Wayne Technologies Inc.<br>Wayne Enterprises")
 
     @patch(ADMIN_PATH + ".RelayConfigAdmin.message_user")
-    @patch(ADMIN_PATH + ".DiscordClient.create_channel_message")
+    @patch(ADMIN_PATH + ".create_discordproxy_client")
     def test_action_send_test_message(
-        self, mock_create_channel_message, mock_message_user
+        self, mock_create_discord_client, mock_message_user
     ):
         # given
         config = create_relay_config(character=self.character)
         request = create_fake_request(user=self.admin_user)
         queryset = RelayConfig.objects.all()
         # when
         self.modeladmin.send_test_message(request, queryset)
         # then
         channel_ids = {
-            obj[1]["channel_id"] for obj in mock_create_channel_message.call_args_list
+            obj[1]["channel_id"]
+            for obj in mock_create_discord_client.return_value.create_channel_message.call_args_list
         }
         self.assertSetEqual(channel_ids, {config.discord_channel.pk})
         self.assertTrue(mock_message_user.called)
 
-    @patch(ADMIN_PATH + ".RelayConfigAdmin.message_user")
-    @patch(ADMIN_PATH + ".DiscordClient.create_channel_message")
+    @patch(ADMIN_PATH + ".RelayConfigAdmin.message_user", spec=True)
+    @patch(ADMIN_PATH + ".create_discordproxy_client", spec=True)
     def test_action_send_test_message_with_error(
-        self, mock_create_channel_message, mock_message_user
+        self, mock_create_discord_client, mock_message_user
     ):
         # given
-        mock_create_channel_message.side_effect = DiscordProxyException
+        mock_create_discord_client.return_value.create_channel_message.side_effect = (
+            DiscordProxyException
+        )
         create_relay_config(character=self.character)
         request = create_fake_request(user=self.admin_user)
         queryset = RelayConfig.objects.all()
         # when
         self.modeladmin.send_test_message(request, queryset)
         # then
         self.assertTrue(mock_message_user.called)
```

### Comparing `aa_mailrelay-1.3.0/mailrelay/tests/test_core_xml_converter.py` & `aa_mailrelay-1.4.0/mailrelay/tests/test_core_xml_converter.py`

 * *Files identical despite different names*

### Comparing `aa_mailrelay-1.3.0/mailrelay/tests/test_integration.py` & `aa_mailrelay-1.4.0/mailrelay/tests/test_integration.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,18 +27,18 @@
 def dummy_task(*args, **kwargs):
     """Can replace tasks that need to run."""
     pass
 
 
 @override_settings(CELERY_ALWAYS_EAGER=True, CELERY_EAGER_PROPAGATES_EXCEPTIONS=True)
 @patch(MODELS_PATH + ".MAILRELAY_OLDEST_MAIL_HOURS", 2)
-@patch(MODELS_PATH + ".DiscordClient", spec=True)
+@patch(MODELS_PATH + ".create_discordproxy_client", spec=True)
 @patch(TASKS_PATH + ".update_character_mails", new=dummy_task)
 class TestForwardNewMails(NoSocketsTestCase):
-    def test_should_forward_mail_with_one_config(self, mock_DiscordClient):
+    def test_should_forward_mail_with_one_config(self, mock_create_discord_client):
         # given
         user_1001 = create_fake_user(1001, "Bruce Wayne")
         character_1001 = add_memberaudit_character_to_user(user_1001, 1001)
         create_eve_entities_from_evecharacter(
             character_1001.character_ownership.character
         )
         create_eve_entity(id=1002, name="Peter Parker")
@@ -48,18 +48,20 @@
         # when
         with patch(MODELS_PATH + ".now") as mock_now:
             mock_now.return_value = dt.datetime(2021, 12, 24, 12, 30, tzinfo=utc)
             forward_new_mails.delay()
 
         # then
         self.assertEqual(
-            mock_DiscordClient.return_value.create_channel_message.call_count, 1
+            mock_create_discord_client.return_value.create_channel_message.call_count, 1
         )
 
-    def test_should_forward_mail_with_multiple_configs(self, mock_DiscordClient):
+    def test_should_forward_mail_with_multiple_configs(
+        self, mock_create_discord_client
+    ):
         # given
         user_1001 = create_fake_user(1001, "Bruce Wayne")
         character_1001 = add_memberaudit_character_to_user(user_1001, 1001)
         create_eve_entities_from_evecharacter(
             character_1001.character_ownership.character
         )
         user_1002 = create_fake_user(1002, "Peter Parker")
@@ -75,9 +77,9 @@
         )
         # when
         with patch(MODELS_PATH + ".now") as mock_now:
             mock_now.return_value = dt.datetime(2021, 12, 24, 12, 30, tzinfo=utc)
             forward_new_mails.delay()
         # then
         self.assertEqual(
-            mock_DiscordClient.return_value.create_channel_message.call_count, 2
+            mock_create_discord_client.return_value.create_channel_message.call_count, 2
         )
```

### Comparing `aa_mailrelay-1.3.0/mailrelay/tests/test_models.py` & `aa_mailrelay-1.4.0/mailrelay/tests/test_models.py`

 * *Files 8% similar despite different names*

```diff
@@ -177,52 +177,59 @@
             result = config.new_mails_queryset()
 
         # then
         mail_pks = set(result.values_list("pk", flat=True))
         self.assertSetEqual(mail_pks, {old_mail.pk, new_mail.pk})
 
 
-@patch(MODELS_PATH + ".DiscordClient.create_channel_message")
+@patch(MODELS_PATH + ".create_discordproxy_client", spec=True)
 class TestRelayConfigSendMail(NoSocketsTestCase):
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
         user = create_fake_user(1001, "Bruce Wayne")
         cls.character = add_memberaudit_character_to_user(user, 1001)
         create_eve_entities_from_evecharacter(cls.character.eve_character)
         create_eve_entity(id=1002, name="Peter Parker")
 
-    def test_should_send_valid_mail(self, mock_create_channel_message):
+    def test_should_send_valid_mail(self, mock_create_discord_client):
         # given
         mail = create_character_mail(character=self.character, sender_id=1002)
         config = create_relay_config(character=self.character)
         # when
         config.send_mail(mail)
         # then
-        self.assertTrue(mock_create_channel_message.called)
+        self.assertTrue(
+            mock_create_discord_client.return_value.create_channel_message.called
+        )
 
-    def test_should_not_send_mail_without_body(self, mock_create_channel_message):
+    def test_should_not_send_mail_without_body(self, mock_create_discord_client):
         # given
         mail = create_character_mail(character=self.character, sender_id=1002, body="")
         config = create_relay_config(character=self.character)
         # when
         config.send_mail(mail)
         # then
-        self.assertFalse(mock_create_channel_message.called)
+        self.assertFalse(
+            mock_create_discord_client.return_value.create_channel_message.called
+        )
 
-    def test_should_send_mail_with_everbody_ping(self, mock_create_channel_message):
+    def test_should_send_mail_with_everybody_ping(self, mock_create_discord_client):
         # given
         mail = create_character_mail(character=self.character, sender_id=1002)
         config = create_relay_config(
             character=self.character, ping_type=RelayConfig.ChannelPingType.EVERYONE
         )
         # when
         config.send_mail(mail)
         # then
-        _, kwargs = mock_create_channel_message.call_args
+        (
+            _,
+            kwargs,
+        ) = mock_create_discord_client.return_value.create_channel_message.call_args
         self.assertIn("@everyone", kwargs["content"])
 
 
 class TestRelayConfigOther(NoSocketsTestCase):
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
@@ -275,19 +282,21 @@
         with patch(MODELS_PATH + ".now") as mock_now:
             mock_now.return_value = dt.datetime(2021, 12, 24, 12, 30, tzinfo=utc)
             result = config.is_service_up
         # then
         self.assertIsNone(result)
 
 
-@patch(MANAGERS_PATH + ".DiscordClient.get_guild_channels", spec=True)
+@patch(MANAGERS_PATH + ".create_discordproxy_client", spec=True)
 class TestDiscordChannelManager(NoSocketsTestCase):
-    def test_should_create_new_channels_and_categories(self, mock_get_channels):
+    def test_should_create_new_channels_and_categories(
+        self, mock_create_discord_client
+    ):
         # given
-        mock_get_channels.return_value = [
+        mock_create_discord_client.return_value.get_guild_channels.return_value = [
             create_discordproxy_channel(id=1, name="alpha"),
             create_discordproxy_channel(id=2, name="bravo", parent_id=3),
             create_discordproxy_channel(
                 id=3, name="zulu", type=Channel.Type.GUILD_CATEGORY
             ),
         ]
         # when
@@ -298,17 +307,19 @@
         obj = DiscordChannel.objects.get(id=1)
         self.assertEqual(obj.name, "alpha")
         self.assertIsNone(obj.category)
         obj = DiscordChannel.objects.get(id=2)
         self.assertEqual(obj.name, "bravo")
         self.assertEqual(obj.category.name, "zulu")
 
-    def test_should_update_existing_channels_and_categores(self, mock_get_channels):
+    def test_should_update_existing_channels_and_categories(
+        self, mock_create_discord_client
+    ):
         # given
-        mock_get_channels.return_value = [
+        mock_create_discord_client.return_value.get_guild_channels.return_value = [
             create_discordproxy_channel(id=1, name="alpha"),
             create_discordproxy_channel(id=2, name="bravo", parent_id=3),
             create_discordproxy_channel(
                 id=3, name="zulu", type=Channel.Type.GUILD_CATEGORY
             ),
         ]
         create_discord_channel(id=1, name="update-me")
@@ -321,17 +332,19 @@
         obj = DiscordChannel.objects.get(id=1)
         self.assertEqual(obj.name, "alpha")
         obj = DiscordChannel.objects.get(id=2)
         self.assertEqual(obj.name, "bravo")
         obj = DiscordCategory.objects.get(id=3)
         self.assertEqual(obj.name, "zulu")
 
-    def test_should_remove_obsolete_channels_and_categories(self, mock_get_channels):
+    def test_should_remove_obsolete_channels_and_categories(
+        self, mock_create_discord_client
+    ):
         # given
-        mock_get_channels.return_value = [
+        mock_create_discord_client.return_value.get_guild_channels.return_value = [
             create_discordproxy_channel(id=1, name="alpha"),
             create_discordproxy_channel(id=2, name="bravo"),
         ]
         create_discord_channel(id=3, name="delete-me")
         create_discord_category(id=4, name="delete-me")
         # when
         result = DiscordChannel.objects.sync()
```

### Comparing `aa_mailrelay-1.3.0/mailrelay/tests/test_tasks.py` & `aa_mailrelay-1.4.0/mailrelay/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `aa_mailrelay-1.3.0/mailrelay/tests/test_views.py` & `aa_mailrelay-1.4.0/mailrelay/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `aa_mailrelay-1.3.0/mailrelay/utils.py` & `aa_mailrelay-1.4.0/mailrelay/utils.py`

 * *Files identical despite different names*

### Comparing `aa_mailrelay-1.3.0/mailrelay/views.py` & `aa_mailrelay-1.4.0/mailrelay/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,28 +7,25 @@
 from django.contrib.auth.decorators import login_required
 from django.shortcuts import redirect
 
 from allianceauth.services.hooks import get_extension_logger
 from app_utils.logging import LoggerAddTag
 
 from . import __title__
-from .app_settings import MAILRELAY_DISCORD_USER_TIMEOUT
 from .models import DiscordChannel
 
 logger = LoggerAddTag(get_extension_logger(__name__), __title__)
 
 
 @login_required
 @staff_member_required
 def admin_update_discord_channels(request):
     """View to update the discord channels."""
     try:
-        channels_count = DiscordChannel.objects.sync(
-            timeout=MAILRELAY_DISCORD_USER_TIMEOUT
-        )
+        channels_count = DiscordChannel.objects.sync()
         messages.success(
             request, f"Successfully updated {channels_count} channels from Discord."
         )
     except DiscordProxyException as ex:
         logger.error("Failed to fetch channels from Discord", exc_info=True)
         messages.warning(request, f"Failed to fetch channels from Discord: {ex}")
     return redirect("admin:mailrelay_relayconfig_changelist")
```

### Comparing `aa_mailrelay-1.3.0/pyproject.toml` & `aa_mailrelay-1.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
 ]
 dependencies = [
     "aa-memberaudit>=3.7.0",
     "allianceauth-app-utils>=1.19",
     "allianceauth>=3",
-    "discordproxy>=1",
+    "discordproxy>=1.3.2",
     "django-eveuniverse>=1",
 ]
 
 [project.urls]
 Homepage = "https://gitlab.com/ErikKalkoken/aa-mailrelay"
 
 [tool.flit.module]
```

### Comparing `aa_mailrelay-1.3.0/PKG-INFO` & `aa_mailrelay-1.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-mailrelay
-Version: 1.3.0
+Version: 1.4.0
 Summary: An app for relaying Eve mails to Discord.
 Author-email: Erik Kalkoken <kalkoken87@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Dist: aa-memberaudit>=3.7.0
 Requires-Dist: allianceauth-app-utils>=1.19
 Requires-Dist: allianceauth>=3
-Requires-Dist: discordproxy>=1
+Requires-Dist: discordproxy>=1.3.2
 Requires-Dist: django-eveuniverse>=1
 Project-URL: Homepage, https://gitlab.com/ErikKalkoken/aa-mailrelay
 
 # Mailrelay
 
 An app for relaying Eve mails to Discord.
 
@@ -115,12 +115,13 @@
 
 Here is a list of available settings for this app. They can be configured by adding them to your AA settings file (`local.py`).
 
 Note that all settings are optional and the app will use the documented default settings if they are not used.
 
 Name|Description|Default
 --|--|--
-`MAILRELAY_DISCORD_TASK_TIMEOUT`|Timeout for asynchronous Discord requests in seconds.|`60`
-`MAILRELAY_DISCORD_USER_TIMEOUT`|Timeout for user facing Discord requests in seconds.|`30`
+`DISCORDPROXY_HOST`|Port used to communicate with Discord Proxy.|`localhost`
+`DISCORDPROXY_PORT`|Host used to communicate with Discord Proxy.|`50051`
+`MAILRELAY_DISCORDPROXY_TIMEOUT`|Timeout for sending request to DISCORDPROXY in seconds.|`30`
 `MAILRELAY_OLDEST_MAIL_HOURS`|Oldest mail to be forwarded in hours. Set to 0 to disable.|`2`
 `MAILRELAY_RELAY_GRACE_MINUTES`|Max time in minutes since last successful relay before service is reported as down.|`30`
```

