# Comparing `tmp/celus_nigiri-2.1.0.tar.gz` & `tmp/celus_nigiri-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celus_nigiri-2.1.0.tar", max compression
+gzip compressed data, was "celus_nigiri-2.2.0.tar", max compression
```

## Comparing `celus_nigiri-2.1.0.tar` & `celus_nigiri-2.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1052 2022-07-22 09:08:04.346975 celus_nigiri-2.1.0/LICENSE
--rw-r--r--   0        0        0       63 2024-03-18 16:37:21.128669 celus_nigiri-2.1.0/celus_nigiri/__init__.py
--rw-r--r--   0        0        0     3154 2024-03-18 16:37:21.120669 celus_nigiri-2.1.0/celus_nigiri/celus.py
--rw-r--r--   0        0        0    18417 2024-04-15 14:43:20.507022 celus_nigiri-2.1.0/celus_nigiri/client.py
--rw-r--r--   0        0        0     3808 2024-03-18 16:37:21.124669 celus_nigiri-2.1.0/celus_nigiri/counter4.py
--rw-r--r--   0        0        0    20034 2024-04-16 09:00:37.721970 celus_nigiri-2.1.0/celus_nigiri/counter5.py
--rw-r--r--   0        0        0     2716 2024-03-18 16:37:21.124669 celus_nigiri-2.1.0/celus_nigiri/csv_detect/__init__.py
--rw-r--r--   0        0        0      734 2022-12-15 15:30:38.889754 celus_nigiri-2.1.0/celus_nigiri/csv_detect/__main__.py
--rw-r--r--   0        0        0        0 2024-03-18 14:21:20.036714 celus_nigiri-2.1.0/celus_nigiri/download/__init__.py
--rw-r--r--   0        0        0     2249 2024-03-18 14:21:20.040714 celus_nigiri-2.1.0/celus_nigiri/download/__main__.py
--rw-r--r--   0        0        0     3926 2022-07-12 14:45:27.530086 celus_nigiri-2.1.0/celus_nigiri/error_codes.py
--rw-r--r--   0        0        0      212 2024-03-18 16:37:21.124669 celus_nigiri-2.1.0/celus_nigiri/exceptions.py
--rw-r--r--   0        0        0     2143 2024-03-18 16:39:33.444805 celus_nigiri-2.1.0/celus_nigiri/record.py
--rw-r--r--   0        0        0     1614 2024-03-18 16:37:21.128669 celus_nigiri-2.1.0/celus_nigiri/utils.py
--rw-r--r--   0        0        0     1291 2024-04-16 09:03:32.150312 celus_nigiri-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      833 1970-01-01 00:00:00.000000 celus_nigiri-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1052 2022-07-22 09:08:04.346975 celus_nigiri-2.2.0/LICENSE
+-rw-r--r--   0        0        0       63 2024-03-18 16:37:21.128669 celus_nigiri-2.2.0/celus_nigiri/__init__.py
+-rw-r--r--   0        0        0     3154 2024-03-18 16:37:21.120669 celus_nigiri-2.2.0/celus_nigiri/celus.py
+-rw-r--r--   0        0        0    18417 2024-04-15 14:43:20.507022 celus_nigiri-2.2.0/celus_nigiri/client.py
+-rw-r--r--   0        0        0     3808 2024-03-18 16:37:21.124669 celus_nigiri-2.2.0/celus_nigiri/counter4.py
+-rw-r--r--   0        0        0    20093 2024-05-10 11:41:26.215662 celus_nigiri-2.2.0/celus_nigiri/counter5.py
+-rw-r--r--   0        0        0     2716 2024-03-18 16:37:21.124669 celus_nigiri-2.2.0/celus_nigiri/csv_detect/__init__.py
+-rw-r--r--   0        0        0      734 2022-12-15 15:30:38.889754 celus_nigiri-2.2.0/celus_nigiri/csv_detect/__main__.py
+-rw-r--r--   0        0        0        0 2024-03-18 14:21:20.036714 celus_nigiri-2.2.0/celus_nigiri/download/__init__.py
+-rw-r--r--   0        0        0     2249 2024-03-18 14:21:20.040714 celus_nigiri-2.2.0/celus_nigiri/download/__main__.py
+-rw-r--r--   0        0        0     3926 2022-07-12 14:45:27.530086 celus_nigiri-2.2.0/celus_nigiri/error_codes.py
+-rw-r--r--   0        0        0      212 2024-03-18 16:37:21.124669 celus_nigiri-2.2.0/celus_nigiri/exceptions.py
+-rw-r--r--   0        0        0     2143 2024-03-18 16:39:33.444805 celus_nigiri-2.2.0/celus_nigiri/record.py
+-rw-r--r--   0        0        0     1614 2024-03-18 16:37:21.128669 celus_nigiri-2.2.0/celus_nigiri/utils.py
+-rw-r--r--   0        0        0     1291 2024-05-10 11:40:45.299457 celus_nigiri-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0      833 1970-01-01 00:00:00.000000 celus_nigiri-2.2.0/PKG-INFO
```

### Comparing `celus_nigiri-2.1.0/LICENSE` & `celus_nigiri-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `celus_nigiri-2.1.0/celus_nigiri/celus.py` & `celus_nigiri-2.2.0/celus_nigiri/celus.py`

 * *Files identical despite different names*

### Comparing `celus_nigiri-2.1.0/celus_nigiri/client.py` & `celus_nigiri-2.2.0/celus_nigiri/client.py`

 * *Files identical despite different names*

### Comparing `celus_nigiri-2.1.0/celus_nigiri/counter4.py` & `celus_nigiri-2.2.0/celus_nigiri/counter4.py`

 * *Files identical despite different names*

### Comparing `celus_nigiri-2.1.0/celus_nigiri/counter5.py` & `celus_nigiri-2.2.0/celus_nigiri/counter5.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Module dealing with data in the COUNTER5 format.
 """
 
 import csv
 import json
 import typing
+from copy import deepcopy
 from datetime import date
 
 import ijson.backends.yajl2_c as ijson
 
 from .celus import get_months as celus_format_get_months
 from .csv_detect import detect_csv_dialect, detect_file_encoding
 from .error_codes import ErrorCode, error_code_to_severity
@@ -252,14 +253,15 @@
         if header:
             # Try to extract exceptions from header
             self.extract_errors(header)
             if not any((self.errors, self.warnings, self.infos)):
                 # no  error/warning/info = > file has to contain a valid header
                 self.check_header(header, fd)
                 fd.seek(0)
+            self.header = deepcopy(header)
         elif not self.record_found:
             # Header is missing and no data
             raise SushiException("Incorrect format", content=fd.read())
         else:
             # Header is empty, but data are present
             pass
 
@@ -307,16 +309,16 @@
         if date_start and date_end:
             return get_date_range(date_start, date_end)
         else:
             return []
 
     def file_to_records(self, filename: str) -> typing.Generator[CounterRecord, None, None]:
         f = open(filename, "rb")  # file will be closed later (once generator struct is discarded)
-        self.header, items = self.fd_to_dicts(f)
-        return self.read_report(self.header, items)
+        header, items = self.fd_to_dicts(f)
+        return self.read_report(header, items)
 
     @classmethod
     def file_to_input(cls, filename: str):
         with open(filename, "r", encoding="utf-8") as infile:
             return json.load(infile)
 
     @classmethod
```

### Comparing `celus_nigiri-2.1.0/celus_nigiri/csv_detect/__init__.py` & `celus_nigiri-2.2.0/celus_nigiri/csv_detect/__init__.py`

 * *Files identical despite different names*

### Comparing `celus_nigiri-2.1.0/celus_nigiri/csv_detect/__main__.py` & `celus_nigiri-2.2.0/celus_nigiri/csv_detect/__main__.py`

 * *Files identical despite different names*

### Comparing `celus_nigiri-2.1.0/celus_nigiri/download/__main__.py` & `celus_nigiri-2.2.0/celus_nigiri/download/__main__.py`

 * *Files identical despite different names*

### Comparing `celus_nigiri-2.1.0/celus_nigiri/error_codes.py` & `celus_nigiri-2.2.0/celus_nigiri/error_codes.py`

 * *Files identical despite different names*

### Comparing `celus_nigiri-2.1.0/celus_nigiri/record.py` & `celus_nigiri-2.2.0/celus_nigiri/record.py`

 * *Files identical despite different names*

### Comparing `celus_nigiri-2.1.0/celus_nigiri/utils.py` & `celus_nigiri-2.2.0/celus_nigiri/utils.py`

 * *Files identical despite different names*

### Comparing `celus_nigiri-2.1.0/pyproject.toml` & `celus_nigiri-2.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 "test_*.py" = ["B011"]  # test files should have asserts
 
 [tool.pytest.ini_options]
 testpaths = "tests/"
 
 [tool.poetry]
 name = "celus-nigiri"
-version = "2.1.0"
+version = "2.2.0"
 description = "Library for downloading and parsing counter-like data."
 authors = ["Beda Kosata <beda@bigdigdata.com>", "Stepan Henek <stepan@bigdigdata.com>"]
 license = "MIT"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"Topic :: Software Development :: Libraries"
 ]
```

### Comparing `celus_nigiri-2.1.0/PKG-INFO` & `celus_nigiri-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celus-nigiri
-Version: 2.1.0
+Version: 2.2.0
 Summary: Library for downloading and parsing counter-like data.
 License: MIT
 Author: Beda Kosata
 Author-email: beda@bigdigdata.com
 Requires-Python: >=3.8.9,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

