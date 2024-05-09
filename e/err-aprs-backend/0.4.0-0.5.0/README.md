# Comparing `tmp/err_aprs_backend-0.4.0.tar.gz` & `tmp/err_aprs_backend-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "err_aprs_backend-0.4.0.tar", max compression
+gzip compressed data, was "err_aprs_backend-0.5.0.tar", max compression
```

## Comparing `err_aprs_backend-0.4.0.tar` & `err_aprs_backend-0.5.0.tar`

### file list

```diff
@@ -1,30 +1,39 @@
--rw-r--r--   0        0        0     1063 2024-05-05 15:58:45.130718 err_aprs_backend-0.4.0/LICENSE
--rw-r--r--   0        0        0     4600 2024-05-05 15:58:45.130718 err_aprs_backend-0.4.0/README.md
--rw-r--r--   0        0        0      105 2024-05-05 15:58:45.130718 err_aprs_backend-0.4.0/aprs_backend/__init__.py
--rw-r--r--   0        0        0       81 2024-05-05 15:58:45.130718 err_aprs_backend-0.4.0/aprs_backend/aprs.plug
--rw-r--r--   0        0        0    20931 2024-05-05 15:58:45.130718 err_aprs_backend-0.4.0/aprs_backend/aprs.py
--rw-r--r--   0        0        0      212 2024-05-05 15:58:45.130718 err_aprs_backend-0.4.0/aprs_backend/clients/__init__.py
--rw-r--r--   0        0        0      959 2024-05-05 15:58:45.130718 err_aprs_backend-0.4.0/aprs_backend/clients/_base.py
--rw-r--r--   0        0        0     2174 2024-05-05 15:58:45.130718 err_aprs_backend-0.4.0/aprs_backend/clients/aprs_registry.py
--rw-r--r--   0        0        0     6945 2024-05-05 15:58:45.130718 err_aprs_backend-0.4.0/aprs_backend/clients/aprsis.py
--rw-r--r--   0        0        0     1560 2024-05-05 15:58:45.134718 err_aprs_backend-0.4.0/aprs_backend/clients/beacon.py
--rw-r--r--   0        0        0       82 2024-05-05 15:58:45.134718 err_aprs_backend-0.4.0/aprs_backend/clients/kiss.py
--rw-r--r--   0        0        0      562 2024-05-05 15:58:45.134718 err_aprs_backend-0.4.0/aprs_backend/exceptions/__init__.py
--rw-r--r--   0        0        0       48 2024-05-05 15:58:45.134718 err_aprs_backend-0.4.0/aprs_backend/exceptions/base.py
--rw-r--r--   0        0        0      158 2024-05-05 15:58:45.134718 err_aprs_backend-0.4.0/aprs_backend/exceptions/client/__init__.py
--rw-r--r--   0        0        0      396 2024-05-05 15:58:45.134718 err_aprs_backend-0.4.0/aprs_backend/exceptions/client/aprsis.py
--rw-r--r--   0        0        0      118 2024-05-05 15:58:45.134718 err_aprs_backend-0.4.0/aprs_backend/exceptions/packets/__init__.py
--rw-r--r--   0        0        0      112 2024-05-05 15:58:45.134718 err_aprs_backend-0.4.0/aprs_backend/exceptions/packets/parser.py
--rw-r--r--   0        0        0      117 2024-05-05 15:58:45.134718 err_aprs_backend-0.4.0/aprs_backend/exceptions/processor.py
--rw-r--r--   0        0        0      744 2024-05-05 15:58:45.134718 err_aprs_backend-0.4.0/aprs_backend/message.py
--rw-r--r--   0        0        0     9038 2024-05-05 15:58:45.134718 err_aprs_backend-0.4.0/aprs_backend/packets/__init__.py
--rw-r--r--   0        0        0    10116 2024-05-05 15:58:45.134718 err_aprs_backend-0.4.0/aprs_backend/packets/parser.py
--rw-r--r--   0        0        0     1038 2024-05-05 15:58:45.134718 err_aprs_backend-0.4.0/aprs_backend/person.py
--rw-r--r--   0        0        0       83 2024-05-05 15:58:45.134718 err_aprs_backend-0.4.0/aprs_backend/room.py
--rw-r--r--   0        0        0      495 2024-05-05 15:58:45.134718 err_aprs_backend-0.4.0/aprs_backend/utils/__init__.py
--rw-r--r--   0        0        0      975 2024-05-05 15:58:45.134718 err_aprs_backend-0.4.0/aprs_backend/utils/counter.py
--rw-r--r--   0        0        0      118 2024-05-05 15:58:45.134718 err_aprs_backend-0.4.0/aprs_backend/utils/datetime.py
--rw-r--r--   0        0        0      565 2024-05-05 15:58:45.134718 err_aprs_backend-0.4.0/aprs_backend/utils/position.py
--rw-r--r--   0        0        0       22 2024-05-05 15:58:45.134718 err_aprs_backend-0.4.0/aprs_backend/version.py
--rw-r--r--   0        0        0     1412 2024-05-05 15:58:45.134718 err_aprs_backend-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     5272 1970-01-01 00:00:00.000000 err_aprs_backend-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-09 23:51:57.882527 err_aprs_backend-0.5.0/LICENSE
+-rw-r--r--   0        0        0     4600 2024-05-09 23:51:57.882527 err_aprs_backend-0.5.0/README.md
+-rw-r--r--   0        0        0      165 2024-05-09 23:51:57.882527 err_aprs_backend-0.5.0/aprs_backend/APRSHealth.plug
+-rw-r--r--   0        0        0      161 2024-05-09 23:51:57.882527 err_aprs_backend-0.5.0/aprs_backend/APRSHelp.plug
+-rw-r--r--   0        0        0      165 2024-05-09 23:51:57.882527 err_aprs_backend-0.5.0/aprs_backend/APRSWebserver.plug
+-rw-r--r--   0        0        0      105 2024-05-09 23:51:57.882527 err_aprs_backend-0.5.0/aprs_backend/__init__.py
+-rw-r--r--   0        0        0      138 2024-05-09 23:51:57.882527 err_aprs_backend-0.5.0/aprs_backend/aprs.plug
+-rw-r--r--   0        0        0    21550 2024-05-09 23:51:57.882527 err_aprs_backend-0.5.0/aprs_backend/aprs.py
+-rw-r--r--   0        0        0      188 2024-05-09 23:51:57.882527 err_aprs_backend-0.5.0/aprs_backend/aprs_core_plugins.py
+-rw-r--r--   0        0        0      212 2024-05-09 23:51:57.882527 err_aprs_backend-0.5.0/aprs_backend/clients/__init__.py
+-rw-r--r--   0        0        0      959 2024-05-09 23:51:57.882527 err_aprs_backend-0.5.0/aprs_backend/clients/_base.py
+-rw-r--r--   0        0        0     2174 2024-05-09 23:51:57.882527 err_aprs_backend-0.5.0/aprs_backend/clients/aprs_registry.py
+-rw-r--r--   0        0        0     6945 2024-05-09 23:51:57.882527 err_aprs_backend-0.5.0/aprs_backend/clients/aprsis.py
+-rw-r--r--   0        0        0     1560 2024-05-09 23:51:57.882527 err_aprs_backend-0.5.0/aprs_backend/clients/beacon.py
+-rw-r--r--   0        0        0       82 2024-05-09 23:51:57.882527 err_aprs_backend-0.5.0/aprs_backend/clients/kiss.py
+-rw-r--r--   0        0        0      562 2024-05-09 23:51:57.882527 err_aprs_backend-0.5.0/aprs_backend/exceptions/__init__.py
+-rw-r--r--   0        0        0       48 2024-05-09 23:51:57.882527 err_aprs_backend-0.5.0/aprs_backend/exceptions/base.py
+-rw-r--r--   0        0        0      158 2024-05-09 23:51:57.882527 err_aprs_backend-0.5.0/aprs_backend/exceptions/client/__init__.py
+-rw-r--r--   0        0        0      396 2024-05-09 23:51:57.886527 err_aprs_backend-0.5.0/aprs_backend/exceptions/client/aprsis.py
+-rw-r--r--   0        0        0      118 2024-05-09 23:51:57.886527 err_aprs_backend-0.5.0/aprs_backend/exceptions/packets/__init__.py
+-rw-r--r--   0        0        0      112 2024-05-09 23:51:57.886527 err_aprs_backend-0.5.0/aprs_backend/exceptions/packets/parser.py
+-rw-r--r--   0        0        0      117 2024-05-09 23:51:57.886527 err_aprs_backend-0.5.0/aprs_backend/exceptions/processor.py
+-rw-r--r--   0        0        0      744 2024-05-09 23:51:57.886527 err_aprs_backend-0.5.0/aprs_backend/message.py
+-rw-r--r--   0        0        0     9038 2024-05-09 23:51:57.886527 err_aprs_backend-0.5.0/aprs_backend/packets/__init__.py
+-rw-r--r--   0        0        0    10116 2024-05-09 23:51:57.886527 err_aprs_backend-0.5.0/aprs_backend/packets/parser.py
+-rw-r--r--   0        0        0     1038 2024-05-09 23:51:57.886527 err_aprs_backend-0.5.0/aprs_backend/person.py
+-rw-r--r--   0        0        0      204 2024-05-09 23:51:57.886527 err_aprs_backend-0.5.0/aprs_backend/plugins/__init__.py
+-rw-r--r--   0        0        0     2099 2024-05-09 23:51:57.886527 err_aprs_backend-0.5.0/aprs_backend/plugins/health.py
+-rw-r--r--   0        0        0      695 2024-05-09 23:51:57.886527 err_aprs_backend-0.5.0/aprs_backend/plugins/help.py
+-rw-r--r--   0        0        0     2345 2024-05-09 23:51:57.886527 err_aprs_backend-0.5.0/aprs_backend/plugins/web.py
+-rw-r--r--   0        0        0       83 2024-05-09 23:51:57.886527 err_aprs_backend-0.5.0/aprs_backend/room.py
+-rw-r--r--   0        0        0      495 2024-05-09 23:51:57.886527 err_aprs_backend-0.5.0/aprs_backend/utils/__init__.py
+-rw-r--r--   0        0        0      975 2024-05-09 23:51:57.886527 err_aprs_backend-0.5.0/aprs_backend/utils/counter.py
+-rw-r--r--   0        0        0      118 2024-05-09 23:51:57.886527 err_aprs_backend-0.5.0/aprs_backend/utils/datetime.py
+-rw-r--r--   0        0        0     8386 2024-05-09 23:51:57.886527 err_aprs_backend-0.5.0/aprs_backend/utils/plugins.py
+-rw-r--r--   0        0        0      565 2024-05-09 23:51:57.886527 err_aprs_backend-0.5.0/aprs_backend/utils/position.py
+-rw-r--r--   0        0        0       22 2024-05-09 23:51:57.886527 err_aprs_backend-0.5.0/aprs_backend/version.py
+-rw-r--r--   0        0        0     1483 2024-05-09 23:51:57.886527 err_aprs_backend-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5272 1970-01-01 00:00:00.000000 err_aprs_backend-0.5.0/PKG-INFO
```

### Comparing `err_aprs_backend-0.4.0/LICENSE` & `err_aprs_backend-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.4.0/README.md` & `err_aprs_backend-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.4.0/aprs_backend/aprs.py` & `err_aprs_backend-0.5.0/aprs_backend/aprs.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,43 +3,48 @@
 from aprs_backend.message import APRSMessage
 from aprs_backend.clients import APRSISClient
 from aprs_backend.person import APRSPerson
 from aprs_backend.room import APRSRoom
 from aprs_backend.version import __version__ as ERR_APRS_VERSION
 from errbot.backends.base import Message
 from errbot.backends.base import ONLINE
+from errbot.plugin_manager import BotPluginManager
 from errbot.core import ErrBot
 from aprs_backend.exceptions import ProcessorError, PacketParseError, APRSISConnnectError
 from aprs_backend.packets.parser import parse, hash_packet
 from expiringdict import ExpiringDict
 from functools import cached_property
 from aprs_backend.packets import AckPacket, RejectPacket, MessagePacket, BeaconPacket
 from aprs_backend.utils.counter import MessageCounter
 from random import randint
 from datetime import datetime
+
 from better_profanity import profanity
 from aprs_backend.clients.aprs_registry import APRSRegistryClient, RegistryAppConfig
 import logging
 import asyncio
 from errbot.version import VERSION as ERR_VERSION
 from aprs_backend.clients.beacon import BeaconConfig, BeaconClient
+from aprs_backend.utils.plugins import _load_plugins_generic, activate_non_started_plugins
+from types import MethodType
+
 
 log = logging.getLogger(__name__)
 
 for handler in log.handlers:
     handler.setFormatter(
         logging.Formatter("%(filename)s: " "%(levelname)s: " "%(funcName)s(): " "%(lineno)d:\t" "%(message)s")
     )
 
 
 class APRSBackend(ErrBot):
     def __init__(self, config):
-        log.debug("Initied")
+        super().__init__(config)
+        log.debug("Init called")
 
-        self._errbot_config = config
         self._multiline = False
 
         aprs_config = {"host": "rotate.aprs.net", "port": 14580}
         aprs_config.update(config.BOT_IDENTITY)
         aprs_config["aprs_app_name"] = "ErrbotAPRS"
         aprs_config["app_version"] = f"{ERR_APRS_VERSION}:{ERR_VERSION}"
 
@@ -60,17 +65,14 @@
             # bot is using a different callsign from the signin, add it to the filter
             aprs_config["aprs_filter"] = f"g/{aprs_config['callsign']}/{self.callsign}"
             self.listening_callsigns.append(self.callsign)
         self._client = APRSISClient(**aprs_config, logger=log)
         self._send_queue: asyncio.Queue[MessagePacket] = asyncio.Queue(
             maxsize=int(self._get_from_config("APRS_SEND_MAX_QUEUE", "2048"))
         )
-        self.help_text = self._get_from_config(
-            "APRS_HELP_TEXT", f"Errbot {ERR_VERSION} & err-aprs-backend {ERR_APRS_VERSION} by {aprs_config['callsign']}"
-        )
 
         self._message_counter = MessageCounter(initial_value=randint(1, 20))  # nosec not used cryptographically
         self._max_dropped_packets = int(self._get_from_config("APRS_MAX_DROPPED_PACKETS", "25"))
         self._max_cached_packets = int(self._get_from_config("APRS_MAX_CACHED_PACKETS", "2048"))
         self._message_max_retry = int(self._get_from_config("APRS_MESSAGE_MAX_RETRIES", "7"))
         self._message_retry_wait = int(self._get_from_config("APRS_MESSAGE_RETRY_WAIT", "90"))
 
@@ -121,18 +123,31 @@
                 beacon_config=self.beacon_config,
                 send_queue=self._send_queue,
                 log=log,
                 frequency_seconds=int(self._get_from_config("APRS_BEACON_INTERVAL_SECONDS", "1200")),
             )
         else:
             self.beacon_client = None
-        super().__init__(config)
+
+    def attach_plugin_manager(self, plugin_manager: BotPluginManager | None) -> None:
+        """Modified attach_plugin_manager that patches the plugin manager
+
+        _log_plugins_generic is modified to remove a check on multiple plugin classes in
+        a single module
+        """
+        log.debug("In aprs-backend attach_plugin_manager")
+        if plugin_manager is not None:
+            log.debug("Patching plugin manager with custom _load_plugins_generic")
+            funcType = MethodType
+            plugin_manager._load_plugins_generic = funcType(_load_plugins_generic, plugin_manager)
+            plugin_manager.activate_non_started_plugins = funcType(activate_non_started_plugins, plugin_manager)
+        self.plugin_manager = plugin_manager
 
     def _get_from_config(self, key: str, default: any = None) -> any:
-        return getattr(self._errbot_config, key, default)
+        return getattr(self.bot_config, key, default)
 
     def _get_beacon_config(self) -> BeaconConfig | None:
         if self._get_from_config("APRS_BEACON_ENABLE", "false") == "true":
             return None
         beacon_config = {}
         beacon_config["latitude"] = self._get_from_config("APRS_BEACON_LATITUDE", None)
         beacon_config["longitude"] = self._get_from_config("APRS_BEACON_LONGITUDE", None)
@@ -313,14 +328,21 @@
             log.info("Interrupt received, shutting down..")
             return True
         except Exception as exc:
             log.error("Fatal unhandled error reading from APRS %s", exc)
             return False
 
     async def async_serve_once(self) -> bool:
+        """The async portion of serve once
+
+        Starts the bot tasks for receiving aprs messages, sending messages, and retrying
+        """
+        log.debug(
+            "Bot plugins: %s", [plugin.__class__.__name__ for plugin in self.plugin_manager.get_all_active_plugins()]
+        )
         receive_task = asyncio.create_task(self.receive_worker())
 
         worker_tasks = [asyncio.create_task(self.send_worker()), asyncio.create_task(self.retry_worker())]
         # if reporting to the aprs service registry is enabled, start a task for it
         if self.registry_client is not None:
             worker_tasks.append(asyncio.create_task(self.registry_client()))
         if self.beacon_client is not None:
@@ -422,21 +444,14 @@
         async with self._waiting_ack_lock:
             packet = self._waiting_ack.pop(message_hash)
         if packet is None:
             log.error("Tried to drop hash %s and it didn't exist in waiting ack", message_hash)
         else:
             log.debug("Dropped Packet from waiting_ack: %s", packet)
 
-    def handle_help(self, msg: APRSMessage) -> None:
-        """Returns simplified help text for the APRS backend"""
-        help_msg = APRSMessage(body=self.help_text, extras=msg.extras)
-        help_msg.to = msg.frm
-        help_msg.frm = self.bot_identifier
-        self.send_message(help_msg)
-
     async def _process_message(self, packet: MessagePacket) -> None:
         """
         Check if this message is a dupe of one the bot is already processing
         (waiting for an ack), and dispatch it to plugins
         """
         log.debug(packet.raw_dict)
         # send an ack to this message
@@ -445,16 +460,14 @@
         async with self._packet_cache_lock:
             if self._packet_cache.get(this_packet_hash, None) is not None:
                 log.info("Duplicate packet %s. Skipping processing", packet.json)
                 return
             self._packet_cache[this_packet_hash] = packet
         msg = APRSMessage.from_message_packet(packet)
         msg.body = msg.body.strip("\n").strip("\r")
-        if msg.body.lower().strip(" ") == "help":
-            return self.handle_help(msg)
         return self.callback_message(msg)
 
     async def _ack_message(self, packet: MessagePacket) -> None:
         log.debug("Sending ack for packet %s", packet.json)
         this_ack = AckPacket(
             from_call=packet.to, to_call=packet.from_call, addresse=packet.from_call, msgNo=packet.msgNo
         )
```

### Comparing `err_aprs_backend-0.4.0/aprs_backend/clients/_base.py` & `err_aprs_backend-0.5.0/aprs_backend/clients/_base.py`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.4.0/aprs_backend/clients/aprs_registry.py` & `err_aprs_backend-0.5.0/aprs_backend/clients/aprs_registry.py`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.4.0/aprs_backend/clients/aprsis.py` & `err_aprs_backend-0.5.0/aprs_backend/clients/aprsis.py`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.4.0/aprs_backend/clients/beacon.py` & `err_aprs_backend-0.5.0/aprs_backend/clients/beacon.py`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.4.0/aprs_backend/exceptions/__init__.py` & `err_aprs_backend-0.5.0/aprs_backend/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.4.0/aprs_backend/message.py` & `err_aprs_backend-0.5.0/aprs_backend/message.py`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.4.0/aprs_backend/packets/__init__.py` & `err_aprs_backend-0.5.0/aprs_backend/packets/__init__.py`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.4.0/aprs_backend/packets/parser.py` & `err_aprs_backend-0.5.0/aprs_backend/packets/parser.py`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.4.0/aprs_backend/person.py` & `err_aprs_backend-0.5.0/aprs_backend/person.py`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.4.0/aprs_backend/utils/counter.py` & `err_aprs_backend-0.5.0/aprs_backend/utils/counter.py`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.4.0/aprs_backend/utils/position.py` & `err_aprs_backend-0.5.0/aprs_backend/utils/position.py`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.4.0/pyproject.toml` & `err_aprs_backend-0.5.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "err-aprs-backend"
-version = "0.4.0"
+version = "0.5.0"
 description = "Errbot APRS backend plugin"
 authors = ["Andrew Herrington <andrew.the.techie@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "aprs_backend"}]
 include = ["*.plug"]
 
@@ -18,24 +18,27 @@
 
 
 [tool.poetry.plugins]
 
 [tool.poetry.plugins."errbot.backend_plugins"]
 aprs = "aprs_backend:APRSBackend"
 
+[tool.poetry.plugins."errbot.plugins"]
+help = "aprs_backend:APRSHelp"
+
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
 coverage = {extras = ["toml"], version = ">=6.5,<8.0"}
 pre-commit = ">=2.12.1"
 pep8-naming = "^0.13.2"
 reorder-python-imports = "^3.9.0"
 pre-commit-hooks = "^4.2.0"
 pyupgrade = "^3.15.2"
 pytest-xdist = "^3.1.0"
-ruff = ">=0.0.249,<0.4.3"
+ruff = ">=0.0.249,<0.4.4"
 bandit = "^1.7.8"
 pytest-subtests = "^0.12.1"
 pytest-cov = "^5.0.0"
 pytest-asyncio = "^0.23.6"
 pytest-httpx = "^0.30.0"
```

### Comparing `err_aprs_backend-0.4.0/PKG-INFO` & `err_aprs_backend-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: err-aprs-backend
-Version: 0.4.0
+Version: 0.5.0
 Summary: Errbot APRS backend plugin
 License: MIT
 Author: Andrew Herrington
 Author-email: andrew.the.techie@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

