# Comparing `tmp/icsystemutils-0.0.1.tar.gz` & `tmp/icsystemutils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icsystemutils-0.0.1.tar", last modified: Wed May  1 11:46:15 2024, max compression
+gzip compressed data, was "icsystemutils-0.0.2.tar", last modified: Fri May 10 11:04:35 2024, max compression
```

## Comparing `icsystemutils-0.0.1.tar` & `icsystemutils-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,32 @@
-drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-01 11:46:15.347785 icsystemutils-0.0.1/
--rw-r--r--   0 jgrogan    (503) staff       (20)    34621 2024-04-11 07:38:39.000000 icsystemutils-0.0.1/LICENSE
--rw-r--r--   0 jgrogan    (503) staff       (20)     2306 2024-05-01 11:46:15.347630 icsystemutils-0.0.1/PKG-INFO
--rw-r--r--   0 jgrogan    (503) staff       (20)     1277 2024-05-01 11:42:02.000000 icsystemutils-0.0.1/README.md
--rw-r--r--   0 jgrogan    (503) staff       (20)     1855 2024-05-01 11:42:02.000000 icsystemutils-0.0.1/pyproject.toml
--rw-r--r--   0 jgrogan    (503) staff       (20)       93 2024-05-01 11:46:15.348378 icsystemutils-0.0.1/setup.cfg
-drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-01 11:46:15.317363 icsystemutils-0.0.1/src/
-drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-01 11:46:15.320491 icsystemutils-0.0.1/src/icsystemutils/
--rw-r--r--   0 jgrogan    (503) staff       (20)        0 2024-04-11 07:37:06.000000 icsystemutils-0.0.1/src/icsystemutils/__init__.py
-drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-01 11:46:15.344766 icsystemutils-0.0.1/src/icsystemutils/cpu/
--rw-r--r--   0 jgrogan    (503) staff       (20)        0 2024-04-11 07:56:16.000000 icsystemutils-0.0.1/src/icsystemutils/cpu/__init__.py
--rw-r--r--   0 jgrogan    (503) staff       (20)      586 2024-04-11 07:59:33.000000 icsystemutils-0.0.1/src/icsystemutils/cpu/cpu.py
--rw-r--r--   0 jgrogan    (503) staff       (20)      959 2024-04-11 08:04:08.000000 icsystemutils-0.0.1/src/icsystemutils/cpu/cpu_info.py
--rw-r--r--   0 jgrogan    (503) staff       (20)     2803 2024-05-01 11:42:02.000000 icsystemutils-0.0.1/src/icsystemutils/cpu/linux_cpu.py
--rw-r--r--   0 jgrogan    (503) staff       (20)     1527 2024-05-01 11:42:02.000000 icsystemutils-0.0.1/src/icsystemutils/cpu/mac_cpu.py
-drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-01 11:46:15.345409 icsystemutils-0.0.1/src/icsystemutils/network/
--rw-r--r--   0 jgrogan    (503) staff       (20)        0 2024-04-11 08:05:38.000000 icsystemutils-0.0.1/src/icsystemutils/network/__init__.py
--rw-r--r--   0 jgrogan    (503) staff       (20)      855 2024-05-01 11:42:02.000000 icsystemutils-0.0.1/src/icsystemutils/network/remote.py
-drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-01 11:46:15.346738 icsystemutils-0.0.1/src/icsystemutils.egg-info/
--rw-r--r--   0 jgrogan    (503) staff       (20)     2306 2024-05-01 11:46:15.000000 icsystemutils-0.0.1/src/icsystemutils.egg-info/PKG-INFO
--rw-r--r--   0 jgrogan    (503) staff       (20)      562 2024-05-01 11:46:15.000000 icsystemutils-0.0.1/src/icsystemutils.egg-info/SOURCES.txt
--rw-r--r--   0 jgrogan    (503) staff       (20)        1 2024-05-01 11:46:15.000000 icsystemutils-0.0.1/src/icsystemutils.egg-info/dependency_links.txt
--rw-r--r--   0 jgrogan    (503) staff       (20)       57 2024-05-01 11:46:15.000000 icsystemutils-0.0.1/src/icsystemutils.egg-info/requires.txt
--rw-r--r--   0 jgrogan    (503) staff       (20)       14 2024-05-01 11:46:15.000000 icsystemutils-0.0.1/src/icsystemutils.egg-info/top_level.txt
-drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-01 11:46:15.345990 icsystemutils-0.0.1/test/
--rw-r--r--   0 jgrogan    (503) staff       (20)      116 2024-05-01 11:42:02.000000 icsystemutils-0.0.1/test/test_cpu_info.py
--rw-r--r--   0 jgrogan    (503) staff       (20)      132 2024-05-01 11:42:02.000000 icsystemutils-0.0.1/test/test_remote_ping.py
+drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-10 11:04:35.774652 icsystemutils-0.0.2/
+-rw-r--r--   0 jgrogan    (503) staff       (20)    34621 2024-04-11 07:38:39.000000 icsystemutils-0.0.2/LICENSE
+-rw-r--r--   0 jgrogan    (503) staff       (20)     2313 2024-05-10 11:04:35.774515 icsystemutils-0.0.2/PKG-INFO
+-rw-r--r--   0 jgrogan    (503) staff       (20)     1277 2024-05-01 11:42:02.000000 icsystemutils-0.0.2/README.md
+-rw-r--r--   0 jgrogan    (503) staff       (20)     1967 2024-05-10 11:02:45.000000 icsystemutils-0.0.2/pyproject.toml
+-rw-r--r--   0 jgrogan    (503) staff       (20)       93 2024-05-10 11:04:35.775271 icsystemutils-0.0.2/setup.cfg
+drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-10 11:04:35.710524 icsystemutils-0.0.2/src/
+drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-10 11:04:35.737290 icsystemutils-0.0.2/src/icsystemutils/
+-rw-r--r--   0 jgrogan    (503) staff       (20)      141 2024-05-02 15:17:21.000000 icsystemutils-0.0.2/src/icsystemutils/__init__.py
+drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-10 11:04:35.757007 icsystemutils-0.0.2/src/icsystemutils/cluster/
+-rw-r--r--   0 jgrogan    (503) staff       (20)       42 2024-05-03 07:37:46.000000 icsystemutils-0.0.2/src/icsystemutils/cluster/__init__.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)      132 2024-05-03 07:37:46.000000 icsystemutils-0.0.2/src/icsystemutils/cluster/cluster_allocation.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)      290 2024-05-03 07:37:46.000000 icsystemutils-0.0.2/src/icsystemutils/cluster/node.py
+drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-10 11:04:35.770542 icsystemutils-0.0.2/src/icsystemutils/cpu/
+-rw-r--r--   0 jgrogan    (503) staff       (20)      169 2024-05-02 15:17:21.000000 icsystemutils-0.0.2/src/icsystemutils/cpu/__init__.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)     1903 2024-05-02 15:54:00.000000 icsystemutils-0.0.2/src/icsystemutils/cpu/cpu.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)     1265 2024-05-02 15:17:21.000000 icsystemutils-0.0.2/src/icsystemutils/cpu/cpu_info.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)     3019 2024-05-02 15:54:00.000000 icsystemutils-0.0.2/src/icsystemutils/cpu/linux_cpu.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)     1751 2024-05-02 15:54:00.000000 icsystemutils-0.0.2/src/icsystemutils/cpu/mac_cpu.py
+drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-10 11:04:35.771336 icsystemutils-0.0.2/src/icsystemutils/gpu/
+-rw-r--r--   0 jgrogan    (503) staff       (20)       27 2024-05-03 07:37:46.000000 icsystemutils-0.0.2/src/icsystemutils/gpu/__init__.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)       82 2024-05-03 07:37:46.000000 icsystemutils-0.0.2/src/icsystemutils/gpu/gpu.py
+drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-10 11:04:35.773004 icsystemutils-0.0.2/src/icsystemutils/network/
+-rw-r--r--   0 jgrogan    (503) staff       (20)       80 2024-05-02 15:17:21.000000 icsystemutils-0.0.2/src/icsystemutils/network/__init__.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)     1297 2024-05-10 07:54:19.000000 icsystemutils-0.0.2/src/icsystemutils/network/remote.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)        0 2024-05-10 07:54:19.000000 icsystemutils-0.0.2/src/icsystemutils/py.typed
+drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-10 11:04:35.773620 icsystemutils-0.0.2/src/icsystemutils.egg-info/
+-rw-r--r--   0 jgrogan    (503) staff       (20)     2313 2024-05-10 11:04:35.000000 icsystemutils-0.0.2/src/icsystemutils.egg-info/PKG-INFO
+-rw-r--r--   0 jgrogan    (503) staff       (20)      725 2024-05-10 11:04:35.000000 icsystemutils-0.0.2/src/icsystemutils.egg-info/SOURCES.txt
+-rw-r--r--   0 jgrogan    (503) staff       (20)        1 2024-05-10 11:04:35.000000 icsystemutils-0.0.2/src/icsystemutils.egg-info/dependency_links.txt
+-rw-r--r--   0 jgrogan    (503) staff       (20)       64 2024-05-10 11:04:35.000000 icsystemutils-0.0.2/src/icsystemutils.egg-info/requires.txt
+-rw-r--r--   0 jgrogan    (503) staff       (20)       14 2024-05-10 11:04:35.000000 icsystemutils-0.0.2/src/icsystemutils.egg-info/top_level.txt
```

### Comparing `icsystemutils-0.0.1/LICENSE` & `icsystemutils-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `icsystemutils-0.0.1/PKG-INFO` & `icsystemutils-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: icsystemutils
-Version: 0.0.1
+Version: 0.0.2
 Summary: Utilities for interacting with system resources, e.g. cpu, network etc.
 Author-email: "James Grogan, Irish Centre for High End Computing" <james.grogan@ichec.ie>
 Project-URL: Repository, https://git.ichec.ie/performance/toolshed/icsystemutils
 Project-URL: Homepage, https://git.ichec.ie/performance/toolshed/icsystemutils
 Keywords: System Utilities,HPC
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: System :: Distributed Computing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: fabric
+Requires-Dist: fabric>=3.2.2
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-sugar; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: mypy; extra == "test"
```

### Comparing `icsystemutils-0.0.1/README.md` & `icsystemutils-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `icsystemutils-0.0.1/pyproject.toml` & `icsystemutils-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "icsystemutils"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="James Grogan, Irish Centre for High End Computing", email="james.grogan@ichec.ie" },
 ]
 description = "Utilities for interacting with system resources, e.g. cpu, network etc."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -12,15 +12,15 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: OS Independent",
     "Topic :: System :: Distributed Computing"
 ]
 keywords = ["System Utilities", "HPC"]
 
-dependencies = ["fabric"]
+dependencies = ["fabric>=3.2.2"]
 
 [project.urls]
 Repository = "https://git.ichec.ie/performance/toolshed/icsystemutils"
 Homepage = "https://git.ichec.ie/performance/toolshed/icsystemutils"
 
 [project.optional-dependencies]
 test = [
@@ -31,14 +31,20 @@
     "mypy"
 ]
 
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
+[tool.setuptools.package-data]
+"icsystemutils" = ["py.typed"]
+
+[tool.setuptools.packages.find]
+where = ["src"]
+
 [tool.pytest.ini_options]
 testpaths = ["test",]
 log_cli = 1
 log_cli_level = "debug"
 
 [tool.mypy]
 ignore_missing_imports = true
@@ -59,15 +65,15 @@
 commands =
     pytest {posargs:test}
 
 [testenv:lint]
 description = run linters
 skip_install = true
 deps =
-    black==22.12
+    black
 commands = black {posargs:src}
 
 [testenv:style]
 description = run style check
 skip_install = true
 deps =
     flake8
```

### Comparing `icsystemutils-0.0.1/src/icsystemutils/cpu/cpu_info.py` & `icsystemutils-0.0.2/src/icsystemutils/cpu/cpu_info.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 import sys
 
 from .linux_cpu import ProcInfoReader
 from .mac_cpu import SysctlCpuReader
 
 
 class CpuInfo:
+    """Class to read and store system cpu information
 
-    """
-    If something fancier is needed there is https://github.com/pytorch/cpuinfo
+    Attributes:
+        physical_procs (dict): Collection of physical processor info
+        threads_per_core (:obj:`int`): Number of threads available per processor core
+        cores_per_node (:obj:`int`): Number of cores per compute node (network location)
     """
 
-    def __init__(self) -> None:
+    def __init__(
+        self,
+    ) -> None:
         self.physical_procs: dict = {}
         self.threads_per_core = 1
         self.cores_per_node = 1
 
         if sys.platform == "darwin":
             self.reader = SysctlCpuReader()
         else:
             self.reader = ProcInfoReader()
 
         self.read()
 
     def read(self):
+        """Read the processor information from the system."""
         self.reader.read()
-        self.refresh()
+        self._refresh()
 
-    def refresh(self):
+    def _refresh(self):
         if not self.physical_procs:
             return
 
         # This is assuming all processors have same number of cores
         # and all cores have same number of threads
         self.cores_per_node = len(self.physical_procs.values()[0].cores)
         self.threads_per_core = len(
```

### Comparing `icsystemutils-0.0.1/src/icsystemutils/cpu/linux_cpu.py` & `icsystemutils-0.0.2/src/icsystemutils/cpu/linux_cpu.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,55 @@
 from pathlib import Path
 
 from .cpu import PhysicalProcessor
 
 
 class ProcInfoReader:
+    """Class to read and store cpu information using the Linux "/proc/cpuinfo" file"""
+
     def __init__(self, path: None | Path = None) -> None:
         if path:
             self.path = path
         else:
             self.path = Path("/proc/cpuinfo")
-        self.init()
+        self._init()
+
+    def read(self, content: str | None = None) -> dict[int, PhysicalProcessor]:
+        self._init()
+
+        if not content:
+            with open(self.path, "r") as f:
+                lines = f.readlines()
+        else:
+            lines = content.splitlines()
+
+        offset = 0
+        while offset < len(lines):
+            offset += self._read_block(lines[offset:])
+
+        self._populate_processors()
+        return self.processors
 
-    def init(self):
+    def _init(self):
         self.blocks = []
         self.processors = {}
 
-    def get_key_value(self, line):
+    def _get_key_value(self, line) -> tuple:
         key, value = line.split(":")
         return key.strip(), value.strip()
 
-    def read_block(self, content):
+    def _read_block(self, content):
         offset = 0
 
         block = {}
         for line in content:
             stripped_line = line.strip()
             if not stripped_line:
                 break
-            key, value = self.get_key_value(stripped_line)
+            key, value = self._get_key_value(stripped_line)
             block[key] = value
             offset += 1
 
         if offset > 0:
             self.blocks.append(block)
         return offset + 1
 
@@ -46,47 +64,33 @@
         if "cpu cores" in block:
             self.cpu_cores = int(block["cpu cores"])
         self.processors[id] = proc
 
     def _on_new_core(self, physical_id, core_id):
         self.processors[physical_id].add_core(core_id)
 
-    def on_new_thread(self, physical_id, core_id, thread_id):
+    def _on_new_thread(self, physical_id, core_id, thread_id):
         self.processors[physical_id].cores[core_id].add_thread(thread_id)
 
     def _populate_processors(self):
         for block in self.blocks:
             if "physical id" in block:
-                physical_id = block["physical id"]
+                physical_id = int(block["physical id"])
             else:
                 physical_id = 0
             if physical_id not in self.processors:
                 self._on_new_physical_proc(physical_id, block)
 
             if "core id" in block:
-                core_id = block["core id"]
+                core_id = int(block["core id"])
             else:
                 core_id = 0
             if core_id not in self.processors[physical_id].cores:
                 self._on_new_core(physical_id, core_id)
 
             if "processor" in block:
-                processor_id = block["processor"]
+                processor_id = int(block["processor"])
             else:
                 processor_id = 0
             threads = self.processors[physical_id].cores[core_id].threads
             if processor_id not in threads:
-                self.on_new_thread(physical_id, core_id, processor_id)
-
-    def read(self, content=None):
-        self.init()
-
-        if not content:
-            with open(self.path, "r") as f:
-                content = f.readlines()
-
-        offset = 0
-        while offset < len(content):
-            offset += self.read_block(content[offset:])
-
-        self._populate_processors()
-        return self.processors
+                self._on_new_thread(physical_id, core_id, processor_id)
```

### Comparing `icsystemutils-0.0.1/src/icsystemutils/cpu/mac_cpu.py` & `icsystemutils-0.0.2/src/icsystemutils/cpu/mac_cpu.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,54 @@
 import subprocess
 from pathlib import Path
 
 from .cpu import PhysicalProcessor
 
 
 class SysctlCpuReader:
+    """Class to read and store cpu information using the BSD sysctl utility
+
+    See https://man.freebsd.org/cgi/man.cgi?sysctl(8) for sysctl info
+    """
+
     def __init__(self) -> None:
         self.sysctl_path = Path("/usr/sbin/sysctl")
 
-    def read_sysctl_key(self, key: str):
-        # https://man.freebsd.org/cgi/man.cgi?sysctl(8)
+    def read(self, content: str | None = None) -> dict[int, PhysicalProcessor]:
+        if not content:
+            content = self._read_sysctl_key("machdep.cpu")
+        return self._parse_machdep_cpu(content)
+
+    def _read_sysctl_key(self, key: str) -> str:
         ret = subprocess.check_output([str(self.sysctl_path), key])
         return ret.decode("utf-8").strip()
 
-    def read(self):
-        machdep_cpu = self.read_sysctl_key("machdep.cpu")
-        return self._parse_machdep_cpu(machdep_cpu)
-
-    def get_key_value(self, line: str):
+    def _get_key_value(self, line: str) -> tuple:
         key, value = line.split(":")
         return key.strip(), value.strip()
 
-    def _parse_machdep_cpu(self, content: str):
+    def _parse_machdep_cpu(self, content: str) -> dict[int, PhysicalProcessor]:
         dict = {}
         for line in content.splitlines():
-            key, value = self.get_key_value(line)
-            key_no_prefix = key[len("machdep.cpu") :]
+            key, value = self._get_key_value(line)
+            key_no_prefix = key[len("machdep.cpu.") :]
             dict[key_no_prefix] = value
 
-        proc = PhysicalProcessor("0")
+        proc = PhysicalProcessor(0)
         if "brand_string" in dict:
             proc.model = dict["brand_string"]
 
         core_count = 1
         if "core_count" in dict:
             core_count = int(dict["core_count"])
 
         for idx in range(core_count):
-            proc.add_core(str(idx))
+            proc.add_core(idx)
 
         thread_count = 1
         if "thread_count" in dict:
             thread_count = int(dict["thread_count"])
         threads_per_core = int(thread_count / core_count)
         for core in proc.cores.values():
             for idx in range(threads_per_core):
                 core.add_thread(idx)
-        return {"0": proc}
+        return {0: proc}
```

### Comparing `icsystemutils-0.0.1/src/icsystemutils.egg-info/PKG-INFO` & `icsystemutils-0.0.2/src/icsystemutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: icsystemutils
-Version: 0.0.1
+Version: 0.0.2
 Summary: Utilities for interacting with system resources, e.g. cpu, network etc.
 Author-email: "James Grogan, Irish Centre for High End Computing" <james.grogan@ichec.ie>
 Project-URL: Repository, https://git.ichec.ie/performance/toolshed/icsystemutils
 Project-URL: Homepage, https://git.ichec.ie/performance/toolshed/icsystemutils
 Keywords: System Utilities,HPC
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: System :: Distributed Computing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: fabric
+Requires-Dist: fabric>=3.2.2
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-sugar; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: mypy; extra == "test"
```

### Comparing `icsystemutils-0.0.1/src/icsystemutils.egg-info/SOURCES.txt` & `icsystemutils-0.0.2/src/icsystemutils.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 src/icsystemutils/__init__.py
+src/icsystemutils/py.typed
 src/icsystemutils.egg-info/PKG-INFO
 src/icsystemutils.egg-info/SOURCES.txt
 src/icsystemutils.egg-info/dependency_links.txt
 src/icsystemutils.egg-info/requires.txt
 src/icsystemutils.egg-info/top_level.txt
+src/icsystemutils/cluster/__init__.py
+src/icsystemutils/cluster/cluster_allocation.py
+src/icsystemutils/cluster/node.py
 src/icsystemutils/cpu/__init__.py
 src/icsystemutils/cpu/cpu.py
 src/icsystemutils/cpu/cpu_info.py
 src/icsystemutils/cpu/linux_cpu.py
 src/icsystemutils/cpu/mac_cpu.py
+src/icsystemutils/gpu/__init__.py
+src/icsystemutils/gpu/gpu.py
 src/icsystemutils/network/__init__.py
-src/icsystemutils/network/remote.py
-test/test_cpu_info.py
-test/test_remote_ping.py
+src/icsystemutils/network/remote.py
```

