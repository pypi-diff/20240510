# Comparing `tmp/nonebot_plugin_tetris_stats-1.1.1.tar.gz` & `tmp/nonebot_plugin_tetris_stats-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_tetris_stats-1.1.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_tetris_stats-1.1.2.tar", max compression
```

## Comparing `nonebot_plugin_tetris_stats-1.1.1.tar` & `nonebot_plugin_tetris_stats-1.1.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0    34523 2024-05-10 03:30:47.362498 nonebot_plugin_tetris_stats-1.1.1/LICENSE
--rw-r--r--   0        0        0     2242 2024-05-10 03:30:47.362498 nonebot_plugin_tetris_stats-1.1.1/README.md
--rw-r--r--   0        0        0      719 2024-05-10 03:30:47.362498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/__init__.py
--rw-r--r--   0        0        0      331 2024-05-10 03:30:47.362498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/config/config.py
--rw-r--r--   0        0        0     1674 2024-05-10 03:30:47.362498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/config/migrations/09d4bb60160d_rename_field.py
--rw-r--r--   0        0        0     1311 2024-05-10 03:30:47.362498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/config/migrations/0d50142b780f_add_field.py
--rw-r--r--   0        0        0     1995 2024-05-10 03:30:47.362498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/config/migrations/6c3206f90cc3_add_field.py
--rw-r--r--   0        0        0     2985 2024-05-10 03:30:47.362498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/config/migrations/8a91210ce14d_correct_the_data_in_historicaldata.py
--rw-r--r--   0        0        0     6222 2024-05-10 03:30:47.362498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/config/migrations/9866f53ce44f_init_db.py
--rw-r--r--   0        0        0     3262 2024-05-10 03:30:47.362498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/config/migrations/9cd1647db502_merge_old_db.py
--rw-r--r--   0        0        0     5483 2024-05-10 03:30:47.362498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/config/migrations/9f6582279ce2_recreate_historical_data.py
--rw-r--r--   0        0        0        0 2024-05-10 03:30:47.362498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/config/migrations/__init__.py
--rw-r--r--   0        0        0     3911 2024-05-10 03:30:47.362498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/config/migrations/b7fbdafc339a_add_user_unique_identifier_field_to_.py
--rw-r--r--   0        0        0      948 2024-05-10 03:30:47.362498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/config/migrations/b9d65badc713_del_old_tos_bind_data.py
--rw-r--r--   0        0        0     1407 2024-05-10 03:30:47.362498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/db/__init__.py
--rw-r--r--   0        0        0     3417 2024-05-10 03:30:47.362498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/db/models.py
--rw-r--r--   0        0        0     3167 2024-05-10 03:30:47.362498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/game_data_processor/__init__.py
--rw-r--r--   0        0        0      108 2024-05-10 03:30:47.362498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/game_data_processor/constant.py
--rw-r--r--   0        0        0     7346 2024-05-10 03:30:47.362498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/__init__.py
--rw-r--r--   0        0        0     1045 2024-05-10 03:30:47.362498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/cache.py
--rw-r--r--   0        0        0      422 2024-05-10 03:30:47.362498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/constant.py
--rw-r--r--   0        0        0     1148 2024-05-10 03:30:47.362498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/model.py
--rw-r--r--   0        0        0    20640 2024-05-10 03:30:47.362498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/processor.py
--rw-r--r--   0        0        0      334 2024-05-10 03:30:47.362498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/base.py
--rw-r--r--   0        0        0     1483 2024-05-10 03:30:47.362498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/league_all.py
--rw-r--r--   0        0        0      590 2024-05-10 03:30:47.362498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/response.py
--rw-r--r--   0        0        0      368 2024-05-10 03:30:47.362498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/user.py
--rw-r--r--   0        0        0     4264 2024-05-10 03:30:47.362498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/user_info.py
--rw-r--r--   0        0        0     2538 2024-05-10 03:30:47.362498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/user_records.py
--rw-r--r--   0        0        0      231 2024-05-10 03:30:47.362498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/typing.py
--rw-r--r--   0        0        0      625 2024-05-10 03:30:47.366498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/game_data_processor/schemas.py
--rw-r--r--   0        0        0     4195 2024-05-10 03:30:47.366498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/__init__.py
--rw-r--r--   0        0        0      103 2024-05-10 03:30:47.366498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/constant.py
--rw-r--r--   0        0        0     6313 2024-05-10 03:30:47.366498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/processor.py
--rw-r--r--   0        0        0      357 2024-05-10 03:30:47.366498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/schemas/response.py
--rw-r--r--   0        0        0     6412 2024-05-10 03:30:47.366498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/__init__.py
--rw-r--r--   0        0        0      293 2024-05-10 03:30:47.366498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/constant.py
--rw-r--r--   0        0        0    10066 2024-05-10 03:30:47.366498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/processor.py
--rw-r--r--   0        0        0      524 2024-05-10 03:30:47.366498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/schemas/response.py
--rw-r--r--   0        0        0     3847 2024-05-10 03:30:47.366498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/schemas/user_info.py
--rw-r--r--   0        0        0      690 2024-05-10 03:30:47.366498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/schemas/user_profile.py
--rw-r--r--   0        0        0     1725 2024-05-10 03:30:47.366498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/utils/avatar.py
--rw-r--r--   0        0        0     2996 2024-05-10 03:30:47.366498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/utils/browser.py
--rw-r--r--   0        0        0      945 2024-05-10 03:30:47.366498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/utils/exception.py
--rw-r--r--   0        0        0     2045 2024-05-10 03:30:47.366498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/utils/host.py
--rw-r--r--   0        0        0     8031 2024-05-10 03:30:47.366498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/utils/metrics.py
--rw-r--r--   0        0        0      440 2024-05-10 03:30:47.366498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/utils/platform.py
--rw-r--r--   0        0        0     3064 2024-05-10 03:30:47.366498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/utils/recorder.py
--rw-r--r--   0        0        0     2703 2024-05-10 03:30:47.366498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/utils/render.py
--rw-r--r--   0        0        0     6222 2024-05-10 03:30:47.366498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/utils/request.py
--rw-r--r--   0        0        0     1390 2024-05-10 03:30:47.366498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/utils/retry.py
--rw-r--r--   0        0        0      394 2024-05-10 03:30:47.366498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/utils/screenshot.py
--rw-r--r--   0        0        0     2308 2024-05-10 03:30:47.366498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/utils/templates.py
--rw-r--r--   0        0        0      922 2024-05-10 03:30:47.366498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/utils/typing.py
--rw-r--r--   0        0        0       93 2024-05-10 03:30:47.366498 nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/version.py
--rw-r--r--   0        0        0     3054 2024-05-10 03:30:47.366498 nonebot_plugin_tetris_stats-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     3738 1970-01-01 00:00:00.000000 nonebot_plugin_tetris_stats-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-10 03:49:43.782285 nonebot_plugin_tetris_stats-1.1.2/LICENSE
+-rw-r--r--   0        0        0     2242 2024-05-10 03:49:43.782285 nonebot_plugin_tetris_stats-1.1.2/README.md
+-rw-r--r--   0        0        0      719 2024-05-10 03:49:43.782285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/__init__.py
+-rw-r--r--   0        0        0      331 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/config/config.py
+-rw-r--r--   0        0        0     1674 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/config/migrations/09d4bb60160d_rename_field.py
+-rw-r--r--   0        0        0     1311 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/config/migrations/0d50142b780f_add_field.py
+-rw-r--r--   0        0        0     1995 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/config/migrations/6c3206f90cc3_add_field.py
+-rw-r--r--   0        0        0     2985 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/config/migrations/8a91210ce14d_correct_the_data_in_historicaldata.py
+-rw-r--r--   0        0        0     6222 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/config/migrations/9866f53ce44f_init_db.py
+-rw-r--r--   0        0        0     3262 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/config/migrations/9cd1647db502_merge_old_db.py
+-rw-r--r--   0        0        0     5483 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/config/migrations/9f6582279ce2_recreate_historical_data.py
+-rw-r--r--   0        0        0        0 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/config/migrations/__init__.py
+-rw-r--r--   0        0        0     3911 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/config/migrations/b7fbdafc339a_add_user_unique_identifier_field_to_.py
+-rw-r--r--   0        0        0      948 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/config/migrations/b9d65badc713_del_old_tos_bind_data.py
+-rw-r--r--   0        0        0     1407 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/db/__init__.py
+-rw-r--r--   0        0        0     3417 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/db/models.py
+-rw-r--r--   0        0        0     3167 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/game_data_processor/__init__.py
+-rw-r--r--   0        0        0      108 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/game_data_processor/constant.py
+-rw-r--r--   0        0        0     7346 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/__init__.py
+-rw-r--r--   0        0        0     1045 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/cache.py
+-rw-r--r--   0        0        0      422 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/constant.py
+-rw-r--r--   0        0        0     1148 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/model.py
+-rw-r--r--   0        0        0    20994 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/processor.py
+-rw-r--r--   0        0        0      334 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/base.py
+-rw-r--r--   0        0        0     1483 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/league_all.py
+-rw-r--r--   0        0        0      590 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/response.py
+-rw-r--r--   0        0        0      368 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/user.py
+-rw-r--r--   0        0        0     4264 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/user_info.py
+-rw-r--r--   0        0        0     2538 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/user_records.py
+-rw-r--r--   0        0        0      231 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/typing.py
+-rw-r--r--   0        0        0      625 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/game_data_processor/schemas.py
+-rw-r--r--   0        0        0     4195 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/__init__.py
+-rw-r--r--   0        0        0      103 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/constant.py
+-rw-r--r--   0        0        0     6313 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/processor.py
+-rw-r--r--   0        0        0      357 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/schemas/response.py
+-rw-r--r--   0        0        0     6412 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/__init__.py
+-rw-r--r--   0        0        0      293 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/constant.py
+-rw-r--r--   0        0        0    10066 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/processor.py
+-rw-r--r--   0        0        0      524 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/schemas/response.py
+-rw-r--r--   0        0        0     3847 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/schemas/user_info.py
+-rw-r--r--   0        0        0      690 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/schemas/user_profile.py
+-rw-r--r--   0        0        0     1725 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/utils/avatar.py
+-rw-r--r--   0        0        0     2996 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/utils/browser.py
+-rw-r--r--   0        0        0      945 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/utils/exception.py
+-rw-r--r--   0        0        0     2045 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/utils/host.py
+-rw-r--r--   0        0        0     8031 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/utils/metrics.py
+-rw-r--r--   0        0        0      440 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/utils/platform.py
+-rw-r--r--   0        0        0     3064 2024-05-10 03:49:43.786285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/utils/recorder.py
+-rw-r--r--   0        0        0     2703 2024-05-10 03:49:43.790285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/utils/render.py
+-rw-r--r--   0        0        0     6222 2024-05-10 03:49:43.790285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/utils/request.py
+-rw-r--r--   0        0        0     1390 2024-05-10 03:49:43.790285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/utils/retry.py
+-rw-r--r--   0        0        0      394 2024-05-10 03:49:43.790285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/utils/screenshot.py
+-rw-r--r--   0        0        0     2308 2024-05-10 03:49:43.790285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/utils/templates.py
+-rw-r--r--   0        0        0      922 2024-05-10 03:49:43.790285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/utils/typing.py
+-rw-r--r--   0        0        0       93 2024-05-10 03:49:43.790285 nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/version.py
+-rw-r--r--   0        0        0     3054 2024-05-10 03:49:43.790285 nonebot_plugin_tetris_stats-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3738 1970-01-01 00:00:00.000000 nonebot_plugin_tetris_stats-1.1.2/PKG-INFO
```

### Comparing `nonebot_plugin_tetris_stats-1.1.1/LICENSE` & `nonebot_plugin_tetris_stats-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.1/README.md` & `nonebot_plugin_tetris_stats-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/__init__.py` & `nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/config/migrations/09d4bb60160d_rename_field.py` & `nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/config/migrations/09d4bb60160d_rename_field.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/config/migrations/0d50142b780f_add_field.py` & `nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/config/migrations/0d50142b780f_add_field.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/config/migrations/6c3206f90cc3_add_field.py` & `nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/config/migrations/6c3206f90cc3_add_field.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/config/migrations/8a91210ce14d_correct_the_data_in_historicaldata.py` & `nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/config/migrations/8a91210ce14d_correct_the_data_in_historicaldata.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/config/migrations/9866f53ce44f_init_db.py` & `nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/config/migrations/9866f53ce44f_init_db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/config/migrations/9cd1647db502_merge_old_db.py` & `nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/config/migrations/9cd1647db502_merge_old_db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/config/migrations/9f6582279ce2_recreate_historical_data.py` & `nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/config/migrations/9f6582279ce2_recreate_historical_data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/config/migrations/b7fbdafc339a_add_user_unique_identifier_field_to_.py` & `nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/config/migrations/b7fbdafc339a_add_user_unique_identifier_field_to_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/config/migrations/b9d65badc713_del_old_tos_bind_data.py` & `nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/config/migrations/b9d65badc713_del_old_tos_bind_data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/db/__init__.py` & `nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/db/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/db/models.py` & `nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/db/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/game_data_processor/__init__.py` & `nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/game_data_processor/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/__init__.py` & `nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/cache.py` & `nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/model.py` & `nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/processor.py` & `nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,15 +237,21 @@
                         .where(HistoricalData.id < min([i.id for i in historical_data]))
                         .limit(1)
                     )
                 ).one_or_none()
                 if extra is not None:
                     historical_data = list(historical_data)
                     historical_data.append(extra)
-
+        if not historical_data:
+            return [
+                TETRIOInfo.TetraLeagueHistory.Data(record_at=today - forward, tr=user_info.data.user.league.rating),
+                TETRIOInfo.TetraLeagueHistory.Data(
+                    record_at=today.replace(microsecond=1000), tr=user_info.data.user.league.rating
+                ),
+            ]
         histories = [
             TETRIOInfo.TetraLeagueHistory.Data(
                 record_at=i.processed_data.user_info.cache.cached_at.astimezone(ZoneInfo('Asia/Shanghai')),
                 tr=i.processed_data.user_info.data.user.league.rating,
             )
             for i in historical_data
             if isinstance(i.processed_data, ProcessedData)
```

### Comparing `nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/league_all.py` & `nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/league_all.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/response.py` & `nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/response.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/user_info.py` & `nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/user_info.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/user_records.py` & `nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/user_records.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/game_data_processor/schemas.py` & `nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/game_data_processor/schemas.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/__init__.py` & `nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/processor.py` & `nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/processor.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/__init__.py` & `nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/processor.py` & `nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/processor.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/schemas/response.py` & `nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/schemas/response.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/schemas/user_info.py` & `nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/schemas/user_info.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/schemas/user_profile.py` & `nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/schemas/user_profile.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/utils/avatar.py` & `nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/utils/avatar.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/utils/browser.py` & `nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/utils/browser.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/utils/exception.py` & `nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/utils/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/utils/host.py` & `nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/utils/host.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/utils/metrics.py` & `nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/utils/recorder.py` & `nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/utils/recorder.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/utils/render.py` & `nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/utils/render.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/utils/request.py` & `nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/utils/request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/utils/retry.py` & `nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/utils/retry.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/utils/templates.py` & `nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/utils/templates.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.1/nonebot_plugin_tetris_stats/utils/typing.py` & `nonebot_plugin_tetris_stats-1.1.2/nonebot_plugin_tetris_stats/utils/typing.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.1.1/pyproject.toml` & `nonebot_plugin_tetris_stats-1.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'nonebot-plugin-tetris-stats'
-version = '1.1.1'
+version = '1.1.2'
 description = '一款基于 NoneBot2 的用于查询 Tetris 相关游戏数据的插件'
 authors = ['scdhh <wallfjjd@gmail.com>']
 readme = 'README.md'
 homepage = 'https://github.com/shoucandanghehe/nonebot-plugin-tetris-stats'
 repository = 'https://github.com/shoucandanghehe/nonebot-plugin-tetris-stats'
 license = 'AGPL-3.0'
```

### Comparing `nonebot_plugin_tetris_stats-1.1.1/PKG-INFO` & `nonebot_plugin_tetris_stats-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-tetris-stats
-Version: 1.1.1
+Version: 1.1.2
 Summary: 一款基于 NoneBot2 的用于查询 Tetris 相关游戏数据的插件
 Home-page: https://github.com/shoucandanghehe/nonebot-plugin-tetris-stats
 License: AGPL-3.0
 Author: scdhh
 Author-email: wallfjjd@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-tetris-stats Version: 1.1.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-tetris-stats Version: 1.1.2 Summary:
 ä¸æ¬¾åºäº NoneBot2 çç¨äºæ¥è¯¢ Tetris ç¸å³æ¸¸ææ°æ®çæä»¶ Home-
 page: https://github.com/shoucandanghehe/nonebot-plugin-tetris-stats License:
 AGPL-3.0 Author: scdhh Author-email: wallfjjd@gmail.com Requires-Python:
 >=3.10,<4.0 Classifier: License :: OSI Approved :: GNU Affero General Public
 License v3 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
```

