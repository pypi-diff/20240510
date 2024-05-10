# Comparing `tmp/jobspec-0.1.1.tar.gz` & `tmp/jobspec-0.1.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jobspec-0.1.1.tar", last modified: Sun May  5 18:39:17 2024, max compression
+gzip compressed data, was "jobspec-0.1.11.tar", last modified: Fri May 10 06:00:37 2024, max compression
```

## Comparing `jobspec-0.1.1.tar` & `jobspec-0.1.11.tar`

### file list

```diff
@@ -1,50 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:39:17.479181 jobspec-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-05 18:38:50.000000 jobspec-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-05 18:38:50.000000 jobspec-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-05 18:38:50.000000 jobspec-0.1.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-05 18:39:17.479181 jobspec-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-05 18:38:50.000000 jobspec-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:39:17.475181 jobspec-0.1.1/jobspec/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:39:17.479181 jobspec-0.1.1/jobspec/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/cli/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:39:17.479181 jobspec-0.1.1/jobspec/core/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/core/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/core/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/core/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/core/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:39:17.479181 jobspec-0.1.1/jobspec/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/plugin/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     7192 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:39:17.479181 jobspec-0.1.1/jobspec/steps/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/steps/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/steps/empty.py
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/steps/fileio.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/steps/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:39:17.479181 jobspec-0.1.1/jobspec/transformer/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/transformer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:39:17.479181 jobspec-0.1.1/jobspec/transformer/flux/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/transformer/flux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8507 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/transformer/flux/steps.py
--rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/transformer/flux/workload.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/transformer/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:39:17.475181 jobspec-0.1.1/jobspec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-05 18:39:17.000000 jobspec-0.1.1/jobspec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-05 18:39:17.000000 jobspec-0.1.1/jobspec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 18:39:17.000000 jobspec-0.1.1/jobspec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-05 18:39:17.000000 jobspec-0.1.1/jobspec.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 18:39:17.000000 jobspec-0.1.1/jobspec.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-05 18:39:17.000000 jobspec-0.1.1/jobspec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-05 18:39:17.000000 jobspec-0.1.1/jobspec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-05 18:38:50.000000 jobspec-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-05 18:39:17.479181 jobspec-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-05-05 18:38:50.000000 jobspec-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:00:37.473936 jobspec-0.1.11/
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-10 06:00:21.000000 jobspec-0.1.11/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-10 06:00:21.000000 jobspec-0.1.11/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-10 06:00:21.000000 jobspec-0.1.11/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-10 06:00:37.473936 jobspec-0.1.11/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-10 06:00:21.000000 jobspec-0.1.11/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:00:37.469936 jobspec-0.1.11/jobspec/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:00:37.469936 jobspec-0.1.11/jobspec/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/cli/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:00:37.469936 jobspec-0.1.11/jobspec/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/core/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/core/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:00:37.469936 jobspec-0.1.11/jobspec/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/plugin/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:00:37.469936 jobspec-0.1.11/jobspec/steps/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/steps/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/steps/empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/steps/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/steps/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:00:37.473936 jobspec-0.1.11/jobspec/transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/transformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:00:37.473936 jobspec-0.1.11/jobspec/transformer/flux/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/transformer/flux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8592 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/transformer/flux/steps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/transformer/flux/workload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/transformer/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:00:37.473936 jobspec-0.1.11/jobspec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-10 06:00:37.000000 jobspec-0.1.11/jobspec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-10 06:00:37.000000 jobspec-0.1.11/jobspec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 06:00:37.000000 jobspec-0.1.11/jobspec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-10 06:00:37.000000 jobspec-0.1.11/jobspec.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 06:00:37.000000 jobspec-0.1.11/jobspec.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-10 06:00:37.000000 jobspec-0.1.11/jobspec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-10 06:00:37.000000 jobspec-0.1.11/jobspec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-10 06:00:21.000000 jobspec-0.1.11/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-10 06:00:37.473936 jobspec-0.1.11/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-05-10 06:00:21.000000 jobspec-0.1.11/setup.py
```

### Comparing `jobspec-0.1.1/LICENSE` & `jobspec-0.1.11/LICENSE`

 * *Files identical despite different names*

### Comparing `jobspec-0.1.1/NOTICE` & `jobspec-0.1.11/NOTICE`

 * *Files identical despite different names*

### Comparing `jobspec-0.1.1/PKG-INFO` & `jobspec-0.1.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jobspec
-Version: 0.1.1
+Version: 0.1.11
 Summary: Jobspec specification and translation layer for cluster work
 Home-page: https://github.com/compspec/jobspec
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: cluster,orchestration,transformer,jobspec,flux
```

### Comparing `jobspec-0.1.1/README.md` & `jobspec-0.1.11/README.md`

 * *Files identical despite different names*

### Comparing `jobspec-0.1.1/jobspec/cli/__init__.py` & `jobspec-0.1.11/jobspec/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `jobspec-0.1.1/jobspec/cli/run.py` & `jobspec-0.1.11/jobspec/cli/run.py`

 * *Files identical despite different names*

### Comparing `jobspec-0.1.1/jobspec/core/base.py` & `jobspec-0.1.11/jobspec/core/base.py`

 * *Files identical despite different names*

### Comparing `jobspec-0.1.1/jobspec/core/core.py` & `jobspec-0.1.11/jobspec/core/core.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+import copy
+
 import jsonschema
 
 import jobspec.schema as schema
 
 from .base import ResourceBase
-from .resources import find_resources
+from .resources import find_resources, to_jobspec
 
 
 class Jobspec(ResourceBase):
     def __init__(self, filename, validate=True, schema=schema.jobspec_nextgen):
         """
         Load in and validate a Jobspec
         """
@@ -47,14 +49,34 @@
         slot = slot or self.slot
 
         # Traverse each section. There is usually only one I guess
         flat = {}
         find_resources(flat, self.data, slot)
         return flat
 
+    def to_jobspec(self, slot_name):
+        """
+        Turn the resource into a flux jobspec
+
+        Note this is not currently used - it was too error prone
+        """
+        slot = self.slot or {}
+        label = slot_name or (slot.get("label") or "default")
+
+        # Hold onto the original data so it is not mangled
+        js = copy.deepcopy(self.data)
+
+        # Traverse each section and convert to flux jobspec
+        has_slot = to_jobspec(js, slot_name=label)
+
+        # If we don't have a slot, we have to make a fake one at the top
+        if not has_slot:
+            js = {"type": "slot", "count": 1, "label": label, "with": [js]}
+        return js
+
 
 class Attributes(ResourceBase):
     """
     Job attributes, not formally defined yet.
     """
 
     pass
```

### Comparing `jobspec-0.1.1/jobspec/logger.py` & `jobspec-0.1.11/jobspec/logger.py`

 * *Files identical despite different names*

### Comparing `jobspec-0.1.1/jobspec/plugin/registry.py` & `jobspec-0.1.11/jobspec/plugin/registry.py`

 * *Files identical despite different names*

### Comparing `jobspec-0.1.1/jobspec/runner.py` & `jobspec-0.1.11/jobspec/runner.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os
 
 # This imports the latest version
 import jobspec.core as js
-import jobspec.defaults as defaults
 import jobspec.steps.runner as step_runner
 
 
 class TransformerBase:
     """
     A Transformer base is the core of a JobSpec
 
@@ -34,30 +33,14 @@
         """
         # Allow registering an empty step if needed
         # An empty step does nothing, an explicit declaration
         # by the transformer developer it's not needed, etc.
         name = name or step.name
         cls.steps[name] = step
 
-    def update_settings(self, settings, typ, step):
-        """
-        Update settings, either set or unset
-        """
-        if "name" not in step or "value" not in step:
-            return
-        if not step["key"]:
-            return
-        # This is important for typos, etc.
-        if step["key"] not in defaults.valid_settings:
-            raise ValueError(f"{step['key']} is not a known setting.")
-        if typ == "set":
-            settings[step["key"]] = step["value"]
-        elif typ == "unset" and step["key"] in settings:
-            del settings[step["key"]]
-
     def parse(self, jobspec):
         """
         parse validates logic and returns a series of steps, which
         will depend on the underlying transformer. It might be:
 
         - a batch that includes logic to write a script and then run it
         - one or more submit commands
```

### Comparing `jobspec-0.1.1/jobspec/schema.py` & `jobspec-0.1.11/jobspec/schema.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,52 +12,59 @@
         "name": {"type": "string"},
         # This is not a flux JobSpec, and we start at v1
         "version": {
             "description": "the jobspec version",
             "type": "integer",
             "enum": [1],
         },
-        # These are optional global resources
-        "requires": {"$ref": "#/definitions/requires"},
-        # Resources at the top level are key (identifier) and value (resource) pairs
         "resources": {
             "type": "object",
             "patternProperties": {
                 "^([a-z]|[|]|&|[0-9]+)+$": {"$ref": "#/definitions/resources"},
             },
         },
-        "attributes": {"$ref": "#/definitions/attributes"},
         # The top level jobspec has groups and tasks
         # Groups are "flux batch"
         "groups": {"type": "array", "items": {"$ref": "#/definitions/group"}},
         # Tasks are one or more named tasks
         # Tasks are "flux submit" on the level they are defined
         "tasks": {"$ref": "#/definitions/tasks"},
+        "attributes": {"$ref": "#/definitions/attributes"},
         "additionalProperties": False,
     },
     "definitions": {
         "attributes": {
             "description": "system, parameter, and user attributes",
             "type": "object",
             "properties": {
                 "duration": {"type": "number", "minimum": 0},
                 "cwd": {"type": "string"},
                 "environment": {"type": "object"},
             },
         },
-        "requires": {
-            "description": "compatibility requirements",
-            "type": "object",
-        },
         "resources": {
             "description": "requested resources",
-            "oneOf": [
-                {"$ref": "#/definitions/node_vertex"},
-                {"$ref": "#/definitions/slot_vertex"},
-            ],
+            "type": "object",
+            "required": ["type"],
+            "properties": {
+                "type": {"type": "string"},
+                # Count is only required when below a slot
+                "count": {"type": "integer", "minimum": 1},
+                "requires": {
+                    "type": "array",
+                    "items": {"type": "object"},
+                },
+                "attributes": {"$ref": "#/definitions/attributes"},
+                "schedule": {"type": "boolean"},
+                "with": {
+                    "type": "array",
+                    "minItems": 1,
+                    "items": {"$ref": "#/definitions/resources"},
+                },
+            },
         },
         "steps": {
             "type": ["array"],
             "items": {
                 "type": "object",
                 "properties": {
                     "name": {
@@ -72,103 +79,46 @@
             "description": "tasks configuration",
             "type": "array",
             # If no slot is defined, it's implied to be at the top level (the node)
             "items": {
                 "type": "object",
                 "properties": {
                     # These are task level items that over-ride global
-                    "requires": {"$ref": "#/definitions/requires"},
                     # Resources in a task can be traditional OR a string reference
                     "resources": {"type": "string"},
-                    "attributes": {"$ref": "#/definitions/attributes"},
                     # A task can reference another group (a flux batch)
                     "group": {"type": "string"},
+                    # If the task is run locally on the level it is currently at.
+                    "local": {"type": "boolean"},
                     # Name only is needed to reference the task elsewhere
                     "name": {"type": "string"},
                     "depends_on": {"type": "array", "items": {"type": "string"}},
                     # How many of this task are to be run?
                     "replicas": {"type": "number", "minimum": 1, "default": 1},
                     # A command can be a string or a list of strings
                     "command": {
                         "type": ["string", "array"],
                         "minItems": 1,
                         "items": {"type": "string"},
                     },
                     # Custom logic for the transformer
-                    "steps": {"$ref": "#definitions/steps"},
+                    "steps": {"$ref": "#/definitions/steps"},
                 },
             },
         },
         "group": {
             "description": "group of tasks (batch)",
             "type": "object",
             # If no slot is defined, it's implied to be at the top level (the node)
             "properties": {
                 # Name only is needed to reference the group elsewhere
                 "name": {"type": "string"},
-                # These are task level items that over-ride global
-                "requires": {"$ref": "#/definitions/requires"},
-                # Resources in a task can be traditional OR a string reference
                 "resources": {"type": "string"},
-                "attributes": {"$ref": "#/definitions/attributes"},
                 "depends_on": {"type": "array", "items": {"type": "string"}},
                 # Tasks for the group
-                "tasks": {"$ref": "#definitions/tasks"},
-            },
-            "additionalProperties": False,
-        },
-        "intranode_resource_vertex": {
-            "description": "schema for resource vertices within a node, cannot have child vertices",
-            "type": "object",
-            "required": ["type", "count"],
-            "properties": {
-                "type": {"enum": ["core", "gpu"]},
-                "count": {"type": "integer", "minimum": 1},
-                "unit": {"type": "string"},
-            },
-            "additionalProperties": False,
-        },
-        "node_vertex": {
-            "description": "schema for the node resource vertex",
-            "type": "object",
-            "required": ["type", "count"],
-            "properties": {
-                "type": {"enum": ["node"]},
-                "count": {"type": "integer", "minimum": 1},
-                "unit": {"type": "string"},
-                "schedule": {"type": "boolean"},
-                "with": {
-                    "type": "array",
-                    "minItems": 1,
-                    "maxItems": 1,
-                    "items": {
-                        "oneOf": [
-                            {"$ref": "#/definitions/slot_vertex"},
-                            {"$ref": "#/definitions/intranode_resource_vertex"},
-                        ]
-                    },
-                },
-            },
-            "additionalProperties": False,
-        },
-        "slot_vertex": {
-            "description": "special slot resource type - label assigns to task slot",
-            "type": "object",
-            "required": ["type", "count", "with", "label"],
-            "properties": {
-                "type": {"enum": ["slot"]},
-                "count": {"type": "integer", "minimum": 1},
-                "unit": {"type": "string"},
-                "label": {"type": "string"},
-                "schedule": {"type": "boolean"},
-                "exclusive": {"type": "boolean"},
-                "with": {
-                    "type": "array",
-                    "minItems": 1,
-                    "maxItems": 2,
-                    "items": {"oneOf": [{"$ref": "#/definitions/intranode_resource_vertex"}]},
-                },
+                "tasks": {"$ref": "#/definitions/tasks"},
+                "groups": {"type": "array", "items": {"$ref": "#/definitions/group"}},
             },
             "additionalProperties": False,
         },
     },
 }
```

### Comparing `jobspec-0.1.1/jobspec/steps/base.py` & `jobspec-0.1.11/jobspec/steps/base.py`

 * *Files identical despite different names*

### Comparing `jobspec-0.1.1/jobspec/steps/fileio.py` & `jobspec-0.1.11/jobspec/steps/fileio.py`

 * *Files identical despite different names*

### Comparing `jobspec-0.1.1/jobspec/steps/runner.py` & `jobspec-0.1.11/jobspec/steps/runner.py`

 * *Files identical despite different names*

### Comparing `jobspec-0.1.1/jobspec/transformer/flux/steps.py` & `jobspec-0.1.11/jobspec/transformer/flux/steps.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,15 @@
         attributes = self.options.get("attributes") or {}
         task = self.options.get("task") or {}
 
         # This flattens to be what we ask flux for
         slot = resources.flatten_slot()
         nodes = slot.get("node")
         tasks = slot.get("core")
+        gpus = slot.get("gpu")
 
         # Get name, jobspec, depends, etc
         name = self.options.get("name")
         duration = attributes.get("duration")
         cwd = attributes.get("cwd")
         watch = attributes.get("watch")
 
@@ -113,14 +114,16 @@
         if watch is True:
             cmd += ["--watch"]
 
         if nodes:
             cmd += ["-N", str(nodes)]
         if tasks:
             cmd += ["-n", str(tasks)]
+        if gpus:
+            cmd += ["-g", str(gpus)]
 
         # Replicas we do with cc
         replicas = task.get("replicas")
         if replicas:
             replicas -= 1
             cmd += ["--cc", f"0-{replicas}"]
```

### Comparing `jobspec-0.1.1/jobspec/transformer/flux/workload.py` & `jobspec-0.1.11/jobspec/transformer/flux/workload.py`

 * *Files identical despite different names*

### Comparing `jobspec-0.1.1/jobspec/utils.py` & `jobspec-0.1.11/jobspec/utils.py`

 * *Files identical despite different names*

### Comparing `jobspec-0.1.1/jobspec/version.py` & `jobspec-0.1.11/jobspec/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.1"
+__version__ = "0.1.11"
 AUTHOR = "Vanessa Sochat"
 AUTHOR_EMAIL = "vsoch@users.noreply.github.com"
 NAME = "jobspec"
 PACKAGE_URL = "https://github.com/compspec/jobspec"
 KEYWORDS = "cluster, orchestration, transformer, jobspec, flux"
 DESCRIPTION = "Jobspec specification and translation layer for cluster work"
 LICENSE = "LICENSE"
```

### Comparing `jobspec-0.1.1/jobspec.egg-info/PKG-INFO` & `jobspec-0.1.11/jobspec.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jobspec
-Version: 0.1.1
+Version: 0.1.11
 Summary: Jobspec specification and translation layer for cluster work
 Home-page: https://github.com/compspec/jobspec
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: cluster,orchestration,transformer,jobspec,flux
```

### Comparing `jobspec-0.1.1/jobspec.egg-info/SOURCES.txt` & `jobspec-0.1.11/jobspec.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 jobspec.egg-info/not-zip-safe
 jobspec.egg-info/requires.txt
 jobspec.egg-info/top_level.txt
 jobspec/cli/__init__.py
 jobspec/cli/run.py
 jobspec/core/__init__.py
 jobspec/core/base.py
-jobspec/core/converter.py
 jobspec/core/core.py
 jobspec/core/resources.py
 jobspec/plugin/__init__.py
 jobspec/plugin/registry.py
 jobspec/steps/__init__.py
 jobspec/steps/base.py
 jobspec/steps/empty.py
```

### Comparing `jobspec-0.1.1/setup.py` & `jobspec-0.1.11/setup.py`

 * *Files identical despite different names*

