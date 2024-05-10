# Comparing `tmp/langfun-0.0.2.dev20240508.tar.gz` & `tmp/langfun-0.0.2.dev20240509.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langfun-0.0.2.dev20240508.tar", last modified: Wed May  8 08:03:49 2024, max compression
+gzip compressed data, was "langfun-0.0.2.dev20240509.tar", last modified: Thu May  9 08:03:36 2024, max compression
```

## Comparing `langfun-0.0.2.dev20240508.tar` & `langfun-0.0.2.dev20240509.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:49.385272 langfun-0.0.2.dev20240508/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-08 08:03:49.385272 langfun-0.0.2.dev20240508/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:49.365272 langfun-0.0.2.dev20240508/langfun/
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:49.373272 langfun-0.0.2.dev20240508/langfun/core/
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:49.373272 langfun-0.0.2.dev20240508/langfun/core/coding/
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/coding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:49.373272 langfun-0.0.2.dev20240508/langfun/core/coding/python/
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/coding/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/coding/python/correction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/coding/python/correction_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/coding/python/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/coding/python/errors_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/coding/python/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/coding/python/execution_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/coding/python/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/coding/python/generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/coding/python/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/coding/python/parsing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/coding/python/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/coding/python/permissions_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/component_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/concurrent_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/console_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:49.377272 langfun-0.0.2.dev20240508/langfun/core/eval/
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    74268 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/eval/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    26743 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/eval/base_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9782 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/eval/matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/eval/matching_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/eval/patching.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/eval/patching_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/eval/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/eval/scoring_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11060 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/langfunc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8501 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/langfunc_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    20202 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/language_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    19548 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/language_model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:49.377272 langfun-0.0.2.dev20240508/langfun/core/llms/
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/llms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/llms/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/llms/anthropic_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:49.377272 langfun-0.0.2.dev20240508/langfun/core/llms/cache/
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/llms/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/llms/cache/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/llms/cache/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/llms/cache/in_memory_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/llms/fake.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/llms/fake_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8624 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/llms/google_genai.py
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/llms/google_genai_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/llms/groq.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/llms/groq_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/llms/llama_cpp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/llms/llama_cpp_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13257 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/llms/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)    14854 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/llms/openai_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:49.381272 langfun-0.0.2.dev20240508/langfun/core/memories/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/memories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/memories/conversation_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/memories/conversation_history_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    15734 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/message_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:49.381272 langfun-0.0.2.dev20240508/langfun/core/modalities/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/modalities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/modalities/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/modalities/image_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/modalities/mime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/modalities/mime_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/modalities/video.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/modalities/video_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/modality.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/modality_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/natural_language.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/natural_language_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/sampling_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:49.385272 langfun-0.0.2.dev20240508/langfun/core/structured/
--rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/structured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/structured/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)    19273 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/structured/completion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/structured/description.py
--rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/structured/description_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/structured/function_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/structured/function_generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    12253 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/structured/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/structured/mapping_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/structured/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    20895 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/structured/parsing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/structured/prompting.py
--rw-r--r--   0 runner    (1001) docker     (127)    21700 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/structured/prompting_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    25818 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/structured/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/structured/schema_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/structured/schema_generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    23078 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/structured/schema_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/structured/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/structured/scoring_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/subscription_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    22284 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/template.py
--rw-r--r--   0 runner    (1001) docker     (127)    15464 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/template_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:49.385272 langfun-0.0.2.dev20240508/langfun/core/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/templates/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/templates/completion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/templates/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/templates/conversation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/templates/demonstration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/templates/demonstration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/templates/selfplay.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/templates/selfplay_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/text_formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/text_formatting_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:49.385272 langfun-0.0.2.dev20240508/langfun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-08 08:03:49.000000 langfun-0.0.2.dev20240508/langfun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-05-08 08:03:49.000000 langfun-0.0.2.dev20240508/langfun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 08:03:49.000000 langfun-0.0.2.dev20240508/langfun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-08 08:03:49.000000 langfun-0.0.2.dev20240508/langfun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 08:03:49.000000 langfun-0.0.2.dev20240508/langfun.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 08:03:49.385272 langfun-0.0.2.dev20240508/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:03:36.547569 langfun-0.0.2.dev20240509/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-09 08:03:36.547569 langfun-0.0.2.dev20240509/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:03:36.531569 langfun-0.0.2.dev20240509/langfun/
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:03:36.535569 langfun-0.0.2.dev20240509/langfun/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:03:36.535569 langfun-0.0.2.dev20240509/langfun/core/coding/
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/coding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:03:36.539569 langfun-0.0.2.dev20240509/langfun/core/coding/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/coding/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/coding/python/correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/coding/python/correction_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/coding/python/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/coding/python/errors_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/coding/python/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/coding/python/execution_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/coding/python/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/coding/python/generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/coding/python/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/coding/python/parsing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/coding/python/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/coding/python/permissions_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/component_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/concurrent_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/console_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:03:36.539569 langfun-0.0.2.dev20240509/langfun/core/eval/
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74268 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/eval/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26743 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/eval/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9782 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/eval/matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/eval/matching_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/eval/patching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/eval/patching_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/eval/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/eval/scoring_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11060 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/langfunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8501 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/langfunc_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20202 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/language_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19548 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/language_model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:03:36.539569 langfun-0.0.2.dev20240509/langfun/core/llms/
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/llms/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/llms/anthropic_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:03:36.543569 langfun-0.0.2.dev20240509/langfun/core/llms/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/llms/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/llms/cache/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/llms/cache/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/llms/cache/in_memory_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/llms/fake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/llms/fake_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8624 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/llms/google_genai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/llms/google_genai_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/llms/groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/llms/groq_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/llms/llama_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/llms/llama_cpp_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13286 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/llms/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14854 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/llms/openai_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:03:36.543569 langfun-0.0.2.dev20240509/langfun/core/memories/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/memories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/memories/conversation_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/memories/conversation_history_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15734 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/message_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:03:36.543569 langfun-0.0.2.dev20240509/langfun/core/modalities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/modalities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/modalities/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/modalities/image_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/modalities/mime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/modalities/mime_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/modalities/video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/modalities/video_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/modality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/modality_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/natural_language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/natural_language_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/sampling_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:03:36.547569 langfun-0.0.2.dev20240509/langfun/core/structured/
+-rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/structured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/structured/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19273 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/structured/completion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/structured/description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/structured/description_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/structured/function_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/structured/function_generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12253 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/structured/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/structured/mapping_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/structured/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20895 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/structured/parsing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/structured/prompting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21700 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/structured/prompting_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25818 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/structured/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/structured/schema_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/structured/schema_generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23078 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/structured/schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/structured/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/structured/scoring_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/subscription_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22284 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15464 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/template_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:03:36.547569 langfun-0.0.2.dev20240509/langfun/core/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/templates/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/templates/completion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/templates/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/templates/conversation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/templates/demonstration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/templates/demonstration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/templates/selfplay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/templates/selfplay_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/text_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/langfun/core/text_formatting_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:03:36.547569 langfun-0.0.2.dev20240509/langfun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-09 08:03:36.000000 langfun-0.0.2.dev20240509/langfun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-05-09 08:03:36.000000 langfun-0.0.2.dev20240509/langfun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 08:03:36.000000 langfun-0.0.2.dev20240509/langfun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-09 08:03:36.000000 langfun-0.0.2.dev20240509/langfun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-09 08:03:36.000000 langfun-0.0.2.dev20240509/langfun.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 08:03:36.547569 langfun-0.0.2.dev20240509/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-09 08:03:18.000000 langfun-0.0.2.dev20240509/setup.py
```

### Comparing `langfun-0.0.2.dev20240508/LICENSE` & `langfun-0.0.2.dev20240509/LICENSE`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/PKG-INFO` & `langfun-0.0.2.dev20240509/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langfun
-Version: 0.0.2.dev20240508
+Version: 0.0.2.dev20240509
 Summary: Langfun: Language as Functions.
 Home-page: https://github.com/google/langfun
 Author: Langfun Authors
 Author-email: langfun-authors@google.com
 License: Apache License 2.0
 Keywords: llm generative-ai machine-learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langfun-0.0.2.dev20240508/README.md` & `langfun-0.0.2.dev20240509/README.md`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/__init__.py` & `langfun-0.0.2.dev20240509/langfun/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/__init__.py` & `langfun-0.0.2.dev20240509/langfun/core/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/coding/__init__.py` & `langfun-0.0.2.dev20240509/langfun/core/coding/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/coding/python/__init__.py` & `langfun-0.0.2.dev20240509/langfun/core/coding/python/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/coding/python/correction.py` & `langfun-0.0.2.dev20240509/langfun/core/coding/python/correction.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/coding/python/correction_test.py` & `langfun-0.0.2.dev20240509/langfun/core/coding/python/correction_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/coding/python/errors.py` & `langfun-0.0.2.dev20240509/langfun/core/coding/python/errors.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/coding/python/errors_test.py` & `langfun-0.0.2.dev20240509/langfun/core/coding/python/errors_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/coding/python/execution.py` & `langfun-0.0.2.dev20240509/langfun/core/coding/python/execution.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/coding/python/execution_test.py` & `langfun-0.0.2.dev20240509/langfun/core/coding/python/execution_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/coding/python/generation.py` & `langfun-0.0.2.dev20240509/langfun/core/coding/python/generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/coding/python/generation_test.py` & `langfun-0.0.2.dev20240509/langfun/core/coding/python/generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/coding/python/parsing.py` & `langfun-0.0.2.dev20240509/langfun/core/coding/python/parsing.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/coding/python/parsing_test.py` & `langfun-0.0.2.dev20240509/langfun/core/coding/python/parsing_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/coding/python/permissions.py` & `langfun-0.0.2.dev20240509/langfun/core/coding/python/permissions.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/coding/python/permissions_test.py` & `langfun-0.0.2.dev20240509/langfun/core/coding/python/permissions_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/component.py` & `langfun-0.0.2.dev20240509/langfun/core/component.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/component_test.py` & `langfun-0.0.2.dev20240509/langfun/core/component_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/concurrent.py` & `langfun-0.0.2.dev20240509/langfun/core/concurrent.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/concurrent_test.py` & `langfun-0.0.2.dev20240509/langfun/core/concurrent_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/console.py` & `langfun-0.0.2.dev20240509/langfun/core/console.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/console_test.py` & `langfun-0.0.2.dev20240509/langfun/core/console_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/eval/__init__.py` & `langfun-0.0.2.dev20240509/langfun/core/eval/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/eval/base.py` & `langfun-0.0.2.dev20240509/langfun/core/eval/base.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/eval/base_test.py` & `langfun-0.0.2.dev20240509/langfun/core/eval/base_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/eval/matching.py` & `langfun-0.0.2.dev20240509/langfun/core/eval/matching.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/eval/matching_test.py` & `langfun-0.0.2.dev20240509/langfun/core/eval/matching_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/eval/patching.py` & `langfun-0.0.2.dev20240509/langfun/core/eval/patching.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/eval/patching_test.py` & `langfun-0.0.2.dev20240509/langfun/core/eval/patching_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/eval/scoring.py` & `langfun-0.0.2.dev20240509/langfun/core/eval/scoring.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/eval/scoring_test.py` & `langfun-0.0.2.dev20240509/langfun/core/eval/scoring_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/langfunc.py` & `langfun-0.0.2.dev20240509/langfun/core/langfunc.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/langfunc_test.py` & `langfun-0.0.2.dev20240509/langfun/core/langfunc_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/language_model.py` & `langfun-0.0.2.dev20240509/langfun/core/language_model.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/language_model_test.py` & `langfun-0.0.2.dev20240509/langfun/core/language_model_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/llms/__init__.py` & `langfun-0.0.2.dev20240509/langfun/core/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/llms/anthropic.py` & `langfun-0.0.2.dev20240509/langfun/core/llms/anthropic.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/llms/anthropic_test.py` & `langfun-0.0.2.dev20240509/langfun/core/llms/anthropic_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/llms/cache/__init__.py` & `langfun-0.0.2.dev20240509/langfun/core/llms/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/llms/cache/base.py` & `langfun-0.0.2.dev20240509/langfun/core/llms/cache/base.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/llms/cache/in_memory.py` & `langfun-0.0.2.dev20240509/langfun/core/llms/cache/in_memory.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/llms/cache/in_memory_test.py` & `langfun-0.0.2.dev20240509/langfun/core/llms/cache/in_memory_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/llms/fake.py` & `langfun-0.0.2.dev20240509/langfun/core/llms/fake.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/llms/fake_test.py` & `langfun-0.0.2.dev20240509/langfun/core/llms/fake_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/llms/google_genai.py` & `langfun-0.0.2.dev20240509/langfun/core/llms/google_genai.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/llms/google_genai_test.py` & `langfun-0.0.2.dev20240509/langfun/core/llms/google_genai_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/llms/groq.py` & `langfun-0.0.2.dev20240509/langfun/core/llms/groq.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/llms/groq_test.py` & `langfun-0.0.2.dev20240509/langfun/core/llms/groq_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/llms/llama_cpp.py` & `langfun-0.0.2.dev20240509/langfun/core/llms/llama_cpp.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/llms/llama_cpp_test.py` & `langfun-0.0.2.dev20240509/langfun/core/llms/llama_cpp_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/llms/openai.py` & `langfun-0.0.2.dev20240509/langfun/core/llms/openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,16 +229,17 @@
   ) -> list[lf.LMSamplingResult]:
     def _open_ai_chat_completion(prompt: lf.Message):
       if self.multimodal:
         content = []
         for chunk in prompt.chunk():
           if isinstance(chunk, str):
             item = dict(type='text', text=chunk)
-          elif isinstance(chunk, lf_modalities.Image) and chunk.uri:
-            item = dict(type='image_url', image_url=dict(url=chunk.uri))
+          elif isinstance(chunk, lf_modalities.Image):
+            uri = chunk.uri or chunk.content_uri
+            item = dict(type='image_url', image_url=dict(url=uri))
           else:
             raise ValueError(f'Unsupported modality object: {chunk!r}.')
           content.append(item)
       else:
         content = prompt.text
 
       response = openai.ChatCompletion.create(
```

### Comparing `langfun-0.0.2.dev20240508/langfun/core/llms/openai_test.py` & `langfun-0.0.2.dev20240509/langfun/core/llms/openai_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/memories/__init__.py` & `langfun-0.0.2.dev20240509/langfun/core/memories/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/memories/conversation_history.py` & `langfun-0.0.2.dev20240509/langfun/core/memories/conversation_history.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/memories/conversation_history_test.py` & `langfun-0.0.2.dev20240509/langfun/core/memories/conversation_history_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/memory.py` & `langfun-0.0.2.dev20240509/langfun/core/memory.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/message.py` & `langfun-0.0.2.dev20240509/langfun/core/message.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/message_test.py` & `langfun-0.0.2.dev20240509/langfun/core/message_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/modalities/__init__.py` & `langfun-0.0.2.dev20240509/langfun/core/modalities/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/modalities/image.py` & `langfun-0.0.2.dev20240509/langfun/core/modalities/image.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Image modality."""
 
-import base64
 import imghdr
 from typing import cast
 from langfun.core.modalities import mime
 
 
 class Image(mime.MimeType):
   """Base class for image."""
@@ -32,9 +31,8 @@
   @property
   def mime_type(self) -> str:
     return f'image/{self.image_format}'
 
   def _repr_html_(self) -> str:
     if self.uri and self.uri.lower().startswith(('http:', 'https:', 'ftp:')):
       return f'<img src="{self.uri}">'
-    image_raw = base64.b64encode(self.to_bytes()).decode()
-    return f'<img src="data:image/{self.image_format};base64,{image_raw}">'
+    return f'<img src="{self.content_uri}">'
```

### Comparing `langfun-0.0.2.dev20240508/langfun/core/modalities/image_test.py` & `langfun-0.0.2.dev20240509/langfun/core/modalities/image_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/modalities/mime.py` & `langfun-0.0.2.dev20240509/langfun/core/modalities/mime.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """MIME type data."""
 
 import abc
+import base64
 from typing import Annotated, Union
 import langfun.core as lf
 import pyglove as pg
 import requests
 
 
 class MimeType(lf.Modality):
@@ -50,14 +51,19 @@
           headers={'User-Agent': 'Langfun'},
       ).content
     else:
       content = pg.io.readfile(self.uri, mode='rb')
     self.rebind(content=content, skip_notification=True)
     return self.content
 
+  @property
+  def content_uri(self) -> str:
+    base64_content = base64.b64encode(self.to_bytes()).decode()
+    return f'data:{self.mime_type};base64,{base64_content}'
+
   @classmethod
   def from_uri(cls, uri: str, **kwargs) -> 'MimeType':
     return cls(uri=uri, content=None, **kwargs)
 
   @classmethod
   def from_bytes(cls, content: bytes | str, **kwargs) -> 'MimeType':
     return cls(content=content, **kwargs)
```

### Comparing `langfun-0.0.2.dev20240508/langfun/core/modalities/mime_test.py` & `langfun-0.0.2.dev20240509/langfun/core/modalities/mime_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/modalities/video.py` & `langfun-0.0.2.dev20240509/langfun/core/modalities/video.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Video modality."""
 
-import base64
 from typing import cast
 from langfun.core.modalities import mime
 
 
 class Video(mime.MimeType):
   """Base class for Video."""
 
@@ -36,12 +35,11 @@
     if 'video/' not in video_mime_type:
       raise ValueError(f'Not a video: {video_mime_type!r}.')
     return video_mime_type
 
   def _repr_html_(self) -> str:
     if self.uri and self.uri.lower().startswith(('http:', 'https:', 'ftp:')):
       return f'<video controls> <source src="{self.uri}"> </video>'
-    video_raw = base64.b64encode(self.to_bytes()).decode()
     return (
         '<video controls> <source'
-        f' src="data:video/{self.video_format};base64,{video_raw}"> </video>'
+        f' src="data:video/{self.content_uri}"> </video>'
     )
```

### Comparing `langfun-0.0.2.dev20240508/langfun/core/modalities/video_test.py` & `langfun-0.0.2.dev20240509/langfun/core/modalities/video_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/modality.py` & `langfun-0.0.2.dev20240509/langfun/core/modality.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/modality_test.py` & `langfun-0.0.2.dev20240509/langfun/core/modality_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/natural_language.py` & `langfun-0.0.2.dev20240509/langfun/core/natural_language.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/natural_language_test.py` & `langfun-0.0.2.dev20240509/langfun/core/natural_language_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/sampling.py` & `langfun-0.0.2.dev20240509/langfun/core/sampling.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/sampling_test.py` & `langfun-0.0.2.dev20240509/langfun/core/sampling_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/structured/__init__.py` & `langfun-0.0.2.dev20240509/langfun/core/structured/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/structured/completion.py` & `langfun-0.0.2.dev20240509/langfun/core/structured/completion.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/structured/completion_test.py` & `langfun-0.0.2.dev20240509/langfun/core/structured/completion_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/structured/description.py` & `langfun-0.0.2.dev20240509/langfun/core/structured/description.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/structured/description_test.py` & `langfun-0.0.2.dev20240509/langfun/core/structured/description_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/structured/function_generation.py` & `langfun-0.0.2.dev20240509/langfun/core/structured/function_generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/structured/function_generation_test.py` & `langfun-0.0.2.dev20240509/langfun/core/structured/function_generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/structured/mapping.py` & `langfun-0.0.2.dev20240509/langfun/core/structured/mapping.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/structured/mapping_test.py` & `langfun-0.0.2.dev20240509/langfun/core/structured/mapping_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/structured/parsing.py` & `langfun-0.0.2.dev20240509/langfun/core/structured/parsing.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/structured/parsing_test.py` & `langfun-0.0.2.dev20240509/langfun/core/structured/parsing_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/structured/prompting.py` & `langfun-0.0.2.dev20240509/langfun/core/structured/prompting.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/structured/prompting_test.py` & `langfun-0.0.2.dev20240509/langfun/core/structured/prompting_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/structured/schema.py` & `langfun-0.0.2.dev20240509/langfun/core/structured/schema.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/structured/schema_generation.py` & `langfun-0.0.2.dev20240509/langfun/core/structured/schema_generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/structured/schema_generation_test.py` & `langfun-0.0.2.dev20240509/langfun/core/structured/schema_generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/structured/schema_test.py` & `langfun-0.0.2.dev20240509/langfun/core/structured/schema_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/structured/scoring.py` & `langfun-0.0.2.dev20240509/langfun/core/structured/scoring.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/structured/scoring_test.py` & `langfun-0.0.2.dev20240509/langfun/core/structured/scoring_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/subscription.py` & `langfun-0.0.2.dev20240509/langfun/core/subscription.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/subscription_test.py` & `langfun-0.0.2.dev20240509/langfun/core/subscription_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/template.py` & `langfun-0.0.2.dev20240509/langfun/core/template.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/template_test.py` & `langfun-0.0.2.dev20240509/langfun/core/template_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/templates/__init__.py` & `langfun-0.0.2.dev20240509/langfun/core/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/templates/completion.py` & `langfun-0.0.2.dev20240509/langfun/core/templates/completion.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/templates/completion_test.py` & `langfun-0.0.2.dev20240509/langfun/core/templates/completion_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/templates/conversation.py` & `langfun-0.0.2.dev20240509/langfun/core/templates/conversation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/templates/conversation_test.py` & `langfun-0.0.2.dev20240509/langfun/core/templates/conversation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/templates/demonstration.py` & `langfun-0.0.2.dev20240509/langfun/core/templates/demonstration.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/templates/demonstration_test.py` & `langfun-0.0.2.dev20240509/langfun/core/templates/demonstration_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/templates/selfplay.py` & `langfun-0.0.2.dev20240509/langfun/core/templates/selfplay.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/templates/selfplay_test.py` & `langfun-0.0.2.dev20240509/langfun/core/templates/selfplay_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/text_formatting.py` & `langfun-0.0.2.dev20240509/langfun/core/text_formatting.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun/core/text_formatting_test.py` & `langfun-0.0.2.dev20240509/langfun/core/text_formatting_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/langfun.egg-info/PKG-INFO` & `langfun-0.0.2.dev20240509/langfun.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langfun
-Version: 0.0.2.dev20240508
+Version: 0.0.2.dev20240509
 Summary: Langfun: Language as Functions.
 Home-page: https://github.com/google/langfun
 Author: Langfun Authors
 Author-email: langfun-authors@google.com
 License: Apache License 2.0
 Keywords: llm generative-ai machine-learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langfun-0.0.2.dev20240508/langfun.egg-info/SOURCES.txt` & `langfun-0.0.2.dev20240509/langfun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240508/setup.py` & `langfun-0.0.2.dev20240509/setup.py`

 * *Files identical despite different names*

