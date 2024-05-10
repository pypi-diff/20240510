# Comparing `tmp/snews_pt-1.3.3.tar.gz` & `tmp/snews_pt-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/bj7780/Desktop/Kara/GitHub/SNEWS/SNEWS_Publishing_Tools/dist/.tmp-0pipga2x/snews_pt-1.3.3.tar", last modified: Fri May 12 08:19:34 2023, max compression
+gzip compressed data, was "snews_pt-1.3.4.tar", last modified: Fri May 10 12:59:55 2024, max compression
```

## Comparing `snews_pt-1.3.3.tar` & `snews_pt-1.3.4.tar`

### file list

```diff
@@ -1,102 +1,98 @@
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-05-12 08:19:34.000000 snews_pt-1.3.3/
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-05-12 08:19:31.000000 snews_pt-1.3.3/.github/
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-05-12 08:19:32.000000 snews_pt-1.3.3/.github/workflows/
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1878 2022-05-20 12:43:48.000000 snews_pt-1.3.3/.github/workflows/mac10-py37.yml
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1878 2022-05-20 12:43:48.000000 snews_pt-1.3.3/.github/workflows/mac10-py38.yml
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1877 2022-05-20 12:43:48.000000 snews_pt-1.3.3/.github/workflows/mac11-py310.yml
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1875 2022-05-20 12:43:48.000000 snews_pt-1.3.3/.github/workflows/mac11-py37.yml
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1875 2022-05-20 12:43:48.000000 snews_pt-1.3.3/.github/workflows/mac11-py38.yml
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1817 2022-07-29 18:24:09.000000 snews_pt-1.3.3/.github/workflows/mac11-py39.yml
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2367 2023-02-06 12:44:04.000000 snews_pt-1.3.3/.github/workflows/ubuntu20-py310.yml
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2135 2023-02-06 12:44:04.000000 snews_pt-1.3.3/.github/workflows/ubuntu20-py37-310.yml
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2378 2022-05-20 13:27:18.000000 snews_pt-1.3.3/.github/workflows/ubuntu20-py37.yml
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2378 2022-05-20 13:27:18.000000 snews_pt-1.3.3/.github/workflows/ubuntu20-py38.yml
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2090 2023-02-06 12:44:04.000000 snews_pt-1.3.3/.github/workflows/ubuntu20-py39.yml
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      178 2022-05-20 14:39:26.000000 snews_pt-1.3.3/.readthedocs.yaml
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      436 2023-05-12 08:19:27.000000 snews_pt-1.3.3/AUTHORS
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)    16952 2023-05-12 08:19:26.000000 snews_pt-1.3.3/ChangeLog
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)    10037 2023-05-12 08:19:34.000000 snews_pt-1.3.3/PKG-INFO
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     9034 2022-09-27 15:09:46.000000 snews_pt-1.3.3/README.md
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-05-12 08:19:32.000000 snews_pt-1.3.3/docs/
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      623 2022-05-20 12:43:48.000000 snews_pt-1.3.3/docs/Makefile
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      205 2022-05-20 12:43:48.000000 snews_pt-1.3.3/docs/README.md
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-05-12 08:19:31.000000 snews_pt-1.3.3/docs/_static/
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-05-12 08:19:32.000000 snews_pt-1.3.3/docs/_static/css/
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      616 2022-05-20 12:43:48.000000 snews_pt-1.3.3/docs/_static/css/my_theme.css
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-05-12 08:19:32.000000 snews_pt-1.3.3/docs/_templates/
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)       60 2022-05-20 12:43:48.000000 snews_pt-1.3.3/docs/_templates/layout.html
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-05-12 08:19:32.000000 snews_pt-1.3.3/docs/api/
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      148 2022-05-20 12:43:48.000000 snews_pt-1.3.3/docs/api/api.rst
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      129 2022-05-20 13:27:18.000000 snews_pt-1.3.3/docs/api/message_schema.rst
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      123 2022-05-20 13:27:18.000000 snews_pt-1.3.3/docs/api/snews_pt_utils.rst
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      111 2022-05-20 13:27:18.000000 snews_pt-1.3.3/docs/api/snews_pub.rst
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      114 2022-05-20 13:27:18.000000 snews_pt-1.3.3/docs/api/snews_sub.rst
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     6080 2022-05-20 13:27:18.000000 snews_pt-1.3.3/docs/cli_docs.md
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      535 2022-05-20 12:43:48.000000 snews_pt-1.3.3/docs/cli_help.txt
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     4472 2022-09-27 15:04:20.000000 snews_pt-1.3.3/docs/conf.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)   139863 2022-04-28 07:02:44.000000 snews_pt-1.3.3/docs/custom_logo.png
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      408 2022-09-27 15:01:02.000000 snews_pt-1.3.3/docs/index.rst
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)    17706 2022-05-20 12:43:49.000000 snews_pt-1.3.3/docs/snews_logo.png
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1107 2022-05-20 12:43:49.000000 snews_pt-1.3.3/docs/subscribed_messages.json
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-05-12 08:19:32.000000 snews_pt-1.3.3/docs/user/
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      258 2022-05-20 12:43:49.000000 snews_pt-1.3.3/docs/user/architecture.rst
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     5119 2022-05-20 13:27:18.000000 snews_pt-1.3.3/docs/user/command_line_interface.md
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     4242 2022-09-29 07:36:14.000000 snews_pt-1.3.3/docs/user/firedrills.md
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      840 2022-05-20 12:43:49.000000 snews_pt-1.3.3/docs/user/installation.rst
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1603 2023-03-30 14:38:00.000000 snews_pt-1.3.3/docs/user/message_schema.md
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1259 2022-05-20 12:43:49.000000 snews_pt-1.3.3/docs/user/protocol.rst
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1258 2023-03-30 14:38:00.000000 snews_pt-1.3.3/docs/user/publishing_protocols.md
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     8746 2022-05-20 13:27:18.000000 snews_pt-1.3.3/docs/user/quickstart.md
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     4786 2022-12-01 10:17:24.000000 snews_pt-1.3.3/examples.ipynb
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)    34654 2023-05-08 14:52:18.000000 snews_pt-1.3.3/firedrill.ipynb
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)   108013 2022-05-20 12:43:49.000000 snews_pt-1.3.3/img.png
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-05-12 08:19:32.000000 snews_pt-1.3.3/logs/
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        2 2022-08-01 20:52:31.000000 snews_pt-1.3.3/logs/.gitignore
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      440 2023-04-21 11:47:54.000000 snews_pt-1.3.3/requirements.txt
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      169 2023-05-12 08:19:34.000000 snews_pt-1.3.3/setup.cfg
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2419 2023-03-30 14:38:00.000000 snews_pt-1.3.3/setup.py
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-05-12 08:19:33.000000 snews_pt-1.3.3/snews_pt/
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      747 2022-09-27 12:03:30.000000 snews_pt-1.3.3/snews_pt/__init__.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     9898 2023-05-08 13:02:05.000000 snews_pt-1.3.3/snews_pt/__main__.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)       19 2023-04-21 11:47:54.000000 snews_pt-1.3.3/snews_pt/_version.py
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-05-12 08:19:33.000000 snews_pt-1.3.3/snews_pt/auxiliary/
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1523 2022-05-20 13:27:18.000000 snews_pt-1.3.3/snews_pt/auxiliary/custom_script.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1565 2022-11-18 16:58:48.000000 snews_pt-1.3.3/snews_pt/auxiliary/detector_properties.json
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2435 2023-03-30 14:38:00.000000 snews_pt-1.3.3/snews_pt/auxiliary/make_scenarios.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     3543 2023-03-30 14:38:00.000000 snews_pt-1.3.3/snews_pt/auxiliary/scenarios.json
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      619 2023-05-08 13:02:06.000000 snews_pt-1.3.3/snews_pt/auxiliary/test-config.env
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2267 2023-03-30 14:38:00.000000 snews_pt-1.3.3/snews_pt/auxiliary/try_scenarios.py
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-05-12 08:19:33.000000 snews_pt-1.3.3/snews_pt/core/
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2022-09-27 12:03:31.000000 snews_pt-1.3.3/snews_pt/core/__init__.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1314 2022-09-27 12:03:31.000000 snews_pt-1.3.3/snews_pt/core/logging.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     4011 2023-04-21 11:47:54.000000 snews_pt-1.3.3/snews_pt/message_schema.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     6361 2023-05-08 13:02:05.000000 snews_pt-1.3.3/snews_pt/remote_commands.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     9366 2023-04-21 11:47:54.000000 snews_pt-1.3.3/snews_pt/snews_format_checker.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)    11921 2023-04-21 11:47:54.000000 snews_pt-1.3.3/snews_pt/snews_pt_utils.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     9081 2023-04-21 11:47:54.000000 snews_pt-1.3.3/snews_pt/snews_pub.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     5042 2023-04-21 11:47:54.000000 snews_pt-1.3.3/snews_pt/snews_sub.py
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-05-12 08:19:34.000000 snews_pt-1.3.3/snews_pt/test/
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      272 2022-11-18 16:58:49.000000 snews_pt-1.3.3/snews_pt/test/example_coincidence_tier_message.json
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      483 2022-11-18 16:58:49.000000 snews_pt-1.3.3/snews_pt/test/example_combined_message.json
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      182 2022-11-18 16:58:49.000000 snews_pt-1.3.3/snews_pt/test/example_heartbeat_message.json
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      318 2022-11-18 16:58:49.000000 snews_pt-1.3.3/snews_pt/test/example_significance_tier_message.json
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      328 2022-11-18 16:58:49.000000 snews_pt-1.3.3/snews_pt/test/example_timing_tier_message.json
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1161 2022-05-20 13:27:19.000000 snews_pt-1.3.3/snews_pt/test/random_plugin.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1689 2023-04-21 11:47:54.000000 snews_pt-1.3.3/snews_pt/test/test_coincidence_tier.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      239 2022-05-20 13:27:19.000000 snews_pt-1.3.3/snews_pt/test/test_install.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1705 2022-11-18 16:58:49.000000 snews_pt-1.3.3/snews_pt/test/test_old_crashes.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      842 2022-11-18 16:58:49.000000 snews_pt-1.3.3/snews_pt/test/test_plugin.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1288 2023-03-30 14:38:00.000000 snews_pt-1.3.3/snews_pt/test/test_retraction.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2384 2023-04-21 11:47:54.000000 snews_pt-1.3.3/snews_pt/test/test_significance_tier.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      643 2022-11-18 16:58:49.000000 snews_pt-1.3.3/snews_pt/test/test_subscribe.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1820 2023-04-21 11:47:54.000000 snews_pt-1.3.3/snews_pt/test/test_timing_tier.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     3880 2023-04-21 11:47:54.000000 snews_pt-1.3.3/snews_pt/tier_decider.py
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-05-12 08:19:33.000000 snews_pt-1.3.3/snews_pt.egg-info/
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)    10037 2023-05-12 08:19:27.000000 snews_pt-1.3.3/snews_pt.egg-info/PKG-INFO
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2398 2023-05-12 08:19:31.000000 snews_pt-1.3.3/snews_pt.egg-info/SOURCES.txt
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        1 2023-05-12 08:19:27.000000 snews_pt-1.3.3/snews_pt.egg-info/dependency_links.txt
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)       52 2023-05-12 08:19:27.000000 snews_pt-1.3.3/snews_pt.egg-info/entry_points.txt
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        1 2022-05-20 13:36:30.000000 snews_pt-1.3.3/snews_pt.egg-info/not-zip-safe
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)       47 2023-05-12 08:19:27.000000 snews_pt-1.3.3/snews_pt.egg-info/pbr.json
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      417 2023-05-12 08:19:27.000000 snews_pt-1.3.3/snews_pt.egg-info/requires.txt
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        9 2023-05-12 08:19:27.000000 snews_pt-1.3.3/snews_pt.egg-info/top_level.txt
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2024-05-10 12:59:55.214353 snews_pt-1.3.4/
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2024-05-10 12:59:52.028236 snews_pt-1.3.4/.github/
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2024-05-10 12:59:52.479787 snews_pt-1.3.4/.github/workflows/
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1882 2024-04-08 12:47:31.000000 snews_pt-1.3.4/.github/workflows/mac12-py311-312.yml
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1882 2024-04-08 12:47:31.000000 snews_pt-1.3.4/.github/workflows/mac13-py311-312.yml
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1884 2024-04-08 12:47:31.000000 snews_pt-1.3.4/.github/workflows/mac14-py311-312.yml
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2488 2024-04-08 12:47:31.000000 snews_pt-1.3.4/.github/workflows/ubuntu22-py311-312.yml
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      598 2024-04-08 11:54:25.000000 snews_pt-1.3.4/.readthedocs.yaml
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      660 2024-05-10 12:59:42.000000 snews_pt-1.3.4/AUTHORS
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)    19861 2024-05-10 12:59:41.000000 snews_pt-1.3.4/ChangeLog
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1657 2023-06-02 15:02:47.000000 snews_pt-1.3.4/LICENSE
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     5726 2024-05-10 12:59:55.199824 snews_pt-1.3.4/PKG-INFO
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     4465 2023-06-02 15:03:09.000000 snews_pt-1.3.4/README.md
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2024-05-10 12:59:52.827771 snews_pt-1.3.4/docs/
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      623 2022-05-20 12:43:48.000000 snews_pt-1.3.4/docs/Makefile
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      205 2022-05-20 12:43:48.000000 snews_pt-1.3.4/docs/README.md
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2024-05-10 12:59:52.047233 snews_pt-1.3.4/docs/_static/
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2024-05-10 12:59:52.861765 snews_pt-1.3.4/docs/_static/css/
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      616 2022-05-20 12:43:48.000000 snews_pt-1.3.4/docs/_static/css/my_theme.css
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2024-05-10 12:59:52.896764 snews_pt-1.3.4/docs/_templates/
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)       60 2022-05-20 12:43:48.000000 snews_pt-1.3.4/docs/_templates/layout.html
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2024-05-10 12:59:53.051764 snews_pt-1.3.4/docs/api/
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      148 2022-05-20 12:43:48.000000 snews_pt-1.3.4/docs/api/api.rst
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      129 2022-05-20 13:27:18.000000 snews_pt-1.3.4/docs/api/message_schema.rst
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      123 2022-05-20 13:27:18.000000 snews_pt-1.3.4/docs/api/snews_pt_utils.rst
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      111 2022-05-20 13:27:18.000000 snews_pt-1.3.4/docs/api/snews_pub.rst
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      114 2022-05-20 13:27:18.000000 snews_pt-1.3.4/docs/api/snews_sub.rst
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     6080 2022-05-20 13:27:18.000000 snews_pt-1.3.4/docs/cli_docs.md
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      535 2022-05-20 12:43:48.000000 snews_pt-1.3.4/docs/cli_help.txt
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     4472 2024-04-08 11:54:25.000000 snews_pt-1.3.4/docs/conf.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)   139863 2022-04-28 07:02:44.000000 snews_pt-1.3.4/docs/custom_logo.png
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)   132449 2023-06-02 15:03:09.000000 snews_pt-1.3.4/docs/example_publishing.png
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      472 2023-06-02 15:03:09.000000 snews_pt-1.3.4/docs/index.rst
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)   270035 2023-06-02 15:03:09.000000 snews_pt-1.3.4/docs/required_permissions.png
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      457 2024-04-08 11:54:25.000000 snews_pt-1.3.4/docs/requirements.txt
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)    17706 2022-05-20 12:43:49.000000 snews_pt-1.3.4/docs/snews_logo.png
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1107 2022-05-20 12:43:49.000000 snews_pt-1.3.4/docs/subscribed_messages.json
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)    35771 2023-06-02 15:03:09.000000 snews_pt-1.3.4/docs/test-connection-screenshot.png
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2024-05-10 12:59:53.343770 snews_pt-1.3.4/docs/user/
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     6719 2023-12-19 10:37:38.000000 snews_pt-1.3.4/docs/user/command_line_interface.md
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     4596 2023-12-08 12:58:06.000000 snews_pt-1.3.4/docs/user/firedrills.md
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      475 2023-06-02 15:03:09.000000 snews_pt-1.3.4/docs/user/installation.md
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     5564 2023-12-08 12:58:06.000000 snews_pt-1.3.4/docs/user/publishing_protocols.md
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     6356 2023-06-02 15:03:09.000000 snews_pt-1.3.4/docs/user/quickstart.md
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     4450 2023-06-02 15:03:09.000000 snews_pt-1.3.4/docs/user/remote_commands.md
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2856 2023-06-02 15:03:09.000000 snews_pt-1.3.4/docs/user/subscribing.md
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)   370285 2024-05-10 12:33:03.000000 snews_pt-1.3.4/examples.ipynb
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)    45832 2024-05-10 12:33:04.000000 snews_pt-1.3.4/firedrill.ipynb
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2024-05-10 12:59:53.399768 snews_pt-1.3.4/logs/
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        2 2022-08-01 20:52:31.000000 snews_pt-1.3.4/logs/.gitignore
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      123 2024-04-08 12:47:31.000000 snews_pt-1.3.4/requirements.txt
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      169 2024-05-10 12:59:55.246890 snews_pt-1.3.4/setup.cfg
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2465 2024-05-07 13:48:44.000000 snews_pt-1.3.4/setup.py
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2024-05-10 12:59:53.788772 snews_pt-1.3.4/snews_pt/
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      747 2022-09-27 12:03:30.000000 snews_pt-1.3.4/snews_pt/__init__.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     9720 2024-04-08 12:31:39.000000 snews_pt-1.3.4/snews_pt/__main__.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)       19 2023-12-19 10:37:38.000000 snews_pt-1.3.4/snews_pt/_version.py
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2024-05-10 12:59:54.364970 snews_pt-1.3.4/snews_pt/auxiliary/
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1523 2022-05-20 13:27:18.000000 snews_pt-1.3.4/snews_pt/auxiliary/custom_script.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1565 2022-11-18 16:58:48.000000 snews_pt-1.3.4/snews_pt/auxiliary/detector_properties.json
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2435 2023-03-30 14:38:00.000000 snews_pt-1.3.4/snews_pt/auxiliary/make_scenarios.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     3543 2023-03-30 14:38:00.000000 snews_pt-1.3.4/snews_pt/auxiliary/scenarios.json
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      640 2024-05-10 12:33:03.000000 snews_pt-1.3.4/snews_pt/auxiliary/test-config.env
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2264 2023-12-08 12:58:06.000000 snews_pt-1.3.4/snews_pt/auxiliary/try_scenarios.py
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2024-05-10 12:59:54.442968 snews_pt-1.3.4/snews_pt/core/
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2022-09-27 12:03:31.000000 snews_pt-1.3.4/snews_pt/core/__init__.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1314 2022-09-27 12:03:31.000000 snews_pt-1.3.4/snews_pt/core/logging.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)    23925 2024-05-10 12:32:59.000000 snews_pt-1.3.4/snews_pt/messages.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     7601 2023-12-08 12:58:06.000000 snews_pt-1.3.4/snews_pt/remote_commands.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)    11338 2024-04-08 11:54:25.000000 snews_pt-1.3.4/snews_pt/snews_format_checker.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     6805 2023-12-08 12:58:07.000000 snews_pt-1.3.4/snews_pt/snews_pt_utils.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     5573 2023-12-19 10:37:38.000000 snews_pt-1.3.4/snews_pt/snews_sub.py
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2024-05-10 12:59:55.077819 snews_pt-1.3.4/snews_pt/test/
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      272 2022-11-18 16:58:49.000000 snews_pt-1.3.4/snews_pt/test/example_coincidence_tier_message.json
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      483 2022-11-18 16:58:49.000000 snews_pt-1.3.4/snews_pt/test/example_combined_message.json
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      182 2022-11-18 16:58:49.000000 snews_pt-1.3.4/snews_pt/test/example_heartbeat_message.json
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      318 2022-11-18 16:58:49.000000 snews_pt-1.3.4/snews_pt/test/example_significance_tier_message.json
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      328 2022-11-18 16:58:49.000000 snews_pt-1.3.4/snews_pt/test/example_timing_tier_message.json
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1161 2022-05-20 13:27:19.000000 snews_pt-1.3.4/snews_pt/test/random_plugin.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1770 2024-04-08 12:31:39.000000 snews_pt-1.3.4/snews_pt/test/test_coincidence_tier.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      338 2023-12-08 12:58:07.000000 snews_pt-1.3.4/snews_pt/test/test_connection_to_server.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1600 2024-04-08 12:31:39.000000 snews_pt-1.3.4/snews_pt/test/test_heartbeat.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      239 2022-05-20 13:27:19.000000 snews_pt-1.3.4/snews_pt/test/test_install.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1532 2024-04-08 11:54:25.000000 snews_pt-1.3.4/snews_pt/test/test_old_crashes.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      842 2022-11-18 16:58:49.000000 snews_pt-1.3.4/snews_pt/test/test_plugin.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2442 2024-04-08 12:31:39.000000 snews_pt-1.3.4/snews_pt/test/test_retraction.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     3227 2024-04-08 12:31:39.000000 snews_pt-1.3.4/snews_pt/test/test_significance_tier.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      643 2023-12-12 08:51:14.000000 snews_pt-1.3.4/snews_pt/test/test_subscribe.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     4036 2024-05-10 12:32:59.000000 snews_pt-1.3.4/snews_pt/test/test_timing_tier.py
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2024-05-10 12:59:55.164819 snews_pt-1.3.4/snews_pt.egg-info/
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     5726 2024-05-10 12:59:42.000000 snews_pt-1.3.4/snews_pt.egg-info/PKG-INFO
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2282 2024-05-10 12:59:52.000000 snews_pt-1.3.4/snews_pt.egg-info/SOURCES.txt
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        1 2024-05-10 12:59:42.000000 snews_pt-1.3.4/snews_pt.egg-info/dependency_links.txt
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)       52 2024-05-10 12:59:42.000000 snews_pt-1.3.4/snews_pt.egg-info/entry_points.txt
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        1 2022-05-20 13:36:30.000000 snews_pt-1.3.4/snews_pt.egg-info/not-zip-safe
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)       47 2024-05-10 12:59:43.000000 snews_pt-1.3.4/snews_pt.egg-info/pbr.json
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      115 2024-05-10 12:59:42.000000 snews_pt-1.3.4/snews_pt.egg-info/requires.txt
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        9 2024-05-10 12:59:42.000000 snews_pt-1.3.4/snews_pt.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `snews_pt-1.3.3/.github/workflows/mac10-py37.yml` & `snews_pt-1.3.4/.github/workflows/mac12-py311-312.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-name: Mac 10 Python 3.7
+name: Mac 12 Python 3.11-12
 
 on:
   push:
     branches: [ smolsky/testing ]
 
 jobs:
   build:
-    runs-on: macos-10.15
+    runs-on: macos-12
     strategy:
       # Add a list of python versions we want to use for testing.
       matrix:
-        python-version: ['3.7']
+        python-version: ['3.11', '3.12']
 
     steps:
-    - uses: actions/checkout@v2
-    
+    - uses: actions/checkout@v4
+
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
-    
+
     - name: Lint with flake8
       run: |
         # stop the build if there are Python syntax errors or undefined names
         pip install flake8
         flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
         # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
         flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
@@ -61,8 +61,8 @@
 
     - name: Check version
       run: snews_pt --version
 
     - name: Run pytest
       run: |
         pip install pytest
-        pytest
+        pytest
```

### Comparing `snews_pt-1.3.3/.github/workflows/mac10-py38.yml` & `snews_pt-1.3.4/.github/workflows/mac13-py311-312.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-name: Mac 10 Python 3.8
+name: Mac 13 Python 3.11-12
 
 on:
   push:
     branches: [ smolsky/testing ]
 
 jobs:
   build:
-    runs-on: macos-10.15
+    runs-on: macos-13
     strategy:
       # Add a list of python versions we want to use for testing.
       matrix:
-        python-version: ['3.8']
+        python-version: ['3.11', '3.12']
 
     steps:
-    - uses: actions/checkout@v2
-    
+    - uses: actions/checkout@v4
+
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
-    
+
     - name: Lint with flake8
       run: |
         # stop the build if there are Python syntax errors or undefined names
         pip install flake8
         flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
         # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
         flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
@@ -61,8 +61,8 @@
 
     - name: Check version
       run: snews_pt --version
 
     - name: Run pytest
       run: |
         pip install pytest
-        pytest
+        pytest
```

### Comparing `snews_pt-1.3.3/.github/workflows/mac11-py310.yml` & `snews_pt-1.3.4/.github/workflows/mac14-py311-312.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-name: Mac 11 Python 3.10
+name: Mac 14
+ Python 3.11-12
 
 on:
   push:
     branches: [ smolsky/testing ]
 
 jobs:
   build:
-    runs-on: macos-11
+    runs-on: macos-14
     strategy:
       # Add a list of python versions we want to use for testing.
       matrix:
-        python-version: ['3.10']
+        python-version: ['3.11', '3.12']
 
     steps:
-    - uses: actions/checkout@v2
-    
+    - uses: actions/checkout@v4
+
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
-    
+
     - name: Lint with flake8
       run: |
         # stop the build if there are Python syntax errors or undefined names
         pip install flake8
         flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
         # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
         flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
@@ -61,8 +62,8 @@
 
     - name: Check version
       run: snews_pt --version
 
     - name: Run pytest
       run: |
         pip install pytest
-        pytest
+        pytest
```

### Comparing `snews_pt-1.3.3/.github/workflows/ubuntu20-py310.yml` & `snews_pt-1.3.4/.github/workflows/ubuntu22-py311-312.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,53 +1,54 @@
-name: Ubuntu 20.04 Python 3.10
+name: Ubuntu 22.04 Python 3.11-12
 
 on:
   push:
-    branches: 
+    branches:
       - smolsky/testing
       - main
-      
+
   pull_request:
     branches:
       - main
 
 jobs:
   # Copied from snewpy. ;)
   build:
     # The type of runner that the job will run on.
     runs-on: ubuntu-latest
     strategy:
       # Add a list of python versions we want to use for testing.
       matrix:
-        python-version: ['3.10']
+        python-version: ["3.11", "3.12"]
 
     steps:
-    - uses: actions/checkout@v2
-    
+    - uses: actions/checkout@v4
+
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
-      
+
     - name: Check python version
       run: python --version
 
     - name: Lint with flake8
       run: |
         # stop the build if there are Python syntax errors or undefined names
         pip install flake8
         flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
         # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
         flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
 
     - name: Install hop-client
       run: |
-        wget https://files.pythonhosted.org/packages/de/a2/1f663c824b7e6ac139110005888cda7e1aea74e3bb8a57d774a00a1802f5/hop-client-0.5.0.tar.gz
-        tar -xzf hop-client-0.5.0.tar.gz
-        cd hop-client-0.5.0
+        pip install install setuptools wheel
+        wget https://files.pythonhosted.org/packages/64/d1/108cea042128c7ea7790e15e12e3e5ed595bfcf4b051c34fe1064924beba/hop-client-0.9.0.tar.gz
+        tar -xzf hop-client-0.9.0.tar.gz
+        cd hop-client-0.9.0
         python setup.py install
         cd /home/runner/work/SNEWS_Publishing_Tools/SNEWS_Publishing_Tools
 
     - name: Install requirements
       run: |
         python -m pip install --upgrade pip
         pip install wheel
@@ -64,21 +65,23 @@
         spawn hop auth add
         expect "Username:"
         send "$USERNAME\n"
         expect "Password:"
         send "$PASSWORD\n"
         expect "Hostname (may be empty):"
         send "kafka.scimma.org\n"
+        expect "Token endpoint (empty if not applicable):"
+        send "\n"
         expect eof
         HOP
         hop auth locate
 
     - name: Install snews-pt
       run:  pip install .
 
     - name: Check version
       run: snews_pt --version
 
     - name: Run pytest
       run: |
         pip install pytest
-        pytest snews_pt
+        pytest snews_pt
```

### Comparing `snews_pt-1.3.3/ChangeLog` & `snews_pt-1.3.4/ChangeLog`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,114 @@
 CHANGES
 =======
 
+v1.3.4
+------
+
+* clean a line
+* add neutrino times for time tier
+* placeholder for prod topic
+* Fix typo on setup.py
+* adjust floating implementation
+* adjust tests
+* revert firedrill fix
+* move firedrill location
+* fix machine time overwrite
+* time tier accepts floats
+* CLI fix for publish and hb
+* Modify github testing workflow configs
+* Upgrade and clean up dependencies
+* add todo for timetier
+* Fix stupid typo in YAML file
+* Modernize readthedocs version
+* Point to documentation requirements
+* Add documentation-specific requirements
+* Add default language
+* update tests
+* remove wrong-semicolon test
+* remove pandas
+* converting to numpy datetimes
+* wrong spacing
+* missing import
+* avoid TimeTier crash
+* avoid TimeTier crash
+* avoid TimeTier crash
+* Fixed iso format issue
+* minor improvement, backw compatible
+* Relaxed the setup tools, ~= -> >=
+* fix tier schema display in CLI
+* pvalues in sigtier validation
+* bump versions in tests
+* print schema also displays kwargs
+* better print tier contents
+* better print tier contents
+* update version
+* update tests
+* time tier pval validation
+* update notebook
+* update examples
+* fix detector name set reintroduce meta field add is\_test to accepted fields
+* don't set the name, just get it
+* legacy. is test no longer under meta key, but CS uses this script to check
+* set name, fetch if name has already been changed
+* check p-value range for coincidence tier + improve md repr
+* adapt to new msg construction
+* Remove Python 3.7 unit tests
+* oopsie fix
+* update notebooks
+* set name echoes only when not returned
+* turn json import into a classmethod
+* numpy requirement
+* clean-up
+* test connection returns bool
+* automated server connection test
+* remove neutrino time from time tier fields
+* fix test script
+* new heartbeat test
+* typo fix
+* fix retraction unit test
+* fix timing unit test
+* fix significance unit test
+* fix coincidence unit test
+* fetch and append machine time
+* return is\_valid true, and keep tiernames
+* convert message schema display
+* rename functions
+* is\_valid method for Time,HB, and retr tiers
+* is\_valid method for Time,HB, and retr tiers
+* check detector name in base, add SigTier is valid
+* is valid method for coinc tier
+* irrelevant fix
+* when sending avoid using other-tier keys in the meta
+* add a publisher
+* times in timing series must be checked
+* markdown representations
+* Refector message builder, enable to/from JSON
+* Test SNEWSMessageBuilder for tier message lists
+* Print schema. Rename validate function
+* Add SNEWSMessage class hierarchy
+* update docstring
+* update docstring
+* update docstring
+* update docstring
+* update docstring
+* update docstring
+* update docstring
+* minor
+* replace images
+* improve docs
+* improve docs
+* improve docs
+* improve docs
+* Add link to contributions page
+* Add BSD 3-clause license
+* Enable message output to JSON
+* add screenshots
+* start changind the docs
+
 v1.3.3
 ------
 
 * fix docstring
 * add doc
 * add patience
 * update notebook
```

### Comparing `snews_pt-1.3.3/docs/Makefile` & `snews_pt-1.3.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.3/docs/_static/css/my_theme.css` & `snews_pt-1.3.4/docs/_static/css/my_theme.css`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.3/docs/cli_docs.md` & `snews_pt-1.3.4/docs/cli_docs.md`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.3/docs/cli_help.txt` & `snews_pt-1.3.4/docs/cli_help.txt`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.3/docs/conf.py` & `snews_pt-1.3.4/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 master_doc = 'index'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = 'en'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path .
 exclude_patterns = ['_build']
 
 # The name of the Pygments (syntax highlighting) style to use.
```

### Comparing `snews_pt-1.3.3/docs/custom_logo.png` & `snews_pt-1.3.4/docs/custom_logo.png`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.3/docs/snews_logo.png` & `snews_pt-1.3.4/docs/snews_logo.png`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.3/docs/subscribed_messages.json` & `snews_pt-1.3.4/docs/subscribed_messages.json`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.3/docs/user/command_line_interface.md` & `snews_pt-1.3.4/docs/user/publishing_protocols.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,114 +1,101 @@
-# Command Line Interface (CLI)
+# Publishing Protocols
 
-It is also possible to interact with `snews_pt` through the command line. <br>
-All the commands have their short descriptions accessible via `--help` flag. 
-```bash
-(venv) User$: snews_pt --help 
-```
-```bash
-Usage: snews_pt [OPTIONS] COMMAND [ARGS]...
-  User interface for snews_pt tools
+Users from certain experiments can send their observations to SNEWS for creating a coincidence with the other incoming messages. 
+These "observation messages" are not public unless they coincide with another observation message from another experiment within 10 seconds. 
+In which case the SNEWS server triggers a "coincidence alert message" to all of its subsribers.
 
-Options:
-  --version   Show the version and exit.
-  --env TEXT  environment file containing the configurations  [default: (auxiliary/test-config.env)]
-  --help      Show this message and exit.
-
-Commands:
-  heartbeat       Publish heartbeat messages.
-  message-schema  Display the message format for `tier`, default 'all'
-  publish         Publish a message using snews_pub
-  retract         Retract N latest message
-  subscribe       Subscribe to Alert topic 
-```
-The main command `snews_pt` serves an entry point. It is also possible to set an _environment_ by passing it to this with any other command. 
-E.g. `snews_pt --env myenvfile.env subscribe` will set the variables in _myenvfile.env_  and subscribe to the _ALERT_TOPIC_ specified in this file. <br>
-By default, it uses the environment file that comes with the package.
-
----
-## Subscribing to Alert Topics
-The subscription command can be called without any arguments.
-```bash 
-(venv) User$: snews_pt subscribe 
-```
-```bash
-> You are subscribing to ALERT 
-> Broker:kafka://kafka.scimma.org/snews.alert-test
-```
----
-## Message Schemas
-`snews_pt message-schema` can tell you the required contents for each tiers. You can display the contents of a single tier by calling e.g.
-```bash
-(venv) User$: snews_pt message-schema time
-```
-In which case it displays the following
-```bash
-         >The Message Schema for TimeTier 
-_id                 :(SNEWS SETS)
-detector_name       :(SNEWS SETS)
-sent_time           :(SNEWS SETS)
-machine_time        :(User Input)
-neutrino_time       :(User Input)
-timing_series       :(User Input)  
-```
-or you can simply call `snews_pt message-schema` without any positional arguments in which case it displays all the message schemes. <br>
+Members can share information about their observation. Based on the scope of shared information different tiers can work on different aspects. 
 
----
 
-## Publishing Observation Messages
-User can publish observation messages to one of the 'CoincidenceTier', 'TimeTier', or 'SigTier'. It is also possible to publish _Heartbeat_ and _Retraction_ messages, see respective section below.
+The most basic information a detector can share is the initial neutrino time of their observation. 
+This information is used to form a **Coincidence** with other initial neutrino times acquired from other detectors. 
+The coincidences are handled within the **"Coincidence Tier"** and by the [SNEWS Coincidence System](https://github.com/SNEWS2/SNEWS_Coincidence_System).
 
-To publish one or more tier user can request arbitrary number of tiers in one line
-```bash
-(venv) User$: snews_pt publish coincidence time time significance s
-```
-The `publish` tool takes all the request and queries known aliases e.g. `s` is accepted as `SignificanceTier`, and returns a list of unique requested tiers.<br>
-Without any additional _options_ this by default publishes a dummy observation to each of the requested tiers with their required data fields.
+If further information is shared e.g. combined sensitivities can be computed (**"Significance Tier"**) by using the individual neutrino events, or 
+the location of the supernova can be triangulated (**"Time Tier"**).
 
-For a more realistic case, we would want to submit a message that is saved by our experiment as a _json_ file. This can be passed with a `--file` (or `-f`) flag.
-```bash
-(venv) User$: snews_pt publish coincidence -f my_coincidence_message.json
-```
-There are several dummy examples [here](../test/) that can be used as a reference. In principle, SNEWS only accept specific fields (see `snews_pt message-schema`), however the tools does not fail if you provide additional arguments. It kindly warns you about them and publishes the remaining parts.
+The user can share as much information as they desire with one simple function call. The predetermined fields 
+sets the "Tier" and any additional information is passed under `meta` field.
 
-Try publishing the following file which contains an `extra_key` field.
-```bash
-(venv) User$: snews_pt publish coincidence -f snews_pt/test/example_coincidence_tier_message.json
+The user can use `SNEWSTiersPublisher` to create observation message(s) and send them to snews.
+
+```python
+from snews_pt.messages import SNEWSMessageBuilder
+
+messages = SNEWSMessageBuilder(neutrino_time="2022-02-28T04:31:08.678999")
+messages.send_messages()
 ```
+User can also investigate their messages before sending it to SNEWS. The `SNEWSTiersPublisher` creates an object which contains 
+the generated and formatted messages. It can also tell you what "Tiers" are selected based on the input that is given. 
 
-It should give the following
+The example above shows the minimal working example. Assuming that the detector name has already been set by `snews_pt.snews_pt_utils.set_name()` function
+only passing the neutrino time in ISO-format creates a message for the Coincidence Tier which can be sent to snews easily. 
+Similarly, if you have a JSON file that contains the same information in the correct format, this can also be passed to snews using command line interface;
 ```bash
-Requested tiers are;
-                > CoincidenceTier
-Publishing to CoincidenceTier;
-extra_key not a valid key for CoincidenceTier
----------------------------------------------------------
-_id                 :0_CoincidenceTier_22/01/01_20:19:06:356690
-detector_name       :TEST
-sent_time           :22/01/01 20:19:06
-machine_time        :test machine time
-neutrino_time       :test nu time
-p_value             :test p-values 
+snews_pt publish myjsonfile.json
 ```
-----
 
-## Publishing Heartbeat messages
+### Things to note
 
-`snews_pt heartbeat`  can be used to publish heartbeat messages. It is up to the user to invoke this function with a desired frequency, however it is recommended to publish heartbeats consistently and with couple of minutes intervals.
+For your messages to pass your name has to be set. If you haven't done so, `snews_pt` will raise a warning. 
+Unless you are sending messages with a known name they will not be read by the server.
 
-The `heartbeat` command takes a `status` argument which can either be 'ON' or 'OFF'. 
-Additionaly, `machine_time` can be passed using `--machine_time` (`-mt`) flag as a string. Each heartbeat message is appended with a `sent_time`, if machine time is also provided, the latency can be tracked.
+Similarly, the times are always in ISO-format (``"%Y-%m-%dT%H:%M:%S.%f"``) otherwise, the tools will raise an error.
 
-```bash
-(venv) User$: snews_pt heartbeat ON -mt '22/01/01 20:19:06' --verbose False
-```
----
+If you are testing, you need to pass the argument `is_test=True` otherwise, the messages that contain a neutrino time that 
+is not within the last 48 hours will be rejected. Testing allows setting times in the future or from past.
 
-## Retraction Messages
+The server runs a specific kafka topic, some topics (e.g. "OBSERVATION_TOPIC", "ALERT_TOPIC", "FIREDRILL_TOPIC") are set 
+on the environment file by default. The `snews_pt` tools can read these, but you can tell it whether you want to use the 
+firedrill topic or not by passing `firedrill_mode=True` or `firedrill_mode=False` based on which it selects either of the topics.
+
+
+### Tier Decider
+There is a `tier_decider` module that decides and generates different messages with the SNEWS format based on the input you pass.
+> if you pass `neutrino_time` the Publisher labels it as "Coincidence Tier" <br>
+> if you pass `p_values` and `t_bin_width` it is labeled as "Significance Tier Message" <br>
+> if you pass `timing_series` it is labeled as "Time Tier" <br>
+> if you pass `retract_latest` (e.g. retract_latest=1 retracts the last 1 message) it labels as "Retraction Message" <br>
+> if you pass `detector_status` it labels as "Heartbeat Message" (Notice HB doesn't require time as it stamps itself) <br>
+
+
+**Coincidence Tier**
+
+* ``neutrino_time`` need to be passed.
+    * ``neutrino_time`` must be a ``string`` with ISO format: ``"%Y-%m-%dT%H:%M:%S.%f"``
+
+**Significance Tier**
+
+* ``p_values`` needs to be passed.
+    * ``p_values`` must be a ``list (float)``.
+
+**Timing Tier**
+
+* ``p_value`` and ``timing_series`` need to be passed.
+    * ``p_val`` must be a ``float``.
+    * ``timing_series`` must be a ``list (string)``, ISO format: ``"%Y-%m-%dT%H:%M:%S.%f"``
+
+**Retraction**
+
+* ``retract_latest`` need to be passed.
+    * ``retract_latest`` must be a ``int (and >0 )``. 
+
+**Pre-SN Timing Tier**
+
+* ``is_pre_sn`` and ``timing_series`` need to be passed.
+    * ``is_pre_sn`` must be a ``bool``.
+    * ``timing_series`` must be a ``list (string)``, ISO format: ``"%Y-%m-%dT%H:%M:%S.%f"``
+
+Notice that your message can contain fields that correspond to several tiers e.g. if you have ``p_value``, ``neutrino_time``, and ``p_values`` we submit two separate messages to _Coincidence_ and _Significance_ tiers by selecting the relevant fields from your input.
+
+
+#### Example;
+
+In the example below `SNEWSTierPublisher` creates a message for "CoincidenceTier" because the `neutrino_time` is passed, and it creates 
+another message for the "Significance Tier" because the `p_values` together with the `t_bin_width` is passed. 
+
+Here the `p_val` is the p value of the detection, and it is optional. The `detector_name` can be passed manually, however, if the name is initially set, this is also not needed.
+
+<img src="../example_publishing.png" alt="Publication example" width="2000"/>
 
-It can happen that user publishes a message by accident or with wrong input. In these cases `snews_pt` allows for retraction messages. <br>
-While the specific message id can be passed, it is also possible to publish a retraction message for the last `n` number of messages. This
 
-```bash
-(venv) User$: snews_pt retract --tier Coinc -n 3 --reason 'daq failure' 
-```
```

### Comparing `snews_pt-1.3.3/docs/user/firedrills.md` & `snews_pt-1.3.4/docs/user/firedrills.md`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 More elaborate firedrills including extracting statistical information based on the active detectors by tracking the heartbeats, 
 selecting a candidate star and computing the time delays from such star to add as delays to the detectors, and trying to triangulate are work in progress.
 
 ----
 
 ## To Do's for the Detectors
+First, please follow the [Installation Guide](https://snews-publishing-tools.readthedocs.io/en/latest/user/installation.html) and 
+[**Quick Start**](https://snews-publishing-tools.readthedocs.io/en/latest/user/quickstart.html)
 
 In order to participate in the firedrills, the detectors should have the latest version of the publishing tools `snews_pt`.
 
 Each user have the option to use either the API or the CLI tools to interact with the server. 
 
 We would like to test two main interactions; **subscribing**  & **publishing** to snews.
 
@@ -38,29 +40,32 @@
   user/home$: snews_pt subscribe
    ```
 
 ### Publish
 
 - API:
     ```python
-     from snews_pt.snews_pub import SNEWSTiersPublisher
-     SNEWSTiersPublisher(detector_name='KamLAND', neutrino_time="2022-02-28T04:31:08.678999",
+     from snews_pt.messages import SNEWSMessageBuilder
+     SNEWSMessageBuilder(detector_name='KamLAND', 
+                         neutrino_time="2022-02-28T04:31:08.678999",
                          p_val=0.000007,
                          machine_time="2022-02-28T04:31:09.778859", 
                          firedrill_mode=True,
-                         ).send_to_snews()
+                         is_test=True,
+                         ).send_messages()
     ```
-  or 
+  or
   ```python
-  from snews_pt.snews_pub import SNEWSTiersPublisher
-  observation = SNEWSTiersPublisher.from_json('somejsonfile.json', 
+  from snews_pt.messages import SNEWSMessageBuilder
+  observation = SNEWSMessageBuilder.from_json('somejsonfile.json', 
                                               detector_name='XENONnT',
-                                              firedrill_mode=True, 
+                                              firedrill_mode=True,
+                                              is_test=True, 
                                               comment="This is submitted from a json file")
-  observation.send_to_snews()
+  observation.send_messages()
   ```
 Notice that `SNEWSTiersPublisher` returns an object which actually contains the decided tiers, and formatted messages. 
 One can play with this object before finally `send_to_snews()`.  
 
 - CLI
    ```bash
   user/home$: snews_pt publish --firedrill myjsonfile.json
```

### Comparing `snews_pt-1.3.3/setup.py` & `snews_pt-1.3.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import re
+
 from setuptools import find_packages, setup
 
 # read in README
 this_dir = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_dir, 'README.md'), 'rb') as f:
     long_description = f.read().decode().strip()
 
@@ -17,29 +18,28 @@
 with open('requirements.txt', 'r') as f:
     for line in f:
         if line.strip():
             install_requires.append(line.strip())
 
 extras_require = {
     'dev': [
-        'autopep8',
-        'flake8',
-        'mongomock',
-        'pytest >= 5.0, < 5.4',
-        'pytest-console-scripts',
-        'pytest-cov',
-        'pytest-mongodb',
-        'pytest-runner',
-        'twine',
-        'schedule',
+        'pytest~=8.0',
+        'pytest-console-scripts~=1.4',
+        'pytest-cov~=4.1',
+        'pytest-mongodb~=2.4',
+        'pytest-runner~=6.0',
+        'virtualenv~=20.13',
     ],
     'docs': [
-        'sphinx',
-        'sphinx_rtd_theme',
-        'sphinxcontrib-programoutput'
+        'autoapi~=2.0',
+        'myst_parser~=2.0',
+        'sphinx~=7.2',
+        'sphinx-autoapi~=3.0',
+        'sphinx-rtd-theme~=2.0',
+        'sphinxcontrib-programoutput~=0.17',
     ],
 }
 
 setup(
     name='snews_pt',
     version=version,
     description='An alert application for observing supernovas.',
@@ -56,15 +56,15 @@
 
     entry_points={
         'console_scripts': [
             'snews_pt = snews_pt.__main__:main',
         ],
     },
 
-    python_requires='>=3.7',
+    python_requires='~=3.11',
     install_requires=install_requires,
     extras_require=extras_require,
 
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
```

### Comparing `snews_pt-1.3.3/snews_pt/__init__.py` & `snews_pt-1.3.4/snews_pt/__init__.py`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.3/snews_pt/__main__.py` & `snews_pt-1.3.4/snews_pt/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,20 @@
 """ CLI for snews_pt
     
     Notes to dev team
     https://stackoverflow.com/questions/55099243/python3-dataclass-with-kwargsasterisk
 """
-from datetime import datetime
 
 from . import __version__
 from . import snews_pt_utils
-from .snews_pub import SNEWSTiersPublisher
+from .messages import SNEWSMessageBuilder
 from .snews_sub import Subscriber
-from .snews_pt_utils import coincidence_tier_data, sig_tier_data, time_tier_data
-from .snews_pt_utils import retraction_data, heartbeat_data
-from hop import Stream
 import click
 import os
-from inspect import signature
-import getpass
+
 
 @click.group(invoke_without_command=True)
 @click.version_option(__version__)
 @click.option('--env', type=str,
     default='/auxiliary/test-config.env',
     show_default='auxiliary/test-config.env',
     help='environment file containing the configurations')
@@ -50,105 +45,105 @@
 
     The topics are read from the defaults i.e. from auxiliary/test-config.env
     If no file is given it can still submit dummy messages with default values
     """
     click.clear()
     for f in file:
         if f.endswith('.json'):
-            SNEWSTiersPublisher.from_json(jsonfile=f, env_file=ctx.obj['env'], firedrill_mode=firedrill).send_to_snews()
+            SNEWSMessageBuilder.from_json(jsonfile=f, env_file=ctx.obj['env']).send_messages(firedrill_mode=firedrill)
 
         else:
             # maybe just print instead of raising
             raise TypeError(f"Expected json file with .json format! Got {f}")
 
 @main.command()
 @click.option('--firedrill/--no-firedrill', default=True, show_default='True', help='Whether to use firedrill brokers or default ones')
 @click.option('--status', '-s', type=str, default='OFF', show_default='OFF', help='Heartbeat at the time of execution')
 @click.option('--time', '-t', type=str, default=None, show_default='None', help='Machine time, format: %Y-%m-%dT%H:%M:%S.%f')
 @click.pass_context
 def heartbeat(ctx, status, time, firedrill):
     """ Send Heartbeats
-        :para status: Status of the experiment ON/OFF.
+        :param status: Status of the experiment ON/OFF.
         :param time: (optional) Machine time is appended as the time of execution
                      different time can be passed following the iso-format
     """
-    message = SNEWSTiersPublisher(detector_name=ctx.obj['DETECTOR_NAME'],
+    message = SNEWSMessageBuilder(detector_name=ctx.obj['DETECTOR_NAME'],
                                   machine_time=time,
                                   detector_status=status,
-                                  firedrill_mode=firedrill)
-    message.send_to_snews()
+    )
+    message.send_messages(firedrill_mode=firedrill)
 
 
 @main.command()
 @click.option('--plugin', '-p', type=str, default="None")
+@click.option('--outputfolder', '-o', type=str, default="None")
 @click.option('--firedrill/--no-firedrill', default=True, show_default='True', help='Whether to use firedrill brokers or default ones')
 @click.pass_context
-def subscribe(ctx, plugin, firedrill):
+def subscribe(ctx, plugin, outputfolder, firedrill):
     """ Subscribe to Alert topic
         Optionally, `plugin` script can be passed
         The message content as a single dictionary will be passed to
         this script as a positional argument.
         dictionary follows the snews_alert message schema
 
     """
+    outputfolder = None if type(outputfolder)==type(None) else outputfolder
     sub = Subscriber(ctx.obj['env'], firedrill_mode=firedrill)
     try:
         if plugin != "None":
             print(f"Redirecting output to {plugin}")
-            for saved_json in sub.subscribe_and_redirect_alert():
+            for saved_json in sub.subscribe_and_redirect_alert(outputfolder=outputfolder):
                 os.system(f"python {plugin} {saved_json}")
         else:
-            sub.subscribe()
+            sub.subscribe(outputfolder=outputfolder)
     except KeyboardInterrupt:
         pass
 
-
 @main.command()
 @click.argument('requested_tier', nargs=-1)
 @click.pass_context
 def message_schema(ctx, requested_tier):
     """ Display the message format for `tier` if 'all'
         displays everything
-
     """
-    detector = ctx.obj['DETECTOR_NAME']
-    detector_str = click.style(detector, fg='yellow')
-    tier_data_pairs = {'CoincidenceTier': (coincidence_tier_data, 'neutrino_time'),
-                       'SigTier': (sig_tier_data, 'p_values'),
-                       'TimeTier': (time_tier_data, 'timing_series'),
-                       'FalseOBS': (retraction_data, 'retract_latest'),
-                       'Heartbeat': (heartbeat_data, 'detector_status')}
+    from .messages import SNEWSHeartbeatMessage, SNEWSTimingTierMessage, SNEWSSignificanceTierMessage, \
+        SNEWSCoincidenceTierMessage, SNEWSRetractionMessage, SNEWSMessage
+
+    tier_data_pairs = {'CoincidenceTier': SNEWSCoincidenceTierMessage,
+                       'SigTier': SNEWSSignificanceTierMessage,
+                       'TimeTier': SNEWSTimingTierMessage,
+                       'FalseOBS': SNEWSRetractionMessage,
+                       'Heartbeat': SNEWSHeartbeatMessage,}
 
     if len(requested_tier)>1:
         tier = []
         for t in requested_tier:
             tier.append(snews_pt_utils._check_aliases(t))
     else:
         if requested_tier[0].lower()=='all':
             # display all
             tier = list(tier_data_pairs.keys())
         else:
             # check for aliases e.g. coinc = coincidence = CoinCideNceTier
-            tier = snews_pt_utils._check_aliases(requested_tier[0])
+            tier = list(snews_pt_utils._check_aliases(requested_tier[0]))
 
+    basefields = SNEWSMessage.basefields
     for t in tier:
-        tier_keys = list(signature(tier_data_pairs[t][0]).parameters.keys())
-        tier_keys.pop(tier_keys.index('meta'))
-        must_key = tier_data_pairs[t][1]
-        click.secho(f'\t >The Message Schema for {t}', bg='white', fg='blue')
-        click.secho(f"{'_id':<20s}:(SNEWS SETS)", fg='bright_red')
-        click.secho(f"{'schema_version':<20s}:(SNEWS SETS)", fg='bright_red')
-        click.echo(click.style(f"{'detector_name':<20s}:(FETCHED FROM ENV {detector_str})", fg='red'))
-        for key in tier_keys:
-            if key == must_key:
-                click.secho(f'{key:<20s}:(User Input*)', fg='bright_cyan')
+        TierMessage = tier_data_pairs[t]
+        fields = TierMessage.fields
+        reqfields = TierMessage.reqfields
+        click.secho(f'Message schema for {t}', bg='white', fg='blue')
+        for f in fields:
+            if f in basefields:
+                click.secho(f'{f:<20s} : (SET AUTOMATICALLY)', fg='bright_red')
+            elif f in reqfields:
+                click.secho(f'{f:<20s} : (REQUIRED USER INPUT)', fg='bright_blue')
             else:
-                click.secho(f'{key:<20s}:(User Input)', fg='bright_cyan')
-        click.secho(f"{'**kwargs':<20s}:(APPENDED AS 'META')\n", fg='red')
-        
+                click.secho(f'{f:<20s} : (USER INPUT)', fg='bright_cyan')
+        click.secho(f'{"**kwargs":<20s} : (GROUPED AS META)', fg='bright_green')
 
 @main.command()
 @click.option('--firedrill/--no-firedrill', default=True, show_default='True', help='Whether to use firedrill brokers or default ones')
 def run_scenarios(firedrill):
     """
     """
     base = os.path.dirname(os.path.realpath(__file__))
```

### Comparing `snews_pt-1.3.3/snews_pt/auxiliary/custom_script.py` & `snews_pt-1.3.4/snews_pt/auxiliary/custom_script.py`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.3/snews_pt/auxiliary/detector_properties.json` & `snews_pt-1.3.4/snews_pt/auxiliary/detector_properties.json`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.3/snews_pt/auxiliary/make_scenarios.py` & `snews_pt-1.3.4/snews_pt/auxiliary/make_scenarios.py`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.3/snews_pt/auxiliary/scenarios.json` & `snews_pt-1.3.4/snews_pt/auxiliary/scenarios.json`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.3/snews_pt/auxiliary/test-config.env` & `snews_pt-1.3.4/snews_pt/auxiliary/test-config.env`

 * *Files 2% similar despite different names*

```diff
@@ -10,11 +10,12 @@
 COINCIDENCE_THRESHOLD=10
 MSG_EXPIRATION=120
 
 HOP_BROKER="kafka.scimma.org"
 
 OBSERVATION_TOPIC="kafka://${HOP_BROKER}/snews.experiments-test"
 ALERT_TOPIC="kafka://${HOP_BROKER}/snews.alert-test"
+PRODUCTION_TOPIC=""
 
 FIREDRILL_OBSERVATION_TOPIC="kafka://${HOP_BROKER}/snews.experiments-firedrill"
 FIREDRILL_ALERT_TOPIC="kafka://${HOP_BROKER}/snews.alert-firedrill"
 CONNECTION_TEST_TOPIC="kafka://${HOP_BROKER}/snews.connection-testing"
```

### Comparing `snews_pt-1.3.3/snews_pt/auxiliary/try_scenarios.py` & `snews_pt-1.3.4/snews_pt/auxiliary/try_scenarios.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,142 +1,142 @@
 00000000: 0d0a 696d 706f 7274 206a 736f 6e2c 2063  ..import json, c
 00000010: 6c69 636b 2c20 7469 6d65 2c20 7379 730d  lick, time, sys.
 00000020: 0a66 726f 6d20 6f73 2069 6d70 6f72 7420  .from os import 
 00000030: 7061 7468 2061 7320 6f73 700d 0a66 726f  path as osp..fro
-00000040: 6d20 736e 6577 735f 7074 2e73 6e65 7773  m snews_pt.snews
-00000050: 5f70 7562 2069 6d70 6f72 7420 534e 4557  _pub import SNEW
-00000060: 5354 6965 7273 5075 626c 6973 6865 722c  STiersPublisher,
-00000070: 2050 7562 6c69 7368 6572 0d0a 6664 5f6d   Publisher..fd_m
-00000080: 6f64 6520 3d20 5472 7565 2069 6620 7379  ode = True if sy
-00000090: 732e 6172 6776 5b31 5d2e 6c6f 7765 7228  s.argv[1].lower(
-000000a0: 2920 3d3d 2022 7472 7565 2220 656c 7365  ) == "true" else
-000000b0: 2046 616c 7365 0d0a 0d0a 7769 7468 206f   False....with o
-000000c0: 7065 6e28 6f73 702e 6a6f 696e 286f 7370  pen(osp.join(osp
-000000d0: 2e64 6972 6e61 6d65 285f 5f66 696c 655f  .dirname(__file_
-000000e0: 5f29 2c20 2273 6365 6e61 7269 6f73 2e6a  _), "scenarios.j
-000000f0: 736f 6e22 2929 2061 7320 6a73 6f6e 5f66  son")) as json_f
-00000100: 696c 653a 0d0a 2020 2020 6461 7461 203d  ile:..    data =
-00000110: 206a 736f 6e2e 6c6f 6164 286a 736f 6e5f   json.load(json_
-00000120: 6669 6c65 290d 0a0d 0a74 7279 3a0d 0a20  file)....try:.. 
-00000130: 2020 2069 6d70 6f72 7420 696e 7175 6972     import inquir
-00000140: 6572 0d0a 2020 2020 7175 6573 7469 6f6e  er..    question
-00000150: 7320 3d20 5b0d 0a20 2020 2069 6e71 7569  s = [..    inqui
-00000160: 7265 722e 4368 6563 6b62 6f78 2827 7363  rer.Checkbox('sc
-00000170: 656e 6172 696f 7327 2c0d 0a20 2020 2020  enarios',..     
-00000180: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00000190: 6573 7361 6765 3d63 6c69 636b 2e73 7479  essage=click.sty
-000001a0: 6c65 2822 2057 6869 6368 2073 6365 6e61  le(" Which scena
-000001b0: 7269 6f28 7329 2077 6f75 6c64 2079 6f75  rio(s) would you
-000001c0: 206c 696b 6520 746f 2072 756e 206e 6578   like to run nex
-000001d0: 743f 222c 2062 673d 2779 656c 6c6f 7727  t?", bg='yellow'
-000001e0: 2c20 626f 6c64 3d54 7275 6529 2c0d 0a20  , bold=True),.. 
+00000040: 6d20 736e 6577 735f 7074 2e6d 6573 7361  m snews_pt.messa
+00000050: 6765 7320 696d 706f 7274 2053 4e45 5753  ges import SNEWS
+00000060: 4d65 7373 6167 6542 7569 6c64 6572 2c20  MessageBuilder, 
+00000070: 5075 626c 6973 6865 720d 0a66 645f 6d6f  Publisher..fd_mo
+00000080: 6465 203d 2054 7275 6520 6966 2073 7973  de = True if sys
+00000090: 2e61 7267 765b 315d 2e6c 6f77 6572 2829  .argv[1].lower()
+000000a0: 203d 3d20 2274 7275 6522 2065 6c73 6520   == "true" else 
+000000b0: 4661 6c73 650d 0a0d 0a77 6974 6820 6f70  False....with op
+000000c0: 656e 286f 7370 2e6a 6f69 6e28 6f73 702e  en(osp.join(osp.
+000000d0: 6469 726e 616d 6528 5f5f 6669 6c65 5f5f  dirname(__file__
+000000e0: 292c 2022 7363 656e 6172 696f 732e 6a73  ), "scenarios.js
+000000f0: 6f6e 2229 2920 6173 206a 736f 6e5f 6669  on")) as json_fi
+00000100: 6c65 3a0d 0a20 2020 2064 6174 6120 3d20  le:..    data = 
+00000110: 6a73 6f6e 2e6c 6f61 6428 6a73 6f6e 5f66  json.load(json_f
+00000120: 696c 6529 0d0a 0d0a 7472 793a 0d0a 2020  ile)....try:..  
+00000130: 2020 696d 706f 7274 2069 6e71 7569 7265    import inquire
+00000140: 720d 0a20 2020 2071 7565 7374 696f 6e73  r..    questions
+00000150: 203d 205b 0d0a 2020 2020 696e 7175 6972   = [..    inquir
+00000160: 6572 2e43 6865 636b 626f 7828 2773 6365  er.Checkbox('sce
+00000170: 6e61 7269 6f73 272c 0d0a 2020 2020 2020  narios',..      
+00000180: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+00000190: 7373 6167 653d 636c 6963 6b2e 7374 796c  ssage=click.styl
+000001a0: 6528 2220 5768 6963 6820 7363 656e 6172  e(" Which scenar
+000001b0: 696f 2873 2920 776f 756c 6420 796f 7520  io(s) would you 
+000001c0: 6c69 6b65 2074 6f20 7275 6e20 6e65 7874  like to run next
+000001d0: 3f22 2c20 6267 3d27 7965 6c6c 6f77 272c  ?", bg='yellow',
+000001e0: 2062 6f6c 643d 5472 7565 292c 0d0a 2020   bold=True),..  
 000001f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000200: 2020 2063 686f 6963 6573 3d6c 6973 7428     choices=list(
-00000210: 6461 7461 2e6b 6579 7328 2929 2b6c 6973  data.keys())+lis
-00000220: 7428 5b22 6669 6e69 7368 2026 2065 7869  t(["finish & exi
-00000230: 7422 2c20 2272 6573 7461 7274 2063 6163  t", "restart cac
-00000240: 6865 225d 292c 0d0a 2020 2020 2020 2020  he"]),..        
-00000250: 2020 2020 2020 2020 290d 0a20 2020 205d          )..    ]
-00000260: 0d0a 0d0a 2020 2020 7768 696c 6520 5472  ....    while Tr
-00000270: 7565 3a0d 0a20 2020 2020 2020 2074 7279  ue:..        try
-00000280: 3a0d 0a20 2020 2020 2020 2020 2020 2061  :..            a
-00000290: 6e73 7765 7273 203d 2069 6e71 7569 7265  nswers = inquire
-000002a0: 722e 7072 6f6d 7074 2871 7565 7374 696f  r.prompt(questio
-000002b0: 6e73 290d 0a20 2020 2020 2020 2020 2020  ns)..           
-000002c0: 2066 6f72 2073 6365 6e61 7269 6f20 696e   for scenario in
-000002d0: 2061 6e73 7765 7273 5b27 7363 656e 6172   answers['scenar
-000002e0: 696f 7327 5d3a 0d0a 2020 2020 2020 2020  ios']:..        
-000002f0: 2020 2020 2020 2020 6966 2073 6365 6e61          if scena
-00000300: 7269 6f3d 3d22 6669 6e69 7368 2026 2065  rio=="finish & e
-00000310: 7869 7422 3a0d 0a20 2020 2020 2020 2020  xit":..         
-00000320: 2020 2020 2020 2020 2020 2063 6c69 636b             click
-00000330: 2e73 6563 686f 2822 5465 726d 696e 6174  .secho("Terminat
-00000340: 696e 672e 2229 0d0a 2020 2020 2020 2020  ing.")..        
-00000350: 2020 2020 2020 2020 2020 2020 7379 732e              sys.
-00000360: 6578 6974 2829 0d0a 2020 2020 2020 2020  exit()..        
-00000370: 2020 2020 2020 2020 656c 6966 2073 6365          elif sce
-00000380: 6e61 7269 6f3d 3d22 7265 7374 6172 7420  nario=="restart 
-00000390: 6361 6368 6522 3a0d 0a20 2020 2020 2020  cache":..       
-000003a0: 2020 2020 2020 2020 2020 2020 2077 6974               wit
-000003b0: 6820 5075 626c 6973 6865 7228 6669 7265  h Publisher(fire
-000003c0: 6472 696c 6c5f 6d6f 6465 3d66 645f 6d6f  drill_mode=fd_mo
-000003d0: 6465 2c20 7665 7262 6f73 653d 4661 6c73  de, verbose=Fals
-000003e0: 6529 2061 7320 7075 623a 0d0a 2020 2020  e) as pub:..    
+00000200: 2020 6368 6f69 6365 733d 6c69 7374 2864    choices=list(d
+00000210: 6174 612e 6b65 7973 2829 292b 6c69 7374  ata.keys())+list
+00000220: 285b 2266 696e 6973 6820 2620 6578 6974  (["finish & exit
+00000230: 222c 2022 7265 7374 6172 7420 6361 6368  ", "restart cach
+00000240: 6522 5d29 2c0d 0a20 2020 2020 2020 2020  e"]),..         
+00000250: 2020 2020 2020 2029 0d0a 2020 2020 5d0d         )..    ].
+00000260: 0a0d 0a20 2020 2077 6869 6c65 2054 7275  ...    while Tru
+00000270: 653a 0d0a 2020 2020 2020 2020 7472 793a  e:..        try:
+00000280: 0d0a 2020 2020 2020 2020 2020 2020 616e  ..            an
+00000290: 7377 6572 7320 3d20 696e 7175 6972 6572  swers = inquirer
+000002a0: 2e70 726f 6d70 7428 7175 6573 7469 6f6e  .prompt(question
+000002b0: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
+000002c0: 666f 7220 7363 656e 6172 696f 2069 6e20  for scenario in 
+000002d0: 616e 7377 6572 735b 2773 6365 6e61 7269  answers['scenari
+000002e0: 6f73 275d 3a0d 0a20 2020 2020 2020 2020  os']:..         
+000002f0: 2020 2020 2020 2069 6620 7363 656e 6172         if scenar
+00000300: 696f 3d3d 2266 696e 6973 6820 2620 6578  io=="finish & ex
+00000310: 6974 223a 0d0a 2020 2020 2020 2020 2020  it":..          
+00000320: 2020 2020 2020 2020 2020 636c 6963 6b2e            click.
+00000330: 7365 6368 6f28 2254 6572 6d69 6e61 7469  secho("Terminati
+00000340: 6e67 2e22 290d 0a20 2020 2020 2020 2020  ng.")..         
+00000350: 2020 2020 2020 2020 2020 2073 7973 2e65             sys.e
+00000360: 7869 7428 290d 0a20 2020 2020 2020 2020  xit()..         
+00000370: 2020 2020 2020 2065 6c69 6620 7363 656e         elif scen
+00000380: 6172 696f 3d3d 2272 6573 7461 7274 2063  ario=="restart c
+00000390: 6163 6865 223a 0d0a 2020 2020 2020 2020  ache":..        
+000003a0: 2020 2020 2020 2020 2020 2020 7769 7468              with
+000003b0: 2050 7562 6c69 7368 6572 2866 6972 6564   Publisher(fired
+000003c0: 7269 6c6c 5f6d 6f64 653d 6664 5f6d 6f64  rill_mode=fd_mod
+000003d0: 652c 2076 6572 626f 7365 3d46 616c 7365  e, verbose=False
+000003e0: 2920 6173 2070 7562 3a0d 0a20 2020 2020  ) as pub:..     
 000003f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000400: 2020 2020 2370 6173 7377 203d 206f 732e      #passw = os.
-00000410: 6765 7465 6e76 2822 4144 4d49 4e5f 5041  getenv("ADMIN_PA
-00000420: 5353 222c 2022 4e4f 5f41 5554 4822 2920  SS", "NO_AUTH") 
-00000430: 2320 6e65 6564 2061 2062 6574 7465 7220  # need a better 
-00000440: 7465 7374 2d62 726f 6b65 7220 2f20 7465  test-broker / te
-00000450: 7374 2d63 6163 6865 0d0a 2020 2020 2020  st-cache..      
+00000400: 2020 2023 7061 7373 7720 3d20 6f73 2e67     #passw = os.g
+00000410: 6574 656e 7628 2241 444d 494e 5f50 4153  etenv("ADMIN_PAS
+00000420: 5322 2c20 224e 4f5f 4155 5448 2229 2023  S", "NO_AUTH") #
+00000430: 206e 6565 6420 6120 6265 7474 6572 2074   need a better t
+00000440: 6573 742d 6272 6f6b 6572 202f 2074 6573  est-broker / tes
+00000450: 742d 6361 6368 650d 0a20 2020 2020 2020  t-cache..       
 00000460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000470: 2020 7075 622e 7365 6e64 285b 7b27 5f69    pub.send([{'_i
-00000480: 6427 3a20 2730 5f68 6172 642d 7265 7365  d': '0_hard-rese
-00000490: 745f 272c 2027 7061 7373 273a 2027 7665  t_', 'pass': 've
-000004a0: 7279 3173 6563 7265 7432 7061 7373 776f  ry1secret2passwo
-000004b0: 7264 272c 2027 6465 7465 6374 6f72 5f6e  rd', 'detector_n
-000004c0: 616d 6527 3a27 5845 4e4f 4e6e 5427 2c0d  ame':'XENONnT',.
-000004d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000470: 2070 7562 2e73 656e 6428 5b7b 275f 6964   pub.send([{'_id
+00000480: 273a 2027 305f 6861 7264 2d72 6573 6574  ': '0_hard-reset
+00000490: 5f27 2c20 2770 6173 7327 3a20 2776 6572  _', 'pass': 'ver
+000004a0: 7931 7365 6372 6574 3270 6173 7377 6f72  y1secret2passwor
+000004b0: 6427 2c20 2764 6574 6563 746f 725f 6e61  d', 'detector_na
+000004c0: 6d65 273a 2758 454e 4f4e 6e54 272c 0d0a  me':'XENONnT',..
+000004d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000004e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000004f0: 2020 2020 276d 6574 6127 3a7b 7d7d 5d29      'meta':{}}])
-00000500: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000510: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00000520: 273e 2043 6163 6865 2063 6c65 616e 6564  '> Cache cleaned
-00000530: 5c6e 2729 0d0a 2020 2020 2020 2020 2020  \n')..          
-00000540: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+000004f0: 2020 2027 6d65 7461 273a 7b7d 7d5d 290d     'meta':{}}]).
+00000500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000510: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
+00000520: 3e20 4361 6368 6520 636c 6561 6e65 645c  > Cache cleaned\
+00000530: 6e27 290d 0a20 2020 2020 2020 2020 2020  n')..           
+00000540: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
 00000550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000560: 2063 6c69 636b 2e73 6563 686f 2866 225c   click.secho(f"\
-00000570: 6e3e 3e3e 2054 6573 7469 6e67 207b 7363  n>>> Testing {sc
-00000580: 656e 6172 696f 7d22 2c20 6667 3d27 7965  enario}", fg='ye
-00000590: 6c6c 6f77 272c 2062 6f6c 643d 5472 7565  llow', bold=True
-000005a0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000005b0: 2020 2020 2020 206d 6573 7361 6765 7320         messages 
-000005c0: 3d20 6461 7461 5b73 6365 6e61 7269 6f5d  = data[scenario]
-000005d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000005e0: 2020 2020 2020 666f 7220 6d73 6720 696e        for msg in
-000005f0: 206d 6573 7361 6765 733a 2023 2073 656e   messages: # sen
-00000600: 6420 6f6e 6520 6279 206f 6e65 2061 6e64  d one by one and
-00000610: 2073 6c65 6570 2069 6e20 6265 7477 6565   sleep in betwee
-00000620: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
-00000630: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00000640: 286d 7367 2c20 225c 6e5c 6e22 290d 0a20  (msg, "\n\n").. 
+00000560: 636c 6963 6b2e 7365 6368 6f28 6622 5c6e  click.secho(f"\n
+00000570: 3e3e 3e20 5465 7374 696e 6720 7b73 6365  >>> Testing {sce
+00000580: 6e61 7269 6f7d 222c 2066 673d 2779 656c  nario}", fg='yel
+00000590: 6c6f 7727 2c20 626f 6c64 3d54 7275 6529  low', bold=True)
+000005a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000005b0: 2020 2020 2020 6d65 7373 6167 6573 203d        messages =
+000005c0: 2064 6174 615b 7363 656e 6172 696f 5d0d   data[scenario].
+000005d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000005e0: 2020 2020 2066 6f72 206d 7367 2069 6e20       for msg in 
+000005f0: 6d65 7373 6167 6573 3a20 2320 7365 6e64  messages: # send
+00000600: 206f 6e65 2062 7920 6f6e 6520 616e 6420   one by one and 
+00000610: 736c 6565 7020 696e 2062 6574 7765 656e  sleep in between
+00000620: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000630: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00000640: 6d73 672c 2022 5c6e 5c6e 2229 0d0a 2020  msg, "\n\n")..  
 00000650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000660: 2020 2020 2020 2053 4e45 5753 5469 6572         SNEWSTier
-00000670: 7350 7562 6c69 7368 6572 282a 2a6d 7367  sPublisher(**msg
-00000680: 2c20 6669 7265 6472 696c 6c5f 6d6f 6465  , firedrill_mode
-00000690: 3d66 645f 6d6f 6465 292e 7365 6e64 5f74  =fd_mode).send_t
-000006a0: 6f5f 736e 6577 7328 290d 0a20 2020 2020  o_snews()..     
+00000660: 2020 2020 2020 534e 4557 534d 6573 7361        SNEWSMessa
+00000670: 6765 4275 696c 6465 7228 2a2a 6d73 6729  geBuilder(**msg)
+00000680: 2e73 656e 645f 6d65 7373 6167 6573 2866  .send_messages(f
+00000690: 6972 6564 7269 6c6c 5f6d 6f64 653d 6664  iredrill_mode=fd
+000006a0: 5f6d 6f64 6529 0d0a 2020 2020 2020 2020  _mode)..        
 000006b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000006c0: 2020 2074 696d 652e 736c 6565 7028 3129     time.sleep(1)
-000006d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000006e0: 2020 2020 2020 2020 2020 2320 636c 6561            # clea
-000006f0: 7220 6361 6368 6520 6166 7465 7220 6561  r cache after ea
-00000700: 6368 2073 6365 6e61 7269 6f0d 0a20 2020  ch scenario..   
-00000710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000720: 2077 6974 6820 5075 626c 6973 6865 7228   with Publisher(
-00000730: 6669 7265 6472 696c 6c5f 6d6f 6465 3d66  firedrill_mode=f
-00000740: 645f 6d6f 6465 2c20 7665 7262 6f73 653d  d_mode, verbose=
-00000750: 4661 6c73 6529 2061 7320 7075 623a 0d0a  False) as pub:..
+000006c0: 7469 6d65 2e73 6c65 6570 2831 290d 0a20  time.sleep(1).. 
+000006d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000006e0: 2020 2020 2020 2023 2063 6c65 6172 2063         # clear c
+000006f0: 6163 6865 2061 6674 6572 2065 6163 6820  ache after each 
+00000700: 7363 656e 6172 696f 0d0a 2020 2020 2020  scenario..      
+00000710: 2020 2020 2020 2020 2020 2020 2020 7769                wi
+00000720: 7468 2050 7562 6c69 7368 6572 2866 6972  th Publisher(fir
+00000730: 6564 7269 6c6c 5f6d 6f64 653d 6664 5f6d  edrill_mode=fd_m
+00000740: 6f64 652c 2076 6572 626f 7365 3d46 616c  ode, verbose=Fal
+00000750: 7365 2920 6173 2070 7562 3a0d 0a20 2020  se) as pub:..   
 00000760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000770: 2020 2020 2020 2020 7075 622e 7365 6e64          pub.send
-00000780: 285b 7b27 5f69 6427 3a20 2730 5f68 6172  ([{'_id': '0_har
-00000790: 642d 7265 7365 745f 272c 2027 7061 7373  d-reset_', 'pass
-000007a0: 273a 2776 6572 7931 7365 6372 6574 3270  ':'very1secret2p
-000007b0: 6173 7377 6f72 6427 2c20 2764 6574 6563  assword', 'detec
-000007c0: 746f 725f 6e61 6d65 273a 2758 454e 4f4e  tor_name':'XENON
-000007d0: 6e54 272c 0d0a 2020 2020 2020 2020 2020  nT',..          
+00000770: 2020 2020 2070 7562 2e73 656e 6428 5b7b       pub.send([{
+00000780: 275f 6964 273a 2027 305f 6861 7264 2d72  '_id': '0_hard-r
+00000790: 6573 6574 5f27 2c20 2770 6173 7327 3a27  eset_', 'pass':'
+000007a0: 7665 7279 3173 6563 7265 7432 7061 7373  very1secret2pass
+000007b0: 776f 7264 272c 2027 6465 7465 6374 6f72  word', 'detector
+000007c0: 5f6e 616d 6527 3a27 5845 4e4f 4e6e 5427  _name':'XENONnT'
+000007d0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
 000007e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000007f0: 2020 2020 2020 2020 2027 6d65 7461 273a           'meta':
-00000800: 7b7d 7d5d 290d 0a20 2020 2020 2020 2020  {}}])..         
-00000810: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00000820: 7269 6e74 2827 3e20 4361 6368 6520 636c  rint('> Cache cl
-00000830: 6561 6e65 645c 6e27 290d 0a20 2020 2020  eaned\n')..     
-00000840: 2020 2065 7863 6570 7420 4b65 7962 6f61     except Keyboa
-00000850: 7264 496e 7465 7272 7570 743a 0d0a 2020  rdInterrupt:..  
-00000860: 2020 2020 2020 2020 2020 6272 6561 6b0d            break.
-00000870: 0a65 7863 6570 7420 4578 6365 7074 696f  .except Exceptio
-00000880: 6e20 6173 2065 3a0d 0a20 2020 2070 7269  n as e:..    pri
-00000890: 6e74 2822 536f 6d65 7468 696e 6720 7765  nt("Something we
-000008a0: 6e74 2077 726f 6e67 5c6e 222c 2065 2c20  nt wrong\n", e, 
-000008b0: 225c 6e54 7279 206d 616e 7561 6c6c 7920  "\nTry manually 
-000008c0: 7375 626d 6974 7469 6e67 206d 6573 7361  submitting messa
-000008d0: 6765 7320 3a2f 2229 0d0a 23              ges :/")..#
+000007f0: 2020 2020 2020 276d 6574 6127 3a7b 7d7d        'meta':{}}
+00000800: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00000810: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00000820: 7428 273e 2043 6163 6865 2063 6c65 616e  t('> Cache clean
+00000830: 6564 5c6e 2729 0d0a 2020 2020 2020 2020  ed\n')..        
+00000840: 6578 6365 7074 204b 6579 626f 6172 6449  except KeyboardI
+00000850: 6e74 6572 7275 7074 3a0d 0a20 2020 2020  nterrupt:..     
+00000860: 2020 2020 2020 2062 7265 616b 0d0a 6578         break..ex
+00000870: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
+00000880: 7320 653a 0d0a 2020 2020 7072 696e 7428  s e:..    print(
+00000890: 2253 6f6d 6574 6869 6e67 2077 656e 7420  "Something went 
+000008a0: 7772 6f6e 675c 6e22 2c20 652c 2022 5c6e  wrong\n", e, "\n
+000008b0: 5472 7920 6d61 6e75 616c 6c79 2073 7562  Try manually sub
+000008c0: 6d69 7474 696e 6720 6d65 7373 6167 6573  mitting messages
+000008d0: 203a 2f22 290d 0a23                       :/")..#
```

### Comparing `snews_pt-1.3.3/snews_pt/core/logging.py` & `snews_pt-1.3.4/snews_pt/core/logging.py`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.3/snews_pt/snews_format_checker.py` & `snews_pt-1.3.4/snews_pt/snews_format_checker.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,27 +5,68 @@
 except AttributeError:
     from dateutil.parser import isoparse as fromisoformat
 
 import os, json
 from .core.logging import getLogger, log_file
 import warnings
 import click
-import copy
+import numpy as np
+import re
 
 log_default = getLogger(__name__)
 
+def is_valid_iso_utc(text):
+    """
+    Checks if a string is a valid ISO 8601 UTC datetime string,
+    accepting any precision up to 12 digits and an optional Z.
+
+    Args:
+    text: The string to check.
+
+    Returns:
+    True if the string is a valid ISO 8601 UTC datetime string,
+    False otherwise.
+    """
+    pattern = r"^" \
+            r"(?P<year>\d{4})" \
+            r"(?:-(?P<month>\d{2}))" \
+            r"(?:-(?P<day>\d{2}))" \
+            r"(?:[Tt ](?P<hour>\d{2})" \
+            r"(?::(?P<minute>\d{2}))" \
+            r"(?::(?P<second>\d{2}))" \
+            r"(?:\.(?P<precision>\d{1,12})?)?)?" \
+            r"(?:Z)?" \
+            r"$"
+    match = re.match(pattern, text)
+    if not match:
+        return False
+  # Check if mandatory components are present
+    if not all([match.group(comp) for comp in ("year", "month", "day", "hour", "minute", "second")]):
+        return False
+  # Check if precision part is within limits (max 12 digits)
+    if match.group("precision") and len(match.group("precision")) > 12:
+        return False
+    return True
+
 # Check if detector name is in registered list.
 detector_file = os.path.abspath(os.path.join(os.path.dirname(__file__), 'auxiliary/detector_properties.json'))
 with open(detector_file) as file:
     snews_detectors = json.load(file)
 snews_detectors = list(snews_detectors.keys())
 
 
 class SnewsFormat:
+    """ Class to validate message formats. It checks;
+        ID
+        Detector name
+        Message type
+        Times in the message
+        p values
 
+    """
     def __init__(self, message, log=None):
         self.message = message
         self.message_keys = message.keys()
         self.log = log or log_default
         self.bypass = False # bypass if retraction, or remote command (bypasses all time checks!)
         self.is_test = self.check_if_test() # if True, don't check if times are reasonable (still checks format!)
 
@@ -52,53 +93,64 @@
         except Exception as e:
             self.log.error(f"\t> Something went wrong! {e}")
             warnings.warn(f"\n\n Something went wrong! \nSee the full logs {click.style(log_file, fg='blue')}", UserWarning)
             self.log.debug("*" * 40 + " END OF lOGS\n")
             return False
 
     def check_if_test(self):
+        """ Check if the submitted message is a test message
+
+        Returns
+        -------
+            True if the message contains ['meta']['is_test'] = True, else False
+        """
+        if "is_test" in self.message_keys:
+            return self.message['is_test']
+
         if "meta" in self.message_keys:
             if "is_test" in self.message['meta'].keys():
                 return self.message["meta"]["is_test"]
         return False
 
     def check_id(self):
-        """ check if the format is correct
+        """ check if the id is correct
             snews_pt sends messages in mongodb format
-            which HAS TO contain an _id field
+            which has ti contain an _id field
         """
         self.log.debug(f"\t> Checking _id ..")
         if "_id" not in self.message_keys:
             self.log.error(f"\t> Message without '_id' field")
             return False
         else:
             self.log.info(f"\t> Message has an '_id' field")
             idsplit = self.message['_id'].split('_')
             if len(idsplit) < 2:
                 self.log.error(f"\t> Message '_id' has different format. Expected '#_string' got {self.message['_id']}")
                 return False
             return True
 
     def check_detector(self):
+        """ Check if the detector name is valid
+        """
         self.log.debug(f"\t> Checking detector name.")
         if self.bypass:
             self.log.info(f"\t> Detector name check bypassed.")
             return True
         if 'detector_name' not in self.message_keys:
             self.log.error(f'\t> Does not have required key: "detector_name"')
             return False
         if self.message['detector_name'] not in snews_detectors:
             self.log.error(f'\t> Detector not found: {self.message["detector_name"]}')
             return False
         self.log.info(f'\t> Detector: {self.message["detector_name"]} valid')
         return True
 
     def check_message_type(self):
-        """ We expect Tier messages, and Commands,
-            and Tier messages require different checks
+        """ We expect Tier messages, and Commands, and Tier messages require different checks.
+            Check what the message type is.
         """
         self.log.debug(f"\t> Checking message type..")
         if "hard-reset" in self.message['_id']:
             self.log.debug("\t> Hard reset. Skipping format check.")
             self.bypass = True
 
         elif "test-connection" in self.message['_id']:
@@ -130,27 +182,32 @@
         else:
             self.log.error(f"\t> Unknown id Passed : {self.message['_id']}.")
             return False
         self.log.info(f"\t> Message type : {self.message['_id']} valid.")
         return True
 
     def check_detector_status(self):
-        """ if _id is for HB, check detector status field and neutrino time
+        """ if _id is for heartbeat,
+            check detector status field and neutrino time
         """
         self.log.debug(f"\t> Checking detector status..")
         if "detector_status" not in self.message_keys:
             self.log.error(f"\t> Heartbeat Message but detector_status not in keys.")
             return False
         if self.message["detector_status"].upper() not in ["ON", "OFF"]:
             self.log.error(f"\t> detector_status not ON or OFF.")
             return False
         self.log.info(f"\t> detector_status is valid.")
         return True
 
     def check_times(self):
+        """ Check the neutrino times. Unless it is a test message,
+        the times should be within last 24 hours to be valid.
+
+        """
         self.log.debug(f"\t> Checking Times..")
         if self.bypass:
             self.log.info(f"\t> Time checks bypassed.")
             return True
 
         # check if neutrino times exists and in string format
         if 'neutrino_time' not in self.message_keys:
@@ -159,40 +216,45 @@
         if type(self.message['neutrino_time']) is not str:
             self.log.error(f"\t> neutrino_time is not a string!.")
             return False
         self.log.info(f"\t> neutrino_time exists and is string.")
 
         # it exists and string, check if ISO format, and reasonable
         try:
-            dateobj = fromisoformat(self.message["neutrino_time"])
+            dateobj = np.datetime64(self.message['neutrino_time'])
             self.log.info(f"\t> neutrino_time is ISO formattable.")
         except Exception as e:
             self.log.error("\t> neutrino_time does not match "
                       f"SNEWS 2.0 (ISO) format: '%Y-%m-%dT%H:%M:%S.%f'\n\t{e}")
             return False
 
         # neutrino_times exists, and in str - ISO format, check dates
         if self.is_test:
             # for tests, exact time is irrelevant
             self.log.info(f"\t> neutrino_time is checked for is_test=True, not checking time interval.")
             return True
+        now_datetime = datetime.utcnow()
+        now_datetime64 = np.datetime64(now_datetime)
+        time_delta = dateobj- now_datetime64
+        total_seconds = time_delta / np.timedelta64(1, 's')
 
-        if (dateobj - datetime.utcnow()).total_seconds() <= -172800.0:
+        if total_seconds <= -172800.0:
             self.log.error(f'\t> neutrino time is more than 48 hrs olds !\n')
             return False
 
-        if (dateobj - datetime.utcnow()).total_seconds() > 0:
+        if total_seconds > 0:
             self.log.error(f'\t> neutrino time comes from the future, please stop breaking causality.')
             return False
         # if all passed, return True
         self.log.info(f"\t> neutrino_time passed all time checks.")
         return True
 
     def check_pvals(self):
-        """ check if p_val exists, and valid
+        """ check if `p_val` exists, and valid
+
         """
         self.log.debug(f"\t> Checking p_val..")
         if 'p_val' in self.message_keys:
             if self.message['p_val'] is None:
                 self.log.info(f"\t> p_val is defaulted to None.")
                 return True # does not exist/default to None
```

### Comparing `snews_pt-1.3.3/snews_pt/snews_sub.py` & `snews_pt-1.3.4/snews_pt/snews_sub.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,36 +2,47 @@
 from datetime import datetime
 import os, json, click
 from hop import Stream
 from . import snews_pt_utils
 
 def make_file(outputfolder):
     """ Get a proper json file name at a given folder
+        It applies an increment to the file name at a given folder to avoid overwrite
+
     """
     os.makedirs(outputfolder, exist_ok=True)
     date = datetime.utcnow().isoformat().split('T')[0]
     file = os.path.join(outputfolder, f"0-SNEWS_ALERT_{date}.json")
     while os.path.isfile(file):
         i = int(file.split('/')[-1].split('-')[0])
         file = os.path.join(outputfolder, f"{i+1}-SNEWS_ALERT_{date}.json")
     return file
 
 def save_message(message, outputfolder, return_file=False):
     """ Save messages to a json file.
+        Parameters
+        ----------
+        message : dict
+            The incoming alert message
+        outputfolder : str
+            The path where to save the incoming alerts
+        return_file : bool
+            Whether to return file name as a string
 
     """
     file = make_file(outputfolder)
     with open(file, 'w') as outfile:
         json.dump(message, outfile, indent=4, sort_keys=True)
 
     if return_file:
         return file
 
 def display(message):
-    """ Function to format output messages
+    """ Display the incoming alert message on screen
+
     """
     click.echo(click.style('ALERT MESSAGE'.center(65, '_'), bg='red', bold=True))
 
     for k, v in message.items():
         key_type = type(v)
         if key_type == type(None):
             v = 'None'
@@ -59,18 +70,17 @@
 
 
 class Subscriber:
     """ Class to subscribe ALERT message stream
 
     Parameters
     ----------
-    env_path : `str`
-        path for the environment file.
-        Use default settings if not given
-    firedrill_mode : `bool`
+    env_path : str
+        path for the environment file. Use default settings if not given
+    firedrill_mode : bool
         tell Subscriber to get messages from the firedrill hop broker, defaults to False
 
     """
     def __init__(self, env_path=None, firedrill_mode=True):
         snews_pt_utils.set_env(env_path)
         self.alert_topic = os.getenv("ALERT_TOPIC")
         if firedrill_mode:
@@ -81,17 +91,16 @@
 
 
     def subscribe(self, outputfolder=None, auth=True):
         """ Subscribe and listen to a given topic
 
         Parameters
         ----------
-        outputfolder: `str`
-            where to save the alert messages, if None
-            creates a file based on env file
+        outputfolder: str
+            where to save the alert messages, if None, creates a file based on env file
         auth: A `bool` or :class:`Auth <hop.auth.Auth>` instance. Defaults to
             loading from :meth:`auth.load_auth <hop.auth.load_auth>` if set to
             True. To disable authentication, set to False.
 
         """
         outputfolder = outputfolder or self.default_output
         click.echo('You are subscribing to ' +
@@ -109,15 +118,15 @@
                     save_message(message, outputfolder)
                     snews_pt_utils.display_gif()
                     display(message)
         except KeyboardInterrupt:
             click.secho('Done', fg='green')
 
 
-    def subscribe_and_redirect_alert(self, outputfolder=None,  auth=True):
+    def subscribe_and_redirect_alert(self, outputfolder=None, auth=True, _display=True, _return='file'):
         """ subscribe generator
         """
         outputfolder = outputfolder or self.default_output
         click.echo('You are subscribing to ' +
                    click.style(f'ALERT', bg='red', bold=True) + '\nBroker:' +
                    click.style(f'{ self.alert_topic}', bg='green'))
 
@@ -126,12 +135,16 @@
         try:
             with stream.open(self.alert_topic, "r") as s:
                 for message in s:
                     # Access message dictionary from JSONBlobg
                     message = message.content
                     # Save and display
                     file = save_message(message, outputfolder, return_file=True)
-                    snews_pt_utils.display_gif()
-                    display(message)
-                    yield file
+                    if _display:
+                        snews_pt_utils.display_gif()
+                        display(message)
+                    if _return == 'message':
+                        yield message
+                    else:
+                        yield file
         except KeyboardInterrupt:
             click.secho('Done', fg='green')
```

### Comparing `snews_pt-1.3.3/snews_pt/test/random_plugin.py` & `snews_pt-1.3.4/snews_pt/test/random_plugin.py`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.3/snews_pt/test/test_coincidence_tier.py` & `snews_pt-1.3.4/snews_pt/test/test_heartbeat.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-"""Test publishing coincidence tier messages."""
-from snews_pt.snews_pub import SNEWSTiersPublisher
-from snews_pt.snews_format_checker import SnewsFormat
+"""Test publishing heartbeat messages."""
+from snews_pt.messages import SNEWSMessageBuilder
 
-def test_coincidence_expected():
+def test_heartbeat_expected():
     """Test with example of expected message type."""
-    # Create coincidence tier message.
-    coin = SNEWSTiersPublisher(detector_name='KamLAND', neutrino_time='2012-06-09T15:31:08.891011',
-                               firedrill_mode=False, is_test=True)
+    # Create heartbeat tier message.
+    hb = SNEWSMessageBuilder(detector_name='XENONnT', machine_time='2012-06-09T15:30:00.000501',
+                             detector_status='ON',
+                             firedrill_mode=False, is_test=True)
     # Check that message has expected structure.
-    assert list(coin.tiernames) == ['CoincidenceTier']
-    assert len(coin.messages) == 1, f"Expected 1 CoincidenceTier Message got {len(coin.messages)}!"
+    assert hb.selected_tiers == ['SNEWSHeartbeatMessage']
+    assert len(hb.messages) == 1, f"Expected 1 Heartbeat Message got {len(hb.messages)}!"
 
-    assert coin.message_data == {'detector_name': 'KamLAND', 'machine_time': None,
-                                 'neutrino_time': '2012-06-09T15:31:08.891011',
-                                 'p_val': None, 'p_values': None, 't_bin_width': None, 'timing_series': None,
-                                 'retract_latest': None, 'retraction_reason': None,
-                                 'detector_status': None, 'is_pre_sn': False, 'is_test':True}
+    assert hb.messages[0].message_data == {'_id': 'XENONnT_Heartbeat_2012-06-09T15:30:00.000501000',
+                                           'schema_version': '1.3.1',
+                                           'detector_name': 'XENONnT',
+                                           'machine_time': '2012-06-09T15:30:00.000501000',
+                                           'detector_status': 'ON',
+                                           'is_test': True}
 
-    # the SNEWSTierPublisher already checks this in creation, but we can double check
-    for message in coin.messages:
-        format_checker = SnewsFormat(message)
-        assert format_checker() is True, "Message is not in the snews format"
+    # firedrill_mode is an argument of hb.send_messages(), so it becomes meta here
+    assert hb.messages[0].meta == {'firedrill_mode': False}
 
-    assert len(coin.invalid_messages) == 0, "There are invalid messages"
+    # # check if valid snews format
+    assert hb.messages[0].is_valid() is True, "Message is not valid"
 
     # Try to send message to SNEWS 2.0 server.
     try:
-        coin.send_to_snews()
+        hb.send_messages()
     except Exception as exc:
-        print('SNEWSTiersPublisher.send_to_snews() test failed!\n')
-        assert False, f"Exception raised:\n {exc}"
+        print('SNEWSMessageBuilder.send_messages() test failed!\n')
+        assert False, f"Exception raised:\n {exc}"
```

### Comparing `snews_pt-1.3.3/snews_pt/test/test_plugin.py` & `snews_pt-1.3.4/snews_pt/test/test_plugin.py`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.3/snews_pt/test/test_retraction.py` & `snews_pt-1.3.4/snews_pt/test/test_coincidence_tier.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,33 @@
+"""Test publishing coincidence tier messages."""
+from snews_pt.messages import SNEWSMessageBuilder
 
-"""Test publishing coincidence tier message and then retracting it"""
-from snews_pt.snews_pub import SNEWSTiersPublisher
-
-def test_retraction():
+def test_coincidence_expected():
     """Test with example of expected message type."""
     # Create coincidence tier message.
-    coin = SNEWSTiersPublisher(detector_name='KamLAND', neutrino_time='2012-06-09T15:31:08.891011',
+    coin = SNEWSMessageBuilder(detector_name='KamLAND', machine_time='2012-06-09T15:30:00.000501',
+                               neutrino_time='2012-06-09T15:31:08.891011',
                                firedrill_mode=False, is_test=True)
-
     # Check that message has expected structure.
-    assert list(coin.tiernames) == ['CoincidenceTier']
+    assert coin.selected_tiers == ['SNEWSCoincidenceTierMessage']
     assert len(coin.messages) == 1, f"Expected 1 CoincidenceTier Message got {len(coin.messages)}!"
+
+    assert coin.messages[0].message_data == {'_id': 'KamLAND_CoincidenceTier_2012-06-09T15:30:00.000501000',
+                                             'detector_name': 'KamLAND',
+                                             'machine_time': '2012-06-09T15:30:00.000501000',
+                                             'schema_version': '1.3.1',
+                                             'neutrino_time': '2012-06-09T15:31:08.891011000',
+                                             'is_test': True,
+                                             'p_val': None}
+
+    # firedrill_mode is an argument of coinc.send_messages(), so it becomes meta here
+    assert coin.messages[0].meta == {'firedrill_mode': False}
+
+    # check if valid snews format
+    assert coin.messages[0].is_valid() is True, "Message is not valid"
+
     # Try to send message to SNEWS 2.0 server.
     try:
-        coin.send_to_snews()
+        coin.send_messages()
     except Exception as exc:
-        print('SNEWSTiersPublisher.send_to_snews() test failed!\n')
+        print('SNEWSMessageBuilder.send_messages() test failed!\n')
         assert False, f"Exception raised:\n {exc}"
-
-    # Now try to retract it
-    retraction_message = SNEWSTiersPublisher(detector_name='KamLAND', retract_latest=1, is_test=True, firedrill_mode=False)
-    try:
-        # we can only test if the retraction message is send, not if it really retracted.
-        retraction_message.send_to_snews()
-    except Exception as exc:
-        print('Retraction test failed!\n')
-        assert False, f"Exception raised:\n {exc}"
```

### Comparing `snews_pt-1.3.3/snews_pt/test/test_significance_tier.py` & `snews_pt-1.3.4/snews_pt/test/test_old_crashes.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,49 +1,31 @@
-"""Test publishing significane tier messages."""
-from snews_pt.snews_pub import SNEWSTiersPublisher
-from snews_pt.snews_format_checker import SnewsFormat
+"""Test publishing coincidence tier messages."""
+from snews_pt.messages import SNEWSMessageBuilder
 
-def test_significance_expected():
-    """Test with example of expected message type."""
-    # Create significance tier message.
-    sign = SNEWSTiersPublisher(detector_name='DS-20K',
-                               neutrino_time = '2012-06-09T15:31:08.109876',
-                               neutrino_times=['2012-06-09T15:31:08.109876', 
-                                               '2012-06-09T15:33:07.891098'],
-                               p_values=[0.4, 0.5],
-                               t_bin_width=0.8,
-                               firedrill_mode=False,
-                               is_test=True)
+def test_colon_in_time():
+    """Test with example of expected message type.
+        If works properly both format of times should pass
+    """
+    # Create coincidence tier message.
+    coin = SNEWSMessageBuilder(detector_name='XENONnT', neutrino_time='2012-06-09T15:31:07.891011', p_val=0.4,
+                               firedrill_mode=False, is_test=True)
 
-    # Check that message has expected structure.
-    assert list(sign.tiernames) == ['CoincidenceTier', 'SigTier']
-    assert sign.message_data == {'detector_name': 'DS-20K',
-                                'machine_time': None,
-                                'neutrino_time': '2012-06-09T15:31:08.109876',
-                                'p_val': None,
-                                'p_values': [0.4, 0.5],
-                                't_bin_width': 0.8,
-                                'timing_series': None,
-                                'retract_latest': None,
-                                'retraction_reason': None,
-                                'detector_status': None,
-                                'is_pre_sn': False,
-                                'neutrino_times': ['2012-06-09T15:31:08.109876',
-                                                   '2012-06-09T15:33:07.891098'],
-                                'is_test':True}
-    assert sign.env_file is None
-
-    # the SNEWSTierPublisher already checks this in creation, but we can double check
-    for message in sign.messages:
-        format_checker = SnewsFormat(message)
-        assert format_checker() is True, "Message is not in the snews format"
-
-    assert len(sign.invalid_messages)==0, "There are invalid messages"
-
-    # Try to send message to SNEWS 2.0 server.
+    # the SNEWSTierPublisher already checks this in creation, but we can double-check
+    assert coin.messages[0].is_valid() is True, "dot separated neutrino time failed!"
     try:
-        sign.send_to_snews()
+        coin.send_messages()
     except Exception as exc:
         print('SNEWSTiersPublisher.send_to_snews() test failed!\n')
         assert False, f"Exception raised:\n {exc}"
 
-test_significance_expected()
+    # ------------------------------------------------------------------------------------------------------
+    # coin2 = SNEWSMessageBuilder(detector_name='KamLAND', neutrino_time='2012-06-09T15:31:08:891011', p_val=0.4,
+    #                             firedrill_mode=False, is_test=True)
+    #
+    # # the SNEWSTierPublisher already checks this in creation, but we can double-check
+    # assert coin2.messages[0].is_valid() is True, "Semicolon separated neutrino time failed!"
+    # try:
+    #     coin2.send_messages()
+    # except Exception as exc:
+    #     print('SNEWSTiersPublisher.send_to_snews() test failed!\n')
+    #     assert False, f"Exception raised:\n {exc}"
+
```

### Comparing `snews_pt-1.3.3/snews_pt/test/test_subscribe.py` & `snews_pt-1.3.4/snews_pt/test/test_subscribe.py`

 * *Files identical despite different names*

