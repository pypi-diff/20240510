# Comparing `tmp/dosview-0.1.8.tar.gz` & `tmp/dosview-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dosview-0.1.8.tar", last modified: Wed Apr 24 01:24:57 2024, max compression
+gzip compressed data, was "dosview-0.1.9.tar", last modified: Thu Apr 25 21:02:35 2024, max compression
```

## Comparing `dosview-0.1.8.tar` & `dosview-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:24:57.006067 dosview-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-24 01:24:57.002067 dosview-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-24 01:24:29.000000 dosview-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:24:57.002067 dosview-0.1.8/dosview/
--rw-r--r--   0 runner    (1001) docker     (127)    17677 2024-04-24 01:24:29.000000 dosview-0.1.8/dosview/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:24:57.002067 dosview-0.1.8/dosview.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-24 01:24:56.000000 dosview-0.1.8/dosview.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-24 01:24:56.000000 dosview-0.1.8/dosview.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 01:24:56.000000 dosview-0.1.8/dosview.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-24 01:24:56.000000 dosview-0.1.8/dosview.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-24 01:24:56.000000 dosview-0.1.8/dosview.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-24 01:24:56.000000 dosview-0.1.8/dosview.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 01:24:57.006067 dosview-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-24 01:24:29.000000 dosview-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:02:35.956459 dosview-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-25 21:02:35.956459 dosview-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-25 21:02:08.000000 dosview-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:02:35.956459 dosview-0.1.9/dosview/
+-rw-r--r--   0 runner    (1001) docker     (127)    40695 2024-04-25 21:02:08.000000 dosview-0.1.9/dosview/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:02:35.956459 dosview-0.1.9/dosview.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-25 21:02:35.000000 dosview-0.1.9/dosview.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-25 21:02:35.000000 dosview-0.1.9/dosview.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 21:02:35.000000 dosview-0.1.9/dosview.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-25 21:02:35.000000 dosview-0.1.9/dosview.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-25 21:02:35.000000 dosview-0.1.9/dosview.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-25 21:02:35.000000 dosview-0.1.9/dosview.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 21:02:35.956459 dosview-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-25 21:02:08.000000 dosview-0.1.9/setup.py
```

### Comparing `dosview-0.1.8/PKG-INFO` & `dosview-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dosview
-Version: 0.1.8
+Version: 0.1.9
 Summary: A .dos file viewer
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dosview-0.1.8/README.md` & `dosview-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `dosview-0.1.8/dosview.egg-info/PKG-INFO` & `dosview-0.1.9/dosview.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dosview
-Version: 0.1.8
+Version: 0.1.9
 Summary: A .dos file viewer
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dosview-0.1.8/setup.py` & `dosview-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         copyfile('media/icon_ust.png', '/usr/local/share/icons/icon_ust.png')
 
 # Get the commit hash
 #commit_hash = subprocess.check_output(['git', 'rev-parse', 'HEAD']).decode().strip()
 
 setup(
     name='dosview',
-    version=f'0.1.8',
+    version=f'0.1.9',
     description='A .dos file viewer', 
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'dosview = dosview:main',
```

