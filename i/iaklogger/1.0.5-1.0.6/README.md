# Comparing `tmp/iaklogger-1.0.5.tar.gz` & `tmp/iaklogger-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iaklogger-1.0.5.tar", last modified: Tue May  7 18:44:04 2024, max compression
+gzip compressed data, was "iaklogger-1.0.6.tar", last modified: Fri May 10 13:43:18 2024, max compression
```

## Comparing `iaklogger-1.0.5.tar` & `iaklogger-1.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:44:04.543305 iaklogger-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-07 18:44:04.543305 iaklogger-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-05-07 18:44:00.000000 iaklogger-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:44:04.543305 iaklogger-1.0.5/iaklogger/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-07 18:44:00.000000 iaklogger-1.0.5/iaklogger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-07 18:44:00.000000 iaklogger-1.0.5/iaklogger/iaklogger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-07 18:44:00.000000 iaklogger-1.0.5/iaklogger/test_iaklogger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:44:04.543305 iaklogger-1.0.5/iaklogger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-07 18:44:04.000000 iaklogger-1.0.5/iaklogger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-07 18:44:04.000000 iaklogger-1.0.5/iaklogger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 18:44:04.000000 iaklogger-1.0.5/iaklogger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-07 18:44:04.000000 iaklogger-1.0.5/iaklogger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-07 18:44:04.543305 iaklogger-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-07 18:44:00.000000 iaklogger-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:43:18.245875 iaklogger-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-10 13:43:18.245875 iaklogger-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-05-10 13:43:14.000000 iaklogger-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:43:18.245875 iaklogger-1.0.6/iaklogger/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-10 13:43:14.000000 iaklogger-1.0.6/iaklogger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-05-10 13:43:14.000000 iaklogger-1.0.6/iaklogger/iaklogger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-10 13:43:14.000000 iaklogger-1.0.6/iaklogger/test_iaklogger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:43:18.245875 iaklogger-1.0.6/iaklogger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-10 13:43:18.000000 iaklogger-1.0.6/iaklogger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-10 13:43:18.000000 iaklogger-1.0.6/iaklogger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 13:43:18.000000 iaklogger-1.0.6/iaklogger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-10 13:43:18.000000 iaklogger-1.0.6/iaklogger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-10 13:43:18.245875 iaklogger-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-10 13:43:14.000000 iaklogger-1.0.6/setup.py
```

### Comparing `iaklogger-1.0.5/PKG-INFO` & `iaklogger-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iaklogger
-Version: 1.0.5
+Version: 1.0.6
 Summary: Very basic and easy logger
 Home-page: https://github.com/Iakl/iaklogger
 Download-URL: https://github.com/Iakl/iaklogger/archive/refs/tags/v1.0.0.tar.gz
 Author: Iakl
 Author-email: estebaniakl@gmail.com
 License: MIT
 Keywords: logger,easy,print,log,basic,logging
```

### Comparing `iaklogger-1.0.5/README.md` & `iaklogger-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `iaklogger-1.0.5/iaklogger/iaklogger.py` & `iaklogger-1.0.6/iaklogger/iaklogger.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import time
+import warnings
 
 DEFAULT = "DEFAULT"  # prints default messages
 
 
 class OPTIONS:
     allowed_tags = []
     """list (Default: Empty): list of allowed tags. Tag DEFAULT is always allowed unless mute_default is true."""
@@ -52,14 +53,21 @@
         print(f"{time_str}{tags_str}{new_line_str}{printable_obj}")
         if OPTIONS.log_file:
             log_to_file(printable_obj)
         return True
 
 
 def log_to_file(printable_obj):
+    """
+    Logs the message to a file. The path to the file has to be set in the OPTIONS.log_file attribute.
+    Args:
+        printable_obj (str): Message to log.
+    Returns:
+        None
+    """
     printable_obj_size = len(printable_obj.encode('utf-8'))
     with open(OPTIONS.log_file, "a+") as f:
         f.seek(0, 2)  # Mueve el puntero al final del archivo
         if f.tell() + printable_obj_size < OPTIONS.log_file_max_size_mb * 1024 * 1024:
             f.write(printable_obj + "\n")
         else:
             f.seek(0)  # Mueve el puntero al principio del archivo
@@ -67,7 +75,25 @@
             total_size = sum(len(line.encode('utf-8')) for line in lines)
             while lines and total_size + printable_obj_size > OPTIONS.log_file_max_size_mb * 1024 * 1024:
                 total_size -= len(lines.pop(0).encode('utf-8'))
             f.seek(0)
             f.truncate()
             f.writelines(lines)
             f.write(printable_obj + "\n")
+
+
+def set_options(opts):
+    """
+    Set OPTIONS from the provided dictionary opts.
+
+    Parameters:
+        opts (dict): A dictionary containing the options to be set.
+
+    Returns:
+        None
+    """
+    if not isinstance(opts, dict):
+        raise TypeError("opts must be a dictionary")
+    for key, value in opts.items():
+        if key not in OPTIONS.__dict__:
+            warnings.warn(f"Option {key} not found in OPTIONS")
+        setattr(OPTIONS, key, value)
```

### Comparing `iaklogger-1.0.5/iaklogger/test_iaklogger.py` & `iaklogger-1.0.6/iaklogger/test_iaklogger.py`

 * *Files 16% similar despite different names*

```diff
@@ -38,28 +38,32 @@
     assert iak.log("Debug", tags=["DEBUG"]) == True
 
     # Test case 10: Log message with invalid tags
     iak.OPTIONS.allowed_tags = ["INFO", "WARNING"]
     assert iak.log("Invalid tag", tags=["ERROR", "DEBUG"]) == False
 
 
-iak.OPTIONS.allowed_tags = [
-    "FORECAST",
-    "RESULTS",
-    "OPTIMIZER",
-    "SOLVING",
-    "CONTINUOUS",
-    "SYSMANAGER",
-    "NETWORK",
-    "LOADING",
-    "UPDATE",
-    "DEBUG",
-    "TESTS",
-    "ERROR",
-    "INFO",
-    "WARNING",
-    "CONVERSATION",
-    "APP"
-]
-iak.OPTIONS.show_tags = True
+options = {
+    "allowed_tags": [
+        "FORECAST",
+        "RESULTS",
+        "OPTIMIZER",
+        "SOLVING",
+        "CONTINUOUS",
+        "SYSMANAGER",
+        "NETWORK",
+        "LOADING",
+        "UPDATE",
+        "DEBUG",
+        "TESTS",
+        "ERROR",
+        "INFO",
+        "WARNING",
+        "CONVERSATION",
+        "APP"
+    ],
+    "show_tags": True,
+}
+
+iak.set_options(options)
 
 test_log()
```

### Comparing `iaklogger-1.0.5/iaklogger.egg-info/PKG-INFO` & `iaklogger-1.0.6/iaklogger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iaklogger
-Version: 1.0.5
+Version: 1.0.6
 Summary: Very basic and easy logger
 Home-page: https://github.com/Iakl/iaklogger
 Download-URL: https://github.com/Iakl/iaklogger/archive/refs/tags/v1.0.0.tar.gz
 Author: Iakl
 Author-email: estebaniakl@gmail.com
 License: MIT
 Keywords: logger,easy,print,log,basic,logging
```

### Comparing `iaklogger-1.0.5/setup.py` & `iaklogger-1.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from distutils.core import setup
 setup(
     name='iaklogger',         # How you named your package folder (MyLib)
     packages=['iaklogger'],   # Chose the same as "name"
-    version='1.0.5',      # Start with a small number and increase it with every change you make
+    version='1.0.6',      # Start with a small number and increase it with every change you make
     # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     license='MIT',
     # Give a short description about your library
     description='Very basic and easy logger',
     long_description='Very basic and easy logger for python. It allows to print logs to the console and/or to a file. It also allows to mute logs by tags, mute all logs, show tags before the message, show time before the message, and set a maximum size for the log file.',
     author='Iakl',                   # Type in your name
     author_email='estebaniakl@gmail.com',      # Type in your E-Mail
```

