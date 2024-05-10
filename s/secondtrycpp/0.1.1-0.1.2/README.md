# Comparing `tmp/secondtrycpp-0.1.1.tar.gz` & `tmp/secondtrycpp-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secondtrycpp-0.1.1.tar", max compression
+gzip compressed data, was "secondtrycpp-0.1.2.tar", max compression
```

## Comparing `secondtrycpp-0.1.1.tar` & `secondtrycpp-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0        0 2024-05-10 15:25:54.678404 secondtrycpp-0.1.1/README.md
--rw-r--r--   0        0        0      283 2024-05-10 15:29:38.618890 secondtrycpp-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       18 2024-05-10 15:29:03.091448 secondtrycpp-0.1.1/secondtrycpp/__init__.py
--rw-r--r--   0        0        0       92 2024-05-10 15:26:42.489654 secondtrycpp-0.1.1/secondtrycpp/a.cpp
--rw-r--r--   0        0        0      368 2024-05-10 15:28:03.204388 secondtrycpp-0.1.1/secondtrycpp/a.py
--rw-r--r--   0        0        0      404 1970-01-01 00:00:00.000000 secondtrycpp-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-10 15:25:54.678404 secondtrycpp-0.1.2/README.md
+-rw-r--r--   0        0        0      283 2024-05-10 15:35:44.605597 secondtrycpp-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       18 2024-05-10 15:29:03.091448 secondtrycpp-0.1.2/secondtrycpp/__init__.py
+-rw-r--r--   0        0        0       92 2024-05-10 15:26:42.489654 secondtrycpp-0.1.2/secondtrycpp/a.cpp
+-rw-r--r--   0        0        0      382 2024-05-10 15:35:20.350445 secondtrycpp-0.1.2/secondtrycpp/a.py
+-rwxr-xr-x   0        0        0    15776 2024-05-10 15:27:27.916941 secondtrycpp-0.1.2/secondtrycpp/a.so
+-rw-r--r--   0        0        0      404 1970-01-01 00:00:00.000000 secondtrycpp-0.1.2/PKG-INFO
```

