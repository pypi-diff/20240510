# Comparing `tmp/batchfetch-1.0.7.tar.gz` & `tmp/batchfetch-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batchfetch-1.0.7.tar", last modified: Mon May  6 02:42:52 2024, max compression
+gzip compressed data, was "batchfetch-1.0.8.tar", last modified: Thu May  9 20:56:45 2024, max compression
```

## Comparing `batchfetch-1.0.7.tar` & `batchfetch-1.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-06 02:42:52.363884 batchfetch-1.0.7/
--rw-r--r--   0 dev        (455) work      (1000)    35149 2024-05-06 02:42:44.000000 batchfetch-1.0.7/LICENSE
--rw-r--r--   0 dev        (455) work      (1000)     4337 2024-05-06 02:42:52.363884 batchfetch-1.0.7/PKG-INFO
--rw-r--r--   0 dev        (455) work      (1000)     3560 2024-05-06 02:42:44.000000 batchfetch-1.0.7/README.md
-drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-06 02:42:52.363884 batchfetch-1.0.7/batchfetch/
--rw-r--r--   0 dev        (455) work      (1000)      774 2024-05-06 02:42:44.000000 batchfetch-1.0.7/batchfetch/__init__.py
--rw-r--r--   0 dev        (455) work      (1000)     5437 2024-05-06 02:42:44.000000 batchfetch-1.0.7/batchfetch/batchfetch_base.py
--rw-r--r--   0 dev        (455) work      (1000)     9639 2024-05-06 02:42:44.000000 batchfetch-1.0.7/batchfetch/batchfetch_cli.py
--rw-r--r--   0 dev        (455) work      (1000)    13084 2024-05-06 02:42:44.000000 batchfetch-1.0.7/batchfetch/batchfetch_git.py
--rw-r--r--   0 dev        (455) work      (1000)     4101 2024-05-06 02:42:44.000000 batchfetch-1.0.7/batchfetch/helpers.py
-drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-06 02:42:52.363884 batchfetch-1.0.7/batchfetch.egg-info/
--rw-r--r--   0 dev        (455) work      (1000)     4337 2024-05-06 02:42:52.000000 batchfetch-1.0.7/batchfetch.egg-info/PKG-INFO
--rw-r--r--   0 dev        (455) work      (1000)      365 2024-05-06 02:42:52.000000 batchfetch-1.0.7/batchfetch.egg-info/SOURCES.txt
--rw-r--r--   0 dev        (455) work      (1000)        1 2024-05-06 02:42:52.000000 batchfetch-1.0.7/batchfetch.egg-info/dependency_links.txt
--rw-r--r--   0 dev        (455) work      (1000)       80 2024-05-06 02:42:52.000000 batchfetch-1.0.7/batchfetch.egg-info/entry_points.txt
--rw-r--r--   0 dev        (455) work      (1000)       36 2024-05-06 02:42:52.000000 batchfetch-1.0.7/batchfetch.egg-info/requires.txt
--rw-r--r--   0 dev        (455) work      (1000)       11 2024-05-06 02:42:52.000000 batchfetch-1.0.7/batchfetch.egg-info/top_level.txt
--rw-r--r--   0 dev        (455) work      (1000)       38 2024-05-06 02:42:52.363884 batchfetch-1.0.7/setup.cfg
--rwxr-xr-x   0 dev        (455) work      (1000)     2029 2024-05-06 02:42:43.000000 batchfetch-1.0.7/setup.py
+drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-09 20:56:45.893095 batchfetch-1.0.8/
+-rw-r--r--   0 dev        (455) work      (1000)    35149 2024-05-09 20:56:41.000000 batchfetch-1.0.8/LICENSE
+-rw-r--r--   0 dev        (455) work      (1000)     4337 2024-05-09 20:56:45.893095 batchfetch-1.0.8/PKG-INFO
+-rw-r--r--   0 dev        (455) work      (1000)     3560 2024-05-09 20:56:41.000000 batchfetch-1.0.8/README.md
+drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-09 20:56:45.893095 batchfetch-1.0.8/batchfetch/
+-rw-r--r--   0 dev        (455) work      (1000)      774 2024-05-09 20:56:41.000000 batchfetch-1.0.8/batchfetch/__init__.py
+-rw-r--r--   0 dev        (455) work      (1000)     5437 2024-05-09 20:56:41.000000 batchfetch-1.0.8/batchfetch/batchfetch_base.py
+-rw-r--r--   0 dev        (455) work      (1000)     9749 2024-05-09 20:56:41.000000 batchfetch-1.0.8/batchfetch/batchfetch_cli.py
+-rw-r--r--   0 dev        (455) work      (1000)    13606 2024-05-09 20:56:41.000000 batchfetch-1.0.8/batchfetch/batchfetch_git.py
+-rw-r--r--   0 dev        (455) work      (1000)     4101 2024-05-09 20:56:41.000000 batchfetch-1.0.8/batchfetch/helpers.py
+drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-09 20:56:45.893095 batchfetch-1.0.8/batchfetch.egg-info/
+-rw-r--r--   0 dev        (455) work      (1000)     4337 2024-05-09 20:56:45.000000 batchfetch-1.0.8/batchfetch.egg-info/PKG-INFO
+-rw-r--r--   0 dev        (455) work      (1000)      365 2024-05-09 20:56:45.000000 batchfetch-1.0.8/batchfetch.egg-info/SOURCES.txt
+-rw-r--r--   0 dev        (455) work      (1000)        1 2024-05-09 20:56:45.000000 batchfetch-1.0.8/batchfetch.egg-info/dependency_links.txt
+-rw-r--r--   0 dev        (455) work      (1000)       80 2024-05-09 20:56:45.000000 batchfetch-1.0.8/batchfetch.egg-info/entry_points.txt
+-rw-r--r--   0 dev        (455) work      (1000)       36 2024-05-09 20:56:45.000000 batchfetch-1.0.8/batchfetch.egg-info/requires.txt
+-rw-r--r--   0 dev        (455) work      (1000)       11 2024-05-09 20:56:45.000000 batchfetch-1.0.8/batchfetch.egg-info/top_level.txt
+-rw-r--r--   0 dev        (455) work      (1000)       38 2024-05-09 20:56:45.897095 batchfetch-1.0.8/setup.cfg
+-rwxr-xr-x   0 dev        (455) work      (1000)     2029 2024-05-09 20:56:41.000000 batchfetch-1.0.8/setup.py
```

### Comparing `batchfetch-1.0.7/LICENSE` & `batchfetch-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `batchfetch-1.0.7/PKG-INFO` & `batchfetch-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batchfetch
-Version: 1.0.7
+Version: 1.0.8
 Summary: Efficiently clone and pull multiple Git repositories.
 Home-page: https://github.com/jamescherti/batchfetch
 Author: James Cherti
 License: GPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `batchfetch-1.0.7/README.md` & `batchfetch-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `batchfetch-1.0.7/batchfetch/__init__.py` & `batchfetch-1.0.8/batchfetch/__init__.py`

 * *Files identical despite different names*

### Comparing `batchfetch-1.0.7/batchfetch/batchfetch_base.py` & `batchfetch-1.0.8/batchfetch/batchfetch_base.py`

 * *Files identical despite different names*

### Comparing `batchfetch-1.0.7/batchfetch/batchfetch_cli.py` & `batchfetch-1.0.8/batchfetch/batchfetch_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 class BatchFetchCli:
     """Command-line-interface that downloads."""
 
     def __init__(self, max_workers: int, verbose: bool = False):
         self.cfg: dict = {}
         self.folder = Path(".")
-        self.managed_filenames: Set[str] = set()
+        self.managed_paths: Set[Path] = set()
         self.verbose = verbose
         self.max_workers = max_workers
         self._logger = logging.getLogger(self.__class__.__name__)
         self.dirs_relative_to_batchfetch: Set[str] = set()
 
         # Plugin
         self.batchfetch_schemas: Dict[Any, Any] = {}
@@ -145,45 +145,47 @@
             dict_local_dir[str(dest_path)] = batchfetch_instance[keyword]
 
     def run_tasks(self) -> bool:
         failed = []
         error = False
         threads = []
         num_success = 0
-        self.managed_filenames = set()
+        self.managed_paths = set()
 
         executor_update = ThreadPoolExecutor(max_workers=self.max_workers)
 
         try:
             self.dirs_relative_to_batchfetch = set()
 
             all_tasks = self.cfg["tasks"]
             for task in all_tasks:
                 self.dirs_relative_to_batchfetch.add(str(task["path"]))
                 if not task["delete"]:
-                    self.managed_filenames.add(task["path"])
+                    self.managed_paths.add(Path(task["path"]).absolute())
                 threads.append(executor_update.submit(task.update))
 
             for future in as_completed(threads):
                 data = future.result()
                 if data["result"]["error"]:
-                    print(Fore.RED, end="")
-                elif data["result"]["changed"]:
-                    print(Fore.YELLOW, end="")
+                    error = True
+                    failed.append(data)
                 else:
-                    if not self.verbose:
-                        continue
+                    num_success += 1
 
-                    print(Fore.GREEN, end="")
+                if (not self.verbose and
+                    not data["result"]["error"] and
+                        not data["result"]["changed"]):
+                    continue
 
                 if data["result"]["error"]:
-                    error = True
-                    failed.append(data)
+                    print(Fore.RED, end="")
+                elif data["result"]["changed"]:
+                    print(Fore.YELLOW, end="")
                 else:
-                    num_success += 1
+                    print(Fore.GREEN, end="")
 
                 if data["result"]["output"]:
                     print(data["result"]["output"].rstrip("\n"))
 
                 print(Fore.RESET, end="")
                 print()
         except KeyboardInterrupt:
```

### Comparing `batchfetch-1.0.7/batchfetch/batchfetch_git.py` & `batchfetch-1.0.8/batchfetch/batchfetch_git.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,15 @@
         elif is_clone:
             update_type = "CLONE"
         else:
             update_type = "UPDATE"
 
         self.add_output(
             f"[GIT {update_type}] {self[self.main_key]}" +
-            (f" (Reference: {self['reference']})"
+            (f" (Ref: {self['reference']})"
              if self["reference"] else "") + "\n"
         )
 
         try:
             # Delete
             if self["delete"]:
                 self._repo_delete()
@@ -214,35 +214,43 @@
 
         if self["reference"]:
             ignore_git_pull = False
             # Check if the new branch exists
             try:
                 self._git_tags(self["reference"])
             except GitReferenceDoesNotExist:
-                pass
+                # The reference does not exist. We should maybe git pull
+                # in case the reference is in a new commit.
+                ignore_git_pull = False
             else:
-                # The branch exists:
-                # 1. Ignore Git pull when the git reference is the same
-                # as the "branch:" key
-                try:
-                    commit_ref = self._git_ref(cwd=self.git_local_dir)
-                except subprocess.CalledProcessError:
-                    # Ignore git pull because the head is detached
-                    pass
+                if self.current_branch and \
+                        self.current_branch == self["reference"]:
+                    ignore_git_pull = False
                 else:
-                    if (self.current_branch and
-                        (commit_ref == self["reference"] or
-                         self.current_branch == self["reference"])):
+                    # The reference exists:
+                    # 1. Ignore Git pull when the git reference is the same
+                    # as the "branch:" key
+                    try:
+                        commit_ref = self._git_ref(cwd=self.git_local_dir)
+                    except subprocess.CalledProcessError:
+                        # Ignore git pull because the head is detached
+                        pass
+                    else:
+                        # The head is not detached
+                        # self.current_branch contains the current branch
+                        if (commit_ref == self["reference"] or
+                            (self.current_branch and
+                                self.current_branch == self["reference"])):
+                            ignore_git_pull = True
+
+                    # 2. Ignore Git pull if it is not a local branch
+                    if (not ignore_git_pull and
+                            not self._git_is_local_branch(self["reference"])):
                         ignore_git_pull = True
 
-                # 2. Ignore Git pull if it is not a local branch
-                if (not ignore_git_pull and
-                        not self._git_is_local_branch(self["reference"])):
-                    ignore_git_pull = True
-
         if ignore_git_pull:
             self.add_output(self.indent_spaces +
                             "[INFO] git pull ignored\n")
         else:
             cmd = ["git", "fetch", "origin"]
             self._run(cmd, cwd=str(self.git_local_dir), env=self.env)
```

### Comparing `batchfetch-1.0.7/batchfetch/helpers.py` & `batchfetch-1.0.8/batchfetch/helpers.py`

 * *Files identical despite different names*

### Comparing `batchfetch-1.0.7/batchfetch.egg-info/PKG-INFO` & `batchfetch-1.0.8/batchfetch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batchfetch
-Version: 1.0.7
+Version: 1.0.8
 Summary: Efficiently clone and pull multiple Git repositories.
 Home-page: https://github.com/jamescherti/batchfetch
 Author: James Cherti
 License: GPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `batchfetch-1.0.7/setup.py` & `batchfetch-1.0.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 setup(
     name="batchfetch",
-    version="1.0.7",
+    version="1.0.8",
     packages=find_packages(),
     description="Efficiently clone and pull multiple Git repositories.",
     license="GPLv3",
     long_description=((Path(__file__).parent.resolve().joinpath("README.md"))
                       .read_text(encoding="utf-8")),
     long_description_content_type="text/markdown",
     url="https://github.com/jamescherti/batchfetch",
```

