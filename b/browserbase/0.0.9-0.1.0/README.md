# Comparing `tmp/browserbase-0.0.9.tar.gz` & `tmp/browserbase-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "browserbase-0.0.9.tar", last modified: Fri Apr 19 10:54:26 2024, max compression
+gzip compressed data, was "browserbase-0.1.0.tar", last modified: Fri May 10 12:23:01 2024, max compression
```

## Comparing `browserbase-0.0.9.tar` & `browserbase-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-04-19 10:54:26.814656 browserbase-0.0.9/
--rw-r--r--   0 mish       (501) staff       (20)     1064 2024-04-09 17:45:47.000000 browserbase-0.0.9/LICENSE
--rw-r--r--   0 mish       (501) staff       (20)     1524 2024-04-19 10:54:26.814443 browserbase-0.0.9/PKG-INFO
--rw-r--r--   0 mish       (501) staff       (20)      942 2024-04-19 10:53:32.000000 browserbase-0.0.9/README.md
-drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-04-19 10:54:26.812392 browserbase-0.0.9/browserbase/
--rw-r--r--   0 mish       (501) staff       (20)     3186 2024-04-18 21:05:58.000000 browserbase-0.0.9/browserbase/__init__.py
-drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-04-19 10:54:26.813836 browserbase-0.0.9/browserbase/helpers/
--rw-r--r--   0 mish       (501) staff       (20)      301 2024-04-16 18:32:01.000000 browserbase-0.0.9/browserbase/helpers/anthropic.py
--rw-r--r--   0 mish       (501) staff       (20)      503 2024-04-15 12:54:51.000000 browserbase-0.0.9/browserbase/helpers/gpt4.py
-drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-04-19 10:54:26.814180 browserbase-0.0.9/browserbase.egg-info/
--rw-r--r--   0 mish       (501) staff       (20)     1524 2024-04-19 10:54:26.000000 browserbase-0.0.9/browserbase.egg-info/PKG-INFO
--rw-r--r--   0 mish       (501) staff       (20)      291 2024-04-19 10:54:26.000000 browserbase-0.0.9/browserbase.egg-info/SOURCES.txt
--rw-r--r--   0 mish       (501) staff       (20)        1 2024-04-19 10:54:26.000000 browserbase-0.0.9/browserbase.egg-info/dependency_links.txt
--rw-r--r--   0 mish       (501) staff       (20)       19 2024-04-19 10:54:26.000000 browserbase-0.0.9/browserbase.egg-info/requires.txt
--rw-r--r--   0 mish       (501) staff       (20)       12 2024-04-19 10:54:26.000000 browserbase-0.0.9/browserbase.egg-info/top_level.txt
--rw-r--r--   0 mish       (501) staff       (20)      653 2024-04-19 10:54:21.000000 browserbase-0.0.9/pyproject.toml
--rw-r--r--   0 mish       (501) staff       (20)       38 2024-04-19 10:54:26.816197 browserbase-0.0.9/setup.cfg
+drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-10 12:23:01.816158 browserbase-0.1.0/
+-rw-r--r--   0 mish       (501) staff       (20)     1064 2024-04-09 17:45:47.000000 browserbase-0.1.0/LICENSE
+-rw-r--r--   0 mish       (501) staff       (20)     1575 2024-05-10 12:23:01.815942 browserbase-0.1.0/PKG-INFO
+-rw-r--r--   0 mish       (501) staff       (20)      933 2024-04-19 10:57:22.000000 browserbase-0.1.0/README.md
+drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-10 12:23:01.814439 browserbase-0.1.0/browserbase/
+-rw-r--r--   0 mish       (501) staff       (20)    11429 2024-05-10 12:20:14.000000 browserbase-0.1.0/browserbase/__init__.py
+drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-10 12:23:01.815550 browserbase-0.1.0/browserbase/helpers/
+-rw-r--r--   0 mish       (501) staff       (20)      301 2024-04-16 18:32:01.000000 browserbase-0.1.0/browserbase/helpers/anthropic.py
+-rw-r--r--   0 mish       (501) staff       (20)      503 2024-04-15 12:54:51.000000 browserbase-0.1.0/browserbase/helpers/gpt4.py
+drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-10 12:23:01.815726 browserbase-0.1.0/browserbase.egg-info/
+-rw-r--r--   0 mish       (501) staff       (20)     1575 2024-05-10 12:23:01.000000 browserbase-0.1.0/browserbase.egg-info/PKG-INFO
+-rw-r--r--   0 mish       (501) staff       (20)      291 2024-05-10 12:23:01.000000 browserbase-0.1.0/browserbase.egg-info/SOURCES.txt
+-rw-r--r--   0 mish       (501) staff       (20)        1 2024-05-10 12:23:01.000000 browserbase-0.1.0/browserbase.egg-info/dependency_links.txt
+-rw-r--r--   0 mish       (501) staff       (20)       49 2024-05-10 12:23:01.000000 browserbase-0.1.0/browserbase.egg-info/requires.txt
+-rw-r--r--   0 mish       (501) staff       (20)       12 2024-05-10 12:23:01.000000 browserbase-0.1.0/browserbase.egg-info/top_level.txt
+-rw-r--r--   0 mish       (501) staff       (20)      697 2024-05-10 12:22:32.000000 browserbase-0.1.0/pyproject.toml
+-rw-r--r--   0 mish       (501) staff       (20)       38 2024-05-10 12:23:01.816203 browserbase-0.1.0/setup.cfg
```

### Comparing `browserbase-0.0.9/LICENSE` & `browserbase-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `browserbase-0.0.9/PKG-INFO` & `browserbase-0.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
 Name: browserbase
-Version: 0.0.9
+Version: 0.1.0
 Summary: Browserbase Python SDK
 Author-email: Browserbase <info@browserbase.com>
 Project-URL: Homepage, https://browserbase.com
 Project-URL: Source, https://github.com/browserbase/python-sdk
 Project-URL: Issues, https://github.com/browserbase/python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: playwright>=1.43.0
+Requires-Dist: pydantic>=2.7.1
+Requires-Dist: httpx>=0.27.0
 
 # Browserbase Python SDK
 
 [Browserbase](https://browserbase.com) is a serverless platform for running headless browsers, it offers advanced debugging, session recordings, stealth mode, integrated proxies and captcha solving.
 
 ## Installation and setup
 
 - Get an API key from [browserbase.com](https://browserbase.com) and set it in environment variables (`BROWSERBASE_API_KEY`).
 - Install the required dependencies:
 
 ```
-pip install browserbase-haystack
+pip install browserbase
 ```
 
 ## Usage
 
 ```py
 from browserbase import Browserbase
```

### Comparing `browserbase-0.0.9/README.md` & `browserbase-0.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ## Installation and setup
 
 - Get an API key from [browserbase.com](https://browserbase.com) and set it in environment variables (`BROWSERBASE_API_KEY`).
 - Install the required dependencies:
 
 ```
-pip install browserbase-haystack
+pip install browserbase
 ```
 
 ## Usage
 
 ```py
 from browserbase import Browserbase
```

### Comparing `browserbase-0.0.9/browserbase.egg-info/PKG-INFO` & `browserbase-0.1.0/browserbase.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
 Name: browserbase
-Version: 0.0.9
+Version: 0.1.0
 Summary: Browserbase Python SDK
 Author-email: Browserbase <info@browserbase.com>
 Project-URL: Homepage, https://browserbase.com
 Project-URL: Source, https://github.com/browserbase/python-sdk
 Project-URL: Issues, https://github.com/browserbase/python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: playwright>=1.43.0
+Requires-Dist: pydantic>=2.7.1
+Requires-Dist: httpx>=0.27.0
 
 # Browserbase Python SDK
 
 [Browserbase](https://browserbase.com) is a serverless platform for running headless browsers, it offers advanced debugging, session recordings, stealth mode, integrated proxies and captcha solving.
 
 ## Installation and setup
 
 - Get an API key from [browserbase.com](https://browserbase.com) and set it in environment variables (`BROWSERBASE_API_KEY`).
 - Install the required dependencies:
 
 ```
-pip install browserbase-haystack
+pip install browserbase
 ```
 
 ## Usage
 
 ```py
 from browserbase import Browserbase
```

### Comparing `browserbase-0.0.9/pyproject.toml` & `browserbase-0.1.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [project]
 name = "browserbase"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
   { name="Browserbase", email="info@browserbase.com" },
 ]
 description = "Browserbase Python SDK"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
-  "playwright >= 1.43.0"
+  "playwright >= 1.43.0",
+  "pydantic >= 2.7.1",
+  "httpx >= 0.27.0"
 ]
 
 [project.urls]
 Homepage = "https://browserbase.com"
 Source = "https://github.com/browserbase/python-sdk"
 Issues = "https://github.com/browserbase/python-sdk/issues"
```

