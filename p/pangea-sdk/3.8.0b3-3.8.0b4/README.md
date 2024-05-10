# Comparing `tmp/pangea_sdk-3.8.0b3.tar.gz` & `tmp/pangea_sdk-3.8.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pangea_sdk-3.8.0b3.tar", max compression
+gzip compressed data, was "pangea_sdk-3.8.0b4.tar", max compression
```

## Comparing `pangea_sdk-3.8.0b3.tar` & `pangea_sdk-3.8.0b4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     6531 2024-03-25 21:21:53.316793 pangea_sdk-3.8.0b3/README.md
--rw-r--r--   0        0        0      251 2024-03-25 21:21:53.316793 pangea_sdk-3.8.0b3/pangea/__init__.py
--rw-r--r--   0        0        0       45 2024-03-25 21:21:53.316793 pangea_sdk-3.8.0b3/pangea/asyncio/__init__.py
--rw-r--r--   0        0        0     1462 2024-03-25 21:21:53.316793 pangea_sdk-3.8.0b3/pangea/asyncio/file_uploader.py
--rw-r--r--   0        0        0    17272 2024-03-25 21:21:53.316793 pangea_sdk-3.8.0b3/pangea/asyncio/request.py
--rw-r--r--   0        0        0      386 2024-03-25 21:21:53.316793 pangea_sdk-3.8.0b3/pangea/asyncio/services/__init__.py
--rw-r--r--   0        0        0    19594 2024-03-25 21:21:53.317793 pangea_sdk-3.8.0b3/pangea/asyncio/services/audit.py
--rw-r--r--   0        0        0    43812 2024-03-25 21:21:53.317793 pangea_sdk-3.8.0b3/pangea/asyncio/services/authn.py
--rw-r--r--   0        0        0     9958 2024-03-25 21:21:53.317793 pangea_sdk-3.8.0b3/pangea/asyncio/services/authz.py
--rw-r--r--   0        0        0     2663 2024-03-25 21:21:53.317793 pangea_sdk-3.8.0b3/pangea/asyncio/services/base.py
--rw-r--r--   0        0        0     3056 2024-03-25 21:21:53.317793 pangea_sdk-3.8.0b3/pangea/asyncio/services/embargo.py
--rw-r--r--   0        0        0     6301 2024-03-25 21:21:53.317793 pangea_sdk-3.8.0b3/pangea/asyncio/services/file_scan.py
--rw-r--r--   0        0        0    37665 2024-03-25 21:21:53.317793 pangea_sdk-3.8.0b3/pangea/asyncio/services/intel.py
--rw-r--r--   0        0        0     5174 2024-03-25 21:21:53.317793 pangea_sdk-3.8.0b3/pangea/asyncio/services/redact.py
--rw-r--r--   0        0        0     7576 2024-03-25 21:21:53.318793 pangea_sdk-3.8.0b3/pangea/asyncio/services/sanitize.py
--rw-r--r--   0        0        0    24759 2024-03-25 21:21:53.318793 pangea_sdk-3.8.0b3/pangea/asyncio/services/share.py
--rw-r--r--   0        0        0    47360 2024-03-25 21:21:53.318793 pangea_sdk-3.8.0b3/pangea/asyncio/services/vault.py
--rw-r--r--   0        0        0     3842 2024-03-25 21:21:53.318793 pangea_sdk-3.8.0b3/pangea/audit_logger.py
--rw-r--r--   0        0        0     1662 2024-03-25 21:21:53.318793 pangea_sdk-3.8.0b3/pangea/config.py
--rw-r--r--   0        0        0     8443 2024-03-25 21:21:53.318793 pangea_sdk-3.8.0b3/pangea/deep_verify.py
--rw-r--r--   0        0        0      608 2024-03-25 21:21:53.318793 pangea_sdk-3.8.0b3/pangea/deprecated.py
--rw-r--r--   0        0        0     7019 2024-03-25 21:21:53.318793 pangea_sdk-3.8.0b3/pangea/dump_audit.py
--rw-r--r--   0        0        0     5656 2024-03-25 21:21:53.318793 pangea_sdk-3.8.0b3/pangea/exceptions.py
--rw-r--r--   0        0        0     1227 2024-03-25 21:21:53.318793 pangea_sdk-3.8.0b3/pangea/file_uploader.py
--rw-r--r--   0        0        0        0 2024-03-25 21:21:53.423792 pangea_sdk-3.8.0b3/pangea/py.typed
--rw-r--r--   0        0        0    24346 2024-03-25 21:21:53.318793 pangea_sdk-3.8.0b3/pangea/request.py
--rw-r--r--   0        0        0     7042 2024-03-25 21:21:53.318793 pangea_sdk-3.8.0b3/pangea/response.py
--rw-r--r--   0        0        0      340 2024-03-25 21:21:53.319793 pangea_sdk-3.8.0b3/pangea/services/__init__.py
--rw-r--r--   0        0        0    32834 2024-03-25 21:21:53.319793 pangea_sdk-3.8.0b3/pangea/services/audit/audit.py
--rw-r--r--   0        0        0      471 2024-03-25 21:21:53.319793 pangea_sdk-3.8.0b3/pangea/services/audit/exceptions.py
--rw-r--r--   0        0        0    12644 2024-03-25 21:21:53.319793 pangea_sdk-3.8.0b3/pangea/services/audit/models.py
--rw-r--r--   0        0        0     5567 2024-03-25 21:21:53.319793 pangea_sdk-3.8.0b3/pangea/services/audit/signing.py
--rw-r--r--   0        0        0     7596 2024-03-25 21:21:53.319793 pangea_sdk-3.8.0b3/pangea/services/audit/util.py
--rw-r--r--   0        0        0    43280 2024-03-25 21:21:53.319793 pangea_sdk-3.8.0b3/pangea/services/authn/authn.py
--rw-r--r--   0        0        0    18104 2024-03-25 21:21:53.319793 pangea_sdk-3.8.0b3/pangea/services/authn/models.py
--rw-r--r--   0        0        0    12627 2024-03-25 21:21:53.319793 pangea_sdk-3.8.0b3/pangea/services/authz.py
--rw-r--r--   0        0        0     3012 2024-03-25 21:21:53.319793 pangea_sdk-3.8.0b3/pangea/services/base.py
--rw-r--r--   0        0        0     3885 2024-03-25 21:21:53.319793 pangea_sdk-3.8.0b3/pangea/services/embargo.py
--rw-r--r--   0        0        0     6923 2024-03-25 21:21:53.319793 pangea_sdk-3.8.0b3/pangea/services/file_scan.py
--rw-r--r--   0        0        0    51637 2024-03-25 21:21:53.319793 pangea_sdk-3.8.0b3/pangea/services/intel.py
--rw-r--r--   0        0        0     7772 2024-03-25 21:21:53.319793 pangea_sdk-3.8.0b3/pangea/services/redact.py
--rw-r--r--   0        0        0    10092 2024-03-25 21:21:53.320793 pangea_sdk-3.8.0b3/pangea/services/sanitize.py
--rw-r--r--   0        0        0     2797 2024-03-25 21:21:53.320793 pangea_sdk-3.8.0b3/pangea/services/share/file_format.py
--rw-r--r--   0        0        0    32497 2024-03-25 21:21:53.320793 pangea_sdk-3.8.0b3/pangea/services/share/share.py
--rw-r--r--   0        0        0     1450 2024-03-25 21:21:53.320793 pangea_sdk-3.8.0b3/pangea/services/vault/models/asymmetric.py
--rw-r--r--   0        0        0    11120 2024-03-25 21:21:53.320793 pangea_sdk-3.8.0b3/pangea/services/vault/models/common.py
--rw-r--r--   0        0        0      481 2024-03-25 21:21:53.320793 pangea_sdk-3.8.0b3/pangea/services/vault/models/secret.py
--rw-r--r--   0        0        0     1330 2024-03-25 21:21:53.320793 pangea_sdk-3.8.0b3/pangea/services/vault/models/symmetric.py
--rw-r--r--   0        0        0    47168 2024-03-25 21:21:53.320793 pangea_sdk-3.8.0b3/pangea/services/vault/vault.py
--rw-r--r--   0        0        0     6429 2024-03-25 21:21:53.320793 pangea_sdk-3.8.0b3/pangea/tools.py
--rw-r--r--   0        0        0     5289 2024-03-25 21:21:53.320793 pangea_sdk-3.8.0b3/pangea/utils.py
--rw-r--r--   0        0        0    10756 2024-03-25 21:21:53.320793 pangea_sdk-3.8.0b3/pangea/verify_audit.py
--rw-r--r--   0        0        0     1370 2024-03-25 21:21:53.321793 pangea_sdk-3.8.0b3/pyproject.toml
--rw-r--r--   0        0        0     7735 1970-01-01 00:00:00.000000 pangea_sdk-3.8.0b3/PKG-INFO
+-rw-r--r--   0        0        0     6531 2024-03-28 14:16:53.329991 pangea_sdk-3.8.0b4/README.md
+-rw-r--r--   0        0        0      251 2024-03-28 14:16:53.329991 pangea_sdk-3.8.0b4/pangea/__init__.py
+-rw-r--r--   0        0        0       45 2024-03-28 14:16:53.329991 pangea_sdk-3.8.0b4/pangea/asyncio/__init__.py
+-rw-r--r--   0        0        0     1462 2024-03-28 14:16:53.329991 pangea_sdk-3.8.0b4/pangea/asyncio/file_uploader.py
+-rw-r--r--   0        0        0    17272 2024-03-28 14:16:53.330991 pangea_sdk-3.8.0b4/pangea/asyncio/request.py
+-rw-r--r--   0        0        0      386 2024-03-28 14:16:53.330991 pangea_sdk-3.8.0b4/pangea/asyncio/services/__init__.py
+-rw-r--r--   0        0        0    19594 2024-03-28 14:16:53.330991 pangea_sdk-3.8.0b4/pangea/asyncio/services/audit.py
+-rw-r--r--   0        0        0    43812 2024-03-28 14:16:53.330991 pangea_sdk-3.8.0b4/pangea/asyncio/services/authn.py
+-rw-r--r--   0        0        0     9958 2024-03-28 14:16:53.330991 pangea_sdk-3.8.0b4/pangea/asyncio/services/authz.py
+-rw-r--r--   0        0        0     2663 2024-03-28 14:16:53.330991 pangea_sdk-3.8.0b4/pangea/asyncio/services/base.py
+-rw-r--r--   0        0        0     3056 2024-03-28 14:16:53.330991 pangea_sdk-3.8.0b4/pangea/asyncio/services/embargo.py
+-rw-r--r--   0        0        0     6301 2024-03-28 14:16:53.330991 pangea_sdk-3.8.0b4/pangea/asyncio/services/file_scan.py
+-rw-r--r--   0        0        0    37665 2024-03-28 14:16:53.331991 pangea_sdk-3.8.0b4/pangea/asyncio/services/intel.py
+-rw-r--r--   0        0        0     5174 2024-03-28 14:16:53.331991 pangea_sdk-3.8.0b4/pangea/asyncio/services/redact.py
+-rw-r--r--   0        0        0     7576 2024-03-28 14:16:53.331991 pangea_sdk-3.8.0b4/pangea/asyncio/services/sanitize.py
+-rw-r--r--   0        0        0    24761 2024-03-28 14:16:53.331991 pangea_sdk-3.8.0b4/pangea/asyncio/services/share.py
+-rw-r--r--   0        0        0    47360 2024-03-28 14:16:53.331991 pangea_sdk-3.8.0b4/pangea/asyncio/services/vault.py
+-rw-r--r--   0        0        0     3842 2024-03-28 14:16:53.331991 pangea_sdk-3.8.0b4/pangea/audit_logger.py
+-rw-r--r--   0        0        0     1662 2024-03-28 14:16:53.331991 pangea_sdk-3.8.0b4/pangea/config.py
+-rw-r--r--   0        0        0     8443 2024-03-28 14:16:53.331991 pangea_sdk-3.8.0b4/pangea/deep_verify.py
+-rw-r--r--   0        0        0      608 2024-03-28 14:16:53.331991 pangea_sdk-3.8.0b4/pangea/deprecated.py
+-rw-r--r--   0        0        0     7019 2024-03-28 14:16:53.331991 pangea_sdk-3.8.0b4/pangea/dump_audit.py
+-rw-r--r--   0        0        0     5656 2024-03-28 14:16:53.331991 pangea_sdk-3.8.0b4/pangea/exceptions.py
+-rw-r--r--   0        0        0     1227 2024-03-28 14:16:53.331991 pangea_sdk-3.8.0b4/pangea/file_uploader.py
+-rw-r--r--   0        0        0        0 2024-03-28 14:16:53.442991 pangea_sdk-3.8.0b4/pangea/py.typed
+-rw-r--r--   0        0        0    24346 2024-03-28 14:16:53.332991 pangea_sdk-3.8.0b4/pangea/request.py
+-rw-r--r--   0        0        0     7042 2024-03-28 14:16:53.332991 pangea_sdk-3.8.0b4/pangea/response.py
+-rw-r--r--   0        0        0      340 2024-03-28 14:16:53.332991 pangea_sdk-3.8.0b4/pangea/services/__init__.py
+-rw-r--r--   0        0        0    32834 2024-03-28 14:16:53.332991 pangea_sdk-3.8.0b4/pangea/services/audit/audit.py
+-rw-r--r--   0        0        0      471 2024-03-28 14:16:53.332991 pangea_sdk-3.8.0b4/pangea/services/audit/exceptions.py
+-rw-r--r--   0        0        0    12644 2024-03-28 14:16:53.332991 pangea_sdk-3.8.0b4/pangea/services/audit/models.py
+-rw-r--r--   0        0        0     5567 2024-03-28 14:16:53.332991 pangea_sdk-3.8.0b4/pangea/services/audit/signing.py
+-rw-r--r--   0        0        0     7596 2024-03-28 14:16:53.332991 pangea_sdk-3.8.0b4/pangea/services/audit/util.py
+-rw-r--r--   0        0        0    43280 2024-03-28 14:16:53.332991 pangea_sdk-3.8.0b4/pangea/services/authn/authn.py
+-rw-r--r--   0        0        0    18104 2024-03-28 14:16:53.333991 pangea_sdk-3.8.0b4/pangea/services/authn/models.py
+-rw-r--r--   0        0        0    12627 2024-03-28 14:16:53.333991 pangea_sdk-3.8.0b4/pangea/services/authz.py
+-rw-r--r--   0        0        0     3012 2024-03-28 14:16:53.333991 pangea_sdk-3.8.0b4/pangea/services/base.py
+-rw-r--r--   0        0        0     3885 2024-03-28 14:16:53.333991 pangea_sdk-3.8.0b4/pangea/services/embargo.py
+-rw-r--r--   0        0        0     6923 2024-03-28 14:16:53.333991 pangea_sdk-3.8.0b4/pangea/services/file_scan.py
+-rw-r--r--   0        0        0    51637 2024-03-28 14:16:53.333991 pangea_sdk-3.8.0b4/pangea/services/intel.py
+-rw-r--r--   0        0        0     7772 2024-03-28 14:16:53.333991 pangea_sdk-3.8.0b4/pangea/services/redact.py
+-rw-r--r--   0        0        0    10092 2024-03-28 14:16:53.333991 pangea_sdk-3.8.0b4/pangea/services/sanitize.py
+-rw-r--r--   0        0        0     2797 2024-03-28 14:16:53.333991 pangea_sdk-3.8.0b4/pangea/services/share/file_format.py
+-rw-r--r--   0        0        0    32499 2024-03-28 14:16:53.333991 pangea_sdk-3.8.0b4/pangea/services/share/share.py
+-rw-r--r--   0        0        0     1450 2024-03-28 14:16:53.333991 pangea_sdk-3.8.0b4/pangea/services/vault/models/asymmetric.py
+-rw-r--r--   0        0        0    11120 2024-03-28 14:16:53.333991 pangea_sdk-3.8.0b4/pangea/services/vault/models/common.py
+-rw-r--r--   0        0        0      481 2024-03-28 14:16:53.333991 pangea_sdk-3.8.0b4/pangea/services/vault/models/secret.py
+-rw-r--r--   0        0        0     1330 2024-03-28 14:16:53.333991 pangea_sdk-3.8.0b4/pangea/services/vault/models/symmetric.py
+-rw-r--r--   0        0        0    47168 2024-03-28 14:16:53.333991 pangea_sdk-3.8.0b4/pangea/services/vault/vault.py
+-rw-r--r--   0        0        0     6429 2024-03-28 14:16:53.333991 pangea_sdk-3.8.0b4/pangea/tools.py
+-rw-r--r--   0        0        0     5289 2024-03-28 14:16:53.334991 pangea_sdk-3.8.0b4/pangea/utils.py
+-rw-r--r--   0        0        0    10756 2024-03-28 14:16:53.334991 pangea_sdk-3.8.0b4/pangea/verify_audit.py
+-rw-r--r--   0        0        0     1370 2024-03-28 14:16:53.334991 pangea_sdk-3.8.0b4/pyproject.toml
+-rw-r--r--   0        0        0     7735 1970-01-01 00:00:00.000000 pangea_sdk-3.8.0b4/PKG-INFO
```

### Comparing `pangea_sdk-3.8.0b3/README.md` & `pangea_sdk-3.8.0b4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -36,21 +36,21 @@
 version number. These releases serve to preview beta services and APIs. Per
 Semantic Versioning, they are considered unstable and do not carry the same
 compatibility guarantees as stable releases. [Beta changelog](https://github.com/pangeacyber/pangea-python/blob/beta/CHANGELOG.md).
 
 Via pip:
 
 ```bash
-$ pip3 install pangea-sdk==3.8.0b3
+$ pip3 install pangea-sdk==3.8.0b4
 ```
 
 Via poetry:
 
 ```bash
-$ poetry add pangea-sdk==3.8.0b3
+$ poetry add pangea-sdk==3.8.0b4
 ```
 
 ## Usage
 
 - [Documentation][]
 - [GA Examples][]
 - [Beta Examples][]
```

### Comparing `pangea_sdk-3.8.0b3/pangea/asyncio/file_uploader.py` & `pangea_sdk-3.8.0b4/pangea/asyncio/file_uploader.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-3.8.0b3/pangea/asyncio/request.py` & `pangea_sdk-3.8.0b4/pangea/asyncio/request.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-3.8.0b3/pangea/asyncio/services/audit.py` & `pangea_sdk-3.8.0b4/pangea/asyncio/services/audit.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-3.8.0b3/pangea/asyncio/services/authn.py` & `pangea_sdk-3.8.0b4/pangea/asyncio/services/authn.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-3.8.0b3/pangea/asyncio/services/authz.py` & `pangea_sdk-3.8.0b4/pangea/asyncio/services/authz.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-3.8.0b3/pangea/asyncio/services/base.py` & `pangea_sdk-3.8.0b4/pangea/asyncio/services/base.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-3.8.0b3/pangea/asyncio/services/embargo.py` & `pangea_sdk-3.8.0b4/pangea/asyncio/services/embargo.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-3.8.0b3/pangea/asyncio/services/file_scan.py` & `pangea_sdk-3.8.0b4/pangea/asyncio/services/file_scan.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-3.8.0b3/pangea/asyncio/services/intel.py` & `pangea_sdk-3.8.0b4/pangea/asyncio/services/intel.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-3.8.0b3/pangea/asyncio/services/redact.py` & `pangea_sdk-3.8.0b4/pangea/asyncio/services/redact.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-3.8.0b3/pangea/asyncio/services/sanitize.py` & `pangea_sdk-3.8.0b4/pangea/asyncio/services/sanitize.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-3.8.0b3/pangea/asyncio/services/share.py` & `pangea_sdk-3.8.0b4/pangea/asyncio/services/share.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,15 @@
                     print(f"Response: {response.result}")
             except pe.PangeaAPIException as e:
                 print(f"Request Error: {e.response.summary}")
                 for err in e.errors:
                     print(f"\\t{err.detail} \\n")
         """
 
-        files: List[Tuple] = [("upload", (name, file, "application/octet-stream"))]
+        files: List[Tuple] = [("upload", ("file", file, "application/octet-stream"))]
 
         if transfer_method == TransferMethod.POST_URL:
             params = get_file_upload_params(file)
             crc32c = params.crc_hex
             sha256 = params.sha256_hex
             size = params.size
         elif size is None and get_file_size(file=file) == 0:
```

### Comparing `pangea_sdk-3.8.0b3/pangea/asyncio/services/vault.py` & `pangea_sdk-3.8.0b4/pangea/asyncio/services/vault.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-3.8.0b3/pangea/audit_logger.py` & `pangea_sdk-3.8.0b4/pangea/audit_logger.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-3.8.0b3/pangea/config.py` & `pangea_sdk-3.8.0b4/pangea/config.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-3.8.0b3/pangea/deep_verify.py` & `pangea_sdk-3.8.0b4/pangea/deep_verify.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-3.8.0b3/pangea/deprecated.py` & `pangea_sdk-3.8.0b4/pangea/deprecated.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-3.8.0b3/pangea/dump_audit.py` & `pangea_sdk-3.8.0b4/pangea/dump_audit.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-3.8.0b3/pangea/exceptions.py` & `pangea_sdk-3.8.0b4/pangea/exceptions.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-3.8.0b3/pangea/file_uploader.py` & `pangea_sdk-3.8.0b4/pangea/file_uploader.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-3.8.0b3/pangea/request.py` & `pangea_sdk-3.8.0b4/pangea/request.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-3.8.0b3/pangea/response.py` & `pangea_sdk-3.8.0b4/pangea/response.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-3.8.0b3/pangea/services/audit/audit.py` & `pangea_sdk-3.8.0b4/pangea/services/audit/audit.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-3.8.0b3/pangea/services/audit/models.py` & `pangea_sdk-3.8.0b4/pangea/services/audit/models.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-3.8.0b3/pangea/services/audit/signing.py` & `pangea_sdk-3.8.0b4/pangea/services/audit/signing.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-3.8.0b3/pangea/services/audit/util.py` & `pangea_sdk-3.8.0b4/pangea/services/audit/util.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-3.8.0b3/pangea/services/authn/authn.py` & `pangea_sdk-3.8.0b4/pangea/services/authn/authn.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-3.8.0b3/pangea/services/authn/models.py` & `pangea_sdk-3.8.0b4/pangea/services/authn/models.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-3.8.0b3/pangea/services/authz.py` & `pangea_sdk-3.8.0b4/pangea/services/authz.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-3.8.0b3/pangea/services/base.py` & `pangea_sdk-3.8.0b4/pangea/services/base.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-3.8.0b3/pangea/services/embargo.py` & `pangea_sdk-3.8.0b4/pangea/services/embargo.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-3.8.0b3/pangea/services/file_scan.py` & `pangea_sdk-3.8.0b4/pangea/services/file_scan.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-3.8.0b3/pangea/services/intel.py` & `pangea_sdk-3.8.0b4/pangea/services/intel.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-3.8.0b3/pangea/services/redact.py` & `pangea_sdk-3.8.0b4/pangea/services/redact.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-3.8.0b3/pangea/services/sanitize.py` & `pangea_sdk-3.8.0b4/pangea/services/sanitize.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-3.8.0b3/pangea/services/share/file_format.py` & `pangea_sdk-3.8.0b4/pangea/services/share/file_format.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-3.8.0b3/pangea/services/share/share.py` & `pangea_sdk-3.8.0b4/pangea/services/share/share.py`

 * *Files identical despite different names*

```diff
@@ -561,15 +561,15 @@
                     response = share.put(file=f)
                     print(f"Response: {response.result}")
             except pe.PangeaAPIException as e:
                 print(f"Request Error: {e.response.summary}")
                 for err in e.errors:
                     print(f"\\t{err.detail} \\n")
         """
-        files: List[Tuple] = [("upload", (name, file, "application/octet-stream"))]
+        files: List[Tuple] = [("upload", ("file", file, "application/octet-stream"))]
 
         if transfer_method == TransferMethod.POST_URL:
             params = get_file_upload_params(file)
             crc32c = params.crc_hex
             sha256 = params.sha256_hex
             size = params.size
         elif size is None and get_file_size(file=file) == 0:
```

### Comparing `pangea_sdk-3.8.0b3/pangea/services/vault/models/asymmetric.py` & `pangea_sdk-3.8.0b4/pangea/services/vault/models/asymmetric.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-3.8.0b3/pangea/services/vault/models/common.py` & `pangea_sdk-3.8.0b4/pangea/services/vault/models/common.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-3.8.0b3/pangea/services/vault/models/symmetric.py` & `pangea_sdk-3.8.0b4/pangea/services/vault/models/symmetric.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-3.8.0b3/pangea/services/vault/vault.py` & `pangea_sdk-3.8.0b4/pangea/services/vault/vault.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-3.8.0b3/pangea/tools.py` & `pangea_sdk-3.8.0b4/pangea/tools.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-3.8.0b3/pangea/utils.py` & `pangea_sdk-3.8.0b4/pangea/utils.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-3.8.0b3/pangea/verify_audit.py` & `pangea_sdk-3.8.0b4/pangea/verify_audit.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-3.8.0b3/pyproject.toml` & `pangea_sdk-3.8.0b4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pangea-sdk"
-version = "3.8.0beta3"
+version = "3.8.0beta4"
 description = "Pangea API SDK"
 authors = ["Glenn Gallien <glenn.gallien@pangea.cloud>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://pangea.cloud/docs/sdk/python/"
 repository = "https://github.com/pangeacyber/pangea-python/tree/main/packages/pangea-sdk"
 keywords = ["Pangea", "SDK", "Audit"]
```

### Comparing `pangea_sdk-3.8.0b3/PKG-INFO` & `pangea_sdk-3.8.0b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pangea-sdk
-Version: 3.8.0b3
+Version: 3.8.0b4
 Summary: Pangea API SDK
 Home-page: https://pangea.cloud/docs/sdk/python/
 License: MIT
 Keywords: Pangea,SDK,Audit
 Author: Glenn Gallien
 Author-email: glenn.gallien@pangea.cloud
 Requires-Python: >=3.7.2,<4.0.0
@@ -66,21 +66,21 @@
 version number. These releases serve to preview beta services and APIs. Per
 Semantic Versioning, they are considered unstable and do not carry the same
 compatibility guarantees as stable releases. [Beta changelog](https://github.com/pangeacyber/pangea-python/blob/beta/CHANGELOG.md).
 
 Via pip:
 
 ```bash
-$ pip3 install pangea-sdk==3.8.0b3
+$ pip3 install pangea-sdk==3.8.0b4
 ```
 
 Via poetry:
 
 ```bash
-$ poetry add pangea-sdk==3.8.0b3
+$ poetry add pangea-sdk==3.8.0b4
 ```
 
 ## Usage
 
 - [Documentation][]
 - [GA Examples][]
 - [Beta Examples][]
```

