# Comparing `tmp/zboxapi-0.0.2.tar.gz` & `tmp/zboxapi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zboxapi-0.0.2.tar", max compression
+gzip compressed data, was "zboxapi-0.0.3.tar", max compression
```

## Comparing `zboxapi-0.0.2.tar` & `zboxapi-0.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1297 2024-05-07 19:02:19.662896 zboxapi-0.0.2/README.md
--rw-r--r--   0        0        0      897 2024-05-08 18:17:32.642603 zboxapi-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       22 2024-05-08 18:17:32.646603 zboxapi-0.0.2/src/zboxapi/__init__.py
--rw-r--r--   0        0        0     7041 2024-05-08 17:44:28.545019 zboxapi-0.0.2/src/zboxapi/main.py
--rw-r--r--   0        0        0     1693 1970-01-01 00:00:00.000000 zboxapi-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      545 2024-05-10 14:13:39.488068 zboxapi-0.0.3/README.md
+-rw-r--r--   0        0        0      896 2024-05-10 14:16:38.496339 zboxapi-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-10 14:16:38.504339 zboxapi-0.0.3/src/zboxapi/__init__.py
+-rw-r--r--   0        0        0     7041 2024-05-08 17:44:28.545019 zboxapi-0.0.3/src/zboxapi/main.py
+-rw-r--r--   0        0        0     1043 1970-01-01 00:00:00.000000 zboxapi-0.0.3/PKG-INFO
```

### Comparing `zboxapi-0.0.2/pyproject.toml` & `zboxapi-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "zboxapi"
-version = "0.0.2"
+version = "0.0.3"
 description = ""
 authors = ["Kelby Valenti <kelby.valenti@gmail.com>", "Timo Sugliani <timo.sugliani@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 zboxapi = "zboxapi.main:launch"
 
 [tool.poetry.dependencies]
 fastapi = "0.111.0"
-python = ">=3.12"
+python = ">=3.10"
 uvicorn = "0.29.0"
 ipython = "^8.24.0"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.4"
 
 [build-system]
@@ -37,8 +37,7 @@
 
 [[tool.poetry_bumpversion.replacements]]
 files = [
     "src/zboxapi/__init__.py",
 ]
 search = '__version__ = "{current_version}"'
 replace = '__version__ = "{new_version}"'
-
```

### Comparing `zboxapi-0.0.2/src/zboxapi/main.py` & `zboxapi-0.0.3/src/zboxapi/main.py`

 * *Files identical despite different names*

