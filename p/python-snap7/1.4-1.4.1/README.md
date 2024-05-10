# Comparing `tmp/python_snap7-1.4.tar.gz` & `tmp/python_snap7-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_snap7-1.4.tar", last modified: Fri May  3 10:38:25 2024, max compression
+gzip compressed data, was "python_snap7-1.4.1.tar", last modified: Fri May 10 13:50:03 2024, max compression
```

## Comparing `python_snap7-1.4.tar` & `python_snap7-1.4.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 gijs      (1000) gijs      (1000)        0 2024-05-03 10:38:25.133252 python_snap7-1.4/
--rw-rw-r--   0 gijs      (1000) gijs      (1000)     1097 2024-05-02 10:39:46.000000 python_snap7-1.4/LICENSE
--rw-rw-r--   0 gijs      (1000) gijs      (1000)       19 2024-05-02 10:39:46.000000 python_snap7-1.4/MANIFEST.in
--rw-r--r--   0 gijs      (1000) gijs      (1000)     1298 2024-05-03 10:38:25.133252 python_snap7-1.4/PKG-INFO
--rw-rw-r--   0 gijs      (1000) gijs      (1000)      699 2024-05-03 09:44:07.000000 python_snap7-1.4/README.rst
--rw-rw-r--   0 gijs      (1000) gijs      (1000)     1695 2024-05-03 09:44:07.000000 python_snap7-1.4/pyproject.toml
-drwxrwxr-x   0 gijs      (1000) gijs      (1000)        0 2024-05-03 10:38:25.132252 python_snap7-1.4/python_snap7.egg-info/
--rw-r--r--   0 gijs      (1000) gijs      (1000)     1298 2024-05-03 10:38:25.000000 python_snap7-1.4/python_snap7.egg-info/PKG-INFO
--rw-rw-r--   0 gijs      (1000) gijs      (1000)      705 2024-05-03 10:38:25.000000 python_snap7-1.4/python_snap7.egg-info/SOURCES.txt
--rw-rw-r--   0 gijs      (1000) gijs      (1000)        1 2024-05-03 10:38:25.000000 python_snap7-1.4/python_snap7.egg-info/dependency_links.txt
--rw-rw-r--   0 gijs      (1000) gijs      (1000)       60 2024-05-03 10:38:25.000000 python_snap7-1.4/python_snap7.egg-info/entry_points.txt
--rw-rw-r--   0 gijs      (1000) gijs      (1000)       91 2024-05-03 10:38:25.000000 python_snap7-1.4/python_snap7.egg-info/requires.txt
--rw-rw-r--   0 gijs      (1000) gijs      (1000)        6 2024-05-03 10:38:25.000000 python_snap7-1.4/python_snap7.egg-info/top_level.txt
--rw-rw-r--   0 gijs      (1000) gijs      (1000)       38 2024-05-03 10:38:25.133252 python_snap7-1.4/setup.cfg
-drwxrwxr-x   0 gijs      (1000) gijs      (1000)        0 2024-05-03 10:38:25.131252 python_snap7-1.4/snap7/
--rw-rw-r--   0 gijs      (1000) gijs      (1000)      418 2024-05-02 10:39:46.000000 python_snap7-1.4/snap7/__init__.py
-drwxrwxr-x   0 gijs      (1000) gijs      (1000)        0 2024-05-03 10:38:25.131252 python_snap7-1.4/snap7/client/
--rw-rw-r--   0 gijs      (1000) gijs      (1000)    52714 2024-05-03 10:38:12.000000 python_snap7-1.4/snap7/client/__init__.py
--rw-rw-r--   0 gijs      (1000) gijs      (1000)     4812 2024-05-02 10:39:46.000000 python_snap7-1.4/snap7/common.py
--rw-rw-r--   0 gijs      (1000) gijs      (1000)     3591 2024-05-02 10:39:46.000000 python_snap7-1.4/snap7/error.py
--rw-rw-r--   0 gijs      (1000) gijs      (1000)       81 2024-05-02 10:39:46.000000 python_snap7-1.4/snap7/exceptions.py
--rw-rw-r--   0 gijs      (1000) gijs      (1000)    11808 2024-05-02 10:39:46.000000 python_snap7-1.4/snap7/logo.py
--rw-rw-r--   0 gijs      (1000) gijs      (1000)     7643 2024-05-02 10:39:46.000000 python_snap7-1.4/snap7/partner.py
--rw-rw-r--   0 gijs      (1000) gijs      (1000)        0 2024-05-02 10:39:46.000000 python_snap7-1.4/snap7/py.typed
-drwxrwxr-x   0 gijs      (1000) gijs      (1000)        0 2024-05-03 10:38:25.131252 python_snap7-1.4/snap7/server/
--rw-rw-r--   0 gijs      (1000) gijs      (1000)    16440 2024-05-02 10:39:46.000000 python_snap7-1.4/snap7/server/__init__.py
--rw-rw-r--   0 gijs      (1000) gijs      (1000)     1676 2024-05-02 10:39:46.000000 python_snap7-1.4/snap7/server/__main__.py
--rwxrwxr-x   0 gijs      (1000) gijs      (1000)     8007 2024-05-02 10:39:46.000000 python_snap7-1.4/snap7/types.py
-drwxrwxr-x   0 gijs      (1000) gijs      (1000)        0 2024-05-03 10:38:25.132252 python_snap7-1.4/snap7/util/
--rw-rw-r--   0 gijs      (1000) gijs      (1000)     5809 2024-05-02 10:39:46.000000 python_snap7-1.4/snap7/util/__init__.py
--rw-rw-r--   0 gijs      (1000) gijs      (1000)    21098 2024-05-03 09:44:07.000000 python_snap7-1.4/snap7/util/db.py
--rw-rw-r--   0 gijs      (1000) gijs      (1000)    22786 2024-05-02 10:39:46.000000 python_snap7-1.4/snap7/util/getters.py
--rw-rw-r--   0 gijs      (1000) gijs      (1000)    16703 2024-05-02 10:39:46.000000 python_snap7-1.4/snap7/util/setters.py
-drwxrwxr-x   0 gijs      (1000) gijs      (1000)        0 2024-05-03 10:38:25.132252 python_snap7-1.4/tests/
--rwxrwxr-x   0 gijs      (1000) gijs      (1000)    39525 2024-05-03 10:38:12.000000 python_snap7-1.4/tests/test_client.py
--rw-rw-r--   0 gijs      (1000) gijs      (1000)      755 2024-05-02 10:39:46.000000 python_snap7-1.4/tests/test_common.py
--rw-rw-r--   0 gijs      (1000) gijs      (1000)     3495 2024-05-02 10:39:46.000000 python_snap7-1.4/tests/test_logo_client.py
--rw-rw-r--   0 gijs      (1000) gijs      (1000)     5290 2024-05-02 10:39:46.000000 python_snap7-1.4/tests/test_mainloop.py
--rw-rw-r--   0 gijs      (1000) gijs      (1000)     4275 2024-05-02 10:39:46.000000 python_snap7-1.4/tests/test_partner.py
--rw-rw-r--   0 gijs      (1000) gijs      (1000)     5314 2024-05-03 09:44:07.000000 python_snap7-1.4/tests/test_server.py
--rw-rw-r--   0 gijs      (1000) gijs      (1000)    19902 2024-05-03 09:44:07.000000 python_snap7-1.4/tests/test_util.py
+drwxr-xr-x   0 gijsm      (501) staff       (20)        0 2024-05-10 13:50:03.180111 python_snap7-1.4.1/
+-rw-r--r--   0 gijsm      (501) staff       (20)     1097 2024-05-01 11:02:59.000000 python_snap7-1.4.1/LICENSE
+-rw-r--r--   0 gijsm      (501) staff       (20)       19 2024-05-01 11:02:59.000000 python_snap7-1.4.1/MANIFEST.in
+-rw-r--r--   0 gijsm      (501) staff       (20)     2026 2024-05-10 13:50:03.179888 python_snap7-1.4.1/PKG-INFO
+-rw-r--r--   0 gijsm      (501) staff       (20)      699 2024-05-03 08:38:40.000000 python_snap7-1.4.1/README.rst
+-rw-r--r--   0 gijsm      (501) staff       (20)     1727 2024-05-10 13:49:29.000000 python_snap7-1.4.1/pyproject.toml
+drwxr-xr-x   0 gijsm      (501) staff       (20)        0 2024-05-10 13:50:03.179304 python_snap7-1.4.1/python_snap7.egg-info/
+-rw-r--r--   0 gijsm      (501) staff       (20)     2026 2024-05-10 13:50:03.000000 python_snap7-1.4.1/python_snap7.egg-info/PKG-INFO
+-rw-r--r--   0 gijsm      (501) staff       (20)      705 2024-05-10 13:50:03.000000 python_snap7-1.4.1/python_snap7.egg-info/SOURCES.txt
+-rw-r--r--   0 gijsm      (501) staff       (20)        1 2024-05-10 13:50:03.000000 python_snap7-1.4.1/python_snap7.egg-info/dependency_links.txt
+-rw-r--r--   0 gijsm      (501) staff       (20)       60 2024-05-10 13:50:03.000000 python_snap7-1.4.1/python_snap7.egg-info/entry_points.txt
+-rw-r--r--   0 gijsm      (501) staff       (20)       91 2024-05-10 13:50:03.000000 python_snap7-1.4.1/python_snap7.egg-info/requires.txt
+-rw-r--r--   0 gijsm      (501) staff       (20)        6 2024-05-10 13:50:03.000000 python_snap7-1.4.1/python_snap7.egg-info/top_level.txt
+-rw-r--r--   0 gijsm      (501) staff       (20)       38 2024-05-10 13:50:03.180160 python_snap7-1.4.1/setup.cfg
+drwxr-xr-x   0 gijsm      (501) staff       (20)        0 2024-05-10 13:50:03.171897 python_snap7-1.4.1/snap7/
+-rw-r--r--   0 gijsm      (501) staff       (20)      418 2024-05-02 07:46:59.000000 python_snap7-1.4.1/snap7/__init__.py
+drwxr-xr-x   0 gijsm      (501) staff       (20)        0 2024-05-10 13:50:03.172108 python_snap7-1.4.1/snap7/client/
+-rw-r--r--   0 gijsm      (501) staff       (20)    52893 2024-05-10 13:49:29.000000 python_snap7-1.4.1/snap7/client/__init__.py
+-rw-r--r--   0 gijsm      (501) staff       (20)     3906 2024-05-10 13:49:29.000000 python_snap7-1.4.1/snap7/common.py
+-rw-r--r--   0 gijsm      (501) staff       (20)     3591 2024-05-02 07:46:59.000000 python_snap7-1.4.1/snap7/error.py
+-rw-r--r--   0 gijsm      (501) staff       (20)       81 2024-05-01 11:02:59.000000 python_snap7-1.4.1/snap7/exceptions.py
+-rw-r--r--   0 gijsm      (501) staff       (20)    11808 2024-05-02 07:46:59.000000 python_snap7-1.4.1/snap7/logo.py
+-rw-r--r--   0 gijsm      (501) staff       (20)     7643 2024-05-02 07:46:59.000000 python_snap7-1.4.1/snap7/partner.py
+-rw-r--r--   0 gijsm      (501) staff       (20)        0 2024-05-01 11:02:59.000000 python_snap7-1.4.1/snap7/py.typed
+drwxr-xr-x   0 gijsm      (501) staff       (20)        0 2024-05-10 13:50:03.172425 python_snap7-1.4.1/snap7/server/
+-rw-r--r--   0 gijsm      (501) staff       (20)    16563 2024-05-10 13:49:29.000000 python_snap7-1.4.1/snap7/server/__init__.py
+-rw-r--r--   0 gijsm      (501) staff       (20)     1676 2024-05-02 07:46:59.000000 python_snap7-1.4.1/snap7/server/__main__.py
+-rwxr-xr-x   0 gijsm      (501) staff       (20)     9077 2024-05-10 13:49:29.000000 python_snap7-1.4.1/snap7/types.py
+drwxr-xr-x   0 gijsm      (501) staff       (20)        0 2024-05-10 13:50:03.173503 python_snap7-1.4.1/snap7/util/
+-rw-r--r--   0 gijsm      (501) staff       (20)     5809 2024-05-02 07:46:59.000000 python_snap7-1.4.1/snap7/util/__init__.py
+-rw-r--r--   0 gijsm      (501) staff       (20)    21098 2024-05-02 16:17:13.000000 python_snap7-1.4.1/snap7/util/db.py
+-rw-r--r--   0 gijsm      (501) staff       (20)    22786 2024-05-02 07:46:59.000000 python_snap7-1.4.1/snap7/util/getters.py
+-rw-r--r--   0 gijsm      (501) staff       (20)    16703 2024-05-02 07:57:37.000000 python_snap7-1.4.1/snap7/util/setters.py
+drwxr-xr-x   0 gijsm      (501) staff       (20)        0 2024-05-10 13:50:03.179111 python_snap7-1.4.1/tests/
+-rwxr-xr-x   0 gijsm      (501) staff       (20)    38567 2024-05-10 13:49:29.000000 python_snap7-1.4.1/tests/test_client.py
+-rw-r--r--   0 gijsm      (501) staff       (20)      901 2024-05-10 13:49:29.000000 python_snap7-1.4.1/tests/test_common.py
+-rw-r--r--   0 gijsm      (501) staff       (20)     3495 2024-05-02 07:46:59.000000 python_snap7-1.4.1/tests/test_logo_client.py
+-rw-r--r--   0 gijsm      (501) staff       (20)     5290 2024-05-02 07:46:59.000000 python_snap7-1.4.1/tests/test_mainloop.py
+-rw-r--r--   0 gijsm      (501) staff       (20)     4275 2024-05-02 07:46:59.000000 python_snap7-1.4.1/tests/test_partner.py
+-rw-r--r--   0 gijsm      (501) staff       (20)     5385 2024-05-10 13:49:29.000000 python_snap7-1.4.1/tests/test_server.py
+-rw-r--r--   0 gijsm      (501) staff       (20)    19902 2024-05-02 16:17:13.000000 python_snap7-1.4.1/tests/test_util.py
```

### Comparing `python_snap7-1.4/LICENSE` & `python_snap7-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_snap7-1.4/README.rst` & `python_snap7-1.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `python_snap7-1.4/pyproject.toml` & `python_snap7-1.4.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 [build-system]
 requires = ["setuptools>=68.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-snap7"
-version = "1.4"
+version = "1.4.1"
 description = "Python wrapper for the snap7 library"
+readme = "README.rst"
 authors = [
     {name = "Gijs Molenaar", email = "gijsmolenaar@gmail.com"},
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Topic :: System :: Hardware",
     "Intended Audience :: Developers",
     "Intended Audience :: Manufacturing",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
-license = {text = "MIT"}
-requires-python = ">=3.8"
+license = {text = "MIT License"}
+requires-python = ">=3.9"
+keywords = ["snap7", "s7", "siemens", "plc"]
 
 [project.urls]
 Homepage = "https://github.com/gijzelaerr/python-snap7"
 Documentation = "https://python-snap7.readthedocs.io/en/latest/"
 
 [project.optional-dependencies]
 test = ["pytest", "mypy", "types-setuptools", "ruff"]
@@ -58,12 +59,12 @@
 
 [tool.mypy]
 ignore_missing_imports = true
 
 [tool.ruff]
 output-format = "full"
 line-length = 130
-target-version = "py38"
+target-version = "py39"
 
 [lint]
 ignore = []
 mccabe.max-complexity = 10
```

### Comparing `python_snap7-1.4/python_snap7.egg-info/SOURCES.txt` & `python_snap7-1.4.1/python_snap7.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python_snap7-1.4/snap7/client/__init__.py` & `python_snap7-1.4.1/snap7/client/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,100 +43,109 @@
         bytearray(b"\\x00\\x00\\x00\\x00")
         >>> data[3] = 0b00000001
         >>> data
         bytearray(b'\\x00\\x00\\x00\\x01')
         >>> client.db_write(1, 0, data)
     """
 
+    _lib: Any  # since this is dynamically loaded from a DLL we don't have the type signature.
+    _read_callback = None
+    _callback = None
+    _s7_client: Optional[S7Object] = None
+
     def __init__(self, lib_location: Optional[str] = None):
         """Creates a new `Client` instance.
 
         Args:
             lib_location: Full path to the snap7.dll file. Optional.
 
         Examples:
             >>> import snap7
             >>> client = snap7.client.Client()  # If the `snap7.dll` file is in the path location
             >>> client = snap7.client.Client(lib_location="/path/to/snap7.dll")  # If the `snap7.dll` file is in another location
             >>> client
             <snap7.client.Client object at 0x0000028B257128E0>
         """
-        self._read_callback = None
-        self._callback = None
-        self._pointer = None
-        self._library = load_library(lib_location)
+
+        self._lib = load_library(lib_location)
         self.create()
 
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.destroy()
+
     def __del__(self):
         self.destroy()
 
     def create(self):
         """Creates a SNAP7 client."""
         logger.info("creating snap7 client")
-        self._library.Cli_Create.restype = c_void_p
-        self._pointer = S7Object(self._library.Cli_Create())
+        self._lib.Cli_Create.restype = S7Object
+        self._s7_client = S7Object(self._lib.Cli_Create())
 
     def destroy(self) -> Optional[int]:
         """Destroys the Client object.
 
         Returns:
             Error code from snap7 library.
 
         Examples:
             >>> client.destroy()
             640719840
         """
         logger.info("destroying snap7 client")
-        if self._pointer:
-            return self._library.Cli_Destroy(byref(self._pointer))
-        self._pointer = None
+        if self._lib and self._s7_client is not None:
+            return self._lib.Cli_Destroy(byref(self._s7_client))
+        self._s7_client = None
         return None
 
     def plc_stop(self) -> int:
         """Puts the CPU in STOP mode
 
         Returns:
             Error code from snap7 library.
         """
         logger.info("stopping plc")
-        return self._library.Cli_PlcStop(self._pointer)
+        return self._lib.Cli_PlcStop(self._s7_client)
 
     def plc_cold_start(self) -> int:
         """Puts the CPU in RUN mode performing a COLD START.
 
         Returns:
             Error code from snap7 library.
         """
         logger.info("cold starting plc")
-        return self._library.Cli_PlcColdStart(self._pointer)
+        return self._lib.Cli_PlcColdStart(self._s7_client)
 
     def plc_hot_start(self) -> int:
         """Puts the CPU in RUN mode performing an HOT START.
 
         Returns:
             Error code from snap7 library.
         """
         logger.info("hot starting plc")
-        return self._library.Cli_PlcHotStart(self._pointer)
+        return self._lib.Cli_PlcHotStart(self._s7_client)
 
     def get_cpu_state(self) -> str:
         """Returns the CPU status (running/stopped)
 
         Returns:
             Description of the cpu state.
 
         Raises:
             :obj:`ValueError`: if the cpu state is invalid.
 
         Examples:
-            >>> client.get_cpu_statE()
+            >>> client.get_cpu_state()
             'S7CpuStatusRun'
         """
         state = c_int(0)
-        self._library.Cli_GetPlcStatus(self._pointer, byref(state))
+        self._lib.Cli_GetPlcStatus(self._s7_client, byref(state))
         try:
             status_string = cpu_statuses[state.value]
         except KeyError:
             raise ValueError(f"The cpu state ({state.value}) is invalid")
 
         logger.debug(f"CPU state is {status_string}")
         return status_string
@@ -152,27 +161,27 @@
             >>> print(cpu_info)
             "<S7CpuInfo ModuleTypeName: b'CPU 315-2 PN/DP'
                 SerialNumber: b'S C-C2UR28922012'
                 ASName: b'SNAP7-SERVER' Copyright: b'Original Siemens Equipment'
                 ModuleName: b'CPU 315-2 PN/DP'>
         """
         info = S7CpuInfo()
-        result = self._library.Cli_GetCpuInfo(self._pointer, byref(info))
+        result = self._lib.Cli_GetCpuInfo(self._s7_client, byref(info))
         check_error(result, context="client")
         return info
 
     @error_wrap
     def disconnect(self) -> int:
         """Disconnect a client.
 
         Returns:
             Error code from snap7 library.
         """
         logger.info("disconnecting snap7 client")
-        return self._library.Cli_Disconnect(self._pointer)
+        return self._lib.Cli_Disconnect(self._s7_client)
 
     @error_wrap
     def connect(self, address: str, rack: int, slot: int, tcpport: int = 102) -> int:
         """Connects a Client Object to a PLC.
 
         Args:
             address: IP address of the PLC.
@@ -187,15 +196,15 @@
             >>> import snap7
             >>> client = snap7.client.Client()
             >>> client.connect("192.168.0.1", 0, 0)  # port is implicit = 102.
         """
         logger.info(f"connecting to {address}:{tcpport} rack {rack} slot {slot}")
 
         self.set_param(RemotePort, tcpport)
-        return self._library.Cli_ConnectTo(self._pointer, c_char_p(address.encode()), c_int(rack), c_int(slot))
+        return self._lib.Cli_ConnectTo(self._s7_client, c_char_p(address.encode()), c_int(rack), c_int(slot))
 
     def db_read(self, db_number: int, start: int, size: int) -> bytearray:
         """Reads a part of a DB from a PLC
 
         Note:
             Use it only for reading DBs, not Marks, Inputs, Outputs.
 
@@ -215,15 +224,15 @@
             >>> buffer
             bytearray(b'\\x00\\x00')
         """
         logger.debug(f"db_read, db_number:{db_number}, start:{start}, size:{size}")
 
         type_ = wordlen_to_ctypes[WordLen.Byte.value]
         data = (type_ * size)()
-        result = self._library.Cli_DBRead(self._pointer, db_number, start, size, byref(data))
+        result = self._lib.Cli_DBRead(self._s7_client, db_number, start, size, byref(data))
         check_error(result, context="client")
         return bytearray(data)
 
     @error_wrap
     def db_write(self, db_number: int, start: int, data: bytearray) -> int:
         """Writes a part of a DB into a PLC.
 
@@ -243,29 +252,29 @@
             >>> client.db_write(1, 10, buffer)  # writes the bit number 0 from the byte 10 to TRUE.
         """
         wordlen = WordLen.Byte
         type_ = wordlen_to_ctypes[wordlen.value]
         size = len(data)
         cdata = (type_ * size).from_buffer_copy(data)
         logger.debug(f"db_write db_number:{db_number} start:{start} size:{size} data:{data}")
-        return self._library.Cli_DBWrite(self._pointer, db_number, start, size, byref(cdata))
+        return self._lib.Cli_DBWrite(self._s7_client, db_number, start, size, byref(cdata))
 
     def delete(self, block_type: str, block_num: int) -> int:
         """Delete a block into AG.
 
         Args:
             block_type: type of block.
             block_num: block number.
 
         Returns:
             Error code from snap7 library.
         """
         logger.info("deleting block")
         blocktype = block_types[block_type]
-        result = self._library.Cli_Delete(self._pointer, blocktype, block_num)
+        result = self._lib.Cli_Delete(self._s7_client, blocktype, block_num)
         return result
 
     def full_upload(self, _type: str, block_num: int) -> Tuple[bytearray, int]:
         """Uploads a block from AG with Header and Footer infos.
         The whole block (including header and footer) is copied into the user
         buffer.
 
@@ -275,15 +284,15 @@
 
         Returns:
             Tuple of the buffer and size.
         """
         _buffer = buffer_type()
         size = c_int(sizeof(_buffer))
         block_type = block_types[_type]
-        result = self._library.Cli_FullUpload(self._pointer, block_type, block_num, byref(_buffer), byref(size))
+        result = self._lib.Cli_FullUpload(self._s7_client, block_type, block_num, byref(_buffer), byref(size))
         check_error(result, context="client")
         return bytearray(_buffer)[: size.value], size.value
 
     def upload(self, block_num: int) -> bytearray:
         """Uploads a block from AG.
 
         Note:
@@ -296,15 +305,15 @@
             Buffer with the uploaded block.
         """
         logger.debug(f"db_upload block_num: {block_num}")
         block_type = block_types["DB"]
         _buffer = buffer_type()
         size = c_int(sizeof(_buffer))
 
-        result = self._library.Cli_Upload(self._pointer, block_type, block_num, byref(_buffer), byref(size))
+        result = self._lib.Cli_Upload(self._s7_client, block_type, block_num, byref(_buffer), byref(size))
 
         check_error(result, context="client")
         logger.info(f"received {size} bytes")
         return bytearray(_buffer)
 
     @error_wrap
     def download(self, data: bytearray, block_num: int = -1) -> int:
@@ -321,15 +330,15 @@
 
         Returns:
             Error code from snap7 library.
         """
         type_ = c_byte
         size = len(data)
         cdata = (type_ * len(data)).from_buffer_copy(data)
-        return self._library.Cli_Download(self._pointer, block_num, byref(cdata), size)
+        return self._lib.Cli_Download(self._s7_client, block_num, byref(cdata), size)
 
     def db_get(self, db_number: int) -> bytearray:
         """Uploads a DB from AG using DBRead.
 
         Note:
             This method can't be use for 1200/1500 PLCs.
 
@@ -345,15 +354,15 @@
             >>> client.connect("192.168.0.1", 0, 0)
             >>> buffer = client.db_get(1)  # reads the db number 1.
             >>> buffer
             bytearray(b"\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00...<truncated>\\x00\\x00")
         """
         logger.debug(f"db_get db_number: {db_number}")
         _buffer = buffer_type()
-        result = self._library.Cli_DBGet(self._pointer, db_number, byref(_buffer), byref(c_int(buffer_size)))
+        result = self._lib.Cli_DBGet(self._s7_client, db_number, byref(_buffer), byref(c_int(buffer_size)))
         check_error(result, context="client")
         return bytearray(_buffer)
 
     def read_area(self, area: Areas, dbnumber: int, start: int, size: int) -> bytearray:
         """Reads a data area from a PLC
                 With it you can read DB, Inputs, Outputs, Merkers, Timers and Counters.
 
@@ -387,15 +396,15 @@
             wordlen = WordLen.Byte
         type_ = wordlen_to_ctypes[wordlen.value]
         logger.debug(
             f"reading area: {area.name} dbnumber: {dbnumber} start: {start} amount: {size} "
             f"wordlen: {wordlen.name}={wordlen.value}"
         )
         data = (type_ * size)()
-        result = self._library.Cli_ReadArea(self._pointer, area.value, dbnumber, start, size, wordlen.value, byref(data))
+        result = self._lib.Cli_ReadArea(self._s7_client, area.value, dbnumber, start, size, wordlen.value, byref(data))
         check_error(result, context="client")
         return bytearray(data)
 
     @error_wrap
     def write_area(self, area: Areas, dbnumber: int, start: int, data: bytearray) -> int:
         """Writes a data area into a PLC.
 
@@ -426,26 +435,26 @@
         type_ = wordlen_to_ctypes[WordLen.Byte.value]
         size = len(data)
         logger.debug(
             f"writing area: {area.name} dbnumber: {dbnumber} start: {start}: size {size}: "
             f"wordlen {wordlen.name}={wordlen.value} type: {type_}"
         )
         cdata = (type_ * len(data)).from_buffer_copy(data)
-        return self._library.Cli_WriteArea(self._pointer, area.value, dbnumber, start, size, wordlen.value, byref(cdata))
+        return self._lib.Cli_WriteArea(self._s7_client, area.value, dbnumber, start, size, wordlen.value, byref(cdata))
 
     def read_multi_vars(self, items) -> Tuple[int, S7DataItem]:
         """Reads different kind of variables from a PLC simultaneously.
 
         Args:
             items: list of items to be read.
 
         Returns:
             Tuple with the return code from the snap7 library and the list of items.
         """
-        result = self._library.Cli_ReadMultiVars(self._pointer, byref(items), c_int32(len(items)))
+        result = self._lib.Cli_ReadMultiVars(self._s7_client, byref(items), c_int32(len(items)))
         check_error(result, context="client")
         return result, items
 
     def list_blocks(self) -> BlocksList:
         """Returns the AG blocks amount divided by type.
 
         Returns:
@@ -454,15 +463,15 @@
         Examples:
             >>> block_list = client.list_blocks()
             >>> print(block_list)
             <block list count OB: 0 FB: 0 FC: 0 SFB: 0 SFC: 0x0 DB: 1 SDB: 0>
         """
         logger.debug("listing blocks")
         blocksList = BlocksList()
-        result = self._library.Cli_ListBlocks(self._pointer, byref(blocksList))
+        result = self._lib.Cli_ListBlocks(self._s7_client, byref(blocksList))
         check_error(result, context="client")
         logger.debug(f"blocks: {blocksList}")
         return blocksList
 
     def list_blocks_of_type(self, blocktype: str, size: int) -> Union[int, Array]:
         """This function returns the AG list of a specified block type.
 
@@ -484,15 +493,15 @@
         logger.debug(f"listing blocks of type: {_blocktype} size: {size}")
 
         if size == 0:
             return 0
 
         data = (c_uint16 * size)()
         count = c_int(size)
-        result = self._library.Cli_ListBlocksOfType(self._pointer, _blocktype, byref(data), byref(count))
+        result = self._lib.Cli_ListBlocksOfType(self._s7_client, _blocktype, byref(data), byref(count))
 
         logger.debug(f"number of items found: {count}")
 
         check_error(result, context="client")
         return data
 
     def get_block_info(self, blocktype: str, db_number: int) -> TS7BlockInfo:
@@ -531,15 +540,15 @@
 
         if not blocktype_:
             raise ValueError("The blocktype parameter was invalid")
         logger.debug(f"retrieving block info for block {db_number} of type {blocktype_}")
 
         data = TS7BlockInfo()
 
-        result = self._library.Cli_GetAgBlockInfo(self._pointer, blocktype_, db_number, byref(data))
+        result = self._lib.Cli_GetAgBlockInfo(self._s7_client, blocktype_, db_number, byref(data))
         check_error(result, context="client")
         return data
 
     @error_wrap
     def set_session_password(self, password: str) -> int:
         """Send the password to the PLC to meet its security level.
 
@@ -550,24 +559,24 @@
             Snap7 code.
 
         Raises:
             :obj:`ValueError`: if the length of the `password` is more than 8 characters.
         """
         if len(password) > 8:
             raise ValueError("Maximum password length is 8")
-        return self._library.Cli_SetSessionPassword(self._pointer, c_char_p(password.encode()))
+        return self._lib.Cli_SetSessionPassword(self._s7_client, c_char_p(password.encode()))
 
     @error_wrap
     def clear_session_password(self) -> int:
         """Clears the password set for the current session (logout).
 
         Returns:
             Snap7 code.
         """
-        return self._library.Cli_ClearSessionPassword(self._pointer)
+        return self._lib.Cli_ClearSessionPassword(self._s7_client)
 
     def set_connection_params(self, address: str, local_tsap: int, remote_tsap: int) -> None:
         """Sets internally (IP, LocalTSAP, RemoteTSAP) Coordinates.
 
         Note:
             This function must be called just before `Cli_Connect()`.
 
@@ -579,43 +588,43 @@
         Raises:
             :obj:`ValueError`: if the `address` is not a valid IPV4.
             :obj:`ValueError`: if the result of setting the connection params is
                 different than 0.
         """
         if not re.match(ipv4, address):
             raise ValueError(f"{address} is invalid ipv4")
-        result = self._library.Cli_SetConnectionParams(self._pointer, address, c_uint16(local_tsap), c_uint16(remote_tsap))
+        result = self._lib.Cli_SetConnectionParams(self._s7_client, address, c_uint16(local_tsap), c_uint16(remote_tsap))
         if result != 0:
             raise ValueError("The parameter was invalid")
 
     def set_connection_type(self, connection_type: int):
         """Sets the connection resource type, i.e the way in which the Clients connects to a PLC.
 
         Args:
             connection_type: 1 for PG, 2 for OP, 3 to 10 for S7 Basic
 
         Raises:
             :obj:`ValueError`: if the result of setting the connection type is
                 different than 0.
         """
-        result = self._library.Cli_SetConnectionType(self._pointer, c_uint16(connection_type))
+        result = self._lib.Cli_SetConnectionType(self._s7_client, c_uint16(connection_type))
         if result != 0:
             raise ValueError("The parameter was invalid")
 
     def get_connected(self) -> bool:
         """Returns the connection status
 
         Note:
             Sometimes returns True, while connection is lost.
 
         Returns:
             True if is connected, otherwise false.
         """
         connected = c_int32()
-        result = self._library.Cli_GetConnected(self._pointer, byref(connected))
+        result = self._lib.Cli_GetConnected(self._s7_client, byref(connected))
         check_error(result, context="client")
         return bool(connected)
 
     def ab_read(self, start: int, size: int) -> bytearray:
         """Reads a part of IPU area from a PLC.
 
         Args:
@@ -625,15 +634,15 @@
         Returns:
             Buffer with the data read.
         """
         wordlen = WordLen.Byte
         type_ = wordlen_to_ctypes[wordlen.value]
         data = (type_ * size)()
         logger.debug(f"ab_read: start: {start}: size {size}: ")
-        result = self._library.Cli_ABRead(self._pointer, start, size, byref(data))
+        result = self._lib.Cli_ABRead(self._s7_client, start, size, byref(data))
         check_error(result, context="client")
         return bytearray(data)
 
     def ab_write(self, start: int, data: bytearray) -> int:
         """Writes a part of IPU area into a PLC.
 
         Args:
@@ -644,29 +653,29 @@
             Snap7 code.
         """
         wordlen = WordLen.Byte
         type_ = wordlen_to_ctypes[wordlen.value]
         size = len(data)
         cdata = (type_ * size).from_buffer_copy(data)
         logger.debug(f"ab write: start: {start}: size: {size}: ")
-        return self._library.Cli_ABWrite(self._pointer, start, size, byref(cdata))
+        return self._lib.Cli_ABWrite(self._s7_client, start, size, byref(cdata))
 
     def as_ab_read(self, start: int, size: int, data) -> int:
         """Reads a part of IPU area from a PLC asynchronously.
 
         Args:
             start: byte index from where start to read.
             size: amount of bytes to read.
             data: buffer where the data will be place.
 
         Returns:
             Snap7 code.
         """
         logger.debug(f"ab_read: start: {start}: size {size}: ")
-        result = self._library.Cli_AsABRead(self._pointer, start, size, byref(data))
+        result = self._lib.Cli_AsABRead(self._s7_client, start, size, byref(data))
         check_error(result, context="client")
         return result
 
     def as_ab_write(self, start: int, data: bytearray) -> int:
         """Writes a part of IPU area into a PLC asynchronously.
 
         Args:
@@ -677,56 +686,56 @@
             Snap7 code.
         """
         wordlen = WordLen.Byte
         type_ = wordlen_to_ctypes[wordlen.value]
         size = len(data)
         cdata = (type_ * size).from_buffer_copy(data)
         logger.debug(f"ab write: start: {start}: size: {size}: ")
-        result = self._library.Cli_AsABWrite(self._pointer, start, size, byref(cdata))
+        result = self._lib.Cli_AsABWrite(self._s7_client, start, size, byref(cdata))
         check_error(result, context="client")
         return result
 
     def as_compress(self, time: int) -> int:
         """Performs the Compress action asynchronously.
 
         Args:
             time: timeout.
 
         Returns:
             Snap7 code.
         """
-        result = self._library.Cli_AsCompress(self._pointer, time)
+        result = self._lib.Cli_AsCompress(self._s7_client, time)
         check_error(result, context="client")
         return result
 
     def as_copy_ram_to_rom(self, timeout: int = 1) -> int:
         """Performs the Copy Ram to Rom action asynchronously.
 
         Args:
             timeout: time to wait unly fail.
 
         Returns:
             Snap7 code.
         """
-        result = self._library.Cli_AsCopyRamToRom(self._pointer, timeout)
+        result = self._lib.Cli_AsCopyRamToRom(self._s7_client, timeout)
         check_error(result, context="client")
         return result
 
     def as_ct_read(self, start: int, amount: int, data) -> int:
         """Reads counters from a PLC asynchronously.
 
         Args:
             start: byte index to start to read from.
             amount: amount of bytes to read.
             data: buffer where the value read will be place.
 
         Returns:
             Snap7 code.
         """
-        result = self._library.Cli_AsCTRead(self._pointer, start, amount, byref(data))
+        result = self._lib.Cli_AsCTRead(self._s7_client, start, amount, byref(data))
         check_error(result, context="client")
         return result
 
     def as_ct_write(self, start: int, amount: int, data: bytearray) -> int:
         """Write counters into a PLC.
 
         Args:
@@ -735,29 +744,29 @@
             data: buffer to be write.
 
         Returns:
             Snap7 code.
         """
         type_ = wordlen_to_ctypes[WordLen.Counter.value]
         cdata = (type_ * amount).from_buffer_copy(data)
-        result = self._library.Cli_AsCTWrite(self._pointer, start, amount, byref(cdata))
+        result = self._lib.Cli_AsCTWrite(self._s7_client, start, amount, byref(cdata))
         check_error(result, context="client")
         return result
 
     def as_db_fill(self, db_number: int, filler) -> int:
         """Fills a DB in AG with a given byte.
 
         Args:
             db_number: number of DB to fill.
             filler: buffer to fill with.
 
         Returns:
             Snap7 code.
         """
-        result = self._library.Cli_AsDBFill(self._pointer, db_number, filler)
+        result = self._lib.Cli_AsDBFill(self._s7_client, db_number, filler)
         check_error(result, context="client")
         return result
 
     def as_db_get(self, db_number: int, _buffer, size) -> bytearray:
         """Uploads a DB from AG using DBRead.
 
         Note:
@@ -767,15 +776,15 @@
             db_number: number of DB to get.
             _buffer: buffer where the data read will be place.
             size: amount of bytes to be read.
 
         Returns:
             Snap7 code.
         """
-        result = self._library.Cli_AsDBGet(self._pointer, db_number, byref(_buffer), byref(size))
+        result = self._lib.Cli_AsDBGet(self._s7_client, db_number, byref(_buffer), byref(size))
         check_error(result, context="client")
         return result
 
     def as_db_read(self, db_number: int, start: int, size: int, data) -> Array:
         """Reads a part of a DB from a PLC.
 
         Args:
@@ -790,15 +799,15 @@
         Examples:
             >>> import ctypes
             >>> data = (ctypes.c_uint8 * size_to_read)()  # In this ctypes array data will be stored.
             >>> result = client.as_db_read(1, 0, size_to_read, data)
             >>> result  # 0 = success
             0
         """
-        result = self._library.Cli_AsDBRead(self._pointer, db_number, start, size, byref(data))
+        result = self._lib.Cli_AsDBRead(self._s7_client, db_number, start, size, byref(data))
         check_error(result, context="client")
         return result
 
     def as_db_write(self, db_number: int, start: int, size: int, data) -> int:
         """Writes a part of a DB into a PLC.
 
         Args:
@@ -806,15 +815,15 @@
             start: byte index from where start to write to.
             size: amount of bytes to write.
             data: buffer to be write.
 
         Returns:
             Snap7 code.
         """
-        result = self._library.Cli_AsDBWrite(self._pointer, db_number, start, size, byref(data))
+        result = self._lib.Cli_AsDBWrite(self._s7_client, db_number, start, size, byref(data))
         check_error(result, context="client")
         return result
 
     def as_download(self, data: bytearray, block_num: int) -> int:
         """Download a block into AG asynchronously.
 
         Note:
@@ -826,58 +835,58 @@
 
         Returns:
             Snap7 code.
         """
         size = len(data)
         type_ = c_byte * len(data)
         cdata = type_.from_buffer_copy(data)
-        result = self._library.Cli_AsDownload(self._pointer, block_num, byref(cdata), size)
+        result = self._lib.Cli_AsDownload(self._s7_client, block_num, byref(cdata), size)
         check_error(result)
         return result
 
     @error_wrap
     def compress(self, time: int) -> int:
         """Performs the Compress action.
 
         Args:
             time: timeout.
 
         Returns:
             Snap7 code.
         """
-        return self._library.Cli_Compress(self._pointer, time)
+        return self._lib.Cli_Compress(self._s7_client, time)
 
     @error_wrap
     def set_param(self, number: int, value: int) -> int:
         """Writes an internal Server Parameter.
 
         Args:
             number: number of argument to be written.
             value: value to be written.
 
         Returns:
             Snap7 code.
         """
         logger.debug(f"setting param number {number} to {value}")
         type_ = param_types[number]
-        return self._library.Cli_SetParam(self._pointer, number, byref(type_(value)))
+        return self._lib.Cli_SetParam(self._s7_client, number, byref(type_(value)))
 
     def get_param(self, number: int) -> int:
         """Reads an internal Server parameter.
 
         Args:
             number: number of argument to be read.
 
         Return:
             Value of the param read.
         """
         logger.debug(f"retreiving param number {number}")
         type_ = param_types[number]
         value = type_()
-        code = self._library.Cli_GetParam(self._pointer, c_int(number), byref(value))
+        code = self._lib.Cli_GetParam(self._s7_client, c_int(number), byref(value))
         check_error(code)
         return value.value
 
     def get_pdu_length(self) -> int:
         """Returns info about the PDU length (requested and negotiated).
 
         Returns:
@@ -886,15 +895,15 @@
         Examples:
             >>> client.get_pdu_length()
             480
         """
         logger.info("getting PDU length")
         requested_ = c_uint16()
         negotiated_ = c_uint16()
-        code = self._library.Cli_GetPduLength(self._pointer, byref(requested_), byref(negotiated_))
+        code = self._lib.Cli_GetPduLength(self._s7_client, byref(requested_), byref(negotiated_))
         check_error(code)
         return negotiated_.value
 
     def get_plc_datetime(self) -> datetime:
         """Returns the PLC date/time.
 
         Returns:
@@ -902,15 +911,15 @@
 
         Examples:
             >>> client.get_plc_datetime()
             datetime.datetime(2021, 4, 6, 12, 12, 36)
         """
         type_ = c_int32
         buffer = (type_ * 9)()
-        result = self._library.Cli_GetPlcDateTime(self._pointer, byref(buffer))
+        result = self._lib.Cli_GetPlcDateTime(self._s7_client, byref(buffer))
         check_error(result, context="client")
 
         return datetime(
             year=buffer[5] + 1900, month=buffer[4] + 1, day=buffer[3], hour=buffer[2], minute=buffer[1], second=buffer[0]
         )
 
     @error_wrap
@@ -928,30 +937,34 @@
         buffer[0] = dt.second
         buffer[1] = dt.minute
         buffer[2] = dt.hour
         buffer[3] = dt.day
         buffer[4] = dt.month - 1
         buffer[5] = dt.year - 1900
 
-        return self._library.Cli_SetPlcDateTime(self._pointer, byref(buffer))
+        return self._lib.Cli_SetPlcDateTime(self._s7_client, byref(buffer))
 
     def check_as_completion(self, p_value) -> int:
         """Method to check Status of an async request. Result contains if the check was successful, not the data value itself
 
         Args:
             p_value: Pointer where result of this check shall be written.
 
         Returns:
             Snap7 code. If 0 - Job is done successfully. If 1 - Job is either pending or contains s7errors
         """
-        result = self._library.Cli_CheckAsCompletion(self._pointer, p_value)
+        result = self._lib.Cli_CheckAsCompletion(self._s7_client, p_value)
         check_error(result, context="client")
         return result
 
     def set_as_callback(self, call_back: Callable[..., Any]) -> int:
+        """
+        Sets the user callback that is called when a asynchronous data sent is complete.
+
+        """
         logger.info("setting event callback")
         callback_wrap: Callable[..., Any] = CFUNCTYPE(None, c_void_p, c_int, c_int)
 
         def wrapper(usrptr: Optional[c_void_p], op_code: int, op_result: int) -> int:
             """Wraps python function into a ctypes function
 
             Args:
@@ -965,29 +978,29 @@
             logger.info(f"callback event: op_code: {op_code} op_result: {op_result}")
             call_back(op_code, op_result)
             return 0
 
         self._callback = callback_wrap(wrapper)
         usrPtr = c_void_p()
 
-        result = self._library.Cli_SetAsCallback(self._pointer, self._callback, usrPtr)
+        result = self._lib.Cli_SetAsCallback(self._s7_client, self._callback, usrPtr)
         check_error(result, context="client")
         return result
 
     def wait_as_completion(self, timeout: int) -> int:
         """Snap7 Cli_WaitAsCompletion representative.
 
         Args:
             timeout: ms to wait for async job
 
         Returns:
             Snap7 code.
         """
         # Cli_WaitAsCompletion
-        result = self._library.Cli_WaitAsCompletion(self._pointer, c_ulong(timeout))
+        result = self._lib.Cli_WaitAsCompletion(self._s7_client, c_ulong(timeout))
         check_error(result, context="client")
         return result
 
     def _prepare_as_read_area(self, area: Areas, size: int) -> Tuple[WordLen, Array]:
         if area not in Areas:
             raise ValueError(f"{area} is not implemented in types")
         elif area == Areas.TM:
@@ -1015,15 +1028,15 @@
         Returns:
             Snap7 code.
         """
         logger.debug(
             f"reading area: {area.name} dbnumber: {dbnumber} start: {start} amount: {size} "
             f"wordlen: {wordlen.name}={wordlen.value}"
         )
-        result = self._library.Cli_AsReadArea(self._pointer, area.value, dbnumber, start, size, wordlen.value, pusrdata)
+        result = self._lib.Cli_AsReadArea(self._s7_client, area.value, dbnumber, start, size, wordlen.value, pusrdata)
         check_error(result, context="client")
         return result
 
     def _prepare_as_write_area(self, area: Areas, data: bytearray) -> Tuple[WordLen, Array]:
         if area not in Areas:
             raise ValueError(f"{area} is not implemented in types")
         elif area == Areas.TM:
@@ -1051,30 +1064,30 @@
             Snap7 code.
         """
         type_ = wordlen_to_ctypes[WordLen.Byte.value]
         logger.debug(
             f"writing area: {area.name} dbnumber: {dbnumber} start: {start}: size {size}: " f"wordlen {wordlen} type: {type_}"
         )
         cdata = (type_ * len(pusrdata)).from_buffer_copy(pusrdata)
-        res = self._library.Cli_AsWriteArea(self._pointer, area.value, dbnumber, start, size, wordlen.value, byref(cdata))
+        res = self._lib.Cli_AsWriteArea(self._s7_client, area.value, dbnumber, start, size, wordlen.value, byref(cdata))
         check_error(res, context="client")
         return res
 
     def as_eb_read(self, start: int, size: int, data) -> int:
         """Reads a part of IPI area from a PLC asynchronously.
 
         Args:
             start: byte index from where to start reading from.
             size: amount of bytes to read.
             data: buffer where the data read will be place.
 
         Returns:
             Snap7 code.
         """
-        result = self._library.Cli_AsEBRead(self._pointer, start, size, byref(data))
+        result = self._lib.Cli_AsEBRead(self._s7_client, start, size, byref(data))
         check_error(result, context="client")
         return result
 
     def as_eb_write(self, start: int, size: int, data: bytearray) -> int:
         """Writes a part of IPI area into a PLC.
 
         Args:
@@ -1083,15 +1096,15 @@
             data: buffer to write.
 
         Returns:
             Snap7 code.
         """
         type_ = wordlen_to_ctypes[WordLen.Byte.value]
         cdata = (type_ * size).from_buffer_copy(data)
-        result = self._library.Cli_AsEBWrite(self._pointer, start, size, byref(cdata))
+        result = self._lib.Cli_AsEBWrite(self._s7_client, start, size, byref(cdata))
         check_error(result, context="client")
         return result
 
     def as_full_upload(self, _type: str, block_num: int) -> int:
         """Uploads a block from AG with Header and Footer infos.
 
         Note:
@@ -1103,15 +1116,15 @@
 
         Returns:
             Snap7 code.
         """
         _buffer = buffer_type()
         size = c_int(sizeof(_buffer))
         block_type = block_types[_type]
-        result = self._library.Cli_AsFullUpload(self._pointer, block_type, block_num, byref(_buffer), byref(size))
+        result = self._lib.Cli_AsFullUpload(self._s7_client, block_type, block_num, byref(_buffer), byref(size))
         check_error(result, context="client")
         return result
 
     def as_list_blocks_of_type(self, blocktype: str, data, count) -> int:
         """Returns the AG blocks list of a given type.
 
         Args:
@@ -1124,30 +1137,30 @@
 
         Raises:
             :obj:`ValueError`: if the `blocktype` is invalid
         """
         _blocktype = block_types.get(blocktype)
         if not _blocktype:
             raise ValueError("The blocktype parameter was invalid")
-        result = self._library.Cli_AsListBlocksOfType(self._pointer, _blocktype, byref(data), byref(count))
+        result = self._lib.Cli_AsListBlocksOfType(self._s7_client, _blocktype, byref(data), byref(count))
         check_error(result, context="client")
         return result
 
     def as_mb_read(self, start: int, size: int, data) -> int:
         """Reads a part of Merkers area from a PLC.
 
         Args:
             start: byte index from where to start to read from.
             size: amount of byte to read.
             data: buffer where the data read will be place.
 
         Returns:
             Snap7 code.
         """
-        result = self._library.Cli_AsMBRead(self._pointer, start, size, byref(data))
+        result = self._lib.Cli_AsMBRead(self._s7_client, start, size, byref(data))
         check_error(result, context="client")
         return result
 
     def as_mb_write(self, start: int, size: int, data: bytearray) -> int:
         """Writes a part of Merkers area into a PLC.
 
         Args:
@@ -1156,15 +1169,15 @@
             data: buffer to write.
 
         Returns:
             Snap7 code.
         """
         type_ = wordlen_to_ctypes[WordLen.Byte.value]
         cdata = (type_ * size).from_buffer_copy(data)
-        result = self._library.Cli_AsMBWrite(self._pointer, start, size, byref(cdata))
+        result = self._lib.Cli_AsMBWrite(self._s7_client, start, size, byref(cdata))
         check_error(result, context="client")
         return result
 
     def as_read_szl(self, ssl_id: int, index: int, s7_szl: S7SZL, size) -> int:
         """Reads a partial list of given ID and Index.
 
         Args:
@@ -1172,44 +1185,44 @@
             index: TODO
             s7_szl: TODO
             size: TODO
 
         Returns:
             Snap7 code.
         """
-        result = self._library.Cli_AsReadSZL(self._pointer, ssl_id, index, byref(s7_szl), byref(size))
+        result = self._lib.Cli_AsReadSZL(self._s7_client, ssl_id, index, byref(s7_szl), byref(size))
         check_error(result, context="client")
         return result
 
     def as_read_szl_list(self, szl_list, items_count) -> int:
         """Reads the list of partial lists available in the CPU.
 
         Args:
             szl_list: TODO
             items_count: TODO
 
         Returns:
             Snap7 code.
         """
-        result = self._library.Cli_AsReadSZLList(self._pointer, byref(szl_list), byref(items_count))
+        result = self._lib.Cli_AsReadSZLList(self._s7_client, byref(szl_list), byref(items_count))
         check_error(result, context="client")
         return result
 
     def as_tm_read(self, start: int, amount: int, data) -> bytearray:
         """Reads timers from a PLC.
 
         Args:
             start: byte index to start read from.
             amount: amount of bytes to read.
             data: buffer where the data will be placed.
 
         Returns:
             Snap7 code.
         """
-        result = self._library.Cli_AsTMRead(self._pointer, start, amount, byref(data))
+        result = self._lib.Cli_AsTMRead(self._s7_client, start, amount, byref(data))
         check_error(result, context="client")
         return result
 
     def as_tm_write(self, start: int, amount: int, data: bytearray) -> int:
         """Write timers into a PLC.
 
         Args:
@@ -1218,15 +1231,15 @@
             data: buffer to write.
 
         Returns:
             Snap7 code.
         """
         type_ = wordlen_to_ctypes[WordLen.Timer.value]
         cdata = (type_ * amount).from_buffer_copy(data)
-        result = self._library.Cli_AsTMWrite(self._pointer, start, amount, byref(cdata))
+        result = self._lib.Cli_AsTMWrite(self._s7_client, start, amount, byref(cdata))
         check_error(result)
         return result
 
     def as_upload(self, block_num: int, _buffer, size) -> int:
         """Uploads a block from AG.
 
         Note:
@@ -1237,28 +1250,28 @@
             _buffer: buffer where the data will be place.
             size: amount of bytes to uplaod.
 
         Returns:
             Snap7 code.
         """
         block_type = block_types["DB"]
-        result = self._library.Cli_AsUpload(self._pointer, block_type, block_num, byref(_buffer), byref(size))
+        result = self._lib.Cli_AsUpload(self._s7_client, block_type, block_num, byref(_buffer), byref(size))
         check_error(result, context="client")
         return result
 
     def copy_ram_to_rom(self, timeout: int = 1) -> int:
         """Performs the Copy Ram to Rom action.
 
         Args:
             timeout: timeout time.
 
         Returns:
             Snap7 code.
         """
-        result = self._library.Cli_CopyRamToRom(self._pointer, timeout)
+        result = self._lib.Cli_CopyRamToRom(self._s7_client, timeout)
         check_error(result, context="client")
         return result
 
     def ct_read(self, start: int, amount: int) -> bytearray:
         """Reads counters from a PLC.
 
         Args:
@@ -1266,15 +1279,15 @@
             amount: amount of bytes to read.
 
         Returns:
             Buffer read.
         """
         type_ = wordlen_to_ctypes[WordLen.Counter.value]
         data = (type_ * amount)()
-        result = self._library.Cli_CTRead(self._pointer, start, amount, byref(data))
+        result = self._lib.Cli_CTRead(self._s7_client, start, amount, byref(data))
         check_error(result, context="client")
         return bytearray(data)
 
     def ct_write(self, start: int, amount: int, data: bytearray) -> int:
         """Write counters into a PLC.
 
         Args:
@@ -1283,29 +1296,29 @@
             data: buffer data to write.
 
         Returns:
             Snap7 code.
         """
         type_ = wordlen_to_ctypes[WordLen.Counter.value]
         cdata = (type_ * amount).from_buffer_copy(data)
-        result = self._library.Cli_CTWrite(self._pointer, start, amount, byref(cdata))
+        result = self._lib.Cli_CTWrite(self._s7_client, start, amount, byref(cdata))
         check_error(result)
         return result
 
     def db_fill(self, db_number: int, filler: int) -> int:
         """Fills a DB in AG with a given byte.
 
         Args:
             db_number: db number to fill.
             filler: value filler.
 
         Returns:
             Snap7 code.
         """
-        result = self._library.Cli_DBFill(self._pointer, db_number, filler)
+        result = self._lib.Cli_DBFill(self._s7_client, db_number, filler)
         check_error(result)
         return result
 
     def eb_read(self, start: int, size: int) -> bytearray:
         """Reads a part of IPI area from a PLC.
 
         Args:
@@ -1313,15 +1326,15 @@
             size: amount of bytes to read.
 
         Returns:
             Data read.
         """
         type_ = wordlen_to_ctypes[WordLen.Byte.value]
         data = (type_ * size)()
-        result = self._library.Cli_EBRead(self._pointer, start, size, byref(data))
+        result = self._lib.Cli_EBRead(self._s7_client, start, size, byref(data))
         check_error(result, context="client")
         return bytearray(data)
 
     def eb_write(self, start: int, size: int, data: bytearray) -> int:
         """Writes a part of IPI area into a PLC.
 
         Args:
@@ -1330,15 +1343,15 @@
             data: data to write.
 
         Returns:
             Snap7 code.
         """
         type_ = wordlen_to_ctypes[WordLen.Byte.value]
         cdata = (type_ * size).from_buffer_copy(data)
-        result = self._library.Cli_EBWrite(self._pointer, start, size, byref(cdata))
+        result = self._lib.Cli_EBWrite(self._s7_client, start, size, byref(cdata))
         check_error(result)
         return result
 
     def error_text(self, error: int) -> str:
         """Returns a textual explanation of a given error number.
 
         Args:
@@ -1346,60 +1359,60 @@
 
         Returns:
             Text error.
         """
         text_length = c_int(256)
         error_code = c_int32(error)
         text = create_string_buffer(buffer_size)
-        response = self._library.Cli_ErrorText(error_code, byref(text), text_length)
+        response = self._lib.Cli_ErrorText(error_code, byref(text), text_length)
         check_error(response)
         result = bytearray(text)[: text_length.value].decode().strip("\x00")
         return result
 
     def get_cp_info(self) -> S7CpInfo:
         """Returns some information about the CP (communication processor).
 
         Returns:
             Structure object containing the CP information.
         """
         cp_info = S7CpInfo()
-        result = self._library.Cli_GetCpInfo(self._pointer, byref(cp_info))
+        result = self._lib.Cli_GetCpInfo(self._s7_client, byref(cp_info))
         check_error(result)
         return cp_info
 
     def get_exec_time(self) -> int:
         """Returns the last job execution time in milliseconds.
 
         Returns:
             Execution time value.
         """
         time = c_int32()
-        result = self._library.Cli_GetExecTime(self._pointer, byref(time))
+        result = self._lib.Cli_GetExecTime(self._s7_client, byref(time))
         check_error(result)
         return time.value
 
     def get_last_error(self) -> int:
         """Returns the last job result.
 
         Returns:
             Returns the last error value.
         """
         last_error = c_int32()
-        result = self._library.Cli_GetLastError(self._pointer, byref(last_error))
+        result = self._lib.Cli_GetLastError(self._s7_client, byref(last_error))
         check_error(result)
         return last_error.value
 
     def get_order_code(self) -> S7OrderCode:
         """Returns the CPU order code.
 
         Returns:
             Order of the code in a structure object.
         """
         order_code = S7OrderCode()
-        result = self._library.Cli_GetOrderCode(self._pointer, byref(order_code))
+        result = self._lib.Cli_GetOrderCode(self._s7_client, byref(order_code))
         check_error(result)
         return order_code
 
     def get_pg_block_info(self, block: bytearray) -> TS7BlockInfo:
         """Returns detailed information about a block loaded in memory.
 
         Args:
@@ -1407,41 +1420,41 @@
 
         Returns:
             Structure object that contains the block information.
         """
         block_info = TS7BlockInfo()
         size = c_int(len(block))
         buffer = (c_byte * len(block)).from_buffer_copy(block)
-        result = self._library.Cli_GetPgBlockInfo(self._pointer, byref(buffer), byref(block_info), size)
+        result = self._lib.Cli_GetPgBlockInfo(self._s7_client, byref(buffer), byref(block_info), size)
         check_error(result)
         return block_info
 
     def get_protection(self) -> S7Protection:
         """Gets the CPU protection level info.
 
         Returns:
             Structure object with protection attributes.
         """
         s7_protection = S7Protection()
-        result = self._library.Cli_GetProtection(self._pointer, byref(s7_protection))
+        result = self._lib.Cli_GetProtection(self._s7_client, byref(s7_protection))
         check_error(result)
         return s7_protection
 
     def iso_exchange_buffer(self, data: bytearray) -> bytearray:
         """Exchanges a given S7 PDU (protocol data unit) with the CPU.
 
         Args:
             data: buffer to exchange.
 
         Returns:
             Snap7 code.
         """
         size = c_int(len(data))
         cdata = (c_byte * len(data)).from_buffer_copy(data)
-        response = self._library.Cli_IsoExchangeBuffer(self._pointer, byref(cdata), byref(size))
+        response = self._lib.Cli_IsoExchangeBuffer(self._s7_client, byref(cdata), byref(size))
         check_error(response)
         result = bytearray(cdata)[: size.value]
         return result
 
     def mb_read(self, start: int, size: int) -> bytearray:
         """Reads a part of Merkers area from a PLC.
 
@@ -1450,15 +1463,15 @@
             size: amount of bytes to read.
 
         Returns:
             Buffer with the data read.
         """
         type_ = wordlen_to_ctypes[WordLen.Byte.value]
         data = (type_ * size)()
-        result = self._library.Cli_MBRead(self._pointer, start, size, byref(data))
+        result = self._lib.Cli_MBRead(self._s7_client, start, size, byref(data))
         check_error(result, context="client")
         return bytearray(data)
 
     def mb_write(self, start: int, size: int, data: bytearray) -> int:
         """Writes a part of Merkers area into a PLC.
 
         Args:
@@ -1467,15 +1480,15 @@
             data: buffer to write.
 
         Returns:
             Snap7 code.
         """
         type_ = wordlen_to_ctypes[WordLen.Byte.value]
         cdata = (type_ * size).from_buffer_copy(data)
-        result = self._library.Cli_MBWrite(self._pointer, start, size, byref(cdata))
+        result = self._lib.Cli_MBWrite(self._s7_client, start, size, byref(cdata))
         check_error(result)
         return result
 
     def read_szl(self, ssl_id: int, index: int = 0x0000) -> S7SZL:
         """Reads a partial list of given ID and Index.
 
         Args:
@@ -1483,38 +1496,38 @@
             index: index to be read.
 
         Returns:
             SZL structure object.
         """
         s7_szl = S7SZL()
         size = c_int(sizeof(s7_szl))
-        result = self._library.Cli_ReadSZL(self._pointer, ssl_id, index, byref(s7_szl), byref(size))
+        result = self._lib.Cli_ReadSZL(self._s7_client, ssl_id, index, byref(s7_szl), byref(size))
         check_error(result, context="client")
         return s7_szl
 
     def read_szl_list(self) -> bytearray:
         """Reads the list of partial lists available in the CPU.
 
         Returns:
             Buffer read.
         """
         szl_list = S7SZLList()
         items_count = c_int(sizeof(szl_list))
-        response = self._library.Cli_ReadSZLList(self._pointer, byref(szl_list), byref(items_count))
+        response = self._lib.Cli_ReadSZLList(self._s7_client, byref(szl_list), byref(items_count))
         check_error(response, context="client")
         result = bytearray(szl_list.List)[: items_count.value]
         return result
 
     def set_plc_system_datetime(self) -> int:
         """Sets the PLC date/time with the host (PC) date/time.
 
         Returns:
             Snap7 code.
         """
-        result = self._library.Cli_SetPlcSystemDateTime(self._pointer)
+        result = self._lib.Cli_SetPlcSystemDateTime(self._s7_client)
         check_error(result)
         return result
 
     def tm_read(self, start: int, amount: int) -> bytearray:
         """Reads timers from a PLC.
 
         Args:
@@ -1523,15 +1536,15 @@
 
         Returns:
             Buffer read.
         """
         wordlen = WordLen.Timer
         type_ = wordlen_to_ctypes[wordlen.value]
         data = (type_ * amount)()
-        result = self._library.Cli_TMRead(self._pointer, start, amount, byref(data))
+        result = self._lib.Cli_TMRead(self._s7_client, start, amount, byref(data))
         check_error(result, context="client")
         return bytearray(data)
 
     def tm_write(self, start: int, amount: int, data: bytearray) -> int:
         """Write timers into a PLC.
 
         Args:
@@ -1541,15 +1554,15 @@
 
         Returns:
             Snap7 code.
         """
         wordlen = WordLen.Timer
         type_ = wordlen_to_ctypes[wordlen.value]
         cdata = (type_ * amount).from_buffer_copy(data)
-        result = self._library.Cli_TMWrite(self._pointer, start, amount, byref(cdata))
+        result = self._lib.Cli_TMWrite(self._s7_client, start, amount, byref(cdata))
         check_error(result)
         return result
 
     def write_multi_vars(self, items: List[S7DataItem]) -> int:
         """Writes different kind of variables into a PLC simultaneously.
 
         Args:
@@ -1559,10 +1572,10 @@
             Snap7 code.
         """
         items_count = c_int32(len(items))
         data = bytearray()
         for item in items:
             data += bytearray(item)
         cdata = (S7DataItem * len(items)).from_buffer_copy(data)
-        result = self._library.Cli_WriteMultiVars(self._pointer, byref(cdata), items_count)
+        result = self._lib.Cli_WriteMultiVars(self._s7_client, byref(cdata), items_count)
         check_error(result, context="client")
         return result
```

### Comparing `python_snap7-1.4/snap7/common.py` & `python_snap7-1.4.1/snap7/common.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,87 +1,100 @@
 import sys
 import logging
 import pathlib
 import platform
 from pathlib import Path
 from ctypes import c_char
-from typing import Optional
+from typing import Any, Literal, Optional
 from ctypes.util import find_library
+from functools import cache
 
 if platform.system() == "Windows":
     from ctypes import windll as cdll  # type: ignore
 else:
     from ctypes import cdll
 
 logger = logging.getLogger(__name__)
 
 # regexp for checking if an ipv4 address is valid.
 ipv4 = r"^(([0-9]|[1-9][0-9]|1[0-9]{2}|2[0-4][0-9]|25[0-5])\.){3}([0-9]|[1-9][0-9]|1[0-9]{2}|2[0-4][0-9]|25[0-5])$"
 
 
-class Snap7Library:
-    """Snap7 loader and encapsulator. We make this a singleton to make
-        sure the library is loaded only once.
-
-    Attributes:
-        lib_location: full path to the `snap7.dll` file. Optional.
-    """
-
-    _instance = None
-    lib_location: Optional[str]
-
-    def __new__(cls, *args, **kwargs):
-        if not cls._instance:
-            cls._instance = object.__new__(cls)
-            cls._instance.lib_location = None
-            cls._instance.cdll = None
-        return cls._instance
-
-    def __init__(self, lib_location: Optional[str] = None):
-        """Loads the snap7 library using ctypes cdll.
-
-        Args:
-            lib_location: full path to the `snap7.dll` file. Optional.
-
-        Raises:
-            RuntimeError: if `lib_location` is not found.
-        """
-        if self.cdll:  # type: ignore
-            return
-        self.lib_location = (
-            lib_location or self.lib_location or find_in_package() or find_library("snap7") or find_locally("snap7")
-        )
-        if not self.lib_location:
-            error = f"""can't find snap7 shared library.
+def _raise_error():
+    error = f"""can't find snap7 shared library.
 
 This probably means you are installing python-snap7 from source. When no binary wheel is found for you architecture, pip
 install falls back on a source install. For this to work, you need to manually install the snap7 library, which python-snap7
 uses under the hood.
 
 The shortest path to success is to try to get a binary wheel working. Probably you are running on an unsupported
 platform or python version. You are running:
 
 machine: {platform.machine()}
 system: {platform.system()}
 python version: {platform.python_version()}
 """
-            logger.error(error)
-            raise RuntimeError(error)
-        self.cdll = cdll.LoadLibrary(self.lib_location)
+    logger.error(error)
+    raise RuntimeError(error)
+
+
+def _find_locally(fname: str = "snap7") -> Optional[str]:
+    """Finds the `snap7.dll` file in the local project directory.
+
+    Args:
+        fname: file name to search for. Optional.
+
+    Returns:
+        Full path to the `snap7.dll` file.
+    """
+    file = pathlib.Path.cwd() / f"{fname}.dll"
+    if file.exists():
+        return str(file)
+    return None
+
+
+def _find_in_package() -> Optional[str]:
+    """Find the `snap7.dll` file according to the os used.
+
+    Returns:
+        Full path to the `snap7.dll` file.
+    """
+    basedir = pathlib.Path(__file__).parent.absolute()
+    if sys.platform == "darwin":
+        lib = "libsnap7.dylib"
+    elif sys.platform == "win32":
+        lib = "snap7.dll"
+    else:
+        lib = "libsnap7.so"
+    full_path = basedir.joinpath("lib", lib)
+    if Path.exists(full_path) and Path.is_file(full_path):
+        return str(full_path)
+    return None
 
 
-def load_library(lib_location: Optional[str] = None):
+@cache
+def load_library(lib_location: Optional[str] = None) -> Any:
     """Loads the `snap7.dll` library.
     Returns:
         cdll: a ctypes cdll object with the snap7 shared library loaded.
     """
-    return Snap7Library(lib_location).cdll
+    if not lib_location:
+        lib_location = _find_in_package() or find_library("snap7") or _find_locally("snap7")
 
+    if not lib_location:
+        _raise_error()
 
-def check_error(code: int, context: str = "client") -> None:
+    return cdll.LoadLibrary(lib_location)
+
+
+Context = Literal["client", "server", "partner"]
+
+
+@cache
+def check_error(code: int, context: Context = "client") -> None:
     """Check if the error code is set. If so, a Python log message is generated
         and an error is raised.
 
     Args:
         code: error code number.
         context: context in which is called.
 
@@ -90,15 +103,15 @@
     """
     if code and code != 1:
         error = error_text(code, context)
         logger.error(error)
         raise RuntimeError(error)
 
 
-def error_text(error, context: str = "client") -> bytes:
+def error_text(error, context: Context = "client") -> bytes:
     """Returns a textual explanation of a given error number
 
     Args:
         error: an error integer
         context: context in which is called from, server, client or partner
 
     Returns:
@@ -110,48 +123,10 @@
     if context not in ("client", "server", "partner"):
         raise TypeError(f"Unkown context {context} used, should be either client, server or partner")
     logger.debug(f"error text for {hex(error)}")
     len_ = 1024
     text_type = c_char * len_
     text = text_type()
     library = load_library()
-    if context == "client":
-        library.Cli_ErrorText(error, text, len_)
-    elif context == "server":
-        library.Srv_ErrorText(error, text, len_)
-    elif context == "partner":
-        library.Par_ErrorText(error, text, len_)
+    map_ = {"client": library.Cli_ErrorText, "server": library.Srv_ErrorText, "partner": library.Par_ErrorText}
+    map_[context](error, text, len_)
     return text.value
-
-
-def find_locally(fname: str = "snap7") -> Optional[str]:
-    """Finds the `snap7.dll` file in the local project directory.
-
-    Args:
-        fname: file name to search for. Optional.
-
-    Returns:
-        Full path to the `snap7.dll` file.
-    """
-    file = pathlib.Path.cwd() / f"{fname}.dll"
-    if file.exists():
-        return str(file)
-    return None
-
-
-def find_in_package() -> Optional[str]:
-    """Find the `snap7.dll` file according to the os used.
-
-    Returns:
-        Full path to the `snap7.dll` file.
-    """
-    basedir = pathlib.Path(__file__).parent.absolute()
-    if sys.platform == "darwin":
-        lib = "libsnap7.dylib"
-    elif sys.platform == "win32":
-        lib = "snap7.dll"
-    else:
-        lib = "libsnap7.so"
-    full_path = basedir.joinpath("lib", lib)
-    if Path.exists(full_path) and Path.is_file(full_path):
-        return str(full_path)
-    return None
```

### Comparing `python_snap7-1.4/snap7/error.py` & `python_snap7-1.4.1/snap7/error.py`

 * *Files identical despite different names*

### Comparing `python_snap7-1.4/snap7/logo.py` & `python_snap7-1.4.1/snap7/logo.py`

 * *Files identical despite different names*

### Comparing `python_snap7-1.4/snap7/partner.py` & `python_snap7-1.4.1/snap7/partner.py`

 * *Files identical despite different names*

### Comparing `python_snap7-1.4/snap7/server/__init__.py` & `python_snap7-1.4.1/snap7/server/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Snap7 server used for mimicking a siemens 7 server.
 """
 
 import re
 import time
-import ctypes
+from ctypes import c_char, byref, sizeof, c_int, c_int32, c_uint32, c_void_p, CFUNCTYPE, POINTER, Array, c_int8
 import struct
 import logging
 from typing import Any, Tuple, Callable, Optional
 
 from ..common import ipv4, check_error, load_library
 from ..types import SrvEvent, LocalPort, cpu_statuses, server_statuses
 from ..types import longword, wordlen_to_ctypes, WordLen, S7Object
@@ -28,81 +28,89 @@
 
 
 class Server:
     """
     A fake S7 server.
     """
 
+    _lib: Any  # since this is dynamically loaded from a DLL we don't have the type signature.
+    _s7_server: Optional[S7Object] = None
+    _read_callback = None
+    _callback: Optional[Callable[..., Any]] = None
+
     def __init__(self, log: bool = True):
         """Create a fake S7 server. set log to false if you want to disable
             event logging to python logging.
 
         Args:
             log: `True` for enabling the event logging. Optinoal.
         """
-        self._read_callback = None
-        self._callback = Optional[Callable[..., Any]]
-        self.pointer = None
-        self.library = load_library()
+        self._lib = load_library()
         self.create()
         if log:
             self._set_log_callback()
 
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.destroy()
+
     def __del__(self):
         self.destroy()
 
     def event_text(self, event: SrvEvent) -> str:
         """Returns a textual explanation of a given event object
 
         Args:
             event: an PSrvEvent struct object
 
         Returns:
             The error string
         """
         logger.debug(f"error text for {hex(event.EvtCode)}")
         len_ = 1024
-        text_type = ctypes.c_char * len_
+        text_type = c_char * len_
         text = text_type()
-        error = self.library.Srv_EventText(ctypes.byref(event), ctypes.byref(text), len_)
+        error = self._lib.Srv_EventText(byref(event), byref(text), len_)
         check_error(error)
         return text.value.decode("ascii")
 
     def create(self):
         """Create the server."""
         logger.info("creating server")
-        self.library.Srv_Create.restype = S7Object
-        self.pointer = S7Object(self.library.Srv_Create())
+        self._lib.Srv_Create.restype = S7Object
+        self._s7_server = S7Object(self._lib.Srv_Create())
 
     @error_wrap
-    def register_area(self, area_code: int, index: int, userdata: ctypes.Array[ctypes.c_int8]):
+    def register_area(self, area_code: int, index: int, userdata: Array[c_int8]):
         """Shares a memory area with the server. That memory block will be
             visible by the clients.
 
         Args:
             area_code: memory area to register.
             index: number of area to write.
             userdata: buffer with the data to write.
 
         Returns:
             Error code from snap7 library.
         """
-        size = ctypes.sizeof(userdata)
+        size = sizeof(userdata)
         logger.info(f"registering area {area_code}, index {index}, size {size}")
-        return self.library.Srv_RegisterArea(self.pointer, area_code, index, ctypes.byref(userdata), size)
+        return self._lib.Srv_RegisterArea(self._s7_server, area_code, index, byref(userdata), size)
 
     @error_wrap
     def set_events_callback(self, call_back: Callable[..., Any]) -> int:
         """Sets the user callback that the Server object has to call when an
         event is created.
         """
         logger.info("setting event callback")
-        callback_wrap: Callable[..., Any] = ctypes.CFUNCTYPE(None, ctypes.c_void_p, ctypes.POINTER(SrvEvent), ctypes.c_int)
+        callback_wrap: Callable[..., Any] = CFUNCTYPE(None, c_void_p, POINTER(SrvEvent), c_int)
 
-        def wrapper(usrptr: Optional[ctypes.c_void_p], pevent: SrvEvent, size: int) -> int:
+        def wrapper(usrptr: Optional[c_void_p], pevent: SrvEvent, size: int) -> int:
             """Wraps python function into a ctypes function
 
             Args:
                 usrptr: not used
                 pevent: pointer to snap7 event struct
                 size:
 
@@ -110,29 +118,29 @@
                 Should return an int
             """
             logger.info(f"callback event: {self.event_text(pevent.contents)}")
             call_back(pevent.contents)
             return 0
 
         self._callback = callback_wrap(wrapper)
-        usrPtr = ctypes.c_void_p()
-        return self.library.Srv_SetEventsCallback(self.pointer, self._callback, usrPtr)
+        usrPtr = c_void_p()
+        return self._lib.Srv_SetEventsCallback(self._s7_server, self._callback, usrPtr)
 
     @error_wrap
     def set_read_events_callback(self, call_back: Callable[..., Any]):
         """Sets the user callback that the Server object has to call when a Read
             event is created.
 
         Args:
             call_back: a callback function that accepts a pevent argument.
         """
         logger.info("setting read event callback")
-        callback_wrapper: Callable[..., Any] = ctypes.CFUNCTYPE(None, ctypes.c_void_p, ctypes.POINTER(SrvEvent), ctypes.c_int)
+        callback_wrapper: Callable[..., Any] = CFUNCTYPE(None, c_void_p, POINTER(SrvEvent), c_int)
 
-        def wrapper(usrptr: Optional[ctypes.c_void_p], pevent: SrvEvent, size: int) -> int:
+        def wrapper(usrptr: Optional[c_void_p], pevent: SrvEvent, size: int) -> int:
             """Wraps python function into a ctypes function
 
             Args:
                 usrptr: not used
                 pevent: pointer to snap7 event struct
                 size:
 
@@ -140,15 +148,15 @@
                 Should return an int
             """
             logger.info(f"callback event: {self.event_text(pevent.contents)}")
             call_back(pevent.contents)
             return 0
 
         self._read_callback = callback_wrapper(wrapper)
-        return self.library.Srv_SetReadEventsCallback(self.pointer, self._read_callback)
+        return self._lib.Srv_SetReadEventsCallback(self._s7_server, self._read_callback)
 
     def _set_log_callback(self):
         """Sets a callback that logs the events"""
         logger.debug("setting up event logger")
 
         def log_callback(event):
             logger.info(f"callback event: {self.event_text(event)}")
@@ -162,42 +170,42 @@
         Args:
             tcpport: port that the server will listen. Optional.
         """
         if tcpport != 102:
             logger.info(f"setting server TCP port to {tcpport}")
             self.set_param(LocalPort, tcpport)
         logger.info(f"starting server on 0.0.0.0:{tcpport}")
-        return self.library.Srv_Start(self.pointer)
+        return self._lib.Srv_Start(self._s7_server)
 
     @error_wrap
     def stop(self):
         """Stop the server."""
         logger.info("stopping server")
-        return self.library.Srv_Stop(self.pointer)
+        return self._lib.Srv_Stop(self._s7_server)
 
-    def destroy(self):
+    def destroy(self) -> Optional[int]:
         """Destroy the server."""
         logger.info("destroying server")
-        if hasattr(self, "library") and self.library:
-            self.library.Srv_Destroy(ctypes.byref(self.pointer))
+        if self._lib and self._s7_server is not None:
+            return self._lib.Srv_Destroy(byref(self._s7_server))
+        self._s7_server = None
+        return None
 
     def get_status(self) -> Tuple[str, str, int]:
         """Reads the server status, the Virtual CPU status and the number of
             the clients connected.
 
         Returns:
             Server status, cpu status, client count
         """
         logger.debug("get server status")
-        server_status = ctypes.c_int()
-        cpu_status = ctypes.c_int()
-        clients_count = ctypes.c_int()
-        error = self.library.Srv_GetStatus(
-            self.pointer, ctypes.byref(server_status), ctypes.byref(cpu_status), ctypes.byref(clients_count)
-        )
+        server_status = c_int()
+        cpu_status = c_int()
+        clients_count = c_int()
+        error = self._lib.Srv_GetStatus(self._s7_server, byref(server_status), byref(cpu_status), byref(clients_count))
         check_error(error)
         logger.debug(f"status server {server_status.value} cpu {cpu_status.value} clients {clients_count.value}")
         return (server_statuses[server_status.value], cpu_statuses[cpu_status.value], clients_count.value)
 
     @error_wrap
     def unregister_area(self, area_code: int, index: int):
         """'Unshares' a memory area previously shared with Srv_RegisterArea().
@@ -208,43 +216,43 @@
         Args:
             area_code: memory area.
             index: number of the memory area.
 
         Returns:
             Error code from snap7 library.
         """
-        return self.library.Srv_UnregisterArea(self.pointer, area_code, index)
+        return self._lib.Srv_UnregisterArea(self._s7_server, area_code, index)
 
     @error_wrap
     def unlock_area(self, code: int, index: int):
         """Unlocks a previously locked shared memory area.
 
         Args:
             code: memory area.
             index: number of the memory area.
 
         Returns:
             Error code from snap7 library.
         """
         logger.debug(f"unlocking area code {code} index {index}")
-        return self.library.Srv_UnlockArea(self.pointer, code, index)
+        return self._lib.Srv_UnlockArea(self._s7_server, code, index)
 
     @error_wrap
     def lock_area(self, code: int, index: int):
         """Locks a shared memory area.
 
         Args:
             code: memory area.
             index: number of the memory area.
 
         Returns:
             Error code from snap7 library.
         """
         logger.debug(f"locking area code {code} index {index}")
-        return self.library.Srv_LockArea(self.pointer, code, index)
+        return self._lib.Srv_LockArea(self._s7_server, code, index)
 
     @error_wrap
     def start_to(self, ip: str, tcpport: int = 102):
         """Start server on a specific interface.
 
         Args:
             ip: IPV4 address where the server is located.
@@ -255,43 +263,43 @@
         """
         if tcpport != 102:
             logger.info(f"setting server TCP port to {tcpport}")
             self.set_param(LocalPort, tcpport)
         if not re.match(ipv4, ip):
             raise ValueError(f"{ip} is invalid ipv4")
         logger.info(f"starting server to {ip}:102")
-        return self.library.Srv_StartTo(self.pointer, ip.encode())
+        return self._lib.Srv_StartTo(self._s7_server, ip.encode())
 
     @error_wrap
     def set_param(self, number: int, value: int):
         """Sets an internal Server object parameter.
 
         Args:
             number: number of the parameter.
             value: value to be set.
 
         Returns:
             Error code from snap7 library.
         """
         logger.debug(f"setting param number {number} to {value}")
-        return self.library.Srv_SetParam(self.pointer, number, ctypes.byref(ctypes.c_int(value)))
+        return self._lib.Srv_SetParam(self._s7_server, number, byref(c_int(value)))
 
     @error_wrap
     def set_mask(self, kind: int, mask: int):
         """Writes the specified filter mask.
 
         Args:
             kind:
             mask:
 
         Returns:
             Error code from snap7 library.
         """
         logger.debug(f"setting mask kind {kind} to {mask}")
-        return self.library.Srv_SetMask(self.pointer, kind, mask)
+        return self._lib.Srv_SetMask(self._s7_server, kind, mask)
 
     @error_wrap
     def set_cpu_status(self, status: int):
         """Sets the Virtual CPU status.
 
         Args:
             status: :obj:`cpu_statuses` object type.
@@ -301,26 +309,26 @@
 
         Raises:
             :obj:`ValueError`: if `status` is not in :obj:`cpu_statuses`.
         """
         if status not in cpu_statuses:
             raise ValueError(f"The cpu state ({status}) is invalid")
         logger.debug(f"setting cpu status to {status}")
-        return self.library.Srv_SetCpuStatus(self.pointer, status)
+        return self._lib.Srv_SetCpuStatus(self._s7_server, status)
 
     def pick_event(self) -> Optional[SrvEvent]:
         """Extracts an event (if available) from the Events queue.
 
         Returns:
             Server event.
         """
         logger.debug("checking event queue")
         event = SrvEvent()
-        ready = ctypes.c_int32()
-        code = self.library.Srv_PickEvent(self.pointer, ctypes.byref(event), ctypes.byref(ready))
+        ready = c_int32()
+        code = self._lib.Srv_PickEvent(self._s7_server, byref(event), byref(ready))
         check_error(code)
         if ready:
             logger.debug(f"one event ready: {event}")
             return event
         logger.debug("no events ready")
         return None
 
@@ -330,43 +338,43 @@
         Args:
             number: number of the parameter to be set.
 
         Returns:
             Value of the parameter.
         """
         logger.debug(f"retreiving param number {number}")
-        value = ctypes.c_int()
-        code = self.library.Srv_GetParam(self.pointer, number, ctypes.byref(value))
+        value = c_int()
+        code = self._lib.Srv_GetParam(self._s7_server, number, byref(value))
         check_error(code)
         return value.value
 
-    def get_mask(self, kind: int) -> ctypes.c_uint32:
+    def get_mask(self, kind: int) -> c_uint32:
         """Reads the specified filter mask.
 
         Args:
             kind:
 
         Returns:
             Mask
         """
         logger.debug(f"retrieving mask kind {kind}")
         mask = longword()
-        code = self.library.Srv_GetMask(self.pointer, kind, ctypes.byref(mask))
+        code = self._lib.Srv_GetMask(self._s7_server, kind, byref(mask))
         check_error(code)
         return mask
 
     @error_wrap
     def clear_events(self) -> int:
         """Empties the Event queue.
 
         Returns:
             Error code from snap7 library.
         """
         logger.debug("clearing event queue")
-        return self.library.Srv_ClearEvents(self.pointer)
+        return self._lib.Srv_ClearEvents(self._s7_server)
 
 
 def mainloop(tcpport: int = 1102, init_standard_values: bool = False):
     """Init a fake Snap7 server with some default values.
 
     Args:
         tcpport: port that the server will listen.
```

### Comparing `python_snap7-1.4/snap7/server/__main__.py` & `python_snap7-1.4.1/snap7/server/__main__.py`

 * *Files identical despite different names*

### Comparing `python_snap7-1.4/snap7/types.py` & `python_snap7-1.4.1/snap7/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -249,14 +249,27 @@
         return (
             f"<S7DataItem Area: {self.Area} WordLen: {self.WordLen} Result: {self.Result} "
             f"DBNumber: {self.DBNumber} Start: {self.Start} Amount: {self.Amount} pData: {self.pData}>"
         )
 
 
 class S7CpuInfo(ctypes.Structure):
+    """
+    S7CpuInfo class for handling CPU with :
+        - ModuleTypeName => Model of S7-CPU
+        - SerialNumber => SN of the S7-CPU
+        - ASName => Family Class of the S7-CPU
+        - Copyright => Siemens Copyright
+        - ModuleName => TIA project name or for other S7-CPU, same as ModuleTypeName
+    Examples:
+        For str handling instead of bytes
+        >>> if hasattr(self, 'SerialNumber'):
+        >>>     return str(self.SerialNumber, encoding="utf-8")
+    """
+
     _fields_ = [
         ("ModuleTypeName", ctypes.c_char * 33),
         ("SerialNumber", ctypes.c_char * 25),
         ("ASName", ctypes.c_char * 25),
         ("Copyright", ctypes.c_char * 27),
         ("ModuleName", ctypes.c_char * 25),
     ]
@@ -294,14 +307,28 @@
 
 
 class S7OrderCode(ctypes.Structure):
     _fields_ = [("OrderCode", ctypes.c_char * 21), ("V1", ctypes.c_byte), ("V2", ctypes.c_byte), ("V3", ctypes.c_byte)]
 
 
 class S7CpInfo(ctypes.Structure):
+    """
+    S7 Cp class for Communication Information :
+        - MaxPduLength => Size of the maximum PDU length in bytes
+        - MaxConnections => Max connection allowed to S7-CPU or Server
+        - MaxMpiRate => MPI rate (MPI use is deprecated)
+        - MaxBusRate => Profibus rate
+    Every data packet exchanged with a PLC must fit within the PDU size,
+    whose is fixed from 240 up to 960 bytes.
+    For debugging S7 protocol, this informations are essentials !
+    Examples:
+        >>> if hasattr(self, 'MaxBusRate'):
+        >>>     return int(self.MaxBusRate)
+    """
+
     _fields_ = [
         ("MaxPduLength", ctypes.c_uint16),
         ("MaxConnections", ctypes.c_uint16),
         ("MaxMpiRate", ctypes.c_uint16),
         ("MaxBusRate", ctypes.c_uint16),
     ]
```

### Comparing `python_snap7-1.4/snap7/util/__init__.py` & `python_snap7-1.4.1/snap7/util/__init__.py`

 * *Files identical despite different names*

### Comparing `python_snap7-1.4/snap7/util/db.py` & `python_snap7-1.4.1/snap7/util/db.py`

 * *Files identical despite different names*

### Comparing `python_snap7-1.4/snap7/util/getters.py` & `python_snap7-1.4.1/snap7/util/getters.py`

 * *Files identical despite different names*

### Comparing `python_snap7-1.4/snap7/util/setters.py` & `python_snap7-1.4.1/snap7/util/setters.py`

 * *Files identical despite different names*

### Comparing `python_snap7-1.4/tests/test_client.py` & `python_snap7-1.4.1/tests/test_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,23 +5,46 @@
 import time
 import pytest
 import unittest
 from datetime import datetime, timedelta, date
 from multiprocessing import Process
 from unittest import mock
 
-
-import snap7
-import snap7.util.getters
-import snap7.util.setters
+from snap7.util.getters import get_real, get_int
+from snap7.util.setters import set_int
 from snap7 import util
 from snap7.common import check_error
 from snap7.server import mainloop
-from snap7.types import S7AreaDB, S7DataItem, S7SZL, S7SZLList, buffer_type, buffer_size, Areas, WordLen
-
+from snap7.client import Client
+from snap7.types import (
+    S7AreaDB,
+    S7DataItem,
+    S7SZL,
+    S7SZLList,
+    buffer_type,
+    buffer_size,
+    Areas,
+    WordLen,
+    wordlen_to_ctypes,
+    RemotePort,
+    LocalPort,
+    WorkInterval,
+    MaxClients,
+    BSendTimeout,
+    BRecvTimeout,
+    PingTimeout,
+    SendTimeout,
+    RecvTimeout,
+    SrcRef,
+    DstRef,
+    SrcTSap,
+    PDURequest,
+    RecoveryTime,
+    KeepAliveTime,
+)
 
 logging.basicConfig(level=logging.WARNING)
 
 ip = "127.0.0.1"
 tcpport = 1102
 db_number = 1
 rack = 1
@@ -42,15 +65,15 @@
     def tearDownClass(cls):
         cls.process.terminate()
         cls.process.join(1)
         if cls.process.is_alive():
             cls.process.kill()
 
     def setUp(self):
-        self.client = snap7.client.Client()
+        self.client = Client()
         self.client.connect(ip, rack, slot, tcpport)
 
     def tearDown(self):
         self.client.disconnect()
         self.client.destroy()
 
     def _as_check_loop(self, check_times=20) -> int:
@@ -92,15 +115,15 @@
 
         test_value_2 = -129.5
         test_bytes_2 = bytearray(struct.pack(">f", test_value_2))
         self.client.db_write(db, 4, test_bytes_2)
 
         test_value_3 = 123
         test_bytes_3 = bytearray([0, 0])
-        snap7.util.setters.set_int(test_bytes_3, 0, test_value_3)
+        set_int(test_bytes_3, 0, test_value_3)
         self.client.db_write(db, 8, test_bytes_3)
 
         test_values = [test_value_1, test_value_2, test_value_3]
 
         # build up our requests
         data_items = (S7DataItem * 3)()
 
@@ -134,20 +157,19 @@
             pBuffer = ctypes.cast(ctypes.pointer(dataBuffer), ctypes.POINTER(ctypes.c_uint8))
             di.pData = pBuffer
 
         result, data_items = self.client.read_multi_vars(data_items)
 
         result_values = []
         # function to cast bytes to match data_types[] above
-        byte_to_value = [snap7.util.getters.get_real, snap7.util.getters.get_real, snap7.util.getters.get_int]
+        byte_to_value = [get_real, get_real, get_int]
 
         # unpack and test the result of each read
-        for i in range(len(data_items)):
+        for i, di in enumerate(data_items):
             btv = byte_to_value[i]
-            di = data_items[i]
             value = btv(di.pData, 0)
             result_values.append(value)
 
         self.assertEqual(result_values[0], test_values[0])
         self.assertEqual(result_values[1], test_values[1])
         self.assertEqual(result_values[2], test_values[2])
 
@@ -276,15 +298,15 @@
         self.assertEqual(0, result)
 
     def test_as_ab_read(self):
         expected = b"\x10\x01"
         self.client.ab_write(0, bytearray(expected))
 
         wordlen = WordLen.Byte
-        type_ = snap7.types.wordlen_to_ctypes[wordlen.value]
+        type_ = wordlen_to_ctypes[wordlen.value]
         buffer = (type_ * 2)()
         self.client.as_ab_read(0, 2, buffer)
         result = self.client.wait_as_completion(500)
         self.assertEqual(0, result)
         self.assertEqual(expected, bytearray(buffer))
 
     def test_as_ab_write(self):
@@ -304,49 +326,49 @@
         response = self.client.as_compress(time_)
         result = self.client.wait_as_completion(500)
         self.assertEqual(0, response)
         self.assertEqual(0, result)
 
     def test_set_param(self):
         values = (
-            (snap7.types.PingTimeout, 800),
-            (snap7.types.SendTimeout, 15),
-            (snap7.types.RecvTimeout, 3500),
-            (snap7.types.SrcRef, 128),
-            (snap7.types.DstRef, 128),
-            (snap7.types.SrcTSap, 128),
-            (snap7.types.PDURequest, 470),
+            (PingTimeout, 800),
+            (SendTimeout, 15),
+            (RecvTimeout, 3500),
+            (SrcRef, 128),
+            (DstRef, 128),
+            (SrcTSap, 128),
+            (PDURequest, 470),
         )
         for param, value in values:
             self.client.set_param(param, value)
 
-        self.assertRaises(Exception, self.client.set_param, snap7.types.RemotePort, 1)
+        self.assertRaises(Exception, self.client.set_param, RemotePort, 1)
 
     def test_get_param(self):
         expected = (
-            (snap7.types.RemotePort, tcpport),
-            (snap7.types.PingTimeout, 750),
-            (snap7.types.SendTimeout, 10),
-            (snap7.types.RecvTimeout, 3000),
-            (snap7.types.SrcRef, 256),
-            (snap7.types.DstRef, 0),
-            (snap7.types.SrcTSap, 256),
-            (snap7.types.PDURequest, 480),
+            (RemotePort, tcpport),
+            (PingTimeout, 750),
+            (SendTimeout, 10),
+            (RecvTimeout, 3000),
+            (SrcRef, 256),
+            (DstRef, 0),
+            (SrcTSap, 256),
+            (PDURequest, 480),
         )
         for param, value in expected:
             self.assertEqual(self.client.get_param(param), value)
 
         non_client = (
-            snap7.types.LocalPort,
-            snap7.types.WorkInterval,
-            snap7.types.MaxClients,
-            snap7.types.BSendTimeout,
-            snap7.types.BRecvTimeout,
-            snap7.types.RecoveryTime,
-            snap7.types.KeepAliveTime,
+            LocalPort,
+            WorkInterval,
+            MaxClients,
+            BSendTimeout,
+            BRecvTimeout,
+            RecoveryTime,
+            KeepAliveTime,
         )
 
         # invalid param for client
         for param in non_client:
             self.assertRaises(Exception, self.client.get_param, non_client)
 
     def test_as_copy_ram_to_rom(self):
@@ -354,15 +376,15 @@
         self.client.wait_as_completion(1100)
         self.assertEqual(0, response)
 
     def test_as_ct_read(self):
         # Cli_AsCTRead
         expected = b"\x10\x01"
         self.client.ct_write(0, 1, bytearray(expected))
-        type_ = snap7.types.wordlen_to_ctypes[WordLen.Counter.value]
+        type_ = wordlen_to_ctypes[WordLen.Counter.value]
         buffer = (type_ * 1)()
         self.client.as_ct_read(0, 1, buffer)
         self.client.wait_as_completion(500)
         self.assertEqual(expected, bytearray(buffer))
 
     def test_as_ct_write(self):
         # Cli_CTWrite
@@ -392,25 +414,25 @@
         size = 40
         start = 0
         db = 1
         expected = bytearray(40)
         self.client.db_write(db_number=db, start=start, data=expected)
 
         wordlen = WordLen.Byte
-        type_ = snap7.types.wordlen_to_ctypes[wordlen.value]
+        type_ = wordlen_to_ctypes[wordlen.value]
         data = (type_ * size)()
         self.client.as_db_read(db, start, size, data)
         self.client.wait_as_completion(500)
         self.assertEqual(data, expected)
 
     def test_as_db_write(self):
         size = 40
         data = bytearray(size)
         wordlen = WordLen.Byte
-        type_ = snap7.types.wordlen_to_ctypes[wordlen.value]
+        type_ = wordlen_to_ctypes[wordlen.value]
         size = len(data)
         result = (type_ * size).from_buffer_copy(data)
         self.client.as_db_write(db_number=1, start=0, size=size, data=result)
         self.client.wait_as_completion(500)
         self.assertEqual(data, result)
 
     @unittest.skip("TODO: not yet fully implemented")
@@ -443,119 +465,119 @@
         cpuInfo = self.client.get_cpu_info()
         for param, value in expected:
             self.assertEqual(getattr(cpuInfo, param).decode("utf-8"), value)
 
     def test_db_write_with_byte_literal_does_not_throw(self):
         mock_write = mock.MagicMock()
         mock_write.return_value = None
-        original = self.client._library.Cli_DBWrite
-        self.client._library.Cli_DBWrite = mock_write
+        original = self.client._lib.Cli_DBWrite
+        self.client._lib.Cli_DBWrite = mock_write
         data = b"\xde\xad\xbe\xef"
 
         try:
             self.client.db_write(db_number=1, start=0, data=bytearray(data))
         except TypeError as e:
             self.fail(str(e))
         finally:
-            self.client._library.Cli_DBWrite = original
+            self.client._lib.Cli_DBWrite = original
 
     def test_download_with_byte_literal_does_not_throw(self):
         mock_download = mock.MagicMock()
         mock_download.return_value = None
-        original = self.client._library.Cli_Download
-        self.client._library.Cli_Download = mock_download
+        original = self.client._lib.Cli_Download
+        self.client._lib.Cli_Download = mock_download
         data = b"\xde\xad\xbe\xef"
 
         try:
             self.client.download(block_num=db_number, data=bytearray(data))
         except TypeError as e:
             self.fail(str(e))
         finally:
-            self.client._library.Cli_Download = original
+            self.client._lib.Cli_Download = original
 
     def test_write_area_with_byte_literal_does_not_throw(self):
         mock_writearea = mock.MagicMock()
         mock_writearea.return_value = None
-        original = self.client._library.Cli_WriteArea
-        self.client._library.Cli_WriteArea = mock_writearea
+        original = self.client._lib.Cli_WriteArea
+        self.client._lib.Cli_WriteArea = mock_writearea
 
         area = Areas.DB
         dbnumber = 1
         start = 1
         data = b"\xde\xad\xbe\xef"
 
         try:
             self.client.write_area(area, dbnumber, start, bytearray(data))
         except TypeError as e:
             self.fail(str(e))
         finally:
-            self.client._library.Cli_WriteArea = original
+            self.client._lib.Cli_WriteArea = original
 
     def test_ab_write_with_byte_literal_does_not_throw(self):
         mock_write = mock.MagicMock()
         mock_write.return_value = None
-        original = self.client._library.Cli_ABWrite
-        self.client._library.Cli_ABWrite = mock_write
+        original = self.client._lib.Cli_ABWrite
+        self.client._lib.Cli_ABWrite = mock_write
 
         start = 1
         data = b"\xde\xad\xbe\xef"
 
         try:
             self.client.ab_write(start=start, data=bytearray(data))
         except TypeError as e:
             self.fail(str(e))
         finally:
-            self.client._library.Cli_ABWrite = original
+            self.client._lib.Cli_ABWrite = original
 
     @unittest.skip("TODO: not yet fully implemented")
     def test_as_ab_write_with_byte_literal_does_not_throw(self):
         mock_write = mock.MagicMock()
         mock_write.return_value = None
-        original = self.client._library.Cli_AsABWrite
-        self.client._library.Cli_AsABWrite = mock_write
+        original = self.client._lib.Cli_AsABWrite
+        self.client._lib.Cli_AsABWrite = mock_write
 
         start = 1
         data = b"\xde\xad\xbe\xef"
 
         try:
             self.client.as_ab_write(start=start, data=bytearray(data))
         except TypeError as e:
             self.fail(str(e))
         finally:
-            self.client._library.Cli_AsABWrite = original
+            self.client._lib.Cli_AsABWrite = original
 
     @unittest.skip("TODO: not yet fully implemented")
     def test_as_db_write_with_byte_literal_does_not_throw(self):
         mock_write = mock.MagicMock()
         mock_write.return_value = None
-        original = self.client._library.Cli_AsDBWrite
-        self.client._library.Cli_AsDBWrite = mock_write
+        original = self.client._lib.Cli_AsDBWrite
+        self.client._lib.Cli_AsDBWrite = mock_write
         data = b"\xde\xad\xbe\xef"
 
         try:
             self.client.db_write(db_number=1, start=0, data=bytearray(data))
         except TypeError as e:
             self.fail(str(e))
         finally:
-            self.client._library.Cli_AsDBWrite = original
+            self.client._lib.Cli_AsDBWrite = original
 
     @unittest.skip("TODO: not yet fully implemented")
     def test_as_download_with_byte_literal_does_not_throw(self):
         mock_download = mock.MagicMock()
         mock_download.return_value = None
-        original = self.client._library.Cli_AsDownload
-        self.client._library.Cli_AsDownload = mock_download
+        original = self.client._lib.Cli_AsDownload
+        self.client._lib.Cli_AsDownload = mock_download
         data = b"\xde\xad\xbe\xef"
 
         try:
             self.client.as_download(block_num=db_number, data=bytearray(data))
         except TypeError as e:
             self.fail(str(e))
         finally:
-            self.client._library.Cli_AsDownload = original
+            self.client._lib.Cli_AsDownload = original
 
     def test_get_plc_time(self):
         self.assertAlmostEqual(datetime.now().replace(microsecond=0), self.client.get_plc_datetime(), delta=timedelta(seconds=1))
 
     def test_set_plc_datetime(self):
         new_dt = datetime(2011, 1, 1, 1, 1, 1, 0)
         self.client.set_plc_datetime(new_dt)
@@ -709,15 +731,15 @@
         self.client.wait_as_completion(1000)
         res = self.client.read_area(area, dbnumber, start, 1)
         self.assertEqual(timer, bytearray(res))
 
     def test_as_eb_read(self):
         # Cli_AsEBRead
         wordlen = WordLen.Byte
-        type_ = snap7.types.wordlen_to_ctypes[wordlen.value]
+        type_ = wordlen_to_ctypes[wordlen.value]
         buffer = (type_ * 1)()
         response = self.client.as_eb_read(0, 1, buffer)
         self.assertEqual(0, response)
         self.assertRaises(RuntimeError, self.client.wait_as_completion, 500)
 
     def test_as_eb_write(self):
         # Cli_AsEBWrite
@@ -735,15 +757,15 @@
         count = ctypes.c_int()
         self.client.as_list_blocks_of_type("DB", data, count)
         self.assertRaises(RuntimeError, self.client.wait_as_completion, 500)
 
     def test_as_mb_read(self):
         # Cli_AsMBRead
         wordlen = WordLen.Byte
-        type_ = snap7.types.wordlen_to_ctypes[wordlen.value]
+        type_ = wordlen_to_ctypes[wordlen.value]
         data = (type_ * 1)()
         self.client.as_mb_read(0, 1, data)
         bytearray(data)
         self.assertRaises(RuntimeError, self.client.wait_as_completion, 500)
 
     def test_as_mb_write(self):
         # Cli_AsMBWrite
@@ -774,15 +796,15 @@
         self.assertEqual(expected, result)
 
     def test_as_tm_read(self):
         # Cli_AsMBRead
         expected = b"\x10\x01"
         wordlen = WordLen.Timer
         self.client.tm_write(0, 1, bytearray(expected))
-        type_ = snap7.types.wordlen_to_ctypes[wordlen.value]
+        type_ = wordlen_to_ctypes[wordlen.value]
         buffer = (type_ * 1)()
         self.client.as_tm_read(0, 1, buffer)
         self.client.wait_as_completion(500)
         self.assertEqual(expected, bytearray(buffer))
 
     def test_as_tm_write(self):
         # Cli_AsMBWrite
@@ -815,22 +837,22 @@
         filler = 31
         expected = bytearray(filler.to_bytes(1, byteorder="big") * 100)
         self.client.db_fill(1, filler)
         self.assertEqual(expected, self.client.db_read(1, 0, 100))
 
     def test_eb_read(self):
         # Cli_EBRead
-        self.client._library.Cli_EBRead = mock.Mock(return_value=0)
+        self.client._lib.Cli_EBRead = mock.Mock(return_value=0)
         response = self.client.eb_read(0, 1)
         self.assertTrue(isinstance(response, bytearray))
         self.assertEqual(1, len(response))
 
     def test_eb_write(self):
         # Cli_EBWrite
-        self.client._library.Cli_EBWrite = mock.Mock(return_value=0)
+        self.client._lib.Cli_EBWrite = mock.Mock(return_value=0)
         response = self.client.eb_write(0, 1, bytearray(b"\x00"))
         self.assertEqual(0, response)
 
     def test_error_text(self):
         # Cli_ErrorText
         CPU_INVALID_PASSWORD = 0x01E00000
         CPU_INVLID_VALUE = 0x00D00000
@@ -894,22 +916,22 @@
         data = b"\x32\x01\x00\x00\x01\x00\x00\x0e\x00\x00\x04\x01\x12\x0a\x10\x02\x00\x01\x00\x01\x84\x00\x00\x00"
         # PDU response
         expected = bytearray(b"2\x03\x00\x00\x01\x00\x00\x02\x00\x05\x00\x00\x04\x01\xff\x04\x00\x08\x11")
         self.assertEqual(expected, self.client.iso_exchange_buffer(bytearray(data)))
 
     def test_mb_read(self):
         # Cli_MBRead
-        self.client._library.Cli_MBRead = mock.Mock(return_value=0)
+        self.client._lib.Cli_MBRead = mock.Mock(return_value=0)
         response = self.client.mb_read(0, 10)
         self.assertTrue(isinstance(response, bytearray))
         self.assertEqual(10, len(response))
 
     def test_mb_write(self):
         # Cli_MBWrite
-        self.client._library.Cli_MBWrite = mock.Mock(return_value=0)
+        self.client._lib.Cli_MBWrite = mock.Mock(return_value=0)
         response = self.client.mb_write(0, 1, bytearray(b"\x00"))
         self.assertEqual(0, response)
 
     def test_read_szl(self):
         # read_szl_partial_list
         expected_number_of_records = 10
         expected_length_of_record = 34
@@ -991,50 +1013,33 @@
     def test_set_as_callback(self):
         def event_call_back(op_code, op_result):
             logging.info(f"callback event: {op_code} op_result: {op_result}")
 
         self.client.set_as_callback(event_call_back)
 
 
-#        expected = b"\x11\x11"
-#        self.callback_counter = 0
-#        cObj = ctypes.cast(ctypes.pointer(ctypes.py_object(self)), S7Object)
-
-#        def callback(FUsrPtr, JobOp, response):
-#            self = ctypes.cast(FUsrPtr, ctypes.POINTER(ctypes.py_object)).contents.value
-#            self.callback_counter += 1
-#
-#        cfunc_type = ctypes.CFUNCTYPE(ctypes.c_void_p, ctypes.POINTER(S7Object), ctypes.c_int, ctypes.c_int)
-#        self.client.set_as_callback(cfunc_type(callback), cObj)
-#        self.client.as_ct_write(0, 1, bytearray(expected))
-
-#        self._as_check_loop()
-#        self.assertEqual(expected, self.client.ct_read(0, 1))
-#        self.assertEqual(1, self.callback_counter)
-
-
 @pytest.mark.client
 class TestClientBeforeConnect(unittest.TestCase):
     """
     Test suite of items that should run without an open connection.
     """
 
     def setUp(self):
-        self.client = snap7.client.Client()
+        self.client = Client()
 
     def test_set_param(self):
         values = (
-            (snap7.types.RemotePort, 1102),
-            (snap7.types.PingTimeout, 800),
-            (snap7.types.SendTimeout, 15),
-            (snap7.types.RecvTimeout, 3500),
-            (snap7.types.SrcRef, 128),
-            (snap7.types.DstRef, 128),
-            (snap7.types.SrcTSap, 128),
-            (snap7.types.PDURequest, 470),
+            (RemotePort, 1102),
+            (PingTimeout, 800),
+            (SendTimeout, 15),
+            (RecvTimeout, 3500),
+            (SrcRef, 128),
+            (DstRef, 128),
+            (SrcTSap, 128),
+            (PDURequest, 470),
         )
         for param, value in values:
             self.client.set_param(param, value)
 
 
 @pytest.mark.client
 class TestLibraryIntegration(unittest.TestCase):
@@ -1045,27 +1050,31 @@
 
         # have load_library return another mock
         self.mocklib = mock.MagicMock()
         self.loadlib_func.return_value = self.mocklib
 
         # have the Cli_Create of the mock return None
         self.mocklib.Cli_Create.return_value = None
+        self.mocklib.Cli_Destroy.return_value = None
 
     def tearDown(self):
         # restore load_library
         self.loadlib_patch.stop()
 
     def test_create(self):
-        snap7.client.Client()
+        Client()
         self.mocklib.Cli_Create.assert_called_once()
 
-    @mock.patch("snap7.client.byref")
-    def test_gc(self, byref_mock):
-        client = snap7.client.Client()
-        client._pointer = 10
+    def test_gc(self):
+        client = Client()
         del client
         gc.collect()
         self.mocklib.Cli_Destroy.assert_called_once()
 
+    def test_context_manager(self):
+        with Client() as _:
+            pass
+        self.mocklib.Cli_Destroy.assert_called_once()
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `python_snap7-1.4/tests/test_logo_client.py` & `python_snap7-1.4.1/tests/test_logo_client.py`

 * *Files identical despite different names*

### Comparing `python_snap7-1.4/tests/test_mainloop.py` & `python_snap7-1.4.1/tests/test_mainloop.py`

 * *Files identical despite different names*

### Comparing `python_snap7-1.4/tests/test_partner.py` & `python_snap7-1.4.1/tests/test_partner.py`

 * *Files identical despite different names*

### Comparing `python_snap7-1.4/tests/test_server.py` & `python_snap7-1.4.1/tests/test_server.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import ctypes
+import gc
 import logging
 import pytest
 import unittest
 from unittest import mock
 
 from snap7.common import error_text
 from snap7.error import server_errors
@@ -152,27 +153,29 @@
 
         # have load_library return another mock
         self.mocklib = mock.MagicMock()
         self.loadlib_func.return_value = self.mocklib
 
         # have the Srv_Create of the mock return None
         self.mocklib.Srv_Create.return_value = None
+        self.mocklib.Srv_Destroy.return_value = None
 
     def tearDown(self):
         # restore load_library
         self.loadlib_patch.stop()
 
     def test_create(self):
-        Server(log=False)
-        self.mocklib.Srv_Create.assert_called_once()
-
-    def test_gc(self):
         server = Server(log=False)
         del server
-        self.mocklib.Srv_Destroy.assert_called_once()
+        gc.collect()
+        self.mocklib.Srv_Create.assert_called_once()
+
+    def test_context_manager(self):
+        with Server(log=False) as _:
+            pass
 
 
 if __name__ == "__main__":
     import logging
 
     logging.basicConfig()
     unittest.main()
```

### Comparing `python_snap7-1.4/tests/test_util.py` & `python_snap7-1.4.1/tests/test_util.py`

 * *Files identical despite different names*

