# Comparing `tmp/work-1.1.0b1.tar.gz` & `tmp/work-1.1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "work-1.1.0b1.tar", max compression
+gzip compressed data, was "work-1.1.0b2.tar", max compression
```

## Comparing `work-1.1.0b1.tar` & `work-1.1.0b2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1033 2022-08-29 19:21:01.200221 work-1.1.0b1/README.md
--rw-r--r--   0        0        0      594 2024-05-10 14:25:40.109274 work-1.1.0b1/pyproject.toml
--rw-r--r--   0        0        0    91750 2024-05-10 14:24:35.320649 work-1.1.0b1/src/work.py
--rw-r--r--   0        0        0        0 2021-02-24 12:12:04.352563 work-1.1.0b1/src/work_components/__init__.py
--rw-r--r--   0        0        0    24509 2024-05-10 10:13:29.676889 work-1.1.0b1/src/work_components/arguments.py
--rw-r--r--   0        0        0     2188 2024-05-10 14:25:32.289198 work-1.1.0b1/src/work_components/consts.py
--rw-r--r--   0        0        0    22908 2024-05-10 14:13:32.158045 work-1.1.0b1/src/work_components/container.py
--rw-r--r--   0        0        0        0 2022-08-23 18:01:16.135701 work-1.1.0b1/src/work_components/dao/__init__.py
--rw-r--r--   0        0        0    16504 2024-05-10 14:24:35.320649 work-1.1.0b1/src/work_components/dao/core.py
--rw-r--r--   0        0        0      268 2024-05-09 22:17:55.296856 work-1.1.0b1/src/work_components/dao/env.py
--rw-r--r--   0        0        0     1641 2024-05-09 22:17:55.296856 work-1.1.0b1/src/work_components/dao/flags.py
--rw-r--r--   0        0        0     8513 2024-05-09 22:17:55.296856 work-1.1.0b1/src/work_components/dao/rc.py
--rw-r--r--   0        0        0    10484 2024-05-09 22:17:55.296856 work-1.1.0b1/src/work_components/dao/recess.py
--rw-r--r--   0        0        0     1734 2024-05-09 22:17:55.296856 work-1.1.0b1/src/work_components/dt_format.py
--rw-r--r--   0        0        0     6236 2024-05-09 22:17:55.296856 work-1.1.0b1/src/work_components/dt_parse.py
--rw-r--r--   0        0        0     3982 2024-05-10 14:24:35.320649 work-1.1.0b1/src/work_components/migrate.py
--rw-r--r--   0        0        0      525 2024-05-10 14:24:35.320649 work-1.1.0b1/src/work_components/protocols.py
--rw-r--r--   0        0        0     2660 2024-05-10 14:24:35.320649 work-1.1.0b1/src/work_components/timestamps.py
--rw-r--r--   0        0        0     8065 2024-05-09 22:17:55.300856 work-1.1.0b1/src/work_components/util.py
--rw-r--r--   0        0        0     1614 1970-01-01 00:00:00.000000 work-1.1.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1033 2022-08-29 19:21:01.200221 work-1.1.0b2/README.md
+-rw-r--r--   0        0        0      594 2024-05-10 14:30:49.868234 work-1.1.0b2/pyproject.toml
+-rw-r--r--   0        0        0    91750 2024-05-10 14:24:35.320649 work-1.1.0b2/src/work.py
+-rw-r--r--   0        0        0        0 2021-02-24 12:12:04.352563 work-1.1.0b2/src/work_components/__init__.py
+-rw-r--r--   0        0        0    24509 2024-05-10 10:13:29.676889 work-1.1.0b2/src/work_components/arguments.py
+-rw-r--r--   0        0        0     2188 2024-05-10 14:30:55.752290 work-1.1.0b2/src/work_components/consts.py
+-rw-r--r--   0        0        0    22908 2024-05-10 14:13:32.158045 work-1.1.0b2/src/work_components/container.py
+-rw-r--r--   0        0        0        0 2022-08-23 18:01:16.135701 work-1.1.0b2/src/work_components/dao/__init__.py
+-rw-r--r--   0        0        0    16504 2024-05-10 14:24:35.320649 work-1.1.0b2/src/work_components/dao/core.py
+-rw-r--r--   0        0        0      268 2024-05-09 22:17:55.296856 work-1.1.0b2/src/work_components/dao/env.py
+-rw-r--r--   0        0        0     1641 2024-05-09 22:17:55.296856 work-1.1.0b2/src/work_components/dao/flags.py
+-rw-r--r--   0        0        0     8513 2024-05-09 22:17:55.296856 work-1.1.0b2/src/work_components/dao/rc.py
+-rw-r--r--   0        0        0    10484 2024-05-09 22:17:55.296856 work-1.1.0b2/src/work_components/dao/recess.py
+-rw-r--r--   0        0        0     1734 2024-05-09 22:17:55.296856 work-1.1.0b2/src/work_components/dt_format.py
+-rw-r--r--   0        0        0     6236 2024-05-09 22:17:55.296856 work-1.1.0b2/src/work_components/dt_parse.py
+-rw-r--r--   0        0        0     4007 2024-05-10 14:30:08.803844 work-1.1.0b2/src/work_components/migrate.py
+-rw-r--r--   0        0        0      525 2024-05-10 14:24:35.320649 work-1.1.0b2/src/work_components/protocols.py
+-rw-r--r--   0        0        0     2660 2024-05-10 14:24:35.320649 work-1.1.0b2/src/work_components/timestamps.py
+-rw-r--r--   0        0        0     8065 2024-05-09 22:17:55.300856 work-1.1.0b2/src/work_components/util.py
+-rw-r--r--   0        0        0     1614 1970-01-01 00:00:00.000000 work-1.1.0b2/PKG-INFO
```

### Comparing `work-1.1.0b1/README.md` & `work-1.1.0b2/README.md`

 * *Files identical despite different names*

### Comparing `work-1.1.0b1/pyproject.toml` & `work-1.1.0b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "work"
-version = "1.1.0b1"
+version = "1.1.0b2"
 description = "Manual time tracking via a CLI that works similarly to git."
 authors = ["vauhochzett <vauhoch@zett.cc>"]
 readme = "README.md"
 homepage = "https://vauhoch.zett.cc/work/"
 packages = [
     { include = "work.py", from = "src" },
     { include = "work_components", from = "src" },
```

### Comparing `work-1.1.0b1/src/work.py` & `work-1.1.0b2/src/work.py`

 * *Files identical despite different names*

### Comparing `work-1.1.0b1/src/work_components/arguments.py` & `work-1.1.0b2/src/work_components/arguments.py`

 * *Files identical despite different names*

### Comparing `work-1.1.0b1/src/work_components/consts.py` & `work-1.1.0b2/src/work_components/consts.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """Shared constants"""
 
 import os
 import pathlib
 from typing import List, Tuple
 
-VERSION: str = "1.1.0b1"
+VERSION: str = "1.1.0b2"
 RECORDS_VERSION: int = 3
 
 # Directories
 PARENT_DIR: pathlib.Path = pathlib.Path("~", ".local", "share").expanduser()
 DIRECTORY: pathlib.Path = PARENT_DIR.joinpath("work")
 DIRECTORY_DEBUG: pathlib.Path = PARENT_DIR.joinpath("debug", "work")
```

### Comparing `work-1.1.0b1/src/work_components/container.py` & `work-1.1.0b2/src/work_components/container.py`

 * *Files identical despite different names*

### Comparing `work-1.1.0b1/src/work_components/dao/core.py` & `work-1.1.0b2/src/work_components/dao/core.py`

 * *Files identical despite different names*

### Comparing `work-1.1.0b1/src/work_components/dao/flags.py` & `work-1.1.0b2/src/work_components/dao/flags.py`

 * *Files identical despite different names*

### Comparing `work-1.1.0b1/src/work_components/dao/rc.py` & `work-1.1.0b2/src/work_components/dao/rc.py`

 * *Files identical despite different names*

### Comparing `work-1.1.0b1/src/work_components/dao/recess.py` & `work-1.1.0b2/src/work_components/dao/recess.py`

 * *Files identical despite different names*

### Comparing `work-1.1.0b1/src/work_components/dt_format.py` & `work-1.1.0b2/src/work_components/dt_format.py`

 * *Files identical despite different names*

### Comparing `work-1.1.0b1/src/work_components/dt_parse.py` & `work-1.1.0b2/src/work_components/dt_parse.py`

 * *Files identical despite different names*

### Comparing `work-1.1.0b1/src/work_components/migrate.py` & `work-1.1.0b2/src/work_components/migrate.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 
 def offer_midnight_migration_if_not_denied(flags: IFlags, dao: IMigratable):
     """Hint at migrate functionality if that was not denied."""
     migration_flag: str = "migrate:records_touching_midnight"
     if flags.is_set(migration_flag):
         return
+    flags.set(migration_flag)
 
     print(
         textwrap.indent(
             "\nNote: work now handles runs that end at or extend beyond midnight.\n\n"
             "If you have previously worked around the missing functionality by\n"
             "ending runs at, e.g., 23:59, they can be automatically migrated.\n\n",
             prefix="  ",
@@ -28,15 +29,15 @@
             "Press [Enter] to ask again on next startup,\n"
             'Enter "deny" to permanently disable this message, or\n'
             'Enter "migrate" to start migration.\n'
         )
     )
     user_says: str = input("> ").strip().casefold()
     if user_says == "deny":
-        flags.set(migration_flag)
+        # Flag was set above
         return
     elif user_says != "migrate":
         flags.remove(migration_flag)
         print("Deferred.")
         return
 
     # User has requested migration
```

### Comparing `work-1.1.0b1/src/work_components/protocols.py` & `work-1.1.0b2/src/work_components/protocols.py`

 * *Files identical despite different names*

### Comparing `work-1.1.0b1/src/work_components/timestamps.py` & `work-1.1.0b2/src/work_components/timestamps.py`

 * *Files identical despite different names*

### Comparing `work-1.1.0b1/src/work_components/util.py` & `work-1.1.0b2/src/work_components/util.py`

 * *Files identical despite different names*

### Comparing `work-1.1.0b1/PKG-INFO` & `work-1.1.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: work
-Version: 1.1.0b1
+Version: 1.1.0b2
 Summary: Manual time tracking via a CLI that works similarly to git.
 Home-page: https://vauhoch.zett.cc/work/
 Author: vauhochzett
 Author-email: vauhoch@zett.cc
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

