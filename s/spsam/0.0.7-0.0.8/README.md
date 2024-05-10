# Comparing `tmp/spsam-0.0.7.tar.gz` & `tmp/spsam-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spsam-0.0.7.tar", last modified: Mon Apr 15 08:19:14 2024, max compression
+gzip compressed data, was "spsam-0.0.8.tar", last modified: Fri May 10 09:27:11 2024, max compression
```

## Comparing `spsam-0.0.7.tar` & `spsam-0.0.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 08:19:14.106663 spsam-0.0.7/
--rw-rw-rw-   0        0        0        0 2024-02-03 13:10:46.000000 spsam-0.0.7/LICENSE
--rw-rw-rw-   0        0        0        0 2024-02-03 13:12:25.000000 spsam-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0      843 2024-04-15 08:19:14.105663 spsam-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      105 2024-02-22 07:07:45.000000 spsam-0.0.7/README.md
--rw-rw-rw-   0        0        0      755 2024-03-08 01:18:43.000000 spsam-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-15 08:19:14.106663 spsam-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-15 08:19:13.948679 spsam-0.0.7/src/
--rw-rw-rw-   0        0        0      490 2024-02-03 13:12:00.000000 spsam-0.0.7/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 08:19:13.955663 spsam-0.0.7/src/spsam/
--rw-rw-rw-   0        0        0      328 2024-03-02 13:54:23.000000 spsam-0.0.7/src/spsam/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 08:19:13.994752 spsam-0.0.7/src/spsam/get/
--rw-rw-rw-   0        0        0       30 2024-01-31 07:57:24.000000 spsam-0.0.7/src/spsam/get/__init__.py
--rw-rw-rw-   0        0        0      607 2024-02-02 06:13:06.000000 spsam-0.0.7/src/spsam/get/get.py
-drwxrwxrwx   0        0        0        0 2024-04-15 08:19:14.035678 spsam-0.0.7/src/spsam/plotting/
--rw-rw-rw-   0        0        0      232 2024-02-07 09:10:14.000000 spsam-0.0.7/src/spsam/plotting/__init__.py
--rw-rw-rw-   0        0        0     7953 2024-04-14 05:56:59.000000 spsam-0.0.7/src/spsam/plotting/_anndata.py
--rw-rw-rw-   0        0        0    54187 2024-02-07 09:10:14.000000 spsam-0.0.7/src/spsam/plotting/_scatterplots.py
-drwxrwxrwx   0        0        0        0 2024-04-15 08:19:14.036663 spsam-0.0.7/src/spsam/plotting/_tools/
--rw-rw-rw-   0        0        0        0 2024-02-07 08:44:19.000000 spsam-0.0.7/src/spsam/plotting/_tools/__init__.py
--rw-rw-rw-   0        0        0     4615 2023-08-31 09:31:29.000000 spsam-0.0.7/src/spsam/plotting/palettes.py
-drwxrwxrwx   0        0        0        0 2024-04-15 08:19:14.086665 spsam-0.0.7/src/spsam/preprocessing/
--rw-rw-rw-   0        0        0      229 2024-02-03 12:53:59.000000 spsam-0.0.7/src/spsam/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     1631 2024-02-08 07:55:27.000000 spsam-0.0.7/src/spsam/preprocessing/_cycle_spot_count.py
--rw-rw-rw-   0        0        0     6391 2024-02-01 05:21:17.000000 spsam-0.0.7/src/spsam/preprocessing/_find_core_area.py
--rw-rw-rw-   0        0        0      906 2024-02-08 07:55:01.000000 spsam-0.0.7/src/spsam/preprocessing/_get_cell_abundance.py
--rw-rw-rw-   0        0        0     1112 2024-02-03 12:53:59.000000 spsam-0.0.7/src/spsam/preprocessing/_minmaxscaler.py
--rw-rw-rw-   0        0        0     1119 2024-01-31 08:36:04.000000 spsam-0.0.7/src/spsam/preprocessing/_score_lever.py
-drwxrwxrwx   0        0        0        0 2024-04-15 08:19:14.102762 spsam-0.0.7/src/spsam/tools/
--rw-rw-rw-   0        0        0       39 2024-02-07 08:17:11.000000 spsam-0.0.7/src/spsam/tools/__init__.py
--rw-rw-rw-   0        0        0     6316 2024-02-07 05:27:41.000000 spsam-0.0.7/src/spsam/tools/_score_genes.py
-drwxrwxrwx   0        0        0        0 2024-04-15 08:19:14.104663 spsam-0.0.7/src/spsam.egg-info/
--rw-rw-rw-   0        0        0      843 2024-04-15 08:19:13.000000 spsam-0.0.7/src/spsam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      772 2024-04-15 08:19:13.000000 spsam-0.0.7/src/spsam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 08:19:13.000000 spsam-0.0.7/src/spsam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      112 2024-04-15 08:19:13.000000 spsam-0.0.7/src/spsam.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-15 08:19:13.000000 spsam-0.0.7/src/spsam.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 09:27:11.697027 spsam-0.0.8/
+-rw-rw-rw-   0        0        0        0 2024-02-03 13:10:46.000000 spsam-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0        0 2024-02-03 13:12:25.000000 spsam-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      837 2024-05-10 09:27:11.696026 spsam-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      105 2024-02-22 07:07:45.000000 spsam-0.0.8/README.md
+-rw-rw-rw-   0        0        0      749 2024-05-10 09:26:40.000000 spsam-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-10 09:27:11.697027 spsam-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-10 09:27:11.564405 spsam-0.0.8/src/
+-rw-rw-rw-   0        0        0      490 2024-02-03 13:12:00.000000 spsam-0.0.8/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:27:11.570427 spsam-0.0.8/src/spsam/
+-rw-rw-rw-   0        0        0      328 2024-03-02 13:54:23.000000 spsam-0.0.8/src/spsam/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:27:11.603428 spsam-0.0.8/src/spsam/get/
+-rw-rw-rw-   0        0        0       30 2024-01-31 07:57:24.000000 spsam-0.0.8/src/spsam/get/__init__.py
+-rw-rw-rw-   0        0        0      607 2024-02-02 06:13:06.000000 spsam-0.0.8/src/spsam/get/get.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:27:11.636506 spsam-0.0.8/src/spsam/plotting/
+-rw-rw-rw-   0        0        0      232 2024-02-07 09:10:14.000000 spsam-0.0.8/src/spsam/plotting/__init__.py
+-rw-rw-rw-   0        0        0     7953 2024-04-14 05:56:59.000000 spsam-0.0.8/src/spsam/plotting/_anndata.py
+-rw-rw-rw-   0        0        0    54187 2024-02-07 09:10:14.000000 spsam-0.0.8/src/spsam/plotting/_scatterplots.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:27:11.638412 spsam-0.0.8/src/spsam/plotting/_tools/
+-rw-rw-rw-   0        0        0        0 2024-02-07 08:44:19.000000 spsam-0.0.8/src/spsam/plotting/_tools/__init__.py
+-rw-rw-rw-   0        0        0     4615 2023-08-31 09:31:29.000000 spsam-0.0.8/src/spsam/plotting/palettes.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:27:11.679043 spsam-0.0.8/src/spsam/preprocessing/
+-rw-rw-rw-   0        0        0      229 2024-02-03 12:53:59.000000 spsam-0.0.8/src/spsam/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     2107 2024-05-10 09:00:05.000000 spsam-0.0.8/src/spsam/preprocessing/_cycle_spot_count.py
+-rw-rw-rw-   0        0        0     6391 2024-02-01 05:21:17.000000 spsam-0.0.8/src/spsam/preprocessing/_find_core_area.py
+-rw-rw-rw-   0        0        0      906 2024-02-08 07:55:01.000000 spsam-0.0.8/src/spsam/preprocessing/_get_cell_abundance.py
+-rw-rw-rw-   0        0        0     1112 2024-02-03 12:53:59.000000 spsam-0.0.8/src/spsam/preprocessing/_minmaxscaler.py
+-rw-rw-rw-   0        0        0     1119 2024-01-31 08:36:04.000000 spsam-0.0.8/src/spsam/preprocessing/_score_lever.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:27:11.694048 spsam-0.0.8/src/spsam/tools/
+-rw-rw-rw-   0        0        0       39 2024-02-07 08:17:11.000000 spsam-0.0.8/src/spsam/tools/__init__.py
+-rw-rw-rw-   0        0        0     6316 2024-02-07 05:27:41.000000 spsam-0.0.8/src/spsam/tools/_score_genes.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:27:11.695027 spsam-0.0.8/src/spsam.egg-info/
+-rw-rw-rw-   0        0        0      837 2024-05-10 09:27:11.000000 spsam-0.0.8/src/spsam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      772 2024-05-10 09:27:11.000000 spsam-0.0.8/src/spsam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 09:27:11.000000 spsam-0.0.8/src/spsam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      112 2024-05-10 09:27:11.000000 spsam-0.0.8/src/spsam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-10 09:27:11.000000 spsam-0.0.8/src/spsam.egg-info/top_level.txt
```

### Comparing `spsam-0.0.7/PKG-INFO` & `spsam-0.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: spsam
-Version: 0.0.7
+Version: 0.0.8
 Summary: spSAM: 10X visium spot Split Align Map
-Author-email: renzhg <rzgedu@163.com>
-Project-URL: Homepage, https://github.com/renzhonggan/spsam
-Project-URL: Bug Tracker, https://github.com/renzhonggan/spsam/issues
+Author-email: Erganzi <xxx@163.com>
+Project-URL: Homepage, https://github.com/erganzi90/spsam
+Project-URL: Bug Tracker, https://github.com/erganzi90/spsam/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9.17
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: plotly==5.17.0
```

### Comparing `spsam-0.0.7/src/spsam/get/get.py` & `spsam-0.0.8/src/spsam/get/get.py`

 * *Files identical despite different names*

### Comparing `spsam-0.0.7/src/spsam/plotting/_anndata.py` & `spsam-0.0.8/src/spsam/plotting/_anndata.py`

 * *Files identical despite different names*

### Comparing `spsam-0.0.7/src/spsam/plotting/_scatterplots.py` & `spsam-0.0.8/src/spsam/plotting/_scatterplots.py`

 * *Files identical despite different names*

### Comparing `spsam-0.0.7/src/spsam/plotting/palettes.py` & `spsam-0.0.8/src/spsam/plotting/palettes.py`

 * *Files identical despite different names*

### Comparing `spsam-0.0.7/src/spsam/preprocessing/_find_core_area.py` & `spsam-0.0.8/src/spsam/preprocessing/_find_core_area.py`

 * *Files identical despite different names*

### Comparing `spsam-0.0.7/src/spsam/preprocessing/_get_cell_abundance.py` & `spsam-0.0.8/src/spsam/preprocessing/_get_cell_abundance.py`

 * *Files identical despite different names*

### Comparing `spsam-0.0.7/src/spsam/preprocessing/_minmaxscaler.py` & `spsam-0.0.8/src/spsam/preprocessing/_minmaxscaler.py`

 * *Files identical despite different names*

### Comparing `spsam-0.0.7/src/spsam/preprocessing/_score_lever.py` & `spsam-0.0.8/src/spsam/preprocessing/_score_lever.py`

 * *Files identical despite different names*

### Comparing `spsam-0.0.7/src/spsam/tools/_score_genes.py` & `spsam-0.0.8/src/spsam/tools/_score_genes.py`

 * *Files identical despite different names*

### Comparing `spsam-0.0.7/src/spsam.egg-info/PKG-INFO` & `spsam-0.0.8/src/spsam.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: spsam
-Version: 0.0.7
+Version: 0.0.8
 Summary: spSAM: 10X visium spot Split Align Map
-Author-email: renzhg <rzgedu@163.com>
-Project-URL: Homepage, https://github.com/renzhonggan/spsam
-Project-URL: Bug Tracker, https://github.com/renzhonggan/spsam/issues
+Author-email: Erganzi <xxx@163.com>
+Project-URL: Homepage, https://github.com/erganzi90/spsam
+Project-URL: Bug Tracker, https://github.com/erganzi90/spsam/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9.17
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: plotly==5.17.0
```

### Comparing `spsam-0.0.7/src/spsam.egg-info/SOURCES.txt` & `spsam-0.0.8/src/spsam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

