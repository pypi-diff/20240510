# Comparing `tmp/kfsconvert_to_si-1.0.1.tar.gz` & `tmp/kfsconvert_to_si-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfsconvert_to_si-1.0.1.tar", max compression
+gzip compressed data, was "kfsconvert_to_si-1.0.2.tar", max compression
```

## Comparing `kfsconvert_to_si-1.0.1.tar` & `kfsconvert_to_si-1.0.2.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0     1831 2023-09-22 23:03:04.613872 kfsconvert_to_si-1.0.1/KFSconvert_to_SI/KFSconvert_to_SI.py
--rw-r--r--   0        0        0        0 2023-09-22 23:03:04.613872 kfsconvert_to_si-1.0.1/KFSconvert_to_SI/__init__.py
--rw-r--r--   0        0        0      443 2023-09-22 23:03:04.613872 kfsconvert_to_si-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      683 2023-09-22 23:03:04.613872 kfsconvert_to_si-1.0.1/readme.md
--rw-r--r--   0        0        0     1198 1970-01-01 00:00:00.000000 kfsconvert_to_si-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1831 2024-05-09 22:27:08.732741 kfsconvert_to_si-1.0.2/KFSconvert_to_SI/KFSconvert_to_SI.py
+-rw-r--r--   0        0        0      539 2024-05-09 22:27:08.732741 kfsconvert_to_si-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      667 2024-05-09 22:27:08.732741 kfsconvert_to_si-1.0.2/readme.md
+-rw-r--r--   0        0        0     1166 1970-01-01 00:00:00.000000 kfsconvert_to_si-1.0.2/PKG-INFO
```

### Comparing `kfsconvert_to_si-1.0.1/KFSconvert_to_SI/KFSconvert_to_SI.py` & `kfsconvert_to_si-1.0.2/KFSconvert_to_SI/KFSconvert_to_SI.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2023 구FS, all rights reserved. Subject to the MIT licence in `licence.md`.
+# Copyright (c) 2024 구FS, all rights reserved. Subject to the MIT licence in `licence.md`.
 LENGTH={        # m
     "ft": 0.3048,
     "in": 0.0254,
     "NM": 1852,
     "SM": 1609.344,
     "yd": 0.9144
 }
```

### Comparing `kfsconvert_to_si-1.0.1/readme.md` & `kfsconvert_to_si-1.0.2/readme.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ---
-Topic: "KFSconvert_to_SI Library"
+Topic: "KFSconvert_to_SI"
 Author: "구FS"
 ---
 <link href="./doc_templates/md_style.css" rel="stylesheet"></link>
 <body>
 
-# <p style="text-align: center;">KFSconvert_to_SI Library</p>
+# <p style="text-align: center;">KFSconvert_to_SI</p>
 <br>
 <br>
 
 - [1. General](#1-general)
 - [2. Installation](#2-installation)
 
 ## 1. General
```

### Comparing `kfsconvert_to_si-1.0.1/PKG-INFO` & `kfsconvert_to_si-1.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: KFSconvert_to_SI
-Version: 1.0.1
+Version: 1.0.2
 Summary: 
-Home-page: https://github.com/9-FS/2023-09-20-KFSconvert_to_SI-Library
+Home-page: https://github.com/9-FS/2023-09-20-KFSconvert_to_SI
 License: MIT
 Author: 9FS
 Author-email: pray4spam@googlemail.com
-Requires-Python: >=3.11.0,<4.0.0
+Requires-Python: >=3.12.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Project-URL: Repository, https://github.com/9-FS/2023-09-20-KFSconvert_to_SI-Library
+Classifier: Programming Language :: Python :: 3.12
+Project-URL: Repository, https://github.com/9-FS/2023-09-20-KFSconvert_to_SI
 Description-Content-Type: text/markdown
 
 ---
-Topic: "KFSconvert_to_SI Library"
+Topic: "KFSconvert_to_SI"
 Author: "구FS"
 ---
 <link href="./doc_templates/md_style.css" rel="stylesheet"></link>
 <body>
 
-# <p style="text-align: center;">KFSconvert_to_SI Library</p>
+# <p style="text-align: center;">KFSconvert_to_SI</p>
 <br>
 <br>
 
 - [1. General](#1-general)
 - [2. Installation](#2-installation)
 
 ## 1. General
```

