# Comparing `tmp/hxm_refuel-0.2.8.tar.gz` & `tmp/hxm_refuel-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hxm_refuel-0.2.8.tar", max compression
+gzip compressed data, was "hxm_refuel-0.2.9.tar", max compression
```

## Comparing `hxm_refuel-0.2.8.tar` & `hxm_refuel-0.2.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0        0 2023-12-01 11:06:34.970622 hxm_refuel-0.2.8/hxm_refuel/__init__.py
--rw-r--r--   0        0        0      105 2023-09-24 14:23:26.541224 hxm_refuel-0.2.8/hxm_refuel/bloomberg/__init__.py
--rw-r--r--   0        0        0    14912 2024-03-19 17:19:40.062775 hxm_refuel-0.2.8/hxm_refuel/bloomberg/bloomberg_api.py
--rw-r--r--   0        0        0     2910 2023-09-24 12:17:44.083265 hxm_refuel-0.2.8/hxm_refuel/bloomberg/bloomberg_recipies.py
--rw-r--r--   0        0        0     5958 2024-02-28 12:48:30.731267 hxm_refuel-0.2.8/hxm_refuel/jeeves.py
--rw-r--r--   0        0        0      148 2024-02-09 07:15:41.900434 hxm_refuel-0.2.8/hxm_refuel/snowflake/__init__.py
--rw-r--r--   0        0        0     4389 2023-11-16 09:53:55.341194 hxm_refuel-0.2.8/hxm_refuel/snowflake/connector.py
--rw-r--r--   0        0        0     1431 2024-02-09 07:24:40.724467 hxm_refuel-0.2.8/hxm_refuel/snowflake/snowflake_recipes.py
--rw-r--r--   0        0        0     6627 2023-11-20 18:51:50.473891 hxm_refuel-0.2.8/hxm_refuel/snowflake/sql_recipes.py
--rw-r--r--   0        0        0     6649 2023-02-08 07:39:46.066344 hxm_refuel-0.2.8/hxm_refuel/validation.py
--rw-r--r--   0        0        0     1085 2023-09-24 11:04:20.427375 hxm_refuel-0.2.8/LICENSE
--rw-r--r--   0        0        0      766 2024-05-08 15:58:18.041334 hxm_refuel-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     4021 2023-11-16 10:18:45.692284 hxm_refuel-0.2.8/README.md
--rw-r--r--   0        0        0     4583 1970-01-01 00:00:00.000000 hxm_refuel-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-12-01 11:06:34.970622 hxm_refuel-0.2.9/hxm_refuel/__init__.py
+-rw-r--r--   0        0        0      105 2023-09-24 14:23:26.541224 hxm_refuel-0.2.9/hxm_refuel/bloomberg/__init__.py
+-rw-r--r--   0        0        0    14912 2024-03-19 17:19:40.062775 hxm_refuel-0.2.9/hxm_refuel/bloomberg/bloomberg_api.py
+-rw-r--r--   0        0        0     2910 2023-09-24 12:17:44.083265 hxm_refuel-0.2.9/hxm_refuel/bloomberg/bloomberg_recipies.py
+-rw-r--r--   0        0        0     5958 2024-02-28 12:48:30.731267 hxm_refuel-0.2.9/hxm_refuel/jeeves.py
+-rw-r--r--   0        0        0      148 2024-02-09 07:15:41.900434 hxm_refuel-0.2.9/hxm_refuel/snowflake/__init__.py
+-rw-r--r--   0        0        0     4389 2023-11-16 09:53:55.341194 hxm_refuel-0.2.9/hxm_refuel/snowflake/connector.py
+-rw-r--r--   0        0        0     1431 2024-02-09 07:24:40.724467 hxm_refuel-0.2.9/hxm_refuel/snowflake/snowflake_recipes.py
+-rw-r--r--   0        0        0     6627 2023-11-20 18:51:50.473891 hxm_refuel-0.2.9/hxm_refuel/snowflake/sql_recipes.py
+-rw-r--r--   0        0        0     6649 2023-02-08 07:39:46.066344 hxm_refuel-0.2.9/hxm_refuel/validation.py
+-rw-r--r--   0        0        0     1085 2023-09-24 11:04:20.427375 hxm_refuel-0.2.9/LICENSE
+-rw-r--r--   0        0        0      766 2024-05-10 20:22:58.402656 hxm_refuel-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     4021 2023-11-16 10:18:45.692284 hxm_refuel-0.2.9/README.md
+-rw-r--r--   0        0        0     4543 1970-01-01 00:00:00.000000 hxm_refuel-0.2.9/PKG-INFO
```

### Comparing `hxm_refuel-0.2.8/hxm_refuel/bloomberg/bloomberg_api.py` & `hxm_refuel-0.2.9/hxm_refuel/bloomberg/bloomberg_api.py`

 * *Files identical despite different names*

### Comparing `hxm_refuel-0.2.8/hxm_refuel/bloomberg/bloomberg_recipies.py` & `hxm_refuel-0.2.9/hxm_refuel/bloomberg/bloomberg_recipies.py`

 * *Files identical despite different names*

### Comparing `hxm_refuel-0.2.8/hxm_refuel/jeeves.py` & `hxm_refuel-0.2.9/hxm_refuel/jeeves.py`

 * *Files identical despite different names*

### Comparing `hxm_refuel-0.2.8/hxm_refuel/snowflake/connector.py` & `hxm_refuel-0.2.9/hxm_refuel/snowflake/connector.py`

 * *Files identical despite different names*

### Comparing `hxm_refuel-0.2.8/hxm_refuel/snowflake/snowflake_recipes.py` & `hxm_refuel-0.2.9/hxm_refuel/snowflake/snowflake_recipes.py`

 * *Files identical despite different names*

### Comparing `hxm_refuel-0.2.8/hxm_refuel/snowflake/sql_recipes.py` & `hxm_refuel-0.2.9/hxm_refuel/snowflake/sql_recipes.py`

 * *Files identical despite different names*

### Comparing `hxm_refuel-0.2.8/hxm_refuel/validation.py` & `hxm_refuel-0.2.9/hxm_refuel/validation.py`

 * *Files identical despite different names*

### Comparing `hxm_refuel-0.2.8/LICENSE` & `hxm_refuel-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hxm_refuel-0.2.8/pyproject.toml` & `hxm_refuel-0.2.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "hxm-refuel"
-version = "0.2.8"
+version = "0.2.9"
 description = "Wrapper for financial database APIs"
 authors = ["djmcnay <39102979+djmcnay@users.noreply.github.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <3.12"
 xbbg = "^0.7.7"
 snowflake-connector-python = "^3.2.0"
 snowflake-sqlalchemy = "^1.5.0"
 pyarrow = ">=10.0.1, <10.1.0"
 cryptography = "^41.0.5"
-blpapi = {version = "^3.18.0", source = "bloomberg"}
 
 [tool.poetry.group.dev.dependencies]
 jupyterlab = "^4.0.8"
 python-dotenv = "^1.0.0"
 pytest = "^7.4.2"
+blpapi = {version = "^3.24.4", source = "bloomberg"}
 
 [[tool.poetry.source]]
 name = "bloomberg"
 url = "https://bcms.bloomberg.com/pip/simple"
 priority = "explicit"
 
 [build-system]
```

### Comparing `hxm_refuel-0.2.8/README.md` & `hxm_refuel-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `hxm_refuel-0.2.8/PKG-INFO` & `hxm_refuel-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: hxm-refuel
-Version: 0.2.8
+Version: 0.2.9
 Summary: Wrapper for financial database APIs
 Author: djmcnay
 Author-email: 39102979+djmcnay@users.noreply.github.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: blpapi (>=3.18.0,<4.0.0)
 Requires-Dist: cryptography (>=41.0.5,<42.0.0)
 Requires-Dist: pyarrow (>=10.0.1,<10.1.0)
 Requires-Dist: snowflake-connector-python (>=3.2.0,<4.0.0)
 Requires-Dist: snowflake-sqlalchemy (>=1.5.0,<2.0.0)
 Requires-Dist: xbbg (>=0.7.7,<0.8.0)
 Description-Content-Type: text/markdown
```

