# Comparing `tmp/kayer_pretty_logger-1.2.0.tar.gz` & `tmp/kayer_pretty_logger-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kayer_pretty_logger-1.2.0.tar", last modified: Thu May  9 11:01:39 2024, max compression
+gzip compressed data, was "kayer_pretty_logger-1.2.1.tar", last modified: Fri May 10 12:08:33 2024, max compression
```

## Comparing `kayer_pretty_logger-1.2.0.tar` & `kayer_pretty_logger-1.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 11:01:39.938748 kayer_pretty_logger-1.2.0/
--rw-rw-rw-   0        0        0     4448 2024-05-09 11:01:39.924220 kayer_pretty_logger-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3866 2024-03-13 11:04:12.000000 kayer_pretty_logger-1.2.0/README.md
--rw-rw-rw-   0        0        0      108 2024-03-08 11:52:17.000000 kayer_pretty_logger-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0      742 2024-05-09 11:01:39.945268 kayer_pretty_logger-1.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-09 11:01:39.862035 kayer_pretty_logger-1.2.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-09 11:01:39.924220 kayer_pretty_logger-1.2.0/src/kayer_pretty_logger.egg-info/
--rw-rw-rw-   0        0        0     4448 2024-05-09 11:01:39.000000 kayer_pretty_logger-1.2.0/src/kayer_pretty_logger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      348 2024-05-09 11:01:39.000000 kayer_pretty_logger-1.2.0/src/kayer_pretty_logger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 11:01:39.000000 kayer_pretty_logger-1.2.0/src/kayer_pretty_logger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-09 11:01:39.000000 kayer_pretty_logger-1.2.0/src/kayer_pretty_logger.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-09 11:01:39.924220 kayer_pretty_logger-1.2.0/src/pretty_logger/
--rw-rw-rw-   0        0        0     5315 2024-05-09 10:59:15.000000 kayer_pretty_logger-1.2.0/src/pretty_logger/__init__.py
--rw-rw-rw-   0        0        0      566 2024-05-09 10:59:15.000000 kayer_pretty_logger-1.2.0/src/pretty_logger/constants.py
--rw-rw-rw-   0        0        0     1548 2024-05-09 10:59:15.000000 kayer_pretty_logger-1.2.0/src/pretty_logger/decorators.py
--rw-rw-rw-   0        0        0     4294 2024-05-09 10:59:28.000000 kayer_pretty_logger-1.2.0/src/pretty_logger/file_logger.py
+drwxrwxrwx   0        0        0        0 2024-05-10 12:08:33.024412 kayer_pretty_logger-1.2.1/
+-rw-rw-rw-   0        0        0     4448 2024-05-10 12:08:33.024412 kayer_pretty_logger-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3866 2024-03-13 11:04:12.000000 kayer_pretty_logger-1.2.1/README.md
+-rw-rw-rw-   0        0        0      108 2024-03-08 11:52:17.000000 kayer_pretty_logger-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0      742 2024-05-10 12:08:33.030805 kayer_pretty_logger-1.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-10 12:08:32.908067 kayer_pretty_logger-1.2.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-10 12:08:33.024412 kayer_pretty_logger-1.2.1/src/kayer_pretty_logger.egg-info/
+-rw-rw-rw-   0        0        0     4448 2024-05-10 12:08:32.000000 kayer_pretty_logger-1.2.1/src/kayer_pretty_logger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2024-05-10 12:08:32.000000 kayer_pretty_logger-1.2.1/src/kayer_pretty_logger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 12:08:32.000000 kayer_pretty_logger-1.2.1/src/kayer_pretty_logger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-10 12:08:32.000000 kayer_pretty_logger-1.2.1/src/kayer_pretty_logger.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 12:08:33.014777 kayer_pretty_logger-1.2.1/src/pretty_logger/
+-rw-rw-rw-   0        0        0     5468 2024-05-10 12:06:15.000000 kayer_pretty_logger-1.2.1/src/pretty_logger/__init__.py
+-rw-rw-rw-   0        0        0      566 2024-05-09 10:59:15.000000 kayer_pretty_logger-1.2.1/src/pretty_logger/constants.py
+-rw-rw-rw-   0        0        0     1548 2024-05-09 10:59:15.000000 kayer_pretty_logger-1.2.1/src/pretty_logger/decorators.py
+-rw-rw-rw-   0        0        0     4294 2024-05-09 10:59:28.000000 kayer_pretty_logger-1.2.1/src/pretty_logger/file_logger.py
```

### Comparing `kayer_pretty_logger-1.2.0/PKG-INFO` & `kayer_pretty_logger-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kayer-pretty-logger
-Version: 1.2.0
+Version: 1.2.1
 Summary: A pretty and colorful logger to emulate nest.js's logger and overwrite the python print function.
 Home-page: https://github.com/PilotKayer/pretty_logger
 Author: Kayer
 Author-email: devkayer@gmail.com
 Project-URL: Docs, https://github.com/PilotKayer/pretty_logger/blob/main/README.md
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `kayer_pretty_logger-1.2.0/README.md` & `kayer_pretty_logger-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `kayer_pretty_logger-1.2.0/setup.cfg` & `kayer_pretty_logger-1.2.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206b 6179 6572 2d70 7265 7474 792d   = kayer-pretty-
 00000020: 6c6f 6767 6572 0d0a 7665 7273 696f 6e20  logger..version 
-00000030: 3d20 312e 322e 300d 0a61 7574 686f 7220  = 1.2.0..author 
+00000030: 3d20 312e 322e 310d 0a61 7574 686f 7220  = 1.2.1..author 
 00000040: 3d20 4b61 7965 720d 0a61 7574 686f 725f  = Kayer..author_
 00000050: 656d 6169 6c20 3d20 6465 766b 6179 6572  email = devkayer
 00000060: 4067 6d61 696c 2e63 6f6d 0d0a 6465 7363  @gmail.com..desc
 00000070: 7269 7074 696f 6e20 3d20 4120 7072 6574  ription = A pret
 00000080: 7479 2061 6e64 2063 6f6c 6f72 6675 6c20  ty and colorful 
 00000090: 6c6f 6767 6572 2074 6f20 656d 756c 6174  logger to emulat
 000000a0: 6520 6e65 7374 2e6a 7327 7320 6c6f 6767  e nest.js's logg
```

### Comparing `kayer_pretty_logger-1.2.0/src/kayer_pretty_logger.egg-info/PKG-INFO` & `kayer_pretty_logger-1.2.1/src/kayer_pretty_logger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kayer-pretty-logger
-Version: 1.2.0
+Version: 1.2.1
 Summary: A pretty and colorful logger to emulate nest.js's logger and overwrite the python print function.
 Home-page: https://github.com/PilotKayer/pretty_logger
 Author: Kayer
 Author-email: devkayer@gmail.com
 Project-URL: Docs, https://github.com/PilotKayer/pretty_logger/blob/main/README.md
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `kayer_pretty_logger-1.2.0/src/pretty_logger/__init__.py` & `kayer_pretty_logger-1.2.1/src/pretty_logger/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #  Author:      Davide Alejandro Castejon (aka Kayer)
 #               devkayer@gmail.com
-
+import json
 from time import time
 from datetime import datetime
 from sys import argv, __stdout__
+from json import dumps
 
 from pretty_logger.constants import BColors
 from pretty_logger.file_logger import FileLogger
 
 
 def stringify_args(args: tuple[any, ...]) -> str:
     """
@@ -17,14 +18,17 @@
     :return: Concatenated str
     """
     output: str = ''
 
     for var in args:
         if type(var) is str:
             output += var + ' '
+        elif type(var) is dict:
+            pretty = dumps(var, indent=3)
+            output += "\n" + str(pretty)
         else:
             output += str(var) + ' '
 
     return output
 
 
 class Logger:
```

### Comparing `kayer_pretty_logger-1.2.0/src/pretty_logger/constants.py` & `kayer_pretty_logger-1.2.1/src/pretty_logger/constants.py`

 * *Files identical despite different names*

### Comparing `kayer_pretty_logger-1.2.0/src/pretty_logger/decorators.py` & `kayer_pretty_logger-1.2.1/src/pretty_logger/decorators.py`

 * *Files identical despite different names*

### Comparing `kayer_pretty_logger-1.2.0/src/pretty_logger/file_logger.py` & `kayer_pretty_logger-1.2.1/src/pretty_logger/file_logger.py`

 * *Files identical despite different names*

