# Comparing `tmp/ydb-sqlalchemy-0.0.1b8.tar.gz` & `tmp/ydb-sqlalchemy-0.0.1b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ydb-sqlalchemy-0.0.1b8.tar", last modified: Mon Mar 25 18:16:27 2024, max compression
+gzip compressed data, was "ydb-sqlalchemy-0.0.1b9.tar", last modified: Mon Mar 25 18:18:39 2024, max compression
```

## Comparing `ydb-sqlalchemy-0.0.1b8.tar` & `ydb-sqlalchemy-0.0.1b9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:16:27.801683 ydb-sqlalchemy-0.0.1b8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-25 18:16:22.000000 ydb-sqlalchemy-0.0.1b8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-25 18:16:22.000000 ydb-sqlalchemy-0.0.1b8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-03-25 18:16:27.801683 ydb-sqlalchemy-0.0.1b8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-03-25 18:16:22.000000 ydb-sqlalchemy-0.0.1b8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-25 18:16:22.000000 ydb-sqlalchemy-0.0.1b8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-25 18:16:22.000000 ydb-sqlalchemy-0.0.1b8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-03-25 18:16:27.801683 ydb-sqlalchemy-0.0.1b8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-03-25 18:16:25.000000 ydb-sqlalchemy-0.0.1b8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:16:27.797683 ydb-sqlalchemy-0.0.1b8/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 18:16:22.000000 ydb-sqlalchemy-0.0.1b8/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-25 18:16:22.000000 ydb-sqlalchemy-0.0.1b8/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    26965 2024-03-25 18:16:22.000000 ydb-sqlalchemy-0.0.1b8/test/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-03-25 18:16:22.000000 ydb-sqlalchemy-0.0.1b8/test/test_inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)    18310 2024-03-25 18:16:22.000000 ydb-sqlalchemy-0.0.1b8/test/test_suite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:16:27.797683 ydb-sqlalchemy-0.0.1b8/test_dbapi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 18:16:22.000000 ydb-sqlalchemy-0.0.1b8/test_dbapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7114 2024-03-25 18:16:22.000000 ydb-sqlalchemy-0.0.1b8/test_dbapi/test_dbapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:16:27.797683 ydb-sqlalchemy-0.0.1b8/ydb_sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-25 18:16:22.000000 ydb-sqlalchemy-0.0.1b8/ydb_sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-25 18:16:25.000000 ydb-sqlalchemy-0.0.1b8/ydb_sqlalchemy/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:16:27.797683 ydb-sqlalchemy-0.0.1b8/ydb_sqlalchemy/dbapi/
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-03-25 18:16:22.000000 ydb-sqlalchemy-0.0.1b8/ydb_sqlalchemy/dbapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7254 2024-03-25 18:16:22.000000 ydb-sqlalchemy-0.0.1b8/ydb_sqlalchemy/dbapi/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-03-25 18:16:22.000000 ydb-sqlalchemy-0.0.1b8/ydb_sqlalchemy/dbapi/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    11151 2024-03-25 18:16:22.000000 ydb-sqlalchemy-0.0.1b8/ydb_sqlalchemy/dbapi/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-03-25 18:16:22.000000 ydb-sqlalchemy-0.0.1b8/ydb_sqlalchemy/dbapi/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:16:27.797683 ydb-sqlalchemy-0.0.1b8/ydb_sqlalchemy/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (127)    28730 2024-03-25 18:16:22.000000 ydb-sqlalchemy-0.0.1b8/ydb_sqlalchemy/sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-25 18:16:22.000000 ydb-sqlalchemy-0.0.1b8/ydb_sqlalchemy/sqlalchemy/dml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-03-25 18:16:22.000000 ydb-sqlalchemy-0.0.1b8/ydb_sqlalchemy/sqlalchemy/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-03-25 18:16:22.000000 ydb-sqlalchemy-0.0.1b8/ydb_sqlalchemy/sqlalchemy/requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-03-25 18:16:22.000000 ydb-sqlalchemy-0.0.1b8/ydb_sqlalchemy/sqlalchemy/test_sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-03-25 18:16:22.000000 ydb-sqlalchemy-0.0.1b8/ydb_sqlalchemy/sqlalchemy/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:16:27.801683 ydb-sqlalchemy-0.0.1b8/ydb_sqlalchemy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-03-25 18:16:27.000000 ydb-sqlalchemy-0.0.1b8/ydb_sqlalchemy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-03-25 18:16:27.000000 ydb-sqlalchemy-0.0.1b8/ydb_sqlalchemy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 18:16:27.000000 ydb-sqlalchemy-0.0.1b8/ydb_sqlalchemy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-03-25 18:16:27.000000 ydb-sqlalchemy-0.0.1b8/ydb_sqlalchemy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-25 18:16:27.000000 ydb-sqlalchemy-0.0.1b8/ydb_sqlalchemy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-25 18:16:27.000000 ydb-sqlalchemy-0.0.1b8/ydb_sqlalchemy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:18:39.386036 ydb-sqlalchemy-0.0.1b9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-25 18:18:29.000000 ydb-sqlalchemy-0.0.1b9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-25 18:18:29.000000 ydb-sqlalchemy-0.0.1b9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-03-25 18:18:39.386036 ydb-sqlalchemy-0.0.1b9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-03-25 18:18:29.000000 ydb-sqlalchemy-0.0.1b9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-25 18:18:29.000000 ydb-sqlalchemy-0.0.1b9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-25 18:18:29.000000 ydb-sqlalchemy-0.0.1b9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-03-25 18:18:39.386036 ydb-sqlalchemy-0.0.1b9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-03-25 18:18:37.000000 ydb-sqlalchemy-0.0.1b9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:18:39.382036 ydb-sqlalchemy-0.0.1b9/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 18:18:29.000000 ydb-sqlalchemy-0.0.1b9/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-25 18:18:29.000000 ydb-sqlalchemy-0.0.1b9/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26965 2024-03-25 18:18:29.000000 ydb-sqlalchemy-0.0.1b9/test/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-03-25 18:18:29.000000 ydb-sqlalchemy-0.0.1b9/test/test_inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18310 2024-03-25 18:18:29.000000 ydb-sqlalchemy-0.0.1b9/test/test_suite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:18:39.382036 ydb-sqlalchemy-0.0.1b9/test_dbapi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 18:18:29.000000 ydb-sqlalchemy-0.0.1b9/test_dbapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7114 2024-03-25 18:18:29.000000 ydb-sqlalchemy-0.0.1b9/test_dbapi/test_dbapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:18:39.382036 ydb-sqlalchemy-0.0.1b9/ydb_sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-25 18:18:29.000000 ydb-sqlalchemy-0.0.1b9/ydb_sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-25 18:18:37.000000 ydb-sqlalchemy-0.0.1b9/ydb_sqlalchemy/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:18:39.382036 ydb-sqlalchemy-0.0.1b9/ydb_sqlalchemy/dbapi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-03-25 18:18:29.000000 ydb-sqlalchemy-0.0.1b9/ydb_sqlalchemy/dbapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7254 2024-03-25 18:18:29.000000 ydb-sqlalchemy-0.0.1b9/ydb_sqlalchemy/dbapi/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-03-25 18:18:29.000000 ydb-sqlalchemy-0.0.1b9/ydb_sqlalchemy/dbapi/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11151 2024-03-25 18:18:29.000000 ydb-sqlalchemy-0.0.1b9/ydb_sqlalchemy/dbapi/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-03-25 18:18:29.000000 ydb-sqlalchemy-0.0.1b9/ydb_sqlalchemy/dbapi/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:18:39.382036 ydb-sqlalchemy-0.0.1b9/ydb_sqlalchemy/sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (127)    28730 2024-03-25 18:18:29.000000 ydb-sqlalchemy-0.0.1b9/ydb_sqlalchemy/sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-25 18:18:29.000000 ydb-sqlalchemy-0.0.1b9/ydb_sqlalchemy/sqlalchemy/dml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-03-25 18:18:29.000000 ydb-sqlalchemy-0.0.1b9/ydb_sqlalchemy/sqlalchemy/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-03-25 18:18:29.000000 ydb-sqlalchemy-0.0.1b9/ydb_sqlalchemy/sqlalchemy/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-03-25 18:18:29.000000 ydb-sqlalchemy-0.0.1b9/ydb_sqlalchemy/sqlalchemy/test_sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-03-25 18:18:29.000000 ydb-sqlalchemy-0.0.1b9/ydb_sqlalchemy/sqlalchemy/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:18:39.386036 ydb-sqlalchemy-0.0.1b9/ydb_sqlalchemy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-03-25 18:18:39.000000 ydb-sqlalchemy-0.0.1b9/ydb_sqlalchemy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-03-25 18:18:39.000000 ydb-sqlalchemy-0.0.1b9/ydb_sqlalchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 18:18:39.000000 ydb-sqlalchemy-0.0.1b9/ydb_sqlalchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-03-25 18:18:39.000000 ydb-sqlalchemy-0.0.1b9/ydb_sqlalchemy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-25 18:18:39.000000 ydb-sqlalchemy-0.0.1b9/ydb_sqlalchemy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-25 18:18:39.000000 ydb-sqlalchemy-0.0.1b9/ydb_sqlalchemy.egg-info/top_level.txt
```

### Comparing `ydb-sqlalchemy-0.0.1b8/LICENSE` & `ydb-sqlalchemy-0.0.1b9/LICENSE`

 * *Files identical despite different names*

### Comparing `ydb-sqlalchemy-0.0.1b8/PKG-INFO` & `ydb-sqlalchemy-0.0.1b9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ydb-sqlalchemy
-Version: 0.0.1b8
+Version: 0.0.1b9
 Summary: YDB Dialect for SQLAlchemy
 Home-page: http://github.com/ydb-platform/ydb-sqlalchemy
 Author: Yandex LLC
 Author-email: ydb@yandex-team.ru
 License: Apache 2.0
 Keywords: SQLAlchemy YDB YQL
 Classifier: Programming Language :: Python
```

### Comparing `ydb-sqlalchemy-0.0.1b8/README.md` & `ydb-sqlalchemy-0.0.1b9/README.md`

 * *Files identical despite different names*

### Comparing `ydb-sqlalchemy-0.0.1b8/setup.py` & `ydb-sqlalchemy-0.0.1b9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     for line in f.readlines():
         line = line.strip()
         if line:
             requirements.append(line)
 
 setuptools.setup(
     name="ydb-sqlalchemy",
-    version="0.0.1b8",  # AUTOVERSION
+    version="0.0.1b9",  # AUTOVERSION
     description="YDB Dialect for SQLAlchemy",
     author="Yandex LLC",
     author_email="ydb@yandex-team.ru",
     url="http://github.com/ydb-platform/ydb-sqlalchemy",
     license="Apache 2.0",
     package_dir={"": "."},
     long_description=long_description,
```

### Comparing `ydb-sqlalchemy-0.0.1b8/test/conftest.py` & `ydb-sqlalchemy-0.0.1b9/test/conftest.py`

 * *Files identical despite different names*

### Comparing `ydb-sqlalchemy-0.0.1b8/test/test_core.py` & `ydb-sqlalchemy-0.0.1b9/test/test_core.py`

 * *Files identical despite different names*

### Comparing `ydb-sqlalchemy-0.0.1b8/test/test_inspect.py` & `ydb-sqlalchemy-0.0.1b9/test/test_inspect.py`

 * *Files identical despite different names*

### Comparing `ydb-sqlalchemy-0.0.1b8/test/test_suite.py` & `ydb-sqlalchemy-0.0.1b9/test/test_suite.py`

 * *Files identical despite different names*

### Comparing `ydb-sqlalchemy-0.0.1b8/test_dbapi/test_dbapi.py` & `ydb-sqlalchemy-0.0.1b9/test_dbapi/test_dbapi.py`

 * *Files identical despite different names*

### Comparing `ydb-sqlalchemy-0.0.1b8/ydb_sqlalchemy/dbapi/__init__.py` & `ydb-sqlalchemy-0.0.1b9/ydb_sqlalchemy/dbapi/__init__.py`

 * *Files identical despite different names*

### Comparing `ydb-sqlalchemy-0.0.1b8/ydb_sqlalchemy/dbapi/connection.py` & `ydb-sqlalchemy-0.0.1b9/ydb_sqlalchemy/dbapi/connection.py`

 * *Files identical despite different names*

### Comparing `ydb-sqlalchemy-0.0.1b8/ydb_sqlalchemy/dbapi/constants.py` & `ydb-sqlalchemy-0.0.1b9/ydb_sqlalchemy/dbapi/constants.py`

 * *Files identical despite different names*

### Comparing `ydb-sqlalchemy-0.0.1b8/ydb_sqlalchemy/dbapi/cursor.py` & `ydb-sqlalchemy-0.0.1b9/ydb_sqlalchemy/dbapi/cursor.py`

 * *Files identical despite different names*

### Comparing `ydb-sqlalchemy-0.0.1b8/ydb_sqlalchemy/dbapi/errors.py` & `ydb-sqlalchemy-0.0.1b9/ydb_sqlalchemy/dbapi/errors.py`

 * *Files identical despite different names*

### Comparing `ydb-sqlalchemy-0.0.1b8/ydb_sqlalchemy/sqlalchemy/__init__.py` & `ydb-sqlalchemy-0.0.1b9/ydb_sqlalchemy/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `ydb-sqlalchemy-0.0.1b8/ydb_sqlalchemy/sqlalchemy/json.py` & `ydb-sqlalchemy-0.0.1b9/ydb_sqlalchemy/sqlalchemy/json.py`

 * *Files identical despite different names*

### Comparing `ydb-sqlalchemy-0.0.1b8/ydb_sqlalchemy/sqlalchemy/requirements.py` & `ydb-sqlalchemy-0.0.1b9/ydb_sqlalchemy/sqlalchemy/requirements.py`

 * *Files identical despite different names*

### Comparing `ydb-sqlalchemy-0.0.1b8/ydb_sqlalchemy/sqlalchemy/test_sqlalchemy.py` & `ydb-sqlalchemy-0.0.1b9/ydb_sqlalchemy/sqlalchemy/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `ydb-sqlalchemy-0.0.1b8/ydb_sqlalchemy/sqlalchemy/types.py` & `ydb-sqlalchemy-0.0.1b9/ydb_sqlalchemy/sqlalchemy/types.py`

 * *Files identical despite different names*

### Comparing `ydb-sqlalchemy-0.0.1b8/ydb_sqlalchemy.egg-info/PKG-INFO` & `ydb-sqlalchemy-0.0.1b9/ydb_sqlalchemy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ydb-sqlalchemy
-Version: 0.0.1b8
+Version: 0.0.1b9
 Summary: YDB Dialect for SQLAlchemy
 Home-page: http://github.com/ydb-platform/ydb-sqlalchemy
 Author: Yandex LLC
 Author-email: ydb@yandex-team.ru
 License: Apache 2.0
 Keywords: SQLAlchemy YDB YQL
 Classifier: Programming Language :: Python
```

### Comparing `ydb-sqlalchemy-0.0.1b8/ydb_sqlalchemy.egg-info/SOURCES.txt` & `ydb-sqlalchemy-0.0.1b9/ydb_sqlalchemy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

