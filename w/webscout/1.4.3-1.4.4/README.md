# Comparing `tmp/webscout-1.4.3.tar.gz` & `tmp/webscout-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscout-1.4.3.tar", last modified: Wed May  8 15:50:22 2024, max compression
+gzip compressed data, was "webscout-1.4.4.tar", last modified: Fri May 10 02:44:01 2024, max compression
```

## Comparing `webscout-1.4.3.tar` & `webscout-1.4.4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 15:50:22.372252 webscout-1.4.3/
-drwxrwxrwx   0        0        0        0 2024-05-08 15:50:21.768551 webscout-1.4.3/DeepWEBS/
--rw-rw-rw-   0        0        0        0 2024-05-04 05:22:54.000000 webscout-1.4.3/DeepWEBS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 15:50:21.800794 webscout-1.4.3/DeepWEBS/documents/
--rw-rw-rw-   0        0        0        0 2024-05-04 05:22:54.000000 webscout-1.4.3/DeepWEBS/documents/__init__.py
--rw-rw-rw-   0        0        0     4049 2024-05-04 05:22:54.000000 webscout-1.4.3/DeepWEBS/documents/query_results_extractor.py
--rw-rw-rw-   0        0        0     5272 2024-05-04 05:22:54.000000 webscout-1.4.3/DeepWEBS/documents/webpage_content_extractor.py
-drwxrwxrwx   0        0        0        0 2024-05-08 15:50:21.838069 webscout-1.4.3/DeepWEBS/networks/
--rw-rw-rw-   0        0        0        0 2024-05-04 05:22:54.000000 webscout-1.4.3/DeepWEBS/networks/__init__.py
--rw-rw-rw-   0        0        0     3183 2024-05-04 05:22:54.000000 webscout-1.4.3/DeepWEBS/networks/filepath_converter.py
--rw-rw-rw-   0        0        0     1966 2024-05-04 05:22:54.000000 webscout-1.4.3/DeepWEBS/networks/google_searcher.py
--rw-rw-rw-   0        0        0      726 2024-05-04 05:22:54.000000 webscout-1.4.3/DeepWEBS/networks/network_configs.py
--rw-rw-rw-   0        0        0     3590 2024-05-04 05:22:54.000000 webscout-1.4.3/DeepWEBS/networks/webpage_fetcher.py
-drwxrwxrwx   0        0        0        0 2024-05-08 15:50:21.917049 webscout-1.4.3/DeepWEBS/utilsdw/
--rw-rw-rw-   0        0        0        0 2024-05-04 05:22:54.000000 webscout-1.4.3/DeepWEBS/utilsdw/__init__.py
--rw-rw-rw-   0        0        0     2472 2024-05-04 05:22:54.000000 webscout-1.4.3/DeepWEBS/utilsdw/enver.py
--rw-rw-rw-   0        0        0     8174 2024-05-04 05:22:54.000000 webscout-1.4.3/DeepWEBS/utilsdw/logger.py
--rw-rw-rw-   0        0        0     3150 2024-05-04 05:22:54.000000 webscout-1.4.3/LICENSE.md
--rw-rw-rw-   0        0        0    40456 2024-05-08 15:50:22.345375 webscout-1.4.3/PKG-INFO
--rw-rw-rw-   0        0        0    38155 2024-05-08 15:02:08.000000 webscout-1.4.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-08 15:50:22.372252 webscout-1.4.3/setup.cfg
--rw-rw-rw-   0        0        0     2800 2024-05-08 15:49:40.000000 webscout-1.4.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-08 15:50:22.266898 webscout-1.4.3/webscout/
--rw-rw-rw-   0        0        0   215473 2024-05-08 14:44:29.000000 webscout-1.4.3/webscout/AI.py
--rw-rw-rw-   0        0        0     4710 2024-05-04 05:22:54.000000 webscout-1.4.3/webscout/AIbase.py
--rw-rw-rw-   0        0        0    33159 2024-05-08 14:46:11.000000 webscout-1.4.3/webscout/AIutel.py
--rw-rw-rw-   0        0        0     7332 2024-05-04 05:22:54.000000 webscout-1.4.3/webscout/DWEBS.py
--rw-rw-rw-   0        0        0     1910 2024-05-04 05:22:54.000000 webscout-1.4.3/webscout/LLM.py
--rw-rw-rw-   0        0        0     1073 2024-05-08 14:46:32.000000 webscout-1.4.3/webscout/__init__.py
--rw-rw-rw-   0        0        0      126 2024-05-04 05:22:54.000000 webscout-1.4.3/webscout/__main__.py
--rw-rw-rw-   0        0        0      971 2024-05-04 05:22:54.000000 webscout-1.4.3/webscout/async_providers.py
--rw-rw-rw-   0        0        0    17059 2024-05-04 05:22:54.000000 webscout-1.4.3/webscout/cli.py
--rw-rw-rw-   0        0        0      378 2024-05-04 05:22:54.000000 webscout-1.4.3/webscout/exceptions.py
--rw-rw-rw-   0        0        0    24489 2024-05-08 03:37:35.000000 webscout-1.4.3/webscout/g4f.py
--rw-rw-rw-   0        0        0      692 2024-05-04 05:22:54.000000 webscout-1.4.3/webscout/models.py
--rw-rw-rw-   0        0        0     5896 2024-05-04 10:19:38.000000 webscout-1.4.3/webscout/tempid.py
--rw-rw-rw-   0        0        0    20622 2024-05-04 05:22:54.000000 webscout-1.4.3/webscout/transcriber.py
--rw-rw-rw-   0        0        0     2605 2024-05-04 05:22:54.000000 webscout-1.4.3/webscout/utils.py
--rw-rw-rw-   0        0        0       25 2024-05-08 15:50:01.000000 webscout-1.4.3/webscout/version.py
--rw-rw-rw-   0        0        0      967 2024-05-04 05:22:54.000000 webscout-1.4.3/webscout/voice.py
--rw-rw-rw-   0        0        0    82281 2024-05-08 14:52:22.000000 webscout-1.4.3/webscout/webai.py
--rw-rw-rw-   0        0        0     3085 2024-05-04 05:22:54.000000 webscout-1.4.3/webscout/webscout_search.py
--rw-rw-rw-   0        0        0    40670 2024-05-04 05:22:54.000000 webscout-1.4.3/webscout/webscout_search_async.py
-drwxrwxrwx   0        0        0        0 2024-05-08 15:50:22.337356 webscout-1.4.3/webscout.egg-info/
--rw-rw-rw-   0        0        0    40456 2024-05-08 15:50:20.000000 webscout-1.4.3/webscout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1042 2024-05-08 15:50:21.000000 webscout-1.4.3/webscout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 15:50:20.000000 webscout-1.4.3/webscout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      197 2024-05-08 15:50:20.000000 webscout-1.4.3/webscout.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      379 2024-05-08 15:50:20.000000 webscout-1.4.3/webscout.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-08 15:50:20.000000 webscout-1.4.3/webscout.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 02:44:01.315008 webscout-1.4.4/
+drwxrwxrwx   0        0        0        0 2024-05-10 02:43:59.854618 webscout-1.4.4/DeepWEBS/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-1.4.4/DeepWEBS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 02:43:59.869629 webscout-1.4.4/DeepWEBS/documents/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-1.4.4/DeepWEBS/documents/__init__.py
+-rw-rw-rw-   0        0        0     4049 2024-05-08 15:52:48.000000 webscout-1.4.4/DeepWEBS/documents/query_results_extractor.py
+-rw-rw-rw-   0        0        0     5272 2024-05-08 15:52:48.000000 webscout-1.4.4/DeepWEBS/documents/webpage_content_extractor.py
+drwxrwxrwx   0        0        0        0 2024-05-10 02:43:59.967230 webscout-1.4.4/DeepWEBS/networks/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-1.4.4/DeepWEBS/networks/__init__.py
+-rw-rw-rw-   0        0        0     3183 2024-05-08 15:52:48.000000 webscout-1.4.4/DeepWEBS/networks/filepath_converter.py
+-rw-rw-rw-   0        0        0     1966 2024-05-08 15:52:48.000000 webscout-1.4.4/DeepWEBS/networks/google_searcher.py
+-rw-rw-rw-   0        0        0      726 2024-05-08 15:52:48.000000 webscout-1.4.4/DeepWEBS/networks/network_configs.py
+-rw-rw-rw-   0        0        0     3590 2024-05-08 15:52:48.000000 webscout-1.4.4/DeepWEBS/networks/webpage_fetcher.py
+drwxrwxrwx   0        0        0        0 2024-05-10 02:43:59.988225 webscout-1.4.4/DeepWEBS/utilsdw/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-1.4.4/DeepWEBS/utilsdw/__init__.py
+-rw-rw-rw-   0        0        0     2472 2024-05-08 15:52:48.000000 webscout-1.4.4/DeepWEBS/utilsdw/enver.py
+-rw-rw-rw-   0        0        0     8174 2024-05-08 15:52:48.000000 webscout-1.4.4/DeepWEBS/utilsdw/logger.py
+-rw-rw-rw-   0        0        0     3150 2024-05-08 15:52:48.000000 webscout-1.4.4/LICENSE.md
+-rw-rw-rw-   0        0        0    43415 2024-05-10 02:44:01.311375 webscout-1.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0    41114 2024-05-10 02:21:13.000000 webscout-1.4.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-10 02:44:01.316036 webscout-1.4.4/setup.cfg
+-rw-rw-rw-   0        0        0     2800 2024-05-10 02:22:02.000000 webscout-1.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 02:44:00.570905 webscout-1.4.4/webscout/
+-rw-rw-rw-   0        0        0   226145 2024-05-09 17:13:40.000000 webscout-1.4.4/webscout/AI.py
+-rw-rw-rw-   0        0        0     4710 2024-05-08 15:52:48.000000 webscout-1.4.4/webscout/AIbase.py
+-rw-rw-rw-   0        0        0    33217 2024-05-09 17:15:58.000000 webscout-1.4.4/webscout/AIutel.py
+-rw-rw-rw-   0        0        0     7332 2024-05-08 15:52:48.000000 webscout-1.4.4/webscout/DWEBS.py
+-rw-rw-rw-   0        0        0     1910 2024-05-08 15:52:48.000000 webscout-1.4.4/webscout/LLM.py
+-rw-rw-rw-   0        0        0     1090 2024-05-09 17:15:47.000000 webscout-1.4.4/webscout/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-05-08 15:52:48.000000 webscout-1.4.4/webscout/__main__.py
+-rw-rw-rw-   0        0        0      971 2024-05-08 15:52:48.000000 webscout-1.4.4/webscout/async_providers.py
+-rw-rw-rw-   0        0        0    17059 2024-05-08 15:52:48.000000 webscout-1.4.4/webscout/cli.py
+-rw-rw-rw-   0        0        0      378 2024-05-08 15:52:48.000000 webscout-1.4.4/webscout/exceptions.py
+-rw-rw-rw-   0        0        0    24489 2024-05-08 15:52:48.000000 webscout-1.4.4/webscout/g4f.py
+-rw-rw-rw-   0        0        0      692 2024-05-08 15:52:48.000000 webscout-1.4.4/webscout/models.py
+-rw-rw-rw-   0        0        0     5896 2024-05-08 15:52:48.000000 webscout-1.4.4/webscout/tempid.py
+-rw-rw-rw-   0        0        0    20622 2024-05-08 15:52:48.000000 webscout-1.4.4/webscout/transcriber.py
+-rw-rw-rw-   0        0        0     2603 2024-05-09 03:33:11.000000 webscout-1.4.4/webscout/utils.py
+-rw-rw-rw-   0        0        0       25 2024-05-10 02:22:14.000000 webscout-1.4.4/webscout/version.py
+-rw-rw-rw-   0        0        0      967 2024-05-08 15:52:48.000000 webscout-1.4.4/webscout/voice.py
+-rw-rw-rw-   0        0        0    82831 2024-05-09 17:15:32.000000 webscout-1.4.4/webscout/webai.py
+-rw-rw-rw-   0        0        0     3085 2024-05-08 15:52:48.000000 webscout-1.4.4/webscout/webscout_search.py
+-rw-rw-rw-   0        0        0    40670 2024-05-08 15:52:48.000000 webscout-1.4.4/webscout/webscout_search_async.py
+drwxrwxrwx   0        0        0        0 2024-05-10 02:44:01.302466 webscout-1.4.4/webscout.egg-info/
+-rw-rw-rw-   0        0        0    43415 2024-05-10 02:43:57.000000 webscout-1.4.4/webscout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1042 2024-05-10 02:43:58.000000 webscout-1.4.4/webscout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 02:43:57.000000 webscout-1.4.4/webscout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      197 2024-05-10 02:43:57.000000 webscout-1.4.4/webscout.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      379 2024-05-10 02:43:57.000000 webscout-1.4.4/webscout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-10 02:43:57.000000 webscout-1.4.4/webscout.egg-info/top_level.txt
```

### Comparing `webscout-1.4.3/DeepWEBS/documents/query_results_extractor.py` & `webscout-1.4.4/DeepWEBS/documents/query_results_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.3/DeepWEBS/documents/webpage_content_extractor.py` & `webscout-1.4.4/DeepWEBS/documents/webpage_content_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.3/DeepWEBS/networks/filepath_converter.py` & `webscout-1.4.4/DeepWEBS/networks/filepath_converter.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.3/DeepWEBS/networks/google_searcher.py` & `webscout-1.4.4/DeepWEBS/networks/google_searcher.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.3/DeepWEBS/networks/network_configs.py` & `webscout-1.4.4/DeepWEBS/networks/network_configs.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.3/DeepWEBS/networks/webpage_fetcher.py` & `webscout-1.4.4/DeepWEBS/networks/webpage_fetcher.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.3/DeepWEBS/utilsdw/enver.py` & `webscout-1.4.4/DeepWEBS/utilsdw/enver.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.3/DeepWEBS/utilsdw/logger.py` & `webscout-1.4.4/DeepWEBS/utilsdw/logger.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.3/LICENSE.md` & `webscout-1.4.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `webscout-1.4.3/PKG-INFO` & `webscout-1.4.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,74 +1,40 @@
-Metadata-Version: 2.1
-Name: webscout
-Version: 1.4.3
-Summary: Search for anything using the Google, DuckDuckGo, phind.com. Also containes AI models, can transcribe yt videos, temporary email and phone number generation, have TTS support and webai(terminal gpt and open interpeter)
-Author: OEvortex
-Author-email: helpingai5@gmail.com
-License: HelpingAI Simplified Universal License
-Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
-Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
-Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
-Project-URL: YouTube, https://youtube.com/@OEvortex
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: Other/Proprietary License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: docstring_inheritance>=2.1.2
-Requires-Dist: click>=8.1.7
-Requires-Dist: curl_cffi>=0.6.0b7
-Requires-Dist: lxml>=5.1.0
-Requires-Dist: nest-asyncio>=1.6.0
-Requires-Dist: selenium>=4.1.3
-Requires-Dist: tqdm>=4.64.0
-Requires-Dist: webdriver-manager>=3.5.4
-Requires-Dist: halo>=0.0.31
-Requires-Dist: g4f>=0.2.2.3
-Requires-Dist: rich
-Requires-Dist: python-dotenv
-Requires-Dist: Helpingai-T2
-Requires-Dist: beautifulsoup4
-Requires-Dist: markdownify
-Requires-Dist: pydantic
-Requires-Dist: requests
-Requires-Dist: sse_starlette
-Requires-Dist: termcolor
-Requires-Dist: tiktoken
-Requires-Dist: tldextract
-Requires-Dist: orjson
-Requires-Dist: PyYAML
-Requires-Dist: appdirs
-Requires-Dist: GoogleBard1>=2.1.4
-Requires-Dist: tls_client
-Provides-Extra: dev
-Requires-Dist: ruff>=0.1.6; extra == "dev"
-Requires-Dist: pytest>=7.4.2; extra == "dev"
+<div align="center">
+  <!-- Replace `#` with your actual links -->
+  <a href="https://t.me/devsdocode"><img alt="Telegram" src="https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white"></a>
+  <a href="https://www.instagram.com/sree.shades_/"><img alt="Instagram" src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white"></a>
+  <a href="https://www.linkedin.com/in/developer-sreejan/"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a>
+  <a href="https://buymeacoffee.com/devsdocode"><img alt="Buy Me A Coffee" src="https://img.shields.io/badge/Buy%20Me%20A%20Coffee-FFDD00?style=for-the-badge&logo=buymeacoffee&logoColor=black"></a>
+</div>
+
+<div align="center">
+  <!-- Replace `#` with your actual links -->
+  <a href="https://youtube.com/@@OEvortex">&#10148; Vortex's YouTube Channel</a>
+  </div>
+<div align="center">
+  <a href="https://youtube.com/@devsdocode">&#10148; Devs Do Code's YouTube Channel</a>
+</div>
+
 
-#  webscout
-<p align="center">
 
+  
+# WEBSCOUT
+</div>
+<p align="center">
+<div align="center">
+  <img src="https://img.shields.io/badge/WebScout-API-blue?style=for-the-badge&logo=WebScout" alt="WebScout API Badge">
+</div>
 <a href="#"><img alt="Python version" src="https://img.shields.io/pypi/pyversions/webscout"/></a>
 <a href="https://pepy.tech/project/webscout"><img alt="Downloads" src="https://static.pepy.tech/badge/webscout"></a>
 
 Search for anything using the Google, DuckDuckGo, phind.com. Also containes AI models, can transcribe yt videos, temporary email and phone number generation, have TTS support and webai(terminal gpt and open interpeter)
 
 
 ## Table of Contents
-- [webscout](#webscout)
+- [WEBSCOUT](#webscout)
   - [Table of Contents](#table-of-contents)
   - [Install](#install)
   - [CLI version](#cli-version)
   - [CLI to use LLM](#cli-to-use-llm)
   - [Regions](#regions)
   - [Tempmail and Temp number](#tempmail-and-temp-number)
     - [Temp number](#temp-number)
@@ -101,14 +67,15 @@
     - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---searchchat-with-blackbox)
     - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---search-with-perplexity)
     - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-with-opengpt)
     - [9. `KOBOLDIA` -](#9-koboldia--)
     - [10. `Reka` - chat with reka](#10-reka---chat-with-reka)
     - [11. `Cohere` - chat with cohere](#11-cohere---chat-with-cohere)
     - [12. `Xjai` - chat with free gpt 3.5](#12-xjai---chat-with-free-gpt-35)
+    - [`ThinkAny` - AI search engine](#thinkany---ai-search-engine)
     - [`LLM`](#llm)
     - [`LLM` with internet](#llm-with-internet)
     - [LLM with deepwebs](#llm-with-deepwebs)
   - [`Webai` - terminal gpt and a open interpeter](#webai---terminal-gpt-and-a-open-interpeter)
 
 ## Install
 ```python
@@ -786,15 +753,15 @@
 response = perplexity.chat(prompt)
 print(response)
 ```
 ### 8. `OpenGPT` - chat With OPENGPT
 ```python
 from webscout.AI import OPENGPT
 
-opengpt = OPENGPT(is_conversation=True, max_tokens=8000, timeout=30)
+opengpt = OPENGPT(is_conversation=True, max_tokens=8000, timeout=30, assistant_id="bca37014-6f97-4f2b-8928-81ea8d478d88")
 while True:
     # Prompt the user for input
     prompt = input("Enter your prompt: ")
     # Send the prompt to the OPENGPT model and print the response
     response_str = opengpt.chat(prompt)
     print(response_str)
 ```
@@ -858,15 +825,39 @@
 )
 
 prompt = "Tell me about india"
 
 response = ai.chat(prompt)
 print(response)
 ```
+### `ThinkAny` - AI search engine
+```python
+from webscout.AI import ThinkAnyAI
+
+ai = ThinkAnyAI(
+    is_conversation=True,
+    max_tokens=800,
+    timeout=30,
+    intro=None,
+    filepath=None,
+    update_file=True,
+    proxies={},
+    history_offset=10250,
+    act=None,
+    web_search=False,
+)
+
+prompt = "what is meaning of life"
 
+response = ai.ask(prompt)
+
+# Extract and print the message from the response
+message = ai.get_message(response)
+print(message)
+```
 ### `LLM` 
 ```python
 from webscout.LLM import LLM
 
 # Read the system message from the file
 with open('system.txt', 'r') as file:
     system_message = file.read()
@@ -1089,7 +1080,25 @@
     user_prompt = input("Enter your prompt: ")
     use_rawdog_with_webai(user_prompt)
 
 ```
 ```shell
 python -m webscout.webai webai --provider "phind" --rawdog
 ```
+
+<div align="center">
+  <!-- Replace `#` with your actual links -->
+  <a href="https://t.me/devsdocode"><img alt="Telegram" src="https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white"></a>
+  <a href="https://www.instagram.com/sree.shades_/"><img alt="Instagram" src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white"></a>
+  <a href="https://www.linkedin.com/in/developer-sreejan/"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a>
+  <a href="https://buymeacoffee.com/devsdocode"><img alt="Buy Me A Coffee" src="https://img.shields.io/badge/Buy%20Me%20A%20Coffee-FFDD00?style=for-the-badge&logo=buymeacoffee&logoColor=black"></a>
+</div>
+
+<div align="center">
+  <!-- Replace `#` with your actual links -->
+  <a href="https://youtube.com/@@OEvortex">&#10148; Vortex's YouTube Channel</a>
+  </div>
+<div align="center">
+  <a href="https://youtube.com/@devsdocode">&#10148; Devs Do Code's YouTube Channel</a>
+</div>
+
+
```

#### html2text {}

```diff
@@ -1,42 +1,16 @@
-Metadata-Version: 2.1 Name: webscout Version: 1.4.3 Summary: Search for
-anything using the Google, DuckDuckGo, phind.com. Also containes AI models, can
-transcribe yt videos, temporary email and phone number generation, have TTS
-support and webai(terminal gpt and open interpeter) Author: OEvortex Author-
-email: helpingai5@gmail.com License: HelpingAI Simplified Universal License
-Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
-Project-URL: Source, https://github.com/OE-LUCIFER/Webscout Project-URL:
-Tracker, https://github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube,
-https://youtube.com/@OEvortex Classifier: Development Status :: 5 - Production/
-Stable Classifier: Intended Audience :: Developers Classifier: License ::
-Other/Proprietary License Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search Classifier: Topic
-:: Software Development :: Libraries :: Python Modules Description-Content-
-Type: text/markdown License-File: LICENSE.md Requires-Dist:
-docstring_inheritance>=2.1.2 Requires-Dist: click>=8.1.7 Requires-Dist:
-curl_cffi>=0.6.0b7 Requires-Dist: lxml>=5.1.0 Requires-Dist: nest-
-asyncio>=1.6.0 Requires-Dist: selenium>=4.1.3 Requires-Dist: tqdm>=4.64.0
-Requires-Dist: webdriver-manager>=3.5.4 Requires-Dist: halo>=0.0.31 Requires-
-Dist: g4f>=0.2.2.3 Requires-Dist: rich Requires-Dist: python-dotenv Requires-
-Dist: Helpingai-T2 Requires-Dist: beautifulsoup4 Requires-Dist: markdownify
-Requires-Dist: pydantic Requires-Dist: requests Requires-Dist: sse_starlette
-Requires-Dist: termcolor Requires-Dist: tiktoken Requires-Dist: tldextract
-Requires-Dist: orjson Requires-Dist: PyYAML Requires-Dist: appdirs Requires-
-Dist: GoogleBard1>=2.1.4 Requires-Dist: tls_client Provides-Extra: dev
-Requires-Dist: ruff>=0.1.6; extra == "dev" Requires-Dist: pytest>=7.4.2; extra
-== "dev" # webscout
+               _[_T_e_l_e_g_r_a_m_]_[_I_n_s_t_a_g_r_a_m_]_[_L_i_n_k_e_d_I_n_]_[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
+                          _➤_ _V_o_r_t_e_x_'_s_ _Y_o_u_T_u_b_e_ _C_h_a_n_n_e_l
+                       _➤_ _D_e_v_s_ _D_o_ _C_o_d_e_'_s_ _Y_o_u_T_u_b_e_ _C_h_a_n_n_e_l
+# WEBSCOUT
+                             [WebScout API Badge]
  _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]Search for anything using the Google, DuckDuckGo,
 phind.com. Also containes AI models, can transcribe yt videos, temporary email
  and phone number generation, have TTS support and webai(terminal gpt and open
-interpeter) ## Table of Contents - [webscout](#webscout) - [Table of Contents]
+interpeter) ## Table of Contents - [WEBSCOUT](#webscout) - [Table of Contents]
 (#table-of-contents) - [Install](#install) - [CLI version](#cli-version) - [CLI
 to use LLM](#cli-to-use-llm) - [Regions](#regions) - [Tempmail and Temp number]
     (#tempmail-and-temp-number) - [Temp number](#temp-number) - [Tempmail]
  (#tempmail) - [Transcriber](#transcriber) - [DeepWEBS: Advanced Web Searches]
 (#deepwebs-advanced-web-searches) - [Activating DeepWEBS](#activating-deepwebs)
 - [Point to remember before using `DeepWEBS`](#point-to-remember-before-using-
    deepwebs) - [Usage Example](#usage-example) - [Text-to-Speech:](#text-to-
@@ -63,87 +37,87 @@
 gemini) - [5. `Prodia` - make image using prodia](#5-prodia---make-image-using-
 prodia) - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---searchchat-
  with-blackbox) - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---
 search-with-perplexity) - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-
   with-opengpt) - [9. `KOBOLDIA` -](#9-koboldia--) - [10. `Reka` - chat with
    reka](#10-reka---chat-with-reka) - [11. `Cohere` - chat with cohere](#11-
 cohere---chat-with-cohere) - [12. `Xjai` - chat with free gpt 3.5](#12-xjai---
-   chat-with-free-gpt-35) - [`LLM`](#llm) - [`LLM` with internet](#llm-with-
- internet) - [LLM with deepwebs](#llm-with-deepwebs) - [`Webai` - terminal gpt
-and a open interpeter](#webai---terminal-gpt-and-a-open-interpeter) ## Install
-   ```python pip install -U webscout ``` ## CLI version ```python3 python -
-m webscout --help ``` | Command | Description | |------------------------------
--------------|-----------------------------------------------------------------
---------------------------------------| | python -m webscout answers -k Text |
-    CLI function to perform an answers search using Webscout. | | python -
-  m webscout images -k Text | CLI function to perform an images search using
-Webscout. | | python -m webscout maps -k Text | CLI function to perform a maps
- search using Webscout. | | python -m webscout news -k Text | CLI function to
-  perform a news search using Webscout. | | python -m webscout suggestions -
-   k Text | CLI function to perform a suggestions search using Webscout. | |
- python -m webscout text -k Text | CLI function to perform a text search using
- Webscout. | | python -m webscout translate -k Text | CLI function to perform
-   translate using Webscout. | | python -m webscout version | A command-line
-   interface command that prints and returns the version of the program. | |
-  python -m webscout videos -k Text | CLI function to perform a videos search
-  using DuckDuckGo API. | ## CLI to use LLM ```python python -m webscout.LLM
- model_name ``` [Go To TOP](#TOP) ## Regions expand xa-ar for Arabia xa-en for
-Arabia (en) ar-es for Argentina au-en for Australia at-de for Austria be-fr for
- Belgium (fr) be-nl for Belgium (nl) br-pt for Brazil bg-bg for Bulgaria ca-en
- for Canada ca-fr for Canada (fr) ct-ca for Catalan cl-es for Chile cn-zh for
- China co-es for Colombia hr-hr for Croatia cz-cs for Czech Republic dk-da for
-Denmark ee-et for Estonia fi-fi for Finland fr-fr for France de-de for Germany
- gr-el for Greece hk-tzh for Hong Kong hu-hu for Hungary in-en for India id-id
-for Indonesia id-en for Indonesia (en) ie-en for Ireland il-he for Israel it-it
-for Italy jp-jp for Japan kr-kr for Korea lv-lv for Latvia lt-lt for Lithuania
- xl-es for Latin America my-ms for Malaysia my-en for Malaysia (en) mx-es for
- Mexico nl-nl for Netherlands nz-en for New Zealand no-no for Norway pe-es for
- Peru ph-en for Philippines ph-tl for Philippines (tl) pl-pl for Poland pt-pt
- for Portugal ro-ro for Romania ru-ru for Russia sg-en for Singapore sk-sk for
-Slovak Republic sl-sl for Slovenia za-en for South Africa es-es for Spain se-sv
-  for Sweden ch-de for Switzerland (de) ch-fr for Switzerland (fr) ch-it for
- Switzerland (it) tw-tzh for Taiwan th-th for Thailand tr-tr for Turkey ua-uk
- for Ukraine uk-en for United Kingdom us-en for United States ue-es for United
- States (es) ve-es for Venezuela vn-vi for Vietnam wt-wt for No region ___ [Go
-   To TOP](#TOP) ## Tempmail and Temp number ### Temp number ```python from
- rich.console import Console from webscout import tempid def main(): console =
- Console() phone = tempid.TemporaryPhoneNumber() try: # Get a temporary phone
-      number for a specific country (or random) number = phone.get_number
- (country="Finland") console.print(f"Your temporary phone number: [bold cyan]
-  {number}[/bold cyan]") # Pause execution briefly (replace with your actual
-  logic) # import time module import time time.sleep(30) # Adjust the waiting
-  time as needed # Retrieve and print messages messages = phone.get_messages
-      (number) if messages: # Access individual messages using indexing:
- console.print(f"[bold green]{messages[0].frm}:[/] {messages[0].content}") #
-   (Add more lines if you expect multiple messages) else: console.print("No
-messages received.") except Exception as e: console.print(f"[bold red]An error
- occurred: {e}") if __name__ == "__main__": main() ``` ### Tempmail ```python
- import asyncio from rich.console import Console from rich.table import Table
-   from rich.text import Text from webscout import tempid async def main() -
-   > None: console = Console() client = tempid.Client() try: domains = await
-   client.get_domains() if not domains: console.print("[bold red]No domains
- available. Please try again later.") return email = await client.create_email
-  (domain=domains[0].name) console.print(f"Your temporary email: [bold cyan]
-  {email.email}[/bold cyan]") console.print(f"Token for accessing the email:
-      [bold cyan]{email.token}[/bold cyan]") while True: messages = await
- client.get_messages(email.email) if messages is not None: break if messages:
- table = Table(show_header=True, header_style="bold magenta") table.add_column
- ("From", style="bold cyan") table.add_column("Subject", style="bold yellow")
-     table.add_column("Body", style="bold green") for message in messages:
-  body_preview = Text(message.body_text if message.body_text else "No body")
-table.add_row(message.email_from or "Unknown", message.subject or "No Subject",
- body_preview) console.print(table) else: console.print("No messages found.")
-   except Exception as e: console.print(f"[bold red]An error occurred: {e}")
- finally: await client.close() if __name__ == '__main__': asyncio.run(main())
- ``` ## Transcriber The transcriber function in webscout is a handy tool that
-  transcribes YouTube videos. Here's an example code demonstrating its usage:
- ```python import sys from webscout import transcriber def extract_transcript
-     (video_id): """Extracts the transcript from a YouTube video.""" try:
-  transcript_list = transcriber.list_transcripts(video_id) for transcript in
-       transcript_list: transcript_data_list = transcript.fetch() lang =
+chat-with-free-gpt-35) - [`ThinkAny` - AI search engine](#thinkany---ai-search-
+engine) - [`LLM`](#llm) - [`LLM` with internet](#llm-with-internet) - [LLM with
+deepwebs](#llm-with-deepwebs) - [`Webai` - terminal gpt and a open interpeter]
+(#webai---terminal-gpt-and-a-open-interpeter) ## Install ```python pip install
+   -U webscout ``` ## CLI version ```python3 python -m webscout --help ``` |
+Command | Description | |-------------------------------------------|----------
+-------------------------------------------------------------------------------
+--------------| | python -m webscout answers -k Text | CLI function to perform
+ an answers search using Webscout. | | python -m webscout images -k Text | CLI
+  function to perform an images search using Webscout. | | python -m webscout
+maps -k Text | CLI function to perform a maps search using Webscout. | | python
+    -m webscout news -k Text | CLI function to perform a news search using
+Webscout. | | python -m webscout suggestions -k Text | CLI function to perform
+a suggestions search using Webscout. | | python -m webscout text -k Text | CLI
+   function to perform a text search using Webscout. | | python -m webscout
+   translate -k Text | CLI function to perform translate using Webscout. | |
+ python -m webscout version | A command-line interface command that prints and
+returns the version of the program. | | python -m webscout videos -k Text | CLI
+ function to perform a videos search using DuckDuckGo API. | ## CLI to use LLM
+ ```python python -m webscout.LLM model_name ``` [Go To TOP](#TOP) ## Regions
+  expand xa-ar for Arabia xa-en for Arabia (en) ar-es for Argentina au-en for
+Australia at-de for Austria be-fr for Belgium (fr) be-nl for Belgium (nl) br-pt
+for Brazil bg-bg for Bulgaria ca-en for Canada ca-fr for Canada (fr) ct-ca for
+ Catalan cl-es for Chile cn-zh for China co-es for Colombia hr-hr for Croatia
+cz-cs for Czech Republic dk-da for Denmark ee-et for Estonia fi-fi for Finland
+fr-fr for France de-de for Germany gr-el for Greece hk-tzh for Hong Kong hu-hu
+for Hungary in-en for India id-id for Indonesia id-en for Indonesia (en) ie-en
+ for Ireland il-he for Israel it-it for Italy jp-jp for Japan kr-kr for Korea
+lv-lv for Latvia lt-lt for Lithuania xl-es for Latin America my-ms for Malaysia
+ my-en for Malaysia (en) mx-es for Mexico nl-nl for Netherlands nz-en for New
+    Zealand no-no for Norway pe-es for Peru ph-en for Philippines ph-tl for
+ Philippines (tl) pl-pl for Poland pt-pt for Portugal ro-ro for Romania ru-ru
+for Russia sg-en for Singapore sk-sk for Slovak Republic sl-sl for Slovenia za-
+en for South Africa es-es for Spain se-sv for Sweden ch-de for Switzerland (de)
+ ch-fr for Switzerland (fr) ch-it for Switzerland (it) tw-tzh for Taiwan th-th
+for Thailand tr-tr for Turkey ua-uk for Ukraine uk-en for United Kingdom us-en
+ for United States ue-es for United States (es) ve-es for Venezuela vn-vi for
+ Vietnam wt-wt for No region ___ [Go To TOP](#TOP) ## Tempmail and Temp number
+### Temp number ```python from rich.console import Console from webscout import
+ tempid def main(): console = Console() phone = tempid.TemporaryPhoneNumber()
+try: # Get a temporary phone number for a specific country (or random) number =
+   phone.get_number(country="Finland") console.print(f"Your temporary phone
+ number: [bold cyan]{number}[/bold cyan]") # Pause execution briefly (replace
+   with your actual logic) # import time module import time time.sleep(30) #
+  Adjust the waiting time as needed # Retrieve and print messages messages =
+  phone.get_messages(number) if messages: # Access individual messages using
+     indexing: console.print(f"[bold green]{messages[0].frm}:[/] {messages
+    [0].content}") # (Add more lines if you expect multiple messages) else:
+console.print("No messages received.") except Exception as e: console.print(f"
+ [bold red]An error occurred: {e}") if __name__ == "__main__": main() ``` ###
+    Tempmail ```python import asyncio from rich.console import Console from
+rich.table import Table from rich.text import Text from webscout import tempid
+  async def main() -> None: console = Console() client = tempid.Client() try:
+   domains = await client.get_domains() if not domains: console.print("[bold
+   red]No domains available. Please try again later.") return email = await
+  client.create_email(domain=domains[0].name) console.print(f"Your temporary
+    email: [bold cyan]{email.email}[/bold cyan]") console.print(f"Token for
+    accessing the email: [bold cyan]{email.token}[/bold cyan]") while True:
+  messages = await client.get_messages(email.email) if messages is not None:
+break if messages: table = Table(show_header=True, header_style="bold magenta")
+    table.add_column("From", style="bold cyan") table.add_column("Subject",
+ style="bold yellow") table.add_column("Body", style="bold green") for message
+ in messages: body_preview = Text(message.body_text if message.body_text else
+ "No body") table.add_row(message.email_from or "Unknown", message.subject or
+   "No Subject", body_preview) console.print(table) else: console.print("No
+  messages found.") except Exception as e: console.print(f"[bold red]An error
+   occurred: {e}") finally: await client.close() if __name__ == '__main__':
+asyncio.run(main()) ``` ## Transcriber The transcriber function in webscout is
+     a handy tool that transcribes YouTube videos. Here's an example code
+demonstrating its usage: ```python import sys from webscout import transcriber
+  def extract_transcript(video_id): """Extracts the transcript from a YouTube
+  video.""" try: transcript_list = transcriber.list_transcripts(video_id) for
+transcript in transcript_list: transcript_data_list = transcript.fetch() lang =
  transcript.language transcript_text = "" if transcript.language_code == 'en':
     for line in transcript_data_list: start_time = line['start'] end_time =
      start_time + line['duration'] formatted_line = f"{start_time:.2f} -
   {end_time:.2f}: {line['text']}\n" transcript_text += formatted_line return
   transcript_text elif transcript.is_translatable: english_transcript_list =
     transcript.translate('en').fetch() for line in english_transcript_list:
       start_time = line['start'] end_time = start_time + line['duration']
@@ -339,63 +313,70 @@
 prompt.lower() == "exit": break # Use the 'chat' method to send the prompt and
    receive a response r = ai.chat(prompt) print(r) ``` ### 7. `PERPLEXITY` -
 Search With PERPLEXITY ```python from webscout.AI import PERPLEXITY # Create an
   instance of the PERPLEXITY class perplexity = PERPLEXITY() # Example usage:
     prompt = "Explain the concept of recursion in simple terms." response =
    perplexity.chat(prompt) print(response) ``` ### 8. `OpenGPT` - chat With
       OPENGPT ```python from webscout.AI import OPENGPT opengpt = OPENGPT
- (is_conversation=True, max_tokens=8000, timeout=30) while True: # Prompt the
- user for input prompt = input("Enter your prompt: ") # Send the prompt to the
-OPENGPT model and print the response response_str = opengpt.chat(prompt) print
-   (response_str) ``` ### 9. `KOBOLDIA` - ```python from webscout.AI import
- KOBOLDAI # Instantiate the KOBOLDAI class with default parameters koboldai =
-KOBOLDAI() # Define a prompt to send to the AI prompt = "What is the capital of
-   France?" # Use the 'ask' method to get a response from the AI response =
-koboldai.ask(prompt) # Extract and print the message from the response message
-= koboldai.get_message(response) print(message) ``` ### 10. `Reka` - chat with
-  reka ```python from webscout.AI import REKA a = REKA(is_conversation=True,
+  (is_conversation=True, max_tokens=8000, timeout=30, assistant_id="bca37014-
+6f97-4f2b-8928-81ea8d478d88") while True: # Prompt the user for input prompt =
+ input("Enter your prompt: ") # Send the prompt to the OPENGPT model and print
+the response response_str = opengpt.chat(prompt) print(response_str) ``` ### 9.
+   `KOBOLDIA` - ```python from webscout.AI import KOBOLDAI # Instantiate the
+KOBOLDAI class with default parameters koboldai = KOBOLDAI() # Define a prompt
+  to send to the AI prompt = "What is the capital of France?" # Use the 'ask'
+method to get a response from the AI response = koboldai.ask(prompt) # Extract
+    and print the message from the response message = koboldai.get_message
+ (response) print(message) ``` ### 10. `Reka` - chat with reka ```python from
+    webscout.AI import REKA a = REKA(is_conversation=True, max_tokens=8000,
+  timeout=30,api_key="") prompt = "tell me about india" response_str = a.chat
+(prompt) print(response_str) ``` ### 11. `Cohere` - chat with cohere ```python
+        from webscout.AI import Cohere a = Cohere(is_conversation=True,
     max_tokens=8000, timeout=30,api_key="") prompt = "tell me about india"
- response_str = a.chat(prompt) print(response_str) ``` ### 11. `Cohere` - chat
-        with cohere ```python from webscout.AI import Cohere a = Cohere
- (is_conversation=True, max_tokens=8000, timeout=30,api_key="") prompt = "tell
- me about india" response_str = a.chat(prompt) print(response_str) ``` ### 12.
-      `Xjai` - chat with free gpt 3.5 Gratitude to [Devs do Code](http://
- www.youtube.com/@DevsDoCode) for their assistance. ```python from webscout.AI
-      import Xjai from rich import print ai = Xjai( is_conversation=True,
-   max_tokens=800, timeout=30, intro=None, filepath=None, update_file=True,
- proxies={}, history_offset=10250, act=None, ) prompt = "Tell me about india"
-    response = ai.chat(prompt) print(response) ``` ### `LLM` ```python from
-   webscout.LLM import LLM # Read the system message from the file with open
-('system.txt', 'r') as file: system_message = file.read() # Initialize the LLM
-   class with the model name and system message llm = LLM(model="microsoft/
- WizardLM-2-8x22B", system_message=system_message) while True: # Get the user
-input user_input = input("User: ") # Define the messages to be sent messages =
- [ {"role": "user", "content": user_input} ] # Use the mistral_chat method to
-get the response response = llm.chat(messages) # Print the response print("AI:
-   ", response) ``` ### `LLM` with internet ```python from __future__ import
-annotations from typing import List, Optional from webscout.LLM import LLM from
-    webscout import WEBS import warnings system_message: str = ( "As an AI
-assistant, I have been designed with advanced capabilities, including real-time
-  access to online resources. This enables me to enrich our conversations and
-provide you with informed and accurate responses, drawing from a vast array of
-    information. With each interaction, my goal is to create a seamless and
-  meaningful connection, offering insights and sharing relevant content." "My
-directives emphasize the importance of respect, impartiality, and intellectual
-  integrity. I am here to provide unbiased responses, ensuring an ethical and
- respectful exchange. I will respect your privacy and refrain from sharing any
- personal information that may be obtained during our conversations or through
-web searches, only utilizing web search functionality when necessary to provide
-   the most accurate and up-to-date information." "Together, let's explore a
-diverse range of topics, creating an enjoyable and informative experience, all
-while maintaining the highest standards of privacy and respect" ) # Ignore the
- specific UserWarning warnings.filterwarnings("ignore", category=UserWarning,
- module="curl_cffi.aio", lineno=205) LLM = LLM(model="mistralai/Mixtral-8x22B-
-Instruct-v0.1", system_message=system_message) def chat( user_input: str, webs:
-WEBS, max_results: int = 10 ) -> Optional[str]: """ Chat function to perform a
-web search based on the user input and generate a response using the LLM model.
+  response_str = a.chat(prompt) print(response_str) ``` ### 12. `Xjai` - chat
+     with free gpt 3.5 Gratitude to [Devs do Code](http://www.youtube.com/
+@DevsDoCode) for their assistance. ```python from webscout.AI import Xjai from
+rich import print ai = Xjai( is_conversation=True, max_tokens=800, timeout=30,
+intro=None, filepath=None, update_file=True, proxies={}, history_offset=10250,
+  act=None, ) prompt = "Tell me about india" response = ai.chat(prompt) print
+  (response) ``` ### `ThinkAny` - AI search engine ```python from webscout.AI
+   import ThinkAnyAI ai = ThinkAnyAI( is_conversation=True, max_tokens=800,
+     timeout=30, intro=None, filepath=None, update_file=True, proxies={},
+ history_offset=10250, act=None, web_search=False, ) prompt = "what is meaning
+  of life" response = ai.ask(prompt) # Extract and print the message from the
+   response message = ai.get_message(response) print(message) ``` ### `LLM`
+```python from webscout.LLM import LLM # Read the system message from the file
+with open('system.txt', 'r') as file: system_message = file.read() # Initialize
+        the LLM class with the model name and system message llm = LLM
+(model="microsoft/WizardLM-2-8x22B", system_message=system_message) while True:
+ # Get the user input user_input = input("User: ") # Define the messages to be
+     sent messages = [ {"role": "user", "content": user_input} ] # Use the
+ mistral_chat method to get the response response = llm.chat(messages) # Print
+the response print("AI: ", response) ``` ### `LLM` with internet ```python from
+     __future__ import annotations from typing import List, Optional from
+       webscout.LLM import LLM from webscout import WEBS import warnings
+system_message: str = ( "As an AI assistant, I have been designed with advanced
+ capabilities, including real-time access to online resources. This enables me
+    to enrich our conversations and provide you with informed and accurate
+responses, drawing from a vast array of information. With each interaction, my
+ goal is to create a seamless and meaningful connection, offering insights and
+sharing relevant content." "My directives emphasize the importance of respect,
+    impartiality, and intellectual integrity. I am here to provide unbiased
+  responses, ensuring an ethical and respectful exchange. I will respect your
+privacy and refrain from sharing any personal information that may be obtained
+  during our conversations or through web searches, only utilizing web search
+   functionality when necessary to provide the most accurate and up-to-date
+ information." "Together, let's explore a diverse range of topics, creating an
+    enjoyable and informative experience, all while maintaining the highest
+     standards of privacy and respect" ) # Ignore the specific UserWarning
+warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffi.aio",
+     lineno=205) LLM = LLM(model="mistralai/Mixtral-8x22B-Instruct-v0.1",
+     system_message=system_message) def chat( user_input: str, webs: WEBS,
+ max_results: int = 10 ) -> Optional[str]: """ Chat function to perform a web
+  search based on the user input and generate a response using the LLM model.
  Parameters ---------- user_input : str The user input to be used for the web
   search webs : WEBS The web search instance to be used to perform the search
 max_results : int, optional The maximum number of search results to include in
     the response, by default 10 Returns ------- Optional[str] The response
 generated by the LLM model, or None if there is no response """ # Perform a web
     search based on the user input search_results: List[str] = [] for r in
     webs.text( user_input, region="wt-wt", safesearch="off", timelimit="y",
@@ -460,7 +441,10 @@
   key/value (if needed) timeout=30, disable_conversation=True, filepath=None,
        update_file=True, intro=None, rawdog=True, history_offset=10250,
       awesome_prompt=None, proxy_path=None, quiet=True ) webai_response =
 webai_bot.default(prompt) except Exception as e: print("Unexpected error:", e)
      if __name__ == "__main__": user_prompt = input("Enter your prompt: ")
 use_rawdog_with_webai(user_prompt) ``` ```shell python -m webscout.webai webai
                         --provider "phind" --rawdog ```
+               _[_T_e_l_e_g_r_a_m_]_[_I_n_s_t_a_g_r_a_m_]_[_L_i_n_k_e_d_I_n_]_[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
+                          _➤_ _V_o_r_t_e_x_'_s_ _Y_o_u_T_u_b_e_ _C_h_a_n_n_e_l
+                       _➤_ _D_e_v_s_ _D_o_ _C_o_d_e_'_s_ _Y_o_u_T_u_b_e_ _C_h_a_n_n_e_l
```

### Comparing `webscout-1.4.3/README.md` & `webscout-1.4.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,96 @@
-#  webscout
+Metadata-Version: 2.1
+Name: webscout
+Version: 1.4.4
+Summary: Search for anything using the Google, DuckDuckGo, phind.com. Also containes AI models, can transcribe yt videos, temporary email and phone number generation, have TTS support and webai(terminal gpt and open interpeter)
+Author: OEvortex
+Author-email: helpingai5@gmail.com
+License: HelpingAI Simplified Universal License
+Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
+Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
+Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
+Project-URL: YouTube, https://youtube.com/@OEvortex
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: docstring_inheritance>=2.1.2
+Requires-Dist: click>=8.1.7
+Requires-Dist: curl_cffi>=0.6.0b7
+Requires-Dist: lxml>=5.1.0
+Requires-Dist: nest-asyncio>=1.6.0
+Requires-Dist: selenium>=4.1.3
+Requires-Dist: tqdm>=4.64.0
+Requires-Dist: webdriver-manager>=3.5.4
+Requires-Dist: halo>=0.0.31
+Requires-Dist: g4f>=0.2.2.3
+Requires-Dist: rich
+Requires-Dist: python-dotenv
+Requires-Dist: Helpingai-T2
+Requires-Dist: beautifulsoup4
+Requires-Dist: markdownify
+Requires-Dist: pydantic
+Requires-Dist: requests
+Requires-Dist: sse_starlette
+Requires-Dist: termcolor
+Requires-Dist: tiktoken
+Requires-Dist: tldextract
+Requires-Dist: orjson
+Requires-Dist: PyYAML
+Requires-Dist: appdirs
+Requires-Dist: GoogleBard1>=2.1.4
+Requires-Dist: tls_client
+Provides-Extra: dev
+Requires-Dist: ruff>=0.1.6; extra == "dev"
+Requires-Dist: pytest>=7.4.2; extra == "dev"
+
+<div align="center">
+  <!-- Replace `#` with your actual links -->
+  <a href="https://t.me/devsdocode"><img alt="Telegram" src="https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white"></a>
+  <a href="https://www.instagram.com/sree.shades_/"><img alt="Instagram" src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white"></a>
+  <a href="https://www.linkedin.com/in/developer-sreejan/"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a>
+  <a href="https://buymeacoffee.com/devsdocode"><img alt="Buy Me A Coffee" src="https://img.shields.io/badge/Buy%20Me%20A%20Coffee-FFDD00?style=for-the-badge&logo=buymeacoffee&logoColor=black"></a>
+</div>
+
+<div align="center">
+  <!-- Replace `#` with your actual links -->
+  <a href="https://youtube.com/@@OEvortex">&#10148; Vortex's YouTube Channel</a>
+  </div>
+<div align="center">
+  <a href="https://youtube.com/@devsdocode">&#10148; Devs Do Code's YouTube Channel</a>
+</div>
+
+
+
+  
+# WEBSCOUT
+</div>
 <p align="center">
-
+<div align="center">
+  <img src="https://img.shields.io/badge/WebScout-API-blue?style=for-the-badge&logo=WebScout" alt="WebScout API Badge">
+</div>
 <a href="#"><img alt="Python version" src="https://img.shields.io/pypi/pyversions/webscout"/></a>
 <a href="https://pepy.tech/project/webscout"><img alt="Downloads" src="https://static.pepy.tech/badge/webscout"></a>
 
 Search for anything using the Google, DuckDuckGo, phind.com. Also containes AI models, can transcribe yt videos, temporary email and phone number generation, have TTS support and webai(terminal gpt and open interpeter)
 
 
 ## Table of Contents
-- [webscout](#webscout)
+- [WEBSCOUT](#webscout)
   - [Table of Contents](#table-of-contents)
   - [Install](#install)
   - [CLI version](#cli-version)
   - [CLI to use LLM](#cli-to-use-llm)
   - [Regions](#regions)
   - [Tempmail and Temp number](#tempmail-and-temp-number)
     - [Temp number](#temp-number)
@@ -45,14 +123,15 @@
     - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---searchchat-with-blackbox)
     - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---search-with-perplexity)
     - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-with-opengpt)
     - [9. `KOBOLDIA` -](#9-koboldia--)
     - [10. `Reka` - chat with reka](#10-reka---chat-with-reka)
     - [11. `Cohere` - chat with cohere](#11-cohere---chat-with-cohere)
     - [12. `Xjai` - chat with free gpt 3.5](#12-xjai---chat-with-free-gpt-35)
+    - [`ThinkAny` - AI search engine](#thinkany---ai-search-engine)
     - [`LLM`](#llm)
     - [`LLM` with internet](#llm-with-internet)
     - [LLM with deepwebs](#llm-with-deepwebs)
   - [`Webai` - terminal gpt and a open interpeter](#webai---terminal-gpt-and-a-open-interpeter)
 
 ## Install
 ```python
@@ -730,15 +809,15 @@
 response = perplexity.chat(prompt)
 print(response)
 ```
 ### 8. `OpenGPT` - chat With OPENGPT
 ```python
 from webscout.AI import OPENGPT
 
-opengpt = OPENGPT(is_conversation=True, max_tokens=8000, timeout=30)
+opengpt = OPENGPT(is_conversation=True, max_tokens=8000, timeout=30, assistant_id="bca37014-6f97-4f2b-8928-81ea8d478d88")
 while True:
     # Prompt the user for input
     prompt = input("Enter your prompt: ")
     # Send the prompt to the OPENGPT model and print the response
     response_str = opengpt.chat(prompt)
     print(response_str)
 ```
@@ -802,15 +881,39 @@
 )
 
 prompt = "Tell me about india"
 
 response = ai.chat(prompt)
 print(response)
 ```
+### `ThinkAny` - AI search engine
+```python
+from webscout.AI import ThinkAnyAI
+
+ai = ThinkAnyAI(
+    is_conversation=True,
+    max_tokens=800,
+    timeout=30,
+    intro=None,
+    filepath=None,
+    update_file=True,
+    proxies={},
+    history_offset=10250,
+    act=None,
+    web_search=False,
+)
+
+prompt = "what is meaning of life"
 
+response = ai.ask(prompt)
+
+# Extract and print the message from the response
+message = ai.get_message(response)
+print(message)
+```
 ### `LLM` 
 ```python
 from webscout.LLM import LLM
 
 # Read the system message from the file
 with open('system.txt', 'r') as file:
     system_message = file.read()
@@ -1033,7 +1136,25 @@
     user_prompt = input("Enter your prompt: ")
     use_rawdog_with_webai(user_prompt)
 
 ```
 ```shell
 python -m webscout.webai webai --provider "phind" --rawdog
 ```
+
+<div align="center">
+  <!-- Replace `#` with your actual links -->
+  <a href="https://t.me/devsdocode"><img alt="Telegram" src="https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white"></a>
+  <a href="https://www.instagram.com/sree.shades_/"><img alt="Instagram" src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white"></a>
+  <a href="https://www.linkedin.com/in/developer-sreejan/"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a>
+  <a href="https://buymeacoffee.com/devsdocode"><img alt="Buy Me A Coffee" src="https://img.shields.io/badge/Buy%20Me%20A%20Coffee-FFDD00?style=for-the-badge&logo=buymeacoffee&logoColor=black"></a>
+</div>
+
+<div align="center">
+  <!-- Replace `#` with your actual links -->
+  <a href="https://youtube.com/@@OEvortex">&#10148; Vortex's YouTube Channel</a>
+  </div>
+<div align="center">
+  <a href="https://youtube.com/@devsdocode">&#10148; Devs Do Code's YouTube Channel</a>
+</div>
+
+
```

#### html2text {}

```diff
@@ -1,12 +1,47 @@
-# webscout
+Metadata-Version: 2.1 Name: webscout Version: 1.4.4 Summary: Search for
+anything using the Google, DuckDuckGo, phind.com. Also containes AI models, can
+transcribe yt videos, temporary email and phone number generation, have TTS
+support and webai(terminal gpt and open interpeter) Author: OEvortex Author-
+email: helpingai5@gmail.com License: HelpingAI Simplified Universal License
+Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
+Project-URL: Source, https://github.com/OE-LUCIFER/Webscout Project-URL:
+Tracker, https://github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube,
+https://youtube.com/@OEvortex Classifier: Development Status :: 5 - Production/
+Stable Classifier: Intended Audience :: Developers Classifier: License ::
+Other/Proprietary License Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search Classifier: Topic
+:: Software Development :: Libraries :: Python Modules Description-Content-
+Type: text/markdown License-File: LICENSE.md Requires-Dist:
+docstring_inheritance>=2.1.2 Requires-Dist: click>=8.1.7 Requires-Dist:
+curl_cffi>=0.6.0b7 Requires-Dist: lxml>=5.1.0 Requires-Dist: nest-
+asyncio>=1.6.0 Requires-Dist: selenium>=4.1.3 Requires-Dist: tqdm>=4.64.0
+Requires-Dist: webdriver-manager>=3.5.4 Requires-Dist: halo>=0.0.31 Requires-
+Dist: g4f>=0.2.2.3 Requires-Dist: rich Requires-Dist: python-dotenv Requires-
+Dist: Helpingai-T2 Requires-Dist: beautifulsoup4 Requires-Dist: markdownify
+Requires-Dist: pydantic Requires-Dist: requests Requires-Dist: sse_starlette
+Requires-Dist: termcolor Requires-Dist: tiktoken Requires-Dist: tldextract
+Requires-Dist: orjson Requires-Dist: PyYAML Requires-Dist: appdirs Requires-
+Dist: GoogleBard1>=2.1.4 Requires-Dist: tls_client Provides-Extra: dev
+Requires-Dist: ruff>=0.1.6; extra == "dev" Requires-Dist: pytest>=7.4.2; extra
+== "dev"
+               _[_T_e_l_e_g_r_a_m_]_[_I_n_s_t_a_g_r_a_m_]_[_L_i_n_k_e_d_I_n_]_[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
+                          _➤_ _V_o_r_t_e_x_'_s_ _Y_o_u_T_u_b_e_ _C_h_a_n_n_e_l
+                       _➤_ _D_e_v_s_ _D_o_ _C_o_d_e_'_s_ _Y_o_u_T_u_b_e_ _C_h_a_n_n_e_l
+# WEBSCOUT
+                             [WebScout API Badge]
  _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]Search for anything using the Google, DuckDuckGo,
 phind.com. Also containes AI models, can transcribe yt videos, temporary email
  and phone number generation, have TTS support and webai(terminal gpt and open
-interpeter) ## Table of Contents - [webscout](#webscout) - [Table of Contents]
+interpeter) ## Table of Contents - [WEBSCOUT](#webscout) - [Table of Contents]
 (#table-of-contents) - [Install](#install) - [CLI version](#cli-version) - [CLI
 to use LLM](#cli-to-use-llm) - [Regions](#regions) - [Tempmail and Temp number]
     (#tempmail-and-temp-number) - [Temp number](#temp-number) - [Tempmail]
  (#tempmail) - [Transcriber](#transcriber) - [DeepWEBS: Advanced Web Searches]
 (#deepwebs-advanced-web-searches) - [Activating DeepWEBS](#activating-deepwebs)
 - [Point to remember before using `DeepWEBS`](#point-to-remember-before-using-
    deepwebs) - [Usage Example](#usage-example) - [Text-to-Speech:](#text-to-
@@ -33,87 +68,87 @@
 gemini) - [5. `Prodia` - make image using prodia](#5-prodia---make-image-using-
 prodia) - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---searchchat-
  with-blackbox) - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---
 search-with-perplexity) - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-
   with-opengpt) - [9. `KOBOLDIA` -](#9-koboldia--) - [10. `Reka` - chat with
    reka](#10-reka---chat-with-reka) - [11. `Cohere` - chat with cohere](#11-
 cohere---chat-with-cohere) - [12. `Xjai` - chat with free gpt 3.5](#12-xjai---
-   chat-with-free-gpt-35) - [`LLM`](#llm) - [`LLM` with internet](#llm-with-
- internet) - [LLM with deepwebs](#llm-with-deepwebs) - [`Webai` - terminal gpt
-and a open interpeter](#webai---terminal-gpt-and-a-open-interpeter) ## Install
-   ```python pip install -U webscout ``` ## CLI version ```python3 python -
-m webscout --help ``` | Command | Description | |------------------------------
--------------|-----------------------------------------------------------------
---------------------------------------| | python -m webscout answers -k Text |
-    CLI function to perform an answers search using Webscout. | | python -
-  m webscout images -k Text | CLI function to perform an images search using
-Webscout. | | python -m webscout maps -k Text | CLI function to perform a maps
- search using Webscout. | | python -m webscout news -k Text | CLI function to
-  perform a news search using Webscout. | | python -m webscout suggestions -
-   k Text | CLI function to perform a suggestions search using Webscout. | |
- python -m webscout text -k Text | CLI function to perform a text search using
- Webscout. | | python -m webscout translate -k Text | CLI function to perform
-   translate using Webscout. | | python -m webscout version | A command-line
-   interface command that prints and returns the version of the program. | |
-  python -m webscout videos -k Text | CLI function to perform a videos search
-  using DuckDuckGo API. | ## CLI to use LLM ```python python -m webscout.LLM
- model_name ``` [Go To TOP](#TOP) ## Regions expand xa-ar for Arabia xa-en for
-Arabia (en) ar-es for Argentina au-en for Australia at-de for Austria be-fr for
- Belgium (fr) be-nl for Belgium (nl) br-pt for Brazil bg-bg for Bulgaria ca-en
- for Canada ca-fr for Canada (fr) ct-ca for Catalan cl-es for Chile cn-zh for
- China co-es for Colombia hr-hr for Croatia cz-cs for Czech Republic dk-da for
-Denmark ee-et for Estonia fi-fi for Finland fr-fr for France de-de for Germany
- gr-el for Greece hk-tzh for Hong Kong hu-hu for Hungary in-en for India id-id
-for Indonesia id-en for Indonesia (en) ie-en for Ireland il-he for Israel it-it
-for Italy jp-jp for Japan kr-kr for Korea lv-lv for Latvia lt-lt for Lithuania
- xl-es for Latin America my-ms for Malaysia my-en for Malaysia (en) mx-es for
- Mexico nl-nl for Netherlands nz-en for New Zealand no-no for Norway pe-es for
- Peru ph-en for Philippines ph-tl for Philippines (tl) pl-pl for Poland pt-pt
- for Portugal ro-ro for Romania ru-ru for Russia sg-en for Singapore sk-sk for
-Slovak Republic sl-sl for Slovenia za-en for South Africa es-es for Spain se-sv
-  for Sweden ch-de for Switzerland (de) ch-fr for Switzerland (fr) ch-it for
- Switzerland (it) tw-tzh for Taiwan th-th for Thailand tr-tr for Turkey ua-uk
- for Ukraine uk-en for United Kingdom us-en for United States ue-es for United
- States (es) ve-es for Venezuela vn-vi for Vietnam wt-wt for No region ___ [Go
-   To TOP](#TOP) ## Tempmail and Temp number ### Temp number ```python from
- rich.console import Console from webscout import tempid def main(): console =
- Console() phone = tempid.TemporaryPhoneNumber() try: # Get a temporary phone
-      number for a specific country (or random) number = phone.get_number
- (country="Finland") console.print(f"Your temporary phone number: [bold cyan]
-  {number}[/bold cyan]") # Pause execution briefly (replace with your actual
-  logic) # import time module import time time.sleep(30) # Adjust the waiting
-  time as needed # Retrieve and print messages messages = phone.get_messages
-      (number) if messages: # Access individual messages using indexing:
- console.print(f"[bold green]{messages[0].frm}:[/] {messages[0].content}") #
-   (Add more lines if you expect multiple messages) else: console.print("No
-messages received.") except Exception as e: console.print(f"[bold red]An error
- occurred: {e}") if __name__ == "__main__": main() ``` ### Tempmail ```python
- import asyncio from rich.console import Console from rich.table import Table
-   from rich.text import Text from webscout import tempid async def main() -
-   > None: console = Console() client = tempid.Client() try: domains = await
-   client.get_domains() if not domains: console.print("[bold red]No domains
- available. Please try again later.") return email = await client.create_email
-  (domain=domains[0].name) console.print(f"Your temporary email: [bold cyan]
-  {email.email}[/bold cyan]") console.print(f"Token for accessing the email:
-      [bold cyan]{email.token}[/bold cyan]") while True: messages = await
- client.get_messages(email.email) if messages is not None: break if messages:
- table = Table(show_header=True, header_style="bold magenta") table.add_column
- ("From", style="bold cyan") table.add_column("Subject", style="bold yellow")
-     table.add_column("Body", style="bold green") for message in messages:
-  body_preview = Text(message.body_text if message.body_text else "No body")
-table.add_row(message.email_from or "Unknown", message.subject or "No Subject",
- body_preview) console.print(table) else: console.print("No messages found.")
-   except Exception as e: console.print(f"[bold red]An error occurred: {e}")
- finally: await client.close() if __name__ == '__main__': asyncio.run(main())
- ``` ## Transcriber The transcriber function in webscout is a handy tool that
-  transcribes YouTube videos. Here's an example code demonstrating its usage:
- ```python import sys from webscout import transcriber def extract_transcript
-     (video_id): """Extracts the transcript from a YouTube video.""" try:
-  transcript_list = transcriber.list_transcripts(video_id) for transcript in
-       transcript_list: transcript_data_list = transcript.fetch() lang =
+chat-with-free-gpt-35) - [`ThinkAny` - AI search engine](#thinkany---ai-search-
+engine) - [`LLM`](#llm) - [`LLM` with internet](#llm-with-internet) - [LLM with
+deepwebs](#llm-with-deepwebs) - [`Webai` - terminal gpt and a open interpeter]
+(#webai---terminal-gpt-and-a-open-interpeter) ## Install ```python pip install
+   -U webscout ``` ## CLI version ```python3 python -m webscout --help ``` |
+Command | Description | |-------------------------------------------|----------
+-------------------------------------------------------------------------------
+--------------| | python -m webscout answers -k Text | CLI function to perform
+ an answers search using Webscout. | | python -m webscout images -k Text | CLI
+  function to perform an images search using Webscout. | | python -m webscout
+maps -k Text | CLI function to perform a maps search using Webscout. | | python
+    -m webscout news -k Text | CLI function to perform a news search using
+Webscout. | | python -m webscout suggestions -k Text | CLI function to perform
+a suggestions search using Webscout. | | python -m webscout text -k Text | CLI
+   function to perform a text search using Webscout. | | python -m webscout
+   translate -k Text | CLI function to perform translate using Webscout. | |
+ python -m webscout version | A command-line interface command that prints and
+returns the version of the program. | | python -m webscout videos -k Text | CLI
+ function to perform a videos search using DuckDuckGo API. | ## CLI to use LLM
+ ```python python -m webscout.LLM model_name ``` [Go To TOP](#TOP) ## Regions
+  expand xa-ar for Arabia xa-en for Arabia (en) ar-es for Argentina au-en for
+Australia at-de for Austria be-fr for Belgium (fr) be-nl for Belgium (nl) br-pt
+for Brazil bg-bg for Bulgaria ca-en for Canada ca-fr for Canada (fr) ct-ca for
+ Catalan cl-es for Chile cn-zh for China co-es for Colombia hr-hr for Croatia
+cz-cs for Czech Republic dk-da for Denmark ee-et for Estonia fi-fi for Finland
+fr-fr for France de-de for Germany gr-el for Greece hk-tzh for Hong Kong hu-hu
+for Hungary in-en for India id-id for Indonesia id-en for Indonesia (en) ie-en
+ for Ireland il-he for Israel it-it for Italy jp-jp for Japan kr-kr for Korea
+lv-lv for Latvia lt-lt for Lithuania xl-es for Latin America my-ms for Malaysia
+ my-en for Malaysia (en) mx-es for Mexico nl-nl for Netherlands nz-en for New
+    Zealand no-no for Norway pe-es for Peru ph-en for Philippines ph-tl for
+ Philippines (tl) pl-pl for Poland pt-pt for Portugal ro-ro for Romania ru-ru
+for Russia sg-en for Singapore sk-sk for Slovak Republic sl-sl for Slovenia za-
+en for South Africa es-es for Spain se-sv for Sweden ch-de for Switzerland (de)
+ ch-fr for Switzerland (fr) ch-it for Switzerland (it) tw-tzh for Taiwan th-th
+for Thailand tr-tr for Turkey ua-uk for Ukraine uk-en for United Kingdom us-en
+ for United States ue-es for United States (es) ve-es for Venezuela vn-vi for
+ Vietnam wt-wt for No region ___ [Go To TOP](#TOP) ## Tempmail and Temp number
+### Temp number ```python from rich.console import Console from webscout import
+ tempid def main(): console = Console() phone = tempid.TemporaryPhoneNumber()
+try: # Get a temporary phone number for a specific country (or random) number =
+   phone.get_number(country="Finland") console.print(f"Your temporary phone
+ number: [bold cyan]{number}[/bold cyan]") # Pause execution briefly (replace
+   with your actual logic) # import time module import time time.sleep(30) #
+  Adjust the waiting time as needed # Retrieve and print messages messages =
+  phone.get_messages(number) if messages: # Access individual messages using
+     indexing: console.print(f"[bold green]{messages[0].frm}:[/] {messages
+    [0].content}") # (Add more lines if you expect multiple messages) else:
+console.print("No messages received.") except Exception as e: console.print(f"
+ [bold red]An error occurred: {e}") if __name__ == "__main__": main() ``` ###
+    Tempmail ```python import asyncio from rich.console import Console from
+rich.table import Table from rich.text import Text from webscout import tempid
+  async def main() -> None: console = Console() client = tempid.Client() try:
+   domains = await client.get_domains() if not domains: console.print("[bold
+   red]No domains available. Please try again later.") return email = await
+  client.create_email(domain=domains[0].name) console.print(f"Your temporary
+    email: [bold cyan]{email.email}[/bold cyan]") console.print(f"Token for
+    accessing the email: [bold cyan]{email.token}[/bold cyan]") while True:
+  messages = await client.get_messages(email.email) if messages is not None:
+break if messages: table = Table(show_header=True, header_style="bold magenta")
+    table.add_column("From", style="bold cyan") table.add_column("Subject",
+ style="bold yellow") table.add_column("Body", style="bold green") for message
+ in messages: body_preview = Text(message.body_text if message.body_text else
+ "No body") table.add_row(message.email_from or "Unknown", message.subject or
+   "No Subject", body_preview) console.print(table) else: console.print("No
+  messages found.") except Exception as e: console.print(f"[bold red]An error
+   occurred: {e}") finally: await client.close() if __name__ == '__main__':
+asyncio.run(main()) ``` ## Transcriber The transcriber function in webscout is
+     a handy tool that transcribes YouTube videos. Here's an example code
+demonstrating its usage: ```python import sys from webscout import transcriber
+  def extract_transcript(video_id): """Extracts the transcript from a YouTube
+  video.""" try: transcript_list = transcriber.list_transcripts(video_id) for
+transcript in transcript_list: transcript_data_list = transcript.fetch() lang =
  transcript.language transcript_text = "" if transcript.language_code == 'en':
     for line in transcript_data_list: start_time = line['start'] end_time =
      start_time + line['duration'] formatted_line = f"{start_time:.2f} -
   {end_time:.2f}: {line['text']}\n" transcript_text += formatted_line return
   transcript_text elif transcript.is_translatable: english_transcript_list =
     transcript.translate('en').fetch() for line in english_transcript_list:
       start_time = line['start'] end_time = start_time + line['duration']
@@ -309,63 +344,70 @@
 prompt.lower() == "exit": break # Use the 'chat' method to send the prompt and
    receive a response r = ai.chat(prompt) print(r) ``` ### 7. `PERPLEXITY` -
 Search With PERPLEXITY ```python from webscout.AI import PERPLEXITY # Create an
   instance of the PERPLEXITY class perplexity = PERPLEXITY() # Example usage:
     prompt = "Explain the concept of recursion in simple terms." response =
    perplexity.chat(prompt) print(response) ``` ### 8. `OpenGPT` - chat With
       OPENGPT ```python from webscout.AI import OPENGPT opengpt = OPENGPT
- (is_conversation=True, max_tokens=8000, timeout=30) while True: # Prompt the
- user for input prompt = input("Enter your prompt: ") # Send the prompt to the
-OPENGPT model and print the response response_str = opengpt.chat(prompt) print
-   (response_str) ``` ### 9. `KOBOLDIA` - ```python from webscout.AI import
- KOBOLDAI # Instantiate the KOBOLDAI class with default parameters koboldai =
-KOBOLDAI() # Define a prompt to send to the AI prompt = "What is the capital of
-   France?" # Use the 'ask' method to get a response from the AI response =
-koboldai.ask(prompt) # Extract and print the message from the response message
-= koboldai.get_message(response) print(message) ``` ### 10. `Reka` - chat with
-  reka ```python from webscout.AI import REKA a = REKA(is_conversation=True,
+  (is_conversation=True, max_tokens=8000, timeout=30, assistant_id="bca37014-
+6f97-4f2b-8928-81ea8d478d88") while True: # Prompt the user for input prompt =
+ input("Enter your prompt: ") # Send the prompt to the OPENGPT model and print
+the response response_str = opengpt.chat(prompt) print(response_str) ``` ### 9.
+   `KOBOLDIA` - ```python from webscout.AI import KOBOLDAI # Instantiate the
+KOBOLDAI class with default parameters koboldai = KOBOLDAI() # Define a prompt
+  to send to the AI prompt = "What is the capital of France?" # Use the 'ask'
+method to get a response from the AI response = koboldai.ask(prompt) # Extract
+    and print the message from the response message = koboldai.get_message
+ (response) print(message) ``` ### 10. `Reka` - chat with reka ```python from
+    webscout.AI import REKA a = REKA(is_conversation=True, max_tokens=8000,
+  timeout=30,api_key="") prompt = "tell me about india" response_str = a.chat
+(prompt) print(response_str) ``` ### 11. `Cohere` - chat with cohere ```python
+        from webscout.AI import Cohere a = Cohere(is_conversation=True,
     max_tokens=8000, timeout=30,api_key="") prompt = "tell me about india"
- response_str = a.chat(prompt) print(response_str) ``` ### 11. `Cohere` - chat
-        with cohere ```python from webscout.AI import Cohere a = Cohere
- (is_conversation=True, max_tokens=8000, timeout=30,api_key="") prompt = "tell
- me about india" response_str = a.chat(prompt) print(response_str) ``` ### 12.
-      `Xjai` - chat with free gpt 3.5 Gratitude to [Devs do Code](http://
- www.youtube.com/@DevsDoCode) for their assistance. ```python from webscout.AI
-      import Xjai from rich import print ai = Xjai( is_conversation=True,
-   max_tokens=800, timeout=30, intro=None, filepath=None, update_file=True,
- proxies={}, history_offset=10250, act=None, ) prompt = "Tell me about india"
-    response = ai.chat(prompt) print(response) ``` ### `LLM` ```python from
-   webscout.LLM import LLM # Read the system message from the file with open
-('system.txt', 'r') as file: system_message = file.read() # Initialize the LLM
-   class with the model name and system message llm = LLM(model="microsoft/
- WizardLM-2-8x22B", system_message=system_message) while True: # Get the user
-input user_input = input("User: ") # Define the messages to be sent messages =
- [ {"role": "user", "content": user_input} ] # Use the mistral_chat method to
-get the response response = llm.chat(messages) # Print the response print("AI:
-   ", response) ``` ### `LLM` with internet ```python from __future__ import
-annotations from typing import List, Optional from webscout.LLM import LLM from
-    webscout import WEBS import warnings system_message: str = ( "As an AI
-assistant, I have been designed with advanced capabilities, including real-time
-  access to online resources. This enables me to enrich our conversations and
-provide you with informed and accurate responses, drawing from a vast array of
-    information. With each interaction, my goal is to create a seamless and
-  meaningful connection, offering insights and sharing relevant content." "My
-directives emphasize the importance of respect, impartiality, and intellectual
-  integrity. I am here to provide unbiased responses, ensuring an ethical and
- respectful exchange. I will respect your privacy and refrain from sharing any
- personal information that may be obtained during our conversations or through
-web searches, only utilizing web search functionality when necessary to provide
-   the most accurate and up-to-date information." "Together, let's explore a
-diverse range of topics, creating an enjoyable and informative experience, all
-while maintaining the highest standards of privacy and respect" ) # Ignore the
- specific UserWarning warnings.filterwarnings("ignore", category=UserWarning,
- module="curl_cffi.aio", lineno=205) LLM = LLM(model="mistralai/Mixtral-8x22B-
-Instruct-v0.1", system_message=system_message) def chat( user_input: str, webs:
-WEBS, max_results: int = 10 ) -> Optional[str]: """ Chat function to perform a
-web search based on the user input and generate a response using the LLM model.
+  response_str = a.chat(prompt) print(response_str) ``` ### 12. `Xjai` - chat
+     with free gpt 3.5 Gratitude to [Devs do Code](http://www.youtube.com/
+@DevsDoCode) for their assistance. ```python from webscout.AI import Xjai from
+rich import print ai = Xjai( is_conversation=True, max_tokens=800, timeout=30,
+intro=None, filepath=None, update_file=True, proxies={}, history_offset=10250,
+  act=None, ) prompt = "Tell me about india" response = ai.chat(prompt) print
+  (response) ``` ### `ThinkAny` - AI search engine ```python from webscout.AI
+   import ThinkAnyAI ai = ThinkAnyAI( is_conversation=True, max_tokens=800,
+     timeout=30, intro=None, filepath=None, update_file=True, proxies={},
+ history_offset=10250, act=None, web_search=False, ) prompt = "what is meaning
+  of life" response = ai.ask(prompt) # Extract and print the message from the
+   response message = ai.get_message(response) print(message) ``` ### `LLM`
+```python from webscout.LLM import LLM # Read the system message from the file
+with open('system.txt', 'r') as file: system_message = file.read() # Initialize
+        the LLM class with the model name and system message llm = LLM
+(model="microsoft/WizardLM-2-8x22B", system_message=system_message) while True:
+ # Get the user input user_input = input("User: ") # Define the messages to be
+     sent messages = [ {"role": "user", "content": user_input} ] # Use the
+ mistral_chat method to get the response response = llm.chat(messages) # Print
+the response print("AI: ", response) ``` ### `LLM` with internet ```python from
+     __future__ import annotations from typing import List, Optional from
+       webscout.LLM import LLM from webscout import WEBS import warnings
+system_message: str = ( "As an AI assistant, I have been designed with advanced
+ capabilities, including real-time access to online resources. This enables me
+    to enrich our conversations and provide you with informed and accurate
+responses, drawing from a vast array of information. With each interaction, my
+ goal is to create a seamless and meaningful connection, offering insights and
+sharing relevant content." "My directives emphasize the importance of respect,
+    impartiality, and intellectual integrity. I am here to provide unbiased
+  responses, ensuring an ethical and respectful exchange. I will respect your
+privacy and refrain from sharing any personal information that may be obtained
+  during our conversations or through web searches, only utilizing web search
+   functionality when necessary to provide the most accurate and up-to-date
+ information." "Together, let's explore a diverse range of topics, creating an
+    enjoyable and informative experience, all while maintaining the highest
+     standards of privacy and respect" ) # Ignore the specific UserWarning
+warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffi.aio",
+     lineno=205) LLM = LLM(model="mistralai/Mixtral-8x22B-Instruct-v0.1",
+     system_message=system_message) def chat( user_input: str, webs: WEBS,
+ max_results: int = 10 ) -> Optional[str]: """ Chat function to perform a web
+  search based on the user input and generate a response using the LLM model.
  Parameters ---------- user_input : str The user input to be used for the web
   search webs : WEBS The web search instance to be used to perform the search
 max_results : int, optional The maximum number of search results to include in
     the response, by default 10 Returns ------- Optional[str] The response
 generated by the LLM model, or None if there is no response """ # Perform a web
     search based on the user input search_results: List[str] = [] for r in
     webs.text( user_input, region="wt-wt", safesearch="off", timelimit="y",
@@ -430,7 +472,10 @@
   key/value (if needed) timeout=30, disable_conversation=True, filepath=None,
        update_file=True, intro=None, rawdog=True, history_offset=10250,
       awesome_prompt=None, proxy_path=None, quiet=True ) webai_response =
 webai_bot.default(prompt) except Exception as e: print("Unexpected error:", e)
      if __name__ == "__main__": user_prompt = input("Enter your prompt: ")
 use_rawdog_with_webai(user_prompt) ``` ```shell python -m webscout.webai webai
                         --provider "phind" --rawdog ```
+               _[_T_e_l_e_g_r_a_m_]_[_I_n_s_t_a_g_r_a_m_]_[_L_i_n_k_e_d_I_n_]_[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
+                          _➤_ _V_o_r_t_e_x_'_s_ _Y_o_u_T_u_b_e_ _C_h_a_n_n_e_l
+                       _➤_ _D_e_v_s_ _D_o_ _C_o_d_e_'_s_ _Y_o_u_T_u_b_e_ _C_h_a_n_n_e_l
```

### Comparing `webscout-1.4.3/setup.py` & `webscout-1.4.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="webscout",
-    version="1.4.3", 
+    version="1.4.4", 
     description="Search for anything using the Google, DuckDuckGo, phind.com. Also containes AI models, can transcribe yt videos, temporary email and phone number generation, have TTS support and webai(terminal gpt and open interpeter)",
     long_description=README,
     long_description_content_type="text/markdown",
     author="OEvortex",
     author_email="helpingai5@gmail.com",
     packages=find_packages(),
     classifiers=[
```

### Comparing `webscout-1.4.3/webscout/AI.py` & `webscout-1.4.4/webscout/AI.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,17 +21,267 @@
 import yaml
 from webscout.AIutel import Optimizers
 from webscout.AIutel import Conversation
 from webscout.AIutel import AwesomePrompts, sanitize_stream
 from webscout.AIbase import  Provider, AsyncProvider
 from Helpingai_T2 import Perplexity
 from webscout import exceptions
-from typing import Any, AsyncGenerator
+from typing import Any, AsyncGenerator, Dict
 import logging
 import httpx
+#------------------------------------ThinkAnyAI------------
+class ThinkAnyAI(Provider):
+    def __init__(
+        self,
+        model: str = "claude-3-haiku",
+        locale: str = "en",
+        web_search: bool = False,
+        chunk_size: int = 1,
+        streaming: bool = True,
+        is_conversation: bool = True,
+        max_tokens: int = 600,
+        timeout: int = 30,
+        intro: str = None,
+        filepath: str = None,
+        update_file: bool = True,
+        proxies: dict = {},
+        history_offset: int = 10250,
+        act: str = None,
+    ):
+        """Initializes ThinkAnyAI
+
+        Args:
+            model (str): The AI model to be used for generating responses. Defaults to "claude-3-haiku".
+            locale (str): The language locale. Defaults to "en" (English).
+            web_search (bool): Whether to include web search results in the response. Defaults to False.
+            chunk_size (int): The size of data chunks when streaming responses. Defaults to 1.
+            streaming (bool): Whether to stream response data. Defaults to True.
+            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True.
+            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
+            timeout (int, optional): Http request timeout. Defaults to 30.
+            intro (str, optional): Conversation introductory prompt. Defaults to None.
+            filepath (str, optional): Path to file containing conversation history. Defaults to None.
+            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
+            proxies (dict, optional): Http request proxies. Defaults to {}.
+            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
+            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
+        """
+        self.base_url = "https://thinkany.ai/api"
+        self.model = model
+        self.locale = locale
+        self.web_search = web_search
+        self.chunk_size = chunk_size
+        self.streaming = streaming
+        self.last_response = {}
+        self.session = requests.Session()
+        self.session.proxies = proxies
+
+        self.__available_optimizers = (
+            method
+            for method in dir(Optimizers)
+            if callable(getattr(Optimizers, method)) and not method.startswith("__")
+        )
+
+        Conversation.intro = (
+            AwesomePrompts().get_act(
+                act, raise_not_found=True, default=None, case_insensitive=True
+            )
+            if act
+            else intro or Conversation.intro
+        )
+        self.conversation = Conversation(
+            is_conversation, max_tokens, filepath, update_file
+        )
+        self.conversation.history_offset = history_offset
+
+    def ask(
+        self,
+        prompt: str,
+        stream: bool = False,
+        raw: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> dict | AsyncGenerator:
+        """Chat with AI asynchronously.
+
+            Args:
+                prompt (str): Prompt to be send.
+                stream (bool, optional): Flag for streaming response. Defaults to False.
+                raw (bool, optional): Stream back raw response as received. Defaults to False.
+                optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defeaults to None
+                conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+            Returns:
+                dict : {}
+            ```json
+            {
+                "content": "General Kenobi! \n\n(I couldn't help but respond with the iconic Star Wars greeting since you used it first. )\n\nIs there anything I can help you with today?\n[Image of Hello there General Kenobi]",
+                "conversation_id": "c_f13f6217f9a997aa",
+                "response_id": "r_d3665f95975c368f",
+                "factualityQueries": null,
+                "textQuery": [
+                    "hello there",
+                    1
+                    ],
+                "choices": [
+                    {
+                        "id": "rc_ea075c9671bfd8cb",
+                        "content": [
+                            "General Kenobi! \n\n(I couldn't help but respond with the iconic Star Wars greeting since you used it first. )\n\nIs there anything I can help you with today?\n[Image of Hello there General Kenobi]"
+                        ]
+                    },
+                    {
+                        "id": "rc_de6dd3fb793a5402",
+                        "content": [
+                            "General Kenobi! (or just a friendly hello, whichever you prefer!). \n\nI see you're a person of culture as well. *Star Wars* references are always appreciated.  \n\nHow can I help you today?\n"
+                            ]
+                    },
+                {
+                    "id": "rc_a672ac089caf32db",
+                    "content": [
+                        "General Kenobi! (or just a friendly hello if you're not a Star Wars fan!). \n\nHow can I help you today? Feel free to ask me anything, or tell me what you'd like to chat about. I'm here to assist in any way I can.\n[Image of Obi-Wan Kenobi saying hello there]"
+                    ]
+                }
+            ],
+
+            "images": [
+                "https://i.pinimg.com/originals/40/74/60/407460925c9e419d82b93313f0b42f71.jpg"
+            ]
+        }
+
+            ```
+        """
+        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
+        if optimizer:
+            if optimizer in self.__available_optimizers:
+                conversation_prompt = getattr(Optimizers, optimizer)(
+                    conversation_prompt if conversationally else prompt
+                )
+            else:
+                raise Exception(
+                    f"Optimizer is not one of {self.__available_optimizers}"
+                )
+
+        def initiate_conversation(query: str) -> str:
+            """
+            Initiates a new conversation with the ThinkAny AI API.
+
+            Args:
+                query (str): The initial query to start the conversation.
+
+            Returns:
+                str: The UUID (Unique Identifier) of the conversation.
+            """
+            url = f"{self.base_url}/new-conversation"
+            payload = {
+                "content": query,
+                "locale": self.locale,
+                "mode": "search" if self.web_search else "chat",
+                "model": self.model,
+                "source": "all",
+            }
+            response = self.session.post(url, json=payload)
+            return response.json().get("data", {}).get("uuid", "DevsDoCode")
+
+        def RAG_search(uuid: str) -> tuple[bool, list]:
+            """
+            Performs a web search using the Retrieve And Generate (RAG) model.
+
+            Args:
+                uuid (str): The UUID of the conversation.
+
+            Returns:
+                tuple: A tuple containing a boolean indicating the success of the search
+                        and a list of search result links.
+            """
+            if not self.web_search:
+                return True, []
+            url = f"{self.base_url}/rag-search"
+            payload = {"conv_uuid": uuid}
+            response = self.session.post(url, json=payload)
+            links = [source["link"] for source in response.json().get("data", [])]
+            return response.json().get("message", "").strip(), links
+
+        def for_stream():
+            conversation_uuid = initiate_conversation(conversation_prompt)
+            web_search_result, links = RAG_search(conversation_uuid)
+            if not web_search_result:
+                print("Failed to generate WEB response. Making normal Query...")
+
+            url = f"{self.base_url}/chat"
+            payload = {
+                "role": "user",
+                "content": prompt,
+                "conv_uuid": conversation_uuid,
+                "model": self.model,
+            }
+            response = self.session.post(url, json=payload, stream=True)
+            complete_content = ""
+            for content in response.iter_content(
+                decode_unicode=True, chunk_size=self.chunk_size
+            ):
+                complete_content += content
+                yield content if raw else dict(text=complete_content)
+            self.last_response.update(dict(text=complete_content, links=links))
+            self.conversation.update_chat_history(
+                prompt, self.get_message(self.last_response)
+            )
+
+        def for_non_stream():
+            for _ in for_stream():
+                pass
+            return self.last_response
+
+        return for_stream() if stream else for_non_stream()
+
+    def chat(
+        self,
+        prompt: str,
+        stream: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> str:
+        """Generate response `str`
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+            str: Response generated
+        """
+
+        def for_stream():
+            for response in self.ask(
+                prompt, True, optimizer=optimizer, conversationally=conversationally
+            ):
+                yield self.get_message(response)
+
+        def for_non_stream():
+            return self.get_message(
+                self.ask(
+                    prompt,
+                    False,
+                    optimizer=optimizer,
+                    conversationally=conversationally,
+                )
+            )
+
+        return for_stream() if stream else for_non_stream()
+
+    def get_message(self, response: Dict[str, Any]) -> str:
+        """Retrieves message only from response
+
+        Args:
+            response (dict): Response generated by `self.ask`
+
+        Returns:
+            str: Message extracted
+        """
+        assert isinstance(response, dict), "Response should be of dict data-type only"
+        return response["text"]
 #-----------------------------------------------xjai-------------------------------------------
 class Xjai(Provider):
     def __init__(
         self,
         is_conversation: bool = True,
         max_tokens: int = 600,
         temperature: float = 0.8,
@@ -2798,14 +3048,15 @@
         """
         assert isinstance(response, dict), "Response should be of dict data-type only"
         return response.get("token")
 #------------------------------------------------------OpenGPT-----------------------------------------------------------
 class OPENGPT:
     def __init__(
         self,
+        assistant_id,
         is_conversation: bool = True,
         max_tokens: int = 600,
         timeout: int = 30,
         intro: str = None,
         filepath: str = None,
         update_file: bool = True,
         proxies: dict = {},
@@ -2830,15 +3081,15 @@
         self.is_conversation = is_conversation
         self.chat_endpoint = (
             "https://opengpts-example-vz4y4ooboq-uc.a.run.app/runs/stream"
         )
         self.stream_chunk_size = 64
         self.timeout = timeout
         self.last_response = {}
-        self.assistant_id = "bca37014-6f97-4f2b-8928-81ea8d478d88"
+        self.assistant_id = assistant_id
         self.authority = "opengpts-example-vz4y4ooboq-uc.a.run.app"
 
         self.headers = {
             "authority": self.authority,
             "accept": "text/event-stream",
             "accept-language": "en-US,en;q=0.7",
             "cache-control": "no-cache",
@@ -3022,15 +3273,14 @@
         Args:
             response (dict): Response generated by `self.ask`
 
         Returns:
             str: Message extracted
         """
         assert isinstance(response, dict), "Response should be of dict data-type only"
-        return response["content"]
 class AsyncOPENGPT(AsyncProvider):
     def __init__(
         self,
         is_conversation: bool = True,
         max_tokens: int = 600,
         timeout: int = 30,
         intro: str = None,
```

### Comparing `webscout-1.4.3/webscout/AIbase.py` & `webscout-1.4.4/webscout/AIbase.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.3/webscout/AIutel.py` & `webscout-1.4.4/webscout/AIutel.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from typing import Union
 from typing import NoReturn
 import requests
 from pathlib import Path
 from playsound import playsound
 from time import sleep as wait
 import pathlib
+import urllib.parse
 appdir = appdirs.AppDirs("AIWEBS", "vortex")
 
 default_path = appdir.user_cache_dir
 
 if not os.path.exists(default_path):
     os.makedirs(default_path)
 webai = [
@@ -35,15 +36,16 @@
     "g4fauto",
     "perplexity",
     "groq",
     "reka",
     "cohere",
     "yepchat",
     "you",
-    "xjai"
+    "xjai",
+    "thinkany"
 ]
 
 gpt4free_providers = [
     provider.__name__ for provider in g4f.Provider.__providers__  # if provider.working
 ]
 
 available_providers = webai + gpt4free_providers
@@ -934,15 +936,15 @@
             result (Union[str, bytes]): Path to saved contents or audio content.
         """
         assert (
             voice in cls.all_voices
         ), f"Voice '{voice}' not one of [{', '.join(cls.all_voices)}]"
         # Base URL for provider API
         url: str = (
-            f"https://api.streamelements.com/kappa/v2/speech?voice={voice}&text={{{message}}}"
+            f"https://api.streamelements.com/kappa/v2/speech?voice={voice}&text={{{urllib.parse.quote(message)}}}"
         )
         resp = requests.get(url=url, headers=cls.headers, stream=True)
         if not resp.ok:
             raise Exception(
                 f"Failed to perform the operation - ({resp.status_code}, {resp.reason}) - {resp.text}"
             )
```

### Comparing `webscout-1.4.3/webscout/DWEBS.py` & `webscout-1.4.4/webscout/DWEBS.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.3/webscout/LLM.py` & `webscout-1.4.4/webscout/LLM.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.3/webscout/__init__.py` & `webscout-1.4.4/webscout/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,16 @@
     "g4fauto",
     "perplexity",
     "groq",
     "reka",
     "cohere",
     "yepchat",
     "you",
-    "xjai"
+    "xjai",
+    "thinkany"
 ]
 
 gpt4free_providers = [
     provider.__name__ for provider in g4f.Provider.__providers__  # if provider.working
 ]
 
 available_providers = webai + gpt4free_providers
```

### Comparing `webscout-1.4.3/webscout/async_providers.py` & `webscout-1.4.4/webscout/async_providers.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.3/webscout/cli.py` & `webscout-1.4.4/webscout/cli.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.3/webscout/g4f.py` & `webscout-1.4.4/webscout/g4f.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.3/webscout/models.py` & `webscout-1.4.4/webscout/models.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.3/webscout/tempid.py` & `webscout-1.4.4/webscout/tempid.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.3/webscout/transcriber.py` & `webscout-1.4.4/webscout/transcriber.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.3/webscout/utils.py` & `webscout-1.4.4/webscout/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import re
 from decimal import Decimal
 from html import unescape
 from math import atan2, cos, radians, sin, sqrt
 from typing import Any, Dict, List, Union
 from urllib.parse import unquote
-
 import orjson
 
 from .exceptions import WebscoutE
 
 REGEX_STRIP_TAGS = re.compile("<.*?>")
```

### Comparing `webscout-1.4.3/webscout/voice.py` & `webscout-1.4.4/webscout/voice.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.3/webscout/webai.py` & `webscout-1.4.4/webscout/webai.py`

 * *Files 1% similar despite different names*

```diff
@@ -467,14 +467,28 @@
                     intro=intro,
                     filepath=filepath,
                     update_file=update_file,
                     proxies=proxies,
                     history_offset=history_offset,
                     act=awesome_prompt,
                 )
+            elif provider == "thinkany":
+                from webscout.AI import ThinkAnyAI
+
+                self.bot = ThinkAnyAI(
+                    is_conversation=disable_conversation,
+                    max_tokens=max_tokens,
+                    timeout=timeout,
+                    intro=intro,
+                    filepath=filepath,
+                    update_file=update_file,
+                    proxies=proxies,
+                    history_offset=history_offset,
+                    act=awesome_prompt,
+                )
             elif provider == "yepchat":
                 from webscout.AI import YEPCHAT
 
                 self.bot = YEPCHAT(
                     is_conversation=disable_conversation,
                     max_tokens=max_tokens,
                     temperature=temperature,
@@ -977,15 +991,15 @@
             "\nLLM :",
             "\n\n**LLM** :",
             re.sub("\nUser :", "\n\n**User** :", history),
         )
         self.output_bond("Chat History", formatted_history, self.color)
         if click.confirm("Do you wish to save this chat"):
             save_to = click.prompt(
-                "Enter path/file-name", default="llama-conversation.txt"
+                "Enter path/file-name", default=f"{self.provider}-chat.txt"
             )
             with open(save_to, "a") as fh:
                 fh.write(history)
             click.secho(f"Conversation saved successfully to '{save_to}'", fg="cyan")
 
     @busy_bar.run("while resetting conversation")
     def do_reset(self, line):
```

### Comparing `webscout-1.4.3/webscout/webscout_search.py` & `webscout-1.4.4/webscout/webscout_search.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.3/webscout/webscout_search_async.py` & `webscout-1.4.4/webscout/webscout_search_async.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.3/webscout.egg-info/PKG-INFO` & `webscout-1.4.4/webscout.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 1.4.3
+Version: 1.4.4
 Summary: Search for anything using the Google, DuckDuckGo, phind.com. Also containes AI models, can transcribe yt videos, temporary email and phone number generation, have TTS support and webai(terminal gpt and open interpeter)
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
@@ -50,25 +50,47 @@
 Requires-Dist: appdirs
 Requires-Dist: GoogleBard1>=2.1.4
 Requires-Dist: tls_client
 Provides-Extra: dev
 Requires-Dist: ruff>=0.1.6; extra == "dev"
 Requires-Dist: pytest>=7.4.2; extra == "dev"
 
-#  webscout
-<p align="center">
+<div align="center">
+  <!-- Replace `#` with your actual links -->
+  <a href="https://t.me/devsdocode"><img alt="Telegram" src="https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white"></a>
+  <a href="https://www.instagram.com/sree.shades_/"><img alt="Instagram" src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white"></a>
+  <a href="https://www.linkedin.com/in/developer-sreejan/"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a>
+  <a href="https://buymeacoffee.com/devsdocode"><img alt="Buy Me A Coffee" src="https://img.shields.io/badge/Buy%20Me%20A%20Coffee-FFDD00?style=for-the-badge&logo=buymeacoffee&logoColor=black"></a>
+</div>
+
+<div align="center">
+  <!-- Replace `#` with your actual links -->
+  <a href="https://youtube.com/@@OEvortex">&#10148; Vortex's YouTube Channel</a>
+  </div>
+<div align="center">
+  <a href="https://youtube.com/@devsdocode">&#10148; Devs Do Code's YouTube Channel</a>
+</div>
+
 
+
+  
+# WEBSCOUT
+</div>
+<p align="center">
+<div align="center">
+  <img src="https://img.shields.io/badge/WebScout-API-blue?style=for-the-badge&logo=WebScout" alt="WebScout API Badge">
+</div>
 <a href="#"><img alt="Python version" src="https://img.shields.io/pypi/pyversions/webscout"/></a>
 <a href="https://pepy.tech/project/webscout"><img alt="Downloads" src="https://static.pepy.tech/badge/webscout"></a>
 
 Search for anything using the Google, DuckDuckGo, phind.com. Also containes AI models, can transcribe yt videos, temporary email and phone number generation, have TTS support and webai(terminal gpt and open interpeter)
 
 
 ## Table of Contents
-- [webscout](#webscout)
+- [WEBSCOUT](#webscout)
   - [Table of Contents](#table-of-contents)
   - [Install](#install)
   - [CLI version](#cli-version)
   - [CLI to use LLM](#cli-to-use-llm)
   - [Regions](#regions)
   - [Tempmail and Temp number](#tempmail-and-temp-number)
     - [Temp number](#temp-number)
@@ -101,14 +123,15 @@
     - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---searchchat-with-blackbox)
     - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---search-with-perplexity)
     - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-with-opengpt)
     - [9. `KOBOLDIA` -](#9-koboldia--)
     - [10. `Reka` - chat with reka](#10-reka---chat-with-reka)
     - [11. `Cohere` - chat with cohere](#11-cohere---chat-with-cohere)
     - [12. `Xjai` - chat with free gpt 3.5](#12-xjai---chat-with-free-gpt-35)
+    - [`ThinkAny` - AI search engine](#thinkany---ai-search-engine)
     - [`LLM`](#llm)
     - [`LLM` with internet](#llm-with-internet)
     - [LLM with deepwebs](#llm-with-deepwebs)
   - [`Webai` - terminal gpt and a open interpeter](#webai---terminal-gpt-and-a-open-interpeter)
 
 ## Install
 ```python
@@ -786,15 +809,15 @@
 response = perplexity.chat(prompt)
 print(response)
 ```
 ### 8. `OpenGPT` - chat With OPENGPT
 ```python
 from webscout.AI import OPENGPT
 
-opengpt = OPENGPT(is_conversation=True, max_tokens=8000, timeout=30)
+opengpt = OPENGPT(is_conversation=True, max_tokens=8000, timeout=30, assistant_id="bca37014-6f97-4f2b-8928-81ea8d478d88")
 while True:
     # Prompt the user for input
     prompt = input("Enter your prompt: ")
     # Send the prompt to the OPENGPT model and print the response
     response_str = opengpt.chat(prompt)
     print(response_str)
 ```
@@ -858,15 +881,39 @@
 )
 
 prompt = "Tell me about india"
 
 response = ai.chat(prompt)
 print(response)
 ```
+### `ThinkAny` - AI search engine
+```python
+from webscout.AI import ThinkAnyAI
 
+ai = ThinkAnyAI(
+    is_conversation=True,
+    max_tokens=800,
+    timeout=30,
+    intro=None,
+    filepath=None,
+    update_file=True,
+    proxies={},
+    history_offset=10250,
+    act=None,
+    web_search=False,
+)
+
+prompt = "what is meaning of life"
+
+response = ai.ask(prompt)
+
+# Extract and print the message from the response
+message = ai.get_message(response)
+print(message)
+```
 ### `LLM` 
 ```python
 from webscout.LLM import LLM
 
 # Read the system message from the file
 with open('system.txt', 'r') as file:
     system_message = file.read()
@@ -1089,7 +1136,25 @@
     user_prompt = input("Enter your prompt: ")
     use_rawdog_with_webai(user_prompt)
 
 ```
 ```shell
 python -m webscout.webai webai --provider "phind" --rawdog
 ```
+
+<div align="center">
+  <!-- Replace `#` with your actual links -->
+  <a href="https://t.me/devsdocode"><img alt="Telegram" src="https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white"></a>
+  <a href="https://www.instagram.com/sree.shades_/"><img alt="Instagram" src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white"></a>
+  <a href="https://www.linkedin.com/in/developer-sreejan/"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a>
+  <a href="https://buymeacoffee.com/devsdocode"><img alt="Buy Me A Coffee" src="https://img.shields.io/badge/Buy%20Me%20A%20Coffee-FFDD00?style=for-the-badge&logo=buymeacoffee&logoColor=black"></a>
+</div>
+
+<div align="center">
+  <!-- Replace `#` with your actual links -->
+  <a href="https://youtube.com/@@OEvortex">&#10148; Vortex's YouTube Channel</a>
+  </div>
+<div align="center">
+  <a href="https://youtube.com/@devsdocode">&#10148; Devs Do Code's YouTube Channel</a>
+</div>
+
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: webscout Version: 1.4.3 Summary: Search for
+Metadata-Version: 2.1 Name: webscout Version: 1.4.4 Summary: Search for
 anything using the Google, DuckDuckGo, phind.com. Also containes AI models, can
 transcribe yt videos, temporary email and phone number generation, have TTS
 support and webai(terminal gpt and open interpeter) Author: OEvortex Author-
 email: helpingai5@gmail.com License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout Project-URL:
 Tracker, https://github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube,
@@ -24,19 +24,24 @@
 Dist: g4f>=0.2.2.3 Requires-Dist: rich Requires-Dist: python-dotenv Requires-
 Dist: Helpingai-T2 Requires-Dist: beautifulsoup4 Requires-Dist: markdownify
 Requires-Dist: pydantic Requires-Dist: requests Requires-Dist: sse_starlette
 Requires-Dist: termcolor Requires-Dist: tiktoken Requires-Dist: tldextract
 Requires-Dist: orjson Requires-Dist: PyYAML Requires-Dist: appdirs Requires-
 Dist: GoogleBard1>=2.1.4 Requires-Dist: tls_client Provides-Extra: dev
 Requires-Dist: ruff>=0.1.6; extra == "dev" Requires-Dist: pytest>=7.4.2; extra
-== "dev" # webscout
+== "dev"
+               _[_T_e_l_e_g_r_a_m_]_[_I_n_s_t_a_g_r_a_m_]_[_L_i_n_k_e_d_I_n_]_[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
+                          _➤_ _V_o_r_t_e_x_'_s_ _Y_o_u_T_u_b_e_ _C_h_a_n_n_e_l
+                       _➤_ _D_e_v_s_ _D_o_ _C_o_d_e_'_s_ _Y_o_u_T_u_b_e_ _C_h_a_n_n_e_l
+# WEBSCOUT
+                             [WebScout API Badge]
  _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]Search for anything using the Google, DuckDuckGo,
 phind.com. Also containes AI models, can transcribe yt videos, temporary email
  and phone number generation, have TTS support and webai(terminal gpt and open
-interpeter) ## Table of Contents - [webscout](#webscout) - [Table of Contents]
+interpeter) ## Table of Contents - [WEBSCOUT](#webscout) - [Table of Contents]
 (#table-of-contents) - [Install](#install) - [CLI version](#cli-version) - [CLI
 to use LLM](#cli-to-use-llm) - [Regions](#regions) - [Tempmail and Temp number]
     (#tempmail-and-temp-number) - [Temp number](#temp-number) - [Tempmail]
  (#tempmail) - [Transcriber](#transcriber) - [DeepWEBS: Advanced Web Searches]
 (#deepwebs-advanced-web-searches) - [Activating DeepWEBS](#activating-deepwebs)
 - [Point to remember before using `DeepWEBS`](#point-to-remember-before-using-
    deepwebs) - [Usage Example](#usage-example) - [Text-to-Speech:](#text-to-
@@ -63,87 +68,87 @@
 gemini) - [5. `Prodia` - make image using prodia](#5-prodia---make-image-using-
 prodia) - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---searchchat-
  with-blackbox) - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---
 search-with-perplexity) - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-
   with-opengpt) - [9. `KOBOLDIA` -](#9-koboldia--) - [10. `Reka` - chat with
    reka](#10-reka---chat-with-reka) - [11. `Cohere` - chat with cohere](#11-
 cohere---chat-with-cohere) - [12. `Xjai` - chat with free gpt 3.5](#12-xjai---
-   chat-with-free-gpt-35) - [`LLM`](#llm) - [`LLM` with internet](#llm-with-
- internet) - [LLM with deepwebs](#llm-with-deepwebs) - [`Webai` - terminal gpt
-and a open interpeter](#webai---terminal-gpt-and-a-open-interpeter) ## Install
-   ```python pip install -U webscout ``` ## CLI version ```python3 python -
-m webscout --help ``` | Command | Description | |------------------------------
--------------|-----------------------------------------------------------------
---------------------------------------| | python -m webscout answers -k Text |
-    CLI function to perform an answers search using Webscout. | | python -
-  m webscout images -k Text | CLI function to perform an images search using
-Webscout. | | python -m webscout maps -k Text | CLI function to perform a maps
- search using Webscout. | | python -m webscout news -k Text | CLI function to
-  perform a news search using Webscout. | | python -m webscout suggestions -
-   k Text | CLI function to perform a suggestions search using Webscout. | |
- python -m webscout text -k Text | CLI function to perform a text search using
- Webscout. | | python -m webscout translate -k Text | CLI function to perform
-   translate using Webscout. | | python -m webscout version | A command-line
-   interface command that prints and returns the version of the program. | |
-  python -m webscout videos -k Text | CLI function to perform a videos search
-  using DuckDuckGo API. | ## CLI to use LLM ```python python -m webscout.LLM
- model_name ``` [Go To TOP](#TOP) ## Regions expand xa-ar for Arabia xa-en for
-Arabia (en) ar-es for Argentina au-en for Australia at-de for Austria be-fr for
- Belgium (fr) be-nl for Belgium (nl) br-pt for Brazil bg-bg for Bulgaria ca-en
- for Canada ca-fr for Canada (fr) ct-ca for Catalan cl-es for Chile cn-zh for
- China co-es for Colombia hr-hr for Croatia cz-cs for Czech Republic dk-da for
-Denmark ee-et for Estonia fi-fi for Finland fr-fr for France de-de for Germany
- gr-el for Greece hk-tzh for Hong Kong hu-hu for Hungary in-en for India id-id
-for Indonesia id-en for Indonesia (en) ie-en for Ireland il-he for Israel it-it
-for Italy jp-jp for Japan kr-kr for Korea lv-lv for Latvia lt-lt for Lithuania
- xl-es for Latin America my-ms for Malaysia my-en for Malaysia (en) mx-es for
- Mexico nl-nl for Netherlands nz-en for New Zealand no-no for Norway pe-es for
- Peru ph-en for Philippines ph-tl for Philippines (tl) pl-pl for Poland pt-pt
- for Portugal ro-ro for Romania ru-ru for Russia sg-en for Singapore sk-sk for
-Slovak Republic sl-sl for Slovenia za-en for South Africa es-es for Spain se-sv
-  for Sweden ch-de for Switzerland (de) ch-fr for Switzerland (fr) ch-it for
- Switzerland (it) tw-tzh for Taiwan th-th for Thailand tr-tr for Turkey ua-uk
- for Ukraine uk-en for United Kingdom us-en for United States ue-es for United
- States (es) ve-es for Venezuela vn-vi for Vietnam wt-wt for No region ___ [Go
-   To TOP](#TOP) ## Tempmail and Temp number ### Temp number ```python from
- rich.console import Console from webscout import tempid def main(): console =
- Console() phone = tempid.TemporaryPhoneNumber() try: # Get a temporary phone
-      number for a specific country (or random) number = phone.get_number
- (country="Finland") console.print(f"Your temporary phone number: [bold cyan]
-  {number}[/bold cyan]") # Pause execution briefly (replace with your actual
-  logic) # import time module import time time.sleep(30) # Adjust the waiting
-  time as needed # Retrieve and print messages messages = phone.get_messages
-      (number) if messages: # Access individual messages using indexing:
- console.print(f"[bold green]{messages[0].frm}:[/] {messages[0].content}") #
-   (Add more lines if you expect multiple messages) else: console.print("No
-messages received.") except Exception as e: console.print(f"[bold red]An error
- occurred: {e}") if __name__ == "__main__": main() ``` ### Tempmail ```python
- import asyncio from rich.console import Console from rich.table import Table
-   from rich.text import Text from webscout import tempid async def main() -
-   > None: console = Console() client = tempid.Client() try: domains = await
-   client.get_domains() if not domains: console.print("[bold red]No domains
- available. Please try again later.") return email = await client.create_email
-  (domain=domains[0].name) console.print(f"Your temporary email: [bold cyan]
-  {email.email}[/bold cyan]") console.print(f"Token for accessing the email:
-      [bold cyan]{email.token}[/bold cyan]") while True: messages = await
- client.get_messages(email.email) if messages is not None: break if messages:
- table = Table(show_header=True, header_style="bold magenta") table.add_column
- ("From", style="bold cyan") table.add_column("Subject", style="bold yellow")
-     table.add_column("Body", style="bold green") for message in messages:
-  body_preview = Text(message.body_text if message.body_text else "No body")
-table.add_row(message.email_from or "Unknown", message.subject or "No Subject",
- body_preview) console.print(table) else: console.print("No messages found.")
-   except Exception as e: console.print(f"[bold red]An error occurred: {e}")
- finally: await client.close() if __name__ == '__main__': asyncio.run(main())
- ``` ## Transcriber The transcriber function in webscout is a handy tool that
-  transcribes YouTube videos. Here's an example code demonstrating its usage:
- ```python import sys from webscout import transcriber def extract_transcript
-     (video_id): """Extracts the transcript from a YouTube video.""" try:
-  transcript_list = transcriber.list_transcripts(video_id) for transcript in
-       transcript_list: transcript_data_list = transcript.fetch() lang =
+chat-with-free-gpt-35) - [`ThinkAny` - AI search engine](#thinkany---ai-search-
+engine) - [`LLM`](#llm) - [`LLM` with internet](#llm-with-internet) - [LLM with
+deepwebs](#llm-with-deepwebs) - [`Webai` - terminal gpt and a open interpeter]
+(#webai---terminal-gpt-and-a-open-interpeter) ## Install ```python pip install
+   -U webscout ``` ## CLI version ```python3 python -m webscout --help ``` |
+Command | Description | |-------------------------------------------|----------
+-------------------------------------------------------------------------------
+--------------| | python -m webscout answers -k Text | CLI function to perform
+ an answers search using Webscout. | | python -m webscout images -k Text | CLI
+  function to perform an images search using Webscout. | | python -m webscout
+maps -k Text | CLI function to perform a maps search using Webscout. | | python
+    -m webscout news -k Text | CLI function to perform a news search using
+Webscout. | | python -m webscout suggestions -k Text | CLI function to perform
+a suggestions search using Webscout. | | python -m webscout text -k Text | CLI
+   function to perform a text search using Webscout. | | python -m webscout
+   translate -k Text | CLI function to perform translate using Webscout. | |
+ python -m webscout version | A command-line interface command that prints and
+returns the version of the program. | | python -m webscout videos -k Text | CLI
+ function to perform a videos search using DuckDuckGo API. | ## CLI to use LLM
+ ```python python -m webscout.LLM model_name ``` [Go To TOP](#TOP) ## Regions
+  expand xa-ar for Arabia xa-en for Arabia (en) ar-es for Argentina au-en for
+Australia at-de for Austria be-fr for Belgium (fr) be-nl for Belgium (nl) br-pt
+for Brazil bg-bg for Bulgaria ca-en for Canada ca-fr for Canada (fr) ct-ca for
+ Catalan cl-es for Chile cn-zh for China co-es for Colombia hr-hr for Croatia
+cz-cs for Czech Republic dk-da for Denmark ee-et for Estonia fi-fi for Finland
+fr-fr for France de-de for Germany gr-el for Greece hk-tzh for Hong Kong hu-hu
+for Hungary in-en for India id-id for Indonesia id-en for Indonesia (en) ie-en
+ for Ireland il-he for Israel it-it for Italy jp-jp for Japan kr-kr for Korea
+lv-lv for Latvia lt-lt for Lithuania xl-es for Latin America my-ms for Malaysia
+ my-en for Malaysia (en) mx-es for Mexico nl-nl for Netherlands nz-en for New
+    Zealand no-no for Norway pe-es for Peru ph-en for Philippines ph-tl for
+ Philippines (tl) pl-pl for Poland pt-pt for Portugal ro-ro for Romania ru-ru
+for Russia sg-en for Singapore sk-sk for Slovak Republic sl-sl for Slovenia za-
+en for South Africa es-es for Spain se-sv for Sweden ch-de for Switzerland (de)
+ ch-fr for Switzerland (fr) ch-it for Switzerland (it) tw-tzh for Taiwan th-th
+for Thailand tr-tr for Turkey ua-uk for Ukraine uk-en for United Kingdom us-en
+ for United States ue-es for United States (es) ve-es for Venezuela vn-vi for
+ Vietnam wt-wt for No region ___ [Go To TOP](#TOP) ## Tempmail and Temp number
+### Temp number ```python from rich.console import Console from webscout import
+ tempid def main(): console = Console() phone = tempid.TemporaryPhoneNumber()
+try: # Get a temporary phone number for a specific country (or random) number =
+   phone.get_number(country="Finland") console.print(f"Your temporary phone
+ number: [bold cyan]{number}[/bold cyan]") # Pause execution briefly (replace
+   with your actual logic) # import time module import time time.sleep(30) #
+  Adjust the waiting time as needed # Retrieve and print messages messages =
+  phone.get_messages(number) if messages: # Access individual messages using
+     indexing: console.print(f"[bold green]{messages[0].frm}:[/] {messages
+    [0].content}") # (Add more lines if you expect multiple messages) else:
+console.print("No messages received.") except Exception as e: console.print(f"
+ [bold red]An error occurred: {e}") if __name__ == "__main__": main() ``` ###
+    Tempmail ```python import asyncio from rich.console import Console from
+rich.table import Table from rich.text import Text from webscout import tempid
+  async def main() -> None: console = Console() client = tempid.Client() try:
+   domains = await client.get_domains() if not domains: console.print("[bold
+   red]No domains available. Please try again later.") return email = await
+  client.create_email(domain=domains[0].name) console.print(f"Your temporary
+    email: [bold cyan]{email.email}[/bold cyan]") console.print(f"Token for
+    accessing the email: [bold cyan]{email.token}[/bold cyan]") while True:
+  messages = await client.get_messages(email.email) if messages is not None:
+break if messages: table = Table(show_header=True, header_style="bold magenta")
+    table.add_column("From", style="bold cyan") table.add_column("Subject",
+ style="bold yellow") table.add_column("Body", style="bold green") for message
+ in messages: body_preview = Text(message.body_text if message.body_text else
+ "No body") table.add_row(message.email_from or "Unknown", message.subject or
+   "No Subject", body_preview) console.print(table) else: console.print("No
+  messages found.") except Exception as e: console.print(f"[bold red]An error
+   occurred: {e}") finally: await client.close() if __name__ == '__main__':
+asyncio.run(main()) ``` ## Transcriber The transcriber function in webscout is
+     a handy tool that transcribes YouTube videos. Here's an example code
+demonstrating its usage: ```python import sys from webscout import transcriber
+  def extract_transcript(video_id): """Extracts the transcript from a YouTube
+  video.""" try: transcript_list = transcriber.list_transcripts(video_id) for
+transcript in transcript_list: transcript_data_list = transcript.fetch() lang =
  transcript.language transcript_text = "" if transcript.language_code == 'en':
     for line in transcript_data_list: start_time = line['start'] end_time =
      start_time + line['duration'] formatted_line = f"{start_time:.2f} -
   {end_time:.2f}: {line['text']}\n" transcript_text += formatted_line return
   transcript_text elif transcript.is_translatable: english_transcript_list =
     transcript.translate('en').fetch() for line in english_transcript_list:
       start_time = line['start'] end_time = start_time + line['duration']
@@ -339,63 +344,70 @@
 prompt.lower() == "exit": break # Use the 'chat' method to send the prompt and
    receive a response r = ai.chat(prompt) print(r) ``` ### 7. `PERPLEXITY` -
 Search With PERPLEXITY ```python from webscout.AI import PERPLEXITY # Create an
   instance of the PERPLEXITY class perplexity = PERPLEXITY() # Example usage:
     prompt = "Explain the concept of recursion in simple terms." response =
    perplexity.chat(prompt) print(response) ``` ### 8. `OpenGPT` - chat With
       OPENGPT ```python from webscout.AI import OPENGPT opengpt = OPENGPT
- (is_conversation=True, max_tokens=8000, timeout=30) while True: # Prompt the
- user for input prompt = input("Enter your prompt: ") # Send the prompt to the
-OPENGPT model and print the response response_str = opengpt.chat(prompt) print
-   (response_str) ``` ### 9. `KOBOLDIA` - ```python from webscout.AI import
- KOBOLDAI # Instantiate the KOBOLDAI class with default parameters koboldai =
-KOBOLDAI() # Define a prompt to send to the AI prompt = "What is the capital of
-   France?" # Use the 'ask' method to get a response from the AI response =
-koboldai.ask(prompt) # Extract and print the message from the response message
-= koboldai.get_message(response) print(message) ``` ### 10. `Reka` - chat with
-  reka ```python from webscout.AI import REKA a = REKA(is_conversation=True,
+  (is_conversation=True, max_tokens=8000, timeout=30, assistant_id="bca37014-
+6f97-4f2b-8928-81ea8d478d88") while True: # Prompt the user for input prompt =
+ input("Enter your prompt: ") # Send the prompt to the OPENGPT model and print
+the response response_str = opengpt.chat(prompt) print(response_str) ``` ### 9.
+   `KOBOLDIA` - ```python from webscout.AI import KOBOLDAI # Instantiate the
+KOBOLDAI class with default parameters koboldai = KOBOLDAI() # Define a prompt
+  to send to the AI prompt = "What is the capital of France?" # Use the 'ask'
+method to get a response from the AI response = koboldai.ask(prompt) # Extract
+    and print the message from the response message = koboldai.get_message
+ (response) print(message) ``` ### 10. `Reka` - chat with reka ```python from
+    webscout.AI import REKA a = REKA(is_conversation=True, max_tokens=8000,
+  timeout=30,api_key="") prompt = "tell me about india" response_str = a.chat
+(prompt) print(response_str) ``` ### 11. `Cohere` - chat with cohere ```python
+        from webscout.AI import Cohere a = Cohere(is_conversation=True,
     max_tokens=8000, timeout=30,api_key="") prompt = "tell me about india"
- response_str = a.chat(prompt) print(response_str) ``` ### 11. `Cohere` - chat
-        with cohere ```python from webscout.AI import Cohere a = Cohere
- (is_conversation=True, max_tokens=8000, timeout=30,api_key="") prompt = "tell
- me about india" response_str = a.chat(prompt) print(response_str) ``` ### 12.
-      `Xjai` - chat with free gpt 3.5 Gratitude to [Devs do Code](http://
- www.youtube.com/@DevsDoCode) for their assistance. ```python from webscout.AI
-      import Xjai from rich import print ai = Xjai( is_conversation=True,
-   max_tokens=800, timeout=30, intro=None, filepath=None, update_file=True,
- proxies={}, history_offset=10250, act=None, ) prompt = "Tell me about india"
-    response = ai.chat(prompt) print(response) ``` ### `LLM` ```python from
-   webscout.LLM import LLM # Read the system message from the file with open
-('system.txt', 'r') as file: system_message = file.read() # Initialize the LLM
-   class with the model name and system message llm = LLM(model="microsoft/
- WizardLM-2-8x22B", system_message=system_message) while True: # Get the user
-input user_input = input("User: ") # Define the messages to be sent messages =
- [ {"role": "user", "content": user_input} ] # Use the mistral_chat method to
-get the response response = llm.chat(messages) # Print the response print("AI:
-   ", response) ``` ### `LLM` with internet ```python from __future__ import
-annotations from typing import List, Optional from webscout.LLM import LLM from
-    webscout import WEBS import warnings system_message: str = ( "As an AI
-assistant, I have been designed with advanced capabilities, including real-time
-  access to online resources. This enables me to enrich our conversations and
-provide you with informed and accurate responses, drawing from a vast array of
-    information. With each interaction, my goal is to create a seamless and
-  meaningful connection, offering insights and sharing relevant content." "My
-directives emphasize the importance of respect, impartiality, and intellectual
-  integrity. I am here to provide unbiased responses, ensuring an ethical and
- respectful exchange. I will respect your privacy and refrain from sharing any
- personal information that may be obtained during our conversations or through
-web searches, only utilizing web search functionality when necessary to provide
-   the most accurate and up-to-date information." "Together, let's explore a
-diverse range of topics, creating an enjoyable and informative experience, all
-while maintaining the highest standards of privacy and respect" ) # Ignore the
- specific UserWarning warnings.filterwarnings("ignore", category=UserWarning,
- module="curl_cffi.aio", lineno=205) LLM = LLM(model="mistralai/Mixtral-8x22B-
-Instruct-v0.1", system_message=system_message) def chat( user_input: str, webs:
-WEBS, max_results: int = 10 ) -> Optional[str]: """ Chat function to perform a
-web search based on the user input and generate a response using the LLM model.
+  response_str = a.chat(prompt) print(response_str) ``` ### 12. `Xjai` - chat
+     with free gpt 3.5 Gratitude to [Devs do Code](http://www.youtube.com/
+@DevsDoCode) for their assistance. ```python from webscout.AI import Xjai from
+rich import print ai = Xjai( is_conversation=True, max_tokens=800, timeout=30,
+intro=None, filepath=None, update_file=True, proxies={}, history_offset=10250,
+  act=None, ) prompt = "Tell me about india" response = ai.chat(prompt) print
+  (response) ``` ### `ThinkAny` - AI search engine ```python from webscout.AI
+   import ThinkAnyAI ai = ThinkAnyAI( is_conversation=True, max_tokens=800,
+     timeout=30, intro=None, filepath=None, update_file=True, proxies={},
+ history_offset=10250, act=None, web_search=False, ) prompt = "what is meaning
+  of life" response = ai.ask(prompt) # Extract and print the message from the
+   response message = ai.get_message(response) print(message) ``` ### `LLM`
+```python from webscout.LLM import LLM # Read the system message from the file
+with open('system.txt', 'r') as file: system_message = file.read() # Initialize
+        the LLM class with the model name and system message llm = LLM
+(model="microsoft/WizardLM-2-8x22B", system_message=system_message) while True:
+ # Get the user input user_input = input("User: ") # Define the messages to be
+     sent messages = [ {"role": "user", "content": user_input} ] # Use the
+ mistral_chat method to get the response response = llm.chat(messages) # Print
+the response print("AI: ", response) ``` ### `LLM` with internet ```python from
+     __future__ import annotations from typing import List, Optional from
+       webscout.LLM import LLM from webscout import WEBS import warnings
+system_message: str = ( "As an AI assistant, I have been designed with advanced
+ capabilities, including real-time access to online resources. This enables me
+    to enrich our conversations and provide you with informed and accurate
+responses, drawing from a vast array of information. With each interaction, my
+ goal is to create a seamless and meaningful connection, offering insights and
+sharing relevant content." "My directives emphasize the importance of respect,
+    impartiality, and intellectual integrity. I am here to provide unbiased
+  responses, ensuring an ethical and respectful exchange. I will respect your
+privacy and refrain from sharing any personal information that may be obtained
+  during our conversations or through web searches, only utilizing web search
+   functionality when necessary to provide the most accurate and up-to-date
+ information." "Together, let's explore a diverse range of topics, creating an
+    enjoyable and informative experience, all while maintaining the highest
+     standards of privacy and respect" ) # Ignore the specific UserWarning
+warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffi.aio",
+     lineno=205) LLM = LLM(model="mistralai/Mixtral-8x22B-Instruct-v0.1",
+     system_message=system_message) def chat( user_input: str, webs: WEBS,
+ max_results: int = 10 ) -> Optional[str]: """ Chat function to perform a web
+  search based on the user input and generate a response using the LLM model.
  Parameters ---------- user_input : str The user input to be used for the web
   search webs : WEBS The web search instance to be used to perform the search
 max_results : int, optional The maximum number of search results to include in
     the response, by default 10 Returns ------- Optional[str] The response
 generated by the LLM model, or None if there is no response """ # Perform a web
     search based on the user input search_results: List[str] = [] for r in
     webs.text( user_input, region="wt-wt", safesearch="off", timelimit="y",
@@ -460,7 +472,10 @@
   key/value (if needed) timeout=30, disable_conversation=True, filepath=None,
        update_file=True, intro=None, rawdog=True, history_offset=10250,
       awesome_prompt=None, proxy_path=None, quiet=True ) webai_response =
 webai_bot.default(prompt) except Exception as e: print("Unexpected error:", e)
      if __name__ == "__main__": user_prompt = input("Enter your prompt: ")
 use_rawdog_with_webai(user_prompt) ``` ```shell python -m webscout.webai webai
                         --provider "phind" --rawdog ```
+               _[_T_e_l_e_g_r_a_m_]_[_I_n_s_t_a_g_r_a_m_]_[_L_i_n_k_e_d_I_n_]_[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
+                          _➤_ _V_o_r_t_e_x_'_s_ _Y_o_u_T_u_b_e_ _C_h_a_n_n_e_l
+                       _➤_ _D_e_v_s_ _D_o_ _C_o_d_e_'_s_ _Y_o_u_T_u_b_e_ _C_h_a_n_n_e_l
```

### Comparing `webscout-1.4.3/webscout.egg-info/SOURCES.txt` & `webscout-1.4.4/webscout.egg-info/SOURCES.txt`

 * *Files identical despite different names*

