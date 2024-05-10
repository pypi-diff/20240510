# Comparing `tmp/secondtrycpp-0.1.3.tar.gz` & `tmp/secondtrycpp-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secondtrycpp-0.1.3.tar", max compression
+gzip compressed data, was "secondtrycpp-0.1.4.tar", max compression
```

## Comparing `secondtrycpp-0.1.3.tar` & `secondtrycpp-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2024-05-10 15:25:54.678404 secondtrycpp-0.1.3/README.md
--rw-r--r--   0        0        0      283 2024-05-10 15:38:28.552163 secondtrycpp-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       18 2024-05-10 15:38:17.005007 secondtrycpp-0.1.3/secondtrycpp/__init__.py
--rw-r--r--   0        0        0       92 2024-05-10 15:26:42.489654 secondtrycpp-0.1.3/secondtrycpp/a.cpp
--rwxr-xr-x   0        0        0    15776 2024-05-10 15:27:27.916941 secondtrycpp-0.1.3/secondtrycpp/a.so
--rw-r--r--   0        0        0      382 2024-05-10 15:35:20.350445 secondtrycpp-0.1.3/secondtrycpp/b.py
--rw-r--r--   0        0        0      404 1970-01-01 00:00:00.000000 secondtrycpp-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-10 15:25:54.678404 secondtrycpp-0.1.4/README.md
+-rw-r--r--   0        0        0      283 2024-05-10 15:40:01.348319 secondtrycpp-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       18 2024-05-10 15:38:17.005007 secondtrycpp-0.1.4/secondtrycpp/__init__.py
+-rw-r--r--   0        0        0       92 2024-05-10 15:26:42.489654 secondtrycpp-0.1.4/secondtrycpp/a.cpp
+-rwxr-xr-x   0        0        0    15776 2024-05-10 15:27:27.916941 secondtrycpp-0.1.4/secondtrycpp/a.so
+-rw-r--r--   0        0        0      369 2024-05-10 15:39:57.597877 secondtrycpp-0.1.4/secondtrycpp/b.py
+-rw-r--r--   0        0        0      404 1970-01-01 00:00:00.000000 secondtrycpp-0.1.4/PKG-INFO
```

### Comparing `secondtrycpp-0.1.3/secondtrycpp/a.so` & `secondtrycpp-0.1.4/secondtrycpp/a.so`

 * *Files identical despite different names*

