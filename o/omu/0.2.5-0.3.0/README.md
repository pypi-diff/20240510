# Comparing `tmp/omu-0.2.5.tar.gz` & `tmp/omu-0.3.0.tar.gz`

## Comparing `omu-0.2.5.tar` & `omu-0.3.0.tar`

### file list

```diff
@@ -1,60 +1,69 @@
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/__init__.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/app.py
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/event_emitter.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/helper.py
--rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/identifier.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/model.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/plugin.py
--rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/serializer.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/client/__init__.py
--rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/client/client.py
--rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/client/omuclient.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/__init__.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/extension.py
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/extension_registry.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/asset/__init__.py
--rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/asset/asset_extension.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/dashboard/__init__.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/dashboard/dashboard.py
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/dashboard/dashboard_extension.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/endpoint/__init__.py
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/endpoint/endpoint.py
--rw-r--r--   0        0        0     6277 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/endpoint/endpoint_extension.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/i18n/__init__.py
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/i18n/i18n_extension.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/message/__init__.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/message/message.py
--rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/message/message_extension.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/permission/__init__.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/permission/permission.py
--rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/permission/permission_extension.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/plugin/__init__.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/plugin/plugin_extension.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/registry/__init__.py
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/registry/registry.py
--rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/registry/registry_extension.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/server/__init__.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/server/server_extension.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/table/__init__.py
--rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/table/table.py
--rw-r--r--   0        0        0    15097 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/table/table_extension.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/interface/__init__.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/interface/keyable.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/interface/named.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/localization/__init__.py
--rw-r--r--   0        0        0    33905 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/localization/locale.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/localization/localization.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/network/__init__.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/network/address.py
--rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/network/bytebuffer.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/network/connection.py
--rw-r--r--   0        0        0     5470 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/network/network.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/network/packet_mapper.py
--rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/network/websocket_connection.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/network/packet/__init__.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/network/packet/packet.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/network/packet/packet_types.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omu-0.2.5/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omu-0.2.5/README.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 omu-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 omu-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/__init__.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/address.py
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/app.py
+-rw-r--r--   0        0        0     5078 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/bytebuffer.py
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/errors.py
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/event_emitter.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/helper.py
+-rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/identifier.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/model.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/plugin.py
+-rw-r--r--   0        0        0     4410 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/serializer.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/version.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/client/__init__.py
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/client/client.py
+-rw-r--r--   0        0        0     5618 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/client/omuclient.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/client/token.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/extension/__init__.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/extension/extension.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/extension/extension_registry.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/extension/asset/__init__.py
+-rw-r--r--   0        0        0     4368 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/extension/asset/asset_extension.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/extension/dashboard/__init__.py
+-rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/extension/dashboard/dashboard_extension.py
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/extension/dashboard/packets.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/extension/endpoint/__init__.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/extension/endpoint/endpoint.py
+-rw-r--r--   0        0        0     5910 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/extension/endpoint/endpoint_extension.py
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/extension/endpoint/packets.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/extension/i18n/__init__.py
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/extension/i18n/i18n_extension.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/extension/permission/__init__.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/extension/permission/permission.py
+-rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/extension/permission/permission_extension.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/extension/plugin/__init__.py
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/extension/plugin/package_info.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/extension/plugin/plugin.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/extension/plugin/plugin_extension.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/extension/registry/__init__.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/extension/registry/packets.py
+-rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/extension/registry/registry.py
+-rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/extension/registry/registry_extension.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/extension/server/__init__.py
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/extension/server/server_extension.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/extension/signal/__init__.py
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/extension/signal/packets.py
+-rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/extension/signal/signal.py
+-rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/extension/signal/signal_extension.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/extension/table/__init__.py
+-rw-r--r--   0        0        0     7542 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/extension/table/packets.py
+-rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/extension/table/table.py
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/extension/table/table_extension.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/interface/__init__.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/interface/keyable.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/interface/named.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/localization/__init__.py
+-rw-r--r--   0        0        0    33932 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/localization/locale.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/localization/localization.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/network/__init__.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/network/connection.py
+-rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/network/network.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/network/packet_mapper.py
+-rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/network/websocket_connection.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/network/packet/__init__.py
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/network/packet/packet.py
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 omu-0.3.0/src/omu/network/packet/packet_types.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 omu-0.3.0/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omu-0.3.0/README.md
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 omu-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 omu-0.3.0/PKG-INFO
```

### Comparing `omu-0.2.5/src/omu/app.py` & `omu-0.3.0/src/omu/app.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,72 +1,71 @@
 from __future__ import annotations
 
-from typing import Final, List, NotRequired, TypedDict
+from typing import Final, NotRequired, TypedDict
 
 from omu.identifier import Identifier
 from omu.interface import Keyable
-from omu.localization import LocalizedText
-from omu.localization.locale import Locale
+from omu.localization import Locale, LocalizedText
 from omu.model import Model
 
 
 class AppMetadata(TypedDict):
     locale: Locale
     name: NotRequired[LocalizedText]
     description: NotRequired[LocalizedText]
     image: NotRequired[LocalizedText]
     site: NotRequired[LocalizedText]
     repository: NotRequired[LocalizedText]
     authors: NotRequired[LocalizedText]
     license: NotRequired[LocalizedText]
-    tags: NotRequired[List[str]]
+    tags: NotRequired[list[str]]
 
 
 class AppJson(TypedDict):
-    identifier: str
+    id: str
     version: NotRequired[str] | None
     url: NotRequired[str] | None
     metadata: NotRequired[AppMetadata] | None
 
 
 class App(Keyable, Model[AppJson]):
     def __init__(
         self,
-        identifier: Identifier | str,
+        id: Identifier | str,
         *,
         version: str | None = None,
         url: str | None = None,
         metadata: AppMetadata | None = None,
     ) -> None:
-        if isinstance(identifier, str):
-            identifier = Identifier.from_key(identifier)
-        self.identifier: Final[Identifier] = identifier
+        if isinstance(id, str):
+            id = Identifier.from_key(id)
+        self.id: Final[Identifier] = id
         self.version = version
         self.url = url
         self.metadata = metadata
 
     @classmethod
     def from_json(cls, json: AppJson) -> App:
-        identifier = Identifier.from_key(json["identifier"])
+        id = Identifier.from_key(json["id"])
         return cls(
-            identifier,
+            id,
             version=json.get("version"),
             url=json.get("url"),
             metadata=json.get("metadata"),
         )
 
     def to_json(self) -> AppJson:
         return AppJson(
-            identifier=self.key(),
+            id=self.key(),
             version=self.version,
             url=self.url,
             metadata=self.metadata,
         )
 
     def key(self) -> str:
-        return self.identifier.key()
+        return self.id.key()
 
     def __hash__(self) -> int:
         return hash(self.key())
 
     def __repr__(self) -> str:
         return f"App({self.key()})"
```

### Comparing `omu-0.2.5/src/omu/event_emitter.py` & `omu-0.3.0/src/omu/event_emitter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,65 @@
 from __future__ import annotations
 
 import asyncio
-from typing import Callable, List, Self
+from collections.abc import Callable
+from typing import Self
 
 from omu.helper import Coro
 
+type Unlisten = Callable[[], None]
+
 
 class EventEmitter[**P]:
     def __init__(
         self,
         on_subscribe: Callable[[], None] | Coro[[], None] | None = None,
         on_empty: Callable[[], None] | Coro[[], None] | None = None,
     ) -> None:
         self.on_subscribe = on_subscribe
         self.on_empty = on_empty
-        self._listeners: List[Callable[P, None] | Coro[P, None]] = []
+        self._listeners: list[Callable[P, None] | Coro[P, None]] = []
+        self.closed = False
 
     @property
     def empty(self) -> bool:
         return len(self._listeners) == 0
 
-    def subscribe(self, listener: Callable[P, None] | Coro[P, None]) -> None:
+    def close(self) -> None:
+        self.closed = True
+        self._listeners.clear()
+
+    def listen(self, listener: Callable[P, None] | Coro[P, None]) -> Unlisten:
+        if self.closed:
+            raise ValueError("EventEmitter is closed")
         if listener in self._listeners:
             raise ValueError("Listener already subscribed")
         if self.on_subscribe and len(self._listeners) == 0:
             coroutine = self.on_subscribe()
             if asyncio.iscoroutine(coroutine):
                 asyncio.create_task(coroutine)
         self._listeners.append(listener)
+        return lambda: self.unlisten(listener)
 
-    def unsubscribe(self, listener: Callable[P, None] | Coro[P, None]) -> None:
+    def unlisten(self, listener: Callable[P, None] | Coro[P, None]) -> None:
         if listener not in self._listeners:
             return
         self._listeners.remove(listener)
         if self.on_empty and len(self._listeners) == 0:
             coroutine = self.on_empty()
             if asyncio.iscoroutine(coroutine):
                 asyncio.create_task(coroutine)
 
-    def __iadd__(self, listener: Callable[P, None] | Coro[P, None]) -> Self:
-        self.subscribe(listener)
-        return self
-
-    def __isub__(self, listener: Callable[P, None] | Coro[P, None]) -> Self:
-        self.unsubscribe(listener)
-        return self
-
     async def emit(self, *args: P.args, **kwargs: P.kwargs) -> None:
+        if self.closed:
+            raise ValueError("EventEmitter is closed")
         for listener in tuple(self._listeners):
             if asyncio.iscoroutinefunction(listener):
                 await listener(*args, **kwargs)
             else:
                 listener(*args, **kwargs)
 
+    def __iadd__(self, listener: Callable[P, None] | Coro[P, None]) -> Self:
+        self.listen(listener)
+        return self
+
     __call__ = emit
```

### Comparing `omu-0.2.5/src/omu/helper.py` & `omu-0.3.0/src/omu/helper.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import re
 import typing
 
 type AsyncCallback[**P] = typing.Callable[P, typing.Coroutine[None, None, None]]
 type Coro[**P, T] = typing.Callable[P, typing.Coroutine[None, None, T]]
 
 
-def instance[T](cls: typing.Type[T]) -> T:
+def instance[T](cls: type[T]) -> T:
     return cls()
 
 
 def map_optional[V, T](
     data: V | None, func: typing.Callable[[V], T], default: T | None = None
 ) -> T | None:
     if data is None:
@@ -25,7 +25,15 @@
 
 def sanitize_filename(name: str) -> str:
     return sanitize_re.sub("_", name)
 
 
 def generate_md5_hash(id: str) -> str:
     return hashlib.md5(id.encode()).hexdigest()
+
+
+def batch_call(*funcs: typing.Callable[[], None]) -> typing.Callable[[], None]:
+    def wrapper():
+        for func in funcs:
+            func()
+
+    return wrapper
```

### Comparing `omu-0.2.5/src/omu/identifier.py` & `omu-0.3.0/src/omu/identifier.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from __future__ import annotations
 
 import re
 import urllib.parse
 from pathlib import Path
-from typing import Final, Tuple
+from typing import Final
 
 from omu.helper import generate_md5_hash, sanitize_filename
 from omu.model import Model
 
 from .interface import Keyable
 
 NAMESPACE_REGEX = re.compile(r"^(\.[^/:.]|[\w-])+$")
 NAME_REGEX = re.compile(r"^[^/:.]+$")
 
 
 class Identifier(Model[str], Keyable):
     def __init__(self, namespace: str, *path: str) -> None:
         self.validate(namespace, *path)
         self.namespace: Final[str] = namespace
-        self.path: Final[Tuple[str, ...]] = path
+        self.path: Final[tuple[str, ...]] = path
 
     @classmethod
     def validate(cls, namespace: str, *path: str) -> None:
         if not namespace:
             raise Exception("Invalid namespace: Namespace cannot be empty")
         if len(path) == 0:
             raise Exception("Invalid path: Path must have at least one name")
@@ -75,20 +75,32 @@
 
     def get_sanitized_path(self) -> Path:
         namespace = (
             f"{sanitize_filename(self.namespace)}-{generate_md5_hash(self.namespace)}"
         )
         return Path(namespace, *self.path)
 
-    def is_subpart_of(self, base: Identifier) -> bool:
+    def is_subpath_of(self, base: Identifier) -> bool:
         return (
             self.namespace == base.namespace
             and self.path[: len(base.path)] == base.path
         )
 
+    def is_namepath_equal(
+        self,
+        other: Identifier,
+        path_length: int | None = None,
+    ) -> bool:
+        if path_length is None:
+            path_length = len(self.path)
+        return (
+            self.namespace == other.namespace
+            and self.path[:path_length] == other.path[:path_length]
+        )
+
     def join(self, *path: str) -> Identifier:
         return Identifier(self.namespace, *self.path, *path)
 
     def __truediv__(self, name: str) -> Identifier:
         return self.join(name)
 
     def __eq__(self, other: object) -> bool:
```

### Comparing `omu-0.2.5/src/omu/plugin.py` & `omu-0.3.0/src/omu/plugin.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+from collections.abc import Callable
 from dataclasses import dataclass
-from typing import Callable
 
 from omuserver.server import Server
 
 from omu.helper import Coro
 
 from .client import Client
```

### Comparing `omu-0.2.5/src/omu/serializer.py` & `omu-0.3.0/src/omu/serializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import abc
 import json
-from typing import Callable, Mapping, Protocol
+from collections.abc import Callable, Mapping
+from typing import Protocol
 
 
 class SerializeError(Exception):
     pass
 
 
 class Serializable[T, D](Protocol):
```

### Comparing `omu-0.2.5/src/omu/client/client.py` & `omu-0.3.0/src/omu/client/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,46 @@
 from __future__ import annotations
 
 import abc
 import asyncio
 from typing import TYPE_CHECKING
 
-from omu.event_emitter import EventEmitter
+from omu.app import App
+from omu.event_emitter import EventEmitter, Unlisten
+from omu.helper import Coro
 
 if TYPE_CHECKING:
-    from omu.app import App
     from omu.extension import ExtensionRegistry
     from omu.extension.dashboard import DashboardExtension
     from omu.extension.endpoint import EndpointExtension
     from omu.extension.i18n import I18nExtension
-    from omu.extension.message import MessageExtension
     from omu.extension.permission import PermissionExtension
+    from omu.extension.plugin import PluginExtension
     from omu.extension.registry import RegistryExtension
     from omu.extension.server import ServerExtension
+    from omu.extension.signal import SignalExtension
     from omu.extension.table import TableExtension
     from omu.network import Network
     from omu.network.packet import PacketType
 
 
-class ClientListeners:
+class ClientEvents:
     def __init__(self) -> None:
-        self.initialized = EventEmitter[[]]()
         self.started = EventEmitter[[]]()
         self.stopped = EventEmitter[[]]()
         self.ready = EventEmitter[[]]()
 
 
 class Client(abc.ABC):
     @property
     @abc.abstractmethod
+    def ready(self) -> bool: ...
+
+    @property
+    @abc.abstractmethod
     def app(self) -> App: ...
 
     @property
     @abc.abstractmethod
     def loop(self) -> asyncio.AbstractEventLoop: ...
 
     @property
@@ -48,23 +53,27 @@
 
     @property
     @abc.abstractmethod
     def endpoints(self) -> EndpointExtension: ...
 
     @property
     @abc.abstractmethod
+    def plugins(self) -> PluginExtension: ...
+
+    @property
+    @abc.abstractmethod
     def tables(self) -> TableExtension: ...
 
     @property
     @abc.abstractmethod
     def registry(self) -> RegistryExtension: ...
 
     @property
     @abc.abstractmethod
-    def message(self) -> MessageExtension: ...
+    def signal(self) -> SignalExtension: ...
 
     @property
     @abc.abstractmethod
     def server(self) -> ServerExtension: ...
 
     @property
     @abc.abstractmethod
@@ -92,8 +101,11 @@
     async def stop(self) -> None: ...
 
     @abc.abstractmethod
     async def send[T](self, type: PacketType[T], data: T) -> None: ...
 
     @property
     @abc.abstractmethod
-    def listeners(self) -> ClientListeners: ...
+    def event(self) -> ClientEvents: ...
+
+    @abc.abstractmethod
+    def when_ready(self, coro: Coro[[], None]) -> Unlisten: ...
```

### Comparing `omu-0.2.5/src/omu/client/omuclient.py` & `omu-0.3.0/src/omu/client/omuclient.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from __future__ import annotations
 
 import asyncio
 
 from loguru import logger
 
+from omu.address import Address
 from omu.app import App
+from omu.client.token import JsonTokenProvider, TokenProvider
+from omu.event_emitter import Unlisten
 from omu.extension import ExtensionRegistry
 from omu.extension.asset import (
     ASSET_EXTENSION_TYPE,
     AssetExtension,
 )
 from omu.extension.dashboard import (
     DASHBOARD_EXTENSION_TYPE,
@@ -18,73 +21,83 @@
     ENDPOINT_EXTENSION_TYPE,
     EndpointExtension,
 )
 from omu.extension.i18n import (
     I18N_EXTENSION_TYPE,
     I18nExtension,
 )
-from omu.extension.message import (
-    MESSAGE_EXTENSION_TYPE,
-    MessageExtension,
-)
 from omu.extension.permission import (
     PERMISSION_EXTENSION_TYPE,
     PermissionExtension,
 )
+from omu.extension.plugin import (
+    PLUGIN_EXTENSION_TYPE,
+    PluginExtension,
+)
 from omu.extension.registry import (
     REGISTRY_EXTENSION_TYPE,
     RegistryExtension,
 )
 from omu.extension.server import (
     SERVER_EXTENSION_TYPE,
     ServerExtension,
 )
+from omu.extension.signal import (
+    SIGNAL_EXTENSION_TYPE,
+    SignalExtension,
+)
 from omu.extension.table import (
     TABLE_EXTENSION_TYPE,
     TableExtension,
 )
-from omu.network import Address, Network
+from omu.helper import Coro
+from omu.network import Network
 from omu.network.packet import Packet, PacketType
 from omu.network.websocket_connection import WebsocketsConnection
 
-from .client import Client, ClientListeners
+from .client import Client, ClientEvents
 
 
 class OmuClient(Client):
     def __init__(
         self,
         app: App,
         address: Address,
+        token: TokenProvider | None = None,
         connection: WebsocketsConnection | None = None,
         extension_registry: ExtensionRegistry | None = None,
         loop: asyncio.AbstractEventLoop | None = None,
     ):
         self._loop = loop or asyncio.get_event_loop()
+        self._ready = False
         self._running = False
-        self._listeners = ClientListeners()
+        self._event = ClientEvents()
         self._app = app
         self._network = Network(
             self,
             address,
+            token or JsonTokenProvider(),
             connection or WebsocketsConnection(self, address),
         )
-        self._network.listeners.connected += self._listeners.ready.emit
         self._extensions = extension_registry or ExtensionRegistry(self)
 
         self._endpoints = self.extensions.register(ENDPOINT_EXTENSION_TYPE)
+        self._plugins = self.extensions.register(PLUGIN_EXTENSION_TYPE)
         self._tables = self.extensions.register(TABLE_EXTENSION_TYPE)
         self._registry = self.extensions.register(REGISTRY_EXTENSION_TYPE)
-        self._message = self.extensions.register(MESSAGE_EXTENSION_TYPE)
-        self._assets = self.extensions.register(ASSET_EXTENSION_TYPE)
-        self._server = self.extensions.register(SERVER_EXTENSION_TYPE)
+        self._signal = self.extensions.register(SIGNAL_EXTENSION_TYPE)
         self._permissions = self.extensions.register(PERMISSION_EXTENSION_TYPE)
+        self._server = self.extensions.register(SERVER_EXTENSION_TYPE)
+        self._assets = self.extensions.register(ASSET_EXTENSION_TYPE)
         self._dashboard = self.extensions.register(DASHBOARD_EXTENSION_TYPE)
         self._i18n = self.extensions.register(I18N_EXTENSION_TYPE)
 
-        self._loop.create_task(self._listeners.initialized.emit())
+    @property
+    def ready(self) -> bool:
+        return self._ready
 
     @property
     def app(self) -> App:
         return self._app
 
     @property
     def loop(self) -> asyncio.AbstractEventLoop:
@@ -99,24 +112,28 @@
         return self._extensions
 
     @property
     def endpoints(self) -> EndpointExtension:
         return self._endpoints
 
     @property
+    def plugins(self) -> PluginExtension:
+        return self._plugins
+
+    @property
     def tables(self) -> TableExtension:
         return self._tables
 
     @property
     def registry(self) -> RegistryExtension:
         return self._registry
 
     @property
-    def message(self) -> MessageExtension:
-        return self._message
+    def signal(self) -> SignalExtension:
+        return self._signal
 
     @property
     def assets(self) -> AssetExtension:
         return self._assets
 
     @property
     def server(self) -> ServerExtension:
@@ -137,39 +154,44 @@
     @property
     def running(self) -> bool:
         return self._running
 
     async def send[T](self, type: PacketType[T], data: T) -> None:
         await self._network.send(Packet(type, data))
 
-    def run(self, *, token: str | None = None, reconnect: bool = True) -> None:
+    def run(self, *, reconnect: bool = True) -> None:
         try:
             self.loop.set_exception_handler(self.handle_exception)
-            self.loop.create_task(self.start(token=token, reconnect=reconnect))
+            self.loop.create_task(self.start(reconnect=reconnect))
             self.loop.run_forever()
         finally:
             self.loop.close()
             asyncio.run(self.stop())
 
     def handle_exception(self, loop: asyncio.AbstractEventLoop, context: dict) -> None:
         logger.error(context["message"])
         exception = context.get("exception")
         if exception:
             raise exception
 
-    async def start(self, *, token: str | None = None, reconnect: bool = True) -> None:
+    async def start(self, *, reconnect: bool = True) -> None:
         if self._running:
             raise RuntimeError("Already running")
         self._running = True
-        self.loop.create_task(self._network.connect(token=token, reconnect=reconnect))
-        await self._listeners.started()
+        self.loop.create_task(self._network.connect(reconnect=reconnect))
+        await self._event.started()
 
     async def stop(self) -> None:
         if not self._running:
             raise RuntimeError("Not running")
         self._running = False
         await self._network.disconnect()
-        await self._listeners.stopped()
+        await self._event.stopped()
 
     @property
-    def listeners(self) -> ClientListeners:
-        return self._listeners
+    def event(self) -> ClientEvents:
+        return self._event
+
+    def when_ready(self, coro: Coro[[], None]) -> Unlisten:
+        if self._ready:
+            self.loop.create_task(coro())
+        return self.event.ready.listen(coro)
```

### Comparing `omu-0.2.5/src/omu/extension/extension.py` & `omu-0.3.0/src/omu/extension/extension.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 from __future__ import annotations
 
 import abc
-from typing import TYPE_CHECKING, Callable, List
+from collections.abc import Callable
 
+from omu.client import Client
 from omu.identifier import Identifier
 
-if TYPE_CHECKING:
-    from omu.client import Client
-
 
 class Extension(abc.ABC):
     pass
 
 
 class ExtensionType[T: Extension](Identifier):
     name: str
     create: Callable[[Client], T]
-    dependencies: Callable[[], List[ExtensionType]]
+    dependencies: Callable[[], list[ExtensionType]]
 
     def __init__(
         self,
         name: str,
         create: Callable[[Client], T],
-        dependencies: Callable[[], List[ExtensionType]],
+        dependencies: Callable[[], list[ExtensionType]],
     ) -> None:
         super().__init__("ext", name)
         self.name = name
         self.create = create
         self.dependencies = dependencies
 
     def key(self) -> str:
```

### Comparing `omu-0.2.5/src/omu/extension/extension_registry.py` & `omu-0.3.0/src/omu/extension/extension_registry.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Dict
-
-if TYPE_CHECKING:
-    from omu.client import Client
-    from omu.extension import Extension, ExtensionType
+from omu.client import Client
+from omu.extension import Extension, ExtensionType
 
 
 class ExtensionRegistry:
     def __init__(self, client: Client) -> None:
         self._client = client
-        self._extensions: Dict[str, Extension] = {}
+        self._extensions: dict[str, Extension] = {}
 
     def register[T: Extension](self, type: ExtensionType[T]) -> T:
         if self.has(type):
             raise ValueError(f"Extension type {type} already registered")
         for dependency in type.dependencies():
             if not self.has(dependency):
                 raise ValueError(
```

### Comparing `omu-0.2.5/src/omu/extension/asset/asset_extension.py` & `omu-0.3.0/src/omu/extension/asset/asset_extension.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from dataclasses import dataclass
-from typing import List
 
+from omu.bytebuffer import ByteReader, ByteWriter
 from omu.client import Client
 from omu.extension import Extension, ExtensionType
 from omu.extension.endpoint import EndpointType
 from omu.identifier import Identifier
-from omu.network.bytebuffer import ByteReader, ByteWriter
 from omu.serializer import Serializer
 
 ASSET_EXTENSION_TYPE = ExtensionType(
     "asset",
     lambda client: AssetExtension(client),
     lambda: [],
 )
@@ -35,78 +34,86 @@
             identifier = Identifier.from_key(reader.read_string())
             value = reader.read_byte_array()
         return File(identifier, value)
 
 
 class FileArraySerializer:
     @classmethod
-    def serialize(cls, item: List[File]) -> bytes:
+    def serialize(cls, item: list[File]) -> bytes:
         writer = ByteWriter()
         writer.write_int(len(item))
         for file in item:
             writer.write_string(file.identifier.key())
             writer.write_byte_array(file.buffer)
         return writer.finish()
 
     @classmethod
-    def deserialize(cls, item: bytes) -> List[File]:
+    def deserialize(cls, item: bytes) -> list[File]:
         with ByteReader(item) as reader:
             count = reader.read_int()
-            files: List[File] = []
+            files: list[File] = []
             for _ in range(count):
                 identifier = Identifier.from_key(reader.read_string())
                 value = reader.read_byte_array()
                 files.append(File(identifier, value))
         return files
 
 
+ASSET_UPLOAD_PERMISSION_ID = ASSET_EXTENSION_TYPE / "upload"
 ASSET_UPLOAD_ENDPOINT = EndpointType[File, Identifier].create_serialized(
     ASSET_EXTENSION_TYPE,
     "upload",
     request_serializer=FileSerializer,
     response_serializer=Serializer.model(Identifier).to_json(),
+    permission_id=ASSET_UPLOAD_PERMISSION_ID,
 )
+ASSET_UPLOAD_MANY_PERMISSION_ID = ASSET_EXTENSION_TYPE / "upload" / "many"
 ASSET_UPLOAD_MANY_ENDPOINT = EndpointType[
-    List[File], List[Identifier]
+    list[File], list[Identifier]
 ].create_serialized(
     ASSET_EXTENSION_TYPE,
     "upload_many",
     request_serializer=FileArraySerializer,
     response_serializer=Serializer.model(Identifier).to_array().to_json(),
+    permission_id=ASSET_UPLOAD_MANY_PERMISSION_ID,
 )
+ASSET_DOWNLOAD_PERMISSION_ID = ASSET_EXTENSION_TYPE / "download"
 ASSET_DOWNLOAD_ENDPOINT = EndpointType[Identifier, File].create_serialized(
     ASSET_EXTENSION_TYPE,
     "download",
     request_serializer=Serializer.model(Identifier).to_json(),
     response_serializer=FileSerializer,
+    permission_id=ASSET_DOWNLOAD_PERMISSION_ID,
 )
+ASSET_DOWNLOAD_MANY_PERMISSION_ID = ASSET_EXTENSION_TYPE / "download" / "many"
 ASSET_DOWNLOAD_MANY_ENDPOINT = EndpointType[
-    List[Identifier], List[File]
+    list[Identifier], list[File]
 ].create_serialized(
     ASSET_EXTENSION_TYPE,
     "download_many",
     request_serializer=Serializer.model(Identifier).to_array().to_json(),
     response_serializer=FileArraySerializer,
+    permission_id=ASSET_DOWNLOAD_MANY_PERMISSION_ID,
 )
 
 
 class AssetExtension(Extension):
     def __init__(self, client: Client) -> None:
         self.client = client
 
     async def upload(self, file: File) -> Identifier:
         return await self.client.endpoints.call(ASSET_UPLOAD_ENDPOINT, file)
 
-    async def upload_many(self, files: List[File]) -> List[Identifier]:
+    async def upload_many(self, files: list[File]) -> list[Identifier]:
         return await self.client.endpoints.call(ASSET_UPLOAD_MANY_ENDPOINT, files)
 
     async def download(self, identifier: Identifier) -> File:
         return await self.client.endpoints.call(ASSET_DOWNLOAD_ENDPOINT, identifier)
 
-    async def download_many(self, identifiers: List[Identifier]) -> List[File]:
+    async def download_many(self, identifiers: list[Identifier]) -> list[File]:
         return await self.client.endpoints.call(
             ASSET_DOWNLOAD_MANY_ENDPOINT, identifiers
         )
 
     def url(self, identifier: Identifier) -> str:
         address = self.client.network.address
         protocol = "https" if address.secure else "http"
```

### Comparing `omu-0.2.5/src/omu/extension/dashboard/dashboard.py` & `omu-0.3.0/src/omu/extension/permission/permission.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,52 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import List, TypedDict
+from typing import Literal, TypedDict
 
-from omu.app import App, AppJson
-from omu.extension.permission.permission import PermissionType, PermissionTypeJson
+from omu.identifier import Identifier
+from omu.localization import LocalizedText
 from omu.model import Model
 
+type PermissionLevel = Literal["low", "medium", "high"]
 
-class PermissionRequestJson(TypedDict):
-    request_id: int
-    app: AppJson
-    permissions: List[PermissionTypeJson]
+
+class PermissionMetadata(TypedDict):
+    name: LocalizedText
+    note: LocalizedText
+    level: PermissionLevel
+
+
+class PermissionTypeJson(TypedDict):
+    id: str
+    metadata: PermissionMetadata
 
 
 @dataclass(frozen=True)
-class PermissionRequest(Model[PermissionRequestJson]):
-    request_id: int
-    app: App
-    permissions: List[PermissionType]
+class PermissionType(Model[PermissionTypeJson]):
+    id: Identifier
+    metadata: PermissionMetadata
 
     @classmethod
-    def from_json(cls, json: PermissionRequestJson) -> PermissionRequest:
-        return cls(
-            request_id=json["request_id"],
-            app=App.from_json(json["app"]),
-            permissions=[PermissionType.from_json(p) for p in json["permissions"]],
+    def create(
+        cls,
+        identifier: Identifier,
+        name: str,
+        metadata: PermissionMetadata,
+    ) -> PermissionType:
+        return PermissionType(
+            id=identifier / name,
+            metadata=metadata,
         )
 
-    def to_json(self) -> PermissionRequestJson:
+    def to_json(self) -> PermissionTypeJson:
         return {
-            "request_id": self.request_id,
-            "app": self.app.to_json(),
-            "permissions": [p.to_json() for p in self.permissions],
+            "id": self.id.key(),
+            "metadata": self.metadata,
         }
 
-
-class DashboardOpenAppResponse(TypedDict):
-    success: bool
-    already_open: bool
-    dashboard_not_connected: bool
+    @classmethod
+    def from_json(cls, json: PermissionTypeJson) -> PermissionType:
+        return PermissionType(
+            id=Identifier.from_key(json["id"]),
+            metadata=json["metadata"],
+        )
```

### Comparing `omu-0.2.5/src/omu/extension/i18n/i18n_extension.py` & `omu-0.3.0/src/omu/extension/i18n/i18n_extension.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,35 @@
-from typing import List
-
 from omu.client import Client
 from omu.extension import Extension, ExtensionType
 from omu.extension.registry import RegistryType
+from omu.extension.registry.packets import RegistryPermissions
 from omu.localization import Locale, LocalizedText
 
 I18N_EXTENSION_TYPE = ExtensionType(
     "i18n", lambda client: I18nExtension(client), lambda: []
 )
-
-LOCALES_REGISTRY = RegistryType[List[Locale]].create_json(
-    I18N_EXTENSION_TYPE, name="locales", default_value=[]
+I18N_SET_LOCALES_PERMISSION_ID = I18N_EXTENSION_TYPE / "locales" / "set"
+I18N_GET_LOCALES_PERMISSION_ID = I18N_EXTENSION_TYPE / "locales" / "get"
+I18N_LOCALES_REGISTRY_TYPE = RegistryType[list[Locale]].create_json(
+    I18N_EXTENSION_TYPE,
+    name="locales",
+    default_value=[],
+    permissions=RegistryPermissions(
+        read=I18N_GET_LOCALES_PERMISSION_ID,
+        write=I18N_SET_LOCALES_PERMISSION_ID,
+    ),
 )
 
 
 class I18nExtension(Extension):
     def __init__(self, client: Client):
         self.client = client
-        self.locales_registry = client.registry.get(LOCALES_REGISTRY)
-        self.locales: List[Locale] = []
-        client.network.listeners.connected += self._handle_connected
-
-    async def _handle_connected(self) -> None:
-        self.locales = await self.locales_registry.get()
+        client.permissions.require(I18N_GET_LOCALES_PERMISSION_ID)
+        self.locales_registry = client.registry.get(I18N_LOCALES_REGISTRY_TYPE)
+        self.locales: list[Locale] = []
 
     def translate(self, localized_text: LocalizedText) -> str:
         if not self.locales:
             raise RuntimeError("Locales not loaded")
         if isinstance(localized_text, str):
             return localized_text
         translation = self.select_best_translation(localized_text)
```

### Comparing `omu-0.2.5/src/omu/extension/permission/permission_extension.py` & `omu-0.3.0/src/omu/extension/permission/permission_extension.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,76 +1,93 @@
-from typing import Dict, List
 
 from omu.client import Client
 from omu.extension import Extension, ExtensionType
-from omu.extension.endpoint.endpoint import EndpointType
+from omu.extension.endpoint import EndpointType
 from omu.identifier import Identifier
-from omu.network.packet.packet import PacketType
+from omu.network.packet import PacketType
 from omu.serializer import Serializer
 
 from .permission import PermissionType
 
 PERMISSION_EXTENSION_TYPE = ExtensionType(
     "permission",
     lambda client: PermissionExtension(client),
     lambda: [],
 )
 
 
 class PermissionExtension(Extension):
     def __init__(self, client: Client):
         self.client = client
-        self.permissions: List[PermissionType] = []
-        self.registered_permissions: Dict[Identifier, PermissionType] = {}
-        self.required_permissions: Dict[Identifier, PermissionType] = {}
+        self.permissions: list[PermissionType] = []
+        self.registered_permissions: dict[Identifier, PermissionType] = {}
+        self.required_permission_ids: set[Identifier] = set()
         client.network.register_packet(
             PERMISSION_REGISTER_PACKET,
+            PERMISSION_REQUIRE_PACKET,
             PERMISSION_GRANT_PACKET,
         )
         client.network.add_packet_handler(
             PERMISSION_GRANT_PACKET,
             self.handle_grant,
         )
-        client.network.listeners.connected += self.on_connected
+        client.network.add_task(self.on_network_task)
 
-    def register(self, permission: PermissionType):
-        base_identifier = self.client.app.identifier
-        if not permission.identifier.is_subpart_of(base_identifier):
-            raise ValueError(
-                f"Permission identifier {permission.identifier} is not a subpart of app identifier {base_identifier}"
-            )
-        self.registered_permissions[permission.identifier] = permission
-
-    def require(self, permission: PermissionType):
-        self.required_permissions[permission.identifier] = permission
+    def register(self, *permission_types: PermissionType):
+        base_identifier = self.client.app.id
+        for permission in permission_types:
+            if permission.id in self.registered_permissions:
+                raise ValueError(f"Permission {permission.id} already registered")
+            if not permission.id.is_namepath_equal(base_identifier, path_length=1):
+                msg = f"Permission identifier {permission.id} is not a subpath of {base_identifier}"
+                raise ValueError(msg)
+            self.registered_permissions[permission.id] = permission
+
+    def require(self, permission_id: Identifier):
+        self.required_permission_ids.add(permission_id)
+
+    async def request(self, *permissions_ids: Identifier):
+        self.required_permission_ids = {
+            *self.required_permission_ids,
+            *permissions_ids,
+        }
+        await self.client.endpoints.call(
+            PERMISSION_REQUEST_ENDPOINT, [*self.required_permission_ids]
+        )
 
     def has(self, permission_identifier: Identifier):
         return permission_identifier in self.permissions
 
-    async def on_connected(self):
-        await self.client.send(
-            PERMISSION_REGISTER_PACKET,
-            [*self.registered_permissions.values()],
-        )
-        if len(self.required_permissions) > 0:
-            await self.client.endpoints.call(
-                PERMISSION_REQUEST_ENDPOINT,
-                [*self.required_permissions.keys()],
+    async def on_network_task(self):
+        if len(self.required_permission_ids) > 0:
+            await self.client.send(
+                PERMISSION_REQUIRE_PACKET,
+                [*self.required_permission_ids],
+            )
+        if len(self.registered_permissions) > 0:
+            await self.client.send(
+                PERMISSION_REGISTER_PACKET,
+                [*self.registered_permissions.values()],
             )
 
-    async def handle_grant(self, permissions: List[PermissionType]):
+    async def handle_grant(self, permissions: list[PermissionType]):
         self.permissions = permissions
 
 
-PERMISSION_REGISTER_PACKET = PacketType.create_json(
+PERMISSION_REGISTER_PACKET = PacketType[list[PermissionType]].create_json(
     PERMISSION_EXTENSION_TYPE,
     "register",
     Serializer.model(PermissionType).to_array(),
 )
-PERMISSION_REQUEST_ENDPOINT = EndpointType[List[Identifier], None].create_json(
+PERMISSION_REQUIRE_PACKET = PacketType[list[Identifier]].create_json(
+    PERMISSION_EXTENSION_TYPE,
+    "require",
+    serializer=Serializer.model(Identifier).to_array(),
+)
+PERMISSION_REQUEST_ENDPOINT = EndpointType[list[Identifier], None].create_json(
     PERMISSION_EXTENSION_TYPE,
     "request",
     request_serializer=Serializer.model(Identifier).to_array(),
 )
 PERMISSION_GRANT_PACKET = PacketType.create_json(
     PERMISSION_EXTENSION_TYPE,
     "grant",
```

### Comparing `omu-0.2.5/src/omu/extension/plugin/plugin_extension.py` & `omu-0.3.0/src/omu/extension/plugin/plugin_extension.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,52 +1,42 @@
-from typing import Dict, List, TypedDict
-
 from omu.client import Client
 from omu.extension import Extension, ExtensionType
-from omu.extension.endpoint.endpoint import EndpointType
-from omu.extension.permission.permission import PermissionType
-from omu.network.packet.packet import PacketType
+from omu.extension.table import TableType
+from omu.network.packet import PacketType
+
+from .plugin import PluginPackageInfo
 
 PLUGIN_EXTENSION_TYPE = ExtensionType(
     "plugin",
     lambda client: PluginExtension(client),
     lambda: [],
 )
 
 
 class PluginExtension(Extension):
     def __init__(self, client: Client):
         self.client = client
-        self.plugins: Dict[str, str | None] = {}
+        self.plugins: dict[str, str | None] = {}
 
         self.client.network.register_packet(
             PLUGIN_REQUIRE_PACKET,
         )
-        self.client.network.listeners.connected += self.on_connected
+        self.client.network.add_task(self.on_task)
 
-    async def on_connected(self):
+    async def on_task(self):
         await self.client.send(PLUGIN_REQUIRE_PACKET, self.plugins)
-        await self.client.endpoints.call(PLUGIN_WAIT_ENDPOINT, [*self.plugins.keys()])
 
-    def require(self, plugins: Dict[str, str | None]):
+    def require(self, plugins: dict[str, str | None]):
+        if self.client.running:
+            raise RuntimeError("Cannot require plugins after client has started")
         self.plugins.update(plugins)
-        self.client.permissions.require(PLUGIN_PERMISSION)
 
 
-PLUGIN_PERMISSION = PermissionType.create(
-    PLUGIN_EXTENSION_TYPE,
-    "request",
-)
-PLUGIN_REQUIRE_PACKET = PacketType[Dict[str, str | None]].create_json(
+PLUGIN_REQUIRE_PACKET = PacketType[dict[str, str | None]].create_json(
     PLUGIN_EXTENSION_TYPE,
     "require",
 )
-
-
-class WaitResponse(TypedDict):
-    success: bool
-
-
-PLUGIN_WAIT_ENDPOINT = EndpointType[List[str], WaitResponse].create_json(
+PLUGIN_ALLOWED_PACKAGE_TABLE = TableType.create_model(
     PLUGIN_EXTENSION_TYPE,
-    "wait",
+    "allowed_package",
+    PluginPackageInfo,
 )
```

### Comparing `omu-0.2.5/src/omu/extension/registry/registry_extension.py` & `omu-0.3.0/src/omu/extension/registry/registry_extension.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,148 +1,151 @@
 from __future__ import annotations
 
-from dataclasses import dataclass
-from typing import Callable, List
-
 from omu.client import Client
+from omu.event_emitter import Unlisten
 from omu.extension import Extension, ExtensionType
 from omu.extension.endpoint import EndpointType
 from omu.helper import Coro
 from omu.identifier import Identifier
-from omu.network.bytebuffer import ByteReader, ByteWriter
 from omu.network.packet import PacketType
-from omu.serializer import Serializable, SerializeError, Serializer
+from omu.serializer import SerializeError, Serializer
 
+from .packets import RegistryPacket, RegistryRegisterPacket
 from .registry import Registry, RegistryType
 
 REGISTRY_EXTENSION_TYPE = ExtensionType(
     "registry",
     lambda client: RegistryExtension(client),
     lambda: [],
 )
 
+REGISTRY_PERMISSION_ID = REGISTRY_EXTENSION_TYPE / "permission"
 
-@dataclass(frozen=True)
-class RegistryPacket:
-    identifier: Identifier
-    value: bytes | None
-
-
-class REGISTRY_DATA_SERIALIZER:
-    @classmethod
-    def serialize(cls, item: RegistryPacket) -> bytes:
-        writer = ByteWriter()
-        writer.write_string(item.identifier.key())
-        writer.write_boolean(item.value is not None)
-        if item.value is not None:
-            writer.write_byte_array(item.value)
-        return writer.finish()
-
-    @classmethod
-    def deserialize(cls, item: bytes) -> RegistryPacket:
-        with ByteReader(item) as reader:
-            key = Identifier.from_key(reader.read_string())
-            existing = reader.read_boolean()
-            value = reader.read_byte_array() if existing else None
-        return RegistryPacket(key, value)
-
-
+REGISTRY_REGISTER_PACKET = PacketType[RegistryRegisterPacket].create_serialized(
+    REGISTRY_EXTENSION_TYPE,
+    "register",
+    serializer=RegistryRegisterPacket,
+)
 REGISTRY_UPDATE_PACKET = PacketType[RegistryPacket].create_serialized(
     REGISTRY_EXTENSION_TYPE,
     "update",
-    serializer=REGISTRY_DATA_SERIALIZER,
+    serializer=RegistryPacket,
 )
 REGISTRY_LISTEN_PACKET = PacketType[Identifier].create_json(
     REGISTRY_EXTENSION_TYPE,
     "listen",
     Serializer.model(Identifier),
 )
 REGISTRY_GET_ENDPOINT = EndpointType[Identifier, RegistryPacket].create_serialized(
     REGISTRY_EXTENSION_TYPE,
     "get",
     request_serializer=Serializer.model(Identifier).to_json(),
-    response_serializer=REGISTRY_DATA_SERIALIZER,
+    response_serializer=RegistryPacket,
+    permission_id=REGISTRY_PERMISSION_ID,
 )
 
 
 class RegistryExtension(Extension):
     def __init__(self, client: Client) -> None:
         self.client = client
-        client.network.register_packet(REGISTRY_UPDATE_PACKET)
+        self.registries: dict[Identifier, Registry] = {}
+        client.network.register_packet(
+            REGISTRY_REGISTER_PACKET,
+            REGISTRY_LISTEN_PACKET,
+            REGISTRY_UPDATE_PACKET,
+        )
 
-    def get[T](self, registry_type: RegistryType[T]) -> Registry[T]:
+    def create_registry[T](self, registry_type: RegistryType[T]) -> Registry[T]:
+        self.client.permissions.require(REGISTRY_PERMISSION_ID)
+        if registry_type.id in self.registries:
+            raise ValueError(f"Registry {registry_type.id} already exists")
         return RegistryImpl(
             self.client,
-            registry_type.identifier,
-            registry_type.default_value,
-            registry_type.serializer,
+            registry_type,
         )
 
+    def get[T](self, registry_type: RegistryType[T]) -> Registry[T]:
+        return self.create_registry(registry_type)
+
     def create[T](self, name: str, default_value: T) -> Registry[T]:
-        identifier = self.client.app.identifier / name
-        return RegistryImpl(self.client, identifier, default_value, Serializer.json())
+        identifier = self.client.app.id / name
+        registry_type = RegistryType(
+            identifier,
+            default_value,
+            Serializer.json(),
+        )
+        return self.create_registry(registry_type)
 
 
 class RegistryImpl[T](Registry[T]):
     def __init__(
         self,
         client: Client,
-        identifier: Identifier,
-        default_value: T,
-        serializer: Serializable[T, bytes],
+        registry_type: RegistryType[T],
     ) -> None:
         self.client = client
-        self.identifier = identifier
-        self.default_value = default_value
-        self.serializer = serializer
-        self.listeners: List[Coro[[T], None]] = []
+        self.type = registry_type
+        self._value = registry_type.default_value
+        self.listeners: list[Coro[[T], None]] = []
         self.listening = False
-        client.network.add_packet_handler(REGISTRY_UPDATE_PACKET, self._on_update)
+        client.network.add_packet_handler(REGISTRY_UPDATE_PACKET, self._handle_update)
+        client.network.add_task(self._on_ready_task)
+
+    @property
+    def value(self) -> T:
+        return self._value
 
     async def get(self) -> T:
-        result = await self.client.endpoints.call(
-            REGISTRY_GET_ENDPOINT, self.identifier
-        )
+        result = await self.client.endpoints.call(REGISTRY_GET_ENDPOINT, self.type.id)
         if result.value is None:
-            return self.default_value
+            return self.type.default_value
         try:
-            return self.serializer.deserialize(result.value)
+            return self.type.serializer.deserialize(result.value)
         except SerializeError as e:
             raise SerializeError(
-                f"Failed to deserialize registry value for identifier {self.identifier}"
+                f"Failed to deserialize registry value for identifier {self.type.id}"
             ) from e
 
     async def update(self, handler: Coro[[T], T]) -> None:
         value = await self.get()
         new_value = await handler(value)
         await self.client.send(
             REGISTRY_UPDATE_PACKET,
             RegistryPacket(
-                identifier=self.identifier,
-                value=self.serializer.serialize(new_value),
+                id=self.type.id,
+                value=self.type.serializer.serialize(new_value),
             ),
         )
 
-    def listen(self, handler: Coro[[T], None]) -> Callable[[], None]:
+    def listen(self, handler: Coro[[T], None]) -> Unlisten:
         if not self.listening:
-            self.client.network.add_task(
-                lambda: self.client.send(REGISTRY_LISTEN_PACKET, self.identifier)
-            )
+
+            async def on_ready():
+                await self.client.send(REGISTRY_LISTEN_PACKET, self.type.id)
+
+            self.client.when_ready(on_ready)
             self.listening = True
 
         self.listeners.append(handler)
         return lambda: self.listeners.remove(handler)
 
-    async def _on_update(self, event: RegistryPacket) -> None:
-        if event.identifier != self.identifier:
+    async def _handle_update(self, event: RegistryPacket) -> None:
+        if event.id != self.type.id:
             return
         if event.value is not None:
             try:
-                value = self.serializer.deserialize(event.value)
+                self._value = self.type.serializer.deserialize(event.value)
             except SerializeError as e:
                 raise SerializeError(
-                    f"Failed to deserialize registry value for identifier {self.identifier}"
+                    f"Failed to deserialize registry value for identifier {self.type.id}"
                 ) from e
-        else:
-            value = self.default_value
         for listener in self.listeners:
-            await listener(value)
+            await listener(self.value)
+
+    async def _on_ready_task(self) -> None:
+        if not self.type.id.is_subpath_of(self.client.app.id):
+            return
+        packet = RegistryRegisterPacket(
+            id=self.type.id,
+            permissions=self.type.permissions,
+        )
+        await self.client.send(REGISTRY_REGISTER_PACKET, packet)
```

### Comparing `omu-0.2.5/src/omu/extension/table/table.py` & `omu-0.3.0/src/omu/extension/table/table.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,22 @@
 from __future__ import annotations
 
 import abc
+from collections.abc import AsyncGenerator, Callable, Mapping
 from dataclasses import dataclass
 from typing import (
-    TYPE_CHECKING,
-    AsyncGenerator,
-    Callable,
-    Dict,
-    Mapping,
     NotRequired,
     TypedDict,
 )
 
-from omu.event_emitter import EventEmitter
+from omu.event_emitter import EventEmitter, Unlisten
+from omu.helper import AsyncCallback, Coro
 from omu.identifier import Identifier
 from omu.interface import Keyable
-from omu.serializer import Serializer
-
-if TYPE_CHECKING:
-    from omu.helper import AsyncCallback, Coro
-    from omu.serializer import JsonSerializable, Serializable
+from omu.serializer import JsonSerializable, Serializable, Serializer
 
 
 class TableConfig(TypedDict):
     cache_size: NotRequired[int]
 
 
 class Table[T](abc.ABC):
@@ -34,15 +27,15 @@
     @abc.abstractmethod
     def set_cache_size(self, size: int) -> None: ...
 
     @abc.abstractmethod
     async def get(self, key: str) -> T | None: ...
 
     @abc.abstractmethod
-    async def get_many(self, *keys: str) -> Dict[str, T]: ...
+    async def get_many(self, *keys: str) -> dict[str, T]: ...
 
     @abc.abstractmethod
     async def add(self, *items: T) -> None: ...
 
     @abc.abstractmethod
     async def update(self, *items: T) -> None: ...
 
@@ -57,48 +50,48 @@
         self,
         before: int | None = None,
         after: int | None = None,
         cursor: str | None = None,
     ) -> Mapping[str, T]: ...
 
     @abc.abstractmethod
-    async def fetch_all(self) -> Dict[str, T]: ...
+    async def fetch_all(self) -> dict[str, T]: ...
 
     @abc.abstractmethod
     async def iterate(
         self,
         backward: bool = False,
         cursor: str | None = None,
     ) -> AsyncGenerator[T, None]: ...
 
     @abc.abstractmethod
     async def size(self) -> int: ...
 
     @abc.abstractmethod
     def listen(
         self, listener: AsyncCallback[Mapping[str, T]] | None = None
-    ) -> Callable[[], None]: ...
+    ) -> Unlisten: ...
 
     @abc.abstractmethod
-    def proxy(self, callback: Coro[[T], T | None]) -> Callable[[], None]: ...
+    def proxy(self, callback: Coro[[T], T | None]) -> Unlisten: ...
 
     @abc.abstractmethod
     def set_config(self, config: TableConfig) -> None: ...
 
     @property
     @abc.abstractmethod
-    def listeners(self) -> TableListeners[T]: ...
+    def event(self) -> TableEvents[T]: ...
 
 
-class TableListeners[T]:
+class TableEvents[T]:
     def __init__(
         self,
         table: Table[T],
     ) -> None:
-        self.unlisten: Callable[[], None] | None = None
+        self.unlisten: Unlisten | None = None
 
         def listen():
             self.unlisten = table.listen()
 
         def unlisten():
             if self.unlisten:
                 self.unlisten()
@@ -120,37 +113,51 @@
         )
 
 
 type ModelEntry[T: Keyable, D] = JsonSerializable[T, D]
 
 
 @dataclass(frozen=True)
+class TablePermissions:
+    all: Identifier | None = None
+    read: Identifier | None = None
+    write: Identifier | None = None
+    remove: Identifier | None = None
+    proxy: Identifier | None = None
+
+
+@dataclass(frozen=True)
 class TableType[T]:
-    identifier: Identifier
+    id: Identifier
     serializer: Serializable[T, bytes]
-    key_func: Callable[[T], str]
+    key_function: Callable[[T], str]
+    permissions: TablePermissions | None = None
 
     @classmethod
     def create_model[_T: Keyable, _D](
         cls,
         identifier: Identifier,
         name: str,
         model_type: type[ModelEntry[_T, _D]],
+        permissions: TablePermissions | None = None,
     ) -> TableType[_T]:
         return TableType(
-            identifier=identifier / name,
+            id=identifier / name,
             serializer=Serializer.model(model_type).to_json(),
-            key_func=lambda item: item.key(),
+            key_function=lambda item: item.key(),
+            permissions=permissions,
         )
 
     @classmethod
     def create_serialized[_T: Keyable](
         cls,
         identifier: Identifier,
         name: str,
         serializer: Serializable[_T, bytes],
+        permissions: TablePermissions | None = None,
     ) -> TableType[_T]:
         return TableType(
-            identifier=identifier / name,
+            id=identifier / name,
             serializer=serializer,
-            key_func=lambda item: item.key(),
+            key_function=lambda item: item.key(),
+            permissions=permissions,
         )
```

### Comparing `omu-0.2.5/src/omu/extension/table/table_extension.py` & `omu-0.3.0/src/omu/extension/table/table_extension.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,327 +1,281 @@
-from typing import (
-    AsyncGenerator,
-    Callable,
-    Dict,
-    Iterable,
-    List,
-    Mapping,
-    Sequence,
-    TypedDict,
-)
+from __future__ import annotations
+
+from collections.abc import AsyncGenerator, Iterable, Mapping
 
 from omu.client import Client
+from omu.event_emitter import Unlisten
 from omu.extension import Extension, ExtensionType
-from omu.extension.endpoint import EndpointType
+from omu.extension.endpoint.endpoint import EndpointType
 from omu.helper import AsyncCallback, Coro
 from omu.identifier import Identifier
 from omu.interface import Keyable
-from omu.network.bytebuffer import ByteReader, ByteWriter
-from omu.network.packet import PacketType
-from omu.serializer import JsonSerializable, Serializable, Serializer
+from omu.network.packet.packet import PacketType
+from omu.serializer import JsonSerializable, Serializer
 
+from .packets import (
+    SetConfigPacket,
+    SetPermissionPacket,
+    TableFetchPacket,
+    TableItemsPacket,
+    TableKeysPacket,
+    TablePacket,
+    TableProxyPacket,
+)
 from .table import (
     Table,
     TableConfig,
-    TableListeners,
+    TableEvents,
+    TablePermissions,
     TableType,
 )
 
 type ModelType[T: Keyable, D] = JsonSerializable[T, D]
 
 
 class TableExtension(Extension):
     def __init__(self, client: Client):
         self._client = client
-        self._tables: Dict[Identifier, Table] = {}
+        self._tables: dict[Identifier, Table] = {}
         client.network.register_packet(
-            TABLE_CONFIG_PACKET,
+            TABLE_SET_PERMISSION_PACKET,
+            TABLE_SET_CONFIG_PACKET,
             TABLE_LISTEN_PACKET,
             TABLE_PROXY_LISTEN_PACKET,
             TABLE_PROXY_PACKET,
             TABLE_ITEM_ADD_PACKET,
             TABLE_ITEM_UPDATE_PACKET,
-            TABLE_ITEM_REMOVE_EVENT,
+            TABLE_ITEM_REMOVE_PACKET,
             TABLE_ITEM_CLEAR_PACKET,
         )
 
     def create[T](
         self,
-        identifier: Identifier,
-        serializer: Serializable[T, bytes],
-        key_function: Callable[[T], str],
+        table_type: TableType[T],
     ) -> Table[T]:
-        if self.has(identifier):
-            raise ValueError(f"Table with identifier {identifier} already exists")
+        self._client.permissions.require(TABLE_PERMISSION_ID)
+        if self.has(table_type.id):
+            raise ValueError(f"Table with identifier {table_type.id} already exists")
         table = TableImpl(
             self._client,
-            identifier=identifier,
-            serializer=serializer,
-            key_function=key_function,
+            table_type=table_type,
         )
-        self._tables[identifier] = table
+        self._tables[table_type.id] = table
         return table
 
     def get[T](self, type: TableType[T]) -> Table[T]:
-        if self.has(type.identifier):
-            return self._tables[type.identifier]
-        return self.create(type.identifier, type.serializer, type.key_func)
+        if self.has(type.id):
+            return self._tables[type.id]
+        return self.create(type)
 
     def model[T: Keyable, D](
-        self, identifier: Identifier, name: str, model_type: type[ModelType[T, D]]
+        self, id: Identifier, name: str, model_type: type[ModelType[T, D]]
     ) -> Table[T]:
-        identifier = identifier / name
-        if self.has(identifier):
-            return self._tables[identifier]
-        return self.create(
-            identifier,
-            Serializer.model(model_type).to_json(),
-            lambda item: item.key(),
-        )
+        id = id / name
+        if self.has(id):
+            raise ValueError(f"Table with identifier {id} already exists")
+        table_type = TableType.create_model(id, name, model_type)
+        return self.create(table_type)
 
-    def has(self, identifier: Identifier) -> bool:
-        return identifier in self._tables
+    def has(self, id: Identifier) -> bool:
+        return id in self._tables
 
 
 TABLE_EXTENSION_TYPE = ExtensionType(
     "table", lambda client: TableExtension(client), lambda: []
 )
 
+TABLE_PERMISSION_ID = TABLE_EXTENSION_TYPE / "permission"
 
-class TableEventData(TypedDict):
-    type: str
-
-
-class TableItemsData(TableEventData):
-    items: Mapping[str, bytes]
-
-
-class TableKeysData(TableEventData):
-    keys: Sequence[str]
-
-
-class TableProxyData(TableItemsData):
-    key: int
-
-
-class TableFetchReq(TableEventData):
-    before: int | None
-    after: int | None
-    cursor: str | None
-
-
-class ITEMS_SERIALIZER:
-    @classmethod
-    def serialize(cls, item: TableItemsData) -> bytes:
-        writer = ByteWriter()
-        writer.write_string(item["type"])
-        writer.write_int(len(item["items"]))
-        for key, value in item["items"].items():
-            writer.write_string(key)
-            writer.write_byte_array(value)
-        return writer.finish()
-
-    @classmethod
-    def deserialize(cls, item: bytes) -> TableItemsData:
-        with ByteReader(item) as reader:
-            type = reader.read_string()
-            item_count = reader.read_int()
-            items: Mapping[str, bytes] = {}
-            for _ in range(item_count):
-                key = reader.read_string()
-                value = reader.read_byte_array()
-                items[key] = value
-        return {"type": type, "items": items}
-
-
-class ITEM_PROXY_SERIALIZER:
-    @staticmethod
-    def serialize(item: TableProxyData) -> bytes:
-        writer = ByteWriter()
-        writer.write_string(item["type"])
-        writer.write_int(item["key"])
-        writer.write_int(len(item["items"]))
-        for key, value in item["items"].items():
-            writer.write_string(key)
-            writer.write_byte_array(value)
-        return writer.finish()
-
-    @staticmethod
-    def deserialize(item: bytes) -> TableProxyData:
-        with ByteReader(item) as reader:
-            type = reader.read_string()
-            key = reader.read_int()
-            item_count = reader.read_int()
-            items: Dict[str, bytes] = {}
-            for _ in range(item_count):
-                item_key = reader.read_string()
-                value = reader.read_byte_array()
-                items[item_key] = value
-        return {"type": type, "key": key, "items": items}
-
-
-class SetConfigReq(TypedDict):
-    type: str
-    config: TableConfig
-
-
-TABLE_CONFIG_PACKET = PacketType[SetConfigReq].create_json(
+TABLE_SET_PERMISSION_PACKET = PacketType[SetPermissionPacket].create(
     TABLE_EXTENSION_TYPE,
-    "config",
+    "set_permission",
+    SetPermissionPacket,
 )
-TABLE_LISTEN_PACKET = PacketType[str].create_json(
+TABLE_SET_CONFIG_PACKET = PacketType[SetConfigPacket].create(
+    TABLE_EXTENSION_TYPE,
+    "set_config",
+    SetConfigPacket,
+)
+TABLE_LISTEN_PACKET = PacketType[Identifier].create_json(
     TABLE_EXTENSION_TYPE,
     "listen",
+    serializer=Serializer.model(Identifier),
 )
-TABLE_PROXY_LISTEN_PACKET = PacketType[str].create_json(
-    TABLE_EXTENSION_TYPE, "proxy_listen"
+TABLE_PROXY_LISTEN_PACKET = PacketType[Identifier].create_json(
+    TABLE_EXTENSION_TYPE,
+    "proxy_listen",
+    serializer=Serializer.model(Identifier),
 )
-TABLE_PROXY_PACKET = PacketType[TableProxyData].create_serialized(
+TABLE_PROXY_PACKET = PacketType[TableProxyPacket].create_serialized(
     TABLE_EXTENSION_TYPE,
     "proxy",
-    serializer=ITEM_PROXY_SERIALIZER,
+    TableProxyPacket,
 )
-TABLE_ITEM_ADD_PACKET = PacketType[TableItemsData].create_serialized(
+TABLE_ITEM_ADD_PACKET = PacketType[TableItemsPacket].create(
     TABLE_EXTENSION_TYPE,
     "item_add",
-    ITEMS_SERIALIZER,
+    TableItemsPacket,
 )
-TABLE_ITEM_UPDATE_PACKET = PacketType[TableItemsData].create_serialized(
+TABLE_ITEM_UPDATE_PACKET = PacketType[TableItemsPacket].create(
     TABLE_EXTENSION_TYPE,
     "item_update",
-    ITEMS_SERIALIZER,
+    TableItemsPacket,
 )
-TABLE_ITEM_REMOVE_EVENT = PacketType[TableItemsData].create_serialized(
+TABLE_ITEM_REMOVE_PACKET = PacketType[TableItemsPacket].create(
     TABLE_EXTENSION_TYPE,
     "item_remove",
-    ITEMS_SERIALIZER,
+    TableItemsPacket,
 )
-TABLE_ITEM_GET_ENDPOINT = EndpointType[TableKeysData, TableItemsData].create_serialized(
+TABLE_ITEM_GET_ENDPOINT = EndpointType[
+    TableKeysPacket, TableItemsPacket
+].create_serialized(
     TABLE_EXTENSION_TYPE,
     "item_get",
-    request_serializer=Serializer.json(),
-    response_serializer=ITEMS_SERIALIZER,
+    request_serializer=TableKeysPacket,
+    response_serializer=TableItemsPacket,
+    permission_id=TABLE_PERMISSION_ID,
 )
-TABLE_FETCH_ENDPOINT = EndpointType[TableFetchReq, TableItemsData].create_serialized(
+TABLE_FETCH_ENDPOINT = EndpointType[
+    TableFetchPacket, TableItemsPacket
+].create_serialized(
     TABLE_EXTENSION_TYPE,
     "fetch",
-    request_serializer=Serializer.json(),
-    response_serializer=ITEMS_SERIALIZER,
+    request_serializer=TableFetchPacket,
+    response_serializer=TableItemsPacket,
+    permission_id=TABLE_PERMISSION_ID,
 )
 TABLE_FETCH_ALL_ENDPOINT = EndpointType[
-    TableEventData, TableItemsData
+    TablePacket, TableItemsPacket
 ].create_serialized(
     TABLE_EXTENSION_TYPE,
     "fetch_all",
-    request_serializer=Serializer.json(),
-    response_serializer=ITEMS_SERIALIZER,
+    request_serializer=TablePacket,
+    response_serializer=TableItemsPacket,
+    permission_id=TABLE_PERMISSION_ID,
 )
-TABLE_SIZE_ENDPOINT = EndpointType[TableEventData, int].create_json(
-    TABLE_EXTENSION_TYPE, "size"
+TABLE_SIZE_ENDPOINT = EndpointType[TablePacket, int].create_serialized(
+    TABLE_EXTENSION_TYPE,
+    "size",
+    request_serializer=TablePacket,
+    response_serializer=Serializer.json(),
+    permission_id=TABLE_PERMISSION_ID,
 )
-TABLE_ITEM_CLEAR_PACKET = PacketType[TableEventData].create_json(
+TABLE_ITEM_CLEAR_PACKET = PacketType[TablePacket].create(
     TABLE_EXTENSION_TYPE,
     "clear",
+    TablePacket,
 )
 
 
 class TableImpl[T](Table[T]):
     def __init__(
         self,
         client: Client,
-        identifier: Identifier,
-        serializer: Serializable[T, bytes],
-        key_function: Callable[[T], str],
+        table_type: TableType,
     ):
         self._client = client
-        self._identifier = identifier
-        self._serializer = serializer
-        self._key_function = key_function
-        self._cache: Dict[str, T] = {}
-        self._listeners = TableListeners[T](self)
-        self._proxies: List[Coro[[T], T | None]] = []
+        self._id = table_type.id
+        self._serializer = table_type.serializer
+        self._key_function = table_type.key_function
+        self._cache: dict[str, T] = {}
+        self._event = TableEvents[T](self)
+        self._proxies: list[Coro[[T], T | None]] = []
         self._chunk_size = 100
         self._cache_size: int | None = None
         self._listening = False
         self._config: TableConfig | None = None
-        self.key = identifier.key()
+        self._permissions: TablePermissions | None = table_type.permissions
 
-        client.network.add_packet_handler(TABLE_PROXY_PACKET, self._on_proxy)
-        client.network.add_packet_handler(TABLE_ITEM_ADD_PACKET, self._on_item_add)
         client.network.add_packet_handler(
-            TABLE_ITEM_UPDATE_PACKET, self._on_item_update
+            TABLE_PROXY_PACKET,
+            self._on_proxy,
+        )
+        client.network.add_packet_handler(
+            TABLE_ITEM_ADD_PACKET,
+            self._on_item_add,
+        )
+        client.network.add_packet_handler(
+            TABLE_ITEM_UPDATE_PACKET,
+            self._on_item_update,
+        )
+        client.network.add_packet_handler(
+            TABLE_ITEM_REMOVE_PACKET,
+            self._on_item_remove,
         )
-        client.network.add_packet_handler(TABLE_ITEM_REMOVE_EVENT, self._on_item_remove)
-        client.network.add_packet_handler(TABLE_ITEM_CLEAR_PACKET, self._on_item_clear)
-        client.network.add_task(self.on_connected)
+        client.network.add_packet_handler(
+            TABLE_ITEM_CLEAR_PACKET,
+            self._on_item_clear,
+        )
+        client.network.add_task(self._on_ready)
 
     @property
     def cache(self) -> Mapping[str, T]:
         return self._cache
 
     async def get(self, key: str) -> T | None:
         if key in self._cache:
             return self._cache[key]
         res = await self._client.endpoints.call(
-            TABLE_ITEM_GET_ENDPOINT, TableKeysData(type=self.key, keys=[key])
+            TABLE_ITEM_GET_ENDPOINT, TableKeysPacket(id=self._id, keys=[key])
         )
-        items = self._parse_items(res["items"])
+        items = self._parse_items(res.items)
         self._cache.update(items)
         if key in items:
             return items[key]
         return None
 
-    async def get_many(self, *keys: str) -> Dict[str, T]:
+    async def get_many(self, *keys: str) -> dict[str, T]:
         res = await self._client.endpoints.call(
-            TABLE_ITEM_GET_ENDPOINT, TableKeysData(type=self.key, keys=keys)
+            TABLE_ITEM_GET_ENDPOINT, TableKeysPacket(id=self._id, keys=keys)
         )
-        items = self._parse_items(res["items"])
+        items = self._parse_items(res.items)
         self._cache.update(items)
         return items
 
     async def add(self, *items: T) -> None:
         data = self._serialize_items(items)
         await self._client.send(
-            TABLE_ITEM_ADD_PACKET, TableItemsData(type=self.key, items=data)
+            TABLE_ITEM_ADD_PACKET, TableItemsPacket(id=self._id, items=data)
         )
 
     async def update(self, *items: T) -> None:
         data = self._serialize_items(items)
         await self._client.send(
-            TABLE_ITEM_UPDATE_PACKET, TableItemsData(type=self.key, items=data)
+            TABLE_ITEM_UPDATE_PACKET, TableItemsPacket(id=self._id, items=data)
         )
 
     async def remove(self, *items: T) -> None:
         data = self._serialize_items(items)
         await self._client.send(
-            TABLE_ITEM_REMOVE_EVENT, TableItemsData(type=self.key, items=data)
+            TABLE_ITEM_REMOVE_PACKET, TableItemsPacket(id=self._id, items=data)
         )
 
     async def clear(self) -> None:
-        await self._client.send(TABLE_ITEM_CLEAR_PACKET, TableEventData(type=self.key))
+        await self._client.send(TABLE_ITEM_CLEAR_PACKET, TablePacket(id=self._id))
 
     async def fetch_items(
         self,
         before: int | None = None,
         after: int | None = None,
         cursor: str | None = None,
-    ) -> Dict[str, T]:
+    ) -> dict[str, T]:
         items_response = await self._client.endpoints.call(
             TABLE_FETCH_ENDPOINT,
-            TableFetchReq(type=self.key, before=before, after=after, cursor=cursor),
+            TableFetchPacket(id=self._id, before=before, after=after, cursor=cursor),
         )
-        items = self._parse_items(items_response["items"])
+        items = self._parse_items(items_response.items)
         await self.update_cache(items)
         return items
 
-    async def fetch_all(self) -> Dict[str, T]:
+    async def fetch_all(self) -> dict[str, T]:
         items_response = await self._client.endpoints.call(
-            TABLE_FETCH_ALL_ENDPOINT, TableEventData(type=self.key)
+            TABLE_FETCH_ALL_ENDPOINT, TablePacket(id=self._id)
         )
-        items = self._parse_items(items_response["items"])
+        items = self._parse_items(items_response.items)
         await self.update_cache(items)
         return items
 
     async def iterate(
         self,
         backward: bool = False,
         cursor: str | None = None,
@@ -342,108 +296,133 @@
             )
             for item in items.values():
                 yield item
             items.pop(cursor, None)
 
     async def size(self) -> int:
         res = await self._client.endpoints.call(
-            TABLE_SIZE_ENDPOINT, TableEventData(type=self.key)
+            TABLE_SIZE_ENDPOINT, TablePacket(id=self._id)
         )
         return res
 
     def listen(
         self, listener: AsyncCallback[Mapping[str, T]] | None = None
-    ) -> Callable[[], None]:
-        self._listening = True
+    ) -> Unlisten:
+        if not self._listening:
+
+            async def on_ready():
+                await self._client.send(TABLE_LISTEN_PACKET, self._id)
+
+            self._client.when_ready(on_ready)
+            self._listening = True
+
         if listener is not None:
-            self._listeners.cache_update += listener
-            return lambda: self._listeners.cache_update.unsubscribe(listener)
+            return self._event.cache_update.listen(listener)
         return lambda: None
 
-    def proxy(self, callback: Coro[[T], T | None]) -> Callable[[], None]:
+    def proxy(self, callback: Coro[[T], T | None]) -> Unlisten:
+        if not self._proxies:
+
+            async def listen():
+                await self._client.send(TABLE_PROXY_LISTEN_PACKET, self._id)
+
+            self._client.when_ready(listen)
         self._proxies.append(callback)
         return lambda: self._proxies.remove(callback)
 
     def set_config(self, config: TableConfig) -> None:
+        if self._client.running:
+            raise ValueError("Cannot set config after client has started")
         self._config = config
 
-    async def on_connected(self) -> None:
+    async def _on_ready(self) -> None:
         if self._config is not None:
             await self._client.send(
-                TABLE_CONFIG_PACKET,
-                SetConfigReq(type=self.key, config=self._config),
+                TABLE_SET_CONFIG_PACKET,
+                SetConfigPacket(id=self._id, config=self._config),
             )
-        if self._listening:
-            await self._client.send(TABLE_LISTEN_PACKET, self.key)
-        if len(self._proxies) > 0:
-            await self._client.send(TABLE_PROXY_LISTEN_PACKET, self.key)
+        if self._permissions is None:
+            return
+        if not self._id.is_subpath_of(self._client.app.id):
+            return
+        await self._client.send(
+            TABLE_SET_PERMISSION_PACKET,
+            SetPermissionPacket(
+                id=self._id,
+                all=self._permissions.all,
+                read=self._permissions.read,
+                write=self._permissions.write,
+                remove=self._permissions.remove,
+                proxy=self._permissions.proxy,
+            ),
+        )
 
-    async def _on_proxy(self, event: TableProxyData) -> None:
-        if event["type"] != self.key:
+    async def _on_proxy(self, packet: TableProxyPacket) -> None:
+        if packet.id != self._id:
             return
-        items = self._parse_items(event["items"])
+        items = self._parse_items(packet.items)
         for proxy in self._proxies:
             for key, item in list(items.items()):
                 updated_item = await proxy(item)
                 if updated_item is None:
                     del items[key]
                 else:
                     items[key] = updated_item
         serialized_items = self._serialize_items(items.values())
         await self._client.send(
             TABLE_PROXY_PACKET,
-            TableProxyData(
-                type=self.key,
-                key=event["key"],
+            TableProxyPacket(
+                id=self._id,
+                key=packet.key,
                 items=serialized_items,
             ),
         )
 
-    async def _on_item_add(self, event: TableItemsData) -> None:
-        if event["type"] != self.key:
+    async def _on_item_add(self, packet: TableItemsPacket) -> None:
+        if packet.id != self._id:
             return
-        items = self._parse_items(event["items"])
-        await self._listeners.add(items)
+        items = self._parse_items(packet.items)
+        await self._event.add(items)
         await self.update_cache(items)
 
-    async def _on_item_update(self, event: TableItemsData) -> None:
-        if event["type"] != self.key:
+    async def _on_item_update(self, packet: TableItemsPacket) -> None:
+        if packet.id != self._id:
             return
-        items = self._parse_items(event["items"])
-        await self._listeners.update(items)
+        items = self._parse_items(packet.items)
+        await self._event.update(items)
         await self.update_cache(items)
 
-    async def _on_item_remove(self, event: TableItemsData) -> None:
-        if event["type"] != self.key:
+    async def _on_item_remove(self, packet: TableItemsPacket) -> None:
+        if packet.id != self._id:
             return
-        items = self._parse_items(event["items"])
-        await self._listeners.remove(items)
+        items = self._parse_items(packet.items)
+        await self._event.remove(items)
         for key in items.keys():
             if key not in self._cache:
                 continue
             del self._cache[key]
-        await self._listeners.cache_update(self._cache)
+        await self._event.cache_update(self._cache)
 
-    async def _on_item_clear(self, event: TableEventData) -> None:
-        if event["type"] != self.key:
+    async def _on_item_clear(self, packet: TablePacket) -> None:
+        if packet.id != self._id:
             return
-        await self._listeners.clear()
+        await self._event.clear()
         self._cache.clear()
-        await self._listeners.cache_update(self._cache)
+        await self._event.cache_update(self._cache)
 
     async def update_cache(self, items: Mapping[str, T]) -> None:
         if self._cache_size is None:
             self._cache = {**items}
         else:
             merged_cache = {**self._cache, **items}
             cache_array = tuple(merged_cache.items())
             self._cache = dict(cache_array[: self._cache_size])
-        await self._listeners.cache_update(self._cache)
+        await self._event.cache_update(self._cache)
 
-    def _parse_items(self, items: Mapping[str, bytes]) -> Dict[str, T]:
+    def _parse_items(self, items: Mapping[str, bytes]) -> dict[str, T]:
         parsed_items: Mapping[str, T] = {}
         for key, item_bytes in items.items():
             item = self._serializer.deserialize(item_bytes)
             if item is None:
                 raise ValueError(f"Failed to deserialize item with key: {key}")
             parsed_items[key] = item
         return parsed_items
@@ -455,9 +434,9 @@
             serialized_items[key] = self._serializer.serialize(item)
         return serialized_items
 
     def set_cache_size(self, size: int | None) -> None:
         self._cache_size = size
 
     @property
-    def listeners(self) -> TableListeners[T]:
-        return self._listeners
+    def event(self) -> TableEvents[T]:
+        return self._event
```

### Comparing `omu-0.2.5/src/omu/localization/locale.py` & `omu-0.3.0/src/omu/localization/locale.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Literal, Mapping
+from collections.abc import Mapping
+from typing import Literal
 
 # Locale Identifiers - https://gist.github.com/ndbroadbent/588fefab8e0f1b459fcec8181b41b39c
 type Locale = Literal[
     "af",
     "af-NA",
     "af-ZA",
     "agq",
```

### Comparing `omu-0.2.5/src/omu/network/connection.py` & `omu-0.3.0/src/omu/network/connection.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.5/src/omu/network/packet_mapper.py` & `omu-0.3.0/src/omu/network/packet_mapper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,36 @@
-from typing import Dict
-
+from omu.errors import InvalidPacket
 from omu.identifier import Identifier
 from omu.serializer import Serializable
 
 from .packet import Packet, PacketData, PacketType
 
 
 class PacketMapper(Serializable[Packet, PacketData]):
     def __init__(self) -> None:
-        self._map: Dict[Identifier, PacketType] = {}
+        self._map: dict[Identifier, PacketType] = {}
 
     def register(self, *packet_types: PacketType) -> None:
         for packet_type in packet_types:
-            if self._map.get(packet_type.identifier):
-                raise ValueError(
-                    f"Packet id {packet_type.identifier} already registered"
-                )
-            self._map[packet_type.identifier] = packet_type
+            if self._map.get(packet_type.id):
+                raise ValueError(f"Packet id {packet_type.id} already registered")
+            self._map[packet_type.id] = packet_type
 
     def serialize(self, item: Packet) -> PacketData:
         return PacketData(
-            type=item.type.identifier.key(),
+            type=item.type.id.key(),
             data=item.type.serializer.serialize(item.data),
         )
 
     def deserialize(self, item: PacketData) -> Packet:
-        identifier = Identifier.from_key(item.type)
-        packet_type = self._map.get(identifier)
+        id = Identifier.from_key(item.type)
+        packet_type = self._map.get(id)
         if not packet_type:
-            raise ValueError(f"Packet type {identifier} not registered")
+            raise InvalidPacket(id, f"Packet type {id} not registered")
+        try:
+            data = packet_type.serializer.deserialize(item.data)
+        except Exception as e:
+            raise InvalidPacket(id, "Failed to deserialize packet data") from e
         return Packet(
             type=packet_type,
-            data=packet_type.serializer.deserialize(item.data),
+            data=data,
         )
```

### Comparing `omu-0.2.5/src/omu/network/websocket_connection.py` & `omu-0.3.0/src/omu/network/websocket_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 import aiohttp
 from aiohttp import web
 
+from omu.address import Address
+from omu.bytebuffer import ByteReader, ByteWriter
 from omu.client import Client
 from omu.serializer import Serializable
 
-from .address import Address
-from .bytebuffer import ByteReader, ByteWriter
 from .connection import Connection
 from .packet import Packet, PacketData
 
 
 class WebsocketsConnection(Connection):
     def __init__(self, client: Client, address: Address):
         self._client = client
```

### Comparing `omu-0.2.5/src/omu/network/packet/packet.py` & `omu-0.3.0/src/omu/network/packet/packet.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,54 +1,67 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, Any
+from typing import Any, Protocol
 
 from omu.identifier import Identifier
-from omu.serializer import Serializer
-
-if TYPE_CHECKING:
-    from omu.serializer import Serializable
+from omu.serializer import Serializable, Serializer
 
 
 @dataclass(frozen=True)
 class PacketData:
     type: str
     data: bytes
 
 
 @dataclass(frozen=True)
 class Packet[T]:
     type: PacketType[T]
     data: T
 
 
+class PacketClass[T](Protocol):
+    def serialize(self, item: T) -> bytes: ...
+
+    def deserialize(self, item: bytes) -> T: ...
+
+
 @dataclass(frozen=True)
 class PacketType[T]:
-    identifier: Identifier
+    id: Identifier
     serializer: Serializable[T, bytes]
 
     @classmethod
     def create_json[_T](
         cls,
         identifier: Identifier,
         name: str,
         serializer: Serializable[_T, Any] | None = None,
     ) -> PacketType[_T]:
         return PacketType(
-            identifier=identifier / name,
-            serializer=Serializer.of(serializer or Serializer.noop()).pipe(
-                Serializer.json()
-            ),
+            id=identifier / name,
+            serializer=Serializer.of(serializer or Serializer.noop()).to_json(),
         )
 
     @classmethod
     def create_serialized[_T](
         cls,
         identifier: Identifier,
         name: str,
         serializer: Serializable[_T, bytes],
     ) -> PacketType[_T]:
         return PacketType(
-            identifier=identifier / name,
+            id=identifier / name,
             serializer=serializer,
         )
+
+    @classmethod
+    def create[_T](
+        cls,
+        identifier: Identifier,
+        name: str,
+        type_class: PacketClass[_T],
+    ) -> PacketType[_T]:
+        return PacketType(
+            id=identifier / name,
+            serializer=type_class,
+        )
```

### Comparing `omu-0.2.5/src/omu/network/packet/packet_types.py` & `omu-0.3.0/src/omu/network/packet/packet_types.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,67 +1,100 @@
 from __future__ import annotations
 
-from typing import Mapping
+from enum import Enum
+from typing import TypedDict
 
-from omu.app import App
+from omu.app import App, AppJson
 from omu.identifier import Identifier
 from omu.model import Model
 from omu.serializer import Serializer
 
 from .packet import PacketType
 
 
-class ConnectPacket(Model):
-    def __init__(self, app: App, token: str | None = None):
+class ConnectPacketData(TypedDict):
+    app: AppJson
+    token: str | None
+
+
+class ConnectPacket(Model[ConnectPacketData]):
+    def __init__(
+        self,
+        app: App,
+        token: str | None = None,
+    ):
         self.app = app
         self.token = token
 
-    def to_json(self) -> Mapping:
+    def to_json(self) -> ConnectPacketData:
         return {
             "app": self.app.to_json(),
             "token": self.token,
         }
 
     @classmethod
-    def from_json(cls, json: Mapping) -> ConnectPacket:
+    def from_json(cls, json: ConnectPacketData) -> ConnectPacket:
         return cls(
             app=App.from_json(json["app"]),
             token=json["token"],
         )
 
 
-class DisconnectPacket(Model):
-    def __init__(self, reason: str):
-        self.reason = reason
+class DisconnectType(str, Enum):
+    INVALID_TOKEN = "invalid_token"
+    INVALID_ORIGIN = "invalid_origin"
+    INVALID_VERSION = "invalid_version"
+    INVALID_PACKET_TYPE = "invalid_packet_type"
+    INVALID_PACKET_DATA = "invalid_packet_data"
+    INVALID_PACKET = "invalid_packet"
+    ANOTHER_CONNECTION = "another_connection"
+    PERMISSION_DENIED = "permission_denied"
+    SHUTDOWN = "shutdown"
+    CLOSE = "close"
+
+
+class DisconnectPacketData(TypedDict):
+    type: str
+    message: str | None
+
+
+class DisconnectPacket(Model[DisconnectPacketData]):
+    def __init__(self, type: DisconnectType, message: str | None = None):
+        self.type: DisconnectType = type
+        self.message = message
 
-    def to_json(self) -> Mapping:
-        return {"reason": self.reason}
+    def to_json(self) -> DisconnectPacketData:
+        return {
+            "type": self.type.value,
+            "message": self.message,
+        }
 
     @classmethod
-    def from_json(cls, json: Mapping) -> DisconnectPacket:
+    def from_json(cls, json: DisconnectPacketData) -> DisconnectPacket:
         return cls(
-            reason=json["reason"],
+            type=DisconnectType(json["type"]),
+            message=json["message"],
         )
 
 
+IDENTIFIER = Identifier("core", "packet")
+
+
 class PACKET_TYPES:
-    IDENTIFIER = Identifier("core", "packet")
     CONNECT = PacketType.create_json(
         IDENTIFIER,
         "connect",
         Serializer.model(ConnectPacket),
     )
     DISCONNECT = PacketType.create_json(
         IDENTIFIER,
         "disconnect",
         Serializer.model(DisconnectPacket),
     )
     TOKEN = PacketType[str].create_json(
         IDENTIFIER,
         "token",
-        Serializer.noop(),
     )
     READY = PacketType[None].create_json(
         IDENTIFIER,
         "ready",
-        Serializer.noop(),
     )
```

