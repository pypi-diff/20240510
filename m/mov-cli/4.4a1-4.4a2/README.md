# Comparing `tmp/mov_cli-4.4a1.tar.gz` & `tmp/mov_cli-4.4a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov_cli-4.4a1.tar", last modified: Sat May  4 16:39:46 2024, max compression
+gzip compressed data, was "mov_cli-4.4a2.tar", last modified: Fri May 10 02:34:55 2024, max compression
```

## Comparing `mov_cli-4.4a1.tar` & `mov_cli-4.4a2.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-04 16:39:46.289717 mov_cli-4.4a1/
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-04 16:39:46.279717 mov_cli-4.4a1/.github/
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-04 16:39:46.279717 mov_cli-4.4a1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      185 2023-12-08 21:51:24.000000 mov_cli-4.4a1/.github/ISSUE_TEMPLATE/addprovider.md
--rw-r--r--   0 goldy     (1000) goldy     (1000)      925 2023-12-08 21:51:24.000000 mov_cli-4.4a1/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 goldy     (1000) goldy     (1000)      319 2023-12-08 21:51:24.000000 mov_cli-4.4a1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 goldy     (1000) goldy     (1000)      300 2023-12-08 21:51:24.000000 mov_cli-4.4a1/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 goldy     (1000) goldy     (1000)      500 2023-12-08 21:51:24.000000 mov_cli-4.4a1/.github/dependabot.yml
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-04 16:39:46.279717 mov_cli-4.4a1/.github/workflows/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1047 2023-12-08 21:51:24.000000 mov_cli-4.4a1/.github/workflows/pypi.yml
--rw-r--r--   0 goldy     (1000) goldy     (1000)      704 2024-03-20 02:02:17.000000 mov_cli-4.4a1/.github/workflows/ruff.yml
--rw-r--r--   0 goldy     (1000) goldy     (1000)       78 2023-12-08 21:51:24.000000 mov_cli-4.4a1/.gitignore
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1064 2024-03-04 00:50:47.000000 mov_cli-4.4a1/LICENSE
--rw-r--r--   0 goldy     (1000) goldy     (1000)      296 2024-04-25 20:43:50.000000 mov_cli-4.4a1/Makefile
--rw-r--r--   0 goldy     (1000) goldy     (1000)     8018 2024-05-04 16:39:46.289717 mov_cli-4.4a1/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)     5336 2024-05-03 21:25:09.000000 mov_cli-4.4a1/README.md
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1549 2024-04-19 20:31:56.000000 mov_cli-4.4a1/disclaimer.md
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-04 16:39:46.283050 mov_cli-4.4a1/mov_cli/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      135 2024-05-04 16:39:41.000000 mov_cli-4.4a1/mov_cli/__init__.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-04 16:39:46.286383 mov_cli-4.4a1/mov_cli/cli/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       17 2023-12-08 21:51:24.000000 mov_cli-4.4a1/mov_cli/cli/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     5935 2024-05-04 16:39:20.000000 mov_cli-4.4a1/mov_cli/cli/__main__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      416 2024-04-19 20:31:56.000000 mov_cli-4.4a1/mov_cli/cli/auto_select.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2089 2024-04-19 20:31:56.000000 mov_cli-4.4a1/mov_cli/cli/configuration.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2063 2024-04-19 20:31:56.000000 mov_cli-4.4a1/mov_cli/cli/episode.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     3640 2024-05-03 21:25:09.000000 mov_cli-4.4a1/mov_cli/cli/play.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1533 2024-04-29 18:49:16.000000 mov_cli-4.4a1/mov_cli/cli/plugins.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      159 2024-05-03 21:25:09.000000 mov_cli-4.4a1/mov_cli/cli/random_tips.json
--rw-r--r--   0 goldy     (1000) goldy     (1000)     6217 2024-05-03 22:20:27.000000 mov_cli-4.4a1/mov_cli/cli/scraper.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1259 2024-04-25 20:43:50.000000 mov_cli-4.4a1/mov_cli/cli/search.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     6946 2024-04-25 20:43:50.000000 mov_cli-4.4a1/mov_cli/cli/ui.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1320 2024-04-19 20:31:56.000000 mov_cli-4.4a1/mov_cli/cli/watch_options.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     7617 2024-05-03 21:25:09.000000 mov_cli-4.4a1/mov_cli/config.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      621 2024-05-03 21:25:09.000000 mov_cli-4.4a1/mov_cli/config.template.toml
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2245 2024-05-03 21:25:09.000000 mov_cli-4.4a1/mov_cli/download.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      563 2024-05-03 21:25:09.000000 mov_cli-4.4a1/mov_cli/errors.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     3434 2024-05-03 21:25:09.000000 mov_cli-4.4a1/mov_cli/http_client.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-04 16:39:46.286383 mov_cli-4.4a1/mov_cli/iterfzf/
--rw-r--r--   0 goldy     (1000) goldy     (1000)    35147 2024-03-10 14:47:07.000000 mov_cli-4.4a1/mov_cli/iterfzf/LICENSE.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)     4123 2024-04-04 00:43:21.000000 mov_cli-4.4a1/mov_cli/iterfzf/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      229 2023-12-08 21:51:24.000000 mov_cli-4.4a1/mov_cli/logger.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-04 16:39:46.286383 mov_cli-4.4a1/mov_cli/media/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       44 2023-12-08 21:51:24.000000 mov_cli-4.4a1/mov_cli/media/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2953 2024-04-29 18:49:16.000000 mov_cli-4.4a1/mov_cli/media/media.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1859 2024-04-19 20:31:56.000000 mov_cli-4.4a1/mov_cli/media/metadata.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-04 16:39:46.286383 mov_cli-4.4a1/mov_cli/players/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      134 2024-05-03 21:25:09.000000 mov_cli-4.4a1/mov_cli/players/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      972 2024-05-03 21:25:09.000000 mov_cli-4.4a1/mov_cli/players/custom_player.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1599 2024-05-03 21:25:09.000000 mov_cli-4.4a1/mov_cli/players/iina.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1885 2024-05-03 21:25:09.000000 mov_cli-4.4a1/mov_cli/players/mpv.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      715 2024-05-03 21:25:09.000000 mov_cli-4.4a1/mov_cli/players/player.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2305 2024-05-03 21:25:09.000000 mov_cli-4.4a1/mov_cli/players/syncplay.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     3632 2024-05-03 21:25:09.000000 mov_cli-4.4a1/mov_cli/players/vlc.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2047 2024-04-29 18:49:16.000000 mov_cli-4.4a1/mov_cli/plugins.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1776 2024-05-03 22:17:47.000000 mov_cli-4.4a1/mov_cli/scraper.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-04 16:39:46.289717 mov_cli-4.4a1/mov_cli/utils/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       99 2024-04-22 21:39:57.000000 mov_cli-4.4a1/mov_cli/utils/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      620 2024-04-04 00:43:21.000000 mov_cli-4.4a1/mov_cli/utils/episode_selector.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2018 2024-04-22 23:14:10.000000 mov_cli-4.4a1/mov_cli/utils/paths.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      652 2024-03-13 15:29:53.000000 mov_cli-4.4a1/mov_cli/utils/platform.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-04 16:39:46.289717 mov_cli-4.4a1/mov_cli/utils/scraper/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       69 2024-04-19 20:31:56.000000 mov_cli-4.4a1/mov_cli/utils/scraper/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     4751 2024-04-19 20:31:56.000000 mov_cli-4.4a1/mov_cli/utils/scraper/the_movie_db.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2824 2024-05-01 08:46:47.000000 mov_cli-4.4a1/mov_cli/utils/version.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-04 16:39:46.289717 mov_cli-4.4a1/mov_cli.egg-info/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     8018 2024-05-04 16:39:46.000000 mov_cli-4.4a1/mov_cli.egg-info/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1510 2024-05-04 16:39:46.000000 mov_cli-4.4a1/mov_cli.egg-info/SOURCES.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-05-04 16:39:46.000000 mov_cli-4.4a1/mov_cli.egg-info/dependency_links.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)       53 2024-05-04 16:39:46.000000 mov_cli-4.4a1/mov_cli.egg-info/entry_points.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)      228 2024-05-04 16:39:46.000000 mov_cli-4.4a1/mov_cli.egg-info/requires.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)        8 2024-05-04 16:39:46.000000 mov_cli-4.4a1/mov_cli.egg-info/top_level.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1778 2024-05-03 22:13:19.000000 mov_cli-4.4a1/pyproject.toml
--rw-r--r--   0 goldy     (1000) goldy     (1000)      243 2024-04-04 00:43:21.000000 mov_cli-4.4a1/ruff.toml
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-04 16:39:46.289717 mov_cli-4.4a1/scripts/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      285 2023-12-08 21:51:24.000000 mov_cli-4.4a1/scripts/test_cli.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-05-04 16:39:46.289717 mov_cli-4.4a1/setup.cfg
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-10 02:34:55.513348 mov_cli-4.4a2/
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-10 02:34:55.500015 mov_cli-4.4a2/.github/
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-10 02:34:55.503348 mov_cli-4.4a2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      185 2023-12-08 21:51:24.000000 mov_cli-4.4a2/.github/ISSUE_TEMPLATE/addprovider.md
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      925 2023-12-08 21:51:24.000000 mov_cli-4.4a2/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      319 2023-12-08 21:51:24.000000 mov_cli-4.4a2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      300 2023-12-08 21:51:24.000000 mov_cli-4.4a2/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      500 2023-12-08 21:51:24.000000 mov_cli-4.4a2/.github/dependabot.yml
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-10 02:34:55.503348 mov_cli-4.4a2/.github/workflows/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1047 2023-12-08 21:51:24.000000 mov_cli-4.4a2/.github/workflows/pypi.yml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      704 2024-03-20 02:02:17.000000 mov_cli-4.4a2/.github/workflows/ruff.yml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       78 2023-12-08 21:51:24.000000 mov_cli-4.4a2/.gitignore
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1064 2024-03-04 00:50:47.000000 mov_cli-4.4a2/LICENSE
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      296 2024-04-25 20:43:50.000000 mov_cli-4.4a2/Makefile
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     8049 2024-05-10 02:34:55.513348 mov_cli-4.4a2/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     5336 2024-05-03 21:25:09.000000 mov_cli-4.4a2/README.md
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1549 2024-04-19 20:31:56.000000 mov_cli-4.4a2/disclaimer.md
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-10 02:34:55.506681 mov_cli-4.4a2/mov_cli/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      135 2024-05-10 01:48:21.000000 mov_cli-4.4a2/mov_cli/__init__.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-10 02:34:55.510015 mov_cli-4.4a2/mov_cli/cli/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       17 2023-12-08 21:51:24.000000 mov_cli-4.4a2/mov_cli/cli/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     6033 2024-05-10 02:23:24.000000 mov_cli-4.4a2/mov_cli/cli/__main__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      416 2024-04-19 20:31:56.000000 mov_cli-4.4a2/mov_cli/cli/auto_select.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2265 2024-05-10 02:23:30.000000 mov_cli-4.4a2/mov_cli/cli/configuration.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2063 2024-04-19 20:31:56.000000 mov_cli-4.4a2/mov_cli/cli/episode.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     3640 2024-05-03 21:25:09.000000 mov_cli-4.4a2/mov_cli/cli/play.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1533 2024-04-29 18:49:16.000000 mov_cli-4.4a2/mov_cli/cli/plugins.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      159 2024-05-03 21:25:09.000000 mov_cli-4.4a2/mov_cli/cli/random_tips.json
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     6217 2024-05-03 22:20:27.000000 mov_cli-4.4a2/mov_cli/cli/scraper.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1105 2024-05-10 01:47:20.000000 mov_cli-4.4a2/mov_cli/cli/search.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     6946 2024-04-25 20:43:50.000000 mov_cli-4.4a2/mov_cli/cli/ui.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1320 2024-04-19 20:31:56.000000 mov_cli-4.4a2/mov_cli/cli/watch_options.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     8406 2024-05-10 02:04:37.000000 mov_cli-4.4a2/mov_cli/config.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      621 2024-05-03 21:25:09.000000 mov_cli-4.4a2/mov_cli/config.template.toml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2245 2024-05-03 21:25:09.000000 mov_cli-4.4a2/mov_cli/download.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      563 2024-05-03 21:25:09.000000 mov_cli-4.4a2/mov_cli/errors.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     3434 2024-05-03 21:25:09.000000 mov_cli-4.4a2/mov_cli/http_client.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-10 02:34:55.510015 mov_cli-4.4a2/mov_cli/iterfzf/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)    35147 2024-03-10 14:47:07.000000 mov_cli-4.4a2/mov_cli/iterfzf/LICENSE.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     4123 2024-04-04 00:43:21.000000 mov_cli-4.4a2/mov_cli/iterfzf/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      229 2023-12-08 21:51:24.000000 mov_cli-4.4a2/mov_cli/logger.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-10 02:34:55.510015 mov_cli-4.4a2/mov_cli/media/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       44 2023-12-08 21:51:24.000000 mov_cli-4.4a2/mov_cli/media/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2953 2024-04-29 18:49:16.000000 mov_cli-4.4a2/mov_cli/media/media.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2134 2024-05-10 01:51:12.000000 mov_cli-4.4a2/mov_cli/media/metadata.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-10 02:34:55.510015 mov_cli-4.4a2/mov_cli/players/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      134 2024-05-03 21:25:09.000000 mov_cli-4.4a2/mov_cli/players/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      972 2024-05-03 21:25:09.000000 mov_cli-4.4a2/mov_cli/players/custom_player.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1599 2024-05-03 21:25:09.000000 mov_cli-4.4a2/mov_cli/players/iina.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1885 2024-05-03 21:25:09.000000 mov_cli-4.4a2/mov_cli/players/mpv.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      715 2024-05-03 21:25:09.000000 mov_cli-4.4a2/mov_cli/players/player.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2305 2024-05-03 21:25:09.000000 mov_cli-4.4a2/mov_cli/players/syncplay.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     3632 2024-05-03 21:25:09.000000 mov_cli-4.4a2/mov_cli/players/vlc.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2047 2024-04-29 18:49:16.000000 mov_cli-4.4a2/mov_cli/plugins.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1776 2024-05-03 22:17:47.000000 mov_cli-4.4a2/mov_cli/scraper.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-10 02:34:55.513348 mov_cli-4.4a2/mov_cli/utils/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       99 2024-04-22 21:39:57.000000 mov_cli-4.4a2/mov_cli/utils/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      620 2024-04-04 00:43:21.000000 mov_cli-4.4a2/mov_cli/utils/episode_selector.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2018 2024-04-22 23:14:10.000000 mov_cli-4.4a2/mov_cli/utils/paths.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      652 2024-03-13 15:29:53.000000 mov_cli-4.4a2/mov_cli/utils/platform.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-10 02:34:55.513348 mov_cli-4.4a2/mov_cli/utils/scraper/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       69 2024-04-19 20:31:56.000000 mov_cli-4.4a2/mov_cli/utils/scraper/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     4751 2024-04-19 20:31:56.000000 mov_cli-4.4a2/mov_cli/utils/scraper/the_movie_db.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2824 2024-05-01 08:46:47.000000 mov_cli-4.4a2/mov_cli/utils/version.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-10 02:34:55.513348 mov_cli-4.4a2/mov_cli.egg-info/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     8049 2024-05-10 02:34:55.000000 mov_cli-4.4a2/mov_cli.egg-info/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1510 2024-05-10 02:34:55.000000 mov_cli-4.4a2/mov_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-05-10 02:34:55.000000 mov_cli-4.4a2/mov_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       53 2024-05-10 02:34:55.000000 mov_cli-4.4a2/mov_cli.egg-info/entry_points.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      244 2024-05-10 02:34:55.000000 mov_cli-4.4a2/mov_cli.egg-info/requires.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)        8 2024-05-10 02:34:55.000000 mov_cli-4.4a2/mov_cli.egg-info/top_level.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1801 2024-05-10 02:03:17.000000 mov_cli-4.4a2/pyproject.toml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      243 2024-04-04 00:43:21.000000 mov_cli-4.4a2/ruff.toml
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-10 02:34:55.513348 mov_cli-4.4a2/scripts/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      285 2023-12-08 21:51:24.000000 mov_cli-4.4a2/scripts/test_cli.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-05-10 02:34:55.513348 mov_cli-4.4a2/setup.cfg
```

### Comparing `mov_cli-4.4a1/.github/ISSUE_TEMPLATE/bug-report.md` & `mov_cli-4.4a2/.github/ISSUE_TEMPLATE/bug-report.md`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a1/.github/workflows/pypi.yml` & `mov_cli-4.4a2/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a1/.github/workflows/ruff.yml` & `mov_cli-4.4a2/.github/workflows/ruff.yml`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a1/LICENSE` & `mov_cli-4.4a2/LICENSE`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a1/PKG-INFO` & `mov_cli-4.4a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli
-Version: 4.4a1
+Version: 4.4a2
 Summary: Watch everything from your terminal.
 Author-email: Pain <painedposeidon444@gmail.com>, Ananas <ananas@r3tr0ananas.pro>, Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -47,14 +47,15 @@
 Requires-Dist: typer>=0.12.2
 Requires-Dist: inquirer
 Requires-Dist: beautifulsoup4
 Requires-Dist: Unidecode
 Requires-Dist: deprecation
 Requires-Dist: packaging
 Requires-Dist: thefuzz
+Requires-Dist: python-decouple
 Requires-Dist: mov-cli-test>=1.1.0
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: devgoldyutils[pprint]>=2.5.7; extra == "dev"
 
 <a name="readme-top"></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mov-cli Version: 4.4a1 Summary: Watch everything
+Metadata-Version: 2.1 Name: mov-cli Version: 4.4a2 Summary: Watch everything
 from your terminal. Author-email: Pain
 gmail.com>, Ananas
 r3tr0ananas.pro>, Goldy
 devgoldy.xyz> License: MIT License Copyright (c) 2024 mov-cli Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
@@ -26,21 +26,21 @@
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 httpx Requires-Dist: importlib-metadata; python_version < "3.8" Requires-Dist:
 toml Requires-Dist: devgoldyutils>=3.0.0beta1 Requires-Dist: typer>=0.12.2
 Requires-Dist: inquirer Requires-Dist: beautifulsoup4 Requires-Dist: Unidecode
 Requires-Dist: deprecation Requires-Dist: packaging Requires-Dist: thefuzz
-Requires-Dist: mov-cli-test>=1.1.0 Provides-Extra: dev Requires-Dist: ruff;
-extra == "dev" Requires-Dist: build; extra == "dev" Requires-Dist:
-devgoldyutils[pprint]>=2.5.7; extra == "dev" [![Stargazers][stars-shield]]
-[stars-url] [![Pypi Version][pypi-shield]][pypi-url] [![Pypi Downloads][pypi-
-dl-shield]][pypi-stats-url] [![Python Versions][python-shield]][pypi-url] [!
-[Issues][issues-shield]][issues-url] [![MIT License][license-shield]][license-
-url]
+Requires-Dist: python-decouple Requires-Dist: mov-cli-test>=1.1.0 Provides-
+Extra: dev Requires-Dist: ruff; extra == "dev" Requires-Dist: build; extra ==
+"dev" Requires-Dist: devgoldyutils[pprint]>=2.5.7; extra == "dev" [!
+[Stargazers][stars-shield]][stars-url] [![Pypi Version][pypi-shield]][pypi-url]
+[![Pypi Downloads][pypi-dl-shield]][pypi-stats-url] [![Python Versions][python-
+shield]][pypi-url] [![Issues][issues-shield]][issues-url] [![MIT License]
+[license-shield]][license-url]
                   _[_L_o_g_o_]Watch everything from your terminal.
 
                          _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 
                                     _[_L_o_g_o_]
 
 > [!Note] > v4 is constantly changing so be sure to **keep the tool and your
```

### Comparing `mov_cli-4.4a1/README.md` & `mov_cli-4.4a2/README.md`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a1/disclaimer.md` & `mov_cli-4.4a2/disclaimer.md`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a1/mov_cli/cli/__main__.py` & `mov_cli-4.4a2/mov_cli/cli/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import List, Optional, TYPE_CHECKING
 
 if TYPE_CHECKING:
     ...
 
 import typer
 import logging
+from pathlib import Path
 from devgoldyutils import Colours
 
 from .play import play
 from .search import search
 from .ui import welcome_msg
 from .episode import handle_episode
 from .plugins import show_all_plugins
@@ -54,15 +55,16 @@
 
     if config.debug:
         mov_cli_logger.setLevel(logging.DEBUG)
 
     mov_cli_logger.debug(f"Config -> {config.data}")
 
     if edit:
-        open_config_file(config)
+        file_path = None if query is None else Path(query[0])
+        open_config_file(config, file_path)
         return None
 
     plugins = config.plugins
 
     if list_plugins:
         show_all_plugins(plugins)
         return None
```

### Comparing `mov_cli-4.4a1/mov_cli/cli/configuration.py` & `mov_cli-4.4a2/mov_cli/cli/configuration.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
+    from pathlib import Path
     from typing import Optional, Any
     from ..config import Config
 
 import os
 from subprocess import check_call, CalledProcessError
 
 from .. import utils
@@ -33,20 +34,20 @@
         if config.data.get("ui") is None:
             config.data["ui"] = {}
 
         config.data["ui"]["fzf"] = fzf
 
     return config
 
-def open_config_file(config: Config):
+def open_config_file(config: Config, file_path: Optional[Path] = None):
     """Opens the config file in the respectable editor for that platform."""
     editor = config.editor
+    platform = utils.what_platform()
 
     if editor is None: 
-        platform = utils.what_platform()
         env_editor = os.environ.get("EDITOR")        
 
         if env_editor is not None:
             editor = env_editor
         else:
             if platform == "Windows":
                 editor = "notepad"
@@ -55,14 +56,16 @@
             elif platform == "iOS":
                 editor = "vi"
             elif platform == "Linux" or platform == "Android":
                 editor = "nano"
 
     mov_cli_logger.debug("Opening config file...")
 
+    appdata_path = utils.get_appdata_directory(platform)
+
     try:
-        check_call([editor, config.config_path])
+        check_call([editor, config.config_path if file_path is None else appdata_path.joinpath(file_path)])
     except (FileNotFoundError, CalledProcessError) as e:
         mov_cli_logger.error(
             f"Failed to open config file with the editor '{editor}'! Error: {e}" \
                 f"\nYou can manually edit it over here: '{config.config_path}'."
         )
```

### Comparing `mov_cli-4.4a1/mov_cli/cli/episode.py` & `mov_cli-4.4a2/mov_cli/cli/episode.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a1/mov_cli/cli/play.py` & `mov_cli-4.4a2/mov_cli/cli/play.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a1/mov_cli/cli/plugins.py` & `mov_cli-4.4a2/mov_cli/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a1/mov_cli/cli/scraper.py` & `mov_cli-4.4a2/mov_cli/cli/scraper.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a1/mov_cli/cli/search.py` & `mov_cli-4.4a2/mov_cli/cli/search.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,13 +28,12 @@
 
     if auto_select is not None:
         choice = auto_select_choice((choice for choice in search_results), auto_select)
     else:
         choice = prompt(
             "Choose Result", 
             choices = (choice for choice in search_results), 
-            display = lambda x: f"{Colours.BLUE if x.type == MetadataType.SINGLE else Colours.PINK_GREY}{x.title}" \
-                f"{Colours.RESET}" + (f" ({x.year})" if x.year is not None else ""), 
+            display = lambda x: x.display_name, 
             fzf_enabled = fzf_enabled
         )
 
     return choice
```

### Comparing `mov_cli-4.4a1/mov_cli/cli/ui.py` & `mov_cli-4.4a2/mov_cli/cli/ui.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a1/mov_cli/cli/watch_options.py` & `mov_cli-4.4a2/mov_cli/cli/watch_options.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a1/mov_cli/config.py` & `mov_cli-4.4a2/mov_cli/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
     ScrapersConfigT = Dict[Literal["default"], str] | Dict[str, ScraperData]
 
 import os
 import toml
 import shutil
 from pathlib import Path
+from decouple import AutoConfig
 from importlib.util import find_spec
 from devgoldyutils import LoggerAdapter
 
 from . import players, utils
 from .logger import mov_cli_logger
 from .utils import get_appdata_directory
 
@@ -66,14 +67,15 @@
 
 logger = LoggerAdapter(mov_cli_logger, prefix = "Config")
 
 class Config():
     """Class that wraps the mov-cli configuration file. Mostly used under the CLI interface."""
     def __init__(self, override_config: ConfigData = None, config_path: Path = None) -> None:
         self.config_path = config_path
+        self._env_path = self.__get_env_file()
 
         self.data: ConfigData = {}
 
         if override_config is None:
             self.config_path = self.__get_config_file()
 
             try:
@@ -211,14 +213,18 @@
 
         return self.data.get("http", {}).get("headers", default_headers)
 
     @property
     def resolution(self) -> Optional[int]:
         return self.data.get("quality", {}).get("resolution")
 
+    def get_env_config(self) -> AutoConfig:
+        """Returns python decouple config object for mov-cli's appdata .env file."""
+        return AutoConfig(self._env_path)
+
     def __get_config_file(self) -> Path:
         """Function that returns the path to the config file with multi platform support."""
         platform = utils.what_platform()
 
         appdata_folder = get_appdata_directory(platform)
 
         config_path = appdata_folder.joinpath("config.toml")
@@ -231,8 +237,23 @@
 
             with open(template_config_path, "r") as config_template:
                 config_file.write(config_template.read())
 
             config_file.close()
             logger.info(f"Config created at '{config_path}'.")
 
-        return config_path
+        return config_path
+
+    def __get_env_file(self) -> Path:
+        """Function that returns the path to the mov-cli .env file."""
+        platform = utils.what_platform()
+
+        appdata_folder = get_appdata_directory(platform)
+
+        env_file_path = appdata_folder.joinpath(".env")
+
+        if not env_file_path.exists():
+            logger.debug("The 'config.toml' file doesn't exist so we're creating it...")
+            open(env_file_path, "w").close()
+            logger.info(f".env file created at '{env_file_path}'.")
+
+        return env_file_path
```

### Comparing `mov_cli-4.4a1/mov_cli/config.template.toml` & `mov_cli-4.4a2/mov_cli/config.template.toml`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a1/mov_cli/download.py` & `mov_cli-4.4a2/mov_cli/download.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a1/mov_cli/errors.py` & `mov_cli-4.4a2/mov_cli/errors.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a1/mov_cli/http_client.py` & `mov_cli-4.4a2/mov_cli/http_client.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a1/mov_cli/iterfzf/LICENSE.txt` & `mov_cli-4.4a2/mov_cli/iterfzf/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a1/mov_cli/iterfzf/__init__.py` & `mov_cli-4.4a2/mov_cli/iterfzf/__init__.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a1/mov_cli/media/media.py` & `mov_cli-4.4a2/mov_cli/media/media.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a1/mov_cli/media/metadata.py` & `mov_cli-4.4a2/mov_cli/media/metadata.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from typing import List, Callable, Optional, Tuple
 
 from enum import Enum
+from devgoldyutils import Colours
 from dataclasses import dataclass, field
 
 __all__ = ("MetadataType", "Metadata", "ExtraMetadata", "AiringType")
 
 class MetadataType(Enum):
     MULTI = 0
     """Media with multiple seasons and episodes."""
@@ -37,25 +38,29 @@
     """The type of metadata. Is it a Series, Film or LIVE TV Station?"""
     year: Optional[str] = field(default = None)
     """Year the Series or Film was released."""
 
     extra_func: Callable[[], Optional[ExtraMetadata]] = field(default = lambda: None)
     """Callback that returns extra metadata."""
 
+    @property
+    def display_name(self) -> str:
+        return f"{Colours.BLUE if self.type == MetadataType.SINGLE else Colours.PINK_GREY}{self.title}" \
+            f"{Colours.RESET}" + (f" ({self.year})" if self.year is not None else "")
+
     def get_extra(self) -> Optional[ExtraMetadata]:
         """Returns extra metadata."""
         return self.extra_func()
 
 @dataclass
 class ExtraMetadata():
     """More in-depth metadata about media."""
     description: Optional[str]
     """Description of Series, Film or TV Station."""
     image_url: Optional[str]
     """Url to high res image cover of Series, Film or TV Station."""
-
     alternate_titles: List[str] | Tuple[str, str]
 
     cast: List[str] | None = field(default = None)
     genres: List[str] | None = field(default = None)
 
     airing: AiringType | None = field(default = None)
```

### Comparing `mov_cli-4.4a1/mov_cli/players/custom_player.py` & `mov_cli-4.4a2/mov_cli/players/custom_player.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a1/mov_cli/players/iina.py` & `mov_cli-4.4a2/mov_cli/players/iina.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a1/mov_cli/players/mpv.py` & `mov_cli-4.4a2/mov_cli/players/mpv.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a1/mov_cli/players/player.py` & `mov_cli-4.4a2/mov_cli/players/player.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a1/mov_cli/players/syncplay.py` & `mov_cli-4.4a2/mov_cli/players/syncplay.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a1/mov_cli/players/vlc.py` & `mov_cli-4.4a2/mov_cli/players/vlc.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a1/mov_cli/plugins.py` & `mov_cli-4.4a2/mov_cli/plugins.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a1/mov_cli/scraper.py` & `mov_cli-4.4a2/mov_cli/scraper.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a1/mov_cli/utils/episode_selector.py` & `mov_cli-4.4a2/mov_cli/utils/episode_selector.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a1/mov_cli/utils/paths.py` & `mov_cli-4.4a2/mov_cli/utils/paths.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a1/mov_cli/utils/platform.py` & `mov_cli-4.4a2/mov_cli/utils/platform.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a1/mov_cli/utils/scraper/the_movie_db.py` & `mov_cli-4.4a2/mov_cli/utils/scraper/the_movie_db.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a1/mov_cli/utils/version.py` & `mov_cli-4.4a2/mov_cli/utils/version.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a1/mov_cli.egg-info/PKG-INFO` & `mov_cli-4.4a2/mov_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli
-Version: 4.4a1
+Version: 4.4a2
 Summary: Watch everything from your terminal.
 Author-email: Pain <painedposeidon444@gmail.com>, Ananas <ananas@r3tr0ananas.pro>, Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -47,14 +47,15 @@
 Requires-Dist: typer>=0.12.2
 Requires-Dist: inquirer
 Requires-Dist: beautifulsoup4
 Requires-Dist: Unidecode
 Requires-Dist: deprecation
 Requires-Dist: packaging
 Requires-Dist: thefuzz
+Requires-Dist: python-decouple
 Requires-Dist: mov-cli-test>=1.1.0
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: devgoldyutils[pprint]>=2.5.7; extra == "dev"
 
 <a name="readme-top"></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mov-cli Version: 4.4a1 Summary: Watch everything
+Metadata-Version: 2.1 Name: mov-cli Version: 4.4a2 Summary: Watch everything
 from your terminal. Author-email: Pain
 gmail.com>, Ananas
 r3tr0ananas.pro>, Goldy
 devgoldy.xyz> License: MIT License Copyright (c) 2024 mov-cli Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
@@ -26,21 +26,21 @@
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 httpx Requires-Dist: importlib-metadata; python_version < "3.8" Requires-Dist:
 toml Requires-Dist: devgoldyutils>=3.0.0beta1 Requires-Dist: typer>=0.12.2
 Requires-Dist: inquirer Requires-Dist: beautifulsoup4 Requires-Dist: Unidecode
 Requires-Dist: deprecation Requires-Dist: packaging Requires-Dist: thefuzz
-Requires-Dist: mov-cli-test>=1.1.0 Provides-Extra: dev Requires-Dist: ruff;
-extra == "dev" Requires-Dist: build; extra == "dev" Requires-Dist:
-devgoldyutils[pprint]>=2.5.7; extra == "dev" [![Stargazers][stars-shield]]
-[stars-url] [![Pypi Version][pypi-shield]][pypi-url] [![Pypi Downloads][pypi-
-dl-shield]][pypi-stats-url] [![Python Versions][python-shield]][pypi-url] [!
-[Issues][issues-shield]][issues-url] [![MIT License][license-shield]][license-
-url]
+Requires-Dist: python-decouple Requires-Dist: mov-cli-test>=1.1.0 Provides-
+Extra: dev Requires-Dist: ruff; extra == "dev" Requires-Dist: build; extra ==
+"dev" Requires-Dist: devgoldyutils[pprint]>=2.5.7; extra == "dev" [!
+[Stargazers][stars-shield]][stars-url] [![Pypi Version][pypi-shield]][pypi-url]
+[![Pypi Downloads][pypi-dl-shield]][pypi-stats-url] [![Python Versions][python-
+shield]][pypi-url] [![Issues][issues-shield]][issues-url] [![MIT License]
+[license-shield]][license-url]
                   _[_L_o_g_o_]Watch everything from your terminal.
 
                          _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 
                                     _[_L_o_g_o_]
 
 > [!Note] > v4 is constantly changing so be sure to **keep the tool and your
```

### Comparing `mov_cli-4.4a1/mov_cli.egg-info/SOURCES.txt` & `mov_cli-4.4a2/mov_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a1/pyproject.toml` & `mov_cli-4.4a2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     "typer>=0.12.2",
     "inquirer",
     "beautifulsoup4",
     "Unidecode",
     "deprecation",
     "packaging",
     "thefuzz",
+    "python-decouple",
 
     # Included plugins
     "mov-cli-test>=1.1.0"
 ]
 
 dynamic = ["version"]
```

