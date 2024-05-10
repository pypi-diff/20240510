# Comparing `tmp/dpkits-1.2.2.tar.gz` & `tmp/dpkits-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpkits-1.2.2.tar", last modified: Mon Apr 22 09:40:46 2024, max compression
+gzip compressed data, was "dpkits-1.2.3.tar", last modified: Fri May 10 06:48:03 2024, max compression
```

## Comparing `dpkits-1.2.2.tar` & `dpkits-1.2.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 09:40:46.683263 dpkits-1.2.2/
--rw-rw-rw-   0        0        0     1091 2023-08-31 09:04:23.000000 dpkits-1.2.2/LICENSE
--rw-rw-rw-   0        0        0    12196 2024-04-22 09:40:46.682266 dpkits-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0    11652 2023-10-06 10:25:52.000000 dpkits-1.2.2/README.md
--rw-rw-rw-   0        0        0      626 2024-04-22 09:39:59.000000 dpkits-1.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-22 09:40:46.684274 dpkits-1.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-22 09:40:46.616301 dpkits-1.2.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-22 09:40:46.646754 dpkits-1.2.2/src/dpkits/
--rw-rw-rw-   0        0        0      565 2024-01-11 08:02:54.000000 dpkits-1.2.2/src/dpkits/__init__.py
--rw-rw-rw-   0        0        0    28970 2024-03-29 03:25:00.000000 dpkits-1.2.2/src/dpkits/ap_data_converter.py
--rw-rw-rw-   0        0        0     9948 2023-10-04 08:35:50.000000 dpkits-1.2.2/src/dpkits/calculate_lsm.py
--rw-rw-rw-   0        0        0    11069 2024-01-31 04:23:09.000000 dpkits-1.2.2/src/dpkits/codeframe_reader.py
--rw-rw-rw-   0        0        0     5104 2024-01-09 08:11:30.000000 dpkits-1.2.2/src/dpkits/data_analysis.py
--rw-rw-rw-   0        0        0     2798 2024-04-09 06:58:27.000000 dpkits-1.2.2/src/dpkits/data_processing.py
--rw-rw-rw-   0        0        0     8198 2024-03-29 03:28:36.000000 dpkits-1.2.2/src/dpkits/data_transpose.py
--rw-rw-rw-   0        0        0    25579 2023-12-01 07:03:09.000000 dpkits-1.2.2/src/dpkits/table_formater.py
--rw-rw-rw-   0        0        0    66039 2024-04-22 09:21:35.000000 dpkits-1.2.2/src/dpkits/table_generator.py
-drwxrwxrwx   0        0        0        0 2024-04-22 09:40:46.679809 dpkits-1.2.2/src/dpkits.egg-info/
--rw-rw-rw-   0        0        0    12196 2024-04-22 09:40:46.000000 dpkits-1.2.2/src/dpkits.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      428 2024-04-22 09:40:46.000000 dpkits-1.2.2/src/dpkits.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 09:40:46.000000 dpkits-1.2.2/src/dpkits.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-22 09:40:46.000000 dpkits-1.2.2/src/dpkits.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 06:48:03.610378 dpkits-1.2.3/
+-rw-rw-rw-   0        0        0     1091 2023-08-31 09:04:23.000000 dpkits-1.2.3/LICENSE
+-rw-rw-rw-   0        0        0    12196 2024-05-10 06:48:03.608365 dpkits-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0    11652 2023-10-06 10:25:52.000000 dpkits-1.2.3/README.md
+-rw-rw-rw-   0        0        0      626 2024-05-10 06:47:15.000000 dpkits-1.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-10 06:48:03.610378 dpkits-1.2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-10 06:48:03.538125 dpkits-1.2.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-10 06:48:03.573798 dpkits-1.2.3/src/dpkits/
+-rw-rw-rw-   0        0        0      565 2024-01-11 08:02:54.000000 dpkits-1.2.3/src/dpkits/__init__.py
+-rw-rw-rw-   0        0        0    28970 2024-03-29 03:25:00.000000 dpkits-1.2.3/src/dpkits/ap_data_converter.py
+-rw-rw-rw-   0        0        0     9948 2023-10-04 08:35:50.000000 dpkits-1.2.3/src/dpkits/calculate_lsm.py
+-rw-rw-rw-   0        0        0    11069 2024-01-31 04:23:09.000000 dpkits-1.2.3/src/dpkits/codeframe_reader.py
+-rw-rw-rw-   0        0        0     5209 2024-05-06 08:45:27.000000 dpkits-1.2.3/src/dpkits/data_analysis.py
+-rw-rw-rw-   0        0        0     2798 2024-04-09 06:58:27.000000 dpkits-1.2.3/src/dpkits/data_processing.py
+-rw-rw-rw-   0        0        0     8198 2024-03-29 03:28:36.000000 dpkits-1.2.3/src/dpkits/data_transpose.py
+-rw-rw-rw-   0        0        0    26578 2024-05-10 06:33:30.000000 dpkits-1.2.3/src/dpkits/table_formater.py
+-rw-rw-rw-   0        0        0    66039 2024-04-24 03:29:44.000000 dpkits-1.2.3/src/dpkits/table_generator.py
+drwxrwxrwx   0        0        0        0 2024-05-10 06:48:03.606366 dpkits-1.2.3/src/dpkits.egg-info/
+-rw-rw-rw-   0        0        0    12196 2024-05-10 06:48:03.000000 dpkits-1.2.3/src/dpkits.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      428 2024-05-10 06:48:03.000000 dpkits-1.2.3/src/dpkits.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 06:48:03.000000 dpkits-1.2.3/src/dpkits.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-10 06:48:03.000000 dpkits-1.2.3/src/dpkits.egg-info/top_level.txt
```

### Comparing `dpkits-1.2.2/LICENSE` & `dpkits-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dpkits-1.2.2/PKG-INFO` & `dpkits-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpkits
-Version: 1.2.2
+Version: 1.2.3
 Summary: A small package for data processing
 Author-email: Hung Dao <hung.daotuan.1991@gmail.com>
 Project-URL: Homepage, https://github.com/HungDaoHD/packaging_dpkits
 Project-URL: Bug Tracker, https://github.com/HungDaoHD/packaging_dpkits/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dpkits-1.2.2/README.md` & `dpkits-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `dpkits-1.2.2/pyproject.toml` & `dpkits-1.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dpkits"
-version = "1.2.2"
+version = "1.2.3"
 authors = [
   { name="Hung Dao", email="hung.daotuan.1991@gmail.com" },
 ]
 description = "A small package for data processing"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `dpkits-1.2.2/src/dpkits/__init__.py` & `dpkits-1.2.3/src/dpkits/__init__.py`

 * *Files identical despite different names*

### Comparing `dpkits-1.2.2/src/dpkits/ap_data_converter.py` & `dpkits-1.2.3/src/dpkits/ap_data_converter.py`

 * *Files identical despite different names*

### Comparing `dpkits-1.2.2/src/dpkits/calculate_lsm.py` & `dpkits-1.2.3/src/dpkits/calculate_lsm.py`

 * *Files identical despite different names*

### Comparing `dpkits-1.2.2/src/dpkits/codeframe_reader.py` & `dpkits-1.2.3/src/dpkits/codeframe_reader.py`

 * *Files identical despite different names*

### Comparing `dpkits-1.2.2/src/dpkits/data_analysis.py` & `dpkits-1.2.3/src/dpkits/data_analysis.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 import pandas as pd
 import numpy as np
 import pingouin as pg
 
-
-
-
-
 from pptx import Presentation
 from pptx.chart.data import XyChartData
 from pptx.enum.chart import XL_CHART_TYPE, XL_LABEL_POSITION
 from pptx.util import Inches
 
+from sklearn.linear_model import LinearRegression, LogisticRegression
 
 
 
 
 class DataAnalysis:
     def __init__(self, df_data: pd.DataFrame, df_info: pd.DataFrame):
 
@@ -102,25 +99,21 @@
         #
         # chart = slide.shapes.add_chart(XL_CHART_TYPE.XY_SCATTER, x, y, cx, cy, chart_data)
         #
         # prs.save('chart-01-test.pptx')
 
 
 
-
-
-
-
-
-
     def linear_regression(self, dict_define_linear: dict, output_name: str):
 
         # Single: y = b + a*x
         # Multiple: y = b + a1*x1 + a2*x2 + ... + an*xn
 
+        # HERE: Going to replace with sklearn func
+
         with pd.ExcelWriter(f'{output_name}.xlsx', engine='openpyxl') as writer:
             for k_ln, v_ln in dict_define_linear.items():
                 print(f'Processing linear regression - {k_ln}')
                 df_data = self.df_data.query(str_query).copy() if v_ln['str_query'] else self.df_data.copy()
 
                 df_data.loc[:, 'dep_var'] = df_data.loc[:, v_ln['dependent_vars']].mean(axis=1)
```

### Comparing `dpkits-1.2.2/src/dpkits/data_processing.py` & `dpkits-1.2.3/src/dpkits/data_processing.py`

 * *Files identical despite different names*

### Comparing `dpkits-1.2.2/src/dpkits/data_transpose.py` & `dpkits-1.2.3/src/dpkits/data_transpose.py`

 * *Files identical despite different names*

### Comparing `dpkits-1.2.2/src/dpkits/table_formater.py` & `dpkits-1.2.3/src/dpkits/table_formater.py`

 * *Files 2% similar despite different names*

```diff
@@ -340,15 +340,14 @@
 
                         if icol in lst_sub_header_col and irow in lst_sub_side_col:
                             cur_cell.border = self.medium_left_3_border
 
                         for irow_hd in range(3, start_side_row):
                             ws.cell(irow_hd, icol).border = self.medium_left_4_border
 
-
                     if ws.cell(irow, 4).value == 'base':
                         cur_cell.font = Font(bold=True)
                         cur_cell.fill = PatternFill(patternType='solid', fgColor='DAEEF3')
 
                     elif ws.cell(irow, 4).value == 'bes':
                         cur_cell.font = Font(bold=True)
                         cur_cell.number_format = '0.0'
@@ -397,18 +396,36 @@
                             cur_cell.font = Font(bold=True)
 
                             if num_format == 'pct':
                                 cur_cell.number_format = '0'
                             elif num_format == 'pct_sign':
                                 cur_cell.number_format = '0%'
 
-                            if '(NET)' in str(ws.cell(irow, 5).value).upper():
-                                ws.cell(irow, 5).font = Font(bold=True, underline='double')
+                            cat_lbl = str(ws.cell(irow, 5).value)
+                            net_cell = ws.cell(irow, icol)
+
+                            # NET CODE UPDATE FOR MSN PROJECTS
+                            if 'NET 0' in cat_lbl.upper():
+                                # Net: #A02B93
+                                net_cell.fill = PatternFill(patternType='solid', fgColor='A02B93')
+                                net_cell.font = Font(bold=True, color='FFFFFF')
+
+                            elif 'NET 1' in cat_lbl.upper():
+                                # Sub-net: #F2CEEF
+                                net_cell.fill = PatternFill(patternType='solid', fgColor='F2CEEF')
+
+                            elif 'NET 2' in cat_lbl.upper():
+                                # Sub-sub-net: #B5E6A2
+                                net_cell.fill = PatternFill(patternType='solid', fgColor='B5E6A2')
+
                             else:
-                                ws.cell(irow, 5).font = Font(bold=True, underline='single')
+                                if '(NET)' in cat_lbl.upper():
+                                    ws.cell(irow, 5).font = Font(bold=True, underline='double')
+                                else:
+                                    ws.cell(irow, 5).font = Font(bold=True, underline='single')
 
                         else:
                             if icol > 5:
                                 if num_format == 'pct':
                                     cur_cell.number_format = '0'
                                 elif num_format == 'pct_sign':
                                     cur_cell.number_format = '0%'
@@ -473,15 +490,16 @@
             ws.column_dimensions['B'].width = 40
             ws.column_dimensions['E'].width = 40
 
             if not is_sig_tbl:
 
                 for icol in range(6, ws.max_column + 1).__reversed__():
                     if icol % 2 != 0:
-                        ws.delete_cols(icol, 1)
+                        # ws.delete_cols(icol, 1)
+                        ws.delete_cols(icol)
 
             else:
                 for icol in range(6, ws.max_column + 1):
                     ws.column_dimensions[get_column_letter(icol)].width = 7
 
 
             ws.column_dimensions['C'].hidden = True
@@ -570,8 +588,8 @@
 
 
         # output_name = self.xlsx_name.replace('.xlsx', '_output.xlsx')
         output_name = self.xlsx_name
 
         print(f"Save wb as {output_name}")
         wb.save(output_name)
-        wb.close()
+        wb.close()
```

### Comparing `dpkits-1.2.2/src/dpkits/table_generator.py` & `dpkits-1.2.3/src/dpkits/table_generator.py`

 * *Files identical despite different names*

### Comparing `dpkits-1.2.2/src/dpkits.egg-info/PKG-INFO` & `dpkits-1.2.3/src/dpkits.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpkits
-Version: 1.2.2
+Version: 1.2.3
 Summary: A small package for data processing
 Author-email: Hung Dao <hung.daotuan.1991@gmail.com>
 Project-URL: Homepage, https://github.com/HungDaoHD/packaging_dpkits
 Project-URL: Bug Tracker, https://github.com/HungDaoHD/packaging_dpkits/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

