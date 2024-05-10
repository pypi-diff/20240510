# Comparing `tmp/dimsdk-1.0.3.tar.gz` & `tmp/dimsdk-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dimsdk-1.0.3.tar", last modified: Tue Dec  5 09:58:04 2023, max compression
+gzip compressed data, was "dist/dimsdk-2.0.0.tar", last modified: Fri May 10 15:45:10 2024, max compression
```

## Comparing `dimsdk-1.0.3.tar` & `dimsdk-2.0.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-12-05 09:58:04.000000 dimsdk-1.0.3/
--rw-r--r--   0 moky       (501) staff       (20)     1047 2023-12-05 09:58:04.000000 dimsdk-1.0.3/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      556 2022-12-11 05:05:26.000000 dimsdk-1.0.3/README.md
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-12-05 09:58:04.000000 dimsdk-1.0.3/dimsdk/
--rw-r--r--   0 moky       (501) staff       (20)     6860 2023-12-04 14:23:14.000000 dimsdk-1.0.3/dimsdk/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3728 2023-10-13 08:54:57.000000 dimsdk-1.0.3/dimsdk/ans.py
--rw-r--r--   0 moky       (501) staff       (20)     9232 2023-12-04 14:31:12.000000 dimsdk-1.0.3/dimsdk/archivist.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-12-05 09:58:04.000000 dimsdk-1.0.3/dimsdk/core/
--rw-r--r--   0 moky       (501) staff       (20)     2338 2023-10-12 07:11:54.000000 dimsdk-1.0.3/dimsdk/core/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     9327 2023-10-13 08:54:17.000000 dimsdk-1.0.3/dimsdk/core/factories.py
--rw-r--r--   0 moky       (501) staff       (20)     6085 2023-10-12 08:48:27.000000 dimsdk-1.0.3/dimsdk/core/proc.py
--rw-r--r--   0 moky       (501) staff       (20)     3263 2023-12-04 13:49:53.000000 dimsdk-1.0.3/dimsdk/core/twins.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-12-05 09:58:04.000000 dimsdk-1.0.3/dimsdk/cpu/
--rw-r--r--   0 moky       (501) staff       (20)     2531 2023-10-12 07:18:22.000000 dimsdk-1.0.3/dimsdk/cpu/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3328 2023-10-13 09:51:11.000000 dimsdk-1.0.3/dimsdk/cpu/base.py
--rw-r--r--   0 moky       (501) staff       (20)    10790 2023-12-04 13:57:16.000000 dimsdk-1.0.3/dimsdk/cpu/commands.py
--rw-r--r--   0 moky       (501) staff       (20)     3175 2023-10-11 03:49:15.000000 dimsdk-1.0.3/dimsdk/cpu/contents.py
--rw-r--r--   0 moky       (501) staff       (20)     3643 2023-10-12 08:47:24.000000 dimsdk-1.0.3/dimsdk/cpu/creator.py
--rw-r--r--   0 moky       (501) staff       (20)     4823 2023-10-13 09:54:29.000000 dimsdk-1.0.3/dimsdk/cpu/customized.py
--rw-r--r--   0 moky       (501) staff       (20)     6589 2023-10-12 07:27:49.000000 dimsdk-1.0.3/dimsdk/delegate.py
--rw-r--r--   0 moky       (501) staff       (20)     7643 2023-12-04 13:45:40.000000 dimsdk-1.0.3/dimsdk/facebook.py
--rw-r--r--   0 moky       (501) staff       (20)     6407 2023-10-13 08:55:05.000000 dimsdk-1.0.3/dimsdk/messenger.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-12-05 09:58:04.000000 dimsdk-1.0.3/dimsdk/mkm/
--rw-r--r--   0 moky       (501) staff       (20)     1584 2023-10-13 09:10:37.000000 dimsdk-1.0.3/dimsdk/mkm/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     2112 2023-10-29 07:01:27.000000 dimsdk-1.0.3/dimsdk/mkm/bot.py
--rw-r--r--   0 moky       (501) staff       (20)     4685 2023-10-10 16:40:26.000000 dimsdk-1.0.3/dimsdk/mkm/roles.py
--rw-r--r--   0 moky       (501) staff       (20)     7867 2023-10-29 07:05:23.000000 dimsdk-1.0.3/dimsdk/mkm/station.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-12-05 09:58:04.000000 dimsdk-1.0.3/dimsdk/msg/
--rw-r--r--   0 moky       (501) staff       (20)     1777 2023-10-29 07:21:47.000000 dimsdk-1.0.3/dimsdk/msg/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4728 2023-10-29 08:10:13.000000 dimsdk-1.0.3/dimsdk/msg/factory.py
--rw-r--r--   0 moky       (501) staff       (20)     2505 2023-10-29 07:19:01.000000 dimsdk-1.0.3/dimsdk/msg/helper.py
--rw-r--r--   0 moky       (501) staff       (20)     6782 2023-10-13 08:43:49.000000 dimsdk-1.0.3/dimsdk/msg/instant.py
--rw-r--r--   0 moky       (501) staff       (20)     3898 2023-10-13 08:49:45.000000 dimsdk-1.0.3/dimsdk/msg/reliable.py
--rw-r--r--   0 moky       (501) staff       (20)     8577 2023-10-13 08:49:50.000000 dimsdk-1.0.3/dimsdk/msg/secure.py
--rw-r--r--   0 moky       (501) staff       (20)     9070 2023-10-29 14:20:07.000000 dimsdk-1.0.3/dimsdk/packer.py
--rw-r--r--   0 moky       (501) staff       (20)     7458 2023-12-04 14:31:40.000000 dimsdk-1.0.3/dimsdk/processor.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-12-05 09:58:04.000000 dimsdk-1.0.3/dimsdk/utils/
--rw-r--r--   0 moky       (501) staff       (20)     1596 2023-12-04 14:33:51.000000 dimsdk-1.0.3/dimsdk/utils/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3803 2023-12-04 14:33:41.000000 dimsdk-1.0.3/dimsdk/utils/checker.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-12-05 09:58:04.000000 dimsdk-1.0.3/dimsdk.egg-info/
--rw-r--r--   0 moky       (501) staff       (20)     1047 2023-12-05 09:58:04.000000 dimsdk-1.0.3/dimsdk.egg-info/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      804 2023-12-05 09:58:04.000000 dimsdk-1.0.3/dimsdk.egg-info/SOURCES.txt
--rw-r--r--   0 moky       (501) staff       (20)        1 2023-12-05 09:58:04.000000 dimsdk-1.0.3/dimsdk.egg-info/dependency_links.txt
--rw-r--r--   0 moky       (501) staff       (20)       34 2023-12-05 09:58:04.000000 dimsdk-1.0.3/dimsdk.egg-info/requires.txt
--rw-r--r--   0 moky       (501) staff       (20)        7 2023-12-05 09:58:04.000000 dimsdk-1.0.3/dimsdk.egg-info/top_level.txt
--rw-r--r--   0 moky       (501) staff       (20)       38 2023-12-05 09:58:04.000000 dimsdk-1.0.3/setup.cfg
--rw-r--r--   0 moky       (501) staff       (20)     1253 2023-12-04 12:13:14.000000 dimsdk-1.0.3/setup.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:45:10.000000 dimsdk-2.0.0/
+-rw-r--r--   0 moky       (501) staff       (20)     1047 2024-05-10 15:45:10.000000 dimsdk-2.0.0/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      556 2022-12-11 05:05:26.000000 dimsdk-2.0.0/README.md
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:45:10.000000 dimsdk-2.0.0/dimsdk/
+-rw-r--r--   0 moky       (501) staff       (20)     6860 2023-12-04 14:23:14.000000 dimsdk-2.0.0/dimsdk/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3728 2023-10-13 08:54:57.000000 dimsdk-2.0.0/dimsdk/ans.py
+-rw-r--r--   0 moky       (501) staff       (20)     9358 2024-05-06 15:49:36.000000 dimsdk-2.0.0/dimsdk/archivist.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:45:10.000000 dimsdk-2.0.0/dimsdk/core/
+-rw-r--r--   0 moky       (501) staff       (20)     2338 2023-10-12 07:11:54.000000 dimsdk-2.0.0/dimsdk/core/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     9327 2023-10-13 08:54:17.000000 dimsdk-2.0.0/dimsdk/core/factories.py
+-rw-r--r--   0 moky       (501) staff       (20)     6091 2024-05-06 15:43:35.000000 dimsdk-2.0.0/dimsdk/core/proc.py
+-rw-r--r--   0 moky       (501) staff       (20)     3263 2023-12-04 13:49:53.000000 dimsdk-2.0.0/dimsdk/core/twins.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:45:10.000000 dimsdk-2.0.0/dimsdk/cpu/
+-rw-r--r--   0 moky       (501) staff       (20)     2531 2023-10-12 07:18:22.000000 dimsdk-2.0.0/dimsdk/cpu/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3340 2024-05-06 15:44:33.000000 dimsdk-2.0.0/dimsdk/cpu/base.py
+-rw-r--r--   0 moky       (501) staff       (20)    10991 2024-05-06 16:42:30.000000 dimsdk-2.0.0/dimsdk/cpu/commands.py
+-rw-r--r--   0 moky       (501) staff       (20)     3199 2024-05-06 16:42:59.000000 dimsdk-2.0.0/dimsdk/cpu/contents.py
+-rw-r--r--   0 moky       (501) staff       (20)     3643 2023-10-12 08:47:24.000000 dimsdk-2.0.0/dimsdk/cpu/creator.py
+-rw-r--r--   0 moky       (501) staff       (20)     4903 2024-05-06 16:44:10.000000 dimsdk-2.0.0/dimsdk/cpu/customized.py
+-rw-r--r--   0 moky       (501) staff       (20)     6605 2024-05-06 15:50:09.000000 dimsdk-2.0.0/dimsdk/delegate.py
+-rw-r--r--   0 moky       (501) staff       (20)     7805 2024-05-06 16:54:46.000000 dimsdk-2.0.0/dimsdk/facebook.py
+-rw-r--r--   0 moky       (501) staff       (20)     6619 2024-05-06 15:57:53.000000 dimsdk-2.0.0/dimsdk/messenger.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:45:10.000000 dimsdk-2.0.0/dimsdk/mkm/
+-rw-r--r--   0 moky       (501) staff       (20)     1584 2023-10-13 09:10:37.000000 dimsdk-2.0.0/dimsdk/mkm/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     2136 2024-05-06 15:26:05.000000 dimsdk-2.0.0/dimsdk/mkm/bot.py
+-rw-r--r--   0 moky       (501) staff       (20)     4685 2023-10-10 16:40:26.000000 dimsdk-2.0.0/dimsdk/mkm/roles.py
+-rw-r--r--   0 moky       (501) staff       (20)     8061 2024-05-06 15:37:54.000000 dimsdk-2.0.0/dimsdk/mkm/station.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:45:10.000000 dimsdk-2.0.0/dimsdk/msg/
+-rw-r--r--   0 moky       (501) staff       (20)     1777 2023-10-29 07:21:47.000000 dimsdk-2.0.0/dimsdk/msg/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4728 2023-10-29 08:10:13.000000 dimsdk-2.0.0/dimsdk/msg/factory.py
+-rw-r--r--   0 moky       (501) staff       (20)     2505 2023-10-29 07:19:01.000000 dimsdk-2.0.0/dimsdk/msg/helper.py
+-rw-r--r--   0 moky       (501) staff       (20)     6824 2024-05-06 15:39:45.000000 dimsdk-2.0.0/dimsdk/msg/instant.py
+-rw-r--r--   0 moky       (501) staff       (20)     3910 2024-05-06 15:42:22.000000 dimsdk-2.0.0/dimsdk/msg/reliable.py
+-rw-r--r--   0 moky       (501) staff       (20)     8619 2024-05-06 15:41:48.000000 dimsdk-2.0.0/dimsdk/msg/secure.py
+-rw-r--r--   0 moky       (501) staff       (20)     9182 2024-05-06 16:00:50.000000 dimsdk-2.0.0/dimsdk/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)     7560 2024-05-07 03:27:36.000000 dimsdk-2.0.0/dimsdk/processor.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:45:10.000000 dimsdk-2.0.0/dimsdk/utils/
+-rw-r--r--   0 moky       (501) staff       (20)     1596 2023-12-04 14:33:51.000000 dimsdk-2.0.0/dimsdk/utils/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3803 2023-12-04 14:33:41.000000 dimsdk-2.0.0/dimsdk/utils/checker.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:45:10.000000 dimsdk-2.0.0/dimsdk.egg-info/
+-rw-r--r--   0 moky       (501) staff       (20)     1047 2024-05-10 15:45:10.000000 dimsdk-2.0.0/dimsdk.egg-info/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      804 2024-05-10 15:45:10.000000 dimsdk-2.0.0/dimsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 moky       (501) staff       (20)        1 2024-05-10 15:45:10.000000 dimsdk-2.0.0/dimsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 moky       (501) staff       (20)       34 2024-05-10 15:45:10.000000 dimsdk-2.0.0/dimsdk.egg-info/requires.txt
+-rw-r--r--   0 moky       (501) staff       (20)        7 2024-05-10 15:45:10.000000 dimsdk-2.0.0/dimsdk.egg-info/top_level.txt
+-rw-r--r--   0 moky       (501) staff       (20)       38 2024-05-10 15:45:10.000000 dimsdk-2.0.0/setup.cfg
+-rw-r--r--   0 moky       (501) staff       (20)     1253 2024-05-10 15:42:50.000000 dimsdk-2.0.0/setup.py
```

### Comparing `dimsdk-1.0.3/PKG-INFO` & `dimsdk-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimsdk
-Version: 1.0.3
+Version: 2.0.0
 Summary: Decentralized Instant Messaging SDK
 Home-page: https://github.com/dimchat/sdk-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # Decentralized Instant Messaging (Python SDK)
```

### Comparing `dimsdk-1.0.3/README.md` & `dimsdk-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `dimsdk-1.0.3/dimsdk/__init__.py` & `dimsdk-2.0.0/dimsdk/__init__.py`

 * *Files identical despite different names*

### Comparing `dimsdk-1.0.3/dimsdk/ans.py` & `dimsdk-2.0.0/dimsdk/ans.py`

 * *Files identical despite different names*

### Comparing `dimsdk-1.0.3/dimsdk/archivist.py` & `dimsdk-2.0.0/dimsdk/archivist.py`

 * *Files 10% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
     #
     #   Meta
     #
 
     # protected
     # noinspection PyMethodMayBeStatic
-    def needs_query_meta(self, identifier: ID, meta: Optional[Meta]) -> bool:
+    async def needs_query_meta(self, identifier: ID, meta: Optional[Meta]) -> bool:
         """ check whether need to query meta """
         if identifier.is_broadcast:
             # broadcast entity has no meta to query
             return False
         elif meta is None:
             # meta not found, sure to query
             return True
@@ -86,31 +86,31 @@
     #   Last Document Times
     #
 
     def set_last_document_time(self, identifier: ID, last_time: Optional[DateTime]):
         return self.__last_document_times.set_last_time(key=identifier, last_time=last_time)
 
     # protected
-    def needs_query_documents(self, identifier: ID, documents: List[Document]) -> bool:
+    async def needs_query_documents(self, identifier: ID, documents: List[Document]) -> bool:
         """ check whether need to query documents """
         if identifier.is_broadcast:
             # broadcast entity has no document to query
             return False
         # elif documents is None:
         #     # assert False, 'should not happen'
         #     return True
         elif len(documents) == 0:
             # documents not found, sure to query
             return True
-        current = self.get_last_document_time(identifier=identifier, documents=documents)
+        current = await self.get_last_document_time(identifier=identifier, documents=documents)
         return self.__last_document_times.is_expired(key=identifier, now=current)
 
     # protected
     # noinspection PyMethodMayBeStatic
-    def get_last_document_time(self, identifier: ID, documents: List[Document]) -> Optional[DateTime]:
+    async def get_last_document_time(self, identifier: ID, documents: List[Document]) -> Optional[DateTime]:
         if documents is None or len(documents) == 0:
             return None
         last_time: Optional[DateTime] = None
         for doc in documents:
             assert doc.identifier == identifier, 'document not match: %s, %s' % (identifier, doc)
             doc_time = doc.time
             if doc_time is None:
@@ -125,114 +125,114 @@
     #   Last Group History Times
     #
 
     def set_last_group_history_time(self, group: ID, last_time: Optional[DateTime]):
         return self.__last_history_times.set_last_time(key=group, last_time=last_time)
 
     # protected
-    def needs_query_members(self, group: ID, members: List[ID]) -> bool:
+    async def needs_query_members(self, group: ID, members: List[ID]) -> bool:
         """ check whether need to query group members """
         if group.is_broadcast:
             # broadcast group has no members to query
             return False
         # elif members is None:
         #     # assert False, 'should not happen'
         #     return True
         elif len(members) == 0:
             # members not found, sure to query
             return True
-        current = self.get_last_group_history_time(group=group)
+        current = await self.get_last_group_history_time(group=group)
         return self.__last_history_times.is_expired(key=group, now=current)
 
     # protected
     @abstractmethod
-    def get_last_group_history_time(self, group: ID) -> Optional[DateTime]:
+    async def get_last_group_history_time(self, group: ID) -> Optional[DateTime]:
         raise NotImplemented
 
     #
     #   Checking
     #
 
-    def check_meta(self, identifier: ID, meta: Optional[Meta]) -> bool:
+    async def check_meta(self, identifier: ID, meta: Optional[Meta]) -> bool:
         """
         Check meta for querying
 
         :param identifier: entity ID
         :param meta:       exists meta
         :return: true on querying
         """
-        if self.needs_query_meta(identifier=identifier, meta=meta):
+        if await self.needs_query_meta(identifier=identifier, meta=meta):
             # if not self.is_meta_query_expired(identifier=identifier):
             #     # query not expired yet
             #     return False
-            return self.query_meta(identifier=identifier)
+            return await self.query_meta(identifier=identifier)
         # no need to query meta again
         return False
 
-    def check_documents(self, identifier: ID, documents: List[Document]) -> bool:
+    async def check_documents(self, identifier: ID, documents: List[Document]) -> bool:
         """
         Check documents for querying/updating
 
         :param identifier: entity ID
         :param documents:  exist documents
         :return: true on querying
         """
-        if self.needs_query_documents(identifier=identifier, documents=documents):
+        if await self.needs_query_documents(identifier=identifier, documents=documents):
             # if not self.is_documents_query_expired(identifier=identifier):
             #     # query not expired yet
             #     return False
-            return self.query_documents(identifier=identifier, documents=documents)
+            return await self.query_documents(identifier=identifier, documents=documents)
         # no need to update document now
         return False
 
-    def check_members(self, group: ID, members: List[ID]) -> bool:
+    async def check_members(self, group: ID, members: List[ID]) -> bool:
         """
         Check group members for querying
 
         :param group:   group ID
         :param members: exist members
         :return: true on querying
         """
-        if self.needs_query_members(group=group, members=members):
+        if await self.needs_query_members(group=group, members=members):
             # if not self.is_members_query_expired(group=group):
             #     # query not expired yet
             #     return False
-            return self.query_members(group=group, members=members)
+            return await self.query_members(group=group, members=members)
         # no need to update group members now
         return False
 
     #
     #   Querying
     #
 
     @abstractmethod
-    def query_meta(self, identifier: ID) -> bool:
+    async def query_meta(self, identifier: ID) -> bool:
         """
         Request for meta with entity ID
         (call 'isMetaQueryExpired()' before sending command)
 
         :param identifier: entity ID
         :return: false on duplicated
         """
         raise NotImplemented
 
     @abstractmethod
-    def query_documents(self, identifier: ID, documents: List[Document]) -> bool:
+    async def query_documents(self, identifier: ID, documents: List[Document]) -> bool:
         """
         Request for documents with entity ID
         (call 'isDocumentQueryExpired()' before sending command)
 
         :param identifier: entity ID
         :param documents:  exist documents
         :return: false on duplicated
         """
         raise NotImplemented
 
     @abstractmethod
-    def query_members(self, group: ID, members: List[ID]) -> bool:
+    async def query_members(self, group: ID, members: List[ID]) -> bool:
         """
         Request for group members with group ID
         (call 'isMembersQueryExpired()' before sending command)
 
         :param group:   group ID
         :param members: exist members
         :return: false on duplicated
@@ -240,26 +240,26 @@
         raise NotImplemented
 
     #
     #   Storage
     #
 
     @abstractmethod
-    def save_meta(self, meta: Meta, identifier: ID) -> bool:
+    async def save_meta(self, meta: Meta, identifier: ID) -> bool:
         """
         Save meta for entity ID (must verify first)
 
         :param meta:       entity meta
         :param identifier: entity ID
         :return: true on success
         """
         raise NotImplemented
 
     @abstractmethod
-    def save_document(self, document: Document) -> bool:
+    async def save_document(self, document: Document) -> bool:
         """
         Save entity document with ID (must verify first)
 
         :param document: entity document
         :return: true on success
         """
         raise NotImplemented
```

### Comparing `dimsdk-1.0.3/dimsdk/core/__init__.py` & `dimsdk-2.0.0/dimsdk/core/__init__.py`

 * *Files identical despite different names*

### Comparing `dimsdk-1.0.3/dimsdk/core/factories.py` & `dimsdk-2.0.0/dimsdk/core/factories.py`

 * *Files identical despite different names*

### Comparing `dimsdk-1.0.3/dimsdk/core/proc.py` & `dimsdk-2.0.0/dimsdk/core/proc.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 class ContentProcessor(ABC):
     """
         CPU: Content Processing Unit
         ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
     """
 
     @abstractmethod
-    def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
+    async def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
         """
         Process message content
 
         :param content: content received
         :param r_msg:   reliable message
         :return: responses to sender
         """
```

### Comparing `dimsdk-1.0.3/dimsdk/core/twins.py` & `dimsdk-2.0.0/dimsdk/core/twins.py`

 * *Files identical despite different names*

### Comparing `dimsdk-1.0.3/dimsdk/cpu/__init__.py` & `dimsdk-2.0.0/dimsdk/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `dimsdk-1.0.3/dimsdk/cpu/base.py` & `dimsdk-2.0.0/dimsdk/cpu/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     @property
     def messenger(self) -> Messenger:
         transceiver = super().messenger
         assert isinstance(transceiver, Messenger), 'transceiver error: %s' % transceiver
         return transceiver
 
     # Override
-    def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
+    async def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
         # override to process this content
         text = 'Content not support.'
         return self._respond_receipt(text=text, envelope=r_msg.envelope, content=content, extra={
             'template': 'Content (type: ${type}) not support yet!',
             'replacements': {
                 'type': content.type,
             }
@@ -79,15 +79,15 @@
 class BaseCommandProcessor(BaseContentProcessor):
     """
         Command Processing Unit
         ~~~~~~~~~~~~~~~~~~~~~~~
     """
 
     # Override
-    def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
+    async def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
         assert isinstance(content, Command), 'command error: %s' % content
         text = 'Command not support.'
         return self._respond_receipt(text=text, envelope=r_msg.envelope, content=content, extra={
             'template': 'Command (name: ${command}) not support yet!',
             'replacements': {
                 'command': content.cmd,
             }
```

### Comparing `dimsdk-1.0.3/dimsdk/cpu/commands.py` & `dimsdk-2.0.0/dimsdk/cpu/commands.py`

 * *Files 19% similar despite different names*

```diff
@@ -44,115 +44,115 @@
     """
         Meta Command Processor
         ~~~~~~~~~~~~~~~~~~~~~~
 
     """
 
     # Override
-    def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
+    async def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
         assert isinstance(content, MetaCommand), 'meta command error: %s' % content
         identifier = content.identifier
         meta = content.meta
         if meta is None:
             # query meta for ID
-            return self._get_meta(identifier=identifier, content=content, envelope=r_msg.envelope)
+            return await self._get_meta(identifier=identifier, content=content, envelope=r_msg.envelope)
         else:
             # received a meta for ID
-            return self._put_meta(meta=meta, identifier=identifier, content=content, envelope=r_msg.envelope)
+            return await self._put_meta(meta=meta, identifier=identifier, content=content, envelope=r_msg.envelope)
 
     # private
-    def _get_meta(self, identifier: ID, content: MetaCommand, envelope: Envelope) -> List[Content]:
-        meta = self.facebook.meta(identifier=identifier)
+    async def _get_meta(self, identifier: ID, content: MetaCommand, envelope: Envelope) -> List[Content]:
+        meta = await self.facebook.get_meta(identifier=identifier)
         if meta is None:
             text = 'Meta not found.'
             return self._respond_receipt(text=text, content=content, envelope=envelope, extra={
                 'template': 'Meta not found: ${ID}.',
                 'replacements': {
                     'ID': str(identifier),
                 }
             })
         # meta got
         return [
             MetaCommand.response(identifier=identifier, meta=meta)
         ]
 
     # private
-    def _put_meta(self, meta: Meta, identifier: ID, content: MetaCommand, envelope: Envelope) -> List[Content]:
+    async def _put_meta(self, meta: Meta, identifier: ID, content: MetaCommand, envelope: Envelope) -> List[Content]:
         # 1. try to save meta
-        errors = self._save_meta(identifier=identifier, meta=meta, content=content, envelope=envelope)
+        errors = await self._save_meta(identifier=identifier, meta=meta, content=content, envelope=envelope)
         if errors is not None:
             # failed
             return errors
         # 2. success
         text = 'Meta received.'
         return self._respond_receipt(text=text, content=content, envelope=envelope, extra={
             'template': 'Meta received: ${ID}.',
             'replacements': {
                 'ID': str(identifier),
             }
         })
 
     # protected
-    def _save_meta(self, meta: Meta, identifier: ID,
-                   content: MetaCommand, envelope: Envelope) -> Optional[List[Content]]:
+    async def _save_meta(self, meta: Meta, identifier: ID,
+                         content: MetaCommand, envelope: Envelope) -> Optional[List[Content]]:
         # check meta
-        if not self._check_meta(meta=meta, identifier=identifier):
+        if not await self._check_meta(meta=meta, identifier=identifier):
             text = 'Meta not valid.'
             return self._respond_receipt(text=text, content=content, envelope=envelope, extra={
                 'template': 'Meta not valid: ${ID}.',
                 'replacements': {
                     'ID': str(identifier),
                 }
             })
-        elif not self.facebook.save_meta(meta=meta, identifier=identifier):
+        elif not await self.facebook.save_meta(meta=meta, identifier=identifier):
             text = 'Meta not accepted.'
             return self._respond_receipt(text=text, content=content, envelope=envelope, extra={
                 'template': 'Meta not accepted: ${ID}.',
                 'replacements': {
                     'ID': str(identifier),
                 }
             })
         # meta saved, return no error
 
     # noinspection PyMethodMayBeStatic
-    def _check_meta(self, meta: Meta, identifier: ID) -> bool:
+    async def _check_meta(self, meta: Meta, identifier: ID) -> bool:
         return meta.valid and meta.match_identifier(identifier=identifier)
 
 
 class DocumentCommandProcessor(MetaCommandProcessor):
     """
         Document Command Processor
         ~~~~~~~~~~~~~~~~~~~~~~~~~~
 
     """
 
     # Override
-    def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
+    async def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
         assert isinstance(content, DocumentCommand), 'document command error: %s' % content
         identifier = content.identifier
         doc = content.document
         if doc is None:
             # query entity document for ID
-            return self._get_documents(identifier=identifier, content=content, envelope=r_msg.envelope)
+            return await self._get_documents(identifier=identifier, content=content, envelope=r_msg.envelope)
         elif identifier == doc.identifier:
             # received a document for ID
-            return self._put_doc(doc, identifier=identifier, content=content, envelope=r_msg.envelope)
+            return await self._put_doc(doc, identifier=identifier, content=content, envelope=r_msg.envelope)
         # error
         text = 'Document ID not match.'
         return self._respond_receipt(text=text, content=content, envelope=r_msg.envelope, extra={
             'template': 'Document ID not match: ${ID}.',
             'replacements': {
                 'ID': str(identifier),
             }
         })
 
     # private
-    def _get_documents(self, identifier: ID, content: DocumentCommand, envelope: Envelope) -> List[Content]:
+    async def _get_documents(self, identifier: ID, content: DocumentCommand, envelope: Envelope) -> List[Content]:
         facebook = self.facebook
-        documents = facebook.documents(identifier=identifier)
+        documents = await facebook.get_documents(identifier=identifier)
         count = 0 if documents is None else len(documents)
         if count == 0:
             text = 'Document not found.'
             return self._respond_receipt(text=text, content=content, envelope=envelope, extra={
                 'template': 'Document not found: ${ID}.',
                 'replacements': {
                     'ID': str(identifier),
@@ -174,85 +174,86 @@
                 return self._respond_receipt(text=text, content=content, envelope=envelope, extra={
                     'template': 'Document not updated: ${ID}, last time: ${time}.',
                     'replacements': {
                         'ID': str(identifier),
                         'time': last_time.timestamp,
                     }
                 })
-        meta = facebook.meta(identifier=identifier)
+        meta = await facebook.get_meta(identifier=identifier)
         # respond first document with meta
         command = DocumentCommand.response(identifier=identifier, meta=meta, document=documents[0])
         responses = [command]
         for i in range(1, count):
             # respond other documents
             command = DocumentCommand.response(identifier=identifier, meta=meta, document=documents[i])
             responses.append(command)
         return responses
 
     # private
-    def _put_doc(self, doc: Document, identifier: ID, content: DocumentCommand, envelope: Envelope) -> List[Content]:
+    async def _put_doc(self, doc: Document, identifier: ID,
+                       content: DocumentCommand, envelope: Envelope) -> List[Content]:
         facebook = self.facebook
         meta = content.meta
         # 0. check meta
         if meta is None:
-            meta = facebook.meta(identifier=identifier)
+            meta = await facebook.get_meta(identifier=identifier)
             if meta is None:
                 text = 'Meta not found.'
                 return self._respond_receipt(text=text, content=content, envelope=envelope, extra={
                     'template': 'Meta not found: ${ID}.',
                     'replacements': {
                         'ID': str(identifier),
                     }
                 })
         else:
             # 1. try to save meta
-            errors = self._save_meta(meta=meta, identifier=identifier, content=content, envelope=envelope)
+            errors = await self._save_meta(meta=meta, identifier=identifier, content=content, envelope=envelope)
             if errors is not None:
                 # failed
                 return errors
         # 2. try to save document
-        errors = self._save_document(doc, meta=meta, identifier=identifier, content=content, envelope=envelope)
+        errors = await self._save_document(doc, meta=meta, identifier=identifier, content=content, envelope=envelope)
         if errors is not None:
             # failed
             return errors
         # 3. success
         text = 'Document received.'
         return self._respond_receipt(text=text, content=content, envelope=envelope, extra={
             'template': 'Document received: ${ID}.',
             'replacements': {
                 'ID': str(identifier),
             }
         })
 
     # protected
-    def _save_document(self, doc: Document, meta: Meta, identifier: ID,
-                       content: DocumentCommand, envelope: Envelope) -> Optional[List[Content]]:
+    async def _save_document(self, doc: Document, meta: Meta, identifier: ID,
+                             content: DocumentCommand, envelope: Envelope) -> Optional[List[Content]]:
         # check document
-        if not self._check_document(doc, meta=meta):
+        if not await self._check_document(doc, meta=meta):
             # document error
             text = 'Document not accepted.'
             return self._respond_receipt(text=text, content=content, envelope=envelope, extra={
                 'template': 'Document not accepted: ${ID}.',
                 'replacements': {
                     'ID': str(identifier),
                 }
             })
-        elif not self.facebook.save_document(document=doc):
+        elif not await self.facebook.save_document(document=doc):
             # document expired
             text = 'Document not changed.'
             return self._respond_receipt(text=text, content=content, envelope=envelope, extra={
                 'template': 'Document not changed: ${ID}.',
                 'replacements': {
                     'ID': str(identifier),
                 }
             })
         # document saved, return no error
 
     # noinspection PyMethodMayBeStatic
-    def _check_document(self, doc: Document, meta: Meta) -> bool:
+    async def _check_document(self, doc: Document, meta: Meta) -> bool:
         if doc.valid:
             return True
         # NOTICE: if this is a bulletin document for group,
         #             verify it with the group owner's meta.key
         #         else (this is a visa document for user)
         #             verify it with the user's meta.key
         return doc.verify(public_key=meta.public_key)
```

### Comparing `dimsdk-1.0.3/dimsdk/cpu/contents.py` & `dimsdk-2.0.0/dimsdk/cpu/contents.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,22 +41,22 @@
     """
         Forward Content Processor
         ~~~~~~~~~~~~~~~~~~~~~~~~~
 
     """
 
     # Override
-    def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
+    async def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
         assert isinstance(content, ForwardContent), 'forward content error: %s' % content
         # call messenger to process it
         messenger = self.messenger
         secrets = content.secrets
         responses = []
         for item in secrets:
-            results = messenger.process_reliable_message(msg=item)
+            results = await messenger.process_reliable_message(msg=item)
             if len(results) == 1:
                 res = ForwardContent.create(message=results[0])
             else:
                 res = ForwardContent.create(messages=results)
             responses.append(res)
         return responses
 
@@ -65,21 +65,21 @@
     """
         Array Content Processor
         ~~~~~~~~~~~~~~~~~~~~~~~
 
     """
 
     # Override
-    def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
+    async def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
         assert isinstance(content, ArrayContent), 'forward content error: %s' % content
         # call messenger to process it
         messenger = self.messenger
         contents = content.contents
         responses = []
         for item in contents:
-            results = messenger.process_content(content=item, r_msg=r_msg)
+            results = await messenger.process_content(content=item, r_msg=r_msg)
             if len(results) == 1:
                 res = results[0]
             else:
                 res = ArrayContent.create(contents=results)
             responses.append(res)
         return responses
```

### Comparing `dimsdk-1.0.3/dimsdk/cpu/creator.py` & `dimsdk-2.0.0/dimsdk/cpu/creator.py`

 * *Files identical despite different names*

### Comparing `dimsdk-1.0.3/dimsdk/cpu/customized.py` & `dimsdk-2.0.0/dimsdk/cpu/customized.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,15 +41,16 @@
 class CustomizedContentHandler(ABC):
     """
         Handler for Customized Content
         ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
     """
 
     @abstractmethod
-    def handle_action(self, act: str, sender: ID, content: CustomizedContent, msg: ReliableMessage) -> List[Content]:
+    async def handle_action(self, act: str, sender: ID,
+                            content: CustomizedContent, msg: ReliableMessage) -> List[Content]:
         """
         Do your job
 
         @param act:     action
         @param sender:  user ID
         @param content: customized content
         @param msg:     network message
@@ -61,15 +62,15 @@
 class CustomizedContentProcessor(BaseContentProcessor, CustomizedContentHandler):
     """
         Customized Content Processing Unit
         ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
     """
 
     # Override
-    def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
+    async def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
         assert isinstance(content, CustomizedContent), 'customized content error: %s' % content
         # 1. check app id
         app = content.application
         responses = self._filter(app, content=content, msg=r_msg)
         if responses is not None:
             # app id not found
             return responses
@@ -78,15 +79,15 @@
         handler = self._fetch(mod, content=content, msg=r_msg)
         if handler is None:
             # module not support
             return []
         # 3. do the job
         act = content.action
         sender = r_msg.sender
-        return handler.handle_action(act, sender=sender, content=content, msg=r_msg)
+        return await handler.handle_action(act, sender=sender, content=content, msg=r_msg)
 
     # noinspection PyUnusedLocal
     def _filter(self, app: str, content: CustomizedContent, msg: ReliableMessage) -> Optional[List[Content]]:
         # Override for your application
         """
         Check for application
 
@@ -107,15 +108,16 @@
     def _fetch(self, mod: str, content: CustomizedContent, msg: ReliableMessage) -> Optional[CustomizedContentHandler]:
         """ Override for you module """
         # if the application has too many modules, I suggest you to
         # use different handler to do the job for each module.
         return self
 
     # Override
-    def handle_action(self, act: str, sender: ID, content: CustomizedContent, msg: ReliableMessage) -> List[Content]:
+    async def handle_action(self, act: str, sender: ID,
+                            content: CustomizedContent, msg: ReliableMessage) -> List[Content]:
         """ Override for customized actions """
         app = content.application
         mod = content.module
         text = 'Content not support.'
         return self._respond_receipt(text=text, content=content, envelope=msg.envelope, extra={
             'template': 'Customized content (app: ${app}, mod: ${mod}, act: ${act}) not support yet!',
             'replacements': {
```

### Comparing `dimsdk-1.0.3/dimsdk/delegate.py` & `dimsdk-2.0.0/dimsdk/delegate.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,27 +108,27 @@
             return receiver
         else:
             # H    : group message split for someone
             # J    : (receiver == group) non-split group message
             return group
 
     @abstractmethod
-    def cipher_key(self, sender: ID, receiver: ID, generate: bool = False) -> Optional[SymmetricKey]:
+    async def get_cipher_key(self, sender: ID, receiver: ID, generate: bool = False) -> Optional[SymmetricKey]:
         """
         Get cipher key for encrypt message from 'sender' to 'receiver'
 
         :param sender:   user or contact ID
         :param receiver: contact or user/group ID
         :param generate: generate when key not exists
         :return:         cipher key
         """
         raise NotImplemented
 
     @abstractmethod
-    def cache_cipher_key(self, key: SymmetricKey, sender: ID, receiver: ID):
+    async def cache_cipher_key(self, key: SymmetricKey, sender: ID, receiver: ID):
         """
         Cache cipher key for reusing, with direction (from 'sender' to 'receiver')
 
         :param key:      cipher key from a contact
         :param sender:   user or contact ID
         :param receiver: contact or user/group ID
         """
```

### Comparing `dimsdk-1.0.3/dimsdk/facebook.py` & `dimsdk-2.0.0/dimsdk/facebook.py`

 * *Files 11% similar despite different names*

```diff
@@ -54,19 +54,19 @@
 
     @property
     @abstractmethod
     def archivist(self) -> Archivist:
         raise NotImplemented
 
     # Override
-    def create_user(self, identifier: ID) -> Optional[User]:
+    async def create_user(self, identifier: ID) -> Optional[User]:
         assert identifier.is_user, 'user ID error: %s' % identifier
         # check visa key
         if not identifier.is_broadcast:
-            if self.public_key_for_encryption(identifier=identifier) is None:
+            if await self.public_key_for_encryption(identifier=identifier) is None:
                 # assert False, 'visa.key not found: %s' % identifier
                 return None
             #
             #   NOTICE: if visa.key exists, then visa & meta must exist too.
             #
         network = identifier.type
         # check user type
@@ -74,19 +74,19 @@
             return Station(identifier=identifier)
         elif network == EntityType.BOT:
             return Bot(identifier=identifier)
         # general user, or 'anyone@anywhere'
         return BaseUser(identifier=identifier)
 
     # Override
-    def create_group(self, identifier: ID) -> Optional[Group]:
+    async def create_group(self, identifier: ID) -> Optional[Group]:
         assert identifier.is_group, 'group ID error: %s' % identifier
         # check members
         if not identifier.is_broadcast:
-            members = self.members(identifier=identifier)
+            members = await self.get_members(identifier=identifier)
             if len(members) == 0:
                 # assert False, 'group members not found: %s' % identifier
                 return None
             #
             #   NOTICE: if members exist, then owner (founder) must exist,
             #           and bulletin & meta must exist too.
             #
@@ -95,25 +95,25 @@
         if network == EntityType.ISP:
             return ServiceProvider(identifier=identifier)
         # general group, or 'everyone@everywhere'
         return BaseGroup(identifier=identifier)
 
     @property
     @abstractmethod
-    def local_users(self) -> List[User]:
+    async def local_users(self) -> List[User]:
         """
         Get all local users (for decrypting received message)
 
         :return: users with private key
         """
         raise NotImplemented
 
-    def select_user(self, receiver: ID) -> Optional[User]:
+    async def select_user(self, receiver: ID) -> Optional[User]:
         """ Select local user for receiver """
-        users = self.local_users
+        users = await self.local_users
         if len(users) == 0:
             assert False, 'local users should not be empty'
             # return None
         elif receiver.is_broadcast:
             # broadcast message can decrypt by anyone, so just return current user
             return users[0]
         elif receiver.is_user:
@@ -125,81 +125,81 @@
                     return item
             # not me?
             return None
         # group message (recipient not designated)
         assert receiver.is_group, 'receiver error: %s' % receiver
         # the messenger will check group info before decrypting message,
         # so we can trust that the group's meta & members MUST exist here.
-        members = self.members(identifier=receiver)
+        members = await self.get_members(identifier=receiver)
         assert len(members) > 0, 'members not found: %s' % receiver
         for item in users:
             if item.identifier in members:
                 # DISCUSS: set this item to be current user?
                 return item
 
-    def save_meta(self, meta: Meta, identifier: ID) -> bool:
+    async def save_meta(self, meta: Meta, identifier: ID) -> bool:
         if meta.valid and meta.match_identifier(identifier=identifier):
             # meta ok
             pass
         else:
             # assert False, 'meta not valid: %s' % identifier
             return False
         # check old meta
-        old = self.meta(identifier=identifier)
+        old = await self.get_meta(identifier=identifier)
         if old is not None:
             # assert meta == old, 'meta should not changed'
             return True
         # meta not exists yet, save it
         db = self.archivist
-        return db.save_meta(meta=meta, identifier=identifier)
+        return await db.save_meta(meta=meta, identifier=identifier)
 
-    def save_document(self, document: Document) -> bool:
+    async def save_document(self, document: Document) -> bool:
         identifier = document.identifier
         # assert identifier is not None, 'document error: %s' % document
         if not document.valid:
             # try to verify
-            meta = self.meta(identifier=identifier)
+            meta = await self.get_meta(identifier=identifier)
             if meta is None:
                 # assert False, 'meta not found: %s' % identifier
                 return False
             elif document.verify(public_key=meta.public_key):
                 # document ok
                 pass
             else:
                 # assert False, 'failed to verify document: %s' % identifier
                 return False
         doc_type = document.type
         if doc_type is None:
             doc_type = '*'
         # check old documents with type
-        all_documents = self.documents(identifier=identifier)
+        all_documents = await self.get_documents(identifier=identifier)
         old_doc = DocumentHelper.last_document(documents=all_documents, doc_type=doc_type)
         if old_doc is not None and DocumentHelper.is_expired(document, old_doc):
             # assert False, 'drop expired document: %s' % identifier
             return False
         # document ok, save it
         db = self.archivist
-        return db.save_document(document=document)
+        return await db.save_document(document=document)
 
     #
     #   EntityDataSource
     #
 
     # Override
-    def meta(self, identifier: ID) -> Optional[Meta]:
+    async def get_meta(self, identifier: ID) -> Optional[Meta]:
         # if identifier.is_broadcast:
         #     # broadcast ID has no meta
         #     return None
         db = self.archivist
-        info = db.meta(identifier=identifier)
-        db.check_meta(identifier=identifier, meta=info)
+        info = await db.get_meta(identifier=identifier)
+        await db.check_meta(identifier=identifier, meta=info)
         return info
 
     # Override
-    def documents(self, identifier: ID) -> List[Document]:
+    async def get_documents(self, identifier: ID) -> List[Document]:
         if identifier.is_broadcast:
             # broadcast ID has no documents
             return []
         db = self.archivist
-        docs = db.documents(identifier=identifier)
-        db.check_documents(identifier=identifier, documents=docs)
+        docs = await db.get_documents(identifier=identifier)
+        await db.check_documents(identifier=identifier, documents=docs)
         return docs
```

### Comparing `dimsdk-1.0.3/dimsdk/messenger.py` & `dimsdk-2.0.0/dimsdk/messenger.py`

 * *Files 12% similar despite different names*

```diff
@@ -66,112 +66,112 @@
         """ Delegate for Processing Message """
         raise NotImplemented
 
     #
     #   Interfaces for Cipher Key
     #
 
-    def get_encrypt_key(self, msg: InstantMessage) -> Optional[SymmetricKey]:
+    async def get_encrypt_key(self, msg: InstantMessage) -> Optional[SymmetricKey]:
         sender = msg.sender
         target = CipherKeyDelegate.destination_for_message(msg=msg)
         delegate = self.key_cache
-        return delegate.cipher_key(sender=sender, receiver=target, generate=True)
+        return await delegate.get_cipher_key(sender=sender, receiver=target, generate=True)
 
-    def get_decrypt_key(self, msg: SecureMessage) -> Optional[SymmetricKey]:
+    async def get_decrypt_key(self, msg: SecureMessage) -> Optional[SymmetricKey]:
         sender = msg.sender
         target = CipherKeyDelegate.destination_for_message(msg=msg)
         delegate = self.key_cache
-        return delegate.cipher_key(sender=sender, receiver=target, generate=False)
+        return await delegate.get_cipher_key(sender=sender, receiver=target, generate=False)
 
-    def cache_decrypt_key(self, key: SymmetricKey, msg: SecureMessage):
+    async def cache_decrypt_key(self, key: SymmetricKey, msg: SecureMessage):
         sender = msg.sender
         target = CipherKeyDelegate.destination_for_message(msg=msg)
         delegate = self.key_cache
-        return delegate.cache_cipher_key(key=key, sender=sender, receiver=target)
+        return await delegate.cache_cipher_key(key=key, sender=sender, receiver=target)
 
     #
     #   Interfaces for Packing Message
     #
 
     # Override
-    def encrypt_message(self, msg: InstantMessage) -> Optional[SecureMessage]:
+    async def encrypt_message(self, msg: InstantMessage) -> Optional[SecureMessage]:
         delegate = self.packer
-        return delegate.encrypt_message(msg=msg)
+        return await delegate.encrypt_message(msg=msg)
 
     # Override
-    def sign_message(self, msg: SecureMessage) -> Optional[ReliableMessage]:
+    async def sign_message(self, msg: SecureMessage) -> Optional[ReliableMessage]:
         delegate = self.packer
-        return delegate.sign_message(msg=msg)
+        return await delegate.sign_message(msg=msg)
 
     # Override
-    def serialize_message(self, msg: ReliableMessage) -> Optional[bytes]:
+    async def serialize_message(self, msg: ReliableMessage) -> Optional[bytes]:
         delegate = self.packer
-        return delegate.serialize_message(msg=msg)
+        return await delegate.serialize_message(msg=msg)
 
     # Override
-    def deserialize_message(self, data: bytes) -> Optional[ReliableMessage]:
+    async def deserialize_message(self, data: bytes) -> Optional[ReliableMessage]:
         delegate = self.packer
-        return delegate.deserialize_message(data=data)
+        return await delegate.deserialize_message(data=data)
 
     # Override
-    def verify_message(self, msg: ReliableMessage) -> Optional[SecureMessage]:
+    async def verify_message(self, msg: ReliableMessage) -> Optional[SecureMessage]:
         delegate = self.packer
-        return delegate.verify_message(msg=msg)
+        return await delegate.verify_message(msg=msg)
 
     # Override
-    def decrypt_message(self, msg: SecureMessage) -> Optional[InstantMessage]:
+    async def decrypt_message(self, msg: SecureMessage) -> Optional[InstantMessage]:
         delegate = self.packer
-        return delegate.decrypt_message(msg=msg)
+        return await delegate.decrypt_message(msg=msg)
 
     #
     #   Interfaces for Processing Message
     #
 
     # Override
-    def process_package(self, data: bytes) -> List[bytes]:
+    async def process_package(self, data: bytes) -> List[bytes]:
         delegate = self.processor
-        return delegate.process_package(data=data)
+        return await delegate.process_package(data=data)
 
     # Override
-    def process_reliable_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
+    async def process_reliable_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
         delegate = self.processor
-        return delegate.process_reliable_message(msg=msg)
+        return await delegate.process_reliable_message(msg=msg)
 
     # Override
-    def process_secure_message(self, msg: SecureMessage, r_msg: ReliableMessage) -> List[SecureMessage]:
+    async def process_secure_message(self, msg: SecureMessage, r_msg: ReliableMessage) -> List[SecureMessage]:
         delegate = self.processor
-        return delegate.process_secure_message(msg=msg, r_msg=r_msg)
+        return await delegate.process_secure_message(msg=msg, r_msg=r_msg)
 
     # Override
-    def process_instant_message(self, msg: InstantMessage, r_msg: ReliableMessage) -> List[InstantMessage]:
+    async def process_instant_message(self, msg: InstantMessage, r_msg: ReliableMessage) -> List[InstantMessage]:
         delegate = self.processor
-        return delegate.process_instant_message(msg=msg, r_msg=r_msg)
+        return await delegate.process_instant_message(msg=msg, r_msg=r_msg)
 
     # Override
-    def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
+    async def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
         delegate = self.processor
-        return delegate.process_content(content=content, r_msg=r_msg)
+        return await delegate.process_content(content=content, r_msg=r_msg)
 
     #
     #   SecureMessageDelegate
     #
 
     # Override
-    def deserialize_key(self, data: Optional[bytes], msg: SecureMessage) -> Optional[SymmetricKey]:
+    async def deserialize_key(self, data: Optional[bytes], msg: SecureMessage) -> Optional[SymmetricKey]:
         if data is None:
             # get key from cache with direction: sender -> receiver(group)
-            return self.get_decrypt_key(msg=msg)
+            return await self.get_decrypt_key(msg=msg)
         else:
-            return super().deserialize_key(data=data, msg=msg)
+            return await super().deserialize_key(data=data, msg=msg)
 
     # Override
-    def deserialize_content(self, data: bytes, key: SymmetricKey, msg: SecureMessage) -> Optional[Content]:
-        content = super().deserialize_content(data=data, key=key, msg=msg)
+    async def deserialize_content(self, data: bytes, key: SymmetricKey, msg: SecureMessage) -> Optional[Content]:
+        content = await super().deserialize_content(data=data, key=key, msg=msg)
         # cache decrypt key when success
         if content is None:
             assert False, 'content error: %d' % len(data)
         else:
             # cache the key with direction: sender -> receiver(group)
-            self.cache_decrypt_key(key=key, msg=msg)
+            await self.cache_decrypt_key(key=key, msg=msg)
         # NOTICE: check attachment for File/Image/Audio/Video message content
         #         after deserialize content, this job should be do in subclass
         return content
```

### Comparing `dimsdk-1.0.3/dimsdk/mkm/__init__.py` & `dimsdk-2.0.0/dimsdk/mkm/__init__.py`

 * *Files identical despite different names*

### Comparing `dimsdk-1.0.3/dimsdk/mkm/bot.py` & `dimsdk-2.0.0/dimsdk/mkm/bot.py`

 * *Files 12% similar despite different names*

```diff
@@ -43,17 +43,17 @@
 class Bot(BaseUser):
 
     def __init__(self, identifier: ID):
         super().__init__(identifier=identifier)
         assert identifier.type == EntityType.BOT, 'Bot ID type error: %s' % identifier
 
     @property
-    def profile(self) -> Optional[Document]:
+    async def profile(self) -> Optional[Document]:
         """ Bot Document """
-        return self.visa
+        return await self.visa
 
     @property
-    def provider(self) -> Optional[ID]:
-        doc = self.profile
+    async def provider(self) -> Optional[ID]:
+        doc = await self.profile
         if doc is not None:
             icp = doc.get_property(key='ICP')
             return ID.parse(identifier=icp)
```

### Comparing `dimsdk-1.0.3/dimsdk/mkm/roles.py` & `dimsdk-2.0.0/dimsdk/mkm/roles.py`

 * *Files identical despite different names*

### Comparing `dimsdk-1.0.3/dimsdk/mkm/station.py` & `dimsdk-2.0.0/dimsdk/mkm/station.py`

 * *Files 19% similar despite different names*

```diff
@@ -85,53 +85,54 @@
         """ Return self!=value. """
         if isinstance(other, Station):
             # check ID, host & port
             return not same_stations(self, other)
         # check with inner user's ID
         return self.__user != other
 
-    def reload(self):
+    async def reload(self):
         """ Reload station info: host & port, SP ID """
-        doc = self.profile
+        doc = await self.profile
         if doc is not None:
             host = doc.get_property(key='host')
+            host = Converter.get_str(value=host, default=None)
             if host is not None:
-                self.__host = Converter.get_str(value=host, default=None)
+                self.__host = host
             port = doc.get_property(key='port')
-            if port is not None:
-                self.__port = Converter.get_int(value=port, default=0)
+            port = Converter.get_int(value=port, default=0)
+            if port > 0:
+                self.__port = port
             isp = doc.get_property(key='ISP')
+            isp = ID.parse(identifier=isp)
             if isp is not None:
-                self.__isp = ID.parse(identifier=isp)
+                self.__isp = isp
 
     @property
-    def profile(self) -> Optional[Document]:
+    async def profile(self) -> Optional[Document]:
         """ Station Document """
-        return DocumentHelper.last_document(documents=self.documents)
+        docs = await self.documents
+        return DocumentHelper.last_document(documents=docs)
 
     #
     #   Server
     #
 
     @property
     def host(self) -> str:
-        if self.__host is None:
-            self.reload()
+        """ Station IP """
         return self.__host
 
     @property
     def port(self) -> int:
-        if self.__port == 0:
-            self.reload()
+        """ Station Port """
         return self.__port
 
     @property
     def provider(self) -> Optional[ID]:
-        if self.__isp is None:
-            self.reload()
+        """ ISP ID, station group """
         return self.__isp
 
     #
     #   Entity
     #
 
     @property  # Override
@@ -153,72 +154,73 @@
         return self.__user.data_source
 
     @data_source.setter  # Override
     def data_source(self, delegate: UserDataSource):
         self.__user.data_source = delegate
 
     @property  # Override
-    def meta(self) -> Meta:
-        return self.__user.meta
+    async def meta(self) -> Meta:
+        return await self.__user.meta
 
     @property  # Override
-    def documents(self) -> List[Document]:
-        return self.__user.documents
+    async def documents(self) -> List[Document]:
+        return await self.__user.documents
 
     #
     #   User
     #
 
     @property  # Override
-    def visa(self) -> Optional[Visa]:
-        return self.__user.visa
+    async def visa(self) -> Optional[Visa]:
+        return await self.__user.visa
 
     @property  # Override
-    def contacts(self) -> List[ID]:
-        return self.__user.contacts
+    async def contacts(self) -> List[ID]:
+        return await self.__user.contacts
 
     # Override
-    def verify(self, data: bytes, signature: bytes) -> bool:
-        return self.__user.verify(data=data, signature=signature)
+    async def verify(self, data: bytes, signature: bytes) -> bool:
+        return await self.__user.verify(data=data, signature=signature)
 
     # Override
-    def encrypt(self, data: bytes) -> bytes:
-        return self.__user.encrypt(data=data)
+    async def encrypt(self, data: bytes) -> bytes:
+        return await self.__user.encrypt(data=data)
 
     # Override
-    def sign(self, data: bytes) -> bytes:
-        return self.__user.sign(data=data)
+    async def sign(self, data: bytes) -> bytes:
+        return await self.__user.sign(data=data)
 
     # Override
-    def decrypt(self, data: bytes) -> Optional[bytes]:
-        return self.__user.decrypt(data=data)
+    async def decrypt(self, data: bytes) -> Optional[bytes]:
+        return await self.__user.decrypt(data=data)
 
     # Override
-    def sign_visa(self, visa: Visa) -> Visa:
-        return self.__user.sign_visa(visa=visa)
+    async def sign_visa(self, visa: Visa) -> Visa:
+        return await self.__user.sign_visa(visa=visa)
 
     # Override
-    def verify_visa(self, visa: Visa) -> bool:
-        return self.__user.verify_visa(visa=visa)
+    async def verify_visa(self, visa: Visa) -> bool:
+        return await self.__user.verify_visa(visa=visa)
 
 
 class ServiceProvider(BaseGroup):
 
     def __init__(self, identifier: ID):
         super().__init__(identifier=identifier)
         assert identifier.type == EntityType.ISP, 'Service Provider ID type error: %s' % identifier
 
     @property
-    def profile(self) -> Optional[Document]:
+    async def profile(self) -> Optional[Document]:
         """ Provider Document """
-        return DocumentHelper.last_document(documents=self.documents)
+        docs = await self.documents
+        return DocumentHelper.last_document(documents=docs)
 
     @property
-    def stations(self) -> List:
-        doc = self.profile
+    async def stations(self) -> List:
+        doc = await self.profile
         if doc is not None:
             array = doc.get_property(key='stations')
             if array is not None:
                 return array
         # TODO: load from local storage
         return []
```

### Comparing `dimsdk-1.0.3/dimsdk/msg/__init__.py` & `dimsdk-2.0.0/dimsdk/msg/__init__.py`

 * *Files identical despite different names*

### Comparing `dimsdk-1.0.3/dimsdk/msg/factory.py` & `dimsdk-2.0.0/dimsdk/msg/factory.py`

 * *Files identical despite different names*

### Comparing `dimsdk-1.0.3/dimsdk/msg/helper.py` & `dimsdk-2.0.0/dimsdk/msg/helper.py`

 * *Files identical despite different names*

### Comparing `dimsdk-1.0.3/dimsdk/msg/instant.py` & `dimsdk-2.0.0/dimsdk/msg/instant.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,16 +61,16 @@
             | time     |  ->  | time     |
             |          |      |          |
             | content  |      | data     |  1. data = encrypt(content, PW)
             +----------+      | key/keys |  2. key  = encrypt(PW, receiver.PK)
                               +----------+
     """
 
-    def encrypt_message(self, msg: InstantMessage, password: SymmetricKey,
-                        members: List[ID] = None) -> Optional[SecureMessage]:
+    async def encrypt_message(self, msg: InstantMessage, password: SymmetricKey,
+                              members: List[ID] = None) -> Optional[SecureMessage]:
         """
         1. Encrypt message, replace 'content' field with encrypted 'data'
         2. Encrypt group message, replace 'content' field with encrypted 'data'
 
         :param msg:      plain message
         :param password: symmetric key
         :param members:  group members for group message
@@ -78,20 +78,20 @@
         """
         # TODO: check attachment for File/Image/Audio/Video message content
         #       (do it by application)
         transceiver = self.delegate
         #
         #   1. Serialize 'message.content' to data (JsON / ProtoBuf / ...)
         #
-        body = transceiver.serialize_content(content=msg.content, key=password, msg=msg)
+        body = await transceiver.serialize_content(content=msg.content, key=password, msg=msg)
         assert len(body) > 0, 'failed to serialize content: %s' % msg.content
         #
         #   2. Encrypt content data to 'message.data' with symmetric key
         #
-        ciphertext = transceiver.encrypt_content(data=body, key=password, msg=msg)
+        ciphertext = await transceiver.encrypt_content(data=body, key=password, msg=msg)
         assert len(ciphertext) > 0, 'failed to encrypt content with key: %s' % password
         #
         #   3. Encode 'message.data' to String (Base64)
         #
         if BaseMessage.is_broadcast(msg=msg):
             # broadcast message content will not be encrypted (just encoded to JsON),
             # so no need to encode to Base64 here
@@ -104,28 +104,28 @@
         # replace 'content' with encrypted 'data
         info = msg.copy_dictionary(deep_copy=False)
         info.pop('content', None)
         info['data'] = encoded_data
         #
         #   4. Serialize message key to data (JsON / ProtoBuf / ...)
         #
-        pwd = transceiver.serialize_key(key=password, msg=msg)
+        pwd = await transceiver.serialize_key(key=password, msg=msg)
         if pwd is None:
             # A) broadcast message has no key
             # B) reused key
             return SecureMessage.parse(msg=info)
         # encrypt + encode key
         if members is None:
             # personal message
             receiver = msg.receiver
             assert receiver.is_user, 'message.receiver error: %s' % receiver
             #
             #   5. Encrypt key data to 'message.key/keys' with receiver's public key
             #
-            encrypted_key = transceiver.encrypt_key(data=pwd, receiver=receiver, msg=msg)
+            encrypted_key = await transceiver.encrypt_key(data=pwd, receiver=receiver, msg=msg)
             if encrypted_key is None:
                 # public key for encryption not found
                 # TODO: suspend this message for waiting receiver's visa
                 return None
             #
             #   6. Encode message key to String (Base64)
             #
@@ -135,15 +135,15 @@
         else:
             # group message
             keys = {}
             for receiver in members:
                 #
                 #   5. Encrypt key data to 'message.keys' with member's public key
                 #
-                encrypted_key = transceiver.encrypt_key(data=pwd, receiver=receiver, msg=msg)
+                encrypted_key = await transceiver.encrypt_key(data=pwd, receiver=receiver, msg=msg)
                 if encrypted_key is None:
                     # public key for member not found
                     # TODO: suspend this message for waiting member's visa
                     continue
                 #
                 #   6. Encode message key to String (Base64)
                 #
```

### Comparing `dimsdk-1.0.3/dimsdk/msg/reliable.py` & `dimsdk-2.0.0/dimsdk/msg/reliable.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             | data     |      | data     |  1. verify(data, signature, sender.PK)
             | key/keys |      | key/keys |
             | signature|      +----------+
             +----------+
     """
 
     @abstractmethod
-    def verify_message(self, msg: ReliableMessage) -> Optional[SecureMessage]:
+    async def verify_message(self, msg: ReliableMessage) -> Optional[SecureMessage]:
         """
         Verify 'data' and 'signature' field with sender's public key
 
         :param msg: network message
         :return: SecureMessage object if signature matched
         """
         transceiver = self.delegate
@@ -85,15 +85,15 @@
         if len(signature) == 0:
             # assert False, 'failed to decode message signature: %s => %s, %s'\
             #               % (msg.sender, msg.receiver, msg.group)
             return None
         #
         #   2. Verify the message data and signature with sender's public key
         #
-        ok = transceiver.verify_data_signature(data=ciphertext, signature=signature, msg=msg)
+        ok = await transceiver.verify_data_signature(data=ciphertext, signature=signature, msg=msg)
         if not ok:
             # assert False, 'message signature not match: %s => %s, %s'\
             #               % (msg.sender, msg.receiver, msg.group)
             return None
         # OK, pack message
         info = msg.copy_dictionary(deep_copy=False)
         info.pop('signature', None)
```

### Comparing `dimsdk-1.0.3/dimsdk/msg/secure.py` & `dimsdk-2.0.0/dimsdk/msg/secure.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             |          |      |          |  1. PW      = decrypt(key, receiver.SK)
             | data     |      | content  |  2. content = decrypt(data, PW)
             | key/keys |      +----------+
             +----------+
     """
 
     @abstractmethod
-    def decrypt_message(self, msg: SecureMessage, receiver: ID) -> Optional[InstantMessage]:
+    async def decrypt_message(self, msg: SecureMessage, receiver: ID) -> Optional[InstantMessage]:
         """
         Decrypt message, replace encrypted 'data' with 'content' field
 
         :param msg:      encrypted message
         :param receiver: actual receiver (local user)
         :return: InstantMessage object
         """
@@ -81,28 +81,28 @@
             key_data = None
         else:
             assert len(encrypted_key) > 0, 'encrypted key data should not be empty: %s => %s, %s'\
                                            % (msg.sender, receiver, msg.group)
             #
             #   2. Decrypt 'message.key' with receiver's private key
             #
-            key_data = transceiver.decrypt_key(data=encrypted_key, receiver=receiver, msg=msg)
+            key_data = await transceiver.decrypt_key(data=encrypted_key, receiver=receiver, msg=msg)
             if key_data is None:
                 # A: my visa updated but the sender doesn't got the new one;
                 # B: key data error.
                 raise ValueError('failed to decrypt message key: %d byte(s) %s => %s, %s'
                                  % (len(encrypted_key), msg.sender, receiver, msg.group))
                 # TODO: check whether my visa key is changed, push new visa to this contact
             assert len(key_data) > 0, 'message key data should not be empty: %s => %s, %s'\
                                       % (msg.sender, receiver, msg.group)
         #
         #   3. Deserialize message key from data (JsON / ProtoBuf / ...)
         #      (if key is empty, means it should be reused, get it from key cache)
         #
-        password = transceiver.deserialize_key(data=key_data, msg=msg)
+        password = await transceiver.deserialize_key(data=key_data, msg=msg)
         if password is None:
             # A: key data is empty, and cipher key not found from local storage;
             # B: key data error.
             raise ValueError('failed to get message key: %d byte(s) %s => %s, %s'
                              % (0 if key_data is None else len(key_data), msg.sender, receiver, msg.group))
             # TODO: ask the sender to send again (with new message key)
         #
@@ -111,27 +111,27 @@
         ciphertext = msg.data
         if len(ciphertext) == 0:
             # assert False, 'failed to decode message data: %s => %s, %s' % (msg.sender, receiver, msg.group)
             return None
         #
         #   5. Decrypt 'message.data' with symmetric key
         #
-        body = transceiver.decrypt_content(data=ciphertext, key=password, msg=msg)
+        body = await transceiver.decrypt_content(data=ciphertext, key=password, msg=msg)
         if body is None:
             # A: password is a reused key loaded from local storage, but it's expired;
             # B: key error.
             raise ValueError('failed to decrypt message data with key: %s, data length: %d bytes %s => %s, %s'
                              % (password, len(ciphertext), msg.sender, receiver, msg.group))
             # TODO: ask the sender to send again
         assert len(body) > 0, 'message data should not be empty: %s => %s, %s'\
                               % (msg.sender, receiver, msg.group)
         #
         #   6. Deserialize message content from data (JsON / ProtoBuf / ...)
         #
-        content = transceiver.deserialize_content(data=body, key=password, msg=msg)
+        content = await transceiver.deserialize_content(data=body, key=password, msg=msg)
         if content is None:
             # assert False, 'failed to deserialize content: %d byte(s) %s => %s, %s'\
             #               % (len(body), msg.sender, receiver, msg.group)
             return None
         # TODO: check attachment for File/Image/Audio/Video message content
         #      if URL exists, means file data was uploaded to a CDN,
         #          1. save password as 'content.key';
@@ -158,15 +158,15 @@
             |          |      |          |
             | data     |      | data     |
             | key/keys |      | key/keys |
             +----------+      | signature|  1. signature = sign(data, sender.SK)
                               +----------+
     """
 
-    def sign_message(self, msg: SecureMessage) -> ReliableMessage:
+    async def sign_message(self, msg: SecureMessage) -> ReliableMessage:
         """
         Sign message.data, add 'signature' field
 
         :param msg: encrypted message
         :return: ReliableMessage object
         """
         transceiver = self.delegate
@@ -175,15 +175,15 @@
         #
         ciphertext = msg.data
         assert len(ciphertext) > 0, 'failed to decode message data: %s => %s, %s'\
                                     % (msg.sender, msg.receiver, msg.group)
         #
         #   1. Sign 'message.data' with sender's private key
         #
-        signature = transceiver.sign_data(data=ciphertext, msg=msg)
+        signature = await transceiver.sign_data(data=ciphertext, msg=msg)
         assert len(signature) > 0, 'failed to sign message: %d byte(s) %s => %s, %s'\
                                    % (len(ciphertext), msg.sender, msg.receiver, msg.group)
         #
         #   2. Encode 'message.signature' to String (Base64)
         #
         base64 = TransportableData.encode(data=signature)
         assert base64 is not None, 'failed to encode signature: %d byte(s) %s => %s, %s'\
```

### Comparing `dimsdk-1.0.3/dimsdk/packer.py` & `dimsdk-2.0.0/dimsdk/packer.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         return self.__reliablePacker
 
     #
     #   InstantMessage -> SecureMessage -> ReliableMessage -> Data
     #
 
     # Override
-    def encrypt_message(self, msg: InstantMessage) -> Optional[SecureMessage]:
+    async def encrypt_message(self, msg: InstantMessage) -> Optional[SecureMessage]:
         # TODO: check receiver before calling this, make sure the visa.key exists;
         #       otherwise, suspend this message for waiting receiver's visa/meta;
         #       if receiver is a group, query all members' visa too!
 
         # NOTICE: before sending group message, you can decide whether expose the group ID
         #       (A) if you don't want to expose the group ID,
         #           you can split it to multi-messages before encrypting,
@@ -96,60 +96,60 @@
         #           to encrypt the message, and the remote packer can get the overt group ID before
         #           decrypting to take the right message key.
         receiver = msg.receiver
 
         #
         #   1. get message key with direction (sender -> receiver) or (sender -> group)
         #
-        password = self.messenger.get_encrypt_key(msg=msg)
+        password = await self.messenger.get_encrypt_key(msg=msg)
         assert password is not None, 'failed to get msg key: %s => %s, %s' % (msg.sender, receiver, msg.get('group'))
 
         #
         #   2. encrypt 'content' to 'data' for receiver/group members
         #
         if receiver.is_group:
             # group message
-            members = self.facebook.members(identifier=receiver)
+            members = await self.facebook.get_members(identifier=receiver)
             assert len(members) > 0, 'group not ready: %s' % receiver
             # a station will never send group message, so here must be a client;
             # the client messenger should check the group's meta & members before encrypting,
             # so we can trust that the group members MUST exist here.
-            s_msg = self.instant_packer.encrypt_message(msg=msg, password=password, members=members)
+            s_msg = await self.instant_packer.encrypt_message(msg=msg, password=password, members=members)
         else:
             # personal message (or split group message)
-            s_msg = self.instant_packer.encrypt_message(msg=msg, password=password)
+            s_msg = await self.instant_packer.encrypt_message(msg=msg, password=password)
         if s_msg is None:
             # public key for encryption not found
             # TODO: suspend this message for waiting receiver's meta
             # assert False, 'failed to encrypt message: %s' % msg
             return None
 
         # NOTICE: copy content type to envelope
         #         this help the intermediate nodes to recognize message type
         s_msg.envelope.type = msg.content.type
 
         # OK
         return s_msg
 
     # Override
-    def sign_message(self, msg: SecureMessage) -> ReliableMessage:
+    async def sign_message(self, msg: SecureMessage) -> ReliableMessage:
         assert len(msg.data) > 0, 'message data cannot be empty: %s' % msg
         # sign 'data' by sender
-        return self.secure_packer.sign_message(msg=msg)
+        return await self.secure_packer.sign_message(msg=msg)
 
     # Override
-    def serialize_message(self, msg: ReliableMessage) -> bytes:
+    async def serialize_message(self, msg: ReliableMessage) -> bytes:
         js = json_encode(obj=msg.dictionary)
         return utf8_encode(string=js)
 
     #
     #   Data -> ReliableMessage -> SecureMessage -> InstantMessage
     #
 
-    def deserialize_message(self, data: bytes) -> Optional[ReliableMessage]:
+    async def deserialize_message(self, data: bytes) -> Optional[ReliableMessage]:
         js = utf8_decode(data=data)
         if js is None:
             # assert False, 'message data error: %d' % len(data)
             return None
         dictionary = json_decode(string=js)
         # TODO: translate short keys
         #       'S' -> 'sender'
@@ -162,48 +162,48 @@
         #       'V' -> 'signature'
         #       'K' -> 'key'
         #       ------------------
         #       'M' -> 'meta'
         #       'P' -> 'visa'
         return ReliableMessage.parse(msg=dictionary)
 
-    def _check_attachments(self, msg: ReliableMessage) -> bool:
+    async def _check_attachments(self, msg: ReliableMessage) -> bool:
         """ Check meta & visa """
         sender = msg.sender
         # [Meta Protocol]
         meta = MessageHelper.get_meta(msg=msg)
         if meta is not None:
-            self.facebook.save_meta(meta=meta, identifier=sender)
+            await self.facebook.save_meta(meta=meta, identifier=sender)
         # [Visa Protocol]
         visa = MessageHelper.get_visa(msg=msg)
         if visa is not None:
-            self.facebook.save_document(document=visa)
+            await self.facebook.save_document(document=visa)
         #
         # NOTICE: check [Visa Protocol] before calling this
         #         make sure the sender's meta(visa) exists
         #         (do it by application)
         #
         return True
 
-    def verify_message(self, msg: ReliableMessage) -> Optional[SecureMessage]:
+    async def verify_message(self, msg: ReliableMessage) -> Optional[SecureMessage]:
         # make sure sender's meta exists before verifying message
-        if not self._check_attachments(msg=msg):
+        if not await self._check_attachments(msg=msg):
             return None
         assert len(msg.signature) > 0, 'message signature cannot be empty: %s' % msg
         # verify 'data' with 'signature'
-        return self.reliable_packer.verify_message(msg=msg)
+        return await self.reliable_packer.verify_message(msg=msg)
 
-    def decrypt_message(self, msg: SecureMessage) -> Optional[InstantMessage]:
+    async def decrypt_message(self, msg: SecureMessage) -> Optional[InstantMessage]:
         # TODO: check receiver before calling this, make sure you are the receiver,
         #       or you are a member of the group when this is a group message,
         #       so that you will have a private key (decrypt key) to decrypt it.
         facebook = self.facebook
         receiver = msg.receiver
-        user = facebook.select_user(receiver=receiver)
+        user = await facebook.select_user(receiver=receiver)
         if user is None:
             # not for you?
             raise LookupError('receiver error: %s, from %s, %s' % (receiver, msg.sender, msg.group))
         assert len(msg.data) > 0, 'message data empty: %s => %s, %s' % (msg.sender, msg.receiver, msg.group)
         # decrypt 'data' to 'content'
-        return self.secure_packer.decrypt_message(msg=msg, receiver=user.identifier)
+        return await self.secure_packer.decrypt_message(msg=msg, receiver=user.identifier)
         # TODO: check top-secret message
         #       (do it by application)
```

### Comparing `dimsdk-1.0.3/dimsdk/processor.py` & `dimsdk-2.0.0/dimsdk/processor.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,92 +84,92 @@
         return self.__factory.get_command_processor(msg_type, cmd=cmd)
 
     #
     #  Processing Message
     #
 
     # Override
-    def process_package(self, data: bytes) -> List[bytes]:
+    async def process_package(self, data: bytes) -> List[bytes]:
         messenger = self.messenger
         # 1. deserialize message
-        msg = messenger.deserialize_message(data=data)
+        msg = await messenger.deserialize_message(data=data)
         if msg is None:
             # no valid message received
             return []
         # 2. process message
-        responses = messenger.process_reliable_message(msg=msg)
+        responses = await messenger.process_reliable_message(msg=msg)
         if len(responses) == 0:
             # nothing to respond
             return []
         # 3. serialize messages
         packages = []
         for res in responses:
-            pack = messenger.serialize_message(msg=res)
+            pack = await messenger.serialize_message(msg=res)
             if pack is not None:
                 packages.append(pack)
         return packages
 
     # Override
-    def process_reliable_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
+    async def process_reliable_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
         # TODO: override to check broadcast message before calling it
         messenger = self.messenger
         # 1. verify message
-        s_msg = messenger.verify_message(msg=msg)
+        s_msg = await messenger.verify_message(msg=msg)
         if s_msg is None:
             # TODO: suspend and waiting for sender's meta if not exists
             return []
         # 2. process message
-        responses = messenger.process_secure_message(msg=s_msg, r_msg=msg)
+        responses = await messenger.process_secure_message(msg=s_msg, r_msg=msg)
         if len(responses) == 0:
             # nothing to respond
             return []
         # 3. sign message
         messages = []
         for res in responses:
-            signed = messenger.sign_message(msg=res)
+            signed = await messenger.sign_message(msg=res)
             if signed is not None:
                 messages.append(signed)
         return messages
         # TODO: override to deliver to the receiver when catch exception "receiver error ..."
 
     # Override
-    def process_secure_message(self, msg: SecureMessage, r_msg: ReliableMessage) -> List[SecureMessage]:
+    async def process_secure_message(self, msg: SecureMessage, r_msg: ReliableMessage) -> List[SecureMessage]:
         messenger = self.messenger
         # 1. decrypt message
-        i_msg = messenger.decrypt_message(msg=msg)
+        i_msg = await messenger.decrypt_message(msg=msg)
         if i_msg is None:
             # cannot decrypt this message, not for you?
             # delivering message to other receiver?
             return []
         # 2. process message
-        responses = messenger.process_instant_message(msg=i_msg, r_msg=r_msg)
+        responses = await messenger.process_instant_message(msg=i_msg, r_msg=r_msg)
         if len(responses) == 0:
             # nothing to respond
             return []
         # 3. encrypt messages
         messages = []
         for res in responses:
-            encrypted = messenger.encrypt_message(msg=res)
+            encrypted = await messenger.encrypt_message(msg=res)
             if encrypted is not None:
                 messages.append(encrypted)
         return messages
 
     # Override
-    def process_instant_message(self, msg: InstantMessage, r_msg: ReliableMessage) -> List[InstantMessage]:
+    async def process_instant_message(self, msg: InstantMessage, r_msg: ReliableMessage) -> List[InstantMessage]:
         messenger = self.messenger
         # 1. process content from sender
-        responses = messenger.process_content(content=msg.content, r_msg=r_msg)
+        responses = await messenger.process_content(content=msg.content, r_msg=r_msg)
         if len(responses) == 0:
             # nothing to respond
             return []
         # 2. select a local user to build message
         sender = msg.sender
         receiver = msg.receiver
         facebook = self.facebook
-        user = facebook.select_user(receiver=receiver)
+        user = await facebook.select_user(receiver=receiver)
         if user is None:
             # assert False, 'receiver error: %s' % receiver
             return []
         me = user.identifier
         # 3. package messages
         messages = []
         for res in responses:
@@ -177,16 +177,16 @@
             env = Envelope.create(sender=me, receiver=sender)
             msg = InstantMessage.create(head=env, body=res)
             assert msg is not None, 'should not happen'
             messages.append(msg)
         return messages
 
     # Override
-    def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
+    async def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
         # TODO: override to check group
         cpu = self.get_processor(content=content)
         if cpu is None:
             # default content processor
             cpu = self.get_content_processor(0)
             assert cpu is not None, 'default CPU not defined'
-        return cpu.process_content(content=content, r_msg=r_msg)
+        return await cpu.process_content(content=content, r_msg=r_msg)
         # TODO: override to filter the response
```

### Comparing `dimsdk-1.0.3/dimsdk/utils/__init__.py` & `dimsdk-2.0.0/dimsdk/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dimsdk-1.0.3/dimsdk/utils/checker.py` & `dimsdk-2.0.0/dimsdk/utils/checker.py`

 * *Files identical despite different names*

### Comparing `dimsdk-1.0.3/dimsdk.egg-info/PKG-INFO` & `dimsdk-2.0.0/dimsdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimsdk
-Version: 1.0.3
+Version: 2.0.0
 Summary: Decentralized Instant Messaging SDK
 Home-page: https://github.com/dimchat/sdk-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # Decentralized Instant Messaging (Python SDK)
```

### Comparing `dimsdk-1.0.3/dimsdk.egg-info/SOURCES.txt` & `dimsdk-2.0.0/dimsdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dimsdk-1.0.3/setup.py` & `dimsdk-2.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     communications between accounts safely by end-to-end encryption.
 """
 
 import io
 
 from setuptools import setup, find_packages
 
-__version__ = '1.0.3'
+__version__ = '2.0.0'
 __author__ = 'Albert Moky'
 __contact__ = 'albert.moky@gmail.com'
 
 with io.open('README.md', 'r', encoding='utf-8') as fh:
     readme = fh.read()
 
 setup(
@@ -37,12 +37,12 @@
     },
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     install_requires=[
-        'dimp>=1.0.3',
-        'dkd>=1.0.2',
-        'mkm>=1.0.2',
+        'dimp>=2.0.0',
+        'dkd>=2.0.0',
+        'mkm>=2.0.0',
     ]
 )
```

