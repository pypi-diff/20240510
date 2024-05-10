# Comparing `tmp/FasterAPI-0.0.8.tar.gz` & `tmp/FasterAPI-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FasterAPI-0.0.8.tar", last modified: Mon Dec 18 04:34:36 2023, max compression
+gzip compressed data, was "FasterAPI-0.0.9.tar", last modified: Mon Dec 18 08:16:00 2023, max compression
```

## Comparing `FasterAPI-0.0.8.tar` & `FasterAPI-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-12-18 04:34:36.439427 FasterAPI-0.0.8/
-drwxrwxrwx   0        0        0        0 2023-12-18 04:34:36.419195 FasterAPI-0.0.8/FasterAPI/
--rw-rw-rw-   0        0        0     2618 2023-12-18 02:22:32.000000 FasterAPI-0.0.8/FasterAPI/__init__.py
--rw-rw-rw-   0        0        0     1426 2023-12-18 04:33:28.000000 FasterAPI-0.0.8/FasterAPI/app.py
--rw-rw-rw-   0        0        0      702 2023-12-01 07:11:05.000000 FasterAPI-0.0.8/FasterAPI/models.py
--rw-rw-rw-   0        0        0     5381 2023-12-01 16:48:01.000000 FasterAPI-0.0.8/FasterAPI/router.py
--rw-rw-rw-   0        0        0      451 2023-12-01 06:34:20.000000 FasterAPI-0.0.8/FasterAPI/schemas.py
--rw-rw-rw-   0        0        0     4816 2023-12-18 02:22:32.000000 FasterAPI-0.0.8/FasterAPI/utils.py
-drwxrwxrwx   0        0        0        0 2023-12-18 04:34:36.435416 FasterAPI-0.0.8/FasterAPI.egg-info/
--rw-rw-rw-   0        0        0     3814 2023-12-18 04:34:36.000000 FasterAPI-0.0.8/FasterAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-12-18 04:34:36.000000 FasterAPI-0.0.8/FasterAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-18 04:34:36.000000 FasterAPI-0.0.8/FasterAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      105 2023-12-18 04:34:36.000000 FasterAPI-0.0.8/FasterAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-12-18 04:34:36.000000 FasterAPI-0.0.8/FasterAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3814 2023-12-18 04:34:36.437605 FasterAPI-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3075 2023-12-18 02:22:32.000000 FasterAPI-0.0.8/README.md
--rw-rw-rw-   0        0        0      748 2023-12-18 04:34:14.000000 FasterAPI-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-12-18 04:34:36.439934 FasterAPI-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-12-18 08:16:00.868338 FasterAPI-0.0.9/
+drwxrwxrwx   0        0        0        0 2023-12-18 08:16:00.850026 FasterAPI-0.0.9/FasterAPI/
+-rw-rw-rw-   0        0        0     2618 2023-12-18 02:22:32.000000 FasterAPI-0.0.9/FasterAPI/__init__.py
+-rw-rw-rw-   0        0        0     1891 2023-12-18 08:14:47.000000 FasterAPI-0.0.9/FasterAPI/app.py
+-rw-rw-rw-   0        0        0      702 2023-12-01 07:11:05.000000 FasterAPI-0.0.9/FasterAPI/models.py
+-rw-rw-rw-   0        0        0     5381 2023-12-01 16:48:01.000000 FasterAPI-0.0.9/FasterAPI/router.py
+-rw-rw-rw-   0        0        0      451 2023-12-01 06:34:20.000000 FasterAPI-0.0.9/FasterAPI/schemas.py
+-rw-rw-rw-   0        0        0     4816 2023-12-18 02:22:32.000000 FasterAPI-0.0.9/FasterAPI/utils.py
+drwxrwxrwx   0        0        0        0 2023-12-18 08:16:00.864337 FasterAPI-0.0.9/FasterAPI.egg-info/
+-rw-rw-rw-   0        0        0     3814 2023-12-18 08:16:00.000000 FasterAPI-0.0.9/FasterAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-12-18 08:16:00.000000 FasterAPI-0.0.9/FasterAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-12-18 08:16:00.000000 FasterAPI-0.0.9/FasterAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      105 2023-12-18 08:16:00.000000 FasterAPI-0.0.9/FasterAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-12-18 08:16:00.000000 FasterAPI-0.0.9/FasterAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3814 2023-12-18 08:16:00.866335 FasterAPI-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3075 2023-12-18 02:22:32.000000 FasterAPI-0.0.9/README.md
+-rw-rw-rw-   0        0        0      748 2023-12-18 08:15:04.000000 FasterAPI-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-12-18 08:16:00.868338 FasterAPI-0.0.9/setup.cfg
```

### Comparing `FasterAPI-0.0.8/FasterAPI/__init__.py` & `FasterAPI-0.0.9/FasterAPI/__init__.py`

 * *Files identical despite different names*

### Comparing `FasterAPI-0.0.8/FasterAPI/models.py` & `FasterAPI-0.0.9/FasterAPI/models.py`

 * *Files identical despite different names*

### Comparing `FasterAPI-0.0.8/FasterAPI/router.py` & `FasterAPI-0.0.9/FasterAPI/router.py`

 * *Files identical despite different names*

### Comparing `FasterAPI-0.0.8/FasterAPI/utils.py` & `FasterAPI-0.0.9/FasterAPI/utils.py`

 * *Files identical despite different names*

### Comparing `FasterAPI-0.0.8/FasterAPI.egg-info/PKG-INFO` & `FasterAPI-0.0.9/FasterAPI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FasterAPI
-Version: 0.0.8
+Version: 0.0.9
 Summary: Just a FasterAPI starting point with JWT user authentication.
 Author-email: Yifei Ren <ryf0510@live.com>
 Project-URL: Homepage, https://github.com/ulfaric/FasterAPI
 Project-URL: Bug Tracker, https://github.com/ulfaric/FasterAPI/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `FasterAPI-0.0.8/PKG-INFO` & `FasterAPI-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FasterAPI
-Version: 0.0.8
+Version: 0.0.9
 Summary: Just a FasterAPI starting point with JWT user authentication.
 Author-email: Yifei Ren <ryf0510@live.com>
 Project-URL: Homepage, https://github.com/ulfaric/FasterAPI
 Project-URL: Bug Tracker, https://github.com/ulfaric/FasterAPI/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `FasterAPI-0.0.8/README.md` & `FasterAPI-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `FasterAPI-0.0.8/pyproject.toml` & `FasterAPI-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "FasterAPI"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Yifei Ren", email="ryf0510@live.com" },
 ]
 description = "Just a FasterAPI starting point with JWT user authentication."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

