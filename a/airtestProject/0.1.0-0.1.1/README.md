# Comparing `tmp/airtestproject-0.1.0.tar.gz` & `tmp/airtestproject-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "G:\pyProject\odin-testautomation\TestAutomation\dist\.tmp-po62ebm_\airtestproject-0.1.0.tar", last modified: Fri May 10 09:57:18 2024, max compression
+gzip compressed data, was "G:\pyProject\odin-testautomation\TestAutomation\dist\.tmp-hjmf8lgp\airtestproject-0.1.1.tar", last modified: Fri May 10 10:40:34 2024, max compression
```

## Comparing `airtestproject-0.1.0.tar` & `airtestproject-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 09:57:18.308244 airtestproject-0.1.0/
--rw-rw-rw-   0        0        0     1093 2024-05-10 09:37:02.000000 airtestproject-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      623 2024-05-10 09:57:18.307237 airtestproject-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      134 2024-05-10 09:55:18.000000 airtestproject-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 09:57:18.306240 airtestproject-0.1.0/airtestProject.egg-info/
--rw-rw-rw-   0        0        0      623 2024-05-10 09:57:18.000000 airtestproject-0.1.0/airtestProject.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2024-05-10 09:57:18.000000 airtestproject-0.1.0/airtestProject.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 09:57:18.000000 airtestproject-0.1.0/airtestProject.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      139 2024-05-10 09:57:18.000000 airtestproject-0.1.0/airtestProject.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 09:57:18.000000 airtestproject-0.1.0/airtestProject.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 09:57:18.308244 airtestproject-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      819 2024-05-10 09:57:08.000000 airtestproject-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 10:40:34.570884 airtestproject-0.1.1/
+-rw-rw-rw-   0        0        0     1093 2024-05-10 09:37:02.000000 airtestproject-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      623 2024-05-10 10:40:34.569887 airtestproject-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      134 2024-05-10 09:55:18.000000 airtestproject-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 10:40:34.568889 airtestproject-0.1.1/airtestProject.egg-info/
+-rw-rw-rw-   0        0        0      623 2024-05-10 10:40:34.000000 airtestproject-0.1.1/airtestProject.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2024-05-10 10:40:34.000000 airtestproject-0.1.1/airtestProject.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 10:40:34.000000 airtestproject-0.1.1/airtestProject.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      139 2024-05-10 10:40:34.000000 airtestproject-0.1.1/airtestProject.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 10:40:34.000000 airtestproject-0.1.1/airtestProject.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 10:40:34.571880 airtestproject-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      819 2024-05-10 10:40:26.000000 airtestproject-0.1.1/setup.py
```

### Comparing `airtestproject-0.1.0/LICENSE` & `airtestproject-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.0/PKG-INFO` & `airtestproject-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airtestProject
-Version: 0.1.0
+Version: 0.1.1
 Author: mortal_sjh
 Author-email: mortal_sjh@qq.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: airtest==1.3.3
 Requires-Dist: openpyxl==1.1.0
```

### Comparing `airtestproject-0.1.0/airtestProject.egg-info/PKG-INFO` & `airtestproject-0.1.1/airtestProject.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airtestProject
-Version: 0.1.0
+Version: 0.1.1
 Author: mortal_sjh
 Author-email: mortal_sjh@qq.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: airtest==1.3.3
 Requires-Dist: openpyxl==1.1.0
```

### Comparing `airtestproject-0.1.0/setup.py` & `airtestproject-0.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name='airtestProject',
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(include=['airtestProject', 'airtestProject.*']),
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         "airtest==1.3.3",
         "openpyxl==1.1.0",
         "pocoui==1.0.94",
```

