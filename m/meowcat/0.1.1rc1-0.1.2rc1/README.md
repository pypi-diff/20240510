# Comparing `tmp/meowcat-0.1.1rc1.tar.gz` & `tmp/meowcat-0.1.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meowcat-0.1.1rc1.tar", max compression
+gzip compressed data, was "meowcat-0.1.2rc1.tar", max compression
```

## Comparing `meowcat-0.1.1rc1.tar` & `meowcat-0.1.2rc1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2024-05-10 11:25:09.597047 meowcat-0.1.1rc1/README.md
--rw-r--r--   0        0        0        0 2024-05-10 11:25:09.597004 meowcat-0.1.1rc1/meowcat/__init__.py
--rw-r--r--   0        0        0      265 2024-05-10 11:28:47.870625 meowcat-0.1.1rc1/pyproject.toml
--rw-r--r--   0        0        0      335 1970-01-01 00:00:00.000000 meowcat-0.1.1rc1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-10 11:25:09.597047 meowcat-0.1.2rc1/README.md
+-rw-r--r--   0        0        0        0 2024-05-10 11:25:09.597004 meowcat-0.1.2rc1/meowcat/__init__.py
+-rw-r--r--   0        0        0      219 2024-05-10 12:03:47.620139 meowcat-0.1.2rc1/pyproject.toml
+-rw-r--r--   0        0        0      755 1970-01-01 00:00:00.000000 meowcat-0.1.2rc1/PKG-INFO
```

