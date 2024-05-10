# Comparing `tmp/dbt_score-0.1.0a0.tar.gz` & `tmp/dbt_score-0.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_score-0.1.0a0.tar", last modified: Wed May  8 13:37:16 2024, max compression
+gzip compressed data, was "dbt_score-0.1.0b1.tar", last modified: Fri May 10 12:36:10 2024, max compression
```

## Comparing `dbt_score-0.1.0a0.tar` & `dbt_score-0.1.0b1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1079 2024-05-08 13:37:01.484995 dbt_score-0.1.0a0/LICENSE.txt
--rw-r--r--   0        0        0     1683 2024-05-08 13:37:01.484995 dbt_score-0.1.0a0/README.md
--rw-r--r--   0        0        0     1711 2024-05-08 13:37:16.953051 dbt_score-0.1.0a0/pyproject.toml
--rw-r--r--   0        0        0      195 2024-05-08 13:37:01.488995 dbt_score-0.1.0a0/src/dbt_score/__init__.py
--rwxr-xr-x   0        0        0      546 2024-05-08 13:37:01.488995 dbt_score-0.1.0a0/src/dbt_score/__main__.py
--rw-r--r--   0        0        0     1677 2024-05-08 13:37:01.488995 dbt_score-0.1.0a0/src/dbt_score/cli.py
--rw-r--r--   0        0        0     2673 2024-05-08 13:37:01.488995 dbt_score-0.1.0a0/src/dbt_score/evaluation.py
--rw-r--r--   0        0        0      318 2024-05-08 13:37:01.488995 dbt_score-0.1.0a0/src/dbt_score/exceptions.py
--rw-r--r--   0        0        0      710 2024-05-08 13:37:01.488995 dbt_score-0.1.0a0/src/dbt_score/formatters/__init__.py
--rw-r--r--   0        0        0     1541 2024-05-08 13:37:01.488995 dbt_score-0.1.0a0/src/dbt_score/formatters/human_readable_formatter.py
--rw-r--r--   0        0        0      881 2024-05-08 13:37:01.488995 dbt_score-0.1.0a0/src/dbt_score/lint.py
--rw-r--r--   0        0        0     9041 2024-05-08 13:37:01.488995 dbt_score-0.1.0a0/src/dbt_score/models.py
--rw-r--r--   0        0        0      932 2024-05-08 13:37:01.488995 dbt_score-0.1.0a0/src/dbt_score/parse.py
--rw-r--r--   0        0        0     3606 2024-05-08 13:37:01.488995 dbt_score-0.1.0a0/src/dbt_score/rule.py
--rw-r--r--   0        0        0     2068 2024-05-08 13:37:01.488995 dbt_score-0.1.0a0/src/dbt_score/rule_registry.py
--rw-r--r--   0        0        0       13 2024-05-08 13:37:01.488995 dbt_score-0.1.0a0/src/dbt_score/rules/__init__.py
--rw-r--r--   0        0        0      714 2024-05-08 13:37:01.488995 dbt_score-0.1.0a0/src/dbt_score/rules/generic.py
--rw-r--r--   0        0        0     1981 2024-05-08 13:37:01.488995 dbt_score-0.1.0a0/src/dbt_score/scoring.py
--rw-r--r--   0        0        0       30 2024-05-08 13:37:01.488995 dbt_score-0.1.0a0/tests/__init__.py
--rw-r--r--   0        0        0     4262 2024-05-08 13:37:01.488995 dbt_score-0.1.0a0/tests/conftest.py
--rw-r--r--   0        0        0     1302 2024-05-08 13:37:01.488995 dbt_score-0.1.0a0/tests/formatters/test_human_readable_formatter.py
--rw-r--r--   0        0        0     2199 2024-05-08 13:37:01.488995 dbt_score-0.1.0a0/tests/resources/manifest.json
--rw-r--r--   0        0        0       18 2024-05-08 13:37:01.488995 dbt_score-0.1.0a0/tests/resources/manifest_empty.json
--rw-r--r--   0        0        0      169 2024-05-08 13:37:01.488995 dbt_score-0.1.0a0/tests/rules/example.py
--rw-r--r--   0        0        0       49 2024-05-08 13:37:01.488995 dbt_score-0.1.0a0/tests/rules/nested/__init__.py
--rw-r--r--   0        0        0      174 2024-05-08 13:37:01.488995 dbt_score-0.1.0a0/tests/rules/nested/example.py
--rw-r--r--   0        0        0     1015 2024-05-08 13:37:01.488995 dbt_score-0.1.0a0/tests/test_cli.py
--rw-r--r--   0        0        0     4252 2024-05-08 13:37:01.488995 dbt_score-0.1.0a0/tests/test_evaluation.py
--rw-r--r--   0        0        0      448 2024-05-08 13:37:01.488995 dbt_score-0.1.0a0/tests/test_lint.py
--rw-r--r--   0        0        0      707 2024-05-08 13:37:01.488995 dbt_score-0.1.0a0/tests/test_models.py
--rw-r--r--   0        0        0     1984 2024-05-08 13:37:01.488995 dbt_score-0.1.0a0/tests/test_rule.py
--rw-r--r--   0        0        0      797 2024-05-08 13:37:01.488995 dbt_score-0.1.0a0/tests/test_rule_registry.py
--rw-r--r--   0        0        0     4192 2024-05-08 13:37:01.488995 dbt_score-0.1.0a0/tests/test_scoring.py
--rw-r--r--   0        0        0     2206 1970-01-01 00:00:00.000000 dbt_score-0.1.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-05-10 12:35:55.752205 dbt_score-0.1.0b1/LICENSE.txt
+-rw-r--r--   0        0        0     1683 2024-05-10 12:35:55.752205 dbt_score-0.1.0b1/README.md
+-rw-r--r--   0        0        0     1711 2024-05-10 12:36:10.908123 dbt_score-0.1.0b1/pyproject.toml
+-rw-r--r--   0        0        0      195 2024-05-10 12:35:55.756204 dbt_score-0.1.0b1/src/dbt_score/__init__.py
+-rwxr-xr-x   0        0        0      546 2024-05-10 12:35:55.756204 dbt_score-0.1.0b1/src/dbt_score/__main__.py
+-rw-r--r--   0        0        0     1677 2024-05-10 12:35:55.756204 dbt_score-0.1.0b1/src/dbt_score/cli.py
+-rw-r--r--   0        0        0     2673 2024-05-10 12:35:55.756204 dbt_score-0.1.0b1/src/dbt_score/evaluation.py
+-rw-r--r--   0        0        0      318 2024-05-10 12:35:55.756204 dbt_score-0.1.0b1/src/dbt_score/exceptions.py
+-rw-r--r--   0        0        0      710 2024-05-10 12:35:55.756204 dbt_score-0.1.0b1/src/dbt_score/formatters/__init__.py
+-rw-r--r--   0        0        0     1541 2024-05-10 12:35:55.756204 dbt_score-0.1.0b1/src/dbt_score/formatters/human_readable_formatter.py
+-rw-r--r--   0        0        0      881 2024-05-10 12:35:55.756204 dbt_score-0.1.0b1/src/dbt_score/lint.py
+-rw-r--r--   0        0        0     9041 2024-05-10 12:35:55.756204 dbt_score-0.1.0b1/src/dbt_score/models.py
+-rw-r--r--   0        0        0      932 2024-05-10 12:35:55.756204 dbt_score-0.1.0b1/src/dbt_score/parse.py
+-rw-r--r--   0        0        0     3606 2024-05-10 12:35:55.756204 dbt_score-0.1.0b1/src/dbt_score/rule.py
+-rw-r--r--   0        0        0     2068 2024-05-10 12:35:55.756204 dbt_score-0.1.0b1/src/dbt_score/rule_registry.py
+-rw-r--r--   0        0        0       13 2024-05-10 12:35:55.756204 dbt_score-0.1.0b1/src/dbt_score/rules/__init__.py
+-rw-r--r--   0        0        0      714 2024-05-10 12:35:55.756204 dbt_score-0.1.0b1/src/dbt_score/rules/generic.py
+-rw-r--r--   0        0        0     1981 2024-05-10 12:35:55.756204 dbt_score-0.1.0b1/src/dbt_score/scoring.py
+-rw-r--r--   0        0        0       30 2024-05-10 12:35:55.756204 dbt_score-0.1.0b1/tests/__init__.py
+-rw-r--r--   0        0        0     4262 2024-05-10 12:35:55.756204 dbt_score-0.1.0b1/tests/conftest.py
+-rw-r--r--   0        0        0     1302 2024-05-10 12:35:55.756204 dbt_score-0.1.0b1/tests/formatters/test_human_readable_formatter.py
+-rw-r--r--   0        0        0     2199 2024-05-10 12:35:55.756204 dbt_score-0.1.0b1/tests/resources/manifest.json
+-rw-r--r--   0        0        0       18 2024-05-10 12:35:55.756204 dbt_score-0.1.0b1/tests/resources/manifest_empty.json
+-rw-r--r--   0        0        0      169 2024-05-10 12:35:55.756204 dbt_score-0.1.0b1/tests/rules/example.py
+-rw-r--r--   0        0        0       49 2024-05-10 12:35:55.756204 dbt_score-0.1.0b1/tests/rules/nested/__init__.py
+-rw-r--r--   0        0        0      174 2024-05-10 12:35:55.756204 dbt_score-0.1.0b1/tests/rules/nested/example.py
+-rw-r--r--   0        0        0     1015 2024-05-10 12:35:55.756204 dbt_score-0.1.0b1/tests/test_cli.py
+-rw-r--r--   0        0        0     4252 2024-05-10 12:35:55.756204 dbt_score-0.1.0b1/tests/test_evaluation.py
+-rw-r--r--   0        0        0      448 2024-05-10 12:35:55.756204 dbt_score-0.1.0b1/tests/test_lint.py
+-rw-r--r--   0        0        0      707 2024-05-10 12:35:55.756204 dbt_score-0.1.0b1/tests/test_models.py
+-rw-r--r--   0        0        0     1984 2024-05-10 12:35:55.756204 dbt_score-0.1.0b1/tests/test_rule.py
+-rw-r--r--   0        0        0      797 2024-05-10 12:35:55.756204 dbt_score-0.1.0b1/tests/test_rule_registry.py
+-rw-r--r--   0        0        0     4192 2024-05-10 12:35:55.756204 dbt_score-0.1.0b1/tests/test_scoring.py
+-rw-r--r--   0        0        0     2206 1970-01-01 00:00:00.000000 dbt_score-0.1.0b1/PKG-INFO
```

### Comparing `dbt_score-0.1.0a0/LICENSE.txt` & `dbt_score-0.1.0b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dbt_score-0.1.0a0/README.md` & `dbt_score-0.1.0b1/README.md`

 * *Files identical despite different names*

### Comparing `dbt_score-0.1.0a0/pyproject.toml` & `dbt_score-0.1.0b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ]
 dependencies = [
     "dbt-core>=1.5",
     "click>=7.1.1, <9.0.0",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
-version = "0.1.0a0"
+version = "0.1.0b1"
 
 [[project.authors]]
 name = "Picnic Analyst Development Platform"
 email = "analyst-development-platform@teampicnic.com"
 
 [project.license]
 text = "MIT"
```

### Comparing `dbt_score-0.1.0a0/src/dbt_score/__main__.py` & `dbt_score-0.1.0b1/src/dbt_score/__main__.py`

 * *Files identical despite different names*

### Comparing `dbt_score-0.1.0a0/src/dbt_score/cli.py` & `dbt_score-0.1.0b1/src/dbt_score/cli.py`

 * *Files identical despite different names*

### Comparing `dbt_score-0.1.0a0/src/dbt_score/evaluation.py` & `dbt_score-0.1.0b1/src/dbt_score/evaluation.py`

 * *Files identical despite different names*

### Comparing `dbt_score-0.1.0a0/src/dbt_score/formatters/__init__.py` & `dbt_score-0.1.0b1/src/dbt_score/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_score-0.1.0a0/src/dbt_score/formatters/human_readable_formatter.py` & `dbt_score-0.1.0b1/src/dbt_score/formatters/human_readable_formatter.py`

 * *Files identical despite different names*

### Comparing `dbt_score-0.1.0a0/src/dbt_score/lint.py` & `dbt_score-0.1.0b1/src/dbt_score/lint.py`

 * *Files identical despite different names*

### Comparing `dbt_score-0.1.0a0/src/dbt_score/models.py` & `dbt_score-0.1.0b1/src/dbt_score/models.py`

 * *Files identical despite different names*

### Comparing `dbt_score-0.1.0a0/src/dbt_score/parse.py` & `dbt_score-0.1.0b1/src/dbt_score/parse.py`

 * *Files identical despite different names*

### Comparing `dbt_score-0.1.0a0/src/dbt_score/rule.py` & `dbt_score-0.1.0b1/src/dbt_score/rule.py`

 * *Files identical despite different names*

### Comparing `dbt_score-0.1.0a0/src/dbt_score/rule_registry.py` & `dbt_score-0.1.0b1/src/dbt_score/rule_registry.py`

 * *Files identical despite different names*

### Comparing `dbt_score-0.1.0a0/src/dbt_score/rules/generic.py` & `dbt_score-0.1.0b1/src/dbt_score/rules/generic.py`

 * *Files identical despite different names*

### Comparing `dbt_score-0.1.0a0/src/dbt_score/scoring.py` & `dbt_score-0.1.0b1/src/dbt_score/scoring.py`

 * *Files identical despite different names*

### Comparing `dbt_score-0.1.0a0/tests/conftest.py` & `dbt_score-0.1.0b1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dbt_score-0.1.0a0/tests/formatters/test_human_readable_formatter.py` & `dbt_score-0.1.0b1/tests/formatters/test_human_readable_formatter.py`

 * *Files identical despite different names*

### Comparing `dbt_score-0.1.0a0/tests/resources/manifest.json` & `dbt_score-0.1.0b1/tests/resources/manifest.json`

 * *Files identical despite different names*

### Comparing `dbt_score-0.1.0a0/tests/test_cli.py` & `dbt_score-0.1.0b1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `dbt_score-0.1.0a0/tests/test_evaluation.py` & `dbt_score-0.1.0b1/tests/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `dbt_score-0.1.0a0/tests/test_models.py` & `dbt_score-0.1.0b1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `dbt_score-0.1.0a0/tests/test_rule.py` & `dbt_score-0.1.0b1/tests/test_rule.py`

 * *Files identical despite different names*

### Comparing `dbt_score-0.1.0a0/tests/test_rule_registry.py` & `dbt_score-0.1.0b1/tests/test_rule_registry.py`

 * *Files identical despite different names*

### Comparing `dbt_score-0.1.0a0/tests/test_scoring.py` & `dbt_score-0.1.0b1/tests/test_scoring.py`

 * *Files identical despite different names*

### Comparing `dbt_score-0.1.0a0/PKG-INFO` & `dbt_score-0.1.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-score
-Version: 0.1.0a0
+Version: 0.1.0b1
 Summary: Linter for dbt model metadata.
 Author-Email: Picnic Analyst Development Platform <analyst-development-platform@teampicnic.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

