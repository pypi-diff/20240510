# Comparing `tmp/gogotable-0.0.4.tar.gz` & `tmp/gogotable-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gogotable-0.0.4.tar", max compression
+gzip compressed data, was "gogotable-0.1.0.tar", max compression
```

## Comparing `gogotable-0.0.4.tar` & `gogotable-0.1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1211 2024-04-27 14:32:31.956850 gogotable-0.0.4/LICENSE
--rw-r--r--   0        0        0     1178 2024-04-27 14:32:31.957569 gogotable-0.0.4/README.md
--rw-r--r--   0        0        0      848 2024-05-10 08:57:08.567169 gogotable-0.0.4/pyproject.toml
--rw-r--r--   0        0        0       41 2024-04-27 14:32:31.961336 gogotable-0.0.4/src/gogotable/__init__.py
--rw-r--r--   0        0        0     1269 2024-04-27 14:32:31.961753 gogotable-0.0.4/src/gogotable/gogotable.py
--rw-r--r--   0        0        0     1704 1970-01-01 00:00:00.000000 gogotable-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-27 14:32:31.956850 gogotable-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1178 2024-04-27 14:32:31.957569 gogotable-0.1.0/README.md
+-rw-r--r--   0        0        0      848 2024-05-10 12:55:41.355470 gogotable-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0       41 2024-04-27 14:32:31.961336 gogotable-0.1.0/src/gogotable/__init__.py
+-rw-r--r--   0        0        0     1492 2024-05-10 12:52:39.471145 gogotable-0.1.0/src/gogotable/gogotable.py
+-rw-r--r--   0        0        0     1704 1970-01-01 00:00:00.000000 gogotable-0.1.0/PKG-INFO
```

### Comparing `gogotable-0.0.4/LICENSE` & `gogotable-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gogotable-0.0.4/README.md` & `gogotable-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `gogotable-0.0.4/pyproject.toml` & `gogotable-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 
 [tool.poetry]
 name = "gogotable"
-version = "0.0.4"
+version = "0.1.0"
 description = "Convert structured data to a table"
 authors = ["Luís Miranda <luistm@gmail.com>"]
 license = "The Unlicense"
 readme = "README.md"
 packages = [{ include = "gogotable", from = "src" }]
 exclude = ["**/*_test.py"]
```

### Comparing `gogotable-0.0.4/src/gogotable/gogotable.py` & `gogotable-0.1.0/src/gogotable/gogotable.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,22 +4,27 @@
 
     :param headers: headers of the table
     :param rows: the data of the table
     :return: a list of strings representing the table
     """
 
     table = []
+    skip_data = False
 
     # Find the size of each column
     columns_length = []
     for i, _ in enumerate(headers):
         try:
             column_length = max(len(str(row[i])) for row in rows)
         except IndexError:
             column_length = 0
+        except ValueError:
+            # There are no rows to calculate the max
+            column_length = 0
+            skip_data = True
 
         # Sometimes, the header size is greater than the value
         if len(headers[i]) > column_length:
             column_length = len(headers[i])
 
         columns_length.append(column_length)
 
@@ -29,21 +34,22 @@
             f" {header:^{length}} " for header, length in zip(headers, columns_length)
         )
         + "|"
     )
     border = "|" + "-".join("-" * (length + 2) for length in columns_length) + "|"
     table.extend([border, header_line, border])
 
-    # Build the table data rows
-    for row in rows:
-        data_line = (
-            "|"
-            + "|".join(
-                f" {data:>{length}} " for data, length in zip(row, columns_length)
+    if not skip_data:
+        # Build the table data rows
+        for row in rows:
+            data_line = (
+                "|"
+                + "|".join(
+                    f" {data:>{length}} " for data, length in zip(row, columns_length)
+                )
+                + "|"
             )
-            + "|"
-        )
-        table.append(data_line)
+            table.append(data_line)
 
     table.append(border)
 
     return table
```

### Comparing `gogotable-0.0.4/PKG-INFO` & `gogotable-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gogotable
-Version: 0.0.4
+Version: 0.1.0
 Summary: Convert structured data to a table
 License: Unlicense
 Author: Luís Miranda
 Author-email: luistm@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
```

