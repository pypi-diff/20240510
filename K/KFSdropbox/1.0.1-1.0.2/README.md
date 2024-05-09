# Comparing `tmp/kfsdropbox-1.0.1.tar.gz` & `tmp/kfsdropbox-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfsdropbox-1.0.1.tar", max compression
+gzip compressed data, was "kfsdropbox-1.0.2.tar", max compression
```

## Comparing `kfsdropbox-1.0.1.tar` & `kfsdropbox-1.0.2.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0     4725 2023-09-22 23:08:21.535684 kfsdropbox-1.0.1/KFSdropbox/KFSdropbox.py
--rw-r--r--   0        0        0        0 2023-09-22 23:08:21.535684 kfsdropbox-1.0.1/KFSdropbox/__init__.py
--rw-r--r--   0        0        0      447 2023-09-22 23:08:21.535684 kfsdropbox-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      659 2023-09-22 23:08:21.535684 kfsdropbox-1.0.1/readme.md
--rw-r--r--   0        0        0     1199 1970-01-01 00:00:00.000000 kfsdropbox-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     4725 2024-05-09 22:43:17.297458 kfsdropbox-1.0.2/KFSdropbox/KFSdropbox.py
+-rw-r--r--   0        0        0      543 2024-05-09 22:43:17.297458 kfsdropbox-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      643 2024-05-09 22:43:17.297458 kfsdropbox-1.0.2/readme.md
+-rw-r--r--   0        0        0     1167 1970-01-01 00:00:00.000000 kfsdropbox-1.0.2/PKG-INFO
```

### Comparing `kfsdropbox-1.0.1/KFSdropbox/KFSdropbox.py` & `kfsdropbox-1.0.2/KFSdropbox/KFSdropbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2023 구FS, all rights reserved. Subject to the MIT licence in `licence.md`.
+# Copyright (c) 2024 구FS, all rights reserved. Subject to the MIT licence in `licence.md`.
 import dropbox.dropbox_client, dropbox.exceptions, dropbox.files
 import os
 import requests
 import time
 
 
 def list_files(dbx: dropbox.dropbox_client.Dropbox, path: str, not_exist_ok=True) -> list[str]:
```

### Comparing `kfsdropbox-1.0.1/readme.md` & `kfsdropbox-1.0.2/readme.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ---
-Topic: "KFSdropbox Library"
+Topic: "KFSdropbox"
 Author: "구FS"
 ---
 <link href="./doc_templates/md_style.css" rel="stylesheet"></link>
 <body>
 
-# <p style="text-align: center;">KFSdropbox Library</p>
+# <p style="text-align: center;">KFSdropbox</p>
 <br>
 <br>
 
 - [1. General](#1-general)
 - [2. Installation](#2-installation)
 
 ## 1. General
```

### Comparing `kfsdropbox-1.0.1/PKG-INFO` & `kfsdropbox-1.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: KFSdropbox
-Version: 1.0.1
+Version: 1.0.2
 Summary: 
-Home-page: https://github.com/9-FS/2023-09-20-KFSdropbox-Library
+Home-page: https://github.com/9-FS/2023-09-20-KFSdropbox
 License: MIT
 Author: 9FS
 Author-email: pray4spam@googlemail.com
-Requires-Python: >=3.11.0,<4.0.0
+Requires-Python: >=3.12.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: dropbox (>=11.36.2,<12.0.0)
-Project-URL: Repository, https://github.com/9-FS/2023-09-20-KFSdropbox-Library
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: dropbox (>=11.36.0,<12.0.0)
+Project-URL: Repository, https://github.com/9-FS/2023-09-20-KFSdropbox
 Description-Content-Type: text/markdown
 
 ---
-Topic: "KFSdropbox Library"
+Topic: "KFSdropbox"
 Author: "구FS"
 ---
 <link href="./doc_templates/md_style.css" rel="stylesheet"></link>
 <body>
 
-# <p style="text-align: center;">KFSdropbox Library</p>
+# <p style="text-align: center;">KFSdropbox</p>
 <br>
 <br>
 
 - [1. General](#1-general)
 - [2. Installation](#2-installation)
 
 ## 1. General
```

