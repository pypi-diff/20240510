# Comparing `tmp/blendsql-0.0.13.tar.gz` & `tmp/blendsql-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blendsql-0.0.13.tar", last modified: Thu Mar 14 15:16:07 2024, max compression
+gzip compressed data, was "blendsql-0.0.14.tar", last modified: Thu May  9 19:14:44 2024, max compression
```

## Comparing `blendsql-0.0.13.tar` & `blendsql-0.0.14.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:16:07.917047 blendsql-0.0.13/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-14 15:16:03.000000 blendsql-0.0.13/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    26438 2024-03-14 15:16:07.917047 blendsql-0.0.13/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    24820 2024-03-14 15:16:03.000000 blendsql-0.0.13/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:16:07.909047 blendsql-0.0.13/blendsql/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-14 15:16:03.000000 blendsql-0.0.13/blendsql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-03-14 15:16:03.000000 blendsql-0.0.13/blendsql/_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-03-14 15:16:03.000000 blendsql-0.0.13/blendsql/_dialect.py
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-03-14 15:16:03.000000 blendsql-0.0.13/blendsql/_grammar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-03-14 15:16:03.000000 blendsql-0.0.13/blendsql/_program.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-03-14 15:16:03.000000 blendsql-0.0.13/blendsql/_smoothie.py
--rw-r--r--   0 runner    (1001) docker     (127)    27335 2024-03-14 15:16:03.000000 blendsql-0.0.13/blendsql/_sqlglot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-03-14 15:16:03.000000 blendsql-0.0.13/blendsql/blend_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    40768 2024-03-14 15:16:03.000000 blendsql-0.0.13/blendsql/blendsql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:16:07.913047 blendsql-0.0.13/blendsql/db/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-14 15:16:03.000000 blendsql-0.0.13/blendsql/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-03-14 15:16:03.000000 blendsql-0.0.13/blendsql/db/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-14 15:16:03.000000 blendsql-0.0.13/blendsql/db/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:16:07.913047 blendsql-0.0.13/blendsql/ingredients/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-03-14 15:16:03.000000 blendsql-0.0.13/blendsql/ingredients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:16:07.913047 blendsql-0.0.13/blendsql/ingredients/builtin/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-14 15:16:03.000000 blendsql-0.0.13/blendsql/ingredients/builtin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:16:07.913047 blendsql-0.0.13/blendsql/ingredients/builtin/dt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 15:16:03.000000 blendsql-0.0.13/blendsql/ingredients/builtin/dt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-03-14 15:16:03.000000 blendsql-0.0.13/blendsql/ingredients/builtin/dt/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-03-14 15:16:03.000000 blendsql-0.0.13/blendsql/ingredients/builtin/dt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:16:07.913047 blendsql-0.0.13/blendsql/ingredients/builtin/llm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 15:16:03.000000 blendsql-0.0.13/blendsql/ingredients/builtin/llm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:16:07.913047 blendsql-0.0.13/blendsql/ingredients/builtin/llm/join/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 15:16:03.000000 blendsql-0.0.13/blendsql/ingredients/builtin/llm/join/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-03-14 15:16:03.000000 blendsql-0.0.13/blendsql/ingredients/builtin/llm/join/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:16:07.913047 blendsql-0.0.13/blendsql/ingredients/builtin/llm/map/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-14 15:16:03.000000 blendsql-0.0.13/blendsql/ingredients/builtin/llm/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-03-14 15:16:03.000000 blendsql-0.0.13/blendsql/ingredients/builtin/llm/map/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:16:07.913047 blendsql-0.0.13/blendsql/ingredients/builtin/llm/qa/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-14 15:16:03.000000 blendsql-0.0.13/blendsql/ingredients/builtin/llm/qa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-03-14 15:16:03.000000 blendsql-0.0.13/blendsql/ingredients/builtin/llm/qa/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-03-14 15:16:03.000000 blendsql-0.0.13/blendsql/ingredients/builtin/llm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:16:07.913047 blendsql-0.0.13/blendsql/ingredients/builtin/llm/validate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 15:16:03.000000 blendsql-0.0.13/blendsql/ingredients/builtin/llm/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-03-14 15:16:03.000000 blendsql-0.0.13/blendsql/ingredients/builtin/llm/validate/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    14304 2024-03-14 15:16:03.000000 blendsql-0.0.13/blendsql/ingredients/ingredient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:16:07.913047 blendsql-0.0.13/blendsql/models/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-14 15:16:03.000000 blendsql-0.0.13/blendsql/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-03-14 15:16:03.000000 blendsql-0.0.13/blendsql/models/_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:16:07.913047 blendsql-0.0.13/blendsql/models/local/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 15:16:03.000000 blendsql-0.0.13/blendsql/models/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-03-14 15:16:03.000000 blendsql-0.0.13/blendsql/models/local/_transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:16:07.917047 blendsql-0.0.13/blendsql/models/remote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 15:16:03.000000 blendsql-0.0.13/blendsql/models/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-03-14 15:16:03.000000 blendsql-0.0.13/blendsql/models/remote/_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-03-14 15:16:03.000000 blendsql-0.0.13/blendsql/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:16:07.917047 blendsql-0.0.13/blendsql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    26438 2024-03-14 15:16:07.000000 blendsql-0.0.13/blendsql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-03-14 15:16:07.000000 blendsql-0.0.13/blendsql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 15:16:07.000000 blendsql-0.0.13/blendsql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-14 15:16:07.000000 blendsql-0.0.13/blendsql.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-14 15:16:07.000000 blendsql-0.0.13/blendsql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-14 15:16:07.000000 blendsql-0.0.13/blendsql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-03-14 15:16:03.000000 blendsql-0.0.13/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 15:16:07.917047 blendsql-0.0.13/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-03-14 15:16:03.000000 blendsql-0.0.13/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:16:07.917047 blendsql-0.0.13/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 15:16:03.000000 blendsql-0.0.13/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-03-14 15:16:03.000000 blendsql-0.0.13/tests/test_generic_blendsql.py
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-03-14 15:16:03.000000 blendsql-0.0.13/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    16381 2024-03-14 15:16:03.000000 blendsql-0.0.13/tests/test_multi_table_blendsql.py
--rw-r--r--   0 runner    (1001) docker     (127)    14557 2024-03-14 15:16:03.000000 blendsql-0.0.13/tests/test_single_table_blendsql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-03-14 15:16:03.000000 blendsql-0.0.13/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:14:44.733924 blendsql-0.0.14/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-09 19:14:40.000000 blendsql-0.0.14/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    26516 2024-05-09 19:14:44.733924 blendsql-0.0.14/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24889 2024-05-09 19:14:40.000000 blendsql-0.0.14/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:14:44.725923 blendsql-0.0.14/blendsql/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-09 19:14:40.000000 blendsql-0.0.14/blendsql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-09 19:14:40.000000 blendsql-0.0.14/blendsql/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-09 19:14:40.000000 blendsql-0.0.14/blendsql/_dialect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-09 19:14:40.000000 blendsql-0.0.14/blendsql/_grammar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-05-09 19:14:40.000000 blendsql-0.0.14/blendsql/_program.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-09 19:14:40.000000 blendsql-0.0.14/blendsql/_smoothie.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27335 2024-05-09 19:14:40.000000 blendsql-0.0.14/blendsql/_sqlglot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-09 19:14:40.000000 blendsql-0.0.14/blendsql/blend_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40768 2024-05-09 19:14:40.000000 blendsql-0.0.14/blendsql/blendsql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:14:44.725923 blendsql-0.0.14/blendsql/db/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-09 19:14:40.000000 blendsql-0.0.14/blendsql/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-05-09 19:14:40.000000 blendsql-0.0.14/blendsql/db/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-09 19:14:40.000000 blendsql-0.0.14/blendsql/db/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:14:44.725923 blendsql-0.0.14/blendsql/ingredients/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-09 19:14:40.000000 blendsql-0.0.14/blendsql/ingredients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:14:44.725923 blendsql-0.0.14/blendsql/ingredients/builtin/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-09 19:14:40.000000 blendsql-0.0.14/blendsql/ingredients/builtin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:14:44.725923 blendsql-0.0.14/blendsql/ingredients/builtin/dt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 19:14:40.000000 blendsql-0.0.14/blendsql/ingredients/builtin/dt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-09 19:14:40.000000 blendsql-0.0.14/blendsql/ingredients/builtin/dt/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-05-09 19:14:40.000000 blendsql-0.0.14/blendsql/ingredients/builtin/dt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:14:44.725923 blendsql-0.0.14/blendsql/ingredients/builtin/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 19:14:40.000000 blendsql-0.0.14/blendsql/ingredients/builtin/llm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:14:44.725923 blendsql-0.0.14/blendsql/ingredients/builtin/llm/join/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 19:14:40.000000 blendsql-0.0.14/blendsql/ingredients/builtin/llm/join/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-09 19:14:40.000000 blendsql-0.0.14/blendsql/ingredients/builtin/llm/join/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:14:44.729923 blendsql-0.0.14/blendsql/ingredients/builtin/llm/map/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-09 19:14:40.000000 blendsql-0.0.14/blendsql/ingredients/builtin/llm/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-05-09 19:14:40.000000 blendsql-0.0.14/blendsql/ingredients/builtin/llm/map/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:14:44.729923 blendsql-0.0.14/blendsql/ingredients/builtin/llm/qa/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 19:14:40.000000 blendsql-0.0.14/blendsql/ingredients/builtin/llm/qa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-09 19:14:40.000000 blendsql-0.0.14/blendsql/ingredients/builtin/llm/qa/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-09 19:14:40.000000 blendsql-0.0.14/blendsql/ingredients/builtin/llm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:14:44.729923 blendsql-0.0.14/blendsql/ingredients/builtin/llm/validate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 19:14:40.000000 blendsql-0.0.14/blendsql/ingredients/builtin/llm/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-09 19:14:40.000000 blendsql-0.0.14/blendsql/ingredients/builtin/llm/validate/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14304 2024-05-09 19:14:40.000000 blendsql-0.0.14/blendsql/ingredients/ingredient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:14:44.729923 blendsql-0.0.14/blendsql/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-09 19:14:40.000000 blendsql-0.0.14/blendsql/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-05-09 19:14:40.000000 blendsql-0.0.14/blendsql/models/_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:14:44.729923 blendsql-0.0.14/blendsql/models/local/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 19:14:40.000000 blendsql-0.0.14/blendsql/models/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-09 19:14:40.000000 blendsql-0.0.14/blendsql/models/local/_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:14:44.729923 blendsql-0.0.14/blendsql/models/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 19:14:40.000000 blendsql-0.0.14/blendsql/models/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-05-09 19:14:40.000000 blendsql-0.0.14/blendsql/models/remote/_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-09 19:14:40.000000 blendsql-0.0.14/blendsql/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:14:44.729923 blendsql-0.0.14/blendsql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    26516 2024-05-09 19:14:44.000000 blendsql-0.0.14/blendsql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-09 19:14:44.000000 blendsql-0.0.14/blendsql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 19:14:44.000000 blendsql-0.0.14/blendsql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-09 19:14:44.000000 blendsql-0.0.14/blendsql.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-09 19:14:44.000000 blendsql-0.0.14/blendsql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-09 19:14:44.000000 blendsql-0.0.14/blendsql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-09 19:14:40.000000 blendsql-0.0.14/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 19:14:44.733924 blendsql-0.0.14/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-09 19:14:40.000000 blendsql-0.0.14/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:14:44.729923 blendsql-0.0.14/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 19:14:40.000000 blendsql-0.0.14/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-09 19:14:40.000000 blendsql-0.0.14/tests/test_generic_blendsql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-05-09 19:14:40.000000 blendsql-0.0.14/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16381 2024-05-09 19:14:40.000000 blendsql-0.0.14/tests/test_multi_table_blendsql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14557 2024-05-09 19:14:40.000000 blendsql-0.0.14/tests/test_single_table_blendsql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-05-09 19:14:40.000000 blendsql-0.0.14/tests/utils.py
```

### Comparing `blendsql-0.0.13/LICENSE` & `blendsql-0.0.14/LICENSE`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.13/PKG-INFO` & `blendsql-0.0.14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: blendsql
-Version: 0.0.13
+Version: 0.0.14
 Summary: Orchestrate SQLite logic and LLM reasoning within a unified dialect.
 Home-page: https://github.com/parkervg/blendsql
 Author: Parker Glenn
 Author-email: parkervg5@gmail.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: guidance>=0.1.0
 Requires-Dist: pyparsing==3.1.1
 Requires-Dist: pandas>=2.0.0
 Requires-Dist: bottleneck>=1.3.6
 Requires-Dist: python-dotenv==1.0.1
+Requires-Dist: sqlglot==18.13.0
 Requires-Dist: platformdirs
-Requires-Dist: sqlglot
 Requires-Dist: pre-commit
 Requires-Dist: attrs
 Requires-Dist: tqdm
 Requires-Dist: dateparser
 Requires-Dist: colorama
 Requires-Dist: fiscalyear
 Requires-Dist: tabulate
@@ -61,18 +61,24 @@
 <b>Check out our <a href="https://parkervg.github.io/blendsql/" target="_blank">online documentation</a> for a more comprehensive overview.</b>
 
 <i>Results from the paper are available [here](https://github.com/parkervg/blendsql/tree/research-paper/research/paper-results)</i>
 </div>
 <br/>
 
 ## Intro
-BlendSQL is a *superset of SQLite* for problem decomposition and hybrid question-answering with LLMs. It builds off of the syntax of SQL to create an intermediate representation for tasks requiring complex reasoning over both structured and unstructured data.
+BlendSQL is a *superset of SQLite* for problem decomposition and hybrid question-answering with LLMs. 
+
+As a result, we can *Blend* together...
+
+- 🥤 ...operations over heterogeneous data sources (e.g. tables, text, images)
+- 🥤 ...the structured & interpretable reasoning of SQL with the generalizable reasoning of LLMs
 
 It can be viewed as an inversion of the typical text-to-SQL paradigm, where a user calls a LLM, and the LLM calls a SQL program.
-Here, the user is given the control to oversee all calls (LLM + SQL) within a unified query language.
+
+**Now, the user is given the control to oversee all calls (LLM + SQL) within a unified query language.**
 
 ![comparison](docs/img/comparison.jpg)
 
 For example, imagine we have the following tables.
 
 ### `w`
 | **date** | **rival**                 | **city**  | **venue**                   | **score** |
```

#### html2text {}

```diff
@@ -1,52 +1,53 @@
-Metadata-Version: 2.1 Name: blendsql Version: 0.0.13 Summary: Orchestrate
+Metadata-Version: 2.1 Name: blendsql Version: 0.0.14 Summary: Orchestrate
 SQLite logic and LLM reasoning within a unified dialect. Home-page: https://
 github.com/parkervg/blendsql Author: Parker Glenn Author-email:
 parkervg5@gmail.com License: Apache License 2.0 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: guidance>=0.1.0 Requires-Dist:
 pyparsing==3.1.1 Requires-Dist: pandas>=2.0.0 Requires-Dist: bottleneck>=1.3.6
-Requires-Dist: python-dotenv==1.0.1 Requires-Dist: platformdirs Requires-Dist:
-sqlglot Requires-Dist: pre-commit Requires-Dist: attrs Requires-Dist: tqdm
-Requires-Dist: dateparser Requires-Dist: colorama Requires-Dist: fiscalyear
-Requires-Dist: tabulate Requires-Dist: typeguard Provides-Extra: research
-Requires-Dist: datasets==2.16.1; extra == "research" Requires-Dist: nltk; extra
-== "research" Requires-Dist: wikiextractor; extra == "research" Requires-Dist:
-rouge_score; extra == "research" Requires-Dist: rapidfuzz; extra == "research"
-Requires-Dist: records; extra == "research" Requires-Dist: SQLAlchemy; extra ==
-"research" Requires-Dist: recognizers-text; extra == "research" Requires-Dist:
-recognizers-text-suite; extra == "research" Requires-Dist: emoji==1.7.0; extra
-== "research" Provides-Extra: test Requires-Dist: pytest; extra == "test"
-Requires-Dist: huggingface_hub; extra == "test" Provides-Extra: docs Requires-
-Dist: mkdocs-material; extra == "docs" Requires-Dist: mkdocstrings; extra ==
-"docs" Requires-Dist: mkdocs-section-index; extra == "docs" Requires-Dist:
-mkdocstrings-python; extra == "docs" Requires-Dist: mkdocs-jupyter; extra ==
-"docs"
+Requires-Dist: python-dotenv==1.0.1 Requires-Dist: sqlglot==18.13.0 Requires-
+Dist: platformdirs Requires-Dist: pre-commit Requires-Dist: attrs Requires-
+Dist: tqdm Requires-Dist: dateparser Requires-Dist: colorama Requires-Dist:
+fiscalyear Requires-Dist: tabulate Requires-Dist: typeguard Provides-Extra:
+research Requires-Dist: datasets==2.16.1; extra == "research" Requires-Dist:
+nltk; extra == "research" Requires-Dist: wikiextractor; extra == "research"
+Requires-Dist: rouge_score; extra == "research" Requires-Dist: rapidfuzz; extra
+== "research" Requires-Dist: records; extra == "research" Requires-Dist:
+SQLAlchemy; extra == "research" Requires-Dist: recognizers-text; extra ==
+"research" Requires-Dist: recognizers-text-suite; extra == "research" Requires-
+Dist: emoji==1.7.0; extra == "research" Provides-Extra: test Requires-Dist:
+pytest; extra == "test" Requires-Dist: huggingface_hub; extra == "test"
+Provides-Extra: docs Requires-Dist: mkdocs-material; extra == "docs" Requires-
+Dist: mkdocstrings; extra == "docs" Requires-Dist: mkdocs-section-index; extra
+== "docs" Requires-Dist: mkdocstrings-python; extra == "docs" Requires-Dist:
+mkdocs-jupyter; extra == "docs"
             _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_A_p_a_c_h_e___2_._0_-_b_l_u_e_._s_v_g_][https://
       img.shields.io/github/last-commit/parkervg/blendsql?color=green][https://
                                         img.shields.io/badge/PRs-Welcome-Green]
                                   [blendsql]
                                  SQL ð¤ LLMs
  CChheecckk oouutt oouurr _oo_nn_ll_ii_nn_ee_ _dd_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn ffoorr aa mmoorree ccoommpprreehheennssiivvee oovveerrvviieeww.. Results
 from the paper are available [here](https://github.com/parkervg/blendsql/tree/
                     research-paper/research/paper-results)
 
 ## Intro BlendSQL is a *superset of SQLite* for problem decomposition and
-hybrid question-answering with LLMs. It builds off of the syntax of SQL to
-create an intermediate representation for tasks requiring complex reasoning
-over both structured and unstructured data. It can be viewed as an inversion of
-the typical text-to-SQL paradigm, where a user calls a LLM, and the LLM calls a
-SQL program. Here, the user is given the control to oversee all calls (LLM +
-SQL) within a unified query language. ![comparison](docs/img/comparison.jpg)
-For example, imagine we have the following tables. ### `w` | **date** |
-**rival** | **city** | **venue** | **score** | |----------|--------------------
--------|-----------|-----------------------------|-----------| | 31 may | nsw
-waratahs | sydney | agricultural society ground | 11-0 | | 5 jun | northern
-districts | newcastle | sports ground | 29-0 | | 7 jun | nsw waratahs | sydney
-| agricultural society ground | 21-2 | | 11 jun | western districts | bathurst
-| bathurst ground | 11-0 | | 12 jun | wallaroo & university nsw | sydney |
+hybrid question-answering with LLMs. As a result, we can *Blend* together... -
+ð¥¤ ...operations over heterogeneous data sources (e.g. tables, text, images)
+- ð¥¤ ...the structured & interpretable reasoning of SQL with the
+generalizable reasoning of LLMs It can be viewed as an inversion of the typical
+text-to-SQL paradigm, where a user calls a LLM, and the LLM calls a SQL
+program. **Now, the user is given the control to oversee all calls (LLM + SQL)
+within a unified query language.** ![comparison](docs/img/comparison.jpg) For
+example, imagine we have the following tables. ### `w` | **date** | **rival** |
+**city** | **venue** | **score** | |----------|---------------------------|----
+-------|-----------------------------|-----------| | 31 may | nsw waratahs |
+sydney | agricultural society ground | 11-0 | | 5 jun | northern districts |
+newcastle | sports ground | 29-0 | | 7 jun | nsw waratahs | sydney |
+agricultural society ground | 21-2 | | 11 jun | western districts | bathurst |
+bathurst ground | 11-0 | | 12 jun | wallaroo & university nsw | sydney |
 cricket ground | 23-10 | ### `documents` | **title** | **content** | |---------
 -----------------------|---------------------------------------------------| |
 sydney | sydney ( /ËsÉªdni/ ( listen ) sid-nee ) is the ... | | new south
 wales waratahs | the new south wales waratahs ( /ËwÉrÉtÉËz/ or ... | |
 sydney showground (moore park) | the former sydney showground ( moore park )
 at... | | sydney cricket ground | the sydney cricket ground ( scg ) is a sports
 ... | | newcastle, new south wales | the newcastle ( /ËnuËkÉËsÉl/ new-kah-
```

### Comparing `blendsql-0.0.13/README.md` & `blendsql-0.0.14/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,24 @@
 <b>Check out our <a href="https://parkervg.github.io/blendsql/" target="_blank">online documentation</a> for a more comprehensive overview.</b>
 
 <i>Results from the paper are available [here](https://github.com/parkervg/blendsql/tree/research-paper/research/paper-results)</i>
 </div>
 <br/>
 
 ## Intro
-BlendSQL is a *superset of SQLite* for problem decomposition and hybrid question-answering with LLMs. It builds off of the syntax of SQL to create an intermediate representation for tasks requiring complex reasoning over both structured and unstructured data.
+BlendSQL is a *superset of SQLite* for problem decomposition and hybrid question-answering with LLMs. 
+
+As a result, we can *Blend* together...
+
+- 🥤 ...operations over heterogeneous data sources (e.g. tables, text, images)
+- 🥤 ...the structured & interpretable reasoning of SQL with the generalizable reasoning of LLMs
 
 It can be viewed as an inversion of the typical text-to-SQL paradigm, where a user calls a LLM, and the LLM calls a SQL program.
-Here, the user is given the control to oversee all calls (LLM + SQL) within a unified query language.
+
+**Now, the user is given the control to oversee all calls (LLM + SQL) within a unified query language.**
 
 ![comparison](docs/img/comparison.jpg)
 
 For example, imagine we have the following tables.
 
 ### `w`
 | **date** | **rival**                 | **city**  | **venue**                   | **score** |
```

#### html2text {}

```diff
@@ -4,27 +4,28 @@
                                   [blendsql]
                                  SQL ð¤ LLMs
  CChheecckk oouutt oouurr _oo_nn_ll_ii_nn_ee_ _dd_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn ffoorr aa mmoorree ccoommpprreehheennssiivvee oovveerrvviieeww.. Results
 from the paper are available [here](https://github.com/parkervg/blendsql/tree/
                     research-paper/research/paper-results)
 
 ## Intro BlendSQL is a *superset of SQLite* for problem decomposition and
-hybrid question-answering with LLMs. It builds off of the syntax of SQL to
-create an intermediate representation for tasks requiring complex reasoning
-over both structured and unstructured data. It can be viewed as an inversion of
-the typical text-to-SQL paradigm, where a user calls a LLM, and the LLM calls a
-SQL program. Here, the user is given the control to oversee all calls (LLM +
-SQL) within a unified query language. ![comparison](docs/img/comparison.jpg)
-For example, imagine we have the following tables. ### `w` | **date** |
-**rival** | **city** | **venue** | **score** | |----------|--------------------
--------|-----------|-----------------------------|-----------| | 31 may | nsw
-waratahs | sydney | agricultural society ground | 11-0 | | 5 jun | northern
-districts | newcastle | sports ground | 29-0 | | 7 jun | nsw waratahs | sydney
-| agricultural society ground | 21-2 | | 11 jun | western districts | bathurst
-| bathurst ground | 11-0 | | 12 jun | wallaroo & university nsw | sydney |
+hybrid question-answering with LLMs. As a result, we can *Blend* together... -
+ð¥¤ ...operations over heterogeneous data sources (e.g. tables, text, images)
+- ð¥¤ ...the structured & interpretable reasoning of SQL with the
+generalizable reasoning of LLMs It can be viewed as an inversion of the typical
+text-to-SQL paradigm, where a user calls a LLM, and the LLM calls a SQL
+program. **Now, the user is given the control to oversee all calls (LLM + SQL)
+within a unified query language.** ![comparison](docs/img/comparison.jpg) For
+example, imagine we have the following tables. ### `w` | **date** | **rival** |
+**city** | **venue** | **score** | |----------|---------------------------|----
+-------|-----------------------------|-----------| | 31 may | nsw waratahs |
+sydney | agricultural society ground | 11-0 | | 5 jun | northern districts |
+newcastle | sports ground | 29-0 | | 7 jun | nsw waratahs | sydney |
+agricultural society ground | 21-2 | | 11 jun | western districts | bathurst |
+bathurst ground | 11-0 | | 12 jun | wallaroo & university nsw | sydney |
 cricket ground | 23-10 | ### `documents` | **title** | **content** | |---------
 -----------------------|---------------------------------------------------| |
 sydney | sydney ( /ËsÉªdni/ ( listen ) sid-nee ) is the ... | | new south
 wales waratahs | the new south wales waratahs ( /ËwÉrÉtÉËz/ or ... | |
 sydney showground (moore park) | the former sydney showground ( moore park )
 at... | | sydney cricket ground | the sydney cricket ground ( scg ) is a sports
 ... | | newcastle, new south wales | the newcastle ( /ËnuËkÉËsÉl/ new-kah-
```

### Comparing `blendsql-0.0.13/blendsql/_constants.py` & `blendsql-0.0.14/blendsql/_constants.py`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.13/blendsql/_dialect.py` & `blendsql-0.0.14/blendsql/_dialect.py`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.13/blendsql/_grammar.py` & `blendsql-0.0.14/blendsql/_grammar.py`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.13/blendsql/_program.py` & `blendsql-0.0.14/blendsql/_program.py`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.13/blendsql/_smoothie.py` & `blendsql-0.0.14/blendsql/_smoothie.py`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.13/blendsql/_sqlglot.py` & `blendsql-0.0.14/blendsql/_sqlglot.py`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.13/blendsql/blend_cli.py` & `blendsql-0.0.14/blendsql/blend_cli.py`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.13/blendsql/blendsql.py` & `blendsql-0.0.14/blendsql/blendsql.py`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.13/blendsql/db/sqlite.py` & `blendsql-0.0.14/blendsql/db/sqlite.py`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.13/blendsql/ingredients/builtin/dt/main.py` & `blendsql-0.0.14/blendsql/ingredients/builtin/dt/main.py`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.13/blendsql/ingredients/builtin/dt/utils.py` & `blendsql-0.0.14/blendsql/ingredients/builtin/dt/utils.py`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.13/blendsql/ingredients/builtin/llm/join/main.py` & `blendsql-0.0.14/blendsql/ingredients/builtin/llm/join/main.py`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.13/blendsql/ingredients/builtin/llm/map/main.py` & `blendsql-0.0.14/blendsql/ingredients/builtin/llm/map/main.py`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.13/blendsql/ingredients/builtin/llm/qa/main.py` & `blendsql-0.0.14/blendsql/ingredients/builtin/llm/qa/main.py`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.13/blendsql/ingredients/builtin/llm/utils.py` & `blendsql-0.0.14/blendsql/ingredients/builtin/llm/utils.py`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.13/blendsql/ingredients/builtin/llm/validate/main.py` & `blendsql-0.0.14/blendsql/ingredients/builtin/llm/validate/main.py`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.13/blendsql/ingredients/ingredient.py` & `blendsql-0.0.14/blendsql/ingredients/ingredient.py`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.13/blendsql/models/_model.py` & `blendsql-0.0.14/blendsql/models/_model.py`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.13/blendsql/models/local/_transformers.py` & `blendsql-0.0.14/blendsql/models/local/_transformers.py`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.13/blendsql/models/remote/_openai.py` & `blendsql-0.0.14/blendsql/models/remote/_openai.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,15 +71,16 @@
             api_key=os.getenv("OPENAI_API_KEY"),
             azure_endpoint=os.getenv("OPENAI_API_BASE"),
             azure_deployment=os.getenv("API_VERSION"),
             echo=False,
         )
 
     def _setup(self, **kwargs) -> None:
-        return openai_setup()
+        openai_setup()
+        self.model = self._load_model()
 
 
 class OpenaiLLM(Model):
     """Class for OpenAI Model API.
 
     Args:
         model_name_or_path: Name of the OpenAI model to use
@@ -99,8 +100,9 @@
 
     def _load_model(self) -> Model:
         return OpenAI(
             self.model_name_or_path, api_key=os.getenv("OPENAI_API_KEY"), echo=False
         )
 
     def _setup(self, **kwargs) -> None:
-        return openai_setup()
+        openai_setup()
+        self.model = self._load_model()
```

### Comparing `blendsql-0.0.13/blendsql/utils.py` & `blendsql-0.0.14/blendsql/utils.py`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.13/blendsql.egg-info/PKG-INFO` & `blendsql-0.0.14/blendsql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: blendsql
-Version: 0.0.13
+Version: 0.0.14
 Summary: Orchestrate SQLite logic and LLM reasoning within a unified dialect.
 Home-page: https://github.com/parkervg/blendsql
 Author: Parker Glenn
 Author-email: parkervg5@gmail.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: guidance>=0.1.0
 Requires-Dist: pyparsing==3.1.1
 Requires-Dist: pandas>=2.0.0
 Requires-Dist: bottleneck>=1.3.6
 Requires-Dist: python-dotenv==1.0.1
+Requires-Dist: sqlglot==18.13.0
 Requires-Dist: platformdirs
-Requires-Dist: sqlglot
 Requires-Dist: pre-commit
 Requires-Dist: attrs
 Requires-Dist: tqdm
 Requires-Dist: dateparser
 Requires-Dist: colorama
 Requires-Dist: fiscalyear
 Requires-Dist: tabulate
@@ -61,18 +61,24 @@
 <b>Check out our <a href="https://parkervg.github.io/blendsql/" target="_blank">online documentation</a> for a more comprehensive overview.</b>
 
 <i>Results from the paper are available [here](https://github.com/parkervg/blendsql/tree/research-paper/research/paper-results)</i>
 </div>
 <br/>
 
 ## Intro
-BlendSQL is a *superset of SQLite* for problem decomposition and hybrid question-answering with LLMs. It builds off of the syntax of SQL to create an intermediate representation for tasks requiring complex reasoning over both structured and unstructured data.
+BlendSQL is a *superset of SQLite* for problem decomposition and hybrid question-answering with LLMs. 
+
+As a result, we can *Blend* together...
+
+- 🥤 ...operations over heterogeneous data sources (e.g. tables, text, images)
+- 🥤 ...the structured & interpretable reasoning of SQL with the generalizable reasoning of LLMs
 
 It can be viewed as an inversion of the typical text-to-SQL paradigm, where a user calls a LLM, and the LLM calls a SQL program.
-Here, the user is given the control to oversee all calls (LLM + SQL) within a unified query language.
+
+**Now, the user is given the control to oversee all calls (LLM + SQL) within a unified query language.**
 
 ![comparison](docs/img/comparison.jpg)
 
 For example, imagine we have the following tables.
 
 ### `w`
 | **date** | **rival**                 | **city**  | **venue**                   | **score** |
```

#### html2text {}

```diff
@@ -1,52 +1,53 @@
-Metadata-Version: 2.1 Name: blendsql Version: 0.0.13 Summary: Orchestrate
+Metadata-Version: 2.1 Name: blendsql Version: 0.0.14 Summary: Orchestrate
 SQLite logic and LLM reasoning within a unified dialect. Home-page: https://
 github.com/parkervg/blendsql Author: Parker Glenn Author-email:
 parkervg5@gmail.com License: Apache License 2.0 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: guidance>=0.1.0 Requires-Dist:
 pyparsing==3.1.1 Requires-Dist: pandas>=2.0.0 Requires-Dist: bottleneck>=1.3.6
-Requires-Dist: python-dotenv==1.0.1 Requires-Dist: platformdirs Requires-Dist:
-sqlglot Requires-Dist: pre-commit Requires-Dist: attrs Requires-Dist: tqdm
-Requires-Dist: dateparser Requires-Dist: colorama Requires-Dist: fiscalyear
-Requires-Dist: tabulate Requires-Dist: typeguard Provides-Extra: research
-Requires-Dist: datasets==2.16.1; extra == "research" Requires-Dist: nltk; extra
-== "research" Requires-Dist: wikiextractor; extra == "research" Requires-Dist:
-rouge_score; extra == "research" Requires-Dist: rapidfuzz; extra == "research"
-Requires-Dist: records; extra == "research" Requires-Dist: SQLAlchemy; extra ==
-"research" Requires-Dist: recognizers-text; extra == "research" Requires-Dist:
-recognizers-text-suite; extra == "research" Requires-Dist: emoji==1.7.0; extra
-== "research" Provides-Extra: test Requires-Dist: pytest; extra == "test"
-Requires-Dist: huggingface_hub; extra == "test" Provides-Extra: docs Requires-
-Dist: mkdocs-material; extra == "docs" Requires-Dist: mkdocstrings; extra ==
-"docs" Requires-Dist: mkdocs-section-index; extra == "docs" Requires-Dist:
-mkdocstrings-python; extra == "docs" Requires-Dist: mkdocs-jupyter; extra ==
-"docs"
+Requires-Dist: python-dotenv==1.0.1 Requires-Dist: sqlglot==18.13.0 Requires-
+Dist: platformdirs Requires-Dist: pre-commit Requires-Dist: attrs Requires-
+Dist: tqdm Requires-Dist: dateparser Requires-Dist: colorama Requires-Dist:
+fiscalyear Requires-Dist: tabulate Requires-Dist: typeguard Provides-Extra:
+research Requires-Dist: datasets==2.16.1; extra == "research" Requires-Dist:
+nltk; extra == "research" Requires-Dist: wikiextractor; extra == "research"
+Requires-Dist: rouge_score; extra == "research" Requires-Dist: rapidfuzz; extra
+== "research" Requires-Dist: records; extra == "research" Requires-Dist:
+SQLAlchemy; extra == "research" Requires-Dist: recognizers-text; extra ==
+"research" Requires-Dist: recognizers-text-suite; extra == "research" Requires-
+Dist: emoji==1.7.0; extra == "research" Provides-Extra: test Requires-Dist:
+pytest; extra == "test" Requires-Dist: huggingface_hub; extra == "test"
+Provides-Extra: docs Requires-Dist: mkdocs-material; extra == "docs" Requires-
+Dist: mkdocstrings; extra == "docs" Requires-Dist: mkdocs-section-index; extra
+== "docs" Requires-Dist: mkdocstrings-python; extra == "docs" Requires-Dist:
+mkdocs-jupyter; extra == "docs"
             _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_A_p_a_c_h_e___2_._0_-_b_l_u_e_._s_v_g_][https://
       img.shields.io/github/last-commit/parkervg/blendsql?color=green][https://
                                         img.shields.io/badge/PRs-Welcome-Green]
                                   [blendsql]
                                  SQL ð¤ LLMs
  CChheecckk oouutt oouurr _oo_nn_ll_ii_nn_ee_ _dd_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn ffoorr aa mmoorree ccoommpprreehheennssiivvee oovveerrvviieeww.. Results
 from the paper are available [here](https://github.com/parkervg/blendsql/tree/
                     research-paper/research/paper-results)
 
 ## Intro BlendSQL is a *superset of SQLite* for problem decomposition and
-hybrid question-answering with LLMs. It builds off of the syntax of SQL to
-create an intermediate representation for tasks requiring complex reasoning
-over both structured and unstructured data. It can be viewed as an inversion of
-the typical text-to-SQL paradigm, where a user calls a LLM, and the LLM calls a
-SQL program. Here, the user is given the control to oversee all calls (LLM +
-SQL) within a unified query language. ![comparison](docs/img/comparison.jpg)
-For example, imagine we have the following tables. ### `w` | **date** |
-**rival** | **city** | **venue** | **score** | |----------|--------------------
--------|-----------|-----------------------------|-----------| | 31 may | nsw
-waratahs | sydney | agricultural society ground | 11-0 | | 5 jun | northern
-districts | newcastle | sports ground | 29-0 | | 7 jun | nsw waratahs | sydney
-| agricultural society ground | 21-2 | | 11 jun | western districts | bathurst
-| bathurst ground | 11-0 | | 12 jun | wallaroo & university nsw | sydney |
+hybrid question-answering with LLMs. As a result, we can *Blend* together... -
+ð¥¤ ...operations over heterogeneous data sources (e.g. tables, text, images)
+- ð¥¤ ...the structured & interpretable reasoning of SQL with the
+generalizable reasoning of LLMs It can be viewed as an inversion of the typical
+text-to-SQL paradigm, where a user calls a LLM, and the LLM calls a SQL
+program. **Now, the user is given the control to oversee all calls (LLM + SQL)
+within a unified query language.** ![comparison](docs/img/comparison.jpg) For
+example, imagine we have the following tables. ### `w` | **date** | **rival** |
+**city** | **venue** | **score** | |----------|---------------------------|----
+-------|-----------------------------|-----------| | 31 may | nsw waratahs |
+sydney | agricultural society ground | 11-0 | | 5 jun | northern districts |
+newcastle | sports ground | 29-0 | | 7 jun | nsw waratahs | sydney |
+agricultural society ground | 21-2 | | 11 jun | western districts | bathurst |
+bathurst ground | 11-0 | | 12 jun | wallaroo & university nsw | sydney |
 cricket ground | 23-10 | ### `documents` | **title** | **content** | |---------
 -----------------------|---------------------------------------------------| |
 sydney | sydney ( /ËsÉªdni/ ( listen ) sid-nee ) is the ... | | new south
 wales waratahs | the new south wales waratahs ( /ËwÉrÉtÉËz/ or ... | |
 sydney showground (moore park) | the former sydney showground ( moore park )
 at... | | sydney cricket ground | the sydney cricket ground ( scg ) is a sports
 ... | | newcastle, new south wales | the newcastle ( /ËnuËkÉËsÉl/ new-kah-
```

### Comparing `blendsql-0.0.13/blendsql.egg-info/SOURCES.txt` & `blendsql-0.0.14/blendsql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.13/pyproject.toml` & `blendsql-0.0.14/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.13/setup.py` & `blendsql-0.0.14/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,16 +35,16 @@
     packages=find_packages(exclude=["examples", "research", "img"]),
     install_requires=[
         "guidance>=0.1.0",
         "pyparsing==3.1.1",
         "pandas>=2.0.0",
         "bottleneck>=1.3.6",
         "python-dotenv==1.0.1",
+        "sqlglot==18.13.0",
         "platformdirs",
-        "sqlglot",
         "pre-commit",
         "attrs",
         "tqdm",
         "dateparser",
         "colorama",
         "fiscalyear",
         "tabulate",
```

### Comparing `blendsql-0.0.13/tests/test_generic_blendsql.py` & `blendsql-0.0.14/tests/test_generic_blendsql.py`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.13/tests/test_model.py` & `blendsql-0.0.14/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.13/tests/test_multi_table_blendsql.py` & `blendsql-0.0.14/tests/test_multi_table_blendsql.py`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.13/tests/test_single_table_blendsql.py` & `blendsql-0.0.14/tests/test_single_table_blendsql.py`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.13/tests/utils.py` & `blendsql-0.0.14/tests/utils.py`

 * *Files identical despite different names*

