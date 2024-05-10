# Comparing `tmp/pennylane-kq-0.0.7.tar.gz` & `tmp/pennylane-kq-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pennylane-kq-0.0.7.tar", last modified: Wed May  8 01:00:03 2024, max compression
+gzip compressed data, was "pennylane-kq-0.0.8.tar", last modified: Fri May 10 02:19:02 2024, max compression
```

## Comparing `pennylane-kq-0.0.7.tar` & `pennylane-kq-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 ino        (501) staff       (20)        0 2024-05-08 01:00:03.172272 pennylane-kq-0.0.7/
--rw-r--r--   0 ino        (501) staff       (20)     1335 2023-08-22 08:26:43.000000 pennylane-kq-0.0.7/LICENSE
--rw-r--r--   0 ino        (501) staff       (20)     1636 2024-05-08 01:00:03.172151 pennylane-kq-0.0.7/PKG-INFO
--rw-r--r--   0 ino        (501) staff       (20)     1304 2023-12-21 01:57:51.000000 pennylane-kq-0.0.7/README.md
-drwxr-xr-x   0 ino        (501) staff       (20)        0 2024-05-08 01:00:03.170864 pennylane-kq-0.0.7/pennylane_kq/
--rw-r--r--   0 ino        (501) staff       (20)      293 2023-12-21 00:35:30.000000 pennylane-kq-0.0.7/pennylane_kq/__init__.py
--rw-r--r--   0 ino        (501) staff       (20)       97 2024-05-08 00:52:08.000000 pennylane-kq-0.0.7/pennylane_kq/_version.py
--rw-r--r--   0 ino        (501) staff       (20)     4621 2024-05-07 08:59:35.000000 pennylane-kq-0.0.7/pennylane_kq/kq_emulator.py
--rw-r--r--   0 ino        (501) staff       (20)     3479 2023-12-27 04:57:04.000000 pennylane-kq-0.0.7/pennylane_kq/kq_emulator_aws.py
--rw-r--r--   0 ino        (501) staff       (20)     3451 2023-12-27 04:56:48.000000 pennylane-kq-0.0.7/pennylane_kq/kq_hardware.py
--rw-r--r--   0 ino        (501) staff       (20)     3541 2024-05-07 08:44:16.000000 pennylane-kq-0.0.7/pennylane_kq/kq_local_emulator.py
-drwxr-xr-x   0 ino        (501) staff       (20)        0 2024-05-08 01:00:03.171984 pennylane-kq-0.0.7/pennylane_kq.egg-info/
--rw-r--r--   0 ino        (501) staff       (20)     1636 2024-05-08 01:00:03.000000 pennylane-kq-0.0.7/pennylane_kq.egg-info/PKG-INFO
--rw-r--r--   0 ino        (501) staff       (20)      451 2024-05-08 01:00:03.000000 pennylane-kq-0.0.7/pennylane_kq.egg-info/SOURCES.txt
--rw-r--r--   0 ino        (501) staff       (20)        1 2024-05-08 01:00:03.000000 pennylane-kq-0.0.7/pennylane_kq.egg-info/dependency_links.txt
--rw-r--r--   0 ino        (501) staff       (20)      231 2024-05-08 01:00:03.000000 pennylane-kq-0.0.7/pennylane_kq.egg-info/entry_points.txt
--rw-r--r--   0 ino        (501) staff       (20)        1 2023-11-13 13:51:28.000000 pennylane-kq-0.0.7/pennylane_kq.egg-info/not-zip-safe
--rw-r--r--   0 ino        (501) staff       (20)       22 2024-05-08 01:00:03.000000 pennylane-kq-0.0.7/pennylane_kq.egg-info/requires.txt
--rw-r--r--   0 ino        (501) staff       (20)       13 2024-05-08 01:00:03.000000 pennylane-kq-0.0.7/pennylane_kq.egg-info/top_level.txt
--rw-r--r--   0 ino        (501) staff       (20)       38 2024-05-08 01:00:03.172317 pennylane-kq-0.0.7/setup.cfg
--rw-r--r--   0 ino        (501) staff       (20)     1113 2023-12-21 01:55:43.000000 pennylane-kq-0.0.7/setup.py
+drwxr-xr-x   0 ino        (501) staff       (20)        0 2024-05-10 02:19:02.487699 pennylane-kq-0.0.8/
+-rw-r--r--   0 ino        (501) staff       (20)     1335 2023-08-22 08:26:43.000000 pennylane-kq-0.0.8/LICENSE
+-rw-r--r--   0 ino        (501) staff       (20)     1886 2024-05-10 02:19:02.487583 pennylane-kq-0.0.8/PKG-INFO
+-rw-r--r--   0 ino        (501) staff       (20)     1554 2024-05-08 01:07:56.000000 pennylane-kq-0.0.8/README.md
+drwxr-xr-x   0 ino        (501) staff       (20)        0 2024-05-10 02:19:02.486222 pennylane-kq-0.0.8/pennylane_kq/
+-rw-r--r--   0 ino        (501) staff       (20)      293 2023-12-21 00:35:30.000000 pennylane-kq-0.0.8/pennylane_kq/__init__.py
+-rw-r--r--   0 ino        (501) staff       (20)       97 2024-05-10 02:18:46.000000 pennylane-kq-0.0.8/pennylane_kq/_version.py
+-rw-r--r--   0 ino        (501) staff       (20)     4621 2024-05-07 08:59:35.000000 pennylane-kq-0.0.8/pennylane_kq/kq_emulator.py
+-rw-r--r--   0 ino        (501) staff       (20)     3479 2023-12-27 04:57:04.000000 pennylane-kq-0.0.8/pennylane_kq/kq_emulator_aws.py
+-rw-r--r--   0 ino        (501) staff       (20)     3451 2023-12-27 04:56:48.000000 pennylane-kq-0.0.8/pennylane_kq/kq_hardware.py
+-rw-r--r--   0 ino        (501) staff       (20)     3541 2024-05-07 08:44:16.000000 pennylane-kq-0.0.8/pennylane_kq/kq_local_emulator.py
+-rw-r--r--   0 ino        (501) staff       (20)     3560 2024-05-10 02:16:32.000000 pennylane-kq-0.0.8/pennylane_kq/kq_remote_emulator.py
+drwxr-xr-x   0 ino        (501) staff       (20)        0 2024-05-10 02:19:02.487412 pennylane-kq-0.0.8/pennylane_kq.egg-info/
+-rw-r--r--   0 ino        (501) staff       (20)     1886 2024-05-10 02:19:02.000000 pennylane-kq-0.0.8/pennylane_kq.egg-info/PKG-INFO
+-rw-r--r--   0 ino        (501) staff       (20)      486 2024-05-10 02:19:02.000000 pennylane-kq-0.0.8/pennylane_kq.egg-info/SOURCES.txt
+-rw-r--r--   0 ino        (501) staff       (20)        1 2024-05-10 02:19:02.000000 pennylane-kq-0.0.8/pennylane_kq.egg-info/dependency_links.txt
+-rw-r--r--   0 ino        (501) staff       (20)      231 2024-05-10 02:19:02.000000 pennylane-kq-0.0.8/pennylane_kq.egg-info/entry_points.txt
+-rw-r--r--   0 ino        (501) staff       (20)        1 2023-11-13 13:51:28.000000 pennylane-kq-0.0.8/pennylane_kq.egg-info/not-zip-safe
+-rw-r--r--   0 ino        (501) staff       (20)       22 2024-05-10 02:19:02.000000 pennylane-kq-0.0.8/pennylane_kq.egg-info/requires.txt
+-rw-r--r--   0 ino        (501) staff       (20)       13 2024-05-10 02:19:02.000000 pennylane-kq-0.0.8/pennylane_kq.egg-info/top_level.txt
+-rw-r--r--   0 ino        (501) staff       (20)       38 2024-05-10 02:19:02.487740 pennylane-kq-0.0.8/setup.cfg
+-rw-r--r--   0 ino        (501) staff       (20)     1113 2023-12-21 01:55:43.000000 pennylane-kq-0.0.8/setup.py
```

### Comparing `pennylane-kq-0.0.7/LICENSE` & `pennylane-kq-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pennylane-kq-0.0.7/PKG-INFO` & `pennylane-kq-0.0.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pennylane-kq
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Pennylane plugin for KQ Cloud System
 Home-page: https://www.github.com/inojeon/pennylane-kq
 Author: Inho Jeon
 Author-email: inojeon@kisti.re.kr
 License: BSD-2
 Platform: UNKNOWN
 Provides: pennylane_kq
@@ -44,8 +44,27 @@
 -[**Source Code:**](https://github.com/inojeon/pennylane-kq)
 
 -[**Issue Tracker:**](https://github.com/inojeon/pennylane-kq/issues)
 
 If you are having issues, please let us know by posting the issue on our Github issue tracker, or
 by asking a question in the forum.
 
+## pypi 업데이트 방법
+
+\_version.py 에서 버전 변경,
+
+```
+python setup.py sdist bdist_wheel
+python -m twine upload  --skip-existing  dist/*
+```
+
+```
+python setup.py sdist bdist_wheel
+```
+
+에러시 wheel 설치
+
+```
+pip install wheel
+```
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pennylane-kq-0.0.7/pennylane_kq/kq_emulator.py` & `pennylane-kq-0.0.8/pennylane_kq/kq_emulator.py`

 * *Files identical despite different names*

### Comparing `pennylane-kq-0.0.7/pennylane_kq/kq_emulator_aws.py` & `pennylane-kq-0.0.8/pennylane_kq/kq_emulator_aws.py`

 * *Files identical despite different names*

### Comparing `pennylane-kq-0.0.7/pennylane_kq/kq_hardware.py` & `pennylane-kq-0.0.8/pennylane_kq/kq_hardware.py`

 * *Files identical despite different names*

### Comparing `pennylane-kq-0.0.7/pennylane_kq/kq_local_emulator.py` & `pennylane-kq-0.0.8/pennylane_kq/kq_local_emulator.py`

 * *Files identical despite different names*

### Comparing `pennylane-kq-0.0.7/pennylane_kq.egg-info/PKG-INFO` & `pennylane-kq-0.0.8/pennylane_kq.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pennylane-kq
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Pennylane plugin for KQ Cloud System
 Home-page: https://www.github.com/inojeon/pennylane-kq
 Author: Inho Jeon
 Author-email: inojeon@kisti.re.kr
 License: BSD-2
 Platform: UNKNOWN
 Provides: pennylane_kq
@@ -44,8 +44,27 @@
 -[**Source Code:**](https://github.com/inojeon/pennylane-kq)
 
 -[**Issue Tracker:**](https://github.com/inojeon/pennylane-kq/issues)
 
 If you are having issues, please let us know by posting the issue on our Github issue tracker, or
 by asking a question in the forum.
 
+## pypi 업데이트 방법
+
+\_version.py 에서 버전 변경,
+
+```
+python setup.py sdist bdist_wheel
+python -m twine upload  --skip-existing  dist/*
+```
+
+```
+python setup.py sdist bdist_wheel
+```
+
+에러시 wheel 설치
+
+```
+pip install wheel
+```
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pennylane-kq-0.0.7/setup.py` & `pennylane-kq-0.0.8/setup.py`

 * *Files identical despite different names*

