# Comparing `tmp/pygramcore-1.0.1.tar.gz` & `tmp/pygramcore-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygramcore-1.0.1.tar", last modified: Thu May  9 18:28:23 2024, max compression
+gzip compressed data, was "pygramcore-1.0.2.tar", last modified: Thu May  9 18:34:55 2024, max compression
```

## Comparing `pygramcore-1.0.1.tar` & `pygramcore-1.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 18:28:23.547564 pygramcore-1.0.1/
--rw-rw-rw-   0        0        0     1089 2024-05-05 17:27:36.000000 pygramcore-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     3888 2024-05-09 18:28:23.546564 pygramcore-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3172 2024-05-09 18:21:40.000000 pygramcore-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 18:28:23.515995 pygramcore-1.0.1/pygramcore/
--rw-rw-rw-   0        0        0       54 2024-05-09 13:07:12.000000 pygramcore-1.0.1/pygramcore/__init__.py
--rw-rw-rw-   0        0        0      266 2024-05-09 13:07:12.000000 pygramcore-1.0.1/pygramcore/constants.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:28:23.538066 pygramcore-1.0.1/pygramcore/elements/
--rw-rw-rw-   0        0        0       48 2024-05-09 13:07:12.000000 pygramcore-1.0.1/pygramcore/elements/__init__.py
--rw-rw-rw-   0        0        0     9663 2024-05-09 16:17:22.000000 pygramcore-1.0.1/pygramcore/elements/post.py
--rw-rw-rw-   0        0        0    14390 2024-05-09 16:20:10.000000 pygramcore-1.0.1/pygramcore/elements/user.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:28:23.543065 pygramcore-1.0.1/pygramcore/exceptions/
--rw-rw-rw-   0        0        0        0 2024-05-09 12:49:58.000000 pygramcore-1.0.1/pygramcore/exceptions/__init__.py
--rw-rw-rw-   0        0        0      148 2024-05-09 17:13:14.000000 pygramcore-1.0.1/pygramcore/exceptions/auth.py
--rw-rw-rw-   0        0        0      238 2024-05-09 17:07:39.000000 pygramcore-1.0.1/pygramcore/exceptions/format.py
--rw-rw-rw-   0        0        0      494 2024-05-09 13:07:12.000000 pygramcore-1.0.1/pygramcore/exceptions/post.py
--rw-rw-rw-   0        0        0      638 2024-05-09 13:07:12.000000 pygramcore-1.0.1/pygramcore/exceptions/user.py
--rw-rw-rw-   0        0        0     8945 2024-05-09 17:16:12.000000 pygramcore-1.0.1/pygramcore/pygram.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:28:23.545064 pygramcore-1.0.1/pygramcore/utils/
--rw-rw-rw-   0        0        0       21 2024-05-09 13:07:12.000000 pygramcore-1.0.1/pygramcore/utils/__init__.py
--rw-rw-rw-   0        0        0      977 2024-05-09 13:07:12.000000 pygramcore-1.0.1/pygramcore/utils/misc.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:28:23.546064 pygramcore-1.0.1/pygramcore.egg-info/
--rw-rw-rw-   0        0        0     3888 2024-05-09 18:28:23.000000 pygramcore-1.0.1/pygramcore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      561 2024-05-09 18:28:23.000000 pygramcore-1.0.1/pygramcore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 18:28:23.000000 pygramcore-1.0.1/pygramcore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-05-09 18:28:23.000000 pygramcore-1.0.1/pygramcore.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-09 18:28:23.000000 pygramcore-1.0.1/pygramcore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 18:28:23.548064 pygramcore-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1174 2024-05-09 18:27:01.000000 pygramcore-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:34:55.028375 pygramcore-1.0.2/
+-rw-rw-rw-   0        0        0     1089 2024-05-05 17:27:36.000000 pygramcore-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3865 2024-05-09 18:34:55.027377 pygramcore-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3149 2024-05-09 18:34:13.000000 pygramcore-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 18:34:54.999376 pygramcore-1.0.2/pygramcore/
+-rw-rw-rw-   0        0        0       54 2024-05-09 13:07:12.000000 pygramcore-1.0.2/pygramcore/__init__.py
+-rw-rw-rw-   0        0        0      266 2024-05-09 13:07:12.000000 pygramcore-1.0.2/pygramcore/constants.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:34:55.017877 pygramcore-1.0.2/pygramcore/elements/
+-rw-rw-rw-   0        0        0       48 2024-05-09 13:07:12.000000 pygramcore-1.0.2/pygramcore/elements/__init__.py
+-rw-rw-rw-   0        0        0     9663 2024-05-09 16:17:22.000000 pygramcore-1.0.2/pygramcore/elements/post.py
+-rw-rw-rw-   0        0        0    14390 2024-05-09 16:20:10.000000 pygramcore-1.0.2/pygramcore/elements/user.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:34:55.023376 pygramcore-1.0.2/pygramcore/exceptions/
+-rw-rw-rw-   0        0        0        0 2024-05-09 12:49:58.000000 pygramcore-1.0.2/pygramcore/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      148 2024-05-09 17:13:14.000000 pygramcore-1.0.2/pygramcore/exceptions/auth.py
+-rw-rw-rw-   0        0        0      238 2024-05-09 17:07:39.000000 pygramcore-1.0.2/pygramcore/exceptions/format.py
+-rw-rw-rw-   0        0        0      494 2024-05-09 13:07:12.000000 pygramcore-1.0.2/pygramcore/exceptions/post.py
+-rw-rw-rw-   0        0        0      638 2024-05-09 13:07:12.000000 pygramcore-1.0.2/pygramcore/exceptions/user.py
+-rw-rw-rw-   0        0        0     8945 2024-05-09 17:16:12.000000 pygramcore-1.0.2/pygramcore/pygram.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:34:55.025378 pygramcore-1.0.2/pygramcore/utils/
+-rw-rw-rw-   0        0        0       21 2024-05-09 13:07:12.000000 pygramcore-1.0.2/pygramcore/utils/__init__.py
+-rw-rw-rw-   0        0        0      977 2024-05-09 13:07:12.000000 pygramcore-1.0.2/pygramcore/utils/misc.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:34:55.026377 pygramcore-1.0.2/pygramcore.egg-info/
+-rw-rw-rw-   0        0        0     3865 2024-05-09 18:34:54.000000 pygramcore-1.0.2/pygramcore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      561 2024-05-09 18:34:54.000000 pygramcore-1.0.2/pygramcore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 18:34:54.000000 pygramcore-1.0.2/pygramcore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-05-09 18:34:54.000000 pygramcore-1.0.2/pygramcore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-09 18:34:54.000000 pygramcore-1.0.2/pygramcore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 18:34:55.028375 pygramcore-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1174 2024-05-09 18:34:44.000000 pygramcore-1.0.2/setup.py
```

### Comparing `pygramcore-1.0.1/LICENSE` & `pygramcore-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pygramcore-1.0.1/PKG-INFO` & `pygramcore-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygramcore
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simple-to-use Instagram Python interface using Selenium.
 Author: Joel Taylor
 Author-email: contact@joeltaylor.business
 License: MIT
 Keywords: instagram,instagram bot,selenium,automation,bot
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -13,15 +13,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: selenium
 Requires-Dist: selenium-stealth
 
 <h1 align="center">
   <br>
-  <img src="https://github.com/jtayped/pygramcore/blob/40436d7b57e247742b1697a88e52f06821e2f9f8/images/icon.png" alt="PyGramCore" width="200">
+  <img src="https://github.com/jtayped/pygramcore/blob/main/images/icon.png?raw=true" alt="PyGramCore" width="200">
   <br>
   📷 pygramcore
   <br>
 </h1>
 
 <h4 align="center">An easy-to-use Instagram SDK using <a href="https://www.selenium.dev/" target="_blank">Selenium</a>.</h4>
 
@@ -36,19 +36,19 @@
     <img src="https://img.shields.io/github/issues/jtayped/pygramcore?style=for-the-badge" alt="License">
   </a>
   <a href="https://www.linkedin.com/in/jtayped/">
     <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
   </a>
 </div>
 
-<p align="center">
+<div align="center">
   <a href="#key-features">Key Features</a> •
   <a href="#how-to-use">How To Use</a> •
   <a href="#related">Related</a>
-</p>
+</div>
 
 <div id="key-features"></div>
 
 ## 🔑 Key Features
 
 - **Modular Elements**: Easily use and customize modular elements such as Posts, Comments, and Users.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pygramcore Version: 1.0.1 Summary: A simple-to-use
+Metadata-Version: 2.1 Name: pygramcore Version: 1.0.2 Summary: A simple-to-use
 Instagram Python interface using Selenium. Author: Joel Taylor Author-email:
 contact@joeltaylor.business License: MIT Keywords: instagram,instagram
 bot,selenium,automation,bot Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3.12 Classifier: Programming Language :: Python :: Implementation ::
 CPython Description-Content-Type: text/markdown License-File: LICENSE Requires-
 Dist: selenium Requires-Dist: selenium-stealth
```

### Comparing `pygramcore-1.0.1/README.md` & `pygramcore-1.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <h1 align="center">
   <br>
-  <img src="https://github.com/jtayped/pygramcore/blob/40436d7b57e247742b1697a88e52f06821e2f9f8/images/icon.png" alt="PyGramCore" width="200">
+  <img src="https://github.com/jtayped/pygramcore/blob/main/images/icon.png?raw=true" alt="PyGramCore" width="200">
   <br>
   📷 pygramcore
   <br>
 </h1>
 
 <h4 align="center">An easy-to-use Instagram SDK using <a href="https://www.selenium.dev/" target="_blank">Selenium</a>.</h4>
 
@@ -19,19 +19,19 @@
     <img src="https://img.shields.io/github/issues/jtayped/pygramcore?style=for-the-badge" alt="License">
   </a>
   <a href="https://www.linkedin.com/in/jtayped/">
     <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
   </a>
 </div>
 
-<p align="center">
+<div align="center">
   <a href="#key-features">Key Features</a> •
   <a href="#how-to-use">How To Use</a> •
   <a href="#related">Related</a>
-</p>
+</div>
 
 <div id="key-features"></div>
 
 ## 🔑 Key Features
 
 - **Modular Elements**: Easily use and customize modular elements such as Posts, Comments, and Users.
```

### Comparing `pygramcore-1.0.1/pygramcore/elements/post.py` & `pygramcore-1.0.2/pygramcore/elements/post.py`

 * *Files identical despite different names*

### Comparing `pygramcore-1.0.1/pygramcore/elements/user.py` & `pygramcore-1.0.2/pygramcore/elements/user.py`

 * *Files identical despite different names*

### Comparing `pygramcore-1.0.1/pygramcore/exceptions/user.py` & `pygramcore-1.0.2/pygramcore/exceptions/user.py`

 * *Files identical despite different names*

### Comparing `pygramcore-1.0.1/pygramcore/pygram.py` & `pygramcore-1.0.2/pygramcore/pygram.py`

 * *Files identical despite different names*

### Comparing `pygramcore-1.0.1/pygramcore/utils/misc.py` & `pygramcore-1.0.2/pygramcore/utils/misc.py`

 * *Files identical despite different names*

### Comparing `pygramcore-1.0.1/pygramcore.egg-info/PKG-INFO` & `pygramcore-1.0.2/pygramcore.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygramcore
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simple-to-use Instagram Python interface using Selenium.
 Author: Joel Taylor
 Author-email: contact@joeltaylor.business
 License: MIT
 Keywords: instagram,instagram bot,selenium,automation,bot
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -13,15 +13,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: selenium
 Requires-Dist: selenium-stealth
 
 <h1 align="center">
   <br>
-  <img src="https://github.com/jtayped/pygramcore/blob/40436d7b57e247742b1697a88e52f06821e2f9f8/images/icon.png" alt="PyGramCore" width="200">
+  <img src="https://github.com/jtayped/pygramcore/blob/main/images/icon.png?raw=true" alt="PyGramCore" width="200">
   <br>
   📷 pygramcore
   <br>
 </h1>
 
 <h4 align="center">An easy-to-use Instagram SDK using <a href="https://www.selenium.dev/" target="_blank">Selenium</a>.</h4>
 
@@ -36,19 +36,19 @@
     <img src="https://img.shields.io/github/issues/jtayped/pygramcore?style=for-the-badge" alt="License">
   </a>
   <a href="https://www.linkedin.com/in/jtayped/">
     <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
   </a>
 </div>
 
-<p align="center">
+<div align="center">
   <a href="#key-features">Key Features</a> •
   <a href="#how-to-use">How To Use</a> •
   <a href="#related">Related</a>
-</p>
+</div>
 
 <div id="key-features"></div>
 
 ## 🔑 Key Features
 
 - **Modular Elements**: Easily use and customize modular elements such as Posts, Comments, and Users.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pygramcore Version: 1.0.1 Summary: A simple-to-use
+Metadata-Version: 2.1 Name: pygramcore Version: 1.0.2 Summary: A simple-to-use
 Instagram Python interface using Selenium. Author: Joel Taylor Author-email:
 contact@joeltaylor.business License: MIT Keywords: instagram,instagram
 bot,selenium,automation,bot Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3.12 Classifier: Programming Language :: Python :: Implementation ::
 CPython Description-Content-Type: text/markdown License-File: LICENSE Requires-
 Dist: selenium Requires-Dist: selenium-stealth
```

### Comparing `pygramcore-1.0.1/pygramcore.egg-info/SOURCES.txt` & `pygramcore-1.0.2/pygramcore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygramcore-1.0.1/setup.py` & `pygramcore-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from codecs import open
 from os import path
 
 # Read version from VERSION file
 here = path.abspath(path.dirname(__file__))
 
-VERSION = "1.0.1"
+VERSION = "1.0.2"
 DESCRIPTION = "A simple-to-use Instagram Python interface using Selenium."
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
```

