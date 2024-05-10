# Comparing `tmp/secondtrycpp-0.1.8.tar.gz` & `tmp/secondtrycpp-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secondtrycpp-0.1.8.tar", max compression
+gzip compressed data, was "secondtrycpp-0.1.9.tar", max compression
```

## Comparing `secondtrycpp-0.1.8.tar` & `secondtrycpp-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2024-05-10 15:25:54.678404 secondtrycpp-0.1.8/README.md
--rw-r--r--   0        0        0      283 2024-05-10 19:37:55.297472 secondtrycpp-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       18 2024-05-10 15:38:17.005007 secondtrycpp-0.1.8/secondtrycpp/__init__.py
--rw-r--r--   0        0        0       92 2024-05-10 15:26:42.489654 secondtrycpp-0.1.8/secondtrycpp/a.cpp
--rwxr-xr-x   0        0        0    15776 2024-05-10 15:27:27.916941 secondtrycpp-0.1.8/secondtrycpp/a.so
--rw-r--r--   0        0        0      440 2024-05-10 19:37:32.818227 secondtrycpp-0.1.8/secondtrycpp/b.py
--rw-r--r--   0        0        0      404 1970-01-01 00:00:00.000000 secondtrycpp-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-10 15:25:54.678404 secondtrycpp-0.1.9/README.md
+-rw-r--r--   0        0        0      283 2024-05-10 19:38:33.928175 secondtrycpp-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       18 2024-05-10 19:38:28.788347 secondtrycpp-0.1.9/secondtrycpp/__init__.py
+-rw-r--r--   0        0        0       92 2024-05-10 15:26:42.489654 secondtrycpp-0.1.9/secondtrycpp/a.cpp
+-rwxr-xr-x   0        0        0    15776 2024-05-10 15:27:27.916941 secondtrycpp-0.1.9/secondtrycpp/a.so
+-rw-r--r--   0        0        0      440 2024-05-10 19:37:32.818227 secondtrycpp-0.1.9/secondtrycpp/b.py
+-rw-r--r--   0        0        0      404 1970-01-01 00:00:00.000000 secondtrycpp-0.1.9/PKG-INFO
```

### Comparing `secondtrycpp-0.1.8/secondtrycpp/a.so` & `secondtrycpp-0.1.9/secondtrycpp/a.so`

 * *Files identical despite different names*

