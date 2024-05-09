# Comparing `tmp/kfsfstr-1.1.0.tar.gz` & `tmp/kfsfstr-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfsfstr-1.1.0.tar", max compression
+gzip compressed data, was "kfsfstr-1.1.1.tar", max compression
```

## Comparing `kfsfstr-1.1.0.tar` & `kfsfstr-1.1.1.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0     8098 2023-10-01 10:29:32.523088 kfsfstr-1.1.0/KFSfstr/KFSfstr.py
--rw-r--r--   0        0        0        0 2023-10-01 10:29:32.523088 kfsfstr-1.1.0/KFSfstr/__init__.py
--rw-r--r--   0        0        0      553 2023-10-01 10:29:32.523088 kfsfstr-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      644 2023-10-01 10:29:32.523088 kfsfstr-1.1.0/readme.md
--rw-r--r--   0        0        0     1236 1970-01-01 00:00:00.000000 kfsfstr-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     8098 2024-05-09 21:34:55.311732 kfsfstr-1.1.1/KFSfstr/KFSfstr.py
+-rw-r--r--   0        0        0      532 2024-05-09 21:34:55.311732 kfsfstr-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      644 2024-05-09 21:34:55.311732 kfsfstr-1.1.1/readme.md
+-rw-r--r--   0        0        0     1197 1970-01-01 00:00:00.000000 kfsfstr-1.1.1/PKG-INFO
```

### Comparing `kfsfstr-1.1.0/KFSfstr/KFSfstr.py` & `kfsfstr-1.1.1/KFSfstr/KFSfstr.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2023 구FS, all rights reserved. Subject to the MIT licence in `licence.md`.
+# Copyright (c) 2024 구FS, all rights reserved. Subject to the MIT licence in `licence.md`.
 import colorama
 import inspect
 import math
 import sys
 from KFSmath import KFSmath
```

### Comparing `kfsfstr-1.1.0/pyproject.toml` & `kfsfstr-1.1.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 authors     = ["9FS <pray4spam@googlemail.com>"]
 description = ""
 license     = "MIT"
 name        = "KFSfstr"
 packages    = [{ include = "KFSfstr" }]
 readme      = "readme.md"
 repository  = "https://github.com/9-FS/2023-09-20-KFSfstr"
-version     = "1.1.0"
+version     = "1.1.1"
 
 [tool.poetry.dependencies]
-colorama = "^0.4.6"
-kfslog   = "^1.0.0"
+colorama = "^0.4.0"
 kfsmath  = "^1.0.0"
-python   = "^3.11.0"
+python   = "^3.12.0"
 
 [tool.poetry.group.dev.dependencies]
-hypothesis = "^6.87.0"
-pytest     = "^7.4.2"
+hypothesis = "^6.0.0"
+pytest     = "^8.0.0"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires      = ["poetry-core"]
```

### Comparing `kfsfstr-1.1.0/readme.md` & `kfsfstr-1.1.1/readme.md`

 * *Files identical despite different names*

