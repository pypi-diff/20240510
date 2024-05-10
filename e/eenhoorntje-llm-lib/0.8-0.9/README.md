# Comparing `tmp/eenhoorntje_llm_lib-0.8.tar.gz` & `tmp/eenhoorntje_llm_lib-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eenhoorntje_llm_lib-0.8.tar", last modified: Mon Apr 22 03:03:45 2024, max compression
+gzip compressed data, was "eenhoorntje_llm_lib-0.9.tar", last modified: Mon Apr 22 03:33:36 2024, max compression
```

## Comparing `eenhoorntje_llm_lib-0.8.tar` & `eenhoorntje_llm_lib-0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 03:03:45.979712 eenhoorntje_llm_lib-0.8/
--rw-rw-rw-   0        0        0      284 2024-04-22 03:03:45.978715 eenhoorntje_llm_lib-0.8/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-20 02:23:05.000000 eenhoorntje_llm_lib-0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-22 03:03:45.966747 eenhoorntje_llm_lib-0.8/eenhoorntje_llm_lib/
--rw-rw-rw-   0        0        0        0 2024-04-18 09:27:19.000000 eenhoorntje_llm_lib-0.8/eenhoorntje_llm_lib/__init__.py
--rw-rw-rw-   0        0        0     1634 2024-04-20 01:20:42.000000 eenhoorntje_llm_lib-0.8/eenhoorntje_llm_lib/deepl.py
--rw-rw-rw-   0        0        0     2437 2024-04-20 01:57:53.000000 eenhoorntje_llm_lib-0.8/eenhoorntje_llm_lib/gemini.py
--rw-rw-rw-   0        0        0    11811 2024-04-20 02:11:12.000000 eenhoorntje_llm_lib-0.8/eenhoorntje_llm_lib/language_codes.py
--rw-rw-rw-   0        0        0     1457 2024-04-22 02:59:55.000000 eenhoorntje_llm_lib-0.8/eenhoorntje_llm_lib/llm.py
--rw-rw-rw-   0        0        0     1988 2024-04-18 09:36:38.000000 eenhoorntje_llm_lib-0.8/eenhoorntje_llm_lib/llm_cache.py
--rw-rw-rw-   0        0        0      882 2024-04-20 02:21:34.000000 eenhoorntje_llm_lib-0.8/eenhoorntje_llm_lib/translate.py
--rw-rw-rw-   0        0        0     1558 2024-04-20 02:21:34.000000 eenhoorntje_llm_lib-0.8/eenhoorntje_llm_lib/translate_llm.py
--rw-rw-rw-   0        0        0      938 2024-04-22 03:03:43.000000 eenhoorntje_llm_lib-0.8/eenhoorntje_llm_lib/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-22 03:03:45.977718 eenhoorntje_llm_lib-0.8/eenhoorntje_llm_lib.egg-info/
--rw-rw-rw-   0        0        0      284 2024-04-22 03:03:45.000000 eenhoorntje_llm_lib-0.8/eenhoorntje_llm_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2024-04-22 03:03:45.000000 eenhoorntje_llm_lib-0.8/eenhoorntje_llm_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 03:03:45.000000 eenhoorntje_llm_lib-0.8/eenhoorntje_llm_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-04-22 03:03:45.000000 eenhoorntje_llm_lib-0.8/eenhoorntje_llm_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-22 03:03:45.000000 eenhoorntje_llm_lib-0.8/eenhoorntje_llm_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-22 03:03:45.979712 eenhoorntje_llm_lib-0.8/setup.cfg
--rw-rw-rw-   0        0        0      523 2024-04-22 03:03:43.000000 eenhoorntje_llm_lib-0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 03:33:36.568414 eenhoorntje_llm_lib-0.9/
+-rw-rw-rw-   0        0        0      284 2024-04-22 03:33:36.567418 eenhoorntje_llm_lib-0.9/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-20 02:23:05.000000 eenhoorntje_llm_lib-0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-22 03:33:36.556447 eenhoorntje_llm_lib-0.9/eenhoorntje_llm_lib/
+-rw-rw-rw-   0        0        0        0 2024-04-18 09:27:19.000000 eenhoorntje_llm_lib-0.9/eenhoorntje_llm_lib/__init__.py
+-rw-rw-rw-   0        0        0     1634 2024-04-20 01:20:42.000000 eenhoorntje_llm_lib-0.9/eenhoorntje_llm_lib/deepl.py
+-rw-rw-rw-   0        0        0     2437 2024-04-20 01:57:53.000000 eenhoorntje_llm_lib-0.9/eenhoorntje_llm_lib/gemini.py
+-rw-rw-rw-   0        0        0    11811 2024-04-20 02:11:12.000000 eenhoorntje_llm_lib-0.9/eenhoorntje_llm_lib/language_codes.py
+-rw-rw-rw-   0        0        0     1457 2024-04-22 02:59:55.000000 eenhoorntje_llm_lib-0.9/eenhoorntje_llm_lib/llm.py
+-rw-rw-rw-   0        0        0     1988 2024-04-18 09:36:38.000000 eenhoorntje_llm_lib-0.9/eenhoorntje_llm_lib/llm_cache.py
+-rw-rw-rw-   0        0        0      882 2024-04-20 02:21:34.000000 eenhoorntje_llm_lib-0.9/eenhoorntje_llm_lib/translate.py
+-rw-rw-rw-   0        0        0     1558 2024-04-20 02:21:34.000000 eenhoorntje_llm_lib-0.9/eenhoorntje_llm_lib/translate_llm.py
+-rw-rw-rw-   0        0        0      937 2024-04-22 03:33:08.000000 eenhoorntje_llm_lib-0.9/eenhoorntje_llm_lib/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-22 03:33:36.567418 eenhoorntje_llm_lib-0.9/eenhoorntje_llm_lib.egg-info/
+-rw-rw-rw-   0        0        0      284 2024-04-22 03:33:36.000000 eenhoorntje_llm_lib-0.9/eenhoorntje_llm_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2024-04-22 03:33:36.000000 eenhoorntje_llm_lib-0.9/eenhoorntje_llm_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 03:33:36.000000 eenhoorntje_llm_lib-0.9/eenhoorntje_llm_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-04-22 03:33:36.000000 eenhoorntje_llm_lib-0.9/eenhoorntje_llm_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-22 03:33:36.000000 eenhoorntje_llm_lib-0.9/eenhoorntje_llm_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-22 03:33:36.569412 eenhoorntje_llm_lib-0.9/setup.cfg
+-rw-rw-rw-   0        0        0      523 2024-04-22 03:33:08.000000 eenhoorntje_llm_lib-0.9/setup.py
```

### Comparing `eenhoorntje_llm_lib-0.8/eenhoorntje_llm_lib/deepl.py` & `eenhoorntje_llm_lib-0.9/eenhoorntje_llm_lib/deepl.py`

 * *Files identical despite different names*

### Comparing `eenhoorntje_llm_lib-0.8/eenhoorntje_llm_lib/gemini.py` & `eenhoorntje_llm_lib-0.9/eenhoorntje_llm_lib/gemini.py`

 * *Files identical despite different names*

### Comparing `eenhoorntje_llm_lib-0.8/eenhoorntje_llm_lib/language_codes.py` & `eenhoorntje_llm_lib-0.9/eenhoorntje_llm_lib/language_codes.py`

 * *Files identical despite different names*

### Comparing `eenhoorntje_llm_lib-0.8/eenhoorntje_llm_lib/llm.py` & `eenhoorntje_llm_lib-0.9/eenhoorntje_llm_lib/llm.py`

 * *Files identical despite different names*

### Comparing `eenhoorntje_llm_lib-0.8/eenhoorntje_llm_lib/llm_cache.py` & `eenhoorntje_llm_lib-0.9/eenhoorntje_llm_lib/llm_cache.py`

 * *Files identical despite different names*

### Comparing `eenhoorntje_llm_lib-0.8/eenhoorntje_llm_lib/translate.py` & `eenhoorntje_llm_lib-0.9/eenhoorntje_llm_lib/translate.py`

 * *Files identical despite different names*

### Comparing `eenhoorntje_llm_lib-0.8/eenhoorntje_llm_lib/translate_llm.py` & `eenhoorntje_llm_lib-0.9/eenhoorntje_llm_lib/translate_llm.py`

 * *Files identical despite different names*

### Comparing `eenhoorntje_llm_lib-0.8/eenhoorntje_llm_lib/utils.py` & `eenhoorntje_llm_lib-0.9/eenhoorntje_llm_lib/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 default_content = """{
     "OPEN_AI_API_KEY": "<YOUR OPEN_AI API KEY>",
     "OPEN_ROUTER_API_KEY": "<YOUR OPEN_ROUTER API KEY>",
     "DEEPL_API_KEY": "<YOUR DEEPL API KEY>",
     "GOOGLE_API_KEY": "<YOUR GOOGLE API KEY>",
-    "GEMINI_API_KEY": "<YOUR GEMINI API KEY>",
+    "GEMINI_API_KEY": "<YOUR GEMINI API KEY>"
 }
 """
 
 
 def get_key(key_name):
     file_name = "keys.json"
     if os.path.exists(file_name):
```

### Comparing `eenhoorntje_llm_lib-0.8/eenhoorntje_llm_lib.egg-info/SOURCES.txt` & `eenhoorntje_llm_lib-0.9/eenhoorntje_llm_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eenhoorntje_llm_lib-0.8/setup.py` & `eenhoorntje_llm_lib-0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='eenhoorntje_llm_lib',
-    version='0.8',
+    version='0.9',
     description='A lib for cached LLM calling and translation',
     author='Dmitrii Lukianov',
     author_email='unicornporated@gmil.com',
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["openai", "google-generativeai"],
```

