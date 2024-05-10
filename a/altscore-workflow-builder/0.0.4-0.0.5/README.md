# Comparing `tmp/altscore_workflow_builder-0.0.4.tar.gz` & `tmp/altscore_workflow_builder-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "altscore_workflow_builder-0.0.4.tar", last modified: Fri May 10 19:35:49 2024, max compression
+gzip compressed data, was "altscore_workflow_builder-0.0.5.tar", last modified: Fri May 10 19:46:00 2024, max compression
```

## Comparing `altscore_workflow_builder-0.0.4.tar` & `altscore_workflow_builder-0.0.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:35:49.638885 altscore_workflow_builder-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-10 19:35:45.000000 altscore_workflow_builder-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-10 19:35:49.638885 altscore_workflow_builder-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-10 19:35:45.000000 altscore_workflow_builder-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 19:35:49.638885 altscore_workflow_builder-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-10 19:35:45.000000 altscore_workflow_builder-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:35:49.634885 altscore_workflow_builder-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:35:49.638885 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-10 19:35:45.000000 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/Home.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:35:45.000000 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-10 19:35:45.000000 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/launch_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:35:49.638885 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/pages/
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-10 19:35:45.000000 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/pages/Borrowers.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-10 19:35:45.000000 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/pages/Evaluators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-10 19:35:45.000000 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/pages/Packages.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-10 19:35:45.000000 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/pages/Rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-10 19:35:45.000000 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/pages/Workflow_Inspector.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:35:45.000000 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-05-10 19:35:45.000000 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/pages/workflow_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-10 19:35:45.000000 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-10 19:35:45.000000 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-10 19:35:45.000000 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:35:49.638885 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-10 19:35:49.000000 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-10 19:35:49.000000 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 19:35:49.000000 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-10 19:35:49.000000 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-10 19:35:49.000000 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-10 19:35:49.000000 altscore_workflow_builder-0.0.4/src/altscore_workflow_builder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:46:00.482757 altscore_workflow_builder-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-10 19:45:56.000000 altscore_workflow_builder-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-10 19:46:00.482757 altscore_workflow_builder-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-10 19:45:56.000000 altscore_workflow_builder-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 19:46:00.482757 altscore_workflow_builder-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-10 19:45:56.000000 altscore_workflow_builder-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:46:00.478757 altscore_workflow_builder-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:46:00.478757 altscore_workflow_builder-0.0.5/src/altscore_workflow_builder/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-10 19:45:56.000000 altscore_workflow_builder-0.0.5/src/altscore_workflow_builder/Home.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:45:56.000000 altscore_workflow_builder-0.0.5/src/altscore_workflow_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-10 19:45:56.000000 altscore_workflow_builder-0.0.5/src/altscore_workflow_builder/launch_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:46:00.482757 altscore_workflow_builder-0.0.5/src/altscore_workflow_builder/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-10 19:45:56.000000 altscore_workflow_builder-0.0.5/src/altscore_workflow_builder/pages/Borrowers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-10 19:45:56.000000 altscore_workflow_builder-0.0.5/src/altscore_workflow_builder/pages/Evaluators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-10 19:45:56.000000 altscore_workflow_builder-0.0.5/src/altscore_workflow_builder/pages/Packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-10 19:45:56.000000 altscore_workflow_builder-0.0.5/src/altscore_workflow_builder/pages/Rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-10 19:45:56.000000 altscore_workflow_builder-0.0.5/src/altscore_workflow_builder/pages/Workflow_Inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:45:56.000000 altscore_workflow_builder-0.0.5/src/altscore_workflow_builder/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-05-10 19:45:56.000000 altscore_workflow_builder-0.0.5/src/altscore_workflow_builder/pages/workflow_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-10 19:45:56.000000 altscore_workflow_builder-0.0.5/src/altscore_workflow_builder/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-10 19:45:56.000000 altscore_workflow_builder-0.0.5/src/altscore_workflow_builder/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-10 19:45:56.000000 altscore_workflow_builder-0.0.5/src/altscore_workflow_builder/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:46:00.482757 altscore_workflow_builder-0.0.5/src/altscore_workflow_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-10 19:46:00.000000 altscore_workflow_builder-0.0.5/src/altscore_workflow_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-10 19:46:00.000000 altscore_workflow_builder-0.0.5/src/altscore_workflow_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 19:46:00.000000 altscore_workflow_builder-0.0.5/src/altscore_workflow_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-10 19:46:00.000000 altscore_workflow_builder-0.0.5/src/altscore_workflow_builder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-10 19:46:00.000000 altscore_workflow_builder-0.0.5/src/altscore_workflow_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-10 19:46:00.000000 altscore_workflow_builder-0.0.5/src/altscore_workflow_builder.egg-info/top_level.txt
```

### Comparing `altscore_workflow_builder-0.0.4/LICENSE` & `altscore_workflow_builder-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `altscore_workflow_builder-0.0.4/PKG-INFO` & `altscore_workflow_builder-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altscore-workflow-builder
-Version: 0.0.4
+Version: 0.0.5
 Summary: Streamlit-based workflow builder for AltScore
 Home-page: https://github.com/altscore/altscore-python
 Author: AltScore
 Author-email: developers@altscore.ai
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -20,9 +20,10 @@
 Requires-Dist: httpx
 Requires-Dist: stringcase
 Requires-Dist: python-decouple
 Requires-Dist: python-dateutil==2.8.2
 Requires-Dist: pyjwt
 Requires-Dist: altscore
 Requires-Dist: streamlit
+Requires-Dist: streamlit-agraph
 
 Streamlit-based workflow builder for AltScore
```

### Comparing `altscore_workflow_builder-0.0.4/setup.py` & `altscore_workflow_builder-0.0.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 long_description = "Streamlit-based workflow builder for AltScore"
 
 setup(
     name="altscore-workflow-builder",
-    version="0.0.4",
+    version="0.0.5",
     description="Streamlit-based workflow builder for AltScore",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/altscore/altscore-python",
     author="AltScore",
@@ -33,11 +33,12 @@
         "httpx",
         "stringcase",
         "python-decouple",
         "python-dateutil==2.8.2",
         "pyjwt",
         "altscore",
         "streamlit",
+        "streamlit-agraph",
     ],
     extras_require={},
     python_requires=">=3.8",
 )
```

### Comparing `altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/launch_app.py` & `altscore_workflow_builder-0.0.5/src/altscore_workflow_builder/launch_app.py`

 * *Files identical despite different names*

### Comparing `altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/pages/Borrowers.py` & `altscore_workflow_builder-0.0.5/src/altscore_workflow_builder/pages/Borrowers.py`

 * *Files identical despite different names*

### Comparing `altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/pages/Evaluators.py` & `altscore_workflow_builder-0.0.5/src/altscore_workflow_builder/pages/Evaluators.py`

 * *Files identical despite different names*

### Comparing `altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/pages/Packages.py` & `altscore_workflow_builder-0.0.5/src/altscore_workflow_builder/pages/Packages.py`

 * *Files identical despite different names*

### Comparing `altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/pages/Workflow_Inspector.py` & `altscore_workflow_builder-0.0.5/src/altscore_workflow_builder/pages/Workflow_Inspector.py`

 * *Files identical despite different names*

### Comparing `altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/pages/workflow_builder.py` & `altscore_workflow_builder-0.0.5/src/altscore_workflow_builder/pages/workflow_builder.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
     save_workflow_definition
 from altscore_workflow_builder.workflow import task_instance_dropdown, task_instance_graph
 from altscore_workflow_builder.task import task_graph
 from altscore_workflow_builder.utils import hide_deploy_button
 from streamlit_agraph import agraph, Node, Edge, Config
 import json
 
+st.set_page_config(layout="wide")
 hide_deploy_button()
 st.title("Workflow Inspector")
-st.set_page_config(layout="wide")
 st.sidebar.header("Graph Configuration")
 workflow = st.sidebar.selectbox("Select Workflow", list_workflows())
 flow_definition = load_workflow_definition(workflow['alias'], workflow['version'])
 task_definitions = load_task_definitions()
 
 # Configurable parameters in the sidebar
 graph_height = st.sidebar.number_input("Height", min_value=500, max_value=1500, value=750)
```

### Comparing `altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/utils.py` & `altscore_workflow_builder-0.0.5/src/altscore_workflow_builder/utils.py`

 * *Files identical despite different names*

### Comparing `altscore_workflow_builder-0.0.4/src/altscore_workflow_builder/workflow.py` & `altscore_workflow_builder-0.0.5/src/altscore_workflow_builder/workflow.py`

 * *Files identical despite different names*

### Comparing `altscore_workflow_builder-0.0.4/src/altscore_workflow_builder.egg-info/PKG-INFO` & `altscore_workflow_builder-0.0.5/src/altscore_workflow_builder.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altscore-workflow-builder
-Version: 0.0.4
+Version: 0.0.5
 Summary: Streamlit-based workflow builder for AltScore
 Home-page: https://github.com/altscore/altscore-python
 Author: AltScore
 Author-email: developers@altscore.ai
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -20,9 +20,10 @@
 Requires-Dist: httpx
 Requires-Dist: stringcase
 Requires-Dist: python-decouple
 Requires-Dist: python-dateutil==2.8.2
 Requires-Dist: pyjwt
 Requires-Dist: altscore
 Requires-Dist: streamlit
+Requires-Dist: streamlit-agraph
 
 Streamlit-based workflow builder for AltScore
```

### Comparing `altscore_workflow_builder-0.0.4/src/altscore_workflow_builder.egg-info/SOURCES.txt` & `altscore_workflow_builder-0.0.5/src/altscore_workflow_builder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

