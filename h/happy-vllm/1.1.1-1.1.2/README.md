# Comparing `tmp/happy_vllm-1.1.1.tar.gz` & `tmp/happy_vllm-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "happy_vllm-1.1.1.tar", last modified: Fri Apr 19 08:57:49 2024, max compression
+gzip compressed data, was "happy_vllm-1.1.2.tar", last modified: Fri May 10 11:50:00 2024, max compression
```

## Comparing `happy_vllm-1.1.1.tar` & `happy_vllm-1.1.2.tar`

### file list

```diff
@@ -1,62 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:57:49.376431 happy_vllm-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    31709 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-19 08:57:49.376431 happy_vllm-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 08:57:49.376431 happy_vllm-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:57:49.368431 happy_vllm-1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:57:49.372431 happy_vllm-1.1.1/src/happy_vllm/
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/application.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:57:49.372431 happy_vllm-1.1.1/src/happy_vllm/core/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/core/logtools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/core/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/launch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:57:49.372431 happy_vllm-1.1.1/src/happy_vllm/logits_processors/
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/logits_processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/logits_processors/json_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/logits_processors/response_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/logits_processors/utils_parse_logits_processors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:57:49.372431 happy_vllm-1.1.1/src/happy_vllm/middlewares/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/middlewares/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:57:49.372431 happy_vllm-1.1.1/src/happy_vllm/model/
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12907 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/model/model_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    15713 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/model/openai_serving_chat_fixed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:57:49.372431 happy_vllm-1.1.1/src/happy_vllm/routers/
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16949 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/routers/functional.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:57:49.376431 happy_vllm-1.1.1/src/happy_vllm/routers/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/routers/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:57:49.376431 happy_vllm-1.1.1/src/happy_vllm/routers/schemas/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    16580 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/routers/schemas/examples/request.json
--rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/routers/schemas/examples/response.json
--rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/routers/schemas/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/routers/schemas/technical.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/routers/schemas/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/routers/technical.py
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13597 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/utils_args.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:57:49.376431 happy_vllm-1.1.1/src/happy_vllm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-19 08:57:49.000000 happy_vllm-1.1.1/src/happy_vllm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-19 08:57:49.000000 happy_vllm-1.1.1/src/happy_vllm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 08:57:49.000000 happy_vllm-1.1.1/src/happy_vllm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-19 08:57:49.000000 happy_vllm-1.1.1/src/happy_vllm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-19 08:57:49.000000 happy_vllm-1.1.1/src/happy_vllm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 08:57:49.000000 happy_vllm-1.1.1/src/happy_vllm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:57:49.376431 happy_vllm-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9486 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/tests/test_json_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/tests/test_model_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/tests/test_response_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    22506 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/tests/test_routers_functionnal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/tests/test_routers_technical.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/tests/test_schemas_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/tests/test_utils_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/tests/test_utils_parse_logits_processors.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-19 08:57:47.000000 happy_vllm-1.1.1/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:50:00.273030 happy_vllm-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    31709 2024-05-10 11:49:55.000000 happy_vllm-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-10 11:49:55.000000 happy_vllm-1.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-10 11:50:00.273030 happy_vllm-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-05-10 11:49:55.000000 happy_vllm-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-10 11:49:55.000000 happy_vllm-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 11:50:00.273030 happy_vllm-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-10 11:49:55.000000 happy_vllm-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:50:00.265030 happy_vllm-1.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:50:00.265030 happy_vllm-1.1.2/src/happy_vllm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-10 11:49:55.000000 happy_vllm-1.1.2/src/happy_vllm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-10 11:49:55.000000 happy_vllm-1.1.2/src/happy_vllm/application.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:50:00.269030 happy_vllm-1.1.2/src/happy_vllm/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-10 11:49:55.000000 happy_vllm-1.1.2/src/happy_vllm/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-10 11:49:55.000000 happy_vllm-1.1.2/src/happy_vllm/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-10 11:49:55.000000 happy_vllm-1.1.2/src/happy_vllm/core/logtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-10 11:49:55.000000 happy_vllm-1.1.2/src/happy_vllm/core/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-10 11:49:55.000000 happy_vllm-1.1.2/src/happy_vllm/launch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:50:00.269030 happy_vllm-1.1.2/src/happy_vllm/logits_processors/
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-10 11:49:55.000000 happy_vllm-1.1.2/src/happy_vllm/logits_processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-10 11:49:55.000000 happy_vllm-1.1.2/src/happy_vllm/logits_processors/json_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-05-10 11:49:55.000000 happy_vllm-1.1.2/src/happy_vllm/logits_processors/response_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-10 11:49:55.000000 happy_vllm-1.1.2/src/happy_vllm/logits_processors/utils_parse_logits_processors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:50:00.269030 happy_vllm-1.1.2/src/happy_vllm/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 11:49:55.000000 happy_vllm-1.1.2/src/happy_vllm/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-10 11:49:55.000000 happy_vllm-1.1.2/src/happy_vllm/middlewares/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:50:00.269030 happy_vllm-1.1.2/src/happy_vllm/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-10 11:49:55.000000 happy_vllm-1.1.2/src/happy_vllm/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12513 2024-05-10 11:49:55.000000 happy_vllm-1.1.2/src/happy_vllm/model/model_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:50:00.269030 happy_vllm-1.1.2/src/happy_vllm/routers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-10 11:49:55.000000 happy_vllm-1.1.2/src/happy_vllm/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16979 2024-05-10 11:49:55.000000 happy_vllm-1.1.2/src/happy_vllm/routers/functional.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:50:00.269030 happy_vllm-1.1.2/src/happy_vllm/routers/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-10 11:49:55.000000 happy_vllm-1.1.2/src/happy_vllm/routers/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:50:00.273030 happy_vllm-1.1.2/src/happy_vllm/routers/schemas/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    16580 2024-05-10 11:49:55.000000 happy_vllm-1.1.2/src/happy_vllm/routers/schemas/examples/request.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-05-10 11:49:55.000000 happy_vllm-1.1.2/src/happy_vllm/routers/schemas/examples/response.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-05-10 11:49:55.000000 happy_vllm-1.1.2/src/happy_vllm/routers/schemas/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-05-10 11:49:55.000000 happy_vllm-1.1.2/src/happy_vllm/routers/schemas/technical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-10 11:49:55.000000 happy_vllm-1.1.2/src/happy_vllm/routers/schemas/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-10 11:49:55.000000 happy_vllm-1.1.2/src/happy_vllm/routers/technical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-10 11:49:55.000000 happy_vllm-1.1.2/src/happy_vllm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14458 2024-05-10 11:49:55.000000 happy_vllm-1.1.2/src/happy_vllm/utils_args.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:50:00.273030 happy_vllm-1.1.2/src/happy_vllm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-10 11:50:00.000000 happy_vllm-1.1.2/src/happy_vllm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-10 11:50:00.000000 happy_vllm-1.1.2/src/happy_vllm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 11:50:00.000000 happy_vllm-1.1.2/src/happy_vllm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-10 11:50:00.000000 happy_vllm-1.1.2/src/happy_vllm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-10 11:50:00.000000 happy_vllm-1.1.2/src/happy_vllm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-10 11:50:00.000000 happy_vllm-1.1.2/src/happy_vllm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:50:00.273030 happy_vllm-1.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9486 2024-05-10 11:49:55.000000 happy_vllm-1.1.2/tests/test_json_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-05-10 11:49:55.000000 happy_vllm-1.1.2/tests/test_model_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-05-10 11:49:55.000000 happy_vllm-1.1.2/tests/test_response_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22506 2024-05-10 11:49:55.000000 happy_vllm-1.1.2/tests/test_routers_functionnal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-10 11:49:55.000000 happy_vllm-1.1.2/tests/test_routers_technical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-10 11:49:55.000000 happy_vllm-1.1.2/tests/test_schemas_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-10 11:49:55.000000 happy_vllm-1.1.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-10 11:49:55.000000 happy_vllm-1.1.2/tests/test_utils_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-10 11:49:55.000000 happy_vllm-1.1.2/tests/test_utils_parse_logits_processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 11:49:58.000000 happy_vllm-1.1.2/version.txt
```

### Comparing `happy_vllm-1.1.1/LICENSE` & `happy_vllm-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.1/PKG-INFO` & `happy_vllm-1.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: happy_vllm
-Version: 1.1.1
+Version: 1.1.2
 Summary: happy_vllm is a REST API for vLLM, production ready
 Requires-Python: <4.0,>=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: vllm<1.0,>=0.4.0
-Requires-Dist: fastapi<1.0,>=0.110.1
+Requires-Dist: vllm<1.0,>=0.4.2
+Requires-Dist: fastapi<1.0,>=0.111.0
 Requires-Dist: pydantic_settings<3.0,>=2.2.1
 Requires-Dist: uvicorn[standard]<1.0,>=0.29.0
 Requires-Dist: prometheus_client<1.0,>=0.20.0
 Requires-Dist: numpy>=1.26.4
-Requires-Dist: lm-format-enforcer<0.10.0,>=0.9.0
+Requires-Dist: jsonschema<5.0,>=4.22.0
 Provides-Extra: test
 Requires-Dist: httpx<1.0,>=0.23; extra == "test"
-Requires-Dist: pytest<8.0,>=7.4.3; extra == "test"
-Requires-Dist: pytest-cov<5.0,>=4.1.0; extra == "test"
+Requires-Dist: pytest<9.0,>=8.2.0; extra == "test"
+Requires-Dist: pytest-cov<6.0,>=5.0.0; extra == "test"
 Requires-Dist: mypy<2.0,>=1.7.1; extra == "test"
 
 ![happy_vllm logo](https://raw.githubusercontent.com/OSS-Pole-Emploi/happy_vllm/main/docs/source/assets/logo/logo_happy_vllm.svg)
 
 [![pypi badge](https://img.shields.io/pypi/v/happy_vllm.svg)](https://pypi.python.org/pypi/happy_vllm)
 [![Generic badge](https://img.shields.io/badge/python-3.10|3.11-blue.svg)](https://shields.io/)
 [![License: AGPL v3](https://img.shields.io/badge/License-AGPL%20v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
```

### Comparing `happy_vllm-1.1.1/README.md` & `happy_vllm-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.1/pyproject.toml` & `happy_vllm-1.1.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 
 [project]
 name = "happy_vllm"
 description = "happy_vllm is a REST API for vLLM, production ready"
 readme = "README.md"
 requires-python = ">=3.10,<4.0"
 dependencies = [
-    "vllm>=0.4.0,<1.0",
-    "fastapi>=0.110.1,<1.0",
+    "vllm>=0.4.2,<1.0",
+    "fastapi>=0.111.0,<1.0",
     "pydantic_settings>=2.2.1,<3.0",
     "uvicorn[standard]>=0.29.0,<1.0",
     "prometheus_client>=0.20.0,<1.0",
     "numpy>=1.26.4",
-    "lm-format-enforcer>=0.9.0,<0.10.0"
+    "jsonschema>=4.22.0,<5.0"
 ]
 
 dynamic = ["version"]
 
 [tool.setuptools.dynamic]
 version = {file = "version.txt"}
 
@@ -26,15 +26,15 @@
 where = ["src"]
 include = ["happy_vllm*"]
 
 [project.scripts]
 happy-vllm = "happy_vllm.launch:main"
 
 [project.optional-dependencies]
-test = ["httpx>=0.23,<1.0", "pytest>=7.4.3,<8.0", "pytest-cov>=4.1.0,<5.0", "mypy>=1.7.1,<2.0"]
+test = ["httpx>=0.23,<1.0", "pytest>=8.2.0,<9.0", "pytest-cov>=5.0.0,<6.0", "mypy>=1.7.1,<2.0"]
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 addopts = "-v --cov=happy_vllm"
 filterwarnings = [
     "ignore:The hookimpl CovPlugin.pytest_",
     "ignore:IPython could not be loaded!"
```

### Comparing `happy_vllm-1.1.1/src/happy_vllm/__init__.py` & `happy_vllm-1.1.2/src/happy_vllm/__init__.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.1/src/happy_vllm/application.py` & `happy_vllm-1.1.2/src/happy_vllm/application.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.1/src/happy_vllm/core/__init__.py` & `happy_vllm-1.1.2/src/happy_vllm/core/__init__.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.1/src/happy_vllm/core/config.py` & `happy_vllm-1.1.2/src/happy_vllm/core/config.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.1/src/happy_vllm/core/logtools.py` & `happy_vllm-1.1.2/src/happy_vllm/core/logtools.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.1/src/happy_vllm/core/resources.py` & `happy_vllm-1.1.2/src/happy_vllm/core/resources.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.1/src/happy_vllm/launch.py` & `happy_vllm-1.1.2/src/happy_vllm/launch.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.1/src/happy_vllm/logits_processors/__init__.py` & `happy_vllm-1.1.2/src/happy_vllm/logits_processors/__init__.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.1/src/happy_vllm/logits_processors/json_format.py` & `happy_vllm-1.1.2/src/happy_vllm/logits_processors/json_format.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.1/src/happy_vllm/logits_processors/response_pool.py` & `happy_vllm-1.1.2/src/happy_vllm/logits_processors/response_pool.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.1/src/happy_vllm/logits_processors/utils_parse_logits_processors.py` & `happy_vllm-1.1.2/src/happy_vllm/logits_processors/utils_parse_logits_processors.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.1/src/happy_vllm/middlewares/exception.py` & `happy_vllm-1.1.2/src/happy_vllm/middlewares/exception.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.1/src/happy_vllm/model/__init__.py` & `happy_vllm-1.1.2/src/happy_vllm/model/__init__.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.1/src/happy_vllm/model/model_base.py` & `happy_vllm-1.1.2/src/happy_vllm/model/model_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,19 +28,15 @@
 from vllm.engine.arg_utils import AsyncEngineArgs
 from vllm.engine.async_llm_engine import AsyncLLMEngine
 from vllm.entrypoints.openai.serving_completion import OpenAIServingCompletion
 from vllm.transformers_utils.tokenizer_group.tokenizer_group import TokenizerGroup
 from lmformatenforcer.integrations.transformers import build_token_enforcer_tokenizer_data
 
 from happy_vllm import utils
-# We use our own version of OpenAIServingChat to avoid this issue (https://github.com/vllm-project/vllm/issues/2683)
-# To solve this issue, we do what is described in this PR (https://github.com/vllm-project/vllm/pull/2727)
-# When it is resolved, please go back to the vLLM version of OpenAIServingChat and delete this one
-# from vllm.entrypoints.openai.serving_chat import OpenAIServingChat
-from happy_vllm.model.openai_serving_chat_fixed import OpenAIServingChat
+from vllm.entrypoints.openai.serving_chat import OpenAIServingChat
 
 logger = logging.getLogger(__name__)
 
 
 class Model:
     """Parent model class.
     """
@@ -79,19 +75,19 @@
             if isinstance(self._model.engine.tokenizer, TokenizerGroup): # type: ignore
                 self._tokenizer = self._model.engine.tokenizer.tokenizer # type: ignore
             else:
                 self._tokenizer = self._model.engine.tokenizer # type: ignore
             self._tokenizer_lmformatenforcer = build_token_enforcer_tokenizer_data(self._tokenizer)
             self.max_model_len = self._model.engine.model_config.max_model_len # type: ignore
             self.original_truncation_side = self._tokenizer.truncation_side
-            self.openai_serving_chat = OpenAIServingChat(self._model, args.model_name,
+            self.openai_serving_chat = OpenAIServingChat(self._model, [args.model_name],
                                                         args.response_role,
                                                         args.lora_modules,
                                                         args.chat_template)
-            self.openai_serving_completion = OpenAIServingCompletion(self._model, args.model_name, args.lora_modules)
+            self.openai_serving_completion = OpenAIServingCompletion(self._model, [args.model_name], args.lora_modules)
         # For test purpose
         else:
             self.max_model_len = 2048
             self.original_truncation_side = 'right'
             self._tokenizer = AutoTokenizer.from_pretrained(utils.TEST_TOKENIZER_NAME,
                                                      cache_dir=os.environ["TEST_MODELS_DIR"], truncation_side=self.original_truncation_side)
             self._tokenizer_lmformatenforcer = build_token_enforcer_tokenizer_data(self._tokenizer)
```

### Comparing `happy_vllm-1.1.1/src/happy_vllm/routers/__init__.py` & `happy_vllm-1.1.2/src/happy_vllm/routers/__init__.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.1/src/happy_vllm/routers/functional.py` & `happy_vllm-1.1.2/src/happy_vllm/routers/functional.py`

 * *Files 0% similar despite different names*

```diff
@@ -334,18 +334,18 @@
     model: Model = RESOURCES.get(RESOURCE_MODEL)
     generator = await model.openai_serving_chat.create_chat_completion(
         request, raw_request)
     if isinstance(generator, vllm_protocol.ErrorResponse):
         return JSONResponse(content=generator.model_dump(),
                             status_code=generator.code)
     if request.stream:
-        return StreamingResponse(content=generator,
+        return StreamingResponse(content=generator, # type: ignore
                                  media_type="text/event-stream")
     else:
-        return JSONResponse(content=generator.model_dump())
+        return JSONResponse(content=generator.model_dump()) # type: ignore
 
 
 @router.post("/v1/completions", response_model=functional_schema.HappyvllmCompletionResponse)
 async def create_completion(request: Annotated[vllm_protocol.CompletionRequest, Body(openapi_examples=request_openapi_examples["completions"])],
                             raw_request: Request):
     """Open AI compatible completion. See https://docs.vllm.ai/en/latest/serving/openai_compatible_server.html for more details
     """
```

### Comparing `happy_vllm-1.1.1/src/happy_vllm/routers/schemas/__init__.py` & `happy_vllm-1.1.2/src/happy_vllm/routers/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.1/src/happy_vllm/routers/schemas/examples/request.json` & `happy_vllm-1.1.2/src/happy_vllm/routers/schemas/examples/request.json`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.1/src/happy_vllm/routers/schemas/examples/response.json` & `happy_vllm-1.1.2/src/happy_vllm/routers/schemas/examples/response.json`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.1/src/happy_vllm/routers/schemas/functional.py` & `happy_vllm-1.1.2/src/happy_vllm/routers/schemas/functional.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.1/src/happy_vllm/routers/schemas/technical.py` & `happy_vllm-1.1.2/src/happy_vllm/routers/schemas/technical.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.1/src/happy_vllm/routers/schemas/utils.py` & `happy_vllm-1.1.2/src/happy_vllm/routers/schemas/utils.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.1/src/happy_vllm/routers/technical.py` & `happy_vllm-1.1.2/src/happy_vllm/routers/technical.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.1/src/happy_vllm/utils.py` & `happy_vllm-1.1.2/src/happy_vllm/utils.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.1/src/happy_vllm/utils_args.py` & `happy_vllm-1.1.2/src/happy_vllm/utils_args.py`

 * *Files 6% similar despite different names*

```diff
@@ -94,20 +94,22 @@
 
     # Define ModelSettings with the default values of the args (which will be replaced)
     # by the environnement variables or those of the .env file
     class ModelSettings(BaseSettings):
         model: str = default_args.model
         model_name: str = default_args.model_name
         tokenizer: Optional[str] = default_args.tokenizer
+        skip_tokenizer_init: bool = False
         tokenizer_mode: str = default_args.tokenizer_mode
         trust_remote_code: bool = False
         download_dir: Optional[str] = default_args.download_dir
         load_format: str = default_args.load_format
         dtype: str = default_args.dtype
         kv_cache_dtype: str = default_args.kv_cache_dtype
+        quantization_param_path: Optional[str] = default_args.quantization_param_path
         seed: int = default_args.seed
         max_model_len: Optional[int] = default_args.max_model_len
         worker_use_ray: bool = False
         pipeline_parallel_size: int = default_args.pipeline_parallel_size
         tensor_parallel_size: int = default_args.tensor_parallel_size
         max_parallel_loading_workers: Optional[int] = default_args.max_parallel_loading_workers
         block_size: int = default_args.block_size
@@ -118,39 +120,49 @@
         max_num_seqs: int = default_args.max_num_seqs
         disable_log_stats: bool = False
         revision: Optional[str] = default_args.revision
         code_revision: Optional[str] = default_args.code_revision
         tokenizer_revision: Optional[str] = default_args.tokenizer_revision
         quantization: Optional[str] = default_args.quantization
         enforce_eager: bool = False
-        max_context_len_to_capture: int = default_args.max_context_len_to_capture
+        max_context_len_to_capture: Optional[int] = default_args.max_context_len_to_capture
+        max_seq_len_to_capture: int = default_args.max_seq_len_to_capture
         disable_custom_all_reduce: bool = False
         enable_lora: bool = False
         max_loras: int = default_args.max_loras
         max_lora_rank: int = default_args.max_lora_rank
+        fully_sharded_loras: bool = False
         lora_extra_vocab_size: int = default_args.lora_extra_vocab_size
         lora_dtype: str = default_args.lora_dtype
         max_cpu_loras: Optional[int] = default_args.max_cpu_loras
         device: str = default_args.device
         ray_workers_use_nsight: bool = False
+        num_gpu_blocks_override: Optional[int] = default_args.num_gpu_blocks_override
+        num_lookahead_slots: int = default_args.num_lookahead_slots
+        model_loader_extra_config: Optional[dict] = default_args.model_loader_extra_config
         max_log_len: Optional[int] = default_args.max_log_len
         disable_log_requests: bool = False
         engine_use_ray: bool = False
         use_v2_block_manager: bool = False
-        num_lookahead_slots: int = default_args.num_lookahead_slots
-        forced_num_gpu_blocks: Optional[int] = default_args.forced_num_gpu_blocks
         max_logprobs: int = default_args.max_logprobs
         tokenizer_pool_size: int = default_args.tokenizer_pool_size
         tokenizer_pool_type: str = default_args.tokenizer_pool_type
         tokenizer_pool_extra_config: Optional[str] = default_args.tokenizer_pool_extra_config
         image_input_type: Optional[str] = default_args.image_input_type
         image_input_shape: Optional[str] = default_args.image_input_shape
         image_feature_size: Optional[int] = default_args.image_feature_size
         scheduler_delay_factor: float = default_args.scheduler_delay_factor
-        enable_chunked_prefill: bool = default_args.enable_chunked_prefill
+        enable_chunked_prefill: bool = False
+        guided_decoding_backend: str = default_args.guided_decoding_backend
+        # Speculative decoding configuration.
+        speculative_model: Optional[str] = default_args.speculative_model
+        num_speculative_tokens: Optional[int] = default_args.num_speculative_tokens
+        speculative_max_model_len: Optional[int] = default_args.speculative_max_model_len
+        ngram_prompt_lookup_max: Optional[int] = default_args.ngram_prompt_lookup_max
+        ngram_prompt_lookup_min: Optional[int] = default_args.ngram_prompt_lookup_min
 
         model_config = SettingsConfigDict(env_file=".env", extra='ignore', protected_namespaces=('settings', ))
 
     model_settings = ModelSettings()
 
     return model_settings
```

### Comparing `happy_vllm-1.1.1/src/happy_vllm.egg-info/PKG-INFO` & `happy_vllm-1.1.2/src/happy_vllm.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: happy_vllm
-Version: 1.1.1
+Version: 1.1.2
 Summary: happy_vllm is a REST API for vLLM, production ready
 Requires-Python: <4.0,>=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: vllm<1.0,>=0.4.0
-Requires-Dist: fastapi<1.0,>=0.110.1
+Requires-Dist: vllm<1.0,>=0.4.2
+Requires-Dist: fastapi<1.0,>=0.111.0
 Requires-Dist: pydantic_settings<3.0,>=2.2.1
 Requires-Dist: uvicorn[standard]<1.0,>=0.29.0
 Requires-Dist: prometheus_client<1.0,>=0.20.0
 Requires-Dist: numpy>=1.26.4
-Requires-Dist: lm-format-enforcer<0.10.0,>=0.9.0
+Requires-Dist: jsonschema<5.0,>=4.22.0
 Provides-Extra: test
 Requires-Dist: httpx<1.0,>=0.23; extra == "test"
-Requires-Dist: pytest<8.0,>=7.4.3; extra == "test"
-Requires-Dist: pytest-cov<5.0,>=4.1.0; extra == "test"
+Requires-Dist: pytest<9.0,>=8.2.0; extra == "test"
+Requires-Dist: pytest-cov<6.0,>=5.0.0; extra == "test"
 Requires-Dist: mypy<2.0,>=1.7.1; extra == "test"
 
 ![happy_vllm logo](https://raw.githubusercontent.com/OSS-Pole-Emploi/happy_vllm/main/docs/source/assets/logo/logo_happy_vllm.svg)
 
 [![pypi badge](https://img.shields.io/pypi/v/happy_vllm.svg)](https://pypi.python.org/pypi/happy_vllm)
 [![Generic badge](https://img.shields.io/badge/python-3.10|3.11-blue.svg)](https://shields.io/)
 [![License: AGPL v3](https://img.shields.io/badge/License-AGPL%20v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
```

### Comparing `happy_vllm-1.1.1/src/happy_vllm.egg-info/SOURCES.txt` & `happy_vllm-1.1.2/src/happy_vllm.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 src/happy_vllm/logits_processors/json_format.py
 src/happy_vllm/logits_processors/response_pool.py
 src/happy_vllm/logits_processors/utils_parse_logits_processors.py
 src/happy_vllm/middlewares/__init__.py
 src/happy_vllm/middlewares/exception.py
 src/happy_vllm/model/__init__.py
 src/happy_vllm/model/model_base.py
-src/happy_vllm/model/openai_serving_chat_fixed.py
 src/happy_vllm/routers/__init__.py
 src/happy_vllm/routers/functional.py
 src/happy_vllm/routers/technical.py
 src/happy_vllm/routers/schemas/__init__.py
 src/happy_vllm/routers/schemas/functional.py
 src/happy_vllm/routers/schemas/technical.py
 src/happy_vllm/routers/schemas/utils.py
```

### Comparing `happy_vllm-1.1.1/tests/test_json_format.py` & `happy_vllm-1.1.2/tests/test_json_format.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.1/tests/test_model_base.py` & `happy_vllm-1.1.2/tests/test_model_base.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.1/tests/test_response_pool.py` & `happy_vllm-1.1.2/tests/test_response_pool.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.1/tests/test_routers_functionnal.py` & `happy_vllm-1.1.2/tests/test_routers_functionnal.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.1/tests/test_routers_technical.py` & `happy_vllm-1.1.2/tests/test_routers_technical.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.1/tests/test_schemas_utils.py` & `happy_vllm-1.1.2/tests/test_schemas_utils.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.1/tests/test_utils.py` & `happy_vllm-1.1.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.1/tests/test_utils_args.py` & `happy_vllm-1.1.2/tests/test_utils_args.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.1/tests/test_utils_parse_logits_processors.py` & `happy_vllm-1.1.2/tests/test_utils_parse_logits_processors.py`

 * *Files identical despite different names*

