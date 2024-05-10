# Comparing `tmp/autobean-0.2.1.tar.gz` & `tmp/autobean-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autobean-0.2.1.tar", last modified: Mon Jun 26 10:16:01 2023, max compression
+gzip compressed data, was "autobean-0.2.2.tar", last modified: Fri May 10 00:10:47 2024, max compression
```

## Comparing `autobean-0.2.1.tar` & `autobean-0.2.2.tar`

### file list

```diff
@@ -1,63 +1,44 @@
-drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-06-26 10:16:01.132926 autobean-0.2.1/
--rw-r--r--   0 seiarotg   (501) staff       (20)    18092 2019-09-03 05:14:19.000000 autobean-0.2.1/LICENSE
--rw-r--r--   0 seiarotg   (501) staff       (20)     2311 2023-06-26 10:16:01.132270 autobean-0.2.1/PKG-INFO
--rw-r--r--   0 seiarotg   (501) staff       (20)     1701 2023-05-13 12:32:14.000000 autobean-0.2.1/README.md
-drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-06-26 10:16:01.085144 autobean-0.2.1/autobean/
--rw-r--r--   0 seiarotg   (501) staff       (20)        0 2021-01-02 21:42:25.000000 autobean-0.2.1/autobean/__init__.py
-drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-06-26 10:16:01.090978 autobean-0.2.1/autobean/include/
--rw-r--r--   0 seiarotg   (501) staff       (20)       88 2023-01-29 01:35:33.000000 autobean-0.2.1/autobean/include/__init__.py
--rw-r--r--   0 seiarotg   (501) staff       (20)     1028 2023-01-29 01:35:33.000000 autobean-0.2.1/autobean/include/plugin.py
-drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-06-26 10:16:01.092545 autobean-0.2.1/autobean/include/tests/
--rw-r--r--   0 seiarotg   (501) staff       (20)        0 2019-09-05 14:56:04.000000 autobean-0.2.1/autobean/include/tests/__init__.py
--rw-r--r--   0 seiarotg   (501) staff       (20)      869 2023-01-29 01:35:33.000000 autobean-0.2.1/autobean/include/tests/test_runner.py
-drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-06-26 10:16:01.096265 autobean-0.2.1/autobean/narration/
--rw-r--r--   0 seiarotg   (501) staff       (20)       69 2019-09-01 11:30:46.000000 autobean-0.2.1/autobean/narration/__init__.py
--rw-r--r--   0 seiarotg   (501) staff       (20)      464 2022-06-11 14:47:44.000000 autobean-0.2.1/autobean/narration/comments.py
--rw-r--r--   0 seiarotg   (501) staff       (20)     1458 2022-06-11 14:47:44.000000 autobean-0.2.1/autobean/narration/plugin.py
-drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-06-26 10:16:01.097639 autobean-0.2.1/autobean/narration/tests/
--rw-r--r--   0 seiarotg   (501) staff       (20)        0 2019-09-01 14:17:47.000000 autobean-0.2.1/autobean/narration/tests/__init__.py
--rw-r--r--   0 seiarotg   (501) staff       (20)      195 2022-06-11 14:47:44.000000 autobean-0.2.1/autobean/narration/tests/test_runner.py
-drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-06-26 10:16:01.109920 autobean-0.2.1/autobean/share/
--rw-r--r--   0 seiarotg   (501) staff       (20)       59 2023-01-29 01:35:33.000000 autobean-0.2.1/autobean/share/__init__.py
--rw-r--r--   0 seiarotg   (501) staff       (20)     3512 2023-06-26 10:08:53.000000 autobean-0.2.1/autobean/share/include.py
--rw-r--r--   0 seiarotg   (501) staff       (20)      826 2023-01-29 01:35:33.000000 autobean-0.2.1/autobean/share/include_context.py
--rw-r--r--   0 seiarotg   (501) staff       (20)     8890 2023-01-29 01:35:33.000000 autobean-0.2.1/autobean/share/link_accounts.py
--rw-r--r--   0 seiarotg   (501) staff       (20)     9345 2023-01-29 01:59:08.000000 autobean-0.2.1/autobean/share/plugin.py
--rw-r--r--   0 seiarotg   (501) staff       (20)    10792 2023-01-29 03:37:02.000000 autobean-0.2.1/autobean/share/policy_lib.py
--rw-r--r--   0 seiarotg   (501) staff       (20)    23168 2023-01-29 03:38:18.000000 autobean-0.2.1/autobean/share/policy_lib_test.py
--rw-r--r--   0 seiarotg   (501) staff       (20)    21459 2023-01-29 01:59:21.000000 autobean-0.2.1/autobean/share/split_account.py
-drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-06-26 10:16:01.111709 autobean-0.2.1/autobean/share/tests/
--rw-r--r--   0 seiarotg   (501) staff       (20)        0 2019-08-10 06:00:31.000000 autobean-0.2.1/autobean/share/tests/__init__.py
--rw-r--r--   0 seiarotg   (501) staff       (20)      358 2023-01-29 01:35:33.000000 autobean-0.2.1/autobean/share/tests/test_runner.py
--rw-r--r--   0 seiarotg   (501) staff       (20)      125 2023-01-29 01:35:33.000000 autobean-0.2.1/autobean/share/viewpoint_lib.py
-drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-06-26 10:16:01.113824 autobean-0.2.1/autobean/sorted/
--rw-r--r--   0 seiarotg   (501) staff       (20)       66 2021-01-01 19:45:48.000000 autobean-0.2.1/autobean/sorted/__init__.py
--rw-r--r--   0 seiarotg   (501) staff       (20)     3836 2022-12-19 14:01:53.000000 autobean-0.2.1/autobean/sorted/plugin.py
-drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-06-26 10:16:01.117613 autobean-0.2.1/autobean/stock_split/
--rw-r--r--   0 seiarotg   (501) staff       (20)       58 2023-01-29 01:35:33.000000 autobean-0.2.1/autobean/stock_split/__init__.py
--rw-r--r--   0 seiarotg   (501) staff       (20)     3057 2023-01-29 01:35:33.000000 autobean-0.2.1/autobean/stock_split/plugin.py
--rw-r--r--   0 seiarotg   (501) staff       (20)     4040 2023-01-29 01:35:33.000000 autobean-0.2.1/autobean/stock_split/plugin_test.py
-drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-06-26 10:16:01.119105 autobean-0.2.1/autobean/truelayer/
--rw-r--r--   0 seiarotg   (501) staff       (20)       49 2020-12-29 22:03:00.000000 autobean-0.2.1/autobean/truelayer/__init__.py
--rw-r--r--   0 seiarotg   (501) staff       (20)    17776 2023-05-13 12:50:56.000000 autobean-0.2.1/autobean/truelayer/importer.py
-drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-06-26 10:16:01.125065 autobean-0.2.1/autobean/utils/
--rw-r--r--   0 seiarotg   (501) staff       (20)        0 2019-08-10 06:00:31.000000 autobean-0.2.1/autobean/utils/__init__.py
--rw-r--r--   0 seiarotg   (501) staff       (20)      953 2022-06-11 14:47:44.000000 autobean-0.2.1/autobean/utils/compare.py
--rw-r--r--   0 seiarotg   (501) staff       (20)     5637 2023-01-02 23:04:05.000000 autobean-0.2.1/autobean/utils/deduplicate.py
--rw-r--r--   0 seiarotg   (501) staff       (20)     1124 2023-01-29 01:35:33.000000 autobean-0.2.1/autobean/utils/error_lib.py
--rw-r--r--   0 seiarotg   (501) staff       (20)     7686 2023-01-29 01:35:33.000000 autobean-0.2.1/autobean/utils/plugin_lib.py
--rw-r--r--   0 seiarotg   (501) staff       (20)     9373 2023-01-29 01:35:33.000000 autobean-0.2.1/autobean/utils/plugin_test_utils.py
-drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-06-26 10:16:01.128287 autobean-0.2.1/autobean/xcheck/
--rw-r--r--   0 seiarotg   (501) staff       (20)       93 2023-01-29 01:35:33.000000 autobean-0.2.1/autobean/xcheck/__init__.py
--rw-r--r--   0 seiarotg   (501) staff       (20)     4205 2023-01-29 01:35:33.000000 autobean-0.2.1/autobean/xcheck/plugin.py
-drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-06-26 10:16:01.131100 autobean-0.2.1/autobean/xcheck/tests/
--rw-r--r--   0 seiarotg   (501) staff       (20)        0 2019-08-10 06:00:31.000000 autobean-0.2.1/autobean/xcheck/tests/__init__.py
--rw-r--r--   0 seiarotg   (501) staff       (20)      868 2023-01-29 01:35:33.000000 autobean-0.2.1/autobean/xcheck/tests/test_runner.py
-drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-06-26 10:16:01.088417 autobean-0.2.1/autobean.egg-info/
--rw-r--r--   0 seiarotg   (501) staff       (20)     2311 2023-06-26 10:16:00.000000 autobean-0.2.1/autobean.egg-info/PKG-INFO
--rw-r--r--   0 seiarotg   (501) staff       (20)     1360 2023-06-26 10:16:01.000000 autobean-0.2.1/autobean.egg-info/SOURCES.txt
--rw-r--r--   0 seiarotg   (501) staff       (20)        1 2023-06-26 10:16:00.000000 autobean-0.2.1/autobean.egg-info/dependency_links.txt
--rw-r--r--   0 seiarotg   (501) staff       (20)       42 2023-06-26 10:16:00.000000 autobean-0.2.1/autobean.egg-info/requires.txt
--rw-r--r--   0 seiarotg   (501) staff       (20)        9 2023-06-26 10:16:00.000000 autobean-0.2.1/autobean.egg-info/top_level.txt
--rw-r--r--   0 seiarotg   (501) staff       (20)       38 2023-06-26 10:16:01.133059 autobean-0.2.1/setup.cfg
--rw-r--r--   0 seiarotg   (501) staff       (20)      959 2023-06-26 10:11:25.000000 autobean-0.2.1/setup.py
+-rw-r--r--   0        0        0    18092 2024-05-10 00:10:31.093033 autobean-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1612 2024-05-10 00:10:31.093033 autobean-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-10 00:10:31.093033 autobean-0.2.2/autobean/__init__.py
+-rw-r--r--   0        0        0     1245 2024-05-10 00:10:31.093033 autobean-0.2.2/autobean/include/README.md
+-rw-r--r--   0        0        0       88 2024-05-10 00:10:31.093033 autobean-0.2.2/autobean/include/__init__.py
+-rw-r--r--   0        0        0     1028 2024-05-10 00:10:31.093033 autobean-0.2.2/autobean/include/plugin.py
+-rw-r--r--   0        0        0     2935 2024-05-10 00:10:31.093033 autobean-0.2.2/autobean/narration/README.md
+-rw-r--r--   0        0        0       69 2024-05-10 00:10:31.093033 autobean-0.2.2/autobean/narration/__init__.py
+-rw-r--r--   0        0        0      464 2024-05-10 00:10:31.093033 autobean-0.2.2/autobean/narration/comments.py
+-rw-r--r--   0        0        0     1458 2024-05-10 00:10:31.093033 autobean-0.2.2/autobean/narration/plugin.py
+-rw-r--r--   0        0        0      100 2024-05-10 00:10:31.093033 autobean-0.2.2/autobean/refactor/README.md
+-rw-r--r--   0        0        0     8234 2024-05-10 00:10:31.093033 autobean-0.2.2/autobean/share/README.md
+-rw-r--r--   0        0        0       59 2024-05-10 00:10:31.093033 autobean-0.2.2/autobean/share/__init__.py
+-rw-r--r--   0        0        0    21290 2024-05-10 00:10:31.093033 autobean-0.2.2/autobean/share/docs/advanced.md
+-rw-r--r--   0        0        0     6628 2024-05-10 00:10:31.093033 autobean-0.2.2/autobean/share/docs/rationale.md
+-rw-r--r--   0        0        0     3512 2024-05-10 00:10:31.093033 autobean-0.2.2/autobean/share/include.py
+-rw-r--r--   0        0        0      826 2024-05-10 00:10:31.093033 autobean-0.2.2/autobean/share/include_context.py
+-rw-r--r--   0        0        0     8890 2024-05-10 00:10:31.093033 autobean-0.2.2/autobean/share/link_accounts.py
+-rw-r--r--   0        0        0     9345 2024-05-10 00:10:31.093033 autobean-0.2.2/autobean/share/plugin.py
+-rw-r--r--   0        0        0    11050 2024-05-10 00:10:31.097033 autobean-0.2.2/autobean/share/policy_lib.py
+-rw-r--r--   0        0        0    23976 2024-05-10 00:10:31.097033 autobean-0.2.2/autobean/share/policy_lib_test.py
+-rw-r--r--   0        0        0    21459 2024-05-10 00:10:31.097033 autobean-0.2.2/autobean/share/split_account.py
+-rw-r--r--   0        0        0      125 2024-05-10 00:10:31.097033 autobean-0.2.2/autobean/share/viewpoint_lib.py
+-rw-r--r--   0        0        0     1378 2024-05-10 00:10:31.097033 autobean-0.2.2/autobean/sorted/README.md
+-rw-r--r--   0        0        0       66 2024-05-10 00:10:31.097033 autobean-0.2.2/autobean/sorted/__init__.py
+-rw-r--r--   0        0        0     3836 2024-05-10 00:10:31.097033 autobean-0.2.2/autobean/sorted/plugin.py
+-rw-r--r--   0        0        0     1237 2024-05-10 00:10:31.097033 autobean-0.2.2/autobean/stock_split/README.md
+-rw-r--r--   0        0        0       58 2024-05-10 00:10:31.097033 autobean-0.2.2/autobean/stock_split/__init__.py
+-rw-r--r--   0        0        0     3057 2024-05-10 00:10:31.097033 autobean-0.2.2/autobean/stock_split/plugin.py
+-rw-r--r--   0        0        0     4040 2024-05-10 00:10:31.097033 autobean-0.2.2/autobean/stock_split/plugin_test.py
+-rw-r--r--   0        0        0     2214 2024-05-10 00:10:31.097033 autobean-0.2.2/autobean/truelayer/README.md
+-rw-r--r--   0        0        0       49 2024-05-10 00:10:31.097033 autobean-0.2.2/autobean/truelayer/__init__.py
+-rw-r--r--   0        0        0    17776 2024-05-10 00:10:31.097033 autobean-0.2.2/autobean/truelayer/importer.py
+-rw-r--r--   0        0        0        0 2024-05-10 00:10:31.097033 autobean-0.2.2/autobean/utils/__init__.py
+-rw-r--r--   0        0        0      953 2024-05-10 00:10:31.097033 autobean-0.2.2/autobean/utils/compare.py
+-rw-r--r--   0        0        0     5762 2024-05-10 00:10:31.097033 autobean-0.2.2/autobean/utils/deduplicate.py
+-rw-r--r--   0        0        0     1124 2024-05-10 00:10:31.097033 autobean-0.2.2/autobean/utils/error_lib.py
+-rw-r--r--   0        0        0     7686 2024-05-10 00:10:31.101033 autobean-0.2.2/autobean/utils/plugin_lib.py
+-rw-r--r--   0        0        0     9373 2024-05-10 00:10:31.101033 autobean-0.2.2/autobean/utils/plugin_test_utils.py
+-rw-r--r--   0        0        0     1823 2024-05-10 00:10:31.101033 autobean-0.2.2/autobean/xcheck/README.md
+-rw-r--r--   0        0        0       93 2024-05-10 00:10:31.101033 autobean-0.2.2/autobean/xcheck/__init__.py
+-rw-r--r--   0        0        0     4258 2024-05-10 00:10:31.101033 autobean-0.2.2/autobean/xcheck/plugin.py
+-rw-r--r--   0        0        0      800 2024-05-10 00:10:31.101033 autobean-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1881 1970-01-01 00:00:00.000000 autobean-0.2.2/PKG-INFO
```

### Comparing `autobean-0.2.1/LICENSE` & `autobean-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autobean-0.2.1/PKG-INFO` & `autobean-0.2.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,19 @@
 Metadata-Version: 2.1
 Name: autobean
-Version: 0.2.1
+Version: 0.2.2
 Summary: A collection of plugins and scripts that help automating bookkeeping with beancount
-Home-page: https://github.com/SEIAROTg/autobean
-Author: SEIAROTg
-Author-email: seiarotg@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
-Classifier: Topic :: Office/Business :: Financial :: Accounting
+License: GPL2
+Author-email: SEIAROTg <seiarotg@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # autobean
-[![CircleCI](https://circleci.com/gh/SEIAROTg/autobean.svg?style=shield)](https://circleci.com/gh/SEIAROTg/autobean)
+[![build](https://github.com/SEIAROTg/autobean/actions/workflows/build.yml/badge.svg)](https://github.com/SEIAROTg/autobean/actions/workflows/build.yml)
 [![pypi](https://img.shields.io/pypi/v/autobean)](https://pypi.org/project/autobean/)
-[![codecov](https://codecov.io/gh/SEIAROTg/autobean/branch/master/graph/badge.svg)](https://codecov.io/gh/SEIAROTg/autobean)
 [![Maintainability](https://api.codeclimate.com/v1/badges/65e79b66e57139ed8bd0/maintainability)](https://codeclimate.com/github/SEIAROTg/autobean/maintainability)
 [![Test Coverage](https://api.codeclimate.com/v1/badges/65e79b66e57139ed8bd0/test_coverage)](https://codeclimate.com/github/SEIAROTg/autobean/test_coverage)
 [![license](https://img.shields.io/github/license/SEIAROTg/autobean.svg)](https://github.com/SEIAROTg/autobean)
 
 A collection of plugins and scripts that help automating bookkeeping with [beancount](http://furius.ca/beancount/).
 
 ## Components
@@ -35,7 +27,8 @@
 * [autobean.stock_split](autobean/stock_split): Simplifies stock split.
 
 ## Install
 
 ```sh
 pip install autobean
 ```
+
```

### Comparing `autobean-0.2.1/README.md` & `autobean-0.2.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # autobean
-[![CircleCI](https://circleci.com/gh/SEIAROTg/autobean.svg?style=shield)](https://circleci.com/gh/SEIAROTg/autobean)
+[![build](https://github.com/SEIAROTg/autobean/actions/workflows/build.yml/badge.svg)](https://github.com/SEIAROTg/autobean/actions/workflows/build.yml)
 [![pypi](https://img.shields.io/pypi/v/autobean)](https://pypi.org/project/autobean/)
-[![codecov](https://codecov.io/gh/SEIAROTg/autobean/branch/master/graph/badge.svg)](https://codecov.io/gh/SEIAROTg/autobean)
 [![Maintainability](https://api.codeclimate.com/v1/badges/65e79b66e57139ed8bd0/maintainability)](https://codeclimate.com/github/SEIAROTg/autobean/maintainability)
 [![Test Coverage](https://api.codeclimate.com/v1/badges/65e79b66e57139ed8bd0/test_coverage)](https://codeclimate.com/github/SEIAROTg/autobean/test_coverage)
 [![license](https://img.shields.io/github/license/SEIAROTg/autobean.svg)](https://github.com/SEIAROTg/autobean)
 
 A collection of plugins and scripts that help automating bookkeeping with [beancount](http://furius.ca/beancount/).
 
 ## Components
```

### Comparing `autobean-0.2.1/autobean/include/plugin.py` & `autobean-0.2.2/autobean/include/plugin.py`

 * *Files identical despite different names*

### Comparing `autobean-0.2.1/autobean/narration/plugin.py` & `autobean-0.2.2/autobean/narration/plugin.py`

 * *Files identical despite different names*

### Comparing `autobean-0.2.1/autobean/share/include.py` & `autobean-0.2.2/autobean/share/include.py`

 * *Files identical despite different names*

### Comparing `autobean-0.2.1/autobean/share/include_context.py` & `autobean-0.2.2/autobean/share/include_context.py`

 * *Files identical despite different names*

### Comparing `autobean-0.2.1/autobean/share/link_accounts.py` & `autobean-0.2.2/autobean/share/link_accounts.py`

 * *Files identical despite different names*

### Comparing `autobean-0.2.1/autobean/share/plugin.py` & `autobean-0.2.2/autobean/share/plugin.py`

 * *Files identical despite different names*

### Comparing `autobean-0.2.1/autobean/share/policy_lib.py` & `autobean-0.2.2/autobean/share/policy_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,15 +152,19 @@
         if policy_def.parent and policy_def.parent not in self._named_policies:
             raise error_lib.PluginException(
                 f'Reference to unknown share policy {policy_def.parent!r}')
         if policy_def.enforced and not policy_def.ownership:
             raise error_lib.PluginException(
                 f'Policy with share_enforced must define ownership')
         if name.endswith(':*'):
-            self._wildcard_account_policies[name.removesuffix(':*')] = policy_def
+            prefix = name.removesuffix(':*')
+            self._wildcard_account_policies[prefix] = policy_def
+            if (account_policy_def := self._account_policies.get(prefix)) is not None:
+                self._account_policies[prefix] = _override_policy_def(
+                    policy_def, account_policy_def, is_ephemeral=False)
         elif ':' in name:
             self._account_policies[name] = policy_def
         else:
             self._named_policies[name] = policy_def
 
     def _get_account_policy_definition(self, account: str) -> Optional[PolicyDefinition]:
         policy_def = None
```

### Comparing `autobean-0.2.1/autobean/share/policy_lib_test.py` & `autobean-0.2.2/autobean/share/policy_lib_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,25 +197,41 @@
     @_parse_doc(Transaction)
     def test_priority_account(self, txn: Transaction) -> None:
         """
         2000-01-01 *
             share-Alice: 1
             Assets:Account 100.00 USD
                 share_prorated_included: FALSE
+            Assets:Account:Account 100.00 USD
+                share_prorated_included: FALSE
         """
-        self._policy_db.add_policy('Assets:Account', self._create_policy(42))
-        self._policy_db.add_policy('Assets:Account:*', self._create_policy(2))
+        self._policy_db.add_policy('Assets:Account:*', self._create_policy(42))
+        self._policy_db.add_policy('Assets:Account', self._create_policy(43))
         self._policy_db.add_policy('Assets:*', self._create_policy(3))
         self._policy_db.add_policy('default', self._create_policy(4))
 
         policy_def = policy_lib.try_parse_policy_definition(txn.meta)
+
         policy = self._policy_db.get_posting_policy(txn.postings[0], policy_def)
         assert isinstance(policy.ownership, policy_lib.WeightedOwnership)
+        assert policy.ownership.weights['Alice'] == 43
+        policy = self._policy_db.get_posting_policy(txn.postings[1], policy_def)
+        assert isinstance(policy.ownership, policy_lib.WeightedOwnership)
         assert policy.ownership.weights['Alice'] == 42
 
+        self._policy_db.add_policy('Assets:Account:*', self._create_policy(42))
+
+        policy = self._policy_db.get_posting_policy(txn.postings[0], policy_def)
+        assert isinstance(policy.ownership, policy_lib.WeightedOwnership)
+        assert policy.ownership.weights['Alice'] == 42
+        policy = self._policy_db.get_posting_policy(txn.postings[1], policy_def)
+        assert isinstance(policy.ownership, policy_lib.WeightedOwnership)
+        assert policy.ownership.weights['Alice'] == 42
+
+
     @_parse_doc(Transaction)
     def test_priority_wildcard_account_same(self, txn: Transaction) -> None:
         """
         2000-01-01 *
             share-Alice: 1
             Assets:Account 100.00 USD
                 share_prorated_included: FALSE
```

### Comparing `autobean-0.2.1/autobean/share/split_account.py` & `autobean-0.2.2/autobean/share/split_account.py`

 * *Files identical despite different names*

### Comparing `autobean-0.2.1/autobean/sorted/plugin.py` & `autobean-0.2.2/autobean/sorted/plugin.py`

 * *Files identical despite different names*

### Comparing `autobean-0.2.1/autobean/stock_split/plugin.py` & `autobean-0.2.2/autobean/stock_split/plugin.py`

 * *Files identical despite different names*

### Comparing `autobean-0.2.1/autobean/stock_split/plugin_test.py` & `autobean-0.2.2/autobean/stock_split/plugin_test.py`

 * *Files identical despite different names*

### Comparing `autobean-0.2.1/autobean/truelayer/importer.py` & `autobean-0.2.2/autobean/truelayer/importer.py`

 * *Files identical despite different names*

### Comparing `autobean-0.2.1/autobean/utils/compare.py` & `autobean-0.2.2/autobean/utils/compare.py`

 * *Files identical despite different names*

### Comparing `autobean-0.2.1/autobean/utils/deduplicate.py` & `autobean-0.2.2/autobean/utils/deduplicate.py`

 * *Files 12% similar despite different names*

```diff
@@ -107,43 +107,42 @@
 
     return ret
 
 
 class _Matcher:
     def __init__(self) -> None:
         self._new_nodes: set[_Node] = set()
-        self._edges: defaultdict[_Node, set[_Node]] = defaultdict(set)
+        self._edges = defaultdict[_Node, list[_Node]](list)
 
     def add_edge(self, new_entry: Directive, existing_entry: Directive) -> None:
         new_node = (True, new_entry)
         existing_node = (False, existing_entry)
         self._new_nodes.add(new_node)
-        self._edges[new_node].add(existing_node)
-        self._edges[existing_node].add(new_node)
+        self._edges[new_node].append(existing_node)
+        self._edges[existing_node].append(new_node)
+
+    def _dfs(self, node: _Node, matches: dict[_Node, _Node], visited: set[_Node]) -> bool:
+        visited.add(node)
+        for sibling in self._edges[node]:
+            if sibling not in matches:
+                matches[sibling] = node
+                matches[node] = sibling
+                return True
+        for sibling in self._edges[node]:
+            if matches[sibling] not in visited and self._dfs(matches[sibling], matches, visited):
+                matches[sibling] = node
+                matches[node] = sibling
+                return True
+        return False
 
     def matches(self) -> set[_Node]:
-        matches = set()
+        matches = dict[_Node, _Node]()
         for new_node in self._new_nodes:
-            if new_node in matches:
-                continue
-            q: deque[_Node] = deque()
-            q.append(new_node)
-            visited = set()
-            while q:
-                u = q.popleft()
-                if u in visited:
-                    continue
-                visited.add(u)
-                if u not in matches and u != new_node:
-                    matches.add(new_node)
-                    matches.add(u)
-                    break
-                for v in self._edges[u]:
-                    q.append(v)
-        return matches
+            self._dfs(new_node, matches, set())
+        return matches.keys() | matches.values()
 
     def subgraphs(self) -> Iterable[set[_Node]]:
         visited = set()
         for new_node in self._new_nodes:
             if new_node in visited:
                 continue
             subgraph_nodes = set()
```

### Comparing `autobean-0.2.1/autobean/utils/error_lib.py` & `autobean-0.2.2/autobean/utils/error_lib.py`

 * *Files identical despite different names*

### Comparing `autobean-0.2.1/autobean/utils/plugin_lib.py` & `autobean-0.2.2/autobean/utils/plugin_lib.py`

 * *Files identical despite different names*

### Comparing `autobean-0.2.1/autobean/utils/plugin_test_utils.py` & `autobean-0.2.2/autobean/utils/plugin_test_utils.py`

 * *Files identical despite different names*

### Comparing `autobean-0.2.1/autobean/xcheck/plugin.py` & `autobean-0.2.2/autobean/xcheck/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             ))
         for posting in missing:
             self._error_logger.log_error(CrossCheckError(
                 posting.posting.meta, 'Missing posting', posting.transaction
             ))
         self._includes.add(path)
         for stmt_entry in stmt_entries:
-            if isinstance(stmt_entry, Balance):
+            if isinstance(stmt_entry, Balance) and (not accounts or stmt_entry.account in accounts):
                 yield stmt_entry
         yield entry
 
 
 def _extract_related_postings(entries: list[Directive], accounts: set[str]) -> Iterable[PostingToCompare]:
     for entry in entries:
         if not isinstance(entry, Transaction):
```

