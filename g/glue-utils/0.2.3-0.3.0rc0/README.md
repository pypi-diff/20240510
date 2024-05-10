# Comparing `tmp/glue_utils-0.2.3.tar.gz` & `tmp/glue_utils-0.3.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glue_utils-0.2.3.tar", max compression
+gzip compressed data, was "glue_utils-0.3.0rc0.tar", max compression
```

## Comparing `glue_utils-0.2.3.tar` & `glue_utils-0.3.0rc0.tar`

### file list

```diff
@@ -1,9 +1,14 @@
--rw-r--r--   0        0        0     1077 2024-03-06 15:16:48.910706 glue_utils-0.2.3/LICENSE
--rw-r--r--   0        0        0     1138 2024-03-07 09:36:58.526889 glue_utils-0.2.3/README.md
--rw-r--r--   0        0        0     3657 2024-05-05 09:45:57.367172 glue_utils-0.2.3/pyproject.toml
--rw-r--r--   0        0        0       96 2024-05-05 09:45:57.367513 glue_utils-0.2.3/src/glue_utils/__init__.py
--rw-r--r--   0        0        0       68 2024-05-03 09:05:30.885798 glue_utils-0.2.3/src/glue_utils/glueetl/__init__.py
--rw-r--r--   0        0        0     2579 2024-05-05 07:24:30.940613 glue_utils-0.2.3/src/glue_utils/glueetl/job.py
--rw-r--r--   0        0        0     1050 2024-05-05 07:24:30.940979 glue_utils-0.2.3/src/glue_utils/options.py
--rw-r--r--   0        0        0        0 2024-05-03 09:02:47.986990 glue_utils-0.2.3/src/glue_utils/py.typed
--rw-r--r--   0        0        0     2250 1970-01-01 00:00:00.000000 glue_utils-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-03-06 15:16:48.910706 glue_utils-0.3.0rc0/LICENSE
+-rw-r--r--   0        0        0     1138 2024-03-07 09:36:58.526889 glue_utils-0.3.0rc0/README.md
+-rw-r--r--   0        0        0     3828 2024-05-10 12:38:24.110323 glue_utils-0.3.0rc0/pyproject.toml
+-rw-r--r--   0        0        0       85 2024-05-10 12:38:24.110688 glue_utils-0.3.0rc0/src/glue_utils/__init__.py
+-rw-r--r--   0        0        0     1050 2024-05-10 09:44:26.756369 glue_utils-0.3.0rc0/src/glue_utils/options.py
+-rw-r--r--   0        0        0        0 2024-05-03 09:02:47.986990 glue_utils-0.3.0rc0/src/glue_utils/py.typed
+-rw-r--r--   0        0        0      110 2024-05-10 12:17:39.961246 glue_utils-0.3.0rc0/src/glue_utils/pyspark/__init__.py
+-rw-r--r--   0        0        0      674 2024-05-10 12:17:39.961510 glue_utils-0.3.0rc0/src/glue_utils/pyspark/context.py
+-rw-r--r--   0        0        0     2652 2024-05-10 12:17:39.961783 glue_utils-0.3.0rc0/src/glue_utils/pyspark/job.py
+-rw-r--r--   0        0        0        0 2024-05-10 12:17:39.961858 glue_utils-0.3.0rc0/src/glue_utils/pyspark/mixins/__init__.py
+-rw-r--r--   0        0        0      849 2024-05-10 12:17:39.962157 glue_utils-0.3.0rc0/src/glue_utils/pyspark/mixins/connection_types.py
+-rw-r--r--   0        0        0    10346 2024-05-10 12:17:39.962531 glue_utils-0.3.0rc0/src/glue_utils/pyspark/mixins/jdbc.py
+-rw-r--r--   0        0        0    17373 2024-05-10 12:17:39.962785 glue_utils-0.3.0rc0/src/glue_utils/pyspark/mixins/s3.py
+-rw-r--r--   0        0        0     2253 1970-01-01 00:00:00.000000 glue_utils-0.3.0rc0/PKG-INFO
```

### Comparing `glue_utils-0.2.3/LICENSE` & `glue_utils-0.3.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `glue_utils-0.2.3/README.md` & `glue_utils-0.3.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `glue_utils-0.2.3/pyproject.toml` & `glue_utils-0.3.0rc0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 [tool.poetry]
 name = "glue-utils"
-version = "0.2.3"
-# Uncomment this when dependabot has finally been updated to it is 
-# supported by dependabot.
-# package-mode = true
+version = "0.3.0rc0"
+package-mode = true
 description = "Reusable utilities for working with Glue PySpark jobs"
 authors = ["Noel Llevares <dashmug@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/dashmug/glue-utils"
 repository = "https://github.com/dashmug/glue-utils/issues"
 documentation = "https://github.com/dashmug/glue-utils/wiki"
@@ -32,16 +30,18 @@
 [tool.poetry.dependencies]
 python = "^3.9"
 
 [tool.poetry.group.dev.dependencies]
 pytest-randomly = "^3.15.0"
 pytest-cov = "^5.0.0"
 mypy = "^1.10.0"
-ruff = "^0.4.3"
 bumpver = "^2023.1129"
+pytest = "^8.2.0"
+import-linter = "^2.0"
+ruff = "^0.4.4"
 
 [tool.poetry.group.local.dependencies]
 # The "local" dependency group refers to dependencies that already 
 # exist in AWS Glue's runtime. We don't need to install these in the
 # container. We only need them for local (non-container) development to 
 # aid the IDE in providing code completion and type checking.
 # 
@@ -54,39 +54,42 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 line-length = 88
 output-format = "full"
-respect-gitignore = true
 target-version = "py39"
+unsafe-fixes = true
+show-fixes = true
 
 [tool.ruff.lint]
 select = ["ALL"]
 ignore = [
+    "D104",
     "D203",
     "D213",
     # Conflicts with ruff format
     "COM812",
     "ISC001",
     # missing-type-self
     "ANN101",
     # missing-type-cls
     "ANN102",
+    # line-too-long
+    "E501"
 ]
-exclude = [".venv"]
 # # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
 [tool.ruff.lint.mccabe]
 max-complexity = 5
 
 [tool.ruff.lint.per-file-ignores]
-"test/**" = ["S101", "ANN", "ARG001", "ARG002", "PLR2004", "PT", "PD", "D"]
+"test/**" = ["S101", "ANN", "ARG001", "ARG002", "PLR2004", "PLR0913", "PT", "PD", "D"]
 
 [tool.mypy]
 files = "**/*.py"
 python_version = "3.9"
 show_error_codes = true
 pretty = true
 strict = true
@@ -94,20 +97,18 @@
 implicit_reexport = true
 explicit_package_bases = true
 
 [[tool.mypy.overrides]]
 module = "test.*"
 disallow_incomplete_defs = false
 disallow_untyped_defs = false
-disallow_untyped_calls = false
 
 [tool.pytest.ini_options]
 filterwarnings = [
-    "ignore::DeprecationWarning",
-    "ignore::FutureWarning:.*pyspark.*",
+    "ignore::FutureWarning:pyspark.sql.context",
 ]
 
 [tool.coverage.run]
 omit = ["**/test_*.py"]
 
 [tool.coverage.paths]
 source = ["src/glue_utils", "*/site-packages/glue_utils"]
@@ -121,24 +122,32 @@
     "raise AssertionError",
     "raise NotImplementedError",
     "if 0:",
     "if __name__ == .__main__.:",
     "if TYPE_CHECKING:",
     "class .*\\bProtocol\\):",
     "@(abc\\.)?abstractmethod",
+    "@overload",
 ]
 
 [tool.bumpver]
-current_version = "0.2.3"
-version_pattern = "MAJOR.MINOR.PATCH"
+current_version = "0.3.0rc0"
+version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "release: Bump version {old_version} -> {new_version}"
 commit = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
     'current_version = "{version}"',
     'version = "{version}"',
 ]
 "src/glue_utils/__init__.py" = [
     '^__version__ = "{version}"$',
 ]
 
+[tool.importlinter]
+root_package = "glue_utils"
+
+[[tool.importlinter.contracts]]
+name = "Generic code should not import specific code"
+type = "layers"
+layers = ["glue_utils.pyspark", "glue_utils.options"]
```

### Comparing `glue_utils-0.2.3/src/glue_utils/options.py` & `glue_utils-0.3.0rc0/src/glue_utils/options.py`

 * *Files identical despite different names*

### Comparing `glue_utils-0.2.3/PKG-INFO` & `glue_utils-0.3.0rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glue-utils
-Version: 0.2.3
+Version: 0.3.0rc0
 Summary: Reusable utilities for working with Glue PySpark jobs
 Home-page: https://github.com/dashmug/glue-utils
 License: MIT
 Keywords: aws,glue,pyspark,spark,etl,data,data-engineering
 Author: Noel Llevares
 Author-email: dashmug@gmail.com
 Requires-Python: >=3.9,<4.0
```

