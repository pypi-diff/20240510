# Comparing `tmp/graph_validation_test_runners-0.0.12.tar.gz` & `tmp/graph_validation_test_runners-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graph_validation_test_runners-0.0.12.tar", max compression
+gzip compressed data, was "graph_validation_test_runners-0.1.1.tar", max compression
```

## Comparing `graph_validation_test_runners-0.0.12.tar` & `graph_validation_test_runners-0.1.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1070 2024-05-07 05:22:12.493355 graph_validation_test_runners-0.0.12/LICENSE
--rw-r--r--   0        0        0    11160 2024-05-07 05:22:12.493355 graph_validation_test_runners-0.0.12/README.md
--rw-r--r--   0        0        0    30149 2024-05-07 05:22:12.493355 graph_validation_test_runners-0.0.12/graph_validation_tests/__init__.py
--rw-r--r--   0        0        0        0 2024-05-07 05:22:12.493355 graph_validation_test_runners-0.0.12/graph_validation_tests/translator/__init__.py
--rw-r--r--   0        0        0    36673 2024-05-07 05:22:12.493355 graph_validation_test_runners-0.0.12/graph_validation_tests/translator/registry/__init__.py
--rw-r--r--   0        0        0    10859 2024-05-07 05:22:12.493355 graph_validation_test_runners-0.0.12/graph_validation_tests/translator/trapi/__init__.py
--rw-r--r--   0        0        0        0 2024-05-07 05:22:12.493355 graph_validation_test_runners-0.0.12/graph_validation_tests/utils/__init__.py
--rw-r--r--   0        0        0      722 2024-05-07 05:22:12.493355 graph_validation_test_runners-0.0.12/graph_validation_tests/utils/asyncio.py
--rw-r--r--   0        0        0      113 2024-05-07 05:22:12.493355 graph_validation_test_runners-0.0.12/graph_validation_tests/utils/constants.py
--rw-r--r--   0        0        0      886 2024-05-07 05:22:12.493355 graph_validation_test_runners-0.0.12/graph_validation_tests/utils/http.py
--rw-r--r--   0        0        0     4268 2024-05-07 05:22:12.493355 graph_validation_test_runners-0.0.12/graph_validation_tests/utils/ontology_kp.py
--rw-r--r--   0        0        0    19691 2024-05-07 05:22:12.493355 graph_validation_test_runners-0.0.12/graph_validation_tests/utils/unit_test_templates.py
--rw-r--r--   0        0        0     8962 2024-05-07 05:22:12.493355 graph_validation_test_runners-0.0.12/one_hop_test_runner/__init__.py
--rw-r--r--   0        0        0     3029 2024-05-07 05:22:24.785319 graph_validation_test_runners-0.0.12/pyproject.toml
--rw-r--r--   0        0        0     4854 2024-05-07 05:22:12.497355 graph_validation_test_runners-0.0.12/standards_validation_test_runner/__init__.py
--rw-r--r--   0        0        0     1292 2024-05-07 05:22:12.497355 graph_validation_test_runners-0.0.12/tests/__init__.py
--rw-r--r--   0        0        0    18034 2024-05-07 05:22:12.497355 graph_validation_test_runners-0.0.12/tests/graph_validation_test/translator/test_translator_smartapi_registry.py
--rw-r--r--   0        0        0     4893 2024-05-07 05:22:12.497355 graph_validation_test_runners-0.0.12/tests/graph_validation_test/translator/trapi/test_trapi.py
--rw-r--r--   0        0        0        0 2024-05-07 05:22:12.497355 graph_validation_test_runners-0.0.12/tests/graph_validation_test_runner/__init__.py
--rw-r--r--   0        0        0     4776 2024-05-07 05:22:12.497355 graph_validation_test_runners-0.0.12/tests/graph_validation_test_runner/test_graph_validation_test.py
--rw-r--r--   0        0        0     5765 2024-05-07 05:22:12.497355 graph_validation_test_runners-0.0.12/tests/graph_validation_test_runner/test_unit_test_templates.py
--rw-r--r--   0        0        0        0 2024-05-07 05:22:12.497355 graph_validation_test_runners-0.0.12/tests/graph_validation_test_runner/translator/__init__.py
--rw-r--r--   0        0        0        0 2024-05-07 05:22:12.497355 graph_validation_test_runners-0.0.12/tests/graph_validation_test_runner/translator/biolink/__init__.py
--rw-r--r--   0        0        0     1066 2024-05-07 05:22:12.497355 graph_validation_test_runners-0.0.12/tests/graph_validation_test_runner/translator/biolink/test_ontology_kp.py
--rw-r--r--   0        0        0    18032 2024-05-07 05:22:12.497355 graph_validation_test_runners-0.0.12/tests/graph_validation_test_runner/translator/test_translator_smartapi_registry.py
--rw-r--r--   0        0        0        0 2024-05-07 05:22:12.497355 graph_validation_test_runners-0.0.12/tests/graph_validation_test_runner/translator/trapi/__init__.py
--rw-r--r--   0        0        0     4891 2024-05-07 05:22:12.497355 graph_validation_test_runners-0.0.12/tests/graph_validation_test_runner/translator/trapi/test_trapi.py
--rw-r--r--   0        0        0        0 2024-05-07 05:22:12.497355 graph_validation_test_runners-0.0.12/tests/one_hop_test_runner/__init__.py
--rw-r--r--   0        0        0     3029 2024-05-07 05:22:12.497355 graph_validation_test_runners-0.0.12/tests/one_hop_test_runner/test_one_hop_test.py
--rw-r--r--   0        0        0       70 2024-05-07 05:22:12.497355 graph_validation_test_runners-0.0.12/tests/scripts/one_hop_test.cmd
--rw-r--r--   0        0        0        0 2024-05-07 05:22:12.497355 graph_validation_test_runners-0.0.12/tests/standards_validation_test_runner/__init__.py
--rw-r--r--   0        0        0     1482 2024-05-07 05:22:12.497355 graph_validation_test_runners-0.0.12/tests/standards_validation_test_runner/test_standards_validation_test.py
--rw-r--r--   0        0        0    13091 1970-01-01 00:00:00.000000 graph_validation_test_runners-0.0.12/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-10 04:20:39.176122 graph_validation_test_runners-0.1.1/LICENSE
+-rw-r--r--   0        0        0    11042 2024-05-10 04:20:39.176122 graph_validation_test_runners-0.1.1/README.md
+-rw-r--r--   0        0        0    30224 2024-05-10 04:20:39.176122 graph_validation_test_runners-0.1.1/graph_validation_tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 04:20:39.176122 graph_validation_test_runners-0.1.1/graph_validation_tests/translator/__init__.py
+-rw-r--r--   0        0        0    36673 2024-05-10 04:20:39.176122 graph_validation_test_runners-0.1.1/graph_validation_tests/translator/registry/__init__.py
+-rw-r--r--   0        0        0    10817 2024-05-10 04:20:39.180122 graph_validation_test_runners-0.1.1/graph_validation_tests/translator/trapi/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 04:20:39.180122 graph_validation_test_runners-0.1.1/graph_validation_tests/utils/__init__.py
+-rw-r--r--   0        0        0      722 2024-05-10 04:20:39.180122 graph_validation_test_runners-0.1.1/graph_validation_tests/utils/asyncio.py
+-rw-r--r--   0        0        0      113 2024-05-10 04:20:39.180122 graph_validation_test_runners-0.1.1/graph_validation_tests/utils/constants.py
+-rw-r--r--   0        0        0      886 2024-05-10 04:20:39.180122 graph_validation_test_runners-0.1.1/graph_validation_tests/utils/http.py
+-rw-r--r--   0        0        0     4268 2024-05-10 04:20:39.180122 graph_validation_test_runners-0.1.1/graph_validation_tests/utils/ontology_kp.py
+-rw-r--r--   0        0        0    19691 2024-05-10 04:20:39.180122 graph_validation_test_runners-0.1.1/graph_validation_tests/utils/unit_test_templates.py
+-rw-r--r--   0        0        0     7857 2024-05-10 04:20:39.180122 graph_validation_test_runners-0.1.1/one_hop_test_runner/__init__.py
+-rw-r--r--   0        0        0     2610 2024-05-10 04:20:51.180182 graph_validation_test_runners-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4526 2024-05-10 04:20:39.180122 graph_validation_test_runners-0.1.1/standards_validation_test_runner/__init__.py
+-rw-r--r--   0        0        0     1933 2024-05-10 04:20:39.180122 graph_validation_test_runners-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0    18172 2024-05-10 04:20:39.180122 graph_validation_test_runners-0.1.1/tests/graph_validation_test/translator/test_translator_smartapi_registry.py
+-rw-r--r--   0        0        0     4960 2024-05-10 04:20:39.180122 graph_validation_test_runners-0.1.1/tests/graph_validation_test/translator/trapi/test_trapi.py
+-rw-r--r--   0        0        0        0 2024-05-10 04:20:39.180122 graph_validation_test_runners-0.1.1/tests/graph_validation_test_runner/__init__.py
+-rw-r--r--   0        0        0     4776 2024-05-10 04:20:39.180122 graph_validation_test_runners-0.1.1/tests/graph_validation_test_runner/test_graph_validation_test.py
+-rw-r--r--   0        0        0     5765 2024-05-10 04:20:39.180122 graph_validation_test_runners-0.1.1/tests/graph_validation_test_runner/test_unit_test_templates.py
+-rw-r--r--   0        0        0        0 2024-05-10 04:20:39.180122 graph_validation_test_runners-0.1.1/tests/graph_validation_test_runner/translator/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 04:20:39.180122 graph_validation_test_runners-0.1.1/tests/graph_validation_test_runner/translator/biolink/__init__.py
+-rw-r--r--   0        0        0     1066 2024-05-10 04:20:39.180122 graph_validation_test_runners-0.1.1/tests/graph_validation_test_runner/translator/biolink/test_ontology_kp.py
+-rw-r--r--   0        0        0    18172 2024-05-10 04:20:39.180122 graph_validation_test_runners-0.1.1/tests/graph_validation_test_runner/translator/test_translator_smartapi_registry.py
+-rw-r--r--   0        0        0        0 2024-05-10 04:20:39.180122 graph_validation_test_runners-0.1.1/tests/graph_validation_test_runner/translator/trapi/__init__.py
+-rw-r--r--   0        0        0     5028 2024-05-10 04:20:39.180122 graph_validation_test_runners-0.1.1/tests/graph_validation_test_runner/translator/trapi/test_trapi.py
+-rw-r--r--   0        0        0        0 2024-05-10 04:20:39.180122 graph_validation_test_runners-0.1.1/tests/one_hop_test_runner/__init__.py
+-rw-r--r--   0        0        0     3770 2024-05-10 04:20:39.184122 graph_validation_test_runners-0.1.1/tests/one_hop_test_runner/test_one_hop_test.py
+-rw-r--r--   0        0        0       70 2024-05-10 04:20:39.184122 graph_validation_test_runners-0.1.1/tests/scripts/one_hop_test.cmd
+-rw-r--r--   0        0        0        0 2024-05-10 04:20:39.184122 graph_validation_test_runners-0.1.1/tests/standards_validation_test_runner/__init__.py
+-rw-r--r--   0        0        0     2573 2024-05-10 04:20:39.184122 graph_validation_test_runners-0.1.1/tests/standards_validation_test_runner/test_standards_validation_test.py
+-rw-r--r--   0        0        0    12921 1970-01-01 00:00:00.000000 graph_validation_test_runners-0.1.1/PKG-INFO
```

### Comparing `graph_validation_test_runners-0.0.12/LICENSE` & `graph_validation_test_runners-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `graph_validation_test_runners-0.0.12/README.md` & `graph_validation_test_runners-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Graph Validation Tests
 
-[![Pyversions](https://img.shields.io/pypi/pyversions/graph-validation-test-runners)](https://pypi.python.org/pypi/graph-validation-test-runners)
-[![Publish Python Package](https://github.com/TranslatorSRI/graph-validation-test-runners/actions/workflows/python-publish.yml/badge.svg)](https://pypi.org/project/graph-validation-test-runners/)
+![Pyversions](https://img.shields.io/pypi/pyversions/graph-validation-test-runners)
+[![PyPI - Version](https://img.shields.io/pypi/v/graph-validation-test-runners)](https://pypi.python.org/pypi/graph-validation-test-runners)
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
 [![Run tests](https://github.com/TranslatorSRI/graph-validation-test-runners/actions/workflows/test.yml/badge.svg)](https://github.com/TranslatorSRI/graph-validation-test-runners/actions/workflows/test.yml)
 
 
 This repository provides the implementation of Translator knowledge graph validation test runners within the new 2023 Testing Infrastructure.  The current package currently contains two such test runners:
 
 - **StandardsValidationTest:** is a wrapper of the [Translator reasoner-validator package](https://github.com/NCATSTranslator/reasoner-validator) which certifies that knowledge graph data access is TRAPI compliant and the graph semantic content is Biolink Model compliant.
@@ -17,15 +17,15 @@
 
 The **standards_validation_test_runner** and **one_hop_test_runner* may be run directly from the command line or programmatically, from within a Python script.
 
 ### Installation
 
 The **graph-validation-test-runners** module can be installed from pypi and used as part of the Translator-wide automated testing.
 
-_Note: Requires 3.9 <= Python release <= 3.12_
+_Note: Requires 3.9 <= Python release < 3.12_
 
 #### From Pypi
 
 From within your target working directory:
 
 - Create a python virtual environment: `python -m venv venv`
 - Activate your environment: `. ./venv/bin/activate`
```

### Comparing `graph_validation_test_runners-0.0.12/graph_validation_tests/__init__.py` & `graph_validation_test_runners-0.1.1/graph_validation_tests/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,29 +2,30 @@
 Abstract base class for the GraphValidation TestRunners
 """
 from typing import Dict, List, Optional, Tuple
 
 from argparse import ArgumentParser
 
 from reasoner_validator.biolink import BiolinkValidator
+from reasoner_validator.validator import TRAPIResponseValidator
 from reasoner_validator.message import MESSAGES_BY_TARGET, MESSAGE_CATALOG, MESSAGES_BY_TEST
 from translator_testing_model.datamodel.pydanticmodel import TestAsset, TestCaseResultEnum
 
 from graph_validation_tests.translator.registry import (
     get_the_registry_data,
     extract_component_test_metadata_from_registry
 )
 from graph_validation_tests.translator.trapi import get_available_components
 from graph_validation_tests.utils.asyncio import gather
 
 import logging
 logger = logging.getLogger(__name__)
 
 
-class TestCaseRun(BiolinkValidator):
+class TestCaseRun(TRAPIResponseValidator):
     """
     TestCaseRun is a wrapper for BiolinkValidator, used to aggregate
     validation messages from the GraphValidationTest processing of a specific
     TestCase, derived from the TestAsset - bound to the 'test_run' - which is
     based on a TRAPI query against the test_run bound 'target' endpoint. Results
     of a TestCaseRun are stored within the parent BiolinkValidator class.
     """
@@ -36,15 +37,15 @@
         :param test: declared generator of a TestCase TRAPI query being processed (generally, an executable function).
         :param kwargs: Dict, optional extra named BiolinkValidator parameters
                              which may be specified for the test run.
         """
         assert test_run, "'test_run' is uninitialized!"
         self.test_run = test_run
 
-        BiolinkValidator.__init__(
+        TRAPIResponseValidator.__init__(
             self,
             default_test=test.__name__,
             default_target=test_run.default_target,
             trapi_version=test_run.trapi_version,
             biolink_version=test_run.biolink_version,
             **kwargs
         )
@@ -194,27 +195,27 @@
             biolink_version=biolink_version,
             **kwargs
         )
         self.environment: str = environment
         self.test_asset: TestAsset = test_asset
 
         # trapi_generators should usually not be empty, but just in case...
-        self.trapi_generators: List = trapi_generators or []
+        self.trapi_generators: Tuple = trapi_generators or ()
 
         self.runner_settings = runner_settings
 
         self.results: Dict = dict()
 
     def get_run_id(self):
         # First implementation of 'run identifier' is
         # is to return the default target endpoint?
         # TODO: likely need a more appropriate run identifier here, e.g. ARS PK-like?
         return self.default_target
 
-    def get_trapi_generators(self) -> List:
+    def get_trapi_generators(self) -> Tuple:
         return self.trapi_generators
 
     def get_runner_settings(self) -> List[str]:
         return self.runner_settings.copy()
 
     @classmethod
     def build_test_asset(
@@ -368,15 +369,15 @@
         #         etc...
         #     }
         #     etc...
         # ]
         # where the 'test_asset_id_#' is something sensible, probably composite of the test asset identifier and
         # the identifier of the test template method used to generate the TestCase-specific TRAPI query.
         #
-        # The <result_#> value could minimally simply be be "PASSED" or "FAILED"; however, perhaps it ought to be
+        # The <result_#> value could minimally simply be "PASSED" or "FAILED"; however, perhaps it ought to be
         # a somewhat more complex informative data value for this TestRunner, accounting for the extensive validation
         # messages categories provided by reasoner-validator, i.e. 'info', 'skipped', 'warning', 'error', 'critical'.
         #
         # How should these messages be binned into test PASSED or FAILED? Should “PASSED” only be tolerant of
         # “information” messages? Are “skipped test” messages indicative of a failed test?
         #
         # Are “Warnings” to also be taken as an indication of a test failure? Could/should we give TestRunner
```

### Comparing `graph_validation_test_runners-0.0.12/graph_validation_tests/translator/registry/__init__.py` & `graph_validation_test_runners-0.1.1/graph_validation_tests/translator/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `graph_validation_test_runners-0.0.12/graph_validation_tests/translator/trapi/__init__.py` & `graph_validation_test_runners-0.1.1/graph_validation_tests/translator/trapi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -279,15 +279,14 @@
                           'ars', ARA acronym (e.g. 'arax') or KP acronym (e.g. 'molepro')
     :param environment: Optional[str] = None, Target Translator execution environment for the test,
                                               one of 'dev', 'ci', 'test' or 'prod' (default: 'ci')
     :param target_trapi_version: Optional[str], target TRAPI version (default: latest public release)
     :param target_biolink_version: Optional[str], target Biolink Model version (default: Biolink toolkit release)
     :return:  Dict, TRAPI response JSON, as a Python data structure.
     """
-    trapi_response: Optional[Dict] = None
     endpoint: str = resolve_component_endpoint(
         component=component,
         environment=environment,
         target_trapi_version=target_trapi_version,
         target_biolink_version=target_biolink_version
     )
     if not endpoint:
```

### Comparing `graph_validation_test_runners-0.0.12/graph_validation_tests/utils/asyncio.py` & `graph_validation_test_runners-0.1.1/graph_validation_tests/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `graph_validation_test_runners-0.0.12/graph_validation_tests/utils/http.py` & `graph_validation_test_runners-0.1.1/graph_validation_tests/utils/http.py`

 * *Files identical despite different names*

### Comparing `graph_validation_test_runners-0.0.12/graph_validation_tests/utils/ontology_kp.py` & `graph_validation_test_runners-0.1.1/graph_validation_tests/utils/ontology_kp.py`

 * *Files identical despite different names*

### Comparing `graph_validation_test_runners-0.0.12/graph_validation_tests/utils/unit_test_templates.py` & `graph_validation_test_runners-0.1.1/graph_validation_tests/utils/unit_test_templates.py`

 * *Files identical despite different names*

### Comparing `graph_validation_test_runners-0.0.12/one_hop_test_runner/__init__.py` & `graph_validation_test_runners-0.1.1/one_hop_test_runner/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -54,17 +54,15 @@
                 identifier=context[1],
                 context=context[0],
                 reason=output_node_binding
             )
 
         else:
             # sanity check: verify first that the TRAPI request is well-formed by the creator(case)
-            validator: TRAPISchemaValidator = TRAPISchemaValidator(trapi_version=self.trapi_version)
-            validator.validate(trapi_request, component="Query")
-            self.merge(validator)
+            self.validate(trapi_request, component="Query")
             if not self.has_messages():
 
                 # if no messages are reported, then continue with the validation
 
                 # TODO: this is SRI_Testing harness functionality which we don't yet support here?
                 #
                 # if 'ara_source' in _test_asset and _test_asset['ara_source']:
@@ -138,28 +136,15 @@
                             #     object_category: 'biolink:Disease',
                             #     predicate: 'biolink:treats',
                             #     subject_id: 'CHEBI:3002',  # may have the deprecated key 'subject' here
                             #     object_id: 'MESH:D001249', # may have the deprecated key 'object' here
                             #
                             # the contents for which ought to be returned in
                             # the TRAPI Knowledge Graph, as a Result mapping?
-                            #
-                            validator: TRAPIResponseValidator = TRAPIResponseValidator(
-                                trapi_version=self.trapi_version,
-                                biolink_version=self.biolink_version
-                            )
-                            if not validator.case_input_found_in_response(test_asset, response, self.trapi_version):
-                                test_edge_id: str = f"{test_asset['idx']}|" \
-                                                    f"({test_asset['subject_id']}#{test_asset['subject_category']})" + \
-                                                    f"-[{test_asset['predicate_id']}]->" + \
-                                                    f"({test_asset['object_id']}#{test_asset['object_category']})"
-                                self.report(
-                                    code="error.trapi.response.knowledge_graph.missing_expected_edge",
-                                    identifier=test_edge_id
-                                )
+                            self.case_input_found_in_response(test_asset, response)
                         else:
                             self.report(code="error.trapi.response.empty")
 
 
 class OneHopTest(GraphValidationTest):
     def test_case_wrapper(self, test, **kwargs) -> TestCaseRun:
         return OneHopTestCaseRun(test_run=self, test=test, **kwargs)
```

### Comparing `graph_validation_test_runners-0.0.12/pyproject.toml` & `graph_validation_test_runners-0.1.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "graph-validation-test-runners"
-version = "0.0.12"
+version = "0.1.1"
 description = "Validation of Translator Knowledge Graphs - TRAPI, Biolink Model and One Hop navigation"
 authors = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
     "Chris Bizon <bizon.renci.org>",
     "Tim Putnam <tim@tislab>"
 ]
 maintainers = ["Richard Bruskiewich <richard.bruskiewich@delphinai.com>"]
@@ -28,16 +28,15 @@
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Intended Audience :: Healthcare Industry",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3.12"
+    "Programming Language :: Python :: 3.11"
 ]
 
 packages = [
     {include = "graph_validation_tests"},
     {include = "one_hop_test_runner"},
     {include = "standards_validation_test_runner"}
 ]
@@ -45,28 +44,23 @@
 include = [
     { path = "tests" }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 deepdiff = "^6.7.1"
-
-#reasoner-validator = { git = "https://github.com/NCATSTranslator/reasoner-validator.git", branch = "graph-validation-test-revisions" }
-reasoner-validator = "^4.1.2"
-
-#translator-testing-model = { git = "https://github.com/TranslatorSRI/TranslatorTestingModel.git", rev = "ef5d68e" }
-#translator-testing-model = { git = "https://github.com/TranslatorSRI/TranslatorTestingModel.git", branch = "main" }
-translator-testing-model = "^0.3.1"
-
 fastapi = "*"
 httpx = "^0.27.0"
 tqdm = "^4.66.2"
 requests = "^2.31.0"
 matplotlib = "^3.8.3"
 
+reasoner-validator = "^4.1.4"
+translator-testing-model = "^0.3.1"
+
 [tool.poetry.group.dev.dependencies]
 setuptools = "^69.5.1"
 pytest = "^7.4.4"
 pytest-cov = "^4.1.0"
 pytest-asyncio = "^0.23.3"
 
 [tool.poetry.urls]
```

### Comparing `graph_validation_test_runners-0.0.12/standards_validation_test_runner/__init__.py` & `graph_validation_test_runners-0.1.1/standards_validation_test_runner/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 TRAPI and Biolink Model Standards Validation
 test (using reasoner-validator)
 """
 from typing import Optional, Dict
 import asyncio
 
-from reasoner_validator.validator import TRAPIResponseValidator
 from graph_validation_tests import (
     GraphValidationTest,
     TestCaseRun,
     get_parameters
 )
 from graph_validation_tests.translator.trapi import run_trapi_query
 
@@ -49,22 +48,16 @@
                 identifier=context[1],
                 context=context[0],
                 reason=output_node_binding
             )
 
         else:
             # sanity check: verify first that the TRAPI request
-            # is well-formed by the by_subject(test_asset)
-            validator: TRAPIResponseValidator = \
-                TRAPIResponseValidator(
-                    trapi_version=self.trapi_version,
-                    biolink_version=self.biolink_version
-                )
-            validator.validate(trapi_request, component="Query")
-            self.merge(validator)
+            # is well-formed by the self.test(test_asset)
+            self.validate(trapi_request, component="Query")
 
             # We'll ignore warnings and info messages
             if not (self.has_critical() or self.has_errors() or self.has_skipped()):
 
                 # Capture the raw TRAPI query request for reporting
                 self.trapi_request = trapi_request
 
@@ -89,15 +82,15 @@
                     status_code: int = trapi_response['status_code']
                     if status_code != 200:
                         self.report("critical.trapi.response.unexpected_http_code", identifier=status_code)
                     else:
                         #########################################################
                         # Looks good so far, so now validate the TRAPI response #
                         #########################################################
-                        validator.check_compliance_of_trapi_response(
+                        self.check_compliance_of_trapi_response(
                             response=trapi_response['response_json']
                         )
 
 
 class StandardsValidationTest(GraphValidationTest):
     def test_case_wrapper(self, test, **kwargs) -> TestCaseRun:
         return StandardsValidationTestCaseRun(test_run=self, test=test, **kwargs)
```

### Comparing `graph_validation_test_runners-0.0.12/tests/__init__.py` & `graph_validation_test_runners-0.1.1/tests/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,22 +5,40 @@
 
 TEST_DIR = os.path.abspath(os.path.dirname(__file__))
 PROJECT_DIR = os.path.join(os.path.abspath(os.path.dirname(__file__)), "..")
 SCRIPTS_DIR = os.path.join(os.path.abspath(os.path.dirname(__file__)), "scripts")
 
 DEFAULT_TRAPI_VERSION = get_latest_version("1")
 DEFAULT_BMT: Toolkit = get_biolink_model_toolkit()
-SAMPLE_TEST_INPUT_1 = {
+SAMPLE_MOLEPRO_INPUT_DATA = {
     # One test edge (asset)
     "test_asset_id": "TestAsset_1",
-    "subject_id": "CHEBI:58579",
-    "subject_category": "biolink:SmallMolecule",
-    "predicate_id": "biolink:is_active_metabolite_of",
-    "object_id": "UniProtKB:Q9NQ88",
-    "object_category": "biolink:Protein",
+    "subject_id": "CHEBI:16796",   # Melatonin
+    "subject_category": "biolink:ChemicalEntity",
+    "predicate_id": "biolink:treats",
+    "object_id": "MONDO:0005258",  # Autism
+    "object_category": "biolink:Disease",
     #
     #     "environment": environment, # Optional[TestEnvEnum] = None; default: 'TestEnvEnum.ci' if not given
     #     "components": components,  # Optional[str] = None; default: 'ars' if not given
     #     "trapi_version": trapi_version,  # Optional[str] = None; latest community release if not given
     #     "biolink_version": biolink_version,  # Optional[str] = None; current Biolink Toolkit default if not given
     #     "runner_settings": asset.test_runner_settings,  # Optional[List[str]] = None
 }
+
+SAMPLE_ARAX_INPUT_DATA = {
+    "test_asset_id": "TestAsset_1",
+    "subject_id": "PUBCHEM.COMPOUND:2801",  # Clomipramine
+    "subject_category": "biolink:ChemicalEntity",
+    "predicate_id": "biolink:treats",
+    "object_id": "ORPHANET:33110",  # Autosomal agammaglobulinemia?
+    "object_category": "biolink:Disease",
+}
+
+SAMPLE_ARAGORN_INPUT_DATA = {
+    "test_asset_id": "TestAsset_1",
+    "subject_id": "PUBCHEM.COMPOUND:2801",  # Clomipramine
+    "subject_category": "biolink:ChemicalEntity",
+    "predicate_id": "biolink:treats",
+    "object_id": "ORPHANET:251636",  # Ependymoma
+    "object_category": "biolink:Disease"
+}
```

### Comparing `graph_validation_test_runners-0.0.12/tests/graph_validation_test/translator/test_translator_smartapi_registry.py` & `graph_validation_test_runners-0.1.1/tests/graph_validation_test/translator/test_translator_smartapi_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -472,21 +472,25 @@
         assert 'url' in resource_metadata
         assert url in resource_metadata['url']
         assert x_maturity in resource_metadata['x_maturity']
     else:
         assert not resource_metadata
 
 
+@pytest.mark.skip(
+    reason="These tests often work fine with fresh data, " +
+           "but fail later due to changes in online resources"
+)
 @pytest.mark.parametrize(
     "component,environment,result",
     [
         ("arax", "dev", "https://arax.ncats.io/beta/api/arax/v1.4"),
-        # ("aragorn", "prod", "https://aragorn.transltr.io/aragorn"),
-        ("biothings-explorer", "test", "https://bte.test.transltr.io/v1"),
-        # ("improving-agent", "test", "https://ia.test.transltr.io/api/v1.4/"),
+        ("aragorn", "ci", "https://aragorn.ci.transltr.io/aragorn"),
+        ("biothings-explorer", "ci", "https://bte.ci.transltr.io/v1"),
+        ("improving-agent", "test", "https://ia.test.transltr.io/api/v1.4/"),
         ("molepro", "ci", "https://molepro-trapi.ci.transltr.io/molepro/trapi/v1.5"),
         ("foobar", "ci", None)
     ]
 )
 def test_get_component_endpoint_from_registry(
         component: str,
         environment: str,
```

### Comparing `graph_validation_test_runners-0.0.12/tests/graph_validation_test/translator/trapi/test_trapi.py` & `graph_validation_test_runners-0.1.1/tests/graph_validation_test/translator/trapi/test_trapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,14 @@
 from graph_validation_tests.utils.ontology_kp import (
     ONTOLOGY_KP_TRAPI_SERVER,
     NODE_NORMALIZER_SERVER
 )
 
 pytest_plugins = ('pytest_asyncio',)
 
-TRAPI_TEST_ENDPOINT = "https://molepro-trapi.transltr.io/molepro/trapi/v1.4"
-
 
 @pytest.mark.parametrize(
     "component,infores",
     [
         ("arax", "arax"),
         ("aragorn", "aragorn"),
         ("bte", "biothings-explorer"),
@@ -29,14 +27,18 @@
         ("molepro", "molepro")
     ]
 )
 def test_get_get_component_infores_object_id(component: str, infores: str):
     assert get_component_infores_object_id(component=component) == infores
 
 
+@pytest.mark.skip(
+    reason="These tests often work fine with fresh data, " +
+           "but fail later due to changes in online resources"
+)
 @pytest.mark.parametrize(
     "component,environment,result",
     [
         (None, None, f"https://ars.ci.transltr.io/ars/api/"),
         ("ars", None, f"https://ars.ci.transltr.io/ars/api/"),
         ("ars", "non-environment", None),
         ("ars", "test", f"https://ars.test.transltr.io/ars/api/"),
```

### Comparing `graph_validation_test_runners-0.0.12/tests/graph_validation_test_runner/test_graph_validation_test.py` & `graph_validation_test_runners-0.1.1/tests/graph_validation_test_runner/test_graph_validation_test.py`

 * *Files identical despite different names*

### Comparing `graph_validation_test_runners-0.0.12/tests/graph_validation_test_runner/test_unit_test_templates.py` & `graph_validation_test_runners-0.1.1/tests/graph_validation_test_runner/test_unit_test_templates.py`

 * *Files identical despite different names*

### Comparing `graph_validation_test_runners-0.0.12/tests/graph_validation_test_runner/translator/biolink/test_ontology_kp.py` & `graph_validation_test_runners-0.1.1/tests/graph_validation_test_runner/translator/biolink/test_ontology_kp.py`

 * *Files identical despite different names*

### Comparing `graph_validation_test_runners-0.0.12/tests/graph_validation_test_runner/translator/test_translator_smartapi_registry.py` & `graph_validation_test_runners-0.1.1/tests/graph_validation_test_runner/translator/test_translator_smartapi_registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -472,21 +472,25 @@
         assert 'url' in resource_metadata
         assert url in resource_metadata['url']
         assert x_maturity in resource_metadata['x_maturity']
     else:
         assert not resource_metadata
 
 
+@pytest.mark.skip(
+    reason="These tests often work fine with fresh data, " +
+           "but fail later due to changes in online resources"
+)
 @pytest.mark.parametrize(
     "component,environment,result",
     [
         ("arax", "dev", "https://arax.ncats.io/beta/api/arax/v1.4"),
-        # ("aragorn", "prod", "https://aragorn.transltr.io/aragorn"),
-        ("biothings-explorer", "test", "https://bte.test.transltr.io/v1"),
-        ("improving-agent", "test", "https://ia.test.transltr.io/api/v1.4/"),
+        ("aragorn", "ci", "https://aragorn.ci.transltr.io/aragorn"),
+        ("biothings-explorer", "ci", "https://bte.test.transltr.io/v1"),
+        ("improving-agent", "ci", "https://ia.test.transltr.io/api/v1.4/"),
         ("molepro", "ci", "https://molepro-trapi.ci.transltr.io/molepro/trapi/v1.5"),
         ("foobar", "ci", None)
     ]
 )
 def test_get_component_endpoint_from_registry(
         component: str,
         environment: str,
```

### Comparing `graph_validation_test_runners-0.0.12/tests/graph_validation_test_runner/translator/trapi/test_trapi.py` & `graph_validation_test_runners-0.1.1/tests/graph_validation_test_runner/translator/trapi/test_trapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,25 +29,29 @@
         ("molepro", "molepro")
     ]
 )
 def test_get_get_component_infores_object_id(component: str, infores: str):
     assert get_component_infores_object_id(component=component) == infores
 
 
+@pytest.mark.skip(
+    reason="These tests often work fine with fresh data, " +
+           "but fail later due to changes in online resources"
+)
 @pytest.mark.parametrize(
     "component,environment,result",
     [
         (None, None, f"https://ars.ci.transltr.io/ars/api/"),
         ("ars", None, f"https://ars.ci.transltr.io/ars/api/"),
         ("ars", "non-environment", None),
         ("ars", "test", f"https://ars.test.transltr.io/ars/api/"),
         ("arax", "dev", "https://arax.ncats.io/beta/api/arax/v1.4"),
-        # ("aragorn", "prod", "https://aragorn.transltr.io/aragorn"),
-        ("bte", "test", "https://bte.test.transltr.io/v1"),
-        ("improving", "test", "https://ia.test.transltr.io/api/v1.4/"),
+        ("aragorn", "ci", "https://aragorn.transltr.io/aragorn"),
+        ("bte", "ci", "https://bte.test.transltr.io/v1"),
+        ("improving", "ci", "https://ia.test.transltr.io/api/v1.4/"),
         ("molepro", "ci", "https://molepro-trapi.ci.transltr.io/molepro/trapi/v1.5"),
         ("foobar", "ci", None),
         ("arax", "non-environment", None),
     ]
 )
 def test_resolve_component_endpoint(
         component: Optional[str],
```

### Comparing `graph_validation_test_runners-0.0.12/tests/one_hop_test_runner/test_one_hop_test.py` & `graph_validation_test_runners-0.1.1/tests/one_hop_test_runner/test_one_hop_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,32 +13,32 @@
     by_object,
     raise_subject_entity,
     raise_object_entity,
     raise_object_by_subject,
     raise_predicate_by_subject
 )
 from one_hop_test_runner import OneHopTest, run_one_hop_tests
-from tests import SAMPLE_TEST_INPUT_1, SCRIPTS_DIR
+from tests import SAMPLE_MOLEPRO_INPUT_DATA, SCRIPTS_DIR, SAMPLE_ARAX_INPUT_DATA
 
 
 @pytest.mark.asyncio
 async def test_one_hop_test():
     trapi_generators = [
         by_subject,
         inverse_by_new_subject,
         by_object,
         raise_subject_entity,
         raise_object_entity,
         raise_object_by_subject,
         raise_predicate_by_subject
     ]
     results: Dict = await OneHopTest.run_tests(
-        **SAMPLE_TEST_INPUT_1,
+        **SAMPLE_MOLEPRO_INPUT_DATA,
         trapi_generators=trapi_generators,
-        environment="prod",
+        environment="ci",
         components=["arax", "molepro"]
     )
     dump(results, stderr, indent=4)
 
 
 # ARS tests not yet supported so yes... results will
 # always be empty, with a logger message to inform why
@@ -50,38 +50,77 @@
         by_object,
         raise_subject_entity,
         raise_object_entity,
         raise_object_by_subject,
         raise_predicate_by_subject
     ]
     results: Dict = await OneHopTest.run_tests(
-        **SAMPLE_TEST_INPUT_1,
+        **SAMPLE_MOLEPRO_INPUT_DATA,
         trapi_generators=trapi_generators,
         environment="prod"
     )
     assert not results
 
 
+@pytest.mark.parametrize(
+    "data,environment,component,expected_result",
+    [
+        (
+            SAMPLE_MOLEPRO_INPUT_DATA,
+            "ci",
+            "molepro",
+            None
+        ),
+        (
+            SAMPLE_ARAX_INPUT_DATA,
+            "ci",
+            "arax",
+            None
+        )
+    ]
+)
 @pytest.mark.asyncio
-async def test_run_one_hop_tests():
+async def test_run_one_hop_tests(
+        data: Dict,
+        environment: str,
+        component: str,
+        expected_result
+):
     results: Dict = await run_one_hop_tests(
-        **SAMPLE_TEST_INPUT_1,
-        environment="prod",
-        components=["arax", "molepro"]
+        **data,
+        environment=environment,
+        components=[component]
     )
     assert results
     dump(results, stderr, indent=4)
 
 
+@pytest.mark.parametrize(
+    "data,environment,component,expected_result",
+    [
+        (
+            SAMPLE_MOLEPRO_INPUT_DATA,
+            "ci",
+            "molepro",
+            None
+        )
+    ]
+)
+@pytest.mark.asyncio
 @pytest.mark.asyncio
-async def test_run_one_hop_tests_with_runner_parameters():
+async def test_run_one_hop_tests_with_runner_parameters(
+        data: Dict,
+        environment: str,
+        component: str,
+        expected_result
+):
     results: Dict = await run_one_hop_tests(
-        **SAMPLE_TEST_INPUT_1,
-        environment="prod",
-        components=["arax", "molepro"],
+        **data,
+        environment=environment,
+        components=[component],
         strict_validation=True
     )
     assert results
     dump(results, stderr, indent=4)
 
 
 # subprocess.run(
```

### Comparing `graph_validation_test_runners-0.0.12/PKG-INFO` & `graph_validation_test_runners-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graph-validation-test-runners
-Version: 0.0.12
+Version: 0.1.1
 Summary: Validation of Translator Knowledge Graphs - TRAPI, Biolink Model and One Hop navigation
 Home-page: https://github.com/TranslatorSRI
 License: MIT
 Keywords: NCATS,Biomedical Data Translator,Translator,ReasonerAPI,TRAPI,validation,Biolink Model
 Author: Richard Bruskiewich
 Author-email: richard.bruskiewich@delphinai.com
 Maintainer: Richard Bruskiewich
@@ -15,35 +15,34 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: deepdiff (>=6.7.1,<7.0.0)
 Requires-Dist: fastapi
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: matplotlib (>=3.8.3,<4.0.0)
-Requires-Dist: reasoner-validator (>=4.1.2,<5.0.0)
+Requires-Dist: reasoner-validator (>=4.1.4,<5.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Requires-Dist: translator-testing-model (>=0.3.1,<0.4.0)
 Project-URL: Bug Tracker, https://github.com/TranslatorSRI/graph-validation-test-runners/issues
 Project-URL: Change Log, https://github.com/TranslatorSRI/graph-validation-test-runners/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://github.com/TranslatorSRI/graph-validation-test-runners/blob/main/README.md
 Project-URL: Repository, https://github.com/TranslatorSRI/graph-validation-test-runners
 Description-Content-Type: text/markdown
 
 # Graph Validation Tests
 
-[![Pyversions](https://img.shields.io/pypi/pyversions/graph-validation-test-runners)](https://pypi.python.org/pypi/graph-validation-test-runners)
-[![Publish Python Package](https://github.com/TranslatorSRI/graph-validation-test-runners/actions/workflows/python-publish.yml/badge.svg)](https://pypi.org/project/graph-validation-test-runners/)
+![Pyversions](https://img.shields.io/pypi/pyversions/graph-validation-test-runners)
+[![PyPI - Version](https://img.shields.io/pypi/v/graph-validation-test-runners)](https://pypi.python.org/pypi/graph-validation-test-runners)
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
 [![Run tests](https://github.com/TranslatorSRI/graph-validation-test-runners/actions/workflows/test.yml/badge.svg)](https://github.com/TranslatorSRI/graph-validation-test-runners/actions/workflows/test.yml)
 
 
 This repository provides the implementation of Translator knowledge graph validation test runners within the new 2023 Testing Infrastructure.  The current package currently contains two such test runners:
 
 - **StandardsValidationTest:** is a wrapper of the [Translator reasoner-validator package](https://github.com/NCATSTranslator/reasoner-validator) which certifies that knowledge graph data access is TRAPI compliant and the graph semantic content is Biolink Model compliant.
@@ -55,15 +54,15 @@
 
 The **standards_validation_test_runner** and **one_hop_test_runner* may be run directly from the command line or programmatically, from within a Python script.
 
 ### Installation
 
 The **graph-validation-test-runners** module can be installed from pypi and used as part of the Translator-wide automated testing.
 
-_Note: Requires 3.9 <= Python release <= 3.12_
+_Note: Requires 3.9 <= Python release < 3.12_
 
 #### From Pypi
 
 From within your target working directory:
 
 - Create a python virtual environment: `python -m venv venv`
 - Activate your environment: `. ./venv/bin/activate`
```

