# Comparing `tmp/tiny_progress_bar-0.1.1.tar.gz` & `tmp/tiny_progress_bar-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiny_progress_bar-0.1.1.tar", last modified: Fri May 10 02:46:44 2024, max compression
+gzip compressed data, was "tiny_progress_bar-0.1.2.tar", last modified: Fri May 10 04:05:27 2024, max compression
```

## Comparing `tiny_progress_bar-0.1.1.tar` & `tiny_progress_bar-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,11 @@
-drwxr-xr-x   0 alan       (501) staff       (20)        0 2024-05-10 02:46:44.204315 tiny_progress_bar-0.1.1/
--rw-r--r--   0 alan       (501) staff       (20)    35149 2024-05-09 21:02:19.000000 tiny_progress_bar-0.1.1/LICENSE
--rw-r--r--   0 alan       (501) staff       (20)      701 2024-05-10 02:46:44.204365 tiny_progress_bar-0.1.1/PKG-INFO
--rw-r--r--   0 alan       (501) staff       (20)     1101 2024-05-10 02:37:19.000000 tiny_progress_bar-0.1.1/README.md
--rw-r--r--   0 alan       (501) staff       (20)      100 2024-05-10 02:46:44.204512 tiny_progress_bar-0.1.1/setup.cfg
--rw-r--r--   0 alan       (501) staff       (20)     1587 2024-05-10 02:46:01.000000 tiny_progress_bar-0.1.1/setup.py
-drwxr-xr-x   0 alan       (501) staff       (20)        0 2024-05-10 02:46:44.203667 tiny_progress_bar-0.1.1/tiny_progress_bar/
--rw-r--r--   0 alan       (501) staff       (20)     4266 2024-05-10 02:24:06.000000 tiny_progress_bar-0.1.1/tiny_progress_bar/test_tiny_progress_bar.py
--rw-r--r--   0 alan       (501) staff       (20)     2034 2024-05-10 02:23:26.000000 tiny_progress_bar-0.1.1/tiny_progress_bar/tiny_progress_bar.py
-drwxr-xr-x   0 alan       (501) staff       (20)        0 2024-05-10 02:46:44.204229 tiny_progress_bar-0.1.1/tiny_progress_bar.egg-info/
--rw-r--r--   0 alan       (501) staff       (20)      701 2024-05-10 02:46:44.000000 tiny_progress_bar-0.1.1/tiny_progress_bar.egg-info/PKG-INFO
--rw-r--r--   0 alan       (501) staff       (20)      283 2024-05-10 02:46:44.000000 tiny_progress_bar-0.1.1/tiny_progress_bar.egg-info/SOURCES.txt
--rw-r--r--   0 alan       (501) staff       (20)        1 2024-05-10 02:46:44.000000 tiny_progress_bar-0.1.1/tiny_progress_bar.egg-info/dependency_links.txt
--rw-r--r--   0 alan       (501) staff       (20)       18 2024-05-10 02:46:44.000000 tiny_progress_bar-0.1.1/tiny_progress_bar.egg-info/top_level.txt
+drwxr-xr-x   0 alan       (501) staff       (20)        0 2024-05-10 04:05:27.048636 tiny_progress_bar-0.1.2/
+-rw-r--r--   0 alan       (501) staff       (20)    35149 2024-05-09 21:02:19.000000 tiny_progress_bar-0.1.2/LICENSE
+-rw-r--r--   0 alan       (501) staff       (20)     1843 2024-05-10 04:05:27.048709 tiny_progress_bar-0.1.2/PKG-INFO
+-rw-r--r--   0 alan       (501) staff       (20)     1101 2024-05-10 02:37:19.000000 tiny_progress_bar-0.1.2/README.md
+-rw-r--r--   0 alan       (501) staff       (20)      160 2024-05-10 04:05:27.048910 tiny_progress_bar-0.1.2/setup.cfg
+-rw-r--r--   0 alan       (501) staff       (20)     1816 2024-05-10 04:04:06.000000 tiny_progress_bar-0.1.2/setup.py
+drwxr-xr-x   0 alan       (501) staff       (20)        0 2024-05-10 04:05:27.048489 tiny_progress_bar-0.1.2/tiny_progress_bar.egg-info/
+-rw-r--r--   0 alan       (501) staff       (20)     1843 2024-05-10 04:05:27.000000 tiny_progress_bar-0.1.2/tiny_progress_bar.egg-info/PKG-INFO
+-rw-r--r--   0 alan       (501) staff       (20)      200 2024-05-10 04:05:27.000000 tiny_progress_bar-0.1.2/tiny_progress_bar.egg-info/SOURCES.txt
+-rw-r--r--   0 alan       (501) staff       (20)        1 2024-05-10 04:05:27.000000 tiny_progress_bar-0.1.2/tiny_progress_bar.egg-info/dependency_links.txt
+-rw-r--r--   0 alan       (501) staff       (20)       18 2024-05-10 04:05:27.000000 tiny_progress_bar-0.1.2/tiny_progress_bar.egg-info/top_level.txt
```

### Comparing `tiny_progress_bar-0.1.1/LICENSE` & `tiny_progress_bar-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tiny_progress_bar-0.1.1/README.md` & `tiny_progress_bar-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `tiny_progress_bar-0.1.1/setup.py` & `tiny_progress_bar-0.1.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 from distutils.core import setup
 
+try:
+    import pypandoc
+
+    long_description = pypandoc.convert_file("README.md", "rst")
+except (IOError, ImportError):
+    long_description = open("README.md").read()
+
+version = "0.1.2"
+
 setup(
     name="tiny_progress_bar",  # How you named your package folder (MyLib)
     packages=["tiny_progress_bar"],  # Chose the same as "name"
-    version="0.1.1",  # Start with a small number and increase it with every change you make
+    version=version,  # Start with a small number and increase it with every change you make
     license="GPL-3.0",  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description="Simple progress bar for Python 3",  # Give a short description about your library
+    long_description=long_description,
     readme="README.md",
     author="Alan Lin",  # Type in your name
     author_email="lin.alan.k@gmail.com",  # Type in your E-Mail
     url="https://github.com/aklin2/tiny_progress_bar",  # Provide either the link to your github or to your website
-    download_url="https://github.com/aklin2/tiny_progress_bar/archive/refs/tags/v0.1.1.tar.gz",  # I explain this later on
+    download_url="https://github.com/aklin2/tiny_progress_bar/archive/refs/tags/v0.1.2.tar.gz",  # I explain this later on
     keywords=[
         "progress",
         "progress bar",
         "tiny_progress_bar",
         "loading",
         "loading bar",
         "loading_bar",
```

