# Comparing `tmp/ollama-0.1.9.tar.gz` & `tmp/ollama-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ollama-0.1.9.tar", max compression
+gzip compressed data, was "ollama-0.2.0.tar", max compression
```

## Comparing `ollama-0.1.9.tar` & `ollama-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1058 2024-04-26 00:13:08.529790 ollama-0.1.9/LICENSE
--rw-r--r--   0        0        0     3062 2024-04-26 00:13:08.529790 ollama-0.1.9/README.md
--rw-r--r--   0        0        0      720 2024-04-26 00:13:08.529790 ollama-0.1.9/ollama/__init__.py
--rw-r--r--   0        0        0    23836 2024-04-26 00:13:08.529790 ollama-0.1.9/ollama/_client.py
--rw-r--r--   0        0        0     3399 2024-04-26 00:13:08.529790 ollama-0.1.9/ollama/_types.py
--rw-r--r--   0        0        0      855 2024-04-26 00:13:18.773812 ollama-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     3778 1970-01-01 00:00:00.000000 ollama-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1058 2024-05-10 21:13:46.155142 ollama-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3421 2024-05-10 21:13:46.155142 ollama-0.2.0/README.md
+-rw-r--r--   0        0        0      720 2024-05-10 21:13:46.155142 ollama-0.2.0/ollama/__init__.py
+-rw-r--r--   0        0        0    23982 2024-05-10 21:13:46.155142 ollama-0.2.0/ollama/_client.py
+-rw-r--r--   0        0        0     3325 2024-05-10 21:13:46.155142 ollama-0.2.0/ollama/_types.py
+-rw-r--r--   0        0        0      855 2024-05-10 21:13:54.623158 ollama-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4137 1970-01-01 00:00:00.000000 ollama-0.2.0/PKG-INFO
```

### Comparing `ollama-0.1.9/LICENSE` & `ollama-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ollama-0.1.9/ollama/__init__.py` & `ollama-0.2.0/ollama/__init__.py`

 * *Files identical despite different names*

### Comparing `ollama-0.1.9/ollama/_client.py` & `ollama-0.2.0/ollama/_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,14 +251,15 @@
     )
 
   def create(
     self,
     model: str,
     path: Optional[Union[str, PathLike]] = None,
     modelfile: Optional[str] = None,
+    quantize: Optional[str] = None,
     stream: bool = False,
   ) -> Union[Mapping[str, Any], Iterator[Mapping[str, Any]]]:
     """
     Raises `ResponseError` if the request could not be fulfilled.
 
     Returns `ProgressResponse` if `stream` is `False`, otherwise returns a `ProgressResponse` generator.
     """
@@ -272,14 +273,15 @@
     return self._request_stream(
       'POST',
       '/api/create',
       json={
         'name': model,
         'modelfile': modelfile,
         'stream': stream,
+        'quantize': quantize,
       },
       stream=stream,
     )
 
   def _parse_modelfile(self, modelfile: str, base: Optional[Path] = None) -> str:
     base = Path.cwd() if base is None else base
 
@@ -470,15 +472,15 @@
 
   async def embeddings(
     self,
     model: str = '',
     prompt: str = '',
     options: Optional[Options] = None,
     keep_alive: Optional[Union[float, str]] = None,
-  ) -> Sequence[float]:
+  ) -> Mapping[str, Sequence[float]]:
     response = await self._request(
       'POST',
       '/api/embeddings',
       json={
         'model': model,
         'prompt': prompt,
         'options': options or {},
@@ -533,14 +535,15 @@
     )
 
   async def create(
     self,
     model: str,
     path: Optional[Union[str, PathLike]] = None,
     modelfile: Optional[str] = None,
+    quantize: Optional[str] = None,
     stream: bool = False,
   ) -> Union[Mapping[str, Any], AsyncIterator[Mapping[str, Any]]]:
     """
     Raises `ResponseError` if the request could not be fulfilled.
 
     Returns `ProgressResponse` if `stream` is `False`, otherwise returns a `ProgressResponse` generator.
     """
@@ -554,14 +557,15 @@
     return await self._request_stream(
       'POST',
       '/api/create',
       json={
         'name': model,
         'modelfile': modelfile,
         'stream': stream,
+        'quantize': quantize,
       },
       stream=stream,
     )
 
   async def _parse_modelfile(self, modelfile: str, base: Optional[Path] = None) -> str:
     base = Path.cwd() if base is None else base
```

### Comparing `ollama-0.1.9/ollama/_types.py` & `ollama-0.2.0/ollama/_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,26 +91,23 @@
 
 
 class Options(TypedDict, total=False):
   # load time options
   numa: bool
   num_ctx: int
   num_batch: int
-  num_gqa: int
   num_gpu: int
   main_gpu: int
   low_vram: bool
   f16_kv: bool
   logits_all: bool
   vocab_only: bool
   use_mmap: bool
   use_mlock: bool
   embedding_only: bool
-  rope_frequency_base: float
-  rope_frequency_scale: float
   num_thread: int
 
   # runtime options
   num_keep: int
   seed: int
   num_predict: int
   top_k: int
```

### Comparing `ollama-0.1.9/pyproject.toml` & `ollama-0.2.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ollama"
-version = "0.1.9"
+version = "0.2.0"
 description = "The official Python client for Ollama."
 authors = ["Ollama <hello@ollama.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://ollama.ai"
 repository = "https://github.com/jmorganca/ollama-python"
```

