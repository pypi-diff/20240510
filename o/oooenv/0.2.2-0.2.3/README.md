# Comparing `tmp/oooenv-0.2.2.tar.gz` & `tmp/oooenv-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oooenv-0.2.2.tar", max compression
+gzip compressed data, was "oooenv-0.2.3.tar", max compression
```

## Comparing `oooenv-0.2.2.tar` & `oooenv-0.2.3.tar`

### file list

```diff
@@ -1,24 +1,16 @@
--rwxr-xr-x   0        0        0     1073 2023-03-29 17:32:33.108507 oooenv-0.2.2/LICENSE
--rwxr-xr-x   0        0        0     2681 2023-06-17 19:01:17.362300 oooenv-0.2.2/README.md
--rwxr-xr-x   0        0        0        0 2023-03-29 14:28:44.487665 oooenv-0.2.2/oooenv/__init__.py
--rwxr-xr-x   0        0        0        0 2023-03-29 17:14:51.509563 oooenv-0.2.2/oooenv/cli/__init__.py
--rwxr-xr-x   0        0        0     8066 2023-06-17 17:49:31.367107 oooenv-0.2.2/oooenv/cli/main.py
--rwxr-xr-x   0        0        0        0 2023-03-29 14:36:41.949832 oooenv-0.2.2/oooenv/cmds/__init__.py
--rwxr-xr-x   0        0        0      174 2023-03-29 15:00:18.797439 oooenv-0.2.2/oooenv/cmds/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     5103 2023-03-29 17:06:15.560117 oooenv-0.2.2/oooenv/cmds/__pycache__/manage_env_cfg.cpython-310.pyc
--rwxr-xr-x   0        0        0     2841 2023-03-29 15:00:18.802246 oooenv-0.2.2/oooenv/cmds/__pycache__/uno_lnk.cpython-310.pyc
--rwxr-xr-x   0        0        0      883 2023-06-17 17:49:31.368191 oooenv-0.2.2/oooenv/cmds/install.py
--rwxr-xr-x   0        0        0     5767 2023-06-17 17:49:31.369339 oooenv-0.2.2/oooenv/cmds/manage_env_cfg.py
--rwxr-xr-x   0        0        0     4627 2023-06-17 17:49:31.370392 oooenv-0.2.2/oooenv/cmds/uno_lnk.py
--rwxr-xr-x   0        0        0     1216 2023-06-17 17:49:31.371160 oooenv-0.2.2/oooenv/cmds/updater.py
--rwxr-xr-x   0        0        0        0 2023-03-29 14:34:49.616759 oooenv-0.2.2/oooenv/utils/__init__.py
--rwxr-xr-x   0        0        0      175 2023-03-29 15:00:18.812804 oooenv-0.2.2/oooenv/utils/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     3710 2023-03-29 15:00:18.815799 oooenv-0.2.2/oooenv/utils/__pycache__/local_paths.cpython-310.pyc
--rwxr-xr-x   0        0        0     1146 2023-03-29 15:00:18.820968 oooenv-0.2.2/oooenv/utils/__pycache__/sys_info.cpython-310.pyc
--rwxr-xr-x   0        0        0     5887 2023-03-29 15:00:18.819281 oooenv-0.2.2/oooenv/utils/__pycache__/uno_paths.cpython-310.pyc
--rwxr-xr-x   0        0        0     3708 2023-03-29 14:34:49.621334 oooenv-0.2.2/oooenv/utils/__pycache__/util.cpython-310.pyc
--rwxr-xr-x   0        0        0     3573 2023-06-17 19:02:46.802447 oooenv-0.2.2/oooenv/utils/local_paths.py
--rwxr-xr-x   0        0        0      773 2023-06-17 17:49:31.374581 oooenv-0.2.2/oooenv/utils/sys_info.py
--rwxr-xr-x   0        0        0    10430 2023-06-17 19:02:37.679772 oooenv-0.2.2/oooenv/utils/uno_paths.py
--rwxr-xr-x   0        0        0     1419 2023-06-17 17:50:51.464403 oooenv-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3740 1970-01-01 00:00:00.000000 oooenv-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-10 19:38:38.177533 oooenv-0.2.3/LICENSE
+-rw-r--r--   0        0        0     2681 2024-05-10 19:38:38.177533 oooenv-0.2.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-10 19:38:38.177533 oooenv-0.2.3/oooenv/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 19:38:38.181533 oooenv-0.2.3/oooenv/cli/__init__.py
+-rw-r--r--   0        0        0     8225 2024-05-10 19:46:21.704519 oooenv-0.2.3/oooenv/cli/main.py
+-rw-r--r--   0        0        0        0 2024-05-10 19:38:38.181533 oooenv-0.2.3/oooenv/cmds/__init__.py
+-rw-r--r--   0        0        0     1181 2024-05-10 20:04:23.963339 oooenv-0.2.3/oooenv/cmds/install.py
+-rw-r--r--   0        0        0     5767 2024-05-10 19:38:38.181533 oooenv-0.2.3/oooenv/cmds/manage_env_cfg.py
+-rw-r--r--   0        0        0     4627 2024-05-10 19:38:38.181533 oooenv-0.2.3/oooenv/cmds/uno_lnk.py
+-rw-r--r--   0        0        0     1216 2024-05-10 19:38:38.181533 oooenv-0.2.3/oooenv/cmds/updater.py
+-rw-r--r--   0        0        0        0 2024-05-10 19:38:38.181533 oooenv-0.2.3/oooenv/utils/__init__.py
+-rw-r--r--   0        0        0     3573 2024-05-10 19:38:38.181533 oooenv-0.2.3/oooenv/utils/local_paths.py
+-rw-r--r--   0        0        0      773 2024-05-10 19:38:38.181533 oooenv-0.2.3/oooenv/utils/sys_info.py
+-rw-r--r--   0        0        0    10430 2024-05-10 19:38:38.181533 oooenv-0.2.3/oooenv/utils/uno_paths.py
+-rw-r--r--   0        0        0     1419 2024-05-10 20:04:34.035423 oooenv-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3791 1970-01-01 00:00:00.000000 oooenv-0.2.3/PKG-INFO
```

### Comparing `oooenv-0.2.2/LICENSE` & `oooenv-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `oooenv-0.2.2/README.md` & `oooenv-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `oooenv-0.2.2/oooenv/cli/main.py` & `oooenv-0.2.3/oooenv/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,31 +206,30 @@
         action="store_true",
         dest="show_version",
         default=False,
     )
     parser.add_argument(
         "-e",
         "--editable",
-        help="Install a project in editable mode from the local project path. Similar to pip install -e .",
-        action="store_true",
-        dest="editable",
-        default=False,
+        help="Install a project in editable mode from the local project path. Similar to pip install -e <package>. Defaults to . (the current package itself), but the root folder of any package source can be given (relative or absolute).",
+        action="store",
+        dest="editable_package_path",
+        default=".",
     )
 
 
 def _args_action_global(a_parser: argparse.ArgumentParser, args: argparse.Namespace) -> str | None:
     # sourcery skip: assign-if-exp, reintroduce-else
     if args.show_version:
         # return importlib.metadata.version(__package__ or __name__)
         return importlib.metadata.version("oooenv")
-    if args.editable:
-        if result := install.pip_e():
+    if args.editable_package_path:
+        if result := install.pip_e(args.editable_package_path):
             return result
-        else:
-            return "Install Failed for unknown reason."
+        return "Install Failed for unknown reason."
     return None
 
 
 # endregion process arg command for global
 
 # endregion parser
```

### Comparing `oooenv-0.2.2/oooenv/cmds/install.py` & `oooenv-0.2.3/oooenv/cmds/install.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 from __future__ import annotations
 from pathlib import Path
-import os
 from ..utils import local_paths
 
 
-def pip_e() -> str:
+def pip_e(package_path: str = ".") -> str:
     """
     Install root path in virtual environment site-packages directory.
 
     Basically the same thing as ``pip -e .`` but without the need for pip.
 
+    Args:
+        package_path (str, optional): Path to package. Defaults to ``"."``.
+
     Returns:
         str: Message indicating success or failure. Empty string on failure.
     """
     try:
         root_path = Path(local_paths.get_virtual_env_path()).parent
+        if package_path and package_path != ".":
+            root_path = root_path / package_path
+
+        if not root_path.exists():
+            return f"No such package path as: {str(root_path)}"
         site_packages_dir = local_paths.get_site_packages_dir()
         if site_packages_dir is None:
             return ""
         file_name = site_packages_dir / f"{root_path.name.replace('.', '_').replace(' ', '_')}.pth"
         with open(file_name, "w") as f:
             f.write(str(root_path))
         return f"Created file: {file_name}"
```

### Comparing `oooenv-0.2.2/oooenv/cmds/manage_env_cfg.py` & `oooenv-0.2.3/oooenv/cmds/manage_env_cfg.py`

 * *Files identical despite different names*

### Comparing `oooenv-0.2.2/oooenv/cmds/uno_lnk.py` & `oooenv-0.2.3/oooenv/cmds/uno_lnk.py`

 * *Files identical despite different names*

### Comparing `oooenv-0.2.2/oooenv/cmds/updater.py` & `oooenv-0.2.3/oooenv/cmds/updater.py`

 * *Files identical despite different names*

### Comparing `oooenv-0.2.2/oooenv/utils/local_paths.py` & `oooenv-0.2.3/oooenv/utils/local_paths.py`

 * *Files identical despite different names*

### Comparing `oooenv-0.2.2/oooenv/utils/sys_info.py` & `oooenv-0.2.3/oooenv/utils/sys_info.py`

 * *Files identical despite different names*

### Comparing `oooenv-0.2.2/oooenv/utils/uno_paths.py` & `oooenv-0.2.3/oooenv/utils/uno_paths.py`

 * *Files identical despite different names*

### Comparing `oooenv-0.2.2/pyproject.toml` & `oooenv-0.2.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oooenv"
-version = "0.2.2"
+version = "0.2.3"
 description = "Configures a project python environment for LibreOffice UNO."
 authors = [":Barry-Thomas-Paul: Moss <vibrationoflife@protonmail.com>"]
 keywords = ["libreoffice", "macro", "uno", "ooouno", "venv"]
 homepage = "https://github.com/Amourspirit/python_oooenv"
 documentation = "https://github.com/Amourspirit/python_oooenv"
 repository = "https://github.com/Amourspirit/python_oooenv"
 license = "MIT"
```

### Comparing `oooenv-0.2.2/PKG-INFO` & `oooenv-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oooenv
-Version: 0.2.2
+Version: 0.2.3
 Summary: Configures a project python environment for LibreOffice UNO.
 Home-page: https://github.com/Amourspirit/python_oooenv
 License: MIT
 Keywords: libreoffice,macro,uno,ooouno,venv
 Author: :Barry-Thomas-Paul: Moss
 Author-email: vibrationoflife@protonmail.com
 Requires-Python: >=3.8,<4.0
@@ -14,14 +14,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Office/Business
 Project-URL: Documentation, https://github.com/Amourspirit/python_oooenv
 Project-URL: Repository, https://github.com/Amourspirit/python_oooenv
 Description-Content-Type: text/markdown
 
 # OOOENV
```

