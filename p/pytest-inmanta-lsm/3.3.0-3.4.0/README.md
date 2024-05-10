# Comparing `tmp/pytest_inmanta_lsm-3.3.0.tar.gz` & `tmp/pytest_inmanta_lsm-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_inmanta_lsm-3.3.0.tar", last modified: Mon Apr 15 13:33:15 2024, max compression
+gzip compressed data, was "pytest_inmanta_lsm-3.4.0.tar", last modified: Fri May 10 12:25:54 2024, max compression
```

## Comparing `pytest_inmanta_lsm-3.3.0.tar` & `pytest_inmanta_lsm-3.4.0.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxrwxr-x   0 jenkins    (988) jenkins    (986)        0 2024-04-15 13:33:15.755594 pytest_inmanta_lsm-3.3.0/
--rw-rw-r--   0 jenkins    (988) jenkins    (986)     6731 2024-04-15 13:33:11.000000 pytest_inmanta_lsm-3.3.0/CHANGELOG.md
--rw-rw-r--   0 jenkins    (988) jenkins    (986)       86 2024-04-15 13:32:59.000000 pytest_inmanta_lsm-3.3.0/LICENSE
--rw-rw-r--   0 jenkins    (988) jenkins    (986)       12 2024-04-15 13:32:59.000000 pytest_inmanta_lsm-3.3.0/MANIFEST.in
--rw-r--r--   0 jenkins    (988) jenkins    (986)    20261 2024-04-15 13:33:15.755594 pytest_inmanta_lsm-3.3.0/PKG-INFO
--rw-rw-r--   0 jenkins    (988) jenkins    (986)    19327 2024-04-15 13:33:09.000000 pytest_inmanta_lsm-3.3.0/README.md
--rw-rw-r--   0 jenkins    (988) jenkins    (986)      228 2024-04-15 13:32:59.000000 pytest_inmanta_lsm-3.3.0/pyproject.toml
--rw-rw-r--   0 jenkins    (988) jenkins    (986)      610 2024-04-15 13:33:15.755594 pytest_inmanta_lsm-3.3.0/setup.cfg
--rw-rw-r--   0 jenkins    (988) jenkins    (986)     1818 2024-04-15 13:33:11.000000 pytest_inmanta_lsm-3.3.0/setup.py
-drwxrwxr-x   0 jenkins    (988) jenkins    (986)        0 2024-04-15 13:33:15.751594 pytest_inmanta_lsm-3.3.0/src/
-drwxrwxr-x   0 jenkins    (988) jenkins    (986)        0 2024-04-15 13:33:15.753594 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/
--rw-rw-r--   0 jenkins    (988) jenkins    (986)      775 2024-04-15 13:32:59.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/__init__.py
--rw-rw-r--   0 jenkins    (988) jenkins    (986)     1847 2024-04-15 13:32:59.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/exceptions.py
--rw-rw-r--   0 jenkins    (988) jenkins    (986)     2635 2024-04-15 13:32:59.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/failed_resources_logs.py
--rw-rw-r--   0 jenkins    (988) jenkins    (986)    42233 2024-04-15 13:33:09.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/lsm_project.py
--rw-rw-r--   0 jenkins    (988) jenkins    (986)    18098 2024-04-15 13:33:09.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/managed_service_instance.py
--rw-rw-r--   0 jenkins    (988) jenkins    (986)     9905 2024-04-15 13:33:09.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/orchestrator_container.py
--rw-rw-r--   0 jenkins    (988) jenkins    (986)     7956 2024-04-15 13:33:09.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/parameters.py
--rw-rw-r--   0 jenkins    (988) jenkins    (986)    19222 2024-04-15 13:33:09.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/plugin.py
--rw-rw-r--   0 jenkins    (988) jenkins    (986)        0 2024-04-15 13:32:59.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/py.typed
--rw-rw-r--   0 jenkins    (988) jenkins    (986)    36800 2024-04-15 13:33:09.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/remote_orchestrator.py
--rw-rw-r--   0 jenkins    (988) jenkins    (986)     2915 2024-04-15 13:33:09.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/remote_service_instance.py
--rw-rw-r--   0 jenkins    (988) jenkins    (986)     9257 2024-04-15 13:33:09.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/remote_service_instance.pyi
--rw-rw-r--   0 jenkins    (988) jenkins    (986)    23508 2024-04-15 13:33:09.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/remote_service_instance_async.py
-drwxrwxr-x   0 jenkins    (988) jenkins    (986)        0 2024-04-15 13:33:15.754594 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/resources/
--rw-rw-r--   0 jenkins    (988) jenkins    (986)      773 2024-04-15 13:32:59.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/resources/docker-compose.yml
--rw-rw-r--   0 jenkins    (988) jenkins    (986)       25 2024-04-15 13:32:59.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/resources/my-env-file
--rw-rw-r--   0 jenkins    (988) jenkins    (986)     3444 2024-04-15 13:32:59.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/resources/my-server-conf.cfg
--rw-rw-r--   0 jenkins    (988) jenkins    (986)     3517 2024-04-15 13:32:59.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/resources/setup_project.py
--rw-rw-r--   0 jenkins    (988) jenkins    (986)     3421 2024-04-15 13:33:09.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/util.py
--rw-rw-r--   0 jenkins    (988) jenkins    (986)     7957 2024-04-15 13:32:59.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/wait_for_state.py
-drwxrwxr-x   0 jenkins    (988) jenkins    (986)        0 2024-04-15 13:33:15.754594 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm.egg-info/
--rw-r--r--   0 jenkins    (988) jenkins    (986)    20261 2024-04-15 13:33:15.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins    (988) jenkins    (986)     1279 2024-04-15 13:33:15.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins    (988) jenkins    (986)        1 2024-04-15 13:33:15.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins    (988) jenkins    (986)       51 2024-04-15 13:33:15.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm.egg-info/entry_points.txt
--rw-rw-r--   0 jenkins    (988) jenkins    (986)       41 2024-04-15 13:33:15.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm.egg-info/requires.txt
--rw-rw-r--   0 jenkins    (988) jenkins    (986)       19 2024-04-15 13:33:15.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm.egg-info/top_level.txt
-drwxrwxr-x   0 jenkins    (988) jenkins    (986)        0 2024-04-15 13:33:15.754594 pytest_inmanta_lsm-3.3.0/tests/
--rw-rw-r--   0 jenkins    (988) jenkins    (986)      840 2024-04-15 13:33:09.000000 pytest_inmanta_lsm-3.3.0/tests/test_basic_example.py
--rw-rw-r--   0 jenkins    (988) jenkins    (986)     2342 2024-04-15 13:33:09.000000 pytest_inmanta_lsm-3.3.0/tests/test_containerized_orchestrator.py
--rw-rw-r--   0 jenkins    (988) jenkins    (986)     1893 2024-04-15 13:32:59.000000 pytest_inmanta_lsm-3.3.0/tests/test_partial.py
+drwxrwxr-x   0 jenkins    (988) jenkins    (986)        0 2024-05-10 12:25:54.317861 pytest_inmanta_lsm-3.4.0/
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)     7414 2024-05-10 12:25:50.000000 pytest_inmanta_lsm-3.4.0/CHANGELOG.md
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)       86 2024-05-10 12:25:38.000000 pytest_inmanta_lsm-3.4.0/LICENSE
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)       12 2024-05-10 12:25:38.000000 pytest_inmanta_lsm-3.4.0/MANIFEST.in
+-rw-r--r--   0 jenkins    (988) jenkins    (986)    21347 2024-05-10 12:25:54.317861 pytest_inmanta_lsm-3.4.0/PKG-INFO
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)    20413 2024-05-10 12:25:48.000000 pytest_inmanta_lsm-3.4.0/README.md
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)      228 2024-05-10 12:25:38.000000 pytest_inmanta_lsm-3.4.0/pyproject.toml
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)      610 2024-05-10 12:25:54.318861 pytest_inmanta_lsm-3.4.0/setup.cfg
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)     1869 2024-05-10 12:25:50.000000 pytest_inmanta_lsm-3.4.0/setup.py
+drwxrwxr-x   0 jenkins    (988) jenkins    (986)        0 2024-05-10 12:25:54.312861 pytest_inmanta_lsm-3.4.0/src/
+drwxrwxr-x   0 jenkins    (988) jenkins    (986)        0 2024-05-10 12:25:54.315861 pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm/
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)      775 2024-05-10 12:25:38.000000 pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm/__init__.py
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)     1847 2024-05-10 12:25:38.000000 pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm/exceptions.py
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)     2635 2024-05-10 12:25:38.000000 pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm/failed_resources_logs.py
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)     8776 2024-05-10 12:25:48.000000 pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm/load_generator.py
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)    43166 2024-05-10 12:25:48.000000 pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm/lsm_project.py
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)    18098 2024-05-10 12:25:38.000000 pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm/managed_service_instance.py
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)    10049 2024-05-10 12:25:48.000000 pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm/orchestrator_container.py
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)     8458 2024-05-10 12:25:48.000000 pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm/parameters.py
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)    24409 2024-05-10 12:25:48.000000 pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm/plugin.py
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)        0 2024-05-10 12:25:38.000000 pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm/py.typed
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)    41371 2024-05-10 12:25:48.000000 pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm/remote_orchestrator.py
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)     2915 2024-05-10 12:25:38.000000 pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm/remote_service_instance.py
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)     9410 2024-05-10 12:25:48.000000 pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm/remote_service_instance.pyi
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)    24939 2024-05-10 12:25:48.000000 pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm/remote_service_instance_async.py
+drwxrwxr-x   0 jenkins    (988) jenkins    (986)        0 2024-05-10 12:25:54.317861 pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm/resources/
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)      773 2024-05-10 12:25:48.000000 pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm/resources/docker-compose-legacy.yml
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)      945 2024-05-10 12:25:48.000000 pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm/resources/docker-compose.yml
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)       25 2024-05-10 12:25:38.000000 pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm/resources/my-env-file
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)     3444 2024-05-10 12:25:38.000000 pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm/resources/my-server-conf.cfg
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)     3517 2024-05-10 12:25:38.000000 pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm/resources/setup_project.py
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)     3421 2024-05-10 12:25:38.000000 pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm/util.py
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)     7957 2024-05-10 12:25:38.000000 pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm/wait_for_state.py
+drwxrwxr-x   0 jenkins    (988) jenkins    (986)        0 2024-05-10 12:25:54.317861 pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm.egg-info/
+-rw-r--r--   0 jenkins    (988) jenkins    (986)    21347 2024-05-10 12:25:54.000000 pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)     1379 2024-05-10 12:25:54.000000 pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)        1 2024-05-10 12:25:54.000000 pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)       51 2024-05-10 12:25:54.000000 pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm.egg-info/entry_points.txt
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)       41 2024-05-10 12:25:54.000000 pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm.egg-info/requires.txt
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)       19 2024-05-10 12:25:54.000000 pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm.egg-info/top_level.txt
+drwxrwxr-x   0 jenkins    (988) jenkins    (986)        0 2024-05-10 12:25:54.317861 pytest_inmanta_lsm-3.4.0/tests/
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)     1416 2024-05-10 12:25:48.000000 pytest_inmanta_lsm-3.4.0/tests/test_basic_example.py
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)     2901 2024-05-10 12:25:48.000000 pytest_inmanta_lsm-3.4.0/tests/test_containerized_orchestrator.py
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)     1893 2024-05-10 12:25:38.000000 pytest_inmanta_lsm-3.4.0/tests/test_partial.py
```

### Comparing `pytest_inmanta_lsm-3.3.0/CHANGELOG.md` & `pytest_inmanta_lsm-3.4.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# v 3.4.0 (2024-05-10)
+Changes in this release:
+- Add support to `LsmProject.compile` to have multiple instances selected
+- Add `LoadGenerator` helper to generate some load on the remote orchestrator
+- Add `--lsm-dump-on-failure` option, allowing to generate a support archive of the orchestrator when a test fails, and save it in the host /tmp directory. (#409)
+- Make sure that the orchestrators started by pytest-inmanta-lsm log their output to `/var/log/inmanta/server.log` instead of stdout.
+- Fix race condition in `RemoteServiceInstance.wait_for_state` that would make it return a `ServiceInstance` for the latest version rather than the one we asked the method to wait for.
+
 # v 3.3.0 (2024-04-15)
 Changes in this release:
 - Better logs when `docker-compose` in not installed
 - Add async `RemoteServiceInstance` class, for async service testing.
 - Add `export_service_entities` helper to `LsmProject` class.  Allowing to test the definition of a service.  (#352)
 - Allow to easily reuse model used in `export_service_entities` for all later compiles.
 - Validate that any service added to the `LsmProject` object using `add_service` method is part of one of the exported services. (#354)
```

### Comparing `pytest_inmanta_lsm-3.3.0/PKG-INFO` & `pytest_inmanta_lsm-3.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-inmanta-lsm
-Version: 3.3.0
+Version: 3.4.0
 Summary: Common fixtures for inmanta LSM related modules
 Home-page: https://github.com/inmanta/pytest-inmanta-lsm
 Author: Inmanta
 Author-email: code@inmanta.com
 License: inmanta EULA
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
@@ -65,32 +65,39 @@
 
     # Test the synchronous service instance class
     instance = remote_service_instance.RemoteServiceInstance(
         remote_orchestrator=remote_orchestrator,
         service_entity_name=SERVICE_NAME,
     )
 
-    # Create the service instance and stop waiting in a transient state
+    # Create the service instance and stop waiting in a transient state, and get the service instance
+    # as it is in the target state.
     created = instance.create(
         {
             "router_ip": "10.1.9.17",
             "interface_name": "eth1",
             "address": "10.0.0.254/24",
             "vlan_id": 14,
         },
         wait_for_state="creating",
         timeout=60,
     )
 
-    # Wait for up state, we provide here the version from which we should follow the
-    # service, which is the version in which we last stopped following the service.  This
-    # guarantees that we don't "miss" the target state, in case it is a transient one, and
-    # don't confuse the start state for the target one in case it is the same one.
-    # The start version should always be the last version in which we know our service has
-    # been, BEFORE the target state we expect our service to go into.
+    # Wait for up state.  The method will check each version that the service goes through,
+    # starting AFTER the start_version if it is provided, or the current version of the service
+    # if start_version is not provided.  As soon as a version is a match, the helper will return the
+    # service instance at this given state.
+    # It is important to provide the correct start_version to avoid falling in any of these situations:
+    # 1. We could miss the target state, if at the moment we start waiting for the target state, it is
+    #    already reached and no start_version is provided (as we would start looking AFTER the current
+    #    version).
+    # 2. We could select the wrong target state if we start looking at too old versions (in the case of
+    #    an update for example, we might mistake the source up state for the target one).
+    # In this example, we start after the version of the creating state, as we know it is before our up
+    # state.
     instance.wait_for_state(
         target_state="up",
         start_version=created.version,
         timeout=60,
     )
 
     # Delete the instance
@@ -367,14 +374,21 @@
   --lsm-ssl             [True | False] Choose whether to use SSL/TLS or not when
                         connecting to the remote orchestrator. (overrides
                         INMANTA_LSM_SSL, defaults to False)
   --lsm-token
                         The token used to authenticate to the remote
                         orchestrator when authentication is enabled. (overrides
                         INMANTA_LSM_TOKEN)
+  --lsm-dump-on-failure
+                        Whether to create and save a support archive when a test fails.
+                        The support archive will be saved in the /tmp directory of the
+                        host running the test and will not be cleaned up. The value of
+                        this option can be overwritten for each test case individually
+                        by overwriting the value of the remote_orchestrator_dump_on_failure
+                        fixture. (overrides INMANTA_LSM_DUMP_ON_FAILURE, defaults to False)
 
 ```
 
 ## Running tests
 
 ### How the test suite is structured
```

### Comparing `pytest_inmanta_lsm-3.3.0/README.md` & `pytest_inmanta_lsm-3.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -39,32 +39,39 @@
 
     # Test the synchronous service instance class
     instance = remote_service_instance.RemoteServiceInstance(
         remote_orchestrator=remote_orchestrator,
         service_entity_name=SERVICE_NAME,
     )
 
-    # Create the service instance and stop waiting in a transient state
+    # Create the service instance and stop waiting in a transient state, and get the service instance
+    # as it is in the target state.
     created = instance.create(
         {
             "router_ip": "10.1.9.17",
             "interface_name": "eth1",
             "address": "10.0.0.254/24",
             "vlan_id": 14,
         },
         wait_for_state="creating",
         timeout=60,
     )
 
-    # Wait for up state, we provide here the version from which we should follow the
-    # service, which is the version in which we last stopped following the service.  This
-    # guarantees that we don't "miss" the target state, in case it is a transient one, and
-    # don't confuse the start state for the target one in case it is the same one.
-    # The start version should always be the last version in which we know our service has
-    # been, BEFORE the target state we expect our service to go into.
+    # Wait for up state.  The method will check each version that the service goes through,
+    # starting AFTER the start_version if it is provided, or the current version of the service
+    # if start_version is not provided.  As soon as a version is a match, the helper will return the
+    # service instance at this given state.
+    # It is important to provide the correct start_version to avoid falling in any of these situations:
+    # 1. We could miss the target state, if at the moment we start waiting for the target state, it is
+    #    already reached and no start_version is provided (as we would start looking AFTER the current
+    #    version).
+    # 2. We could select the wrong target state if we start looking at too old versions (in the case of
+    #    an update for example, we might mistake the source up state for the target one).
+    # In this example, we start after the version of the creating state, as we know it is before our up
+    # state.
     instance.wait_for_state(
         target_state="up",
         start_version=created.version,
         timeout=60,
     )
 
     # Delete the instance
@@ -341,14 +348,21 @@
   --lsm-ssl             [True | False] Choose whether to use SSL/TLS or not when
                         connecting to the remote orchestrator. (overrides
                         INMANTA_LSM_SSL, defaults to False)
   --lsm-token
                         The token used to authenticate to the remote
                         orchestrator when authentication is enabled. (overrides
                         INMANTA_LSM_TOKEN)
+  --lsm-dump-on-failure
+                        Whether to create and save a support archive when a test fails.
+                        The support archive will be saved in the /tmp directory of the
+                        host running the test and will not be cleaned up. The value of
+                        this option can be overwritten for each test case individually
+                        by overwriting the value of the remote_orchestrator_dump_on_failure
+                        fixture. (overrides INMANTA_LSM_DUMP_ON_FAILURE, defaults to False)
 
 ```
 
 ## Running tests
 
 ### How the test suite is structured
```

### Comparing `pytest_inmanta_lsm-3.3.0/setup.cfg` & `pytest_inmanta_lsm-3.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytest_inmanta_lsm-3.3.0/setup.py` & `pytest_inmanta_lsm-3.4.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,27 +17,28 @@
 def read(fname):
     file_path = os.path.join(os.path.dirname(__file__), fname)
     return codecs.open(file_path, encoding="utf-8").read()
 
 
 setup(
     name="pytest-inmanta-lsm",
-    version="3.3.0",
+    version="3.4.0",
     python_requires=">=3.6",  # also update classifiers
     author="Inmanta",
     author_email="code@inmanta.com",
     license="inmanta EULA",
     url="https://github.com/inmanta/pytest-inmanta-lsm",
     description="Common fixtures for inmanta LSM related modules",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     package_dir={"": "src"},
     packages=["pytest_inmanta_lsm"],
     package_data={
         "pytest_inmanta_lsm": [
+            "resources/docker-compose-legacy.yml",
             "resources/docker-compose.yml",
             "resources/my-env-file",
             "resources/my-server-conf.cfg",
             "resources/setup_project.py",
             "py.typed",
         ]
     },
```

### Comparing `pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/__init__.py` & `pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/exceptions.py` & `pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/failed_resources_logs.py` & `pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm/failed_resources_logs.py`

 * *Files identical despite different names*

### Comparing `pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/lsm_project.py` & `pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm/lsm_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -630,15 +630,15 @@
             # Delegate the proper export to the existing logic in lsm module
             inmanta_plugins.lsm.do_export_service_entities(
                 exporter,
                 types,
                 False,
             )
 
-    def get_service(self, service_id: uuid.UUID) -> inmanta_lsm.model.ServiceInstance:
+    def get_service(self, service_id: typing.Union[uuid.UUID, str]) -> inmanta_lsm.model.ServiceInstance:
         """
         Get the service with the given id from our inventory.  If no such service exists,
         raise a LookupError.
 
         :param service_id: The id of the service we are looking for
         """
         if str(service_id) not in self.services:
@@ -858,28 +858,29 @@
                 )
 
         self.services[str(service.id)] = service
 
     def compile(
         self,
         model: typing.Optional[str] = None,
-        service_id: typing.Optional[uuid.UUID] = None,
+        service_id: typing.Optional[typing.Union[uuid.UUID, str, typing.Sequence[typing.Union[uuid.UUID, str]]]] = None,
         validation: bool = True,
     ) -> None:
         """
         Perform a compile for the service whose id is passed in argument.  The correct attribute
         set will be selected based on the current state of the service.  If some allocation is
         involved, the attributes of the service will be updated accordingly.
 
         :param model: The model to compile (passed to project.compile).  If no model is specified,
             default to the model that was exported (in export_service_entities).  If no model was
             exported, raise a ValueError.
         :param service_id: The id of the service that should be compiled, the service must have
             been added to the set of services prior to the compile.  If no service_id is provided,
             do a normal, full-compile.
+            For validation only one ID can be provided. For other compiles, multiple can be provided
         :param validation: Whether this is a validation compile or not.
         """
         # Make sure we have a model to compile
         if model is not None:
             pass
         elif self.model is not None:
             model = self.model
@@ -892,37 +893,53 @@
 
         if service_id is None:
             # This is not a service-specific compile, we can just run the compile
             # without setting any environment variables
             self.project.compile(model, no_dedent=False)
             return
 
-        # Get the service targeted by the compile
-        service = self.get_service(service_id)
+        # Sort out the type variance of service_id
+        if isinstance(service_id, (str, uuid.UUID)):
+            # strings are also sequences
+            service_ids = str(service_id)
+        elif isinstance(service_id, typing.Sequence):
+            service_ids = " ".join(str(i) for i in service_id)
+        else:
+            raise TypeError(f"Unexpected argument type for service_id, got {service_id} ({type(service_id)})")
+
+        # Make sure all instances exist in the inventory
+        for service_id in service_ids.split(" "):
+            service = self.get_service(service_id)
 
         env: dict[str, str] = {}
-        env[inmanta_lsm.const.ENV_INSTANCE_ID] = str(service_id)
-        env[inmanta_lsm.const.ENV_INSTANCE_VERSION] = str(service.version)
+        env[inmanta_lsm.const.ENV_INSTANCE_ID] = service_ids
+
+        if validation:
+            if len(service_ids.split(" ")) != 1:
+                raise Exception(
+                    f"when performing a validation compile, only one service id can be passed, got {repr(service_ids)}"
+                )
+            service = self.get_service(service_ids)
+            env[inmanta_lsm.const.ENV_INSTANCE_VERSION] = str(service.version)
 
         try:
             env[inmanta_lsm.const.ENV_PARTIAL_COMPILE] = str(self.partial_compile)
         except AttributeError:
             # This attribute only exists for iso5+, iso4 doesn't support partial compile.
             # We then simply don't set the value.
             if self.partial_compile:
                 warnings.warn("Partial compile is enabled but it is not supported, it will be ignored.")
 
         if validation:
             # If we have a validation compile, we need to set an additional env var
             env[inmanta_lsm.const.ENV_MODEL_STATE] = inmanta_lsm.model.ModelState.candidate
 
         LOGGER.debug(
-            "Triggering compile for service %s (%s) with the following environment variables: %s",
-            service.id,
-            service.service_entity,
+            "Triggering compile for service %s with the following environment variables: %s",
+            service_ids,
             env,
         )
         with self.monkeypatch.context() as m:
             for k, v in env.items():
                 m.setenv(k, v)
             self.project.compile(model, no_dedent=False)
```

### Comparing `pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/managed_service_instance.py` & `pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm/managed_service_instance.py`

 * *Files identical despite different names*

### Comparing `pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/orchestrator_container.py` & `pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm/orchestrator_container.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,15 +143,15 @@
         docker_compose_dir = self.compose_file.parent
         shutil.copytree(str(docker_compose_dir), str(self._cwd), dirs_exist_ok=True)
 
         shutil.copy(str(self.config_file), str(self._cwd / "my-server-conf.cfg"))
         shutil.copy(str(self.env_file), str(self._cwd / "my-env-file"))
 
         # Generate a unique name for the db host (we use the same strategy as docker-compose)
-        db_hostname = f"{self._cwd.name}_postgres_1"
+        db_hostname = f"{self._cwd.name}-postgres-1"
 
         env_file = f"""
             INMANTA_LSM_CONTAINER_DB_HOSTNAME={db_hostname}
             INMANTA_LSM_CONTAINER_DB_VERSION={self.postgres_version}
             INMANTA_LSM_CONTAINER_ORCHESTRATOR_IMAGE={self.orchestrator_image}
             INMANTA_LSM_CONTAINER_PUBLIC_KEY_FILE={self.public_key_file}
             INMANTA_LSM_CONTAINER_LICENSE_FILE={self.license_file}
@@ -219,28 +219,28 @@
 
     @property
     def orchestrator_port(self) -> int:
         return int(self.config.get("server", "bind-port", vars={"fallback": "8888"}))
 
     def _up(self) -> None:
         # Pull container images
-        cmd = ["docker-compose", "--verbose", "pull"]
+        cmd = ["docker-compose", f"--file={self.compose_file.name}", "--verbose", "pull"]
         run_cmd(cmd=cmd, cwd=self.cwd)
         # Starting the lab
-        cmd = ["docker-compose", "--verbose", "up", "-d"]
+        cmd = ["docker-compose", f"--file={self.compose_file.name}", "--verbose", "up", "-d"]
         run_cmd(cmd=cmd, cwd=self.cwd)
 
         # Getting the containers ids
-        cmd = ["docker-compose", "--verbose", "ps", "-q"]
+        cmd = ["docker-compose", f"--file={self.compose_file.name}", "--verbose", "ps", "-q"]
         stdout, _ = run_cmd(cmd=cmd, cwd=self.cwd)
         self._containers = stdout.strip("\n").split("\n")
 
     def _down(self) -> None:
         # Stopping the lab
-        cmd = ["docker-compose", "--verbose", "down", "-v"]
+        cmd = ["docker-compose", f"--file={self.compose_file.name}", "--verbose", "down", "-v"]
         run_cmd(cmd=cmd, cwd=self.cwd)
 
     def __enter__(self) -> "OrchestratorContainer":
         try:
             self._up()
             return self
         except subprocess.CalledProcessError as e:
```

### Comparing `pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/parameters.py` & `pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm/parameters.py`

 * *Files 3% similar despite different names*

```diff
@@ -165,15 +165,14 @@
     group=param_group,
 )
 
 inm_lsm_ctr_compose = PathTestParameter(
     argument="--lsm-ctr-compose-file",
     environment_variable="INMANTA_LSM_CONTAINER_COMPOSE_FILE",
     usage="The path to a docker-compose file, that should be used to setup an orchestrator",
-    default=Path(__file__).parent / "resources/docker-compose.yml",
     group=param_group,
     exists=True,
     is_file=True,
 )
 
 inm_lsm_ctr_image = StringTestParameter(
     argument="--lsm-ctr-image",
@@ -236,7 +235,20 @@
     environment_variable="INMANTA_LSM_CONTAINER_ENV_FILE",
     usage="A path to an env file that should be loaded in the container.",
     default=Path(__file__).parent / "resources/my-env-file",
     group=param_group,
     exists=True,
     is_file=True,
 )
+
+inm_lsm_dump = BooleanTestParameter(
+    argument="--lsm-dump-on-failure",
+    environment_variable="INMANTA_LSM_DUMP_ON_FAILURE",
+    usage=(
+        "Whether to create and save a support archive when a test fails.  The support "
+        "archive will be saved in the /tmp directory of the host running the test and will not be cleaned up.  "
+        "The value of this option can be overwritten for each test case individually by overwriting the "
+        "value of the remote_orchestrator_dump_on_failure fixture."
+    ),
+    default=False,
+    group=param_group,
+)
```

### Comparing `pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/plugin.py` & `pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm/plugin.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,26 +4,29 @@
     :copyright: 2020 Inmanta
     :contact: code@inmanta.com
     :license: Inmanta EULA
 """
 
 import logging
 import os
+import pathlib
+import re
 import shlex
 import shutil
+import tempfile
 import textwrap
 import time
 import uuid
-from typing import Dict, Generator, Iterator, Optional, Tuple, Union
+from typing import Any, Dict, Generator, Iterator, Optional, Tuple, Union
 from uuid import UUID
 
 import pkg_resources
 import pytest
 import pytest_inmanta.plugin
-import requests
+import pytest_inmanta.test_parameter
 from inmanta import module
 from packaging import version
 from pytest_inmanta.plugin import Project
 from pytest_inmanta.test_parameter import (
     ParameterNotSetException,
     ParameterType,
     TestParameter,
@@ -42,14 +45,15 @@
     inm_lsm_ctr_config,
     inm_lsm_ctr_db_version,
     inm_lsm_ctr_entitlement,
     inm_lsm_ctr_env,
     inm_lsm_ctr_image,
     inm_lsm_ctr_license,
     inm_lsm_ctr_pub_key,
+    inm_lsm_dump,
     inm_lsm_env,
     inm_lsm_env_name,
     inm_lsm_host,
     inm_lsm_no_clean,
     inm_lsm_no_halt,
     inm_lsm_partial_compile,
     inm_lsm_project_name,
@@ -74,14 +78,32 @@
     # the reset fixture clears the methods on the client. This import ensures that are
     # available.
     pass
 
 
 LOGGER = logging.getLogger(__name__)
 
+# https://docs.pytest.org/en/latest/example/simple.html#making-test-result-information-available-in-fixtures
+phase_report_key = pytest.StashKey[dict[str, pytest.CollectReport]]()
+
+
+@pytest.hookimpl(hookwrapper=True, tryfirst=True)
+def pytest_runtest_makereport(item: pytest.Item, call: pytest.CallInfo[None]) -> Generator[None, Any, None]:
+    # execute all other hooks to obtain the report object
+    # https://docs.pytest.org/en/latest/example/simple.html#making-test-result-information-available-in-fixtures
+    # https://github.com/pytest-dev/pytest/issues/6780#issue-568447972
+    outcome = yield
+
+    rep: pytest.TestReport = outcome.get_result()
+
+    # store test results for each phase of a call, which can
+    # be "setup", "call", "teardown"
+    default: dict = {}
+    item.stash.setdefault(phase_report_key, default)[rep.when] = rep
+
 
 @pytest.fixture(name="lsm_project")
 def lsm_project_fixture(
     monkeypatch: pytest.MonkeyPatch,
     project: pytest_inmanta.plugin.Project,
     remote_orchestrator_partial: bool,
 ) -> "lsm_project.LsmProject":
@@ -109,18 +131,53 @@
     Deploy, if the user required it, an orchestrator in a container locally.
     """
     enabled = inm_lsm_ctr.resolve(request.config)
     if not enabled:
         yield None
         return
 
+    orchestrator_image = inm_lsm_ctr_image.resolve(request.config)
+    latest_compose_file = pathlib.Path(__file__).parent / "resources/docker-compose.yml"
+    legacy_compose_file = pathlib.Path(__file__).parent / "resources/docker-compose-legacy.yml"
+    try:
+        compose_file = inm_lsm_ctr_compose.resolve(request.config)
+    except pytest_inmanta.test_parameter.ParameterNotSetException:
+        # The compose file is not set, we can then either use the default one, or
+        # the default legacy one (for <iso7.1).  To decide which one is the most
+        # appropriate, we parse the container image tag and extract the iso version
+        iso_major_version_match = re.fullmatch(
+            r".*\/service-orchestrator:(?P<tag>(?P<version>\d+(\.\d+)*)(\-dev)?|dev)",
+            orchestrator_image,
+        )
+        if not iso_major_version_match:
+            # The tag is not something we know, probably a custom container image, we then
+            # use the previous docker-compose file, as the custom container image probably
+            # expects it to stay like this.
+            LOGGER.info(
+                "Can not parse orchestrator image tag: %s.  Using legacy docker-compose file %s",
+                orchestrator_image,
+                str(legacy_compose_file),
+            )
+            compose_file = legacy_compose_file
+        elif iso_major_version_match.group("tag") == "dev":
+            # Latest dev, use the the latest compose file, this is always safe because we don't distribute this externally
+            compose_file = latest_compose_file
+        elif version.Version(iso_major_version_match.group("version")) >= version.Version("7.1"):
+            # The server has the --db-wait-time option
+            # https://github.com/inmanta/inmanta-core/pull/7217
+            compose_file = latest_compose_file
+        else:
+            # The image is not recent enough for the --db-wait-time option, we have to use the
+            # legacy docker-compose file which relies on the entrypoint to wait for the db
+            compose_file = legacy_compose_file
+
     LOGGER.debug("Deploying an orchestrator using docker")
     with OrchestratorContainer(
-        compose_file=inm_lsm_ctr_compose.resolve(request.config),
-        orchestrator_image=inm_lsm_ctr_image.resolve(request.config),
+        compose_file=compose_file,
+        orchestrator_image=orchestrator_image,
         postgres_version=inm_lsm_ctr_db_version.resolve(request.config),
         public_key_file=inm_lsm_ctr_pub_key.resolve(request.config),
         license_file=inm_lsm_ctr_license.resolve(request.config),
         entitlement_file=inm_lsm_ctr_entitlement.resolve(request.config),
         config_file=inm_lsm_ctr_config.resolve(request.config),
         env_file=inm_lsm_ctr_env.resolve(request.config),
     ) as orchestrator:
@@ -162,42 +219,25 @@
 @pytest.fixture(scope="session")
 def remote_orchestrator_host(
     remote_orchestrator_container: Optional[OrchestratorContainer],
     request: pytest.FixtureRequest,
 ) -> Tuple[str, int]:
     """
     Resolve the host and port options or take the values from the deployed docker orchestrator.
-    Tries to reach the orchestrator 10 times, if it fails, raises a RuntimeError.
-
     Returns a tuple containing the host and port at which the orchestrator has been reached.
     """
-    host, port = (
+    return (
         (
             inm_lsm_host.resolve(request.config),
             inm_lsm_srv_port.resolve(request.config),
         )
         if remote_orchestrator_container is None
         else (str(remote_orchestrator_container.orchestrator_ips[0]), remote_orchestrator_container.orchestrator_port)
     )
 
-    for _ in range(0, 10):
-        try:
-            http = "https" if inm_lsm_ssl.resolve(request.config) else "http"
-            response = requests.get(f"{http}://{host}:{port}/api/v1/serverstatus", timeout=2, verify=False)
-            response.raise_for_status()
-        except Exception as exc:
-            LOGGER.warning(str(exc))
-            time.sleep(1)
-            continue
-
-        if response.status_code == 200:
-            return host, port
-
-    raise RuntimeError(f"Couldn't reach the orchestrator at {host}:{port}")
-
 
 @pytest.fixture
 def remote_orchestrator_settings() -> Dict[str, Union[str, int, bool]]:
     """Override this fixture in your tests or conf test to set custom environment settings after cleanup. The supported
     settings are documented in https://docs.inmanta.com/inmanta-service-orchestrator/3/reference/environmentsettings.html
 
     The remote_orchestrator fixture already sets a number of non-default values to make the fixture work as it should.
@@ -267,14 +307,15 @@
     remote_orchestrator_environment: str,
     remote_orchestrator_host: tuple[str, int],
 ) -> RemoteOrchestrator:
     """
     This fixture allows to get the remote orchestrator object, without any of the initial cleanup.
     This allows to easily build helper tests that simply sync a remote environment with our local
     project, without clearing its service inventory.
+    Tries to reach the orchestrator 10 times, if it fails, raises a RuntimeError.
     """
     LOGGER.info("Setting up remote orchestrator")
 
     host, port = remote_orchestrator_host
 
     def get_optional_option(option: TestParameter[ParameterType]) -> Optional[ParameterType]:
         try:
@@ -309,15 +350,15 @@
         ):
             LOGGER.warning("SSL currently doesn't work with the default docker-compose file.")
 
     token = get_optional_option(inm_lsm_token)
     environment_name = get_optional_option(inm_lsm_env_name)
     project_name = get_optional_option(inm_lsm_project_name)
 
-    return RemoteOrchestrator(
+    remote_orchestrator = RemoteOrchestrator(
         OrchestratorEnvironment(
             id=UUID(remote_orchestrator_environment),
             name=environment_name,
             project=project_name,
         ),
         host=host,
         port=port,
@@ -327,14 +368,32 @@
         token=token,
         ca_cert=ca_cert,
         container_env=container_env,
         remote_shell=shlex.split(remote_shell) if remote_shell is not None else None,
         remote_host=remote_host,
     )
 
+    # Make sure the remote orchestrator is running
+    for _ in range(0, 10):
+        try:
+            # Try to get the status of the server, use the session object to set
+            # a custom timeout
+            remote_orchestrator.session.get("/api/v1/serverstatus", timeout=2).raise_for_status()
+            break
+        except Exception as exc:
+            LOGGER.warning(str(exc))
+            time.sleep(1)
+    else:
+        raise RuntimeError(f"Couldn't reach the orchestrator at {host}:{port}")
+
+    # Configure the environment on the remote orchestrator
+    remote_orchestrator.orchestrator_environment.configure_environment(remote_orchestrator.client)
+
+    return remote_orchestrator
+
 
 @pytest.fixture(scope="session")
 def remote_orchestrator_shared(
     request: pytest.FixtureRequest,
     project_shared: Project,
     remote_orchestrator_access: RemoteOrchestrator,
     remote_orchestrator_no_clean: bool,
@@ -406,20 +465,30 @@
     # Reload the config after the project fixture has run
     remote_orchestrator_shared.setup_config()
 
     yield project
 
 
 @pytest.fixture
+def remote_orchestrator_dump_on_failure(request: pytest.FixtureRequest) -> bool:
+    """
+    Whether we should produce a support archive in the case where the test fail.
+    """
+    return inm_lsm_dump.resolve(request.config)
+
+
+@pytest.fixture
 def remote_orchestrator(
     remote_orchestrator_shared: RemoteOrchestrator,
     remote_orchestrator_project: Project,
     remote_orchestrator_settings: Dict[str, Union[str, int, bool]],
     remote_orchestrator_partial: bool,
-) -> RemoteOrchestrator:
+    remote_orchestrator_dump_on_failure: bool,
+    request: pytest.FixtureRequest,
+) -> Iterator[RemoteOrchestrator]:
     # Clean environment, but keep project files
     remote_orchestrator_shared.clear_environment(soft=True)
 
     # set the defaults here and lets the fixture override specific values
     settings: Dict[str, Union[bool, str, int]] = {
         "auto_deploy": True,
         "server_compile": True,
@@ -439,15 +508,50 @@
         # orchestrator.
         remote_orchestrator_shared.client.set_setting(remote_orchestrator_shared.environment, k, v)
 
     # Make sure the environment is running
     result = remote_orchestrator_shared.client.resume_environment(remote_orchestrator_shared.environment)
     assert result.code in range(200, 300), str(result.result)
 
-    return remote_orchestrator_shared
+    yield remote_orchestrator_shared
+
+    # Check that status of the test that just ran
+    # https://docs.pytest.org/en/latest/example/simple.html#making-test-result-information-available-in-fixtures
+    report = request.node.stash[phase_report_key]
+    if "call" not in report or not report["call"].failed:
+        # The test didn't fail, we don't need to create a support archive
+        return
+
+    if not remote_orchestrator_dump_on_failure:
+        # We don't want to create a support archive on failure
+        return
+
+    # Check that the version of the remote orchestrator is recent enough to
+    # support the archive dump endpoint
+    if remote_orchestrator_shared.server_version < version.Version("6.4.0.dev"):
+        # This version is too old, we can't create the dump, log a warning and
+        # exit here
+        LOGGER.warning(
+            "Orchestrator version (%s) doesn't have the api call we need to dump the support archive: /api/v2/support",
+            remote_orchestrator_shared.server_version,
+        )
+        return
+
+    # Get the support archive from the orchestrator and save it to a temp file
+    # This archive is intentionally "leaked" so that anyone investigating the test
+    # failure can gather more information about the failure
+    # Download the file and stream the output to a file
+    _, tmp_file = tempfile.mkstemp(suffix="_support_archive.zip", prefix=f"{request.node.name}_")
+    with remote_orchestrator_shared.session.get("/api/v2/support", stream=True) as r:
+        r.raise_for_status()
+        with open(tmp_file, "wb") as f:
+            for chunk in r.iter_content(chunk_size=8192):
+                f.write(chunk)
+
+    LOGGER.info("Support archive of orchestrator has been saved at %s", tmp_file)
 
 
 @pytest.fixture
 def unittest_lsm(project: Project) -> Iterator[None]:
     """
     Adds a module named unittest_lsm to the project with a simple resource that always deploys successfully. The module is
     compatible with the remote orchestrator fixtures.
```

### Comparing `pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/remote_orchestrator.py` & `pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm/remote_orchestrator.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,27 +3,31 @@
 
     :copyright: 2020 Inmanta
     :contact: code@inmanta.com
     :license: Inmanta EULA
 """
 
 import dataclasses
+import functools
 import logging
 import pathlib
 import shlex
 import subprocess
 import typing
+import urllib.parse
 import uuid
 from pprint import pformat
 from uuid import UUID
 
 import inmanta.data.model
+import inmanta.model
 import inmanta.module
 import inmanta.protocol.endpoints
 import pydantic
+import requests
 from inmanta.agent import config as inmanta_config
 from inmanta.protocol.common import Result
 from packaging.version import Version
 
 from pytest_inmanta_lsm import managed_service_instance, retry_limited
 
 LOGGER = logging.getLogger(__name__)
@@ -236,27 +240,31 @@
                 "-l",
                 ssh_user,
             ]
 
         # Cached value of the name of the user we have on the remote orchestrator
         self._whoami: typing.Optional[str] = None
 
+        # requests.Session object allowing to interact with the orchestrator api.  This is
+        # useful for the api endpoints that can not be reached using the "native" inmanta client.
+        self._session: typing.Optional[requests.Session] = None
+
         # Allow to change the remote host, as the access to the remote shell or to the
         # remote api might be different (i.e. podman exec -i <container-name> vs curl <container-ip>)
         self.remote_host = remote_host if remote_host is not None else host
 
         # Build the client once, it loads the config on every call
         self.client = inmanta.protocol.endpoints.SyncClient("client")
         self.async_client = inmanta.protocol.endpoints.Client("client")
 
         # Setting up the client when the config is loaded
         self.setup_config()
 
-        self.orchestrator_environment.configure_environment(self.client)
-        self.server_version = self._get_server_version()
+        # Save the version of the remote orchestrator server
+        self._server_version: typing.Optional[Version] = None
 
         # The path on the remote orchestrator where the project will be synced
         self.remote_project_path = pathlib.Path(
             "/var/lib/inmanta/server/environments/",
             str(self.environment),
         )
         self.remote_project_cache_path = self.remote_project_path.with_name(self.remote_project_path.name + "_cache")
@@ -291,14 +299,79 @@
             if self.ssl:
                 inmanta_config.Config.set(section, "ssl", str(self.ssl))
                 if self.ca_cert:
                     inmanta_config.Config.set(section, "ssl_ca_cert_file", self.ca_cert)
             if self.token:
                 inmanta_config.Config.set(section, "token", self.token)
 
+    @property
+    def session(self) -> requests.Session:
+        """
+        Get a requests.Session object pre-configured to communicate with the remote
+        orchestrator.  The session already handles authentication and ssl for the user.
+        It also sets up a default base_url, matching the protocol, host and port of the
+        remote orchestrator (as specified in the inmanta config).  To use the client,
+        you can then simply do:
+
+            .. code-block:: python
+
+                with remote_orchestrator.session.get("/api/v2/support", stream=True) as r:
+                    r.raise_for_status()
+                    with open("support_archive.zip", "wb") as f:
+                        for chunk in r.iter_content(chunk_size=8192):
+                            f.write(chunk)
+
+        For most api calls, it will be easier to use the self.request and self.sync_request
+        methods.  The requests.Session object gives you however more flexibility that the
+        for-mentioned methods, allowing to also interact with some api endpoints not supported
+        by the native inmanta client helper.
+        """
+        if self._session is not None:
+            # Return the existing session object
+            return self._session
+
+        # Create a new session towards the orchestrator
+        self._session = requests.Session()
+
+        # Read the config to know where the orchestrator is, and how we should
+        # communicate with it
+        token: typing.Optional[str] = inmanta_config.Config.get("client_rest_transport", "token", None)
+        ca_certs: typing.Optional[str] = inmanta_config.Config.get("client_rest_transport", "ssl_ca_cert_file", None)
+        port: int = int(inmanta_config.Config.get("client_rest_transport", "port") or 8888)
+        host: str = inmanta_config.Config.get("client_rest_transport", "host") or "localhost"
+        ssl: bool = inmanta_config.Config.getboolean("client_rest_transport", "ssl", False)
+        protocol = "https" if ssl else "http"
+
+        # Setup authentication (if required)
+        if token is not None:
+            self._session.headers["Authorization"] = f"Bearer {token}"
+
+        # Setup ca_certs (if required)
+        if ca_certs is not None:
+            self._session.cert = ca_certs
+
+        # Setup base url for all requests made
+        def request_with_base_url(
+            request: typing.Callable, base_url: str, method: str, url: str, *args: object, **kwargs: object
+        ) -> requests.Response:
+            return request(
+                method,
+                urllib.parse.urljoin(base_url, url),
+                *args,
+                **kwargs,
+            )
+
+        self._session.request = functools.partial(  # type: ignore[method-assign]
+            request_with_base_url,
+            self._session.request,
+            f"{protocol}://{host}:{port}",
+        )
+
+        return self._session
+
     @typing.overload
     async def request(self, method: str, returned_type: None = None, **kwargs: object) -> None:
         pass
 
     @typing.overload
     async def request(self, method: str, returned_type: type[T], **kwargs: object) -> T:
         pass
@@ -325,26 +398,59 @@
                 return pydantic.TypeAdapter(returned_type).validate_python(response.result["data"])
             except AttributeError:
                 # Handle pydantic v1
                 return pydantic.parse_obj_as(returned_type, response.result["data"])
         else:
             return None
 
-    def _get_server_version(self) -> Version:
+    @typing.overload
+    def sync_request(self, method: str, returned_type: None = None, **kwargs: object) -> None:
+        pass
+
+    @typing.overload
+    def sync_request(self, method: str, returned_type: type[T], **kwargs: object) -> T:
+        pass
+
+    def sync_request(
+        self,
+        method: str,
+        returned_type: typing.Optional[type[T]] = None,
+        **kwargs: object,
+    ) -> typing.Optional[T]:
+        """
+        Helper method to send a request to the orchestrator, which we expect to succeed with 20X code and
+        return an object of a given type.
+
+        :param method: The name of the method to execute
+        :param returned_type: The type of the object that the api should return
+        :param **kwargs: Parameters to pass to the method we are calling
+        """
+        response: Result = getattr(self.client, method)(**kwargs)
+        assert response.code in range(200, 300), str(response.result)
+        if returned_type is not None:
+            assert response.result is not None, str(response)
+            try:
+                return pydantic.TypeAdapter(returned_type).validate_python(response.result["data"])
+            except AttributeError:
+                # Handle pydantic v1
+                return pydantic.parse_obj_as(returned_type, response.result["data"])
+        else:
+            return None
+
+    @property
+    def server_version(self) -> Version:
         """
-        Get the version of the remote orchestrator
+        Get the version of the remote orchestrator.  The version is not expected to change
+        for the duration of the test case, so that value is cached after the first call.
         """
-        server_status: Result = self.client.get_server_status()
-        if server_status.code != 200:
-            raise Exception(f"Failed to get server status for {self.host}")
-        try:
-            assert server_status.result is not None
-            return Version(server_status.result["data"]["version"])
-        except (KeyError, TypeError):
-            raise Exception(f"Unexpected response for server status API call: {server_status.result}")
+        if self._server_version is None:
+            status = self.sync_request("get_server_status", inmanta.data.model.StatusResponse)
+            self._server_version = Version(status.version)
+            LOGGER.debug("Remote orchestrator has version %s", self._server_version)
+        return self._server_version
 
     @property
     def remote_user(self) -> str:
         """
         Execute the whoami command in the remote shell, to discover which user we have access to
         in this shell and returns its name.  The result is cached, as we don't expect the remote
         shell to change within the lifecycle of this remote orchestrator object.
```

### Comparing `pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/remote_service_instance.py` & `pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm/remote_service_instance.py`

 * *Files identical despite different names*

### Comparing `pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/remote_service_instance.pyi` & `pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm/remote_service_instance.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -61,27 +61,28 @@
         target_version: typing.Optional[int] = None,
         *,
         bad_states: typing.Optional[typing.Collection[str]] = None,
         timeout: typing.Optional[float] = None,
         start_version: int,
     ) -> model.ServiceInstance:
         """
-        Wait for this service instance to reach the desired target state.
+        Wait for this service instance to reach the desired target state.  Returns a ServiceInstance
+        object that is in the state that was waited for.
 
         :param target_state: The state we want to wait our service instance to reach.
         :param target_version: The version the service is expected to be in once we reached the target
             state.  If we reach this version but not the target state or the opposite, the state will
             not be a match.
         :param bad_states: A collection of bad state that should interrupt the waiting
             process and trigger a BadStateError.  If set to None, default to self.ALL_BAD_STATES.
         :param timeout: The time, in seconds, after which we should stop waiting and
             raise a StateTimeoutError.  If set to None, uses the DEFAULT_TIMEOUT attribute of the
             object.
-        :param start_version: The initial version we know the service has been in, we only
-            look for versions after this one.
+        :param start_version: A service version from which we should search for the target state.
+            This version and all of the prior versions will not be checked for a match as the target state.
         :raises BadStateError: If the instance went into a bad state
         :raises StateTimeoutError: If the timeout is reached while waiting for the desired state
         :raises VersionExceededError: If version is provided and the current state goes past it
         """
 
     def create(
         self,
```

### Comparing `pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/remote_service_instance_async.py` & `pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm/remote_service_instance_async.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,45 @@
 
 LOGGER = logging.getLogger(__name__)
 
 
 T = typing.TypeVar("T")
 
 
+def get_service_instance_from_log(log: model.ServiceInstanceLog) -> model.ServiceInstance:
+    """
+    This helper method allow to convert of a ServiceInstanceLog into the corresponding ServiceInstance.
+    The method `to_service_instance()` was only recently added to inmanta_lsm, this offers compatibility
+    with older versions of the orchestrator.
+
+    :param log: The ServiceInstanceLog to convert to a ServiceInstance object.
+    """
+    try:
+        return log.to_service_instance()
+    except AttributeError:
+        return model.ServiceInstance(
+            id=log.service_instance_id,
+            environment=log.environment,
+            service_entity=log.service_entity,
+            version=log.version,
+            config=log.config,
+            state=log.state,
+            candidate_attributes=log.candidate_attributes,
+            active_attributes=log.active_attributes,
+            rollback_attributes=log.rollback_attributes,
+            created_at=log.created_at,
+            last_updated=log.last_updated,
+            callback=log.callback,
+            deleted=log.deleted,
+            deployment_progress=None,
+            service_identity_attribute_value=log.service_identity_attribute_value,
+            referenced_by=None,
+        )
+
+
 class RemoteServiceInstanceError(RuntimeError, typing.Generic[T]):
     """
     Base exception for error raised by a managed service instance.
     """
 
     def __init__(self, instance: T, *args: object) -> None:
         super().__init__(*args)
@@ -110,15 +141,14 @@
         self.target_version = target_version
         self.timeout = timeout
         self.last_state = last_state
         self.last_version = last_version
 
 
 class RemoteServiceInstance:
-
     DEFAULT_TIMEOUT = 600.0
     RETRY_INTERVAL = 5.0
     CREATE_FLOW_BAD_STATES: list[str] = ["rejected", "failed"]
 
     UPDATE_FLOW_BAD_STATES: list[str] = [
         "update_start_failed",
         "update_acknowledged_failed",
@@ -219,27 +249,28 @@
         target_version: typing.Optional[int] = None,
         *,
         bad_states: typing.Optional[typing.Collection[str]] = None,
         timeout: typing.Optional[float] = None,
         start_version: int,
     ) -> model.ServiceInstance:
         """
-        Wait for this service instance to reach the desired target state.
+        Wait for this service instance to reach the desired target state.  Returns a ServiceInstance
+        object that is in the state that was waited for.
 
         :param target_state: The state we want to wait our service instance to reach.
         :param target_version: The version the service is expected to be in once we reached the target
             state.  If we reach this version but not the target state or the opposite, the state will
             not be a match.
         :param bad_states: A collection of bad state that should interrupt the waiting
             process and trigger a BadStateError.  If set to None, default to self.ALL_BAD_STATES.
         :param timeout: The time, in seconds, after which we should stop waiting and
             raise a StateTimeoutError.  If set to None, uses the DEFAULT_TIMEOUT attribute of the
             object.
-        :param start_version: The initial version we know the service has been in, we only
-            look for versions after this one.
+        :param start_version: A service version from which we should search for the target state.
+            This version and all of the prior versions will not be checked for a match as the target state.
         :raises BadStateError: If the instance went into a bad state
         :raises StateTimeoutError: If the timeout is reached while waiting for the desired state
         :raises VersionExceededError: If version is provided and the current state goes past it
         """
         if timeout is None:
             timeout = self.DEFAULT_TIMEOUT
 
@@ -285,15 +316,15 @@
                 await self.history(since_version=last_version),
                 key=lambda log: log.version,
             ):
                 try:
                     # Always skip the last version, as it is either our start version, or a
                     # version we checked on the previous iteration.
                     if log.version > last_version and is_done(log):
-                        return await self.get()
+                        return get_service_instance_from_log(log)
                 except BadStateError:
                     # We encountered a bad state, print the diagnosis then quit
                     diagnosis = await self.diagnose(version=log.version)
                     LOGGER.info(
                         "Service instance %s reached bad state %s: \n%s",
                         self.instance_name,
                         log.state,
```

### Comparing `pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/resources/docker-compose.yml` & `pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm/resources/docker-compose-legacy.yml`

 * *Files identical despite different names*

### Comparing `pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/resources/my-server-conf.cfg` & `pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm/resources/my-server-conf.cfg`

 * *Files identical despite different names*

### Comparing `pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/resources/setup_project.py` & `pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm/resources/setup_project.py`

 * *Files identical despite different names*

### Comparing `pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/util.py` & `pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm/util.py`

 * *Files identical despite different names*

### Comparing `pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/wait_for_state.py` & `pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm/wait_for_state.py`

 * *Files identical despite different names*

### Comparing `pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm.egg-info/PKG-INFO` & `pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-inmanta-lsm
-Version: 3.3.0
+Version: 3.4.0
 Summary: Common fixtures for inmanta LSM related modules
 Home-page: https://github.com/inmanta/pytest-inmanta-lsm
 Author: Inmanta
 Author-email: code@inmanta.com
 License: inmanta EULA
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
@@ -65,32 +65,39 @@
 
     # Test the synchronous service instance class
     instance = remote_service_instance.RemoteServiceInstance(
         remote_orchestrator=remote_orchestrator,
         service_entity_name=SERVICE_NAME,
     )
 
-    # Create the service instance and stop waiting in a transient state
+    # Create the service instance and stop waiting in a transient state, and get the service instance
+    # as it is in the target state.
     created = instance.create(
         {
             "router_ip": "10.1.9.17",
             "interface_name": "eth1",
             "address": "10.0.0.254/24",
             "vlan_id": 14,
         },
         wait_for_state="creating",
         timeout=60,
     )
 
-    # Wait for up state, we provide here the version from which we should follow the
-    # service, which is the version in which we last stopped following the service.  This
-    # guarantees that we don't "miss" the target state, in case it is a transient one, and
-    # don't confuse the start state for the target one in case it is the same one.
-    # The start version should always be the last version in which we know our service has
-    # been, BEFORE the target state we expect our service to go into.
+    # Wait for up state.  The method will check each version that the service goes through,
+    # starting AFTER the start_version if it is provided, or the current version of the service
+    # if start_version is not provided.  As soon as a version is a match, the helper will return the
+    # service instance at this given state.
+    # It is important to provide the correct start_version to avoid falling in any of these situations:
+    # 1. We could miss the target state, if at the moment we start waiting for the target state, it is
+    #    already reached and no start_version is provided (as we would start looking AFTER the current
+    #    version).
+    # 2. We could select the wrong target state if we start looking at too old versions (in the case of
+    #    an update for example, we might mistake the source up state for the target one).
+    # In this example, we start after the version of the creating state, as we know it is before our up
+    # state.
     instance.wait_for_state(
         target_state="up",
         start_version=created.version,
         timeout=60,
     )
 
     # Delete the instance
@@ -367,14 +374,21 @@
   --lsm-ssl             [True | False] Choose whether to use SSL/TLS or not when
                         connecting to the remote orchestrator. (overrides
                         INMANTA_LSM_SSL, defaults to False)
   --lsm-token
                         The token used to authenticate to the remote
                         orchestrator when authentication is enabled. (overrides
                         INMANTA_LSM_TOKEN)
+  --lsm-dump-on-failure
+                        Whether to create and save a support archive when a test fails.
+                        The support archive will be saved in the /tmp directory of the
+                        host running the test and will not be cleaned up. The value of
+                        this option can be overwritten for each test case individually
+                        by overwriting the value of the remote_orchestrator_dump_on_failure
+                        fixture. (overrides INMANTA_LSM_DUMP_ON_FAILURE, defaults to False)
 
 ```
 
 ## Running tests
 
 ### How the test suite is structured
```

### Comparing `pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm.egg-info/SOURCES.txt` & `pytest_inmanta_lsm-3.4.0/src/pytest_inmanta_lsm.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 src/pytest_inmanta_lsm/__init__.py
 src/pytest_inmanta_lsm/exceptions.py
 src/pytest_inmanta_lsm/failed_resources_logs.py
+src/pytest_inmanta_lsm/load_generator.py
 src/pytest_inmanta_lsm/lsm_project.py
 src/pytest_inmanta_lsm/managed_service_instance.py
 src/pytest_inmanta_lsm/orchestrator_container.py
 src/pytest_inmanta_lsm/parameters.py
 src/pytest_inmanta_lsm/plugin.py
 src/pytest_inmanta_lsm/py.typed
 src/pytest_inmanta_lsm/remote_orchestrator.py
@@ -22,14 +23,15 @@
 src/pytest_inmanta_lsm/wait_for_state.py
 src/pytest_inmanta_lsm.egg-info/PKG-INFO
 src/pytest_inmanta_lsm.egg-info/SOURCES.txt
 src/pytest_inmanta_lsm.egg-info/dependency_links.txt
 src/pytest_inmanta_lsm.egg-info/entry_points.txt
 src/pytest_inmanta_lsm.egg-info/requires.txt
 src/pytest_inmanta_lsm.egg-info/top_level.txt
+src/pytest_inmanta_lsm/resources/docker-compose-legacy.yml
 src/pytest_inmanta_lsm/resources/docker-compose.yml
 src/pytest_inmanta_lsm/resources/my-env-file
 src/pytest_inmanta_lsm/resources/my-server-conf.cfg
 src/pytest_inmanta_lsm/resources/setup_project.py
 tests/test_basic_example.py
 tests/test_containerized_orchestrator.py
 tests/test_partial.py
```

### Comparing `pytest_inmanta_lsm-3.3.0/tests/test_partial.py` & `pytest_inmanta_lsm-3.4.0/tests/test_partial.py`

 * *Files identical despite different names*

