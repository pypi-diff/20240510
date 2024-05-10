# Comparing `tmp/batchfetch-1.0.8.tar.gz` & `tmp/batchfetch-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batchfetch-1.0.8.tar", last modified: Thu May  9 20:56:45 2024, max compression
+gzip compressed data, was "batchfetch-1.0.9.tar", last modified: Fri May 10 17:26:18 2024, max compression
```

## Comparing `batchfetch-1.0.8.tar` & `batchfetch-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,26 @@
-drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-09 20:56:45.893095 batchfetch-1.0.8/
--rw-r--r--   0 dev        (455) work      (1000)    35149 2024-05-09 20:56:41.000000 batchfetch-1.0.8/LICENSE
--rw-r--r--   0 dev        (455) work      (1000)     4337 2024-05-09 20:56:45.893095 batchfetch-1.0.8/PKG-INFO
--rw-r--r--   0 dev        (455) work      (1000)     3560 2024-05-09 20:56:41.000000 batchfetch-1.0.8/README.md
-drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-09 20:56:45.893095 batchfetch-1.0.8/batchfetch/
--rw-r--r--   0 dev        (455) work      (1000)      774 2024-05-09 20:56:41.000000 batchfetch-1.0.8/batchfetch/__init__.py
--rw-r--r--   0 dev        (455) work      (1000)     5437 2024-05-09 20:56:41.000000 batchfetch-1.0.8/batchfetch/batchfetch_base.py
--rw-r--r--   0 dev        (455) work      (1000)     9749 2024-05-09 20:56:41.000000 batchfetch-1.0.8/batchfetch/batchfetch_cli.py
--rw-r--r--   0 dev        (455) work      (1000)    13606 2024-05-09 20:56:41.000000 batchfetch-1.0.8/batchfetch/batchfetch_git.py
--rw-r--r--   0 dev        (455) work      (1000)     4101 2024-05-09 20:56:41.000000 batchfetch-1.0.8/batchfetch/helpers.py
-drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-09 20:56:45.893095 batchfetch-1.0.8/batchfetch.egg-info/
--rw-r--r--   0 dev        (455) work      (1000)     4337 2024-05-09 20:56:45.000000 batchfetch-1.0.8/batchfetch.egg-info/PKG-INFO
--rw-r--r--   0 dev        (455) work      (1000)      365 2024-05-09 20:56:45.000000 batchfetch-1.0.8/batchfetch.egg-info/SOURCES.txt
--rw-r--r--   0 dev        (455) work      (1000)        1 2024-05-09 20:56:45.000000 batchfetch-1.0.8/batchfetch.egg-info/dependency_links.txt
--rw-r--r--   0 dev        (455) work      (1000)       80 2024-05-09 20:56:45.000000 batchfetch-1.0.8/batchfetch.egg-info/entry_points.txt
--rw-r--r--   0 dev        (455) work      (1000)       36 2024-05-09 20:56:45.000000 batchfetch-1.0.8/batchfetch.egg-info/requires.txt
--rw-r--r--   0 dev        (455) work      (1000)       11 2024-05-09 20:56:45.000000 batchfetch-1.0.8/batchfetch.egg-info/top_level.txt
--rw-r--r--   0 dev        (455) work      (1000)       38 2024-05-09 20:56:45.897095 batchfetch-1.0.8/setup.cfg
--rwxr-xr-x   0 dev        (455) work      (1000)     2029 2024-05-09 20:56:41.000000 batchfetch-1.0.8/setup.py
+drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-10 17:26:18.106605 batchfetch-1.0.9/
+-rw-r--r--   0 dev        (455) work      (1000)     2034 2024-05-10 17:26:12.000000 batchfetch-1.0.9/.gitignore
+-rw-r--r--   0 dev        (455) work      (1000)    35149 2024-05-10 17:26:12.000000 batchfetch-1.0.9/LICENSE
+-rw-r--r--   0 dev        (455) work      (1000)     4433 2024-05-10 17:26:18.106605 batchfetch-1.0.9/PKG-INFO
+-rw-r--r--   0 dev        (455) work      (1000)     3560 2024-05-10 17:26:12.000000 batchfetch-1.0.9/README.md
+drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-10 17:26:18.106605 batchfetch-1.0.9/batchfetch/
+-rw-r--r--   0 dev        (455) work      (1000)      774 2024-05-10 17:26:12.000000 batchfetch-1.0.9/batchfetch/__init__.py
+-rw-r--r--   0 dev        (455) work      (1000)     5437 2024-05-10 17:26:12.000000 batchfetch-1.0.9/batchfetch/batchfetch_base.py
+-rw-r--r--   0 dev        (455) work      (1000)     9749 2024-05-10 17:26:12.000000 batchfetch-1.0.9/batchfetch/batchfetch_cli.py
+-rw-r--r--   0 dev        (455) work      (1000)    13257 2024-05-10 17:26:12.000000 batchfetch-1.0.9/batchfetch/batchfetch_git.py
+-rw-r--r--   0 dev        (455) work      (1000)     4101 2024-05-10 17:26:12.000000 batchfetch-1.0.9/batchfetch/helpers.py
+drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-10 17:26:18.106605 batchfetch-1.0.9/batchfetch.egg-info/
+-rw-r--r--   0 dev        (455) work      (1000)     4433 2024-05-10 17:26:17.000000 batchfetch-1.0.9/batchfetch.egg-info/PKG-INFO
+-rw-r--r--   0 dev        (455) work      (1000)      468 2024-05-10 17:26:18.000000 batchfetch-1.0.9/batchfetch.egg-info/SOURCES.txt
+-rw-r--r--   0 dev        (455) work      (1000)        1 2024-05-10 17:26:17.000000 batchfetch-1.0.9/batchfetch.egg-info/dependency_links.txt
+-rw-r--r--   0 dev        (455) work      (1000)       80 2024-05-10 17:26:17.000000 batchfetch-1.0.9/batchfetch.egg-info/entry_points.txt
+-rw-r--r--   0 dev        (455) work      (1000)       36 2024-05-10 17:26:17.000000 batchfetch-1.0.9/batchfetch.egg-info/requires.txt
+-rw-r--r--   0 dev        (455) work      (1000)       11 2024-05-10 17:26:17.000000 batchfetch-1.0.9/batchfetch.egg-info/top_level.txt
+-rwxr-xr-x   0 dev        (455) work      (1000)      916 2024-05-10 17:26:12.000000 batchfetch-1.0.9/run_tests.sh
+-rw-r--r--   0 dev        (455) work      (1000)       38 2024-05-10 17:26:18.106605 batchfetch-1.0.9/setup.cfg
+-rwxr-xr-x   0 dev        (455) work      (1000)     2029 2024-05-10 17:26:12.000000 batchfetch-1.0.9/setup.py
+drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-10 17:26:18.106605 batchfetch-1.0.9/tests/
+drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-10 17:26:18.106605 batchfetch-1.0.9/tests/data/
+-rw-r--r--   0 dev        (455) work      (1000)       24 2024-05-10 17:26:12.000000 batchfetch-1.0.9/tests/data/test-md5sum.txt
+-rwxr-xr-x   0 dev        (455) work      (1000)      117 2024-05-10 17:26:12.000000 batchfetch-1.0.9/tests/data/test-run_simple.sh
+-rw-r--r--   0 dev        (455) work      (1000)     1870 2024-05-10 17:26:12.000000 batchfetch-1.0.9/tests/test_helpers.py
```

### Comparing `batchfetch-1.0.8/LICENSE` & `batchfetch-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `batchfetch-1.0.8/PKG-INFO` & `batchfetch-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batchfetch
-Version: 1.0.8
+Version: 1.0.9
 Summary: Efficiently clone and pull multiple Git repositories.
 Home-page: https://github.com/jamescherti/batchfetch
 Author: James Cherti
 License: GPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -13,14 +13,18 @@
 Classifier: Operating System :: POSIX :: Other
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Version Control :: Git
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: colorama
+Requires-Dist: schema
+Requires-Dist: setproctitle
+Requires-Dist: PyYAML
 
 # Batchfetch - Efficiently clone or pull multiple Git repositories in parallel
 
 ## Introduction
 
 Batchfetch is a command-line tool designed to clone, fetch, and merge multiple Git repositories simultaneously.
```

### Comparing `batchfetch-1.0.8/README.md` & `batchfetch-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `batchfetch-1.0.8/batchfetch/__init__.py` & `batchfetch-1.0.9/batchfetch/__init__.py`

 * *Files identical despite different names*

### Comparing `batchfetch-1.0.8/batchfetch/batchfetch_base.py` & `batchfetch-1.0.9/batchfetch/batchfetch_base.py`

 * *Files identical despite different names*

### Comparing `batchfetch-1.0.8/batchfetch/batchfetch_cli.py` & `batchfetch-1.0.9/batchfetch/batchfetch_cli.py`

 * *Files identical despite different names*

### Comparing `batchfetch-1.0.8/batchfetch/batchfetch_git.py` & `batchfetch-1.0.9/batchfetch/batchfetch_git.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,15 +88,15 @@
                     self.values[self.main_key])  # type: ignore
 
     def _git_ref(self, cwd: Union[None, Path] = None) -> str:
         """Get the commit reference of HEAD.
 
         The command will fail if the branch is detached.
         """
-        cmd = "git show-ref --head --verify HEAD"
+        cmd = ["git", "show-ref", "--head", "--verify", "HEAD"]
         try:
             stdout, _ = run_simple(cmd, cwd=cwd, env=self.env)
             output = stdout[0].split(" ")[0]
         except IndexError:
             return ""
         return output
 
@@ -204,74 +204,66 @@
         cmd = ["git", "reset", "--hard", "HEAD"]
         self._run(cmd, cwd=str(self.git_local_dir), env=self.env)
 
     def _repo_pull(self):
         git_merge = False
 
         # Merge
-        ignore_git_pull = False
-        if not self["git_pull"]:
-            ignore_git_pull = True
-
+        do_git_pull = self["git_pull"]
+        disable_merge = False
         if self["reference"]:
-            ignore_git_pull = False
-            # Check if the new branch exists
+            commit_ref = None
             try:
-                self._git_tags(self["reference"])
+                # Returns the commit ref of the branch or commit
+                commit_ref = self._git_tags(self["reference"])[0]
             except GitReferenceDoesNotExist:
-                # The reference does not exist. We should maybe git pull
-                # in case the reference is in a new commit.
-                ignore_git_pull = False
-            else:
-                if self.current_branch and \
-                        self.current_branch == self["reference"]:
-                    ignore_git_pull = False
+                # The reference does not exist. We should git pull
+                # in case we can get the reference
+                do_git_pull = True
+            else:  # The reference exists
+                if not self._git_is_local_branch(self["reference"]):
+                    # This is not a real branch where we can merge
+                    disable_merge = True
+
+                try:
+                    # Returns the commit ref of the branch or commit
+                    commit_ref_head = self._git_tags("HEAD")[0]
+                except GitReferenceDoesNotExist:
+                    # HEAD is detached
+                    commit_ref_head = None
+
+                # The wanted commit reference does not exist
+                # Or the commit ref of HEAD hasn't changed
+                if not commit_ref or commit_ref_head != commit_ref:
+                    do_git_pull = True
                 else:
-                    # The reference exists:
-                    # 1. Ignore Git pull when the git reference is the same
-                    # as the "branch:" key
-                    try:
-                        commit_ref = self._git_ref(cwd=self.git_local_dir)
-                    except subprocess.CalledProcessError:
-                        # Ignore git pull because the head is detached
-                        pass
-                    else:
-                        # The head is not detached
-                        # self.current_branch contains the current branch
-                        if (commit_ref == self["reference"] or
-                            (self.current_branch and
-                                self.current_branch == self["reference"])):
-                            ignore_git_pull = True
-
-                    # 2. Ignore Git pull if it is not a local branch
-                    if (not ignore_git_pull and
-                            not self._git_is_local_branch(self["reference"])):
-                        ignore_git_pull = True
+                    do_git_pull = False
 
-        if ignore_git_pull:
+        if not do_git_pull:
             self.add_output(self.indent_spaces +
                             "[INFO] git pull ignored\n")
         else:
             cmd = ["git", "fetch", "origin"]
             self._run(cmd, cwd=str(self.git_local_dir), env=self.env)
 
             # TODO: only merge when difference from upstream
-            commit_ref = self._git_ref(cwd=self.git_local_dir)
-            self._run(["git", "merge", "--ff-only"],
-                      cwd=str(self.git_local_dir), env=self.env)
-            git_ref_after_merge = self._git_ref(cwd=self.git_local_dir)
-            if commit_ref != git_ref_after_merge:
-                git_merge = True
-                self.set_changed(True)
-                self._run(["git", "log",
-                           '--pretty=format:"%h %ad %s [%cn]"',
-                           "--decorate", "--date=short",
-                           f"{commit_ref}..{git_ref_after_merge}"],
-                          cwd=str(self.git_local_dir),
-                          env=self.env)
+            commit_ref_head = self._git_ref(cwd=self.git_local_dir)
+            if not disable_merge:
+                self._run(["git", "merge", "--ff-only"],
+                          cwd=str(self.git_local_dir), env=self.env)
+                git_ref_after_merge = self._git_ref(cwd=self.git_local_dir)
+                if commit_ref_head != git_ref_after_merge:
+                    git_merge = True
+                    self.set_changed(True)
+                    self._run(["git", "log",
+                               '--pretty=format:"%h %ad %s [%cn]"',
+                               "--decorate", "--date=short",
+                               f"{commit_ref_head}..{git_ref_after_merge}"],
+                              cwd=str(self.git_local_dir),
+                              env=self.env)
 
         return git_merge
 
     def _git_is_local_branch(self, branch: str) -> bool:
         try:
             stdout, _ = run_simple(["git", "rev-parse", "--symbolic-full-name",
                                     branch], env=self.env,
@@ -287,18 +279,17 @@
             pass
 
         return False
 
     def _git_tags(self, branch: str) -> List[str]:
         stdout: List[str] = []
         try:
-            stdout, _ = run_simple(
-                ["git", "rev-parse", "--verify", branch],
-                env=self.env,
-                cwd=self.git_local_dir)
+            stdout, _ = run_simple(["git", "rev-parse", "--verify", branch],
+                                   env=self.env,
+                                   cwd=self.git_local_dir)
         except subprocess.CalledProcessError as err:
             raise GitReferenceDoesNotExist(
                 f"The reference '{branch}' does not exist.") from err
 
         return stdout
 
     def _repo_fix_branch(self) -> bool:
```

### Comparing `batchfetch-1.0.8/batchfetch/helpers.py` & `batchfetch-1.0.9/batchfetch/helpers.py`

 * *Files identical despite different names*

### Comparing `batchfetch-1.0.8/batchfetch.egg-info/PKG-INFO` & `batchfetch-1.0.9/batchfetch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batchfetch
-Version: 1.0.8
+Version: 1.0.9
 Summary: Efficiently clone and pull multiple Git repositories.
 Home-page: https://github.com/jamescherti/batchfetch
 Author: James Cherti
 License: GPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -13,14 +13,18 @@
 Classifier: Operating System :: POSIX :: Other
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Version Control :: Git
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: colorama
+Requires-Dist: schema
+Requires-Dist: setproctitle
+Requires-Dist: PyYAML
 
 # Batchfetch - Efficiently clone or pull multiple Git repositories in parallel
 
 ## Introduction
 
 Batchfetch is a command-line tool designed to clone, fetch, and merge multiple Git repositories simultaneously.
```

### Comparing `batchfetch-1.0.8/setup.py` & `batchfetch-1.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 setup(
     name="batchfetch",
-    version="1.0.8",
+    version="1.0.9",
     packages=find_packages(),
     description="Efficiently clone and pull multiple Git repositories.",
     license="GPLv3",
     long_description=((Path(__file__).parent.resolve().joinpath("README.md"))
                       .read_text(encoding="utf-8")),
     long_description_content_type="text/markdown",
     url="https://github.com/jamescherti/batchfetch",
```

