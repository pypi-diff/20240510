# Comparing `tmp/aigents-0.7.8.tar.gz` & `tmp/aigents-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aigents-0.7.8.tar", max compression
+gzip compressed data, was "aigents-0.7.9.tar", max compression
```

## Comparing `aigents-0.7.8.tar` & `aigents-0.7.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    35149 2024-02-29 18:27:57.056767 aigents-0.7.8/LICENSE
--rw-r--r--   0        0        0     7402 2024-05-06 13:16:01.219386 aigents-0.7.8/README.md
--rw-r--r--   0        0        0     1044 2024-05-10 14:04:58.226122 aigents-0.7.8/pyproject.toml
--rw-r--r--   0        0        0      843 2024-05-06 12:53:46.596803 aigents-0.7.8/src/aigents/__init__.py
--rw-r--r--   0        0        0    19383 2024-03-15 16:50:10.476341 aigents-0.7.8/src/aigents/base.py
--rw-r--r--   0        0        0     1144 2024-05-03 19:26:39.754455 aigents-0.7.8/src/aigents/constants.py
--rw-r--r--   0        0        0      376 2024-05-05 20:28:48.665557 aigents-0.7.8/src/aigents/context/__init__.py
--rw-r--r--   0        0        0     2023 2024-05-06 17:26:15.624797 aigents-0.7.8/src/aigents/context/base.py
--rw-r--r--   0        0        0    13079 2024-05-06 23:50:53.193957 aigents-0.7.8/src/aigents/context/core.py
--rw-r--r--   0        0        0      337 2024-05-03 19:26:39.754455 aigents-0.7.8/src/aigents/context/errors.py
--rw-r--r--   0        0        0        0 2024-05-03 19:26:39.754455 aigents-0.7.8/src/aigents/context/nlp/__init__.py
--rw-r--r--   0        0        0     1098 2024-05-06 12:34:29.130871 aigents-0.7.8/src/aigents/context/nlp/base.py
--rw-r--r--   0        0        0      105 2024-05-03 19:26:39.754455 aigents-0.7.8/src/aigents/context/nlp/constants.py
--rw-r--r--   0        0        0      149 2024-05-03 19:26:39.754455 aigents-0.7.8/src/aigents/context/nlp/errors.py
--rw-r--r--   0        0        0    17637 2024-05-10 12:40:21.261161 aigents-0.7.8/src/aigents/context/nlp/processors.py
--rw-r--r--   0        0        0     3101 2024-05-09 19:39:39.988951 aigents-0.7.8/src/aigents/context/nlp/utils.py
--rw-r--r--   0        0        0     2502 2024-05-04 14:41:42.569117 aigents-0.7.8/src/aigents/context/utils.py
--rw-r--r--   0        0        0    31095 2024-03-14 11:18:28.044644 aigents-0.7.8/src/aigents/core.py
--rw-r--r--   0        0        0      188 2024-02-23 18:20:01.705095 aigents-0.7.8/src/aigents/data.py
--rw-r--r--   0        0        0      640 2024-02-29 13:47:18.770982 aigents-0.7.8/src/aigents/errors.py
--rw-r--r--   0        0        0    28395 2024-03-08 19:28:00.158179 aigents-0.7.8/src/aigents/prompts.py
--rw-r--r--   0        0        0     2822 2024-05-05 20:28:48.665557 aigents-0.7.8/src/aigents/settings.py
--rw-r--r--   0        0        0     6814 2024-05-03 19:26:39.754455 aigents-0.7.8/src/aigents/utils.py
--rw-r--r--   0        0        0     8712 1970-01-01 00:00:00.000000 aigents-0.7.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-02-29 18:27:57.056767 aigents-0.7.9/LICENSE
+-rw-r--r--   0        0        0     7402 2024-05-06 13:16:01.219386 aigents-0.7.9/README.md
+-rw-r--r--   0        0        0     1044 2024-05-10 17:25:02.079544 aigents-0.7.9/pyproject.toml
+-rw-r--r--   0        0        0      843 2024-05-06 12:53:46.596803 aigents-0.7.9/src/aigents/__init__.py
+-rw-r--r--   0        0        0    19383 2024-03-15 16:50:10.476341 aigents-0.7.9/src/aigents/base.py
+-rw-r--r--   0        0        0     1144 2024-05-03 19:26:39.754455 aigents-0.7.9/src/aigents/constants.py
+-rw-r--r--   0        0        0      376 2024-05-05 20:28:48.665557 aigents-0.7.9/src/aigents/context/__init__.py
+-rw-r--r--   0        0        0     2023 2024-05-06 17:26:15.624797 aigents-0.7.9/src/aigents/context/base.py
+-rw-r--r--   0        0        0    13079 2024-05-06 23:50:53.193957 aigents-0.7.9/src/aigents/context/core.py
+-rw-r--r--   0        0        0      337 2024-05-03 19:26:39.754455 aigents-0.7.9/src/aigents/context/errors.py
+-rw-r--r--   0        0        0        0 2024-05-03 19:26:39.754455 aigents-0.7.9/src/aigents/context/nlp/__init__.py
+-rw-r--r--   0        0        0     1098 2024-05-06 12:34:29.130871 aigents-0.7.9/src/aigents/context/nlp/base.py
+-rw-r--r--   0        0        0      105 2024-05-03 19:26:39.754455 aigents-0.7.9/src/aigents/context/nlp/constants.py
+-rw-r--r--   0        0        0      149 2024-05-03 19:26:39.754455 aigents-0.7.9/src/aigents/context/nlp/errors.py
+-rw-r--r--   0        0        0    17637 2024-05-10 12:40:21.261161 aigents-0.7.9/src/aigents/context/nlp/processors.py
+-rw-r--r--   0        0        0     3101 2024-05-09 19:39:39.988951 aigents-0.7.9/src/aigents/context/nlp/utils.py
+-rw-r--r--   0        0        0     4020 2024-05-10 17:24:48.875825 aigents-0.7.9/src/aigents/context/utils.py
+-rw-r--r--   0        0        0    31095 2024-03-14 11:18:28.044644 aigents-0.7.9/src/aigents/core.py
+-rw-r--r--   0        0        0      188 2024-02-23 18:20:01.705095 aigents-0.7.9/src/aigents/data.py
+-rw-r--r--   0        0        0      640 2024-02-29 13:47:18.770982 aigents-0.7.9/src/aigents/errors.py
+-rw-r--r--   0        0        0    28395 2024-03-08 19:28:00.158179 aigents-0.7.9/src/aigents/prompts.py
+-rw-r--r--   0        0        0     2822 2024-05-05 20:28:48.665557 aigents-0.7.9/src/aigents/settings.py
+-rw-r--r--   0        0        0     6814 2024-05-03 19:26:39.754455 aigents-0.7.9/src/aigents/utils.py
+-rw-r--r--   0        0        0     8712 1970-01-01 00:00:00.000000 aigents-0.7.9/PKG-INFO
```

### Comparing `aigents-0.7.8/LICENSE` & `aigents-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aigents-0.7.8/README.md` & `aigents-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `aigents-0.7.8/pyproject.toml` & `aigents-0.7.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aigents"
-version = "0.7.8"
+version = "0.7.9"
 description = "Adapters for Large Language Models and Generative Pre-trained Transformers APIs"
 authors = ["Vagner Bessa <bessavagner@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 packages = [{include = "aigents", from = "src"}]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `aigents-0.7.8/src/aigents/__init__.py` & `aigents-0.7.9/src/aigents/__init__.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.8/src/aigents/base.py` & `aigents-0.7.9/src/aigents/base.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.8/src/aigents/constants.py` & `aigents-0.7.9/src/aigents/constants.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.8/src/aigents/context/base.py` & `aigents-0.7.9/src/aigents/context/base.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.8/src/aigents/context/core.py` & `aigents-0.7.9/src/aigents/context/core.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.8/src/aigents/context/nlp/base.py` & `aigents-0.7.9/src/aigents/context/nlp/base.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.8/src/aigents/context/nlp/processors.py` & `aigents-0.7.9/src/aigents/context/nlp/processors.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.8/src/aigents/context/nlp/utils.py` & `aigents-0.7.9/src/aigents/context/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.8/src/aigents/context/utils.py` & `aigents-0.7.9/src/aigents/context/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,61 +9,101 @@
 
 def to_embeddings(
         text: str,
         pipeline: str = PIPE_LINES[-1],
         max_tokens=120,
         threshold=0.8,
         embedding_model='openai',
+        clean: bool = True,
+        deep_clean_: bool = True,
+        language: str = "english",
+        n_grams_number: int = 20,
+        n_grams_tolerance: int = 2,
 ) -> DataFrame:
     return TextProcessor(pipeline=pipeline).embeddings(
         text,
         max_tokens=max_tokens,
         threshold=threshold,
         embedding_model=embedding_model,
+        clean=clean,
+        deep_clean_=deep_clean_,
+        language=language,
+        n_grams_number=n_grams_number,
+        n_grams_tolerance=n_grams_tolerance,
     )
 
 
 async def to_embeddings_async(
         text: str,
         pipeline: str = PIPE_LINES[-1],
         max_tokens=120,
         threshold=0.8,
         embedding_model='openai',
+        clean: bool = True,
+        deep_clean_: bool = True,
+        language: str = "english",
+        n_grams_number: int = 20,
+        n_grams_tolerance: int = 2,
 ) -> DataFrame:
     return await TextProcessor(pipeline=pipeline).async_embeddings(
         text,
         max_tokens=max_tokens,
         threshold=threshold,
         embedding_model=embedding_model,
+        clean=clean,
+        deep_clean_=deep_clean_,
+        language=language,
+        n_grams_number=n_grams_number,
+        n_grams_tolerance=n_grams_tolerance,
     )
 
 
 def to_embeddings_pt(text: str,
                      max_tokens=120,
                      threshold=0.8,
-                     embedding_model='openai',) -> DataFrame:
+                     embedding_model='openai',
+                     clean: bool = True,
+                     deep_clean_: bool = True,
+                     language: str = "english",
+                     n_grams_number: int = 20,
+                     n_grams_tolerance: int = 2,) -> DataFrame:
     return to_embeddings(
         text,
         pipeline=PIPE_LINES[0],
         max_tokens=max_tokens,
         threshold=threshold,
         embedding_model=embedding_model,
+        clean=clean,
+        deep_clean_=deep_clean_,
+        language=language,
+        n_grams_number=n_grams_number,
+        n_grams_tolerance=n_grams_tolerance,
     )
 
 
 async def to_embeddings_pt_async(text: str,
                                  max_tokens=120,
                                  threshold=0.8,
-                                 embedding_model='openai',) -> DataFrame:
+                                 embedding_model='openai',
+                                 clean: bool = True,
+                                 deep_clean_: bool = True,
+                                 language: str = "english",
+                                 n_grams_number: int = 20,
+                                 n_grams_tolerance: int = 2,) -> DataFrame:
     return await to_embeddings_async(
         text,
         pipeline=PIPE_LINES[0],
         max_tokens=max_tokens,
         threshold=threshold,
         embedding_model=embedding_model,
+        clean=clean,
+        deep_clean_=deep_clean_,
+        language=language,
+        n_grams_number=n_grams_number,
+        n_grams_tolerance=n_grams_tolerance,
     )
 
 def distances_from_embeddings(
     query_embedding: List[float],
     embeddings: List[List[float]],
     distance_metric="cosine",
 ) -> List[List]:
```

### Comparing `aigents-0.7.8/src/aigents/core.py` & `aigents-0.7.9/src/aigents/core.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.8/src/aigents/errors.py` & `aigents-0.7.9/src/aigents/errors.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.8/src/aigents/prompts.py` & `aigents-0.7.9/src/aigents/prompts.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.8/src/aigents/settings.py` & `aigents-0.7.9/src/aigents/settings.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.8/src/aigents/utils.py` & `aigents-0.7.9/src/aigents/utils.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.8/PKG-INFO` & `aigents-0.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aigents
-Version: 0.7.8
+Version: 0.7.9
 Summary: Adapters for Large Language Models and Generative Pre-trained Transformers APIs
 Home-page: https://github.com/bessavagner/aigents.git
 License: GPL-3.0-only
 Author: Vagner Bessa
 Author-email: bessavagner@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

