# Comparing `tmp/gluestick-2.1.8.tar.gz` & `tmp/gluestick-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gluestick-2.1.8.tar", last modified: Mon Feb  5 17:14:39 2024, max compression
+gzip compressed data, was "gluestick-2.1.9.tar", last modified: Mon Feb  5 17:31:13 2024, max compression
```

## Comparing `gluestick-2.1.8.tar` & `gluestick-2.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 hassansyyid   (501) staff       (20)        0 2024-02-05 17:14:39.057215 gluestick-2.1.8/
--rw-r--r--   0 hassansyyid   (501) staff       (20)     1047 2022-08-01 18:09:19.000000 gluestick-2.1.8/LICENSE
--rw-r--r--   0 hassansyyid   (501) staff       (20)     1280 2024-02-05 17:14:39.056993 gluestick-2.1.8/PKG-INFO
--rw-r--r--   0 hassansyyid   (501) staff       (20)      884 2022-08-01 18:09:19.000000 gluestick-2.1.8/README.md
-drwxr-xr-x   0 hassansyyid   (501) staff       (20)        0 2024-02-05 17:14:39.055551 gluestick-2.1.8/gluestick/
--rw-r--r--   0 hassansyyid   (501) staff       (20)      149 2022-11-25 14:49:32.000000 gluestick-2.1.8/gluestick/__init__.py
--rw-r--r--   0 hassansyyid   (501) staff       (20)    18716 2024-02-05 17:13:41.000000 gluestick-2.1.8/gluestick/etl_utils.py
--rw-r--r--   0 hassansyyid   (501) staff       (20)    10364 2023-10-26 20:31:22.000000 gluestick-2.1.8/gluestick/pandas_utils.py
--rw-r--r--   0 hassansyyid   (501) staff       (20)     5841 2024-02-05 17:13:00.000000 gluestick-2.1.8/gluestick/singer.py
-drwxr-xr-x   0 hassansyyid   (501) staff       (20)        0 2024-02-05 17:14:39.056761 gluestick-2.1.8/gluestick.egg-info/
--rw-r--r--   0 hassansyyid   (501) staff       (20)     1280 2024-02-05 17:14:39.000000 gluestick-2.1.8/gluestick.egg-info/PKG-INFO
--rw-r--r--   0 hassansyyid   (501) staff       (20)      328 2024-02-05 17:14:39.000000 gluestick-2.1.8/gluestick.egg-info/SOURCES.txt
--rw-r--r--   0 hassansyyid   (501) staff       (20)        1 2024-02-05 17:14:39.000000 gluestick-2.1.8/gluestick.egg-info/dependency_links.txt
--rw-r--r--   0 hassansyyid   (501) staff       (20)        1 2022-08-01 18:12:05.000000 gluestick-2.1.8/gluestick.egg-info/not-zip-safe
--rw-r--r--   0 hassansyyid   (501) staff       (20)       61 2024-02-05 17:14:39.000000 gluestick-2.1.8/gluestick.egg-info/requires.txt
--rw-r--r--   0 hassansyyid   (501) staff       (20)       10 2024-02-05 17:14:39.000000 gluestick-2.1.8/gluestick.egg-info/top_level.txt
--rw-r--r--   0 hassansyyid   (501) staff       (20)      383 2022-11-25 14:49:32.000000 gluestick-2.1.8/pyproject.toml
--rw-r--r--   0 hassansyyid   (501) staff       (20)       38 2024-02-05 17:14:39.057255 gluestick-2.1.8/setup.cfg
--rw-r--r--   0 hassansyyid   (501) staff       (20)      611 2024-02-05 17:13:41.000000 gluestick-2.1.8/setup.py
+drwxr-xr-x   0 hassansyyid   (501) staff       (20)        0 2024-02-05 17:31:13.986631 gluestick-2.1.9/
+-rw-r--r--   0 hassansyyid   (501) staff       (20)     1047 2022-08-01 18:09:19.000000 gluestick-2.1.9/LICENSE
+-rw-r--r--   0 hassansyyid   (501) staff       (20)     1280 2024-02-05 17:31:13.986389 gluestick-2.1.9/PKG-INFO
+-rw-r--r--   0 hassansyyid   (501) staff       (20)      884 2022-08-01 18:09:19.000000 gluestick-2.1.9/README.md
+drwxr-xr-x   0 hassansyyid   (501) staff       (20)        0 2024-02-05 17:31:13.985016 gluestick-2.1.9/gluestick/
+-rw-r--r--   0 hassansyyid   (501) staff       (20)      149 2022-11-25 14:49:32.000000 gluestick-2.1.9/gluestick/__init__.py
+-rw-r--r--   0 hassansyyid   (501) staff       (20)    18810 2024-02-05 17:30:23.000000 gluestick-2.1.9/gluestick/etl_utils.py
+-rw-r--r--   0 hassansyyid   (501) staff       (20)    10364 2023-10-26 20:31:22.000000 gluestick-2.1.9/gluestick/pandas_utils.py
+-rw-r--r--   0 hassansyyid   (501) staff       (20)     5841 2024-02-05 17:13:00.000000 gluestick-2.1.9/gluestick/singer.py
+drwxr-xr-x   0 hassansyyid   (501) staff       (20)        0 2024-02-05 17:31:13.986154 gluestick-2.1.9/gluestick.egg-info/
+-rw-r--r--   0 hassansyyid   (501) staff       (20)     1280 2024-02-05 17:31:13.000000 gluestick-2.1.9/gluestick.egg-info/PKG-INFO
+-rw-r--r--   0 hassansyyid   (501) staff       (20)      328 2024-02-05 17:31:13.000000 gluestick-2.1.9/gluestick.egg-info/SOURCES.txt
+-rw-r--r--   0 hassansyyid   (501) staff       (20)        1 2024-02-05 17:31:13.000000 gluestick-2.1.9/gluestick.egg-info/dependency_links.txt
+-rw-r--r--   0 hassansyyid   (501) staff       (20)        1 2022-08-01 18:12:05.000000 gluestick-2.1.9/gluestick.egg-info/not-zip-safe
+-rw-r--r--   0 hassansyyid   (501) staff       (20)       61 2024-02-05 17:31:13.000000 gluestick-2.1.9/gluestick.egg-info/requires.txt
+-rw-r--r--   0 hassansyyid   (501) staff       (20)       10 2024-02-05 17:31:13.000000 gluestick-2.1.9/gluestick.egg-info/top_level.txt
+-rw-r--r--   0 hassansyyid   (501) staff       (20)      383 2022-11-25 14:49:32.000000 gluestick-2.1.9/pyproject.toml
+-rw-r--r--   0 hassansyyid   (501) staff       (20)       38 2024-02-05 17:31:13.986668 gluestick-2.1.9/setup.cfg
+-rw-r--r--   0 hassansyyid   (501) staff       (20)      611 2024-02-05 17:30:33.000000 gluestick-2.1.9/setup.py
```

### Comparing `gluestick-2.1.8/LICENSE` & `gluestick-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gluestick-2.1.8/PKG-INFO` & `gluestick-2.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gluestick
-Version: 2.1.8
+Version: 2.1.9
 Summary: ETL utility functions built on Pandas
 Home-page: https://github.com/hotgluexyz/gluestick
 Author: hotglue
 Author-email: hello@hotglue.xyz
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gluestick-2.1.8/README.md` & `gluestick-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `gluestick-2.1.8/gluestick/etl_utils.py` & `gluestick-2.1.9/gluestick/etl_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -416,14 +416,18 @@
 
     Returns
     -------
     return: dict, list
         parsed dict or list of dicts.
 
     """
+    # if it's not a string, we just return the input
+    if type(x) != str:
+        return x
+
     try:
         return ast.literal_eval(x)
     except:
         return json.loads(x)
 
 def to_export(data, name, output_dir, keys=[], export_format=os.environ.get("DEFAULT_EXPORT_FORMAT", "singer"), output_file_prefix=os.environ.get("OUTPUT_FILE_PREFIX")):
     """Parse a stringified dict or list of dicts.
```

### Comparing `gluestick-2.1.8/gluestick/pandas_utils.py` & `gluestick-2.1.9/gluestick/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `gluestick-2.1.8/gluestick/singer.py` & `gluestick-2.1.9/gluestick/singer.py`

 * *Files identical despite different names*

### Comparing `gluestick-2.1.8/gluestick.egg-info/PKG-INFO` & `gluestick-2.1.9/gluestick.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gluestick
-Version: 2.1.8
+Version: 2.1.9
 Summary: ETL utility functions built on Pandas
 Home-page: https://github.com/hotgluexyz/gluestick
 Author: hotglue
 Author-email: hello@hotglue.xyz
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gluestick-2.1.8/setup.py` & `gluestick-2.1.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="gluestick",
-    version="2.1.8",
+    version="2.1.9",
     description="ETL utility functions built on Pandas",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hotgluexyz/gluestick",
     install_requires=[
         "singer-python>=4.0.0",
         "numpy>=1.4",
```

