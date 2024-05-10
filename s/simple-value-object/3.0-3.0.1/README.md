# Comparing `tmp/simple_value_object-3.0.tar.gz` & `tmp/simple-value-object-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_value_object-3.0.tar", last modified: Sat Apr 13 21:21:15 2024, max compression
+gzip compressed data, was "simple-value-object-3.0.1.tar", last modified: Fri May 10 11:26:03 2024, max compression
```

## Comparing `simple_value_object-3.0.tar` & `simple-value-object-3.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 quique    (1000) quique    (1000)        0 2024-04-13 21:21:15.311469 simple_value_object-3.0/
--rw-rw-r--   0 quique    (1000) quique    (1000)      315 2024-04-13 16:21:10.000000 simple_value_object-3.0/AUTHORS
--rw-rw-r--   0 quique    (1000) quique    (1000)     1057 2024-04-13 16:21:10.000000 simple_value_object-3.0/LICENSE
--rw-r--r--   0 quique    (1000) quique    (1000)     3836 2024-04-13 21:21:15.307469 simple_value_object-3.0/PKG-INFO
--rw-rw-r--   0 quique    (1000) quique    (1000)     3107 2024-04-13 21:09:50.000000 simple_value_object-3.0/README.md
--rw-rw-r--   0 quique    (1000) quique    (1000)       38 2024-04-13 21:21:15.311469 simple_value_object-3.0/setup.cfg
--rw-rw-r--   0 quique    (1000) quique    (1000)      926 2024-04-13 21:20:52.000000 simple_value_object-3.0/setup.py
-drwxrwxr-x   0 quique    (1000) quique    (1000)        0 2024-04-13 21:21:15.307469 simple_value_object-3.0/simple_value_object/
--rw-rw-r--   0 quique    (1000) quique    (1000)      477 2024-04-13 20:49:58.000000 simple_value_object-3.0/simple_value_object/__init__.py
--rw-rw-r--   0 quique    (1000) quique    (1000)      233 2024-04-13 20:49:19.000000 simple_value_object-3.0/simple_value_object/decorators.py
--rw-rw-r--   0 quique    (1000) quique    (1000)      461 2024-04-13 20:49:45.000000 simple_value_object-3.0/simple_value_object/exceptions.py
--rw-rw-r--   0 quique    (1000) quique    (1000)     3725 2024-04-13 20:58:57.000000 simple_value_object-3.0/simple_value_object/value_object.py
-drwxrwxr-x   0 quique    (1000) quique    (1000)        0 2024-04-13 21:21:15.307469 simple_value_object-3.0/simple_value_object.egg-info/
--rw-r--r--   0 quique    (1000) quique    (1000)     3836 2024-04-13 21:21:15.000000 simple_value_object-3.0/simple_value_object.egg-info/PKG-INFO
--rw-rw-r--   0 quique    (1000) quique    (1000)      342 2024-04-13 21:21:15.000000 simple_value_object-3.0/simple_value_object.egg-info/SOURCES.txt
--rw-rw-r--   0 quique    (1000) quique    (1000)        1 2024-04-13 21:21:15.000000 simple_value_object-3.0/simple_value_object.egg-info/dependency_links.txt
--rw-rw-r--   0 quique    (1000) quique    (1000)       20 2024-04-13 21:21:15.000000 simple_value_object-3.0/simple_value_object.egg-info/top_level.txt
+drwxrwxr-x   0 quique    (1000) quique    (1000)        0 2024-05-10 11:26:03.498903 simple-value-object-3.0.1/
+-rw-rw-r--   0 quique    (1000) quique    (1000)      315 2024-04-13 16:21:10.000000 simple-value-object-3.0.1/AUTHORS
+-rw-rw-r--   0 quique    (1000) quique    (1000)     1057 2024-04-13 16:21:10.000000 simple-value-object-3.0.1/LICENSE
+-rw-rw-r--   0 quique    (1000) quique    (1000)     3842 2024-05-10 11:26:03.498903 simple-value-object-3.0.1/PKG-INFO
+-rw-rw-r--   0 quique    (1000) quique    (1000)     3091 2024-05-10 11:22:14.000000 simple-value-object-3.0.1/README.md
+-rw-rw-r--   0 quique    (1000) quique    (1000)       38 2024-05-10 11:26:03.498903 simple-value-object-3.0.1/setup.cfg
+-rw-rw-r--   0 quique    (1000) quique    (1000)      926 2024-04-13 21:26:13.000000 simple-value-object-3.0.1/setup.py
+drwxrwxr-x   0 quique    (1000) quique    (1000)        0 2024-05-10 11:26:03.498903 simple-value-object-3.0.1/simple_value_object/
+-rw-rw-r--   0 quique    (1000) quique    (1000)      477 2024-05-10 11:21:09.000000 simple-value-object-3.0.1/simple_value_object/__init__.py
+-rw-rw-r--   0 quique    (1000) quique    (1000)      233 2024-05-09 21:19:03.000000 simple-value-object-3.0.1/simple_value_object/decorators.py
+-rw-rw-r--   0 quique    (1000) quique    (1000)      461 2024-04-13 21:26:13.000000 simple-value-object-3.0.1/simple_value_object/exceptions.py
+-rw-rw-r--   0 quique    (1000) quique    (1000)     3699 2024-05-10 11:20:38.000000 simple-value-object-3.0.1/simple_value_object/value_object.py
+drwxrwxr-x   0 quique    (1000) quique    (1000)        0 2024-05-10 11:26:03.498903 simple-value-object-3.0.1/simple_value_object.egg-info/
+-rw-r--r--   0 quique    (1000) quique    (1000)     3842 2024-05-10 11:26:03.000000 simple-value-object-3.0.1/simple_value_object.egg-info/PKG-INFO
+-rw-rw-r--   0 quique    (1000) quique    (1000)      342 2024-05-10 11:26:03.000000 simple-value-object-3.0.1/simple_value_object.egg-info/SOURCES.txt
+-rw-rw-r--   0 quique    (1000) quique    (1000)        1 2024-05-10 11:26:03.000000 simple-value-object-3.0.1/simple_value_object.egg-info/dependency_links.txt
+-rw-rw-r--   0 quique    (1000) quique    (1000)       20 2024-05-10 11:26:03.000000 simple-value-object-3.0.1/simple_value_object.egg-info/top_level.txt
```

### Comparing `simple_value_object-3.0/LICENSE` & `simple-value-object-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_value_object-3.0/PKG-INFO` & `simple-value-object-3.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 Metadata-Version: 2.1
 Name: simple-value-object
-Version: 3.0
+Version: 3.0.1
 Summary: A simple library to create Value Objects
 Home-page: https://github.com/quiqueporta/value-object
-Download-URL: https://github.com/quiqueporta/simple-value-object/releases
 Author: Quique Porta
 Author-email: me@quiqueporta.com
 License: MIT/X11
+Download-URL: https://github.com/quiqueporta/simple-value-object/releases
 Keywords: python,ddd
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
 # Value Object
 
-![Version number](https://img.shields.io/badge/version-3.0.0-blue.svg) ![License MIT](https://img.shields.io/github/license/quiqueporta/simple-value-object) ![Python Version](https://img.shields.io/badge/python-3.7,_3.8,_3.9,_3.10,3.11,3.12-blue.svg)
+![Version number](https://img.shields.io/badge/version-3.0.1-blue.svg) ![License MIT](https://img.shields.io/github/license/quiqueporta/simple-value-object) ![Python Version](https://img.shields.io/badge/python-3.7,_3.8,_3.9,_3.10,3.11,3.12-blue.svg)
 
 Based on Ruby Gem by [NoFlopSquad](https://github.com/noflopsquad/value-object)
 
 A **value object** is a small object that represents a simple entity whose equality isn't based on identity:
 i.e. two value objects are equal when they have the same value, not necessarily being the same object.
 
 [Wikipedia](http://en.wikipedia.org/wiki/Value_object)
 
-## New version 3.0
+## New version 3.x
 
-This new version is a complete rewrite of the library, now it uses **dataclasses** to define the value objects.
-With this change we can use **type hints** to define the fields and the library will take care of the rest.
-Now you have autocomplete and **type checking** in your IDE. With the previous version you had not autocomplete nor type checking.
-You should be able to use this library with any version of python **3.7 or higher**.
+This new version is a complete rewrite of the library, now it uses data classes to define the value objects.
+With this change we can use type hints to define the fields and the library will take care of the rest.
+Now you have autocomplete and type checking in your IDE. With the previous version, you did no autocomplete or type-checking.
+You should be able to use this library with any version of Python 3.7 or higher.
 
 ## Installation
 
 ```sh
 pip install simple-value-object
 ```
 
@@ -175,7 +176,9 @@
 ```
 
 ## Tests
 
 ```sh
 docker/test
 ```
+
+
```

### Comparing `simple_value_object-3.0/README.md` & `simple-value-object-3.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # Value Object
 
-![Version number](https://img.shields.io/badge/version-3.0.0-blue.svg) ![License MIT](https://img.shields.io/github/license/quiqueporta/simple-value-object) ![Python Version](https://img.shields.io/badge/python-3.7,_3.8,_3.9,_3.10,3.11,3.12-blue.svg)
+![Version number](https://img.shields.io/badge/version-3.0.1-blue.svg) ![License MIT](https://img.shields.io/github/license/quiqueporta/simple-value-object) ![Python Version](https://img.shields.io/badge/python-3.7,_3.8,_3.9,_3.10,3.11,3.12-blue.svg)
 
 Based on Ruby Gem by [NoFlopSquad](https://github.com/noflopsquad/value-object)
 
 A **value object** is a small object that represents a simple entity whose equality isn't based on identity:
 i.e. two value objects are equal when they have the same value, not necessarily being the same object.
 
 [Wikipedia](http://en.wikipedia.org/wiki/Value_object)
 
-## New version 3.0
+## New version 3.x
 
-This new version is a complete rewrite of the library, now it uses **dataclasses** to define the value objects.
-With this change we can use **type hints** to define the fields and the library will take care of the rest.
-Now you have autocomplete and **type checking** in your IDE. With the previous version you had not autocomplete nor type checking.
-You should be able to use this library with any version of python **3.7 or higher**.
+This new version is a complete rewrite of the library, now it uses data classes to define the value objects.
+With this change we can use type hints to define the fields and the library will take care of the rest.
+Now you have autocomplete and type checking in your IDE. With the previous version, you did no autocomplete or type-checking.
+You should be able to use this library with any version of Python 3.7 or higher.
 
 ## Installation
 
 ```sh
 pip install simple-value-object
 ```
```

### Comparing `simple_value_object-3.0/setup.py` & `simple-value-object-3.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `simple_value_object-3.0/simple_value_object/value_object.py` & `simple-value-object-3.0.1/simple_value_object/value_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-import inspect
 import hashlib
-import sys
 from dataclasses import dataclass
 
 from .exceptions import (
     CannotBeChanged,
     InvariantMustReturnBool,
     InvariantViolation,
 )
```

### Comparing `simple_value_object-3.0/simple_value_object.egg-info/PKG-INFO` & `simple-value-object-3.0.1/simple_value_object.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 Metadata-Version: 2.1
 Name: simple-value-object
-Version: 3.0
+Version: 3.0.1
 Summary: A simple library to create Value Objects
 Home-page: https://github.com/quiqueporta/value-object
-Download-URL: https://github.com/quiqueporta/simple-value-object/releases
 Author: Quique Porta
 Author-email: me@quiqueporta.com
 License: MIT/X11
+Download-URL: https://github.com/quiqueporta/simple-value-object/releases
 Keywords: python,ddd
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
 # Value Object
 
-![Version number](https://img.shields.io/badge/version-3.0.0-blue.svg) ![License MIT](https://img.shields.io/github/license/quiqueporta/simple-value-object) ![Python Version](https://img.shields.io/badge/python-3.7,_3.8,_3.9,_3.10,3.11,3.12-blue.svg)
+![Version number](https://img.shields.io/badge/version-3.0.1-blue.svg) ![License MIT](https://img.shields.io/github/license/quiqueporta/simple-value-object) ![Python Version](https://img.shields.io/badge/python-3.7,_3.8,_3.9,_3.10,3.11,3.12-blue.svg)
 
 Based on Ruby Gem by [NoFlopSquad](https://github.com/noflopsquad/value-object)
 
 A **value object** is a small object that represents a simple entity whose equality isn't based on identity:
 i.e. two value objects are equal when they have the same value, not necessarily being the same object.
 
 [Wikipedia](http://en.wikipedia.org/wiki/Value_object)
 
-## New version 3.0
+## New version 3.x
 
-This new version is a complete rewrite of the library, now it uses **dataclasses** to define the value objects.
-With this change we can use **type hints** to define the fields and the library will take care of the rest.
-Now you have autocomplete and **type checking** in your IDE. With the previous version you had not autocomplete nor type checking.
-You should be able to use this library with any version of python **3.7 or higher**.
+This new version is a complete rewrite of the library, now it uses data classes to define the value objects.
+With this change we can use type hints to define the fields and the library will take care of the rest.
+Now you have autocomplete and type checking in your IDE. With the previous version, you did no autocomplete or type-checking.
+You should be able to use this library with any version of Python 3.7 or higher.
 
 ## Installation
 
 ```sh
 pip install simple-value-object
 ```
 
@@ -175,7 +176,9 @@
 ```
 
 ## Tests
 
 ```sh
 docker/test
 ```
+
+
```

