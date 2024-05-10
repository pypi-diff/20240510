# Comparing `tmp/ddir-3.0.1-py3-none-any.whl.zip` & `tmp/ddir-3.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 14114 bytes, number of entries: 13
--rw-r--r--  2.0 unx     4924 b- defN 24-Mar-04 09:14 ddir/__init__.py
--rw-r--r--  2.0 unx     4445 b- defN 24-Mar-04 09:14 ddir/__main__.py
--rw-r--r--  2.0 unx      156 b- defN 24-Mar-04 09:14 ddir/__version__.py
--rw-r--r--  2.0 unx    12161 b- defN 24-Mar-04 09:14 ddir/diff.py
--rw-r--r--  2.0 unx      673 b- defN 24-Mar-04 09:14 ddir/initialize.py
--rw-r--r--  2.0 unx     2600 b- defN 24-Mar-04 09:14 ddir/legacy.py
--rw-r--r--  2.0 unx     5828 b- defN 24-Mar-04 09:14 ddir/target.py
--rw-r--r--  2.0 unx      191 b- defN 24-Mar-04 09:14 ddir-3.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     3933 b- defN 24-Mar-04 09:14 ddir-3.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-04 09:14 ddir-3.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       44 b- defN 24-Mar-04 09:14 ddir-3.0.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 24-Mar-04 09:14 ddir-3.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      968 b- defN 24-Mar-04 09:14 ddir-3.0.1.dist-info/RECORD
-13 files, 36020 bytes uncompressed, 12524 bytes compressed:  65.2%
+Zip file size: 14354 bytes, number of entries: 13
+-rw-r--r--  2.0 unx     4924 b- defN 24-May-10 16:32 ddir/__init__.py
+-rw-r--r--  2.0 unx     4445 b- defN 24-May-10 16:32 ddir/__main__.py
+-rw-r--r--  2.0 unx      156 b- defN 24-May-10 16:32 ddir/__version__.py
+-rw-r--r--  2.0 unx    11931 b- defN 24-May-10 16:32 ddir/diff.py
+-rw-r--r--  2.0 unx      673 b- defN 24-May-10 16:32 ddir/initialize.py
+-rw-r--r--  2.0 unx     2600 b- defN 24-May-10 16:32 ddir/legacy.py
+-rw-r--r--  2.0 unx     5828 b- defN 24-May-10 16:32 ddir/target.py
+-rw-r--r--  2.0 unx     1211 b- defN 24-May-10 16:32 ddir-3.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3622 b- defN 24-May-10 16:32 ddir-3.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-10 16:32 ddir-3.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       44 b- defN 24-May-10 16:32 ddir-3.1.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 24-May-10 16:32 ddir-3.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      969 b- defN 24-May-10 16:32 ddir-3.1.0.dist-info/RECORD
+13 files, 36500 bytes uncompressed, 12764 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: ddir/legacy.py
 Comment: 
 
 Filename: ddir/target.py
 Comment: 
 
-Filename: ddir-3.0.1.dist-info/LICENSE
+Filename: ddir-3.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: ddir-3.0.1.dist-info/METADATA
+Filename: ddir-3.1.0.dist-info/METADATA
 Comment: 
 
-Filename: ddir-3.0.1.dist-info/WHEEL
+Filename: ddir-3.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: ddir-3.0.1.dist-info/entry_points.txt
+Filename: ddir-3.1.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: ddir-3.0.1.dist-info/top_level.txt
+Filename: ddir-3.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: ddir-3.0.1.dist-info/RECORD
+Filename: ddir-3.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ddir/__version__.py

```diff
@@ -1,7 +1,7 @@
 """
 This module holds the version of ddir.
 
 It contains a placeholder for the version number, which is replaced by the build script.
 """
 
-VERSION = '3.0.1'
+VERSION = '3.1.0'
```

## ddir/diff.py

```diff
@@ -4,18 +4,17 @@
 All diffs are stored in `*.diff` files located in each targets subdirectory in
 `.ddir/target.d`. Diffs can be created and resolved.
 """
 
 from __future__ import annotations
 
 from dataclasses import dataclass
-from datetime import date
+from datetime import date, datetime
 from enum import Enum
 from hashlib import md5
-from math import ceil
 from os import sep, listdir, mkdir, stat
 from os.path import exists, isfile, isdir
 from random import randint as rand
 from re import match
 from shutil import copy2 as cp
 from time import localtime, strftime
 from typing import List
@@ -255,38 +254,34 @@
 
 
 def _create_for_file(diff: DiffFileCreator, source: str, target: str, fast: bool) -> None:
     if not exists(target):
         print(f'file not in target: {source} {target}')
         diff.add_diff(Diff(DiffType.POSITIVE, 'f', source, target))
     else:
-        # It may occur that the source modification time has a higher/lower
-        # precision than the target modification time. As rounding to e.g. 2
-        # decimal places may lead to a difference of .01, we round to the
-        # ceiling to avoid false positives.
-        source_last_changed = ceil(stat(source).st_mtime)
-        target_last_changed = ceil(stat(target).st_mtime)
-
-        # Here, we check if the files are different by more than one second.
-        # This is because on some file systems, the modification time may be
-        # different by one second, even if the file has not been changed.
-        if source_last_changed - target_last_changed > 1:
-            print(f'files differ: {source} is newer than {target}')
+        source_last_changed = stat(source).st_mtime
+        target_last_changed = stat(target).st_mtime
+
+        source_last_changed_str = datetime.fromtimestamp(source_last_changed).isoformat()
+        target_last_changed_str = datetime.fromtimestamp(target_last_changed).isoformat()
+
+        if source_last_changed > target_last_changed:
+            print(f'[metadata] files differ: {source} is newer than {target} ({source_last_changed_str} > {target_last_changed_str})')
             diff.add_diff(Diff(DiffType.NEWER, 'f', source, target))
-        elif target_last_changed - source_last_changed > 1:
-            print(f'files differ: {target} is newer than {source}')
+        elif target_last_changed > source_last_changed:
+            print(f'[metadata] files differ: {target} is newer than {source} ({target_last_changed_str} > {source_last_changed_str})')
             diff.add_diff(Diff(DiffType.OLDER, 'f', source, target))
         elif not fast:
             with open(source, 'rb', encoding=ENCODING) as source_file, \
                     open(target, 'rb', encoding=ENCODING) as target_file:
                 source_md5 = md5(source_file.read()).hexdigest()
                 target_md5 = md5(target_file.read()).hexdigest()
 
                 if source_md5 != target_md5:
-                    print(f'files differ: {source} (change dates are equal)')
+                    print(f'[content ] files differ: {source}')
                     diff.add_diff(Diff(DiffType.UNKNOWN, 'f', source, target))
 
 
 def resolve(reader: DiffFileReader, modes=(0, 0, 0, 0, 0)) -> None:
     """Resolves all diffs from a given diff file.
 
     The modes work like this: for each type (the order is "+", "-", ">", "<", "?")
```

## Comparing `ddir-3.0.1.dist-info/METADATA` & `ddir-3.1.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddir
-Version: 3.0.1
+Version: 3.1.0
 Summary: Diff a directory and sync changes.
 License: Public Domain
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ddir
 
@@ -23,15 +23,18 @@
 `pip install ddir`
 
 This will install a binary called `ddir` on your `PATH` that you can execute.
 Depending on your system, you may need sudo/admin permissions.
 
 ### Installation on macOS
 
-In case you're using Homebrew, the installation via pip fails (at least on my machine). In that case, create a virtual environment and install `ddir` in there. The `venv` directory will be set ignored when initializing a new directory. In case you have `ddir`-controlled directory that has been initialized with an older version, please add `venv` to `.ddir/ddir.json`.
+```bash
+brew tap yannickkirschen/tap
+brew install ddir
+```
 
 ## Usage
 
 ```txt
 Usage: ddir <commands>
 
 Available commands:
```

## Comparing `ddir-3.0.1.dist-info/RECORD` & `ddir-3.1.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ddir/__init__.py,sha256=hhcbMVrBNnaITOn7qp9LtkF6cXaZcwIxGh9ew2IKgsA,4924
 ddir/__main__.py,sha256=oV1gLrsOBY4j91BquC-W3m6CDSTJ-dXpICrZrjKQMgk,4445
-ddir/__version__.py,sha256=tv1LPDhz-wNdekE0-9jM7Tt3Ymjhv0Wrw8dXwEy2kmM,156
-ddir/diff.py,sha256=LlMSDzGMbZQUCgv5f7Wc1eFkDXyj7RSQDqqZsHtFMKI,12161
+ddir/__version__.py,sha256=GsbCdKMqLSXfuahJcWyput_5Q6SPPkZr_1QpPqc8O7I,156
+ddir/diff.py,sha256=slS6qn1k5wJO0yrMlZdoKvzz-S_6E-qPdmc79fA8K54,11931
 ddir/initialize.py,sha256=XbgoD4YBxEsLfP5zabvuGIcOd2hAzHAYuBaPgeCY260,673
 ddir/legacy.py,sha256=shoCl9H9ZEO7Z_hh6urAyrUWzWnfgpygJsE7NIiBfGo,2600
 ddir/target.py,sha256=DK4riv1VBpjkomsulZeoc6JjPPcVL4Gp731y_ey9Oqo,5828
-ddir-3.0.1.dist-info/LICENSE,sha256=1dg3ZNX6FUSHfzQSyWE3rLl3_gqt-AELy1RrujtcFtY,191
-ddir-3.0.1.dist-info/METADATA,sha256=mp26Y1QT4esqr88gqiy9sQLAu3Yry4i0w-LJXfpqQnM,3933
-ddir-3.0.1.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-ddir-3.0.1.dist-info/entry_points.txt,sha256=uEQJqxm8H6cL_TYsi1-Vd7vdRnesOSVPbnr4noyXnwE,44
-ddir-3.0.1.dist-info/top_level.txt,sha256=F7NGOmHjOI4UseDtkAR3bTsbwIxLi4Gy8KaMMpIl6Ws,5
-ddir-3.0.1.dist-info/RECORD,,
+ddir-3.1.0.dist-info/LICENSE,sha256=fhLl30uuEsshWBuhV87SDhmGoFCN0Q0Oikq5pM-U6Fw,1211
+ddir-3.1.0.dist-info/METADATA,sha256=yxYPMsUTPxYEtznFCPCyxk8a37l-s2zkQjISQEFXL3A,3622
+ddir-3.1.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+ddir-3.1.0.dist-info/entry_points.txt,sha256=uEQJqxm8H6cL_TYsi1-Vd7vdRnesOSVPbnr4noyXnwE,44
+ddir-3.1.0.dist-info/top_level.txt,sha256=F7NGOmHjOI4UseDtkAR3bTsbwIxLi4Gy8KaMMpIl6Ws,5
+ddir-3.1.0.dist-info/RECORD,,
```

