# Comparing `tmp/gdatalog-0.3.2.tar.gz` & `tmp/gdatalog-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdatalog-0.3.2.tar", max compression
+gzip compressed data, was "gdatalog-0.3.3.tar", max compression
```

## Comparing `gdatalog-0.3.2.tar` & `gdatalog-0.3.3.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0    11357 2022-04-12 16:40:14.248719 gdatalog-0.3.2/LICENSE
--rw-r--r--   0        0        0        0 2022-03-14 14:53:06.573903 gdatalog-0.3.2/gdatalog/__init__.py
--rwxr-xr-x   0        0        0       99 2022-09-15 18:33:51.662671 gdatalog-0.3.2/gdatalog/__main__.py
--rw-r--r--   0        0        0     5574 2024-03-23 13:20:56.849761 gdatalog-0.3.2/gdatalog/cli.py
--rw-r--r--   0        0        0     7357 2024-03-23 15:04:54.736506 gdatalog-0.3.2/gdatalog/delta_terms.py
--rw-r--r--   0        0        0     7387 2024-03-23 15:03:14.192566 gdatalog-0.3.2/gdatalog/program.py
--rw-r--r--   0        0        0     1662 2024-03-20 13:41:27.185221 gdatalog-0.3.2/gdatalog/utils.py
--rw-r--r--   0        0        0      505 2024-03-23 15:05:03.456507 gdatalog-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      621 1970-01-01 00:00:00.000000 gdatalog-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-04-12 16:40:14.248719 gdatalog-0.3.3/LICENSE
+-rw-r--r--   0        0        0        0 2022-03-14 14:53:06.573903 gdatalog-0.3.3/gdatalog/__init__.py
+-rwxr-xr-x   0        0        0       99 2022-09-15 18:33:51.662671 gdatalog-0.3.3/gdatalog/__main__.py
+-rw-r--r--   0        0        0     5574 2024-03-23 13:20:56.849761 gdatalog-0.3.3/gdatalog/cli.py
+-rw-r--r--   0        0        0     7357 2024-03-23 15:04:54.736506 gdatalog-0.3.3/gdatalog/delta_terms.py
+-rw-r--r--   0        0        0     7387 2024-03-23 15:03:14.192566 gdatalog-0.3.3/gdatalog/program.py
+-rw-r--r--   0        0        0     1316 2024-05-10 16:25:13.501431 gdatalog-0.3.3/gdatalog/server.py
+-rw-r--r--   0        0        0     1662 2024-03-20 13:41:27.185221 gdatalog-0.3.3/gdatalog/utils.py
+-rw-r--r--   0        0        0      527 2024-05-10 16:17:15.970401 gdatalog-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      666 1970-01-01 00:00:00.000000 gdatalog-0.3.3/PKG-INFO
```

### Comparing `gdatalog-0.3.2/LICENSE` & `gdatalog-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gdatalog-0.3.2/gdatalog/cli.py` & `gdatalog-0.3.3/gdatalog/cli.py`

 * *Files identical despite different names*

### Comparing `gdatalog-0.3.2/gdatalog/delta_terms.py` & `gdatalog-0.3.3/gdatalog/delta_terms.py`

 * *Files identical despite different names*

### Comparing `gdatalog-0.3.2/gdatalog/program.py` & `gdatalog-0.3.3/gdatalog/program.py`

 * *Files identical despite different names*

### Comparing `gdatalog-0.3.2/gdatalog/utils.py` & `gdatalog-0.3.3/gdatalog/utils.py`

 * *Files identical despite different names*

### Comparing `gdatalog-0.3.2/PKG-INFO` & `gdatalog-0.3.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: gdatalog
-Version: 0.3.2
+Version: 0.3.3
 Summary: Genereative Datalog with stable negation
 Author: Mario Alviano
 Author-email: mario.alviano@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: distlib (>=0.3.6,<0.4.0)
-Requires-Dist: dumbo-asp (>=0.3.6,<0.4.0)
+Requires-Dist: distlib (>=0.3.8,<0.4.0)
+Requires-Dist: dumbo-asp (>=0.3.8,<0.4.0)
+Requires-Dist: fastapi (>=0.111.0,<0.112.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
-Requires-Dist: scipy (>=1.12.0,<2.0.0)
-Requires-Dist: typeguard (>=4.1.5,<5.0.0)
-Requires-Dist: typer (>=0.9.0,<0.10.0)
+Requires-Dist: scipy (>=1.13.0,<2.0.0)
+Requires-Dist: typeguard (>=4.2.1,<5.0.0)
+Requires-Dist: typer (>=0.12.3,<0.13.0)
 Requires-Dist: valid8 (>=5.1.2,<6.0.0)
```

