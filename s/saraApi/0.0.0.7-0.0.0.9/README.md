# Comparing `tmp/saraapi-0.0.0.7.tar.gz` & `tmp/saraapi-0.0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saraapi-0.0.0.7.tar", last modified: Fri May 10 04:30:51 2024, max compression
+gzip compressed data, was "saraapi-0.0.0.9.tar", last modified: Fri May 10 04:41:49 2024, max compression
```

## Comparing `saraapi-0.0.0.7.tar` & `saraapi-0.0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 04:30:51.035965 saraapi-0.0.0.7/
--rw-rw-rw-   0        0        0        0 2024-05-05 23:25:57.000000 saraapi-0.0.0.7/LICENSE
--rw-rw-rw-   0        0        0     4817 2024-05-10 04:30:51.030630 saraapi-0.0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     4084 2024-05-06 04:15:07.000000 saraapi-0.0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 04:30:50.994140 saraapi-0.0.0.7/sara/
--rw-rw-rw-   0        0        0       81 2024-04-29 01:35:10.000000 saraapi-0.0.0.7/sara/__init__.py
--rw-rw-rw-   0        0        0      587 2024-04-29 01:33:03.000000 saraapi-0.0.0.7/sara/ext.py
--rw-rw-rw-   0        0        0     1937 2024-04-29 01:33:40.000000 saraapi-0.0.0.7/sara/nsfw.py
--rw-rw-rw-   0        0        0      626 2024-05-06 01:28:07.000000 saraapi-0.0.0.7/sara/req.py
--rw-rw-rw-   0        0        0      219 2024-04-29 01:34:39.000000 saraapi-0.0.0.7/sara/sfw.py
-drwxrwxrwx   0        0        0        0 2024-05-10 04:30:51.027924 saraapi-0.0.0.7/saraApi.egg-info/
--rw-rw-rw-   0        0        0     4817 2024-05-10 04:30:50.000000 saraapi-0.0.0.7/saraApi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-05-10 04:30:50.000000 saraapi-0.0.0.7/saraApi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 04:30:50.000000 saraapi-0.0.0.7/saraApi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-10 04:30:50.000000 saraapi-0.0.0.7/saraApi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-10 04:30:50.000000 saraapi-0.0.0.7/saraApi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 04:30:51.035965 saraapi-0.0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1106 2024-05-10 04:30:37.000000 saraapi-0.0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 04:41:49.927851 saraapi-0.0.0.9/
+-rw-rw-rw-   0        0        0        0 2024-05-05 23:25:57.000000 saraapi-0.0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     4817 2024-05-10 04:41:49.920968 saraapi-0.0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4084 2024-05-06 04:15:07.000000 saraapi-0.0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 04:41:49.852371 saraapi-0.0.0.9/sara/
+-rw-rw-rw-   0        0        0       81 2024-04-29 01:35:10.000000 saraapi-0.0.0.9/sara/__init__.py
+-rw-rw-rw-   0        0        0      587 2024-04-29 01:33:03.000000 saraapi-0.0.0.9/sara/ext.py
+-rw-rw-rw-   0        0        0     1937 2024-04-29 01:33:40.000000 saraapi-0.0.0.9/sara/nsfw.py
+-rw-rw-rw-   0        0        0      626 2024-05-06 01:28:07.000000 saraapi-0.0.0.9/sara/req.py
+-rw-rw-rw-   0        0        0      219 2024-04-29 01:34:39.000000 saraapi-0.0.0.9/sara/sfw.py
+drwxrwxrwx   0        0        0        0 2024-05-10 04:41:49.912833 saraapi-0.0.0.9/saraApi.egg-info/
+-rw-rw-rw-   0        0        0     4817 2024-05-10 04:41:49.000000 saraapi-0.0.0.9/saraApi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-05-10 04:41:49.000000 saraapi-0.0.0.9/saraApi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 04:41:49.000000 saraapi-0.0.0.9/saraApi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-10 04:41:49.000000 saraapi-0.0.0.9/saraApi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-10 04:41:49.000000 saraapi-0.0.0.9/saraApi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 04:41:49.929366 saraapi-0.0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1106 2024-05-10 04:41:25.000000 saraapi-0.0.0.9/setup.py
```

### Comparing `saraapi-0.0.0.7/PKG-INFO` & `saraapi-0.0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saraApi
-Version: 0.0.0.7
+Version: 0.0.0.9
 Summary: sara api public based akanekopy
 Home-page: https://github.com/EverGasterXd/sara_api
 Author: evergaster
 License: MIT license
 Keywords: sara anime wallpaper hentai
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: saraApi Version: 0.0.0.7 Summary: sara api public
+Metadata-Version: 2.1 Name: saraApi Version: 0.0.0.9 Summary: sara api public
 based akanekopy Home-page: https://github.com/EverGasterXd/sara_api Author:
 evergaster License: MIT license Keywords: sara anime wallpaper hentai
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Development Status :: 4 - Beta Classifier:
 Natural Language :: English Classifier: Operating System :: Microsoft ::
 Windows :: Windows 10 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Topic :: Internet
```

### Comparing `saraapi-0.0.0.7/README.md` & `saraapi-0.0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `saraapi-0.0.0.7/sara/ext.py` & `saraapi-0.0.0.9/sara/ext.py`

 * *Files identical despite different names*

### Comparing `saraapi-0.0.0.7/sara/nsfw.py` & `saraapi-0.0.0.9/sara/nsfw.py`

 * *Files identical despite different names*

### Comparing `saraapi-0.0.0.7/sara/req.py` & `saraapi-0.0.0.9/sara/req.py`

 * *Files identical despite different names*

### Comparing `saraapi-0.0.0.7/saraApi.egg-info/PKG-INFO` & `saraapi-0.0.0.9/saraApi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saraApi
-Version: 0.0.0.7
+Version: 0.0.0.9
 Summary: sara api public based akanekopy
 Home-page: https://github.com/EverGasterXd/sara_api
 Author: evergaster
 License: MIT license
 Keywords: sara anime wallpaper hentai
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: saraApi Version: 0.0.0.7 Summary: sara api public
+Metadata-Version: 2.1 Name: saraApi Version: 0.0.0.9 Summary: sara api public
 based akanekopy Home-page: https://github.com/EverGasterXd/sara_api Author:
 evergaster License: MIT license Keywords: sara anime wallpaper hentai
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Development Status :: 4 - Beta Classifier:
 Natural Language :: English Classifier: Operating System :: Microsoft ::
 Windows :: Windows 10 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Topic :: Internet
```

### Comparing `saraapi-0.0.0.7/setup.py` & `saraapi-0.0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.md','r', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 install_requires = [
 	'requests'
 ]
 
-version = '0.0.0.7'
+version = '0.0.0.9'
 
 setup(
     author='evergaster',
     version=version,
     description='sara api public based akanekopy',
     install_package_data=True,
     install_requires=install_requires,
```

