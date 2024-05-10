# Comparing `tmp/reasoner_validator-4.1.3.tar.gz` & `tmp/reasoner_validator-4.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner_validator-4.1.3.tar", max compression
+gzip compressed data, was "reasoner_validator-4.1.4.tar", max compression
```

## Comparing `reasoner_validator-4.1.3.tar` & `reasoner_validator-4.1.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1153 2024-05-03 06:58:05.392860 reasoner_validator-4.1.3/LICENSE
--rw-r--r--   0        0        0    13727 2024-05-03 06:58:05.392860 reasoner_validator-4.1.3/README.md
--rw-r--r--   0        0        0      131 2024-05-03 06:58:05.392860 reasoner_validator-4.1.3/docs/.nojekyll
--rw-r--r--   0        0        0      634 2024-05-03 06:58:05.392860 reasoner_validator-4.1.3/docs/Makefile
--rw-r--r--   0        0        0     2291 2024-05-03 06:58:05.392860 reasoner_validator-4.1.3/docs/conf.py
--rw-r--r--   0        0        0    20564 2024-05-03 06:58:05.392860 reasoner_validator-4.1.3/docs/index.rst
--rw-r--r--   0        0        0      795 2024-05-03 06:58:05.392860 reasoner_validator-4.1.3/docs/make.bat
--rw-r--r--   0        0        0      136 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/docs/reasoner_validator.biolink.rst
--rw-r--r--   0        0        0      135 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/docs/reasoner_validator.report.rst
--rw-r--r--   0        0        0      152 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/docs/reasoner_validator.rst
--rw-r--r--   0        0        0      146 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/docs/reasoner_validator.trapi.mapping.rst
--rw-r--r--   0        0        0      144 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/docs/reasoner_validator.trapi.rst
--rw-r--r--   0        0        0      163 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/docs/reasoner_validator.validation_codes.rst
--rw-r--r--   0        0        0      157 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/docs/reasoner_validator.versioning.rst
--rw-r--r--   0        0        0    42104 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/docs/validation_codes_dictionary.md
--rw-r--r--   0        0        0     2298 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/reasoner_validator/__init__.py
--rw-r--r--   0        0        0    94451 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/reasoner_validator/biolink/__init__.py
--rw-r--r--   0        0        0    45890 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/reasoner_validator/codes.yaml
--rw-r--r--   0        0        0     1761 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/reasoner_validator/github.py
--rw-r--r--   0        0        0     3973 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/reasoner_validator/message.py
--rw-r--r--   0        0        0    46754 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/reasoner_validator/report.py
--rw-r--r--   0        0        0        0 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/reasoner_validator/sri/__init__.py
--rw-r--r--   0        0        0     4754 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/reasoner_validator/sri/util.py
--rw-r--r--   0        0        0    15057 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/reasoner_validator/trapi/__init__.py
--rw-r--r--   0        0        0     1120 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/reasoner_validator/trapi/mapping.py
--rw-r--r--   0        0        0    14745 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/reasoner_validator/validation_codes.py
--rw-r--r--   0        0        0    35631 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/reasoner_validator/validator.py
--rw-r--r--   0        0        0    12127 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/reasoner_validator/versioning.py
--rw-r--r--   0        0        0      866 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/reasoner_validator/versions.yaml
--rw-r--r--   0        0        0     3601 2024-05-03 06:58:05.400860 reasoner_validator-4.1.3/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 06:58:05.400860 reasoner_validator-4.1.3/tests/conftest.py
--rw-r--r--   0        0        0   146649 2024-05-03 06:58:05.400860 reasoner_validator-4.1.3/tests/test_biolink_compliance_validation.py
--rw-r--r--   0        0        0    62107 2024-05-03 06:58:05.400860 reasoner_validator-4.1.3/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
--rw-r--r--   0        0        0    41831 2024-05-03 06:58:05.400860 reasoner_validator-4.1.3/tests/test_response_validator.py
--rw-r--r--   0        0        0     6157 2024-05-03 06:58:05.400860 reasoner_validator-4.1.3/tests/test_semver.py
--rw-r--r--   0        0        0     2248 2024-05-03 06:58:05.400860 reasoner_validator-4.1.3/tests/test_trapi_versioning.py
--rw-r--r--   0        0        0    36620 2024-05-03 06:58:05.400860 reasoner_validator-4.1.3/tests/test_validate.py
--rw-r--r--   0        0        0    30223 2024-05-03 06:58:05.400860 reasoner_validator-4.1.3/tests/test_validation_report.py
--rw-r--r--   0        0        0     3411 2024-05-03 06:58:05.400860 reasoner_validator-4.1.3/tests/test_workflows.py
--rw-r--r--   0        0        0    15315 1970-01-01 00:00:00.000000 reasoner_validator-4.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1153 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/LICENSE
+-rw-r--r--   0        0        0    13727 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/README.md
+-rw-r--r--   0        0        0      131 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/docs/.nojekyll
+-rw-r--r--   0        0        0      634 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/docs/Makefile
+-rw-r--r--   0        0        0     2291 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/docs/conf.py
+-rw-r--r--   0        0        0    20564 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/docs/index.rst
+-rw-r--r--   0        0        0      795 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/docs/make.bat
+-rw-r--r--   0        0        0      136 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/docs/reasoner_validator.biolink.rst
+-rw-r--r--   0        0        0      135 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/docs/reasoner_validator.report.rst
+-rw-r--r--   0        0        0      152 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/docs/reasoner_validator.rst
+-rw-r--r--   0        0        0      146 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/docs/reasoner_validator.trapi.mapping.rst
+-rw-r--r--   0        0        0      144 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/docs/reasoner_validator.trapi.rst
+-rw-r--r--   0        0        0      163 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/docs/reasoner_validator.validation_codes.rst
+-rw-r--r--   0        0        0      157 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/docs/reasoner_validator.versioning.rst
+-rw-r--r--   0        0        0    43141 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/docs/validation_codes_dictionary.md
+-rw-r--r--   0        0        0     2298 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/reasoner_validator/__init__.py
+-rw-r--r--   0        0        0    94673 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/reasoner_validator/biolink/__init__.py
+-rw-r--r--   0        0        0    47008 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/reasoner_validator/codes.yaml
+-rw-r--r--   0        0        0     1761 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/reasoner_validator/github.py
+-rw-r--r--   0        0        0     3973 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/reasoner_validator/message.py
+-rw-r--r--   0        0        0    46754 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/reasoner_validator/report.py
+-rw-r--r--   0        0        0        0 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/reasoner_validator/sri/__init__.py
+-rw-r--r--   0        0        0     4754 2024-05-10 01:21:27.779950 reasoner_validator-4.1.4/reasoner_validator/sri/util.py
+-rw-r--r--   0        0        0    15057 2024-05-10 01:21:27.783950 reasoner_validator-4.1.4/reasoner_validator/trapi/__init__.py
+-rw-r--r--   0        0        0     1120 2024-05-10 01:21:27.783950 reasoner_validator-4.1.4/reasoner_validator/trapi/mapping.py
+-rw-r--r--   0        0        0    14745 2024-05-10 01:21:27.783950 reasoner_validator-4.1.4/reasoner_validator/validation_codes.py
+-rw-r--r--   0        0        0    38176 2024-05-10 01:21:27.783950 reasoner_validator-4.1.4/reasoner_validator/validator.py
+-rw-r--r--   0        0        0    12127 2024-05-10 01:21:27.783950 reasoner_validator-4.1.4/reasoner_validator/versioning.py
+-rw-r--r--   0        0        0      866 2024-05-10 01:21:27.783950 reasoner_validator-4.1.4/reasoner_validator/versions.yaml
+-rw-r--r--   0        0        0     3601 2024-05-10 01:21:27.783950 reasoner_validator-4.1.4/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 01:21:27.783950 reasoner_validator-4.1.4/tests/conftest.py
+-rw-r--r--   0        0        0   149129 2024-05-10 01:21:27.783950 reasoner_validator-4.1.4/tests/test_biolink_compliance_validation.py
+-rw-r--r--   0        0        0    62107 2024-05-10 01:21:27.783950 reasoner_validator-4.1.4/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
+-rw-r--r--   0        0        0    49059 2024-05-10 01:21:27.783950 reasoner_validator-4.1.4/tests/test_response_validator.py
+-rw-r--r--   0        0        0     6157 2024-05-10 01:21:27.783950 reasoner_validator-4.1.4/tests/test_semver.py
+-rw-r--r--   0        0        0     2351 2024-05-10 01:21:27.783950 reasoner_validator-4.1.4/tests/test_trapi_versioning.py
+-rw-r--r--   0        0        0    36764 2024-05-10 01:21:27.783950 reasoner_validator-4.1.4/tests/test_validate.py
+-rw-r--r--   0        0        0    30239 2024-05-10 01:21:27.783950 reasoner_validator-4.1.4/tests/test_validation_report.py
+-rw-r--r--   0        0        0     3421 2024-05-10 01:21:27.783950 reasoner_validator-4.1.4/tests/test_workflows.py
+-rw-r--r--   0        0        0    15315 1970-01-01 00:00:00.000000 reasoner_validator-4.1.4/PKG-INFO
```

### Comparing `reasoner_validator-4.1.3/LICENSE` & `reasoner_validator-4.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.3/README.md` & `reasoner_validator-4.1.4/README.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.3/docs/Makefile` & `reasoner_validator-4.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.3/docs/conf.py` & `reasoner_validator-4.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.3/docs/index.rst` & `reasoner_validator-4.1.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.3/docs/make.bat` & `reasoner_validator-4.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.3/docs/validation_codes_dictionary.md` & `reasoner_validator-4.1.4/docs/validation_codes_dictionary.md`

 * *Files 4% similar despite different names*

```diff
@@ -44,59 +44,81 @@
 
 ### error.trapi.response.message.empty
 
 **Message:** TRAPI Response missing its Message!
 
 **Description:** TRAPI Response should at least have non-empty original TRAPI request Message in its reply.
 
-### error.trapi.response.query_graph.missing
+### error.trapi.response.message.query_graph.missing
 
 **Message:** TRAPI Message is missing its Query Graph!
 
 **Description:** TRAPI Response should generally have a TRAPI request message Query Graph key value in its reply.
 
-### error.trapi.response.query_graph.empty
+### error.trapi.response.message.query_graph.empty
 
 **Message:** Response returned an empty Message Query Graph!
 
 **Description:** TRAPI Response should at least have original non-empty TRAPI request message Query Graph in its reply.
 
-### error.trapi.response.knowledge_graph.missing
+### error.trapi.response.message.knowledge_graph.missing
 
 **Message:** TRAPI Message is missing its Knowledge Graph component!
 
 **Description:** TRAPI Response should generally have a TRAPI request message Knowledge Graph key value in its reply.
 
-### error.trapi.response.knowledge_graph.missing_expected_edge
+### error.trapi.response.message.knowledge_graph.empty
 
-**Message:** Knowledge Graph of TRAPI Response Message is missing expected Edge
+**Message:** Response returned an empty Message Knowledge Graph, which is an error in this context!
+
+**Description:** An empty Knowledge Graph is considered an error in this validation context!
+
+### error.trapi.response.message.knowledge_graph.node.missing
+
+**Message:** Knowledge Graph of TRAPI Response Message Knowledge Graph is missing an expected Node
 
 **Context:** identifier
 
-**Description:** The given TRAPI Response is expected to return specific edge(s) relating to the original (test edge?) data used to prepare the TRAPI Request!
+**Description:** The given TRAPI Response is expected to return specific node(s) related to the original input data used to prepare the TRAPI Request!
 
-### error.trapi.response.knowledge_graph.empty
+### error.trapi.response.message.knowledge_graph.edge.missing
 
-**Message:** Response returned an empty Message Knowledge Graph, which is an error in this context!
+**Message:** Knowledge Graph of TRAPI Response Message Knowledge Graph is missing expected Edge
 
-**Description:** An empty Knowledge Graph is considered an error in this validation context!
+**Context:** identifier
+
+**Description:** The given TRAPI Response is expected to return specific edge(s) related to the original input data used to prepare the TRAPI Request!
 
-### error.trapi.response.results.missing
+### error.trapi.response.message.result.missing
+
+**Message:** TRAPI Response Message is missing expected knowledge graph edge mapping in its Results
+
+**Context:** identifier
+
+**Description:** The given TRAPI Response is expected to return a specified edge - in its list of Results - relating to the original input data used to prepare the TRAPI Request!
+
+### error.trapi.response.message.results.missing
 
 **Message:** TRAPI Message is missing its Results component!
 
-**Description:** TRAPI Response should generally have a TRAPI request message Request key value in its reply.
+**Description:** In this context, the TRAPI Response should generally have a non-empty TRAPI Response Message Results component.
+
+### error.trapi.response.message.results.empty
+
+**Message:** Response returned an empty Message Results, which is an error in this context!
+
+**Description:** An empty block of Results is considered an error in the specific validation context!
 
-### error.trapi.response.results.not_array
+### error.trapi.response.message.results.not_array
 
 **Message:** Response returned a non-array Message.Results!
 
 **Description:** TRAPI Message.Results must be an array data type (even if empty)
 
-### error.trapi.response.results.missing_bindings
+### error.trapi.response.message.results.missing_bindings
 
 **Message:** Result object IDs for output node binding did not return the original identifier nor aliases for input id
 
 **Context:** identifier, output_node_binding
 
 **Description:** TRAPI Message.Results cannot resolve its reported identifier mappings to the original query.
 
@@ -870,21 +892,21 @@
 
 ### warning.trapi.response.biolink_version.missing
 
 **Message:** TRAPI Response is missing its Biolink Model version
 
 **Description:** The TRAPI Response should specify its Biolink Model version compliance.
 
-### warning.trapi.response.knowledge_graph.empty
+### warning.trapi.response.message.knowledge_graph.empty
 
 **Message:** Response returned an empty Message Knowledge Graph?
 
 **Description:** An empty Knowledge Graph is allowed but merits a boundary response warning?
 
-### warning.trapi.response.results.empty
+### warning.trapi.response.message.results.empty
 
 **Message:** Response returned empty Message.results?
 
 **Description:** Empty Results is allowed but merits a boundary response warning?
 
 ### warning.trapi.response.workflow.runner_parameters.missing
```

### Comparing `reasoner_validator-4.1.3/pyproject.toml` & `reasoner_validator-4.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reasoner-validator"
-version = "4.1.3"
+version = "4.1.4"
 description = "Validation tools for Reasoner API"
 authors = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
     "Patrick Wang <patrickelvin@gmail.com>"
 ]
 maintainers = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
```

### Comparing `reasoner_validator-4.1.3/reasoner_validator/biolink/__init__.py` & `reasoner_validator-4.1.4/reasoner_validator/biolink/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -493,14 +493,16 @@
                     source_trail=source_trail,
                     identifier=identifier,
                     edge_id=edge_id
                 )
 
         elif self.bmt.is_mixin(identifier):
             # A mixin cannot be instantiated ...
+            # but can be used in QueryGraphs
+            # or when explicitly permitted
             if self.is_strict_validation(graph_type):
                 self.report(
                     code=f"error.{context}.mixin",
                     source_trail=source_trail,
                     identifier=identifier,
                     edge_id=edge_id
                 )
@@ -1399,22 +1401,25 @@
         :param predicate: str, putative Biolink Model predicate to be validated
         :param source_trail: str, putative Biolink Model predicate to be validated
         :param graph_type: TRAPIGraphType, type of TRAPI graph component being validated
         :return: None (validation communicated via class instance of method)
         """
         # PREDICATE_INCLUSIONS provides for selective
         # override of validation of particular predicates
-        if predicate not in self.PREDICATE_INCLUSIONS:
+        if self.minimum_required_biolink_version("4.2.0") or \
+                predicate not in self.PREDICATE_INCLUSIONS:
 
             graph_type_context: str = graph_type.name.lower()
             if graph_type_context != "input_edge":
                 graph_type_context += ".edge"
             context: str = f"{graph_type_context}.predicate"
 
-            # Validate the putative predicate as *not* being abstract, deprecated or a mixin
+            # Validate the putative predicate as
+            # *not* being abstract, deprecated or
+            # a mixin (for Biolink Model release >= 4.2.0?)
             biolink_class = self.validate_element_status(
                 graph_type=graph_type,
                 context=context,
                 identifier=predicate,
                 edge_id=edge_id,
                 source_trail=source_trail
             )
```

### Comparing `reasoner_validator-4.1.3/reasoner_validator/codes.yaml` & `reasoner_validator-4.1.4/reasoner_validator/codes.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -45,46 +45,62 @@
       empty:
         $message: "TRAPI Response is missing!"
         $description: "TRAPI Response to be validated should not be totally empty but should have a Message body."
       message:
         empty:
           $message: "TRAPI Response missing its Message!"
           $description: "TRAPI Response should at least have non-empty original TRAPI request Message in its reply."
-      query_graph:
-        missing:
-          $message: "TRAPI Message is missing its Query Graph!"
-          $description: "TRAPI Response should generally have a TRAPI request message Query Graph key value in its reply."
-        empty:
-          $message: "Response returned an empty Message Query Graph!"
-          $description: "TRAPI Response should at least have original non-empty TRAPI request message Query Graph in its reply."
-      knowledge_graph:
-        missing:
-          $message: "TRAPI Message is missing its Knowledge Graph component!"
-          $description: "TRAPI Response should generally have a TRAPI request message Knowledge Graph key value in its reply."
-        missing_expected_edge:
-          $message: "Knowledge Graph of TRAPI Response Message is missing expected Edge"
-          $context:
-            - identifier
-          $description: "The given TRAPI Response is expected to return specific edge(s) relating to the original (test edge?) data used to prepare the TRAPI Request!"
-        empty:
-          $message: "Response returned an empty Message Knowledge Graph, which is an error in this context!"
-          $description: "An empty Knowledge Graph is considered an error in this validation context!"
-      results:
-        missing:
-          $message: "TRAPI Message is missing its Results component!"
-          $description: "TRAPI Response should generally have a TRAPI request message Request key value in its reply."
-        not_array:
-          $message: "Response returned a non-array Message.Results!"
-          $description: "TRAPI Message.Results must be an array data type (even if empty)"
-        missing_bindings:
-          $message: "Result object IDs for output node binding did not return the original identifier nor aliases for input id"
-          $context:
-            - identifier
-            - output_node_binding
-          $description: "TRAPI Message.Results cannot resolve its reported identifier mappings to the original query."
+        query_graph:
+          missing:
+            $message: "TRAPI Message is missing its Query Graph!"
+            $description: "TRAPI Response should generally have a TRAPI request message Query Graph key value in its reply."
+          empty:
+            $message: "Response returned an empty Message Query Graph!"
+            $description: "TRAPI Response should at least have original non-empty TRAPI request message Query Graph in its reply."
+        knowledge_graph:
+          missing:
+            $message: "TRAPI Message is missing its Knowledge Graph component!"
+            $description: "TRAPI Response should generally have a TRAPI request message Knowledge Graph key value in its reply."
+          empty:
+            $message: "Response returned an empty Message Knowledge Graph, which is an error in this context!"
+            $description: "An empty Knowledge Graph is considered an error in this validation context!"
+          node:
+            missing:
+              $message: "Knowledge Graph of TRAPI Response Message Knowledge Graph is missing an expected Node"
+              $context:
+                - identifier
+              $description: "The given TRAPI Response is expected to return specific node(s) related to the original input data used to prepare the TRAPI Request!"
+          edge:
+            missing:
+              $message: "Knowledge Graph of TRAPI Response Message Knowledge Graph is missing expected Edge"
+              $context:
+                - identifier
+              $description: "The given TRAPI Response is expected to return specific edge(s) related to the original input data used to prepare the TRAPI Request!"
+        result:
+          missing:
+            $message: "TRAPI Response Message is missing expected knowledge graph edge mapping in its Results"
+            $context:
+              - identifier
+            $description: "The given TRAPI Response is expected to return a specified edge - in its list of Results - relating to the original input data used to prepare the TRAPI Request!"
+        results:
+          missing:
+            $message: "TRAPI Message is missing its Results component!"
+            $description: "In this context, the TRAPI Response should generally have a non-empty TRAPI Response Message Results component."
+          empty:
+            $message: "Response returned an empty Message Results, which is an error in this context!"
+            $description: "An empty block of Results is considered an error in the specific validation context!"
+          not_array:
+            $message: "Response returned a non-array Message.Results!"
+            $description: "TRAPI Message.Results must be an array data type (even if empty)"
+          missing_bindings:
+            $message: "Result object IDs for output node binding did not return the original identifier nor aliases for input id"
+            $context:
+              - identifier
+              - output_node_binding
+            $description: "TRAPI Message.Results cannot resolve its reported identifier mappings to the original query."
   input_edge:
     node:
       category:
         missing:
           $message: "Category missing for node"
           $context:
             - identifier
@@ -669,22 +685,23 @@
         missing:
           $message: "TRAPI Response is missing its TRAPI schema version"
           $description:  "The TRAPI Response should specify its TRAPI version compliance."
       biolink_version:
         missing:
           $message: "TRAPI Response is missing its Biolink Model version"
           $description:  "The TRAPI Response should specify its Biolink Model version compliance."
-      knowledge_graph:
-        empty:
-          $message: "Response returned an empty Message Knowledge Graph?"
-          $description: "An empty Knowledge Graph is allowed but merits a boundary response warning?"
-      results:
-        empty:
-          $message: "Response returned empty Message.results?"
-          $description: "Empty Results is allowed but merits a boundary response warning?"
+      message:
+        knowledge_graph:
+          empty:
+            $message: "Response returned an empty Message Knowledge Graph?"
+            $description: "An empty Knowledge Graph is allowed but merits a boundary response warning?"
+        results:
+          empty:
+            $message: "Response returned empty Message.results?"
+            $description: "Empty Results is allowed but merits a boundary response warning?"
       workflow:
         runner_parameters:
           missing:
             $message: "TRAPI Response.workflow.runner_parameters property is missing?"
             $description: "If a 'runner_parameters' property value is given for a workflow step specification, it should not be null. This field will be ignored?"
         parameters:
           missing:
```

### Comparing `reasoner_validator-4.1.3/reasoner_validator/github.py` & `reasoner_validator-4.1.4/reasoner_validator/github.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.3/reasoner_validator/message.py` & `reasoner_validator-4.1.4/reasoner_validator/message.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.3/reasoner_validator/report.py` & `reasoner_validator-4.1.4/reasoner_validator/report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.3/reasoner_validator/sri/util.py` & `reasoner_validator-4.1.4/reasoner_validator/sri/util.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.3/reasoner_validator/trapi/__init__.py` & `reasoner_validator-4.1.4/reasoner_validator/trapi/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.3/reasoner_validator/trapi/mapping.py` & `reasoner_validator-4.1.4/reasoner_validator/trapi/mapping.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.3/reasoner_validator/validation_codes.py` & `reasoner_validator-4.1.4/reasoner_validator/validation_codes.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.3/reasoner_validator/validator.py` & `reasoner_validator-4.1.4/reasoner_validator/validator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,10 @@
-from typing import Optional, List, Dict
-
-from bmt import Toolkit
+from typing import Optional, Tuple, List, Dict
 
 from reasoner_validator.biolink import (
-    BMTWrapper,
     BiolinkValidator,
     get_biolink_model_toolkit
 )
 
 from reasoner_validator.report import TRAPIGraphType
 from reasoner_validator.trapi import LATEST_TRAPI_RELEASE, TRAPI_1_4_0_SEMVER
 from reasoner_validator.trapi.mapping import MappingValidator, check_node_edge_mappings
@@ -71,15 +68,16 @@
             self._is_trapi_1_4_or_later = target_major_version >= TRAPI_1_4_0_SEMVER
         except SemVerError as sve:
             logger.error(f"Current TRAPI release '{self.trapi_version}' seems invalid: {str(sve)}. Reset to latest?")
             self.trapi_version = LATEST_TRAPI_RELEASE
             self._is_trapi_1_4_or_later = True
         return self._is_trapi_1_4_or_later
 
-    def sanitize_workflow(self, response: Dict) -> Dict:
+    @staticmethod
+    def sanitize_workflow(response: Dict) -> Dict:
         """
         Workflows in TRAPI Responses cannot be validated further due to missing tags and None values.
         This method is a temporary workaround to sanitize the query for additional validation.
 
         :param response: Dict full TRAPI Response JSON object
         :return: Dict, response with discretionary removal of content which
                        triggers (temporarily) unwarranted TRAPI validation failures
@@ -257,21 +255,21 @@
         Validate a TRAPI Query Graph.
         :param message: input message expected to contain the 'query_graph'
         :return: bool, False, if validation errors
         """
         # Query Graph must not be missing...
         if 'query_graph' not in message:
             if not self.suppress_empty_data_warnings:
-                self.report(code="error.trapi.response.query_graph.missing")
+                self.report(code="error.trapi.response.message.query_graph.missing")
         else:
             # ... nor empty
             query_graph = message['query_graph']
             if not (query_graph and len(query_graph) > 0):
                 if not self.suppress_empty_data_warnings:
-                    self.report(code="error.trapi.response.query_graph.empty")
+                    self.report(code="error.trapi.response.message.query_graph.empty")
             else:
                 # Validate the TRAPI compliance of the Query Graph
                 self.is_valid_trapi_query(instance=query_graph, component="QueryGraph")
 
                 if self.validate_biolink():
                     # Conduct validation of Biolink Model compliance
                     # of the Query Graph, if not suppressed...
@@ -297,27 +295,27 @@
         # This integrity constraint may not really be necessary
         # since negative numbers are functionally equivalent to zero
         assert edges_limit >= 0, "The 'edges_limit' must be zero or a positive integer!"
 
         # The Knowledge Graph should not be missing
         if 'knowledge_graph' not in message:
             if not self.suppress_empty_data_warnings:
-                self.report(code="error.trapi.response.knowledge_graph.missing")
+                self.report(code="error.trapi.response.message.knowledge_graph.missing")
         else:
             knowledge_graph = message['knowledge_graph']
             # The Knowledge Graph should also not generally be empty? Issue a warning
             if not (
                     knowledge_graph and len(knowledge_graph) > 0 and
                     "nodes" in knowledge_graph and knowledge_graph["nodes"] and
                     "edges" in knowledge_graph and knowledge_graph["edges"]
             ):
                 # An empty knowledge graph (warning) does not generally invalidate
                 # the whole Message, but no more validation tests are needed
                 if not self.suppress_empty_data_warnings:
-                    self.report(code="warning.trapi.response.knowledge_graph.empty")
+                    self.report(code="warning.trapi.response.message.knowledge_graph.empty")
             else:
                 mapping_validator: MappingValidator = check_node_edge_mappings(knowledge_graph)
                 if mapping_validator.has_messages():
                     self.merge(mapping_validator)
 
                 # ...then if not empty, validate a subgraph sample of the associated
                 # Knowledge Graph (since some TRAPI response kg's may be huge!)
@@ -352,27 +350,27 @@
         #     :type output_element: str
         #     :param output_node_binding: node 'a' or 'b' of the ('one hop') QGraph test query
         #     :type output_node_binding: str
 
         # The Message.Results key should not be missing?
         if 'results' not in message:
             if not self.suppress_empty_data_warnings:
-                self.report(code="error.trapi.response.results.missing")
+                self.report(code="error.trapi.response.message.results.missing")
         else:
             results = message['results']
 
             if not (results and len(results) > 0):
                 if not self.suppress_empty_data_warnings:
-                    self.report(code="warning.trapi.response.results.empty")
+                    self.report(code="warning.trapi.response.message.results.empty")
                     # An empty result (warning) does not generally invalidate
                     # the whole Message, but no more validation tests are needed
 
             elif not isinstance(results, List):
                 # The Message.results should be an array of Result objects
-                self.report(code="error.trapi.response.results.not_array")
+                self.report(code="error.trapi.response.message.results.not_array")
 
             else:
                 # Validate a subsample of a non-empty Message.results component.
                 results_sample = self.sample_results(results, sample_size=sample_size)
                 for result in results_sample:
 
                     # generally validate against the pertinent schema
@@ -412,16 +410,15 @@
                     #         )
                     #         # data_dump=f"Resolved aliases:\n{','.join(output_aliases)}\n" +
                     #         #           f"Result object IDs:\n{_output(object_ids,flat=True)}"
 
         # Only 'error' but not 'info' nor 'warning' messages invalidate the overall Message
         return False if self.has_errors() else True
 
-    @staticmethod
-    def case_node_found(target: str, identifiers: List[str], case: Dict, nodes: Dict) -> bool:
+    def case_node_found(self, target: str, identifiers: List[str], case: Dict, nodes: Dict) -> bool:
         """
         Check for presence of the target identifier,
         with expected categories, in the "nodes" catalog.
 
         :param target: 'subject' or 'object'
         :param identifiers: List of node (CURIE) identifiers to be checked in the "nodes" catalog
         :param case: Dict, full test case (to access the target node 'category')
@@ -440,59 +437,64 @@
         for identifier in identifiers:
             if identifier in nodes.keys():
                 # Found the target node identifier,
                 # but is the expected category present?
                 node_details = nodes[identifier]
                 if "categories" in node_details:
                     category = case[f"{target}_category"]
-                    if category in node_details["categories"]:
+                    categories: List[str] = self.bmt.get_ancestors(category, formatted=True, mixin=False)
+                    if any([category in node_details["categories"] for category in categories]):
                         return True
 
         # Target node identifier or categories is missing,
         # or not annotated with the expected category?
         return False
 
     @staticmethod
-    def case_edge_bindings(target_edge_id: str, data: Dict) -> bool:
+    def case_edge_bindings(q_edge_ids: Tuple[str], target_edge_id: str, data: Dict) -> bool:
         """
         Check if target query edge id and knowledge graph edge id are in specified edge_bindings.
+        :rtype: object
+        :param q_edge_ids: Tuple[str], expected query edge identifiers in a matching result
         :param target_edge_id:  str, expected knowledge edge identifier in a matching result
         :param data: TRAPI version-specific Response context from which the 'edge_bindings' may be retrieved
         :return: True, if found
         """
         edge_bindings: Dict = data["edge_bindings"]
         for bound_query_id, edge in edge_bindings.items():
-            # The expected query identifier in this context is
-            # hard coded as 'ab' in the 'one_hop.util.py' model
-            if bound_query_id == "ab":
+            if bound_query_id in q_edge_ids:
                 for binding_details in edge:
                     # TRAPI schema validation actually
                     # catches missing id's, but sanity check...
                     if "id" in binding_details:
                         if target_edge_id == binding_details["id"]:
                             return True
         return False
 
     def case_result_found(
             self,
+            query_graph: Dict,
             subject_id: str,
             object_id: str,
             edge_id: str,
-            results: List,
-            trapi_version: str
+            results: List
     ) -> bool:
         """
         Validate that test case S--P->O edge is found bound to the Results?
+        :param query_graph: Dict, query graph to which the results pertain
         :param subject_id: str, subject node (CURIE) identifier
         :param object_id:  str, subject node (CURIE) identifier
         :param edge_id:  str, subject node (CURIE) identifier
         :param results: List of (TRAPI-version specific) Result objects
-        :param trapi_version: str, target TRAPI version of the Response being validated
         :return: bool, True if case S-P-O edge was found in the results
         """
+        assert query_graph, "case_result_found() encountered an empty query graph"
+        q_edges: Dict = query_graph["edges"]
+        q_edge_ids = tuple(q_edges.keys())
+
         result_found: bool = False
         result: Dict
 
         for result in results:
 
             # Node binding validation still currently same for recent TRAPI versions
             node_bindings: Dict = result["node_bindings"]
@@ -526,14 +528,15 @@
                 #         "a2": {
                 #             "edges" [
                 #                 "extra_edge1"
                 #             ]
                 #         }
                 #     },
                 #     "results": [
+                #         # Single result in list:
                 #         {
                 #             "node_bindings": {
                 #                 "n0": [
                 #                     "id": "diabetes"
                 #                 ],
                 #                 "n1": [
                 #                     "id": "metformin"
@@ -562,111 +565,147 @@
                 #         }
                 #     ]
 
                 # result["analyses"] may be empty but prior TRAPI 1.4.0 schema validation ensures that
                 # the "analysis" key is at least present plus the objects themselves are 'well-formed'
                 analyses: List = result["analyses"]
                 for analysis in analyses:
-                    edge_id_found = self.case_edge_bindings(edge_id, analysis)
+                    edge_id_found: bool = self.case_edge_bindings(q_edge_ids, edge_id, analysis)
                     if edge_id_found:
                         break
 
             else:
                 # TRAPI 1.3.0 or earlier?
                 #
                 # Then, the TRAPI 1.3.0 Message Results (referencing the
                 # Response Knowledge Graph) could be something like this:
                 #
                 #     "results": [
+                #         # Single result in list:
                 #         {
                 #             "node_bindings": {
                 #                # node "id"'s in knowledge graph, in edge "id"
                 #                 "type-2 diabetes": [{"id": "MONDO:0005148"}],
                 #                 "drug": [{"id": "CHEBI:6801"}]
                 #             },
                 #             "edge_bindings": {
                 #                 # the edge binding key should be the query edge id
                 #                 # bounded edge "id" is from knowledge graph
-                #                 "treats": [{"id": "df87ff82"}]
+                #                 "treated_by": [{"id": "df87ff82"}]
                 #             }
                 #         }
                 #     ]
                 #
-                edge_id_found = self.case_edge_bindings(edge_id, result)
+                edge_id_found: bool = self.case_edge_bindings(q_edge_ids, edge_id, result)
 
             if subject_id_found and object_id_found and edge_id_found:
                 result_found = True
                 break
 
         return result_found
 
     def case_input_found_in_response(
             self,
             case: Dict,
-            response: Dict,
-            trapi_version: str
+            response: Dict
     ) -> bool:
         """
         Predicate to validate if test data test case specified edge is returned
         in the Knowledge Graph of the TRAPI Response Message. This method assumes
         that the TRAPI response is already generally validated as well-formed.
 
         :param case: Dict, input data test case
         :param response: Dict, TRAPI Response whose message ought to contain the test case edge
-        :param trapi_version: str, TRAPI version of response being tested
         :return: True if test case edge found; False otherwise
         """
         # sanity checks
         assert case, "case_input_found_in_response(): Empty or missing test case data!"
         assert response, "case_input_found_in_response(): Empty or missing TRAPI Response!"
         assert "message" in response, "case_input_found_in_response(): TRAPI Response missing its Message component!"
-        assert trapi_version
 
         #
         # case: Dict parameter contains something like:
         #
         #     idx: 0,
         #     subject_category: 'biolink:SmallMolecule',
         #     object_category: 'biolink:Disease',
         #     predicate: 'biolink:treats',
         #     subject_id: 'CHEBI:3002',  # may have the deprecated key 'subject' here
         #     object_id: 'MESH:D001249', # may have the deprecated key 'object' here
         #
         # the contents for which ought to be returned in
-        # the TRAPI Knowledge Graph, as a Result mapping?
+        # the TRAPI Knowledge Graph, with a Result mapping?
         #
-
         message: Dict = response["message"]
-        if not (
-            "knowledge_graph" in message and message["knowledge_graph"] and
-            "results" in message and message["results"]
-        ):
-            # empty knowledge graph is syntactically ok, but in
-            # this, input test data edge is automatically deemed missing
-            return False
 
-        # TODO: We need to check **here*** whether or not the
-        #       TRAPI response returned the original test case edge!!?!!
-        #       Not totally sure if we should first search the Results then
-        #       the Knowledge Graph, or go directly to the Knowledge Graph...
+        # Another sanity check - unlikely to be a problem since
+        # TRAPI schema validation should have picked it up since
+        # the TRAPI Message is "nullable: false" in the schema
+        assert message, "case_input_found_in_response(): Empty or missing TRAPI message component!"
+
+        message_found: bool = False
+        if "query_graph" not in message:
+            # missing query graph allowed by the TRAPI schema but
+            # the input test data edge is automatically deemed missing
+            self.report(
+                code="error.trapi.response.message.query_graph.missing"
+            )
+        elif not message["query_graph"]:
+            # empty query graph is also allowed by the TRAPI schema
+            # but the input test data edge is automatically deemed missing
+            self.report(
+                code="error.trapi.response.message.query_graph.empty"
+            )
+        elif "knowledge_graph" not in message:
+            # missing knowledge graph allowed by the TRAPI schema but
+            # the input test data edge is automatically deemed missing
+            self.report(
+                code="error.trapi.response.message.knowledge_graph.missing"
+            )
+        elif not message["knowledge_graph"]:
+            # empty knowledge graph is also allowed by the TRAPI schema
+            # but the input test data edge is automatically deemed missing
+            self.report(
+                code="error.trapi.response.message.knowledge_graph.empty"
+            )
+        elif "results" not in message:
+            # missing results are allowed by the TRAPI schema but
+            # the input test data edge is automatically deemed missing
+            self.report(
+                code="error.trapi.response.message.results.missing"
+            )
+        elif not message["results"]:
+            # missing results are allowed by the TRAPI schema but
+            # the input test data edge are automatically deemed missing
+            self.report(
+                code="error.trapi.response.message.results.empty"
+            )
+        else:
+            message_found = True
+
+        if not message_found:
+            return False
 
         # The Message Query Graph could be something like:
         # "query_graph": {
         #     "nodes": {
         #         "type-2 diabetes": {"ids": ["MONDO:0005148"]},
         #         "drug": {"categories": ["biolink:Drug"]}
         #     },
         #     "edges": {
-        #         "treats": {
-        #             "subject": "drug",
-        #             "predicates": ["biolink:treats"],
-        #             "object": "type-2 diabetes"
+        #         "treated_by": {
+        #             "subject": "type-2 diabetes",
+        #             "predicates": ["biolink:treated_by"],
+        #             "object": "drug"
         #         }
         #     }
         # }
+
+        query_graph: Dict = message["query_graph"]
+
         #
         # with a Response Message Knowledge Graph
         # dictionary with 'nodes' and 'edges':
         #
         # "knowledge_graph": {
         #     "nodes": ...,
         #     "edges": ...
@@ -682,21 +721,29 @@
         #
         # Check for case 'subject_id' and 'object_id',
         # with expected categories, in nodes catalog
         nodes: Dict = knowledge_graph["nodes"]
         subject_id = case["subject_id"] if "subject_id" in case else case["subject"]
         subject_aliases = get_aliases(subject_id)
         if not self.case_node_found("subject", subject_aliases, case, nodes):
-            # 'subject' node identifier not found?
+            self.report(
+                code="error.trapi.response.message.knowledge_graph.node.missing",
+                identifier=subject_id,
+                context="subject"
+            )
             return False
 
         object_id = case["object_id"] if "object_id" in case else case["object"]
         object_aliases = get_aliases(object_id)
         if not self.case_node_found("object", object_aliases, case, nodes):
-            # 'object' node identifier not found?
+            self.report(
+                code="error.trapi.response.message.knowledge_graph.node.missing",
+                identifier=object_id,
+                context="object"
+            )
             return False
 
         # In the Knowledge Graph:
         #
         #     "edges": {
         #         "df87ff82": {
         #             "subject": "CHEBI:6801",
@@ -705,26 +752,22 @@
         #         }
         #     }
         #
         # Check in the edges catalog for an edge containing
         # the case 'subject_id', 'predicate' and 'object_id'
         edges: Dict = knowledge_graph["edges"]
 
-        bmtw = BMTWrapper(biolink_version=self.biolink_version)
-
         predicate = case["predicate"] if "predicate" in case else case["predicate_id"]
-
-        bmt: Optional[Toolkit] = bmtw.get_bmt()
         predicate_descendants: List[str]
         inverse_predicate_descendants: List[str] = list()  # may sometimes remain empty...
-        if bmt is not None:
-            predicate_descendants = bmt.get_descendants(predicate, formatted=True)
-            inverse_predicate = bmtw.get_inverse_predicate(predicate)
+        if self.validate_biolink():
+            predicate_descendants = self.bmt.get_descendants(predicate, formatted=True)
+            inverse_predicate = self.get_inverse_predicate(predicate)
             if inverse_predicate:
-                inverse_predicate_descendants = bmt.get_descendants(inverse_predicate, formatted=True)
+                inverse_predicate_descendants = self.bmt.get_descendants(inverse_predicate, formatted=True)
         else:
             # simpler case in which we are ignoring deep Biolink Model validation
             predicate_descendants = [predicate]
 
         edge_id_match: Optional[str] = None
         subject_match: Optional[str] = None
         object_match: Optional[str] = None
@@ -742,20 +785,31 @@
                     edge["object"] in subject_aliases:
                 # observation of the inverse edge is also counted as a match?
                 subject_match = edge["subject"]
                 object_match = edge["object"]
                 edge_id_match = edge_id
                 break
 
+        edge_id: str = \
+            f"{case['idx']}|" +\
+            f"({case['subject_id']}#{case['subject_category']})" + \
+            f"-[{predicate}]->" + \
+            f"({case['object_id']}#{case['object_category']})"
+
         if edge_id_match is None:
-            # Test case S--P->O edge not found?
+            self.report(
+                code="error.trapi.response.message.knowledge_graph.edge.missing",
+                identifier=edge_id
+            )
             return False
 
         results: List = message["results"]
-        if not self.case_result_found(subject_match, object_match, edge_id_match, results, trapi_version):
-            # Some components of test case S--P->O edge
-            # NOT bound within any Results?
+        if not self.case_result_found(query_graph, subject_match, object_match, edge_id_match, results):
+            self.report(
+                code="error.trapi.response.message.result.missing",
+                identifier=edge_id
+            )
             return False
 
         # By this point, the case data assumed to be
         # successfully validated in the TRAPI Response?
         return True
```

### Comparing `reasoner_validator-4.1.3/reasoner_validator/versioning.py` & `reasoner_validator-4.1.4/reasoner_validator/versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.3/reasoner_validator/versions.yaml` & `reasoner_validator-4.1.4/reasoner_validator/versions.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.3/tests/__init__.py` & `reasoner_validator-4.1.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.3/tests/test_biolink_compliance_validation.py` & `reasoner_validator-4.1.4/tests/test_biolink_compliance_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,19 +232,19 @@
             "info.input_edge.predicate.abstract"
         ),
         (   # Query 10 - Predicate is a mixin; default 'strict_validation' == False for input_edge
             LATEST_BIOLINK_MODEL_VERSION,
             {
                 'subject_category': 'biolink:Drug',
                 'object_category': 'biolink:BiologicalProcess',
-                'predicate': 'biolink:decreases_amount_or_activity_of',
+                'predicate': 'biolink:treats',
                 'subject_id': 'NDC:50090‑0766',  # Metformin
                 'object_id': 'GO:0006094'  # Gluconeogenesis
             },
-            # f"{INPUT_EDGE_PREFIX}: INFO - Predicate element 'biolink:decreases_amount_or_activity_of' is a mixin."
+            # f"{INPUT_EDGE_PREFIX}: INFO - Predicate element 'biolink:treats' is a mixin."
             "info.input_edge.predicate.mixin"
         ),
         (   # Query 11 - Unknown predicate element
             LATEST_BIOLINK_MODEL_VERSION,
             {
                 'subject_category': 'biolink:AnatomicalEntity',
                 'object_category': 'biolink:AnatomicalEntity',
@@ -830,15 +830,35 @@
                 }
             },
             # f"{QUERY_GRAPH_PREFIX}: WARNING - Edge predicate 'biolink:affected_by' is non-canonical?"
             "warning.query_graph.edge.predicate.non_canonical"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 18: 'Subject' id used in edge is mandatory
+            # Query 18: ... but can be now be a mixin for Biolink Model release >= 4.2.0
+            {
+                "nodes": {
+                    "type-2 diabetes": {"ids": ["MONDO:0005148"]},
+                    "drug": {
+                        "categories": ["biolink:Drug"]
+                    }
+                },
+                "edges": {
+                    "treats": {
+                        "subject": "drug",
+                        "predicates": ["biolink:treats"],
+                        "object": "type-2 diabetes"
+                    }
+                }
+            },
+            "info.query_graph.edge.predicate.mixin"
+        ),
+        (
+            LATEST_BIOLINK_MODEL_VERSION,
+            # Query 19: 'Subject' id used in edge is mandatory
             {
                 "nodes": {
                     "drug": {
                         "categories": ["biolink:Drug"]
                     },
                     "type-2 diabetes": {"ids": ["MONDO:0005148"]}
                 },
@@ -851,15 +871,15 @@
             },
             # f"{QUERY_GRAPH_PREFIX}: ERROR - Edge 'None--['biolink:ameliorates_condition']->type-2 diabetes' " +
             # "has a missing or empty 'subject' slot value!"
             "error.query_graph.edge.subject.missing"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 19: 'Subject' id used in edge is missing from the nodes catalog?
+            # Query 20: 'Subject' id used in edge is missing from the nodes catalog?
             {
                 "nodes": {
                     "type-2 diabetes": {"ids": ["MONDO:0005148"]}
                 },
                 "edges": {
                     "treats": {
                         "subject": "drug",
@@ -869,15 +889,15 @@
                 }
             },
             # f"{QUERY_GRAPH_PREFIX}: ERROR - Edge 'subject' id 'drug' is missing from the nodes catalog!"
             "error.query_graph.edge.subject.missing_from_nodes"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 20: 'Object' id used in edge is mandatory
+            # Query 21: 'Object' id used in edge is mandatory
             {
                 "nodes": {
                     "drug": {
                         "categories": ["biolink:Drug"]
                     },
                     "type-2 diabetes": {"ids": ["MONDO:0005148"]}
                 },
@@ -890,15 +910,15 @@
             },
             # f"{QUERY_GRAPH_PREFIX}: ERROR - Edge 'drug--['biolink:ameliorates_condition']->None' " +
             # f"has a missing or empty 'object' slot value!"
             "error.query_graph.edge.object.missing"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 21: 'Object' id used in edge is missing from the nodes catalog?
+            # Query 22: 'Object' id used in edge is missing from the nodes catalog?
             {
                 "nodes": {
                     "drug": {
                         "categories": ["biolink:Drug"]
                     }
                 },
                 "edges": {
@@ -910,15 +930,15 @@
                 }
             },
             # f"{QUERY_GRAPH_PREFIX}: ERROR - Edge 'object' id 'type-2 diabetes' is missing from the nodes catalog!"
             "error.query_graph.edge.object.missing_from_nodes"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 22: Node 'is_set' value is not a boolean
+            # Query 23: Node 'is_set' value is not a boolean
             {
                 "nodes": {
                     "type-2 diabetes": {"ids": ["MONDO:0005148"]},
                     "drug": {
                         "categories": ["biolink:Drug"],
                         "is_set": "should-be-a-boolean"
                     }
@@ -932,15 +952,15 @@
                 }
             },
             # f"{QUERY_GRAPH_PREFIX}: ERROR - Node 'drug.is_set' slot is not a boolean value!"
             "error.query_graph.node.is_set.not_boolean"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 23: Unmapped node ids against any of the specified Biolink Model categories
+            # Query 24: Unmapped node ids against any of the specified Biolink Model categories
             {
                 "nodes": {
                     "type-2 diabetes": {
                         "ids": ["FOO:12345", "BAR:67890"],
                         "categories": ["biolink:Disease", "biolink:Gene"]
                     },
                     "drug": {
@@ -957,15 +977,15 @@
             },
             # f"{QUERY_GRAPH_PREFIX}: WARNING - Node 'type-2 diabetes' has identifiers ['FOO:12345', 'BAR:67890'] " +
             # "unmapped to the target categories: ['biolink:Disease', 'biolink:Gene']?"
             "warning.query_graph.node.ids.unmapped_prefix"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 24: Abstract category in query graph? Simply ignored now during validation...
+            # Query 25: Abstract category in query graph? Simply ignored now during validation...
             {
                 "nodes": {
                     "type-2 diabetes": {"ids": ["MONDO:0005148"]},
                     "drug": {
                         "categories": ["biolink:BiologicalEntity"]
                     }
                 },
@@ -977,15 +997,15 @@
                     }
                 }
             },
             ""
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 25: Mixin category in query graph? Simply ignored now during validation...
+            # Query 26: Mixin category in query graph? Simply ignored now during validation...
             {
                 "nodes": {
                     "type-2 diabetes": {"ids": ["MONDO:0005148"]},
                     "drug": {
                         "categories": ["biolink:ChemicalOrDrugOrTreatment"]
                     }
                 },
@@ -997,15 +1017,15 @@
                     }
                 }
             },
             ""
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 26: Query edge predicate is a mixin; default 'strict_validation' == False for query graphs
+            # Query 27: Query edge predicate is a mixin; default 'strict_validation' == False for query graphs
             {
                 "nodes": {
                     "drug": {
                         "ids": ["RXCUI:861026"],
                         "categories": ["biolink:Drug"]
                     },
                     "gene": {
@@ -1021,15 +1041,15 @@
                 }
             },
             # f"{QUERY_GRAPH_PREFIX}: INFO - Predicate element 'biolink:treats' is a mixin."
             "info.query_graph.edge.predicate.mixin"
         ),
         (
             "4.1.6",
-            # Query 27: Query edge 'treats' predicate is a special case of mixin;
+            # Query 28: Query edge 'treats' predicate is a special case of mixin;
             #           default 'strict_validation' == False for query graphs
             {
                 "nodes": {
                     "drug": {
                         "ids": ["RXCUI:861026"],
                         "categories": ["biolink:Drug"]
                     },
@@ -1045,15 +1065,15 @@
                     }
                 }
             },
             ""
         ),
         (
             SUPPRESS_BIOLINK_MODEL_VALIDATION,
-            # Query 28: ... but if present, predicates must be valid
+            # Query 29: ... but if present, predicates must be valid
             #           for the specified Biolink Model version, but...
             {
                 "nodes": {
                     "type-2 diabetes": {"ids": ["MONDO:0005148"]},
                     "drug": {
                         "categories": ["biolink:Drug"]
                     }
@@ -1068,15 +1088,15 @@
             },
             # ...since Biolink Model validation is tagged as 'suppress',
             # we  don't expect any validation output here?
             ""
         ),
         (
             SUPPRESS_BIOLINK_MODEL_VALIDATION,
-            # Query 29: Query edge predicate is a mixin...but...
+            # Query 30: Query edge predicate is a mixin...but...
             {
                 "nodes": {
                     "IRS1": {"ids": ["HGNC:6125"], "categories": ["biolink:Gene"]},
                     "drug": {
                         "categories": ["biolink:Drug"]
                     }
                 },
@@ -3065,17 +3085,18 @@
                         ]
                     }
                 }
             },
             "error.knowledge_graph.edge.predicate.mixin"
         ),
         (
-            LATEST_BIOLINK_MODEL_VERSION,
+            "4.1.6",
             # Query 20: predicate is a mixin - not allowed in Knowledge Graphs, but "biolink:interacts_with"
             #           is tagged as an exception (see https://github.com/NCATSTranslator/reasoner-validator/issues/97)
+            #           for Biolink Model releases < 4.2.0
             {
                 "nodes": {
                     "HGNC:3059": {
                         "name": "Heparin binding EGF like growth factor",
                         "categories": [
                            "biolink:Gene"
                         ],
@@ -3110,15 +3131,58 @@
                 }
             },
             ""  # predicate "biolink:interacts_with" is now on
                 # the PREDICATE_INCLUSIONS list so 'mixin' validation is skipped
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 21: predicate is abstract - not allowed in Knowledge Graphs
+            # Query 21: predicate is a mixin - not allowed in Knowledge Graphs,
+            #           but only in QueryGraphs from Biolink Model 4.2.0 onwards
+            {
+                "nodes": {
+                    "HGNC:3059": {
+                        "name": "Heparin binding EGF like growth factor",
+                        "categories": [
+                           "biolink:Gene"
+                        ],
+                        "description": "heparin binding EGF like growth factor"
+                    },
+                    "HGNC:391": {
+                        "name": "AKT serine/threonine kinase 1",
+                        "categories": [
+                            "biolink:Gene"
+                        ],
+                        "description": "AKT serine/threonine kinase 1"
+                    }
+                },
+                "edges": {
+                    "edge_1": {
+                        "subject": "HGNC:3059",
+                        "predicate": "biolink:interacts_with",
+                        "object": "HGNC:391",
+                        "attributes": [
+                            {
+                                "attribute_type_id": "biolink:stoichiometry",
+                                "value": 2
+                            }
+                        ] + DEFAULT_KL_AND_AT_ATTRIBUTES,
+                        "sources": [
+                            {
+                                "resource_id": "infores:molepro",
+                                "resource_role": "primary_knowledge_source"
+                            }
+                        ]
+                    }
+                }
+            },
+            "error.knowledge_graph.edge.predicate.mixin"
+        ),
+        (
+            LATEST_BIOLINK_MODEL_VERSION,
+            # Query 22: predicate is abstract - not allowed in Knowledge Graphs
             {
                 "nodes": {
                     "PMID:1234": {
                         "name": "article title",
                         "categories": [
                            "biolink:InformationContentEntity"
                         ],
@@ -3152,15 +3216,15 @@
                     }
                 }
             },
             "error.knowledge_graph.edge.predicate.abstract"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 22: predicate is non-canonical
+            # Query 23: predicate is non-canonical
             {
                 "nodes": SIMPLE_SAMPLE_NODES,
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:affected_by",
                         "object": "PUBCHEM.COMPOUND:597",
@@ -3179,15 +3243,15 @@
                     }
                 }
             },
             "warning.knowledge_graph.edge.predicate.non_canonical"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 23: 'object' id is missing from the nodes catalog
+            # Query 24: 'object' id is missing from the nodes catalog
             {
                 "nodes": SIMPLE_SAMPLE_NODES,
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "PUBCHEM.COMPOUND:678",
@@ -3206,15 +3270,15 @@
                     }
                 }
             },
             "error.knowledge_graph.edge.object.missing_from_nodes"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 24: attribute 'attribute_type_id' is missing
+            # Query 25: attribute 'attribute_type_id' is missing
             {
                 "nodes": SIMPLE_SAMPLE_NODES,
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "PUBCHEM.COMPOUND:597",
@@ -3232,15 +3296,15 @@
                     }
                 }
             },
             "error.knowledge_graph.edge.attribute.type_id.missing"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 25: attribute 'value' is missing?
+            # Query 26: attribute 'value' is missing?
             {
                 "nodes": SIMPLE_SAMPLE_NODES,
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "PUBCHEM.COMPOUND:597",
@@ -3259,15 +3323,15 @@
                     }
                 }
             },
             "error.knowledge_graph.edge.attribute.value.missing"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 26: 'attribute_type_id' is not a CURIE
+            # Query 27: 'attribute_type_id' is not a CURIE
             {
                 "nodes": SIMPLE_SAMPLE_NODES,
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "PUBCHEM.COMPOUND:597",
@@ -3286,15 +3350,15 @@
                     }
                 }
             },
             "error.knowledge_graph.edge.attribute.type_id.not_curie"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 27: 'attribute_type_id' is a Biolink (node) category - not sure yet
+            # Query 28: 'attribute_type_id' is a Biolink (node) category - not sure yet
             #           whether this reflects "best practices" so issue a warning for now
             {
                 "nodes": SIMPLE_SAMPLE_NODES,
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
@@ -3314,15 +3378,15 @@
                     }
                 }
             },
             "warning.knowledge_graph.edge.attribute.type_id.is_category"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 28: 'attribute_type_id' is a Biolink (edge) predicate - not sure yet
+            # Query 29: 'attribute_type_id' is a Biolink (edge) predicate - not sure yet
             #           whether this reflects "best practices" so issue a warning for now
             {
                 "nodes": SIMPLE_SAMPLE_NODES,
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
@@ -3342,15 +3406,15 @@
                     }
                 }
             },
             "warning.knowledge_graph.edge.attribute.type_id.is_predicate"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 29: 'attribute_type_id' is not a 'biolink:association_slot' (biolink:synonym is a node property)
+            # Query 30: 'attribute_type_id' is not a 'biolink:association_slot' (biolink:synonym is a node property)
             {
                 "nodes": SIMPLE_SAMPLE_NODES,
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "PUBCHEM.COMPOUND:597",
@@ -3369,15 +3433,15 @@
                     }
                 }
             },
             "warning.knowledge_graph.edge.attribute.type_id.not_association_slot"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 30: 'attribute_type_id' has a 'biolink' CURIE prefix and
+            # Query 31: 'attribute_type_id' has a 'biolink' CURIE prefix and
             #           is an association_slot, so it should pass
             {
                 "nodes": SIMPLE_SAMPLE_NODES,
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
@@ -3401,15 +3465,15 @@
                     }
                 }
             },
             ""  # this should recognize the 'attribute_type_id' as a Biolink CURIE
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 31: 'attribute_type_id' has a CURIE prefix namespace unknown to Biolink?
+            # Query 32: 'attribute_type_id' has a CURIE prefix namespace unknown to Biolink?
             {
                 "nodes": SIMPLE_SAMPLE_NODES,
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "PUBCHEM.COMPOUND:597",
@@ -3426,15 +3490,15 @@
                             }
                         ]
                     }
                 }
             },
             "warning.knowledge_graph.edge.attribute.type_id.non_biolink_prefix"
         ),
-        (   # Query 32:  # An earlier Biolink Model won't recognize a category not found in its specified release
+        (   # Query 33:  # An earlier Biolink Model won't recognize a category not found in its specified release
             "1.8.2",
             {
                 # Sample nodes
                 'nodes': {
                     "NCBIGene:29974": {
                         "categories": [
                             "biolink:Gene"
@@ -3455,15 +3519,15 @@
                        "predicate": "biolink:physically_interacts_with",
                        "object": "PUBCHEM.COMPOUND:597",
                     }
                 }
             },
             "error.knowledge_graph.node.category.unknown"
         ),
-        (   # Query 33:  # 'attribute_type_id' has a CURIE prefix namespace unknown to Biolink but...
+        (   # Query 34:  # 'attribute_type_id' has a CURIE prefix namespace unknown to Biolink but...
             SUPPRESS_BIOLINK_MODEL_VALIDATION,
             {
                 "nodes": SIMPLE_SAMPLE_NODES,
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
@@ -3485,15 +3549,15 @@
             },
             # ...since Biolink Model validation is tagged as 'suppress',
             # we don't expect any validation output here?
             ""
         ),
         (
             SUPPRESS_BIOLINK_MODEL_VALIDATION,
-            # Query 34: 'attribute_type_id' is not a 'biolink:association_slot'
+            # Query 35: 'attribute_type_id' is not a 'biolink:association_slot'
             #           (biolink:synonym is a node property) but...
             {
                 "nodes": SIMPLE_SAMPLE_NODES,
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
@@ -3516,27 +3580,27 @@
             # ...since Biolink Model validation is tagged as 'suppress',
             # we don't expect any validation output here?
             ""
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
 
-            # Query 35: Knowledge Graph dangling nodes error
+            # Query 36: Knowledge Graph dangling nodes error
             {
                 # Sample nodes with extra  unused node
                 'nodes': SAMPLE_NODES_WITH_UNUSED_NODE,
                 # Sample edge
                 'edges': SAMPLE_EDGE_WITH_ATTRIBUTES_AND_SOURCES
             },
             "warning.knowledge_graph.nodes.dangling"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
 
-            # Query 36: Knowledge Graph edge duplicated Knowledge Level
+            # Query 37: Knowledge Graph edge duplicated Knowledge Level
             {
                 'nodes': SAMPLE_NODES_WITH_ATTRIBUTES,
                 'edges': sample_edge_with_attributes(
                     attributes=[
                         DEFAULT_KL,
                         DEFAULT_KL,
                         DEFAULT_AT
@@ -3544,30 +3608,30 @@
                 )
             },
             "error.knowledge_graph.edge.knowledge_level.duplicated"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
 
-            # Query 37: Knowledge Graph edge missing Knowledge Level
+            # Query 38: Knowledge Graph edge missing Knowledge Level
             {
                 'nodes': SAMPLE_NODES_WITH_ATTRIBUTES,
                 'edges': sample_edge_with_attributes(
                     attributes=[
                         DEFAULT_AT
                     ]
                 )
             },
             # This will be a warning for TRAPI 1.5.0 but should become an error in TRAPI 1.6.0
             "warning.knowledge_graph.edge.knowledge_level.missing"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
 
-            # Query 38: Knowledge Graph edge invalid Knowledge Level
+            # Query 39: Knowledge Graph edge invalid Knowledge Level
             {
                 'nodes': SAMPLE_NODES_WITH_ATTRIBUTES,
                 'edges': sample_edge_with_attributes(
                     attributes=[
                         {
                            "attribute_type_id": "biolink:knowledge_level",
                            "value": "not-a-knowledge-level"
@@ -3577,15 +3641,15 @@
                 )
             },
             "error.knowledge_graph.edge.knowledge_level.invalid"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
 
-            # Query 39: Knowledge Graph edge duplicated Agent Type
+            # Query 40: Knowledge Graph edge duplicated Agent Type
             {
                 'nodes': SAMPLE_NODES_WITH_ATTRIBUTES,
                 'edges': sample_edge_with_attributes(
                     attributes=[
                         DEFAULT_KL,
                         DEFAULT_AT,
                         DEFAULT_AT
@@ -3593,48 +3657,48 @@
                 )
             },
             "error.knowledge_graph.edge.agent_type.duplicated"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
 
-            # Query 40: Knowledge Graph edge missing Agent Type
+            # Query 41: Knowledge Graph edge missing Agent Type
             {
                 'nodes': SAMPLE_NODES_WITH_ATTRIBUTES,
                 'edges': sample_edge_with_attributes(
                     attributes=[
                         DEFAULT_KL
                     ]
                 )
             },
             # This will be a warning for TRAPI 1.5.0 but should become an error in TRAPI 1.6.0
             "warning.knowledge_graph.edge.agent_type.missing"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
 
-            # Query 41: Knowledge Graph edge invalid Agent Type
+            # Query 42: Knowledge Graph edge invalid Agent Type
             {
                 'nodes': SAMPLE_NODES_WITH_ATTRIBUTES,
                 'edges': sample_edge_with_attributes(
                     attributes=[
                         DEFAULT_KL,
                         {
                            "attribute_type_id": "biolink:agent_type",
                            "value": "not-an-agent-type"
                         }
                     ]
                 )
             },
             "error.knowledge_graph.edge.agent_type.invalid"
         ),
-(
+        (
             "4.1.6",
 
-            # Query 42: Sample full valid TRAPI Knowledge Graph
+            # Query 43: Sample full valid TRAPI Knowledge Graph
             {
                 # Sample nodes
                 'nodes': SAMPLE_NODES_WITH_ATTRIBUTES,
                 # Sample edge
                 'edges': SAMPLE_EDGE_WITH_ATTRIBUTES_AND_SOURCES
             },
             ""
```

### Comparing `reasoner_validator-4.1.3/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml` & `reasoner_validator-4.1.4/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.3/tests/test_response_validator.py` & `reasoner_validator-4.1.4/tests/test_response_validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,24 +69,24 @@
 
 _TEST_KG_1 = {
     "nodes": SAMPLE_NODES_WITH_ATTRIBUTES,
     "edges": _TEST_EDGES_1
 }
 
 _TEST_RESULTS_1 = [
-        {
-            "node_bindings": {
-                "type-2 diabetes": [{"id": "MONDO:0005148"}],
-                "drug": [{"id": "ncats.drug:9100L32L2N"}]
-            },
-            "edge_bindings": {
-                "treats": [{"id": "df87ff82"}]
-            }
+    {
+        "node_bindings": {
+            "type-2 diabetes": [{"id": "MONDO:0005148"}],
+            "drug": [{"id": "ncats.drug:9100L32L2N"}]
+        },
+        "edge_bindings": {
+            "treats": [{"id": "df87ff82"}]
         }
-    ]
+    }
+]
 
 # Sample edge 2
 _TEST_EDGES_2 = {
        "edge_1": {
            "subject": "NCBIGene:29974",
            "predicate": "biolink:physically_interacts_with",
            "object": "PUBCHEM.COMPOUND:597",
@@ -200,14 +200,43 @@
 
 
 _TEST_KG_4 = {
     "nodes": SAMPLE_NODES_WITH_ATTRIBUTES,
     "edges": _TEST_EDGES_4
 }
 
+_TEST_KG_EDGE_SOURCES = [
+    {
+        "resource_id": "infores:chebi",
+        "resource_role": "primary_knowledge_source",
+        "upstream_resource_ids": []
+    },
+    {
+        "resource_id": "infores:biothings-explorer",
+        "resource_role": "aggregator_knowledge_source",
+        "upstream_resource_ids": [
+            "infores:chebi"
+        ]
+    },
+    {
+        "resource_id": "infores:molepro",
+        "resource_role": "aggregator_knowledge_source",
+        "upstream_resource_ids": [
+            "infores:biothings-explorer"
+        ]
+    },
+    {
+        "resource_id": "infores:arax",
+        "resource_role": "aggregator_knowledge_source",
+        "upstream_resource_ids": [
+            "infores:molepro"
+        ]
+    }
+]
+
 # From Implementation Guidelines circa June 2023
 _TEST_TRAPI_1_4_2_FULL_SAMPLE = {
     "message": {
         "query_graph": {
             "nodes": {
                 "type-2 diabetes": {"ids": ["MONDO:0005148"]},
                 "drug": {"categories": ["biolink:Drug"]}
@@ -223,42 +252,15 @@
                 "ncats.drug:9100L32L2N": {"name": "metformin", "categories": ["biolink:Drug"]}
             },
             "edges": {
                 "df87ff82": {
                     "subject": "ncats.drug:9100L32L2N",
                     "predicate": "biolink:ameliorates_condition",
                     "object": "MONDO:0005148",
-                    "sources": [
-                        {
-                            "resource_id": "infores:chebi",
-                            "resource_role": "primary_knowledge_source",
-                            "upstream_resource_ids": []
-                        },
-                        {
-                            "resource_id": "infores:biothings-explorer",
-                            "resource_role": "aggregator_knowledge_source",
-                            "upstream_resource_ids": [
-                                "infores:chebi"
-                            ]
-                        },
-                        {
-                            "resource_id": "infores:molepro",
-                            "resource_role": "aggregator_knowledge_source",
-                            "upstream_resource_ids": [
-                                "infores:biothings-explorer"
-                            ]
-                        },
-                        {
-                            "resource_id": "infores:arax",
-                            "resource_role": "aggregator_knowledge_source",
-                            "upstream_resource_ids": [
-                                "infores:molepro"
-                            ]
-                        }
-                    ]
+                    "sources": _TEST_KG_EDGE_SOURCES
                 }
             }
         },
         "auxiliary_graphs": {
             "a0": {
                 "edges": [
                     "e02",
@@ -323,42 +325,15 @@
                 "ncats.drug:9100L32L2N": {"name": "metformin", "categories": ["biolink:Drug"]}
             },
             "edges": {
                 "df87ff82": {
                     "subject": "MONDO:0005148",
                     "predicate": "biolink:treated_by",
                     "object": "ncats.drug:9100L32L2N",
-                    "sources": [
-                        {
-                            "resource_id": "infores:chebi",
-                            "resource_role": "primary_knowledge_source",
-                            "upstream_resource_ids": []
-                        },
-                        {
-                            "resource_id": "infores:biothings-explorer",
-                            "resource_role": "aggregator_knowledge_source",
-                            "upstream_resource_ids": [
-                                "infores:chebi"
-                            ]
-                        },
-                        {
-                            "resource_id": "infores:molepro",
-                            "resource_role": "aggregator_knowledge_source",
-                            "upstream_resource_ids": [
-                                "infores:biothings-explorer"
-                            ]
-                        },
-                        {
-                            "resource_id": "infores:arax",
-                            "resource_role": "aggregator_knowledge_source",
-                            "upstream_resource_ids": [
-                                "infores:molepro"
-                            ]
-                        }
-                    ]
+                    "sources": _TEST_KG_EDGE_SOURCES
                 }
             }
         },
         "auxiliary_graphs": {
             "a0": {
                 "edges": [
                     "e02",
@@ -471,15 +446,15 @@
     kg_sample: Dict = validator.sample_graph(graph=TEST_GRAPH, edges_limit=edges_limit)
     assert kg_sample
     assert len(kg_sample["nodes"]) == number_of_nodes_returned
     assert len(kg_sample["edges"]) == number_of_edges_returned
 
 
 @pytest.mark.parametrize(
-    "response,trapi_version,biolink_version,target_provenance,strict_validation,message",
+    "response,trapi_version,biolink_version,target_provenance,strict_validation,code",
     [
         (   # Query 0 - Completely empty Response.Message
             {
                 "message": {
 
                 }
             },
@@ -498,30 +473,30 @@
                 }
             },
             TRAPI_1_3_0,
             None,
             None,
             False,
             # "Validate TRAPI Response: ERROR - TRAPI Message is missing its Query Graph!"
-            "error.trapi.response.query_graph.missing"
+            "error.trapi.response.message.query_graph.missing"
         ),
         (   # Query 2 - Response.Message also devoid of content, null QGraph trapped first....
             {
                 "message": {
                     "query_graph": None,
                     "knowledge_graph": None,
                     "results": None
                 }
             },
             TRAPI_1_3_0,
             None,
             None,
             False,
             # "Validate TRAPI Response: ERROR - Response returned a null or empty Message Query Graph!"
-            "error.trapi.response.query_graph.empty"
+            "error.trapi.response.message.query_graph.empty"
         ),
         (
             # Query 3 - Partly empty Response.Message with a modest but
             #           workable query graph? Missing KG trapped next?
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
@@ -530,15 +505,15 @@
                 }
             },
             TRAPI_1_3_0,
             None,
             None,
             False,
             # "Validate TRAPI Response: ERROR - TRAPI Message is missing its Knowledge Graph component?"
-            "error.trapi.response.knowledge_graph.missing"
+            "error.trapi.response.message.knowledge_graph.missing"
         ),
         (
             # Query 4 - Partly empty Response.Message with a modest
             #           but workable query graph? Empty KG trapped next?
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
@@ -547,15 +522,15 @@
                 }
             },
             TRAPI_1_3_0,
             None,
             None,
             False,
             # "Validate TRAPI Response: WARNING - Response returned an empty Message Knowledge Graph?"
-            "warning.trapi.response.knowledge_graph.empty"
+            "warning.trapi.response.message.knowledge_graph.empty"
         ),
         (
             # Query 5 - Partly empty Response.Message with a modest but workable
             #           query and knowledge graphs? Missing Results detected next?
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
@@ -564,15 +539,15 @@
                 }
             },
             TRAPI_1_3_0,
             None,
             None,
             False,
             # "Validate TRAPI Response: ERROR - TRAPI Message is missing its Results component!"
-            "error.trapi.response.results.missing"
+            "error.trapi.response.message.results.missing"
         ),
         (
             # Query 6 - Partly empty Response.Message with a modest but workable query and
             #           knowledge graphs? Null valued Results detected next - just issue a warning?
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
@@ -581,15 +556,15 @@
                 }
             },
             TRAPI_1_3_0,
             None,
             None,
             False,
             # "Validate TRAPI Response: WARNING -Response returned empty Message.results?"
-            "warning.trapi.response.results.empty"
+            "warning.trapi.response.message.results.empty"
         ),
         (
             # Query 7 - Partly empty Response.Message with a modest but workable
             #           query and knowledge graphs? Non-array Results detected next?
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
@@ -598,15 +573,15 @@
                 }
             },
             TRAPI_1_3_0,
             None,
             None,
             False,
             # "Validate TRAPI Response: ERROR - Response returned a non-array Message.Results!
-            "error.trapi.response.results.not_array"
+            "error.trapi.response.message.results.not_array"
         ),
         (
             # Query 8 - Partly empty Response.Message with a modest but workable query and
             #           knowledge graphs? Empty Results detected next - just issue a warning?
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
@@ -615,15 +590,15 @@
                 }
             },
             TRAPI_1_3_0,
             None,
             None,
             False,
             # "Validate TRAPI Response: ERROR - Response returned empty Message.results?"
-            "warning.trapi.response.results.empty"
+            "warning.trapi.response.message.results.empty"
         ),
         (
             # Query 9 - Full Message, without "sources" and "strict_validation": False - should pass?
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
@@ -1020,24 +995,24 @@
 )
 def test_check_biolink_model_compliance_of_trapi_response(
         response: Dict,
         trapi_version: str,
         biolink_version: str,
         target_provenance: Dict,
         strict_validation: bool,
-        message: str
+        code
 ):
     validator: TRAPIResponseValidator = TRAPIResponseValidator(
         trapi_version=trapi_version,
         biolink_version=biolink_version,
         strict_validation=strict_validation,
         target_provenance=target_provenance
     )
     validator.check_compliance_of_trapi_response(response=response)
-    check_messages(validator, message, no_errors=True)
+    check_messages(validator, code, no_errors=True)
 
 
 @pytest.mark.parametrize(
     "response,trapi_version,biolink_version,sources,strict_validation,code",
     [
         (   # Query 0 - Completely empty Response.Message
             {
@@ -1220,7 +1195,264 @@
     ]
 )
 def test_dump_report_of_biolink_model_compliance_of_trapi_response_with_errors(response: Dict):
     validator: TRAPIResponseValidator = TRAPIResponseValidator()
     validator.check_compliance_of_trapi_response(response=response)
     validator.dump(file=stderr)
     print("\n"+"="*80+"\n", file=stderr)
+
+
+@pytest.mark.parametrize(
+    "case,response",
+    [
+        (dict(), {"empty": "nonsense"}),
+        ({"empty": "nonsense"}, dict()),
+    ]
+)
+def test_empty_case_input_found_in_response(case, response):
+    validator = TRAPIResponseValidator()
+    with pytest.raises(AssertionError):
+        validator.case_input_found_in_response(case, response)
+
+
+#
+# case: Dict parameter contains something like:
+#
+SAMPLE_TEST_CASE = {
+    "idx": 0,
+    "subject_id": "MONDO:0005148",
+    "subject_category": "biolink:Disease",
+    "predicate_id": 'biolink:treated_by',
+    "object_id": "ncats.drug:9100L32L2N",
+    "object_category": "biolink:Drug"
+}
+#
+# the contents for which ought to be returned in
+# the TRAPI Knowledge Graph, with a Result mapping?
+#
+SAMPLE_QUERY_GRAPH = {
+    "nodes": {
+        "type-2 diabetes": {
+            "ids": ["diabetes"]
+        },
+        "drug": {
+            "categories": ["biolink:Drug"]
+        }
+    },
+    "edges": {
+        "treated_by": {
+            "subject": "type-2 diabetes",
+            "predicates": ["biolink:treated_by"],
+            "object": "drug"
+        }
+    }
+}
+
+SAMPLE_TEST_NODES = {
+    "MONDO:0005148": {"name": "type-2 diabetes", "categories": ["biolink:Disease"]},
+    "ncats.drug:9100L32L2N": {"name": "metformin", "categories": ["biolink:Drug"]}
+}
+
+SAMPLE_TEST_EDGES = {
+    "df879999": {
+        "subject": "MONDO:0005148",
+        "predicate": "biolink:treated_by",
+        "object": "ncats.drug:9100L32L2N"
+    }
+}
+SAMPLE_TEST_GRAPH = {
+    "nodes": SAMPLE_TEST_NODES,
+    "edges": SAMPLE_TEST_EDGES
+}
+
+SAMPLE_TEST_RESULTS = [
+    {
+        "node_bindings": {
+            "type-2 diabetes": [{"id": "MONDO:0005148"}],
+            "drug": [{"id": "ncats.drug:9100L32L2N"}]
+        },
+        "edge_bindings": {
+            "treated_by": [{"id": "df879999"}]
+        }
+    }
+]
+
+SAMPLE_TEST_INCOMPLETE_RESULTS = [
+    {
+        "node_bindings": {
+            "type-2 diabetes": [{"id": "MONDO:0005148"}],
+            "drug": [{"id": "ncats.drug:9100L32L2N"}]
+        },
+        "analyses": [
+            {
+                "resource_id": "infores:ara0",
+                # not pointing to an edge in the existing sample KG
+                "edge_bindings": {"treated_by": [{"id": "abcde999"}]},
+                "support_graphs": [],
+                "score": 0.7
+            }
+        ]
+    }
+]
+
+
+@pytest.mark.parametrize(
+    "case,response,code",
+    [
+        (   # Query 0 - missing message 'knowledge_graph' property key
+            SAMPLE_TEST_CASE,
+            {
+                "message": {
+                    "query_graph": SAMPLE_QUERY_GRAPH,
+                    "results": SAMPLE_TEST_RESULTS
+                }
+            },
+            "error.trapi.response.message.knowledge_graph.missing"
+        ),
+        (  # Query 1 - empty message 'knowledge_graph' value
+                SAMPLE_TEST_CASE,
+                {
+                    "message": {
+                        "query_graph": SAMPLE_QUERY_GRAPH,
+                        "knowledge_graph": {},
+                        "results": SAMPLE_TEST_RESULTS
+                    }
+                },
+                "error.trapi.response.message.knowledge_graph.empty"
+        ),
+        (   # Query 2 - missing message 'results' property key
+            SAMPLE_TEST_CASE,
+            {
+                "message": {
+                    "query_graph": SAMPLE_QUERY_GRAPH,
+                    "knowledge_graph": {"nodes": {}, "edges": {}}
+                }
+            },
+            "error.trapi.response.message.results.missing"
+        ),
+        (   # Query 3 - empty message 'results' property value
+            SAMPLE_TEST_CASE,
+            {
+                "message": {
+                    "query_graph": SAMPLE_QUERY_GRAPH,
+                    "knowledge_graph": {"nodes": {}, "edges": {}},
+                    "results": []
+                }
+            },
+            "error.trapi.response.message.results.empty"
+        ),
+        (   # Query 4 - missing message subject node
+            SAMPLE_TEST_CASE,
+            {
+                "message": {
+                    "query_graph": SAMPLE_QUERY_GRAPH,
+                    "knowledge_graph": {
+                        "nodes": {
+                            # "MONDO:0005148": {"name": "type-2 diabetes", "categories": ["biolink:Disease"]},
+                            "ncats.drug:9100L32L2N": {"name": "metformin", "categories": ["biolink:Drug"]}
+                        },
+                        "edges": {
+                            "df87ff82": {
+                                "subject": "CHEBI:3002",
+                                "predicate": "biolink:treated_by",
+                                "object": "MESH:D001249"
+                            }
+                        }
+                    },
+                    "results": SAMPLE_TEST_RESULTS
+                }
+            },
+            "error.trapi.response.message.knowledge_graph.node.missing"
+        ),
+        (   # Query 5 - the test case 'subject' node category is not an exact match against
+            #           the knowledge graph edge category; however, the test case has a
+            #           parent category which does match the knowledge graph, so we let it pass!
+            SAMPLE_TEST_CASE,
+            {
+                "message": {
+                    "query_graph": SAMPLE_QUERY_GRAPH,
+                    "knowledge_graph": {
+                        "nodes": {
+                            "MONDO:0005148": {
+                                "name": "type-2 diabetes",
+                                "categories": [
+                                    "biolink:DiseaseOrPhenotypicFeature"
+                                ]
+                            },
+                            "ncats.drug:9100L32L2N": {
+                                "name": "metformin",
+                                "categories": [
+                                    "biolink:Drug"
+                                ]
+                            }
+                        },
+                        "edges": {
+                            "df87ff82": {
+                                "subject": "CHEBI:3002",
+                                "predicate": "biolink:treated_by",
+                                "object": "MESH:D001249"
+                            }
+                        }
+                    },
+                    "results": SAMPLE_TEST_RESULTS
+                }
+            },
+            # NOT "error.trapi.response.message.knowledge_graph.node.missing"
+            ""
+        ),
+        (   # Query 6 - missing message object node
+            SAMPLE_TEST_CASE,
+            {
+                "message": {
+                    "query_graph": SAMPLE_QUERY_GRAPH,
+                    "knowledge_graph": {
+                        "nodes": {
+                            "MONDO:0005148": {"name": "type-2 diabetes", "categories": ["biolink:Disease"]},
+                            # "ncats.drug:9100L32L2N": {"name": "metformin", "categories": ["biolink:Drug"]}
+                        },
+                        "edges": {
+                            "df87ff82": {
+                                "subject": "CHEBI:3002",
+                                "predicate": "biolink:treated_by",
+                                "object": "MESH:D001249"
+                            }
+                        }
+                    },
+                    "results": SAMPLE_TEST_RESULTS
+                }
+            },
+            "error.trapi.response.message.knowledge_graph.node.missing"
+        ),
+        (   # Query 7 - missing message edge
+            SAMPLE_TEST_CASE,
+            {
+                "message": {
+                    "query_graph": SAMPLE_QUERY_GRAPH,
+                    "knowledge_graph": {
+                        "nodes": {
+                            "MONDO:0005148": {"name": "type-2 diabetes", "categories": ["biolink:Disease"]},
+                            "ncats.drug:9100L32L2N": {"name": "metformin", "categories": ["biolink:Drug"]}
+                        },
+                        "edges": {}
+                    },
+                    "results": SAMPLE_TEST_RESULTS
+                }
+            },
+            "error.trapi.response.message.knowledge_graph.edge.missing"
+        ),
+        (   # Query 8 -  missing specific result in messages results matching input values
+            SAMPLE_TEST_CASE,
+            {
+                "message": {
+                    "query_graph": SAMPLE_QUERY_GRAPH,
+                    "knowledge_graph": SAMPLE_TEST_GRAPH,
+                    "results": SAMPLE_TEST_INCOMPLETE_RESULTS
+                }
+            },
+            "error.trapi.response.message.result.missing"
+        )
+    ]
+)
+def test_case_input_found_in_response(case, response, code):
+    validator = TRAPIResponseValidator()
+    assert not validator.case_input_found_in_response(case, response) if code else True
+    check_messages(validator, code)
```

### Comparing `reasoner_validator-4.1.3/tests/test_semver.py` & `reasoner_validator-4.1.4/tests/test_semver.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.3/tests/test_trapi_versioning.py` & `reasoner_validator-4.1.4/tests/test_trapi_versioning.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 
 def test_load_schema_with_semver_trapi_version():
     trapi_version: str = get_latest_version(release_tag="1")
     schema: Dict = load_schema(trapi_version)
     assert schema
 
 
+@pytest.mark.skip("May 9, 2024 master branch of ReasonerAPI has a schema bug which crashes this test")
 def test_load_schema_with_branch_name_as_trapi_version():
     trapi_version: str = get_latest_version(release_tag="master")
     schema: Dict = load_schema(trapi_version)
     assert schema
     with pytest.raises(ValueError):
         load_schema(target="not-a-branch-name")
```

### Comparing `reasoner_validator-4.1.3/tests/test_validate.py` & `reasoner_validator-4.1.4/tests/test_validate.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,14 +91,15 @@
 @pytest.mark.parametrize("trapi_version", ALL_TEST_VERSIONS)
 def test_load_schema(trapi_version: str):
     """Test load_schema(trapi_version)."""
     schema = load_schema(trapi_version)
     assert schema, f"TRAPI Schema for release '{trapi_version}' is not available?"
 
 
+@pytest.mark.skip("May 9, 2024 master branch of ReasonerAPI has a schema bug which crashes this test")
 def test_load_master_schema():
     """Test load_schema('master')."""
     schema = load_schema("master")
     assert schema, "TRAPI Schema for ('master') branch is not available?"
 
 
 def test_message():
@@ -140,15 +141,15 @@
     }, "EdgeBinding")
     with pytest.raises(ValidationError):
         validator.validate({
             "foo": {},
         }, "EdgeBinding")
 
 
-@pytest.mark.skip("Test inputs are not yet TRAPI 1.5 compliant")
+@pytest.mark.skip(reason="Not updated to work correctly with TRAPI 1.5.0")
 @pytest.mark.parametrize("trapi_version", LATEST_TEST_RELEASES)
 def test_trapi_1_5_edgebinding(trapi_version: str):
     """Test TRAPIValidator(trapi_version=query).validate_EdgeBinding()."""
     validator = TRAPISchemaValidator(trapi_version=trapi_version)
     validator.validate({
         "id": "hello",
     }, "EdgeBinding")
@@ -319,15 +320,15 @@
                     "allowlist": []
                 }
             }
         ]
         validator.validate(faulty_query_wf, "Query")
 
 
-@pytest.mark.skip("Test inputs are not yet TRAPI 1.5 compliant")
+@pytest.mark.skip(reason="Not updated to work correctly with TRAPI 1.5.0")
 @pytest.mark.parametrize("trapi_version", LATEST_TEST_RELEASES)
 def test_1_5_query_latest_trapi_workflow_properties(trapi_version: str):
     """Test flawed TRAPI Query workflow properties."""
     validator = TRAPISchemaValidator(trapi_version=trapi_version)
     query = deepcopy(SAMPLE_QUERY)
     query["workflow"] = SAMPLE_WORKFLOW_1_3_4
     validator.validate(query, "Query")
@@ -588,15 +589,15 @@
         validator.validate({
             # missing required: node_bindings, edge_bindings
             "foo": {},
             "bar": {},
         }, "Result")
 
 
-@pytest.mark.skip("Test inputs are not yet TRAPI 1.5 compliant")
+@pytest.mark.skip(reason="Not updated to work correctly with TRAPI 1.5.0")
 @pytest.mark.parametrize("trapi_version", LATEST_TEST_RELEASES)
 def test_latest_trapi_message_results_component_validation(trapi_version: str):
     """Test Message.Results component in TRAPIValidator(trapi_version=query).validate()."""
     #     Result:
     #       type: object
     #       description: >-
     #         A Result object specifies the nodes and edges in the knowledge graph
@@ -754,15 +755,16 @@
     with pytest.raises(ValidationError):
         validator.validate({
             # missing required: id
             "foo": {},
             "bar": {},
         }, "NodeBinding")
 
-@pytest.mark.skip("Test inputs are not yet TRAPI 1.5 compliant")
+
+@pytest.mark.skip(reason="Not updated to work correctly with TRAPI 1.5.0")
 @pytest.mark.parametrize("trapi_version", LATEST_TEST_RELEASES)
 def test_latest_trapi_message_node_binding_component_validation(trapi_version: str):
     """Test NodeBinding component in TRAPIValidator(trapi_version=query).validate()."""
     validator = TRAPISchemaValidator(trapi_version=trapi_version)
     sample_node_binding = {
         "id": "SGD:S000000065",
         # 'qnode_id' is not formally specified in spec, but it is an
```

### Comparing `reasoner_validator-4.1.3/tests/test_validation_report.py` & `reasoner_validator-4.1.4/tests/test_validation_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -643,21 +643,21 @@
         default_target="2nd Test Message Set"
     )
     reporter2.report(
         code="info.query_graph.edge.predicate.mixin",
         identifier="biolink:this_is_a_mixin",
         edge_id="a-biolink:this_is_a_mixin->b"
     )
-    reporter2.report("warning.trapi.response.results.empty")
+    reporter2.report("warning.trapi.response.message.results.empty")
     reporter2.report("error.knowledge_graph.edges.empty")
     reporter1.merge(reporter2)
 
     # No prefix...
     reporter3 = ValidationReporter()
-    reporter3.report("error.trapi.response.query_graph.missing")
+    reporter3.report("error.trapi.response.message.query_graph.missing")
     reporter1.merge(reporter3)
 
     # testing addition a few raw batch messages
     reporter1.add_messages(full_test_messages_by_target)
 
     # Verify what we have
     test_message_type: MessageType
```

### Comparing `reasoner_validator-4.1.3/tests/test_workflows.py` & `reasoner_validator-4.1.4/tests/test_workflows.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     validator = TRAPISchemaValidator(trapi_version=trapi_version)
     validator.validate(query, "Query")
 
 
 TRAPI_LATEST_TRAPI_QUERY_VERSION = [qv for qv in product(LATEST_TEST_RELEASES, (SAMPLE_QUERY_1, SAMPLE_QUERY_2))]
 
 
-@pytest.mark.skip("Test inputs are not yet TRAPI 1.5 compliant")
+@pytest.mark.skip(reason="Not updated to work correctly with TRAPI 1.5.0")
 @pytest.mark.parametrize("trapi_version,query", TRAPI_LATEST_TRAPI_QUERY_VERSION)
 def test_query_latest_trapi_workflow_properties(trapi_version: str, query: Dict):
     """Test flawed TRAPI Query workflow properties."""
 
     print(f"\nTRAPI release: '{trapi_version}'")
     print(f"Test Workflow: '{dumps(query['workflow'], indent=2)}'")
```

### Comparing `reasoner_validator-4.1.3/PKG-INFO` & `reasoner_validator-4.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-validator
-Version: 4.1.3
+Version: 4.1.4
 Summary: Validation tools for Reasoner API
 Home-page: https://github.com/NCATSTranslator
 License: MIT
 Keywords: NCATS,Biomedical Data Translator,Translator,ReasonerAPI,TRAPI,validation,Biolink Model
 Author: Richard Bruskiewich
 Author-email: richard.bruskiewich@delphinai.com
 Maintainer: Richard Bruskiewich
```

