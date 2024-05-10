# Comparing `tmp/observer_machine-0.0.1.tar.gz` & `tmp/observer_machine-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "observer_machine-0.0.1.tar", last modified: Fri May  3 01:29:08 2024, max compression
+gzip compressed data, was "observer_machine-0.0.2.tar", last modified: Fri May 10 19:07:27 2024, max compression
```

## Comparing `observer_machine-0.0.1.tar` & `observer_machine-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-03 01:29:08.659195 observer_machine-0.0.1/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1074 2024-05-03 01:25:26.000000 observer_machine-0.0.1/LICENSE
--rw-r--r--   0 alxfed    (1001) alxfed    (1001)      664 2024-05-03 01:29:08.659195 observer_machine-0.0.1/PKG-INFO
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      135 2024-05-03 01:28:15.000000 observer_machine-0.0.1/README.md
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      610 2024-05-03 01:28:15.000000 observer_machine-0.0.1/pyproject.toml
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2024-05-03 01:29:08.659195 observer_machine-0.0.1/setup.cfg
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-03 01:29:08.659195 observer_machine-0.0.1/src/
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-03 01:29:08.659195 observer_machine-0.0.1/src/observer_machine/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2024-05-03 01:25:26.000000 observer_machine-0.0.1/src/observer_machine/__init__.py
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-03 01:29:08.659195 observer_machine-0.0.1/src/observer_machine.egg-info/
--rw-r--r--   0 alxfed    (1001) alxfed    (1001)      664 2024-05-03 01:29:08.000000 observer_machine-0.0.1/src/observer_machine.egg-info/PKG-INFO
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      241 2024-05-03 01:29:08.000000 observer_machine-0.0.1/src/observer_machine.egg-info/SOURCES.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        1 2024-05-03 01:29:08.000000 observer_machine-0.0.1/src/observer_machine.egg-info/dependency_links.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       17 2024-05-03 01:29:08.000000 observer_machine-0.0.1/src/observer_machine.egg-info/top_level.txt
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-10 19:07:27.614084 observer_machine-0.0.2/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1074 2024-05-03 01:25:26.000000 observer_machine-0.0.2/LICENSE
+-rw-r--r--   0 alxfed    (1001) alxfed    (1001)      659 2024-05-10 19:07:27.614084 observer_machine-0.0.2/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      130 2024-05-10 19:06:26.000000 observer_machine-0.0.2/README.md
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      610 2024-05-10 19:06:26.000000 observer_machine-0.0.2/pyproject.toml
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2024-05-10 19:07:27.614084 observer_machine-0.0.2/setup.cfg
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-10 19:07:27.614084 observer_machine-0.0.2/src/
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-10 19:07:27.614084 observer_machine-0.0.2/src/observer_machine/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2024-05-03 01:25:26.000000 observer_machine-0.0.2/src/observer_machine/__init__.py
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-10 19:07:27.614084 observer_machine-0.0.2/src/observer_machine.egg-info/
+-rw-r--r--   0 alxfed    (1001) alxfed    (1001)      659 2024-05-10 19:07:27.000000 observer_machine-0.0.2/src/observer_machine.egg-info/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      241 2024-05-10 19:07:27.000000 observer_machine-0.0.2/src/observer_machine.egg-info/SOURCES.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        1 2024-05-10 19:07:27.000000 observer_machine-0.0.2/src/observer_machine.egg-info/dependency_links.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       17 2024-05-10 19:07:27.000000 observer_machine-0.0.2/src/observer_machine.egg-info/top_level.txt
```

### Comparing `observer_machine-0.0.1/LICENSE` & `observer_machine-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `observer_machine-0.0.1/PKG-INFO` & `observer_machine-0.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: observer-machine
-Version: 0.0.1
+Version: 0.0.2
 Summary: Observer.
 Author-email: Alexander Fedotov <alex.fedotov@aol.com>
 Project-URL: Homepage, https://github.com/observer-machine/observer-machine
 Project-URL: Bug Tracker, https://github.com/observer-machine/observer-machine/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Observer Machine
 Observer.
 <pre>
-  pip install <obse></obse>-machine
+  pip install observer-machine
 </pre>
 Then:
 ```Python
   # Python
   import observer_machine
 ```
```

### Comparing `observer_machine-0.0.1/pyproject.toml` & `observer_machine-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=67.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "observer-machine"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     {name="Alexander Fedotov", email="alex.fedotov@aol.com"},
 ]
 description = "Observer."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers=[
```

### Comparing `observer_machine-0.0.1/src/observer_machine.egg-info/PKG-INFO` & `observer_machine-0.0.2/src/observer_machine.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: observer-machine
-Version: 0.0.1
+Version: 0.0.2
 Summary: Observer.
 Author-email: Alexander Fedotov <alex.fedotov@aol.com>
 Project-URL: Homepage, https://github.com/observer-machine/observer-machine
 Project-URL: Bug Tracker, https://github.com/observer-machine/observer-machine/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Observer Machine
 Observer.
 <pre>
-  pip install <obse></obse>-machine
+  pip install observer-machine
 </pre>
 Then:
 ```Python
   # Python
   import observer_machine
 ```
```

