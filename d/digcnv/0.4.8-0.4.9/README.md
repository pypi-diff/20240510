# Comparing `tmp/digcnv-0.4.8.tar.gz` & `tmp/digcnv-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digcnv-0.4.8.tar", last modified: Fri Feb  9 03:34:30 2024, max compression
+gzip compressed data, was "digcnv-0.4.9.tar", last modified: Fri Feb  9 03:56:50 2024, max compression
```

## Comparing `digcnv-0.4.8.tar` & `digcnv-0.4.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-02-09 03:34:30.837295 digcnv-0.4.8/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    35149 2024-02-03 00:54:46.000000 digcnv-0.4.8/LICENSE
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       22 2024-02-05 00:26:09.000000 digcnv-0.4.8/MANIFEST.in
--rw-r--r--   0 thomas    (1000) thomas    (1000)    50866 2024-02-09 03:34:30.833295 digcnv-0.4.8/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     9084 2024-02-03 00:54:46.000000 digcnv-0.4.8/README.md
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-02-09 03:34:30.825295 digcnv-0.4.8/digcnv/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5784 2024-02-03 00:54:46.000000 digcnv-0.4.8/digcnv/CNVision.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3707 2024-02-03 00:54:46.000000 digcnv-0.4.8/digcnv/DigCnvPreProcessing.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4750 2024-02-03 00:54:46.000000 digcnv-0.4.8/digcnv/DigCnvTunning.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2024-02-03 00:54:46.000000 digcnv-0.4.8/digcnv/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3320 2024-02-06 18:01:05.000000 digcnv-0.4.8/digcnv/__main__.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-02-09 03:34:30.829295 digcnv-0.4.8/digcnv/data/
--rwxrwxr-x   0 thomas    (1000) thomas    (1000)    33389 2024-02-03 00:54:46.000000 digcnv-0.4.8/digcnv/data/CNVision_format_merge_ukbb.pl
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      605 2024-02-03 00:54:47.000000 digcnv-0.4.8/digcnv/data/Region_centromere_hg19.dat
--rw-rw-r--   0 thomas    (1000) thomas    (1000)   373840 2024-02-03 00:54:47.000000 digcnv-0.4.8/digcnv/data/SegDup_filtres_Ok_Oct.map
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    11836 2024-02-04 23:52:52.000000 digcnv-0.4.8/digcnv/dataPreparation.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5623 2024-02-03 00:54:47.000000 digcnv-0.4.8/digcnv/dataVerif.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      434 2024-02-03 00:54:47.000000 digcnv-0.4.8/digcnv/digCNV_logger.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    14090 2024-02-09 03:25:33.000000 digcnv-0.4.8/digcnv/digCnvModel.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2670 2024-02-04 23:48:11.000000 digcnv-0.4.8/digcnv/utils.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-02-09 03:34:30.833295 digcnv-0.4.8/digcnv.egg-info/
--rw-r--r--   0 thomas    (1000) thomas    (1000)    50866 2024-02-09 03:34:30.000000 digcnv-0.4.8/digcnv.egg-info/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      618 2024-02-09 03:34:30.000000 digcnv-0.4.8/digcnv.egg-info/SOURCES.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2024-02-09 03:34:30.000000 digcnv-0.4.8/digcnv.egg-info/dependency_links.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       48 2024-02-09 03:34:30.000000 digcnv-0.4.8/digcnv.egg-info/entry_points.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       96 2024-02-09 03:34:30.000000 digcnv-0.4.8/digcnv.egg-info/requires.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        7 2024-02-09 03:34:30.000000 digcnv-0.4.8/digcnv.egg-info/top_level.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1388 2024-02-09 03:27:19.000000 digcnv-0.4.8/pyproject.toml
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       38 2024-02-09 03:34:30.837295 digcnv-0.4.8/setup.cfg
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-02-09 03:34:30.833295 digcnv-0.4.8/tests/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1079 2024-02-04 01:10:13.000000 digcnv-0.4.8/tests/test_dataPreparation.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2024-02-03 00:54:47.000000 digcnv-0.4.8/tests/test_dataVerif.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-02-09 03:56:50.191520 digcnv-0.4.9/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    35149 2024-02-03 00:54:46.000000 digcnv-0.4.9/LICENSE
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       22 2024-02-05 00:26:09.000000 digcnv-0.4.9/MANIFEST.in
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    50866 2024-02-09 03:56:50.191520 digcnv-0.4.9/PKG-INFO
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     9084 2024-02-03 00:54:46.000000 digcnv-0.4.9/README.md
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-02-09 03:56:50.183520 digcnv-0.4.9/digcnv/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5784 2024-02-03 00:54:46.000000 digcnv-0.4.9/digcnv/CNVision.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3707 2024-02-03 00:54:46.000000 digcnv-0.4.9/digcnv/DigCnvPreProcessing.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4750 2024-02-03 00:54:46.000000 digcnv-0.4.9/digcnv/DigCnvTunning.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2024-02-03 00:54:46.000000 digcnv-0.4.9/digcnv/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3320 2024-02-06 18:01:05.000000 digcnv-0.4.9/digcnv/__main__.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-02-09 03:56:50.187520 digcnv-0.4.9/digcnv/data/
+-rwxrwxr-x   0 thomas    (1000) thomas    (1000)    33389 2024-02-03 00:54:46.000000 digcnv-0.4.9/digcnv/data/CNVision_format_merge_ukbb.pl
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      605 2024-02-03 00:54:47.000000 digcnv-0.4.9/digcnv/data/Region_centromere_hg19.dat
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)   373840 2024-02-03 00:54:47.000000 digcnv-0.4.9/digcnv/data/SegDup_filtres_Ok_Oct.map
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    11836 2024-02-04 23:52:52.000000 digcnv-0.4.9/digcnv/dataPreparation.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5623 2024-02-03 00:54:47.000000 digcnv-0.4.9/digcnv/dataVerif.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      434 2024-02-03 00:54:47.000000 digcnv-0.4.9/digcnv/digCNV_logger.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    14090 2024-02-09 03:56:10.000000 digcnv-0.4.9/digcnv/digCnvModel.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2670 2024-02-04 23:48:11.000000 digcnv-0.4.9/digcnv/utils.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-02-09 03:56:50.187520 digcnv-0.4.9/digcnv.egg-info/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    50866 2024-02-09 03:56:50.000000 digcnv-0.4.9/digcnv.egg-info/PKG-INFO
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      618 2024-02-09 03:56:50.000000 digcnv-0.4.9/digcnv.egg-info/SOURCES.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2024-02-09 03:56:50.000000 digcnv-0.4.9/digcnv.egg-info/dependency_links.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       48 2024-02-09 03:56:50.000000 digcnv-0.4.9/digcnv.egg-info/entry_points.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       96 2024-02-09 03:56:50.000000 digcnv-0.4.9/digcnv.egg-info/requires.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        7 2024-02-09 03:56:50.000000 digcnv-0.4.9/digcnv.egg-info/top_level.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1388 2024-02-09 03:56:21.000000 digcnv-0.4.9/pyproject.toml
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       38 2024-02-09 03:56:50.191520 digcnv-0.4.9/setup.cfg
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-02-09 03:56:50.187520 digcnv-0.4.9/tests/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1079 2024-02-04 01:10:13.000000 digcnv-0.4.9/tests/test_dataPreparation.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2024-02-03 00:54:47.000000 digcnv-0.4.9/tests/test_dataVerif.py
```

### Comparing `digcnv-0.4.8/LICENSE` & `digcnv-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `digcnv-0.4.8/PKG-INFO` & `digcnv-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digcnv
-Version: 0.4.8
+Version: 0.4.9
 Summary: DigCNV: Discriminating True CNVs from artifacts from genotyping without further visualisation
 Author-email: Thomas Renne <thomas.renne@umontreal.ca>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `digcnv-0.4.8/README.md` & `digcnv-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `digcnv-0.4.8/digcnv/CNVision.py` & `digcnv-0.4.9/digcnv/CNVision.py`

 * *Files identical despite different names*

### Comparing `digcnv-0.4.8/digcnv/DigCnvPreProcessing.py` & `digcnv-0.4.9/digcnv/DigCnvPreProcessing.py`

 * *Files identical despite different names*

### Comparing `digcnv-0.4.8/digcnv/DigCnvTunning.py` & `digcnv-0.4.9/digcnv/DigCnvTunning.py`

 * *Files identical despite different names*

### Comparing `digcnv-0.4.8/digcnv/__main__.py` & `digcnv-0.4.9/digcnv/__main__.py`

 * *Files identical despite different names*

### Comparing `digcnv-0.4.8/digcnv/data/CNVision_format_merge_ukbb.pl` & `digcnv-0.4.9/digcnv/data/CNVision_format_merge_ukbb.pl`

 * *Files identical despite different names*

### Comparing `digcnv-0.4.8/digcnv/data/Region_centromere_hg19.dat` & `digcnv-0.4.9/digcnv/data/Region_centromere_hg19.dat`

 * *Files identical despite different names*

### Comparing `digcnv-0.4.8/digcnv/data/SegDup_filtres_Ok_Oct.map` & `digcnv-0.4.9/digcnv/data/SegDup_filtres_Ok_Oct.map`

 * *Files identical despite different names*

### Comparing `digcnv-0.4.8/digcnv/dataPreparation.py` & `digcnv-0.4.9/digcnv/dataPreparation.py`

 * *Files identical despite different names*

### Comparing `digcnv-0.4.8/digcnv/dataVerif.py` & `digcnv-0.4.9/digcnv/dataVerif.py`

 * *Files identical despite different names*

### Comparing `digcnv-0.4.8/digcnv/digCnvModel.py` & `digcnv-0.4.9/digcnv/digCnvModel.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,15 +203,15 @@
         :param training_cat: A list of binary annotation for CNVs indicating if each CNV is a True CNV or an artefact, must int values.
         :type training_cat: pd.Series
         """   
         scaler = preprocessing.MinMaxScaler()
         cols = training_data.columns
         X_train_scale = pd.DataFrame(scaler.fit_transform(training_data, training_cat), columns=cols) 
         for col in cols:
-            self._dimensions_ranges[col] = [training_data[col].min(), training_data[col].min()] 
+            self._dimensions_ranges[col] = [training_data[col].min(), training_data[col].max()] 
         self._dimensions = X_train_scale.columns.tolist()
         self._model.fit(X_train_scale, training_cat)
 
     def saveDigCnvModelToPkl(self, output_path: str):
         """Save a trained DigCNV model to a pkl file to be used later
 
         :param output_path: Pathway of the pkl file must be finishing by `,pkl`
```

### Comparing `digcnv-0.4.8/digcnv/utils.py` & `digcnv-0.4.9/digcnv/utils.py`

 * *Files identical despite different names*

### Comparing `digcnv-0.4.8/digcnv.egg-info/PKG-INFO` & `digcnv-0.4.9/digcnv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digcnv
-Version: 0.4.8
+Version: 0.4.9
 Summary: DigCNV: Discriminating True CNVs from artifacts from genotyping without further visualisation
 Author-email: Thomas Renne <thomas.renne@umontreal.ca>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `digcnv-0.4.8/digcnv.egg-info/SOURCES.txt` & `digcnv-0.4.9/digcnv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `digcnv-0.4.8/pyproject.toml` & `digcnv-0.4.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "digcnv"
-version = "0.4.8"
+version = "0.4.9"
 description = "DigCNV: Discriminating True CNVs from artifacts from genotyping without further visualisation"
 readme = "README.md"
 authors = [{ name = "Thomas Renne", email = "thomas.renne@umontreal.ca" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Programming Language :: Python",
```

### Comparing `digcnv-0.4.8/tests/test_dataPreparation.py` & `digcnv-0.4.9/tests/test_dataPreparation.py`

 * *Files identical despite different names*

