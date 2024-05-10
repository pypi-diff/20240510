# Comparing `tmp/pulumi_prefect-0.1.0a1715347486.tar.gz` & `tmp/pulumi_prefect-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_prefect-0.1.0a1715347486.tar", last modified: Fri May 10 13:27:49 2024, max compression
+gzip compressed data, was "pulumi_prefect-0.1.4.tar", last modified: Fri May 10 14:01:09 2024, max compression
```

## Comparing `pulumi_prefect-0.1.0a1715347486.tar` & `pulumi_prefect-0.1.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:27:49.101511 pulumi_prefect-0.1.0a1715347486/
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-10 13:27:49.101511 pulumi_prefect-0.1.0a1715347486/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-10 13:27:41.000000 pulumi_prefect-0.1.0a1715347486/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:27:49.097510 pulumi_prefect-0.1.0a1715347486/pulumi_prefect/
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-05-10 13:27:41.000000 pulumi_prefect-0.1.0a1715347486/pulumi_prefect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9297 2024-05-10 13:27:41.000000 pulumi_prefect-0.1.0a1715347486/pulumi_prefect/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    17818 2024-05-10 13:27:41.000000 pulumi_prefect-0.1.0a1715347486/pulumi_prefect/account.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:27:49.101511 pulumi_prefect-0.1.0a1715347486/pulumi_prefect/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-10 13:27:41.000000 pulumi_prefect-0.1.0a1715347486/pulumi_prefect/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-10 13:27:41.000000 pulumi_prefect-0.1.0a1715347486/pulumi_prefect/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-10 13:27:41.000000 pulumi_prefect-0.1.0a1715347486/pulumi_prefect/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     6387 2024-05-10 13:27:41.000000 pulumi_prefect-0.1.0a1715347486/pulumi_prefect/get_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     7384 2024-05-10 13:27:41.000000 pulumi_prefect-0.1.0a1715347486/pulumi_prefect/get_account_member.py
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-10 13:27:41.000000 pulumi_prefect-0.1.0a1715347486/pulumi_prefect/get_account_members.py
--rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-10 13:27:41.000000 pulumi_prefect-0.1.0a1715347486/pulumi_prefect/get_account_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     8643 2024-05-10 13:27:41.000000 pulumi_prefect-0.1.0a1715347486/pulumi_prefect/get_service_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-05-10 13:27:41.000000 pulumi_prefect-0.1.0a1715347486/pulumi_prefect/get_team.py
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-10 13:27:41.000000 pulumi_prefect-0.1.0a1715347486/pulumi_prefect/get_teams.py
--rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-05-10 13:27:41.000000 pulumi_prefect-0.1.0a1715347486/pulumi_prefect/get_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)    10123 2024-05-10 13:27:41.000000 pulumi_prefect-0.1.0a1715347486/pulumi_prefect/get_work_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-05-10 13:27:41.000000 pulumi_prefect-0.1.0a1715347486/pulumi_prefect/get_work_pools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-10 13:27:41.000000 pulumi_prefect-0.1.0a1715347486/pulumi_prefect/get_worker_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5984 2024-05-10 13:27:41.000000 pulumi_prefect-0.1.0a1715347486/pulumi_prefect/get_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     6915 2024-05-10 13:27:41.000000 pulumi_prefect-0.1.0a1715347486/pulumi_prefect/get_workspace_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    13359 2024-05-10 13:27:41.000000 pulumi_prefect-0.1.0a1715347486/pulumi_prefect/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8701 2024-05-10 13:27:41.000000 pulumi_prefect-0.1.0a1715347486/pulumi_prefect/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-10 13:27:41.000000 pulumi_prefect-0.1.0a1715347486/pulumi_prefect/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:27:41.000000 pulumi_prefect-0.1.0a1715347486/pulumi_prefect/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    22171 2024-05-10 13:27:41.000000 pulumi_prefect-0.1.0a1715347486/pulumi_prefect/service_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    16417 2024-05-10 13:27:41.000000 pulumi_prefect-0.1.0a1715347486/pulumi_prefect/variable.py
--rw-r--r--   0 runner    (1001) docker     (127)    26063 2024-05-10 13:27:41.000000 pulumi_prefect-0.1.0a1715347486/pulumi_prefect/work_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    14486 2024-05-10 13:27:41.000000 pulumi_prefect-0.1.0a1715347486/pulumi_prefect/workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)    17794 2024-05-10 13:27:41.000000 pulumi_prefect-0.1.0a1715347486/pulumi_prefect/workspace_access.py
--rw-r--r--   0 runner    (1001) docker     (127)    16675 2024-05-10 13:27:41.000000 pulumi_prefect-0.1.0a1715347486/pulumi_prefect/workspace_role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:27:49.101511 pulumi_prefect-0.1.0a1715347486/pulumi_prefect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-10 13:27:49.000000 pulumi_prefect-0.1.0a1715347486/pulumi_prefect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-10 13:27:49.000000 pulumi_prefect-0.1.0a1715347486/pulumi_prefect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 13:27:49.000000 pulumi_prefect-0.1.0a1715347486/pulumi_prefect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-10 13:27:49.000000 pulumi_prefect-0.1.0a1715347486/pulumi_prefect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-10 13:27:49.000000 pulumi_prefect-0.1.0a1715347486/pulumi_prefect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-10 13:27:41.000000 pulumi_prefect-0.1.0a1715347486/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 13:27:49.101511 pulumi_prefect-0.1.0a1715347486/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:01:09.888512 pulumi_prefect-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-10 14:01:09.888512 pulumi_prefect-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-10 14:01:02.000000 pulumi_prefect-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:01:09.888512 pulumi_prefect-0.1.4/pulumi_prefect/
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-05-10 14:01:02.000000 pulumi_prefect-0.1.4/pulumi_prefect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9297 2024-05-10 14:01:02.000000 pulumi_prefect-0.1.4/pulumi_prefect/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17818 2024-05-10 14:01:02.000000 pulumi_prefect-0.1.4/pulumi_prefect/account.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:01:09.888512 pulumi_prefect-0.1.4/pulumi_prefect/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-10 14:01:02.000000 pulumi_prefect-0.1.4/pulumi_prefect/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-10 14:01:02.000000 pulumi_prefect-0.1.4/pulumi_prefect/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-10 14:01:02.000000 pulumi_prefect-0.1.4/pulumi_prefect/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6387 2024-05-10 14:01:02.000000 pulumi_prefect-0.1.4/pulumi_prefect/get_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7384 2024-05-10 14:01:02.000000 pulumi_prefect-0.1.4/pulumi_prefect/get_account_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-10 14:01:02.000000 pulumi_prefect-0.1.4/pulumi_prefect/get_account_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-10 14:01:02.000000 pulumi_prefect-0.1.4/pulumi_prefect/get_account_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8643 2024-05-10 14:01:02.000000 pulumi_prefect-0.1.4/pulumi_prefect/get_service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-05-10 14:01:02.000000 pulumi_prefect-0.1.4/pulumi_prefect/get_team.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-10 14:01:02.000000 pulumi_prefect-0.1.4/pulumi_prefect/get_teams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-05-10 14:01:02.000000 pulumi_prefect-0.1.4/pulumi_prefect/get_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10123 2024-05-10 14:01:02.000000 pulumi_prefect-0.1.4/pulumi_prefect/get_work_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-05-10 14:01:02.000000 pulumi_prefect-0.1.4/pulumi_prefect/get_work_pools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-10 14:01:02.000000 pulumi_prefect-0.1.4/pulumi_prefect/get_worker_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5984 2024-05-10 14:01:02.000000 pulumi_prefect-0.1.4/pulumi_prefect/get_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6915 2024-05-10 14:01:02.000000 pulumi_prefect-0.1.4/pulumi_prefect/get_workspace_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13359 2024-05-10 14:01:02.000000 pulumi_prefect-0.1.4/pulumi_prefect/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8701 2024-05-10 14:01:02.000000 pulumi_prefect-0.1.4/pulumi_prefect/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-10 14:01:02.000000 pulumi_prefect-0.1.4/pulumi_prefect/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:01:02.000000 pulumi_prefect-0.1.4/pulumi_prefect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    22155 2024-05-10 14:01:02.000000 pulumi_prefect-0.1.4/pulumi_prefect/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16417 2024-05-10 14:01:02.000000 pulumi_prefect-0.1.4/pulumi_prefect/variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26063 2024-05-10 14:01:02.000000 pulumi_prefect-0.1.4/pulumi_prefect/work_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14486 2024-05-10 14:01:02.000000 pulumi_prefect-0.1.4/pulumi_prefect/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17794 2024-05-10 14:01:02.000000 pulumi_prefect-0.1.4/pulumi_prefect/workspace_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16675 2024-05-10 14:01:02.000000 pulumi_prefect-0.1.4/pulumi_prefect/workspace_role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:01:09.888512 pulumi_prefect-0.1.4/pulumi_prefect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-10 14:01:09.000000 pulumi_prefect-0.1.4/pulumi_prefect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-10 14:01:09.000000 pulumi_prefect-0.1.4/pulumi_prefect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 14:01:09.000000 pulumi_prefect-0.1.4/pulumi_prefect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-10 14:01:09.000000 pulumi_prefect-0.1.4/pulumi_prefect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-10 14:01:09.000000 pulumi_prefect-0.1.4/pulumi_prefect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-10 14:01:02.000000 pulumi_prefect-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 14:01:09.888512 pulumi_prefect-0.1.4/setup.cfg
```

### Comparing `pulumi_prefect-0.1.0a1715347486/PKG-INFO` & `pulumi_prefect-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_prefect
-Version: 0.1.0a1715347486
+Version: 0.1.4
 Summary: A Pulumi package for creating and managing Prefect cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://www.pulumi.com
 Project-URL: Repository, https://github.com/ru5j4r0/pulumi-prefect
 Keywords: prefect,prefect-cloud,category/cloud
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_prefect-0.1.0a1715347486/README.md` & `pulumi_prefect-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_prefect-0.1.0a1715347486/pulumi_prefect/__init__.py` & `pulumi_prefect-0.1.4/pulumi_prefect/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_prefect-0.1.0a1715347486/pulumi_prefect/_utilities.py` & `pulumi_prefect-0.1.4/pulumi_prefect/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_prefect-0.1.0a1715347486/pulumi_prefect/account.py` & `pulumi_prefect-0.1.4/pulumi_prefect/account.py`

 * *Files identical despite different names*

### Comparing `pulumi_prefect-0.1.0a1715347486/pulumi_prefect/config/__init__.pyi` & `pulumi_prefect-0.1.4/pulumi_prefect/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_prefect-0.1.0a1715347486/pulumi_prefect/config/vars.py` & `pulumi_prefect-0.1.4/pulumi_prefect/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_prefect-0.1.0a1715347486/pulumi_prefect/get_account.py` & `pulumi_prefect-0.1.4/pulumi_prefect/get_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_prefect-0.1.0a1715347486/pulumi_prefect/get_account_member.py` & `pulumi_prefect-0.1.4/pulumi_prefect/get_account_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_prefect-0.1.0a1715347486/pulumi_prefect/get_account_members.py` & `pulumi_prefect-0.1.4/pulumi_prefect/get_account_members.py`

 * *Files identical despite different names*

### Comparing `pulumi_prefect-0.1.0a1715347486/pulumi_prefect/get_account_role.py` & `pulumi_prefect-0.1.4/pulumi_prefect/get_account_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_prefect-0.1.0a1715347486/pulumi_prefect/get_service_account.py` & `pulumi_prefect-0.1.4/pulumi_prefect/get_service_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_prefect-0.1.0a1715347486/pulumi_prefect/get_team.py` & `pulumi_prefect-0.1.4/pulumi_prefect/get_team.py`

 * *Files identical despite different names*

### Comparing `pulumi_prefect-0.1.0a1715347486/pulumi_prefect/get_teams.py` & `pulumi_prefect-0.1.4/pulumi_prefect/get_teams.py`

 * *Files identical despite different names*

### Comparing `pulumi_prefect-0.1.0a1715347486/pulumi_prefect/get_variable.py` & `pulumi_prefect-0.1.4/pulumi_prefect/get_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_prefect-0.1.0a1715347486/pulumi_prefect/get_work_pool.py` & `pulumi_prefect-0.1.4/pulumi_prefect/get_work_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_prefect-0.1.0a1715347486/pulumi_prefect/get_work_pools.py` & `pulumi_prefect-0.1.4/pulumi_prefect/get_work_pools.py`

 * *Files identical despite different names*

### Comparing `pulumi_prefect-0.1.0a1715347486/pulumi_prefect/get_worker_metadata.py` & `pulumi_prefect-0.1.4/pulumi_prefect/get_worker_metadata.py`

 * *Files identical despite different names*

### Comparing `pulumi_prefect-0.1.0a1715347486/pulumi_prefect/get_workspace.py` & `pulumi_prefect-0.1.4/pulumi_prefect/get_workspace.py`

 * *Files identical despite different names*

### Comparing `pulumi_prefect-0.1.0a1715347486/pulumi_prefect/get_workspace_role.py` & `pulumi_prefect-0.1.4/pulumi_prefect/get_workspace_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_prefect-0.1.0a1715347486/pulumi_prefect/outputs.py` & `pulumi_prefect-0.1.4/pulumi_prefect/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_prefect-0.1.0a1715347486/pulumi_prefect/provider.py` & `pulumi_prefect-0.1.4/pulumi_prefect/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_prefect-0.1.0a1715347486/pulumi_prefect/service_account.py` & `pulumi_prefect-0.1.4/pulumi_prefect/service_account.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,22 +269,22 @@
         API Keys for `service_account` resources can be rotated by modifying the `api_key_expiration` attribute.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_prefect as prefect
-        import pulumi_time as time
+        import pulumiverse_time as time
 
         # NON-EXPIRING API KEY
         example_service_account = prefect.ServiceAccount("exampleServiceAccount")
-        ninety_days = time.index.Time_rotating("ninetyDays", rotation_days=90)
+        ninety_days = time.Rotating("ninetyDays", rotation_days=90)
         # Pass the time_rotating resource to the `api_key_expiration` attribute
         # in order to automate the rotation of the Service Account key
-        example_index_service_account_service_account = prefect.ServiceAccount("exampleIndex/serviceAccountServiceAccount", api_key_expiration=ninety_days["rotationRfc3339"])
+        example_index_service_account_service_account = prefect.ServiceAccount("exampleIndex/serviceAccountServiceAccount", api_key_expiration=ninety_days.rotation_rfc3339)
         ```
 
         ## Import
 
         Prefect Service Accounts can be imported via name in the form `name/my-bot-name`
 
         ```sh
@@ -318,22 +318,22 @@
         API Keys for `service_account` resources can be rotated by modifying the `api_key_expiration` attribute.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_prefect as prefect
-        import pulumi_time as time
+        import pulumiverse_time as time
 
         # NON-EXPIRING API KEY
         example_service_account = prefect.ServiceAccount("exampleServiceAccount")
-        ninety_days = time.index.Time_rotating("ninetyDays", rotation_days=90)
+        ninety_days = time.Rotating("ninetyDays", rotation_days=90)
         # Pass the time_rotating resource to the `api_key_expiration` attribute
         # in order to automate the rotation of the Service Account key
-        example_index_service_account_service_account = prefect.ServiceAccount("exampleIndex/serviceAccountServiceAccount", api_key_expiration=ninety_days["rotationRfc3339"])
+        example_index_service_account_service_account = prefect.ServiceAccount("exampleIndex/serviceAccountServiceAccount", api_key_expiration=ninety_days.rotation_rfc3339)
         ```
 
         ## Import
 
         Prefect Service Accounts can be imported via name in the form `name/my-bot-name`
 
         ```sh
```

### Comparing `pulumi_prefect-0.1.0a1715347486/pulumi_prefect/variable.py` & `pulumi_prefect-0.1.4/pulumi_prefect/variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_prefect-0.1.0a1715347486/pulumi_prefect/work_pool.py` & `pulumi_prefect-0.1.4/pulumi_prefect/work_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_prefect-0.1.0a1715347486/pulumi_prefect/workspace.py` & `pulumi_prefect-0.1.4/pulumi_prefect/workspace.py`

 * *Files identical despite different names*

### Comparing `pulumi_prefect-0.1.0a1715347486/pulumi_prefect/workspace_access.py` & `pulumi_prefect-0.1.4/pulumi_prefect/workspace_access.py`

 * *Files identical despite different names*

### Comparing `pulumi_prefect-0.1.0a1715347486/pulumi_prefect/workspace_role.py` & `pulumi_prefect-0.1.4/pulumi_prefect/workspace_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_prefect-0.1.0a1715347486/pulumi_prefect.egg-info/PKG-INFO` & `pulumi_prefect-0.1.4/pulumi_prefect.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_prefect
-Version: 0.1.0a1715347486
+Version: 0.1.4
 Summary: A Pulumi package for creating and managing Prefect cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://www.pulumi.com
 Project-URL: Repository, https://github.com/ru5j4r0/pulumi-prefect
 Keywords: prefect,prefect-cloud,category/cloud
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_prefect-0.1.0a1715347486/pulumi_prefect.egg-info/SOURCES.txt` & `pulumi_prefect-0.1.4/pulumi_prefect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_prefect-0.1.0a1715347486/pyproject.toml` & `pulumi_prefect-0.1.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_prefect"
   description = "A Pulumi package for creating and managing Prefect cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["prefect", "prefect-cloud", "category/cloud"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.1.0a1715347486"
+  version = "0.1.4"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://www.pulumi.com"
     Repository = "https://github.com/ru5j4r0/pulumi-prefect"
 
 [build-system]
```

