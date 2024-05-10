# Comparing `tmp/telq-1.3.1.tar.gz` & `tmp/telq-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telq-1.3.1.tar", max compression
+gzip compressed data, was "telq-1.3.2.tar", max compression
```

## Comparing `telq-1.3.1.tar` & `telq-1.3.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11345 2024-05-08 12:17:51.315054 telq-1.3.1/LICENSE
--rwxr-xr-x   0        0        0      461 2024-05-08 12:17:51.315054 telq-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     6148 2024-05-08 12:17:51.315054 telq-1.3.1/telq/.DS_Store
--rwxr-xr-x   0        0        0     6325 2024-05-08 12:17:51.315054 telq-1.3.1/telq/__init__.py
--rwxr-xr-x   0        0        0     3026 2024-05-08 12:17:51.315054 telq-1.3.1/telq/authentication/__init__.py
--rwxr-xr-x   0        0        0     4481 2024-05-08 12:17:51.315054 telq-1.3.1/telq/endpoints/__init__.py
--rwxr-xr-x   0        0        0     2004 2024-05-08 12:17:51.315054 telq-1.3.1/telq/networks/__init__.py
--rwxr-xr-x   0        0        0     5066 2024-05-08 12:17:51.319054 telq-1.3.1/telq/session/__init__.py
--rw-r--r--   0        0        0     1685 2024-05-08 12:17:51.319054 telq-1.3.1/telq/session/session_data.py
--rwxr-xr-x   0        0        0     6376 2024-05-08 12:17:51.319054 telq-1.3.1/telq/supplier/__init__.py
--rw-r--r--   0        0        0     1514 2024-05-08 12:17:51.319054 telq-1.3.1/telq/supplier/supplier_data.py
--rwxr-xr-x   0        0        0       94 2024-05-08 12:17:51.319054 telq-1.3.1/telq/tests/__init__.py
--rwxr-xr-x   0        0        0     7267 2024-05-08 12:17:51.319054 telq-1.3.1/telq/tests/lnt.py
--rw-r--r--   0        0        0      277 2024-05-08 12:17:51.319054 telq-1.3.1/telq/tests/model.py
--rwxr-xr-x   0        0        0     5051 2024-05-08 12:17:51.319054 telq-1.3.1/telq/tests/mt.py
--rw-r--r--   0        0        0     1369 2024-05-08 12:17:51.319054 telq-1.3.1/telq/util/rest.py
--rw-r--r--   0        0        0       20 2024-05-08 12:17:51.319054 telq-1.3.1/telq/util/version.py
--rw-r--r--   0        0        0      709 1970-01-01 00:00:00.000000 telq-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11345 2024-05-10 07:58:38.432867 telq-1.3.2/LICENSE
+-rwxr-xr-x   0        0        0      461 2024-05-10 07:58:38.432867 telq-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     6148 2024-05-10 07:58:38.432867 telq-1.3.2/telq/.DS_Store
+-rwxr-xr-x   0        0        0     6325 2024-05-10 07:58:38.432867 telq-1.3.2/telq/__init__.py
+-rwxr-xr-x   0        0        0     3026 2024-05-10 07:58:38.432867 telq-1.3.2/telq/authentication/__init__.py
+-rwxr-xr-x   0        0        0     4479 2024-05-10 07:58:38.432867 telq-1.3.2/telq/endpoints/__init__.py
+-rwxr-xr-x   0        0        0     2004 2024-05-10 07:58:38.432867 telq-1.3.2/telq/networks/__init__.py
+-rwxr-xr-x   0        0        0     5066 2024-05-10 07:58:38.432867 telq-1.3.2/telq/session/__init__.py
+-rw-r--r--   0        0        0     1685 2024-05-10 07:58:38.432867 telq-1.3.2/telq/session/session_data.py
+-rwxr-xr-x   0        0        0     6376 2024-05-10 07:58:38.432867 telq-1.3.2/telq/supplier/__init__.py
+-rw-r--r--   0        0        0     1514 2024-05-10 07:58:38.432867 telq-1.3.2/telq/supplier/supplier_data.py
+-rwxr-xr-x   0        0        0       94 2024-05-10 07:58:38.432867 telq-1.3.2/telq/tests/__init__.py
+-rwxr-xr-x   0        0        0     7267 2024-05-10 07:58:38.432867 telq-1.3.2/telq/tests/lnt.py
+-rw-r--r--   0        0        0      277 2024-05-10 07:58:38.432867 telq-1.3.2/telq/tests/model.py
+-rwxr-xr-x   0        0        0     5059 2024-05-10 07:58:38.432867 telq-1.3.2/telq/tests/mt.py
+-rw-r--r--   0        0        0     1369 2024-05-10 07:58:38.432867 telq-1.3.2/telq/util/rest.py
+-rw-r--r--   0        0        0       20 2024-05-10 07:58:38.432867 telq-1.3.2/telq/util/version.py
+-rw-r--r--   0        0        0      709 1970-01-01 00:00:00.000000 telq-1.3.2/PKG-INFO
```

### Comparing `telq-1.3.1/LICENSE` & `telq-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `telq-1.3.1/telq/.DS_Store` & `telq-1.3.2/telq/.DS_Store`

 * *Files identical despite different names*

### Comparing `telq-1.3.1/telq/__init__.py` & `telq-1.3.2/telq/__init__.py`

 * *Files identical despite different names*

### Comparing `telq-1.3.1/telq/authentication/__init__.py` & `telq-1.3.2/telq/authentication/__init__.py`

 * *Files identical despite different names*

### Comparing `telq-1.3.1/telq/endpoints/__init__.py` & `telq-1.3.2/telq/endpoints/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         return "/lnt/tests"
 
 
 class ResultsURL(TelQURL):
     """Endpoint for results"""
 
     def path(self, test_id) -> str:
-        return f"/results/{test_id}"
+        return f"/tests/{test_id}"
 
 
 class BatchResultsURL(TelQURL):
     """Endpoint for batch results"""
     def url(self, date_from: Optional[str], date_to: Optional[str], page: int = 1, size: int = 100, order: str = "asc") -> str:
         query_params = {
             "page": page,
```

### Comparing `telq-1.3.1/telq/networks/__init__.py` & `telq-1.3.2/telq/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `telq-1.3.1/telq/session/__init__.py` & `telq-1.3.2/telq/session/__init__.py`

 * *Files identical despite different names*

### Comparing `telq-1.3.1/telq/session/session_data.py` & `telq-1.3.2/telq/session/session_data.py`

 * *Files identical despite different names*

### Comparing `telq-1.3.1/telq/supplier/__init__.py` & `telq-1.3.2/telq/supplier/__init__.py`

 * *Files identical despite different names*

### Comparing `telq-1.3.1/telq/supplier/supplier_data.py` & `telq-1.3.2/telq/supplier/supplier_data.py`

 * *Files identical despite different names*

### Comparing `telq-1.3.1/telq/tests/lnt.py` & `telq-1.3.2/telq/tests/lnt.py`

 * *Files identical despite different names*

### Comparing `telq-1.3.1/telq/tests/mt.py` & `telq-1.3.2/telq/tests/mt.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         destinationNetworks: List[Dict[str, str]],
         resultsCallbackUrl: Union[str, None] = None,
         maxCallbackRetries: int = 3,
         testIdTextType: str = "ALPHA",
         testIdTextCase: str = "MIXED",
         testIdTextLength: int = 10,
         testTimeToLiveInSeconds: int = 3600,
-    ):
+    ) -> Dict:
         """Initiate a new test
 
         Parameters
         ----------
         destinationNetworks : List[Dict[str, str]]
             The list of networks you want to issue tests to. This is required and cannot be empty.
             Each network are required to have at least the mcc and mc as keys. optional are portedFromMnc
```

### Comparing `telq-1.3.1/telq/util/rest.py` & `telq-1.3.2/telq/util/rest.py`

 * *Files identical despite different names*

### Comparing `telq-1.3.1/PKG-INFO` & `telq-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telq
-Version: 1.3.1
+Version: 1.3.2
 Summary: Python SDK for TelQ Telecom API
 Author: Tuvshinbayar Davaa
 Author-email: tuvshinbayar.davaa@telqtele.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

