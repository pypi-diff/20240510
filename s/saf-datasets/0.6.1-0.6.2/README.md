# Comparing `tmp/saf_datasets-0.6.1.tar.gz` & `tmp/saf_datasets-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saf_datasets-0.6.1.tar", last modified: Wed May  8 18:49:28 2024, max compression
+gzip compressed data, was "saf_datasets-0.6.2.tar", last modified: Fri May 10 05:53:32 2024, max compression
```

## Comparing `saf_datasets-0.6.1.tar` & `saf_datasets-0.6.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-08 18:49:28.328628 saf_datasets-0.6.1/
--rw-------   0 dsilvadecarvalho   (505) staff       (20)    35149 2023-03-15 12:32:16.000000 saf_datasets-0.6.1/LICENSE
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     4322 2024-05-08 18:49:28.328457 saf_datasets-0.6.1/PKG-INFO
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     3491 2024-05-08 18:45:21.000000 saf_datasets-0.6.1/README.md
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      671 2024-05-08 18:47:45.000000 saf_datasets-0.6.1/pyproject.toml
--rw-------   0 dsilvadecarvalho   (505) staff       (20)       77 2024-05-08 14:09:52.000000 saf_datasets-0.6.1/requirements.txt
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-08 18:49:28.323305 saf_datasets-0.6.1/saf_datasets/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      420 2024-02-12 18:30:07.000000 saf_datasets-0.6.1/saf_datasets/__init__.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-08 18:49:28.325322 saf_datasets-0.6.1/saf_datasets/annotators/
--rw-------   0 dsilvadecarvalho   (505) staff       (20)       80 2024-04-22 11:09:48.000000 saf_datasets-0.6.1/saf_datasets/annotators/__init__.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     1362 2024-05-08 15:57:27.000000 saf_datasets-0.6.1/saf_datasets/annotators/allennlp_srl.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)      165 2023-11-29 15:12:10.000000 saf_datasets-0.6.1/saf_datasets/annotators/models.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)     1088 2024-05-08 16:03:49.000000 saf_datasets-0.6.1/saf_datasets/annotators/spacy.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)     4742 2024-05-08 16:14:10.000000 saf_datasets-0.6.1/saf_datasets/annotators/transformer.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-08 18:49:28.327370 saf_datasets-0.6.1/saf_datasets/data_access/
--rw-------   0 dsilvadecarvalho   (505) staff       (20)        0 2023-03-13 13:13:57.000000 saf_datasets-0.6.1/saf_datasets/data_access/__init__.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)     1941 2024-05-08 15:54:57.000000 saf_datasets-0.6.1/saf_datasets/data_access/allnli.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)     5375 2024-05-08 15:28:33.000000 saf_datasets-0.6.1/saf_datasets/data_access/codwoe.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)     1907 2024-05-08 15:32:04.000000 saf_datasets-0.6.1/saf_datasets/data_access/cpae.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)    12727 2024-05-08 14:56:10.000000 saf_datasets-0.6.1/saf_datasets/data_access/dataset.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)     2922 2024-05-08 15:37:48.000000 saf_datasets-0.6.1/saf_datasets/data_access/entailmentbank.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     2608 2024-05-08 17:18:08.000000 saf_datasets-0.6.1/saf_datasets/data_access/stsb.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     8793 2024-05-08 15:08:33.000000 saf_datasets-0.6.1/saf_datasets/data_access/wiktionary.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     4059 2024-05-08 15:14:59.000000 saf_datasets-0.6.1/saf_datasets/data_access/wordnet_filtered.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-08 18:49:28.327960 saf_datasets-0.6.1/saf_datasets/wrappers/
--rw-------   0 dsilvadecarvalho   (505) staff       (20)        0 2023-11-13 14:11:53.000000 saf_datasets-0.6.1/saf_datasets/wrappers/__init__.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)      793 2024-05-08 15:45:05.000000 saf_datasets-0.6.1/saf_datasets/wrappers/hf.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     2062 2024-05-08 15:51:39.000000 saf_datasets-0.6.1/saf_datasets/wrappers/torch.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-08 18:49:28.328250 saf_datasets-0.6.1/saf_datasets.egg-info/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     4322 2024-05-08 18:49:28.000000 saf_datasets-0.6.1/saf_datasets.egg-info/PKG-INFO
--rw-------   0 dsilvadecarvalho   (505) staff       (20)      873 2024-05-08 18:49:28.000000 saf_datasets-0.6.1/saf_datasets.egg-info/SOURCES.txt
--rw-------   0 dsilvadecarvalho   (505) staff       (20)        1 2024-05-08 18:49:28.000000 saf_datasets-0.6.1/saf_datasets.egg-info/dependency_links.txt
--rw-------   0 dsilvadecarvalho   (505) staff       (20)       77 2024-05-08 18:49:28.000000 saf_datasets-0.6.1/saf_datasets.egg-info/requires.txt
--rw-------   0 dsilvadecarvalho   (505) staff       (20)       13 2024-05-08 18:49:28.000000 saf_datasets-0.6.1/saf_datasets.egg-info/top_level.txt
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       38 2024-05-08 18:49:28.328670 saf_datasets-0.6.1/setup.cfg
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      815 2024-05-08 18:47:46.000000 saf_datasets-0.6.1/setup.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-10 05:53:32.031966 saf_datasets-0.6.2/
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)    35149 2023-03-15 12:32:16.000000 saf_datasets-0.6.2/LICENSE
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     4322 2024-05-10 05:53:32.031690 saf_datasets-0.6.2/PKG-INFO
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     3491 2024-05-08 18:45:21.000000 saf_datasets-0.6.2/README.md
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      671 2024-05-09 14:05:21.000000 saf_datasets-0.6.2/pyproject.toml
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)       77 2024-05-08 14:09:52.000000 saf_datasets-0.6.2/requirements.txt
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-10 05:53:32.022665 saf_datasets-0.6.2/saf_datasets/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      366 2024-05-09 14:03:38.000000 saf_datasets-0.6.2/saf_datasets/__init__.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-10 05:53:32.025968 saf_datasets-0.6.2/saf_datasets/annotators/
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)       80 2024-04-22 11:09:48.000000 saf_datasets-0.6.2/saf_datasets/annotators/__init__.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     1362 2024-05-08 15:57:27.000000 saf_datasets-0.6.2/saf_datasets/annotators/allennlp_srl.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)      165 2023-11-29 15:12:10.000000 saf_datasets-0.6.2/saf_datasets/annotators/models.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)     1088 2024-05-08 16:03:49.000000 saf_datasets-0.6.2/saf_datasets/annotators/spacy.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)     4742 2024-05-08 16:14:10.000000 saf_datasets-0.6.2/saf_datasets/annotators/transformer.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-10 05:53:32.029623 saf_datasets-0.6.2/saf_datasets/data_access/
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)        0 2023-03-13 13:13:57.000000 saf_datasets-0.6.2/saf_datasets/data_access/__init__.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)     1941 2024-05-08 15:54:57.000000 saf_datasets-0.6.2/saf_datasets/data_access/allnli.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)     5375 2024-05-08 15:28:33.000000 saf_datasets-0.6.2/saf_datasets/data_access/codwoe.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)     1907 2024-05-08 15:32:04.000000 saf_datasets-0.6.2/saf_datasets/data_access/cpae.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)    12727 2024-05-08 14:56:10.000000 saf_datasets-0.6.2/saf_datasets/data_access/dataset.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)     2922 2024-05-08 15:37:48.000000 saf_datasets-0.6.2/saf_datasets/data_access/entailmentbank.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     2608 2024-05-08 17:18:08.000000 saf_datasets-0.6.2/saf_datasets/data_access/stsb.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     8793 2024-05-08 15:08:33.000000 saf_datasets-0.6.2/saf_datasets/data_access/wiktionary.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     4059 2024-05-08 15:14:59.000000 saf_datasets-0.6.2/saf_datasets/data_access/wordnet_filtered.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-10 05:53:32.030711 saf_datasets-0.6.2/saf_datasets/wrappers/
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)        0 2023-11-13 14:11:53.000000 saf_datasets-0.6.2/saf_datasets/wrappers/__init__.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)      793 2024-05-08 15:45:05.000000 saf_datasets-0.6.2/saf_datasets/wrappers/hf.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     2062 2024-05-08 15:51:39.000000 saf_datasets-0.6.2/saf_datasets/wrappers/torch.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-10 05:53:32.031332 saf_datasets-0.6.2/saf_datasets.egg-info/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     4322 2024-05-10 05:53:32.000000 saf_datasets-0.6.2/saf_datasets.egg-info/PKG-INFO
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)      873 2024-05-10 05:53:32.000000 saf_datasets-0.6.2/saf_datasets.egg-info/SOURCES.txt
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)        1 2024-05-10 05:53:32.000000 saf_datasets-0.6.2/saf_datasets.egg-info/dependency_links.txt
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)       77 2024-05-10 05:53:32.000000 saf_datasets-0.6.2/saf_datasets.egg-info/requires.txt
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)       13 2024-05-10 05:53:32.000000 saf_datasets-0.6.2/saf_datasets.egg-info/top_level.txt
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       38 2024-05-10 05:53:32.032025 saf_datasets-0.6.2/setup.cfg
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      815 2024-05-09 14:05:21.000000 saf_datasets-0.6.2/setup.py
```

### Comparing `saf_datasets-0.6.1/LICENSE` & `saf_datasets-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.1/PKG-INFO` & `saf_datasets-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saf-datasets
-Version: 0.6.1
+Version: 0.6.2
 Summary: Data set loading and annotation facilities for the Simple Annotation Framework
 Home-page: 
 Author: Danilo S. Carvalho
 Author-email: "Danilo S. Carvalho" <danilo.carvalho@manchester.ac.uk>
 Project-URL: Homepage, https://github.com/neuro-symbolic-ai/saf_datasets
 Project-URL: Issues, https://github.com/neuro-symbolic-ai/saf_datasets/issues
 Keywords: datasets,annotated,nlp
```

### Comparing `saf_datasets-0.6.1/README.md` & `saf_datasets-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.1/pyproject.toml` & `saf_datasets-0.6.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "saf-datasets"
-version = "0.6.1"
+version = "0.6.2"
 authors = [
   { name="Danilo S. Carvalho", email="danilo.carvalho@manchester.ac.uk" }
 ]
 description = "Data set loading and annotation facilities for the Simple Annotation Framework"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `saf_datasets-0.6.1/saf_datasets/annotators/allennlp_srl.py` & `saf_datasets-0.6.2/saf_datasets/annotators/allennlp_srl.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.1/saf_datasets/annotators/spacy.py` & `saf_datasets-0.6.2/saf_datasets/annotators/spacy.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.1/saf_datasets/annotators/transformer.py` & `saf_datasets-0.6.2/saf_datasets/annotators/transformer.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.1/saf_datasets/data_access/allnli.py` & `saf_datasets-0.6.2/saf_datasets/data_access/allnli.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.1/saf_datasets/data_access/codwoe.py` & `saf_datasets-0.6.2/saf_datasets/data_access/codwoe.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.1/saf_datasets/data_access/cpae.py` & `saf_datasets-0.6.2/saf_datasets/data_access/cpae.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.1/saf_datasets/data_access/dataset.py` & `saf_datasets-0.6.2/saf_datasets/data_access/dataset.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.1/saf_datasets/data_access/entailmentbank.py` & `saf_datasets-0.6.2/saf_datasets/data_access/entailmentbank.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.1/saf_datasets/data_access/stsb.py` & `saf_datasets-0.6.2/saf_datasets/data_access/stsb.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.1/saf_datasets/data_access/wiktionary.py` & `saf_datasets-0.6.2/saf_datasets/data_access/wiktionary.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.1/saf_datasets/data_access/wordnet_filtered.py` & `saf_datasets-0.6.2/saf_datasets/data_access/wordnet_filtered.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.1/saf_datasets/wrappers/hf.py` & `saf_datasets-0.6.2/saf_datasets/wrappers/hf.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.1/saf_datasets/wrappers/torch.py` & `saf_datasets-0.6.2/saf_datasets/wrappers/torch.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.1/saf_datasets.egg-info/PKG-INFO` & `saf_datasets-0.6.2/saf_datasets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saf-datasets
-Version: 0.6.1
+Version: 0.6.2
 Summary: Data set loading and annotation facilities for the Simple Annotation Framework
 Home-page: 
 Author: Danilo S. Carvalho
 Author-email: "Danilo S. Carvalho" <danilo.carvalho@manchester.ac.uk>
 Project-URL: Homepage, https://github.com/neuro-symbolic-ai/saf_datasets
 Project-URL: Issues, https://github.com/neuro-symbolic-ai/saf_datasets/issues
 Keywords: datasets,annotated,nlp
```

### Comparing `saf_datasets-0.6.1/saf_datasets.egg-info/SOURCES.txt` & `saf_datasets-0.6.2/saf_datasets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

