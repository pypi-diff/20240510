# Comparing `tmp/python_glowplug-0.2.5.tar.gz` & `tmp/python_glowplug-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_glowplug-0.2.5.tar", max compression
+gzip compressed data, was "python_glowplug-0.3.0.tar", max compression
```

## Comparing `python_glowplug-0.2.5.tar` & `python_glowplug-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,17 @@
--rw-r--r--   0        0        0     1060 2024-05-10 18:28:45.550413 python_glowplug-0.2.5/LICENSE
--rw-r--r--   0        0        0      561 2024-05-10 19:17:51.575391 python_glowplug-0.2.5/README.md
--rw-r--r--   0        0        0      499 2024-05-10 21:17:44.071044 python_glowplug-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      195 2024-05-10 18:22:44.644755 python_glowplug-0.2.5/src/glowplug/__init__.py
--rw-r--r--   0        0        0     2845 2024-05-10 20:09:03.896403 python_glowplug-0.2.5/src/glowplug/base.py
--rw-r--r--   0        0        0     2635 2024-05-10 21:18:25.176417 python_glowplug-0.2.5/src/glowplug/mssql.py
--rw-r--r--   0        0        0     2600 2024-05-10 18:07:21.425190 python_glowplug-0.2.5/src/glowplug/pg.py
--rw-r--r--   0        0        0     1020 2024-05-10 18:07:21.426500 python_glowplug-0.2.5/src/glowplug/sqlite.py
--rw-r--r--   0        0        0     1257 1970-01-01 00:00:00.000000 python_glowplug-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-05-10 18:28:45.550413 python_glowplug-0.3.0/LICENSE
+-rw-r--r--   0        0        0      561 2024-05-10 19:17:51.575391 python_glowplug-0.3.0/README.md
+-rw-r--r--   0        0        0      540 2024-05-10 21:35:57.015226 python_glowplug-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      378 2024-05-10 21:38:36.780174 python_glowplug-0.3.0/src/glowplug/__init__.py
+-rw-r--r--   0        0        0     1732 2024-05-10 21:38:36.779948 python_glowplug-0.3.0/src/glowplug/config/__init__.py
+-rw-r--r--   0        0        0     3880 2024-05-10 21:37:04.043624 python_glowplug-0.3.0/src/glowplug/config/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2024-05-10 21:34:44.661098 python_glowplug-0.3.0/src/glowplug/driver/__init__.py
+-rw-r--r--   0        0        0      178 2024-05-10 21:36:15.846033 python_glowplug-0.3.0/src/glowplug/driver/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     6373 2024-05-10 21:36:15.848539 python_glowplug-0.3.0/src/glowplug/driver/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     4576 2024-05-10 21:36:17.022664 python_glowplug-0.3.0/src/glowplug/driver/__pycache__/mssql.cpython-311.pyc
+-rw-r--r--   0        0        0     4805 2024-05-10 21:36:17.021555 python_glowplug-0.3.0/src/glowplug/driver/__pycache__/pg.cpython-311.pyc
+-rw-r--r--   0        0        0     2437 2024-05-10 21:36:17.022045 python_glowplug-0.3.0/src/glowplug/driver/__pycache__/sqlite.cpython-311.pyc
+-rw-r--r--   0        0        0     2845 2024-05-10 20:09:03.896403 python_glowplug-0.3.0/src/glowplug/driver/base.py
+-rw-r--r--   0        0        0     2635 2024-05-10 21:18:25.176417 python_glowplug-0.3.0/src/glowplug/driver/mssql.py
+-rw-r--r--   0        0        0     2600 2024-05-10 18:07:21.425190 python_glowplug-0.3.0/src/glowplug/driver/pg.py
+-rw-r--r--   0        0        0     1020 2024-05-10 18:07:21.426500 python_glowplug-0.3.0/src/glowplug/driver/sqlite.py
+-rw-r--r--   0        0        0     1332 1970-01-01 00:00:00.000000 python_glowplug-0.3.0/PKG-INFO
```

### Comparing `python_glowplug-0.2.5/LICENSE` & `python_glowplug-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_glowplug-0.2.5/README.md` & `python_glowplug-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `python_glowplug-0.2.5/src/glowplug/base.py` & `python_glowplug-0.3.0/src/glowplug/driver/base.py`

 * *Files identical despite different names*

### Comparing `python_glowplug-0.2.5/src/glowplug/mssql.py` & `python_glowplug-0.3.0/src/glowplug/driver/mssql.py`

 * *Files identical despite different names*

### Comparing `python_glowplug-0.2.5/src/glowplug/pg.py` & `python_glowplug-0.3.0/src/glowplug/driver/pg.py`

 * *Files identical despite different names*

### Comparing `python_glowplug-0.2.5/src/glowplug/sqlite.py` & `python_glowplug-0.3.0/src/glowplug/driver/sqlite.py`

 * *Files identical despite different names*

### Comparing `python_glowplug-0.2.5/PKG-INFO` & `python_glowplug-0.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: python-glowplug
-Version: 0.2.5
+Version: 0.3.0
 Summary: 
 Home-page: https://github.com/jnu/python-glowplug
 License: MIT
 Author: Joe Nudell
 Author-email: jnudell@hks.harvard.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: alembic (>=1.5,<2.0)
+Requires-Dist: pydantic (>=2,<3)
+Requires-Dist: pydantic-settings (>=2,<3)
 Requires-Dist: sqlalchemy (>=2,<3)
 Project-URL: Repository, https://github.com/jnu/python-glowplug
 Description-Content-Type: text/markdown
 
 Glowplug
 ===
```

