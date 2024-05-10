# Comparing `tmp/tiny_progress_bar-0.1.tar.gz` & `tmp/tiny_progress_bar-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiny_progress_bar-0.1.tar", last modified: Fri May 10 02:40:36 2024, max compression
+gzip compressed data, was "tiny_progress_bar-0.1.1.tar", last modified: Fri May 10 02:46:44 2024, max compression
```

## Comparing `tiny_progress_bar-0.1.tar` & `tiny_progress_bar-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 alan       (501) staff       (20)        0 2024-05-10 02:40:36.860665 tiny_progress_bar-0.1/
--rw-r--r--   0 alan       (501) staff       (20)    35149 2024-05-09 21:02:19.000000 tiny_progress_bar-0.1/LICENSE
--rw-r--r--   0 alan       (501) staff       (20)      697 2024-05-10 02:40:36.860712 tiny_progress_bar-0.1/PKG-INFO
--rw-r--r--   0 alan       (501) staff       (20)     1101 2024-05-10 02:37:19.000000 tiny_progress_bar-0.1/README.md
--rw-r--r--   0 alan       (501) staff       (20)       79 2024-05-10 02:40:36.860953 tiny_progress_bar-0.1/setup.cfg
--rw-r--r--   0 alan       (501) staff       (20)     1559 2024-05-10 02:40:15.000000 tiny_progress_bar-0.1/setup.py
-drwxr-xr-x   0 alan       (501) staff       (20)        0 2024-05-10 02:40:36.860014 tiny_progress_bar-0.1/tiny_progress_bar/
--rw-r--r--   0 alan       (501) staff       (20)     4266 2024-05-10 02:24:06.000000 tiny_progress_bar-0.1/tiny_progress_bar/test_tiny_progress_bar.py
--rw-r--r--   0 alan       (501) staff       (20)     2034 2024-05-10 02:23:26.000000 tiny_progress_bar-0.1/tiny_progress_bar/tiny_progress_bar.py
-drwxr-xr-x   0 alan       (501) staff       (20)        0 2024-05-10 02:40:36.860574 tiny_progress_bar-0.1/tiny_progress_bar.egg-info/
--rw-r--r--   0 alan       (501) staff       (20)      697 2024-05-10 02:40:36.000000 tiny_progress_bar-0.1/tiny_progress_bar.egg-info/PKG-INFO
--rw-r--r--   0 alan       (501) staff       (20)      283 2024-05-10 02:40:36.000000 tiny_progress_bar-0.1/tiny_progress_bar.egg-info/SOURCES.txt
--rw-r--r--   0 alan       (501) staff       (20)        1 2024-05-10 02:40:36.000000 tiny_progress_bar-0.1/tiny_progress_bar.egg-info/dependency_links.txt
--rw-r--r--   0 alan       (501) staff       (20)       18 2024-05-10 02:40:36.000000 tiny_progress_bar-0.1/tiny_progress_bar.egg-info/top_level.txt
+drwxr-xr-x   0 alan       (501) staff       (20)        0 2024-05-10 02:46:44.204315 tiny_progress_bar-0.1.1/
+-rw-r--r--   0 alan       (501) staff       (20)    35149 2024-05-09 21:02:19.000000 tiny_progress_bar-0.1.1/LICENSE
+-rw-r--r--   0 alan       (501) staff       (20)      701 2024-05-10 02:46:44.204365 tiny_progress_bar-0.1.1/PKG-INFO
+-rw-r--r--   0 alan       (501) staff       (20)     1101 2024-05-10 02:37:19.000000 tiny_progress_bar-0.1.1/README.md
+-rw-r--r--   0 alan       (501) staff       (20)      100 2024-05-10 02:46:44.204512 tiny_progress_bar-0.1.1/setup.cfg
+-rw-r--r--   0 alan       (501) staff       (20)     1587 2024-05-10 02:46:01.000000 tiny_progress_bar-0.1.1/setup.py
+drwxr-xr-x   0 alan       (501) staff       (20)        0 2024-05-10 02:46:44.203667 tiny_progress_bar-0.1.1/tiny_progress_bar/
+-rw-r--r--   0 alan       (501) staff       (20)     4266 2024-05-10 02:24:06.000000 tiny_progress_bar-0.1.1/tiny_progress_bar/test_tiny_progress_bar.py
+-rw-r--r--   0 alan       (501) staff       (20)     2034 2024-05-10 02:23:26.000000 tiny_progress_bar-0.1.1/tiny_progress_bar/tiny_progress_bar.py
+drwxr-xr-x   0 alan       (501) staff       (20)        0 2024-05-10 02:46:44.204229 tiny_progress_bar-0.1.1/tiny_progress_bar.egg-info/
+-rw-r--r--   0 alan       (501) staff       (20)      701 2024-05-10 02:46:44.000000 tiny_progress_bar-0.1.1/tiny_progress_bar.egg-info/PKG-INFO
+-rw-r--r--   0 alan       (501) staff       (20)      283 2024-05-10 02:46:44.000000 tiny_progress_bar-0.1.1/tiny_progress_bar.egg-info/SOURCES.txt
+-rw-r--r--   0 alan       (501) staff       (20)        1 2024-05-10 02:46:44.000000 tiny_progress_bar-0.1.1/tiny_progress_bar.egg-info/dependency_links.txt
+-rw-r--r--   0 alan       (501) staff       (20)       18 2024-05-10 02:46:44.000000 tiny_progress_bar-0.1.1/tiny_progress_bar.egg-info/top_level.txt
```

### Comparing `tiny_progress_bar-0.1/LICENSE` & `tiny_progress_bar-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tiny_progress_bar-0.1/PKG-INFO` & `tiny_progress_bar-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tiny_progress_bar
-Version: 0.1
+Version: 0.1.1
 Summary: Simple progress bar for Python 3
 Home-page: https://github.com/aklin2/tiny_progress_bar
-Download-URL: https://github.com/aklin2/tiny_progress_bar/archive/refs/tags/v_01.tar.gz
+Download-URL: https://github.com/aklin2/tiny_progress_bar/archive/refs/tags/v0.1.1.tar.gz
 Author: Alan Lin
 Author-email: lin.alan.k@gmail.com
 License: GPL-3.0
 Keywords: progress,progress bar,tiny_progress_bar,loading,loading bar,loading_bar
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `tiny_progress_bar-0.1/README.md` & `tiny_progress_bar-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tiny_progress_bar-0.1/setup.py` & `tiny_progress_bar-0.1.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from distutils.core import setup
 
 setup(
     name="tiny_progress_bar",  # How you named your package folder (MyLib)
     packages=["tiny_progress_bar"],  # Chose the same as "name"
-    version="0.1",  # Start with a small number and increase it with every change you make
+    version="0.1.1",  # Start with a small number and increase it with every change you make
     license="GPL-3.0",  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description="Simple progress bar for Python 3",  # Give a short description about your library
+    readme="README.md",
     author="Alan Lin",  # Type in your name
     author_email="lin.alan.k@gmail.com",  # Type in your E-Mail
     url="https://github.com/aklin2/tiny_progress_bar",  # Provide either the link to your github or to your website
-    download_url="https://github.com/aklin2/tiny_progress_bar/archive/refs/tags/v_01.tar.gz",  # I explain this later on
+    download_url="https://github.com/aklin2/tiny_progress_bar/archive/refs/tags/v0.1.1.tar.gz",  # I explain this later on
     keywords=[
         "progress",
         "progress bar",
         "tiny_progress_bar",
         "loading",
         "loading bar",
         "loading_bar",
```

### Comparing `tiny_progress_bar-0.1/tiny_progress_bar/test_tiny_progress_bar.py` & `tiny_progress_bar-0.1.1/tiny_progress_bar/test_tiny_progress_bar.py`

 * *Files identical despite different names*

### Comparing `tiny_progress_bar-0.1/tiny_progress_bar/tiny_progress_bar.py` & `tiny_progress_bar-0.1.1/tiny_progress_bar/tiny_progress_bar.py`

 * *Files identical despite different names*

### Comparing `tiny_progress_bar-0.1/tiny_progress_bar.egg-info/PKG-INFO` & `tiny_progress_bar-0.1.1/tiny_progress_bar.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tiny-progress-bar
-Version: 0.1
+Version: 0.1.1
 Summary: Simple progress bar for Python 3
 Home-page: https://github.com/aklin2/tiny_progress_bar
-Download-URL: https://github.com/aklin2/tiny_progress_bar/archive/refs/tags/v_01.tar.gz
+Download-URL: https://github.com/aklin2/tiny_progress_bar/archive/refs/tags/v0.1.1.tar.gz
 Author: Alan Lin
 Author-email: lin.alan.k@gmail.com
 License: GPL-3.0
 Keywords: progress,progress bar,tiny_progress_bar,loading,loading bar,loading_bar
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

