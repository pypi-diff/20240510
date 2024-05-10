# Comparing `tmp/python_sysinformer-1.8.1.tar.gz` & `tmp/python_sysinformer-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_sysinformer-1.8.1.tar", max compression
+gzip compressed data, was "python_sysinformer-1.9.0.tar", max compression
```

## Comparing `python_sysinformer-1.8.1.tar` & `python_sysinformer-1.9.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    35149 2024-04-29 16:22:12.024822 python_sysinformer-1.8.1/LICENSE
--rw-r--r--   0        0        0     5404 2024-04-29 16:22:12.024822 python_sysinformer-1.8.1/README.md
--rw-r--r--   0        0        0     1623 2024-04-29 16:22:40.304932 python_sysinformer-1.8.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-29 16:22:12.028822 python_sysinformer-1.8.1/src/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 16:22:12.028822 python_sysinformer-1.8.1/src/config/__init__.py
--rw-r--r--   0        0        0     1102 2024-04-29 16:22:12.028822 python_sysinformer-1.8.1/src/config/config_parser.py
--rw-r--r--   0        0        0     1233 2024-04-29 16:22:12.028822 python_sysinformer-1.8.1/src/config/default_config.py
--rw-r--r--   0        0        0      221 2024-04-29 16:22:12.028822 python_sysinformer-1.8.1/src/constants.py
--rw-r--r--   0        0        0        0 2024-04-29 16:22:12.028822 python_sysinformer-1.8.1/src/core/__init__.py
--rw-r--r--   0        0        0     4448 2024-04-29 16:22:12.028822 python_sysinformer-1.8.1/src/core/containers.py
--rw-r--r--   0        0        0     6261 2024-04-29 16:22:12.028822 python_sysinformer-1.8.1/src/core/cpu.py
--rw-r--r--   0        0        0     2041 2024-04-29 16:22:12.028822 python_sysinformer-1.8.1/src/core/disks.py
--rw-r--r--   0        0        0     3745 2024-04-29 16:22:12.032822 python_sysinformer-1.8.1/src/core/latency.py
--rw-r--r--   0        0        0     5799 2024-04-29 16:22:12.032822 python_sysinformer-1.8.1/src/core/memory.py
--rw-r--r--   0        0        0     2597 2024-04-29 16:22:12.032822 python_sysinformer-1.8.1/src/core/networking.py
--rw-r--r--   0        0        0     2764 2024-04-29 16:22:12.032822 python_sysinformer-1.8.1/src/core/processes.py
--rw-r--r--   0        0        0     2605 2024-04-29 16:22:12.032822 python_sysinformer-1.8.1/src/core/services.py
--rw-r--r--   0        0        0     4865 2024-04-29 16:22:12.032822 python_sysinformer-1.8.1/src/core/system.py
--rw-r--r--   0        0        0     4417 2024-04-29 16:22:12.032822 python_sysinformer-1.8.1/src/main.py
--rw-r--r--   0        0        0        0 2024-04-29 16:22:12.032822 python_sysinformer-1.8.1/src/utilities/__init__.py
--rw-r--r--   0        0        0      442 2024-04-29 16:22:12.032822 python_sysinformer-1.8.1/src/utilities/exceptions.py
--rw-r--r--   0        0        0      560 2024-04-29 16:22:12.032822 python_sysinformer-1.8.1/src/utilities/utils.py
--rw-r--r--   0        0        0     6124 1970-01-01 00:00:00.000000 python_sysinformer-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-10 18:49:07.797009 python_sysinformer-1.9.0/LICENSE
+-rw-r--r--   0        0        0     5404 2024-05-10 18:49:07.797009 python_sysinformer-1.9.0/README.md
+-rw-r--r--   0        0        0     1623 2024-05-10 18:49:37.657249 python_sysinformer-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-10 18:49:07.801009 python_sysinformer-1.9.0/src/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 18:49:07.801009 python_sysinformer-1.9.0/src/config/__init__.py
+-rw-r--r--   0        0        0     1102 2024-05-10 18:49:07.801009 python_sysinformer-1.9.0/src/config/config_parser.py
+-rw-r--r--   0        0        0     1233 2024-05-10 18:49:07.801009 python_sysinformer-1.9.0/src/config/default_config.py
+-rw-r--r--   0        0        0      221 2024-05-10 18:49:07.801009 python_sysinformer-1.9.0/src/constants.py
+-rw-r--r--   0        0        0        0 2024-05-10 18:49:07.801009 python_sysinformer-1.9.0/src/core/__init__.py
+-rw-r--r--   0        0        0     4448 2024-05-10 18:49:07.801009 python_sysinformer-1.9.0/src/core/containers.py
+-rw-r--r--   0        0        0     6261 2024-05-10 18:49:07.801009 python_sysinformer-1.9.0/src/core/cpu.py
+-rw-r--r--   0        0        0     2041 2024-05-10 18:49:07.801009 python_sysinformer-1.9.0/src/core/disks.py
+-rw-r--r--   0        0        0     3745 2024-05-10 18:49:07.801009 python_sysinformer-1.9.0/src/core/latency.py
+-rw-r--r--   0        0        0     6395 2024-05-10 18:49:07.801009 python_sysinformer-1.9.0/src/core/memory.py
+-rw-r--r--   0        0        0     2597 2024-05-10 18:49:07.801009 python_sysinformer-1.9.0/src/core/networking.py
+-rw-r--r--   0        0        0     2764 2024-05-10 18:49:07.801009 python_sysinformer-1.9.0/src/core/processes.py
+-rw-r--r--   0        0        0     2605 2024-05-10 18:49:07.801009 python_sysinformer-1.9.0/src/core/services.py
+-rw-r--r--   0        0        0     4865 2024-05-10 18:49:07.801009 python_sysinformer-1.9.0/src/core/system.py
+-rw-r--r--   0        0        0     4417 2024-05-10 18:49:07.801009 python_sysinformer-1.9.0/src/main.py
+-rw-r--r--   0        0        0        0 2024-05-10 18:49:07.801009 python_sysinformer-1.9.0/src/utilities/__init__.py
+-rw-r--r--   0        0        0      442 2024-05-10 18:49:07.801009 python_sysinformer-1.9.0/src/utilities/exceptions.py
+-rw-r--r--   0        0        0      560 2024-05-10 18:49:07.801009 python_sysinformer-1.9.0/src/utilities/utils.py
+-rw-r--r--   0        0        0     6124 1970-01-01 00:00:00.000000 python_sysinformer-1.9.0/PKG-INFO
```

### Comparing `python_sysinformer-1.8.1/LICENSE` & `python_sysinformer-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.8.1/README.md` & `python_sysinformer-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.8.1/pyproject.toml` & `python_sysinformer-1.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-SysInformer"
-version = "1.8.1"
+version = "1.9.0"
 description = "A simple system information tool for Linux"
 authors = ["Timothy Bryant <timothybryant3@gmail.com>"]
 readme = "README.md"
 packages = [{include = "src", from = "."}]
 # classifiers = ["Private :: Do not Upload"]
 
 [tool.poetry.dependencies]
```

### Comparing `python_sysinformer-1.8.1/src/config/config_parser.py` & `python_sysinformer-1.9.0/src/config/config_parser.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.8.1/src/config/default_config.py` & `python_sysinformer-1.9.0/src/config/default_config.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.8.1/src/core/containers.py` & `python_sysinformer-1.9.0/src/core/containers.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.8.1/src/core/cpu.py` & `python_sysinformer-1.9.0/src/core/cpu.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.8.1/src/core/disks.py` & `python_sysinformer-1.9.0/src/core/disks.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.8.1/src/core/latency.py` & `python_sysinformer-1.9.0/src/core/latency.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.8.1/src/core/memory.py` & `python_sysinformer-1.9.0/src/core/memory.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import platform
 import re
 import subprocess
 
 from typing import Literal, Optional
 from tabulate import tabulate
+import psutil
 
 from src.utilities.utils import print_title
 
 
 def calculate_memory_usage(
     total: int, free: int, buffers: int, cached: int
 ) -> tuple[int, int, float]:
@@ -35,55 +36,59 @@
     if value_in_mb > 1000:
         return f"{value_in_mb / 1024:.2f}GB"
     else:
         return f"{value_in_mb}MB"
 
 
 def get_memory_info() -> (
-    tuple[str, str, float | Literal[0], str, str, float | Literal[0]]
+    tuple[str, str, float | Literal[0], float | Literal[0], str, str, float | Literal[0], float | Literal[0]]
 ):
     """Get memory information"""
     if platform.system() == "Darwin":
         return get_memory_info_macos()
     elif platform.system() == "Linux":
         try:
             mem_info = {
                 i.split()[0].rstrip(":"): int(i.split()[1])
                 for i in open("/proc/meminfo", encoding="UTF-8").readlines()
             }
         except (FileNotFoundError, PermissionError):
             # print(f"Error reading file '/proc/meminfo': {exception}")
-            return ("0MB", "0MB", 0, "0MB", "0MB", 0)
+            return ("0MB", "0MB", 0, 0, "0MB", "0MB", 0, 0)
 
         keys = ["MemTotal", "MemFree", "Buffers", "Cached", "SwapTotal", "SwapFree"]
         if any(key not in mem_info for key in keys):
             print("Not all keys found in '/proc/meminfo'")
-            return ("0MB", "0MB", 0, "0MB", "0MB", 0)
+            return ("0MB", "0MB", 0, 0, "0MB", "0MB", 0, 0)
 
-        total_memory, mem_free, mem_used_percentage = calculate_memory_usage(
+        total_memory, mem_free, mem_used_percentage_calc = calculate_memory_usage(
             mem_info["MemTotal"],
             mem_info["MemFree"],
             mem_info["Buffers"],
             mem_info["Cached"],
         )
 
-        swap_total, swap_free, swap_used_percentage = calculate_memory_usage(
+        memory_usage = psutil.virtual_memory().percent
+        swap_usage = psutil.swap_memory().percent
+        swap_total, swap_free, swap_used_percentage_calc = calculate_memory_usage(
             mem_info["SwapTotal"], mem_info["SwapFree"], 0, 0
         )
 
         return (
             format_memory_value(total_memory),
             format_memory_value(mem_free),
-            mem_used_percentage,
+            memory_usage,
+            mem_used_percentage_calc,
             format_memory_value(swap_total),
             format_memory_value(swap_free),
-            swap_used_percentage,
+            swap_usage,
+            swap_used_percentage_calc,
         )
     else:
-        return ("0MB", "0MB", 0, "0MB", "0MB", 0)
+        return ("0MB", "0MB", 0, 0, "0MB", "0MB", 0, 0)
 
 
 def get_total_memory_of_all_processes() -> float:
     """
     Get the total memory usage of all processes on macOS.
 
     Returns:
@@ -108,77 +113,83 @@
         except (ValueError, IndexError):
             rss = 0  # ignore...
         ps_total += rss
     return ps_total / 1024 / 1024 or 0
 
 
 def get_memory_info_macos() -> (
-    tuple[str, str, float | Literal[0], str, str, float | Literal[0]]
+    tuple[str, str, float | Literal[0], float | Literal[0], str, str, float | Literal[0], float | Literal[0]]
 ):
     """Get memory information on macOS"""
     try:
         sysctl_output = subprocess.check_output(["sysctl", "-n", "hw.memsize"]).decode()
     except (subprocess.CalledProcessError, PermissionError):
-        return ("0MB", "0MB", 0, "0MB", "0MB", 0)
+        return ("0MB", "0MB", 0, 0, "0MB", "0MB", 0, 0)
 
     total_memory = int(sysctl_output.strip()) // (1024 * 1024)  # Convert bytes to MB
 
     mem_usage_process = get_total_memory_of_all_processes()
     mem_free = round(total_memory - mem_usage_process)
-    mem_used_percentage = (
+    memory_usage = psutil.virtual_memory().percent
+    mem_used_percentage_calc = (
         ((total_memory - mem_free) / total_memory) * 100 if total_memory != 0 else 0
     )
 
     swap_output = subprocess.check_output(["sysctl", "-n", "vm.swapusage"]).decode()
     swap_stats = {
         k: float(v.replace("M", ""))
         for k, v in re.findall(r"(\w+) = (\d+\.?\d*)M", swap_output)
     }
     swap_total = swap_stats.get("total", 0)  # Already in MB
     swap_free = swap_stats.get("free", 0)  # Already in MB
-    swap_used_percentage = (
+    swap_usage = psutil.swap_memory().percent
+    swap_used_percentage_calc = (
         ((swap_total - swap_free) / swap_total) * 100 if swap_total != 0 else 0
     )
 
     return (
         format_memory_value(total_memory),
         format_memory_value(mem_free),
-        mem_used_percentage,
+        memory_usage,
+        mem_used_percentage_calc,
         format_memory_value(swap_total),
         format_memory_value(swap_free),
-        swap_used_percentage,
+        swap_usage,
+        swap_used_percentage_calc,
     )
 
 
 def show_warning_msg() -> Optional[str]:
     """
     Print the macOS warning message
     """
     if platform.system() == "Darwin":
-        return "\033[1mWARNING\033[0m: memory usage of all processes used to calculate free memory"
-    return "\033[1mWARNING\033[0m: memory usage derived from '/proc/meminfo'"
+        return "\033[1mWARNING\033[0m: calc memory usage derived from process info; sys usage from psutil"
+    return "\033[1mWARNING\033[0m: memory usage derived from '/proc/meminfo' and psutil"
 
 
 def print_memory_info() -> None:
     """
     Print the memory information table
     """
     # Memory
     (
         mem_total,
         mem_free,
-        mem_used_percentage,
+        memory_usage,
+        mem_used_percentage_calc,
         swap_total,
         swap_free,
-        swap_used_percentage,
+        swap_usage,
+        swap_used_percentage_calc,
     ) = get_memory_info()
 
     table = [
-        ["Memory", f"{mem_free}", f"{mem_total}", f"{mem_used_percentage:.2f}%"],
-        ["Swap", f"{swap_free}", f"{swap_total}", f"{swap_used_percentage:.2f}%"],
+        ["Memory", f"{mem_free}", f"{mem_total}", f"{mem_used_percentage_calc:.2f}%", f"{memory_usage:.2f}%"],
+        ["Swap", f"{swap_free}", f"{swap_total}", f"{swap_used_percentage_calc:.2f}%", f"{swap_usage:.2f}%"],
     ]
 
-    headers = ["Type", "Free", "Total", "Usage"]
+    headers = ["Type", "Free", "Total", "Calc Usage", "Sys Usage"]
 
     print_title("Memory Information")
     print(show_warning_msg())
     print(tabulate(table, headers, tablefmt="simple_grid"))
```

### Comparing `python_sysinformer-1.8.1/src/core/networking.py` & `python_sysinformer-1.9.0/src/core/networking.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.8.1/src/core/processes.py` & `python_sysinformer-1.9.0/src/core/processes.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.8.1/src/core/services.py` & `python_sysinformer-1.9.0/src/core/services.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.8.1/src/core/system.py` & `python_sysinformer-1.9.0/src/core/system.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.8.1/src/main.py` & `python_sysinformer-1.9.0/src/main.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.8.1/src/utilities/utils.py` & `python_sysinformer-1.9.0/src/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.8.1/PKG-INFO` & `python_sysinformer-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sysinformer
-Version: 1.8.1
+Version: 1.9.0
 Summary: A simple system information tool for Linux
 Author: Timothy Bryant
 Author-email: timothybryant3@gmail.com
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

