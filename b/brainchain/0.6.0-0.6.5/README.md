# Comparing `tmp/brainchain-0.6.0.tar.gz` & `tmp/brainchain-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainchain-0.6.0.tar", max compression
+gzip compressed data, was "brainchain-0.6.5.tar", max compression
```

## Comparing `brainchain-0.6.0.tar` & `brainchain-0.6.5.tar`

### file list

```diff
@@ -1,29 +1,47 @@
--rw-r--r--   0        0        0     6148 2024-04-10 15:41:29.802452 brainchain-0.6.0/brainchain/.DS_Store
--rw-r--r--   0        0        0     1732 2023-06-20 22:57:22.671703 brainchain-0.6.0/brainchain/README.md
--rw-r--r--   0        0        0      671 2024-04-15 19:33:12.465156 brainchain-0.6.0/brainchain/__init__.py
--rw-r--r--   0        0        0    13624 2024-04-15 19:41:12.625248 brainchain-0.6.0/brainchain/assistants
--rw-r--r--   0        0        0    13624 2024-04-15 19:52:38.518975 brainchain-0.6.0/brainchain/assistants.py
--rw-r--r--   0        0        0    17664 2024-04-15 19:52:45.029786 brainchain-0.6.0/brainchain/brainchain.py
--rw-r--r--   0        0        0     5663 2024-03-27 22:17:28.214003 brainchain-0.6.0/brainchain/carnivore.py
--rw-r--r--   0        0        0     2243 2024-02-14 04:10:52.129450 brainchain-0.6.0/brainchain/coredata.py
--rw-r--r--   0        0        0     2155 2023-09-12 01:13:30.915323 brainchain-0.6.0/brainchain/embeddings.py
--rw-r--r--   0        0        0     3426 2024-04-15 19:43:17.579942 brainchain-0.6.0/brainchain/logger.py
--rw-r--r--   0        0        0    11498 2024-03-19 23:11:27.374089 brainchain-0.6.0/brainchain/products.py
--rw-r--r--   0        0        0    15070 2023-07-05 18:42:36.359889 brainchain-0.6.0/brainchain/requirements.txt
--rw-r--r--   0        0        0     6024 2024-02-29 23:10:12.854589 brainchain-0.6.0/brainchain/sales_intel.py
--rw-r--r--   0        0        0     1977 2024-02-29 23:10:12.854747 brainchain-0.6.0/brainchain/search_v2.py
--rw-r--r--   0        0        0     6148 2024-03-18 17:43:54.835290 brainchain-0.6.0/brainchain/tools/.DS_Store
--rw-r--r--   0        0        0      595 2024-04-12 19:05:17.907126 brainchain-0.6.0/brainchain/tools/__init__.py
--rw-r--r--   0        0        0     2118 2024-03-18 17:46:16.438013 brainchain-0.6.0/brainchain/tools/coding.py
--rw-r--r--   0        0        0     3948 2024-04-15 19:12:36.615790 brainchain-0.6.0/brainchain/tools/diffbot.py
--rw-r--r--   0        0        0      632 2024-02-29 23:10:12.855578 brainchain-0.6.0/brainchain/tools/factual.py
--rw-r--r--   0        0        0     5800 2024-04-10 01:04:48.531327 brainchain-0.6.0/brainchain/tools/fts.py
--rw-r--r--   0        0        0     1450 2024-02-29 23:10:12.856798 brainchain-0.6.0/brainchain/tools/graph.py
--rw-r--r--   0        0        0     1029 2024-02-29 23:10:12.857047 brainchain-0.6.0/brainchain/tools/memory.py
--rw-r--r--   0        0        0     2154 2024-02-29 23:10:12.857190 brainchain-0.6.0/brainchain/tools/plan.py
--rw-r--r--   0        0        0     1660 2024-04-15 19:40:33.833814 brainchain-0.6.0/brainchain/tools/tokens.py
--rw-r--r--   0        0        0    20787 2024-04-15 19:32:38.611665 brainchain-0.6.0/brainchain/tools/tools.py
--rw-r--r--   0        0        0    10427 2024-04-10 00:54:22.728479 brainchain-0.6.0/brainchain/tools/web.py
--rw-r--r--   0        0        0      731 2024-04-15 19:33:06.073495 brainchain-0.6.0/brainchain/tools.py
--rw-r--r--   0        0        0      538 2024-04-15 19:45:20.212527 brainchain-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      556 1970-01-01 00:00:00.000000 brainchain-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1732 2023-06-20 22:57:22.671703 brainchain-0.6.5/brainchain/README.md
+-rw-r--r--   0        0        0     2982 2024-05-10 17:23:42.151722 brainchain-0.6.5/brainchain/__init__.py
+-rw-r--r--   0        0        0    13634 2024-05-07 16:51:46.069513 brainchain-0.6.5/brainchain/assistants
+-rw-r--r--   0        0        0    13624 2024-05-07 16:51:46.070229 brainchain-0.6.5/brainchain/assistants.py
+-rw-r--r--   0        0        0    11851 2024-05-09 17:42:15.555016 brainchain-0.6.5/brainchain/brainchain.py
+-rw-r--r--   0        0        0     5663 2024-05-09 05:35:25.596909 brainchain-0.6.5/brainchain/carnivore.py
+-rw-r--r--   0        0        0     2243 2024-02-14 04:10:52.129450 brainchain-0.6.5/brainchain/coredata.py
+-rw-r--r--   0        0        0     2155 2023-09-12 01:13:30.915323 brainchain-0.6.5/brainchain/embeddings.py
+-rw-r--r--   0        0        0    17779 2024-05-10 17:26:05.409771 brainchain-0.6.5/brainchain/graph/base.py
+-rw-r--r--   0        0        0     7386 2024-05-10 17:23:37.046295 brainchain-0.6.5/brainchain/graph/schema.py
+-rw-r--r--   0        0        0     3426 2024-05-07 16:51:46.072116 brainchain-0.6.5/brainchain/logger.py
+-rw-r--r--   0        0        0    11959 2024-05-07 16:51:46.072448 brainchain-0.6.5/brainchain/products.py
+-rw-r--r--   0        0        0    15070 2023-07-05 18:42:36.359889 brainchain-0.6.5/brainchain/requirements.txt
+-rw-r--r--   0        0        0     6024 2024-05-07 16:20:56.058058 brainchain-0.6.5/brainchain/sales_intel.py
+-rw-r--r--   0        0        0     1977 2024-02-29 23:10:12.854747 brainchain-0.6.5/brainchain/search_v2.py
+-rw-r--r--   0        0        0      595 2024-04-12 19:05:17.907126 brainchain-0.6.5/brainchain/tools/__init__.py
+-rw-r--r--   0        0        0     2118 2024-05-09 17:28:37.403805 brainchain-0.6.5/brainchain/tools/coding.py
+-rw-r--r--   0        0        0     3948 2024-05-07 16:51:46.073351 brainchain-0.6.5/brainchain/tools/diffbot.py
+-rw-r--r--   0        0        0      632 2024-02-29 23:10:12.855578 brainchain-0.6.5/brainchain/tools/factual.py
+-rw-r--r--   0        0        0     5800 2024-04-10 01:04:48.531327 brainchain-0.6.5/brainchain/tools/fts.py
+-rw-r--r--   0        0        0     1450 2024-02-29 23:10:12.856798 brainchain-0.6.5/brainchain/tools/graph.py
+-rw-r--r--   0        0        0     1029 2024-02-29 23:10:12.857047 brainchain-0.6.5/brainchain/tools/memory.py
+-rw-r--r--   0        0        0     2154 2024-02-29 23:10:12.857190 brainchain-0.6.5/brainchain/tools/plan.py
+-rw-r--r--   0        0        0     1660 2024-04-15 19:40:33.833814 brainchain-0.6.5/brainchain/tools/tokens.py
+-rw-r--r--   0        0        0    21273 2024-05-07 16:51:46.073960 brainchain-0.6.5/brainchain/tools/tools.py
+-rw-r--r--   0        0        0    12159 2024-05-07 16:51:46.074887 brainchain-0.6.5/brainchain/tools/web.py
+-rw-r--r--   0        0        0      731 2024-04-23 19:21:58.552351 brainchain-0.6.5/brainchain/tools.py
+-rw-r--r--   0        0        0      791 2024-05-07 16:51:51.752365 brainchain-0.6.5/brainchain/webapp/__init__.py
+-rw-r--r--   0        0        0       82 2024-05-07 16:51:51.752653 brainchain-0.6.5/brainchain/webapp/agents.py
+-rw-r--r--   0        0        0      173 2024-05-07 16:51:51.752960 brainchain-0.6.5/brainchain/webapp/base.py
+-rw-r--r--   0        0        0      977 2024-05-07 16:51:51.753234 brainchain-0.6.5/brainchain/webapp/business_ideas.py
+-rw-r--r--   0        0        0     1282 2024-05-07 16:51:51.753423 brainchain-0.6.5/brainchain/webapp/contents.py
+-rw-r--r--   0        0        0      895 2024-05-07 16:51:51.753590 brainchain-0.6.5/brainchain/webapp/conversations.py
+-rw-r--r--   0        0        0       91 2024-05-07 16:51:51.753815 brainchain-0.6.5/brainchain/webapp/embedding_models.py
+-rw-r--r--   0        0        0     2709 2024-05-07 16:51:51.753990 brainchain-0.6.5/brainchain/webapp/embeddings.py
+-rw-r--r--   0        0        0     1138 2024-05-07 16:51:51.754142 brainchain-0.6.5/brainchain/webapp/files.py
+-rw-r--r--   0        0        0      218 2024-05-07 16:51:51.754320 brainchain-0.6.5/brainchain/webapp/health.py
+-rw-r--r--   0        0        0       90 2024-05-07 16:51:51.754539 brainchain-0.6.5/brainchain/webapp/language_models.py
+-rw-r--r--   0        0        0      622 2024-05-07 16:51:51.754700 brainchain-0.6.5/brainchain/webapp/laws.py
+-rw-r--r--   0        0        0     1110 2024-05-07 16:51:51.754849 brainchain-0.6.5/brainchain/webapp/messages.py
+-rw-r--r--   0        0        0     2220 2024-05-07 16:51:51.755068 brainchain-0.6.5/brainchain/webapp/namespaces.py
+-rw-r--r--   0        0        0     1029 2024-05-07 16:51:51.755220 brainchain-0.6.5/brainchain/webapp/programs.py
+-rw-r--r--   0        0        0      626 2024-05-07 16:51:51.755369 brainchain-0.6.5/brainchain/webapp/tasks.py
+-rw-r--r--   0        0        0      853 2024-05-07 16:51:51.755565 brainchain-0.6.5/brainchain/webapp/tools.py
+-rw-r--r--   0        0        0      677 2024-05-07 16:51:51.755730 brainchain-0.6.5/brainchain/webapp/users.py
+-rw-r--r--   0        0        0      538 2024-05-10 17:26:18.966160 brainchain-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0      556 1970-01-01 00:00:00.000000 brainchain-0.6.5/PKG-INFO
```

### Comparing `brainchain-0.6.0/brainchain/README.md` & `brainchain-0.6.5/brainchain/README.md`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.0/brainchain/__init__.py` & `brainchain-0.6.5/brainchain/tools.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from .brainchain import Brainchain
-from .products import ProductsAPI
-from .tools.web import web_search, web_content, web_cache, web_scanner
-from .tools.coding import python_agent, sql_database_agent, terminal
-from .tools.memory import insert_memory, lookup_similar_memories, delete_memories
-from .tools.tokens import encode_text, decode_tokens
-from .tools.fts import fts_ingest_document, fts_search_index, fts_document_qa, fts_extract, fts_indices, fts_health_check
-from .tools.graph import execute_cypher_query, graph_query
-from .tools.factual import fact_check
-from .tools.diffbot import diffbot_analyze
-from .tools.plan import generate_plan, improve_plan, execute_plan
+from brainchain.tools.web import web_search, web_content, web_cache, web_scanner
+from brainchain.tools.coding import python_agent, sql_database_agent, terminal
+from brainchain.tools.memory import insert_memory, lookup_similar_memories, delete_memories
+from brainchain.tools.tokens import encode_text, decode_tokens
+from brainchain.tools.fts import fts_ingest_document, fts_search_index, fts_document_qa, fts_extract, fts_indices, fts_health_check
+from brainchain.tools.graph import execute_cypher_query, graph_query
+from brainchain.tools.factual import fact_check
+from brainchain.tools.diffbot import diffbot_analyze
+from brainchain.tools.plan import generate_plan, improve_plan, execute_plan
+from brainchain.tools import functions
```

### Comparing `brainchain-0.6.0/brainchain/assistants` & `brainchain-0.6.5/brainchain/assistants`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import requests
 import json
 from logger import log_function_info
 from tools import *
+import os
 import time
 import math
 
 class AssistantClient:
     def __init__(self, assistants_api_host: str = "https://assistants-api.brainchain.cloud", api_host: str = "https://api.brainchain.cloud"):
         self.API_HOST = api_host or os.getenv("ASSISTANTS_API_HOST") 
         self.ASSISTANTS_API_HOST = assistants_api_host or os.getenv("API_HOST")
```

### Comparing `brainchain-0.6.0/brainchain/assistants.py` & `brainchain-0.6.5/brainchain/assistants.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.0/brainchain/carnivore.py` & `brainchain-0.6.5/brainchain/carnivore.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.0/brainchain/coredata.py` & `brainchain-0.6.5/brainchain/coredata.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.0/brainchain/embeddings.py` & `brainchain-0.6.5/brainchain/embeddings.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.0/brainchain/logger.py` & `brainchain-0.6.5/brainchain/logger.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.0/brainchain/products.py` & `brainchain-0.6.5/brainchain/products.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,23 +45,19 @@
     unix_timestamp_seconds = int(date_obj.timestamp())
     # Correct the conversion process: apply the Keepa-specific adjustments
     keepa_timestamp = (unix_timestamp_seconds // 60) - 21564000
     return keepa_timestamp
 
 import time
 class ProductsAPI():
-    def __init__(self, base_url: str = "http://localhost:8000"):
+    def __init__(self, base_url: str = "https://api.brainchain.cloud"):
         self.base_url = base_url
         self.wd = WebDataClient()
         self.session = requests.Session()
     
-    base_url: str = "http://localhost:8000"
-    wd: WebDataClient = WebDataClient()
-    session: requests.Session = requests.Session()
-
     @staticmethod
     def _convert_camel_to_snake(name):
         """
         Convert a camelCase name into snake_case.
         Ex: 'camelCase' -> 'camel_case'
         """
         s1 = re.sub('(.)([A-Z][a-z]+)', r'\1_\2', name)
@@ -77,15 +73,15 @@
         Returns:
             str: The normalized search query.
         """
         # Add normalization logic here
         return query
     
 
-    def search_keepa_and_save(self, asins: List[str] = [], max_products: int = 5, title: str = "", offers: int = 20, trackingSince_lte: dt = dt.now(), trackingSince_gte: dt = dt.now() - td(days=30)) -> List[Dict]:
+    def search_keepa_and_save(self, asins: List[str] = [], max_products: int = 5, title: str = "", offers: int = 20, trackingSince_lte: dt = dt.now(), trackingSince_gte: dt = dt.now() - td(days=30), excludeCategories: List[int] = []) -> List[Dict]:
         """
         Searches products on Keepa via WebDataClient and saves them to the database.
         
         Args:
             search_query (str): The search query for finding products.
         
         Returns:
@@ -164,14 +160,28 @@
                         price_response = self.create_product_instance_price(price_data)
                         print(price_response)
                     else:
                         print("Skipping price data because it's not the right length")
                         print(price)
                         
         return asin_product_map
+    
+    def get_product_instance_prices(self, product_instance_uuid):
+        """
+        Retrieve prices for a product instance.
+        
+        Args:
+            product_instance_uuid (str): The unique identifier for the product instance.
+            
+        Returns:
+            dict: The response data containing the product instance prices.
+        """
+        url = f"{self.base_url}/v1/products/product_instance/prices?product_instance_uuid={quote(product_instance_uuid)}"
+        response = self.session.get(url)
+        return response.json()
 
 
 
     def create_product(self, name: str):
         """
         Create a new product.
```

### Comparing `brainchain-0.6.0/brainchain/requirements.txt` & `brainchain-0.6.5/brainchain/requirements.txt`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.0/brainchain/sales_intel.py` & `brainchain-0.6.5/brainchain/sales_intel.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.0/brainchain/search_v2.py` & `brainchain-0.6.5/brainchain/search_v2.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.0/brainchain/tools/__init__.py` & `brainchain-0.6.5/brainchain/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.0/brainchain/tools/coding.py` & `brainchain-0.6.5/brainchain/tools/coding.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.0/brainchain/tools/diffbot.py` & `brainchain-0.6.5/brainchain/tools/diffbot.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.0/brainchain/tools/factual.py` & `brainchain-0.6.5/brainchain/tools/factual.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.0/brainchain/tools/fts.py` & `brainchain-0.6.5/brainchain/tools/fts.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.0/brainchain/tools/graph.py` & `brainchain-0.6.5/brainchain/tools/graph.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.0/brainchain/tools/memory.py` & `brainchain-0.6.5/brainchain/tools/memory.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.0/brainchain/tools/plan.py` & `brainchain-0.6.5/brainchain/tools/plan.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.0/brainchain/tools/tokens.py` & `brainchain-0.6.5/brainchain/tools/tokens.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.0/brainchain/tools/tools.py` & `brainchain-0.6.5/brainchain/tools/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-def tool_schemas():
+def tool_schemas(openai: bool = True, anthropic: bool = False):
     functions_ = [ {
             "type": "function",
             "name": "diffbot_analyze",
             "description": "Performs analysis on a specified URL using the Diffbot Analyze API, returning structured data. This function can be tailored to use specific modes, handle fallbacks, and extract particular fields.",
             "parameters": {
                 "type": "object",
                 "properties": {
@@ -466,8 +466,23 @@
       },
       "returns": {
         "type": "object",
         "description": "The JSON response with similar memories found."
       }
     }
     ]
-    return functions_
+
+    if anthropic:
+        new_out = []
+        for item in functions_:
+            new_item = {}
+            for k in item:
+                if k == "parameters":
+                    new_item["input_schema"] = item[k]
+                elif k == "type" or k == "returns":
+                    pass
+                else:
+                    new_item[k] = item[k]
+            new_out.append(new_item)
+        return new_out
+    if openai:    
+        return functions_
```

### Comparing `brainchain-0.6.0/brainchain/tools/web.py` & `brainchain-0.6.5/brainchain/tools/web.py`

 * *Files 15% similar despite different names*

```diff
@@ -86,31 +86,60 @@
         }
     else:
         return {
             "url": url,
             "google_cache_url": google_cache_url
         }
 
-def web_content(url, ephemeral=True, use_google_web_cache=False, tags=None, exclude_tags=None):
+import requests
+
+def web_content(url, ephemeral=True, use_google_web_cache=False, use_browser=True, raw_html=False,
+                use_web_archive_api=False, use_jina_reader=False, use_assistants=False,
+                tags=None, exclude_tags=None):
+    """
+    Scrape content from the given URL using various options for content rendering and filtering.
+    
+    Parameters:
+        url (str): The URL to scrape.
+        ephemeral (bool): If true, the data will not be stored persistently.
+        use_google_web_cache (bool): Use Google's cache to fetch older versions of the site if available.
+        use_browser (bool): Use a full browser environment for scraping, enabling JavaScript rendering.
+        raw_html (bool): Return raw HTML without any processing.
+        use_web_archive_api (bool): Use the Web Archive API to fetch archived versions of the site if available.
+        use_jina_reader (bool): Use Jina AI's reader for enhanced processing of the content.
+        use_assistants (bool): Use AI assistants for additional processing of the content.
+        tags (list[str]): Specific tags to include in the scraped content. Defaults to all tags if not specified.
+        exclude_tags (list[str]): Tags to exclude from the scraped content. Defaults to ["html", "script", "style"].
+
+    Returns:
+        dict: The JSON response from the API with the scraped data.
+    """
     base_url = "https://brainchain--carnivore.modal.run"
 
-    """Scrape content from the given URL."""
+    # Default values for tags and exclude_tags
     if tags is None:
         tags = ["*"]
     if exclude_tags is None:
         exclude_tags = ["html", "script", "style"]
-        
+
+    # Organize the data to be sent in the POST request
     data = {
         "url": url,
         "ephemeral": ephemeral,
         "use_google_web_cache": use_google_web_cache,
+        "use_browser": use_browser,
+        "raw_html": raw_html,
+        "use_web_archive_api": use_web_archive_api,
+        "use_jina_reader": use_jina_reader,
+        "use_assistants": use_assistants,
         "tags": tags,
         "exclude_tags": exclude_tags
     }
 
+    # Make the POST request and return the response
     response = requests.post(f"{base_url}/carnivore", json=data)
     return response.json()
 
 
 import requests
 from typing import List, Optional
 from pydantic import BaseModel, Field, validator
@@ -184,14 +213,15 @@
 
 class ProductFinderParameters(BaseModel):
     title: Optional[str] = None
     brand: Optional[str] = None
     manufacturer: Optional[str] = None
     trackingSince_lte: Optional[str] = None
     trackingSince_gte: Optional[str] = None
+    excludeCategories: Optional[List[int]] = []
 
 
 class BestSellersQueryParams(BaseModel):
     category: str
     domain: Optional[str] = "US"
     wait: Optional[bool] = True
 
@@ -216,21 +246,22 @@
 
     def find_and_query(
         self,
         title: Optional[str],
         asins: Optional[List[str]] = [],
         trackingSince_gte: Optional[dt] = dt.now() - td(days=30),
         trackingSince_lte: Optional[dt] = dt.now(),
+        excludeCategories: Optional[List[int]] = [],
         offers: int = 20,
         max_products: int = 5,
         history: bool = True,
     ) -> dict:
         if title:
             params = ProductFinderParameters(
-                title=title, trackingSince_gte=trackingSince_gte.strftime("%Y-%m-%d"), trackingSince_lte=trackingSince_lte.strftime("%Y-%m-%d")
+                title=title, trackingSince_gte=trackingSince_gte.strftime("%Y-%m-%d"), trackingSince_lte=trackingSince_lte.strftime("%Y-%m-%d"), excludeCategories=excludeCategories
             )
             asins = self.product_finder(params)
             print(asins)
             query = ProductQueryPayload(items=asins, options=QueryOptions(offers=offers, history=history))
             print(query)
             x = self.query_product(query)
             print(x)
```

### Comparing `brainchain-0.6.0/pyproject.toml` & `brainchain-0.6.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "brainchain"
-version = "0.6.0"
+version = "0.6.5"
 description = "Brainchain API client"
 authors = ["Arthur M. Collé <arthur@brainchain.ai>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 urllib3 = "2.0.6"
 requests = "2.31.0"
```

### Comparing `brainchain-0.6.0/PKG-INFO` & `brainchain-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainchain
-Version: 0.6.0
+Version: 0.6.5
 Summary: Brainchain API client
 Author: Arthur M. Collé
 Author-email: arthur@brainchain.ai
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

