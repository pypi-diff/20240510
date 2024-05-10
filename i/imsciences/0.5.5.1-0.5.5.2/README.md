# Comparing `tmp/imsciences-0.5.5.1.tar.gz` & `tmp/imsciences-0.5.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imsciences-0.5.5.1.tar", last modified: Fri May 10 09:36:43 2024, max compression
+gzip compressed data, was "imsciences-0.5.5.2.tar", last modified: Fri May 10 09:53:11 2024, max compression
```

## Comparing `imsciences-0.5.5.1.tar` & `imsciences-0.5.5.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 09:36:43.943484 imsciences-0.5.5.1/
--rw-rw-rw-   0        0        0     5465 2024-05-10 09:36:43.936963 imsciences-0.5.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     4962 2024-03-14 19:13:12.000000 imsciences-0.5.5.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 09:36:43.891540 imsciences-0.5.5.1/imsciences/
--rw-rw-rw-   0        0        0       41 2024-03-14 19:23:10.000000 imsciences-0.5.5.1/imsciences/__init__.py
--rw-rw-rw-   0        0        0    49415 2024-05-10 09:28:04.000000 imsciences-0.5.5.1/imsciences/datafunctions.py
-drwxrwxrwx   0        0        0        0 2024-05-10 09:36:43.932956 imsciences-0.5.5.1/imsciences.egg-info/
--rw-rw-rw-   0        0        0     5465 2024-05-10 09:36:43.000000 imsciences-0.5.5.1/imsciences.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2024-05-10 09:36:43.000000 imsciences-0.5.5.1/imsciences.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 09:36:43.000000 imsciences-0.5.5.1/imsciences.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-10 09:36:43.000000 imsciences-0.5.5.1/imsciences.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-10 09:36:43.000000 imsciences-0.5.5.1/imsciences.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 09:36:43.943484 imsciences-0.5.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1093 2024-05-10 09:36:34.000000 imsciences-0.5.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:53:11.489184 imsciences-0.5.5.2/
+-rw-rw-rw-   0        0        0     7464 2024-05-10 09:53:11.484198 imsciences-0.5.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6959 2024-05-10 09:52:39.000000 imsciences-0.5.5.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 09:53:11.456744 imsciences-0.5.5.2/imsciences/
+-rw-rw-rw-   0        0        0       41 2024-03-14 19:23:10.000000 imsciences-0.5.5.2/imsciences/__init__.py
+-rw-rw-rw-   0        0        0    49453 2024-05-10 09:53:01.000000 imsciences-0.5.5.2/imsciences/datafunctions.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:53:11.481507 imsciences-0.5.5.2/imsciences.egg-info/
+-rw-rw-rw-   0        0        0     7464 2024-05-10 09:53:11.000000 imsciences-0.5.5.2/imsciences.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-05-10 09:53:11.000000 imsciences-0.5.5.2/imsciences.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 09:53:11.000000 imsciences-0.5.5.2/imsciences.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-10 09:53:11.000000 imsciences-0.5.5.2/imsciences.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-10 09:53:11.000000 imsciences-0.5.5.2/imsciences.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 09:53:11.489184 imsciences-0.5.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     1093 2024-05-10 09:52:54.000000 imsciences-0.5.5.2/setup.py
```

### Comparing `imsciences-0.5.5.1/PKG-INFO` & `imsciences-0.5.5.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: imsciences
-Version: 0.5.5.1
-Summary: IMS Data Processing Package
-Author: IMS
-Author-email: cam@im-sciences.com
-Keywords: python,data processing
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-
 # IMS Package Documentation
 
 The IMS package is a python library for processing incoming data into a format that can be used for projects. IMS processing offers a variety of functions to manipulate and analyze data efficiently. Here are the functionalities provided by the package:
 
 ### 1. `get_wd_levels(levels)`
 - **Description**: Get the working directory with the option of moving up parents.
 - **Usage**: `get_wd_levels(levels)`
@@ -81,14 +66,34 @@
 - **Description**: Combines multiple DataFrames from a dictionary into a single DataFrame.
 - **Usage**: `combine_sheets({'Sheet1': df1, 'Sheet2': df2})`
 
 ### 17. `dynamic_pivot(data_frame, index_col, columns, values_col, fill_value=0)`
 - **Description**: Dynamically pivots a DataFrame based on specified columns.
 - **Usage**: `dynamic_pivot(df, 'Date', ['Category1', 'Category2'], ['Value1'])`
 
-### 18. `classify_within_column(df, col_name, to_find_dict, default_value = 'other')`
-- **Description**: Allows you to map a dictionary of substrings within a column.
-- **Usage**: `classify_within_column(df, 'campaign', {'uk_': 'uk'}, 'other')`
+### 18. `apply_lookup_table_for_columns(df, col_names, to_find_dict, if_not_in_country_dict='Other'), new_column_name='Mapping')`
+- **Description**: Equivalent of xlookup in excel. Allows you to map a dictionary of substrings within a column. If multiple columns are need for the LUT then a | seperator is needed.
+- **Usage**: `classify_within_column(df, ['campaign type','media type'], {'France Paid Social FB|paid social': 'facebook','France Paid Social TW|paid social': 'twitter'}, 'other','mapping')`
 
 ### 19. `aggregate_daily_to_wc_wide(df, date_column, group_columns, sum_columns, wc, aggregation='sum', include_totals=False)`
 - **Description**: Aggregates daily data into weekly data, grouping and summing specified columns, starting on a specified day of the week. In the wide format.
 - **Usage**: `aggregate_daily_to_wc_wide(df, date_column, group_columns, sum_columns, wc, aggregation='sum', include_totals=False)`
+
+### 20. `merge_cols_with_seperator(df, col_names,output_column_name = 'Merged')`
+- **Description**: Merge multiple columns in a dataframe into 1 column with a seperator '|'.Can be used if multiple columns are needed for a LUT.
+- **Usage**: `merge_cols_with_seperator(df, ['Campaign','Product'],'Merged Columns')`
+
+### 21. `check_sum_of_df_cols_are_equal(df_1,df_2,cols_1,cols_2)`
+- **Description**: Checks if the sum of two columns in two dataframes are the same, and provides the sums of each column and the difference between them.
+- **Usage**: `check_sum_of_df_cols_are_equal(df_1,df_2,'Media Cost','Spend')`
+
+### 22. `convert_2_df_cols_to_dict(df, key_col, value_col)`
+- **Description**: Can be used to create an LUT. Creates a dictionary using two columns in a dataframe.
+- **Usage**: `convert_2_df_cols_to_dict(df, 'Campaign', 'Channel')`
+
+### 23. `create_FY_and_H_columns(df, index_col, start_date, starting_FY,short_format='No',half_years='No',combined_FY_and_H='No')`
+- **Description**: Used to create a financial year, half year, and financial half year column.
+- **Usage**: `create_FY_and_H_columns(df, 'Week (M-S)', '2022-10-03', 'FY2023',short_format='Yes',half_years='Yes',combined_FY_and_H='Yes')`
+
+### 24. `keyword_lookup_replacement(df, col, replacement_rows, cols_to_merge, replacement_lookup_dict,output_column_name='Updated Column')`
+- **Description**: Essentially provides an if statement with a xlookup if a value is something. Updates certain chosen values in a specified column of the DataFrame based on a lookup dictionary.
+- **Usage**: `keyword_lookup_replacement(df, 'channel', 'Paid Search Generic', ['channel','segment','product'], qlik_dict_for_channel,output_column_name='Channel New')`
```

### Comparing `imsciences-0.5.5.1/imsciences/datafunctions.py` & `imsciences-0.5.5.2/imsciences/datafunctions.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,40 +97,40 @@
         
         print("\n17. dynamic_pivot")
         print("    - Description: Dynamically pivots a DataFrame based on specified columns.")
         print("    - Usage: dynamic_pivot(data_frame, index_col, columns, values_col, fill_value=0)")
         print("    - Example: dynamic_pivot(df, 'Date', ['Category1', 'Category2'], ['Value1'])")
         
         print("\n18. apply_lookup_table_for_columns")
-        print("    - Description: Equivalent of xlookup in excel. Allows you to map a dictionary of substrings within a column.If multiple columns are need for the LUT then a | seperator is needed")
+        print("    - Description: Equivalent of xlookup in excel. Allows you to map a dictionary of substrings within a column. If multiple columns are need for the LUT then a | seperator is needed.")
         print("    - Usage: classify_within_column(df, col_names, to_find_dict, if_not_in_country_dict='Other'), new_column_name='Mapping'")
         print("    - Example: classify_within_column(df, ['campaign type','media type'], {'France Paid Social FB|paid social': 'facebook','France Paid Social TW|paid social': 'twitter'}, 'other','mapping')")
 
         print("\n19. aggregate_daily_to_wc_wide")
         print("   - Description: Aggregates daily data into weekly data, grouping and summing specified columns, starting on a specified day of the week.")
         print("   - Usage: aggregate_daily_to_wc_wide(df, date_column, group_columns, sum_columns, wc, aggregation='sum', include_totals=False)")
         print("   - Example: aggregate_daily_to_wc_wide(df, 'date', ['platform'], ['cost', 'impressions', 'clicks'], 'mon', 'average', True)")
 
         print("\n20. merge_cols_with_seperator")
-        print("   - Description: Merged multiples columns in a dataframe into 1 with a seperator '|'.Can be used if multiple columns are needed for a LUT")
+        print("   - Description: Merge multiple columns in a dataframe into 1 column with a seperator '|'.Can be used if multiple columns are needed for a LUT.")
         print("   - Usage: merge_cols_with_seperator(df, col_names,output_column_name = 'Merged')")
         print("   - Example: merge_cols_with_seperator(df, ['Campaign','Product'],'Merged Columns')")        
 
         print("\n21. check_sum_of_df_cols_are_equal")
-        print("   - Description: Checks if the sum of two columns in two dataframes are the same, and provides the sums of each column")
+        print("   - Description: Checks if the sum of two columns in two dataframes are the same, and provides the sums of each column and the difference between them.")
         print("   - Usage: check_sum_of_df_cols_are_equal(df_1,df_2,cols_1,cols_2)")
-        print("   - Example: check_sum_of_df_cols_are_equal(df_1,df_2,['Media Cost'],['Spend'])")        
+        print("   - Example: check_sum_of_df_cols_are_equal(df_1,df_2,'Media Cost','Spend')")        
 
         print("\n22. convert_2_df_cols_to_dict")
         print("   - Description: Can be used to create an LUT. Creates a dictionary using two columns in a dataframe.")
         print("   - Usage: convert_2_df_cols_to_dict(df, key_col, value_col)")
         print("   - Example: convert_2_df_cols_to_dict(df, 'Campaign', 'Channel')")        
 
         print("\n23. create_FY_and_H_columns")
-        print("   - Description: Used to create a financial year, half year, and financial half year column")
+        print("   - Description: Used to create a financial year, half year, and financial half year column.")
         print("   - Usage: create_FY_and_H_columns(df, index_col, start_date, starting_FY,short_format='No',half_years='No',combined_FY_and_H='No')")
         print("   - Example: create_FY_and_H_columns(df, 'Week (M-S)', '2022-10-03', 'FY2023',short_format='Yes',half_years='Yes',combined_FY_and_H='Yes')")        
         
         print("\n24. keyword_lookup_replacement")
         print("   - Description: Essentially provides an if statement with a xlookup if a value is something. Updates certain chosen values in a specified column of the DataFrame based on a lookup dictionary.")
         print("   - Usage: keyword_lookup_replacement(df, col, replacement_rows, cols_to_merge, replacement_lookup_dict,output_column_name='Updated Column')")
         print("   - Example: keyword_lookup_replacement(df, 'channel', 'Paid Search Generic', ['channel','segment','product'], qlik_dict_for_channel,output_column_name='Channel New')")
```

### Comparing `imsciences-0.5.5.1/setup.py` & `imsciences-0.5.5.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Function to read the contents of the README file
 def read_md(file_name):
     if os.path.isfile(file_name):
         with open(file_name, 'r', encoding='utf-8') as f:
             return f.read()
     return ''
 
-VERSION = '0.5.5.1'
+VERSION = '0.5.5.2'
 DESCRIPTION = 'IMS Data Processing Package'
 LONG_DESCRIPTION = read_md('README.md')  # Reading from README.md
 
 # Setting up
 setup(
     name="imsciences",
     version=VERSION,
```

