# Comparing `tmp/turbofan-0.2.0.tar.gz` & `tmp/turbofan-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbofan-0.2.0.tar", max compression
+gzip compressed data, was "turbofan-0.2.1.tar", max compression
```

## Comparing `turbofan-0.2.0.tar` & `turbofan-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1211 2024-03-30 19:58:06.156642 turbofan-0.2.0/LICENSE
--rw-r--r--   0        0        0      182 2024-03-30 19:58:06.157065 turbofan-0.2.0/README.md
--rw-r--r--   0        0        0     1145 2024-04-09 12:54:03.619200 turbofan-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       24 2024-03-30 19:58:06.160060 turbofan-0.2.0/src/turbofan/__init__.py
--rw-r--r--   0        0        0     1022 2024-03-30 19:58:06.160278 turbofan-0.2.0/src/turbofan/command.py
--rw-r--r--   0        0        0     2847 2024-03-30 19:58:06.160598 turbofan-0.2.0/src/turbofan/database.py
--rw-r--r--   0        0        0      306 2024-03-30 19:58:06.161069 turbofan-0.2.0/src/turbofan/files.py
--rw-r--r--   0        0        0      727 2024-03-30 20:55:50.159301 turbofan-0.2.0/src/turbofan/fixtures.py
--rw-r--r--   0        0        0      809 2024-03-30 19:58:06.161679 turbofan-0.2.0/src/turbofan/project.py
--rw-r--r--   0        0        0      830 1970-01-01 00:00:00.000000 turbofan-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-05-10 06:54:47.362897 turbofan-0.2.1/LICENSE
+-rw-r--r--   0        0        0      182 2024-05-10 06:54:47.363519 turbofan-0.2.1/README.md
+-rw-r--r--   0        0        0     1147 2024-05-10 07:02:32.344246 turbofan-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       24 2024-05-10 06:54:47.366362 turbofan-0.2.1/src/turbofan/__init__.py
+-rw-r--r--   0        0        0     1022 2024-05-10 06:54:47.366611 turbofan-0.2.1/src/turbofan/command.py
+-rw-r--r--   0        0        0     2847 2024-05-10 06:54:47.366845 turbofan-0.2.1/src/turbofan/database.py
+-rw-r--r--   0        0        0      306 2024-05-10 06:54:47.367409 turbofan-0.2.1/src/turbofan/files.py
+-rw-r--r--   0        0        0      727 2024-05-10 06:54:47.367667 turbofan-0.2.1/src/turbofan/fixtures.py
+-rw-r--r--   0        0        0      809 2024-05-10 06:54:47.368207 turbofan-0.2.1/src/turbofan/project.py
+-rw-r--r--   0        0        0      830 1970-01-01 00:00:00.000000 turbofan-0.2.1/PKG-INFO
```

### Comparing `turbofan-0.2.0/LICENSE` & `turbofan-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `turbofan-0.2.0/pyproject.toml` & `turbofan-0.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -12,37 +12,37 @@
 [tool.mypy]
 ignore_missing_imports = true
 # https://stackoverflow.com/questions/62265366/does-mypy-only-type-check-a-function-if-it-declares-a-return-type
 check_untyped_defs = true
 
 [tool.poetry]
 name = "turbofan"
-version = "0.2.0"
+version = "0.2.1"
 description = "Essential Libraries and Tools for Streamlined Development"
 authors = ["Luís Miranda <luistm@gmail.com>"]
 license = "The Unlicence"
 readme = "README.md"
 packages = [
     { include = "turbofan", from = "src" },
 ]
 exclude = ["**/*_test.py", "src/testrig"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 toml = "^0.10.2"
-sqlalchemy = "^2.0.29"
+sqlalchemy = "^2.0.30"
 
 [tool.poetry.group.dev.dependencies]
 bandit = { extras = ["toml"], version = "^1.7.8" }
-black = "^24.3.0"
-coverage = "^7.4.4"
+black = "^24.4.2"
+coverage = "^7.5.1"
 flake8 = "^7.0.0"
 isort = "^5.13.2"
-mypy = "^1.9.0"
-nox = "^2024.3.2"
+mypy = "^1.10.0"
+nox = "^2024.4.15"
 pre-commit = "^3.7.0"
-pytest = "^8.1.1"
-pytest-xdist = "^3.5.0"
+pytest = "^8.2.0"
+pytest-xdist = "^3.6.1"
 types-toml = "^0.10.8.7"
 
 [tool.pytest.ini_options]
 markers = ["integration: tags a test as integration tests"]
```

### Comparing `turbofan-0.2.0/src/turbofan/command.py` & `turbofan-0.2.1/src/turbofan/command.py`

 * *Files identical despite different names*

### Comparing `turbofan-0.2.0/src/turbofan/database.py` & `turbofan-0.2.1/src/turbofan/database.py`

 * *Files identical despite different names*

### Comparing `turbofan-0.2.0/src/turbofan/fixtures.py` & `turbofan-0.2.1/src/turbofan/fixtures.py`

 * *Files identical despite different names*

### Comparing `turbofan-0.2.0/src/turbofan/project.py` & `turbofan-0.2.1/src/turbofan/project.py`

 * *Files identical despite different names*

### Comparing `turbofan-0.2.0/PKG-INFO` & `turbofan-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: turbofan
-Version: 0.2.0
+Version: 0.2.1
 Summary: Essential Libraries and Tools for Streamlined Development
 License: The Unlicence
 Author: Luís Miranda
 Author-email: luistm@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: sqlalchemy (>=2.0.29,<3.0.0)
+Requires-Dist: sqlalchemy (>=2.0.30,<3.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Description-Content-Type: text/markdown
 
 # Turbofan
 
 Essential Libraries and Tools for Streamlined Development
```

