# Comparing `tmp/tiny_progress_bar-0.1.3.tar.gz` & `tmp/tiny_progress_bar-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiny_progress_bar-0.1.3.tar", last modified: Fri May 10 04:14:15 2024, max compression
+gzip compressed data, was "tiny_progress_bar-0.1.4.tar", last modified: Fri May 10 04:20:01 2024, max compression
```

## Comparing `tiny_progress_bar-0.1.3.tar` & `tiny_progress_bar-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 alan       (501) staff       (20)        0 2024-05-10 04:14:15.010503 tiny_progress_bar-0.1.3/
--rw-r--r--   0 alan       (501) staff       (20)    35149 2024-05-09 21:02:19.000000 tiny_progress_bar-0.1.3/LICENSE
--rw-r--r--   0 alan       (501) staff       (20)     1843 2024-05-10 04:14:15.010568 tiny_progress_bar-0.1.3/PKG-INFO
--rw-r--r--   0 alan       (501) staff       (20)     1101 2024-05-10 02:37:19.000000 tiny_progress_bar-0.1.3/README.md
--rw-r--r--   0 alan       (501) staff       (20)      160 2024-05-10 04:14:15.010730 tiny_progress_bar-0.1.3/setup.cfg
--rw-r--r--   0 alan       (501) staff       (20)     1816 2024-05-10 04:13:46.000000 tiny_progress_bar-0.1.3/setup.py
-drwxr-xr-x   0 alan       (501) staff       (20)        0 2024-05-10 04:14:15.010004 tiny_progress_bar-0.1.3/tiny_progress_bar/
--rw-r--r--   0 alan       (501) staff       (20)        0 2024-05-10 04:11:41.000000 tiny_progress_bar-0.1.3/tiny_progress_bar/__init__.py
--rw-r--r--   0 alan       (501) staff       (20)     4266 2024-05-10 02:24:06.000000 tiny_progress_bar-0.1.3/tiny_progress_bar/test_tiny_progress_bar.py
--rw-r--r--   0 alan       (501) staff       (20)     2034 2024-05-10 04:11:11.000000 tiny_progress_bar-0.1.3/tiny_progress_bar/tiny_progress_bar.py
-drwxr-xr-x   0 alan       (501) staff       (20)        0 2024-05-10 04:14:15.010409 tiny_progress_bar-0.1.3/tiny_progress_bar.egg-info/
--rw-r--r--   0 alan       (501) staff       (20)     1843 2024-05-10 04:14:15.000000 tiny_progress_bar-0.1.3/tiny_progress_bar.egg-info/PKG-INFO
--rw-r--r--   0 alan       (501) staff       (20)      313 2024-05-10 04:14:15.000000 tiny_progress_bar-0.1.3/tiny_progress_bar.egg-info/SOURCES.txt
--rw-r--r--   0 alan       (501) staff       (20)        1 2024-05-10 04:14:15.000000 tiny_progress_bar-0.1.3/tiny_progress_bar.egg-info/dependency_links.txt
--rw-r--r--   0 alan       (501) staff       (20)       18 2024-05-10 04:14:15.000000 tiny_progress_bar-0.1.3/tiny_progress_bar.egg-info/top_level.txt
+drwxr-xr-x   0 alan       (501) staff       (20)        0 2024-05-10 04:20:01.453692 tiny_progress_bar-0.1.4/
+-rw-r--r--   0 alan       (501) staff       (20)    35149 2024-05-09 21:02:19.000000 tiny_progress_bar-0.1.4/LICENSE
+-rw-r--r--   0 alan       (501) staff       (20)     1843 2024-05-10 04:20:01.453744 tiny_progress_bar-0.1.4/PKG-INFO
+-rw-r--r--   0 alan       (501) staff       (20)     1101 2024-05-10 02:37:19.000000 tiny_progress_bar-0.1.4/README.md
+-rw-r--r--   0 alan       (501) staff       (20)      160 2024-05-10 04:20:01.453887 tiny_progress_bar-0.1.4/setup.cfg
+-rw-r--r--   0 alan       (501) staff       (20)     1816 2024-05-10 04:19:52.000000 tiny_progress_bar-0.1.4/setup.py
+drwxr-xr-x   0 alan       (501) staff       (20)        0 2024-05-10 04:20:01.453073 tiny_progress_bar-0.1.4/tiny_progress_bar/
+-rw-r--r--   0 alan       (501) staff       (20)       25 2024-05-10 04:18:50.000000 tiny_progress_bar-0.1.4/tiny_progress_bar/__init__.py
+-rw-r--r--   0 alan       (501) staff       (20)     4266 2024-05-10 02:24:06.000000 tiny_progress_bar-0.1.4/tiny_progress_bar/test_tiny_progress_bar.py
+-rw-r--r--   0 alan       (501) staff       (20)     2034 2024-05-10 04:11:11.000000 tiny_progress_bar-0.1.4/tiny_progress_bar/tiny_progress_bar.py
+drwxr-xr-x   0 alan       (501) staff       (20)        0 2024-05-10 04:20:01.453594 tiny_progress_bar-0.1.4/tiny_progress_bar.egg-info/
+-rw-r--r--   0 alan       (501) staff       (20)     1843 2024-05-10 04:20:01.000000 tiny_progress_bar-0.1.4/tiny_progress_bar.egg-info/PKG-INFO
+-rw-r--r--   0 alan       (501) staff       (20)      313 2024-05-10 04:20:01.000000 tiny_progress_bar-0.1.4/tiny_progress_bar.egg-info/SOURCES.txt
+-rw-r--r--   0 alan       (501) staff       (20)        1 2024-05-10 04:20:01.000000 tiny_progress_bar-0.1.4/tiny_progress_bar.egg-info/dependency_links.txt
+-rw-r--r--   0 alan       (501) staff       (20)       18 2024-05-10 04:20:01.000000 tiny_progress_bar-0.1.4/tiny_progress_bar.egg-info/top_level.txt
```

### Comparing `tiny_progress_bar-0.1.3/LICENSE` & `tiny_progress_bar-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tiny_progress_bar-0.1.3/PKG-INFO` & `tiny_progress_bar-0.1.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tiny_progress_bar
-Version: 0.1.3
+Version: 0.1.4
 Summary: Simple progress bar for Python 3
 Home-page: https://github.com/aklin2/tiny_progress_bar
-Download-URL: https://github.com/aklin2/tiny_progress_bar/archive/refs/tags/v0.1.3.tar.gz
+Download-URL: https://github.com/aklin2/tiny_progress_bar/archive/refs/tags/v0.1.4.tar.gz
 Author: Alan Lin
 Author-email: lin.alan.k@gmail.com
 License: GPL-3.0
 Keywords: progress,progress bar,tiny_progress_bar,loading,loading bar,loading_bar
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `tiny_progress_bar-0.1.3/README.md` & `tiny_progress_bar-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `tiny_progress_bar-0.1.3/setup.py` & `tiny_progress_bar-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 try:
     import pypandoc
 
     long_description = pypandoc.convert_file("README.md", "rst")
 except (IOError, ImportError):
     long_description = open("README.md").read()
 
-version = "0.1.3"
+version = "0.1.4"
 
 setup(
     name="tiny_progress_bar",  # How you named your package folder (MyLib)
     packages=["tiny_progress_bar"],  # Chose the same as "name"
     version=version,  # Start with a small number and increase it with every change you make
     license="GPL-3.0",  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description="Simple progress bar for Python 3",  # Give a short description about your library
     long_description=long_description,
     readme="README.md",
     author="Alan Lin",  # Type in your name
     author_email="lin.alan.k@gmail.com",  # Type in your E-Mail
     url="https://github.com/aklin2/tiny_progress_bar",  # Provide either the link to your github or to your website
-    download_url="https://github.com/aklin2/tiny_progress_bar/archive/refs/tags/v0.1.3.tar.gz",  # I explain this later on
+    download_url="https://github.com/aklin2/tiny_progress_bar/archive/refs/tags/v0.1.4.tar.gz",  # I explain this later on
     keywords=[
         "progress",
         "progress bar",
         "tiny_progress_bar",
         "loading",
         "loading bar",
         "loading_bar",
```

### Comparing `tiny_progress_bar-0.1.3/tiny_progress_bar/test_tiny_progress_bar.py` & `tiny_progress_bar-0.1.4/tiny_progress_bar/test_tiny_progress_bar.py`

 * *Files identical despite different names*

### Comparing `tiny_progress_bar-0.1.3/tiny_progress_bar/tiny_progress_bar.py` & `tiny_progress_bar-0.1.4/tiny_progress_bar/tiny_progress_bar.py`

 * *Files identical despite different names*

### Comparing `tiny_progress_bar-0.1.3/tiny_progress_bar.egg-info/PKG-INFO` & `tiny_progress_bar-0.1.4/tiny_progress_bar.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tiny-progress-bar
-Version: 0.1.3
+Version: 0.1.4
 Summary: Simple progress bar for Python 3
 Home-page: https://github.com/aklin2/tiny_progress_bar
-Download-URL: https://github.com/aklin2/tiny_progress_bar/archive/refs/tags/v0.1.3.tar.gz
+Download-URL: https://github.com/aklin2/tiny_progress_bar/archive/refs/tags/v0.1.4.tar.gz
 Author: Alan Lin
 Author-email: lin.alan.k@gmail.com
 License: GPL-3.0
 Keywords: progress,progress bar,tiny_progress_bar,loading,loading bar,loading_bar
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

