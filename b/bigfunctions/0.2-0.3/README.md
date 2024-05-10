# Comparing `tmp/bigfunctions-0.2.tar.gz` & `tmp/bigfunctions-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigfunctions-0.2.tar", last modified: Fri May 10 16:37:56 2024, max compression
+gzip compressed data, was "bigfunctions-0.3.tar", last modified: Fri May 10 16:52:31 2024, max compression
```

## Comparing `bigfunctions-0.2.tar` & `bigfunctions-0.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-10 16:37:56.658268 bigfunctions-0.2/
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1064 2023-11-08 21:20:23.000000 bigfunctions-0.2/LICENSE
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     9822 2024-05-10 16:37:56.657268 bigfunctions-0.2/PKG-INFO
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     9097 2024-02-22 22:16:20.000000 bigfunctions-0.2/README.md
-drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-10 16:37:56.645267 bigfunctions-0.2/bigfun/
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2023-11-08 21:20:23.000000 bigfunctions-0.2/bigfun/__init__.py
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     9876 2024-05-10 13:07:40.000000 bigfunctions-0.2/bigfun/bigfunctions.py
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     7860 2024-05-10 13:28:21.000000 bigfunctions-0.2/bigfun/cli.py
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      844 2023-12-01 17:33:50.000000 bigfunctions-0.2/bigfun/load_table.py
-drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-10 16:37:56.649267 bigfunctions-0.2/bigfun/templates/
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1086 2023-11-08 21:20:23.000000 bigfunctions-0.2/bigfun/templates/Dockerfile
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    11320 2024-05-10 12:31:51.000000 bigfunctions-0.2/bigfun/templates/bigfunction.md
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     3784 2024-01-19 20:34:23.000000 bigfunctions-0.2/bigfun/templates/bookmarklet.js
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1618 2024-05-10 09:49:39.000000 bigfunctions-0.2/bigfun/templates/categories.md
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1958 2024-03-01 20:43:46.000000 bigfunctions-0.2/bigfun/templates/categories.yaml
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     4164 2024-01-24 23:20:01.000000 bigfunctions-0.2/bigfun/templates/data.md
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      554 2024-02-23 19:54:09.000000 bigfunctions-0.2/bigfun/templates/function_js.sql
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     7724 2024-02-23 21:48:51.000000 bigfunctions-0.2/bigfun/templates/function_py.py
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      316 2024-02-23 19:48:03.000000 bigfunctions-0.2/bigfun/templates/function_py.sql
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      212 2024-02-23 21:42:39.000000 bigfunctions-0.2/bigfun/templates/function_py_test.py
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      410 2024-02-23 19:54:09.000000 bigfunctions-0.2/bigfun/templates/function_sql.sql
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      251 2024-02-23 22:59:01.000000 bigfunctions-0.2/bigfun/templates/function_sql_test.sql
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      702 2024-02-23 19:54:09.000000 bigfunctions-0.2/bigfun/templates/procedure.sql
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      717 2024-02-23 22:23:06.000000 bigfunctions-0.2/bigfun/templates/procedure_test.sql
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      345 2024-02-23 19:54:09.000000 bigfunctions-0.2/bigfun/templates/table_function.sql
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    13249 2024-02-28 09:48:29.000000 bigfunctions-0.2/bigfun/utils.py
-drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-10 16:37:56.649267 bigfunctions-0.2/bigfun/website/
-drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-10 16:37:56.654268 bigfunctions-0.2/bigfun/website/assets/
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1714 2023-11-29 13:48:58.000000 bigfunctions-0.2/bigfun/website/assets/GitHub-Mark-32px.png
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)  1353755 2024-01-19 20:34:23.000000 bigfunctions-0.2/bigfun/website/assets/bookmarklet_usage.gif
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    23806 2023-11-29 13:48:58.000000 bigfunctions-0.2/bigfun/website/assets/logo.png
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    73519 2023-11-29 13:48:58.000000 bigfunctions-0.2/bigfun/website/assets/logo_and_name.png
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    49771 2023-11-29 13:48:58.000000 bigfunctions-0.2/bigfun/website/assets/logo_and_name_wo_supercharge.png
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      888 2024-05-10 16:32:26.000000 bigfunctions-0.2/bigfun/website/mkdocs.yml
-drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-10 16:37:56.655268 bigfunctions-0.2/bigfun/website/theme_overrides/
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     6185 2024-05-10 12:11:21.000000 bigfunctions-0.2/bigfun/website/theme_overrides/main.html
-drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-10 16:37:56.657268 bigfunctions-0.2/bigfunctions.egg-info/
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     9822 2024-05-10 16:37:56.000000 bigfunctions-0.2/bigfunctions.egg-info/PKG-INFO
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1109 2024-05-10 16:37:56.000000 bigfunctions-0.2/bigfunctions.egg-info/SOURCES.txt
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)        1 2024-05-10 16:37:56.000000 bigfunctions-0.2/bigfunctions.egg-info/dependency_links.txt
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)       42 2024-05-10 16:37:56.000000 bigfunctions-0.2/bigfunctions.egg-info/entry_points.txt
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      130 2024-05-10 16:37:56.000000 bigfunctions-0.2/bigfunctions.egg-info/requires.txt
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)        7 2024-05-10 16:37:56.000000 bigfunctions-0.2/bigfunctions.egg-info/top_level.txt
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)       38 2024-05-10 16:37:56.658268 bigfunctions-0.2/setup.cfg
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1329 2024-05-10 16:29:21.000000 bigfunctions-0.2/setup.py
+drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-10 16:52:31.490811 bigfunctions-0.3/
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1064 2023-11-08 21:20:23.000000 bigfunctions-0.3/LICENSE
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     9822 2024-05-10 16:52:31.490811 bigfunctions-0.3/PKG-INFO
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     9097 2024-02-22 22:16:20.000000 bigfunctions-0.3/README.md
+drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-10 16:52:31.478810 bigfunctions-0.3/bigfun/
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2023-11-08 21:20:23.000000 bigfunctions-0.3/bigfun/__init__.py
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     9876 2024-05-10 13:07:40.000000 bigfunctions-0.3/bigfun/bigfunctions.py
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     7860 2024-05-10 13:28:21.000000 bigfunctions-0.3/bigfun/cli.py
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      844 2023-12-01 17:33:50.000000 bigfunctions-0.3/bigfun/load_table.py
+drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-10 16:52:31.482811 bigfunctions-0.3/bigfun/templates/
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1086 2023-11-08 21:20:23.000000 bigfunctions-0.3/bigfun/templates/Dockerfile
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    11320 2024-05-10 12:31:51.000000 bigfunctions-0.3/bigfun/templates/bigfunction.md
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     3784 2024-01-19 20:34:23.000000 bigfunctions-0.3/bigfun/templates/bookmarklet.js
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1618 2024-05-10 09:49:39.000000 bigfunctions-0.3/bigfun/templates/categories.md
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1958 2024-03-01 20:43:46.000000 bigfunctions-0.3/bigfun/templates/categories.yaml
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     4164 2024-01-24 23:20:01.000000 bigfunctions-0.3/bigfun/templates/data.md
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      554 2024-02-23 19:54:09.000000 bigfunctions-0.3/bigfun/templates/function_js.sql
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     7724 2024-02-23 21:48:51.000000 bigfunctions-0.3/bigfun/templates/function_py.py
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      316 2024-02-23 19:48:03.000000 bigfunctions-0.3/bigfun/templates/function_py.sql
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      212 2024-02-23 21:42:39.000000 bigfunctions-0.3/bigfun/templates/function_py_test.py
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      410 2024-02-23 19:54:09.000000 bigfunctions-0.3/bigfun/templates/function_sql.sql
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      251 2024-02-23 22:59:01.000000 bigfunctions-0.3/bigfun/templates/function_sql_test.sql
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      702 2024-02-23 19:54:09.000000 bigfunctions-0.3/bigfun/templates/procedure.sql
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      717 2024-02-23 22:23:06.000000 bigfunctions-0.3/bigfun/templates/procedure_test.sql
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      345 2024-02-23 19:54:09.000000 bigfunctions-0.3/bigfun/templates/table_function.sql
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    13249 2024-02-28 09:48:29.000000 bigfunctions-0.3/bigfun/utils.py
+drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-10 16:52:31.482811 bigfunctions-0.3/bigfun/website/
+drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-10 16:52:31.487811 bigfunctions-0.3/bigfun/website/assets/
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1714 2023-11-29 13:48:58.000000 bigfunctions-0.3/bigfun/website/assets/GitHub-Mark-32px.png
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)  1353755 2024-01-19 20:34:23.000000 bigfunctions-0.3/bigfun/website/assets/bookmarklet_usage.gif
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    23806 2023-11-29 13:48:58.000000 bigfunctions-0.3/bigfun/website/assets/logo.png
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    73519 2023-11-29 13:48:58.000000 bigfunctions-0.3/bigfun/website/assets/logo_and_name.png
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    49771 2023-11-29 13:48:58.000000 bigfunctions-0.3/bigfun/website/assets/logo_and_name_wo_supercharge.png
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      888 2024-05-10 16:32:26.000000 bigfunctions-0.3/bigfun/website/mkdocs.yml
+drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-10 16:52:31.487811 bigfunctions-0.3/bigfun/website/theme_overrides/
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     6185 2024-05-10 12:11:21.000000 bigfunctions-0.3/bigfun/website/theme_overrides/main.html
+drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-10 16:52:31.489811 bigfunctions-0.3/bigfunctions.egg-info/
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     9822 2024-05-10 16:52:31.000000 bigfunctions-0.3/bigfunctions.egg-info/PKG-INFO
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1109 2024-05-10 16:52:31.000000 bigfunctions-0.3/bigfunctions.egg-info/SOURCES.txt
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)        1 2024-05-10 16:52:31.000000 bigfunctions-0.3/bigfunctions.egg-info/dependency_links.txt
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)       42 2024-05-10 16:52:31.000000 bigfunctions-0.3/bigfunctions.egg-info/entry_points.txt
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      130 2024-05-10 16:52:31.000000 bigfunctions-0.3/bigfunctions.egg-info/requires.txt
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)        7 2024-05-10 16:52:31.000000 bigfunctions-0.3/bigfunctions.egg-info/top_level.txt
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)       38 2024-05-10 16:52:31.491811 bigfunctions-0.3/setup.cfg
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1335 2024-05-10 16:50:26.000000 bigfunctions-0.3/setup.py
```

### Comparing `bigfunctions-0.2/LICENSE` & `bigfunctions-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.2/PKG-INFO` & `bigfunctions-0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: bigfunctions
-Version: 0.2
+Version: 0.3
 Summary: Supercharge BigQuery with BigFunctions
-Download-URL: https://github.com/unytics/bigfunctions/archive/refs/tags/v0.2.tar.gz
+Download-URL: https://github.com/unytics/bigfunctions/archive/refs/tags/v0.3.tar.gz
 Author: Unytics
 Author-email: paul.marcombes@unytics.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: bigfunctions Version: 0.2 Summary: Supercharge
+Metadata-Version: 2.1 Name: bigfunctions Version: 0.3 Summary: Supercharge
 BigQuery with BigFunctions Download-URL: https://github.com/unytics/
-bigfunctions/archive/refs/tags/v0.2.tar.gz Author: Unytics Author-email:
+bigfunctions/archive/refs/tags/v0.3.tar.gz Author: Unytics Author-email:
 paul.marcombes@unytics.io Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.10 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: google-cloud-bigquery Requires-
 Dist: google-cloud-bigquery_connection Requires-Dist: google-cloud-storage
 Requires-Dist: pyyaml Requires-Dist: jinja2 Requires-Dist: mkdocs-material
 Requires-Dist: click Requires-Dist: click-help-colors
```

### Comparing `bigfunctions-0.2/README.md` & `bigfunctions-0.3/README.md`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.2/bigfun/bigfunctions.py` & `bigfunctions-0.3/bigfun/bigfunctions.py`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.2/bigfun/cli.py` & `bigfunctions-0.3/bigfun/cli.py`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.2/bigfun/load_table.py` & `bigfunctions-0.3/bigfun/load_table.py`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.2/bigfun/templates/Dockerfile` & `bigfunctions-0.3/bigfun/templates/Dockerfile`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.2/bigfun/templates/bigfunction.md` & `bigfunctions-0.3/bigfun/templates/bigfunction.md`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.2/bigfun/templates/bookmarklet.js` & `bigfunctions-0.3/bigfun/templates/bookmarklet.js`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.2/bigfun/templates/categories.md` & `bigfunctions-0.3/bigfun/templates/categories.md`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.2/bigfun/templates/categories.yaml` & `bigfunctions-0.3/bigfun/templates/categories.yaml`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.2/bigfun/templates/data.md` & `bigfunctions-0.3/bigfun/templates/data.md`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.2/bigfun/templates/function_js.sql` & `bigfunctions-0.3/bigfun/templates/function_js.sql`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.2/bigfun/templates/function_py.py` & `bigfunctions-0.3/bigfun/templates/function_py.py`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.2/bigfun/templates/procedure.sql` & `bigfunctions-0.3/bigfun/templates/procedure.sql`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.2/bigfun/templates/procedure_test.sql` & `bigfunctions-0.3/bigfun/templates/procedure_test.sql`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.2/bigfun/utils.py` & `bigfunctions-0.3/bigfun/utils.py`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.2/bigfun/website/assets/GitHub-Mark-32px.png` & `bigfunctions-0.3/bigfun/website/assets/GitHub-Mark-32px.png`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.2/bigfun/website/assets/bookmarklet_usage.gif` & `bigfunctions-0.3/bigfun/website/assets/bookmarklet_usage.gif`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.2/bigfun/website/assets/logo.png` & `bigfunctions-0.3/bigfun/website/assets/logo.png`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.2/bigfun/website/assets/logo_and_name.png` & `bigfunctions-0.3/bigfun/website/assets/logo_and_name.png`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.2/bigfun/website/assets/logo_and_name_wo_supercharge.png` & `bigfunctions-0.3/bigfun/website/assets/logo_and_name_wo_supercharge.png`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.2/bigfun/website/mkdocs.yml` & `bigfunctions-0.3/bigfun/website/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.2/bigfun/website/theme_overrides/main.html` & `bigfunctions-0.3/bigfun/website/theme_overrides/main.html`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.2/bigfunctions.egg-info/PKG-INFO` & `bigfunctions-0.3/bigfunctions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: bigfunctions
-Version: 0.2
+Version: 0.3
 Summary: Supercharge BigQuery with BigFunctions
-Download-URL: https://github.com/unytics/bigfunctions/archive/refs/tags/v0.2.tar.gz
+Download-URL: https://github.com/unytics/bigfunctions/archive/refs/tags/v0.3.tar.gz
 Author: Unytics
 Author-email: paul.marcombes@unytics.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: bigfunctions Version: 0.2 Summary: Supercharge
+Metadata-Version: 2.1 Name: bigfunctions Version: 0.3 Summary: Supercharge
 BigQuery with BigFunctions Download-URL: https://github.com/unytics/
-bigfunctions/archive/refs/tags/v0.2.tar.gz Author: Unytics Author-email:
+bigfunctions/archive/refs/tags/v0.3.tar.gz Author: Unytics Author-email:
 paul.marcombes@unytics.io Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.10 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: google-cloud-bigquery Requires-
 Dist: google-cloud-bigquery_connection Requires-Dist: google-cloud-storage
 Requires-Dist: pyyaml Requires-Dist: jinja2 Requires-Dist: mkdocs-material
 Requires-Dist: click Requires-Dist: click-help-colors
```

### Comparing `bigfunctions-0.2/bigfunctions.egg-info/SOURCES.txt` & `bigfunctions-0.3/bigfunctions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.2/setup.py` & `bigfunctions-0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import setuptools
 
 
-VERSION = '0.2'
+VERSION = '0.3'
 
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 extra_files = [
     os.path.join(root, f)
@@ -31,15 +31,15 @@
     download_url=f'https://github.com/unytics/bigfunctions/archive/refs/tags/v{VERSION}.tar.gz',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.10',
-    package_data={'': extra_files},
+    package_data={'bigfun': extra_files},
     install_requires=[
         'google-cloud-bigquery',
         'google-cloud-bigquery_connection',
         'google-cloud-storage',
         'pyyaml',
         'jinja2',
         'mkdocs-material',
```

