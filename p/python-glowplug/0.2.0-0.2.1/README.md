# Comparing `tmp/python_glowplug-0.2.0.tar.gz` & `tmp/python_glowplug-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_glowplug-0.2.0.tar", max compression
+gzip compressed data, was "python_glowplug-0.2.1.tar", max compression
```

## Comparing `python_glowplug-0.2.0.tar` & `python_glowplug-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1060 2024-05-10 18:28:45.550413 python_glowplug-0.2.0/LICENSE
--rw-r--r--   0        0        0      561 2024-05-10 19:17:51.575391 python_glowplug-0.2.0/README.md
--rw-r--r--   0        0        0      499 2024-05-10 19:16:21.052178 python_glowplug-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      195 2024-05-10 18:22:44.644755 python_glowplug-0.2.0/src/glowplug/__init__.py
--rw-r--r--   0        0        0     2800 2024-05-10 19:18:04.572166 python_glowplug-0.2.0/src/glowplug/base.py
--rw-r--r--   0        0        0     2094 2024-05-10 18:24:29.874971 python_glowplug-0.2.0/src/glowplug/mssql.py
--rw-r--r--   0        0        0     2600 2024-05-10 18:07:21.425190 python_glowplug-0.2.0/src/glowplug/pg.py
--rw-r--r--   0        0        0     1020 2024-05-10 18:07:21.426500 python_glowplug-0.2.0/src/glowplug/sqlite.py
--rw-r--r--   0        0        0     1257 1970-01-01 00:00:00.000000 python_glowplug-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-05-10 18:28:45.550413 python_glowplug-0.2.1/LICENSE
+-rw-r--r--   0        0        0      561 2024-05-10 19:17:51.575391 python_glowplug-0.2.1/README.md
+-rw-r--r--   0        0        0      499 2024-05-10 20:09:09.267101 python_glowplug-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      195 2024-05-10 18:22:44.644755 python_glowplug-0.2.1/src/glowplug/__init__.py
+-rw-r--r--   0        0        0     2845 2024-05-10 20:09:03.896403 python_glowplug-0.2.1/src/glowplug/base.py
+-rw-r--r--   0        0        0     2094 2024-05-10 18:24:29.874971 python_glowplug-0.2.1/src/glowplug/mssql.py
+-rw-r--r--   0        0        0     2600 2024-05-10 18:07:21.425190 python_glowplug-0.2.1/src/glowplug/pg.py
+-rw-r--r--   0        0        0     1020 2024-05-10 18:07:21.426500 python_glowplug-0.2.1/src/glowplug/sqlite.py
+-rw-r--r--   0        0        0     1257 1970-01-01 00:00:00.000000 python_glowplug-0.2.1/PKG-INFO
```

### Comparing `python_glowplug-0.2.0/LICENSE` & `python_glowplug-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_glowplug-0.2.0/README.md` & `python_glowplug-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `python_glowplug-0.2.0/src/glowplug/base.py` & `python_glowplug-0.2.1/src/glowplug/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from abc import ABC, abstractmethod
 from functools import cached_property
 from typing import Any
 
 import alembic
+import alembic.command
+import alembic.config
 from sqlalchemy import Engine, create_engine
 from sqlalchemy.ext.asyncio import (
     AsyncEngine,
     AsyncSession,
     async_sessionmaker,
     create_async_engine,
 )
```

### Comparing `python_glowplug-0.2.0/src/glowplug/mssql.py` & `python_glowplug-0.2.1/src/glowplug/mssql.py`

 * *Files identical despite different names*

### Comparing `python_glowplug-0.2.0/src/glowplug/pg.py` & `python_glowplug-0.2.1/src/glowplug/pg.py`

 * *Files identical despite different names*

### Comparing `python_glowplug-0.2.0/src/glowplug/sqlite.py` & `python_glowplug-0.2.1/src/glowplug/sqlite.py`

 * *Files identical despite different names*

### Comparing `python_glowplug-0.2.0/PKG-INFO` & `python_glowplug-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-glowplug
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Home-page: https://github.com/jnu/python-glowplug
 License: MIT
 Author: Joe Nudell
 Author-email: jnudell@hks.harvard.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

