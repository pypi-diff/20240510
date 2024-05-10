# Comparing `tmp/tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.1.tar.gz` & `tmp/tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.1.tar", last modified: Fri May 10 14:35:42 2024, max compression
+gzip compressed data, was "tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.2.tar", last modified: Fri May 10 14:40:48 2024, max compression
```

## Comparing `tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.1.tar` & `tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-05-10 14:35:42.233625 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.1/
--rw-r--r--   0 test      (1000) test      (1000)      126 2024-05-10 14:35:42.233625 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.1/PKG-INFO
--rw-rw-r--   0 test      (1000) test      (1000)      211 2024-05-10 10:01:14.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.1/pyproject.toml
--rw-rw-r--   0 test      (1000) test      (1000)       38 2024-05-10 14:35:42.233625 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.1/setup.cfg
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-05-10 14:35:42.229625 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.1/src/
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-05-10 14:35:42.233625 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.1/src/tp_sql/
--rw-rw-r--   0 test      (1000) test      (1000)     2552 2024-05-10 14:34:56.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.1/src/tp_sql/main.py
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-05-10 14:35:42.233625 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.1/src/tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064.egg-info/
--rw-r--r--   0 test      (1000) test      (1000)      126 2024-05-10 14:35:42.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.1/src/tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064.egg-info/PKG-INFO
--rw-rw-r--   0 test      (1000) test      (1000)      387 2024-05-10 14:35:42.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.1/src/tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064.egg-info/SOURCES.txt
--rw-rw-r--   0 test      (1000) test      (1000)        1 2024-05-10 14:35:42.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.1/src/tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064.egg-info/dependency_links.txt
--rw-rw-r--   0 test      (1000) test      (1000)       24 2024-05-10 14:35:42.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.1/src/tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064.egg-info/requires.txt
--rw-rw-r--   0 test      (1000) test      (1000)        7 2024-05-10 14:35:42.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.1/src/tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064.egg-info/top_level.txt
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-05-10 14:40:48.527428 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.2/
+-rw-r--r--   0 test      (1000) test      (1000)      126 2024-05-10 14:40:48.523428 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.2/PKG-INFO
+-rw-rw-r--   0 test      (1000) test      (1000)      211 2024-05-10 14:39:37.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.2/pyproject.toml
+-rw-rw-r--   0 test      (1000) test      (1000)       38 2024-05-10 14:40:48.527428 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.2/setup.cfg
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-05-10 14:40:48.507428 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.2/src/
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-05-10 14:40:48.511427 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.2/src/tp_sql/
+-rw-rw-r--   0 test      (1000) test      (1000)     2552 2024-05-10 14:34:56.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.2/src/tp_sql/main.py
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-05-10 14:40:48.523428 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.2/src/tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064.egg-info/
+-rw-r--r--   0 test      (1000) test      (1000)      126 2024-05-10 14:40:48.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.2/src/tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064.egg-info/PKG-INFO
+-rw-rw-r--   0 test      (1000) test      (1000)      387 2024-05-10 14:40:48.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.2/src/tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064.egg-info/SOURCES.txt
+-rw-rw-r--   0 test      (1000) test      (1000)        1 2024-05-10 14:40:48.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.2/src/tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064.egg-info/dependency_links.txt
+-rw-rw-r--   0 test      (1000) test      (1000)       24 2024-05-10 14:40:48.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.2/src/tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064.egg-info/requires.txt
+-rw-rw-r--   0 test      (1000) test      (1000)        7 2024-05-10 14:40:48.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.2/src/tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064.egg-info/top_level.txt
```

### Comparing `tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.1/src/tp_sql/main.py` & `tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.2/src/tp_sql/main.py`

 * *Files identical despite different names*

