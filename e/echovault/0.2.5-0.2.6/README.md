# Comparing `tmp/echovault-0.2.5.tar.gz` & `tmp/echovault-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echovault-0.2.5.tar", max compression
+gzip compressed data, was "echovault-0.2.6.tar", max compression
```

## Comparing `echovault-0.2.5.tar` & `echovault-0.2.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1075 2024-04-19 19:04:53.372948 echovault-0.2.5/README.md
--rw-r--r--   0        0        0       34 2024-04-25 18:14:25.800920 echovault-0.2.5/echovault/__init__.py
--rw-r--r--   0        0        0        0 2024-04-14 05:54:15.655547 echovault-0.2.5/echovault/__init__.py~
--rw-r--r--   0        0        0     1028 2024-04-28 19:08:59.099761 echovault-0.2.5/echovault/_container.py
--rw-r--r--   0        0        0     1030 2024-04-24 19:49:03.244111 echovault-0.2.5/echovault/_container.py~
--rw-r--r--   0        0        0        0 2024-04-11 19:04:01.114880 echovault-0.2.5/echovault/db.py~
--rw-r--r--   0        0        0     2733 2024-04-30 18:15:33.064347 echovault-0.2.5/echovault/dict.py
--rw-r--r--   0        0        0     2283 2024-04-23 18:43:20.644733 echovault-0.2.5/echovault/dict.py~
--rw-r--r--   0        0        0     2305 2024-04-30 19:41:38.740513 echovault-0.2.5/echovault/list.py
--rw-r--r--   0        0        0     1176 2024-04-24 19:49:34.034385 echovault-0.2.5/echovault/list.py~
--rw-r--r--   0        0        0     2903 2024-04-14 19:48:17.176500 echovault-0.2.5/echovault/table.py~
--rw-r--r--   0        0        0     7210 2024-05-08 19:07:16.968735 echovault-0.2.5/echovault/vault.py
--rw-r--r--   0        0        0     8070 2024-05-05 18:08:25.266920 echovault-0.2.5/echovault/vault.py.bck
--rw-r--r--   0        0        0     1289 2024-04-14 19:18:41.190124 echovault-0.2.5/echovault/vault.py~
--rw-r--r--   0        0        0      380 2024-05-08 19:11:10.643977 echovault-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     1492 1970-01-01 00:00:00.000000 echovault-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-04-19 19:04:53.372948 echovault-0.2.6/README.md
+-rw-r--r--   0        0        0       34 2024-04-25 18:14:25.800920 echovault-0.2.6/echovault/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-14 05:54:15.655547 echovault-0.2.6/echovault/__init__.py~
+-rw-r--r--   0        0        0     1028 2024-04-28 19:08:59.099761 echovault-0.2.6/echovault/_container.py
+-rw-r--r--   0        0        0     1030 2024-04-24 19:49:03.244111 echovault-0.2.6/echovault/_container.py~
+-rw-r--r--   0        0        0        0 2024-04-11 19:04:01.114880 echovault-0.2.6/echovault/db.py~
+-rw-r--r--   0        0        0     2733 2024-04-30 18:15:33.064347 echovault-0.2.6/echovault/dict.py
+-rw-r--r--   0        0        0     2283 2024-04-23 18:43:20.644733 echovault-0.2.6/echovault/dict.py~
+-rw-r--r--   0        0        0     2366 2024-05-10 17:54:28.098196 echovault-0.2.6/echovault/list.py
+-rw-r--r--   0        0        0     1176 2024-04-24 19:49:34.034385 echovault-0.2.6/echovault/list.py~
+-rw-r--r--   0        0        0     2903 2024-04-14 19:48:17.176500 echovault-0.2.6/echovault/table.py~
+-rw-r--r--   0        0        0     7253 2024-05-10 17:53:25.300309 echovault-0.2.6/echovault/vault.py
+-rw-r--r--   0        0        0     8070 2024-05-05 18:08:25.266920 echovault-0.2.6/echovault/vault.py.bck
+-rw-r--r--   0        0        0     1289 2024-04-14 19:18:41.190124 echovault-0.2.6/echovault/vault.py~
+-rw-r--r--   0        0        0      380 2024-05-10 17:57:41.072393 echovault-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     1492 1970-01-01 00:00:00.000000 echovault-0.2.6/PKG-INFO
```

### Comparing `echovault-0.2.5/README.md` & `echovault-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `echovault-0.2.5/echovault/_container.py` & `echovault-0.2.6/echovault/_container.py`

 * *Files identical despite different names*

### Comparing `echovault-0.2.5/echovault/_container.py~` & `echovault-0.2.6/echovault/_container.py~`

 * *Files identical despite different names*

### Comparing `echovault-0.2.5/echovault/dict.py` & `echovault-0.2.6/echovault/dict.py`

 * *Files identical despite different names*

### Comparing `echovault-0.2.5/echovault/dict.py~` & `echovault-0.2.6/echovault/dict.py~`

 * *Files identical despite different names*

### Comparing `echovault-0.2.5/echovault/list.py` & `echovault-0.2.6/echovault/list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from dulwich.objects import Tree, Blob
 from stat import S_IFREG, S_IFDIR
 from uuid import uuid4
 from echovault._container import Container
 from echovault.dict import Dict
 
 class List(Container):
+    Dict = Dict
+    
     def __init__(self, object_store, container, identifier, values=(), *, tree=None):
         super().__init__(object_store, container, identifier, tree)
         self.extend(values)
 
     def __getitem__(self, key):
         _, id_ = self.tree[key]
-        return Dict(self.object_store,
-                    self,
-                    key,
-                    tree=self.object_store[id_])
+        return self.Dict(self.object_store,
+                         self,
+                         key,
+                         tree=self.object_store[id_])
 
         
     def __iter__(self):
         for key in self.tree:
             if key == b'_':
                 continue
             
@@ -30,18 +32,18 @@
     def append(self, value):
         self.extend((value,))
             
     def extend(self, iterable):
         for item in iterable:
             identifier = str(uuid4()).encode('utf-8')
             self.tree[identifier] = S_IFDIR, None
-            entry = Dict(self.object_store,
-                         self,
-                         identifier,
-                         item)
+            entry = self.Dict(self.object_store,
+                              self,
+                              identifier,
+                              item)
 
         self._update()
             
     def remove(self, entry):
         del self.tree[entry.identifier]
         
         self._update()
```

### Comparing `echovault-0.2.5/echovault/list.py~` & `echovault-0.2.6/echovault/list.py~`

 * *Files identical despite different names*

### Comparing `echovault-0.2.5/echovault/table.py~` & `echovault-0.2.6/echovault/table.py~`

 * *Files identical despite different names*

### Comparing `echovault-0.2.5/echovault/vault.py` & `echovault-0.2.6/echovault/vault.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,16 @@
     
     return common_ancestor
 
 class Conflict(Exception):
     pass
 
 class Vault(Container):
+    List = List
+    
     @staticmethod
     def encode(string):
         return string.encode('utf-8')
 
     @staticmethod
     def decode(value):
         return value.decode('utf-8')
@@ -73,23 +75,23 @@
     def ref(self):
         return self._ref[len(ref_head):].decode('utf-8')
             
     def __getitem__(self, name:str):
         identifier = self.encode(name)
         _, oid = self.tree[identifier]
         tree = self.object_store[oid]
-        return List(self.object_store,
-                     self,
-                     identifier,
-                     tree=tree)
+        return self.List(self.object_store,
+                         self,
+                         identifier,
+                         tree=tree)
 
     def __setitem__(self, name:str, iterable):
         identifier = self.encode(name)
         self.tree[identifier] = S_IFDIR, None
-        table = List(self.object_store, self, identifier, iterable)
+        table = self.List(self.object_store, self, identifier, iterable)
         self._update()
 
     def __delitem__(self, name:str):
         del self.tree[self.encode(name)]
         self._update()
 
     def __iter__(self):
```

### Comparing `echovault-0.2.5/echovault/vault.py.bck` & `echovault-0.2.6/echovault/vault.py.bck`

 * *Files identical despite different names*

### Comparing `echovault-0.2.5/echovault/vault.py~` & `echovault-0.2.6/echovault/vault.py~`

 * *Files identical despite different names*

### Comparing `echovault-0.2.5/PKG-INFO` & `echovault-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echovault
-Version: 0.2.5
+Version: 0.2.6
 Summary: echovault is git data storage
 Author: Charles Bajeux
 Author-email: charles.bajeux@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

