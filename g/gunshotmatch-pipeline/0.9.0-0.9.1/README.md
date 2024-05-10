# Comparing `tmp/gunshotmatch_pipeline-0.9.0.tar.gz` & `tmp/gunshotmatch_pipeline-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gunshotmatch_pipeline-0.9.0.tar", last modified: Fri Mar 15 10:03:30 2024, max compression
+gzip compressed data, was "gunshotmatch_pipeline-0.9.1.tar", last modified: Fri May 10 16:36:58 2024, max compression
```

## Comparing `gunshotmatch_pipeline-0.9.0.tar` & `gunshotmatch_pipeline-0.9.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-15 10:03:30.179926 gunshotmatch_pipeline-0.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6313 2024-03-15 10:03:30.183926 gunshotmatch_pipeline-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-03-15 10:03:30.179926 gunshotmatch_pipeline-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-03-15 10:03:30.183926 gunshotmatch_pipeline-0.9.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-15 10:03:30.175926 gunshotmatch_pipeline-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12176 2024-03-15 10:03:02.931756 gunshotmatch_pipeline-0.9.0/gunshotmatch_pipeline/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-03-15 10:03:02.931756 gunshotmatch_pipeline-0.9.0/gunshotmatch_pipeline/unknowns.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-03-15 10:03:02.931756 gunshotmatch_pipeline-0.9.0/gunshotmatch_pipeline/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-03-15 10:03:02.931756 gunshotmatch_pipeline-0.9.0/gunshotmatch_pipeline/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7270 2024-03-15 10:03:02.931756 gunshotmatch_pipeline-0.9.0/gunshotmatch_pipeline/results.py
--rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-03-15 10:03:02.931756 gunshotmatch_pipeline-0.9.0/gunshotmatch_pipeline/nist_ms_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     5933 2024-03-15 10:03:02.931756 gunshotmatch_pipeline-0.9.0/gunshotmatch_pipeline/exporters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-03-15 10:03:02.931756 gunshotmatch_pipeline-0.9.0/gunshotmatch_pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-03-15 10:03:02.931756 gunshotmatch_pipeline-0.9.0/gunshotmatch_pipeline/peaks.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 10:03:02.931756 gunshotmatch_pipeline-0.9.0/gunshotmatch_pipeline/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-03-15 10:03:02.931756 gunshotmatch_pipeline-0.9.0/gunshotmatch_pipeline/decision_tree/predictions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11327 2024-03-15 10:03:02.931756 gunshotmatch_pipeline-0.9.0/gunshotmatch_pipeline/decision_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11760 2024-03-15 10:03:02.931756 gunshotmatch_pipeline-0.9.0/gunshotmatch_pipeline/decision_tree/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-10 16:36:58.797248 gunshotmatch_pipeline-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-05-10 16:36:58.801248 gunshotmatch_pipeline-0.9.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6313 2024-05-10 16:36:58.801248 gunshotmatch_pipeline-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-05-10 16:36:58.797248 gunshotmatch_pipeline-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-10 16:36:58.797248 gunshotmatch_pipeline-0.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-05-10 16:36:34.565227 gunshotmatch_pipeline-0.9.1/gunshotmatch_pipeline/unknowns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7270 2024-05-10 16:36:34.565227 gunshotmatch_pipeline-0.9.1/gunshotmatch_pipeline/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-05-10 16:36:34.565227 gunshotmatch_pipeline-0.9.1/gunshotmatch_pipeline/nist_ms_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-05-10 16:36:34.565227 gunshotmatch_pipeline-0.9.1/gunshotmatch_pipeline/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-05-10 16:36:34.565227 gunshotmatch_pipeline-0.9.1/gunshotmatch_pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 16:36:34.565227 gunshotmatch_pipeline-0.9.1/gunshotmatch_pipeline/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5933 2024-05-10 16:36:34.565227 gunshotmatch_pipeline-0.9.1/gunshotmatch_pipeline/exporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12176 2024-05-10 16:36:34.565227 gunshotmatch_pipeline-0.9.1/gunshotmatch_pipeline/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-10 16:36:34.565227 gunshotmatch_pipeline-0.9.1/gunshotmatch_pipeline/peaks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-05-10 16:36:34.565227 gunshotmatch_pipeline-0.9.1/gunshotmatch_pipeline/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11327 2024-05-10 16:36:34.565227 gunshotmatch_pipeline-0.9.1/gunshotmatch_pipeline/decision_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11760 2024-05-10 16:36:34.565227 gunshotmatch_pipeline-0.9.1/gunshotmatch_pipeline/decision_tree/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-10 16:36:34.565227 gunshotmatch_pipeline-0.9.1/gunshotmatch_pipeline/decision_tree/predictions.py
```

### Comparing `gunshotmatch_pipeline-0.9.0/PKG-INFO` & `gunshotmatch_pipeline-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.2
 Name: gunshotmatch-pipeline
-Version: 0.9.0
+Version: 0.9.1
 Summary: GunShotMatch Analysis Pipeline
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: MIT
 Home-page: https://github.com/GunShotMatch/gunshotmatch-pipeline
 Project-URL: Issue Tracker, https://github.com/GunShotMatch/gunshotmatch-pipeline/issues
 Project-URL: Source Code, https://github.com/GunShotMatch/gunshotmatch-pipeline
 Project-URL: Documentation, https://gunshotmatch-pipeline.readthedocs.io/en/latest
@@ -124,15 +124,15 @@
 .. |license| image:: https://img.shields.io/github/license/GunShotMatch/gunshotmatch-pipeline
 	:target: https://github.com/GunShotMatch/gunshotmatch-pipeline/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/GunShotMatch/gunshotmatch-pipeline
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/GunShotMatch/gunshotmatch-pipeline/v0.9.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/GunShotMatch/gunshotmatch-pipeline/v0.9.1
 	:target: https://github.com/GunShotMatch/gunshotmatch-pipeline/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/GunShotMatch/gunshotmatch-pipeline
 	:target: https://github.com/GunShotMatch/gunshotmatch-pipeline/commit/master
 	:alt: GitHub last commit
```

### Comparing `gunshotmatch_pipeline-0.9.0/pyproject.toml` & `gunshotmatch_pipeline-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "whey",]
 build-backend = "whey"
 
 [project]
 name = "gunshotmatch-pipeline"
-version = "0.9.0"
+version = "0.9.1"
 description = "GunShotMatch Analysis Pipeline"
 readme = "README.rst"
 keywords = []
 dynamic = []
 dependencies = [
     "attrs>=23.1.0",
     "domdf-python-tools>=3.6.1",
@@ -36,22 +36,21 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: Implementation :: CPython",
     "Typing :: Typed",
 ]
 requires-python = ">=3.8"
 
+[project.license]
+file = "LICENSE"
+
 [[project.authors]]
 name = "Dominic Davis-Foster"
 email = "dominic@davis-foster.co.uk"
 
-
-[project.license]
-file = "LICENSE"
-
 [project.urls]
 Homepage = "https://github.com/GunShotMatch/gunshotmatch-pipeline"
 "Issue Tracker" = "https://github.com/GunShotMatch/gunshotmatch-pipeline/issues"
 "Source Code" = "https://github.com/GunShotMatch/gunshotmatch-pipeline"
 Documentation = "https://gunshotmatch-pipeline.readthedocs.io/en/latest"
 
 [tool.whey]
@@ -83,17 +82,32 @@
 warn_unused_ignores = true
 no_implicit_optional = true
 show_error_codes = true
 
 [tool.snippet-fmt]
 directives = [ "code-block",]
 
+[tool.snippet-fmt.languages.python]
+reformat = true
+
+[tool.snippet-fmt.languages.TOML]
+reformat = true
+
+[tool.snippet-fmt.languages.ini]
+
+[tool.snippet-fmt.languages.json]
+
 [tool.dep_checker]
 allowed_unused = "tomli"
 
+[tool.dep_checker.name_mapping]
+attrs = "attr"
+pymassspec = "pyms"
+scikit-learn = "sklearn"
+
 [tool.sphinx-pyproject]
 github_username = "GunShotMatch"
 github_repository = "gunshotmatch-pipeline"
 author = "Dominic Davis-Foster"
 project = "gunshotmatch-pipeline"
 copyright = "2020-2023 Dominic Davis-Foster"
 language = "en"
@@ -107,26 +121,24 @@
     "sphinxcontrib.toctree_plus",
     "sphinx_toolbox.tweaks.latex_layout",
     "sphinx_toolbox.tweaks.latex_toc",
     "sphinx.ext.intersphinx",
     "sphinx.ext.mathjax",
     "sphinxcontrib.extras_require",
     "sphinx.ext.todo",
-    "sphinxemoji.sphinxemoji",
     "notfound.extension",
     "sphinx_copybutton",
     "sphinxcontrib.default_values",
     "sphinx_debuginfo",
     "sphinx_licenseinfo",
     "seed_intersphinx_mapping",
     "html_section",
     "attr_utils.autoattrs",
     "sphinx_toolbox.more_autosummary.column_widths",
 ]
-sphinxemoji_style = "twemoji"
 gitstamp_fmt = "%d %b %Y"
 templates_path = [ "_templates",]
 html_static_path = [ "_static",]
 source_suffix = ".rst"
 master_doc = "index"
 suppress_warnings = [ "image.nonlocal_uri",]
 pygments_style = "default"
@@ -167,32 +179,17 @@
     "__init__",
     "__new__",
     "__getnewargs__",
     "__abstractmethods__",
     "__hash__",
 ]
 
-[tool.dep_checker.name_mapping]
-attrs = "attr"
-pymassspec = "pyms"
-scikit-learn = "sklearn"
-
 [tool.dependency-dash."requirements.txt"]
 order = 10
 
 [tool.dependency-dash."doc-source/requirements.txt"]
 order = 30
 include = false
 
 [tool.dependency-dash."tests/requirements.txt"]
 order = 20
 include = false
-
-[tool.snippet-fmt.languages.python]
-reformat = true
-
-[tool.snippet-fmt.languages.TOML]
-reformat = true
-
-[tool.snippet-fmt.languages.ini]
-
-[tool.snippet-fmt.languages.json]
```

### Comparing `gunshotmatch_pipeline-0.9.0/README.rst` & `gunshotmatch_pipeline-0.9.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 .. |license| image:: https://img.shields.io/github/license/GunShotMatch/gunshotmatch-pipeline
 	:target: https://github.com/GunShotMatch/gunshotmatch-pipeline/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/GunShotMatch/gunshotmatch-pipeline
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/GunShotMatch/gunshotmatch-pipeline/v0.9.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/GunShotMatch/gunshotmatch-pipeline/v0.9.1
 	:target: https://github.com/GunShotMatch/gunshotmatch-pipeline/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/GunShotMatch/gunshotmatch-pipeline
 	:target: https://github.com/GunShotMatch/gunshotmatch-pipeline/commit/master
 	:alt: GitHub last commit
```

### Comparing `gunshotmatch_pipeline-0.9.0/LICENSE` & `gunshotmatch_pipeline-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gunshotmatch_pipeline-0.9.0/gunshotmatch_pipeline/projects.py` & `gunshotmatch_pipeline-0.9.1/gunshotmatch_pipeline/projects.py`

 * *Files identical despite different names*

### Comparing `gunshotmatch_pipeline-0.9.0/gunshotmatch_pipeline/unknowns.py` & `gunshotmatch_pipeline-0.9.1/gunshotmatch_pipeline/unknowns.py`

 * *Files identical despite different names*

### Comparing `gunshotmatch_pipeline-0.9.0/gunshotmatch_pipeline/utils.py` & `gunshotmatch_pipeline-0.9.1/gunshotmatch_pipeline/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,14 +71,14 @@
 		"Benzenamine, 4-nitro-N-phenyl-": "4-NDPA",
 		"Benzenamine, 2-nitro-N-phenyl-": "2-NDPA",
 		"N,N'-Diethyl-N,N'-diphenylurea": "Ethyl Centralite",
 		"Benzene, nitro-": "Nitrobenzene",
 		"Benzene, 2-methyl-1,3-dinitro-": "2,6-DNT",
 		"Benzene, 1-methyl-2,3-dinitro-": "2,3-DNT",
 		"Benzene, 1-methyl-2,4-dinitro-": "2,4-DNT",
-		"Benzene, 1-methyl-2-nitro-": "1-Methyl-2-nitroenzene",
+		"Benzene, 1-methyl-2-nitro-": "1-Methyl-2-nitrobenzene",
 		"Phenol, 2-nitro-": "2-Nitrophenol",
 		"Benzene, 1-methyl-4-nitro-": "4-Nitrotoluene",
 		"Benzene, 1-methyl-3-nitro-": "3-Nitrotoluene",
 		"Benzenamine, N-ethyl-N-nitroso-": "N-Nitroso-N-ethylaniline",
 		"Phenol, 4-methyl-2-nitro-": "4-Methyl-2-nitrophenol",
 		})
```

### Comparing `gunshotmatch_pipeline-0.9.0/gunshotmatch_pipeline/config.py` & `gunshotmatch_pipeline-0.9.1/gunshotmatch_pipeline/config.py`

 * *Files identical despite different names*

### Comparing `gunshotmatch_pipeline-0.9.0/gunshotmatch_pipeline/results.py` & `gunshotmatch_pipeline-0.9.1/gunshotmatch_pipeline/results.py`

 * *Files identical despite different names*

### Comparing `gunshotmatch_pipeline-0.9.0/gunshotmatch_pipeline/nist_ms_search.py` & `gunshotmatch_pipeline-0.9.1/gunshotmatch_pipeline/nist_ms_search.py`

 * *Files identical despite different names*

### Comparing `gunshotmatch_pipeline-0.9.0/gunshotmatch_pipeline/exporters.py` & `gunshotmatch_pipeline-0.9.1/gunshotmatch_pipeline/exporters.py`

 * *Files identical despite different names*

### Comparing `gunshotmatch_pipeline-0.9.0/gunshotmatch_pipeline/__init__.py` & `gunshotmatch_pipeline-0.9.1/gunshotmatch_pipeline/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 from gunshotmatch_pipeline.peaks import align_and_filter_peaks, prepare_peak_list
 
 __all__ = ("prepare_datafile", "project_from_repeats")
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2020-2023 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "0.9.0"
+__version__: str = "0.9.1"
 __email__: str = "dominic@davis-foster.co.uk"
 
 
 def prepare_datafile(
 		filename: PathLike,
 		method: Method,
 		verbose: bool = False,
```

### Comparing `gunshotmatch_pipeline-0.9.0/gunshotmatch_pipeline/peaks.py` & `gunshotmatch_pipeline-0.9.1/gunshotmatch_pipeline/peaks.py`

 * *Files identical despite different names*

### Comparing `gunshotmatch_pipeline-0.9.0/gunshotmatch_pipeline/decision_tree/predictions.py` & `gunshotmatch_pipeline-0.9.1/gunshotmatch_pipeline/decision_tree/predictions.py`

 * *Files identical despite different names*

### Comparing `gunshotmatch_pipeline-0.9.0/gunshotmatch_pipeline/decision_tree/__init__.py` & `gunshotmatch_pipeline-0.9.1/gunshotmatch_pipeline/decision_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `gunshotmatch_pipeline-0.9.0/gunshotmatch_pipeline/decision_tree/export.py` & `gunshotmatch_pipeline-0.9.1/gunshotmatch_pipeline/decision_tree/export.py`

 * *Files identical despite different names*

