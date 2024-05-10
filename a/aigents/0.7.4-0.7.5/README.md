# Comparing `tmp/aigents-0.7.4.tar.gz` & `tmp/aigents-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aigents-0.7.4.tar", max compression
+gzip compressed data, was "aigents-0.7.5.tar", max compression
```

## Comparing `aigents-0.7.4.tar` & `aigents-0.7.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    35149 2024-02-29 18:27:57.056767 aigents-0.7.4/LICENSE
--rw-r--r--   0        0        0     7402 2024-05-06 13:16:01.219386 aigents-0.7.4/README.md
--rw-r--r--   0        0        0     1028 2024-05-06 23:50:58.914168 aigents-0.7.4/pyproject.toml
--rw-r--r--   0        0        0      843 2024-05-06 12:53:46.596803 aigents-0.7.4/src/aigents/__init__.py
--rw-r--r--   0        0        0    19383 2024-03-15 16:50:10.476341 aigents-0.7.4/src/aigents/base.py
--rw-r--r--   0        0        0     1144 2024-05-03 19:26:39.754455 aigents-0.7.4/src/aigents/constants.py
--rw-r--r--   0        0        0      376 2024-05-05 20:28:48.665557 aigents-0.7.4/src/aigents/context/__init__.py
--rw-r--r--   0        0        0     2023 2024-05-06 17:26:15.624797 aigents-0.7.4/src/aigents/context/base.py
--rw-r--r--   0        0        0    13079 2024-05-06 23:50:53.193957 aigents-0.7.4/src/aigents/context/core.py
--rw-r--r--   0        0        0      337 2024-05-03 19:26:39.754455 aigents-0.7.4/src/aigents/context/errors.py
--rw-r--r--   0        0        0        0 2024-05-03 19:26:39.754455 aigents-0.7.4/src/aigents/context/nlp/__init__.py
--rw-r--r--   0        0        0     1098 2024-05-06 12:34:29.130871 aigents-0.7.4/src/aigents/context/nlp/base.py
--rw-r--r--   0        0        0      105 2024-05-03 19:26:39.754455 aigents-0.7.4/src/aigents/context/nlp/constants.py
--rw-r--r--   0        0        0      149 2024-05-03 19:26:39.754455 aigents-0.7.4/src/aigents/context/nlp/errors.py
--rw-r--r--   0        0        0    15091 2024-05-06 12:57:38.654315 aigents-0.7.4/src/aigents/context/nlp/processors.py
--rw-r--r--   0        0        0     1378 2024-05-05 20:28:48.665557 aigents-0.7.4/src/aigents/context/nlp/utils.py
--rw-r--r--   0        0        0     2502 2024-05-04 14:41:42.569117 aigents-0.7.4/src/aigents/context/utils.py
--rw-r--r--   0        0        0    31095 2024-03-14 11:18:28.044644 aigents-0.7.4/src/aigents/core.py
--rw-r--r--   0        0        0      188 2024-02-23 18:20:01.705095 aigents-0.7.4/src/aigents/data.py
--rw-r--r--   0        0        0      640 2024-02-29 13:47:18.770982 aigents-0.7.4/src/aigents/errors.py
--rw-r--r--   0        0        0    28395 2024-03-08 19:28:00.158179 aigents-0.7.4/src/aigents/prompts.py
--rw-r--r--   0        0        0     2822 2024-05-05 20:28:48.665557 aigents-0.7.4/src/aigents/settings.py
--rw-r--r--   0        0        0     6814 2024-05-03 19:26:39.754455 aigents-0.7.4/src/aigents/utils.py
--rw-r--r--   0        0        0     8675 1970-01-01 00:00:00.000000 aigents-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-02-29 18:27:57.056767 aigents-0.7.5/LICENSE
+-rw-r--r--   0        0        0     7402 2024-05-06 13:16:01.219386 aigents-0.7.5/README.md
+-rw-r--r--   0        0        0     1044 2024-05-09 19:39:39.988951 aigents-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0      843 2024-05-06 12:53:46.596803 aigents-0.7.5/src/aigents/__init__.py
+-rw-r--r--   0        0        0    19383 2024-03-15 16:50:10.476341 aigents-0.7.5/src/aigents/base.py
+-rw-r--r--   0        0        0     1144 2024-05-03 19:26:39.754455 aigents-0.7.5/src/aigents/constants.py
+-rw-r--r--   0        0        0      376 2024-05-05 20:28:48.665557 aigents-0.7.5/src/aigents/context/__init__.py
+-rw-r--r--   0        0        0     2023 2024-05-06 17:26:15.624797 aigents-0.7.5/src/aigents/context/base.py
+-rw-r--r--   0        0        0    13079 2024-05-06 23:50:53.193957 aigents-0.7.5/src/aigents/context/core.py
+-rw-r--r--   0        0        0      337 2024-05-03 19:26:39.754455 aigents-0.7.5/src/aigents/context/errors.py
+-rw-r--r--   0        0        0        0 2024-05-03 19:26:39.754455 aigents-0.7.5/src/aigents/context/nlp/__init__.py
+-rw-r--r--   0        0        0     1098 2024-05-06 12:34:29.130871 aigents-0.7.5/src/aigents/context/nlp/base.py
+-rw-r--r--   0        0        0      105 2024-05-03 19:26:39.754455 aigents-0.7.5/src/aigents/context/nlp/constants.py
+-rw-r--r--   0        0        0      149 2024-05-03 19:26:39.754455 aigents-0.7.5/src/aigents/context/nlp/errors.py
+-rw-r--r--   0        0        0    15197 2024-05-09 19:39:39.988951 aigents-0.7.5/src/aigents/context/nlp/processors.py
+-rw-r--r--   0        0        0     3101 2024-05-09 19:39:39.988951 aigents-0.7.5/src/aigents/context/nlp/utils.py
+-rw-r--r--   0        0        0     2502 2024-05-04 14:41:42.569117 aigents-0.7.5/src/aigents/context/utils.py
+-rw-r--r--   0        0        0    31095 2024-03-14 11:18:28.044644 aigents-0.7.5/src/aigents/core.py
+-rw-r--r--   0        0        0      188 2024-02-23 18:20:01.705095 aigents-0.7.5/src/aigents/data.py
+-rw-r--r--   0        0        0      640 2024-02-29 13:47:18.770982 aigents-0.7.5/src/aigents/errors.py
+-rw-r--r--   0        0        0    28395 2024-03-08 19:28:00.158179 aigents-0.7.5/src/aigents/prompts.py
+-rw-r--r--   0        0        0     2822 2024-05-05 20:28:48.665557 aigents-0.7.5/src/aigents/settings.py
+-rw-r--r--   0        0        0     6814 2024-05-03 19:26:39.754455 aigents-0.7.5/src/aigents/utils.py
+-rw-r--r--   0        0        0     8712 1970-01-01 00:00:00.000000 aigents-0.7.5/PKG-INFO
```

### Comparing `aigents-0.7.4/LICENSE` & `aigents-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aigents-0.7.4/README.md` & `aigents-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `aigents-0.7.4/pyproject.toml` & `aigents-0.7.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aigents"
-version = "0.7.4"
+version = "0.7.5"
 description = "Adapters for Large Language Models and Generative Pre-trained Transformers APIs"
 authors = ["Vagner Bessa <bessavagner@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 packages = [{include = "aigents", from = "src"}]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -22,14 +22,15 @@
 google-generativeai = "^0.3.2"
 tomlkit = "^0.12.4"
 pillow = "^10.2.0"
 g4f = {extras = ["all"], version = "^0.2.4.1"}
 spacy = "^3.7.4"
 pandas = "^2.2.2"
 scipy = "^1.13.0"
+nltk = "^3.8.1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "^8.22.1"
 ipykernel = "^6.29.2"
 tomlkit = "^0.12.3"
 
 [build-system]
```

### Comparing `aigents-0.7.4/src/aigents/__init__.py` & `aigents-0.7.5/src/aigents/__init__.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.4/src/aigents/base.py` & `aigents-0.7.5/src/aigents/base.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.4/src/aigents/constants.py` & `aigents-0.7.5/src/aigents/constants.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.4/src/aigents/context/base.py` & `aigents-0.7.5/src/aigents/context/base.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.4/src/aigents/context/core.py` & `aigents-0.7.5/src/aigents/context/core.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.4/src/aigents/context/nlp/base.py` & `aigents-0.7.5/src/aigents/context/nlp/base.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.4/src/aigents/context/nlp/processors.py` & `aigents-0.7.5/src/aigents/context/nlp/processors.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     MODELS,
     MODELS_EMBEDDING,
     EMBEDDINGS_COLUMNS,
 )
 from aigents.utils import get_encoding, run_async
 
 from .base import BaseTextProcessor
-from .utils import clean_text
+from .utils import clean_text, deep_clean
 from .errors import ProcessingError
 
 
 logger = logging.getLogger('standard')
 
 
 class TextProcessor(BaseTextProcessor):
@@ -78,18 +78,20 @@
                             openai_organization=None,
                             **kwargs) -> pd.DataFrame:
             Asynchronously obtain embeddings for chunks using OpenAI API.
 
         """
         super().__init__(*args, pipeline=pipeline, **kwargs)
 
-    def split(self, text, clean=True) -> List[str]:
+    def split(self, text, clean=True, deep_clean=True) -> List[str]:
         self.text = text
         if clean:
             self.text = clean_text(self.text)
+            if deep_clean:
+                self.text = deep_clean(self.text)
         self.doc = self.nlp(self.text)
         self.sequences = [sent.text for sent in self.doc.sents]
         return self.sequences
 
     def to_chunks(self,
                   text: str = None,
                   model: str = MODELS[0],
```

### Comparing `aigents-0.7.4/src/aigents/context/utils.py` & `aigents-0.7.5/src/aigents/context/utils.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.4/src/aigents/core.py` & `aigents-0.7.5/src/aigents/core.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.4/src/aigents/errors.py` & `aigents-0.7.5/src/aigents/errors.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.4/src/aigents/prompts.py` & `aigents-0.7.5/src/aigents/prompts.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.4/src/aigents/settings.py` & `aigents-0.7.5/src/aigents/settings.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.4/src/aigents/utils.py` & `aigents-0.7.5/src/aigents/utils.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.4/PKG-INFO` & `aigents-0.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aigents
-Version: 0.7.4
+Version: 0.7.5
 Summary: Adapters for Large Language Models and Generative Pre-trained Transformers APIs
 Home-page: https://github.com/bessavagner/aigents.git
 License: GPL-3.0-only
 Author: Vagner Bessa
 Author-email: bessavagner@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: g4f[all] (>=0.2.4.1,<0.3.0.0)
 Requires-Dist: google-generativeai (>=0.3.2,<0.4.0)
+Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: openai (>=1.12.0,<2.0.0)
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: pillow (>=10.2.0,<11.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: scipy (>=1.13.0,<2.0.0)
 Requires-Dist: spacy (>=3.7.4,<4.0.0)
 Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
```

