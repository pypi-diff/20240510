# Comparing `tmp/indent-concluder-1.1.1.tar.gz` & `tmp/indent-concluder-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indent-concluder-1.1.1.tar", last modified: Fri May 10 12:34:40 2024, max compression
+gzip compressed data, was "indent-concluder-1.1.2.tar", last modified: Fri May 10 12:46:52 2024, max compression
```

## Comparing `indent-concluder-1.1.1.tar` & `indent-concluder-1.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:34:40.130120 indent-concluder-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-10 12:34:40.130120 indent-concluder-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-10 12:34:32.000000 indent-concluder-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:34:40.130120 indent-concluder-1.1.1/indent_concluder/
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-05-10 12:34:32.000000 indent-concluder-1.1.1/indent_concluder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:34:40.130120 indent-concluder-1.1.1/indent_concluder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-10 12:34:40.000000 indent-concluder-1.1.1/indent_concluder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-10 12:34:40.000000 indent-concluder-1.1.1/indent_concluder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 12:34:40.000000 indent-concluder-1.1.1/indent_concluder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-10 12:34:40.000000 indent-concluder-1.1.1/indent_concluder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-10 12:34:40.000000 indent-concluder-1.1.1/indent_concluder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-10 12:34:40.134120 indent-concluder-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-10 12:34:32.000000 indent-concluder-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:46:52.465339 indent-concluder-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-10 12:46:52.465339 indent-concluder-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-10 12:46:46.000000 indent-concluder-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:46:52.465339 indent-concluder-1.1.2/indent_concluder/
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-05-10 12:46:46.000000 indent-concluder-1.1.2/indent_concluder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:46:52.465339 indent-concluder-1.1.2/indent_concluder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-10 12:46:52.000000 indent-concluder-1.1.2/indent_concluder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-10 12:46:52.000000 indent-concluder-1.1.2/indent_concluder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 12:46:52.000000 indent-concluder-1.1.2/indent_concluder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-10 12:46:52.000000 indent-concluder-1.1.2/indent_concluder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-10 12:46:52.000000 indent-concluder-1.1.2/indent_concluder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-10 12:46:52.465339 indent-concluder-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-10 12:46:46.000000 indent-concluder-1.1.2/setup.py
```

### Comparing `indent-concluder-1.1.1/PKG-INFO` & `indent-concluder-1.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indent-concluder
-Version: 1.1.1
+Version: 1.1.2
 Summary: UNKNOWN
 Home-page: https://github.com/EvATive7/indent-concluder
 Author: EvATive7
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `indent-concluder-1.1.1/indent_concluder/__init__.py` & `indent-concluder-1.1.2/indent_concluder/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,19 +29,19 @@
     def succeed(self, value: bool):
         self._succeed = value
 
     def __str__(self) -> str:
         return self._get_str(0)
 
     def failed_markdown(self, succeed_symbol=False):
-        list_: list[str] = self._get_summaries(succeed_symbol=succeed_symbol)
+        list_: list[str] = self._get_summaries([], succeed_symbol=succeed_symbol)
         list_ = [' - '+_s for _s in list_]
         return '\n'.join(list_)
 
-    def _get_summaries(self, prefixs: list[str] = [], succeed_symbol: bool = False) -> list[str]:
+    def _get_summaries(self, prefixs: list[str], succeed_symbol: bool = False) -> list[str]:
         def prefixed(item: Item, _prefixs: list[str]):
             result = ''
             for prefix in _prefixs:
                 result += f'[{prefix}]'
             if succeed_symbol:
                 result += f' {item.succeed_symbol}: {item.reason}'
             else:
@@ -51,15 +51,15 @@
         prefixs = prefixs + [self.name]
         result = []
         for child in self.children:
             if child.meta:
                 if not child.succeed:
                     result.append(prefixed(child, prefixs + [child.name]))
             else:
-                result += child._get_summaries(succeed_symbol=succeed_symbol)
+                result += child._get_summaries(prefixs=prefixs, succeed_symbol=succeed_symbol)
         return result
 
     def _get_str(self, indent=0):
         succeed_symbol = '√' if self.succeed else '×'
         meta = self.meta
 
         indent_str = ' ' * indent
```

### Comparing `indent-concluder-1.1.1/indent_concluder.egg-info/PKG-INFO` & `indent-concluder-1.1.2/indent_concluder.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indent-concluder
-Version: 1.1.1
+Version: 1.1.2
 Summary: UNKNOWN
 Home-page: https://github.com/EvATive7/indent-concluder
 Author: EvATive7
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `indent-concluder-1.1.1/setup.py` & `indent-concluder-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="indent-concluder",
-    version="1.1.1",
+    version="1.1.2",
     author="EvATive7",
     author_email="",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/EvATive7/indent-concluder",
     packages=setuptools.find_packages(),
     install_requires=[],
```

