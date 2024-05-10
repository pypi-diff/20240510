# Comparing `tmp/pyDataverse-0.3.1.tar.gz` & `tmp/pydataverse-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyDataverse-0.3.1.tar", last modified: Tue Apr  6 11:53:35 2021, max compression
+gzip compressed data, was "pydataverse-0.3.2.tar", max compression
```

## Comparing `pyDataverse-0.3.1.tar` & `pydataverse-0.3.2.tar`

### file list

```diff
@@ -1,27 +1,37 @@
-drwxrwxr-x   0 cheeseman  (1000) cheeseman  (1000)        0 2021-04-06 11:53:35.000000 pyDataverse-0.3.1/
--rw-rw-r--   0 cheeseman  (1000) cheeseman  (1000)       44 2021-01-27 01:07:36.000000 pyDataverse-0.3.1/MANIFEST.in
--rw-rw-r--   0 cheeseman  (1000) cheeseman  (1000)     1112 2021-01-27 01:07:36.000000 pyDataverse-0.3.1/LICENSE.txt
--rw-rw-r--   0 cheeseman  (1000) cheeseman  (1000)      448 2021-04-06 11:53:35.000000 pyDataverse-0.3.1/setup.cfg
--rw-rw-r--   0 cheeseman  (1000) cheeseman  (1000)     3119 2021-02-25 20:56:47.000000 pyDataverse-0.3.1/setup.py
--rw-rw-r--   0 cheeseman  (1000) cheeseman  (1000)     1255 2021-04-06 11:50:15.000000 pyDataverse-0.3.1/README.md
-drwxrwxr-x   0 cheeseman  (1000) cheeseman  (1000)        0 2021-04-06 11:53:35.000000 pyDataverse-0.3.1/src/
-drwxrwxr-x   0 cheeseman  (1000) cheeseman  (1000)        0 2021-04-06 11:53:35.000000 pyDataverse-0.3.1/src/pyDataverse.egg-info/
--rw-rw-r--   0 cheeseman  (1000) cheeseman  (1000)        1 2021-01-27 02:01:54.000000 pyDataverse-0.3.1/src/pyDataverse.egg-info/not-zip-safe
--rw-rw-r--   0 cheeseman  (1000) cheeseman  (1000)        1 2021-04-06 11:53:35.000000 pyDataverse-0.3.1/src/pyDataverse.egg-info/dependency_links.txt
--rw-rw-r--   0 cheeseman  (1000) cheeseman  (1000)       12 2021-04-06 11:53:35.000000 pyDataverse-0.3.1/src/pyDataverse.egg-info/top_level.txt
--rw-rw-r--   0 cheeseman  (1000) cheeseman  (1000)      643 2021-04-06 11:53:35.000000 pyDataverse-0.3.1/src/pyDataverse.egg-info/SOURCES.txt
--rw-rw-r--   0 cheeseman  (1000) cheeseman  (1000)       35 2021-04-06 11:53:35.000000 pyDataverse-0.3.1/src/pyDataverse.egg-info/requires.txt
--rw-rw-r--   0 cheeseman  (1000) cheeseman  (1000)     2355 2021-04-06 11:53:35.000000 pyDataverse-0.3.1/src/pyDataverse.egg-info/PKG-INFO
-drwxrwxr-x   0 cheeseman  (1000) cheeseman  (1000)        0 2021-04-06 11:53:35.000000 pyDataverse-0.3.1/src/pyDataverse/
-drwxrwxr-x   0 cheeseman  (1000) cheeseman  (1000)        0 2021-04-06 11:53:35.000000 pyDataverse-0.3.1/src/pyDataverse/schemas/
-drwxrwxr-x   0 cheeseman  (1000) cheeseman  (1000)        0 2021-04-06 11:53:35.000000 pyDataverse-0.3.1/src/pyDataverse/schemas/json/
--rw-rw-r--   0 cheeseman  (1000) cheeseman  (1000)     1289 2021-01-27 01:07:36.000000 pyDataverse-0.3.1/src/pyDataverse/schemas/json/datafile_upload_schema.json
--rw-rw-r--   0 cheeseman  (1000) cheeseman  (1000)     1577 2021-01-27 01:07:36.000000 pyDataverse-0.3.1/src/pyDataverse/schemas/json/dataverse_upload_schema.json
--rw-rw-r--   0 cheeseman  (1000) cheeseman  (1000)    29903 2021-01-27 01:07:36.000000 pyDataverse-0.3.1/src/pyDataverse/schemas/json/dataset_upload_default_schema.json
--rw-rw-r--   0 cheeseman  (1000) cheeseman  (1000)     8840 2021-01-27 01:07:36.000000 pyDataverse-0.3.1/src/pyDataverse/schemas/json/dspace_schema.json
--rw-rw-r--   0 cheeseman  (1000) cheeseman  (1000)    59600 2021-04-06 11:34:36.000000 pyDataverse-0.3.1/src/pyDataverse/models.py
--rw-rw-r--   0 cheeseman  (1000) cheeseman  (1000)    17795 2021-04-06 08:03:27.000000 pyDataverse-0.3.1/src/pyDataverse/utils.py
--rw-rw-r--   0 cheeseman  (1000) cheeseman  (1000)      583 2021-04-06 11:34:36.000000 pyDataverse-0.3.1/src/pyDataverse/__init__.py
--rw-rw-r--   0 cheeseman  (1000) cheeseman  (1000)    81424 2021-04-06 10:56:45.000000 pyDataverse-0.3.1/src/pyDataverse/api.py
--rw-rw-r--   0 cheeseman  (1000) cheeseman  (1000)     1196 2021-01-27 01:07:36.000000 pyDataverse-0.3.1/src/pyDataverse/exceptions.py
--rw-rw-r--   0 cheeseman  (1000) cheeseman  (1000)     2355 2021-04-06 11:53:35.000000 pyDataverse-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1112 2024-05-10 16:01:48.624027 pydataverse-0.3.2/LICENSE.txt
+-rw-r--r--   0        0        0     3544 2024-05-10 16:01:48.624027 pydataverse-0.3.2/README.md
+-rw-r--r--   0        0        0      510 2024-05-10 16:01:48.624027 pydataverse-0.3.2/pyDataverse/__init__.py
+-rw-r--r--   0        0        0    84753 2024-05-10 16:01:48.624027 pydataverse-0.3.2/pyDataverse/api.py
+-rw-r--r--   0        0        0    34961 2024-05-10 16:01:48.624027 pydataverse-0.3.2/pyDataverse/docs/source/_images/collection_dataset.png
+-rw-r--r--   0        0        0        0 2024-05-10 16:01:48.624027 pydataverse-0.3.2/pyDataverse/docs/source/_static/.gitkeep
+-rw-r--r--   0        0        0      712 2024-05-10 16:01:48.624027 pydataverse-0.3.2/pyDataverse/docs/source/_templates/layout.html
+-rw-r--r--   0        0        0     1040 2024-05-10 16:01:48.624027 pydataverse-0.3.2/pyDataverse/docs/source/_templates/sidebar_intro.html
+-rw-r--r--   0        0        0      366 2024-05-10 16:01:48.624027 pydataverse-0.3.2/pyDataverse/docs/source/_templates/sidebar_related-links.html
+-rw-r--r--   0        0        0      673 2024-05-10 16:01:48.624027 pydataverse-0.3.2/pyDataverse/docs/source/community/contact.rst
+-rw-r--r--   0        0        0      109 2024-05-10 16:01:48.624027 pydataverse-0.3.2/pyDataverse/docs/source/community/releases.rst
+-rw-r--r--   0        0        0     6280 2024-05-10 16:01:48.624027 pydataverse-0.3.2/pyDataverse/docs/source/conf.py
+-rw-r--r--   0        0        0       77 2024-05-10 16:01:48.624027 pydataverse-0.3.2/pyDataverse/docs/source/contributing/contributing.rst
+-rw-r--r--   0        0        0     7972 2024-05-10 16:01:48.624027 pydataverse-0.3.2/pyDataverse/docs/source/index.rst
+-rw-r--r--   0        0        0      936 2024-05-10 16:01:48.624027 pydataverse-0.3.2/pyDataverse/docs/source/reference.rst
+-rw-r--r--   0        0        0       54 2024-05-10 16:01:48.624027 pydataverse-0.3.2/pyDataverse/docs/source/snippets/pip-install.rst
+-rw-r--r--   0        0        0      336 2024-05-10 16:01:48.624027 pydataverse-0.3.2/pyDataverse/docs/source/snippets/requirements.rst
+-rw-r--r--   0        0        0      103 2024-05-10 16:01:48.624027 pydataverse-0.3.2/pyDataverse/docs/source/snippets/warning_production.rst
+-rw-r--r--   0        0        0     7437 2024-05-10 16:01:48.624027 pydataverse-0.3.2/pyDataverse/docs/source/user/advanced-usage.rst
+-rw-r--r--   0        0        0    16978 2024-05-10 16:01:48.624027 pydataverse-0.3.2/pyDataverse/docs/source/user/basic-usage.rst
+-rw-r--r--   0        0        0     6901 2024-05-10 16:01:48.624027 pydataverse-0.3.2/pyDataverse/docs/source/user/csv-templates.rst
+-rw-r--r--   0        0        0     1607 2024-05-10 16:01:48.624027 pydataverse-0.3.2/pyDataverse/docs/source/user/faq.rst
+-rw-r--r--   0        0        0     1790 2024-05-10 16:01:48.624027 pydataverse-0.3.2/pyDataverse/docs/source/user/installation.rst
+-rw-r--r--   0        0        0     1265 2024-05-10 16:01:48.624027 pydataverse-0.3.2/pyDataverse/docs/source/user/resources.rst
+-rw-r--r--   0        0        0     4030 2024-05-10 16:01:48.624027 pydataverse-0.3.2/pyDataverse/docs/source/user/use-cases.rst
+-rw-r--r--   0        0        0     1196 2024-05-10 16:01:48.624027 pydataverse-0.3.2/pyDataverse/exceptions.py
+-rw-r--r--   0        0        0    59774 2024-05-10 16:01:48.624027 pydataverse-0.3.2/pyDataverse/models.py
+-rw-r--r--   0        0        0     1289 2024-05-10 16:01:48.624027 pydataverse-0.3.2/pyDataverse/schemas/json/datafile_upload_schema.json
+-rw-r--r--   0        0        0    29903 2024-05-10 16:01:48.624027 pydataverse-0.3.2/pyDataverse/schemas/json/dataset_upload_default_schema.json
+-rw-r--r--   0        0        0     1577 2024-05-10 16:01:48.624027 pydataverse-0.3.2/pyDataverse/schemas/json/dataverse_upload_schema.json
+-rw-r--r--   0        0        0     8840 2024-05-10 16:01:48.624027 pydataverse-0.3.2/pyDataverse/schemas/json/dspace_schema.json
+-rw-r--r--   0        0        0     1379 2024-05-10 16:01:48.624027 pydataverse-0.3.2/pyDataverse/templates/datafiles.csv
+-rw-r--r--   0        0        0     9592 2024-05-10 16:01:48.628027 pydataverse-0.3.2/pyDataverse/templates/datasets.csv
+-rw-r--r--   0        0        0     1569 2024-05-10 16:01:48.628027 pydataverse-0.3.2/pyDataverse/templates/dataverses.csv
+-rw-r--r--   0        0        0    17804 2024-05-10 16:01:48.628027 pydataverse-0.3.2/pyDataverse/utils.py
+-rw-r--r--   0        0        0     1918 2024-05-10 16:01:48.628027 pydataverse-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     4290 1970-01-01 00:00:00.000000 pydataverse-0.3.2/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyDataverse-0.3.1/LICENSE.txt` & `pydataverse-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyDataverse-0.3.1/src/pyDataverse/schemas/json/datafile_upload_schema.json` & `pydataverse-0.3.2/pyDataverse/schemas/json/datafile_upload_schema.json`

 * *Files identical despite different names*

### Comparing `pyDataverse-0.3.1/src/pyDataverse/schemas/json/dataverse_upload_schema.json` & `pydataverse-0.3.2/pyDataverse/schemas/json/dataverse_upload_schema.json`

 * *Files identical despite different names*

### Comparing `pyDataverse-0.3.1/src/pyDataverse/schemas/json/dataset_upload_default_schema.json` & `pydataverse-0.3.2/pyDataverse/schemas/json/dataset_upload_default_schema.json`

 * *Files identical despite different names*

### Comparing `pyDataverse-0.3.1/src/pyDataverse/schemas/json/dspace_schema.json` & `pydataverse-0.3.2/pyDataverse/schemas/json/dspace_schema.json`

 * *Files identical despite different names*

### Comparing `pyDataverse-0.3.1/src/pyDataverse/models.py` & `pydataverse-0.3.2/pyDataverse/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Dataverse data-types data model."""
+
 from __future__ import absolute_import
 
 import json
 import os
 
 from pyDataverse.utils import validate_data
 
@@ -99,15 +100,17 @@
             filename_schema = os.path.join(
                 os.path.dirname(os.path.realpath(__file__)),
                 self._default_json_schema_filename,
             )
         assert isinstance(filename_schema, str)
 
         return validate_data(
-            json.loads(self.json(validate=False)), filename_schema, file_format="json",
+            json.loads(self.json(validate=False)),
+            filename_schema,
+            file_format="json",
         )
 
     def from_json(
         self, json_str, data_format=None, validate=True, filename_schema=None
     ):
         """Import metadata from a JSON file.
 
@@ -863,15 +866,14 @@
                         print(
                             "Attribute {0} not valid for import (format={1}).".format(
                                 key, data_format
                             )
                         )
 
             if "metadataBlocks" in json_dict["datasetVersion"]:
-
                 # citation
                 if "citation" in json_dict["datasetVersion"]["metadataBlocks"]:
                     citation = json_dict["datasetVersion"]["metadataBlocks"]["citation"]
                     if "displayName" in citation:
                         data["citation_displayName"] = citation["displayName"]
 
                     for field in citation["fields"]:
@@ -950,47 +952,48 @@
                 if "socialscience" in json_dict["datasetVersion"]["metadataBlocks"]:
                     socialscience = json_dict["datasetVersion"]["metadataBlocks"][
                         "socialscience"
                     ]
 
                     if "displayName" in socialscience:
                         self.__setattr__(
-                            "socialscience_displayName", socialscience["displayName"],
+                            "socialscience_displayName",
+                            socialscience["displayName"],
                         )
 
                     for field in socialscience["fields"]:
                         if (
                             field["typeName"]
                             in self.__attr_import_dv_up_socialscience_fields_values
                         ):
                             data[field["typeName"]] = field["value"]
                         elif field["typeName"] == "targetSampleSize":
                             data["targetSampleSize"] = {}
                             if "targetSampleActualSize" in field["value"]:
-                                data["targetSampleSize"][
-                                    "targetSampleActualSize"
-                                ] = field["value"]["targetSampleActualSize"]["value"]
+                                data["targetSampleSize"]["targetSampleActualSize"] = (
+                                    field["value"]["targetSampleActualSize"]["value"]
+                                )
                             if "targetSampleSizeFormula" in field["value"]:
-                                data["targetSampleSize"][
-                                    "targetSampleSizeFormula"
-                                ] = field["value"]["targetSampleSizeFormula"]["value"]
+                                data["targetSampleSize"]["targetSampleSizeFormula"] = (
+                                    field["value"]["targetSampleSizeFormula"]["value"]
+                                )
                         elif field["typeName"] == "socialScienceNotes":
                             data["socialScienceNotes"] = {}
                             if "socialScienceNotesType" in field["value"]:
-                                data["socialScienceNotes"][
-                                    "socialScienceNotesType"
-                                ] = field["value"]["socialScienceNotesType"]["value"]
+                                data["socialScienceNotes"]["socialScienceNotesType"] = (
+                                    field["value"]["socialScienceNotesType"]["value"]
+                                )
                             if "socialScienceNotesSubject" in field["value"]:
                                 data["socialScienceNotes"][
                                     "socialScienceNotesSubject"
                                 ] = field["value"]["socialScienceNotesSubject"]["value"]
                             if "socialScienceNotesText" in field["value"]:
-                                data["socialScienceNotes"][
-                                    "socialScienceNotesText"
-                                ] = field["value"]["socialScienceNotesText"]["value"]
+                                data["socialScienceNotes"]["socialScienceNotesText"] = (
+                                    field["value"]["socialScienceNotesText"]["value"]
+                                )
                         else:
                             print(
                                 "Attribute {0} not valid for import (dv_up).".format(
                                     field["typeName"]
                                 )
                             )
                 else:
@@ -1196,15 +1199,18 @@
                             "multiple": multiple,
                             "typeClass": type_class,
                             "value": v,
                         }
                     )
 
             # Generate fields attributes
-            for (key, val,) in self.__attr_import_dv_up_citation_fields_arrays.items():
+            for (
+                key,
+                val,
+            ) in self.__attr_import_dv_up_citation_fields_arrays.items():
                 if key in data_dict:
                     v = data_dict[key]
                     citation["fields"].append(
                         {
                             "typeName": key,
                             "multiple": True,
                             "typeClass": "compound",
@@ -1337,33 +1343,33 @@
             # Generate targetSampleSize attributes
             if "targetSampleSize" in data_dict:
                 target_sample_size = data_dict["targetSampleSize"]
                 tmp_dict = {}
                 if "targetSampleActualSize" in target_sample_size:
                     if target_sample_size["targetSampleActualSize"] is not None:
                         tmp_dict["targetSampleActualSize"] = {}
-                        tmp_dict["targetSampleActualSize"][
-                            "typeName"
-                        ] = "targetSampleActualSize"
+                        tmp_dict["targetSampleActualSize"]["typeName"] = (
+                            "targetSampleActualSize"
+                        )
                         tmp_dict["targetSampleActualSize"]["multiple"] = False
                         tmp_dict["targetSampleActualSize"]["typeClass"] = "primitive"
-                        tmp_dict["targetSampleActualSize"][
-                            "value"
-                        ] = target_sample_size["targetSampleActualSize"]
+                        tmp_dict["targetSampleActualSize"]["value"] = (
+                            target_sample_size["targetSampleActualSize"]
+                        )
                 if "targetSampleSizeFormula" in target_sample_size:
                     if target_sample_size["targetSampleSizeFormula"] is not None:
                         tmp_dict["targetSampleSizeFormula"] = {}
-                        tmp_dict["targetSampleSizeFormula"][
-                            "typeName"
-                        ] = "targetSampleSizeFormula"
+                        tmp_dict["targetSampleSizeFormula"]["typeName"] = (
+                            "targetSampleSizeFormula"
+                        )
                         tmp_dict["targetSampleSizeFormula"]["multiple"] = False
                         tmp_dict["targetSampleSizeFormula"]["typeClass"] = "primitive"
-                        tmp_dict["targetSampleSizeFormula"][
-                            "value"
-                        ] = target_sample_size["targetSampleSizeFormula"]
+                        tmp_dict["targetSampleSizeFormula"]["value"] = (
+                            target_sample_size["targetSampleSizeFormula"]
+                        )
                 socialscience["fields"].append(
                     {
                         "typeName": "targetSampleSize",
                         "multiple": False,
                         "typeClass": "compound",
                         "value": tmp_dict,
                     }
@@ -1372,44 +1378,44 @@
             # Generate socialScienceNotes attributes
             if "socialScienceNotes" in data_dict:
                 social_science_notes = data_dict["socialScienceNotes"]
                 tmp_dict = {}
                 if "socialScienceNotesType" in social_science_notes:
                     if social_science_notes["socialScienceNotesType"] is not None:
                         tmp_dict["socialScienceNotesType"] = {}
-                        tmp_dict["socialScienceNotesType"][
-                            "typeName"
-                        ] = "socialScienceNotesType"
+                        tmp_dict["socialScienceNotesType"]["typeName"] = (
+                            "socialScienceNotesType"
+                        )
                         tmp_dict["socialScienceNotesType"]["multiple"] = False
                         tmp_dict["socialScienceNotesType"]["typeClass"] = "primitive"
-                        tmp_dict["socialScienceNotesType"][
-                            "value"
-                        ] = social_science_notes["socialScienceNotesType"]
+                        tmp_dict["socialScienceNotesType"]["value"] = (
+                            social_science_notes["socialScienceNotesType"]
+                        )
                 if "socialScienceNotesSubject" in social_science_notes:
                     if social_science_notes["socialScienceNotesSubject"] is not None:
                         tmp_dict["socialScienceNotesSubject"] = {}
-                        tmp_dict["socialScienceNotesSubject"][
-                            "typeName"
-                        ] = "socialScienceNotesSubject"
+                        tmp_dict["socialScienceNotesSubject"]["typeName"] = (
+                            "socialScienceNotesSubject"
+                        )
                         tmp_dict["socialScienceNotesSubject"]["multiple"] = False
                         tmp_dict["socialScienceNotesSubject"]["typeClass"] = "primitive"
-                        tmp_dict["socialScienceNotesSubject"][
-                            "value"
-                        ] = social_science_notes["socialScienceNotesSubject"]
+                        tmp_dict["socialScienceNotesSubject"]["value"] = (
+                            social_science_notes["socialScienceNotesSubject"]
+                        )
                 if "socialScienceNotesText" in social_science_notes:
                     if social_science_notes["socialScienceNotesText"] is not None:
                         tmp_dict["socialScienceNotesText"] = {}
-                        tmp_dict["socialScienceNotesText"][
-                            "typeName"
-                        ] = "socialScienceNotesText"
+                        tmp_dict["socialScienceNotesText"]["typeName"] = (
+                            "socialScienceNotesText"
+                        )
                         tmp_dict["socialScienceNotesText"]["multiple"] = False
                         tmp_dict["socialScienceNotesText"]["typeClass"] = "primitive"
-                        tmp_dict["socialScienceNotesText"][
-                            "value"
-                        ] = social_science_notes["socialScienceNotesText"]
+                        tmp_dict["socialScienceNotesText"]["value"] = (
+                            social_science_notes["socialScienceNotesText"]
+                        )
                 socialscience["fields"].append(
                     {
                         "typeName": "socialScienceNotes",
                         "multiple": False,
                         "typeClass": "compound",
                         "value": tmp_dict,
                     }
@@ -1452,30 +1458,33 @@
                             "multiple": multiple,
                             "typeClass": type_class,
                             "value": v,
                         }
                     )
 
             # Generate fields attributes
-            for (key, val,) in self.__attr_import_dv_up_journal_fields_arrays.items():
+            for (
+                key,
+                val,
+            ) in self.__attr_import_dv_up_journal_fields_arrays.items():
                 if key in data_dict:
                     journal["fields"].append(
                         {
                             "typeName": key,
                             "multiple": True,
                             "typeClass": "compound",
                             "value": self.__generate_field_arrays(key, val),
                         }
                     )
 
             data["datasetVersion"]["metadataBlocks"]["citation"] = citation
             if "socialscience" in locals():
-                data["datasetVersion"]["metadataBlocks"][
-                    "socialscience"
-                ] = socialscience
+                data["datasetVersion"]["metadataBlocks"]["socialscience"] = (
+                    socialscience
+                )
             if "geospatial" in locals():
                 data["datasetVersion"]["metadataBlocks"]["geospatial"] = geospatial
             if "journal" in locals():
                 data["datasetVersion"]["metadataBlocks"]["journal"] = journal
         elif data_format == "dspace":
             data = None
             print("INFO: Not implemented yet.")
```

### Comparing `pyDataverse-0.3.1/src/pyDataverse/utils.py` & `pydataverse-0.3.2/pyDataverse/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Helper functions."""
+
 import csv
 import json
 import os
 import pickle
 
 from jsonschema import validate
 
@@ -581,21 +582,21 @@
     tuple
         (List of Dataverse, List of Datasets, List of Datafiles)
     """
     dataverses = []
     datasets = []
     datafiles = []
 
-    if type(data) == list:
+    if isinstance(data, list):
         for elem in data:
             dv, ds, df = dataverse_tree_walker(elem)
             dataverses += dv
             datasets += ds
             datafiles += df
-    elif type(data) == dict:
+    elif isinstance(data, dict):
         if data["type"] == "dataverse":
             dv_tmp = {}
             for key in dv_keys:
                 if key in data:
                     dv_tmp[key] = data[key]
             dataverses.append(dv_tmp)
         elif data["type"] == "dataset":
@@ -624,17 +625,17 @@
     datasets: list,
     datafiles: list,
     filename_dv: str = "dataverses.json",
     filename_ds: str = "datasets.json",
     filename_df: str = "datafiles.json",
     filename_md: str = "metadata.json",
 ) -> None:
-    """Save lists from data returend by ``dv_tree_walker``.
+    """Save lists from data returned by ``dv_tree_walker``.
 
-    Collect lists of Dataverses, Datasets and Datafiles and save them in seperated JSON files.
+    Collect lists of Dataverses, Datasets and Datafiles and save them in separated JSON files.
 
     Parameters
     ----------
     data : dict
         Tree data structure returned by ``get_children()``.
     filename_dv : str
         Filename with full path for the Dataverse JSON file.
```

### Comparing `pyDataverse-0.3.1/src/pyDataverse/api.py` & `pydataverse-0.3.2/pyDataverse/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 """Dataverse API wrapper for all it's API's."""
+
 import json
+from typing import Any, Dict, Optional
+import httpx
 import subprocess as sp
 
-from requests import ConnectionError, Response, delete, get, post, put
+from httpx import ConnectError, Response
 
 from pyDataverse.exceptions import (
     ApiAuthorizationError,
     ApiUrlError,
     DatasetNotFoundError,
     DataverseNotEmptyError,
     DataverseNotFoundError,
@@ -19,26 +22,29 @@
 
     Parameters
     ----------
         base_url : str
             Base URL of Dataverse instance. Without trailing `/` at the end.
             e.g. `http://demo.dataverse.org`
         api_token : str
-            Authenication token for the api.
+            Authentication token for the api.
 
     Attributes
     ----------
     base_url
     api_token
     dataverse_version
 
     """
 
     def __init__(
-        self, base_url: str, api_token: str = None, api_version: str = "latest"
+        self,
+        base_url: str,
+        api_token: Optional[str] = None,
+        api_version: str = "latest",
     ):
         """Init an Api() class.
 
         Scheme, host and path combined create the base-url for the api.
         See more about URL at `Wikipedia <https://en.wikipedia.org/wiki/URL>`_.
 
         Parameters
@@ -57,14 +63,15 @@
             >>> api = Api(base_url)
 
         """
         if not isinstance(base_url, str):
             raise ApiUrlError("base_url {0} is not a string.".format(base_url))
 
         self.base_url = base_url
+        self.client = None
 
         if not isinstance(api_version, ("".__class__, "".__class__)):
             raise ApiUrlError("api_version {0} is not a string.".format(api_version))
         self.api_version = api_version
 
         if api_token:
             if not isinstance(api_token, ("".__class__, "".__class__)):
@@ -113,35 +120,25 @@
 
         """
         params = {}
         params["User-Agent"] = "pydataverse"
         if self.api_token:
             params["key"] = str(self.api_token)
 
-        try:
-            resp = get(url, params=params)
-            if resp.status_code == 401:
-                error_msg = resp.json()["message"]
-                raise ApiAuthorizationError(
-                    "ERROR: GET - Authorization invalid {0}. MSG: {1}.".format(
-                        url, error_msg
-                    )
-                )
-            elif resp.status_code >= 300:
-                if resp.text:
-                    error_msg = resp.text
-                    raise OperationFailedError(
-                        "ERROR: GET HTTP {0} - {1}. MSG: {2}".format(
-                            resp.status_code, url, error_msg
-                        )
-                    )
-            return resp
-        except ConnectionError:
-            raise ConnectionError(
-                "ERROR: GET - Could not establish connection to api {0}.".format(url)
+        if self.client is None:
+            return self._sync_request(
+                method=httpx.get,
+                url=url,
+                params=params,
+            )
+        else:
+            return self._async_request(
+                method=self.client.get,
+                url=url,
+                params=params,
             )
 
     def post_request(self, url, data=None, auth=False, params=None, files=None):
         """Make a POST request.
 
         params will be added as key-value pairs to the URL.
 
@@ -166,27 +163,32 @@
 
         """
         params = {}
         params["User-Agent"] = "pydataverse"
         if self.api_token:
             params["key"] = self.api_token
 
-        try:
-            resp = post(url, data=data, params=params, files=files)
-            if resp.status_code == 401:
-                error_msg = resp.json()["message"]
-                raise ApiAuthorizationError(
-                    "ERROR: POST HTTP 401 - Authorization error {0}. MSG: {1}".format(
-                        url, error_msg
-                    )
-                )
-            return resp
-        except ConnectionError:
-            raise ConnectionError(
-                "ERROR: POST - Could not establish connection to API: {0}".format(url)
+        if isinstance(data, str):
+            data = json.loads(data)
+
+        if self.client is None:
+            return self._sync_request(
+                method=httpx.post,
+                url=url,
+                json=data,
+                params=params,
+                files=files,
+            )
+        else:
+            return self._async_request(
+                method=self.client.post,
+                url=url,
+                json=data,
+                params=params,
+                files=files,
             )
 
     def put_request(self, url, data=None, auth=False, params=None):
         """Make a PUT request.
 
         Parameters
         ----------
@@ -207,27 +209,30 @@
 
         """
         params = {}
         params["User-Agent"] = "pydataverse"
         if self.api_token:
             params["key"] = self.api_token
 
-        try:
-            resp = put(url, data=data, params=params)
-            if resp.status_code == 401:
-                error_msg = resp.json()["message"]
-                raise ApiAuthorizationError(
-                    "ERROR: PUT HTTP 401 - Authorization error {0}. MSG: {1}".format(
-                        url, error_msg
-                    )
-                )
-            return resp
-        except ConnectionError:
-            raise ConnectionError(
-                "ERROR: PUT - Could not establish connection to api '{0}'.".format(url)
+        if isinstance(data, str):
+            data = json.loads(data)
+
+        if self.client is None:
+            return self._sync_request(
+                method=httpx.put,
+                url=url,
+                json=data,
+                params=params,
+            )
+        else:
+            return self._async_request(
+                method=self.client.put,
+                url=url,
+                json=data,
+                params=params,
             )
 
     def delete_request(self, url, auth=False, params=None):
         """Make a Delete request.
 
         Parameters
         ----------
@@ -246,21 +251,148 @@
 
         """
         params = {}
         params["User-Agent"] = "pydataverse"
         if self.api_token:
             params["key"] = self.api_token
 
+        if self.client is None:
+            return self._sync_request(
+                method=httpx.delete,
+                url=url,
+                params=params,
+            )
+        else:
+            return self._async_request(
+                method=self.client.delete,
+                url=url,
+                params=params,
+            )
+
+    def _sync_request(
+        self,
+        method,
+        **kwargs,
+    ):
+        """
+        Sends a synchronous request to the specified URL using the specified HTTP method.
+
+        Args:
+            method (function): The HTTP method to use for the request.
+            **kwargs: Additional keyword arguments to be passed to the method.
+
+        Returns:
+            requests.Response: The response object returned by the request.
+
+        Raises:
+            ApiAuthorizationError: If the response status code is 401 (Authorization error).
+            ConnectError: If a connection to the API cannot be established.
+        """
+        assert "url" in kwargs, "URL is required for a request."
+
+        kwargs = self._filter_kwargs(kwargs)
+
+        try:
+            resp = method(**kwargs, follow_redirects=True)
+            if resp.status_code == 401:
+                error_msg = resp.json()["message"]
+                raise ApiAuthorizationError(
+                    "ERROR: HTTP 401 - Authorization error {0}. MSG: {1}".format(
+                        kwargs["url"], error_msg
+                    )
+                )
+
+            return resp
+
+        except ConnectError:
+            raise ConnectError(
+                "ERROR - Could not establish connection to api '{0}'.".format(
+                    kwargs["url"]
+                )
+            )
+
+    async def _async_request(
+        self,
+        method,
+        **kwargs,
+    ):
+        """
+        Sends an asynchronous request to the specified URL using the specified HTTP method.
+
+        Args:
+            method (callable): The HTTP method to use for the request.
+            **kwargs: Additional keyword arguments to be passed to the method.
+
+        Raises:
+            ApiAuthorizationError: If the response status code is 401 (Authorization error).
+            ConnectError: If a connection to the API cannot be established.
+
+        Returns:
+            The response object.
+
+        """
+        assert "url" in kwargs, "URL is required for a request."
+
+        kwargs = self._filter_kwargs(kwargs)
+
         try:
-            return delete(url, params=params)
-        except ConnectionError:
-            raise ConnectionError(
-                "ERROR: DELETE could not establish connection to api {}.".format(url)
+            resp = await method(**kwargs)
+
+            if resp.status_code == 401:
+                error_msg = resp.json()["message"]
+                raise ApiAuthorizationError(
+                    "ERROR: HTTP 401 - Authorization error {0}. MSG: {1}".format(
+                        kwargs["url"], error_msg
+                    )
+                )
+
+            return resp
+
+        except ConnectError:
+            raise ConnectError(
+                "ERROR - Could not establish connection to api '{0}'.".format(
+                    kwargs["url"]
+                )
             )
 
+    @staticmethod
+    def _filter_kwargs(kwargs: Dict[str, Any]) -> Dict[str, Any]:
+        """
+        Filters out any keyword arguments that are `None` from the specified dictionary.
+
+        Args:
+            kwargs (Dict[str, Any]): The dictionary to filter.
+
+        Returns:
+            Dict[str, Any]: The filtered dictionary.
+        """
+        return {k: v for k, v in kwargs.items() if v is not None}
+
+    async def __aenter__(self):
+        """
+        Context manager method that initializes an instance of httpx.AsyncClient.
+
+        Returns:
+            httpx.AsyncClient: An instance of httpx.AsyncClient.
+        """
+        self.client = httpx.AsyncClient()
+
+    async def __aexit__(self, exc_type, exc_value, traceback):
+        """
+        Closes the client connection when exiting a context manager.
+
+        Args:
+            exc_type (type): The type of the exception raised, if any.
+            exc_value (Exception): The exception raised, if any.
+            traceback (traceback): The traceback object associated with the exception, if any.
+        """
+
+        await self.client.aclose()
+        self.client = None
+
 
 class DataAccessApi(Api):
     """Class to access Dataverse's Data Access API.
 
     Examples
     -------
     Examples should be written in doctest format, and
@@ -330,21 +462,21 @@
         -------
         requests.Response
             Response object of requests library.
 
         """
         is_first_param = True
         if is_pid:
-            url = "{0}/datafile/{1}".format(self.base_url_api_data_access, identifier)
-            if data_format or no_var_header or image_thumb:
-                url += "?"
-        else:
             url = "{0}/datafile/:persistentId/?persistentId={1}".format(
                 self.base_url_api_data_access, identifier
             )
+        else:
+            url = "{0}/datafile/{1}".format(self.base_url_api_data_access, identifier)
+            if data_format or no_var_header or image_thumb:
+                url += "?"
         if data_format:
             url += "format={0}".format(data_format)
             is_first_param = False
         if no_var_header:
             if not is_first_param:
                 url += "&"
             url += "noVarHeader={0}".format(no_var_header)
```

### Comparing `pyDataverse-0.3.1/src/pyDataverse/exceptions.py` & `pydataverse-0.3.2/pyDataverse/exceptions.py`

 * *Files identical despite different names*

