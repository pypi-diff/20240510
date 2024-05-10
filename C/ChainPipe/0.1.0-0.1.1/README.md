# Comparing `tmp/ChainPipe-0.1.0.tar.gz` & `tmp/ChainPipe-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ChainPipe-0.1.0.tar", last modified: Fri May 10 07:28:53 2024, max compression
+gzip compressed data, was "ChainPipe-0.1.1.tar", last modified: Fri May 10 08:09:52 2024, max compression
```

## Comparing `ChainPipe-0.1.0.tar` & `ChainPipe-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 aymanmoustafa   (501) staff       (20)        0 2024-05-10 07:28:53.239601 ChainPipe-0.1.0/
-drwxr-xr-x   0 aymanmoustafa   (501) staff       (20)        0 2024-05-10 07:28:53.238029 ChainPipe-0.1.0/ChainPipe.egg-info/
--rw-r--r--   0 aymanmoustafa   (501) staff       (20)     3280 2024-05-10 07:28:53.000000 ChainPipe-0.1.0/ChainPipe.egg-info/PKG-INFO
--rw-r--r--   0 aymanmoustafa   (501) staff       (20)      263 2024-05-10 07:28:53.000000 ChainPipe-0.1.0/ChainPipe.egg-info/SOURCES.txt
--rw-r--r--   0 aymanmoustafa   (501) staff       (20)        1 2024-05-10 07:28:53.000000 ChainPipe-0.1.0/ChainPipe.egg-info/dependency_links.txt
--rw-r--r--   0 aymanmoustafa   (501) staff       (20)       10 2024-05-10 07:28:53.000000 ChainPipe-0.1.0/ChainPipe.egg-info/top_level.txt
--rw-r--r--   0 aymanmoustafa   (501) staff       (20)     1072 2024-05-10 07:07:11.000000 ChainPipe-0.1.0/LICENSE.md
--rw-r--r--   0 aymanmoustafa   (501) staff       (20)     3280 2024-05-10 07:28:53.239342 ChainPipe-0.1.0/PKG-INFO
--rw-r--r--   0 aymanmoustafa   (501) staff       (20)     2494 2024-05-10 07:18:27.000000 ChainPipe-0.1.0/README.md
-drwxr-xr-x   0 aymanmoustafa   (501) staff       (20)        0 2024-05-10 07:28:53.238900 ChainPipe-0.1.0/chainpipe/
--rw-r--r--   0 aymanmoustafa   (501) staff       (20)        0 2024-05-10 06:37:10.000000 ChainPipe-0.1.0/chainpipe/__init__.py
--rw-r--r--   0 aymanmoustafa   (501) staff       (20)        0 2024-05-10 06:37:10.000000 ChainPipe-0.1.0/chainpipe/chain.py
--rw-r--r--   0 aymanmoustafa   (501) staff       (20)      520 2024-05-10 06:40:13.000000 ChainPipe-0.1.0/chainpipe/logger.py
--rw-r--r--   0 aymanmoustafa   (501) staff       (20)        0 2024-05-10 06:37:10.000000 ChainPipe-0.1.0/chainpipe/pipeline.py
--rw-r--r--   0 aymanmoustafa   (501) staff       (20)      511 2024-05-10 06:40:04.000000 ChainPipe-0.1.0/chainpipe/timer.py
--rw-r--r--   0 aymanmoustafa   (501) staff       (20)       38 2024-05-10 07:28:53.239647 ChainPipe-0.1.0/setup.cfg
--rw-r--r--   0 aymanmoustafa   (501) staff       (20)     1176 2024-05-10 06:46:05.000000 ChainPipe-0.1.0/setup.py
+drwxr-xr-x   0 aymanmoustafa   (501) staff       (20)        0 2024-05-10 08:09:52.790356 ChainPipe-0.1.1/
+drwxr-xr-x   0 aymanmoustafa   (501) staff       (20)        0 2024-05-10 08:09:52.788611 ChainPipe-0.1.1/ChainPipe.egg-info/
+-rw-r--r--   0 aymanmoustafa   (501) staff       (20)     3280 2024-05-10 08:09:52.000000 ChainPipe-0.1.1/ChainPipe.egg-info/PKG-INFO
+-rw-r--r--   0 aymanmoustafa   (501) staff       (20)      263 2024-05-10 08:09:52.000000 ChainPipe-0.1.1/ChainPipe.egg-info/SOURCES.txt
+-rw-r--r--   0 aymanmoustafa   (501) staff       (20)        1 2024-05-10 08:09:52.000000 ChainPipe-0.1.1/ChainPipe.egg-info/dependency_links.txt
+-rw-r--r--   0 aymanmoustafa   (501) staff       (20)       10 2024-05-10 08:09:52.000000 ChainPipe-0.1.1/ChainPipe.egg-info/top_level.txt
+-rw-r--r--   0 aymanmoustafa   (501) staff       (20)     1072 2024-05-10 07:07:11.000000 ChainPipe-0.1.1/LICENSE.md
+-rw-r--r--   0 aymanmoustafa   (501) staff       (20)     3280 2024-05-10 08:09:52.790068 ChainPipe-0.1.1/PKG-INFO
+-rw-r--r--   0 aymanmoustafa   (501) staff       (20)     2494 2024-05-10 07:18:27.000000 ChainPipe-0.1.1/README.md
+drwxr-xr-x   0 aymanmoustafa   (501) staff       (20)        0 2024-05-10 08:09:52.789650 ChainPipe-0.1.1/chainpipe/
+-rw-r--r--   0 aymanmoustafa   (501) staff       (20)       55 2024-05-10 08:03:10.000000 ChainPipe-0.1.1/chainpipe/__init__.py
+-rw-r--r--   0 aymanmoustafa   (501) staff       (20)     1874 2024-05-10 07:54:59.000000 ChainPipe-0.1.1/chainpipe/chain.py
+-rw-r--r--   0 aymanmoustafa   (501) staff       (20)      520 2024-05-10 06:40:13.000000 ChainPipe-0.1.1/chainpipe/logger.py
+-rw-r--r--   0 aymanmoustafa   (501) staff       (20)     1597 2024-05-10 07:55:19.000000 ChainPipe-0.1.1/chainpipe/pipeline.py
+-rw-r--r--   0 aymanmoustafa   (501) staff       (20)      511 2024-05-10 06:40:04.000000 ChainPipe-0.1.1/chainpipe/timer.py
+-rw-r--r--   0 aymanmoustafa   (501) staff       (20)       38 2024-05-10 08:09:52.790400 ChainPipe-0.1.1/setup.cfg
+-rw-r--r--   0 aymanmoustafa   (501) staff       (20)     1176 2024-05-10 08:09:19.000000 ChainPipe-0.1.1/setup.py
```

### Comparing `ChainPipe-0.1.0/ChainPipe.egg-info/PKG-INFO` & `ChainPipe-0.1.1/ChainPipe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChainPipe
-Version: 0.1.0
+Version: 0.1.1
 Summary: A utility package for chaining and pipeline operations with enhanced logging and timing.
 Home-page: https://github.com/ayman3000/ChainPipe
 Author: Ayman Hamed
 Author-email: ayman3000@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `ChainPipe-0.1.0/LICENSE.md` & `ChainPipe-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ChainPipe-0.1.0/PKG-INFO` & `ChainPipe-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChainPipe
-Version: 0.1.0
+Version: 0.1.1
 Summary: A utility package for chaining and pipeline operations with enhanced logging and timing.
 Home-page: https://github.com/ayman3000/ChainPipe
 Author: Ayman Hamed
 Author-email: ayman3000@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `ChainPipe-0.1.0/README.md` & `ChainPipe-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ChainPipe-0.1.0/chainpipe/logger.py` & `ChainPipe-0.1.1/chainpipe/logger.py`

 * *Files identical despite different names*

### Comparing `ChainPipe-0.1.0/setup.py` & `ChainPipe-0.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ChainPipe',
-    version='0.1.0',  # Increment with updates
+    version='0.1.1',  # Increment with updates
     author='Ayman Hamed',
     author_email='ayman3000@gmail.com',
     description='A utility package for chaining and pipeline operations with enhanced logging and timing.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/ayman3000/ChainPipe',  # Replace with the URL of your repository
     packages=find_packages(),
```

