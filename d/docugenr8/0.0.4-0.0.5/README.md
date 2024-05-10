# Comparing `tmp/docugenr8-0.0.4.tar.gz` & `tmp/docugenr8-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docugenr8-0.0.4.tar", last modified: Fri May 10 19:59:34 2024, max compression
+gzip compressed data, was "docugenr8-0.0.5.tar", last modified: Fri May 10 20:17:51 2024, max compression
```

## Comparing `docugenr8-0.0.4.tar` & `docugenr8-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:59:34.760092 docugenr8-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-10 19:59:01.000000 docugenr8-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-10 19:59:34.760092 docugenr8-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-10 19:59:01.000000 docugenr8-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-10 19:59:01.000000 docugenr8-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 19:59:34.760092 docugenr8-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:59:34.756092 docugenr8-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:59:34.756092 docugenr8-0.0.4/src/docugenr8/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:59:01.000000 docugenr8-0.0.4/src/docugenr8/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7899 2024-05-10 19:59:01.000000 docugenr8-0.0.4/src/docugenr8/document.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:59:34.756092 docugenr8-0.0.4/src/docugenr8.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-10 19:59:34.000000 docugenr8-0.0.4/src/docugenr8.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-10 19:59:34.000000 docugenr8-0.0.4/src/docugenr8.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 19:59:34.000000 docugenr8-0.0.4/src/docugenr8.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-10 19:59:34.000000 docugenr8-0.0.4/src/docugenr8.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-10 19:59:34.000000 docugenr8-0.0.4/src/docugenr8.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:59:34.756092 docugenr8-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-10 19:59:01.000000 docugenr8-0.0.4/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 19:59:01.000000 docugenr8-0.0.4/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:17:51.191430 docugenr8-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-10 20:17:19.000000 docugenr8-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-10 20:17:51.191430 docugenr8-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-10 20:17:19.000000 docugenr8-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-10 20:17:19.000000 docugenr8-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 20:17:51.191430 docugenr8-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:17:51.187430 docugenr8-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:17:51.191430 docugenr8-0.0.5/src/docugenr8/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 20:17:19.000000 docugenr8-0.0.5/src/docugenr8/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-05-10 20:17:19.000000 docugenr8-0.0.5/src/docugenr8/document.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:17:51.191430 docugenr8-0.0.5/src/docugenr8.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-10 20:17:51.000000 docugenr8-0.0.5/src/docugenr8.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-10 20:17:51.000000 docugenr8-0.0.5/src/docugenr8.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 20:17:51.000000 docugenr8-0.0.5/src/docugenr8.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-10 20:17:51.000000 docugenr8-0.0.5/src/docugenr8.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-10 20:17:51.000000 docugenr8-0.0.5/src/docugenr8.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:17:51.191430 docugenr8-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-10 20:17:19.000000 docugenr8-0.0.5/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 20:17:19.000000 docugenr8-0.0.5/version.txt
```

### Comparing `docugenr8-0.0.4/LICENSE` & `docugenr8-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `docugenr8-0.0.4/PKG-INFO` & `docugenr8-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docugenr8
-Version: 0.0.4
+Version: 0.0.5
 Summary: Library for document creating
 Author-email: Vladimir Jovanovic <vladimirjo@protonmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `docugenr8-0.0.4/pyproject.toml` & `docugenr8-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `docugenr8-0.0.4/src/docugenr8/document.py` & `docugenr8-0.0.5/src/docugenr8/document.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,14 +254,20 @@
     def height(self):
         return self.__core_page._height
 
     @height.setter
     def height(self, height: float):
         self.__core_page._height = height
 
+    def add_content(
+        self,
+        content: object,
+    ) -> None:
+        self.__core_page.add_content(content)
+
 
 class DocAttributes:
     def __init__(
         self,
     ) -> None:
         pass
```

### Comparing `docugenr8-0.0.4/src/docugenr8.egg-info/PKG-INFO` & `docugenr8-0.0.5/src/docugenr8.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docugenr8
-Version: 0.0.4
+Version: 0.0.5
 Summary: Library for document creating
 Author-email: Vladimir Jovanovic <vladimirjo@protonmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `docugenr8-0.0.4/tests/test_init.py` & `docugenr8-0.0.5/tests/test_init.py`

 * *Files identical despite different names*

