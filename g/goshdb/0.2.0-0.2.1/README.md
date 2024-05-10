# Comparing `tmp/goshdb-0.2.0.tar.gz` & `tmp/goshdb-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goshdb-0.2.0.tar", max compression
+gzip compressed data, was "goshdb-0.2.1.tar", max compression
```

## Comparing `goshdb-0.2.0.tar` & `goshdb-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1063 2024-05-09 20:05:17.913447 goshdb-0.2.0/LICENSE
--rw-r--r--   0        0        0     4092 2024-05-09 20:57:38.631275 goshdb-0.2.0/README.md
--rw-r--r--   0        0        0      690 2024-05-09 20:57:38.696262 goshdb-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       31 2024-05-09 20:09:00.057862 goshdb-0.2.0/src/goshdb/__init__.py
--rw-r--r--   0        0        0     1901 2024-05-09 20:09:00.055620 goshdb-0.2.0/src/goshdb/integrated_test.py
--rw-r--r--   0        0        0     7068 2024-05-09 20:09:00.029869 goshdb-0.2.0/src/goshdb/sheet.py
--rw-r--r--   0        0        0     5641 2024-05-09 21:32:30.853618 goshdb-0.2.0/src/goshdb/table.py
--rw-r--r--   0        0        0     4910 1970-01-01 00:00:00.000000 goshdb-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-09 20:05:17.913447 goshdb-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4092 2024-05-10 10:51:50.241403 goshdb-0.2.1/README.md
+-rw-r--r--   0        0        0      690 2024-05-10 10:52:39.076491 goshdb-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       31 2024-05-09 20:09:00.057862 goshdb-0.2.1/src/goshdb/__init__.py
+-rw-r--r--   0        0        0     1901 2024-05-09 20:09:00.055620 goshdb-0.2.1/src/goshdb/integrated_test.py
+-rw-r--r--   0        0        0     7068 2024-05-09 20:09:00.029869 goshdb-0.2.1/src/goshdb/sheet.py
+-rw-r--r--   0        0        0     5641 2024-05-09 21:32:30.853618 goshdb-0.2.1/src/goshdb/table.py
+-rw-r--r--   0        0        0     4910 1970-01-01 00:00:00.000000 goshdb-0.2.1/PKG-INFO
```

### Comparing `goshdb-0.2.0/LICENSE` & `goshdb-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `goshdb-0.2.0/README.md` & `goshdb-0.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,25 @@
 * Though `Table` uses only provided spreadsheet, credentials technically 
 allow to read/write all the spreadsheets in the account.
 * So it's recommended to use `Table` with a special service (non-personal)
 account that doesn't have critical/secret spreadsheets that might be compromised.
 
 </details>
 
-#### Step 2. Obtain credentials.json file with this the [instruction](https://developers.google.com/sheets/api/quickstart/python)
+#### Step 2. Create a spreadsheet in your Google Sheets account.
+
+<details>
+<summary>Details</summary>
+
+* You should share the spreadsheet and provide write access to the account that will be used to 
+access it (see Step 1).
+
+</details>
+
+#### Step 3. Obtain credentials.json file with this the [instruction](https://developers.google.com/sheets/api/quickstart/python)
 
 <details>
 <summary>Details</summary>
 
 * If you do this for the first time - take `credentials.json` and put it in `secret_dir`.
 * On a first attempt to create `Table` it'll open a browser window, ask you to sign in 
 the target test account.
@@ -69,38 +79,28 @@
 * The `token.json` file will be used automatically for further access to the
 target spreadsheet.
 * You can use `token.json` to access the spreadsheet from another machine without completing the 
 steps above
 
 </details>
 
-#### Step 3. Create a spreadsheet in your Google Sheets account.
-
-<details>
-<summary>Details</summary>
-
-* You should share the spreadsheet and provide write access to the account that will be used to 
-access it (see Step 1).
-
-</details>
-
 
 # Usage
 ```python
 from goshdb import Table
 from pathlib import Path
 
 # Take spreadsheet ID from your spreadsheet URL:
 # https://docs.google.com/spreadsheets/d/[SPREADSHEET_ID]/edit#gid=0
 SPREADSHEET_ID = '...'
 # Provide a sheet name. It should be either new sheet or existing one that follows the required structure.
 SHEET_NAME = '...'  
 
 
-# Create a Table object. If you do this for the first time - it'll open a browser window (see Step 2 details)
+# Create a Table object. If you do this for the first time - it'll open a browser window (see Step 3 details)
 table = Table(
     secret_dir=Path('path/to/secret_dir'),
     spreadsheet_id=SPREADSHEET_ID,
     sheet_name=SHEET_NAME
 )
 
 # Write a key-value pair
```

### Comparing `goshdb-0.2.0/pyproject.toml` & `goshdb-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "goshdb"
-version = "0.2.0"
+version = "0.2.1"
 description = "GOogle SHeets DataBase - Python client to key-value database based on Google Sheets"
 authors = ["Artyom Vorobyov <artyom.vorobyov@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/artoby/goshdb"
 keywords = ["google", "sheets", "spreadsheet", "database", "key-value", "free", "nosql"]
 classifiers = [
```

### Comparing `goshdb-0.2.0/src/goshdb/integrated_test.py` & `goshdb-0.2.1/src/goshdb/integrated_test.py`

 * *Files identical despite different names*

### Comparing `goshdb-0.2.0/src/goshdb/sheet.py` & `goshdb-0.2.1/src/goshdb/sheet.py`

 * *Files identical despite different names*

### Comparing `goshdb-0.2.0/src/goshdb/table.py` & `goshdb-0.2.1/src/goshdb/table.py`

 * *Files identical despite different names*

### Comparing `goshdb-0.2.0/PKG-INFO` & `goshdb-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goshdb
-Version: 0.2.0
+Version: 0.2.1
 Summary: GOogle SHeets DataBase - Python client to key-value database based on Google Sheets
 Home-page: https://github.com/artoby/goshdb
 License: MIT
 Keywords: google,sheets,spreadsheet,database,key-value,free,nosql
 Author: Artyom Vorobyov
 Author-email: artyom.vorobyov@gmail.com
 Requires-Python: >=3.10,<3.11
@@ -74,15 +74,25 @@
 * Though `Table` uses only provided spreadsheet, credentials technically 
 allow to read/write all the spreadsheets in the account.
 * So it's recommended to use `Table` with a special service (non-personal)
 account that doesn't have critical/secret spreadsheets that might be compromised.
 
 </details>
 
-#### Step 2. Obtain credentials.json file with this the [instruction](https://developers.google.com/sheets/api/quickstart/python)
+#### Step 2. Create a spreadsheet in your Google Sheets account.
+
+<details>
+<summary>Details</summary>
+
+* You should share the spreadsheet and provide write access to the account that will be used to 
+access it (see Step 1).
+
+</details>
+
+#### Step 3. Obtain credentials.json file with this the [instruction](https://developers.google.com/sheets/api/quickstart/python)
 
 <details>
 <summary>Details</summary>
 
 * If you do this for the first time - take `credentials.json` and put it in `secret_dir`.
 * On a first attempt to create `Table` it'll open a browser window, ask you to sign in 
 the target test account.
@@ -90,38 +100,28 @@
 * The `token.json` file will be used automatically for further access to the
 target spreadsheet.
 * You can use `token.json` to access the spreadsheet from another machine without completing the 
 steps above
 
 </details>
 
-#### Step 3. Create a spreadsheet in your Google Sheets account.
-
-<details>
-<summary>Details</summary>
-
-* You should share the spreadsheet and provide write access to the account that will be used to 
-access it (see Step 1).
-
-</details>
-
 
 # Usage
 ```python
 from goshdb import Table
 from pathlib import Path
 
 # Take spreadsheet ID from your spreadsheet URL:
 # https://docs.google.com/spreadsheets/d/[SPREADSHEET_ID]/edit#gid=0
 SPREADSHEET_ID = '...'
 # Provide a sheet name. It should be either new sheet or existing one that follows the required structure.
 SHEET_NAME = '...'  
 
 
-# Create a Table object. If you do this for the first time - it'll open a browser window (see Step 2 details)
+# Create a Table object. If you do this for the first time - it'll open a browser window (see Step 3 details)
 table = Table(
     secret_dir=Path('path/to/secret_dir'),
     spreadsheet_id=SPREADSHEET_ID,
     sheet_name=SHEET_NAME
 )
 
 # Write a key-value pair
```

