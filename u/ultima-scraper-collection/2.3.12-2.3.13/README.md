# Comparing `tmp/ultima_scraper_collection-2.3.12.tar.gz` & `tmp/ultima_scraper_collection-2.3.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultima_scraper_collection-2.3.12.tar", max compression
+gzip compressed data, was "ultima_scraper_collection-2.3.13.tar", max compression
```

## Comparing `ultima_scraper_collection-2.3.12.tar` & `ultima_scraper_collection-2.3.13.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0      925 2024-05-03 05:40:32.991512 ultima_scraper_collection-2.3.12/pyproject.toml
--rw-r--r--   0        0        0      293 2023-09-08 23:34:07.011359 ultima_scraper_collection-2.3.12/ultima_scraper_collection/__init__.py
--rw-r--r--   0        0        0     3785 2023-11-30 08:43:28.338336 ultima_scraper_collection-2.3.12/ultima_scraper_collection/config.py
--rw-r--r--   0        0        0        0 2023-07-12 11:29:22.237223 ultima_scraper_collection-2.3.12/ultima_scraper_collection/helpers/__init__.py
--rw-r--r--   0        0        0     3899 2024-04-19 12:56:15.595721 ultima_scraper_collection-2.3.12/ultima_scraper_collection/helpers/main_helper.py
--rw-r--r--   0        0        0        0 2023-02-26 11:42:41.007744 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/__init__.py
--rw-r--r--   0        0        0     2265 2024-01-06 09:20:24.925735 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/content_manager.py
--rw-r--r--   0        0        0        0 2023-02-26 11:42:54.441267 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/__init__.py
--rw-r--r--   0        0        0        0 2023-03-06 01:27:30.462039 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/__init__.py
--rw-r--r--   0        0        0        0 2023-03-04 04:03:12.661102 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/__init__.py
--rw-r--r--   0        0        0        0 2023-02-26 11:42:54.461267 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/__init__.py
--rw-r--r--   0        0        0       38 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/README
--rw-r--r--   0        0        0     2150 2023-03-05 04:16:43.534861 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/env.py
--rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/script.py.mako
--rw-r--r--   0        0        0      662 2023-03-05 04:20:42.303797 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/0d4d92c0498e_content.py
--rw-r--r--   0        0        0      941 2023-03-05 04:20:47.520466 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/1454e4d1c6b8_content.py
--rw-r--r--   0        0        0      861 2022-04-25 23:29:43.807242 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/37c4f2719d65_content.py
--rw-r--r--   0        0        0     3182 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/5493253cc03c_content.py
--rw-r--r--   0        0        0     1651 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/b791cf213df9_content.py
--rw-r--r--   0        0        0     1415 2023-03-05 04:20:57.727140 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/d2f2002f3c36_content.py
--rw-r--r--   0        0        0     2201 2023-03-03 17:13:51.407142 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic.ini
--rw-r--r--   0        0        0    77824 2023-02-14 03:46:10.695467 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/base_user_database.db
--rw-r--r--   0        0        0        0 2023-03-10 12:28:15.033139 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/__init__.py
--rw-r--r--   0        0        0        0 2023-03-10 12:28:22.753355 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/__init__.py
--rw-r--r--   0        0        0        0 2023-03-10 12:27:11.408006 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/__init__.py
--rw-r--r--   0        0        0     2296 2023-03-10 12:28:05.882882 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/env.py
--rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/script.py.mako
--rw-r--r--   0        0        0     1769 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/2c36fcc0b921_content.py
--rw-r--r--   0        0        0     1649 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/7c1c6e101059_content.py
--rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/aeb9fe314556_content.py
--rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/bf20242a238f_content.py
--rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/d0118d8ec0b4_content.py
--rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic.ini
--rw-r--r--   0        0        0      493 2023-03-10 12:30:45.700616 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/messages.py
--rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/test_messages.db
--rw-r--r--   0        0        0     2288 2023-03-10 12:32:59.654189 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/env.py
--rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/script.py.mako
--rw-r--r--   0        0        0     1762 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/194e05269f09_content.py
--rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/5b4bea08c27f_content.py
--rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/6b1b10eb67de_content.py
--rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/990fc1108317_content.py
--rw-r--r--   0        0        0     1643 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/a918b6b05d2f_content.py
--rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic.ini
--rw-r--r--   0        0        0      488 2023-03-10 12:32:58.467491 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/posts.py
--rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/test_posts.db
--rw-r--r--   0        0        0     2294 2023-03-10 12:32:46.997189 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/env.py
--rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/script.py.mako
--rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/29f675c35eee_content.py
--rw-r--r--   0        0        0     1647 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/2e4f8364f7e2_content.py
--rw-r--r--   0        0        0     1766 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/3076beb33c1b_content.py
--rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/e0c73f066547_content.py
--rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/ebc3f4bb0782_content.py
--rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic.ini
--rw-r--r--   0        0        0      490 2023-03-10 12:32:57.520800 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/stories.py
--rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/test_stories.db
--rw-r--r--   0        0        0        0 2022-12-05 14:27:20.696663 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/__init__.py
--rw-r--r--   0        0        0     1611 2023-06-03 17:34:00.273754 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/api_model.py
--rw-r--r--   0        0        0     2764 2023-05-08 21:50:28.707049 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/media_model.py
--rw-r--r--   0        0        0     2073 2023-04-20 22:22:10.068827 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/user_database.py
--rw-r--r--   0        0        0    10292 2023-07-18 00:51:38.377898 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/sqlite_database.py
--rw-r--r--   0        0        0      442 2023-03-12 15:01:42.766490 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/database_manager.py
--rw-r--r--   0        0        0        0 2023-02-26 16:06:18.482305 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/datascraper_manager/__init__.py
--rw-r--r--   0        0        0     2306 2023-12-02 00:03:22.382921 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/datascraper_manager/datascraper_manager.py
--rw-r--r--   0        0        0        0 2023-02-26 16:04:46.426896 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/datascraper_manager/datascrapers/__init__.py
--rw-r--r--   0        0        0     5349 2023-07-13 02:40:41.499162 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/datascraper_manager/datascrapers/fansly.py
--rw-r--r--   0        0        0     7775 2024-04-19 16:09:08.875404 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/datascraper_manager/datascrapers/onlyfans.py
--rw-r--r--   0        0        0    12574 2024-04-19 16:12:18.369164 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/download_manager.py
--rw-r--r--   0        0        0    27537 2024-04-24 15:09:00.096812 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/filesystem_manager.py
--rw-r--r--   0        0        0        0 2023-01-26 08:21:03.864558 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/metadata_manager/__init__.py
--rw-r--r--   0        0        0    35493 2024-04-25 14:10:09.139536 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/metadata_manager/metadata_manager.py
--rw-r--r--   0        0        0     7120 2023-11-30 21:46:23.292998 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/option_manager.py
--rw-r--r--   0        0        0     4126 2023-12-14 12:20:50.835331 ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/server_manager.py
--rw-r--r--   0        0        0        0 2023-03-14 06:55:35.872202 ultima_scraper_collection-2.3.12/ultima_scraper_collection/modules/__init__.py
--rw-r--r--   0        0        0    23537 2024-04-19 15:22:34.174028 ultima_scraper_collection-2.3.12/ultima_scraper_collection/modules/module_streamliner.py
--rw-r--r--   0        0        0        0 2023-08-06 03:54:32.746530 ultima_scraper_collection-2.3.12/ultima_scraper_collection/projects/__init__.py
--rw-r--r--   0        0        0     1954 2023-10-25 18:13:55.913824 ultima_scraper_collection-2.3.12/ultima_scraper_collection/projects/project_manager.py
--rw-r--r--   0        0        0     1006 2023-12-30 17:37:44.717342 ultima_scraper_collection-2.3.12/ultima_scraper_collection/projects/ultima_archive.py
--rw-r--r--   0        0        0        0 2023-02-26 16:07:35.717380 ultima_scraper_collection-2.3.12/ultima_scraper_collection/py.typed
--rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 ultima_scraper_collection-2.3.12/PKG-INFO
+-rw-r--r--   0        0        0      925 2024-05-10 06:59:53.787266 ultima_scraper_collection-2.3.13/pyproject.toml
+-rw-r--r--   0        0        0      293 2023-09-08 23:34:07.011359 ultima_scraper_collection-2.3.13/ultima_scraper_collection/__init__.py
+-rw-r--r--   0        0        0     3835 2024-05-03 05:56:52.883663 ultima_scraper_collection-2.3.13/ultima_scraper_collection/config.py
+-rw-r--r--   0        0        0        0 2023-07-12 11:29:22.237223 ultima_scraper_collection-2.3.13/ultima_scraper_collection/helpers/__init__.py
+-rw-r--r--   0        0        0     3899 2024-04-19 12:56:15.595721 ultima_scraper_collection-2.3.13/ultima_scraper_collection/helpers/main_helper.py
+-rw-r--r--   0        0        0        0 2023-02-26 11:42:41.007744 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/__init__.py
+-rw-r--r--   0        0        0     2265 2024-01-06 09:20:24.925735 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/content_manager.py
+-rw-r--r--   0        0        0        0 2023-02-26 11:42:54.441267 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-06 01:27:30.462039 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-04 04:03:12.661102 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-26 11:42:54.461267 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/__init__.py
+-rw-r--r--   0        0        0       38 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/README
+-rw-r--r--   0        0        0     2150 2023-03-05 04:16:43.534861 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/env.py
+-rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/script.py.mako
+-rw-r--r--   0        0        0      662 2023-03-05 04:20:42.303797 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/0d4d92c0498e_content.py
+-rw-r--r--   0        0        0      941 2023-03-05 04:20:47.520466 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/1454e4d1c6b8_content.py
+-rw-r--r--   0        0        0      861 2022-04-25 23:29:43.807242 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/37c4f2719d65_content.py
+-rw-r--r--   0        0        0     3182 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/5493253cc03c_content.py
+-rw-r--r--   0        0        0     1651 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/b791cf213df9_content.py
+-rw-r--r--   0        0        0     1415 2023-03-05 04:20:57.727140 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/d2f2002f3c36_content.py
+-rw-r--r--   0        0        0     2201 2023-03-03 17:13:51.407142 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic.ini
+-rw-r--r--   0        0        0    77824 2023-02-14 03:46:10.695467 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/base_user_database.db
+-rw-r--r--   0        0        0        0 2023-03-10 12:28:15.033139 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-10 12:28:22.753355 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-10 12:27:11.408006 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/__init__.py
+-rw-r--r--   0        0        0     2296 2023-03-10 12:28:05.882882 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/env.py
+-rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/script.py.mako
+-rw-r--r--   0        0        0     1769 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/2c36fcc0b921_content.py
+-rw-r--r--   0        0        0     1649 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/7c1c6e101059_content.py
+-rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/aeb9fe314556_content.py
+-rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/bf20242a238f_content.py
+-rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/d0118d8ec0b4_content.py
+-rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic.ini
+-rw-r--r--   0        0        0      493 2023-03-10 12:30:45.700616 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/messages.py
+-rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/test_messages.db
+-rw-r--r--   0        0        0     2288 2023-03-10 12:32:59.654189 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/env.py
+-rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/script.py.mako
+-rw-r--r--   0        0        0     1762 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/194e05269f09_content.py
+-rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/5b4bea08c27f_content.py
+-rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/6b1b10eb67de_content.py
+-rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/990fc1108317_content.py
+-rw-r--r--   0        0        0     1643 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/a918b6b05d2f_content.py
+-rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic.ini
+-rw-r--r--   0        0        0      488 2023-03-10 12:32:58.467491 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/posts.py
+-rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/test_posts.db
+-rw-r--r--   0        0        0     2294 2023-03-10 12:32:46.997189 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/env.py
+-rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/script.py.mako
+-rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/29f675c35eee_content.py
+-rw-r--r--   0        0        0     1647 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/2e4f8364f7e2_content.py
+-rw-r--r--   0        0        0     1766 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/3076beb33c1b_content.py
+-rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/e0c73f066547_content.py
+-rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/ebc3f4bb0782_content.py
+-rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic.ini
+-rw-r--r--   0        0        0      490 2023-03-10 12:32:57.520800 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/stories.py
+-rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/test_stories.db
+-rw-r--r--   0        0        0        0 2022-12-05 14:27:20.696663 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/__init__.py
+-rw-r--r--   0        0        0     1611 2023-06-03 17:34:00.273754 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/api_model.py
+-rw-r--r--   0        0        0     2764 2023-05-08 21:50:28.707049 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/media_model.py
+-rw-r--r--   0        0        0     2073 2023-04-20 22:22:10.068827 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/user_database.py
+-rw-r--r--   0        0        0    10292 2023-07-18 00:51:38.377898 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/sqlite_database.py
+-rw-r--r--   0        0        0      442 2023-03-12 15:01:42.766490 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/database_manager.py
+-rw-r--r--   0        0        0        0 2023-02-26 16:06:18.482305 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/datascraper_manager/__init__.py
+-rw-r--r--   0        0        0     2306 2023-12-02 00:03:22.382921 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/datascraper_manager/datascraper_manager.py
+-rw-r--r--   0        0        0        0 2023-02-26 16:04:46.426896 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/datascraper_manager/datascrapers/__init__.py
+-rw-r--r--   0        0        0     5349 2023-07-13 02:40:41.499162 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/datascraper_manager/datascrapers/fansly.py
+-rw-r--r--   0        0        0     7775 2024-04-19 16:09:08.875404 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/datascraper_manager/datascrapers/onlyfans.py
+-rw-r--r--   0        0        0    12574 2024-04-19 16:12:18.369164 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/download_manager.py
+-rw-r--r--   0        0        0    27492 2024-05-10 06:59:17.923177 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/filesystem_manager.py
+-rw-r--r--   0        0        0        0 2023-01-26 08:21:03.864558 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/metadata_manager/__init__.py
+-rw-r--r--   0        0        0    35493 2024-04-25 14:10:09.139536 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/metadata_manager/metadata_manager.py
+-rw-r--r--   0        0        0     7120 2023-11-30 21:46:23.292998 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/option_manager.py
+-rw-r--r--   0        0        0     4126 2023-12-14 12:20:50.835331 ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/server_manager.py
+-rw-r--r--   0        0        0        0 2023-03-14 06:55:35.872202 ultima_scraper_collection-2.3.13/ultima_scraper_collection/modules/__init__.py
+-rw-r--r--   0        0        0    23537 2024-04-19 15:22:34.174028 ultima_scraper_collection-2.3.13/ultima_scraper_collection/modules/module_streamliner.py
+-rw-r--r--   0        0        0        0 2023-08-06 03:54:32.746530 ultima_scraper_collection-2.3.13/ultima_scraper_collection/projects/__init__.py
+-rw-r--r--   0        0        0     1954 2023-10-25 18:13:55.913824 ultima_scraper_collection-2.3.13/ultima_scraper_collection/projects/project_manager.py
+-rw-r--r--   0        0        0     1032 2024-05-10 07:02:58.071166 ultima_scraper_collection-2.3.13/ultima_scraper_collection/projects/ultima_archive.py
+-rw-r--r--   0        0        0        0 2023-02-26 16:07:35.717380 ultima_scraper_collection-2.3.13/ultima_scraper_collection/py.typed
+-rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 ultima_scraper_collection-2.3.13/PKG-INFO
```

### Comparing `ultima_scraper_collection-2.3.12/pyproject.toml` & `ultima_scraper_collection-2.3.13/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ultima-scraper-collection"
-version = "2.3.12"
+version = "2.3.13"
 description = ""
 authors = ["UltimaHoarder <1285176+UltimaHoarder@users.noreply.github.com>"]
 packages = [{ include = "ultima_scraper_collection" }]
 include = ["ultima_scraper_collection/py.typed"]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4"
```

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/config.py` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,20 +94,20 @@
 
 
 class GlobalAPI(USAGlobalAPI):
     auto_profile_choice: auto_types = None
     auto_performer_choice: auto_types = None
     auto_content_choice: auto_types = None
     auto_media_choice: auto_types = None
-    jobs = Jobs()
-    metadata_setup = GlobalXPathSetup()
+    jobs: Jobs = Jobs()
+    metadata_setup: GlobalXPathSetup = GlobalXPathSetup()
     metadata_setup.directory_format = (
         "{site_name}/{first_letter}/{model_username}/Metadata"
     )  # type: ignore
-    download_setup = DownloadPathSetup()
+    download_setup: DownloadPathSetup = DownloadPathSetup()
     download_setup.directory_format = (
         "{site_name}/{first_letter}/{model_username}/{api_type}/{value}/{media_type}"
     )  # type: ignore
     download_setup.filename_format = "{filename}.{ext}"  # type: ignore
     blacklists: list[str] = []
 
 
@@ -126,15 +126,15 @@
 
 
 class UltimaScraperCollectionConfig(UltimaScraperAPIConfig):
     class Settings(Settings):
         auto_site_choice: str = ""
         databases: list[Database] = [Database()]
         tools: Tools = Tools()
-        trash = Trash()
+        trash: Trash = Trash()
         infinite_loop: bool = False
         exit_on_completion: bool = True
 
         def get_main_database(self):
             return [x for x in self.databases if x.main][0]
 
     settings: Settings = Settings()
```

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/helpers/main_helper.py` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/helpers/main_helper.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/content_manager.py` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/content_manager.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/env.py` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/0d4d92c0498e_content.py` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/0d4d92c0498e_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/1454e4d1c6b8_content.py` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/1454e4d1c6b8_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/37c4f2719d65_content.py` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/37c4f2719d65_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/5493253cc03c_content.py` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/5493253cc03c_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/b791cf213df9_content.py` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/b791cf213df9_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/d2f2002f3c36_content.py` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/d2f2002f3c36_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic.ini` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic.ini`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/base_user_database.db` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/base_user_database.db`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/env.py` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/2c36fcc0b921_content.py` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/2c36fcc0b921_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/7c1c6e101059_content.py` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/7c1c6e101059_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/aeb9fe314556_content.py` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/aeb9fe314556_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/bf20242a238f_content.py` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/bf20242a238f_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/d0118d8ec0b4_content.py` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/d0118d8ec0b4_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic.ini` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic.ini`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/test_messages.db` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/test_messages.db`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/env.py` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/194e05269f09_content.py` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/194e05269f09_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/5b4bea08c27f_content.py` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/5b4bea08c27f_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/6b1b10eb67de_content.py` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/6b1b10eb67de_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/990fc1108317_content.py` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/990fc1108317_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/a918b6b05d2f_content.py` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/a918b6b05d2f_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic.ini` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic.ini`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/test_posts.db` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/test_posts.db`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/env.py` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/29f675c35eee_content.py` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/29f675c35eee_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/2e4f8364f7e2_content.py` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/2e4f8364f7e2_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/3076beb33c1b_content.py` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/3076beb33c1b_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/e0c73f066547_content.py` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/e0c73f066547_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/ebc3f4bb0782_content.py` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/ebc3f4bb0782_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic.ini` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic.ini`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/test_stories.db` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/test_stories.db`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/api_model.py` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/api_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/media_model.py` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/media_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/user_database.py` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/user_database.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/database_manager/connections/sqlite/sqlite_database.py` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/database_manager/connections/sqlite/sqlite_database.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/datascraper_manager/datascraper_manager.py` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/datascraper_manager/datascraper_manager.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/datascraper_manager/datascrapers/fansly.py` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/datascraper_manager/datascrapers/fansly.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/datascraper_manager/datascrapers/onlyfans.py` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/datascraper_manager/datascrapers/onlyfans.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/download_manager.py` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/download_manager.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/filesystem_manager.py` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/filesystem_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -308,16 +308,14 @@
         final_download_directory = await self.discover_main_directory(performer)
         directory_manager.user.download_directory = final_download_directory
 
         api = authed.api
         performer_username = performer.get_usernames(ignore_id=True)[-1]
         site_name = authed.api.site_name
         alt_directories = await self.discover_alternative_directories(performer)
-        if alt_directories:
-            pass
         await file_manager.set_default_files()
         _metadata_filepaths = await file_manager.find_metadata_files(legacy_files=False)
         # for metadata_filepath in metadata_filepaths:
         #     if file_manager.directory_manager.user.metadata_directory.as_posix() in metadata_filepath.parent.as_posix():
         #         continue
         #     new_filepath = file_manager.directory_manager.user.metadata_directory.joinpath(metadata_filepath.name)
         #     if new_filepath.exists():
```

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/metadata_manager/metadata_manager.py` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/metadata_manager/metadata_manager.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/option_manager.py` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/option_manager.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/managers/server_manager.py` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/managers/server_manager.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/modules/module_streamliner.py` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/modules/module_streamliner.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/projects/project_manager.py` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/projects/project_manager.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.3.12/ultima_scraper_collection/projects/ultima_archive.py` & `ultima_scraper_collection-2.3.13/ultima_scraper_collection/projects/ultima_archive.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,10 +11,10 @@
     async def init(self, config: UltimaScraperCollectionConfig):
         # We could pass a database manager instead of config
         db_info = config.settings.databases[0].connection_info.dict()
         ultima_archive_db = await super()._init_db(
             db_info, Alembica(generate=False, migrate=False), merged_metadata
         )
         self.ultima_archive_db_api = await ArchiveAPI(ultima_archive_db).init()
-        self.fast_api = UAClient()
+        self.fast_api = UAClient(self.ultima_archive_db_api)
         UAClient.database_api = self.ultima_archive_db_api
         return self
```

### Comparing `ultima_scraper_collection-2.3.12/PKG-INFO` & `ultima_scraper_collection-2.3.13/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultima-scraper-collection
-Version: 2.3.12
+Version: 2.3.13
 Summary: 
 Author: UltimaHoarder
 Author-email: 1285176+UltimaHoarder@users.noreply.github.com
 Requires-Python: >=3.10,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

