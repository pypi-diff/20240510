# Comparing `tmp/bigdata_client-0.2.0.tar.gz` & `tmp/bigdata_client-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigdata_client-0.2.0.tar", max compression
+gzip compressed data, was "bigdata_client-0.3.0.tar", max compression
```

## Comparing `bigdata_client-0.2.0.tar` & `bigdata_client-0.3.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0      358 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/README.md
--rw-r--r--   0        0        0      155 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/__init__.py
--rw-r--r--   0        0        0     6556 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/advanced_search_query.py
--rw-r--r--   0        0        0        0 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/api/__init__.py
--rw-r--r--   0        0        0      888 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/api/knowledge_graph.py
--rw-r--r--   0        0        0     8329 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/api/search.py
--rw-r--r--   0        0        0     2985 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/api/uploads.py
--rw-r--r--   0        0        0      975 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/api/watchlist.py
--rw-r--r--   0        0        0     6464 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/auth.py
--rw-r--r--   0        0        0        0 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/clerk/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/clerk/authenticators/__init__.py
--rw-r--r--   0        0        0     2256 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/clerk/authenticators/base_instance.py
--rw-r--r--   0        0        0     4166 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/clerk/authenticators/dev_instance.py
--rw-r--r--   0        0        0     3650 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/clerk/authenticators/production_instance.py
--rw-r--r--   0        0        0      853 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/clerk/exceptions.py
--rw-r--r--   0        0        0      245 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/clerk/models.py
--rw-r--r--   0        0        0        0 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/clerk/sign_in_strategies/__init__.py
--rw-r--r--   0        0        0      243 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/clerk/sign_in_strategies/base.py
--rw-r--r--   0        0        0     1008 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/clerk/sign_in_strategies/password.py
--rw-r--r--   0        0        0     2510 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/clerk/token_manager.py
--rw-r--r--   0        0        0     2040 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/clerk/token_manager_factory.py
--rw-r--r--   0        0        0    13702 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/connection.py
--rw-r--r--   0        0        0      475 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/connection_protocol.py
--rw-r--r--   0        0        0      154 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/constants.py
--rw-r--r--   0        0        0     4501 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/daterange.py
--rw-r--r--   0        0        0     1234 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/entity_types.py
--rw-r--r--   0        0        0      664 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/enum_utils.py
--rw-r--r--   0        0        0       82 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/errors.py
--rw-r--r--   0        0        0      196 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/file_status.py
--rw-r--r--   0        0        0      513 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/jwt.py
--rw-r--r--   0        0        0        0 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/models/__init__.py
--rw-r--r--   0        0        0    21160 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/models/advanced_search_query.py
--rw-r--r--   0        0        0     1181 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/models/comentions.py
--rw-r--r--   0        0        0     5961 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/models/entities.py
--rw-r--r--   0        0        0     1094 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/models/languages.py
--rw-r--r--   0        0        0     3841 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/models/parse.py
--rw-r--r--   0        0        0     1710 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/models/search.py
--rw-r--r--   0        0        0     2280 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/models/sources.py
--rw-r--r--   0        0        0      876 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/models/story.py
--rw-r--r--   0        0        0     2180 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/models/topics.py
--rw-r--r--   0        0        0     6580 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/models/uploads.py
--rw-r--r--   0        0        0     2820 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/models/watchlists.py
--rw-r--r--   0        0        0     4773 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/old_auth.py
--rw-r--r--   0        0        0      177 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/pdf_utils.py
--rw-r--r--   0        0        0      970 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/query.py
--rw-r--r--   0        0        0      251 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/query_type.py
--rw-r--r--   0        0        0     6746 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/search.py
--rw-r--r--   0        0        0    14376 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/services.py
--rw-r--r--   0        0        0     1086 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/settings.py
--rw-r--r--   0        0        0     2091 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/story.py
--rw-r--r--   0        0        0      465 2024-05-03 16:46:20.949843 bigdata_client-0.2.0/bigdata/user_agent.py
--rw-r--r--   0        0        0     1359 2024-05-03 16:46:20.953843 bigdata_client-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1058 1970-01-01 00:00:00.000000 bigdata_client-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      358 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/README.md
+-rw-r--r--   0        0        0      155 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/__init__.py
+-rw-r--r--   0        0        0     6556 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/advanced_search_query.py
+-rw-r--r--   0        0        0        0 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/api/__init__.py
+-rw-r--r--   0        0        0      888 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/api/knowledge_graph.py
+-rw-r--r--   0        0        0     8970 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/api/search.py
+-rw-r--r--   0        0        0     2985 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/api/uploads.py
+-rw-r--r--   0        0        0      975 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/api/watchlist.py
+-rw-r--r--   0        0        0     6464 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/auth.py
+-rw-r--r--   0        0        0        0 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/clerk/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/clerk/authenticators/__init__.py
+-rw-r--r--   0        0        0     2256 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/clerk/authenticators/base_instance.py
+-rw-r--r--   0        0        0     4166 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/clerk/authenticators/dev_instance.py
+-rw-r--r--   0        0        0     3650 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/clerk/authenticators/production_instance.py
+-rw-r--r--   0        0        0      853 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/clerk/exceptions.py
+-rw-r--r--   0        0        0      245 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/clerk/models.py
+-rw-r--r--   0        0        0        0 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/clerk/sign_in_strategies/__init__.py
+-rw-r--r--   0        0        0      243 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/clerk/sign_in_strategies/base.py
+-rw-r--r--   0        0        0     1008 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/clerk/sign_in_strategies/password.py
+-rw-r--r--   0        0        0     2510 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/clerk/token_manager.py
+-rw-r--r--   0        0        0     2040 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/clerk/token_manager_factory.py
+-rw-r--r--   0        0        0    14138 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/connection.py
+-rw-r--r--   0        0        0      475 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/connection_protocol.py
+-rw-r--r--   0        0        0      154 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/constants.py
+-rw-r--r--   0        0        0     4501 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/daterange.py
+-rw-r--r--   0        0        0     1234 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/entity_types.py
+-rw-r--r--   0        0        0      664 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/enum_utils.py
+-rw-r--r--   0        0        0       82 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/errors.py
+-rw-r--r--   0        0        0      196 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/file_status.py
+-rw-r--r--   0        0        0      513 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/jwt.py
+-rw-r--r--   0        0        0        0 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/models/__init__.py
+-rw-r--r--   0        0        0    33261 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/models/advanced_search_query.py
+-rw-r--r--   0        0        0     1181 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/models/comentions.py
+-rw-r--r--   0        0        0     5961 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/models/entities.py
+-rw-r--r--   0        0        0     1094 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/models/languages.py
+-rw-r--r--   0        0        0     3841 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/models/parse.py
+-rw-r--r--   0        0        0     3513 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/models/search.py
+-rw-r--r--   0        0        0     2280 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/models/sources.py
+-rw-r--r--   0        0        0      897 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/models/story.py
+-rw-r--r--   0        0        0     2180 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/models/topics.py
+-rw-r--r--   0        0        0     6902 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/models/uploads.py
+-rw-r--r--   0        0        0     2820 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/models/watchlists.py
+-rw-r--r--   0        0        0     4773 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/old_auth.py
+-rw-r--r--   0        0        0      177 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/pdf_utils.py
+-rw-r--r--   0        0        0     1296 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/query.py
+-rw-r--r--   0        0        0      251 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/query_type.py
+-rw-r--r--   0        0        0     9523 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/search.py
+-rw-r--r--   0        0        0    14376 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/services.py
+-rw-r--r--   0        0        0     1086 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/settings.py
+-rw-r--r--   0        0        0     2146 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/story.py
+-rw-r--r--   0        0        0      465 2024-05-10 15:57:33.962221 bigdata_client-0.3.0/bigdata/user_agent.py
+-rw-r--r--   0        0        0     1359 2024-05-10 15:57:33.966220 bigdata_client-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1058 1970-01-01 00:00:00.000000 bigdata_client-0.3.0/PKG-INFO
```

### Comparing `bigdata_client-0.2.0/bigdata/advanced_search_query.py` & `bigdata_client-0.3.0/bigdata/advanced_search_query.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.2.0/bigdata/api/knowledge_graph.py` & `bigdata_client-0.3.0/bigdata/api/knowledge_graph.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.2.0/bigdata/api/search.py` & `bigdata_client-0.3.0/bigdata/api/search.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from bigdata.models.languages import Language
 from bigdata.models.search import (
     Expression,
     FileType,
     Ranking,
     SearchChain,
     SearchPagination,
+    SearchSharePermission,
     SortBy,
 )
 from bigdata.models.sources import Source
 from bigdata.models.story import StoryType
 from bigdata.models.topics import Topic
 from bigdata.query_type import QueryType
 from bigdata.settings import settings
@@ -63,14 +64,34 @@
 class UpdateSearchRequest(BaseModel):
     """Model to represent the request to update a search"""
 
     name: Optional[str]
     query: SaveSearchQueryRequest
 
 
+# Share a saved search
+
+
+class UserQueryShareCompanyContext(BaseModel):
+    permission: SearchSharePermission
+
+
+class UserQueryShareUserContext(BaseModel):
+    id: str
+    permission: SearchSharePermission
+
+
+class UserQueryShareContext(BaseModel):
+    company: UserQueryShareCompanyContext
+    users: list[UserQueryShareUserContext]
+
+
+class ShareSavedSearchRequest(UserQueryShareContext): ...
+
+
 # Get saved searches
 
 
 class SavedSearchQueryResponse(BaseModel):
     """
     Model to represent the "query" attribute of a response from getting a saved
     search.
@@ -88,14 +109,15 @@
 class SavedSearchResponse(BaseModel):
     """Model to represent the response from getting a saved search"""
 
     id: str
     name: str
     query: SavedSearchQueryResponse
     save_status: Literal["saved"] = Field(default="saved", alias="saveStatus")
+    shared: UserQueryShareContext
     # TODO: Add dateCreated, lastExecuted, lastUpdated, owner, ownerName, permissions
 
 
 # Delete a saved search
 
 
 class DeleteSavedSearchResponse(BaseModel):
@@ -214,14 +236,15 @@
     source_rank: int
     language: str
 
     class ChunkedStoryResponseSentence(BaseModel):
         text: str
         cnum: int
         relevance: float
+        sentiment: float
 
         class StoryResponseEntity(BaseModel):
             key: str
             start: int
             end: int
             queryType: QueryType
 
@@ -271,15 +294,15 @@
     search_chain: Optional[SearchChain] = Field(alias="searchChain", default=None)
     hybrid: bool = settings.LLM.USE_HYBRID
 
 
 class DiscoveryPanelResponse(BaseModel):
     """Model to represent the response from getting comentions"""
 
-    companies: list[Company]
-    concepts: list[Concept]
-    languages: list[Language]
-    organizations: list[Union[Organization, OrganizationType]]
-    places: list[Union[Place, Facility, Landmark]]
-    products: list[Union[Product, ProductType]]
-    sources: list[Source]
-    topics: list[Topic]
+    companies: list[Company] = Field(default=[])
+    concepts: list[Concept] = Field(default=[])
+    languages: list[Language] = Field(default=[])
+    organizations: list[Union[Organization, OrganizationType]] = Field(default=[])
+    places: list[Union[Place, Facility, Landmark]] = Field(default=[])
+    products: list[Union[Product, ProductType]] = Field(default=[])
+    sources: list[Source] = Field(default=[])
+    topics: list[Topic] = Field(default=[])
```

### Comparing `bigdata_client-0.2.0/bigdata/api/uploads.py` & `bigdata_client-0.3.0/bigdata/api/uploads.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.2.0/bigdata/api/watchlist.py` & `bigdata_client-0.3.0/bigdata/api/watchlist.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.2.0/bigdata/auth.py` & `bigdata_client-0.3.0/bigdata/auth.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.2.0/bigdata/clerk/authenticators/base_instance.py` & `bigdata_client-0.3.0/bigdata/clerk/authenticators/base_instance.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.2.0/bigdata/clerk/authenticators/dev_instance.py` & `bigdata_client-0.3.0/bigdata/clerk/authenticators/dev_instance.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.2.0/bigdata/clerk/authenticators/production_instance.py` & `bigdata_client-0.3.0/bigdata/clerk/authenticators/production_instance.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.2.0/bigdata/clerk/exceptions.py` & `bigdata_client-0.3.0/bigdata/clerk/exceptions.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.2.0/bigdata/clerk/sign_in_strategies/password.py` & `bigdata_client-0.3.0/bigdata/clerk/sign_in_strategies/password.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.2.0/bigdata/clerk/token_manager.py` & `bigdata_client-0.3.0/bigdata/clerk/token_manager.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.2.0/bigdata/clerk/token_manager_factory.py` & `bigdata_client-0.3.0/bigdata/clerk/token_manager_factory.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.2.0/bigdata/connection.py` & `bigdata_client-0.3.0/bigdata/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     DiscoveryPanelRequest,
     DiscoveryPanelResponse,
     ListSavedSearchesResponse,
     QueryChunksRequest,
     QueryChunksResponse,
     SavedSearchResponse,
     SaveSearchRequest,
+    ShareSavedSearchRequest,
     UpdateSearchRequest,
 )
 from bigdata.api.uploads import (
     DeleteFileResponse,
     GetDownloadPresignedUrlResponse,
     GetFileResponse,
     GetFileStatusResponse,
@@ -178,14 +179,24 @@
         return SavedSearchResponse(**response)
 
     def delete_search(self, id: str) -> DeleteSavedSearchResponse:
         """Calls DELETE /user-data/queries/{id}"""
         response = self.http.delete(f"user-data/queries/{id}")
         return DeleteSavedSearchResponse(**response)
 
+    def share_search(
+        self, id_: str, request: ShareSavedSearchRequest
+    ) -> SavedSearchResponse:
+        """Calls POST /user-data/queries/{id}/share"""
+        json_request = request.model_dump(exclude_none=True, by_alias=True)
+        json_response = self.http.post(
+            f"user-data/queries/{id_}/share", json=json_request
+        )
+        return SavedSearchResponse(**json_response)
+
     def query_discovery_panel(
         self, request: DiscoveryPanelRequest
     ) -> DiscoveryPanelResponse:
         """Calls POST /cqs/discovery-panel"""
         json_request = request.model_dump(exclude_none=True, by_alias=True)
         json_response = self.http.post("cqs/discovery-panel", json=json_request)
         return DiscoveryPanelResponse(**json_response)
```

### Comparing `bigdata_client-0.2.0/bigdata/daterange.py` & `bigdata_client-0.3.0/bigdata/daterange.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.2.0/bigdata/entity_types.py` & `bigdata_client-0.3.0/bigdata/entity_types.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.2.0/bigdata/enum_utils.py` & `bigdata_client-0.3.0/bigdata/enum_utils.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.2.0/bigdata/jwt.py` & `bigdata_client-0.3.0/bigdata/jwt.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.2.0/bigdata/models/advanced_search_query.py` & `bigdata_client-0.3.0/bigdata/models/advanced_search_query.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 from abc import ABC, ABCMeta, abstractmethod
-from typing import Protocol, Union, runtime_checkable
+from typing import Optional, Protocol, Union, runtime_checkable
 
-from bigdata.models.search import Expression, ExpressionOperation, ExpressionTypes
+from bigdata.models.search import (
+    DocumentTypes,
+    Expression,
+    ExpressionOperation,
+    ExpressionTypes,
+    FiscalQuarterValidator,
+    FiscalYearValidator,
+    SectionTypes,
+)
 
 
 # Decorated with runtime_checkable to allow isinstance checks
 @runtime_checkable
 class QueryComponent(Protocol):
     """
     Protocol for any query component.
@@ -457,14 +465,320 @@
 
 
 class Source(ListQueryComponent):
     def get_expression_type(self) -> ExpressionTypes:
         return ExpressionTypes.SOURCE
 
 
+class SectionMetadata(BaseQueryComponent):
+
+    def __init__(self, section_id: SectionTypes):
+        self.section_id = str(section_id)
+
+    def to_expression(self) -> Expression:
+        return Expression(
+            type=ExpressionTypes.SECTION_METADATA,
+            operation=ExpressionOperation.IN,
+            value=[self.section_id],
+        )
+
+    def __repr__(self):
+        return f"SectionMetadata({self.section_id})"
+
+    def make_copy(self) -> QueryComponent:
+        """Make a deep copy of the query component"""
+        return SectionMetadata(section_id=SectionTypes(self.section_id))
+
+
+class DocumentType(BaseQueryComponent):
+    def __init__(self, doc_type_id: DocumentTypes):
+        self.doc_type_id = str(doc_type_id)
+
+    def to_expression(self) -> Expression:
+        return Expression(
+            type=ExpressionTypes.DOCUMENT_TYPE,
+            operation=ExpressionOperation.IN,
+            value=[self.doc_type_id],
+        )
+
+    def __repr__(self):
+        return f"DocumentType({self.doc_type_id})"
+
+    def make_copy(self) -> QueryComponent:
+        """Make a deep copy of the query component"""
+        return DocumentType(doc_type_id=DocumentTypes(self.doc_type_id))
+
+
+class FiscalYear(ListQueryComponent):
+    def __init__(
+        self, *items: int, operation: ExpressionOperation = ExpressionOperation.IN
+    ):
+        # Validate the items but keep them stored raw, this is so FiscalYear can operate with itself
+        [FiscalYearValidator(value=i) for i in items]
+        super().__init__(*items, operation=operation)
+
+    def get_expression_type(self) -> ExpressionTypes:
+        return ExpressionTypes.REPORTING_PERIOD
+
+    def to_expression(self) -> Expression:
+        return Expression(
+            type=self.get_expression_type(),
+            operation=self.operation,
+            value=[FiscalYearValidator(value=i).get_string() for i in self.items],
+        )
+
+    def __or__(self, other: QueryComponent) -> QueryComponent:
+        """
+        Implementation similar to ListQueryComponent but returning
+        a ReportingPeriodAndWrapper when combining FiscalYear | FiscalQuarter
+        """
+        cls = self.__class__
+        default = Or(self, other)
+        operation = ExpressionOperation.IN
+        if not isinstance(other, (cls, FiscalQuarter, ReportingPeriodWrapper)):
+            return default
+        if len(other.items) > 1 and other.operation != operation:
+            return default
+        if len(self.items) > 1 and self.operation != operation:
+            return default
+        if isinstance(other, FiscalQuarter):
+            return ReportingPeriodWrapper(
+                FiscalYearQuarterAggregate(fiscal_year=self, fiscal_quarter=other),
+                operation=operation,
+            )
+        if isinstance(other, ReportingPeriodWrapper):
+            return (
+                ReportingPeriodWrapper(
+                    FiscalYearQuarterAggregate(fiscal_year=self), operation=operation
+                )
+                | other
+            )
+        return cls(*self.items, *other.items, operation=operation)
+
+    def __and__(self, other: QueryComponent) -> QueryComponent:
+        """
+        Implementation similar to ListQueryComponent but returning
+        a ReportingPeriodAndWrapper when combining FiscalYear & FiscalQuarter
+        """
+        cls = self.__class__
+        default = And(self, other)
+        operation = ExpressionOperation.ALL
+        if not isinstance(other, (cls, FiscalQuarter, ReportingPeriodWrapper)):
+            return default
+        if len(other.items) > 1 and other.operation != operation:
+            return default
+        if len(self.items) > 1 and self.operation != operation:
+            return default
+        if isinstance(other, FiscalQuarter):
+            return ReportingPeriodWrapper(
+                FiscalYearQuarterAggregate(fiscal_year=self, fiscal_quarter=other),
+                operation=operation,
+            )
+        if isinstance(other, ReportingPeriodWrapper):
+            return (
+                ReportingPeriodWrapper(
+                    FiscalYearQuarterAggregate(fiscal_year=self), operation=operation
+                )
+                & other
+            )
+        return cls(*self.items, *other.items, operation=operation)
+
+
+class FiscalQuarter(ListQueryComponent):
+    def __init__(
+        self, *items: int, operation: ExpressionOperation = ExpressionOperation.IN
+    ):
+        # Validate the items but keep them stored raw, this is so FiscalQuarter can operate with itself
+        [FiscalQuarterValidator(value=i).get_string() for i in items]
+        super().__init__(*items, operation=operation)
+
+    def get_expression_type(self) -> ExpressionTypes:
+        return ExpressionTypes.REPORTING_PERIOD
+
+    def to_expression(self) -> Expression:
+        return Expression(
+            type=self.get_expression_type(),
+            operation=self.operation,
+            value=[FiscalQuarterValidator(value=i).get_string() for i in self.items],
+        )
+
+    def __or__(self, other: QueryComponent) -> QueryComponent:
+        """
+        Implementation similar to ListQueryComponent but returning
+        a ReportingPeriodAndWrapper when combining FiscalYear | FiscalQuarter
+        """
+        cls = self.__class__
+        default = Or(self, other)
+        operation = ExpressionOperation.IN
+        if not isinstance(other, (cls, FiscalYear, ReportingPeriodWrapper)):
+            return default
+        if len(other.items) > 1 and other.operation != operation:
+            return default
+        if len(self.items) > 1 and self.operation != operation:
+            return default
+        if isinstance(other, FiscalYear):
+            return ReportingPeriodWrapper(
+                FiscalYearQuarterAggregate(fiscal_quarter=self, fiscal_year=other),
+                operation=operation,
+            )
+        if isinstance(other, ReportingPeriodWrapper):
+            return (
+                ReportingPeriodWrapper(
+                    FiscalYearQuarterAggregate(fiscal_quarter=self), operation=operation
+                )
+                | other
+            )
+        return cls(*self.items, *other.items, operation=operation)
+
+    def __and__(self, other: QueryComponent) -> QueryComponent:
+        """
+        Implementation similar to ListQueryComponent but returning
+        a ReportingPeriodAndWrapper when combining FiscalYear & FiscalQuarter
+        """
+        cls = self.__class__
+        default = And(self, other)
+        operation = ExpressionOperation.ALL
+        if not isinstance(other, (cls, FiscalYear, ReportingPeriodWrapper)):
+            return default
+        if len(other.items) > 1 and other.operation != operation:
+            return default
+        if len(self.items) > 1 and self.operation != operation:
+            return default
+        if isinstance(other, FiscalYear):
+            return ReportingPeriodWrapper(
+                FiscalYearQuarterAggregate(fiscal_quarter=self, fiscal_year=other),
+                operation=operation,
+            )
+        if isinstance(other, ReportingPeriodWrapper):
+            return (
+                ReportingPeriodWrapper(
+                    FiscalYearQuarterAggregate(fiscal_quarter=self), operation=operation
+                )
+                & other
+            )
+
+        return cls(*self.items, *other.items, operation=operation)
+
+
+class FiscalYearQuarterAggregate:
+    def __init__(
+        self,
+        fiscal_year: Optional[FiscalYear] = None,
+        fiscal_quarter: Optional[FiscalQuarter] = None,
+    ):
+        self.fiscal_year = fiscal_year
+        self.fiscal_quarter = fiscal_quarter
+
+
+class ReportingPeriodWrapper(ListQueryComponent):
+    """
+    This is an class that will be used when the user combines FiscalYear and FiscalQuarter so that when the expression
+    is generated elements from FiscalYear and FiscalQuarter are combined into the same values array.
+    E.g:
+    >>> (FiscalYear(2099) & FiscalQuarter(2) & FiscalQuarter(3)).to_dict()
+    {'type': 'reporting_period', 'value': ['FQ2', 'FQ3', '2099FY'], 'operation': 'all'}
+
+    """
+
+    def __init__(
+        self,
+        *items: FiscalYearQuarterAggregate,
+        operation: ExpressionOperation = ExpressionOperation.IN,
+    ):
+        super().__init__(*items, operation=operation)
+
+    def to_expression(self) -> Expression:
+        fiscal_quarters, fiscal_years = self._get_items_as_string()
+        return Expression(
+            type=self.get_expression_type(),
+            operation=self.operation,
+            value=fiscal_quarters + fiscal_years,
+        )
+
+    def make_copy(self) -> QueryComponent:
+        return ReportingPeriodWrapper(
+            fiscal_year=self.fiscal_year.make_copy(),
+            fiscal_quarter=self.fiscal_quarter.make_copy(),
+            operation=self.operation,
+        )
+
+    def get_expression_type(self) -> ExpressionTypes:
+        return ExpressionTypes.REPORTING_PERIOD
+
+    def _get_items_as_string(self) -> tuple[list[str]]:
+        fiscal_years = []
+        fiscal_quarters = []
+        for aggregate in self.items:
+            if aggregate.fiscal_year is not None:
+                fiscal_years.extend(
+                    FiscalYearValidator(value=year).get_string()
+                    for year in aggregate.fiscal_year.items
+                )
+            if aggregate.fiscal_quarter is not None:
+                fiscal_quarters.extend(
+                    FiscalQuarterValidator(value=quarter).get_string()
+                    for quarter in aggregate.fiscal_quarter.items
+                )
+        return fiscal_quarters, fiscal_years
+
+    def __repr__(self):
+        fiscal_quarters, fiscal_years = self._get_items_as_string()
+        operator = " & " if self.operation == ExpressionOperation.ALL else " | "
+        return f"FiscalYear({fiscal_years}) {operator} FiscalQuarter({fiscal_quarters})"
+
+    def __or__(self, other: QueryComponent) -> QueryComponent:
+        """
+        Implementation similar to ListQueryComponent but returning
+        a ReportingPeriodAndWrapper when combining FiscalYear | FiscalQuarter
+        """
+        cls = self.__class__
+        default = Or(self, other)
+        operation = ExpressionOperation.IN
+        if not isinstance(other, (cls, FiscalYear, FiscalQuarter)):
+            return default
+        if len(other.items) > 1 and other.operation != operation:
+            return default
+        if len(self.items) > 1 and self.operation != operation:
+            return default
+        if isinstance(other, FiscalYear):
+            return self | ReportingPeriodWrapper(
+                FiscalYearQuarterAggregate(fiscal_year=other), operation=operation
+            )
+        if isinstance(other, FiscalQuarter):
+            return self | ReportingPeriodWrapper(
+                FiscalYearQuarterAggregate(fiscal_quarter=other), operation=operation
+            )
+        return cls(*self.items, *other.items, operation=operation)
+
+    def __and__(self, other: QueryComponent) -> QueryComponent:
+        """
+        Implementation similar to ListQueryComponent but returning
+        a ReportingPeriodAndWrapper when combining FiscalYear & FiscalQuarter
+        """
+        cls = self.__class__
+        default = And(self, other)
+        operation = ExpressionOperation.ALL
+        if not isinstance(other, (cls, FiscalYear, FiscalQuarter)):
+            return default
+        if len(other.items) > 1 and other.operation != operation:
+            return default
+        if len(self.items) > 1 and self.operation != operation:
+            return default
+        if isinstance(other, FiscalYear):
+            return self & ReportingPeriodWrapper(
+                FiscalYearQuarterAggregate(fiscal_year=other), operation=operation
+            )
+        if isinstance(other, FiscalQuarter):
+            return self & ReportingPeriodWrapper(
+                FiscalYearQuarterAggregate(fiscal_quarter=other), operation=operation
+            )
+
+        return cls(*self.items, *other.items, operation=operation)
+
+
 # Watchlist is a special case, as it's not a list of items
 
 
 class Watchlist(BaseQueryComponent):
     def __init__(self, watchlist_id: str):
         self.watchlist_id = watchlist_id
```

### Comparing `bigdata_client-0.2.0/bigdata/models/comentions.py` & `bigdata_client-0.3.0/bigdata/models/comentions.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.2.0/bigdata/models/entities.py` & `bigdata_client-0.3.0/bigdata/models/entities.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.2.0/bigdata/models/languages.py` & `bigdata_client-0.3.0/bigdata/models/languages.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.2.0/bigdata/models/parse.py` & `bigdata_client-0.3.0/bigdata/models/parse.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.2.0/bigdata/models/sources.py` & `bigdata_client-0.3.0/bigdata/models/sources.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.2.0/bigdata/models/story.py` & `bigdata_client-0.3.0/bigdata/models/story.py`

 * *Files 10% similar despite different names*

```diff
@@ -48,7 +48,8 @@
     """
 
     text: str
     chunk: int
     entities: list[StorySentenceEntity]
     sentences: list[StorySentence]
     relevance: float
+    sentiment: float
```

### Comparing `bigdata_client-0.2.0/bigdata/models/topics.py` & `bigdata_client-0.3.0/bigdata/models/topics.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.2.0/bigdata/models/uploads.py` & `bigdata_client-0.3.0/bigdata/models/uploads.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,22 @@
         if self.id is None:
             raise ValueError("File not uploaded")
         content = self._api.download_analytics(self.id)
         with open(filename, "wb") as f:
             for chunk in content:
                 f.write(chunk)
 
+    def get_analytics_dict(self):
+        """Retrieves the analytics in the file, as a dictionary."""
+        if self.id is None:
+            raise ValueError("File not uploaded")
+        content_chunks = self._api.download_analytics(self.id)
+        content = b"".join(content_chunks)
+        return json.loads(content)
+
     def download_annotated(self, filename: str):
         """Downloads the annotated version of the file."""
         if self.id is None:
             raise ValueError("File not uploaded")
         content = self._api.download_annotated(self.id)
         with open(filename, "wb") as f:
             for chunk in content:
```

### Comparing `bigdata_client-0.2.0/bigdata/models/watchlists.py` & `bigdata_client-0.3.0/bigdata/models/watchlists.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.2.0/bigdata/old_auth.py` & `bigdata_client-0.3.0/bigdata/old_auth.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.2.0/bigdata/query.py` & `bigdata_client-0.3.0/bigdata/query.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,16 +3,20 @@
 This is for the user to import
 """
 
 # Coming soon:
 # from bigdata.models.advanced_search_query import ContentType  # pyright: ignore
 # from bigdata.models.advanced_search_query import Sentiment  # pyright: ignore
 
+from bigdata.models.advanced_search_query import DocumentType  # pyright: ignore
 from bigdata.models.advanced_search_query import Entity  # pyright: ignore
+from bigdata.models.advanced_search_query import FiscalQuarter  # pyright: ignore
+from bigdata.models.advanced_search_query import FiscalYear  # pyright: ignore
 from bigdata.models.advanced_search_query import Keyword  # pyright: ignore
 from bigdata.models.advanced_search_query import Language  # pyright: ignore
+from bigdata.models.advanced_search_query import SectionMetadata  # pyright: ignore
 from bigdata.models.advanced_search_query import Similarity  # pyright: ignore
 from bigdata.models.advanced_search_query import Source  # pyright: ignore
 from bigdata.models.advanced_search_query import Topic  # pyright: ignore
 from bigdata.models.advanced_search_query import Watchlist  # pyright: ignore
 from bigdata.models.advanced_search_query import all_  # pyright: ignore
 from bigdata.models.advanced_search_query import any_  # pyright: ignore
```

### Comparing `bigdata_client-0.2.0/bigdata/services.py` & `bigdata_client-0.3.0/bigdata/services.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.2.0/bigdata/settings.py` & `bigdata_client-0.3.0/bigdata/settings.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.2.0/bigdata/story.py` & `bigdata_client-0.3.0/bigdata/story.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,21 +37,22 @@
                 chunk=s.cnum,
                 entities=[
                     StorySentenceEntity(e.key, e.start, e.end, e.queryType)
                     for e in s.entities
                 ],
                 sentences=[StorySentence(e.pnum, e.snum) for e in s.sentences],
                 relevance=s.relevance,
+                sentiment=s.sentiment / 100.0,
             )
             for s in response.chunks
         ]
         story = cls(
             id=response.id,
             headline=response.headline,
-            sentiment=response.sentiment,
+            sentiment=response.sentiment / 100.0,
             story_type=response.story_type,
             source=source,
             timestamp=response.timestamp,
             chunks=chunks,
             language=response.language,
         )
         return story
```

### Comparing `bigdata_client-0.2.0/pyproject.toml` & `bigdata_client-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "bigdata-client"
 packages = [
     { include = "bigdata" },
 ]
-version = "0.2.0"
+version = "0.3.0"
 description = ""
 authors = [
     "Bigdata Team <support@bigdata.com>"
 ]
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `bigdata_client-0.2.0/PKG-INFO` & `bigdata_client-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigdata-client
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 Author: Bigdata Team
 Author-email: support@bigdata.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

