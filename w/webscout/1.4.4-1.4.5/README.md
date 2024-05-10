# Comparing `tmp/webscout-1.4.4.tar.gz` & `tmp/webscout-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscout-1.4.4.tar", last modified: Fri May 10 02:44:01 2024, max compression
+gzip compressed data, was "webscout-1.4.5.tar", last modified: Fri May 10 04:43:15 2024, max compression
```

## Comparing `webscout-1.4.4.tar` & `webscout-1.4.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 02:44:01.315008 webscout-1.4.4/
-drwxrwxrwx   0        0        0        0 2024-05-10 02:43:59.854618 webscout-1.4.4/DeepWEBS/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-1.4.4/DeepWEBS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 02:43:59.869629 webscout-1.4.4/DeepWEBS/documents/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-1.4.4/DeepWEBS/documents/__init__.py
--rw-rw-rw-   0        0        0     4049 2024-05-08 15:52:48.000000 webscout-1.4.4/DeepWEBS/documents/query_results_extractor.py
--rw-rw-rw-   0        0        0     5272 2024-05-08 15:52:48.000000 webscout-1.4.4/DeepWEBS/documents/webpage_content_extractor.py
-drwxrwxrwx   0        0        0        0 2024-05-10 02:43:59.967230 webscout-1.4.4/DeepWEBS/networks/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-1.4.4/DeepWEBS/networks/__init__.py
--rw-rw-rw-   0        0        0     3183 2024-05-08 15:52:48.000000 webscout-1.4.4/DeepWEBS/networks/filepath_converter.py
--rw-rw-rw-   0        0        0     1966 2024-05-08 15:52:48.000000 webscout-1.4.4/DeepWEBS/networks/google_searcher.py
--rw-rw-rw-   0        0        0      726 2024-05-08 15:52:48.000000 webscout-1.4.4/DeepWEBS/networks/network_configs.py
--rw-rw-rw-   0        0        0     3590 2024-05-08 15:52:48.000000 webscout-1.4.4/DeepWEBS/networks/webpage_fetcher.py
-drwxrwxrwx   0        0        0        0 2024-05-10 02:43:59.988225 webscout-1.4.4/DeepWEBS/utilsdw/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-1.4.4/DeepWEBS/utilsdw/__init__.py
--rw-rw-rw-   0        0        0     2472 2024-05-08 15:52:48.000000 webscout-1.4.4/DeepWEBS/utilsdw/enver.py
--rw-rw-rw-   0        0        0     8174 2024-05-08 15:52:48.000000 webscout-1.4.4/DeepWEBS/utilsdw/logger.py
--rw-rw-rw-   0        0        0     3150 2024-05-08 15:52:48.000000 webscout-1.4.4/LICENSE.md
--rw-rw-rw-   0        0        0    43415 2024-05-10 02:44:01.311375 webscout-1.4.4/PKG-INFO
--rw-rw-rw-   0        0        0    41114 2024-05-10 02:21:13.000000 webscout-1.4.4/README.md
--rw-rw-rw-   0        0        0       42 2024-05-10 02:44:01.316036 webscout-1.4.4/setup.cfg
--rw-rw-rw-   0        0        0     2800 2024-05-10 02:22:02.000000 webscout-1.4.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-10 02:44:00.570905 webscout-1.4.4/webscout/
--rw-rw-rw-   0        0        0   226145 2024-05-09 17:13:40.000000 webscout-1.4.4/webscout/AI.py
--rw-rw-rw-   0        0        0     4710 2024-05-08 15:52:48.000000 webscout-1.4.4/webscout/AIbase.py
--rw-rw-rw-   0        0        0    33217 2024-05-09 17:15:58.000000 webscout-1.4.4/webscout/AIutel.py
--rw-rw-rw-   0        0        0     7332 2024-05-08 15:52:48.000000 webscout-1.4.4/webscout/DWEBS.py
--rw-rw-rw-   0        0        0     1910 2024-05-08 15:52:48.000000 webscout-1.4.4/webscout/LLM.py
--rw-rw-rw-   0        0        0     1090 2024-05-09 17:15:47.000000 webscout-1.4.4/webscout/__init__.py
--rw-rw-rw-   0        0        0      126 2024-05-08 15:52:48.000000 webscout-1.4.4/webscout/__main__.py
--rw-rw-rw-   0        0        0      971 2024-05-08 15:52:48.000000 webscout-1.4.4/webscout/async_providers.py
--rw-rw-rw-   0        0        0    17059 2024-05-08 15:52:48.000000 webscout-1.4.4/webscout/cli.py
--rw-rw-rw-   0        0        0      378 2024-05-08 15:52:48.000000 webscout-1.4.4/webscout/exceptions.py
--rw-rw-rw-   0        0        0    24489 2024-05-08 15:52:48.000000 webscout-1.4.4/webscout/g4f.py
--rw-rw-rw-   0        0        0      692 2024-05-08 15:52:48.000000 webscout-1.4.4/webscout/models.py
--rw-rw-rw-   0        0        0     5896 2024-05-08 15:52:48.000000 webscout-1.4.4/webscout/tempid.py
--rw-rw-rw-   0        0        0    20622 2024-05-08 15:52:48.000000 webscout-1.4.4/webscout/transcriber.py
--rw-rw-rw-   0        0        0     2603 2024-05-09 03:33:11.000000 webscout-1.4.4/webscout/utils.py
--rw-rw-rw-   0        0        0       25 2024-05-10 02:22:14.000000 webscout-1.4.4/webscout/version.py
--rw-rw-rw-   0        0        0      967 2024-05-08 15:52:48.000000 webscout-1.4.4/webscout/voice.py
--rw-rw-rw-   0        0        0    82831 2024-05-09 17:15:32.000000 webscout-1.4.4/webscout/webai.py
--rw-rw-rw-   0        0        0     3085 2024-05-08 15:52:48.000000 webscout-1.4.4/webscout/webscout_search.py
--rw-rw-rw-   0        0        0    40670 2024-05-08 15:52:48.000000 webscout-1.4.4/webscout/webscout_search_async.py
-drwxrwxrwx   0        0        0        0 2024-05-10 02:44:01.302466 webscout-1.4.4/webscout.egg-info/
--rw-rw-rw-   0        0        0    43415 2024-05-10 02:43:57.000000 webscout-1.4.4/webscout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1042 2024-05-10 02:43:58.000000 webscout-1.4.4/webscout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 02:43:57.000000 webscout-1.4.4/webscout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      197 2024-05-10 02:43:57.000000 webscout-1.4.4/webscout.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      379 2024-05-10 02:43:57.000000 webscout-1.4.4/webscout.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-10 02:43:57.000000 webscout-1.4.4/webscout.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 04:43:15.902631 webscout-1.4.5/
+drwxrwxrwx   0        0        0        0 2024-05-10 04:43:13.667609 webscout-1.4.5/DeepWEBS/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-1.4.5/DeepWEBS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 04:43:13.700147 webscout-1.4.5/DeepWEBS/documents/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-1.4.5/DeepWEBS/documents/__init__.py
+-rw-rw-rw-   0        0        0     4049 2024-05-08 15:52:48.000000 webscout-1.4.5/DeepWEBS/documents/query_results_extractor.py
+-rw-rw-rw-   0        0        0     5272 2024-05-08 15:52:48.000000 webscout-1.4.5/DeepWEBS/documents/webpage_content_extractor.py
+drwxrwxrwx   0        0        0        0 2024-05-10 04:43:13.801515 webscout-1.4.5/DeepWEBS/networks/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-1.4.5/DeepWEBS/networks/__init__.py
+-rw-rw-rw-   0        0        0     3183 2024-05-08 15:52:48.000000 webscout-1.4.5/DeepWEBS/networks/filepath_converter.py
+-rw-rw-rw-   0        0        0     1966 2024-05-08 15:52:48.000000 webscout-1.4.5/DeepWEBS/networks/google_searcher.py
+-rw-rw-rw-   0        0        0      726 2024-05-08 15:52:48.000000 webscout-1.4.5/DeepWEBS/networks/network_configs.py
+-rw-rw-rw-   0        0        0     3590 2024-05-08 15:52:48.000000 webscout-1.4.5/DeepWEBS/networks/webpage_fetcher.py
+drwxrwxrwx   0        0        0        0 2024-05-10 04:43:13.965411 webscout-1.4.5/DeepWEBS/utilsdw/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-1.4.5/DeepWEBS/utilsdw/__init__.py
+-rw-rw-rw-   0        0        0     2472 2024-05-08 15:52:48.000000 webscout-1.4.5/DeepWEBS/utilsdw/enver.py
+-rw-rw-rw-   0        0        0     8174 2024-05-08 15:52:48.000000 webscout-1.4.5/DeepWEBS/utilsdw/logger.py
+-rw-rw-rw-   0        0        0     3150 2024-05-08 15:52:48.000000 webscout-1.4.5/LICENSE.md
+-rw-rw-rw-   0        0        0    43415 2024-05-10 04:43:15.889556 webscout-1.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0    41114 2024-05-10 02:21:13.000000 webscout-1.4.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-10 04:43:15.903626 webscout-1.4.5/setup.cfg
+-rw-rw-rw-   0        0        0     2800 2024-05-10 04:42:14.000000 webscout-1.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 04:43:15.716486 webscout-1.4.5/webscout/
+-rw-rw-rw-   0        0        0   226145 2024-05-09 17:13:40.000000 webscout-1.4.5/webscout/AI.py
+-rw-rw-rw-   0        0        0     4710 2024-05-08 15:52:48.000000 webscout-1.4.5/webscout/AIbase.py
+-rw-rw-rw-   0        0        0    33217 2024-05-09 17:15:58.000000 webscout-1.4.5/webscout/AIutel.py
+-rw-rw-rw-   0        0        0     7332 2024-05-08 15:52:48.000000 webscout-1.4.5/webscout/DWEBS.py
+-rw-rw-rw-   0        0        0     1910 2024-05-08 15:52:48.000000 webscout-1.4.5/webscout/LLM.py
+-rw-rw-rw-   0        0        0     1090 2024-05-09 17:15:47.000000 webscout-1.4.5/webscout/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-05-08 15:52:48.000000 webscout-1.4.5/webscout/__main__.py
+-rw-rw-rw-   0        0        0      971 2024-05-08 15:52:48.000000 webscout-1.4.5/webscout/async_providers.py
+-rw-rw-rw-   0        0        0    17059 2024-05-08 15:52:48.000000 webscout-1.4.5/webscout/cli.py
+-rw-rw-rw-   0        0        0      378 2024-05-08 15:52:48.000000 webscout-1.4.5/webscout/exceptions.py
+-rw-rw-rw-   0        0        0    24489 2024-05-08 15:52:48.000000 webscout-1.4.5/webscout/g4f.py
+-rw-rw-rw-   0        0        0      692 2024-05-08 15:52:48.000000 webscout-1.4.5/webscout/models.py
+-rw-rw-rw-   0        0        0     5896 2024-05-08 15:52:48.000000 webscout-1.4.5/webscout/tempid.py
+-rw-rw-rw-   0        0        0    20622 2024-05-08 15:52:48.000000 webscout-1.4.5/webscout/transcriber.py
+-rw-rw-rw-   0        0        0     2603 2024-05-09 03:33:11.000000 webscout-1.4.5/webscout/utils.py
+-rw-rw-rw-   0        0        0       25 2024-05-10 04:42:09.000000 webscout-1.4.5/webscout/version.py
+-rw-rw-rw-   0        0        0      967 2024-05-08 15:52:48.000000 webscout-1.4.5/webscout/voice.py
+-rw-rw-rw-   0        0        0    82831 2024-05-09 17:15:32.000000 webscout-1.4.5/webscout/webai.py
+-rw-rw-rw-   0        0        0     3393 2024-05-10 04:31:54.000000 webscout-1.4.5/webscout/webscout_search.py
+-rw-rw-rw-   0        0        0    42902 2024-05-10 04:39:59.000000 webscout-1.4.5/webscout/webscout_search_async.py
+drwxrwxrwx   0        0        0        0 2024-05-10 04:43:15.882006 webscout-1.4.5/webscout.egg-info/
+-rw-rw-rw-   0        0        0    43415 2024-05-10 04:43:12.000000 webscout-1.4.5/webscout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1042 2024-05-10 04:43:13.000000 webscout-1.4.5/webscout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 04:43:12.000000 webscout-1.4.5/webscout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      197 2024-05-10 04:43:12.000000 webscout-1.4.5/webscout.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      379 2024-05-10 04:43:12.000000 webscout-1.4.5/webscout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-10 04:43:12.000000 webscout-1.4.5/webscout.egg-info/top_level.txt
```

### Comparing `webscout-1.4.4/DeepWEBS/documents/query_results_extractor.py` & `webscout-1.4.5/DeepWEBS/documents/query_results_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.4/DeepWEBS/documents/webpage_content_extractor.py` & `webscout-1.4.5/DeepWEBS/documents/webpage_content_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.4/DeepWEBS/networks/filepath_converter.py` & `webscout-1.4.5/DeepWEBS/networks/filepath_converter.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.4/DeepWEBS/networks/google_searcher.py` & `webscout-1.4.5/DeepWEBS/networks/google_searcher.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.4/DeepWEBS/networks/network_configs.py` & `webscout-1.4.5/DeepWEBS/networks/network_configs.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.4/DeepWEBS/networks/webpage_fetcher.py` & `webscout-1.4.5/DeepWEBS/networks/webpage_fetcher.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.4/DeepWEBS/utilsdw/enver.py` & `webscout-1.4.5/DeepWEBS/utilsdw/enver.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.4/DeepWEBS/utilsdw/logger.py` & `webscout-1.4.5/DeepWEBS/utilsdw/logger.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.4/LICENSE.md` & `webscout-1.4.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `webscout-1.4.4/PKG-INFO` & `webscout-1.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 1.4.4
+Version: 1.4.5
 Summary: Search for anything using the Google, DuckDuckGo, phind.com. Also containes AI models, can transcribe yt videos, temporary email and phone number generation, have TTS support and webai(terminal gpt and open interpeter)
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: webscout Version: 1.4.4 Summary: Search for
+Metadata-Version: 2.1 Name: webscout Version: 1.4.5 Summary: Search for
 anything using the Google, DuckDuckGo, phind.com. Also containes AI models, can
 transcribe yt videos, temporary email and phone number generation, have TTS
 support and webai(terminal gpt and open interpeter) Author: OEvortex Author-
 email: helpingai5@gmail.com License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout Project-URL:
 Tracker, https://github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube,
```

### Comparing `webscout-1.4.4/README.md` & `webscout-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `webscout-1.4.4/setup.py` & `webscout-1.4.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="webscout",
-    version="1.4.4", 
+    version="1.4.5", 
     description="Search for anything using the Google, DuckDuckGo, phind.com. Also containes AI models, can transcribe yt videos, temporary email and phone number generation, have TTS support and webai(terminal gpt and open interpeter)",
     long_description=README,
     long_description_content_type="text/markdown",
     author="OEvortex",
     author_email="helpingai5@gmail.com",
     packages=find_packages(),
     classifiers=[
```

### Comparing `webscout-1.4.4/webscout/AI.py` & `webscout-1.4.5/webscout/AI.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.4/webscout/AIbase.py` & `webscout-1.4.5/webscout/AIbase.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.4/webscout/AIutel.py` & `webscout-1.4.5/webscout/AIutel.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.4/webscout/DWEBS.py` & `webscout-1.4.5/webscout/DWEBS.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.4/webscout/LLM.py` & `webscout-1.4.5/webscout/LLM.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.4/webscout/__init__.py` & `webscout-1.4.5/webscout/__init__.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.4/webscout/async_providers.py` & `webscout-1.4.5/webscout/async_providers.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.4/webscout/cli.py` & `webscout-1.4.5/webscout/cli.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.4/webscout/g4f.py` & `webscout-1.4.5/webscout/g4f.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.4/webscout/models.py` & `webscout-1.4.5/webscout/models.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.4/webscout/tempid.py` & `webscout-1.4.5/webscout/tempid.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.4/webscout/transcriber.py` & `webscout-1.4.5/webscout/transcriber.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.4/webscout/utils.py` & `webscout-1.4.5/webscout/utils.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.4/webscout/voice.py` & `webscout-1.4.5/webscout/voice.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.4/webscout/webai.py` & `webscout-1.4.5/webscout/webai.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.4/webscout/webscout_search_async.py` & `webscout-1.4.5/webscout/webscout_search_async.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import asyncio
 import logging
 import warnings
 from concurrent.futures import ThreadPoolExecutor
 from contextlib import suppress
 from datetime import datetime, timezone
 from decimal import Decimal
-from functools import partial
+from functools import cached_property, partial
 from itertools import cycle, islice
 from types import TracebackType
-from typing import Dict, List, Optional, Tuple, Union
+from typing import Dict, List, Optional, Tuple, Type, Union, cast
 
 from curl_cffi import requests
 
 try:
     from lxml.html import HTMLParser as LHTMLParser
     from lxml.html import document_fromstring
 
@@ -30,100 +30,102 @@
     json_loads,
 )
 
 logger = logging.getLogger("webscout_search.AsyncWEBS")
 
 
 class AsyncWEBS:
-    """Webscout async class to get search results from duckduckgo.com."""
+    """webscout_search async class to get search results from duckduckgo.com."""
 
     _executor: Optional[ThreadPoolExecutor] = None
 
     def __init__(
         self,
         headers: Optional[Dict[str, str]] = None,
-        proxies: Union[Dict[str, str], str, None] = None,
+        proxy: Optional[str] = None,
+        proxies: Union[Dict[str, str], str, None] = None,  # deprecated
         timeout: Optional[int] = 10,
     ) -> None:
         """Initialize the AsyncWEBS object.
 
         Args:
             headers (dict, optional): Dictionary of headers for the HTTP client. Defaults to None.
-            proxies (Union[dict, str], optional): Proxies for the HTTP client (can be dict or str). Defaults to None.
+            proxy (str, optional): proxy for the HTTP client, supports http/https/socks5 protocols.
+                example: "http://user:pass@example.com:3128". Defaults to None.
             timeout (int, optional): Timeout value for the HTTP client. Defaults to 10.
         """
-        self.proxies = {"all": proxies} if isinstance(proxies, str) else proxies
+        self.proxy: Optional[str] = proxy
+        assert self.proxy is None or isinstance(self.proxy, str), "proxy must be a str"
+        if not proxy and proxies:
+            warnings.warn("'proxies' is deprecated, use 'proxy' instead.", stacklevel=1)
+            self.proxy = proxies.get("http") or proxies.get("https") if isinstance(proxies, dict) else proxies
         self._asession = requests.AsyncSession(
             headers=headers,
-            proxies=self.proxies,
+            proxy=self.proxy,
             timeout=timeout,
             impersonate="chrome",
             allow_redirects=False,
         )
         self._asession.headers["Referer"] = "https://duckduckgo.com/"
-        self._parser: Optional[LHTMLParser] = None
         self._exception_event = asyncio.Event()
-        self._exit_done = False
 
     async def __aenter__(self) -> "AsyncWEBS":
         return self
 
     async def __aexit__(
         self,
-        exc_type: Optional[BaseException] = None,
+        exc_type: Optional[Type[BaseException]] = None,
         exc_val: Optional[BaseException] = None,
         exc_tb: Optional[TracebackType] = None,
     ) -> None:
-        await self._session_close()
+        await self._asession.__aexit__(exc_type, exc_val, exc_tb)  # type: ignore
 
     def __del__(self) -> None:
-        if self._exit_done is False:
-            asyncio.create_task(self._session_close())
+        if hasattr(self, "_asession") and self._asession._closed is False:
+            with suppress(RuntimeError, RuntimeWarning):
+                asyncio.create_task(self._asession.close())  # type: ignore
 
-    async def _session_close(self) -> None:
-        """Close the curl-cffi async session."""
-        if self._exit_done is False:
-            await self._asession.close()
-            self._exit_done = True
-
-    def _get_parser(self) -> "LHTMLParser":
+    @cached_property
+    def parser(self) -> Optional["LHTMLParser"]:
         """Get HTML parser."""
-        if self._parser is None:
-            self._parser = LHTMLParser(remove_blank_text=True, remove_comments=True, remove_pis=True, collect_ids=False)
-        return self._parser
+        return LHTMLParser(remove_blank_text=True, remove_comments=True, remove_pis=True, collect_ids=False)
 
-    def _get_executor(self, max_workers: int = 1) -> ThreadPoolExecutor:
+    @classmethod
+    def _get_executor(cls, max_workers: int = 1) -> ThreadPoolExecutor:
         """Get ThreadPoolExecutor. Default max_workers=1, because >=2 leads to a big overhead"""
-        if AsyncWEBS._executor is None:
-            AsyncWEBS._executor = ThreadPoolExecutor(max_workers=max_workers)
-        return AsyncWEBS._executor
+        if cls._executor is None:
+            cls._executor = ThreadPoolExecutor(max_workers=max_workers)
+        return cls._executor
+
+    @property
+    def executor(cls) -> Optional[ThreadPoolExecutor]:
+        return cls._get_executor()
 
     async def _aget_url(
         self,
         method: str,
         url: str,
         data: Optional[Union[Dict[str, str], bytes]] = None,
         params: Optional[Dict[str, str]] = None,
     ) -> bytes:
         if self._exception_event.is_set():
             raise WebscoutE("Exception occurred in previous call.")
         try:
-            resp = await self._asession.request(method, url, data=data, params=params, stream=True)
-            resp_content: bytes = await resp.acontent()
+            resp = await self._asession.request(method, url, data=data, params=params)
         except Exception as ex:
             self._exception_event.set()
             if "time" in str(ex).lower():
                 raise TimeoutE(f"{url} {type(ex).__name__}: {ex}") from ex
             raise WebscoutE(f"{url} {type(ex).__name__}: {ex}") from ex
-        logger.debug(f"_aget_url() {resp.url} {resp.status_code} {resp.elapsed:.2f} {len(resp_content)}")
+        logger.debug(f"_aget_url() {resp.url} {resp.status_code} {resp.elapsed:.2f} {len(resp.content)}")
         if resp.status_code == 200:
-            return resp_content
+            return cast(bytes, resp.content)
         self._exception_event.set()
         if resp.status_code in (202, 301, 403):
-            raise RatelimitE(f"{resp.url} {resp.status_code}")
+            raise RatelimitE(f"{resp.url} {resp.status_code} Ratelimit")
         raise WebscoutE(f"{resp.url} return None. {params=} {data=}")
 
     async def _aget_vqd(self, keywords: str) -> str:
         """Get vqd value for a search query."""
         resp_content = await self._aget_url("POST", "https://duckduckgo.com", data={"q": keywords})
         return _extract_vqd(resp_content, keywords)
 
@@ -132,15 +134,15 @@
         keywords: str,
         region: str = "wt-wt",
         safesearch: str = "moderate",
         timelimit: Optional[str] = None,
         backend: str = "api",
         max_results: Optional[int] = None,
     ) -> List[Dict[str, str]]:
-        """Webscout text search generator. Query params: https://duckduckgo.com/params.
+        """webscout text search generator. Query params: https://duckduckgo.com/params.
 
         Args:
             keywords: keywords for query.
             region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
             safesearch: on, moderate, off. Defaults to "moderate".
             timelimit: d, w, m, y. Defaults to None.
             backend: api, html, lite. Defaults to api.
@@ -149,15 +151,15 @@
                 lite - collect data from https://lite.duckduckgo.com.
             max_results: max number of results. If None, returns results only from the first response. Defaults to None.
 
         Returns:
             List of dictionaries with search results, or None if there was an error.
 
         Raises:
-            WebscoutE: Base exception for Webscout errors.
+            WebscoutE: Base exception for webscout_search errors.
             RatelimitE: Inherits from WebscoutE, raised for exceeding API request rate limits.
             TimeoutE: Inherits from WebscoutE, raised for API request timeouts.
         """
         if LXML_AVAILABLE is False and backend != "api":
             backend = "api"
             warnings.warn("lxml is not installed. Using backend='api'.", stacklevel=2)
 
@@ -173,28 +175,28 @@
         self,
         keywords: str,
         region: str = "wt-wt",
         safesearch: str = "moderate",
         timelimit: Optional[str] = None,
         max_results: Optional[int] = None,
     ) -> List[Dict[str, str]]:
-        """Webscout text search generator. Query params: https://duckduckgo.com/params.
+        """webscout text search generator. Query params: https://duckduckgo.com/params.
 
         Args:
             keywords: keywords for query.
             region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
             safesearch: on, moderate, off. Defaults to "moderate".
             timelimit: d, w, m, y. Defaults to None.
             max_results: max number of results. If None, returns results only from the first response. Defaults to None.
 
         Returns:
             List of dictionaries with search results.
 
         Raises:
-            WebscoutE: Base exception for Webscout errors.
+            WebscoutE: Base exception for webscout_search errors.
             RatelimitE: Inherits from WebscoutE, raised for exceeding API request rate limits.
             TimeoutE: Inherits from WebscoutE, raised for API request timeouts.
         """
         assert keywords, "keywords is mandatory"
 
         vqd = await self._aget_vqd(keywords)
 
@@ -237,44 +239,52 @@
                         result = {
                             "title": _normalize(row["t"]),
                             "href": _normalize_url(href),
                             "body": body,
                         }
                         results[priority] = result
 
-        tasks = [_text_api_page(0, 0)]
+        tasks = [asyncio.create_task(_text_api_page(0, 0))]
         if max_results:
             max_results = min(max_results, 500)
-            tasks.extend(_text_api_page(s, i) for i, s in enumerate(range(23, max_results, 50), start=1))
-        await asyncio.gather(*tasks)
+            tasks.extend(
+                asyncio.create_task(_text_api_page(s, i)) for i, s in enumerate(range(23, max_results, 50), start=1)
+            )
+        try:
+            await asyncio.gather(*tasks)
+        except Exception as e:
+            for task in tasks:
+                task.cancel()
+            await asyncio.gather(*tasks, return_exceptions=True)
+            raise e
 
         return list(islice(filter(None, results), max_results))
 
     async def _text_html(
         self,
         keywords: str,
         region: str = "wt-wt",
         safesearch: str = "moderate",
         timelimit: Optional[str] = None,
         max_results: Optional[int] = None,
     ) -> List[Dict[str, str]]:
-        """Webscout text search generator. Query params: https://duckduckgo.com/params.
+        """webscout text search generator. Query params: https://duckduckgo.com/params.
 
         Args:
             keywords: keywords for query.
             region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
             safesearch: on, moderate, off. Defaults to "moderate".
             timelimit: d, w, m, y. Defaults to None.
             max_results: max number of results. If None, returns results only from the first response. Defaults to None.
 
         Returns:
             List of dictionaries with search results.
 
         Raises:
-            WebscoutE: Base exception for Webscout errors.
+            WebscoutE: Base exception for webscout_search errors.
             RatelimitE: Inherits from WebscoutE, raised for exceeding API request rate limits.
             TimeoutE: Inherits from WebscoutE, raised for API request timeouts.
         """
         assert keywords, "keywords is mandatory"
 
         self._asession.headers["Referer"] = "https://html.duckduckgo.com/"
         safesearch_base = {"on": "1", "moderate": "-1", "off": "-2"}
@@ -298,15 +308,15 @@
             priority = page * 100
             payload["s"] = f"{s}"
             resp_content = await self._aget_url("POST", "https://html.duckduckgo.com/html", data=payload)
             if b"No  results." in resp_content:
                 return
 
             tree = await self._asession.loop.run_in_executor(
-                self._get_executor(), partial(document_fromstring, resp_content, self._get_parser())
+                self.executor, partial(document_fromstring, resp_content, self.parser)
             )
 
             for e in tree.xpath("//div[h2]"):
                 href = e.xpath("./a/@href")
                 href = href[0] if href else None
                 if (
                     href
@@ -323,42 +333,50 @@
                     result = {
                         "title": _normalize(title[0]),
                         "href": _normalize_url(href),
                         "body": _normalize("".join(body)),
                     }
                     results[priority] = result
 
-        tasks = [_text_html_page(0, 0)]
+        tasks = [asyncio.create_task(_text_html_page(0, 0))]
         if max_results:
             max_results = min(max_results, 500)
-            tasks.extend(_text_html_page(s, i) for i, s in enumerate(range(23, max_results, 50), start=1))
-        await asyncio.gather(*tasks)
+            tasks.extend(
+                asyncio.create_task(_text_html_page(s, i)) for i, s in enumerate(range(23, max_results, 50), start=1)
+            )
+        try:
+            await asyncio.gather(*tasks)
+        except Exception as e:
+            for task in tasks:
+                task.cancel()
+            await asyncio.gather(*tasks, return_exceptions=True)
+            raise e
 
         return list(islice(filter(None, results), max_results))
 
     async def _text_lite(
         self,
         keywords: str,
         region: str = "wt-wt",
         timelimit: Optional[str] = None,
         max_results: Optional[int] = None,
     ) -> List[Dict[str, str]]:
-        """Webscout text search generator. Query params: https://duckduckgo.com/params.
+        """webscout text search generator. Query params: https://duckduckgo.com/params.
 
         Args:
             keywords: keywords for query.
             region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
             timelimit: d, w, m, y. Defaults to None.
             max_results: max number of results. If None, returns results only from the first response. Defaults to None.
 
         Returns:
             List of dictionaries with search results.
 
         Raises:
-            WebscoutE: Base exception for Webscout errors.
+            WebscoutE: Base exception for webscout_search errors.
             RatelimitE: Inherits from WebscoutE, raised for exceeding API request rate limits.
             TimeoutE: Inherits from WebscoutE, raised for API request timeouts.
         """
         assert keywords, "keywords is mandatory"
 
         self._asession.headers["Referer"] = "https://lite.duckduckgo.com/"
         payload = {
@@ -377,15 +395,15 @@
             priority = page * 100
             payload["s"] = f"{s}"
             resp_content = await self._aget_url("POST", "https://lite.duckduckgo.com/lite/", data=payload)
             if b"No more results." in resp_content:
                 return
 
             tree = await self._asession.loop.run_in_executor(
-                self._get_executor(), partial(document_fromstring, resp_content, self._get_parser())
+                self.executor, partial(document_fromstring, resp_content, self.parser)
             )
 
             data = zip(cycle(range(1, 5)), tree.xpath("//table[last()]//tr"))
             for i, e in data:
                 if i == 1:
                     href = e.xpath(".//a//@href")
                     href = href[0] if href else None
@@ -406,19 +424,27 @@
                     result = {
                         "title": _normalize(title),
                         "href": _normalize_url(href),
                         "body": _normalize(body),
                     }
                     results[priority] = result
 
-        tasks = [_text_lite_page(0, 0)]
+        tasks = [asyncio.create_task(_text_lite_page(0, 0))]
         if max_results:
             max_results = min(max_results, 500)
-            tasks.extend(_text_lite_page(s, i) for i, s in enumerate(range(23, max_results, 50), start=1))
-        await asyncio.gather(*tasks)
+            tasks.extend(
+                asyncio.create_task(_text_lite_page(s, i)) for i, s in enumerate(range(23, max_results, 50), start=1)
+            )
+        try:
+            await asyncio.gather(*tasks)
+        except Exception as e:
+            for task in tasks:
+                task.cancel()
+            await asyncio.gather(*tasks, return_exceptions=True)
+            raise e
 
         return list(islice(filter(None, results), max_results))
 
     async def images(
         self,
         keywords: str,
         region: str = "wt-wt",
@@ -427,15 +453,15 @@
         size: Optional[str] = None,
         color: Optional[str] = None,
         type_image: Optional[str] = None,
         layout: Optional[str] = None,
         license_image: Optional[str] = None,
         max_results: Optional[int] = None,
     ) -> List[Dict[str, str]]:
-        """Webscout images search. Query params: https://duckduckgo.com/params.
+        """webscout images search. Query params: https://duckduckgo.com/params.
 
         Args:
             keywords: keywords for query.
             region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
             safesearch: on, moderate, off. Defaults to "moderate".
             timelimit: Day, Week, Month, Year. Defaults to None.
             size: Small, Medium, Large, Wallpaper. Defaults to None.
@@ -450,15 +476,15 @@
                 Use Commercially). Defaults to None.
             max_results: max number of results. If None, returns results only from the first response. Defaults to None.
 
         Returns:
             List of dictionaries with images search results.
 
         Raises:
-            WebscoutE: Base exception for Webscout errors.
+            WebscoutE: Base exception for webscout_search errors.
             RatelimitE: Inherits from WebscoutE, raised for exceeding API request rate limits.
             TimeoutE: Inherits from WebscoutE, raised for API request timeouts.
         """
         assert keywords, "keywords is mandatory"
 
         vqd = await self._aget_vqd(keywords)
 
@@ -501,34 +527,42 @@
                         "url": _normalize_url(row["url"]),
                         "height": row["height"],
                         "width": row["width"],
                         "source": row["source"],
                     }
                     results[priority] = result
 
-        tasks = [_images_page(0, page=0)]
+        tasks = [asyncio.create_task(_images_page(0, page=0))]
         if max_results:
             max_results = min(max_results, 500)
-            tasks.extend(_images_page(s, i) for i, s in enumerate(range(100, max_results, 100), start=1))
-        await asyncio.gather(*tasks)
+            tasks.extend(
+                asyncio.create_task(_images_page(s, i)) for i, s in enumerate(range(100, max_results, 100), start=1)
+            )
+        try:
+            await asyncio.gather(*tasks)
+        except Exception as e:
+            for task in tasks:
+                task.cancel()
+            await asyncio.gather(*tasks, return_exceptions=True)
+            raise e
 
         return list(islice(filter(None, results), max_results))
 
     async def videos(
         self,
         keywords: str,
         region: str = "wt-wt",
         safesearch: str = "moderate",
         timelimit: Optional[str] = None,
         resolution: Optional[str] = None,
         duration: Optional[str] = None,
         license_videos: Optional[str] = None,
         max_results: Optional[int] = None,
     ) -> List[Dict[str, str]]:
-        """Webscout videos search. Query params: https://duckduckgo.com/params.
+        """webscout videos search. Query params: https://duckduckgo.com/params.
 
         Args:
             keywords: keywords for query.
             region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
             safesearch: on, moderate, off. Defaults to "moderate".
             timelimit: d, w, m. Defaults to None.
             resolution: high, standart. Defaults to None.
@@ -536,15 +570,15 @@
             license_videos: creativeCommon, youtube. Defaults to None.
             max_results: max number of results. If None, returns results only from the first response. Defaults to None.
 
         Returns:
             List of dictionaries with videos search results.
 
         Raises:
-            WebscoutE: Base exception for Webscout errors.
+            WebscoutE: Base exception for webscout_search errors.
             RatelimitE: Inherits from WebscoutE, raised for exceeding API request rate limits.
             TimeoutE: Inherits from WebscoutE, raised for API request timeouts.
         """
         assert keywords, "keywords is mandatory"
 
         vqd = await self._aget_vqd(keywords)
 
@@ -575,44 +609,52 @@
 
             for row in page_data:
                 if row["content"] not in cache:
                     cache.add(row["content"])
                     priority += 1
                     results[priority] = row
 
-        tasks = [_videos_page(0, 0)]
+        tasks = [asyncio.create_task(_videos_page(0, 0))]
         if max_results:
             max_results = min(max_results, 400)
-            tasks.extend(_videos_page(s, i) for i, s in enumerate(range(59, max_results, 59), start=1))
-        await asyncio.gather(*tasks)
+            tasks.extend(
+                asyncio.create_task(_videos_page(s, i)) for i, s in enumerate(range(59, max_results, 59), start=1)
+            )
+        try:
+            await asyncio.gather(*tasks)
+        except Exception as e:
+            for task in tasks:
+                task.cancel()
+            await asyncio.gather(*tasks, return_exceptions=True)
+            raise e
 
         return list(islice(filter(None, results), max_results))
 
     async def news(
         self,
         keywords: str,
         region: str = "wt-wt",
         safesearch: str = "moderate",
         timelimit: Optional[str] = None,
         max_results: Optional[int] = None,
     ) -> List[Dict[str, str]]:
-        """Webscout news search. Query params: https://duckduckgo.com/params.
+        """webscout news search. Query params: https://duckduckgo.com/params.
 
         Args:
             keywords: keywords for query.
             region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
             safesearch: on, moderate, off. Defaults to "moderate".
             timelimit: d, w, m. Defaults to None.
             max_results: max number of results. If None, returns results only from the first response. Defaults to None.
 
         Returns:
             List of dictionaries with news search results.
 
         Raises:
-            WebscoutE: Base exception for Webscout errors.
+            WebscoutE: Base exception for webscout_search errors.
             RatelimitE: Inherits from WebscoutE, raised for exceeding API request rate limits.
             TimeoutE: Inherits from WebscoutE, raised for API request timeouts.
         """
         assert keywords, "keywords is mandatory"
 
         vqd = await self._aget_vqd(keywords)
 
@@ -649,33 +691,41 @@
                         "body": _normalize(row["excerpt"]),
                         "url": _normalize_url(row["url"]),
                         "image": _normalize_url(image_url),
                         "source": row["source"],
                     }
                     results[priority] = result
 
-        tasks = [_news_page(0, 0)]
+        tasks = [asyncio.create_task(_news_page(0, 0))]
         if max_results:
             max_results = min(max_results, 200)
-            tasks.extend(_news_page(s, i) for i, s in enumerate(range(29, max_results, 29), start=1))
-        await asyncio.gather(*tasks)
+            tasks.extend(
+                asyncio.create_task(_news_page(s, i)) for i, s in enumerate(range(29, max_results, 29), start=1)
+            )
+        try:
+            await asyncio.gather(*tasks)
+        except Exception as e:
+            for task in tasks:
+                task.cancel()
+            await asyncio.gather(*tasks, return_exceptions=True)
+            raise e
 
         return list(islice(filter(None, results), max_results))
 
     async def answers(self, keywords: str) -> List[Dict[str, str]]:
-        """Webscout instant answers. Query params: https://duckduckgo.com/params.
+        """webscout instant answers. Query params: https://duckduckgo.com/params.
 
         Args:
             keywords: keywords for query,
 
         Returns:
             List of dictionaries with instant answers results.
 
         Raises:
-            WebscoutE: Base exception for Webscout errors.
+            WebscoutE: Base exception for webscout_search errors.
             RatelimitE: Inherits from WebscoutE, raised for exceeding API request rate limits.
             TimeoutE: Inherits from WebscoutE, raised for API request timeouts.
         """
         assert keywords, "keywords is mandatory"
 
         payload = {
             "q": f"what is {keywords}",
@@ -729,25 +779,25 @@
                             "url": subrow["FirstURL"],
                         }
                     )
 
         return results
 
     async def suggestions(self, keywords: str, region: str = "wt-wt") -> List[Dict[str, str]]:
-        """Webscout suggestions. Query params: https://duckduckgo.com/params.
+        """webscout suggestions. Query params: https://duckduckgo.com/params.
 
         Args:
             keywords: keywords for query.
             region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
 
         Returns:
             List of dictionaries with suggestions results.
 
         Raises:
-            WebscoutE: Base exception for Webscout errors.
+            WebscoutE: Base exception for webscout_search errors.
             RatelimitE: Inherits from WebscoutE, raised for exceeding API request rate limits.
             TimeoutE: Inherits from WebscoutE, raised for API request timeouts.
         """
         assert keywords, "keywords is mandatory"
 
         payload = {
             "q": keywords,
@@ -768,15 +818,15 @@
         country: Optional[str] = None,
         postalcode: Optional[str] = None,
         latitude: Optional[str] = None,
         longitude: Optional[str] = None,
         radius: int = 0,
         max_results: Optional[int] = None,
     ) -> List[Dict[str, str]]:
-        """Webscout maps search. Query params: https://duckduckgo.com/params.
+        """webscout maps search. Query params: https://duckduckgo.com/params.
 
         Args:
             keywords: keywords for query
             place: if set, the other parameters are not used. Defaults to None.
             street: house number/street. Defaults to None.
             city: city of search. Defaults to None.
             county: county of search. Defaults to None.
@@ -789,15 +839,15 @@
             radius: expand the search square by the distance in kilometers. Defaults to 0.
             max_results: max number of results. If None, returns results only from the first response. Defaults to None.
 
         Returns:
             List of dictionaries with maps search results, or None if there was an error.
 
         Raises:
-            WebscoutE: Base exception for Webscout errors.
+            WebscoutE: Base exception for webscout_search errors.
             RatelimitE: Inherits from WebscoutE, raised for exceeding API request rate limits.
             TimeoutE: Inherits from WebscoutE, raised for API request timeouts.
         """
         assert keywords, "keywords is mandatory"
 
         vqd = await self._aget_vqd(keywords)
 
@@ -941,26 +991,26 @@
                 break
 
         return list(islice(results, max_results))
 
     async def translate(
         self, keywords: Union[List[str], str], from_: Optional[str] = None, to: str = "en"
     ) -> List[Dict[str, str]]:
-        """Webscout translate.
+        """webscout translate.
 
         Args:
             keywords: string or list of strings to translate.
             from_: translate from (defaults automatically). Defaults to None.
             to: what language to translate. Defaults to "en".
 
         Returns:
             List od dictionaries with translated keywords.
 
         Raises:
-            WebscoutE: Base exception for Webscout errors.
+            WebscoutE: Base exception for webscout_search errors.
             RatelimitE: Inherits from WebscoutE, raised for exceeding API request rate limits.
             TimeoutE: Inherits from WebscoutE, raised for API request timeouts.
         """
         assert keywords, "keywords is mandatory"
 
         vqd = await self._aget_vqd("translate")
 
@@ -983,11 +1033,17 @@
             )
             page_data = json_loads(resp_content)
             page_data["original"] = keyword
             results.append(page_data)
 
         if isinstance(keywords, str):
             keywords = [keywords]
-        tasks = [_translate_keyword(keyword) for keyword in keywords]
-        await asyncio.gather(*tasks)
+        tasks = [asyncio.create_task(_translate_keyword(keyword)) for keyword in keywords]
+        try:
+            await asyncio.gather(*tasks)
+        except Exception as e:
+            for task in tasks:
+                task.cancel()
+            await asyncio.gather(*tasks, return_exceptions=True)
+            raise e
 
         return results
```

### Comparing `webscout-1.4.4/webscout.egg-info/PKG-INFO` & `webscout-1.4.5/webscout.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 1.4.4
+Version: 1.4.5
 Summary: Search for anything using the Google, DuckDuckGo, phind.com. Also containes AI models, can transcribe yt videos, temporary email and phone number generation, have TTS support and webai(terminal gpt and open interpeter)
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: webscout Version: 1.4.4 Summary: Search for
+Metadata-Version: 2.1 Name: webscout Version: 1.4.5 Summary: Search for
 anything using the Google, DuckDuckGo, phind.com. Also containes AI models, can
 transcribe yt videos, temporary email and phone number generation, have TTS
 support and webai(terminal gpt and open interpeter) Author: OEvortex Author-
 email: helpingai5@gmail.com License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout Project-URL:
 Tracker, https://github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube,
```

### Comparing `webscout-1.4.4/webscout.egg-info/SOURCES.txt` & `webscout-1.4.5/webscout.egg-info/SOURCES.txt`

 * *Files identical despite different names*

