# Comparing `tmp/openinference_instrumentation_mistralai-0.0.5.tar.gz` & `tmp/openinference_instrumentation_mistralai-0.0.6.tar.gz`

## Comparing `openinference_instrumentation_mistralai-0.0.5.tar` & `openinference_instrumentation_mistralai-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.5/src/openinference/instrumentation/mistralai/__init__.py
--rw-r--r--   0        0        0    14815 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.5/src/openinference/instrumentation/mistralai/_chat_wrapper.py
--rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.5/src/openinference/instrumentation/mistralai/_request_attributes_extractor.py
--rw-r--r--   0        0        0     6761 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.5/src/openinference/instrumentation/mistralai/_response_accumulator.py
--rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.5/src/openinference/instrumentation/mistralai/_response_attributes_extractor.py
--rw-r--r--   0        0        0     5308 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.5/src/openinference/instrumentation/mistralai/_stream.py
--rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.5/src/openinference/instrumentation/mistralai/_utils.py
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.5/src/openinference/instrumentation/mistralai/_with_span.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.5/src/openinference/instrumentation/mistralai/package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.5/src/openinference/instrumentation/mistralai/py.typed
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.5/src/openinference/instrumentation/mistralai/version.py
--rw-r--r--   0        0        0    65793 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.5/tests/openinference/instrumentation/mistralai/test_instrumentor.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.5/.gitignore
--rw-r--r--   0        0        0    10870 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.5/LICENSE
--rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.5/README.md
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     4263 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.6/src/openinference/instrumentation/mistralai/__init__.py
+-rw-r--r--   0        0        0    15245 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.6/src/openinference/instrumentation/mistralai/_chat_wrapper.py
+-rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.6/src/openinference/instrumentation/mistralai/_request_attributes_extractor.py
+-rw-r--r--   0        0        0     6761 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.6/src/openinference/instrumentation/mistralai/_response_accumulator.py
+-rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.6/src/openinference/instrumentation/mistralai/_response_attributes_extractor.py
+-rw-r--r--   0        0        0     5308 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.6/src/openinference/instrumentation/mistralai/_stream.py
+-rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.6/src/openinference/instrumentation/mistralai/_utils.py
+-rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.6/src/openinference/instrumentation/mistralai/_with_span.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.6/src/openinference/instrumentation/mistralai/package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.6/src/openinference/instrumentation/mistralai/py.typed
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.6/src/openinference/instrumentation/mistralai/version.py
+-rw-r--r--   0        0        0    78196 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.6/tests/openinference/instrumentation/mistralai/test_instrumentor.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.6/.gitignore
+-rw-r--r--   0        0        0    10870 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2932 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.6/README.md
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.6/PKG-INFO
```

### Comparing `openinference_instrumentation_mistralai-0.0.5/src/openinference/instrumentation/mistralai/__init__.py` & `openinference_instrumentation_mistralai-0.0.6/src/openinference/instrumentation/mistralai/__init__.py`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_mistralai-0.0.5/src/openinference/instrumentation/mistralai/_chat_wrapper.py` & `openinference_instrumentation_mistralai-0.0.6/src/openinference/instrumentation/mistralai/_chat_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     Dict,
     Iterable,
     Iterator,
     Mapping,
     Tuple,
 )
 
+from openinference.instrumentation import get_attributes_from_context
 from openinference.instrumentation.mistralai._request_attributes_extractor import (
     _RequestAttributesExtractor,
 )
 from openinference.instrumentation.mistralai._response_accumulator import _ChatCompletionAccumulator
 from openinference.instrumentation.mistralai._response_attributes_extractor import (
     _ResponseAttributesExtractor,
 )
@@ -56,14 +57,15 @@
         self._tracer = tracer
 
     @contextmanager
     def _start_as_current_span(
         self,
         span_name: str,
         attributes: Iterable[Tuple[str, AttributeValue]],
+        context_attributes: Iterable[Tuple[str, AttributeValue]],
         extra_attributes: Iterable[Tuple[str, AttributeValue]],
     ) -> Iterator[_WithSpan]:
         # Because OTEL has a default limit of 128 attributes, we split our
         # attributes into two tiers, where "extra_attributes" are added first to
         # ensure that the most important "attributes" are added last and are not
         # dropped.
         try:
@@ -73,15 +75,19 @@
             span = INVALID_SPAN
         with trace_api.use_span(
             span,
             end_on_exit=False,
             record_exception=False,
             set_status_on_exception=False,
         ) as span:
-            yield _WithSpan(span=span, extra_attributes=dict(attributes))
+            yield _WithSpan(
+                span=span,
+                context_attributes=dict(context_attributes),
+                extra_attributes=dict(attributes),
+            )
 
 
 class _WithMistralAI(ABC):
     __slots__ = (
         "_mistral_client",
         "_request_attributes_extractor",
         "_response_attributes_extractor",
@@ -213,14 +219,15 @@
             span_name = "MistralClient.chat"
         except Exception:
             logger.exception("Failed to parse request args")
             return wrapped(*args, **kwargs)
         with self._start_as_current_span(
             span_name=span_name,
             attributes=self._get_attributes_from_request(request_parameters),
+            context_attributes=get_attributes_from_context(),
             extra_attributes=self._get_extra_attributes_from_request(request_parameters),
         ) as with_span:
             try:
                 response = wrapped(*args, **kwargs)
             except Exception as exception:
                 with_span.record_exception(exception)
                 status = trace_api.Status(
@@ -260,14 +267,15 @@
             span_name = "MistralAsyncClient.chat"
         except Exception:
             logger.exception("Failed to parse request args")
             return await wrapped(*args, **kwargs)
         with self._start_as_current_span(
             span_name=span_name,
             attributes=self._get_attributes_from_request(request_parameters),
+            context_attributes=get_attributes_from_context(),
             extra_attributes=self._get_extra_attributes_from_request(request_parameters),
         ) as with_span:
             try:
                 response = await wrapped(*args, **kwargs)
             except Exception as exception:
                 with_span.record_exception(exception)
                 status = trace_api.Status(
@@ -307,14 +315,15 @@
             span_name = "MistralAsyncClient.chat"
         except Exception:
             logger.exception("Failed to parse request args")
             return wrapped(*args, **kwargs)
         with self._start_as_current_span(
             span_name=span_name,
             attributes=self._get_attributes_from_request(request_parameters),
+            context_attributes=get_attributes_from_context(),
             extra_attributes=self._get_extra_attributes_from_request(request_parameters),
         ) as with_span:
             try:
                 response = wrapped(*args, **kwargs)
             except Exception as exception:
                 with_span.record_exception(exception)
                 status = trace_api.Status(
```

### Comparing `openinference_instrumentation_mistralai-0.0.5/src/openinference/instrumentation/mistralai/_request_attributes_extractor.py` & `openinference_instrumentation_mistralai-0.0.6/src/openinference/instrumentation/mistralai/_request_attributes_extractor.py`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_mistralai-0.0.5/src/openinference/instrumentation/mistralai/_response_accumulator.py` & `openinference_instrumentation_mistralai-0.0.6/src/openinference/instrumentation/mistralai/_response_accumulator.py`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_mistralai-0.0.5/src/openinference/instrumentation/mistralai/_response_attributes_extractor.py` & `openinference_instrumentation_mistralai-0.0.6/src/openinference/instrumentation/mistralai/_response_attributes_extractor.py`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_mistralai-0.0.5/src/openinference/instrumentation/mistralai/_stream.py` & `openinference_instrumentation_mistralai-0.0.6/src/openinference/instrumentation/mistralai/_stream.py`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_mistralai-0.0.5/src/openinference/instrumentation/mistralai/_utils.py` & `openinference_instrumentation_mistralai-0.0.6/src/openinference/instrumentation/mistralai/_utils.py`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_mistralai-0.0.5/src/openinference/instrumentation/mistralai/_with_span.py` & `openinference_instrumentation_mistralai-0.0.6/src/openinference/instrumentation/mistralai/_with_span.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,24 +7,27 @@
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
 
 
 class _WithSpan:
     __slots__ = (
         "_span",
+        "_context_attributes",
         "_extra_attributes",
         "_is_finished",
     )
 
     def __init__(
         self,
         span: trace_api.Span,
+        context_attributes: Attributes = None,
         extra_attributes: Attributes = None,
     ) -> None:
         self._span = span
+        self._context_attributes = context_attributes
         self._extra_attributes = extra_attributes
         try:
             self._is_finished = not self._span.is_recording()
         except Exception:
             logger.exception("Failed to check if span is recording")
             self._is_finished = True
 
@@ -54,14 +57,15 @@
         attributes: Attributes = None,
         extra_attributes: Attributes = None,
     ) -> None:
         if self._is_finished:
             return
         for mapping in (
             attributes,
+            self._context_attributes,
             self._extra_attributes,
             extra_attributes,
         ):
             if not mapping:
                 continue
             for key, value in mapping.items():
                 if value is None:
```

### Comparing `openinference_instrumentation_mistralai-0.0.5/tests/openinference/instrumentation/mistralai/test_instrumentor.py` & `openinference_instrumentation_mistralai-0.0.6/tests/openinference/instrumentation/mistralai/test_instrumentor.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,35 @@
 import json
 from typing import (
     Any,
     AsyncIterator,
+    Dict,
     Generator,
     Iterable,
     Iterator,
     List,
     Mapping,
     cast,
 )
 
 import pytest
 import respx
 from httpx import AsyncByteStream, Response
 from mistralai.async_client import MistralAsyncClient
 from mistralai.client import MistralClient
 from mistralai.exceptions import MistralAPIException
-from mistralai.models.chat_completion import ChatMessage, FunctionCall, ToolCall, ToolChoice
+from mistralai.models.chat_completion import (
+    ChatCompletionResponse,
+    ChatCompletionStreamResponse,
+    ChatMessage,
+    FunctionCall,
+    ToolCall,
+    ToolChoice,
+)
+from openinference.instrumentation import using_attributes
 from openinference.instrumentation.mistralai import MistralAIInstrumentor
 from openinference.semconv.trace import (
     EmbeddingAttributes,
     MessageAttributes,
     OpenInferenceMimeTypeValues,
     OpenInferenceSpanKindValues,
     SpanAttributes,
@@ -30,18 +39,27 @@
 from opentelemetry.sdk import trace as trace_sdk
 from opentelemetry.sdk.resources import Resource
 from opentelemetry.sdk.trace.export import SimpleSpanProcessor
 from opentelemetry.sdk.trace.export.in_memory_span_exporter import InMemorySpanExporter
 from opentelemetry.util.types import AttributeValue
 
 
+@pytest.mark.parametrize("use_context_attributes", [False, True])
 def test_synchronous_chat_completions_emits_expected_span(
+    use_context_attributes: bool,
     mistral_sync_client: MistralClient,
     in_memory_span_exporter: InMemorySpanExporter,
     respx_mock: Any,
+    session_id: str,
+    user_id: str,
+    metadata: Dict[str, Any],
+    tags: List[str],
+    prompt_template: str,
+    prompt_template_version: str,
+    prompt_template_variables: Dict[str, Any],
 ) -> None:
     respx.post("https://api.mistral.ai/v1/chat/completions").mock(
         return_value=Response(
             200,
             json={
                 "id": "a21b3c92f73642ccb6352ff9883c327b",
                 "object": "chat.completion",
@@ -59,24 +77,40 @@
                         "logprobs": None,
                     }
                 ],
                 "usage": {"prompt_tokens": 15, "total_tokens": 156, "completion_tokens": 141},
             },
         )
     )
-    response = mistral_sync_client.chat(
-        model="mistral-large-latest",
-        messages=[
-            ChatMessage(
-                content="Who won the World Cup in 2018? Answer in one word, no punctuation.",
-                role="user",
-            )
-        ],
-        temperature=0.1,
-    )
+
+    def mistral_chat() -> ChatCompletionResponse:
+        return mistral_sync_client.chat(
+            model="mistral-large-latest",
+            messages=[
+                ChatMessage(
+                    content="Who won the World Cup in 2018? Answer in one word, no punctuation.",
+                    role="user",
+                )
+            ],
+            temperature=0.1,
+        )
+
+    if use_context_attributes:
+        with using_attributes(
+            session_id=session_id,
+            user_id=user_id,
+            metadata=metadata,
+            tags=tags,
+            prompt_template=prompt_template,
+            prompt_template_version=prompt_template_version,
+            prompt_template_variables=prompt_template_variables,
+        ):
+            response = mistral_chat()
+    else:
+        response = mistral_chat()
     choices = response.choices
     assert len(choices) == 1
     response_content = choices[0].message.content
     assert isinstance(response_content, str)
     assert "France" in response_content
 
     spans = in_memory_span_exporter.get_finished_spans()
@@ -118,21 +152,41 @@
         OpenInferenceMimeTypeValues(attributes.pop(OUTPUT_MIME_TYPE))
         == OpenInferenceMimeTypeValues.JSON
     )
     assert attributes.pop(LLM_TOKEN_COUNT_PROMPT) == 15
     assert attributes.pop(LLM_TOKEN_COUNT_COMPLETION) == 141
     assert attributes.pop(LLM_TOKEN_COUNT_TOTAL) == 156
     assert attributes.pop(LLM_MODEL_NAME) == "mistral-large-latest"
+    if use_context_attributes:
+        _check_context_attributes(
+            attributes,
+            session_id,
+            user_id,
+            metadata,
+            tags,
+            prompt_template,
+            prompt_template_version,
+            prompt_template_variables,
+        )
     assert attributes == {}  # test should account for all span attributes
 
 
+@pytest.mark.parametrize("use_context_attributes", [False, True])
 def test_synchronous_chat_completions_with_tool_call_response_emits_expected_spans(
+    use_context_attributes: bool,
     mistral_sync_client: MistralClient,
     in_memory_span_exporter: InMemorySpanExporter,
     respx_mock: Any,
+    session_id: str,
+    user_id: str,
+    metadata: Dict[str, Any],
+    tags: List[str],
+    prompt_template: str,
+    prompt_template_version: str,
+    prompt_template_variables: Dict[str, Any],
 ) -> None:
     respx.post("https://api.mistral.ai/v1/chat/completions").mock(
         return_value=Response(
             200,
             json={
                 "id": "6e8cf9abaac64c038c97e8db21e90567",
                 "object": "chat.completion",
@@ -157,43 +211,59 @@
                         "logprobs": None,
                     }
                 ],
                 "usage": {"prompt_tokens": 96, "total_tokens": 119, "completion_tokens": 23},
             },
         )
     )
-    response = mistral_sync_client.chat(
-        model="mistral-large-latest",
-        tool_choice=ToolChoice.any,
-        tools=[
-            {
-                "type": "function",
-                "function": {
-                    "name": "get_weather",
-                    "description": "finds the weather for a given city",
-                    "parameters": {
-                        "type": "object",
-                        "properties": {
-                            "city": {
-                                "type": "string",
-                                "description": "The city to find the weather for, e.g. 'London'",
-                            }
-                        },
-                        "required": ["city"],
+
+    def mistral_chat() -> ChatCompletionResponse:
+        tool = {
+            "type": "function",
+            "function": {
+                "name": "get_weather",
+                "description": "finds the weather for a given city",
+                "parameters": {
+                    "type": "object",
+                    "properties": {
+                        "city": {
+                            "type": "string",
+                            "description": "The city to find the weather for, e.g. 'London'",
+                        }
                     },
+                    "required": ["city"],
                 },
             },
-        ],
-        messages=[
-            ChatMessage(
-                content="What's the weather like in San Francisco?",
-                role="user",
-            )
-        ],
-    )
+        }
+
+        return mistral_sync_client.chat(
+            model="mistral-large-latest",
+            tool_choice=ToolChoice.any,
+            tools=[tool],
+            messages=[
+                ChatMessage(
+                    content="What's the weather like in San Francisco?",
+                    role="user",
+                )
+            ],
+        )
+
+    if use_context_attributes:
+        with using_attributes(
+            session_id=session_id,
+            user_id=user_id,
+            metadata=metadata,
+            tags=tags,
+            prompt_template=prompt_template,
+            prompt_template_version=prompt_template_version,
+            prompt_template_variables=prompt_template_variables,
+        ):
+            response = mistral_chat()
+    else:
+        response = mistral_chat()
     choices = response.choices
     assert len(choices) == 1
     assert choices[0].message.content == ""
 
     assert (tool_calls := choices[0].message.tool_calls)
     assert len(tool_calls) == 1
     assert (tool_call := tool_calls[0])
@@ -245,21 +315,41 @@
         OpenInferenceMimeTypeValues(attributes.pop(OUTPUT_MIME_TYPE))
         == OpenInferenceMimeTypeValues.JSON
     )
     assert attributes.pop(LLM_TOKEN_COUNT_PROMPT) == 96
     assert attributes.pop(LLM_TOKEN_COUNT_COMPLETION) == 23
     assert attributes.pop(LLM_TOKEN_COUNT_TOTAL) == 119
     assert attributes.pop(LLM_MODEL_NAME) == "mistral-large-latest"
+    if use_context_attributes:
+        _check_context_attributes(
+            attributes,
+            session_id,
+            user_id,
+            metadata,
+            tags,
+            prompt_template,
+            prompt_template_version,
+            prompt_template_variables,
+        )
     assert attributes == {}  # test should account for all span attributes
 
 
+@pytest.mark.parametrize("use_context_attributes", [False, True])
 def test_synchronous_chat_completions_with_tool_call_message_emits_expected_spans(
+    use_context_attributes: bool,
     mistral_sync_client: MistralClient,
     in_memory_span_exporter: InMemorySpanExporter,
     respx_mock: Any,
+    session_id: str,
+    user_id: str,
+    metadata: Dict[str, Any],
+    tags: List[str],
+    prompt_template: str,
+    prompt_template_version: str,
+    prompt_template_variables: Dict[str, Any],
 ) -> None:
     respx.post("https://api.mistral.ai/v1/chat/completions").mock(
         return_value=Response(
             200,
             json={
                 "id": "55ef30fc9c13499f92c77214ff056e7f",
                 "object": "chat.completion",
@@ -277,35 +367,53 @@
                         "logprobs": None,
                     }
                 ],
                 "usage": {"prompt_tokens": 64, "total_tokens": 74, "completion_tokens": 10},
             },
         )
     )
-    response = mistral_sync_client.chat(
-        model="mistral-large-latest",
-        messages=[
-            ChatMessage(
-                content="What's the weather like in San Francisco?",
-                role="user",
-            ),
-            ChatMessage(
-                content="",
-                role="assistant",
-                tool_calls=[
-                    ToolCall(
-                        function=FunctionCall(
-                            name="get_weather", arguments='{"city": "San Francisco"}'
+
+    def mistral_chat() -> ChatCompletionResponse:
+        return mistral_sync_client.chat(
+            model="mistral-large-latest",
+            messages=[
+                ChatMessage(
+                    content="What's the weather like in San Francisco?",
+                    role="user",
+                ),
+                ChatMessage(
+                    content="",
+                    role="assistant",
+                    tool_calls=[
+                        ToolCall(
+                            function=FunctionCall(
+                                name="get_weather", arguments='{"city": "San Francisco"}'
+                            )
                         )
-                    )
-                ],
-            ),
-            ChatMessage(role="tool", name="get_weather", content='{"weather_category": "sunny"}'),
-        ],
-    )
+                    ],
+                ),
+                ChatMessage(
+                    role="tool", name="get_weather", content='{"weather_category": "sunny"}'
+                ),
+            ],
+        )
+
+    if use_context_attributes:
+        with using_attributes(
+            session_id=session_id,
+            user_id=user_id,
+            metadata=metadata,
+            tags=tags,
+            prompt_template=prompt_template,
+            prompt_template_version=prompt_template_version,
+            prompt_template_variables=prompt_template_variables,
+        ):
+            response = mistral_chat()
+    else:
+        response = mistral_chat()
     choices = response.choices
     assert len(choices) == 1
     assert choices[0].message.content == "The weather in San Francisco is currently sunny."
 
     spans = in_memory_span_exporter.get_finished_spans()
     assert len(spans) == 1
 
@@ -362,40 +470,76 @@
         OpenInferenceMimeTypeValues(attributes.pop(OUTPUT_MIME_TYPE))
         == OpenInferenceMimeTypeValues.JSON
     )
     assert attributes.pop(LLM_TOKEN_COUNT_PROMPT) == 64
     assert attributes.pop(LLM_TOKEN_COUNT_COMPLETION) == 10
     assert attributes.pop(LLM_TOKEN_COUNT_TOTAL) == 74
     assert attributes.pop(LLM_MODEL_NAME) == "mistral-large-latest"
+    if use_context_attributes:
+        _check_context_attributes(
+            attributes,
+            session_id,
+            user_id,
+            metadata,
+            tags,
+            prompt_template,
+            prompt_template_version,
+            prompt_template_variables,
+        )
     assert attributes == {}  # test should account for all span attributes
 
 
+@pytest.mark.parametrize("use_context_attributes", [False, True])
 def test_synchronous_chat_completions_emits_span_with_exception_event_on_error(
+    use_context_attributes: bool,
     mistral_sync_client: MistralClient,
     in_memory_span_exporter: InMemorySpanExporter,
     respx_mock: Any,
+    session_id: str,
+    user_id: str,
+    metadata: Dict[str, Any],
+    tags: List[str],
+    prompt_template: str,
+    prompt_template_version: str,
+    prompt_template_variables: Dict[str, Any],
 ) -> None:
     respx.post("https://api.mistral.ai/v1/chat/completions").mock(
         return_value=Response(
             401,
             json={"message": "Unauthorized", "request_id": "2387442eca7ad4280697667d25a36f14"},
         )
     )
-    with pytest.raises(MistralAPIException):
-        mistral_sync_client.chat(
+
+    def mistral_chat() -> ChatCompletionResponse:
+        return mistral_sync_client.chat(
             model="mistral-large-latest",
             messages=[
                 ChatMessage(
                     content="Who won the World Cup in 2018? Answer in one word, no punctuation.",
                     role="user",
                 )
             ],
             temperature=0.1,
         )
 
+    with pytest.raises(MistralAPIException):
+        if use_context_attributes:
+            with using_attributes(
+                session_id=session_id,
+                user_id=user_id,
+                metadata=metadata,
+                tags=tags,
+                prompt_template=prompt_template,
+                prompt_template_version=prompt_template_version,
+                prompt_template_variables=prompt_template_variables,
+            ):
+                mistral_chat()
+        else:
+            mistral_chat()
+
     spans = in_memory_span_exporter.get_finished_spans()
     assert len(spans) == 1
     span = spans[0]
     assert not span.status.is_ok
     assert isinstance(span.status.description, str)
     assert "Unauthorized" in span.status.description
     assert len(span.events) == 1
@@ -416,22 +560,42 @@
     }
 
     assert attributes.pop(f"{LLM_INPUT_MESSAGES}.0.{MESSAGE_ROLE}") == "user"
     assert (
         attributes.pop(f"{LLM_INPUT_MESSAGES}.0.{MESSAGE_CONTENT}")
         == "Who won the World Cup in 2018? Answer in one word, no punctuation."
     )
+    if use_context_attributes:
+        _check_context_attributes(
+            attributes,
+            session_id,
+            user_id,
+            metadata,
+            tags,
+            prompt_template,
+            prompt_template_version,
+            prompt_template_variables,
+        )
     assert attributes == {}  # test should account for all span attributes
 
 
 @pytest.mark.asyncio
+@pytest.mark.parametrize("use_context_attributes", [False, True])
 async def test_asynchronous_chat_completions_emits_expected_span(
+    use_context_attributes: bool,
     mistral_async_client: MistralAsyncClient,
     in_memory_span_exporter: InMemorySpanExporter,
     respx_mock: Any,
+    session_id: str,
+    user_id: str,
+    metadata: Dict[str, Any],
+    tags: List[str],
+    prompt_template: str,
+    prompt_template_version: str,
+    prompt_template_variables: Dict[str, Any],
 ) -> None:
     respx.post("https://api.mistral.ai/v1/chat/completions").mock(
         return_value=Response(
             200,
             json={
                 "id": "a21b3c92f73642ccb6352ff9883c327b",
                 "object": "chat.completion",
@@ -449,24 +613,40 @@
                         "logprobs": None,
                     }
                 ],
                 "usage": {"prompt_tokens": 15, "total_tokens": 156, "completion_tokens": 141},
             },
         )
     )
-    response = await mistral_async_client.chat(
-        model="mistral-large-latest",
-        messages=[
-            ChatMessage(
-                content="Who won the World Cup in 2018? Answer in one word, no punctuation.",
-                role="user",
-            )
-        ],
-        temperature=0.1,
-    )
+
+    async def mistral_chat() -> ChatCompletionResponse:
+        return await mistral_async_client.chat(
+            model="mistral-large-latest",
+            messages=[
+                ChatMessage(
+                    content="Who won the World Cup in 2018? Answer in one word, no punctuation.",
+                    role="user",
+                )
+            ],
+            temperature=0.1,
+        )
+
+    if use_context_attributes:
+        with using_attributes(
+            session_id=session_id,
+            user_id=user_id,
+            metadata=metadata,
+            tags=tags,
+            prompt_template=prompt_template,
+            prompt_template_version=prompt_template_version,
+            prompt_template_variables=prompt_template_variables,
+        ):
+            response = await mistral_chat()
+    else:
+        response = await mistral_chat()
     choices = response.choices
     assert len(choices) == 1
     response_content = choices[0].message.content
     assert isinstance(response_content, str)
     assert "France" in response_content
 
     spans = in_memory_span_exporter.get_finished_spans()
@@ -508,41 +688,77 @@
         OpenInferenceMimeTypeValues(attributes.pop(OUTPUT_MIME_TYPE))
         == OpenInferenceMimeTypeValues.JSON
     )
     assert attributes.pop(LLM_TOKEN_COUNT_PROMPT) == 15
     assert attributes.pop(LLM_TOKEN_COUNT_COMPLETION) == 141
     assert attributes.pop(LLM_TOKEN_COUNT_TOTAL) == 156
     assert attributes.pop(LLM_MODEL_NAME) == "mistral-large-latest"
+    if use_context_attributes:
+        _check_context_attributes(
+            attributes,
+            session_id,
+            user_id,
+            metadata,
+            tags,
+            prompt_template,
+            prompt_template_version,
+            prompt_template_variables,
+        )
     assert attributes == {}  # test should account for all span attributes
 
 
 @pytest.mark.asyncio
+@pytest.mark.parametrize("use_context_attributes", [False, True])
 async def test_asynchronous_chat_completions_emits_span_with_exception_event_on_error(
+    use_context_attributes: bool,
     mistral_async_client: MistralAsyncClient,
     in_memory_span_exporter: InMemorySpanExporter,
     respx_mock: Any,
+    session_id: str,
+    user_id: str,
+    metadata: Dict[str, Any],
+    tags: List[str],
+    prompt_template: str,
+    prompt_template_version: str,
+    prompt_template_variables: Dict[str, Any],
 ) -> None:
     respx.post("https://api.mistral.ai/v1/chat/completions").mock(
         return_value=Response(
             401,
             json={"message": "Unauthorized", "request_id": "2387442eca7ad4280697667d25a36f14"},
         )
     )
-    with pytest.raises(MistralAPIException):
-        await mistral_async_client.chat(
+
+    async def mistral_chat() -> ChatCompletionResponse:
+        return await mistral_async_client.chat(
             model="mistral-large-latest",
             messages=[
                 ChatMessage(
                     content="Who won the World Cup in 2018? Answer in one word, no punctuation.",
                     role="user",
                 )
             ],
             temperature=0.1,
         )
 
+    with pytest.raises(MistralAPIException):
+        if use_context_attributes:
+            with using_attributes(
+                session_id=session_id,
+                user_id=user_id,
+                metadata=metadata,
+                tags=tags,
+                prompt_template=prompt_template,
+                prompt_template_version=prompt_template_version,
+                prompt_template_variables=prompt_template_variables,
+            ):
+                await mistral_chat()
+        else:
+            await mistral_chat()
+
     spans = in_memory_span_exporter.get_finished_spans()
     assert len(spans) == 1
     span = spans[0]
     assert not span.status.is_ok
     assert isinstance(span.status.description, str)
     assert "Unauthorized" in span.status.description
     assert len(span.events) == 1
@@ -563,39 +779,75 @@
     }
 
     assert attributes.pop(f"{LLM_INPUT_MESSAGES}.0.{MESSAGE_ROLE}") == "user"
     assert (
         attributes.pop(f"{LLM_INPUT_MESSAGES}.0.{MESSAGE_CONTENT}")
         == "Who won the World Cup in 2018? Answer in one word, no punctuation."
     )
+    if use_context_attributes:
+        _check_context_attributes(
+            attributes,
+            session_id,
+            user_id,
+            metadata,
+            tags,
+            prompt_template,
+            prompt_template_version,
+            prompt_template_variables,
+        )
     assert attributes == {}  # test should account for all span attributes
 
 
+@pytest.mark.parametrize("use_context_attributes", [False, True])
 def test_synchronous_streaming_chat_completions_emits_expected_span(
+    use_context_attributes: bool,
     mistral_sync_client: MistralClient,
     in_memory_span_exporter: InMemorySpanExporter,
     chat_stream: AsyncByteStream,
     respx_mock: Any,
+    session_id: str,
+    user_id: str,
+    metadata: Dict[str, Any],
+    tags: List[str],
+    prompt_template: str,
+    prompt_template_version: str,
+    prompt_template_variables: Dict[str, Any],
 ) -> None:
     respx.post("https://api.mistral.ai/v1/chat/completions").mock(
         return_value=Response(
             200,
             stream=chat_stream,
         )
     )
-    response_stream = mistral_sync_client.chat_stream(
-        model="mistral-large-latest",
-        messages=[
-            ChatMessage(
-                content="Who won the World Cup in 2018? Answer in one word, no punctuation.",
-                role="user",
-            )
-        ],
-        temperature=0.1,
-    )
+
+    def mistral_stream() -> Iterable[ChatCompletionStreamResponse]:
+        return mistral_sync_client.chat_stream(
+            model="mistral-large-latest",
+            messages=[
+                ChatMessage(
+                    content="Who won the World Cup in 2018? Answer in one word, no punctuation.",
+                    role="user",
+                )
+            ],
+            temperature=0.1,
+        )
+
+    if use_context_attributes:
+        with using_attributes(
+            session_id=session_id,
+            user_id=user_id,
+            metadata=metadata,
+            tags=tags,
+            prompt_template=prompt_template,
+            prompt_template_version=prompt_template_version,
+            prompt_template_variables=prompt_template_variables,
+        ):
+            response_stream = mistral_stream()
+    else:
+        response_stream = mistral_stream()
     response_content = ""
     for chunk in response_stream:
         if chunk_content := chunk.choices[0].delta.content:
             response_content += chunk_content
 
     assert (
         response_content
@@ -643,40 +895,76 @@
         OpenInferenceMimeTypeValues(attributes.pop(OUTPUT_MIME_TYPE))
         == OpenInferenceMimeTypeValues.JSON
     )
     assert attributes.pop(LLM_TOKEN_COUNT_PROMPT) == 15
     assert attributes.pop(LLM_TOKEN_COUNT_COMPLETION) == 109
     assert attributes.pop(LLM_TOKEN_COUNT_TOTAL) == 124
     assert attributes.pop(LLM_MODEL_NAME) == "mistral-large-latest"
+    if use_context_attributes:
+        _check_context_attributes(
+            attributes,
+            session_id,
+            user_id,
+            metadata,
+            tags,
+            prompt_template,
+            prompt_template_version,
+            prompt_template_variables,
+        )
     assert attributes == {}  # test should account for all span attributes
 
 
 @pytest.mark.asyncio
+@pytest.mark.parametrize("use_context_attributes", [False, True])
 async def test_asynchronous_streaming_chat_completions_emits_expected_span(
+    use_context_attributes: bool,
     mistral_async_client: MistralAsyncClient,
     in_memory_span_exporter: InMemorySpanExporter,
     chat_stream: AsyncByteStream,
     respx_mock: Any,
+    session_id: str,
+    user_id: str,
+    metadata: Dict[str, Any],
+    tags: List[str],
+    prompt_template: str,
+    prompt_template_version: str,
+    prompt_template_variables: Dict[str, Any],
 ) -> None:
     respx.post("https://api.mistral.ai/v1/chat/completions").mock(
         return_value=Response(
             200,
             stream=chat_stream,
         )
     )
-    response_stream = mistral_async_client.chat_stream(
-        model="mistral-large-latest",
-        messages=[
-            ChatMessage(
-                content="Who won the World Cup in 2018? Answer in one word, no punctuation.",
-                role="user",
-            )
-        ],
-        temperature=0.1,
-    )
+
+    async def mistral_stream() -> AsyncIterator[ChatCompletionStreamResponse]:
+        return mistral_async_client.chat_stream(
+            model="mistral-large-latest",
+            messages=[
+                ChatMessage(
+                    content="Who won the World Cup in 2018? Answer in one word, no punctuation.",
+                    role="user",
+                )
+            ],
+            temperature=0.1,
+        )
+
+    if use_context_attributes:
+        with using_attributes(
+            session_id=session_id,
+            user_id=user_id,
+            metadata=metadata,
+            tags=tags,
+            prompt_template=prompt_template,
+            prompt_template_version=prompt_template_version,
+            prompt_template_variables=prompt_template_variables,
+        ):
+            response_stream = await mistral_stream()
+    else:
+        response_stream = await mistral_stream()
     response_content = ""
     async for chunk in response_stream:
         if chunk_content := chunk.choices[0].delta.content:
             response_content += chunk_content
 
     assert (
         response_content
@@ -724,58 +1012,94 @@
         OpenInferenceMimeTypeValues(attributes.pop(OUTPUT_MIME_TYPE))
         == OpenInferenceMimeTypeValues.JSON
     )
     assert attributes.pop(LLM_TOKEN_COUNT_PROMPT) == 15
     assert attributes.pop(LLM_TOKEN_COUNT_COMPLETION) == 109
     assert attributes.pop(LLM_TOKEN_COUNT_TOTAL) == 124
     assert attributes.pop(LLM_MODEL_NAME) == "mistral-large-latest"
+    if use_context_attributes:
+        _check_context_attributes(
+            attributes,
+            session_id,
+            user_id,
+            metadata,
+            tags,
+            prompt_template,
+            prompt_template_version,
+            prompt_template_variables,
+        )
     assert attributes == {}  # test should account for all span attributes
 
 
+@pytest.mark.parametrize("use_context_attributes", [False, True])
 def test_synchronous_streaming_chat_completions_with_tool_call_response_emits_expected_spans(
+    use_context_attributes: bool,
     mistral_sync_client: MistralClient,
     in_memory_span_exporter: InMemorySpanExporter,
     chat_stream_with_tool_call: AsyncByteStream,
     respx_mock: Any,
+    session_id: str,
+    user_id: str,
+    metadata: Dict[str, Any],
+    tags: List[str],
+    prompt_template: str,
+    prompt_template_version: str,
+    prompt_template_variables: Dict[str, Any],
 ) -> None:
     respx.post("https://api.mistral.ai/v1/chat/completions").mock(
         return_value=Response(
             200,
             stream=chat_stream_with_tool_call,
         )
     )
-    response_stream = mistral_sync_client.chat_stream(
-        model="mistral-large-latest",
-        tool_choice=ToolChoice.any,
-        tools=[
-            {
-                "type": "function",
-                "function": {
-                    "name": "get_weather",
-                    "description": "finds the weather for a given city",
-                    "parameters": {
-                        "type": "object",
-                        "properties": {
-                            "city": {
-                                "type": "string",
-                                "description": "The city to find the weather for, e.g. 'London'",
-                            }
-                        },
-                        "required": ["city"],
-                    },
+    tool = {
+        "type": "function",
+        "function": {
+            "name": "get_weather",
+            "description": "finds the weather for a given city",
+            "parameters": {
+                "type": "object",
+                "properties": {
+                    "city": {
+                        "type": "string",
+                        "description": "The city to find the weather for, e.g. 'London'",
+                    }
                 },
+                "required": ["city"],
             },
-        ],
-        messages=[
-            ChatMessage(
-                content="What's the weather like in San Francisco?",
-                role="user",
-            )
-        ],
-    )
+        },
+    }
+
+    def mistral_chat() -> Iterable[ChatCompletionStreamResponse]:
+        return mistral_sync_client.chat_stream(
+            model="mistral-large-latest",
+            tool_choice=ToolChoice.any,
+            tools=[tool],
+            messages=[
+                ChatMessage(
+                    content="What's the weather like in San Francisco?",
+                    role="user",
+                )
+            ],
+        )
+
+    if use_context_attributes:
+        with using_attributes(
+            session_id=session_id,
+            user_id=user_id,
+            metadata=metadata,
+            tags=tags,
+            prompt_template=prompt_template,
+            prompt_template_version=prompt_template_version,
+            prompt_template_variables=prompt_template_variables,
+        ):
+            response_stream = mistral_chat()
+    else:
+        response_stream = mistral_chat()
+
     for chunk in response_stream:
         delta = chunk.choices[0].delta
         assert not delta.content
         if tool_calls := delta.tool_calls:
             tool_call = tool_calls[0]
             assert tool_call.function.name == "get_weather"
             assert tool_call.function.arguments == '{"city": "San Francisco"}'
@@ -827,17 +1151,108 @@
         OpenInferenceMimeTypeValues(attributes.pop(OUTPUT_MIME_TYPE))
         == OpenInferenceMimeTypeValues.JSON
     )
     assert attributes.pop(LLM_TOKEN_COUNT_PROMPT) == 96
     assert attributes.pop(LLM_TOKEN_COUNT_COMPLETION) == 23
     assert attributes.pop(LLM_TOKEN_COUNT_TOTAL) == 119
     assert attributes.pop(LLM_MODEL_NAME) == "mistral-large-latest"
+    if use_context_attributes:
+        _check_context_attributes(
+            attributes,
+            session_id,
+            user_id,
+            metadata,
+            tags,
+            prompt_template,
+            prompt_template_version,
+            prompt_template_variables,
+        )
     assert attributes == {}  # test should account for all span attributes
 
 
+def _check_context_attributes(
+    attributes: Dict[str, Any],
+    session_id: str,
+    user_id: str,
+    metadata: Dict[str, Any],
+    tags: List[str],
+    prompt_template: str,
+    prompt_template_version: str,
+    prompt_template_variables: Dict[str, Any],
+) -> None:
+    assert attributes.pop(SESSION_ID, None) == session_id
+    assert attributes.pop(USER_ID, None) == user_id
+    attr_metadata = attributes.pop(METADATA, None)
+    assert attr_metadata is not None
+    assert isinstance(attr_metadata, str)  # must be json string
+    metadata_dict = json.loads(attr_metadata)
+    assert metadata_dict == metadata
+    attr_tags = attributes.pop(TAG_TAGS, None)
+    assert attr_tags is not None
+    assert len(attr_tags) == len(tags)
+    assert list(attr_tags) == tags
+    assert attributes.pop(SpanAttributes.LLM_PROMPT_TEMPLATE, None) == prompt_template
+    assert (
+        attributes.pop(SpanAttributes.LLM_PROMPT_TEMPLATE_VERSION, None) == prompt_template_version
+    )
+    assert attributes.pop(SpanAttributes.LLM_PROMPT_TEMPLATE_VARIABLES, None) == json.dumps(
+        prompt_template_variables
+    )
+
+
+@pytest.fixture()
+def session_id() -> str:
+    return "my-test-session-id"
+
+
+@pytest.fixture()
+def user_id() -> str:
+    return "my-test-user-id"
+
+
+@pytest.fixture()
+def metadata() -> Dict[str, Any]:
+    return {
+        "test-int": 1,
+        "test-str": "string",
+        "test-list": [1, 2, 3],
+        "test-dict": {
+            "key-1": "val-1",
+            "key-2": "val-2",
+        },
+    }
+
+
+@pytest.fixture()
+def tags() -> List[str]:
+    return ["tag-1", "tag-2"]
+
+
+@pytest.fixture
+def prompt_template() -> str:
+    return (
+        "This is a test prompt template with int {var_int}, "
+        "string {var_string}, and list {var_list}"
+    )
+
+
+@pytest.fixture
+def prompt_template_version() -> str:
+    return "v1.0"
+
+
+@pytest.fixture
+def prompt_template_variables() -> Dict[str, Any]:
+    return {
+        "var_int": 1,
+        "var_str": "2",
+        "var_list": [1, 2, 3],
+    }
+
+
 @pytest.fixture(scope="module")
 def mistral_sync_client() -> MistralClient:
     return MistralClient()
 
 
 @pytest.fixture(scope="module")
 def mistral_async_client() -> MistralAsyncClient:
@@ -1040,7 +1455,11 @@
 MESSAGE_NAME = MessageAttributes.MESSAGE_NAME
 TOOL_CALL_FUNCTION_NAME = ToolCallAttributes.TOOL_CALL_FUNCTION_NAME
 TOOL_CALL_FUNCTION_ARGUMENTS_JSON = ToolCallAttributes.TOOL_CALL_FUNCTION_ARGUMENTS_JSON
 EMBEDDING_EMBEDDINGS = SpanAttributes.EMBEDDING_EMBEDDINGS
 EMBEDDING_MODEL_NAME = SpanAttributes.EMBEDDING_MODEL_NAME
 EMBEDDING_VECTOR = EmbeddingAttributes.EMBEDDING_VECTOR
 EMBEDDING_TEXT = EmbeddingAttributes.EMBEDDING_TEXT
+SESSION_ID = SpanAttributes.SESSION_ID
+USER_ID = SpanAttributes.USER_ID
+METADATA = SpanAttributes.METADATA
+TAG_TAGS = SpanAttributes.TAG_TAGS
```

### Comparing `openinference_instrumentation_mistralai-0.0.5/LICENSE` & `openinference_instrumentation_mistralai-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_mistralai-0.0.5/README.md` & `openinference_instrumentation_mistralai-0.0.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # OpenInference Mistral AI Instrumentation
+[![PyPI Version](https://img.shields.io/pypi/v/openinference-instrumentation-mistralai.svg)](https://pypi.python.org/pypi/openinference-instrumentation-mistralai) 
 
 Python autoinstrumentation library for MistralAI's Python SDK.
 
 The traces emitted by this instrumentation are fully OpenTelemetry compatible and can be sent to an OpenTelemetry collector for viewing, such as [`arize-phoenix`](https://github.com/Arize-ai/phoenix)
 
 ## Installation
```

### Comparing `openinference_instrumentation_mistralai-0.0.5/PKG-INFO` & `openinference_instrumentation_mistralai-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.3
 Name: openinference-instrumentation-mistralai
-Version: 0.0.5
+Version: 0.0.6
 Summary: OpenInference Mistral AI Instrumentation
 Project-URL: Homepage, https://github.com/Arize-ai/openinference/tree/main/python/instrumentation/openinference-instrumentation-mistralai
 Author-email: OpenInference Authors <oss@arize.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: <3.13,>=3.8
+Requires-Python: <3.13,>=3.9
+Requires-Dist: openinference-instrumentation>=0.1.5
 Requires-Dist: openinference-semantic-conventions
 Requires-Dist: opentelemetry-api
 Requires-Dist: opentelemetry-instrumentation
 Requires-Dist: opentelemetry-semantic-conventions
 Requires-Dist: wrapt
 Provides-Extra: instruments
 Requires-Dist: mistralai; extra == 'instruments'
@@ -29,14 +29,15 @@
 Requires-Dist: opentelemetry-instrumentation-httpx; extra == 'test'
 Requires-Dist: opentelemetry-sdk; extra == 'test'
 Requires-Dist: pytest-asyncio; extra == 'test'
 Requires-Dist: respx; extra == 'test'
 Description-Content-Type: text/markdown
 
 # OpenInference Mistral AI Instrumentation
+[![PyPI Version](https://img.shields.io/pypi/v/openinference-instrumentation-mistralai.svg)](https://pypi.python.org/pypi/openinference-instrumentation-mistralai) 
 
 Python autoinstrumentation library for MistralAI's Python SDK.
 
 The traces emitted by this instrumentation are fully OpenTelemetry compatible and can be sent to an OpenTelemetry collector for viewing, such as [`arize-phoenix`](https://github.com/Arize-ai/phoenix)
 
 ## Installation
```

