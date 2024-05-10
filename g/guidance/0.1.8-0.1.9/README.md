# Comparing `tmp/guidance-0.1.8.tar.gz` & `tmp/guidance-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guidance-0.1.8.tar", last modified: Fri Dec 15 00:04:06 2023, max compression
+gzip compressed data, was "guidance-0.1.9.tar", last modified: Fri Dec 22 18:43:33 2023, max compression
```

## Comparing `guidance-0.1.8.tar` & `guidance-0.1.9.tar`

### file list

```diff
@@ -1,98 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 00:04:06.899126 guidance-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2023-12-15 00:04:00.000000 guidance-0.1.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2023-12-15 00:04:06.899126 guidance-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    33909 2023-12-15 00:04:00.000000 guidance-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 00:04:06.887126 guidance-0.1.8/guidance/
--rw-r--r--   0 runner    (1001) docker     (127)     8196 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 00:04:06.891126 guidance-0.1.8/guidance/_cpp/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/_cpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/_cpp/byte_trie.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/_cpp/byte_trie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/_cpp/main.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    21938 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/_grammar.py
--rw-r--r--   0 runner    (1001) docker     (127)    20400 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    10264 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 00:04:06.891126 guidance-0.1.8/guidance/library/
--rw-r--r--   0 runner    (1001) docker     (127)      998 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/library/_any_char.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/library/_any_char_but.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/library/_block.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/library/_char_range.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/library/_char_set.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/library/_format.py
--rw-r--r--   0 runner    (1001) docker     (127)    10535 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/library/_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/library/_image.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/library/_one_or_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/library/_optional.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/library/_prefix_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     5063 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/library/_regex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/library/_role.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/library/_silent.py
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/library/_substring.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/library/_tool.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/library/_zero_or_more.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 00:04:06.895126 guidance-0.1.8/guidance/models/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/models/_anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/models/_azure_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/models/_cohere.py
--rw-r--r--   0 runner    (1001) docker     (127)     6193 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/models/_lite_llm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/models/_mock.py
--rw-r--r--   0 runner    (1001) docker     (127)    50692 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/models/_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7655 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/models/_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)    16601 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/models/_remote.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 00:04:06.895126 guidance-0.1.8/guidance/models/llama_cpp/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/models/llama_cpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7253 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/models/llama_cpp/_llama_cpp.py
--rw-r--r--   0 runner    (1001) docker     (127)      980 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/models/llama_cpp/_mistral.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 00:04:06.895126 guidance-0.1.8/guidance/models/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/models/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/models/transformers/_llama.py
--rw-r--r--   0 runner    (1001) docker     (127)     6334 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/models/transformers/_transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 00:04:06.895126 guidance-0.1.8/guidance/models/vertexai/
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/models/vertexai/_Codey.py
--rw-r--r--   0 runner    (1001) docker     (127)     5190 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/models/vertexai/_Gemini.py
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/models/vertexai/_PaLM2.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/models/vertexai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8536 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/models/vertexai/_vertexai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 00:04:06.895126 guidance-0.1.8/guidance/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6008 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/resources/main.js
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2023-12-15 00:04:00.000000 guidance-0.1.8/guidance/selectors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 00:04:06.899126 guidance-0.1.8/guidance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2023-12-15 00:04:06.000000 guidance-0.1.8/guidance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2023-12-15 00:04:06.000000 guidance-0.1.8/guidance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-15 00:04:06.000000 guidance-0.1.8/guidance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      212 2023-12-15 00:04:06.000000 guidance-0.1.8/guidance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-15 00:04:06.000000 guidance-0.1.8/guidance.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      128 2023-12-15 00:04:00.000000 guidance-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-15 00:04:06.899126 guidance-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2023-12-15 00:04:00.000000 guidance-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 00:04:06.895126 guidance-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 00:04:00.000000 guidance-0.1.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 00:04:06.899126 guidance-0.1.8/tests/library/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 00:04:00.000000 guidance-0.1.8/tests/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2023-12-15 00:04:00.000000 guidance-0.1.8/tests/library/test_any_char.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2023-12-15 00:04:00.000000 guidance-0.1.8/tests/library/test_any_char_but.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2023-12-15 00:04:00.000000 guidance-0.1.8/tests/library/test_block.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2023-12-15 00:04:00.000000 guidance-0.1.8/tests/library/test_capture.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2023-12-15 00:04:00.000000 guidance-0.1.8/tests/library/test_char_set.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2023-12-15 00:04:00.000000 guidance-0.1.8/tests/library/test_commit_point.py
--rw-r--r--   0 runner    (1001) docker     (127)    12732 2023-12-15 00:04:00.000000 guidance-0.1.8/tests/library/test_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2023-12-15 00:04:00.000000 guidance-0.1.8/tests/library/test_one_or_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2023-12-15 00:04:00.000000 guidance-0.1.8/tests/library/test_silent.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2023-12-15 00:04:00.000000 guidance-0.1.8/tests/library/test_substring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 00:04:06.899126 guidance-0.1.8/tests/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 00:04:00.000000 guidance-0.1.8/tests/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2023-12-15 00:04:00.000000 guidance-0.1.8/tests/models/test_anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2023-12-15 00:04:00.000000 guidance-0.1.8/tests/models/test_azureai_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2023-12-15 00:04:00.000000 guidance-0.1.8/tests/models/test_cohere.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2023-12-15 00:04:00.000000 guidance-0.1.8/tests/models/test_lite_llm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2023-12-15 00:04:00.000000 guidance-0.1.8/tests/models/test_llama_cpp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2023-12-15 00:04:00.000000 guidance-0.1.8/tests/models/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2023-12-15 00:04:00.000000 guidance-0.1.8/tests/models/test_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2023-12-15 00:04:00.000000 guidance-0.1.8/tests/models/test_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2023-12-15 00:04:00.000000 guidance-0.1.8/tests/models/test_vertexai.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2023-12-15 00:04:00.000000 guidance-0.1.8/tests/test_grammar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4565 2023-12-15 00:04:00.000000 guidance-0.1.8/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2023-12-15 00:04:00.000000 guidance-0.1.8/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2023-12-15 00:04:00.000000 guidance-0.1.8/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 18:43:33.646618 guidance-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2023-12-22 18:43:26.000000 guidance-0.1.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2023-12-22 18:43:33.646618 guidance-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    33909 2023-12-22 18:43:26.000000 guidance-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 18:43:33.634618 guidance-0.1.9/guidance/
+-rw-r--r--   0 runner    (1001) docker     (127)     8200 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 18:43:33.634618 guidance-0.1.9/guidance/_cpp/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/_cpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/_cpp/byte_trie.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/_cpp/byte_trie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/_cpp/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    21938 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/_grammar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20400 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10264 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 18:43:33.638618 guidance-0.1.9/guidance/library/
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/library/_any_char.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/library/_any_char_but.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/library/_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/library/_char_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/library/_char_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/library/_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10535 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/library/_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/library/_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/library/_one_or_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/library/_optional.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/library/_prefix_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5063 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/library/_regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/library/_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/library/_silent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/library/_substring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/library/_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/library/_zero_or_more.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 18:43:33.638618 guidance-0.1.9/guidance/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/models/_anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3973 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/models/_azure_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/models/_cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7228 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/models/_googleai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6282 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/models/_lite_llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/models/_mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51034 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/models/_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9329 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/models/_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17021 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/models/_remote.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 18:43:33.638618 guidance-0.1.9/guidance/models/llama_cpp/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/models/llama_cpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7798 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/models/llama_cpp/_llama_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/models/llama_cpp/_mistral.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 18:43:33.638618 guidance-0.1.9/guidance/models/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/models/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/models/transformers/_llama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6878 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/models/transformers/_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 18:43:33.638618 guidance-0.1.9/guidance/models/vertexai/
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/models/vertexai/_Codey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5190 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/models/vertexai/_Gemini.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/models/vertexai/_PaLM2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/models/vertexai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8626 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/models/vertexai/_vertexai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 18:43:33.638618 guidance-0.1.9/guidance/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6008 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/resources/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2023-12-22 18:43:26.000000 guidance-0.1.9/guidance/selectors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 18:43:33.646618 guidance-0.1.9/guidance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2023-12-22 18:43:33.000000 guidance-0.1.9/guidance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2023-12-22 18:43:33.000000 guidance-0.1.9/guidance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-22 18:43:33.000000 guidance-0.1.9/guidance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2023-12-22 18:43:33.000000 guidance-0.1.9/guidance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-22 18:43:33.000000 guidance-0.1.9/guidance.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2023-12-22 18:43:26.000000 guidance-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-22 18:43:33.646618 guidance-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2023-12-22 18:43:26.000000 guidance-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 18:43:33.642618 guidance-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 18:43:26.000000 guidance-0.1.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 18:43:33.642618 guidance-0.1.9/tests/library/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 18:43:26.000000 guidance-0.1.9/tests/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2023-12-22 18:43:26.000000 guidance-0.1.9/tests/library/test_any_char.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2023-12-22 18:43:26.000000 guidance-0.1.9/tests/library/test_any_char_but.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2023-12-22 18:43:26.000000 guidance-0.1.9/tests/library/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2023-12-22 18:43:26.000000 guidance-0.1.9/tests/library/test_capture.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2023-12-22 18:43:26.000000 guidance-0.1.9/tests/library/test_char_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2023-12-22 18:43:26.000000 guidance-0.1.9/tests/library/test_commit_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12732 2023-12-22 18:43:26.000000 guidance-0.1.9/tests/library/test_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2023-12-22 18:43:26.000000 guidance-0.1.9/tests/library/test_one_or_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2023-12-22 18:43:26.000000 guidance-0.1.9/tests/library/test_silent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2023-12-22 18:43:26.000000 guidance-0.1.9/tests/library/test_substring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 18:43:33.646618 guidance-0.1.9/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 18:43:26.000000 guidance-0.1.9/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2023-12-22 18:43:26.000000 guidance-0.1.9/tests/models/test_anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2023-12-22 18:43:26.000000 guidance-0.1.9/tests/models/test_azureai_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2023-12-22 18:43:26.000000 guidance-0.1.9/tests/models/test_cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2023-12-22 18:43:26.000000 guidance-0.1.9/tests/models/test_googleai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2023-12-22 18:43:26.000000 guidance-0.1.9/tests/models/test_lite_llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2023-12-22 18:43:26.000000 guidance-0.1.9/tests/models/test_llama_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2023-12-22 18:43:26.000000 guidance-0.1.9/tests/models/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3838 2023-12-22 18:43:26.000000 guidance-0.1.9/tests/models/test_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2023-12-22 18:43:26.000000 guidance-0.1.9/tests/models/test_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2023-12-22 18:43:26.000000 guidance-0.1.9/tests/models/test_vertexai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2023-12-22 18:43:26.000000 guidance-0.1.9/tests/test_grammar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4565 2023-12-22 18:43:26.000000 guidance-0.1.9/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2023-12-22 18:43:26.000000 guidance-0.1.9/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2023-12-22 18:43:26.000000 guidance-0.1.9/tests/utils.py
```

### Comparing `guidance-0.1.8/LICENSE.md` & `guidance-0.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `guidance-0.1.8/PKG-INFO` & `guidance-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guidance
-Version: 0.1.8
+Version: 0.1.9
 Summary: A guidance language for controlling large language models.
 Home-page: https://github.com/guidance-ai/guidance
 Author: Scott Lundberg and Marco Tulio Ribeiro
 Author-email: scott@scottlundberg.com
 Requires-Python: >=3.8
 License-File: LICENSE.md
 Requires-Dist: diskcache
```

### Comparing `guidance-0.1.8/README.md` & `guidance-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `guidance-0.1.8/guidance/__init__.py` & `guidance-0.1.9/guidance/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 
 import functools
 import os
 import sys
 import types
 import requests
 
@@ -77,16 +77,16 @@
                     return node
 
             # otherwise must be stateful (which means we can't be inside a select() call)
             else:
                 return StatefulFunction(f, args, kwargs)
         
         # attach this as a method of the model class (if given)
-        if model is not None:
-            setattr(model, f.__name__, f)
+        # if model is not None:
+        #     setattr(model, f.__name__, f)
         
         return wrapped
 
 # def _decorator(f, *, model=None, dedent='python'):
 
 #     def _decorator_inner(f, model=models.Model):
 #         """Decorator to turn a normal function into a guidance function.
```

### Comparing `guidance-0.1.8/guidance/_cpp/byte_trie.cpp` & `guidance-0.1.9/guidance/_cpp/byte_trie.cpp`

 * *Files identical despite different names*

### Comparing `guidance-0.1.8/guidance/_cpp/byte_trie.py` & `guidance-0.1.9/guidance/_cpp/byte_trie.py`

 * *Files identical despite different names*

### Comparing `guidance-0.1.8/guidance/_cpp/main.cpp` & `guidance-0.1.9/guidance/_cpp/main.cpp`

 * *Files identical despite different names*

### Comparing `guidance-0.1.8/guidance/_grammar.py` & `guidance-0.1.9/guidance/_grammar.py`

 * *Files identical despite different names*

### Comparing `guidance-0.1.8/guidance/_parser.py` & `guidance-0.1.9/guidance/_parser.py`

 * *Files identical despite different names*

### Comparing `guidance-0.1.8/guidance/_utils.py` & `guidance-0.1.9/guidance/_utils.py`

 * *Files identical despite different names*

### Comparing `guidance-0.1.8/guidance/library/__init__.py` & `guidance-0.1.9/guidance/library/__init__.py`

 * *Files identical despite different names*

### Comparing `guidance-0.1.8/guidance/library/_any_char_but.py` & `guidance-0.1.9/guidance/library/_any_char_but.py`

 * *Files identical despite different names*

### Comparing `guidance-0.1.8/guidance/library/_char_set.py` & `guidance-0.1.9/guidance/library/_char_set.py`

 * *Files identical despite different names*

### Comparing `guidance-0.1.8/guidance/library/_gen.py` & `guidance-0.1.9/guidance/library/_gen.py`

 * *Files identical despite different names*

### Comparing `guidance-0.1.8/guidance/library/_prefix_tree.py` & `guidance-0.1.9/guidance/library/_prefix_tree.py`

 * *Files identical despite different names*

### Comparing `guidance-0.1.8/guidance/library/_regex.py` & `guidance-0.1.9/guidance/library/_regex.py`

 * *Files identical despite different names*

### Comparing `guidance-0.1.8/guidance/library/_role.py` & `guidance-0.1.9/guidance/library/_role.py`

 * *Files identical despite different names*

### Comparing `guidance-0.1.8/guidance/library/_substring.py` & `guidance-0.1.9/guidance/library/_substring.py`

 * *Files identical despite different names*

### Comparing `guidance-0.1.8/guidance/library/_tool.py` & `guidance-0.1.9/guidance/library/_tool.py`

 * *Files identical despite different names*

### Comparing `guidance-0.1.8/guidance/models/__init__.py` & `guidance-0.1.9/guidance/models/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,16 @@
-from ._model import Model, Chat
-from .vertexai._vertexai import VertexAI, VertexAIChat, VertexAICompletion, VertexAIInstruct
-from ._azure_openai import AzureOpenAI, AzureOpenAIChat, AzureOpenAICompletion, AzureOpenAIInstruct
-from ._openai import OpenAI, OpenAIChat, OpenAIInstruct, OpenAICompletion
+from ._model import Model, Instruct, Chat
+
+# local models
 from .transformers._transformers import Transformers, TransformersChat
 from .llama_cpp import LlamaCpp, LlamaCppChat, MistralInstruct, MistralChat
 from ._mock import Mock, MockChat
-from ._lite_llm import LiteLLMChat, LiteLLMInstruct, LiteLLMCompletion
-from ._cohere import CohereCompletion, CohereInstruct
-from . import transformers
-from ._anthropic import AnthropicChat
+
+# remote models
+from ._remote import Remote
+from .vertexai._vertexai import VertexAI, VertexAIChat, VertexAICompletion, VertexAIInstruct
+from ._azure_openai import AzureOpenAI, AzureOpenAIChat, AzureOpenAICompletion, AzureOpenAIInstruct
+from ._openai import OpenAI, OpenAIChat, OpenAIInstruct, OpenAICompletion
+from ._lite_llm import LiteLLM, LiteLLMChat, LiteLLMInstruct, LiteLLMCompletion
+from ._cohere import Cohere,CohereCompletion, CohereInstruct
+from ._anthropic import Anthropic, AnthropicChat
+from ._googleai import GoogleAI, GoogleAIChat
```

### Comparing `guidance-0.1.8/guidance/models/_azure_openai.py` & `guidance-0.1.9/guidance/models/_azure_openai.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,15 @@
         caching=True,
         temperature=0.0,
         top_p=1.0,
         max_streaming_tokens=500,
         version="2023-10-01-preview",
         **kwargs,
     ):
+        '''Build a new AzureOpenAI model object that represents a model in a given state.'''
         if not is_openai or not hasattr(openai_package, "OpenAI"):
             raise Exception(
                 "Please install the openai package version >= 1 using `pip install openai -U` "
                 "in order to use guidance.models.OpenAI!"
             )
 
         if api_key is None and azure_ad_token_provider is None:
@@ -70,14 +71,15 @@
             # convert to any found subclass
             self.__class__ = found_subclass
             found_subclass.__init__(
                 self,
                 model=model,
                 azure_endpoint=azure_endpoint,
                 api_key=api_key,
+                azure_ad_token_provider=azure_ad_token_provider,
                 tokenizer=tokenizer,
                 echo=echo,
                 caching=caching,
                 temperature=temperature,
                 max_streaming_tokens=max_streaming_tokens,
                 version=version,
                 top_p=top_p,
```

### Comparing `guidance-0.1.8/guidance/models/_cohere.py` & `guidance-0.1.9/guidance/models/_cohere.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from ._lite_llm import LiteLLM, LiteLLMCompletion, LiteLLMInstruct
 
 class Cohere(LiteLLM):
     def __init__(self, model, tokenizer=None, echo=True, caching=True, api_base=None, api_key=None, custom_llm_provider=None, temperature=0.0, max_streaming_tokens=1000, **kwargs):
+        '''Build a new Anthropic model object that represents a model in a given state.'''
         try:
             import tokenizers
         except ImportError:
             raise Exception("Please install the HuggingFace tokenizers package using `pip install tokenizers -U` in order to use guidance.models.Cohere!")
 
         # get the tokenizer
         if tokenizer is None:
```

### Comparing `guidance-0.1.8/guidance/models/_lite_llm.py` & `guidance-0.1.9/guidance/models/_lite_llm.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 from ._model import Chat, Instruct
 from ._remote import Remote
 
 
 class LiteLLM(Remote):
     def __init__(self, model, tokenizer=None, echo=True, caching=True, api_base=None, api_key=None, custom_llm_provider=None, temperature=0.0, max_streaming_tokens=1000, **kwargs):
+        '''Build a new LiteLLM model object that represents a model in a given state.'''
         try:
             import litellm
         except ImportError:
             raise Exception("Please install the litellm package version >= 1.7 using `pip install litellm -U` in order to use guidance.models.LiteLLM!")
         
         # if we are called directly (as opposed to through super()) then we convert ourselves to a more specific subclass if possible
         if self.__class__ is LiteLLM:
```

### Comparing `guidance-0.1.8/guidance/models/_mock.py` & `guidance-0.1.9/guidance/models/_mock.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 
 from ._model import Model, Chat
 
 
 class Mock(Model):
     def __init__(self, byte_patterns=[], echo=True):
-        
+        '''Build a new Mock model object that represents a model in a given state.'''
         super().__init__(
             # our tokens are all bytes and all lowercase letter pairs
             [b"<s>"] + [bytes([i,j]) for i in range(ord('a'), ord('z')) for j in range(ord('a'), ord('z'))] + [bytes([i]) for i in range(256)],
             0,
             0,
             echo=echo
         )
```

### Comparing `guidance-0.1.8/guidance/models/_model.py` & `guidance-0.1.9/guidance/models/_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,19 +30,21 @@
 _null_grammar = string('')
 format_pattern = re.compile(r"<\|\|_.*?_\|\|>", flags=re.DOTALL)
 nodisp_pattern = re.compile(r"&lt;\|\|_#NODISP_\|\|&gt;.*?&lt;\|\|_/NODISP_\|\|&gt;", flags=re.DOTALL)
 html_pattern = re.compile(r"&lt;\|\|_html:(.*?)_\|\|&gt;", flags=re.DOTALL)
 image_pattern = re.compile(r"&lt;\|_image:(.*?)\|&gt;")
 
 class Model:
-    '''A guidance model object, which represents a sequence model in a given state.
+    '''The base guidance model object, which represents a sequence model in a given state.
     
     Model objects are immutable representations of model state, so whenever you change
     them you get a new model object. However, these copies share the "expensive"
     parts of the model like the the parameters and KV-cache, so making copies is cheap.
+
+    .. automethod:: __add__
     '''
 
     open_blocks = {} # track what context blocks are open
     _grammar_only = 0 # a flag that tracks when we are forced to be executing only compiled grammars (like when we are inside a select)
     _throttle_refresh = 0 # a flag that tracks when we can throttle our display since we know future display calls are going to happen
 
     def __init__(self, tokens, bos_token_id=None, eos_token_id=None, echo=True, compute_log_probs=False):
@@ -168,27 +170,31 @@
             The bytes we should append to our current state.
         '''
 
         # update the byte state
         self._state += str(value) # TODO: make _state to be bytes not a string
 
         # see if we should update the display
-        if self.echo and not force_silent:
+        if not force_silent:
+            self._update_display()
+        
+        # TODO: is this needed? This was for programmatic streaming...
+        self._send_to_event_queue(self)
+
+    def _update_display(self, throttle=True):
+        if self.echo:
             if Model._throttle_refresh > 0:
                 curr_time = time.time()
-                if curr_time - self._last_display < self.max_display_rate:
+                if throttle and curr_time - self._last_display < self.max_display_rate:
                     return # we are throttling the update
                 else:
                     self._last_display = curr_time
         
             clear_output(wait=True)
             display(HTML(self._html()))
-        
-        # TODO: is this needed? This was for programmatic streaming...
-        self._send_to_event_queue(self)
     
     def reset(self, clear_variables=True):
         '''This resets the state of the model object.
         
         Parameters
         ----------
         clear_variables : bool
@@ -302,17 +308,17 @@
                     raise Exception(f"A guidance function did not return a model object! Did you forget to return the new lm at the end of your function?")
         
         # this flushes the display
         out._inplace_append("")
 
         return out
     
-    def endswith(self, s):
-        '''Checks if the current model state ends with the given value.'''
-        return self._current_prompt().endswith(s)
+    # def endswith(self, s):
+    #     '''Checks if the current model state ends with the given value.'''
+    #     return self._current_prompt().endswith(s)
     
     def __len__(self):
         '''The string length of the current state.
         
         TODO: This should change to the byte length...
         '''
         return len(str(self))
@@ -385,57 +391,57 @@
             The name of the variable.
         default : any
             The value to return if the variable is not current set.
         '''
         # TODO: support calling without a key to get the log prob of the whole model
         return self._variables_log_probs.get(key, default)
     
-    def get_cache(self):
-        return self.engine.cache
+    # def get_cache(self):
+    #     return self.engine.cache
     
-    def tool_def(self, functions):
+#     def tool_def(self, functions):
 
-        self += """
-# Tools
+#         self += """
+# # Tools
 
-"""
-        if len(functions) > 0:
-            self += '''## functions
-
-namespace functions {
-
-'''
-        for function in functions:
-            self += f"""// {function['description']}
-type {function['name']} = (_: {{"""
-            for prop_name,prop_data in function["parameters"]["properties"].items():
-                if "description" in prop_data:
-                    self += f"\n// {prop_data['description']}\n"
-                self += prop_name
-                if prop_name not in function["parameters"]["required"]:
-                    self += "?"
-                self += ": "
-                if "enum" in prop_data:
-                    for enum in prop_data["enum"]:
-                        self += f'"{enum}"'
-                        if enum != prop_data["enum"][-1]:
-                            self += " | "
-                else:
-                    self += prop_data["type"]
+# """
+#         if len(functions) > 0:
+#             self += '''## functions
+
+# namespace functions {
+
+# '''
+#         for function in functions:
+#             self += f"""// {function['description']}
+# type {function['name']} = (_: {{"""
+#             for prop_name,prop_data in function["parameters"]["properties"].items():
+#                 if "description" in prop_data:
+#                     self += f"\n// {prop_data['description']}\n"
+#                 self += prop_name
+#                 if prop_name not in function["parameters"]["required"]:
+#                     self += "?"
+#                 self += ": "
+#                 if "enum" in prop_data:
+#                     for enum in prop_data["enum"]:
+#                         self += f'"{enum}"'
+#                         if enum != prop_data["enum"][-1]:
+#                             self += " | "
+#                 else:
+#                     self += prop_data["type"]
                 
-                if prop_name != list(function["parameters"]["properties"].keys())[-1]:
-                    self += ",\n"
-            self += """
-}) => any;
-
-"""
-            self[function['name']] = function
-        self += "} // namespace functions\n"
+#                 if prop_name != list(function["parameters"]["properties"].keys())[-1]:
+#                     self += ",\n"
+#             self += """
+# }) => any;
+
+# """
+#             self[function['name']] = function
+#         self += "} // namespace functions\n"
         
-        return self
+#         return self
 
     def _run_stateless(lm, stateless_function, temperature=0.0, top_p=1.0, n=1):
         assert Model._grammar_only == 0, "We can't run grammar parsing while in context free mode! (for example inside a block closer)"
         
         logger.debug("start Model._run_stateless")
 
         # This needs to be here for streaming
@@ -608,17 +614,17 @@
 
     def _clean_duplicate_tokens(self, probs):
         '''This moves all the probability mass from duplicate positons on to their primary index.'''
         for i,j in self.duplicate_tokens:
             probs[j] += probs[i]
             probs[i] = 0
 
-    def _report_failed_match(self):
+    def _report_failed_match(self, prompt):
         """Note that this can be overridden by subclasses that have more likely reasons than a bug in the token set (like remote models)."""
-        return Exception("We can't consume any more tokens, but we are not yet done! Perhaps your model's token set is incomplete?")
+        return Exception("We can't consume any more tokens, but we are not yet done! Perhaps your model's token set is incomplete? This happened after the prompt:" + str(prompt[-40:]))
 
     def __call__(self, grammar, max_tokens=1000000, n=1, top_p=1, temperature=0.0, ensure_bos_token=True):
         assert n == 1, "Still need to add support for n > 1!"
         
         # get our current context in bytes
         prompt = self._current_prompt()
         prompt = bytes(prompt, encoding="utf8")
@@ -659,14 +665,15 @@
             # note where we are starting for this token
             start_pos = parser.pos
 
             # let the parser know that we have advanced another token (used ofr tracking max token limits)
             parser.mark_new_token()
 
             # walk down the trie as far as possible before computing the logits
+            is_generated = False
             retry_token_gen = False
             trie = self._token_trie
             trie.match_version += 1 # this invalidates all the match caches from the previous token
             # trie.prob = 0.0 # need to reset when we reset the match_version
             while True:
                 next_byte_mask = parser.next_byte_mask()
                 next_byte_mask_sum = next_byte_mask.sum()
@@ -772,14 +779,15 @@
                 # if we were forced we might need to clean up the greedy tokenization to match the global tokenization behavior as seen in training
                 if was_forced:
                     token_ids,token_byte_positions = self._cleanup_tokens(token_ids, token_byte_positions)
                     was_forced = False
                 grammar_temp = parser.next_byte_temperature()
                 current_temp = grammar_temp if grammar_temp >= 0 else temperature # we prefer to use the grammar temp when it is specified
                 logits = self._get_logits(token_ids, parser.bytes[start_pos:forced_pos], current_temp)
+                is_generated = True
 
                 # if requested we compute the log probabilities so we can track the probabilities of each node
                 if self.compute_log_probs:
                     if torch:
                         probs = torch.nn.functional.softmax(torch.tensor(logits), dim=-1).cpu().numpy() # note we don't adjust for temp since we consider that a sampling step, not part of the probs
                     else:
                         probs = softmax(logits, axis=-1) # this numpy code is slower, so we don't use it if we have torch...
@@ -932,24 +940,24 @@
                 #     self._cache_state["new_token_ids"].append(sampled_token_ind)
 
                 # capture the named groups from the parse tree
                 parse_tree = parser.parse_tree()
                 _record_captures(parse_tree, captured_data, captured_log_prob_data, parser.bytes)
                 
                 # we have no valid log prob data if we didn't compute it
-                yield new_bytes[hidden_count:], not is_forced, new_bytes_prob, captured_data, captured_log_prob_data, token_count - last_token_count
+                yield new_bytes[hidden_count:], is_generated, new_bytes_prob, captured_data, captured_log_prob_data, token_count - last_token_count
                 last_token_count = token_count
                 break # we are done!
             else:
                 generated_pos += len(new_bytes)
 
                 # yeild the snippet of text created by the next token
                 out = new_bytes[hidden_count:]
                 if len(out) > 0:
-                    yield out, not is_forced, new_bytes_prob, {}, {}, token_count - last_token_count # note that we don't capture groups until a complete parse right now...
+                    yield out, is_generated, new_bytes_prob, {}, {}, token_count - last_token_count # note that we don't capture groups until a complete parse right now...
                     last_token_count = token_count
                     hidden_count = 0
                     token_count += 1 # note we only update this for tokens that emit non-hidden content
                 else:
                     hidden_count -= len(new_bytes)
 
                 token_ids.append(sampled_token_ind)
```

### Comparing `guidance-0.1.8/guidance/models/_openai.py` & `guidance-0.1.9/guidance/models/_openai.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,15 +19,47 @@
     is_openai = True
 except ImportError:
     is_openai = False
 
 chat_model_pattern = r'^(ft:)?(gpt-3\.5-turbo|gpt-4)(?:(?!-instruct$)(-\w+)+)?(:[\w-]+(?:[:\w-]+)*)?(::\w+)?$'
 
 class OpenAI(Remote):
-    def __init__(self, model, tokenizer=None, echo=True, caching=True, api_key=None, organization=None, base_url=None, temperature=0.0, top_p=1.0, max_streaming_tokens=1000, **kwargs):
+    def __init__(self, model, tokenizer=None, echo=True, caching=True, api_key=None,
+                 temperature=0.0, top_p=1.0, max_streaming_tokens=1000, **kwargs):
+        '''Build a new OpenAI model object that represents a model in a given state.
+
+        This class automatically subclasses itself into the appropriate OpenAIChat, OpenAIInstruct,
+        or OpenAICompletion subclass based on the model name.
+        
+        Parameters
+        ----------
+        model : str
+            The name of the OpenAI model to use (e.g. gpt-3.5-turbo).
+        tokenizer : None or tiktoken.Encoding
+            The tokenizer to use for the given model. If set to None we use `tiktoken.encoding_for_model(model)`.
+        echo : bool
+            If true the final result of creating this model state will be displayed (as HTML in a notebook).
+        api_key : None or str
+            The OpenAI API key to use for remote requests, passed directly to the `openai.OpenAI` constructor.
+        temperature : float
+            The default temperature to use for generation requests. Note this default value may be overridden by the
+            grammars that are executed.
+        top_p : float
+            The default top_p to use for generation requests. Note this default value may be overridden by the
+            grammars that are executed.
+        max_streaming_tokens : int
+            The maximum number of tokens we allow this model to generate in a single stream. Normally this is set very
+            high and we rely either on early stopping on the remote side, or on the grammar terminating causing the
+            stream loop to break on the local side. This number needs to be longer than the longest stream you want
+            to generate.
+        **kwargs : 
+            All extra keyword arguments are passed directly to the `openai.OpenAI` constructor. Commonly used argument
+            names include `base_url` and `organization`
+        '''
+
         if not is_openai or not hasattr(openai_package, "OpenAI"):
             raise Exception("Please install the openai package version >= 1 using `pip install openai -U` in order to use guidance.models.OpenAI!")
         
         # if we are called directly (as opposed to through super()) then we convert ourselves to a more specific subclass if possible
         if self.__class__ is OpenAI:
             found_subclass = None
 
@@ -41,28 +73,28 @@
 
             # regular completion
             else:
                 found_subclass = OpenAICompletion
             
             # convert to any found subclass
             self.__class__ = found_subclass
-            found_subclass.__init__(self, model, tokenizer=tokenizer, echo=echo, caching=caching, api_key=api_key, organization=organization, base_url=base_url, temperature=temperature, max_streaming_tokens=max_streaming_tokens, **kwargs)
+            found_subclass.__init__(self, model, tokenizer=tokenizer, echo=echo, caching=caching, api_key=api_key, temperature=temperature, max_streaming_tokens=max_streaming_tokens, **kwargs)
             return # we return since we just ran init above and don't need to run again
 
-        self.client = openai_package.OpenAI(api_key=api_key, organization=organization, base_url=base_url)
+        self.client = openai_package.OpenAI(api_key=api_key, **kwargs)
         self.model_name = model
         self.top_p = top_p
 
         if tokenizer is None:
             tokenizer = tiktoken.encoding_for_model(model)
 
         super().__init__(
             model, tokenizer=tokenizer, echo=echo,
             caching=caching, temperature=temperature,
-            max_streaming_tokens=max_streaming_tokens, **kwargs
+            max_streaming_tokens=max_streaming_tokens
         )
 
 class OAICompletionMixin(Instruct):
 
     def _generator(self, prompt, temperature):
         
         self._reset_shared_data(prompt, temperature) # update our shared data state
@@ -123,15 +155,15 @@
                 stream=True
             )
         except Exception as e: # TODO: add retry logic
             raise e
 
         for part in generator:
             if len(part.choices) > 0:
-                chunk = part.choices[0].delta.content or ""
+                chunk = part.choices[0].text or ""
             else:
                 chunk = ""
             yield chunk.encode("utf8")
 
 class OAIChatMixin(Chat):
     def _generator(self, prompt, temperature):
```

### Comparing `guidance-0.1.8/guidance/models/_remote.py` & `guidance-0.1.9/guidance/models/_remote.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,21 @@
 import logging
 from ._model import Model, format_pattern, ConstraintException
 
 logger = logging.getLogger(__name__)
 
 
 class Remote(Model):
+    '''The base class for all remote models (hosted behind a remote API).'''
+    
     def __init__(self, model, tokenizer=None, echo=True, caching=True, temperature=0.0, top_p=1.0, max_streaming_tokens=None, timeout=0.5, **kwargs):
+        '''Build a new remote model object that represents a model in a given state.
+
+        This is an abstract class. To instantiate it use a specific subclass like guidance.models.OpenAI.
+        '''
         logger.debug(f"start Remote.__init__(model=\"{model}\")")
         self.caching = caching
         self.temperature = temperature
         self.top_p = top_p
         self.max_streaming_tokens = max_streaming_tokens
         self.timeout = timeout
 
@@ -121,14 +127,17 @@
         if self._running_stream():
             dqueue.put(self.tokens[self.eos_token_id])
         self._shared_state["not_running_stream"].set()
         dqueue.put(b'') # so we never get stuck waiting for a running stream to return something
 
     def _start_new_stream(self, prompt, temperature):
 
+        # make sure the display is up to date (since we are about to delay for a while)
+        self._update_display(throttle=False)
+
         if self._shared_state["num_calls_made"] > self.max_repeated_calls:
             raise Exception(f"We have exceeded the maximum number of repeat calls ({self.max_repeated_calls}) per grammar execution!")
 
         # stop any running stream
         if self._running_stream():
             self._shared_state["not_running_stream"].set() # stop the generator
             self._shared_state["remote_thread"].join() # wait for the thread to finish
```

### Comparing `guidance-0.1.8/guidance/models/llama_cpp/_llama_cpp.py` & `guidance-0.1.9/guidance/models/llama_cpp/_llama_cpp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import os
 from pathlib import Path
 from itertools import takewhile
 import operator
-
+import sys
+import logging
 import numpy as np
 
 from .._model import Model, Chat
 from ..._utils import normalize_notebook_stdout_stderr
 
 try:
     import llama_cpp
     is_llama_cpp = True
 except ImportError:
     is_llama_cpp = False
 
+logger = logging.getLogger(__name__)
+
 class _LlamaBatchContext:
     def __init__(self, n_batch, n_ctx):
         self._llama_batch_free = llama_cpp.llama_batch_free
         self.batch = llama_cpp.llama_batch_init(n_tokens=n_batch, embd=0, n_seq_max=n_ctx)
         if self.batch is None:
             raise Exception("call to llama_cpp.llama_batch_init returned NULL.")
 
@@ -27,15 +30,15 @@
         if batch is not None and llama_batch_free is not None:
             self._llama_batch_free = None
             self.batch = None
             llama_batch_free(batch)
 
 class LlamaCpp(Model):
     def __init__(self, model=None, tokenizer=None, echo=True, compute_log_probs=False, caching=True, temperature=0.0, **kwargs):
-
+        '''Build a new LlamaCpp model object that represents a model in a given state.'''
         if not is_llama_cpp:
             raise Exception("Please install llama-cpp-python with `pip install llama-cpp-python` in order to use guidance.models.LlamaCpp!")
 
         if isinstance(model, Path):
             model = str(model)
         if model is None or isinstance(model, str) and len(model.strip()) == 0:
             model = os.environ.get("LLAMA_CPP_MODEL", "")
@@ -49,14 +52,21 @@
                     raise ValueError("If model is None then a model file must be specified in either the LLAMA_CPP_MODEL environment variable or in the ~/.llama_cpp_model file.")
 
         if isinstance(model, str):
             self.model = model
             if "verbose" not in kwargs:
                 kwargs["verbose"] = False
 
+            # patch over https://github.com/abetlen/llama-cpp-python/issues/729
+            try:
+                sys.stdout.fileno()
+            except:
+                logger.warn("Cannot use verbose=True in this context (probably CoLab). See https://github.com/abetlen/llama-cpp-python/issues/729")
+                kwargs["verbose"] = True # llama-cpp-python can't hide output in this case
+
             with normalize_notebook_stdout_stderr():
                 self.model_obj = llama_cpp.Llama(model_path=model, **kwargs)
         elif isinstance(model, llama_cpp.Llama):
             self.model = model.__class__.__name__
             self.model_obj = model
         else:
             raise TypeError("model must be None, a file path string, or a llama_cpp.Llama object.")
```

### Comparing `guidance-0.1.8/guidance/models/llama_cpp/_mistral.py` & `guidance-0.1.9/guidance/models/llama_cpp/_mistral.py`

 * *Files identical despite different names*

### Comparing `guidance-0.1.8/guidance/models/transformers/_llama.py` & `guidance-0.1.9/guidance/models/transformers/_llama.py`

 * *Files identical despite different names*

### Comparing `guidance-0.1.8/guidance/models/transformers/_transformers.py` & `guidance-0.1.9/guidance/models/transformers/_transformers.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,16 @@
     pass
 
 from .._model import Model, Chat
 
 
 class Transformers(Model):
     def __init__(self, model=None, tokenizer=None, echo=True, caching=True, temperature=0.0, compute_log_probs=False, device=None, **kwargs):
-        
+        '''Build a new Transformers model object that represents a model in a given state.'''
+
         # fill in default model value
         if model is None:
             model = os.environ.get("TRANSFORMERS_MODEL", None)
         if model is None:
             try:
                 with open(os.path.expanduser('~/.transformers_model'), 'r') as file:
                     model = file.read().replace('\n', '')
@@ -82,14 +83,20 @@
                 import transformers
             except:
                 raise Exception("Please install transformers with `pip install transformers` in order to use guidance.models.Transformers!")
 
             if tokenizer is None:
                 try:
                     tokenizer = transformers.AutoTokenizer.from_pretrained(model, use_fast=False, **kwargs)
+                    # This is here because some tokenizers are bad and don't have all the bytes (I'm looking at you, microsoft/phi2)
+                    if hasattr(tokenizer, "byte_decoder"):
+                        all_bytes = set()
+                        for x in tokenizer.get_vocab().keys():
+                            [all_bytes.add(y) for y in x]
+                        assert set(tokenizer.byte_decoder.keys()).intersection(all_bytes) == all_bytes
                 except:
                     tokenizer = transformers.AutoTokenizer.from_pretrained(model, use_fast=True, **kwargs) # fall back to the fast tokenizer
             model = transformers.AutoModelForCausalLM.from_pretrained(model, **kwargs)
         
         assert tokenizer is not None, "You must give a tokenizer object when you provide a model object (as opposed to just a model name)!"
             
         return model, tokenizer
```

### Comparing `guidance-0.1.8/guidance/models/vertexai/_Codey.py` & `guidance-0.1.9/guidance/models/vertexai/_Codey.py`

 * *Files identical despite different names*

### Comparing `guidance-0.1.8/guidance/models/vertexai/_Gemini.py` & `guidance-0.1.9/guidance/models/vertexai/_Gemini.py`

 * *Files identical despite different names*

### Comparing `guidance-0.1.8/guidance/models/vertexai/_PaLM2.py` & `guidance-0.1.9/guidance/models/vertexai/_PaLM2.py`

 * *Files identical despite different names*

### Comparing `guidance-0.1.8/guidance/models/vertexai/_vertexai.py` & `guidance-0.1.9/guidance/models/vertexai/_vertexai.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     import vertexai
     is_vertexai = True
 except ImportError:
     is_vertexai = False
 
 class VertexAI(Remote):
     def __init__(self, model, tokenizer=None, echo=True, caching=True, temperature=0.0, top_p=1.0, max_streaming_tokens=None, **kwargs):
+        '''Build a new VertexAI model object that represents a model in a given state.'''
         if not is_vertexai:
             raise Exception("Please install the vertexai package using `pip install google-cloud-aiplatform` in order to use guidance.models.VertexAI!")
         
         # if we are called directly (as opposed to through super()) then we convert ourselves to a more specific subclass if possible
         if self.__class__ is VertexAI:
             found_subclass = None
             from .. import vertexai
```

### Comparing `guidance-0.1.8/guidance/resources/main.js` & `guidance-0.1.9/guidance/resources/main.js`

 * *Files identical despite different names*

### Comparing `guidance-0.1.8/guidance/selectors.py` & `guidance-0.1.9/guidance/selectors.py`

 * *Files identical despite different names*

### Comparing `guidance-0.1.8/guidance.egg-info/PKG-INFO` & `guidance-0.1.9/guidance.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guidance
-Version: 0.1.8
+Version: 0.1.9
 Summary: A guidance language for controlling large language models.
 Home-page: https://github.com/guidance-ai/guidance
 Author: Scott Lundberg and Marco Tulio Ribeiro
 Author-email: scott@scottlundberg.com
 Requires-Python: >=3.8
 License-File: LICENSE.md
 Requires-Dist: diskcache
```

### Comparing `guidance-0.1.8/guidance.egg-info/SOURCES.txt` & `guidance-0.1.9/guidance.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 guidance/library/_substring.py
 guidance/library/_tool.py
 guidance/library/_zero_or_more.py
 guidance/models/__init__.py
 guidance/models/_anthropic.py
 guidance/models/_azure_openai.py
 guidance/models/_cohere.py
+guidance/models/_googleai.py
 guidance/models/_lite_llm.py
 guidance/models/_mock.py
 guidance/models/_model.py
 guidance/models/_openai.py
 guidance/models/_remote.py
 guidance/models/llama_cpp/__init__.py
 guidance/models/llama_cpp/_llama_cpp.py
@@ -71,13 +72,14 @@
 tests/library/test_one_or_more.py
 tests/library/test_silent.py
 tests/library/test_substring.py
 tests/models/__init__.py
 tests/models/test_anthropic.py
 tests/models/test_azureai_openai.py
 tests/models/test_cohere.py
+tests/models/test_googleai.py
 tests/models/test_lite_llm.py
 tests/models/test_llama_cpp.py
 tests/models/test_model.py
 tests/models/test_openai.py
 tests/models/test_transformers.py
 tests/models/test_vertexai.py
```

### Comparing `guidance-0.1.8/setup.py` & `guidance-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `guidance-0.1.8/tests/library/test_block.py` & `guidance-0.1.9/tests/library/test_block.py`

 * *Files identical despite different names*

### Comparing `guidance-0.1.8/tests/library/test_char_set.py` & `guidance-0.1.9/tests/library/test_char_set.py`

 * *Files identical despite different names*

### Comparing `guidance-0.1.8/tests/library/test_commit_point.py` & `guidance-0.1.9/tests/library/test_commit_point.py`

 * *Files identical despite different names*

### Comparing `guidance-0.1.8/tests/library/test_gen.py` & `guidance-0.1.9/tests/library/test_gen.py`

 * *Files identical despite different names*

### Comparing `guidance-0.1.8/tests/models/test_anthropic.py` & `guidance-0.1.9/tests/models/test_anthropic.py`

 * *Files identical despite different names*

### Comparing `guidance-0.1.8/tests/models/test_azureai_openai.py` & `guidance-0.1.9/tests/models/test_azureai_openai.py`

 * *Files identical despite different names*

### Comparing `guidance-0.1.8/tests/models/test_cohere.py` & `guidance-0.1.9/tests/models/test_cohere.py`

 * *Files identical despite different names*

### Comparing `guidance-0.1.8/tests/models/test_lite_llm.py` & `guidance-0.1.9/tests/models/test_lite_llm.py`

 * *Files identical despite different names*

### Comparing `guidance-0.1.8/tests/models/test_llama_cpp.py` & `guidance-0.1.9/tests/models/test_llama_cpp.py`

 * *Files identical despite different names*

### Comparing `guidance-0.1.8/tests/models/test_model.py` & `guidance-0.1.9/tests/models/test_model.py`

 * *Files identical despite different names*

### Comparing `guidance-0.1.8/tests/models/test_openai.py` & `guidance-0.1.9/tests/models/test_openai.py`

 * *Files 11% similar despite different names*

```diff
@@ -36,14 +36,28 @@
     lm += "Count to 20: 1,2,3,4,"
     nl = "\n"
     lm += f"""\
 5,6,7"""
     lm += f"""{gen(max_tokens=1, suffix=nl)}aaaaaa"""
     assert str(lm)[-5:] == "aaaaa"
 
+def test_openai_gpt35_instruct():
+    from guidance import gen, instruction
+
+    # this relies on the environment variable OPENAI_API_KEY being set
+    try:
+        lm = guidance.models.OpenAI('gpt-3.5-turbo-instruct')
+    except:
+        pytest.skip("Skipping OpenAI test because we can't load the model!")
+
+    with instruction():
+        lm += "What is a popular flavor?"
+    lm += gen('flavor', max_tokens=2, stop=".")
+    assert len(lm['flavor']) > 0
+
 def test_openai_select():
     try:
         lm = guidance.models.OpenAI("text-curie-001")
     except:
         pytest.skip("Skipping OpenAI test because we can't load the model!")
     lm += "Pick a number: "
     lm += select(["1", "11", "111", "1111", "11111", "111111", "1111111"], name='the number')
```

### Comparing `guidance-0.1.8/tests/models/test_transformers.py` & `guidance-0.1.9/tests/models/test_transformers.py`

 * *Files identical despite different names*

### Comparing `guidance-0.1.8/tests/models/test_vertexai.py` & `guidance-0.1.9/tests/models/test_vertexai.py`

 * *Files identical despite different names*

### Comparing `guidance-0.1.8/tests/test_grammar.py` & `guidance-0.1.9/tests/test_grammar.py`

 * *Files identical despite different names*

### Comparing `guidance-0.1.8/tests/test_parser.py` & `guidance-0.1.9/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `guidance-0.1.8/tests/test_utils.py` & `guidance-0.1.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `guidance-0.1.8/tests/utils.py` & `guidance-0.1.9/tests/utils.py`

 * *Files identical despite different names*

