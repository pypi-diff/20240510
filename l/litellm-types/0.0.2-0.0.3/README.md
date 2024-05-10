# Comparing `tmp/litellm_types-0.0.2.tar.gz` & `tmp/litellm_types-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm_types-0.0.2.tar", last modified: Mon May  6 12:28:46 2024, max compression
+gzip compressed data, was "litellm_types-0.0.3.tar", last modified: Fri May 10 08:30:58 2024, max compression
```

## Comparing `litellm_types-0.0.2.tar` & `litellm_types-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-05-06 12:28:46.823899 litellm_types-0.0.2/
--rw-r--r--   0 salamanderxing   (501) staff       (20)      128 2024-05-06 12:28:46.823709 litellm_types-0.0.2/PKG-INFO
-drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-05-06 12:28:46.822887 litellm_types-0.0.2/litellm_types/
--rw-r--r--   0 salamanderxing   (501) staff       (20)        2 2024-05-05 16:42:41.000000 litellm_types-0.0.2/litellm_types/__init__.py
--rw-r--r--   0 salamanderxing   (501) staff       (20)     5043 2024-05-05 19:19:35.000000 litellm_types-0.0.2/litellm_types/completion.py
--rw-r--r--   0 salamanderxing   (501) staff       (20)      134 2024-05-05 16:26:12.000000 litellm_types-0.0.2/litellm_types/document.py
--rw-r--r--   0 salamanderxing   (501) staff       (20)     1341 2024-05-05 19:21:12.000000 litellm_types-0.0.2/litellm_types/messages.py
--rw-r--r--   0 salamanderxing   (501) staff       (20)      293 2024-05-05 16:23:45.000000 litellm_types-0.0.2/litellm_types/prompt.py
-drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-05-06 12:28:46.823532 litellm_types-0.0.2/litellm_types.egg-info/
--rw-r--r--   0 salamanderxing   (501) staff       (20)      128 2024-05-06 12:28:46.000000 litellm_types-0.0.2/litellm_types.egg-info/PKG-INFO
--rw-r--r--   0 salamanderxing   (501) staff       (20)      322 2024-05-06 12:28:46.000000 litellm_types-0.0.2/litellm_types.egg-info/SOURCES.txt
--rw-r--r--   0 salamanderxing   (501) staff       (20)        1 2024-05-06 12:28:46.000000 litellm_types-0.0.2/litellm_types.egg-info/dependency_links.txt
--rw-r--r--   0 salamanderxing   (501) staff       (20)       26 2024-05-06 12:28:46.000000 litellm_types-0.0.2/litellm_types.egg-info/requires.txt
--rw-r--r--   0 salamanderxing   (501) staff       (20)       14 2024-05-06 12:28:46.000000 litellm_types-0.0.2/litellm_types.egg-info/top_level.txt
--rw-r--r--   0 salamanderxing   (501) staff       (20)       38 2024-05-06 12:28:46.823945 litellm_types-0.0.2/setup.cfg
--rw-r--r--   0 salamanderxing   (501) staff       (20)      263 2024-05-06 12:28:34.000000 litellm_types-0.0.2/setup.py
+drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-05-10 08:30:58.542448 litellm_types-0.0.3/
+-rw-r--r--   0 salamanderxing   (501) staff       (20)    11357 2024-05-06 12:34:17.000000 litellm_types-0.0.3/LICENSE
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      150 2024-05-10 08:30:58.542270 litellm_types-0.0.3/PKG-INFO
+drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-05-10 08:30:58.541430 litellm_types-0.0.3/litellm_types/
+-rw-r--r--   0 salamanderxing   (501) staff       (20)        2 2024-05-05 16:42:41.000000 litellm_types-0.0.3/litellm_types/__init__.py
+-rw-r--r--   0 salamanderxing   (501) staff       (20)     5030 2024-05-06 12:30:27.000000 litellm_types-0.0.3/litellm_types/completion.py
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      134 2024-05-05 16:26:12.000000 litellm_types-0.0.3/litellm_types/document.py
+-rw-r--r--   0 salamanderxing   (501) staff       (20)     1341 2024-05-05 19:21:12.000000 litellm_types-0.0.3/litellm_types/messages.py
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      293 2024-05-05 16:23:45.000000 litellm_types-0.0.3/litellm_types/prompt.py
+drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-05-10 08:30:58.542085 litellm_types-0.0.3/litellm_types.egg-info/
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      150 2024-05-10 08:30:58.000000 litellm_types-0.0.3/litellm_types.egg-info/PKG-INFO
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      330 2024-05-10 08:30:58.000000 litellm_types-0.0.3/litellm_types.egg-info/SOURCES.txt
+-rw-r--r--   0 salamanderxing   (501) staff       (20)        1 2024-05-10 08:30:58.000000 litellm_types-0.0.3/litellm_types.egg-info/dependency_links.txt
+-rw-r--r--   0 salamanderxing   (501) staff       (20)       26 2024-05-10 08:30:58.000000 litellm_types-0.0.3/litellm_types.egg-info/requires.txt
+-rw-r--r--   0 salamanderxing   (501) staff       (20)       14 2024-05-10 08:30:58.000000 litellm_types-0.0.3/litellm_types.egg-info/top_level.txt
+-rw-r--r--   0 salamanderxing   (501) staff       (20)       38 2024-05-10 08:30:58.542484 litellm_types-0.0.3/setup.cfg
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      263 2024-05-10 08:30:52.000000 litellm_types-0.0.3/setup.py
```

### Comparing `litellm_types-0.0.2/litellm_types/completion.py` & `litellm_types-0.0.3/litellm_types/completion.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from rich import print
 from .messages import AssistantMessage, AnyMessage
 
 
 ACompletion = Callable[[list[AnyMessage]], Awaitable[AssistantMessage]]
 
 
-def get_acompletion_with_retries(
+def get_acompletion(
     model: str,
     # Optional OpenAI params: see https://platform.openai.com/docs/api-reference/chat/create
     timeout: float | str | httpx.Timeout | None = None,
     temperature: float | None = None,
     top_p: float | None = None,
     n: int | None = None,
     stream: bool | None = None,
```

### Comparing `litellm_types-0.0.2/litellm_types/messages.py` & `litellm_types-0.0.3/litellm_types/messages.py`

 * *Files identical despite different names*

