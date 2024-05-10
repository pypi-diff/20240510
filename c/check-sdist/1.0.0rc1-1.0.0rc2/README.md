# Comparing `tmp/check_sdist-1.0.0rc1.tar.gz` & `tmp/check_sdist-1.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue May  7 21:35:39 2024, max compression
+gzip compressed data, last modified: Fri May 10 15:15:28 2024, max compression
```

## Comparing `check_sdist-1.0.0rc1.tar` & `check_sdist-1.0.0rc2.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0     2366 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      500 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0     1576 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/noxfile.py
--rw-r--r--   0        0        0     2246 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      224 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/.github/matchers/pylint.json
--rw-r--r--   0        0        0      669 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1586 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/.github/workflows/ci.yml
--rwxr-xr-x   0        0        0     1005 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/scripts/generate_schema.py
--rw-r--r--   0        0        0      207 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/src/check_sdist/__init__.py
--rw-r--r--   0        0        0     5182 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/src/check_sdist/__main__.py
--rw-r--r--   0        0        0      642 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/src/check_sdist/git.py
--rw-r--r--   0        0        0     1898 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/src/check_sdist/inject.py
--rw-r--r--   0        0        0        0 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/src/check_sdist/py.typed
--rw-r--r--   0        0        0      452 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/src/check_sdist/schema.py
--rw-r--r--   0        0        0     1326 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/src/check_sdist/sdist.py
--rw-r--r--   0        0        0        0 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/src/check_sdist/_compat/__init__.py
--rw-r--r--   0        0        0      238 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/src/check_sdist/_compat/importlib.py
--rw-r--r--   0        0        0      161 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/src/check_sdist/_compat/tomllib.py
--rw-r--r--   0        0        0      169 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/src/check_sdist/resources/__init__.py
--rw-r--r--   0        0        0     1008 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/src/check_sdist/resources/check-sdist.schema.json
--rw-r--r--   0        0        0      100 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/src/check_sdist/resources/default-ignore.txt
--rw-r--r--   0        0        0      272 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/src/check_sdist/resources/junk-paths.txt
--rw-r--r--   0        0        0      471 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/tests/downstream.toml
--rw-r--r--   0        0        0      321 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/tests/test_cli.py
--rw-r--r--   0        0        0      817 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/tests/test_downstream.py
--rw-r--r--   0        0        0     1418 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/tests/test_inject.py
--rw-r--r--   0        0        0      758 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/tests/test_package.py
--rw-r--r--   0        0        0     1131 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/tests/test_validate_pyproject.py
--rw-r--r--   0        0        0     2217 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/.gitignore
--rw-r--r--   0        0        0     1526 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/LICENSE
--rw-r--r--   0        0        0     3635 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/README.md
--rw-r--r--   0        0        0     3600 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0     5181 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     2366 2024-05-10 15:15:28.000000 check_sdist-1.0.0rc2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      500 2024-05-10 15:15:28.000000 check_sdist-1.0.0rc2/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0     1576 2024-05-10 15:15:28.000000 check_sdist-1.0.0rc2/noxfile.py
+-rw-r--r--   0        0        0     2246 2024-05-10 15:15:28.000000 check_sdist-1.0.0rc2/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      224 2024-05-10 15:15:28.000000 check_sdist-1.0.0rc2/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2024-05-10 15:15:28.000000 check_sdist-1.0.0rc2/.github/release.yml
+-rw-r--r--   0        0        0      668 2024-05-10 15:15:28.000000 check_sdist-1.0.0rc2/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      669 2024-05-10 15:15:28.000000 check_sdist-1.0.0rc2/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1586 2024-05-10 15:15:28.000000 check_sdist-1.0.0rc2/.github/workflows/ci.yml
+-rwxr-xr-x   0        0        0     1005 2024-05-10 15:15:28.000000 check_sdist-1.0.0rc2/scripts/generate_schema.py
+-rw-r--r--   0        0        0      207 2024-05-10 15:15:28.000000 check_sdist-1.0.0rc2/src/check_sdist/__init__.py
+-rw-r--r--   0        0        0     5182 2024-05-10 15:15:28.000000 check_sdist-1.0.0rc2/src/check_sdist/__main__.py
+-rw-r--r--   0        0        0      642 2024-05-10 15:15:28.000000 check_sdist-1.0.0rc2/src/check_sdist/git.py
+-rw-r--r--   0        0        0     1898 2024-05-10 15:15:28.000000 check_sdist-1.0.0rc2/src/check_sdist/inject.py
+-rw-r--r--   0        0        0        0 2024-05-10 15:15:28.000000 check_sdist-1.0.0rc2/src/check_sdist/py.typed
+-rw-r--r--   0        0        0      452 2024-05-10 15:15:28.000000 check_sdist-1.0.0rc2/src/check_sdist/schema.py
+-rw-r--r--   0        0        0     1293 2024-05-10 15:15:28.000000 check_sdist-1.0.0rc2/src/check_sdist/sdist.py
+-rw-r--r--   0        0        0        0 2024-05-10 15:15:28.000000 check_sdist-1.0.0rc2/src/check_sdist/_compat/__init__.py
+-rw-r--r--   0        0        0      238 2024-05-10 15:15:28.000000 check_sdist-1.0.0rc2/src/check_sdist/_compat/importlib.py
+-rw-r--r--   0        0        0      161 2024-05-10 15:15:28.000000 check_sdist-1.0.0rc2/src/check_sdist/_compat/tomllib.py
+-rw-r--r--   0        0        0      169 2024-05-10 15:15:28.000000 check_sdist-1.0.0rc2/src/check_sdist/resources/__init__.py
+-rw-r--r--   0        0        0     1008 2024-05-10 15:15:28.000000 check_sdist-1.0.0rc2/src/check_sdist/resources/check-sdist.schema.json
+-rw-r--r--   0        0        0      100 2024-05-10 15:15:28.000000 check_sdist-1.0.0rc2/src/check_sdist/resources/default-ignore.txt
+-rw-r--r--   0        0        0      272 2024-05-10 15:15:28.000000 check_sdist-1.0.0rc2/src/check_sdist/resources/junk-paths.txt
+-rw-r--r--   0        0        0      471 2024-05-10 15:15:28.000000 check_sdist-1.0.0rc2/tests/downstream.toml
+-rw-r--r--   0        0        0      321 2024-05-10 15:15:28.000000 check_sdist-1.0.0rc2/tests/test_cli.py
+-rw-r--r--   0        0        0      817 2024-05-10 15:15:28.000000 check_sdist-1.0.0rc2/tests/test_downstream.py
+-rw-r--r--   0        0        0     1418 2024-05-10 15:15:28.000000 check_sdist-1.0.0rc2/tests/test_inject.py
+-rw-r--r--   0        0        0      758 2024-05-10 15:15:28.000000 check_sdist-1.0.0rc2/tests/test_package.py
+-rw-r--r--   0        0        0     1131 2024-05-10 15:15:28.000000 check_sdist-1.0.0rc2/tests/test_validate_pyproject.py
+-rw-r--r--   0        0        0     2217 2024-05-10 15:15:28.000000 check_sdist-1.0.0rc2/.gitignore
+-rw-r--r--   0        0        0     1526 2024-05-10 15:15:28.000000 check_sdist-1.0.0rc2/LICENSE
+-rw-r--r--   0        0        0     3635 2024-05-10 15:15:28.000000 check_sdist-1.0.0rc2/README.md
+-rw-r--r--   0        0        0     3600 2024-05-10 15:15:28.000000 check_sdist-1.0.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     5181 2024-05-10 15:15:28.000000 check_sdist-1.0.0rc2/PKG-INFO
```

### Comparing `check_sdist-1.0.0rc1/.pre-commit-config.yaml` & `check_sdist-1.0.0rc2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `check_sdist-1.0.0rc1/noxfile.py` & `check_sdist-1.0.0rc2/noxfile.py`

 * *Files identical despite different names*

### Comparing `check_sdist-1.0.0rc1/.github/CONTRIBUTING.md` & `check_sdist-1.0.0rc2/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `check_sdist-1.0.0rc1/.github/matchers/pylint.json` & `check_sdist-1.0.0rc2/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `check_sdist-1.0.0rc1/.github/workflows/cd.yml` & `check_sdist-1.0.0rc2/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `check_sdist-1.0.0rc1/.github/workflows/ci.yml` & `check_sdist-1.0.0rc2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `check_sdist-1.0.0rc1/scripts/generate_schema.py` & `check_sdist-1.0.0rc2/scripts/generate_schema.py`

 * *Files identical despite different names*

### Comparing `check_sdist-1.0.0rc1/src/check_sdist/__main__.py` & `check_sdist-1.0.0rc2/src/check_sdist/__main__.py`

 * *Files identical despite different names*

### Comparing `check_sdist-1.0.0rc1/src/check_sdist/git.py` & `check_sdist-1.0.0rc2/src/check_sdist/git.py`

 * *Files identical despite different names*

### Comparing `check_sdist-1.0.0rc1/src/check_sdist/inject.py` & `check_sdist-1.0.0rc2/src/check_sdist/inject.py`

 * *Files identical despite different names*

### Comparing `check_sdist-1.0.0rc1/src/check_sdist/sdist.py` & `check_sdist-1.0.0rc2/src/check_sdist/sdist.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,26 +17,24 @@
         cmd = [
             sys.executable,
             "-m",
             "build",
             "--sdist",
             "--outdir",
             outdir,
-            f"--installer={installer}",
+            f"--installer={installer}" if isolated else "--no-isolation",
         ]
-        if not isolated:
-            cmd.append("--no-isolation")
         subprocess.run(cmd, check=True, cwd=source_dir)
 
         (outpath,) = Path(outdir).glob("*.tar.gz")
 
         with tarfile.open(outpath) as tar:
             prefixes = {n.split("/", maxsplit=1)[0] for n in tar.getnames()}
             if len(prefixes) != 1:
-                msg = f"malformted SDist, contains multiple packages {prefixes}"
+                msg = f"malformed SDist, contains multiple packages {prefixes}"
                 raise AssertionError(msg)
             return frozenset(
                 t.name.split("/", maxsplit=1)[1]
                 for t in tar.getmembers()
                 if t.isfile() or t.issym()
             )
```

### Comparing `check_sdist-1.0.0rc1/src/check_sdist/resources/check-sdist.schema.json` & `check_sdist-1.0.0rc2/src/check_sdist/resources/check-sdist.schema.json`

 * *Files identical despite different names*

### Comparing `check_sdist-1.0.0rc1/tests/test_downstream.py` & `check_sdist-1.0.0rc2/tests/test_downstream.py`

 * *Files identical despite different names*

### Comparing `check_sdist-1.0.0rc1/tests/test_inject.py` & `check_sdist-1.0.0rc2/tests/test_inject.py`

 * *Files identical despite different names*

### Comparing `check_sdist-1.0.0rc1/tests/test_package.py` & `check_sdist-1.0.0rc2/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `check_sdist-1.0.0rc1/tests/test_validate_pyproject.py` & `check_sdist-1.0.0rc2/tests/test_validate_pyproject.py`

 * *Files identical despite different names*

### Comparing `check_sdist-1.0.0rc1/.gitignore` & `check_sdist-1.0.0rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `check_sdist-1.0.0rc1/LICENSE` & `check_sdist-1.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `check_sdist-1.0.0rc1/README.md` & `check_sdist-1.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `check_sdist-1.0.0rc1/pyproject.toml` & `check_sdist-1.0.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `check_sdist-1.0.0rc1/PKG-INFO` & `check_sdist-1.0.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: check-sdist
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: Check the contents of an SDist vs. git
 Project-URL: Homepage, https://github.com/henryiii/check-sdist
 Project-URL: Bug Tracker, https://github.com/henryiii/check-sdist/issues
 Project-URL: Changelog, https://github.com/henryiii/check-sdist/releases
 Author-email: Henry Schreiner <henryschreineriii@gmail.com>
 License-File: LICENSE
 Keywords: lint,packaging,sdist
```

