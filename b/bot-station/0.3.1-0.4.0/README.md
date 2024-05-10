# Comparing `tmp/bot_station-0.3.1.tar.gz` & `tmp/bot_station-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bot_station-0.3.1.tar", last modified: Wed May  8 19:14:51 2024, max compression
+gzip compressed data, was "bot_station-0.4.0.tar", last modified: Fri May 10 20:07:13 2024, max compression
```

## Comparing `bot_station-0.3.1.tar` & `bot_station-0.4.0.tar`

### file list

```diff
@@ -1,86 +1,87 @@
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.177519 bot_station-0.3.1/
--rw-r--r--   0 mmarashan (1826057312) 593637566     1070 2024-05-05 19:58:38.000000 bot_station-0.3.1/LICENSE
--rw-r--r--   0 mmarashan (1826057312) 593637566      707 2024-05-08 19:14:51.177299 bot_station-0.3.1/PKG-INFO
--rw-r--r--   0 mmarashan (1826057312) 593637566       17 2024-05-05 19:58:38.000000 bot_station-0.3.1/README.md
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.166216 bot_station-0.3.1/bot_station/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/__init__.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.167618 bot_station-0.3.1/bot_station/api/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/api/__init__.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.167965 bot_station-0.3.1/bot_station/api/rest/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/api/rest/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566     6988 2024-05-08 06:14:06.000000 bot_station-0.3.1/bot_station/api/rest/api.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.170214 bot_station-0.3.1/bot_station/api/rest/model/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/api/rest/model/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      257 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/api/rest/model/bot_call_dto.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      331 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/api/rest/model/bot_call_result.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      486 2024-05-06 05:44:47.000000 bot_station-0.3.1/bot_station/api/rest/model/bot_creation_dto.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      126 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/api/rest/model/bot_creation_result.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      433 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/api/rest/model/bot_dto.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      401 2024-05-08 05:52:39.000000 bot_station-0.3.1/bot_station/api/rest/model/bot_train_dto.py
--rw-r--r--   0 mmarashan (1826057312) 593637566       90 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/api/rest/model/bot_train_result.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      204 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/api/rest/model/web_app_config.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.170404 bot_station-0.3.1/bot_station/data/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/data/__init__.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.170523 bot_station-0.3.1/bot_station/data/base/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/data/base/__init__.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.170916 bot_station-0.3.1/bot_station/data/base/database/
--rw-r--r--   0 mmarashan (1826057312) 593637566      975 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/data/base/database/UUID.py
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/data/base/database/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      428 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/data/base/database/base_db_dto.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.171542 bot_station-0.3.1/bot_station/data/bot/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/data/bot/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      992 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/data/bot/bot_factory_impl.py
--rw-r--r--   0 mmarashan (1826057312) 593637566     7893 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/data/bot/bot_impl.py
--rw-r--r--   0 mmarashan (1826057312) 593637566     2169 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/data/bot/chat_message_storage_impl.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.171808 bot_station-0.3.1/bot_station/data/bot/mapper/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/data/bot/mapper/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      972 2024-05-08 05:40:36.000000 bot_station-0.3.1/bot_station/data/bot/mapper/document_mapper.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.172238 bot_station-0.3.1/bot_station/data/bot/model/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/data/bot/model/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      238 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/data/bot/model/yandex_cloud_config.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.172563 bot_station-0.3.1/bot_station/data/bot_station/
--rw-r--r--   0 mmarashan (1826057312) 593637566      508 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/data/bot_station/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566     3061 2024-05-06 05:42:48.000000 bot_station-0.3.1/bot_station/data/bot_station/bot_registry_impl.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.172997 bot_station-0.3.1/bot_station/data/bot_station/model/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/data/bot_station/model/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      853 2024-05-06 05:42:37.000000 bot_station-0.3.1/bot_station/data/bot_station/model/bot_info_dto.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.173452 bot_station-0.3.1/bot_station/di/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/di/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566     1268 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/di/bot_station_module.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.173621 bot_station-0.3.1/bot_station/domain/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/domain/__init__.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.173957 bot_station-0.3.1/bot_station/domain/base/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/domain/base/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      544 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/domain/base/const.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      391 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/domain/base/utils.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.174526 bot_station-0.3.1/bot_station/domain/bot/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/domain/bot/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      673 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/domain/bot/bot.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      267 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/domain/bot/bot_factory.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      798 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/domain/bot/chat_message_storage.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.175533 bot_station-0.3.1/bot_station/domain/bot/model/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/domain/bot/model/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      222 2024-05-08 05:38:32.000000 bot_station-0.3.1/bot_station/domain/bot/model/document.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      350 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/domain/bot/model/lm_bot_meta_info.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      254 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/domain/bot/model/lm_call_result.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      361 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/domain/bot/model/lm_chat_message.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      379 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/domain/bot/model/lm_train_data.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.175934 bot_station-0.3.1/bot_station/domain/bot_station/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/domain/bot_station/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      692 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/domain/bot_station/bot_registry.py
--rw-r--r--   0 mmarashan (1826057312) 593637566     2715 2024-05-08 06:12:30.000000 bot_station-0.3.1/bot_station/domain/bot_station/bot_station.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.176288 bot_station-0.3.1/bot_station/domain/bot_station/model/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/domain/bot_station/model/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      279 2024-05-06 05:37:14.000000 bot_station-0.3.1/bot_station/domain/bot_station/model/bot_creation_config.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.177036 bot_station-0.3.1/bot_station.egg-info/
--rw-r--r--   0 mmarashan (1826057312) 593637566      707 2024-05-08 19:14:51.000000 bot_station-0.3.1/bot_station.egg-info/PKG-INFO
--rw-r--r--   0 mmarashan (1826057312) 593637566     2363 2024-05-08 19:14:51.000000 bot_station-0.3.1/bot_station.egg-info/SOURCES.txt
--rw-r--r--   0 mmarashan (1826057312) 593637566        1 2024-05-08 19:14:51.000000 bot_station-0.3.1/bot_station.egg-info/dependency_links.txt
--rw-r--r--   0 mmarashan (1826057312) 593637566      190 2024-05-08 19:14:51.000000 bot_station-0.3.1/bot_station.egg-info/requires.txt
--rw-r--r--   0 mmarashan (1826057312) 593637566       18 2024-05-08 19:14:51.000000 bot_station-0.3.1/bot_station.egg-info/top_level.txt
--rw-r--r--   0 mmarashan (1826057312) 593637566       38 2024-05-08 19:14:51.177567 bot_station-0.3.1/setup.cfg
--rw-r--r--   0 mmarashan (1826057312) 593637566      834 2024-05-08 19:12:16.000000 bot_station-0.3.1/setup.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.176810 bot_station-0.3.1/tests/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.3.1/tests/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566     4483 2024-05-08 05:55:27.000000 bot_station-0.3.1/tests/bot_station_api_test.py
--rw-r--r--   0 mmarashan (1826057312) 593637566     1051 2024-05-05 19:58:38.000000 bot_station-0.3.1/tests/test_bot_factory.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-10 20:07:13.432534 bot_station-0.4.0/
+-rw-r--r--   0 mmarashan (1826057312) 593637566     1070 2024-05-05 19:58:38.000000 bot_station-0.4.0/LICENSE
+-rw-r--r--   0 mmarashan (1826057312) 593637566      707 2024-05-10 20:07:13.432349 bot_station-0.4.0/PKG-INFO
+-rw-r--r--   0 mmarashan (1826057312) 593637566       17 2024-05-05 19:58:38.000000 bot_station-0.4.0/README.md
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-10 20:07:13.423982 bot_station-0.4.0/bot_station/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.4.0/bot_station/__init__.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-10 20:07:13.424779 bot_station-0.4.0/bot_station/api/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.4.0/bot_station/api/__init__.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-10 20:07:13.424968 bot_station-0.4.0/bot_station/api/rest/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.4.0/bot_station/api/rest/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566     6988 2024-05-08 19:40:03.000000 bot_station-0.4.0/bot_station/api/rest/api.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-10 20:07:13.426695 bot_station-0.4.0/bot_station/api/rest/model/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.4.0/bot_station/api/rest/model/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      257 2024-05-05 19:58:38.000000 bot_station-0.4.0/bot_station/api/rest/model/bot_call_dto.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      331 2024-05-05 19:58:38.000000 bot_station-0.4.0/bot_station/api/rest/model/bot_call_result.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      486 2024-05-08 19:40:03.000000 bot_station-0.4.0/bot_station/api/rest/model/bot_creation_dto.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      126 2024-05-05 19:58:38.000000 bot_station-0.4.0/bot_station/api/rest/model/bot_creation_result.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      433 2024-05-05 19:58:38.000000 bot_station-0.4.0/bot_station/api/rest/model/bot_dto.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      401 2024-05-08 19:40:03.000000 bot_station-0.4.0/bot_station/api/rest/model/bot_train_dto.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566       90 2024-05-05 19:58:38.000000 bot_station-0.4.0/bot_station/api/rest/model/bot_train_result.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      204 2024-05-05 19:58:38.000000 bot_station-0.4.0/bot_station/api/rest/model/web_app_config.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-10 20:07:13.426823 bot_station-0.4.0/bot_station/data/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.4.0/bot_station/data/__init__.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-10 20:07:13.426934 bot_station-0.4.0/bot_station/data/base/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.4.0/bot_station/data/base/__init__.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-10 20:07:13.427268 bot_station-0.4.0/bot_station/data/base/database/
+-rw-r--r--   0 mmarashan (1826057312) 593637566      975 2024-05-05 19:58:38.000000 bot_station-0.4.0/bot_station/data/base/database/UUID.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.4.0/bot_station/data/base/database/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      428 2024-05-05 19:58:38.000000 bot_station-0.4.0/bot_station/data/base/database/base_db_dto.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-10 20:07:13.427803 bot_station-0.4.0/bot_station/data/bot/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.4.0/bot_station/data/bot/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566     1298 2024-05-10 19:58:08.000000 bot_station-0.4.0/bot_station/data/bot/bot_factory_impl.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566     8294 2024-05-10 20:00:38.000000 bot_station-0.4.0/bot_station/data/bot/bot_impl.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566     2169 2024-05-05 19:58:38.000000 bot_station-0.4.0/bot_station/data/bot/chat_message_storage_impl.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-10 20:07:13.428066 bot_station-0.4.0/bot_station/data/bot/mapper/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.4.0/bot_station/data/bot/mapper/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      972 2024-05-08 19:40:03.000000 bot_station-0.4.0/bot_station/data/bot/mapper/document_mapper.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-10 20:07:13.428491 bot_station-0.4.0/bot_station/data/bot/model/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.4.0/bot_station/data/bot/model/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      124 2024-05-10 19:41:12.000000 bot_station-0.4.0/bot_station/data/bot/model/qdrant_config.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      128 2024-05-10 19:41:18.000000 bot_station-0.4.0/bot_station/data/bot/model/yandex_cloud_config.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-10 20:07:13.428728 bot_station-0.4.0/bot_station/data/bot_station/
+-rw-r--r--   0 mmarashan (1826057312) 593637566      508 2024-05-05 19:58:38.000000 bot_station-0.4.0/bot_station/data/bot_station/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566     3061 2024-05-08 19:40:03.000000 bot_station-0.4.0/bot_station/data/bot_station/bot_registry_impl.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-10 20:07:13.428951 bot_station-0.4.0/bot_station/data/bot_station/model/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.4.0/bot_station/data/bot_station/model/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      853 2024-05-08 19:40:03.000000 bot_station-0.4.0/bot_station/data/bot_station/model/bot_info_dto.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-10 20:07:13.429186 bot_station-0.4.0/bot_station/di/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.4.0/bot_station/di/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566     1529 2024-05-10 19:53:19.000000 bot_station-0.4.0/bot_station/di/bot_station_module.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-10 20:07:13.429310 bot_station-0.4.0/bot_station/domain/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.4.0/bot_station/domain/__init__.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-10 20:07:13.429608 bot_station-0.4.0/bot_station/domain/base/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.4.0/bot_station/domain/base/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      605 2024-05-10 20:00:38.000000 bot_station-0.4.0/bot_station/domain/base/const.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      391 2024-05-05 19:58:38.000000 bot_station-0.4.0/bot_station/domain/base/utils.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-10 20:07:13.430073 bot_station-0.4.0/bot_station/domain/bot/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.4.0/bot_station/domain/bot/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      673 2024-05-05 19:58:38.000000 bot_station-0.4.0/bot_station/domain/bot/bot.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      267 2024-05-05 19:58:38.000000 bot_station-0.4.0/bot_station/domain/bot/bot_factory.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      798 2024-05-05 19:58:38.000000 bot_station-0.4.0/bot_station/domain/bot/chat_message_storage.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-10 20:07:13.430945 bot_station-0.4.0/bot_station/domain/bot/model/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.4.0/bot_station/domain/bot/model/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      222 2024-05-08 19:40:03.000000 bot_station-0.4.0/bot_station/domain/bot/model/document.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      350 2024-05-05 19:58:38.000000 bot_station-0.4.0/bot_station/domain/bot/model/lm_bot_meta_info.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      254 2024-05-05 19:58:38.000000 bot_station-0.4.0/bot_station/domain/bot/model/lm_call_result.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      361 2024-05-05 19:58:38.000000 bot_station-0.4.0/bot_station/domain/bot/model/lm_chat_message.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      379 2024-05-05 19:58:38.000000 bot_station-0.4.0/bot_station/domain/bot/model/lm_train_data.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-10 20:07:13.431318 bot_station-0.4.0/bot_station/domain/bot_station/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.4.0/bot_station/domain/bot_station/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      692 2024-05-05 19:58:38.000000 bot_station-0.4.0/bot_station/domain/bot_station/bot_registry.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566     2715 2024-05-08 19:40:03.000000 bot_station-0.4.0/bot_station/domain/bot_station/bot_station.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-10 20:07:13.431552 bot_station-0.4.0/bot_station/domain/bot_station/model/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.4.0/bot_station/domain/bot_station/model/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      279 2024-05-08 19:40:03.000000 bot_station-0.4.0/bot_station/domain/bot_station/model/bot_creation_config.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-10 20:07:13.432114 bot_station-0.4.0/bot_station.egg-info/
+-rw-r--r--   0 mmarashan (1826057312) 593637566      707 2024-05-10 20:07:13.000000 bot_station-0.4.0/bot_station.egg-info/PKG-INFO
+-rw-r--r--   0 mmarashan (1826057312) 593637566     2407 2024-05-10 20:07:13.000000 bot_station-0.4.0/bot_station.egg-info/SOURCES.txt
+-rw-r--r--   0 mmarashan (1826057312) 593637566        1 2024-05-10 20:07:13.000000 bot_station-0.4.0/bot_station.egg-info/dependency_links.txt
+-rw-r--r--   0 mmarashan (1826057312) 593637566      190 2024-05-10 20:07:13.000000 bot_station-0.4.0/bot_station.egg-info/requires.txt
+-rw-r--r--   0 mmarashan (1826057312) 593637566       18 2024-05-10 20:07:13.000000 bot_station-0.4.0/bot_station.egg-info/top_level.txt
+-rw-r--r--   0 mmarashan (1826057312) 593637566       38 2024-05-10 20:07:13.432570 bot_station-0.4.0/setup.cfg
+-rw-r--r--   0 mmarashan (1826057312) 593637566      834 2024-05-08 19:40:03.000000 bot_station-0.4.0/setup.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-10 20:07:13.431887 bot_station-0.4.0/tests/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.4.0/tests/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566     4727 2024-05-10 19:52:45.000000 bot_station-0.4.0/tests/bot_station_api_test.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566     1051 2024-05-05 19:58:38.000000 bot_station-0.4.0/tests/test_bot_factory.py
```

### Comparing `bot_station-0.3.1/LICENSE` & `bot_station-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bot_station-0.3.1/PKG-INFO` & `bot_station-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: bot_station
-Version: 0.3.1
+Version: 0.4.0
 Summary: Bot Station SDK + Web App
 Author: Maxim Marashan
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.31.0
 Requires-Dist: langchain==0.1.17
 Requires-Dist: langchain-community==0.0.36
 Requires-Dist: qdrant-client==1.9.0
-Requires-Dist: fastembed==0.2.6
+Requires-Dist: fastembed==0.2.7
 Requires-Dist: yandexcloud==0.271.0
 Requires-Dist: tiktoken==0.6.0
 Requires-Dist: SQLAlchemy==2.0.29
 Requires-Dist: fastapi==0.110.3
 Requires-Dist: uvicorn==0.29.0
 
 # Bot Station SDK
```

### Comparing `bot_station-0.3.1/bot_station/api/rest/api.py` & `bot_station-0.4.0/bot_station/api/rest/api.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.3.1/bot_station/data/base/database/UUID.py` & `bot_station-0.4.0/bot_station/data/base/database/UUID.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.3.1/bot_station/data/bot/bot_factory_impl.py` & `bot_station-0.4.0/bot_station/data/bot/bot_factory_impl.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 import logging
 
 from bot_station.data.bot.bot_impl import BotImpl
 from bot_station.data.bot.chat_message_storage_impl import ChatMessageStorageImpl
+from bot_station.data.bot.model.qdrant_config import QdrantConfig
 from bot_station.data.bot.model.yandex_cloud_config import YandexCloudConfig
 from bot_station.domain.base.const import message_history_path
 from bot_station.domain.bot.bot import Bot
 from bot_station.domain.bot.bot_factory import BotFactory
 from bot_station.domain.bot.model.lm_bot_meta_info import LMBotMetaInfo
 
 
 class BotFactoryImpl(BotFactory):
-    config: YandexCloudConfig
+    yandex_cloud_config: YandexCloudConfig
+    qdrant_config: QdrantConfig
 
     def __init__(
             self,
-            config: YandexCloudConfig,
+            yandex_cloud_config: YandexCloudConfig,
+            qdrant_config: QdrantConfig,
     ):
-        self.config = config
+        self.yandex_cloud_config = yandex_cloud_config
+        self.qdrant_config = qdrant_config
 
     async def create(self, meta: LMBotMetaInfo) -> Bot:
         logging.debug(f"create new bot {meta}")
         bot = BotImpl(
             message_storage=ChatMessageStorageImpl(
                 root_message_history_path=message_history_path
             ),
-            config=self.config,
+            yandex_cloud_config=self.yandex_cloud_config,
+            qdrant_config=self.qdrant_config,
         )
         await bot.load(meta=meta)
         return bot
```

### Comparing `bot_station-0.3.1/bot_station/data/bot/bot_impl.py` & `bot_station-0.4.0/bot_station/data/bot/bot_impl.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 from langchain_core.documents import Document as LangchainDocument
 from langchain_core.embeddings import Embeddings
 from langchain_core.language_models import BaseChatModel
 from langchain_core.vectorstores import VectorStoreRetriever
 from qdrant_client import QdrantClient
 
 from bot_station.data.bot.mapper.document_mapper import DocumentMapper
+from bot_station.data.bot.model.qdrant_config import QdrantConfig
 from bot_station.data.bot.model.yandex_cloud_config import YandexCloudConfig
+from bot_station.domain.base.const import embeddings_cache_dir
 from bot_station.domain.bot.bot import Bot
 from bot_station.domain.bot.chat_message_storage import ChatMessageStorage
 from bot_station.domain.bot.model.document import Document
 from bot_station.domain.bot.model.lm_bot_meta_info import LMBotMetaInfo
 from bot_station.domain.bot.model.lm_call_result import CallResult
 from bot_station.domain.bot.model.lm_chat_message import LMBotMessage, LmChatMessage
 from bot_station.domain.bot.model.lm_chat_message import LMUserMessage
@@ -38,55 +40,58 @@
     embeddings: Embeddings = None
 
     knowledge_vector_store: Qdrant = None
     qdrant_cli: QdrantClient = None
     knowledge_retriever: VectorStoreRetriever = None
 
     gpt: BaseChatModel = None
-    config: YandexCloudConfig = None
+    yandex_cloud_config: YandexCloudConfig = None
+    qdrant_config: QdrantConfig = None
 
     message_storage: ChatMessageStorage = None
 
     meta: LMBotMetaInfo = None
 
     __is_loaded: bool = False
 
     save_doc_max_per_second_count = 10
     doc_splitter_chunk_size = 2000
     doc_splitter_chunk_overlap = 30
 
     def __init__(
             self,
             message_storage: ChatMessageStorage,
-            config: YandexCloudConfig,
+            yandex_cloud_config: YandexCloudConfig,
+            qdrant_config: QdrantConfig,
     ):
         self.message_storage = message_storage
-        self.config = config
+        self.yandex_cloud_config = yandex_cloud_config
+        self.qdrant_config = qdrant_config
 
     async def load(self, meta: LMBotMetaInfo):
         if self.__is_loaded:
             return
         logging.debug(f"load(meta = {meta})")
 
         langchain.debug = True
 
-        self.embeddings: Embeddings = FastEmbedEmbeddings()
+        self.embeddings: Embeddings = FastEmbedEmbeddings(cache_dir=embeddings_cache_dir)
         self.gpt = ChatYandexGPT(
-            api_key=self.config.api_key,
-            folder_id=self.config.folder_id,
+            api_key=self.yandex_cloud_config.api_key,
+            folder_id=self.yandex_cloud_config.folder_id,
             temperature=meta.temperature,
-            model_name=self.config.model_name,
+            model_name=self.yandex_cloud_config.model_name,
             verbose=True,
         )
         self.meta = meta
 
-        if self.config.qdrant_url is not None:
-            self.qdrant_cli = QdrantClient(url=self.config.qdrant_url)
-        elif self.config.qdrant_db_path is not None:
-            self.qdrant_cli = QdrantClient(path=self.config.qdrant_db_path)
+        if self.qdrant_config.qdrant_url is not None:
+            self.qdrant_cli = QdrantClient(url=self.qdrant_config.qdrant_url)
+        elif self.qdrant_config.qdrant_db_path is not None:
+            self.qdrant_cli = QdrantClient(path=self.qdrant_config.qdrant_db_path)
         else:
             raise AssertionError("qdrant_uri or qdrant_db_path not set")
 
         self._prepare_vectorstore()
         self.__is_loaded = True
 
     async def train(self, data: TrainData):
```

### Comparing `bot_station-0.3.1/bot_station/data/bot/chat_message_storage_impl.py` & `bot_station-0.4.0/bot_station/data/bot/chat_message_storage_impl.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.3.1/bot_station/data/bot/mapper/document_mapper.py` & `bot_station-0.4.0/bot_station/data/bot/mapper/document_mapper.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.3.1/bot_station/data/bot_station/bot_registry_impl.py` & `bot_station-0.4.0/bot_station/data/bot_station/bot_registry_impl.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.3.1/bot_station/data/bot_station/model/bot_info_dto.py` & `bot_station-0.4.0/bot_station/data/bot_station/model/bot_info_dto.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.3.1/bot_station/di/bot_station_module.py` & `bot_station-0.4.0/bot_station/di/bot_station_module.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from bot_station.data.bot.bot_factory_impl import BotFactoryImpl
+from bot_station.data.bot.model.qdrant_config import QdrantConfig
 from bot_station.data.bot.model.yandex_cloud_config import YandexCloudConfig
 from bot_station.data.bot_station.bot_registry_impl import BotRegistryImpl
 from bot_station.domain.bot.bot_factory import BotFactory
 from bot_station.domain.bot_station.bot_registry import BotRegistry
 from bot_station.domain.bot_station.bot_station import BotStation, BotStationImpl
 
 
@@ -10,21 +11,27 @@
     overrides_bot_factory: BotFactory | None = None
 
     @staticmethod
     def provide_bot_factory(bot_factory: BotFactory):
         BotStationModule.overrides_bot_factory = bot_factory
 
     @staticmethod
-    def create_bot_station(env_config: YandexCloudConfig) -> BotStation:
+    def create_bot_station(
+            yandex_cloud_config: YandexCloudConfig,
+            qdrant_config: QdrantConfig,
+    ) -> BotStation:
         bot_registry: BotRegistry = BotRegistryImpl()
         bot_station: BotStation = BotStationImpl(
             bot_registry=bot_registry,
-            bot_factory=BotStationModule.__get_bot_factory(env_config),
+            bot_factory=BotStationModule.__get_bot_factory(yandex_cloud_config, qdrant_config),
         )
         return bot_station
 
     @staticmethod
-    def __get_bot_factory(env_config: YandexCloudConfig) -> BotFactory:
+    def __get_bot_factory(
+            env_config: YandexCloudConfig,
+            qdrant_config: QdrantConfig,
+    ) -> BotFactory:
         if BotStationModule.overrides_bot_factory is not None:
             return BotStationModule.overrides_bot_factory
         else:
-            return BotFactoryImpl(config=env_config)
+            return BotFactoryImpl(yandex_cloud_config=env_config, qdrant_config=qdrant_config)
```

### Comparing `bot_station-0.3.1/bot_station/domain/base/const.py` & `bot_station-0.4.0/bot_station/domain/base/const.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,7 +3,8 @@
             """
 
 # TODO: обернуть это и пути в ConfigProvider и передавать через конструктор
 data_folder_path = "./.data"
 databases_path = data_folder_path + "/database"
 message_history_path = data_folder_path + "/message_history"
 chat_files_path = data_folder_path + "/chat_files"
+embeddings_cache_dir = data_folder_path + "/embedings_cache"
```

### Comparing `bot_station-0.3.1/bot_station/domain/bot/bot.py` & `bot_station-0.4.0/bot_station/domain/bot/bot.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.3.1/bot_station/domain/bot/chat_message_storage.py` & `bot_station-0.4.0/bot_station/domain/bot/chat_message_storage.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.3.1/bot_station/domain/bot_station/bot_registry.py` & `bot_station-0.4.0/bot_station/domain/bot_station/bot_registry.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.3.1/bot_station/domain/bot_station/bot_station.py` & `bot_station-0.4.0/bot_station/domain/bot_station/bot_station.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.3.1/bot_station.egg-info/PKG-INFO` & `bot_station-0.4.0/bot_station.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: bot_station
-Version: 0.3.1
+Version: 0.4.0
 Summary: Bot Station SDK + Web App
 Author: Maxim Marashan
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.31.0
 Requires-Dist: langchain==0.1.17
 Requires-Dist: langchain-community==0.0.36
 Requires-Dist: qdrant-client==1.9.0
-Requires-Dist: fastembed==0.2.6
+Requires-Dist: fastembed==0.2.7
 Requires-Dist: yandexcloud==0.271.0
 Requires-Dist: tiktoken==0.6.0
 Requires-Dist: SQLAlchemy==2.0.29
 Requires-Dist: fastapi==0.110.3
 Requires-Dist: uvicorn==0.29.0
 
 # Bot Station SDK
```

### Comparing `bot_station-0.3.1/bot_station.egg-info/SOURCES.txt` & `bot_station-0.4.0/bot_station.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 bot_station/data/bot/__init__.py
 bot_station/data/bot/bot_factory_impl.py
 bot_station/data/bot/bot_impl.py
 bot_station/data/bot/chat_message_storage_impl.py
 bot_station/data/bot/mapper/__init__.py
 bot_station/data/bot/mapper/document_mapper.py
 bot_station/data/bot/model/__init__.py
+bot_station/data/bot/model/qdrant_config.py
 bot_station/data/bot/model/yandex_cloud_config.py
 bot_station/data/bot_station/__init__.py
 bot_station/data/bot_station/bot_registry_impl.py
 bot_station/data/bot_station/model/__init__.py
 bot_station/data/bot_station/model/bot_info_dto.py
 bot_station/di/__init__.py
 bot_station/di/bot_station_module.py
```

### Comparing `bot_station-0.3.1/setup.py` & `bot_station-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.3.1/tests/bot_station_api_test.py` & `bot_station-0.4.0/tests/bot_station_api_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 import logging
 import unittest
 
 from fastapi.testclient import TestClient
 
 from bot_station.api.rest.api import BotStationWebApp
 from bot_station.api.rest.model.web_app_config import WebAppConfig
+from bot_station.data.bot.model.qdrant_config import QdrantConfig
 from bot_station.data.bot.model.yandex_cloud_config import YandexCloudConfig
 from bot_station.di.bot_station_module import BotStationModule
 from bot_station.domain.bot.bot import Bot
 from bot_station.domain.bot_station.bot_station import BotStation
 from test_bot_factory import TestBotFactory, TestBot
 
 
 def launch_test_web_app(bot: Bot):
-    env_config = YandexCloudConfig(
+    yandex_cloud_config = YandexCloudConfig(
         api_key="",
         folder_id="",
         model_name="",
+    )
+    qdrant_config = QdrantConfig(
         qdrant_url="",
         qdrant_db_path=None,
     )
     bot_factory = TestBotFactory()
     bot_factory.set_bot(bot)
     BotStationModule.provide_bot_factory(bot_factory)
-    test_bot_station: BotStation = BotStationModule.create_bot_station(env_config)
+    test_bot_station: BotStation = BotStationModule.create_bot_station(yandex_cloud_config=yandex_cloud_config,
+                                                                       qdrant_config=qdrant_config)
 
     BotStationWebApp.prepare(bot_station=test_bot_station, config=WebAppConfig())
 
 
 class BotStationApiTest(unittest.TestCase):
     mock_bot = TestBot()
     bot_station_test_client: TestClient
```

### Comparing `bot_station-0.3.1/tests/test_bot_factory.py` & `bot_station-0.4.0/tests/test_bot_factory.py`

 * *Files identical despite different names*

