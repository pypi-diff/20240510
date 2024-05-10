# Comparing `tmp/goshdb-0.1.0.tar.gz` & `tmp/goshdb-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goshdb-0.1.0.tar", max compression
+gzip compressed data, was "goshdb-0.2.0.tar", max compression
```

## Comparing `goshdb-0.1.0.tar` & `goshdb-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1063 2024-05-09 20:05:17.913447 goshdb-0.1.0/LICENSE
--rw-r--r--   0        0        0     2444 2024-05-09 20:10:10.506450 goshdb-0.1.0/README.md
--rw-r--r--   0        0        0      690 2024-05-09 20:10:10.512867 goshdb-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       31 2024-05-09 20:09:00.057862 goshdb-0.1.0/src/goshdb/__init__.py
--rw-r--r--   0        0        0     1901 2024-05-09 20:09:00.055620 goshdb-0.1.0/src/goshdb/integrated_test.py
--rw-r--r--   0        0        0     7068 2024-05-09 20:09:00.029869 goshdb-0.1.0/src/goshdb/sheet.py
--rw-r--r--   0        0        0     4117 2024-05-09 20:09:00.053209 goshdb-0.1.0/src/goshdb/table.py
--rw-r--r--   0        0        0     3262 1970-01-01 00:00:00.000000 goshdb-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-09 20:05:17.913447 goshdb-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4092 2024-05-09 20:57:38.631275 goshdb-0.2.0/README.md
+-rw-r--r--   0        0        0      690 2024-05-09 20:57:38.696262 goshdb-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       31 2024-05-09 20:09:00.057862 goshdb-0.2.0/src/goshdb/__init__.py
+-rw-r--r--   0        0        0     1901 2024-05-09 20:09:00.055620 goshdb-0.2.0/src/goshdb/integrated_test.py
+-rw-r--r--   0        0        0     7068 2024-05-09 20:09:00.029869 goshdb-0.2.0/src/goshdb/sheet.py
+-rw-r--r--   0        0        0     5641 2024-05-09 21:32:30.853618 goshdb-0.2.0/src/goshdb/table.py
+-rw-r--r--   0        0        0     4910 1970-01-01 00:00:00.000000 goshdb-0.2.0/PKG-INFO
```

### Comparing `goshdb-0.1.0/LICENSE` & `goshdb-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `goshdb-0.1.0/pyproject.toml` & `goshdb-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "goshdb"
-version = "0.1.0"
+version = "0.2.0"
 description = "GOogle SHeets DataBase - Python client to key-value database based on Google Sheets"
 authors = ["Artyom Vorobyov <artyom.vorobyov@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/artoby/goshdb"
 keywords = ["google", "sheets", "spreadsheet", "database", "key-value", "free", "nosql"]
 classifiers = [
```

### Comparing `goshdb-0.1.0/src/goshdb/integrated_test.py` & `goshdb-0.2.0/src/goshdb/integrated_test.py`

 * *Files identical despite different names*

### Comparing `goshdb-0.1.0/src/goshdb/sheet.py` & `goshdb-0.2.0/src/goshdb/sheet.py`

 * *Files identical despite different names*

### Comparing `goshdb-0.1.0/PKG-INFO` & `goshdb-0.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goshdb
-Version: 0.1.0
+Version: 0.2.0
 Summary: GOogle SHeets DataBase - Python client to key-value database based on Google Sheets
 Home-page: https://github.com/artoby/goshdb
 License: MIT
 Keywords: google,sheets,spreadsheet,database,key-value,free,nosql
 Author: Artyom Vorobyov
 Author-email: artyom.vorobyov@gmail.com
 Requires-Python: >=3.10,<3.11
@@ -18,22 +18,50 @@
 Requires-Dist: openpyxl (>=3.1.0)
 Project-URL: Repository, https://github.com/artoby/goshdb
 Description-Content-Type: text/markdown
 
 # goshdb
 GOogle SHeets DataBase - Python client to key-value database based on Google Sheets
 
-Sheet works as a table and has the following structure:
-```
-| key | value |
-|-----|-------|
-|     |       |
-|     |       |
-|     |       |
-```
+Sheet works as a table and has the following look & structure:
+
+<img src="https://github.com/artoby/goshdb/assets/6637041/cf3ba5d4-e1df-42ff-8487-3f18a27190fd" width="300">
+
+
+# Use cases
+- Store configuration with ability to change it on the fly
+- Store data that should be shared between multiple users / machines
+- Write status of a long-running process and observe it in real-time in Google Sheets
+- Review data modification history in Google Sheets UI (File -> Version history -> See version history)
+
+Features
+- Simple key-value interface (get/set string/object)
+
+Advantages
+- Free storage (Google Sheets API has free quota)
+- Concurrent read (Supports parallel read from multiple clients)
+- No need to create a server
+- User-friendly Google Sheets UI for data review & modification
+- No need to install any software on the client side (only Python)
+- Simple get/set methods instead of SQL queries
+- No need to create a database schema (just create a new sheet)
+- Data backup, synchronization, availability, and security are managed by Google Sheets
+
+Limitations
+- Not suitable for high-frequency read/write operations (Google Sheets API has read/write quota: 
+300/minute per project, 60/minute per user per project)
+- Not suitable for concurrent write (Google Sheets API has no locking mechanism)
+- Not suitable for very large data (Google Sheets has a limit of 10 million cells per spreadsheet, 
+i.e. 5 million key-value pairs
+- Not suitable for high-speed data access (Google Sheets API has a delay, takes ~0.3-1 second per 
+get/set operation)
+- Not suitable for complex queries, types, data structures, relations, validation and indexing 
+(only key-value interface)
+- Not suitable for sensitive & high-security data (Google Sheets API has access to all 
+spreadsheets in the account)
 
 # Installation
 ```bash
 pip install goshdb
 ```
 
 # Configuration
```

