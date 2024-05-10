# Comparing `tmp/spyder_index-0.1.2.tar.gz` & `tmp/spyder_index-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spyder_index-0.1.2.tar", last modified: Thu May  9 01:54:59 2024, max compression
+gzip compressed data, was "spyder_index-0.2.0.tar", last modified: Fri May 10 11:49:29 2024, max compression
```

## Comparing `spyder_index-0.1.2.tar` & `spyder_index-0.2.0.tar`

### file list

```diff
@@ -1,39 +1,45 @@
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-09 01:54:59.078690 spyder_index-0.1.2/
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)     1071 2024-05-07 19:51:35.000000 spyder_index-0.1.2/LICENSE
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)     8925 2024-05-09 01:54:59.077741 spyder_index-0.1.2/PKG-INFO
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)     7632 2024-05-09 01:06:16.000000 spyder_index-0.1.2/README.md
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)     1368 2024-05-09 01:54:15.000000 spyder_index-0.1.2/pyproject.toml
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)       38 2024-05-09 01:54:59.078881 spyder_index-0.1.2/setup.cfg
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-09 01:54:59.034161 spyder_index-0.1.2/spyder_index/
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)       21 2024-05-09 01:54:10.000000 spyder_index-0.1.2/spyder_index/__init__.py
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-09 01:54:59.028389 spyder_index-0.1.2/spyder_index/core/
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-09 01:54:59.044357 spyder_index-0.1.2/spyder_index/core/document/
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)       83 2024-05-07 19:52:45.000000 spyder_index-0.1.2/spyder_index/core/document/__init__.py
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)     3199 2024-05-09 00:45:07.000000 spyder_index-0.1.2/spyder_index/core/document/base.py
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-09 01:54:59.048182 spyder_index-0.1.2/spyder_index/core/embeddings/
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)       89 2024-05-07 19:53:08.000000 spyder_index-0.1.2/spyder_index/core/embeddings/__init__.py
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)      728 2024-05-07 20:19:50.000000 spyder_index-0.1.2/spyder_index/core/embeddings/base.py
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-09 01:54:59.052110 spyder_index-0.1.2/spyder_index/core/vector_stores/
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)      116 2024-05-07 19:53:25.000000 spyder_index-0.1.2/spyder_index/core/vector_stores/__init__.py
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)      256 2024-05-07 19:53:31.000000 spyder_index-0.1.2/spyder_index/core/vector_stores/base.py
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-09 01:54:59.056095 spyder_index-0.1.2/spyder_index/embeddings/
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)      117 2024-05-07 19:54:12.000000 spyder_index-0.1.2/spyder_index/embeddings/__init__.py
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)     2024 2024-05-07 20:24:21.000000 spyder_index-0.1.2/spyder_index/embeddings/huggingface.py
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-09 01:54:59.063596 spyder_index-0.1.2/spyder_index/ingestion/
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)      255 2024-05-08 20:23:42.000000 spyder_index-0.1.2/spyder_index/ingestion/__init__.py
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)     1249 2024-05-09 00:48:53.000000 spyder_index-0.1.2/spyder_index/ingestion/directory_file.py
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)     1408 2024-05-08 14:47:33.000000 spyder_index-0.1.2/spyder_index/ingestion/ibm_cos.py
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)      723 2024-05-09 00:44:40.000000 spyder_index-0.1.2/spyder_index/ingestion/json.py
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-09 01:54:59.068738 spyder_index-0.1.2/spyder_index/text_splitters/
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)      200 2024-05-07 19:55:01.000000 spyder_index-0.1.2/spyder_index/text_splitters/__init__.py
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)     1832 2024-05-07 19:55:07.000000 spyder_index-0.1.2/spyder_index/text_splitters/semantic.py
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)     1511 2024-05-07 19:55:15.000000 spyder_index-0.1.2/spyder_index/text_splitters/sentence.py
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-09 01:54:59.073184 spyder_index-0.1.2/spyder_index/vector_stores/
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)      128 2024-05-07 19:55:30.000000 spyder_index-0.1.2/spyder_index/vector_stores/__init__.py
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)     7619 2024-05-07 19:55:41.000000 spyder_index-0.1.2/spyder_index/vector_stores/elasticsearch.py
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-09 01:54:59.076360 spyder_index-0.1.2/spyder_index.egg-info/
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)     8925 2024-05-09 01:54:59.000000 spyder_index-0.1.2/spyder_index.egg-info/PKG-INFO
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)      891 2024-05-09 01:54:59.000000 spyder_index-0.1.2/spyder_index.egg-info/SOURCES.txt
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)        1 2024-05-09 01:54:59.000000 spyder_index-0.1.2/spyder_index.egg-info/dependency_links.txt
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)      286 2024-05-09 01:54:59.000000 spyder_index-0.1.2/spyder_index.egg-info/requires.txt
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)       13 2024-05-09 01:54:59.000000 spyder_index-0.1.2/spyder_index.egg-info/top_level.txt
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-10 11:49:29.792106 spyder_index-0.2.0/
+-rw-rw-r--   0 leonardofurnielis   (501) staff       (20)     1071 2024-05-07 19:51:35.000000 spyder_index-0.2.0/LICENSE
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)     9471 2024-05-10 11:49:29.790828 spyder_index-0.2.0/PKG-INFO
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)     8242 2024-05-10 11:38:25.000000 spyder_index-0.2.0/README.md
+-rw-rw-r--   0 leonardofurnielis   (501) staff       (20)     1309 2024-05-10 11:44:39.000000 spyder_index-0.2.0/pyproject.toml
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)       38 2024-05-10 11:49:29.792353 spyder_index-0.2.0/setup.cfg
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-10 11:49:29.693249 spyder_index-0.2.0/spyder_index/
+-rw-rw-r--   0 leonardofurnielis   (501) staff       (20)       21 2024-05-10 11:44:46.000000 spyder_index-0.2.0/spyder_index/__init__.py
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-10 11:49:29.684346 spyder_index-0.2.0/spyder_index/core/
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-10 11:49:29.735169 spyder_index-0.2.0/spyder_index/core/document/
+-rw-rw-r--   0 leonardofurnielis   (501) staff       (20)       83 2024-05-07 19:52:45.000000 spyder_index-0.2.0/spyder_index/core/document/__init__.py
+-rw-rw-r--   0 leonardofurnielis   (501) staff       (20)     2168 2024-05-10 11:01:20.000000 spyder_index-0.2.0/spyder_index/core/document/base.py
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-10 11:49:29.738903 spyder_index-0.2.0/spyder_index/core/embeddings/
+-rw-rw-r--   0 leonardofurnielis   (501) staff       (20)       89 2024-05-07 19:53:08.000000 spyder_index-0.2.0/spyder_index/core/embeddings/__init__.py
+-rw-rw-r--   0 leonardofurnielis   (501) staff       (20)      728 2024-05-09 16:51:50.000000 spyder_index-0.2.0/spyder_index/core/embeddings/base.py
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-10 11:49:29.748732 spyder_index-0.2.0/spyder_index/core/readers/
+-rw-rw-r--   0 leonardofurnielis   (501) staff       (20)       86 2024-05-09 21:26:45.000000 spyder_index-0.2.0/spyder_index/core/readers/__init__.py
+-rw-rw-r--   0 leonardofurnielis   (501) staff       (20)      533 2024-05-09 20:15:29.000000 spyder_index-0.2.0/spyder_index/core/readers/base.py
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-10 11:49:29.755622 spyder_index-0.2.0/spyder_index/core/vector_stores/
+-rw-rw-r--   0 leonardofurnielis   (501) staff       (20)      116 2024-05-07 19:53:25.000000 spyder_index-0.2.0/spyder_index/core/vector_stores/__init__.py
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)      256 2024-05-09 11:34:49.000000 spyder_index-0.2.0/spyder_index/core/vector_stores/base.py
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-10 11:49:29.760419 spyder_index-0.2.0/spyder_index/embeddings/
+-rw-rw-r--   0 leonardofurnielis   (501) staff       (20)      117 2024-05-07 19:54:12.000000 spyder_index-0.2.0/spyder_index/embeddings/__init__.py
+-rw-rw-r--   0 leonardofurnielis   (501) staff       (20)     2024 2024-05-07 20:24:21.000000 spyder_index-0.2.0/spyder_index/embeddings/huggingface.py
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-10 11:49:29.765832 spyder_index-0.2.0/spyder_index/readers/
+-rw-rw-r--   0 leonardofurnielis   (501) staff       (20)      165 2024-05-10 11:39:21.000000 spyder_index-0.2.0/spyder_index/readers/__init__.py
+-rw-rw-r--   0 leonardofurnielis   (501) staff       (20)     1918 2024-05-10 10:52:51.000000 spyder_index-0.2.0/spyder_index/readers/directory.py
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-10 11:49:29.771624 spyder_index-0.2.0/spyder_index/readers/file/
+-rw-rw-r--   0 leonardofurnielis   (501) staff       (20)      163 2024-05-10 11:40:17.000000 spyder_index-0.2.0/spyder_index/readers/file/__init__.py
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)     1112 2024-05-10 01:42:18.000000 spyder_index-0.2.0/spyder_index/readers/file/json.py
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)      812 2024-05-10 01:44:20.000000 spyder_index-0.2.0/spyder_index/readers/file/pdf.py
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)     1595 2024-05-10 10:49:23.000000 spyder_index-0.2.0/spyder_index/readers/s3.py
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-10 11:49:29.782528 spyder_index-0.2.0/spyder_index/text_splitters/
+-rw-rw-r--   0 leonardofurnielis   (501) staff       (20)      200 2024-05-07 19:55:01.000000 spyder_index-0.2.0/spyder_index/text_splitters/__init__.py
+-rw-rw-r--   0 leonardofurnielis   (501) staff       (20)     1832 2024-05-07 19:55:07.000000 spyder_index-0.2.0/spyder_index/text_splitters/semantic.py
+-rw-rw-r--   0 leonardofurnielis   (501) staff       (20)     1371 2024-05-10 11:27:40.000000 spyder_index-0.2.0/spyder_index/text_splitters/sentence.py
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-10 11:49:29.785606 spyder_index-0.2.0/spyder_index/vector_stores/
+-rw-rw-r--   0 leonardofurnielis   (501) staff       (20)      128 2024-05-07 19:55:30.000000 spyder_index-0.2.0/spyder_index/vector_stores/__init__.py
+-rw-rw-r--   0 leonardofurnielis   (501) staff       (20)     7619 2024-05-07 19:55:41.000000 spyder_index-0.2.0/spyder_index/vector_stores/elasticsearch.py
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-10 11:49:29.789024 spyder_index-0.2.0/spyder_index.egg-info/
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)     9471 2024-05-10 11:49:29.000000 spyder_index-0.2.0/spyder_index.egg-info/PKG-INFO
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)     1021 2024-05-10 11:49:29.000000 spyder_index-0.2.0/spyder_index.egg-info/SOURCES.txt
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)        1 2024-05-10 11:49:29.000000 spyder_index-0.2.0/spyder_index.egg-info/dependency_links.txt
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)      237 2024-05-10 11:49:29.000000 spyder_index-0.2.0/spyder_index.egg-info/requires.txt
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)       13 2024-05-10 11:49:29.000000 spyder_index-0.2.0/spyder_index.egg-info/top_level.txt
```

### Comparing `spyder_index-0.1.2/LICENSE` & `spyder_index-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spyder_index-0.1.2/PKG-INFO` & `spyder_index-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,68 +1,80 @@
 Metadata-Version: 2.1
 Name: spyder-index
-Version: 0.1.2
+Version: 0.2.0
 Summary: Spyder Index is an open-source framework for building LLM applications
 Author: Leonardo Furnielis
 License: MIT License
 Project-URL: Homepage, https://github.com/leonardofurnielis/spyder_index
 Project-URL: Issues, https://github.com/leonardofurnielis/spyder_index/issues
 Keywords: framework,RAG,index,data,LLM,AI,semantic search
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: llama-index-core~=0.10.30
-Requires-Dist: llama-index-readers-file~=0.1.19
 Requires-Dist: langchain-core~=0.1.48
 Requires-Dist: langchain-community~=0.0.36
 Requires-Dist: langchain-text-splitters~=0.0.1
 Requires-Dist: langchain-experimental~=0.0.57
 Requires-Dist: sentence-transformers~=2.7.0
 Requires-Dist: pydantic~=2.7.1
 Requires-Dist: pypdf~=4.2.0
 Requires-Dist: torch==2.1.0
 Requires-Dist: elasticsearch~=8.13.0
 Requires-Dist: ibm-cos-sdk~=2.13.2
+Requires-Dist: jq~=1.7.0
 
-# Spyder Index
+# 🕸️ Spyder Index
+
+![PyPI - Version](https://img.shields.io/pypi/v/spyder-index)
+![PyPI - License](https://img.shields.io/pypi/l/spyder-index)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/spyder-index)
+
+## Installation 
+
+```bash
+pip install spyder-index
+```
 
 ## Table of Contents
 
 - Embeddings
   - [HuggingFace](#embeddings-huggingface)
-- Ingestion
-  - [Directory Files](#ingestion-directory-files)
-  - [IBM Cloud Object Storage (s3)](#ingestion-ibm-cloud-object-store-s3)
-  - [JSON](#ingestion-json)
+- Readers
+  - [Directory](#readers-directory)
+  - [JSON File](#readers-json)
+  - [PDF File](#readers-pdf)
+  - [S3](#readers-s3)
 - Text Splitter
   - [Semantic Splitter](#text-splitter-semantic-splitter)
   - [Sentence Splitter](#text-splitter-sentence-splitter)
 - Vector Store
   - [Elasticsearch](#vector-store-elasticsearch)
 
 ## Embeddings: HuggingFace
 
 ### Overview
 Class for computing text embeddings using HuggingFace models.
 
 ### API Reference
 
-`from spyder_index.embeddings import HuggingFaceEmbeddings`
+```py 
+from spyder_index.embeddings import HuggingFaceEmbeddings
+```
 
 ##### **`HuggingFaceEmbeddings(model_name: str= "sentence-transformers/all-MiniLM-L6-v2", device: Literal["cpu", "cuda"] = "cpu")`**
 
 Initialize a HuggingFaceEmbeddings object.
 
-- `model_name` (str, optional): Name of the HuggingFace model to be used. Defaults to "sentence-transformers/all-MiniLM-L6-v2".
-- `device` (Literal["cpu", "cuda"], optional): Device to run the model on. Defaults to "cpu".
+- `model_name` (str, optional): Name of the HuggingFace model to be used. Defaults to `sentence-transformers/all-MiniLM-L6-v2`.
+- `device` (Literal["cpu", "cuda"], optional): Device to run the model on. Defaults to `cpu`.
 
 ##### **`get_query_embedding(query: str) -> List[float]`**
 
 Compute embedding for a query.
 
 - `text` (str): Input query to compute embedding.
 
@@ -74,91 +86,125 @@
 
 ##### **`get_documents_embedding(documents: List[str]) -> List[List[float]]`**
 
 Compute embeddings for a list of Documents.
 
 - `documents` (List[Documents])
 
-## Ingestion: Directory Files
+## Readers: Directory
 
 ### Overview
-This class provides functionality to load documents from a directory using various file loaders.
+This class provides functionality to load documents from a directory.
 
 ### API Reference
 
-`from spyder_index.ingestion import DirectoryLoader`
+```py 
+from spyder_index.readers import DirectoryReader
+```
+
+##### **`DirectoryReader(input_dir: str, extra_info: Optional[dict], recursive: bool)`**
+
+Initialize a DirectoryReader object.
 
-##### **`load_data(dir: str) -> List[Document]`**
+- `input_dir` (str): The directory path from which to load the documents.
+- `extra_info` (Optional[dict]): Additional metadata to include in the document.
+- `recursive` (Optional[bool]): Whether to recursively search for files. Defaults to `False`.
+
+##### **`load_data() -> List[Document]`**
 
 Loads data from the specified directory.
 
-- `dir` (str): The directory path from which to load the documents.
-- `metadata` (Optional[dict]): Additional metadata to include in the document.
+## Readers: JSON
+
+### Overview
+
+Loads data from JSON.
+
+### API Reference
+
+```py 
+from spyder_index.readers.file import JSONReader
+```
 
-## Ingestion: IBM Cloud Object Store (s3)
+##### **`JSONReader(input_file: str, jq_schema: str, text_content: bool)`**
+
+Initialize an JSONReader object.
+- `input_file` (str): File path to read.
+- `jq_schema` (str): The jq schema to use to extract the data from the JSON.
+- `text_content` (bool): Flag to indicate whether the content is in string format. Default is `False`
+
+##### **`load_data() -> List[Document]`**
+
+Loads data from the specified directory.
+
+## Readers: PDF
 
 ### Overview
-Loads data from IBM Cloud Object Storage (COS) using S3 interface.
+
+Loads data from PDF.
 
 ### API Reference
 
-`from spyder_index.ingestion import IBMS3Loader`
+```py 
+from spyder_index.readers.file import PDFReader
+```
 
-##### **`IBMS3Loader(bucket: str, ibm_api_key_id: str, ibm_service_instance_id: str, s3_endpoint_url: str)`**
+##### **`PDFReader(input_file: str)`**
 
-Initialize an IBMS3Loader object.
+Initialize an PDFReader object.
 
-- `bucket` (str): The name of the IBM COS bucket.
-- `ibm_api_key_id` (str): The IBM Cloud API key ID for accessing the bucket.
-- `ibm_service_instance_id` (str): The service instance ID for the IBM COS.
-- `s3_endpoint_url` (str): The endpoint URL for the IBM COS S3 service.
+- `input_file` (str)
 
 ##### **`load_data() -> List[Document]`**
 
 Loads data from the specified directory.
 
-## Ingestion: JSON
+## Readers: S3
 
 ### Overview
-Loads data from JSON.
+Loads data from S3 bucket.
 
 ### API Reference
 
-`from spyder_index.ingestion import JSONLoader`
+```py 
+from spyder_index.readers import S3Reader
+```
 
-##### **`JSONLoader(jq_schema: str, text_content: bool)`**
+##### **`S3Reader(bucket: str, ibm_api_key_id: str, ibm_service_instance_id: str, s3_endpoint_url: str)`**
 
-Initialize an JSONLoader object.
+Initialize an S3Reader object.
 
-- `jq_schema` (str): The jq schema to use to extract the data from the JSON.
-- `text_content` (bool): Flag to indicate whether the content is in string format. Default is `False`
+- `bucket` (str): The name of the IBM COS bucket.
+- `ibm_api_key_id` (str): The IBM Cloud API key ID for accessing the bucket.
+- `ibm_service_instance_id` (str): The service instance ID for the IBM COS.
+- `s3_endpoint_url` (str): The endpoint URL for the IBM COS S3 service.
 
 ##### **`load_data() -> List[Document]`**
 
 Loads data from the specified directory.
 
-- `file` (str): The file path of JSON.
-
 ## Text Splitter: Semantic Splitter
 
 ### Overview
 Semantic Splitter is a Python class designed to split text into chunks using semantic understanding. It utilizes pre-trained embeddings to identify breakpoints in the text and divide it into meaningful segments.
 
 ### API Reference
 
-`from spyder_index.text_splitters import SemanticSplitter`
+```py 
+from spyder_index.text_splitters import SemanticSplitter
+```
 
 ##### **`SemanticSplitter(model_name: str = "sentence-transformers/all-MiniLM-L6-v2", buffer_size: int = 1, breakpoint_threshold_amount: int = 95, device: Literal["cpu", "cuda"] = "cpu") -> None`**
 
 Initialize the SemanticSplitter instance.
 
-- `model_name`: Name of the pre-trained embeddings model to use. Default is "sentence-transformers/all-MiniLM-L6-v2".
-- `buffer_size`: Size of the buffer for semantic chunking. Default is 1.
-- `breakpoint_threshold_amount`: Threshold percentage for detecting breakpoints. Default is 95.
-- `device`: Device to use for processing, either "cpu" or "cuda". Default is "cpu".
+- `model_name`: Name of the pre-trained embeddings model to use. Default is `sentence-transformers/all-MiniLM-L6-v2`.
+- `buffer_size`: Size of the buffer for semantic chunking. Default is `1`.
+- `breakpoint_threshold_amount`: Threshold percentage for detecting breakpoints. Default is `95`.
+- `device`: Device to use for processing, either "cpu" or "cuda". Default is `cpu`.
 
 ##### **`from_text(text: str) -> List[str]`**
 
 Split text into chunks.
 - `text`: Input text to split.
 
 ##### **`from_documents(documents: List[Document]) -> List[Document]`**
@@ -169,23 +215,24 @@
 ## Text Splitter: Sentence Splitter
 
 ### Overview
 This Python class `SentenceSplitter` is designed to split input text into smaller chunks, particularly useful for processing large documents or texts. It provides methods to split text into chunks and to split a list of documents into chunks.
 
 ### API Reference
 
-`from spyder_index.text_splitters import SentenceSplitter`
+```py 
+from spyder_index.text_splitters import SentenceSplitter
+```
 
-##### **`SentenceSplitter(chunk_size: int = 512, chunk_overlap: int = 256, length_function = len, separators: List[str] = ["\n\n", "\n", " ", ""]) -> None`**
+##### **`SentenceSplitter(chunk_size: int = 512, chunk_overlap: int = 256, separators: List[str] = ["\n\n", "\n", " ", ""]) -> None`**
 
 Creates a new instance of the `SentenceSplitter` class.
 
-- `chunk_size` (int, optional): Size of each chunk. Default is 512.
-- `chunk_overlap` (int, optional): Amount of overlap between chunks. Default is 256.
-- `length_function` (function, optional): Function to compute the length of the text. Default is `len`.
+- `chunk_size` (int, optional): Size of each chunk. Default is `512`.
+- `chunk_overlap` (int, optional): Amount of overlap between chunks. Default is `256`.
 - `separators` (List[str], optional): List of separators used to split the text into chunks. Default separators are `["\n\n", "\n", " ", ""]`.
 
 
 ##### **`from_text(text: str) -> List[str]`**
 
 Splits the input text into chunks.
 
@@ -200,44 +247,46 @@
 ## Vector Store: Elasticsearch
 
 ### Overview
 The `ElasticsearchVectorStore` class provides functionality to interact with Elasticsearch for storing and querying document embeddings. It facilitates adding documents, performing similarity searches, and deleting documents from an Elasticsearch index.
 
 ### API Reference
 
-`from spyder_index.vector_stores import ElasticsearchVectorStore`
+```py 
+from spyder_index.vector_stores import ElasticsearchVectorStore
+```
 
 ##### **`ElasticsearchVectorStore(index_name, es_hostname, es_user, es_password, dims_length, embedding, batch_size=200, ssl=False, distance_strategy="cosine", text_field="text", vector_field="embedding")`**
 
 Initializes the ElasticsearchVectorStore instance.
 
 - `index_name`: The name of the Elasticsearch index.
 - `es_hostname`: The hostname of the Elasticsearch instance.
 - `es_user`: The username for authentication.
 - `es_password`: The password for authentication.
 - `dims_length`: The length of the embedding dimensions.
 - `embedding`: An instance of embeddings.
-- `batch_size`: The batch size for bulk operations. Defaults to 200.
-- `ssl`: Whether to use SSL. Defaults to False.
-- `distance_strategy`: The distance strategy for similarity search. Defaults to "cosine".
-- `text_field`: The name of the field containing text. Defaults to "text".
-- `vector_field`: The name of the field containing vector embeddings. Defaults to "embedding".
+- `batch_size`: The batch size for bulk operations. Defaults to `200`.
+- `ssl`: Whether to use SSL. Defaults to `False`.
+- `distance_strategy`: The distance strategy for similarity search. Defaults to `cosine`.
+- `text_field`: The name of the field containing text. Defaults to `text`.
+- `vector_field`: The name of the field containing vector embeddings. Defaults to `embedding`.
 
 ##### **`add_documents(documents, create_index_if_not_exists=True)`**
 
 Adds documents to the Elasticsearch index.
 
 - `documents`: A list of Document objects to add to the index.
-- `create_index_if_not_exists`: Whether to create the index if it doesn't exist. Defaults to True.
+- `create_index_if_not_exists`: Whether to create the index if it doesn't exist. Defaults to `True`.
 
 ##### **`similarity_search(query, top_k=4)`**
 
 Performs a similarity search based on the documents most similar to the query.
 
 - `query`: The query text.
-- `top_k`: The number of top results to return. Defaults to 4.
+- `top_k`: The number of top results to return. Defaults to `4`.
 
 ##### **`delete(ids=None)`**
 
 Deletes documents from the Elasticsearch index.
 
-- `ids`: A list of document IDs to delete. Defaults to None.
+- `ids`: A list of document IDs to delete. Defaults to `None`.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `spyder_index-0.1.2/README.md` & `spyder_index-0.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,51 @@
-# Spyder Index
+# 🕸️ Spyder Index
+
+![PyPI - Version](https://img.shields.io/pypi/v/spyder-index)
+![PyPI - License](https://img.shields.io/pypi/l/spyder-index)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/spyder-index)
+
+## Installation 
+
+```bash
+pip install spyder-index
+```
 
 ## Table of Contents
 
 - Embeddings
   - [HuggingFace](#embeddings-huggingface)
-- Ingestion
-  - [Directory Files](#ingestion-directory-files)
-  - [IBM Cloud Object Storage (s3)](#ingestion-ibm-cloud-object-store-s3)
-  - [JSON](#ingestion-json)
+- Readers
+  - [Directory](#readers-directory)
+  - [JSON File](#readers-json)
+  - [PDF File](#readers-pdf)
+  - [S3](#readers-s3)
 - Text Splitter
   - [Semantic Splitter](#text-splitter-semantic-splitter)
   - [Sentence Splitter](#text-splitter-sentence-splitter)
 - Vector Store
   - [Elasticsearch](#vector-store-elasticsearch)
 
 ## Embeddings: HuggingFace
 
 ### Overview
 Class for computing text embeddings using HuggingFace models.
 
 ### API Reference
 
-`from spyder_index.embeddings import HuggingFaceEmbeddings`
+```py 
+from spyder_index.embeddings import HuggingFaceEmbeddings
+```
 
 ##### **`HuggingFaceEmbeddings(model_name: str= "sentence-transformers/all-MiniLM-L6-v2", device: Literal["cpu", "cuda"] = "cpu")`**
 
 Initialize a HuggingFaceEmbeddings object.
 
-- `model_name` (str, optional): Name of the HuggingFace model to be used. Defaults to "sentence-transformers/all-MiniLM-L6-v2".
-- `device` (Literal["cpu", "cuda"], optional): Device to run the model on. Defaults to "cpu".
+- `model_name` (str, optional): Name of the HuggingFace model to be used. Defaults to `sentence-transformers/all-MiniLM-L6-v2`.
+- `device` (Literal["cpu", "cuda"], optional): Device to run the model on. Defaults to `cpu`.
 
 ##### **`get_query_embedding(query: str) -> List[float]`**
 
 Compute embedding for a query.
 
 - `text` (str): Input query to compute embedding.
 
@@ -44,91 +57,125 @@
 
 ##### **`get_documents_embedding(documents: List[str]) -> List[List[float]]`**
 
 Compute embeddings for a list of Documents.
 
 - `documents` (List[Documents])
 
-## Ingestion: Directory Files
+## Readers: Directory
 
 ### Overview
-This class provides functionality to load documents from a directory using various file loaders.
+This class provides functionality to load documents from a directory.
 
 ### API Reference
 
-`from spyder_index.ingestion import DirectoryLoader`
+```py 
+from spyder_index.readers import DirectoryReader
+```
+
+##### **`DirectoryReader(input_dir: str, extra_info: Optional[dict], recursive: bool)`**
+
+Initialize a DirectoryReader object.
 
-##### **`load_data(dir: str) -> List[Document]`**
+- `input_dir` (str): The directory path from which to load the documents.
+- `extra_info` (Optional[dict]): Additional metadata to include in the document.
+- `recursive` (Optional[bool]): Whether to recursively search for files. Defaults to `False`.
+
+##### **`load_data() -> List[Document]`**
 
 Loads data from the specified directory.
 
-- `dir` (str): The directory path from which to load the documents.
-- `metadata` (Optional[dict]): Additional metadata to include in the document.
+## Readers: JSON
+
+### Overview
+
+Loads data from JSON.
+
+### API Reference
+
+```py 
+from spyder_index.readers.file import JSONReader
+```
 
-## Ingestion: IBM Cloud Object Store (s3)
+##### **`JSONReader(input_file: str, jq_schema: str, text_content: bool)`**
+
+Initialize an JSONReader object.
+- `input_file` (str): File path to read.
+- `jq_schema` (str): The jq schema to use to extract the data from the JSON.
+- `text_content` (bool): Flag to indicate whether the content is in string format. Default is `False`
+
+##### **`load_data() -> List[Document]`**
+
+Loads data from the specified directory.
+
+## Readers: PDF
 
 ### Overview
-Loads data from IBM Cloud Object Storage (COS) using S3 interface.
+
+Loads data from PDF.
 
 ### API Reference
 
-`from spyder_index.ingestion import IBMS3Loader`
+```py 
+from spyder_index.readers.file import PDFReader
+```
 
-##### **`IBMS3Loader(bucket: str, ibm_api_key_id: str, ibm_service_instance_id: str, s3_endpoint_url: str)`**
+##### **`PDFReader(input_file: str)`**
 
-Initialize an IBMS3Loader object.
+Initialize an PDFReader object.
 
-- `bucket` (str): The name of the IBM COS bucket.
-- `ibm_api_key_id` (str): The IBM Cloud API key ID for accessing the bucket.
-- `ibm_service_instance_id` (str): The service instance ID for the IBM COS.
-- `s3_endpoint_url` (str): The endpoint URL for the IBM COS S3 service.
+- `input_file` (str)
 
 ##### **`load_data() -> List[Document]`**
 
 Loads data from the specified directory.
 
-## Ingestion: JSON
+## Readers: S3
 
 ### Overview
-Loads data from JSON.
+Loads data from S3 bucket.
 
 ### API Reference
 
-`from spyder_index.ingestion import JSONLoader`
+```py 
+from spyder_index.readers import S3Reader
+```
 
-##### **`JSONLoader(jq_schema: str, text_content: bool)`**
+##### **`S3Reader(bucket: str, ibm_api_key_id: str, ibm_service_instance_id: str, s3_endpoint_url: str)`**
 
-Initialize an JSONLoader object.
+Initialize an S3Reader object.
 
-- `jq_schema` (str): The jq schema to use to extract the data from the JSON.
-- `text_content` (bool): Flag to indicate whether the content is in string format. Default is `False`
+- `bucket` (str): The name of the IBM COS bucket.
+- `ibm_api_key_id` (str): The IBM Cloud API key ID for accessing the bucket.
+- `ibm_service_instance_id` (str): The service instance ID for the IBM COS.
+- `s3_endpoint_url` (str): The endpoint URL for the IBM COS S3 service.
 
 ##### **`load_data() -> List[Document]`**
 
 Loads data from the specified directory.
 
-- `file` (str): The file path of JSON.
-
 ## Text Splitter: Semantic Splitter
 
 ### Overview
 Semantic Splitter is a Python class designed to split text into chunks using semantic understanding. It utilizes pre-trained embeddings to identify breakpoints in the text and divide it into meaningful segments.
 
 ### API Reference
 
-`from spyder_index.text_splitters import SemanticSplitter`
+```py 
+from spyder_index.text_splitters import SemanticSplitter
+```
 
 ##### **`SemanticSplitter(model_name: str = "sentence-transformers/all-MiniLM-L6-v2", buffer_size: int = 1, breakpoint_threshold_amount: int = 95, device: Literal["cpu", "cuda"] = "cpu") -> None`**
 
 Initialize the SemanticSplitter instance.
 
-- `model_name`: Name of the pre-trained embeddings model to use. Default is "sentence-transformers/all-MiniLM-L6-v2".
-- `buffer_size`: Size of the buffer for semantic chunking. Default is 1.
-- `breakpoint_threshold_amount`: Threshold percentage for detecting breakpoints. Default is 95.
-- `device`: Device to use for processing, either "cpu" or "cuda". Default is "cpu".
+- `model_name`: Name of the pre-trained embeddings model to use. Default is `sentence-transformers/all-MiniLM-L6-v2`.
+- `buffer_size`: Size of the buffer for semantic chunking. Default is `1`.
+- `breakpoint_threshold_amount`: Threshold percentage for detecting breakpoints. Default is `95`.
+- `device`: Device to use for processing, either "cpu" or "cuda". Default is `cpu`.
 
 ##### **`from_text(text: str) -> List[str]`**
 
 Split text into chunks.
 - `text`: Input text to split.
 
 ##### **`from_documents(documents: List[Document]) -> List[Document]`**
@@ -139,23 +186,24 @@
 ## Text Splitter: Sentence Splitter
 
 ### Overview
 This Python class `SentenceSplitter` is designed to split input text into smaller chunks, particularly useful for processing large documents or texts. It provides methods to split text into chunks and to split a list of documents into chunks.
 
 ### API Reference
 
-`from spyder_index.text_splitters import SentenceSplitter`
+```py 
+from spyder_index.text_splitters import SentenceSplitter
+```
 
-##### **`SentenceSplitter(chunk_size: int = 512, chunk_overlap: int = 256, length_function = len, separators: List[str] = ["\n\n", "\n", " ", ""]) -> None`**
+##### **`SentenceSplitter(chunk_size: int = 512, chunk_overlap: int = 256, separators: List[str] = ["\n\n", "\n", " ", ""]) -> None`**
 
 Creates a new instance of the `SentenceSplitter` class.
 
-- `chunk_size` (int, optional): Size of each chunk. Default is 512.
-- `chunk_overlap` (int, optional): Amount of overlap between chunks. Default is 256.
-- `length_function` (function, optional): Function to compute the length of the text. Default is `len`.
+- `chunk_size` (int, optional): Size of each chunk. Default is `512`.
+- `chunk_overlap` (int, optional): Amount of overlap between chunks. Default is `256`.
 - `separators` (List[str], optional): List of separators used to split the text into chunks. Default separators are `["\n\n", "\n", " ", ""]`.
 
 
 ##### **`from_text(text: str) -> List[str]`**
 
 Splits the input text into chunks.
 
@@ -170,44 +218,46 @@
 ## Vector Store: Elasticsearch
 
 ### Overview
 The `ElasticsearchVectorStore` class provides functionality to interact with Elasticsearch for storing and querying document embeddings. It facilitates adding documents, performing similarity searches, and deleting documents from an Elasticsearch index.
 
 ### API Reference
 
-`from spyder_index.vector_stores import ElasticsearchVectorStore`
+```py 
+from spyder_index.vector_stores import ElasticsearchVectorStore
+```
 
 ##### **`ElasticsearchVectorStore(index_name, es_hostname, es_user, es_password, dims_length, embedding, batch_size=200, ssl=False, distance_strategy="cosine", text_field="text", vector_field="embedding")`**
 
 Initializes the ElasticsearchVectorStore instance.
 
 - `index_name`: The name of the Elasticsearch index.
 - `es_hostname`: The hostname of the Elasticsearch instance.
 - `es_user`: The username for authentication.
 - `es_password`: The password for authentication.
 - `dims_length`: The length of the embedding dimensions.
 - `embedding`: An instance of embeddings.
-- `batch_size`: The batch size for bulk operations. Defaults to 200.
-- `ssl`: Whether to use SSL. Defaults to False.
-- `distance_strategy`: The distance strategy for similarity search. Defaults to "cosine".
-- `text_field`: The name of the field containing text. Defaults to "text".
-- `vector_field`: The name of the field containing vector embeddings. Defaults to "embedding".
+- `batch_size`: The batch size for bulk operations. Defaults to `200`.
+- `ssl`: Whether to use SSL. Defaults to `False`.
+- `distance_strategy`: The distance strategy for similarity search. Defaults to `cosine`.
+- `text_field`: The name of the field containing text. Defaults to `text`.
+- `vector_field`: The name of the field containing vector embeddings. Defaults to `embedding`.
 
 ##### **`add_documents(documents, create_index_if_not_exists=True)`**
 
 Adds documents to the Elasticsearch index.
 
 - `documents`: A list of Document objects to add to the index.
-- `create_index_if_not_exists`: Whether to create the index if it doesn't exist. Defaults to True.
+- `create_index_if_not_exists`: Whether to create the index if it doesn't exist. Defaults to `True`.
 
 ##### **`similarity_search(query, top_k=4)`**
 
 Performs a similarity search based on the documents most similar to the query.
 
 - `query`: The query text.
-- `top_k`: The number of top results to return. Defaults to 4.
+- `top_k`: The number of top results to return. Defaults to `4`.
 
 ##### **`delete(ids=None)`**
 
 Deletes documents from the Elasticsearch index.
 
-- `ids`: A list of document IDs to delete. Defaults to None.
+- `ids`: A list of document IDs to delete. Defaults to `None`.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `spyder_index-0.1.2/pyproject.toml` & `spyder_index-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 [build-system]
 requires = ["setuptools >= 61.0","wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spyder-index"
-version = "0.1.2"
+version = "0.2.0"
 description = "Spyder Index is an open-source framework for building LLM applications"
 readme = "README.md"
 authors = [{ name = "Leonardo Furnielis" }]
 license = {text = "MIT License"}
 keywords = ["framework", "RAG", "index", "data", "LLM", "AI", "semantic search"]
 dependencies = [
-    "llama-index-core ~= 0.10.30",
-    "llama-index-readers-file ~= 0.1.19",
     "langchain-core ~= 0.1.48",
     "langchain-community ~= 0.0.36",
     "langchain-text-splitters ~= 0.0.1",
     "langchain-experimental ~= 0.0.57",
     "sentence-transformers ~= 2.7.0",
     "pydantic ~= 2.7.1",
     "pypdf ~= 4.2.0",
     "torch == 2.1.0",
     "elasticsearch ~= 8.13.0",
-    "ibm-cos-sdk ~= 2.13.2"
+    "ibm-cos-sdk ~= 2.13.2",
+    "jq ~= 1.7.0"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
```

### Comparing `spyder_index-0.1.2/spyder_index/core/document/base.py` & `spyder_index-0.2.0/spyder_index/core/document/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import uuid
 import mimetypes
 from typing import TYPE_CHECKING, Literal, Optional
 from datetime import datetime
 from pydantic import BaseModel, Field
 
 if TYPE_CHECKING:
-    from llama_index.core.schema import Document as LlamaIndexDocument
     from langchain_core.documents import Document as LangchainDocument
 
 class Document(BaseModel):
     doc_id: str = Field(default_factory=lambda: str(uuid.uuid4()))
     text: str = Field(default="")
     metadata: dict = Field(default={})
 
@@ -23,34 +22,29 @@
         return self.text
     
     def get_metadata(self) -> dict:
         """Get the metadata of the document."""
         return self.metadata
     
     @classmethod
-    def _convert_metadata(cls, metadata: dict, framework: Literal["llama_index", "langchain"]) -> dict:
+    def _convert_metadata(cls, metadata: dict, framework: Literal["langchain"]) -> dict:
         """
         Convert metadata based on the framework (supported llama_index, langchain).
 
         Args:
             metadata (dict): Metadata to convert.
             framework (Literal["llama_index", "langchain"]): Framework indicator.
 
         Returns:
             dict: converted metadata.
         """
         today = datetime.now()
         _metadata: dict = {}
         _metadata["creation_date"] = "%s-%s-%s" % (today.year, today.month, today.day)
 
-        if framework == "llama_index":
-            _metadata["page"] = metadata.get("page_label")
-            _metadata["file_name"] = metadata.get("file_name")
-            _metadata["file_type"] = metadata.get("file_type")
-
         if framework == "langchain":
             _metadata["page"] = metadata.get("page")
             _metadata["file_name"] = os.path.basename(metadata.get("source"))
             _metadata["file_type"] = mimetypes.guess_type(_metadata["file_name"])[0]
 
             if type(_metadata.get("page")) == int:
                 _metadata.get("page") + 1
@@ -67,26 +61,7 @@
 
         Returns:
             Document: Converted document.
         """
         
         converted_metadata = cls._convert_metadata(doc.metadata, "langchain")
         return cls(text=doc.page_content, metadata=converted_metadata)
-    
-    @classmethod
-    def _from_llama_index_format(cls, doc: "LlamaIndexDocument", metadata: Optional[dict] = None) -> "Document":
-        """
-        Convert a document from LlamaIndex format to spyder_index Document format.
-
-        Args:
-            doc (LlamaIndexDocument): Document in LlamaIndex format.
-            metadata (Optional[dict]): Additional metadata to include in the converted document.
-
-        Returns:
-            Document: Converted document.
-        """
-        converted_metadata = cls._convert_metadata(doc.metadata, "llama_index")
-        
-        if metadata:
-            converted_metadata = metadata | converted_metadata
-
-        return cls(text=doc.text, metadata=converted_metadata)
```

### Comparing `spyder_index-0.1.2/spyder_index/core/embeddings/base.py` & `spyder_index-0.2.0/spyder_index/core/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `spyder_index-0.1.2/spyder_index/embeddings/huggingface.py` & `spyder_index-0.2.0/spyder_index/embeddings/huggingface.py`

 * *Files identical despite different names*

### Comparing `spyder_index-0.1.2/spyder_index/text_splitters/semantic.py` & `spyder_index-0.2.0/spyder_index/text_splitters/semantic.py`

 * *Files identical despite different names*

### Comparing `spyder_index-0.1.2/spyder_index/text_splitters/sentence.py` & `spyder_index-0.2.0/spyder_index/text_splitters/sentence.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,22 +5,20 @@
 from langchain_text_splitters.character import RecursiveCharacterTextSplitter
 
 class SentenceSplitter():
 
     def __init__(self, 
                  chunk_size: int = 512 , 
                  chunk_overlap: int = 256,
-                 length_function = len,
                  separators = ["\n\n", "\n", " ", ""]
                  ) -> None:
 
         
         self.chunk_size = chunk_size
         self.chunk_overlap = chunk_overlap
-        self.length_function = length_function
         self.separators = separators
 
 
     def from_text(self, text: str) -> List[str]: 
         """
         Split text into chunks.
         
@@ -29,15 +27,14 @@
         
         Returns:
         - List[str]: List of chunks.
         """
         text_splitter = RecursiveCharacterTextSplitter(
             chunk_size=self.chunk_size,
             chunk_overlap=self.chunk_overlap,
-            length_function=self.length_function,
             separators=self.separators,
         )
         
         return text_splitter.split_text(text)
 
     
     def from_documents(self, documents: List[Document]) -> List[Document]:
```

### Comparing `spyder_index-0.1.2/spyder_index/vector_stores/elasticsearch.py` & `spyder_index-0.2.0/spyder_index/vector_stores/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `spyder_index-0.1.2/spyder_index.egg-info/PKG-INFO` & `spyder_index-0.2.0/spyder_index.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,68 +1,80 @@
 Metadata-Version: 2.1
 Name: spyder-index
-Version: 0.1.2
+Version: 0.2.0
 Summary: Spyder Index is an open-source framework for building LLM applications
 Author: Leonardo Furnielis
 License: MIT License
 Project-URL: Homepage, https://github.com/leonardofurnielis/spyder_index
 Project-URL: Issues, https://github.com/leonardofurnielis/spyder_index/issues
 Keywords: framework,RAG,index,data,LLM,AI,semantic search
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: llama-index-core~=0.10.30
-Requires-Dist: llama-index-readers-file~=0.1.19
 Requires-Dist: langchain-core~=0.1.48
 Requires-Dist: langchain-community~=0.0.36
 Requires-Dist: langchain-text-splitters~=0.0.1
 Requires-Dist: langchain-experimental~=0.0.57
 Requires-Dist: sentence-transformers~=2.7.0
 Requires-Dist: pydantic~=2.7.1
 Requires-Dist: pypdf~=4.2.0
 Requires-Dist: torch==2.1.0
 Requires-Dist: elasticsearch~=8.13.0
 Requires-Dist: ibm-cos-sdk~=2.13.2
+Requires-Dist: jq~=1.7.0
 
-# Spyder Index
+# 🕸️ Spyder Index
+
+![PyPI - Version](https://img.shields.io/pypi/v/spyder-index)
+![PyPI - License](https://img.shields.io/pypi/l/spyder-index)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/spyder-index)
+
+## Installation 
+
+```bash
+pip install spyder-index
+```
 
 ## Table of Contents
 
 - Embeddings
   - [HuggingFace](#embeddings-huggingface)
-- Ingestion
-  - [Directory Files](#ingestion-directory-files)
-  - [IBM Cloud Object Storage (s3)](#ingestion-ibm-cloud-object-store-s3)
-  - [JSON](#ingestion-json)
+- Readers
+  - [Directory](#readers-directory)
+  - [JSON File](#readers-json)
+  - [PDF File](#readers-pdf)
+  - [S3](#readers-s3)
 - Text Splitter
   - [Semantic Splitter](#text-splitter-semantic-splitter)
   - [Sentence Splitter](#text-splitter-sentence-splitter)
 - Vector Store
   - [Elasticsearch](#vector-store-elasticsearch)
 
 ## Embeddings: HuggingFace
 
 ### Overview
 Class for computing text embeddings using HuggingFace models.
 
 ### API Reference
 
-`from spyder_index.embeddings import HuggingFaceEmbeddings`
+```py 
+from spyder_index.embeddings import HuggingFaceEmbeddings
+```
 
 ##### **`HuggingFaceEmbeddings(model_name: str= "sentence-transformers/all-MiniLM-L6-v2", device: Literal["cpu", "cuda"] = "cpu")`**
 
 Initialize a HuggingFaceEmbeddings object.
 
-- `model_name` (str, optional): Name of the HuggingFace model to be used. Defaults to "sentence-transformers/all-MiniLM-L6-v2".
-- `device` (Literal["cpu", "cuda"], optional): Device to run the model on. Defaults to "cpu".
+- `model_name` (str, optional): Name of the HuggingFace model to be used. Defaults to `sentence-transformers/all-MiniLM-L6-v2`.
+- `device` (Literal["cpu", "cuda"], optional): Device to run the model on. Defaults to `cpu`.
 
 ##### **`get_query_embedding(query: str) -> List[float]`**
 
 Compute embedding for a query.
 
 - `text` (str): Input query to compute embedding.
 
@@ -74,91 +86,125 @@
 
 ##### **`get_documents_embedding(documents: List[str]) -> List[List[float]]`**
 
 Compute embeddings for a list of Documents.
 
 - `documents` (List[Documents])
 
-## Ingestion: Directory Files
+## Readers: Directory
 
 ### Overview
-This class provides functionality to load documents from a directory using various file loaders.
+This class provides functionality to load documents from a directory.
 
 ### API Reference
 
-`from spyder_index.ingestion import DirectoryLoader`
+```py 
+from spyder_index.readers import DirectoryReader
+```
+
+##### **`DirectoryReader(input_dir: str, extra_info: Optional[dict], recursive: bool)`**
+
+Initialize a DirectoryReader object.
 
-##### **`load_data(dir: str) -> List[Document]`**
+- `input_dir` (str): The directory path from which to load the documents.
+- `extra_info` (Optional[dict]): Additional metadata to include in the document.
+- `recursive` (Optional[bool]): Whether to recursively search for files. Defaults to `False`.
+
+##### **`load_data() -> List[Document]`**
 
 Loads data from the specified directory.
 
-- `dir` (str): The directory path from which to load the documents.
-- `metadata` (Optional[dict]): Additional metadata to include in the document.
+## Readers: JSON
+
+### Overview
+
+Loads data from JSON.
+
+### API Reference
+
+```py 
+from spyder_index.readers.file import JSONReader
+```
 
-## Ingestion: IBM Cloud Object Store (s3)
+##### **`JSONReader(input_file: str, jq_schema: str, text_content: bool)`**
+
+Initialize an JSONReader object.
+- `input_file` (str): File path to read.
+- `jq_schema` (str): The jq schema to use to extract the data from the JSON.
+- `text_content` (bool): Flag to indicate whether the content is in string format. Default is `False`
+
+##### **`load_data() -> List[Document]`**
+
+Loads data from the specified directory.
+
+## Readers: PDF
 
 ### Overview
-Loads data from IBM Cloud Object Storage (COS) using S3 interface.
+
+Loads data from PDF.
 
 ### API Reference
 
-`from spyder_index.ingestion import IBMS3Loader`
+```py 
+from spyder_index.readers.file import PDFReader
+```
 
-##### **`IBMS3Loader(bucket: str, ibm_api_key_id: str, ibm_service_instance_id: str, s3_endpoint_url: str)`**
+##### **`PDFReader(input_file: str)`**
 
-Initialize an IBMS3Loader object.
+Initialize an PDFReader object.
 
-- `bucket` (str): The name of the IBM COS bucket.
-- `ibm_api_key_id` (str): The IBM Cloud API key ID for accessing the bucket.
-- `ibm_service_instance_id` (str): The service instance ID for the IBM COS.
-- `s3_endpoint_url` (str): The endpoint URL for the IBM COS S3 service.
+- `input_file` (str)
 
 ##### **`load_data() -> List[Document]`**
 
 Loads data from the specified directory.
 
-## Ingestion: JSON
+## Readers: S3
 
 ### Overview
-Loads data from JSON.
+Loads data from S3 bucket.
 
 ### API Reference
 
-`from spyder_index.ingestion import JSONLoader`
+```py 
+from spyder_index.readers import S3Reader
+```
 
-##### **`JSONLoader(jq_schema: str, text_content: bool)`**
+##### **`S3Reader(bucket: str, ibm_api_key_id: str, ibm_service_instance_id: str, s3_endpoint_url: str)`**
 
-Initialize an JSONLoader object.
+Initialize an S3Reader object.
 
-- `jq_schema` (str): The jq schema to use to extract the data from the JSON.
-- `text_content` (bool): Flag to indicate whether the content is in string format. Default is `False`
+- `bucket` (str): The name of the IBM COS bucket.
+- `ibm_api_key_id` (str): The IBM Cloud API key ID for accessing the bucket.
+- `ibm_service_instance_id` (str): The service instance ID for the IBM COS.
+- `s3_endpoint_url` (str): The endpoint URL for the IBM COS S3 service.
 
 ##### **`load_data() -> List[Document]`**
 
 Loads data from the specified directory.
 
-- `file` (str): The file path of JSON.
-
 ## Text Splitter: Semantic Splitter
 
 ### Overview
 Semantic Splitter is a Python class designed to split text into chunks using semantic understanding. It utilizes pre-trained embeddings to identify breakpoints in the text and divide it into meaningful segments.
 
 ### API Reference
 
-`from spyder_index.text_splitters import SemanticSplitter`
+```py 
+from spyder_index.text_splitters import SemanticSplitter
+```
 
 ##### **`SemanticSplitter(model_name: str = "sentence-transformers/all-MiniLM-L6-v2", buffer_size: int = 1, breakpoint_threshold_amount: int = 95, device: Literal["cpu", "cuda"] = "cpu") -> None`**
 
 Initialize the SemanticSplitter instance.
 
-- `model_name`: Name of the pre-trained embeddings model to use. Default is "sentence-transformers/all-MiniLM-L6-v2".
-- `buffer_size`: Size of the buffer for semantic chunking. Default is 1.
-- `breakpoint_threshold_amount`: Threshold percentage for detecting breakpoints. Default is 95.
-- `device`: Device to use for processing, either "cpu" or "cuda". Default is "cpu".
+- `model_name`: Name of the pre-trained embeddings model to use. Default is `sentence-transformers/all-MiniLM-L6-v2`.
+- `buffer_size`: Size of the buffer for semantic chunking. Default is `1`.
+- `breakpoint_threshold_amount`: Threshold percentage for detecting breakpoints. Default is `95`.
+- `device`: Device to use for processing, either "cpu" or "cuda". Default is `cpu`.
 
 ##### **`from_text(text: str) -> List[str]`**
 
 Split text into chunks.
 - `text`: Input text to split.
 
 ##### **`from_documents(documents: List[Document]) -> List[Document]`**
@@ -169,23 +215,24 @@
 ## Text Splitter: Sentence Splitter
 
 ### Overview
 This Python class `SentenceSplitter` is designed to split input text into smaller chunks, particularly useful for processing large documents or texts. It provides methods to split text into chunks and to split a list of documents into chunks.
 
 ### API Reference
 
-`from spyder_index.text_splitters import SentenceSplitter`
+```py 
+from spyder_index.text_splitters import SentenceSplitter
+```
 
-##### **`SentenceSplitter(chunk_size: int = 512, chunk_overlap: int = 256, length_function = len, separators: List[str] = ["\n\n", "\n", " ", ""]) -> None`**
+##### **`SentenceSplitter(chunk_size: int = 512, chunk_overlap: int = 256, separators: List[str] = ["\n\n", "\n", " ", ""]) -> None`**
 
 Creates a new instance of the `SentenceSplitter` class.
 
-- `chunk_size` (int, optional): Size of each chunk. Default is 512.
-- `chunk_overlap` (int, optional): Amount of overlap between chunks. Default is 256.
-- `length_function` (function, optional): Function to compute the length of the text. Default is `len`.
+- `chunk_size` (int, optional): Size of each chunk. Default is `512`.
+- `chunk_overlap` (int, optional): Amount of overlap between chunks. Default is `256`.
 - `separators` (List[str], optional): List of separators used to split the text into chunks. Default separators are `["\n\n", "\n", " ", ""]`.
 
 
 ##### **`from_text(text: str) -> List[str]`**
 
 Splits the input text into chunks.
 
@@ -200,44 +247,46 @@
 ## Vector Store: Elasticsearch
 
 ### Overview
 The `ElasticsearchVectorStore` class provides functionality to interact with Elasticsearch for storing and querying document embeddings. It facilitates adding documents, performing similarity searches, and deleting documents from an Elasticsearch index.
 
 ### API Reference
 
-`from spyder_index.vector_stores import ElasticsearchVectorStore`
+```py 
+from spyder_index.vector_stores import ElasticsearchVectorStore
+```
 
 ##### **`ElasticsearchVectorStore(index_name, es_hostname, es_user, es_password, dims_length, embedding, batch_size=200, ssl=False, distance_strategy="cosine", text_field="text", vector_field="embedding")`**
 
 Initializes the ElasticsearchVectorStore instance.
 
 - `index_name`: The name of the Elasticsearch index.
 - `es_hostname`: The hostname of the Elasticsearch instance.
 - `es_user`: The username for authentication.
 - `es_password`: The password for authentication.
 - `dims_length`: The length of the embedding dimensions.
 - `embedding`: An instance of embeddings.
-- `batch_size`: The batch size for bulk operations. Defaults to 200.
-- `ssl`: Whether to use SSL. Defaults to False.
-- `distance_strategy`: The distance strategy for similarity search. Defaults to "cosine".
-- `text_field`: The name of the field containing text. Defaults to "text".
-- `vector_field`: The name of the field containing vector embeddings. Defaults to "embedding".
+- `batch_size`: The batch size for bulk operations. Defaults to `200`.
+- `ssl`: Whether to use SSL. Defaults to `False`.
+- `distance_strategy`: The distance strategy for similarity search. Defaults to `cosine`.
+- `text_field`: The name of the field containing text. Defaults to `text`.
+- `vector_field`: The name of the field containing vector embeddings. Defaults to `embedding`.
 
 ##### **`add_documents(documents, create_index_if_not_exists=True)`**
 
 Adds documents to the Elasticsearch index.
 
 - `documents`: A list of Document objects to add to the index.
-- `create_index_if_not_exists`: Whether to create the index if it doesn't exist. Defaults to True.
+- `create_index_if_not_exists`: Whether to create the index if it doesn't exist. Defaults to `True`.
 
 ##### **`similarity_search(query, top_k=4)`**
 
 Performs a similarity search based on the documents most similar to the query.
 
 - `query`: The query text.
-- `top_k`: The number of top results to return. Defaults to 4.
+- `top_k`: The number of top results to return. Defaults to `4`.
 
 ##### **`delete(ids=None)`**
 
 Deletes documents from the Elasticsearch index.
 
-- `ids`: A list of document IDs to delete. Defaults to None.
+- `ids`: A list of document IDs to delete. Defaults to `None`.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `spyder_index-0.1.2/spyder_index.egg-info/SOURCES.txt` & `spyder_index-0.2.0/spyder_index.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -7,20 +7,24 @@
 spyder_index.egg-info/dependency_links.txt
 spyder_index.egg-info/requires.txt
 spyder_index.egg-info/top_level.txt
 spyder_index/core/document/__init__.py
 spyder_index/core/document/base.py
 spyder_index/core/embeddings/__init__.py
 spyder_index/core/embeddings/base.py
+spyder_index/core/readers/__init__.py
+spyder_index/core/readers/base.py
 spyder_index/core/vector_stores/__init__.py
 spyder_index/core/vector_stores/base.py
 spyder_index/embeddings/__init__.py
 spyder_index/embeddings/huggingface.py
-spyder_index/ingestion/__init__.py
-spyder_index/ingestion/directory_file.py
-spyder_index/ingestion/ibm_cos.py
-spyder_index/ingestion/json.py
+spyder_index/readers/__init__.py
+spyder_index/readers/directory.py
+spyder_index/readers/s3.py
+spyder_index/readers/file/__init__.py
+spyder_index/readers/file/json.py
+spyder_index/readers/file/pdf.py
 spyder_index/text_splitters/__init__.py
 spyder_index/text_splitters/semantic.py
 spyder_index/text_splitters/sentence.py
 spyder_index/vector_stores/__init__.py
 spyder_index/vector_stores/elasticsearch.py
```

