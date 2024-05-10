# Comparing `tmp/snek_sploit-0.4.0.tar.gz` & `tmp/snek_sploit-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snek_sploit-0.4.0.tar", max compression
+gzip compressed data, was "snek_sploit-0.5.0.tar", max compression
```

## Comparing `snek_sploit-0.4.0.tar` & `snek_sploit-0.5.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1069 2024-04-17 11:49:05.731010 snek_sploit-0.4.0/LICENSE
--rw-r--r--   0        0        0     1420 2024-04-17 11:49:05.731010 snek_sploit-0.4.0/README.md
--rw-r--r--   0        0        0      648 2024-04-17 11:49:05.731010 snek_sploit-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1331 2024-04-17 11:49:05.731010 snek_sploit-0.4.0/snek_sploit/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 11:49:05.731010 snek_sploit-0.4.0/snek_sploit/lib/__init__.py
--rw-r--r--   0        0        0     4595 2024-04-17 11:49:05.731010 snek_sploit-0.4.0/snek_sploit/lib/context.py
--rw-r--r--   0        0        0     3004 2024-04-17 11:49:05.731010 snek_sploit-0.4.0/snek_sploit/lib/metasploit.py
--rw-r--r--   0        0        0        0 2024-04-17 11:49:05.731010 snek_sploit-0.4.0/snek_sploit/lib/rpc/__init__.py
--rw-r--r--   0        0        0     3086 2024-04-17 11:49:05.731010 snek_sploit-0.4.0/snek_sploit/lib/rpc/auth.py
--rw-r--r--   0        0        0     9284 2024-04-17 11:49:05.731010 snek_sploit-0.4.0/snek_sploit/lib/rpc/consoles.py
--rw-r--r--   0        0        0     7892 2024-04-17 11:49:05.731010 snek_sploit-0.4.0/snek_sploit/lib/rpc/core.py
--rw-r--r--   0        0        0    12331 2024-04-17 11:49:05.731010 snek_sploit-0.4.0/snek_sploit/lib/rpc/db.py
--rw-r--r--   0        0        0      728 2024-04-17 11:49:05.731010 snek_sploit-0.4.0/snek_sploit/lib/rpc/health.py
--rw-r--r--   0        0        0     2676 2024-04-17 11:49:05.731010 snek_sploit-0.4.0/snek_sploit/lib/rpc/jobs.py
--rw-r--r--   0        0        0    19865 2024-04-17 11:49:05.731010 snek_sploit-0.4.0/snek_sploit/lib/rpc/modules.py
--rw-r--r--   0        0        0     1629 2024-04-17 11:49:05.735010 snek_sploit-0.4.0/snek_sploit/lib/rpc/plugins.py
--rw-r--r--   0        0        0    24221 2024-04-17 11:49:05.735010 snek_sploit-0.4.0/snek_sploit/lib/rpc/sessions.py
--rw-r--r--   0        0        0        0 2024-04-17 11:49:05.735010 snek_sploit-0.4.0/snek_sploit/util/__init__.py
--rw-r--r--   0        0        0     1887 2024-04-17 11:49:05.735010 snek_sploit-0.4.0/snek_sploit/util/constants.py
--rw-r--r--   0        0        0      448 2024-04-17 11:49:05.735010 snek_sploit-0.4.0/snek_sploit/util/enums.py
--rw-r--r--   0        0        0      276 2024-04-17 11:49:05.735010 snek_sploit-0.4.0/snek_sploit/util/exceptions.py
--rw-r--r--   0        0        0     2308 1970-01-01 00:00:00.000000 snek_sploit-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-10 12:23:03.555946 snek_sploit-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1420 2024-05-10 12:23:03.559946 snek_sploit-0.5.0/README.md
+-rw-r--r--   0        0        0      686 2024-05-10 12:23:03.559946 snek_sploit-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1331 2024-05-10 12:23:03.559946 snek_sploit-0.5.0/snek_sploit/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 12:23:03.559946 snek_sploit-0.5.0/snek_sploit/lib/__init__.py
+-rw-r--r--   0        0        0     4595 2024-05-10 12:23:03.559946 snek_sploit-0.5.0/snek_sploit/lib/context.py
+-rw-r--r--   0        0        0     3004 2024-05-10 12:23:03.559946 snek_sploit-0.5.0/snek_sploit/lib/metasploit.py
+-rw-r--r--   0        0        0        0 2024-05-10 12:23:03.559946 snek_sploit-0.5.0/snek_sploit/lib/rpc/__init__.py
+-rw-r--r--   0        0        0     3086 2024-05-10 12:23:03.559946 snek_sploit-0.5.0/snek_sploit/lib/rpc/auth.py
+-rw-r--r--   0        0        0    10952 2024-05-10 12:23:03.559946 snek_sploit-0.5.0/snek_sploit/lib/rpc/consoles.py
+-rw-r--r--   0        0        0     7892 2024-05-10 12:23:03.559946 snek_sploit-0.5.0/snek_sploit/lib/rpc/core.py
+-rw-r--r--   0        0        0    12331 2024-05-10 12:23:03.559946 snek_sploit-0.5.0/snek_sploit/lib/rpc/db.py
+-rw-r--r--   0        0        0      728 2024-05-10 12:23:03.559946 snek_sploit-0.5.0/snek_sploit/lib/rpc/health.py
+-rw-r--r--   0        0        0     2676 2024-05-10 12:23:03.559946 snek_sploit-0.5.0/snek_sploit/lib/rpc/jobs.py
+-rw-r--r--   0        0        0    19865 2024-05-10 12:23:03.559946 snek_sploit-0.5.0/snek_sploit/lib/rpc/modules.py
+-rw-r--r--   0        0        0     1629 2024-05-10 12:23:03.559946 snek_sploit-0.5.0/snek_sploit/lib/rpc/plugins.py
+-rw-r--r--   0        0        0    24221 2024-05-10 12:23:03.559946 snek_sploit-0.5.0/snek_sploit/lib/rpc/sessions.py
+-rw-r--r--   0        0        0        0 2024-05-10 12:23:03.559946 snek_sploit-0.5.0/snek_sploit/util/__init__.py
+-rw-r--r--   0        0        0     1887 2024-05-10 12:23:03.559946 snek_sploit-0.5.0/snek_sploit/util/constants.py
+-rw-r--r--   0        0        0      448 2024-05-10 12:23:03.559946 snek_sploit-0.5.0/snek_sploit/util/enums.py
+-rw-r--r--   0        0        0      276 2024-05-10 12:23:03.559946 snek_sploit-0.5.0/snek_sploit/util/exceptions.py
+-rw-r--r--   0        0        0     2320 1970-01-01 00:00:00.000000 snek_sploit-0.5.0/PKG-INFO
```

### Comparing `snek_sploit-0.4.0/LICENSE` & `snek_sploit-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.4.0/README.md` & `snek_sploit-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.4.0/pyproject.toml` & `snek_sploit-0.5.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snek-sploit"
-version = "0.4.0"
+version = "0.5.0"
 description = "Python RPC client for Metasploit Framework"
 authors = [
     "Jiří Rája <jiri.raja@gmail.com>"
 ]
 maintainers = [
     "Jiří Rája <jiri.raja@gmail.com>"
 ]
@@ -14,16 +14,19 @@
 keywords = [
     "metasploit", "msf", "rpc", "client"
 ]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-requests = "^2.31"
-msgpack = "^1"
+requests = "^2.31.0"
+msgpack = "^1.0.8"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24"
 
+[tool.black]
+line-length = 120
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `snek_sploit-0.4.0/snek_sploit/__init__.py` & `snek_sploit-0.5.0/snek_sploit/__init__.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.4.0/snek_sploit/lib/context.py` & `snek_sploit-0.5.0/snek_sploit/lib/context.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.4.0/snek_sploit/lib/metasploit.py` & `snek_sploit-0.5.0/snek_sploit/lib/metasploit.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.4.0/snek_sploit/lib/rpc/auth.py` & `snek_sploit-0.5.0/snek_sploit/lib/rpc/auth.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.4.0/snek_sploit/lib/rpc/consoles.py` & `snek_sploit-0.5.0/snek_sploit/lib/rpc/consoles.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import random
+import string
 from dataclasses import dataclass, asdict
 from typing import List
 import time
 
 from snek_sploit.lib.context import ContextBase, Context
 from snek_sploit.util import constants, exceptions
 
@@ -217,47 +219,80 @@
 
     def destroy(self) -> bool:
         return self._rpc.destroy(self.id)
 
     def tabs(self, line: str) -> List[str]:
         return self._rpc.tabs(self.id, line)
 
-    def gather_output(self, timeout: float = None, reading_delay: float = 1) -> str:
+    def gather_output(
+        self, timeout: float = None, reading_delay: float = 1, end_check: str = "", end_check_hard_stop: bool = False
+    ) -> str:
         """
         Gather output from the console.
         :param timeout: The maximum time to wait for the output
         :param reading_delay: Delay between the readings
+        :param end_check: String that is checked regularly to check whether the execution has finished
+        :param end_check_hard_stop: Whether to exit once the `end_check` is found
         :return: Gathered output
         """
         if timeout is not None:
             timeout = time.time() + timeout
 
         output = ""
-        # TODO: shell wont be busy until the command is executed, check for the execution
-        while (console := self.read()).busy:
+        end_is_nigh = False
+        while (console := self.read()).busy or console.data or not output or (end_check and not end_is_nigh):
             output += console.data
 
+            if end_check and end_check in console.data:
+                if end_check_hard_stop:
+                    break
+                end_is_nigh = True  # In case the console is still busy, continue to gather the data
+
             if timeout and time.time() >= timeout:
                 break
+
             time.sleep(reading_delay)
 
         return output
 
     def clear_buffer(self) -> None:
         """
         Clear unread data from the console.
         :return: None
         """
         self.read()
 
-    def execute(self, command: str, timeout: float = None, reading_delay: float = 1) -> str:
+    def execute(
+        self,
+        command: str,
+        timeout: float = None,
+        reading_delay: float = 1,
+        end_check: str = "",
+        generate_end_check: bool = True,
+        end_check_hard_stop: bool = False,
+    ) -> str:
+        """
+        Execute a command or a set of commands (separated with `\n`) and gather it's output.
+        By default, an end_check is generated and appended to the command to ensure the whole output is captured.
+        :param command: Command that will be executed in the console.
+        :param timeout: The maximum time to wait for the output
+        :param reading_delay: Delay between the readings
+        :param end_check: String that is checked regularly to check whether the execution has finished
+        :param generate_end_check: If `end_check` is empty, generate a custom one and add it to the command
+        :param end_check_hard_stop: Whether to exit once the `end_check` is found and discard the rest of the output
+        :return: Execution output
+        """
+        if not end_check and generate_end_check:
+            end_check = "".join(random.choices(string.ascii_letters + string.digits, k=20))
+            command += f"\necho '{end_check}'"
+
         self.clear_buffer()
         self.write(command)
 
-        return self.gather_output(timeout, reading_delay)
+        return self.gather_output(timeout, reading_delay, end_check, end_check_hard_stop)
 
 
 class Consoles(ContextBase):
     def __init__(self, context: Context):
         super().__init__(context)
         self.rpc = RPCConsoles(context)
```

### Comparing `snek_sploit-0.4.0/snek_sploit/lib/rpc/core.py` & `snek_sploit-0.5.0/snek_sploit/lib/rpc/core.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.4.0/snek_sploit/lib/rpc/db.py` & `snek_sploit-0.5.0/snek_sploit/lib/rpc/db.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.4.0/snek_sploit/lib/rpc/health.py` & `snek_sploit-0.5.0/snek_sploit/lib/rpc/health.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.4.0/snek_sploit/lib/rpc/jobs.py` & `snek_sploit-0.5.0/snek_sploit/lib/rpc/jobs.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.4.0/snek_sploit/lib/rpc/modules.py` & `snek_sploit-0.5.0/snek_sploit/lib/rpc/modules.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.4.0/snek_sploit/lib/rpc/plugins.py` & `snek_sploit-0.5.0/snek_sploit/lib/rpc/plugins.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.4.0/snek_sploit/lib/rpc/sessions.py` & `snek_sploit-0.5.0/snek_sploit/lib/rpc/sessions.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.4.0/snek_sploit/util/constants.py` & `snek_sploit-0.5.0/snek_sploit/util/constants.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.4.0/PKG-INFO` & `snek_sploit-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snek-sploit
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python RPC client for Metasploit Framework
 Home-page: https://github.com/SadParad1se/snek-sploit
 License: MIT
 Keywords: metasploit,msf,rpc,client
 Author: Jiří Rája
 Author-email: jiri.raja@gmail.com
 Maintainer: Jiří Rája
@@ -13,16 +13,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: msgpack (>=1,<2)
-Requires-Dist: requests (>=2.31,<3.0)
+Requires-Dist: msgpack (>=1.0.8,<2.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/SadParad1se/snek-sploit
 Description-Content-Type: text/markdown
 
 # snek-sploit
 Python typed RPC client for Metasploit Framework.
 
 ![](logo.png)
```

