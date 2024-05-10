# Comparing `tmp/autoimport-1.3.3.tar.gz` & `tmp/autoimport-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoimport-1.3.3.tar", last modified: Wed Feb  8 16:52:36 2023, max compression
+gzip compressed data, was "autoimport-1.4.0.tar", last modified: Thu Nov 23 11:09:49 2023, max compression
```

## Comparing `autoimport-1.3.3.tar` & `autoimport-1.4.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    35150 2021-11-23 09:35:47.000000 autoimport-1.3.3/LICENSE
--rw-r--r--   0        0        0     1402 2022-09-15 09:31:19.517820 autoimport-1.3.3/README.md
--rw-r--r--   0        0        0     7139 2023-02-08 16:52:29.727006 autoimport-1.3.3/pyproject.toml
--rw-r--r--   0        0        0      346 2022-05-02 16:14:19.000000 autoimport-1.3.3/src/autoimport/__init__.py
--rw-r--r--   0        0        0      333 2022-10-14 11:54:18.025698 autoimport-1.3.3/src/autoimport/__main__.py
--rw-r--r--   0        0        0      971 2022-05-02 16:14:19.000000 autoimport-1.3.3/src/autoimport/entrypoints/__init__.py
--rw-r--r--   0        0        0     3048 2022-10-14 11:54:18.025698 autoimport-1.3.3/src/autoimport/entrypoints/cli.py
--rw-r--r--   0        0        0    19984 2023-02-08 16:52:25.674951 autoimport-1.3.3/src/autoimport/model.py
--rw-r--r--   0        0        0        0 2020-11-25 08:51:28.000000 autoimport-1.3.3/src/autoimport/py.typed
--rw-r--r--   0        0        0     2236 2022-11-03 14:21:08.039155 autoimport-1.3.3/src/autoimport/services.py
--rw-r--r--   0        0        0      644 2023-02-08 16:52:29.639005 autoimport-1.3.3/src/autoimport/version.py
--rw-r--r--   0        0        0        0 2020-11-25 08:51:28.000000 autoimport-1.3.3/tests/__init__.py
--rw-r--r--   0        0        0      723 2022-11-25 19:30:36.188496 autoimport-1.3.3/tests/conftest.py
--rw-r--r--   0        0        0        0 2020-11-25 08:51:28.000000 autoimport-1.3.3/tests/e2e/__init__.py
--rw-r--r--   0        0        0    11185 2023-02-08 16:52:25.674951 autoimport-1.3.3/tests/e2e/test_cli.py
--rw-r--r--   0        0        0        0 2020-11-25 08:51:28.000000 autoimport-1.3.3/tests/unit/__init__.py
--rw-r--r--   0        0        0     2093 2022-09-15 09:31:19.529820 autoimport-1.3.3/tests/unit/test_entrypoints.py
--rw-r--r--   0        0        0     2026 2022-09-15 09:31:19.529820 autoimport-1.3.3/tests/unit/test_extract_package.py
--rw-r--r--   0        0        0    25780 2023-02-08 16:52:25.674951 autoimport-1.3.3/tests/unit/test_services.py
--rw-r--r--   0        0        0      416 2022-09-15 09:31:19.529820 autoimport-1.3.3/tests/unit/test_version.py
--rw-r--r--   0        0        0     2434 1970-01-01 00:00:00.000000 autoimport-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0    35150 2021-11-23 09:35:47.000000 autoimport-1.4.0/LICENSE
+-rw-r--r--   0        0        0     1402 2023-08-30 08:51:25.775829 autoimport-1.4.0/README.md
+-rw-r--r--   0        0        0     7128 2023-11-23 11:09:49.383810 autoimport-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      346 2022-05-02 16:14:19.000000 autoimport-1.4.0/src/autoimport/__init__.py
+-rw-r--r--   0        0        0      333 2022-10-14 11:54:18.025698 autoimport-1.4.0/src/autoimport/__main__.py
+-rw-r--r--   0        0        0      971 2022-05-02 16:14:19.000000 autoimport-1.4.0/src/autoimport/entrypoints/__init__.py
+-rw-r--r--   0        0        0     3053 2023-11-05 13:11:23.027027 autoimport-1.4.0/src/autoimport/entrypoints/cli.py
+-rw-r--r--   0        0        0    19974 2023-03-24 11:43:06.109135 autoimport-1.4.0/src/autoimport/model.py
+-rw-r--r--   0        0        0        0 2020-11-25 08:51:28.000000 autoimport-1.4.0/src/autoimport/py.typed
+-rw-r--r--   0        0        0     2236 2023-03-24 11:43:06.093135 autoimport-1.4.0/src/autoimport/services.py
+-rw-r--r--   0        0        0      644 2023-11-23 11:09:40.647685 autoimport-1.4.0/src/autoimport/version.py
+-rw-r--r--   0        0        0        0 2020-11-25 08:51:28.000000 autoimport-1.4.0/tests/__init__.py
+-rw-r--r--   0        0        0      723 2022-11-25 19:30:36.188496 autoimport-1.4.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-11-25 08:51:28.000000 autoimport-1.4.0/tests/e2e/__init__.py
+-rw-r--r--   0        0        0    11185 2023-03-24 11:43:06.081135 autoimport-1.4.0/tests/e2e/test_cli.py
+-rw-r--r--   0        0        0        0 2020-11-25 08:51:28.000000 autoimport-1.4.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0     2054 2023-08-04 14:00:43.765007 autoimport-1.4.0/tests/unit/test_entrypoints.py
+-rw-r--r--   0        0        0     2026 2022-09-15 09:31:19.529820 autoimport-1.4.0/tests/unit/test_extract_package.py
+-rw-r--r--   0        0        0    25780 2023-03-24 11:43:06.133135 autoimport-1.4.0/tests/unit/test_services.py
+-rw-r--r--   0        0        0      416 2022-09-15 09:31:19.529820 autoimport-1.4.0/tests/unit/test_version.py
+-rw-r--r--   0        0        0     2656 1970-01-01 00:00:00.000000 autoimport-1.4.0/PKG-INFO
```

### Comparing `autoimport-1.3.3/LICENSE` & `autoimport-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autoimport-1.3.3/README.md` & `autoimport-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `autoimport-1.3.3/pyproject.toml` & `autoimport-1.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.3.3"
+version = "1.4.0"
 tag_format = "$version"
 version_files = [
     "pyproject.toml:version",
     "src/autoimport/version.py",
 ]
 
 [tool.autoimport.common_statements]
 factories = "from tests import factories"
 
 [tool.pdm]
+allow_prereleases = true
+
+[tool.pdm.build]
+editable-backend = "path"
 package-dir = "src"
 source-includes = [
     "tests/",
 ]
-editable-backend = "path"
-allow_prereleases = true
 
 [tool.pdm.version]
-from = "src/autoimport/version.py"
-
-[tool.pdm.build]
-editable-backend = "path"
+source = "file"
+path = "src/autoimport/version.py"
 
 [tool.pdm.overrides]
 importlib-metadata = ">=3.10"
 
 [tool.pdm.dev-dependencies]
 lint = [
     "yamllint>=1.27.1",
@@ -317,42 +317,42 @@
 warn_untyped_fields = true
 
 [project]
 dynamic = []
 authors = [
     { name = "Lyz", email = "lyz@riseup.net" },
 ]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dependencies = [
     "click>=8.1.3",
     "autoflake>=1.4",
     "pyprojroot>=0.2.0",
     "sh>=1.14.2",
     "maison>=1.4.0",
-    "xdg>=5.1.1",
+    "xdg>=6.0.0",
 ]
 name = "autoimport"
 description = "Autoimport missing python libraries."
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: Unix",
     "Operating System :: POSIX",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Utilities",
     "Natural Language :: English",
 ]
-version = "1.3.3"
+version = "1.4.0"
 
 [project.license]
 text = "GPL-3.0-only"
 
 [project.urls]
 Issues = "https://github.com/lyz-code/autoimport/issues"
 homepage = "https://github.com/lyz-code/autoimport"
@@ -361,10 +361,10 @@
 [project.scripts]
 autoimport = "autoimport.entrypoints.cli:cli"
 
 [project.optional-dependencies]
 
 [build-system]
 requires = [
-    "pdm-pep517",
+    "pdm-backend",
 ]
-build-backend = "pdm.pep517.api"
+build-backend = "pdm.backend"
```

### Comparing `autoimport-1.3.3/src/autoimport/entrypoints/__init__.py` & `autoimport-1.4.0/src/autoimport/entrypoints/__init__.py`

 * *Files identical despite different names*

### Comparing `autoimport-1.3.3/src/autoimport/entrypoints/cli.py` & `autoimport-1.4.0/src/autoimport/entrypoints/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 """Command line interface definition."""
 
 import logging
-from io import TextIOWrapper
 from pathlib import Path
-from typing import Any, List, Optional, Sequence, Tuple, Union
+from typing import IO, Any, List, Optional, Sequence, Tuple, Union
 
 import click
+
+# Migrate away from xdg to xdg-base-dirs once only Python >= 3.10 is supported
+# https://github.com/lyz-code/autoimport/issues/239
 import xdg
 from maison.config import ProjectConfig
 
 from autoimport import services, version
 
 log = logging.getLogger(__name__)
 
-FileStreams = Union[TextIOWrapper, Sequence[TextIOWrapper]]
-NestedSequence = Sequence[FileStreams]
-
 
-def get_files(source_path: str) -> Sequence[TextIOWrapper]:
+def get_files(source_path: str) -> List[IO[Any]]:
     """Get all files recursively from the given source path."""
     files = []
     for py_file in Path(source_path).glob("**/*.py"):
         if py_file.is_file():
             files.append(click.File("r+").convert(py_file, None, None))
     return files
 
@@ -43,30 +42,30 @@
     """Custom parameter type that accepts either a directory or file."""
 
     def convert(
         self,
         value: Union[str, Path],
         param: Optional[click.Parameter],
         ctx: Optional[click.Context],
-    ) -> FileStreams:
+    ) -> List[IO[Any]]:
         """Convert the value to the correct type."""
         try:
-            return click.File("r+").convert(value, param, ctx)
+            return [click.File("r+").convert(value, param, ctx)]
         except click.BadParameter:
             path = click.Path(exists=True).convert(value, param, ctx)
-            return get_files(path)
+            return get_files(str(path))
 
 
 @click.command()
 @click.version_option(version="", message=version.version_info())
 @click.option("--config-file", default=None)
 @click.option("--ignore-init-modules", is_flag=True, help="Ignore __init__.py files.")
 @click.argument("files", type=FileOrDir(), nargs=-1)
 def cli(
-    files: NestedSequence,
+    files: List[IO[Any]],
     config_file: Optional[str] = None,
     ignore_init_modules: bool = False,
 ) -> None:
     """Corrects the source code of the specified files."""
     # Compose configuration
     config_files: List[str] = []
```

### Comparing `autoimport-1.3.3/src/autoimport/model.py` & `autoimport-1.4.0/src/autoimport/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -354,16 +354,16 @@
 
         Returns:
             import_string: String required to import the package.
         """
         # Find the package name
         try:
             project_package = os.path.basename(here()).replace("-", "_")
-        except RecursionError:  # pragma: no cover
-            # I don't know how to make a test that raises this error :(
+        except RuntimeError:  # pragma: no cover
+            # I don't know how to make a test that raises it :(
             # To manually reproduce, follow the steps of
             # https://github.com/lyz-code/autoimport/issues/131
             return None
         package_objects = extract_package_objects(project_package)
 
         # nocover: as the tests are run inside the autoimport virtualenv, it will
         # always find the objects on that package
```

### Comparing `autoimport-1.3.3/src/autoimport/services.py` & `autoimport-1.4.0/src/autoimport/services.py`

 * *Files identical despite different names*

### Comparing `autoimport-1.3.3/src/autoimport/version.py` & `autoimport-1.4.0/src/autoimport/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import platform
 import sys
 from textwrap import dedent
 
 # Do not edit the version manually, let `make bump` do it.
 
-__version__ = "1.3.3"
+__version__ = "1.4.0"
 
 
 def version_info() -> str:
     """Display the version of the program, python and the platform."""
     return dedent(
         f"""\
         ------------------------------------------------------------------
```

### Comparing `autoimport-1.3.3/tests/conftest.py` & `autoimport-1.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `autoimport-1.3.3/tests/e2e/test_cli.py` & `autoimport-1.4.0/tests/e2e/test_cli.py`

 * *Files identical despite different names*

### Comparing `autoimport-1.3.3/tests/unit/test_entrypoints.py` & `autoimport-1.4.0/tests/unit/test_entrypoints.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,17 +40,16 @@
 
 def test_custom_param_type_works_with_file(test_dir: Path) -> None:
     """Ensure the custom param type can be parsed a file."""
     param_type = FileOrDir()
 
     result = param_type.convert(test_dir / "test_file1.py", None, None)
 
-    assert isinstance(result, TextIOWrapper)
-    assert re.match(r".*file[1-2].py", result.name)
-    result.close()
+    assert re.match(r".*file[1-2].py", result[0].name)
+    result[0].close()
 
 
 @pytest.mark.parametrize("filename", ["h.py", "new_dir"])
 def test_custom_param_type_with_non_existing_files(
     test_dir: Path, filename: str
 ) -> None:
     """Ensure an error occurs when a non existing file or dir is parsed."""
```

### Comparing `autoimport-1.3.3/tests/unit/test_extract_package.py` & `autoimport-1.4.0/tests/unit/test_extract_package.py`

 * *Files identical despite different names*

### Comparing `autoimport-1.3.3/tests/unit/test_services.py` & `autoimport-1.4.0/tests/unit/test_services.py`

 * *Files identical despite different names*

### Comparing `autoimport-1.3.3/PKG-INFO` & `autoimport-1.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 Metadata-Version: 2.1
 Name: autoimport
-Version: 1.3.3
+Version: 1.4.0
 Summary: Autoimport missing python libraries.
+Home-page: https://github.com/lyz-code/autoimport
+Author-Email: Lyz <lyz@riseup.net>
 License: GPL-3.0-only
-Author-email: Lyz <lyz@riseup.net>
-Requires-Python: >=3.7
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Natural Language :: English
-Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
+Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
+Classifier: Natural Language :: English
 Project-URL: Issues, https://github.com/lyz-code/autoimport/issues
-Project-URL: documentation, https://lyz-code.github.io/autoimport
-Project-URL: homepage, https://github.com/lyz-code/autoimport
+Project-URL: Homepage, https://github.com/lyz-code/autoimport
+Project-URL: Documentation, https://lyz-code.github.io/autoimport
+Requires-Python: >=3.8
+Requires-Dist: click>=8.1.3
+Requires-Dist: autoflake>=1.4
+Requires-Dist: pyprojroot>=0.2.0
+Requires-Dist: sh>=1.14.2
+Requires-Dist: maison>=1.4.0
+Requires-Dist: xdg>=6.0.0
 Description-Content-Type: text/markdown
 
 # Autoimport
 
 [![Actions Status](https://github.com/lyz-code/autoimport/workflows/Tests/badge.svg)](https://github.com/lyz-code/autoimport/actions)
 [![Actions Status](https://github.com/lyz-code/autoimport/workflows/Build/badge.svg)](https://github.com/lyz-code/autoimport/actions)
 [![Coverage Status](https://coveralls.io/repos/github/lyz-code/autoimport/badge.svg?branch=main)](https://coveralls.io/github/lyz-code/autoimport?branch=main)
@@ -56,8 +63,7 @@
 For guidance on setting up a development environment, and how to make
 a contribution to *autoimport*, see [Contributing to
 autoimport](https://lyz-code.github.io/autoimport/contributing).
 
 ## License
 
 GPLv3
-
```

