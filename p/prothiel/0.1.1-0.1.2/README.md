# Comparing `tmp/prothiel-0.1.1.tar.gz` & `tmp/prothiel-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prothiel-0.1.1.tar", last modified: Fri May 10 11:03:44 2024, max compression
+gzip compressed data, was "prothiel-0.1.2.tar", last modified: Fri May 10 11:07:47 2024, max compression
```

## Comparing `prothiel-0.1.1.tar` & `prothiel-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:03:44.182370 prothiel-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-10 11:03:39.000000 prothiel-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-05-10 11:03:44.178370 prothiel-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-05-10 11:03:39.000000 prothiel-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:03:44.178370 prothiel-0.1.1/prothiel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-05-10 11:03:44.000000 prothiel-0.1.1/prothiel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-10 11:03:44.000000 prothiel-0.1.1/prothiel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 11:03:44.000000 prothiel-0.1.1/prothiel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-10 11:03:44.000000 prothiel-0.1.1/prothiel.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-10 11:03:44.000000 prothiel-0.1.1/prothiel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 11:03:44.000000 prothiel-0.1.1/prothiel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 11:03:44.182370 prothiel-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-10 11:03:39.000000 prothiel-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:03:44.178370 prothiel-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-10 11:03:39.000000 prothiel-0.1.1/tests/test_extract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:07:47.485598 prothiel-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-10 11:07:43.000000 prothiel-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-05-10 11:07:47.485598 prothiel-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-05-10 11:07:43.000000 prothiel-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:07:47.485598 prothiel-0.1.2/prothiel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-05-10 11:07:47.000000 prothiel-0.1.2/prothiel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-10 11:07:47.000000 prothiel-0.1.2/prothiel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 11:07:47.000000 prothiel-0.1.2/prothiel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-10 11:07:47.000000 prothiel-0.1.2/prothiel.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-10 11:07:47.000000 prothiel-0.1.2/prothiel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 11:07:47.000000 prothiel-0.1.2/prothiel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 11:07:47.485598 prothiel-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-10 11:07:43.000000 prothiel-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:07:47.485598 prothiel-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-10 11:07:43.000000 prothiel-0.1.2/tests/test_extract.py
```

### Comparing `prothiel-0.1.1/LICENSE` & `prothiel-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prothiel-0.1.1/PKG-INFO` & `prothiel-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: prothiel
-Version: 0.1.1
+Version: 0.1.2
 Home-page: https://github.com/Sunwood-ai-labs/Prothiel
 Author: Maki
 Author-email: sunwood.ai.labs@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: termcolor
 Requires-Dist: art
 
 
 <p align="center">
-<img src="docs/Prothiel_icon.png" width="100%">
+<img src="https://raw.githubusercontent.com/Sunwood-ai-labs/Prothiel/main/docs/Prothiel_icon.png" width="100%">
 <br>
 <h1 align="center">Prothiel</h1>
 <h2 align="center">
   ～AI Harmony, Infinite Possibilities～
 
 [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/MakiAi/Prothiel)
 [![Prothiel - Sunwood-ai-labs](https://img.shields.io/static/v1?label=Prothiel&message=Sunwood-ai-labs&color=blue&logo=github)](https://github.com/Sunwood-ai-labs/Prothiel "Go to GitHub repo")
```

### Comparing `prothiel-0.1.1/README.md` & `prothiel-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 <p align="center">
-<img src="docs/Prothiel_icon.png" width="100%">
+<img src="https://raw.githubusercontent.com/Sunwood-ai-labs/Prothiel/main/docs/Prothiel_icon.png" width="100%">
 <br>
 <h1 align="center">Prothiel</h1>
 <h2 align="center">
   ～AI Harmony, Infinite Possibilities～
 
 [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/MakiAi/Prothiel)
 [![Prothiel - Sunwood-ai-labs](https://img.shields.io/static/v1?label=Prothiel&message=Sunwood-ai-labs&color=blue&logo=github)](https://github.com/Sunwood-ai-labs/Prothiel "Go to GitHub repo")
```

### Comparing `prothiel-0.1.1/prothiel.egg-info/PKG-INFO` & `prothiel-0.1.2/prothiel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: prothiel
-Version: 0.1.1
+Version: 0.1.2
 Home-page: https://github.com/Sunwood-ai-labs/Prothiel
 Author: Maki
 Author-email: sunwood.ai.labs@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: termcolor
 Requires-Dist: art
 
 
 <p align="center">
-<img src="docs/Prothiel_icon.png" width="100%">
+<img src="https://raw.githubusercontent.com/Sunwood-ai-labs/Prothiel/main/docs/Prothiel_icon.png" width="100%">
 <br>
 <h1 align="center">Prothiel</h1>
 <h2 align="center">
   ～AI Harmony, Infinite Possibilities～
 
 [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/MakiAi/Prothiel)
 [![Prothiel - Sunwood-ai-labs](https://img.shields.io/static/v1?label=Prothiel&message=Sunwood-ai-labs&color=blue&logo=github)](https://github.com/Sunwood-ai-labs/Prothiel "Go to GitHub repo")
```

### Comparing `prothiel-0.1.1/setup.py` & `prothiel-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # READMEファイルの内容を読み込む
 with open("README.md", "r", encoding="utf-8") as fh:
    long_description = fh.read()
 
 setup(
     name='prothiel',
-    version='0.1.1',
+    version='0.1.2',
     # PyPIに表示される長い説明文
     long_description=long_description,
     # 長い説明文のフォーマット
     long_description_content_type="text/markdown",
     # プロジェクトのURL
     url="https://github.com/Sunwood-ai-labs/Prothiel",
     author='Maki',
```

### Comparing `prothiel-0.1.1/tests/test_extract.py` & `prothiel-0.1.2/tests/test_extract.py`

 * *Files identical despite different names*

