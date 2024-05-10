# Comparing `tmp/xhlog-0.0.1.tar.gz` & `tmp/xhlog-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xhlog-0.0.1.tar", max compression
+gzip compressed data, was "xhlog-0.0.2.tar", max compression
```

## Comparing `xhlog-0.0.1.tar` & `xhlog-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1083 2024-05-10 13:12:40.547765 xhlog-0.0.1/LICENSE
--rw-r--r--   0        0        0      341 2024-05-10 13:11:53.047753 xhlog-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       61 2024-05-10 13:05:53.980355 xhlog-0.0.1/README.md
--rw-r--r--   0        0        0     1204 2024-05-10 13:18:31.854976 xhlog-0.0.1/xhlog/__init__.py
--rw-r--r--   0        0        0      806 1970-01-01 00:00:00.000000 xhlog-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-05-10 13:12:40.547765 xhlog-0.0.2/LICENSE
+-rw-r--r--   0        0        0      341 2024-05-10 15:28:06.583591 xhlog-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       60 2024-05-10 15:27:55.197927 xhlog-0.0.2/README.md
+-rw-r--r--   0        0        0     1270 2024-05-10 15:27:16.449859 xhlog-0.0.2/xhlog/__init__.py
+-rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 xhlog-0.0.2/PKG-INFO
```

### Comparing `xhlog-0.0.1/LICENSE` & `xhlog-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xhlog-0.0.1/PKG-INFO` & `xhlog-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xhlog
-Version: 0.0.1
+Version: 0.0.2
 Summary: [XhLog]一个轻量，简易的Python日志记录模块。
 Author: Yeying-Xingchen
 Author-email: yeyingxingchen@yeah.net
 Requires-Python: >=3,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
@@ -13,9 +13,9 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 
-# xh-log
+# xhlog
 一个轻量，简易的Python日志记录模块。
```

