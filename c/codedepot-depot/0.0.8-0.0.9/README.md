# Comparing `tmp/codedepot_depot-0.0.8.tar.gz` & `tmp/codedepot_depot-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codedepot_depot-0.0.8.tar", last modified: Mon Apr 29 09:53:27 2024, max compression
+gzip compressed data, was "codedepot_depot-0.0.9.tar", last modified: Mon Apr 29 09:55:21 2024, max compression
```

## Comparing `codedepot_depot-0.0.8.tar` & `codedepot_depot-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       54 2024-04-15 07:13:36.336177 codedepot_depot-0.0.8/README.md
--rw-r--r--   0        0        0        0 2024-04-15 13:02:27.184638 codedepot_depot-0.0.8/depot/__init__.py
--rw-r--r--   0        0        0     7623 2024-04-29 09:50:26.764206 codedepot_depot-0.0.8/depot/api.py
--rw-r--r--   0        0        0      624 2024-04-18 08:11:02.116570 codedepot_depot-0.0.8/depot/cluster_spec.py
--rw-r--r--   0        0        0     3998 2024-04-21 22:00:24.992845 codedepot_depot-0.0.8/depot/config.py
--rw-r--r--   0        0        0      507 2024-04-18 06:56:25.799963 codedepot_depot-0.0.8/depot/jobfile.py
--rw-r--r--   0        0        0     4283 2024-04-29 09:51:52.234881 codedepot_depot-0.0.8/depot/main.py
--rw-r--r--   0        0        0      616 2024-04-16 05:00:55.267184 codedepot_depot-0.0.8/depot/provider_spec.py
--rw-r--r--   0        0        0      817 2024-04-29 09:53:27.801464 codedepot_depot-0.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-15 20:33:04.196404 codedepot_depot-0.0.8/test/__init__.py
--rw-r--r--   0        0        0       86 2024-04-16 05:02:59.830823 codedepot_depot-0.0.8/test/resources/cluster_test.yaml
--rw-r--r--   0        0        0       87 2024-04-15 20:48:31.758568 codedepot_depot-0.0.8/test/resources/config.json
--rw-r--r--   0        0        0       80 2024-04-15 20:35:06.454038 codedepot_depot-0.0.8/test/resources/local_cred.json
--rw-r--r--   0        0        0       96 2024-04-16 04:58:41.947831 codedepot_depot-0.0.8/test/resources/provider_test.yaml
--rw-r--r--   0        0        0        0 2024-04-16 04:06:38.432329 codedepot_depot-0.0.8/test/test_client.py
--rw-r--r--   0        0        0      408 2024-04-16 05:35:56.755146 codedepot_depot-0.0.8/test/test_provider.py
--rw-r--r--   0        0        0      666 2024-04-16 05:28:37.442814 codedepot_depot-0.0.8/test/utils.py
--rw-r--r--   0        0        0      791 1970-01-01 00:00:00.000000 codedepot_depot-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       54 2024-04-15 07:13:36.336177 codedepot_depot-0.0.9/README.md
+-rw-r--r--   0        0        0        0 2024-04-15 13:02:27.184638 codedepot_depot-0.0.9/depot/__init__.py
+-rw-r--r--   0        0        0     7623 2024-04-29 09:50:26.764206 codedepot_depot-0.0.9/depot/api.py
+-rw-r--r--   0        0        0      624 2024-04-18 08:11:02.116570 codedepot_depot-0.0.9/depot/cluster_spec.py
+-rw-r--r--   0        0        0     3998 2024-04-21 22:00:24.992845 codedepot_depot-0.0.9/depot/config.py
+-rw-r--r--   0        0        0      507 2024-04-18 06:56:25.799963 codedepot_depot-0.0.9/depot/jobfile.py
+-rw-r--r--   0        0        0     4283 2024-04-29 09:54:57.642107 codedepot_depot-0.0.9/depot/main.py
+-rw-r--r--   0        0        0      616 2024-04-16 05:00:55.267184 codedepot_depot-0.0.9/depot/provider_spec.py
+-rw-r--r--   0        0        0      849 2024-04-29 09:55:21.599027 codedepot_depot-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-15 20:33:04.196404 codedepot_depot-0.0.9/test/__init__.py
+-rw-r--r--   0        0        0       86 2024-04-16 05:02:59.830823 codedepot_depot-0.0.9/test/resources/cluster_test.yaml
+-rw-r--r--   0        0        0       87 2024-04-15 20:48:31.758568 codedepot_depot-0.0.9/test/resources/config.json
+-rw-r--r--   0        0        0       80 2024-04-15 20:35:06.454038 codedepot_depot-0.0.9/test/resources/local_cred.json
+-rw-r--r--   0        0        0       96 2024-04-16 04:58:41.947831 codedepot_depot-0.0.9/test/resources/provider_test.yaml
+-rw-r--r--   0        0        0        0 2024-04-16 04:06:38.432329 codedepot_depot-0.0.9/test/test_client.py
+-rw-r--r--   0        0        0      408 2024-04-16 05:35:56.755146 codedepot_depot-0.0.9/test/test_provider.py
+-rw-r--r--   0        0        0      666 2024-04-16 05:28:37.442814 codedepot_depot-0.0.9/test/utils.py
+-rw-r--r--   0        0        0      831 1970-01-01 00:00:00.000000 codedepot_depot-0.0.9/PKG-INFO
```

### Comparing `codedepot_depot-0.0.8/depot/api.py` & `codedepot_depot-0.0.9/depot/api.py`

 * *Files identical despite different names*

### Comparing `codedepot_depot-0.0.8/depot/cluster_spec.py` & `codedepot_depot-0.0.9/depot/cluster_spec.py`

 * *Files identical despite different names*

### Comparing `codedepot_depot-0.0.8/depot/config.py` & `codedepot_depot-0.0.9/depot/config.py`

 * *Files identical despite different names*

### Comparing `codedepot_depot-0.0.8/depot/main.py` & `codedepot_depot-0.0.9/depot/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     # Parse the arguments
     return parser.parse_args()
 
 
 def main():
     args = parse_args()
     if args.version:
-        print("0.0.8")
+        print("0.0.9")
         return
 
     if args.command == 'login':
         DepotConfig.create()
         return
 
     config = DepotConfig.default()
```

### Comparing `codedepot_depot-0.0.8/depot/provider_spec.py` & `codedepot_depot-0.0.9/depot/provider_spec.py`

 * *Files identical despite different names*

### Comparing `codedepot_depot-0.0.8/pyproject.toml` & `codedepot_depot-0.0.9/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.pdm]
 
 [project]
 name = "codedepot-depot"
-version = "0.0.8"
+version = "0.0.9"
 description = "Job launch support for Git AI"
 readme = "README.md"
 authors = [
     { name = "CodeDepot", email = "contact@codedepot.ai" },
 ]
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -23,14 +23,15 @@
     "pydantic",
     "pygit2",
     "requests",
     "depot_api",
     "codedepot-git-ai>=0.0.20",
     "depot-api>=1.0.3",
     "depot-api>=1.0.4",
+    "codedepot-git-ai>=0.0.24",
 ]
 
 [project.urls]
 Homepage = "https://github.com/codedepotai/git-ai"
 
 [project.scripts]
 depot = "depot.main:main"
```

### Comparing `codedepot_depot-0.0.8/test/utils.py` & `codedepot_depot-0.0.9/test/utils.py`

 * *Files identical despite different names*

### Comparing `codedepot_depot-0.0.8/PKG-INFO` & `codedepot_depot-0.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codedepot-depot
-Version: 0.0.8
+Version: 0.0.9
 Summary: Job launch support for Git AI
 Author-Email: CodeDepot <contact@codedepot.ai>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Homepage, https://github.com/codedepotai/git-ai
 Requires-Python: >=3.10
@@ -16,12 +16,13 @@
 Requires-Dist: pydantic
 Requires-Dist: pygit2
 Requires-Dist: requests
 Requires-Dist: depot_api
 Requires-Dist: codedepot-git-ai>=0.0.20
 Requires-Dist: depot-api>=1.0.3
 Requires-Dist: depot-api>=1.0.4
+Requires-Dist: codedepot-git-ai>=0.0.24
 Description-Content-Type: text/markdown
 
 # Depot
 
 This is the depot client. More docs to come.
```

