# Comparing `tmp/bdmc-0.1.4.tar.gz` & `tmp/bdmc-0.1.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdmc-0.1.4.tar", last modified: Fri May  3 08:33:16 2024, max compression
+gzip compressed data, was "bdmc-0.1.4a0.tar", last modified: Fri Apr 26 02:34:30 2024, max compression
```

## Comparing `bdmc-0.1.4.tar` & `bdmc-0.1.4a0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     5466 2024-05-03 08:32:56.103859 bdmc-0.1.4/README.md
--rw-r--r--   0        0        0      545 2024-05-03 08:33:16.659988 bdmc-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      526 2024-05-03 08:32:56.107859 bdmc-0.1.4/src/bdmc/__init__.py
--rw-r--r--   0        0        0      419 2024-05-03 08:32:56.107859 bdmc-0.1.4/src/bdmc/modules/cmd.py
--rw-r--r--   0        0        0    16964 2024-05-03 08:32:56.107859 bdmc-0.1.4/src/bdmc/modules/controller.py
--rw-r--r--   0        0        0     2266 2024-05-03 08:32:56.107859 bdmc-0.1.4/src/bdmc/modules/debug.py
--rw-r--r--   0        0        0      574 2024-05-03 08:32:56.107859 bdmc-0.1.4/src/bdmc/modules/logger.py
--rw-r--r--   0        0        0     1356 2024-05-03 08:32:56.107859 bdmc-0.1.4/src/bdmc/modules/port.py
--rw-r--r--   0        0        0     7404 2024-05-03 08:32:56.107859 bdmc-0.1.4/src/bdmc/modules/seriald.py
--rw-r--r--   0        0        0      682 2024-05-03 08:32:56.107859 bdmc-0.1.4/tests/find_tests.py
--rw-r--r--   0        0        0     4405 2024-05-03 08:32:56.107859 bdmc-0.1.4/tests/test_context.py
--rw-r--r--   0        0        0     1991 2024-05-03 08:32:56.107859 bdmc-0.1.4/tests/test_controller.py
--rw-r--r--   0        0        0     5780 1970-01-01 00:00:00.000000 bdmc-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     5296 2024-04-26 02:34:08.669059 bdmc-0.1.4a0/README.md
+-rw-r--r--   0        0        0      547 2024-04-26 02:34:30.017123 bdmc-0.1.4a0/pyproject.toml
+-rw-r--r--   0        0        0      526 2024-04-26 02:34:08.669059 bdmc-0.1.4a0/src/bdmc/__init__.py
+-rw-r--r--   0        0        0      133 2024-04-26 02:34:08.669059 bdmc-0.1.4a0/src/bdmc/modules/cmd.py
+-rw-r--r--   0        0        0    16964 2024-04-26 02:34:08.669059 bdmc-0.1.4a0/src/bdmc/modules/controller.py
+-rw-r--r--   0        0        0     2266 2024-04-26 02:34:08.669059 bdmc-0.1.4a0/src/bdmc/modules/debug.py
+-rw-r--r--   0        0        0      574 2024-04-26 02:34:08.669059 bdmc-0.1.4a0/src/bdmc/modules/logger.py
+-rw-r--r--   0        0        0     1356 2024-04-26 02:34:08.669059 bdmc-0.1.4a0/src/bdmc/modules/port.py
+-rw-r--r--   0        0        0     7404 2024-04-26 02:34:08.669059 bdmc-0.1.4a0/src/bdmc/modules/seriald.py
+-rw-r--r--   0        0        0      682 2024-04-26 02:34:08.669059 bdmc-0.1.4a0/tests/find_tests.py
+-rw-r--r--   0        0        0     4405 2024-04-26 02:34:08.673059 bdmc-0.1.4a0/tests/test_context.py
+-rw-r--r--   0        0        0     1991 2024-04-26 02:34:08.673059 bdmc-0.1.4a0/tests/test_controller.py
+-rw-r--r--   0        0        0     5612 1970-01-01 00:00:00.000000 bdmc-0.1.4a0/PKG-INFO
```

### Comparing `bdmc-0.1.4/README.md` & `bdmc-0.1.4a0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,26 +10,15 @@
 - [ ] More capable controller implementations that support more complicated control strategies.
 
 ## Install
 
 Install use pdm
 
 ```shell
-
-# install pdm
-python -m pip install pdm
-
-# config pdm
-pdm config pypi.url https://pypi.tuna.tsinghua.edu.cn/simple
-
-# for stable version
 pdm add bdmc 
-
-# for unstable version
-pdm add bdmc -pre
 ```
 
 ## QuickStart
 
 The minimal example is as below.
 
 ```python
@@ -124,15 +113,15 @@
         con.set_motors_speed([555] * 4)  # Switch to this case if the breaker has never returned a non-zero value
     case _:
         raise ValueError("should never be here")
 
 
 ```
 
-use `set_log_level` to silent the console to improve the performance in high pressure conditions
+use `set_log_level` to silent the console, this should improve the performance in high pressure conditions
 
 ```python
 from bdmc import set_log_level
 
 """
 Logging DEBUG - Debugging information, used for detailed development phase logs, typically with a value of 10.
 Logging INFO - Information message, used to inform the general program running status, with a value of 20.
```

### Comparing `bdmc-0.1.4/pyproject.toml` & `bdmc-0.1.4a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bdmc"
-version = "0.1.4"
+version = "0.1.4a0"
 description = "An api wrapper lib designed for the uptech BDMC divers"
 authors = [
     { name = "Whth", email = "88489697+Whth@users.noreply.github.com" },
 ]
 dependencies = [
     "pyserial>=3.5",
     "coloredlogs>=15.0.1",
```

### Comparing `bdmc-0.1.4/src/bdmc/__init__.py` & `bdmc-0.1.4a0/src/bdmc/__init__.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.4/src/bdmc/modules/controller.py` & `bdmc-0.1.4a0/src/bdmc/modules/controller.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.4/src/bdmc/modules/debug.py` & `bdmc-0.1.4a0/src/bdmc/modules/debug.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.4/src/bdmc/modules/logger.py` & `bdmc-0.1.4a0/src/bdmc/modules/logger.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.4/src/bdmc/modules/port.py` & `bdmc-0.1.4a0/src/bdmc/modules/port.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.4/src/bdmc/modules/seriald.py` & `bdmc-0.1.4a0/src/bdmc/modules/seriald.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.4/tests/find_tests.py` & `bdmc-0.1.4a0/tests/find_tests.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.4/tests/test_context.py` & `bdmc-0.1.4a0/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.4/tests/test_controller.py` & `bdmc-0.1.4a0/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.4/PKG-INFO` & `bdmc-0.1.4a0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdmc
-Version: 0.1.4
+Version: 0.1.4a0
 Summary: An api wrapper lib designed for the uptech BDMC divers
 Author-Email: Whth <88489697+Whth@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: pyserial>=3.5
 Requires-Dist: coloredlogs>=15.0.1
 Description-Content-Type: text/markdown
@@ -21,26 +21,15 @@
 - [ ] More capable controller implementations that support more complicated control strategies.
 
 ## Install
 
 Install use pdm
 
 ```shell
-
-# install pdm
-python -m pip install pdm
-
-# config pdm
-pdm config pypi.url https://pypi.tuna.tsinghua.edu.cn/simple
-
-# for stable version
 pdm add bdmc 
-
-# for unstable version
-pdm add bdmc -pre
 ```
 
 ## QuickStart
 
 The minimal example is as below.
 
 ```python
@@ -135,15 +124,15 @@
         con.set_motors_speed([555] * 4)  # Switch to this case if the breaker has never returned a non-zero value
     case _:
         raise ValueError("should never be here")
 
 
 ```
 
-use `set_log_level` to silent the console to improve the performance in high pressure conditions
+use `set_log_level` to silent the console, this should improve the performance in high pressure conditions
 
 ```python
 from bdmc import set_log_level
 
 """
 Logging DEBUG - Debugging information, used for detailed development phase logs, typically with a value of 10.
 Logging INFO - Information message, used to inform the general program running status, with a value of 20.
```

