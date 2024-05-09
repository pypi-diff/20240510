# Comparing `tmp/kfsmedia-2.5.1.tar.gz` & `tmp/kfsmedia-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfsmedia-2.5.1.tar", max compression
+gzip compressed data, was "kfsmedia-2.5.2.tar", max compression
```

## Comparing `kfsmedia-2.5.1.tar` & `kfsmedia-2.5.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    27160 2024-02-13 15:53:16.055019 kfsmedia-2.5.1/KFSmedia/KFSmedia.py
--rw-r--r--   0        0        0      617 2024-02-13 15:53:16.055019 kfsmedia-2.5.1/pyproject.toml
--rw-r--r--   0        0        0      635 2024-02-13 15:53:16.055019 kfsmedia-2.5.1/readme.md
--rw-r--r--   0        0        0     1349 1970-01-01 00:00:00.000000 kfsmedia-2.5.1/PKG-INFO
+-rw-r--r--   0        0        0    27160 2024-05-09 22:33:40.650922 kfsmedia-2.5.2/KFSmedia/KFSmedia.py
+-rw-r--r--   0        0        0      616 2024-05-09 22:33:40.650922 kfsmedia-2.5.2/pyproject.toml
+-rw-r--r--   0        0        0      635 2024-05-09 22:33:40.650922 kfsmedia-2.5.2/readme.md
+-rw-r--r--   0        0        0     1349 1970-01-01 00:00:00.000000 kfsmedia-2.5.2/PKG-INFO
```

### Comparing `kfsmedia-2.5.1/KFSmedia/KFSmedia.py` & `kfsmedia-2.5.2/KFSmedia/KFSmedia.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2023 구FS, all rights reserved. Subject to the MIT licence in `licence.md`.
+# Copyright (c) 2024 구FS, all rights reserved. Subject to the MIT licence in `licence.md`.
 import asyncio
 import copy
 import inspect
 import io                               # PDF byte stream
 from KFSfstr import KFSfstr
 from KFSlog import KFSlog
 import logging
```

### Comparing `kfsmedia-2.5.1/pyproject.toml` & `kfsmedia-2.5.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 authors     = ["9FS <pray4spam@googlemail.com>"]
 description = ""
 license     = "MIT"
 name        = "KFSmedia"
 packages    = [{ include = "KFSmedia" }]
 readme      = "readme.md"
 repository  = "https://github.com/9-FS/2023-09-20-KFSmedia"
-version     = "2.5.1"
+version     = "2.5.2"
 
 [tool.poetry.dependencies]
 kfsfstr  = "^1.1.0"
-kfslog   = "^1.0.0"
+kfslog   = "^2.0.0"
 olefile  = "^0.47"
-pebble   = "^5.0.3"
+pebble   = "^5.0.0"
 pillow   = "^10.2.0"
 python   = "^3.12.0"
 requests = "^2.31.0"
 
 [tool.poetry.group.dev.dependencies]
-hypothesis = "^6.87.0"
-pytest     = "^7.4.2"
+hypothesis = "^6.0.0"
+pytest     = "^8.0.0"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires      = ["poetry-core"]
```

### Comparing `kfsmedia-2.5.1/readme.md` & `kfsmedia-2.5.2/readme.md`

 * *Files identical despite different names*

### Comparing `kfsmedia-2.5.1/PKG-INFO` & `kfsmedia-2.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: KFSmedia
-Version: 2.5.1
+Version: 2.5.2
 Summary: 
 Home-page: https://github.com/9-FS/2023-09-20-KFSmedia
 License: MIT
 Author: 9FS
 Author-email: pray4spam@googlemail.com
 Requires-Python: >=3.12.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: kfsfstr (>=1.1.0,<2.0.0)
-Requires-Dist: kfslog (>=1.0.0,<2.0.0)
+Requires-Dist: kfslog (>=2.0.0,<3.0.0)
 Requires-Dist: olefile (>=0.47,<0.48)
-Requires-Dist: pebble (>=5.0.3,<6.0.0)
+Requires-Dist: pebble (>=5.0.0,<6.0.0)
 Requires-Dist: pillow (>=10.2.0,<11.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/9-FS/2023-09-20-KFSmedia
 Description-Content-Type: text/markdown
 
 ---
 Topic: "KFSmedia"
```

