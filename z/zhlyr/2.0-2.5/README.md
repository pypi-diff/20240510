# Comparing `tmp/zhlyr-2.0.tar.gz` & `tmp/zhlyr-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhlyr-2.0.tar", last modified: Fri May 10 13:37:17 2024, max compression
+gzip compressed data, was "zhlyr-2.5.tar", last modified: Fri May 10 13:45:58 2024, max compression
```

## Comparing `zhlyr-2.0.tar` & `zhlyr-2.5.tar`

### file list

```diff
@@ -1,9 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 13:37:17.865372 zhlyr-2.0/
--rw-rw-rw-   0        0        0      889 2024-05-10 13:37:17.862348 zhlyr-2.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-10 13:37:17.866369 zhlyr-2.0/setup.cfg
--rw-rw-rw-   0        0        0     1086 2024-05-10 13:36:16.000000 zhlyr-2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-10 13:37:17.860838 zhlyr-2.0/zhlyr.egg-info/
--rw-rw-rw-   0        0        0      889 2024-05-10 13:37:17.000000 zhlyr-2.0/zhlyr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      124 2024-05-10 13:37:17.000000 zhlyr-2.0/zhlyr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 13:37:17.000000 zhlyr-2.0/zhlyr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 13:37:17.000000 zhlyr-2.0/zhlyr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 13:45:58.310684 zhlyr-2.5/
+-rw-rw-rw-   0        0        0      889 2024-05-10 13:45:58.309162 zhlyr-2.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-10 13:45:58.310684 zhlyr-2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1079 2024-05-10 13:45:29.000000 zhlyr-2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:45:58.293076 zhlyr-2.5/zhlyr/
+-rw-rw-rw-   0        0        0       91 2024-05-10 13:42:14.000000 zhlyr-2.5/zhlyr/__init__.py
+-rw-rw-rw-   0        0        0     1445 2024-05-10 10:49:35.000000 zhlyr-2.5/zhlyr/recosnize.py
+-rw-rw-rw-   0        0        0     1933 2024-05-10 13:40:19.000000 zhlyr-2.5/zhlyr/serilize.py
+-rw-rw-rw-   0        0        0     2159 2024-05-10 13:04:05.000000 zhlyr-2.5/zhlyr/zhlyr.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:45:58.307165 zhlyr-2.5/zhlyr.egg-info/
+-rw-rw-rw-   0        0        0      889 2024-05-10 13:45:58.000000 zhlyr-2.5/zhlyr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2024-05-10 13:45:58.000000 zhlyr-2.5/zhlyr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 13:45:58.000000 zhlyr-2.5/zhlyr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-10 13:45:58.000000 zhlyr-2.5/zhlyr.egg-info/top_level.txt
```

### Comparing `zhlyr-2.0/PKG-INFO` & `zhlyr-2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhlyr
-Version: 2.0
+Version: 2.5
 Summary: Python library for music handling
 Home-page: https://github.com/Gaoc3/zhlyr
 Author: Mtsky
 Author-email: secon2636@gmail.com
 License: MIT
 Keywords: lyrics,music,shazam,serialize,serializer,recognize
 Classifier: Development Status :: 1 - Planning
```

### Comparing `zhlyr-2.0/setup.py` & `zhlyr-2.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup , find_packages
 
 setup(
     name = 'zhlyr',
-    version = '2.0',
-    packages = find_packages('zhlib'),
+    version = '2.5',
+    packages = find_packages(),
     requires = ['requests','shazamio','shazam'],
     long_description ='**A python package to get lyrics from music , serialize data from json response and recognize data from musics**',
     long_description_content_type='text/markdown',
     description = 'Python library for music handling',
     author = 'Mtsky',
     author_email = 'secon2636@gmail.com',
     url = 'https://github.com/Gaoc3/zhlyr',
```

### Comparing `zhlyr-2.0/zhlyr.egg-info/PKG-INFO` & `zhlyr-2.5/zhlyr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhlyr
-Version: 2.0
+Version: 2.5
 Summary: Python library for music handling
 Home-page: https://github.com/Gaoc3/zhlyr
 Author: Mtsky
 Author-email: secon2636@gmail.com
 License: MIT
 Keywords: lyrics,music,shazam,serialize,serializer,recognize
 Classifier: Development Status :: 1 - Planning
```

