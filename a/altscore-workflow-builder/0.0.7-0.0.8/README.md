# Comparing `tmp/altscore_workflow_builder-0.0.7.tar.gz` & `tmp/altscore_workflow_builder-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "altscore_workflow_builder-0.0.7.tar", last modified: Fri May 10 19:53:52 2024, max compression
+gzip compressed data, was "altscore_workflow_builder-0.0.8.tar", last modified: Fri May 10 20:20:16 2024, max compression
```

## Comparing `altscore_workflow_builder-0.0.7.tar` & `altscore_workflow_builder-0.0.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:53:52.972760 altscore_workflow_builder-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-10 19:53:45.000000 altscore_workflow_builder-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-10 19:53:52.972760 altscore_workflow_builder-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-10 19:53:45.000000 altscore_workflow_builder-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 19:53:52.972760 altscore_workflow_builder-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-10 19:53:45.000000 altscore_workflow_builder-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:53:52.968760 altscore_workflow_builder-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:53:52.968760 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-10 19:53:45.000000 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/Home.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:53:45.000000 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-10 19:53:45.000000 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/launch_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:53:52.972760 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/pages/
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-10 19:53:45.000000 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/pages/Borrowers.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-10 19:53:45.000000 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/pages/Evaluators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-10 19:53:45.000000 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/pages/Packages.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-10 19:53:45.000000 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/pages/Rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-10 19:53:45.000000 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/pages/Workflow_Inspector.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:53:45.000000 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-05-10 19:53:45.000000 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/pages/workflow_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-10 19:53:45.000000 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-10 19:53:45.000000 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-10 19:53:45.000000 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:53:52.972760 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-10 19:53:52.000000 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-10 19:53:52.000000 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 19:53:52.000000 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-10 19:53:52.000000 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-10 19:53:52.000000 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-10 19:53:52.000000 altscore_workflow_builder-0.0.7/src/altscore_workflow_builder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:20:16.266027 altscore_workflow_builder-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-10 20:20:12.000000 altscore_workflow_builder-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-10 20:20:16.266027 altscore_workflow_builder-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-10 20:20:12.000000 altscore_workflow_builder-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 20:20:16.266027 altscore_workflow_builder-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-10 20:20:12.000000 altscore_workflow_builder-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:20:16.262027 altscore_workflow_builder-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:20:16.262027 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-10 20:20:12.000000 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/Home.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 20:20:12.000000 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-10 20:20:12.000000 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/launch_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:20:16.266027 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-10 20:20:12.000000 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/pages/Borrowers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-10 20:20:12.000000 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/pages/Evaluators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-10 20:20:12.000000 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/pages/Packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-10 20:20:12.000000 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/pages/Rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-10 20:20:12.000000 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/pages/Workflow_Inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-05-10 20:20:12.000000 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/pages/Workflow_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 20:20:12.000000 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-10 20:20:12.000000 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-10 20:20:12.000000 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-10 20:20:12.000000 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:20:16.266027 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-10 20:20:16.000000 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-10 20:20:16.000000 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 20:20:16.000000 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-10 20:20:16.000000 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-10 20:20:16.000000 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-10 20:20:16.000000 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder.egg-info/top_level.txt
```

### Comparing `altscore_workflow_builder-0.0.7/LICENSE` & `altscore_workflow_builder-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `altscore_workflow_builder-0.0.7/PKG-INFO` & `altscore_workflow_builder-0.0.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altscore-workflow-builder
-Version: 0.0.7
+Version: 0.0.8
 Summary: Streamlit-based workflow builder for AltScore
 Home-page: https://github.com/altscore/altscore-python
 Author: AltScore
 Author-email: developers@altscore.ai
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `altscore_workflow_builder-0.0.7/setup.py` & `altscore_workflow_builder-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 long_description = "Streamlit-based workflow builder for AltScore"
 
 setup(
     name="altscore-workflow-builder",
-    version="0.0.7",
+    version="0.0.8",
     description="Streamlit-based workflow builder for AltScore",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/altscore/altscore-python",
     author="AltScore",
```

### Comparing `altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/launch_app.py` & `altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/launch_app.py`

 * *Files identical despite different names*

### Comparing `altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/pages/Borrowers.py` & `altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/pages/Borrowers.py`

 * *Files identical despite different names*

### Comparing `altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/pages/Evaluators.py` & `altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/pages/Evaluators.py`

 * *Files identical despite different names*

### Comparing `altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/pages/Packages.py` & `altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/pages/Packages.py`

 * *Files identical despite different names*

### Comparing `altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/pages/Workflow_Inspector.py` & `altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/pages/Workflow_Inspector.py`

 * *Files identical despite different names*

### Comparing `altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/pages/workflow_builder.py` & `altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/pages/Workflow_builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import streamlit as st
 from altscore_workflow_builder.utils import list_workflows, load_workflow_definition, load_task_definitions, \
-    save_workflow_definition
+    save_workflow_definition, save_task_definitions, calculate_task_levels
 from altscore_workflow_builder.workflow import task_instance_dropdown, task_instance_graph
 from altscore_workflow_builder.task import task_graph
 from altscore_workflow_builder.utils import hide_deploy_button
 from streamlit_agraph import agraph, Node, Edge, Config
 import json
 
 st.set_page_config(layout="wide")
@@ -26,22 +26,24 @@
 solver_type = st.sidebar.selectbox("Physics Solver",
                                    ["barnesHut", "repulsion", "hierarchicalRepulsion", "forceAtlas2Based"])
 directed = st.sidebar.checkbox("Directed Graph", True)
 node_highlight = st.sidebar.checkbox("Highlight Nodes", True)
 collapsible = st.sidebar.checkbox("Collapsible Nodes", True)
 hierarchical_view = st.sidebar.checkbox("Hierarchical View", False)
 
-# Create nodes and edges for the agraph
+# Create nodes, edges, and levels for the agraph
 nodes = []
 edges = []
 task_nodes = flow_definition["task_instances"]
+levels = calculate_task_levels(task_nodes)
+all_task_names = list(task_nodes.keys())
 for task_name, task_info in task_nodes.items():
     task_details = task_definitions.get(task_info['type'], {})
     label = f"{task_name}\nInputs: {', '.join([inp['alias'] for inp in task_details.get('inputs', [])])}\nOutputs: {', '.join([out['alias'] for out in task_details.get('outputs', [])])}"
-    nodes.append(Node(id=task_name, label=label, color=node_color, size=30))
+    nodes.append(Node(id=task_name, label=label, color=node_color, size=30, y=levels[task_name] * 100))
 
 for task_name, task_info in task_nodes.items():
     if 'to' in task_info:
         for next_task in task_info['to']:
             edges.append(Edge(source=task_name, target=next_task, color=edge_color, type=edge_type))
 
 # Configuration for agraph
@@ -77,17 +79,25 @@
     input_json = st.sidebar.text_area("Inputs", value=json.dumps(task_details.get('inputs', []), indent=4))
     output_json = st.sidebar.text_area("Outputs", value=json.dumps(task_details.get('outputs', []), indent=4))
     input_override = st.sidebar.text_area("Input Override",
                                           value=json.dumps(task_info.get("input_override", {}), indent=4))
     input_conversion = st.sidebar.text_area("Input Conversion",
                                             value=json.dumps(task_info.get("input_conversion", {}), indent=4))
 
+    current_edges = task_nodes[selected_task].get("to", [])
+    new_edges = st.sidebar.multiselect("Select tasks that this task should point to:",
+                                       all_task_names,
+                                       default=current_edges)
+
+    # Display the task graph
     if st.sidebar.button("Save Changes"):
         try:
             task_details['inputs'] = json.loads(input_json)
             task_details['outputs'] = json.loads(output_json)
             task_info['input_override'] = json.loads(input_override)
             task_info['input_conversion'] = json.loads(input_conversion)
             save_workflow_definition(workflow['alias'], workflow['version'], flow_definition)
+            save_task_definitions(task_definitions)
             st.sidebar.success("Changes saved successfully!")
+            st.experimental_rerun()
         except json.JSONDecodeError:
             st.sidebar.error("Invalid JSON format. Please check your input.")
```

### Comparing `altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/utils.py` & `altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,14 +19,19 @@
 
 
 def load_task_definitions():
     with open(Path(config("PROJECT_ROOT")) / "app" / "tasks" / "task_definitions.json") as f:
         return json.load(f)
 
 
+def save_task_definitions(task_definitions):
+    with open(Path(config("PROJECT_ROOT")) / "app" / "tasks" / "task_definitions.json", "w") as f:
+        json.dump(task_definitions, f)
+
+
 def load_workflow_definition(workflow_alias: str, workflow_version: str):
     with open(Path(config(
             "PROJECT_ROOT")) / "app" / "workflows" / f"{workflow_alias}_{workflow_version}/flow_definition.json") as f:
         return json.load(f)
 
 
 def save_workflow_definition(workflow_alias: str, workflow_version: str, flow_definition: dict):
@@ -39,7 +44,29 @@
 def list_workflows():
     workflows = [f for f in os.listdir(Path(config("PROJECT_ROOT")) / "app" / "workflows") if
                  os.path.isdir(Path(config("PROJECT_ROOT")) / "app" / "workflows" / f)]
     return [
         {"alias": workflow.split("_")[0], "version": workflow.split("_")[-1], "label": workflow} for workflow in
         workflows
     ]
+
+
+def calculate_task_levels(task_nodes):
+    levels = {}
+    queue = []
+
+    # Start with tasks that have no incoming edges (sources)
+    sources = [task for task, details in task_nodes.items() if
+               all(task not in t.get("to", []) for t in task_nodes.values())]
+    for source in sources:
+        queue.append((source, 0))  # (task_name, level)
+
+    # BFS to assign levels
+    while queue:
+        current_task, current_level = queue.pop(0)
+        if current_task in levels:
+            continue
+        levels[current_task] = current_level
+        for next_task in task_nodes[current_task].get("to", []):
+            queue.append((next_task, current_level + 1))
+
+    return levels
```

### Comparing `altscore_workflow_builder-0.0.7/src/altscore_workflow_builder/workflow.py` & `altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/workflow.py`

 * *Files identical despite different names*

### Comparing `altscore_workflow_builder-0.0.7/src/altscore_workflow_builder.egg-info/PKG-INFO` & `altscore_workflow_builder-0.0.8/src/altscore_workflow_builder.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altscore-workflow-builder
-Version: 0.0.7
+Version: 0.0.8
 Summary: Streamlit-based workflow builder for AltScore
 Home-page: https://github.com/altscore/altscore-python
 Author: AltScore
 Author-email: developers@altscore.ai
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `altscore_workflow_builder-0.0.7/src/altscore_workflow_builder.egg-info/SOURCES.txt` & `altscore_workflow_builder-0.0.8/src/altscore_workflow_builder.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,9 +14,9 @@
 src/altscore_workflow_builder.egg-info/requires.txt
 src/altscore_workflow_builder.egg-info/top_level.txt
 src/altscore_workflow_builder/pages/Borrowers.py
 src/altscore_workflow_builder/pages/Evaluators.py
 src/altscore_workflow_builder/pages/Packages.py
 src/altscore_workflow_builder/pages/Rules.py
 src/altscore_workflow_builder/pages/Workflow_Inspector.py
-src/altscore_workflow_builder/pages/__init__.py
-src/altscore_workflow_builder/pages/workflow_builder.py
+src/altscore_workflow_builder/pages/Workflow_builder.py
+src/altscore_workflow_builder/pages/__init__.py
```

