# Comparing `tmp/profcomff_definitions-2024.5.7.tar.gz` & `tmp/profcomff_definitions-2024.5.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "profcomff_definitions-2024.5.7.tar", last modified: Tue May  7 00:24:11 2024, max compression
+gzip compressed data, was "profcomff_definitions-2024.5.7.1.tar", last modified: Tue May  7 02:16:21 2024, max compression
```

## Comparing `profcomff_definitions-2024.5.7.tar` & `profcomff_definitions-2024.5.7.1.tar`

### file list

```diff
@@ -1,82 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:24:11.162075 profcomff_definitions-2024.5.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:24:11.150075 profcomff_definitions-2024.5.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:24:11.154075 profcomff_definitions-2024.5.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/.github/workflows/checks.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/.github/workflows/deploy_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     9030 2024-05-07 00:24:11.162075 profcomff_definitions-2024.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/alembic.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:24:11.154075 profcomff_definitions-2024.5.7/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/migrations/README
--rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/migrations/env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:24:11.154075 profcomff_definitions-2024.5.7/migrations/rights/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/migrations/rights/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/migrations/rights/operations_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/migrations/rights/operations_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/migrations/rights/render.py
--rw-r--r--   0 runner    (1001) docker     (127)     8112 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/migrations/rights/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:24:11.154075 profcomff_definitions-2024.5.7/migrations/schema/
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/migrations/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/migrations/schema/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/migrations/schema/render.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/migrations/schema/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/migrations/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:24:11.158075 profcomff_definitions-2024.5.7/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/migrations/versions/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/migrations/versions/0a24041f09d1_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/migrations/versions/1e868db5c6ea_physics_contacts.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/migrations/versions/45f0a9e06fca_add_social_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/migrations/versions/4892e78eb989_add_raw_html.py
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/migrations/versions/6f659c404b5f_add_container_log.py
--rw-r--r--   0 runner    (1001) docker     (127)    85873 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/migrations/versions/77d9cf76373d_the_great_megre.py
--rw-r--r--   0 runner    (1001) docker     (127)    59583 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/migrations/versions/a80b250420e4_schema_integrity_fixes.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/migrations/versions/b0d0bbe799db_fix_reciever.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/migrations/versions/d71054079206_fix_tg_chat_int_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/migrations/versions/fa6331fe4c72_rights.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:24:11.158075 profcomff_definitions-2024.5.7/profcomff_definitions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:24:11.158075 profcomff_definitions-2024.5.7/profcomff_definitions/DM/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/profcomff_definitions/DM/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/profcomff_definitions/DM/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:24:11.158075 profcomff_definitions-2024.5.7/profcomff_definitions/DWH/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/profcomff_definitions/DWH/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/profcomff_definitions/DWH/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:24:11.158075 profcomff_definitions-2024.5.7/profcomff_definitions/ODS/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/profcomff_definitions/ODS/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/profcomff_definitions/ODS/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/profcomff_definitions/ODS/timetable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:24:11.162075 profcomff_definitions-2024.5.7/profcomff_definitions/STG/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/profcomff_definitions/STG/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/profcomff_definitions/STG/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/profcomff_definitions/STG/achievement.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/profcomff_definitions/STG/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/profcomff_definitions/STG/infra.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/profcomff_definitions/STG/marketing.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/profcomff_definitions/STG/physics.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/profcomff_definitions/STG/pinger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/profcomff_definitions/STG/print.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/profcomff_definitions/STG/rasphysmsu.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/profcomff_definitions/STG/services.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/profcomff_definitions/STG/social.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/profcomff_definitions/STG/timetable.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/profcomff_definitions/STG/union_member.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/profcomff_definitions/STG/userdata.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/profcomff_definitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/profcomff_definitions/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:24:11.162075 profcomff_definitions-2024.5.7/profcomff_definitions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9030 2024-05-07 00:24:11.000000 profcomff_definitions-2024.5.7/profcomff_definitions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-07 00:24:11.000000 profcomff_definitions-2024.5.7/profcomff_definitions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 00:24:11.000000 profcomff_definitions-2024.5.7/profcomff_definitions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-07 00:24:11.000000 profcomff_definitions-2024.5.7/profcomff_definitions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-07 00:24:11.000000 profcomff_definitions-2024.5.7/profcomff_definitions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/requirements.dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 00:24:11.162075 profcomff_definitions-2024.5.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:24:11.162075 profcomff_definitions-2024.5.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/tests/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-07 00:23:53.000000 profcomff_definitions-2024.5.7/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:16:21.046528 profcomff_definitions-2024.5.7.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:16:21.034528 profcomff_definitions-2024.5.7.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:16:21.034528 profcomff_definitions-2024.5.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/.github/workflows/checks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/.github/workflows/deploy_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     9032 2024-05-07 02:16:21.046528 profcomff_definitions-2024.5.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/alembic.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:16:21.038529 profcomff_definitions-2024.5.7.1/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/migrations/README
+-rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/migrations/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:16:21.038529 profcomff_definitions-2024.5.7.1/migrations/rights/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/migrations/rights/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/migrations/rights/operations_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/migrations/rights/operations_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/migrations/rights/render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8112 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/migrations/rights/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:16:21.038529 profcomff_definitions-2024.5.7.1/migrations/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/migrations/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/migrations/schema/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/migrations/schema/render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/migrations/schema/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/migrations/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:16:21.038529 profcomff_definitions-2024.5.7.1/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/migrations/versions/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/migrations/versions/20230828_1334_0a24041f09d1_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/migrations/versions/20230828_1335_fa6331fe4c72_rights.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85873 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/migrations/versions/20230910_1318_77d9cf76373d_the_great_megre.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/migrations/versions/20230911_2126_1e868db5c6ea_physics_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/migrations/versions/20240422_1624_4892e78eb989_add_raw_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59583 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/migrations/versions/20240505_0010_a80b250420e4_schema_integrity_fixes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/migrations/versions/20240505_0047_b0d0bbe799db_fix_reciever.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/migrations/versions/20240505_0135_d71054079206_fix_tg_chat_int_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/migrations/versions/20240507_0035_45f0a9e06fca_add_social_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/migrations/versions/20240507_0246_6f659c404b5f_add_container_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/migrations/versions/20240507_0436_45fc3ad3a4db_add_container_log_in_ods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/migrations/versions/20240507_0454_33f7db929809_docker_ps_table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:16:21.042528 profcomff_definitions-2024.5.7.1/profcomff_definitions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:16:21.042528 profcomff_definitions-2024.5.7.1/profcomff_definitions/DM/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/profcomff_definitions/DM/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/profcomff_definitions/DM/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:16:21.042528 profcomff_definitions-2024.5.7.1/profcomff_definitions/DWH/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/profcomff_definitions/DWH/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/profcomff_definitions/DWH/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:16:21.042528 profcomff_definitions-2024.5.7.1/profcomff_definitions/ODS/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/profcomff_definitions/ODS/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/profcomff_definitions/ODS/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/profcomff_definitions/ODS/infra_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/profcomff_definitions/ODS/timetable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:16:21.046528 profcomff_definitions-2024.5.7.1/profcomff_definitions/STG/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/profcomff_definitions/STG/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/profcomff_definitions/STG/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/profcomff_definitions/STG/achievement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/profcomff_definitions/STG/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/profcomff_definitions/STG/infra.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/profcomff_definitions/STG/marketing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/profcomff_definitions/STG/physics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/profcomff_definitions/STG/pinger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/profcomff_definitions/STG/print.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/profcomff_definitions/STG/rasphysmsu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/profcomff_definitions/STG/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/profcomff_definitions/STG/social.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/profcomff_definitions/STG/timetable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/profcomff_definitions/STG/union_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/profcomff_definitions/STG/userdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/profcomff_definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/profcomff_definitions/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:16:21.046528 profcomff_definitions-2024.5.7.1/profcomff_definitions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9032 2024-05-07 02:16:21.000000 profcomff_definitions-2024.5.7.1/profcomff_definitions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-07 02:16:21.000000 profcomff_definitions-2024.5.7.1/profcomff_definitions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 02:16:21.000000 profcomff_definitions-2024.5.7.1/profcomff_definitions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-07 02:16:21.000000 profcomff_definitions-2024.5.7.1/profcomff_definitions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-07 02:16:21.000000 profcomff_definitions-2024.5.7.1/profcomff_definitions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/requirements.dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 02:16:21.046528 profcomff_definitions-2024.5.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:16:21.046528 profcomff_definitions-2024.5.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/tests/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-07 02:16:12.000000 profcomff_definitions-2024.5.7.1/tests/tests.py
```

### Comparing `profcomff_definitions-2024.5.7/.github/workflows/checks.yml` & `profcomff_definitions-2024.5.7.1/.github/workflows/checks.yml`

 * *Files identical despite different names*

### Comparing `profcomff_definitions-2024.5.7/.github/workflows/deploy_and_publish.yml` & `profcomff_definitions-2024.5.7.1/.github/workflows/deploy_and_publish.yml`

 * *Files identical despite different names*

### Comparing `profcomff_definitions-2024.5.7/.gitignore` & `profcomff_definitions-2024.5.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `profcomff_definitions-2024.5.7/LICENSE` & `profcomff_definitions-2024.5.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `profcomff_definitions-2024.5.7/Makefile` & `profcomff_definitions-2024.5.7.1/Makefile`

 * *Files identical despite different names*

### Comparing `profcomff_definitions-2024.5.7/PKG-INFO` & `profcomff_definitions-2024.5.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: profcomff_definitions
-Version: 2024.5.7
+Version: 2024.5.7.1
 Summary: Data warehouse definitions and schemas
 Author-email: "profcomff.com" <admin@profcomff.com>, Roman Dyakov <roman@dyakov.space>, Stanislav Roslavtsev <roslavtzev.stanislaw@yandex.ru>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Профком студентов физфака МГУ
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `profcomff_definitions-2024.5.7/README.md` & `profcomff_definitions-2024.5.7.1/README.md`

 * *Files identical despite different names*

### Comparing `profcomff_definitions-2024.5.7/alembic.ini` & `profcomff_definitions-2024.5.7.1/alembic.ini`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # A generic, single database configuration.
 
 [alembic]
 # path to migration scripts
 script_location = migrations
 
 # template used to generate migration files
-# file_template = %%(rev)s_%%(slug)s
+file_template = %%(year)d%%(month).2d%%(day).2d_%%(hour).2d%%(minute).2d_%%(rev)s_%%(slug)s
 
 # sys.path path, will be prepended to sys.path if present.
 # defaults to the current working directory.
 prepend_sys_path = .
 
 # timezone to use when rendering the date within the migration file
 # as well as the filename.
@@ -90,8 +90,8 @@
 class = StreamHandler
 args = (sys.stderr,)
 level = NOTSET
 formatter = generic
 
 [formatter_generic]
 format = %(levelname)-5.5s [%(name)s] %(message)s
-datefmt = %H:%M:%S
+datefmt = %H:%M:%S
```

### Comparing `profcomff_definitions-2024.5.7/migrations/env.py` & `profcomff_definitions-2024.5.7.1/migrations/env.py`

 * *Files identical despite different names*

### Comparing `profcomff_definitions-2024.5.7/migrations/rights/operations_groups.py` & `profcomff_definitions-2024.5.7.1/migrations/rights/operations_groups.py`

 * *Files identical despite different names*

### Comparing `profcomff_definitions-2024.5.7/migrations/rights/operations_tables.py` & `profcomff_definitions-2024.5.7.1/migrations/rights/operations_tables.py`

 * *Files identical despite different names*

### Comparing `profcomff_definitions-2024.5.7/migrations/rights/render.py` & `profcomff_definitions-2024.5.7.1/migrations/rights/render.py`

 * *Files identical despite different names*

### Comparing `profcomff_definitions-2024.5.7/migrations/rights/schemas.py` & `profcomff_definitions-2024.5.7.1/migrations/rights/schemas.py`

 * *Files identical despite different names*

### Comparing `profcomff_definitions-2024.5.7/migrations/schema/operations.py` & `profcomff_definitions-2024.5.7.1/migrations/schema/operations.py`

 * *Files identical despite different names*

### Comparing `profcomff_definitions-2024.5.7/migrations/schema/schemas.py` & `profcomff_definitions-2024.5.7.1/migrations/schema/schemas.py`

 * *Files identical despite different names*

### Comparing `profcomff_definitions-2024.5.7/migrations/versions/0a24041f09d1_init.py` & `profcomff_definitions-2024.5.7.1/migrations/versions/20230828_1334_0a24041f09d1_init.py`

 * *Files identical despite different names*

### Comparing `profcomff_definitions-2024.5.7/migrations/versions/1e868db5c6ea_physics_contacts.py` & `profcomff_definitions-2024.5.7.1/migrations/versions/20230911_2126_1e868db5c6ea_physics_contacts.py`

 * *Files identical despite different names*

### Comparing `profcomff_definitions-2024.5.7/migrations/versions/45f0a9e06fca_add_social_fields.py` & `profcomff_definitions-2024.5.7.1/migrations/versions/20240507_0035_45f0a9e06fca_add_social_fields.py`

 * *Files identical despite different names*

### Comparing `profcomff_definitions-2024.5.7/migrations/versions/4892e78eb989_add_raw_html.py` & `profcomff_definitions-2024.5.7.1/migrations/versions/20240422_1624_4892e78eb989_add_raw_html.py`

 * *Files identical despite different names*

### Comparing `profcomff_definitions-2024.5.7/migrations/versions/6f659c404b5f_add_container_log.py` & `profcomff_definitions-2024.5.7.1/migrations/versions/20240507_0246_6f659c404b5f_add_container_log.py`

 * *Files identical despite different names*

### Comparing `profcomff_definitions-2024.5.7/migrations/versions/77d9cf76373d_the_great_megre.py` & `profcomff_definitions-2024.5.7.1/migrations/versions/20230910_1318_77d9cf76373d_the_great_megre.py`

 * *Files identical despite different names*

### Comparing `profcomff_definitions-2024.5.7/migrations/versions/a80b250420e4_schema_integrity_fixes.py` & `profcomff_definitions-2024.5.7.1/migrations/versions/20240505_0010_a80b250420e4_schema_integrity_fixes.py`

 * *Files identical despite different names*

### Comparing `profcomff_definitions-2024.5.7/migrations/versions/d71054079206_fix_tg_chat_int_type.py` & `profcomff_definitions-2024.5.7.1/migrations/versions/20240505_0135_d71054079206_fix_tg_chat_int_type.py`

 * *Files identical despite different names*

### Comparing `profcomff_definitions-2024.5.7/migrations/versions/fa6331fe4c72_rights.py` & `profcomff_definitions-2024.5.7.1/migrations/versions/20230828_1335_fa6331fe4c72_rights.py`

 * *Files identical despite different names*

### Comparing `profcomff_definitions-2024.5.7/profcomff_definitions/STG/achievement.py` & `profcomff_definitions-2024.5.7.1/profcomff_definitions/STG/achievement.py`

 * *Files identical despite different names*

### Comparing `profcomff_definitions-2024.5.7/profcomff_definitions/STG/auth.py` & `profcomff_definitions-2024.5.7.1/profcomff_definitions/STG/auth.py`

 * *Files identical despite different names*

### Comparing `profcomff_definitions-2024.5.7/profcomff_definitions/STG/marketing.py` & `profcomff_definitions-2024.5.7.1/profcomff_definitions/STG/marketing.py`

 * *Files identical despite different names*

### Comparing `profcomff_definitions-2024.5.7/profcomff_definitions/STG/pinger.py` & `profcomff_definitions-2024.5.7.1/profcomff_definitions/STG/pinger.py`

 * *Files identical despite different names*

### Comparing `profcomff_definitions-2024.5.7/profcomff_definitions/STG/print.py` & `profcomff_definitions-2024.5.7.1/profcomff_definitions/STG/print.py`

 * *Files identical despite different names*

### Comparing `profcomff_definitions-2024.5.7/profcomff_definitions/STG/services.py` & `profcomff_definitions-2024.5.7.1/profcomff_definitions/STG/services.py`

 * *Files identical despite different names*

### Comparing `profcomff_definitions-2024.5.7/profcomff_definitions/STG/social.py` & `profcomff_definitions-2024.5.7.1/profcomff_definitions/STG/social.py`

 * *Files identical despite different names*

### Comparing `profcomff_definitions-2024.5.7/profcomff_definitions/STG/timetable.py` & `profcomff_definitions-2024.5.7.1/profcomff_definitions/STG/timetable.py`

 * *Files identical despite different names*

### Comparing `profcomff_definitions-2024.5.7/profcomff_definitions/STG/union_member.py` & `profcomff_definitions-2024.5.7.1/profcomff_definitions/STG/union_member.py`

 * *Files identical despite different names*

### Comparing `profcomff_definitions-2024.5.7/profcomff_definitions/STG/userdata.py` & `profcomff_definitions-2024.5.7.1/profcomff_definitions/STG/userdata.py`

 * *Files identical despite different names*

### Comparing `profcomff_definitions-2024.5.7/profcomff_definitions/__init__.py` & `profcomff_definitions-2024.5.7.1/profcomff_definitions/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import sys
 
 
-__version__ = '2024.05.07'
+__version__ = '2024.05.07.1'
 
 
 dir_path = os.path.dirname(os.path.abspath(__file__))
 for folder in ['STG', 'DWH', 'DM', 'ODS']:
     files_in_dir = [f[:-3] for f in os.listdir(dir_path + '/' + folder) if f.endswith('.py') and f != '__init__.py']
     for f in files_in_dir:
         mod = __import__('.'.join([__name__, folder, f]), fromlist=[f])
```

### Comparing `profcomff_definitions-2024.5.7/profcomff_definitions/base.py` & `profcomff_definitions-2024.5.7.1/profcomff_definitions/base.py`

 * *Files identical despite different names*

### Comparing `profcomff_definitions-2024.5.7/profcomff_definitions.egg-info/PKG-INFO` & `profcomff_definitions-2024.5.7.1/profcomff_definitions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: profcomff_definitions
-Version: 2024.5.7
+Version: 2024.5.7.1
 Summary: Data warehouse definitions and schemas
 Author-email: "profcomff.com" <admin@profcomff.com>, Roman Dyakov <roman@dyakov.space>, Stanislav Roslavtsev <roslavtzev.stanislaw@yandex.ru>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Профком студентов физфака МГУ
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `profcomff_definitions-2024.5.7/profcomff_definitions.egg-info/SOURCES.txt` & `profcomff_definitions-2024.5.7.1/profcomff_definitions.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -17,37 +17,40 @@
 migrations/rights/render.py
 migrations/rights/schemas.py
 migrations/schema/__init__.py
 migrations/schema/operations.py
 migrations/schema/render.py
 migrations/schema/schemas.py
 migrations/versions/.gitkeep
-migrations/versions/0a24041f09d1_init.py
-migrations/versions/1e868db5c6ea_physics_contacts.py
-migrations/versions/45f0a9e06fca_add_social_fields.py
-migrations/versions/4892e78eb989_add_raw_html.py
-migrations/versions/6f659c404b5f_add_container_log.py
-migrations/versions/77d9cf76373d_the_great_megre.py
-migrations/versions/a80b250420e4_schema_integrity_fixes.py
-migrations/versions/b0d0bbe799db_fix_reciever.py
-migrations/versions/d71054079206_fix_tg_chat_int_type.py
-migrations/versions/fa6331fe4c72_rights.py
+migrations/versions/20230828_1334_0a24041f09d1_init.py
+migrations/versions/20230828_1335_fa6331fe4c72_rights.py
+migrations/versions/20230910_1318_77d9cf76373d_the_great_megre.py
+migrations/versions/20230911_2126_1e868db5c6ea_physics_contacts.py
+migrations/versions/20240422_1624_4892e78eb989_add_raw_html.py
+migrations/versions/20240505_0010_a80b250420e4_schema_integrity_fixes.py
+migrations/versions/20240505_0047_b0d0bbe799db_fix_reciever.py
+migrations/versions/20240505_0135_d71054079206_fix_tg_chat_int_type.py
+migrations/versions/20240507_0035_45f0a9e06fca_add_social_fields.py
+migrations/versions/20240507_0246_6f659c404b5f_add_container_log.py
+migrations/versions/20240507_0436_45fc3ad3a4db_add_container_log_in_ods.py
+migrations/versions/20240507_0454_33f7db929809_docker_ps_table.py
 profcomff_definitions/__init__.py
 profcomff_definitions/base.py
 profcomff_definitions.egg-info/PKG-INFO
 profcomff_definitions.egg-info/SOURCES.txt
 profcomff_definitions.egg-info/dependency_links.txt
 profcomff_definitions.egg-info/requires.txt
 profcomff_definitions.egg-info/top_level.txt
 profcomff_definitions/DM/README.md
 profcomff_definitions/DM/__init__.py
 profcomff_definitions/DWH/README.md
 profcomff_definitions/DWH/__init__.py
 profcomff_definitions/ODS/README.md
 profcomff_definitions/ODS/__init__.py
+profcomff_definitions/ODS/infra_logs.py
 profcomff_definitions/ODS/timetable.py
 profcomff_definitions/STG/README.md
 profcomff_definitions/STG/__init__.py
 profcomff_definitions/STG/achievement.py
 profcomff_definitions/STG/auth.py
 profcomff_definitions/STG/infra.py
 profcomff_definitions/STG/marketing.py
```

### Comparing `profcomff_definitions-2024.5.7/pyproject.toml` & `profcomff_definitions-2024.5.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `profcomff_definitions-2024.5.7/tests/conftest.py` & `profcomff_definitions-2024.5.7.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `profcomff_definitions-2024.5.7/tests/tests.py` & `profcomff_definitions-2024.5.7.1/tests/tests.py`

 * *Files identical despite different names*

