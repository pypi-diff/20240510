# Comparing `tmp/llama_index_packs_cohere_citation_chat-0.1.4.tar.gz` & `tmp/llama_index_packs_cohere_citation_chat-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_packs_cohere_citation_chat-0.1.4.tar", max compression
+gzip compressed data, was "llama_index_packs_cohere_citation_chat-0.1.5.tar", max compression
```

## Comparing `llama_index_packs_cohere_citation_chat-0.1.4.tar` & `llama_index_packs_cohere_citation_chat-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2010 2024-05-07 22:47:10.990522 llama_index_packs_cohere_citation_chat-0.1.4/README.md
--rw-r--r--   0        0        0      129 2024-05-07 22:47:10.990522 llama_index_packs_cohere_citation_chat-0.1.4/llama_index/packs/cohere_citation_chat/__init__.py
--rw-r--r--   0        0        0     1889 2024-05-07 22:47:10.990522 llama_index_packs_cohere_citation_chat-0.1.4/llama_index/packs/cohere_citation_chat/base.py
--rw-r--r--   0        0        0    17396 2024-05-07 22:47:10.990522 llama_index_packs_cohere_citation_chat-0.1.4/llama_index/packs/cohere_citation_chat/citations_context_chat_engine.py
--rw-r--r--   0        0        0      744 2024-05-07 22:47:10.990522 llama_index_packs_cohere_citation_chat-0.1.4/llama_index/packs/cohere_citation_chat/types.py
--rw-r--r--   0        0        0     1688 2024-05-07 22:47:10.990522 llama_index_packs_cohere_citation_chat-0.1.4/llama_index/packs/cohere_citation_chat/utils.py
--rw-r--r--   0        0        0     1670 2024-05-07 22:47:10.990522 llama_index_packs_cohere_citation_chat-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2782 1970-01-01 00:00:00.000000 llama_index_packs_cohere_citation_chat-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     2010 2024-05-10 17:31:25.441083 llama_index_packs_cohere_citation_chat-0.1.5/README.md
+-rw-r--r--   0        0        0      129 2024-05-10 17:31:25.441083 llama_index_packs_cohere_citation_chat-0.1.5/llama_index/packs/cohere_citation_chat/__init__.py
+-rw-r--r--   0        0        0     1889 2024-05-10 17:31:25.441083 llama_index_packs_cohere_citation_chat-0.1.5/llama_index/packs/cohere_citation_chat/base.py
+-rw-r--r--   0        0        0    17396 2024-05-10 17:31:25.441083 llama_index_packs_cohere_citation_chat-0.1.5/llama_index/packs/cohere_citation_chat/citations_context_chat_engine.py
+-rw-r--r--   0        0        0      744 2024-05-10 17:31:25.441083 llama_index_packs_cohere_citation_chat-0.1.5/llama_index/packs/cohere_citation_chat/types.py
+-rw-r--r--   0        0        0     1688 2024-05-10 17:31:25.441083 llama_index_packs_cohere_citation_chat-0.1.5/llama_index/packs/cohere_citation_chat/utils.py
+-rw-r--r--   0        0        0     1671 2024-05-10 17:31:25.441083 llama_index_packs_cohere_citation_chat-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2775 1970-01-01 00:00:00.000000 llama_index_packs_cohere_citation_chat-0.1.5/PKG-INFO
```

### Comparing `llama_index_packs_cohere_citation_chat-0.1.4/README.md` & `llama_index_packs_cohere_citation_chat-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_packs_cohere_citation_chat-0.1.4/llama_index/packs/cohere_citation_chat/base.py` & `llama_index_packs_cohere_citation_chat-0.1.5/llama_index/packs/cohere_citation_chat/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_packs_cohere_citation_chat-0.1.4/llama_index/packs/cohere_citation_chat/citations_context_chat_engine.py` & `llama_index_packs_cohere_citation_chat-0.1.5/llama_index/packs/cohere_citation_chat/citations_context_chat_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index_packs_cohere_citation_chat-0.1.4/llama_index/packs/cohere_citation_chat/types.py` & `llama_index_packs_cohere_citation_chat-0.1.5/llama_index/packs/cohere_citation_chat/types.py`

 * *Files identical despite different names*

### Comparing `llama_index_packs_cohere_citation_chat-0.1.4/llama_index/packs/cohere_citation_chat/utils.py` & `llama_index_packs_cohere_citation_chat-0.1.5/llama_index/packs/cohere_citation_chat/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_packs_cohere_citation_chat-0.1.4/pyproject.toml` & `llama_index_packs_cohere_citation_chat-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,20 +25,20 @@
 description = "llama-index packs cohere_citation_chat integration"
 exclude = ["**/BUILD"]
 keywords = ["chat", "citation", "cite", "cohere", "engine", "index"]
 license = "MIT"
 maintainers = ["EugeneLightsOn"]
 name = "llama-index-packs-cohere-citation-chat"
 readme = "README.md"
-version = "0.1.4"
+version = "0.1.5"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.35"
-llama-index-llms-cohere = "^0.1.2"
+llama-index-llms-cohere = ">=0.1.2"
 llama-index-embeddings-cohere = "^0.1.2"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
```

### Comparing `llama_index_packs_cohere_citation_chat-0.1.4/PKG-INFO` & `llama_index_packs_cohere_citation_chat-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: llama-index-packs-cohere-citation-chat
-Version: 0.1.4
+Version: 0.1.5
 Summary: llama-index packs cohere_citation_chat integration
 License: MIT
 Keywords: chat,citation,cite,cohere,engine,index
 Author: Your Name
 Author-email: you@example.com
 Maintainer: EugeneLightsOn
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: llama-index-core (>=0.10.35,<0.11.0)
 Requires-Dist: llama-index-embeddings-cohere (>=0.1.2,<0.2.0)
-Requires-Dist: llama-index-llms-cohere (>=0.1.2,<0.2.0)
+Requires-Dist: llama-index-llms-cohere (>=0.1.2)
 Description-Content-Type: text/markdown
 
 # Cohere Citations Chat Engine Pack
 
 Creates and runs a custom `VectorStoreIndexWithCitationsChat` -- which provides the chat engine with documents/citation mode.
 See the documentation [here](https://docs.cohere.com/docs/retrieval-augmented-generation-rag) and [here](https://docs.cohere.com/docs/retrieval-augmented-generation-rag).
```

