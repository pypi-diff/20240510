# Comparing `tmp/fds_sdk_utils-1.1.1.tar.gz` & `tmp/fds_sdk_utils-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fds_sdk_utils-1.1.1.tar", max compression
+gzip compressed data, was "fds_sdk_utils-2.0.0.tar", max compression
```

## Comparing `fds_sdk_utils-1.1.1.tar` & `fds_sdk_utils-2.0.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2024-05-02 12:53:38.399939 fds_sdk_utils-1.1.1/LICENSE
--rw-r--r--   0        0        0     6461 2024-05-02 12:53:38.399939 fds_sdk_utils-1.1.1/README.md
--rw-r--r--   0        0        0      853 2024-05-02 12:53:38.399939 fds_sdk_utils-1.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-02 12:53:38.399939 fds_sdk_utils-1.1.1/src/fds/__init__.py
--rw-r--r--   0        0        0        0 2024-05-02 12:53:38.399939 fds_sdk_utils-1.1.1/src/fds/sdk/__init__.py
--rw-r--r--   0        0        0      253 2024-05-02 12:53:38.399939 fds_sdk_utils-1.1.1/src/fds/sdk/utils/__init__.py
--rw-r--r--   0        0        0      273 2024-05-02 12:53:38.399939 fds_sdk_utils-1.1.1/src/fds/sdk/utils/authentication/__init__.py
--rw-r--r--   0        0        0    12392 2024-05-02 12:53:38.399939 fds_sdk_utils-1.1.1/src/fds/sdk/utils/authentication/confidential.py
--rw-r--r--   0        0        0      722 2024-05-02 12:53:38.399939 fds_sdk_utils-1.1.1/src/fds/sdk/utils/authentication/constants.py
--rw-r--r--   0        0        0      724 2024-05-02 12:53:38.399939 fds_sdk_utils-1.1.1/src/fds/sdk/utils/authentication/exceptions.py
--rw-r--r--   0        0        0      332 2024-05-02 12:53:38.399939 fds_sdk_utils-1.1.1/src/fds/sdk/utils/authentication/oauth2client.py
--rw-r--r--   0        0        0     7371 1970-01-01 00:00:00.000000 fds_sdk_utils-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-10 12:53:13.596362 fds_sdk_utils-2.0.0/LICENSE
+-rw-r--r--   0        0        0     6461 2024-05-10 12:53:13.596362 fds_sdk_utils-2.0.0/README.md
+-rw-r--r--   0        0        0      765 2024-05-10 12:53:13.596362 fds_sdk_utils-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-10 12:53:13.596362 fds_sdk_utils-2.0.0/src/fds/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 12:53:13.596362 fds_sdk_utils-2.0.0/src/fds/sdk/__init__.py
+-rw-r--r--   0        0        0      253 2024-05-10 12:53:13.596362 fds_sdk_utils-2.0.0/src/fds/sdk/utils/__init__.py
+-rw-r--r--   0        0        0      273 2024-05-10 12:53:13.596362 fds_sdk_utils-2.0.0/src/fds/sdk/utils/authentication/__init__.py
+-rw-r--r--   0        0        0    12486 2024-05-10 12:53:13.596362 fds_sdk_utils-2.0.0/src/fds/sdk/utils/authentication/confidential.py
+-rw-r--r--   0        0        0      722 2024-05-10 12:53:13.596362 fds_sdk_utils-2.0.0/src/fds/sdk/utils/authentication/constants.py
+-rw-r--r--   0        0        0      724 2024-05-10 12:53:13.596362 fds_sdk_utils-2.0.0/src/fds/sdk/utils/authentication/exceptions.py
+-rw-r--r--   0        0        0      332 2024-05-10 12:53:13.600362 fds_sdk_utils-2.0.0/src/fds/sdk/utils/authentication/oauth2client.py
+-rw-r--r--   0        0        0     7304 1970-01-01 00:00:00.000000 fds_sdk_utils-2.0.0/PKG-INFO
```

### Comparing `fds_sdk_utils-1.1.1/LICENSE` & `fds_sdk_utils-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fds_sdk_utils-1.1.1/README.md` & `fds_sdk_utils-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `fds_sdk_utils-1.1.1/pyproject.toml` & `fds_sdk_utils-2.0.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fds.sdk.utils"
-version = "1.1.1"
+version = "2.0.0"
 description = "Utilities for interacting with FactSet APIs."
 authors = ["FactSet Research Systems"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://developer.factset.com"
 keywords = [
   "FactSet",
@@ -13,27 +13,27 @@
 ]
 packages = [
   { include = "fds", from = "src" }
 ]
 exclude = ["tests"]
 
 [tool.poetry.dependencies]
-python = "^3.7.0"
-python-jose = { extras = ["cryptography"], version = "^3.3.0" }
-requests-oauthlib = "^1.3.0"
+python = "^3.8.0"
+requests-oauthlib = "^2.0.0"
 requests = "^2.28.2"
 oauthlib = "^3.2.2"
+joserfc = "^0.9.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.4"
-black = { version = "^23.3", allow-prereleases = true }
-pytest-cov = "^4.1.0"
+pytest = "^8.2.0"
+black = "^24.4.2"
+pytest-cov = "^5.0.0"
 pytest-mock = "^3.11.1"
 tox = "^4.8.0"
 tox-gh-actions = "^3.2.0"
 
 [tool.black]
 line-length = 120
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `fds_sdk_utils-1.1.1/src/fds/sdk/utils/authentication/confidential.py` & `fds_sdk_utils-2.0.0/src/fds/sdk/utils/authentication/confidential.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import logging
 import time
 import uuid
 
-import requests
-from jose import JWSError, jws
+from joserfc import jwt
+from joserfc.jwk import RSAKey
 from oauthlib.oauth2 import BackendApplicationClient
 from requests import Session
 from requests.adapters import HTTPAdapter
 from requests_oauthlib import OAuth2Session
 from urllib3 import Retry
 
 from .constants import CONSTS
@@ -212,31 +212,35 @@
             "Retrieved issuer: %s and token_endpoint: %s from well_known_uri",
             self._well_known_uri_metadata[CONSTS.META_ISSUER],
             self._well_known_uri_metadata[CONSTS.META_TOKEN_ENDPOINT],
         )
 
     def _get_client_assertion_jws(self) -> str:
         issued_at = time.time()
+        key = RSAKey.import_key(self._config["jwk"])
+
         try:
-            return jws.sign(
-                payload={
+            return jwt.encode(
+                claims={
                     "sub": self._config[CONSTS.CONFIG_CLIENT_ID],
                     "iss": self._config[CONSTS.CONFIG_CLIENT_ID],
                     "aud": [self._well_known_uri_metadata[CONSTS.META_ISSUER]],
                     "nbf": issued_at - CONSTS.CC_JWT_NOT_BEFORE_SECS,
                     "iat": issued_at,
                     "exp": issued_at + CONSTS.CC_JWT_EXPIRE_AFTER_SECS,
                     "jti": str(uuid.uuid4()),
                 },
-                key=self._config[CONSTS.CONFIG_JWK],
-                algorithm=self._config[CONSTS.CONFIG_JWK][CONSTS.JWK_ALG],
-                headers={"kid": self._config[CONSTS.CONFIG_JWK][CONSTS.JWK_KID]},
+                key=key,
+                header={
+                    "kid": self._config[CONSTS.CONFIG_JWK][CONSTS.JWK_KID],
+                    "alg": self._config[CONSTS.CONFIG_JWK][CONSTS.JWK_ALG],
+                },
             )
-        except JWSError as je:
-            raise JWSSigningError("Error attempting to sign JWS") from je
+        except ValueError as value_error:
+            raise JWSSigningError("Error attempting to sign JWS") from value_error
 
     def _is_cached_token_valid(self) -> bool:
         if not self._cached_token:
             log.debug("Access Token cache is empty")
             return False
         if time.time() < self._cached_token[CONSTS.TOKEN_EXPIRES_AT]:
             return True
```

### Comparing `fds_sdk_utils-1.1.1/src/fds/sdk/utils/authentication/constants.py` & `fds_sdk_utils-2.0.0/src/fds/sdk/utils/authentication/constants.py`

 * *Files identical despite different names*

### Comparing `fds_sdk_utils-1.1.1/src/fds/sdk/utils/authentication/exceptions.py` & `fds_sdk_utils-2.0.0/src/fds/sdk/utils/authentication/exceptions.py`

 * *Files identical despite different names*

### Comparing `fds_sdk_utils-1.1.1/PKG-INFO` & `fds_sdk_utils-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: fds.sdk.utils
-Version: 1.1.1
+Version: 2.0.0
 Summary: Utilities for interacting with FactSet APIs.
 Home-page: https://developer.factset.com
 License: Apache-2.0
 Keywords: FactSet,API,SDK
 Author: FactSet Research Systems
-Requires-Python: >=3.7.0,<4.0.0
+Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: joserfc (>=0.9.0,<0.10.0)
 Requires-Dist: oauthlib (>=3.2.2,<4.0.0)
-Requires-Dist: python-jose[cryptography] (>=3.3.0,<4.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
-Requires-Dist: requests-oauthlib (>=1.3.0,<2.0.0)
+Requires-Dist: requests-oauthlib (>=2.0.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 <img alt="FactSet" src="https://www.factset.com/hubfs/Assets/images/factset-logo.svg" height="56" width="290">
 
 # FactSet SDK Utilities for Python
 
 [![PyPi](https://img.shields.io/pypi/v/fds.sdk.utils)](https://pypi.org/project/fds.sdk.utils/)
```

