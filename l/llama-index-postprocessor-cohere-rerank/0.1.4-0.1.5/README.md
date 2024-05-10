# Comparing `tmp/llama_index_postprocessor_cohere_rerank-0.1.4.tar.gz` & `tmp/llama_index_postprocessor_cohere_rerank-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_postprocessor_cohere_rerank-0.1.4.tar", max compression
+gzip compressed data, was "llama_index_postprocessor_cohere_rerank-0.1.5.tar", max compression
```

## Comparing `llama_index_postprocessor_cohere_rerank-0.1.4.tar` & `llama_index_postprocessor_cohere_rerank-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       54 2024-03-29 16:11:38.737421 llama_index_postprocessor_cohere_rerank-0.1.4/README.md
--rw-r--r--   0        0        0       98 2024-03-29 16:11:38.737421 llama_index_postprocessor_cohere_rerank-0.1.4/llama_index/postprocessor/cohere_rerank/__init__.py
--rw-r--r--   0        0        0     2591 2024-03-29 16:11:38.737421 llama_index_postprocessor_cohere_rerank-0.1.4/llama_index/postprocessor/cohere_rerank/base.py
--rw-r--r--   0        0        0     1493 2024-03-29 16:11:38.737421 llama_index_postprocessor_cohere_rerank-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      672 1970-01-01 00:00:00.000000 llama_index_postprocessor_cohere_rerank-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       54 2024-05-10 01:33:57.806810 llama_index_postprocessor_cohere_rerank-0.1.5/README.md
+-rw-r--r--   0        0        0       98 2024-05-10 01:33:57.806810 llama_index_postprocessor_cohere_rerank-0.1.5/llama_index/postprocessor/cohere_rerank/__init__.py
+-rw-r--r--   0        0        0     3168 2024-05-10 01:33:57.806810 llama_index_postprocessor_cohere_rerank-0.1.5/llama_index/postprocessor/cohere_rerank/base.py
+-rw-r--r--   0        0        0     1493 2024-05-10 01:33:57.806810 llama_index_postprocessor_cohere_rerank-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      672 1970-01-01 00:00:00.000000 llama_index_postprocessor_cohere_rerank-0.1.5/PKG-INFO
```

### Comparing `llama_index_postprocessor_cohere_rerank-0.1.4/llama_index/postprocessor/cohere_rerank/base.py` & `llama_index_postprocessor_cohere_rerank-0.1.5/llama_index/postprocessor/cohere_rerank/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 import os
 from typing import Any, List, Optional
 
 from llama_index.core.bridge.pydantic import Field, PrivateAttr
 from llama_index.core.callbacks import CBEventType, EventPayload
+from llama_index.core.instrumentation import get_dispatcher
+from llama_index.core.instrumentation.events.rerank import (
+    ReRankEndEvent,
+    ReRankStartEvent,
+)
 from llama_index.core.postprocessor.types import BaseNodePostprocessor
-from llama_index.core.schema import NodeWithScore, QueryBundle
+from llama_index.core.schema import NodeWithScore, QueryBundle, MetadataMode
+
+dispatcher = get_dispatcher(__name__)
 
 
 class CohereRerank(BaseNodePostprocessor):
     model: str = Field(description="Cohere model name.")
     top_n: int = Field(description="Top N nodes to return.")
 
     _client: Any = PrivateAttr()
@@ -41,29 +48,39 @@
         return "CohereRerank"
 
     def _postprocess_nodes(
         self,
         nodes: List[NodeWithScore],
         query_bundle: Optional[QueryBundle] = None,
     ) -> List[NodeWithScore]:
+        dispatch_event = dispatcher.get_dispatch_event()
+        dispatch_event(
+            ReRankStartEvent(
+                query=query_bundle, nodes=nodes, top_n=self.top_n, model_name=self.model
+            )
+        )
+
         if query_bundle is None:
             raise ValueError("Missing query bundle in extra info.")
         if len(nodes) == 0:
             return []
 
         with self.callback_manager.event(
             CBEventType.RERANKING,
             payload={
                 EventPayload.NODES: nodes,
                 EventPayload.MODEL_NAME: self.model,
                 EventPayload.QUERY_STR: query_bundle.query_str,
                 EventPayload.TOP_K: self.top_n,
             },
         ) as event:
-            texts = [node.node.get_content() for node in nodes]
+            texts = [
+                node.node.get_content(metadata_mode=MetadataMode.EMBED)
+                for node in nodes
+            ]
             results = self._client.rerank(
                 model=self.model,
                 top_n=self.top_n,
                 query=query_bundle.query_str,
                 documents=texts,
             )
 
@@ -71,8 +88,9 @@
             for result in results.results:
                 new_node_with_score = NodeWithScore(
                     node=nodes[result.index].node, score=result.relevance_score
                 )
                 new_nodes.append(new_node_with_score)
             event.on_end(payload={EventPayload.NODES: new_nodes})
 
+        dispatch_event(ReRankEndEvent(nodes=new_nodes))
         return new_nodes
```

### Comparing `llama_index_postprocessor_cohere_rerank-0.1.4/pyproject.toml` & `llama_index_postprocessor_cohere_rerank-0.1.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index postprocessor cohere rerank integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-postprocessor-cohere-rerank"
 readme = "README.md"
-version = "0.1.4"
+version = "0.1.5"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 cohere = "^5.1.1"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_postprocessor_cohere_rerank-0.1.4/PKG-INFO` & `llama_index_postprocessor_cohere_rerank-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-postprocessor-cohere-rerank
-Version: 0.1.4
+Version: 0.1.5
 Summary: llama-index postprocessor cohere rerank integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

