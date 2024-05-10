# Comparing `tmp/miqatools-1.1.9.tar.gz` & `tmp/miqatools-1.1.9rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miqatools-1.1.9.tar", last modified: Tue Feb 27 14:45:28 2024, max compression
+gzip compressed data, was "miqatools-1.1.9rc0.tar", last modified: Tue Feb 27 02:47:32 2024, max compression
```

## Comparing `miqatools-1.1.9.tar` & `miqatools-1.1.9rc0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 gwennberry   (501) staff       (20)        0 2024-02-27 14:45:28.314517 miqatools-1.1.9/
--rw-r--r--   0 gwennberry   (501) staff       (20)     1238 2023-08-11 19:34:11.000000 miqatools-1.1.9/LICENSE.txt
--rw-r--r--   0 gwennberry   (501) staff       (20)     1696 2024-02-27 14:45:28.314622 miqatools-1.1.9/PKG-INFO
--rw-r--r--   0 gwennberry   (501) staff       (20)     1423 2024-01-26 22:57:53.000000 miqatools-1.1.9/README.rst
--rw-r--r--   0 gwennberry   (501) staff       (20)      108 2024-02-27 14:45:28.315467 miqatools-1.1.9/setup.cfg
--rw-r--r--   0 gwennberry   (501) staff       (20)      664 2024-02-27 02:53:26.000000 miqatools-1.1.9/setup.py
-drwxr-xr-x   0 gwennberry   (501) staff       (20)        0 2024-02-27 14:45:28.291582 miqatools-1.1.9/src/
-drwxr-xr-x   0 gwennberry   (501) staff       (20)        0 2024-02-27 14:45:28.300229 miqatools-1.1.9/src/miqatools/
--rw-r--r--   0 gwennberry   (501) staff       (20)        0 2023-08-11 19:14:15.000000 miqatools-1.1.9/src/miqatools/__init__.py
-drwxr-xr-x   0 gwennberry   (501) staff       (20)        0 2024-02-27 14:45:28.304299 miqatools-1.1.9/src/miqatools/datamanagement/
--rw-r--r--   0 gwennberry   (501) staff       (20)        0 2023-08-11 19:06:53.000000 miqatools-1.1.9/src/miqatools/datamanagement/__init__.py
-drwxr-xr-x   0 gwennberry   (501) staff       (20)        0 2024-02-27 14:45:28.304754 miqatools-1.1.9/src/miqatools/datamanagement/datasethelpers/
--rw-r--r--   0 gwennberry   (501) staff       (20)     4575 2024-01-27 02:09:48.000000 miqatools-1.1.9/src/miqatools/datamanagement/datasethelpers/__init__.py
-drwxr-xr-x   0 gwennberry   (501) staff       (20)        0 2024-02-27 14:45:28.305631 miqatools-1.1.9/src/miqatools/remoteexecution/
--rw-r--r--   0 gwennberry   (501) staff       (20)        0 2023-08-11 19:06:53.000000 miqatools-1.1.9/src/miqatools/remoteexecution/__init__.py
-drwxr-xr-x   0 gwennberry   (501) staff       (20)        0 2024-02-27 14:45:28.305964 miqatools-1.1.9/src/miqatools/remoteexecution/baseuploadhelpers/
--rw-r--r--   0 gwennberry   (501) staff       (20)     2483 2024-02-12 18:48:55.000000 miqatools-1.1.9/src/miqatools/remoteexecution/baseuploadhelpers/__init__.py
-drwxr-xr-x   0 gwennberry   (501) staff       (20)        0 2024-02-27 14:45:28.306805 miqatools-1.1.9/src/miqatools/remoteexecution/executionhelpers/
--rw-r--r--   0 gwennberry   (501) staff       (20)      905 2024-02-05 23:35:41.000000 miqatools-1.1.9/src/miqatools/remoteexecution/executionhelpers/__init__.py
-drwxr-xr-x   0 gwennberry   (501) staff       (20)        0 2024-02-27 14:45:28.307375 miqatools-1.1.9/src/miqatools/remoteexecution/offlineexecution/
--rw-r--r--   0 gwennberry   (501) staff       (20)     3508 2024-02-12 18:53:53.000000 miqatools-1.1.9/src/miqatools/remoteexecution/offlineexecution/__init__.py
-drwxr-xr-x   0 gwennberry   (501) staff       (20)        0 2024-02-27 14:45:28.308038 miqatools-1.1.9/src/miqatools/remoteexecution/triggertest_helpers/
--rw-r--r--   0 gwennberry   (501) staff       (20)     3717 2024-02-12 20:11:03.000000 miqatools-1.1.9/src/miqatools/remoteexecution/triggertest_helpers/__init__.py
-drwxr-xr-x   0 gwennberry   (501) staff       (20)        0 2024-02-27 14:45:28.309072 miqatools-1.1.9/src/miqatools/remoteexecution/triggertestandupload_dockercmd/
--rw-r--r--   0 gwennberry   (501) staff       (20)     2154 2024-01-26 22:09:58.000000 miqatools-1.1.9/src/miqatools/remoteexecution/triggertestandupload_dockercmd/__init__.py
-drwxr-xr-x   0 gwennberry   (501) staff       (20)        0 2024-02-27 14:45:28.309653 miqatools-1.1.9/src/miqatools/remoteexecution/triggertestandupload_python/
--rw-r--r--   0 gwennberry   (501) staff       (20)    15741 2024-02-12 21:16:50.000000 miqatools-1.1.9/src/miqatools/remoteexecution/triggertestandupload_python/__init__.py
-drwxr-xr-x   0 gwennberry   (501) staff       (20)        0 2024-02-27 14:45:28.310418 miqatools-1.1.9/src/miqatools/remoteexecution/uploadhelpers/
--rw-r--r--   0 gwennberry   (501) staff       (20)    16551 2024-02-27 02:46:45.000000 miqatools-1.1.9/src/miqatools/remoteexecution/uploadhelpers/__init__.py
-drwxr-xr-x   0 gwennberry   (501) staff       (20)        0 2024-02-27 14:45:28.313895 miqatools-1.1.9/src/miqatools/utilities/
--rw-r--r--   0 gwennberry   (501) staff       (20)      438 2024-02-12 20:09:23.000000 miqatools-1.1.9/src/miqatools/utilities/__init__.py
-drwxr-xr-x   0 gwennberry   (501) staff       (20)        0 2024-02-27 14:45:28.303205 miqatools-1.1.9/src/miqatools.egg-info/
--rw-r--r--   0 gwennberry   (501) staff       (20)     1696 2024-02-27 14:45:28.000000 miqatools-1.1.9/src/miqatools.egg-info/PKG-INFO
--rw-r--r--   0 gwennberry   (501) staff       (20)      865 2024-02-27 14:45:28.000000 miqatools-1.1.9/src/miqatools.egg-info/SOURCES.txt
--rw-r--r--   0 gwennberry   (501) staff       (20)        1 2024-02-27 14:45:28.000000 miqatools-1.1.9/src/miqatools.egg-info/dependency_links.txt
--rw-r--r--   0 gwennberry   (501) staff       (20)       16 2024-02-27 14:45:28.000000 miqatools-1.1.9/src/miqatools.egg-info/requires.txt
--rw-r--r--   0 gwennberry   (501) staff       (20)       10 2024-02-27 14:45:28.000000 miqatools-1.1.9/src/miqatools.egg-info/top_level.txt
+drwxr-xr-x   0 gwennberry   (501) staff       (20)        0 2024-02-27 02:47:32.947953 miqatools-1.1.9rc0/
+-rw-r--r--   0 gwennberry   (501) staff       (20)     1238 2023-08-11 19:34:11.000000 miqatools-1.1.9rc0/LICENSE.txt
+-rw-r--r--   0 gwennberry   (501) staff       (20)     1699 2024-02-27 02:47:32.948072 miqatools-1.1.9rc0/PKG-INFO
+-rw-r--r--   0 gwennberry   (501) staff       (20)     1423 2024-01-26 22:57:53.000000 miqatools-1.1.9rc0/README.rst
+-rw-r--r--   0 gwennberry   (501) staff       (20)      108 2024-02-27 02:47:32.948859 miqatools-1.1.9rc0/setup.cfg
+-rw-r--r--   0 gwennberry   (501) staff       (20)      667 2024-02-27 02:47:12.000000 miqatools-1.1.9rc0/setup.py
+drwxr-xr-x   0 gwennberry   (501) staff       (20)        0 2024-02-27 02:47:32.899076 miqatools-1.1.9rc0/src/
+drwxr-xr-x   0 gwennberry   (501) staff       (20)        0 2024-02-27 02:47:32.921211 miqatools-1.1.9rc0/src/miqatools/
+-rw-r--r--   0 gwennberry   (501) staff       (20)        0 2023-08-11 19:14:15.000000 miqatools-1.1.9rc0/src/miqatools/__init__.py
+drwxr-xr-x   0 gwennberry   (501) staff       (20)        0 2024-02-27 02:47:32.936017 miqatools-1.1.9rc0/src/miqatools/datamanagement/
+-rw-r--r--   0 gwennberry   (501) staff       (20)        0 2023-08-11 19:06:53.000000 miqatools-1.1.9rc0/src/miqatools/datamanagement/__init__.py
+drwxr-xr-x   0 gwennberry   (501) staff       (20)        0 2024-02-27 02:47:32.936789 miqatools-1.1.9rc0/src/miqatools/datamanagement/datasethelpers/
+-rw-r--r--   0 gwennberry   (501) staff       (20)     4575 2024-01-27 02:09:48.000000 miqatools-1.1.9rc0/src/miqatools/datamanagement/datasethelpers/__init__.py
+drwxr-xr-x   0 gwennberry   (501) staff       (20)        0 2024-02-27 02:47:32.938224 miqatools-1.1.9rc0/src/miqatools/remoteexecution/
+-rw-r--r--   0 gwennberry   (501) staff       (20)        0 2023-08-11 19:06:53.000000 miqatools-1.1.9rc0/src/miqatools/remoteexecution/__init__.py
+drwxr-xr-x   0 gwennberry   (501) staff       (20)        0 2024-02-27 02:47:32.939096 miqatools-1.1.9rc0/src/miqatools/remoteexecution/baseuploadhelpers/
+-rw-r--r--   0 gwennberry   (501) staff       (20)     2483 2024-02-12 18:48:55.000000 miqatools-1.1.9rc0/src/miqatools/remoteexecution/baseuploadhelpers/__init__.py
+drwxr-xr-x   0 gwennberry   (501) staff       (20)        0 2024-02-27 02:47:32.940247 miqatools-1.1.9rc0/src/miqatools/remoteexecution/executionhelpers/
+-rw-r--r--   0 gwennberry   (501) staff       (20)      905 2024-02-05 23:35:41.000000 miqatools-1.1.9rc0/src/miqatools/remoteexecution/executionhelpers/__init__.py
+drwxr-xr-x   0 gwennberry   (501) staff       (20)        0 2024-02-27 02:47:32.941775 miqatools-1.1.9rc0/src/miqatools/remoteexecution/offlineexecution/
+-rw-r--r--   0 gwennberry   (501) staff       (20)     3508 2024-02-12 18:53:53.000000 miqatools-1.1.9rc0/src/miqatools/remoteexecution/offlineexecution/__init__.py
+drwxr-xr-x   0 gwennberry   (501) staff       (20)        0 2024-02-27 02:47:32.942837 miqatools-1.1.9rc0/src/miqatools/remoteexecution/triggertest_helpers/
+-rw-r--r--   0 gwennberry   (501) staff       (20)     3717 2024-02-12 20:11:03.000000 miqatools-1.1.9rc0/src/miqatools/remoteexecution/triggertest_helpers/__init__.py
+drwxr-xr-x   0 gwennberry   (501) staff       (20)        0 2024-02-27 02:47:32.943906 miqatools-1.1.9rc0/src/miqatools/remoteexecution/triggertestandupload_dockercmd/
+-rw-r--r--   0 gwennberry   (501) staff       (20)     2154 2024-01-26 22:09:58.000000 miqatools-1.1.9rc0/src/miqatools/remoteexecution/triggertestandupload_dockercmd/__init__.py
+drwxr-xr-x   0 gwennberry   (501) staff       (20)        0 2024-02-27 02:47:32.944855 miqatools-1.1.9rc0/src/miqatools/remoteexecution/triggertestandupload_python/
+-rw-r--r--   0 gwennberry   (501) staff       (20)    15741 2024-02-12 21:16:50.000000 miqatools-1.1.9rc0/src/miqatools/remoteexecution/triggertestandupload_python/__init__.py
+drwxr-xr-x   0 gwennberry   (501) staff       (20)        0 2024-02-27 02:47:32.945855 miqatools-1.1.9rc0/src/miqatools/remoteexecution/uploadhelpers/
+-rw-r--r--   0 gwennberry   (501) staff       (20)    16551 2024-02-27 02:46:45.000000 miqatools-1.1.9rc0/src/miqatools/remoteexecution/uploadhelpers/__init__.py
+drwxr-xr-x   0 gwennberry   (501) staff       (20)        0 2024-02-27 02:47:32.947312 miqatools-1.1.9rc0/src/miqatools/utilities/
+-rw-r--r--   0 gwennberry   (501) staff       (20)      438 2024-02-12 20:09:23.000000 miqatools-1.1.9rc0/src/miqatools/utilities/__init__.py
+drwxr-xr-x   0 gwennberry   (501) staff       (20)        0 2024-02-27 02:47:32.934951 miqatools-1.1.9rc0/src/miqatools.egg-info/
+-rw-r--r--   0 gwennberry   (501) staff       (20)     1699 2024-02-27 02:47:32.000000 miqatools-1.1.9rc0/src/miqatools.egg-info/PKG-INFO
+-rw-r--r--   0 gwennberry   (501) staff       (20)      865 2024-02-27 02:47:32.000000 miqatools-1.1.9rc0/src/miqatools.egg-info/SOURCES.txt
+-rw-r--r--   0 gwennberry   (501) staff       (20)        1 2024-02-27 02:47:32.000000 miqatools-1.1.9rc0/src/miqatools.egg-info/dependency_links.txt
+-rw-r--r--   0 gwennberry   (501) staff       (20)       16 2024-02-27 02:47:32.000000 miqatools-1.1.9rc0/src/miqatools.egg-info/requires.txt
+-rw-r--r--   0 gwennberry   (501) staff       (20)       10 2024-02-27 02:47:32.000000 miqatools-1.1.9rc0/src/miqatools.egg-info/top_level.txt
```

### Comparing `miqatools-1.1.9/LICENSE.txt` & `miqatools-1.1.9rc0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `miqatools-1.1.9/PKG-INFO` & `miqatools-1.1.9rc0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miqatools
-Version: 1.1.9
+Version: 1.1.9rc0
 Summary: UNKNOWN
 Home-page: https://www.magnalabs.co
 Author: Gwenn Berry
 Author-email: gwenn@magnalabs.co
 License: GPLv3
 Keywords: miqa
 Platform: UNKNOWN
```

### Comparing `miqatools-1.1.9/README.rst` & `miqatools-1.1.9rc0/README.rst`

 * *Files identical despite different names*

### Comparing `miqatools-1.1.9/setup.py` & `miqatools-1.1.9rc0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = path.abspath(path.dirname(__file__))
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='miqatools',
-    version='1.1.9',
+    version='1.1.9rc0',
     license='GPLv3',
     author="Gwenn Berry",
     author_email='gwenn@magnalabs.co',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     url='https://www.magnalabs.co',
     keywords='miqa',
```

### Comparing `miqatools-1.1.9/src/miqatools/datamanagement/datasethelpers/__init__.py` & `miqatools-1.1.9rc0/src/miqatools/datamanagement/datasethelpers/__init__.py`

 * *Files identical despite different names*

### Comparing `miqatools-1.1.9/src/miqatools/remoteexecution/baseuploadhelpers/__init__.py` & `miqatools-1.1.9rc0/src/miqatools/remoteexecution/baseuploadhelpers/__init__.py`

 * *Files identical despite different names*

### Comparing `miqatools-1.1.9/src/miqatools/remoteexecution/executionhelpers/__init__.py` & `miqatools-1.1.9rc0/src/miqatools/remoteexecution/executionhelpers/__init__.py`

 * *Files identical despite different names*

### Comparing `miqatools-1.1.9/src/miqatools/remoteexecution/offlineexecution/__init__.py` & `miqatools-1.1.9rc0/src/miqatools/remoteexecution/offlineexecution/__init__.py`

 * *Files identical despite different names*

### Comparing `miqatools-1.1.9/src/miqatools/remoteexecution/triggertest_helpers/__init__.py` & `miqatools-1.1.9rc0/src/miqatools/remoteexecution/triggertest_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `miqatools-1.1.9/src/miqatools/remoteexecution/triggertestandupload_dockercmd/__init__.py` & `miqatools-1.1.9rc0/src/miqatools/remoteexecution/triggertestandupload_dockercmd/__init__.py`

 * *Files identical despite different names*

### Comparing `miqatools-1.1.9/src/miqatools/remoteexecution/triggertestandupload_python/__init__.py` & `miqatools-1.1.9rc0/src/miqatools/remoteexecution/triggertestandupload_python/__init__.py`

 * *Files identical despite different names*

### Comparing `miqatools-1.1.9/src/miqatools/remoteexecution/uploadhelpers/__init__.py` & `miqatools-1.1.9rc0/src/miqatools/remoteexecution/uploadhelpers/__init__.py`

 * *Files identical despite different names*

### Comparing `miqatools-1.1.9/src/miqatools.egg-info/PKG-INFO` & `miqatools-1.1.9rc0/src/miqatools.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miqatools
-Version: 1.1.9
+Version: 1.1.9rc0
 Summary: UNKNOWN
 Home-page: https://www.magnalabs.co
 Author: Gwenn Berry
 Author-email: gwenn@magnalabs.co
 License: GPLv3
 Keywords: miqa
 Platform: UNKNOWN
```

### Comparing `miqatools-1.1.9/src/miqatools.egg-info/SOURCES.txt` & `miqatools-1.1.9rc0/src/miqatools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

