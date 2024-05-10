# Comparing `tmp/cheatsheetify-0.1.0.tar.gz` & `tmp/cheatsheetify-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cheatsheetify-0.1.0.tar", max compression
+gzip compressed data, was "cheatsheetify-0.1.1.tar", max compression
```

## Comparing `cheatsheetify-0.1.0.tar` & `cheatsheetify-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       15 2024-05-02 09:14:08.023326 cheatsheetify-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-02 09:02:17.637619 cheatsheetify-0.1.0/cheatsheetify/__init__.py
--rw-r--r--   0        0        0       83 2024-05-08 10:44:48.663364 cheatsheetify-0.1.0/cheatsheetify/__main__.py
--rw-r--r--   0        0        0     1382 2024-05-09 13:07:03.402214 cheatsheetify-0.1.0/cheatsheetify/cheatsheet_generator.py
--rw-r--r--   0        0        0     3216 2024-05-09 14:59:36.652214 cheatsheetify-0.1.0/cheatsheetify/core.py
--rwxr-xr-x   0        0        0   289624 2024-05-08 14:22:58.360499 cheatsheetify-0.1.0/cheatsheetify/fonts/FiraCode.ttf
--rw-r--r--   0        0        0   412848 2024-05-08 14:23:04.261882 cheatsheetify-0.1.0/cheatsheetify/fonts/Inter-Italic.ttf
--rw-r--r--   0        0        0       81 2024-05-08 14:23:04.261882 cheatsheetify-0.1.0/cheatsheetify/fonts/Inter-Italic.ttf:Zone.Identifier
--rwxr-xr-x   0        0        0   407056 2024-05-08 14:23:03.836019 cheatsheetify-0.1.0/cheatsheetify/fonts/Inter.ttf
--rw-r--r--   0        0        0     1643 2024-05-09 14:52:53.392213 cheatsheetify-0.1.0/cheatsheetify/pdf_generator.py
--rw-r--r--   0        0        0     1081 2024-05-09 14:27:13.402214 cheatsheetify-0.1.0/cheatsheetify/themes.py
--rw-r--r--   0        0        0      388 2024-05-09 12:01:44.362213 cheatsheetify-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      681 1970-01-01 00:00:00.000000 cheatsheetify-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       15 2024-05-09 16:25:24.740499 cheatsheetify-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 16:25:24.740499 cheatsheetify-0.1.1/cheatsheetify/__init__.py
+-rw-r--r--   0        0        0       83 2024-05-09 16:25:24.740499 cheatsheetify-0.1.1/cheatsheetify/__main__.py
+-rw-r--r--   0        0        0     1382 2024-05-09 16:25:24.740499 cheatsheetify-0.1.1/cheatsheetify/cheatsheet_generator.py
+-rw-r--r--   0        0        0     3216 2024-05-09 16:25:24.740499 cheatsheetify-0.1.1/cheatsheetify/core.py
+-rwxr-xr-x   0        0        0   289624 2024-05-09 16:25:24.744499 cheatsheetify-0.1.1/cheatsheetify/fonts/FiraCode.ttf
+-rw-r--r--   0        0        0   412848 2024-05-09 16:25:24.748499 cheatsheetify-0.1.1/cheatsheetify/fonts/Inter-Italic.ttf
+-rw-r--r--   0        0        0       81 2024-05-09 16:25:24.748499 cheatsheetify-0.1.1/cheatsheetify/fonts/Inter-Italic.ttf:Zone.Identifier
+-rwxr-xr-x   0        0        0   407056 2024-05-09 16:25:24.748499 cheatsheetify-0.1.1/cheatsheetify/fonts/Inter.ttf
+-rw-r--r--   0        0        0     1643 2024-05-09 16:25:24.748499 cheatsheetify-0.1.1/cheatsheetify/pdf_generator.py
+-rw-r--r--   0        0        0     1081 2024-05-09 16:25:24.748499 cheatsheetify-0.1.1/cheatsheetify/themes.py
+-rw-r--r--   0        0        0      388 2024-05-09 16:25:24.748499 cheatsheetify-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      681 1970-01-01 00:00:00.000000 cheatsheetify-0.1.1/PKG-INFO
```

### Comparing `cheatsheetify-0.1.0/cheatsheetify/cheatsheet_generator.py` & `cheatsheetify-0.1.1/cheatsheetify/cheatsheet_generator.py`

 * *Files identical despite different names*

### Comparing `cheatsheetify-0.1.0/cheatsheetify/core.py` & `cheatsheetify-0.1.1/cheatsheetify/core.py`

 * *Files identical despite different names*

### Comparing `cheatsheetify-0.1.0/cheatsheetify/fonts/FiraCode.ttf` & `cheatsheetify-0.1.1/cheatsheetify/fonts/FiraCode.ttf`

 * *Files identical despite different names*

### Comparing `cheatsheetify-0.1.0/cheatsheetify/fonts/Inter-Italic.ttf` & `cheatsheetify-0.1.1/cheatsheetify/fonts/Inter-Italic.ttf`

 * *Files identical despite different names*

### Comparing `cheatsheetify-0.1.0/cheatsheetify/fonts/Inter.ttf` & `cheatsheetify-0.1.1/cheatsheetify/fonts/Inter.ttf`

 * *Files identical despite different names*

### Comparing `cheatsheetify-0.1.0/cheatsheetify/pdf_generator.py` & `cheatsheetify-0.1.1/cheatsheetify/pdf_generator.py`

 * *Files identical despite different names*

### Comparing `cheatsheetify-0.1.0/cheatsheetify/themes.py` & `cheatsheetify-0.1.1/cheatsheetify/themes.py`

 * *Files identical despite different names*

### Comparing `cheatsheetify-0.1.0/PKG-INFO` & `cheatsheetify-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cheatsheetify
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 License: MIT
 Author: HYP3R00T
 Author-email: hyperoot.tech@proton.me
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

