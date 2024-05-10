# Comparing `tmp/watchmen_inquiry_trino-16.6.8.tar.gz` & `tmp/watchmen_inquiry_trino-16.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_inquiry_trino-16.6.8.tar", max compression
+gzip compressed data, was "watchmen_inquiry_trino-16.6.9.tar", max compression
```

## Comparing `watchmen_inquiry_trino-16.6.8.tar` & `watchmen_inquiry_trino-16.6.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1061 2024-01-08 07:58:02.512594 watchmen_inquiry_trino-16.6.8/LICENSE
--rw-r--r--   0        0        0      482 2024-01-08 07:58:02.512594 watchmen_inquiry_trino-16.6.8/pyproject.toml
--rw-r--r--   0        0        0      150 2024-01-08 07:58:02.512594 watchmen_inquiry_trino-16.6.8/src/watchmen_inquiry_trino/__init__.py
--rw-r--r--   0        0        0       46 2024-01-08 07:58:02.512594 watchmen_inquiry_trino-16.6.8/src/watchmen_inquiry_trino/exception.py
--rw-r--r--   0        0        0     1171 2024-01-08 07:58:02.512594 watchmen_inquiry_trino-16.6.8/src/watchmen_inquiry_trino/settings.py
--rw-r--r--   0        0        0    37618 2024-01-08 07:58:02.512594 watchmen_inquiry_trino-16.6.8/src/watchmen_inquiry_trino/trino_storage.py
--rw-r--r--   0        0        0      257 2024-01-08 07:58:02.512594 watchmen_inquiry_trino-16.6.8/src/watchmen_inquiry_trino/trino_storage_helper.py
--rw-r--r--   0        0        0     7684 2024-01-08 07:58:02.512594 watchmen_inquiry_trino-16.6.8/src/watchmen_inquiry_trino/trino_storage_spi.py
--rw-r--r--   0        0        0      586 1970-01-01 00:00:00.000000 watchmen_inquiry_trino-16.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-02-01 01:32:37.243322 watchmen_inquiry_trino-16.6.9/LICENSE
+-rw-r--r--   0        0        0      482 2024-02-01 01:32:37.243322 watchmen_inquiry_trino-16.6.9/pyproject.toml
+-rw-r--r--   0        0        0      150 2024-02-01 01:32:37.243322 watchmen_inquiry_trino-16.6.9/src/watchmen_inquiry_trino/__init__.py
+-rw-r--r--   0        0        0       46 2024-02-01 01:32:37.243322 watchmen_inquiry_trino-16.6.9/src/watchmen_inquiry_trino/exception.py
+-rw-r--r--   0        0        0     1171 2024-02-01 01:32:37.243322 watchmen_inquiry_trino-16.6.9/src/watchmen_inquiry_trino/settings.py
+-rw-r--r--   0        0        0    37618 2024-02-01 01:32:37.243322 watchmen_inquiry_trino-16.6.9/src/watchmen_inquiry_trino/trino_storage.py
+-rw-r--r--   0        0        0      257 2024-02-01 01:32:37.243322 watchmen_inquiry_trino-16.6.9/src/watchmen_inquiry_trino/trino_storage_helper.py
+-rw-r--r--   0        0        0     7684 2024-02-01 01:32:37.243322 watchmen_inquiry_trino-16.6.9/src/watchmen_inquiry_trino/trino_storage_spi.py
+-rw-r--r--   0        0        0      586 1970-01-01 00:00:00.000000 watchmen_inquiry_trino-16.6.9/PKG-INFO
```

### Comparing `watchmen_inquiry_trino-16.6.8/LICENSE` & `watchmen_inquiry_trino-16.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_trino-16.6.8/src/watchmen_inquiry_trino/settings.py` & `watchmen_inquiry_trino-16.6.9/src/watchmen_inquiry_trino/settings.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_trino-16.6.8/src/watchmen_inquiry_trino/trino_storage.py` & `watchmen_inquiry_trino-16.6.9/src/watchmen_inquiry_trino/trino_storage.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_trino-16.6.8/src/watchmen_inquiry_trino/trino_storage_spi.py` & `watchmen_inquiry_trino-16.6.9/src/watchmen_inquiry_trino/trino_storage_spi.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_trino-16.6.8/PKG-INFO` & `watchmen_inquiry_trino-16.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: watchmen-inquiry-trino
-Version: 16.6.8
+Version: 16.6.9
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: trino (>=0.312.0,<0.313.0)
-Requires-Dist: watchmen-data-kernel (==16.6.8)
+Requires-Dist: watchmen-data-kernel (==16.6.9)
```

