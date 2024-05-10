# Comparing `tmp/cancel_contexts-0.1.1.tar.gz` & `tmp/cancel_contexts-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cancel_contexts-0.1.1.tar", max compression
+gzip compressed data, was "cancel_contexts-0.1.2.tar", max compression
```

## Comparing `cancel_contexts-0.1.1.tar` & `cancel_contexts-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,9 @@
--rw-r--r--   0        0        0      674 2024-05-09 11:21:33.392148 cancel_contexts-0.1.1/README.md
--rw-r--r--   0        0        0       50 2024-05-09 11:14:37.354739 cancel_contexts-0.1.1/cancel_contexts/__init__.py
--rw-r--r--   0        0        0       72 2024-05-09 08:31:07.421755 cancel_contexts-0.1.1/cancel_contexts/contexts/__init__.py
--rw-r--r--   0        0        0      239 2024-05-09 09:08:34.770331 cancel_contexts-0.1.1/cancel_contexts/contexts/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     2871 2024-05-09 10:41:03.491070 cancel_contexts-0.1.1/cancel_contexts/contexts/__pycache__/base.cpython-312.pyc
--rw-r--r--   0        0        0      780 2024-05-09 10:41:03.490443 cancel_contexts-0.1.1/cancel_contexts/contexts/__pycache__/cancel.cpython-312.pyc
--rw-r--r--   0        0        0     1551 2024-05-09 10:56:45.669742 cancel_contexts-0.1.1/cancel_contexts/contexts/__pycache__/protocols.cpython-312.pyc
--rw-r--r--   0        0        0     1208 2024-05-09 10:41:01.568238 cancel_contexts-0.1.1/cancel_contexts/contexts/base.py
--rw-r--r--   0        0        0      278 2024-05-09 10:41:01.561153 cancel_contexts-0.1.1/cancel_contexts/contexts/cancel.py
--rw-r--r--   0        0        0      490 2024-05-09 10:56:59.535110 cancel_contexts-0.1.1/cancel_contexts/contexts/protocols.py
--rw-r--r--   0        0        0      114 2024-05-09 09:01:11.108905 cancel_contexts-0.1.1/cancel_contexts/exceptions.py
--rw-r--r--   0        0        0     1806 2024-05-09 11:29:27.392579 cancel_contexts-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1890 1970-01-01 00:00:00.000000 cancel_contexts-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      674 2024-05-09 11:21:33.392148 cancel_contexts-0.1.2/README.md
+-rw-r--r--   0        0        0       50 2024-05-09 11:14:37.354739 cancel_contexts-0.1.2/cancel_contexts/__init__.py
+-rw-r--r--   0        0        0       72 2024-05-09 08:31:07.421755 cancel_contexts-0.1.2/cancel_contexts/contexts/__init__.py
+-rw-r--r--   0        0        0     1208 2024-05-09 10:41:01.568238 cancel_contexts-0.1.2/cancel_contexts/contexts/base.py
+-rw-r--r--   0        0        0      278 2024-05-09 10:41:01.561153 cancel_contexts-0.1.2/cancel_contexts/contexts/cancel.py
+-rw-r--r--   0        0        0      490 2024-05-09 10:56:59.535110 cancel_contexts-0.1.2/cancel_contexts/contexts/protocols.py
+-rw-r--r--   0        0        0      114 2024-05-09 09:01:11.108905 cancel_contexts-0.1.2/cancel_contexts/exceptions.py
+-rw-r--r--   0        0        0     1806 2024-05-09 11:42:32.020130 cancel_contexts-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1890 1970-01-01 00:00:00.000000 cancel_contexts-0.1.2/PKG-INFO
```

### Comparing `cancel_contexts-0.1.1/README.md` & `cancel_contexts-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `cancel_contexts-0.1.1/cancel_contexts/contexts/base.py` & `cancel_contexts-0.1.2/cancel_contexts/contexts/base.py`

 * *Files identical despite different names*

### Comparing `cancel_contexts-0.1.1/pyproject.toml` & `cancel_contexts-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cancel-contexts"
-version = "0.1.1"
+version = "0.1.2"
 description = "Realisation for canceling contexts (cancelled tokens) for Python"
 authors = ["Denis Novikov <alpden550@gmail.com>"]
 readme = "README.md"
 license = 'MIT'
 classifiers = [
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
```

### Comparing `cancel_contexts-0.1.1/PKG-INFO` & `cancel_contexts-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cancel-contexts
-Version: 0.1.1
+Version: 0.1.2
 Summary: Realisation for canceling contexts (cancelled tokens) for Python
 Home-page: https://github.com/alpden550/cancel-contexts
 License: MIT
 Keywords: python,python3,cancel token,cancel context
 Author: Denis Novikov
 Author-email: alpden550@gmail.com
 Requires-Python: >=3.11,<4.0
```

