# Comparing `tmp/csa_ai_foundation_model_api_clients-0.0.3.tar.gz` & `tmp/csa_ai_foundation_model_api_clients-0.0.4.tar.gz`

## Comparing `csa_ai_foundation_model_api_clients-0.0.3.tar` & `csa_ai_foundation_model_api_clients-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rwxr-xr-x   0        0        0      333 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.3/manual-package-update.md
--rwxr-xr-x   0        0        0      486 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.3/setup-venv.sh
--rwxr-xr-x   0        0        0      474 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.3/.github/workflows/release.yml
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.3/src/csa_ai_foundation_model_api_clients/__init__.py
--rwxr-xr-x   0        0        0     4081 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.3/src/csa_ai_foundation_model_api_clients/foundation_model_api_clients.py
--rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.3/src/csa_ai_foundation_model_api_clients/ai_client/__init__.py
--rwxr-xr-x   0        0        0     3023 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.3/src/csa_ai_foundation_model_api_clients/ai_client/chatgpt.py
--rwxr-xr-x   0        0        0     2515 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.3/src/csa_ai_foundation_model_api_clients/ai_client/claude.py
--rwxr-xr-x   0        0        0     1688 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.3/src/csa_ai_foundation_model_api_clients/ai_client/gemini.py
--rwxr-xr-x   0        0        0      578 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.3/tests/ask-chatgpt-the-capital-of-france.py
--rwxr-xr-x   0        0        0      580 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.3/tests/ask-claude-the-capital-of-france.py
--rwxr-xr-x   0        0        0      580 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.3/tests/ask-gemini-the-capital-of-france.py
--rwxr-xr-x   0        0        0     3078 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.3/.gitignore
--rwxr-xr-x   0        0        0    11357 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.3/LICENSE
--rwxr-xr-x   0        0        0     1418 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.3/README.md
--rwxr-xr-x   0        0        0      787 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.3/PKG-INFO
+-rwxr-xr-x   0        0        0      333 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.4/manual-package-update.md
+-rwxr-xr-x   0        0        0      486 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.4/setup-venv.sh
+-rwxr-xr-x   0        0        0      474 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.4/.github/workflows/release.yml
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.4/src/csa_ai_foundation_model_api_clients/__init__.py
+-rwxr-xr-x   0        0        0     4081 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.4/src/csa_ai_foundation_model_api_clients/foundation_model_api_clients.py
+-rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.4/src/csa_ai_foundation_model_api_clients/ai_client/__init__.py
+-rwxr-xr-x   0        0        0     3023 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.4/src/csa_ai_foundation_model_api_clients/ai_client/chatgpt.py
+-rwxr-xr-x   0        0        0     2515 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.4/src/csa_ai_foundation_model_api_clients/ai_client/claude.py
+-rwxr-xr-x   0        0        0     1688 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.4/src/csa_ai_foundation_model_api_clients/ai_client/gemini.py
+-rwxr-xr-x   0        0        0      578 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.4/tests/ask-chatgpt-the-capital-of-france.py
+-rwxr-xr-x   0        0        0      580 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.4/tests/ask-claude-the-capital-of-france.py
+-rwxr-xr-x   0        0        0      580 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.4/tests/ask-gemini-the-capital-of-france.py
+-rwxr-xr-x   0        0        0     3078 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.4/.gitignore
+-rwxr-xr-x   0        0        0    11357 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.4/LICENSE
+-rwxr-xr-x   0        0        0     1418 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.4/README.md
+-rwxr-xr-x   0        0        0      838 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.4/PKG-INFO
```

### Comparing `csa_ai_foundation_model_api_clients-0.0.3/src/csa_ai_foundation_model_api_clients/foundation_model_api_clients.py` & `csa_ai_foundation_model_api_clients-0.0.4/src/csa_ai_foundation_model_api_clients/foundation_model_api_clients.py`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.0.3/src/csa_ai_foundation_model_api_clients/ai_client/chatgpt.py` & `csa_ai_foundation_model_api_clients-0.0.4/src/csa_ai_foundation_model_api_clients/ai_client/chatgpt.py`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.0.3/src/csa_ai_foundation_model_api_clients/ai_client/claude.py` & `csa_ai_foundation_model_api_clients-0.0.4/src/csa_ai_foundation_model_api_clients/ai_client/claude.py`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.0.3/src/csa_ai_foundation_model_api_clients/ai_client/gemini.py` & `csa_ai_foundation_model_api_clients-0.0.4/src/csa_ai_foundation_model_api_clients/ai_client/gemini.py`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.0.3/tests/ask-chatgpt-the-capital-of-france.py` & `csa_ai_foundation_model_api_clients-0.0.4/tests/ask-chatgpt-the-capital-of-france.py`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.0.3/tests/ask-claude-the-capital-of-france.py` & `csa_ai_foundation_model_api_clients-0.0.4/tests/ask-claude-the-capital-of-france.py`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.0.3/tests/ask-gemini-the-capital-of-france.py` & `csa_ai_foundation_model_api_clients-0.0.4/tests/ask-gemini-the-capital-of-france.py`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.0.3/.gitignore` & `csa_ai_foundation_model_api_clients-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.0.3/LICENSE` & `csa_ai_foundation_model_api_clients-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.0.3/README.md` & `csa_ai_foundation_model_api_clients-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.0.3/pyproject.toml` & `csa_ai_foundation_model_api_clients-0.0.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "csa_ai_foundation_model_api_clients"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Kurt Seifried", email="kseifried@cloudsecurityalliance.org" },
 ]
 description = "Cloud Security Alliance AI Foundation Model API Clients"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -18,10 +18,16 @@
 ]
 dependencies = [
   "anthropic",
   "google-generativeai",
   "openai",
 ]
 
+[project.packages.find]
+where = [
+      	"src"
+]
+
+
 [project.urls]
 Homepage = "https://github.com/CloudSecurityAlliance/csa-ai-foundation-model-api-clients"
 Issues = "https://github.com/CloudSecurityAlliance/csa-ai-foundation-model-api-clients/issues"
```

### Comparing `csa_ai_foundation_model_api_clients-0.0.3/PKG-INFO` & `csa_ai_foundation_model_api_clients-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: csa_ai_foundation_model_api_clients
-Version: 0.0.3
+Version: 0.0.4
 Summary: Cloud Security Alliance AI Foundation Model API Clients
 Project-URL: Homepage, https://github.com/CloudSecurityAlliance/csa-ai-foundation-model-api-clients
 Project-URL: Issues, https://github.com/CloudSecurityAlliance/csa-ai-foundation-model-api-clients/issues
 Author-email: Kurt Seifried <kseifried@cloudsecurityalliance.org>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

