# Comparing `tmp/npc_shields-0.1.5.tar.gz` & `tmp/npc_shields-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npc_shields-0.1.5.tar", last modified: Tue Dec  5 02:04:18 2023, max compression
+gzip compressed data, was "npc_shields-0.1.6.tar", last modified: Thu May  9 21:56:43 2024, max compression
```

## Comparing `npc_shields-0.1.5.tar` & `npc_shields-0.1.6.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 02:04:18.078724 npc_shields-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2023-12-05 02:04:18.078724 npc_shields-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2023-12-05 02:03:50.000000 npc_shields-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2023-12-05 02:04:15.000000 npc_shields-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-05 02:04:18.078724 npc_shields-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 02:04:18.074724 npc_shields-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 02:04:18.074724 npc_shields-0.1.5/src/npc_shields/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-12-05 02:03:50.000000 npc_shields-0.1.5/src/npc_shields/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 02:04:18.078724 npc_shields-0.1.5/src/npc_shields/drawings/
--rw-r--r--   0 runner    (1001) docker     (127)    85004 2023-12-05 02:03:50.000000 npc_shields-0.1.5/src/npc_shields/drawings/2001.svg
--rw-r--r--   0 runner    (1001) docker     (127)   150594 2023-12-05 02:03:50.000000 npc_shields-0.1.5/src/npc_shields/drawings/2002.svg
--rw-r--r--   0 runner    (1001) docker     (127)   108511 2023-12-05 02:03:50.000000 npc_shields-0.1.5/src/npc_shields/drawings/2005.svg
--rw-r--r--   0 runner    (1001) docker     (127)    99489 2023-12-05 02:03:50.000000 npc_shields-0.1.5/src/npc_shields/drawings/2006.svg
--rw-r--r--   0 runner    (1001) docker     (127)    84797 2023-12-05 02:03:50.000000 npc_shields-0.1.5/src/npc_shields/drawings/Templeton_combos.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7205 2023-12-05 02:03:50.000000 npc_shields-0.1.5/src/npc_shields/insertions.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-05 02:03:50.000000 npc_shields-0.1.5/src/npc_shields/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4088 2023-12-05 02:03:50.000000 npc_shields-0.1.5/src/npc_shields/shields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2023-12-05 02:03:50.000000 npc_shields-0.1.5/src/npc_shields/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8627 2023-12-05 02:04:13.000000 npc_shields-0.1.5/src/npc_shields/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 02:04:18.078724 npc_shields-0.1.5/src/npc_shields.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2023-12-05 02:04:18.000000 npc_shields-0.1.5/src/npc_shields.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      562 2023-12-05 02:04:18.000000 npc_shields-0.1.5/src/npc_shields.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-05 02:04:18.000000 npc_shields-0.1.5/src/npc_shields.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-05 02:04:18.000000 npc_shields-0.1.5/src/npc_shields.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-05 02:04:18.000000 npc_shields-0.1.5/src/npc_shields.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:56:43.497014 npc_shields-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-09 21:56:43.497014 npc_shields-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-09 21:56:06.000000 npc_shields-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-05-09 21:56:41.000000 npc_shields-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 21:56:43.497014 npc_shields-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:56:43.493014 npc_shields-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:56:43.493014 npc_shields-0.1.6/src/npc_shields/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-09 21:56:06.000000 npc_shields-0.1.6/src/npc_shields/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:56:43.497014 npc_shields-0.1.6/src/npc_shields/drawings/
+-rw-r--r--   0 runner    (1001) docker     (127)    85004 2024-05-09 21:56:06.000000 npc_shields-0.1.6/src/npc_shields/drawings/2001.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   150594 2024-05-09 21:56:06.000000 npc_shields-0.1.6/src/npc_shields/drawings/2002.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   108511 2024-05-09 21:56:06.000000 npc_shields-0.1.6/src/npc_shields/drawings/2005.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    99489 2024-05-09 21:56:06.000000 npc_shields-0.1.6/src/npc_shields/drawings/2006.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    84797 2024-05-09 21:56:06.000000 npc_shields-0.1.6/src/npc_shields/drawings/Templeton_combos.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-05-09 21:56:38.000000 npc_shields-0.1.6/src/npc_shields/injections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7164 2024-05-09 21:56:06.000000 npc_shields-0.1.6/src/npc_shields/insertions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 21:56:06.000000 npc_shields-0.1.6/src/npc_shields/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-05-09 21:56:06.000000 npc_shields-0.1.6/src/npc_shields/shields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-09 21:56:38.000000 npc_shields-0.1.6/src/npc_shields/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8627 2024-05-09 21:56:06.000000 npc_shields-0.1.6/src/npc_shields/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:56:43.497014 npc_shields-0.1.6/src/npc_shields.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-09 21:56:43.000000 npc_shields-0.1.6/src/npc_shields.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-09 21:56:43.000000 npc_shields-0.1.6/src/npc_shields.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 21:56:43.000000 npc_shields-0.1.6/src/npc_shields.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-09 21:56:43.000000 npc_shields-0.1.6/src/npc_shields.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-09 21:56:43.000000 npc_shields-0.1.6/src/npc_shields.egg-info/top_level.txt
```

### Comparing `npc_shields-0.1.5/PKG-INFO` & `npc_shields-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npc_shields
-Version: 0.1.5
+Version: 0.1.6
 Summary: Tools for Neuropixels probe insertion: providing suggested targets, recording actual insertions, storing notes.
 Author-email: bjhardcastle <ben.hardcastle@alleninstitute.org>
 License: MIT
 Project-URL: Repository, https://github.com/AllenInstitute/npc_shields
 Project-URL: Issues, https://github.com/AllenInstitute/npc_shields/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `npc_shields-0.1.5/README.md` & `npc_shields-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `npc_shields-0.1.5/pyproject.toml` & `npc_shields-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "npc_shields"
-version = "0.1.5"
+version = "0.1.6"
 description = "Tools for Neuropixels probe insertion: providing suggested targets, recording actual insertions, storing notes."
 authors = [
     { name = "bjhardcastle", email = "ben.hardcastle@alleninstitute.org" },
 ]
 dependencies = [
     "ipywidgets>=7",
     "npc-session>=0.1.30",
```

### Comparing `npc_shields-0.1.5/src/npc_shields/drawings/2001.svg` & `npc_shields-0.1.6/src/npc_shields/drawings/2001.svg`

 * *Files identical despite different names*

### Comparing `npc_shields-0.1.5/src/npc_shields/drawings/2002.svg` & `npc_shields-0.1.6/src/npc_shields/drawings/2002.svg`

 * *Files identical despite different names*

### Comparing `npc_shields-0.1.5/src/npc_shields/drawings/2005.svg` & `npc_shields-0.1.6/src/npc_shields/drawings/2005.svg`

 * *Files identical despite different names*

### Comparing `npc_shields-0.1.5/src/npc_shields/drawings/2006.svg` & `npc_shields-0.1.6/src/npc_shields/drawings/2006.svg`

 * *Files identical despite different names*

### Comparing `npc_shields-0.1.5/src/npc_shields/drawings/Templeton_combos.svg` & `npc_shields-0.1.6/src/npc_shields/drawings/Templeton_combos.svg`

 * *Files identical despite different names*

### Comparing `npc_shields-0.1.5/src/npc_shields/insertions.py` & `npc_shields-0.1.6/src/npc_shields/insertions.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
     def to_json(self) -> dict[str, Any]:
         """
         >>> i = Insertion(npc_shields.shields.DR2002)
         >>> j = i.to_json()
         >>> assert j["shield"]["name"] == "2002"
         """
         return {
-            "shield": dict(name=self.shield.name, drawing_id=self.shield.drawing_id),
+            "shield": self.shield.to_json(),
             "probes": dict(self.probes),
             "notes": self.notes,
         }
 
     def to_svg(self) -> str:
         return npc_shields.shields.get_svg_data_with_insertions(
             self.shield, self.probes
```

### Comparing `npc_shields-0.1.5/src/npc_shields/shields.py` & `npc_shields-0.1.6/src/npc_shields/shields.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 @dataclasses.dataclass(frozen=True, unsafe_hash=True)
 class Shield:
     name: str
     drawing_id: int | str
     labels: Iterable[str] = dataclasses.field(repr=False)
     svg: pathlib.Path
 
+    def to_json(self) -> dict[str, str | int]:
+        return dict(name=self.name, drawing_id=self.drawing_id)
+
 
 def get_labels_from_mapping(mapping: Mapping[str, Iterable[int]]) -> tuple[str, ...]:
     """Convert a mapping of probe letter to insertion holes to a tuple of labels.
 
     >>> get_labels_from_mapping({"A": (1, 2, 3), "B": (1, 2, 3, 4)})
     ('A1', 'A2', 'A3', 'B1', 'B2', 'B3', 'B4')
     """
```

### Comparing `npc_shields-0.1.5/src/npc_shields/widgets.py` & `npc_shields-0.1.6/src/npc_shields/widgets.py`

 * *Files identical despite different names*

### Comparing `npc_shields-0.1.5/src/npc_shields.egg-info/PKG-INFO` & `npc_shields-0.1.6/src/npc_shields.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: npc-shields
-Version: 0.1.5
+Name: npc_shields
+Version: 0.1.6
 Summary: Tools for Neuropixels probe insertion: providing suggested targets, recording actual insertions, storing notes.
 Author-email: bjhardcastle <ben.hardcastle@alleninstitute.org>
 License: MIT
 Project-URL: Repository, https://github.com/AllenInstitute/npc_shields
 Project-URL: Issues, https://github.com/AllenInstitute/npc_shields/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `npc_shields-0.1.5/src/npc_shields.egg-info/SOURCES.txt` & `npc_shields-0.1.6/src/npc_shields.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 README.md
 pyproject.toml
 src/npc_shields/__init__.py
+src/npc_shields/injections.py
 src/npc_shields/insertions.py
 src/npc_shields/py.typed
 src/npc_shields/shields.py
 src/npc_shields/types.py
 src/npc_shields/widgets.py
 src/npc_shields.egg-info/PKG-INFO
 src/npc_shields.egg-info/SOURCES.txt
```

