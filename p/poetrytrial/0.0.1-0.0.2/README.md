# Comparing `tmp/poetrytrial-0.0.1.tar.gz` & `tmp/poetrytrial-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetrytrial-0.0.1.tar", max compression
+gzip compressed data, was "poetrytrial-0.0.2.tar", max compression
```

## Comparing `poetrytrial-0.0.1.tar` & `poetrytrial-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1091 2024-05-02 20:47:16.563924 poetrytrial-0.0.1/LICENSE
--rw-r--r--   0        0        0      187 2024-05-10 00:12:26.346059 poetrytrial-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-02 20:39:36.915138 poetrytrial-0.0.1/src/poetrytrial/__init__.py
--rw-r--r--   0        0        0       43 2024-05-02 21:17:30.984394 poetrytrial-0.0.1/src/poetrytrial/example.py
--rw-r--r--   0        0        0      266 1970-01-01 00:00:00.000000 poetrytrial-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2024-05-02 20:47:16.563924 poetrytrial-0.0.2/LICENSE
+-rw-r--r--   0        0        0      202 2024-05-10 01:31:50.623602 poetrytrial-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-02 20:39:36.915138 poetrytrial-0.0.2/src/poetrytrial/__init__.py
+-rw-r--r--   0        0        0       43 2024-05-02 21:17:30.984394 poetrytrial-0.0.2/src/poetrytrial/example.py
+-rw-r--r--   0        0        0      303 1970-01-01 00:00:00.000000 poetrytrial-0.0.2/PKG-INFO
```

### Comparing `poetrytrial-0.0.1/LICENSE` & `poetrytrial-0.0.2/LICENSE`

 * *Files identical despite different names*

