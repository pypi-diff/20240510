# Comparing `tmp/metabolights_utils-0.9.8.tar.gz` & `tmp/metabolights_utils-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metabolights_utils-0.9.8.tar", max compression
+gzip compressed data, was "metabolights_utils-0.9.9.tar", max compression
```

## Comparing `metabolights_utils-0.9.8.tar` & `metabolights_utils-0.9.9.tar`

### file list

```diff
@@ -1,55 +1,56 @@
--rw-r--r--   0        0        0    11357 2023-07-11 10:00:28.160792 metabolights_utils-0.9.8/LICENSE
--rw-r--r--   0        0        0    17709 2023-07-20 21:36:19.778680 metabolights_utils-0.9.8/README.md
--rw-r--r--   0        0        0        0 2023-07-19 00:16:47.456526 metabolights_utils-0.9.8/metabolights_utils/__init__.py
--rw-r--r--   0        0        0      263 2023-07-20 22:58:12.607673 metabolights_utils-0.9.8/metabolights_utils/common.py
--rw-r--r--   0        0        0     2198 2023-07-19 09:21:04.692280 metabolights_utils-0.9.8/metabolights_utils/isatab/__init__.py
--rw-r--r--   0        0        0        0 2023-07-19 00:16:47.525753 metabolights_utils-0.9.8/metabolights_utils/isatab/default/__init__.py
--rw-r--r--   0        0        0      718 2023-07-25 21:14:05.704460 metabolights_utils-0.9.8/metabolights_utils/isatab/default/assay_file.py
--rw-r--r--   0        0        0     1268 2023-07-19 00:16:47.587091 metabolights_utils-0.9.8/metabolights_utils/isatab/default/assignment_file.py
--rw-r--r--   0        0        0     1536 2023-07-19 00:16:47.626096 metabolights_utils-0.9.8/metabolights_utils/isatab/default/base_isa_file.py
--rw-r--r--   0        0        0     5878 2023-07-20 09:45:20.078824 metabolights_utils-0.9.8/metabolights_utils/isatab/default/base_isa_table_file.py
--rw-r--r--   0        0        0     1881 2023-07-19 09:14:50.131288 metabolights_utils-0.9.8/metabolights_utils/isatab/default/factory.py
--rw-r--r--   0        0        0    11163 2023-07-19 00:16:47.792874 metabolights_utils-0.9.8/metabolights_utils/isatab/default/investigation_file.py
--rw-r--r--   0        0        0      705 2023-07-25 21:14:42.499180 metabolights_utils-0.9.8/metabolights_utils/isatab/default/sample_file.py
--rw-r--r--   0        0        0     1488 2023-07-19 00:16:47.917232 metabolights_utils-0.9.8/metabolights_utils/isatab/default/writer.py
--rw-r--r--   0        0        0     9754 2023-07-25 21:16:06.789386 metabolights_utils-0.9.8/metabolights_utils/isatab/reader.py
--rw-r--r--   0        0        0     3740 2023-07-20 23:07:06.886505 metabolights_utils-0.9.8/metabolights_utils/isatab/writer.py
--rw-r--r--   0        0        0        0 2023-07-19 00:16:47.940900 metabolights_utils-0.9.8/metabolights_utils/models/__init__.py
--rw-r--r--   0        0        0      443 2023-07-25 21:15:26.531786 metabolights_utils-0.9.8/metabolights_utils/models/common.py
--rw-r--r--   0        0        0      149 2023-07-19 00:16:48.007068 metabolights_utils-0.9.8/metabolights_utils/models/enums.py
--rw-r--r--   0        0        0        0 2023-07-19 00:16:48.019187 metabolights_utils-0.9.8/metabolights_utils/models/isa/__init__.py
--rw-r--r--   0        0        0      531 2023-07-19 00:16:48.049609 metabolights_utils-0.9.8/metabolights_utils/models/isa/assay_file.py
--rw-r--r--   0        0        0      402 2023-07-19 00:16:48.089220 metabolights_utils-0.9.8/metabolights_utils/models/isa/assignment_file.py
--rw-r--r--   0        0        0     9505 2023-08-31 07:17:30.961135 metabolights_utils-0.9.8/metabolights_utils/models/isa/common.py
--rw-r--r--   0        0        0      478 2023-07-19 00:16:48.146363 metabolights_utils-0.9.8/metabolights_utils/models/isa/enums.py
--rw-r--r--   0        0        0    11080 2023-07-19 00:16:48.173059 metabolights_utils-0.9.8/metabolights_utils/models/isa/investigation_file.py
--rw-r--r--   0        0        0    18440 2023-07-20 09:45:19.894366 metabolights_utils-0.9.8/metabolights_utils/models/isa/parser/common.py
--rw-r--r--   0        0        0    22198 2023-07-19 00:16:48.338368 metabolights_utils-0.9.8/metabolights_utils/models/isa/parser/investigation_parser.py
--rw-r--r--   0        0        0    18266 2023-08-30 13:35:57.386201 metabolights_utils-0.9.8/metabolights_utils/models/isa/parser/isa_table_parser.py
--rw-r--r--   0        0        0      455 2023-08-31 07:17:45.630167 metabolights_utils-0.9.8/metabolights_utils/models/isa/samples_file.py
--rw-r--r--   0        0        0        0 2023-07-19 00:16:48.415532 metabolights_utils-0.9.8/metabolights_utils/models/metabolights/__init__.py
--rw-r--r--   0        0        0     1077 2023-07-19 00:16:48.427548 metabolights_utils-0.9.8/metabolights_utils/models/metabolights/metabolights_study.py
--rw-r--r--   0        0        0        0 2023-07-19 00:16:48.443379 metabolights_utils-0.9.8/metabolights_utils/models/parser/__init__.py
--rw-r--r--   0        0        0      766 2023-07-19 00:16:48.470689 metabolights_utils-0.9.8/metabolights_utils/models/parser/common.py
--rw-r--r--   0        0        0      148 2023-07-19 00:16:48.476458 metabolights_utils-0.9.8/metabolights_utils/models/parser/enums.py
--rw-r--r--   0        0        0        0 2023-07-19 00:16:48.501180 metabolights_utils-0.9.8/metabolights_utils/tsv/__init__.py
--rw-r--r--   0        0        0        0 2023-07-19 00:16:48.528354 metabolights_utils-0.9.8/metabolights_utils/tsv/actions/__init__.py
--rw-r--r--   0        0        0     3559 2023-07-19 08:23:28.339563 metabolights_utils-0.9.8/metabolights_utils/tsv/actions/add_column.py
--rw-r--r--   0        0        0     3488 2023-07-19 08:26:08.140976 metabolights_utils-0.9.8/metabolights_utils/tsv/actions/add_row.py
--rw-r--r--   0        0        0     1339 2023-07-19 07:58:19.960337 metabolights_utils-0.9.8/metabolights_utils/tsv/actions/base.py
--rw-r--r--   0        0        0     3390 2023-07-19 08:23:28.347823 metabolights_utils-0.9.8/metabolights_utils/tsv/actions/copy_column.py
--rw-r--r--   0        0        0     3144 2023-07-19 08:23:28.383070 metabolights_utils-0.9.8/metabolights_utils/tsv/actions/copy_row.py
--rw-r--r--   0        0        0     2492 2023-07-19 08:23:28.528233 metabolights_utils-0.9.8/metabolights_utils/tsv/actions/delete_column.py
--rw-r--r--   0        0        0     1986 2023-07-19 09:13:04.618046 metabolights_utils-0.9.8/metabolights_utils/tsv/actions/delete_row.py
--rw-r--r--   0        0        0     2867 2023-07-19 08:23:28.613461 metabolights_utils-0.9.8/metabolights_utils/tsv/actions/move_column.py
--rw-r--r--   0        0        0     3363 2023-07-19 08:23:28.672360 metabolights_utils-0.9.8/metabolights_utils/tsv/actions/move_row.py
--rw-r--r--   0        0        0     3157 2023-07-19 08:23:28.701280 metabolights_utils-0.9.8/metabolights_utils/tsv/actions/update_cell.py
--rw-r--r--   0        0        0     3544 2023-07-19 09:13:21.371457 metabolights_utils-0.9.8/metabolights_utils/tsv/actions/update_column.py
--rw-r--r--   0        0        0     2077 2023-07-19 09:13:17.513241 metabolights_utils-0.9.8/metabolights_utils/tsv/actions/update_column_header.py
--rw-r--r--   0        0        0     2229 2023-07-19 08:23:28.847528 metabolights_utils-0.9.8/metabolights_utils/tsv/actions/update_row.py
--rw-r--r--   0        0        0    19935 2023-07-20 22:52:30.816088 metabolights_utils-0.9.8/metabolights_utils/tsv/filter.py
--rw-r--r--   0        0        0     6043 2023-07-22 14:53:04.282869 metabolights_utils-0.9.8/metabolights_utils/tsv/model.py
--rw-r--r--   0        0        0    12899 2023-07-20 13:14:20.411943 metabolights_utils-0.9.8/metabolights_utils/tsv/sort.py
--rw-r--r--   0        0        0     5647 2023-07-19 08:26:02.864303 metabolights_utils-0.9.8/metabolights_utils/tsv/tsv_file_updater.py
--rw-r--r--   0        0        0     1472 2023-08-31 07:18:03.161308 metabolights_utils-0.9.8/pyproject.toml
--rw-r--r--   0        0        0    18762 1970-01-01 00:00:00.000000 metabolights_utils-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-11 10:00:28.160792 metabolights_utils-0.9.9/LICENSE
+-rw-r--r--   0        0        0    17817 2023-11-03 08:32:30.594723 metabolights_utils-0.9.9/README.md
+-rw-r--r--   0        0        0        0 2023-07-19 00:16:47.456526 metabolights_utils-0.9.9/metabolights_utils/__init__.py
+-rw-r--r--   0        0        0      275 2023-11-02 20:16:10.332222 metabolights_utils-0.9.9/metabolights_utils/common.py
+-rw-r--r--   0        0        0     2198 2023-11-03 02:23:02.498653 metabolights_utils-0.9.9/metabolights_utils/isatab/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-19 00:16:47.525753 metabolights_utils-0.9.9/metabolights_utils/isatab/default/__init__.py
+-rw-r--r--   0        0        0      759 2023-11-03 11:58:23.178806 metabolights_utils-0.9.9/metabolights_utils/isatab/default/assay_file.py
+-rw-r--r--   0        0        0     1267 2023-11-03 11:58:23.175702 metabolights_utils-0.9.9/metabolights_utils/isatab/default/assignment_file.py
+-rw-r--r--   0        0        0     1598 2023-11-03 12:22:29.362790 metabolights_utils-0.9.9/metabolights_utils/isatab/default/base_isa_file.py
+-rw-r--r--   0        0        0     6429 2023-11-03 18:46:08.116389 metabolights_utils-0.9.9/metabolights_utils/isatab/default/base_isa_table_file.py
+-rw-r--r--   0        0        0     1881 2023-11-03 02:23:02.501782 metabolights_utils-0.9.9/metabolights_utils/isatab/default/factory.py
+-rw-r--r--   0        0        0    12246 2023-11-03 18:46:08.235550 metabolights_utils-0.9.9/metabolights_utils/isatab/default/investigation_file.py
+-rw-r--r--   0        0        0      796 2023-11-03 11:58:23.179036 metabolights_utils-0.9.9/metabolights_utils/isatab/default/sample_file.py
+-rw-r--r--   0        0        0     1488 2023-11-03 02:23:02.528304 metabolights_utils-0.9.9/metabolights_utils/isatab/default/writer.py
+-rw-r--r--   0        0        0     9828 2023-11-03 08:34:05.257149 metabolights_utils-0.9.9/metabolights_utils/isatab/reader.py
+-rw-r--r--   0        0        0     3756 2023-11-02 22:36:27.088267 metabolights_utils-0.9.9/metabolights_utils/isatab/writer.py
+-rw-r--r--   0        0        0        0 2023-07-19 00:16:47.940900 metabolights_utils-0.9.9/metabolights_utils/models/__init__.py
+-rw-r--r--   0        0        0      443 2023-07-25 21:15:26.531786 metabolights_utils-0.9.9/metabolights_utils/models/common.py
+-rw-r--r--   0        0        0      149 2023-07-19 00:16:48.007068 metabolights_utils-0.9.9/metabolights_utils/models/enums.py
+-rw-r--r--   0        0        0        0 2023-07-19 00:16:48.019187 metabolights_utils-0.9.9/metabolights_utils/models/isa/__init__.py
+-rw-r--r--   0        0        0      531 2023-07-19 00:16:48.049609 metabolights_utils-0.9.9/metabolights_utils/models/isa/assay_file.py
+-rw-r--r--   0        0        0      402 2023-07-19 00:16:48.089220 metabolights_utils-0.9.9/metabolights_utils/models/isa/assignment_file.py
+-rw-r--r--   0        0        0     9961 2023-11-03 18:46:08.203128 metabolights_utils-0.9.9/metabolights_utils/models/isa/common.py
+-rw-r--r--   0        0        0      478 2023-07-19 00:16:48.146363 metabolights_utils-0.9.9/metabolights_utils/models/isa/enums.py
+-rw-r--r--   0        0        0    11069 2023-11-02 19:50:49.717593 metabolights_utils-0.9.9/metabolights_utils/models/isa/investigation_file.py
+-rw-r--r--   0        0        0    18631 2023-11-03 02:23:02.876176 metabolights_utils-0.9.9/metabolights_utils/models/isa/parser/common.py
+-rw-r--r--   0        0        0    24553 2023-11-03 18:46:08.437985 metabolights_utils-0.9.9/metabolights_utils/models/isa/parser/investigation_parser.py
+-rw-r--r--   0        0        0    18638 2023-11-03 02:23:02.981181 metabolights_utils-0.9.9/metabolights_utils/models/isa/parser/isa_table_parser.py
+-rw-r--r--   0        0        0      455 2023-11-03 00:02:24.839165 metabolights_utils-0.9.9/metabolights_utils/models/isa/samples_file.py
+-rw-r--r--   0        0        0        0 2023-07-19 00:16:48.415532 metabolights_utils-0.9.9/metabolights_utils/models/metabolights/__init__.py
+-rw-r--r--   0        0        0     1077 2023-07-19 00:16:48.427548 metabolights_utils-0.9.9/metabolights_utils/models/metabolights/metabolights_study.py
+-rw-r--r--   0        0        0        0 2023-07-19 00:16:48.443379 metabolights_utils-0.9.9/metabolights_utils/models/parser/__init__.py
+-rw-r--r--   0        0        0      766 2023-07-19 00:16:48.470689 metabolights_utils-0.9.9/metabolights_utils/models/parser/common.py
+-rw-r--r--   0        0        0      148 2023-07-19 00:16:48.476458 metabolights_utils-0.9.9/metabolights_utils/models/parser/enums.py
+-rw-r--r--   0        0        0        0 2023-07-19 00:16:48.501180 metabolights_utils-0.9.9/metabolights_utils/tsv/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-19 00:16:48.528354 metabolights_utils-0.9.9/metabolights_utils/tsv/actions/__init__.py
+-rw-r--r--   0        0        0     3599 2023-11-03 18:46:08.170484 metabolights_utils-0.9.9/metabolights_utils/tsv/actions/add_column.py
+-rw-r--r--   0        0        0     3528 2023-11-03 18:46:08.252995 metabolights_utils-0.9.9/metabolights_utils/tsv/actions/add_row.py
+-rw-r--r--   0        0        0     1353 2023-11-03 02:23:02.894392 metabolights_utils-0.9.9/metabolights_utils/tsv/actions/base.py
+-rw-r--r--   0        0        0     3487 2023-11-03 18:46:08.302607 metabolights_utils-0.9.9/metabolights_utils/tsv/actions/copy_column.py
+-rw-r--r--   0        0        0     3202 2023-11-03 18:46:08.290606 metabolights_utils-0.9.9/metabolights_utils/tsv/actions/copy_row.py
+-rw-r--r--   0        0        0     2495 2023-11-03 18:46:08.297052 metabolights_utils-0.9.9/metabolights_utils/tsv/actions/delete_column.py
+-rw-r--r--   0        0        0     2026 2023-11-03 12:05:19.906092 metabolights_utils-0.9.9/metabolights_utils/tsv/actions/delete_row.py
+-rw-r--r--   0        0        0     2907 2023-11-03 18:46:08.346110 metabolights_utils-0.9.9/metabolights_utils/tsv/actions/move_column.py
+-rw-r--r--   0        0        0     3379 2023-11-03 12:05:19.906147 metabolights_utils-0.9.9/metabolights_utils/tsv/actions/move_row.py
+-rw-r--r--   0        0        0     3186 2023-11-03 18:46:08.357212 metabolights_utils-0.9.9/metabolights_utils/tsv/actions/update_cell.py
+-rw-r--r--   0        0        0     3583 2023-11-03 18:46:08.379977 metabolights_utils-0.9.9/metabolights_utils/tsv/actions/update_column.py
+-rw-r--r--   0        0        0     2117 2023-11-03 18:46:08.388898 metabolights_utils-0.9.9/metabolights_utils/tsv/actions/update_column_header.py
+-rw-r--r--   0        0        0     2269 2023-11-03 18:46:08.393014 metabolights_utils-0.9.9/metabolights_utils/tsv/actions/update_row.py
+-rw-r--r--   0        0        0    20825 2023-11-03 18:46:08.720460 metabolights_utils-0.9.9/metabolights_utils/tsv/filter.py
+-rw-r--r--   0        0        0     6043 2023-07-22 14:53:04.282869 metabolights_utils-0.9.9/metabolights_utils/tsv/model.py
+-rw-r--r--   0        0        0    12971 2023-11-03 02:23:03.290193 metabolights_utils-0.9.9/metabolights_utils/tsv/sort.py
+-rw-r--r--   0        0        0     5427 2023-11-03 02:23:03.190933 metabolights_utils-0.9.9/metabolights_utils/tsv/tsv_file_updater.py
+-rw-r--r--   0        0        0      251 2023-11-03 01:17:28.960201 metabolights_utils-0.9.9/metabolights_utils/tsv/utils.py
+-rw-r--r--   0        0        0     1542 2023-11-03 08:44:00.776290 metabolights_utils-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0    18840 1970-01-01 00:00:00.000000 metabolights_utils-0.9.9/PKG-INFO
```

### Comparing `metabolights_utils-0.9.8/LICENSE` & `metabolights_utils-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.8/README.md` & `metabolights_utils-0.9.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -33,33 +33,30 @@
 
 
 ### Installation
 ---
 The following command installs metabolights-utils from the Python Package Index. You will need a working installation of Python 3.8+ and pip3.
 
 ```shell
-pip install -U sphinx
+pip3 install -U metabolights_utils
 ```
 
 
 ### Read and update Investigation files
 ---
-Read and update an investigation file. Returned objects are json serializable so you can use them with REST APIs.  
+Read and update an investigation file. Results are json serializable, so you can use them with REST APIs.  
 
 ```python 
 import os
 import pathlib
 import uuid
-from ast import List
+from typing import List
 
 from metabolights_utils.isatab import Reader, Writer
-from metabolights_utils.isatab.reader import (
-    InvestigationFileReader,
-    InvestigationFileReaderResult,
-)
+from metabolights_utils.isatab.reader import InvestigationFileReader, InvestigationFileReaderResult
 from metabolights_utils.isatab.writer import InvestigationFileWriter
 from metabolights_utils.models.isa.common import OntologyItem
 from metabolights_utils.models.isa.investigation_file import Assay, Study
 
 
 def test_investigation_file_write_01():
     file_path = pathlib.Path("tests/test-data/MTBLS398/i_Investigation.txt")
@@ -83,33 +80,33 @@
     assert assay_read.measurement_type.term == "test"
     assert assay_read.measurement_type.term_source_ref == "test source"
     assert assay_read.measurement_type.term_accession_number == "test accesion"
     os.remove(tmp_path)
 
 ```
 
-### ISA table file pagination
+### Read and Update ISA Table Files with Pagination Support
 ---
-* Update page size (number of rows in a page) and read results with the selected page size.
-* Define custom row offset and read rows with a limit. Row indices in a page can be unordered after filter and sort operations. You can get actual row index of the selected row using result.
-* Read only the selected columns you defined. If a selected column has additional columns (Term Source REF, etc) and these columns are not defined, they will be in result. Column names may be different than header if there are multiple column with same header. 
-* If no column selected, columns will be ordered. If columns are selected, result will contain columns in the selected order. You can get actual column index of a column using result.
+* Select page size (number of rows in a page) and read results with the selected page size.
+* Define custom row offset and read only selected rows. Actual row indices in a result may be unordered after filter and sort operations. 
+* Read the selected columns you defined. If a selected column has additional columns (Term Source REF, etc) and these columns are not defined by user, they will also be in the result. Column names may be different than header if there are multiple columns with same header. 
+* If columns are not selected, all table columns will be returned in result. If columns are selected, result will contain only these columns in selected order.
 
 ---
 #### Example 1: Read ISA table file
 ---
 
 Read selected assay file (a_*.txt) rows and columns with pagination support. You can use same methods with sample (s_*.txt) and metabolite assignment (m_*.tsv) files.
 ```python
 import pathlib
 
 from metabolights_utils.isatab import Reader
 from metabolights_utils.isatab.reader import (
     IsaTableFileReader,
-    IsaTableFileReaderResult,
+    IsaTableFileReaderResult
 )
 
 
 def test_assay_file_success_01():
     file_path = pathlib.Path(
         "tests/test-data/MTBLS373/a_MTBLS373_sevinaskascreen_metabolite_profiling_mass_spectrometry.txt"
     )
@@ -162,41 +159,42 @@
         page=294, results_per_page=50, file_path=file_path
     )
     assert len(result.parser_report.messages) == 0
     assert result.isa_table_file.table.row_count == 20
 
     # get page 2 with selected columns from isa table.
     # read 50 items from offset 50 (page 2)
-    # If addition columns are not added to result even if they are not selected.
+    # Addition columns will be in result even if they are not selected.
+    # Parameter Value[Autosampler model] is ontology column. So 2 new columns will be added to result.
     result: IsaTableFileReaderResult = reader.get_page(
         page=2,
         results_per_page=50,
         file_path=file_path,
         selected_columns=["Sample Name", "Parameter Value[Autosampler model]"],
     )
     assert len(result.parser_report.messages) == 0
     assert result.isa_table_file.table.row_count == 50
     assert len(result.isa_table_file.table.columns) == 4
 ```
 
 
-#### Example 2: Read and update ISA table file
+#### Example 2: Update ISA table file
 ---
 
 Load ISA table page and save after update table content
 
 ```python
 import os
 import pathlib
 import shutil
 
 from metabolights_utils.isatab import Reader, Writer
 from metabolights_utils.isatab.reader import (
     IsaTableFileReader,
-    IsaTableFileReaderResult,
+    IsaTableFileReaderResult
 )
 from metabolights_utils.isatab.writer import IsaTableFileWriter
 
 
 def test_assay_file_read_write():
     path_original = pathlib.Path(
         "tests/test-data/MTBLS1/a_MTBLS1_metabolite_profiling_NMR_spectroscopy.txt"
@@ -204,15 +202,15 @@
     file_path = (
         ".test-temp/test-data/MTBLS1/a_MTBLS1_metabolite_profiling_NMR_spectroscopy.txt"
     )
     os.makedirs(os.path.dirname(file_path), exist_ok=True)
     shutil.copy(path_original, file_path)
     helper: IsaTableFileReader = Reader.get_assay_file_reader()
 
-    with open(file_path, "r") as file_buffer:
+    with open(file_path, "r", encoding="utf-8") as file_buffer:
         # read second page of assa file
         result: IsaTableFileReaderResult = helper.get_page(
             file_buffer=file_buffer,
             page=2,
             results_per_page=50,
             file_path=str(file_path),
             selected_columns=[
@@ -222,19 +220,20 @@
             ],
         )
         assert len(result.parser_report.messages) == 0
         assert result.isa_table_file.table.row_count == 50
         assert len(result.isa_table_file.table.columns) == 3
     
     writer: IsaTableFileWriter = Writer.get_assay_file_writer()
-    sha256 = "6ea4c731ce35165f83a5d30438cd8753a6afa5fa9a1109893ffc1c213b1da869"
     isa_table = result.isa_table_file.table
+
+    sha256_hash = result.isa_table_file.sha256_hash
     # save same content without any update
     report = writer.save_isa_table(
-        file_path=str(file_path), file_sha256_hash=sha256, isa_table=isa_table
+        file_path=str(file_path), file_sha256_hash=sha256_hash, isa_table=isa_table
     )
     assert report.success
 
     first_column = result.isa_table_file.table.columns[0]
     result.isa_table_file.table.data[first_column][0] = "Updated Sample Name"
     # save updated content
     report = writer.save_isa_table(
@@ -245,57 +244,58 @@
     assert not report.message
 
 ```
 
 ### Multi-column filters and sort options
 ---
 * Case sensitive or case insensitive multi-column sort is supported.
-    - Multi-column sorts with ascending and descending order can be defined. For example; You can sort  by 'Parameter Value\[Gender\]' as ascending and Parameter Value\[Age\] as descending order. 
-    - Columns can be sorted as different data type. Supported sort data types are str, int, float and datetime. datetime pattern can be defined for datetime data type.
-    - Sort orders for invalid and empty values can be defined. For example, If sort value order is defined as VALID_EMPTY_INVALID, invalid values will follow empty values and empty values will follow valid values. This value order option is applicable for int, datetime and float data types. All combinations are poossible for EMPTY, INVALID, VALID values.
-    - You can define your custom sorters. "enum-sorter" as a custom sorter has been already implemented. It sorts enums with given string values.
-* There are **10 different filters** (with inverse options). Any filter can be applied to any column. Multiple filters can be defined. 
+    - Multi-column sorts can be defined with combination of ascending and descending orders. For example; You can sort 'Parameter Value\[Gender\]' by ascending and Parameter Value\[Age\] by descending order. 
+    - Columns can be sorted as different data type. Supported sort data types are: str, int, float and datetime. datetime pattern can be defined.
+    - Sort orders for invalid and empty values can also be defined. For example, If it is defined as VALID_EMPTY_INVALID, invalid values will be at the end. Empty values will follow valid values. This value order option is applicable for only int, datetime and float data types. All sort placement combinations are poossible for EMPTY, INVALID, VALID values.
+    - You can define your custom sorters. A custom "enum-sorter" sorter has been already implemented. It sorts enums with given string values.
+
+* There are **10 different filters** (plus (NOT) options of them). Any filter can be applied to any column. Multiple filters can be defined. 
     - CONTAINS / NOT CONTAINS
     - EQUAL / NOT EQUAL
     - STARTSWITH / NOT STARTSWITH
     - ENDSWITH / NOT ENDSWITH
     - GREATER / NOT GREATER
     - GREATER_EQUAL / NOT GREATER_EQUAL
     - LESS / NOT LESS
     - LESS_EQUAL / NOT LESS_EQUAL
     - REGEX (regex match) / NOT REGEX (not regex match)
     - EMPTY / NOT EMPTY (None or empty)
 * You can define multiple filters. If one filter rejects row, row will not be selected (AND operation).
 * You can define one or more columns for a filter. If there are multiple columns for a filter. If any column matches, the filter selects the row (OR operation).
-* If you do not select any column for a filter, the filter will evaluate all columns. If filter matches with any column, it will select the row. You can define column names to skip them while evaluating all rows. 
+* If you do not select any column for a filter, the filter will evaluate all columns. If filter matches with any column, it will select the row. Moreover, you can define some column names to skip them while filter is evaluating a row. 
+
 * You can define your custom filters. Some custom filters have been already implemented.
     - "between-equal": Returns row if value between given min and max. Min and max inputs can be datetime, str, int or float.
     - "valid-datetime" Return row if value is valid datetime with given pattern. Default pattern is DD/MM/YYYY.
     - "valid-number": Return row if value is valid int or float.
-    - "enum-contains": Gets a map to define a text for each enum value. Returns row if input parameter is in the enum-mapped text. Enums can be any allowed type (str, int, etc.).
-        + Example: Enum values are 1, 2, 3, 4. Enum values are mapped to 1: "In Review", 2: "Published", 3: "In Curation", 4: "Public". If parameter is "Pub", all rows contain enum value 2 and 4 will be returned.
+    - "enum-contains": Gets a map to define a text for each enum value. Returns row if input parameter is in the enum text map. Enum data typese can be any allowed type (str, int, etc.).
+        + Example: Enum values are 1, 2, 3, 4 (You store status values as in on database). Enum values are mapped to 1: "In Review", 2: "Published", 3: "In Curation", 4: "Public". If parameter is "Pub", all rows contain enum value 2 or 4 will be returned.
 
 #### Example
 Users can apply multiple filters and sort operations before retriving ISA table rows.
 
 ```python
 import pathlib
 
 from metabolights_utils.isatab import Reader
 from metabolights_utils.isatab.reader import (
     IsaTableFileReader,
-    IsaTableFileReaderResult,
+    IsaTableFileReaderResult
 )
 from metabolights_utils.models.isa.common import (
     FilterOperation,
     SortType,
     TsvFileFilterOption,
     TsvFileSortOption,
-    TsvFileSortValueOrder,
-)
+    TsvFileSortValueOrder)
 
 
 def test_with_filter_and_sort_option_01():
     # Sample Name value does not start with 'control'  and
     # Parameter Value[Chromatography Instrument] value is 'Thermo Scientific TRACE GC Ultra'.
     # Both filters are applied in case insesitive mode.
     filter_options = [
```

### Comparing `metabolights_utils-0.9.8/metabolights_utils/isatab/__init__.py` & `metabolights_utils-0.9.9/metabolights_utils/isatab/__init__.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.8/metabolights_utils/isatab/default/assignment_file.py` & `metabolights_utils-0.9.9/metabolights_utils/isatab/default/assignment_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,9 +29,9 @@
         ["^(smallmolecule_abundance_stdev_sub)$", ""],
         ["^(smallmolecule_abundance_std_error_sub)$", ""],
     ]
 
     def __init__(self, results_per_page=100) -> None:
         super().__init__(results_per_page=results_per_page)
 
-    def _get_expected_patterns(self) -> List[List[str]]:
+    def get_expected_patterns(self) -> List[List[str]]:
         return DefaultAssignmentFileReader.patterns
```

### Comparing `metabolights_utils-0.9.8/metabolights_utils/isatab/default/base_isa_file.py` & `metabolights_utils-0.9.9/metabolights_utils/isatab/default/base_isa_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,35 @@
-import os
 import pathlib
 from abc import ABC
 from io import IOBase
-from typing import Union
+from typing import Tuple, Union
 
 
 class BaseIsaFile(ABC):
     def _get_file_buffer_and_path(
         self,
         file_buffer: IOBase = None,
         file_path: Union[str, pathlib.Path] = None,
-    ) -> int:
+    ) -> Tuple[Union[str, pathlib.Path, IOBase], str]:
         if not file_buffer and not file_path:
-            ValueError("At least file buffer or file path should be defined")
+            raise ValueError("At least file buffer or file path should be defined")
 
         selected_file_buffer = (
             file_path if file_path and not file_buffer else file_buffer
         )
         selected_file_path = file_path if file_path else "<processed content>"
         return selected_file_buffer, selected_file_path
 
     def _get_file_buffer(self, file: Union[str, pathlib.Path, IOBase]) -> IOBase:
         if isinstance(file, IOBase):
             file_buffer = file
         elif isinstance(file, pathlib.Path):
             file_buffer = file.open()
         elif isinstance(file, str):
-            file_buffer = open(file=file, mode="r")
+            file_buffer = open(file=file, mode="r", encoding="utf-8")
         else:
             raise ValueError("file type is not defined")
 
         return file_buffer
 
     def _close_file(
         self,
```

### Comparing `metabolights_utils-0.9.8/metabolights_utils/isatab/default/base_isa_table_file.py` & `metabolights_utils-0.9.9/metabolights_utils/isatab/default/base_isa_table_file.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,27 +5,29 @@
 from typing import List, Union
 
 from metabolights_utils.isatab.default.base_isa_file import BaseIsaFile
 from metabolights_utils.isatab.reader import (
     IsaTableFileReader,
     IsaTableFileReaderResult,
 )
-from metabolights_utils.models.isa.parser.isa_table_parser import get_isa_table
+from metabolights_utils.models.isa.common import IsaTable, IsaTableFile
+from metabolights_utils.models.isa.parser.isa_table_parser import get_isa_table_file
 from metabolights_utils.models.parser.common import ParserMessage, ParserReport
 from metabolights_utils.models.parser.enums import ParserMessageType
 from metabolights_utils.tsv.filter import TsvFileFilterOption
 from metabolights_utils.tsv.sort import TsvFileSortOption
+from metabolights_utils.tsv.utils import calculate_sha256
 
 
 class BaseIsaTableFileReader(BaseIsaFile, IsaTableFileReader, ABC):
     def __init__(self, results_per_page=100) -> None:
         self.results_per_page = results_per_page if results_per_page > 0 else 100
 
     @abstractmethod
-    def _get_expected_patterns(self) -> List[List[str]]:
+    def get_expected_patterns(self) -> List[List[str]]:
         pass
 
     def get_total_pages(
         self,
         file_buffer: IOBase = None,
         results_per_page: int = 100,
         file_path: Union[str, pathlib.Path] = None,
@@ -40,16 +42,20 @@
     def get_total_row_count(
         self,
         file_buffer: IOBase = None,
         file_path: Union[str, pathlib.Path] = None,
     ) -> int:
         buffer_or_path, path = self._get_file_buffer_and_path(file_buffer, file_path)
 
-        isa_file_result = self.get_headers(buffer_or_path, path)
-        return isa_file_result.isa_table_file.table.total_row_count
+        isa_file_result: IsaTableFileReaderResult = self.get_headers(
+            buffer_or_path, path
+        )
+        table_file: IsaTableFile = isa_file_result.isa_table_file
+        table: IsaTable = table_file.table
+        return table.total_row_count
 
     def get_page(
         self,
         file_buffer: IOBase = None,
         page: int = 1,
         results_per_page: int = 100,
         selected_columns: Union[List[str], None] = None,
@@ -132,28 +138,33 @@
         read_messages: List[ParserMessage] = []
         try:
             buffer_or_path, path = self._get_file_buffer_and_path(
                 file_path_or_buffer, file_path
             )
             basename = os.path.basename(str(path))
             file_buffer = self._get_file_buffer(buffer_or_path)
-            isa_table = get_isa_table(
+            isa_table_file: IsaTableFile = get_isa_table_file(
                 file_buffer,
                 basename,
                 messages=read_messages,
-                expected_patterns=self._get_expected_patterns(),
+                expected_patterns=self.get_expected_patterns(),
                 offset=offset,
                 limit=limit,
                 selected_columns=selected_columns,
                 filter_options=filter_options,
                 sort_options=sort_options,
             )
+            if os.path.exists(file_path):
+                isa_table_file.sha256_hash = calculate_sha256(file_path)
+            elif os.path.exists(str(file_path_or_buffer)):
+                isa_table_file.sha256_hash = calculate_sha256(str(file_path_or_buffer))
+
         finally:
             self._close_file(buffer, file_path_or_buffer)
 
         messages = read_messages
         if skip_parser_info_messages:
             messages = [x for x in read_messages if x.type != ParserMessageType.INFO]
         parser_report = ParserReport(messages=messages)
         return IsaTableFileReaderResult(
-            isa_table_file=isa_table, parser_report=parser_report
+            isa_table_file=isa_table_file, parser_report=parser_report
         )
```

### Comparing `metabolights_utils-0.9.8/metabolights_utils/isatab/default/factory.py` & `metabolights_utils-0.9.9/metabolights_utils/isatab/default/factory.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.8/metabolights_utils/isatab/default/investigation_file.py` & `metabolights_utils-0.9.9/metabolights_utils/isatab/default/investigation_file.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+import os
 import pathlib
 import sys
 from io import IOBase
 from typing import List, Union
 
-import humps
+from pydantic.alias_generators import to_camel, to_snake
 from pydantic import BaseModel
 
 from metabolights_utils.isatab.default.base_isa_file import BaseIsaFile
 from metabolights_utils.isatab.reader import (
     InvestigationFileReader,
     InvestigationFileReaderResult,
 )
@@ -16,14 +17,20 @@
 from metabolights_utils.models.isa.investigation_file import BaseSection, Investigation
 from metabolights_utils.models.isa.investigation_file import (
     module_name as inv_module_name,
 )
 from metabolights_utils.models.isa.parser.investigation_parser import get_investigation
 from metabolights_utils.models.parser.common import ParserMessage, ParserReport
 from metabolights_utils.models.parser.enums import ParserMessageType
+from metabolights_utils.tsv.utils import calculate_sha256
+
+
+class InvestigationFileException(Exception):
+    def __init__(self, message) -> None:
+        self.message = message
 
 
 class DefaultInvestigationFileReader(InvestigationFileReader, BaseIsaFile):
     def read(
         self,
         file_buffer: IOBase = None,
         file_path: Union[str, pathlib.Path] = None,
@@ -36,17 +43,27 @@
             investigation = get_investigation(file_buffer, path, messages=read_messages)
             messages = read_messages
             if skip_parser_info_messages:
                 messages = [
                     x for x in read_messages if x.type != ParserMessageType.INFO
                 ]
             report = ParserReport(messages=messages)
-            return InvestigationFileReaderResult(
-                investigation=investigation, parser_report=report
+
+            result = InvestigationFileReaderResult(
+                investigation=investigation, parser_report=report, file_path=str(path)
             )
+
+            if pathlib.Path(path).exists():
+                result.sha256_hash = calculate_sha256(path)
+            elif (
+                isinstance(buffer_or_path, str)
+                or isinstance(buffer_or_path, pathlib.Path)
+            ) and pathlib.Path(str(buffer_or_path)).exists():
+                result.sha256_hash = calculate_sha256(str(buffer_or_path))
+            return result
         except Exception as exc:
             raise exc
         finally:
             self._close_file(file_buffer, file_path)
 
 
 class DefaultInvestigationFileWriter(InvestigationFileWriter, BaseIsaFile):
@@ -64,34 +81,39 @@
             values_in_quatation_mark=values_in_quatation_mark,
         )
         buffer_or_path, path = self._get_file_buffer_and_path(file_buffer, file_path)
         try:
             if file_buffer:
                 file_buffer.write(content)
             else:
-                with open(buffer_or_path, "w") as f:
+                with open(buffer_or_path, "w", encoding="utf-8") as f:
                     f.write(content)
-
+            report = ParserReport()
             if verify_file_after_update:
                 read_messages: List[ParserMessage] = []
-                new_investigation = get_investigation(
+                investigation = get_investigation(
                     buffer_or_path, path, messages=read_messages
                 )
                 messages = read_messages
                 if skip_parser_info_messages:
                     messages = [
                         x for x in read_messages if x.type != ParserMessageType.INFO
                     ]
                 report = ParserReport(messages=messages)
-                return InvestigationFileReaderResult(
-                    investigation=new_investigation, parser_report=report
+
+                result = InvestigationFileReaderResult(
+                    investigation=investigation,
+                    parser_report=report,
+                    file_path=str(path),
                 )
-            return InvestigationFileReaderResult(
-                investigation=investigation, parser_report=ParserReport()
-            )
+            if os.path.exists(path):
+                result.sha256_hash = calculate_sha256(path)
+            elif os.path.exists(str(buffer_or_path)):
+                result.sha256_hash = calculate_sha256(str(buffer_or_path))
+            return result
         except Exception as exc:
             raise exc
 
 
 class InvestigationFileSerializer(object):
     @classmethod
     def to_isa_file_lines(
@@ -145,65 +167,67 @@
                 cls.add_sub_section(study.section_prefix, study.study_protocols)
             )
             rows.extend(cls.add_sub_section(study.section_prefix, study.study_contacts))
         return rows
 
     @staticmethod
     def get_attribute(model, field_name):
-        model_field_name = humps.decamelize(field_name)
+        model_field_name = to_snake(field_name)
         return getattr(model, model_field_name)
 
     @classmethod
     def add_sub_section(cls, prefix, model: BaseSection):
         rows: List[List[str]] = [[model.section_header]]
         header = []
         if prefix:
             header.append(prefix)
-        data_schema = model.schema()
+        data_schema = model.model_json_schema()
         field_order = model.field_order
         if not field_order:
             field_order = []
         header_name = model.section_prefix
         if header_name:
             header.append(header_name)
 
         for field_name in field_order:
             value = cls.get_attribute(model, field_name)
-            field_key = humps.camelize(field_name)
+            field_key = to_camel(field_name)
             if isinstance(value, list):
                 properties = data_schema["properties"]
                 if "allOf" in properties[field_key] or "items" in properties[field_key]:
                     if "allOf" in "allOf" in properties[field_key]:
                         item_ref = properties[field_key]["allOf"][0]["$ref"]
                     else:
                         item_ref = properties[field_key]["items"]["$ref"]
                     default_object_name = item_ref.replace(
                         "#/definitions/", ""
                     ).replace("#/$defs/", "")
                     obj = getattr(sys.modules[inv_module_name], default_object_name)
-                    props = obj.schema()["properties"]
+                    props = obj.model_json_schema()["properties"]
                     header.append(data_schema["properties"][field_key]["header_name"])
                     sub_model_rows = cls.add_model_content(
                         " ".join(header).strip(), value, props
                     )
                     if sub_model_rows:
                         rows.extend(sub_model_rows)
             elif isinstance(value, str):
-                field_attribute = humps.decamelize(field_name)
-                header_name = model.__fields__[field_attribute].field_info.extra[
+                field_attribute = to_snake(field_name)
+                header_name = model.model_fields[field_attribute].json_schema_extra[
                     "header_name"
                 ]
                 header_name = (
                     f"{model.section_prefix} {header_name}"
                     if model.section_prefix
                     else header_name
                 )
                 rows.append([header_name, value])
             else:
-                raise Exception()
+                raise InvestigationFileException(
+                    message=f"Unsopported type {type(value)}. Value {str(value)}"
+                )
 
         cls.add_comments(model, rows)
         return rows
 
     @classmethod
     def add_comments(cls, model: BaseSection, rows: List[List[str]]):
         for comment in model.comments:
@@ -215,27 +239,27 @@
     @classmethod
     def add_model_content(cls, prefix, items: List[IsaAbstractModel], properties):
         rows = []
         row_map = {}
         fields = properties["fieldOrder"]["default"]
         for i in range(len(fields)):
             field = fields[i]
-            field_key = humps.camelize(field)
+            field_key = to_camel(field)
             header_name = properties[field_key]["header_name"]
             header_name = f"{prefix} {header_name}".strip() if prefix else header_name
             if "allOf" in properties[field_key] or "items" in properties[field_key]:
                 if "allOf" in "allOf" in properties[field_key]:
                     item_ref: str = properties[field_key]["allOf"][0]["$ref"]
                 else:
                     item_ref: str = properties[field_key]["items"]["$ref"]
                 class_name = item_ref.replace("#/definitions/", "").replace(
                     "#/$defs/", ""
                 )
                 obj: BaseModel = getattr(sys.modules[inv_module_name], class_name)
-                props = obj.schema()["properties"]
+                props = obj.model_json_schema()["properties"]
                 input_items = (
                     [cls.get_attribute(item, field_key) for item in items]
                     if items
                     else [obj()]
                 )
 
                 item_values = cls.add_model_content(header_name, input_items, props)
@@ -245,15 +269,15 @@
                     items, properties, rows, row_map, fields, i, header_name
                 )
 
         return rows
 
     @classmethod
     def assign_type(cls, items, properties, rows, row_map, fields, i, header_name):
-        field_key = humps.camelize(fields[i])
+        field_key = to_camel(fields[i])
         object_type = properties[field_key]["type"]
         if object_type == "string":
             row_map[header_name] = [header_name]
             rows.append(row_map[header_name])
             if items:
                 for item in items:
                     if isinstance(item, list):
@@ -266,8 +290,10 @@
                         row_map[header_name].append(";".join(sub_items))
                     else:
                         value = cls.get_attribute(item, field_key)
                         row_map[header_name].append(value)
             else:
                 row_map[header_name].append("")
         else:
-            raise Exception()
+            raise InvestigationFileException(
+                message=f"Invalid object type {object_type}"
+            )
```

### Comparing `metabolights_utils-0.9.8/metabolights_utils/isatab/default/writer.py` & `metabolights_utils-0.9.9/metabolights_utils/isatab/default/writer.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.8/metabolights_utils/isatab/reader.py` & `metabolights_utils-0.9.9/metabolights_utils/isatab/reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,16 @@
     isa_table_file: IsaTableFile = Field(IsaTableFile())
     parser_report: ParserReport = Field(ParserReport())
 
 
 class InvestigationFileReaderResult(MetabolightsBaseModel):
     investigation: Investigation = Field(Investigation())
     parser_report: ParserReport = Field(ParserReport())
+    file_path: str = ""
+    sha256_hash: Union[None, str] = None
 
 
 class InvestigationFileReader(ABC):
     @abstractmethod
     def read(
         self,
         file_buffer: IOBase = None,
@@ -105,43 +107,43 @@
 
     @abstractmethod
     def get_page(
         self,
         file_buffer: IOBase = None,
         page: int = 1,
         results_per_page: int = 100,
-        column_names: Union[List[str], None] = None,
+        selected_columns: Union[List[str], None] = None,
         file_path: Union[str, pathlib.Path] = None,
         filter_options: List[TsvFileFilterOption] = None,
         sort_options: List[TsvFileSortOption] = None,
     ) -> IsaTableFileReaderResult:
         """Reads file and returns the selected page of file. At least one of the file_buffer and file_path parameters should be defined.
            If file_buffer is not defined, file_path is not used to read content.
            If file_path is not defined, file path and name will not be added to messages.
 
         Args:
             file_buffer (IOBase): File buffer to read file content. io.StringIO, io.TextIOWrapper with open(), etc.
             page (int, optional): The page number requested. Defaults to 1.
             results_per_page (int, optional): Number of rows in each page. Defaults to 100.
-            column_names (Union[List[str], None], optional): Column names will be returned. Returns all columns if it is None. Defaults to None.
+            selected_columns (Union[List[str], None], optional): Column names will be returned. Returns all columns if it is None. Defaults to None.
             file_path (Union[str, pathlib.Path], optional): File path str or pathlib.Path object
             filter_options (List[TsvFileFilterOption]): filter column names and filter methods. Defaults to None.
             sort_options (List[TsvFileSortOption]): Sort column names. Defaults to None.
         Returns:
             IsaTableFileReaderResult: IsaTableFile model and parser messages
         """
 
     @abstractmethod
     def get_rows(
         self,
         file_buffer: IOBase = None,
         file_path: Union[str, pathlib.Path] = None,
         offset: int = 0,
         limit: Union[int, None] = None,
-        column_names: Union[None, List[str]] = None,
+        selected_columns: Union[None, List[str]] = None,
         filter_options: List[TsvFileFilterOption] = None,
         sort_options: List[TsvFileSortOption] = None,
     ) -> IsaTableFileReaderResult:
         """Reads file and returns rows of the file starting from offset.
            At least one of the file_buffer and file_path parameters should be defined.
            If limit is defined, size of the returned rows will be limited to this value.
 
@@ -158,30 +160,30 @@
             IsaTableFileReaderResult: IsaTableFile model and parser messages.
         """
 
     @abstractmethod
     def read(
         self,
         file_path_or_buffer: Union[str, pathlib.Path, IOBase],
+        offset: Union[None, int],
+        limit: Union[None, int],
+        selected_columns: Union[None, List[str]] = None,
         file_path: Union[str, pathlib.Path] = None,
-        offset: Union[None, int] = 0,
-        limit: Union[None, int] = 1000,
-        column_names: Union[None, List[str]] = None,
         skip_parser_info_messages: bool = True,
         filter_options: List[TsvFileFilterOption] = None,
         sort_options: List[TsvFileSortOption] = None,
     ) -> IsaTableFileReaderResult:
         """Reads selected rows with selected columns from tsv file. If sort and filter options are enabled, offset and limit are applied to the final filter and sort result.
 
         Args:
             file_path_or_buffer (Union[str, pathlib.Path, IOBase]): File buffer or path to read file content. file path str, io.StringIO, io.TextIOWrapper with open(), etc.
             file_path (Union[str, pathlib.Path], optional): File path str or pathlib.Path object. It is required if file_path_or_buffer is None. Defaults to None.
             offset (int, optional): Starting index of rows will be returned. First rows is header and index of the second row is 0. Defaults to 0.
             limit (Union[int, None], optional): Number of rows will be returned. If it is None, return all rows. Defaults to 1000.
-            column_names (Union[List[str], None], optional): Column names will be returned. Returns all columns if it is None. Defaults to None.
+            selected_columns (Union[List[str], None], optional): Column names will be returned. Returns all columns if it is None. Defaults to None.
             skip_parser_info_messages (bool, optional): clear INFO messages from parser messages. Defaults to True.
             filter_options (List[TsvFileFilterOption]): filter column names and filter methods. Defaults to None.
             sort_options (List[TsvFileSortOption]): Sort column names. Defaults to None.
         Returns:
             IsaTableFileReaderResult: IsaTableFile model and parser messages.
         """
```

### Comparing `metabolights_utils-0.9.8/metabolights_utils/isatab/writer.py` & `metabolights_utils-0.9.9/metabolights_utils/isatab/writer.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,21 +73,21 @@
         Returns:
             TsvActionReport: results of each action. If an action result is not success, result message will be available.
         """
 
 
 class IsaTabWriterFactory(ABC):
     @abstractmethod
-    def get_investigation_file_writer() -> InvestigationFileWriter:
+    def get_investigation_file_writer(self) -> InvestigationFileWriter:
         pass
 
     @abstractmethod
-    def get_assay_file_writer() -> IsaTableFileWriter:
+    def get_assay_file_writer(self) -> IsaTableFileWriter:
         pass
 
     @abstractmethod
-    def get_sample_file_writer() -> IsaTableFileWriter:
+    def get_sample_file_writer(self) -> IsaTableFileWriter:
         pass
 
     @abstractmethod
-    def get_assignment_file_writer() -> IsaTableFileWriter:
+    def get_assignment_file_writer(self) -> IsaTableFileWriter:
         pass
```

### Comparing `metabolights_utils-0.9.8/metabolights_utils/models/isa/assay_file.py` & `metabolights_utils-0.9.9/metabolights_utils/models/isa/assay_file.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.8/metabolights_utils/models/isa/common.py` & `metabolights_utils-0.9.9/metabolights_utils/models/isa/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,31 @@
 from typing import Dict, List, Union
 
-import humps
-from pydantic import BaseModel, Extra, Field
+from pydantic.alias_generators import to_snake
+from pydantic import ConfigDict, BaseModel, Field
 
 from metabolights_utils.models.common import MetabolightsBaseModel
 from metabolights_utils.models.isa.enums import ColumnsStructure
 from metabolights_utils.tsv.filter import TsvFileFilterOption
 from metabolights_utils.tsv.sort import TsvFileSortOption
 
+INVESTIGATION_FILE_SECTION_NAMES = {
+    "ONTOLOGY SOURCE REFERENCE",
+    "INVESTIGATION",
+    "INVESTIGATION PUBLICATIONS",
+    "INVESTIGATION CONTACTS",
+    "STUDY",
+    "STUDY DESIGN DESCRIPTORS",
+    "STUDY PUBLICATIONS",
+    "STUDY FACTORS",
+    "STUDY ASSAYS",
+    "STUDY PROTOCOLS",
+    "STUDY CONTACTS",
+}
+
 INVESTIGATION_FILE_INITIAL_ROWS = [
     "ONTOLOGY SOURCE REFERENCE",
     "Term Source Name",
     "Term Source File",
     "Term Source Version",
     "Term Source Description",
     "INVESTIGATION",
@@ -107,35 +121,33 @@
 
 INVESTIGATION_FILE_INITIAL_ROWS_SET = set(INVESTIGATION_FILE_INITIAL_ROWS)
 INVESTIGATION_FILE_STUDY_ROWS_SET = set(INVESTIGATION_FILE_STUDY_ROWS)
 
 
 class IsaAbstractModel(MetabolightsBaseModel):
     field_order: Union[None, List[str]] = Field(None, auto_fill=False)
-
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     @classmethod
     def get_attribute(cls, model: BaseModel, attribute_name):
-        model_attribute_key = humps.decamelize(attribute_name)
+        model_attribute_key = to_snake(attribute_name)
         return getattr(model, model_attribute_key)
 
     @classmethod
     def is_empty_model(cls, model: BaseModel):
-        schema = model.schema()
+        schema = model.model_json_schema()
         for item_key in schema["properties"]:
             item_field_definition = schema["properties"][item_key]
             if (
                 not item_field_definition
                 or "auto_fill" not in item_field_definition
                 or not item_field_definition["auto_fill"]
             ):
                 continue
-            model_attribute_key = humps.decamelize(item_key)
+            model_attribute_key = to_snake(item_key)
             item_val = cls.get_attribute(model, model_attribute_key)
             if isinstance(item_val, IsaAbstractModel):
                 is_empty = IsaAbstractModel.is_empty_model(item_val)
                 if not is_empty:
                     return False
             elif item_val:
                 return False
@@ -269,15 +281,15 @@
 
 class Comment(IsaAbstractModel):
     name: str = ""
     value: List[str] = []
 
 
 class IsaTableColumn(IsaAbstractModel):
-    column_index: Union[int, str] = ""
+    column_index: Union[int, None] = None
     column_name: str = ""
     column_header: str = ""
     additional_columns: List[str] = []
     column_category: str = ""
     colummn_structure: ColumnsStructure = ColumnsStructure.SINGLE_COLUMN
     column_prefix: str = ""
     column_search_pattern: str = ""
@@ -300,8 +312,11 @@
     total_column_count: int = 0
     filter_options: List[TsvFileFilterOption] = []
     sort_options: List[TsvFileSortOption] = []
 
 
 class IsaTableFile(IsaAbstractModel):
     file_path: str = ""
+    sha256_hash: str = (
+        "e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855"
+    )
     table: IsaTable = Field(IsaTable())
```

### Comparing `metabolights_utils-0.9.8/metabolights_utils/models/isa/investigation_file.py` & `metabolights_utils-0.9.9/metabolights_utils/models/isa/investigation_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from typing import List
 
-from pydantic import Field
+from pydantic import ConfigDict, Field
 
 from metabolights_utils.models.isa.common import Comment, IsaAbstractModel
 
 module_name = __name__
 
 
 class BaseSection(IsaAbstractModel):
     section_header: str = Field("ONTOLOGY SOURCE REFERENCE", exclude=True)
     section_prefix: str = Field("", exclude=True)
 
     comments: List[Comment] = []
-
-    class Config:
-        field_order: List[str] = []
+    model_config = ConfigDict()
 
 
 class OntologySourceReference(IsaAbstractModel):
     field_order: List[str] = [
         "source_name",
         "source_file",
         "source_version",
```

### Comparing `metabolights_utils-0.9.8/metabolights_utils/models/isa/parser/common.py` & `metabolights_utils-0.9.9/metabolights_utils/models/isa/parser/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,15 @@
 from metabolights_utils.models.isa.common import (
     INVESTIGATION_FILE_INITIAL_ROWS_SET,
     INVESTIGATION_FILE_STUDY_ROWS_SET,
 )
 from metabolights_utils.models.parser.common import ParserMessage
 from metabolights_utils.models.parser.enums import ParserMessageType
 from metabolights_utils.tsv.filter import Filter, FilterRegistry, TsvFileFilterOption
-from metabolights_utils.tsv.sort import (
-    Sorter,
-    SorterRegistry,
-    TsvFileSortOption,
-    TsvSortException,
-)
+from metabolights_utils.tsv.sort import Sorter, SorterRegistry, TsvFileSortOption
 
 
 def read_investigation_file(file_buffer: IOBase, messages: List[ParserMessage]):
     new_lines = read_investigation_file_lines(file_buffer, messages)
     dict_format = {}
     for i in range(len(new_lines)):
         detail = {}
@@ -136,17 +131,17 @@
     column_header: str = ""
     rows: Dict[int, str] = {}
 
 
 class SelectedTsvFileContent(MetabolightsBaseModel):
     columns: List[TsvColumn] = []
     total_rows: int = 0
-    total_filtered_rows = 0
-    offset = 0
-    limit = 0
+    total_filtered_rows: int = 0
+    offset: int = 0
+    limit: int = 0
     selected_column_count: int = 0
     total_columns: int = 0
     filter_options: List[TsvFileFilterOption] = []
     sort_options: List[TsvFileSortOption] = []
 
 
 def read_table_file(
@@ -236,15 +231,15 @@
                         row,
                         row_index - 1,
                         columns,
                         selected_column_indices=selected_column_indices,
                     )
     except Exception as exc:
         message = ParserMessage(type=ParserMessageType.CRITICAL)
-        message.short = f"ISA table file can not be read successfully."
+        message.short = "ISA table file can not be read successfully."
         message.detail = f"Returned result is not complete. {str(exc)}"
         messages.append(message)
         return SelectedTsvFileContent()
     return content
 
 
 def read_table_file_with_filter_and_sort_option(
@@ -282,31 +277,31 @@
                 if filter_options:
                     for filter_option in filter_options:
                         filter_option.search_columns = (
                             filter_option.search_columns
                             if filter_option.search_columns
                             else []
                         )
-                        filter: Filter = FilterRegistry.get_filter(
+                        selected_filter: Filter = FilterRegistry.get_filter(
                             filter_option, column_name_indices, column_indices
                         )
-                        filters.append(filter)
+                        filters.append(selected_filter)
                     # empty search column filters will be moved to end
                     filters.sort(
                         key=lambda x: len(x.filter_option.search_columns)
                         if x.filter_option.search_columns
                         else sys.maxsize
                     )
             else:
                 if not filter_options:
                     filtered_rows.append((row_index - 1, row))
                 else:
                     select: bool = True
-                    for filter in filters:
-                        select = filter.filter(row)
+                    for selected_filter in filters:
+                        select = selected_filter.filter(row)
                         if not select:
                             break
                     if select:
                         filtered_rows.append((row_index - 1, row))
         reader = None
 
         sorters: List[Sorter] = []
@@ -361,15 +356,15 @@
                     row,
                     data_row_index,
                     columns,
                     selected_column_indices=selected_column_indices,
                 )
     except Exception as exc:
         message = ParserMessage(type=ParserMessageType.CRITICAL)
-        message.short = f"ISA table file can not be read successfully."
+        message.short = "ISA table file can not be read successfully."
         message.detail = f"Returned result is not complete. {str(exc)}"
         messages.append(message)
     return content
 
 
 def add_tsv_file_data_row(
     data_row,
@@ -422,35 +417,40 @@
                 invalid_column_names.append(name)
                 continue
             else:
                 new_ordered_columns.append(name)
                 col_index = column_name_indices[name]
                 term_source_relative_index = 1
                 if col_index + 1 < len(header_row):
-                    next: str = column_indices[col_index + 1]
-                    if next == "Unit" or next.startswith("Unit."):
-                        new_ordered_columns.append(next)
+                    next_item: str = column_indices[col_index + 1]
+                    if next_item == "Unit" or next_item.startswith("Unit."):
+                        new_ordered_columns.append(next_item)
                         term_source_relative_index = 2
 
                 if col_index + term_source_relative_index + 1 < len(header_row):
-                    next: str = column_indices[col_index + term_source_relative_index]
-                    if next == "Term Source REF" or next.startswith("Term Source REF."):
-                        new_ordered_columns.append(next)
-                        next: str = column_indices[
+                    next_item: str = column_indices[
+                        col_index + term_source_relative_index
+                    ]
+                    if next_item == "Term Source REF" or next_item.startswith(
+                        "Term Source REF."
+                    ):
+                        new_ordered_columns.append(next_item)
+                        next_item: str = column_indices[
                             col_index + term_source_relative_index + 1
                         ]
-                        if next == "Term Accession Number" or next.startswith(
-                            "Term Accession Number."
+                        if (
+                            next_item == "Term Accession Number"
+                            or next_item.startswith("Term Accession Number.")
                         ):
-                            new_ordered_columns.append(next)
+                            new_ordered_columns.append(next_item)
         selected_column_names.clear()
         selected_column_names.extend(new_ordered_columns)
     if invalid_column_names:
         raise TypeError(
-            f"Column(s) do(es) not exist: " + ", ".join(invalid_column_names)
+            "Column(s) do(es) not exist: " + ", ".join(invalid_column_names)
         )
 
 
 def read_tsv_file_header(
     content: SelectedTsvFileContent,
     header_row,
     column_names: Union[None, List[str]],
```

### Comparing `metabolights_utils-0.9.8/metabolights_utils/models/isa/parser/investigation_parser.py` & `metabolights_utils-0.9.9/metabolights_utils/models/isa/parser/investigation_parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,22 @@
-import os
+import pathlib
 import re
 import sys
 from io import IOBase
 from typing import Dict, List, Tuple, Union
 
-import humps
+from pydantic.alias_generators import to_snake
 from pydantic import BaseModel
 
 from metabolights_utils.models.isa import investigation_file as model
 from metabolights_utils.models.isa.common import (
+    INVESTIGATION_FILE_INITIAL_ROWS,
     INVESTIGATION_FILE_INITIAL_ROWS_SET,
+    INVESTIGATION_FILE_SECTION_NAMES,
+    INVESTIGATION_FILE_STUDY_ROWS,
     INVESTIGATION_FILE_STUDY_ROWS_SET,
     Comment,
     IsaAbstractModel,
 )
 from metabolights_utils.models.isa.parser.common import read_investigation_file
 from metabolights_utils.models.parser.common import ParserMessage
 from metabolights_utils.models.parser.enums import ParserMessageType
@@ -21,32 +24,33 @@
 model_module_name = model.__name__
 
 
 def parse_investigation_from_fs(
     file_path: str,
 ) -> Tuple[Union[model.Investigation, None], List[ParserMessage]]:
     messages: List[ParserMessage] = []
-    basename = os.path.basename(file_path)
-    if not os.path.exists(file_path):
+    file = pathlib.Path(file_path)
+    basename = pathlib.Path(file).name
+    if not file.exists():
         print(f"File does not exist: {basename}")
         message = ParserMessage(
             short="File does not exist", type=ParserMessageType.CRITICAL
         )
         message.detail = f"File does not exist: {basename}"
         messages.append(message)
         return None, messages
-    file_size = os.stat(file_path).st_size
+    file_size = file.stat().st_size
     if file_size == 0:
         print(f"File is empty: {basename}")
         message = ParserMessage(short="File is empty", type=ParserMessageType.CRITICAL)
         message.detail = f"File is empty: {basename}"
         messages.append(message)
         return None, messages
 
-    with open(file_path, "r") as f:
+    with open(file_path, "r", encoding="utf-8") as f:
         investigation = get_investigation(f, file_path, messages=messages)
         return investigation, messages
 
 
 def get_investigation(
     file_buffer: IOBase, file_path: str, messages: List[ParserMessage]
 ):
@@ -238,14 +242,45 @@
     file_path,
     index_map: dict,
     content: dict,
     comments_map: dict,
     messages: Union[None, List[ParserMessage]] = None,
 ):
     study: model.Study = model.Study()
+
+    missing_rows = [
+        x
+        for x in INVESTIGATION_FILE_STUDY_ROWS
+        if x not in index_map and x not in INVESTIGATION_FILE_SECTION_NAMES
+    ]
+    if missing_rows:
+        message = ParserMessage(
+            short=f"Some rows are missing for study: {', '.join(missing_rows)}",
+            type=ParserMessageType.CRITICAL,
+        )
+        message.detail = "Investigation file is not complete."
+        messages.append(message)
+        return study, messages
+    extra_rows = [
+        x
+        for x in index_map
+        if x not in INVESTIGATION_FILE_STUDY_ROWS
+        and not x.lower().startswith(
+            "comment[" and x not in INVESTIGATION_FILE_SECTION_NAMES
+        )
+    ]
+    if extra_rows:
+        row_messages = ", ".join([f"Line {index_map[x]}:{x}" for x in extra_rows])
+        message = ParserMessage(
+            short=f"Some rows are missing for study: {row_messages}",
+            type=ParserMessageType.CRITICAL,
+        )
+        message.detail = "Investigation file has unexpected rows."
+        messages.append(message)
+
     assign_by_field_name(
         file_path,
         study,
         index_map,
         content,
         comments_map=comments_map,
         messages=messages,
@@ -259,28 +294,60 @@
     content: dict,
     studies: List[model.Study],
     comments_map: dict,
     messages: Union[None, List[ParserMessage]] = None,
 ):
     messages = messages if messages is not None else []
     investigation: model.Investigation = model.Investigation()
+
+    missing_rows = [
+        x
+        for x in INVESTIGATION_FILE_INITIAL_ROWS
+        if x not in index_map and x not in INVESTIGATION_FILE_SECTION_NAMES
+    ]
+    if missing_rows:
+        message = ParserMessage(
+            short=f"Some rows are missing for investigation: {', '.join(missing_rows)}",
+            type=ParserMessageType.CRITICAL,
+        )
+        message.detail = "Investigation file is not complete."
+        messages.append(message)
+        return investigation, messages
+
+    extra_rows = [
+        x
+        for x in index_map
+        if x not in INVESTIGATION_FILE_INITIAL_ROWS
+        and not x.lower().startswith(
+            "comment[" and x not in INVESTIGATION_FILE_SECTION_NAMES
+        )
+    ]
+    if extra_rows:
+        row_messages = ", ".join([f"Line {index_map[x]}:{x}" for x in extra_rows])
+        message = ParserMessage(
+            short=f"Some rows are missing for study: {row_messages}",
+            type=ParserMessageType.CRITICAL,
+        )
+        message.detail = "Investigation file has unexpected lines."
+        messages.append(message)
+
     assign_by_field_name(
         file_path,
         investigation,
         index_map,
         content,
         comments_map=comments_map,
         messages=messages,
     )
     investigation.studies = studies
     return investigation, messages
 
 
 def set_value(obj, key, value):
-    camel_key = humps.decamelize(key)
+    camel_key = to_snake(key)
     setattr(obj, camel_key, value)
 
 
 def assign_by_field_name(
     file_path,
     data: BaseModel,
     index_map: dict,
@@ -288,15 +355,15 @@
     messages: List[ParserMessage],
     prefix="",
     value_index=1,
     comments_map=None,
 ) -> None:
     if messages is None:
         messages = []
-    data_schema = data.schema()
+    data_schema = data.model_json_schema()
     if "properties" not in data_schema or not data_schema["properties"]:
         print(f"Properties are not defined in {file_path}")
         message = ParserMessage(
             short="Property is not defined for object", type=ParserMessageType.WARNING
         )
         message.detail = f"{data.__repr_name__} values will not assigned."
         messages.append(message)
@@ -403,25 +470,25 @@
                         if search_field not in index_map:
                             print(
                                 f"{search_field} is not in file. Skipping {field_name} in {file_path}"
                             )
                             continue
                         index = index_map[search_field]
 
-                        max = len(tab[index])
+                        max_index = len(tab[index])
                         ref_class_name = (
                             items["$ref"]
                             .replace("#/definitions/", "")
                             .replace("#/$defs/", "")
                         )
                         ref_class = getattr(
                             sys.modules[model_module_name],
                             ref_class_name,
                         )
-                        for i in range(1, max):
+                        for i in range(1, max_index):
                             instance = ref_class()
                             item_list.append(instance)
                             assign_by_field_name(
                                 file_path,
                                 instance,
                                 index_map,
                                 tab,
@@ -459,15 +526,15 @@
                             index_map,
                             tab,
                             prefix=field_name,
                             value_index=value_index,
                             messages=messages,
                             comments_map=comments_map,
                         )
-                        item_schema = instance.schema()
+                        item_schema = instance.model_json_schema()
 
                         new_instances = []
                         separator = ";"
                         for item_key in item_schema["properties"]:
                             item_field_definition = item_schema["properties"][item_key]
                             if (
                                 not item_field_definition
@@ -476,15 +543,15 @@
                             ):
                                 continue
                             if (
                                 "seperator" in item_field_definition
                                 and item_field_definition["seperator"]
                             ):
                                 separator = item_field_definition["seperator"]
-                            attribute_key = humps.decamelize(item_key)
+                            attribute_key = to_snake(item_key)
                             item_val = getattr(instance, attribute_key) or ""
                             seperated_values = item_val.split(separator)
                             for _ in range(len(seperated_values)):
                                 instance_count = len(new_instances)
                                 values_count = len(seperated_values)
                                 if instance_count < values_count:
                                     for _ in range(instance_count, values_count):
```

### Comparing `metabolights_utils-0.9.8/metabolights_utils/models/isa/parser/isa_table_parser.py` & `metabolights_utils-0.9.9/metabolights_utils/models/isa/parser/isa_table_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     SelectedTsvFileContent,
     TsvFileFilterOption,
     read_table_file,
 )
 from metabolights_utils.models.parser.common import ParserMessage
 from metabolights_utils.models.parser.enums import ParserMessageType
 from metabolights_utils.tsv.sort import TsvFileSortOption
+from metabolights_utils.tsv.utils import calculate_sha256
 
 
 def parse_isa_table_sheet_from_fs(
     file_path: str,
     expected_patterns: Union[None, List[List[str]]] = None,
     selected_columns: Union[None, List[str]] = None,
     offset: Union[int, None] = None,
@@ -53,75 +54,79 @@
     if file_size == 0:
         message = ParserMessage(short="File is empty", type=ParserMessageType.CRITICAL)
         message.detail = f"File is empty: {basename} in {dirname}"
         messages.append(message)
         return IsaTableFile(), messages
     basename = os.path.basename(file_path)
 
-    with open(file_path, "r") as f:
+    with open(file_path, "r", encoding="utf-8") as f:
         read_messages: List[ParserMessage] = []
-        isa_table: IsaTableFile = get_isa_table(
+        isa_table_file: IsaTableFile = get_isa_table_file(
             f,
             basename,
             messages=read_messages,
             expected_patterns=expected_patterns,
             selected_columns=selected_columns,
             offset=offset,
             limit=limit,
             filter_options=filter_options,
             sort_options=sort_options,
         )
-        if isa_table.table.columns:
-            messages.extend(read_messages)
-            messages = [x for x in messages if x.type != ParserMessageType.INFO]
-            return isa_table, messages
+    if os.path.exists(file_path):
+        isa_table_file.sha256_hash = calculate_sha256(file_path)
+    if isa_table_file.table.columns:
+        messages.extend(read_messages)
+        messages = [x for x in messages if x.type != ParserMessageType.INFO]
+        return isa_table_file, messages
 
-    with open(file_path, "r", errors="backslashreplace") as f:
+    with open(file_path, "r", errors="ignore", encoding="utf-8") as f:
         read_messages: List[ParserMessage] = []
-        isa_table = get_isa_table(
+        isa_table_file: IsaTableFile = get_isa_table_file(
             f,
             basename,
             messages=read_messages,
             expected_patterns=expected_patterns,
             selected_columns=selected_columns,
             offset=offset,
             limit=limit,
             filter_options=filter_options,
             sort_options=sort_options,
         )
-        isa_table.file_path = basename
+    isa_table_file.file_path = basename
+    if os.path.exists(file_path):
+        isa_table_file.sha256_hash = calculate_sha256(file_path)
 
-        if isa_table.table.columns:
-            message = ParserMessage(
-                short="File is read utf-8 encoding and invalid characters errors are replaced with backslash",
-                type=ParserMessageType.WARNING,
-            )
-            message.detail = (
-                "Invalid characters are replaced with backslash characters: "
-                + f"{basename} in {dirname}"
-            )
-            messages.append(message)
-            messages.extend(read_messages)
-            messages = [x for x in messages if x.type != ParserMessageType.INFO]
-            return isa_table, messages
+    if isa_table_file.table.columns:
+        message = ParserMessage(
+            short="File is read utf-8 encoding and invalid characters errors are replaced with backslash",
+            type=ParserMessageType.WARNING,
+        )
+        message.detail = (
+            "Invalid characters are replaced with backslash characters: "
+            + f"{basename} in {dirname}"
+        )
+        messages.append(message)
+        messages.extend(read_messages)
+        messages = [x for x in messages if x.type != ParserMessageType.INFO]
+        return isa_table_file, messages
     messages = [x for x in messages if x.type != ParserMessageType.INFO]
-    return isa_table, messages
+    return isa_table_file, messages
 
 
-def get_isa_table(
+def get_isa_table_file(
     file_path_or_buffer: IOBase,
     file_name: str,
     messages: List[ParserMessage],
     expected_patterns: List[List[str]],
     selected_columns: Union[None, List[str]] = None,
     offset: Union[int, None] = None,
     limit: Union[int, None] = None,
     filter_options: List[TsvFileFilterOption] = None,
     sort_options: List[TsvFileSortOption] = None,
-):
+) -> IsaTableFile:
     study_table = IsaTableFile()
     if messages is None:
         messages = []
     if not expected_patterns:
         expected_patterns = []
     file_path_or_buffer.seek(0)
     content: SelectedTsvFileContent = read_table_file(
@@ -147,29 +152,28 @@
 def update_isa_table_file(
     study_table: IsaTableFile,
     content: SelectedTsvFileContent,
     file_name: str,
     messages: List[ParserMessage],
     expected_patterns,
 ):
-    # columns = list(df.columns)
     columns = [x.column_name for x in content.columns]
     column_indices = {x.column_name: x.column_index for x in content.columns}
     first_column_name = None
     for column_name in columns:
         if not first_column_name:
             first_column_name = column_name
         cleaned_column_name = get_cleaned_header(column_name)
 
         if not len(cleaned_column_name.strip()) or len(cleaned_column_name) != len(
             cleaned_column_name.strip()
         ):
             message = ParserMessage(type=ParserMessageType.ERROR)
             column_index = column_indices[column_name]
-            message.column = str(column_index)
+            message.column = column_index
             if len(cleaned_column_name.strip()) > 0:
                 message.short = "Column header starts or ends with space"
                 message.detail = (
                     f"'{column_name}' header at column {column_index + 1} "
                     + "ends or starts with space."
                 )
             else:
@@ -202,77 +206,76 @@
         column.column_index for column in content.columns
     ]
     # data = df.to_dict(orient="list")
     study_table.table.data = filtered_data
     study_table.table.columns = columns
     # study_table.table.row_count = len(content.columns[0].rows)
     study_table.file_path = file_name
-
     return study_table
 
 
 MULTI_COLUMN_TEMPLATES = {
     ColumnsStructure.ONTOLOGY_COLUMN: {
         "column_names": [
             IsaTableAdditionalColumn.TERM_SOURCE_REF,
             IsaTableAdditionalColumn.TERM_ACCSSION_NUMBER,
         ],
         "searchPatterns": [
-            "(Term Source REF)(\.\d+)?",
-            "(Term Accession Number)(\.\d+)?",
+            r"(Term Source REF)(\.\d+)?",
+            r"(Term Accession Number)(\.\d+)?",
         ],
     },
     ColumnsStructure.SINGLE_COLUMN_AND_UNIT_ONTOLOGY: {
         "column_names": [
             IsaTableAdditionalColumn.UNIT,
             IsaTableAdditionalColumn.TERM_SOURCE_REF,
             IsaTableAdditionalColumn.TERM_ACCSSION_NUMBER,
         ],
         "searchPatterns": [
-            "(Unit)(\.\d+)?",
-            "(Term Source REF)(\.\d+)?",
-            "(Term Accession Number)(\.\d+)?",
+            r"(Unit)(\.\d+)?",
+            r"(Term Source REF)(\.\d+)?",
+            r"(Term Accession Number)(\.\d+)?",
         ],
     },
 }
 
 additional_column_templates = [
     MULTI_COLUMN_TEMPLATES[ColumnsStructure.SINGLE_COLUMN_AND_UNIT_ONTOLOGY][
         "searchPatterns"
     ],
     MULTI_COLUMN_TEMPLATES[ColumnsStructure.ONTOLOGY_COLUMN]["searchPatterns"],
 ]
 
-additional_column_headers = [
+ADDITIONAL_COLUMN_HEADERS = [
     MULTI_COLUMN_TEMPLATES[ColumnsStructure.SINGLE_COLUMN_AND_UNIT_ONTOLOGY][
         "column_names"
     ],
     MULTI_COLUMN_TEMPLATES[ColumnsStructure.ONTOLOGY_COLUMN]["column_names"],
 ]
 
 multiple_columns_additional_header_patterns = MULTI_COLUMN_TEMPLATES[
     ColumnsStructure.SINGLE_COLUMN_AND_UNIT_ONTOLOGY
 ]["searchPatterns"]
 
 
 samples_file_expected_patterns = [
     [r"^(Source Name)$", ""],
-    [r"^Characteristics[(\w[ -~]*)]$", "Characteristics"],
-    [r"^(Protocol REF)(.\d+)?$", "Protocol"],
+    [r"^Characteristics\[(\w[ -~]*)\]$", "Characteristics"],
+    [r"^(Protocol REF)(\.\d+)?$", "Protocol"],
     [r"^(Sample Name)$", ""],
-    [r"^Factor Value[(\w[ -~]*)]$", "Factor Value"],
-    [r"^Comment\b[(\w{1}[ -~]*)]$", "Comment"],
+    [r"^Factor Value\[(\w[ -~]*)\]$", "Factor Value"],
+    [r"^Comment\b\[(\w{1}[ -~]*)\]$", "Comment"],
 ]
 
 assay_file_expected_patterns = [
     [r"^(Extract Name)$", ""],
-    [r"^(Protocol REF)(.\d+)?$", "Protocol"],
+    [r"^(Protocol REF)(\.\d+)?$", "Protocol"],
     [r"^(Sample Name)$", ""],
-    [r"^Parameter Value[(\w[ -~]*)]$", "Parameter Value"],
-    [r"^Comment\b[(\w{1}[ -~]*)]$", "Comment"],
+    [r"^[ ]*Parameter[ ]+Value[ ]*\[[ ]*(\w[ -~]*)[ ]*\][ ]*$", "Parameter Value"],
+    [r"^Comment\b\[(\w{1}[ -~]*)\]$", "Comment"],
     [r"^(Labeled Extract Name)$", ""],
     [r"^(Label)$", ""],
 ]
 
 
 def get_cleaned_header(column_name):
     cleaned_column_name = column_name
@@ -288,15 +291,15 @@
 def get_headers(columns: List[str], expected_patterns, messages: List[ParserMessage]):
     headers = []
     column_index = 0
     columns_count = len(columns)
     while column_index < columns_count:
         column_name = columns[column_index]
         cleaned_column_name = get_cleaned_header(column_name)
-        column_structure, additional_column_headers = define_column_structure(
+        column_structure, defined_additional_column_headers = define_column_structure(
             column_index, columns
         )
 
         result = None
         pattern_index = -1
         expected_header: bool = False
         message = ParserMessage(type=ParserMessageType.INFO)
@@ -304,15 +307,15 @@
             result = re.search(expected_patterns[i][0], column_name)
             if result and result.groups():
                 pattern_index = i
                 expected_header = result and result.groups()
                 break
 
         column = IsaTableColumn(
-            column_index=str(column_index), colummn_structure=column_structure
+            column_index=column_index, colummn_structure=column_structure
         )
         column.column_name = column_name
         column.column_header = cleaned_column_name
         linked_columns = []
 
         if column_structure == ColumnsStructure.ADDITIONAL_COLUMN:
             column.column_category = "Additional"
@@ -337,21 +340,21 @@
                 cleaned_column_name,
                 pattern_index,
                 expected_header,
                 message,
                 column,
             )
         else:
-            column.additional_columns = additional_column_headers
+            column.additional_columns = defined_additional_column_headers
             additional_column_index = column_index
 
             for additional_column in column.additional_columns:
                 additional_column_index = additional_column_index + 1
                 linked_column = IsaTableColumn(
-                    column_index=str(additional_column_index),
+                    column_index=additional_column_index,
                     colummn_structure=ColumnsStructure.LINKED_COLUMN,
                 )
                 linked_column.column_header = additional_column
                 linked_column.column_category = "Linked Column"
                 linked_column.column_name = columns[additional_column_index]
                 linked_columns.append(linked_column)
 
@@ -359,27 +362,29 @@
                 expected_patterns,
                 cleaned_column_name,
                 pattern_index,
                 expected_header,
                 message,
                 column,
             )
-            column_index = column_index + len(additional_column_headers)
+            column_index = column_index + len(defined_additional_column_headers)
 
         headers.append(column)
         if linked_columns:
             headers.extend(linked_columns)
 
         update_message(messages, column_index, message, column)
 
         column_index = column_index + 1
     return headers
 
 
-def update_message(messages, column_index, message, column):
+def update_message(
+    messages, column_index, message: ParserMessage, column: IsaTableColumn
+):
     if not message.detail:
         column_message = " ".join(
             [
                 f"Column {(column.column_index + 1):03}: '{column.column_category}' column",
                 f"column name: '{column.column_header}'",
             ]
         )
@@ -496,23 +501,23 @@
 
     return ColumnsStructure.SINGLE_COLUMN, []
 
 
 def select_additional_columns(column_index, columns: List[str]):
     for i in range(len(additional_column_templates)):
         template = additional_column_templates[i]
-        next = column_index + 1
+        next_item = column_index + 1
         maximum_match = 0
         matched = True
         internal_index = 0
         for pattern in template:
-            if next >= len(columns) or not re.match(pattern, columns[next]):
+            if next_item >= len(columns) or not re.match(pattern, columns[next_item]):
                 matched = False
                 break
-            next = next + 1
+            next_item = next_item + 1
             internal_index = internal_index + 1
             if maximum_match < internal_index:
                 maximum_match = internal_index
 
         if matched:
-            return additional_column_headers[i], maximum_match
+            return ADDITIONAL_COLUMN_HEADERS[i], maximum_match
     return [], maximum_match
```

### Comparing `metabolights_utils-0.9.8/metabolights_utils/models/metabolights/metabolights_study.py` & `metabolights_utils-0.9.9/metabolights_utils/models/metabolights/metabolights_study.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.8/metabolights_utils/models/parser/common.py` & `metabolights_utils-0.9.9/metabolights_utils/models/parser/common.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.8/metabolights_utils/tsv/actions/add_column.py` & `metabolights_utils-0.9.9/metabolights_utils/tsv/actions/add_column.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,20 +30,20 @@
         cell_default_values: Dict[int, str] = (
             action.cell_default_values if action.cell_default_values else {}
         )
 
         column_indices: List[int] = list(column_data.keys()).copy()
         column_indices.sort()
 
-        if action.id:
+        if not action.id:
             uuid_value = str(uuid.uuid4().hex)
             action.id = uuid_value
 
         try:
-            with open(source_file_path, "r") as source:
+            with open(source_file_path, "r", encoding="utf-8") as source:
                 header_line = source.readline()
                 header_names = header_line.strip().split("\t")
                 for column_idx in column_indices:
                     if column_idx < 0:
                         column_idx = len(header_names)
                     default_value = (
                         cell_default_values[column_idx]
@@ -55,15 +55,15 @@
                     if not value or not value.header_name:
                         result.message = (
                             f"There is not header name for column index {column_idx}"
                         )
                         return result
                     header_names.insert(column_idx, value.header_name)
 
-                with open(target_file_path, "w") as target:
+                with open(target_file_path, "w", encoding="utf-8") as target:
                     self.write_row(target, header_names)
                     row_index = 0
                     for line in source:
                         row = line.strip().split("\t")
                         for column_idx in column_indices:
                             default_value = (
                                 cell_default_values[column_idx]
```

### Comparing `metabolights_utils-0.9.8/metabolights_utils/tsv/actions/add_row.py` & `metabolights_utils-0.9.9/metabolights_utils/tsv/actions/add_row.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,25 +28,25 @@
         row_data: Dict[int, model.TsvRowData] = (
             action.row_data if action.row_data else {}
         )
 
         row_indices = target_row_indices.copy()
         row_indices.sort()
 
-        if action.id:
+        if not action.id:
             uuid_value = str(uuid.uuid4().hex)
             action.id = uuid_value
 
         try:
-            with open(source_file_path, "r") as source:
+            with open(source_file_path, "r", encoding="utf-8") as source:
                 header_line = source.readline()
                 header_names = header_line.strip().split("\t")
                 empty_row = [""] * len(header_names)
 
-                with open(target_file_path, "w") as target:
+                with open(target_file_path, "w", encoding="utf-8") as target:
                     self.write_row(target, header_names)
                     row_index = -1
                     for line in source:
                         row_index += 1
                         if row_index in row_indices:
                             while row_index in row_indices:
                                 input_row = (
```

### Comparing `metabolights_utils-0.9.8/metabolights_utils/tsv/actions/base.py` & `metabolights_utils-0.9.9/metabolights_utils/tsv/actions/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     def __init__(self, message: str) -> None:
         self.message = message
 
 
 class BaseTsvAction(ABC):
     @abstractmethod
     def apply_action(
+        self,
         source_file_path: pathlib.Path,
         target_file_path: pathlib.Path,
         action: actions.TsvAction,
     ) -> actions.TsvActionResult:
         pass
 
     def delete_file(self, path):
```

### Comparing `metabolights_utils-0.9.8/metabolights_utils/tsv/actions/copy_column.py` & `metabolights_utils-0.9.9/metabolights_utils/tsv/actions/update_column.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,81 +2,87 @@
 import uuid
 from typing import Dict, List
 
 from metabolights_utils.tsv import model as actions
 from metabolights_utils.tsv.actions.base import BaseTsvAction
 
 
-class CopyColumnTsvAction(BaseTsvAction):
+class UpdateColumnsTsvAction(BaseTsvAction):
     def apply_action(
         self,
         source_file_path: pathlib.Path,
         target_file_path: pathlib.Path,
-        action: actions.TsvCopyColumnAction,
+        action: actions.TsvUpdateColumnsAction,
     ) -> actions.TsvActionResult:
         result: actions.TsvActionResult = actions.TsvActionResult(action=action)
-        if action.type != actions.TsvActionType.COPY_COLUMN:
+        if action.type != actions.TsvActionType.UPDATE_COLUMN_DATA:
             result.message = "Action name is not valid"
             return result
 
-        action: actions.TsvCopyColumnAction = action
-        source_column_index = action.source_column_index
-        source_column_header = action.source_column_header
-
-        columns: Dict[int, str] = action.target_columns if action.target_columns else {}
-        selected_row_indices = (
-            set(action.selected_row_indices) if action.selected_row_indices else None
+        action: actions.TsvUpdateColumnsAction = action
+
+        columns: Dict[int, actions.TsvColumnData] = (
+            action.columns if action.columns else {}
         )
+
         if not columns:
             result.message = "There is not target column index"
             return result
 
         column_indices: List[int] = list(columns.keys()).copy()
         column_indices.sort()
 
-        if action.id:
+        if not action.id:
             uuid_value = str(uuid.uuid4().hex)
             action.id = uuid_value
 
         try:
-            with open(source_file_path, "r") as source:
+            with open(source_file_path, "r", encoding="utf-8") as source:
                 header_line = source.readline()
                 header_names = header_line.strip().split("\t")
-                source_column_found: bool = False
+                selected_columns: List[int] = []
                 for column_idx, value in enumerate(header_names):
-                    if column_idx == source_column_index:
-                        if source_column_header != value:
-                            result.message = f"Input header name does not math the actual one for index {column_idx}. Expected: {source_column_header}, found: {value}"
+                    if column_idx in column_indices:
+                        if columns[column_idx].header_name != value:
+                            result.message = (
+                                f"Input header name does not math the actual one for index {column_idx}."
+                                + f"Expected: {columns[column_idx].header_name}, found: {value}"
+                            )
                             return result
-                        source_column_found = True
-                        break
+                        selected_columns.append(column_idx)
 
-                if not source_column_found:
-                    result.message = f"Source column index is not found: {column_idx}."
+                if len(selected_columns) != len(column_indices):
+                    invalid_indices = [
+                        x for x in column_indices if x not in selected_columns
+                    ]
+                    result.message = (
+                        "Some column indices are not found :"
+                        + f"{', '.join(invalid_indices)}"
+                    )
                     return result
-                invalid_targets = []
-                for column_idx in columns:
-                    if column_idx >= len(header_names) and column_idx < 0:
-                        invalid_targets.append(column_idx)
 
+                invalid_targets = [
+                    x for x in columns if x >= len(header_names) and x < 0
+                ]
                 if invalid_targets:
                     result.message = f"Target column indices are not valid: {', '.join(invalid_targets)}."
                     return result
 
-                with open(target_file_path, "w") as target:
+                with open(target_file_path, "w", encoding="utf-8") as target:
                     self.write_row(target, header_names)
                     row_index = 0
                     for line in source:
                         row = line.strip().split("\t")
-                        for column_idx in columns:
+                        for column_idx, value in columns.items():
+                            column_data: actions.TsvColumnData = value
                             if (
-                                not selected_row_indices
-                                or row_index in selected_row_indices
+                                not column_data.values
+                                or row_index in column_data.values
                             ):
-                                row[column_idx] = row[source_column_index]
+                                row[column_idx] = column_data.values[row_index]
 
                         self.write_row(target, row)
                         row_index += 1
 
             result.success = True
         except Exception as exc:
             result.message = f"{str(exc)}"
```

### Comparing `metabolights_utils-0.9.8/metabolights_utils/tsv/actions/copy_row.py` & `metabolights_utils-0.9.9/metabolights_utils/tsv/actions/copy_row.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,37 +30,37 @@
         if not source_index or source_index < 0:
             result.message = "There is not row index"
             return result
 
         row_indices = target_row_indices.copy()
         row_indices.sort()
 
-        if action.id:
+        if not action.id:
             uuid_value = str(uuid.uuid4().hex)
             action.id = uuid_value
         copied_row = None
-        with open(source_file_path, "r") as source:
+        with open(source_file_path, "r", encoding="utf-8") as source:
             source.readline()
             row_index = 0
             for line in source:
                 if row_index > source_index:
                     break
                 if row_index == source_index:
                     copied_row = line.strip().split("\t")
                     break
                 row_index += 1
         if not copied_row:
             result.message = "Row will be copied is not found"
             return result
 
         try:
-            with open(source_file_path, "r") as source:
+            with open(source_file_path, "r", encoding="utf-8") as source:
                 header_line = source.readline()
 
-                with open(target_file_path, "w") as target:
+                with open(target_file_path, "w", encoding="utf-8") as target:
                     target.write(header_line)
                     row_index = 0
                     for line in source:
                         if row_index in row_indices:
                             if not selected_column_indices:
                                 self.write_row(target, copied_row)
                             else:
```

### Comparing `metabolights_utils-0.9.8/metabolights_utils/tsv/actions/delete_column.py` & `metabolights_utils-0.9.9/metabolights_utils/tsv/actions/delete_column.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,37 +26,36 @@
         if not columns:
             result.message = "There is not column index"
             return result
 
         column_indices: List[int] = list(columns.keys()).copy()
         column_indices.sort()
 
-        if action.id:
+        if not action.id:
             uuid_value = str(uuid.uuid4().hex)
             action.id = uuid_value
 
         try:
-            with open(source_file_path, "r") as source:
+            with open(source_file_path, "r", encoding="utf-8") as source:
                 header_line = source.readline()
                 header_names = header_line.strip().split("\t")
                 new_header_names = []
                 for column_idx, value in enumerate(header_names):
                     if column_idx in column_indices:
                         header_name = columns[column_idx]
                         if header_name != value:
                             result.message = f"Input header name does not math the actual one for index {column_idx}. Expected: {header_name}, found: {value}"
                             return result
                         continue
 
                     new_header_names.append(value)
 
-                with open(target_file_path, "w") as target:
+                with open(target_file_path, "w", encoding="utf-8") as target:
                     self.write_row(target, new_header_names)
                     for line in source:
-                        new_row = []
                         row = line.strip().split("\t")
                         new_row = [
                             x[1] for x in enumerate(row) if x[0] not in column_indices
                         ]
                         new_row.append(value)
                         self.write_row(target, new_row)
             result.success = True
```

### Comparing `metabolights_utils-0.9.8/metabolights_utils/tsv/actions/delete_row.py` & `metabolights_utils-0.9.9/metabolights_utils/tsv/actions/update_row.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,58 +1,61 @@
 import pathlib
 import uuid
-from typing import List
+from typing import Dict
 
 from metabolights_utils.tsv import model as actions
 from metabolights_utils.tsv.actions.base import BaseTsvAction
 
 
-class DeleteRowsTsvAction(BaseTsvAction):
+class UpdateRowsTsvAction(BaseTsvAction):
     def apply_action(
         self,
         source_file_path: pathlib.Path,
         target_file_path: pathlib.Path,
-        action: actions.TsvDeleteRowsAction,
+        action: actions.TsvUpdateRowsAction,
     ) -> actions.TsvActionResult:
         result: actions.TsvActionResult = actions.TsvActionResult(action=action)
-        if action.type != actions.TsvActionType.DELETE_ROW:
+        if action.type != actions.TsvActionType.UPDATE_ROW_DATA:
             result.message = "Action name is not valid"
             return result
 
-        action: actions.TsvDeleteRowsAction = action
-        target_row_indices: List[int] = action.current_row_indices
+        action: actions.TsvUpdateRowsAction = action
 
-        if not target_row_indices:
-            result.message = "There is not row index"
+        row_data: Dict[int, actions.TsvRowData] = action.rows if action.rows else {}
+        if not row_data:
+            result.message = "There is not row data"
             return result
 
-        row_indices = target_row_indices.copy()
+        row_indices = list(row_data.keys())
         row_indices.sort()
 
-        if action.id:
+        if not action.id:
             uuid_value = str(uuid.uuid4().hex)
             action.id = uuid_value
 
         try:
-            with open(source_file_path, "r") as source:
+            with open(source_file_path, "r", encoding="utf-8") as source:
                 header_line = source.readline()
                 header_names = header_line.strip().split("\t")
+                empty_row = [""] * len(header_names)
 
-                with open(target_file_path, "w") as target:
+                with open(target_file_path, "w", encoding="utf-8") as target:
                     self.write_row(target, header_names)
                     row_index = -1
                     for line in source:
                         row_index += 1
                         if row_index in row_indices:
+                            input_row = row_data[row_index]
+                            new_row = self.get_updated_row(empty_row, input_row)
+                            self.write_row(target, new_row)
                             row_indices.remove(row_index)
-                            continue
                         else:
                             target.write(line)
 
                     if len(row_indices):
-                        result.message = f"Invalid row indices {', '.join(row_indices)}"
+                        result.message = f"Invalid row indices {', '.join([str(x) for x in row_indices])}"
                         return result
             result.success = True
         except Exception as exc:
             result.message = f"{str(exc)}"
 
         return result
```

### Comparing `metabolights_utils-0.9.8/metabolights_utils/tsv/actions/move_column.py` & `metabolights_utils-0.9.9/metabolights_utils/tsv/actions/move_column.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,20 +18,20 @@
             return result
 
         action: actions.TsvMoveColumnAction = action
         source_column_index = action.source_column_index
         source_column_header = action.source_column_header
         new_column_index = action.new_column_index
 
-        if action.id:
+        if not action.id:
             uuid_value = str(uuid.uuid4().hex)
             action.id = uuid_value
 
         try:
-            with open(source_file_path, "r") as source:
+            with open(source_file_path, "r", encoding="utf-8") as source:
                 header_line = source.readline()
                 header_names = header_line.strip().split("\t")
                 new_header_names = []
                 if source_column_index < 0 or source_column_index >= len(header_names):
                     result.message = (
                         f"Source column index is not in range. {source_column_index}"
                     )
@@ -48,15 +48,15 @@
                         f"Input header name does not math the actual one for the index {source_column_index}."
                         + f"Expected: {source_column_header}, found: {moved_header}"
                     )
                     return result
                 new_header_names = [x for x in header_names if x != source_column_index]
                 new_header_names.insert(new_column_index, moved_header)
 
-                with open(target_file_path, "w") as target:
+                with open(target_file_path, "w", encoding="utf-8") as target:
                     self.write_row(target, new_header_names)
                     for line in source:
                         row = line.strip().split("\t")
                         moved_data = row[source_column_index]
                         new_row = [x for x in row if x != source_column_index]
                         new_row.insert(new_column_index, moved_data)
                         self.write_row(target, new_row)
```

### Comparing `metabolights_utils-0.9.8/metabolights_utils/tsv/actions/move_row.py` & `metabolights_utils-0.9.9/metabolights_utils/tsv/actions/move_row.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import pathlib
-import sys
 import uuid
-from typing import Dict, List
 
 from metabolights_utils.tsv import model as actions
 from metabolights_utils.tsv.actions.base import BaseTsvAction
 
 
 class MoveRowTsvAction(BaseTsvAction):
     def apply_action(
@@ -28,21 +26,21 @@
 
         source_index = action.source_row_index
 
         if source_index is None or source_index < 0:
             result.message = "There is not source row index"
             return result
 
-        if action.id:
+        if not action.id:
             uuid_value = str(uuid.uuid4().hex)
             action.id = uuid_value
         new_source_index = source_index
         moved_row = None
         if source_index >= new_row_index:
-            with open(source_file_path, "r") as source:
+            with open(source_file_path, "r", encoding="utf-8") as source:
                 source.readline()
                 row_index = -1
                 for line in source:
                     row_index += 1
                     if row_index > source_index:
                         break
                     if row_index == source_index:
@@ -53,18 +51,18 @@
                 result.message = "The row will be moved is not found"
                 return result
             new_source_index += 1
 
         moved = False
         source_deleted = False
         try:
-            with open(source_file_path, "r") as source:
+            with open(source_file_path, "r", encoding="utf-8") as source:
                 header_line = source.readline()
 
-                with open(target_file_path, "w") as target:
+                with open(target_file_path, "w", encoding="utf-8") as target:
                     target.write(header_line)
                     row_index = -1
                     for line in source:
                         row_index += 1
                         if row_index == new_row_index and not moved:
                             self.write_row(target, moved_row)
                             moved = True
@@ -79,14 +77,14 @@
                             else:
                                 target.write(line)
                     if new_row_index == row_index + 1 and not moved:
                         self.write_row(target, moved_row)
                         moved = True
 
             if not moved:
-                result.message = f"Move is failed"
+                result.message = "Move is failed"
                 return result
             result.success = True
         except Exception as exc:
             result.message = f"{str(exc)}"
 
         return result
```

### Comparing `metabolights_utils-0.9.8/metabolights_utils/tsv/actions/update_cell.py` & `metabolights_utils-0.9.9/metabolights_utils/tsv/actions/update_cell.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pathlib
-import sys
 import uuid
 from typing import Dict, List
 
 from metabolights_utils.tsv import model as actions
 from metabolights_utils.tsv.actions.base import BaseTsvAction
 
 
@@ -36,32 +35,32 @@
                 row_data[row_idx] = actions.TsvRowData()
             data: actions.TsvRowData = row_data[row_idx]
             data.values[col_idx] = val.value
 
         row_indices = {x.row_index for x in cells}
         column_indices = {x.column_index for x in cells}
 
-        if action.id:
+        if not action.id:
             uuid_value = str(uuid.uuid4().hex)
             action.id = uuid_value
 
         try:
-            with open(source_file_path, "r") as source:
+            with open(source_file_path, "r", encoding="utf-8") as source:
                 header_line = source.readline()
                 header_names = header_line.strip().split("\t")
                 invalid_column_indices = [
                     x for x in column_indices if x < 0 or x > len(header_names)
                 ]
                 if invalid_column_indices:
                     result.message = (
                         f"Invalid column indices: {', '.join(invalid_column_indices)}"
                     )
                     return result
 
-                with open(target_file_path, "w") as target:
+                with open(target_file_path, "w", encoding="utf-8") as target:
                     self.write_row(target, header_names)
                     row_index = 0
                     for line in source:
                         row = line.strip().split("\t")
                         if row_index in row_data:
                             row_data_item = row_data[row_index]
                             for column_idx in row_data_item.values:
```

### Comparing `metabolights_utils-0.9.8/metabolights_utils/tsv/actions/update_column_header.py` & `metabolights_utils-0.9.9/metabolights_utils/tsv/actions/update_column_header.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,33 +21,33 @@
         action: actions.TsvUpdateColumnHeaderAction = action
 
         headers: Dict[int, str] = action.new_headers if action.new_headers else {}
 
         column_indices = list(headers.keys())
         column_indices.sort()
 
-        if action.id:
+        if not action.id:
             uuid_value = str(uuid.uuid4().hex)
             action.id = uuid_value
 
         try:
-            with open(source_file_path, "r") as source:
+            with open(source_file_path, "r", encoding="utf-8") as source:
                 header_line = source.readline()
                 header_names = header_line.strip().split("\t")
                 column_count = len(header_names)
                 for column_idx in column_indices:
                     if column_idx < column_count and headers[column_idx]:
                         header_names[column_idx] = headers[column_idx]
                     else:
                         headers[column_idx] = (
                             headers[column_idx] if headers[column_idx] else ""
                         )
                         result.message = f"Invalid column index {column_idx} with column name '{headers[column_idx]}'"
                         return result
-                with open(target_file_path, "w") as target:
+                with open(target_file_path, "w", encoding="utf-8") as target:
                     self.write_row(target, header_names)
                     for line in source:
                         target.write(line)
             result.success = True
         except Exception as exc:
             result.message = f"{str(exc)}"
```

### Comparing `metabolights_utils-0.9.8/metabolights_utils/tsv/actions/update_row.py` & `metabolights_utils-0.9.9/metabolights_utils/tsv/actions/delete_row.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,61 +1,58 @@
 import pathlib
 import uuid
-from typing import Dict
+from typing import List
 
 from metabolights_utils.tsv import model as actions
 from metabolights_utils.tsv.actions.base import BaseTsvAction
 
 
-class UpdateRowsTsvAction(BaseTsvAction):
+class DeleteRowsTsvAction(BaseTsvAction):
     def apply_action(
         self,
         source_file_path: pathlib.Path,
         target_file_path: pathlib.Path,
-        action: actions.TsvUpdateRowsAction,
+        action: actions.TsvDeleteRowsAction,
     ) -> actions.TsvActionResult:
         result: actions.TsvActionResult = actions.TsvActionResult(action=action)
-        if action.type != actions.TsvActionType.UPDATE_ROW_DATA:
+        if action.type != actions.TsvActionType.DELETE_ROW:
             result.message = "Action name is not valid"
             return result
 
-        action: actions.TsvUpdateRowsAction = action
+        action: actions.TsvDeleteRowsAction = action
+        target_row_indices: List[int] = action.current_row_indices
 
-        row_data: Dict[int, actions.TsvRowData] = action.rows if action.rows else {}
-        if not row_data:
-            result.message = "There is not row data"
+        if not target_row_indices:
+            result.message = "There is not row index"
             return result
 
-        row_indices = list(row_data.keys())
+        row_indices = target_row_indices.copy()
         row_indices.sort()
 
-        if action.id:
+        if not action.id:
             uuid_value = str(uuid.uuid4().hex)
             action.id = uuid_value
 
         try:
-            with open(source_file_path, "r") as source:
+            with open(source_file_path, "r", encoding="utf-8") as source:
                 header_line = source.readline()
                 header_names = header_line.strip().split("\t")
-                empty_row = [""] * len(header_names)
 
-                with open(target_file_path, "w") as target:
+                with open(target_file_path, "w", encoding="utf-8") as target:
                     self.write_row(target, header_names)
                     row_index = -1
                     for line in source:
                         row_index += 1
                         if row_index in row_indices:
-                            input_row = row_data[row_index]
-                            new_row = self.get_updated_row(empty_row, input_row)
-                            self.write_row(target, new_row)
                             row_indices.remove(row_index)
+                            continue
                         else:
                             target.write(line)
 
                     if len(row_indices):
-                        result.message = f"Invalid row indices {', '.join([str(x) for x in row_indices])}"
+                        result.message = f"Invalid row indices {', '.join(row_indices)}"
                         return result
             result.success = True
         except Exception as exc:
             result.message = f"{str(exc)}"
 
         return result
```

### Comparing `metabolights_utils-0.9.8/metabolights_utils/tsv/filter.py` & `metabolights_utils-0.9.9/metabolights_utils/tsv/filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,27 +87,27 @@
 
         if self.filter_option.search_columns:
             invalid_columns = []
             for column in self.filter_option.search_columns:
                 if not column in self.column_name_indices:
                     invalid_columns.append(column)
             if invalid_columns:
-                raise TsvFileFilterOption(
+                raise TsvFilterException(
                     f"Invalid search columns: {', '.join(invalid_columns)}"
                 )
         else:
             self.filter_option.search_columns = []
 
         if self.filter_option.search_ignore_columns:
             invalid_columns = []
             for column in self.filter_option.search_ignore_columns:
                 if not column in self.column_name_indices:
                     invalid_columns.append(column)
             if invalid_columns:
-                raise TsvFileFilterOption(
+                raise TsvFilterException(
                     f"Invalid search ignore columns: {', '.join(invalid_columns)}"
                 )
         else:
             self.filter_option.search_ignore_columns = []
 
         self.target_column_indices: Set[int] = set(
             self.column_name_indices[column_name]
@@ -137,15 +137,15 @@
                     self.parameter_data_type = FilterDataType.FLOAT
                 elif isinstance(self.filter_option.parameter, int):
                     self.parameter_data_type = FilterDataType.INTEGER
                 elif isinstance(self.filter_option.parameter, datetime):
                     self.parameter_data_type = FilterDataType.DATETIME
                 else:
                     self.parameter_data_type = FilterDataType.STRING
-                self.parameter = self.convert_to_selected_data_type(self.parameter)
+            self.parameter = self.convert_to_selected_data_type(self.parameter)
 
     def convert_to_selected_data_type(self, value):
         if self.parameter_data_type == FilterDataType.FLOAT:
             return float(value)
         elif self.parameter_data_type == FilterDataType.INTEGER:
             return int(value)
         elif self.parameter_data_type == FilterDataType.DATETIME:
@@ -186,16 +186,16 @@
 
 
 class FilterRegistry:
     custom_filters: Dict[str, Any] = {}
     default_filters: Dict[str, Any] = {}
 
     @classmethod
-    def register_filter(cls, name: str, filter: Any) -> None:
-        cls.default_filters[name] = filter
+    def register_filter(cls, name: str, filter_class: Filter) -> None:
+        cls.default_filters[name] = filter_class
 
     @classmethod
     def get_filter(
         cls,
         filter_option: TsvFileFilterOption,
         column_name_indices: Dict[str, int],
         column_indices: Dict[int, str],
@@ -212,16 +212,16 @@
             if name in cls.default_filters:
                 return cls.default_filters[name](
                     filter_option, column_name_indices, column_indices
                 )
         raise TsvFilterException(f"Filter name {name} is not registered")
 
     @classmethod
-    def register_custom_filter(cls, name: str, filter: Any) -> None:
-        cls.custom_filters[name] = filter
+    def register_custom_filter(cls, name: str, filter_class: CustomFilter) -> None:
+        cls.custom_filters[name] = filter_class
 
     @classmethod
     def unregister_custom_filter(cls, name: str) -> None:
         if name in cls.custom_filters:
             del cls.custom_filters[name]
 
     @classmethod
@@ -247,15 +247,15 @@
         self,
         filter_option: TsvFileFilterOption,
         column_name_indices: Dict[str, int],
         column_indices: Dict[int, str],
     ) -> None:
         super().__init__(filter_option, column_name_indices, column_indices)
         self.custom_filter: CustomFilter = FilterRegistry.get_custom_filter(
-            self.filter_option
+            self.filter_option, column_name_indices, column_indices
         )
 
     def evaluate(self, row_value: str) -> bool:
         if not self.custom_filter:
             return False
         return self.custom_filter.evaluate(row_value)
 
@@ -326,15 +326,15 @@
         super().__init__(filter_option, column_name_indices, column_indices)
 
     def evaluate(self, row_value: str) -> bool:
         if row_value:
             try:
                 value = self.convert_to_selected_data_type(row_value)
                 return True if value > self.parameter else False
-            except:
+            except Exception:
                 return False
         return False
 
 
 class GreaterEqualFilter(Filter):
     def __init__(
         self,
@@ -345,15 +345,15 @@
         super().__init__(filter_option, column_name_indices, column_indices)
 
     def evaluate(self, row_value: str) -> bool:
         if row_value:
             try:
                 value = self.convert_to_selected_data_type(row_value)
                 return True if value >= self.parameter else False
-            except:
+            except Exception:
                 return False
         return False
 
 
 class LessFilter(Filter):
     def __init__(
         self,
@@ -364,15 +364,15 @@
         super().__init__(filter_option, column_name_indices, column_indices)
 
     def evaluate(self, row_value: str) -> bool:
         if row_value:
             try:
                 value = self.convert_to_selected_data_type(row_value)
                 return True if value < self.parameter else False
-            except:
+            except Exception:
                 return False
         return False
 
 
 class LessEqualFilter(Filter):
     def __init__(
         self,
@@ -383,15 +383,15 @@
         super().__init__(filter_option, column_name_indices, column_indices)
 
     def evaluate(self, row_value: str) -> bool:
         if row_value:
             try:
                 value = self.convert_to_selected_data_type(row_value)
                 return True if value <= self.parameter else False
-            except:
+            except Exception:
                 return False
         return False
 
 
 class EmptyFilter(Filter):
     def __init__(
         self,
@@ -441,15 +441,15 @@
     ) -> None:
         super().__init__(filter_option, column_name_indices, column_indices)
 
     def evaluate(self, row_value: str) -> bool:
         try:
             _ = float(row_value)
             return True
-        except:
+        except Exception:
             return False
 
 
 class ValidDatetimeCustomFilter(CustomFilter):
     def __init__(
         self,
         filter_option: TsvFileFilterOption,
@@ -460,15 +460,15 @@
 
     def evaluate(self, row_value: str) -> bool:
         try:
             value = datetime.strptime(
                 row_value, self.filter_option.default_datetime_pattern
             )
             return True if value else False
-        except:
+        except Exception:
             return False
 
 
 class EnumContainsCustomFilter(CustomFilter):
     def __init__(
         self,
         filter_option: TsvFileFilterOption,
@@ -485,22 +485,22 @@
 
                     if len(splitted_value) == 2:
                         self.enum_class = getattr(
                             sys.modules[splitted_value[0]], splitted_value[1]
                         )
                     else:
                         raise TsvFilterException(
-                            f"Selected enum class name is not valid. Use format <module name>:<enum class name>"
+                            "Selected enum class name is not valid. Use format <module name>:<enum class name>"
                         )
             except Exception as exc:
                 if isinstance(exc, TsvFilterException):
                     raise exc
                 raise TsvFilterException(
-                    f"selected class name is not converted to enum: {str(exc)}"
-                )
+                    "Selected class name is not converted to enum"
+                ) from exc
         if not isinstance(self.enum_class, EnumMeta):
             raise TsvFilterException("selected class is not enum")
 
         self.enum_string_map: Dict[str, str] = {}
         if "enum-value-map" in filter_option.custom_filter_arguments:
             self.enum_value_map = filter_option.custom_filter_arguments[
                 "enum-value-map"
@@ -514,21 +514,24 @@
                     self.enum_string_map[str(key)] = str(value)
                 else:
                     self.enum_string_map[str(key)] = str(value).lower()
 
             enum_values = {str(e.value) for e in self.enum_class}
             missing_values = [x for x in enum_values if x not in self.enum_string_map]
             if missing_values:
-                raise TsvSortException(
+                raise TsvFilterException(
                     f"There are some missing values to map an enum {', '.join(missing_values)}"
                 )
 
     def evaluate(self, row_value: str) -> bool:
         try:
-            value = self.parameter in self.enum_string_map[row_value]
+            if self.filter_option.case_sensitive:
+                value = self.parameter in self.enum_string_map[row_value]
+            else:
+                value = self.parameter in self.enum_string_map[str(row_value).lower()]
             return True if value else False
         except Exception:
             return False
 
 
 class BetweenEqualCustomFilter(CustomFilter):
     def __init__(
@@ -542,21 +545,33 @@
         self.max = None
         if "min" in self.filter_option.custom_filter_arguments:
             self.min = self.filter_option.custom_filter_arguments["min"]
         if "max" in self.filter_option.custom_filter_arguments:
             self.max = self.filter_option.custom_filter_arguments["max"]
         self.min = self.convert_to_selected_data_type(self.min)
         self.max = self.convert_to_selected_data_type(self.max)
+        if not self.min or not self.max:
+            raise TsvFilterException("min and max values are not valid.")
+
+        if self.filter_option.data_type == FilterDataType.AUTO:
+            if isinstance(self.min, float):
+                self.parameter_data_type = FilterDataType.FLOAT
+            elif isinstance(self.min, int):
+                self.parameter_data_type = FilterDataType.INTEGER
+            elif isinstance(self.min, datetime):
+                self.parameter_data_type = FilterDataType.DATETIME
+            else:
+                self.parameter_data_type = FilterDataType.STRING
 
     def evaluate(self, row_value: str) -> bool:
         if row_value:
             try:
                 value = self.convert_to_selected_data_type(row_value)
                 return True if self.min <= value <= self.max else False
-            except:
+            except Exception:
                 return False
         return False
 
 
 FilterRegistry.register_custom_filter("between-equal", BetweenEqualCustomFilter)
 FilterRegistry.register_custom_filter("valid-datetime", ValidDatetimeCustomFilter)
 FilterRegistry.register_custom_filter("valid-number", ValidNumberCustomFilter)
```

### Comparing `metabolights_utils-0.9.8/metabolights_utils/tsv/model.py` & `metabolights_utils-0.9.9/metabolights_utils/tsv/model.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.8/metabolights_utils/tsv/sort.py` & `metabolights_utils-0.9.9/metabolights_utils/tsv/sort.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,15 +195,15 @@
                 return str(order) + self.get_sorted_string(value).zfill(length)
             else:
                 return str(order) + self.get_sorted_string(value)
         except Exception:
             return self.get_invalid_value(value)
 
     @abstractmethod
-    def get_sorted_string(value: str) -> str:
+    def get_sorted_string(self, value: str) -> str:
         pass
 
 
 class CustomSorter(AbstractSorter, ABC):
     def __init__(
         self,
         sort_option: TsvFileSortOption,
@@ -226,15 +226,17 @@
         self,
         sort_option: TsvFileSortOption,
         column_idx: int,
         column_name_indices: Dict[str, int],
         column_indices: Dict[int, str],
     ) -> None:
         super().__init__(sort_option, column_idx, column_name_indices, column_indices)
-        self.custom_sorter: CustomSorter = SorterRegistry.get_sorter(sort_option)
+        self.custom_sorter: CustomSorter = SorterRegistry.get_sorter(
+            sort_option, column_idx, column_name_indices, column_indices
+        )
 
     def sort(self, row: Tuple[int, List[str]]) -> str:
         value = row[1][self.column_idx]
         if not value:
             return self.get_none_value()
         try:
             sorter = self.custom_sorter
@@ -340,22 +342,22 @@
 
                     if len(splitted_value) == 2:
                         self.enum_class = getattr(
                             sys.modules[splitted_value[0]], splitted_value[1]
                         )
                     else:
                         raise TsvSortException(
-                            f"Selected enum class name is not valid. Use format <module name>:<enum class name>"
+                            "Selected enum class name is not valid. Use format <module name>:<enum class name>"
                         )
             except Exception as exc:
                 if isinstance(exc, TsvSortException):
                     raise exc
                 raise TsvSortException(
-                    f"selected class name is not converted to enum: {str(exc)}"
-                )
+                    "Selected class name is not converted to enum"
+                ) from exc
         if not isinstance(self.enum_class, EnumMeta):
             raise TsvSortException("selected class is not enum")
 
         self.enum_string_map: Dict[str, str] = {}
         if "enum-value-map" in sort_option.custom_sorter_arguments:
             self.enum_value_map = sort_option.custom_sorter_arguments["enum-value-map"]
             if not isinstance(self.enum_value_map, dict) or not self.enum_value_map:
```

### Comparing `metabolights_utils-0.9.8/metabolights_utils/tsv/tsv_file_updater.py` & `metabolights_utils-0.9.9/metabolights_utils/tsv/tsv_file_updater.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import datetime
-import hashlib
 import os
 import pathlib
 import shutil
 import uuid
 from typing import Dict, List, Union
 
 from metabolights_utils.tsv.actions.add_column import AddColumnsTsvAction
@@ -23,14 +22,15 @@
 from metabolights_utils.tsv.actions.update_row import UpdateRowsTsvAction
 from metabolights_utils.tsv.model import (
     TsvAction,
     TsvActionReport,
     TsvActionResult,
     TsvActionType,
 )
+from metabolights_utils.tsv.utils import calculate_sha256
 
 TSV_FILE_ACTIONS: Dict[TsvActionType, BaseTsvAction] = {}
 TSV_FILE_ACTIONS[TsvActionType.ADD_ROW] = AddRowsTsvAction()
 TSV_FILE_ACTIONS[TsvActionType.DELETE_ROW] = DeleteRowsTsvAction()
 TSV_FILE_ACTIONS[TsvActionType.UPDATE_ROW_DATA] = UpdateRowsTsvAction()
 TSV_FILE_ACTIONS[TsvActionType.COPY_ROW] = CopyRowTsvAction()
 TSV_FILE_ACTIONS[TsvActionType.MOVE_ROW] = MoveRowTsvAction()
@@ -46,15 +46,15 @@
 class TsvFileUpdater:
     def apply_actions(
         self,
         file_path: Union[str, pathlib.Path],
         file_sha256_hash: str,
         actions: List[TsvAction],
     ) -> TsvActionReport:
-        report = TsvActionReport()
+        report: TsvActionReport = TsvActionReport()
         if not file_path:
             report.message = "Invalid input for file path"
             return report
         if not file_sha256_hash:
             report.message = "Invalid input for file hash value"
             return report
         if not file_sha256_hash:
@@ -71,15 +71,15 @@
             file = pathlib.Path(file_path)
 
         if not file.exists() or not file.is_file():
             report.message = (
                 f"File '{str(file)}' does not exist or it is not a regular file."
             )
             return report
-        sha256 = self.calculate_sha256(file)
+        sha256 = calculate_sha256(file)
 
         if sha256 != file_sha256_hash:
             report.message = f"SH256 of '{str(file)}' does not match the input value."
             return report
 
         task_id = str(uuid.uuid4().hex)
         timestamp = str(int(datetime.datetime.now().timestamp()))
@@ -96,15 +96,15 @@
 
         source_path = file_copy_path
         target_path = temp_target_file_path
         last_file = None
         try:
             for action in actions:
                 if action.type not in TSV_FILE_ACTIONS:
-                    report.message = f"Upsupported action: action.type."
+                    report.message = "Upsupported action: action.type."
                     return report
             shutil.move(file, file_copy_path)
             for action in actions:
                 helper = TSV_FILE_ACTIONS[action.type]
                 result: TsvActionResult = helper.apply_action(
                     source_path, target_path, action
                 )
@@ -115,26 +115,19 @@
                     if source_path == temp_source_file_path
                     else temp_source_file_path
                 )
 
                 report.results.append(result)
                 if not result.success:
                     raise TsvActionException(message=result.message)
-            new_sha256 = self.calculate_sha256(last_file)
+            new_sha256 = calculate_sha256(last_file)
             report.updated_file_sha256_hash = new_sha256
             report.success = True
         except Exception as exc:
             raise exc
         finally:
             if report.success and last_file:
                 shutil.move(last_file, file)
             else:
                 shutil.move(file_copy_path, file)
             shutil.rmtree(temp_folder)
         return report
-
-    def calculate_sha256(self, file_path):
-        sha256_hash = hashlib.sha256()
-        with open(file_path, "rb") as file:
-            for chunk in iter(lambda: file.read(4096), b""):
-                sha256_hash.update(chunk)
-        return sha256_hash.hexdigest()
```

### Comparing `metabolights_utils-0.9.8/pyproject.toml` & `metabolights_utils-0.9.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "metabolights-utils"
-version = "0.9.8"
+version = "0.9.9"
 description = "Metabolights common models, utility methods and classes for python-based Metabolights projects."
 authors = ["Ozgur Yurekten <ozgur@ebi.ac.uk>"]
 readme = "README.md"
 packages = [{include = "metabolights_utils"}]
 license = "Apache-2.0"
 homepage = "https://github.com/EBI-Metabolights/metabolights-utils"
 repository = "https://github.com/EBI-Metabolights/metabolights-utils"
@@ -15,38 +15,39 @@
     "Programming Language :: Python :: 3.9",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: File Formats",
     "Topic :: Scientific/Engineering :: Bio-Informatics"
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8.1,<3.9"
-psycopg2-binary = ">=2.8"
-pydantic = "1.10.11"
-pyhumps = "^3.8.0"
+python = ">=3.8.1,<3.10"
+pydantic = "2.4.1"
+pydantic-settings = "^2.0.3"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.0"
+pytest-cov = "^4.1.0"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.0.0"
 flake8-bugbear = "^23.7.10"
 black = "^23.3.0"
 coverage = {extras = ["toml"], version = "^7.2.7"}
 mypy = "^1.4.1"
-pytest-cov = "^4.1.0"
 mkdocs = "^1.4.3"
 griffe = "^0.32.3"
 mkdocstrings-python = "^1.2.1"
 markdown-mdantic = "^1.3.3"
+bump-pydantic = "^0.7.0"
+pylint = "^3.0.2"
 
 
 
 [tool.coverage.run]
-omit = [".*", "*/tests/*", "*/site-packages/*"]
+omit = [".*", "*/tests/*", "*/site-packages/*", "*/docs/*", "*/site/*", "*/dist/*", ".*/*"]
 
 [tool.coverage.report]
 fail_under = 80
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `metabolights_utils-0.9.8/PKG-INFO` & `metabolights_utils-0.9.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: metabolights-utils
-Version: 0.9.8
+Version: 0.9.9
 Summary: Metabolights common models, utility methods and classes for python-based Metabolights projects.
 Home-page: https://github.com/EBI-Metabolights/metabolights-utils
 License: Apache-2.0
 Keywords: metabolights,metabolomics,ISA data model
 Author: Ozgur Yurekten
 Author-email: ozgur@ebi.ac.uk
-Requires-Python: >=3.8.1,<3.9
+Requires-Python: >=3.8.1,<3.10
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: File Formats
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: psycopg2-binary (>=2.8)
-Requires-Dist: pydantic (==1.10.11)
-Requires-Dist: pyhumps (>=3.8.0,<4.0.0)
+Requires-Dist: pydantic (==2.4.1)
+Requires-Dist: pydantic-settings (>=2.0.3,<3.0.0)
 Project-URL: Repository, https://github.com/EBI-Metabolights/metabolights-utils
 Description-Content-Type: text/markdown
 
 
 
 
 
@@ -57,33 +56,30 @@
 
 
 ### Installation
 ---
 The following command installs metabolights-utils from the Python Package Index. You will need a working installation of Python 3.8+ and pip3.
 
 ```shell
-pip install -U sphinx
+pip3 install -U metabolights_utils
 ```
 
 
 ### Read and update Investigation files
 ---
-Read and update an investigation file. Returned objects are json serializable so you can use them with REST APIs.  
+Read and update an investigation file. Results are json serializable, so you can use them with REST APIs.  
 
 ```python 
 import os
 import pathlib
 import uuid
-from ast import List
+from typing import List
 
 from metabolights_utils.isatab import Reader, Writer
-from metabolights_utils.isatab.reader import (
-    InvestigationFileReader,
-    InvestigationFileReaderResult,
-)
+from metabolights_utils.isatab.reader import InvestigationFileReader, InvestigationFileReaderResult
 from metabolights_utils.isatab.writer import InvestigationFileWriter
 from metabolights_utils.models.isa.common import OntologyItem
 from metabolights_utils.models.isa.investigation_file import Assay, Study
 
 
 def test_investigation_file_write_01():
     file_path = pathlib.Path("tests/test-data/MTBLS398/i_Investigation.txt")
@@ -107,33 +103,33 @@
     assert assay_read.measurement_type.term == "test"
     assert assay_read.measurement_type.term_source_ref == "test source"
     assert assay_read.measurement_type.term_accession_number == "test accesion"
     os.remove(tmp_path)
 
 ```
 
-### ISA table file pagination
+### Read and Update ISA Table Files with Pagination Support
 ---
-* Update page size (number of rows in a page) and read results with the selected page size.
-* Define custom row offset and read rows with a limit. Row indices in a page can be unordered after filter and sort operations. You can get actual row index of the selected row using result.
-* Read only the selected columns you defined. If a selected column has additional columns (Term Source REF, etc) and these columns are not defined, they will be in result. Column names may be different than header if there are multiple column with same header. 
-* If no column selected, columns will be ordered. If columns are selected, result will contain columns in the selected order. You can get actual column index of a column using result.
+* Select page size (number of rows in a page) and read results with the selected page size.
+* Define custom row offset and read only selected rows. Actual row indices in a result may be unordered after filter and sort operations. 
+* Read the selected columns you defined. If a selected column has additional columns (Term Source REF, etc) and these columns are not defined by user, they will also be in the result. Column names may be different than header if there are multiple columns with same header. 
+* If columns are not selected, all table columns will be returned in result. If columns are selected, result will contain only these columns in selected order.
 
 ---
 #### Example 1: Read ISA table file
 ---
 
 Read selected assay file (a_*.txt) rows and columns with pagination support. You can use same methods with sample (s_*.txt) and metabolite assignment (m_*.tsv) files.
 ```python
 import pathlib
 
 from metabolights_utils.isatab import Reader
 from metabolights_utils.isatab.reader import (
     IsaTableFileReader,
-    IsaTableFileReaderResult,
+    IsaTableFileReaderResult
 )
 
 
 def test_assay_file_success_01():
     file_path = pathlib.Path(
         "tests/test-data/MTBLS373/a_MTBLS373_sevinaskascreen_metabolite_profiling_mass_spectrometry.txt"
     )
@@ -186,41 +182,42 @@
         page=294, results_per_page=50, file_path=file_path
     )
     assert len(result.parser_report.messages) == 0
     assert result.isa_table_file.table.row_count == 20
 
     # get page 2 with selected columns from isa table.
     # read 50 items from offset 50 (page 2)
-    # If addition columns are not added to result even if they are not selected.
+    # Addition columns will be in result even if they are not selected.
+    # Parameter Value[Autosampler model] is ontology column. So 2 new columns will be added to result.
     result: IsaTableFileReaderResult = reader.get_page(
         page=2,
         results_per_page=50,
         file_path=file_path,
         selected_columns=["Sample Name", "Parameter Value[Autosampler model]"],
     )
     assert len(result.parser_report.messages) == 0
     assert result.isa_table_file.table.row_count == 50
     assert len(result.isa_table_file.table.columns) == 4
 ```
 
 
-#### Example 2: Read and update ISA table file
+#### Example 2: Update ISA table file
 ---
 
 Load ISA table page and save after update table content
 
 ```python
 import os
 import pathlib
 import shutil
 
 from metabolights_utils.isatab import Reader, Writer
 from metabolights_utils.isatab.reader import (
     IsaTableFileReader,
-    IsaTableFileReaderResult,
+    IsaTableFileReaderResult
 )
 from metabolights_utils.isatab.writer import IsaTableFileWriter
 
 
 def test_assay_file_read_write():
     path_original = pathlib.Path(
         "tests/test-data/MTBLS1/a_MTBLS1_metabolite_profiling_NMR_spectroscopy.txt"
@@ -228,15 +225,15 @@
     file_path = (
         ".test-temp/test-data/MTBLS1/a_MTBLS1_metabolite_profiling_NMR_spectroscopy.txt"
     )
     os.makedirs(os.path.dirname(file_path), exist_ok=True)
     shutil.copy(path_original, file_path)
     helper: IsaTableFileReader = Reader.get_assay_file_reader()
 
-    with open(file_path, "r") as file_buffer:
+    with open(file_path, "r", encoding="utf-8") as file_buffer:
         # read second page of assa file
         result: IsaTableFileReaderResult = helper.get_page(
             file_buffer=file_buffer,
             page=2,
             results_per_page=50,
             file_path=str(file_path),
             selected_columns=[
@@ -246,19 +243,20 @@
             ],
         )
         assert len(result.parser_report.messages) == 0
         assert result.isa_table_file.table.row_count == 50
         assert len(result.isa_table_file.table.columns) == 3
     
     writer: IsaTableFileWriter = Writer.get_assay_file_writer()
-    sha256 = "6ea4c731ce35165f83a5d30438cd8753a6afa5fa9a1109893ffc1c213b1da869"
     isa_table = result.isa_table_file.table
+
+    sha256_hash = result.isa_table_file.sha256_hash
     # save same content without any update
     report = writer.save_isa_table(
-        file_path=str(file_path), file_sha256_hash=sha256, isa_table=isa_table
+        file_path=str(file_path), file_sha256_hash=sha256_hash, isa_table=isa_table
     )
     assert report.success
 
     first_column = result.isa_table_file.table.columns[0]
     result.isa_table_file.table.data[first_column][0] = "Updated Sample Name"
     # save updated content
     report = writer.save_isa_table(
@@ -269,57 +267,58 @@
     assert not report.message
 
 ```
 
 ### Multi-column filters and sort options
 ---
 * Case sensitive or case insensitive multi-column sort is supported.
-    - Multi-column sorts with ascending and descending order can be defined. For example; You can sort  by 'Parameter Value\[Gender\]' as ascending and Parameter Value\[Age\] as descending order. 
-    - Columns can be sorted as different data type. Supported sort data types are str, int, float and datetime. datetime pattern can be defined for datetime data type.
-    - Sort orders for invalid and empty values can be defined. For example, If sort value order is defined as VALID_EMPTY_INVALID, invalid values will follow empty values and empty values will follow valid values. This value order option is applicable for int, datetime and float data types. All combinations are poossible for EMPTY, INVALID, VALID values.
-    - You can define your custom sorters. "enum-sorter" as a custom sorter has been already implemented. It sorts enums with given string values.
-* There are **10 different filters** (with inverse options). Any filter can be applied to any column. Multiple filters can be defined. 
+    - Multi-column sorts can be defined with combination of ascending and descending orders. For example; You can sort 'Parameter Value\[Gender\]' by ascending and Parameter Value\[Age\] by descending order. 
+    - Columns can be sorted as different data type. Supported sort data types are: str, int, float and datetime. datetime pattern can be defined.
+    - Sort orders for invalid and empty values can also be defined. For example, If it is defined as VALID_EMPTY_INVALID, invalid values will be at the end. Empty values will follow valid values. This value order option is applicable for only int, datetime and float data types. All sort placement combinations are poossible for EMPTY, INVALID, VALID values.
+    - You can define your custom sorters. A custom "enum-sorter" sorter has been already implemented. It sorts enums with given string values.
+
+* There are **10 different filters** (plus (NOT) options of them). Any filter can be applied to any column. Multiple filters can be defined. 
     - CONTAINS / NOT CONTAINS
     - EQUAL / NOT EQUAL
     - STARTSWITH / NOT STARTSWITH
     - ENDSWITH / NOT ENDSWITH
     - GREATER / NOT GREATER
     - GREATER_EQUAL / NOT GREATER_EQUAL
     - LESS / NOT LESS
     - LESS_EQUAL / NOT LESS_EQUAL
     - REGEX (regex match) / NOT REGEX (not regex match)
     - EMPTY / NOT EMPTY (None or empty)
 * You can define multiple filters. If one filter rejects row, row will not be selected (AND operation).
 * You can define one or more columns for a filter. If there are multiple columns for a filter. If any column matches, the filter selects the row (OR operation).
-* If you do not select any column for a filter, the filter will evaluate all columns. If filter matches with any column, it will select the row. You can define column names to skip them while evaluating all rows. 
+* If you do not select any column for a filter, the filter will evaluate all columns. If filter matches with any column, it will select the row. Moreover, you can define some column names to skip them while filter is evaluating a row. 
+
 * You can define your custom filters. Some custom filters have been already implemented.
     - "between-equal": Returns row if value between given min and max. Min and max inputs can be datetime, str, int or float.
     - "valid-datetime" Return row if value is valid datetime with given pattern. Default pattern is DD/MM/YYYY.
     - "valid-number": Return row if value is valid int or float.
-    - "enum-contains": Gets a map to define a text for each enum value. Returns row if input parameter is in the enum-mapped text. Enums can be any allowed type (str, int, etc.).
-        + Example: Enum values are 1, 2, 3, 4. Enum values are mapped to 1: "In Review", 2: "Published", 3: "In Curation", 4: "Public". If parameter is "Pub", all rows contain enum value 2 and 4 will be returned.
+    - "enum-contains": Gets a map to define a text for each enum value. Returns row if input parameter is in the enum text map. Enum data typese can be any allowed type (str, int, etc.).
+        + Example: Enum values are 1, 2, 3, 4 (You store status values as in on database). Enum values are mapped to 1: "In Review", 2: "Published", 3: "In Curation", 4: "Public". If parameter is "Pub", all rows contain enum value 2 or 4 will be returned.
 
 #### Example
 Users can apply multiple filters and sort operations before retriving ISA table rows.
 
 ```python
 import pathlib
 
 from metabolights_utils.isatab import Reader
 from metabolights_utils.isatab.reader import (
     IsaTableFileReader,
-    IsaTableFileReaderResult,
+    IsaTableFileReaderResult
 )
 from metabolights_utils.models.isa.common import (
     FilterOperation,
     SortType,
     TsvFileFilterOption,
     TsvFileSortOption,
-    TsvFileSortValueOrder,
-)
+    TsvFileSortValueOrder)
 
 
 def test_with_filter_and_sort_option_01():
     # Sample Name value does not start with 'control'  and
     # Parameter Value[Chromatography Instrument] value is 'Thermo Scientific TRACE GC Ultra'.
     # Both filters are applied in case insesitive mode.
     filter_options = [
```

