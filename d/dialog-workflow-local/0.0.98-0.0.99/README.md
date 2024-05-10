# Comparing `tmp/dialog_workflow_local-0.0.98.tar.gz` & `tmp/dialog_workflow_local-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dialog_workflow_local-0.0.98.tar", last modified: Sat Apr 27 23:36:07 2024, max compression
+gzip compressed data, was "dialog_workflow_local-0.0.99.tar", last modified: Tue Apr 30 20:02:30 2024, max compression
```

## Comparing `dialog_workflow_local-0.0.98.tar` & `dialog_workflow_local-0.0.99.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:36:07.036055 dialog_workflow_local-0.0.98/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-27 23:36:07.036055 dialog_workflow_local-0.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-27 23:35:33.000000 dialog_workflow_local-0.0.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:36:07.032055 dialog_workflow_local-0.0.98/dialog_workflow_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:36:07.036055 dialog_workflow_local-0.0.98/dialog_workflow_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-27 23:35:33.000000 dialog_workflow_local-0.0.98/dialog_workflow_local/src/Constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-04-27 23:35:33.000000 dialog_workflow_local-0.0.98/dialog_workflow_local/src/DialogWorkflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-27 23:35:33.000000 dialog_workflow_local-0.0.98/dialog_workflow_local/src/ProfileContext.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:35:33.000000 dialog_workflow_local-0.0.98/dialog_workflow_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29881 2024-04-27 23:35:33.000000 dialog_workflow_local-0.0.98/dialog_workflow_local/src/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     9680 2024-04-27 23:35:33.000000 dialog_workflow_local-0.0.98/dialog_workflow_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:36:07.036055 dialog_workflow_local-0.0.98/dialog_workflow_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-27 23:36:07.000000 dialog_workflow_local-0.0.98/dialog_workflow_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-27 23:36:07.000000 dialog_workflow_local-0.0.98/dialog_workflow_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 23:36:07.000000 dialog_workflow_local-0.0.98/dialog_workflow_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-27 23:36:07.000000 dialog_workflow_local-0.0.98/dialog_workflow_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-27 23:36:07.000000 dialog_workflow_local-0.0.98/dialog_workflow_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-27 23:35:33.000000 dialog_workflow_local-0.0.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 23:36:07.036055 dialog_workflow_local-0.0.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-27 23:35:33.000000 dialog_workflow_local-0.0.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:02:30.840299 dialog_workflow_local-0.0.99/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-30 20:02:30.840299 dialog_workflow_local-0.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-30 20:02:00.000000 dialog_workflow_local-0.0.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:02:30.836299 dialog_workflow_local-0.0.99/dialog_workflow_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:02:30.840299 dialog_workflow_local-0.0.99/dialog_workflow_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-30 20:02:00.000000 dialog_workflow_local-0.0.99/dialog_workflow_local/src/Constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-04-30 20:02:00.000000 dialog_workflow_local-0.0.99/dialog_workflow_local/src/DialogWorkflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-30 20:02:00.000000 dialog_workflow_local-0.0.99/dialog_workflow_local/src/ProfileContext.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:02:00.000000 dialog_workflow_local-0.0.99/dialog_workflow_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29881 2024-04-30 20:02:00.000000 dialog_workflow_local-0.0.99/dialog_workflow_local/src/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9680 2024-04-30 20:02:00.000000 dialog_workflow_local-0.0.99/dialog_workflow_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:02:30.840299 dialog_workflow_local-0.0.99/dialog_workflow_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-30 20:02:30.000000 dialog_workflow_local-0.0.99/dialog_workflow_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-30 20:02:30.000000 dialog_workflow_local-0.0.99/dialog_workflow_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 20:02:30.000000 dialog_workflow_local-0.0.99/dialog_workflow_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-30 20:02:30.000000 dialog_workflow_local-0.0.99/dialog_workflow_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-30 20:02:30.000000 dialog_workflow_local-0.0.99/dialog_workflow_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-30 20:02:00.000000 dialog_workflow_local-0.0.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 20:02:30.840299 dialog_workflow_local-0.0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-30 20:02:00.000000 dialog_workflow_local-0.0.99/setup.py
```

### Comparing `dialog_workflow_local-0.0.98/README.md` & `dialog_workflow_local-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `dialog_workflow_local-0.0.98/dialog_workflow_local/src/Constants.py` & `dialog_workflow_local-0.0.99/dialog_workflow_local/src/Constants.py`

 * *Files identical despite different names*

### Comparing `dialog_workflow_local-0.0.98/dialog_workflow_local/src/DialogWorkflow.py` & `dialog_workflow_local-0.0.99/dialog_workflow_local/src/DialogWorkflow.py`

 * *Files identical despite different names*

### Comparing `dialog_workflow_local-0.0.98/dialog_workflow_local/src/ProfileContext.py` & `dialog_workflow_local-0.0.99/dialog_workflow_local/src/ProfileContext.py`

 * *Files identical despite different names*

### Comparing `dialog_workflow_local-0.0.98/dialog_workflow_local/src/action.py` & `dialog_workflow_local-0.0.99/dialog_workflow_local/src/action.py`

 * *Files identical despite different names*

### Comparing `dialog_workflow_local-0.0.98/dialog_workflow_local/src/utils.py` & `dialog_workflow_local-0.0.99/dialog_workflow_local/src/utils.py`

 * *Files identical despite different names*

### Comparing `dialog_workflow_local-0.0.98/setup.py` & `dialog_workflow_local-0.0.99/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "dialog-workflow-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.98',  # https://pypi.org/project/dialog-workflow-local/
+    version='0.0.99',  # https://pypi.org/project/dialog-workflow-local/
     author="Circles",
     author_email="info@circle.life",
     description="PyPI Package for dialog workflow",
     long_description="This is a package for running the dialog workflow",
     long_description_content_type="text/markdown",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
```

