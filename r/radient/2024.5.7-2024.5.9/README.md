# Comparing `tmp/radient-2024.5.7.tar.gz` & `tmp/radient-2024.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radient-2024.5.7.tar", last modified: Wed May  8 05:58:34 2024, max compression
+gzip compressed data, was "radient-2024.5.9.tar", last modified: Fri May 10 07:24:41 2024, max compression
```

## Comparing `radient-2024.5.7.tar` & `radient-2024.5.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 zilliz     (501) staff       (20)        0 2024-05-08 05:58:34.349063 radient-2024.5.7/
--rw-r--r--   0 zilliz     (501) staff       (20)     1266 2024-05-08 04:55:23.000000 radient-2024.5.7/LICENSE
--rw-r--r--   0 zilliz     (501) staff       (20)     4068 2024-05-08 05:58:34.348594 radient-2024.5.7/PKG-INFO
--rw-r--r--   0 zilliz     (501) staff       (20)     3594 2024-05-08 04:59:54.000000 radient-2024.5.7/README.md
--rw-r--r--   0 zilliz     (501) staff       (20)      472 2024-05-08 05:58:18.000000 radient-2024.5.7/pyproject.toml
-drwxr-xr-x   0 zilliz     (501) staff       (20)        0 2024-05-08 05:58:34.321150 radient-2024.5.7/radient/
--rw-r--r--   0 zilliz     (501) staff       (20)      313 2024-05-07 07:33:50.000000 radient-2024.5.7/radient/__init__.py
-drwxr-xr-x   0 zilliz     (501) staff       (20)        0 2024-05-08 05:58:34.325430 radient-2024.5.7/radient/sinks/
--rw-r--r--   0 zilliz     (501) staff       (20)     2887 2024-05-07 07:33:50.000000 radient-2024.5.7/radient/sinks/milvus.py
-drwxr-xr-x   0 zilliz     (501) staff       (20)        0 2024-05-08 05:58:34.326476 radient-2024.5.7/radient/util/
--rw-r--r--   0 zilliz     (501) staff       (20)     2002 2024-05-08 02:54:42.000000 radient-2024.5.7/radient/util/lazy_import.py
--rw-r--r--   0 zilliz     (501) staff       (20)     2715 2024-05-07 22:31:22.000000 radient-2024.5.7/radient/vector.py
-drwxr-xr-x   0 zilliz     (501) staff       (20)        0 2024-05-08 05:58:34.328667 radient-2024.5.7/radient/vectorizers/
--rw-r--r--   0 zilliz     (501) staff       (20)     4966 2024-05-07 07:33:50.000000 radient-2024.5.7/radient/vectorizers/accelerate.py
-drwxr-xr-x   0 zilliz     (501) staff       (20)        0 2024-05-08 05:58:34.331749 radient-2024.5.7/radient/vectorizers/audio/
--rw-r--r--   0 zilliz     (501) staff       (20)      618 2024-05-07 07:33:50.000000 radient-2024.5.7/radient/vectorizers/audio/__init__.py
--rw-r--r--   0 zilliz     (501) staff       (20)      629 2024-05-07 07:33:50.000000 radient-2024.5.7/radient/vectorizers/audio/base.py
--rw-r--r--   0 zilliz     (501) staff       (20)     2155 2024-05-07 22:55:44.000000 radient-2024.5.7/radient/vectorizers/audio/torchaudio.py
--rw-r--r--   0 zilliz     (501) staff       (20)     2420 2024-05-08 03:55:59.000000 radient-2024.5.7/radient/vectorizers/base.py
-drwxr-xr-x   0 zilliz     (501) staff       (20)        0 2024-05-08 05:58:34.335900 radient-2024.5.7/radient/vectorizers/graph/
--rw-r--r--   0 zilliz     (501) staff       (20)      598 2024-05-07 07:33:50.000000 radient-2024.5.7/radient/vectorizers/graph/__init__.py
--rw-r--r--   0 zilliz     (501) staff       (20)      950 2024-05-07 07:33:50.000000 radient-2024.5.7/radient/vectorizers/graph/base.py
--rw-r--r--   0 zilliz     (501) staff       (20)     1629 2024-05-07 21:05:22.000000 radient-2024.5.7/radient/vectorizers/graph/fastrp.py
-drwxr-xr-x   0 zilliz     (501) staff       (20)        0 2024-05-08 05:58:34.338053 radient-2024.5.7/radient/vectorizers/image/
--rw-r--r--   0 zilliz     (501) staff       (20)      612 2024-05-07 07:33:50.000000 radient-2024.5.7/radient/vectorizers/image/__init__.py
--rw-r--r--   0 zilliz     (501) staff       (20)     2081 2024-05-07 07:33:50.000000 radient-2024.5.7/radient/vectorizers/image/base.py
--rw-r--r--   0 zilliz     (501) staff       (20)     1719 2024-05-07 22:46:37.000000 radient-2024.5.7/radient/vectorizers/image/timm.py
-drwxr-xr-x   0 zilliz     (501) staff       (20)        0 2024-05-08 05:58:34.340759 radient-2024.5.7/radient/vectorizers/molecule/
--rw-r--r--   0 zilliz     (501) staff       (20)      617 2024-05-07 07:33:50.000000 radient-2024.5.7/radient/vectorizers/molecule/__init__.py
--rw-r--r--   0 zilliz     (501) staff       (20)      761 2024-05-07 07:33:50.000000 radient-2024.5.7/radient/vectorizers/molecule/base.py
--rw-r--r--   0 zilliz     (501) staff       (20)     1235 2024-05-07 22:47:01.000000 radient-2024.5.7/radient/vectorizers/molecule/rdkit.py
-drwxr-xr-x   0 zilliz     (501) staff       (20)        0 2024-05-08 05:58:34.346734 radient-2024.5.7/radient/vectorizers/text/
--rw-r--r--   0 zilliz     (501) staff       (20)      974 2024-05-08 02:13:26.000000 radient-2024.5.7/radient/vectorizers/text/__init__.py
--rw-r--r--   0 zilliz     (501) staff       (20)      452 2024-05-07 07:33:50.000000 radient-2024.5.7/radient/vectorizers/text/base.py
--rw-r--r--   0 zilliz     (501) staff       (20)     1006 2024-05-08 02:45:55.000000 radient-2024.5.7/radient/vectorizers/text/cohere.py
--rw-r--r--   0 zilliz     (501) staff       (20)     2247 2024-05-08 03:54:50.000000 radient-2024.5.7/radient/vectorizers/text/sbert.py
--rw-r--r--   0 zilliz     (501) staff       (20)     1037 2024-05-07 09:17:22.000000 radient-2024.5.7/radient/vectorizers/text/sklearn.py
--rw-r--r--   0 zilliz     (501) staff       (20)      772 2024-05-08 02:59:26.000000 radient-2024.5.7/radient/vectorizers/text/voyage.py
-drwxr-xr-x   0 zilliz     (501) staff       (20)        0 2024-05-08 05:58:34.348127 radient-2024.5.7/radient.egg-info/
--rw-r--r--   0 zilliz     (501) staff       (20)     4068 2024-05-08 05:58:34.000000 radient-2024.5.7/radient.egg-info/PKG-INFO
--rw-r--r--   0 zilliz     (501) staff       (20)      990 2024-05-08 05:58:34.000000 radient-2024.5.7/radient.egg-info/SOURCES.txt
--rw-r--r--   0 zilliz     (501) staff       (20)        1 2024-05-08 05:58:34.000000 radient-2024.5.7/radient.egg-info/dependency_links.txt
--rw-r--r--   0 zilliz     (501) staff       (20)       12 2024-05-08 05:58:34.000000 radient-2024.5.7/radient.egg-info/requires.txt
--rw-r--r--   0 zilliz     (501) staff       (20)        8 2024-05-08 05:58:34.000000 radient-2024.5.7/radient.egg-info/top_level.txt
--rw-r--r--   0 zilliz     (501) staff       (20)       38 2024-05-08 05:58:34.349148 radient-2024.5.7/setup.cfg
+drwxr-xr-x   0 zilliz     (501) staff       (20)        0 2024-05-10 07:24:41.302611 radient-2024.5.9/
+-rw-r--r--   0 zilliz     (501) staff       (20)     1266 2024-05-08 04:55:23.000000 radient-2024.5.9/LICENSE
+-rw-r--r--   0 zilliz     (501) staff       (20)     4068 2024-05-10 07:24:41.301745 radient-2024.5.9/PKG-INFO
+-rw-r--r--   0 zilliz     (501) staff       (20)     3594 2024-05-09 07:38:50.000000 radient-2024.5.9/README.md
+-rw-r--r--   0 zilliz     (501) staff       (20)      470 2024-05-10 07:24:25.000000 radient-2024.5.9/pyproject.toml
+drwxr-xr-x   0 zilliz     (501) staff       (20)        0 2024-05-10 07:24:41.264944 radient-2024.5.9/radient/
+-rw-r--r--   0 zilliz     (501) staff       (20)      313 2024-05-07 07:33:50.000000 radient-2024.5.9/radient/__init__.py
+drwxr-xr-x   0 zilliz     (501) staff       (20)        0 2024-05-10 07:24:41.270275 radient-2024.5.9/radient/sinks/
+-rw-r--r--   0 zilliz     (501) staff       (20)     2807 2024-05-09 07:37:00.000000 radient-2024.5.9/radient/sinks/milvus.py
+drwxr-xr-x   0 zilliz     (501) staff       (20)        0 2024-05-10 07:24:41.271574 radient-2024.5.9/radient/util/
+-rw-r--r--   0 zilliz     (501) staff       (20)     2082 2024-05-09 07:30:38.000000 radient-2024.5.9/radient/util/lazy_import.py
+-rw-r--r--   0 zilliz     (501) staff       (20)     2715 2024-05-07 22:31:22.000000 radient-2024.5.9/radient/vector.py
+drwxr-xr-x   0 zilliz     (501) staff       (20)        0 2024-05-10 07:24:41.274370 radient-2024.5.9/radient/vectorizers/
+-rw-r--r--   0 zilliz     (501) staff       (20)     4966 2024-05-07 07:33:50.000000 radient-2024.5.9/radient/vectorizers/accelerate.py
+drwxr-xr-x   0 zilliz     (501) staff       (20)        0 2024-05-10 07:24:41.279194 radient-2024.5.9/radient/vectorizers/audio/
+-rw-r--r--   0 zilliz     (501) staff       (20)      618 2024-05-07 07:33:50.000000 radient-2024.5.9/radient/vectorizers/audio/__init__.py
+-rw-r--r--   0 zilliz     (501) staff       (20)      629 2024-05-07 07:33:50.000000 radient-2024.5.9/radient/vectorizers/audio/base.py
+-rw-r--r--   0 zilliz     (501) staff       (20)     2155 2024-05-07 22:55:44.000000 radient-2024.5.9/radient/vectorizers/audio/torchaudio.py
+-rw-r--r--   0 zilliz     (501) staff       (20)     2420 2024-05-08 03:55:59.000000 radient-2024.5.9/radient/vectorizers/base.py
+drwxr-xr-x   0 zilliz     (501) staff       (20)        0 2024-05-10 07:24:41.283487 radient-2024.5.9/radient/vectorizers/graph/
+-rw-r--r--   0 zilliz     (501) staff       (20)      598 2024-05-07 07:33:50.000000 radient-2024.5.9/radient/vectorizers/graph/__init__.py
+-rw-r--r--   0 zilliz     (501) staff       (20)      950 2024-05-07 07:33:50.000000 radient-2024.5.9/radient/vectorizers/graph/base.py
+-rw-r--r--   0 zilliz     (501) staff       (20)     1659 2024-05-09 07:34:21.000000 radient-2024.5.9/radient/vectorizers/graph/fastrp.py
+drwxr-xr-x   0 zilliz     (501) staff       (20)        0 2024-05-10 07:24:41.287258 radient-2024.5.9/radient/vectorizers/image/
+-rw-r--r--   0 zilliz     (501) staff       (20)      612 2024-05-07 07:33:50.000000 radient-2024.5.9/radient/vectorizers/image/__init__.py
+-rw-r--r--   0 zilliz     (501) staff       (20)     2064 2024-05-09 07:35:19.000000 radient-2024.5.9/radient/vectorizers/image/base.py
+-rw-r--r--   0 zilliz     (501) staff       (20)     1719 2024-05-07 22:46:37.000000 radient-2024.5.9/radient/vectorizers/image/timm.py
+drwxr-xr-x   0 zilliz     (501) staff       (20)        0 2024-05-10 07:24:41.291786 radient-2024.5.9/radient/vectorizers/molecule/
+-rw-r--r--   0 zilliz     (501) staff       (20)      617 2024-05-07 07:33:50.000000 radient-2024.5.9/radient/vectorizers/molecule/__init__.py
+-rw-r--r--   0 zilliz     (501) staff       (20)      748 2024-05-09 07:35:36.000000 radient-2024.5.9/radient/vectorizers/molecule/base.py
+-rw-r--r--   0 zilliz     (501) staff       (20)     1235 2024-05-07 22:47:01.000000 radient-2024.5.9/radient/vectorizers/molecule/rdkit.py
+drwxr-xr-x   0 zilliz     (501) staff       (20)        0 2024-05-10 07:24:41.299121 radient-2024.5.9/radient/vectorizers/text/
+-rw-r--r--   0 zilliz     (501) staff       (20)      974 2024-05-08 02:13:26.000000 radient-2024.5.9/radient/vectorizers/text/__init__.py
+-rw-r--r--   0 zilliz     (501) staff       (20)      452 2024-05-07 07:33:50.000000 radient-2024.5.9/radient/vectorizers/text/base.py
+-rw-r--r--   0 zilliz     (501) staff       (20)     1006 2024-05-08 02:45:55.000000 radient-2024.5.9/radient/vectorizers/text/cohere.py
+-rw-r--r--   0 zilliz     (501) staff       (20)     2295 2024-05-09 07:35:54.000000 radient-2024.5.9/radient/vectorizers/text/sbert.py
+-rw-r--r--   0 zilliz     (501) staff       (20)     1052 2024-05-09 07:36:09.000000 radient-2024.5.9/radient/vectorizers/text/sklearn.py
+-rw-r--r--   0 zilliz     (501) staff       (20)      772 2024-05-08 02:59:26.000000 radient-2024.5.9/radient/vectorizers/text/voyage.py
+drwxr-xr-x   0 zilliz     (501) staff       (20)        0 2024-05-10 07:24:41.300847 radient-2024.5.9/radient.egg-info/
+-rw-r--r--   0 zilliz     (501) staff       (20)     4068 2024-05-10 07:24:41.000000 radient-2024.5.9/radient.egg-info/PKG-INFO
+-rw-r--r--   0 zilliz     (501) staff       (20)      990 2024-05-10 07:24:41.000000 radient-2024.5.9/radient.egg-info/SOURCES.txt
+-rw-r--r--   0 zilliz     (501) staff       (20)        1 2024-05-10 07:24:41.000000 radient-2024.5.9/radient.egg-info/dependency_links.txt
+-rw-r--r--   0 zilliz     (501) staff       (20)       12 2024-05-10 07:24:41.000000 radient-2024.5.9/radient.egg-info/requires.txt
+-rw-r--r--   0 zilliz     (501) staff       (20)        8 2024-05-10 07:24:41.000000 radient-2024.5.9/radient.egg-info/top_level.txt
+-rw-r--r--   0 zilliz     (501) staff       (20)       38 2024-05-10 07:24:41.302812 radient-2024.5.9/setup.cfg
```

### Comparing `radient-2024.5.7/LICENSE` & `radient-2024.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `radient-2024.5.7/PKG-INFO` & `radient-2024.5.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radient
-Version: 2024.5.7
+Version: 2024.5.9
 Summary: Turn unstructured data into vectors
 Author-email: Frank Liu <frank@frankzliu.com>
 Project-URL: Homepage, https://github.com/fzliu/radient
 Project-URL: Issues, https://github.com/fzliu/radient/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.8
@@ -30,36 +30,33 @@
 
 Vectorization can be performed as follows:
 
 ```python
 >>> from radient import text_vectorizer
 >>> vectorizer = text_vectorizer()
 >>> vectorizer.vectorize("Hello, world!")
-Vector([-3.21440510e-02, -5.10351397e-02,  3.69579718e-02,
-...
+Vector([-3.21440510e-02, -5.10351397e-02,  3.69579718e-02, ...
 ```
 
 You're not limited to text modalities. Audio, graphs, images, and molecules can be vectorized as well:
 
 ```python
 >>> from pathlib import Path
 >>> from radient import audio_vectorizer, molecule_vectorizer
 >>> audio_vectorizer().vectorize(str(Path.home() / "audio.wav"))
-Vector([-5.26519306e-03, -4.55586426e-03,  1.79212391e-02,
-...
+Vector([-5.26519306e-03, -4.55586426e-03,  1.79212391e-02, ...
 >>> molecule_vectorizer().vectorize("O=C=O")  # O=C=O == SMILES string for CO2
-Vector([False, False, False,
-...
+Vector([False, False, False, ...
 ```
 
 You can attach metadata to the resulting embeddings and store them in sinks. Radient currently supports [Milvus](https://milvus.io):
 
 ```python
 >>> vector = vectorizer.vectorize("My name is Slim Shady")
->>> vector.add_key_value("artist", "Eminem"). # {"artist": "Eminem"}
+>>> vector.add_key_value("artist", "Eminem")  # {"artist": "Eminem"}
 >>> vector.store()
 ```
 
 For production use cases with large quantities of data, performance is key. Radient provides an `accelerate` function to optimize some vectorizers on-the-fly:
 
 ```python
 >>> vectorizer.vectorize("Hello, world!")  # runtime: ~32ms
```

### Comparing `radient-2024.5.7/README.md` & `radient-2024.5.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,36 +16,33 @@
 
 Vectorization can be performed as follows:
 
 ```python
 >>> from radient import text_vectorizer
 >>> vectorizer = text_vectorizer()
 >>> vectorizer.vectorize("Hello, world!")
-Vector([-3.21440510e-02, -5.10351397e-02,  3.69579718e-02,
-...
+Vector([-3.21440510e-02, -5.10351397e-02,  3.69579718e-02, ...
 ```
 
 You're not limited to text modalities. Audio, graphs, images, and molecules can be vectorized as well:
 
 ```python
 >>> from pathlib import Path
 >>> from radient import audio_vectorizer, molecule_vectorizer
 >>> audio_vectorizer().vectorize(str(Path.home() / "audio.wav"))
-Vector([-5.26519306e-03, -4.55586426e-03,  1.79212391e-02,
-...
+Vector([-5.26519306e-03, -4.55586426e-03,  1.79212391e-02, ...
 >>> molecule_vectorizer().vectorize("O=C=O")  # O=C=O == SMILES string for CO2
-Vector([False, False, False,
-...
+Vector([False, False, False, ...
 ```
 
 You can attach metadata to the resulting embeddings and store them in sinks. Radient currently supports [Milvus](https://milvus.io):
 
 ```python
 >>> vector = vectorizer.vectorize("My name is Slim Shady")
->>> vector.add_key_value("artist", "Eminem"). # {"artist": "Eminem"}
+>>> vector.add_key_value("artist", "Eminem")  # {"artist": "Eminem"}
 >>> vector.store()
 ```
 
 For production use cases with large quantities of data, performance is key. Radient provides an `accelerate` function to optimize some vectorizers on-the-fly:
 
 ```python
 >>> vectorizer.vectorize("Hello, world!")  # runtime: ~32ms
```

### Comparing `radient-2024.5.7/radient/sinks/milvus.py` & `radient-2024.5.9/radient/sinks/milvus.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Optional
 
 from radient.util.lazy_import import fully_qualified_name, LazyImport
 
-milvus = LazyImport("milvus", package="milvus")  # embedded Milvus server
-MilvusClient = LazyImport("pymilvus", package="pymilvus", attribute="MilvusClient")
-pymilvus = LazyImport("pymilvus", package="pymilvus")  # Milvus Python SDK
-validators = LazyImport("validators", package="validators")
+milvus = LazyImport("milvus")  # embedded Milvus server
+MilvusClient = LazyImport("pymilvus", attribute="MilvusClient")
+pymilvus = LazyImport("pymilvus")  # Milvus Python SDK
+validators = LazyImport("validators")
 
 
 class MilvusInterface(object):
     """Interface to the Milvus vector database. Because there are 
 
     This interface also works with Zilliz Cloud (https://zilliz.com/cloud).
     """
```

### Comparing `radient-2024.5.7/radient/util/lazy_import.py` & `radient-2024.5.9/radient/util/lazy_import.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,25 +32,26 @@
     Adapted from tensorflow/python/util/lazy_loader.py.
     """
 
     def __init__(
         self,
         name: str,
         attribute: Optional[str] = None,
-        package: Optional[str] = None
+        package_name: Optional[str] = None
     ):
         super().__init__(name)
         self._attribute = attribute
-        self._package = package if package else name
+        self._top_name = name.split(".")[0]
+        self._package_name = package_name if package_name else self._top_name
         self._module = None
 
     def _load(self) -> ModuleType:
         if not self._module:
-            if not importlib.util.find_spec(self.__name__):
-                prompt_install(self._package)
+            if not importlib.util.find_spec(self._top_name):
+                prompt_install(self._package_name)
             self._module = importlib.import_module(self.__name__)
             self.__dict__.update(self._module.__dict__)
         if self._attribute:
             return getattr(self._module, self._attribute)
         return self._module
 
     def __call__(self, *args, **kwargs) -> Any:
```

### Comparing `radient-2024.5.7/radient/vector.py` & `radient-2024.5.9/radient/vector.py`

 * *Files identical despite different names*

### Comparing `radient-2024.5.7/radient/vectorizers/accelerate.py` & `radient-2024.5.9/radient/vectorizers/accelerate.py`

 * *Files identical despite different names*

### Comparing `radient-2024.5.7/radient/vectorizers/audio/__init__.py` & `radient-2024.5.9/radient/vectorizers/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `radient-2024.5.7/radient/vectorizers/audio/base.py` & `radient-2024.5.9/radient/vectorizers/audio/base.py`

 * *Files identical despite different names*

### Comparing `radient-2024.5.7/radient/vectorizers/audio/torchaudio.py` & `radient-2024.5.9/radient/vectorizers/audio/torchaudio.py`

 * *Files identical despite different names*

### Comparing `radient-2024.5.7/radient/vectorizers/base.py` & `radient-2024.5.9/radient/vectorizers/base.py`

 * *Files identical despite different names*

### Comparing `radient-2024.5.7/radient/vectorizers/graph/__init__.py` & `radient-2024.5.9/radient/vectorizers/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `radient-2024.5.7/radient/vectorizers/graph/base.py` & `radient-2024.5.9/radient/vectorizers/graph/base.py`

 * *Files identical despite different names*

### Comparing `radient-2024.5.7/radient/vectorizers/graph/fastrp.py` & `radient-2024.5.9/radient/vectorizers/graph/fastrp.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import numpy as np
 
 from radient.util.lazy_import import LazyImport
 from radient.vector import Vector
 from radient.vectorizers.graph.base import GraphVectorizer
 
 sp = LazyImport("scipy")
-SparseRandomProjection = LazyImport("sklearn.random_projection", attribute="SparseRandomProjection")
+SparseRandomProjection = LazyImport( "sklearn.random_projection", attribute="SparseRandomProjection", package_name="scikit-learn")
 
 
 class FastRPGraphVectorizer(GraphVectorizer):
     """Computes node (not graph) embeddings using the FastRP algorithm.
     """
 
     def __init__(
```

### Comparing `radient-2024.5.7/radient/vectorizers/image/__init__.py` & `radient-2024.5.9/radient/vectorizers/image/__init__.py`

 * *Files identical despite different names*

### Comparing `radient-2024.5.7/radient/vectorizers/image/base.py` & `radient-2024.5.9/radient/vectorizers/image/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 
 import numpy as np
 
 from radient.util.lazy_import import fully_qualified_name, LazyImport
 from radient.vectorizers.base import Vector
 from radient.vectorizers.base import Vectorizer
 
-Image = LazyImport("PIL.Image", package="pillow")
-validators = LazyImport("validators", package="validators")
+Image = LazyImport("PIL.Image", package_name="pillow")
+validators = LazyImport("validators")
 
 
 class ImageVectorizer(Vectorizer):
 
     @abstractmethod
     def __init__(self):
         super().__init__()
```

### Comparing `radient-2024.5.7/radient/vectorizers/image/timm.py` & `radient-2024.5.9/radient/vectorizers/image/timm.py`

 * *Files identical despite different names*

### Comparing `radient-2024.5.7/radient/vectorizers/molecule/__init__.py` & `radient-2024.5.9/radient/vectorizers/molecule/__init__.py`

 * *Files identical despite different names*

### Comparing `radient-2024.5.7/radient/vectorizers/molecule/base.py` & `radient-2024.5.9/radient/vectorizers/molecule/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from abc import abstractmethod
 from typing import Any, List
 
 from radient.vectorizers.base import Vector, Vectorizer
 from radient.util.lazy_import import fully_qualified_name, LazyImport
 
-Chem = LazyImport("rdkit", attribute="Chem")
+Chem = LazyImport("rdkit.Chem")
 
 
 class MoleculeVectorizer(Vectorizer):
 
     @abstractmethod
     def __init__(self):
         super().__init__()
```

### Comparing `radient-2024.5.7/radient/vectorizers/molecule/rdkit.py` & `radient-2024.5.9/radient/vectorizers/molecule/rdkit.py`

 * *Files identical despite different names*

### Comparing `radient-2024.5.7/radient/vectorizers/text/__init__.py` & `radient-2024.5.9/radient/vectorizers/text/__init__.py`

 * *Files identical despite different names*

### Comparing `radient-2024.5.7/radient/vectorizers/text/cohere.py` & `radient-2024.5.9/radient/vectorizers/text/cohere.py`

 * *Files identical despite different names*

### Comparing `radient-2024.5.7/radient/vectorizers/text/sbert.py` & `radient-2024.5.9/radient/vectorizers/text/sbert.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 from typing import List
 
 from radient.util.lazy_import import LazyImport
 from radient.vector import Vector
 from radient.vectorizers.text.base import TextVectorizer
 from radient.vectorizers.accelerate import export_to_onnx, ONNXForward
 
-SentenceTransformer = LazyImport("sentence_transformers", attribute="SentenceTransformer", package="sentence-transformers")
+SentenceTransformer = LazyImport("sentence_transformers", attribute="SentenceTransformer", package_name="sentence-transformers")
 torch = LazyImport("torch")
 
 
 class SBERTTextVectorizer(TextVectorizer):
     """Text vectorization with `sentence-transformers`.
     """
 
-    def __init__(self, model_name: str = "BAAI/bge-small-en-v1.5", **kwargs):
+    def __init__(self, model_name_or_path: str = "BAAI/bge-small-en-v1.5", **kwargs):
         super().__init__()
-        self._model_name = model_name
-        self._model = SentenceTransformer(model_name, **kwargs)
+        self._model_name = model_name_or_path
+        self._model = SentenceTransformer(model_name_or_path=model_name_or_path, **kwargs)
 
     def _vectorize(self, text: str) -> Vector:
         # TODO(fzliu): token length check
         # TODO(fzliu): dynamic batching
         with torch.inference_mode():
             vector = self._model.encode(text)
         return vector.view(Vector)
```

### Comparing `radient-2024.5.7/radient/vectorizers/text/sklearn.py` & `radient-2024.5.9/radient/vectorizers/text/sklearn.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from typing import Dict, List, Optional
 import warnings
 
 from radient.util.lazy_import import LazyImport
 from radient.vector import Vector
 from radient.vectorizers.text.base import TextVectorizer
 
-CountVectorizer = LazyImport("sklearn.feature_extraction.text", attribute="CountVectorizer", package="scikit-learn")
-TfidfVectorizer = LazyImport("sklearn.feature_extraction.text", attribute="TfidfVectorizer", package="scikit-learn")
-HashingVectorizer = LazyImport("sklearn.feature_extraction.text", attribute="HashingVectorizer", package="scikit-learn")
+CountVectorizer = LazyImport("sklearn.feature_extraction.text", attribute="CountVectorizer", package_name="scikit-learn")
+TfidfVectorizer = LazyImport("sklearn.feature_extraction.text", attribute="TfidfVectorizer", package_name="scikit-learn")
+HashingVectorizer = LazyImport("sklearn.feature_extraction.text", attribute="HashingVectorizer", package_name="scikit-learn")
 
 
 class SklearnTextVectorizer(TextVectorizer):
     """Text vectorization with `sentence-transformers`.
     """
 
     def __init__(self, **kwargs):
```

### Comparing `radient-2024.5.7/radient/vectorizers/text/voyage.py` & `radient-2024.5.9/radient/vectorizers/text/voyage.py`

 * *Files identical despite different names*

### Comparing `radient-2024.5.7/radient.egg-info/PKG-INFO` & `radient-2024.5.9/radient.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radient
-Version: 2024.5.7
+Version: 2024.5.9
 Summary: Turn unstructured data into vectors
 Author-email: Frank Liu <frank@frankzliu.com>
 Project-URL: Homepage, https://github.com/fzliu/radient
 Project-URL: Issues, https://github.com/fzliu/radient/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.8
@@ -30,36 +30,33 @@
 
 Vectorization can be performed as follows:
 
 ```python
 >>> from radient import text_vectorizer
 >>> vectorizer = text_vectorizer()
 >>> vectorizer.vectorize("Hello, world!")
-Vector([-3.21440510e-02, -5.10351397e-02,  3.69579718e-02,
-...
+Vector([-3.21440510e-02, -5.10351397e-02,  3.69579718e-02, ...
 ```
 
 You're not limited to text modalities. Audio, graphs, images, and molecules can be vectorized as well:
 
 ```python
 >>> from pathlib import Path
 >>> from radient import audio_vectorizer, molecule_vectorizer
 >>> audio_vectorizer().vectorize(str(Path.home() / "audio.wav"))
-Vector([-5.26519306e-03, -4.55586426e-03,  1.79212391e-02,
-...
+Vector([-5.26519306e-03, -4.55586426e-03,  1.79212391e-02, ...
 >>> molecule_vectorizer().vectorize("O=C=O")  # O=C=O == SMILES string for CO2
-Vector([False, False, False,
-...
+Vector([False, False, False, ...
 ```
 
 You can attach metadata to the resulting embeddings and store them in sinks. Radient currently supports [Milvus](https://milvus.io):
 
 ```python
 >>> vector = vectorizer.vectorize("My name is Slim Shady")
->>> vector.add_key_value("artist", "Eminem"). # {"artist": "Eminem"}
+>>> vector.add_key_value("artist", "Eminem")  # {"artist": "Eminem"}
 >>> vector.store()
 ```
 
 For production use cases with large quantities of data, performance is key. Radient provides an `accelerate` function to optimize some vectorizers on-the-fly:
 
 ```python
 >>> vectorizer.vectorize("Hello, world!")  # runtime: ~32ms
```

### Comparing `radient-2024.5.7/radient.egg-info/SOURCES.txt` & `radient-2024.5.9/radient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

