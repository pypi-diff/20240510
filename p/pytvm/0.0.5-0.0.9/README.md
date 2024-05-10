# Comparing `tmp/pytvm-0.0.5.tar.gz` & `tmp/pytvm-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytvm-0.0.5.tar", last modified: Wed Feb 28 13:43:34 2024, max compression
+gzip compressed data, was "pytvm-0.0.9.tar", last modified: Wed Feb 28 16:05:50 2024, max compression
```

## Comparing `pytvm-0.0.5.tar` & `pytvm-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 13:43:34.473097 pytvm-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-02-28 13:43:34.473097 pytvm-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-28 13:43:23.000000 pytvm-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 13:43:34.469097 pytvm-0.0.5/pytvm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 13:43:23.000000 pytvm-0.0.5/pytvm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 13:43:34.469097 pytvm-0.0.5/pytvm/engine/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-28 13:43:23.000000 pytvm-0.0.5/pytvm/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-02-28 13:43:23.000000 pytvm-0.0.5/pytvm/engine/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-02-28 13:43:23.000000 pytvm-0.0.5/pytvm/engine/engine_c.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 13:43:34.473097 pytvm-0.0.5/pytvm/transaction_emulator/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-28 13:43:23.000000 pytvm-0.0.5/pytvm/transaction_emulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-02-28 13:43:23.000000 pytvm-0.0.5/pytvm/transaction_emulator/blockchain_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-02-28 13:43:23.000000 pytvm-0.0.5/pytvm/transaction_emulator/trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-02-28 13:43:23.000000 pytvm-0.0.5/pytvm/transaction_emulator/transaction_emulator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 13:43:34.473097 pytvm-0.0.5/pytvm/tvm_emulator/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-28 13:43:23.000000 pytvm-0.0.5/pytvm/tvm_emulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-02-28 13:43:23.000000 pytvm-0.0.5/pytvm/tvm_emulator/tvm_emulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-02-28 13:43:23.000000 pytvm-0.0.5/pytvm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 13:43:34.473097 pytvm-0.0.5/pytvm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-02-28 13:43:34.000000 pytvm-0.0.5/pytvm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-02-28 13:43:34.000000 pytvm-0.0.5/pytvm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 13:43:34.000000 pytvm-0.0.5/pytvm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-28 13:43:34.000000 pytvm-0.0.5/pytvm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-28 13:43:34.000000 pytvm-0.0.5/pytvm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-28 13:43:34.473097 pytvm-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-02-28 13:43:23.000000 pytvm-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:05:50.125751 pytvm-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-02-28 16:05:50.125751 pytvm-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-02-28 16:05:37.000000 pytvm-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:05:50.121751 pytvm-0.0.9/pytvm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 16:05:37.000000 pytvm-0.0.9/pytvm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:05:50.125751 pytvm-0.0.9/pytvm/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-28 16:05:37.000000 pytvm-0.0.9/pytvm/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-02-28 16:05:37.000000 pytvm-0.0.9/pytvm/engine/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-02-28 16:05:37.000000 pytvm-0.0.9/pytvm/engine/engine_c.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:05:50.125751 pytvm-0.0.9/pytvm/transaction_emulator/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-28 16:05:37.000000 pytvm-0.0.9/pytvm/transaction_emulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-02-28 16:05:37.000000 pytvm-0.0.9/pytvm/transaction_emulator/blockchain_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-02-28 16:05:37.000000 pytvm-0.0.9/pytvm/transaction_emulator/trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-02-28 16:05:37.000000 pytvm-0.0.9/pytvm/transaction_emulator/transaction_emulator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:05:50.125751 pytvm-0.0.9/pytvm/tvm_emulator/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-28 16:05:37.000000 pytvm-0.0.9/pytvm/tvm_emulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-02-28 16:05:37.000000 pytvm-0.0.9/pytvm/tvm_emulator/tvm_emulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-02-28 16:05:37.000000 pytvm-0.0.9/pytvm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:05:50.125751 pytvm-0.0.9/pytvm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-02-28 16:05:50.000000 pytvm-0.0.9/pytvm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-02-28 16:05:50.000000 pytvm-0.0.9/pytvm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 16:05:50.000000 pytvm-0.0.9/pytvm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-28 16:05:50.000000 pytvm-0.0.9/pytvm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-28 16:05:50.000000 pytvm-0.0.9/pytvm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-28 16:05:50.125751 pytvm-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-02-28 16:05:37.000000 pytvm-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:05:50.125751 pytvm-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-02-28 16:05:37.000000 pytvm-0.0.9/tests/test_trans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-02-28 16:05:37.000000 pytvm-0.0.9/tests/test_tvm.py
```

### Comparing `pytvm-0.0.5/pytvm/engine/engine.py` & `pytvm-0.0.9/pytvm/engine/engine.py`

 * *Files identical despite different names*

### Comparing `pytvm-0.0.5/pytvm/engine/engine_c.py` & `pytvm-0.0.9/pytvm/engine/engine_c.py`

 * *Files identical despite different names*

### Comparing `pytvm-0.0.5/pytvm/transaction_emulator/trace.py` & `pytvm-0.0.9/pytvm/transaction_emulator/trace.py`

 * *Files identical despite different names*

### Comparing `pytvm-0.0.5/pytvm/transaction_emulator/transaction_emulator.py` & `pytvm-0.0.9/pytvm/transaction_emulator/transaction_emulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+import typing
+
 from ..engine import EmulatorEngine
 from ..utils import cell_to_b64, DEFAULT_CONFIG_BOC
 
 from pytoniq_core import Cell, Slice
 
 
 class TransactionEmulator:
 
     def __init__(
             self,
-            config: Cell | str = None,
+            config: typing.Union[Cell, str] = None,
             verbosity_level: int = 0,
             engine: EmulatorEngine = None
     ):
         """
         :param engine: TVM Engine
         :param config: blockchain config boc or Cell, if None - default config will be used
         :param verbosity_level:  Verbosity level of VM log. 0 - log truncated to last 256 characters. 1 - unlimited length log. 2 - for each command prints its cell hash and offset. 3 - for each command log prints all stack values.
```

### Comparing `pytvm-0.0.5/pytvm/tvm_emulator/tvm_emulator.py` & `pytvm-0.0.9/pytvm/tvm_emulator/tvm_emulator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import typing
+
 from ..engine import EmulatorEngine
 from ..utils import cell_to_b64, get_method_id, b64_to_cell
 
 from pytoniq_core import Cell, Slice
 
 
 class TvmEmulator:
@@ -40,40 +42,46 @@
 
     def set_debug_enabled(self, debug_enabled: bool):
         return self.engine.tvm_emulator_set_debug_enabled(self.emulator, debug_enabled)
 
     def raw_run_get_method(self, method_id: int, stack: Cell):
         return self.engine.tvm_emulator_run_get_method(self.emulator, method_id, cell_to_b64(stack))
 
-    def run_get_method(self, method: int | str, stack: list):
+    def run_get_method(self, method: typing.Union[int, str], stack: list):
         from pytoniq_core.tlb import VmStack
         if isinstance(method, str):
             method = get_method_id(method)
         stack = VmStack.serialize(stack)
         res = self.raw_run_get_method(method, stack)
         res['stack'] = VmStack.deserialize(Slice.one_from_boc(res['stack']))
+        if 'gas_used' in res:
+            res['gas_used'] = int(res['gas_used'])
         return res
 
     def raw_send_external_message(self, message: Cell):
         return self.engine.tvm_emulator_send_external_message(self.emulator, cell_to_b64(message))
 
     def send_external_message(self, body: Cell):
         from pytoniq_core.tlb.transaction import OutList
         res = self.raw_send_external_message(body)
         res['new_code'] = b64_to_cell(res['new_code'])
         res['new_data'] = b64_to_cell(res['new_data'])
         res['actions'] = OutList.deserialize(Slice.one_from_boc(res['actions'])) if res['actions'] else []
+        if 'gas_used' in res:
+            res['gas_used'] = int(res['gas_used'])
         return res
 
     def raw_send_internal_message(self, message: Cell, amount: int):
         return self.engine.tvm_emulator_send_internal_message(self.emulator, cell_to_b64(message), amount)
 
     def send_internal_message(self, message: Cell, amount: int):
         from pytoniq_core.tlb.transaction import OutList
         res = self.engine.tvm_emulator_send_internal_message(self.emulator, cell_to_b64(message), amount)
         res['new_code'] = b64_to_cell(res['new_code'])
         res['new_data'] = b64_to_cell(res['new_data'])
         res['actions'] = OutList.deserialize(Slice.one_from_boc(res['actions']))
+        if 'gas_used' in res:
+            res['gas_used'] = int(res['gas_used'])
         return res
 
     def __del__(self):
         self.engine.tvm_emulator_destroy(self.emulator)
```

### Comparing `pytvm-0.0.5/pytvm/utils.py` & `pytvm-0.0.9/pytvm/utils.py`

 * *Files identical despite different names*

### Comparing `pytvm-0.0.5/setup.py` & `pytvm-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     """Distribution which always forces a binary package with platform name"""
     def has_ext_modules(foo):
         return True
 
 
 setuptools.setup(
     name="pytvm",
-    version="0.0.5",
+    version="0.0.9",
     author="Maksim Kurbatov",
     author_email="cyrbatoff@gmail.com",
     description="Python TVM emulator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages('.', exclude=['.idea', 'tests', 'examples']),
     package_data={'pytvm': ['engine/**/*']},
```

