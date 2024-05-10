# Comparing `tmp/docmesh_cli-0.0.1.tar.gz` & `tmp/docmesh_cli-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docmesh_cli-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "docmesh_cli-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `docmesh_cli-0.0.1.tar` & `docmesh_cli-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       16 2024-05-09 06:03:26.957936 docmesh_cli-0.0.1/README.md
--rw-r--r--   0        0        0       83 2024-05-09 05:44:56.516666 docmesh_cli-0.0.1/docmesh_cli/__init__.py
--rw-r--r--   0        0        0     1874 2024-05-09 05:16:46.269763 docmesh_cli-0.0.1/docmesh_cli/client.py
--rw-r--r--   0        0        0      598 2024-05-09 05:29:56.398617 docmesh_cli-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      417 1970-01-01 00:00:00.000000 docmesh_cli-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       17 2024-05-09 08:25:56.000000 docmesh_cli-0.0.2/README.md
+-rw-r--r--   0        0        0       83 2024-05-10 03:25:30.838495 docmesh_cli-0.0.2/docmesh_cli/__init__.py
+-rw-r--r--   0        0        0     4075 2024-05-10 03:25:06.242493 docmesh_cli-0.0.2/docmesh_cli/client.py
+-rw-r--r--   0        0        0      598 2024-05-09 05:29:56.000000 docmesh_cli-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 docmesh_cli-0.0.2/PKG-INFO
```

### Comparing `docmesh_cli-0.0.1/pyproject.toml` & `docmesh_cli-0.0.2/pyproject.toml`

 * *Files identical despite different names*

