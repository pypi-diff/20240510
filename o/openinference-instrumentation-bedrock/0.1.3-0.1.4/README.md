# Comparing `tmp/openinference_instrumentation_bedrock-0.1.3.tar.gz` & `tmp/openinference_instrumentation_bedrock-0.1.4.tar.gz`

## Comparing `openinference_instrumentation_bedrock-0.1.3.tar` & `openinference_instrumentation_bedrock-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.3/src/openinference/instrumentation/bedrock/__init__.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.3/src/openinference/instrumentation/bedrock/package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.3/src/openinference/instrumentation/bedrock/py.typed
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.3/src/openinference/instrumentation/bedrock/version.py
--rw-r--r--   0        0        0     5663 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.3/tests/test_instrumentor.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.3/.gitignore
--rw-r--r--   0        0        0    10870 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.3/LICENSE
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.3/README.md
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     7938 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.4/src/openinference/instrumentation/bedrock/__init__.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.4/src/openinference/instrumentation/bedrock/package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.4/src/openinference/instrumentation/bedrock/py.typed
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.4/src/openinference/instrumentation/bedrock/version.py
+-rw-r--r--   0        0        0    11168 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.4/tests/test_instrumentor.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.4/.gitignore
+-rw-r--r--   0        0        0    10870 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.4/README.md
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.4/PKG-INFO
```

### Comparing `openinference_instrumentation_bedrock-0.1.3/src/openinference/instrumentation/bedrock/__init__.py` & `openinference_instrumentation_bedrock-0.1.4/src/openinference/instrumentation/bedrock/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from functools import wraps
 from importlib import import_module
 from inspect import signature
 from typing import IO, Any, Callable, Collection, Dict, Optional, Tuple, TypeVar, cast
 
 from botocore.client import BaseClient
 from botocore.response import StreamingBody
+from openinference.instrumentation import get_attributes_from_context
 from openinference.instrumentation.bedrock.package import _instruments
 from openinference.instrumentation.bedrock.version import __version__
 from openinference.semconv.trace import (
     OpenInferenceSpanKindValues,
     SpanAttributes,
 )
 from opentelemetry import context as context_api
@@ -148,14 +149,15 @@
                         content = str(response_body.get("generations"))
                     else:
                         content = ""
 
                     if content:
                         _set_span_attribute(span, SpanAttributes.OUTPUT_VALUE, content)
 
+                span.set_attributes(dict(get_attributes_from_context()))
                 return response  # type: ignore
 
         return instrumented_response
 
     return _invocation_wrapper
```

### Comparing `openinference_instrumentation_bedrock-0.1.3/LICENSE` & `openinference_instrumentation_bedrock-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_bedrock-0.1.3/pyproject.toml` & `openinference_instrumentation_bedrock-0.1.4/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -24,14 +24,15 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
   "opentelemetry-api",
   "opentelemetry-instrumentation",
   "opentelemetry-semantic-conventions",
+  "openinference-instrumentation>=0.1.5",
   "openinference-semantic-conventions",
   "wrapt",
 ]
 
 [project.optional-dependencies]
 instruments = [
   "boto3 >= 11.28.57",
@@ -52,7 +53,38 @@
 include = [
   "/src",
   "/tests",
 ]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/openinference"]
+
+[tool.mypy]
+strict = true
+explicit_package_bases = true
+exclude = [
+  "examples",
+  "dist",
+  "sdist",
+]
+
+[[tool.mypy.overrides]]
+ignore_missing_imports = true
+module = [
+  "wrapt",
+  "boto3",
+  "botocore.*",
+]
+
+[tool.ruff]
+line-length = 100
+target-version = "py38"
+
+[tool.ruff.lint.per-file-ignores]
+"*.ipynb" = ["E402", "E501"]
+
+[tool.ruff.lint]
+ignore-init-module-imports = true
+select = ["E", "F", "W", "I"]
+
+[tool.ruff.lint.isort]
+force-single-line = false
```

