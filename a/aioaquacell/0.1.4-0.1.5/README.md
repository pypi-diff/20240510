# Comparing `tmp/aioaquacell-0.1.4.tar.gz` & `tmp/aioaquacell-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\aioaquacell-0.1.4.tar", last modified: Mon Apr 29 20:31:41 2024, max compression
+gzip compressed data, was "dist\aioaquacell-0.1.5.tar", last modified: Fri May 10 13:50:18 2024, max compression
```

## Comparing `aioaquacell-0.1.4.tar` & `aioaquacell-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 20:31:41.201890 aioaquacell-0.1.4/
--rw-rw-rw-   0        0        0    11542 2023-09-29 19:48:26.000000 aioaquacell-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     1262 2024-04-29 20:31:41.201890 aioaquacell-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      818 2023-10-12 20:07:12.000000 aioaquacell-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 20:31:41.196891 aioaquacell-0.1.4/aioaquacell/
--rw-rw-rw-   0        0        0      149 2024-02-05 17:27:05.000000 aioaquacell-0.1.4/aioaquacell/__init__.py
--rw-rw-rw-   0        0        0     2916 2024-04-29 20:30:36.000000 aioaquacell-0.1.4/aioaquacell/aquacell_api.py
--rw-rw-rw-   0        0        0      297 2024-02-05 14:02:18.000000 aioaquacell-0.1.4/aioaquacell/authentication_tokens.py
--rw-rw-rw-   0        0        0     3465 2023-10-12 18:10:05.000000 aioaquacell-0.1.4/aioaquacell/aws_cognito_authenticator.py
--rw-rw-rw-   0        0        0      289 2023-09-27 20:13:49.000000 aioaquacell-0.1.4/aioaquacell/aws_credentials.py
--rw-rw-rw-   0        0        0     1106 2023-10-04 17:49:18.000000 aioaquacell-0.1.4/aioaquacell/aws_signature_request.py
--rw-rw-rw-   0        0        0      340 2024-02-05 14:20:59.000000 aioaquacell-0.1.4/aioaquacell/exceptions.py
--rw-rw-rw-   0        0        0     1771 2024-03-09 22:46:27.000000 aioaquacell-0.1.4/aioaquacell/softener.py
-drwxrwxrwx   0        0        0        0 2024-04-29 20:31:41.201890 aioaquacell-0.1.4/aioaquacell.egg-info/
--rw-rw-rw-   0        0        0     1262 2024-04-29 20:31:41.000000 aioaquacell-0.1.4/aioaquacell.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      458 2024-04-29 20:31:41.000000 aioaquacell-0.1.4/aioaquacell.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 20:31:41.000000 aioaquacell-0.1.4/aioaquacell.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2024-04-29 20:31:41.000000 aioaquacell-0.1.4/aioaquacell.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-29 20:31:41.000000 aioaquacell-0.1.4/aioaquacell.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-29 20:31:41.202891 aioaquacell-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      900 2024-04-29 20:30:49.000000 aioaquacell-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:50:18.145942 aioaquacell-0.1.5/
+-rw-rw-rw-   0        0        0    11542 2023-09-29 19:48:26.000000 aioaquacell-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     1262 2024-05-10 13:50:18.145942 aioaquacell-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      818 2023-10-12 20:07:12.000000 aioaquacell-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 13:50:18.137941 aioaquacell-0.1.5/aioaquacell/
+-rw-rw-rw-   0        0        0      149 2024-05-10 07:03:37.000000 aioaquacell-0.1.5/aioaquacell/__init__.py
+-rw-rw-rw-   0        0        0     3202 2024-05-10 07:07:46.000000 aioaquacell-0.1.5/aioaquacell/aquacell_api.py
+-rw-rw-rw-   0        0        0      297 2024-02-05 14:02:18.000000 aioaquacell-0.1.5/aioaquacell/authentication_tokens.py
+-rw-rw-rw-   0        0        0     3701 2024-05-10 07:09:20.000000 aioaquacell-0.1.5/aioaquacell/aws_cognito_authenticator.py
+-rw-rw-rw-   0        0        0      289 2023-09-27 20:13:49.000000 aioaquacell-0.1.5/aioaquacell/aws_credentials.py
+-rw-rw-rw-   0        0        0     1106 2023-10-04 17:49:18.000000 aioaquacell-0.1.5/aioaquacell/aws_signature_request.py
+-rw-rw-rw-   0        0        0      340 2024-02-05 14:20:59.000000 aioaquacell-0.1.5/aioaquacell/exceptions.py
+-rw-rw-rw-   0        0        0     2131 2024-05-09 21:49:17.000000 aioaquacell-0.1.5/aioaquacell/softener.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:50:18.144942 aioaquacell-0.1.5/aioaquacell.egg-info/
+-rw-rw-rw-   0        0        0     1262 2024-05-10 13:50:18.000000 aioaquacell-0.1.5/aioaquacell.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      458 2024-05-10 13:50:18.000000 aioaquacell-0.1.5/aioaquacell.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 13:50:18.000000 aioaquacell-0.1.5/aioaquacell.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2024-05-10 13:50:18.000000 aioaquacell-0.1.5/aioaquacell.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-10 13:50:18.000000 aioaquacell-0.1.5/aioaquacell.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-10 13:50:18.146942 aioaquacell-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      900 2024-05-10 13:45:02.000000 aioaquacell-0.1.5/setup.py
```

### Comparing `aioaquacell-0.1.4/LICENSE` & `aioaquacell-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aioaquacell-0.1.4/PKG-INFO` & `aioaquacell-0.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: aioaquacell
-Version: 0.1.4
+Version: 0.1.5
 Summary: Asynchronous library to retrieve details of your Aquacell water softener device
 Home-page: https://github.com/Jordi1990/aioaquacell
-Download-URL: https://github.com/Jordi1990/aioaquacell/archive/refs/tags/v0.1.4.tar.gz
+Download-URL: https://github.com/Jordi1990/aioaquacell/archive/refs/tags/v0.1.5.tar.gz
 Author: Jordi Epema
 Author-email: jordi.epema@gmail.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Aioaquacell
```

### Comparing `aioaquacell-0.1.4/README.md` & `aioaquacell-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `aioaquacell-0.1.4/aioaquacell/aquacell_api.py` & `aioaquacell-0.1.5/aioaquacell/aquacell_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """ Parses data from the Aquacell API. """
 import json
+import logging
 import string
 
 import botocore
 from aiohttp import ClientSession
 
 from aioaquacell.aws_cognito_authenticator import AwsCognitoAuthenticator
 from aioaquacell.aws_signature_request import AwsSignatureRequest
 from aioaquacell.exceptions import NotAuthenticated, ApiException, AuthenticationFailed
 from aioaquacell.softener import Softener
 
+_LOGGER = logging.getLogger(__name__)
 
 class AquacellApi:
     base_url = "https://y7xyrocicl.execute-api.eu-west-1.amazonaws.com"
     all_softeners = f"{base_url}/prod/v1/softeners/all"
     region_name = "eu-west-1"
     client_id = "64kp67l1jo9toeesan7s1sdpae"
     pool_id = "eu-west-1_noZbcE2Av"
@@ -31,23 +33,25 @@
         return await self.__authenticate(None, None, refresh_token)
 
     """" Authenticate using username and password. """
     async def authenticate(self, user_name, password) -> string:
         return await self.__authenticate(user_name, password, None)
 
     async def __authenticate(self, user_name, password, refresh_token) -> string:
+        _LOGGER.debug("Authenticating with %s - %s (%s)", user_name, password, refresh_token)
         try:
             if refresh_token is None:
                 token = await self.authenticator.get_new_token(user_name, password)
             else:
                 token = await self.authenticator.refresh_token(refresh_token)
 
             self.id_token = token.id_token
             return token.refresh_token
         except botocore.exceptions.ClientError as e:
+            _LOGGER.exception("Exception while authenticating")
             if e.response['Error']['Code'] == 'NotAuthorizedException':
                 raise AuthenticationFailed(e)
             else:
                 raise ApiException(e)
 
     async def get_all_softeners(self) -> list[Softener]:
         if self.id_token is None:
@@ -68,8 +72,9 @@
 
             softeners = []
             for softener_as_json in json_response:
                 softeners.append(Softener(softener_as_json))
 
             return softeners
         except botocore.exceptions.ClientError as e:
+            _LOGGER.exception("Exception while retrieving softeners")
             raise ApiException(e)
```

### Comparing `aioaquacell-0.1.4/aioaquacell/aws_cognito_authenticator.py` & `aioaquacell-0.1.5/aioaquacell/aws_cognito_authenticator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 """ AWS Cognito authentication and identity management. """
+import logging
+
 import aioboto3
 from pycognito import AWSSRP
 
 from aioaquacell.authentication_tokens import AuthenticationTokens
 from aioaquacell.aws_credentials import AwsCredentials
 
+_LOGGER = logging.getLogger(__name__)
+
 
 class AwsCognitoAuthenticator:
     def __init__(self, region_name, client_id, pool_id, identity_pool_id):
         self.region_name = region_name
         self.identity_pool_id = identity_pool_id
         self.client_id = client_id
         self.pool_id = pool_id
@@ -23,15 +27,15 @@
             resp = await cognito_identity_provider.initiate_auth(
                 AuthFlow="REFRESH_TOKEN_AUTH",
                 AuthParameters={
                     "REFRESH_TOKEN": refresh_token,
                 },
                 ClientId=self.client_id,
             )
-
+        _LOGGER.debug("Authentication response %s", resp)
         return AuthenticationTokens(resp["AuthenticationResult"])
 
     """ Gets the initial token by providing username and password. """
 
     async def get_new_token(self, username, password) -> AuthenticationTokens:
         async with self.session.client(
             "cognito-idp", region_name=self.region_name
@@ -58,15 +62,15 @@
 
             # Respond to PASSWORD_VERIFIER
             resp = await cognito_identity_provider.respond_to_auth_challenge(
                 ClientId=self.client_id,
                 ChallengeName="PASSWORD_VERIFIER",
                 ChallengeResponses=challenge_response,
             )
-
+        _LOGGER.debug("Authentication result %s", resp)
         return AuthenticationTokens(resp["AuthenticationResult"])
 
     """ Retrieves the AWS credentials to sign a request. """
 
     async def get_credentials(self, id_token) -> AwsCredentials:
         async with self.session.client(
             "cognito-identity", region_name=self.region_name
@@ -81,9 +85,9 @@
                 IdentityPoolId=self.identity_pool_id, Logins=logins
             )
 
             # Get credentials for the identity
             credentials_response = await cognito_identity.get_credentials_for_identity(
                 IdentityId=identity_response["IdentityId"], Logins=logins
             )
-
+        _LOGGER.debug("Get credentials %s", credentials_response)
         return AwsCredentials(credentials_response["Credentials"])
```

### Comparing `aioaquacell-0.1.4/aioaquacell/aws_signature_request.py` & `aioaquacell-0.1.5/aioaquacell/aws_signature_request.py`

 * *Files identical despite different names*

### Comparing `aioaquacell-0.1.4/aioaquacell.egg-info/PKG-INFO` & `aioaquacell-0.1.5/aioaquacell.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: aioaquacell
-Version: 0.1.4
+Version: 0.1.5
 Summary: Asynchronous library to retrieve details of your Aquacell water softener device
 Home-page: https://github.com/Jordi1990/aioaquacell
-Download-URL: https://github.com/Jordi1990/aioaquacell/archive/refs/tags/v0.1.4.tar.gz
+Download-URL: https://github.com/Jordi1990/aioaquacell/archive/refs/tags/v0.1.5.tar.gz
 Author: Jordi Epema
 Author-email: jordi.epema@gmail.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Aioaquacell
```

### Comparing `aioaquacell-0.1.4/setup.py` & `aioaquacell-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from setuptools import setup
 
 PROJECT_DIR = Path(__file__).parent.resolve()
 README_FILE = PROJECT_DIR / "README.md"
-VERSION = "0.1.4"
+VERSION = "0.1.5"
 
 setup(
     name="aioaquacell",
     version=VERSION,
     packages=["aioaquacell"],
     install_requires=[
         "aiohttp",
@@ -20,9 +20,9 @@
     url="https://github.com/Jordi1990/aioaquacell",
     license="Apache License 2.0",
     author="Jordi Epema",
     author_email="jordi.epema@gmail.com",
     description="Asynchronous library to retrieve details of your Aquacell water softener device",
     long_description=README_FILE.read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
-    download_url="https://github.com/Jordi1990/aioaquacell/archive/refs/tags/v0.1.4.tar.gz",
+    download_url="https://github.com/Jordi1990/aioaquacell/archive/refs/tags/v0.1.5.tar.gz",
 )
```

