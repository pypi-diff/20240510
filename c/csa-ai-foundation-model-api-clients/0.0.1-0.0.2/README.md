# Comparing `tmp/csa_ai_foundation_model_api_clients-0.0.1.tar.gz` & `tmp/csa_ai_foundation_model_api_clients-0.0.2.tar.gz`

## Comparing `csa_ai_foundation_model_api_clients-0.0.1.tar` & `csa_ai_foundation_model_api_clients-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,22 @@
--rwxr-xr-x   0        0        0      486 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.1/setup-venv.sh
--rwxr-xr-x   0        0        0      474 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.1/.github/workflows/release.yml
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.1/src/csa_ai_foundation_model_api_clients/__init__.py
--rwxr-xr-x   0        0        0     3802 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.1/src/csa_ai_foundation_model_api_clients/foundation_model_api_clients.py
--rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.1/src/csa_ai_foundation_model_api_clients/ai_client/__init__.py
--rwxr-xr-x   0        0        0     3178 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.1/src/csa_ai_foundation_model_api_clients/ai_client/chatgpt.py
--rwxr-xr-x   0        0        0     2690 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.1/src/csa_ai_foundation_model_api_clients/ai_client/claude.py
--rwxr-xr-x   0        0        0     1879 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.1/src/csa_ai_foundation_model_api_clients/ai_client/gemini.py
--rwxr-xr-x   0        0        0     3078 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.1/.gitignore
--rwxr-xr-x   0        0        0    11357 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.1/LICENSE
--rwxr-xr-x   0        0        0      752 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.1/README.md
--rwxr-xr-x   0        0        0      716 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0      210 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/manual-package-update.md
+-rwxr-xr-x   0        0        0      486 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/setup-venv.sh
+-rwxr-xr-x   0        0        0      474 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/.github/workflows/release.yml
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/src/0.0.1/__init__.py
+-rwxr-xr-x   0        0        0     3802 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/src/0.0.1/foundation_model_api_clients.py
+-rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/src/0.0.1/ai_client/__init__.py
+-rwxr-xr-x   0        0        0     3178 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/src/0.0.1/ai_client/chatgpt.py
+-rwxr-xr-x   0        0        0     2690 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/src/0.0.1/ai_client/claude.py
+-rwxr-xr-x   0        0        0     1879 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/src/0.0.1/ai_client/gemini.py
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/src/csa_ai_foundation_model_api_clients/__init__.py
+-rwxr-xr-x   0        0        0     4081 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/src/csa_ai_foundation_model_api_clients/foundation_model_api_clients.py
+-rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/src/csa_ai_foundation_model_api_clients/ai_client/__init__.py
+-rwxr-xr-x   0        0        0     3023 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/src/csa_ai_foundation_model_api_clients/ai_client/chatgpt.py
+-rwxr-xr-x   0        0        0     2515 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/src/csa_ai_foundation_model_api_clients/ai_client/claude.py
+-rwxr-xr-x   0        0        0     1688 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/src/csa_ai_foundation_model_api_clients/ai_client/gemini.py
+-rwxr-xr-x   0        0        0      574 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/tests/ask-claude-the-capital-of-france.py
+-rwxr-xr-x   0        0        0      568 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/tests/ask-claude-the-capital-of-france.py~
+-rwxr-xr-x   0        0        0     3078 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/.gitignore
+-rwxr-xr-x   0        0        0    11357 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/LICENSE
+-rwxr-xr-x   0        0        0      752 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/README.md
+-rwxr-xr-x   0        0        0      716 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.2/PKG-INFO
```

### Comparing `csa_ai_foundation_model_api_clients-0.0.1/src/csa_ai_foundation_model_api_clients/foundation_model_api_clients.py` & `csa_ai_foundation_model_api_clients-0.0.2/src/0.0.1/foundation_model_api_clients.py`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.0.1/src/csa_ai_foundation_model_api_clients/ai_client/chatgpt.py` & `csa_ai_foundation_model_api_clients-0.0.2/src/0.0.1/ai_client/chatgpt.py`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.0.1/src/csa_ai_foundation_model_api_clients/ai_client/claude.py` & `csa_ai_foundation_model_api_clients-0.0.2/src/0.0.1/ai_client/claude.py`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.0.1/src/csa_ai_foundation_model_api_clients/ai_client/gemini.py` & `csa_ai_foundation_model_api_clients-0.0.2/src/0.0.1/ai_client/gemini.py`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.0.1/.gitignore` & `csa_ai_foundation_model_api_clients-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.0.1/LICENSE` & `csa_ai_foundation_model_api_clients-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.0.1/README.md` & `csa_ai_foundation_model_api_clients-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.0.1/pyproject.toml` & `csa_ai_foundation_model_api_clients-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "csa_ai_foundation_model_api_clients"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Kurt Seifried", email="kseifried@cloudsecurityalliance.org" },
 ]
 description = "Cloud Security Alliance AI Foundation Model API Clients"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `csa_ai_foundation_model_api_clients-0.0.1/PKG-INFO` & `csa_ai_foundation_model_api_clients-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: csa_ai_foundation_model_api_clients
-Version: 0.0.1
+Version: 0.0.2
 Summary: Cloud Security Alliance AI Foundation Model API Clients
 Project-URL: Homepage, https://github.com/CloudSecurityAlliance/csa-ai-foundation-model-api-clients
 Project-URL: Issues, https://github.com/CloudSecurityAlliance/csa-ai-foundation-model-api-clients/issues
 Author-email: Kurt Seifried <kseifried@cloudsecurityalliance.org>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

