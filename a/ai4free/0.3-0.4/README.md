# Comparing `tmp/ai4free-0.3.tar.gz` & `tmp/ai4free-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai4free-0.3.tar", last modified: Thu May  9 14:56:36 2024, max compression
+gzip compressed data, was "ai4free-0.4.tar", last modified: Thu May  9 16:26:15 2024, max compression
```

## Comparing `ai4free-0.3.tar` & `ai4free-0.4.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 14:56:36.677263 ai4free-0.3/
--rw-rw-rw-   0        0        0     3186 2024-05-09 14:51:32.000000 ai4free-0.3/LICENSE.md
--rw-rw-rw-   0        0        0    10604 2024-05-09 14:56:36.669559 ai4free-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     9321 2024-05-09 10:57:47.000000 ai4free-0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 14:56:36.590855 ai4free-0.3/ai4free/
--rw-rw-rw-   0        0        0    16349 2024-05-09 10:57:47.000000 ai4free-0.3/ai4free/Blackbox.py
--rw-rw-rw-   0        0        0     8277 2024-05-09 10:57:47.000000 ai4free-0.3/ai4free/Cohere.py
--rw-rw-rw-   0        0        0    15388 2024-05-09 10:57:47.000000 ai4free-0.3/ai4free/KOBOLDAI.py
--rw-rw-rw-   0        0        0    18500 2024-05-09 10:57:47.000000 ai4free-0.3/ai4free/OpenGPT.py
--rw-rw-rw-   0        0        0    20211 2024-05-09 10:57:47.000000 ai4free-0.3/ai4free/Openai.py
--rw-rw-rw-   0        0        0    19512 2024-05-09 10:57:47.000000 ai4free-0.3/ai4free/Phind.py
--rw-rw-rw-   0        0        0      319 2024-05-09 10:57:47.000000 ai4free-0.3/ai4free/__init__.py
--rw-rw-rw-   0        0        0    20824 2024-05-09 10:57:47.000000 ai4free-0.3/ai4free/groq.py
--rw-rw-rw-   0        0        0    20051 2024-05-09 10:57:47.000000 ai4free-0.3/ai4free/leo.py
--rw-rw-rw-   0        0        0     8482 2024-05-09 10:57:47.000000 ai4free-0.3/ai4free/reka.py
--rw-rw-rw-   0        0        0    19935 2024-05-09 10:57:47.000000 ai4free-0.3/ai4free/yep.py
--rw-rw-rw-   0        0        0     7580 2024-05-09 10:57:47.000000 ai4free-0.3/ai4free/you.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:56:36.664510 ai4free-0.3/ai4free.egg-info/
--rw-rw-rw-   0        0        0    10604 2024-05-09 14:56:35.000000 ai4free-0.3/ai4free.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      392 2024-05-09 14:56:36.000000 ai4free-0.3/ai4free.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 14:56:35.000000 ai4free-0.3/ai4free.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-05-09 14:56:35.000000 ai4free-0.3/ai4free.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-09 14:56:35.000000 ai4free-0.3/ai4free.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 14:56:36.685293 ai4free-0.3/setup.cfg
--rw-rw-rw-   0        0        0     1607 2024-05-09 14:56:07.000000 ai4free-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 16:26:15.834266 ai4free-0.4/
+-rw-rw-rw-   0        0        0     3186 2024-05-09 14:51:32.000000 ai4free-0.4/LICENSE.md
+-rw-rw-rw-   0        0        0    10604 2024-05-09 16:26:15.824694 ai4free-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     9321 2024-05-09 10:57:47.000000 ai4free-0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 16:26:15.745703 ai4free-0.4/ai4free/
+-rw-rw-rw-   0        0        0    16349 2024-05-09 10:57:47.000000 ai4free-0.4/ai4free/Blackbox.py
+-rw-rw-rw-   0        0        0     8277 2024-05-09 10:57:47.000000 ai4free-0.4/ai4free/Cohere.py
+-rw-rw-rw-   0        0        0    15388 2024-05-09 10:57:47.000000 ai4free-0.4/ai4free/KOBOLDAI.py
+-rw-rw-rw-   0        0        0    18500 2024-05-09 10:57:47.000000 ai4free-0.4/ai4free/OpenGPT.py
+-rw-rw-rw-   0        0        0    20211 2024-05-09 10:57:47.000000 ai4free-0.4/ai4free/Openai.py
+-rw-rw-rw-   0        0        0    19512 2024-05-09 10:57:47.000000 ai4free-0.4/ai4free/Phind.py
+-rw-rw-rw-   0        0        0      353 2024-05-09 16:19:10.000000 ai4free-0.4/ai4free/__init__.py
+-rw-rw-rw-   0        0        0    20824 2024-05-09 10:57:47.000000 ai4free-0.4/ai4free/groq.py
+-rw-rw-rw-   0        0        0    20051 2024-05-09 10:57:47.000000 ai4free-0.4/ai4free/leo.py
+-rw-rw-rw-   0        0        0     8397 2024-05-09 16:18:46.000000 ai4free-0.4/ai4free/perplexity.py
+-rw-rw-rw-   0        0        0     8482 2024-05-09 10:57:47.000000 ai4free-0.4/ai4free/reka.py
+-rw-rw-rw-   0        0        0    19935 2024-05-09 10:57:47.000000 ai4free-0.4/ai4free/yep.py
+-rw-rw-rw-   0        0        0     7580 2024-05-09 10:57:47.000000 ai4free-0.4/ai4free/you.py
+drwxrwxrwx   0        0        0        0 2024-05-09 16:26:15.813700 ai4free-0.4/ai4free.egg-info/
+-rw-rw-rw-   0        0        0    10604 2024-05-09 16:26:13.000000 ai4free-0.4/ai4free.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      414 2024-05-09 16:26:15.000000 ai4free-0.4/ai4free.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 16:26:13.000000 ai4free-0.4/ai4free.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-05-09 16:26:13.000000 ai4free-0.4/ai4free.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-09 16:26:13.000000 ai4free-0.4/ai4free.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 16:26:15.835275 ai4free-0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1607 2024-05-09 16:11:55.000000 ai4free-0.4/setup.py
```

### Comparing `ai4free-0.3/LICENSE.md` & `ai4free-0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ai4free-0.3/PKG-INFO` & `ai4free-0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai4free
-Version: 0.3
+Version: 0.4
 Summary: collection of free AI provides
 Author: OEvortex, Sree
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Source, https://github.com/Devs-Do-Code/ai4free
 Project-URL: Tracker, https://github.com/Devs-Do-Code/ai4free/issues
 Project-URL: YouTube, https://youtube.com/@OEvortex
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ai4free Version: 0.3 Summary: collection of free AI
+Metadata-Version: 2.1 Name: ai4free Version: 0.4 Summary: collection of free AI
 provides Author: OEvortex, Sree Author-email: helpingai5@gmail.com License:
 HelpingAI Simplified Universal License Project-URL: Source, https://github.com/
 Devs-Do-Code/ai4free Project-URL: Tracker, https://github.com/Devs-Do-Code/
 ai4free/issues Project-URL: YouTube, https://youtube.com/@OEvortex Project-URL:
 Youtube, https://www.youtube.com/@DevsDoCode Classifier: Development Status ::
 5 - Production/Stable Classifier: Intended Audience :: Developers Classifier:
 License :: Other/Proprietary License Classifier: Operating System :: OS
```

### Comparing `ai4free-0.3/README.md` & `ai4free-0.4/README.md`

 * *Files identical despite different names*

### Comparing `ai4free-0.3/ai4free/Blackbox.py` & `ai4free-0.4/ai4free/Blackbox.py`

 * *Files identical despite different names*

### Comparing `ai4free-0.3/ai4free/Cohere.py` & `ai4free-0.4/ai4free/Cohere.py`

 * *Files identical despite different names*

### Comparing `ai4free-0.3/ai4free/KOBOLDAI.py` & `ai4free-0.4/ai4free/KOBOLDAI.py`

 * *Files identical despite different names*

### Comparing `ai4free-0.3/ai4free/OpenGPT.py` & `ai4free-0.4/ai4free/OpenGPT.py`

 * *Files identical despite different names*

### Comparing `ai4free-0.3/ai4free/Openai.py` & `ai4free-0.4/ai4free/Openai.py`

 * *Files identical despite different names*

### Comparing `ai4free-0.3/ai4free/Phind.py` & `ai4free-0.4/ai4free/Phind.py`

 * *Files identical despite different names*

### Comparing `ai4free-0.3/ai4free/groq.py` & `ai4free-0.4/ai4free/groq.py`

 * *Files identical despite different names*

### Comparing `ai4free-0.3/ai4free/leo.py` & `ai4free-0.4/ai4free/leo.py`

 * *Files identical despite different names*

### Comparing `ai4free-0.3/ai4free/reka.py` & `ai4free-0.4/ai4free/reka.py`

 * *Files identical despite different names*

### Comparing `ai4free-0.3/ai4free/yep.py` & `ai4free-0.4/ai4free/yep.py`

 * *Files identical despite different names*

### Comparing `ai4free-0.3/ai4free/you.py` & `ai4free-0.4/ai4free/you.py`

 * *Files identical despite different names*

### Comparing `ai4free-0.3/ai4free.egg-info/PKG-INFO` & `ai4free-0.4/ai4free.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai4free
-Version: 0.3
+Version: 0.4
 Summary: collection of free AI provides
 Author: OEvortex, Sree
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Source, https://github.com/Devs-Do-Code/ai4free
 Project-URL: Tracker, https://github.com/Devs-Do-Code/ai4free/issues
 Project-URL: YouTube, https://youtube.com/@OEvortex
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ai4free Version: 0.3 Summary: collection of free AI
+Metadata-Version: 2.1 Name: ai4free Version: 0.4 Summary: collection of free AI
 provides Author: OEvortex, Sree Author-email: helpingai5@gmail.com License:
 HelpingAI Simplified Universal License Project-URL: Source, https://github.com/
 Devs-Do-Code/ai4free Project-URL: Tracker, https://github.com/Devs-Do-Code/
 ai4free/issues Project-URL: YouTube, https://youtube.com/@OEvortex Project-URL:
 Youtube, https://www.youtube.com/@DevsDoCode Classifier: Development Status ::
 5 - Production/Stable Classifier: Intended Audience :: Developers Classifier:
 License :: Other/Proprietary License Classifier: Operating System :: OS
```

### Comparing `ai4free-0.3/setup.py` & `ai4free-0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="ai4free",
-    version="0.3", 
+    version="0.4", 
     description="collection of free AI provides",
     long_description=README,
     long_description_content_type="text/markdown",
     author="OEvortex, Sree",  # List both authors here
     author_email="helpingai5@gmail.com",  # Specify the email for the first author
     packages=find_packages(),
     classifiers=[
```

