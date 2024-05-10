# Comparing `tmp/edcpy-0.2.0a0.tar.gz` & `tmp/edcpy-0.3.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edcpy-0.2.0a0.tar", max compression
+gzip compressed data, was "edcpy-0.3.0a0.tar", max compression
```

## Comparing `edcpy-0.2.0a0.tar` & `edcpy-0.3.0a0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      113 2024-02-22 13:28:36.210108 edcpy-0.2.0a0/README.md
--rw-r--r--   0        0        0        0 2024-02-22 13:28:36.210108 edcpy-0.2.0a0/edcpy/__init__.py
--rw-r--r--   0        0        0     6135 2024-02-22 13:28:36.210108 edcpy-0.2.0a0/edcpy/backend.py
--rw-r--r--   0        0        0     2442 2024-02-22 13:28:36.210108 edcpy-0.2.0a0/edcpy/config.py
--rw-r--r--   0        0        0    12150 2024-02-22 13:28:36.210108 edcpy-0.2.0a0/edcpy/edc_api.py
--rw-r--r--   0        0        0    10682 2024-02-22 13:28:36.210108 edcpy-0.2.0a0/edcpy/keycloak.py
--rw-r--r--   0        0        0     4247 2024-02-22 13:28:36.210108 edcpy-0.2.0a0/edcpy/messaging.py
--rw-r--r--   0        0        0        0 2024-02-22 13:28:36.210108 edcpy-0.2.0a0/edcpy/models/__init__.py
--rw-r--r--   0        0        0     1621 2024-02-22 13:28:36.210108 edcpy-0.2.0a0/edcpy/models/asset.py
--rw-r--r--   0        0        0      708 2024-02-22 13:28:36.210108 edcpy-0.2.0a0/edcpy/models/contract_definition.py
--rw-r--r--   0        0        0     1198 2024-02-22 13:28:36.210108 edcpy-0.2.0a0/edcpy/models/contract_negotiation.py
--rw-r--r--   0        0        0      835 2024-02-22 13:28:36.210108 edcpy-0.2.0a0/edcpy/models/data_plane_instance.py
--rw-r--r--   0        0        0      645 2024-02-22 13:28:36.210108 edcpy-0.2.0a0/edcpy/models/policy_definition.py
--rw-r--r--   0        0        0     1948 2024-02-22 13:28:36.210108 edcpy-0.2.0a0/edcpy/models/transfer_process.py
--rw-r--r--   0        0        0      245 2024-02-22 13:28:36.210108 edcpy-0.2.0a0/edcpy/utils.py
--rw-r--r--   0        0        0      975 2024-02-22 13:28:36.214108 edcpy-0.2.0a0/pyproject.toml
--rw-r--r--   0        0        0     1256 1970-01-01 00:00:00.000000 edcpy-0.2.0a0/PKG-INFO
+-rw-r--r--   0        0        0      113 2024-05-10 12:05:57.779535 edcpy-0.3.0a0/README.md
+-rw-r--r--   0        0        0        0 2024-05-10 12:05:57.779535 edcpy-0.3.0a0/edcpy/__init__.py
+-rw-r--r--   0        0        0     6135 2024-05-10 12:05:57.779535 edcpy-0.3.0a0/edcpy/backend.py
+-rw-r--r--   0        0        0     2442 2024-05-10 12:05:57.779535 edcpy-0.3.0a0/edcpy/config.py
+-rw-r--r--   0        0        0    12027 2024-05-10 12:05:57.779535 edcpy-0.3.0a0/edcpy/edc_api.py
+-rw-r--r--   0        0        0    10682 2024-05-10 12:05:57.779535 edcpy-0.3.0a0/edcpy/keycloak.py
+-rw-r--r--   0        0        0     4247 2024-05-10 12:05:57.779535 edcpy-0.3.0a0/edcpy/messaging.py
+-rw-r--r--   0        0        0        0 2024-05-10 12:05:57.779535 edcpy-0.3.0a0/edcpy/models/__init__.py
+-rw-r--r--   0        0        0     1621 2024-05-10 12:05:57.779535 edcpy-0.3.0a0/edcpy/models/asset.py
+-rw-r--r--   0        0        0      708 2024-05-10 12:05:57.779535 edcpy-0.3.0a0/edcpy/models/contract_definition.py
+-rw-r--r--   0        0        0     1035 2024-05-10 12:05:57.779535 edcpy-0.3.0a0/edcpy/models/contract_negotiation.py
+-rw-r--r--   0        0        0      835 2024-05-10 12:05:57.779535 edcpy-0.3.0a0/edcpy/models/data_plane_instance.py
+-rw-r--r--   0        0        0      645 2024-05-10 12:05:57.779535 edcpy-0.3.0a0/edcpy/models/policy_definition.py
+-rw-r--r--   0        0        0     1948 2024-05-10 12:05:57.779535 edcpy-0.3.0a0/edcpy/models/transfer_process.py
+-rw-r--r--   0        0        0      245 2024-05-10 12:05:57.779535 edcpy-0.3.0a0/edcpy/utils.py
+-rw-r--r--   0        0        0      975 2024-05-10 12:05:57.783535 edcpy-0.3.0a0/pyproject.toml
+-rw-r--r--   0        0        0     1256 1970-01-01 00:00:00.000000 edcpy-0.3.0a0/PKG-INFO
```

### Comparing `edcpy-0.2.0a0/edcpy/backend.py` & `edcpy-0.3.0a0/edcpy/backend.py`

 * *Files identical despite different names*

### Comparing `edcpy-0.2.0a0/edcpy/config.py` & `edcpy-0.3.0a0/edcpy/config.py`

 * *Files identical despite different names*

### Comparing `edcpy-0.2.0a0/edcpy/edc_api.py` & `edcpy-0.3.0a0/edcpy/edc_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -262,15 +262,15 @@
 
     @property
     def default_contract_offer_id(self) -> str:
         return self.default_policy["@id"]
 
     @property
     def default_asset_id(self) -> str:
-        return self.default_policy["odrl:target"]["@id"]
+        return self.data["@id"]
 
 
 @dataclass
 class TransferProcessDetails:
     asset_id: str
     contract_agreement_id: str
     counter_party_protocol_url: str
@@ -312,27 +312,25 @@
         dataset_dict = catalog_content.find_one_dataset(asset_query)
 
         if not dataset_dict:
             raise ValueError(f"Dataset not found for query: {asset_query}")
 
         _logger.debug("Selected dataset:\n%s", pprint.pformat(dataset_dict))
         dataset = CatalogDataset(data=dataset_dict)
-        contract_offer_id = dataset.default_contract_offer_id
-        _logger.debug("Contract Offer ID: %s", contract_offer_id)
         asset_id = dataset.default_asset_id
-        _logger.debug("Asset ID: %s", asset_id)
+        _logger.info("Creating contract negotiation for Asset ID: %s", asset_id)
+
+        # The contract offer needs to be equal to the provider's offer as per the EDC docs
 
         contract_negotiation = await create_contract_negotiation(
             management_url=self.connector_urls.management_url,
             counter_party_connector_id=counter_party_connector_id,
             counter_party_protocol_url=counter_party_protocol_url,
-            consumer_id=self.config.connector.participant_id,
-            provider_id=counter_party_connector_id,
-            offer_id=contract_offer_id,
-            asset_id=asset_id,
+            asset_id=dataset.default_asset_id,
+            policy=dataset.default_policy,
         )
 
         contract_negotiation_id = contract_negotiation["@id"]
         _logger.debug("Contract Negotiation ID: %s", contract_negotiation_id)
 
         contract_agreement_id = await wait_for_contract_negotiation(
             management_url=self.connector_urls.management_url,
```

### Comparing `edcpy-0.2.0a0/edcpy/keycloak.py` & `edcpy-0.3.0a0/edcpy/keycloak.py`

 * *Files identical despite different names*

### Comparing `edcpy-0.2.0a0/edcpy/messaging.py` & `edcpy-0.3.0a0/edcpy/messaging.py`

 * *Files identical despite different names*

### Comparing `edcpy-0.2.0a0/edcpy/models/asset.py` & `edcpy-0.3.0a0/edcpy/models/asset.py`

 * *Files identical despite different names*

### Comparing `edcpy-0.2.0a0/edcpy/models/contract_definition.py` & `edcpy-0.3.0a0/edcpy/models/contract_definition.py`

 * *Files identical despite different names*

### Comparing `edcpy-0.2.0a0/edcpy/models/data_plane_instance.py` & `edcpy-0.3.0a0/edcpy/models/data_plane_instance.py`

 * *Files identical despite different names*

### Comparing `edcpy-0.2.0a0/edcpy/models/policy_definition.py` & `edcpy-0.3.0a0/edcpy/models/policy_definition.py`

 * *Files identical despite different names*

### Comparing `edcpy-0.2.0a0/edcpy/models/transfer_process.py` & `edcpy-0.3.0a0/edcpy/models/transfer_process.py`

 * *Files identical despite different names*

### Comparing `edcpy-0.2.0a0/pyproject.toml` & `edcpy-0.3.0a0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edcpy"
-version = "0.2.0a0"
+version = "0.3.0a0"
 description = "Package that provides a series of utilities to facilitate interaction with the Management and Control APIs of an EDC connector"
 authors = ["Andres Garcia Mangas <andres.garcia@fundacionctic.org>"]
 license = "EUPL-1.2"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `edcpy-0.2.0a0/PKG-INFO` & `edcpy-0.3.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edcpy
-Version: 0.2.0a0
+Version: 0.3.0a0
 Summary: Package that provides a series of utilities to facilitate interaction with the Management and Control APIs of an EDC connector
 License: EUPL-1.2
 Author: Andres Garcia Mangas
 Author-email: andres.garcia@fundacionctic.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Programming Language :: Python :: 3
```

