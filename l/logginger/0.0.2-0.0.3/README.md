# Comparing `tmp/logginger-0.0.2.tar.gz` & `tmp/logginger-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logginger-0.0.2.tar", max compression
+gzip compressed data, was "logginger-0.0.3.tar", max compression
```

## Comparing `logginger-0.0.2.tar` & `logginger-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0    11357 2024-05-10 12:51:49.562627 logginger-0.0.2/LICENSE
--rw-r--r--   0        0        0     4107 2024-05-10 12:50:15.987048 logginger-0.0.2/README.md
--rw-r--r--   0        0        0        0 2024-05-10 13:43:58.288423 logginger-0.0.2/logginger/__init__.py
--rw-r--r--   0        0        0      134 2024-05-10 16:46:05.449184 logginger-0.0.2/logginger/config.py
--rw-r--r--   0        0        0      333 2024-05-10 15:16:32.900348 logginger-0.0.2/logginger/fmts.py
--rw-r--r--   0        0        0     3289 2024-05-10 16:19:52.578314 logginger-0.0.2/logginger/formatters.py
--rw-r--r--   0        0        0        0 2024-05-10 15:21:10.974946 logginger-0.0.2/logginger/handlers/__init__.py
--rw-r--r--   0        0        0     7674 2024-05-10 16:46:05.452178 logginger-0.0.2/logginger/handlers/slack/__init__.py
--rw-r--r--   0        0        0      477 2024-05-10 12:02:14.121035 logginger-0.0.2/logginger/handlers/slack/colors.py
--rw-r--r--   0        0        0      229 2024-05-10 13:05:24.360119 logginger-0.0.2/logginger/utils.py
--rw-r--r--   0        0        0     1873 2024-05-10 15:20:31.721410 logginger-0.0.2/logginger/uvicorn/__init__.py
--rw-r--r--   0        0        0      479 2024-05-10 17:02:44.715727 logginger-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     4702 1970-01-01 00:00:00.000000 logginger-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-10 12:51:49.562627 logginger-0.0.3/LICENSE
+-rw-r--r--   0        0        0     4107 2024-05-10 12:50:15.987048 logginger-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-10 13:43:58.288423 logginger-0.0.3/logginger/__init__.py
+-rw-r--r--   0        0        0      134 2024-05-10 16:46:05.449184 logginger-0.0.3/logginger/config.py
+-rw-r--r--   0        0        0      333 2024-05-10 15:16:32.900348 logginger-0.0.3/logginger/fmts.py
+-rw-r--r--   0        0        0     3289 2024-05-10 16:19:52.578314 logginger-0.0.3/logginger/formatters.py
+-rw-r--r--   0        0        0     7674 2024-05-10 16:46:05.452178 logginger-0.0.3/logginger/slack/__init__.py
+-rw-r--r--   0        0        0      477 2024-05-10 12:02:14.121035 logginger-0.0.3/logginger/slack/colors.py
+-rw-r--r--   0        0        0      229 2024-05-10 13:05:24.360119 logginger-0.0.3/logginger/utils.py
+-rw-r--r--   0        0        0     1873 2024-05-10 15:20:31.721410 logginger-0.0.3/logginger/uvicorn/__init__.py
+-rw-r--r--   0        0        0      479 2024-05-10 17:06:00.648858 logginger-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4702 1970-01-01 00:00:00.000000 logginger-0.0.3/PKG-INFO
```

### Comparing `logginger-0.0.2/LICENSE` & `logginger-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `logginger-0.0.2/README.md` & `logginger-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `logginger-0.0.2/logginger/formatters.py` & `logginger-0.0.3/logginger/formatters.py`

 * *Files identical despite different names*

### Comparing `logginger-0.0.2/logginger/handlers/slack/__init__.py` & `logginger-0.0.3/logginger/slack/__init__.py`

 * *Files identical despite different names*

### Comparing `logginger-0.0.2/logginger/uvicorn/__init__.py` & `logginger-0.0.3/logginger/uvicorn/__init__.py`

 * *Files identical despite different names*

### Comparing `logginger-0.0.2/PKG-INFO` & `logginger-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logginger
-Version: 0.0.2
+Version: 0.0.3
 Summary: Logginger is a simple logging library that includes tools to extend the logging module.
 Author: Hikmat Samadov
 Author-email: hikmat@cublya.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

