# Comparing `tmp/openframe_criteria_set_protocol-1.4.6.tar.gz` & `tmp/openframe_criteria_set_protocol-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openframe_criteria_set_protocol-1.4.6.tar", last modified: Fri Apr 19 08:06:47 2024, max compression
+gzip compressed data, was "openframe_criteria_set_protocol-1.4.7.tar", last modified: Fri May 10 10:09:22 2024, max compression
```

## Comparing `openframe_criteria_set_protocol-1.4.6.tar` & `openframe_criteria_set_protocol-1.4.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 andresangulo   (501) staff       (20)        0 2024-04-19 08:06:47.853041 openframe_criteria_set_protocol-1.4.6/
--rw-r--r--   0 andresangulo   (501) staff       (20)    19134 2023-10-19 16:06:44.000000 openframe_criteria_set_protocol-1.4.6/LICENSE
--rw-r--r--   0 andresangulo   (501) staff       (20)     5434 2024-04-19 08:06:47.852790 openframe_criteria_set_protocol-1.4.6/PKG-INFO
--rw-r--r--   0 andresangulo   (501) staff       (20)     4797 2023-10-25 12:32:39.000000 openframe_criteria_set_protocol-1.4.6/README.md
-drwxr-xr-x   0 andresangulo   (501) staff       (20)        0 2024-04-19 08:06:47.848745 openframe_criteria_set_protocol-1.4.6/openframe_criteria_set_protocol/
--rw-r--r--   0 andresangulo   (501) staff       (20)       17 2024-01-06 19:43:41.000000 openframe_criteria_set_protocol-1.4.6/openframe_criteria_set_protocol/__init__.py
-drwxr-xr-x   0 andresangulo   (501) staff       (20)        0 2024-04-19 08:06:47.850793 openframe_criteria_set_protocol-1.4.6/openframe_criteria_set_protocol/v1/
--rw-r--r--   0 andresangulo   (501) staff       (20)       62 2024-01-09 10:55:39.000000 openframe_criteria_set_protocol-1.4.6/openframe_criteria_set_protocol/v1/__init__.py
--rw-r--r--   0 andresangulo   (501) staff       (20)      741 2024-01-05 22:18:50.000000 openframe_criteria_set_protocol-1.4.6/openframe_criteria_set_protocol/v1/errors.py
--rw-r--r--   0 andresangulo   (501) staff       (20)      585 2024-02-01 10:45:40.000000 openframe_criteria_set_protocol-1.4.6/openframe_criteria_set_protocol/v1/schemas.py
--rw-r--r--   0 andresangulo   (501) staff       (20)     3315 2024-02-01 10:44:34.000000 openframe_criteria_set_protocol-1.4.6/openframe_criteria_set_protocol/v1/services.py
--rw-r--r--   0 andresangulo   (501) staff       (20)     6404 2024-04-19 08:06:35.000000 openframe_criteria_set_protocol-1.4.6/openframe_criteria_set_protocol/v1/types.py
--rw-r--r--   0 andresangulo   (501) staff       (20)     1628 2024-03-08 19:22:46.000000 openframe_criteria_set_protocol-1.4.6/openframe_criteria_set_protocol/v1/utils.py
-drwxr-xr-x   0 andresangulo   (501) staff       (20)        0 2024-04-19 08:06:47.852470 openframe_criteria_set_protocol-1.4.6/openframe_criteria_set_protocol.egg-info/
--rw-r--r--   0 andresangulo   (501) staff       (20)     5434 2024-04-19 08:06:47.000000 openframe_criteria_set_protocol-1.4.6/openframe_criteria_set_protocol.egg-info/PKG-INFO
--rw-r--r--   0 andresangulo   (501) staff       (20)      665 2024-04-19 08:06:47.000000 openframe_criteria_set_protocol-1.4.6/openframe_criteria_set_protocol.egg-info/SOURCES.txt
--rw-r--r--   0 andresangulo   (501) staff       (20)        1 2024-04-19 08:06:47.000000 openframe_criteria_set_protocol-1.4.6/openframe_criteria_set_protocol.egg-info/dependency_links.txt
--rw-r--r--   0 andresangulo   (501) staff       (20)       38 2024-04-19 08:06:47.000000 openframe_criteria_set_protocol-1.4.6/openframe_criteria_set_protocol.egg-info/top_level.txt
--rw-r--r--   0 andresangulo   (501) staff       (20)      671 2024-04-19 08:05:48.000000 openframe_criteria_set_protocol-1.4.6/pyproject.toml
--rw-r--r--   0 andresangulo   (501) staff       (20)       38 2024-04-19 08:06:47.853097 openframe_criteria_set_protocol-1.4.6/setup.cfg
--rw-r--r--   0 andresangulo   (501) staff       (20)      417 2024-04-19 08:05:48.000000 openframe_criteria_set_protocol-1.4.6/setup.py
-drwxr-xr-x   0 andresangulo   (501) staff       (20)        0 2024-04-19 08:06:47.851101 openframe_criteria_set_protocol-1.4.6/tests/
--rw-r--r--   0 andresangulo   (501) staff       (20)        0 2023-10-19 14:05:39.000000 openframe_criteria_set_protocol-1.4.6/tests/__init__.py
-drwxr-xr-x   0 andresangulo   (501) staff       (20)        0 2024-04-19 08:06:47.851865 openframe_criteria_set_protocol-1.4.6/tests/v1/
--rw-r--r--   0 andresangulo   (501) staff       (20)       41 2023-10-24 11:21:14.000000 openframe_criteria_set_protocol-1.4.6/tests/v1/__init__.py
--rw-r--r--   0 andresangulo   (501) staff       (20)      788 2023-10-24 11:36:52.000000 openframe_criteria_set_protocol-1.4.6/tests/v1/test_schemas.py
--rw-r--r--   0 andresangulo   (501) staff       (20)    11950 2024-01-27 14:13:37.000000 openframe_criteria_set_protocol-1.4.6/tests/v1/test_types.py
+drwxr-xr-x   0 andresangulo   (501) staff       (20)        0 2024-05-10 10:09:22.794661 openframe_criteria_set_protocol-1.4.7/
+-rw-r--r--   0 andresangulo   (501) staff       (20)    19134 2023-10-19 16:06:44.000000 openframe_criteria_set_protocol-1.4.7/LICENSE
+-rw-r--r--   0 andresangulo   (501) staff       (20)     5434 2024-05-10 10:09:22.794466 openframe_criteria_set_protocol-1.4.7/PKG-INFO
+-rw-r--r--   0 andresangulo   (501) staff       (20)     4797 2023-10-25 12:32:39.000000 openframe_criteria_set_protocol-1.4.7/README.md
+drwxr-xr-x   0 andresangulo   (501) staff       (20)        0 2024-05-10 10:09:22.790309 openframe_criteria_set_protocol-1.4.7/openframe_criteria_set_protocol/
+-rw-r--r--   0 andresangulo   (501) staff       (20)       17 2024-01-06 19:43:41.000000 openframe_criteria_set_protocol-1.4.7/openframe_criteria_set_protocol/__init__.py
+drwxr-xr-x   0 andresangulo   (501) staff       (20)        0 2024-05-10 10:09:22.792659 openframe_criteria_set_protocol-1.4.7/openframe_criteria_set_protocol/v1/
+-rw-r--r--   0 andresangulo   (501) staff       (20)       62 2024-01-09 10:55:39.000000 openframe_criteria_set_protocol-1.4.7/openframe_criteria_set_protocol/v1/__init__.py
+-rw-r--r--   0 andresangulo   (501) staff       (20)      741 2024-01-05 22:18:50.000000 openframe_criteria_set_protocol-1.4.7/openframe_criteria_set_protocol/v1/errors.py
+-rw-r--r--   0 andresangulo   (501) staff       (20)      585 2024-02-01 10:45:40.000000 openframe_criteria_set_protocol-1.4.7/openframe_criteria_set_protocol/v1/schemas.py
+-rw-r--r--   0 andresangulo   (501) staff       (20)     3315 2024-02-01 10:44:34.000000 openframe_criteria_set_protocol-1.4.7/openframe_criteria_set_protocol/v1/services.py
+-rw-r--r--   0 andresangulo   (501) staff       (20)     6404 2024-04-19 08:06:35.000000 openframe_criteria_set_protocol-1.4.7/openframe_criteria_set_protocol/v1/types.py
+-rw-r--r--   0 andresangulo   (501) staff       (20)     2761 2024-05-10 10:04:43.000000 openframe_criteria_set_protocol-1.4.7/openframe_criteria_set_protocol/v1/utils.py
+drwxr-xr-x   0 andresangulo   (501) staff       (20)        0 2024-05-10 10:09:22.794118 openframe_criteria_set_protocol-1.4.7/openframe_criteria_set_protocol.egg-info/
+-rw-r--r--   0 andresangulo   (501) staff       (20)     5434 2024-05-10 10:09:22.000000 openframe_criteria_set_protocol-1.4.7/openframe_criteria_set_protocol.egg-info/PKG-INFO
+-rw-r--r--   0 andresangulo   (501) staff       (20)      665 2024-05-10 10:09:22.000000 openframe_criteria_set_protocol-1.4.7/openframe_criteria_set_protocol.egg-info/SOURCES.txt
+-rw-r--r--   0 andresangulo   (501) staff       (20)        1 2024-05-10 10:09:22.000000 openframe_criteria_set_protocol-1.4.7/openframe_criteria_set_protocol.egg-info/dependency_links.txt
+-rw-r--r--   0 andresangulo   (501) staff       (20)       38 2024-05-10 10:09:22.000000 openframe_criteria_set_protocol-1.4.7/openframe_criteria_set_protocol.egg-info/top_level.txt
+-rw-r--r--   0 andresangulo   (501) staff       (20)      671 2024-05-10 10:08:51.000000 openframe_criteria_set_protocol-1.4.7/pyproject.toml
+-rw-r--r--   0 andresangulo   (501) staff       (20)       38 2024-05-10 10:09:22.794700 openframe_criteria_set_protocol-1.4.7/setup.cfg
+-rw-r--r--   0 andresangulo   (501) staff       (20)      417 2024-05-10 10:08:51.000000 openframe_criteria_set_protocol-1.4.7/setup.py
+drwxr-xr-x   0 andresangulo   (501) staff       (20)        0 2024-05-10 10:09:22.793058 openframe_criteria_set_protocol-1.4.7/tests/
+-rw-r--r--   0 andresangulo   (501) staff       (20)        0 2023-10-19 14:05:39.000000 openframe_criteria_set_protocol-1.4.7/tests/__init__.py
+drwxr-xr-x   0 andresangulo   (501) staff       (20)        0 2024-05-10 10:09:22.793699 openframe_criteria_set_protocol-1.4.7/tests/v1/
+-rw-r--r--   0 andresangulo   (501) staff       (20)       41 2023-10-24 11:21:14.000000 openframe_criteria_set_protocol-1.4.7/tests/v1/__init__.py
+-rw-r--r--   0 andresangulo   (501) staff       (20)      788 2023-10-24 11:36:52.000000 openframe_criteria_set_protocol-1.4.7/tests/v1/test_schemas.py
+-rw-r--r--   0 andresangulo   (501) staff       (20)    11950 2024-01-27 14:13:37.000000 openframe_criteria_set_protocol-1.4.7/tests/v1/test_types.py
```

### Comparing `openframe_criteria_set_protocol-1.4.6/LICENSE` & `openframe_criteria_set_protocol-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `openframe_criteria_set_protocol-1.4.6/PKG-INFO` & `openframe_criteria_set_protocol-1.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openframe-criteria-set-protocol
-Version: 1.4.6
+Version: 1.4.7
 Summary: A protocol and tools for defining and working with criteria sets
 Author: Andrés Angulo <aa@openframe.org>
 Author-email: Andrés Angulo <aa@openframe.org>
 Project-URL: Homepage, https://github.com/openframe-org/criteria-set-protocol
 Project-URL: Bug Tracker, https://github.com/openframe-org/criteria-set-protocol/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `openframe_criteria_set_protocol-1.4.6/README.md` & `openframe_criteria_set_protocol-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `openframe_criteria_set_protocol-1.4.6/openframe_criteria_set_protocol/v1/errors.py` & `openframe_criteria_set_protocol-1.4.7/openframe_criteria_set_protocol/v1/errors.py`

 * *Files identical despite different names*

### Comparing `openframe_criteria_set_protocol-1.4.6/openframe_criteria_set_protocol/v1/schemas.py` & `openframe_criteria_set_protocol-1.4.7/openframe_criteria_set_protocol/v1/schemas.py`

 * *Files identical despite different names*

### Comparing `openframe_criteria_set_protocol-1.4.6/openframe_criteria_set_protocol/v1/services.py` & `openframe_criteria_set_protocol-1.4.7/openframe_criteria_set_protocol/v1/services.py`

 * *Files identical despite different names*

### Comparing `openframe_criteria_set_protocol-1.4.6/openframe_criteria_set_protocol/v1/types.py` & `openframe_criteria_set_protocol-1.4.7/openframe_criteria_set_protocol/v1/types.py`

 * *Files identical despite different names*

### Comparing `openframe_criteria_set_protocol-1.4.6/openframe_criteria_set_protocol/v1/utils.py` & `openframe_criteria_set_protocol-1.4.7/openframe_criteria_set_protocol/v1/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,80 @@
 from typing import Optional
 
-from .types import Quality, CriteriaTreeElement, Criterion, TaskGroup, Task
+from .types import Quality, CriteriaTreeElement, Criterion, TaskGroup, Task, CriteriaTree
 
 
 def to_color_hex_string(color):
+    """
+    Convert a color object to a hex string
+    """
     if isinstance(color, str):
         return color
     return f"#{color.red:02x}{color.green:02x}{color.blue:02x}"
 
 
 def should_hide_code(element: CriteriaTreeElement | str | dict) -> bool:
+    """
+    Check if a tree element should be hidden in the output
+    """
     if isinstance(element, str):
         return element.startswith('_')
     if isinstance(element, dict):
         code: Optional[str] = element.get('code', None)
         if code is None:
             raise ValueError("Element must have a 'code' key")
         return code.startswith('_')
     return element.code.startswith('_')
 
 
 def get_qualified_name(element: Quality | Criterion | TaskGroup | Task | dict) -> str:
+    """
+    Get the qualified name of a tree element, which is the title with the code prepended if it is different
+    """
     if isinstance(element, dict):
         title, code = (element.get('title', None), element.get('code', None))
         if title is None or code is None:
             raise ValueError("Element must have 'title' and 'code' keys")
     else:
         title, code = element.title, element.code
     if code.startswith('_'):
         code = code[1:]
     if element.title == code:
         return element.title
     return f"{code} {element.title}"
 
 
 def resolve_code(element: CriteriaTreeElement | str | dict) -> str:
+    """
+    Get the code for a tree element, stripping away unnecessary characters
+    """
     if isinstance(element, str):
         resolved_code = element
     elif isinstance(element, dict):
         resolved_code = element.get('code', None)
         if resolved_code is None:
             raise ValueError("Element must have a 'code' key")
     else:
         resolved_code = element.code
     return resolved_code[1:] if resolved_code.startswith('_') else resolved_code
+
+
+def find_in_tree(tree: CriteriaTree, code: str) -> Optional[CriteriaTreeElement]:
+    """
+    Find an element in the criteria tree by its code
+    """
+    for quality in tree.qualities:
+        if quality.code == code:
+            return quality
+        for criteria in quality.items:
+            if criteria.code == code:
+                return criteria
+            for task_group in criteria.items:
+                if task_group.code == code:
+                    return task_group
+                for task in task_group.items:
+                    if task.code == code:
+                        return task
+                    for task_item in task.items:
+                        if task_item.code == code:
+                            return task_item
+    return None
```

### Comparing `openframe_criteria_set_protocol-1.4.6/openframe_criteria_set_protocol.egg-info/PKG-INFO` & `openframe_criteria_set_protocol-1.4.7/openframe_criteria_set_protocol.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openframe-criteria-set-protocol
-Version: 1.4.6
+Version: 1.4.7
 Summary: A protocol and tools for defining and working with criteria sets
 Author: Andrés Angulo <aa@openframe.org>
 Author-email: Andrés Angulo <aa@openframe.org>
 Project-URL: Homepage, https://github.com/openframe-org/criteria-set-protocol
 Project-URL: Bug Tracker, https://github.com/openframe-org/criteria-set-protocol/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `openframe_criteria_set_protocol-1.4.6/openframe_criteria_set_protocol.egg-info/SOURCES.txt` & `openframe_criteria_set_protocol-1.4.7/openframe_criteria_set_protocol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openframe_criteria_set_protocol-1.4.6/pyproject.toml` & `openframe_criteria_set_protocol-1.4.7/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "openframe-criteria-set-protocol"
-version = "1.4.6"
+version = "1.4.7"
 authors = [
     { name="Andrés Angulo", email="aa@openframe.org" },
 ]
 description = "A protocol and tools for defining and working with criteria sets"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

### Comparing `openframe_criteria_set_protocol-1.4.6/tests/v1/test_schemas.py` & `openframe_criteria_set_protocol-1.4.7/tests/v1/test_schemas.py`

 * *Files identical despite different names*

### Comparing `openframe_criteria_set_protocol-1.4.6/tests/v1/test_types.py` & `openframe_criteria_set_protocol-1.4.7/tests/v1/test_types.py`

 * *Files identical despite different names*

