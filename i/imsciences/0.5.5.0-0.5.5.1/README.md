# Comparing `tmp/imsciences-0.5.5.0.tar.gz` & `tmp/imsciences-0.5.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imsciences-0.5.5.0.tar", last modified: Wed May  1 10:23:53 2024, max compression
+gzip compressed data, was "imsciences-0.5.5.1.tar", last modified: Fri May 10 09:36:43 2024, max compression
```

## Comparing `imsciences-0.5.5.0.tar` & `imsciences-0.5.5.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 10:23:53.674617 imsciences-0.5.5.0/
--rw-rw-rw-   0        0        0     5465 2024-05-01 10:23:53.671407 imsciences-0.5.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     4962 2024-03-14 19:13:12.000000 imsciences-0.5.5.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 10:23:53.637571 imsciences-0.5.5.0/imsciences/
--rw-rw-rw-   0        0        0       41 2024-03-14 19:23:10.000000 imsciences-0.5.5.0/imsciences/__init__.py
--rw-rw-rw-   0        0        0    33182 2024-05-01 09:40:46.000000 imsciences-0.5.5.0/imsciences/datafunctions.py
-drwxrwxrwx   0        0        0        0 2024-05-01 10:23:53.666425 imsciences-0.5.5.0/imsciences.egg-info/
--rw-rw-rw-   0        0        0     5465 2024-05-01 10:23:53.000000 imsciences-0.5.5.0/imsciences.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2024-05-01 10:23:53.000000 imsciences-0.5.5.0/imsciences.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 10:23:53.000000 imsciences-0.5.5.0/imsciences.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-01 10:23:53.000000 imsciences-0.5.5.0/imsciences.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-01 10:23:53.000000 imsciences-0.5.5.0/imsciences.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 10:23:53.674617 imsciences-0.5.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1093 2024-05-01 10:23:21.000000 imsciences-0.5.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:36:43.943484 imsciences-0.5.5.1/
+-rw-rw-rw-   0        0        0     5465 2024-05-10 09:36:43.936963 imsciences-0.5.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4962 2024-03-14 19:13:12.000000 imsciences-0.5.5.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 09:36:43.891540 imsciences-0.5.5.1/imsciences/
+-rw-rw-rw-   0        0        0       41 2024-03-14 19:23:10.000000 imsciences-0.5.5.1/imsciences/__init__.py
+-rw-rw-rw-   0        0        0    49415 2024-05-10 09:28:04.000000 imsciences-0.5.5.1/imsciences/datafunctions.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:36:43.932956 imsciences-0.5.5.1/imsciences.egg-info/
+-rw-rw-rw-   0        0        0     5465 2024-05-10 09:36:43.000000 imsciences-0.5.5.1/imsciences.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-05-10 09:36:43.000000 imsciences-0.5.5.1/imsciences.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 09:36:43.000000 imsciences-0.5.5.1/imsciences.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-10 09:36:43.000000 imsciences-0.5.5.1/imsciences.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-10 09:36:43.000000 imsciences-0.5.5.1/imsciences.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 09:36:43.943484 imsciences-0.5.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1093 2024-05-10 09:36:34.000000 imsciences-0.5.5.1/setup.py
```

### Comparing `imsciences-0.5.5.0/PKG-INFO` & `imsciences-0.5.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsciences
-Version: 0.5.5.0
+Version: 0.5.5.1
 Summary: IMS Data Processing Package
 Author: IMS
 Author-email: cam@im-sciences.com
 Keywords: python,data processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `imsciences-0.5.5.0/README.md` & `imsciences-0.5.5.1/README.md`

 * *Files identical despite different names*

### Comparing `imsciences-0.5.5.0/imsciences/datafunctions.py` & `imsciences-0.5.5.1/imsciences/datafunctions.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import pandas as pd
 import calendar
 import os
 import plotly.express as px
 import plotly.graph_objs as go
 from dateutil.parser import parse
 import numpy as np
+from datetime import datetime
+import datetime
+from datetime import datetime, timedelta
 
 class dataprocessing:
     
     def help(self):
         print("This is the help section. The functions in the package are as follows:")
 
         print("\n1. get_wd_levels")
@@ -93,24 +96,50 @@
         print("    - Example: combine_sheets({'Sheet1': df1, 'Sheet2': df2})")
         
         print("\n17. dynamic_pivot")
         print("    - Description: Dynamically pivots a DataFrame based on specified columns.")
         print("    - Usage: dynamic_pivot(data_frame, index_col, columns, values_col, fill_value=0)")
         print("    - Example: dynamic_pivot(df, 'Date', ['Category1', 'Category2'], ['Value1'])")
         
-        print("\n18. classify_within_column")
-        print("    - Description: Allows you to map a dictionary of substrings within a column.")
-        print("    - Usage: classify_within_column(df, col_name, to_find_dict, if_not_in_country_dict='Other')")
-        print("    - Example: classify_within_column(df, 'campaign', {'uk_': 'uk'}, 'other')")
+        print("\n18. apply_lookup_table_for_columns")
+        print("    - Description: Equivalent of xlookup in excel. Allows you to map a dictionary of substrings within a column.If multiple columns are need for the LUT then a | seperator is needed")
+        print("    - Usage: classify_within_column(df, col_names, to_find_dict, if_not_in_country_dict='Other'), new_column_name='Mapping'")
+        print("    - Example: classify_within_column(df, ['campaign type','media type'], {'France Paid Social FB|paid social': 'facebook','France Paid Social TW|paid social': 'twitter'}, 'other','mapping')")
 
         print("\n19. aggregate_daily_to_wc_wide")
         print("   - Description: Aggregates daily data into weekly data, grouping and summing specified columns, starting on a specified day of the week.")
         print("   - Usage: aggregate_daily_to_wc_wide(df, date_column, group_columns, sum_columns, wc, aggregation='sum', include_totals=False)")
         print("   - Example: aggregate_daily_to_wc_wide(df, 'date', ['platform'], ['cost', 'impressions', 'clicks'], 'mon', 'average', True)")
 
+        print("\n20. merge_cols_with_seperator")
+        print("   - Description: Merged multiples columns in a dataframe into 1 with a seperator '|'.Can be used if multiple columns are needed for a LUT")
+        print("   - Usage: merge_cols_with_seperator(df, col_names,output_column_name = 'Merged')")
+        print("   - Example: merge_cols_with_seperator(df, ['Campaign','Product'],'Merged Columns')")        
+
+        print("\n21. check_sum_of_df_cols_are_equal")
+        print("   - Description: Checks if the sum of two columns in two dataframes are the same, and provides the sums of each column")
+        print("   - Usage: check_sum_of_df_cols_are_equal(df_1,df_2,cols_1,cols_2)")
+        print("   - Example: check_sum_of_df_cols_are_equal(df_1,df_2,['Media Cost'],['Spend'])")        
+
+        print("\n22. convert_2_df_cols_to_dict")
+        print("   - Description: Can be used to create an LUT. Creates a dictionary using two columns in a dataframe.")
+        print("   - Usage: convert_2_df_cols_to_dict(df, key_col, value_col)")
+        print("   - Example: convert_2_df_cols_to_dict(df, 'Campaign', 'Channel')")        
+
+        print("\n23. create_FY_and_H_columns")
+        print("   - Description: Used to create a financial year, half year, and financial half year column")
+        print("   - Usage: create_FY_and_H_columns(df, index_col, start_date, starting_FY,short_format='No',half_years='No',combined_FY_and_H='No')")
+        print("   - Example: create_FY_and_H_columns(df, 'Week (M-S)', '2022-10-03', 'FY2023',short_format='Yes',half_years='Yes',combined_FY_and_H='Yes')")        
+        
+        print("\n24. keyword_lookup_replacement")
+        print("   - Description: Essentially provides an if statement with a xlookup if a value is something. Updates certain chosen values in a specified column of the DataFrame based on a lookup dictionary.")
+        print("   - Usage: keyword_lookup_replacement(df, col, replacement_rows, cols_to_merge, replacement_lookup_dict,output_column_name='Updated Column')")
+        print("   - Example: keyword_lookup_replacement(df, 'channel', 'Paid Search Generic', ['channel','segment','product'], qlik_dict_for_channel,output_column_name='Channel New')")        
+
+
     def get_wd_levels(self, levels):
         """
         Gets the current wd of whoever is working on it and gives the options to move the number of levels up.
 
         Parameters:
         - data_frame: pandas DataFrame
             The input data frame.
@@ -134,15 +163,15 @@
         Parameters:
         - data_frame: pandas DataFrame
             The input data frame.
         - num_rows_to_remove: int
             The number of rows to remove from the data frame, starting from the original header.
 
         Returns:
-        - pandas DataFrame
+        - pandas DataFrames
             The modified data frame with rows removed and new column headings.
 
         Raises:
         - TypeError: If num_rows_to_remove is not an integer.
         - ValueError: If num_rows_to_remove is negative or exceeds the total number of rows.
         """
         
@@ -220,79 +249,14 @@
             grouped = df_copy.groupby(['week_start'] + group_columns)[sum_columns].sum().reset_index()
 
         # Rename 'week_start' column to 'OBS'
         grouped = grouped.rename(columns={'week_start': 'OBS'})
 
         return grouped
     
-    def aggregate_daily_to_wc_wide(self, df : pd.DataFrame, date_column : str, group_columns : list[str], sum_columns : list[str], wc : str = 'sun', aggregation : str = 'sum', include_totals : bool = False) -> pd.DataFrame:
-        """
-        Aggregates daily data into weekly data, starting on a specified day of the week, 
-        and groups the data by additional specified columns. It aggregates specified numeric columns 
-        by summing, averaging, or counting them, and pivots the data to create separate columns for each combination 
-        of the group columns and sum columns. NaN values are replaced with 0 and the index is reset. 
-        The day column is renamed from 'Day' to 'OBS'.
-
-        Parameters:
-        - df: pandas DataFrame
-            The input DataFrame containing daily data.
-        - date_column: string
-            The name of the column in the DataFrame that contains date information.
-        - group_columns: list of strings
-            Additional column names to group by along with the weekly grouping.
-        - sum_columns: list of strings
-            Numeric column names to be aggregated during aggregation.
-        - wc: string
-            The week commencing day (e.g., 'sun' for Sunday, 'mon' for Monday).
-        - aggregation: string, optional (default 'sum')
-            Aggregation method, either 'sum', 'average', or 'count'.
-        - include_totals: boolean, optional (default False)
-            If True, include total columns for each sum_column.
-
-
-
-        Returns:
-        - pandas DataFrame
-            A new DataFrame with weekly aggregated data. The index is reset,
-            and columns represent the grouped and aggregated metrics. The DataFrame 
-            is in wide format, with separate columns for each combination of 
-            grouped metrics.
-        """
-        
-        grouped = self.aggregate_daily_to_wc_long(df, date_column, group_columns, sum_columns, wc, aggregation)
-        
-        # Pivot the data to wide format
-        if group_columns:
-            wide_df = grouped.pivot_table(index='OBS', 
-                                        columns=group_columns, 
-                                        values=sum_columns,
-                                        aggfunc='first')
-            # Flatten the multi-level column index and create combined column names
-            wide_df.columns = ['_'.join(col).strip() for col in wide_df.columns.values]
-        else:
-            wide_df = grouped.set_index('OBS')
-
-        # Fill NaN values with 0
-        wide_df = wide_df.fillna(0)
-
-        # Adding total columns for each unique sum_column, if include_totals is True
-        if include_totals:
-            for col in sum_columns:
-                total_column_name = f'Total {col}'
-                if group_columns:
-                    columns_to_sum = [column for column in wide_df.columns if col in column]
-                else:
-                    columns_to_sum = [col]
-                wide_df[total_column_name] = wide_df[columns_to_sum].sum(axis=1)
-
-        # Reset the index of the final DataFrame
-        wide_df = wide_df.reset_index()
-
-        return wide_df
-    
     def convert_monthly_to_daily(self, df, date_column, divide = True):
         """
         Convert a DataFrame with monthly data to daily data.
         This function takes a DataFrame and a date column, then it expands each
         monthly record into daily records by dividing the numeric values by the number of days in that month.
 
         :param df: DataFrame with monthly data.
@@ -647,33 +611,364 @@
         # Convert OBS back to a string in YYYY-MM-DD format for display purposes
         pivoted_df[index_col] = pivoted_df[index_col].dt.strftime('%Y-%m-%d')
         
         # Fill in any NaNs
         pivoted_df = pivoted_df.fillna(fill_value)
         
         return pivoted_df
-    
-    def classify_within_column(self, df, col_name, to_find_dict, if_not_in_country_dict="Other"):
+
+    def apply_lookup_table_for_columns(self, df, col_names, to_find_dict, if_not_in_dict="Other", new_column_name="Mapping"):
         """
-        Classify entries in a DataFrame column based on a dictionary of substrings to class mappings.
-        
+        Creates a new DataFrame column based on a look up table, possibly with multiple columns to look up on (dictionary of substrings to class mappings).
+
         Parameters:
-        - df: pandas.DataFrame to operate on.
-        - col_name: String, name of the column to classify.
-        - to_find_dict: Dictionary, where keys are substrings to find and values are the corresponding classifications.
-        - if_not_in_country_dict: String, default classification if no substring matches are found.
-        
+        df (pandas.DataFrame): The DataFrame containing the data.
+        col_names (list of str): these are the columns which are used for the lookup. One column or several columns can be inputted as a list, provided there is a merged column to lookup on. If there are multiple columns to look up on then a merged column must be inputted as the key of the dictionary of format e.g. col1|col2|col3
+        to_find_dict (dict): your look up table, where keys are the values being looked up, and the values are the resulting mappings. 
+        if_not_in_dict (str, optional): default value if no substring matches are found in the look up table dictionary. Defaults to "Other".
+        new_column_name (str, optional): name of new column. Defaults to "Mapping".
+
         Returns:
-        - DataFrame with a new column '<col_name>_mapping' containing the classification results.
+        pandas.DataFrame: DataFrame with a new column containing the look up table results.
         """
+        
         # Define the inner function for classification
-        def find_word_in_string(x_string, to_find_dict=to_find_dict, default_value=if_not_in_country_dict):
+        def find_word_in_string(x_string, to_find_dict=to_find_dict, default_value=if_not_in_dict):
             x_string_lower = x_string.lower()
             for key, value in to_find_dict.items():
                 if key.lower() in x_string_lower:
                     return value
             return default_value
 
-        # Apply the inner function to the specified column and create a new column with the results
-        df[col_name + '_mapping'] = df[col_name].apply(find_word_in_string)
+        # Check if there is multiple columns to look up on
+        if len(col_names) == 1:
+
+            # Create copy of df to avoid SettingWithCopyWarning warning
+            df_2 = df.copy()
+            
+            try:
+                # Apply the inner function to the specified column and create a new column with the results
+                df_2[new_column_name] = df_2.loc[:,''.join(col_names)].apply(find_word_in_string)
+                
+            # Raise an error if list has not been inputted for column names
+            except TypeError:
+                print("Error: Column Names even if only one must be specified as a list, so must be inputted as e.g." + str(["Product"]) + ". to_find_dict must be specified as dictionary")
+                
+            
+        # Check if there is multiple columns to look up on
+        if len(col_names) > 1:
+            
+            # Create copy of df to avoid SettingWithCopyWarning warning
+            df_2 = df.copy()
+            
+            try:
+                # Apply a lambda function to join the chosen columns togther with a seperator
+                df_2["Merged"] = df_2.loc[:,col_names].apply(lambda row: '|'.join(row.values.astype(str)), axis=1)
+            
+            except TypeError:
+                print("Error: Column Names even if only one must be specified as a list, so must be inputted as e.g." + str(["Product"]) + ". to_find_dict must be specified as dictionary")
+            
+            # Apply the inner function to the specified column and create a new column with the results
+            df_2[new_column_name] = df_2.loc[:,"Merged"].apply(find_word_in_string)
+            
+        return df_2
+
+    def aggregate_daily_to_wc_wide(self, df : pd.DataFrame, date_column : str, group_columns : list[str], sum_columns : list[str], wc : str = 'sun', aggregation : str = 'sum', include_totals : bool = False) -> pd.DataFrame:
+        """
+        Aggregates daily data into weekly data, starting on a specified day of the week, 
+        and groups the data by additional specified columns. It aggregates specified numeric columns 
+        by summing, averaging, or counting them, and pivots the data to create separate columns for each combination 
+        of the group columns and sum columns. NaN values are replaced with 0 and the index is reset. 
+        The day column is renamed from 'Day' to 'OBS'.
+
+        Parameters:
+        - df: pandas DataFrame
+            The input DataFrame containing daily data.
+        - date_column: string
+            The name of the column in the DataFrame that contains date information.
+        - group_columns: list of strings
+            Additional column names to group by along with the weekly grouping.
+        - sum_columns: list of strings
+            Numeric column names to be aggregated during aggregation.
+        - wc: string
+            The week commencing day (e.g., 'sun' for Sunday, 'mon' for Monday).
+        - aggregation: string, optional (default 'sum')
+            Aggregation method, either 'sum', 'average', or 'count'.
+        - include_totals: boolean, optional (default False)
+            If True, include total columns for each sum_column.
+
+
+
+        Returns:
+        - pandas DataFrame
+            A new DataFrame with weekly aggregated data. The index is reset,
+            and columns represent the grouped and aggregated metrics. The DataFrame 
+            is in wide format, with separate columns for each combination of 
+            grouped metrics.
+        """
+        
+        grouped = self.aggregate_daily_to_wc_long(df, date_column, group_columns, sum_columns, wc, aggregation)
+        
+        # Pivot the data to wide format
+        if group_columns:
+            wide_df = grouped.pivot_table(index='OBS', 
+                                        columns=group_columns, 
+                                        values=sum_columns,
+                                        aggfunc='first')
+            # Flatten the multi-level column index and create combined column names
+            wide_df.columns = ['_'.join(col).strip() for col in wide_df.columns.values]
+        else:
+            wide_df = grouped.set_index('OBS')
+
+        # Fill NaN values with 0
+        wide_df = wide_df.fillna(0)
+
+        # Adding total columns for each unique sum_column, if include_totals is True
+        if include_totals:
+            for col in sum_columns:
+                total_column_name = f'Total {col}'
+                if group_columns:
+                    columns_to_sum = [column for column in wide_df.columns if col in column]
+                else:
+                    columns_to_sum = [col]
+                wide_df[total_column_name] = wide_df[columns_to_sum].sum(axis=1)
+
+        # Reset the index of the final DataFrame
+        wide_df = wide_df.reset_index()
+
+        return wide_df
+
+    def merge_cols_with_seperator(self, df, col_names,output_column_name = "Merged"):
+        """
+        Creates a new column in the dataframe that merges 2 or more columns together with a "|" seperator, possibly to be used for a look up table where multiple columns are being looked up
+
+        Parameters:
+        df (pandas.DataFrame): Dataframe to make changes to.
+        col_names (list): list of columm names ot merge.
+        output_column_name (str, optional): Name of column outputted. Defaults to "Merged".
+
+        Raises:
+        ValueError: if more less than two column names are inputted in the list there is nothing to merge on
+
+        Returns:
+        pandas.DataFrame: DataFrame with additional merged column
+        """
+        # Specify more than one column must be entered
+        if len(col_names) < 2:
+            raise ValueError("2 or more columns must be specified to merge")
+        
+        # Create a new column with the merged columns
+        df[output_column_name] = "|".join(df[col_names])
+
+        return df
+
+    def check_sum_of_df_cols_are_equal(self, df_1,df_2,cols_1,cols_2):
+        """
+        Checks the sum of two different dataframe column or columns are equal
+
+        Parameters:
+        df_1 (pandas.DataFrame): First dataframe for columnsa to be summed on.
+        df_2 (pandas.DataFrame): Second dataframe for columnsa to be summed on.
+        cols_1 (list of str): Columns from first dataframe to sum.
+        cols_2 (list of str): Columns from second dataframe to sum.
+
+        Returns:
+        Tuple: Answer is the true or false answer to whether sums are the same, df_1_sum is the sum of the column/columns in the first dataframe, df_2_sum is the sum of the column/columns in the second dataframe
+        """
+        # Find the sum of both sets of columns
+        df_1_sum = df_1[cols_1].sum().sum()
+        df_2_sum = df_2[cols_2].sum().sum()
+        
+        # If the the two columns are 
+        if df_1_sum == df_2_sum:
+            Answer = "They are equal"
+        if df_1_sum != df_2_sum:
+            Answer = "They are different by " + str(df_2_sum-df_1_sum)     
+            
+        return Answer,df_1_sum,df_2_sum
+    
+    def convert_2_df_cols_to_dict(self, df, key_col, value_col):
+        """
+        Create a dictionary mapping from two columns of a DataFrame.
+
+        Parameters:
+        df (pd.DataFrame): The DataFrame containing the data.
+        key_col (str): The column name to use as keys in the dictionary.
+        value_col (str): The column name to use as values in the dictionary.
+
+        Returns:
+        dict: A dictionary with keys from 'key_col' and values from 'value_col'.
+        """
+        if key_col not in df or value_col not in df:
+            raise ValueError("Specified columns are not in the DataFrame")
+
+        return {df[key_col].iloc[i]: df[value_col].iloc[i] for i in range(len(df))}
+    
+    def create_FY_and_H_columns(self, df, index_col, start_date, starting_FY,short_format="No",half_years="No",combined_FY_and_H="No"):
+        """
+        Creates new DataFrame columns containing companies' Financial Year, Half Years and Financial Half years, based on the start date of the first full financial year 
+
+        Parameters:
+        df (pandas.DataFrame): Dataframe to operate on.
+        index_col (str): Name of the column to use for datetime
+        start_date (str): String used to specify the start date of an FY specified, needs to be of format "yyyy-mm-dd" e.g. 2021-11-31
+        starting_FY (str): String used to specify which FY the start date refers to, needs to be formatted LONG e.g. FY2021
+        short_format (str, optional): String used to specify if short format is desired (e.g. FY21) or if long format is desired (e.g. FY2021). Defaults to "No".
+        half_years (str, optional): String used to specify if half year column is desired. Defaults to "No".
+        combined_FY_and_H (str, optional): String used to specify is a combined half year and FY column is desired. Defaults to "No".
+
+        Returns:
+        pandas.DataFrame: DataFrame with a new column 'FY' containing the FY as well as, if desired, a half year column and a combined FY half year column.
+        """
+        
+        # Change string formatted date to datetime format
+        try:
+            start_date = datetime.strptime(start_date, '%Y-%m-%d')
+        except:
+            print("Error: Date must be of format yyyy-mm-dd")
+        
+        # Create new column based off the date column which is in datetime format
+        df["OBS"] = pd.to_datetime(df[index_col])
+
+
+        def calculate_FY(date):
+            try:
+                # Run function for all possible FYs
+                for i in range(0,99):
+                    # If date is in the next ith FY year after the starting date FY then output the starting FY + i
+                    if date >= start_date + timedelta(weeks=i*52) and date < start_date + timedelta(weeks = (i+1)*52):
+                        FY = "FY"+str(int(starting_FY[-4:])+i)
+                    # If date is in the ith FY year before the starting date FY then output the starting FY - i
+                    elif date < start_date - timedelta(weeks=i*52) and date >= start_date - timedelta(weeks=(i+1)*52):
+                        FY = "FY"+str(int(starting_FY[-4:])-(i+1))
+                    # If the date not in the ith year before or after the starting date then move onto the next i
+                    else:
+                        continue
+                    
+                    # Check if short_format of date is needed
+                    if short_format == "No":
+                        pass
+                    elif short_format == "Yes":
+                        FY = "FY"+str(int(FY[-2:]))
+                        
+            # Raise error is the inputs have not been properly specified
+            except ValueError:
+                print("Error: Starting FY must be of format FY2021 and starting date must be of format yyyy-mm-dd")    
+                
+            return FY
+
+        # Apply the function to the date column
+        df["FY"] = df["OBS"].apply(calculate_FY)
+        
+        # Find the start and end date of each FY
+        unique_FYs = df["FY"].unique().tolist()
+        start_dates_list = []
+        end_dates_list = []
+        for i in unique_FYs:
+            df_FY = df[df["FY"]==i]
+            start_date = min(df_FY["OBS"])
+            end_date = max(df_FY["OBS"])
+            start_dates_list.append(start_date)
+            end_dates_list.append(end_date)
+
+        # Create LUT for FY start and end dates
+        data = {
+        "FY":unique_FYs,
+        "Start_date":start_dates_list,
+        "End_date":end_dates_list
+        }
+        df_for_dict = pd.DataFrame(data)
+
+        # Find any FY where we won't be able to take the last date and minus 52 weeks i.e. the last one
+        # First start by finding any non full years
+        df_for_dict["Need_different_calculation"] = df_for_dict["Start_date"] == df_for_dict["End_date"] - timedelta(weeks=51)
+        df_for_dict["Need_different_calculation"] = df_for_dict["Need_different_calculation"].astype(int)
+        # Now change the first FY to 0 
+        df_for_dict.loc[df_for_dict["Start_date"] == df_for_dict["Start_date"].min(),"Need_different_calculation"] = 1
+
+        # Now find end of H1 for each FY
+        conditions = [
+            (df_for_dict["Need_different_calculation"] == 1),
+            (df_for_dict["Need_different_calculation"] == 0),
+        ]
+        choices = [
+            (df_for_dict["End_date"]-timedelta(weeks=26)).dt.strftime('%Y-%m-%d'),
+            (df_for_dict["Start_date"]+timedelta(weeks=25)).dt.strftime('%Y-%m-%d'),
+        ]
+
+        df_for_dict["End of H1"] = np.select(conditions,choices,default="Other")  
+        df_for_dict.drop("Need_different_calculation",inplace=True,axis=1)
+
+        # Change to a dictionary
+        FY_LUT = df_for_dict.set_index('FY').T.to_dict()
+        
+        # Create Half year LUT
+        output = []
+        for i in FY_LUT:
+            start_date = FY_LUT[i]['Start_date'] 
+            end_date = FY_LUT[i]['End_date'] 
+            end_of_h1 = FY_LUT[i]['End of H1'] 
+            for date in pd.date_range(start_date,end_date,freq=pd.Timedelta(days=7)):
+                if date <= end_of_h1:
+                    result = [date,"H1"]
+                elif date >= end_of_h1:
+                    result = [date,"H2"]
+                output.append(result)
+
+        # Change output to dataframe LUT
+        df_date_LUT = pd.DataFrame(output,columns=["Date","Half"])
+        # Change data type to datetime for dates and then to strings for the LUT function
+        df_date_LUT["Date"] = pd.to_datetime(df_date_LUT["Date"]).dt.strftime("%Y-%m-%d")
+        # Convert LUT to dictionary
+        dict_date_LUT = self.convert_2_df_cols_to_dict(df_date_LUT, "Date", "Half")
+
+        # Create a new dataframe column which has the OBS columns as string so that in can be used in the LUT function
+        df["OBS as string"] = df["OBS"].dt.strftime("%Y-%m-%d")
+        
+        # If selected calculate FY Halves    
+        if half_years=="Yes":        
+            # Apply the function to the date column
+            df = self.apply_lookup_table_for_columns(df, ["OBS as string"], dict_date_LUT, if_not_in_dict="Other", new_column_name="Half Years")
+        
+        # Skip if this column is not desired
+        elif half_years=="No":
+            pass   
+            
+        # If FY Half Year Combined column is desired combine the two
+        if combined_FY_and_H=="Yes":
+            df["Financial Half Years"]  = df["FY"] + " " + df["Half Years"]
+        
+        # Skip if this column if not desired
+        elif combined_FY_and_H=="No":
+            pass
+            
+        return df
+    
+    def keyword_lookup_replacement(self, df, col, replacement_rows, cols_to_merge, replacement_lookup_dict,output_column_name="Updated Column"):
+        """
+        This function updates values in a specified column of the DataFrame based on a lookup dictionary.
+        It first merges several columns into a new 'Merged' column, then uses this merged column to determine
+        if replacements are needed based on the dictionary.
+
+        Parameters:
+        df (pd.DataFrame): The DataFrame to process.
+        col (str): The name of the column whose values are potentially replaced.
+        replacement_rows (str): The specific value in 'col' to check for replacements.
+        cols_to_merge (list of str): List of column names whose contents will be merged to form a lookup key.
+        replacement_lookup_dict (dict): Dictionary where keys are merged column values and values are the new data to replace in 'col'.
+        output_column_name (str, optional): Name of column outputted. Defaults to "Updated Column".
+
+        Returns:
+        pd.DataFrame: The modified DataFrame with updated values in the specified column.
+        """
+        df["Merged"] = df[cols_to_merge].apply(lambda row: '|'.join(row.values.astype(str)), axis=1)
+        
+        def replace_values(x):
+            if x[col] == replacement_rows:
+                merged_value = x['Merged']  
+                if merged_value in replacement_lookup_dict:
+                    return replacement_lookup_dict[merged_value]
+            return x[col]
+        
+        df[output_column_name] = df.apply(replace_values, axis=1)
         
         return df
```

### Comparing `imsciences-0.5.5.0/imsciences.egg-info/PKG-INFO` & `imsciences-0.5.5.1/imsciences.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsciences
-Version: 0.5.5.0
+Version: 0.5.5.1
 Summary: IMS Data Processing Package
 Author: IMS
 Author-email: cam@im-sciences.com
 Keywords: python,data processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `imsciences-0.5.5.0/setup.py` & `imsciences-0.5.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Function to read the contents of the README file
 def read_md(file_name):
     if os.path.isfile(file_name):
         with open(file_name, 'r', encoding='utf-8') as f:
             return f.read()
     return ''
 
-VERSION = '0.5.5.0'
+VERSION = '0.5.5.1'
 DESCRIPTION = 'IMS Data Processing Package'
 LONG_DESCRIPTION = read_md('README.md')  # Reading from README.md
 
 # Setting up
 setup(
     name="imsciences",
     version=VERSION,
```

