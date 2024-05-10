# Comparing `tmp/original_sdk-1.3.0.tar.gz` & `tmp/original_sdk-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "original_sdk-1.3.0.tar", last modified: Tue Apr  2 13:56:54 2024, max compression
+gzip compressed data, was "original_sdk-1.3.1.tar", last modified: Fri May 10 15:21:40 2024, max compression
```

## Comparing `original_sdk-1.3.0.tar` & `original_sdk-1.3.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:56:54.485653 original_sdk-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-02 13:56:46.000000 original_sdk-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-02 13:56:46.000000 original_sdk-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    25065 2024-04-02 13:56:54.481653 original_sdk-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    24117 2024-04-02 13:56:46.000000 original_sdk-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:56:54.481653 original_sdk-1.3.0/original_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-02 13:56:46.000000 original_sdk-1.3.0/original_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-02 13:56:46.000000 original_sdk-1.3.0/original_sdk/__pkg__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8647 2024-04-02 13:56:46.000000 original_sdk-1.3.0/original_sdk/async_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:56:54.481653 original_sdk-1.3.0/original_sdk/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:56:46.000000 original_sdk-1.3.0/original_sdk/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9723 2024-04-02 13:56:46.000000 original_sdk-1.3.0/original_sdk/base/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-04-02 13:56:46.000000 original_sdk-1.3.0/original_sdk/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:56:54.481653 original_sdk-1.3.0/original_sdk/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:56:46.000000 original_sdk-1.3.0/original_sdk/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-02 13:56:46.000000 original_sdk-1.3.0/original_sdk/types/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-02 13:56:46.000000 original_sdk-1.3.0/original_sdk/types/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-04-02 13:56:46.000000 original_sdk-1.3.0/original_sdk/types/original_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-02 13:56:46.000000 original_sdk-1.3.0/original_sdk/types/rate_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-02 13:56:46.000000 original_sdk-1.3.0/original_sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:56:54.481653 original_sdk-1.3.0/original_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    25065 2024-04-02 13:56:54.000000 original_sdk-1.3.0/original_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-02 13:56:54.000000 original_sdk-1.3.0/original_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 13:56:54.000000 original_sdk-1.3.0/original_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 13:56:54.000000 original_sdk-1.3.0/original_sdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-02 13:56:54.000000 original_sdk-1.3.0/original_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-02 13:56:54.000000 original_sdk-1.3.0/original_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-02 13:56:46.000000 original_sdk-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 13:56:54.485653 original_sdk-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-02 13:56:46.000000 original_sdk-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:21:40.647016 original_sdk-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-10 15:21:32.000000 original_sdk-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-10 15:21:32.000000 original_sdk-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    25099 2024-05-10 15:21:40.647016 original_sdk-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24151 2024-05-10 15:21:32.000000 original_sdk-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:21:40.647016 original_sdk-1.3.1/original_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-10 15:21:32.000000 original_sdk-1.3.1/original_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-10 15:21:32.000000 original_sdk-1.3.1/original_sdk/__pkg__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8647 2024-05-10 15:21:32.000000 original_sdk-1.3.1/original_sdk/async_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:21:40.647016 original_sdk-1.3.1/original_sdk/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 15:21:32.000000 original_sdk-1.3.1/original_sdk/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9723 2024-05-10 15:21:32.000000 original_sdk-1.3.1/original_sdk/base/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-05-10 15:21:32.000000 original_sdk-1.3.1/original_sdk/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:21:40.647016 original_sdk-1.3.1/original_sdk/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 15:21:32.000000 original_sdk-1.3.1/original_sdk/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-10 15:21:32.000000 original_sdk-1.3.1/original_sdk/types/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-10 15:21:32.000000 original_sdk-1.3.1/original_sdk/types/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-10 15:21:32.000000 original_sdk-1.3.1/original_sdk/types/original_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-10 15:21:32.000000 original_sdk-1.3.1/original_sdk/types/rate_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-10 15:21:32.000000 original_sdk-1.3.1/original_sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:21:40.647016 original_sdk-1.3.1/original_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    25099 2024-05-10 15:21:40.000000 original_sdk-1.3.1/original_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-10 15:21:40.000000 original_sdk-1.3.1/original_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 15:21:40.000000 original_sdk-1.3.1/original_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 15:21:40.000000 original_sdk-1.3.1/original_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-10 15:21:40.000000 original_sdk-1.3.1/original_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-10 15:21:40.000000 original_sdk-1.3.1/original_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-10 15:21:32.000000 original_sdk-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 15:21:40.647016 original_sdk-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-10 15:21:32.000000 original_sdk-1.3.1/setup.py
```

### Comparing `original_sdk-1.3.0/LICENSE` & `original_sdk-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `original_sdk-1.3.0/PKG-INFO` & `original_sdk-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: original_sdk
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python client for Original.
 Home-page: https://github.com/GetOriginal/original-python
 Author: Alexander Turowicz
 Author-email: support@getoriginal.com
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
@@ -223,14 +223,15 @@
 
 ```python
 # prepare the new asset params
 new_asset_params = {
     "user_uid": "324167489835",
     "asset_external_id": "asset_external_id_1",
     "collection_uid": "221137489875",
+    "sale_price_in_usd": 9.99,
     "data": {
         "name": "Dave Starbelly",
         "unique_name": True,
         "image_url": "https://storage.googleapis.com/opensea-prod.appspot.com/puffs/3.png",
         "store_image_on_ipfs": True,
         "description": "Friendly OpenSea Creature that enjoys long swims in the ocean.",
         "external_url": "https://openseacreatures.io/3",
@@ -580,15 +581,15 @@
 ### Create a new allocation
 ```python
 
 # Prepare the allocation parameters
 allocation_params = {
     "amount": 123.123,
     "nonce": "nonce1",
-    "user_uid": "483581848722",
+    "to_user_uid": "483581848722",
     "reward_uid": "708469717542",
 }
 
 # Create an allocation
 allocation_response = client.create_allocation(**allocation_params)
 allocation_uid = allocation_response['data']['uid']
 # Sample allocation_response:
```

### Comparing `original_sdk-1.3.0/README.md` & `original_sdk-1.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -198,14 +198,15 @@
 
 ```python
 # prepare the new asset params
 new_asset_params = {
     "user_uid": "324167489835",
     "asset_external_id": "asset_external_id_1",
     "collection_uid": "221137489875",
+    "sale_price_in_usd": 9.99,
     "data": {
         "name": "Dave Starbelly",
         "unique_name": True,
         "image_url": "https://storage.googleapis.com/opensea-prod.appspot.com/puffs/3.png",
         "store_image_on_ipfs": True,
         "description": "Friendly OpenSea Creature that enjoys long swims in the ocean.",
         "external_url": "https://openseacreatures.io/3",
@@ -555,15 +556,15 @@
 ### Create a new allocation
 ```python
 
 # Prepare the allocation parameters
 allocation_params = {
     "amount": 123.123,
     "nonce": "nonce1",
-    "user_uid": "483581848722",
+    "to_user_uid": "483581848722",
     "reward_uid": "708469717542",
 }
 
 # Create an allocation
 allocation_response = client.create_allocation(**allocation_params)
 allocation_uid = allocation_response['data']['uid']
 # Sample allocation_response:
```

### Comparing `original_sdk-1.3.0/original_sdk/async_client.py` & `original_sdk-1.3.1/original_sdk/async_client.py`

 * *Files identical despite different names*

### Comparing `original_sdk-1.3.0/original_sdk/base/client.py` & `original_sdk-1.3.1/original_sdk/base/client.py`

 * *Files identical despite different names*

### Comparing `original_sdk-1.3.0/original_sdk/client.py` & `original_sdk-1.3.1/original_sdk/client.py`

 * *Files identical despite different names*

### Comparing `original_sdk-1.3.0/original_sdk/types/exceptions.py` & `original_sdk-1.3.1/original_sdk/types/exceptions.py`

 * *Files identical despite different names*

### Comparing `original_sdk-1.3.0/original_sdk/types/original_response.py` & `original_sdk-1.3.1/original_sdk/types/original_response.py`

 * *Files identical despite different names*

### Comparing `original_sdk-1.3.0/original_sdk.egg-info/PKG-INFO` & `original_sdk-1.3.1/original_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: original-sdk
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python client for Original.
 Home-page: https://github.com/GetOriginal/original-python
 Author: Alexander Turowicz
 Author-email: support@getoriginal.com
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
@@ -223,14 +223,15 @@
 
 ```python
 # prepare the new asset params
 new_asset_params = {
     "user_uid": "324167489835",
     "asset_external_id": "asset_external_id_1",
     "collection_uid": "221137489875",
+    "sale_price_in_usd": 9.99,
     "data": {
         "name": "Dave Starbelly",
         "unique_name": True,
         "image_url": "https://storage.googleapis.com/opensea-prod.appspot.com/puffs/3.png",
         "store_image_on_ipfs": True,
         "description": "Friendly OpenSea Creature that enjoys long swims in the ocean.",
         "external_url": "https://openseacreatures.io/3",
@@ -580,15 +581,15 @@
 ### Create a new allocation
 ```python
 
 # Prepare the allocation parameters
 allocation_params = {
     "amount": 123.123,
     "nonce": "nonce1",
-    "user_uid": "483581848722",
+    "to_user_uid": "483581848722",
     "reward_uid": "708469717542",
 }
 
 # Create an allocation
 allocation_response = client.create_allocation(**allocation_params)
 allocation_uid = allocation_response['data']['uid']
 # Sample allocation_response:
```

### Comparing `original_sdk-1.3.0/original_sdk.egg-info/SOURCES.txt` & `original_sdk-1.3.1/original_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `original_sdk-1.3.0/pyproject.toml` & `original_sdk-1.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `original_sdk-1.3.0/setup.py` & `original_sdk-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "requests>=2.22.0,<3",
     "aiodns>=2.0.0",
     "aiohttp>=3.6.0,<4",
     "aiofile>=3.1,<4",
     "pyjwt>=2.0.0,<3",
     "typing_extensions; python_version < '3.8'",
 ]
-tests_require = ["pytest", "pytest-asyncio<=0.21.1", "python-dotenv"]
+tests_require = ["pytest<=8.1.1", "pytest-asyncio<=0.21.1", "python-dotenv"]
 ci_require = [
     "black",
     "flake8",
     "flake8-isort",
     "flake8-bugbear",
     "pytest-cov",
     "mypy",
```

