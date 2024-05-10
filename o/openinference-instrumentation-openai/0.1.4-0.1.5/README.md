# Comparing `tmp/openinference_instrumentation_openai-0.1.4.tar.gz` & `tmp/openinference_instrumentation_openai-0.1.5.tar.gz`

## Comparing `openinference_instrumentation_openai-0.1.4.tar` & `openinference_instrumentation_openai-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.4/src/openinference/instrumentation/openai/__init__.py
--rw-r--r--   0        0        0    17455 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.4/src/openinference/instrumentation/openai/_request.py
--rw-r--r--   0        0        0     7675 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.4/src/openinference/instrumentation/openai/_request_attributes_extractor.py
--rw-r--r--   0        0        0     9090 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.4/src/openinference/instrumentation/openai/_response_accumulator.py
--rw-r--r--   0        0        0    11240 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.4/src/openinference/instrumentation/openai/_response_attributes_extractor.py
--rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.4/src/openinference/instrumentation/openai/_stream.py
--rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.4/src/openinference/instrumentation/openai/_utils.py
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.4/src/openinference/instrumentation/openai/_with_span.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.4/src/openinference/instrumentation/openai/package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.4/src/openinference/instrumentation/openai/py.typed
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.4/src/openinference/instrumentation/openai/version.py
--rw-r--r--   0        0        0    30323 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.4/tests/openinference/instrumentation/openai/test_instrumentor.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.4/.gitignore
--rw-r--r--   0        0        0    10870 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.4/LICENSE
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.4/README.md
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.5/src/openinference/instrumentation/openai/__init__.py
+-rw-r--r--   0        0        0    17823 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.5/src/openinference/instrumentation/openai/_request.py
+-rw-r--r--   0        0        0     7675 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.5/src/openinference/instrumentation/openai/_request_attributes_extractor.py
+-rw-r--r--   0        0        0     9090 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.5/src/openinference/instrumentation/openai/_response_accumulator.py
+-rw-r--r--   0        0        0    11240 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.5/src/openinference/instrumentation/openai/_response_attributes_extractor.py
+-rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.5/src/openinference/instrumentation/openai/_stream.py
+-rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.5/src/openinference/instrumentation/openai/_utils.py
+-rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.5/src/openinference/instrumentation/openai/_with_span.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.5/src/openinference/instrumentation/openai/package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.5/src/openinference/instrumentation/openai/py.typed
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.5/src/openinference/instrumentation/openai/version.py
+-rw-r--r--   0        0        0    35160 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.5/tests/openinference/instrumentation/openai/test_instrumentor.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.5/.gitignore
+-rw-r--r--   0        0        0    10870 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.5/README.md
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.5/PKG-INFO
```

### Comparing `openinference_instrumentation_openai-0.1.4/src/openinference/instrumentation/openai/__init__.py` & `openinference_instrumentation_openai-0.1.5/src/openinference/instrumentation/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_openai-0.1.4/src/openinference/instrumentation/openai/_request.py` & `openinference_instrumentation_openai-0.1.5/src/openinference/instrumentation/openai/_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     Callable,
     Iterable,
     Iterator,
     Mapping,
     Tuple,
 )
 
+from openinference.instrumentation import get_attributes_from_context
 from openinference.instrumentation.openai._request_attributes_extractor import (
     _RequestAttributesExtractor,
 )
 from openinference.instrumentation.openai._response_accumulator import (
     _ChatCompletionAccumulator,
     _CompletionAccumulator,
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
         # Because OTEL has a default limit of 128 attributes, we split our attributes into
         # two tiers, where the addition of "extra_attributes" is deferred until the end
         # and only after the "attributes" are added.
         try:
             span = self._tracer.start_span(name=span_name, attributes=dict(attributes))
@@ -72,15 +74,19 @@
             span = INVALID_SPAN
         with trace_api.use_span(
             span,
             end_on_exit=False,
             record_exception=False,
             set_status_on_exception=False,
         ) as span:
-            yield _WithSpan(span=span, extra_attributes=dict(extra_attributes))
+            yield _WithSpan(
+                span=span,
+                context_attributes=dict(context_attributes),
+                extra_attributes=dict(extra_attributes),
+            )
 
 
 _RequestParameters: TypeAlias = Mapping[str, Any]
 
 
 class _WithOpenAI(ABC):
     __slots__ = (
@@ -261,14 +267,15 @@
             return wrapped(*args, **kwargs)
         with self._start_as_current_span(
             span_name=span_name,
             attributes=self._get_attributes_from_request(
                 cast_to=cast_to,
                 request_parameters=request_parameters,
             ),
+            context_attributes=get_attributes_from_context(),
             extra_attributes=self._get_extra_attributes_from_request(
                 cast_to=cast_to,
                 request_parameters=request_parameters,
             ),
         ) as with_span:
             try:
                 response = wrapped(*args, **kwargs)
@@ -314,14 +321,15 @@
             return await wrapped(*args, **kwargs)
         with self._start_as_current_span(
             span_name=span_name,
             attributes=self._get_attributes_from_request(
                 cast_to=cast_to,
                 request_parameters=request_parameters,
             ),
+            context_attributes=get_attributes_from_context(),
             extra_attributes=self._get_extra_attributes_from_request(
                 cast_to=cast_to,
                 request_parameters=request_parameters,
             ),
         ) as with_span:
             try:
                 response = await wrapped(*args, **kwargs)
```

### Comparing `openinference_instrumentation_openai-0.1.4/src/openinference/instrumentation/openai/_request_attributes_extractor.py` & `openinference_instrumentation_openai-0.1.5/src/openinference/instrumentation/openai/_request_attributes_extractor.py`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_openai-0.1.4/src/openinference/instrumentation/openai/_response_accumulator.py` & `openinference_instrumentation_openai-0.1.5/src/openinference/instrumentation/openai/_response_accumulator.py`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_openai-0.1.4/src/openinference/instrumentation/openai/_response_attributes_extractor.py` & `openinference_instrumentation_openai-0.1.5/src/openinference/instrumentation/openai/_response_attributes_extractor.py`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_openai-0.1.4/src/openinference/instrumentation/openai/_stream.py` & `openinference_instrumentation_openai-0.1.5/src/openinference/instrumentation/openai/_stream.py`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_openai-0.1.4/src/openinference/instrumentation/openai/_utils.py` & `openinference_instrumentation_openai-0.1.5/src/openinference/instrumentation/openai/_utils.py`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_openai-0.1.4/src/openinference/instrumentation/openai/_with_span.py` & `openinference_instrumentation_openai-0.1.5/src/openinference/instrumentation/openai/_with_span.py`

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

### Comparing `openinference_instrumentation_openai-0.1.4/tests/openinference/instrumentation/openai/test_instrumentor.py` & `openinference_instrumentation_openai-0.1.5/tests/openinference/instrumentation/openai/test_instrumentor.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     Tuple,
     Union,
     cast,
 )
 
 import pytest
 from httpx import AsyncByteStream, Response
+from openinference.instrumentation import using_attributes
 from openinference.instrumentation.openai import OpenAIInstrumentor
 from openinference.semconv.trace import (
     EmbeddingAttributes,
     MessageAttributes,
     OpenInferenceMimeTypeValues,
     OpenInferenceSpanKindValues,
     SpanAttributes,
@@ -49,24 +50,33 @@
         logger.addHandler(logging.StreamHandler())
 
 
 @pytest.mark.parametrize("is_async", [False, True])
 @pytest.mark.parametrize("is_raw", [False, True])
 @pytest.mark.parametrize("is_stream", [False, True])
 @pytest.mark.parametrize("status_code", [200, 400])
+@pytest.mark.parametrize("use_context_attributes", [False, True])
 def test_chat_completions(
     is_async: bool,
     is_raw: bool,
     is_stream: bool,
     status_code: int,
+    use_context_attributes: bool,
     respx_mock: MockRouter,
     in_memory_span_exporter: InMemorySpanExporter,
     completion_usage: Dict[str, Any],
     model_name: str,
     chat_completion_mock_stream: Tuple[List[bytes], List[Dict[str, Any]]],
+    session_id: str,
+    user_id: str,
+    metadata: Dict[str, Any],
+    tags: List[str],
+    prompt_template: str,
+    prompt_template_version: str,
+    prompt_template_variables: Dict[str, Any],
 ) -> None:
     input_messages: List[Dict[str, Any]] = get_messages()
     output_messages: List[Dict[str, Any]] = (
         chat_completion_mock_stream[1] if is_stream else get_messages()
     )
     invocation_parameters = {
         "stream": is_stream,
@@ -96,31 +106,50 @@
     openai = import_module("openai")
     completions = (
         openai.AsyncOpenAI(api_key="sk-").chat.completions
         if is_async
         else openai.OpenAI(api_key="sk-").chat.completions
     )
     create = completions.with_raw_response.create if is_raw else completions.create
-    with suppress(openai.BadRequestError):
-        if is_async:
 
-            async def task() -> None:
-                response = await create(**create_kwargs)
+    async def task() -> None:
+        response = await create(**create_kwargs)
+        response = response.parse() if is_raw else response
+        if is_stream:
+            async for _ in response:
+                pass
+
+    with suppress(openai.BadRequestError):
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
+                if is_async:
+                    asyncio.run(task())
+                else:
+                    response = create(**create_kwargs)
+                    response = response.parse() if is_raw else response
+                    if is_stream:
+                        for _ in response:
+                            pass
+        else:
+            if is_async:
+                asyncio.run(task())
+            else:
+                response = create(**create_kwargs)
                 response = response.parse() if is_raw else response
                 if is_stream:
-                    async for _ in response:
+                    for _ in response:
                         pass
-
-            asyncio.run(task())
-        else:
-            response = create(**create_kwargs)
-            response = response.parse() if is_raw else response
-            if is_stream:
-                for _ in response:
-                    pass
     spans = in_memory_span_exporter.get_finished_spans()
     assert len(spans) == 2  # first span should be from the httpx instrumentor
     span: ReadableSpan = spans[1]
     if status_code == 200:
         assert span.status.is_ok
         assert not span.status.description
     elif status_code == 400:
@@ -177,31 +206,51 @@
             assert attributes.pop(LLM_TOKEN_COUNT_PROMPT, None) == completion_usage["prompt_tokens"]
             assert (
                 attributes.pop(LLM_TOKEN_COUNT_COMPLETION, None)
                 == completion_usage["completion_tokens"]
             )
             # We left out model_name from our mock stream.
             assert attributes.pop(LLM_MODEL_NAME, None) == model_name
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
 
 
 @pytest.mark.parametrize("is_async", [False, True])
 @pytest.mark.parametrize("is_raw", [False, True])
 @pytest.mark.parametrize("is_stream", [False, True])
 @pytest.mark.parametrize("status_code", [200, 400])
+@pytest.mark.parametrize("use_context_attributes", [False, True])
 def test_completions(
     is_async: bool,
     is_raw: bool,
     is_stream: bool,
     status_code: int,
+    use_context_attributes: bool,
     respx_mock: MockRouter,
     in_memory_span_exporter: InMemorySpanExporter,
     completion_usage: Dict[str, Any],
     model_name: str,
     completion_mock_stream: Tuple[List[bytes], List[str]],
+    session_id: str,
+    user_id: str,
+    metadata: Dict[str, Any],
+    tags: List[str],
+    prompt_template: str,
+    prompt_template_version: str,
+    prompt_template_variables: Dict[str, Any],
 ) -> None:
     prompt: List[str] = get_texts()
     output_texts: List[str] = completion_mock_stream[1] if is_stream else get_texts()
     invocation_parameters = {
         "stream": is_stream,
         "model": randstr(),
         "temperature": random.random(),
@@ -229,31 +278,50 @@
     openai = import_module("openai")
     completions = (
         openai.AsyncOpenAI(api_key="sk-").completions
         if is_async
         else openai.OpenAI(api_key="sk-").completions
     )
     create = completions.with_raw_response.create if is_raw else completions.create
-    with suppress(openai.BadRequestError):
-        if is_async:
 
-            async def task() -> None:
-                response = await create(**create_kwargs)
+    async def task() -> None:
+        response = await create(**create_kwargs)
+        response = response.parse() if is_raw else response
+        if is_stream:
+            async for _ in response:
+                pass
+
+    with suppress(openai.BadRequestError):
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
+                if is_async:
+                    asyncio.run(task())
+                else:
+                    response = create(**create_kwargs)
+                    response = response.parse() if is_raw else response
+                    if is_stream:
+                        for _ in response:
+                            pass
+        else:
+            if is_async:
+                asyncio.run(task())
+            else:
+                response = create(**create_kwargs)
                 response = response.parse() if is_raw else response
                 if is_stream:
-                    async for _ in response:
+                    for _ in response:
                         pass
-
-            asyncio.run(task())
-        else:
-            response = create(**create_kwargs)
-            response = response.parse() if is_raw else response
-            if is_stream:
-                for _ in response:
-                    pass
     spans = in_memory_span_exporter.get_finished_spans()
     assert len(spans) == 2  # first span should be from the httpx instrumentor
     span: ReadableSpan = spans[1]
     if status_code == 200:
         assert span.status.is_ok
         assert not span.status.description
     elif status_code == 400:
@@ -282,14 +350,25 @@
             assert attributes.pop(LLM_TOKEN_COUNT_PROMPT, None) == completion_usage["prompt_tokens"]
             assert (
                 attributes.pop(LLM_TOKEN_COUNT_COMPLETION, None)
                 == completion_usage["completion_tokens"]
             )
             # We left out model_name from our mock stream.
             assert attributes.pop(LLM_MODEL_NAME, None) == model_name
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
 
 
 @pytest.mark.parametrize("is_async", [False, True])
 @pytest.mark.parametrize("is_raw", [False, True])
 @pytest.mark.parametrize("status_code", [200, 400])
 @pytest.mark.parametrize("encoding_format", ["float", "base64"])
@@ -384,14 +463,94 @@
             assert (
                 attributes.pop(f"{EMBEDDING_EMBEDDINGS}.{i}.{EMBEDDING_VECTOR}", None)
                 == embedding[1]
             )
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
 def in_memory_span_exporter() -> InMemorySpanExporter:
     return InMemorySpanExporter()
 
 
 @pytest.fixture(scope="module")
 def tracer_provider(in_memory_span_exporter: InMemorySpanExporter) -> trace_api.TracerProvider:
@@ -667,7 +826,11 @@
 MESSAGE_TOOL_CALLS = MessageAttributes.MESSAGE_TOOL_CALLS
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

### Comparing `openinference_instrumentation_openai-0.1.4/LICENSE` & `openinference_instrumentation_openai-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_openai-0.1.4/pyproject.toml` & `openinference_instrumentation_openai-0.1.5/pyproject.toml`

 * *Files 12% similar despite different names*

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
   "typing-extensions",
   "wrapt",
 ]
 
 [project.optional-dependencies]
 instruments = [
@@ -55,7 +56,36 @@
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

