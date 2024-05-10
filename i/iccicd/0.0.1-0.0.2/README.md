# Comparing `tmp/iccicd-0.0.1.tar.gz` & `tmp/iccicd-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iccicd-0.0.1.tar", last modified: Fri May  3 11:04:30 2024, max compression
+gzip compressed data, was "iccicd-0.0.2.tar", last modified: Fri May 10 11:24:41 2024, max compression
```

## Comparing `iccicd-0.0.1.tar` & `iccicd-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,36 @@
-drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-03 11:04:30.055978 iccicd-0.0.1/
--rw-r--r--   0 jgrogan    (503) staff       (20)    34621 2024-05-03 09:22:07.000000 iccicd-0.0.1/LICENSE.txt
--rw-r--r--   0 jgrogan    (503) staff       (20)     1135 2024-05-03 11:04:30.055852 iccicd-0.0.1/PKG-INFO
--rw-r--r--   0 jgrogan    (503) staff       (20)      102 2024-05-03 09:22:07.000000 iccicd-0.0.1/README.md
--rw-r--r--   0 jgrogan    (503) staff       (20)     1836 2024-05-03 10:16:29.000000 iccicd-0.0.1/pyproject.toml
--rw-r--r--   0 jgrogan    (503) staff       (20)       93 2024-05-03 11:04:30.067754 iccicd-0.0.1/setup.cfg
-drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-03 11:04:30.031062 iccicd-0.0.1/src/
-drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-03 11:04:30.031649 iccicd-0.0.1/src/iccicd/
--rw-r--r--   0 jgrogan    (503) staff       (20)        0 2024-05-03 09:22:07.000000 iccicd-0.0.1/src/iccicd/__init__.py
--rw-r--r--   0 jgrogan    (503) staff       (20)     1189 2024-05-03 11:03:13.000000 iccicd-0.0.1/src/iccicd/deploy.py
-drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-03 11:04:30.055029 iccicd-0.0.1/src/iccicd.egg-info/
--rw-r--r--   0 jgrogan    (503) staff       (20)     1135 2024-05-03 11:04:30.000000 iccicd-0.0.1/src/iccicd.egg-info/PKG-INFO
--rw-r--r--   0 jgrogan    (503) staff       (20)      296 2024-05-03 11:04:30.000000 iccicd-0.0.1/src/iccicd.egg-info/SOURCES.txt
--rw-r--r--   0 jgrogan    (503) staff       (20)        1 2024-05-03 11:04:30.000000 iccicd-0.0.1/src/iccicd.egg-info/dependency_links.txt
--rw-r--r--   0 jgrogan    (503) staff       (20)       69 2024-05-03 11:04:30.000000 iccicd-0.0.1/src/iccicd.egg-info/requires.txt
--rw-r--r--   0 jgrogan    (503) staff       (20)       18 2024-05-03 11:04:30.000000 iccicd-0.0.1/src/iccicd.egg-info/top_level.txt
--rw-r--r--   0 jgrogan    (503) staff       (20)     1618 2024-05-03 10:59:46.000000 iccicd-0.0.1/src/iccicd_cli.py
-drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-03 11:04:30.054419 iccicd-0.0.1/test/
--rw-r--r--   0 jgrogan    (503) staff       (20)       43 2024-05-03 09:22:07.000000 iccicd-0.0.1/test/test_iccid.py
+drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-10 11:24:41.331371 iccicd-0.0.2/
+-rw-r--r--   0 jgrogan    (503) staff       (20)    34621 2024-05-03 09:22:07.000000 iccicd-0.0.2/LICENSE.txt
+-rw-r--r--   0 jgrogan    (503) staff       (20)     1622 2024-05-10 11:24:41.331234 iccicd-0.0.2/PKG-INFO
+-rw-r--r--   0 jgrogan    (503) staff       (20)      548 2024-05-03 13:22:03.000000 iccicd-0.0.2/README.md
+-rw-r--r--   0 jgrogan    (503) staff       (20)     1968 2024-05-10 11:23:29.000000 iccicd-0.0.2/pyproject.toml
+-rw-r--r--   0 jgrogan    (503) staff       (20)       93 2024-05-10 11:24:41.353712 iccicd-0.0.2/setup.cfg
+drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-10 11:24:41.277130 iccicd-0.0.2/src/
+drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-10 11:24:41.278524 iccicd-0.0.2/src/iccicd/
+-rw-r--r--   0 jgrogan    (503) staff       (20)        0 2024-05-03 09:22:07.000000 iccicd-0.0.2/src/iccicd/__init__.py
+drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-10 11:24:41.308841 iccicd-0.0.2/src/iccicd/packaging/
+-rw-r--r--   0 jgrogan    (503) staff       (20)       38 2024-05-10 11:23:29.000000 iccicd-0.0.2/src/iccicd/packaging/__init__.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)     1185 2024-05-10 11:23:29.000000 iccicd-0.0.2/src/iccicd/packaging/python_package.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)        0 2024-05-10 11:23:29.000000 iccicd-0.0.2/src/iccicd/py.typed
+drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-10 11:24:41.325890 iccicd-0.0.2/src/iccicd/repo/
+-rw-r--r--   0 jgrogan    (503) staff       (20)       63 2024-05-10 11:23:29.000000 iccicd-0.0.2/src/iccicd/repo/__init__.py
+drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-10 11:24:41.327577 iccicd-0.0.2/src/iccicd/repo/python_repo/
+-rw-r--r--   0 jgrogan    (503) staff       (20)      118 2024-05-10 11:23:29.000000 iccicd-0.0.2/src/iccicd/repo/python_repo/__init__.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)     1564 2024-05-10 11:23:29.000000 iccicd-0.0.2/src/iccicd/repo/python_repo/pyproject_interface.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)      633 2024-05-10 11:23:29.000000 iccicd-0.0.2/src/iccicd/repo/python_repo/python_repo.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)      928 2024-05-10 11:23:29.000000 iccicd-0.0.2/src/iccicd/repo/python_repo/sphinx_interface.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)      266 2024-05-10 11:23:29.000000 iccicd-0.0.2/src/iccicd/repo/repo.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)      454 2024-05-10 11:23:29.000000 iccicd-0.0.2/src/iccicd/version.py
+drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-10 11:24:41.329401 iccicd-0.0.2/src/iccicd/version_control/
+-rw-r--r--   0 jgrogan    (503) staff       (20)        0 2024-05-10 11:23:29.000000 iccicd-0.0.2/src/iccicd/version_control/__init__.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)     1054 2024-05-10 11:23:29.000000 iccicd-0.0.2/src/iccicd/version_control/git_interface.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)     1382 2024-05-10 11:23:29.000000 iccicd-0.0.2/src/iccicd/version_control/gitlab.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)      249 2024-05-10 11:23:29.000000 iccicd-0.0.2/src/iccicd/version_control/merge_request.py
+drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-10 11:24:41.330314 iccicd-0.0.2/src/iccicd.egg-info/
+-rw-r--r--   0 jgrogan    (503) staff       (20)     1622 2024-05-10 11:24:41.000000 iccicd-0.0.2/src/iccicd.egg-info/PKG-INFO
+-rw-r--r--   0 jgrogan    (503) staff       (20)      794 2024-05-10 11:24:41.000000 iccicd-0.0.2/src/iccicd.egg-info/SOURCES.txt
+-rw-r--r--   0 jgrogan    (503) staff       (20)        1 2024-05-10 11:24:41.000000 iccicd-0.0.2/src/iccicd.egg-info/dependency_links.txt
+-rw-r--r--   0 jgrogan    (503) staff       (20)       84 2024-05-10 11:24:41.000000 iccicd-0.0.2/src/iccicd.egg-info/requires.txt
+-rw-r--r--   0 jgrogan    (503) staff       (20)        7 2024-05-10 11:24:41.000000 iccicd-0.0.2/src/iccicd.egg-info/top_level.txt
+-rw-r--r--   0 jgrogan    (503) staff       (20)     3262 2024-05-10 11:23:29.000000 iccicd-0.0.2/src/iccicd_cli.py
+drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-10 11:24:41.329829 iccicd-0.0.2/test/
+-rw-r--r--   0 jgrogan    (503) staff       (20)     1057 2024-05-10 11:23:29.000000 iccicd-0.0.2/test/test_bump_version.py
```

### Comparing `iccicd-0.0.1/LICENSE.txt` & `iccicd-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iccicd-0.0.1/pyproject.toml` & `iccicd-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [project]
 name = "iccicd"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="James Grogan, Irish Centre for High End Computing", email="james.grogan@ichec.ie" },
 ]
 description = "A collection of utilities to manage ICHEC project CI/CD pipelines."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: GNU Affero General Public License v3",
+    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: OS Independent",
     "Topic :: System :: Distributed Computing"
 ]
 keywords = ["CICD", "HPC", "Gitlab"]
 
-dependencies = ["build", "twine", "iccore"]
+dependencies = ["build", "twine", "iccore>=0.0.2", "tomlkit"]
 
 [project.urls]
 Repository = "https://git.ichec.ie/performance/toolshed/iccicd"
 Homepage = "https://git.ichec.ie/performance/toolshed/iccicd"
 
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
@@ -31,14 +31,20 @@
     "pytest",
     "pytest-cov",
     "pytest-sugar",
     "black",
     "mypy"
 ]
 
+[tool.setuptools.package-data]
+"iccicd" = ["py.typed"]
+
+[tool.setuptools.packages.find]
+where = ["src"]
+
 [tool.mypy]
 ignore_missing_imports = true
 
 [tool.pytest.ini_options]
 testpaths = ["test",]
 log_cli = 1
 log_cli_level = "debug"
@@ -59,16 +65,16 @@
 commands =
     pytest {posargs:test}
 
 [testenv:lint]
 description = run linters
 skip_install = true
 deps =
-    black==22.12
-commands = black {posargs:src}
+    black
+commands = black {posargs:src test}
 
 [testenv:style]
 description = run style check
 skip_install = true
 deps =
     flake8
 commands = flake8 {posargs:src}
```

### Comparing `iccicd-0.0.1/src/iccicd/deploy.py` & `iccicd-0.0.2/src/iccicd/packaging/python_package.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from pathlib import Path
 import logging
 
 from iccore import process
 
-logger = logging.getLogger(__name__)
 
+logger = logging.getLogger(__name__)
 
-class PyPiContext():
 
+class PyPiContext:
     def __init__(self, token: str, use_test_repo: bool) -> None:
         self.token = token
         self.use_test_repo = use_test_repo
 
 
-class PythonPackage():
-
+class PythonPackage:
     def __init__(self, repo_path: Path) -> None:
         self.repo_path = repo_path
 
     def build(self):
         logger.info("Building Python package")
         output_dir = self.repo_path / "dist"
         cmd = f"python3 -m build --outdir {output_dir} {self.repo_path}"
@@ -35,8 +34,8 @@
         if pypi_context.use_test_repo:
             repo = " -r testpypi "
 
         token = f"-p {pypi_context.token}"
         upload_dir = self.repo_path / "dist"
         cmd = f"twine upload {upload_dir}/*  --non-interactive {token} {repo}"
         process.run(cmd)
-        logger.info("Finished uploading Python package")
+        logger.info("Finished uploading Python package")
```

