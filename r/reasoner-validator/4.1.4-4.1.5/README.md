# Comparing `tmp/reasoner_validator-4.1.4.tar.gz` & `tmp/reasoner_validator-4.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner_validator-4.1.4.tar", max compression
+gzip compressed data, was "reasoner_validator-4.1.5.tar", max compression
```

## Comparing `reasoner_validator-4.1.4.tar` & `reasoner_validator-4.1.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1153 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/LICENSE
--rw-r--r--   0        0        0    13727 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/README.md
--rw-r--r--   0        0        0      131 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/docs/.nojekyll
--rw-r--r--   0        0        0      634 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/docs/Makefile
--rw-r--r--   0        0        0     2291 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/docs/conf.py
--rw-r--r--   0        0        0    20564 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/docs/index.rst
--rw-r--r--   0        0        0      795 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/docs/make.bat
--rw-r--r--   0        0        0      136 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/docs/reasoner_validator.biolink.rst
--rw-r--r--   0        0        0      135 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/docs/reasoner_validator.report.rst
--rw-r--r--   0        0        0      152 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/docs/reasoner_validator.rst
--rw-r--r--   0        0        0      146 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/docs/reasoner_validator.trapi.mapping.rst
--rw-r--r--   0        0        0      144 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/docs/reasoner_validator.trapi.rst
--rw-r--r--   0        0        0      163 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/docs/reasoner_validator.validation_codes.rst
--rw-r--r--   0        0        0      157 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/docs/reasoner_validator.versioning.rst
--rw-r--r--   0        0        0    43141 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/docs/validation_codes_dictionary.md
--rw-r--r--   0        0        0     2298 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/reasoner_validator/__init__.py
--rw-r--r--   0        0        0    94673 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/reasoner_validator/biolink/__init__.py
--rw-r--r--   0        0        0    47008 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/reasoner_validator/codes.yaml
--rw-r--r--   0        0        0     1761 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/reasoner_validator/github.py
--rw-r--r--   0        0        0     3973 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/reasoner_validator/message.py
--rw-r--r--   0        0        0    46754 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/reasoner_validator/report.py
--rw-r--r--   0        0        0        0 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/reasoner_validator/sri/__init__.py
--rw-r--r--   0        0        0     4754 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/reasoner_validator/sri/util.py
--rw-r--r--   0        0        0    15057 2024-05-10 01:21:27.783950 reasoner_validator-4.1.4/reasoner_validator/trapi/__init__.py
--rw-r--r--   0        0        0     1120 2024-05-10 01:21:27.783950 reasoner_validator-4.1.4/reasoner_validator/trapi/mapping.py
--rw-r--r--   0        0        0    14745 2024-05-10 01:21:27.783950 reasoner_validator-4.1.4/reasoner_validator/validation_codes.py
--rw-r--r--   0        0        0    38176 2024-05-10 01:21:27.783950 reasoner_validator-4.1.4/reasoner_validator/validator.py
--rw-r--r--   0        0        0    12127 2024-05-10 01:21:27.783950 reasoner_validator-4.1.4/reasoner_validator/versioning.py
--rw-r--r--   0        0        0      866 2024-05-10 01:21:27.783950 reasoner_validator-4.1.4/reasoner_validator/versions.yaml
--rw-r--r--   0        0        0     3601 2024-05-10 01:21:27.783950 reasoner_validator-4.1.4/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-05-10 01:21:27.783950 reasoner_validator-4.1.4/tests/conftest.py
--rw-r--r--   0        0        0   149129 2024-05-10 01:21:27.783950 reasoner_validator-4.1.4/tests/test_biolink_compliance_validation.py
--rw-r--r--   0        0        0    62107 2024-05-10 01:21:27.783950 reasoner_validator-4.1.4/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
--rw-r--r--   0        0        0    49059 2024-05-10 01:21:27.783950 reasoner_validator-4.1.4/tests/test_response_validator.py
--rw-r--r--   0        0        0     6157 2024-05-10 01:21:27.783950 reasoner_validator-4.1.4/tests/test_semver.py
--rw-r--r--   0        0        0     2351 2024-05-10 01:21:27.783950 reasoner_validator-4.1.4/tests/test_trapi_versioning.py
--rw-r--r--   0        0        0    36764 2024-05-10 01:21:27.783950 reasoner_validator-4.1.4/tests/test_validate.py
--rw-r--r--   0        0        0    30239 2024-05-10 01:21:27.783950 reasoner_validator-4.1.4/tests/test_validation_report.py
--rw-r--r--   0        0        0     3421 2024-05-10 01:21:27.783950 reasoner_validator-4.1.4/tests/test_workflows.py
--rw-r--r--   0        0        0    15315 1970-01-01 00:00:00.000000 reasoner_validator-4.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1153 2024-05-10 05:48:23.477226 reasoner_validator-4.1.5/LICENSE
+-rw-r--r--   0        0        0    13727 2024-05-10 05:48:23.477226 reasoner_validator-4.1.5/README.md
+-rw-r--r--   0        0        0      131 2024-05-10 05:48:23.477226 reasoner_validator-4.1.5/docs/.nojekyll
+-rw-r--r--   0        0        0      634 2024-05-10 05:48:23.477226 reasoner_validator-4.1.5/docs/Makefile
+-rw-r--r--   0        0        0     2291 2024-05-10 05:48:23.477226 reasoner_validator-4.1.5/docs/conf.py
+-rw-r--r--   0        0        0    20564 2024-05-10 05:48:23.477226 reasoner_validator-4.1.5/docs/index.rst
+-rw-r--r--   0        0        0      795 2024-05-10 05:48:23.477226 reasoner_validator-4.1.5/docs/make.bat
+-rw-r--r--   0        0        0      136 2024-05-10 05:48:23.477226 reasoner_validator-4.1.5/docs/reasoner_validator.biolink.rst
+-rw-r--r--   0        0        0      135 2024-05-10 05:48:23.477226 reasoner_validator-4.1.5/docs/reasoner_validator.report.rst
+-rw-r--r--   0        0        0      152 2024-05-10 05:48:23.477226 reasoner_validator-4.1.5/docs/reasoner_validator.rst
+-rw-r--r--   0        0        0      146 2024-05-10 05:48:23.477226 reasoner_validator-4.1.5/docs/reasoner_validator.trapi.mapping.rst
+-rw-r--r--   0        0        0      144 2024-05-10 05:48:23.477226 reasoner_validator-4.1.5/docs/reasoner_validator.trapi.rst
+-rw-r--r--   0        0        0      163 2024-05-10 05:48:23.477226 reasoner_validator-4.1.5/docs/reasoner_validator.validation_codes.rst
+-rw-r--r--   0        0        0      157 2024-05-10 05:48:23.477226 reasoner_validator-4.1.5/docs/reasoner_validator.versioning.rst
+-rw-r--r--   0        0        0    43141 2024-05-10 05:48:23.477226 reasoner_validator-4.1.5/docs/validation_codes_dictionary.md
+-rw-r--r--   0        0        0     2298 2024-05-10 05:48:23.481226 reasoner_validator-4.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-10 05:48:23.481226 reasoner_validator-4.1.5/reasoner_validator/__init__.py
+-rw-r--r--   0        0        0    94743 2024-05-10 05:48:23.481226 reasoner_validator-4.1.5/reasoner_validator/biolink/__init__.py
+-rw-r--r--   0        0        0    47008 2024-05-10 05:48:23.481226 reasoner_validator-4.1.5/reasoner_validator/codes.yaml
+-rw-r--r--   0        0        0     1761 2024-05-10 05:48:23.481226 reasoner_validator-4.1.5/reasoner_validator/github.py
+-rw-r--r--   0        0        0     3973 2024-05-10 05:48:23.481226 reasoner_validator-4.1.5/reasoner_validator/message.py
+-rw-r--r--   0        0        0    46754 2024-05-10 05:48:23.481226 reasoner_validator-4.1.5/reasoner_validator/report.py
+-rw-r--r--   0        0        0        0 2024-05-10 05:48:23.481226 reasoner_validator-4.1.5/reasoner_validator/sri/__init__.py
+-rw-r--r--   0        0        0     4754 2024-05-10 05:48:23.481226 reasoner_validator-4.1.5/reasoner_validator/sri/util.py
+-rw-r--r--   0        0        0    15057 2024-05-10 05:48:23.481226 reasoner_validator-4.1.5/reasoner_validator/trapi/__init__.py
+-rw-r--r--   0        0        0     1120 2024-05-10 05:48:23.481226 reasoner_validator-4.1.5/reasoner_validator/trapi/mapping.py
+-rw-r--r--   0        0        0    14745 2024-05-10 05:48:23.481226 reasoner_validator-4.1.5/reasoner_validator/validation_codes.py
+-rw-r--r--   0        0        0    38176 2024-05-10 05:48:23.481226 reasoner_validator-4.1.5/reasoner_validator/validator.py
+-rw-r--r--   0        0        0    12127 2024-05-10 05:48:23.481226 reasoner_validator-4.1.5/reasoner_validator/versioning.py
+-rw-r--r--   0        0        0      866 2024-05-10 05:48:23.481226 reasoner_validator-4.1.5/reasoner_validator/versions.yaml
+-rw-r--r--   0        0        0     3601 2024-05-10 05:48:23.481226 reasoner_validator-4.1.5/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 05:48:23.481226 reasoner_validator-4.1.5/tests/conftest.py
+-rw-r--r--   0        0        0   149401 2024-05-10 05:48:23.481226 reasoner_validator-4.1.5/tests/test_biolink_compliance_validation.py
+-rw-r--r--   0        0        0    62107 2024-05-10 05:48:23.481226 reasoner_validator-4.1.5/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
+-rw-r--r--   0        0        0    49059 2024-05-10 05:48:23.485226 reasoner_validator-4.1.5/tests/test_response_validator.py
+-rw-r--r--   0        0        0     6157 2024-05-10 05:48:23.485226 reasoner_validator-4.1.5/tests/test_semver.py
+-rw-r--r--   0        0        0     2351 2024-05-10 05:48:23.485226 reasoner_validator-4.1.5/tests/test_trapi_versioning.py
+-rw-r--r--   0        0        0    36764 2024-05-10 05:48:23.485226 reasoner_validator-4.1.5/tests/test_validate.py
+-rw-r--r--   0        0        0    30239 2024-05-10 05:48:23.485226 reasoner_validator-4.1.5/tests/test_validation_report.py
+-rw-r--r--   0        0        0     3421 2024-05-10 05:48:23.485226 reasoner_validator-4.1.5/tests/test_workflows.py
+-rw-r--r--   0        0        0    15315 1970-01-01 00:00:00.000000 reasoner_validator-4.1.5/PKG-INFO
```

### Comparing `reasoner_validator-4.1.4/LICENSE` & `reasoner_validator-4.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.4/README.md` & `reasoner_validator-4.1.5/README.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.4/docs/Makefile` & `reasoner_validator-4.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.4/docs/conf.py` & `reasoner_validator-4.1.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.4/docs/index.rst` & `reasoner_validator-4.1.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.4/docs/make.bat` & `reasoner_validator-4.1.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.4/docs/validation_codes_dictionary.md` & `reasoner_validator-4.1.5/docs/validation_codes_dictionary.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.4/pyproject.toml` & `reasoner_validator-4.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reasoner-validator"
-version = "4.1.4"
+version = "4.1.5"
 description = "Validation tools for Reasoner API"
 authors = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
     "Patrick Wang <patrickelvin@gmail.com>"
 ]
 maintainers = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
```

### Comparing `reasoner_validator-4.1.4/reasoner_validator/biolink/__init__.py` & `reasoner_validator-4.1.5/reasoner_validator/biolink/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1390,36 +1390,37 @@
             self,
             edge_id: str,
             predicate: str,
             graph_type: TRAPIGraphType,
             source_trail: Optional[str] = None
     ):
         """
-        Validates predicates based on their meta-nature: existence, mixin, deprecation, etc.
-        with notable hard-coded explicit PREDICATE_INCLUSIONS exceptions.
+        Validates predicates based on their meta-nature: existence, mixin,
+        deprecation, etc. with some notable hard-coded explicit
+        PREDICATE_INCLUSIONS exceptions in earlier Biolink Model releases.
 
         :param edge_id: str, identifier of the edge whose predicate is being validated
         :param predicate: str, putative Biolink Model predicate to be validated
         :param source_trail: str, putative Biolink Model predicate to be validated
         :param graph_type: TRAPIGraphType, type of TRAPI graph component being validated
         :return: None (validation communicated via class instance of method)
         """
-        # PREDICATE_INCLUSIONS provides for selective
-        # override of validation of particular predicates
-        if self.minimum_required_biolink_version("4.2.0") or \
+        # PREDICATE_INCLUSIONS provides for selective override of
+        # validation of particular predicates prior to Biolink 4.2.1
+        if self.minimum_required_biolink_version("4.2.1") or \
                 predicate not in self.PREDICATE_INCLUSIONS:
 
             graph_type_context: str = graph_type.name.lower()
             if graph_type_context != "input_edge":
                 graph_type_context += ".edge"
             context: str = f"{graph_type_context}.predicate"
 
             # Validate the putative predicate as
             # *not* being abstract, deprecated or
-            # a mixin (for Biolink Model release >= 4.2.0?)
+            # a mixin (for Biolink Model release >= 4.2.1?)
             biolink_class = self.validate_element_status(
                 graph_type=graph_type,
                 context=context,
                 identifier=predicate,
                 edge_id=edge_id,
                 source_trail=source_trail
             )
```

### Comparing `reasoner_validator-4.1.4/reasoner_validator/codes.yaml` & `reasoner_validator-4.1.5/reasoner_validator/codes.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.4/reasoner_validator/github.py` & `reasoner_validator-4.1.5/reasoner_validator/github.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.4/reasoner_validator/message.py` & `reasoner_validator-4.1.5/reasoner_validator/message.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.4/reasoner_validator/report.py` & `reasoner_validator-4.1.5/reasoner_validator/report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.4/reasoner_validator/sri/util.py` & `reasoner_validator-4.1.5/reasoner_validator/sri/util.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.4/reasoner_validator/trapi/__init__.py` & `reasoner_validator-4.1.5/reasoner_validator/trapi/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.4/reasoner_validator/trapi/mapping.py` & `reasoner_validator-4.1.5/reasoner_validator/trapi/mapping.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.4/reasoner_validator/validation_codes.py` & `reasoner_validator-4.1.5/reasoner_validator/validation_codes.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.4/reasoner_validator/validator.py` & `reasoner_validator-4.1.5/reasoner_validator/validator.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.4/reasoner_validator/versioning.py` & `reasoner_validator-4.1.5/reasoner_validator/versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.4/reasoner_validator/versions.yaml` & `reasoner_validator-4.1.5/reasoner_validator/versions.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.4/tests/__init__.py` & `reasoner_validator-4.1.5/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.4/tests/test_biolink_compliance_validation.py` & `reasoner_validator-4.1.5/tests/test_biolink_compliance_validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,15 +237,16 @@
                 'subject_category': 'biolink:Drug',
                 'object_category': 'biolink:BiologicalProcess',
                 'predicate': 'biolink:treats',
                 'subject_id': 'NDC:50090‑0766',  # Metformin
                 'object_id': 'GO:0006094'  # Gluconeogenesis
             },
             # f"{INPUT_EDGE_PREFIX}: INFO - Predicate element 'biolink:treats' is a mixin."
-            "info.input_edge.predicate.mixin"
+            # "info.input_edge.predicate.mixin"
+            ""  # mixin predicate patch < BM 4.2.1 skips validation of biolink:treats
         ),
         (   # Query 11 - Unknown predicate element
             LATEST_BIOLINK_MODEL_VERSION,
             {
                 'subject_category': 'biolink:AnatomicalEntity',
                 'object_category': 'biolink:AnatomicalEntity',
                 'predicate': 'biolink:not_a_predicate',
@@ -846,15 +847,16 @@
                     "treats": {
                         "subject": "drug",
                         "predicates": ["biolink:treats"],
                         "object": "type-2 diabetes"
                     }
                 }
             },
-            "info.query_graph.edge.predicate.mixin"
+            # "info.query_graph.edge.predicate.mixin"
+            ""  # mixin predicate patch < BM 4.2.1 skips validation of biolink:treats
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
             # Query 19: 'Subject' id used in edge is mandatory
             {
                 "nodes": {
                     "drug": {
@@ -3170,15 +3172,16 @@
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
                         ]
                     }
                 }
             },
-            "error.knowledge_graph.edge.predicate.mixin"
+            # "error.knowledge_graph.edge.predicate.mixin"
+            ""  # mixin predicate patch < BM 4.2.1 skips validation of biolink:interacts_with
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
             # Query 22: predicate is abstract - not allowed in Knowledge Graphs
             {
                 "nodes": {
                     "PMID:1234": {
```

### Comparing `reasoner_validator-4.1.4/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml` & `reasoner_validator-4.1.5/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.4/tests/test_response_validator.py` & `reasoner_validator-4.1.5/tests/test_response_validator.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.4/tests/test_semver.py` & `reasoner_validator-4.1.5/tests/test_semver.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.4/tests/test_trapi_versioning.py` & `reasoner_validator-4.1.5/tests/test_trapi_versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.4/tests/test_validate.py` & `reasoner_validator-4.1.5/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.4/tests/test_validation_report.py` & `reasoner_validator-4.1.5/tests/test_validation_report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.4/tests/test_workflows.py` & `reasoner_validator-4.1.5/tests/test_workflows.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.4/PKG-INFO` & `reasoner_validator-4.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-validator
-Version: 4.1.4
+Version: 4.1.5
 Summary: Validation tools for Reasoner API
 Home-page: https://github.com/NCATSTranslator
 License: MIT
 Keywords: NCATS,Biomedical Data Translator,Translator,ReasonerAPI,TRAPI,validation,Biolink Model
 Author: Richard Bruskiewich
 Author-email: richard.bruskiewich@delphinai.com
 Maintainer: Richard Bruskiewich
```

