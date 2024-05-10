# Comparing `tmp/promptmodel-0.1.8.tar.gz` & `tmp/promptmodel-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptmodel-0.1.8.tar", last modified: Fri Dec 22 07:29:40 2023, max compression
+gzip compressed data, was "promptmodel-0.1.9.tar", last modified: Fri Dec 22 09:16:42 2023, max compression
```

## Comparing `promptmodel-0.1.8.tar` & `promptmodel-0.1.9.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 aschung    (501) staff       (20)        0 2023-12-22 07:29:40.342261 promptmodel-0.1.8/
--rw-r--r--   0 aschung    (501) staff       (20)        0 2023-12-15 03:23:34.000000 promptmodel-0.1.8/LICENSE
--rw-r--r--   0 aschung    (501) staff       (20)     1384 2023-12-22 07:29:40.341897 promptmodel-0.1.8/PKG-INFO
--rw-r--r--   0 aschung    (501) staff       (20)      999 2023-12-15 03:23:34.000000 promptmodel-0.1.8/README.md
-drwxr-xr-x   0 aschung    (501) staff       (20)        0 2023-12-22 07:29:40.302212 promptmodel-0.1.8/promptmodel/
--rw-r--r--   0 aschung    (501) staff       (20)      314 2023-12-15 03:23:34.000000 promptmodel-0.1.8/promptmodel/STARTER.py
--rw-r--r--   0 aschung    (501) staff       (20)      186 2023-12-22 07:28:21.000000 promptmodel-0.1.8/promptmodel/__init__.py
-drwxr-xr-x   0 aschung    (501) staff       (20)        0 2023-12-22 07:29:40.305185 promptmodel-0.1.8/promptmodel/apis/
--rw-r--r--   0 aschung    (501) staff       (20)       16 2023-12-15 03:23:34.000000 promptmodel-0.1.8/promptmodel/apis/__init__.py
--rw-r--r--   0 aschung    (501) staff       (20)     7643 2023-12-15 03:23:34.000000 promptmodel-0.1.8/promptmodel/apis/base.py
--rw-r--r--   0 aschung    (501) staff       (20)    13145 2023-12-22 07:27:34.000000 promptmodel-0.1.8/promptmodel/chat_model.py
-drwxr-xr-x   0 aschung    (501) staff       (20)        0 2023-12-22 07:29:40.309113 promptmodel-0.1.8/promptmodel/cli/
--rw-r--r--   0 aschung    (501) staff       (20)       16 2023-12-15 03:23:34.000000 promptmodel-0.1.8/promptmodel/cli/__init__.py
-drwxr-xr-x   0 aschung    (501) staff       (20)        0 2023-12-22 07:29:40.313278 promptmodel-0.1.8/promptmodel/cli/commands/
--rw-r--r--   0 aschung    (501) staff       (20)       16 2023-12-15 03:23:34.000000 promptmodel-0.1.8/promptmodel/cli/commands/__init__.py
--rw-r--r--   0 aschung    (501) staff       (20)     1154 2023-12-22 07:27:34.000000 promptmodel-0.1.8/promptmodel/cli/commands/configure.py
--rw-r--r--   0 aschung    (501) staff       (20)     4845 2023-12-22 07:27:34.000000 promptmodel-0.1.8/promptmodel/cli/commands/connect.py
--rw-r--r--   0 aschung    (501) staff       (20)    27934 2023-12-15 03:23:34.000000 promptmodel-0.1.8/promptmodel/cli/commands/dev.py
--rw-r--r--   0 aschung    (501) staff       (20)     1019 2023-12-15 03:23:34.000000 promptmodel-0.1.8/promptmodel/cli/commands/fix.py
--rw-r--r--   0 aschung    (501) staff       (20)     1191 2023-12-15 03:23:34.000000 promptmodel-0.1.8/promptmodel/cli/commands/init.py
--rw-r--r--   0 aschung    (501) staff       (20)     1517 2023-12-22 07:27:34.000000 promptmodel-0.1.8/promptmodel/cli/commands/login.py
--rw-r--r--   0 aschung    (501) staff       (20)      764 2023-12-22 07:27:34.000000 promptmodel-0.1.8/promptmodel/cli/commands/project.py
--rw-r--r--   0 aschung    (501) staff       (20)      985 2023-12-15 03:23:34.000000 promptmodel-0.1.8/promptmodel/cli/main.py
--rw-r--r--   0 aschung    (501) staff       (20)      371 2023-12-15 03:23:34.000000 promptmodel-0.1.8/promptmodel/cli/signal_handler.py
--rw-r--r--   0 aschung    (501) staff       (20)     1731 2023-12-22 07:27:34.000000 promptmodel-0.1.8/promptmodel/cli/utils.py
--rw-r--r--   0 aschung    (501) staff       (20)      943 2023-12-22 07:27:39.000000 promptmodel-0.1.8/promptmodel/constants.py
-drwxr-xr-x   0 aschung    (501) staff       (20)        0 2023-12-22 07:29:40.316723 promptmodel-0.1.8/promptmodel/database/
--rw-r--r--   0 aschung    (501) staff       (20)       16 2023-12-15 03:23:34.000000 promptmodel-0.1.8/promptmodel/database/__init__.py
--rw-r--r--   0 aschung    (501) staff       (20)      159 2023-12-15 03:23:34.000000 promptmodel-0.1.8/promptmodel/database/config.py
--rw-r--r--   0 aschung    (501) staff       (20)     2959 2023-12-15 03:23:34.000000 promptmodel-0.1.8/promptmodel/database/crud.py
--rw-r--r--   0 aschung    (501) staff       (20)     8859 2023-12-15 03:23:34.000000 promptmodel-0.1.8/promptmodel/database/crud_chat.py
--rw-r--r--   0 aschung    (501) staff       (20)     1829 2023-12-15 03:23:34.000000 promptmodel-0.1.8/promptmodel/database/models.py
--rw-r--r--   0 aschung    (501) staff       (20)     1086 2023-12-15 03:23:34.000000 promptmodel-0.1.8/promptmodel/database/models_chat.py
--rw-r--r--   0 aschung    (501) staff       (20)     1016 2023-12-15 03:23:34.000000 promptmodel-0.1.8/promptmodel/database/orm.py
--rw-r--r--   0 aschung    (501) staff       (20)     5033 2023-12-15 03:23:34.000000 promptmodel-0.1.8/promptmodel/dev_app.py
--rw-r--r--   0 aschung    (501) staff       (20)    15801 2023-12-22 07:27:34.000000 promptmodel-0.1.8/promptmodel/function_model.py
-drwxr-xr-x   0 aschung    (501) staff       (20)        0 2023-12-22 07:29:40.319330 promptmodel-0.1.8/promptmodel/llms/
--rw-r--r--   0 aschung    (501) staff       (20)       16 2023-12-15 03:23:34.000000 promptmodel-0.1.8/promptmodel/llms/__init__.py
--rw-r--r--   0 aschung    (501) staff       (20)    71215 2023-12-15 03:23:34.000000 promptmodel-0.1.8/promptmodel/llms/llm.py
--rw-r--r--   0 aschung    (501) staff       (20)     6589 2023-12-15 03:23:34.000000 promptmodel-0.1.8/promptmodel/llms/llm_dev.py
--rw-r--r--   0 aschung    (501) staff       (20)    36920 2023-12-22 07:27:34.000000 promptmodel-0.1.8/promptmodel/llms/llm_proxy.py
--rw-r--r--   0 aschung    (501) staff       (20)     5074 2023-12-22 07:27:34.000000 promptmodel-0.1.8/promptmodel/promptmodel_init.py
-drwxr-xr-x   0 aschung    (501) staff       (20)        0 2023-12-22 07:29:40.321474 promptmodel-0.1.8/promptmodel/types/
--rw-r--r--   0 aschung    (501) staff       (20)      238 2023-12-15 03:23:34.000000 promptmodel-0.1.8/promptmodel/types/__init__.py
--rw-r--r--   0 aschung    (501) staff       (20)     2518 2023-12-15 03:23:34.000000 promptmodel-0.1.8/promptmodel/types/enums.py
--rw-r--r--   0 aschung    (501) staff       (20)     1089 2023-12-22 07:27:34.000000 promptmodel-0.1.8/promptmodel/types/request.py
--rw-r--r--   0 aschung    (501) staff       (20)     3204 2023-12-15 03:23:34.000000 promptmodel-0.1.8/promptmodel/types/response.py
-drwxr-xr-x   0 aschung    (501) staff       (20)        0 2023-12-22 07:29:40.325412 promptmodel-0.1.8/promptmodel/utils/
--rw-r--r--   0 aschung    (501) staff       (20)       16 2023-12-15 03:23:34.000000 promptmodel-0.1.8/promptmodel/utils/__init__.py
--rw-r--r--   0 aschung    (501) staff       (20)      587 2023-12-15 03:23:34.000000 promptmodel-0.1.8/promptmodel/utils/async_utils.py
--rw-r--r--   0 aschung    (501) staff       (20)     3205 2023-12-15 03:23:34.000000 promptmodel-0.1.8/promptmodel/utils/config_utils.py
--rw-r--r--   0 aschung    (501) staff       (20)     1134 2023-12-15 03:23:34.000000 promptmodel-0.1.8/promptmodel/utils/crypto.py
--rw-r--r--   0 aschung    (501) staff       (20)      910 2023-12-15 03:23:34.000000 promptmodel-0.1.8/promptmodel/utils/logger.py
--rw-r--r--   0 aschung    (501) staff       (20)      810 2023-12-15 03:23:34.000000 promptmodel-0.1.8/promptmodel/utils/output_utils.py
--rw-r--r--   0 aschung    (501) staff       (20)      586 2023-12-15 03:23:34.000000 promptmodel-0.1.8/promptmodel/utils/random_utils.py
--rw-r--r--   0 aschung    (501) staff       (20)     4009 2023-12-15 03:23:34.000000 promptmodel-0.1.8/promptmodel/utils/token_counting.py
-drwxr-xr-x   0 aschung    (501) staff       (20)        0 2023-12-22 07:29:40.326914 promptmodel-0.1.8/promptmodel/websocket/
--rw-r--r--   0 aschung    (501) staff       (20)       95 2023-12-15 03:23:34.000000 promptmodel-0.1.8/promptmodel/websocket/__init__.py
--rw-r--r--   0 aschung    (501) staff       (20)     3840 2023-12-15 03:23:34.000000 promptmodel-0.1.8/promptmodel/websocket/reload_handler.py
--rw-r--r--   0 aschung    (501) staff       (20)    25227 2023-12-15 03:23:34.000000 promptmodel-0.1.8/promptmodel/websocket/websocket_client.py
-drwxr-xr-x   0 aschung    (501) staff       (20)        0 2023-12-22 07:29:40.304246 promptmodel-0.1.8/promptmodel.egg-info/
--rw-r--r--   0 aschung    (501) staff       (20)     1384 2023-12-22 07:29:40.000000 promptmodel-0.1.8/promptmodel.egg-info/PKG-INFO
--rw-r--r--   0 aschung    (501) staff       (20)     2774 2023-12-22 07:29:40.000000 promptmodel-0.1.8/promptmodel.egg-info/SOURCES.txt
--rw-r--r--   0 aschung    (501) staff       (20)        1 2023-12-22 07:29:40.000000 promptmodel-0.1.8/promptmodel.egg-info/dependency_links.txt
--rw-r--r--   0 aschung    (501) staff       (20)       52 2023-12-22 07:29:40.000000 promptmodel-0.1.8/promptmodel.egg-info/entry_points.txt
--rw-r--r--   0 aschung    (501) staff       (20)      167 2023-12-22 07:29:40.000000 promptmodel-0.1.8/promptmodel.egg-info/requires.txt
--rw-r--r--   0 aschung    (501) staff       (20)       18 2023-12-22 07:29:40.000000 promptmodel-0.1.8/promptmodel.egg-info/top_level.txt
--rw-r--r--   0 aschung    (501) staff       (20)       38 2023-12-22 07:29:40.342332 promptmodel-0.1.8/setup.cfg
--rw-r--r--   0 aschung    (501) staff       (20)     1397 2023-12-22 07:28:33.000000 promptmodel-0.1.8/setup.py
-drwxr-xr-x   0 aschung    (501) staff       (20)        0 2023-12-22 07:29:40.327829 promptmodel-0.1.8/tests/
--rw-r--r--   0 aschung    (501) staff       (20)        0 2023-12-15 03:23:34.000000 promptmodel-0.1.8/tests/__init__.py
-drwxr-xr-x   0 aschung    (501) staff       (20)        0 2023-12-22 07:29:40.328384 promptmodel-0.1.8/tests/api_client/
--rw-r--r--   0 aschung    (501) staff       (20)        0 2023-12-15 03:23:34.000000 promptmodel-0.1.8/tests/api_client/__init__.py
--rw-r--r--   0 aschung    (501) staff       (20)     4995 2023-12-15 03:23:34.000000 promptmodel-0.1.8/tests/api_client/api_client_test.py
-drwxr-xr-x   0 aschung    (501) staff       (20)        0 2023-12-22 07:29:40.329890 promptmodel-0.1.8/tests/chat_model/
--rw-r--r--   0 aschung    (501) staff       (20)        0 2023-12-15 03:23:34.000000 promptmodel-0.1.8/tests/chat_model/__init__.py
--rw-r--r--   0 aschung    (501) staff       (20)     7318 2023-12-15 03:23:34.000000 promptmodel-0.1.8/tests/chat_model/chat_model_test.py
--rw-r--r--   0 aschung    (501) staff       (20)     1627 2023-12-15 03:23:34.000000 promptmodel-0.1.8/tests/chat_model/conftest.py
--rw-r--r--   0 aschung    (501) staff       (20)      291 2023-12-15 03:23:34.000000 promptmodel-0.1.8/tests/chat_model/registering_meta_test.py
-drwxr-xr-x   0 aschung    (501) staff       (20)        0 2023-12-22 07:29:40.330300 promptmodel-0.1.8/tests/cli/
--rw-r--r--   0 aschung    (501) staff       (20)      321 2023-12-15 03:23:34.000000 promptmodel-0.1.8/tests/cli/dev_test.py
--rw-r--r--   0 aschung    (501) staff       (20)      568 2023-12-15 03:23:34.000000 promptmodel-0.1.8/tests/constants.py
-drwxr-xr-x   0 aschung    (501) staff       (20)        0 2023-12-22 07:29:40.332489 promptmodel-0.1.8/tests/function_model/
--rw-r--r--   0 aschung    (501) staff       (20)        0 2023-12-15 03:23:34.000000 promptmodel-0.1.8/tests/function_model/__init__.py
--rw-r--r--   0 aschung    (501) staff       (20)      975 2023-12-15 03:23:34.000000 promptmodel-0.1.8/tests/function_model/conftest.py
--rw-r--r--   0 aschung    (501) staff       (20)    11364 2023-12-15 03:23:34.000000 promptmodel-0.1.8/tests/function_model/function_model_test.py
--rw-r--r--   0 aschung    (501) staff       (20)      295 2023-12-15 03:23:34.000000 promptmodel-0.1.8/tests/function_model/registering_meta_test.py
-drwxr-xr-x   0 aschung    (501) staff       (20)        0 2023-12-22 07:29:40.336291 promptmodel-0.1.8/tests/llm/
--rw-r--r--   0 aschung    (501) staff       (20)        0 2023-12-15 03:23:34.000000 promptmodel-0.1.8/tests/llm/__init__.py
--rw-r--r--   0 aschung    (501) staff       (20)    15073 2023-12-15 03:23:34.000000 promptmodel-0.1.8/tests/llm/error_case_test.py
--rw-r--r--   0 aschung    (501) staff       (20)    10006 2023-12-15 03:23:34.000000 promptmodel-0.1.8/tests/llm/function_call_test.py
-drwxr-xr-x   0 aschung    (501) staff       (20)        0 2023-12-22 07:29:40.336903 promptmodel-0.1.8/tests/llm/llm_dev/
--rw-r--r--   0 aschung    (501) staff       (20)        0 2023-12-15 03:23:34.000000 promptmodel-0.1.8/tests/llm/llm_dev/__init__.py
--rw-r--r--   0 aschung    (501) staff       (20)        0 2023-12-15 03:23:34.000000 promptmodel-0.1.8/tests/llm/llm_dev/llm_dev_test.py
-drwxr-xr-x   0 aschung    (501) staff       (20)        0 2023-12-22 07:29:40.338296 promptmodel-0.1.8/tests/llm/llm_proxy/
--rw-r--r--   0 aschung    (501) staff       (20)        0 2023-12-15 03:23:34.000000 promptmodel-0.1.8/tests/llm/llm_proxy/__init__.py
--rw-r--r--   0 aschung    (501) staff       (20)     2335 2023-12-15 03:23:34.000000 promptmodel-0.1.8/tests/llm/llm_proxy/conftest.py
--rw-r--r--   0 aschung    (501) staff       (20)     5344 2023-12-15 03:23:34.000000 promptmodel-0.1.8/tests/llm/llm_proxy/proxy_chat_test.py
--rw-r--r--   0 aschung    (501) staff       (20)     9897 2023-12-15 03:23:34.000000 promptmodel-0.1.8/tests/llm/llm_proxy/proxy_test.py
--rw-r--r--   0 aschung    (501) staff       (20)    29305 2023-12-15 03:23:34.000000 promptmodel-0.1.8/tests/llm/parse_test.py
--rw-r--r--   0 aschung    (501) staff       (20)    12352 2023-12-15 03:23:34.000000 promptmodel-0.1.8/tests/llm/stream_function_call_test.py
--rw-r--r--   0 aschung    (501) staff       (20)     4297 2023-12-15 03:23:34.000000 promptmodel-0.1.8/tests/llm/stream_test.py
--rw-r--r--   0 aschung    (501) staff       (20)    12445 2023-12-15 03:23:34.000000 promptmodel-0.1.8/tests/llm/stream_tool_calls_test.py
--rw-r--r--   0 aschung    (501) staff       (20)     9945 2023-12-15 03:23:34.000000 promptmodel-0.1.8/tests/llm/tool_calls_test.py
-drwxr-xr-x   0 aschung    (501) staff       (20)        0 2023-12-22 07:29:40.338887 promptmodel-0.1.8/tests/utils/
--rw-r--r--   0 aschung    (501) staff       (20)     1190 2023-12-15 03:23:34.000000 promptmodel-0.1.8/tests/utils/async_util_test.py
-drwxr-xr-x   0 aschung    (501) staff       (20)        0 2023-12-22 07:29:40.341212 promptmodel-0.1.8/tests/websocket_client/
--rw-r--r--   0 aschung    (501) staff       (20)        0 2023-12-15 03:23:34.000000 promptmodel-0.1.8/tests/websocket_client/__init__.py
--rw-r--r--   0 aschung    (501) staff       (20)     1085 2023-12-15 03:23:34.000000 promptmodel-0.1.8/tests/websocket_client/conftest.py
--rw-r--r--   0 aschung    (501) staff       (20)     1740 2023-12-15 03:23:34.000000 promptmodel-0.1.8/tests/websocket_client/local_task_test.py
--rw-r--r--   0 aschung    (501) staff       (20)     7933 2023-12-15 03:23:34.000000 promptmodel-0.1.8/tests/websocket_client/run_chatmodel_test.py
--rw-r--r--   0 aschung    (501) staff       (20)    12232 2023-12-15 03:23:34.000000 promptmodel-0.1.8/tests/websocket_client/run_promptmodel_test.py
+drwxr-xr-x   0 aschung    (501) staff       (20)        0 2023-12-22 09:16:42.092718 promptmodel-0.1.9/
+-rw-r--r--   0 aschung    (501) staff       (20)        0 2023-12-15 03:23:34.000000 promptmodel-0.1.9/LICENSE
+-rw-r--r--   0 aschung    (501) staff       (20)     1384 2023-12-22 09:16:42.092203 promptmodel-0.1.9/PKG-INFO
+-rw-r--r--   0 aschung    (501) staff       (20)      999 2023-12-15 03:23:34.000000 promptmodel-0.1.9/README.md
+drwxr-xr-x   0 aschung    (501) staff       (20)        0 2023-12-22 09:16:42.013919 promptmodel-0.1.9/promptmodel/
+-rw-r--r--   0 aschung    (501) staff       (20)      314 2023-12-15 03:23:34.000000 promptmodel-0.1.9/promptmodel/STARTER.py
+-rw-r--r--   0 aschung    (501) staff       (20)      186 2023-12-22 09:16:34.000000 promptmodel-0.1.9/promptmodel/__init__.py
+drwxr-xr-x   0 aschung    (501) staff       (20)        0 2023-12-22 09:16:42.020882 promptmodel-0.1.9/promptmodel/apis/
+-rw-r--r--   0 aschung    (501) staff       (20)       16 2023-12-15 03:23:34.000000 promptmodel-0.1.9/promptmodel/apis/__init__.py
+-rw-r--r--   0 aschung    (501) staff       (20)     7643 2023-12-15 03:23:34.000000 promptmodel-0.1.9/promptmodel/apis/base.py
+-rw-r--r--   0 aschung    (501) staff       (20)    13145 2023-12-22 07:27:34.000000 promptmodel-0.1.9/promptmodel/chat_model.py
+drwxr-xr-x   0 aschung    (501) staff       (20)        0 2023-12-22 09:16:42.024167 promptmodel-0.1.9/promptmodel/cli/
+-rw-r--r--   0 aschung    (501) staff       (20)       16 2023-12-15 03:23:34.000000 promptmodel-0.1.9/promptmodel/cli/__init__.py
+drwxr-xr-x   0 aschung    (501) staff       (20)        0 2023-12-22 09:16:42.033405 promptmodel-0.1.9/promptmodel/cli/commands/
+-rw-r--r--   0 aschung    (501) staff       (20)       16 2023-12-15 03:23:34.000000 promptmodel-0.1.9/promptmodel/cli/commands/__init__.py
+-rw-r--r--   0 aschung    (501) staff       (20)     1154 2023-12-22 07:27:34.000000 promptmodel-0.1.9/promptmodel/cli/commands/configure.py
+-rw-r--r--   0 aschung    (501) staff       (20)     4845 2023-12-22 07:27:34.000000 promptmodel-0.1.9/promptmodel/cli/commands/connect.py
+-rw-r--r--   0 aschung    (501) staff       (20)    27934 2023-12-15 03:23:34.000000 promptmodel-0.1.9/promptmodel/cli/commands/dev.py
+-rw-r--r--   0 aschung    (501) staff       (20)     1019 2023-12-15 03:23:34.000000 promptmodel-0.1.9/promptmodel/cli/commands/fix.py
+-rw-r--r--   0 aschung    (501) staff       (20)     1191 2023-12-15 03:23:34.000000 promptmodel-0.1.9/promptmodel/cli/commands/init.py
+-rw-r--r--   0 aschung    (501) staff       (20)     1517 2023-12-22 07:27:34.000000 promptmodel-0.1.9/promptmodel/cli/commands/login.py
+-rw-r--r--   0 aschung    (501) staff       (20)      764 2023-12-22 07:27:34.000000 promptmodel-0.1.9/promptmodel/cli/commands/project.py
+-rw-r--r--   0 aschung    (501) staff       (20)      985 2023-12-15 03:23:34.000000 promptmodel-0.1.9/promptmodel/cli/main.py
+-rw-r--r--   0 aschung    (501) staff       (20)      371 2023-12-15 03:23:34.000000 promptmodel-0.1.9/promptmodel/cli/signal_handler.py
+-rw-r--r--   0 aschung    (501) staff       (20)     1731 2023-12-22 07:27:34.000000 promptmodel-0.1.9/promptmodel/cli/utils.py
+-rw-r--r--   0 aschung    (501) staff       (20)      943 2023-12-22 07:27:39.000000 promptmodel-0.1.9/promptmodel/constants.py
+drwxr-xr-x   0 aschung    (501) staff       (20)        0 2023-12-22 09:16:42.039703 promptmodel-0.1.9/promptmodel/database/
+-rw-r--r--   0 aschung    (501) staff       (20)       16 2023-12-15 03:23:34.000000 promptmodel-0.1.9/promptmodel/database/__init__.py
+-rw-r--r--   0 aschung    (501) staff       (20)      159 2023-12-15 03:23:34.000000 promptmodel-0.1.9/promptmodel/database/config.py
+-rw-r--r--   0 aschung    (501) staff       (20)     2959 2023-12-15 03:23:34.000000 promptmodel-0.1.9/promptmodel/database/crud.py
+-rw-r--r--   0 aschung    (501) staff       (20)     8859 2023-12-15 03:23:34.000000 promptmodel-0.1.9/promptmodel/database/crud_chat.py
+-rw-r--r--   0 aschung    (501) staff       (20)     1829 2023-12-15 03:23:34.000000 promptmodel-0.1.9/promptmodel/database/models.py
+-rw-r--r--   0 aschung    (501) staff       (20)     1086 2023-12-15 03:23:34.000000 promptmodel-0.1.9/promptmodel/database/models_chat.py
+-rw-r--r--   0 aschung    (501) staff       (20)     1016 2023-12-15 03:23:34.000000 promptmodel-0.1.9/promptmodel/database/orm.py
+-rw-r--r--   0 aschung    (501) staff       (20)     5033 2023-12-15 03:23:34.000000 promptmodel-0.1.9/promptmodel/dev_app.py
+-rw-r--r--   0 aschung    (501) staff       (20)    15801 2023-12-22 09:15:26.000000 promptmodel-0.1.9/promptmodel/function_model.py
+drwxr-xr-x   0 aschung    (501) staff       (20)        0 2023-12-22 09:16:42.045158 promptmodel-0.1.9/promptmodel/llms/
+-rw-r--r--   0 aschung    (501) staff       (20)       16 2023-12-15 03:23:34.000000 promptmodel-0.1.9/promptmodel/llms/__init__.py
+-rw-r--r--   0 aschung    (501) staff       (20)    71215 2023-12-15 03:23:34.000000 promptmodel-0.1.9/promptmodel/llms/llm.py
+-rw-r--r--   0 aschung    (501) staff       (20)     6589 2023-12-22 09:15:33.000000 promptmodel-0.1.9/promptmodel/llms/llm_dev.py
+-rw-r--r--   0 aschung    (501) staff       (20)    36920 2023-12-22 09:15:39.000000 promptmodel-0.1.9/promptmodel/llms/llm_proxy.py
+-rw-r--r--   0 aschung    (501) staff       (20)     5074 2023-12-22 07:27:34.000000 promptmodel-0.1.9/promptmodel/promptmodel_init.py
+drwxr-xr-x   0 aschung    (501) staff       (20)        0 2023-12-22 09:16:42.050547 promptmodel-0.1.9/promptmodel/types/
+-rw-r--r--   0 aschung    (501) staff       (20)      238 2023-12-15 03:23:34.000000 promptmodel-0.1.9/promptmodel/types/__init__.py
+-rw-r--r--   0 aschung    (501) staff       (20)     2518 2023-12-15 03:23:34.000000 promptmodel-0.1.9/promptmodel/types/enums.py
+-rw-r--r--   0 aschung    (501) staff       (20)     1089 2023-12-22 07:27:34.000000 promptmodel-0.1.9/promptmodel/types/request.py
+-rw-r--r--   0 aschung    (501) staff       (20)     3204 2023-12-15 03:23:34.000000 promptmodel-0.1.9/promptmodel/types/response.py
+drwxr-xr-x   0 aschung    (501) staff       (20)        0 2023-12-22 09:16:42.058497 promptmodel-0.1.9/promptmodel/utils/
+-rw-r--r--   0 aschung    (501) staff       (20)       16 2023-12-15 03:23:34.000000 promptmodel-0.1.9/promptmodel/utils/__init__.py
+-rw-r--r--   0 aschung    (501) staff       (20)      587 2023-12-15 03:23:34.000000 promptmodel-0.1.9/promptmodel/utils/async_utils.py
+-rw-r--r--   0 aschung    (501) staff       (20)     3205 2023-12-15 03:23:34.000000 promptmodel-0.1.9/promptmodel/utils/config_utils.py
+-rw-r--r--   0 aschung    (501) staff       (20)     1134 2023-12-15 03:23:34.000000 promptmodel-0.1.9/promptmodel/utils/crypto.py
+-rw-r--r--   0 aschung    (501) staff       (20)      910 2023-12-15 03:23:34.000000 promptmodel-0.1.9/promptmodel/utils/logger.py
+-rw-r--r--   0 aschung    (501) staff       (20)      810 2023-12-15 03:23:34.000000 promptmodel-0.1.9/promptmodel/utils/output_utils.py
+-rw-r--r--   0 aschung    (501) staff       (20)      586 2023-12-15 03:23:34.000000 promptmodel-0.1.9/promptmodel/utils/random_utils.py
+-rw-r--r--   0 aschung    (501) staff       (20)     4009 2023-12-15 03:23:34.000000 promptmodel-0.1.9/promptmodel/utils/token_counting.py
+drwxr-xr-x   0 aschung    (501) staff       (20)        0 2023-12-22 09:16:42.061253 promptmodel-0.1.9/promptmodel/websocket/
+-rw-r--r--   0 aschung    (501) staff       (20)       95 2023-12-15 03:23:34.000000 promptmodel-0.1.9/promptmodel/websocket/__init__.py
+-rw-r--r--   0 aschung    (501) staff       (20)     3840 2023-12-15 03:23:34.000000 promptmodel-0.1.9/promptmodel/websocket/reload_handler.py
+-rw-r--r--   0 aschung    (501) staff       (20)    25227 2023-12-22 08:47:45.000000 promptmodel-0.1.9/promptmodel/websocket/websocket_client.py
+drwxr-xr-x   0 aschung    (501) staff       (20)        0 2023-12-22 09:16:42.018225 promptmodel-0.1.9/promptmodel.egg-info/
+-rw-r--r--   0 aschung    (501) staff       (20)     1384 2023-12-22 09:16:41.000000 promptmodel-0.1.9/promptmodel.egg-info/PKG-INFO
+-rw-r--r--   0 aschung    (501) staff       (20)     2774 2023-12-22 09:16:41.000000 promptmodel-0.1.9/promptmodel.egg-info/SOURCES.txt
+-rw-r--r--   0 aschung    (501) staff       (20)        1 2023-12-22 09:16:41.000000 promptmodel-0.1.9/promptmodel.egg-info/dependency_links.txt
+-rw-r--r--   0 aschung    (501) staff       (20)       52 2023-12-22 09:16:41.000000 promptmodel-0.1.9/promptmodel.egg-info/entry_points.txt
+-rw-r--r--   0 aschung    (501) staff       (20)      167 2023-12-22 09:16:41.000000 promptmodel-0.1.9/promptmodel.egg-info/requires.txt
+-rw-r--r--   0 aschung    (501) staff       (20)       18 2023-12-22 09:16:41.000000 promptmodel-0.1.9/promptmodel.egg-info/top_level.txt
+-rw-r--r--   0 aschung    (501) staff       (20)       38 2023-12-22 09:16:42.092973 promptmodel-0.1.9/setup.cfg
+-rw-r--r--   0 aschung    (501) staff       (20)     1397 2023-12-22 09:16:39.000000 promptmodel-0.1.9/setup.py
+drwxr-xr-x   0 aschung    (501) staff       (20)        0 2023-12-22 09:16:42.063208 promptmodel-0.1.9/tests/
+-rw-r--r--   0 aschung    (501) staff       (20)        0 2023-12-15 03:23:34.000000 promptmodel-0.1.9/tests/__init__.py
+drwxr-xr-x   0 aschung    (501) staff       (20)        0 2023-12-22 09:16:42.064680 promptmodel-0.1.9/tests/api_client/
+-rw-r--r--   0 aschung    (501) staff       (20)        0 2023-12-15 03:23:34.000000 promptmodel-0.1.9/tests/api_client/__init__.py
+-rw-r--r--   0 aschung    (501) staff       (20)     4995 2023-12-15 03:23:34.000000 promptmodel-0.1.9/tests/api_client/api_client_test.py
+drwxr-xr-x   0 aschung    (501) staff       (20)        0 2023-12-22 09:16:42.067854 promptmodel-0.1.9/tests/chat_model/
+-rw-r--r--   0 aschung    (501) staff       (20)        0 2023-12-15 03:23:34.000000 promptmodel-0.1.9/tests/chat_model/__init__.py
+-rw-r--r--   0 aschung    (501) staff       (20)     7318 2023-12-15 03:23:34.000000 promptmodel-0.1.9/tests/chat_model/chat_model_test.py
+-rw-r--r--   0 aschung    (501) staff       (20)     1627 2023-12-15 03:23:34.000000 promptmodel-0.1.9/tests/chat_model/conftest.py
+-rw-r--r--   0 aschung    (501) staff       (20)      291 2023-12-15 03:23:34.000000 promptmodel-0.1.9/tests/chat_model/registering_meta_test.py
+drwxr-xr-x   0 aschung    (501) staff       (20)        0 2023-12-22 09:16:42.068777 promptmodel-0.1.9/tests/cli/
+-rw-r--r--   0 aschung    (501) staff       (20)      321 2023-12-15 03:23:34.000000 promptmodel-0.1.9/tests/cli/dev_test.py
+-rw-r--r--   0 aschung    (501) staff       (20)      568 2023-12-15 03:23:34.000000 promptmodel-0.1.9/tests/constants.py
+drwxr-xr-x   0 aschung    (501) staff       (20)        0 2023-12-22 09:16:42.071964 promptmodel-0.1.9/tests/function_model/
+-rw-r--r--   0 aschung    (501) staff       (20)        0 2023-12-15 03:23:34.000000 promptmodel-0.1.9/tests/function_model/__init__.py
+-rw-r--r--   0 aschung    (501) staff       (20)      975 2023-12-15 03:23:34.000000 promptmodel-0.1.9/tests/function_model/conftest.py
+-rw-r--r--   0 aschung    (501) staff       (20)    11364 2023-12-15 03:23:34.000000 promptmodel-0.1.9/tests/function_model/function_model_test.py
+-rw-r--r--   0 aschung    (501) staff       (20)      295 2023-12-15 03:23:34.000000 promptmodel-0.1.9/tests/function_model/registering_meta_test.py
+drwxr-xr-x   0 aschung    (501) staff       (20)        0 2023-12-22 09:16:42.080087 promptmodel-0.1.9/tests/llm/
+-rw-r--r--   0 aschung    (501) staff       (20)        0 2023-12-15 03:23:34.000000 promptmodel-0.1.9/tests/llm/__init__.py
+-rw-r--r--   0 aschung    (501) staff       (20)    15073 2023-12-15 03:23:34.000000 promptmodel-0.1.9/tests/llm/error_case_test.py
+-rw-r--r--   0 aschung    (501) staff       (20)    10006 2023-12-15 03:23:34.000000 promptmodel-0.1.9/tests/llm/function_call_test.py
+drwxr-xr-x   0 aschung    (501) staff       (20)        0 2023-12-22 09:16:42.081780 promptmodel-0.1.9/tests/llm/llm_dev/
+-rw-r--r--   0 aschung    (501) staff       (20)        0 2023-12-15 03:23:34.000000 promptmodel-0.1.9/tests/llm/llm_dev/__init__.py
+-rw-r--r--   0 aschung    (501) staff       (20)        0 2023-12-15 03:23:34.000000 promptmodel-0.1.9/tests/llm/llm_dev/llm_dev_test.py
+drwxr-xr-x   0 aschung    (501) staff       (20)        0 2023-12-22 09:16:42.085505 promptmodel-0.1.9/tests/llm/llm_proxy/
+-rw-r--r--   0 aschung    (501) staff       (20)        0 2023-12-15 03:23:34.000000 promptmodel-0.1.9/tests/llm/llm_proxy/__init__.py
+-rw-r--r--   0 aschung    (501) staff       (20)     2335 2023-12-15 03:23:34.000000 promptmodel-0.1.9/tests/llm/llm_proxy/conftest.py
+-rw-r--r--   0 aschung    (501) staff       (20)     5344 2023-12-15 03:23:34.000000 promptmodel-0.1.9/tests/llm/llm_proxy/proxy_chat_test.py
+-rw-r--r--   0 aschung    (501) staff       (20)     9897 2023-12-15 03:23:34.000000 promptmodel-0.1.9/tests/llm/llm_proxy/proxy_test.py
+-rw-r--r--   0 aschung    (501) staff       (20)    29305 2023-12-15 03:23:34.000000 promptmodel-0.1.9/tests/llm/parse_test.py
+-rw-r--r--   0 aschung    (501) staff       (20)    12352 2023-12-15 03:23:34.000000 promptmodel-0.1.9/tests/llm/stream_function_call_test.py
+-rw-r--r--   0 aschung    (501) staff       (20)     4297 2023-12-15 03:23:34.000000 promptmodel-0.1.9/tests/llm/stream_test.py
+-rw-r--r--   0 aschung    (501) staff       (20)    12445 2023-12-15 03:23:34.000000 promptmodel-0.1.9/tests/llm/stream_tool_calls_test.py
+-rw-r--r--   0 aschung    (501) staff       (20)     9945 2023-12-15 03:23:34.000000 promptmodel-0.1.9/tests/llm/tool_calls_test.py
+drwxr-xr-x   0 aschung    (501) staff       (20)        0 2023-12-22 09:16:42.086433 promptmodel-0.1.9/tests/utils/
+-rw-r--r--   0 aschung    (501) staff       (20)     1190 2023-12-15 03:23:34.000000 promptmodel-0.1.9/tests/utils/async_util_test.py
+drwxr-xr-x   0 aschung    (501) staff       (20)        0 2023-12-22 09:16:42.090977 promptmodel-0.1.9/tests/websocket_client/
+-rw-r--r--   0 aschung    (501) staff       (20)        0 2023-12-15 03:23:34.000000 promptmodel-0.1.9/tests/websocket_client/__init__.py
+-rw-r--r--   0 aschung    (501) staff       (20)     1085 2023-12-15 03:23:34.000000 promptmodel-0.1.9/tests/websocket_client/conftest.py
+-rw-r--r--   0 aschung    (501) staff       (20)     1740 2023-12-15 03:23:34.000000 promptmodel-0.1.9/tests/websocket_client/local_task_test.py
+-rw-r--r--   0 aschung    (501) staff       (20)     7933 2023-12-15 03:23:34.000000 promptmodel-0.1.9/tests/websocket_client/run_chatmodel_test.py
+-rw-r--r--   0 aschung    (501) staff       (20)    12232 2023-12-15 03:23:34.000000 promptmodel-0.1.9/tests/websocket_client/run_promptmodel_test.py
```

### Comparing `promptmodel-0.1.8/PKG-INFO` & `promptmodel-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptmodel
-Version: 0.1.8
+Version: 0.1.9
 Summary: Prompt & model versioning on the cloud, built for developers.
 Home-page: https://github.com/weavel-ai/promptmodel
 Author: weavel
 Keywords: weavel,agent,llm,tools,promptmodel,llm agent,prompt,versioning,eval,evaluation,collaborative
 Requires-Python: >=3.8.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: promptmodel Version: 0.1.8 Summary: Prompt & model
+Metadata-Version: 2.1 Name: promptmodel Version: 0.1.9 Summary: Prompt & model
 versioning on the cloud, built for developers. Home-page: https://github.com/
 weavel-ai/promptmodel Author: weavel Keywords:
 weavel,agent,llm,tools,promptmodel,llm
 agent,prompt,versioning,eval,evaluation,collaborative Requires-Python: >=3.8.10
 Description-Content-Type: text/markdown License-File: LICENSE
                        _[_h_t_t_p_s_:_/_/_i_._i_m_g_u_r_._c_o_m_/_f_3_M_H_y_H_3_._p_n_g_]
                            ************ PPrroommppttmmooddeell ************
```

### Comparing `promptmodel-0.1.8/README.md` & `promptmodel-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/promptmodel/apis/base.py` & `promptmodel-0.1.9/promptmodel/apis/base.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/promptmodel/chat_model.py` & `promptmodel-0.1.9/promptmodel/chat_model.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/promptmodel/cli/commands/configure.py` & `promptmodel-0.1.9/promptmodel/cli/commands/configure.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/promptmodel/cli/commands/connect.py` & `promptmodel-0.1.9/promptmodel/cli/commands/connect.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/promptmodel/cli/commands/dev.py` & `promptmodel-0.1.9/promptmodel/cli/commands/dev.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/promptmodel/cli/commands/fix.py` & `promptmodel-0.1.9/promptmodel/cli/commands/fix.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/promptmodel/cli/commands/init.py` & `promptmodel-0.1.9/promptmodel/cli/commands/init.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/promptmodel/cli/commands/login.py` & `promptmodel-0.1.9/promptmodel/cli/commands/login.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/promptmodel/cli/commands/project.py` & `promptmodel-0.1.9/promptmodel/cli/commands/project.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/promptmodel/cli/main.py` & `promptmodel-0.1.9/promptmodel/cli/main.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/promptmodel/cli/utils.py` & `promptmodel-0.1.9/promptmodel/cli/utils.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/promptmodel/constants.py` & `promptmodel-0.1.9/promptmodel/constants.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/promptmodel/database/crud.py` & `promptmodel-0.1.9/promptmodel/database/crud.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/promptmodel/database/crud_chat.py` & `promptmodel-0.1.9/promptmodel/database/crud_chat.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/promptmodel/database/models.py` & `promptmodel-0.1.9/promptmodel/database/models.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/promptmodel/database/models_chat.py` & `promptmodel-0.1.9/promptmodel/database/models_chat.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/promptmodel/database/orm.py` & `promptmodel-0.1.9/promptmodel/database/orm.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/promptmodel/dev_app.py` & `promptmodel-0.1.9/promptmodel/dev_app.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/promptmodel/function_model.py` & `promptmodel-0.1.9/promptmodel/function_model.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/promptmodel/llms/llm.py` & `promptmodel-0.1.9/promptmodel/llms/llm.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/promptmodel/llms/llm_dev.py` & `promptmodel-0.1.9/promptmodel/llms/llm_dev.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/promptmodel/llms/llm_proxy.py` & `promptmodel-0.1.9/promptmodel/llms/llm_proxy.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/promptmodel/promptmodel_init.py` & `promptmodel-0.1.9/promptmodel/promptmodel_init.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/promptmodel/types/enums.py` & `promptmodel-0.1.9/promptmodel/types/enums.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/promptmodel/types/request.py` & `promptmodel-0.1.9/promptmodel/types/request.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/promptmodel/types/response.py` & `promptmodel-0.1.9/promptmodel/types/response.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/promptmodel/utils/async_utils.py` & `promptmodel-0.1.9/promptmodel/utils/async_utils.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/promptmodel/utils/config_utils.py` & `promptmodel-0.1.9/promptmodel/utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/promptmodel/utils/crypto.py` & `promptmodel-0.1.9/promptmodel/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/promptmodel/utils/logger.py` & `promptmodel-0.1.9/promptmodel/utils/logger.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/promptmodel/utils/output_utils.py` & `promptmodel-0.1.9/promptmodel/utils/output_utils.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/promptmodel/utils/random_utils.py` & `promptmodel-0.1.9/promptmodel/utils/random_utils.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/promptmodel/utils/token_counting.py` & `promptmodel-0.1.9/promptmodel/utils/token_counting.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/promptmodel/websocket/reload_handler.py` & `promptmodel-0.1.9/promptmodel/websocket/reload_handler.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/promptmodel/websocket/websocket_client.py` & `promptmodel-0.1.9/promptmodel/websocket/websocket_client.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/promptmodel.egg-info/PKG-INFO` & `promptmodel-0.1.9/promptmodel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptmodel
-Version: 0.1.8
+Version: 0.1.9
 Summary: Prompt & model versioning on the cloud, built for developers.
 Home-page: https://github.com/weavel-ai/promptmodel
 Author: weavel
 Keywords: weavel,agent,llm,tools,promptmodel,llm agent,prompt,versioning,eval,evaluation,collaborative
 Requires-Python: >=3.8.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: promptmodel Version: 0.1.8 Summary: Prompt & model
+Metadata-Version: 2.1 Name: promptmodel Version: 0.1.9 Summary: Prompt & model
 versioning on the cloud, built for developers. Home-page: https://github.com/
 weavel-ai/promptmodel Author: weavel Keywords:
 weavel,agent,llm,tools,promptmodel,llm
 agent,prompt,versioning,eval,evaluation,collaborative Requires-Python: >=3.8.10
 Description-Content-Type: text/markdown License-File: LICENSE
                        _[_h_t_t_p_s_:_/_/_i_._i_m_g_u_r_._c_o_m_/_f_3_M_H_y_H_3_._p_n_g_]
                            ************ PPrroommppttmmooddeell ************
```

### Comparing `promptmodel-0.1.8/promptmodel.egg-info/SOURCES.txt` & `promptmodel-0.1.9/promptmodel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/setup.py` & `promptmodel-0.1.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # Read README.md for the long description
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="promptmodel",
-    version="0.1.8",
+    version="0.1.9",
     packages=find_namespace_packages(),
     entry_points={
         "console_scripts": [
             "prompt = promptmodel.cli.main:app",
         ],
     },
     description="Prompt & model versioning on the cloud, built for developers.",
```

### Comparing `promptmodel-0.1.8/tests/api_client/api_client_test.py` & `promptmodel-0.1.9/tests/api_client/api_client_test.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/tests/chat_model/chat_model_test.py` & `promptmodel-0.1.9/tests/chat_model/chat_model_test.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/tests/chat_model/conftest.py` & `promptmodel-0.1.9/tests/chat_model/conftest.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/tests/constants.py` & `promptmodel-0.1.9/tests/constants.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/tests/function_model/conftest.py` & `promptmodel-0.1.9/tests/function_model/conftest.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/tests/function_model/function_model_test.py` & `promptmodel-0.1.9/tests/function_model/function_model_test.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/tests/llm/error_case_test.py` & `promptmodel-0.1.9/tests/llm/error_case_test.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/tests/llm/function_call_test.py` & `promptmodel-0.1.9/tests/llm/function_call_test.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/tests/llm/llm_proxy/conftest.py` & `promptmodel-0.1.9/tests/llm/llm_proxy/conftest.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/tests/llm/llm_proxy/proxy_chat_test.py` & `promptmodel-0.1.9/tests/llm/llm_proxy/proxy_chat_test.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/tests/llm/llm_proxy/proxy_test.py` & `promptmodel-0.1.9/tests/llm/llm_proxy/proxy_test.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/tests/llm/parse_test.py` & `promptmodel-0.1.9/tests/llm/parse_test.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/tests/llm/stream_function_call_test.py` & `promptmodel-0.1.9/tests/llm/stream_function_call_test.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/tests/llm/stream_test.py` & `promptmodel-0.1.9/tests/llm/stream_test.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/tests/llm/stream_tool_calls_test.py` & `promptmodel-0.1.9/tests/llm/stream_tool_calls_test.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/tests/llm/tool_calls_test.py` & `promptmodel-0.1.9/tests/llm/tool_calls_test.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/tests/utils/async_util_test.py` & `promptmodel-0.1.9/tests/utils/async_util_test.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/tests/websocket_client/conftest.py` & `promptmodel-0.1.9/tests/websocket_client/conftest.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/tests/websocket_client/local_task_test.py` & `promptmodel-0.1.9/tests/websocket_client/local_task_test.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/tests/websocket_client/run_chatmodel_test.py` & `promptmodel-0.1.9/tests/websocket_client/run_chatmodel_test.py`

 * *Files identical despite different names*

### Comparing `promptmodel-0.1.8/tests/websocket_client/run_promptmodel_test.py` & `promptmodel-0.1.9/tests/websocket_client/run_promptmodel_test.py`

 * *Files identical despite different names*

