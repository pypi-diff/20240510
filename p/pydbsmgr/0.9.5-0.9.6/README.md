# Comparing `tmp/pydbsmgr-0.9.5.tar.gz` & `tmp/pydbsmgr-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydbsmgr-0.9.5.tar", last modified: Mon Apr 22 22:52:29 2024, max compression
+gzip compressed data, was "pydbsmgr-0.9.6.tar", last modified: Fri May 10 02:50:19 2024, max compression
```

## Comparing `pydbsmgr-0.9.5.tar` & `pydbsmgr-0.9.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:52:29.874944 pydbsmgr-0.9.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-22 22:52:24.000000 pydbsmgr-0.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-04-22 22:52:29.874944 pydbsmgr-0.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-22 22:52:24.000000 pydbsmgr-0.9.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:52:29.870944 pydbsmgr-0.9.5/pydbsmgr/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-22 22:52:24.000000 pydbsmgr-0.9.5/pydbsmgr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10815 2024-04-22 22:52:24.000000 pydbsmgr-0.9.5/pydbsmgr/fast_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     7499 2024-04-22 22:52:24.000000 pydbsmgr-0.9.5/pydbsmgr/health.py
--rw-r--r--   0 runner    (1001) docker     (127)     9412 2024-04-22 22:52:24.000000 pydbsmgr-0.9.5/pydbsmgr/lightest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-04-22 22:52:24.000000 pydbsmgr-0.9.5/pydbsmgr/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14750 2024-04-22 22:52:24.000000 pydbsmgr-0.9.5/pydbsmgr/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:52:29.870944 pydbsmgr-0.9.5/pydbsmgr/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-22 22:52:24.000000 pydbsmgr-0.9.5/pydbsmgr/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10226 2024-04-22 22:52:24.000000 pydbsmgr-0.9.5/pydbsmgr/utils/azure_sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-22 22:52:24.000000 pydbsmgr-0.9.5/pydbsmgr/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    13970 2024-04-22 22:52:24.000000 pydbsmgr-0.9.5/pydbsmgr/utils/sql_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:52:29.870944 pydbsmgr-0.9.5/pydbsmgr/utils/tools/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-22 22:52:24.000000 pydbsmgr-0.9.5/pydbsmgr/utils/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14075 2024-04-22 22:52:24.000000 pydbsmgr-0.9.5/pydbsmgr/utils/tools/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:52:29.874944 pydbsmgr-0.9.5/pydbsmgr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-04-22 22:52:29.000000 pydbsmgr-0.9.5/pydbsmgr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-22 22:52:29.000000 pydbsmgr-0.9.5/pydbsmgr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 22:52:29.000000 pydbsmgr-0.9.5/pydbsmgr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-22 22:52:29.000000 pydbsmgr-0.9.5/pydbsmgr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-22 22:52:29.000000 pydbsmgr-0.9.5/pydbsmgr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 22:52:29.874944 pydbsmgr-0.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-22 22:52:24.000000 pydbsmgr-0.9.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:52:29.874944 pydbsmgr-0.9.5/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 22:52:24.000000 pydbsmgr-0.9.5/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-22 22:52:24.000000 pydbsmgr-0.9.5/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-22 22:52:24.000000 pydbsmgr-0.9.5/test/test_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:50:19.206214 pydbsmgr-0.9.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-10 02:50:13.000000 pydbsmgr-0.9.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-05-10 02:50:19.206214 pydbsmgr-0.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-10 02:50:13.000000 pydbsmgr-0.9.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:50:19.202214 pydbsmgr-0.9.6/pydbsmgr/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-10 02:50:13.000000 pydbsmgr-0.9.6/pydbsmgr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10815 2024-05-10 02:50:13.000000 pydbsmgr-0.9.6/pydbsmgr/fast_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7590 2024-05-10 02:50:13.000000 pydbsmgr-0.9.6/pydbsmgr/health.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9406 2024-05-10 02:50:13.000000 pydbsmgr-0.9.6/pydbsmgr/lightest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-05-10 02:50:13.000000 pydbsmgr-0.9.6/pydbsmgr/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14787 2024-05-10 02:50:13.000000 pydbsmgr-0.9.6/pydbsmgr/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:50:19.206214 pydbsmgr-0.9.6/pydbsmgr/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-10 02:50:13.000000 pydbsmgr-0.9.6/pydbsmgr/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10226 2024-05-10 02:50:13.000000 pydbsmgr-0.9.6/pydbsmgr/utils/azure_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-10 02:50:13.000000 pydbsmgr-0.9.6/pydbsmgr/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14091 2024-05-10 02:50:13.000000 pydbsmgr-0.9.6/pydbsmgr/utils/sql_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:50:19.206214 pydbsmgr-0.9.6/pydbsmgr/utils/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-10 02:50:13.000000 pydbsmgr-0.9.6/pydbsmgr/utils/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14316 2024-05-10 02:50:13.000000 pydbsmgr-0.9.6/pydbsmgr/utils/tools/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:50:19.206214 pydbsmgr-0.9.6/pydbsmgr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-05-10 02:50:19.000000 pydbsmgr-0.9.6/pydbsmgr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-10 02:50:19.000000 pydbsmgr-0.9.6/pydbsmgr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 02:50:19.000000 pydbsmgr-0.9.6/pydbsmgr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-10 02:50:19.000000 pydbsmgr-0.9.6/pydbsmgr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-10 02:50:19.000000 pydbsmgr-0.9.6/pydbsmgr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 02:50:19.206214 pydbsmgr-0.9.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-10 02:50:13.000000 pydbsmgr-0.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:50:19.206214 pydbsmgr-0.9.6/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 02:50:13.000000 pydbsmgr-0.9.6/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-10 02:50:13.000000 pydbsmgr-0.9.6/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-10 02:50:13.000000 pydbsmgr-0.9.6/test/test_functions.py
```

### Comparing `pydbsmgr-0.9.5/LICENSE` & `pydbsmgr-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pydbsmgr-0.9.5/PKG-INFO` & `pydbsmgr-0.9.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydbsmgr
-Version: 0.9.5
+Version: 0.9.6
 Summary: Python package for database control and DataFrame processing
 Home-page: https://github.com/jzsmoreno/pydbsmgr
 Author: J. A. Moreno-Guerra
 Author-email: jzs.gm27@gmail.com
 Maintainer: David Pedroza
 Maintainer-email: david.pedroza.segoviano@gmail.com
 License: MIT
@@ -36,15 +36,15 @@
 ![GitHub last commit](https://img.shields.io/github/last-commit/jzsmoreno/pydbsmgr?style=for-the-badge)
 ![GitHub repo size](https://img.shields.io/github/repo-size/jzsmoreno/pydbsmgr?style=for-the-badge)
 ![License](https://img.shields.io/github/license/jzsmoreno/pydbsmgr?style=for-the-badge)
 [![CI - Test](https://github.com/jzsmoreno/pydbsmgr/actions/workflows/python-app.yml/badge.svg)](https://github.com/jzsmoreno/pydbsmgr/actions/workflows/python-app.yml)
 
 # pydbsmgr
 
-Python package for database control and administration as well as for DataFrame processing. Also contains a simpler [Python SDK for Azure Cloud tools](https://learn.microsoft.com/en-us/azure/developer/python/sdk/azure-sdk-overview) such as uploading `.parquet`, `.csv` and `.xlsx` files, downloading them and DataFrame cleansing.
+Python package for database control and administration as well as for DataFrame processing. Also contains a simpler [Python SDK for Azure Cloud tools](https://learn.microsoft.com/en-us/azure/developer/python/sdk/azure-sdk-overview) such as uploading `.parquet`, `.csv` and `.xlsx` files, downloading them and DataFrame cleansing, for more information review our [`documentation`](https://jzsmoreno.github.io/pydbsmgr/).
 
 ## Prerequisities
 
 Before you begin, ensure you have met the following requirements:
 
 - You have a _Windows/Linux/Mac_ machine running [Python 3.10+](https://www.python.org/).
 - You have installed the latest versions of [`pip`](https://pip.pypa.io/en/stable/installing/) and [`virtualenv`](https://virtualenv.pypa.io/en/stable/installation/) or `conda` ([Anaconda](https://www.anaconda.com/distribution/)).
```

### Comparing `pydbsmgr-0.9.5/README.md` & `pydbsmgr-0.9.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ![GitHub last commit](https://img.shields.io/github/last-commit/jzsmoreno/pydbsmgr?style=for-the-badge)
 ![GitHub repo size](https://img.shields.io/github/repo-size/jzsmoreno/pydbsmgr?style=for-the-badge)
 ![License](https://img.shields.io/github/license/jzsmoreno/pydbsmgr?style=for-the-badge)
 [![CI - Test](https://github.com/jzsmoreno/pydbsmgr/actions/workflows/python-app.yml/badge.svg)](https://github.com/jzsmoreno/pydbsmgr/actions/workflows/python-app.yml)
 
 # pydbsmgr
 
-Python package for database control and administration as well as for DataFrame processing. Also contains a simpler [Python SDK for Azure Cloud tools](https://learn.microsoft.com/en-us/azure/developer/python/sdk/azure-sdk-overview) such as uploading `.parquet`, `.csv` and `.xlsx` files, downloading them and DataFrame cleansing.
+Python package for database control and administration as well as for DataFrame processing. Also contains a simpler [Python SDK for Azure Cloud tools](https://learn.microsoft.com/en-us/azure/developer/python/sdk/azure-sdk-overview) such as uploading `.parquet`, `.csv` and `.xlsx` files, downloading them and DataFrame cleansing, for more information review our [`documentation`](https://jzsmoreno.github.io/pydbsmgr/).
 
 ## Prerequisities
 
 Before you begin, ensure you have met the following requirements:
 
 - You have a _Windows/Linux/Mac_ machine running [Python 3.10+](https://www.python.org/).
 - You have installed the latest versions of [`pip`](https://pip.pypa.io/en/stable/installing/) and [`virtualenv`](https://virtualenv.pypa.io/en/stable/installation/) or `conda` ([Anaconda](https://www.anaconda.com/distribution/)).
```

### Comparing `pydbsmgr-0.9.5/pydbsmgr/fast_upload.py` & `pydbsmgr-0.9.6/pydbsmgr/fast_upload.py`

 * *Files identical despite different names*

### Comparing `pydbsmgr-0.9.5/pydbsmgr/health.py` & `pydbsmgr-0.9.6/pydbsmgr/health.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,18 +29,20 @@
             self._dfs = [_df]
         else:
             raise TypeError("Input should be either a single dataframe or a list of dataframes")
 
     def fix(self, cols_upper_case: bool = False, drop_empty_cols: bool = True) -> None:
         """Performs the clean of the data and validation
 
-        Args:
-        -----
-            cols_upper_case (`bool`, optional): Indicates whether to convert column names to uppercase. Defaults to `False`.
-            drop_empty_cols (`bool`, optional): Variable indicating whether columns with all their values empty should be removed. Defaults to `True`.
+        Parameters
+        ----------
+        cols_upper_case : `bool`, `optional`
+            Indicates whether to convert column names to uppercase. Defaults to `False`.
+        drop_empty_cols : `bool`, `optional`
+            Variable indicating whether columns with all their values empty should be removed. Defaults to `True`.
         """
         if drop_empty_cols:
             for count, df in enumerate(self._dfs):
                 self._dfs[count] = drop_empty_columns(df)
                 logger.info(f"{count+1}) Empty columns have been removed.")
                 self._dfs[count].columns = clean_transform(df.columns, cols_upper_case)
                 logger.info(f"{count+1}) Columns have been cleaned and transformed.")
@@ -56,22 +58,28 @@
         database_name: str = "database",
         directory_name: str = "summary",
         concat_vertically: bool = False,
         encoding: str = "utf-8",
     ) -> None:
         """Generate a `.html` health check report.
 
-        Args:
-        -----
-            report_name (`str`, optional): Name of the quality assessment report. Defaults to `./report.html`.
-            yaml_name (`str`, optional): Indicates the name of the `.yaml` file that will serve as a template for the creation of the SQL table. Defaults to `./output.yaml`.
-            database_name (`str`, optional): The header of the `.yaml` file. Default value is `database`
-            directory_name (`str`, optional): Folder in which the reports will be saved. Defaults to `summary`.
-            concat_vertically: (`bool`, optional), Variable indicating whether the list of dataframes should be vertically concatenated into a single one. Default value is `False`.
-            encoding (`str`, optional): The encoding of dataframes. Defaults to `utf-8`.
+        Parameters
+        ----------
+        report_name : `str`, `optional`
+            Name of the quality assessment report. Defaults to `./report.html`.
+        yaml_name : `str`, `optional`
+            Indicates the name of the `.yaml` file that will serve as a template for the creation of the SQL table. Defaults to `./output.yaml`.
+        database_name : `str`, `optional`
+            The header of the `.yaml` file. Default value is `database`
+        directory_name : `str`, `optional`
+            Folder in which the reports will be saved. Defaults to `summary`.
+        concat_vertically : `bool`, `optional`
+            Variable indicating whether the list of dataframes should be vertically concatenated into a single one. Default value is `False`.
+        encoding : `str`, `optional`
+            The encoding of dataframes. Defaults to `utf-8`.
         """
         self.df_files_info = pd.DataFrame()
         self.yaml_name = yaml_name
         self.database_name = database_name
         if not os.path.exists(directory_name):
             os.mkdir(directory_name)
             warning_type = "UserWarning"
```

### Comparing `pydbsmgr-0.9.5/pydbsmgr/lightest.py` & `pydbsmgr-0.9.6/pydbsmgr/lightest.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 
 
 def process_dates(x: str, format_type: str, auxiliary_type: str, errors: str = "ignore") -> str:
     """Auxiliary function in date type string processing
 
     Parameters
     ----------
-        x : `str`
-            character of type date.
+    x : `str`
+        character of type date.
 
     Returns
     ----------
-        x : `str`
-            character after processing with format `YYYY-MM-DD`.
+    x : `str`
+        character after processing with format `YYYY-MM-DD`.
     """
     # performing data type conversion
     x = str(x)
     if format_type in ["dayfirst", "monthfirst"] and len(x) < 10:
         # split by "/" or "-"
         if format_type == "dayfirst":
             dmy = x.split("/") if "/" in x else x.split("-")
@@ -74,24 +74,25 @@
         two_date_formats: bool = True,
         **kwargs,
     ) -> DataFrame:
         """`DataFrame` cleaning main function
 
         Parameters
         ----------
-        - sample_frac (`float`): The fraction of rows to use for date type inference. Default is 0.1 i.e., 10%.
-        - fast_execution (`bool`): If `False` use `applymap` pandas for extra text cleanup. Default is `True`.
+        sample_frac : `float`
+            The fraction of rows to use for date type inference. Default is 0.1 i.e., 10%.
+        fast_execution : `bool`
+            If `False` use `applymap` pandas for extra text cleanup. Default is `True`.
 
         Keyword Arguments:
         ----------
-        - no_emoji: (`bool`): By default it is set to `False`.
-        If `True`, removes all emojis from text data. Works only when `fast_execution` = `False`.
-        - title_mode: (`bool`): By default it is set to `True`.
-        If `False`, converts the text to lowercase. Works only when `fast_execution` = `False`.
-        By default, converts everything to `title`.
+        no_emoji : `bool`
+            By default it is set to `False`. If `True`, removes all emojis from text data. Works only when `fast_execution` = `False`.
+        title_mode : `bool`
+            By default it is set to `True`. If `False`, converts the text to lowercase. Works only when `fast_execution` = `False`. By default, converts everything to `title`.
         """
         table = (self.df).copy()
         cols = table.columns
         table_sample = table.sample(frac=sample_frac)
         errors = kwargs["errors"] if "errors" in kwargs else "ignore"
         for column_index, datatype in enumerate(table.dtypes):
             if datatype == "object":
```

### Comparing `pydbsmgr-0.9.5/pydbsmgr/logs.py` & `pydbsmgr-0.9.6/pydbsmgr/logs.py`

 * *Files identical despite different names*

### Comparing `pydbsmgr-0.9.5/pydbsmgr/main.py` & `pydbsmgr-0.9.6/pydbsmgr/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,19 +51,23 @@
             else:
                 return False
 
 
 def remove_numeric_char(input_string: str) -> str:
     """Remove all numeric characters from a string.
 
-    Args:
-        input_string (`str`): character string to be cleaned of numeric characters
-
-    Returns:
-        `str`: clean character string
+    Parameters
+    ----------
+    input_string : `str`
+        character string to be cleaned of numeric characters
+
+    Returns
+    -------
+    `str`
+        clean character string
     """
     return re.sub(r"\d", "", input_string)
 
 
 def clean(
     dirty_string: str,
     pattern: str = r"[a-zA-Zñáéíóú_@.0-9]+\b",
```

### Comparing `pydbsmgr-0.9.5/pydbsmgr/utils/azure_sdk.py` & `pydbsmgr-0.9.6/pydbsmgr/utils/azure_sdk.py`

 * *Files identical despite different names*

### Comparing `pydbsmgr-0.9.5/pydbsmgr/utils/config.py` & `pydbsmgr-0.9.6/pydbsmgr/utils/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,40 +2,40 @@
 
 
 def load_config(config_file):
     """Load the configuration file.
 
     Parameters
     ----------
-    config_file : str
+    config_file : `str`
         The path to the configuration file.
 
     Returns
     -------
-    config : ConfigParser
+    config : `ConfigParser`
         A configuration object loaded from file.
     """
 
     config = ConfigParser()
     config.read(config_file)
 
     return config
 
 
 def parse_config(config):
     """Parse the configuration file.
 
     Parameters
     ----------
-    config : ConfigParser
+    config : `ConfigParser`
         A configuration object loaded from file.
 
     Returns
     -------
-    parsed_config : dict
+    parsed_config : `dict`
         A dictionary of parsed configuration values.
     """
 
     parsed_config = {}
 
     for key, child in config.items():
         parsed_config[key] = {}
```

### Comparing `pydbsmgr-0.9.5/pydbsmgr/utils/sql_functions.py` & `pydbsmgr-0.9.6/pydbsmgr/utils/sql_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,26 +24,30 @@
         table_name: str,
         overwrite: bool = True,
         char_length: int = 512,
         override_length: bool = True,
     ) -> None:
         """Insert data into SQL Server.
 
-        Parameters:
+        Parameters
         ----------
-            df (`Dataframe` or `str`): The pandas dataframe that will be inserted into sql server
-            table_name (`str`): Name of the table in which the data is being inserted
-            overwrite (`bool`): If `True` it will delete and recreate the table before inserting new data
-            if `False` it will append the new data onto the end of the existing table
-            char_length (`int`): Length of varchar fields for text columns
-            override_length (`bool`): Override length of varchar fields for text columns.
-
-        Returns:
-        ----------
-            `None`
+        df : `Dataframe` | `str`
+            The pandas dataframe that will be inserted into sql server
+        table_name : `str`
+            Name of the table in which the data is being inserted
+        overwrite : `bool`
+            If `True` it will delete and recreate the table before inserting new data if `False` it will append the new data onto the end of the existing table.
+        char_length : `int`
+            Length of varchar fields for text columns.
+        override_length : `bool`
+            Override length of varchar fields for text columns.
+
+        Returns
+        -------
+        `None`
         """
 
         self.file_type = None
         df_to_load: DataFrame = pd.DataFrame()
         if type(df) == str:
             self.path = df
             # read csv file
@@ -127,30 +131,41 @@
         credential_name: str = "UploadCSV_Credential",
         data_source_name: str = "UploadCSV_DS",
         char_length: int = 512,
         overwrite: bool = True,
     ) -> bool:
         """Insert data from csv files in Azure Blob Storage into SQL Server with Bulk command
 
-        Parameters:
-        ----------
-            file_path (`str`): Path to the file in Azure Blob Storage
-            db_table_name (`str`): Name of the table in which the data is being inserted
-            sas_str (`str`): SAS string to the storage account
-            storage_connection_string (`str`): Connection string to the storage account
-            storage_account (`str`): Name of the storage account
-            container_name (`str`): Name of the container in which the data is being inserted
-            credential_name (`str`): Name of the credentials
-            data_source_name (`str`): Name of the data source
-            char_length (`int`): Length of varchar fields for text columns
-            overwrite (`bool`): If `True` it will delete and recreate the table before inserting new data
-            if `False` it will append the new data onto the end of the existing table
-        Returns:
+        Parameters
         ----------
-            `bool`: True if the data was inserted successfully
+        file_path : `str`
+            Path to the file in Azure Blob Storage
+        db_table_name : `str`
+            Name of the table in which the data is being inserted
+        sas_str : `str`
+            SAS string to the storage account
+        storage_connection_string : `str`
+            Connection string to the storage account
+        storage_account : `str`
+            Name of the storage account
+        container_name : `str`
+            Name of the container in which the data is being inserted
+        credential_name : `str`
+            Name of the credentials
+        data_source_name : `str`
+            Name of the data source
+        char_length : `int`
+            Length of varchar fields for text columns
+        overwrite : `bool`
+            If `True` it will delete and recreate the table before inserting new data if `False` it will append the new data onto the end of the existing table.
+
+        Returns
+        -------
+        `bool`
+            True if the data was inserted successfully
         """
         # Get all the files in the container or file individually
         filter_condition = ""
         if not file_path.endswith("/"):
             filter_condition = file_path.split("/")[-1]
 
         print("GETTING FILES FROM THE CONTAINER")
@@ -264,21 +279,25 @@
         return True
 
     def drop_dropables(
         self, data_source_name: str, credential_name: str, masterkey: bool = False
     ) -> bool:
         """Drop dropable objects
 
-        Parameters:
+        Parameters
         ----------
-            data_source_name (`str`): Name of the data source
-            masterkey (`bool`): If `True` it will drop the master key
-        Returns:
-        ----------
-            `Bool`: True if the data was inserted successfully
+        data_source_name : `str`
+            Name of the data source
+        masterkey : `bool`
+            If `True` it will drop the master key
+
+        Returns
+        -------
+        `bool`
+            True if the data was inserted successfully
         """
         print("DROPPING EXTERNAL DATA SOURCE")
         self._cur.execute(f"DROP EXTERNAL DATA SOURCE {data_source_name}")
         print("DROPPING CREDENTIALS")
         self._cur.execute(f"DROP DATABASE SCOPED CREDENTIAL {credential_name}")
         if masterkey:
             print("DROPPING MASTER KEY")
@@ -335,22 +354,28 @@
         self,
         df_list: list[DataFrame],
         name_list: list[str],
         directory: str = "/",
         write_to_csv: bool = True,
     ) -> None:
         """Write a csv file from parquet files in a container
-        Parameters:
-        ----------
-            connection_string (`str`): Connection string to the storage account
-            container_name (`str`): Name of the container in which the data is being inserted
-            directory (`str`): Directory in which the parquet files are located
-        Returns:
+
+        Parameters
         ----------
-            `bool`: True if the file was created successfully
+        connection_string : `str`
+            Connection string to the storage account
+        container_name : `str`
+            Name of the container in which the data is being inserted
+        directory : `str`
+            Directory in which the parquet files are located
+
+        Returns
+        -------
+        `bool`
+            `True` if the file was created successfully
         """
         # Write the csv files
         if write_to_csv:
             print("WRITING CSV FILES")
             self.storage_controller.upload_excel_csv(
                 directory_name=directory,
                 dfs=df_list,
```

### Comparing `pydbsmgr-0.9.5/pydbsmgr/utils/tools/tools.py` & `pydbsmgr-0.9.6/pydbsmgr/utils/tools/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,22 +38,25 @@
     else:
         return func
 
 
 def most_repeated_item(items: list, two_most_common: bool = False) -> Tuple[str, str | None]:
     """Returns a `Tuple` with the most common elements of a `list`.
 
-    Args:
+    Parameters
     ----------
-        items (`list`): the `list` containing the items to be evaluated.
-        two_most_common (`bool`, optional): If `False`, returns only one element. Defaults to `False`.
-
-    Returns:
-    ----------
-        Tuple[`str`, `str` | `None`]: The two most common elements.
+    items : `list`
+        the `list` containing the items to be evaluated.
+    two_most_common : `bool`, `optional`
+        If `False`, returns only one element. Defaults to `False`.
+
+    Returns
+    -------
+    Tuple[`str`, `str` | `None`]
+        The two most common elements.
     """
     # Use Counter to count occurrences of each item in the list
     counter = Counter(items)
 
     # Find the two most common items and its count
     most_common = counter.most_common(2)
 
@@ -152,15 +155,15 @@
         self,
         directory_name: str,
         dfs: List[DataFrame],
         names: List[str],
         overwrite: bool = True,
         upload: bool = True,
     ) -> None:
-        """Write dataframes as `parquet` format by converting them first into `bytes`"""
+        """Write dataframes as `parquet` format by converting them first into `bytes`."""
         files = []
         format_type = "parquet"
         files_not_loaded = []
         for data, blob_name in zip(dfs, names):
             if data != None:
                 table = pa.Table.from_pandas(data)
                 buf = pa.BufferOutputStream()
@@ -181,28 +184,30 @@
             return files_not_loaded
 
         if not upload:
             return files
 
 
 def column_coincidence(df1: DataFrame, df2: DataFrame) -> float:
+    """Return the percentage of coincident columns between two pandas dataframes."""
     if not isinstance(df1, pd.DataFrame) or not isinstance(df2, pd.DataFrame):
         raise ValueError("Both inputs should be pandas DataFrames")
 
     column_names1 = set(df1.columns)
     column_names2 = set(df2.columns)
 
     common_columns = column_names1.intersection(column_names2)
     total_columns = column_names1.union(column_names2)
 
     coincidence_percentage = len(common_columns) / len(total_columns)
     return coincidence_percentage
 
 
 def merge_by_coincidence(df1: DataFrame, df2: DataFrame, tol: float = 0.9) -> DataFrame:
+    """Merge two pandas dataframes by finding the most similar columns based on their names."""
     percentage = column_coincidence(df1, df2)
     total_columns = set(df1.columns).union(set(df2.columns))
     num_col1 = len(df1.columns)
     num_col2 = len(df2.columns)
     if num_col1 < num_col2:
         min_cols = set(df1.columns)
         min_cols = list(min_cols.intersection(set(df2.columns)))
@@ -245,22 +250,25 @@
 
 
 def get_extraction_date(
     filename: str | List[str], REGEX_PATTERN: str = r"\d{4}-\d{2}-\d{2}"
 ) -> str:
     """Allows to extract the date of extraction according to the directory within the storage account.
 
-    Args:
-    ----------
-        filename (`str` | List[`str`]): file path inside the storage account
-        REGEX_PATTERN (`str`, optional): regular expression pattern to extract the date. Defaults to `r"\d{4}-\d{2}-\d{2}"`.
-
-    Returns:
+    Parameters
     ----------
-        `str`: the date that was extracted if found in the file path.
+    filename : `str` | List[`str`]
+        file path inside the storage account
+    REGEX_PATTERN : `str`, `optional`
+        regular expression pattern to extract the date. Defaults to `r"\d{4}-\d{2}-\d{2}"`.
+
+    Returns
+    -------
+    `str`
+        the date that was extracted if found in the file path.
     """
 
     def sub_extraction_date(filename: str, REGEX_PATTERN: str) -> str:
         extraction_date = re.findall(REGEX_PATTERN, filename)
         if len(extraction_date) > 0:
             _date = extraction_date[0]
         else:
@@ -292,17 +300,15 @@
         self._check_datetime(sample_frac)
         return self.df
 
     def get_frame(self) -> DataFrame:
         return self.df
 
     def _check_int_float(self, drop_values: bool = False, drop_rows: bool = False) -> None:
-        """
-        Check and correct the data types of columns in a `DataFrame`.
-        """
+        """Check and correct the data types of columns in a `DataFrame`."""
 
         def check_float(x):
             if isinstance(x, str):
                 try:
                     return float(x)
                 except:
                     return np.nan
@@ -346,17 +352,15 @@
                                 val_dtype = "object"
                                 print("Checking {%s} for column {%s}" % (val_dtype, col))
 
                         print(f"Successfully transformed the '{col}' column into {val_dtype}.")
         self.df = df_
 
     def _check_datetime(self, sample_frac: float) -> None:
-        """
-        Check and convert date-time string columns to datetime objects.
-        """
+        """Check and convert date-time string columns to `datetime` objects."""
         df_ = self.df
         cols = df_.columns
         df_sample = df_.sample(frac=sample_frac)
         for column_index, datatype in enumerate(df_.dtypes):
             col = cols[column_index]
             if datatype == "object":
                 datetype_column = (df_sample[col].apply(check_if_contains_dates)).isin([True]).any()
@@ -378,27 +382,26 @@
                 df_[col] = df_[col].dt.normalize()
                 print(f"Successfully transformed the '{col}' column into datetime64[ns].")
 
         self.df = df_
 
 
 def create_directory(data, parent_path=""):
-    """
-    Creates the directory tree from a yaml file
-    """
+    """Creates the directory tree from a `yaml` file."""
     for key, value in data.items():
         path = os.path.join(parent_path, key)
         if isinstance(value, dict):
             os.makedirs(path, exist_ok=True)
             create_directory(value, path)
         else:
             os.makedirs(path, exist_ok=True)
 
 
 def create_directories_from_yaml(yaml_file):
+    """Reads a `yaml` file and creates directories based on its content."""
     with open(yaml_file, "r") as file:
         data = yaml.safe_load(file)
         create_directory(data)
 
 
 if __name__ == "__main__":
     yaml_file = "directories.yaml"
```

### Comparing `pydbsmgr-0.9.5/pydbsmgr.egg-info/PKG-INFO` & `pydbsmgr-0.9.6/pydbsmgr.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydbsmgr
-Version: 0.9.5
+Version: 0.9.6
 Summary: Python package for database control and DataFrame processing
 Home-page: https://github.com/jzsmoreno/pydbsmgr
 Author: J. A. Moreno-Guerra
 Author-email: jzs.gm27@gmail.com
 Maintainer: David Pedroza
 Maintainer-email: david.pedroza.segoviano@gmail.com
 License: MIT
@@ -36,15 +36,15 @@
 ![GitHub last commit](https://img.shields.io/github/last-commit/jzsmoreno/pydbsmgr?style=for-the-badge)
 ![GitHub repo size](https://img.shields.io/github/repo-size/jzsmoreno/pydbsmgr?style=for-the-badge)
 ![License](https://img.shields.io/github/license/jzsmoreno/pydbsmgr?style=for-the-badge)
 [![CI - Test](https://github.com/jzsmoreno/pydbsmgr/actions/workflows/python-app.yml/badge.svg)](https://github.com/jzsmoreno/pydbsmgr/actions/workflows/python-app.yml)
 
 # pydbsmgr
 
-Python package for database control and administration as well as for DataFrame processing. Also contains a simpler [Python SDK for Azure Cloud tools](https://learn.microsoft.com/en-us/azure/developer/python/sdk/azure-sdk-overview) such as uploading `.parquet`, `.csv` and `.xlsx` files, downloading them and DataFrame cleansing.
+Python package for database control and administration as well as for DataFrame processing. Also contains a simpler [Python SDK for Azure Cloud tools](https://learn.microsoft.com/en-us/azure/developer/python/sdk/azure-sdk-overview) such as uploading `.parquet`, `.csv` and `.xlsx` files, downloading them and DataFrame cleansing, for more information review our [`documentation`](https://jzsmoreno.github.io/pydbsmgr/).
 
 ## Prerequisities
 
 Before you begin, ensure you have met the following requirements:
 
 - You have a _Windows/Linux/Mac_ machine running [Python 3.10+](https://www.python.org/).
 - You have installed the latest versions of [`pip`](https://pip.pypa.io/en/stable/installing/) and [`virtualenv`](https://virtualenv.pypa.io/en/stable/installation/) or `conda` ([Anaconda](https://www.anaconda.com/distribution/)).
```

### Comparing `pydbsmgr-0.9.5/pydbsmgr.egg-info/SOURCES.txt` & `pydbsmgr-0.9.6/pydbsmgr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydbsmgr-0.9.5/setup.py` & `pydbsmgr-0.9.6/setup.py`

 * *Files identical despite different names*

### Comparing `pydbsmgr-0.9.5/test/conftest.py` & `pydbsmgr-0.9.6/test/conftest.py`

 * *Files identical despite different names*

### Comparing `pydbsmgr-0.9.5/test/test_functions.py` & `pydbsmgr-0.9.6/test/test_functions.py`

 * *Files identical despite different names*

