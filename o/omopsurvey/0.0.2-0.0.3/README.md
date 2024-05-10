# Comparing `tmp/omopsurvey-0.0.2.tar.gz` & `tmp/omopsurvey-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omopsurvey-0.0.2.tar", max compression
+gzip compressed data, was "omopsurvey-0.0.3.tar", max compression
```

## Comparing `omopsurvey-0.0.2.tar` & `omopsurvey-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     5369 2024-05-10 04:47:09.981340 omopsurvey-0.0.2/README.md
--rw-r--r--   0        0        0      308 2024-05-10 04:21:01.287198 omopsurvey-0.0.2/omopsurvey/__init__.py
--rw-r--r--   0        0        0     3699 2024-05-10 04:36:24.494077 omopsurvey-0.0.2/omopsurvey/codebook.py
--rw-r--r--   0        0        0     1190 2024-05-09 23:16:46.722685 omopsurvey-0.0.2/omopsurvey/pivot_data.py
--rw-r--r--   0        0        0      887 2024-05-09 23:16:46.718345 omopsurvey-0.0.2/omopsurvey/recode_missing.py
--rw-r--r--   0        0        0     3686 2024-05-10 04:36:24.488122 omopsurvey-0.0.2/omopsurvey/response_set.py
--rw-r--r--   0        0        0  1172489 2024-05-10 03:42:23.460428 omopsurvey-0.0.2/omopsurvey/survey_key.csv
--rw-r--r--   0        0        0      194 2024-05-01 01:54:49.840855 omopsurvey-0.0.2/omopsurvey/tests/codebook_test.py
--rw-r--r--   0        0        0      194 2024-05-01 01:54:49.844331 omopsurvey-0.0.2/omopsurvey/tests/map_responses_test.py
--rw-r--r--   0        0        0      194 2024-05-01 01:54:49.847047 omopsurvey-0.0.2/omopsurvey/tests/pivot_data_test.py
--rw-r--r--   0        0        0      194 2024-05-01 01:54:49.831523 omopsurvey-0.0.2/omopsurvey/tests/recode_missing_test.py
--rw-r--r--   0        0        0      615 2024-05-01 01:53:42.049881 omopsurvey-0.0.2/omopsurvey/vignettes/example_basics.ipynb
--rw-r--r--   0        0        0      615 2024-05-01 01:53:00.463035 omopsurvey-0.0.2/omopsurvey/vignettes/example_healthcare.ipynb
--rw-r--r--   0        0        0      615 2024-05-01 01:53:25.889124 omopsurvey-0.0.2/omopsurvey/vignettes/example_sdoh.ipynb
--rw-r--r--   0        0        0      722 2024-05-10 05:10:41.697266 omopsurvey-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     6384 1970-01-01 00:00:00.000000 omopsurvey-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     5369 2024-05-10 04:47:09.981340 omopsurvey-0.0.3/README.md
+-rw-r--r--   0        0        0      308 2024-05-10 04:21:01.287198 omopsurvey-0.0.3/omopsurvey/__init__.py
+-rw-r--r--   0        0        0     3699 2024-05-10 04:36:24.494077 omopsurvey-0.0.3/omopsurvey/codebook.py
+-rw-r--r--   0        0        0     1182 2024-05-10 14:16:33.555356 omopsurvey-0.0.3/omopsurvey/pivot_data.py
+-rw-r--r--   0        0        0      887 2024-05-09 23:16:46.718345 omopsurvey-0.0.3/omopsurvey/recode_missing.py
+-rw-r--r--   0        0        0     3686 2024-05-10 04:36:24.488122 omopsurvey-0.0.3/omopsurvey/response_set.py
+-rw-r--r--   0        0        0  1172489 2024-05-10 03:42:23.460428 omopsurvey-0.0.3/omopsurvey/survey_key.csv
+-rw-r--r--   0        0        0      194 2024-05-01 01:54:49.840855 omopsurvey-0.0.3/omopsurvey/tests/codebook_test.py
+-rw-r--r--   0        0        0      194 2024-05-01 01:54:49.844331 omopsurvey-0.0.3/omopsurvey/tests/map_responses_test.py
+-rw-r--r--   0        0        0      194 2024-05-01 01:54:49.847047 omopsurvey-0.0.3/omopsurvey/tests/pivot_data_test.py
+-rw-r--r--   0        0        0      194 2024-05-01 01:54:49.831523 omopsurvey-0.0.3/omopsurvey/tests/recode_missing_test.py
+-rw-r--r--   0        0        0      615 2024-05-01 01:53:42.049881 omopsurvey-0.0.3/omopsurvey/vignettes/example_basics.ipynb
+-rw-r--r--   0        0        0      615 2024-05-01 01:53:00.463035 omopsurvey-0.0.3/omopsurvey/vignettes/example_healthcare.ipynb
+-rw-r--r--   0        0        0      615 2024-05-01 01:53:25.889124 omopsurvey-0.0.3/omopsurvey/vignettes/example_sdoh.ipynb
+-rw-r--r--   0        0        0      722 2024-05-10 14:16:57.307261 omopsurvey-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6384 1970-01-01 00:00:00.000000 omopsurvey-0.0.3/PKG-INFO
```

### Comparing `omopsurvey-0.0.2/README.md` & `omopsurvey-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `omopsurvey-0.0.2/omopsurvey/codebook.py` & `omopsurvey-0.0.3/omopsurvey/codebook.py`

 * *Files identical despite different names*

### Comparing `omopsurvey-0.0.2/omopsurvey/pivot_data.py` & `omopsurvey-0.0.3/omopsurvey/pivot_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pandas as pd
 import os
 
 
 def pivot_data_numeric(data):
 
-    pivot_df = data.pivot_table(index='respondent_id',
+    pivot_df = data.pivot_table(index='person_id',
                                 columns='question_concept_id',
                                 values='answer_numeric',
                                 aggfunc='first')
 
     pivot_df.columns = ['q' + str(col) for col in pivot_df.columns]
     dir_name = os.path.dirname(data)
     new_filename = 'pivot_n_' + os.path.basename(data)
@@ -16,15 +16,15 @@
     pivot_df.to_csv(new_filepath)
 
     print(f"Pivoted dataset with numeric values saved as: {new_filepath}")
 
 
 def pivot_data_text(data):
 
-    pivot_df = data.pivot_table(index='respondent_id',
+    pivot_df = data.pivot_table(index='person_id',
                                 columns='question_concept_id',
                                 values='answer_text',
                                 aggfunc='first')
 
     pivot_df.columns = ['q' + str(col) for col in pivot_df.columns]
     dir_name = os.path.dirname(data)
     new_filename = 'pivot_t_' + os.path.basename(data)
```

### Comparing `omopsurvey-0.0.2/omopsurvey/recode_missing.py` & `omopsurvey-0.0.3/omopsurvey/recode_missing.py`

 * *Files identical despite different names*

### Comparing `omopsurvey-0.0.2/omopsurvey/response_set.py` & `omopsurvey-0.0.3/omopsurvey/response_set.py`

 * *Files identical despite different names*

### Comparing `omopsurvey-0.0.2/omopsurvey/survey_key.csv` & `omopsurvey-0.0.3/omopsurvey/survey_key.csv`

 * *Files identical despite different names*

### Comparing `omopsurvey-0.0.2/omopsurvey/vignettes/example_basics.ipynb` & `omopsurvey-0.0.3/omopsurvey/vignettes/example_basics.ipynb`

 * *Files identical despite different names*

### Comparing `omopsurvey-0.0.2/omopsurvey/vignettes/example_healthcare.ipynb` & `omopsurvey-0.0.3/omopsurvey/vignettes/example_healthcare.ipynb`

 * *Files identical despite different names*

### Comparing `omopsurvey-0.0.2/omopsurvey/vignettes/example_sdoh.ipynb` & `omopsurvey-0.0.3/omopsurvey/vignettes/example_sdoh.ipynb`

 * *Files identical despite different names*

### Comparing `omopsurvey-0.0.2/pyproject.toml` & `omopsurvey-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "omopsurvey"
-version = "0.0.2"
+version = "0.0.3"
 description = "The 'omopsurvey' Python package transforms standardized response codes from the OMOP CDM survey variables into numeric values and simplifies data preparation by providing functionalities for mapping and converting response codes, as well as handling missing data, facilitating easier and more reliable data analysis."
 authors = ["Elif Dede Yildirim <elifdy@auburn.edu>"]
 repository = "https://github.com/elifdy/omopsurvey.git"
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `omopsurvey-0.0.2/PKG-INFO` & `omopsurvey-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omopsurvey
-Version: 0.0.2
+Version: 0.0.3
 Summary: The 'omopsurvey' Python package transforms standardized response codes from the OMOP CDM survey variables into numeric values and simplifies data preparation by providing functionalities for mapping and converting response codes, as well as handling missing data, facilitating easier and more reliable data analysis.
 Home-page: https://github.com/elifdy/omopsurvey.git
 License: MIT
 Author: Elif Dede Yildirim
 Author-email: elifdy@auburn.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

