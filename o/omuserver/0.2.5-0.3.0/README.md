# Comparing `tmp/omuserver-0.2.5.tar.gz` & `tmp/omuserver-0.3.0.tar.gz`

## Comparing `omuserver-0.2.5.tar` & `omuserver-0.3.0.tar`

### file list

```diff
@@ -1,52 +1,58 @@
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/__init__.py
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/__main__.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/config.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/directories.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/helper.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/__init__.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/extension.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/asset/__init__.py
--rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/asset/asset_extension.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/dashboard/__init__.py
--rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/dashboard/dashboard_extension.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/endpoint/__init__.py
--rw-r--r--   0        0        0     6982 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/endpoint/endpoint_extension.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/message/__init__.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/message/message_extension.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/permission/__init__.py
--rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/permission/permission_extension.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/plugin/__init__.py
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/plugin/plugin_connection.py
--rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/plugin/plugin_extension.py
--rw-r--r--   0        0        0     8603 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/plugin/plugin_loader.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/plugin/plugin_session_connection.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/registry/__init__.py
--rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/registry/registry.py
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/registry/registry_extension.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/server/__init__.py
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/server/server_extension.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/table/__init__.py
--rw-r--r--   0        0        0     8307 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/table/cached_table.py
--rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/table/serialized_table.py
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/table/server_table.py
--rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/table/session_table_handler.py
--rw-r--r--   0        0        0     6715 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/table/table_extension.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/table/adapters/__init__.py
--rw-r--r--   0        0        0     4865 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/table/adapters/sqlitetable.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/table/adapters/tableadapter.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/network/__init__.py
--rw-r--r--   0        0        0     5536 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/network/network.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/network/packet_dispatcher.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/security/__init__.py
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/security/security.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/server/__init__.py
--rw-r--r--   0        0        0     6742 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/server/omuserver.py
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/server/server.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/session/__init__.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/session/aiohttp_connection.py
--rw-r--r--   0        0        0     3824 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/session/session.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 omuserver-0.2.5/test/helper_test.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omuserver-0.2.5/.gitignore
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 omuserver-0.2.5/README.md
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 omuserver-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 omuserver-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/__init__.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/__main__.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/config.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/directories.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/helper.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/version.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/extension/__init__.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/extension/extension.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/extension/asset/__init__.py
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/extension/asset/asset_extension.py
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/extension/asset/permissions.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/extension/dashboard/__init__.py
+-rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/extension/dashboard/dashboard_extension.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/extension/dashboard/permission.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/extension/endpoint/__init__.py
+-rw-r--r--   0        0        0     8365 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/extension/endpoint/endpoint_extension.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/extension/i18n/__init__.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/extension/i18n/i18n_extension.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/extension/i18n/permissions.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/extension/permission/__init__.py
+-rw-r--r--   0        0        0     6544 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/extension/permission/permission_extension.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/extension/plugin/__init__.py
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/extension/plugin/plugin_connection.py
+-rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/extension/plugin/plugin_extension.py
+-rw-r--r--   0        0        0     9157 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/extension/plugin/plugin_loader.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/extension/plugin/plugin_session_connection.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/extension/registry/__init__.py
+-rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/extension/registry/registry.py
+-rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/extension/registry/registry_extension.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/extension/server/__init__.py
+-rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/extension/server/server_extension.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/extension/signal/__init__.py
+-rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/extension/signal/signal_extension.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/extension/table/__init__.py
+-rw-r--r--   0        0        0     8729 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/extension/table/cached_table.py
+-rw-r--r--   0        0        0     6039 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/extension/table/serialized_table.py
+-rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/extension/table/server_table.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/extension/table/session_table_handler.py
+-rw-r--r--   0        0        0    10604 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/extension/table/table_extension.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/extension/table/adapters/__init__.py
+-rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/extension/table/adapters/sqlitetable.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/extension/table/adapters/tableadapter.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/network/__init__.py
+-rw-r--r--   0        0        0     6179 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/network/network.py
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/network/packet_dispatcher.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/security/__init__.py
+-rw-r--r--   0        0        0     3692 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/security/security.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/server/__init__.py
+-rw-r--r--   0        0        0     6964 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/server/omuserver.py
+-rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/server/server.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/session/__init__.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/session/aiohttp_connection.py
+-rw-r--r--   0        0        0     6616 2020-02-02 00:00:00.000000 omuserver-0.3.0/src/omuserver/session/session.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 omuserver-0.3.0/test/helper_test.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 omuserver-0.3.0/.gitignore
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 omuserver-0.3.0/README.md
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 omuserver-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 omuserver-0.3.0/PKG-INFO
```

### Comparing `omuserver-0.2.5/src/omuserver/__main__.py` & `omuserver-0.3.0/src/omuserver/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 import asyncio
 import io
 import sys
 import tracemalloc
-from pathlib import Path
 
 import click
 from loguru import logger
-from omu import Address
+from omu.address import Address
 
 from omuserver.config import Config
 from omuserver.server.omuserver import OmuServer
 
 
 def setup_logging():
     if isinstance(sys.stdout, io.TextIOWrapper):
         sys.stdout.reconfigure(encoding="utf-8")
     if isinstance(sys.stderr, io.TextIOWrapper):
         sys.stderr.reconfigure(encoding="utf-8")
     logger.add(
         "logs/{time:YYYY-MM-DD}.log",
         rotation="1 day",
         colorize=False,
-        format="{time:YYYY-MM-DD HH:mm:ss} | {level: <8} | {name}:{function}:{line} - {message}",
+        format=(
+            "{time:YYYY-MM-DD HH:mm:ss} | {level: <8} | "
+            "{name}:{function}:{line} - {message}"
+        ),
     )
 
 
 @click.command()
 @click.option("--debug", is_flag=True)
 @click.option("--token", type=str, default=None)
 def main(debug: bool, token: str | None):
@@ -37,15 +39,14 @@
         port=26423,
         secure=False,
     )
     config.dashboard_token = token
 
     if debug:
         logger.warning("Debug mode enabled")
-        config.directories.plugins = (Path.cwd() / ".." / "plugins").resolve()
         config.strict_origin = False
         tracemalloc.start()
 
     server = OmuServer(config=config, loop=loop)
 
     logger.info("Starting server...")
     server.run()
```

### Comparing `omuserver-0.2.5/src/omuserver/directories.py` & `omuserver-0.3.0/src/omuserver/directories.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.5/src/omuserver/helper.py` & `omuserver-0.3.0/src/omuserver/helper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import sys
 from pathlib import Path
-from typing import List, TypedDict
+from typing import TypedDict
 
 
 def safe_path(root_path: Path, input_path: Path) -> Path:
     """
     How to prevent directory traversal attack from Python code
     https://stackoverflow.com/a/45190125
     """
@@ -17,15 +17,15 @@
 
 def safe_path_join(root: Path, *paths: Path | str) -> Path:
     return root / safe_path(root, root.joinpath(*paths))
 
 
 class LaunchCommand(TypedDict):
     cwd: str
-    args: List[str]
+    args: list[str]
 
 
 def get_launch_command() -> LaunchCommand:
     args = [sys.executable, "-m", "omuserver", *sys.argv[1:]]
     return {
         "cwd": os.getcwd(),
         "args": args,
```

### Comparing `omuserver-0.2.5/src/omuserver/extension/asset/asset_extension.py` & `omuserver-0.3.0/src/omuserver/extension/asset/asset_extension.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 from __future__ import annotations
 
 import abc
 from pathlib import Path
-from typing import TYPE_CHECKING, List
 
 from omu.extension.asset.asset_extension import (
     ASSET_DOWNLOAD_ENDPOINT,
     ASSET_DOWNLOAD_MANY_ENDPOINT,
     ASSET_UPLOAD_ENDPOINT,
     ASSET_UPLOAD_MANY_ENDPOINT,
     File,
 )
 from omu.identifier import Identifier
 
 from omuserver.helper import safe_path_join
+from omuserver.server import Server
+from omuserver.session import Session
 
-if TYPE_CHECKING:
-    from omuserver.server import Server
-    from omuserver.session import Session
+from .permissions import (
+    ASSET_DOWNLOAD_MANY_PERMISSION,
+    ASSET_DOWNLOAD_PERMISSION,
+    ASSET_UPLOAD_MANY_PERMISSION,
+    ASSET_UPLOAD_PERMISSION,
+)
 
 
 class AssetStorage(abc.ABC):
     @abc.abstractmethod
     async def store(self, file: File) -> Identifier: ...
 
     @abc.abstractmethod
@@ -45,40 +49,54 @@
         return File(identifier, file_path.read_bytes())
 
 
 class AssetExtension:
     def __init__(self, server: Server) -> None:
         self._server = server
         self.storage = FileStorage(server.directories.assets)
-        server.endpoints.bind_endpoint(ASSET_UPLOAD_ENDPOINT, self.handle_upload)
+        server.permissions.register(
+            ASSET_UPLOAD_PERMISSION,
+            ASSET_UPLOAD_MANY_PERMISSION,
+            ASSET_DOWNLOAD_PERMISSION,
+            ASSET_DOWNLOAD_MANY_PERMISSION,
+        )
+        server.endpoints.bind_endpoint(
+            ASSET_UPLOAD_ENDPOINT,
+            self.handle_upload,
+        )
+        server.endpoints.bind_endpoint(
+            ASSET_UPLOAD_MANY_ENDPOINT,
+            self.handle_upload_many,
+        )
         server.endpoints.bind_endpoint(
-            ASSET_UPLOAD_MANY_ENDPOINT, self.handle_upload_many
+            ASSET_DOWNLOAD_ENDPOINT,
+            self.handle_download,
         )
-        server.endpoints.bind_endpoint(ASSET_DOWNLOAD_ENDPOINT, self.handle_download)
         server.endpoints.bind_endpoint(
-            ASSET_DOWNLOAD_MANY_ENDPOINT, self.handle_download_many
+            ASSET_DOWNLOAD_MANY_ENDPOINT,
+            self.handle_download_many,
         )
 
     async def handle_upload(self, session: Session, file: File) -> Identifier:
         identifier = await self.storage.store(file)
         return identifier
 
     async def handle_upload_many(
-        self, session: Session, files: List[File]
-    ) -> List[Identifier]:
-        identifiers: List[Identifier] = []
+        self, session: Session, files: list[File]
+    ) -> list[Identifier]:
+        identifiers: list[Identifier] = []
         for file in files:
             identifier = await self.storage.store(file)
             identifiers.append(identifier)
         return identifiers
 
     async def handle_download(self, session: Session, identifier: Identifier) -> File:
         return await self.storage.retrieve(identifier)
 
     async def handle_download_many(
-        self, session: Session, identifiers: List[Identifier]
-    ) -> List[File]:
-        files: List[File] = []
+        self, session: Session, identifiers: list[Identifier]
+    ) -> list[File]:
+        files: list[File] = []
         for identifier in identifiers:
             file = await self.storage.retrieve(identifier)
             files.append(file)
         return files
```

### Comparing `omuserver-0.2.5/src/omuserver/extension/endpoint/endpoint_extension.py` & `omuserver-0.3.0/src/omuserver/extension/endpoint/endpoint_extension.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,83 +1,104 @@
 from __future__ import annotations
 
 import abc
-from typing import Dict, List
 
 from loguru import logger
+from omu.errors import PermissionDenied
 from omu.extension.endpoint.endpoint_extension import (
     ENDPOINT_CALL_PACKET,
     ENDPOINT_ERROR_PACKET,
     ENDPOINT_RECEIVE_PACKET,
     ENDPOINT_REGISTER_PACKET,
     EndpointDataPacket,
     EndpointErrorPacket,
     EndpointType,
 )
+from omu.extension.endpoint.packets import EndpointRegisterPacket
 from omu.helper import Coro
 from omu.identifier import Identifier
 
 from omuserver.server import Server
 from omuserver.session import Session
 
 
 class Endpoint(abc.ABC):
     @property
     @abc.abstractmethod
-    def identifier(self) -> Identifier: ...
+    def id(self) -> Identifier: ...
+
+    @property
+    @abc.abstractmethod
+    def permission(self) -> Identifier | None: ...
 
     @abc.abstractmethod
     async def call(self, data: EndpointDataPacket, session: Session) -> None: ...
 
 
 class SessionEndpoint(Endpoint):
-    def __init__(self, session: Session, identifier: Identifier) -> None:
+    def __init__(
+        self,
+        session: Session,
+        id: Identifier,
+        permission: Identifier | None,
+    ) -> None:
         self._session = session
-        self._identifier = identifier
+        self._id = id
+        self._permission = permission
+
+    @property
+    def id(self) -> Identifier:
+        return self._id
 
     @property
-    def identifier(self) -> Identifier:
-        return self._identifier
+    def permission(self) -> Identifier | None:
+        return self._permission
 
     async def call(self, data: EndpointDataPacket, session: Session) -> None:
         if self._session.closed:
             raise RuntimeError(f"Session {self._session.app.key()} already closed")
         await self._session.send(ENDPOINT_CALL_PACKET, data)
 
 
 class ServerEndpoint[Req, Res](Endpoint):
     def __init__(
         self,
         server: Server,
         endpoint: EndpointType[Req, Res],
         callback: Coro[[Session, Req], Res],
+        permission: Identifier | None = None,
     ) -> None:
         self._server = server
         self._endpoint = endpoint
         self._callback = callback
+        self._permission = permission
+
+    @property
+    def id(self) -> Identifier:
+        return self._endpoint.id
 
     @property
-    def identifier(self) -> Identifier:
-        return self._endpoint.identifier
+    def permission(self) -> Identifier | None:
+        return self._permission
 
     async def call(self, data: EndpointDataPacket, session: Session) -> None:
         if session.closed:
             raise RuntimeError("Session already closed")
         try:
-            req = self._endpoint.request_serializer.deserialize(data["data"])
+            req = self._endpoint.request_serializer.deserialize(data.data)
             res = await self._callback(session, req)
             json = self._endpoint.response_serializer.serialize(res)
             await session.send(
                 ENDPOINT_RECEIVE_PACKET,
-                EndpointDataPacket(type=data["type"], id=data["id"], data=json),
+                EndpointDataPacket(id=data.id, key=data.key, data=json),
             )
         except Exception as e:
             await session.send(
                 ENDPOINT_ERROR_PACKET,
-                EndpointErrorPacket(type=data["type"], id=data["id"], error=str(e)),
+                EndpointErrorPacket(id=data.id, key=data.key, error=str(e)),
             )
             raise e
 
 
 class EndpointCall:
     def __init__(self, session: Session, data: EndpointDataPacket) -> None:
         self._session = session
@@ -85,125 +106,151 @@
 
     async def receive(self, data: EndpointDataPacket) -> None:
         await self._session.send(ENDPOINT_RECEIVE_PACKET, data)
 
     async def error(self, error: str) -> None:
         await self._session.send(
             ENDPOINT_ERROR_PACKET,
-            EndpointErrorPacket(
-                type=self._data["type"], id=self._data["id"], error=error
-            ),
+            EndpointErrorPacket(id=self._data.id, key=self._data.key, error=error),
         )
 
 
 class EndpointExtension:
     def __init__(self, server: Server) -> None:
         self._server = server
-        self._endpoints: Dict[Identifier, Endpoint] = {}
-        self._calls: Dict[str, EndpointCall] = {}
+        self._endpoints: dict[Identifier, Endpoint] = {}
+        self._calls: dict[tuple[Identifier, int], EndpointCall] = {}
         server.packet_dispatcher.register(
             ENDPOINT_REGISTER_PACKET,
             ENDPOINT_CALL_PACKET,
             ENDPOINT_RECEIVE_PACKET,
             ENDPOINT_ERROR_PACKET,
         )
         server.packet_dispatcher.add_packet_handler(
-            ENDPOINT_REGISTER_PACKET, self._on_endpoint_register
+            ENDPOINT_REGISTER_PACKET, self.handle_register
         )
         server.packet_dispatcher.add_packet_handler(
-            ENDPOINT_CALL_PACKET, self._on_endpoint_call
+            ENDPOINT_CALL_PACKET, self.handle_call
         )
         server.packet_dispatcher.add_packet_handler(
-            ENDPOINT_RECEIVE_PACKET, self._on_endpoint_receive
+            ENDPOINT_RECEIVE_PACKET, self.handle_receive
         )
         server.packet_dispatcher.add_packet_handler(
-            ENDPOINT_ERROR_PACKET, self._on_endpoint_error
+            ENDPOINT_ERROR_PACKET, self.handle_error
         )
 
-    async def _on_endpoint_register(
-        self, session: Session, endpoint_identifiers: List[Identifier]
+    async def handle_register(
+        self, session: Session, packet: EndpointRegisterPacket
     ) -> None:
-        for identifier in endpoint_identifiers:
-            endpoint = SessionEndpoint(session, identifier)
-            self._endpoints[identifier] = endpoint
+        for id, permission in packet.endpoints.items():
+            if not id.is_subpath_of(session.app.id):
+                msg = f"App {session.app.key()} not allowed to register endpoint {id}"
+                raise PermissionDenied(msg)
+            self._endpoints[id] = SessionEndpoint(
+                session=session,
+                id=id,
+                permission=permission,
+            )
 
     def bind_endpoint[Req, Res](
         self,
         type: EndpointType[Req, Res],
         callback: Coro[[Session, Req], Res],
     ) -> None:
-        if type.identifier in self._endpoints:
-            raise ValueError(f"Endpoint {type.identifier.key()} already bound")
-        endpoint = ServerEndpoint(self._server, type, callback)
-        self._endpoints[type.identifier] = endpoint
+        if type.id in self._endpoints:
+            raise ValueError(f"Endpoint {type.id.key()} already bound")
+        endpoint = ServerEndpoint(
+            server=self._server,
+            endpoint=type,
+            callback=callback,
+            permission=type.permission_id,
+        )
+        self._endpoints[type.id] = endpoint
 
-    async def _on_endpoint_call(
-        self, session: Session, req: EndpointDataPacket
-    ) -> None:
-        endpoint = await self._get_endpoint(req, session)
+    def verify_permission(self, endpoint: Endpoint, session: Session):
+        if endpoint.id.is_namepath_equal(session.app.id, path_length=1):
+            return
+        if endpoint.permission is not None and self._server.permissions.has_permission(
+            session, endpoint.permission
+        ):
+            return
+        logger.warning(
+            f"{session.app.key()} tried to call endpoint {endpoint.id} "
+            f"without permission {endpoint.permission}"
+        )
+        error = (
+            f"Permission denied for endpoint {endpoint.id} "
+            f"with permission {endpoint.permission}"
+        )
+        raise PermissionDenied(error)
+
+    async def handle_call(self, session: Session, packet: EndpointDataPacket) -> None:
+        endpoint = await self._get_endpoint(packet, session)
         if endpoint is None:
             logger.warning(
-                f"{session.app.key()} tried to call unknown endpoint {req['type']}"
+                f"{session.app.key()} tried to call unknown endpoint {packet.id}"
             )
             await session.send(
                 ENDPOINT_ERROR_PACKET,
                 EndpointErrorPacket(
-                    type=req["type"],
-                    id=req["id"],
-                    error=f"Endpoint {req['type']} not found",
+                    id=packet.id,
+                    key=packet.key,
+                    error=f"Endpoint {packet.id} not found",
                 ),
             )
             return
-        await endpoint.call(req, session)
-        self._calls[f"{req['type']}:{req["id"]}"] = EndpointCall(session, req)
+        self.verify_permission(endpoint, session)
 
-    async def _on_endpoint_receive(
-        self, session: Session, req: EndpointDataPacket
+        await endpoint.call(packet, session)
+        key = (packet.id, packet.key)
+        self._calls[key] = EndpointCall(session, packet)
+
+    async def handle_receive(
+        self, session: Session, packet: EndpointDataPacket
     ) -> None:
-        call = self._calls.get(f"{req['type']}:{req['id']}")
+        key = (packet.id, packet.key)
+        call = self._calls.get(key)
         if call is None:
             await session.send(
                 ENDPOINT_ERROR_PACKET,
                 EndpointErrorPacket(
-                    type=req["type"],
-                    id=req["id"],
-                    error=f"Endpoint not found {req['type']}",
+                    id=packet.id,
+                    key=packet.key,
+                    error=f"Endpoint not found {packet.id}",
                 ),
             )
             return
-        await call.receive(req)
+        await call.receive(packet)
 
-    async def _on_endpoint_error(
-        self, session: Session, error: EndpointErrorPacket
-    ) -> None:
-        call = self._calls.get(f"{error['type']}:{error['id']}")
+    async def handle_error(self, session: Session, packet: EndpointErrorPacket) -> None:
+        key = (packet.id, packet.key)
+        call = self._calls.get(key)
         if call is None:
             await session.send(
                 ENDPOINT_ERROR_PACKET,
                 EndpointErrorPacket(
-                    type=error["type"],
-                    id=error["id"],
-                    error=f"Endpoint {error['type']} not found",
+                    id=packet.id,
+                    key=packet.key,
+                    error=f"Endpoint {packet.id} not found",
                 ),
             )
         else:
-            await call.error(error["error"])
+            await call.error(packet.error)
 
     async def _get_endpoint(
-        self, req: EndpointDataPacket, session: Session
+        self, packet: EndpointDataPacket, session: Session
     ) -> Endpoint | None:
-        identifier = Identifier.from_key(req["type"])
-        endpoint = self._endpoints.get(identifier)
+        endpoint = self._endpoints.get(packet.id)
         if endpoint is None:
             await session.send(
                 ENDPOINT_ERROR_PACKET,
                 EndpointErrorPacket(
-                    type=req["type"],
-                    id=req["id"],
-                    error=f"Endpoint {req['type']} not found",
+                    id=packet.id,
+                    key=packet.key,
+                    error=f"Endpoint {packet.id} not found",
                 ),
             )
             logger.warning(
-                f"{session.app.key()} tried to call unconnected endpoint {req['type']}"
+                f"{session.app.key()} tried to call unconnected endpoint {packet.id}"
             )
             return
         return endpoint
```

### Comparing `omuserver-0.2.5/src/omuserver/extension/plugin/plugin_connection.py` & `omuserver-0.3.0/src/omuserver/extension/plugin/plugin_connection.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.5/src/omuserver/extension/plugin/plugin_extension.py` & `omuserver-0.3.0/src/omuserver/extension/plugin/plugin_extension.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,76 +1,91 @@
 from __future__ import annotations
 
 import asyncio
-from typing import (
-    TYPE_CHECKING,
-    Dict,
-    List,
-)
+import time
 
+from omu.extension.dashboard.packets import PluginRequestPacket
+from omu.extension.plugin import PackageInfo
 from omu.extension.plugin.plugin_extension import (
-    PLUGIN_PERMISSION,
+    PLUGIN_ALLOWED_PACKAGE_TABLE,
     PLUGIN_REQUIRE_PACKET,
-    PLUGIN_WAIT_ENDPOINT,
-    WaitResponse,
 )
 from packaging.specifiers import SpecifierSet
 
+from omuserver.server import Server
 from omuserver.session import Session
 
 from .plugin_loader import DependencyResolver, PluginLoader
 
-if TYPE_CHECKING:
-    from omuserver.server import Server
-
 
 class PluginExtension:
     def __init__(self, server: Server) -> None:
-        self._server = server
-        self.lock = asyncio.Lock()
-        server.listeners.start += self.on_server_start
-        self.loader = PluginLoader(server)
-        self.dependency_resolver = DependencyResolver()
+        self.server = server
         server.packet_dispatcher.register(
             PLUGIN_REQUIRE_PACKET,
         )
         server.packet_dispatcher.add_packet_handler(
             PLUGIN_REQUIRE_PACKET,
             self.handle_require_packet,
         )
-        server.endpoints.bind_endpoint(
-            PLUGIN_WAIT_ENDPOINT,
-            self.handle_wait_endpoint,
-        )
-        server.permissions.register(
-            PLUGIN_PERMISSION,
-        )
+        server.network.event.start += self.on_network_start
+        self.request_id = 0
+        self.lock = asyncio.Lock()
+        self.loader = PluginLoader(server)
+        self.dependency_resolver = DependencyResolver()
+        self.allowed_packages = server.tables.register(PLUGIN_ALLOWED_PACKAGE_TABLE)
 
-    async def on_server_start(self) -> None:
-        await self.loader.load_plugins()
+    async def on_network_start(self) -> None:
+        await self.loader.run_plugins()
+
+    def _get_next_request_id(self) -> str:
+        self.request_id += 1
+        return f"{self.request_id}-{time.time_ns()}"
+
+    async def request_plugins(
+        self, session: Session, packages: dict[str, str | None]
+    ) -> None:
+        to_request: list[PackageInfo] = []
+        for package, version in packages.items():
+            package_info = await self.dependency_resolver.get_installed_package_info(
+                package
+            )
+            if package_info is None:
+                package_info = await self.dependency_resolver.fetch_package_info(
+                    package
+                )
+                to_request.append(package_info)
+                continue
+            await self.allowed_packages.add(package_info)
+        if len(to_request) == 0:
+            return
+        request = PluginRequestPacket(
+            request_id=self._get_next_request_id(),
+            app=session.app,
+            packages=to_request,
+        )
+        accepted = await self.server.dashboard.request_plugins(request)
+        if not accepted:
+            raise Exception("Request was not accepted")
 
     async def handle_require_packet(
-        self, session: Session, packages: Dict[str, str | None]
+        self, session: Session, packages: dict[str, str | None]
     ) -> None:
+        if not packages:
+            return
+        if not session.is_dashboard:
+            await self.request_plugins(session, packages)
+
         changed = False
         for package, version in packages.items():
             specifier = None
             if version is not None:
                 specifier = SpecifierSet(version)
             if self.dependency_resolver.add_dependencies({package: specifier}):
                 changed = True
 
         if not changed:
             return
 
         async with self.lock:
             await self.dependency_resolver.resolve()
             await self.loader.load_updated_plugins()
-
-    async def handle_wait_endpoint(
-        self, session: Session, plugins: List[str]
-    ) -> WaitResponse:
-        async with self.lock:
-            for plugin in plugins:
-                if plugin not in self.loader.plugins:
-                    return {"success": False}
-            return {"success": True}
```

### Comparing `omuserver-0.2.5/src/omuserver/extension/plugin/plugin_loader.py` & `omuserver-0.3.0/src/omuserver/extension/plugin/plugin_loader.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,105 +1,102 @@
 from __future__ import annotations
 
 import asyncio
 import importlib.metadata
 import importlib.util
 import sys
+import tempfile
+from collections.abc import Mapping
 from multiprocessing import Process
 from typing import (
-    TYPE_CHECKING,
-    Dict,
-    List,
-    Mapping,
     Protocol,
 )
 
+import aiohttp
+import uv
 from loguru import logger
-from omu import Address
+from omu.address import Address
+from omu.app import App
+from omu.client.token import TokenProvider
+from omu.extension.plugin import PackageInfo
+from omu.extension.plugin.plugin import PluginPackageInfo
 from omu.network.websocket_connection import WebsocketsConnection
 from omu.plugin import Plugin
 from packaging.specifiers import SpecifierSet
 from packaging.version import Version
 
+from omuserver.server import Server
 from omuserver.session import Session
 
 from .plugin_connection import PluginConnection
 from .plugin_session_connection import PluginSessionConnection
 
-if TYPE_CHECKING:
-    from omuserver.server import Server
-
 PLUGIN_GROUP = "omu.plugins"
 
 
 class PluginModule(Protocol):
     plugin: Plugin
 
 
 class DependencyResolver:
     def __init__(self) -> None:
-        self._dependencies: Dict[str, SpecifierSet] = {}
+        self._dependencies: dict[str, SpecifierSet] = {}
+
+    async def fetch_package_info(self, package: str) -> PackageInfo:
+        async with aiohttp.ClientSession() as session:
+            async with session.get(f"https://pypi.org/pypi/{package}/json") as response:
+                return await response.json()
+
+    async def get_installed_package_info(
+        self, package: str
+    ) -> PluginPackageInfo | None:
+        try:
+            package_info = importlib.metadata.distribution(package)
+        except importlib.metadata.PackageNotFoundError:
+            return None
+        return PluginPackageInfo(
+            package=package_info.name,
+            version=package_info.version,
+        )
 
     def format_dependencies(
         self, dependencies: Mapping[str, SpecifierSet | None]
-    ) -> List[str]:
+    ) -> list[str]:
         args = []
         for dependency, specifier in dependencies.items():
             if specifier is not None:
                 args.append(f"{dependency}{specifier}")
             else:
                 args.append(dependency)
         return args
 
-    async def _install(self, to_install: Mapping[str, SpecifierSet]) -> None:
-        if len(to_install) == 0:
-            return
-        logger.info(
-            "Installing dependencies " + ", ".join(self.format_dependencies(to_install))
-        )
-        install_process = await asyncio.create_subprocess_exec(
-            sys.executable,
-            "-m",
-            "pip",
-            "install",
-            "--upgrade",
-            *self.format_dependencies(to_install),
-            stdout=asyncio.subprocess.PIPE,
-            stderr=asyncio.subprocess.PIPE,
-        )
-        stdout, stderr = await install_process.communicate()
-        if install_process.returncode != 0:
-            logger.error(f"Error installing dependencies: {stderr}")
-            return
-        logger.info(f"Installed dependencies: {stdout}")
-
-    async def _update(self, to_update: Mapping[str, SpecifierSet]) -> None:
-        if len(to_update) == 0:
+    async def update_requirements(self, requirements: dict[str, SpecifierSet]) -> None:
+        if len(requirements) == 0:
             return
-        logger.info(
-            "Updating dependencies " + ", ".join(self.format_dependencies(to_update))
-        )
-        update_process = await asyncio.create_subprocess_exec(
-            sys.executable,
-            "-m",
-            "pip",
-            "install",
-            "--upgrade",
-            *[
-                f"{dependency}{specifier}"
-                for dependency, specifier in to_update.items()
-            ],
-            stdout=asyncio.subprocess.PIPE,
-            stderr=asyncio.subprocess.PIPE,
-        )
-        stdout, stderr = await update_process.communicate()
-        if update_process.returncode != 0:
-            logger.error(f"Error updating dependencies: {stderr}")
+        with tempfile.NamedTemporaryFile(mode="wb", delete=True) as req_file:
+            dependency_lines = self.format_dependencies(requirements)
+            req_file.write("\n".join(dependency_lines).encode("utf-8"))
+            req_file.flush()
+            process = await asyncio.create_subprocess_exec(
+                uv.find_uv_bin(),
+                "pip",
+                "install",
+                "--upgrade",
+                "-r",
+                req_file.name,
+                "--python",
+                sys.executable,
+                stdout=asyncio.subprocess.PIPE,
+                stderr=asyncio.subprocess.PIPE,
+            )
+            stdout, stderr = await process.communicate()
+        if process.returncode != 0:
+            logger.error(f"Error running uv command: {stderr}")
             return
-        logger.info(f"Updated dependencies: {stdout}")
+        logger.info(f"Ran uv command: {stdout or stderr}")
 
     def add_dependencies(self, dependencies: Mapping[str, SpecifierSet | None]) -> bool:
         changed = False
         for dependency, specifier in dependencies.items():
             if dependency not in self._dependencies:
                 self._dependencies[dependency] = SpecifierSet()
                 changed = True
@@ -109,60 +106,55 @@
                 if specifier_set != specifier:
                     changed = True
                 specifier_set &= specifier
                 continue
         return changed
 
     async def resolve(self):
-        to_install: Dict[str, SpecifierSet] = {}
-        to_update: Dict[str, SpecifierSet] = {}
-        skipped: Dict[str, SpecifierSet] = {}
+        requirements: dict[str, SpecifierSet] = {}
+        skipped: dict[str, SpecifierSet] = {}
         packages_distributions: Mapping[str, importlib.metadata.Distribution] = {
             dist.name: dist for dist in importlib.metadata.distributions()
         }
         for dependency, specifier in self._dependencies.items():
             package = packages_distributions.get(dependency)
             if package is None:
-                to_install[dependency] = specifier
+                requirements[dependency] = specifier
                 continue
             distribution = packages_distributions[package.name]
             installed_version = Version(distribution.version)
             specifier_set = self._dependencies[dependency]
             if installed_version in specifier_set:
                 skipped[dependency] = specifier_set
                 continue
-            to_update[dependency] = specifier_set
+            requirements[dependency] = specifier_set
 
-        await self._install(to_install)
-        await self._update(to_update)
+        await self.update_requirements(requirements)
         logger.info(
             f"Skipped dependencies: {", ".join(self.format_dependencies(skipped))}"
         )
 
 
 class PluginLoader:
     def __init__(self, server: Server) -> None:
         self._server = server
-        self.plugins: Dict[str, Plugin] = {}
-        server.listeners.start += self.handle_server_start
-        server.listeners.stop += self.handle_server_stop
+        self.plugins: dict[str, Plugin] = {}
+        server.event.start += self.handle_server_start
+        server.event.stop += self.handle_server_stop
 
     async def handle_server_start(self) -> None:
         for plugin in self.plugins.values():
             if plugin.on_start_server is not None:
                 await plugin.on_start_server(self._server)
 
     async def handle_server_stop(self) -> None:
         for plugin in self.plugins.values():
             if plugin.on_stop_server is not None:
                 await plugin.on_stop_server(self._server)
 
-    async def load_plugins(self) -> None:
-        await self.run_plugins()
-
     async def run_plugins(self):
         entry_points = importlib.metadata.entry_points(group=PLUGIN_GROUP)
         for entry_point in entry_points:
             if entry_point.dist is None:
                 raise ValueError(f"Invalid plugin: {entry_point} has no distribution")
             plugin_key = entry_point.dist.name
             if plugin_key in self.plugins:
@@ -180,29 +172,32 @@
             if plugin_key in self.plugins:
                 continue
             plugin = self.load_plugin_from_entry_point(entry_point)
             self.plugins[plugin_key] = plugin
             await self.run_plugin(plugin)
 
     async def run_plugin(self, plugin: Plugin):
+        token = await self._server.security.generate_plugin_token()
         if plugin.isolated:
             process = Process(
                 target=run_plugin_isolated,
                 args=(
                     plugin,
                     self._server.address,
+                    token,
                 ),
                 daemon=True,
             )
             process.start()
         else:
             if plugin.get_client is not None:
                 plugin_client = plugin.get_client()
                 connection = PluginConnection()
                 plugin_client.network.set_connection(connection)
+                plugin_client.network.set_token_provider(PluginTokenProvider(token))
                 await plugin_client.start()
                 session_connection = PluginSessionConnection(connection)
                 session = await Session.from_connection(
                     self._server,
                     self._server.packet_dispatcher.packet_mapper,
                     session_connection,
                 )
@@ -215,28 +210,41 @@
     ) -> Plugin:
         plugin = entry_point.load()
         if not isinstance(plugin, Plugin):
             raise ValueError(f"Invalid plugin: {plugin} is not a Plugin")
         return plugin
 
 
+class PluginTokenProvider(TokenProvider):
+    def __init__(self, token: str):
+        self._token = token
+
+    def get(self, server_address: Address, app: App) -> str | None:
+        return self._token
+
+    def store(self, server_address: Address, app: App, token: str) -> None:
+        raise NotImplementedError
+
+
 def handle_exception(loop: asyncio.AbstractEventLoop, context: dict) -> None:
     logger.error(context["message"])
     exception = context.get("exception")
     if exception:
         raise exception
 
 
 def run_plugin_isolated(
     plugin: Plugin,
     address: Address,
+    token: str,
 ) -> None:
     if plugin.get_client is None:
         raise ValueError(f"Invalid plugin: {plugin} has no client")
     client = plugin.get_client()
     connection = WebsocketsConnection(client, address)
     client.network.set_connection(connection)
+    client.network.set_token_provider(PluginTokenProvider(token))
     loop = asyncio.get_event_loop()
     loop.set_exception_handler(handle_exception)
     loop.run_until_complete(client.start())
     loop.run_forever()
     loop.close()
```

### Comparing `omuserver-0.2.5/src/omuserver/extension/plugin/plugin_session_connection.py` & `omuserver-0.3.0/src/omuserver/extension/plugin/plugin_session_connection.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.5/src/omuserver/extension/registry/registry.py` & `omuserver-0.3.0/src/omuserver/extension/registry/registry.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,33 @@
-from typing import Dict
-
 from omu import Identifier
+from omu.event_emitter import Unlisten
+from omu.extension.registry.packets import RegistryPermissions
 from omu.extension.registry.registry_extension import (
     REGISTRY_UPDATE_PACKET,
     RegistryPacket,
 )
 from omu.serializer import Serializable
 
 from omuserver.server import Server
 from omuserver.session import Session
 
 
 class ServerRegistry:
-    def __init__(self, server: Server, identifier: Identifier) -> None:
-        self.identifier = identifier
-        self._listeners: Dict[Identifier, Session] = {}
+    def __init__(
+        self,
+        server: Server,
+        id: Identifier,
+        permissions: RegistryPermissions | None = None,
+    ) -> None:
+        self.id = id
+        self.permissions = permissions or RegistryPermissions()
+        self._listeners: dict[Identifier, tuple[Session, Unlisten]] = {}
         self._path = server.directories.get(
             "registry"
-        ) / identifier.get_sanitized_path().with_suffix(".json")
+        ) / id.get_sanitized_path().with_suffix(".json")
         self._changed = False
         self.data: bytes | None = None
 
     async def load(self):
         if self._path.exists():
             self.data = self._path.read_bytes()
 
@@ -31,37 +37,37 @@
         if value is None:
             self._path.unlink(missing_ok=True)
         else:
             self._path.write_bytes(value)
         await self._notify()
 
     async def _notify(self) -> None:
-        for listener in self._listeners.values():
+        for listener, _ in self._listeners.values():
             if listener.closed:
                 raise Exception(f"Session {listener.app=} closed")
             await listener.send(
                 REGISTRY_UPDATE_PACKET,
-                RegistryPacket(identifier=self.identifier, value=self.data),
+                RegistryPacket(id=self.id, value=self.data),
             )
 
     async def attach_session(self, session: Session) -> None:
-        if session.app.identifier in self._listeners:
+        if session.app.id in self._listeners:
             raise Exception("Session already attached")
-        self._listeners[session.app.identifier] = session
-        session.listeners.disconnected += self.detach_session
+        unlisten = session.event.disconnected.listen(self.detach_session)
+        self._listeners[session.app.id] = session, unlisten
         await session.send(
             REGISTRY_UPDATE_PACKET,
-            RegistryPacket(identifier=self.identifier, value=self.data),
+            RegistryPacket(id=self.id, value=self.data),
         )
 
     async def detach_session(self, session: Session) -> None:
-        if session.app.identifier not in self._listeners:
+        if session.app.id not in self._listeners:
             raise Exception("Session not attached")
-        del self._listeners[session.app.identifier]
-        session.listeners.disconnected -= self.detach_session
+        _, unlisten = self._listeners.pop(session.app.id)
+        unlisten()
 
 
 class Registry[T]:
     def __init__(
         self,
         registry: ServerRegistry,
         default_value: T,
```

### Comparing `omuserver-0.2.5/src/omuserver/extension/table/cached_table.py` & `omuserver-0.3.0/src/omuserver/extension/table/cached_table.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,74 +1,81 @@
 from __future__ import annotations
 
 import asyncio
-from typing import TYPE_CHECKING, AsyncGenerator, Dict, List, Mapping
+from collections.abc import AsyncGenerator, Mapping
 
-from omu.extension.table import TableConfig
-from omu.extension.table.table_extension import TABLE_PROXY_PACKET, TableProxyData
+from omu.extension.table import TableConfig, TablePermissions
+from omu.extension.table.table_extension import TABLE_PROXY_PACKET, TableProxyPacket
 from omu.identifier import Identifier
 
+from omuserver.server import Server
+from omuserver.session import Session
+
 from .adapters.tableadapter import TableAdapter
-from .server_table import ServerTable, ServerTableListeners
+from .server_table import ServerTable, ServerTableEvents
 from .session_table_handler import SessionTableListener
 
-if TYPE_CHECKING:
-    from omuserver.server import Server
-    from omuserver.session import Session
-
 
 class CachedTable(ServerTable):
     def __init__(
         self,
         server: Server,
-        identifier: Identifier,
+        id: Identifier,
     ):
         self._server = server
-        self._identifier = identifier
-        self._listeners = ServerTableListeners()
-        self._sessions: Dict[Session, SessionTableListener] = {}
-        self._proxy_sessions: Dict[str, Session] = {}
+        self._id = id
+        self._event = ServerTableEvents()
+        self._sessions: dict[Session, SessionTableListener] = {}
+        self._permissions: TablePermissions | None = None
+        self._proxy_sessions: dict[str, Session] = {}
         self._changed = False
         self._proxy_id = 0
         self._save_task: asyncio.Task | None = None
         self._adapter: TableAdapter | None = None
-        self._config: TableConfig = {}
-
-        self._cache: Dict[str, bytes] = {}
+        self.config: TableConfig = {}
+        self._cache: dict[str, bytes] = {}
         self._cache_size: int | None = None
 
-    @property
-    def adapter(self) -> TableAdapter | None:
-        return self._adapter
+    def set_config(self, config: TableConfig) -> None:
+        self.config = config
+        self._cache_size = config.get("cache_size", None)
 
     @property
-    def cache(self) -> Dict[str, bytes]:
-        return self._cache
+    def permissions(self) -> TablePermissions | None:
+        return self._permissions
 
-    def set_config(self, config: TableConfig) -> None:
-        self._config = config
-        self._cache_size = config.get("cache_size", None)
+    def set_permissions(self, permissions: TablePermissions | None) -> None:
+        self._permissions = permissions
 
     def set_adapter(self, adapter: TableAdapter) -> None:
         self._adapter = adapter
 
+    async def load(self) -> None:
+        if self._adapter is None:
+            raise Exception("Table not set")
+        await self._adapter.load()
+
     async def store(self) -> None:
         if self._adapter is None:
             raise Exception("Table not set")
         if not self._changed:
             return
         self._changed = False
         await self._adapter.store()
 
     def attach_session(self, session: Session) -> None:
         if session in self._sessions:
             return
-        handler = SessionTableListener(self._identifier.key(), session, self)
+        handler = SessionTableListener(
+            id=self._id,
+            session=session,
+            table=self,
+        )
         self._sessions[session] = handler
-        session.listeners.disconnected += self.handle_disconnection
+        session.event.disconnected += self.handle_disconnection
 
     def detach_session(self, session: Session) -> None:
         if session in self._proxy_sessions:
             del self._proxy_sessions[session.app.key()]
         if session in self._sessions:
             handler = self._sessions.pop(session)
             handler.close()
@@ -86,19 +93,19 @@
             return self._cache[key]
         data = await self._adapter.get(key)
         if data is None:
             return None
         await self.update_cache({key: data})
         return data
 
-    async def get_many(self, *keys: str) -> Dict[str, bytes]:
+    async def get_many(self, *keys: str) -> dict[str, bytes]:
         key_list = list(keys)
         if self._adapter is None:
             raise Exception("Table not set")
-        items: Dict[str, bytes] = {}
+        items: dict[str, bytes] = {}
         for key in tuple(key_list):
             if key in self._cache:
                 items[key] = self._cache[key]
                 key_list.remove(key)
         if len(key_list) == 0:
             return items
         data = await self._adapter.get_many(key_list)
@@ -110,26 +117,26 @@
     async def add(self, items: Mapping[str, bytes]) -> None:
         if self._adapter is None:
             raise Exception("Table not set")
         if len(self._proxy_sessions) > 0:
             await self.send_proxy_event(items)
             return
         await self._adapter.set_all(items)
-        await self._listeners.add(items)
+        await self._event.add(items)
         await self.update_cache(items)
         self.mark_changed()
 
     async def send_proxy_event(self, items: Mapping[str, bytes]) -> None:
         session = tuple(self._proxy_sessions.values())[0]
         self._proxy_id += 1
         await session.send(
             TABLE_PROXY_PACKET,
-            TableProxyData(
+            TableProxyPacket(
+                id=self._id,
                 items=items,
-                type=self._identifier.key(),
                 key=self._proxy_id,
             ),
         )
 
     async def proxy(
         self, session: Session, key: int, items: Mapping[str, bytes]
     ) -> int:
@@ -141,91 +148,87 @@
         session_key = session.app.key()
         index = tuple(self._proxy_sessions.keys()).index(session_key)
         if index == len(self._proxy_sessions) - 1:
             adapter = self._adapter
             if adapter is None:
                 raise Exception("Table not set")
             await adapter.set_all(items)
-            await self._listeners.add(items)
+            await self._event.add(items)
             await self.update_cache(items)
             self.mark_changed()
             return 0
         session = tuple(self._proxy_sessions.values())[index + 1]
         await session.send(
             TABLE_PROXY_PACKET,
-            TableProxyData(
+            TableProxyPacket(
+                id=self._id,
                 items=items,
-                type=self._identifier.key(),
                 key=self._proxy_id,
             ),
         )
         return self._proxy_id
 
     async def update(self, items: Mapping[str, bytes]) -> None:
         if self._adapter is None:
             raise Exception("Table not set")
         await self._adapter.set_all(items)
-        await self._listeners.update(items)
+        await self._event.update(items)
         await self.update_cache(items)
         self.mark_changed()
 
-    async def remove(self, keys: List[str]) -> None:
+    async def remove(self, keys: list[str]) -> None:
         if self._adapter is None:
             raise Exception("Table not set")
         removed = await self._adapter.get_many(keys)
         await self._adapter.remove_all(keys)
         for key in keys:
             if key in self._cache:
                 del self._cache[key]
-        await self._listeners.remove(removed)
+        await self._event.remove(removed)
         self.mark_changed()
 
     async def clear(self) -> None:
         if self._adapter is None:
             raise Exception("Table not set")
         await self._adapter.clear()
-        await self._listeners.clear()
+        await self._event.clear()
         self._cache.clear()
         self.mark_changed()
 
     async def fetch_items(
         self,
         before: int | None = None,
         after: int | None = None,
         cursor: str | None = None,
-    ) -> Dict[str, bytes]:
+    ) -> dict[str, bytes]:
         if self._adapter is None:
             raise Exception("Table not set")
         return await self._adapter.fetch_items(before, after, cursor)
 
-    async def fetch_all(self) -> Dict[str, bytes]:
+    async def fetch_all(self) -> dict[str, bytes]:
         if self._adapter is None:
             raise Exception("Table not set")
         return await self._adapter.fetch_all()
 
     async def iterate(self) -> AsyncGenerator[bytes, None]:
         cursor: str | None = None
         while True:
             items = await self.fetch_items(
-                before=self._config.get("chunk_size", 100),
+                before=self.config.get("chunk_size", 100),
                 cursor=cursor,
             )
             if len(items) == 0:
                 break
             for item in items.values():
                 yield item
             *_, cursor = items.keys()
 
     async def size(self) -> int:
         return len(self._cache)
 
-    @property
-    def listeners(self) -> ServerTableListeners:
-        return self._listeners
-
     async def save_task(self) -> None:
         while self._changed:
             await self.store()
             await asyncio.sleep(30)
 
     def mark_changed(self) -> None:
         self._changed = True
@@ -238,8 +241,24 @@
     async def update_cache(self, items: Mapping[str, bytes]) -> None:
         if self._cache_size is None or self._cache_size <= 0:
             return
         for key, item in items.items():
             self._cache[key] = item
             if len(self._cache) > self._cache_size:
                 del self._cache[next(iter(self._cache))]
-        await self._listeners.cache_update(self._cache)
+        await self._event.cache_update(self._cache)
+
+    @property
+    def cache(self) -> Mapping[str, bytes]:
+        return self._cache
+
+    @property
+    def event(self) -> ServerTableEvents:
+        return self._event
+
+    @property
+    def id(self) -> Identifier:
+        return self._id
+
+    @property
+    def adapter(self) -> TableAdapter | None:
+        return self._adapter
```

### Comparing `omuserver-0.2.5/src/omuserver/extension/table/serialized_table.py` & `omuserver-0.3.0/src/omuserver/extension/table/serialized_table.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,14 @@
-from typing import AsyncGenerator, Callable, Dict, List, Mapping
+from collections.abc import AsyncGenerator, Mapping
 
-from omu.extension.table import Table, TableConfig, TableListeners, TableType
+from omu.event_emitter import Unlisten
+from omu.extension.table import Table, TableConfig, TableType
+from omu.extension.table.table import TableEvents, TablePermissions
 from omu.helper import AsyncCallback, Coro
+from omu.identifier import Identifier
 from omu.interface import Keyable
 from omu.serializer import Serializable
 
 from .server_table import ServerTable
 
 
 class SerializeAdapter[T: Keyable](Mapping[str, T]):
@@ -17,44 +20,64 @@
         return self._serializer.deserialize(self._cache[key])
 
 
 class SerializedTable[T: Keyable](Table[T]):
     def __init__(self, table: ServerTable, type: TableType[T]):
         self._table = table
         self._type = type
-        self._listeners = TableListeners[T](self)
-        self._proxies: List[Coro[[T], T | None]] = []
+        self._event = TableEvents[T](self)
+        self._proxies: list[Coro[[T], T | None]] = []
         self._chunk_size = 100
-        self.key = type.identifier.key()
+        self._permissions: TablePermissions | None = None
+        self.permission_read: Identifier | None = None
+        self.permission_write: Identifier | None = None
         self._listening = False
-        table.listeners.cache_update += self.on_cache_update
-        table.listeners.add += self.on_add
-        table.listeners.update += self.on_update
-        table.listeners.remove += self.on_remove
-        table.listeners.clear += self.on_clear
+        table.event.cache_update += self.on_cache_update
+        table.event.add += self.on_add
+        table.event.update += self.on_update
+        table.event.remove += self.on_remove
+        table.event.clear += self.on_clear
 
     @property
     def cache(self) -> Mapping[str, T]:
         return SerializeAdapter(self._table.cache, self._type.serializer)
 
+    def set_permissions(
+        self,
+        /,
+        all: Identifier | None = None,
+        read: Identifier | None = None,
+        write: Identifier | None = None,
+        remove: Identifier | None = None,
+        proxy: Identifier | None = None,
+    ) -> None:
+        self._permissions = TablePermissions(
+            all=all,
+            read=read,
+            write=write,
+            remove=remove,
+            proxy=proxy,
+        )
+        self._table.set_permissions(self._permissions)
+
     def set_config(self, config: TableConfig) -> None:
         self._table.set_config(config)
 
     def set_cache_size(self, size: int) -> None:
         self._table.set_cache_size(size)
 
     async def get(self, key: str) -> T | None:
         if key in self._table.cache:
             return self._type.serializer.deserialize(self._table.cache[key])
         item = await self._table.get(key)
         if item is None:
             return None
         return self._type.serializer.deserialize(item)
 
-    async def get_many(self, *keys: str) -> Dict[str, T]:
+    async def get_many(self, *keys: str) -> dict[str, T]:
         items = await self._table.get_many(*keys)
         return {
             key: self._type.serializer.deserialize(item) for key, item in items.items()
         }
 
     async def add(self, *items: T) -> None:
         data = {item.key(): self._type.serializer.serialize(item) for item in items}
@@ -71,19 +94,19 @@
         await self._table.clear()
 
     async def fetch_items(
         self,
         before: int | None = None,
         after: int | None = None,
         cursor: str | None = None,
-    ) -> Dict[str, T]:
+    ) -> dict[str, T]:
         items = await self._table.fetch_items(before, after, cursor)
         return self._parse_items(items)
 
-    async def fetch_all(self) -> Dict[str, T]:
+    async def fetch_all(self) -> dict[str, T]:
         items = await self._table.fetch_all()
         return self._parse_items(items)
 
     async def iterate(
         self,
         backward: bool = False,
         cursor: str | None = None,
@@ -106,48 +129,47 @@
                 yield item
             items.pop(cursor, None)
 
     async def size(self) -> int:
         return await self._table.size()
 
     @property
-    def listeners(self) -> TableListeners[T]:
-        return self._listeners
+    def event(self) -> TableEvents[T]:
+        return self._event
 
     def listen(
         self, listener: AsyncCallback[Mapping[str, T]] | None = None
-    ) -> Callable[[], None]:
+    ) -> Unlisten:
         self._listening = True
         if listener:
-            self._listeners.cache_update += listener
-            return lambda: self._listeners.cache_update.unsubscribe(listener)
+            return self._event.cache_update.listen(listener)
         return lambda: None
 
     async def on_cache_update(self, cache: Mapping[str, bytes]) -> None:
-        await self._listeners.cache_update(self._parse_items(cache))
+        await self._event.cache_update(self._parse_items(cache))
 
     async def on_add(self, items: Mapping[str, bytes]) -> None:
         _items = self._parse_items(items)
-        await self._listeners.add(_items)
+        await self._event.add(_items)
 
     async def on_update(self, items: Mapping[str, bytes]) -> None:
         _items = self._parse_items(items)
-        await self._listeners.update(_items)
+        await self._event.update(_items)
 
     async def on_remove(self, items: Mapping[str, bytes]) -> None:
         _items = self._parse_items(items)
-        await self._listeners.remove(_items)
+        await self._event.remove(_items)
 
     async def on_clear(self) -> None:
-        await self._listeners.clear()
+        await self._event.clear()
 
-    def proxy(self, callback: Coro[[T], T | None]) -> Callable[[], None]:
+    def proxy(self, callback: Coro[[T], T | None]) -> Unlisten:
         raise NotImplementedError
 
-    def _parse_items(self, items: Mapping[str, bytes]) -> Dict[str, T]:
-        parsed: Dict[str, T] = {}
+    def _parse_items(self, items: Mapping[str, bytes]) -> dict[str, T]:
+        parsed: dict[str, T] = {}
         for key, item in items.items():
             item = self._type.serializer.deserialize(item)
             if not item:
                 raise Exception(f"Failed to deserialize item {key}")
             parsed[key] = item
         return parsed
```

### Comparing `omuserver-0.2.5/src/omuserver/extension/table/server_table.py` & `omuserver-0.3.0/src/omuserver/extension/table/server_table.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,49 @@
 from __future__ import annotations
 
 import abc
-from typing import TYPE_CHECKING, AsyncGenerator, Dict, List, Mapping, Union
+from collections.abc import AsyncGenerator, Mapping
 
 from omu.event_emitter import EventEmitter
+from omu.extension.table import TableConfig
+from omu.extension.table.table import TablePermissions
+from omu.identifier import Identifier
 
-if TYPE_CHECKING:
-    from omu.extension.table import TableConfig
+from omuserver.session import Session
 
-    from omuserver.session import Session
+from .adapters.tableadapter import TableAdapter
 
-    from .adapters.tableadapter import TableAdapter
-
-type Json = Union[str, int, float, bool, None, Dict[str, Json], List[Json]]
+type Json = str | int | float | bool | None | dict[str, Json] | list[Json]
 
 
 class ServerTable(abc.ABC):
+    @abc.abstractmethod
+    async def load(self) -> None: ...
+
+    @abc.abstractmethod
+    async def store(self) -> None: ...
+
+    @property
+    @abc.abstractmethod
+    def id(self) -> Identifier: ...
+
     @property
     @abc.abstractmethod
-    def cache(self) -> Dict[str, bytes]: ...
+    def cache(self) -> Mapping[str, bytes]: ...
 
     @abc.abstractmethod
     def set_config(self, config: TableConfig) -> None: ...
 
+    @property
+    @abc.abstractmethod
+    def permissions(self) -> TablePermissions | None: ...
+
+    @abc.abstractmethod
+    def set_permissions(self, permissions: TablePermissions) -> None: ...
+
     @abc.abstractmethod
     def set_cache_size(self, size: int) -> None: ...
 
     @property
     @abc.abstractmethod
     def adapter(self) -> TableAdapter | None: ...
 
@@ -44,56 +61,53 @@
 
     @abc.abstractmethod
     async def proxy(
         self, session: Session, key: int, items: Mapping[str, bytes]
     ) -> int: ...
 
     @abc.abstractmethod
-    async def store(self) -> None: ...
-
-    @abc.abstractmethod
     async def get(self, key: str) -> bytes | None: ...
 
     @abc.abstractmethod
-    async def get_many(self, *keys: str) -> Dict[str, bytes]: ...
+    async def get_many(self, *keys: str) -> dict[str, bytes]: ...
 
     @abc.abstractmethod
     async def add(self, items: Mapping[str, bytes]) -> None: ...
 
     @abc.abstractmethod
     async def update(self, items: Mapping[str, bytes]) -> None: ...
 
     @abc.abstractmethod
-    async def remove(self, keys: List[str]) -> None: ...
+    async def remove(self, keys: list[str]) -> None: ...
 
     @abc.abstractmethod
     async def clear(self) -> None: ...
 
     @abc.abstractmethod
     async def fetch_items(
         self,
         before: int | None = None,
         after: int | None = None,
         cursor: str | None = None,
-    ) -> Dict[str, bytes]: ...
+    ) -> dict[str, bytes]: ...
 
     @abc.abstractmethod
-    async def fetch_all(self) -> Dict[str, bytes]: ...
+    async def fetch_all(self) -> dict[str, bytes]: ...
 
     @abc.abstractmethod
     async def iterate(self) -> AsyncGenerator[bytes, None]: ...
 
     @abc.abstractmethod
     async def size(self) -> int: ...
 
     @property
     @abc.abstractmethod
-    def listeners(self) -> ServerTableListeners: ...
+    def event(self) -> ServerTableEvents: ...
 
 
-class ServerTableListeners:
+class ServerTableEvents:
     def __init__(self) -> None:
         self.add = EventEmitter[Mapping[str, bytes]]()
         self.update = EventEmitter[Mapping[str, bytes]]()
         self.remove = EventEmitter[Mapping[str, bytes]]()
         self.clear = EventEmitter[[]]()
         self.cache_update = EventEmitter[Mapping[str, bytes]]()
```

### Comparing `omuserver-0.2.5/src/omuserver/extension/table/session_table_handler.py` & `omuserver-0.3.0/src/omuserver/extension/table/session_table_handler.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,75 +1,75 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Mapping
+from collections.abc import Mapping
+from typing import Any
 
 from omu.extension.table.table_extension import (
     TABLE_ITEM_ADD_PACKET,
     TABLE_ITEM_CLEAR_PACKET,
-    TABLE_ITEM_REMOVE_EVENT,
+    TABLE_ITEM_REMOVE_PACKET,
     TABLE_ITEM_UPDATE_PACKET,
-    TableEventData,
-    TableItemsData,
+    TableItemsPacket,
+    TablePacket,
 )
+from omu.helper import batch_call
+from omu.identifier import Identifier
 
 from omuserver.extension.table.server_table import ServerTable
-
-if TYPE_CHECKING:
-    from omuserver.session import Session
+from omuserver.session import Session
 
 
 class SessionTableListener:
-    def __init__(self, id: str, session: Session, table: ServerTable) -> None:
-        self._id = id
-        self._session = session
+    def __init__(self, id: Identifier, session: Session, table: ServerTable) -> None:
+        self.id = id
+        self.session = session
         self.table = table
-        table.listeners.add += self.on_add
-        table.listeners.update += self.on_update
-        table.listeners.remove += self.on_remove
-        table.listeners.clear += self.on_clear
+        self.unlisten = batch_call(
+            table.event.add.listen(self.on_add),
+            table.event.update.listen(self.on_update),
+            table.event.remove.listen(self.on_remove),
+            table.event.clear.listen(self.on_clear),
+        )
 
     def close(self) -> None:
-        self.table.listeners.add -= self.on_add
-        self.table.listeners.update -= self.on_update
-        self.table.listeners.remove -= self.on_remove
-        self.table.listeners.clear -= self.on_clear
+        self.unlisten()
 
     async def on_add(self, items: Mapping[str, Any]) -> None:
-        if self._session.closed:
+        if self.session.closed:
             return
-        await self._session.send(
+        await self.session.send(
             TABLE_ITEM_ADD_PACKET,
-            TableItemsData(
+            TableItemsPacket(
+                id=self.id,
                 items=items,
-                type=self._id,
             ),
         )
 
     async def on_update(self, items: Mapping[str, Any]) -> None:
-        if self._session.closed:
+        if self.session.closed:
             return
-        await self._session.send(
+        await self.session.send(
             TABLE_ITEM_UPDATE_PACKET,
-            TableItemsData(
+            TableItemsPacket(
+                id=self.id,
                 items=items,
-                type=self._id,
             ),
         )
 
     async def on_remove(self, items: Mapping[str, Any]) -> None:
-        if self._session.closed:
+        if self.session.closed:
             return
-        await self._session.send(
-            TABLE_ITEM_REMOVE_EVENT,
-            TableItemsData(
+        await self.session.send(
+            TABLE_ITEM_REMOVE_PACKET,
+            TableItemsPacket(
+                id=self.id,
                 items=items,
-                type=self._id,
             ),
         )
 
     async def on_clear(self) -> None:
-        if self._session.closed:
+        if self.session.closed:
             return
-        await self._session.send(TABLE_ITEM_CLEAR_PACKET, TableEventData(type=self._id))
+        await self.session.send(TABLE_ITEM_CLEAR_PACKET, TablePacket(id=self.id))
 
     def __repr__(self) -> str:
-        return f"<SessionTableHandler key={self._id} app={self._session.app}>"
+        return f"<SessionTableHandler key={self.id} app={self.session.app}>"
```

### Comparing `omuserver-0.2.5/src/omuserver/extension/table/adapters/sqlitetable.py` & `omuserver-0.3.0/src/omuserver/extension/table/adapters/sqlitetable.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import sqlite3
+from collections.abc import Mapping
 from pathlib import Path
-from typing import Dict, Mapping, Tuple
 
 from .tableadapter import TableAdapter
 
 
 class SqliteTableAdapter(TableAdapter):
     def __init__(self, path: Path) -> None:
         self._path = path
@@ -34,30 +34,30 @@
     async def get(self, key: str) -> bytes | None:
         cursor = self._conn.execute("SELECT value FROM data WHERE key = ?", (key,))
         row = cursor.fetchone()
         if row is None:
             return None
         return row[0]
 
-    async def get_many(self, keys: list[str]) -> Dict[str, bytes]:
+    async def get_many(self, keys: list[str]) -> dict[str, bytes]:
         cursor = self._conn.execute(
             f"SELECT key, value FROM data WHERE key IN ({','.join('?' for _ in keys)})",
             keys,
         )
         rows = cursor.fetchall()
         return {row[0]: row[1] for row in rows}
 
     async def set(self, key: str, value: bytes) -> None:
         self._conn.execute(
             "INSERT OR REPLACE INTO data (key, value) VALUES (?, ?)",
             (key, value),
         )
 
     async def set_all(self, items: Mapping[str, bytes]) -> None:
-        query = [(key, value) for key, value in items.items()]
+        query = list(items.items())
         self._conn.executemany(
             "INSERT OR REPLACE INTO data (key, value) VALUES (?, ?)",
             query,
         )
 
     async def remove(self, key: str) -> None:
         self._conn.execute("DELETE FROM data WHERE key = ?", (key,))
@@ -66,55 +66,57 @@
         self._conn.execute(
             f"DELETE FROM data WHERE key IN ({','.join('?' for _ in keys)})",
             keys,
         )
 
     async def fetch_items(
         self, before: int | None, after: int | None, cursor: str | None
-    ) -> Dict[str, bytes]:
+    ) -> dict[str, bytes]:
         cursor_id: int | None = None
         if cursor is not None:
             _cursor = self._conn.execute("SELECT id FROM data WHERE key = ?", (cursor,))
             row = _cursor.fetchone()
             if row is None:
                 raise ValueError(f"Cursor {cursor} not found")
             cursor_id = row[0]
 
         if before is None and after is None:
             _cursor = self._conn.execute("SELECT key, value FROM data")
             return {row[0]: (row[1]) for row in _cursor.fetchall()}
 
-        items: Dict[int, Tuple[str, bytes]] = {}
+        items: dict[int, tuple[str, bytes]] = {}
         if before is not None:
             if cursor_id is None:
                 _cursor = self._conn.execute(
                     "SELECT id, key, value FROM data ORDER BY id DESC LIMIT ?",
                     (before,),
                 )
             else:
                 _cursor = self._conn.execute(
-                    "SELECT id, key, value FROM data WHERE id <= ? ORDER BY id DESC LIMIT ?",
+                    "SELECT id, key, value FROM data WHERE id <= ? "
+                    "ORDER BY id DESC LIMIT ?",
                     (cursor_id, before),
                 )
             items.update({row[0]: (row[1], (row[2])) for row in _cursor.fetchall()})
         if after is not None:
             if cursor_id is None:
                 _cursor = self._conn.execute(
                     "SELECT id, key, value FROM data ORDER BY id LIMIT ?",
                     (after,),
                 )
             else:
                 _cursor = self._conn.execute(
-                    "SELECT id, key, value FROM data WHERE id >= ? ORDER BY id LIMIT ?",
+                    "SELECT id, key, value FROM data WHERE id >= ? "
+                    "ORDER BY id ASC LIMIT ?",
                     (cursor_id, after),
                 )
             items.update({row[0]: (row[1], (row[2])) for row in _cursor.fetchall()})
         return {key: value for _, (key, value) in sorted(items.items(), reverse=True)}
 
-    async def fetch_all(self) -> Dict[str, bytes]:
+    async def fetch_all(self) -> dict[str, bytes]:
         _cursor = self._conn.execute("SELECT key, value FROM data")
         return {row[0]: (row[1]) for row in _cursor.fetchall()}
 
     async def first(self) -> str | None:
         _cursor = self._conn.execute("SELECT key FROM data ORDER BY id LIMIT 1")
         row = _cursor.fetchone()
         if row is None:
```

### Comparing `omuserver-0.2.5/src/omuserver/extension/table/adapters/tableadapter.py` & `omuserver-0.3.0/src/omuserver/extension/table/adapters/tableadapter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import abc
+from collections.abc import Mapping
 from pathlib import Path
-from typing import Dict, List, Mapping
 
 
 class TableAdapter(abc.ABC):
     @classmethod
     @abc.abstractmethod
     def create(cls, path: Path) -> TableAdapter: ...
 
@@ -16,35 +16,35 @@
     @abc.abstractmethod
     async def load(self): ...
 
     @abc.abstractmethod
     async def get(self, key: str) -> bytes | None: ...
 
     @abc.abstractmethod
-    async def get_many(self, keys: List[str]) -> Dict[str, bytes]: ...
+    async def get_many(self, keys: list[str]) -> dict[str, bytes]: ...
 
     @abc.abstractmethod
     async def set(self, key: str, value: bytes) -> None: ...
 
     @abc.abstractmethod
     async def set_all(self, items: Mapping[str, bytes]) -> None: ...
 
     @abc.abstractmethod
     async def remove(self, key: str) -> None: ...
 
     @abc.abstractmethod
-    async def remove_all(self, keys: List[str]) -> None: ...
+    async def remove_all(self, keys: list[str]) -> None: ...
 
     @abc.abstractmethod
     async def fetch_items(
         self, before: int | None, after: int | None, cursor: str | None
-    ) -> Dict[str, bytes]: ...
+    ) -> dict[str, bytes]: ...
 
     @abc.abstractmethod
-    async def fetch_all(self) -> Dict[str, bytes]: ...
+    async def fetch_all(self) -> dict[str, bytes]: ...
 
     @abc.abstractmethod
     async def first(self) -> str | None: ...
 
     @abc.abstractmethod
     async def last(self) -> str | None: ...
```

### Comparing `omuserver-0.2.5/src/omuserver/network/network.py` & `omuserver-0.3.0/src/omuserver/network/network.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,77 @@
 from __future__ import annotations
 
+import asyncio
 import socket
-from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, Dict
 
 import psutil
 from aiohttp import web
 from loguru import logger
 from omu import App, Identifier
 from omu.event_emitter import EventEmitter
 from omu.helper import Coro
 from omu.network.packet import PACKET_TYPES, PacketType
-from omu.network.packet.packet_types import ConnectPacket
+from omu.network.packet.packet_types import DisconnectType
 
 from omuserver.network.packet_dispatcher import ServerPacketDispatcher
+from omuserver.server import Server
 from omuserver.session import Session
 from omuserver.session.aiohttp_connection import WebsocketsConnection
 
-if TYPE_CHECKING:
-    from omuserver.server import Server
-
-
-@dataclass(frozen=True)
-class PacketListeners[T]:
-    event_type: PacketType
-    listeners: EventEmitter[Session, T] = field(default_factory=EventEmitter)
-
 
 class Network:
     def __init__(
         self, server: Server, packet_dispatcher: ServerPacketDispatcher
     ) -> None:
         self._server = server
         self._packet_dispatcher = packet_dispatcher
-        self._listeners = NetworkListeners()
-        self._sessions: Dict[str, Session] = {}
+        self._event = NetworkEvents()
+        self._sessions: dict[Identifier, Session] = {}
         self._app = web.Application()
         self.add_websocket_route("/ws")
         self.register_packet(PACKET_TYPES.CONNECT, PACKET_TYPES.READY)
-        self.listeners.connected += self._packet_dispatcher.process_connection
+        self.add_packet_handler(PACKET_TYPES.READY, self._handle_ready)
+        self.event.connected += self._packet_dispatcher.process_connection
+
+    async def _handle_ready(self, session: Session, packet: None) -> None:
+        await session.wait_for_tasks()
+        if session.closed:
+            return
+        await session.send(PACKET_TYPES.READY, None)
+        logger.info(f"Ready: {session.app.key()}")
 
     def register_packet(self, *packet_types: PacketType) -> None:
         self._packet_dispatcher.register(*packet_types)
 
+    def add_packet_handler[T](
+        self,
+        packet_type: PacketType[T],
+        coro: Coro[[Session, T], None],
+    ) -> None:
+        self._packet_dispatcher.add_packet_handler(packet_type, coro)
+
     def add_http_route(
         self, path: str, handle: Coro[[web.Request], web.StreamResponse]
     ) -> None:
         self._app.router.add_get(path, handle)
 
-    def _validate_origin(self, request: web.Request, session: Session) -> None:
+    async def _validate_origin(self, request: web.Request, session: Session) -> None:
         origin = request.headers.get("origin")
         if origin is None:
             return
         origin_namespace = Identifier.namespace_from_url(origin)
-        namespace = session.app.identifier.namespace
+        namespace = session.app.id.namespace
         if origin_namespace == namespace:
             return
 
         if self._server.config.strict_origin:
+            await session.disconnect(
+                DisconnectType.INVALID_ORIGIN,
+                f"Invalid origin: {origin_namespace} != {namespace}",
+            )
             raise ValueError(f"Invalid origin: {origin_namespace} != {namespace}")
         else:
             logger.warning(f"Invalid origin: {origin_namespace} != {namespace}")
 
     def add_websocket_route(self, path: str) -> None:
         async def websocket_handler(request: web.Request) -> web.WebSocketResponse:
             ws = web.WebSocketResponse()
@@ -69,42 +79,45 @@
             connection = WebsocketsConnection(ws)
             session = await Session.from_connection(
                 self._server,
                 self._packet_dispatcher.packet_mapper,
                 connection,
             )
             if not session.is_dashboard:
-                self._validate_origin(request, session)
+                await self._validate_origin(request, session)
             await self.process_session(session)
             return ws
 
         self._app.router.add_get(path, websocket_handler)
 
     async def process_session(self, session: Session) -> None:
         if self.is_connected(session.app):
             logger.warning(f"Session {session.app} already connected")
-            await self._sessions[session.app.key()].disconnect()
-            return
-        self._sessions[session.app.key()] = session
-        session.listeners.disconnected += self.handle_disconnection
-        await self._listeners.connected.emit(session)
-        await session.send(PACKET_TYPES.CONNECT, ConnectPacket(app=session.app))
-        await session.listen()
+            old_session = self._sessions[session.app.id]
+            await old_session.disconnect(
+                DisconnectType.ANOTHER_CONNECTION,
+                f"Another connection from {session.app}",
+            )
+        self._sessions[session.app.id] = session
+        session.event.disconnected += self.handle_disconnection
+        await self._event.connected.emit(session)
+        listen_task = self._server.loop.create_task(session.listen())
+        await listen_task
 
     def is_connected(self, app: App) -> bool:
-        return app.key() in self._sessions
+        return app.id in self._sessions
 
     async def handle_disconnection(self, session: Session) -> None:
-        if session.app.key() not in self._sessions:
+        if session.app.id not in self._sessions:
             return
-        self._sessions.pop(session.app.key())
-        await self._listeners.disconnected.emit(session)
+        del self._sessions[session.app.id]
+        await self._event.disconnected.emit(session)
 
     async def _handle_start(self, app: web.Application) -> None:
-        await self._listeners.start.emit()
+        asyncio.create_task(self._event.start.emit())
 
     def is_port_free(self) -> bool:
         try:
             with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
                 s.bind(
                     (
                         self._server.address.host or "127.0.0.1",
@@ -117,34 +130,37 @@
 
     def get_process_by_port(self, port: int) -> psutil.Process | None:
         for connection in psutil.net_connections():
             if connection.laddr and connection.laddr.port == port:
                 return psutil.Process(connection.pid)
         return None
 
-    async def start(self) -> None:
+    def check_port_availability(self):
         if not self.is_port_free():
             process = self.get_process_by_port(self._server.address.port)
             if process is None:
                 raise OSError(f"Port {self._server.address.port} already in use")
             port = self._server.address.port
             name = process.name()
             pid = process.pid
             raise OSError(f"Port {port} already in use by {name} ({pid=})")
+
+    async def start(self) -> None:
+        self.check_port_availability()
         self._app.on_startup.append(self._handle_start)
         runner = web.AppRunner(self._app)
         await runner.setup()
         site = web.TCPSite(
             runner, host=self._server.address.host, port=self._server.address.port
         )
         await site.start()
 
     @property
-    def listeners(self) -> NetworkListeners:
-        return self._listeners
+    def event(self) -> NetworkEvents:
+        return self._event
 
 
-class NetworkListeners:
+class NetworkEvents:
     def __init__(self) -> None:
         self.start = EventEmitter[[]]()
         self.connected = EventEmitter[Session]()
         self.disconnected = EventEmitter[Session]()
```

### Comparing `omuserver-0.2.5/src/omuserver/network/packet_dispatcher.py` & `omuserver-0.3.0/src/omuserver/network/packet_dispatcher.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,59 +1,58 @@
 from __future__ import annotations
 
-from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, Callable, Dict
+from collections.abc import Callable
+from dataclasses import dataclass
 
 from loguru import logger
-from omu.event_emitter import EventEmitter
+from omu.helper import Coro
 from omu.identifier import Identifier
+from omu.network.packet import Packet, PacketType
 from omu.network.packet_mapper import PacketMapper
 
 from omuserver.session import Session
 
-if TYPE_CHECKING:
-    from omu.helper import Coro
-    from omu.network.packet import Packet, PacketType
-
 
 class ServerPacketDispatcher:
     def __init__(self):
         self.packet_mapper = PacketMapper()
-        self._packet_listeners: Dict[Identifier, PacketListeners] = {}
+        self._packet_listeners: dict[Identifier, PacketHandler] = {}
 
     async def process_connection(self, session: Session) -> None:
-        session.listeners.packet += self.process_packet
+        session.event.packet += self.process_packet
 
     async def process_packet(self, session: Session, packet: Packet) -> None:
-        listeners = self._packet_listeners.get(packet.type.identifier)
+        listeners = self._packet_listeners.get(packet.type.id)
         if not listeners:
-            logger.warning(f"Received unknown event type {packet.type}")
+            logger.warning(f"Received unknown packet type {packet.type}")
             return
-        await listeners.listeners.emit(session, packet.data)
+        if listeners.handler is None:
+            raise ValueError(f"No handler for packet type {packet.type}")
+        await listeners.handler(session, packet.data)
 
     def register(self, *types: PacketType) -> None:
         self.packet_mapper.register(*types)
         for type in types:
-            if self._packet_listeners.get(type.identifier):
-                raise ValueError(f"Event id {type.identifier} already registered")
-            self._packet_listeners[type.identifier] = PacketListeners(type)
+            if self._packet_listeners.get(type.id):
+                raise ValueError(f"Packet id {type.id} already registered")
+            self._packet_listeners[type.id] = PacketHandler(type)
 
     def add_packet_handler[T](
         self,
-        event_type: PacketType[T],
-        listener: Coro[[Session, T], None] | None = None,
+        packet_type: PacketType[T],
+        handler: Coro[[Session, T], None] | None = None,
     ) -> Callable[[Coro[[Session, T], None]], None]:
-        if not self._packet_listeners.get(event_type.identifier):
-            raise ValueError(f"Event type {event_type.identifier} not registered")
+        if not self._packet_listeners.get(packet_type.id):
+            raise ValueError(f"Packet type {packet_type.id} not registered")
 
         def decorator(func: Coro[[Session, T], None]) -> None:
-            self._packet_listeners[event_type.identifier].listeners.subscribe(func)
+            self._packet_listeners[packet_type.id].handler = func
 
-        if listener:
-            decorator(listener)
+        if handler:
+            decorator(handler)
         return decorator
 
 
-@dataclass(frozen=True)
-class PacketListeners[T]:
-    event_type: PacketType[T]
-    listeners: EventEmitter[Session, T] = field(default_factory=EventEmitter)
+@dataclass
+class PacketHandler[T]:
+    packet_type: PacketType[T]
+    handler: Coro[[Session, T], None] | None = None
```

### Comparing `omuserver-0.2.5/src/omuserver/server/omuserver.py` & `omuserver-0.3.0/src/omuserver/server/omuserver.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 import asyncio
 import json
-from typing import Mapping, Optional
+from collections.abc import Mapping
 
 import aiohttp
 from aiohttp import web
 from loguru import logger
 from omu import Identifier
-from omu.network import Address
+from omu.address import Address
 
 from omuserver import __version__
 from omuserver.config import Config
 from omuserver.directories import Directories
 from omuserver.extension.asset import AssetExtension
 from omuserver.extension.dashboard import DashboardExtension
 from omuserver.extension.endpoint import EndpointExtension
-from omuserver.extension.message import MessageExtension
+from omuserver.extension.i18n import I18nExtension
 from omuserver.extension.permission import PermissionExtension
 from omuserver.extension.plugin import PluginExtension
 from omuserver.extension.registry import RegistryExtension
 from omuserver.extension.server import ServerExtension
+from omuserver.extension.signal import SignalExtension
 from omuserver.extension.table import TableExtension
 from omuserver.helper import safe_path_join
 from omuserver.network import Network
 from omuserver.network.packet_dispatcher import ServerPacketDispatcher
 from omuserver.security.security import Security, ServerAuthenticator
 
-from .server import Server, ServerListeners
+from .server import Server, ServerEvents
 
 client = aiohttp.ClientSession(
     headers={
         "User-Agent": json.dumps(
             [
                 "omu",
                 {
@@ -42,38 +43,39 @@
 )
 
 
 class OmuServer(Server):
     def __init__(
         self,
         config: Config,
-        loop: Optional[asyncio.AbstractEventLoop] = None,
+        loop: asyncio.AbstractEventLoop | None = None,
     ) -> None:
         self._config = config
         self._loop = loop or asyncio.get_event_loop()
         self._address = config.address
-        self._listeners = ServerListeners()
+        self._event = ServerEvents()
         self._directories = config.directories
         self._directories.mkdir()
         self._packet_dispatcher = ServerPacketDispatcher()
         self._network = Network(self, self._packet_dispatcher)
-        self._network.listeners.start += self._handle_network_start
+        self._network.event.start += self._handle_network_start
         self._network.add_http_route("/proxy", self._handle_proxy)
         self._network.add_http_route("/asset", self._handle_assets)
         self._security = ServerAuthenticator(self)
         self._running = False
         self._endpoints = EndpointExtension(self)
-        self._dashboard = DashboardExtension(self)
         self._permissions = PermissionExtension(self)
         self._tables = TableExtension(self)
+        self._dashboard = DashboardExtension(self)
         self._registry = RegistryExtension(self)
         self._server = ServerExtension(self)
-        self._messages = MessageExtension(self)
+        self._signal = SignalExtension(self)
         self._plugins = PluginExtension(self)
         self._assets = AssetExtension(self)
+        self._i18n = I18nExtension(self)
 
     async def _handle_proxy(self, request: web.Request) -> web.StreamResponse:
         url = request.query.get("url")
         no_cache = bool(request.query.get("no_cache"))
         if not url:
             return web.Response(status=400)
         try:
@@ -84,16 +86,19 @@
                 }
                 resp.raise_for_status()
                 response = web.StreamResponse(
                     status=resp.status,
                     headers=headers,
                 )
                 await response.prepare(request)
-                async for chunk in resp.content.iter_any():
-                    await response.write(chunk)
+                try:
+                    async for chunk in resp.content.iter_any():
+                        await response.write(chunk)
+                except ConnectionResetError:
+                    pass
                 return response
         except aiohttp.ClientResponseError as e:
             return web.Response(status=e.status, text=e.message)
         except Exception as e:
             logger.error(e)
             return web.Response(status=500)
 
@@ -131,27 +136,27 @@
         exception = context.get("exception")
         if exception:
             raise exception
 
     async def _handle_network_start(self) -> None:
         logger.info(f"Listening on {self.address}")
         try:
-            await self._listeners.start()
+            await self._event.start()
         except Exception as e:
             await self.shutdown()
             self.loop.stop()
             raise e
 
     async def start(self) -> None:
         self._running = True
         await self._network.start()
 
     async def shutdown(self) -> None:
         self._running = False
-        await self._listeners.stop()
+        await self._event.stop()
 
     @property
     def config(self) -> Config:
         return self._config
 
     @property
     def loop(self) -> asyncio.AbstractEventLoop:
@@ -194,25 +199,29 @@
         return self._tables
 
     @property
     def registry(self) -> RegistryExtension:
         return self._registry
 
     @property
-    def messages(self) -> MessageExtension:
-        return self._messages
+    def signal(self) -> SignalExtension:
+        return self._signal
 
     @property
     def plugins(self) -> PluginExtension:
         return self._plugins
 
     @property
     def assets(self) -> AssetExtension:
         return self._assets
 
     @property
+    def i18n(self) -> I18nExtension:
+        return self._i18n
+
+    @property
     def running(self) -> bool:
         return self._running
 
     @property
-    def listeners(self) -> ServerListeners:
-        return self._listeners
+    def event(self) -> ServerEvents:
+        return self._event
```

### Comparing `omuserver-0.2.5/src/omuserver/server/server.py` & `omuserver-0.3.0/src/omuserver/server/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from __future__ import annotations
 
 import abc
 import asyncio
 from typing import TYPE_CHECKING
 
+from omu.address import Address
 from omu.event_emitter import EventEmitter
 
 if TYPE_CHECKING:
-    from omu.network import Address
-
     from omuserver.config import Config
     from omuserver.directories import Directories
     from omuserver.extension.asset import AssetExtension
     from omuserver.extension.dashboard import DashboardExtension
     from omuserver.extension.endpoint import EndpointExtension
-    from omuserver.extension.message import MessageExtension
+    from omuserver.extension.i18n import I18nExtension
     from omuserver.extension.permission import PermissionExtension
     from omuserver.extension.plugin import PluginExtension
     from omuserver.extension.registry import RegistryExtension
+    from omuserver.extension.signal import SignalExtension
     from omuserver.extension.table import TableExtension
     from omuserver.network import Network
     from omuserver.network.packet_dispatcher import ServerPacketDispatcher
     from omuserver.security import Security
 
 
-class ServerListeners:
+class ServerEvents:
     def __init__(self) -> None:
         self.start = EventEmitter[[]]()
         self.stop = EventEmitter[[]]()
 
 
 class Server(abc.ABC):
     @property
@@ -77,33 +77,37 @@
 
     @property
     @abc.abstractmethod
     def registry(self) -> RegistryExtension: ...
 
     @property
     @abc.abstractmethod
-    def messages(self) -> MessageExtension: ...
+    def signal(self) -> SignalExtension: ...
 
     @property
     @abc.abstractmethod
     def plugins(self) -> PluginExtension: ...
 
     @property
     @abc.abstractmethod
     def assets(self) -> AssetExtension: ...
 
     @property
     @abc.abstractmethod
+    def i18n(self) -> I18nExtension: ...
+
+    @property
+    @abc.abstractmethod
     def running(self) -> bool: ...
 
     @abc.abstractmethod
     def run(self) -> None: ...
 
     @abc.abstractmethod
     async def start(self) -> None: ...
 
     @abc.abstractmethod
     async def shutdown(self) -> None: ...
 
     @property
     @abc.abstractmethod
-    def listeners(self) -> ServerListeners: ...
+    def event(self) -> ServerEvents: ...
```

### Comparing `omuserver-0.2.5/src/omuserver/session/aiohttp_connection.py` & `omuserver-0.3.0/src/omuserver/session/aiohttp_connection.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from aiohttp import web
 from loguru import logger
-from omu.network.bytebuffer import ByteReader, ByteWriter
+from omu.bytebuffer import ByteReader, ByteWriter
 from omu.network.packet import Packet, PacketData
 from omu.network.packet_mapper import PacketMapper
 
 from .session import SessionConnection
 
 
 class WebsocketsConnection(SessionConnection):
@@ -52,10 +52,7 @@
         if self.closed:
             raise ValueError("Socket is closed")
         packet_data = packet_mapper.serialize(packet)
         writer = ByteWriter()
         writer.write_string(packet_data.type)
         writer.write_byte_array(packet_data.data)
         await self.socket.send_bytes(writer.finish())
-
-    def __repr__(self) -> str:
-        return f"WebsocketsConnection(socket={self.socket})"
```

### Comparing `omuserver-0.2.5/pyproject.toml` & `omuserver-0.3.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,30 @@
 [project]
 name = "omuserver"
-version = "0.2.5"
+version = "0.3.0"
 description = "Add your description here"
 authors = [
     { name = "am230", email = "111672334+am230@users.noreply.github.com" },
 ]
 dependencies = [
-    "sqlitedict>=2.1.0",
-    "click>=8.1.7",
-    "aiosqlite>=0.19.0",
     "loguru>=0.7.2",
+    "aiohttp>=3.9.3",
+    "click>=8.1.7",
     "omu>=0.1.4",
     "pip>=24.0",
-    "aiohttp>=3.9.3",
     "packaging>=24.0",
     "psutil>=5.9.8",
+    "result>=0.16.1",
+    "uv>=0.1.39",
 ]
 readme = "README.md"
 requires-python = ">= 3.12"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.rye]
 managed = true
 
-[tool.pylint]
-disable = [
-    "missing-module-docstring",
-    "missing-function-docstring",
-    "missing-class-docstring",
-]
-
 [tool.hatch.metadata]
 allow-direct-references = true
```

### Comparing `omuserver-0.2.5/PKG-INFO` & `omuserver-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.3
 Name: omuserver
-Version: 0.2.5
+Version: 0.3.0
 Summary: Add your description here
 Author-email: am230 <111672334+am230@users.noreply.github.com>
 Requires-Python: >=3.12
 Requires-Dist: aiohttp>=3.9.3
-Requires-Dist: aiosqlite>=0.19.0
 Requires-Dist: click>=8.1.7
 Requires-Dist: loguru>=0.7.2
 Requires-Dist: omu>=0.1.4
 Requires-Dist: packaging>=24.0
 Requires-Dist: pip>=24.0
 Requires-Dist: psutil>=5.9.8
-Requires-Dist: sqlitedict>=2.1.0
+Requires-Dist: result>=0.16.1
+Requires-Dist: uv>=0.1.39
 Description-Content-Type: text/markdown
 
 # server
 
 omuプロトコルのサーバー実装
```

