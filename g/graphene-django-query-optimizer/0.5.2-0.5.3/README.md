# Comparing `tmp/graphene_django_query_optimizer-0.5.2.tar.gz` & `tmp/graphene_django_query_optimizer-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphene_django_query_optimizer-0.5.2.tar", max compression
+gzip compressed data, was "graphene_django_query_optimizer-0.5.3.tar", max compression
```

## Comparing `graphene_django_query_optimizer-0.5.2.tar` & `graphene_django_query_optimizer-0.5.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1064 2024-04-18 09:38:52.432274 graphene_django_query_optimizer-0.5.2/LICENSE
--rw-r--r--   0        0        0     3151 2024-04-18 09:38:52.432274 graphene_django_query_optimizer-0.5.2/README.md
--rw-r--r--   0        0        0     6905 2024-04-18 09:38:52.432274 graphene_django_query_optimizer-0.5.2/pyproject.toml
--rw-r--r--   0        0        0      496 2024-04-18 09:38:52.432274 graphene_django_query_optimizer-0.5.2/query_optimizer/__init__.py
--rw-r--r--   0        0        0    11972 2024-04-18 09:38:52.432274 graphene_django_query_optimizer-0.5.2/query_optimizer/ast.py
--rw-r--r--   0        0        0     8683 2024-04-18 09:38:52.432274 graphene_django_query_optimizer-0.5.2/query_optimizer/compiler.py
--rw-r--r--   0        0        0     2847 2024-04-18 09:38:52.432274 graphene_django_query_optimizer-0.5.2/query_optimizer/converters.py
--rw-r--r--   0        0        0      177 2024-04-18 09:38:52.432274 graphene_django_query_optimizer-0.5.2/query_optimizer/errors.py
--rw-r--r--   0        0        0    15533 2024-04-18 09:38:52.432274 graphene_django_query_optimizer-0.5.2/query_optimizer/fields.py
--rw-r--r--   0        0        0     1686 2024-04-18 09:38:52.432274 graphene_django_query_optimizer-0.5.2/query_optimizer/filter.py
--rw-r--r--   0        0        0     5239 2024-04-18 09:38:52.432274 graphene_django_query_optimizer-0.5.2/query_optimizer/filter_info.py
--rw-r--r--   0        0        0    10870 2024-04-18 09:38:52.432274 graphene_django_query_optimizer-0.5.2/query_optimizer/optimizer.py
--rw-r--r--   0        0        0     4130 2024-04-18 09:38:52.432274 graphene_django_query_optimizer-0.5.2/query_optimizer/prefetch_hack.py
--rw-r--r--   0        0        0        0 2024-04-18 09:38:52.432274 graphene_django_query_optimizer-0.5.2/query_optimizer/py.typed
--rw-r--r--   0        0        0     3529 2024-04-18 09:38:52.432274 graphene_django_query_optimizer-0.5.2/query_optimizer/selections.py
--rw-r--r--   0        0        0     2520 2024-04-18 09:38:52.432274 graphene_django_query_optimizer-0.5.2/query_optimizer/settings.py
--rw-r--r--   0        0        0     2996 2024-04-18 09:38:52.432274 graphene_django_query_optimizer-0.5.2/query_optimizer/types.py
--rw-r--r--   0        0        0     3661 2024-04-18 09:38:52.432274 graphene_django_query_optimizer-0.5.2/query_optimizer/typing.py
--rw-r--r--   0        0        0     6141 2024-04-18 09:38:52.432274 graphene_django_query_optimizer-0.5.2/query_optimizer/utils.py
--rw-r--r--   0        0        0     3840 2024-04-18 09:38:52.432274 graphene_django_query_optimizer-0.5.2/query_optimizer/validators.py
--rw-r--r--   0        0        0     4694 1970-01-01 00:00:00.000000 graphene_django_query_optimizer-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-10 16:32:46.895758 graphene_django_query_optimizer-0.5.3/LICENSE
+-rw-r--r--   0        0        0     3151 2024-05-10 16:32:46.895758 graphene_django_query_optimizer-0.5.3/README.md
+-rw-r--r--   0        0        0     6906 2024-05-10 16:32:46.899758 graphene_django_query_optimizer-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0      496 2024-05-10 16:32:46.899758 graphene_django_query_optimizer-0.5.3/query_optimizer/__init__.py
+-rw-r--r--   0        0        0    11972 2024-05-10 16:32:46.899758 graphene_django_query_optimizer-0.5.3/query_optimizer/ast.py
+-rw-r--r--   0        0        0     8683 2024-05-10 16:32:46.899758 graphene_django_query_optimizer-0.5.3/query_optimizer/compiler.py
+-rw-r--r--   0        0        0     2847 2024-05-10 16:32:46.899758 graphene_django_query_optimizer-0.5.3/query_optimizer/converters.py
+-rw-r--r--   0        0        0      177 2024-05-10 16:32:46.899758 graphene_django_query_optimizer-0.5.3/query_optimizer/errors.py
+-rw-r--r--   0        0        0    15533 2024-05-10 16:32:46.899758 graphene_django_query_optimizer-0.5.3/query_optimizer/fields.py
+-rw-r--r--   0        0        0     1686 2024-05-10 16:32:46.899758 graphene_django_query_optimizer-0.5.3/query_optimizer/filter.py
+-rw-r--r--   0        0        0     5239 2024-05-10 16:32:46.899758 graphene_django_query_optimizer-0.5.3/query_optimizer/filter_info.py
+-rw-r--r--   0        0        0    10870 2024-05-10 16:32:46.899758 graphene_django_query_optimizer-0.5.3/query_optimizer/optimizer.py
+-rw-r--r--   0        0        0     4130 2024-05-10 16:32:46.899758 graphene_django_query_optimizer-0.5.3/query_optimizer/prefetch_hack.py
+-rw-r--r--   0        0        0        0 2024-05-10 16:32:46.899758 graphene_django_query_optimizer-0.5.3/query_optimizer/py.typed
+-rw-r--r--   0        0        0     3529 2024-05-10 16:32:46.899758 graphene_django_query_optimizer-0.5.3/query_optimizer/selections.py
+-rw-r--r--   0        0        0     2520 2024-05-10 16:32:46.899758 graphene_django_query_optimizer-0.5.3/query_optimizer/settings.py
+-rw-r--r--   0        0        0     2996 2024-05-10 16:32:46.899758 graphene_django_query_optimizer-0.5.3/query_optimizer/types.py
+-rw-r--r--   0        0        0     3661 2024-05-10 16:32:46.899758 graphene_django_query_optimizer-0.5.3/query_optimizer/typing.py
+-rw-r--r--   0        0        0     6141 2024-05-10 16:32:46.899758 graphene_django_query_optimizer-0.5.3/query_optimizer/utils.py
+-rw-r--r--   0        0        0     3888 2024-05-10 16:32:46.899758 graphene_django_query_optimizer-0.5.3/query_optimizer/validators.py
+-rw-r--r--   0        0        0     4694 1970-01-01 00:00:00.000000 graphene_django_query_optimizer-0.5.3/PKG-INFO
```

### Comparing `graphene_django_query_optimizer-0.5.2/LICENSE` & `graphene_django_query_optimizer-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.2/README.md` & `graphene_django_query_optimizer-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.2/pyproject.toml` & `graphene_django_query_optimizer-0.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "graphene-django-query-optimizer"
-version = "0.5.2"
+version = "0.5.3"
 description = "Automatically optimize SQL queries in Graphene-Django schemas."
 authors = [
     "Matti Lamppu <lamppu.matti.akseli@gmail.com>",
 ]
 packages = [
     { include = "query_optimizer" },
 ]
@@ -56,34 +56,34 @@
 typing-extensions = { version = ">=4.7.1", python = "<3.10" }
 django-settings-holder = ">=0.1.2"
 
 [tool.poetry.extras]
 filter = ["django-filter"]
 
 [tool.poetry.group.test.dependencies]
-pytest = "8.1.1"
-coverage = "7.4.4"
+pytest = "8.2.0"
+coverage = "7.5.1"
 pytest-django = "4.8.0"
 pre-commit = "3.7.0"
-tox = "4.14.2"
+tox = "4.15.0"
 tox-gh-actions = "3.2.0"
-faker = "24.9.0"
+faker = "25.0.1"
 factory-boy = "3.3.0"
 sqlparse = "0.5.0"
 django-graphiql-debug-toolbar = "0.2.0"
 py-spy = "0.3.14"
 
 [tool.poetry.group.docs.dependencies]
-mkdocs = "1.5.3"
-pymdown-extensions = "10.7.1"
+mkdocs = "1.6.0"
+pymdown-extensions = "10.8.1"
 mkdocs-mermaid2-plugin = "1.1.1"
 
 [tool.poetry.group.lint.dependencies]
-mypy = "1.9.0"
-django-stubs = "4.2.7"
+mypy = "1.10.0"
+django-stubs = "5.0.0"
 
 [tool.ruff]
 fix = true
 line-length = 120
 extend-exclude = [
     "tests/*",
 ]
```

### Comparing `graphene_django_query_optimizer-0.5.2/query_optimizer/ast.py` & `graphene_django_query_optimizer-0.5.3/query_optimizer/ast.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.2/query_optimizer/compiler.py` & `graphene_django_query_optimizer-0.5.3/query_optimizer/compiler.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.2/query_optimizer/converters.py` & `graphene_django_query_optimizer-0.5.3/query_optimizer/converters.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.2/query_optimizer/fields.py` & `graphene_django_query_optimizer-0.5.3/query_optimizer/fields.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.2/query_optimizer/filter.py` & `graphene_django_query_optimizer-0.5.3/query_optimizer/filter.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.2/query_optimizer/filter_info.py` & `graphene_django_query_optimizer-0.5.3/query_optimizer/filter_info.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.2/query_optimizer/optimizer.py` & `graphene_django_query_optimizer-0.5.3/query_optimizer/optimizer.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.2/query_optimizer/prefetch_hack.py` & `graphene_django_query_optimizer-0.5.3/query_optimizer/prefetch_hack.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.2/query_optimizer/selections.py` & `graphene_django_query_optimizer-0.5.3/query_optimizer/selections.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.2/query_optimizer/settings.py` & `graphene_django_query_optimizer-0.5.3/query_optimizer/settings.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.2/query_optimizer/types.py` & `graphene_django_query_optimizer-0.5.3/query_optimizer/types.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.2/query_optimizer/typing.py` & `graphene_django_query_optimizer-0.5.3/query_optimizer/typing.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.2/query_optimizer/utils.py` & `graphene_django_query_optimizer-0.5.3/query_optimizer/utils.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.2/query_optimizer/validators.py` & `graphene_django_query_optimizer-0.5.3/query_optimizer/validators.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,22 +65,23 @@
     if isinstance(max_limit, int) and first is None and last is None:
         first = max_limit
 
     if offset is not None:
         if after is not None or before is not None:
             msg = "Can only use either `offset` or `before`/`after` for pagination."
             raise ValueError(msg)
-        if not isinstance(offset, int) or offset <= 0:
+        if not isinstance(offset, int) or offset < 0:
             msg = "Argument `offset` must be a positive integer."
             raise ValueError(msg)
 
         # Convert offset to after cursor value. Note that after cursor dictates
         # a value _after_ which results should be returned, so we need to subtract
         # 1 from the offset to get the correct cursor value.
-        after = offset - 1
+        if offset > 0:  # ignore zero offset
+            after = offset - 1
 
     if after is not None and (not isinstance(after, int) or after < 0):
         msg = "The node pointed with `after` does not exist."
         raise ValueError(msg)
 
     if before is not None and (not isinstance(before, int) or before < 0):
         msg = "The node pointed with `before` does not exist."
```

### Comparing `graphene_django_query_optimizer-0.5.2/PKG-INFO` & `graphene_django_query_optimizer-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphene-django-query-optimizer
-Version: 0.5.2
+Version: 0.5.3
 Summary: Automatically optimize SQL queries in Graphene-Django schemas.
 Home-page: https://mrthearman.github.io/graphene-django-query-optimizer
 License: MIT
 Keywords: django,graphene,sql,graphql,python,query,optimizer,optimization
 Author: Matti Lamppu
 Author-email: lamppu.matti.akseli@gmail.com
 Requires-Python: >=3.9,<4
```

