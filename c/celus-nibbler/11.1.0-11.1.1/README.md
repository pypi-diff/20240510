# Comparing `tmp/celus_nibbler-11.1.0.tar.gz` & `tmp/celus_nibbler-11.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celus_nibbler-11.1.0.tar", max compression
+gzip compressed data, was "celus_nibbler-11.1.1.tar", max compression
```

## Comparing `celus_nibbler-11.1.0.tar` & `celus_nibbler-11.1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1057 2022-06-17 07:35:22.867507 celus_nibbler-11.1.0/LICENSE
--rw-r--r--   0        0        0      644 2024-03-13 08:47:12.478670 celus_nibbler-11.1.0/celus_nibbler/__init__.py
--rw-r--r--   0        0        0     8253 2024-03-25 08:56:47.282003 celus_nibbler-11.1.0/celus_nibbler/__main__.py
--rw-r--r--   0        0        0     5480 2023-11-22 12:21:31.240892 celus_nibbler-11.1.0/celus_nibbler/aggregator.py
--rw-r--r--   0        0        0     6946 2024-03-13 08:47:12.478670 celus_nibbler-11.1.0/celus_nibbler/conditions.py
--rw-r--r--   0        0        0     6096 2024-03-13 08:47:12.478670 celus_nibbler-11.1.0/celus_nibbler/coordinates.py
--rw-r--r--   0        0        0    14359 2024-03-13 08:47:12.478670 celus_nibbler-11.1.0/celus_nibbler/data_headers.py
--rw-r--r--   0        0        0     2117 2024-03-25 08:56:47.282003 celus_nibbler-11.1.0/celus_nibbler/definitions/__init__.py
--rw-r--r--   0        0        0     1717 2024-03-13 08:47:12.478670 celus_nibbler-11.1.0/celus_nibbler/definitions/base.py
--rw-r--r--   0        0        0     4238 2023-10-27 12:46:00.516284 celus_nibbler-11.1.0/celus_nibbler/definitions/celus_format.py
--rw-r--r--   0        0        0    15825 2024-03-25 08:56:47.282003 celus_nibbler-11.1.0/celus_nibbler/definitions/counter.py
--rw-r--r--   0        0        0     4561 2023-10-27 12:46:00.520284 celus_nibbler-11.1.0/celus_nibbler/definitions/date_based.py
--rw-r--r--   0        0        0     4472 2023-10-27 12:46:00.520284 celus_nibbler-11.1.0/celus_nibbler/definitions/date_metric_based.py
--rw-r--r--   0        0        0     4726 2023-10-27 12:46:00.520284 celus_nibbler-11.1.0/celus_nibbler/definitions/generic.py
--rw-r--r--   0        0        0     4381 2023-10-27 12:46:00.520284 celus_nibbler-11.1.0/celus_nibbler/definitions/metric_based.py
--rw-r--r--   0        0        0    14563 2024-03-25 08:56:47.282003 celus_nibbler-11.1.0/celus_nibbler/eat_and_poop.py
--rw-r--r--   0        0        0     6074 2024-03-27 09:28:05.075344 celus_nibbler-11.1.0/celus_nibbler/errors.py
--rw-r--r--   0        0        0     2785 2022-11-01 15:22:27.669687 celus_nibbler-11.1.0/celus_nibbler/parsers/__init__.py
--rw-r--r--   0        0        0    15074 2024-03-25 08:56:47.282003 celus_nibbler-11.1.0/celus_nibbler/parsers/base.py
--rw-r--r--   0        0        0    13122 2024-03-25 08:56:47.282003 celus_nibbler-11.1.0/celus_nibbler/parsers/counter/__init__.py
--rw-r--r--   0        0        0    11529 2024-03-13 08:47:12.478670 celus_nibbler-11.1.0/celus_nibbler/parsers/counter/c4.py
--rw-r--r--   0        0        0    10694 2024-04-16 09:33:13.184343 celus_nibbler-11.1.0/celus_nibbler/parsers/counter/c5.py
--rw-r--r--   0        0        0     3803 2024-03-25 08:56:47.282003 celus_nibbler-11.1.0/celus_nibbler/parsers/counter/c5json.py
--rw-r--r--   0        0        0      156 2023-08-15 12:26:51.461995 celus_nibbler-11.1.0/celus_nibbler/parsers/dynamic.py
--rw-r--r--   0        0        0        0 2022-10-21 20:55:53.099727 celus_nibbler-11.1.0/celus_nibbler/parsers/non_counter/__init__.py
--rw-r--r--   0        0        0      194 2022-11-04 15:01:01.540828 celus_nibbler-11.1.0/celus_nibbler/parsers/non_counter/base.py
--rw-r--r--   0        0        0     5683 2023-07-29 08:57:05.293613 celus_nibbler-11.1.0/celus_nibbler/parsers/non_counter/celus_format.py
--rw-r--r--   0        0        0      322 2023-07-19 09:21:05.347414 celus_nibbler-11.1.0/celus_nibbler/parsers/non_counter/date_based.py
--rw-r--r--   0        0        0     2547 2023-07-19 09:21:05.347414 celus_nibbler-11.1.0/celus_nibbler/parsers/non_counter/date_metric_based.py
--rw-r--r--   0        0        0      774 2023-07-19 09:21:05.347414 celus_nibbler-11.1.0/celus_nibbler/parsers/non_counter/generic.py
--rw-r--r--   0        0        0     2478 2023-07-19 09:21:05.347414 celus_nibbler-11.1.0/celus_nibbler/parsers/non_counter/metric_based.py
--rw-r--r--   0        0        0    14940 2024-03-27 09:04:12.880873 celus_nibbler-11.1.0/celus_nibbler/reader.py
--rw-r--r--   0        0        0    15482 2024-03-25 08:56:47.286003 celus_nibbler-11.1.0/celus_nibbler/sources.py
--rw-r--r--   0        0        0     1624 2023-10-27 12:46:00.524284 celus_nibbler-11.1.0/celus_nibbler/utils.py
--rw-r--r--   0        0        0     9468 2024-03-13 08:47:12.482670 celus_nibbler-11.1.0/celus_nibbler/validators.py
--rw-r--r--   0        0        0     3311 2024-04-16 09:36:42.696448 celus_nibbler-11.1.0/pyproject.toml
--rw-r--r--   0        0        0     1157 1970-01-01 00:00:00.000000 celus_nibbler-11.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1057 2022-06-17 07:35:22.867507 celus_nibbler-11.1.1/LICENSE
+-rw-r--r--   0        0        0      644 2024-05-02 20:46:59.314165 celus_nibbler-11.1.1/celus_nibbler/__init__.py
+-rw-r--r--   0        0        0     8253 2024-05-02 20:46:59.318165 celus_nibbler-11.1.1/celus_nibbler/__main__.py
+-rw-r--r--   0        0        0     5480 2023-11-22 12:21:31.240892 celus_nibbler-11.1.1/celus_nibbler/aggregator.py
+-rw-r--r--   0        0        0     6946 2024-05-02 20:46:59.318165 celus_nibbler-11.1.1/celus_nibbler/conditions.py
+-rw-r--r--   0        0        0     6096 2024-05-02 20:46:59.318165 celus_nibbler-11.1.1/celus_nibbler/coordinates.py
+-rw-r--r--   0        0        0    14359 2024-05-02 20:46:59.318165 celus_nibbler-11.1.1/celus_nibbler/data_headers.py
+-rw-r--r--   0        0        0     2117 2024-05-02 20:46:59.318165 celus_nibbler-11.1.1/celus_nibbler/definitions/__init__.py
+-rw-r--r--   0        0        0     1717 2024-05-02 20:46:59.318165 celus_nibbler-11.1.1/celus_nibbler/definitions/base.py
+-rw-r--r--   0        0        0     4238 2023-10-27 12:46:00.516284 celus_nibbler-11.1.1/celus_nibbler/definitions/celus_format.py
+-rw-r--r--   0        0        0    15825 2024-05-02 20:46:59.318165 celus_nibbler-11.1.1/celus_nibbler/definitions/counter.py
+-rw-r--r--   0        0        0     4561 2023-10-27 12:46:00.520284 celus_nibbler-11.1.1/celus_nibbler/definitions/date_based.py
+-rw-r--r--   0        0        0     4472 2023-10-27 12:46:00.520284 celus_nibbler-11.1.1/celus_nibbler/definitions/date_metric_based.py
+-rw-r--r--   0        0        0     4726 2023-10-27 12:46:00.520284 celus_nibbler-11.1.1/celus_nibbler/definitions/generic.py
+-rw-r--r--   0        0        0     4381 2023-10-27 12:46:00.520284 celus_nibbler-11.1.1/celus_nibbler/definitions/metric_based.py
+-rw-r--r--   0        0        0    14563 2024-05-02 20:46:59.318165 celus_nibbler-11.1.1/celus_nibbler/eat_and_poop.py
+-rw-r--r--   0        0        0     6074 2024-05-02 20:46:59.318165 celus_nibbler-11.1.1/celus_nibbler/errors.py
+-rw-r--r--   0        0        0     2785 2022-11-01 15:22:27.669687 celus_nibbler-11.1.1/celus_nibbler/parsers/__init__.py
+-rw-r--r--   0        0        0    15190 2024-05-02 20:46:59.318165 celus_nibbler-11.1.1/celus_nibbler/parsers/base.py
+-rw-r--r--   0        0        0    13122 2024-05-02 20:46:59.318165 celus_nibbler-11.1.1/celus_nibbler/parsers/counter/__init__.py
+-rw-r--r--   0        0        0    11529 2024-05-02 20:46:59.318165 celus_nibbler-11.1.1/celus_nibbler/parsers/counter/c4.py
+-rw-r--r--   0        0        0    10694 2024-05-02 20:46:59.318165 celus_nibbler-11.1.1/celus_nibbler/parsers/counter/c5.py
+-rw-r--r--   0        0        0     3803 2024-05-02 20:46:59.318165 celus_nibbler-11.1.1/celus_nibbler/parsers/counter/c5json.py
+-rw-r--r--   0        0        0      156 2023-08-15 12:26:51.461995 celus_nibbler-11.1.1/celus_nibbler/parsers/dynamic.py
+-rw-r--r--   0        0        0        0 2022-10-21 20:55:53.099727 celus_nibbler-11.1.1/celus_nibbler/parsers/non_counter/__init__.py
+-rw-r--r--   0        0        0      194 2022-11-04 15:01:01.540828 celus_nibbler-11.1.1/celus_nibbler/parsers/non_counter/base.py
+-rw-r--r--   0        0        0     5683 2023-07-29 08:57:05.293613 celus_nibbler-11.1.1/celus_nibbler/parsers/non_counter/celus_format.py
+-rw-r--r--   0        0        0      322 2023-07-19 09:21:05.347414 celus_nibbler-11.1.1/celus_nibbler/parsers/non_counter/date_based.py
+-rw-r--r--   0        0        0     2547 2023-07-19 09:21:05.347414 celus_nibbler-11.1.1/celus_nibbler/parsers/non_counter/date_metric_based.py
+-rw-r--r--   0        0        0      774 2023-07-19 09:21:05.347414 celus_nibbler-11.1.1/celus_nibbler/parsers/non_counter/generic.py
+-rw-r--r--   0        0        0     2478 2023-07-19 09:21:05.347414 celus_nibbler-11.1.1/celus_nibbler/parsers/non_counter/metric_based.py
+-rw-r--r--   0        0        0    14940 2024-05-02 20:46:59.322165 celus_nibbler-11.1.1/celus_nibbler/reader.py
+-rw-r--r--   0        0        0    15482 2024-05-02 20:46:59.322165 celus_nibbler-11.1.1/celus_nibbler/sources.py
+-rw-r--r--   0        0        0     1624 2023-10-27 12:46:00.524284 celus_nibbler-11.1.1/celus_nibbler/utils.py
+-rw-r--r--   0        0        0     9468 2024-05-02 20:46:59.322165 celus_nibbler-11.1.1/celus_nibbler/validators.py
+-rw-r--r--   0        0        0     3311 2024-05-02 20:47:55.618084 celus_nibbler-11.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1157 1970-01-01 00:00:00.000000 celus_nibbler-11.1.1/PKG-INFO
```

### Comparing `celus_nibbler-11.1.0/LICENSE` & `celus_nibbler-11.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.0/celus_nibbler/__init__.py` & `celus_nibbler-11.1.1/celus_nibbler/__init__.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.0/celus_nibbler/__main__.py` & `celus_nibbler-11.1.1/celus_nibbler/__main__.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.0/celus_nibbler/aggregator.py` & `celus_nibbler-11.1.1/celus_nibbler/aggregator.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.0/celus_nibbler/conditions.py` & `celus_nibbler-11.1.1/celus_nibbler/conditions.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.0/celus_nibbler/coordinates.py` & `celus_nibbler-11.1.1/celus_nibbler/coordinates.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.0/celus_nibbler/data_headers.py` & `celus_nibbler-11.1.1/celus_nibbler/data_headers.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.0/celus_nibbler/definitions/__init__.py` & `celus_nibbler-11.1.1/celus_nibbler/definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.0/celus_nibbler/definitions/base.py` & `celus_nibbler-11.1.1/celus_nibbler/definitions/base.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.0/celus_nibbler/definitions/celus_format.py` & `celus_nibbler-11.1.1/celus_nibbler/definitions/celus_format.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.0/celus_nibbler/definitions/counter.py` & `celus_nibbler-11.1.1/celus_nibbler/definitions/counter.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.0/celus_nibbler/definitions/date_based.py` & `celus_nibbler-11.1.1/celus_nibbler/definitions/date_based.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.0/celus_nibbler/definitions/date_metric_based.py` & `celus_nibbler-11.1.1/celus_nibbler/definitions/date_metric_based.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.0/celus_nibbler/definitions/generic.py` & `celus_nibbler-11.1.1/celus_nibbler/definitions/generic.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.0/celus_nibbler/definitions/metric_based.py` & `celus_nibbler-11.1.1/celus_nibbler/definitions/metric_based.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.0/celus_nibbler/eat_and_poop.py` & `celus_nibbler-11.1.1/celus_nibbler/eat_and_poop.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.0/celus_nibbler/errors.py` & `celus_nibbler-11.1.1/celus_nibbler/errors.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.0/celus_nibbler/parsers/__init__.py` & `celus_nibbler-11.1.1/celus_nibbler/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.0/celus_nibbler/parsers/base.py` & `celus_nibbler-11.1.1/celus_nibbler/parsers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -359,29 +359,33 @@
 
                 if area.date_source:
                     date = area.date_source.extract(self.sheet, idx, row_offset=row_offset)
                 else:
                     date = None
 
                 dimension_data = {}
+                skip = False
                 for k, dimension_source in dimensions_sources:
                     dimension_text = dimension_source.extract(
                         self.sheet,
                         idx,
                         validator=self.dimensions_validators.get(k),
                         row_offset=row_offset,
                     )
                     if (
                         dimension_text is not None
                         and dimension_text.lower() in dimensions_to_skip.get(k, [])
                     ):
-                        continue
-
+                        skip = True
+                        break
                     dimension_data[self.get_dimension_name(k)] = dimension_text
 
+                if skip:
+                    continue
+
                 title_ids = {}
                 item_ids = {}
                 for key in IDS:
                     if title_source := title_ids_sources.get(key):
                         value = title_source.extract(self.sheet, idx, row_offset=row_offset)
                         if value:
                             title_ids[title_source.last_key] = value
```

### Comparing `celus_nibbler-11.1.0/celus_nibbler/parsers/counter/__init__.py` & `celus_nibbler-11.1.1/celus_nibbler/parsers/counter/__init__.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.0/celus_nibbler/parsers/counter/c4.py` & `celus_nibbler-11.1.1/celus_nibbler/parsers/counter/c4.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.0/celus_nibbler/parsers/counter/c5.py` & `celus_nibbler-11.1.1/celus_nibbler/parsers/counter/c5.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.0/celus_nibbler/parsers/counter/c5json.py` & `celus_nibbler-11.1.1/celus_nibbler/parsers/counter/c5json.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.0/celus_nibbler/parsers/non_counter/celus_format.py` & `celus_nibbler-11.1.1/celus_nibbler/parsers/non_counter/celus_format.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.0/celus_nibbler/parsers/non_counter/date_metric_based.py` & `celus_nibbler-11.1.1/celus_nibbler/parsers/non_counter/date_metric_based.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.0/celus_nibbler/parsers/non_counter/generic.py` & `celus_nibbler-11.1.1/celus_nibbler/parsers/non_counter/generic.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.0/celus_nibbler/parsers/non_counter/metric_based.py` & `celus_nibbler-11.1.1/celus_nibbler/parsers/non_counter/metric_based.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.0/celus_nibbler/reader.py` & `celus_nibbler-11.1.1/celus_nibbler/reader.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.0/celus_nibbler/sources.py` & `celus_nibbler-11.1.1/celus_nibbler/sources.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.0/celus_nibbler/utils.py` & `celus_nibbler-11.1.1/celus_nibbler/utils.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.0/celus_nibbler/validators.py` & `celus_nibbler-11.1.1/celus_nibbler/validators.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.1.0/pyproject.toml` & `celus_nibbler-11.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 plugins = "pydantic.mypy"
 
 [tool.pytest.ini_options]
 testpaths = "tests/"
 
 [tool.poetry]
 name = "celus-nibbler"
-version = "11.1.0"
+version = "11.1.1"
 description = "Counter-like data reader and processor."
 authors = ["Stepan Henek <stepan@bigdigdata.com>", "Zbynek Vyhlas <zbyneksmail@gmail.com>"]
 license = "MIT"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"Topic :: Software Development :: Libraries"
 ]
```

### Comparing `celus_nibbler-11.1.0/PKG-INFO` & `celus_nibbler-11.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celus-nibbler
-Version: 11.1.0
+Version: 11.1.1
 Summary: Counter-like data reader and processor.
 License: MIT
 Keywords: parsing,counter5
 Author: Stepan Henek
 Author-email: stepan@bigdigdata.com
 Requires-Python: >=3.8.9,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

