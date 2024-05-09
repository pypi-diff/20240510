# Comparing `tmp/kfssleep-1.0.1.tar.gz` & `tmp/kfssleep-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfssleep-1.0.1.tar", max compression
+gzip compressed data, was "kfssleep-1.0.2.tar", max compression
```

## Comparing `kfssleep-1.0.1.tar` & `kfssleep-1.0.2.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0     2025 2023-09-22 23:25:34.440846 kfssleep-1.0.1/KFSsleep/KFSsleep.py
--rw-r--r--   0        0        0        0 2023-09-22 23:25:34.440846 kfssleep-1.0.1/KFSsleep/__init__.py
--rw-r--r--   0        0        0      419 2023-09-22 23:25:34.440846 kfssleep-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      651 2023-09-22 23:25:34.440846 kfssleep-1.0.1/readme.md
--rw-r--r--   0        0        0     1142 1970-01-01 00:00:00.000000 kfssleep-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2025 2024-05-09 22:40:31.778094 kfssleep-1.0.2/KFSsleep/KFSsleep.py
+-rw-r--r--   0        0        0      515 2024-05-09 22:40:31.778094 kfssleep-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      635 2024-05-09 22:40:31.778094 kfssleep-1.0.2/readme.md
+-rw-r--r--   0        0        0     1110 1970-01-01 00:00:00.000000 kfssleep-1.0.2/PKG-INFO
```

### Comparing `kfssleep-1.0.1/KFSsleep/KFSsleep.py` & `kfssleep-1.0.2/KFSsleep/KFSsleep.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-# Copyright (c) 2023 구FS, all rights reserved. Subject to the MIT licence in `licence.md`.
+# Copyright (c) 2024 구FS, all rights reserved. Subject to the MIT licence in `licence.md`.
 import datetime as dt
 import math
 import time
 
 
 def sleep_mod(sleep_modulus: int) -> None:
     """
     Blockingly sleeps until the current unix time modulus sleep_modulus equals 0.
 
     Arguments:
     - sleep_modulus: the modulus to use to determin when to stop sleeping
     """
 
-    now_DT: dt.datetime     # now
-    return_DT: dt.datetime  # when to return
+    now_dt: dt.datetime     # now
+    return_dt: dt.datetime  # when to return
 
-    now_DT=dt.datetime.now(dt.timezone.utc)
-    return_DT=now_DT-dt.timedelta(seconds=now_DT.timestamp()%sleep_modulus)+dt.timedelta(seconds=sleep_modulus)
+    now_dt=dt.datetime.now(dt.timezone.utc)
+    return_dt=now_dt-dt.timedelta(seconds=now_dt.timestamp()%sleep_modulus)+dt.timedelta(seconds=sleep_modulus)
 
 
-    sleep_until(return_DT)  # sleep until calculated return time
+    sleep_until(return_dt)  # sleep until calculated return time
 
     return
 
 
-def sleep_until(return_DT: dt.datetime) -> None:
+def sleep_until(return_dt: dt.datetime) -> None:
     """
     Blockingly sleeps until the specified datetime and then returns. Expects timezone-aware datetime object.
 
     Arguments:
-    - return_DT: the datetime when to return
+    - return_dt: the datetime when to return
     """
 
-    now_DT: dt.datetime             # now
+    now_dt: dt.datetime             # now
     time_until_return: dt.timedelta # how long still until return
     time_to_sleep: float            # how many seconds is next sleep? depends on time_until_return magnitude
 
 
-    while (now_DT:=dt.datetime.now(dt.timezone.utc))<return_DT:                             # as long as return datetime not reached yet: sleep
-        time_until_return=return_DT-now_DT                                                  # update time until return
+    while (now_dt:=dt.datetime.now(dt.timezone.utc))<return_dt:                             # as long as return datetime not reached yet: sleep
+        time_until_return=return_dt-now_dt                                                  # update time until return
         try:
             time_to_sleep=10**(math.floor(math.log10(time_until_return.total_seconds()))-1) # time to sleep is 1 magnitude smaller than time until return
         except ValueError:                                                                  # in case time until return is exactly 0: log10 crashes, give time to sleep 0
             time_to_sleep=0
         if time_to_sleep<1e-3:
             time_to_sleep=1e-3                                                              # sleep at least 1ms, otherwise needlessly computing for anyways inaccurate result
```

### Comparing `kfssleep-1.0.1/readme.md` & `kfssleep-1.0.2/readme.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ---
-Topic: "KFSsleep Library"
+Topic: "KFSsleep"
 Author: "구FS"
 ---
 <link href="./doc_templates/md_style.css" rel="stylesheet"></link>
 <body>
 
-# <p style="text-align: center;">KFSsleep Library</p>
+# <p style="text-align: center;">KFSsleep</p>
 <br>
 <br>
 
 - [1. General](#1-general)
 - [2. Installation](#2-installation)
 
 ## 1. General
```

### Comparing `kfssleep-1.0.1/PKG-INFO` & `kfssleep-1.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: KFSsleep
-Version: 1.0.1
+Version: 1.0.2
 Summary: 
-Home-page: https://github.com/9-FS/2023-09-20-KFSsleep-Library
+Home-page: https://github.com/9-FS/2023-09-20-KFSsleep
 License: MIT
 Author: 9FS
 Author-email: pray4spam@googlemail.com
-Requires-Python: >=3.11.0,<4.0.0
+Requires-Python: >=3.12.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Project-URL: Repository, https://github.com/9-FS/2023-09-20-KFSsleep-Library
+Classifier: Programming Language :: Python :: 3.12
+Project-URL: Repository, https://github.com/9-FS/2023-09-20-KFSsleep
 Description-Content-Type: text/markdown
 
 ---
-Topic: "KFSsleep Library"
+Topic: "KFSsleep"
 Author: "구FS"
 ---
 <link href="./doc_templates/md_style.css" rel="stylesheet"></link>
 <body>
 
-# <p style="text-align: center;">KFSsleep Library</p>
+# <p style="text-align: center;">KFSsleep</p>
 <br>
 <br>
 
 - [1. General](#1-general)
 - [2. Installation](#2-installation)
 
 ## 1. General
```

