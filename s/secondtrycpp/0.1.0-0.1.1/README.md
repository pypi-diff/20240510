# Comparing `tmp/secondtrycpp-0.1.0.tar.gz` & `tmp/secondtrycpp-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secondtrycpp-0.1.0.tar", max compression
+gzip compressed data, was "secondtrycpp-0.1.1.tar", max compression
```

## Comparing `secondtrycpp-0.1.0.tar` & `secondtrycpp-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-05-10 15:25:54.678404 secondtrycpp-0.1.0/README.md
--rw-r--r--   0        0        0      283 2024-05-10 15:25:54.682404 secondtrycpp-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-10 15:25:54.678404 secondtrycpp-0.1.0/secondtrycpp/__init__.py
--rw-r--r--   0        0        0       92 2024-05-10 15:26:42.489654 secondtrycpp-0.1.0/secondtrycpp/a.cpp
--rw-r--r--   0        0        0      368 2024-05-10 15:28:03.204388 secondtrycpp-0.1.0/secondtrycpp/a.py
--rw-r--r--   0        0        0      404 1970-01-01 00:00:00.000000 secondtrycpp-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-10 15:25:54.678404 secondtrycpp-0.1.1/README.md
+-rw-r--r--   0        0        0      283 2024-05-10 15:29:38.618890 secondtrycpp-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       18 2024-05-10 15:29:03.091448 secondtrycpp-0.1.1/secondtrycpp/__init__.py
+-rw-r--r--   0        0        0       92 2024-05-10 15:26:42.489654 secondtrycpp-0.1.1/secondtrycpp/a.cpp
+-rw-r--r--   0        0        0      368 2024-05-10 15:28:03.204388 secondtrycpp-0.1.1/secondtrycpp/a.py
+-rw-r--r--   0        0        0      404 1970-01-01 00:00:00.000000 secondtrycpp-0.1.1/PKG-INFO
```

