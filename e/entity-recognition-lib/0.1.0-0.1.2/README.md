# Comparing `tmp/entity_recognition_lib-0.1.0.tar.gz` & `tmp/entity_recognition_lib-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "entity_recognition_lib-0.1.0.tar", max compression
+gzip compressed data, was "entity_recognition_lib-0.1.2.tar", max compression
```

## Comparing `entity_recognition_lib-0.1.0.tar` & `entity_recognition_lib-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1053 2024-05-08 19:51:56.995350 entity_recognition_lib-0.1.0/LICENSE
--rw-r--r--   0        0        0     3172 2024-05-08 19:51:56.995350 entity_recognition_lib-0.1.0/README.md
--rw-r--r--   0        0        0     1311 2024-05-08 19:51:56.999350 entity_recognition_lib-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1797 2024-05-08 19:51:56.999350 entity_recognition_lib-0.1.0/src/entity_recognition_lib/EntityRecognizer.py
--rw-r--r--   0        0        0       47 2024-05-08 19:51:56.999350 entity_recognition_lib-0.1.0/src/entity_recognition_lib/__init__.py
--rw-r--r--   0        0        0    31581 2024-05-08 19:51:56.999350 entity_recognition_lib-0.1.0/src/entity_recognition_lib/data/tech_entities.json
--rw-r--r--   0        0        0        0 2024-05-08 19:51:56.999350 entity_recognition_lib-0.1.0/src/entity_recognition_lib/functions/__init__.py
--rw-r--r--   0        0        0     2823 2024-05-08 19:51:56.999350 entity_recognition_lib-0.1.0/src/entity_recognition_lib/functions/entity_extraction.py
--rw-r--r--   0        0        0     5232 2024-05-08 19:51:56.999350 entity_recognition_lib-0.1.0/src/entity_recognition_lib/functions/recommendation_generation.py
--rw-r--r--   0        0        0     1271 2024-05-08 19:51:56.999350 entity_recognition_lib-0.1.0/src/entity_recognition_lib/functions/topic_classification.py
--rw-r--r--   0        0        0     1725 2024-05-08 19:51:56.999350 entity_recognition_lib-0.1.0/src/entity_recognition_lib/models.py
--rw-r--r--   0        0        0     3269 2024-05-08 19:51:56.999350 entity_recognition_lib-0.1.0/src/entity_recognition_lib/utils.py
--rw-r--r--   0        0        0     4071 1970-01-01 00:00:00.000000 entity_recognition_lib-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1053 2024-05-10 14:53:09.191309 entity_recognition_lib-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3173 2024-05-10 14:53:09.191309 entity_recognition_lib-0.1.2/README.md
+-rw-r--r--   0        0        0     1311 2024-05-10 14:54:10.631680 entity_recognition_lib-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1797 2024-05-10 14:53:09.191309 entity_recognition_lib-0.1.2/src/entity_recognition_lib/EntityRecognizer.py
+-rw-r--r--   0        0        0       47 2024-05-10 14:53:09.191309 entity_recognition_lib-0.1.2/src/entity_recognition_lib/__init__.py
+-rw-r--r--   0        0        0    31581 2024-05-10 14:53:09.191309 entity_recognition_lib-0.1.2/src/entity_recognition_lib/data/tech_entities.json
+-rw-r--r--   0        0        0        0 2024-05-10 14:53:09.191309 entity_recognition_lib-0.1.2/src/entity_recognition_lib/functions/__init__.py
+-rw-r--r--   0        0        0     2823 2024-05-10 14:53:09.191309 entity_recognition_lib-0.1.2/src/entity_recognition_lib/functions/entity_extraction.py
+-rw-r--r--   0        0        0     5232 2024-05-10 14:53:09.191309 entity_recognition_lib-0.1.2/src/entity_recognition_lib/functions/recommendation_generation.py
+-rw-r--r--   0        0        0     1271 2024-05-10 14:53:09.191309 entity_recognition_lib-0.1.2/src/entity_recognition_lib/functions/topic_classification.py
+-rw-r--r--   0        0        0     1725 2024-05-10 14:53:09.191309 entity_recognition_lib-0.1.2/src/entity_recognition_lib/models.py
+-rw-r--r--   0        0        0     3269 2024-05-10 14:53:09.191309 entity_recognition_lib-0.1.2/src/entity_recognition_lib/utils.py
+-rw-r--r--   0        0        0     4072 1970-01-01 00:00:00.000000 entity_recognition_lib-0.1.2/PKG-INFO
```

### Comparing `entity_recognition_lib-0.1.0/LICENSE` & `entity_recognition_lib-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `entity_recognition_lib-0.1.0/README.md` & `entity_recognition_lib-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 - **BERTopic Integration**: Leverages topic modeling to enhance the relevance of recommendations.
 - **spaCy Matchers**: Utilizes custom NLP patterns for precise entity recognition.
 
 ## Installation
 
 ### Prerequisites
 
-- Python 3.6+
+- Python 3.11+
 - pip
 
 ### Getting Started
 
 Install the library directly from PyPI:
 
 ```bash
```

### Comparing `entity_recognition_lib-0.1.0/pyproject.toml` & `entity_recognition_lib-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "entity-recognition-lib"
-version = "0.1.0"
+version = "0.1.2"
 description = "A library for technology entity recognition and recommendation"
 authors = ["Cesar Goncalves <goncalves.cesaraugusto94@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
```

### Comparing `entity_recognition_lib-0.1.0/src/entity_recognition_lib/EntityRecognizer.py` & `entity_recognition_lib-0.1.2/src/entity_recognition_lib/EntityRecognizer.py`

 * *Files identical despite different names*

### Comparing `entity_recognition_lib-0.1.0/src/entity_recognition_lib/data/tech_entities.json` & `entity_recognition_lib-0.1.2/src/entity_recognition_lib/data/tech_entities.json`

 * *Files identical despite different names*

### Comparing `entity_recognition_lib-0.1.0/src/entity_recognition_lib/functions/entity_extraction.py` & `entity_recognition_lib-0.1.2/src/entity_recognition_lib/functions/entity_extraction.py`

 * *Files identical despite different names*

### Comparing `entity_recognition_lib-0.1.0/src/entity_recognition_lib/functions/recommendation_generation.py` & `entity_recognition_lib-0.1.2/src/entity_recognition_lib/functions/recommendation_generation.py`

 * *Files identical despite different names*

### Comparing `entity_recognition_lib-0.1.0/src/entity_recognition_lib/functions/topic_classification.py` & `entity_recognition_lib-0.1.2/src/entity_recognition_lib/functions/topic_classification.py`

 * *Files identical despite different names*

### Comparing `entity_recognition_lib-0.1.0/src/entity_recognition_lib/models.py` & `entity_recognition_lib-0.1.2/src/entity_recognition_lib/models.py`

 * *Files identical despite different names*

### Comparing `entity_recognition_lib-0.1.0/src/entity_recognition_lib/utils.py` & `entity_recognition_lib-0.1.2/src/entity_recognition_lib/utils.py`

 * *Files identical despite different names*

### Comparing `entity_recognition_lib-0.1.0/PKG-INFO` & `entity_recognition_lib-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: entity-recognition-lib
-Version: 0.1.0
+Version: 0.1.2
 Summary: A library for technology entity recognition and recommendation
 License: MIT
 Author: Cesar Goncalves
 Author-email: goncalves.cesaraugusto94@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -36,15 +36,15 @@
 - **BERTopic Integration**: Leverages topic modeling to enhance the relevance of recommendations.
 - **spaCy Matchers**: Utilizes custom NLP patterns for precise entity recognition.
 
 ## Installation
 
 ### Prerequisites
 
-- Python 3.6+
+- Python 3.11+
 - pip
 
 ### Getting Started
 
 Install the library directly from PyPI:
 
 ```bash
```

