# Comparing `tmp/adeft-0.8.0.tar.gz` & `tmp/adeft-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/adeft-0.8.0.tar", last modified: Mon Nov 16 00:22:29 2020, max compression
+gzip compressed data, was "dist/adeft-0.9.0.tar", last modified: Thu Nov 19 05:05:32 2020, max compression
```

## Comparing `adeft-0.8.0.tar` & `adeft-0.9.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 birbir    (1000) birbir    (1000)        0 2020-11-16 00:22:29.496810 adeft-0.8.0/
--rw-rw-r--   0 birbir    (1000) birbir    (1000)       33 2020-11-16 00:21:30.000000 adeft-0.8.0/MANIFEST.in
--rw-rw-r--   0 birbir    (1000) birbir    (1000)     5250 2020-11-16 00:22:29.496810 adeft-0.8.0/PKG-INFO
--rw-rw-r--   0 birbir    (1000) birbir    (1000)     3743 2020-11-16 00:21:30.000000 adeft-0.8.0/README.md
-drwxrwxr-x   0 birbir    (1000) birbir    (1000)        0 2020-11-16 00:22:29.496810 adeft-0.8.0/adeft/
--rw-rw-r--   0 birbir    (1000) birbir    (1000)      242 2020-11-16 00:21:30.000000 adeft-0.8.0/adeft/__init__.py
--rw-rw-r--   0 birbir    (1000) birbir    (1000)    17770 2020-11-16 00:21:30.000000 adeft-0.8.0/adeft/disambiguate.py
--rw-rw-r--   0 birbir    (1000) birbir    (1000)    28836 2020-11-16 00:21:30.000000 adeft-0.8.0/adeft/discover.py
-drwxrwxr-x   0 birbir    (1000) birbir    (1000)        0 2020-11-16 00:22:29.496810 adeft-0.8.0/adeft/download/
--rw-rw-r--   0 birbir    (1000) birbir    (1000)      401 2020-11-16 00:21:30.000000 adeft-0.8.0/adeft/download/__init__.py
--rw-rw-r--   0 birbir    (1000) birbir    (1000)      294 2020-11-16 00:21:30.000000 adeft-0.8.0/adeft/download/__main__.py
--rw-rw-r--   0 birbir    (1000) birbir    (1000)     5924 2020-11-16 00:21:30.000000 adeft-0.8.0/adeft/download/download.py
-drwxrwxr-x   0 birbir    (1000) birbir    (1000)        0 2020-11-16 00:22:29.496810 adeft-0.8.0/adeft/gui/
--rw-rw-r--   0 birbir    (1000) birbir    (1000)     4887 2020-11-16 00:21:30.000000 adeft-0.8.0/adeft/gui/__init__.py
-drwxrwxr-x   0 birbir    (1000) birbir    (1000)        0 2020-11-16 00:22:29.496810 adeft-0.8.0/adeft/gui/ground/
--rw-rw-r--   0 birbir    (1000) birbir    (1000)     2113 2020-11-16 00:21:30.000000 adeft-0.8.0/adeft/gui/ground/__init__.py
--rw-rw-r--   0 birbir    (1000) birbir    (1000)     5744 2020-11-16 00:21:30.000000 adeft-0.8.0/adeft/gui/ground/ground.py
--rw-rw-r--   0 birbir    (1000) birbir    (1000)      730 2020-11-16 00:21:30.000000 adeft-0.8.0/adeft/locations.py
-drwxrwxr-x   0 birbir    (1000) birbir    (1000)        0 2020-11-16 00:22:29.496810 adeft-0.8.0/adeft/modeling/
--rw-rw-r--   0 birbir    (1000) birbir    (1000)      159 2020-11-16 00:21:30.000000 adeft-0.8.0/adeft/modeling/__init__.py
--rw-rw-r--   0 birbir    (1000) birbir    (1000)    23307 2020-11-16 00:21:30.000000 adeft-0.8.0/adeft/modeling/classify.py
--rw-rw-r--   0 birbir    (1000) birbir    (1000)     3681 2020-11-16 00:21:30.000000 adeft-0.8.0/adeft/modeling/label.py
-drwxrwxr-x   0 birbir    (1000) birbir    (1000)        0 2020-11-16 00:22:29.496810 adeft-0.8.0/adeft/nlp/
--rw-rw-r--   0 birbir    (1000) birbir    (1000)      554 2020-11-16 00:21:30.000000 adeft-0.8.0/adeft/nlp/__init__.py
--rw-rw-r--   0 birbir    (1000) birbir    (1000)     5662 2020-11-16 00:21:30.000000 adeft-0.8.0/adeft/nlp/nlp.py
--rw-rw-r--   0 birbir    (1000) birbir    (1000)     4177 2020-11-16 00:21:30.000000 adeft-0.8.0/adeft/nlp/stopwords.json
--rw-rw-r--   0 birbir    (1000) birbir    (1000)     8307 2020-11-16 00:21:30.000000 adeft-0.8.0/adeft/recognize.py
-drwxrwxr-x   0 birbir    (1000) birbir    (1000)        0 2020-11-16 00:22:29.496810 adeft-0.8.0/adeft/score/
--rw-rw-r--   0 birbir    (1000) birbir    (1000)       40 2020-11-16 00:21:30.000000 adeft-0.8.0/adeft/score/__init__.py
--rw-rw-r--   0 birbir    (1000) birbir    (1000)   731817 2020-11-16 00:21:30.000000 adeft-0.8.0/adeft/score/_score.c
--rw-rw-r--   0 birbir    (1000) birbir    (1000)     9848 2020-11-16 00:21:30.000000 adeft-0.8.0/adeft/score/score.py
--rw-rw-r--   0 birbir    (1000) birbir    (1000)     5164 2020-11-16 00:21:30.000000 adeft-0.8.0/adeft/util.py
-drwxrwxr-x   0 birbir    (1000) birbir    (1000)        0 2020-11-16 00:22:29.496810 adeft-0.8.0/adeft.egg-info/
--rw-rw-r--   0 birbir    (1000) birbir    (1000)     5250 2020-11-16 00:22:29.000000 adeft-0.8.0/adeft.egg-info/PKG-INFO
--rw-rw-r--   0 birbir    (1000) birbir    (1000)      661 2020-11-16 00:22:29.000000 adeft-0.8.0/adeft.egg-info/SOURCES.txt
--rw-rw-r--   0 birbir    (1000) birbir    (1000)        1 2020-11-16 00:22:29.000000 adeft-0.8.0/adeft.egg-info/dependency_links.txt
--rw-rw-r--   0 birbir    (1000) birbir    (1000)       68 2020-11-16 00:22:29.000000 adeft-0.8.0/adeft.egg-info/requires.txt
--rw-rw-r--   0 birbir    (1000) birbir    (1000)        6 2020-11-16 00:22:29.000000 adeft-0.8.0/adeft.egg-info/top_level.txt
--rw-rw-r--   0 birbir    (1000) birbir    (1000)       79 2020-11-16 00:22:29.500810 adeft-0.8.0/setup.cfg
--rw-rw-r--   0 birbir    (1000) birbir    (1000)     1742 2020-11-16 00:21:30.000000 adeft-0.8.0/setup.py
+drwxrwxr-x   0 birbir    (1000) birbir    (1000)        0 2020-11-19 05:05:32.187280 adeft-0.9.0/
+-rw-rw-r--   0 birbir    (1000) birbir    (1000)       33 2020-11-19 05:02:52.000000 adeft-0.9.0/MANIFEST.in
+-rw-rw-r--   0 birbir    (1000) birbir    (1000)     5250 2020-11-19 05:05:32.187280 adeft-0.9.0/PKG-INFO
+-rw-rw-r--   0 birbir    (1000) birbir    (1000)     3743 2020-11-19 05:02:52.000000 adeft-0.9.0/README.md
+drwxrwxr-x   0 birbir    (1000) birbir    (1000)        0 2020-11-19 05:05:32.183280 adeft-0.9.0/adeft/
+-rw-rw-r--   0 birbir    (1000) birbir    (1000)      242 2020-11-19 05:02:52.000000 adeft-0.9.0/adeft/__init__.py
+-rw-rw-r--   0 birbir    (1000) birbir    (1000)    17770 2020-11-19 05:02:52.000000 adeft-0.9.0/adeft/disambiguate.py
+-rw-rw-r--   0 birbir    (1000) birbir    (1000)    28836 2020-11-19 05:02:52.000000 adeft-0.9.0/adeft/discover.py
+drwxrwxr-x   0 birbir    (1000) birbir    (1000)        0 2020-11-19 05:05:32.183280 adeft-0.9.0/adeft/download/
+-rw-rw-r--   0 birbir    (1000) birbir    (1000)      425 2020-11-19 05:02:52.000000 adeft-0.9.0/adeft/download/__init__.py
+-rw-rw-r--   0 birbir    (1000) birbir    (1000)      349 2020-11-19 05:02:52.000000 adeft-0.9.0/adeft/download/__main__.py
+-rw-rw-r--   0 birbir    (1000) birbir    (1000)     6902 2020-11-19 05:02:52.000000 adeft-0.9.0/adeft/download/download.py
+drwxrwxr-x   0 birbir    (1000) birbir    (1000)        0 2020-11-19 05:05:32.183280 adeft-0.9.0/adeft/gui/
+-rw-rw-r--   0 birbir    (1000) birbir    (1000)     5723 2020-11-19 05:02:52.000000 adeft-0.9.0/adeft/gui/__init__.py
+drwxrwxr-x   0 birbir    (1000) birbir    (1000)        0 2020-11-19 05:05:32.183280 adeft-0.9.0/adeft/gui/ground/
+-rw-rw-r--   0 birbir    (1000) birbir    (1000)     3215 2020-11-19 05:02:52.000000 adeft-0.9.0/adeft/gui/ground/__init__.py
+-rw-rw-r--   0 birbir    (1000) birbir    (1000)     8798 2020-11-19 05:02:52.000000 adeft-0.9.0/adeft/gui/ground/ground.py
+-rw-rw-r--   0 birbir    (1000) birbir    (1000)      855 2020-11-19 05:02:52.000000 adeft-0.9.0/adeft/locations.py
+drwxrwxr-x   0 birbir    (1000) birbir    (1000)        0 2020-11-19 05:05:32.183280 adeft-0.9.0/adeft/modeling/
+-rw-rw-r--   0 birbir    (1000) birbir    (1000)      159 2020-11-19 05:02:52.000000 adeft-0.9.0/adeft/modeling/__init__.py
+-rw-rw-r--   0 birbir    (1000) birbir    (1000)    23307 2020-11-19 05:02:52.000000 adeft-0.9.0/adeft/modeling/classify.py
+-rw-rw-r--   0 birbir    (1000) birbir    (1000)     3681 2020-11-19 05:02:52.000000 adeft-0.9.0/adeft/modeling/label.py
+drwxrwxr-x   0 birbir    (1000) birbir    (1000)        0 2020-11-19 05:05:32.183280 adeft-0.9.0/adeft/nlp/
+-rw-rw-r--   0 birbir    (1000) birbir    (1000)      554 2020-11-19 05:02:52.000000 adeft-0.9.0/adeft/nlp/__init__.py
+-rw-rw-r--   0 birbir    (1000) birbir    (1000)     5662 2020-11-19 05:02:52.000000 adeft-0.9.0/adeft/nlp/nlp.py
+-rw-rw-r--   0 birbir    (1000) birbir    (1000)     4177 2020-11-19 05:02:52.000000 adeft-0.9.0/adeft/nlp/stopwords.json
+-rw-rw-r--   0 birbir    (1000) birbir    (1000)     8307 2020-11-19 05:02:52.000000 adeft-0.9.0/adeft/recognize.py
+drwxrwxr-x   0 birbir    (1000) birbir    (1000)        0 2020-11-19 05:05:32.183280 adeft-0.9.0/adeft/score/
+-rw-rw-r--   0 birbir    (1000) birbir    (1000)       40 2020-11-19 05:02:52.000000 adeft-0.9.0/adeft/score/__init__.py
+-rw-rw-r--   0 birbir    (1000) birbir    (1000)   731817 2020-11-19 05:02:52.000000 adeft-0.9.0/adeft/score/_score.c
+-rw-rw-r--   0 birbir    (1000) birbir    (1000)     9848 2020-11-19 05:02:52.000000 adeft-0.9.0/adeft/score/score.py
+-rw-rw-r--   0 birbir    (1000) birbir    (1000)     5164 2020-11-19 05:02:52.000000 adeft-0.9.0/adeft/util.py
+drwxrwxr-x   0 birbir    (1000) birbir    (1000)        0 2020-11-19 05:05:32.183280 adeft-0.9.0/adeft.egg-info/
+-rw-rw-r--   0 birbir    (1000) birbir    (1000)     5250 2020-11-19 05:05:32.000000 adeft-0.9.0/adeft.egg-info/PKG-INFO
+-rw-rw-r--   0 birbir    (1000) birbir    (1000)      661 2020-11-19 05:05:32.000000 adeft-0.9.0/adeft.egg-info/SOURCES.txt
+-rw-rw-r--   0 birbir    (1000) birbir    (1000)        1 2020-11-19 05:05:32.000000 adeft-0.9.0/adeft.egg-info/dependency_links.txt
+-rw-rw-r--   0 birbir    (1000) birbir    (1000)       68 2020-11-19 05:05:32.000000 adeft-0.9.0/adeft.egg-info/requires.txt
+-rw-rw-r--   0 birbir    (1000) birbir    (1000)        6 2020-11-19 05:05:32.000000 adeft-0.9.0/adeft.egg-info/top_level.txt
+-rw-rw-r--   0 birbir    (1000) birbir    (1000)       79 2020-11-19 05:05:32.187280 adeft-0.9.0/setup.cfg
+-rw-rw-r--   0 birbir    (1000) birbir    (1000)     1742 2020-11-19 05:02:52.000000 adeft-0.9.0/setup.py
```

### Comparing `adeft-0.8.0/PKG-INFO` & `adeft-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: adeft
-Version: 0.8.0
+Version: 0.9.0
 Summary: Acromine based Disambiguation of Entities From Text
 Home-page: https://github.com/indralab/adeft
 Author: adeft developers, Harvard Medical School
 Author-email: albert_steppi@hms.harvard.edu
 License: UNKNOWN
-Download-URL: https://github.com/indralab/adeft/archive/0.8.0.tar.gz
+Download-URL: https://github.com/indralab/adeft/archive/0.9.0.tar.gz
 Description: # Adeft
         [![DOI](https://joss.theoj.org/papers/10.21105/joss.01708/status.svg)](https://doi.org/10.21105/joss.01708)
         [![DOI](https://zenodo.org/badge/156276061.svg)](https://zenodo.org/badge/latestdoi/156276061)
         [![License](https://img.shields.io/badge/License-BSD%202--Clause-orange.svg)](https://opensource.org/licenses/BSD-2-Clause)
         [![Build](https://travis-ci.org/indralab/adeft.svg)](https://travis-ci.org/indralab/adeft)
         [![Documentation](https://readthedocs.org/projects/adeft/badge/?version=latest)](https://adeft.readthedocs.io/en/latest/?badge=latest)
         [![PyPI version](https://badge.fury.io/py/adeft.svg)](https://badge.fury.io/py/adeft)
```

### Comparing `adeft-0.8.0/README.md` & `adeft-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `adeft-0.8.0/adeft/disambiguate.py` & `adeft-0.9.0/adeft/disambiguate.py`

 * *Files identical despite different names*

### Comparing `adeft-0.8.0/adeft/discover.py` & `adeft-0.9.0/adeft/discover.py`

 * *Files identical despite different names*

### Comparing `adeft-0.8.0/adeft/download/download.py` & `adeft-0.9.0/adeft/download/download.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import os
+import gzip
 import json
 import wget
 import shutil
 import logging
 import requests
 
 
 from adeft.locations import ADEFT_MODELS_PATH, S3_BUCKET_URL, \
-    TEST_RESOURCES_PATH
+    RESOURCES_PATH, TEST_RESOURCES_PATH
 
 
 logger = logging.getLogger(__file__)
 
 
 def setup_models_folder():
     """Create models folder if it does not exist and download models
@@ -60,14 +61,40 @@
             # overwrite existing files, choosing a new name instead
             _remove_if_exists(resource_path)
             wget.download(url=os.path.join(S3_BUCKET_URL, 'Models',
                                            model, resource),
                           out=resource_path)
 
 
+def setup_resources_folder():
+    """Make resources folder and download resources
+
+    Replaces content in existing resources folder if it already exists
+    """
+    if os.path.isdir(RESOURCES_PATH):
+        shutil.rmtree(RESOURCES_PATH)
+    os.mkdir(RESOURCES_PATH)
+    download_resources()
+
+
+def download_resources():
+    resources = ['groundings.csv']
+    for resource in resources:
+        resource_path = os.path.join(RESOURCES_PATH, resource)
+        _remove_if_exists(resource_path + '.gz')
+        wget.download(url=os.path.join(S3_BUCKET_URL, 'Resources',
+                                       resource + '.gz'),
+                      out=resource_path + '.gz')
+        with gzip.open(os.path.join(RESOURCES_PATH, resource + '.gz'),
+                       'rb') as f_in:
+            with open(os.path.join(RESOURCES_PATH, resource), 'wb') as f_out:
+                shutil.copyfileobj(f_in, f_out)
+        os.remove(resource_path + '.gz')
+
+
 def setup_test_resource_folder():
     """Make test resource folders and download content
 
     Replaces content in existing test_resource_folders if they already
     exist.
     """
     if os.path.isdir(TEST_RESOURCES_PATH):
```

### Comparing `adeft-0.8.0/adeft/gui/__init__.py` & `adeft-0.9.0/adeft/gui/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,16 +11,17 @@
 from multiprocessing import Process
 
 
 logger = logging.getLogger(__name__)
 
 
 def ground_with_gui(longforms, scores, grounding_map=None,
-                    names=None, pos_labels=None, verbose=False, port=5000,
-                    no_browser=False, test=False):
+                    names=None, pos_labels=None,
+                    groundings_file=None,
+                    verbose=False, port=5000, no_browser=False, test=False):
     """Opens grounding GUI in browser. Returns output upon user submission.
 
     Parameters
     ----------
     longforms : list of str
         List of longforms to ground
     scores : list of float
@@ -31,14 +32,27 @@
         created by an imperfect grounding function. Default: None
     names : Optional[dict]
         Dictionary map groundings from grounding_map to standardized names.
         This is ignored if grounding_map is set to None. Default: None
     pos_labels : Optional[list]
         List of groundings to be considered as positive labels.
         This is ignored if grounding_map is set to None. Default: None
+    groundings_file : Optional[str]
+        Path to a headerless csv file with three columns, one for
+        namespace, identifier, and standard name respectively. Rows should
+        be of the form
+        MESH,D011839,"Radiation, Ionizing"
+        with commas used as a separator and double quotes for escape.
+        If such a table is supplied, users only need to supply the namespace
+        along with only one of the standard name or identifier for each
+        potential grounding with a row in the table. The missing entry will
+        will be inferred. The path to such a file with groundings for the
+        namespaces
+        CHEBI, DOID, EFO, FPLX, GO, HGNC, HP, IP, MESH, NCIT, and UP
+        can be found at `adeft.locations.GROUNDINGS_FILE_PATH. Default: None
     verbose : Optional[bool]
         When true, display logging from flask's werkzeug server.
         Default: False
     port : Optional[int]
         Port where flask is served. Defaults to flask's default.
         Default: 5000
     no_browser : Optional[bool]
@@ -92,15 +106,15 @@
     # Round scores for better presentation
     scores = [round(score, 2) for score in scores]
 
     # create temporary file for storing output
     outpath = tempfile.mkdtemp()
     # initialize flask app
     app = create_app(longforms, scores, grounding_map,
-                     names_map, labels, pos_labels, outpath,
+                     names_map, labels, pos_labels, groundings_file, outpath,
                      verbose, test=test)
 
     # Run flask server in new process
     flask_server = Process(target=_run_app, args=(app, port))
     flask_server.start()
     # Open app in browser unless a test is being run
     if not test and not no_browser:
```

### Comparing `adeft-0.8.0/adeft/locations.py` & `adeft-0.9.0/adeft/locations.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,9 +11,11 @@
 
 ADEFT_HOME = os.environ.get('ADEFT_HOME')
 if ADEFT_HOME is None:
     ADEFT_HOME = os.path.join(os.path.expanduser('~'), '.adeft')
 
 ADEFT_PATH = os.path.join(ADEFT_HOME, __version__)
 ADEFT_MODELS_PATH = os.path.join(ADEFT_PATH, 'models')
+RESOURCES_PATH = os.path.join(ADEFT_PATH, 'resources')
+GROUNDINGS_FILE_PATH = os.path.join(RESOURCES_PATH, 'groundings.csv')
 TEST_RESOURCES_PATH = os.path.join(ADEFT_PATH, 'test_resources')
 S3_BUCKET_URL = os.path.join('http://adeft.s3.amazonaws.com', __version__)
```

### Comparing `adeft-0.8.0/adeft/modeling/classify.py` & `adeft-0.9.0/adeft/modeling/classify.py`

 * *Files identical despite different names*

### Comparing `adeft-0.8.0/adeft/modeling/label.py` & `adeft-0.9.0/adeft/modeling/label.py`

 * *Files identical despite different names*

### Comparing `adeft-0.8.0/adeft/nlp/__init__.py` & `adeft-0.9.0/adeft/nlp/__init__.py`

 * *Files identical despite different names*

### Comparing `adeft-0.8.0/adeft/nlp/nlp.py` & `adeft-0.9.0/adeft/nlp/nlp.py`

 * *Files identical despite different names*

### Comparing `adeft-0.8.0/adeft/nlp/stopwords.json` & `adeft-0.9.0/adeft/nlp/stopwords.json`

 * *Files identical despite different names*

### Comparing `adeft-0.8.0/adeft/recognize.py` & `adeft-0.9.0/adeft/recognize.py`

 * *Files identical despite different names*

### Comparing `adeft-0.8.0/adeft/score/_score.c` & `adeft-0.9.0/adeft/score/_score.c`

 * *Files identical despite different names*

### Comparing `adeft-0.8.0/adeft/score/score.py` & `adeft-0.9.0/adeft/score/score.py`

 * *Files identical despite different names*

### Comparing `adeft-0.8.0/adeft/util.py` & `adeft-0.9.0/adeft/util.py`

 * *Files identical despite different names*

### Comparing `adeft-0.8.0/adeft.egg-info/PKG-INFO` & `adeft-0.9.0/adeft.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: adeft
-Version: 0.8.0
+Version: 0.9.0
 Summary: Acromine based Disambiguation of Entities From Text
 Home-page: https://github.com/indralab/adeft
 Author: adeft developers, Harvard Medical School
 Author-email: albert_steppi@hms.harvard.edu
 License: UNKNOWN
-Download-URL: https://github.com/indralab/adeft/archive/0.8.0.tar.gz
+Download-URL: https://github.com/indralab/adeft/archive/0.9.0.tar.gz
 Description: # Adeft
         [![DOI](https://joss.theoj.org/papers/10.21105/joss.01708/status.svg)](https://doi.org/10.21105/joss.01708)
         [![DOI](https://zenodo.org/badge/156276061.svg)](https://zenodo.org/badge/latestdoi/156276061)
         [![License](https://img.shields.io/badge/License-BSD%202--Clause-orange.svg)](https://opensource.org/licenses/BSD-2-Clause)
         [![Build](https://travis-ci.org/indralab/adeft.svg)](https://travis-ci.org/indralab/adeft)
         [![Documentation](https://readthedocs.org/projects/adeft/badge/?version=latest)](https://adeft.readthedocs.io/en/latest/?badge=latest)
         [![PyPI version](https://badge.fury.io/py/adeft.svg)](https://badge.fury.io/py/adeft)
```

### Comparing `adeft-0.8.0/adeft.egg-info/SOURCES.txt` & `adeft-0.9.0/adeft.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adeft-0.8.0/setup.py` & `adeft-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,21 +24,21 @@
 
 if USE_CYTHON:
     from Cython.Build import cythonize
     extensions = cythonize(extensions,
                            compiler_directives={'language_level': 3})
 
 setup(name='adeft',
-      version='0.8.0',
+      version='0.9.0',
       description=('Acromine based Disambiguation of Entities From'
                    ' Text'),
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/indralab/adeft',
-      download_url='https://github.com/indralab/adeft/archive/0.8.0.tar.gz',
+      download_url='https://github.com/indralab/adeft/archive/0.9.0.tar.gz',
       author='adeft developers, Harvard Medical School',
       author_email='albert_steppi@hms.harvard.edu',
       classifiers=[
           'Development Status :: 4 - Beta',
           'Programming Language :: Python :: 3.5',
           'Programming Language :: Python :: 3.6',
           'Programming Language :: Python :: 3.7',
```

