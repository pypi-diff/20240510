# Comparing `tmp/digiflow-3.9.1.tar.gz` & `tmp/digiflow-3.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digiflow-3.9.1.tar", last modified: Fri Mar 22 14:09:07 2024, max compression
+gzip compressed data, was "digiflow-3.9.2.tar", last modified: Tue Apr 16 09:29:50 2024, max compression
```

## Comparing `digiflow-3.9.1.tar` & `digiflow-3.9.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2024-03-22 14:09:07.321465 digiflow-3.9.1/
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     1106 2023-07-03 13:56:57.000000 digiflow-3.9.1/LICENCE
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)      205 2023-11-23 08:43:37.000000 digiflow-3.9.1/MANIFEST.in
--rw-r--r--   0 hartwig   (1000) hartwig   (1000)     1580 2024-03-22 14:09:07.321465 digiflow-3.9.1/PKG-INFO
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)      979 2023-11-23 08:43:37.000000 digiflow-3.9.1/README.md
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)      731 2024-03-22 13:55:08.000000 digiflow-3.9.1/pyproject.toml
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       38 2024-03-22 14:09:07.321465 digiflow-3.9.1/setup.cfg
-drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2024-03-22 14:09:07.309465 digiflow-3.9.1/src/
-drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2024-03-22 14:09:07.313465 digiflow-3.9.1/src/digiflow/
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     1120 2024-03-12 14:41:33.000000 digiflow-3.9.1/src/digiflow/__init__.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    12685 2023-07-03 13:38:30.000000 digiflow-3.9.1/src/digiflow/digflow_identifier.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    10920 2023-07-04 07:12:14.000000 digiflow-3.9.1/src/digiflow/digiflow_export.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    17210 2023-11-29 13:33:05.000000 digiflow-3.9.1/src/digiflow/digiflow_generate.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    39114 2024-03-22 13:39:22.000000 digiflow-3.9.1/src/digiflow/digiflow_io.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    31833 2023-12-18 13:32:45.000000 digiflow-3.9.1/src/digiflow/digiflow_metadata.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    10145 2024-02-26 10:19:11.000000 digiflow-3.9.1/src/digiflow/digiflow_validate.py
-drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2024-03-22 14:09:07.313465 digiflow-3.9.1/src/digiflow/resources/
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     2676 2023-07-04 07:49:18.000000 digiflow-3.9.1/src/digiflow/resources/digilife.ini
-drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2024-03-22 14:09:07.313465 digiflow-3.9.1/src/digiflow/resources/xsd/
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    55541 2023-07-03 13:38:30.000000 digiflow-3.9.1/src/digiflow/resources/xsd/alto_4-2.xsd
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)   135665 2023-07-03 13:38:30.000000 digiflow-3.9.1/src/digiflow/resources/xsd/mets_1-12.xsd
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    98153 2023-07-03 13:38:30.000000 digiflow-3.9.1/src/digiflow/resources/xsd/mix_2-0.xsd
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    52954 2023-07-03 13:38:30.000000 digiflow-3.9.1/src/digiflow/resources/xsd/mods_3-7.xsd
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    88414 2023-07-03 13:38:30.000000 digiflow-3.9.1/src/digiflow/resources/xsd/page_2019-07-15.xsd
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     3180 2023-07-03 13:38:30.000000 digiflow-3.9.1/src/digiflow/resources/xsd/xlink.xsd
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     5840 2023-07-03 13:38:30.000000 digiflow-3.9.1/src/digiflow/resources/xsd/xml.xsd
-drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2024-03-22 14:09:07.317465 digiflow-3.9.1/src/digiflow/resources/xsl/
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)   384070 2023-11-22 11:23:45.000000 digiflow-3.9.1/src/digiflow/resources/xsl/ddb_validierung_mets-mods-ap-digitalisierte-medien.xsl
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)   255279 2023-11-23 14:08:32.000000 digiflow-3.9.1/src/digiflow/resources/xsl/ddb_validierung_mets-mods-ap-digitalisierte-zeitungen.xsl
-drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2024-03-22 14:09:07.317465 digiflow-3.9.1/src/digiflow/validate/
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)      801 2024-03-12 14:42:23.000000 digiflow-3.9.1/src/digiflow/validate/__init__.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)      810 2024-03-12 13:58:20.000000 digiflow-3.9.1/src/digiflow/validate/common.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     1470 2024-02-28 08:26:01.000000 digiflow-3.9.1/src/digiflow/validate/fsdata.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    15897 2024-03-12 14:40:39.000000 digiflow-3.9.1/src/digiflow/validate/imgdata.py
-drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2024-03-22 14:09:07.321465 digiflow-3.9.1/src/digiflow.egg-info/
--rw-r--r--   0 hartwig   (1000) hartwig   (1000)     1580 2024-03-22 14:09:07.000000 digiflow-3.9.1/src/digiflow.egg-info/PKG-INFO
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     1347 2024-03-22 14:09:07.000000 digiflow-3.9.1/src/digiflow.egg-info/SOURCES.txt
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)        1 2024-03-22 14:09:07.000000 digiflow-3.9.1/src/digiflow.egg-info/dependency_links.txt
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       43 2024-03-22 14:09:07.000000 digiflow-3.9.1/src/digiflow.egg-info/requires.txt
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)        9 2024-03-22 14:09:07.000000 digiflow-3.9.1/src/digiflow.egg-info/top_level.txt
-drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2024-03-22 14:09:07.317465 digiflow-3.9.1/tests/
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    13100 2023-08-08 11:38:16.000000 digiflow-3.9.1/tests/test_digiflow_generate.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    21727 2023-07-04 07:12:14.000000 digiflow-3.9.1/tests/test_digiflow_identifier.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    54655 2024-03-22 14:05:35.000000 digiflow-3.9.1/tests/test_digiflow_io.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    23083 2023-09-06 14:04:52.000000 digiflow-3.9.1/tests/test_digiflow_metadata.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     4235 2024-02-26 09:14:57.000000 digiflow-3.9.1/tests/test_digiflow_metadata_transform.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    11106 2024-02-22 13:35:11.000000 digiflow-3.9.1/tests/test_digiflow_validate_mets.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    15559 2023-08-08 11:38:09.000000 digiflow-3.9.1/tests/test_export_saf.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     1740 2024-02-28 08:26:01.000000 digiflow-3.9.1/tests/test_validate_fsdata.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     7972 2024-03-12 14:40:39.000000 digiflow-3.9.1/tests/test_validate_imgdata.py
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2024-04-16 09:29:50.207175 digiflow-3.9.2/
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     1106 2024-04-15 08:04:58.000000 digiflow-3.9.2/LICENCE
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)      205 2024-04-15 08:04:58.000000 digiflow-3.9.2/MANIFEST.in
+-rw-r--r--   0 hartwig   (1000) hartwig   (1000)     1580 2024-04-16 09:29:50.207175 digiflow-3.9.2/PKG-INFO
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)      979 2024-04-15 08:04:58.000000 digiflow-3.9.2/README.md
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)      731 2024-04-16 09:25:06.000000 digiflow-3.9.2/pyproject.toml
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       38 2024-04-16 09:29:50.207175 digiflow-3.9.2/setup.cfg
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2024-04-16 09:29:50.207175 digiflow-3.9.2/src/
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2024-04-16 09:29:50.207175 digiflow-3.9.2/src/digiflow/
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     1120 2024-04-15 08:04:58.000000 digiflow-3.9.2/src/digiflow/__init__.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    12685 2024-04-15 08:04:58.000000 digiflow-3.9.2/src/digiflow/digflow_identifier.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    10920 2024-04-15 08:04:58.000000 digiflow-3.9.2/src/digiflow/digiflow_export.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    17210 2024-04-15 08:04:58.000000 digiflow-3.9.2/src/digiflow/digiflow_generate.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    39114 2024-04-15 08:04:58.000000 digiflow-3.9.2/src/digiflow/digiflow_io.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    31866 2024-04-16 09:23:52.000000 digiflow-3.9.2/src/digiflow/digiflow_metadata.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    10145 2024-04-15 08:04:58.000000 digiflow-3.9.2/src/digiflow/digiflow_validate.py
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2024-04-16 09:29:50.207175 digiflow-3.9.2/src/digiflow/resources/
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     2676 2024-04-15 08:04:58.000000 digiflow-3.9.2/src/digiflow/resources/digilife.ini
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2024-04-16 09:29:50.207175 digiflow-3.9.2/src/digiflow/resources/xsd/
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    55541 2024-04-15 08:04:58.000000 digiflow-3.9.2/src/digiflow/resources/xsd/alto_4-2.xsd
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)   135665 2024-04-15 08:04:58.000000 digiflow-3.9.2/src/digiflow/resources/xsd/mets_1-12.xsd
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    98153 2024-04-15 08:04:58.000000 digiflow-3.9.2/src/digiflow/resources/xsd/mix_2-0.xsd
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    52954 2024-04-15 08:04:58.000000 digiflow-3.9.2/src/digiflow/resources/xsd/mods_3-7.xsd
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    88414 2024-04-15 08:04:58.000000 digiflow-3.9.2/src/digiflow/resources/xsd/page_2019-07-15.xsd
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     3180 2024-04-15 08:04:58.000000 digiflow-3.9.2/src/digiflow/resources/xsd/xlink.xsd
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     5840 2024-04-15 08:04:58.000000 digiflow-3.9.2/src/digiflow/resources/xsd/xml.xsd
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2024-04-16 09:29:50.207175 digiflow-3.9.2/src/digiflow/resources/xsl/
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)   384070 2024-04-15 08:04:58.000000 digiflow-3.9.2/src/digiflow/resources/xsl/ddb_validierung_mets-mods-ap-digitalisierte-medien.xsl
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)   255279 2024-04-15 08:04:58.000000 digiflow-3.9.2/src/digiflow/resources/xsl/ddb_validierung_mets-mods-ap-digitalisierte-zeitungen.xsl
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2024-04-16 09:29:50.207175 digiflow-3.9.2/src/digiflow/validate/
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)      801 2024-04-15 08:04:58.000000 digiflow-3.9.2/src/digiflow/validate/__init__.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)      810 2024-04-15 08:04:58.000000 digiflow-3.9.2/src/digiflow/validate/common.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     1470 2024-04-15 08:04:58.000000 digiflow-3.9.2/src/digiflow/validate/fsdata.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    15897 2024-04-15 08:04:58.000000 digiflow-3.9.2/src/digiflow/validate/imgdata.py
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2024-04-16 09:29:50.207175 digiflow-3.9.2/src/digiflow.egg-info/
+-rw-r--r--   0 hartwig   (1000) hartwig   (1000)     1580 2024-04-16 09:29:50.000000 digiflow-3.9.2/src/digiflow.egg-info/PKG-INFO
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     1347 2024-04-16 09:29:50.000000 digiflow-3.9.2/src/digiflow.egg-info/SOURCES.txt
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)        1 2024-04-16 09:29:50.000000 digiflow-3.9.2/src/digiflow.egg-info/dependency_links.txt
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       43 2024-04-16 09:29:50.000000 digiflow-3.9.2/src/digiflow.egg-info/requires.txt
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)        9 2024-04-16 09:29:50.000000 digiflow-3.9.2/src/digiflow.egg-info/top_level.txt
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2024-04-16 09:29:50.207175 digiflow-3.9.2/tests/
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    13100 2024-04-15 08:04:58.000000 digiflow-3.9.2/tests/test_digiflow_generate.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    21727 2024-04-15 08:04:58.000000 digiflow-3.9.2/tests/test_digiflow_identifier.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    55155 2024-04-15 08:04:58.000000 digiflow-3.9.2/tests/test_digiflow_io.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    23609 2024-04-16 09:21:54.000000 digiflow-3.9.2/tests/test_digiflow_metadata.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     4235 2024-04-15 08:04:58.000000 digiflow-3.9.2/tests/test_digiflow_metadata_transform.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    11106 2024-04-15 08:04:58.000000 digiflow-3.9.2/tests/test_digiflow_validate_mets.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    15559 2024-04-15 08:04:58.000000 digiflow-3.9.2/tests/test_export_saf.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     1740 2024-04-15 08:04:58.000000 digiflow-3.9.2/tests/test_validate_fsdata.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     7972 2024-04-15 08:04:58.000000 digiflow-3.9.2/tests/test_validate_imgdata.py
```

### Comparing `digiflow-3.9.1/LICENCE` & `digiflow-3.9.2/LICENCE`

 * *Files identical despite different names*

### Comparing `digiflow-3.9.1/PKG-INFO` & `digiflow-3.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digiflow
-Version: 3.9.1
+Version: 3.9.2
 Summary: Father's Little Digitization Workflow Helper
 Author-email: Universitäts- und Landesbibliothek Sachsen-Anhalt <development@bibliothek.uni-halle.de>
 Project-URL: Homepage, https://github.com/ulb-sachsen-anhalt/digital-flow
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `digiflow-3.9.1/README.md` & `digiflow-3.9.2/README.md`

 * *Files identical despite different names*

### Comparing `digiflow-3.9.1/pyproject.toml` & `digiflow-3.9.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "digiflow"
-version = "3.9.1"
+version = "3.9.2"
 description = "Father's Little Digitization Workflow Helper"
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [
 	{name = "Universitäts- und Landesbibliothek Sachsen-Anhalt", email = "development@bibliothek.uni-halle.de"}
 ]
 classifiers = [
```

### Comparing `digiflow-3.9.1/src/digiflow/__init__.py` & `digiflow-3.9.2/src/digiflow/__init__.py`

 * *Files identical despite different names*

### Comparing `digiflow-3.9.1/src/digiflow/digflow_identifier.py` & `digiflow-3.9.2/src/digiflow/digflow_identifier.py`

 * *Files identical despite different names*

### Comparing `digiflow-3.9.1/src/digiflow/digiflow_export.py` & `digiflow-3.9.2/src/digiflow/digiflow_export.py`

 * *Files identical despite different names*

### Comparing `digiflow-3.9.1/src/digiflow/digiflow_generate.py` & `digiflow-3.9.2/src/digiflow/digiflow_generate.py`

 * *Files identical despite different names*

### Comparing `digiflow-3.9.1/src/digiflow/digiflow_io.py` & `digiflow-3.9.2/src/digiflow/digiflow_io.py`

 * *Files identical despite different names*

### Comparing `digiflow-3.9.1/src/digiflow/digiflow_metadata.py` & `digiflow-3.9.2/src/digiflow/digiflow_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -316,15 +316,16 @@
 
     def contains_group(self, group: 'str|List[str]') -> bool:
         """Test if a certain fileGroup exists"""
 
         if isinstance(group, list):
             return any(self.tree.findall(PATTERN_FILEGROUP_USE.format(g), XMLNS)
                        for g in group)
-        return self.tree.findall(PATTERN_FILEGROUP_USE.format(group), XMLNS) > 0
+        _fgroups = self.tree.findall(PATTERN_FILEGROUP_USE.format(group), XMLNS)
+        return len(_fgroups) > 0
 
     def clear_filegroups(self, black_list=None):
         """Clear file Groups by blacklist"""
 
         cleared = 0
         file_sections = self.tree.findall('.//mets:fileSec', XMLNS)
         if len(file_sections) < 1:
```

### Comparing `digiflow-3.9.1/src/digiflow/digiflow_validate.py` & `digiflow-3.9.2/src/digiflow/digiflow_validate.py`

 * *Files identical despite different names*

### Comparing `digiflow-3.9.1/src/digiflow/resources/digilife.ini` & `digiflow-3.9.2/src/digiflow/resources/digilife.ini`

 * *Files identical despite different names*

### Comparing `digiflow-3.9.1/src/digiflow/resources/xsd/alto_4-2.xsd` & `digiflow-3.9.2/src/digiflow/resources/xsd/alto_4-2.xsd`

 * *Files identical despite different names*

### Comparing `digiflow-3.9.1/src/digiflow/resources/xsd/mets_1-12.xsd` & `digiflow-3.9.2/src/digiflow/resources/xsd/mets_1-12.xsd`

 * *Files identical despite different names*

### Comparing `digiflow-3.9.1/src/digiflow/resources/xsd/mix_2-0.xsd` & `digiflow-3.9.2/src/digiflow/resources/xsd/mix_2-0.xsd`

 * *Files identical despite different names*

### Comparing `digiflow-3.9.1/src/digiflow/resources/xsd/mods_3-7.xsd` & `digiflow-3.9.2/src/digiflow/resources/xsd/mods_3-7.xsd`

 * *Files identical despite different names*

### Comparing `digiflow-3.9.1/src/digiflow/resources/xsd/page_2019-07-15.xsd` & `digiflow-3.9.2/src/digiflow/resources/xsd/page_2019-07-15.xsd`

 * *Files identical despite different names*

### Comparing `digiflow-3.9.1/src/digiflow/resources/xsd/xlink.xsd` & `digiflow-3.9.2/src/digiflow/resources/xsd/xlink.xsd`

 * *Files identical despite different names*

### Comparing `digiflow-3.9.1/src/digiflow/resources/xsd/xml.xsd` & `digiflow-3.9.2/src/digiflow/resources/xsd/xml.xsd`

 * *Files identical despite different names*

### Comparing `digiflow-3.9.1/src/digiflow/resources/xsl/ddb_validierung_mets-mods-ap-digitalisierte-medien.xsl` & `digiflow-3.9.2/src/digiflow/resources/xsl/ddb_validierung_mets-mods-ap-digitalisierte-medien.xsl`

 * *Files identical despite different names*

### Comparing `digiflow-3.9.1/src/digiflow/resources/xsl/ddb_validierung_mets-mods-ap-digitalisierte-zeitungen.xsl` & `digiflow-3.9.2/src/digiflow/resources/xsl/ddb_validierung_mets-mods-ap-digitalisierte-zeitungen.xsl`

 * *Files identical despite different names*

### Comparing `digiflow-3.9.1/src/digiflow/validate/__init__.py` & `digiflow-3.9.2/src/digiflow/validate/__init__.py`

 * *Files identical despite different names*

### Comparing `digiflow-3.9.1/src/digiflow/validate/common.py` & `digiflow-3.9.2/src/digiflow/validate/common.py`

 * *Files identical despite different names*

### Comparing `digiflow-3.9.1/src/digiflow/validate/fsdata.py` & `digiflow-3.9.2/src/digiflow/validate/fsdata.py`

 * *Files identical despite different names*

### Comparing `digiflow-3.9.1/src/digiflow/validate/imgdata.py` & `digiflow-3.9.2/src/digiflow/validate/imgdata.py`

 * *Files identical despite different names*

### Comparing `digiflow-3.9.1/src/digiflow.egg-info/PKG-INFO` & `digiflow-3.9.2/src/digiflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digiflow
-Version: 3.9.1
+Version: 3.9.2
 Summary: Father's Little Digitization Workflow Helper
 Author-email: Universitäts- und Landesbibliothek Sachsen-Anhalt <development@bibliothek.uni-halle.de>
 Project-URL: Homepage, https://github.com/ulb-sachsen-anhalt/digital-flow
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `digiflow-3.9.1/src/digiflow.egg-info/SOURCES.txt` & `digiflow-3.9.2/src/digiflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `digiflow-3.9.1/tests/test_digiflow_generate.py` & `digiflow-3.9.2/tests/test_digiflow_generate.py`

 * *Files identical despite different names*

### Comparing `digiflow-3.9.1/tests/test_digiflow_identifier.py` & `digiflow-3.9.2/tests/test_digiflow_identifier.py`

 * *Files identical despite different names*

### Comparing `digiflow-3.9.1/tests/test_digiflow_io.py` & `digiflow-3.9.2/tests/test_digiflow_io.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,75 +1,74 @@
-# -*- coding: utf-8 -*-
+"""Specification for IO API"""
 
 import ast
 import json
 import os
-import pytest
 import shutil
 import sys
 import uuid
 from json.decoder import (
     JSONDecodeError
 )
 from pathlib import (
     Path
 )
-from smtplib import (
-    SMTP,
-)
 from unittest import (
     mock
 )
 
+import pytest
+
 import lxml.etree as ET
 
 from digiflow import (
-    write_xml_file,
-    OAIRecord,
-    OAIRecordCriteriaState,
-    OAIRecordCriteriaDatetime,
-    OAIRecordCriteriaIdentifier,
-    OAIRecordCriteriaText,
-    OAIFileSweeper,
-    OAIRecordHandler,
-    OAILoadException,
     F_IDENTIFIER,
     F_SPEC,
     F_DATESTAMP,
     F_STATE_INFO,
     F_STATE,
     F_STATE_TS,
     RECORD_STATE_MASK_FRAME,
     HEADER_MIGRATION,
+    OAIRecord,
+    OAIRecordCriteriaState,
+    OAIRecordCriteriaDatetime,
+    OAIRecordCriteriaIdentifier,
+    OAIRecordCriteriaText,
+    OAIFileSweeper,
+    OAIRecordHandler,
+    OAILoadException,
     OAILoader,
     LocalStore,
+    get_enclosed,
     post_oai_extract_mets,
-    smtp_note,
     request_resource,
+    smtp_note,
     transform_to_record,
-    get_enclosed,
+    write_xml_file,
 )
 
 from .conftest import (
     TEST_RES
 )
 
 ROOT = Path(__file__).parents[1]
 
 EXPORT_METS = 'export_mets.xml'
 
 # some test constants
 ID_737429 = '737429'
-OAI_ID_737429 = 'oai:digital.bibliothek.uni-halle.de/hd:{}'.format(ID_737429)
+OAI_ID_737429 = f'oai:digital.bibliothek.uni-halle.de/hd:{ID_737429}'
 OAI_SPEC_737429 = 'ulbhaldod'
 CONTENT_TYPE_TXT = 'text/xml;charset=utf-8'
 OAI_BASE_URL_VD16 = 'digitale.bibliothek.uni-halle.de/vd16/oai'
 OAI_BASE_URL_ZD = 'digitale.bibliothek.uni-halle.de/zd/oai'
 OAI_BASE_URL_OPENDATA = 'opendata.uni-halle.de/oai/dd'
 
+# pylint: disable=c-extension-no-member, line-too-long
 
 @pytest.mark.skipif("sys.version_info < (3,6)")
 def test_intermediate_dirs_created_with_path(tmp_path):
     """Test depends on PosixPath, only works with 3.6+"""
 
     src_path = TEST_RES / "k2_mets_vd18_147638674.xml"
     path_dst = tmp_path / "sub_dir" / "another_sub_dir" / "147638674.xml"
@@ -92,42 +91,47 @@
     # act
     write_xml_file(xml.getroot(), str(path_dst))
 
     assert os.path.isfile(str(path_dst))
 
 
 def test_write_xml_defaults(tmp_path):
+    """Output with deafult write settings"""
+
     txt = '<parent><child name="foo">bar</child></parent>'
     xml_tree = ET.fromstring(txt)
     outpath = tmp_path / "write_foo.xml"
     write_xml_file(xml_tree, str(outpath))
 
     assert os.path.isfile(str(outpath))
-    assert open(str(outpath)).read().startswith(
+    assert open(str(outpath), encoding='utf8').read().startswith(
         '<?xml version="1.0" encoding="UTF-8"?>\n')
 
 
 def test_write_xml_without_preamble(tmp_path):
+    """Test output if no preamble required"""
+
     txt = '<parent><child name="foo">bar</child></parent>'
     xml_tree = ET.fromstring(txt)
     outpath = tmp_path / "write_foo.xml"
     write_xml_file(xml_tree, str(outpath), preamble=None)
 
     assert os.path.isfile(str(outpath))
-    assert open(str(outpath)).read().startswith('<parent>\n')
+    assert open(str(outpath), encoding='utf8').read().startswith('<parent>\n')
 
 
 @pytest.mark.parametrize(['urn', 'local_identifier'],
                          [
     ('oai:digital.bibliothek.uni-halle.de/hd:10595', '10595'),
     ('oai:digitale.bibliothek.uni-halle.de/vd18:9427342', '9427342'),
     ('oai:opendata.uni-halle.de:1981185920/34265', '1981185920_34265'),
     ('oai:dev.opendata.uni-halle.de:123456789/27949', '123456789_27949'),
 ])
 def test_record_local_identifiers(urn, local_identifier):
+    """Ensure local identifier for different URN inputs"""
 
     # act
     record = OAIRecord(urn)
     assert record.local_identifier == local_identifier
 
 
 def fixture_request_results(*args, **kwargs):
@@ -270,20 +274,19 @@
     assert os.path.isfile(str(local_dir / (_id + ".xml")))
     assert os.path.isfile(str(local_dir / "MAX" / "00000011.jpg"))
 
     # check cache
     assert os.path.exists(str(store_dir))
 
 
-DEFAULT_HEADERS = "{}\t{}\t{}\t{}\t{}\t{}\n"\
-    .format(F_IDENTIFIER, F_SPEC, F_DATESTAMP, F_STATE_INFO, F_STATE, F_STATE_TS)
+DEFAULT_HEADERS = f"{F_IDENTIFIER}\t{F_SPEC}\t{F_DATESTAMP}\t{F_STATE_INFO}\t{F_STATE}\t{F_STATE_TS}\n"
 
 
 def _write_datalist(path_data_list, data, headers=DEFAULT_HEADERS):
-    with open(str(path_data_list), 'w') as handle:
+    with open(str(path_data_list), 'w', encoding='utf8') as handle:
         if headers:
             handle.write(headers)
         handle.writelines(data)
 
 
 def test_invalid_input_data(tmp_path):
     """Invalid input data format raises an exception"""
@@ -404,15 +407,15 @@
     # assert
     assert a_set.local_identifier == '1416976'
     handler.save_record_state(a_set.identifier, 'metadata_done', INFO='123,ger')
     handler.save_record_state(a_set.identifier, 'migration_done')
 
     a_set = handler.next_record(state='migration_done')
     assert a_set.local_identifier == '1416976'
-    with open(vl_datasets) as reader:
+    with open(vl_datasets, encoding='utf8') as reader:
         lines = reader.readlines()
     assert lines[1].split('\t')[3] == '123,ger'
 
 
 def test_dataset_cannot_find_entry(vl_datasets):
     """Behavior if want to store with unknown identifier"""
 
@@ -428,23 +431,23 @@
 
 
 def test_statelist_ocr_hdz(tmp_path):
     """Behavior of state lists for ocr pipeline"""
 
     # arrange
     path_state_list = tmp_path / 'ocr_list'
-    first_row = "{}\t{}\t{}\n".format(F_IDENTIFIER, F_STATE, F_STATE_TS)
+    first_row = f"{F_IDENTIFIER}\t{F_STATE}\t{F_STATE_TS}\n"
     data = [
         'oai:digitale.bibliothek.uni-halle.de/zd:123\tn.a.\tn.a.\n'
     ]
     _write_datalist(path_state_list, data, first_row)
-    headers = [F_IDENTIFIER, F_STATE, F_STATE_TS]
+    _headers = [F_IDENTIFIER, F_STATE, F_STATE_TS]
     handler = OAIRecordHandler(
         path_state_list,
-        data_fields=headers,
+        data_fields=_headers,
         transform_func=lambda r: r)
 
     # act
     record = handler.next_record()
     assert handler.position == '0001/0001'
     assert record[F_IDENTIFIER] == 'oai:digitale.bibliothek.uni-halle.de/zd:123'
     handler.save_record_state(record[F_IDENTIFIER])
@@ -453,16 +456,15 @@
     assert not handler.next_record()
 
     # assert there is a record next with default state 'lock'
     assert handler.next_record('busy')
 
 
 # record list header data
-OAI_LIST_HEADER = "{}\t{}\t{}\t{}\t{}\n".format(
-    F_IDENTIFIER, F_DATESTAMP, F_STATE_INFO, F_STATE, F_STATE_TS)
+OAI_LIST_HEADER = f"{F_IDENTIFIER}\t{F_DATESTAMP}\t{F_STATE_INFO}\t{F_STATE}\t{F_STATE_TS}\n"
 
 
 @pytest.fixture(name="oai_record_list")
 def _fixture_oai_record_list(tmp_path):
     path_state_list = tmp_path / 'ocr_list'
     data = [
         "oai:digitale.bibliothek.uni-halle.de/zd:8853011\t2015-08-25T20:00:35Z\tn.a.\tocr_skip\t2021-08-03_15:03:56\n",
@@ -481,24 +483,24 @@
     r[F_IDENTIFIER] = row[F_IDENTIFIER]
     r[F_STATE] = row[F_STATE]
     r[F_STATE_TS] = row[F_STATE_TS]
     return r
 
 
 # OAI record list default headers
-headers = [F_IDENTIFIER, F_DATESTAMP, F_STATE_INFO, F_STATE, F_STATE_TS]
+HEADERS = [F_IDENTIFIER, F_DATESTAMP, F_STATE_INFO, F_STATE, F_STATE_TS]
 
 
 def test_statelist_use_n_a_properly(oai_record_list):
     """Behavior of state lists for ocr pipeline"""
 
     # arrange
     handler = OAIRecordHandler(
         oai_record_list,
-        data_fields=headers,
+        data_fields=HEADERS,
         transform_func=_morph)
 
     # act
     record = handler.next_record()
     assert handler.position == '0006/0006'
     assert record[F_IDENTIFIER] == 'oai:digitale.bibliothek.uni-halle.de/zd:9510508'
     handler.save_record_state(record[F_IDENTIFIER])
@@ -541,18 +543,16 @@
         with open(alto_file + 'zd1-alto-16331001.xml', encoding="utf-8") as hndl:
             result.content = hndl.read().encode()
     return result
 
 
 @mock.patch("digiflow.requests.get")
 def test_oai_load_vls_zd1_with_ocr(mock_request, tmp_path):
-    """Behavior of state lists for ocr pipeline"""
-
-    # arrange
-    """test oai loader implementation for opendata"""
+    """Behavior of state lists for ocr pipeline
+    """
 
     # arrange
     mock_request.side_effect = fixture_request_vls_zd1_16359609
     ident = 'oai:digitale.bibliothek.uni-halle.de/zd:16359609'
     record = OAIRecord(ident)
     _id = record.local_identifier
     local_dir = tmp_path / "WORKDIR" / _id
@@ -638,17 +638,25 @@
     oais.sweep()
 
     for item in Path(migration_sweeper_pdf_fixture).iterdir():
         if str(item.name) == 'DOWNLOAD':
             assert len(list(item.iterdir())) == 0
 
 
-@mock.patch('digiflow.digiflow_io.SMTP.send_message')
+@mock.patch('digiflow.digiflow_io.SMTP')
 def test_send_mail(mock_smtp):
-    """test sending mail"""
+    """Test note using SMTP mock because
+    tails fails outside proper plattform
+    without reachable local smto-host
+
+    Mock called 3 times
+    * object init
+    * object sends message
+    * object quits connection
+    """
 
     # arrange
     random_message = uuid.uuid4().hex
 
     # act
     mess = smtp_note(
         'localhost:25',
@@ -656,25 +664,26 @@
         message=random_message,
         froms='test@example.com',
         tos='me@example.de')
 
     # assert
     assert random_message in mess
     assert 'me@example.de' in mess
-    assert mock_smtp is SMTP.send_message
-    # assert mock_smtp.called == True   # toxic doesnt like this
+    assert mock_smtp.called
+    assert len(mock_smtp.mock_calls) == 3
+    assert mock_smtp.mock_calls[1][0] == '().send_message'
 
 
 def test_record_state_list_set_state_from(oai_record_list):
     """Behavior for changing state matching state and start time"""
 
     # arrange
     handler = OAIRecordHandler(
         oai_record_list,
-        data_fields=headers,
+        data_fields=HEADERS,
         transform_func=_morph)
     c_state = OAIRecordCriteriaState('ocr_skip')
     c_from = OAIRecordCriteriaDatetime(dt_from='2021-08-03_15:03:56')
 
     # pre-check
     record1 = handler.next_record()
     assert record1[F_IDENTIFIER].endswith('9510508')
@@ -750,15 +759,15 @@
 
 def test_record_state_list_set_state_from_dry_run(oai_record_list):
     """Behavior of dry run"""
 
     # arrange
     handler = OAIRecordHandler(
         oai_record_list,
-        data_fields=headers,
+        data_fields=HEADERS,
         transform_func=_morph)
     c_state = OAIRecordCriteriaState('ocr_skip')
     c_from = OAIRecordCriteriaDatetime(dt_from='2021-08-03_15:03:56')
 
     # pre-check
     record1 = handler.next_record()
     assert record1[F_IDENTIFIER].endswith('9510508')
@@ -774,15 +783,15 @@
 
 def test_record_state_list_set_state_from_dry_run_verbose(oai_record_list, capsys):
     """Behavior of dry run"""
 
     # arrange
     handler = OAIRecordHandler(
         oai_record_list,
-        data_fields=headers,
+        data_fields=HEADERS,
         transform_func=_morph)
     c_state = OAIRecordCriteriaState('ocr_skip')
     c_from = OAIRecordCriteriaDatetime(dt_from='2021-08-03_15:03:56')
 
     # pre-check
     record1 = handler.next_record()
     assert record1[F_IDENTIFIER].endswith('9510508')
@@ -799,64 +808,64 @@
 
 def test_record_state_list_rewind_state_upload(oai_record_list):
     """Behavior for changing state"""
 
     # arrange
     handler = OAIRecordHandler(
         oai_record_list,
-        data_fields=headers,
+        data_fields=HEADERS,
         transform_func=_morph)
     c_state = OAIRecordCriteriaState('upload_done')
 
     # pre-check
     record1 = handler.next_record()
     assert record1[F_IDENTIFIER].endswith('9510508')
 
     # act
     handler.states(criterias=[c_state], dry_run=False)
     assert handler.next_record()[F_IDENTIFIER].endswith('17320046')
 
     # assert next open record changed
     h2 = OAIRecordHandler(
-        oai_record_list, data_fields=headers, transform_func=_morph)
+        oai_record_list, data_fields=HEADERS, transform_func=_morph)
     assert h2.next_record()[F_IDENTIFIER].endswith('17320046')
 
 
 def test_record_set_some_other_state(oai_record_list):
     """Behavior for changing state"""
 
     # arrange
     handler = OAIRecordHandler(
         oai_record_list,
-        data_fields=headers,
+        data_fields=HEADERS,
         transform_func=_morph)
     c_state = OAIRecordCriteriaState('upload_done')
 
     # pre-check
     record1 = handler.next_record()
     assert record1[F_IDENTIFIER].endswith('9510508')
 
     # act
     handler.states(
         criterias=[c_state], set_state='metadata_read', dry_run=False)
     assert not handler.next_record(state='upload_done')
 
     # assert next open record changed
     h2 = OAIRecordHandler(
-        oai_record_list, data_fields=headers, transform_func=_morph)
+        oai_record_list, data_fields=HEADERS, transform_func=_morph)
     assert h2.next_record(state='metadata_read')[F_IDENTIFIER].endswith('17320046')
 
 
 def test_record_list_time_range(oai_record_list):
     """Behavior for setting state within time range"""
 
     # arrange
     handler = OAIRecordHandler(
         oai_record_list,
-        data_fields=headers,
+        data_fields=HEADERS,
         transform_func=_morph)
     c_state = OAIRecordCriteriaState('ocr_skip')
     c_range = OAIRecordCriteriaDatetime(dt_from='2021-08-03_15:10:00',
                                         dt_to='2021-08-03_15:20:00')
 
     # pre-check
     record1 = handler.next_record()
@@ -886,15 +895,15 @@
     data2 = [
         "oai:digitale.bibliothek.uni-halle.de/zd:8853012\t2015-08-25T20:00:35Z\tinfo1\tupload_done\t2021-08-03_15:14:45\n",
         "oai:digitale.bibliothek.uni-halle.de/zd:9510507\t2015-08-25T20:00:35Z\tinfo2\tocr_fail\t2021-08-03_16:14:45\n"
     ]
     _write_datalist(path_oai_list2, data2, OAI_LIST_HEADER)
     handler = OAIRecordHandler(
         path_oai_list1,
-        data_fields=headers,
+        data_fields=HEADERS,
         transform_func=_morph)
 
     # assert original next == first record with identifier 8853012
     assert handler.next_record()[F_IDENTIFIER].endswith('8853012')
 
     # act
     merge_result = handler.merges(path_oai_list2, dry_run=False)
@@ -930,15 +939,15 @@
     data2 = [
         "oai:digitale.bibliothek.uni-halle.de/zd:8853012\t2015-08-25T20:00:35Z\tinfo1\tupload_done\t2021-08-03_15:14:45\n",
         "oai:digitale.bibliothek.uni-halle.de/zd:9510507\t2015-08-25T20:00:35Z\tinfo2\tocr_fail\t2021-08-03_16:14:45\n"
     ]
     _write_datalist(path_oai_list2, data2, OAI_LIST_HEADER)
     handler = OAIRecordHandler(
         path_oai_list1,
-        data_fields=headers,
+        data_fields=HEADERS,
         transform_func=_morph)
 
     # act
     merge_result = handler.merges(path_oai_list2, dry_run=False, other_require_state='upload_done')
 
     # list1 and list2 contain same records
     assert merge_result['matches'] == 2
@@ -971,15 +980,15 @@
     data2 = [
         "oai:digitale.bibliothek.uni-halle.de/zd:8853012\t2015-08-25T20:00:35Z\tinfo1\tupload_done\t2021-08-03_15:14:45\n",
         "oai:digitale.bibliothek.uni-halle.de/zd:9510507\t2015-08-25T20:00:35Z\tinfo2\tocr_fail\t2021-08-03_16:14:45\n"
     ]
     _write_datalist(path_oai_list2, data2, OAI_LIST_HEADER)
     handler = OAIRecordHandler(
         path_oai_list1,
-        data_fields=headers,
+        data_fields=HEADERS,
         transform_func=_morph)
 
     # act
     merge_result = handler.merges(path_oai_list2, dry_run=False, other_ignore_state='upload_done')
 
     # list1 and list2 contain same records
     assert merge_result['matches'] == 2
@@ -1006,15 +1015,15 @@
     path_oai_list_a = tmp_path / 'oai_list_a'
     data = [
         "oai:digitale.bibliothek.uni-halle.de/zd:8853012\t2015-08-25T20:00:35Z\tinfo1\tupload_done\t2021-08-03_15:14:45\n"
     ]
     _write_datalist(path_oai_list_a, data, OAI_LIST_HEADER)
     handler = OAIRecordHandler(
         path_oai_list_a,
-        data_fields=headers,
+        data_fields=HEADERS,
         transform_func=_morph)
     path_oai_list_b = tmp_path / 'oai_list_b'
     data = [
         "oai:digitale.bibliothek.uni-halle.de/zd:8853012\t2015-08-25T20:00:35Z\tn.a.\tn.a.\tn.a.\n",
         "oai:digitale.bibliothek.uni-halle.de/zd:8853013\t2015-08-25T20:00:35Z\tn.a.\tn.a.\tn.a.\n"
     ]
     _write_datalist(path_oai_list_b, data, OAI_LIST_HEADER)
@@ -1050,15 +1059,15 @@
     path_oai_list_a = tmp_path / 'oai_list_a'
     data1 = [
         "oai:digitale.bibliothek.uni-halle.de/zd:8853012\t2015-08-25T20:00:35Z\tinfo1\tupload_done\t2021-08-03_15:14:45\n"
     ]
     _write_datalist(path_oai_list_a, data1, OAI_LIST_HEADER)
     handler = OAIRecordHandler(
         path_oai_list_a,
-        data_fields=headers,
+        data_fields=HEADERS,
         transform_func=_morph)
     path_oai_list_b = tmp_path / 'oai_list_b'
     data2 = [
         "oai:digitale.bibliothek.uni-halle.de/zd:8853012\t2015-08-25T20:00:35Z\tn.a.\tn.a.\tn.a.\n",
         "oai:digitale.bibliothek.uni-halle.de/zd:8853013\t2015-08-25T20:00:35Z\tn.a.\tn.a.\tn.a.\n"
     ]
     _write_datalist(path_oai_list_b, data2, OAI_LIST_HEADER)
@@ -1093,15 +1102,15 @@
     path_oai_list_a = tmp_path / 'oai_list_a'
     data1 = [
         "oai:digitale.bibliothek.uni-halle.de/zd:8853012\t2015-08-25T20:00:35Z\tinfo1\tupload_done\t2021-08-03_15:14:45\n"
     ]
     _write_datalist(path_oai_list_a, data1, OAI_LIST_HEADER)
     handler = OAIRecordHandler(
         path_oai_list_a,
-        data_fields=headers,
+        data_fields=HEADERS,
         transform_func=_morph)
     path_oai_list_b = tmp_path / 'oai_list_b'
     data2 = [
         "oai:digitale.bibliothek.uni-halle.de/zd:8853013\t2015-08-25T20:00:35Z\tn.a.\tn.a.\tn.a.\n"
         "oai:digitale.bibliothek.uni-halle.de/zd:8853012\t2015-08-25T20:00:35Z\tn.a.\tn.a.\tn.a.\n",
     ]
     _write_datalist(path_oai_list_b, data2, OAI_LIST_HEADER)
@@ -1144,15 +1153,15 @@
     data2 = [
         "oai:digitale.bibliothek.uni-halle.de/zd:8853012\t2015-08-25T20:00:35Z\tn.a.\tn.a.\tn.a.\n",
         "oai:digitale.bibliothek.uni-halle.de/zd:8853013\t2015-08-25T20:00:35Z\tinfo2\tocr_fail\t2021-08-03_16:14:45\n"
     ]
     _write_datalist(path_oai_list2, data2, OAI_LIST_HEADER)
     handler = OAIRecordHandler(
         path_oai_list1,
-        data_fields=headers,
+        data_fields=HEADERS,
         transform_func=_morph)
 
     # assert original next == first record with identifier 8853012
     assert handler.next_record()[F_IDENTIFIER].endswith('8853013')
 
     # act
     results = handler.merges(path_oai_list2, dry_run=False)
@@ -1161,66 +1170,70 @@
     assert results['merges'] == 1  # because info got merged from 2 record
     assert results['ignores'] == 1  # nothing missed, because all idents present
     assert not results['appendeds']  # no new, because all idents present
     assert not handler.next_record(state='n.a.')    # by now no more open records
 
 
 def test_records_frame_with_start(oai_record_list):
+    """Behavior for framing results with 
+    explicite start value"""
 
     # arrange
     handler = OAIRecordHandler(
         oai_record_list,
-        data_fields=headers,
+        data_fields=HEADERS,
         transform_func=_morph)
 
     # act
     new_path = handler.frame(2)
 
     # assert
     assert os.path.exists(new_path)
     assert os.path.basename(new_path) == 'ocr_list_02_06.csv'
 
     frame_handler = OAIRecordHandler(
         new_path,
-        data_fields=headers,
+        data_fields=HEADERS,
         transform_func=_morph)
 
     # ensure that only first records is set to 'other_load'
     # all other records are within frame
     c_state = OAIRecordCriteriaState('other_load')
     assert frame_handler.states([c_state]) == 1
 
 
 def test_records_frame_range(oai_record_list):
+    """Test framing from-too in range"""
 
     # arrange
     handler = OAIRecordHandler(
         oai_record_list,
-        data_fields=headers,
+        data_fields=HEADERS,
         transform_func=_morph)
 
     # act
     new_path = handler.frame(2, 2)
 
     # assert
     assert os.path.exists(new_path)
     assert os.path.basename(new_path) == 'ocr_list_02_03.csv'
 
     frame_handler = OAIRecordHandler(
         new_path,
-        data_fields=headers,
+        data_fields=HEADERS,
         transform_func=_morph)
 
     # ensure that by now 4 records are set to 'other_load'
     # first record and records 4,5,6
     c_state = OAIRecordCriteriaState('other_load')
     assert frame_handler.states([c_state]) == 4
 
 
 def test_records_default_header_from_file(oai_record_list):
+    """Ensure proper range has been selected"""
 
     # arrange
     handler = OAIRecordHandler(
         oai_record_list,
         transform_func=_morph)
 
     # act
@@ -1276,27 +1289,28 @@
 
 @mock.patch('requests.get')
 def test_response_200_with_error_content(mock_requests):
     """test request results into OAILoadException"""
 
     # arrange
     data_path = os.path.join(str(ROOT), 'tests/resources/opendata/id_not_exist.xml')
-    _req = mock_response(status_code=200, 
-                         headers= {'Content-Type': 'text/xml;charset=UTF-8'},
+    _req = mock_response(status_code=200,
+                         headers={'Content-Type': 'text/xml;charset=UTF-8'},
                          data_path=data_path)
     mock_requests.return_value = _req
 
     # act
     with pytest.raises(OAILoadException) as exc:
         request_resource('http://foo.bar', Path())
 
     assert 'verb requires' in str(exc.value)
 
 
 def test_records_sample_zd1_post_ocr():
+    """Ensure proper state recognized"""
 
     path_list = os.path.join(str(ROOT), 'tests', 'resources',
                              'vls', 'oai-urn-zd1-sample70k.tsv')
     assert os.path.isfile(path_list)
 
     # arrange
     handler = OAIRecordHandler(
@@ -1378,15 +1392,15 @@
     # arrange
     path_list_sample = os.path.join(TEST_RES, 'oai-records-opendata-vd18-sample-broken.csv')
     path_oai_list1 = tmp_path / 'oai-list.csv'
     shutil.copy(path_list_sample, path_oai_list1)
     handler = OAIRecordHandler(path_oai_list1, transform_func=transform_to_record)
 
     # act
-    _next_rec = handler.next_record(state='ocr_fail')    
+    _next_rec = handler.next_record(state='ocr_fail')
     assert _next_rec.info.startswith('141.48.10.202@2023-01-17_15:55:49')
     with pytest.raises(JSONDecodeError) as _decode_err:
         json.loads(_next_rec.info)
     assert 'Extra data: line 1 column 7 (char 6)' in _decode_err.value.args[0]
 
 
 def test_record_handler_quotation_mixture_json(tmp_path):
@@ -1401,20 +1415,21 @@
     # arrange
     path_list_sample = os.path.join(TEST_RES, 'oai-records-opendata-vd18-sample-mixture.csv')
     path_oai_list1 = tmp_path / 'oai-list.csv'
     shutil.copy(path_list_sample, path_oai_list1)
     handler = OAIRecordHandler(path_oai_list1, transform_func=transform_to_record)
 
     # act
-    _next_rec = handler.next_record(state='ocr_fail')    
+    _next_rec = handler.next_record(state='ocr_fail')
     assert _next_rec.info.startswith('141.48.10.202@2023-01-17_15:55:49')
     with pytest.raises(JSONDecodeError) as _decode_err:
         json.loads(_next_rec.info)
     assert 'Extra data: line 1 column 7 (char 6)' in _decode_err.value.args[0]
 
+
 def test_record_handler_quotation_fixed_json(tmp_path):
     """
     Fix behavior when encountering data which
     has been fixed manually resulting in a mixture
     of double and single quotes
 
     originates from ODEM project csv list
@@ -1423,15 +1438,15 @@
     # arrange
     path_list_sample = os.path.join(TEST_RES, 'oai-records-opendata-vd18-sample-fixed.csv')
     path_oai_list1 = tmp_path / 'oai-list.csv'
     shutil.copy(path_list_sample, path_oai_list1)
     handler = OAIRecordHandler(path_oai_list1, transform_func=transform_to_record)
 
     # act
-    _next_rec = handler.next_record(state='ocr_fail')    
+    _next_rec = handler.next_record(state='ocr_fail')
     assert _next_rec.info.startswith('141.48.10.202@2023-01-17_15:55:49')
     _info_token = get_enclosed(_next_rec.info)
     _last_info = json.loads(_info_token)['info']
     assert 'processing https://opendata.uni-halle.de/retrieve/b7f7f81d-e65f-4c7d-95c6-7384b184c6a9/00001051.jpg' in _last_info
 
 
 def test_record_handler_quotation_fixed_ast(tmp_path):
@@ -1446,15 +1461,15 @@
     # arrange
     path_list_sample = os.path.join(TEST_RES, 'oai-records-opendata-vd18-sample-fixed.csv')
     path_oai_list1 = tmp_path / 'oai-list.csv'
     shutil.copy(path_list_sample, path_oai_list1)
     handler = OAIRecordHandler(path_oai_list1, transform_func=transform_to_record)
 
     # act
-    _next_rec = handler.next_record(state='ocr_fail')    
+    _next_rec = handler.next_record(state='ocr_fail')
     assert _next_rec.info.startswith('141.48.10.202@2023-01-17_15:55:49')
     _info_token = get_enclosed(_next_rec.info)
     _last_info = ast.literal_eval(_info_token)['info']
     assert 'processing https://opendata.uni-halle.de/retrieve/b7f7f81d-e65f-4c7d-95c6-7384b184c6a9/00001051.jpg' in _last_info
 
 
 def test_record_handler_quotation_mixture_ast(tmp_path):
@@ -1473,22 +1488,22 @@
     # arrange
     path_list_sample = os.path.join(TEST_RES, 'oai-records-opendata-vd18-sample-mixture.csv')
     path_oai_list1 = tmp_path / 'oai-list.csv'
     shutil.copy(path_list_sample, path_oai_list1)
     handler = OAIRecordHandler(path_oai_list1, transform_func=transform_to_record)
 
     # act
-    _next_rec = handler.next_record(state='ocr_fail')    
+    _next_rec = handler.next_record(state='ocr_fail')
     assert _next_rec.info.startswith('141.48.10.202@2023-01-17_15:55:49')
     _info_token = get_enclosed(_next_rec.info)
     _last_info = ast.literal_eval(_info_token)['info']
     assert "processing 'https://opendata.uni-halle.de/retrieve/b7f7f81d-e65f-4c7d-95c6-7384b184c6a9/00001051.jpg'" in _last_info
 
 
-@pytest.mark.skipif(sys.version_info >= (3,10), reason="Specific to Python <3.10")
+@pytest.mark.skipif(sys.version_info >= (3, 10), reason="Specific to Python <3.10")
 def test_record_handler_quotation_mixture_ast_639763(tmp_path):
     """
     Behavior when encountering data like this:
 
     originates from ODEM project csv list
 
     Please note: changed from python 3.8 to 3.10
@@ -1498,22 +1513,22 @@
     # arrange
     path_list_sample = os.path.join(TEST_RES, 'oai-records-opendata-vd18-sample-mixture.csv')
     path_oai_list1 = tmp_path / 'oai-list.csv'
     shutil.copy(path_list_sample, path_oai_list1)
     handler = OAIRecordHandler(path_oai_list1, transform_func=transform_to_record)
 
     # act
-    _next_rec = handler.next_record(state='ocr_busy')    
+    _next_rec = handler.next_record(state='ocr_busy')
     _info_token = get_enclosed(_next_rec.info)
     with pytest.raises(SyntaxError) as _decode_err:
         ast.literal_eval(_info_token)
     assert 'invalid syntax' in _decode_err.value.args[0]
 
 
-@pytest.mark.skipif(sys.version_info < (3,10), 
+@pytest.mark.skipif(sys.version_info < (3, 10),
                     reason="Specific to Python >= 3.10")
 def test_record_handler_quotation_mixture_ast_639763_python_310(tmp_path):
     """
     Behavior when encountering data like this:
 
     originates from ODEM project csv list
 
@@ -1524,27 +1539,27 @@
     # arrange
     path_list_sample = os.path.join(TEST_RES, 'oai-records-opendata-vd18-sample-mixture.csv')
     path_oai_list1 = tmp_path / 'oai-list.csv'
     shutil.copy(path_list_sample, path_oai_list1)
     handler = OAIRecordHandler(path_oai_list1, transform_func=transform_to_record)
 
     # act
-    _next_rec = handler.next_record(state='ocr_busy')    
+    _next_rec = handler.next_record(state='ocr_busy')
     _info_token = get_enclosed(_next_rec.info)
     with pytest.raises(SyntaxError) as _decode_err:
         ast.literal_eval(_info_token)
     assert "unmatched '}'" in _decode_err.value.args[0]
 
 
 @mock.patch('requests.get')
 def test_oai_load_exception_for_server_error(mock_504, tmp_path):
     """Ensure OAILoadException for Response status_code
     which indicates internal Server-Errors gets properly
     propagated upstream to caller.
-    
+
     Because we're testing the very response status_code,
     any subsequent steps that usually require additional
     information for parsing the response content (like
     prime id) are not needed and thereforse just set
     with dummy identifier 'foo'
     """
```

### Comparing `digiflow-3.9.1/tests/test_digiflow_metadata.py` & `digiflow-3.9.2/tests/test_digiflow_metadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -782,7 +782,24 @@
     mets = os.path.join(TEST_RES, 'k2_mets_mena_12988274719564.xml')
 
     # act
     mets_reader = MetsReader(mets)
 
     # assert
     assert mets_reader.dmd_id == 'DMDLOG_0001'
+
+
+def test_metadata_processor_contains_single_fgroup():
+    """Ensure behavior for passing single str arg
+    Bugfix: 
+    TypeError: '>' not supported between instances of 'list' and 'int'
+    """
+
+    _proc = MetsProcessor(TEST_RES / 'k2_mets_morbio_1748529021.xml')
+    assert _proc.contains_group('MAX')
+
+
+def test_metadata_processor_contains_multiple_fgroup():
+    """Ensure behavior for passing list args"""
+
+    _proc = MetsProcessor(TEST_RES / 'k2_mets_morbio_1748529021.xml')
+    assert _proc.contains_group(['MAX'])
```

### Comparing `digiflow-3.9.1/tests/test_digiflow_metadata_transform.py` & `digiflow-3.9.2/tests/test_digiflow_metadata_transform.py`

 * *Files identical despite different names*

### Comparing `digiflow-3.9.1/tests/test_digiflow_validate_mets.py` & `digiflow-3.9.2/tests/test_digiflow_validate_mets.py`

 * *Files identical despite different names*

### Comparing `digiflow-3.9.1/tests/test_export_saf.py` & `digiflow-3.9.2/tests/test_export_saf.py`

 * *Files identical despite different names*

### Comparing `digiflow-3.9.1/tests/test_validate_fsdata.py` & `digiflow-3.9.2/tests/test_validate_fsdata.py`

 * *Files identical despite different names*

### Comparing `digiflow-3.9.1/tests/test_validate_imgdata.py` & `digiflow-3.9.2/tests/test_validate_imgdata.py`

 * *Files identical despite different names*

