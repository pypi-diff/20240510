# Comparing `tmp/secondtrycpp-0.1.6.tar.gz` & `tmp/secondtrycpp-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secondtrycpp-0.1.6.tar", max compression
+gzip compressed data, was "secondtrycpp-0.1.7.tar", max compression
```

## Comparing `secondtrycpp-0.1.6.tar` & `secondtrycpp-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2024-05-10 15:25:54.678404 secondtrycpp-0.1.6/README.md
--rw-r--r--   0        0        0      283 2024-05-10 16:37:31.231440 secondtrycpp-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       18 2024-05-10 15:38:17.005007 secondtrycpp-0.1.6/secondtrycpp/__init__.py
--rw-r--r--   0        0        0       92 2024-05-10 15:26:42.489654 secondtrycpp-0.1.6/secondtrycpp/a.cpp
--rwxr-xr-x   0        0        0    15776 2024-05-10 15:27:27.916941 secondtrycpp-0.1.6/secondtrycpp/a.so
--rw-r--r--   0        0        0      444 2024-05-10 16:37:21.889183 secondtrycpp-0.1.6/secondtrycpp/b.py
--rw-r--r--   0        0        0      404 1970-01-01 00:00:00.000000 secondtrycpp-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-10 15:25:54.678404 secondtrycpp-0.1.7/README.md
+-rw-r--r--   0        0        0      283 2024-05-10 16:51:02.214690 secondtrycpp-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0       18 2024-05-10 15:38:17.005007 secondtrycpp-0.1.7/secondtrycpp/__init__.py
+-rw-r--r--   0        0        0       92 2024-05-10 15:26:42.489654 secondtrycpp-0.1.7/secondtrycpp/a.cpp
+-rwxr-xr-x   0        0        0    15776 2024-05-10 15:27:27.916941 secondtrycpp-0.1.7/secondtrycpp/a.so
+-rw-r--r--   0        0        0      497 2024-05-10 16:50:54.271857 secondtrycpp-0.1.7/secondtrycpp/b.py
+-rw-r--r--   0        0        0      404 1970-01-01 00:00:00.000000 secondtrycpp-0.1.7/PKG-INFO
```

### Comparing `secondtrycpp-0.1.6/secondtrycpp/a.so` & `secondtrycpp-0.1.7/secondtrycpp/a.so`

 * *Files identical despite different names*

