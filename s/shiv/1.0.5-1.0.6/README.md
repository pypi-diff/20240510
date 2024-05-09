# Comparing `tmp/shiv-1.0.5.tar.gz` & `tmp/shiv-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shiv-1.0.5.tar", last modified: Mon Feb  5 17:37:23 2024, max compression
+gzip compressed data, was "shiv-1.0.6.tar", last modified: Thu May  9 22:05:17 2024, max compression
```

## Comparing `shiv-1.0.5.tar` & `shiv-1.0.6.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 lcarvalh  (5975) staff       (20)        0 2024-02-05 17:37:23.740559 shiv-1.0.5/
--rw-r--r--   0 lcarvalh  (5975) staff       (20)     1326 2023-09-07 16:19:21.000000 shiv-1.0.5/LICENSE
--rw-r--r--   0 lcarvalh  (5975) staff       (20)      155 2023-09-07 16:19:21.000000 shiv-1.0.5/MANIFEST.in
--rw-r--r--   0 lcarvalh  (5975) staff       (20)      174 2023-09-07 16:19:21.000000 shiv-1.0.5/NOTICE
--rw-r--r--   0 lcarvalh  (5975) staff       (20)     4727 2024-02-05 17:37:23.740125 shiv-1.0.5/PKG-INFO
--rw-r--r--   0 lcarvalh  (5975) staff       (20)     3826 2023-09-07 16:19:21.000000 shiv-1.0.5/README.md
-drwxr-xr-x   0 lcarvalh  (5975) staff       (20)        0 2024-02-05 17:37:23.574904 shiv-1.0.5/docs/
--rw-r--r--   0 lcarvalh  (5975) staff       (20)      731 2023-09-07 16:19:21.000000 shiv-1.0.5/docs/api.rst
--rw-r--r--   0 lcarvalh  (5975) staff       (20)     1192 2023-09-07 16:19:21.000000 shiv-1.0.5/docs/cli-reference.rst
--rw-r--r--   0 lcarvalh  (5975) staff       (20)     2008 2023-09-07 16:19:21.000000 shiv-1.0.5/docs/django.rst
--rw-r--r--   0 lcarvalh  (5975) staff       (20)     3015 2023-09-07 16:19:21.000000 shiv-1.0.5/docs/history.rst
--rw-r--r--   0 lcarvalh  (5975) staff       (20)    10914 2023-09-07 16:19:21.000000 shiv-1.0.5/docs/index.rst
--rw-r--r--   0 lcarvalh  (5975) staff       (20)      117 2023-09-07 16:19:21.000000 shiv-1.0.5/pyproject.toml
--rw-r--r--   0 lcarvalh  (5975) staff       (20)     1587 2024-02-05 17:37:23.743866 shiv-1.0.5/setup.cfg
-drwxr-xr-x   0 lcarvalh  (5975) staff       (20)        0 2024-02-05 17:37:23.544788 shiv-1.0.5/src/
-drwxr-xr-x   0 lcarvalh  (5975) staff       (20)        0 2024-02-05 17:37:23.579430 shiv-1.0.5/src/shiv/
--rw-r--r--   0 lcarvalh  (5975) staff       (20)       45 2024-02-05 17:27:20.000000 shiv-1.0.5/src/shiv/__init__.py
--rw-r--r--   0 lcarvalh  (5975) staff       (20)      139 2023-09-07 16:19:21.000000 shiv-1.0.5/src/shiv/__main__.py
--rw-r--r--   0 lcarvalh  (5975) staff       (20)       22 2024-02-05 17:27:32.000000 shiv-1.0.5/src/shiv/__version__.py
-drwxr-xr-x   0 lcarvalh  (5975) staff       (20)        0 2024-02-05 17:37:23.611357 shiv-1.0.5/src/shiv/bootstrap/
--rw-r--r--   0 lcarvalh  (5975) staff       (20)     8977 2023-09-07 16:19:21.000000 shiv-1.0.5/src/shiv/bootstrap/__init__.py
--rw-r--r--   0 lcarvalh  (5975) staff       (20)     2878 2023-09-07 16:19:21.000000 shiv-1.0.5/src/shiv/bootstrap/environment.py
--rw-r--r--   0 lcarvalh  (5975) staff       (20)     2063 2023-09-07 16:19:21.000000 shiv-1.0.5/src/shiv/bootstrap/filelock.py
--rw-r--r--   0 lcarvalh  (5975) staff       (20)     1762 2023-09-07 16:19:21.000000 shiv-1.0.5/src/shiv/bootstrap/interpreter.py
--rw-r--r--   0 lcarvalh  (5975) staff       (20)     7374 2024-02-05 17:27:20.000000 shiv-1.0.5/src/shiv/builder.py
--rw-r--r--   0 lcarvalh  (5975) staff       (20)     9521 2024-02-05 17:27:20.000000 shiv-1.0.5/src/shiv/cli.py
--rw-r--r--   0 lcarvalh  (5975) staff       (20)     1586 2023-09-07 16:19:21.000000 shiv-1.0.5/src/shiv/constants.py
--rw-r--r--   0 lcarvalh  (5975) staff       (20)     1010 2023-09-07 16:19:21.000000 shiv-1.0.5/src/shiv/info.py
--rw-r--r--   0 lcarvalh  (5975) staff       (20)     1983 2023-09-07 16:19:21.000000 shiv-1.0.5/src/shiv/pip.py
-drwxr-xr-x   0 lcarvalh  (5975) staff       (20)        0 2024-02-05 17:37:23.739088 shiv-1.0.5/src/shiv.egg-info/
--rw-r--r--   0 lcarvalh  (5975) staff       (20)     4727 2024-02-05 17:37:23.000000 shiv-1.0.5/src/shiv.egg-info/PKG-INFO
--rw-r--r--   0 lcarvalh  (5975) staff       (20)      817 2024-02-05 17:37:23.000000 shiv-1.0.5/src/shiv.egg-info/SOURCES.txt
--rw-r--r--   0 lcarvalh  (5975) staff       (20)        1 2024-02-05 17:37:23.000000 shiv-1.0.5/src/shiv.egg-info/dependency_links.txt
--rw-r--r--   0 lcarvalh  (5975) staff       (20)       66 2024-02-05 17:37:23.000000 shiv-1.0.5/src/shiv.egg-info/entry_points.txt
--rw-r--r--   0 lcarvalh  (5975) staff       (20)      106 2024-02-05 17:37:23.000000 shiv-1.0.5/src/shiv.egg-info/requires.txt
--rw-r--r--   0 lcarvalh  (5975) staff       (20)        5 2024-02-05 17:37:23.000000 shiv-1.0.5/src/shiv.egg-info/top_level.txt
-drwxr-xr-x   0 lcarvalh  (5975) staff       (20)        0 2024-02-05 17:37:23.725166 shiv-1.0.5/test/
--rw-r--r--   0 lcarvalh  (5975) staff       (20)      917 2023-09-07 16:19:21.000000 shiv-1.0.5/test/conftest.py
-drwxr-xr-x   0 lcarvalh  (5975) staff       (20)        0 2024-02-05 17:37:23.727878 shiv-1.0.5/test/package/
-drwxr-xr-x   0 lcarvalh  (5975) staff       (20)        0 2024-02-05 17:37:23.732743 shiv-1.0.5/test/package/hello/
--rw-r--r--   0 lcarvalh  (5975) staff       (20)       37 2023-09-07 16:19:21.000000 shiv-1.0.5/test/package/hello/__init__.py
--rwxr-xr-x   0 lcarvalh  (5975) staff       (20)       28 2023-09-07 16:19:21.000000 shiv-1.0.5/test/package/hello/script.sh
--rw-r--r--   0 lcarvalh  (5975) staff       (20)      200 2023-09-07 16:19:21.000000 shiv-1.0.5/test/package/setup.py
--rw-r--r--   0 lcarvalh  (5975) staff       (20)      342 2023-09-07 16:19:21.000000 shiv-1.0.5/test/test.zip
--rw-r--r--   0 lcarvalh  (5975) staff       (20)     6765 2023-09-07 16:19:21.000000 shiv-1.0.5/test/test_bootstrap.py
--rw-r--r--   0 lcarvalh  (5975) staff       (20)     2378 2023-09-07 16:19:21.000000 shiv-1.0.5/test/test_builder.py
--rw-r--r--   0 lcarvalh  (5975) staff       (20)    14303 2023-09-07 16:19:21.000000 shiv-1.0.5/test/test_cli.py
--rw-r--r--   0 lcarvalh  (5975) staff       (20)      379 2023-09-07 16:19:21.000000 shiv-1.0.5/test/test_pip.py
+drwxr-xr-x   0 lcarvalh  (5975) staff       (20)        0 2024-05-09 22:05:17.664230 shiv-1.0.6/
+-rw-r--r--   0 lcarvalh  (5975) staff       (20)     1326 2023-09-07 16:19:21.000000 shiv-1.0.6/LICENSE
+-rw-r--r--   0 lcarvalh  (5975) staff       (20)      155 2023-09-07 16:19:21.000000 shiv-1.0.6/MANIFEST.in
+-rw-r--r--   0 lcarvalh  (5975) staff       (20)      174 2023-09-07 16:19:21.000000 shiv-1.0.6/NOTICE
+-rw-r--r--   0 lcarvalh  (5975) staff       (20)     4727 2024-05-09 22:05:17.662927 shiv-1.0.6/PKG-INFO
+-rw-r--r--   0 lcarvalh  (5975) staff       (20)     3826 2023-09-07 16:19:21.000000 shiv-1.0.6/README.md
+drwxr-xr-x   0 lcarvalh  (5975) staff       (20)        0 2024-05-09 22:05:17.560051 shiv-1.0.6/docs/
+-rw-r--r--   0 lcarvalh  (5975) staff       (20)      731 2023-09-07 16:19:21.000000 shiv-1.0.6/docs/api.rst
+-rw-r--r--   0 lcarvalh  (5975) staff       (20)     1192 2023-09-07 16:19:21.000000 shiv-1.0.6/docs/cli-reference.rst
+-rw-r--r--   0 lcarvalh  (5975) staff       (20)     2008 2023-09-07 16:19:21.000000 shiv-1.0.6/docs/django.rst
+-rw-r--r--   0 lcarvalh  (5975) staff       (20)     3015 2023-09-07 16:19:21.000000 shiv-1.0.6/docs/history.rst
+-rw-r--r--   0 lcarvalh  (5975) staff       (20)    10914 2023-09-07 16:19:21.000000 shiv-1.0.6/docs/index.rst
+-rw-r--r--   0 lcarvalh  (5975) staff       (20)      117 2023-09-07 16:19:21.000000 shiv-1.0.6/pyproject.toml
+-rw-r--r--   0 lcarvalh  (5975) staff       (20)     1587 2024-05-09 22:05:17.665750 shiv-1.0.6/setup.cfg
+drwxr-xr-x   0 lcarvalh  (5975) staff       (20)        0 2024-05-09 22:05:17.533412 shiv-1.0.6/src/
+drwxr-xr-x   0 lcarvalh  (5975) staff       (20)        0 2024-05-09 22:05:17.591843 shiv-1.0.6/src/shiv/
+-rw-r--r--   0 lcarvalh  (5975) staff       (20)       45 2024-02-05 17:27:20.000000 shiv-1.0.6/src/shiv/__init__.py
+-rw-r--r--   0 lcarvalh  (5975) staff       (20)      139 2023-09-07 16:19:21.000000 shiv-1.0.6/src/shiv/__main__.py
+-rw-r--r--   0 lcarvalh  (5975) staff       (20)       22 2024-05-09 21:44:20.000000 shiv-1.0.6/src/shiv/__version__.py
+drwxr-xr-x   0 lcarvalh  (5975) staff       (20)        0 2024-05-09 22:05:17.620725 shiv-1.0.6/src/shiv/bootstrap/
+-rw-r--r--   0 lcarvalh  (5975) staff       (20)     8977 2023-09-07 16:19:21.000000 shiv-1.0.6/src/shiv/bootstrap/__init__.py
+-rw-r--r--   0 lcarvalh  (5975) staff       (20)     2878 2023-09-07 16:19:21.000000 shiv-1.0.6/src/shiv/bootstrap/environment.py
+-rw-r--r--   0 lcarvalh  (5975) staff       (20)     2063 2023-09-07 16:19:21.000000 shiv-1.0.6/src/shiv/bootstrap/filelock.py
+-rw-r--r--   0 lcarvalh  (5975) staff       (20)     1762 2023-09-07 16:19:21.000000 shiv-1.0.6/src/shiv/bootstrap/interpreter.py
+-rw-r--r--   0 lcarvalh  (5975) staff       (20)     7434 2024-05-09 21:37:54.000000 shiv-1.0.6/src/shiv/builder.py
+-rw-r--r--   0 lcarvalh  (5975) staff       (20)     9521 2024-02-05 17:27:20.000000 shiv-1.0.6/src/shiv/cli.py
+-rw-r--r--   0 lcarvalh  (5975) staff       (20)     1586 2023-09-07 16:19:21.000000 shiv-1.0.6/src/shiv/constants.py
+-rw-r--r--   0 lcarvalh  (5975) staff       (20)     1010 2023-09-07 16:19:21.000000 shiv-1.0.6/src/shiv/info.py
+-rw-r--r--   0 lcarvalh  (5975) staff       (20)     1983 2023-09-07 16:19:21.000000 shiv-1.0.6/src/shiv/pip.py
+drwxr-xr-x   0 lcarvalh  (5975) staff       (20)        0 2024-05-09 22:05:17.656628 shiv-1.0.6/src/shiv.egg-info/
+-rw-r--r--   0 lcarvalh  (5975) staff       (20)     4727 2024-05-09 22:05:17.000000 shiv-1.0.6/src/shiv.egg-info/PKG-INFO
+-rw-r--r--   0 lcarvalh  (5975) staff       (20)      817 2024-05-09 22:05:17.000000 shiv-1.0.6/src/shiv.egg-info/SOURCES.txt
+-rw-r--r--   0 lcarvalh  (5975) staff       (20)        1 2024-05-09 22:05:17.000000 shiv-1.0.6/src/shiv.egg-info/dependency_links.txt
+-rw-r--r--   0 lcarvalh  (5975) staff       (20)       66 2024-05-09 22:05:17.000000 shiv-1.0.6/src/shiv.egg-info/entry_points.txt
+-rw-r--r--   0 lcarvalh  (5975) staff       (20)      106 2024-05-09 22:05:17.000000 shiv-1.0.6/src/shiv.egg-info/requires.txt
+-rw-r--r--   0 lcarvalh  (5975) staff       (20)        5 2024-05-09 22:05:17.000000 shiv-1.0.6/src/shiv.egg-info/top_level.txt
+drwxr-xr-x   0 lcarvalh  (5975) staff       (20)        0 2024-05-09 22:05:17.646346 shiv-1.0.6/test/
+-rw-r--r--   0 lcarvalh  (5975) staff       (20)      917 2023-09-07 16:19:21.000000 shiv-1.0.6/test/conftest.py
+drwxr-xr-x   0 lcarvalh  (5975) staff       (20)        0 2024-05-09 22:05:17.650164 shiv-1.0.6/test/package/
+drwxr-xr-x   0 lcarvalh  (5975) staff       (20)        0 2024-05-09 22:05:17.655659 shiv-1.0.6/test/package/hello/
+-rw-r--r--   0 lcarvalh  (5975) staff       (20)       37 2023-09-07 16:19:21.000000 shiv-1.0.6/test/package/hello/__init__.py
+-rwxr-xr-x   0 lcarvalh  (5975) staff       (20)       28 2023-09-07 16:19:21.000000 shiv-1.0.6/test/package/hello/script.sh
+-rw-r--r--   0 lcarvalh  (5975) staff       (20)      200 2023-09-07 16:19:21.000000 shiv-1.0.6/test/package/setup.py
+-rw-r--r--   0 lcarvalh  (5975) staff       (20)      342 2023-09-07 16:19:21.000000 shiv-1.0.6/test/test.zip
+-rw-r--r--   0 lcarvalh  (5975) staff       (20)     6765 2023-09-07 16:19:21.000000 shiv-1.0.6/test/test_bootstrap.py
+-rw-r--r--   0 lcarvalh  (5975) staff       (20)     2378 2023-09-07 16:19:21.000000 shiv-1.0.6/test/test_builder.py
+-rw-r--r--   0 lcarvalh  (5975) staff       (20)    14303 2023-09-07 16:19:21.000000 shiv-1.0.6/test/test_cli.py
+-rw-r--r--   0 lcarvalh  (5975) staff       (20)      379 2023-09-07 16:19:21.000000 shiv-1.0.6/test/test_pip.py
```

### Comparing `shiv-1.0.5/LICENSE` & `shiv-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `shiv-1.0.5/PKG-INFO` & `shiv-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shiv
-Version: 1.0.5
+Version: 1.0.6
 Summary: A command line utility for building fully self contained Python zipapps.
 Home-page: https://github.com/linkedin/shiv
 Author: Loren Carvalho
 Author-email: loren@linkedin.com
 License: BSD License
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `shiv-1.0.5/README.md` & `shiv-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `shiv-1.0.5/docs/api.rst` & `shiv-1.0.6/docs/api.rst`

 * *Files identical despite different names*

### Comparing `shiv-1.0.5/docs/cli-reference.rst` & `shiv-1.0.6/docs/cli-reference.rst`

 * *Files identical despite different names*

### Comparing `shiv-1.0.5/docs/django.rst` & `shiv-1.0.6/docs/django.rst`

 * *Files identical despite different names*

### Comparing `shiv-1.0.5/docs/history.rst` & `shiv-1.0.6/docs/history.rst`

 * *Files identical despite different names*

### Comparing `shiv-1.0.5/docs/index.rst` & `shiv-1.0.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `shiv-1.0.5/setup.cfg` & `shiv-1.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `shiv-1.0.5/src/shiv/bootstrap/__init__.py` & `shiv-1.0.6/src/shiv/bootstrap/__init__.py`

 * *Files identical despite different names*

### Comparing `shiv-1.0.5/src/shiv/bootstrap/environment.py` & `shiv-1.0.6/src/shiv/bootstrap/environment.py`

 * *Files identical despite different names*

### Comparing `shiv-1.0.5/src/shiv/bootstrap/filelock.py` & `shiv-1.0.6/src/shiv/bootstrap/filelock.py`

 * *Files identical despite different names*

### Comparing `shiv-1.0.5/src/shiv/bootstrap/interpreter.py` & `shiv-1.0.6/src/shiv/bootstrap/interpreter.py`

 * *Files identical despite different names*

### Comparing `shiv-1.0.5/src/shiv/builder.py` & `shiv-1.0.6/src/shiv/builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,25 +26,25 @@
     import importlib.resources as importlib_resources  # type: ignore
 except ImportError:
     # noinspection PyUnresolvedReferences
     import importlib_resources  # type: ignore
 
 # N.B.: `importlib.resources.{contents,is_resource,path}` are deprecated in 3.11 and gone in 3.13.
 if sys.version_info < (3, 11):
-    def iter_package_files(package: Union[str, ModuleType]) -> Iterator[Path]:
+    def iter_package_files(package: Union[str, ModuleType]) -> Iterator[Tuple[Path, str]]:
         for bootstrap_file in importlib_resources.contents(bootstrap):
             if importlib_resources.is_resource(bootstrap, bootstrap_file):
                 with importlib_resources.path(bootstrap, bootstrap_file) as path:
-                    yield path
+                    yield (path, bootstrap_file)
 else:
-    def iter_package_files(package: Union[str, ModuleType]) -> Iterator[Path]:
+    def iter_package_files(package: Union[str, ModuleType]) -> Iterator[Tuple[Path, str]]:
         for resource in importlib_resources.files(package).iterdir():
             if resource.is_file():
                 with importlib_resources.as_file(resource) as path:
-                    yield path
+                    yield (path, resource.name)
 
 # Typical maximum length for a shebang line
 BINPRM_BUF_SIZE = 128
 
 # zipapp __main__.py template
 MAIN_TEMPLATE = """\
 # -*- coding: utf-8 -*-
@@ -160,20 +160,20 @@
                 # Now that we have a hash of all the source files, use it as our build id if the user did not
                 # specify a custom one.
                 env.build_id = contents_hash.hexdigest()
 
             # now let's add the shiv bootstrap code.
             bootstrap_target = Path("_bootstrap")
 
-            for path in iter_package_files(bootstrap):
+            for path, name in iter_package_files(bootstrap):
                 data = path.read_bytes()
 
                 write_to_zipapp(
                     archive,
-                    str(bootstrap_target / path.name),
+                    str(bootstrap_target / name),
                     data,
                     zipinfo_datetime,
                     compression,
                     stat=path.stat(),
                 )
 
             # Write environment info in json file.
```

### Comparing `shiv-1.0.5/src/shiv/cli.py` & `shiv-1.0.6/src/shiv/cli.py`

 * *Files identical despite different names*

### Comparing `shiv-1.0.5/src/shiv/constants.py` & `shiv-1.0.6/src/shiv/constants.py`

 * *Files identical despite different names*

### Comparing `shiv-1.0.5/src/shiv/info.py` & `shiv-1.0.6/src/shiv/info.py`

 * *Files identical despite different names*

### Comparing `shiv-1.0.5/src/shiv/pip.py` & `shiv-1.0.6/src/shiv/pip.py`

 * *Files identical despite different names*

### Comparing `shiv-1.0.5/src/shiv.egg-info/PKG-INFO` & `shiv-1.0.6/src/shiv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shiv
-Version: 1.0.5
+Version: 1.0.6
 Summary: A command line utility for building fully self contained Python zipapps.
 Home-page: https://github.com/linkedin/shiv
 Author: Loren Carvalho
 Author-email: loren@linkedin.com
 License: BSD License
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `shiv-1.0.5/src/shiv.egg-info/SOURCES.txt` & `shiv-1.0.6/src/shiv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shiv-1.0.5/test/conftest.py` & `shiv-1.0.6/test/conftest.py`

 * *Files identical despite different names*

### Comparing `shiv-1.0.5/test/test_bootstrap.py` & `shiv-1.0.6/test/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `shiv-1.0.5/test/test_builder.py` & `shiv-1.0.6/test/test_builder.py`

 * *Files identical despite different names*

### Comparing `shiv-1.0.5/test/test_cli.py` & `shiv-1.0.6/test/test_cli.py`

 * *Files identical despite different names*

