# Comparing `tmp/omdctk-1.0.tar.gz` & `tmp/omdctk-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omdctk-1.0.tar", last modified: Mon Jul 10 08:32:56 2023, max compression
+gzip compressed data, was "omdctk-1.1.0.tar", last modified: Fri May 10 09:30:15 2024, max compression
```

## Comparing `omdctk-1.0.tar` & `omdctk-1.1.0.tar`

### file list

```diff
@@ -1,33 +1,46 @@
-drwxrwxr-x   0 sapies    (1000) sapies    (1000)        0 2023-07-10 08:32:56.989541 omdctk-1.0/
--rw-rw-r--   0 sapies    (1000) sapies    (1000)     1078 2023-07-05 10:34:25.000000 omdctk-1.0/LICENSE
--rw-rw-r--   0 sapies    (1000) sapies    (1000)     1829 2023-07-10 08:32:56.989541 omdctk-1.0/PKG-INFO
--rw-rw-r--   0 sapies    (1000) sapies    (1000)     1227 2023-07-07 12:16:12.000000 omdctk-1.0/README.md
--rw-rw-r--   0 sapies    (1000) sapies    (1000)     1612 2023-07-07 11:32:21.000000 omdctk-1.0/pyproject.toml
--rw-rw-r--   0 sapies    (1000) sapies    (1000)       38 2023-07-10 08:32:56.989541 omdctk-1.0/setup.cfg
-drwxrwxr-x   0 sapies    (1000) sapies    (1000)        0 2023-07-10 08:32:56.989541 omdctk-1.0/src/
-drwxrwxr-x   0 sapies    (1000) sapies    (1000)        0 2023-07-10 08:32:56.989541 omdctk-1.0/src/omdctk/
--rw-rw-r--   0 sapies    (1000) sapies    (1000)       29 2023-07-07 11:26:29.000000 omdctk-1.0/src/omdctk/__init__.py
--rwxrwxrwx   0 sapies    (1000) sapies    (1000)    24910 2023-07-07 11:37:16.000000 omdctk-1.0/src/omdctk/check_fastqs_ENA.py
--rwxrwxrwx   0 sapies    (1000) sapies    (1000)    67219 2023-07-07 11:38:43.000000 omdctk-1.0/src/omdctk/check_metadata_ENA.py
--rwxrwxrwx   0 sapies    (1000) sapies    (1000)    15590 2023-07-07 11:38:51.000000 omdctk-1.0/src/omdctk/download_fastqs_ENA.py
--rwxrwxrwx   0 sapies    (1000) sapies    (1000)    11448 2023-07-07 11:39:49.000000 omdctk-1.0/src/omdctk/download_metadata_ENA.py
--rwxrwxrwx   0 sapies    (1000) sapies    (1000)    26714 2023-07-07 11:39:41.000000 omdctk-1.0/src/omdctk/filter_metadata.py
--rwxrwxrwx   0 sapies    (1000) sapies    (1000)    15861 2023-07-07 11:39:35.000000 omdctk-1.0/src/omdctk/make_treatment_template_ENA.py
--rw-rw-r--   0 sapies    (1000) sapies    (1000)    14446 2023-07-07 11:39:31.000000 omdctk-1.0/src/omdctk/merge_metadata.py
--rw-rw-r--   0 sapies    (1000) sapies    (1000)    36278 2023-07-07 11:15:22.000000 omdctk-1.0/src/omdctk/omdctk_common.py
-drwxrwxr-x   0 sapies    (1000) sapies    (1000)        0 2023-07-10 08:32:56.989541 omdctk-1.0/src/omdctk/test_info/
--rw-rw-r--   0 sapies    (1000) sapies    (1000)     3341 2023-07-07 11:43:52.000000 omdctk-1.0/src/omdctk/test_info/PRJEB10949_check_fastqs_ENA_reference.log
--rw-rw-r--   0 sapies    (1000) sapies    (1000)     7449 2023-07-07 11:42:41.000000 omdctk-1.0/src/omdctk/test_info/PRJEB10949_check_metadata_ENA_reference.log
--rwxrwxrwx   0 sapies    (1000) sapies    (1000)      308 2023-02-15 14:35:41.000000 omdctk-1.0/src/omdctk/test_info/PRJEB10949_filterfile_example.tsv
--rw-rw-r--   0 sapies    (1000) sapies    (1000)     5420 2023-04-11 17:18:21.000000 omdctk-1.0/src/omdctk/test_info/PRJEB10949_publication_example.tsv
--rw-rw-r--   0 sapies    (1000) sapies    (1000)     1801 2023-02-15 10:47:51.000000 omdctk-1.0/src/omdctk/test_info/treatment_template_filtered_PRJEB10949_merged_metadata_example.tsv
--rw-rw-r--   0 sapies    (1000) sapies    (1000)    24577 2023-07-07 11:52:33.000000 omdctk-1.0/src/omdctk/test_omdctk.py
--rwxrwxrwx   0 sapies    (1000) sapies    (1000)    27182 2023-07-07 11:39:07.000000 omdctk-1.0/src/omdctk/treat_fastqs.py
--rw-rw-r--   0 sapies    (1000) sapies    (1000)    34656 2023-07-07 11:38:59.000000 omdctk-1.0/src/omdctk/treat_metadata_ENA.py
-drwxrwxr-x   0 sapies    (1000) sapies    (1000)        0 2023-07-10 08:32:56.989541 omdctk-1.0/src/omdctk.egg-info/
--rw-rw-r--   0 sapies    (1000) sapies    (1000)     1829 2023-07-10 08:32:56.000000 omdctk-1.0/src/omdctk.egg-info/PKG-INFO
--rw-rw-r--   0 sapies    (1000) sapies    (1000)      937 2023-07-10 08:32:56.000000 omdctk-1.0/src/omdctk.egg-info/SOURCES.txt
--rw-rw-r--   0 sapies    (1000) sapies    (1000)        1 2023-07-10 08:32:56.000000 omdctk-1.0/src/omdctk.egg-info/dependency_links.txt
--rw-rw-r--   0 sapies    (1000) sapies    (1000)      520 2023-07-10 08:32:56.000000 omdctk-1.0/src/omdctk.egg-info/entry_points.txt
--rw-rw-r--   0 sapies    (1000) sapies    (1000)       65 2023-07-10 08:32:56.000000 omdctk-1.0/src/omdctk.egg-info/requires.txt
--rw-rw-r--   0 sapies    (1000) sapies    (1000)        7 2023-07-10 08:32:56.000000 omdctk-1.0/src/omdctk.egg-info/top_level.txt
+drwxrwxr-x   0 sapies    (1000) sapies    (1000)        0 2024-05-10 09:30:15.791482 omdctk-1.1.0/
+-rw-rw-r--   0 sapies    (1000) sapies    (1000)     1078 2024-02-15 00:39:50.000000 omdctk-1.1.0/LICENSE
+-rw-r--r--   0 sapies    (1000) sapies    (1000)     2387 2024-05-10 09:30:15.791482 omdctk-1.1.0/PKG-INFO
+-rw-rw-r--   0 sapies    (1000) sapies    (1000)     1598 2024-05-10 09:29:33.000000 omdctk-1.1.0/README.md
+-rw-rw-r--   0 sapies    (1000) sapies    (1000)     1732 2024-03-11 10:52:34.000000 omdctk-1.1.0/pyproject.toml
+-rw-rw-r--   0 sapies    (1000) sapies    (1000)       38 2024-05-10 09:30:15.791482 omdctk-1.1.0/setup.cfg
+drwxrwxr-x   0 sapies    (1000) sapies    (1000)        0 2024-05-10 09:30:15.787482 omdctk-1.1.0/src/
+drwxrwxr-x   0 sapies    (1000) sapies    (1000)        0 2024-05-10 09:30:15.791482 omdctk-1.1.0/src/omdctk/
+-rw-rw-r--   0 sapies    (1000) sapies    (1000)       29 2024-02-15 00:39:50.000000 omdctk-1.1.0/src/omdctk/__init__.py
+-rwxrwxrwx   0 sapies    (1000) sapies    (1000)    46738 2024-03-06 10:47:45.000000 omdctk-1.1.0/src/omdctk/check_fastqs.py
+-rwxrwxrwx   0 sapies    (1000) sapies    (1000)    67219 2024-02-15 00:39:50.000000 omdctk-1.1.0/src/omdctk/check_metadata_ENA.py
+-rw-rw-r--   0 sapies    (1000) sapies    (1000)    55111 2024-03-01 14:33:46.000000 omdctk-1.1.0/src/omdctk/check_metadata_values.py
+-rw-rw-r--   0 sapies    (1000) sapies    (1000)    15409 2024-02-21 15:48:04.000000 omdctk-1.1.0/src/omdctk/concat_datasets.py
+-rwxrwxrwx   0 sapies    (1000) sapies    (1000)    16051 2024-02-17 18:54:14.000000 omdctk-1.1.0/src/omdctk/download_fastqs.py
+-rwxrwxrwx   0 sapies    (1000) sapies    (1000)    11649 2024-03-05 09:19:52.000000 omdctk-1.1.0/src/omdctk/download_metadata_ENA.py
+-rwxrwxrwx   0 sapies    (1000) sapies    (1000)    26078 2024-03-05 09:38:50.000000 omdctk-1.1.0/src/omdctk/filter_metadata.py
+-rwxrwxrwx   0 sapies    (1000) sapies    (1000)    21756 2024-03-05 17:16:14.000000 omdctk-1.1.0/src/omdctk/make_treatment_template.py
+-rw-rw-r--   0 sapies    (1000) sapies    (1000)    15841 2024-02-17 18:54:14.000000 omdctk-1.1.0/src/omdctk/merge_metadata.py
+-rw-rw-r--   0 sapies    (1000) sapies    (1000)    49366 2024-03-12 12:25:07.000000 omdctk-1.1.0/src/omdctk/omdctk_common.py
+drwxrwxr-x   0 sapies    (1000) sapies    (1000)        0 2024-05-10 09:30:15.791482 omdctk-1.1.0/src/omdctk/test_info/
+-rw-rw-r--   0 sapies    (1000) sapies    (1000)     4285 2024-03-11 11:05:41.000000 omdctk-1.1.0/src/omdctk/test_info/CRA001372_check_fastqs_Generic_reference.log
+-rwxrwxrwx   0 sapies    (1000) sapies    (1000)       88 2024-03-04 16:33:00.000000 omdctk-1.1.0/src/omdctk/test_info/CRA001372_filterfile_example.tsv
+-rw-rw-r--   0 sapies    (1000) sapies    (1000)   665878 2024-03-08 16:27:11.000000 omdctk-1.1.0/src/omdctk/test_info/CRA001372_main_metadata_example.tsv
+-rw-rw-r--   0 sapies    (1000) sapies    (1000)    32523 2024-03-05 15:34:02.000000 omdctk-1.1.0/src/omdctk/test_info/CRA001372_publication_metadata_example.tsv
+-rw-rw-r--   0 sapies    (1000) sapies    (1000)     3340 2024-03-11 09:28:10.000000 omdctk-1.1.0/src/omdctk/test_info/PRJEB10949_check_fastqs_ENA_reference.log
+-rw-rw-r--   0 sapies    (1000) sapies    (1000)     7449 2024-02-15 00:39:50.000000 omdctk-1.1.0/src/omdctk/test_info/PRJEB10949_check_metadata_ENA_reference.log
+-rwxrwxrwx   0 sapies    (1000) sapies    (1000)      308 2024-02-15 00:39:50.000000 omdctk-1.1.0/src/omdctk/test_info/PRJEB10949_filterfile_example.tsv
+-rw-rw-r--   0 sapies    (1000) sapies    (1000)     5420 2024-02-15 00:39:50.000000 omdctk-1.1.0/src/omdctk/test_info/PRJEB10949_publication_example.tsv
+-rw-rw-r--   0 sapies    (1000) sapies    (1000)    14734 2024-03-11 17:42:39.000000 omdctk-1.1.0/src/omdctk/test_info/check_metadata_values_example_reference.log
+-rw-rw-r--   0 sapies    (1000) sapies    (1000)     3633 2024-03-11 17:03:42.000000 omdctk-1.1.0/src/omdctk/test_info/curated_CRA001372_external_example_metadata_final.tsv
+-rw-rw-r--   0 sapies    (1000) sapies    (1000)     2240 2024-03-11 16:52:18.000000 omdctk-1.1.0/src/omdctk/test_info/curated_PRJEB10949_ENA_example_metadata_final.tsv
+-rw-rw-r--   0 sapies    (1000) sapies    (1000)     1560 2024-03-04 16:39:42.000000 omdctk-1.1.0/src/omdctk/test_info/filtered_CRA001372_URLS_example.txt
+-rw-rw-r--   0 sapies    (1000) sapies    (1000)     1399 2024-03-05 17:13:40.000000 omdctk-1.1.0/src/omdctk/test_info/filtered_manifest_CRA001372_example.tsv
+-rw-rw-r--   0 sapies    (1000) sapies    (1000)      937 2024-03-11 14:55:21.000000 omdctk-1.1.0/src/omdctk/test_info/treatment_template_filtered_CRA001372_example.tsv
+-rw-rw-r--   0 sapies    (1000) sapies    (1000)     1801 2024-02-15 00:39:50.000000 omdctk-1.1.0/src/omdctk/test_info/treatment_template_filtered_PRJEB10949_merged_metadata_example.tsv
+-rw-rw-r--   0 sapies    (1000) sapies    (1000)     1613 2024-03-11 16:59:14.000000 omdctk-1.1.0/src/omdctk/test_info/variables_dictionary_example.tsv
+-rw-rw-r--   0 sapies    (1000) sapies    (1000)    44067 2024-03-12 12:24:54.000000 omdctk-1.1.0/src/omdctk/test_omdctk.py
+-rwxrwxrwx   0 sapies    (1000) sapies    (1000)    27182 2024-02-15 00:39:50.000000 omdctk-1.1.0/src/omdctk/treat_fastqs.py
+-rw-rw-r--   0 sapies    (1000) sapies    (1000)    50270 2024-03-07 16:52:43.000000 omdctk-1.1.0/src/omdctk/treat_metadata.py
+drwxrwxr-x   0 sapies    (1000) sapies    (1000)        0 2024-05-10 09:30:15.791482 omdctk-1.1.0/src/omdctk.egg-info/
+-rw-r--r--   0 sapies    (1000) sapies    (1000)     2387 2024-05-10 09:30:15.000000 omdctk-1.1.0/src/omdctk.egg-info/PKG-INFO
+-rw-rw-r--   0 sapies    (1000) sapies    (1000)     1682 2024-05-10 09:30:15.000000 omdctk-1.1.0/src/omdctk.egg-info/SOURCES.txt
+-rw-rw-r--   0 sapies    (1000) sapies    (1000)        1 2024-05-10 09:30:15.000000 omdctk-1.1.0/src/omdctk.egg-info/dependency_links.txt
+-rw-rw-r--   0 sapies    (1000) sapies    (1000)      592 2024-05-10 09:30:15.000000 omdctk-1.1.0/src/omdctk.egg-info/entry_points.txt
+-rw-rw-r--   0 sapies    (1000) sapies    (1000)       65 2024-05-10 09:30:15.000000 omdctk-1.1.0/src/omdctk.egg-info/requires.txt
+-rw-rw-r--   0 sapies    (1000) sapies    (1000)        7 2024-05-10 09:30:15.000000 omdctk-1.1.0/src/omdctk.egg-info/top_level.txt
```

### Comparing `omdctk-1.0/LICENSE` & `omdctk-1.1.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Samuel Piquer Esteban
+Copyright (c) 2024 Samuel Piquer Esteban
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `omdctk-1.0/PKG-INFO` & `omdctk-1.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,42 @@
 Metadata-Version: 2.1
 Name: omdctk
-Version: 1.0
+Version: 1.1.0
 Summary: OMD Curation Toolkit
 Author-email: Samuel Piquer Esteban <samuel.piquer@uv.es>
 Project-URL: GitHub, https://github.com/tbcgit/omdctk
 Project-URL: Documentation, https://github.com/tbcgit/omdctk/wiki
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aioftp
+Requires-Dist: aiohttp
+Requires-Dist: parfive
+Requires-Dist: termcolor
+Requires-Dist: tabulate
+Requires-Dist: tqdm
+Requires-Dist: mg-toolkit
+Requires-Dist: pandas
 
 # OMD Curation Toolkit
-Omics Dataset Curation Toolkit (**OMD Curation Toolkit**) is a suite of programs designed for the download and curation of metadata and fastq files of public omics datasets. Centered on the European Nucleotide Archive (ENA), this workflow provides a standardized framework intended to facilitate the arduous task of curating public omics projects.
+Omics Dataset Curation Toolkit (**OMD Curation Toolkit**) is a suite of programs designed for the download and curation of metadata and fastq files of public omics datasets. This workflow provides a standardized framework intended to facilitate the arduous task of curating public omics projects. While centered on the European Nucleotide Archive (ENA), the majority of provided tools are generic and can be used to curate datasets from different sources.
 
 ## Getting started
 For further details, see the following:
 * **Documentation** (https://github.com/tbcgit/omdctk/wiki)
 * **Installation** (https://github.com/tbcgit/omdctk/wiki/Installation)
 * **Tutorial Full Example** (https://github.com/tbcgit/omdctk/wiki/Tutorial-Full-Example)
-  
+
+## Citation
+If you use OMD Curation Toolkit, please cite:
+Piquer-Esteban, S., Arnau, V., Diaz, W. et al. OMD Curation Toolkit: a workflow for in-house curation of public omics datasets. BMC Bioinformatics 25, 184 (2024). https://doi.org/10.1186/s12859-024-05803-9
+
 ## Acknowledgements
 This package has been jointly developed in the **Theory, Bioinformatics and Computation** (https://www.uv.es/tbc) and **Evolutionary Genetics** (https://www.uv.es/symbiosis) research groups at the **Institute for Integrative Systems Biology (I2SysBio)**, University of Valencia and Consejo Superior de Investigaciones Científicas (CSIC), Valencia, Spain. SPE is supported by an FPU grant from the Spanish Ministry of Universities (Reference: FPU20/05756).
 
 ## License
 This package is licensed under the MIT License. See the LICENSE file for details.
```

### Comparing `omdctk-1.0/README.md` & `omdctk-1.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # OMD Curation Toolkit
-Omics Dataset Curation Toolkit (**OMD Curation Toolkit**) is a suite of programs designed for the download and curation of metadata and fastq files of public omics datasets. Centered on the European Nucleotide Archive (ENA), this workflow provides a standardized framework intended to facilitate the arduous task of curating public omics projects.
+Omics Dataset Curation Toolkit (**OMD Curation Toolkit**) is a suite of programs designed for the download and curation of metadata and fastq files of public omics datasets. This workflow provides a standardized framework intended to facilitate the arduous task of curating public omics projects. While centered on the European Nucleotide Archive (ENA), the majority of provided tools are generic and can be used to curate datasets from different sources.
 
 ## Getting started
 For further details, see the following:
 * **Documentation** (https://github.com/tbcgit/omdctk/wiki)
 * **Installation** (https://github.com/tbcgit/omdctk/wiki/Installation)
 * **Tutorial Full Example** (https://github.com/tbcgit/omdctk/wiki/Tutorial-Full-Example)
-  
+
+## Citation
+If you use OMD Curation Toolkit, please cite:
+Piquer-Esteban, S., Arnau, V., Diaz, W. et al. OMD Curation Toolkit: a workflow for in-house curation of public omics datasets. BMC Bioinformatics 25, 184 (2024). https://doi.org/10.1186/s12859-024-05803-9
+
 ## Acknowledgements
 This package has been jointly developed in the **Theory, Bioinformatics and Computation** (https://www.uv.es/tbc) and **Evolutionary Genetics** (https://www.uv.es/symbiosis) research groups at the **Institute for Integrative Systems Biology (I2SysBio)**, University of Valencia and Consejo Superior de Investigaciones Científicas (CSIC), Valencia, Spain. SPE is supported by an FPU grant from the Spanish Ministry of Universities (Reference: FPU20/05756).
 
 ## License
 This package is licensed under the MIT License. See the LICENSE file for details.
```

### Comparing `omdctk-1.0/pyproject.toml` & `omdctk-1.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "omdctk"
-version = "1.0"
+version = "1.1.0"
 authors = [
   { name="Samuel Piquer Esteban", email="samuel.piquer@uv.es" },
 ]
 description = "OMD Curation Toolkit"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -33,20 +33,22 @@
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ['src']
 namespaces = true
 
 [tool.setuptools.package-data]
-"omdctk.test_info" = ["*.log", "*.tsv"]
+"omdctk.test_info" = ["*.log", "*.tsv","*.txt"]
 
 [project.scripts]
-check_fastqs_ENA            = 'omdctk.check_fastqs_ENA:main'
+check_fastqs                = 'omdctk.check_fastqs:main'
 check_metadata_ENA          = 'omdctk.check_metadata_ENA:main'
-download_fastqs_ENA         = 'omdctk.download_fastqs_ENA:main'
+download_fastqs             = 'omdctk.download_fastqs:main'
 download_metadata_ENA       = 'omdctk.download_metadata_ENA:main'
 filter_metadata             = 'omdctk.filter_metadata:main'
-make_treatment_template_ENA = 'omdctk.make_treatment_template_ENA:main'
+make_treatment_template     = 'omdctk.make_treatment_template:main'
 merge_metadata              = 'omdctk.merge_metadata:main'
 test_omdctk                 = 'omdctk.test_omdctk:main'
 treat_fastqs                = 'omdctk.treat_fastqs:main'
-treat_metadata_ENA          = 'omdctk.treat_metadata_ENA:main'
+treat_metadata              = 'omdctk.treat_metadata:main'
+concat_datasets             = 'omdctk.concat_datasets:main'
+check_metadata_values       = 'omdctk.check_metadata_values:main'
```

### Comparing `omdctk-1.0/src/omdctk/check_fastqs_ENA.py` & `omdctk-1.1.0/src/omdctk/filter_metadata.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,483 +1,466 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
-@program: check_fastqs_ENA.py
+@program: filter_metadata.py
 @author: Samuel Piquer-Esteban
-@date: 7 Jul 2023 
+@date: 5 Mar 2024 
 
 """
 
 #Set program name
-__program__ = 'check_fastqs_ENA.py'
+__program__ = 'filter_metadata.py'
 
 #Imports from MTD_CT common module
-from omdctk import (DATE, VERSION, ENA_FASTQ_URLS_COLUMNS, program_header, 
-                    show_advise_legend, get_urls_from_ENA_column, 
-                    print_list_n_byline, metadata_files_main_information,
-                    get_list_fastqs_in_directory, rich_text_colored,
-                    check_existence_directory_parameter, 
-                    check_headers, treat_headers_check)
+from omdctk import (DATE, VERSION, OMD_CTK_Exception, program_header, check_values_inv,
+                    check_existence_directory_parameter, curly_2_straight_quotation,
+                    check_headers, treat_headers_check,
+                    check_values, treat_values_check,
+                    treat_output_directory_parameter_outfiles,
+                    rich_text_colored)
 
 #Import third-party modules
 from argparse import ArgumentParser
 from tabulate import tabulate
-from hashlib import md5
+from ast import literal_eval
 import pandas as pd
-import os
 
 #Program Constants
-HEADERS_USED = ['sample_accession', 'sample_alias', 'library_layout',
-                'run_accession', 'fastq_ftp', 'fastq_aspera', 'fastq_galaxy',
-                'submitted_ftp', 'submitted_aspera', 'submitted_galaxy',
-                'fastq_md5', 'submitted_md5']
+FILTERFILE_HEADERS = ['variable', 'values', 'filter_type', 'action', 'NA_treatment']
 
-#Program Functions
-def check_files_in_directory_frase(file_name, file_in_directory, color_treatment):
-    """
-    This function gets the check_files_in_directory_frase.
+FILTERFILE_FILTER_TYPES_ACTION_COMB = ['categorical + keep', 'categorical + drop',
+                                       'numerical + greater', 'numerical + greater_equal', 
+                                       'numerical + equal', 'numerical + less',
+                                       'numerical + less_equal']
 
-    Parameters
-    ----------
-    file_name : str
-        The name of the file.
-    file_in_directory : bool
-        Bool value to see if the file is in the provided directory.
-    color_treatment: bool
-        The color treatment option provided.
-        True : Plain Text
-        False : Colored Text
+FILTERFILE_NA_TREATMENT = ['drop', 'keep', 'no']
 
-    Returns
-    -------
-    bool_value : bool
-        Bool to treat warnings.
-    str_frase : str
-        String with the check_files_in_directory_frase.
-
-    """
-    if file_in_directory == True:
-        bool_value = True
-        str_frase = file_name + ' ' + rich_text_colored('True! The file is in the provided directory!', 'true_color', color_treatment)
-    else:
-        bool_value = False
-        str_frase = file_name + ' ' + rich_text_colored('False! The file is not in the provided directory!', 'false_color', color_treatment)
-    return bool_value, str_frase
-
-def treat_metadata_on_directory_checks(urls, fastqs_in_directory, color_treatment):
+#Program Functions
+def check_filterfile_values_column_format(filterfile_df, color_treatment):
     """
-    This function treats the metadata's fastqs checks on the fastqs directory.
+    This function checks the format of the provided values
+    in the "values" column of the filter file.
 
     Parameters
     ----------
-    urls : list
-        List with the fastq urls from the Metadata file.
-    fastqs_in_directory : list
-        List of fastqs detected in the provided directory.
+    filterfile_df : pandas dataframe
+        The provided filterfile dataframe.
     color_treatment: bool
         The color treatment option provided.
         True : Plain Text
         False : Colored Text
 
+    Raises
+    ------
+    OMD_CTK_Exception
+        If format inconsistencies are detected raises an exception.
+
     Returns
     -------
-    bool
-        True: There are warnings.
-        False: There are no warnings.
-
-    """
-    #Init list results
-    directory_checks_warnings = []
-    
-    #For each url do check
-    for i in range(len(urls)):
-        ##Get file name
-        temp_file_name = urls[i].split('/')[-1]
-        ##Check that the file is in fastqs_directory
-        file_in_directory = temp_file_name in fastqs_in_directory
-        ##Directory_check
-        temp_directory_check = check_files_in_directory_frase(temp_file_name, file_in_directory, color_treatment)
-        ##If has warning keep file name
-        if temp_directory_check[0] == False:
-            directory_checks_warnings.append(temp_file_name)
-    
-    #Treat directory_checks_warnings
-    print(rich_text_colored('\n1) Check that expected files from the Metadata Table exist in the provided directory:', 'subsection', color_treatment))
-    if len(directory_checks_warnings) == 0:
-        print(rich_text_colored('All the expected Fastq files from the Metadata Table are in the provided directory!', 'acceptable', color_treatment))
-        #Return info for lately treat advise messages
-        return False
-    else:
-        print(rich_text_colored('\nWarning! The following expected Fastq files from the Metadata Table are not in the provided directory!', 'program_warning', color_treatment))
-        print_list_n_byline(directory_checks_warnings, 5)
-        #Show advise messages
-        print(rich_text_colored('\nThis could be due to:','due_to_header', color_treatment))
-        print('- The presence of untreated download errors', rich_text_colored('[Warning]', 'legend_warning', color_treatment))
-        print(rich_text_colored('\nYou should:', 'you_should_header', color_treatment))
-        print('- Manually confirm that this is your case')
-        print('- If necessary, try to re-download affected files')
-        #Return info for lately treat advise messages
-        return True
-    
+    None.
 
-def treat_directory_on_metadata_check(urls, fastqs_in_directory, color_treatment):
     """
-    This function treats the fastqs directory checks on the metadata's fastqs.
+    #Check format(list) for values
+    format_checks = []
+    for val in filterfile_df['values']:
+        try: 
+            #Try to strip start and end spaces
+            strip_val = val.strip()
+            #Check list format
+            if strip_val.startswith('[') and strip_val.endswith(']'):
+                format_checks.append(True)
+            else:
+                format_checks.append(False)
+        except:
+            format_checks.append(False)
+    
+    #Check empty cells
+    NAs_checks = list(filterfile_df['values'].isna())
+    
+    #Combine checks
+    result_bools = []
+    result_prints = []
+    for i in range(len(format_checks)):
+        #Wrong format and Not NA
+        if format_checks[i] == False and NAs_checks[i] == False:
+            result_bools.append(False)
+            print_strn = ' '.join(['-', rich_text_colored(filterfile_df['variable'][i], 'check_color', color_treatment), rich_text_colored('Does not have the expected "[]" format!', 'program_warning', color_treatment)])
+            result_prints.append(print_strn)
+        #Wrong format and NA
+        elif format_checks[i] == False and NAs_checks[i] == True:
+            result_bools.append(False)
+            print_strn = ' '.join(['-', rich_text_colored(filterfile_df['variable'][i], 'check_color', color_treatment), rich_text_colored('Cell is empty!', 'program_warning', color_treatment)])
+            result_prints.append(print_strn)
+        #Right format (It will never be NA)
+        else:
+            result_bools.append(True)
+            print_strn = ' '.join(['-', rich_text_colored(filterfile_df['variable'][i], 'check_color', color_treatment), rich_text_colored('Everything seems okay!', 'acceptable', color_treatment)])
+            result_prints.append(print_strn)
+    
+    #Treat final checks
+    if False in result_bools:
+        #Prepare exception frase
+        frase0 = 'Error! Some of the values of the "values" column in the Filter Table are not valid!\n Check your filter file!\n'
+        frase1 = '\nShowing checks by variable:'
+        frase = [frase0, frase1]
+        for i in result_prints:
+            temp_line = ' '.join(['\n', i])
+            frase.append(temp_line)
+        #Raise exception
+        raise OMD_CTK_Exception(' '.join(frase))
+    
+  
+def process_filterfile_values_and_checks(variable, values, filter_type, metadata_df, color_treatment):
+    """
+    This function processes the provided values and runs various checks 
+    depending on their filter_type. This function processes only one 
+    input at a time. 
 
     Parameters
     ----------
-    urls : list
-        List with the fastq urls from the Metadata file.
-    fastqs_in_directory : list
-        List of fastqs detected in the provided directory.
+    variable : str
+        The provided variable to check(colname in metadata table).
+    values : str
+        The provided values to check.
+    filter_type : str
+        the filter_type to be applied.
+        Expected values ['categorical','numerical']
+    metadata_df : pandas dataframe
+        The provided metadata dataframe to check with.
     color_treatment: bool
         The color treatment option provided.
         True : Plain Text
         False : Colored Text
 
     Returns
     -------
-    bool
-        True: There are warnings.
-        False: There are no warnings.
-
+    print_strn : str
+        Colored string message indicating if everything is okey (green) or
+        if there is any warning to check (red).
+    bool_value : bool
+        Bool value indicating if everything is okey (True) or there is
+        any warning to check (False).
+    result_value : list
+        The list of provided values processed to properly interact with the
+        metadata table.
+        
     """
-    ##Init list results
-    fastqs_in_metadata = []
-    ##For each url check
-    for i in range(len(urls)):
-        ##Get file name
-        temp_file_name = urls[i].split('/')[-1]
-        ##Save file name for latter
-        fastqs_in_metadata.append(temp_file_name)
-    
-    #Check fastqs that are in the provided directory but not in the metadata table
-    print(rich_text_colored('\n2) Check if there are Fastq files of the provided directory absent in the Metadata Table:', 'subsection', color_treatment))
-    ##Get asymmetric difference between list
-    fastqs_difference = list(set(fastqs_in_directory) - set(fastqs_in_metadata))
-    ##If fastqs_difference is empty show message/ Else show different files
-    if len(fastqs_difference) == 0:
-        print(rich_text_colored('There are no extra Fastq files in the provided directory!', 'acceptable', color_treatment))
-        #Return info for lately treat advise messages
-        return False
+    #Pre-process values until get a list of multiple or single values
+    ##Convert curly to straight quotation(in case file has been edited in calc, or excel)
+    pre_values = curly_2_straight_quotation(values)
+    ##Try to evaluate string to convert it to list
+    try:
+        post_values = literal_eval(pre_values)
+    except:
+        print_strn = ' '.join(['-', rich_text_colored(variable, 'check_color', color_treatment), rich_text_colored('The provided values can not be converted to list!', 'program_warning', color_treatment)])
+        bool_value = False
+        result_value = pre_values
     else:
-        print(rich_text_colored('\nWarning! The following Fastq files are not in the Metadata Table!', 'program_warning', color_treatment))
-        print_list_n_byline(fastqs_difference, 5)
-        #Show advise messages
-        print(rich_text_colored('\nThis could be due to:','due_to_header', color_treatment))
-        print('- The mixture of different dataset projects', rich_text_colored('[Warning]', 'legend_warning', color_treatment))
-        print(rich_text_colored('\nYou should:', 'you_should_header', color_treatment))
-        print('- Manually confirm that this is your case and act accordingly')
-        #Return info for lately treat advise messages
-        return True
+        #Check that the list is not empty
+        if len(post_values) == 0:
+            print_strn = ' '.join(['-', rich_text_colored(variable, 'check_color', color_treatment), rich_text_colored('The provided list is empty!', 'program_warning', color_treatment)])
+            bool_value = False
+            result_value = post_values
+        else:
+            #Type_filter checks
+            ##Treat numerical type_filters values
+            if filter_type == 'numerical':
+                #Get metadata column dtype
+                metadata_colum_dtype = metadata_df[variable].dtype
+                ##If column in metadata table is numerical continue/ else stop
+                if metadata_colum_dtype == int or metadata_colum_dtype == float:
+                    ##Numerical filter values must be a unique number
+                    if len(post_values) == 1:
+                        #Check that the value is int or float
+                        if type(post_values[0]) == int or type(post_values[0]) == float:
+                            print_strn = ' '.join(['-', rich_text_colored(variable, 'check_color', color_treatment), rich_text_colored('Everything seems okay!', 'acceptable', color_treatment)])
+                            bool_value = True
+                            result_value = post_values
+                        else:
+                            print_strn = ' '.join(['-', rich_text_colored(variable, 'check_color', color_treatment), rich_text_colored('The provided value is not numerical!', 'program_warning', color_treatment)])
+                            bool_value = False
+                            result_value = post_values
+                    else:
+                        print_strn = ' '.join(['-', rich_text_colored(variable, 'check_color', color_treatment), rich_text_colored('Values for numerical filters must be a unique number!', 'program_warning', color_treatment)])
+                        bool_value = False
+                        result_value = post_values
+                else:
+                    print_strn = ' '.join(['-', rich_text_colored(variable, 'check_color', color_treatment), rich_text_colored('Is not a numerical variable in the Metadata Table!', 'program_warning', color_treatment)])
+                    bool_value = False
+                    result_value = post_values
+            ##Treat categorical type_filters values
+            else:
+                #Check if ALL the provided categorical values are in the corresponding column in metadata table
+                bool_value = check_values_inv(metadata_df[variable], post_values)
+                result_value = post_values
+                #If true continue/ else warning
+                if bool_value == True:
+                    print_strn = ' '.join(['-', rich_text_colored(variable, 'check_color', color_treatment), rich_text_colored('Everything seems okay!', 'acceptable', color_treatment)])
+                else:
+                    print_strn = ' '.join(['-', rich_text_colored(variable, 'check_color', color_treatment), rich_text_colored('Some of the provided values are not in the Metadata Table!', 'program_warning', color_treatment)])
+            
+    return print_strn, bool_value, result_value
 
 
-def treat_multiple_fastq_matches(metadata_df, column, fastqs_in_directory, color_treatment):
+def treat_process_filterfile_values_and_checks(filterfile_df, metadata_df, color_treatment):
     """
-    This function treats if fastqs in the provided directory have multiple
-    run_accession matches in the metadata.
+    This function treats the processed values checks and returns
+    the processed information of the filterfile.
 
     Parameters
     ----------
+    filterfile_df : pandas dataframe
+        The provided filterfile dataframe to treat.
     metadata_df : pandas dataframe
-        The provided metadata dataframe.
-    column : str
-        The ENA metadata column from which the urls were obtained.
-    fastqs_in_directory : list
-        List of fastqs detected in the provided directory.
+        The provided metadata dataframe to check with.
     color_treatment: bool
         The color treatment option provided.
         True : Plain Text
         False : Colored Text
 
+    Raises
+    ------
+    OMD_CTK_Exception
+        If any warning is detected raises an exception.
+
     Returns
     -------
-    bool
-        True: There are warnings.
-        False: There are no warnings.
+    variables_4_filtering : list
+        List with "variable" column values from filterfile.
+    values_4_filtering : list
+        List with formated "values" column values from filterfile.
+    filtertypes_4_filtering : list
+        List with "filter_type" column values from filterfile.
+    actions_4_filtering : list
+        List with "action" column values from filterfile.
+    na_treatment_4_filtering : list
+        List with "NA_treatment" column values from filterfile.
+
+    """
+    #Check and process values for each variable in filter table
+    
+    ##Init list for results (internal function results)
+    print_4_filter_values_check = []
+    bools_4_filter_values_check = []
+    ##Init lists for results (results to be returned)
+    variables_4_filtering = []
+    values_4_filtering = []
+    filtertypes_4_filtering = []
+    actions_4_filtering = []
+    na_treatment_4_filtering = []
+    
+    ##For each variable
+    for i,r in filterfile_df.iterrows():
+        ##Get temp values
+        temp_variable = r['variable']
+        temp_values = r['values']
+        temp_filtertype = r['filter_type']
+        temp_action = r['action']
+        temp_na_treatment = r['NA_treatment']
+        
+        ##Get temp result check and processed values
+        temp_values_check = process_filterfile_values_and_checks(temp_variable, temp_values, temp_filtertype, metadata_df, color_treatment)
+        
+        ##Append results
+        print_4_filter_values_check.append(temp_values_check[0])
+        bools_4_filter_values_check.append(temp_values_check[1])
+        values_4_filtering.append(temp_values_check[2])
+        variables_4_filtering.append(temp_variable)
+        filtertypes_4_filtering.append(temp_filtertype)
+        actions_4_filtering.append(temp_action)
+        na_treatment_4_filtering.append(temp_na_treatment)
+    
+    ##If/else
+    ##If there are inconsistencies exception
+    if False in bools_4_filter_values_check:
+        #Prepare exception frase
+        frase0 = 'Warning! Inconsistencies detected in the "values" column of the Filter Table!\n Check your filter file!\n'
+        frase1 = '\nShowing checks by variable:'
+        frase = [frase0, frase1]
+        for i in range(len(print_4_filter_values_check)):
+            frase.append(' '.join(['\n\n' + print_4_filter_values_check[i]]))
+            frase.append(' '.join(['\n  Filter Type:', filtertypes_4_filtering[i]]))
+            frase.append(' '.join(['\n  Filter Values:', str(values_4_filtering[i])]))
+            frase.append(' '.join(['\n  Metadata Column dtype:', str(metadata_df[variables_4_filtering[i]].dtype)]))
+        #exception
+        raise OMD_CTK_Exception(' '.join(frase))
 
-    """
-    #Init results lists
-    fastqs_warnings_multiple_match = []
-    
-    #Iter and process fastq files info
-    for fastq in fastqs_in_directory:
-        #Get temp fastq information dataframe
-        temp_fastq_df = metadata_df[metadata_df[column].str.contains(fastq)]
-        #Treat info depending on temp_fastq_df len()/ Treat warnings/ Else pass
-        if len(temp_fastq_df) > 1:
-            fastqs_warnings_multiple_match.append(fastq)
-        else:
-            pass
-        
-    #Check fastqs that are in the provided directory but have multiple matches in the metadata table
-    print(rich_text_colored('\n3) Check if there are Fastq files of the provided directory with multiple matches in the Metadata Table:', 'subsection', color_treatment))
-    
-    ##If fastqs_warnings_multiple_match is empty show message/ Else show different files
-    if len(fastqs_warnings_multiple_match) == 0:
-        print(rich_text_colored('All Fastq files in the provided directory have a unique run_accession match with the Metadata Table!', 'acceptable', color_treatment))
-        #Return info for lately treat advise messages
-        return False
+    ##Else continue an return external results
     else:
-        print(rich_text_colored('\nWarning! The following Fastq files have multiple run_accession matches with the Metadata Table!', 'program_warning', color_treatment))
-        print_list_n_byline(fastqs_warnings_multiple_match, 5)
-        #Show advise messages
-        print(rich_text_colored('\nThis could be due to:','due_to_header', color_treatment))
-        print('- The presence of duplicated entries in the Metadata Table', rich_text_colored('[Warning]', 'legend_warning', color_treatment))
-        print(rich_text_colored('\nYou should:', 'you_should_header', color_treatment))
-        print('- Manually confirm that this is your case and act accordingly')
-        #Return info for lately treat advise messages
-        return True
+        return variables_4_filtering, values_4_filtering, filtertypes_4_filtering, actions_4_filtering, na_treatment_4_filtering
     
 
-def get_md5_from_ENA_column(metadata_df, column, file_name):
+def filter_metadata_variable(variable, processed_values, filter_type, filter_applied, NA_treatment, metadata_df_cp):
     """
-    This function gets the md5s for the file in the indicated ENA metadata column.
-
+    This function filters the provided metadata copy with the provided values 
+    depending on their filter_type and filter. This function processes only 
+    one input at a time.
+    
     Parameters
     ----------
-    metadata_df : pandas dataframe
-        The provided metadata dataframe.
-    column : str
-        The ENA metadata column from which the urls were obtained.
-    file_name : str
-        The Fastq file name
+    variable : str
+        The provided variable to filter the metadata table copy.
+    processed_values : list
+        The provided list of processed values used to filter the metadata table copy.
+    filter_type : str
+        The filter_type to be applied.
+        Expected values ['categorical', 'numerical']
+    filter_applied : str
+        The filter action to be applied.
+        Expected values for numerical ['equal', 'greater', 'greater_equal', 'less', 'less_equal']
+        Expected values for categorical ['keep', 'drop']
+    NA_treatment : str
+        The NA treatment to be applied.
+        Expected values ['keep', 'drop', 'no']
+    metadata_df_cp : pandas dataframe
+        The copy of the original metadata table to be filtered.
 
     Returns
     -------
-    md5_sums : list
-        The list of md5s for the seleccted ENA metadata column.
+    metadata_df_cp_f : pandas dataframe
+        A filtered version of the metadata dataframe copy.
         
     """
-    #Try/except/
-    try:
-        #Get index for row that contains file_name
-        row_index = metadata_df[metadata_df[column].str.contains(file_name)].index.values.item()
-        #Get sample fastq urls
-        file_match = metadata_df.loc[row_index][column].split(';')
-        #Get inner index
-        inner_index = [i for i, w in enumerate(file_match) if file_name in w][0]
-        #Get md5_sum for fastq file
-        if column in ['fastq_ftp', 'fastq_aspera', 'fastq_galaxy']:
-            md5_sums = metadata_df.loc[row_index]['fastq_md5'].split(';')[inner_index]
+    #Construct NA expression
+    if NA_treatment == 'keep':
+        #' | `variable`.isna()'
+        NA_expression = ''.join([' | `',variable, '`.isna()'])
+    elif NA_treatment == 'drop':
+        #' & (~`variable`.isna())'
+        NA_expression = ''.join([' & (~`',variable, '`.isna())'])
+    #Else should be 'no'
+    else:
+        pass
+        
+    #Construct filter expression
+    ##Treat numerical values
+    if filter_type == 'numerical':
+        if filter_applied == 'greater':
+            #'`variable` > processed_values[0]'
+            filter_expression = ''.join(['`',variable, '` > ', str(processed_values[0])])
+        elif filter_applied == 'greater_equal':
+            #'`variable` >= processed_values[0]'
+            filter_expression = ''.join(['`', variable, '` >= ', str(processed_values[0])])
+        elif filter_applied == 'less':
+            #'`variable` < processed_values[0]'
+            filter_expression = ''.join(['`', variable, '` < ', str(processed_values[0])])
+        elif filter_applied == 'less_equal':
+            #'`variable` <= processed_values[0]'
+            filter_expression = ''.join(['`', variable, '` <= ', str(processed_values[0])])
+        #Else should be equal
         else:
-            md5_sums = metadata_df.loc[row_index]['submitted_md5'].split(';')[inner_index]
-    except:
-        md5_sums = 'metadata_error'
-    return md5_sums
-
-
-def get_md5_checksum_for_file(path_file):
-    """
-    This function gets MD5 checksum of a file.
-
-    Parameters
-    ----------
-    path_file : str
-        Path to the file to process.
+            #'`variable` == processed_values[0]'
+            filter_expression = ''.join(['`', variable, '` == ', str(processed_values[0])])
+    ##Treat categorical values
+    else:
+        #Treat different filter options
+        if filter_applied == 'keep':
+            #Keep rows that match values in processed_values for the variable
+            #'`variable`.isin(processed_values)'
+            filter_expression = ''.join(['`', variable, '`.isin(', str(processed_values),')'])
+        else:
+            #Else should be 'drop'
+            #Drop rows that match values in processed_values for the variable
+            #'(~`variable`.isin(processed_values))'
+            filter_expression = ''.join(['(~`', variable, '`.isin(', str(processed_values),'))'])
+            
+    #Combine expressions and apply filter with query
+    if NA_treatment == 'no':
+        metadata_df_cp_f = metadata_df_cp.query(filter_expression)
+    else:
+        metadata_df_cp_f = metadata_df_cp.query(filter_expression + NA_expression)
 
-    Returns
-    -------
-    digest : str
-        The MD5 checksum of the provided file.
-        
-    """
-    try:
-        #Read file content
-        file = open(path_file, 'rb')
-        content = file.read()
-        file.close()
-    
-        #Get md5 checksum
-        md5_hash = md5()
-        md5_hash.update(content)
-        digest = md5_hash.hexdigest()
-    except:
-        digest = 'file_error'
-    return digest
+    #Return filtered table
+    return metadata_df_cp_f
 
 
-def treat_optional_md5(urls, fastqs_in_directory, metadata_df, column, directory, color_treatment):
+def treat_filter_metadata_table(processed_filterfile, metadata_df, color_treatment):
     """
-    This function treats the optional md5 check.
+    This function treats the different filters from the filterfile
+    and provides the filtered metadata table.
 
     Parameters
     ----------
-    urls : list
-        List with the fastq urls from the Metadata file.
-    fastqs_in_directory : list
-        List of fastqs detected in the provided directory.
+    processed_filterfile : tuple of lists
+        The treat_process_filterfile_values_and_checks() results.
+        Processed filterfile.
     metadata_df : pandas dataframe
         The provided metadata dataframe.
-    column : str
-        The ENA metadata column from which the urls were obtained.
-    directory : str
-        Path to the provided directory.
     color_treatment: bool
         The color treatment option provided.
         True : Plain Text
         False : Colored Text
 
+    Raises
+    ------
+    OMD_CTK_Exception
+        If the filtered metadata table is empty after applying filters raises
+        an exception.
+
     Returns
     -------
-    bool
-        True: There are warnings.
-        False: There are no warnings.
+    filtered_metadata : pandas dataframe
+        The filtered metadata dataframe.
 
-    """
-    #Show md5_checks message
-    print(rich_text_colored('\n4) Check that expected MD5s from the Metadata Table match calculated MD5s:', 'subsection', color_treatment))
-    
-    #Get md5_column based on ENA Download column provided
-    if column in ['fastq_ftp', 'fastq_aspera', 'fastq_galaxy']:
-        md5_column = 'fastq_md5'
-    else:
-        md5_column = 'submitted_md5'
-    
-    #Check that the md5_column is not all empty
-    if all(metadata_df[md5_column].isna()):
-        print(rich_text_colored('\nNone of the MD5 checksums are available for the provided ENA Download Column!', 'program_warning', color_treatment))
-        print(rich_text_colored("Skipping MD5s' check, since there is nothig to compare with!", 'program_warning', color_treatment))
-        return False
-    else:
-        #Print message
-        print(rich_text_colored('\nThis may take a while...', 'program_warning2', color_treatment))
-        
-        #Init results lists
-        warning_file_not_in_dir = []
-        warning_file_md5_not_match = []
-        warning_metadata_md5_not_found = []
-        warning_md5_file_error = []
-        
-        ##For each url try to check md5
-        for i in range(len(urls)):
-            ##Get file name
-            temp_file_name = urls[i].split('/')[-1]
-            ##Get MD5 checksum from metadata
-            temp_metadata_md5 = get_md5_from_ENA_column(metadata_df, column, temp_file_name)
-            ##Check that MD5 checksum was found
-            if temp_metadata_md5 == 'metadata_error':
-                warning_metadata_md5_not_found.append(temp_file_name)
-            else:
-                ##Check that the file is in fastqs_directory
-                file_in_directory = temp_file_name in fastqs_in_directory
-                if file_in_directory == False:
-                    warning_file_not_in_dir.append(temp_file_name)
-                else:
-                    #Get full path to file
-                    file_path = os.path.join(directory, temp_file_name)
-                    #Calcule md5 checksum
-                    calculated_md5 = get_md5_checksum_for_file(file_path)
-                    #Check if the md5s match or if there was a file_error
-                    if calculated_md5 == temp_metadata_md5:
-                        pass
-                    elif calculated_md5 == 'file_error':
-                        warning_md5_file_error.append(temp_file_name)
-                    else:
-                        warning_file_md5_not_match.append(temp_file_name)
-        
-        #Calculate total number of warning runs
-        n_file_warnings = len(warning_file_not_in_dir + warning_file_md5_not_match + warning_metadata_md5_not_found + warning_md5_file_error)
-        
-        #Show total number of runs again and total warnings
-        print('  o', rich_text_colored('Total number of Fastqs detected in Metadata Table:', 'general_text', color_treatment), len(urls))
-        print('  o', rich_text_colored('Total number of warnings for MD5s :', 'general_text', color_treatment), n_file_warnings)
-        
-        #Show different information depending on result 
-        if n_file_warnings == 0:
-            print(rich_text_colored('\nAll MD5s present in the Metadata Table match the MD5s calculated for their corresponding Fastq files!', 'acceptable', color_treatment))
-            #Return info for lately treat advise messages
-            return False
-        else:
-            ##Show warning types stats
-            print(rich_text_colored('\nMD5 Warning Types:', 'subsection2', color_treatment))
-            print('  o', rich_text_colored('Number of Fastqs with mismatches between metadata and calculated MD5s:','general_text', color_treatment), len(warning_file_md5_not_match))
-            print('  o', rich_text_colored('Number of Fastqs with errors when calculating MD5s:', 'general_text', color_treatment), len(warning_md5_file_error))
-            print('  o', rich_text_colored('Number of Fastqs not found in the provided directory:', 'general_text', color_treatment), len(warning_file_not_in_dir))
-            print('  o', rich_text_colored('Number of Fastqs with MD5s not found in the Metadata Table:', 'general_text', color_treatment), len(warning_metadata_md5_not_found))
-            
-            ##Show warning message
-            print(rich_text_colored('\nWarning! Some MD5s in the Metadata Table do not match the MD5s calculated for their corresponding Fastq files!', 'program_warning', color_treatment))
-            
-            #Show run_accession values if there are warnings
-            ##warning_file_md5_not_match
-            if len(warning_file_md5_not_match) > 0:
-                print('\n-', rich_text_colored('Fastqs with mismatches between metadata and calculated MD5s:', 'general_text', color_treatment))
-                print_list_n_byline(warning_file_md5_not_match, 5)
-            ##warning_md5_file_error
-            if len(warning_md5_file_error) > 0:
-                print('\n-', rich_text_colored('Fastqs with errors when calculating MD5s:', 'general_text', color_treatment))
-                print_list_n_byline(warning_md5_file_error, 5)
-            ##warning_file_not_in_dir
-            if len(warning_file_not_in_dir) > 0:
-                print('\n-', rich_text_colored('Fastqs not found in the provided directory:', 'general_text', color_treatment))
-                print_list_n_byline(warning_file_not_in_dir, 5)
-            ##warning_metadata_md5_not_found
-            if len(warning_metadata_md5_not_found) > 0:
-                print('\n-', rich_text_colored('Fastqs with MD5s not found in the Metadata Table:', 'general_text', color_treatment))
-                print_list_n_byline(warning_metadata_md5_not_found, 5)
-            
-            #Show advise messages
-            print(rich_text_colored('\nThis could be due to:', 'due_to_header', color_treatment))
-            print('- Memory errors when calculating MD5s', rich_text_colored('[Acceptable]', 'acceptable', color_treatment))
-            print('- The presence of untreated download errors', rich_text_colored('[Warning]', 'legend_warning', color_treatment))
-            print("- Upload errors", rich_text_colored('[Dangerous]', 'dangerous', color_treatment))
-            print(rich_text_colored('\nYou should:', 'you_should_header', color_treatment))
-            print('- Manually confirm which is your case')
-            print('- If any mismatches, try to re-download affected files')
-            print('- If any errors calculating MD5s, try to provide more memory')
-            print('- If any, check missing Fastq cases')
-            print('- If any, check missing MD5 cases')
-            print('- If necessary, contact the ENA Support (https://www.ebi.ac.uk/ena/browser/support)')
-            
-            #Return info for lately treat advise messages
-            return True
-        
+    """   
+    ##Init a copy of the metadata table for filtering
+    filtered_metadata = metadata_df
+    
+    ##Filter with the provided variables
+    for i in range(len(processed_filterfile[0])):
+        ##Get temp values
+        temp_variable = processed_filterfile[0][i]
+        temp_values = processed_filterfile[1][i]
+        temp_filtertype = processed_filterfile[2][i]
+        temp_action = processed_filterfile[3][i]
+        temp_na_treatment = processed_filterfile[4][i]
+        
+        ##Print temp filter information
+        print(rich_text_colored('\nFilter Variable: ', 'general_text', color_treatment), temp_variable)
+        print(rich_text_colored('Values: ', 'general_text', color_treatment), temp_values)
+        print(rich_text_colored('Filter Type: ', 'filter_color', color_treatment), temp_filtertype)
+        print(rich_text_colored('Filter Action: ', 'filter_color', color_treatment), temp_action)
+        print(rich_text_colored('NA Treatment: ', 'filter_color', color_treatment), temp_na_treatment)
+        
+        ##Apply filter
+        filtered_metadata = filter_metadata_variable(temp_variable, temp_values, temp_filtertype, temp_action, temp_na_treatment, filtered_metadata)
+        
+        ##Check if the metadata copy is empty after filtering
+        if filtered_metadata.empty == True:
+            #exception
+            raise OMD_CTK_Exception('Warning! The Metadata Table became empty after this last filter!\n Check your filter file and variables!')
             
+    ##Return filtered metadata table if no exceptions
+    return filtered_metadata
+
+     
 #Main Program
 def main():
     #Setting Arguments
     parser = ArgumentParser()
     ##Parameter metadata_table
     parser.add_argument(
             '-t','--metadata_table', 
             action = 'store',
             required = True,
             help = 'Metadata Table [Expected sep=TABS]. Indicate the path to the Metadata Table file.'
     )
-    ##Parameter fastqs_directory
+    ##Parameter filter_table
     parser.add_argument(
-            '-d','--fastqs_directory', 
+            '-f','--filter_table', 
             action = 'store',
-            required = True,
-            help = 'Fastqs Directory. Indicate the path to the Fastqs Directory.'
+            required = True ,
+            help = 'Filter Table [Expected sep=TABS]. Indicate the path to the Filter Table file. See Documentation for more information and format details.'
     )
-    ##Parameter ena_download_column
+    ##Parameter output_directory
     parser.add_argument(
-            '-c','--ena_download_column', 
+            '-o','--output_directory', 
             action = 'store',
-            choices = ENA_FASTQ_URLS_COLUMNS,
-            required = False,
-            default = 'fastq_ftp',
-            help = 'ENA Download Column (Optional) [Default:fastq_ftp]. Indicate the ENA Metadata Table column that was used to download Fastq files.'
-    )
-    ##Parameter fastq_pattern
-    parser.add_argument(
-            '-p','--fastq_pattern', 
-            action = 'store',
-            default = '.fastq.gz',
-            required = False,
-            help = 'Fastq File Pattern (Optional) [Default:".fastq.gz"]. Indicate the pattern to identify Fastq files.'
-    )
-    ##Parameter md5_check
-    parser.add_argument(
-            '-m', '--md5_check',
-            action = 'store_true',
             required = False,
-            help = 'MD5 Check (Optional). If indicated, it will enable MD5 Check mode.'
+            help = 'Output Directory (Optional). Indicate the path to the Output Directory. Output files will be created in the current directory if not indicated.'
     )
     ##Parameter plain_text
     parser.add_argument(
             '-x', '--plain_text',
             action = 'store_true',
             required = False,
             help = 'Plain Text Mode (Optional). If indicated, it will enable Plain Text mode, and text will appear without colors.'
@@ -488,97 +471,120 @@
             action = 'version',
             version = 'version {} ({})'.format(VERSION, DATE)
     )
     
     #Process arguments
     args = parser.parse_args()
     metadata_table_path = args.metadata_table
-    ena_download_column = args.ena_download_column
-    files_directory = args.fastqs_directory
-    fastq_pattern = args.fastq_pattern
-    md5_option = args.md5_check
+    filterfile_path = args.filter_table
+    outputdir_path = args.output_directory
     plain_text_bool = args.plain_text
     
     #Show Program headers
     print('')
     program_header('#',  __program__, 64, 2, plain_text_bool)
     print('')
     
     #Show Program parameters
     print(rich_text_colored('Program Parameters:', 'section_header', plain_text_bool))
     print(tabulate(vars(args).items(), headers = ['Argument', 'Value'], tablefmt = 'simple_outline'))
     
     #Try/Except block
     try:
         #0)Initial checks
-        #Check that provided files directory exist
-        check_existence_directory_parameter(files_directory, 'Fastqs', '--fastqs_directory')
         
-        #Try to get list of fastqs in the provided directory
-        fastqs_in_directory = get_list_fastqs_in_directory(files_directory, fastq_pattern)
+        #Check that provided output directory exist
+        check_existence_directory_parameter(outputdir_path, 'Output', '--output_directory')
         
-        #1)Try to load metadata file
+        #1)Try to load files
         
         #Section header message
-        print(rich_text_colored('\nLoading File:\n', 'section_header', plain_text_bool))
+        print(rich_text_colored('\nLoading Files:\n', 'section_header', plain_text_bool))
         
         #Try to load Metadata Table as pandas dataframe
         ##Show loading file message
         print(rich_text_colored('Metadata Table file:', 'general_text', plain_text_bool))
         print(metadata_table_path)
-        ##Load metadata file as pandas df
-        metadata = pd.read_csv(metadata_table_path, sep='\t')
-        
-        #2)Check headers used in metadata table
-        check_headers_metadata = check_headers(HEADERS_USED, metadata)
-        frase0_2 = 'Error! Some of the needed headers are not in the Metadata Table!\n Check your metadata file!\n'
-        frase1_2 = '\nThe headers needed are:'
-        treat_headers_check(HEADERS_USED, check_headers_metadata, metadata, frase0_2, frase1_2, plain_text_bool)
-        
-        #3)Try to get urls from the ena_download_column
-        urls = get_urls_from_ENA_column(metadata, ena_download_column)
-        
-        #4)Show Main information
-        
-        #Section header message
-        print(rich_text_colored('\nMain Information:', 'section_header', plain_text_bool))
-        
-        #Print main information
-        metadata_files_main_information(metadata, urls, fastqs_in_directory, plain_text_bool)
-        
-        #5)Fastq Checks 
-        
-        #Section header
-        print(rich_text_colored("\nFastqs' Checks:", 'section_header', plain_text_bool))
-        
-        #5.1)Check fastqs in metadata
-        check1 = treat_metadata_on_directory_checks(urls, fastqs_in_directory, plain_text_bool)        
-        
-        #5.2)Check fastqs in directory
-        check2 = treat_directory_on_metadata_check(urls, fastqs_in_directory, plain_text_bool)
-        
-        #5.3)Check multuple fastq matches in metadata
-        check3 = treat_multiple_fastq_matches(metadata, ena_download_column, fastqs_in_directory, plain_text_bool)
-        
-        #5.4)Treat optional md5_option 
-        if md5_option == True:
-            check4 = treat_optional_md5(urls, fastqs_in_directory, metadata, ena_download_column, files_directory, plain_text_bool)
-            functions_warnings = (check1, check2, check3, check4)
-        else:
-            functions_warnings = (check1, check2, check3)
-            
-        #6)Show Legend if warnings were detected
-        if any(functions_warnings) == True:
-            show_advise_legend(plain_text_bool)
+        ##Try to load the metadata table file
+        metadata = pd.read_csv(metadata_table_path, sep = '\t')
         
+        #Try to load Filter File as pandas dataframe
+        ##Show loading file message
+        print(rich_text_colored('\nFilter Table file:', 'general_text', plain_text_bool))
+        print(filterfile_path)
+        ##Try to load the filterfile
+        filterfile = pd.read_csv(filterfile_path, sep = '\t', dtype = 'string')
+        ##Check headers and treatment
+        check_headers_filterfile = check_headers(FILTERFILE_HEADERS, filterfile)
+        frase0_3 = 'Error! Some of the needed headers are not in the Filter Table!\n Check your filter file!\n'
+        frase1_3 = '\nThe headers needed are:'
+        treat_headers_check(FILTERFILE_HEADERS, check_headers_filterfile, filterfile, frase0_3, frase1_3, plain_text_bool)
+        
+        #2)Check that values in "variable" column from Filter File are headers in Metadata Table
+        
+        #Get list of "variable" column values in filter file
+        provided_variables = list(filterfile['variable'])
+        
+        #Check headers in metadata table and treatment
+        check_provided_variables = check_headers(provided_variables, metadata)
+        frase0_4 = 'Error! Some of the provided variables in the Filter Table do not match the Metadata Table!\n Check your filter file and/or metadata file!\n'
+        frase1_4 = '\nProvided variables are:'
+        treat_headers_check(provided_variables, check_provided_variables, metadata, frase0_4, frase1_4, plain_text_bool)
+        
+        #3)Check that "filter_type" and "action" column combinations are valid
+        
+        #Get "filter_type" and "action" column combinations in filter file
+        type_sum_filter = filterfile['filter_type'] + ' + ' + filterfile['action']
+        
+        #Check that combinations are valid and treatment
+        check_expected_type_sum_filter_values = check_values(FILTERFILE_FILTER_TYPES_ACTION_COMB, type_sum_filter)
+        frase0_5 = 'Error! Some of the "filter_type" to "action" combinations in the Filter Table are not valid!\n Check your filter file!\n'
+        frase1_5 = '\nValid combinations are:'
+        treat_values_check(FILTERFILE_FILTER_TYPES_ACTION_COMB, check_expected_type_sum_filter_values, frase0_5, frase1_5, plain_text_bool)
+        
+        #4)Check that values in "NA_treatment" column from Filter File are valid and treatment
+        check_expected_NA_treatment_values = check_values(FILTERFILE_NA_TREATMENT, filterfile['NA_treatment'])
+        frase0_6 = 'Error! Some of the values of the "NA_treatment" column in the Filter Table are not valid!\n Check your filter file!\n'
+        frase1_6 = '\nValid values are:'
+        treat_values_check(FILTERFILE_NA_TREATMENT, check_expected_NA_treatment_values, frase0_6, frase1_6, plain_text_bool)
+        
+        #5)Check that values in "values" column from Filter File has the right format and treatment
+        check_filterfile_values_column_format(filterfile, plain_text_bool)
+        
+        #6)Check and process values in "values" column from Filter File. And treatment of checks.
+        processed_filterfile = treat_process_filterfile_values_and_checks(filterfile, metadata, plain_text_bool)
+        
+        #7)Filtering metadata table
+        
+        #Previous steps
+        ##Get outfile name
+        outfile_name = 'filtered_'+metadata_table_path.split('/')[-1]
+        ##Treat output_directory parameter / Get full output file path
+        outputfile_path = treat_output_directory_parameter_outfiles(outfile_name, outputdir_path)
+        
+        #Show section header
+        print(rich_text_colored('\nFiltering Metadata Table:', 'section_header', plain_text_bool))
+        
+        #Show rows in metadata before filtering
+        print(rich_text_colored('\nNumber of rows in Provided Metadata Table:', 'subsection2', plain_text_bool), len(metadata.index))
+        
+        #Get filtered metadata table
+        filtered_metadata = treat_filter_metadata_table(processed_filterfile, metadata, plain_text_bool)
+        
+        #Show rows in metadata after filtering
+        print(rich_text_colored('\nNumber of rows in Filtered Metadata Table:', 'subsection2', plain_text_bool), len(filtered_metadata.index))
+        
+        #Show saved file message
+        print(rich_text_colored('\nSaving results in file:', 'general_text', plain_text_bool))
+        print(outputfile_path)
+        #Save filtered_metadata
+        filtered_metadata.to_csv(outputfile_path, header = True, index = False, sep = '\t')
+    
     except Exception as ex:
         print(rich_text_colored('\nThe system returned the following exception:\n', 'exception', plain_text_bool), ex)
-
-    except MemoryError:
-        print(rich_text_colored('\nThe system returned the following exception:\n', 'exception', plain_text_bool), 'MemoryError')
-    
+           
     finally:
         #Print empty line for aesthetic purposes
         print('')
 
 if __name__ == '__main__':
     main()
```

### Comparing `omdctk-1.0/src/omdctk/check_metadata_ENA.py` & `omdctk-1.1.0/src/omdctk/check_metadata_ENA.py`

 * *Files identical despite different names*

### Comparing `omdctk-1.0/src/omdctk/download_fastqs_ENA.py` & `omdctk-1.1.0/src/omdctk/download_fastqs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
-@program: download_fastqs_ENA.py
+@program: download_fastqs.py
 @author: Samuel Piquer-Esteban
-@date: 7 Jul 2023 
+@date: 16 Feb 2024 
 
 """
 
 #Set program name
-__program__ = 'download_fastqs_ENA.py'
+__program__ = 'download_fastqs.py'
 
 #Imports from MTD_CT common module
 from omdctk import (DATE, VERSION, ENA_FASTQ_URLS_COLUMNS, OMD_CTK_Exception, 
                     program_header, get_urls_from_ENA_column, rich_text_colored,
                     check_existence_directory_parameter, 
                     check_headers, treat_headers_check,
                     treat_output_directory_parameter,
@@ -287,15 +287,15 @@
     ##Parameter mode
     parser.add_argument(
             '-m','--mode', 
             action = 'store',
             choices = ['ENA','LINKS'],
             required = False,
             default = 'ENA',
-            help = 'Execution Mode (Optional) [Default:ENA]. Options: 1) ENA Metadata Table File [Expected sep=TABS] or 2) Links TXT File.'
+            help = 'Execution Mode (Optional) [Default:ENA]. Options: 1) ENA Metadata Table File [Expected sep=TABS] or 2) Links TXT File for generic file download.'
     )
     ##Parameter ena_download_column
     parser.add_argument(
             '-c','--ena_download_column', 
             action = 'store',
             choices = ENA_FASTQ_URLS_COLUMNS,
             required = False,
@@ -345,17 +345,18 @@
     inputfile_path = args.input_file
     inputfile_type = args.mode
     outputdir_path = args.output_directory
     ena_download_column = args.ena_download_column
     n_max_conn = args.max_conn
     parfive_verb = args.parfive_verbose
     plain_text_bool = args.plain_text
-    #Skip ena_download_column if LINKS mode is used
+    #Skip ena_download_column if LINKS mode is used(this is only for aesthetic purposes when showing program headers)
+    #It is indiferent since ena_download_column its only used in ENA_mode to get URLs
     if inputfile_type == 'LINKS':
-        args.ENA_download_column = None
+        args.ena_download_column = None
     
     #Show Program headers
     print('')
     program_header('#',  __program__, 64, 2, plain_text_bool)
     print('')
     
     #Show Program parameters
@@ -394,16 +395,21 @@
         ##Get outfile name
         out_name_errors = 'errors_report.tsv'
         ##Treat output_directory parameter / Get full output file path
         outputfile_errors = treat_output_directory_parameter_outfiles(out_name_errors, outputdir_path)
         
         #Save erros dataframe if there are errors
         if len(errors_df) != 0:
+            #Treat warning file initial message depending on mode(for aesthetics)
+            if (parfive_verb == True) or (len(urls) > len(errors_df)):
+                warning_file_frase = '\nError Report Generated!'
+            else:
+                warning_file_frase = 'Error Report Generated!'
             #Show error report message
-            print(rich_text_colored('\nError Report Generated!','program_warning', plain_text_bool))
+            print(rich_text_colored(warning_file_frase,'program_warning', plain_text_bool))
             #Show the number of detected error
             print(rich_text_colored('Total Download Errors Detected:', 'general_text', plain_text_bool), len(errors_df))
             #Show saved file message
             print(rich_text_colored('\nSaving report in file:', 'general_text', plain_text_bool))
             print(outputfile_errors)
             #Save df_merge_ENA
             errors_df.to_csv(outputfile_errors, header = True, index = False, sep = '\t')
```

### Comparing `omdctk-1.0/src/omdctk/download_metadata_ENA.py` & `omdctk-1.1.0/src/omdctk/download_metadata_ENA.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 @program: download_metadata_ENA.py
 @author: Samuel Piquer-Esteban
-@date: 7 Jul 2023 
+@date: 5 Mar 2024 
 
 """
 
 #Set program name
 __program__ = 'download_metadata_ENA.py'
 
 #Imports from MTD_CT common module
@@ -235,15 +235,17 @@
         #Previous steps
         ##Get outfile name
         out_name_ena = study_accession + '_ENA_metadata.tsv'
         ##Treat output_directory parameter / Get full output file path
         outputfile_ena = treat_output_directory_parameter_outfiles(out_name_ena, outputdir_path)
         
         #Join both tables by run accession (left join)
-        df_merge_ENA = pd.merge(tech_table, mgtoolkit_table, left_on = 'run_accession', right_on = 'Run', how = 'left')
+        #We indicate the lef sufflix as None, to avoid renaming of technical columns in case of identical columns in mg-toolkit metadata
+        #I.e. 'scientific_name' column
+        df_merge_ENA = pd.merge(tech_table, mgtoolkit_table, left_on = 'run_accession', right_on = 'Run', how = 'left', suffixes = (None, '_y'))
         
         #Show saved file message
         print(rich_text_colored('\nSaving results in file:', 'general_text', plain_text_bool))
         print(outputfile_ena)
         #Save df_merge_ENA
         df_merge_ENA.to_csv(outputfile_ena, header = True, index = False, sep = '\t')
```

### Comparing `omdctk-1.0/src/omdctk/filter_metadata.py` & `omdctk-1.1.0/src/omdctk/treat_fastqs.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,509 +1,550 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
-@program: filter_metadata.py
+@program: treat_fastqs.py
 @author: Samuel Piquer-Esteban
 @date: 7 Jul 2023 
 
 """
 
 #Set program name
-__program__ = 'filter_metadata.py'
+__program__ = 'treat_fastqs.py'
 
 #Imports from MTD_CT common module
-from omdctk import (DATE, VERSION, OMD_CTK_Exception, program_header, 
+from omdctk import (DATE, VERSION, TEMPLATE_FINAL_COLUMNS, VALID_FASTQ_TYPES,
+                    VALID_TREATMENTS, OMD_CTK_Exception, program_header, 
                     check_existence_directory_parameter, 
+                    check_fastq_PAIRED_patterns, print_list_n_byline,
+                    get_list_fastqs_in_directory, rich_text_colored,
                     check_headers, treat_headers_check,
-                    check_values, treat_values_check,
-                    treat_output_directory_parameter_outfiles,
-                    rich_text_colored)
+                    check_values, treat_values_check, check_na_in_pandas_dataframe,
+                    check_duplicates_in_fastq_names, treat_check_fastq_name_type,
+                    check_treatment_for_samples, check_rename_samples, check_merge_samples)
 
 #Import third-party modules
 from argparse import ArgumentParser
 from tabulate import tabulate
-from ast import literal_eval
 import pandas as pd
-
-#Program Constants
-FILTERFILE_HEADERS = ['variable', 'values', 'filter_type', 'action', 'NA_treatment']
-
-FILTERFILE_FILTER_TYPES_ACTION_COMB = ['categorical + keep', 'categorical + drop',
-                                       'numerical + greater', 'numerical + greater_equal', 
-                                       'numerical + equal', 'numerical + less',
-                                       'numerical + less_equal']
-
-FILTERFILE_NA_TREATMENT = ['drop', 'keep', 'no']
+import shutil
+import os
 
 #Program Functions
-def check_filterfile_values_column_format(filterfile_df, color_treatment):
+def check_directories_are_not_identical(input_dir, output_dir):
     """
-    This function checks the format of the provided values
-    in the "values" column of the filter file.
+    This function checks if the provided directories are the same or not.
 
     Parameters
     ----------
-    filterfile_df : pandas dataframe
-        The provided filterfile dataframe.
-    color_treatment: bool
-        The color treatment option provided.
-        True : Plain Text
-        False : Colored Text
+    input_dir : str
+        Path to the Input Directory.
+    output_dir : str
+        Path to the Output Directory.
 
     Raises
     ------
     OMD_CTK_Exception
-        If format inconsistencies are detected raises an exception.
+        If both directories are the same raises an exception.
 
     Returns
     -------
     None.
 
     """
-    #Check format(list) for values
-    format_checks = []
-    for val in filterfile_df['values']:
-        try: 
-            #Try to strip start and end spaces
-            strip_val = val.strip()
-            #Check list format
-            if strip_val.startswith('[') and strip_val.endswith(']'):
-                format_checks.append(True)
-            else:
-                format_checks.append(False)
-        except:
-            format_checks.append(False)
-    
-    #Check empty cells
-    NAs_checks = list(filterfile_df['values'].isna())
-    
-    #Combine checks
-    result_bools = []
-    result_prints = []
-    for i in range(len(format_checks)):
-        #Wrong format and Not NA
-        if format_checks[i] == False and NAs_checks[i] == False:
-            result_bools.append(False)
-            print_strn = ' '.join(['-', rich_text_colored(filterfile_df['variable'][i], 'check_color', color_treatment), rich_text_colored('Does not have the expected "[]" format!', 'program_warning', color_treatment)])
-            result_prints.append(print_strn)
-        #Wrong format and NA
-        elif format_checks[i] == False and NAs_checks[i] == True:
-            result_bools.append(False)
-            print_strn = ' '.join(['-', rich_text_colored(filterfile_df['variable'][i], 'check_color', color_treatment), rich_text_colored('Cell is empty!', 'program_warning', color_treatment)])
-            result_prints.append(print_strn)
-        #Right format (It will never be NA)
-        else:
-            result_bools.append(True)
-            print_strn = ' '.join(['-', rich_text_colored(filterfile_df['variable'][i], 'check_color', color_treatment), rich_text_colored('Everything seems okay!', 'acceptable', color_treatment)])
-            result_prints.append(print_strn)
+    same_dir = os.path.samefile(input_dir, output_dir)
     
-    #Treat final checks
-    if False in result_bools:
+    if same_dir == True:
+        raise OMD_CTK_Exception('Error! The provided Input and Output directories are the same!')
+
+
+def check_fastq_file_exits(list_fastq_files, fastqs_in_directory, n_elements):
+    """
+    This function checks if all files in the list of fastq files are
+    present in the list of fastq files of the Input Directory.
+
+    Parameters
+    ----------
+    list_fastq_files : list
+        List with the fastq files from the Treatment Template.
+    fastqs_in_directory : list
+        List of fastqs detected in the Input Directory.
+    n_elements : int
+        The number of elements to be printed by line.
+        
+    Raises
+    ------
+    OMD_CTK_Exception
+        If absent Fastq files are detected raises an exception.
+
+    Returns
+    -------
+    None.
+    
+    """
+    #Get asymmetric difference between list
+    fastqs_difference = list(set(list_fastq_files) - set(fastqs_in_directory))
+        
+    #If difference is not empty raise exception
+    if len(fastqs_difference) > 0:
         #Prepare exception frase
-        frase0 = 'Error! Some of the values of the "values" column in the Filter Table are not valid!\n Check your filter file!\n'
-        frase1 = '\nShowing checks by variable:'
+        frase0 = 'Error! Some of the Fastq files in the Treatmente Template are not in the Input Directory!\n'
+        frase1 = '\nThe following files were absent:\n'
         frase = [frase0, frase1]
-        for i in result_prints:
-            temp_line = ' '.join(['\n', i])
+        #Split file names
+        splited_list = [fastqs_difference[i:i+n_elements] for i in range(0, len(fastqs_difference), n_elements)]
+        for i in splited_list:
+            #Format depending on if it is the last line
+            if i == splited_list[-1]:
+                temp_line = ', '.join(i)
+            else:
+                temp_line = ', '.join(i+['\n'])
+            #Append line
             frase.append(temp_line)
         #Raise exception
         raise OMD_CTK_Exception(' '.join(frase))
+        
     
-    
-def curly_2_straight_quotation(value):
+def cat_files(list_inputfiles, outputfile, color_treatment):
     """
-    This function replaces curly for straight quotation
-    in a string.
+    This function cats files together in the specified file.
+    It works with both gz compressed and uncompressed Fastq files.
 
     Parameters
     ----------
-    value : str
-        Provided str to replace characters.
+    list_inputfiles : list
+        The list of paths for the input gzip files to cat.
+    outputfile : str
+        The path for the resulting output gzip file.
+    color_treatment: bool
+        The color treatment option provided.
+        True : Plain Text
+        False : Colored Text
 
     Returns
     -------
-    str
-        Result str with replaced characters.
-
-    """
-    #curly_2_straight_quotation
-    return value.replace("“", '"').replace("”", '"').replace("‘", "'").replace("’", "'")
+    bool
+        True: There are warnings.
+        False: There are no warnings.
     
-         
-def check_values_inv(pandas_column, list_values):
     """
-    This function checks if all values in a list are in a pandas_colum.
+    try:
+        with open(outputfile,'wb') as output:
+            for file in list_inputfiles:
+                with open(file,'rb') as inputs:
+                    shutil.copyfileobj(inputs, output)
+    except:
+        print(rich_text_colored('Error! These files could not be successfully concatenated!', 'exception', color_treatment))
+        return True
+    else:
+        return False
+
+
+def treat_cat_files(sample_df, fastq_type, input_directory_path, output_directory_path, type_pattern, color_treatment):
+    """
+    This function treats the provided sample fastq type files to cat them together.
 
     Parameters
     ----------
-    pandas_column : pandas dataframe column
-        The provided pandas dataframe column used as reference.
-    list_values : list
-        The provided list of values to check.
+    sample_df : pandas dataframe
+        The provided sample dataframe.
+    fastq_type : str
+        The fastq type assigned to the fastq file.
+    input_directory_path : str
+        Path to the Input Directory.
+    output_directory_path : str
+        Path to the Output Directory.
+    type_pattern : str
+        The pattern associated to the provided fastq_type.
+    color_treatment: bool
+        The color treatment option provided.
+        True : Plain Text
+        False : Colored Text
 
     Returns
     -------
     result : bool
-        True: all values in the list are in the pandas_colum.
-        False: not all values in the list are in the pandas_colum.
-        
+        True: There are warnings.
+        False: There are no warnings.
+
     """
-    result = all(elem in list(pandas_column) for elem in list_values)
+    #Get sample_name
+    sample_name = list(set(sample_df['sample_name']))[0]   
+    
+    #Get type info
+    sample_df_type = sample_df[sample_df['fastq_type'] == fastq_type]
     
+    #Get fastq_name and output_path
+    fastq_name = sample_name + type_pattern
+    output_path = os.path.join(output_directory_path, fastq_name)
+    
+    #Get list of input files(and sort by name)
+    input_files = list(sample_df_type['fastq_file_name'])
+    input_files.sort()
+    input_paths = [os.path.join(input_directory_path, file) for file in input_files]
+    
+    #Print cat configuration
+    print(input_files, ' > ', fastq_name)
+    
+    #Cat the gzip files and return bool value
+    result = cat_files(input_paths, output_path, color_treatment)
     return result
+    
 
-
-def process_filterfile_values_and_checks(variable, values, filter_type, metadata_df, color_treatment):
+def merge_mode(sample_df, input_directory_path, output_directory_path, fastq_pattern, R1_pattern, R2_pattern, color_treatment):
     """
-    This function processes the provided values and runs various checks 
-    depending on their filter_type. This function processes only one 
-    input at a time. 
+    This function merges fastq files from the same sample and prints messages.
 
     Parameters
     ----------
-    variable : str
-        The provided variable to check(colname in metadata table).
-    values : str
-        The provided values to check.
-    filter_type : str
-        the filter_type to be applied.
-        Expected values ['categorical','numerical']
-    metadata_df : pandas dataframe
-        The provided metadata dataframe to check with.
+    sample_df : pandas dataframe
+        Pandas dataframe with all the information of the sample files.
+    input_directory_path : str
+        The provided Input Directory.
+    output_directory_path : str
+        The provided Output Directory.
+    fastq_pattern : str
+        The Fastq File Pattern provided.
+    R1_pattern : str
+        The R1 File Pattern provided.
+    R2_pattern : str
+        The R2 File Pattern provided.
     color_treatment: bool
         The color treatment option provided.
         True : Plain Text
         False : Colored Text
 
     Returns
     -------
-    print_strn : str
-        Colored string message indicating if everything is okey (green) or
-        if there is any warning to check (red).
-    bool_value : bool
-        Bool value indicating if everything is okey (True) or there is
-        any warning to check (False).
-    result_value : list
-        The list of provided values processed to properly interact with the
-        metadata table.
+    result : bool
+        True: There are warnings.
+        False: There are no warnings.
         
     """
-    #Pre-process values until get a list of multiple or single values
-    ##Convert curly to straight quotation(in case file has been edited in calc, or excel)
-    pre_values = curly_2_straight_quotation(values)
-    ##Try to evaluate string to convert it to list
-    try:
-        post_values = literal_eval(pre_values)
-    except:
-        print_strn = ' '.join(['-', rich_text_colored(variable, 'check_color', color_treatment), rich_text_colored('The provided values can not be converted to list!', 'program_warning', color_treatment)])
-        bool_value = False
-        result_value = pre_values
+    #Init bool results list
+    bools_list = []
+    
+    #List of fastq_types
+    temp_list_fastqtypes = list(sample_df['fastq_type'])
+    
+    #Get temp number of types
+    temp_n_pair1 = temp_list_fastqtypes.count('pair1')
+    temp_n_pair2 = temp_list_fastqtypes.count('pair2')
+    temp_n_single = temp_list_fastqtypes.count('single')   
+       
+    #Treat different configurations
+    ##Paired files with orphan single fastq files with the same number of files
+    if temp_n_pair1 > 1 and temp_n_pair2 > 1 and temp_n_single > 1 and temp_n_pair1 == temp_n_pair2 and temp_n_pair1 == temp_n_single:
+        #Show message paired
+        print(rich_text_colored('Paired Merging:', 'treatment_mode_color', color_treatment))
+        #Generate pair1 file and add bool
+        catp1 = treat_cat_files(sample_df, 'pair1', input_directory_path, output_directory_path, R1_pattern, color_treatment)
+        bools_list.append(catp1)
+        #Generate pair2 file and add bool 
+        catp2 = treat_cat_files(sample_df, 'pair2', input_directory_path, output_directory_path, R2_pattern, color_treatment)
+        bools_list.append(catp2)
+        
+        #Show message single
+        print(rich_text_colored('Single Merging:', 'treatment_mode_color', color_treatment))
+        #Generate pair2 file and add bool 
+        cat_s = treat_cat_files(sample_df, 'single', input_directory_path, output_directory_path, fastq_pattern, color_treatment)
+        bools_list.append(cat_s)
+    #More than one single fastq file but no pair1 or pair2 files
+    elif temp_n_pair1 == 0 and temp_n_pair2 == 0 and temp_n_single>1:
+        #Show message single
+        print(rich_text_colored('Single Merging:', 'treatment_mode_color', color_treatment))
+        #Generate pair2 file and add bool 
+        cat_s = treat_cat_files(sample_df, 'single', input_directory_path, output_directory_path, fastq_pattern, color_treatment)
+        bools_list.append(cat_s)
+    #More than one fastq file for pair1 and pair2 with the same sumber of files, no single files 
+    elif temp_n_single == 0 and temp_n_pair1 > 1 and temp_n_pair2 > 1 and temp_n_pair1 == temp_n_pair2:
+        #Show message paired
+        print(rich_text_colored('Paired Merging:', 'treatment_mode_color', color_treatment))
+        #Generate pair1 file and add bool
+        catp1 = treat_cat_files(sample_df, 'pair1', input_directory_path, output_directory_path, R1_pattern, color_treatment)
+        bools_list.append(catp1)
+        #Generate pair2 file and add bool 
+        catp2 = treat_cat_files(sample_df, 'pair2', input_directory_path, output_directory_path, R2_pattern, color_treatment)
+        bools_list.append(catp2)
+    #Pass because we have ruled out this possibility previusly with check_merge_samples() function
     else:
-        #Check that the list is not empty
-        if len(post_values) == 0:
-            print_strn = ' '.join(['-', rich_text_colored(variable, 'check_color', color_treatment), rich_text_colored('The provided list is empty!', 'program_warning', color_treatment)])
-            bool_value = False
-            result_value = post_values
-        else:
-            #Type_filter checks
-            ##Treat numerical type_filters values
-            if filter_type == 'numerical':
-                #Get metadata column dtype
-                metadata_colum_dtype = metadata_df[variable].dtype
-                ##If column in metadata table is numerical continue/ else stop
-                if metadata_colum_dtype == int or metadata_colum_dtype == float:
-                    ##Numerical filter values must be a unique number
-                    if len(post_values) == 1:
-                        #Check that the value is int or float
-                        if type(post_values[0]) == int or type(post_values[0]) == float:
-                            print_strn = ' '.join(['-', rich_text_colored(variable, 'check_color', color_treatment), rich_text_colored('Everything seems okay!', 'acceptable', color_treatment)])
-                            bool_value = True
-                            result_value = post_values
-                        else:
-                            print_strn = ' '.join(['-', rich_text_colored(variable, 'check_color', color_treatment), rich_text_colored('The provided value is not numerical!', 'program_warning', color_treatment)])
-                            bool_value = False
-                            result_value = post_values
-                    else:
-                        print_strn = ' '.join(['-', rich_text_colored(variable, 'check_color', color_treatment), rich_text_colored('Values for numerical filters must be a unique number!', 'program_warning', color_treatment)])
-                        bool_value = False
-                        result_value = post_values
-                else:
-                    print_strn = ' '.join(['-', rich_text_colored(variable, 'check_color', color_treatment), rich_text_colored('Is not a numerical variable in the Metadata Table!', 'program_warning', color_treatment)])
-                    bool_value = False
-                    result_value = post_values
-            ##Treat categorical type_filters values
-            else:
-                #Check if ALL the provided categorical values are in the corresponding column in metadata table
-                bool_value = check_values_inv(metadata_df[variable], post_values)
-                result_value = post_values
-                #If true continue/ else warning
-                if bool_value == True:
-                    print_strn = ' '.join(['-', rich_text_colored(variable, 'check_color', color_treatment), rich_text_colored('Everything seems okay!', 'acceptable', color_treatment)])
-                else:
-                    print_strn = ' '.join(['-', rich_text_colored(variable, 'check_color', color_treatment), rich_text_colored('Some of the provided values are not in the Metadata Table!', 'program_warning', color_treatment)])
-            
-    return print_strn, bool_value, result_value
-
+        pass
+    #Return bool value / Check if theare are any warnings with this sample
+    return any(bools_list)
 
-def treat_process_filterfile_values_and_checks(filterfile_df, metadata_df, color_treatment):
+        
+def rename_mode(sample_name, fastq_file_name, fastq_type, input_directory_path, output_directory_path, fastq_pattern, R1_pattern, R2_pattern, color_treatment):
     """
-    This function treats the processed values checks and returns
-    the processed information of the filterfile.
+    This function copies a fastq file with a new name in the provided 
+    Output Directory and prints messages.
 
     Parameters
     ----------
-    filterfile_df : pandas dataframe
-        The provided filterfile dataframe to treat.
-    metadata_df : pandas dataframe
-        The provided metadata dataframe to check with.
+    sample_name : str
+        The sample name of the file that will be used as the new file name.
+    fastq_file_name : str
+        The file name in the provided Input Directory.
+    fastq_type : str
+        The type of fastq file [single, pair1, pair2].
+    input_directory_path : str
+        The provided Input Directory.
+    output_directory_path : str
+        The provided Output Directory.
+    fastq_pattern : str
+        The Fastq File Pattern provided.
+    R1_pattern : str
+        The R1 File Pattern provided.
+    R2_pattern : str
+        The R2 File Pattern provided.
     color_treatment: bool
         The color treatment option provided.
         True : Plain Text
         False : Colored Text
 
-    Raises
-    ------
-    OMD_CTK_Exception
-        If any warning is detected raises an exception.
-
     Returns
     -------
-    variables_4_filtering : list
-        List with "variable" column values from filterfile.
-    values_4_filtering : list
-        List with formated "values" column values from filterfile.
-    filtertypes_4_filtering : list
-        List with "filter_type" column values from filterfile.
-    actions_4_filtering : list
-        List with "action" column values from filterfile.
-    na_treatment_4_filtering : list
-        List with "NA_treatment" column values from filterfile.
-
-    """
-    #Check and process values for each variable in filter table
-    
-    ##Init list for results (internal function results)
-    print_4_filter_values_check = []
-    bools_4_filter_values_check = []
-    ##Init lists for results (results to be returned)
-    variables_4_filtering = []
-    values_4_filtering = []
-    filtertypes_4_filtering = []
-    actions_4_filtering = []
-    na_treatment_4_filtering = []
-    
-    ##For each variable
-    for i,r in filterfile_df.iterrows():
-        ##Get temp values
-        temp_variable = r['variable']
-        temp_values = r['values']
-        temp_filtertype = r['filter_type']
-        temp_action = r['action']
-        temp_na_treatment = r['NA_treatment']
-        
-        ##Get temp result check and processed values
-        temp_values_check = process_filterfile_values_and_checks(temp_variable, temp_values, temp_filtertype, metadata_df, color_treatment)
-        
-        ##Append results
-        print_4_filter_values_check.append(temp_values_check[0])
-        bools_4_filter_values_check.append(temp_values_check[1])
-        values_4_filtering.append(temp_values_check[2])
-        variables_4_filtering.append(temp_variable)
-        filtertypes_4_filtering.append(temp_filtertype)
-        actions_4_filtering.append(temp_action)
-        na_treatment_4_filtering.append(temp_na_treatment)
-    
-    ##If/else
-    ##If there are inconsistencies exception
-    if False in bools_4_filter_values_check:
-        #Prepare exception frase
-        frase0 = 'Warning! Inconsistencies detected in the "values" column of the Filter Table!\n Check your filter file!\n'
-        frase1 = '\nShowing checks by variable:'
-        frase = [frase0, frase1]
-        for i in range(len(print_4_filter_values_check)):
-            frase.append(' '.join(['\n\n' + print_4_filter_values_check[i]]))
-            frase.append(' '.join(['\n  Filter Type:', filtertypes_4_filtering[i]]))
-            frase.append(' '.join(['\n  Filter Values:', str(values_4_filtering[i])]))
-            frase.append(' '.join(['\n  Metadata Column dtype:', str(metadata_df[variables_4_filtering[i]].dtype)]))
-        #exception
-        raise OMD_CTK_Exception(' '.join(frase))
+    result : bool
+        True: There are warnings.
+        False: There are no warnings.
 
-    ##Else continue an return external results
+    """
+    #Treat single and paired files and get new names
+    if fastq_type == 'pair1':
+        fastq_name = sample_name + R1_pattern
+    elif fastq_type == 'pair2':
+        fastq_name = sample_name + R2_pattern
     else:
-        return variables_4_filtering, values_4_filtering, filtertypes_4_filtering, actions_4_filtering, na_treatment_4_filtering
+        fastq_name = sample_name + fastq_pattern
+    
+    #Show message
+    print([fastq_file_name], ' > ', fastq_name)
+    
+    #Set input and output paths
+    output_path = os.path.join(output_directory_path, fastq_name)
+    input_path = os.path.join(input_directory_path, fastq_file_name)
+    
+    #Try to copy file in output directory
+    try:
+        shutil.copyfile(input_path, output_path)    
+    except:
+        print(rich_text_colored('Error! This file could not be successfully renamed in the Output Directory!', 'exception', color_treatment))
+        return True
+    else:
+        return False
     
-
-def filter_metadata_variable(variable, processed_values, filter_type, filter_applied, NA_treatment, metadata_df_cp):
-    """
-    This function filters the provided metadata copy with the provided values 
-    depending on their filter_type and filter. This function processes only 
-    one input at a time.
     
+def copy_only_mode(fastq_file_name, input_directory_path, output_directory_path, color_treatment):
+    """
+    This function copies a file in the provided Output Directory.
+
     Parameters
     ----------
-    variable : str
-        The provided variable to filter the metadata table copy.
-    processed_values : list
-        The provided list of processed values used to filter the metadata table copy.
-    filter_type : str
-        The filter_type to be applied.
-        Expected values ['categorical', 'numerical']
-    filter_applied : str
-        The filter action to be applied.
-        Expected values for numerical ['equal', 'greater', 'greater_equal', 'less', 'less_equal']
-        Expected values for categorical ['keep', 'drop']
-    NA_treatment : str
-        The NA treatment to be applied.
-        Expected values ['keep', 'drop', 'no']
-    metadata_df_cp : pandas dataframe
-        The copy of the original metadata table to be filtered.
+    fastq_file_name : str
+        The file name in the provided Input Directory.
+    input_directory_path : str
+        The provided Input Directory.
+    output_directory_path : str
+        The provided Output Directory.
+    color_treatment: bool
+        The color treatment option provided.
+        True : Plain Text
+        False : Colored Text
 
     Returns
     -------
-    metadata_df_cp_f : pandas dataframe
-        A filtered version of the metadata dataframe copy.
+    result : bool
+        True: There are warnings.
+        False: There are no warnings.
         
     """
-    #Construct NA expression
-    if NA_treatment == 'keep':
-        #' | `variable`.isna()'
-        NA_expression = ''.join([' | `',variable, '`.isna()'])
-    elif NA_treatment == 'drop':
-        #' & (~`variable`.isna())'
-        NA_expression = ''.join([' & (~`',variable, '`.isna())'])
-    #Else should be 'no'
-    else:
-        pass
-        
-    #Construct filter expression
-    ##Treat numerical values
-    if filter_type == 'numerical':
-        if filter_applied == 'greater':
-            #'`variable` > processed_values[0]'
-            filter_expression = ''.join(['`',variable, '` > ', str(processed_values[0])])
-        elif filter_applied == 'greater_equal':
-            #'`variable` >= processed_values[0]'
-            filter_expression = ''.join(['`', variable, '` >= ', str(processed_values[0])])
-        elif filter_applied == 'less':
-            #'`variable` < processed_values[0]'
-            filter_expression = ''.join(['`', variable, '` < ', str(processed_values[0])])
-        elif filter_applied == 'less_equal':
-            #'`variable` <= processed_values[0]'
-            filter_expression = ''.join(['`', variable, '` <= ', str(processed_values[0])])
-        #Else should be equal
-        else:
-            #'`variable` == processed_values[0]'
-            filter_expression = ''.join(['`', variable, '` == ', str(processed_values[0])])
-    ##Treat categorical values
-    else:
-        #Treat different filter options
-        if filter_applied == 'keep':
-            #Keep rows that match values in processed_values for the variable
-            #'`variable`.isin(processed_values)'
-            filter_expression = ''.join(['`', variable, '`.isin(', str(processed_values),')'])
-        else:
-            #Else should be 'drop'
-            #Drop rows that match values in processed_values for the variable
-            #'(~`variable`.isin(processed_values))'
-            filter_expression = ''.join(['(~`', variable, '`.isin(', str(processed_values),'))'])
-            
-    #Combine expressions and apply filter with query
-    if NA_treatment == 'no':
-        metadata_df_cp_f = metadata_df_cp.query(filter_expression)
+    #Show message
+    print([fastq_file_name],' > ',fastq_file_name)
+    
+    #Set input and output paths
+    output_path = os.path.join(output_directory_path, fastq_file_name)
+    input_path = os.path.join(input_directory_path, fastq_file_name)
+    
+    #Try to copy file in output directory
+    try:
+        shutil.copyfile(input_path, output_path)    
+    except:
+        print(rich_text_colored('Error! This file could not be successfully copied in the Output Directory!', 'exception', color_treatment))
+        return True
     else:
-        metadata_df_cp_f = metadata_df_cp.query(filter_expression + NA_expression)
+        return False
 
-    #Return filtered table
-    return metadata_df_cp_f
 
-
-def treat_filter_metadata_table(processed_filterfile, metadata_df, color_treatment):
+def treat_files(treatment_df, unique_samples_list, input_directory_path, output_directory_path, fastq_pattern, R1_pattern, R2_pattern, color_treatment):
     """
-    This function treats the different filters from the filterfile
-    and provides the filtered metadata table.
+    This function treats the provided Fastq files based on the Treatment Template.
 
     Parameters
     ----------
-    processed_filterfile : tuple of lists
-        The treat_process_filterfile_values_and_checks() results.
-        Processed filterfile.
-    metadata_df : pandas dataframe
-        The provided metadata dataframe.
+    treatment_df : pandas dataframe
+        The provided treatment dataframe.
+    unique_samples_list : list
+        List of unique sample_names in Treatment Template.
+    input_directory_path : str
+        The provided Input Directory.
+    output_directory_path : str
+        The provided Output Directory.
+    fastq_pattern : str
+        The Fastq File Pattern provided.
+    R1_pattern : str
+        The R1 File Pattern provided.
+    R2_pattern : str
+        The R2 File Pattern provided.
     color_treatment: bool
         The color treatment option provided.
         True : Plain Text
         False : Colored Text
 
-    Raises
-    ------
-    OMD_CTK_Exception
-        If the filtered metadata table is empty after applying filters raises
-        an exception.
-
     Returns
     -------
-    filtered_metadata : pandas dataframe
-        The filtered metadata dataframe.
-
-    """   
-    ##Init a copy of the metadata table for filtering
-    filtered_metadata = metadata_df
-    
-    ##Filter with the provided variables
-    for i in range(len(processed_filterfile[0])):
-        ##Get temp values
-        temp_variable = processed_filterfile[0][i]
-        temp_values = processed_filterfile[1][i]
-        temp_filtertype = processed_filterfile[2][i]
-        temp_action = processed_filterfile[3][i]
-        temp_na_treatment = processed_filterfile[4][i]
-        
-        ##Print temp filter information
-        print(rich_text_colored('\nFilter Variable: ', 'general_text', color_treatment), temp_variable)
-        print(rich_text_colored('Values: ', 'general_text', color_treatment), temp_values)
-        print(rich_text_colored('Filter Type: ', 'filter_color', color_treatment), temp_filtertype)
-        print(rich_text_colored('Filter Action: ', 'filter_color', color_treatment), temp_action)
-        print(rich_text_colored('NA Treatment: ', 'filter_color', color_treatment), temp_na_treatment)
-        
-        ##Apply filter
-        filtered_metadata = filter_metadata_variable(temp_variable, temp_values, temp_filtertype, temp_action, temp_na_treatment, filtered_metadata)
-        
-        ##Check if the metadata copy is empty after filtering
-        if filtered_metadata.empty == True:
-            #exception
-            raise OMD_CTK_Exception('Warning! The Metadata Table became empty after this last filter!\n Check your filter file and variables!')
-            
-    ##Return filtered metadata table if no exceptions
-    return filtered_metadata
+    None.
 
-     
+    """
+    #Init warning samples
+    warning_samples = []
+    
+    #A)Show main information pre-treatment
+    ##Print information Title
+    print(rich_text_colored('\nPre-treatment Information:\n', 'section_header', color_treatment))
+    ##Show the number of samples
+    print('  o', rich_text_colored('Number of Samples in Treatment Template:', 'subsection', color_treatment), len(unique_samples_list))
+    ##Show the number of files
+    print('  o', rich_text_colored('Number of Fastq files in Treatment Template:', 'subsection', color_treatment), len(treatment_df['fastq_file_name']))   
+    
+    #B)Get files for each sample_name and treat
+    ##Section header
+    print(rich_text_colored('\nTreat Fastqs:', 'section_header', color_treatment))
+    ##Treat FASTQS per sample
+    for sample in unique_samples_list:
+        #Filter table by sample
+        temp_sample = treatment_df[treatment_df['sample_name'] == sample]
+        #Get treatment(get unique with set function)
+        ##NOTE: Up to this point we have check there is only one treatment per sample
+        temp_treatment = list(temp_sample['treatment'])[0]
+        #List of fastq_types
+        temp_list_fastqtypes = list(temp_sample['fastq_type'])
+        #Get temp number of types
+        temp_n_pair1 = temp_list_fastqtypes.count('pair1')
+        temp_n_pair2 = temp_list_fastqtypes.count('pair2')
+        temp_n_single = temp_list_fastqtypes.count('single')
+        
+        #Messages                            
+        ##Show sample ID
+        print(rich_text_colored('\nSample: ', 'treatment_color', color_treatment), sample)
+        ##Show Treatments present
+        print(rich_text_colored('Treatment:', 'treatment_color', color_treatment), temp_treatment)
+        ##Show number of files
+        print(rich_text_colored('Number of Fastq files:', 'general_text', color_treatment), len(temp_sample['fastq_file_name']))
+        ##Show files configuration
+        print(rich_text_colored('Configuration: ', 'general_text', color_treatment) + ''.join(['Number of pair1(s) = ', str(temp_n_pair1), '; Number of pair2(s) = ', str(temp_n_pair2), '; Number of single(s) = ', str(temp_n_single)]))
+        
+        #Treat different
+        if temp_treatment == 'merge':
+            #Merge sample's files
+            sample_result = merge_mode(temp_sample, input_directory_path, output_directory_path, fastq_pattern, R1_pattern, R2_pattern, color_treatment)
+            #If warnings were detected add sample to list
+            if sample_result == True:
+                warning_samples.append(sample)
+        else:
+            if temp_treatment == 'rename':
+                print(rich_text_colored('Renaming file(s):', 'treatment_mode_color', color_treatment))
+            else:
+                print(rich_text_colored('Copying file(s):', 'treatment_mode_color', color_treatment))
+            #Apply treatments by files of sample
+            #Iter files
+            for i,r in temp_sample.iterrows():
+                #Get temp file values
+                temp_file = r['fastq_file_name']
+                temp_file_type = r['fastq_type']
+                #Treat modes
+                if temp_treatment == 'rename':
+                    #Change name for file sample name
+                    file_result = rename_mode(sample, temp_file, temp_file_type, input_directory_path, output_directory_path, fastq_pattern, R1_pattern, R2_pattern, color_treatment)
+                else:
+                    #Copy file sample
+                    file_result = copy_only_mode(temp_file, input_directory_path, output_directory_path, color_treatment)
+                #If warnings were detected for file add sample to list
+                if file_result == True:
+                    warning_samples.append(sample)
+    
+    
+    #C)Show main information pre-treatment
+    ##Previous steps
+    fastqs_in_outputdir = get_list_fastqs_in_directory(output_directory_path, fastq_pattern)
+    
+    ##Print information Title
+    print(rich_text_colored('\nPost-treatment Information:\n', 'section_header', color_treatment))
+    ##Show the number of files
+    print('  o', rich_text_colored('Number of Fastq files in Output Directory:', 'subsection', color_treatment), len(fastqs_in_outputdir))
+    
+    #D)Show saved file message
+    print(rich_text_colored('\nResulting files saved in:', 'general_text', color_treatment))
+    print(output_directory_path)
+    
+    #E)Treat warnings
+    ##Remove duplicates
+    warning_samples = list(set(warning_samples))
+    ##Show message
+    if len(warning_samples) > 0:
+        print(rich_text_colored('Error! Some of the samples in the Treatment Template showed warnings when trying to treat their files!', 'program_warning', color_treatment))
+        print('\nThe following samples present warnings:')
+        print_list_n_byline(warning_samples, 5)
+        
+        
 #Main Program
 def main():
     #Setting Arguments
     parser = ArgumentParser()
-    ##Parameter metadata_table
+    ##Parameter treatment_file
     parser.add_argument(
-            '-t','--metadata_table', 
+            '-t','--treatment_template', 
             action = 'store',
-            required = True,
-            help = 'Metadata Table [Expected sep=TABS]. Indicate the path to the Metadata Table file.'
+            required = True ,
+            help = 'Treatment Template [Expected sep=TABS]. Indicate the path to the Treatment Template file. See Documentation for more information and format details.'
     )
-    ##Parameter filter_table
+    ##Parameter input_directory
     parser.add_argument(
-            '-f','--filter_table', 
+            '-i','--input_directory', 
             action = 'store',
-            required = True ,
-            help = 'Filter Table [Expected sep=TABS]. Indicate the path to the Filter Table file. See Documentation for more information and format details.'
+            required = True,
+            help = 'Input Directory. Indicate the path to the Input Directory with the Fastq files to treat.'
     )
     ##Parameter output_directory
     parser.add_argument(
             '-o','--output_directory', 
             action = 'store',
+            required = True,
+            help = 'Output Directory. Indicate the path to the Output Directory to save the resulting treated Fastq files.'
+    )
+    ##Parameter fastq_pattern
+    parser.add_argument(
+            '-p','--fastq_pattern', 
+            action = 'store',
+            default = '.fastq.gz',
+            required = False,
+            help = 'Fastq File Pattern (Optional) [Default:".fastq.gz"]. Indicate the pattern to identify Fastq files.'
+    )
+    ##Parameter r1_patterns
+    parser.add_argument(
+            '-r1','--r1_pattern', 
+            action = 'store',
+            default = '_1.fastq.gz',
             required = False,
-            help = 'Output Directory (Optional). Indicate the path to the Output Directory. Output files will be created in the current directory if not indicated.'
+            help = 'R1 File Pattern (Optional) [Default:"_1.fastq.gz"]. Indicate the pattern to identify R1 PAIRED Fastq files.'
+    )
+    ##Parameter r2_patterns
+    parser.add_argument(
+            '-r2','--r2_pattern', 
+            action = 'store',
+            default = '_2.fastq.gz',
+            required = False,
+            help = 'R2 File Pattern (Optional) [Default:"_2.fastq.gz"]. Indicate the pattern to identify R2 PAIRED Fastq files.'
     )
     ##Parameter plain_text
     parser.add_argument(
             '-x', '--plain_text',
             action = 'store_true',
             required = False,
             help = 'Plain Text Mode (Optional). If indicated, it will enable Plain Text mode, and text will appear without colors.'
@@ -513,17 +554,20 @@
             '-v','--version',
             action = 'version',
             version = 'version {} ({})'.format(VERSION, DATE)
     )
     
     #Process arguments
     args = parser.parse_args()
-    metadata_table_path = args.metadata_table
-    filterfile_path = args.filter_table
+    treatment_file_path = args.treatment_template
+    inputdir_path = args.input_directory
     outputdir_path = args.output_directory
+    fastq_pattern = args.fastq_pattern
+    r1_files_pattern = args.r1_pattern
+    r2_files_pattern = args.r2_pattern
     plain_text_bool = args.plain_text
     
     #Show Program headers
     print('')
     program_header('#',  __program__, 64, 2, plain_text_bool)
     print('')
     
@@ -531,97 +575,103 @@
     print(rich_text_colored('Program Parameters:', 'section_header', plain_text_bool))
     print(tabulate(vars(args).items(), headers = ['Argument', 'Value'], tablefmt = 'simple_outline'))
     
     #Try/Except block
     try:
         #0)Initial checks
         
+        #Check that provided files directory exist
+        check_existence_directory_parameter(inputdir_path, 'Input', '--input_directory')
+        
         #Check that provided output directory exist
         check_existence_directory_parameter(outputdir_path, 'Output', '--output_directory')
         
-        #1)Try to load files
+        #Check that directories are not the same
+        check_directories_are_not_identical(inputdir_path, outputdir_path)
+        
+        #Check PAIRED Fastq patterns
+        check_fastq_PAIRED_patterns(fastq_pattern, r1_files_pattern, r2_files_pattern)
+        
+        #Try to get list of fastqs in the provided directory
+        fastqs_in_directory = get_list_fastqs_in_directory(inputdir_path, fastq_pattern)
+        
+        #1)Try to load treatment file
         
         #Section header message
         print(rich_text_colored('\nLoading Files:\n', 'section_header', plain_text_bool))
         
-        #Try to load Metadata Table as pandas dataframe
+        #Try to load Treatment Template file as pandas dataframe
         ##Show loading file message
-        print(rich_text_colored('Metadata Table file:', 'general_text', plain_text_bool))
-        print(metadata_table_path)
-        ##Try to load the metadata table file
-        metadata = pd.read_csv(metadata_table_path, sep = '\t')
+        print(rich_text_colored('Treatment Template file:', 'general_text', plain_text_bool))
+        print(treatment_file_path)
+        ##Load metadata file as pandas df
+        treatment_table = pd.read_csv(treatment_file_path, sep='\t')
+
+        #2)Checks related to the treatment file
+        
+        ##Check headers in file and messages
+        check_headers_treatmentfile = check_headers(TEMPLATE_FINAL_COLUMNS, treatment_table)
+        frase0_1 = 'Error! Some of the needed headers are not in the Treatment Template!\n Check your treatment file!\n'
+        frase1_1 = '\nThe headers needed are:'
+        treat_headers_check(TEMPLATE_FINAL_COLUMNS, check_headers_treatmentfile, treatment_table, frase0_1, frase1_1, plain_text_bool)
+        
+        ##Check that values in "fastq_type" column from Treatment Template are valid and treatment
+        check_expected_fastq_type_values = check_values(VALID_FASTQ_TYPES, treatment_table['fastq_type'])
+        frase0_2 = 'Error! Some of the values of the "fastq_type" column in the Treatment Template are not valid!\n Check your treatment file!\n'
+        frase1_2 = '\nValid values are:'
+        treat_values_check(VALID_FASTQ_TYPES, check_expected_fastq_type_values, frase0_2, frase1_2, plain_text_bool)
+        
+        ##Check that values in "treatment" column from Treatment Template are valid and treatment
+        check_expected_treatment_values = check_values(VALID_TREATMENTS, treatment_table['treatment'])
+        frase0_3 = 'Error! Some of the values of the "treatment" column in the Treatment Template are not valid!\n Check your treatment file!\n'
+        frase1_3 = '\nValid values are:'
+        treat_values_check(VALID_TREATMENTS, check_expected_treatment_values, frase0_3, frase1_3, plain_text_bool)
+        
+        ##Check that there are no NA values in "sample_name" column from Treatment Template
+        frase4 = 'Error! Some of the values of the "sample_name" column in the Treatment Template are NAs!\n Check your treatment file!'
+        check_na_in_pandas_dataframe(treatment_table['sample_name'], frase4)
+        
+        ##Check that there are no NA values in "fastq_file_name" column from Treatment Template
+        frase5 = 'Error! Some of the values of the "fastq_file_name" column in the Treatment Template are NAs!\n Check your treatment file!'
+        check_na_in_pandas_dataframe(treatment_table['fastq_file_name'], frase5)
+        
+        ##Check that there are not duplicate names in "fastq_file_name" column
+        check_duplicates_in_fastq_names(treatment_table, 5)
+                
+        #3)Checks per file
+        
+        ##Check that all files in Treatment Template have matching file names and fastq types
+        treat_check_fastq_name_type(treatment_table, fastq_pattern, r1_files_pattern, r2_files_pattern, 5)
+        
+        ##Check that all files in Treatment Template are in the Input Directory
+        list_fastq_files = list(treatment_table['fastq_file_name'])
+        check_fastq_file_exits(list_fastq_files, fastqs_in_directory, 5)
+
+        #4)Checks per sample
+        
+        ##Get unique sample names and sort
+        unique_sample_names = list(set(treatment_table['sample_name']))
+        unique_sample_names.sort()
+        
+        ##Check mixed treatments per sample
+        check_treatment_for_samples(treatment_table, unique_sample_names, 5)
+        
+        ##Check rename mode files configurations per sample
+        check_rename_samples(treatment_table, unique_sample_names, plain_text_bool)
+        
+        ##Check merge mode files configurations per sample
+        check_merge_samples(treatment_table, unique_sample_names, plain_text_bool)
+        
+        #5)Treat Fastq files
+
+        ##Treat Fastq files
+        treat_files(treatment_table, unique_sample_names, inputdir_path, outputdir_path, fastq_pattern, r1_files_pattern, r2_files_pattern, plain_text_bool)
         
-        #Try to load Filter File as pandas dataframe
-        ##Show loading file message
-        print(rich_text_colored('\nFilter Table file:', 'general_text', plain_text_bool))
-        print(filterfile_path)
-        ##Try to load the ena table file
-        filterfile = pd.read_csv(filterfile_path, sep = '\t', dtype = 'string')
-        ##Check headers and treatment
-        check_headers_filterfile = check_headers(FILTERFILE_HEADERS, filterfile)
-        frase0_3 = 'Error! Some of the needed headers are not in the Filter Table!\n Check your filter file!\n'
-        frase1_3 = '\nThe headers needed are:'
-        treat_headers_check(FILTERFILE_HEADERS, check_headers_filterfile, filterfile, frase0_3, frase1_3, plain_text_bool)
-        
-        #2)Check that values in "variable" column from Filter File are headers in Metadata Table
-        
-        #Get list of "variable" column values in filter file
-        provided_variables = list(filterfile['variable'])
-        
-        #Check headers in metadata table and treatment
-        check_provided_variables = check_headers(provided_variables, metadata)
-        frase0_4 = 'Error! Some of the provided variables in the Filter Table do not match the Metadata Table!\n Check your filter file and/or metadata file!\n'
-        frase1_4 = '\nProvided variables are:'
-        treat_headers_check(provided_variables, check_provided_variables, metadata, frase0_4, frase1_4, plain_text_bool)
-        
-        #3)Check that "filter_type" and "action" column combinations are valid
-        
-        #Get "filter_type" and "action" column combinations in filter file
-        type_sum_filter = filterfile['filter_type'] + ' + ' + filterfile['action']
-        
-        #Check that combinations are valid and treatment
-        check_expected_type_sum_filter_values = check_values(FILTERFILE_FILTER_TYPES_ACTION_COMB, type_sum_filter)
-        frase0_5 = 'Error! Some of the "filter_type" to "action" combinations in the Filter Table are not valid!\n Check your filter file!\n'
-        frase1_5 = '\nValid combinations are:'
-        treat_values_check(FILTERFILE_FILTER_TYPES_ACTION_COMB, check_expected_type_sum_filter_values, frase0_5, frase1_5, plain_text_bool)
-        
-        #4)Check that values in "NA_treatment" column from Filter File are valid and treatment
-        check_expected_NA_treatment_values = check_values(FILTERFILE_NA_TREATMENT, filterfile['NA_treatment'])
-        frase0_6 = 'Error! Some of the values of the "NA_treatment" column in the Filter Table are not valid!\n Check your filter file!\n'
-        frase1_6 = '\nValid values are:'
-        treat_values_check(FILTERFILE_NA_TREATMENT, check_expected_NA_treatment_values, frase0_6, frase1_6, plain_text_bool)
-        
-        #5)Check that values in "values" column from Filter File has the right format and treatment
-        check_filterfile_values_column_format(filterfile, plain_text_bool)
-        
-        #6)Check and process values in "values" column from Filter File. And treatment of checks.
-        processed_filterfile = treat_process_filterfile_values_and_checks(filterfile, metadata, plain_text_bool)
-        
-        #7)Filtering metadata table
-        
-        #Previous steps
-        ##Get outfile name
-        outfile_name = 'filtered_'+metadata_table_path.split('/')[-1]
-        ##Treat output_directory parameter / Get full output file path
-        outputfile_path = treat_output_directory_parameter_outfiles(outfile_name, outputdir_path)
-        
-        #Show section header
-        print(rich_text_colored('\nFiltering Metadata Table:', 'section_header', plain_text_bool))
-        
-        #Get filtered metadata table
-        filtered_metadata = treat_filter_metadata_table(processed_filterfile, metadata, plain_text_bool)
-        
-        #Show saved file message
-        print(rich_text_colored('\nSaving results in file:', 'general_text', plain_text_bool))
-        print(outputfile_path)
-        #Save filtered_metadata
-        filtered_metadata.to_csv(outputfile_path, header = True, index = False, sep = '\t')
-    
     except Exception as ex:
         print(rich_text_colored('\nThe system returned the following exception:\n', 'exception', plain_text_bool), ex)
            
     finally:
         #Print empty line for aesthetic purposes
         print('')
-
+                                                                                                   
 if __name__ == '__main__':
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `omdctk-1.0/src/omdctk/make_treatment_template_ENA.py` & `omdctk-1.1.0/src/omdctk/concat_datasets.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,285 +1,231 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
-@program: make_treatment_template_ENA.py
+@program: concat_datasets.py
 @author: Samuel Piquer-Esteban
-@date: 7 Jul 2023 
+@date: 21 Feb 2024 
 
 """
 
 #Set program name
-__program__ = 'make_treatment_template_ENA.py'
+__program__ = 'concat_datasets.py'
 
 #Imports from MTD_CT common module
-from omdctk import (DATE, VERSION, ENA_FASTQ_URLS_COLUMNS, TEMPLATE_FINAL_COLUMNS, 
-                    OMD_CTK_Exception, program_header, check_existence_directory_parameter, 
-                    check_fastq_PAIRED_patterns, rich_text_colored,
-                    get_list_fastqs_in_directory, print_list_n_byline,
-                    check_headers, treat_headers_check,
-                    get_urls_from_ENA_column, 
-                    metadata_files_main_information,
-                    treat_output_directory_parameter_outfiles)
+from omdctk import (DATE, VERSION, VALID_REQUIREDNESS, OMD_CTK_Exception, program_header, treat_headers_check,
+                    check_headers, check_duplicates_in_variables_dict_column, check_required_variables_in_metadata_table, 
+                    check_metadata_table_vars_in_dict, treat_output_directory_parameter_outfiles, check_na_in_pandas_dataframe,
+                    check_existence_directory_parameter, treat_values_check, check_values, rich_text_colored)
 
 #Import third-party modules
 from argparse import ArgumentParser
 from tabulate import tabulate
 import pandas as pd
+import os
 
 #Program Constants
-DEFAULT_SAMPLE_COLUMNS = ['sample_accession', 'secondary_sample_accession',
-                          'run_accession', 'library_name', 'run_alias', 
-                          'sample_alias', 'sample_title']
+VARIABLES_FILE_HEADERS_4_CONCAT = ['variable', 'requiredness']
 
-#Program Functions
-def check_colname_duplicates(possible_sample_names, color_treatment):
+#Program functions
+def treat_output_file_prefix_name(prefix, file_name):
     """
-    This function checks if the possible columns for sample names provided match
-    the final template column names.
+    This function creates the name for the file treating 
+    the --output_name_prefix parameter.
 
     Parameters
     ----------
-    possible_sample_names : list
-        List with the possible columns to use as sample name column.
-    color_treatment: bool
-        The color treatment option provided.
-        True : Plain Text
-        False : Colored Text
-
-    Raises
-    ------
-    OMD_CTK_Exception
-        If the possible columns provided match the final template columns names
-        raises an exception.
+    prefix : str
+        The provided output_name_prefix parameter.
+    file_name : str
+        The name of the file.
 
     Returns
     -------
-    None.
+    final_name : str
+        The final name of the file.
 
     """
-    #Init results list
-    column_duplicates = []
-    
-    #Check if the possible sample column names match the TEMPLATE_FINAL_COLUMNS
-    for possible_name in possible_sample_names:
-        if possible_name in TEMPLATE_FINAL_COLUMNS:
-            column_duplicates.append(possible_name)
-    
-    #Raise exception if duplicates are detected
-    if len(column_duplicates) > 0:
-        #Prepare exception frase
-        frase0 = 'Error! Some of the sample name columns provided match with the final template columns names!\n'
-        frase1 = '\nPlease, change the following column names in the provided Metadata Table:'
-        frase = [frase0, frase1]
-        for i in column_duplicates:
-            temp_line = ' '.join(['\n-', rich_text_colored(i, 'check_color', color_treatment)])
-            frase.append(temp_line)
-        #Raise exception
-        raise OMD_CTK_Exception(' '.join(frase))
+    if prefix is None:
+        final_name = file_name
+    else:
+        final_name = prefix + '_' + file_name
+    return final_name
 
 
-def check_fastqs_uniqueness(metadata_df, column, fastqs_in_directory, color_treatment):
+def get_path_files_in_directory(directory, pattern):
     """
-    This function checks if the provided Fastqs have a unique match in the 
-    Metadata Table.
+    This function gets a list with the files of the provided 
+    directory for the provided pattern.
 
     Parameters
     ----------
-    metadata_df : pandas dataframe
-        The provided metadata dataframe.
-    column : str
-        The ENA metadata column from which the urls were obtained.
-    fastqs_in_directory : list
-        List of fastqs detected in the provided directory.
-    color_treatment: bool
-        The color treatment option provided.
-        True : Plain Text
-        False : Colored Text
-
+    directory : str
+        Path to the directory.
+    pattern : str
+        Extension pattern to recognize the wanted files.
+        
     Raises
     ------
     OMD_CTK_Exception
-        If there are Fastqs that do not have a unique entry in the metadata 
-        raises an exception.
+        If there are no files detected raises an exception.
 
     Returns
     -------
-    None.
-
-    """
-    #Init results lists
-    fastqs_warnings_more_than_one_match = []
-    fastqs_warnings_zero_matches = []
-    
-    #Iter and process fastq files info
-    for fastq in fastqs_in_directory:
-        #Get temp fastq information dataframe
-        temp_fastq_df = metadata_df[metadata_df[column].str.contains(fastq)]
-        #Treat info depending on temp_fastq_df len()/ Treat warnings/ Else pass
-        if len(temp_fastq_df) == 1:
-            pass
-        elif len(temp_fastq_df) > 1:
-            fastqs_warnings_more_than_one_match.append(fastq)
-        else:
-            fastqs_warnings_zero_matches.append(fastq)
+    wanted_files : list
+        List of the wanted files paths.
     
-    #If there are warnings raise exception
-    if len(fastqs_warnings_more_than_one_match) > 0 or len(fastqs_warnings_zero_matches) > 0:
-        if len(fastqs_warnings_more_than_one_match) > 0:
-            print(rich_text_colored('\nWarning! The following Fastq files in the provided directory have more than one match in the Metadata Table!', 'program_warning', color_treatment))
-            print_list_n_byline(fastqs_warnings_more_than_one_match, 5)
-        elif len(fastqs_warnings_zero_matches) > 0:
-            print(rich_text_colored('\nWarning! The following Fastq files in the provided directory do not have a match in the Metadata Table!', 'program_warning', color_treatment))
-            print_list_n_byline(fastqs_warnings_zero_matches, 5)
-        raise OMD_CTK_Exception('Error! Some of the Fastqs in the provided directory do not have a unique match with the Metadata Table (zero or more than one match)!')    
-
-
-def get_fastq_type(fastq_name, r1_pattern, r2_pattern):
     """
-    This function gets the fastq_type from fastq_file_name.
-
-    Parameters
-    ----------
-    fastq_name : str
-        Fastq file name in fastqs directory.
-    r1_pattern : str
-        The provided pair1 pattern.
-    r2_pattern : str
-        The provided pair2 pattern.
-
-    Returns
-    -------
-    result : str
-        Returns the fastq_type [pair1, pair2 or single] 
-        for the provided fastq file name.
-    """   
-    if fastq_name.endswith(r1_pattern):
-        result = 'pair1'
-    elif fastq_name.endswith(r2_pattern):
-        result = 'pair2'
-    else:
-        result = 'single'
-    return result
+    #Get files in directory
+    files = os.listdir(directory)
+    
+    #Filter to retain only fastq.gz files
+    wanted_files = [x for x in files if x.endswith(pattern)]
+    
+    #Check if fastq files were detected
+    if len(wanted_files) == 0:
+        frase0 = 'Error! There are no files with pattern "'
+        frase1 = '" in the provided Input Directory!'
+        raise OMD_CTK_Exception(''.join([frase0, pattern, frase1]))
+    
+    #Get full paths
+    wanted_files_full_path = [os.path.join(directory, x) for x in wanted_files]
+    
+    return wanted_files_full_path
 
 
-def contruct_template(metadata_df, column, fastqs_in_directory, possible_sample_names, r1_files_pattern, r2_files_pattern):
+def get_path_files_in_project_mode(directory, pattern, color_treatment):
     """
-    This function constructs the template dataframe.
+    This function gets a list with the files with the provided pattern
+    at the inmidiate subdir childs of the provided directory.
 
     Parameters
     ----------
-    metadata_df : pandas dataframe
-        The provided metadata dataframe.
-    column : str
-        The ENA metadata column from which the urls were obtained.
-    fastqs_in_directory : list
-        List of fastqs detected in the provided directory.
-    possible_sample_names : list
-        List with the possible columns to use as sample names.
-    r1_files_pattern : str
-        The provided R1 File Pattern.
-    r2_files_pattern : str
-        The provided R2 File Pattern.
+    directory : str
+        Path to the directory.
+    pattern : str
+        Extension pattern to recognize files of interest.
+    color_treatment: bool
+        The color treatment option provided.
+        True : Plain Text
+        False : Colored Text
+        
+    Raises
+    ------
+    OMD_CTK_Exception
+        If there are no final metadata files detected or more than one matching file raises an excepcion.
 
     Returns
     -------
-    template : pandas dataframe
-        The resulting template dataframe.
-
+    mt_files_paths : list
+        List of the final metadata files paths.
+    
     """
-    #Init empty pandas dataframe
-    template=pd.DataFrame()
+    #Set results list
+    mt_files_paths = []
     
-    #Set template columns
-    template_columns = ['sample_name'] + possible_sample_names + ['fastq_file_name', 'fastq_type', 'treatment']
+    #Get list of child subdirs
+    datasets = next(os.walk(directory))[1]
+    
+    #If there are no child subdirs raise exception
+    if len(datasets) == 0:
+        raise OMD_CTK_Exception(''.join(['Error! For Search Mode: project. The provided Input Directory has no child subdirectories (datasets)!']))
+    else:
+        #Show message indicating number of datasets detected
+        print('\n-',rich_text_colored('Total Datasets (child directories) detected:', 'general_text', color_treatment), len(datasets))
+    #For each dataset check if there is a final metadata file
+    for p in datasets:
+        #Get child dir path
+        temp_child_path = os.path.join(directory, p)
+        
+        #Get files in child directory
+        temp_files = os.listdir(temp_child_path)
     
-    #Iter and process fastq files info
-    for fastq in fastqs_in_directory:
-        #Get temp fastq information dataframe
-        temp_fastq_df = metadata_df[metadata_df[column].str.contains(fastq)]
-        #Extract info
-        temp_row = []
-        ##Add empty sample_name
-        temp_row.append('')
-        ##Add values for each possible_sample_name
-        for i in possible_sample_names:
-            temp_row.append(temp_fastq_df[i].values[0])
-        ##Add fastq_file_name
-        temp_row.append(fastq)
-        ##Add fastq_type using get_fastq_type()
-        temp_row.append(get_fastq_type(fastq, r1_files_pattern, r2_files_pattern))
-        ##Add empty treatment
-        temp_row.append('')
-        #Save info in dataframe
-        temp_template = pd.DataFrame([temp_row], columns = template_columns)
-        template = pd.concat([template, temp_template], ignore_index = True)
+        #Filter to retain only files with extension
+        mt_temp_files = [x for x in temp_files if x.endswith(pattern)]
+        
+        #Check if files were detected
+        ##If there were none raise exception
+        if len(mt_temp_files) == 0:
+            raise OMD_CTK_Exception(''.join(['Error! For Dataset: ', p, '. There are no files with pattern extension "', pattern,'"!']))
+        ##If there were more that 1 ask the user what to do
+        elif len(mt_temp_files) > 1:
+            
+            #Initial message informing that there is more than one wanted matching file in dataset folder
+            
+            ##Show warning message
+            print(rich_text_colored(''.join(['\nWarning! There is more than one file with pattern extension "', pattern,'" for the following Dataset: ', p,'!']), 'program_warning2', color_treatment))
+            ##Show files in dataset folder
+            print(rich_text_colored('\nThe following files were found:', 'general_text', color_treatment))
+            for file in mt_temp_files:
+                print(file)
+        
+            #Little menu to see what the user wants to do
+            ##Get initial input
+            print(rich_text_colored('\nDo you want to add all the found files anyway?', 'general_text', color_treatment))
+            response = input('Provide a valid answer {y, n}:')
+            ##While loop only valid answer
+            while response not in ('y','n'):
+                response = input('Provide a valid answer {y, n}:')
+            ##Continue
+            else:
+                ##If it is okay continue and add all files
+                if response == 'y':
+                    for file in mt_temp_files:
+                        mt_files_paths.append(os.path.join(temp_child_path, file))
+                ##Else raise exception
+                else:
+                    raise OMD_CTK_Exception(''.join(['Error! For Dataset: ', p,'. There were unespected files with pattern extension "', pattern,'"!']))
+        ##If there was only one file add normally
+        else:
+            mt_files_paths.append(os.path.join(temp_child_path, mt_temp_files[0]))
     
-    #Return final template
-    return template
+    return mt_files_paths
 
 
 #Main Program
 def main():
     #Setting Arguments
     parser = ArgumentParser()
-    #Setting Arguments
-    parser = ArgumentParser()
-    ##Parameter metadata_table
+    ##Parameter input_directory
     parser.add_argument(
-            '-t','--metadata_table', 
+            '-i','--input_directory',
             action = 'store',
             required = True,
-            help = 'Metadata Table [Expected sep=TABS]. Indicate the path to the Metadata Table file.'
+            help ='Input Directory. Indicate the path to the Input Directory with the Datasets Metadata files.'
     )
-    ##Parameter fastqs_directory
+    ##Parameter variables_dictionary
     parser.add_argument(
-            '-d','--fastqs_directory', 
+            '-d','--variables_dictionary',
             action = 'store',
             required = True,
-            help = 'Fastqs Directory. Indicate the path to the Fastqs Directory.'
+            help ='Variables Dictionary [Expected sep=TABS]. Indicate path to the Variables Dictionary file. See Documentation for more information and format details.'
     )
-    ##Parameter ena_download_column
+    ##Parameter search_mode
     parser.add_argument(
-            '-c','--ena_download_column', 
+            '-s','--search_mode', 
             action = 'store',
-            choices = ENA_FASTQ_URLS_COLUMNS,
+            choices = ['simple','project'],
             required = False,
-            default = 'fastq_ftp',
-            help = 'ENA Download Column (Optional) [Default:fastq_ftp]. Indicate the ENA Metadata Table column that was used to download Fastq files.'
-    ) 
-    ##Parameter fastq_pattern
-    parser.add_argument(
-            '-p','--fastq_pattern', 
-            action = 'store',
-            default = '.fastq.gz',
-            required = False,
-            help = 'Fastq File Pattern (Optional) [Default:".fastq.gz"]. Indicate the pattern to identify Fastq files.'
+            default = 'simple',
+            help = 'Search Mode (Optional) [Default:simple]. Indicate the selected mode to search metadata files for each dataset. Options: 1) Simple (all files are in the provided Input Directory) or 2) Project (the provided Input Directory has one folder for each dataset with their own files).'
     )
-    ##Parameter r1_pattern
+    ##Parameter metadata_pattern
     parser.add_argument(
-            '-r1','--r1_pattern', 
+            '-p','--metadata_pattern', 
             action = 'store',
-            default = '_1.fastq.gz',
             required = False,
-            help = 'R1 File Pattern (Optional) [Default:"_1.fastq.gz"]. Indicate the pattern to identify R1 PAIRED Fastq files.'
+            default = '_metadata_final.tsv',
+            help = 'Dataset Metadata File Pattern (Optional) [Default:"_metadata_final.tsv"]. Indicate the pattern to identify Dataset Metadata files.'
     )
-    ##Parameter r2_pattern
+    ##Parameter output_file_prefix
     parser.add_argument(
-            '-r2','--r2_pattern', 
+            '-op','--output_name_prefix', 
             action = 'store',
-            default = '_2.fastq.gz',
             required = False,
-            help = 'R2 File Pattern (Optional) [Default:"_2.fastq.gz"]. Indicate the pattern to identify R2 PAIRED Fastq files.'
-    )
-    ##Parameter extra_sample_columns
-    parser.add_argument(
-            '-e','--extra_sample_columns', 
-            nargs = '+',
-            required = False,
-            help = 'Extra Sample Columns (Optional). Indicate the column names for the extra possible sample names separated by spaces (If a column name has spaces, quote it).'
+            help = 'Output Name Prefix (Optional). Indicate prefix name for the output files.'
     )
     ##Parameter output_directory
     parser.add_argument(
             '-o','--output_directory', 
             action = 'store',
             required = False,
             help = 'Output Directory (Optional). Indicate the path to the Output Directory. Output files will be created in the current directory if not indicated.'
@@ -294,118 +240,134 @@
     ##Parameter version
     parser.add_argument(
             '-v','--version',
             action = 'version',
             version = 'version {} ({})'.format(VERSION, DATE)
     )
     
-    #Process arguments
+    #Process common arguments
     args = parser.parse_args()
-    metadata_table_path = args.metadata_table
-    ena_download_column = args.ena_download_column
-    files_directory = args.fastqs_directory
+    input_path = args.input_directory
+    search_mode = args.search_mode
+    files_pattern = args.metadata_pattern
     outputdir_path = args.output_directory
-    extra_sample_names = args.extra_sample_columns
-    fastq_pattern = args.fastq_pattern
-    r1_files_pattern = args.r1_pattern
-    r2_files_pattern = args.r2_pattern
+    output_name_prefix = args.output_name_prefix
+    variables_dictionary_path = args.variables_dictionary
     plain_text_bool = args.plain_text
-        
+    
     #Show Program headers
     print('')
     program_header('#',  __program__, 64, 2, plain_text_bool)
     print('')
     
     #Show Program parameters
     print(rich_text_colored('Program Parameters:', 'section_header', plain_text_bool))
     print(tabulate(vars(args).items(), headers = ['Argument', 'Value'], tablefmt = 'simple_outline'))
     
-    #Try/Except block
+    #Check if the files exists and load files/ Try-except-else
     try:
-        #0)Initial checks
-        
-        #Check that provided files directory exist
-        check_existence_directory_parameter(files_directory, 'Fastqs', '--fastqs_directory')
+        #0) Initial checks and steps
         
-        #Check that provided output directory exist
+        ##Check that provided input directory exist
+        check_existence_directory_parameter(input_path, 'Input', '--input_directory')
+    
+        ##Check that provided output directory exist
         check_existence_directory_parameter(outputdir_path, 'Output', '--output_directory')
         
-        #Check PAIRED Fastq patterns
-        check_fastq_PAIRED_patterns(fastq_pattern, r1_files_pattern, r2_files_pattern)
-        
-        #Try to get list of Fastq files in the fastqs directory and sort by name
-        fastqs_in_directory = get_list_fastqs_in_directory(files_directory, fastq_pattern)
-        fastqs_in_directory.sort()
-        
-        #1)Try to load metadata file
-        
+        #1) Search files in Input Directory
         #Section header message
-        print(rich_text_colored('\nLoading File:\n', 'section_header', plain_text_bool))
-        
-        #Try to load Metadata Table as pandas dataframe
-        ##Show loading file message
-        print(rich_text_colored('Metadata Table file:', 'general_text', plain_text_bool))
-        print(metadata_table_path)
-        ##Load metadata file as pandas df
-        metadata = pd.read_csv(metadata_table_path, sep='\t')
-        
-        #2)Check headers used in metadata table and set possible_sample_names
-        
-        #Define headers used and possible_sample_names
-        ##Set variables
-        possible_sample_names = DEFAULT_SAMPLE_COLUMNS
-        headers_used = DEFAULT_SAMPLE_COLUMNS + ENA_FASTQ_URLS_COLUMNS
-        ##If extra_column parameters are given add to headers to be used if they are not already present
-        if type(extra_sample_names) == list:
-            possible_sample_names = list(set(DEFAULT_SAMPLE_COLUMNS + extra_sample_names))
-            headers_used = list(set(DEFAULT_SAMPLE_COLUMNS + ENA_FASTQ_URLS_COLUMNS + extra_sample_names))
-
-        #Do checks and messages
-        check_headers_metadata = check_headers(headers_used, metadata)
-        frase0_2 = 'Error! Some of the needed headers are not in the Metadata Table!\n Check your metadata file!\n'
-        frase1_2 = '\nThe headers needed are:'
-        treat_headers_check(headers_used, check_headers_metadata, metadata, frase0_2, frase1_2, plain_text_bool)
-        
-        #3)Check that the possible_sample_names do not have a match with the final template column names 
-        check_colname_duplicates(possible_sample_names, plain_text_bool)
-        
-        #4)Try to get urls from the ena_download_column
-        urls = get_urls_from_ENA_column(metadata, ena_download_column)
-        
-        #5)Check file uniqueness in metadata file
-        check_fastqs_uniqueness(metadata, ena_download_column, fastqs_in_directory, plain_text_bool)
+        print(rich_text_colored('\nSearching Metadata Files:', 'section_header', plain_text_bool))
         
-        #6)Show main info
-        
-        #Section header message
-        print(rich_text_colored('\nMain Information:', 'section_header', plain_text_bool))
-        
-        #Print main information
-        metadata_files_main_information(metadata, urls, fastqs_in_directory, plain_text_bool)
-        
-        #7)Construct treatmentfile template
+        ##Get list of metadata files for each dataset depending on selected search mode
+        if search_mode == 'project':
+            input_files_full = get_path_files_in_project_mode(input_path, files_pattern, plain_text_bool)
+        else:
+            input_files_full = get_path_files_in_directory(input_path, files_pattern)
         
-        #Previous steps
-        ##Get outfile name
-        outfile_name = 'raw_treatment_template_' + metadata_table_path.split('/')[-1]
-        ##Treat output_directory parameter / Get full output file path
-        outputfile_path = treat_output_directory_parameter_outfiles(outfile_name, outputdir_path)
+        ##Show message indicating the number of metadata tables detected
+        print('\n-',rich_text_colored('Total Metadata Files detected:', 'general_text', plain_text_bool), len(input_files_full))
         
+        #2) Load files and do checks
         #Section header message
-        print(rich_text_colored('\nCreating Raw Treatment Template:', 'section_header', plain_text_bool))
-        template = contruct_template(metadata, ena_download_column, fastqs_in_directory, possible_sample_names, r1_files_pattern, r2_files_pattern)
+        print(rich_text_colored('\nLoading Files:', 'section_header', plain_text_bool))
         
-        #Show saved file message
+        #2.1.Try to load Variables Dictionary File as pandas dataframe
+        ##Show loading file message
+        print(rich_text_colored('\nVariables Dictionary file:', 'general_text', plain_text_bool))
+        print(variables_dictionary_path)
+        ##Try to load the filterfile
+        variables_dict_table = pd.read_csv(variables_dictionary_path, sep = '\t', dtype = 'string')
+        
+        #Do initial checks on Variables Dictionary file for columns of interest
+        ##Check headers
+        check_headers_variablesfile = check_headers(VARIABLES_FILE_HEADERS_4_CONCAT, variables_dict_table)
+        frase0_1 = 'Error! Some of the needed headers are not in the Variables Dictionary!\n Check your variables file!\n'
+        frase1_1 = '\nThe headers needed are:'
+        treat_headers_check(VARIABLES_FILE_HEADERS_4_CONCAT, check_headers_variablesfile, variables_dict_table, frase0_1, frase1_1, plain_text_bool)
+        ##Check duplicates in 'variable' column
+        check_duplicates_in_variables_dict_column(variables_dict_table, 'variable', 5)
+        ##Check NAs in 'variable' column
+        frase2 = 'Error! Some of the values of the "variable" column in the Variables Dictionary are NAs!\n Check your variables file!'
+        check_na_in_pandas_dataframe(variables_dict_table['variable'], frase2)
+        ##Check valid 'requiredness' column values
+        check_requiredness_values = check_values(VALID_REQUIREDNESS, variables_dict_table['requiredness'])
+        frase0_3 = 'Error! Some of the values of the "requiredness" column in the Variables Dictionary are not valid!\n Check your variables file!\n'
+        frase1_3 = '\nValid values are:'
+        treat_values_check(VALID_REQUIREDNESS, check_requiredness_values, frase0_3, frase1_3, plain_text_bool)
+        
+        #2.2.Try to load metadata files and do checks
+        
+        #Prepare variables
+        ##Set list with metadata tables paths
+        mt_tables = []
+        ##Get list of required columns
+        required_cols = variables_dict_table[variables_dict_table['requiredness']=='required']['variable']
+        ##Get list of all possible columns
+        universe_cols = list(variables_dict_table['variable'])
+        
+        ##Show loading files message
+        print(rich_text_colored('\nDatasets Metadata files:', 'general_text', plain_text_bool))
+        
+        ##Try to read each metadata table and do checks
+        for file in input_files_full:
+            ##Show metadata file path
+            print(file)
+            ##Load temp file
+            temp_mt = pd.read_csv(file, sep = '\t')
+            ##Check required variables
+            check_required_variables_in_metadata_table(temp_mt, required_cols, plain_text_bool)
+            ##Check that all columns in metadata are in the variables dictionary
+            check_metadata_table_vars_in_dict(temp_mt, universe_cols, plain_text_bool)
+            ##Save in mt_tables results list
+            mt_tables.append(temp_mt)
+        
+        #3) Concatenate metadata tables
+        ##Section header message
+        print(rich_text_colored('\nConcatenating Metadata Tables:', 'section_header', plain_text_bool))
+        
+        ##Concat metadata tables
+        result = pd.concat(mt_tables)
+        
+        ##Show dimentions of final metadata table
+        print('\n-', rich_text_colored('Number of final Rows:', 'general_text', plain_text_bool),result.shape[0])
+        print('-', rich_text_colored('Number of final Columns:', 'general_text', plain_text_bool),result.shape[1])
+        
+        ##Save final file
+        ###Get final file name
+        out_table = treat_output_file_prefix_name(output_name_prefix, 'concatenated_final_metadata.tsv')
+        ###Treat output_directory parameter / Get full output file path
+        outputfile_table = treat_output_directory_parameter_outfiles(out_table, outputdir_path)
+        ###Message
         print(rich_text_colored('\nSaving results in file:', 'general_text', plain_text_bool))
-        print(outputfile_path)
-        #Save template
-        template.to_csv(outputfile_path, header = True, index = False, sep = '\t')
-        
+        print(outputfile_table)
+        ###Save result dataframe
+        result.to_csv(outputfile_table, header = True, index = False, sep = '\t')
+    
     except Exception as ex:
         print(rich_text_colored('\nThe system returned the following exception:\n', 'exception', plain_text_bool), ex)
-           
+    
     finally:
         #Print empty line for aesthetic purposes
-        print('')
-        
+        print('')    
+
 if __name__ == '__main__':
-    main()    
+    main()
```

### Comparing `omdctk-1.0/src/omdctk/merge_metadata.py` & `omdctk-1.1.0/src/omdctk/merge_metadata.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 @program: merge_metadata.py
 @author: Samuel Piquer-Esteban
-@date: 7 Jul 2023 
+@date: 17 Feb 2024 
 
 """
 
 #Set program name
 __program__ = 'merge_metadata.py'
 
 #Imports from MTD_CT common module
@@ -18,184 +18,183 @@
 
 #Import third-party modules
 from argparse import ArgumentParser
 from tabulate import tabulate
 import pandas as pd
 
 #Program functions
-def check_ena_metadata_file_extension(ena_table_path):
-    """
-    This function checks if the provided ena_table_path has the
-    expected file extension for ENA Metadata Table.
-
-    Parameters
-    ----------
-    ena_table_path : str
-        Path for the ENA Metadata Table file.
-
-    Raises
-    ------
-    OMD_CTK_Exception
-        If the file does not have the expected extension raises an exception.
-        This is done to avoid problems in determining the study accession from
-        the ENA Metadata file name.
-
-    Returns
-    -------
-    None.
-
-    """
-    if ena_table_path.endswith('_ENA_metadata.tsv'):
-        pass
-    else:
-        raise OMD_CTK_Exception('Error! Expected file extension for ENA Metadata Table is "_ENA_metadata.tsv"!')
-
-
-def treat_merge_columns(ena_merge_col_check, publication_merge_col_check):
+def treat_merge_columns(main_merge_col_check, extra_merge_col_check):
     """
     This function treats the merge columns checks.
 
     Parameters
     ----------
-    ena_merge_col_check : bool
-        True: if ena_merge_col present in the ena_table.
-        False: if ena_merge_col is not present in the ena_table.
-    publication_merge_col_check : bool
-        True: if publication_merge_col present in the publication_table.
-        False: if publication_merge_col is not present in the publication_table.
+    main_merge_col_check : bool
+        True: if main_merge_col present in the main_table.
+        False: if main_merge_col is not present in the main_table.
+    extra_merge_col_check : bool
+        True: if extra_merge_col present in the extra_table.
+        False: if extra_merge_col is not present in the extra_table.
 
     Raises
     ------
     OMD_CTK_Exception
         If all or any merge columns are not in their respective metadata tables
         raises an exception.
 
     Returns
     -------
     None.
 
     """
-    if ena_merge_col_check == True and publication_merge_col_check == True:
+    if main_merge_col_check == True and extra_merge_col_check == True:
         pass
-    elif (ena_merge_col_check == True) and (publication_merge_col_check == False):
-        raise OMD_CTK_Exception('Error! The provided Publication Merge Column is not in the Publication Metadata Table!\n Check the provided --publication_merge_column parameter!')
-    elif (ena_merge_col_check == False) and (publication_merge_col_check == True):
-        raise OMD_CTK_Exception('Error! The provided ENA Merge Column is not in the ENA Metadata Table!\n Check the provided --ena_merge_column parameter!')
+    elif (main_merge_col_check == True) and (extra_merge_col_check == False):
+        raise OMD_CTK_Exception('Error! The provided Extra Metadata Merge Column is not in the Extra Metadata Table!\n Check the provided --extra_merge_column parameter!')
+    elif (main_merge_col_check == False) and (extra_merge_col_check == True):
+        raise OMD_CTK_Exception('Error! The provided Main Metadata Merge Column is not in the Main Metadata Table!\n Check the provided --main_merge_column parameter!')
     else:
         raise OMD_CTK_Exception('Error! Both of the provided merge columns are not in their respective metadata tables!\n Check merge columns parameters!')
         
 
-def merge_columns_intersection_checks(ena_merge_column_values, publication_merge_column_values, color_treatment):
+def merge_columns_intersection_checks(main_merge_column_values, extra_merge_column_values, color_treatment):
     """
     This function checks intersections between the provided merge column values
     and shows the corresponding messages if needed.
 
     Parameters
     ----------
-    ena_merge_column_values : list
-        List of values of the provided merge column for the ENA Metadata Table.
-    publication_merge_column_values : list
-        List of values of the provided merge column for the Publication Metadata Table.
+    main_merge_column_values : list
+        List of values of the provided merge column for the Main Metadata Table.
+    extra_merge_column_values : list
+        List of values of the provided merge column for the Extra Metadata Table.
     color_treatment: bool
         The color treatment option provided.
         True : Plain Text
         False : Colored Text
 
     Returns
     -------
     bool
         True: There are intersection warnings.
         False: There are no intersection warnings.
 
     """
     #Get unique values
-    ena_merge_column_values_unique = set(ena_merge_column_values)
-    publication_merge_column_values_unique = set(publication_merge_column_values)
+    main_merge_column_values_unique = set(main_merge_column_values)
+    extra_merge_column_values_unique = set(extra_merge_column_values)
     
     #Show stats
     print(rich_text_colored('\nUnique values:', 'subsection2', color_treatment))
-    print('  o', rich_text_colored('ENA Merge Column (total unique values):', 'general_text', color_treatment), len(ena_merge_column_values_unique))
-    print('  o', rich_text_colored('Publication Merge Column (total unique values):', 'general_text', color_treatment), len(publication_merge_column_values_unique))
+    print('  o', rich_text_colored('Main Metadata Merge Column (total unique values):', 'general_text', color_treatment), len(main_merge_column_values_unique))
+    print('  o', rich_text_colored('Extra Metadata Merge Column (total unique values):', 'general_text', color_treatment), len(extra_merge_column_values_unique))
     
     #Check if all unique values between merge columns are common
-    all_ena_in_publication = ena_merge_column_values_unique.issubset(publication_merge_column_values_unique)
-    all_publication_in_ena = publication_merge_column_values_unique.issubset(ena_merge_column_values_unique)
-    if (all_ena_in_publication and all_publication_in_ena):
+    all_main_in_extra = main_merge_column_values_unique.issubset(extra_merge_column_values_unique)
+    all_extra_in_main = extra_merge_column_values_unique.issubset(main_merge_column_values_unique)
+    if (all_main_in_extra and all_extra_in_main):
         print(rich_text_colored('\nAll unique values are common between the merge columns provided!', 'acceptable', color_treatment))
         #Return info for lately treat advise messages
         return False
     else:
         ##Get lits of non-common values
-        ena_difference = list(ena_merge_column_values_unique.difference(publication_merge_column_values_unique))
-        publication_difference = list(publication_merge_column_values_unique.difference(ena_merge_column_values_unique))
+        main_difference = list(main_merge_column_values_unique.difference(extra_merge_column_values_unique))
+        extra_difference = list(extra_merge_column_values_unique.difference(main_merge_column_values_unique))
         
         ##Show intersection stats
         print(rich_text_colored('\nIntersections:', 'subsection2', color_treatment))
-        print('  o', rich_text_colored('Number of unique common values between merge columns:', 'general_text', color_treatment), len(ena_merge_column_values_unique.intersection(publication_merge_column_values_unique)))
-        print('  o', rich_text_colored('Number of unique specific values for ENA Merge Column:', 'general_text', color_treatment), len(ena_difference))
-        print('  o', rich_text_colored('Number of unique specific values for Publication Merge Column:', 'general_text', color_treatment), len(publication_difference))
+        print('  o', rich_text_colored('Number of unique common values between merge columns:', 'general_text', color_treatment), len(main_merge_column_values_unique.intersection(extra_merge_column_values_unique)))
+        print('  o', rich_text_colored('Number of unique specific values for Main Metadata Merge Column:', 'general_text', color_treatment), len(main_difference))
+        print('  o', rich_text_colored('Number of unique specific values for Extra Metadata Merge Column:', 'general_text', color_treatment), len(extra_difference))
         
         ##Show warning message
         print(rich_text_colored('\nWarning! Some values are not common between merge columns!', 'program_warning', color_treatment))
         
         #Show values if there are warnings
-        ##ena_difference
-        if len(ena_difference) > 0:
-            print('\n-', rich_text_colored('Specific values for ENA Merge Column:', 'general_text', color_treatment))
-            print_list_n_byline(ena_difference, 5)
-        ##publication_difference
-        if len(publication_difference) > 0:
-            print('\n-', rich_text_colored('Specific values for Publication Merge Column:', 'general_text', color_treatment))
-            print_list_n_byline(publication_difference, 5)
+        ##main_difference
+        if len(main_difference) > 0:
+            print('\n-', rich_text_colored('Specific values for Main Metadata Merge Column:', 'general_text', color_treatment))
+            print_list_n_byline(main_difference, 5)
+        ##extra_difference
+        if len(extra_difference) > 0:
+            print('\n-', rich_text_colored('Specific values for Extra Metadata Merge Column:', 'general_text', color_treatment))
+            print_list_n_byline(extra_difference, 5)
         
         #Show advise messages
         print(rich_text_colored('\nThis could be due to:','due_to_header', color_treatment))
-        print('- The presence of extra files or samples not used in the publication (values found only in the ENA Merge Column)', rich_text_colored('[Acceptable]', 'acceptable', color_treatment))
-        print('- The absense of files or samples from the publication (values found only in the Publication Merge Column)', rich_text_colored('[Warning]', 'legend_warning', color_treatment))
+        print('- The presence of additional files or unused samples', rich_text_colored('[Acceptable]', 'acceptable', color_treatment))
+        print('- The absense of files or samples', rich_text_colored('[Warning]', 'legend_warning', color_treatment))
         print("- Authors' mishandle or upload errors", rich_text_colored('[Dangerous]', 'dangerous', color_treatment))
         print(rich_text_colored('\nYou should:', 'you_should_header', color_treatment))
         print('- Manually confirm which is your case')
         print('- Check the original publication and supplementary tables to get some context')
-        print('- If necessary, contact the authors of the original publication and/or the ENA Support (https://www.ebi.ac.uk/ena/browser/support)')
+        print('- If necessary, contact the authors of the original publication')
         
         #Return info for lately treat advise messages
         return True
 
 
 #Main Program
 def main():
     #Setting Arguments
     parser = ArgumentParser()
-    ##Parameter ena_metadata_table
+    ##Parameter main_metadata_table
     parser.add_argument(
-            '-e','--ena_metadata_table', 
+            '-m','--main_metadata_table', 
             action = 'store',
             required = True,
-            help= 'ENA Metadata Table [Expected sep=TABS]. Indicate the path to the ENA Metadata Table file.'
+            help= 'Main Metadata Table [Expected sep=TABS]. Indicate the path to the Main Metadata Table file.'
     )
-    ##Parameter publication_metadata_table
+    ##Parameter extra_metadata_table
     parser.add_argument(
-            '-p','--publication_metadata_table', 
+            '-e','--extra_metadata_table', 
             action = 'store',
             required = True,
-            help = 'Publication Metadata Table [Expected sep=TABS]. Indicate the path to the Publication Metadata Table file.'
+            help = 'Extra Metadata Table [Expected sep=TABS]. Indicate the path to the Extra Metadata Table file.'
     )
-    ##Parameter ena_merge_column
+    ##Parameter main_merge_column
     parser.add_argument(
-            '-ec','--ena_merge_column', 
+            '-mc','--main_merge_column', 
             action = 'store',
-            required = True,
-            help = 'ENA Merge Column. ENA Metadata Table column to be used for merging.'
+            required = False,
+            default = None,
+            help = 'Main Metadata Merge Column. Main Metadata Table column to be used for merging. This parameter will be skipped if pandas_merge_mode = cross.'
     )
-    ##Parameter publication_merge_column
+    ##Parameter extra_merge_column
     parser.add_argument(
-            '-pc','--publication_merge_column', 
+            '-ec','--extra_merge_column', 
             action = 'store',
-            required = True,
-            help = 'Publication Merge Column. Publication Metadata Table column to be used for merging.'
+            required = False,
+            default = None,
+            help = 'Extra Metadata Merge Column. Extra Metadata Table column to be used for merging. This parameter will be skipped if pandas_merge_mode = cross.'
+    )
+    ##Parameter pandas_merge_mode
+    parser.add_argument(
+            '-p','--pandas_merge_mode', 
+            action = 'store',
+            choices = ['left','right','outer','inner','cross'],
+            required = False,
+            default = 'left',
+            help = 'Pandas Merge Mode (Optional) [Default:left]. Indicate the pandas merge mode to be used for merging.'
+    )
+    ##Parameter main_merge_suffix
+    parser.add_argument(
+            '-ms','--main_merge_suffix', 
+            action = 'store',
+            required = False,
+            default = '_x',
+            help = 'Main Metadata Pandas Merge Suffix (Optional) [Default:"_x"]. Suffix to add to overlapping column names for the Main Metadata columns.'
+    )
+    ##Parameter extra_merge_suffix
+    parser.add_argument(
+            '-es','--extra_merge_suffix', 
+            action = 'store',
+            required = False,
+            default = '_y',
+            help = 'Extra Metadata Pandas Merge Suffix (Optional) [Default:"_y"]. Suffix to add to overlapping column names for the Extra Metadata columns.'
     )
     ##Parameter output_directory
     parser.add_argument(
             '-o','--output_directory', 
             action = 'store',
             required = False,
             help = 'Output Directory (Optional). Indicate the path to the Output Directory. Output files will be created in the current directory if not indicated.'
@@ -212,20 +211,31 @@
             '-v','--version',
             action = 'version',
             version = 'version {} ({})'.format(VERSION, DATE)
     )
     
     #Process arguments
     args = parser.parse_args()
-    ena_table_path = args.ena_metadata_table
-    publication_table_path = args.publication_metadata_table
-    ena_merge_col = args.ena_merge_column
-    publication_merge_col = args.publication_merge_column
+    main_table_path = args.main_metadata_table
+    extra_table_path = args.extra_metadata_table
+    main_merge_col = args.main_merge_column
+    extra_merge_col = args.extra_merge_column
+    pd_merge_mode = args.pandas_merge_mode
+    main_cols_suffix = args.main_merge_suffix
+    extra_cols_suffix = args.extra_merge_suffix
     outputdir_path = args.output_directory
     plain_text_bool = args.plain_text
+    #Skip main_merge_column and extra_merge_column if pandas_merge_mode = cross (this is only for aesthetic purposes when showing program headers)
+    if pd_merge_mode == 'cross':
+        args.main_merge_column = None
+        args.extra_merge_column = None
+    
+    #Parser error for -mc and -ec if any are none in a merge mode different than 'cross'
+    if pd_merge_mode != 'cross' and (args.main_merge_column is None or args.extra_merge_column is None):
+        parser.error('the following arguments are required: -mc/--main_merge_column, -ec/--extra_merge_column for this particular merge mode')
     
     #Show Program headers
     print('')
     program_header('#',  __program__, 64, 2, plain_text_bool)
     print('')
     
     #Show Program parameters
@@ -235,87 +245,91 @@
     #Try/Except block
     try:
         #0)Initial checks
         
         #Check that provided output directory exist
         check_existence_directory_parameter(outputdir_path, 'Output', '--output_directory')
         
-        #Check ENA Metadata file extension
-        check_ena_metadata_file_extension(ena_table_path)
-        
         #1)Try to load files
         
         #Section header message
         print(rich_text_colored('\nLoading Files:\n', 'section_header', plain_text_bool))
         
-        #Try to load ENA Metadata Table as pandas dataframe
+        #Try to load Main Metadata Table as pandas dataframe
         ##Show loading file message
-        print(rich_text_colored('ENA Metadata Table file:', 'general_text', plain_text_bool))
-        print(ena_table_path)
+        print(rich_text_colored('Main Metadata Table file:', 'general_text', plain_text_bool))
+        print(main_table_path)
         ##Try to load the ena table file
-        ena_table = pd.read_csv(ena_table_path, sep = '\t')
+        main_table = pd.read_csv(main_table_path, sep = '\t')
         
-        #Try to load Publication Metadata Table as pandas dataframe
+        #Try to load Extra Metadata Table as pandas dataframe
         ##Show loading file message
-        print(rich_text_colored('\nPublication Metadata Table file:', 'general_text', plain_text_bool))
-        print(publication_table_path)
+        print(rich_text_colored('\nExtra Metadata Table file:', 'general_text', plain_text_bool))
+        print(extra_table_path)
         ##Try to load the publication table file
-        publication_table = pd.read_csv(publication_table_path, sep = '\t')
+        extra_table = pd.read_csv(extra_table_path, sep = '\t')
         
-        #2)Check provided merge columns
-        ena_merge_col_check = check_headers(ena_merge_col, ena_table)
-        publication_merge_col_check = check_headers(publication_merge_col, publication_table)
-        treat_merge_columns(ena_merge_col_check, publication_merge_col_check)
+        #2)Check provided merge columns if pd_merge_mode is not cross
+        if pd_merge_mode != 'cross':
+                main_merge_col_check = check_headers(main_merge_col, main_table)
+                extra_merge_col_check = check_headers(extra_merge_col, extra_table)
+                treat_merge_columns(main_merge_col_check, extra_merge_col_check)
         
         #3)Try to merge both tables
         
         #Section header messages
         print(rich_text_colored('\nCreating Merged Metadata Table:', 'section_header', plain_text_bool))
         print(rich_text_colored('\nCombining tables:', 'general_text', plain_text_bool))
-        print('Left Join using ENA Metadata Table as Reference')
+        print(rich_text_colored('Pandas Merge Mode:', 'merge_mode_color', plain_text_bool), pd_merge_mode)
+        print('  o',rich_text_colored('Left Table (x):', 'merge_table_color', plain_text_bool), 'Main Metadata Table')
+        print('  o',rich_text_colored('Right Table (y):', 'merge_table_color', plain_text_bool), 'Extra Metadata Table')
         
         #Previous steps
-        ##Get project accession from ena_table_path
-        study_accession = ena_table_path.split('/')[-1].split('_ENA_metadata.tsv')[0]
+        ##Get project accession from main_table_path
+        main_file_name = main_table_path.split('/')[-1]
         ##Get outfile name
-        out_name_merged = study_accession + '_merged_metadata.tsv'
+        out_name_merged = 'merged_' + main_file_name
+        
         ##Treat output_directory parameter / Get full output file path
         outputfile_merged = treat_output_directory_parameter_outfiles(out_name_merged, outputdir_path)
         
-        #Join both tables by run accession (left join)
-        df_merged_table=pd.merge(ena_table, publication_table, left_on = ena_merge_col, right_on = publication_merge_col, how = 'left')
+        #Join both tables
+        if pd_merge_mode == 'cross':
+            df_merged_table = pd.merge(main_table, extra_table, how = pd_merge_mode, suffixes = (main_cols_suffix, extra_cols_suffix))
+        else:
+            df_merged_table = pd.merge(main_table, extra_table, left_on = main_merge_col, right_on = extra_merge_col, how = pd_merge_mode, suffixes = (main_cols_suffix, extra_cols_suffix))
         
         #Show saved file message
         print(rich_text_colored('\nSaving results in file:', 'general_text', plain_text_bool))
         print(outputfile_merged)
         #Save df_merged_table
         df_merged_table.to_csv(outputfile_merged, header = True, index = False, sep = '\t')
         
     except Exception as ex:
         print(rich_text_colored('\nThe system returned the following exception:\n', 'exception', plain_text_bool), ex)
         
     else:
-        #4)Check intersections between merge columns
-        
-        #Section header message
-        print(rich_text_colored('\nMerge Columns Intersection Checks:', 'section_header', plain_text_bool))
-        print(rich_text_colored("\nCheck merge columns' unique values:", 'general_text', plain_text_bool))
-        print(rich_text_colored('ENA Merge Column selected:','column_color', plain_text_bool), ena_merge_col)
-        print(rich_text_colored('Publication Merge Column selected:','column_color', plain_text_bool), publication_merge_col)
-        
-        #Get list of values for merge columns
-        ena_merge_col_values = list(ena_table[ena_merge_col])
-        publication_merge_col_values = list(publication_table[publication_merge_col])
-        
-        #Check intersections
-        merge_cols_intersec_check = merge_columns_intersection_checks(ena_merge_col_values, publication_merge_col_values, plain_text_bool)
-        
-        #Show Legend if warnings were detected
-        if merge_cols_intersec_check == True:
-            show_advise_legend(plain_text_bool)
+        #4)Check intersections between merge columns if pd_merge_mode is not cross
+        if pd_merge_mode != 'cross':
+            #Section header message
+            print(rich_text_colored('\nMerge Columns Intersection Checks:', 'section_header', plain_text_bool))
+            print(rich_text_colored("\nCheck merge columns' unique values:", 'general_text', plain_text_bool))
+            print(rich_text_colored('Main Metadata Merge Column selected:','column_color', plain_text_bool), main_merge_col)
+            print(rich_text_colored('Extra Metadata Merge Column selected:','column_color', plain_text_bool), extra_merge_col)
+        
+            #Get list of values for merge columns
+            main_merge_col_values = list(main_table[main_merge_col])
+            extra_merge_col_values = list(extra_table[extra_merge_col])
+        
+            #Check intersections
+            merge_cols_intersec_check = merge_columns_intersection_checks(main_merge_col_values, extra_merge_col_values, plain_text_bool)
+        
+            #Show Legend if warnings were detected
+            if merge_cols_intersec_check == True:
+                show_advise_legend(plain_text_bool)
         
     finally:
         #Print empty line for aesthetic purposes
         print('')
         
 if __name__ == '__main__':
     main()
```

### Comparing `omdctk-1.0/src/omdctk/omdctk_common.py` & `omdctk-1.1.0/src/omdctk/omdctk_common.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 @program: omdtk_common.py
 @author: Samuel Piquer-Esteban
-@date:  7 Jul 2023 
+@date:  12 Mar 2024 
 
 """
 
 #Import third-party modules
 from termcolor import colored
 import pandas as pd
 import os
 
 #Common constants
 
 ##Package information
-DATE = '7 Jul 2023'
-VERSION = 'v1'
+DATE = '12 Mar 2024'
+VERSION = 'v1.1.0'
 
 ##Package Figlet Ascii (small)
 FIGLET = (" ___  __  __ ___      ___              _   _",
           "/ _ \|  \/  |   \    / __|  _ _ _ __ _| |_(_)___ _ _",
           "|(_)|| |\/| | |) |   |(_| || | '_/ _` |  _| / _ \ ' \ ",
           "\___/|_|  |_|___/    \___\_,_|_| \__,_|\__|_\___/_||_|",
           "              _____         _ _   _ _",
@@ -35,26 +35,34 @@
 ##Treatment Template check lists
 TEMPLATE_FINAL_COLUMNS = ['sample_name', 'fastq_file_name', 'fastq_type', 'treatment']
 
 VALID_FASTQ_TYPES = ['pair1', 'pair2', 'single']
 
 VALID_TREATMENTS = ['merge', 'copy', 'rename']
 
+##Variables Dictionary check lists
+VALID_REQUIREDNESS = ['required', 'optional']
+
+##Generic manifest table file headers
+VALID_MANIFEST_COLUMNS = ['file_name', 'sample_name','file_md5']
+
 ##Colors Dictionary
 COLORS_DIC = {'acceptable':'green', 'legend_warning':'magenta', 'dangerous':'red',
               'section_header':'cyan', 'subsection':'yellow', 'general_text':'yellow',
               'subsection2':'magenta', 'subsection3':'green', 'exception':'red', 
               'column_color':'blue', 'pattern_color':'blue', 'filter_color':'green',
               'program_warning':'red', 'program_warning2':'magenta',
               'due_to_header':'magenta', 'you_should_header':'green',
               'true_color':'green', 'false_color':'red', 'check_color':'cyan',
               'treatment_mode_color':'blue', 'treatment_color':'green',
               'figlet_border_color':'blue', 'figlet_package_color':'yellow', 
               'figlet_version_color':'yellow', 'figlet_program_color':'green', 
-              'exception':'red'}
+              'exception':'red','merge_mode_color':'blue', 'merge_table_color':'green',
+              'dataset_color':'green', 'variable_color':'yellow', 'test_color':'yellow',
+              'dict_column_color':'blue','dict_column_color2':'yellow'}
 
 #Common classes
 class OMD_CTK_Exception(Exception):
     pass
 
 #Common function 
 def rich_text_colored(text_str, dic_category, color_treatment):
@@ -362,15 +370,45 @@
             else:
                 temp_line = ' '.join(['\n-', rich_text_colored(i, 'check_color', color_treatment), 
                                       rich_text_colored('Not Found!', 'false_color', color_treatment)])
             frase.append(temp_line)
         #Raise exception
         raise OMD_CTK_Exception(' '.join(frase))
     
-    
+def check_generic_column_in_metadata(generic_column, metadata_df, parameter):
+    """
+    This function checks the presence of the provided generic_column in a
+    generic metadata table.
+
+    Parameters
+    ----------
+    generic_column : str
+        Generic column in Metadata Table. 
+    metadata_df : pandas dataframe
+        The provided generic metadata dataframe.
+    parameter :str
+        The associated parameter.
+
+    Raises
+    ------
+    OMD_CTK_Exception
+        If provided generic_column is absent raises and exception.
+
+    Returns
+    -------
+    None.
+
+    """
+    check = check_headers(generic_column, metadata_df)
+    if check == False:
+        frase = ''.join(['Error! The provided column is not in the Metadata Table!\n Check your metadata file and --',parameter,' parameter!'])
+        #Raise exception
+        raise OMD_CTK_Exception(frase)
+
+
 def print_list_n_byline(list_to_print, n_elements):
     """
     This function prints elements of the provided list 
     n_elements by line.
 
     Parameters
     ----------
@@ -455,14 +493,37 @@
         False: not all values in the pandas_colum are in the list.
         
     """
     result = pandas_column.isin(list_values).all()
     return result
 
 
+def check_values_inv(pandas_column, list_values):
+    """
+    This function checks if all values in a list are in a pandas_colum.
+
+    Parameters
+    ----------
+    pandas_column : pandas dataframe column
+        The provided pandas dataframe column used as reference.
+    list_values : list
+        The provided list of values to check.
+
+    Returns
+    -------
+    result : bool
+        True: all values in the list are in the pandas_colum.
+        False: not all values in the list are in the pandas_colum.
+        
+    """
+    result = all(elem in list(pandas_column) for elem in list_values)
+    
+    return result
+
+
 def treat_values_check(expected_values, values_check, frase0, frase1, color_treatment):
     """
     This function treats the results for values checks.
 
     Parameters
     ----------
     expected_values : list
@@ -570,16 +631,16 @@
     elif r1_files_pattern == fastq_pattern or r2_files_pattern == fastq_pattern:
         raise OMD_CTK_Exception('Error! The provided Fastq Pattern is identical to some of the PAIRED files patterns!\n Check the provided patterns parameters!')
 
 
 def metadata_files_main_information(metadata_df, urls, fastqs_in_directory, color_treatment):
     """
     This function prints the main information for the metadata and downloaded
-    Fastq files. Intented to be used in check_fastqs_ENA.py and 
-    make_treatment_template_ENA.py.
+    Fastq files. Intented to be used in check_fastqs.py and 
+    make_treatment_template.py.
 
     Parameters
     ----------
     metadata_df : pandas dataframe
         The provided metadata dataframe.
     urls : list
         List with the fastq urls from the Metadata file.
@@ -606,14 +667,53 @@
     print(metadata_df['library_layout'].value_counts(dropna = False).rename_axis('unique_values').reset_index(name = 'counts').to_string(index = False))
     ##Show the number of detected URLS to download
     print(rich_text_colored('\n5) Number of URLs expected to be downloaded:', 'subsection', color_treatment), len(urls))
     ##Show the number of files downloaded ending in 'fastq.gz' for files_directory
     print(rich_text_colored('\n6) Number of Fastq files in the provided Fastqs Directory:', 'subsection', color_treatment), len(fastqs_in_directory))
 
 
+def generic_files_main_information(metadata_df, generic_merge_col, manifest_df, fastqs_in_directory, color_treatment):
+    """
+    This function print the main information for the generic files and downloaded
+    Fastq files. Intented to be used in check_fastqs.py and 
+    make_treatment_template.py.
+
+    Parameters
+    ----------
+    metadata_df : pandas dataframe
+        The provided generic metadata dataframe.
+    generic_merge_col : str
+        Merge column in Generic Metadata Table. Must be compatible with 
+        'sample_name' column from Manifest Table.
+    manifest_df : pandas dataframe
+        The provided manifest dataframe.
+    fastqs_in_directory : list
+        List of fastqs detected in the provided directory.
+    color_treatment: bool
+        The color treatment option provided.
+        True : Plain Text
+        False : Colored Text
+
+    Returns
+    -------
+    None.
+
+    """
+    ##Show the number of rows in generic metadata table
+    print(rich_text_colored('\n1) Number of rows in Metadata Table:', 'subsection', color_treatment), len(metadata_df.index))
+    ##Show the number of unique sample_accessions
+    print(rich_text_colored('\n2) Number of unique samples for provided generic_merge_column in Metadata Table:', 'subsection', color_treatment), metadata_df[generic_merge_col].nunique(dropna = False))
+    ##Show the number of fastq files in manifest
+    print(rich_text_colored('\n3) Number of Fastq files in the provided Manifest Table:', 'subsection', color_treatment), len(manifest_df.index))
+    ##Show the number of unique sample_accessions
+    print(rich_text_colored('\n4) Number of unique samples for "sample_name" column in Manifest Table:', 'subsection', color_treatment), manifest_df['sample_name'].nunique(dropna = False))
+    ##Show the number of files downloaded ending in 'fastq.gz' for files_directory
+    print(rich_text_colored('\n5) Number of Fastq files in the provided Fastqs Directory:', 'subsection', color_treatment), len(fastqs_in_directory))
+
+
 def check_na_in_pandas_dataframe(pandas_column, frase):
     """
     This function checks if a pandas dataframe column contais any NA.
 
     Parameters
     ----------
     pandas_column : pandas dataframe column
@@ -985,8 +1085,230 @@
         frase2 = '\n- ' + rich_text_colored('An equal number of PAIRED and SINGLE Fastq files with more than 1 file per Fastq type', 'acceptable', color_treatment) + rich_text_colored('\n  Configuration: ', 'general_text', color_treatment) + 'Number of pair1(s) > 1; Number of pair2(s) > 1; Number of single(s) > 1;\n                 Number of pair1(s) = Number of pair2(s) = Number of single(s)'
         frase3 = '\n- ' + rich_text_colored('An equal number of PAIRED Fastq files with more than 1 file per Fastq type', 'acceptable', color_treatment) + rich_text_colored('\n  Configuration: ', 'general_text', color_treatment) + 'Number of pair1(s) > 1; Number of pair2(s) > 1; Number of single(s) = 0;\n                 Number of pair1(s) = Number of pair2(s)'
         frase4 = '\n- ' + rich_text_colored('More than one SINGLE Fastq file', 'acceptable', color_treatment) + rich_text_colored('\n  Configuration: ', 'general_text', color_treatment) + 'Number of pair1(s) = 0; Number of pair2(s) = 0; Number of single(s) > 1'
         frase5 = '\n\nThe following samples present incompatibilities:'
         frase = [frase0, frase1, frase2, frase3, frase4, frase5]
         final_frase = frase + check_frases
         #Raise exception
-        raise OMD_CTK_Exception(' '.join(final_frase))
+        raise OMD_CTK_Exception(' '.join(final_frase))
+
+
+def check_required_variables_in_metadata_table(metadata_df, required_cols, color_treatment):
+    """
+    This functions checks if all required variables in dictionary are in the provided metadata table.
+
+    Parameters
+    ----------
+    metadata_df : pandas dataframe
+        Metadata Table to check.
+    required_cols : pandas series(column)
+        Required columns as indicated in Variables Dictionary.
+    color_treatment: bool
+        The color treatment option provided.
+        True : Plain Text
+        False : Colored Text
+    Raises
+    ------
+    Exception
+        If required columns are missing raises an exception.
+        Handled by treat_headers_check function.
+
+    Returns
+    -------
+    None.
+
+    """   
+    #Check that the required col_names are present
+    requireness = required_cols.isin(list(metadata_df.columns)).all()
+    #Get list of required cols
+    required_cols_list = list(required_cols)
+    if requireness == False:
+        ##Check valid 'requiredness' column values
+        frase0 = 'Error! Some of the values of the required columns in the Variables Dictionary are not present in the last Metadata Table!\n Check your Variables Dictionary file and/or Metadata Table file!\n'
+        frase1 = '\nRequired columns in Variables Dictionary are:'
+        ##The exception will be handled by treat_headers_check function
+        treat_headers_check(required_cols_list, requireness, metadata_df, frase0, frase1, color_treatment)
+        
+        
+def check_metadata_table_vars_in_dict(metadata_df, universe_cols, color_treatment):
+    """
+    This functions checks that all metadata columns are present in the variables dictionary.
+    
+    Parameters
+    ----------
+    metadata_df : pandas dataframe
+        Metadata Table to check.
+    universe_cols : list
+        List with all the provided variables in Variables Dictionary.
+    color_treatment: bool
+        The color treatment option provided.
+        True : Plain Text
+        False : Colored Text
+    Raises
+    ------
+    Exception
+        If extra columns are present raises an exception.
+
+    Returns
+    -------
+    None.
+
+    """   
+    #Check that all col_names in metadata table exist in variables_dict
+    all_present = set(list(metadata_df.columns)).issubset(universe_cols)
+    if all_present == False:
+        #Prepare exception frase
+        frase0 = 'Error! Some of the columns in the last Metadata Table are not present in the Variables Dictionary!\n Check your Variables Dictionary file and/or Metadata Table file!\n'
+        frase1 = '\nColumns for this Metadata Table are:'
+        frase = [frase0, frase1]
+        for col in list(metadata_df.columns):
+            if col in universe_cols:
+                temp_line = ' '.join(['\n-', rich_text_colored(col, 'check_color', color_treatment), 
+                                      rich_text_colored('Found!', 'true_color', color_treatment)])
+            else:
+                temp_line = ' '.join(['\n-', rich_text_colored(col, 'check_color', color_treatment), 
+                                      rich_text_colored('Not Found!', 'false_color', color_treatment)])
+            frase.append(temp_line)
+        #Raise exception
+        raise OMD_CTK_Exception(' '.join(frase))
+
+
+def check_duplicates_in_variables_dict_column(variable_dict_df, col_name, n_elements):
+    """
+    This function checks if there are duplicates in the indicated pandas column of the provided variables dictionary dataframe.
+
+    Parameters
+    ----------
+    variable_dict_df : pandas dataframe
+        The provided variables dictionary dataframe.
+    col_name : str
+        Name of the column to check for duplicates.
+    n_elements : int
+        The number of elements to be printed by line.
+
+    Raises
+    ------
+    OMD_CTK_Exception
+        If duplicates are detected raises an exception.
+
+    Returns
+    -------
+    None.
+
+    """
+    #Get duplicates df
+    duplicates_df = variable_dict_df[variable_dict_df.duplicated(subset=[col_name])]
+    
+    #Treat duplicates
+    if len(duplicates_df) > 0:
+        #Get list of duplicates
+        duplicates = list(duplicates_df[col_name])
+        #Construct frase
+        frase0 = ''.join(['Error! Some of the values of the "', col_name,'" column in the Variables Dictionary are duplicates!\n Check your Variables Dictionary file!\n'])
+        frase1 = '\nThe following variables present duplicates:\n'
+        frase = [frase0, frase1]
+        #Split list of duplicates for aesthetics
+        splited_list = [duplicates[i:i+n_elements] for i in range(0, len(duplicates), n_elements)]
+        for i in splited_list:
+            #Format depending on if it is the last line
+            if i == splited_list[-1]:
+                temp_line = ', '.join(i)
+            else:
+                temp_line = ', '.join(i+['\n'])
+            #Append line
+            frase.append(temp_line)
+        #Raise exception
+        raise OMD_CTK_Exception(' '.join(frase))
+
+
+def curly_2_straight_quotation(value):
+    """
+    This function replaces curly for straight quotation
+    in a string.
+
+    Parameters
+    ----------
+    value : str
+        Provided str to replace characters.
+
+    Returns
+    -------
+    str
+        Result str with replaced characters.
+
+    """
+    #curly_2_straight_quotation
+    return value.replace("“", '"').replace("”", '"').replace("‘", "'").replace("’", "'")
+
+
+def generic_columns_intersection_checks(common_col_df1, common_col_df2, df1, df2, df1_name, df2_name, color_treatment):
+    """
+    This function checks intersections between indicated columns of the 
+    provided dataframes and shows the corresponding messages if needed.
+
+    Parameters
+    ----------
+    common_col_df1 : str
+        Common intersect column from dataframe1.
+    common_col_df2 : str
+        Common intersect column from dataframe2.
+    df1 : pandas datframe
+        The provided dataframe1.
+    df2 : pandas datframe
+        The provided dataframe2.
+    df1_name : str
+        The provided pretty dataframe1 name for messages.
+    df2_name : str
+        The provided pretty dataframe2 name for messages. 
+    color_treatment: bool
+        The color treatment option provided.
+        True : Plain Text
+        False : Colored Text
+
+    Returns
+    -------
+    bool
+        True: There are intersection warnings.
+        False: There are no intersection warnings.
+
+    """
+    #Get unique values
+    df1_merge_column_values_unique = set(list(df1[common_col_df1]))
+    df2_merge_column_values_unique = set(list(df2[common_col_df2]))
+    
+    #Show stats
+    print(rich_text_colored('\nUnique values:', 'subsection2', color_treatment))
+    print('  o', rich_text_colored(''.join([df1_name,' Column [',common_col_df1,'] (total unique values):']), 'general_text', color_treatment), len(df1_merge_column_values_unique))
+    print('  o', rich_text_colored(''.join([df2_name,' Column [',common_col_df2,'] (total unique values):']), 'general_text', color_treatment), len(df2_merge_column_values_unique))
+    
+    #Check if all unique values between merge columns are common
+    all_df1_in_df2 = df1_merge_column_values_unique.issubset(df2_merge_column_values_unique)
+    all_df2_in_df1 = df2_merge_column_values_unique.issubset(df1_merge_column_values_unique)
+    if (all_df1_in_df2 and all_df2_in_df1):
+        print(rich_text_colored('\nAll unique values are common between the columns provided!', 'acceptable', color_treatment))
+        #Return info for lately treat advise messages
+        return False
+    else:
+        ##Get lits of non-common values
+        df1_difference = list(df1_merge_column_values_unique.difference(df2_merge_column_values_unique))
+        df2_difference = list(df2_merge_column_values_unique.difference(df1_merge_column_values_unique))
+        
+        ##Show intersection stats
+        print(rich_text_colored('\nIntersections:', 'subsection2', color_treatment))
+        print('  o', rich_text_colored('Number of unique common values between columns:', 'general_text', color_treatment), len(df1_merge_column_values_unique.intersection(df2_merge_column_values_unique)))
+        print('  o', rich_text_colored(''.join(['Number of unique specific values for ',df1_name, ' Column:']), 'general_text', color_treatment), len(df1_difference))
+        print('  o', rich_text_colored(''.join(['Number of unique specific values for ',df2_name, ' Column:']), 'general_text', color_treatment), len(df2_difference))
+        
+        ##Show warning message
+        print(rich_text_colored('\nWarning! Some values are not common between columns!', 'program_warning', color_treatment))
+        
+        #Show values if there are warnings
+        ##main_difference
+        if len(df1_difference) > 0:
+            print('\n-', rich_text_colored(''.join(['Specific values for ',df1_name, ' Column:']), 'general_text', color_treatment))
+            print_list_n_byline(df1_difference, 5)
+        ##extra_difference
+        if len(df2_difference) > 0:
+            print('\n-', rich_text_colored(''.join(['Specific values for ',df2_name, ' Column:']), 'general_text', color_treatment))
+            print_list_n_byline(df2_difference, 5)
+        #Return info for lately treat advise messages
+        return True
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `omdctk-1.0/src/omdctk/test_info/PRJEB10949_check_fastqs_ENA_reference.log` & `omdctk-1.1.0/src/omdctk/test_info/PRJEB10949_check_fastqs_ENA_reference.log`

 * *Files 0% similar despite different names*

```diff
@@ -59,11 +59,11 @@
 3) Check if there are Fastq files of the provided directory with multiple matches in the Metadata Table:
 All Fastq files in the provided directory have a unique run_accession match with the Metadata Table!
 
 4) Check that expected MD5s from the Metadata Table match calculated MD5s:
 
 This may take a while...
   o Total number of Fastqs detected in Metadata Table: 42
-  o Total number of warnings for MD5s : 0
+  o Total number of warnings for MD5s: 0
 
 All MD5s present in the Metadata Table match the MD5s calculated for their corresponding Fastq files!
```

### Comparing `omdctk-1.0/src/omdctk/test_info/PRJEB10949_check_metadata_ENA_reference.log` & `omdctk-1.1.0/src/omdctk/test_info/PRJEB10949_check_metadata_ENA_reference.log`

 * *Files identical despite different names*

### Comparing `omdctk-1.0/src/omdctk/test_info/PRJEB10949_publication_example.tsv` & `omdctk-1.1.0/src/omdctk/test_info/PRJEB10949_publication_example.tsv`

 * *Files identical despite different names*

### Comparing `omdctk-1.0/src/omdctk/test_info/treatment_template_filtered_PRJEB10949_merged_metadata_example.tsv` & `omdctk-1.1.0/src/omdctk/test_info/treatment_template_filtered_PRJEB10949_merged_metadata_example.tsv`

 * *Files identical despite different names*

### Comparing `omdctk-1.0/src/omdctk/treat_fastqs.py` & `omdctk-1.1.0/src/omdctk/make_treatment_template.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,551 +1,352 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
-@program: treat_fastqs.py
+@program: make_treatment_template.py
 @author: Samuel Piquer-Esteban
-@date: 7 Jul 2023 
+@date: 5 Mar 2024 
 
 """
 
 #Set program name
-__program__ = 'treat_fastqs.py'
+__program__ = 'make_treatment_template.py'
 
 #Imports from MTD_CT common module
-from omdctk import (DATE, VERSION, TEMPLATE_FINAL_COLUMNS, VALID_FASTQ_TYPES,
-                    VALID_TREATMENTS, OMD_CTK_Exception, program_header, 
-                    check_existence_directory_parameter, 
-                    check_fastq_PAIRED_patterns, print_list_n_byline,
-                    get_list_fastqs_in_directory, rich_text_colored,
-                    check_headers, treat_headers_check,
-                    check_values, treat_values_check, check_na_in_pandas_dataframe,
-                    check_duplicates_in_fastq_names, treat_check_fastq_name_type,
-                    check_treatment_for_samples, check_rename_samples, check_merge_samples)
+from omdctk import (DATE, VERSION, ENA_FASTQ_URLS_COLUMNS, TEMPLATE_FINAL_COLUMNS, VALID_MANIFEST_COLUMNS, 
+                    OMD_CTK_Exception, program_header, check_existence_directory_parameter, 
+                    check_fastq_PAIRED_patterns, rich_text_colored, check_na_in_pandas_dataframe,
+                    get_list_fastqs_in_directory, print_list_n_byline,
+                    check_headers, treat_headers_check, get_urls_from_ENA_column, 
+                    metadata_files_main_information, treat_output_directory_parameter_outfiles)
 
 #Import third-party modules
 from argparse import ArgumentParser
 from tabulate import tabulate
 import pandas as pd
-import shutil
-import os
+
+#Program Constants
+DEFAULT_SAMPLE_COLUMNS = ['sample_accession', 'secondary_sample_accession',
+                          'run_accession', 'library_name', 'run_alias', 
+                          'sample_alias', 'sample_title']
 
 #Program Functions
-def check_directories_are_not_identical(input_dir, output_dir):
+def check_colname_duplicates(possible_sample_names, color_treatment):
     """
-    This function checks if the provided directories are the same or not.
+    This function checks if the possible columns for sample names provided match
+    the final template column names.
 
     Parameters
     ----------
-    input_dir : str
-        Path to the Input Directory.
-    output_dir : str
-        Path to the Output Directory.
+    possible_sample_names : list
+        List with the possible columns to use as sample name column.
+    color_treatment: bool
+        The color treatment option provided.
+        True : Plain Text
+        False : Colored Text
 
     Raises
     ------
     OMD_CTK_Exception
-        If both directories are the same raises an exception.
+        If the possible columns provided match the final template columns names
+        raises an exception.
 
     Returns
     -------
     None.
 
     """
-    same_dir = os.path.samefile(input_dir, output_dir)
+    #Init results list
+    column_duplicates = []
     
-    if same_dir == True:
-        raise OMD_CTK_Exception('Error! The provided Input and Output directories are the same!')
-
-
-def check_fastq_file_exits(list_fastq_files, fastqs_in_directory, n_elements):
-    """
-    This function checks if all files in the list of fastq files are
-    present in the list of fastq files of the Input Directory.
-
-    Parameters
-    ----------
-    list_fastq_files : list
-        List with the fastq files from the Treatment Template.
-    fastqs_in_directory : list
-        List of fastqs detected in the Input Directory.
-    n_elements : int
-        The number of elements to be printed by line.
-        
-    Raises
-    ------
-    OMD_CTK_Exception
-        If absent Fastq files are detected raises an exception.
-
-    Returns
-    -------
-    None.
+    #Check if the possible sample column names match the TEMPLATE_FINAL_COLUMNS
+    for possible_name in possible_sample_names:
+        if possible_name in TEMPLATE_FINAL_COLUMNS:
+            column_duplicates.append(possible_name)
     
-    """
-    #Get asymmetric difference between list
-    fastqs_difference = list(set(list_fastq_files) - set(fastqs_in_directory))
-        
-    #If difference is not empty raise exception
-    if len(fastqs_difference) > 0:
+    #Raise exception if duplicates are detected
+    if len(column_duplicates) > 0:
         #Prepare exception frase
-        frase0 = 'Error! Some of the Fastq files in the Treatmente Template are not in the Input Directory!\n'
-        frase1 = '\nThe following files were absent:\n'
+        frase0 = 'Error! Some of the sample name columns provided match with the final template columns names!\n'
+        frase1 = '\nPlease, change the following column names in the provided Metadata Table:'
         frase = [frase0, frase1]
-        #Split file names
-        splited_list = [fastqs_difference[i:i+n_elements] for i in range(0, len(fastqs_difference), n_elements)]
-        for i in splited_list:
-            #Format depending on if it is the last line
-            if i == splited_list[-1]:
-                temp_line = ', '.join(i)
-            else:
-                temp_line = ', '.join(i+['\n'])
-            #Append line
+        for i in column_duplicates:
+            temp_line = ' '.join(['\n-', rich_text_colored(i, 'check_color', color_treatment)])
             frase.append(temp_line)
         #Raise exception
         raise OMD_CTK_Exception(' '.join(frase))
-        
-    
-def cat_files(list_inputfiles, outputfile, color_treatment):
-    """
-    This function cats files together in the specified file.
-    It works with both gz compressed and uncompressed Fastq files.
-
-    Parameters
-    ----------
-    list_inputfiles : list
-        The list of paths for the input gzip files to cat.
-    outputfile : str
-        The path for the resulting output gzip file.
-    color_treatment: bool
-        The color treatment option provided.
-        True : Plain Text
-        False : Colored Text
-
-    Returns
-    -------
-    bool
-        True: There are warnings.
-        False: There are no warnings.
-    
-    """
-    try:
-        with open(outputfile,'wb') as output:
-            for file in list_inputfiles:
-                with open(file,'rb') as inputs:
-                    shutil.copyfileobj(inputs, output)
-    except:
-        print(rich_text_colored('Error! These files could not be successfully concatenated!', 'exception', color_treatment))
-        return True
-    else:
-        return False
 
 
-def treat_cat_files(sample_df, fastq_type, input_directory_path, output_directory_path, type_pattern, color_treatment):
+def check_fastqs_uniqueness(dataframe, column, fastqs_in_directory, color_treatment):
     """
-    This function treats the provided sample fastq type files to cat them together.
+    This function checks if the provided Fastqs have a unique match in the 
+    Metadata Table.
 
     Parameters
     ----------
-    sample_df : pandas dataframe
-        The provided sample dataframe.
-    fastq_type : str
-        The fastq type assigned to the fastq file.
-    input_directory_path : str
-        Path to the Input Directory.
-    output_directory_path : str
-        Path to the Output Directory.
-    type_pattern : str
-        The pattern associated to the provided fastq_type.
+    dataframe : pandas dataframe
+        The provided dataframe to use as reference.
+        ENA Mode: ENA Metadata Table
+        Generic Mode: Generic Manifest Table
+    column : str
+        The provided column to search the fastq files in reference dataframe.
+        ENA Mode: ENA metadata column from which the urls were obtained.
+        Generic Mode: "file_name" column in Manifest Table.
+    fastqs_in_directory : list
+        List of fastqs detected in the provided directory.
     color_treatment: bool
         The color treatment option provided.
         True : Plain Text
         False : Colored Text
 
+    Raises
+    ------
+    OMD_CTK_Exception
+        If there are Fastqs that do not have a unique entry in the reference dataframe 
+        raises an exception.
+
     Returns
     -------
-    result : bool
-        True: There are warnings.
-        False: There are no warnings.
+    None.
 
     """
-    #Get sample_name
-    sample_name = list(set(sample_df['sample_name']))[0]   
-    
-    #Get type info
-    sample_df_type = sample_df[sample_df['fastq_type'] == fastq_type]
-    
-    #Get fastq_name and output_path
-    fastq_name = sample_name + type_pattern
-    output_path = os.path.join(output_directory_path, fastq_name)
-    
-    #Get list of input files(and sort by name)
-    input_files = list(sample_df_type['fastq_file_name'])
-    input_files.sort()
-    input_paths = [os.path.join(input_directory_path, file) for file in input_files]
-    
-    #Print cat configuration
-    print(input_files, ' > ', fastq_name)
-    
-    #Cat the gzip files and return bool value
-    result = cat_files(input_paths, output_path, color_treatment)
-    return result
+    #Init results lists
+    fastqs_warnings_more_than_one_match = []
+    fastqs_warnings_zero_matches = []
+    
+    #Iter and process fastq files info
+    for fastq in fastqs_in_directory:
+        #Get temp fastq information dataframe
+        temp_fastq_df = dataframe[dataframe[column].str.contains(fastq)]
+        #Treat info depending on temp_fastq_df len()/ Treat warnings/ Else pass
+        if len(temp_fastq_df) == 1:
+            pass
+        elif len(temp_fastq_df) > 1:
+            fastqs_warnings_more_than_one_match.append(fastq)
+        else:
+            fastqs_warnings_zero_matches.append(fastq)
     
+    #If there are warnings raise exception
+    if len(fastqs_warnings_more_than_one_match) > 0 or len(fastqs_warnings_zero_matches) > 0:
+        if len(fastqs_warnings_more_than_one_match) > 0:
+            print(rich_text_colored('\nWarning! The following Fastq files in the provided directory have more than one match in the Input Reference File!', 'program_warning', color_treatment))
+            print_list_n_byline(fastqs_warnings_more_than_one_match, 5)
+        elif len(fastqs_warnings_zero_matches) > 0:
+            print(rich_text_colored('\nWarning! The following Fastq files in the provided directory do not have a match in the Input Reference File!', 'program_warning', color_treatment))
+            print_list_n_byline(fastqs_warnings_zero_matches, 5)
+        raise OMD_CTK_Exception('Error! Some of the Fastqs in the provided directory do not have a unique match with the Input Reference File (zero or more than one match)!')    
+
 
-def merge_mode(sample_df, input_directory_path, output_directory_path, fastq_pattern, R1_pattern, R2_pattern, color_treatment):
+def get_fastq_type(fastq_name, r1_pattern, r2_pattern):
     """
-    This function merges fastq files from the same sample and prints messages.
+    This function gets the fastq_type from fastq_file_name.
 
     Parameters
     ----------
-    sample_df : pandas dataframe
-        Pandas dataframe with all the information of the sample files.
-    input_directory_path : str
-        The provided Input Directory.
-    output_directory_path : str
-        The provided Output Directory.
-    fastq_pattern : str
-        The Fastq File Pattern provided.
-    R1_pattern : str
-        The R1 File Pattern provided.
-    R2_pattern : str
-        The R2 File Pattern provided.
-    color_treatment: bool
-        The color treatment option provided.
-        True : Plain Text
-        False : Colored Text
+    fastq_name : str
+        Fastq file name in fastqs directory.
+    r1_pattern : str
+        The provided pair1 pattern.
+    r2_pattern : str
+        The provided pair2 pattern.
 
     Returns
     -------
-    result : bool
-        True: There are warnings.
-        False: There are no warnings.
-        
-    """
-    #Init bool results list
-    bools_list = []
-    
-    #List of fastq_types
-    temp_list_fastqtypes = list(sample_df['fastq_type'])
-    
-    #Get temp number of types
-    temp_n_pair1 = temp_list_fastqtypes.count('pair1')
-    temp_n_pair2 = temp_list_fastqtypes.count('pair2')
-    temp_n_single = temp_list_fastqtypes.count('single')   
-       
-    #Treat different configurations
-    ##Paired files with orphan single fastq files with the same number of files
-    if temp_n_pair1 > 1 and temp_n_pair2 > 1 and temp_n_single > 1 and temp_n_pair1 == temp_n_pair2 and temp_n_pair1 == temp_n_single:
-        #Show message paired
-        print(rich_text_colored('Paired Merging:', 'treatment_mode_color', color_treatment))
-        #Generate pair1 file and add bool
-        catp1 = treat_cat_files(sample_df, 'pair1', input_directory_path, output_directory_path, R1_pattern, color_treatment)
-        bools_list.append(catp1)
-        #Generate pair2 file and add bool 
-        catp2 = treat_cat_files(sample_df, 'pair2', input_directory_path, output_directory_path, R2_pattern, color_treatment)
-        bools_list.append(catp2)
-        
-        #Show message single
-        print(rich_text_colored('Single Merging:', 'treatment_mode_color', color_treatment))
-        #Generate pair2 file and add bool 
-        cat_s = treat_cat_files(sample_df, 'single', input_directory_path, output_directory_path, fastq_pattern, color_treatment)
-        bools_list.append(cat_s)
-    #More than one single fastq file but no pair1 or pair2 files
-    elif temp_n_pair1 == 0 and temp_n_pair2 == 0 and temp_n_single>1:
-        #Show message single
-        print(rich_text_colored('Single Merging:', 'treatment_mode_color', color_treatment))
-        #Generate pair2 file and add bool 
-        cat_s = treat_cat_files(sample_df, 'single', input_directory_path, output_directory_path, fastq_pattern, color_treatment)
-        bools_list.append(cat_s)
-    #More than one fastq file for pair1 and pair2 with the same sumber of files, no single files 
-    elif temp_n_single == 0 and temp_n_pair1 > 1 and temp_n_pair2 > 1 and temp_n_pair1 == temp_n_pair2:
-        #Show message paired
-        print(rich_text_colored('Paired Merging:', 'treatment_mode_color', color_treatment))
-        #Generate pair1 file and add bool
-        catp1 = treat_cat_files(sample_df, 'pair1', input_directory_path, output_directory_path, R1_pattern, color_treatment)
-        bools_list.append(catp1)
-        #Generate pair2 file and add bool 
-        catp2 = treat_cat_files(sample_df, 'pair2', input_directory_path, output_directory_path, R2_pattern, color_treatment)
-        bools_list.append(catp2)
-    #Pass because we have ruled out this possibility previusly with check_merge_samples() function
+    result : str
+        Returns the fastq_type [pair1, pair2 or single] 
+        for the provided fastq file name.
+    """   
+    if fastq_name.endswith(r1_pattern):
+        result = 'pair1'
+    elif fastq_name.endswith(r2_pattern):
+        result = 'pair2'
     else:
-        pass
-    #Return bool value / Check if theare are any warnings with this sample
-    return any(bools_list)
-
-        
-def rename_mode(sample_name, fastq_file_name, fastq_type, input_directory_path, output_directory_path, fastq_pattern, R1_pattern, R2_pattern, color_treatment):
-    """
-    This function copies a fastq file with a new name in the provided 
-    Output Directory and prints messages.
-
-    Parameters
-    ----------
-    sample_name : str
-        The sample name of the file that will be used as the new file name.
-    fastq_file_name : str
-        The file name in the provided Input Directory.
-    fastq_type : str
-        The type of fastq file [single, pair1, pair2].
-    input_directory_path : str
-        The provided Input Directory.
-    output_directory_path : str
-        The provided Output Directory.
-    fastq_pattern : str
-        The Fastq File Pattern provided.
-    R1_pattern : str
-        The R1 File Pattern provided.
-    R2_pattern : str
-        The R2 File Pattern provided.
-    color_treatment: bool
-        The color treatment option provided.
-        True : Plain Text
-        False : Colored Text
+        result = 'single'
+    return result
 
-    Returns
-    -------
-    result : bool
-        True: There are warnings.
-        False: There are no warnings.
 
+def contruct_template_from_ENA(metadata_df, column, fastqs_in_directory, possible_sample_names, r1_files_pattern, r2_files_pattern):
     """
-    #Treat single and paired files and get new names
-    if fastq_type == 'pair1':
-        fastq_name = sample_name + R1_pattern
-    elif fastq_type == 'pair2':
-        fastq_name = sample_name + R2_pattern
-    else:
-        fastq_name = sample_name + fastq_pattern
-    
-    #Show message
-    print([fastq_file_name], ' > ', fastq_name)
-    
-    #Set input and output paths
-    output_path = os.path.join(output_directory_path, fastq_name)
-    input_path = os.path.join(input_directory_path, fastq_file_name)
-    
-    #Try to copy file in output directory
-    try:
-        shutil.copyfile(input_path, output_path)    
-    except:
-        print(rich_text_colored('Error! This file could not be successfully renamed in the Output Directory!', 'exception', color_treatment))
-        return True
-    else:
-        return False
-    
-    
-def copy_only_mode(fastq_file_name, input_directory_path, output_directory_path, color_treatment):
-    """
-    This function copies a file in the provided Output Directory.
+    This function constructs the raw template dataframe when using the ENA mode.
 
     Parameters
     ----------
-    fastq_file_name : str
-        The file name in the provided Input Directory.
-    input_directory_path : str
-        The provided Input Directory.
-    output_directory_path : str
-        The provided Output Directory.
-    color_treatment: bool
-        The color treatment option provided.
-        True : Plain Text
-        False : Colored Text
+    metadata_df : pandas dataframe
+        The provided metadata dataframe.
+    column : str
+        The ENA metadata column from which the urls were obtained.
+    fastqs_in_directory : list
+        List of fastqs detected in the provided directory.
+    possible_sample_names : list
+        List with the possible columns to use as sample names.
+    r1_files_pattern : str
+        The provided R1 File Pattern.
+    r2_files_pattern : str
+        The provided R2 File Pattern.
 
     Returns
     -------
-    result : bool
-        True: There are warnings.
-        False: There are no warnings.
-        
+    template : pandas dataframe
+        The resulting template dataframe.
+
     """
-    #Show message
-    print([fastq_file_name],' > ',fastq_file_name)
+    #Init empty pandas dataframe
+    template=pd.DataFrame()
     
-    #Set input and output paths
-    output_path = os.path.join(output_directory_path, fastq_file_name)
-    input_path = os.path.join(input_directory_path, fastq_file_name)
+    #Set template columns
+    template_columns = ['sample_name'] + possible_sample_names + ['fastq_file_name', 'fastq_type', 'treatment']
+    
+    #Iter and process fastq files info
+    for fastq in fastqs_in_directory:
+        #Get temp fastq information dataframe
+        temp_fastq_df = metadata_df[metadata_df[column].str.contains(fastq)]
+        #Extract info
+        temp_row = []
+        ##Add empty sample_name
+        temp_row.append('')
+        ##Add values for each possible_sample_name
+        for i in possible_sample_names:
+            temp_row.append(temp_fastq_df[i].values[0])
+        ##Add fastq_file_name
+        temp_row.append(fastq)
+        ##Add fastq_type using get_fastq_type()
+        temp_row.append(get_fastq_type(fastq, r1_files_pattern, r2_files_pattern))
+        ##Add empty treatment
+        temp_row.append('')
+        #Save info in dataframe
+        temp_template = pd.DataFrame([temp_row], columns = template_columns)
+        template = pd.concat([template, temp_template], ignore_index = True)
     
-    #Try to copy file in output directory
-    try:
-        shutil.copyfile(input_path, output_path)    
-    except:
-        print(rich_text_colored('Error! This file could not be successfully copied in the Output Directory!', 'exception', color_treatment))
-        return True
-    else:
-        return False
+    #Return final template
+    return template
 
 
-def treat_files(treatment_df, unique_samples_list, input_directory_path, output_directory_path, fastq_pattern, R1_pattern, R2_pattern, color_treatment):
+def contruct_generic_template(manifest_df, fastqs_in_directory, r1_files_pattern, r2_files_pattern):
     """
-    This function treats the provided Fastq files based on the Treatment Template.
+    This function constructs the raw template dataframe when using the Generic mode.
 
     Parameters
     ----------
-    treatment_df : pandas dataframe
-        The provided treatment dataframe.
-    unique_samples_list : list
-        List of unique sample_names in Treatment Template.
-    input_directory_path : str
-        The provided Input Directory.
-    output_directory_path : str
-        The provided Output Directory.
-    fastq_pattern : str
-        The Fastq File Pattern provided.
-    R1_pattern : str
-        The R1 File Pattern provided.
-    R2_pattern : str
-        The R2 File Pattern provided.
-    color_treatment: bool
-        The color treatment option provided.
-        True : Plain Text
-        False : Colored Text
+    manifest_df : pandas dataframe
+        The provided manifest dataframe.
+    fastqs_in_directory : list
+        List of fastqs detected in the provided directory.
+    r1_files_pattern : str
+        The provided R1 File Pattern.
+    r2_files_pattern : str
+        The provided R2 File Pattern.
 
     Returns
     -------
-    None.
+    template : pandas dataframe
+        The resulting template dataframe.
 
     """
-    #Init warning samples
-    warning_samples = []
+    #Init empty pandas dataframe
+    template=pd.DataFrame()
     
-    #A)Show main information pre-treatment
-    ##Print information Title
-    print(rich_text_colored('\nPre-treatment Information:\n', 'section_header', color_treatment))
-    ##Show the number of samples
-    print('  o', rich_text_colored('Number of Samples in Treatment Template:', 'subsection', color_treatment), len(unique_samples_list))
-    ##Show the number of files
-    print('  o', rich_text_colored('Number of Fastq files in Treatment Template:', 'subsection', color_treatment), len(treatment_df['fastq_file_name']))   
-    
-    #B)Get files for each sample_name and treat
-    ##Section header
-    print(rich_text_colored('\nTreat Fastqs:', 'section_header', color_treatment))
-    ##Treat FASTQS per sample
-    for sample in unique_samples_list:
-        #Filter table by sample
-        temp_sample = treatment_df[treatment_df['sample_name'] == sample]
-        #Get treatment(get unique with set function)
-        ##NOTE: Up to this point we have check there is only one treatment per sample
-        temp_treatment = list(temp_sample['treatment'])[0]
-        #List of fastq_types
-        temp_list_fastqtypes = list(temp_sample['fastq_type'])
-        #Get temp number of types
-        temp_n_pair1 = temp_list_fastqtypes.count('pair1')
-        temp_n_pair2 = temp_list_fastqtypes.count('pair2')
-        temp_n_single = temp_list_fastqtypes.count('single')
-        
-        #Messages                            
-        ##Show sample ID
-        print(rich_text_colored('\nSample: ', 'treatment_color', color_treatment), sample)
-        ##Show Treatments present
-        print(rich_text_colored('Treatment:', 'treatment_color', color_treatment), temp_treatment)
-        ##Show number of files
-        print(rich_text_colored('Number of Fastq files:', 'general_text', color_treatment), len(temp_sample['fastq_file_name']))
-        ##Show files configuration
-        print(rich_text_colored('Configuration: ', 'general_text', color_treatment) + ''.join(['Number of pair1(s) = ', str(temp_n_pair1), '; Number of pair2(s) = ', str(temp_n_pair2), '; Number of single(s) = ', str(temp_n_single)]))
-        
-        #Treat different
-        if temp_treatment == 'merge':
-            #Merge sample's files
-            sample_result = merge_mode(temp_sample, input_directory_path, output_directory_path, fastq_pattern, R1_pattern, R2_pattern, color_treatment)
-            #If warnings were detected add sample to list
-            if sample_result == True:
-                warning_samples.append(sample)
-        else:
-            if temp_treatment == 'rename':
-                print(rich_text_colored('Renaming file(s):', 'treatment_mode_color', color_treatment))
-            else:
-                print(rich_text_colored('Copying file(s):', 'treatment_mode_color', color_treatment))
-            #Apply treatments by files of sample
-            #Iter files
-            for i,r in temp_sample.iterrows():
-                #Get temp file values
-                temp_file = r['fastq_file_name']
-                temp_file_type = r['fastq_type']
-                #Treat modes
-                if temp_treatment == 'rename':
-                    #Change name for file sample name
-                    file_result = rename_mode(sample, temp_file, temp_file_type, input_directory_path, output_directory_path, fastq_pattern, R1_pattern, R2_pattern, color_treatment)
-                else:
-                    #Copy file sample
-                    file_result = copy_only_mode(temp_file, input_directory_path, output_directory_path, color_treatment)
-                #If warnings were detected for file add sample to list
-                if file_result == True:
-                    warning_samples.append(sample)
-    
-    
-    #C)Show main information pre-treatment
-    ##Previous steps
-    fastqs_in_outputdir = get_list_fastqs_in_directory(output_directory_path, fastq_pattern)
-    
-    ##Print information Title
-    print(rich_text_colored('\nPost-treatment Information:\n', 'section_header', color_treatment))
-    ##Show the number of files
-    print('  o', rich_text_colored('Number of Fastq files in Output Directory:', 'subsection', color_treatment), len(fastqs_in_outputdir))
-    
-    #D)Show saved file message
-    print(rich_text_colored('\nResulting files saved in:', 'general_text', color_treatment))
-    print(output_directory_path)
-    
-    #E)Treat warnings
-    ##Remove duplicates
-    warning_samples = list(set(warning_samples))
-    ##Show message
-    if len(warning_samples) > 0:
-        print(rich_text_colored('Error! Some of the samples in the Treatment Template showed warnings when trying to treat their files!', 'program_warning', color_treatment))
-        print('\nThe following samples present warnings:')
-        print_list_n_byline(warning_samples, 5)
-        
-        
+    #Set template columns
+    template_columns = ['sample_name', 'fastq_file_name', 'fastq_type', 'treatment']
+    
+    #Iter and process fastq files info
+    for fastq in fastqs_in_directory:
+        #Get temp fastq information dataframe
+        temp_fastq_df = manifest_df[manifest_df['file_name'].str.contains(fastq)]
+        #Extract info
+        temp_row = []
+        ##Add sample_name from manifest
+        temp_row.append(temp_fastq_df['sample_name'].values[0])
+        ##Add fastq_file_name
+        temp_row.append(fastq)
+        ##Add fastq_type using get_fastq_type()
+        temp_row.append(get_fastq_type(fastq, r1_files_pattern, r2_files_pattern))
+        ##Add empty treatment
+        temp_row.append('')
+        #Save info in dataframe
+        temp_template = pd.DataFrame([temp_row], columns = template_columns)
+        template = pd.concat([template, temp_template], ignore_index = True)
+    
+    #Return final template
+    return template
+
 #Main Program
 def main():
     #Setting Arguments
     parser = ArgumentParser()
-    ##Parameter treatment_file
+    #Setting Arguments
+    parser = ArgumentParser()
+    ##Parameter input_file
     parser.add_argument(
-            '-t','--treatment_template', 
+            '-i','--input_file', 
             action = 'store',
-            required = True ,
-            help = 'Treatment Template [Expected sep=TABS]. Indicate the path to the Treatment Template file. See Documentation for more information and format details.'
+            required = True,
+            help = 'Input Reference File. Indicate the path to the Input Reference File with the information to create raw treatment template.'
     )
-    ##Parameter input_directory
+    ##Parameter fastqs_directory
     parser.add_argument(
-            '-i','--input_directory', 
+            '-d','--fastqs_directory', 
             action = 'store',
             required = True,
-            help = 'Input Directory. Indicate the path to the Input Directory with the Fastq files to treat.'
+            help = 'Fastqs Directory. Indicate the path to the Fastqs Directory.'
     )
-    ##Parameter output_directory
+    ##Parameter mode
     parser.add_argument(
-            '-o','--output_directory', 
+            '-s','--mode', 
             action = 'store',
-            required = True,
-            help = 'Output Directory. Indicate the path to the Output Directory to save the resulting treated Fastq files.'
+            choices = ['ENA','Generic'],
+            required = False,
+            default = 'ENA',
+            help = 'Execution Mode (Optional) [Default:ENA]. Options: 1) ENA Metadata Table File [Expected sep=TABS] or 2) Generic Manifest Table File [Expected sep=TABS].'
     )
+    ##Parameter ena_download_column
+    parser.add_argument(
+            '-c','--ena_download_column', 
+            action = 'store',
+            choices = ENA_FASTQ_URLS_COLUMNS,
+            required = False,
+            default = 'fastq_ftp',
+            help = 'ENA Download Column (Optional) [Default:fastq_ftp]. Indicate the ENA Metadata Table column that was used to download Fastq files. This parameter will be skipped if Generic mode is used.'
+    ) 
     ##Parameter fastq_pattern
     parser.add_argument(
             '-p','--fastq_pattern', 
             action = 'store',
             default = '.fastq.gz',
             required = False,
             help = 'Fastq File Pattern (Optional) [Default:".fastq.gz"]. Indicate the pattern to identify Fastq files.'
     )
-    ##Parameter r1_patterns
+    ##Parameter r1_pattern
     parser.add_argument(
             '-r1','--r1_pattern', 
             action = 'store',
             default = '_1.fastq.gz',
             required = False,
             help = 'R1 File Pattern (Optional) [Default:"_1.fastq.gz"]. Indicate the pattern to identify R1 PAIRED Fastq files.'
     )
-    ##Parameter r2_patterns
+    ##Parameter r2_pattern
     parser.add_argument(
             '-r2','--r2_pattern', 
             action = 'store',
             default = '_2.fastq.gz',
             required = False,
             help = 'R2 File Pattern (Optional) [Default:"_2.fastq.gz"]. Indicate the pattern to identify R2 PAIRED Fastq files.'
     )
+    ##Parameter extra_sample_columns
+    parser.add_argument(
+            '-e','--extra_sample_columns', 
+            nargs = '+',
+            required = False,
+            help = 'Extra Sample Columns (Optional). Indicate the column names for the extra possible sample names separated by spaces (If a column name has spaces, quote it). This parameter will be skipped if Generic mode is used.'
+    )
+    ##Parameter output_directory
+    parser.add_argument(
+            '-o','--output_directory', 
+            action = 'store',
+            required = False,
+            help = 'Output Directory (Optional). Indicate the path to the Output Directory. Output files will be created in the current directory if not indicated.'
+    )
     ##Parameter plain_text
     parser.add_argument(
             '-x', '--plain_text',
             action = 'store_true',
             required = False,
             help = 'Plain Text Mode (Optional). If indicated, it will enable Plain Text mode, and text will appear without colors.'
     )
@@ -554,124 +355,164 @@
             '-v','--version',
             action = 'version',
             version = 'version {} ({})'.format(VERSION, DATE)
     )
     
     #Process arguments
     args = parser.parse_args()
-    treatment_file_path = args.treatment_template
-    inputdir_path = args.input_directory
+    input_file_path = args.input_file
+    program_mode = args.mode
+    ena_download_column = args.ena_download_column
+    files_directory = args.fastqs_directory
     outputdir_path = args.output_directory
+    extra_sample_names = args.extra_sample_columns
     fastq_pattern = args.fastq_pattern
     r1_files_pattern = args.r1_pattern
     r2_files_pattern = args.r2_pattern
     plain_text_bool = args.plain_text
-    
+    #Skip parameters depending on mode
+    if program_mode == 'Generic':
+        args.ena_download_column = None
+        args.extra_sample_columns = None
+        
     #Show Program headers
     print('')
     program_header('#',  __program__, 64, 2, plain_text_bool)
     print('')
     
     #Show Program parameters
     print(rich_text_colored('Program Parameters:', 'section_header', plain_text_bool))
     print(tabulate(vars(args).items(), headers = ['Argument', 'Value'], tablefmt = 'simple_outline'))
     
     #Try/Except block
     try:
-        #0)Initial checks
+        #0)Initial checks and previous common preparations
         
         #Check that provided files directory exist
-        check_existence_directory_parameter(inputdir_path, 'Input', '--input_directory')
+        check_existence_directory_parameter(files_directory, 'Fastqs', '--fastqs_directory')
         
         #Check that provided output directory exist
         check_existence_directory_parameter(outputdir_path, 'Output', '--output_directory')
         
-        #Check that directories are not the same
-        check_directories_are_not_identical(inputdir_path, outputdir_path)
-        
         #Check PAIRED Fastq patterns
         check_fastq_PAIRED_patterns(fastq_pattern, r1_files_pattern, r2_files_pattern)
         
-        #Try to get list of fastqs in the provided directory
-        fastqs_in_directory = get_list_fastqs_in_directory(inputdir_path, fastq_pattern)
-        
-        #1)Try to load treatment file
-        
-        #Section header message
-        print(rich_text_colored('\nLoading Files:\n', 'section_header', plain_text_bool))
+        #Try to get list of Fastq files in the fastqs directory and sort by name
+        fastqs_in_directory = get_list_fastqs_in_directory(files_directory, fastq_pattern)
+        fastqs_in_directory.sort()
+        
+        #Previous steps for output file(common to both modes)
+        ##Get outfile name
+        outfile_name = 'raw_treatment_template_' + input_file_path.split('/')[-1]
+        ##Treat output_directory parameter / Get full output file path
+        outputfile_path = treat_output_directory_parameter_outfiles(outfile_name, outputdir_path)
+        
+        #1)Initial Section header message(common to both modes)
+        print(rich_text_colored('\nLoading File:\n', 'section_header', plain_text_bool))
+        
+        #Treat differently depending on program mode
+        ##ENA Mode
+        if program_mode == 'ENA':
+            #1)Try to load metadata file
+            
+            #Try to load Metadata Table as pandas dataframe
+            ##Show loading file message
+            print(rich_text_colored('Metadata Table file:', 'general_text', plain_text_bool))
+            print(input_file_path)
+            ##Load metadata file as pandas df
+            metadata = pd.read_csv(input_file_path, sep='\t')
+            
+            #2)Check headers used in metadata table and set possible_sample_names
+            
+            #Define headers used and possible_sample_names
+            ##Set variables
+            possible_sample_names = DEFAULT_SAMPLE_COLUMNS
+            headers_used = DEFAULT_SAMPLE_COLUMNS + ENA_FASTQ_URLS_COLUMNS
+            ##If extra_column parameters are given add to headers to be used if they are not already present
+            if type(extra_sample_names) == list:
+                possible_sample_names = list(set(DEFAULT_SAMPLE_COLUMNS + extra_sample_names))
+                headers_used = list(set(DEFAULT_SAMPLE_COLUMNS + ENA_FASTQ_URLS_COLUMNS + extra_sample_names))
+
+            #Do checks and messages
+            check_headers_metadata = check_headers(headers_used, metadata)
+            frase0_2 = 'Error! Some of the needed headers are not in the Metadata Table!\n Check your metadata file!\n'
+            frase1_2 = '\nThe headers needed are:'
+            treat_headers_check(headers_used, check_headers_metadata, metadata, frase0_2, frase1_2, plain_text_bool)
+            
+            #3)Check that the possible_sample_names do not have a match with the final template column names 
+            check_colname_duplicates(possible_sample_names, plain_text_bool)
+            
+            #4)Try to get urls from the ena_download_column
+            urls = get_urls_from_ENA_column(metadata, ena_download_column)
+            
+            #5)Check file uniqueness in metadata file
+            check_fastqs_uniqueness(metadata, ena_download_column, fastqs_in_directory, plain_text_bool)
+            
+            #6)Show main info
+            #Section header message
+            print(rich_text_colored('\nMain Information:', 'section_header', plain_text_bool))
+            #Print main information
+            metadata_files_main_information(metadata, urls, fastqs_in_directory, plain_text_bool)
+            
+            #7)Construct raw treatmentfile template
+            #Section header message and get template
+            print(rich_text_colored('\nCreating Raw Treatment Template:', 'section_header', plain_text_bool))
+            template = contruct_template_from_ENA(metadata, ena_download_column, fastqs_in_directory, possible_sample_names, r1_files_pattern, r2_files_pattern)
         
-        #Try to load Treatment Template file as pandas dataframe
-        ##Show loading file message
-        print(rich_text_colored('Treatment Template file:', 'general_text', plain_text_bool))
-        print(treatment_file_path)
-        ##Load metadata file as pandas df
-        treatment_table = pd.read_csv(treatment_file_path, sep='\t')
-
-        #2)Checks related to the treatment file
-        
-        ##Check headers in file and messages
-        check_headers_treatmentfile = check_headers(TEMPLATE_FINAL_COLUMNS, treatment_table)
-        frase0_1 = 'Error! Some of the needed headers are not in the Treatment Template!\n Check your treatment file!\n'
-        frase1_1 = '\nThe headers needed are:'
-        treat_headers_check(TEMPLATE_FINAL_COLUMNS, check_headers_treatmentfile, treatment_table, frase0_1, frase1_1, plain_text_bool)
-        
-        ##Check that values in "fastq_type" column from Treatment Template are valid and treatment
-        check_expected_fastq_type_values = check_values(VALID_FASTQ_TYPES, treatment_table['fastq_type'])
-        frase0_2 = 'Error! Some of the values of the "fastq_type" column in the Treatment Template are not valid!\n Check your treatment file!\n'
-        frase1_2 = '\nValid values are:'
-        treat_values_check(VALID_FASTQ_TYPES, check_expected_fastq_type_values, frase0_2, frase1_2, plain_text_bool)
-        
-        ##Check that values in "treatment" column from Treatment Template are valid and treatment
-        check_expected_treatment_values = check_values(VALID_TREATMENTS, treatment_table['treatment'])
-        frase0_3 = 'Error! Some of the values of the "treatment" column in the Treatment Template are not valid!\n Check your treatment file!\n'
-        frase1_3 = '\nValid values are:'
-        treat_values_check(VALID_TREATMENTS, check_expected_treatment_values, frase0_3, frase1_3, plain_text_bool)
-        
-        ##Check that there are no NA values in "sample_name" column from Treatment Template
-        frase4 = 'Error! Some of the values of the "sample_name" column in the Treatment Template are NAs!\n Check your treatment file!'
-        check_na_in_pandas_dataframe(treatment_table['sample_name'], frase4)
-        
-        ##Check that there are no NA values in "fastq_file_name" column from Treatment Template
-        frase5 = 'Error! Some of the values of the "fastq_file_name" column in the Treatment Template are NAs!\n Check your treatment file!'
-        check_na_in_pandas_dataframe(treatment_table['fastq_file_name'], frase5)
-        
-        ##Check that there are not duplicate names in "fastq_file_name" column
-        check_duplicates_in_fastq_names(treatment_table, 5)
-                
-        #3)Checks per file
-        
-        ##Check that all files in Treatment Template have matching file names and fastq types
-        treat_check_fastq_name_type(treatment_table, fastq_pattern, r1_files_pattern, r2_files_pattern, 5)
-        
-        ##Check that all files in Treatment Template are in the Input Directory
-        list_fastq_files = list(treatment_table['fastq_file_name'])
-        check_fastq_file_exits(list_fastq_files, fastqs_in_directory, 5)
-
-        #4)Checks per sample
-        
-        ##Get unique sample names and sort
-        unique_sample_names = list(set(treatment_table['sample_name']))
-        unique_sample_names.sort()
-        
-        ##Check mixed treatments per sample
-        check_treatment_for_samples(treatment_table, unique_sample_names, 5)
-        
-        ##Check rename mode files configurations per sample
-        check_rename_samples(treatment_table, unique_sample_names, plain_text_bool)
-        
-        ##Check merge mode files configurations per sample
-        check_merge_samples(treatment_table, unique_sample_names, plain_text_bool)
-        
-        #5)Treat Fastq files
-
-        ##Treat Fastq files
-        treat_files(treatment_table, unique_sample_names, inputdir_path, outputdir_path, fastq_pattern, r1_files_pattern, r2_files_pattern, plain_text_bool)
+        ##Generic Mode
+        else:
+            #1)Try to load Manifest Table as pandas dataframe
+            ##Show loading file message
+            print(rich_text_colored('Manifest Table file:', 'general_text', plain_text_bool))
+            print(input_file_path)
+            ##Load manifest file as pandas df
+            manifest = pd.read_csv(input_file_path, sep='\t')
+            
+            #2)Check headers used
+            ##Check headers in manifest table
+            check_headers_manifest = check_headers(VALID_MANIFEST_COLUMNS, manifest)
+            frase0_1 = 'Error! Some of the needed headers are not in the Manifest Table!\n Check your manifest file!\n'
+            frase1_1 = '\nThe headers needed are:'
+            treat_headers_check(VALID_MANIFEST_COLUMNS, check_headers_manifest, manifest, frase0_1, frase1_1, plain_text_bool)
+            
+            ##Check NAs in 'file_name' column manifest
+            frase2 = 'Error! Some of the values of the "file_name" column in the Manifest Table are NAs!\n Check your manifest file!'
+            check_na_in_pandas_dataframe(manifest['file_name'], frase2)
+            
+            ##Check NAs in 'file_name' column manifest
+            frase3 = 'Error! Some of the values of the "sample_name" column in the Manifest Table are NAs!\n Check your manifest file!'
+            check_na_in_pandas_dataframe(manifest['sample_name'], frase3)
+            
+            #3)Check uniqueness in  manifest file
+            check_fastqs_uniqueness(manifest, 'file_name', fastqs_in_directory, plain_text_bool)
+            
+            #4)Show main information
+            ##Section header message
+            print(rich_text_colored('\nMain Information:', 'section_header', plain_text_bool))
+            ##Show the number of fastq files in manifest
+            print(rich_text_colored('\n1) Number of Fastq files in the provided Manifest Table:', 'subsection', plain_text_bool), len(manifest.index))
+            ##Show the number of unique sample_accessions
+            print(rich_text_colored('\n2) Number of unique samples for "sample_name" column in Manifest Table:', 'subsection', plain_text_bool), manifest['sample_name'].nunique(dropna = False))
+            ##Show the number of files downloaded ending in 'fastq.gz' for files_directory
+            print(rich_text_colored('\n3) Number of Fastq files in the provided Fastqs Directory:', 'subsection', plain_text_bool), len(fastqs_in_directory))
+
+            #5)Construct raw treatmentfile template
+            #Section header message and get template
+            print(rich_text_colored('\nCreating Raw Treatment Template:', 'section_header', plain_text_bool))
+            template = contruct_generic_template(manifest, fastqs_in_directory, r1_files_pattern, r2_files_pattern)
+        
+        #Final Common part
+        ##Show saved file message and save result(common to both modes)
+        print(rich_text_colored('\nSaving results in file:', 'general_text', plain_text_bool))
+        print(outputfile_path)
+        #Save template
+        template.to_csv(outputfile_path, header = True, index = False, sep = '\t')
         
     except Exception as ex:
         print(rich_text_colored('\nThe system returned the following exception:\n', 'exception', plain_text_bool), ex)
            
     finally:
         #Print empty line for aesthetic purposes
         print('')
-                                                                                                   
+        
 if __name__ == '__main__':
-    main()
+    main()
```

### Comparing `omdctk-1.0/src/omdctk/treat_metadata_ENA.py` & `omdctk-1.1.0/src/omdctk/treat_metadata.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
-@program: treat_metadata_ENA.py
+@program: treat_metadata.py
 @author: Samuel Piquer-Esteban
-@date: 7 Jul 2023 
+@date: 7 Mar 2024 
 
 """
 
 #Set program name
-__program__ = 'treat_metadata_ENA.py'
+__program__ = 'treat_metadata.py'
 
 #Imports from MTD_CT common module
 from omdctk import (DATE, VERSION, ENA_FASTQ_URLS_COLUMNS, TEMPLATE_FINAL_COLUMNS, 
                     VALID_FASTQ_TYPES, VALID_TREATMENTS, OMD_CTK_Exception, 
                     program_header, check_existence_directory_parameter, 
                     check_fastq_PAIRED_patterns, print_list_n_byline, 
                     check_headers, treat_headers_check, rich_text_colored,
                     check_values, treat_values_check, check_na_in_pandas_dataframe,
                     check_duplicates_in_fastq_names, treat_check_fastq_name_type,
                     check_treatment_for_samples, check_rename_samples, check_merge_samples,
-                    treat_output_directory_parameter_outfiles, show_advise_legend)
+                    treat_output_directory_parameter_outfiles, show_advise_legend,
+                    check_generic_column_in_metadata, generic_columns_intersection_checks)
 
 #Import third-party modules
 from argparse import ArgumentParser
 from tabulate import tabulate
 import pandas as pd
 
 #Program Constants
+GENERIC_TREATMENT_COMMON_COLUMN_CHOICES = ['sample_name', 'fastq_file_name']
+
 DEFAULT_ENA_NO_WARNING_COLUMNS = ['sample_accession', 'secondary_sample_accession', 'experiment_accession', 
                                   'run_accession', 'library_name', 'experiment_title', 'experiment_alias', 
                                   'run_alias', 'sample_alias', 'broker_name','sample_title', 'first_public',
                                   'last_updated', 'ENA-FIRST-PUBLIC', 'ENA-LAST-UPDATE', 'first_created']
 
 ENA_COLUMNS_IGNORED = ['nominal_length', 'read_count', 'base_count',  'fastq_bytes', 'fastq_md5', 'fastq_ftp', 
                        'fastq_aspera', 'fastq_galaxy', 'submitted_bytes', 'submitted_md5', 'submitted_ftp', 
@@ -57,15 +60,15 @@
     Parameters
     ----------
     treatment_df : pandas dataframe
         The provided treatment dataframe.
     metadata_df : pandas dataframe
         The provided metadata dataframe.
     column : str
-        The ENA metadata column from which the urls were obtained.
+        The metadata column from which the urls were obtained(ENA Mode) or fastq files are indicated(Generic Mode).
     color_treatment: bool
         The color treatment option provided.
         True : Plain Text
         False : Colored Text
 
     Raises
     ------
@@ -101,14 +104,55 @@
             print_list_n_byline(fastqs_warnings_more_than_one_match, 5)
         elif len(fastqs_warnings_zero_matches) > 0:
             print(rich_text_colored('\nWarning! The following Fastq files from the Treatment Template do not have a match in the Metadata Table!', 'program_warning', color_treatment))
             print_list_n_byline(fastqs_warnings_zero_matches, 5)
         raise OMD_CTK_Exception('Error! Some of the Fastqs in the Treatment Template do not have a unique match with the Metadata Table (zero or more than one match)!')        
 
 
+def check_common_columns_generic_mode(common_col_tt, common_col_mt, treatment_df, metadata_df, treatment_name, metadata_name, color_treatment):
+    """
+    This function checks intersection between the common columns of the provided
+    Metadata and Treatment Template files.
+
+    Parameters
+    ----------
+    common_col_tt : str
+        Generic Common Treatmente Template Column ['sample_name', 'fastq_file_name'].
+    common_col_mt : str
+        Generic Common Metadata Column.
+    treatment_df : pandas dataframe
+        The provided treatment dataframe.
+    metadata_df : pandas dataframe
+        The provided metadata dataframe.
+    treatment_name : str
+        The provided pretty treatment_df name for messages.
+    metadata_name : str
+        The provided pretty metadata_df name for messages.
+    color_treatment: bool
+        The color treatment option provided.
+        True : Plain Text
+        False : Colored Text
+
+    Raises
+    ------
+    OMD_CTK_Exception
+        If mismatches are detected raises an exception.
+
+    Returns
+    -------
+    None.
+
+    """
+    check = generic_columns_intersection_checks(common_col_tt, common_col_mt, treatment_df, metadata_df, treatment_name, metadata_name, color_treatment)
+    if check == True:
+        frase = ''.join(['Error! Some intersect mismatches were found between common columns!\n Check your files and parameters!'])
+        #Raise exception
+        raise OMD_CTK_Exception(frase)
+
+
 def unique_original_sample_names(sample_treatment_df, fastq_pattern, sep, n_sep):
     """
     This function generates a list with the unique original sample names from
     the treatment template based on "fastq_file_name" column.
 
     Parameters
     ----------
@@ -134,14 +178,49 @@
     ##Process fastq names without extension to keep original sample_name
     unique_original_names = list(set(original_fastq_names_without_extension.str.split(sep).apply(lambda x:x[:n_sep]).str.join(sep)))
     unique_original_names.sort()
     
     return unique_original_names
 
 
+def get_possible_files_suffixes(sample_treatment_df, fastq_pattern, sep, n_sep):
+    """
+    This function generates a list with the possible suffixes for the fastq
+    files based on the treatment template "fastq_file_name" column.
+
+    Parameters
+    ----------
+    sample_treatment_df : pandas dataframe
+        The provided filted sample treatment dataframe.
+    fastq_pattern : str
+        Extension pattern to recognize a Fastq file.
+    sep : str
+        Sample Name separator.
+    n_sep : int
+        Sample Name separator appearance.
+
+    Returns
+    -------
+    unique_rest_fastq_pattern : list
+        Unique list of possible file suffixes.
+
+    """
+    #Process fastq_file_name (sample_name + rest + fastq_pattern)
+    ##Remove fastq_pattern
+    original_fastq_names_without_extension = sample_treatment_df['fastq_file_name'].str.replace(fastq_pattern, '', regex = False)
+    
+    ##Process fastq names without extension to keep original sample_name
+    unique_rest = list(set(original_fastq_names_without_extension.str.split(sep).apply(lambda x:x[n_sep:]).str.join(sep)))
+    unique_rest_fastq_pattern = [sep + s + fastq_pattern for s in unique_rest]
+    ##Add also the fastq_pattern as it is(sample_name+fastq_pattern cases for single files i.e. SRR454159.fastq.gz)
+    unique_rest_fastq_pattern.append(fastq_pattern)
+    
+    return unique_rest_fastq_pattern
+
+
 def combine_metadata_rows(final_files_sample_name, filtered_metadata_df, interest_metadata_column, no_warnings_metadata_columns):
     """
     This function combines the metadata (unique values, and treat NAs to '')
     for the provided metadata column. It also treats the associated warnings.
 
     Parameters
     ----------
@@ -192,25 +271,25 @@
         warnings_df = pd.concat([warnings_df, temp_warning], ignore_index = True)
         
     #5.Convert list to formated str and return 
     result = ';'.join(unique_values_list)
     return result
 
 
-def generic_mode_metadata(sample_treatment_df, treatment_saple_name, metadata_df, ena_download_column, interest_metadata_columns, no_warnings_metadata_columns, fastq_pattern, sep, n_sep):
+def other_modes_ENA_metadata(sample_treatment_df, treatment_sample_name, metadata_df, ena_download_column, interest_metadata_columns, no_warnings_metadata_columns, fastq_pattern, sep, n_sep):
     """
     This function creates the necessary combined metadata lines for the provided 
-    sample in generic cases (rename_mode and merge_mode). Lines will be saved 
-    directy in the treated_metadata_df.
+    sample in other treatment modes (rename_mode and merge_mode) when usign 
+    ENA mode. Lines will be saved directy in the treated_metadata_df.
 
     Parameters
     ----------
     sample_treatment_df : pandas dataframe
-        The provided filted sample treatment dataframe.
-    treatment_saple_name : str
+        The provided filtered sample treatment dataframe.
+    treatment_sample_name : str
         Sample Name from the Treatment Template.
     metadata_df : pandas dataframe
         The provided metadata dataframe.
     ena_download_column : str
         Provided ENA Download Column from the Metadata Table.
     interest_metadata_columns : list
         List with the metadata columns of interest to treat.
@@ -234,61 +313,131 @@
     
     #Get list of unique original sample names for treatment template "fastq_file_name"
     original_sample_names = unique_original_sample_names(sample_treatment_df, fastq_pattern, sep, n_sep)
     
     #0. Set result list
     sample_metadata_line = []
     
-    #1. Filter metadata table based in original_sample_names (treatment template) and ena_download_column (metadata)
-    ##NOTE: We re-add the sep, to avoid unspecific matches. For example, sample1 could match with sample1, sample10, sample100, etc.
-    ##NOTE2: We add the fastq_pattern to try que build the fastq name (in some SE cases, there will not be a separator and this is the way that I came up with to take into account this cases)  
-    
-    ##Previous steps
-    #Get original_sample_names + sep
-    original_sample_names_sep = [i + sep for i in original_sample_names]
-    #Get original_sample_names + fastq_pattern
-    original_sample_names_file = [i + fastq_pattern for i in original_sample_names]
-    
+    #1. Filter metadata table based in fastq file names associates to current sample (treatment template) and ena_download_column (metadata)
+    ##Get list of associated fastq files of the sample
+    sample_tt_fastq_file_names = list(sample_treatment_df['fastq_file_name'])
     ##Filter metadata
-    sample_metadata_df = metadata_df[metadata_df[ena_download_column].str.contains('|'.join(original_sample_names_sep + original_sample_names_file))]
+    sample_metadata_df = metadata_df[metadata_df[ena_download_column].str.contains('|'.join(sample_tt_fastq_file_names))]
     
     #2. Get DEFAULT_TREATED_METADATA_COL_NAMES
     ##Get final_files_sample_name / DEFAULT_TREATED_METADATA_COL_NAMES[0]
-    sample_metadata_line.append(treatment_saple_name)
+    sample_metadata_line.append(treatment_sample_name)
     ##Get original_files_sample_names / DEFAULT_TREATED_METADATA_COL_NAMES[1]
     original_files_sample_names = ';'.join(original_sample_names)
     sample_metadata_line.append(original_files_sample_names)
     ##Get treatment_sample_name / DEFAULT_TREATED_METADATA_COL_NAMES[2]
-    sample_metadata_line.append(treatment_saple_name)
-    ##Get unique list for treatment_fastq_type / DEFAULT_TREATED_METADATA_COL_NAMES[2]
+    sample_metadata_line.append(treatment_sample_name)
+    ##Get unique list for treatment_fastq_type / DEFAULT_TREATED_METADATA_COL_NAMES[3]
     unique_fastq_types = list(set(sample_treatment_df['fastq_type']))
     unique_fastq_types.sort()
     sample_metadata_line.append(';'.join(unique_fastq_types))
     
     #3. Combine each metadata column of interest 
     for col in interest_metadata_columns:
-        temp_combined_metadata = combine_metadata_rows(treatment_saple_name, sample_metadata_df, col, no_warnings_metadata_columns)
+        temp_combined_metadata = combine_metadata_rows(treatment_sample_name, sample_metadata_df, col, no_warnings_metadata_columns)
         sample_metadata_line.append(temp_combined_metadata)
     
     #4. Create new line in treated_metadata_df
     new_metadata_line = pd.DataFrame([sample_metadata_line], columns = DEFAULT_TREATED_METADATA_COL_NAMES + interest_metadata_columns)
     treated_metadata_df = pd.concat([treated_metadata_df, new_metadata_line], ignore_index = True)
 
 
-def copy_only_mode_metadata(sample_treatment_df, treatment_saple_name, metadata_df, ena_download_column, interest_metadata_columns, no_warnings_metadata_columns, fastq_pattern, sep, n_sep):
+def other_modes_generic_metadata(sample_treatment_df, treatment_sample_name, metadata_df, mt_common_column, tt_common_column, interest_metadata_columns, no_warnings_metadata_columns, fastq_pattern, sep, n_sep):
     """
     This function creates the necessary combined metadata lines for the provided 
-    sample in the case of the copy_only_mode. Lines will be saved directy in the
-    treated_metadata_df.
+    sample in other treatment modes (rename_mode and merge_mode) when usign 
+    Generic mode. Lines will be saved directy in the treated_metadata_df.
 
     Parameters
     ----------
     sample_treatment_df : pandas dataframe
-        The provided filted sample treatment dataframe.
-    treatment_saple_name : str
+        The provided filtered sample treatment dataframe.
+    treatment_sample_name : str
+        Sample Name from the Treatment Template.
+    metadata_df : pandas dataframe
+        The provided metadata dataframe.
+    mt_common_column : str
+        Generic Common Metadata Column.
+    tt_common_column : str
+        Generic Common Treatment Template Column.
+    interest_metadata_columns : list
+        List with the metadata columns of interest to treat.
+    no_warnings_metadata_columns : list
+        List of metadata column names that is normal/expected to have
+        multiple values. No warning metadata columns.
+    fastq_pattern : str
+        Extension pattern to recognize a Fastq file.
+    sep : str
+        Sample Name separator.
+    n_sep : int
+        Sample Name separator appearance.
+
+    Returns
+    -------
+    None.
+
+    """
+    #Set global variables
+    global treated_metadata_df
+    
+    #Get list of unique original sample names for treatment template "fastq_file_name"
+    original_sample_names = unique_original_sample_names(sample_treatment_df, fastq_pattern, sep, n_sep)
+    
+    #0. Set result list
+    sample_metadata_line = []
+    
+    #1. Filter metadata table depending on the provided tt_common_column
+    if tt_common_column == 'fastq_file_name':
+        #Get temp possible fastq names
+        sample_tt_fastq_file_names = list(sample_treatment_df['fastq_file_name'])
+        ##Filter based on possible fastq file names
+        sample_metadata_df = metadata_df[metadata_df[mt_common_column].str.contains('|'.join(sample_tt_fastq_file_names))]
+    else:
+        ##Filter metadata based on treatment_sample_name
+        sample_metadata_df = metadata_df[metadata_df[mt_common_column]==treatment_sample_name]
+    
+    #2. Get DEFAULT_TREATED_METADATA_COL_NAMES
+    ##Get final_files_sample_name / DEFAULT_TREATED_METADATA_COL_NAMES[0]
+    sample_metadata_line.append(treatment_sample_name)
+    ##Get original_files_sample_names / DEFAULT_TREATED_METADATA_COL_NAMES[1]
+    original_files_sample_names = ';'.join(original_sample_names)
+    sample_metadata_line.append(original_files_sample_names)
+    ##Get treatment_sample_name / DEFAULT_TREATED_METADATA_COL_NAMES[2]
+    sample_metadata_line.append(treatment_sample_name)
+    ##Get unique list for treatment_fastq_type / DEFAULT_TREATED_METADATA_COL_NAMES[3]
+    unique_fastq_types = list(set(sample_treatment_df['fastq_type']))
+    unique_fastq_types.sort()
+    sample_metadata_line.append(';'.join(unique_fastq_types))
+    
+    #3. Combine each metadata column of interest 
+    for col in interest_metadata_columns:
+        temp_combined_metadata = combine_metadata_rows(treatment_sample_name, sample_metadata_df, col, no_warnings_metadata_columns)
+        sample_metadata_line.append(temp_combined_metadata)
+    
+    #4. Create new line in treated_metadata_df
+    new_metadata_line = pd.DataFrame([sample_metadata_line], columns = DEFAULT_TREATED_METADATA_COL_NAMES + interest_metadata_columns)
+    treated_metadata_df = pd.concat([treated_metadata_df, new_metadata_line], ignore_index = True)
+
+
+def copy_only_mode_ENA_metadata(sample_treatment_df, treatment_sample_name, metadata_df, ena_download_column, interest_metadata_columns, no_warnings_metadata_columns, fastq_pattern, sep, n_sep):
+    """
+    This function creates the necessary combined metadata lines for the provided 
+    sample in the case of the copy_only_mode when usign ENA mode. Lines will be 
+    saved directy in the treated_metadata_df.
+
+    Parameters
+    ----------
+    sample_treatment_df : pandas dataframe
+        The provided filereted sample treatment dataframe.
+    treatment_sample_name : str
         Sample Name from the Treatment Template.
     metadata_df : pandas dataframe
         The provided metadata dataframe.
     ena_download_column : str
         Provided ENA Download Column from the Metadata Table.
     interest_metadata_columns : list
         List with the metadata columns of interest to treat.
@@ -309,57 +458,136 @@
     """
     #Set global variables
     global treated_metadata_df
     
     #Get list of unique original sample names for treatment template "fastq_file_name"
     original_sample_names = unique_original_sample_names(sample_treatment_df, fastq_pattern, sep, n_sep)
     
+    #Get list with possible fastq file suffixes
+    possible_fastq_file_suffixes = get_possible_files_suffixes(sample_treatment_df, fastq_pattern, sep, n_sep)
+    
     #Treat diferent original sample names
     for sample in original_sample_names:
         #0. Set result list
         temp_sample_metadata_line = []
         
-        #1. Filter metadata table based in original_sample_name (treatment template) and ena_download_column (metadata)
-        ##NOTE: We re-add the sep, to avoid unspecific matches. For example, sample1 could match with sample1, sample10, sample100, etc.
-        ##NOTE2: We add the fastq_pattern to try que build the fastq name (in some SE cases, there will not be a separator and this is the way that I came up with to take into account this cases)  
-        
-        ##Previous steps
-        #Get sample + sep
-        sample_plus_sep = sample + sep 
-        #Get sample + fastq_pattern
-        sample_plus_extension = sample + fastq_pattern 
+        #Get temp possible fastq names
+        temp_possible_fastq_names = [sample + s for s in possible_fastq_file_suffixes]
+        
+        #1. Filter metadata table based in possible fastq file names for original sample name (treatment template) and ena_download_column (metadata)
         
         ##Filter metadata table
-        temp_sample_metadata_df = metadata_df[metadata_df[ena_download_column].str.contains('|'.join([sample_plus_sep, sample_plus_extension]))]
+        temp_sample_metadata_df = metadata_df[metadata_df[ena_download_column].str.contains('|'.join(temp_possible_fastq_names))]
         
         #2. Get DEFAULT_TREATED_METADATA_COL_NAMES
         ##Get final_files_sample_name / DEFAULT_TREATED_METADATA_COL_NAMES[0]
         temp_sample_metadata_line.append(sample)
         ##Get original_files_sample_names / DEFAULT_TREATED_METADATA_COL_NAMES[1]
         temp_sample_metadata_line.append(sample)
         ##Get treatment_sample_name / DEFAULT_TREATED_METADATA_COL_NAMES[2]
-        temp_sample_metadata_line.append(treatment_saple_name)
-        ##Get unique list for treatment_fastq_type / DEFAULT_TREATED_METADATA_COL_NAMES[2]
+        temp_sample_metadata_line.append(treatment_sample_name)
+        ##Get unique list for treatment_fastq_type / DEFAULT_TREATED_METADATA_COL_NAMES[3]
         unique_fastq_types = list(set(sample_treatment_df['fastq_type']))
         unique_fastq_types.sort()
         temp_sample_metadata_line.append(';'.join(unique_fastq_types))
         
         #3. Combine each metadata column of interest 
         for col in interest_metadata_columns:
             temp_combined_metadata = combine_metadata_rows(sample, temp_sample_metadata_df, col, no_warnings_metadata_columns)
             temp_sample_metadata_line.append(temp_combined_metadata)
         
         #4. Create new line in treated_metadata_df
         temp_metadata_line = pd.DataFrame([temp_sample_metadata_line], columns = DEFAULT_TREATED_METADATA_COL_NAMES + interest_metadata_columns)
         treated_metadata_df = pd.concat([treated_metadata_df, temp_metadata_line], ignore_index = True)
 
 
-def treat_metadata(treatment_df, unique_samples_list, metadata_df, ena_download_column, interest_metadata_columns, no_warnings_metadata_columns, fastq_pattern, sep, n_sep, output_directory_path, color_treatment):
+def copy_only_mode_generic_metadata(sample_treatment_df, treatment_sample_name, metadata_df, mt_common_column, tt_common_column, interest_metadata_columns, no_warnings_metadata_columns, fastq_pattern, sep, n_sep):
     """
-    This function treats the provided Metadata Table based on the Treatment Template.
+    This function creates the necessary combined metadata lines for the provided 
+    sample in the case of the copy_only_mode when usign Generic mode. Lines will 
+    be saved directy in the treated_metadata_df.
+
+    Parameters
+    ----------
+    sample_treatment_df : pandas dataframe
+        The provided filereted sample treatment dataframe.
+    treatment_sample_name : str
+        Sample Name from the Treatment Template.
+    metadata_df : pandas dataframe
+        The provided metadata dataframe.
+    mt_common_column : str
+        Generic Common Metadata Column.
+    tt_common_column : str
+        Generic Common Treatment Template Column.
+    interest_metadata_columns : list
+        List with the metadata columns of interest to treat.
+    no_warnings_metadata_columns : list
+        List of metadata column names that is normal/expected to have
+        multiple values. No warning metadata columns.
+    fastq_pattern : str
+        Extension pattern to recognize a Fastq file.
+    sep : str
+        Sample Name separator.
+    n_sep : int
+        Sample Name separator appearance.
+
+    Returns
+    -------
+    None.
+
+    """
+    #Set global variables
+    global treated_metadata_df
+    
+    #Get list of unique original sample names for treatment template "fastq_file_name"
+    original_sample_names = unique_original_sample_names(sample_treatment_df, fastq_pattern, sep, n_sep)
+    
+    #Get list with possible fastq file suffixes
+    possible_fastq_file_suffixes = get_possible_files_suffixes(sample_treatment_df, fastq_pattern, sep, n_sep)
+    
+    #Treat diferent original sample names
+    for sample in original_sample_names:
+        #0. Set result list
+        temp_sample_metadata_line = []
+        
+        #1. Filter metadata table depending on the provided tt_common_column
+        if tt_common_column == 'fastq_file_name':
+            #Get temp possible fastq names
+            temp_possible_fastq_names = [sample + s for s in possible_fastq_file_suffixes]
+            ##Filter based on possible fastq file names
+            temp_sample_metadata_df = metadata_df[metadata_df[mt_common_column].str.contains('|'.join(temp_possible_fastq_names))]
+        else:
+            ##Filter metadata based on treatment_sample_name
+            temp_sample_metadata_df = metadata_df[metadata_df[mt_common_column]==treatment_sample_name]
+        
+        #2. Get DEFAULT_TREATED_METADATA_COL_NAMES
+        ##Get final_files_sample_name / DEFAULT_TREATED_METADATA_COL_NAMES[0]
+        temp_sample_metadata_line.append(sample)
+        ##Get original_files_sample_names / DEFAULT_TREATED_METADATA_COL_NAMES[1]
+        temp_sample_metadata_line.append(sample)
+        ##Get treatment_sample_name / DEFAULT_TREATED_METADATA_COL_NAMES[2]
+        temp_sample_metadata_line.append(treatment_sample_name)
+        ##Get unique list for treatment_fastq_type / DEFAULT_TREATED_METADATA_COL_NAMES[3]
+        unique_fastq_types = list(set(sample_treatment_df['fastq_type']))
+        unique_fastq_types.sort()
+        temp_sample_metadata_line.append(';'.join(unique_fastq_types))
+        
+        #3. Combine each metadata column of interest 
+        for col in interest_metadata_columns:
+            temp_combined_metadata = combine_metadata_rows(sample, temp_sample_metadata_df, col, no_warnings_metadata_columns)
+            temp_sample_metadata_line.append(temp_combined_metadata)
+        
+        #4. Create new line in treated_metadata_df
+        temp_metadata_line = pd.DataFrame([temp_sample_metadata_line], columns = DEFAULT_TREATED_METADATA_COL_NAMES + interest_metadata_columns)
+        treated_metadata_df = pd.concat([treated_metadata_df, temp_metadata_line], ignore_index = True)
+
+
+def treat_ENA_metadata(treatment_df, unique_samples_list, metadata_df, ena_download_column, interest_metadata_columns, no_warnings_metadata_columns, fastq_pattern, sep, n_sep):
+    """
+    This function treats the provided ENA Metadata Table in ENA Mode based on the Treatment Template.
 
     Parameters
     ----------
     treatment_df : pandas dataframe
         The provided treatment dataframe.
     unique_samples_list : list
         List of unique sample_names in Treatment Template.
@@ -374,63 +602,94 @@
         multiple values. No warning metadata columns.
     fastq_pattern : str
         Extension pattern to recognize a Fastq file.
     sep : str
         Sample Name separator.
     n_sep : int
         Sample Name separator appearance.
-    output_directory_path : str
-        The provided Output Directory.
-    color_treatment: bool
-        The color treatment option provided.
-        True : Plain Text
-        False : Colored Text
 
     Returns
     -------
     None.
 
     """
     #Set global variables
     global treated_metadata_df
     global warnings_df
     
-    #A)Show main information pre-treatment
-    ##Print information Title
-    print(rich_text_colored('\nPre-treatment Information:\n', 'section_header', color_treatment))
-    ##Show the number of samples
-    print('  o', rich_text_colored('Number of Samples in Treatment Template:', 'subsection', color_treatment), len(unique_samples_list))
-    ##Show the number of files
-    print('  o', rich_text_colored('Number of Lines in the Original Metadata Table:', 'subsection', color_treatment), len(metadata_df))
-    
-    #B)Get METADATA for each sample_name and treat
-    ##Section header
-    print(rich_text_colored('\nTreat Metadata:', 'section_header', color_treatment))
-    print('\nTreating metadata ...')
     ##Treat metadata per sample
     for sample in unique_samples_list:
         #Filter table by sample
         temp_sample = treatment_df[treatment_df['sample_name'] == sample]
+        
         #Get treatment(get unique with set function)
         ##NOTE: Up to this point we have check there is only one treatment per sample
         temp_treatment = list(temp_sample['treatment'])[0]
         
         #Treat metadata depending on mode used for treating fastqs
         if temp_treatment == 'copy':
-            copy_only_mode_metadata(temp_sample, sample, metadata_df, ena_download_column, interest_metadata_columns, no_warnings_metadata_columns, fastq_pattern, sep, n_sep)
+            copy_only_mode_ENA_metadata(temp_sample, sample, metadata_df, ena_download_column, interest_metadata_columns, no_warnings_metadata_columns, fastq_pattern, sep, n_sep)
         else:
-            generic_mode_metadata(temp_sample, sample, metadata_df, ena_download_column, interest_metadata_columns, no_warnings_metadata_columns, fastq_pattern, sep, n_sep)
+            other_modes_ENA_metadata(temp_sample, sample, metadata_df, ena_download_column, interest_metadata_columns, no_warnings_metadata_columns, fastq_pattern, sep, n_sep)
     
-    #C)Show main information post-treatment
-    ##Print information Title
-    print(rich_text_colored('\nPost-treatment Information:\n', 'section_header', color_treatment))
-    ##Show the number of files
-    print('  o', rich_text_colored('Number of Lines in the Treated Metadata Table:', 'subsection', color_treatment), len(treated_metadata_df))
 
+def treat_generic_metadata(treatment_df, unique_samples_list, metadata_df, mt_common_column, tt_common_column, interest_metadata_columns, no_warnings_metadata_columns, fastq_pattern, sep, n_sep):
+    """
+    This function treats the provided Generic Metadata Table in Generic Mode based on the Treatment Template
+    and the provided tt_common_column.
+
+    Parameters
+    ----------
+    treatment_df : pandas dataframe
+        The provided treatment dataframe.
+    unique_samples_list : list
+        List of unique sample_names in Treatment Template.
+    metadata_df : pandas dataframe
+        The provided metadata dataframe.
+    mt_common_column : str
+        Generic Common Metadata Column.
+    tt_common_column : str
+        Generic Common Treatment Template Column.
+    interest_metadata_columns : list
+        List with the metadata columns of interest to treat.
+    no_warnings_metadata_columns : list
+        List of metadata column names that is normal/expected to have
+        multiple values. No warning metadata columns.
+    fastq_pattern : str
+        Extension pattern to recognize a Fastq file.
+    sep : str
+        Sample Name separator.
+    n_sep : int
+        Sample Name separator appearance.
+
+    Returns
+    -------
+    None.
+
+    """
+    #Set global variables
+    global treated_metadata_df
+    global warnings_df
+    
+    ##Treat metadata per sample
+    for sample in unique_samples_list:
+        #Filter table by sample
+        temp_sample = treatment_df[treatment_df['sample_name'] == sample]
+        
+        #Get treatment(get unique with set function)
+        ##NOTE: Up to this point we have check there is only one treatment per sample
+        temp_treatment = list(temp_sample['treatment'])[0]
+        
+        #Treat metadata depending on mode used for treating fastqs
+        if temp_treatment == 'copy':
+            copy_only_mode_generic_metadata(temp_sample, sample, metadata_df, mt_common_column, tt_common_column, interest_metadata_columns, no_warnings_metadata_columns, fastq_pattern, sep, n_sep)
+        else:
+            other_modes_generic_metadata(temp_sample, sample, metadata_df, mt_common_column, tt_common_column, interest_metadata_columns, no_warnings_metadata_columns, fastq_pattern, sep, n_sep)
 
+    
 #Main Program
 def main():
     #Setting Arguments
     parser = ArgumentParser()
     ##Parameter metadata_table
     parser.add_argument(
             '-m','--metadata_table', 
@@ -441,22 +700,48 @@
     ##Parameter treatment_file
     parser.add_argument(
             '-t','--treatment_template', 
             action = 'store',
             required = True ,
             help = 'Treatment Template [Expected sep=TABS]. Indicate the path to the Treatment Template file. See Documentation for more information and format details.'
     )
+    ##Parameter mode
+    parser.add_argument(
+            '-s','--mode', 
+            action = 'store',
+            choices = ['ENA','Generic'],
+            required = False,
+            default = 'ENA',
+            help = 'Execution Mode (Optional) [Default:ENA]. Options: 1) ENA Metadata Table File [Expected sep=TABS] or 2) Generic Metadata Table File [Expected sep=TABS].'
+    )
     ##Parameter ena_download_column
     parser.add_argument(
             '-c','--ena_download_column', 
             action = 'store',
             choices = ENA_FASTQ_URLS_COLUMNS,
             required = False,
             default = 'fastq_ftp',
-            help = 'ENA Download Column (Optional) [Default:fastq_ftp]. Indicate the ENA Metadata Table column that was used to download Fastq files.'
+            help = 'ENA Download Column (Optional) [Default:fastq_ftp]. Indicate the ENA Metadata Table column that was used to download Fastq files. This parameter will be skipped if Generic mode is used.'
+    )
+    ##Parameter generic_common_column_mt
+    parser.add_argument(
+            '-g_mt','--generic_common_column_mt', 
+            action = 'store',
+            required = False,
+            default = 'sample_id',
+            help = 'Generic Common Metadata Column (Optional) [Default:sample_id]. Indicate the name of the Common Column in Metadata Table to compare Metadata Table and Treatment Template Files. This parameter will be skipped if ENA mode is used.'
+    )
+    ##Parameter generic_common_column_tt
+    parser.add_argument(
+            '-g_tt','--generic_common_column_tt', 
+            action = 'store',
+            choices = GENERIC_TREATMENT_COMMON_COLUMN_CHOICES,
+            required = False,
+            default = 'sample_name',
+            help = 'Generic Common Treatment Template Column (Optional) [Default:sample_name]. Indicate the name of the Common Column in Treatment Template to compare Metadata Table and Treatment Template Files. This parameter will be skipped if ENA mode is used.'
     )
     ##Parameter extra_no_warning_columns
     parser.add_argument(
             '-e','--extra_no_warning_columns', 
             nargs = '+',
             required = False,
             help = 'Extra No Warning Columns (Optional). Indicate the column names of the Metadata Table that can be safely merged without warning. Provide column names separated by spaces (If a column name has spaces, quote it).'
@@ -522,59 +807,74 @@
             action = 'version',
             version = 'version {} ({})'.format(VERSION, DATE)
     )
 
     #Process arguments
     args = parser.parse_args()
     metadata_table_path = args.metadata_table
+    treatment_file_path = args.treatment_template
+    program_mode = args.mode
     ena_download_column = args.ena_download_column
+    generic_common_col_mt = args.generic_common_column_mt
+    generic_common_col_tt = args.generic_common_column_tt
     extra_no_warning_cols = args.extra_no_warning_columns
-    treatment_file_path = args.treatment_template
     outputdir_path = args.output_directory
     sample_name_separator = args.sample_name_sep
     sep_appearance = args.sample_name_sep_appearance
     fastq_pattern = args.fastq_pattern
     r1_files_pattern = args.r1_pattern
     r2_files_pattern = args.r2_pattern
     plain_text_bool = args.plain_text
+    #Skip parameters depending on mode
+    if program_mode == 'ENA':
+        args.generic_common_column_mt = None
+        args.generic_common_column_tt = None
+    else:
+        args.ena_download_column = None
     
     #Show Program headers
     print('')
     program_header('#',  __program__, 64, 2, plain_text_bool)
     print('')
     
     #Show Program parameters
     print(rich_text_colored('Program Parameters:', 'section_header', plain_text_bool))
     print(tabulate(vars(args).items(), headers = ['Argument', 'Value'], tablefmt = 'simple_outline'))
     
     #Try/Except block
     try:
         #0)Initial steps and checks
         
-        #Set global variables
+        #Set global variables(common to both modes)
         global treated_metadata_df
         global warnings_df
+        no_warning_columns = []
         
-        #Define headers used and no_warnings_column
-        ##Set variables
-        headers_used = DEFAULT_ENA_NO_WARNING_COLUMNS + ENA_FASTQ_URLS_COLUMNS
-        no_warning_columns = DEFAULT_ENA_NO_WARNING_COLUMNS
-        ##If extra_no_warning_cols parameters are given add to headers to be used if they are not already present
-        ## And also add to final no_warning_columns list
-        if type(extra_no_warning_cols) == list:
-            headers_used = list(set(DEFAULT_ENA_NO_WARNING_COLUMNS + ENA_FASTQ_URLS_COLUMNS + extra_no_warning_cols))
-            no_warning_columns = list(set(DEFAULT_ENA_NO_WARNING_COLUMNS + extra_no_warning_cols))
+        #Define headers used and no_warnings_column depending on mode
+        if program_mode == 'ENA':
+            ##Set variables
+            headers_used = DEFAULT_ENA_NO_WARNING_COLUMNS + ENA_FASTQ_URLS_COLUMNS
+            no_warning_columns = DEFAULT_ENA_NO_WARNING_COLUMNS
+            ##If extra_no_warning_cols parameters are given add to headers to be used if they are not already present
+            ## And also add to final no_warning_columns list
+            if type(extra_no_warning_cols) == list:
+                headers_used = list(set(DEFAULT_ENA_NO_WARNING_COLUMNS + ENA_FASTQ_URLS_COLUMNS + extra_no_warning_cols))
+                no_warning_columns = list(set(DEFAULT_ENA_NO_WARNING_COLUMNS + extra_no_warning_cols))
+        else:
+            if type(extra_no_warning_cols) == list:
+                no_warning_columns = extra_no_warning_cols
         
-        #Check that provided output directory exist
+        #Global Check (common to both modes)
+        ##Check that provided output directory exist
         check_existence_directory_parameter(outputdir_path, 'Output', '--output_directory')
         
-        #Check PAIRED Fastq patterns
+        ##Check PAIRED Fastq patterns
         check_fastq_PAIRED_patterns(fastq_pattern, r1_files_pattern, r2_files_pattern)
         
-        #1)Try to load treatment and metadata files
+        #1)Try to load treatment and metadata files (common to both modes)
         
         #Section header message
         print(rich_text_colored('\nLoading Files:\n', 'section_header', plain_text_bool))
         
         #Try to load Treatment Template file as pandas dataframe
         ##Show loading file message
         print(rich_text_colored('Treatment Template file:', 'general_text', plain_text_bool))
@@ -585,23 +885,26 @@
         #Try to load Metadata Table as pandas dataframe
         ##Show loading file message
         print(rich_text_colored('\nMetadata Table file:', 'general_text', plain_text_bool))
         print(metadata_table_path)
         ##Load metadata file as pandas df
         metadata = pd.read_csv(metadata_table_path, sep='\t')
         
-        #2)Checks related to the metadata file
-
-        #Do checks and messages
-        check_headers_metadata = check_headers(headers_used, metadata)
-        frase0_2 = 'Error! Some of the needed headers are not in the Metadata Table!\n Check your metadata file!\n'
-        frase1_2 = '\nThe headers needed are:'
-        treat_headers_check(headers_used, check_headers_metadata, metadata, frase0_2, frase1_2, plain_text_bool)
+        #2)Checks related to the metadata file depending on mode
+        if program_mode == 'ENA':
+            #Do checks and messages
+            check_headers_metadata = check_headers(headers_used, metadata)
+            frase0_2 = 'Error! Some of the needed headers are not in the Metadata Table!\n Check your metadata file!\n'
+            frase1_2 = '\nThe headers needed are:'
+            treat_headers_check(headers_used, check_headers_metadata, metadata, frase0_2, frase1_2, plain_text_bool)
+        else:
+            ##Check generic_common_col_mt in metadata table
+            check_generic_column_in_metadata(generic_common_col_mt, metadata, 'generic_common_column_mt')
         
-        #3)Checks related to the treatment file
+        #3)Checks related to the treatment file(common to both modes)
         
         ##Check headers in file and messages
         check_headers_treatmentfile = check_headers(TEMPLATE_FINAL_COLUMNS, treatment_table)
         frase0_1 = 'Error! Some of the needed headers are not in the Treatment Template!\n Check your treatment file!\n'
         frase1_1 = '\nThe headers needed are:'
         treat_headers_check(TEMPLATE_FINAL_COLUMNS, check_headers_treatmentfile, treatment_table, frase0_1, frase1_1, plain_text_bool)
         
@@ -624,84 +927,115 @@
         ##Check that there are no NA values in "fastq_file_name" column from Treatment Template
         frase5 = 'Error! Some of the values of the "fastq_file_name" column in the Treatment Template are NAs!\n Check your treatment file!'
         check_na_in_pandas_dataframe(treatment_table['fastq_file_name'], frase5)
         
         ##Check that there are not duplicate names in "fastq_file_name" column
         check_duplicates_in_fastq_names(treatment_table, 5)
         
-        #4)Checks per file
-        
-        ##Check that all files in Treatment Template have matching file names and fastq types
+        #4)Check that all files in Treatment Template have matching file names and fastq types (common to both modes)
         treat_check_fastq_name_type(treatment_table, fastq_pattern, r1_files_pattern, r2_files_pattern, 5)
         
-        ##Check that all files in Treatment Templante appear in the Metadata Table
-        check_treatment_fastqs_in_metadata(treatment_table, metadata, ena_download_column, plain_text_bool)
-        
-        #5)Checks per sample
+        #5) Check reference between template and metadata depending on mode
+        if program_mode == 'ENA':
+            ##Check that all fastq files in Treatment Templante appear in the Metadata Table
+            check_treatment_fastqs_in_metadata(treatment_table, metadata, ena_download_column, plain_text_bool)
+        else:
+            #Treat reference check between tables depending on the provided generic_common_col_tt
+            if generic_common_col_tt == 'fastq_file_name':
+                ##Check that all fastq files in Treatment Templante appear in the Metadata Table
+                check_treatment_fastqs_in_metadata(treatment_table, metadata, generic_common_col_mt, plain_text_bool)
+            else:
+                ##Check common columns intersection between treatment template and metadata
+                check_common_columns_generic_mode(generic_common_col_tt, generic_common_col_mt, treatment_table, metadata, 'Treatment Template', 'Metadata', plain_text_bool)
+                    
+        #6)Checks per sample (common to both modes)
         
         ##Get unique sample names and sort
         unique_sample_names = list(set(treatment_table['sample_name']))
         unique_sample_names.sort()
         
         ##Check mixed treatments per sample
         check_treatment_for_samples(treatment_table, unique_sample_names, 5)
         
         ##Check rename mode files configurations per sample
         check_rename_samples(treatment_table, unique_sample_names, plain_text_bool)
         
         ##Check merge mode files configurations per sample
         check_merge_samples(treatment_table, unique_sample_names, plain_text_bool)
         
-        #6)Treat metadata
-        
-        ##Get list of colnames of interest in metadata table
-        interest_metadata_columns = [i for i in list(metadata.columns) if i not in ENA_COLUMNS_IGNORED]
+        #7)Treat metadata
         
-        ##Treat metadata
-        treat_metadata(treatment_table, unique_sample_names, metadata, ena_download_column, interest_metadata_columns, no_warning_columns, fastq_pattern, sample_name_separator, sep_appearance, outputdir_path, plain_text_bool)
+        #A)Show main information pre-treatment (common to both modes)
+        ##Print information Title
+        print(rich_text_colored('\nPre-treatment Information:\n', 'section_header', plain_text_bool))
+        ##Show the number of samples
+        print('  o', rich_text_colored('Number of Samples in Treatment Template:', 'subsection', plain_text_bool), len(unique_sample_names))
+        ##Show the number of rows
+        print('  o', rich_text_colored('Number of Rows in the Original Metadata Table:', 'subsection', plain_text_bool), len(metadata))
+        
+        #B)treat metadata depending on mode
+        ##Section header
+        print(rich_text_colored('\nTreat Metadata:', 'section_header', plain_text_bool))
+        print('\nTreating metadata ...')
+        ##Different mode treatments
+        if program_mode == 'ENA':
+            ##Get list of colnames of interest in metadata table
+            interest_metadata_columns = [i for i in list(metadata.columns) if i not in ENA_COLUMNS_IGNORED]
+            ##Treat metadata
+            treat_ENA_metadata(treatment_table, unique_sample_names, metadata, ena_download_column, interest_metadata_columns, no_warning_columns, fastq_pattern, sample_name_separator, sep_appearance)
+        else:
+            ##Get list of colnames of interest in metadata table
+            interest_metadata_columns = list(metadata.columns)
+            ##Treat metadata
+            treat_generic_metadata(treatment_table, unique_sample_names, metadata, generic_common_col_mt, generic_common_col_tt, interest_metadata_columns, no_warning_columns, fastq_pattern, sample_name_separator, sep_appearance)
+        
+        #C)Show main information post-treatment
+        ##Print information Title
+        print(rich_text_colored('\nPost-treatment Information:\n', 'section_header', plain_text_bool))
+        ##Show the number of rows
+        print('  o', rich_text_colored('Number of Rows in the Treated Metadata Table:', 'subsection', plain_text_bool), len(treated_metadata_df))
         
-        ##Save generated treated_metadata_df
+        ##8)Save generated treated_metadata_df (common to both modes)
         
         #Previous steps
         ##Get outfile name
         outfile_name = 'treated_' + metadata_table_path.split('/')[-1]
         ##Treat output_directory parameter / Get full output file path
         outputfile_path = treat_output_directory_parameter_outfiles(outfile_name, outputdir_path)
         
         #Show saved file message
         print(rich_text_colored('\nSaving results in file:', 'general_text', plain_text_bool))
         print(outputfile_path)
         
         #Save template
         treated_metadata_df.to_csv(outputfile_path, header = True, index = False, sep = '\t')
         
-        #7)Treat warnings
+        #9)Treat warnings
         if len(warnings_df) > 0:
             #Previous steps
             ##Get outfile name
             outreport_name = 'warning_report_4_treated_' + metadata_table_path.split('/')[-1]
             ##Treat output_directory parameter / Get full output file path
             outreport_path = treat_output_directory_parameter_outfiles(outreport_name, outputdir_path)
             
             #Show warning message
             print(rich_text_colored('\nSome of the samples showed warnings when trying to treat their metadata!', 'program_warning', plain_text_bool))
             print(rich_text_colored('\nThis could be due to:','due_to_header', plain_text_bool))
-            print('- The presence of different data types in the dataset', rich_text_colored('[Acceptable]', 'acceptable', plain_text_bool))
             print('- The presence of quality controlled Fastqs in the dataset', rich_text_colored('[Acceptable]', 'acceptable', plain_text_bool))
-            print('- The presence of different sequencing technologies', rich_text_colored('[Acceptable]', 'acceptable', plain_text_bool))
             print('- Multiple sequencer output Fastqs (runs/lanes) from the same sample', rich_text_colored('[Warning]', 'legend_warning', plain_text_bool))
             print('- Technical replicates from the same sample', rich_text_colored('[Warning]', 'legend_warning', plain_text_bool))
             print('- PAIRED files uploaded as SINGLE Fastq files', rich_text_colored('[Warning]', 'legend_warning', plain_text_bool))
+            print('- The presence of different sequencing technologies', rich_text_colored('[Dangerous]', 'dangerous', plain_text_bool))
+            print('- The presence of different data types in the dataset', rich_text_colored('[Dangerous]', 'dangerous', plain_text_bool))
             print("- Authors' mishandle, upload errors or others", rich_text_colored('[Dangerous]', 'dangerous', plain_text_bool))
             print(rich_text_colored('\nYou should:', 'you_should_header', plain_text_bool))
             print('- Use the following warning report to manually confirm which is your case')
             print('- Check if in your particular case these metadata combination merges with several values are acceptable or not')
             print('- If necessary, search for extra information in the original database (If the dataset was not originally uploaded to ENA, try at Sequence Read Archive, or DNA Data Bank of Japan)')
             print('- Check the original publication and supplementary tables to get some context')
-            print('- If necessary, contact the authors of the original publication and/or the ENA Support (https://www.ebi.ac.uk/ena/browser/support)')
             
             #Show saved file message
             print(rich_text_colored('\nSaving report in file:', 'general_text', plain_text_bool))
             print(outreport_path)
             
             #Save template
             warnings_df.to_csv(outreport_path, header = True, index = False, sep = '\t')
```

### Comparing `omdctk-1.0/src/omdctk.egg-info/PKG-INFO` & `omdctk-1.1.0/src/omdctk.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,42 @@
 Metadata-Version: 2.1
 Name: omdctk
-Version: 1.0
+Version: 1.1.0
 Summary: OMD Curation Toolkit
 Author-email: Samuel Piquer Esteban <samuel.piquer@uv.es>
 Project-URL: GitHub, https://github.com/tbcgit/omdctk
 Project-URL: Documentation, https://github.com/tbcgit/omdctk/wiki
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aioftp
+Requires-Dist: aiohttp
+Requires-Dist: parfive
+Requires-Dist: termcolor
+Requires-Dist: tabulate
+Requires-Dist: tqdm
+Requires-Dist: mg-toolkit
+Requires-Dist: pandas
 
 # OMD Curation Toolkit
-Omics Dataset Curation Toolkit (**OMD Curation Toolkit**) is a suite of programs designed for the download and curation of metadata and fastq files of public omics datasets. Centered on the European Nucleotide Archive (ENA), this workflow provides a standardized framework intended to facilitate the arduous task of curating public omics projects.
+Omics Dataset Curation Toolkit (**OMD Curation Toolkit**) is a suite of programs designed for the download and curation of metadata and fastq files of public omics datasets. This workflow provides a standardized framework intended to facilitate the arduous task of curating public omics projects. While centered on the European Nucleotide Archive (ENA), the majority of provided tools are generic and can be used to curate datasets from different sources.
 
 ## Getting started
 For further details, see the following:
 * **Documentation** (https://github.com/tbcgit/omdctk/wiki)
 * **Installation** (https://github.com/tbcgit/omdctk/wiki/Installation)
 * **Tutorial Full Example** (https://github.com/tbcgit/omdctk/wiki/Tutorial-Full-Example)
-  
+
+## Citation
+If you use OMD Curation Toolkit, please cite:
+Piquer-Esteban, S., Arnau, V., Diaz, W. et al. OMD Curation Toolkit: a workflow for in-house curation of public omics datasets. BMC Bioinformatics 25, 184 (2024). https://doi.org/10.1186/s12859-024-05803-9
+
 ## Acknowledgements
 This package has been jointly developed in the **Theory, Bioinformatics and Computation** (https://www.uv.es/tbc) and **Evolutionary Genetics** (https://www.uv.es/symbiosis) research groups at the **Institute for Integrative Systems Biology (I2SysBio)**, University of Valencia and Consejo Superior de Investigaciones Científicas (CSIC), Valencia, Spain. SPE is supported by an FPU grant from the Spanish Ministry of Universities (Reference: FPU20/05756).
 
 ## License
 This package is licensed under the MIT License. See the LICENSE file for details.
```

