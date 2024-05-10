# Comparing `tmp/python-snippets-0.0.49.tar.gz` & `tmp/python-snippets-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-snippets-0.0.49.tar", last modified: Fri May 10 06:40:05 2024, max compression
+gzip compressed data, was "python-snippets-0.0.6.tar", last modified: Tue Nov  1 06:44:17 2022, max compression
```

## Comparing `python-snippets-0.0.49.tar` & `python-snippets-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,16 @@
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-05-10 06:40:05.839381 python-snippets-0.0.49/
--rw-r--r--   0 chenhao    (501) staff       (20)      426 2024-05-10 06:40:05.839058 python-snippets-0.0.49/PKG-INFO
--rw-r--r--   0 chenhao    (501) staff       (20)       98 2022-05-31 09:28:56.000000 python-snippets-0.0.49/README.md
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-05-10 06:40:05.838135 python-snippets-0.0.49/python_snippets.egg-info/
--rw-r--r--   0 chenhao    (501) staff       (20)      426 2024-05-10 06:40:05.000000 python-snippets-0.0.49/python_snippets.egg-info/PKG-INFO
--rw-r--r--   0 chenhao    (501) staff       (20)      440 2024-05-10 06:40:05.000000 python-snippets-0.0.49/python_snippets.egg-info/SOURCES.txt
--rw-r--r--   0 chenhao    (501) staff       (20)        1 2024-05-10 06:40:05.000000 python-snippets-0.0.49/python_snippets.egg-info/dependency_links.txt
--rw-r--r--   0 chenhao    (501) staff       (20)       58 2024-05-10 06:40:05.000000 python-snippets-0.0.49/python_snippets.egg-info/requires.txt
--rw-r--r--   0 chenhao    (501) staff       (20)        9 2024-05-10 06:40:05.000000 python-snippets-0.0.49/python_snippets.egg-info/top_level.txt
--rw-r--r--   0 chenhao    (501) staff       (20)        1 2024-05-10 06:40:05.000000 python-snippets-0.0.49/python_snippets.egg-info/zip-safe
--rw-r--r--   0 chenhao    (501) staff       (20)       38 2024-05-10 06:40:05.839426 python-snippets-0.0.49/setup.cfg
--rwxr-xr-x   0 chenhao    (501) staff       (20)     1407 2024-02-04 07:32:57.000000 python-snippets-0.0.49/setup.py
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-05-10 06:40:05.836233 python-snippets-0.0.49/snippets/
--rw-r--r--   0 chenhao    (501) staff       (20)      562 2024-03-07 03:20:54.000000 python-snippets-0.0.49/snippets/__init__.py
--rw-r--r--   0 chenhao    (501) staff       (20)     7200 2024-04-25 07:10:58.000000 python-snippets-0.0.49/snippets/decorators.py
--rw-r--r--   0 chenhao    (501) staff       (20)     2936 2024-02-04 07:37:02.000000 python-snippets-0.0.49/snippets/evaluate.py
--rw-r--r--   0 chenhao    (501) staff       (20)     4489 2024-05-09 07:49:33.000000 python-snippets-0.0.49/snippets/logs.py
--rw-r--r--   0 chenhao    (501) staff       (20)      560 2023-10-19 10:20:06.000000 python-snippets-0.0.49/snippets/mixin.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1875 2024-03-07 02:56:24.000000 python-snippets-0.0.49/snippets/perf.py
--rw-r--r--   0 chenhao    (501) staff       (20)    14423 2024-05-06 07:05:18.000000 python-snippets-0.0.49/snippets/utils.py
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-05-10 06:40:05.838703 python-snippets-0.0.49/tests/
--rw-r--r--   0 chenhao    (501) staff       (20)     2412 2024-04-22 08:12:09.000000 python-snippets-0.0.49/tests/test_decorators.py
--rw-r--r--   0 chenhao    (501) staff       (20)     2416 2024-04-30 02:27:39.000000 python-snippets-0.0.49/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 06:44:17.188819 python-snippets-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (121)      247 2022-11-01 06:44:17.188819 python-snippets-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       98 2022-11-01 06:44:01.000000 python-snippets-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 06:44:17.188819 python-snippets-0.0.6/python_snippets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      247 2022-11-01 06:44:17.000000 python-snippets-0.0.6/python_snippets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      314 2022-11-01 06:44:17.000000 python-snippets-0.0.6/python_snippets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 06:44:17.000000 python-snippets-0.0.6/python_snippets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-11-01 06:44:17.000000 python-snippets-0.0.6/python_snippets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-11-01 06:44:17.000000 python-snippets-0.0.6/python_snippets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 06:44:16.000000 python-snippets-0.0.6/python_snippets.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 06:44:17.188819 python-snippets-0.0.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)      849 2022-11-01 06:44:01.000000 python-snippets-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 06:44:17.188819 python-snippets-0.0.6/snippets/
+-rw-r--r--   0 runner    (1001) docker     (121)      514 2022-11-01 06:44:01.000000 python-snippets-0.0.6/snippets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3459 2022-11-01 06:44:01.000000 python-snippets-0.0.6/snippets/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7856 2022-11-01 06:44:01.000000 python-snippets-0.0.6/snippets/utils.py
```

