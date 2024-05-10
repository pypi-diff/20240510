# Comparing `tmp/aigents-0.7.6.tar.gz` & `tmp/aigents-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aigents-0.7.6.tar", max compression
+gzip compressed data, was "aigents-0.7.8.tar", max compression
```

## Comparing `aigents-0.7.6.tar` & `aigents-0.7.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    35149 2024-02-29 18:27:57.056767 aigents-0.7.6/LICENSE
--rw-r--r--   0        0        0     7402 2024-05-06 13:16:01.219386 aigents-0.7.6/README.md
--rw-r--r--   0        0        0     1044 2024-05-10 11:54:56.740076 aigents-0.7.6/pyproject.toml
--rw-r--r--   0        0        0      843 2024-05-06 12:53:46.596803 aigents-0.7.6/src/aigents/__init__.py
--rw-r--r--   0        0        0    19383 2024-03-15 16:50:10.476341 aigents-0.7.6/src/aigents/base.py
--rw-r--r--   0        0        0     1144 2024-05-03 19:26:39.754455 aigents-0.7.6/src/aigents/constants.py
--rw-r--r--   0        0        0      376 2024-05-05 20:28:48.665557 aigents-0.7.6/src/aigents/context/__init__.py
--rw-r--r--   0        0        0     2023 2024-05-06 17:26:15.624797 aigents-0.7.6/src/aigents/context/base.py
--rw-r--r--   0        0        0    13079 2024-05-06 23:50:53.193957 aigents-0.7.6/src/aigents/context/core.py
--rw-r--r--   0        0        0      337 2024-05-03 19:26:39.754455 aigents-0.7.6/src/aigents/context/errors.py
--rw-r--r--   0        0        0        0 2024-05-03 19:26:39.754455 aigents-0.7.6/src/aigents/context/nlp/__init__.py
--rw-r--r--   0        0        0     1098 2024-05-06 12:34:29.130871 aigents-0.7.6/src/aigents/context/nlp/base.py
--rw-r--r--   0        0        0      105 2024-05-03 19:26:39.754455 aigents-0.7.6/src/aigents/context/nlp/constants.py
--rw-r--r--   0        0        0      149 2024-05-03 19:26:39.754455 aigents-0.7.6/src/aigents/context/nlp/errors.py
--rw-r--r--   0        0        0    15199 2024-05-10 11:54:45.136071 aigents-0.7.6/src/aigents/context/nlp/processors.py
--rw-r--r--   0        0        0     3101 2024-05-09 19:39:39.988951 aigents-0.7.6/src/aigents/context/nlp/utils.py
--rw-r--r--   0        0        0     2502 2024-05-04 14:41:42.569117 aigents-0.7.6/src/aigents/context/utils.py
--rw-r--r--   0        0        0    31095 2024-03-14 11:18:28.044644 aigents-0.7.6/src/aigents/core.py
--rw-r--r--   0        0        0      188 2024-02-23 18:20:01.705095 aigents-0.7.6/src/aigents/data.py
--rw-r--r--   0        0        0      640 2024-02-29 13:47:18.770982 aigents-0.7.6/src/aigents/errors.py
--rw-r--r--   0        0        0    28395 2024-03-08 19:28:00.158179 aigents-0.7.6/src/aigents/prompts.py
--rw-r--r--   0        0        0     2822 2024-05-05 20:28:48.665557 aigents-0.7.6/src/aigents/settings.py
--rw-r--r--   0        0        0     6814 2024-05-03 19:26:39.754455 aigents-0.7.6/src/aigents/utils.py
--rw-r--r--   0        0        0     8712 1970-01-01 00:00:00.000000 aigents-0.7.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-02-29 18:27:57.056767 aigents-0.7.8/LICENSE
+-rw-r--r--   0        0        0     7402 2024-05-06 13:16:01.219386 aigents-0.7.8/README.md
+-rw-r--r--   0        0        0     1044 2024-05-10 14:04:58.226122 aigents-0.7.8/pyproject.toml
+-rw-r--r--   0        0        0      843 2024-05-06 12:53:46.596803 aigents-0.7.8/src/aigents/__init__.py
+-rw-r--r--   0        0        0    19383 2024-03-15 16:50:10.476341 aigents-0.7.8/src/aigents/base.py
+-rw-r--r--   0        0        0     1144 2024-05-03 19:26:39.754455 aigents-0.7.8/src/aigents/constants.py
+-rw-r--r--   0        0        0      376 2024-05-05 20:28:48.665557 aigents-0.7.8/src/aigents/context/__init__.py
+-rw-r--r--   0        0        0     2023 2024-05-06 17:26:15.624797 aigents-0.7.8/src/aigents/context/base.py
+-rw-r--r--   0        0        0    13079 2024-05-06 23:50:53.193957 aigents-0.7.8/src/aigents/context/core.py
+-rw-r--r--   0        0        0      337 2024-05-03 19:26:39.754455 aigents-0.7.8/src/aigents/context/errors.py
+-rw-r--r--   0        0        0        0 2024-05-03 19:26:39.754455 aigents-0.7.8/src/aigents/context/nlp/__init__.py
+-rw-r--r--   0        0        0     1098 2024-05-06 12:34:29.130871 aigents-0.7.8/src/aigents/context/nlp/base.py
+-rw-r--r--   0        0        0      105 2024-05-03 19:26:39.754455 aigents-0.7.8/src/aigents/context/nlp/constants.py
+-rw-r--r--   0        0        0      149 2024-05-03 19:26:39.754455 aigents-0.7.8/src/aigents/context/nlp/errors.py
+-rw-r--r--   0        0        0    17637 2024-05-10 12:40:21.261161 aigents-0.7.8/src/aigents/context/nlp/processors.py
+-rw-r--r--   0        0        0     3101 2024-05-09 19:39:39.988951 aigents-0.7.8/src/aigents/context/nlp/utils.py
+-rw-r--r--   0        0        0     2502 2024-05-04 14:41:42.569117 aigents-0.7.8/src/aigents/context/utils.py
+-rw-r--r--   0        0        0    31095 2024-03-14 11:18:28.044644 aigents-0.7.8/src/aigents/core.py
+-rw-r--r--   0        0        0      188 2024-02-23 18:20:01.705095 aigents-0.7.8/src/aigents/data.py
+-rw-r--r--   0        0        0      640 2024-02-29 13:47:18.770982 aigents-0.7.8/src/aigents/errors.py
+-rw-r--r--   0        0        0    28395 2024-03-08 19:28:00.158179 aigents-0.7.8/src/aigents/prompts.py
+-rw-r--r--   0        0        0     2822 2024-05-05 20:28:48.665557 aigents-0.7.8/src/aigents/settings.py
+-rw-r--r--   0        0        0     6814 2024-05-03 19:26:39.754455 aigents-0.7.8/src/aigents/utils.py
+-rw-r--r--   0        0        0     8712 1970-01-01 00:00:00.000000 aigents-0.7.8/PKG-INFO
```

### Comparing `aigents-0.7.6/LICENSE` & `aigents-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aigents-0.7.6/README.md` & `aigents-0.7.8/README.md`

 * *Files identical despite different names*

### Comparing `aigents-0.7.6/pyproject.toml` & `aigents-0.7.8/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aigents"
-version = "0.7.6"
+version = "0.7.8"
 description = "Adapters for Large Language Models and Generative Pre-trained Transformers APIs"
 authors = ["Vagner Bessa <bessavagner@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 packages = [{include = "aigents", from = "src"}]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `aigents-0.7.6/src/aigents/__init__.py` & `aigents-0.7.8/src/aigents/__init__.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.6/src/aigents/base.py` & `aigents-0.7.8/src/aigents/base.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.6/src/aigents/constants.py` & `aigents-0.7.8/src/aigents/constants.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.6/src/aigents/context/base.py` & `aigents-0.7.8/src/aigents/context/base.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.6/src/aigents/context/core.py` & `aigents-0.7.8/src/aigents/context/core.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.6/src/aigents/context/nlp/base.py` & `aigents-0.7.8/src/aigents/context/nlp/base.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.6/src/aigents/context/nlp/processors.py` & `aigents-0.7.8/src/aigents/context/nlp/processors.py`

 * *Files 15% similar despite different names*

```diff
@@ -78,30 +78,53 @@
                             openai_organization=None,
                             **kwargs) -> pd.DataFrame:
             Asynchronously obtain embeddings for chunks using OpenAI API.
 
         """
         super().__init__(*args, pipeline=pipeline, **kwargs)
 
-    def split(self, text, clean=True, deep_clean_=True) -> List[str]:
+    def split(self,
+              text,
+              clean=True,
+              deep_clean_=True,
+              language="english",
+              n_grams_number=20,
+              n_grams_tolerance=2) -> List[str]:
         self.text = text
         if clean:
             self.text = clean_text(self.text)
             if deep_clean_:
-                self.text = deep_clean(self.text)
+                self.text = deep_clean(
+                    self.text,
+                    language=language,
+                    n_grams_number=n_grams_number,
+                    n_grams_tolerance=n_grams_tolerance
+                )
         self.doc = self.nlp(self.text)
         self.sequences = [sent.text for sent in self.doc.sents]
         return self.sequences
 
     def to_chunks(self,
                   text: str = None,
                   model: str = MODELS[0],
-                  max_tokens: int = 100) -> List[str]:
+                  max_tokens: int = 100,
+                  clean=True,
+                  deep_clean_=True,
+                  language="english",
+                  n_grams_number=20,
+                  n_grams_tolerance=2) -> List[str]:
         if text is not None:
-            self.split(text)
+            self.split(
+                text,
+                clean=clean,
+                deep_clean_=deep_clean_,
+                language=language,
+                n_grams_number=n_grams_number,
+                n_grams_tolerance=n_grams_tolerance,
+            )
         # group sentences semantically with a maximum number of tokens
         # using tiktoken to compute tokens
         # example maximum number of tokens
         chunks = []
         tokens = []
         current_chunk = []
         current_tokens = 0
@@ -126,29 +149,39 @@
         self.n_tokens = tokens
         return chunks
 
     def group_by_semantics(self,
                            data: str | List[str] = None,
                            model: str = MODELS[0],
                            max_tokens: int = 100,
-                           threshold: float = 0.8) -> List[str]:
+                           threshold: float = 0.8,
+                           clean=True,
+                           deep_clean_=True,
+                           language="english",
+                           n_grams_number=20,
+                           n_grams_tolerance=2) -> List[str]:
         
         if data is not None:
             if isinstance(data, list):
                 if not self.n_tokens:
                     encoding = get_encoding(model)
                     self.n_tokens = [
                         len(encoding.encode(chunk)) for chunk in data
                     ]
                 self.chunks = data
             else:
                 self.to_chunks(
                     text=data,
                     model=model,
                     max_tokens=max_tokens,
+                    clean=clean,
+                    deep_clean_=deep_clean_,
+                    language=language,
+                    n_grams_number=n_grams_number,
+                    n_grams_tolerance=n_grams_tolerance,
                 )
         
         docs = [self.nlp(sentence) for sentence in self.chunks]
         segments = []
         start_idx = 0
         end_idx = 1
         if len(self.chunks) == 0:
@@ -169,42 +202,62 @@
         self.segments = segments
         return segments
 
     def to_dataframe(self,
                      data: str | List[str] = None,
                      model: str = MODELS[0],
                      max_tokens: int = 120,
-                     threshold: float = 0.8) -> pd.DataFrame:
+                     threshold: float = 0.8,
+                     clean=True,
+                     deep_clean_=True,
+                     language="english",
+                     n_grams_number=20,
+                     n_grams_tolerance=2) -> pd.DataFrame:
         if data is not None:
             self.group_by_semantics(
                 data=data,
                 model=model,
                 max_tokens=max_tokens,
-                threshold=threshold
+                threshold=threshold,
+                clean=clean,
+                deep_clean_=deep_clean_,
+                language=language,
+                n_grams_number=n_grams_number,
+                n_grams_tolerance=n_grams_tolerance,
             )
 
         chunks = self.chunks
         n_tokens = self.n_tokens
         self.dataframe = pd.DataFrame({'chunks': chunks, 'n_tokens': n_tokens})
         return self.dataframe
 
     def embeddings(self,
                    data: str | List[str] | pd.DataFrame = None,
                    model: str = MODELS[0],
                    max_tokens: int = 120,
                    threshold: float = .8,
                    api_key=None,
                    organization=None,
-                   embedding_model='openai') -> pd.DataFrame:
+                   embedding_model='openai',
+                   clean=True,
+                   deep_clean_=True,
+                   language="english",
+                   n_grams_number=20,
+                   n_grams_tolerance=2) -> pd.DataFrame:
         if data is not None and not isinstance(data, pd.DataFrame):
             self.to_dataframe(
                 data=data,
                 model=model,
                 max_tokens=max_tokens,
-                threshold=threshold
+                threshold=threshold,
+                clean=clean,
+                deep_clean_=deep_clean_,
+                language=language,
+                n_grams_number=n_grams_number,
+                n_grams_tolerance=n_grams_tolerance,
             )
 
         embeddings = []
         def create_embedding(row):
             if 'openai' in embedding_model.lower():
                 client = OpenAIChatter(
                     api_key=api_key, organization=organization
@@ -239,21 +292,31 @@
                                data: str | List[str] | pd.DataFrame = None,
                                model: str = MODELS[0],
                                max_tokens: int = 120,
                                threshold: float = .8,
                                api_key=None,
                                organization=None,
                                embedding_model='openai',
+                               clean=True,
+                               deep_clean_=True,
+                               language="english",
+                               n_grams_number=20,
+                               n_grams_tolerance=2,
                                **kwargs) -> pd.DataFrame:
         if data is not None:
             self.to_dataframe(
                 data=data,
                 model=model,
                 max_tokens=max_tokens,
-                threshold=threshold
+                threshold=threshold,
+                clean=clean,
+                deep_clean_=deep_clean_,
+                language=language,
+                n_grams_number=n_grams_number,
+                n_grams_tolerance=n_grams_tolerance,
             )
 
         if 'gemini' in embedding_model.lower():
             GoogleChatter(api_key=api_key)
         tasks = []
         async def create_embedding_openai(row):
```

### Comparing `aigents-0.7.6/src/aigents/context/nlp/utils.py` & `aigents-0.7.8/src/aigents/context/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.6/src/aigents/context/utils.py` & `aigents-0.7.8/src/aigents/context/utils.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.6/src/aigents/core.py` & `aigents-0.7.8/src/aigents/core.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.6/src/aigents/errors.py` & `aigents-0.7.8/src/aigents/errors.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.6/src/aigents/prompts.py` & `aigents-0.7.8/src/aigents/prompts.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.6/src/aigents/settings.py` & `aigents-0.7.8/src/aigents/settings.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.6/src/aigents/utils.py` & `aigents-0.7.8/src/aigents/utils.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.6/PKG-INFO` & `aigents-0.7.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aigents
-Version: 0.7.6
+Version: 0.7.8
 Summary: Adapters for Large Language Models and Generative Pre-trained Transformers APIs
 Home-page: https://github.com/bessavagner/aigents.git
 License: GPL-3.0-only
 Author: Vagner Bessa
 Author-email: bessavagner@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

