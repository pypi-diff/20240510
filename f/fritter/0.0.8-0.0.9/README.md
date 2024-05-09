# Comparing `tmp/fritter-0.0.8.tar.gz` & `tmp/fritter-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fritter-0.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fritter-0.0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fritter-0.0.8.tar` & `fritter-0.0.9.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0      201 2023-08-10 00:35:26.340672 fritter-0.0.8/.coveragerc
--rw-r--r--   0        0        0     2204 2024-02-09 07:57:48.866646 fritter-0.0.8/.github/workflows/test.yaml
--rw-r--r--   0        0        0       24 2023-08-16 00:35:14.486926 fritter-0.0.8/.gitignore
--rw-r--r--   0        0        0      903 2023-08-22 04:31:57.138743 fritter-0.0.8/.pydoctor.cfg
--rw-r--r--   0        0        0      826 2023-10-26 05:55:54.355538 fritter-0.0.8/.readthedocs.yaml
--rw-r--r--   0        0        0     1072 2022-01-20 08:55:34.036044 fritter-0.0.8/LICENSE
--rw-r--r--   0        0        0     3657 2024-02-09 21:33:58.965856 fritter-0.0.8/README.md
--rw-r--r--   0        0        0       55 2023-08-22 03:34:25.725348 fritter-0.0.8/dev-requirements.in
--rw-r--r--   0        0        0     2541 2024-02-09 05:21:25.340308 fritter-0.0.8/dev-requirements.txt
--rw-r--r--   0        0        0      635 2023-08-22 04:28:01.739510 fritter-0.0.8/docs/Makefile
--rw-r--r--   0        0        0        0 2023-08-26 08:41:37.654755 fritter-0.0.8/docs/_static/.exists
--rw-r--r--   0        0        0      230 2023-08-22 04:25:34.901433 fritter-0.0.8/docs/api/index.rst
--rw-r--r--   0        0        0      415 2023-08-25 05:32:05.335750 fritter-0.0.8/docs/asyncio_driver_example.py
--rw-r--r--   0        0        0     2422 2024-02-08 23:00:54.670525 fritter-0.0.8/docs/civil.rst
--rw-r--r--   0        0        0      996 2024-02-09 07:42:42.909194 fritter-0.0.8/docs/civil_example.py
--rw-r--r--   0        0        0     3035 2024-02-08 22:47:45.536361 fritter-0.0.8/docs/conf.py
--rw-r--r--   0        0        0      664 2024-02-09 00:08:02.249952 fritter-0.0.8/docs/drop_repeat.py
--rw-r--r--   0        0        0     5984 2024-02-09 00:08:23.297922 fritter-0.0.8/docs/friendminder.py
--rw-r--r--   0        0        0      522 2023-09-01 06:42:03.925266 fritter-0.0.8/docs/index.rst
--rw-r--r--   0        0        0     8142 2023-10-26 05:49:21.513075 fritter-0.0.8/docs/introduction.rst
--rw-r--r--   0        0        0     1980 2024-02-08 23:24:37.829108 fritter-0.0.8/docs/json_basic_reminder.py
--rw-r--r--   0        0        0      825 2024-02-07 07:41:13.605839 fritter-0.0.8/docs/json_example.py
--rw-r--r--   0        0        0     1219 2024-02-08 23:24:37.545122 fritter-0.0.8/docs/json_identity.py
--rw-r--r--   0        0        0     1018 2024-02-08 23:24:37.261570 fritter-0.0.8/docs/json_instance.py
--rw-r--r--   0        0        0      367 2023-09-01 04:09:09.378133 fritter-0.0.8/docs/json_just_load.py
--rw-r--r--   0        0        0      546 2023-11-15 08:01:20.066547 fritter-0.0.8/docs/json_just_save.py
--rw-r--r--   0        0        0      373 2023-09-01 03:39:24.957501 fritter-0.0.8/docs/json_load_id.py
--rw-r--r--   0        0        0     1411 2024-02-08 23:24:36.934758 fritter-0.0.8/docs/json_methods_example.py
--rw-r--r--   0        0        0      729 2024-02-09 00:08:33.429361 fritter-0.0.8/docs/json_save_repeat.py
--rw-r--r--   0        0        0      732 2024-02-09 00:08:37.112159 fritter-0.0.8/docs/json_save_repeat_id.py
--rw-r--r--   0        0        0     1072 2024-02-08 23:24:36.716371 fritter-0.0.8/docs/json_weekly_friend.py
--rw-r--r--   0        0        0      800 2023-08-16 00:22:48.422697 fritter-0.0.8/docs/make.bat
--rw-r--r--   0        0        0     7030 2024-02-08 23:24:36.358367 fritter-0.0.8/docs/persistence.rst
--rw-r--r--   0        0        0     3752 2024-02-09 21:11:27.992744 fritter-0.0.8/docs/quickstart.rst
--rw-r--r--   0        0        0     2320 2024-02-08 23:34:27.704124 fritter-0.0.8/docs/repeat.rst
--rw-r--r--   0        0        0      778 2024-02-09 00:08:52.715120 fritter-0.0.8/docs/repeating_example.py
--rw-r--r--   0        0        0       18 2023-08-22 03:45:48.947517 fritter-0.0.8/docs/requirements.in
--rw-r--r--   0        0        0     2069 2023-08-22 03:46:27.592144 fritter-0.0.8/docs/requirements.txt
--rw-r--r--   0        0        0      630 2024-02-09 00:09:02.872056 fritter-0.0.8/docs/simple_repeat.py
--rw-r--r--   0        0        0      848 2024-02-09 17:20:46.032787 fritter-0.0.8/docs/tree_example.py
--rw-r--r--   0        0        0      734 2024-02-09 17:21:16.865840 fritter-0.0.8/docs/tree_scaling_example.py
--rw-r--r--   0        0        0     4142 2024-02-09 17:22:16.240198 fritter-0.0.8/docs/trees.rst
--rw-r--r--   0        0        0      106 2023-08-12 09:20:12.658172 fritter-0.0.8/mypy.ini
--rw-r--r--   0        0        0      559 2024-02-09 21:31:15.807504 fritter-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      237 2024-02-01 23:21:16.554164 fritter-0.0.8/requirements.txt
--rw-r--r--   0        0        0      209 2024-02-09 21:34:14.157150 fritter-0.0.8/src/fritter/__init__.py
--rw-r--r--   0        0        0     8243 2024-02-09 07:38:18.438262 fritter-0.0.8/src/fritter/boundaries.py
--rw-r--r--   0        0        0       99 2023-08-26 00:49:11.899997 fritter-0.0.8/src/fritter/drivers/__init__.py
--rw-r--r--   0        0        0     3306 2024-02-09 09:32:19.911617 fritter-0.0.8/src/fritter/drivers/asyncio.py
--rw-r--r--   0        0        0     2748 2024-02-07 07:32:59.140033 fritter-0.0.8/src/fritter/drivers/datetime.py
--rw-r--r--   0        0        0     2693 2024-02-07 07:32:59.135632 fritter-0.0.8/src/fritter/drivers/memory.py
--rw-r--r--   0        0        0     3173 2024-02-07 07:32:59.139091 fritter-0.0.8/src/fritter/drivers/sleep.py
--rw-r--r--   0        0        0     2772 2024-02-09 07:38:18.438899 fritter-0.0.8/src/fritter/drivers/twisted.py
--rw-r--r--   0        0        0     1511 2024-02-07 07:32:59.130731 fritter-0.0.8/src/fritter/heap.py
--rw-r--r--   0        0        0       73 2023-08-26 08:43:39.506278 fritter-0.0.8/src/fritter/persistent/__init__.py
--rw-r--r--   0        0        0    30288 2024-02-09 09:32:33.926149 fritter-0.0.8/src/fritter/persistent/json.py
--rw-r--r--   0        0        0        0 2022-01-20 09:36:50.395812 fritter-0.0.8/src/fritter/py.typed
--rw-r--r--   0        0        0     7861 2024-02-09 07:38:18.454110 fritter-0.0.8/src/fritter/repeat/__init__.py
--rw-r--r--   0        0        0      118 2024-02-08 23:59:08.069000 fritter-0.0.8/src/fritter/repeat/rules/__init__.py
--rw-r--r--   0        0        0     3108 2024-02-09 09:32:19.909488 fritter-0.0.8/src/fritter/repeat/rules/datetimes.py
--rw-r--r--   0        0        0     1056 2024-02-09 07:38:18.438262 fritter-0.0.8/src/fritter/repeat/rules/seconds.py
--rw-r--r--   0        0        0     4934 2024-02-09 07:38:18.462778 fritter-0.0.8/src/fritter/scheduler.py
--rw-r--r--   0        0        0       59 2023-08-06 05:55:00.231920 fritter-0.0.8/src/fritter/test/__init__.py
--rw-r--r--   0        0        0     5423 2024-02-07 07:32:59.146943 fritter-0.0.8/src/fritter/test/test_asyncio.py
--rw-r--r--   0        0        0      376 2024-02-07 07:30:52.751470 fritter-0.0.8/src/fritter/test/test_datetime.py
--rw-r--r--   0        0        0    15391 2024-02-09 09:46:15.626456 fritter-0.0.8/src/fritter/test/test_json.py
--rw-r--r--   0        0        0      848 2024-02-07 07:32:59.145356 fritter-0.0.8/src/fritter/test/test_pq.py
--rw-r--r--   0        0        0     7474 2024-02-09 09:32:19.950231 fritter-0.0.8/src/fritter/test/test_repeat.py
--rw-r--r--   0        0        0     2896 2024-02-09 09:32:19.920558 fritter-0.0.8/src/fritter/test/test_scheduler.py
--rw-r--r--   0        0        0     2726 2024-02-07 07:32:42.132140 fritter-0.0.8/src/fritter/test/test_sleep.py
--rw-r--r--   0        0        0     1065 2023-08-25 05:12:07.439219 fritter-0.0.8/src/fritter/test/test_testing.py
--rw-r--r--   0        0        0     6955 2024-02-09 09:33:48.553579 fritter-0.0.8/src/fritter/test/test_tree.py
--rw-r--r--   0        0        0     3430 2023-08-13 16:47:24.968428 fritter-0.0.8/src/fritter/test/test_twisted.py
--rw-r--r--   0        0        0    10392 2024-02-09 17:23:47.750659 fritter-0.0.8/src/fritter/tree.py
--rw-r--r--   0        0        0      580 2024-02-09 07:54:45.072911 fritter-0.0.8/tox.ini
--rw-r--r--   0        0        0     4111 1970-01-01 00:00:00.000000 fritter-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      201 2023-08-10 00:35:26.340672 fritter-0.0.9/.coveragerc
+-rw-r--r--   0        0        0     2204 2024-02-09 07:57:48.866646 fritter-0.0.9/.github/workflows/test.yaml
+-rw-r--r--   0        0        0       24 2023-08-16 00:35:14.486926 fritter-0.0.9/.gitignore
+-rw-r--r--   0        0        0      903 2024-03-08 01:44:23.831946 fritter-0.0.9/.pydoctor.cfg
+-rw-r--r--   0        0        0      826 2023-10-26 05:55:54.355538 fritter-0.0.9/.readthedocs.yaml
+-rw-r--r--   0        0        0     1072 2022-01-20 08:55:34.036044 fritter-0.0.9/LICENSE
+-rw-r--r--   0        0        0     3661 2024-03-08 00:23:39.752811 fritter-0.0.9/README.md
+-rw-r--r--   0        0        0       55 2023-08-22 03:34:25.725348 fritter-0.0.9/dev-requirements.in
+-rw-r--r--   0        0        0     2541 2024-02-09 05:21:25.340308 fritter-0.0.9/dev-requirements.txt
+-rw-r--r--   0        0        0      635 2023-08-22 04:28:01.739510 fritter-0.0.9/docs/Makefile
+-rw-r--r--   0        0        0        0 2023-08-26 08:41:37.654755 fritter-0.0.9/docs/_static/.exists
+-rw-r--r--   0        0        0      230 2023-08-22 04:25:34.901433 fritter-0.0.9/docs/api/index.rst
+-rw-r--r--   0        0        0      492 2024-03-08 01:39:49.674091 fritter-0.0.9/docs/asyncio_driver_example.py
+-rw-r--r--   0        0        0     2422 2024-03-07 07:29:25.872725 fritter-0.0.9/docs/civil.rst
+-rw-r--r--   0        0        0      980 2024-03-08 01:46:10.436710 fritter-0.0.9/docs/civil_example.py
+-rw-r--r--   0        0        0     3009 2024-03-08 01:45:19.487345 fritter-0.0.9/docs/conf.py
+-rw-r--r--   0        0        0      701 2024-03-08 01:13:54.266616 fritter-0.0.9/docs/drop_repeat.py
+-rw-r--r--   0        0        0     7657 2024-03-08 01:32:19.472684 fritter-0.0.9/docs/friendminder.py
+-rw-r--r--   0        0        0      522 2023-09-01 06:42:03.925266 fritter-0.0.9/docs/index.rst
+-rw-r--r--   0        0        0     8195 2024-03-08 02:00:01.579452 fritter-0.0.9/docs/introduction.rst
+-rw-r--r--   0        0        0     2021 2024-03-08 01:31:39.427268 fritter-0.0.9/docs/json_basic_reminder.py
+-rw-r--r--   0        0        0      878 2024-03-08 01:30:57.226690 fritter-0.0.9/docs/json_example.py
+-rw-r--r--   0        0        0     1245 2024-03-08 00:23:38.126081 fritter-0.0.9/docs/json_identity.py
+-rw-r--r--   0        0        0     1021 2024-03-08 00:23:37.711265 fritter-0.0.9/docs/json_instance.py
+-rw-r--r--   0        0        0      415 2024-03-08 01:39:39.186666 fritter-0.0.9/docs/json_just_load.py
+-rw-r--r--   0        0        0      549 2024-03-08 01:39:09.515569 fritter-0.0.9/docs/json_just_save.py
+-rw-r--r--   0        0        0     1446 2024-03-08 01:30:08.822789 fritter-0.0.9/docs/json_methods_example.py
+-rw-r--r--   0        0        0      732 2024-03-08 01:39:06.117169 fritter-0.0.9/docs/json_save_repeat.py
+-rw-r--r--   0        0        0      735 2024-03-08 01:38:59.310543 fritter-0.0.9/docs/json_save_repeat_id.py
+-rw-r--r--   0        0        0     1092 2024-03-08 00:23:36.854269 fritter-0.0.9/docs/json_weekly_friend.py
+-rw-r--r--   0        0        0      800 2023-08-16 00:22:48.422697 fritter-0.0.9/docs/make.bat
+-rw-r--r--   0        0        0     7537 2024-03-08 00:26:47.940234 fritter-0.0.9/docs/persistence.rst
+-rw-r--r--   0        0        0     4043 2024-03-08 02:04:10.945674 fritter-0.0.9/docs/quickstart.rst
+-rw-r--r--   0        0        0     2328 2024-03-15 00:03:12.818921 fritter-0.0.9/docs/repeat.rst
+-rw-r--r--   0        0        0      838 2024-03-08 01:13:53.905297 fritter-0.0.9/docs/repeating_example.py
+-rw-r--r--   0        0        0       18 2023-08-22 03:45:48.947517 fritter-0.0.9/docs/requirements.in
+-rw-r--r--   0        0        0     2069 2023-08-22 03:46:27.592144 fritter-0.0.9/docs/requirements.txt
+-rw-r--r--   0        0        0      666 2024-03-08 01:13:53.613680 fritter-0.0.9/docs/simple_repeat.py
+-rw-r--r--   0        0        0      927 2024-03-08 01:13:53.255427 fritter-0.0.9/docs/tree_example.py
+-rw-r--r--   0        0        0      812 2024-03-08 01:13:52.858006 fritter-0.0.9/docs/tree_scaling_example.py
+-rw-r--r--   0        0        0     4142 2024-02-09 17:22:16.240198 fritter-0.0.9/docs/trees.rst
+-rw-r--r--   0        0        0      624 2024-03-08 01:56:25.628207 fritter-0.0.9/docs/twisted_driver_example.py
+-rw-r--r--   0        0        0      106 2023-08-12 09:20:12.658172 fritter-0.0.9/mypy.ini
+-rw-r--r--   0        0        0      559 2024-02-09 21:31:15.807504 fritter-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      237 2024-02-01 23:21:16.554164 fritter-0.0.9/requirements.txt
+-rw-r--r--   0        0        0      441 2024-05-09 22:31:25.014898 fritter-0.0.9/src/fritter/__init__.py
+-rw-r--r--   0        0        0    11191 2024-03-08 00:57:24.105259 fritter-0.0.9/src/fritter/boundaries.py
+-rw-r--r--   0        0        0       99 2023-08-26 00:49:11.899997 fritter-0.0.9/src/fritter/drivers/__init__.py
+-rw-r--r--   0        0        0     3542 2024-03-08 01:13:52.435750 fritter-0.0.9/src/fritter/drivers/asyncio.py
+-rw-r--r--   0        0        0     2748 2024-03-07 07:29:25.878723 fritter-0.0.9/src/fritter/drivers/datetimes.py
+-rw-r--r--   0        0        0     2693 2024-02-07 07:32:59.135632 fritter-0.0.9/src/fritter/drivers/memory.py
+-rw-r--r--   0        0        0     3173 2024-02-07 07:32:59.139091 fritter-0.0.9/src/fritter/drivers/sleep.py
+-rw-r--r--   0        0        0     2875 2024-03-08 01:13:52.043190 fritter-0.0.9/src/fritter/drivers/twisted.py
+-rw-r--r--   0        0        0     1511 2024-02-07 07:32:59.130731 fritter-0.0.9/src/fritter/heap.py
+-rw-r--r--   0        0        0       73 2023-08-26 08:43:39.506278 fritter-0.0.9/src/fritter/persistent/__init__.py
+-rw-r--r--   0        0        0    35042 2024-03-08 01:43:39.042141 fritter-0.0.9/src/fritter/persistent/jsonable.py
+-rw-r--r--   0        0        0        0 2022-01-20 09:36:50.395812 fritter-0.0.9/src/fritter/py.typed
+-rw-r--r--   0        0        0     7871 2024-03-08 00:34:47.114722 fritter-0.0.9/src/fritter/repeat/__init__.py
+-rw-r--r--   0        0        0      118 2024-02-08 23:59:08.069000 fritter-0.0.9/src/fritter/repeat/rules/__init__.py
+-rw-r--r--   0        0        0     4305 2024-03-08 01:44:05.864730 fritter-0.0.9/src/fritter/repeat/rules/datetimes.py
+-rw-r--r--   0        0        0     1235 2024-03-08 00:34:05.739737 fritter-0.0.9/src/fritter/repeat/rules/seconds.py
+-rw-r--r--   0        0        0     7241 2024-03-08 01:13:51.346381 fritter-0.0.9/src/fritter/scheduler.py
+-rw-r--r--   0        0        0       59 2023-08-06 05:55:00.231920 fritter-0.0.9/src/fritter/test/__init__.py
+-rw-r--r--   0        0        0     5433 2024-03-07 07:29:25.880775 fritter-0.0.9/src/fritter/test/test_asyncio.py
+-rw-r--r--   0        0        0      335 2024-03-07 07:29:25.881124 fritter-0.0.9/src/fritter/test/test_datetime.py
+-rw-r--r--   0        0        0    20646 2024-03-08 01:38:47.040775 fritter-0.0.9/src/fritter/test/test_json.py
+-rw-r--r--   0        0        0      848 2024-02-07 07:32:59.145356 fritter-0.0.9/src/fritter/test/test_pq.py
+-rw-r--r--   0        0        0     8458 2024-03-08 01:13:51.102492 fritter-0.0.9/src/fritter/test/test_repeat.py
+-rw-r--r--   0        0        0     3344 2024-03-08 01:27:40.936708 fritter-0.0.9/src/fritter/test/test_scheduler.py
+-rw-r--r--   0        0        0     2819 2024-03-08 01:13:50.772422 fritter-0.0.9/src/fritter/test/test_sleep.py
+-rw-r--r--   0        0        0     1065 2023-08-25 05:12:07.439219 fritter-0.0.9/src/fritter/test/test_testing.py
+-rw-r--r--   0        0        0     7209 2024-03-08 01:27:51.051695 fritter-0.0.9/src/fritter/test/test_tree.py
+-rw-r--r--   0        0        0     3507 2024-03-07 07:29:25.882856 fritter-0.0.9/src/fritter/test/test_twisted.py
+-rw-r--r--   0        0        0    10462 2024-05-08 21:56:55.167963 fritter-0.0.9/src/fritter/tree.py
+-rw-r--r--   0        0        0      599 2024-03-07 07:29:25.883436 fritter-0.0.9/tox.ini
+-rw-r--r--   0        0        0     4115 1970-01-01 00:00:00.000000 fritter-0.0.9/PKG-INFO
```

### Comparing `fritter-0.0.8/.github/workflows/test.yaml` & `fritter-0.0.9/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `fritter-0.0.8/.pydoctor.cfg` & `fritter-0.0.9/.pydoctor.cfg`

 * *Files identical despite different names*

### Comparing `fritter-0.0.8/.readthedocs.yaml` & `fritter-0.0.9/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `fritter-0.0.8/LICENSE` & `fritter-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fritter-0.0.8/README.md` & `fritter-0.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 - Do you need to schedule a very *low*-frequency timer, whose rate is measured
   in weeks or months, something that runs so infrequently or so far in the
   future that the current process will almost certainly no longer be running?
   Schedule your timer in terms of
   [`datetime`-ish](https://pypi.org/project/datetype/) objects, then serialize
   it with
-  [`fritter.persistent.json`](https://fritter.readthedocs.io/en/latest/persistence.html)
+  [`fritter.persistent.jsonable`](https://fritter.readthedocs.io/en/latest/persistence.html)
   to load it again when your process restarts.  `fritter.persistent` is careful
   to supply an interface using IANA identifiers to maintain correctness in the
   face of future DST changes, and other things that can start to complicate the
   use of time over longer periods.
 
 - Do you need to manage *groups* of related timers, sometimes pausing some
   groups while allowing others to continue, while all running on the same loop;
```

### Comparing `fritter-0.0.8/dev-requirements.txt` & `fritter-0.0.9/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `fritter-0.0.8/docs/Makefile` & `fritter-0.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fritter-0.0.8/docs/civil.rst` & `fritter-0.0.9/docs/civil.rst`

 * *Files 2% similar despite different names*

```diff
@@ -25,19 +25,20 @@
 ``float`` driver, which we will need first.
 
 .. literalinclude:: civil_example.py
    :start-after: set up memory
    :end-before: set up datetime
 
 :py:class:`DateTimeDriver <fritter.drivers.datetime.DateTimeDriver>` is a
-wrapper around any :py:class:`TimeDriver <fritter.boundaries.TimeDriver>`\ ``[float]``, so we can wrap it around a memory
-driver (or, similarly, another ``TimeDriver[float]`` such as :py:mod:`twisted
-<fritter.drivers.twisted>`, :py:mod:`asyncio <fritter.drivers.asyncio>` or just
-:py:mod:`sleep <fritter.drivers.sleep>`).  We need to create a time zone first
-— a :py:class:`ZoneInfo <zoneinfo.ZoneInfo>`, specifically.
+wrapper around any :py:class:`TimeDriver <fritter.boundaries.TimeDriver>`\
+``[float]``, so we can wrap it around a memory driver (or, similarly, another
+``TimeDriver[float]`` such as :py:mod:`twisted <fritter.drivers.twisted>`,
+:py:mod:`asyncio <fritter.drivers.asyncio>` or just :py:mod:`sleep
+<fritter.drivers.sleep>`).  We need to create a time zone first — a
+:py:class:`ZoneInfo <zoneinfo.ZoneInfo>`, specifically.
 
 .. literalinclude:: civil_example.py
    :start-after: set up datetime
    :end-before: set up scheduler
 
 Next, we'll pick a :py:class:`datetime <datetime.datetime>` as a reference
 point for our example.
```

### Comparing `fritter-0.0.8/docs/civil_example.py` & `fritter-0.0.9/docs/civil_example.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-from typing import Callable
-
 from datetime import datetime, timedelta
 from datetype import DateTime, aware
 from zoneinfo import ZoneInfo
 
-from fritter.boundaries import TimeDriver
+from fritter.boundaries import TimeDriver, CivilScheduler
 from fritter.drivers.memory import MemoryDriver
-from fritter.drivers.datetime import DateTimeDriver
-from fritter.scheduler import Scheduler
+from fritter.drivers.datetimes import DateTimeDriver
+from fritter.scheduler import schedulerFromDriver
 
 # set up memory driver
 advancer = MemoryDriver()
 base: TimeDriver[float] = advancer
 # set up datetime driver
 TZ = ZoneInfo("US/Pacific")
 dtdriver: TimeDriver[DateTime[ZoneInfo]] = DateTimeDriver(base, TZ)
 # set up scheduler
-scheduler = Scheduler[DateTime[ZoneInfo], Callable[[], None]](dtdriver)
+scheduler: CivilScheduler = schedulerFromDriver(dtdriver)
 # create datetime
 dt = datetime(2023, 5, 5, tzinfo=TZ)
 # advance to the timestamp
 advancer.advance(dt.timestamp() - advancer.now())
 # done advancing
```

### Comparing `fritter-0.0.8/docs/conf.py` & `fritter-0.0.9/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # For the full list of built-in configuration values, see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 import os
-from pprint import pprint
 import subprocess
 
 project = "Fritter"
 copyright = "2023, Glyph"
 author = "Glyph"
 
 # -- General configuration ---------------------------------------------------
```

### Comparing `fritter-0.0.8/docs/friendminder.py` & `fritter-0.0.9/docs/friendminder.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,74 +1,87 @@
 from __future__ import annotations
 
 from contextlib import contextmanager
 from dataclasses import dataclass, field
 from datetime import datetime, timedelta
-from json import dump, load
-from pathlib import Path
-from typing import Any, Iterator
+from json import dumps, loads
+from typing import Any, Callable, Iterator
 from zoneinfo import ZoneInfo
 
-from datetype import DateTime, aware, fromisoformat
-
-from fritter.boundaries import Cancellable, TimeDriver
-from fritter.drivers.datetime import DateTimeDriver, guessLocalZone
+from datetype import DateTime, aware
+from fritter.boundaries import SomeScheduledCall, TimeDriver
+from fritter.drivers.datetimes import DateTimeDriver, guessLocalZone
 from fritter.drivers.memory import MemoryDriver
 from fritter.drivers.sleep import SleepDriver
-from fritter.persistent.json import (
+from fritter.persistent.jsonable import (
+    JSONableScheduler,
     JSONObject,
     JSONRegistry,
-    JSONableScheduler,
     LoadProcess,
+    dateTypeAsJSON,
+    dateTypeFromJSON,
 )
-from fritter.repeat.rules.datetimes import weekly
-
+from fritter.repeat.rules.datetimes import weekly, yearly
 
 registry: JSONRegistry[FriendList] = JSONRegistry()
 
 
 @dataclass
 class FriendList:
     friendsByName: dict[str, Friend] = field(default_factory=dict)
+    loadingFriends: dict[str, dict[str, object]] = field(default_factory=dict)
+    scheduler: JSONableScheduler[FriendList] = field(init=False)
+    saver: Callable[[], JSONObject] = field(init=False)
 
-    def save(self, scheduler: JSONableScheduler[FriendList]) -> dict[str, Any]:
+    def getFriendNamed(
+        self, name: str, load: LoadProcess[FriendList]
+    ) -> Friend:
+        self.scheduler = load.scheduler
+        if name not in self.friendsByName:
+            blob = self.loadingFriends.pop(name)
+            self.friendsByName[name] = Friend.fromFriendListJSON(blob, load)
+        return self.friendsByName[name]
+
+    def save(self) -> dict[str, Any]:
         return {
-            "friends": [
-                friend.asFriendListJSON()
+            "friends": {
+                (blob := friend.asFriendListJSON())["name"]: blob
                 for friend in self.friendsByName.values()
-            ],
-            "scheduler": registry.save(scheduler),
+            },
+            "scheduler": self.saver(),
         }
 
     @classmethod
     def load(
         cls, driver: TimeDriver[float], json: dict[str, Any]
-    ) -> tuple[FriendList, JSONableScheduler[FriendList]]:
-        friendsByName = {}
-        for friendJSON in json["friends"]:
-            friend = Friend.fromFriendListJSON(friendJSON)
-            friendsByName[friend.name] = friend
-        self = cls(friendsByName)
-        return self, registry.load(driver, json["scheduler"], self)
+    ) -> FriendList:
+        self = cls(loadingFriends=json["friends"])
+        scheduler, saver = registry.loadScheduler(
+            DateTimeDriver(driver), json["scheduler"], self
+        )
+        self.saver = saver
+        self.scheduler = scheduler
+        assert not self.loadingFriends
+        return self
 
     @classmethod
     def typeCodeForJSON(cls) -> str:
         return "friend-list"
 
     def toJSON(self, registry: JSONRegistry[object]) -> dict[str, object]:
         return {}
 
     @classmethod
     def fromJSON(
         cls, load: LoadProcess[FriendList], json: JSONObject
     ) -> FriendList:
-        return load.context
+        return load.bootstrap
 
     @registry.repeatMethod
-    def getInTouch(self, steps: int, stopper: Cancellable) -> None:
+    def weeklyReminder(self, steps: int, scheduled: SomeScheduledCall) -> None:
         byContact = sorted(
             self.friendsByName.values(),
             key=lambda f: f.lastContact,
         )
         if (friend := next(iter(byContact), None)) is None:
             print("nobody to get in touch with right now")
             return
@@ -79,94 +92,119 @@
         self,
         name: str,
         birthdayDay: int,
         birthdayMonth: int,
         lastContact: DateTime[ZoneInfo],
     ) -> Friend:
         f = self.friendsByName[name] = Friend(
-            name, birthdayDay, birthdayMonth, lastContact
+            name, birthdayDay, birthdayMonth, lastContact, self.scheduler
         )
+        f.birthdaySetup()
         return f
 
     @classmethod
-    def new(
-        cls, driver: TimeDriver[float]
-    ) -> tuple[FriendList, JSONableScheduler[FriendList]]:
+    def new(cls, driver: TimeDriver[float]) -> FriendList:
         self = cls()
-        scheduler = registry.new(DateTimeDriver(driver))
-        registry.repeatedly(scheduler, weekly, self.getInTouch)
-        return self, scheduler
+        self.scheduler, self.saver = registry.createScheduler(DateTimeDriver(driver))
+        registry.repeatedly(self.scheduler, weekly, self.weeklyReminder)
+        return self
 
 
 TZ = guessLocalZone()
 
 
 def now() -> DateTime[ZoneInfo]:
     return DateTime.now(TZ)
 
 
+GRACE_DAYS = 3
+
+
 # friend-class
 @dataclass
 class Friend:
     name: str
-    birthdayDay: int
     birthdayMonth: int
+    birthdayDay: int
     lastContact: DateTime[ZoneInfo]
+    scheduler: JSONableScheduler[FriendList]
     # end-friend-fields
 
     def asFriendListJSON(self) -> dict[str, object]:
         return {
             "name": self.name,
             "birthdayDay": self.birthdayDay,
             "birthdayMonth": self.birthdayMonth,
-            "lastContact": {
-                "ts": self.lastContact.replace(tzinfo=None).isoformat(),
-                "tz": self.lastContact.tzinfo.key,
-            },
+            "lastContact": dateTypeAsJSON(self.lastContact),
         }
 
     @classmethod
-    def fromFriendListJSON(cls, json: dict[str, Any]) -> Friend:
+    def fromFriendListJSON(
+        cls, json: dict[str, Any], load: LoadProcess[FriendList]
+    ) -> Friend:
         return cls(
             json["name"],
             json["birthdayDay"],
             json["birthdayMonth"],
-            fromisoformat(json["lastContact"]["ts"]).replace(
-                tzinfo=ZoneInfo(json["lastContact"]["tz"])
-            ),
+            dateTypeFromJSON(json["lastContact"]),
+            load.scheduler,
         )
 
     @classmethod
     def typeCodeForJSON(cls) -> str:
         return "friend"
 
     def toJSON(self, registry: JSONRegistry[object]) -> dict[str, object]:
         return {"name": self.name}
 
     @classmethod
     def fromJSON(
         cls, load: LoadProcess[FriendList], json: JSONObject
     ) -> Friend:
-        return load.context.friendsByName[json["name"]]
+        return load.bootstrap.getFriendNamed(json["name"], load)
 
+    def birthdaySetup(self) -> None:
+        now = self.scheduler.now()
+        bday = now.replace(day=self.birthdayDay, month=self.birthdayMonth)
+        if bday < now:
+            bday = bday.replace(year=bday.date().year + 1)
+        registry.repeatedly(
+            self.scheduler, yearly, self.everyBirthday, reference=bday
+        )
 
-saved = Path("friend-schedule.json")
+    @registry.repeatMethod
+    def everyBirthday(
+        self, steps: list[DateTime[ZoneInfo]], scheduled: SomeScheduledCall
+    ) -> None:
+        if not steps:
+            print(f"setting up reminder for {self.name}'s birthday")
+            return
+        now = self.scheduler.now()
+        delta = now - steps[-1]
+        if delta > timedelta(days=GRACE_DAYS * 2):
+            print(f"Never mind, missed {self.name}'s birthday")
+            return
+        print(
+            f"Remember to wish {self.name} a happy birthday on {steps[-1].date()} (it's {now.date()})"
+        )
+        self.lastContact = now
+
+
+SAVED_BLOB = ""
 
 
 @contextmanager
 def listLoaded(driver: TimeDriver[float]) -> Iterator[FriendList]:
-    if saved.exists():
-        with saved.open() as f:
-            friendList, scheduler = FriendList.load(driver, load(f))
+    global SAVED_BLOB
+    if SAVED_BLOB:
+        friendList = FriendList.load(driver, loads(SAVED_BLOB))
     else:
-        friendList, scheduler = FriendList.new(driver)
+        friendList = FriendList.new(driver)
     yield friendList
-    blob = friendList.save(scheduler)
-    with saved.open("w") as f:
-        dump(blob, f)
+    SAVED_BLOB = dumps(friendList.save())
 
 
 @contextmanager
 def realTimeList() -> Iterator[FriendList]:
     driver = SleepDriver()
     with listLoaded(driver) as fl:
         driver.block(1.0)
@@ -187,32 +225,41 @@
 
 
 TZ = guessLocalZone()
 
 
 def story() -> None:
     start = aware(datetime(2023, 11, 1, 9, 0, 0, tzinfo=TZ), ZoneInfo)
-
-    print("day 1")
     st = Storyteller(start)
+
+    print("day 1", st.currentTime)
     with st.fakeTimeList(0) as fl1:
         fl1.add("alice", 12, 1, start)
         fl1.add("bob", 12, 15, start)
 
-    print("day 10")
+    print("run 1", st.currentTime)
     with st.fakeTimeList(timedelta(days=10).total_seconds()):
         pass
 
-    print("day 30")
+    print("run 2", st.currentTime)
     with st.fakeTimeList(timedelta(days=20).total_seconds()):
         pass
 
-    print("day 40")
+    print("run 3", st.currentTime)
     with st.fakeTimeList(timedelta(days=10).total_seconds()):
         pass
 
-    print("day 90")
+    print("run 4", st.currentTime)
+    with st.fakeTimeList(timedelta(days=10).total_seconds()):
+        pass
+    print("run 5", st.currentTime)
+    with st.fakeTimeList(timedelta(days=10).total_seconds()):
+        pass
+
+    print("run 6", st.currentTime)
     with st.fakeTimeList(timedelta(days=50).total_seconds()):
         pass
-    print("done")
+    print("done", st.currentTime)
+
+
 if __name__ == "__main__":
     story()
```

### Comparing `fritter-0.0.8/docs/index.rst` & `fritter-0.0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `fritter-0.0.8/docs/introduction.rst` & `fritter-0.0.9/docs/introduction.rst`

 * *Files 2% similar despite different names*

```diff
@@ -117,21 +117,22 @@
 Type Safety
 -----------
 
 Schedulers within Fritter are generic types on both *when* (what represents
 time) and *what* (what represents a callable).
 
 By allowing a given scheduler to constrain what types of work may be scheduled
-on them, you can tell mypy that ``x`` is a ``Scheduler[datetime,
-MyPersistentWork]``, and any attempt to schedule a generic, non-persistent
-callable on it will give you a (somewhat) readable type-checking error.  This
-means that you can specify your work in terms of ``datetime``, in terms of
-``float``, or indeed in terms of whatever custom time-keeping mechanism you
-have invented, if you want to work in terms of, for example, an ``int`` of
-microseconds rather than a ``float`` of seconds.
+on them, you can tell mypy that ``x`` is a :py:class:`Scheduler[datetime,
+MyPersistentWork, int] <fritter.boundaries.Scheduler>`, and any attempt to
+schedule a generic, non-persistent callable on it will give you a (somewhat)
+readable type-checking error.  This means that you can specify your desired
+times in terms of ``datetime``, in terms of ``float``, or indeed in terms of
+whatever custom time-keeping mechanism you have invented, if you want to work
+in terms of, for example, an ``int`` of microseconds rather than a ``float`` of
+seconds.
 
 Grouping Related Work Together
 ------------------------------
 
 You might also need groups of timers to happen on a *related* schedule.  For
 example, if you have a video game, all the timers comprising the game logic may
 need to be paused together when you pause the game, and then resumed together
```

### Comparing `fritter-0.0.8/docs/json_basic_reminder.py` & `fritter-0.0.9/docs/json_basic_reminder.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import sys
 from dataclasses import dataclass
 from datetime import timedelta
 from pathlib import Path
 from typing import Any
 
 from datetype import DateTime
-from fritter.drivers.datetime import guessLocalZone
+from fritter.drivers.datetimes import guessLocalZone, DateTimeDriver
 from fritter.drivers.sleep import SleepDriver
-from fritter.persistent.json import (
+from fritter.persistent.jsonable import (
     JSONableInstance,
     JSONableScheduler,
     JSONObject,
     JSONRegistry,
     LoadProcess,
     schedulerAtPath,
 )
@@ -66,20 +66,20 @@
     now = DateTime.now(guessLocalZone())
     later = now + timedelta(seconds=seconds)
     work = Reminder(message).show
     scheduler.callAt(later, work)
 
 
 def runScheduler(newReminder: tuple[int, str] | None) -> None:
-    context: dict[Any, Any] = {}
+    bootstrap: dict[Any, Any] = {}
     with schedulerAtPath(
         registry,
-        driver := SleepDriver(),
+        DateTimeDriver(driver := SleepDriver()),
         Path("saved-schedule.json"),
-        context,
+        bootstrap,
     ) as sched:
         driver.block(1.0)
         if newReminder:
             newTime, message = newReminder
             remind(sched, newTime, message)
```

### Comparing `fritter-0.0.8/docs/json_example.py` & `fritter-0.0.9/docs/json_example.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 from datetime import datetime
 from zoneinfo import ZoneInfo
 
 from datetype import aware
-from fritter.drivers.datetime import DateTimeDriver, guessLocalZone
+from fritter.drivers.datetimes import DateTimeDriver, guessLocalZone
 from fritter.drivers.memory import MemoryDriver
-from fritter.persistent.json import JSONableScheduler, JSONRegistry
+from fritter.persistent.jsonable import JSONableScheduler, JSONRegistry
 
 ctxtype = dict[str, str]
 
 registry = JSONRegistry[ctxtype]()
 
 
 @registry.function
 def call1() -> None:
     print("hello world")
 
 
 memoryDriver = MemoryDriver()
-scheduler = JSONableScheduler[ctxtype](DateTimeDriver(memoryDriver))
+scheduler: JSONableScheduler[ctxtype]
+scheduler, saver = registry.createScheduler(DateTimeDriver(memoryDriver))
+
 dt = aware(
     datetime(
         2023,
         7,
         21,
         1,
         1,
         1,
         tzinfo=guessLocalZone(),
     ),
     ZoneInfo,
 )
 handle = scheduler.callAt(dt, call1)
-dump = registry.save(scheduler)
+dump = saver()
 print(dump)
-mem2 = MemoryDriver()
-loaded = registry.load(mem2, dump, {})
+loaded = registry.loadScheduler(DateTimeDriver(mem2 := MemoryDriver()), dump, {})
 mem2.advance(dt.timestamp())
```

### Comparing `fritter-0.0.8/docs/json_identity.py` & `fritter-0.0.9/docs/json_instance.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,39 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 
-from fritter.boundaries import Cancellable
-from fritter.persistent.json import JSONObject, JSONRegistry, LoadProcess
+from fritter.boundaries import SomeScheduledCall
+from fritter.persistent.jsonable import JSONObject, JSONRegistry, LoadProcess
 
-registry: JSONRegistry[dict[int, MyClass]] = JSONRegistry()
+registry = JSONRegistry[dict[str, str]]()
 
 
 @dataclass
 class MyClass:
     value: int
 
     @classmethod
     def typeCodeForJSON(cls) -> str:
         return ".".join([cls.__module__, cls.__name__])
 
-    def toJSON(self, registry: JSONRegistry[object]) -> dict[str, object]:
-        return {"value": self.value, "id": id(self)}
+    def toJSON(
+        self, registry: JSONRegistry[dict[str, str]]
+    ) -> dict[str, object]:
+        return {"value": self.value}
 
     @classmethod
     def fromJSON(
-        cls, load: LoadProcess[dict[int, MyClass]], json: JSONObject
+        cls, load: LoadProcess[dict[str, str]], json: JSONObject
     ) -> MyClass:
-        loadingID = int(json["id"])
-        if loadingID in load.context:
-            return load.context[loadingID]
-        else:
-            self = cls(json["value"])
-            load.context[loadingID] = self
-            return self
+        return cls(json["value"])
 
     @registry.method
     def later(self) -> None:
         print("my value is", self.value)
 
     @registry.repeatMethod
-    def repeat(self, steps: int, stopper: Cancellable) -> None:
+    def repeat(self, steps: int, scheduled: SomeScheduledCall) -> None:
         print(f"performing {steps} steps at {self.value}")
         self.value += steps
         if self.value > 10:
-            stopper.cancel()
+            scheduled.cancel()
```

### Comparing `fritter-0.0.8/docs/json_just_save.py` & `fritter-0.0.9/docs/json_save_repeat_id.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 from datetime import timedelta
 from json import dump
 
 from datetype import DateTime
-from fritter.drivers.datetime import DateTimeDriver, guessLocalZone
+from fritter.drivers.datetimes import DateTimeDriver, guessLocalZone
 from fritter.drivers.memory import MemoryDriver
+from fritter.repeat.rules.datetimes import EveryDelta
 
-from json_instance import MyClass, registry
+from json_identity import MyClass, registry
 
 memoryDriver = MemoryDriver()
-scheduler = registry.new(DateTimeDriver(memoryDriver))
+scheduler, saver = registry.createScheduler(DateTimeDriver(memoryDriver))
 dt = DateTime.now(guessLocalZone())
-handle = scheduler.callAt(dt + timedelta(seconds=5), MyClass(3).later)
+memoryDriver.advance(dt.timestamp())
 myInstance = MyClass(3)
+handle = scheduler.callAt(dt + timedelta(seconds=5), myInstance.later)
+registry.repeatedly(
+    scheduler, EveryDelta(timedelta(seconds=0.5)), myInstance.repeat
+)
 
 
-with open("saved-schedule.json", "w") as f:
-    dump(registry.save(scheduler), f)
+with open("saved-id-schedule.json", "w") as f:
+    dump(saver(), f)
```

### Comparing `fritter-0.0.8/docs/json_methods_example.py` & `fritter-0.0.9/docs/json_methods_example.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from datetime import datetime
 from zoneinfo import ZoneInfo
 
 from datetype import aware
-from fritter.drivers.datetime import DateTimeDriver, guessLocalZone
+from fritter.drivers.datetimes import DateTimeDriver, guessLocalZone
 from fritter.drivers.memory import MemoryDriver
-from fritter.persistent.json import (
+from fritter.persistent.jsonable import (
     JSONObject,
     JSONRegistry,
     LoadProcess,
 )
 
 registry = JSONRegistry[dict[str, str]]()
 
@@ -35,15 +35,15 @@
 
     @registry.method
     def later(self) -> None:
         print("my value is", self.value)
 
 
 memoryDriver = MemoryDriver()
-scheduler = registry.new(DateTimeDriver(memoryDriver))
+scheduler, saver = registry.createScheduler(DateTimeDriver(memoryDriver))
 dt = aware(
     datetime(
         2023,
         7,
         21,
         1,
         1,
@@ -53,12 +53,14 @@
     ZoneInfo,
 )
 
 handle = scheduler.callAt(dt, MyClass(3).later)
 myInstance = MyClass(3)
 from json import dumps, loads
 
-dump = dumps(registry.save(scheduler))
+dump = dumps(saver())
 print(dump)
-mem2 = MemoryDriver()
-loaded = registry.load(mem2, loads(dump), {})
+
+loaded = registry.loadScheduler(
+    DateTimeDriver(mem2 := MemoryDriver()), loads(dump), {}
+)
 mem2.advance(dt.timestamp())
```

### Comparing `fritter-0.0.8/docs/json_save_repeat.py` & `fritter-0.0.9/docs/json_save_repeat.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from datetime import timedelta
 from json import dump
 
 from datetype import DateTime
-from fritter.drivers.datetime import DateTimeDriver, guessLocalZone
+from fritter.drivers.datetimes import DateTimeDriver, guessLocalZone
 from fritter.drivers.memory import MemoryDriver
 from fritter.repeat.rules.datetimes import EveryDelta
 
 from json_instance import MyClass, registry
 
 memoryDriver = MemoryDriver()
-scheduler = registry.new(DateTimeDriver(memoryDriver))
+scheduler, saver = registry.createScheduler(DateTimeDriver(memoryDriver))
 dt = DateTime.now(guessLocalZone())
 memoryDriver.advance(dt.timestamp())
 handle = scheduler.callAt(dt + timedelta(seconds=5), MyClass(3).later)
 myInstance = MyClass(3)
 registry.repeatedly(
     scheduler, EveryDelta(timedelta(seconds=0.5)), myInstance.repeat
 )
 
 
 with open("saved-schedule.json", "w") as f:
-    dump(registry.save(scheduler), f)
+    dump(saver(), f)
```

### Comparing `fritter-0.0.8/docs/json_weekly_friend.py` & `fritter-0.0.9/docs/json_weekly_friend.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 
-from fritter.boundaries import Cancellable
-from fritter.persistent.json import JSONObject, JSONRegistry, LoadProcess
+from fritter.boundaries import SomeScheduledCall
+from fritter.persistent.jsonable import JSONObject, JSONRegistry, LoadProcess
 
 registry = JSONRegistry[dict[str, str]]()
 
 
 @dataclass
 class FriendReminder:
     filename: str
@@ -27,12 +27,12 @@
         return cls(json["filename"], json["current"])
 
     @registry.method
     def later(self) -> None:
         print("my value is", self.current)
 
     @registry.repeatMethod
-    def repeat(self, steps: int, stopper: Cancellable) -> None:
+    def repeat(self, steps: int, scheduled: SomeScheduledCall) -> None:
         self.current += steps
         print(f"performing {steps} steps at {self.current}")
         if self.current > 10:
-            stopper.cancel()
+            scheduled.cancel()
```

### Comparing `fritter-0.0.8/docs/make.bat` & `fritter-0.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fritter-0.0.8/docs/persistence.rst` & `fritter-0.0.9/docs/persistence.rst`

 * *Files 5% similar despite different names*

```diff
@@ -11,33 +11,32 @@
 The most basic thing that we can do with a persistent task is remind the user
 to do sommething at some point in the future.  So let's start off by building
 that.
 
 Whever building anything persistent it is important to establish what objects
 are safe to serialize and how to serialize them in this context.  To register
 our serializable objects, we will use a :py:class:`JSONRegistry
-<fritter.persistent.JSONRegistry>`, so let's instantiate one.
+<fritter.persistent.jsonable.JOSNRegistry>`, so let's instantiate one.
 
 .. literalinclude:: json_basic_reminder.py
    :start-after: start-registry
    :end-before: end-registry
 
-Don't worry about the ``[object]`` there just yet; that tells us the type of
-the "load context" for this registry.  We'll get to that a little later, but we
-don't need it yet.
+Don't worry about the ``[object]`` there just yet; it tells us the type of the
+"bootstrap" for this registry.  We'll get to that later.
 
 Next, we'll make a Reminder class, which just holds a bit of text to remind us
 about.
 
 .. literalinclude:: json_basic_reminder.py
    :start-after: reminder-class
    :end-before: reminder-methods
 
 To make this class serializable by our JSON serializer, we have to add a few
-instance and class methods to conform to its interfaces:
+instance and class methods to conform to its required `Protocol`:
 
 - a ``typeCodeForJSON`` classmethod to provide a type-code string that uniquely
   identifies this class within the context of this specific ``JSONRegistry``
   instance, which defines our serialization format.
 
 - an ``toJSON`` instance method to serialize it to a JSON-serializable dict,
   and
@@ -50,35 +49,29 @@
 .. literalinclude:: json_basic_reminder.py
    :start-after: reminder-methods
    :end-before: end-reminder-methods
 
 To complete this object, we need the actual method which we will be scheduling
 to run in the future.  In order to mark a method as serializable by the
 scheduler, we define a 0-argument, ``None``-returning method and decorate it
-with :py:meth:`registry.method <fritter.persistent.json.JSONRegistry.method>`
+with :py:meth:`registry.method <fritter.persistent.jsonable.JSONRegistry.method>`
 from the ``JSONRegistry`` that we instantiated before.
 
 .. literalinclude:: json_basic_reminder.py
    :start-after: app-method
    :end-before: end-reminder
 
-So that's it for our "object model" for this application.  Next we need to add
-the functions to perform the tasks that we need.
+Now, we need to schedule the reminder.  For that, we'll have a function that
+schedules our ``show`` method with a given scheduler, which takes:
+- a scheduler,
+- some number of seconds into the future, and
+- a message to show.
 
-First, we need to actually schedule the reminder.  For that, we'll have a
-function that schedules our ``show`` method with a given scheduler.  To do
-this, we'll take a scheduler, some number of seconds into the future, and a
-message to show.  We'll instantiate a ``Reminder``, and create a
-``datetype.DateTime`` with a ``ZoneInfo`` time zone.
-
-Since the user probably wants their reminders scheduled in their *own* time
-zone, Fritter provides a convenience function, :py:func:`guessLocalZone
-<fritter.drivers.datetime.guessLocalZone>`\ , which uses platform-specific
-heuristics to determine the local machine's IANA timezone identifier and use
-that.
+We'll instantiate a ``Reminder``, and create a ``datetype.DateTime`` with a
+``ZoneInfo`` time zone.
 
 .. note::
 
    In order to serialize time zone information, we need a common method of
    identifying the zone, and a consistent type for using.  To ensure this,
    Fritter uses |datetype|_\ ’s
    type-wrapper for ``datetime.datetime``\ . This is purely for type-checking;
@@ -89,77 +82,104 @@
    not have this attribute and cannot be reliably serialized.  Mypy should
    alert you to any type mismatches here, so you don't need to memorize this,
    but that's why we are using ``datetype`` here.
 
 .. |datetype| replace:: ``datetype``
 .. _datetype: https://pypi.org/project/datetype
 
+Since the user probably wants their reminders scheduled in their *own* time
+zone, Fritter provides a convenience function, :py:func:`guessLocalZone
+<fritter.drivers.datetime.guessLocalZone>`\ , which uses platform-specific
+heuristics to determine the local machine's IANA timezone identifier and use
+that.
+
 .. literalinclude:: json_basic_reminder.py
    :pyobject: remind
 
 Next, when we run our script, we always want to load up the scheduler from the
 file where it is saved, if that file is there, and let it run for a little
 while to take care of any pending work before we do anything else.  We can
 create a :py:class:`SleepDriver <fritter.drivers.sleep.SleepDriver>` and use
 our ``JSONRegistry``'s ``load`` method, then :py:meth:`block
 <fritter.drivers.sleep.SleepDriver.block>` with a short timeout before
 returning the loaded scheduler.  We will then run some code to update the
 scheduler, maybe adding some stuff to it, then save it again with any completed
 calls removed and any new calls added.
 
 Fritter provides a function,
-:py:func:`fritter.persistent.json.schedulerAtPath`, which does most of this
-work for you, returning a contextmanager that either loads or creates a :py:class:`Scheduler <fritter.scheduler.Scheduler>`.
+:py:func:`fritter.persistent.jsonable.schedulerAtPath`, which does most of this
+work for you, returning a contextmanager that either loads or creates a
+:py:class:`Scheduler <fritter.scheduler.Scheduler>`.
 
 .. literalinclude:: json_basic_reminder.py
    :pyobject: runScheduler
 
 Now to put *all* of that together, we'll look at the command-line. If the user
 specifies any arguments, the first should be an integer number of seconds, and
 the rest of the command line is the message we want to get reminded of.
 Otherwise, just run the scheduler to catch up to the current time.
 
 .. literalinclude:: json_basic_reminder.py
    :start-at: __main__
 
-And that's it!  On the command line, you can set yourself some reminders:
+And that's it!  On the command line, you can set yourself some reminders.  Now,
+in a real application, you'd probably want significant amounts of time to pass,
+and run the script every day, or at most every few hours, to check on your
+reminders.  But to simulate that for a quick example, here's a little shell
+script that will set one reminder at 5 seconds, another at 10, then wait for
+them each to trigger:
 
 .. code-block::
 
-   $ python json_basic_reminder.py 5 hello
-   $ python json_basic_reminder.py 10 goodbye
+    python docs/json_basic_reminder.py 5 hello &&
+        python docs/json_basic_reminder.py 10 goodbye &&
+        echo 'one...' &&
+        sleep 6 &&
+        python docs/json_basic_reminder.py &&
+        echo 'two...' &&
+        sleep 6 && python
+        docs/json_basic_reminder.py
 
-And if you run ``python json_basic_reminder.py`` with no arguments after 5 and
-10 seconds respectively, you'll see your reminders print out.
+which will produce output that looks like this:
 
-With the techniques in this section, you can:
+.. code-block::
 
-- persist your timed events to a JSON blob
-- save them for the future
-- schedule bound methods on those objects to save state associated with your timers
+   one...
+   Reminder! hello
+   two...
+   Reminder! goodbye
+
+With the techniques that we reviewed in the section above, you should now be
+able to write a class whose methods can be scheduled with a persistent
+scheduler via ``schedulerAtPath``.
 
 Next, we will move on to a slightly more complex application with more
 interactions.
 
 Adding Recurrences And Counts: Friendminder Example
 ---------------------------------------------------
 
-To illustrate some slightly more complex uses of ``JSONRegistry``, let's build
-a little application that can help you keep in touch with friends.  It's all
-too easy to just forget to send a message to keep in touch, so let's make a
-tool to remind ourselves.
+Saving and loading scheduled calls with a bit of associated state is nice, but
+not generally useful if we can't save the relationships *between* those bits of
+associated state.  So next, we'll build a little application that can help you
+keep in touch with friends.
+
+It's all too easy to just forget to send a message to keep in touch every so
+often, so let's make a tool to remind ourselves.
 
 In this tool, we want to:
 
 1. have a list of friends that we can add to when we want to add more people to
    be reminded about,
 
 2. be reminded to send a message to one of those friends each week, cycling
    through that list.
 
 3. be reminded to get in touch with each friend on their birthday each year.
 
 This means we have two kinds of repeating call; the general "get in touch"
 reminder, which would need to be a method on some shared object that can
-reference the full list of friends, as well as the birthday-specific reminder,
-which should probably be a method on a ``Friend`` class itself.
+reference the full list of friends as we move from one to the next, as well as
+the birthday-specific reminder, which should probably be a method on a
+``Friend`` class itself.
+
```

### Comparing `fritter-0.0.8/docs/quickstart.rst` & `fritter-0.0.9/docs/quickstart.rst`

 * *Files 11% similar despite different names*

```diff
@@ -12,29 +12,34 @@
 :py:mod:`fritter.drivers.memory`.  Getting one is simple enough:
 
 .. code-block:: python
 
    from fritter.drivers.memory import MemoryDriver
    driver = MemoryDriver()
 
-Once you have a driver, you can schedule work on it with a ``Scheduler``, which
-you can find in ``fritter.scheduler``.
+Once you have a driver, you can schedule work on it with a :py:class:`Scheduler
+<fritter.scheduler.Scheduler>`, which you can create with
+:py:func:`fritter.scheduler.schedulerFromDriver`.
 
-Let's begin with a ``SimpleScheduler``, which is a scheduler that uses a
+Let's begin with a :py:class:`PhysicalScheduler
+<fritter.boundaries.PhysicalScheduler>`, which is a scheduler that uses a
 ``float`` timestamp to track time and can invoke any 0-argument callable.
 
 .. code-block:: python
 
-   from fritter.scheduler import SimpleScheduler
-   scheduler = SimpleScheduler(driver)
+   from fritter.boundaries import PhysicalScheduler
+   from fritter.scheduler import schedulerFromDriver
+   scheduler = schedulerFromDriver(driver)
+
+Now, let's define some work to do.  Again, our scheduler considers any callable
+object which takes no arguments and returns nothing to be a thing it can
+schedule for future execution, so we can define a regular function for this.
 
-Now, let's define some work to do.  Again, our ``SimpleScheduler`` considers
-any callable object which takes no arguments and returns nothing to be a valid
-piece of work, so we can define a regular function for this.  We'll make it
-print out the current time according to the scheduler via its ``now`` method.
+We'll make it print out the current time according to the scheduler via its
+``now`` method.
 
 .. code-block:: python
 
    def hello() -> None:
        print("hello", scheduler.now())
 
 
@@ -50,22 +55,24 @@
 
 .. code-block:: python
 
    driver.advance()
 
 From this, you can see ``1.0``.
 
-``MemoryDriver.advance``, when given no arguments, will always advance the
-internal timestamp of the ``MemoryDriver`` to whatever the time of its next
-scheduled work is, call any callables on the way there, then stop.  This does
-not necessarily mean it only does one bit of work; if two bits of work are
-scheduled at precisely the same time, it'll run them both.
-
-Since its main purpose is for testing, you can also ask the memory driver if it
-has any more work to do:
+:py:meth:`MemoryDriver.advance <fritter.drivers.memory.MemoryDriver.advance>`,
+when given no arguments, will always advance the internal timestamp of the
+``MemoryDriver`` to whatever the time of its next scheduled work is, call any
+callables on the way there, then stop.  This does not necessarily mean it only
+does one bit of work; if two bits of work are scheduled at precisely the same
+time, it'll run them both.
+
+Since its main purpose is for testing, you can also ask the
+:py:meth:`MemoryDriver <fritter.drivers.memory.MemoryDriver>` if it has any
+more work to do:
 
 .. code-block:: python
 
    print(driver.isScheduled())
 
 This should show you ``True``, since there is still the work at timestamp 2.0
 and 3.0 yet to complete.  Therefore this idiom will keep running at maximum
@@ -75,15 +82,15 @@
 
    while driver.isScheduled():
        driver.advance()
 
 This should show us ``hello 2.0``, and ``hello 3.0``, as each callable runs,
 then time advances to the scheduled time of the next one.  You can ask the
 driver the time directly with ``driver.now()``, and indeed, that should show
-you ``3.0``.  Even if no work is schedeuled though, you can set the clock by
+you ``3.0``.  Even if no work is scheduled though, you can set the clock by
 advancing by a specific interval:
 
 .. code-block:: python
 
    driver.advance(5000)
    print(driver.now())
```

### Comparing `fritter-0.0.8/docs/repeat.rst` & `fritter-0.0.9/docs/repeat.rst`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ================
 
 The basic form of a repeating function in Fritter has a signature that looks
 like this:
 
 .. code-block::
 
-   def work(steps: StepsT, stopper: Cancellable) -> None: ...
+   def work(steps: StepsT, scheduled: SomeScheduledCall) -> None: ...
 
 The parameters are, respectively, the *steps* that ``work`` should perform in
 this invocation, and an object with a ``.cancel()`` method that will stop the
 next iteration from occurring.
 
 Sometimes, real time moves more quickly than your code can keep up. Perhaps
 your code is slow, or you need to wait on an external system; whatever the
```

### Comparing `fritter-0.0.8/docs/repeating_example.py` & `fritter-0.0.9/docs/repeating_example.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,22 @@
-from fritter.boundaries import Cancellable
+from asyncio import run
+
+from fritter.boundaries import (
+    Cancellable,
+    PhysicalScheduler,
+)
+from fritter.drivers.asyncio import AsyncioAsyncDriver, AsyncioTimeDriver
 from fritter.repeat import Async
 from fritter.repeat.rules.seconds import EverySecond
-from fritter.drivers.asyncio import AsyncioTimeDriver, AsyncioAsyncDriver
-from fritter.scheduler import SimpleScheduler
-from asyncio import run
+from fritter.scheduler import schedulerFromDriver
 
 
 # example coroutine
 async def example() -> None:
-    scheduler = SimpleScheduler(AsyncioTimeDriver())
+    scheduler: PhysicalScheduler = schedulerFromDriver(AsyncioTimeDriver())
     repeatedly = Async(AsyncioAsyncDriver()).repeatedly
     times = 0
 
     # work function
     async def work(steps: int, stopper: Cancellable) -> None:
         nonlocal times
         times += steps
```

### Comparing `fritter-0.0.8/docs/requirements.txt` & `fritter-0.0.9/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `fritter-0.0.8/docs/simple_repeat.py` & `fritter-0.0.9/docs/simple_repeat.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from fritter.boundaries import Cancellable
+from fritter.boundaries import SomeScheduledCall
+from fritter.drivers.sleep import SleepDriver
 from fritter.repeat import repeatedly
 from fritter.repeat.rules.seconds import EverySecond
-from fritter.drivers.sleep import SleepDriver
-from fritter.scheduler import Scheduler
+from fritter.scheduler import schedulerFromDriver
 
 # driver setup
 driver = SleepDriver()
 start = driver.now()
 
 
 # repeating work
-def work(steps: int, stopper: Cancellable) -> None:
+def work(steps: int, scheduled: SomeScheduledCall) -> None:
     elapsed = driver.now() - start
     print(f"took {steps} steps at {elapsed:0.2f}")
     if elapsed >= 2.0:
-        stopper.cancel()
+        scheduled.cancel()
 
 
 # kick off scheduler
-repeatedly(Scheduler(driver), work, EverySecond(0.05))
+repeatedly(schedulerFromDriver(driver), work, EverySecond(0.05))
 steps = driver.block()
 print(f"took {steps } steps, then stopped")
```

### Comparing `fritter-0.0.8/docs/tree_example.py` & `fritter-0.0.9/docs/tree_example.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 # setup
 from typing import Callable
+
+from fritter.boundaries import PhysicalScheduler
 from fritter.drivers.memory import MemoryDriver
-from fritter.scheduler import SimpleScheduler
+from fritter.scheduler import schedulerFromDriver
 from fritter.tree import branch
 
 driver = MemoryDriver()
-trunk = SimpleScheduler(driver)
+trunk: PhysicalScheduler = schedulerFromDriver(driver)
 manager, branched = branch(trunk)
 # end setup
 
 
 # showfunc
 def show(name: str) -> Callable[[], None]:
     def _() -> None:
         print(f"{name} trunk={trunk.now()} branch={branched.now()}")
 
     return _
+
+
 # end showfunc
 
 
 # branchcalls
 branched.callAt(1.0, show("branch 1"))
 branched.callAt(2.0, show("branch 2"))
 branched.callAt(3.0, show("branch 3"))
```

### Comparing `fritter-0.0.8/docs/tree_scaling_example.py` & `fritter-0.0.9/docs/tree_scaling_example.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # setup
 from fritter.drivers.memory import MemoryDriver
-from fritter.scheduler import SimpleScheduler
+from fritter.scheduler import schedulerFromDriver
 from fritter.tree import branch, timesFaster
+from fritter.boundaries import PhysicalScheduler
 
 driver = MemoryDriver()
-trunk = SimpleScheduler(driver)
+trunk: PhysicalScheduler = schedulerFromDriver(driver)
 rate = 3.0
 manager, branched = branch(trunk, timesFaster(rate))
 # end setup
 
 
 # showfunc
-def loop(scheduler: SimpleScheduler, name: str, interval: float = 1.0) -> None:
+def loop(scheduler: PhysicalScheduler, name: str, interval: float = 1.0) -> None:
     def _() -> None:
         print(name)
         scheduler.callAt(scheduler.now() + interval, _)
 
     _()
```

### Comparing `fritter-0.0.8/docs/trees.rst` & `fritter-0.0.9/docs/trees.rst`

 * *Files identical despite different names*

### Comparing `fritter-0.0.8/pyproject.toml` & `fritter-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fritter-0.0.8/src/fritter/drivers/asyncio.py` & `fritter-0.0.9/src/fritter/drivers/asyncio.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,41 +2,50 @@
 
 """
 Implementation of L{TimeDriver} and L{AsyncDriver} for L{asyncio}.
 """
 
 from __future__ import annotations
 
-from asyncio import Future, get_event_loop
-from asyncio.events import AbstractEventLoop
+from asyncio import Future, get_event_loop, AbstractEventLoop
 from contextvars import Context
 from dataclasses import dataclass, field
 from typing import Any, Callable, Coroutine, Protocol
 
-from ..boundaries import AsyncDriver, Cancellable, PriorityQueue, TimeDriver
+from ..boundaries import (
+    AsyncDriver,
+    Cancellable,
+    PriorityQueue,
+    Scheduler,
+    TimeDriver,
+)
 from ..heap import Heap
-from ..scheduler import FutureCall, Scheduler, SimpleScheduler
+from ..scheduler import ConcreteScheduledCall, schedulerFromDriver
 
 
 class LoopTimeInterface(Protocol):
     """
-    Describe the portions of C{AbstractEventLoop} used by L{AsyncioTimeDriver}.
+    Describe the portions of L{AbstractEventLoop} used by L{AsyncioTimeDriver}.
     """
 
-    # TODO: fix code link
-
     def call_at(
         self,
         when: float,
         callback: Callable[[], None],
         *args: object,
         context: Context | None = None,
-    ) -> Cancellable: ...
+    ) -> Cancellable:
+        """
+        @see: L{AbstractEventLoop.call_at <asyncio.loop.call_at>}
+        """
 
-    def time(self) -> float: ...
+    def time(self) -> float:
+        """
+        @see: L{AbstractEventLoop.time <asyncio.loop.time>}
+        """
 
 
 @dataclass
 class AsyncioTimeDriver:
     """
     An implementation of L{TimeDriver} using an L{asyncio} event loop.
     """
@@ -80,15 +89,15 @@
     """
 
     _loop: AbstractEventLoop = field(default_factory=get_event_loop)
 
     def newWithCancel(self, cancel: Callable[[], None]) -> Future[None]:
         """
         Create a new L{Future} with the given callback to execute when
-        canceled.
+        cancelled.
         """
         f = Future[None](loop=self._loop)
 
         @f.add_done_callback
         def done(future: Future[None]) -> None:
             if f.cancelled():
                 cancel()
@@ -109,16 +118,19 @@
 
 
 _AsyncioDriverCheck: type[AsyncDriver[Future[None]]] = AsyncioAsyncDriver
 
 
 def scheduler(
     loop: LoopTimeInterface | None = None,
-    queue: PriorityQueue[FutureCall[float, Callable[[], None]]] | None = None,
-) -> SimpleScheduler:
+    queue: (
+        PriorityQueue[ConcreteScheduledCall[float, Callable[[], None], int]]
+        | None
+    ) = None,
+) -> Scheduler[float, Callable[[], None], int]:
     """
     Create a scheduler that uses Asyncio.
     """
-    return Scheduler(
+    return schedulerFromDriver(
         AsyncioTimeDriver(loop if loop is not None else get_event_loop()),
-        queue if queue is not None else Heap(),
+        queue=queue if queue is not None else Heap(),
     )
```

### Comparing `fritter-0.0.8/src/fritter/drivers/datetime.py` & `fritter-0.0.9/src/fritter/drivers/datetimes.py`

 * *Files identical despite different names*

### Comparing `fritter-0.0.8/src/fritter/drivers/memory.py` & `fritter-0.0.9/src/fritter/drivers/memory.py`

 * *Files identical despite different names*

### Comparing `fritter-0.0.8/src/fritter/drivers/sleep.py` & `fritter-0.0.9/src/fritter/drivers/sleep.py`

 * *Files identical despite different names*

### Comparing `fritter-0.0.8/src/fritter/drivers/twisted.py` & `fritter-0.0.9/src/fritter/drivers/twisted.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,22 @@
 from dataclasses import dataclass
 from typing import Any, Callable, Coroutine, Optional
 
 from twisted.internet.defer import Deferred
 from twisted.internet.interfaces import IDelayedCall, IReactorTime
 from twisted.logger import Logger
 
-from ..boundaries import AsyncDriver, PriorityQueue, TimeDriver
+from ..boundaries import (
+    AsyncDriver,
+    PhysicalScheduler,
+    PriorityQueue,
+    TimeDriver,
+)
 from ..heap import Heap
-from ..scheduler import FutureCall, Scheduler, SimpleScheduler
+from ..scheduler import ConcreteScheduledCall, schedulerFromDriver
 
 log = Logger()
 
 
 @dataclass
 class TwistedTimeDriver:
     """
@@ -66,15 +71,15 @@
     """
     Driver for Deferred-flavored awaitables.
     """
 
     def newWithCancel(self, cancel: Callable[[], None]) -> Deferred[None]:
         """
         Create a new future-ish object with the given callback to execute when
-        canceled.
+        cancelled.
         """
         return Deferred(lambda d: cancel())
 
     def complete(self, asyncObj: Deferred[None]) -> None:
         """
         The asynchronous operation completed successfully.
         """
@@ -87,20 +92,23 @@
 
 
 _AsyncDriverCheck: type[AsyncDriver[Deferred[None]]] = TwistedAsyncDriver
 
 
 def scheduler(
     reactor: IReactorTime | None = None,
-    queue: PriorityQueue[FutureCall[float, Callable[[], None]]] | None = None,
-) -> SimpleScheduler:
+    queue: (
+        PriorityQueue[ConcreteScheduledCall[float, Callable[[], None], int]]
+        | None
+    ) = None,
+) -> PhysicalScheduler:
     """
     Create a scheduler that uses Twisted.
     """
     if reactor is None:
         from twisted.internet import reactor  # type:ignore[assignment]
 
         assert reactor is not None
-    return Scheduler(
+    return schedulerFromDriver(
         TwistedTimeDriver(reactor),
-        queue if queue is not None else Heap(),
+        queue=queue if queue is not None else Heap(),
     )
```

### Comparing `fritter-0.0.8/src/fritter/heap.py` & `fritter-0.0.9/src/fritter/heap.py`

 * *Files identical despite different names*

### Comparing `fritter-0.0.8/src/fritter/repeat/__init__.py` & `fritter-0.0.9/src/fritter/repeat/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,33 +4,29 @@
 been passed so that the repeated calls may catch up to real time to preserve
 timing accuracy when timers cannot always be invoked promptly.
 """
 
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import (
-    Any,
-    Callable,
-    Coroutine,
-    Generic,
-    TypeVar,
-)
+from typing import Any, Callable, Coroutine, Generic, TypeVar
 
 from ..boundaries import (
     AsyncDriver,
     AsyncType,
     Cancellable,
-    RepeatingWork,
     RecurrenceRule,
+    RepeatingWork,
+    Scheduler,
+    SomeScheduledCall,
     StepsT,
+    StepsTInv,
+    WhatT,
+    WhenT,
 )
-from ..scheduler import Scheduler, WhatT, WhenT
-
-StepsTInv = TypeVar("StepsTInv")
 
 
 RepeatingWhatT = TypeVar("RepeatingWhatT", bound=RepeatingWork[object])
 """
 A TypeVar for L{Repeater} to reference a specific type of L{RepeatingWork}.
 """
 
@@ -58,24 +54,24 @@
 
             2. invokes this L{Repeater}'s C{repeat} method.
 
     @ivar reference: The current reference time, i.e. the time at which the
         next invocation of C{work} I{should} occur.
     """
 
-    scheduler: Scheduler[WhenT, WhatT]
+    scheduler: Scheduler[WhenT, WhatT, object]
     rule: RecurrenceRule[WhenT, StepsT]
     work: RepeatingWork[StepsT]
     convert: Callable[[Repeater[WhenT, WhatT, StepsT]], WhatT]
     reference: WhenT
 
     @classmethod
     def new(
         cls,
-        scheduler: Scheduler[WhenT, WhatT],
+        scheduler: Scheduler[WhenT, WhatT, object],
         rule: RecurrenceRule[WhenT, StepsT],
         work: RepeatingWork[StepsT],
         convert: Callable[[Repeater[WhenT, WhatT, StepsT]], WhatT],
         reference: WhenT | None = None,
     ) -> Repeater[WhenT, WhatT, StepsT]:
         """
         Create a L{Repeater}, filling out its reference time with the L{current
@@ -100,15 +96,15 @@
         callIncrement, self.reference = self.rule(self.reference, now)
         callRepeat = self.convert(self)
         stopHandle = self.scheduler.callAt(self.reference, callRepeat)
         self.work(callIncrement, stopHandle)
 
 
 def repeatedly(
-    scheduler: Scheduler[WhenT, Callable[[], None]],
+    scheduler: Scheduler[WhenT, Callable[[], None], object],
     work: RepeatingWork[StepsT],
     rule: RecurrenceRule[WhenT, StepsT],
 ) -> None:
     """
     Create a L{Repeater} and call its C{repeat} method.  This is a utility
     function for use when you have a simple repetition set up on a scheduler
     that accepts a baseline 0-argument callable, and does not require any
@@ -160,15 +156,15 @@
         return.
     """
 
     asyncDriver: AsyncDriver[AsyncType]
 
     def repeatedly(
         self,
-        scheduler: Scheduler[WhenT, Callable[[], None]],
+        scheduler: Scheduler[WhenT, Callable[[], None], object],
         rule: RecurrenceRule[WhenT, StepsTInv],
         work: Callable[
             [StepsTInv, Cancellable],
             AsyncType | Coroutine[AsyncType, Any, Any],
         ],
     ) -> AsyncType:
         """
@@ -198,16 +194,16 @@
         )
 
         def complete() -> None:
             asyncStopper.asyncInProgress = None
             if asyncStopper.timeInProgress is None and not cancelled:
                 repeater.repeat()
 
-        def kickoff(steps: StepsTInv, stopper: Cancellable) -> None:
-            asyncStopper.timeInProgress = stopper
+        def kickoff(steps: StepsTInv, scheduled: SomeScheduledCall) -> None:
+            asyncStopper.timeInProgress = scheduled
             completedSynchronously: bool = False
 
             async def coro() -> None:
                 nonlocal completedSynchronously
                 try:
                     await work(steps, asyncStopper)
                 finally:
```

### Comparing `fritter-0.0.8/src/fritter/repeat/rules/datetimes.py` & `fritter-0.0.9/src/fritter/repeat/rules/datetimes.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,31 @@
+"""
+Recurrence rules for use with L{fritter.repeat.repeatedly} which work with
+C{datetype.DateTime} objects.
+"""
+
 from dataclasses import dataclass
-from datetime import timedelta
+from datetime import timedelta, tzinfo
+from typing import TYPE_CHECKING, TypeVar
 from zoneinfo import ZoneInfo
 
-from datetime import tzinfo
 from datetype import DateTime
-from typing import TYPE_CHECKING, TypeVar
 
-from ...boundaries import RecurrenceRule, Day
+from ...boundaries import Day, RecurrenceRule
 
 DTRule = RecurrenceRule[DateTime[ZoneInfo], int]
 """
 A type alias to describe a recurrence rule function that operates on aware
-datetimes.
+datetimes and tracks an integer count of steps.
+"""
+
+EachDTRule = RecurrenceRule[DateTime[ZoneInfo], list[DateTime[ZoneInfo]]]
+"""
+A type alias to describe a recurrence rule function that operates on aware
+datetimes and tracks a list of desired elapsed occurrences as steps.
 """
 
 TZType = TypeVar("TZType", bound=tzinfo)
 
 
 @dataclass(frozen=True)
 class EveryDelta:
@@ -44,14 +54,41 @@
         nextDesired = reference
         while nextDesired <= current:
             count += 1
             nextDesired += self.delta
         return count, nextDesired
 
 
+@dataclass(frozen=True)
+class EachYear:
+    """
+    An L{EachYear} is a L{RecurrenceRule} based on a number of years between
+    two dates.
+
+    @ivar years: The number of years between recurrences
+    """
+
+    years: int
+
+    def __call__(
+        self,
+        reference: DateTime[ZoneInfo],
+        current: DateTime[ZoneInfo],
+    ) -> tuple[list[DateTime[ZoneInfo]], DateTime[ZoneInfo]]:
+        referenceDate = reference.date()
+        nextDesired = reference
+        years = []
+        while nextDesired <= current:
+            years.append(nextDesired)
+            nextDesired = nextDesired.replace(
+                year=referenceDate.year + (len(years) * self.years)
+            )
+        return years, nextDesired
+
+
 @dataclass
 class EachWeekOn:
     """
     Repeat every week, on each weekday in the given set of C{days}, at the
     given C{hour}, C{minute}, and C{second}.
     """
 
@@ -89,14 +126,19 @@
 
                 # it's after the reference *and* after the current time, we're
                 # done
                 return steps, candidate
             weekOffset += 7
 
 
+yearly: EachDTRule = EachYear(1)
+"""
+Yearly datetime-based delta.
+"""
+
 weekly: DTRule = EveryDelta(timedelta(weeks=1))
 """
 Weekly datetime-based delta.
 """
 
 daily: DTRule = EveryDelta(timedelta(days=1))
 """
@@ -104,11 +146,20 @@
 """
 
 hourly: DTRule = EveryDelta(timedelta(hours=1))
 """
 Hourly datetime-based rule.
 """
 
+
 if TYPE_CHECKING:
-    _isRule: RecurrenceRule[DateTime[ZoneInfo], list[DateTime[ZoneInfo]]] = (
-        EachWeekOn({Day.MONDAY}, 1, 1, 1)
-    )
+    _isRule: EachDTRule = EachWeekOn({Day.MONDAY}, 1, 1, 1)
+
+
+__all__ = [
+    "EveryDelta",
+    "EachWeekOn",
+    "weekly",
+    "daily",
+    "hourly",
+    "yearly",
+]
```

### Comparing `fritter-0.0.8/src/fritter/repeat/rules/seconds.py` & `fritter-0.0.9/src/fritter/repeat/rules/seconds.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,14 @@
-from dataclasses import dataclass
+"""
+Recurrence rules for use with L{fritter.repeat.repeatedly} which work with
+L{float}s representing a number of seconds as both a reference point and a
+delta between times.
+"""
 
+from dataclasses import dataclass
 from typing import TYPE_CHECKING
 
 
 @dataclass
 class EverySecond:
     """
     An L{EverySecond} is a L{RecurrenceRule} based on a L{float} timestamp,
```

### Comparing `fritter-0.0.8/src/fritter/test/test_asyncio.py` & `fritter-0.0.9/src/fritter/test/test_asyncio.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from asyncio.events import new_event_loop
 from asyncio.exceptions import CancelledError, InvalidStateError
 from contextvars import Context
 from dataclasses import dataclass
-from typing import Callable
+from typing import Any, Callable
 from unittest import TestCase
 
 from twisted.internet.task import Clock
 
 from ..boundaries import Cancellable
 from ..drivers.asyncio import AsyncioAsyncDriver, AsyncioTimeDriver, scheduler
 
@@ -180,9 +180,9 @@
 
         sched.callAt(50, hello)
         self.assertEqual(stuff, [])
         clock.advance(60)
         self.assertEqual(stuff, ["hello"])
 
     def test_schedulerDefaults(self) -> None:
-        sched = scheduler()
+        sched: Any = scheduler()
         self.assertIsInstance(sched.driver, AsyncioTimeDriver)
```

### Comparing `fritter-0.0.8/src/fritter/test/test_json.py` & `fritter-0.0.9/src/fritter/test/test_json.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,114 +1,162 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from datetime import datetime, timedelta
 from json import dumps, loads
 from pathlib import Path
 from tempfile import mkdtemp
-from typing import Any, Type
+from typing import Any, Callable, Type
 from unittest import TestCase
 from zoneinfo import ZoneInfo
 
 from datetype import DateTime, aware
-from fritter.persistent.json import schedulerAtPath
 
-from ..boundaries import Cancellable, TimeDriver
-from ..drivers.datetime import DateTimeDriver
+from ..boundaries import (
+    Cancellable,
+    RecurrenceRule,
+    ScheduledCall,
+    ScheduledState,
+    SomeScheduledCall,
+    TimeDriver,
+)
+from ..drivers.datetimes import DateTimeDriver
 from ..drivers.memory import MemoryDriver
-from ..persistent.json import (
+from ..persistent.jsonable import (
     JSONableCallable,
     JSONableInstance,
+    JSONableRepeatable,
     JSONableScheduler,
     JSONObject,
     JSONRegistry,
     LoadProcess,
     MissingPersistentCall,
+    schedulerAtPath,
 )
-from ..repeat.rules.datetimes import daily
-from ..scheduler import FutureCall
+from ..repeat.rules.datetimes import EachYear, daily
 
 
 @dataclass
 class RegInfo:
-    calls: list[str]
+    madeCalls: list[str]
     identityMap: dict[str, Any] = field(default_factory=dict)
+    lookupLater: list[LaterStopper] = field(default_factory=list)
 
 
 registry = JSONRegistry[RegInfo]()
 emptyRegistry = JSONRegistry[RegInfo]()
 PT = ZoneInfo(key="America/Los_Angeles")
 
-calls = []
+globalCalls = []
 
 
 @registry.function
 def call1() -> None:
-    calls.append("hello")
+    globalCalls.append("hello")
 
 
 @registry.function
 def call2() -> None:
-    calls.append("goodbye")
+    globalCalls.append("goodbye")
 
 
 @registry.repeatFunction
-def repeatable(steps: int, stopper: Cancellable) -> None:
-    calls.append(f"repeatable {steps}")
+def repeatable(steps: int, scheduled: SomeScheduledCall) -> None:
+    globalCalls.append(f"repeatable {steps}")
 
 
 @dataclass
 class InstanceWithMethods:
     value: str
     info: RegInfo
-    calls: int = 0
+    callCount: int = 0
     stoppers: list[Cancellable] = field(default_factory=list)
 
     @classmethod
     def typeCodeForJSON(self) -> str:
         return "instanceWithMethods"
 
     @classmethod
     def fromJSON(
         cls, load: LoadProcess[RegInfo], json: JSONObject
     ) -> InstanceWithMethods:
         key = json["identity"]
-        if key in load.context.identityMap:
-            load.context.calls.append("InstanceWithMethods.fromJSON (cached)")
-            self: InstanceWithMethods = load.context.identityMap[key]
+        if key in load.bootstrap.identityMap:
+            load.bootstrap.madeCalls.append(
+                f"InstanceWithMethods.fromJSON: {json['value']} (cached)"
+            )
+            self: InstanceWithMethods = load.bootstrap.identityMap[key]
             return self
-        load.context.calls.append("InstanceWithMethods.fromJSON")
-        new = cls(json["value"], load.context)
-        load.context.identityMap[key] = new
+        load.bootstrap.madeCalls.append(
+            f"InstanceWithMethods.fromJSON: {json['value']}"
+        )
+        new = cls(json["value"], load.bootstrap)
+        load.bootstrap.identityMap[key] = new
         return new
 
     def toJSON(self, registry: JSONRegistry[RegInfo]) -> dict[str, object]:
         return {
             "value": self.value,
             "identity": id(self),
         }
 
     @registry.method
     def method1(self) -> None:
-        self.info.calls.append(f"{self.value}/method1")
+        self.info.madeCalls.append(f"{self.value}/method1")
 
     @registry.method
     def method2(self) -> None:
-        self.info.calls.append(f"{self.value}/method2")
+        self.info.madeCalls.append(f"{self.value}/method2")
 
     @registry.repeatMethod
-    def repeatMethod(self, steps: int, stopper: Cancellable) -> None:
-        self.calls += 1
-        self.stoppers.append(stopper)
-        self.info.calls.append(
-            f"repeatMethod {steps} {self.value=} {self.calls=}"
+    def repeatMethod(self, steps: int, scheduled: SomeScheduledCall) -> None:
+        self.callCount += 1
+        self.stoppers.append(scheduled)
+        self.info.madeCalls.append(
+            f"repeatMethod {steps} {self.value=} {self.callCount=}"
+        )
+
+    @registry.repeatMethod
+    def repeatMethodDTZIL(
+        self, steps: list[DateTime[ZoneInfo]], scheduled: SomeScheduledCall
+    ) -> None:
+        self.callCount += 1
+        self.stoppers.append(scheduled)
+        self.info.madeCalls.append(
+            f"repeatMethod {steps} {self.value=} {self.callCount=}"
         )
 
 
-Handle = FutureCall[DateTime[ZoneInfo], JSONableCallable[RegInfo]]
+Handle = ScheduledCall[DateTime[ZoneInfo], JSONableCallable[RegInfo], int]
+
+
+@dataclass
+class LaterStopper:
+    handle: Handle
+
+    @registry.method
+    def stop(self) -> None:
+        self.handle.cancel()
+
+    @classmethod
+    def typeCodeForJSON(self) -> str:
+        return "later-stopper"
+
+    def toJSON(self, registry: JSONRegistry[RegInfo]) -> dict[str, object]:
+        return {
+            "value": registry.saveScheduledCall(self.handle),
+        }
+
+    @classmethod
+    def fromJSON(
+        cls, load: LoadProcess[RegInfo], json: JSONObject
+    ) -> LaterStopper:
+        new = cls(load.loadScheduledCall(json["value"]))
+        load.bootstrap.lookupLater.append(new)
+        return new
 
 
 @dataclass
 class Stoppable:
     runcall: Handle | None = None
     stopcall: Handle | None = None
     ran: bool = False
@@ -126,42 +174,48 @@
 
     @classmethod
     def typeCodeForJSON(self) -> str:
         return "stoppable"
 
     def toJSON(self, registry: JSONRegistry[RegInfo]) -> dict[str, object]:
         def save(it: Handle | None) -> object:
-            return registry.saveFutureCall(it) if it is not None else it
+            return registry.saveScheduledCall(it) if it is not None else it
 
         return {
             "runcall": save(self.runcall),
             "stopcall": save(self.stopcall),
             "ran": self.ran,
             "id": id(self),
         }
 
     @classmethod
     def fromJSON(
         cls, load: LoadProcess[RegInfo], json: JSONObject
     ) -> Stoppable:
-        if json["id"] in load.context.identityMap:
-            result: Stoppable = load.context.identityMap[json["id"]]
+        ckey = json["id"]
+        if ckey in load.bootstrap.identityMap:
+            result: Stoppable = load.bootstrap.identityMap[ckey]
             return result
 
         def get(
             name: str,
         ) -> Handle | None:
             it = json[name]
-            return it if it is None else load.loadFutureCall(it)
+            assert it is not None
+            loaded = load.loadScheduledCall(it)
+            assert loaded.state is ScheduledState.pending
+            return loaded
 
         self = cls(
-            runcall=get("runcall"), stopcall=get("stopcall"), ran=json["ran"]
+            runcall=get("runcall"),
+            stopcall=get("stopcall"),
+            ran=json["ran"],
         )
         # leave it there for the test to pick up
-        load.context.identityMap[json["id"]] = self
+        load.bootstrap.identityMap[ckey] = self
         return self
 
     @registry.method
     def stopme(self) -> None:
         assert self.runcall is not None
         self.stopcall = None
         self.runcall.cancel()
@@ -172,186 +226,274 @@
         self.ran = True
         self.runcall = None
 
 
 stp: Type[JSONableInstance[RegInfo]] = Stoppable
 
 
-def jsonScheduler(driver: TimeDriver[float]) -> JSONableScheduler[RegInfo]:
-    return registry.new(DateTimeDriver(driver))
+def jsonScheduler(
+    driver: TimeDriver[float],
+) -> tuple[JSONableScheduler[RegInfo], Callable[[], JSONObject]]:
+    return registry.createScheduler(DateTimeDriver(driver))
 
 
 class PersistentSchedulerTests(TestCase):
     def tearDown(self) -> None:
-        del calls[:]
+        del globalCalls[:]
 
     def test_scheduleRunSaveRun(self) -> None:
         """
         Test scheduling module-level functions and instance methods.
         """
         memoryDriver = MemoryDriver()
-        scheduler = jsonScheduler(memoryDriver)
+        scheduler, saver = jsonScheduler(memoryDriver)
         dt = aware(
             datetime(2023, 7, 21, 1, 1, 1, tzinfo=PT),
             ZoneInfo,
         )
         dt2 = aware(
             datetime(2023, 7, 22, 1, 1, 1, tzinfo=PT),
             ZoneInfo,
         )
         ri0 = RegInfo([])
-        iwm = InstanceWithMethods("test_scheduleRunSaveRun value", ri0)
+        iwm = InstanceWithMethods("test_scheduleRunSaveRun-value", ri0)
         scheduler.callAt(dt, call1)
         scheduler.callAt(dt, iwm.method1)
         scheduler.callAt(dt2, call2)
         scheduler.callAt(dt2, iwm.method2)
         memoryDriver.advance(dt.timestamp() + 1)
-        self.assertEqual(calls, ["hello"])
-        del calls[:]
-        saved = registry.save(scheduler)
+        self.assertEqual(globalCalls, ["hello"])
+        del globalCalls[:]
+        saved = saver()
         memory2 = MemoryDriver()
         ri = RegInfo([])
-        registry.load(memory2, saved, ri)
+        registry.loadScheduler(DateTimeDriver(memory2), saved, ri)
         memory2.advance(dt2.timestamp() + 1)
-        self.assertEqual(calls, ["goodbye"])
-        self.assertEqual(ri0.calls, ["test_scheduleRunSaveRun value/method1"])
+        self.assertEqual(globalCalls, ["goodbye"])
+        self.assertEqual(
+            ri0.madeCalls, ["test_scheduleRunSaveRun-value/method1"]
+        )
         self.assertEqual(
-            ri.calls,
+            ri.madeCalls,
             [
-                "InstanceWithMethods.fromJSON",
-                "test_scheduleRunSaveRun value/method2",
+                "InstanceWithMethods.fromJSON: test_scheduleRunSaveRun-value",
+                "test_scheduleRunSaveRun-value/method2",
             ],
         )
 
     def test_persistCancellers(self) -> None:
         """
         scheduled instance methods ought to be able to save handles to other
         instances and stuff
         """
         memoryDriver = MemoryDriver()
-        scheduler = jsonScheduler(memoryDriver)
+        scheduler, saver = jsonScheduler(memoryDriver)
         dt = aware(datetime(2023, 7, 21, 1, 1, 1, tzinfo=PT), ZoneInfo)
         memoryDriver.advance(dt.timestamp() + 1)
         s = Stoppable()
         self.assertEqual(s.ran, False)
         s.runme()
         self.assertEqual(s.ran, True)
 
         s = Stoppable()
         s.scheduleme(scheduler)
-        jsonobj = dumps(registry.save(scheduler))
+        assert s.runcall is not None
+        assert s.stopcall is not None
+        s2 = LaterStopper(s.runcall)
+        s3 = LaterStopper(s.stopcall)
+        s4 = LaterStopper(s.runcall)
+        s5 = LaterStopper(s.stopcall)
+        scheduler.callAt(
+            aware(datetime(2029, 1, 1, tzinfo=PT), ZoneInfo), s2.stop
+        )
+        scheduler.callAt(
+            aware(datetime(2029, 1, 2, tzinfo=PT), ZoneInfo), s3.stop
+        )
+        scheduler.callAt(
+            aware(datetime(2029, 1, 3, tzinfo=PT), ZoneInfo), s4.stop
+        )
+        last = scheduler.callAt(
+            aware(datetime(2029, 1, 4, tzinfo=PT), ZoneInfo), s5.stop
+        )
+        scheduler.callAt(
+            aware(datetime(2029, 1, 5, tzinfo=PT), ZoneInfo),
+            LaterStopper(last).stop,
+        )
+        jsonobj = dumps(saver())
         saved = loads(jsonobj)
         memory2 = MemoryDriver()
         ri = RegInfo([])
-        registry.load(memory2, saved, ri)
+        registry.loadScheduler(DateTimeDriver(memory2), saved, ri)
+        [run1, stop1, run2, stop2, loadedLast] = ri.lookupLater
+        self.assertEqual(run1.handle.state, ScheduledState.pending)
         [(name, loadedStoppable)] = ri.identityMap.items()
         assert isinstance(loadedStoppable, Stoppable)
         self.assertEqual(loadedStoppable.ran, False)
-        self.assertIsNot(loadedStoppable.runcall, None)
-        memory2.advance(dt.timestamp() + 3.0)
+        rc = loadedStoppable.runcall
+        sc = loadedStoppable.stopcall
+        assert rc is not None
+        assert sc is not None
+        self.assertEqual(rc.state, ScheduledState.pending)
+        self.assertEqual(
+            rc.when,
+            datetime(2023, 7, 21, 8, 1, 4, tzinfo=ZoneInfo(key="Etc/UTC")),
+        )
+        self.assertIsNot(rc.what, None)
+        self.assertEqual(rc.id, 0)
+        memory2.advance(dt.timestamp() + 4.0)
         self.assertEqual(loadedStoppable.ran, False)
         self.assertIs(loadedStoppable.runcall, None)
+        self.assertEqual(rc.state, ScheduledState.cancelled)
+        self.assertEqual(loadedLast.handle.state, ScheduledState.pending)
+        loadedLast.stop()
+        self.assertEqual(loadedLast.handle.state, ScheduledState.cancelled)
+
+        # These are loaded reentrantly and cannot be identical, but they map
+        # their IDs and are the same
+        self.assertEqual(rc.id, run1.handle.id)
+        self.assertEqual(sc.id, stop1.handle.id)
+
+        # all references not loaded reentrantly are exactly identical
+        self.assertIs(run1.handle, run2.handle)
+        self.assertEqual(run1.handle.state, ScheduledState.cancelled)
+        self.assertIs(stop1.handle, stop2.handle)
 
     def test_schedulerAtPath(self) -> None:
         ri0 = RegInfo([])
         iwm = InstanceWithMethods("A", ri0)
         mem = MemoryDriver()
         p = Path(mkdtemp()) / "scheduler.json"
         ts = datetime(2024, 2, 1, tzinfo=ZoneInfo("Etc/UTC")).timestamp()
         mem.advance(ts)
         aw = aware(datetime(2024, 2, 2, tzinfo=ZoneInfo("Etc/UTC")), ZoneInfo)
-        with schedulerAtPath(registry, mem, p, ri0) as sched1:
+        with schedulerAtPath(registry, DateTimeDriver(mem), p, ri0) as sched1:
             sched1.callAt(aw, iwm.method1)
         ri1 = RegInfo([])
         mem2 = MemoryDriver()
-        with schedulerAtPath(registry, mem2, p, ri1):
+        with schedulerAtPath(registry, DateTimeDriver(mem2), p, ri1):
             mem2.advance()
         self.assertEqual(
-            ri1.calls, ["InstanceWithMethods.fromJSON", "A/method1"]
+            ri1.madeCalls, ["InstanceWithMethods.fromJSON: A", "A/method1"]
         )
 
     def test_noSuchCallID(self) -> None:
         mem = MemoryDriver()
         with self.assertRaises(MissingPersistentCall) as raised:
-            registry.load(
-                mem,
+            registry.loadScheduler(
+                DateTimeDriver(mem),
                 {
                     "scheduledCalls": [
                         {
                             "when": "2023-07-21T08:01:03",
                             "tz": "Etc/UTC",
                             "what": {
                                 "type": "stoppable.stopme",
                                 "data": {
                                     "runcall": {"id": 7},
                                     "stopcall": {"id": 2},
                                     "ran": False,
                                     "id": 4411099664,
                                 },
                             },
-                            "called": False,
-                            "canceled": False,
                             "id": 2,
                         }
                     ],
                     "counter": "2",
                 },
                 RegInfo([]),
             )
         self.assertEqual(raised.exception.args[0], 7)
 
     def test_idling(self) -> None:
         memoryDriver = MemoryDriver()
-        scheduler = jsonScheduler(memoryDriver)
+        scheduler, saver = jsonScheduler(memoryDriver)
         dt = aware(
             datetime(2023, 7, 21, 1, 1, 1, tzinfo=PT),
             ZoneInfo,
         )
         handle = scheduler.callAt(dt, call1)
         self.assertEqual(memoryDriver.isScheduled(), True)
         handle.cancel()
         self.assertEqual(memoryDriver.isScheduled(), False)
         memoryDriver.advance(dt.timestamp() + 1)
-        self.assertEqual(calls, [])
+        self.assertEqual(globalCalls, [])
 
     def test_emptyScheduler(self) -> None:
         memory = MemoryDriver()
-        registry.load(memory, {"scheduledCalls": []}, RegInfo([]))
+        registry.loadScheduler(
+            DateTimeDriver(memory), {"scheduledCalls": []}, RegInfo([])
+        )
         self.assertEqual(memory.isScheduled(), False)
 
     def test_repeatable(self) -> None:
         dt = aware(
             datetime(2023, 7, 21, 1, 1, 1, tzinfo=PT),
             ZoneInfo,
         )
         memoryDriver = MemoryDriver()
         memoryDriver.advance(dt.timestamp())
-        scheduler = jsonScheduler(memoryDriver)
+        scheduler, saver = jsonScheduler(memoryDriver)
         registry.repeatedly(scheduler, daily, repeatable, dt)
-        self.assertEqual(calls, ["repeatable 1"])
-        del calls[:]
+        self.assertEqual(globalCalls, ["repeatable 1"])
+        del globalCalls[:]
 
         def days(n: int) -> float:
             return 60 * 60 * 24 * n
 
         memoryDriver.advance(days(3))
-        self.assertEqual(calls, ["repeatable 3"])
-        del calls[:]
+        self.assertEqual(globalCalls, ["repeatable 3"])
+        del globalCalls[:]
 
         newInfo = RegInfo([])
         mem2 = MemoryDriver()
         mem2.advance(dt.timestamp())
         mem2.advance(days(7))
         self.assertEqual(mem2.isScheduled(), False)
-        registry.load(mem2, loads(dumps(registry.save(scheduler))), newInfo)
+        registry.loadScheduler(
+            DateTimeDriver(mem2), loads(dumps(saver())), newInfo
+        )
         self.assertEqual(mem2.isScheduled(), True)
         amount = mem2.advance()
         assert amount is not None
         self.assertLess(amount, 0.0001)
-        self.assertEqual(calls, ["repeatable 4"])
+        self.assertEqual(globalCalls, ["repeatable 4"])
+
+    def test_repeatEachYear(self) -> None:
+        memoryDriver = MemoryDriver()
+        dt = aware(
+            datetime(2023, 7, 21, 1, 1, 1, tzinfo=PT),
+            ZoneInfo,
+        )
+        scheduler: JSONableScheduler[RegInfo]
+        scheduler, saver = jsonScheduler(memoryDriver)
+        ri = RegInfo([])
+        iwm = InstanceWithMethods("test_repeatEachYear", ri)
+        rrule: RecurrenceRule[DateTime[ZoneInfo], list[DateTime[ZoneInfo]]] = (
+            EachYear(2)
+        )
+        repeatMethod: JSONableRepeatable[RegInfo, list[DateTime[ZoneInfo]]] = (
+            iwm.repeatMethodDTZIL
+        )
+        registry.repeatedly(scheduler, rrule, repeatMethod, dt)
+        newInfo = RegInfo([])
+        mem2 = MemoryDriver()
+        mem2.advance(dt.timestamp())
+        registry.loadScheduler(
+            DateTimeDriver(mem2), loads(dumps(saver())), newInfo
+        )
+        mem2.advance(timedelta(days=365 * 4).total_seconds())
+        LA = "zoneinfo.ZoneInfo(key='America/Los_Angeles')"
+        expectedCalls = [
+            "InstanceWithMethods.fromJSON: test_repeatEachYear",
+            "repeatMethod ["
+            f"datetime.datetime(2023, 7, 21, 1, 1, 1, tzinfo={LA}), "
+            f"datetime.datetime(2025, 7, 21, 1, 1, 1, tzinfo={LA})"
+            "] self.value='test_repeatEachYear' self.callCount=1",
+        ]
+        self.assertEqual(newInfo.madeCalls, expectedCalls)
 
     def test_repeatLoadError(self) -> None:
         dt = aware(
             datetime(2023, 7, 21, 1, 1, 1, tzinfo=PT),
             ZoneInfo,
         )
         memoryDriver = MemoryDriver()
@@ -374,20 +516,20 @@
                             "value": "sample",
                             "identity": 4335201296,
                         },
                     },
                 },
             },
             "called": False,
-            "canceled": False,
+            "cancelled": False,
             "id": 1,
         }
         with self.assertRaises(KeyError) as ke:
-            registry.load(
-                memoryDriver,
+            registry.loadScheduler(
+                DateTimeDriver(memoryDriver),
                 {
                     "scheduledCalls": [oneCall],
                     "counter": "1",
                 },
                 RegInfo([]),
             )
         self.assertEqual(
@@ -398,76 +540,81 @@
     def test_repeatableMethod(self) -> None:
         dt = aware(
             datetime(2023, 7, 21, 1, 1, 1, tzinfo=PT),
             ZoneInfo,
         )
         memoryDriver = MemoryDriver()
         memoryDriver.advance(dt.timestamp())
-        scheduler = jsonScheduler(memoryDriver)
+        scheduler, saver = jsonScheduler(memoryDriver)
         info = RegInfo([])
         inst = InstanceWithMethods("sample", info)
         method = inst.repeatMethod
         shared = InstanceWithMethods("shared", info)
         registry.repeatedly(scheduler, daily, method)
         registry.repeatedly(scheduler, daily, shared.repeatMethod)
         registry.repeatedly(scheduler, daily, shared.repeatMethod)
         self.assertEqual(
-            info.calls,
+            info.madeCalls,
             [
-                "repeatMethod 1 self.value='sample' self.calls=1",
-                "repeatMethod 1 self.value='shared' self.calls=1",
-                "repeatMethod 1 self.value='shared' self.calls=2",
+                "repeatMethod 1 self.value='sample' self.callCount=1",
+                "repeatMethod 1 self.value='shared' self.callCount=1",
+                "repeatMethod 1 self.value='shared' self.callCount=2",
             ],
         )
-        del info.calls[:]
+        del info.madeCalls[:]
 
         def days(n: int) -> float:
             return 60 * 60 * 24 * n
 
         memoryDriver.advance(days(3))
-        self.assertEqual(
-            info.calls,
-            [
-                "repeatMethod 3 self.value='sample' self.calls=2",
-                "repeatMethod 3 self.value='shared' self.calls=3",
-                "repeatMethod 3 self.value='shared' self.calls=4",
-            ],
-        )
+        expected = [
+            "repeatMethod 3 self.value='sample' self.callCount=2",
+            "repeatMethod 3 self.value='shared' self.callCount=3",
+            "repeatMethod 3 self.value='shared' self.callCount=4",
+        ]
+
+        self.assertEqual(info.madeCalls, expected)
 
         newInfo = RegInfo([])
         newNewInfo = RegInfo([])
 
         def atTimeDriver() -> MemoryDriver:
             x = MemoryDriver()
             x.advance(dt.timestamp())
             x.advance(days(7))
             return x
 
         mem2 = atTimeDriver()
         mem3 = atTimeDriver()
 
         self.assertEqual(mem2.isScheduled(), False)
-        persistent = dumps(registry.save(scheduler))
-        loadedScheduler = registry.load(mem2, loads(persistent), newInfo)
-        repersistent = dumps(registry.save(loadedScheduler))
-        registry.load(mem3, loads(repersistent), newNewInfo)
+        persistent = dumps(saver())
+        loadedScheduler, saver2 = registry.loadScheduler(
+            DateTimeDriver(mem2), loads(persistent), newInfo
+        )
+        repersistent = dumps(saver2())
+        registry.loadScheduler(
+            DateTimeDriver(mem3), loads(repersistent), newNewInfo
+        )
         loaded = loads(persistent)
         with self.assertRaises(KeyError):
             # TODO: allow for better error handling that doesn't just blow up
             # on the type code lookup failure
-            emptyRegistry.load(MemoryDriver(), loaded, newInfo)
+            emptyRegistry.loadScheduler(
+                DateTimeDriver(MemoryDriver()), loaded, newInfo
+            )
         self.assertEqual(mem2.isScheduled(), True)
         mem2.advance()
         expectedCalls = [
-            "InstanceWithMethods.fromJSON",
-            "InstanceWithMethods.fromJSON",
-            "InstanceWithMethods.fromJSON (cached)",
-            "repeatMethod 4 self.value='sample' self.calls=1",
-            "repeatMethod 4 self.value='shared' self.calls=1",
-            "repeatMethod 4 self.value='shared' self.calls=2",
+            "InstanceWithMethods.fromJSON: sample",
+            "InstanceWithMethods.fromJSON: shared",
+            "InstanceWithMethods.fromJSON: shared (cached)",
+            "repeatMethod 4 self.value='sample' self.callCount=1",
+            "repeatMethod 4 self.value='shared' self.callCount=1",
+            "repeatMethod 4 self.value='shared' self.callCount=2",
         ]
-        self.assertEqual(newInfo.calls, expectedCalls)
+        self.assertEqual(newInfo.madeCalls, expectedCalls)
         self.assertEqual(mem3.isScheduled(), True)
         mem3.advance()
-        self.assertEqual(newNewInfo.calls, expectedCalls)
+        self.assertEqual(newNewInfo.madeCalls, expectedCalls)
 
         # round trip:
```

### Comparing `fritter-0.0.8/src/fritter/test/test_pq.py` & `fritter-0.0.9/src/fritter/test/test_pq.py`

 * *Files identical despite different names*

### Comparing `fritter-0.0.8/src/fritter/test/test_repeat.py` & `fritter-0.0.9/src/fritter/test/test_repeat.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,46 @@
 from datetime import datetime
 from itertools import chain
 from typing import Any, Callable
 from unittest import TestCase
 from zoneinfo import ZoneInfo
 
-from datetype import DateTime
+from datetype import DateTime, aware
 from twisted.internet.defer import CancelledError, Deferred, succeed
 
-from ..boundaries import Cancellable, Day, RecurrenceRule
-from ..drivers.datetime import DateTimeDriver
+from ..boundaries import (
+    Cancellable,
+    Day,
+    RecurrenceRule,
+    Scheduler,
+    SomeScheduledCall,
+)
+from ..drivers.datetimes import DateTimeDriver
 from ..drivers.memory import MemoryDriver
 from ..drivers.twisted import TwistedAsyncDriver
 from ..repeat import Async, repeatedly
-from ..repeat.rules.datetimes import EachWeekOn
+from ..repeat.rules.datetimes import EachDTRule, EachWeekOn, EachYear
 from ..repeat.rules.seconds import EverySecond
-from ..scheduler import Scheduler
+from ..scheduler import schedulerFromDriver
+
+TZ = ZoneInfo("America/Los_Angeles")
 
 
 class RepeatTestCase(TestCase):
     def test_synchronous(self) -> None:
         mem = MemoryDriver()
         calls = []
 
-        def work(steps: int, stopper: Cancellable) -> None:
+        def work(steps: int, scheduled: SomeScheduledCall) -> None:
             now = mem.now()
             if mem.now() >= 10.0:
-                stopper.cancel()
+                scheduled.cancel()
             calls.append((steps, now))
 
-        repeatedly(Scheduler(mem), work, EverySecond(5))
+        repeatedly(schedulerFromDriver(mem), work, EverySecond(5))
 
         self.assertTrue(mem.isScheduled())
         self.assertEqual(calls, [(1, 0.0)])
         calls = []
         mem.advance()
         self.assertTrue(mem.isScheduled())
         self.assertEqual(calls, [(1, 5.0)])
@@ -53,15 +61,15 @@
             calls.append(f"before {count} ({times})")
             event = Deferred()
             await event
             calls.append(f"after {count}")
             count += 1
 
         Async(tad).repeatedly(
-            Scheduler(mem),
+            schedulerFromDriver(mem),
             EverySecond(15),
             lambda times, stopper: tick(times),
         )
 
         self.assertEqual(calls, ["before 0 (1)"])
         event.callback(None)
         self.assertEqual(calls, ["before 0 (1)", "after 0"])
@@ -92,15 +100,17 @@
 
         tad = TwistedAsyncDriver()
         mem = MemoryDriver()
         done = False
 
         async def task() -> None:
             nonlocal done
-            await Async(tad).repeatedly(Scheduler(mem), EverySecond(1), step)
+            await Async(tad).repeatedly(
+                schedulerFromDriver(mem), EverySecond(1), step
+            )
             done = True
 
         tad.runAsync(task())
         for ignored in range(threshold):
             mem.advance()
         self.assertTrue(done)
         self.assertEqual(count, threshold)
@@ -108,18 +118,18 @@
     def test_cancel(self) -> None:
         tad = TwistedAsyncDriver()
         mem = MemoryDriver()
         succeeding: int = 0
         repeatCall: Deferred[None] | None = None
         pending: Deferred[None]
 
-        def canceled(d: Deferred[None]) -> None:
+        def cancelled(d: Deferred[None]) -> None:
             return
 
-        pending = Deferred(canceled)
+        pending = Deferred(cancelled)
 
         async def bonk(d: Deferred[None]) -> None:
             # odd idiom for suppressing cancellation to work around
             # https://github.com/nedbat/coveragepy/issues/1595#issuecomment-1931494916
             await d.addErrback(lambda e: e.trap(CancelledError))
 
         async def asynchronously() -> None:
@@ -132,15 +142,15 @@
 
         async def synchronously() -> None:
             pass
 
         def go(how: Callable[[], Any]) -> None:
             nonlocal repeatCall
             repeatCall = Async(tad).repeatedly(
-                Scheduler(mem),
+                schedulerFromDriver(mem),
                 EverySecond(1),
                 lambda times, stopper: how(),
             )
 
         async def run(how: Callable[[], Any]) -> None:
             go(how)
             assert repeatCall is not None, "repeatCall should already be set"
@@ -148,21 +158,21 @@
 
         tad.runAsync(run(asynchronously))
         self.assertTrue(mem.isScheduled())
         assert repeatCall is not None
 
         repeatCall.cancel()
         self.assertFalse(mem.isScheduled())
-        pending = Deferred(canceled)
+        pending = Deferred(cancelled)
         succeeding += 1
         tad.runAsync(run(asynchronously))
         self.assertTrue(mem.isScheduled())
         mem.advance()
         self.assertFalse(mem.isScheduled())
-        p, pending = pending, Deferred(canceled)
+        p, pending = pending, Deferred(cancelled)
         p.callback(None)
         self.assertTrue(mem.isScheduled())
         mem.advance()
         repeatCall.cancel()
         tad.runAsync(run(synchronously))
         self.assertTrue(mem.isScheduled())
         repeatCall.cancel()
@@ -173,17 +183,18 @@
         L{EachWeekOn} provides a recurrence on custom weekdays at custom
         times.
         """
         tad = TwistedAsyncDriver()
         mem = MemoryDriver()
         mem.advance(1706826915.372823)
 
-        TZ = ZoneInfo("America/Los_Angeles")
         dtd = DateTimeDriver(mem, TZ)
-        sch = Scheduler[DateTime[ZoneInfo], Callable[[], None]](dtd)
+        sch: Scheduler[DateTime[ZoneInfo], Callable[[], None], int] = (
+            schedulerFromDriver(dtd)
+        )
         x = []
 
         async def record(
             steps: list[DateTime[ZoneInfo]], stopper: Cancellable
         ) -> None:
             x.append((sch.now(), steps, stopper))
 
@@ -225,10 +236,31 @@
         bigSkip = [
             *[
                 datetime(2024, 2, n, 15, 10, tzinfo=TZ)
                 for n in [12, 14, 16, 19, 21, 23, 26, 28]
             ],
             *[datetime(2024, 3, n, 15, 10, tzinfo=TZ) for n in [1, 4]],
         ]
-        self.maxDiff = 99999
         actual = list(chain(*[tries for (_, tries, _) in rest]))
         self.assertEqual(bigSkip, actual)
+
+    def test_eachYear(self) -> None:
+        """
+        L{EachYear} is a recurrence rule that repeats each year and records the
+        intervening steps as a list of DateType[ZoneInfo].
+        """
+        rule: EachDTRule = EachYear(3)
+        [steps, newReference] = rule(
+            aware(datetime(2020, 12, 11, 9, 0, tzinfo=TZ), ZoneInfo),
+            aware(datetime(2026, 3, 10, 9, 0, tzinfo=TZ), ZoneInfo),
+        )
+        self.assertEqual(
+            newReference,
+            aware(datetime(2026, 12, 11, 9, 0, tzinfo=TZ), ZoneInfo),
+        )
+        self.assertEqual(
+            steps,
+            [
+                aware(datetime(2020, 12, 11, 9, 0, tzinfo=TZ), ZoneInfo),
+                aware(datetime(2023, 12, 11, 9, 0, tzinfo=TZ), ZoneInfo),
+            ],
+        )
```

### Comparing `fritter-0.0.8/src/fritter/test/test_scheduler.py` & `fritter-0.0.9/src/fritter/test/test_scheduler.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,64 +1,74 @@
 from typing import Callable
 from unittest import TestCase
 
+from ..boundaries import ScheduledState, Scheduler, PhysicalScheduler
 from ..drivers.memory import MemoryDriver
-from ..heap import Heap
-from ..scheduler import FutureCall, SimpleScheduler
+from ..scheduler import schedulerFromDriver
 
 
 class SchedulerTests(TestCase):
     """
     Tests for L{Scheduler}.
     """
 
     def test_schedulingSimple(self) -> None:
         """
         Scheduling a call
         """
         driver = MemoryDriver()
-        scheduler = SimpleScheduler(driver)
+        scheduler: PhysicalScheduler = schedulerFromDriver(driver)
         called = 0
 
         def callme() -> None:
             nonlocal called
             called += 1
 
         handle = scheduler.callAt(1.0, callme)
         scheduler.callAt(3.0, callme)
         self.assertEqual(0, called)
         driver.advance(2.0)
         self.assertEqual(1, called)
-        self.assertEqual(handle.called, True)
+        self.assertEqual(handle.state, ScheduledState.called)
         handle.cancel()  # no-op
 
     def test_moveSooner(self) -> None:
         driver = MemoryDriver()
-        scheduler = SimpleScheduler(driver)
+        scheduler: Scheduler[float, Callable[[], None], int] = (
+            schedulerFromDriver(driver)
+        )
         called = 0
 
         def callme() -> None:
             nonlocal called
             called += 1
 
-        scheduler.callAt(1.0, callme)
-        scheduler.callAt(0.5, callme)
+        first = scheduler.callAt(1.0, callme)
+        second = scheduler.callAt(0.5, callme)
+        self.assertEqual(first.state, ScheduledState.pending)
+        self.assertEqual(second.state, ScheduledState.pending)
         self.assertEqual(0, called)
         driver.advance(0.3)
         self.assertEqual(0, called)
         driver.advance(0.3)
+        self.assertEqual(first.state, ScheduledState.pending)
+        self.assertEqual(second.state, ScheduledState.called)
         self.assertEqual(1, called)
         driver.advance(0.6)
         self.assertEqual(2, called)
+        self.assertEqual(first.state, ScheduledState.called)
+        self.assertEqual(second.state, ScheduledState.called)
 
     def test_canceling(self) -> None:
         """
         CallHandle.cancel() cancels an outstanding call.
         """
-        scheduler = SimpleScheduler(driver := MemoryDriver())
+        scheduler: Scheduler[float, Callable[[], None], int] = (
+            schedulerFromDriver(driver := MemoryDriver())
+        )
         callTimes = []
 
         def record(event: str) -> Callable[[], None]:
             def result() -> None:
                 callTimes.append((scheduler.now(), event))
 
             return result
@@ -69,14 +79,15 @@
         last = scheduler.callAt(2.5, record("d"))
         last.cancel()
         didCancel = []
 
         def bCancel() -> None:
             didCancel.append(True)
             bHandle.cancel()
+            self.assertEqual(bHandle.state, ScheduledState.cancelled)
 
         scheduler.callAt(1.5, bCancel)
         self.assertEqual(callTimes, [])
         driver.advance()
         self.assertEqual(callTimes, [(1.0, "a")])
         aHandle.cancel()  # if it's already called it's a no-op
         self.assertEqual(didCancel, [])
@@ -84,18 +95,12 @@
         self.assertEqual(callTimes, [(1.0, "a")])
         self.assertEqual(didCancel, [True])
         bHandle.cancel()  # repeated calls are no-ops
         self.assertEqual(didCancel, [True])
         driver.advance()
         self.assertEqual(callTimes, [(1.0, "a"), (3.0, "c")])
 
-    def test_queueMustBeEmpty(self) -> None:
-        driver = MemoryDriver()
-        q = Heap([FutureCall(1.0, noop, 1, False, False, nocancel)])
-        with self.assertRaises(ValueError):
-            SimpleScheduler(driver, q)
-
 
 def noop() -> None: ...
 
 
 def nocancel(x: object) -> None: ...
```

### Comparing `fritter-0.0.8/src/fritter/test/test_sleep.py` & `fritter-0.0.9/src/fritter/test/test_sleep.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from unittest import TestCase
 
+from ..boundaries import PhysicalScheduler
 from ..drivers.sleep import SleepDriver
-from ..scheduler import SimpleScheduler
+from ..scheduler import schedulerFromDriver
 
 
 class TestSleeping(TestCase):
     def test_sleep(self) -> None:
         sleeps = []
         current = 0.0
 
@@ -14,15 +15,15 @@
             sleeps.append(duration)
             current += duration
 
         def time() -> float:
             return current
 
         driver = SleepDriver(sleep=sleep, time=time)
-        scheduler = SimpleScheduler(driver)
+        scheduler: PhysicalScheduler = schedulerFromDriver(driver)
 
         threeCalledAt = None
         sevenCalledAt = None
 
         def three() -> None:
             nonlocal threeCalledAt
             threeCalledAt = driver.now()
@@ -48,15 +49,15 @@
             sleeps.append(duration)
             current += duration
 
         def time() -> float:
             return current
 
         driver = SleepDriver(sleep=sleep, time=time)
-        scheduler = SimpleScheduler(driver)
+        scheduler: PhysicalScheduler = schedulerFromDriver(driver)
 
         times = 0
 
         def once() -> None:
             nonlocal times
             times += 1
```

### Comparing `fritter-0.0.8/src/fritter/test/test_testing.py` & `fritter-0.0.9/src/fritter/test/test_testing.py`

 * *Files identical despite different names*

### Comparing `fritter-0.0.8/src/fritter/test/test_tree.py` & `fritter-0.0.9/src/fritter/test/test_tree.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from datetime import datetime, timedelta
 from typing import Callable, List, Tuple
 from unittest import TestCase
 from zoneinfo import ZoneInfo
 
 from datetype import DateTime
-from fritter.drivers.datetime import DateTimeDriver
-from fritter.scheduler import Scheduler
 
+from ..boundaries import CivilScheduler, PhysicalScheduler
+from ..drivers.datetimes import DateTimeDriver
 from ..drivers.memory import MemoryDriver
-from ..scheduler import SimpleScheduler
+from ..scheduler import schedulerFromDriver
 from ..tree import _BranchDriver, branch, timesFaster
 
 
 class RecursiveTest(TestCase):
     def _oneRecursiveCall(
         self, scaleFactor: float
     ) -> List[Tuple[float, float]]:
-        scheduler1: Scheduler[float, Callable[[], None]] = SimpleScheduler(
+        scheduler1: PhysicalScheduler = schedulerFromDriver(
             driver := MemoryDriver()
         )
         recursive, scheduler2 = branch(scheduler1, timesFaster(scaleFactor))
         calls = []
         scheduler2.callAt(
             1.0,
             lambda: calls.append((scheduler1.now(), scheduler2.now())),
@@ -33,29 +33,31 @@
         self.assertEqual(calls, [(1.0, 1.0)])
         calls = self._oneRecursiveCall(3.0)
         self.assertEqual(calls, [(1 / 3.0, 1.0)])
         calls = self._oneRecursiveCall(1 / 3.0)
         self.assertEqual(calls, [(3.0, 1.0)])
 
     def test_changeScaling(self) -> None:
-        scheduler1 = SimpleScheduler(driver := MemoryDriver())
+        scheduler1: PhysicalScheduler = schedulerFromDriver(
+            driver := MemoryDriver()
+        )
         recursive, scheduler2 = branch(scheduler1, timesFaster(2.0))
         calls = []
         scheduler2.callAt(
             1.0,
             lambda: calls.append((scheduler1.now(), scheduler2.now())),
         )
         driver.advance(1 / 4)
         recursive.changeScale(timesFaster(4.0))
         self.assertEqual(driver.advance(), 1 / 8)
         self.assertEqual(calls, [((1 / 4) + (1 / 8), 1.0)])
 
     def test_datetime(self) -> None:
-        scheduler1: Scheduler[DateTime[ZoneInfo], Callable[[], None]] = (
-            Scheduler(DateTimeDriver(driver := MemoryDriver()))
+        scheduler1: CivilScheduler = schedulerFromDriver(
+            DateTimeDriver(driver := MemoryDriver())
         )
         recursive, scheduler2 = branch(scheduler1)
         TZ = ZoneInfo("Etc/UTC")
         ts = datetime(2024, 2, 9, tzinfo=TZ).timestamp()
         driver.advance(ts)
         called = False
         called2 = False
@@ -90,19 +92,21 @@
         )
 
     def test_unscheduleNoOp(self) -> None:
         """
         Unscheduling when not scheduled is a no-op.
         """
         _BranchDriver(
-            SimpleScheduler(MemoryDriver()), timesFaster(1.0), 0.0
+            schedulerFromDriver(MemoryDriver()), timesFaster(1.0), 0.0
         ).unschedule()
 
     def test_unpausePauseUnpause(self) -> None:
-        scheduler1 = SimpleScheduler(driver := MemoryDriver())
+        scheduler1: PhysicalScheduler = schedulerFromDriver(
+            driver := MemoryDriver()
+        )
         recursive, scheduler2 = branch(scheduler1, timesFaster(2))
         recursive.pause()
         self.assertEqual(scheduler2.now(), 0.0)
         driver.advance(500)
         self.assertEqual(scheduler2.now(), 0.0)
         recursive.unpause()
         self.assertEqual(scheduler2.now(), 0.0)
@@ -110,28 +114,32 @@
         self.assertEqual(scheduler2.now(), 20.0)
         recursive.unpause()
         self.assertEqual(scheduler2.now(), 20.0)
         driver.advance(10)
         self.assertEqual(scheduler2.now(), 40.0)
 
     def test_moveSooner(self) -> None:
-        scheduler1 = SimpleScheduler(driver := MemoryDriver())
+        scheduler1: PhysicalScheduler = schedulerFromDriver(
+            driver := MemoryDriver()
+        )
         recursive, scheduler2 = branch(scheduler1)
         calls: list[tuple[float, float]] = []
         recursive.unpause()
 
         recordTimestamp = timestampRecorder(calls, scheduler1, scheduler2)
 
         scheduler2.callAt(1.0, recordTimestamp)
         scheduler2.callAt(0.5, recordTimestamp)
         driver.advance(0.6)
         self.assertEqual(calls, [(0.6, 0.6)])
 
     def test_pausing(self) -> None:
-        scheduler1 = SimpleScheduler(driver := MemoryDriver())
+        scheduler1: PhysicalScheduler = schedulerFromDriver(
+            driver := MemoryDriver()
+        )
         recursive, scheduler2 = branch(scheduler1)
         calls = []
         scheduler2.callAt(
             1.0,
             lambda: calls.append((scheduler1.now(), scheduler2.now())),
         )
         scheduler2.callAt(
@@ -152,15 +160,17 @@
         recursive.unpause()
         driver.advance(0.5)
         self.assertEqual(2.7 + 1.5 + 0.5, driver.now())
         self.assertEqual(1.5 + 0.5, scheduler2.now())
         self.assertEqual(calls, [(2.7 + 1.5 + 0.5, 2.0)])
 
     def test_doubleUnpause(self) -> None:
-        scheduler1 = SimpleScheduler(driver := MemoryDriver())
+        scheduler1: PhysicalScheduler = schedulerFromDriver(
+            driver := MemoryDriver()
+        )
         scaleFactor = 2.0
         recursive, scheduler2 = branch(scheduler1, timesFaster(scaleFactor))
         recursive.pause()
         baseTime = 1000.0
         driver.advance(baseTime)
         calls = []
         localDelta = 5.0
@@ -176,26 +186,28 @@
         driver.advance(1.0)
         self.assertEqual(calls, [])
         recursive.unpause()
         driver.advance(0.5)
         self.assertEqual(calls, [(baseTime + scaledDelta, localDelta)])
 
     def test_idling(self) -> None:
-        scheduler1 = SimpleScheduler(driver := MemoryDriver())
+        scheduler1: PhysicalScheduler = schedulerFromDriver(
+            driver := MemoryDriver()
+        )
         recursive, scheduler2 = branch(scheduler1)
         calls: list[tuple[float, float]] = []
         recordTimestamp = timestampRecorder(calls, scheduler1, scheduler2)
         onlyCall = scheduler2.callAt(1.0, recordTimestamp)
         self.assertTrue(driver.isScheduled())
         onlyCall.cancel()
         self.assertFalse(driver.isScheduled())
 
 
 def timestampRecorder(
     calls: list[tuple[float, float]],
-    scheduler1: SimpleScheduler,
-    scheduler2: SimpleScheduler,
+    scheduler1: PhysicalScheduler,
+    scheduler2: PhysicalScheduler,
 ) -> Callable[[], None]:
     def recorder() -> None:
         calls.append((scheduler1.now(), scheduler2.now()))
 
     return recorder
```

### Comparing `fritter-0.0.8/src/fritter/test/test_twisted.py` & `fritter-0.0.9/src/fritter/test/test_twisted.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from __future__ import annotations
 
+from typing import Any
+
 from twisted.internet.task import Clock
 from twisted.trial.unittest import SynchronousTestCase
 
 from ..drivers.twisted import TwistedAsyncDriver, TwistedTimeDriver, scheduler
 
 
 class TestAsyncDriver(SynchronousTestCase):
     def setUp(self) -> None:
-        self.calls = 0
+        self.callCount = 0
 
     def called(self) -> None:
-        self.calls += 1
+        self.callCount += 1
 
     def test_complete(self) -> None:
         driver = TwistedAsyncDriver()
         d = driver.newWithCancel(self.called)
         self.assertNoResult(d)
         driver.complete(d)
         self.assertIsNone(self.successResultOf(d))
@@ -47,64 +49,64 @@
         self.assertEqual(after, 0)
         driver.complete(operation)
         self.assertEqual(after, 1)
 
 
 class TestTimeDriver(SynchronousTestCase):
     def setUp(self) -> None:
-        self.calls = 0
+        self.callCount = 0
 
     def called(self) -> None:
-        self.calls += 1
+        self.callCount += 1
 
     def test_now(self) -> None:
         clock = Clock()
         driver = TwistedTimeDriver(clock)
         clock.advance(1234)
         self.assertEqual(driver.now(), 1234.0)
         self.assertEqual(clock.getDelayedCalls(), [])
 
     def test_schedule(self) -> None:
         clock = Clock()
         driver = TwistedTimeDriver(clock)
         driver.reschedule(1.0, self.called)
         clock.advance(0.5)
-        self.assertEqual(self.calls, 0)
+        self.assertEqual(self.callCount, 0)
         clock.advance(0.6)
-        self.assertEqual(self.calls, 1)
+        self.assertEqual(self.callCount, 1)
         self.assertEqual(clock.getDelayedCalls(), [])
 
     def test_reschedule(self) -> None:
         clock = Clock()
         driver = TwistedTimeDriver(clock)
         driver.reschedule(1.0, self.called)
         clock.advance(0.5)
-        self.assertEqual(self.calls, 0)
+        self.assertEqual(self.callCount, 0)
         driver.reschedule(2.0, self.called)
         clock.advance(0.6)
-        self.assertEqual(self.calls, 0)
+        self.assertEqual(self.callCount, 0)
         clock.advance(0.9)
-        self.assertEqual(self.calls, 1)
+        self.assertEqual(self.callCount, 1)
         self.assertEqual(clock.getDelayedCalls(), [])
 
     def test_unschedule(self) -> None:
         clock = Clock()
         driver = TwistedTimeDriver(clock)
         driver.reschedule(1.0, self.called)
         clock.advance(0.5)
-        self.assertEqual(self.calls, 0)
+        self.assertEqual(self.callCount, 0)
         driver.unschedule()
-        self.assertEqual(self.calls, 0)
+        self.assertEqual(self.callCount, 0)
         clock.advance(0.9)
-        self.assertEqual(self.calls, 0)
+        self.assertEqual(self.callCount, 0)
         driver.unschedule()  # no-op, no exception
         self.assertEqual(clock.getDelayedCalls(), [])
 
     def test_schedulerDefault(self) -> None:
-        sched = scheduler()
+        sched: Any = scheduler()
         self.assertIsInstance(sched.driver, TwistedTimeDriver)
 
     def test_scheduler(self) -> None:
         sched = scheduler(clock := Clock())
         stuff = []
 
         def hello() -> None:
```

### Comparing `fritter-0.0.8/src/fritter/tree.py` & `fritter-0.0.9/src/fritter/tree.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,18 +13,19 @@
     Generic,
     Optional,
     Protocol,
     Tuple,
     TypeVar,
     overload,
 )
+
 from typing_extensions import Self
-from .boundaries import PriorityComparable
 
-from .scheduler import FutureCall, Scheduler
+from .boundaries import Cancellable, PriorityComparable, Scheduler
+from .scheduler import schedulerFromDriver
 
 _BranchTime = TypeVar("_BranchTime", bound=PriorityComparable)
 _TrunkTime = TypeVar("_TrunkTime", bound=PriorityComparable)
 _TrunkDelta = TypeVar("_TrunkDelta")
 
 
 class Scale(Protocol[_BranchTime, _TrunkTime, _TrunkDelta]):
@@ -177,48 +178,50 @@
         to stop advancing and causing any timers schedule with it via
         L{Scheduler.callAt} to stop running.
         """
 
 
 @overload
 def branch(
-    trunk: Scheduler[WhenT, Callable[[], None]],
+    trunk: Scheduler[WhenT, Callable[[], None], object],
     scale: Scale[WhenT, WhenT, _TrunkDelta],
 ) -> tuple[
     BranchManager[WhenT, _TrunkDelta],
-    Scheduler[WhenT, Callable[[], None]],
+    Scheduler[WhenT, Callable[[], None], int],
 ]: ...
 
 
 @overload
-def branch(trunk: Scheduler[WhenT, Callable[[], None]]) -> tuple[
+def branch(trunk: Scheduler[WhenT, Callable[[], None], object]) -> tuple[
     BranchManager[WhenT, WhenT],
-    Scheduler[WhenT, Callable[[], None]],
+    Scheduler[WhenT, Callable[[], None], int],
 ]: ...
 
 
 def branch(
-    trunk: Scheduler[WhenT, Callable[[], None]],
+    trunk: Scheduler[WhenT, Callable[[], None], object],
     scale: Scale[WhenT, WhenT, _TrunkDelta] | None = None,
 ) -> tuple[
     BranchManager[WhenT, _TrunkDelta],
-    Scheduler[WhenT, Callable[[], None]],
+    Scheduler[WhenT, Callable[[], None], int],
 ]:
     """
     Derive a branch (child) scheduler from a C{trunk} (parent) scheduler.
     """
     if scale is None:
         scale = NoScale[_TrunkDelta]()
         # scale = timesFaster(1)  # type:ignore
     assert scale is not None
     driver: _BranchDriver[WhenT, WhenT, _TrunkDelta] = _BranchDriver(
         trunk, scale, scale.shift(None, trunk.now())
     )
     driver.changeScale(scale)
-    branchScheduler: Scheduler[WhenT, Callable[[], None]] = Scheduler(driver)
+    branchScheduler: Scheduler[WhenT, Callable[[], None], int] = (
+        schedulerFromDriver(driver)
+    )
     driver.unpause()
     return driver, branchScheduler
 
 
 _F = TypeVar("_F", bound=float)
 
 
@@ -229,15 +232,15 @@
 @dataclass
 class _BranchDriver(Generic[_TrunkTime, _BranchTime, _TrunkDelta]):
     """
     Implementation of L{TimeDriver} for L{Scheduler} that is stacked on top of
     another L{Scheduler}.
     """
 
-    trunk: Scheduler[_TrunkTime, Callable[[], None]]
+    trunk: Scheduler[_TrunkTime, Callable[[], None], object]
     """
     The scheduler that this driver is a branch of.
     """
     # TODO: support for a generic WhatT would be nice here, but we have our own
     # function that needs to be scheduled with the trunk scheduler, and so we
     # couldn't meaningfully integrate with a higher-level persistent scheduler.
 
@@ -255,15 +258,15 @@
     Timestamp at which we were last paused, if we were last paused.
     """
 
     _scheduleWhenStarted: Optional[Tuple[_BranchTime, Callable[[], None]]] = (
         None
     )
 
-    _call: Optional[FutureCall[_TrunkTime, Callable[[], None]]] = None
+    _call: Optional[Cancellable] = None
     _running: bool = False
 
     def reschedule(
         self, desiredTime: _BranchTime, work: Callable[[], None]
     ) -> None:
         assert (
             self._call is None or self._running
```

### Comparing `fritter-0.0.8/PKG-INFO` & `fritter-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fritter
-Version: 0.0.8
+Version: 0.0.9
 Summary: Fritter, the Frame-Rate IndependenT TimEr tRee.
 Author-email: Glyph <glyph@glyph.im>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Operating System :: OS Independent
@@ -63,15 +63,15 @@
 
 - Do you need to schedule a very *low*-frequency timer, whose rate is measured
   in weeks or months, something that runs so infrequently or so far in the
   future that the current process will almost certainly no longer be running?
   Schedule your timer in terms of
   [`datetime`-ish](https://pypi.org/project/datetype/) objects, then serialize
   it with
-  [`fritter.persistent.json`](https://fritter.readthedocs.io/en/latest/persistence.html)
+  [`fritter.persistent.jsonable`](https://fritter.readthedocs.io/en/latest/persistence.html)
   to load it again when your process restarts.  `fritter.persistent` is careful
   to supply an interface using IANA identifiers to maintain correctness in the
   face of future DST changes, and other things that can start to complicate the
   use of time over longer periods.
 
 - Do you need to manage *groups* of related timers, sometimes pausing some
   groups while allowing others to continue, while all running on the same loop;
```

