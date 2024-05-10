# Comparing `tmp/nvcl-kit-1.1.7.tar.gz` & `tmp/nvcl-kit-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvcl-kit-1.1.7.tar", last modified: Thu Mar 14 02:54:51 2024, max compression
+gzip compressed data, was "nvcl-kit-1.1.8.tar", last modified: Fri May 10 08:05:12 2024, max compression
```

## Comparing `nvcl-kit-1.1.7.tar` & `nvcl-kit-1.1.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     3915 2024-03-14 02:54:28.443588 nvcl-kit-1.1.7/LICENSE
--rw-r--r--   0        0        0     2896 2024-03-14 02:54:28.443588 nvcl-kit-1.1.7/README.md
--rw-r--r--   0        0        0       14 2024-03-14 02:54:28.457588 nvcl-kit-1.1.7/nvcl_kit/__init__.py
--rw-r--r--   0        0        0     6773 2024-03-14 02:54:28.457588 nvcl-kit-1.1.7/nvcl_kit/constants.py
--rw-r--r--   0        0        0     4386 2024-03-14 02:54:28.457588 nvcl-kit-1.1.7/nvcl_kit/generators.py
--rw-r--r--   0        0        0     5806 2024-03-14 02:54:28.457588 nvcl-kit-1.1.7/nvcl_kit/param_builder.py
--rw-r--r--   0        0        0    41167 2024-03-14 02:54:28.457588 nvcl-kit-1.1.7/nvcl_kit/reader.py
--rw-r--r--   0        0        0    16111 2024-03-14 02:54:28.457588 nvcl-kit-1.1.7/nvcl_kit/svc_interface.py
--rw-r--r--   0        0        0    10931 2024-03-14 02:54:28.457588 nvcl-kit-1.1.7/nvcl_kit/wfs_helpers.py
--rw-r--r--   0        0        0      360 2024-03-14 02:54:28.457588 nvcl-kit-1.1.7/nvcl_kit/xml_helpers.py
--rw-r--r--   0        0        0     1020 2024-03-14 02:54:28.458588 nvcl-kit-1.1.7/pyproject.toml
--rw-r--r--   0        0        0     3690 1970-01-01 00:00:00.000000 nvcl-kit-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0     3915 2024-05-10 08:04:48.141348 nvcl-kit-1.1.8/LICENSE
+-rw-r--r--   0        0        0     2896 2024-05-10 08:04:48.141348 nvcl-kit-1.1.8/README.md
+-rw-r--r--   0        0        0       14 2024-05-10 08:04:48.162348 nvcl-kit-1.1.8/nvcl_kit/__init__.py
+-rw-r--r--   0        0        0     6773 2024-05-10 08:04:48.162348 nvcl-kit-1.1.8/nvcl_kit/constants.py
+-rw-r--r--   0        0        0     4386 2024-05-10 08:04:48.162348 nvcl-kit-1.1.8/nvcl_kit/generators.py
+-rw-r--r--   0        0        0     5806 2024-05-10 08:04:48.163348 nvcl-kit-1.1.8/nvcl_kit/param_builder.py
+-rw-r--r--   0        0        0    40455 2024-05-10 08:04:48.163348 nvcl-kit-1.1.8/nvcl_kit/reader.py
+-rw-r--r--   0        0        0    16111 2024-05-10 08:04:48.163348 nvcl-kit-1.1.8/nvcl_kit/svc_interface.py
+-rw-r--r--   0        0        0    10931 2024-05-10 08:04:48.163348 nvcl-kit-1.1.8/nvcl_kit/wfs_helpers.py
+-rw-r--r--   0        0        0     1240 2024-05-10 08:04:48.163348 nvcl-kit-1.1.8/nvcl_kit/xml_helpers.py
+-rw-r--r--   0        0        0     1020 2024-05-10 08:04:48.164348 nvcl-kit-1.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3690 1970-01-01 00:00:00.000000 nvcl-kit-1.1.8/PKG-INFO
```

### Comparing `nvcl-kit-1.1.7/LICENSE` & `nvcl-kit-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nvcl-kit-1.1.7/README.md` & `nvcl-kit-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `nvcl-kit-1.1.7/nvcl_kit/constants.py` & `nvcl-kit-1.1.8/nvcl_kit/constants.py`

 * *Files identical despite different names*

### Comparing `nvcl-kit-1.1.7/nvcl_kit/generators.py` & `nvcl-kit-1.1.8/nvcl_kit/generators.py`

 * *Files identical despite different names*

### Comparing `nvcl-kit-1.1.7/nvcl_kit/param_builder.py` & `nvcl-kit-1.1.8/nvcl_kit/param_builder.py`

 * *Files identical despite different names*

### Comparing `nvcl-kit-1.1.7/nvcl_kit/reader.py` & `nvcl-kit-1.1.8/nvcl_kit/reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,20 +16,18 @@
 from owslib.wfs import WebFeatureService
 from owslib.util import ServiceException
 
 from http.client import HTTPException
 
 from shapely.geometry.polygon import LinearRing
 
-from dateutil.parser import parse, ParserError
-
 from nvcl_kit.svc_interface import _ServiceInterface
 
 from nvcl_kit.wfs_helpers import fetch_wfs_bh_list
-from nvcl_kit.xml_helpers import clean_xml_parse
+from nvcl_kit.xml_helpers import clean_xml_parse, parse_dates
 
 ENFORCE_IS_PUBLIC = True
 ''' Enforce the 'is_public' flag , i.e. any data with 'is_public' set to 'false'
     will be ignored
 '''
 
 LOG_LVL = logging.INFO
@@ -332,15 +330,15 @@
                 datasetid_list.append(dataset_id)
         return datasetid_list
 
     def get_dataset_list(self, nvcl_id):
         ''' Retrieves a list of dataset objects
 
         :param nvcl_id: NVCL 'holeidentifier' parameter, the 'nvcl_id' from each item retrieved from 'get_feature_list()' or 'get_nvcl_id_list()'
-        :returns: a list of SimpleNamespace objects, attributes are: dataset_id, dataset_name, borehole_uri, tray_id, section_id, domain_id, modified_date (datetime object)
+        :returns: a list of SimpleNamespace objects, attributes are: dataset_id, dataset_name, borehole_uri, tray_id, section_id, domain_id, created_date, (optional datetime object), modified_date (optional datetime object)
         '''
         response_str = self.svc.get_dataset_collection(nvcl_id)
         if not response_str:
             return []
         root = clean_xml_parse(response_str)
         dataset_list = []
         for child in root.findall('./Dataset'):
@@ -351,27 +349,22 @@
                 continue
             # Optional
             dataset_obj = SimpleNamespace(dataset_id=dataset_id,
                                           dataset_name=dataset_name)
             for label, key in [('borehole_uri', './boreholeURI'),
                                ('tray_id', './trayID'),
                                ('section_id', './sectionID'),
-                               ('domain_id', './domainID'),
-                               ('modified_date', './modifiedDate')]:
+                               ('domain_id', './domainID')]:
                 val = child.findtext(key, default='')
                 if val:
-                    if label != 'modified_date':
-                        setattr(dataset_obj, label, val)
-                    else:
-                        # Try to parse the modified date
-                        try:
-                            date_obj = parse(val)
-                            setattr(dataset_obj, label, date_obj)
-                        except ParserError:
-                            pass
+                    setattr(dataset_obj, label, val)
+            # Look for created & modified dates
+            for key, val in parse_dates(child).items():
+                setattr(dataset_obj, key, val)
+
             dataset_list.append(dataset_obj)
         return dataset_list
 
     def get_all_imglogs(self, dataset_id):
         ''' Retrieves a list of all log objects from mosaic service
 
         :param dataset_id: dataset id, taken from 'get_datasetid_list()' or 'get_dataset_list()'
@@ -624,43 +617,38 @@
         ''' Retrieves a set of generic log data for a particular borehole, given an nvcl id
 
         :param nvcl_id: NVCL 'holeidentifier' parameter,
                         the 'nvcl_id' from each item retrieved from 'get_feature_list()' or 'get_nvcl_id_list()'
 
         :returns: a list of SimpleNamespace() objects with attributes:
                   log_id, log_name, is_public, log_type, algorithm_id, mask_log_id,
-                     modified_date (optional datetime object not supported by all services)
+                     created_date, modified_date (optional datetime objects not supported by all services)
                   NB: 'mask_log_id' is not supported by all services and may be an empty string'''
         response_str = self.svc.get_dataset_collection(nvcl_id)
         if not response_str:
             return []
         root = clean_xml_parse(response_str)
         log_list = []
         for ds_child in root.findall('./Dataset'):
-            # Get the modified date
-            date_str = ds_child.findtext('./modifiedDate', default='')
-            date_obj = None
-            if date_str:
-                # Try to parse the modified date from the dataset attributes
-                try:
-                    date_obj = parse(date_str)
-                except ParserError:
-                    pass
+            # Get the dates from the 'Dataset' elements
+            date_dict = parse_dates(ds_child)
+            # Get the log data from the 'Logs' elements
             for log_child in ds_child.findall('./Logs/Log'):
                 log_id = log_child.findtext('LogID', default='')
                 log_name = log_child.findtext('logName', default='')
                 is_public = log_child.findtext('ispublic', default='')
                 log_type = log_child.findtext('logType', default='')
                 algorithm_id = log_child.findtext('algorithmoutID', default='')
                 mask_log_id = log_child.findtext('maskLogId', default='')
                 if log_name != '' and log_id != '':
                     log_obj = SimpleNamespace(log_id=log_id, log_name=log_name, is_public=is_public, log_type=log_type,
                                               algorithm_id=algorithm_id, mask_log_id=mask_log_id)
-                    if date_obj is not None:
-                        setattr(log_obj, 'modified_date', date_obj)
+                    # Set dates, if they were found
+                    for key, val in date_dict.items():
+                        setattr(log_obj, key, val)
                     log_list.append(log_obj)
         return log_list
 
     def get_imagelog_data(self, nvcl_id):
         ''' Retrieves a set of image log data for a particular borehole
 
         :param nvcl_id: NVCL 'holeidentifier' parameter,
@@ -670,32 +658,24 @@
                   log_id, log_name, sample_count, modified_date (optional)
         '''
         response_str = self.svc.get_dataset_collection(nvcl_id)
         if not response_str:
             return []
         root = clean_xml_parse(response_str)
         log_list = []
-        mod_date_str = root.findtext('./Dataset/modifiedDate', default='')
-        date_obj = None
-        # Optionally look for 'modifiedDate' element
-        if mod_date_str != '':
-            # Try to parse the modified date
-            try:
-                date_obj = parse(mod_date_str)
-            except ParserError:
-                pass
         for ds_child in root.findall('./Dataset'):
+            date_dict = parse_dates(ds_child)
             for log_child in ds_child.findall('./ImageLogs/Log'):
                 log_name = log_child.findtext('LogName', default='')
                 log_id = log_child.findtext('LogID', default='')
                 sample_count = log_child.findtext('SampleCount', default='')
                 if log_name != '' and log_id != '':
                     log_obj = SimpleNamespace(log_id=log_id, log_name=log_name, sample_count=sample_count)
-                    if date_obj is not None:
-                        setattr(log_obj, 'modified_date', date_obj)
+                    for key, val in date_dict.items():
+                        setattr(log_obj, key, val)
                     log_list.append(log_obj)
         return log_list
 
     def get_spectrallog_data(self, nvcl_id):
         ''' Retrieves a set of spectral log data for a particular borehole
 
         :param nvcl_id: NVCL 'holeidentifier' parameter,
```

### Comparing `nvcl-kit-1.1.7/nvcl_kit/svc_interface.py` & `nvcl-kit-1.1.8/nvcl_kit/svc_interface.py`

 * *Files identical despite different names*

### Comparing `nvcl-kit-1.1.7/nvcl_kit/wfs_helpers.py` & `nvcl-kit-1.1.8/nvcl_kit/wfs_helpers.py`

 * *Files identical despite different names*

### Comparing `nvcl-kit-1.1.7/pyproject.toml` & `nvcl-kit-1.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nvcl_kit"
-version = "1.1.7"
+version = "1.1.8"
 description = "Downloads Australian National Virtual Core Library (NVCL) datasets"
 authors = [
     { name = "Vincent Fazio", email = "vincent.fazio@csiro.au" },
 ]
 dependencies = [
     "owslib>=0.29.2",
     "shapely>=2.0.1",
```

### Comparing `nvcl-kit-1.1.7/PKG-INFO` & `nvcl-kit-1.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvcl_kit
-Version: 1.1.7
+Version: 1.1.8
 Summary: Downloads Australian National Virtual Core Library (NVCL) datasets
 License: CSIRO BSD/MIT
 Author-email: Vincent Fazio <vincent.fazio@csiro.au>
 Requires-Python: >=3.8
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

