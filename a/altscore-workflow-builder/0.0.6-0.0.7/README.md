# Comparing `tmp/altscore_workflow_builder-0.0.6.tar.gz` & `tmp/altscore_workflow_builder-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "altscore_workflow_builder-0.0.6.tar", last modified: Fri May 10 19:50:35 2024, max compression
+gzip compressed data, was "altscore_workflow_builder-0.0.7.tar", last modified: Fri May 10 19:53:52 2024, max compression
```

## Comparing `altscore_workflow_builder-0.0.6.tar` & `altscore_workflow_builder-0.0.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:50:35.807712 altscore_workflow_builder-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-10 19:50:31.000000 altscore_workflow_builder-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-10 19:50:35.807712 altscore_workflow_builder-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-10 19:50:31.000000 altscore_workflow_builder-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 19:50:35.807712 altscore_workflow_builder-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-10 19:50:31.000000 altscore_workflow_builder-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:50:35.803712 altscore_workflow_builder-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:50:35.803712 altscore_workflow_builder-0.0.6/src/altscore_workflow_builder/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-10 19:50:31.000000 altscore_workflow_builder-0.0.6/src/altscore_workflow_builder/Home.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:50:31.000000 altscore_workflow_builder-0.0.6/src/altscore_workflow_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-10 19:50:31.000000 altscore_workflow_builder-0.0.6/src/altscore_workflow_builder/launch_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:50:35.807712 altscore_workflow_builder-0.0.6/src/altscore_workflow_builder/pages/
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-10 19:50:31.000000 altscore_workflow_builder-0.0.6/src/altscore_workflow_builder/pages/Borrowers.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-10 19:50:31.000000 altscore_workflow_builder-0.0.6/src/altscore_workflow_builder/pages/Evaluators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-10 19:50:31.000000 altscore_workflow_builder-0.0.6/src/altscore_workflow_builder/pages/Packages.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-10 19:50:31.000000 altscore_workflow_builder-0.0.6/src/altscore_workflow_builder/pages/Rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-10 19:50:31.000000 altscore_workflow_builder-0.0.6/src/altscore_workflow_builder/pages/Workflow_Inspector.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:50:31.000000 altscore_workflow_builder-0.0.6/src/altscore_workflow_builder/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-05-10 19:50:31.000000 altscore_workflow_builder-0.0.6/src/altscore_workflow_builder/pages/workflow_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-10 19:50:31.000000 altscore_workflow_builder-0.0.6/src/altscore_workflow_builder/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-10 19:50:31.000000 altscore_workflow_builder-0.0.6/src/altscore_workflow_builder/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-10 19:50:31.000000 altscore_workflow_builder-0.0.6/src/altscore_workflow_builder/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:50:35.807712 altscore_workflow_builder-0.0.6/src/altscore_workflow_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-10 19:50:35.000000 altscore_workflow_builder-0.0.6/src/altscore_workflow_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-10 19:50:35.000000 altscore_workflow_builder-0.0.6/src/altscore_workflow_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 19:50:35.000000 altscore_workflow_builder-0.0.6/src/altscore_workflow_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-10 19:50:35.000000 altscore_workflow_builder-0.0.6/src/altscore_workflow_builder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-10 19:50:35.000000 altscore_workflow_builder-0.0.6/src/altscore_workflow_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-10 19:50:35.000000 altscore_workflow_builder-0.0.6/src/altscore_workflow_builder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:53:52.972760 altscore_workflow_builder-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-10 19:53:45.000000 altscore_workflow_builder-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-10 19:53:52.972760 altscore_workflow_builder-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-10 19:53:45.000000 altscore_workflow_builder-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 19:53:52.972760 altscore_workflow_builder-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-10 19:53:45.000000 altscore_workflow_builder-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:53:52.968760 altscore_workflow_builder-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:53:52.968760 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-10 19:53:45.000000 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/Home.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:53:45.000000 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-10 19:53:45.000000 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/launch_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:53:52.972760 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-10 19:53:45.000000 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/pages/Borrowers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-10 19:53:45.000000 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/pages/Evaluators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-10 19:53:45.000000 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/pages/Packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-10 19:53:45.000000 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/pages/Rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-10 19:53:45.000000 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/pages/Workflow_Inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:53:45.000000 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-05-10 19:53:45.000000 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/pages/workflow_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-10 19:53:45.000000 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-10 19:53:45.000000 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-10 19:53:45.000000 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:53:52.972760 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-10 19:53:52.000000 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-10 19:53:52.000000 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 19:53:52.000000 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-10 19:53:52.000000 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-10 19:53:52.000000 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-10 19:53:52.000000 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder.egg-info/top_level.txt
```

### Comparing `altscore_workflow_builder-0.0.6/LICENSE` & `altscore_workflow_builder-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `altscore_workflow_builder-0.0.6/PKG-INFO` & `altscore_workflow_builder-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altscore-workflow-builder
-Version: 0.0.6
+Version: 0.0.7
 Summary: Streamlit-based workflow builder for AltScore
 Home-page: https://github.com/altscore/altscore-python
 Author: AltScore
 Author-email: developers@altscore.ai
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `altscore_workflow_builder-0.0.6/setup.py` & `altscore_workflow_builder-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 long_description = "Streamlit-based workflow builder for AltScore"
 
 setup(
     name="altscore-workflow-builder",
-    version="0.0.6",
+    version="0.0.7",
     description="Streamlit-based workflow builder for AltScore",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/altscore/altscore-python",
     author="AltScore",
```

### Comparing `altscore_workflow_builder-0.0.6/src/altscore_workflow_builder/launch_app.py` & `altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/launch_app.py`

 * *Files identical despite different names*

### Comparing `altscore_workflow_builder-0.0.6/src/altscore_workflow_builder/pages/Borrowers.py` & `altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/pages/Borrowers.py`

 * *Files identical despite different names*

### Comparing `altscore_workflow_builder-0.0.6/src/altscore_workflow_builder/pages/Evaluators.py` & `altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/pages/Evaluators.py`

 * *Files identical despite different names*

### Comparing `altscore_workflow_builder-0.0.6/src/altscore_workflow_builder/pages/Packages.py` & `altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/pages/Packages.py`

 * *Files identical despite different names*

### Comparing `altscore_workflow_builder-0.0.6/src/altscore_workflow_builder/pages/Workflow_Inspector.py` & `altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/pages/Workflow_Inspector.py`

 * *Files identical despite different names*

### Comparing `altscore_workflow_builder-0.0.6/src/altscore_workflow_builder/pages/workflow_builder.py` & `altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/pages/workflow_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 st.sidebar.header("Graph Configuration")
 workflow = st.sidebar.selectbox("Select Workflow", list_workflows())
 flow_definition = load_workflow_definition(workflow['alias'], workflow['version'])
 task_definitions = load_task_definitions()
 
 # Configurable parameters in the sidebar
 graph_height = st.sidebar.number_input("Height", min_value=500, max_value=1500, value=750)
-graph_width = st.sidebar.number_input("Width", value="100%")
 background_color = st.sidebar.color_picker("Background Color", '#ffffff')
 font_size = st.sidebar.slider("Font Size", 10, 20, 14)
 node_color = st.sidebar.color_picker("Node Color", '#88c999')
 edge_color = st.sidebar.color_picker("Edge Color", '#000000')
 edge_type = st.sidebar.selectbox("Edge Type", ["STRAIGHT", "CURVE_SMOOTH", "CURVE_FULL"])
 physics_enabled = st.sidebar.checkbox("Enable Physics", True)
 solver_type = st.sidebar.selectbox("Physics Solver",
```

### Comparing `altscore_workflow_builder-0.0.6/src/altscore_workflow_builder/utils.py` & `altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/utils.py`

 * *Files identical despite different names*

### Comparing `altscore_workflow_builder-0.0.6/src/altscore_workflow_builder/workflow.py` & `altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/workflow.py`

 * *Files identical despite different names*

### Comparing `altscore_workflow_builder-0.0.6/src/altscore_workflow_builder.egg-info/PKG-INFO` & `altscore_workflow_builder-0.0.7/src/altscore_workflow_builder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altscore-workflow-builder
-Version: 0.0.6
+Version: 0.0.7
 Summary: Streamlit-based workflow builder for AltScore
 Home-page: https://github.com/altscore/altscore-python
 Author: AltScore
 Author-email: developers@altscore.ai
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `altscore_workflow_builder-0.0.6/src/altscore_workflow_builder.egg-info/SOURCES.txt` & `altscore_workflow_builder-0.0.7/src/altscore_workflow_builder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

