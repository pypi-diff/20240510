# Comparing `tmp/convkan-0.0.1.tar.gz` & `tmp/convkan-0.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "convkan-0.0.1.tar", last modified: Fri May 10 11:55:58 2024, max compression
+gzip compressed data, was "convkan-0.0.1.1.tar", last modified: Fri May 10 12:50:14 2024, max compression
```

## Comparing `convkan-0.0.1.tar` & `convkan-0.0.1.1.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 11:55:58.572443 convkan-0.0.1/
--rw-rw-rw-   0        0        0     1079 2024-05-10 09:37:05.000000 convkan-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2896 2024-05-10 11:55:58.572443 convkan-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2499 2024-05-10 11:51:14.000000 convkan-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 11:55:58.541805 convkan-0.0.1/convkan/
--rw-rw-rw-   0        0        0      182 2024-05-10 11:26:48.000000 convkan-0.0.1/convkan/__init__.py
--rw-rw-rw-   0        0        0     5640 2024-05-10 11:54:33.000000 convkan-0.0.1/convkan/convkan_layer.py
--rw-rw-rw-   0        0        0     8954 2024-05-10 10:02:30.000000 convkan-0.0.1/convkan/kanlinear.py
--rw-rw-rw-   0        0        0      656 2024-05-09 18:56:14.000000 convkan-0.0.1/convkan/layernorm2d.py
-drwxrwxrwx   0        0        0        0 2024-05-10 11:55:58.570326 convkan-0.0.1/convkan.egg-info/
--rw-rw-rw-   0        0        0     2896 2024-05-10 11:55:58.000000 convkan-0.0.1/convkan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2024-05-10 11:55:58.000000 convkan-0.0.1/convkan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 11:55:58.000000 convkan-0.0.1/convkan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-05-10 11:55:58.000000 convkan-0.0.1/convkan.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-10 11:55:58.000000 convkan-0.0.1/convkan.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 11:55:58.572443 convkan-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      864 2024-05-09 19:00:34.000000 convkan-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-10 11:55:58.571319 convkan-0.0.1/tests/
--rw-rw-rw-   0        0        0        0 2024-05-10 09:58:31.000000 convkan-0.0.1/tests/__init__.py
--rw-rw-rw-   0        0        0     4906 2024-05-10 11:55:04.000000 convkan-0.0.1/tests/test_convkan.py
+drwxrwxrwx   0        0        0        0 2024-05-10 12:50:14.736222 convkan-0.0.1.1/
+-rw-rw-rw-   0        0        0     1079 2024-05-10 09:37:05.000000 convkan-0.0.1.1/LICENSE
+-rw-rw-rw-   0        0        0       64 2024-05-10 12:49:00.000000 convkan-0.0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2965 2024-05-10 12:50:14.735221 convkan-0.0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2566 2024-05-10 12:18:06.000000 convkan-0.0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 12:50:14.700827 convkan-0.0.1.1/convkan/
+-rw-rw-rw-   0        0        0      182 2024-05-10 11:26:48.000000 convkan-0.0.1.1/convkan/__init__.py
+-rw-rw-rw-   0        0        0     5640 2024-05-10 11:54:33.000000 convkan-0.0.1.1/convkan/convkan_layer.py
+-rw-rw-rw-   0        0        0     8954 2024-05-10 10:02:30.000000 convkan-0.0.1.1/convkan/kanlinear.py
+-rw-rw-rw-   0        0        0     9618 2024-05-10 12:33:50.000000 convkan-0.0.1.1/convkan/kanresnet.py
+-rw-rw-rw-   0        0        0      656 2024-05-09 18:56:14.000000 convkan-0.0.1.1/convkan/layernorm2d.py
+drwxrwxrwx   0        0        0        0 2024-05-10 12:50:14.734221 convkan-0.0.1.1/convkan.egg-info/
+-rw-rw-rw-   0        0        0     2965 2024-05-10 12:50:14.000000 convkan-0.0.1.1/convkan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      359 2024-05-10 12:50:14.000000 convkan-0.0.1.1/convkan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 12:50:14.000000 convkan-0.0.1.1/convkan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-05-10 12:50:14.000000 convkan-0.0.1.1/convkan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-10 12:50:14.000000 convkan-0.0.1.1/convkan.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       62 2024-05-10 09:59:45.000000 convkan-0.0.1.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 12:50:14.736222 convkan-0.0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      866 2024-05-10 12:50:05.000000 convkan-0.0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 12:50:14.735221 convkan-0.0.1.1/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-10 09:58:31.000000 convkan-0.0.1.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     4906 2024-05-10 11:55:04.000000 convkan-0.0.1.1/tests/test_convkan.py
```

### Comparing `convkan-0.0.1/LICENSE` & `convkan-0.0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `convkan-0.0.1/PKG-INFO` & `convkan-0.0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convkan
-Version: 0.0.1
+Version: 0.0.1.1
 Summary: Convolutional KAN layer
 Author: Vladimir Starostin
 Author-email: vladimir.starostin@uni-tuebingen.de
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -21,14 +21,22 @@
 
 Currently, supports grouped convolution, padding with different modes, dilation, and stride. 
 
 The KAN implementation is taken from the https://github.com/Blealtan/efficient-kan/ repository.
 
 ## Installation
 
+From PyPI:
+
+```bash
+pip install convkan
+```
+
+From source:
+
 ```bash
 git clone git@github.com:StarostinV/convkan.git
 cd convkan
 pip install .
 ```
 
 ## Usage
```

### Comparing `convkan-0.0.1/README.md` & `convkan-0.0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,22 @@
 
 Currently, supports grouped convolution, padding with different modes, dilation, and stride. 
 
 The KAN implementation is taken from the https://github.com/Blealtan/efficient-kan/ repository.
 
 ## Installation
 
+From PyPI:
+
+```bash
+pip install convkan
+```
+
+From source:
+
 ```bash
 git clone git@github.com:StarostinV/convkan.git
 cd convkan
 pip install .
 ```
 
 ## Usage
```

### Comparing `convkan-0.0.1/convkan/convkan_layer.py` & `convkan-0.0.1.1/convkan/convkan_layer.py`

 * *Files identical despite different names*

### Comparing `convkan-0.0.1/convkan/kanlinear.py` & `convkan-0.0.1.1/convkan/kanlinear.py`

 * *Files identical despite different names*

### Comparing `convkan-0.0.1/convkan/layernorm2d.py` & `convkan-0.0.1.1/convkan/layernorm2d.py`

 * *Files identical despite different names*

### Comparing `convkan-0.0.1/convkan.egg-info/PKG-INFO` & `convkan-0.0.1.1/convkan.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convkan
-Version: 0.0.1
+Version: 0.0.1.1
 Summary: Convolutional KAN layer
 Author: Vladimir Starostin
 Author-email: vladimir.starostin@uni-tuebingen.de
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -21,14 +21,22 @@
 
 Currently, supports grouped convolution, padding with different modes, dilation, and stride. 
 
 The KAN implementation is taken from the https://github.com/Blealtan/efficient-kan/ repository.
 
 ## Installation
 
+From PyPI:
+
+```bash
+pip install convkan
+```
+
+From source:
+
 ```bash
 git clone git@github.com:StarostinV/convkan.git
 cd convkan
 pip install .
 ```
 
 ## Usage
```

### Comparing `convkan-0.0.1/setup.py` & `convkan-0.0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 python_requires = '>=3.8'
 install_requires = read_file('requirements.txt').splitlines()
 
 setup(
     name=PACKAGE_NAME,
     packages=find_packages(),
-    version='0.0.1',
+    version='0.0.1.1',
     author='Vladimir Starostin',
     author_email='vladimir.starostin@uni-tuebingen.de',
     license='MIT',
     description='Convolutional KAN layer',
     long_description=long_description,
     long_description_content_type=long_description_content_type,
     python_requires=python_requires,
```

### Comparing `convkan-0.0.1/tests/test_convkan.py` & `convkan-0.0.1.1/tests/test_convkan.py`

 * *Files identical despite different names*

