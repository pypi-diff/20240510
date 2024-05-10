# Comparing `tmp/openinference_instrumentation_dspy-0.1.7.tar.gz` & `tmp/openinference_instrumentation_dspy-0.1.8.tar.gz`

## Comparing `openinference_instrumentation_dspy-0.1.7.tar` & `openinference_instrumentation_dspy-0.1.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    24031 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.7/src/openinference/instrumentation/dspy/__init__.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.7/src/openinference/instrumentation/dspy/package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.7/src/openinference/instrumentation/dspy/py.typed
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.7/src/openinference/instrumentation/dspy/version.py
--rw-r--r--   0        0        0    15850 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.7/tests/openinference/instrumentation/dspy/test_instrumentor.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.7/.gitignore
--rw-r--r--   0        0        0    10840 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.7/LICENSE
--rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.7/README.md
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    24446 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.8/src/openinference/instrumentation/dspy/__init__.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.8/src/openinference/instrumentation/dspy/package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.8/src/openinference/instrumentation/dspy/py.typed
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.8/src/openinference/instrumentation/dspy/version.py
+-rw-r--r--   0        0        0    28449 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.8/tests/openinference/instrumentation/dspy/test_instrumentor.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.8/.gitignore
+-rw-r--r--   0        0        0    10840 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.8/LICENSE
+-rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.8/README.md
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     4927 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.8/PKG-INFO
```

### Comparing `openinference_instrumentation_dspy-0.1.7/src/openinference/instrumentation/dspy/__init__.py` & `openinference_instrumentation_dspy-0.1.8/src/openinference/instrumentation/dspy/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     List,
     Mapping,
     Optional,
     Tuple,
 )
 
 import opentelemetry.context as context_api
+from openinference.instrumentation import get_attributes_from_context
 from openinference.instrumentation.dspy.package import _instruments
 from openinference.instrumentation.dspy.version import __version__
 from openinference.semconv.trace import (
     DocumentAttributes,
     OpenInferenceMimeTypeValues,
     OpenInferenceSpanKindValues,
     SpanAttributes,
@@ -217,14 +218,15 @@
                         LLM_INVOCATION_PARAMETERS: json.dumps(invocation_parameters),
                         INPUT_VALUE: str(prompt),
                         INPUT_MIME_TYPE: OpenInferenceMimeTypeValues.TEXT.value,
                     }
                 )
             ),
         ) as span:
+            span.set_attributes(dict(get_attributes_from_context()))
             try:
                 response = wrapped(*args, **kwargs)
             except Exception as exception:
                 span.set_status(trace_api.Status(trace_api.StatusCode.ERROR, str(exception)))
                 span.record_exception(exception)
                 raise
             # TODO: parse usage. Need to decide if this
@@ -296,14 +298,15 @@
                             **kwargs,
                         ),
                         INPUT_MIME_TYPE: OpenInferenceMimeTypeValues.JSON.value,
                     }
                 )
             ),
         ) as span:
+            span.set_attributes(dict(get_attributes_from_context()))
             try:
                 prediction = wrapped(*args, **kwargs)
             except Exception as exception:
                 span.set_status(trace_api.Status(trace_api.StatusCode.ERROR, str(exception)))
                 span.record_exception(exception)
                 raise
             span.set_attributes(
@@ -365,14 +368,15 @@
                             else {}
                         ),
                         INPUT_MIME_TYPE: OpenInferenceMimeTypeValues.JSON.value,
                     }
                 )
             ),
         ) as span:
+            span.set_attributes(dict(get_attributes_from_context()))
             try:
                 prediction = wrapped(*args, **kwargs)
             except Exception as exception:
                 span.set_status(trace_api.Status(trace_api.StatusCode.ERROR, str(exception)))
                 span.record_exception(exception)
                 raise
             span.set_attributes(
@@ -416,14 +420,15 @@
                         OPENINFERENCE_SPAN_KIND: RETRIEVER.value,
                         INPUT_VALUE: _get_input_value(wrapped, *args, **kwargs),
                         INPUT_MIME_TYPE: OpenInferenceMimeTypeValues.JSON.value,
                     }
                 )
             ),
         ) as span:
+            span.set_attributes(dict(get_attributes_from_context()))
             try:
                 prediction = wrapped(*args, **kwargs)
             except Exception as exception:
                 span.set_status(trace_api.Status(trace_api.StatusCode.ERROR, str(exception)))
                 span.record_exception(exception)
                 raise
             span.set_attributes(
@@ -468,14 +473,15 @@
                         OPENINFERENCE_SPAN_KIND: RETRIEVER.value,
                         INPUT_VALUE: (_get_input_value(wrapped, *args, **kwargs)),
                         INPUT_MIME_TYPE: OpenInferenceMimeTypeValues.JSON.value,
                     }
                 )
             ),
         ) as span:
+            span.set_attributes(dict(get_attributes_from_context()))
             try:
                 retrieved_documents = wrapped(*args, **kwargs)
             except Exception as exception:
                 span.set_status(trace_api.Status(trace_api.StatusCode.ERROR, str(exception)))
                 span.record_exception(exception)
                 raise
             span.set_attributes(
```

### Comparing `openinference_instrumentation_dspy-0.1.7/LICENSE` & `openinference_instrumentation_dspy-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_dspy-0.1.7/README.md` & `openinference_instrumentation_dspy-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_dspy-0.1.7/pyproject.toml` & `openinference_instrumentation_dspy-0.1.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,15 @@
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
   "typing-extensions",
 ]
 
 [project.optional-dependencies]
 instruments = [
```

### Comparing `openinference_instrumentation_dspy-0.1.7/PKG-INFO` & `openinference_instrumentation_dspy-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: openinference-instrumentation-dspy
-Version: 0.1.7
+Version: 0.1.8
 Summary: OpenInference DSPy Instrumentation
 Project-URL: Homepage, https://github.com/Arize-ai/openinference/tree/main/python/instrumentation/openinference-instrumentation-dspy
 Author-email: OpenInference Authors <oss@arize.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: <3.13,>=3.9
+Requires-Dist: openinference-instrumentation>=0.1.5
 Requires-Dist: openinference-semantic-conventions
 Requires-Dist: opentelemetry-api
 Requires-Dist: opentelemetry-instrumentation
 Requires-Dist: opentelemetry-semantic-conventions
 Requires-Dist: typing-extensions
 Requires-Dist: wrapt
 Provides-Extra: instruments
```

