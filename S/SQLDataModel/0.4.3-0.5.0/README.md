# Comparing `tmp/sqldatamodel-0.4.3.tar.gz` & `tmp/sqldatamodel-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqldatamodel-0.4.3.tar", last modified: Tue May  7 19:28:58 2024, max compression
+gzip compressed data, was "sqldatamodel-0.5.0.tar", last modified: Thu May  9 22:08:42 2024, max compression
```

## Comparing `sqldatamodel-0.4.3.tar` & `sqldatamodel-0.5.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 19:28:58.071769 sqldatamodel-0.4.3/
--rw-rw-rw-   0        0        0     1095 2024-03-19 13:42:59.000000 sqldatamodel-0.4.3/LICENSE
--rw-rw-rw-   0        0        0    29557 2024-05-07 19:28:58.062878 sqldatamodel-0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0    27665 2024-05-07 00:24:25.000000 sqldatamodel-0.4.3/README.md
--rw-rw-rw-   0        0        0       86 2023-12-16 01:14:43.000000 sqldatamodel-0.4.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-07 19:28:58.073546 sqldatamodel-0.4.3/setup.cfg
--rw-rw-rw-   0        0        0     2424 2024-05-07 19:27:52.000000 sqldatamodel-0.4.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-07 19:28:56.209775 sqldatamodel-0.4.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-07 19:28:57.391305 sqldatamodel-0.4.3/src/SQLDataModel/
--rw-rw-rw-   0        0        0     6644 2024-05-03 15:03:44.000000 sqldatamodel-0.4.3/src/SQLDataModel/ANSIColor.py
--rw-rw-rw-   0        0        0     9146 2024-03-20 22:08:53.000000 sqldatamodel-0.4.3/src/SQLDataModel/HTMLParser.py
--rw-rw-rw-   0        0        0     1267 2024-03-19 22:36:01.000000 sqldatamodel-0.4.3/src/SQLDataModel/JSONEncoder.py
--rw-rw-rw-   0        0        0   609546 2024-05-07 18:50:28.000000 sqldatamodel-0.4.3/src/SQLDataModel/SQLDataModel.py
--rw-rw-rw-   0        0        0     2286 2024-03-19 22:36:42.000000 sqldatamodel-0.4.3/src/SQLDataModel/StandardDeviation.py
--rw-rw-rw-   0        0        0      173 2024-03-05 04:16:05.000000 sqldatamodel-0.4.3/src/SQLDataModel/__init__.py
--rw-rw-rw-   0        0        0     1501 2024-03-19 22:35:10.000000 sqldatamodel-0.4.3/src/SQLDataModel/converters.py
--rw-rw-rw-   0        0        0     1269 2024-03-19 22:35:23.000000 sqldatamodel-0.4.3/src/SQLDataModel/demo.py
--rw-rw-rw-   0        0        0     2826 2024-03-19 22:35:37.000000 sqldatamodel-0.4.3/src/SQLDataModel/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-07 19:28:57.978627 sqldatamodel-0.4.3/src/SQLDataModel/extensions/
--rw-rw-rw-   0        0        0        0 2024-01-21 21:36:40.000000 sqldatamodel-0.4.3/src/SQLDataModel/extensions/__init__.py
--rw-rw-rw-   0        0        0     1355 2024-01-21 21:24:09.000000 sqldatamodel-0.4.3/src/SQLDataModel/extensions/str_utils.c
-drwxrwxrwx   0        0        0        0 2024-05-07 19:28:58.056312 sqldatamodel-0.4.3/src/SQLDataModel.egg-info/
--rw-rw-rw-   0        0        0    29557 2024-05-07 19:28:56.000000 sqldatamodel-0.4.3/src/SQLDataModel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      642 2024-05-07 19:28:56.000000 sqldatamodel-0.4.3/src/SQLDataModel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 19:28:56.000000 sqldatamodel-0.4.3/src/SQLDataModel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-07 19:28:56.000000 sqldatamodel-0.4.3/src/SQLDataModel.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-07 19:28:57.993626 sqldatamodel-0.4.3/tests/
--rw-rw-rw-   0        0        0    63183 2024-05-07 19:27:28.000000 sqldatamodel-0.4.3/tests/test_Future.py
--rw-rw-rw-   0        0        0    63186 2024-05-07 19:27:26.000000 sqldatamodel-0.4.3/tests/test_SQLDataModel.py
+drwxrwxrwx   0        0        0        0 2024-05-09 22:08:42.125561 sqldatamodel-0.5.0/
+-rw-rw-rw-   0        0        0     1095 2024-03-19 13:42:59.000000 sqldatamodel-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0    29557 2024-05-09 22:08:42.111772 sqldatamodel-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0    27665 2024-05-07 00:24:25.000000 sqldatamodel-0.5.0/README.md
+-rw-rw-rw-   0        0        0       86 2023-12-16 01:14:43.000000 sqldatamodel-0.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-09 22:08:42.127251 sqldatamodel-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     2424 2024-05-09 21:59:33.000000 sqldatamodel-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 22:08:40.188760 sqldatamodel-0.5.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-09 22:08:41.649551 sqldatamodel-0.5.0/src/SQLDataModel/
+-rw-rw-rw-   0        0        0     6644 2024-05-03 15:03:44.000000 sqldatamodel-0.5.0/src/SQLDataModel/ANSIColor.py
+-rw-rw-rw-   0        0        0     9146 2024-03-20 22:08:53.000000 sqldatamodel-0.5.0/src/SQLDataModel/HTMLParser.py
+-rw-rw-rw-   0        0        0     1267 2024-03-19 22:36:01.000000 sqldatamodel-0.5.0/src/SQLDataModel/JSONEncoder.py
+-rw-rw-rw-   0        0        0   613461 2024-05-09 22:06:51.000000 sqldatamodel-0.5.0/src/SQLDataModel/SQLDataModel.py
+-rw-rw-rw-   0        0        0     2286 2024-03-19 22:36:42.000000 sqldatamodel-0.5.0/src/SQLDataModel/StandardDeviation.py
+-rw-rw-rw-   0        0        0      173 2024-03-05 04:16:05.000000 sqldatamodel-0.5.0/src/SQLDataModel/__init__.py
+-rw-rw-rw-   0        0        0     1501 2024-03-19 22:35:10.000000 sqldatamodel-0.5.0/src/SQLDataModel/converters.py
+-rw-rw-rw-   0        0        0     1269 2024-03-19 22:35:23.000000 sqldatamodel-0.5.0/src/SQLDataModel/demo.py
+-rw-rw-rw-   0        0        0     2826 2024-03-19 22:35:37.000000 sqldatamodel-0.5.0/src/SQLDataModel/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-09 22:08:41.970311 sqldatamodel-0.5.0/src/SQLDataModel/extensions/
+-rw-rw-rw-   0        0        0        0 2024-01-21 21:36:40.000000 sqldatamodel-0.5.0/src/SQLDataModel/extensions/__init__.py
+-rw-rw-rw-   0        0        0     1355 2024-01-21 21:24:09.000000 sqldatamodel-0.5.0/src/SQLDataModel/extensions/str_utils.c
+drwxrwxrwx   0        0        0        0 2024-05-09 22:08:42.100706 sqldatamodel-0.5.0/src/SQLDataModel.egg-info/
+-rw-rw-rw-   0        0        0    29557 2024-05-09 22:08:39.000000 sqldatamodel-0.5.0/src/SQLDataModel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      642 2024-05-09 22:08:40.000000 sqldatamodel-0.5.0/src/SQLDataModel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 22:08:39.000000 sqldatamodel-0.5.0/src/SQLDataModel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-09 22:08:39.000000 sqldatamodel-0.5.0/src/SQLDataModel.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 22:08:42.002331 sqldatamodel-0.5.0/tests/
+-rw-rw-rw-   0        0        0    65049 2024-05-09 21:53:26.000000 sqldatamodel-0.5.0/tests/test_Future.py
+-rw-rw-rw-   0        0        0    65052 2024-05-09 21:53:48.000000 sqldatamodel-0.5.0/tests/test_SQLDataModel.py
```

### Comparing `sqldatamodel-0.4.3/LICENSE` & `sqldatamodel-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.4.3/PKG-INFO` & `sqldatamodel-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLDataModel
-Version: 0.4.3
+Version: 0.5.0
 Summary: SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.
 Home-page: https://github.com/AnteT/SQLDataModel
 Author: Ante Tonkovic-Capin
 Author-email: antetc@icloud.com
 Project-URL: Documentation, https://sqldatamodel.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/AnteT/SQLDataModel.git
 Keywords: SQL,ETL,dataframe,terminal-tables,pretty-print-tables,sql2sql,data-analysis,data-science,datamodel,extract,transform,load,web-scraping-tables,data-mining,html,html-table-parsing,apache-arrow,pyarrow,pyarrow-conversion,pyarrow-to-table,pyarrow-to-sql,pyarrow-to-csv,parquet-file-parsing,csv,csv-parsing,markdown,markdown-table-parsing,latex,latex-table-parsing,delimited,delimited-data-parsing,file-conversion,format-conversion,terminal-styling,table-styling,from-sqlite,to-sqlite,from-postgresql,to-postgresql,sql-to-sql,excel,xlsx-file,excel-to-sql,DataFrames,polars2pandas,pandas2polars
```

### Comparing `sqldatamodel-0.4.3/README.md` & `sqldatamodel-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.4.3/setup.py` & `sqldatamodel-0.5.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='SQLDataModel',  
-     version='0.4.3',
+     version='0.5.0',
      scripts=['src/SQLDataModel/SQLDataModel.py'] ,
      author='Ante Tonkovic-Capin',
      author_email='antetc@icloud.com',
      description='SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.',
      keywords=['SQL','ETL','dataframe','terminal-tables','pretty-print-tables','sql2sql','data-analysis','data-science','datamodel','extract','transform','load','web-scraping-tables','data-mining','html','html-table-parsing','apache-arrow','pyarrow','pyarrow-conversion','pyarrow-to-table','pyarrow-to-sql','pyarrow-to-csv','parquet-file-parsing','csv','csv-parsing','markdown','markdown-table-parsing','latex','latex-table-parsing','delimited','delimited-data-parsing','file-conversion','format-conversion','terminal-styling','table-styling','from-sqlite','to-sqlite','from-postgresql','to-postgresql','sql-to-sql','excel','xlsx-file','excel-to-sql','DataFrames','polars2pandas','pandas2polars'],
      license_file='LICENSE',
      long_description=long_description,
```

### Comparing `sqldatamodel-0.4.3/src/SQLDataModel/ANSIColor.py` & `sqldatamodel-0.5.0/src/SQLDataModel/ANSIColor.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.4.3/src/SQLDataModel/HTMLParser.py` & `sqldatamodel-0.5.0/src/SQLDataModel/HTMLParser.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.4.3/src/SQLDataModel/JSONEncoder.py` & `sqldatamodel-0.5.0/src/SQLDataModel/JSONEncoder.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.4.3/src/SQLDataModel/SQLDataModel.py` & `sqldatamodel-0.5.0/src/SQLDataModel/SQLDataModel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1391,36 +1391,38 @@
         return
 
     def get_display_max_rows(self) -> int|None:
         """
         Retrieves the current value of the ``display_max_rows`` property, which determines the maximum rows displayed for ``SQLDataModel``.
 
         Returns:
-            ``int`` or ``None``: The current value of the 'display_max_rows' property.
+            ``int`` or ``None``: The current value set on :py:attr:`SQLDataModel.display_max_rows`.
 
         Example::
 
+            from SQLDataModel import SQLDataModel
+
             # Create model
             sdm = SQLDataModel.from_csv('example.csv', headers=['ID', 'Name', 'Value'])
 
             # Get current value
             display_max_rows = sdm.get_display_max_rows()
 
-            # By default any display will be limited to 1000 rows max
-            print(display_max_rows) # 1000
+            # By default rows will be limited by current terminal height
+            print(display_max_rows) # None
         
         Note:
             - This does not affect the actual number of rows in the model, only the maximum **displayed**.
+            - Use :meth:`SQLDataModel.set_display_max_rows()` to explicitely set a max row limit instead of using terminal height.
         """
         return self.display_max_rows
     
     def set_display_max_rows(self, rows:int|None) -> None:
         """
-        Set ``display_max_rows`` to limit rows displayed when ``repr`` or ``print`` is called, or set to ``None`` for ``display_max_rows`` to be derived from current terminal height. Using this option will create a table that fits within the dimensions of the current terminal such that the table headers occupy the top-most row with the table caption occupying the lower-most.
-        Modifying this attribute does not change the actual number of rows stored in ``SQLDataModel``, only the number of rows displayed.
+        Sets value at :py:attr:`SQLDataModel.display_max_rows` to limit maximum rows displayed when ``repr`` or ``print`` is called. Use ``rows = None`` to derive max number to display from the current terminal height.
 
         Parameters:
             ``rows`` (int): The maximum number of rows to display.
 
         Raises:
             ``TypeError``: If the provided argument is not ``None`` or is not an integer.
             ``IndexError``: If the provided value is an integer less than or equal to 0.
@@ -1438,16 +1440,15 @@
             # Any call to ``print`` or ``repr`` will be restricted to 500 max rows
             sdm.set_display_max_rows(500)
 
             # Alternatively, auto-detect dimensions by setting to ``None``
             sdm.set_display_max_rows(None)
         
         Note:
-            - This does not affect the actual number of rows in the model, only the maximum **displayed**.
-
+            - Modifying :py:attr:`SQLDataModel.display_max_rows` does not affect the actual number of rows in the model, only the maximum rows **displayed**.
         """
         if not isinstance(rows, (int,type(None))):
             raise TypeError(
                 SQLDataModel.ErrorFormat(f'TypeError: invalid argument type "{type(rows).__name__}", please provide an integer value to set the maximum rows attribute...')
                 )
         if isinstance(rows, int) and rows <= 0:
             raise IndexError(
@@ -4335,25 +4336,26 @@
         """
         return ('sqlite3', 'psycopg2', 'pyodbc', 'cx_oracle', 'teradatasql')
    
 ################################################################################################################
 ############################################## conversion methods ##############################################
 ################################################################################################################
 
-    def data(self, index:bool=False, include_headers:bool=False) -> list[tuple]:
+    def data(self, index:bool=False, include_headers:bool=False, strict_2d:bool=False) -> list[tuple]:
         """
-        Returns the ``SQLDataModel`` data as a list of tuples for multiple rows or as a single tuple for individual rows. 
-        Data is returned without index and headers by default. Use ``include_headers=True`` or ``index=True`` to modify.
+        Returns the ``SQLDataModel`` data as a list of tuples for multiple rows, a single tuple for individual rows, as a single item for individual cells. 
+        Data is returned without index and headers by default, use ``include_headers=True`` or ``index=True`` to modify.
 
         Parameters:
             ``index`` (bool, optional): If True, includes the index in the result; if False, excludes the index. Default is False.
             ``include_headers`` (bool, optional): If True, includes column headers in the result; if False, excludes headers. Default is False.
+            ``strict_2d`` (bool, optional): If True, returns data as a 2-dimensional list of tuples regardless of data dimension. Default is False.
 
         Returns:
-            ``list``: The list of tuples representing the SQLDataModel data.
+            ``list[tuple]``: The data currently stored in the model as a list of tuples.
 
         Example::
 
             from SQLDataModel import SQLDataModel
 
             # Sample data
             headers = ['Name', 'Age', 'Height']
@@ -4388,15 +4390,15 @@
             # Grab data from single row
             row_data = sdm[0].data()
 
             # View it
             print(row_data)
         ```
 
-        This will output:
+        This will output the row as a tuple of values:
 
         ```text
             ('John', 30, 175.3)
         ```
 
         Get data for specific column:
 
@@ -4404,35 +4406,39 @@
             # Grab data from single column
             col_data = sdm['Name'].data()
             
             # View it
             print(col_data)
         ```
 
-        This will output:
+        This will output the column values as a list of tuples:
 
         ```text        
             [('John',), ('Alice',), ('Travis',)]
         ```
 
         Change Log:
             - Version 0.3.0 (2024-03-31):
                 - Renamed ``include_index`` parameter to ``index`` for package consistency.
+            
+            - Version 0.5.0 (2024-05-09):
+                - Added ``strict_2d`` parameter to allow predictable return type regardless of data dimension.
 
         Note:
             - Many other ``SQLDataModel`` methods rely on this method, changing it will lead to undefined behavior.
             - See related :meth:`SQLDataModel.from_data()` for creating a new ``SQLDataModel`` from existing data sources.
-
+            - Use ``strict_2d = True`` to always return data as a list of tuples regardless of data dimension.
         """
         res = self.sql_db_conn.execute(self._generate_sql_stmt(index=index))
         data = res.fetchall()
-        if (len(data) == 1) and (not include_headers): # if only single row
-            data = data[0]
-        if len(data) == 1: # if only single cell
-            data = data[0]
+        if not strict_2d:
+            if (len(data) == 1) and (not include_headers): # if only single row
+                data = data[0]
+                if len(data) == 1: # if only single cell
+                    data = data[0]
         return [tuple(x[0] for x in res.description),*data] if include_headers else data
 
     def to_csv(self, filename:str=None, delimiter:str=',', quotechar:str='"', lineterminator:str='\r\n', na_rep:str='None', index:bool=False, **kwargs) -> str|None:
         """
         Writes ``SQLDataModel`` to the specified file if ``filename`` argument if provided, otherwise returns the model directly as a CSV formatted string literal.
 
         Parameters:
@@ -5168,62 +5174,113 @@
             except Exception as e:
                 raise Exception(
                     SQLDataModel.ErrorFormat(f"{type(e).__name__}: {e} encountered when trying to open and write LaTeX")
                 ) from None
         else:
             return latex_repr 
 
-    def to_list(self, index:bool=True, include_headers:bool=False) -> list[tuple]:
+    def to_list(self, index:bool=False, include_headers:bool=False) -> list:
         """
-        Returns a list of tuples containing all the ``SQLDataModel`` data without the headers by default.
-        Use ``include_headers=True`` to return the headers as the first item in the returned sequence.
+        Returns the current ``SQLDataModel`` data as a 1-dimensional list of values if data dimensions are compatible with flattening, or as a list of lists if data is 2-dimensional.
+        Data is returned without index or headers by default, use ``index = True`` or ``include_headers = True`` to modify.
 
         Parameters:
-            ``index`` (bool, optional): If True, includes the index in the result, if False, excludes the index. Default is True.
+            ``index`` (bool, optional): If True, includes the index in the result, if False, excludes the index. Default is False.
             ``include_headers`` (bool, optional): If True, includes column headers in the result, if False, excludes headers. Default is False.
 
         Returns:
-            ``list``: The list of tuples representing the SQLDataModel data.
+            ``list``: The flattened list of values corresponding to the model data.
 
         Example::
             
             from SQLDataModel import SQLDataModel
 
-            # Output the data with indicies but without headers:
-            result_list = sdm.to_list(index=True, include_headers=False)
-
-            # Format of output:
-            output_list = [
-                (0, 'john', 'smith', 27)
-                ,(1, 'sarah', 'west', 29)
-                ,(2, 'patrick', 'mcdouglas', 42)
+            # Sample data
+            headers = ['Name', 'Age', 'Height']
+            data = [
+                ('Beth', 27, 172.4),
+                ('John', 30, 175.3), 
+                ('Alice', 28, 162.0), 
+                ('Travis', 35, 185.8)
             ]
 
-            # Output the data without indicies and with headers:
-            result_list = sdm.to_list(index=False, include_headers=True)
+            # Create the model
+            sdm = SQLDataModel(data, headers)    
+            
+            # Get all model data as a list of lists
+            model_data = sdm.to_list()
 
-            # View results
-            for row in result_list:
+            # Iterate over each row
+            for row in model_data:
                 print(row)
-        
+
         This will output:
 
         ```text
-            ('first', 'last', 'age')
-            ('john', 'smith', 27)
-            ('sarah', 'west', 29)
-            ('patrick', 'mcdouglas', 42)            
+            ['Beth', 27, 172.4]
+            ['John', 30, 175.3]
+            ['Alice', 28, 162.0]
+            ['Travis', 35, 185.8]
         ```
-        
+
+        Data will be flattened into a single dimension if possible, such as when accessing individual columns:
+
+        ```python
+            # Get 'Name' column as a list
+            col_data = sdm['Name'].to_list()
+
+            # View output
+            print(col_data)
+        ```
+
+        This will output a list containing the values from each row for the column:
+
+        ```text
+            ['Beth', 'John', 'Alice', 'Travis']
+        ```
+
+        Data will also be flattened when accessing individual rows:
+
+        ```python
+            # Get first row as a list with index
+            row_data = sdm[0].to_list(index=True)
+            
+            # View result
+            print(row_data)
+        ```
+
+        This will output the row's values including the index:
+
+        ```text
+            [0, 'Beth', 27, 172.4]
+        ```
+
         Change Log:
             - Version 0.3.0 (2024-03-31):
                 - Renamed ``include_index`` parameter to ``index`` for package consistency.
+            
+            - Version 0.5.0 (2024-05-09):
+                - Modified behavior to output 1-dimensional list when possible and a list of lists when not possible.
+                - Changed default to ``index = False`` to increase surface for 1-dimensional flattening.
+        
+        Note:
+            - See :meth:`SQLDataModel.data()` to return the equivalent of ``cursor.fetchall()`` with data as a list of tuples.
+            - See :meth:`SQLDataModel.iter_rows()` to generate an iterable over the model data, which is preferred wherever possible.
         """
         res = self.sql_db_conn.execute(self._generate_sql_stmt(index=index))
-        return [tuple([x[0] for x in res.description]),*res.fetchall()] if include_headers else res.fetchall()
+        data = res.fetchall()
+        if len(data) <= 1 and not include_headers:
+            return list(data[0])
+        else:
+            if len(data[0]) == 1:
+                data = list(row[0] for row in data)
+                return [res.description[0][0],*data] if include_headers else data
+            else:
+                data = [list(row) for row in data]
+                return [[x[0] for x in res.description],*data] if include_headers else data
     
     def to_markdown(self, filename:str=None, index:bool=False, min_column_width:int=None, max_column_width:int=None, float_precision:int=None, column_alignment:Literal['dynamic', 'left', 'center', 'right']=None) -> str|None:
         """
         Returns the current ``SQLDataModel`` as a markdown table literal if ``filename`` is None, otherwise writes the table to the provided file as markdown.
 
         Parameters:
             ``filename`` (str, optional): The name of the file to write the Markdown content. If not provided, the Markdown content is returned as a string. Default is None.
@@ -7454,17 +7511,21 @@
 
             # Retrieve a range of rows and all columns using a slice
             subset_model = sdm[2:7]
 
             # Retrieve a single column by name
             subset_model = sdm["first_name"]
         
+        Change Log:
+            - Version 0.5.0 (2024-05-09):
+                - Modified index retention behavior to pass through row indicies and avoid resetting view order.
+
         Note:
             - The ``slc`` parameter can be an integer, a tuple of disconnected row indices, a slice representing a range of rows, a string or list of strings representing column names, or a tuple combining row and column indices.
-            - The returned SQLDataModel instance will contain the specified subset of rows and columns.
+            - The returned SQLDataModel instance will contain the specified subset of rows and columns, retaining the row indicies of the original view.
         """         
         try:
             validated_rows, validated_columns = self.validate_indicies(target_indicies)
         except ValueError as e:
             raise ValueError(
                 SQLDataModel.ErrorFormat(f"{e}") # using existing formatting from validation
             ) from None
@@ -7472,15 +7533,15 @@
             raise TypeError(
                 SQLDataModel.ErrorFormat(f"{e}") # using existing formatting from validation
             ) from None
         except IndexError as e:
             raise IndexError(
                 SQLDataModel.ErrorFormat(f"{e}") # using existing formatting from validation
             ) from None 
-        sql_stmt_generated = self._generate_sql_stmt(rows=validated_rows,columns=validated_columns,index=False) # toggle to retain prior indicies after getitem slicing
+        sql_stmt_generated = self._generate_sql_stmt(rows=validated_rows,columns=validated_columns,index=True) # NOTE: toggle to retain prior indicies after getitem slicing, changed in version 0.5.0 to True
         return self.execute_fetch(sql_stmt_generated)
 
     def __setitem__(self, target_indicies, update_values) -> None:
         """
         Updates specified rows and columns in the SQLDataModel with the provided values.
 
         Parameters:
@@ -7849,24 +7910,18 @@
             raise ValueError(
                 SQLDataModel.ErrorFormat(f"ValueError: invalid value '{style}', argument for `style` must be one of 'ascii', 'bare', 'dash', 'default', 'double', 'list', 'markdown', 'outline', 'pandas', 'polars', 'postgresql' or 'round'")
             )
         self.table_style = style
 
     def __repr__(self) -> str:
         """
-        Returns a formatted string representation of the SQLDataModel instance.
+        Returns a pretty printed string representation of ``SQLDataModel`` formatted to the current terminal size.
 
         Returns:
-            ``str``: The string representation of the SQLDataModel instance with tabular formatting.
-
-        Formatting:
-            - Default alignment is right-aligned for numeric types and left-aligned for remaining types
-            - To override default and set custom alignment, use :meth:`SQLDataModel.set_column_alignment()` method
-            - Max displayed rows set to ``1000`` by default, use :meth:`SQLDataModel.set_display_max_rows()` to modify
-            - Set table color using :meth:`SQLDataModel.set_display_color()` method
+            ``str``: The string representation of the SQLDataModel instance output using display and format values set on instance.
 
         Example::
 
             from SQLDataModel import SQLDataModel
 
             # Sample data
             headers = ['idx', 'first', 'last', 'age']
@@ -7879,27 +7934,30 @@
 
             # Create the model
             sdm = SQLDataModel(data,headers)
 
             # Display the string representation
             print(sdm)
 
-        This will output:
+        This will output the default alignment, dynamically aligning columns based on their dtype, right-aligned for numeric, left otherwise:
 
         ```shell
             ┌───┬────────┬─────────┬────────┐
             │   │ first  │ last    │    age │
             ├───┼────────┼─────────┼────────┤
             │ 0 │ john   │ smith   │     27 │
             │ 1 │ sarah  │ west    │     29 │
             │ 2 │ mike   │ harlin  │     36 │
             │ 3 │ pat    │ douglas │     42 │
             └───┴────────┴─────────┴────────┘  
             [4 rows x 3 columns]      
         ```
+
+        Using ``'left'`` column alignment:
+
         ```python        
             # Using left alignment instead
             sdm.set_column_alignment("left")
 
             # See difference
             print(sdm)
         ```
@@ -7913,14 +7971,17 @@
             │ 0 │ john   │ smith   │ 27     │
             │ 1 │ sarah  │ west    │ 29     │
             │ 2 │ mike   │ harlin  │ 36     │
             │ 3 │ pat    │ douglas │ 42     │
             └───┴────────┴─────────┴────────┘
             [4 rows x 3 columns]
         ```
+        
+        Using ``'center'`` column alignment:
+
         ```python        
             # Using center alignment instead
             sdm.set_column_alignment("center")
 
             # See difference
             print(sdm)
         ```
@@ -7934,14 +7995,17 @@
             │ 0 │  john  │  smith  │   27   │
             │ 1 │ sarah  │  west   │   29   │
             │ 2 │  mike  │ harlin  │   36   │
             │ 3 │  pat   │ douglas │   42   │
             └───┴────────┴─────────┴────────┘
             [4 rows x 3 columns]
         ```
+
+        Using ``'right'`` column alignment:
+
         ```python        
             # Using right alignment instead
             sdm.set_column_alignment("right")
 
             # See difference
             print(sdm)
         ```
@@ -7957,18 +8021,19 @@
             │ 2 │   mike │  harlin │     36 │
             │ 3 │    pat │ douglas │     42 │
             └───┴────────┴─────────┴────────┘
             [4 rows x 3 columns]        
         ```
 
         Note:
-            - The representation includes a truncated table view of the SQLDataModel.
-            - The output adjusts column widths dynamically and provides ellipses if the table is truncated.
-            - The number of displayed rows is limited to either the row count or the specified maximum rows.
-            - The output includes column headers, row data, and information about the total number of rows and columns.
+            - Use :meth:`SQLDataModel.set_display_max_rows()` to explicitly set vertical height and modify vertical truncation behavior, which uses current terminal height by default.
+            - Use :meth:`SQLDataModel.set_min_column_width()` and :meth:`SQLDataModel.set_max_column_width()` to adjust column widths and modify horizontal truncation behavior.
+            - Use :meth:`SQLDataModel.set_column_alignment()` to modify column alignment, available options are dynamic alignment based on dtype, left, center or right alignment.
+            - Use :meth:`SQLDataModel.set_display_color()` to modify the table color, by default no color is applied with characters drawn using platform specific settings.
+            - Use :meth:`SQLDataModel.set_table_style()` to modify the table style format and box characters used to draw the table.
         """         
         table_format = self._generate_table_style()
         top_lh, top_hbar, top_sep, top_rh = table_format[0]
         mid_lh, mid_hbar, mid_sep, mid_rh = table_format[1]
         row_lh, row_sep, row_rh = table_format[2]
         low_lh, low_hbar, low_sep, low_rh = table_format[3]
         table_repr = """""" # big things...
@@ -7979,23 +8044,28 @@
         table_truncated_ellipses_width = len(table_truncated_ellipses) + 1 # added extra space after truncation mark before ellipses, looks better
         table_bare_newline = """\n"""
         total_available_width, total_available_height = shutil.get_terminal_size()
         display_max_rows = self.display_max_rows if self.display_max_rows is not None else (total_available_height - 6) if (total_available_height - 6 > 0) else 1
         vertical_truncation_required = display_max_rows < self.row_count
         max_display_rows = display_max_rows if vertical_truncation_required else self.row_count # max rows to display in repr
         split_row = max_display_rows // 2
-        check_width_top = 6 # resolves to 13 rows to ceck from, 7 off top 6 off bottom
-        check_width_bottom = (self.row_count-1) - check_width_top
+        if vertical_truncation_required:
+            check_width_top, check_width_bottom = self.indicies[split_row], self.indicies[-split_row]
+            check_width_top, check_width_bottom = (check_width_bottom, check_width_top) if check_width_top > check_width_bottom else (check_width_top, check_width_bottom)
+            check_width_scope = f'where ("{self.sql_idx}" < {check_width_top} or "{self.sql_idx}" >= {check_width_bottom})'
+        else:
+            check_width_scope = ''
         display_index = self.display_index
         column_alignment = None if self.column_alignment == 'dynamic' else '<' if self.column_alignment == 'left' else '^' if self.column_alignment == 'center' else '>' if self.column_alignment == 'right' else None
         display_headers = [self.sql_idx,*self.headers] if display_index else self.headers
         header_py_dtype_dict = {col:cmeta[1] for col, cmeta in self.header_master.items()}
         # header_printf_modifiers_dict = {col:(f"'% .{self.display_float_precision}f'" if dtype == 'float' else "'% d'" if dtype == 'int' else "'%!s'" if dtype != 'bytes' else "'b''%!s'''") for col,dtype in header_py_dtype_dict.items()}
         header_printf_modifiers_dict = {col:(f"'% .{self.display_float_precision}f'" if dtype == 'float' else "'%!s'" if dtype != 'bytes' else "'b''%!s'''") for col,dtype in header_py_dtype_dict.items()}
-        headers_sub_select = " ".join(("select",f"""max(length("{self.sql_idx}")) as "{self.sql_idx}",""" if display_index else "",",".join([f"""max(max(length(printf({header_printf_modifiers_dict[col]},"{col}"))),length('{col}')) as "{col}" """ for col in display_headers if col != self.sql_idx]),f'from "{self.sql_model}" where "{self.sql_idx}" in (select "{self.sql_idx}" from "{self.sql_model}" where ("{self.sql_idx}" <= {check_width_top} or "{self.sql_idx}" > {check_width_bottom}) order by "{self.sql_idx}" asc limit 13)'))
+        # headers_sub_select = " ".join(("select",f"""max(length("{self.sql_idx}")) as "{self.sql_idx}",""" if display_index else "",",".join([f"""max(max(length(printf({header_printf_modifiers_dict[col]},"{col}"))),length('{col}')) as "{col}" """ for col in display_headers if col != self.sql_idx]),f'from "{self.sql_model}" where "{self.sql_idx}" in (select "{self.sql_idx}" from "{self.sql_model}" where ("{self.sql_idx}" < {check_width_top} or "{self.sql_idx}" >= {check_width_bottom}) order by "{self.sql_idx}" asc limit {max_display_rows})'))
+        headers_sub_select = " ".join(("select",f"""max(length("{self.sql_idx}")) as "{self.sql_idx}",""" if display_index else "",",".join([f"""max(max(length(printf({header_printf_modifiers_dict[col]},"{col}"))),length('{col}')) as "{col}" """ for col in display_headers if col != self.sql_idx]),f'from "{self.sql_model}" where "{self.sql_idx}" in (select "{self.sql_idx}" from "{self.sql_model}" {check_width_scope} order by "{self.sql_idx}" asc limit {max_display_rows})'))
         headers_parse_lengths_select = " ".join(("select",",".join([f"""min(max(ifnull("{col}",length('{col}')),{self.min_column_width}),{self.max_column_width})""" if col != self.sql_idx else f"""ifnull("{col}",1)""" for col in display_headers]),"from"))
         headers_full_select = f"""{headers_parse_lengths_select}({headers_sub_select})"""
         length_meta = self.sql_db_conn.execute(headers_full_select).fetchone()
         header_length_dict = {display_headers[i]:width for i, width in enumerate(length_meta)}
         total_required_width = row_lh_width + sum((row_sep_width + length) for length in header_length_dict.values()) + row_rh_width - row_sep_width
         table_truncation_required = False if total_available_width > total_required_width else True
         # print(f'truncation info: {total_required_width} of {total_available_width}, truncation: {table_truncation_required}')
@@ -8052,14 +8122,15 @@
         table_repr = "".join([table_repr,*[row[0] for row in formatted_response]])
         # table_low_bar = "".join([low_lh, low_sep.join([low_hbar * header_length_dict[col] for col in display_headers]), low_rh, table_bare_newline])
         table_low_bar = "".join([low_lh, low_sep.join([low_hbar * length for length in col_lengths]), low_rh, table_bare_newline])
         table_low_bar = table_low_bar if len(table_low_bar.strip()) >=1 else """"""
         table_repr = "".join([table_repr, table_low_bar])
         table_caption = f"""[{self.row_count} rows x {self.column_count} columns]"""
         table_repr = "".join([table_repr, table_caption])
+        return table_repr if self.display_color is None else self.display_color.wrap(table_repr) 
         return table_repr if self.display_color is None else self.display_color.wrap(table_repr)
     
 ##################################################################################################################
 ############################################## sqldatamodel methods ##############################################
 ##################################################################################################################
 
     def concat(self, other:SQLDataModel|list|tuple, inplace:bool=True) -> None|SQLDataModel:
@@ -8691,15 +8762,15 @@
             )
         if not all(isinstance(sdm, SQLDataModel) for sdm in other):
             raise TypeError(
                 SQLDataModel.ErrorFormat(f"TypeError: invalid type encountered in '{[type(other[n]).__name__ for n in other]}', arguments for `other` must all be of type 'SQLDataModel' to horizontally stack")
             )
         other_headers, other_dtypes = zip(*[(col[0], col[1]) for sdm in other for col in sdm.dtypes.items()])
         other_headers, other_dtypes = list(SQLDataModel.alias_duplicates([*self.headers,*other_headers])), [*self.dtypes.values(), *other_dtypes]
-        other_data = [(sdm[:self.row_count].data() if sdm.row_count > 1 else [sdm[:self.row_count].data()]) + [tuple(None for _ in range(sdm.column_count)) for _ in range(self.row_count - sdm.row_count)] for sdm in other]
+        other_data = [(sdm[:self.row_count].data(strict_2d=True)) + [tuple(None for _ in range(sdm.column_count)) for _ in range(self.row_count - sdm.row_count)] for sdm in other]
         other_data = [tuple(item for sublist in row for item in sublist) for row in list(zip(*other_data))]
         if inplace:
             other_headers = other_headers[self.column_count:] # since in place remove current model's headers
             other_dtypes = other_dtypes[self.column_count:] # since in place remove current model's dtypes
             update_sql_script = ";".join([f"""alter table "{self.sql_model}" add column "{col_name}" {self.static_py_to_sql_map_dict.get(col_type, 'TEXT')}""" for col_name, col_type in zip(other_headers, other_dtypes)])
             col_val_param = ','.join([f""" "{col}" = {SQLDataModel.sqlite_cast_type_format(param='?', dtype=dtype)} """ for col,dtype in zip(other_headers, other_dtypes)])
             update_stmt = f"""update "{self.sql_model}" set {col_val_param} where {self.sql_idx} = ?"""
@@ -8712,15 +8783,15 @@
                 self.sql_db_conn.rollback()
                 raise SQLProgrammingError(
                     SQLDataModel.ErrorFormat(f"SQLProgrammingError: invalid update values, SQL execution failed with '{e}'")
                 ) from None
             self._update_model_metadata()
             return
         else:
-            other_data = [(t1 + t2) for t1, t2 in zip(self.data(index=False, include_headers=False), other_data)]
+            other_data = [(t1 + t2) for t1, t2 in zip(self.data(index=False, include_headers=False, strict_2d=True), other_data)]
             dtype_dict = dict(zip(other_headers, other_dtypes))
             return type(self)(data=other_data, headers=other_headers, dtypes=dtype_dict, **self._get_display_args())
 
     def iter_rows(self, min_row:int=None, max_row:int=None, index:bool=True, include_headers:bool=False) -> Generator:
         """
         Returns a generator object of the rows in the model from ``min_row`` to `max_row`.
 
@@ -9745,29 +9816,29 @@
             raise ValueError(
                 SQLDataModel.ErrorFormat(f"ValueError: insufficient model count '{len(other)}', at least 1 additional 'SQLDataModel' is required to vertically stack against")
             )
         if not all(isinstance(sdm, SQLDataModel) for sdm in other):
             raise TypeError(
                 SQLDataModel.ErrorFormat(f"TypeError: invalid type encountered in '{[type(other[n]).__name__ for n in other]}', arguments for `other` must all be of type 'SQLDataModel' to vertically stack")
             )
-        other_data = [[cell for cell in sublist] + [None] * (self.column_count - len(sublist)) for sublist in [item for sublist in [sdm[:,:self.column_count].data(index=False,include_headers=False) for sdm in other] for item in sublist]]
+        other_data = [[cell for cell in sublist] + [None] * (self.column_count - len(sublist)) for sublist in [item for sublist in [sdm[:,:self.column_count].data(index=False, include_headers=False, strict_2d=True) for sdm in other] for item in sublist]]
         if inplace:
             sql_insert_stmt = f"""insert into "{self.sql_model}" ({','.join([f'"{col}"' for col in self.headers])}) values ({",".join([SQLDataModel.sqlite_cast_type_format(dtype=self.header_master[col][1], as_binding=True) for col in self.headers])})"""
             try:
                 self.sql_db_conn.executemany(sql_insert_stmt, other_data)
                 self.sql_db_conn.commit()
             except sqlite3.ProgrammingError as e:
                 self.sql_db_conn.rollback()
                 raise SQLProgrammingError(
                     SQLDataModel.ErrorFormat(f"SQLProgrammingError: invalid update values, SQL execution failed with '{e}'")
                 ) from None            
             self._update_model_metadata(update_row_meta=True)
             return
         else:
-            other_data = (*self.data(index=False, include_headers=False),*other_data)
+            other_data = (*self.data(index=False, include_headers=False, strict_2d=True),*other_data)
             return type(self)(data=other_data, headers=self.headers, dtypes=self.dtypes, **self._get_display_args())
 
     def where(self, predicate:str) -> SQLDataModel:
         """
         Filters the rows of the current ``SQLDataModel`` object based on the specified SQL predicate and returns a
         new ``SQLDataModel`` containing only the rows that satisfy the condition. Only the predicates are needed as the statement prepends the select clause as "select [current model columns] where [`predicate`]", see below for detailed examples.
```

### Comparing `sqldatamodel-0.4.3/src/SQLDataModel/StandardDeviation.py` & `sqldatamodel-0.5.0/src/SQLDataModel/StandardDeviation.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.4.3/src/SQLDataModel/converters.py` & `sqldatamodel-0.5.0/src/SQLDataModel/converters.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.4.3/src/SQLDataModel/demo.py` & `sqldatamodel-0.5.0/src/SQLDataModel/demo.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.4.3/src/SQLDataModel/exceptions.py` & `sqldatamodel-0.5.0/src/SQLDataModel/exceptions.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.4.3/src/SQLDataModel/extensions/str_utils.c` & `sqldatamodel-0.5.0/src/SQLDataModel/extensions/str_utils.c`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.4.3/src/SQLDataModel.egg-info/PKG-INFO` & `sqldatamodel-0.5.0/src/SQLDataModel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLDataModel
-Version: 0.4.3
+Version: 0.5.0
 Summary: SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.
 Home-page: https://github.com/AnteT/SQLDataModel
 Author: Ante Tonkovic-Capin
 Author-email: antetc@icloud.com
 Project-URL: Documentation, https://sqldatamodel.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/AnteT/SQLDataModel.git
 Keywords: SQL,ETL,dataframe,terminal-tables,pretty-print-tables,sql2sql,data-analysis,data-science,datamodel,extract,transform,load,web-scraping-tables,data-mining,html,html-table-parsing,apache-arrow,pyarrow,pyarrow-conversion,pyarrow-to-table,pyarrow-to-sql,pyarrow-to-csv,parquet-file-parsing,csv,csv-parsing,markdown,markdown-table-parsing,latex,latex-table-parsing,delimited,delimited-data-parsing,file-conversion,format-conversion,terminal-styling,table-styling,from-sqlite,to-sqlite,from-postgresql,to-postgresql,sql-to-sql,excel,xlsx-file,excel-to-sql,DataFrames,polars2pandas,pandas2polars
```

### Comparing `sqldatamodel-0.4.3/src/SQLDataModel.egg-info/SOURCES.txt` & `sqldatamodel-0.5.0/src/SQLDataModel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.4.3/tests/test_Future.py` & `sqldatamodel-0.5.0/tests/test_Future.py`

 * *Files 2% similar despite different names*

```diff
@@ -677,15 +677,57 @@
     sdm_copy_full = sdm_original.copy(data_only=False)  
     assert sdm_original.data(index=True,include_headers=True) == sdm_copy_full.data(index=True,include_headers=True)
     assert sdm_original._get_display_args() == sdm_copy_full._get_display_args()
     # Test data only copy
     sdm_copy_data = sdm_original.copy(data_only=True)  
     assert sdm_original.data(index=True,include_headers=True) == sdm_copy_data.data(index=True,include_headers=True)
     assert sdm_original._get_display_args() != sdm_copy_data._get_display_args()
-    
+
+@pytest.mark.core    
+def test_head(sample_data):
+    n_value = 24
+    input_data, input_headers = sample_data[1:], sample_data[0]
+    sdm = SQLDataModel(input_data, headers=input_headers)
+    expected_output = input_data[:n_value]
+    output_data = sdm.head(n_rows=n_value).data()
+    assert output_data == expected_output
+
+@pytest.mark.core
+def test_tail(sample_data):
+    n_value = 24
+    input_data, input_headers = sample_data[1:], sample_data[0]
+    sdm = SQLDataModel(input_data, headers=input_headers)
+    expected_output = input_data[-n_value:]
+    output_data = sdm.tail(n_rows=n_value).data()
+    assert output_data == expected_output    
+
+@pytest.mark.core
+def test_to_list(sample_data):
+    input_data, input_headers = sample_data[1:], sample_data[0]
+    input_data = [list(row) for row in input_data]
+    sdm = SQLDataModel(input_data, input_headers)
+    ### all data: index=False, include_headers=False ###
+    output_data = sdm.to_list(include_headers=False, index=False)
+    assert output_data == input_data
+    ### all data: index=False, include_headers=True ###
+    output_data = sdm.to_list(include_headers=True, index=False)
+    output_headers, output_data = output_data[0], output_data[1:]
+    assert output_headers == input_headers
+    assert output_data == input_data
+    ### test each row ###
+    for rid, row in enumerate(input_data):
+        expected_output = [rid, *row]
+        output_data = sdm[rid].to_list(index=True) # IMPORTANT: __getitem__ must be set to retain row index for this to work
+        assert output_data == expected_output
+    ### test each column ###
+    for cid in range(len(input_headers)):
+        expected_output = [row[cid] for row in input_data]
+        output_data = sdm[:,cid].to_list(include_headers=False, index=False)
+        assert output_data == expected_output    
+
 @pytest.mark.core
 def test_merge():
     left_headers = ["Name", "Age", "ID"]
     left_data = [        
         ["Bob", 35, 1],
         ["Alice", 30, 5],
         ["David", 40, None],
```

### Comparing `sqldatamodel-0.4.3/tests/test_SQLDataModel.py` & `sqldatamodel-0.5.0/tests/test_SQLDataModel.py`

 * *Files 2% similar despite different names*

```diff
@@ -677,15 +677,57 @@
     sdm_copy_full = sdm_original.copy(data_only=False)  
     assert sdm_original.data(index=True,include_headers=True) == sdm_copy_full.data(index=True,include_headers=True)
     assert sdm_original._get_display_args() == sdm_copy_full._get_display_args()
     # Test data only copy
     sdm_copy_data = sdm_original.copy(data_only=True)  
     assert sdm_original.data(index=True,include_headers=True) == sdm_copy_data.data(index=True,include_headers=True)
     assert sdm_original._get_display_args() != sdm_copy_data._get_display_args()
-    
+
+@pytest.mark.core    
+def test_head(sample_data):
+    n_value = 24
+    input_data, input_headers = sample_data[1:], sample_data[0]
+    sdm = SQLDataModel(input_data, headers=input_headers)
+    expected_output = input_data[:n_value]
+    output_data = sdm.head(n_rows=n_value).data()
+    assert output_data == expected_output
+
+@pytest.mark.core
+def test_tail(sample_data):
+    n_value = 24
+    input_data, input_headers = sample_data[1:], sample_data[0]
+    sdm = SQLDataModel(input_data, headers=input_headers)
+    expected_output = input_data[-n_value:]
+    output_data = sdm.tail(n_rows=n_value).data()
+    assert output_data == expected_output    
+
+@pytest.mark.core
+def test_to_list(sample_data):
+    input_data, input_headers = sample_data[1:], sample_data[0]
+    input_data = [list(row) for row in input_data]
+    sdm = SQLDataModel(input_data, input_headers)
+    ### all data: index=False, include_headers=False ###
+    output_data = sdm.to_list(include_headers=False, index=False)
+    assert output_data == input_data
+    ### all data: index=False, include_headers=True ###
+    output_data = sdm.to_list(include_headers=True, index=False)
+    output_headers, output_data = output_data[0], output_data[1:]
+    assert output_headers == input_headers
+    assert output_data == input_data
+    ### test each row ###
+    for rid, row in enumerate(input_data):
+        expected_output = [rid, *row]
+        output_data = sdm[rid].to_list(index=True) # IMPORTANT: __getitem__ must be set to retain row index for this to work
+        assert output_data == expected_output
+    ### test each column ###
+    for cid in range(len(input_headers)):
+        expected_output = [row[cid] for row in input_data]
+        output_data = sdm[:,cid].to_list(include_headers=False, index=False)
+        assert output_data == expected_output    
+
 @pytest.mark.core
 def test_merge():
     left_headers = ["Name", "Age", "ID"]
     left_data = [        
         ["Bob", 35, 1],
         ["Alice", 30, 5],
         ["David", 40, None],
```

