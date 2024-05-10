# Comparing `tmp/hivebox-2.2.2.tar.gz` & `tmp/hivebox-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hivebox-2.2.2.tar", max compression
+gzip compressed data, was "hivebox-2.3.0.tar", max compression
```

## Comparing `hivebox-2.2.2.tar` & `hivebox-2.3.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0      221 2024-03-07 14:28:38.065710 hivebox-2.2.2/LICENSE
--rw-r--r--   0        0        0     1136 2024-03-07 14:28:38.065710 hivebox-2.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-07 14:28:38.090709 hivebox-2.2.2/src/hivebox/__init__.py
--rw-r--r--   0        0        0     2226 2024-03-07 14:28:38.065710 hivebox-2.2.2/src/hivebox/ai/__init__.py
--rw-r--r--   0        0        0      654 2024-03-07 14:28:38.065710 hivebox-2.2.2/src/hivebox/performance/__init__.py
--rw-r--r--   0        0        0        0 2024-03-07 14:28:38.090709 hivebox-2.2.2/src/hivebox/scripts/__init__.py
--rw-r--r--   0        0        0     3096 2024-03-07 14:28:38.066710 hivebox-2.2.2/src/hivebox/scripts/live.py
--rw-r--r--   0        0        0     3462 2024-03-07 14:28:38.066710 hivebox-2.2.2/src/hivebox/storage/__init__.py
--rw-r--r--   0        0        0      740 1970-01-01 00:00:00.000000 hivebox-2.2.2/PKG-INFO
+-rw-r--r--   0        0        0      221 2024-05-10 11:21:08.276358 hivebox-2.3.0/LICENSE
+-rw-r--r--   0        0        0     1164 2024-05-10 11:21:08.277358 hivebox-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-10 11:21:08.308358 hivebox-2.3.0/src/hivebox/__init__.py
+-rw-r--r--   0        0        0     8018 2024-05-10 11:21:08.277358 hivebox-2.3.0/src/hivebox/common/__init__.py
+-rw-r--r--   0        0        0      654 2024-05-10 11:21:08.277358 hivebox-2.3.0/src/hivebox/performance/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 11:21:08.309358 hivebox-2.3.0/src/hivebox/scripts/__init__.py
+-rw-r--r--   0        0        0     6794 2024-05-10 11:21:08.277358 hivebox-2.3.0/src/hivebox/scripts/collect.py
+-rw-r--r--   0        0        0     3096 2024-05-10 11:21:08.278358 hivebox-2.3.0/src/hivebox/scripts/live.py
+-rw-r--r--   0        0        0      926 2024-05-10 11:21:08.278358 hivebox-2.3.0/src/hivebox/storage/__init__.py
+-rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 hivebox-2.3.0/PKG-INFO
```

### Comparing `hivebox-2.2.2/pyproject.toml` & `hivebox-2.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [tool.poetry]
 name = "hivebox"
-version = "2.2.2"
+version = "2.3.0"
 description = "HiveBox is a toolset helping in AI/ML/CV and other tasks"
 authors = ["HiveCV <lukasz@hivecv.com>"]
 license = "Proprietary"
 packages = [{include = "hivebox", from = "src"}]
 
 
 [tool.poetry.scripts]
 hivebox-live = 'hivebox.scripts.live:main'
+hivebox-capture = 'hivebox.scripts.collect:main'
 
 
 [[tool.poetry.source]]
 name = "PyPI"
 priority = "primary"
 
 [[tool.poetry.source]]
@@ -21,15 +22,14 @@
 priority = "supplemental"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 depthai = "2.24.0.0"
 opencv-python = ">4"
 opencv-contrib-python = ">4"
-flickrapi = "^2.4.0"
 requests = "^2.27"
 numpy = "^1.21"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4"
 twine = "^4.0.2"
```

### Comparing `hivebox-2.2.2/src/hivebox/performance/__init__.py` & `hivebox-2.3.0/src/hivebox/performance/__init__.py`

 * *Files identical despite different names*

### Comparing `hivebox-2.2.2/src/hivebox/scripts/live.py` & `hivebox-2.3.0/src/hivebox/scripts/live.py`

 * *Files identical despite different names*

### Comparing `hivebox-2.2.2/PKG-INFO` & `hivebox-2.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: hivebox
-Version: 2.2.2
+Version: 2.3.0
 Summary: HiveBox is a toolset helping in AI/ML/CV and other tasks
 License: Proprietary
 Author: HiveCV
 Author-email: lukasz@hivecv.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: depthai (==2.24.0.0)
-Requires-Dist: flickrapi (>=2.4.0,<3.0.0)
 Requires-Dist: numpy (>=1.21,<2.0)
 Requires-Dist: opencv-contrib-python (>4)
 Requires-Dist: opencv-python (>4)
 Requires-Dist: requests (>=2.27,<3.0)
```

