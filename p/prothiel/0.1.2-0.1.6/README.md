# Comparing `tmp/prothiel-0.1.2.tar.gz` & `tmp/prothiel-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prothiel-0.1.2.tar", last modified: Fri May 10 11:07:47 2024, max compression
+gzip compressed data, was "prothiel-0.1.6.tar", last modified: Fri May 10 13:45:59 2024, max compression
```

## Comparing `prothiel-0.1.2.tar` & `prothiel-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:07:47.485598 prothiel-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-10 11:07:43.000000 prothiel-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-05-10 11:07:47.485598 prothiel-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-05-10 11:07:43.000000 prothiel-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:07:47.485598 prothiel-0.1.2/prothiel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-05-10 11:07:47.000000 prothiel-0.1.2/prothiel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-10 11:07:47.000000 prothiel-0.1.2/prothiel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 11:07:47.000000 prothiel-0.1.2/prothiel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-10 11:07:47.000000 prothiel-0.1.2/prothiel.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-10 11:07:47.000000 prothiel-0.1.2/prothiel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 11:07:47.000000 prothiel-0.1.2/prothiel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 11:07:47.485598 prothiel-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-10 11:07:43.000000 prothiel-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:07:47.485598 prothiel-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-10 11:07:43.000000 prothiel-0.1.2/tests/test_extract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:45:59.166335 prothiel-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-10 13:45:53.000000 prothiel-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6208 2024-05-10 13:45:59.166335 prothiel-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-05-10 13:45:53.000000 prothiel-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:45:59.166335 prothiel-0.1.6/prothiel/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-10 13:45:53.000000 prothiel-0.1.6/prothiel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-10 13:45:53.000000 prothiel-0.1.6/prothiel/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-10 13:45:53.000000 prothiel-0.1.6/prothiel/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-10 13:45:53.000000 prothiel-0.1.6/prothiel/run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-10 13:45:53.000000 prothiel-0.1.6/prothiel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:45:59.166335 prothiel-0.1.6/prothiel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6208 2024-05-10 13:45:59.000000 prothiel-0.1.6/prothiel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-10 13:45:59.000000 prothiel-0.1.6/prothiel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 13:45:59.000000 prothiel-0.1.6/prothiel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-10 13:45:59.000000 prothiel-0.1.6/prothiel.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-10 13:45:59.000000 prothiel-0.1.6/prothiel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-10 13:45:59.000000 prothiel-0.1.6/prothiel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-10 13:45:53.000000 prothiel-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 13:45:59.166335 prothiel-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-10 13:45:53.000000 prothiel-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:45:59.166335 prothiel-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-10 13:45:53.000000 prothiel-0.1.6/tests/test_extract.py
```

### Comparing `prothiel-0.1.2/LICENSE` & `prothiel-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `prothiel-0.1.2/PKG-INFO` & `prothiel-0.1.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: prothiel
-Version: 0.1.2
-Home-page: https://github.com/Sunwood-ai-labs/Prothiel
-Author: Maki
-Author-email: sunwood.ai.labs@gmail.com
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: termcolor
-Requires-Dist: art
-
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/Sunwood-ai-labs/Prothiel/main/docs/Prothiel_icon.png" width="100%">
 <br>
 <h1 align="center">Prothiel</h1>
 <h2 align="center">
   ～AI Harmony, Infinite Possibilities～
@@ -131,15 +117,16 @@
         raise ValueError("0での除算は許可されていません。")
 ​```
 ```
 
 コードブロックを抽出してPythonファイルに整理するには、次のコマンドを実行します:
 
 ```
-prothiel example.md math_functions
+prothiel --markdown_file=example/01_math_functions.md --root_path=example/01_math_functions
+prothiel --markdown_file=example/02_Project_Example.md --root_path=example/02_Project_Example
 ```
 
 Prothielは次のファイル構造を作成します:
 
 ```
 math_functions/
 ├── basic_math/
@@ -164,8 +151,8 @@
 
 ## 🙏 謝辞
 
 オープンソースコミュニティの皆様の貴重な貢献と着想に感謝いたします。
 
 ---
 
-Prothielを使って、Markdownファイルからのコード抽出を楽々と始めましょう！🚀✨
+Prothielを使って、Markdownファイルからのコード抽出を楽々と始めましょう！🚀✨
```

### Comparing `prothiel-0.1.2/README.md` & `prothiel-0.1.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: prothiel
+Version: 0.1.6
+Home-page: https://github.com/Sunwood-ai-labs/Prothiel
+Author: Maki
+Author-email: sunwood.ai.labs@gmail.com
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Utilities
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: termcolor
+Requires-Dist: art
+
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/Sunwood-ai-labs/Prothiel/main/docs/Prothiel_icon.png" width="100%">
 <br>
 <h1 align="center">Prothiel</h1>
 <h2 align="center">
   ～AI Harmony, Infinite Possibilities～
@@ -117,15 +131,16 @@
         raise ValueError("0での除算は許可されていません。")
 ​```
 ```
 
 コードブロックを抽出してPythonファイルに整理するには、次のコマンドを実行します:
 
 ```
-prothiel example.md math_functions
+prothiel --markdown_file=example/01_math_functions.md --root_path=example/01_math_functions
+prothiel --markdown_file=example/02_Project_Example.md --root_path=example/02_Project_Example
 ```
 
 Prothielは次のファイル構造を作成します:
 
 ```
 math_functions/
 ├── basic_math/
@@ -150,8 +165,8 @@
 
 ## 🙏 謝辞
 
 オープンソースコミュニティの皆様の貴重な貢献と着想に感謝いたします。
 
 ---
 
-Prothielを使って、Markdownファイルからのコード抽出を楽々と始めましょう！🚀✨
+Prothielを使って、Markdownファイルからのコード抽出を楽々と始めましょう！🚀✨
```

### Comparing `prothiel-0.1.2/prothiel.egg-info/PKG-INFO` & `prothiel-0.1.6/prothiel.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prothiel
-Version: 0.1.2
+Version: 0.1.6
 Home-page: https://github.com/Sunwood-ai-labs/Prothiel
 Author: Maki
 Author-email: sunwood.ai.labs@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
@@ -131,15 +131,16 @@
         raise ValueError("0での除算は許可されていません。")
 ​```
 ```
 
 コードブロックを抽出してPythonファイルに整理するには、次のコマンドを実行します:
 
 ```
-prothiel example.md math_functions
+prothiel --markdown_file=example/01_math_functions.md --root_path=example/01_math_functions
+prothiel --markdown_file=example/02_Project_Example.md --root_path=example/02_Project_Example
 ```
 
 Prothielは次のファイル構造を作成します:
 
 ```
 math_functions/
 ├── basic_math/
```

### Comparing `prothiel-0.1.2/setup.py` & `prothiel-0.1.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from setuptools import setup, find_packages
 
+
 # READMEファイルの内容を読み込む
 with open("README.md", "r", encoding="utf-8") as fh:
    long_description = fh.read()
 
 setup(
     name='prothiel',
-    version='0.1.2',
+    version="0.1.6",
     # PyPIに表示される長い説明文
     long_description=long_description,
     # 長い説明文のフォーマット
     long_description_content_type="text/markdown",
     # プロジェクトのURL
     url="https://github.com/Sunwood-ai-labs/Prothiel",
     author='Maki',
```

### Comparing `prothiel-0.1.2/tests/test_extract.py` & `prothiel-0.1.6/tests/test_extract.py`

 * *Files identical despite different names*

