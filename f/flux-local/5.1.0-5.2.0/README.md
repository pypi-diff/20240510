# Comparing `tmp/flux_local-5.1.0.tar.gz` & `tmp/flux_local-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flux_local-5.1.0.tar", last modified: Sat Apr 27 13:38:37 2024, max compression
+gzip compressed data, was "flux_local-5.2.0.tar", last modified: Fri May 10 20:10:03 2024, max compression
```

## Comparing `flux_local-5.1.0.tar` & `flux_local-5.2.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:38:37.293294 flux_local-5.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-27 13:38:33.000000 flux_local-5.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12891 2024-04-27 13:38:37.293294 flux_local-5.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12108 2024-04-27 13:38:33.000000 flux_local-5.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:38:37.285294 flux_local-5.1.0/flux_local/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-27 13:38:33.000000 flux_local-5.1.0/flux_local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-04-27 13:38:33.000000 flux_local-5.1.0/flux_local/command.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-27 13:38:33.000000 flux_local-5.1.0/flux_local/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-27 13:38:33.000000 flux_local-5.1.0/flux_local/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    27320 2024-04-27 13:38:33.000000 flux_local-5.1.0/flux_local/git_repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7896 2024-04-27 13:38:33.000000 flux_local-5.1.0/flux_local/helm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-27 13:38:33.000000 flux_local-5.1.0/flux_local/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     9552 2024-04-27 13:38:33.000000 flux_local-5.1.0/flux_local/kustomize.py
--rw-r--r--   0 runner    (1001) docker     (127)    22676 2024-04-27 13:38:33.000000 flux_local-5.1.0/flux_local/manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:38:37.289294 flux_local-5.1.0/flux_local/tool/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-27 13:38:33.000000 flux_local-5.1.0/flux_local/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-04-27 13:38:33.000000 flux_local-5.1.0/flux_local/tool/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-27 13:38:33.000000 flux_local-5.1.0/flux_local/tool/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)    16733 2024-04-27 13:38:33.000000 flux_local-5.1.0/flux_local/tool/diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-27 13:38:33.000000 flux_local-5.1.0/flux_local/tool/flux_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-27 13:38:33.000000 flux_local-5.1.0/flux_local/tool/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-04-27 13:38:33.000000 flux_local-5.1.0/flux_local/tool/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     7549 2024-04-27 13:38:33.000000 flux_local-5.1.0/flux_local/tool/selector.py
--rw-r--r--   0 runner    (1001) docker     (127)    14249 2024-04-27 13:38:33.000000 flux_local-5.1.0/flux_local/tool/test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10469 2024-04-27 13:38:33.000000 flux_local-5.1.0/flux_local/tool/visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8582 2024-04-27 13:38:33.000000 flux_local-5.1.0/flux_local/values.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:38:37.293294 flux_local-5.1.0/flux_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12891 2024-04-27 13:38:37.000000 flux_local-5.1.0/flux_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-27 13:38:37.000000 flux_local-5.1.0/flux_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 13:38:37.000000 flux_local-5.1.0/flux_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-27 13:38:37.000000 flux_local-5.1.0/flux_local.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-27 13:38:37.000000 flux_local-5.1.0/flux_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-27 13:38:37.000000 flux_local-5.1.0/flux_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-27 13:38:37.293294 flux_local-5.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-27 13:38:33.000000 flux_local-5.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:38:37.289294 flux_local-5.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-27 13:38:33.000000 flux_local-5.1.0/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     8364 2024-04-27 13:38:33.000000 flux_local-5.1.0/tests/test_git_repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-27 13:38:33.000000 flux_local-5.1.0/tests/test_helm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-27 13:38:33.000000 flux_local-5.1.0/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-04-27 13:38:33.000000 flux_local-5.1.0/tests/test_kustomize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-04-27 13:38:33.000000 flux_local-5.1.0/tests/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)    16462 2024-04-27 13:38:33.000000 flux_local-5.1.0/tests/test_values.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:38:37.293294 flux_local-5.1.0/tests/tool/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-27 13:38:33.000000 flux_local-5.1.0/tests/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-27 13:38:33.000000 flux_local-5.1.0/tests/tool/test_build.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-27 13:38:33.000000 flux_local-5.1.0/tests/tool/test_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-27 13:38:33.000000 flux_local-5.1.0/tests/tool/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-27 13:38:33.000000 flux_local-5.1.0/tests/tool/test_diff_hr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-27 13:38:33.000000 flux_local-5.1.0/tests/tool/test_diff_ks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-27 13:38:33.000000 flux_local-5.1.0/tests/tool/test_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-27 13:38:33.000000 flux_local-5.1.0/tests/tool/test_get_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-27 13:38:33.000000 flux_local-5.1.0/tests/tool/test_get_hr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-27 13:38:33.000000 flux_local-5.1.0/tests/tool/test_get_ks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-27 13:38:33.000000 flux_local-5.1.0/tests/tool/test_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:10:03.689629 flux_local-5.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-10 20:09:56.000000 flux_local-5.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12891 2024-05-10 20:10:03.689629 flux_local-5.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12108 2024-05-10 20:09:56.000000 flux_local-5.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:10:03.681629 flux_local-5.2.0/flux_local/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-10 20:09:56.000000 flux_local-5.2.0/flux_local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-10 20:09:56.000000 flux_local-5.2.0/flux_local/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-10 20:09:56.000000 flux_local-5.2.0/flux_local/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-10 20:09:56.000000 flux_local-5.2.0/flux_local/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27576 2024-05-10 20:09:56.000000 flux_local-5.2.0/flux_local/git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7896 2024-05-10 20:09:56.000000 flux_local-5.2.0/flux_local/helm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-10 20:09:56.000000 flux_local-5.2.0/flux_local/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9552 2024-05-10 20:09:56.000000 flux_local-5.2.0/flux_local/kustomize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22676 2024-05-10 20:09:56.000000 flux_local-5.2.0/flux_local/manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:10:03.685629 flux_local-5.2.0/flux_local/tool/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-10 20:09:56.000000 flux_local-5.2.0/flux_local/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-05-10 20:09:56.000000 flux_local-5.2.0/flux_local/tool/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-05-10 20:09:56.000000 flux_local-5.2.0/flux_local/tool/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16948 2024-05-10 20:09:56.000000 flux_local-5.2.0/flux_local/tool/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-10 20:09:56.000000 flux_local-5.2.0/flux_local/tool/flux_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-10 20:09:56.000000 flux_local-5.2.0/flux_local/tool/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-05-10 20:09:56.000000 flux_local-5.2.0/flux_local/tool/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7549 2024-05-10 20:09:56.000000 flux_local-5.2.0/flux_local/tool/selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14249 2024-05-10 20:09:56.000000 flux_local-5.2.0/flux_local/tool/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10469 2024-05-10 20:09:56.000000 flux_local-5.2.0/flux_local/tool/visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8582 2024-05-10 20:09:56.000000 flux_local-5.2.0/flux_local/values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:10:03.689629 flux_local-5.2.0/flux_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12891 2024-05-10 20:10:03.000000 flux_local-5.2.0/flux_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-10 20:10:03.000000 flux_local-5.2.0/flux_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 20:10:03.000000 flux_local-5.2.0/flux_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-10 20:10:03.000000 flux_local-5.2.0/flux_local.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-10 20:10:03.000000 flux_local-5.2.0/flux_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-10 20:10:03.000000 flux_local-5.2.0/flux_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-10 20:10:03.689629 flux_local-5.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-10 20:09:56.000000 flux_local-5.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:10:03.685629 flux_local-5.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-10 20:09:56.000000 flux_local-5.2.0/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8364 2024-05-10 20:09:56.000000 flux_local-5.2.0/tests/test_git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-05-10 20:09:56.000000 flux_local-5.2.0/tests/test_helm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-10 20:09:56.000000 flux_local-5.2.0/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-05-10 20:09:56.000000 flux_local-5.2.0/tests/test_kustomize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-10 20:09:56.000000 flux_local-5.2.0/tests/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16462 2024-05-10 20:09:56.000000 flux_local-5.2.0/tests/test_values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:10:03.689629 flux_local-5.2.0/tests/tool/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-10 20:09:56.000000 flux_local-5.2.0/tests/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-10 20:09:56.000000 flux_local-5.2.0/tests/tool/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-10 20:09:56.000000 flux_local-5.2.0/tests/tool/test_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-10 20:09:56.000000 flux_local-5.2.0/tests/tool/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-05-10 20:09:56.000000 flux_local-5.2.0/tests/tool/test_diff_hr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-10 20:09:56.000000 flux_local-5.2.0/tests/tool/test_diff_ks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-05-10 20:09:56.000000 flux_local-5.2.0/tests/tool/test_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-10 20:09:56.000000 flux_local-5.2.0/tests/tool/test_get_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-10 20:09:56.000000 flux_local-5.2.0/tests/tool/test_get_hr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-10 20:09:56.000000 flux_local-5.2.0/tests/tool/test_get_ks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-10 20:09:56.000000 flux_local-5.2.0/tests/tool/test_test.py
```

### Comparing `flux_local-5.1.0/LICENSE` & `flux_local-5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flux_local-5.1.0/PKG-INFO` & `flux_local-5.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-local
-Version: 5.1.0
+Version: 5.2.0
 Summary: flux-local is a python library and set of tools for managing a flux gitops repository, with validation steps to help improve quality of commits, PRs, and general local testing.
 Home-page: https://github.com/allenporter/flux-local
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.10
```

### Comparing `flux_local-5.1.0/README.md` & `flux_local-5.2.0/README.md`

 * *Files identical despite different names*

### Comparing `flux_local-5.1.0/flux_local/command.py` & `flux_local-5.2.0/flux_local/command.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.1.0/flux_local/context.py` & `flux_local-5.2.0/flux_local/context.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.1.0/flux_local/exceptions.py` & `flux_local-5.2.0/flux_local/exceptions.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.1.0/flux_local/git_repo.py` & `flux_local-5.2.0/flux_local/git_repo.py`

 * *Files 1% similar despite different names*

```diff
@@ -768,24 +768,28 @@
                             None,
                         )
 
         return Manifest(clusters=clusters)
 
 
 @contextlib.contextmanager
-def create_worktree(repo: git.repo.Repo) -> Generator[Path, None, None]:
+def create_worktree(repo: git.repo.Repo, existing_branch: str | None = None) -> Generator[Path, None, None]:
     """Create a ContextManager for a new git worktree in the current repo.
 
     This is used to get a fork of the current repo without any local changes
     in order to produce a diff.
+    Specifying existing_branch allows  to compare the current state with the existing branch.
     """
     orig = os.getcwd()
     with tempfile.TemporaryDirectory() as tmp_dir:
         _LOGGER.debug("Creating worktree in %s", tmp_dir)
-        # Add --detach to avoid creating a branch since we will not make modifications
-        repo.git.worktree("add", "--detach", str(tmp_dir))
+        if existing_branch is None:
+            # Add --detach to avoid creating a branch since we will not make modifications
+            repo.git.worktree("add", "--detach", str(tmp_dir))
+        else:
+            repo.git.worktree("add", str(tmp_dir), existing_branch)
         os.chdir(tmp_dir)
         yield Path(tmp_dir)
     _LOGGER.debug("Restoring to %s", orig)
     # The temp directory should now be removed and this prunes the worktree
     repo.git.worktree("prune")
     os.chdir(orig)
```

### Comparing `flux_local-5.1.0/flux_local/helm.py` & `flux_local-5.2.0/flux_local/helm.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.1.0/flux_local/image.py` & `flux_local-5.2.0/flux_local/image.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.1.0/flux_local/kustomize.py` & `flux_local-5.2.0/flux_local/kustomize.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.1.0/flux_local/manifest.py` & `flux_local-5.2.0/flux_local/manifest.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.1.0/flux_local/tool/build.py` & `flux_local-5.2.0/flux_local/tool/build.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.1.0/flux_local/tool/diagnostics.py` & `flux_local-5.2.0/flux_local/tool/diagnostics.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.1.0/flux_local/tool/diff.py` & `flux_local-5.2.0/flux_local/tool/diff.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,14 +194,23 @@
     args.add_argument(
         "--path-orig",
         help="Path to compare against, or creates a work tree if not specified",
         type=pathlib.Path,
         default=None,
         nargs="?",
     )
+
+    args.add_argument(
+        "--branch-orig",
+        help="Branch to compare against using worktree",
+        type=str,
+        default=None,
+        nargs="?",
+    )
+
     args.add_argument(
         "--strip-attrs",
         help="Labels or annotations to strip from the diff",
         type=_CSV,
     )
     args.add_argument(
         "--limit-bytes",
@@ -221,15 +230,15 @@
     This will create a new worktree by default, or use the path in the flags
     which is useful when run from CI.
     """
     if path_orig := kwargs.get("path_orig"):
         yield git_repo.PathSelector(path_orig, sources=kwargs.get("sources"))
         return
 
-    with git_repo.create_worktree(selector.repo) as worktree:
+    with git_repo.create_worktree(selector.repo, existing_branch=kwargs.get("branch_orig")) as worktree:
         yield git_repo.PathSelector(pathlib.Path(worktree) / selector.relative_path)
 
 
 class DiffKustomizationAction:
     """Flux-local diff for Kustomizations."""
 
     @classmethod
```

### Comparing `flux_local-5.1.0/flux_local/tool/flux_local.py` & `flux_local-5.2.0/flux_local/tool/flux_local.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.1.0/flux_local/tool/format.py` & `flux_local-5.2.0/flux_local/tool/format.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.1.0/flux_local/tool/get.py` & `flux_local-5.2.0/flux_local/tool/get.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.1.0/flux_local/tool/selector.py` & `flux_local-5.2.0/flux_local/tool/selector.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.1.0/flux_local/tool/test.py` & `flux_local-5.2.0/flux_local/tool/test.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.1.0/flux_local/tool/visitor.py` & `flux_local-5.2.0/flux_local/tool/visitor.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.1.0/flux_local/values.py` & `flux_local-5.2.0/flux_local/values.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.1.0/flux_local.egg-info/PKG-INFO` & `flux_local-5.2.0/flux_local.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-local
-Version: 5.1.0
+Version: 5.2.0
 Summary: flux-local is a python library and set of tools for managing a flux gitops repository, with validation steps to help improve quality of commits, PRs, and general local testing.
 Home-page: https://github.com/allenporter/flux-local
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.10
```

### Comparing `flux_local-5.1.0/flux_local.egg-info/SOURCES.txt` & `flux_local-5.2.0/flux_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flux_local-5.1.0/setup.cfg` & `flux_local-5.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flux-local
-version = 5.1.0
+version = 5.2.0
 description = flux-local is a python library and set of tools for managing a flux gitops repository, with validation steps to help improve quality of commits, PRs, and general local testing.
 long_description = file: README.md
 long_description_content_type = text/markdown
 prodid = github.com/allenporter/flux-local
 url = https://github.com/allenporter/flux-local
 author = Allen Porter
 author_email = allen.porter@gmail.com
```

### Comparing `flux_local-5.1.0/tests/test_command.py` & `flux_local-5.2.0/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.1.0/tests/test_git_repo.py` & `flux_local-5.2.0/tests/test_git_repo.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.1.0/tests/test_helm.py` & `flux_local-5.2.0/tests/test_helm.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.1.0/tests/test_image.py` & `flux_local-5.2.0/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.1.0/tests/test_kustomize.py` & `flux_local-5.2.0/tests/test_kustomize.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.1.0/tests/test_manifest.py` & `flux_local-5.2.0/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.1.0/tests/test_values.py` & `flux_local-5.2.0/tests/test_values.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.1.0/tests/tool/test_build.py` & `flux_local-5.2.0/tests/tool/test_build.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.1.0/tests/tool/test_diagnostics.py` & `flux_local-5.2.0/tests/tool/test_diagnostics.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.1.0/tests/tool/test_diff.py` & `flux_local-5.2.0/tests/tool/test_diff.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.1.0/tests/tool/test_diff_hr.py` & `flux_local-5.2.0/tests/tool/test_diff_hr.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.1.0/tests/tool/test_diff_ks.py` & `flux_local-5.2.0/tests/tool/test_diff_ks.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.1.0/tests/tool/test_format.py` & `flux_local-5.2.0/tests/tool/test_format.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.1.0/tests/tool/test_get_cluster.py` & `flux_local-5.2.0/tests/tool/test_get_cluster.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.1.0/tests/tool/test_get_hr.py` & `flux_local-5.2.0/tests/tool/test_get_hr.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.1.0/tests/tool/test_get_ks.py` & `flux_local-5.2.0/tests/tool/test_get_ks.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.1.0/tests/tool/test_test.py` & `flux_local-5.2.0/tests/tool/test_test.py`

 * *Files identical despite different names*

