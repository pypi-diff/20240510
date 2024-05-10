# Comparing `tmp/altscore_workflow_builder-0.0.3.tar.gz` & `tmp/altscore_workflow_builder-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "altscore_workflow_builder-0.0.3.tar", last modified: Sun Apr 28 13:59:43 2024, max compression
+gzip compressed data, was "altscore_workflow_builder-0.0.4.tar", last modified: Fri May 10 19:35:49 2024, max compression
```

## Comparing `altscore_workflow_builder-0.0.3.tar` & `altscore_workflow_builder-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 13:59:43.548347 altscore_workflow_builder-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-28 13:59:39.000000 altscore_workflow_builder-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-28 13:59:43.548347 altscore_workflow_builder-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-28 13:59:39.000000 altscore_workflow_builder-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 13:59:43.548347 altscore_workflow_builder-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-28 13:59:39.000000 altscore_workflow_builder-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 13:59:43.544347 altscore_workflow_builder-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 13:59:43.544347 altscore_workflow_builder-0.0.3/src/altscore_workflow_builder/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-28 13:59:39.000000 altscore_workflow_builder-0.0.3/src/altscore_workflow_builder/Home.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 13:59:39.000000 altscore_workflow_builder-0.0.3/src/altscore_workflow_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-28 13:59:39.000000 altscore_workflow_builder-0.0.3/src/altscore_workflow_builder/launch_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 13:59:43.548347 altscore_workflow_builder-0.0.3/src/altscore_workflow_builder/pages/
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-28 13:59:39.000000 altscore_workflow_builder-0.0.3/src/altscore_workflow_builder/pages/Borrowers.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-28 13:59:39.000000 altscore_workflow_builder-0.0.3/src/altscore_workflow_builder/pages/Evaluators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-28 13:59:39.000000 altscore_workflow_builder-0.0.3/src/altscore_workflow_builder/pages/Packages.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-28 13:59:39.000000 altscore_workflow_builder-0.0.3/src/altscore_workflow_builder/pages/Rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-28 13:59:39.000000 altscore_workflow_builder-0.0.3/src/altscore_workflow_builder/pages/Workflow_Inspector.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 13:59:39.000000 altscore_workflow_builder-0.0.3/src/altscore_workflow_builder/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-28 13:59:39.000000 altscore_workflow_builder-0.0.3/src/altscore_workflow_builder/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-28 13:59:39.000000 altscore_workflow_builder-0.0.3/src/altscore_workflow_builder/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-28 13:59:39.000000 altscore_workflow_builder-0.0.3/src/altscore_workflow_builder/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 13:59:43.548347 altscore_workflow_builder-0.0.3/src/altscore_workflow_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-28 13:59:43.000000 altscore_workflow_builder-0.0.3/src/altscore_workflow_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-28 13:59:43.000000 altscore_workflow_builder-0.0.3/src/altscore_workflow_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 13:59:43.000000 altscore_workflow_builder-0.0.3/src/altscore_workflow_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-28 13:59:43.000000 altscore_workflow_builder-0.0.3/src/altscore_workflow_builder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-28 13:59:43.000000 altscore_workflow_builder-0.0.3/src/altscore_workflow_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-28 13:59:43.000000 altscore_workflow_builder-0.0.3/src/altscore_workflow_builder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:35:49.638885 altscore_workflow_builder-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-10 19:35:45.000000 altscore_workflow_builder-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-10 19:35:49.638885 altscore_workflow_builder-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-10 19:35:45.000000 altscore_workflow_builder-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 19:35:49.638885 altscore_workflow_builder-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-10 19:35:45.000000 altscore_workflow_builder-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:35:49.634885 altscore_workflow_builder-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:35:49.638885 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-10 19:35:45.000000 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/Home.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:35:45.000000 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-10 19:35:45.000000 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/launch_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:35:49.638885 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-10 19:35:45.000000 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/pages/Borrowers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-10 19:35:45.000000 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/pages/Evaluators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-10 19:35:45.000000 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/pages/Packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-10 19:35:45.000000 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/pages/Rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-10 19:35:45.000000 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/pages/Workflow_Inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:35:45.000000 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-05-10 19:35:45.000000 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/pages/workflow_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-10 19:35:45.000000 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-10 19:35:45.000000 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-10 19:35:45.000000 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:35:49.638885 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-10 19:35:49.000000 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-10 19:35:49.000000 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 19:35:49.000000 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-10 19:35:49.000000 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-10 19:35:49.000000 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-10 19:35:49.000000 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder.egg-info/top_level.txt
```

### Comparing `altscore_workflow_builder-0.0.3/LICENSE` & `altscore_workflow_builder-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `altscore_workflow_builder-0.0.3/PKG-INFO` & `altscore_workflow_builder-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altscore-workflow-builder
-Version: 0.0.3
+Version: 0.0.4
 Summary: Streamlit-based workflow builder for AltScore
 Home-page: https://github.com/altscore/altscore-python
 Author: AltScore
 Author-email: developers@altscore.ai
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `altscore_workflow_builder-0.0.3/setup.py` & `altscore_workflow_builder-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 long_description = "Streamlit-based workflow builder for AltScore"
 
 setup(
     name="altscore-workflow-builder",
-    version="0.0.3",
+    version="0.0.4",
     description="Streamlit-based workflow builder for AltScore",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/altscore/altscore-python",
     author="AltScore",
```

### Comparing `altscore_workflow_builder-0.0.3/src/altscore_workflow_builder/launch_app.py` & `altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/launch_app.py`

 * *Files identical despite different names*

### Comparing `altscore_workflow_builder-0.0.3/src/altscore_workflow_builder/pages/Borrowers.py` & `altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/pages/Borrowers.py`

 * *Files identical despite different names*

### Comparing `altscore_workflow_builder-0.0.3/src/altscore_workflow_builder/pages/Evaluators.py` & `altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/pages/Evaluators.py`

 * *Files identical despite different names*

### Comparing `altscore_workflow_builder-0.0.3/src/altscore_workflow_builder/pages/Packages.py` & `altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/pages/Packages.py`

 * *Files identical despite different names*

### Comparing `altscore_workflow_builder-0.0.3/src/altscore_workflow_builder/pages/Workflow_Inspector.py` & `altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/pages/Workflow_Inspector.py`

 * *Files identical despite different names*

### Comparing `altscore_workflow_builder-0.0.3/src/altscore_workflow_builder/utils.py` & `altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,23 +25,21 @@
 
 def load_workflow_definition(workflow_alias: str, workflow_version: str):
     with open(Path(config(
             "PROJECT_ROOT")) / "app" / "workflows" / f"{workflow_alias}_{workflow_version}/flow_definition.json") as f:
         return json.load(f)
 
 
-def get_alias_and_version(workflow_path: str) -> dict:
-    version = workflow_path.split("_")[-1]
-    alias = workflow_path[0:workflow_path.index(version) - 1]
-    return {
-        "alias": alias,
-        "version": version,
-        "label": workflow_path
-    }
+def save_workflow_definition(workflow_alias: str, workflow_version: str, flow_definition: dict):
+    with open(Path(config(
+            "PROJECT_ROOT")) / "app" / "workflows" / f"{workflow_alias}_{workflow_version}/flow_definition.json",
+              "w") as f:
+        json.dump(flow_definition, f)
 
 
 def list_workflows():
     workflows = [f for f in os.listdir(Path(config("PROJECT_ROOT")) / "app" / "workflows") if
                  os.path.isdir(Path(config("PROJECT_ROOT")) / "app" / "workflows" / f)]
     return [
-        get_alias_and_version(workflow) for workflow in workflows
+        {"alias": workflow.split("_")[0], "version": workflow.split("_")[-1], "label": workflow} for workflow in
+        workflows
     ]
```

### Comparing `altscore_workflow_builder-0.0.3/src/altscore_workflow_builder/workflow.py` & `altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/workflow.py`

 * *Files identical despite different names*

### Comparing `altscore_workflow_builder-0.0.3/src/altscore_workflow_builder.egg-info/PKG-INFO` & `altscore_workflow_builder-0.0.4/src/altscore_workflow_builder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altscore-workflow-builder
-Version: 0.0.3
+Version: 0.0.4
 Summary: Streamlit-based workflow builder for AltScore
 Home-page: https://github.com/altscore/altscore-python
 Author: AltScore
 Author-email: developers@altscore.ai
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `altscore_workflow_builder-0.0.3/src/altscore_workflow_builder.egg-info/SOURCES.txt` & `altscore_workflow_builder-0.0.4/src/altscore_workflow_builder.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -14,8 +14,9 @@
 src/altscore_workflow_builder.egg-info/requires.txt
 src/altscore_workflow_builder.egg-info/top_level.txt
 src/altscore_workflow_builder/pages/Borrowers.py
 src/altscore_workflow_builder/pages/Evaluators.py
 src/altscore_workflow_builder/pages/Packages.py
 src/altscore_workflow_builder/pages/Rules.py
 src/altscore_workflow_builder/pages/Workflow_Inspector.py
-src/altscore_workflow_builder/pages/__init__.py
+src/altscore_workflow_builder/pages/__init__.py
+src/altscore_workflow_builder/pages/workflow_builder.py
```

