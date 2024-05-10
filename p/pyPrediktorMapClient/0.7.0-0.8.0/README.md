# Comparing `tmp/pyPrediktorMapClient-0.7.0.tar.gz` & `tmp/pyPrediktorMapClient-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPrediktorMapClient-0.7.0.tar", last modified: Tue Sep 13 06:19:22 2022, max compression
+gzip compressed data, was "pyPrediktorMapClient-0.8.0.tar", last modified: Tue Sep 13 12:12:58 2022, max compression
```

## Comparing `pyPrediktorMapClient-0.7.0.tar` & `pyPrediktorMapClient-0.8.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 andreaslydersen   (501) staff       (20)        0 2022-09-13 06:19:22.732471 pyPrediktorMapClient-0.7.0/
--rw-r--r--   0 andreaslydersen   (501) staff       (20)      603 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.7.0/.coveragerc
-drwxr-xr-x   0 andreaslydersen   (501) staff       (20)        0 2022-09-13 06:19:22.725120 pyPrediktorMapClient-0.7.0/.github/
-drwxr-xr-x   0 andreaslydersen   (501) staff       (20)        0 2022-09-13 06:19:22.728489 pyPrediktorMapClient-0.7.0/.github/workflows/
--rw-r--r--   0 andreaslydersen   (501) staff       (20)     2728 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.7.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 andreaslydersen   (501) staff       (20)      476 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.7.0/.github/workflows/pages.yml
--rw-r--r--   0 andreaslydersen   (501) staff       (20)      604 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.7.0/.gitignore
--rw-r--r--   0 andreaslydersen   (501) staff       (20)      490 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.7.0/.readthedocs.yml
--rw-r--r--   0 andreaslydersen   (501) staff       (20)      118 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.7.0/AUTHORS.rst
--rw-r--r--   0 andreaslydersen   (501) staff       (20)      351 2022-09-12 19:57:51.000000 pyPrediktorMapClient-0.7.0/CHANGELOG.rst
--rw-r--r--   0 andreaslydersen   (501) staff       (20)    11859 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.7.0/CONTRIBUTING.rst
--rw-r--r--   0 andreaslydersen   (501) staff       (20)     1076 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.7.0/LICENSE.txt
--rw-r--r--   0 andreaslydersen   (501) staff       (20)     1464 2022-09-13 06:19:22.732566 pyPrediktorMapClient-0.7.0/PKG-INFO
--rw-r--r--   0 andreaslydersen   (501) staff       (20)      969 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.7.0/README.md
--rw-r--r--   0 andreaslydersen   (501) staff       (20)      657 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.7.0/README.rst
--rw-r--r--   0 andreaslydersen   (501) staff       (20)      170 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.7.0/TODO.md
-drwxr-xr-x   0 andreaslydersen   (501) staff       (20)        0 2022-09-13 06:19:22.729861 pyPrediktorMapClient-0.7.0/docs/
--rw-r--r--   0 andreaslydersen   (501) staff       (20)        0 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.7.0/docs/.nojekyll
--rw-r--r--   0 andreaslydersen   (501) staff       (20)     1154 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.7.0/docs/Makefile
-drwxr-xr-x   0 andreaslydersen   (501) staff       (20)        0 2022-09-13 06:19:22.730004 pyPrediktorMapClient-0.7.0/docs/_static/
--rw-r--r--   0 andreaslydersen   (501) staff       (20)       18 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.7.0/docs/_static/.gitignore
--rw-r--r--   0 andreaslydersen   (501) staff       (20)       41 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.7.0/docs/authors.rst
--rw-r--r--   0 andreaslydersen   (501) staff       (20)       43 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.7.0/docs/changelog.rst
--rw-r--r--   0 andreaslydersen   (501) staff       (20)     9871 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.7.0/docs/conf.py
--rw-r--r--   0 andreaslydersen   (501) staff       (20)       33 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.7.0/docs/contributing.rst
--rw-r--r--   0 andreaslydersen   (501) staff       (20)     1449 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.7.0/docs/index.rst
--rw-r--r--   0 andreaslydersen   (501) staff       (20)       67 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.7.0/docs/license.rst
--rw-r--r--   0 andreaslydersen   (501) staff       (20)       39 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.7.0/docs/readme.rst
--rw-r--r--   0 andreaslydersen   (501) staff       (20)      233 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.7.0/docs/requirements.txt
-drwxr-xr-x   0 andreaslydersen   (501) staff       (20)        0 2022-09-13 06:19:22.730294 pyPrediktorMapClient-0.7.0/notebooks/
--rw-r--r--   0 andreaslydersen   (501) staff       (20)     9116 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.7.0/notebooks/Example_Data_Downloading.ipynb
--rw-r--r--   0 andreaslydersen   (501) staff       (20)     7047 2022-09-13 06:16:49.000000 pyPrediktorMapClient-0.7.0/notebooks/Exploring_API_Functions.ipynb
--rw-r--r--   0 andreaslydersen   (501) staff       (20)      345 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.7.0/pyproject.toml
--rw-r--r--   0 andreaslydersen   (501) staff       (20)       21 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.7.0/requirements.txt
--rw-r--r--   0 andreaslydersen   (501) staff       (20)     1562 2022-09-13 06:19:22.732971 pyPrediktorMapClient-0.7.0/setup.cfg
--rw-r--r--   0 andreaslydersen   (501) staff       (20)      715 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.7.0/setup.py
-drwxr-xr-x   0 andreaslydersen   (501) staff       (20)        0 2022-09-13 06:19:22.725536 pyPrediktorMapClient-0.7.0/src/
-drwxr-xr-x   0 andreaslydersen   (501) staff       (20)        0 2022-09-13 06:19:22.731349 pyPrediktorMapClient-0.7.0/src/pyPrediktorMapClient.egg-info/
--rw-r--r--   0 andreaslydersen   (501) staff       (20)     1464 2022-09-13 06:19:22.000000 pyPrediktorMapClient-0.7.0/src/pyPrediktorMapClient.egg-info/PKG-INFO
--rw-r--r--   0 andreaslydersen   (501) staff       (20)      995 2022-09-13 06:19:22.000000 pyPrediktorMapClient-0.7.0/src/pyPrediktorMapClient.egg-info/SOURCES.txt
--rw-r--r--   0 andreaslydersen   (501) staff       (20)        1 2022-09-13 06:19:22.000000 pyPrediktorMapClient-0.7.0/src/pyPrediktorMapClient.egg-info/dependency_links.txt
--rw-r--r--   0 andreaslydersen   (501) staff       (20)        1 2022-09-12 09:11:54.000000 pyPrediktorMapClient-0.7.0/src/pyPrediktorMapClient.egg-info/not-zip-safe
--rw-r--r--   0 andreaslydersen   (501) staff       (20)      149 2022-09-13 06:19:22.000000 pyPrediktorMapClient-0.7.0/src/pyPrediktorMapClient.egg-info/requires.txt
--rw-r--r--   0 andreaslydersen   (501) staff       (20)       21 2022-09-13 06:19:22.000000 pyPrediktorMapClient-0.7.0/src/pyPrediktorMapClient.egg-info/top_level.txt
-drwxr-xr-x   0 andreaslydersen   (501) staff       (20)        0 2022-09-13 06:19:22.732148 pyPrediktorMapClient-0.7.0/src/pyprediktormapclient/
--rw-r--r--   0 andreaslydersen   (501) staff       (20)      683 2022-09-12 19:57:51.000000 pyPrediktorMapClient-0.7.0/src/pyprediktormapclient/__init__.py
--rw-r--r--   0 andreaslydersen   (501) staff       (20)     4724 2022-09-13 06:16:49.000000 pyPrediktorMapClient-0.7.0/src/pyprediktormapclient/model_index.py
--rw-r--r--   0 andreaslydersen   (501) staff       (20)    13425 2022-09-12 19:57:51.000000 pyPrediktorMapClient-0.7.0/src/pyprediktormapclient/opc_ua.py
--rw-r--r--   0 andreaslydersen   (501) staff       (20)      875 2022-09-12 19:57:51.000000 pyPrediktorMapClient-0.7.0/src/pyprediktormapclient/pyprediktormapclient_shared.py
-drwxr-xr-x   0 andreaslydersen   (501) staff       (20)        0 2022-09-13 06:19:22.732336 pyPrediktorMapClient-0.7.0/tests/
--rw-r--r--   0 andreaslydersen   (501) staff       (20)      288 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.7.0/tests/conftest.py
--rw-r--r--   0 andreaslydersen   (501) staff       (20)     2665 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.7.0/tox.ini
+drwxr-xr-x   0 andreaslydersen   (501) staff       (20)        0 2022-09-13 12:12:58.810178 pyPrediktorMapClient-0.8.0/
+-rw-r--r--   0 andreaslydersen   (501) staff       (20)      603 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.8.0/.coveragerc
+drwxr-xr-x   0 andreaslydersen   (501) staff       (20)        0 2022-09-13 12:12:58.803417 pyPrediktorMapClient-0.8.0/.github/
+drwxr-xr-x   0 andreaslydersen   (501) staff       (20)        0 2022-09-13 12:12:58.806888 pyPrediktorMapClient-0.8.0/.github/workflows/
+-rw-r--r--   0 andreaslydersen   (501) staff       (20)     2728 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.8.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 andreaslydersen   (501) staff       (20)      476 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.8.0/.github/workflows/pages.yml
+-rw-r--r--   0 andreaslydersen   (501) staff       (20)      604 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.8.0/.gitignore
+-rw-r--r--   0 andreaslydersen   (501) staff       (20)      490 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.8.0/.readthedocs.yml
+-rw-r--r--   0 andreaslydersen   (501) staff       (20)      118 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.8.0/AUTHORS.rst
+-rw-r--r--   0 andreaslydersen   (501) staff       (20)      351 2022-09-12 19:57:51.000000 pyPrediktorMapClient-0.8.0/CHANGELOG.rst
+-rw-r--r--   0 andreaslydersen   (501) staff       (20)    11859 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.8.0/CONTRIBUTING.rst
+-rw-r--r--   0 andreaslydersen   (501) staff       (20)     1076 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.8.0/LICENSE.txt
+-rw-r--r--   0 andreaslydersen   (501) staff       (20)     1464 2022-09-13 12:12:58.810269 pyPrediktorMapClient-0.8.0/PKG-INFO
+-rw-r--r--   0 andreaslydersen   (501) staff       (20)      969 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.8.0/README.md
+-rw-r--r--   0 andreaslydersen   (501) staff       (20)      657 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.8.0/README.rst
+-rw-r--r--   0 andreaslydersen   (501) staff       (20)      170 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.8.0/TODO.md
+drwxr-xr-x   0 andreaslydersen   (501) staff       (20)        0 2022-09-13 12:12:58.808154 pyPrediktorMapClient-0.8.0/docs/
+-rw-r--r--   0 andreaslydersen   (501) staff       (20)        0 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.8.0/docs/.nojekyll
+-rw-r--r--   0 andreaslydersen   (501) staff       (20)     1154 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.8.0/docs/Makefile
+drwxr-xr-x   0 andreaslydersen   (501) staff       (20)        0 2022-09-13 12:12:58.808284 pyPrediktorMapClient-0.8.0/docs/_static/
+-rw-r--r--   0 andreaslydersen   (501) staff       (20)       18 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.8.0/docs/_static/.gitignore
+-rw-r--r--   0 andreaslydersen   (501) staff       (20)       41 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.8.0/docs/authors.rst
+-rw-r--r--   0 andreaslydersen   (501) staff       (20)       43 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.8.0/docs/changelog.rst
+-rw-r--r--   0 andreaslydersen   (501) staff       (20)     9871 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.8.0/docs/conf.py
+-rw-r--r--   0 andreaslydersen   (501) staff       (20)       33 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.8.0/docs/contributing.rst
+-rw-r--r--   0 andreaslydersen   (501) staff       (20)     1449 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.8.0/docs/index.rst
+-rw-r--r--   0 andreaslydersen   (501) staff       (20)       67 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.8.0/docs/license.rst
+-rw-r--r--   0 andreaslydersen   (501) staff       (20)       39 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.8.0/docs/readme.rst
+-rw-r--r--   0 andreaslydersen   (501) staff       (20)      233 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.8.0/docs/requirements.txt
+drwxr-xr-x   0 andreaslydersen   (501) staff       (20)        0 2022-09-13 12:12:58.808561 pyPrediktorMapClient-0.8.0/notebooks/
+-rw-r--r--   0 andreaslydersen   (501) staff       (20)     9116 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.8.0/notebooks/Example_Data_Downloading.ipynb
+-rw-r--r--   0 andreaslydersen   (501) staff       (20)     7199 2022-09-13 11:14:59.000000 pyPrediktorMapClient-0.8.0/notebooks/Exploring_API_Functions.ipynb
+-rw-r--r--   0 andreaslydersen   (501) staff       (20)      345 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.8.0/pyproject.toml
+-rw-r--r--   0 andreaslydersen   (501) staff       (20)       21 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.8.0/requirements.txt
+-rw-r--r--   0 andreaslydersen   (501) staff       (20)     1562 2022-09-13 12:12:58.810651 pyPrediktorMapClient-0.8.0/setup.cfg
+-rw-r--r--   0 andreaslydersen   (501) staff       (20)      715 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.8.0/setup.py
+drwxr-xr-x   0 andreaslydersen   (501) staff       (20)        0 2022-09-13 12:12:58.803766 pyPrediktorMapClient-0.8.0/src/
+drwxr-xr-x   0 andreaslydersen   (501) staff       (20)        0 2022-09-13 12:12:58.809362 pyPrediktorMapClient-0.8.0/src/pyPrediktorMapClient.egg-info/
+-rw-r--r--   0 andreaslydersen   (501) staff       (20)     1464 2022-09-13 12:12:58.000000 pyPrediktorMapClient-0.8.0/src/pyPrediktorMapClient.egg-info/PKG-INFO
+-rw-r--r--   0 andreaslydersen   (501) staff       (20)      974 2022-09-13 12:12:58.000000 pyPrediktorMapClient-0.8.0/src/pyPrediktorMapClient.egg-info/SOURCES.txt
+-rw-r--r--   0 andreaslydersen   (501) staff       (20)        1 2022-09-13 12:12:58.000000 pyPrediktorMapClient-0.8.0/src/pyPrediktorMapClient.egg-info/dependency_links.txt
+-rw-r--r--   0 andreaslydersen   (501) staff       (20)        1 2022-09-12 09:11:54.000000 pyPrediktorMapClient-0.8.0/src/pyPrediktorMapClient.egg-info/not-zip-safe
+-rw-r--r--   0 andreaslydersen   (501) staff       (20)      149 2022-09-13 12:12:58.000000 pyPrediktorMapClient-0.8.0/src/pyPrediktorMapClient.egg-info/requires.txt
+-rw-r--r--   0 andreaslydersen   (501) staff       (20)       21 2022-09-13 12:12:58.000000 pyPrediktorMapClient-0.8.0/src/pyPrediktorMapClient.egg-info/top_level.txt
+drwxr-xr-x   0 andreaslydersen   (501) staff       (20)        0 2022-09-13 12:12:58.809845 pyPrediktorMapClient-0.8.0/src/pyprediktormapclient/
+-rw-r--r--   0 andreaslydersen   (501) staff       (20)      662 2022-09-13 11:14:59.000000 pyPrediktorMapClient-0.8.0/src/pyprediktormapclient/__init__.py
+-rw-r--r--   0 andreaslydersen   (501) staff       (20)     4724 2022-09-13 11:14:59.000000 pyPrediktorMapClient-0.8.0/src/pyprediktormapclient/model_index.py
+-rw-r--r--   0 andreaslydersen   (501) staff       (20)    13425 2022-09-13 11:14:59.000000 pyPrediktorMapClient-0.8.0/src/pyprediktormapclient/opc_ua.py
+-rw-r--r--   0 andreaslydersen   (501) staff       (20)      875 2022-09-13 11:14:59.000000 pyPrediktorMapClient-0.8.0/src/pyprediktormapclient/shared.py
+drwxr-xr-x   0 andreaslydersen   (501) staff       (20)        0 2022-09-13 12:12:58.809970 pyPrediktorMapClient-0.8.0/tests/
+-rw-r--r--   0 andreaslydersen   (501) staff       (20)      288 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.8.0/tests/conftest.py
+-rw-r--r--   0 andreaslydersen   (501) staff       (20)     2665 2022-09-12 09:11:00.000000 pyPrediktorMapClient-0.8.0/tox.ini
```

### Comparing `pyPrediktorMapClient-0.7.0/.coveragerc` & `pyPrediktorMapClient-0.8.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `pyPrediktorMapClient-0.7.0/.github/workflows/codeql-analysis.yml` & `pyPrediktorMapClient-0.8.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `pyPrediktorMapClient-0.7.0/.gitignore` & `pyPrediktorMapClient-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyPrediktorMapClient-0.7.0/CONTRIBUTING.rst` & `pyPrediktorMapClient-0.8.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyPrediktorMapClient-0.7.0/LICENSE.txt` & `pyPrediktorMapClient-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyPrediktorMapClient-0.7.0/PKG-INFO` & `pyPrediktorMapClient-0.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPrediktorMapClient
-Version: 0.7.0
+Version: 0.8.0
 Summary: Helper functions for Prediktor Map Services
 Home-page: https://github.com/PrediktorAS/pyPrediktorMapClient
 Author: Prediktor
 Author-email: support@prediktor.com
 License: MIT
 Project-URL: Documentation, https://prediktoras.github.io/pyPrediktorMapClient/
 Project-URL: Source, https://github.com/PrediktorAS/pyPrediktorMapClient
```

### Comparing `pyPrediktorMapClient-0.7.0/README.md` & `pyPrediktorMapClient-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pyPrediktorMapClient-0.7.0/README.rst` & `pyPrediktorMapClient-0.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `pyPrediktorMapClient-0.7.0/docs/Makefile` & `pyPrediktorMapClient-0.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyPrediktorMapClient-0.7.0/docs/conf.py` & `pyPrediktorMapClient-0.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyPrediktorMapClient-0.7.0/docs/index.rst` & `pyPrediktorMapClient-0.8.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyPrediktorMapClient-0.7.0/notebooks/Example_Data_Downloading.ipynb` & `pyPrediktorMapClient-0.8.0/notebooks/Example_Data_Downloading.ipynb`

 * *Files identical despite different names*

### Comparing `pyPrediktorMapClient-0.7.0/notebooks/Exploring_API_Functions.ipynb` & `pyPrediktorMapClient-0.8.0/notebooks/Exploring_API_Functions.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994565217391305%*

 * *Differences: {"'cells'": "{4: {'source': {insert: [(0, '# Setting the path is only needed if you are running "*

 * *            "this locally from source.\\n'), (1, '# Consider using pip to install instead.\\n')], "*

 * *            "delete: [0]}}, 5: {'source': {insert: [(1, 'from pyprediktormapclient.model_index "*

 * *            "import ModelIndex\\n'), (4, 'from pyprediktormapclient.opc_ua import OPC_UA')], "*

 * *            'delete: [4, 1]}}}'}*

```diff
@@ -37,32 +37,33 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# Setting the path\n",
+                "# Setting the path is only needed if you are running this locally from source.\n",
+                "# Consider using pip to install instead.\n",
                 "module_path = os.path.abspath(os.path.join(\"../src/pyprediktormapclient/\"))\n",
                 "print(module_path)\n",
                 "if module_path not in sys.path:\n",
                 "    sys.path.append(module_path)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Import model index functions\n",
-                "from model_index import ModelIndex\n",
+                "from pyprediktormapclient.model_index import ModelIndex\n",
                 "\n",
                 "# Import OPC UA functions\n",
-                "from opc_ua import OPC_UA"
+                "from pyprediktormapclient.opc_ua import OPC_UA"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `pyPrediktorMapClient-0.7.0/setup.cfg` & `pyPrediktorMapClient-0.8.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyPrediktorMapClient-0.7.0/setup.py` & `pyPrediktorMapClient-0.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `pyPrediktorMapClient-0.7.0/src/pyPrediktorMapClient.egg-info/PKG-INFO` & `pyPrediktorMapClient-0.8.0/src/pyPrediktorMapClient.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPrediktorMapClient
-Version: 0.7.0
+Version: 0.8.0
 Summary: Helper functions for Prediktor Map Services
 Home-page: https://github.com/PrediktorAS/pyPrediktorMapClient
 Author: Prediktor
 Author-email: support@prediktor.com
 License: MIT
 Project-URL: Documentation, https://prediktoras.github.io/pyPrediktorMapClient/
 Project-URL: Source, https://github.com/PrediktorAS/pyPrediktorMapClient
```

### Comparing `pyPrediktorMapClient-0.7.0/src/pyPrediktorMapClient.egg-info/SOURCES.txt` & `pyPrediktorMapClient-0.8.0/src/pyPrediktorMapClient.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -33,9 +33,9 @@
 src/pyPrediktorMapClient.egg-info/dependency_links.txt
 src/pyPrediktorMapClient.egg-info/not-zip-safe
 src/pyPrediktorMapClient.egg-info/requires.txt
 src/pyPrediktorMapClient.egg-info/top_level.txt
 src/pyprediktormapclient/__init__.py
 src/pyprediktormapclient/model_index.py
 src/pyprediktormapclient/opc_ua.py
-src/pyprediktormapclient/pyprediktormapclient_shared.py
+src/pyprediktormapclient/shared.py
 tests/conftest.py
```

### Comparing `pyPrediktorMapClient-0.7.0/src/pyprediktormapclient/__init__.py` & `pyPrediktorMapClient-0.8.0/src/pyprediktormapclient/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import sys
-from .pyprediktormapclient_shared import *
+from .shared import *
 from .model_index import *
 from .opc_ua import *
 
 if sys.version_info[:2] >= (3, 8):
     # TODO: Import directly (no need for conditional) when `python_requires = >= 3.8`
     from importlib.metadata import PackageNotFoundError, version  # pragma: no cover
 else:
```

### Comparing `pyPrediktorMapClient-0.7.0/src/pyprediktormapclient/model_index.py` & `pyPrediktorMapClient-0.8.0/src/pyprediktormapclient/model_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import pandas as pd
 from pydantic import BaseModel, HttpUrl
-from pyprediktormapclient_shared import request_from_api
+from pyprediktormapclient.shared import request_from_api
 
 class RESTUrls(BaseModel):
     rest_url: HttpUrl
 
 class ModelIndex:
     """Data structure from the model index API server
     """
```

### Comparing `pyPrediktorMapClient-0.7.0/src/pyprediktormapclient/opc_ua.py` & `pyPrediktorMapClient-0.8.0/src/pyprediktormapclient/opc_ua.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import numpy as np
 import itertools
 from pathlib import Path
 import asyncio
 from typing import Dict, List
 from aiohttp import ClientSession
 from pydantic import BaseModel, HttpUrl, AnyUrl
-from pyprediktormapclient_shared import request_from_api
+from pyprediktormapclient.shared import request_from_api
 
 class OPCUrls(BaseModel):
     rest_url: HttpUrl
     opcua_url: AnyUrl
 
 
 class OPC_UA:
```

### Comparing `pyPrediktorMapClient-0.7.0/src/pyprediktormapclient/pyprediktormapclient_shared.py` & `pyPrediktorMapClient-0.8.0/src/pyprediktormapclient/shared.py`

 * *Files identical despite different names*

### Comparing `pyPrediktorMapClient-0.7.0/tox.ini` & `pyPrediktorMapClient-0.8.0/tox.ini`

 * *Files identical despite different names*

