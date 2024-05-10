# Comparing `tmp/pybiopax-0.1.4.tar.gz` & `tmp/pybiopax-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybiopax-0.1.4.tar", last modified: Tue Jul 11 21:29:06 2023, max compression
+gzip compressed data, was "pybiopax-0.1.5.tar", last modified: Fri May 10 20:41:35 2024, max compression
```

## Comparing `pybiopax-0.1.4.tar` & `pybiopax-0.1.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 ben        (503) staff       (20)        0 2023-07-11 21:29:06.977102 pybiopax-0.1.4/
--rw-r--r--   0 ben        (503) staff       (20)     1346 2022-03-06 12:43:07.000000 pybiopax-0.1.4/LICENSE
--rw-r--r--   0 ben        (503) staff       (20)      160 2023-02-09 04:17:55.000000 pybiopax-0.1.4/MANIFEST.in
--rw-r--r--   0 ben        (503) staff       (20)     4634 2023-07-11 21:29:06.976962 pybiopax-0.1.4/PKG-INFO
--rw-r--r--   0 ben        (503) staff       (20)     3972 2022-09-06 22:49:47.000000 pybiopax-0.1.4/README.md
-drwxr-xr-x   0 ben        (503) staff       (20)        0 2023-07-11 21:29:06.962265 pybiopax-0.1.4/doc/
--rw-r--r--   0 ben        (503) staff       (20)      634 2022-03-06 12:43:07.000000 pybiopax-0.1.4/doc/Makefile
--rw-r--r--   0 ben        (503) staff       (20)     2377 2022-09-06 22:49:47.000000 pybiopax-0.1.4/doc/conf.py
--rw-r--r--   0 ben        (503) staff       (20)      447 2022-09-06 22:49:47.000000 pybiopax-0.1.4/doc/index.rst
--rw-r--r--   0 ben        (503) staff       (20)      795 2022-03-06 12:43:07.000000 pybiopax-0.1.4/doc/make.bat
-drwxr-xr-x   0 ben        (503) staff       (20)        0 2023-07-11 21:29:06.963179 pybiopax-0.1.4/doc/modules/
--rw-r--r--   0 ben        (503) staff       (20)       93 2022-03-06 12:43:07.000000 pybiopax-0.1.4/doc/modules/api.rst
--rw-r--r--   0 ben        (503) staff       (20)      772 2022-09-06 22:49:47.000000 pybiopax-0.1.4/doc/modules/biopax.rst
--rw-r--r--   0 ben        (503) staff       (20)       95 2022-03-06 12:43:07.000000 pybiopax-0.1.4/doc/modules/paths.rst
--rw-r--r--   0 ben        (503) staff       (20)      119 2022-03-06 12:43:07.000000 pybiopax-0.1.4/doc/modules/pc_client.rst
--rw-r--r--   0 ben        (503) staff       (20)      130 2022-03-06 12:43:07.000000 pybiopax-0.1.4/doc/modules/xml_util.rst
--rw-r--r--   0 ben        (503) staff       (20)       82 2022-03-06 12:43:07.000000 pybiopax-0.1.4/doc/requirements.txt
-drwxr-xr-x   0 ben        (503) staff       (20)        0 2023-07-11 21:29:06.964500 pybiopax-0.1.4/pybiopax/
--rw-r--r--   0 ben        (503) staff       (20)       42 2023-07-11 21:28:45.000000 pybiopax-0.1.4/pybiopax/__init__.py
--rw-r--r--   0 ben        (503) staff       (20)    10040 2023-02-09 04:17:55.000000 pybiopax-0.1.4/pybiopax/api.py
-drwxr-xr-x   0 ben        (503) staff       (20)        0 2023-07-11 21:29:06.966373 pybiopax-0.1.4/pybiopax/biopax/
--rw-r--r--   0 ben        (503) staff       (20)      281 2023-02-09 04:17:55.000000 pybiopax-0.1.4/pybiopax/biopax/__init__.py
--rw-r--r--   0 ben        (503) staff       (20)     7579 2023-07-11 21:28:45.000000 pybiopax-0.1.4/pybiopax/biopax/base.py
--rw-r--r--   0 ben        (503) staff       (20)     5544 2022-09-06 22:49:47.000000 pybiopax-0.1.4/pybiopax/biopax/interaction.py
--rw-r--r--   0 ben        (503) staff       (20)     5492 2023-02-09 04:17:55.000000 pybiopax-0.1.4/pybiopax/biopax/model.py
--rw-r--r--   0 ben        (503) staff       (20)     3166 2022-09-06 22:49:47.000000 pybiopax-0.1.4/pybiopax/biopax/physical_entity.py
--rw-r--r--   0 ben        (503) staff       (20)    18908 2023-07-11 21:28:45.000000 pybiopax-0.1.4/pybiopax/biopax/util.py
--rw-r--r--   0 ben        (503) staff       (20)     3363 2022-03-06 12:43:07.000000 pybiopax-0.1.4/pybiopax/paths.py
--rw-r--r--   0 ben        (503) staff       (20)     3017 2022-03-06 12:43:07.000000 pybiopax-0.1.4/pybiopax/pc_client.py
--rw-r--r--   0 ben        (503) staff       (20)        0 2023-02-09 04:17:55.000000 pybiopax-0.1.4/pybiopax/py.typed
--rw-r--r--   0 ben        (503) staff       (20)     1409 2022-09-06 22:49:47.000000 pybiopax-0.1.4/pybiopax/references.py
-drwxr-xr-x   0 ben        (503) staff       (20)        0 2023-07-11 21:29:06.976665 pybiopax-0.1.4/pybiopax/tests/
--rw-r--r--   0 ben        (503) staff       (20)        0 2022-03-06 12:43:07.000000 pybiopax-0.1.4/pybiopax/tests/__init__.py
--rw-r--r--   0 ben        (503) staff       (20)  3623423 2022-03-06 12:43:07.000000 pybiopax-0.1.4/pybiopax/tests/biopax_test.owl.gz
--rw-r--r--   0 ben        (503) staff       (20)     3244 2022-09-06 22:49:47.000000 pybiopax-0.1.4/pybiopax/tests/test_biopax.py
--rw-r--r--   0 ben        (503) staff       (20)     2718 2022-03-06 12:43:07.000000 pybiopax-0.1.4/pybiopax/tests/test_paths.py
--rw-r--r--   0 ben        (503) staff       (20)      470 2023-02-09 04:17:55.000000 pybiopax-0.1.4/pybiopax/tests/test_serialization.py
--rw-r--r--   0 ben        (503) staff       (20)     3995 2022-03-06 12:43:07.000000 pybiopax-0.1.4/pybiopax/xml_util.py
-drwxr-xr-x   0 ben        (503) staff       (20)        0 2023-07-11 21:29:06.965168 pybiopax-0.1.4/pybiopax.egg-info/
--rw-r--r--   0 ben        (503) staff       (20)     4634 2023-07-11 21:29:06.000000 pybiopax-0.1.4/pybiopax.egg-info/PKG-INFO
--rw-r--r--   0 ben        (503) staff       (20)      864 2023-07-11 21:29:06.000000 pybiopax-0.1.4/pybiopax.egg-info/SOURCES.txt
--rw-r--r--   0 ben        (503) staff       (20)        1 2023-07-11 21:29:06.000000 pybiopax-0.1.4/pybiopax.egg-info/dependency_links.txt
--rw-r--r--   0 ben        (503) staff       (20)       19 2023-07-11 21:29:06.000000 pybiopax-0.1.4/pybiopax.egg-info/requires.txt
--rw-r--r--   0 ben        (503) staff       (20)        9 2023-07-11 21:29:06.000000 pybiopax-0.1.4/pybiopax.egg-info/top_level.txt
--rw-r--r--   0 ben        (503) staff       (20)      189 2022-03-06 12:43:07.000000 pybiopax-0.1.4/pyproject.toml
--rw-r--r--   0 ben        (503) staff       (20)       38 2023-07-11 21:29:06.977136 pybiopax-0.1.4/setup.cfg
--rw-r--r--   0 ben        (503) staff       (20)     1474 2022-03-06 12:43:07.000000 pybiopax-0.1.4/setup.py
+drwxr-xr-x   0 ben        (503) staff       (20)        0 2024-05-10 20:41:35.110610 pybiopax-0.1.5/
+-rw-r--r--   0 ben        (503) staff       (20)     1346 2022-03-06 12:43:07.000000 pybiopax-0.1.5/LICENSE
+-rw-r--r--   0 ben        (503) staff       (20)      160 2023-02-09 04:17:55.000000 pybiopax-0.1.5/MANIFEST.in
+-rw-r--r--   0 ben        (503) staff       (20)     4634 2024-05-10 20:41:35.110459 pybiopax-0.1.5/PKG-INFO
+-rw-r--r--   0 ben        (503) staff       (20)     3972 2022-09-06 22:49:47.000000 pybiopax-0.1.5/README.md
+drwxr-xr-x   0 ben        (503) staff       (20)        0 2024-05-10 20:41:35.099512 pybiopax-0.1.5/doc/
+-rw-r--r--   0 ben        (503) staff       (20)      634 2022-03-06 12:43:07.000000 pybiopax-0.1.5/doc/Makefile
+-rw-r--r--   0 ben        (503) staff       (20)     2377 2022-09-06 22:49:47.000000 pybiopax-0.1.5/doc/conf.py
+-rw-r--r--   0 ben        (503) staff       (20)      447 2022-09-06 22:49:47.000000 pybiopax-0.1.5/doc/index.rst
+-rw-r--r--   0 ben        (503) staff       (20)      795 2022-03-06 12:43:07.000000 pybiopax-0.1.5/doc/make.bat
+drwxr-xr-x   0 ben        (503) staff       (20)        0 2024-05-10 20:41:35.100220 pybiopax-0.1.5/doc/modules/
+-rw-r--r--   0 ben        (503) staff       (20)       93 2022-03-06 12:43:07.000000 pybiopax-0.1.5/doc/modules/api.rst
+-rw-r--r--   0 ben        (503) staff       (20)      772 2022-09-06 22:49:47.000000 pybiopax-0.1.5/doc/modules/biopax.rst
+-rw-r--r--   0 ben        (503) staff       (20)       95 2022-03-06 12:43:07.000000 pybiopax-0.1.5/doc/modules/paths.rst
+-rw-r--r--   0 ben        (503) staff       (20)      119 2022-03-06 12:43:07.000000 pybiopax-0.1.5/doc/modules/pc_client.rst
+-rw-r--r--   0 ben        (503) staff       (20)      130 2022-03-06 12:43:07.000000 pybiopax-0.1.5/doc/modules/xml_util.rst
+-rw-r--r--   0 ben        (503) staff       (20)       82 2022-03-06 12:43:07.000000 pybiopax-0.1.5/doc/requirements.txt
+drwxr-xr-x   0 ben        (503) staff       (20)        0 2024-05-10 20:41:35.101479 pybiopax-0.1.5/pybiopax/
+-rw-r--r--   0 ben        (503) staff       (20)       42 2024-05-10 20:41:14.000000 pybiopax-0.1.5/pybiopax/__init__.py
+-rw-r--r--   0 ben        (503) staff       (20)    10267 2024-05-10 20:40:50.000000 pybiopax-0.1.5/pybiopax/api.py
+drwxr-xr-x   0 ben        (503) staff       (20)        0 2024-05-10 20:41:35.103579 pybiopax-0.1.5/pybiopax/biopax/
+-rw-r--r--   0 ben        (503) staff       (20)      281 2023-02-09 04:17:55.000000 pybiopax-0.1.5/pybiopax/biopax/__init__.py
+-rw-r--r--   0 ben        (503) staff       (20)     7579 2023-07-11 21:28:45.000000 pybiopax-0.1.5/pybiopax/biopax/base.py
+-rw-r--r--   0 ben        (503) staff       (20)     5544 2022-09-06 22:49:47.000000 pybiopax-0.1.5/pybiopax/biopax/interaction.py
+-rw-r--r--   0 ben        (503) staff       (20)     5492 2023-02-09 04:17:55.000000 pybiopax-0.1.5/pybiopax/biopax/model.py
+-rw-r--r--   0 ben        (503) staff       (20)     3166 2022-09-06 22:49:47.000000 pybiopax-0.1.5/pybiopax/biopax/physical_entity.py
+-rw-r--r--   0 ben        (503) staff       (20)    18908 2023-07-11 21:28:45.000000 pybiopax-0.1.5/pybiopax/biopax/util.py
+-rw-r--r--   0 ben        (503) staff       (20)     3363 2022-03-06 12:43:07.000000 pybiopax-0.1.5/pybiopax/paths.py
+-rw-r--r--   0 ben        (503) staff       (20)     3018 2024-05-10 20:40:50.000000 pybiopax-0.1.5/pybiopax/pc_client.py
+-rw-r--r--   0 ben        (503) staff       (20)        0 2023-02-09 04:17:55.000000 pybiopax-0.1.5/pybiopax/py.typed
+-rw-r--r--   0 ben        (503) staff       (20)     1409 2022-09-06 22:49:47.000000 pybiopax-0.1.5/pybiopax/references.py
+drwxr-xr-x   0 ben        (503) staff       (20)        0 2024-05-10 20:41:35.110164 pybiopax-0.1.5/pybiopax/tests/
+-rw-r--r--   0 ben        (503) staff       (20)        0 2022-03-06 12:43:07.000000 pybiopax-0.1.5/pybiopax/tests/__init__.py
+-rw-r--r--   0 ben        (503) staff       (20)  3623423 2022-03-06 12:43:07.000000 pybiopax-0.1.5/pybiopax/tests/biopax_test.owl.gz
+-rw-r--r--   0 ben        (503) staff       (20)     3244 2022-09-06 22:49:47.000000 pybiopax-0.1.5/pybiopax/tests/test_biopax.py
+-rw-r--r--   0 ben        (503) staff       (20)     2718 2022-03-06 12:43:07.000000 pybiopax-0.1.5/pybiopax/tests/test_paths.py
+-rw-r--r--   0 ben        (503) staff       (20)      470 2023-02-09 04:17:55.000000 pybiopax-0.1.5/pybiopax/tests/test_serialization.py
+-rw-r--r--   0 ben        (503) staff       (20)     3995 2022-03-06 12:43:07.000000 pybiopax-0.1.5/pybiopax/xml_util.py
+drwxr-xr-x   0 ben        (503) staff       (20)        0 2024-05-10 20:41:35.102118 pybiopax-0.1.5/pybiopax.egg-info/
+-rw-r--r--   0 ben        (503) staff       (20)     4634 2024-05-10 20:41:35.000000 pybiopax-0.1.5/pybiopax.egg-info/PKG-INFO
+-rw-r--r--   0 ben        (503) staff       (20)      864 2024-05-10 20:41:35.000000 pybiopax-0.1.5/pybiopax.egg-info/SOURCES.txt
+-rw-r--r--   0 ben        (503) staff       (20)        1 2024-05-10 20:41:35.000000 pybiopax-0.1.5/pybiopax.egg-info/dependency_links.txt
+-rw-r--r--   0 ben        (503) staff       (20)       19 2024-05-10 20:41:35.000000 pybiopax-0.1.5/pybiopax.egg-info/requires.txt
+-rw-r--r--   0 ben        (503) staff       (20)        9 2024-05-10 20:41:35.000000 pybiopax-0.1.5/pybiopax.egg-info/top_level.txt
+-rw-r--r--   0 ben        (503) staff       (20)      189 2022-03-06 12:43:07.000000 pybiopax-0.1.5/pyproject.toml
+-rw-r--r--   0 ben        (503) staff       (20)       38 2024-05-10 20:41:35.110651 pybiopax-0.1.5/setup.cfg
+-rw-r--r--   0 ben        (503) staff       (20)     1474 2022-03-06 12:43:07.000000 pybiopax-0.1.5/setup.py
```

### Comparing `pybiopax-0.1.4/LICENSE` & `pybiopax-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pybiopax-0.1.4/PKG-INFO` & `pybiopax-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybiopax
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python implementation of the BioPAX object model, and parts of PaxTools.
 Home-page: https://github.com/indralab/pybiopax
 Author: Benjamin M. Gyori, Harvard Medical School
 Author-email: benjamin_gyori@hms.harvard.edu
 Keywords: biology,pathway
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pybiopax-0.1.4/README.md` & `pybiopax-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pybiopax-0.1.4/doc/Makefile` & `pybiopax-0.1.5/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pybiopax-0.1.4/doc/conf.py` & `pybiopax-0.1.5/doc/conf.py`

 * *Files identical despite different names*

### Comparing `pybiopax-0.1.4/doc/make.bat` & `pybiopax-0.1.5/doc/make.bat`

 * *Files identical despite different names*

### Comparing `pybiopax-0.1.4/doc/modules/biopax.rst` & `pybiopax-0.1.5/doc/modules/biopax.rst`

 * *Files identical despite different names*

### Comparing `pybiopax-0.1.4/pybiopax/api.py` & `pybiopax-0.1.5/pybiopax/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,29 +51,35 @@
         A BioPAX Model deserialized from the OWL file.
     """
     with open(fname, 'r', encoding=encoding) as fh:
         owl_str = fh.read()
         return model_from_owl_str(owl_str)
 
 
-def model_from_owl_gz(path: Union[str, pathlib.Path, os.PathLike]) \
-        -> BioPaxModel:
+def model_from_owl_gz(
+    path: Union[str, pathlib.Path, os.PathLike],
+    encoding: Optional[str] = None,
+) -> BioPaxModel:
     """Return a BioPAX Model from an OWL file (gzipped).
 
     Parameters
     ----------
     path :
         A path to a gzipped OWL file of BioPAX content.
+    encoding :
+        The encoding to read the file with. Defaults to the
+        system default. Sometimes, windows users will need to
+        explicitly set this to utf-8.
 
     Returns
     -------
     :
         A BioPAX Model deserialized from the OWL file.
     """
-    with gzip.open(path, 'rt') as fh:
+    with gzip.open(path, 'rt', encoding=encoding) as fh:
         return BioPaxModel.from_xml(etree.parse(fh).getroot())
 
 
 def model_from_owl_gz_str(owl_gz_str: bytes) -> BioPaxModel:
     """Return a BioPAX Model from an OWL string.
 
     Parameters
```

### Comparing `pybiopax-0.1.4/pybiopax/biopax/base.py` & `pybiopax-0.1.5/pybiopax/biopax/base.py`

 * *Files identical despite different names*

### Comparing `pybiopax-0.1.4/pybiopax/biopax/interaction.py` & `pybiopax-0.1.5/pybiopax/biopax/interaction.py`

 * *Files identical despite different names*

### Comparing `pybiopax-0.1.4/pybiopax/biopax/model.py` & `pybiopax-0.1.5/pybiopax/biopax/model.py`

 * *Files identical despite different names*

### Comparing `pybiopax-0.1.4/pybiopax/biopax/physical_entity.py` & `pybiopax-0.1.5/pybiopax/biopax/physical_entity.py`

 * *Files identical despite different names*

### Comparing `pybiopax-0.1.4/pybiopax/biopax/util.py` & `pybiopax-0.1.5/pybiopax/biopax/util.py`

 * *Files identical despite different names*

### Comparing `pybiopax-0.1.4/pybiopax/paths.py` & `pybiopax-0.1.5/pybiopax/paths.py`

 * *Files identical despite different names*

### Comparing `pybiopax-0.1.4/pybiopax/pc_client.py` & `pybiopax-0.1.5/pybiopax/pc_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 the service, see the documentation at https://www.pathwaycommons.org/pc2/."""
 __all__ = ['graph_query']
 
 import logging
 import requests
 
 logger = logging.getLogger(__name__)
-pc2_url = 'http://www.pathwaycommons.org/pc2/'
+pc2_url = 'https://www.pathwaycommons.org/pc2/'
 
 
 def graph_query(kind, source, target=None, **query_params):
     """Perform a graph query on PathwayCommons.
 
     For more information on these queries, see
     http://www.pathwaycommons.org/pc2/#graph
```

### Comparing `pybiopax-0.1.4/pybiopax/references.py` & `pybiopax-0.1.5/pybiopax/references.py`

 * *Files identical despite different names*

### Comparing `pybiopax-0.1.4/pybiopax/tests/biopax_test.owl.gz` & `pybiopax-0.1.5/pybiopax/tests/biopax_test.owl.gz`

 * *Files identical despite different names*

### Comparing `pybiopax-0.1.4/pybiopax/tests/test_biopax.py` & `pybiopax-0.1.5/pybiopax/tests/test_biopax.py`

 * *Files identical despite different names*

### Comparing `pybiopax-0.1.4/pybiopax/tests/test_paths.py` & `pybiopax-0.1.5/pybiopax/tests/test_paths.py`

 * *Files identical despite different names*

### Comparing `pybiopax-0.1.4/pybiopax/xml_util.py` & `pybiopax-0.1.5/pybiopax/xml_util.py`

 * *Files identical despite different names*

### Comparing `pybiopax-0.1.4/pybiopax.egg-info/PKG-INFO` & `pybiopax-0.1.5/pybiopax.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybiopax
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python implementation of the BioPAX object model, and parts of PaxTools.
 Home-page: https://github.com/indralab/pybiopax
 Author: Benjamin M. Gyori, Harvard Medical School
 Author-email: benjamin_gyori@hms.harvard.edu
 Keywords: biology,pathway
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pybiopax-0.1.4/pybiopax.egg-info/SOURCES.txt` & `pybiopax-0.1.5/pybiopax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybiopax-0.1.4/setup.py` & `pybiopax-0.1.5/setup.py`

 * *Files identical despite different names*

