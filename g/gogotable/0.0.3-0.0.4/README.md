# Comparing `tmp/gogotable-0.0.3.tar.gz` & `tmp/gogotable-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gogotable-0.0.3.tar", max compression
+gzip compressed data, was "gogotable-0.0.4.tar", max compression
```

## Comparing `gogotable-0.0.3.tar` & `gogotable-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1211 2024-04-09 17:41:01.686245 gogotable-0.0.3/LICENSE
--rw-r--r--   0        0        0      627 2024-04-09 19:35:49.594688 gogotable-0.0.3/README.md
--rw-r--r--   0        0        0      885 2024-04-09 19:36:47.565136 gogotable-0.0.3/pyproject.toml
--rw-r--r--   0        0        0       41 2024-04-09 19:09:26.225741 gogotable-0.0.3/src/gogotable/__init__.py
--rw-r--r--   0        0        0     1454 2024-04-09 19:30:07.297188 gogotable-0.0.3/src/gogotable/gogotable.py
--rw-r--r--   0        0        0     1153 1970-01-01 00:00:00.000000 gogotable-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-27 14:32:31.956850 gogotable-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1178 2024-04-27 14:32:31.957569 gogotable-0.0.4/README.md
+-rw-r--r--   0        0        0      848 2024-05-10 08:57:08.567169 gogotable-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0       41 2024-04-27 14:32:31.961336 gogotable-0.0.4/src/gogotable/__init__.py
+-rw-r--r--   0        0        0     1269 2024-04-27 14:32:31.961753 gogotable-0.0.4/src/gogotable/gogotable.py
+-rw-r--r--   0        0        0     1704 1970-01-01 00:00:00.000000 gogotable-0.0.4/PKG-INFO
```

### Comparing `gogotable-0.0.3/LICENSE` & `gogotable-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gogotable-0.0.3/pyproject.toml` & `gogotable-0.0.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -7,34 +7,32 @@
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 
 [tool.poetry]
 name = "gogotable"
-version = "0.0.3"
+version = "0.0.4"
 description = "Convert structured data to a table"
 authors = ["Luís Miranda <luistm@gmail.com>"]
 license = "The Unlicense"
 readme = "README.md"
 packages = [{ include = "gogotable", from = "src" }]
 exclude = ["**/*_test.py"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 
 [tool.poetry.group.dev.dependencies]
 bandit = { extras = ["toml"], version = "^1.7.8" }
-behave = "^1.2.6"
-black = "^24.3.0"
-coverage = "^7.4.4"
+black = "^24.4.2"
+coverage = "^7.5.1"
 flake8 = "^7.0.0"
-ipython = "^8.18.1"
 isort = "^5.13.2"
-nox = "^2024.3.2"
+nox = "^2024.4.15"
 pre-commit = "^3.7.0"
-pytest = "^8.1.1"
-pytest-xdist = "^3.5.0"
+pytest = "^8.2.0"
+pytest-xdist = "^3.6.1"
 turbofan = "^0.2.0"
 
 [tool.pytest.ini_options]
 markers = ["integration: tags a test as integration tests"]
```

### Comparing `gogotable-0.0.3/src/gogotable/gogotable.py` & `gogotable-0.0.4/src/gogotable/gogotable.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,35 +19,31 @@
 
         # Sometimes, the header size is greater than the value
         if len(headers[i]) > column_length:
             column_length = len(headers[i])
 
         columns_length.append(column_length)
 
-    # Build the table header
-    header_line = "|"
-    for i, header in enumerate(headers):
-        header_line = header_line + f" {header:^{columns_length[i]}} |"
-
-    # Build the table border
-    border = "|"
-    for _ in range(len(header_line) - 2):  # 2 is the number of '|' characters
-        border += "-"
-    border += "|"
-
-    table.append(border)
-    table.append(header_line)
-    table.append(border)
+    header_line = (
+        "|"
+        + "|".join(
+            f" {header:^{length}} " for header, length in zip(headers, columns_length)
+        )
+        + "|"
+    )
+    border = "|" + "-".join("-" * (length + 2) for length in columns_length) + "|"
+    table.extend([border, header_line, border])
 
     # Build the table data rows
     for row in rows:
-        data_line = "|"
-        for i, _ in enumerate(headers):
-            try:
-                data_line = data_line + f" {row[i]:>{columns_length[i]}} |"
-            except IndexError:
-                data_line = data_line + f" {' ':>{columns_length[i]}} |"
+        data_line = (
+            "|"
+            + "|".join(
+                f" {data:>{length}} " for data, length in zip(row, columns_length)
+            )
+            + "|"
+        )
         table.append(data_line)
 
     table.append(border)
 
     return table
```

