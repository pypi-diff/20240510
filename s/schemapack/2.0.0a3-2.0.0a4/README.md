# Comparing `tmp/schemapack-2.0.0a3.tar.gz` & `tmp/schemapack-2.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schemapack-2.0.0a3.tar", last modified: Thu Mar 21 10:06:00 2024, max compression
+gzip compressed data, was "schemapack-2.0.0a4.tar", last modified: Fri May 10 08:57:10 2024, max compression
```

## Comparing `schemapack-2.0.0a3.tar` & `schemapack-2.0.0a4.tar`

### file list

```diff
@@ -1,65 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:06:00.253058 schemapack-2.0.0a3/
--rw-r--r--   0 runner    (1001) docker     (127)    11452 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-03-21 10:06:00.253058 schemapack-2.0.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 10:06:00.253058 schemapack-2.0.0a3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:06:00.241058 schemapack-2.0.0a3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:06:00.245058 schemapack-2.0.0a3/src/schemapack/
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/src/schemapack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/src/schemapack/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:06:00.249058 schemapack-2.0.0a3/src/schemapack/_internals/
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/src/schemapack/_internals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/src/schemapack/_internals/dump.py
--rw-r--r--   0 runner    (1001) docker     (127)     7135 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/src/schemapack/_internals/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8300 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/src/schemapack/_internals/isolate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/src/schemapack/_internals/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/src/schemapack/_internals/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/src/schemapack/_internals/normalize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:06:00.249058 schemapack-2.0.0a3/src/schemapack/_internals/spec/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/src/schemapack/_internals/spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/src/schemapack/_internals/spec/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/src/schemapack/_internals/spec/datapack.py
--rw-r--r--   0 runner    (1001) docker     (127)    18783 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/src/schemapack/_internals/spec/schemapack.py
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/src/schemapack/_internals/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:06:00.249058 schemapack-2.0.0a3/src/schemapack/_internals/validation/
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/src/schemapack/_internals/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8188 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/src/schemapack/_internals/validation/_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/src/schemapack/_internals/validation/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/src/schemapack/_internals/validation/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:06:00.253058 schemapack-2.0.0a3/src/schemapack/_internals/validation/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/src/schemapack/_internals/validation/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/src/schemapack/_internals/validation/plugins/content_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/src/schemapack/_internals/validation/plugins/expected_root.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/src/schemapack/_internals/validation/plugins/missing_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/src/schemapack/_internals/validation/plugins/missing_origin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/src/schemapack/_internals/validation/plugins/missing_relations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/src/schemapack/_internals/validation/plugins/missing_target.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/src/schemapack/_internals/validation/plugins/multiple_target.py
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/src/schemapack/_internals/validation/plugins/one_to_many_overlap.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/src/schemapack/_internals/validation/plugins/target_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/src/schemapack/_internals/validation/plugins/unexpected_root.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/src/schemapack/_internals/validation/plugins/unknown_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/src/schemapack/_internals/validation/plugins/unknown_relations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/src/schemapack/_internals/validation/plugins/unkown_root_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/src/schemapack/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/src/schemapack/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:06:00.253058 schemapack-2.0.0a3/src/schemapack/spec/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/src/schemapack/spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/src/schemapack/spec/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/src/schemapack/spec/datapack.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/src/schemapack/spec/schemapack.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/src/schemapack/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:06:00.253058 schemapack-2.0.0a3/src/schemapack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-03-21 10:06:00.000000 schemapack-2.0.0a3/src/schemapack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-03-21 10:06:00.000000 schemapack-2.0.0a3/src/schemapack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 10:06:00.000000 schemapack-2.0.0a3/src/schemapack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-21 10:06:00.000000 schemapack-2.0.0a3/src/schemapack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-21 10:06:00.000000 schemapack-2.0.0a3/src/schemapack.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:06:00.253058 schemapack-2.0.0a3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/tests/test_denormalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/tests/test_dump.py
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/tests/test_isolate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/tests/test_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-03-21 10:05:54.000000 schemapack-2.0.0a3/tests/test_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:57:10.721961 schemapack-2.0.0a4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11452 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-05-10 08:57:10.721961 schemapack-2.0.0a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 08:57:10.721961 schemapack-2.0.0a4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:57:10.709962 schemapack-2.0.0a4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:57:10.709962 schemapack-2.0.0a4/src/schemapack/
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:57:10.713961 schemapack-2.0.0a4/src/schemapack/_internals/
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/_internals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:57:10.713961 schemapack-2.0.0a4/src/schemapack/_internals/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/_internals/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/_internals/cli/exception_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/_internals/cli/exit_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8496 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/_internals/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/_internals/cli/printing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/_internals/dump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/_internals/erd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8574 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/_internals/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10194 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/_internals/isolate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/_internals/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/_internals/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/_internals/normalize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:57:10.717961 schemapack-2.0.0a4/src/schemapack/_internals/spec/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/_internals/spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/_internals/spec/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/_internals/spec/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6642 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/_internals/spec/datapack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18418 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/_internals/spec/schemapack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/_internals/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:57:10.717961 schemapack-2.0.0a4/src/schemapack/_internals/validation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/_internals/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8188 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/_internals/validation/_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/_internals/validation/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/_internals/validation/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:57:10.717961 schemapack-2.0.0a4/src/schemapack/_internals/validation/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/_internals/validation/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/_internals/validation/plugins/content_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/_internals/validation/plugins/expected_root.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/_internals/validation/plugins/missing_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/_internals/validation/plugins/missing_origin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/_internals/validation/plugins/missing_relations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/_internals/validation/plugins/missing_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/_internals/validation/plugins/multiple_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/_internals/validation/plugins/one_to_many_overlap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/_internals/validation/plugins/target_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/_internals/validation/plugins/unexpected_root.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/_internals/validation/plugins/unknown_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/_internals/validation/plugins/unknown_relations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/_internals/validation/plugins/unkown_root_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:57:10.721961 schemapack-2.0.0a4/src/schemapack/spec/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/spec/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/spec/datapack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/spec/schemapack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/src/schemapack/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:57:10.721961 schemapack-2.0.0a4/src/schemapack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-05-10 08:57:10.000000 schemapack-2.0.0a4/src/schemapack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-10 08:57:10.000000 schemapack-2.0.0a4/src/schemapack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 08:57:10.000000 schemapack-2.0.0a4/src/schemapack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-10 08:57:10.000000 schemapack-2.0.0a4/src/schemapack.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-10 08:57:10.000000 schemapack-2.0.0a4/src/schemapack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-10 08:57:10.000000 schemapack-2.0.0a4/src/schemapack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:57:10.721961 schemapack-2.0.0a4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    12231 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/tests/test_denormalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/tests/test_dump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/tests/test_export_mermaid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5793 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/tests/test_isolate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/tests/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-10 08:57:06.000000 schemapack-2.0.0a4/tests/test_spec.py
```

### Comparing `schemapack-2.0.0a3/LICENSE` & `schemapack-2.0.0a4/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+   Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
    for the German Human Genome-Phenome Archive (GHGA)
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `schemapack-2.0.0a3/PKG-INFO` & `schemapack-2.0.0a4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: schemapack
-Version: 2.0.0a3
+Version: 2.0.0a4
 Summary: Make your JSON Schemas sociable and create linked data model.
 Author-email: "German Human Genome Phenome Archive (GHGA)" <contact@ghga.de>
 License: Apache 2.0
 Project-URL: Repository, https://github.com/ghga-de/schemapack
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic<3,>=2
 Requires-Dist: pydantic_settings<3,>=2
 Requires-Dist: ruamel.yaml~=0.18.6
 Requires-Dist: jsonschema<5,>=4.19.2
-Requires-Dist: immutabledict<4,>=3.0.0
+Requires-Dist: arcticfreeze~=0.1.1
+Requires-Dist: rich<14,>13
 
 ![tests](https://github.com/ghga-de/schemapack/actions/workflows/tests.yaml/badge.svg)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/schemapack.svg)](https://pypi.python.org/pypi/schemapack/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/schemapack.svg)](https://pypi.python.org/pypi/schemapack/)
 [![Coverage Status](https://coveralls.io/repos/github/ghga-de/schemapack/badge.svg?branch=main)](https://coveralls.io/github/ghga-de/schemapack?branch=main)
 
 # schemapack
```

### Comparing `schemapack-2.0.0a3/README.md` & `schemapack-2.0.0a4/README.md`

 * *Files identical despite different names*

### Comparing `schemapack-2.0.0a3/pyproject.toml` & `schemapack-2.0.0a4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [build-system]
 requires = [
-    "setuptools>=67.7.2",
+    "setuptools>=69",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 readme = "README.md"
 authors = [
     { name = "German Human Genome Phenome Archive (GHGA)", email = "contact@ghga.de" },
@@ -12,36 +12,41 @@
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 1 - Planning",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: Apache Software License",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Software Development :: Libraries",
     "Intended Audience :: Developers",
 ]
 name = "schemapack"
-version = "2.0.0-alpha.3"
+version = "2.0.0-alpha.4"
 description = "Make your JSON Schemas sociable and create linked data model."
 dependencies = [
     "pydantic >=2, <3",
     "pydantic_settings >=2, <3",
-    "ruamel.yaml ~= 0.18.6",
+    "ruamel.yaml ~=0.18.6",
     "jsonschema >=4.19.2, <5",
-    "immutabledict >=3.0.0, <4",
+    "arcticfreeze ~=0.1.1",
+    "rich >13, <14",
 ]
 
 [project.license]
 text = "Apache 2.0"
 
 [project.urls]
 Repository = "https://github.com/ghga-de/schemapack"
 
+[project.scripts]
+schemapack = "schemapack.__main__:cli"
+
 [tool.setuptools.packages.find]
 where = [
     "src",
 ]
 
 [tool.ruff]
 exclude = [
@@ -63,16 +68,17 @@
 [tool.ruff.lint]
 fixable = [
     "UP",
     "I",
     "D",
 ]
 ignore = [
-    "E",
-    "W",
+    "E111",
+    "E114",
+    "E116",
     "PLW",
     "RUF001",
     "RUF010",
     "RUF012",
     "N818",
     "B008",
     "PLR2004",
@@ -137,15 +143,15 @@
 ]
 warn_redundant_casts = true
 warn_unused_ignores = true
 check_untyped_defs = true
 no_site_packages = false
 
 [tool.pytest.ini_options]
-minversion = "7.1"
+minversion = "8.0"
 asyncio_mode = "strict"
 
 [tool.coverage.paths]
 source = [
     "src",
     "/workspace/src",
     "**/lib/python*/site-packages",
```

### Comparing `schemapack-2.0.0a3/src/schemapack/__init__.py` & `schemapack-2.0.0a4/src/schemapack/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -15,27 +15,31 @@
 
 """A specification (plus tooling) for describing linked data models based on JSON
 schema.
 """
 
 from importlib.metadata import version
 
-from ._internals.dump import dump_schemapack
+from ._internals.dump import dump_schemapack, dumps_datapack, dumps_schemapack
+from ._internals.erd import export_mermaid
 from ._internals.isolate import isolate, isolate_class, isolate_resource
 from ._internals.load import load_datapack, load_schemapack
 from ._internals.main import load_and_validate
 from ._internals.normalize import denormalize
 from ._internals.validation import SchemaPackValidator
 
 __all__ = [
+    "export_mermaid",
     "load_and_validate",
     "load_datapack",
     "load_schemapack",
     "isolate",
     "isolate_class",
     "isolate_resource",
     "denormalize",
     "SchemaPackValidator",
+    "dumps_datapack",
     "dump_schemapack",
+    "dumps_schemapack",
 ]
 
 __version__ = version(__package__)
```

### Comparing `schemapack-2.0.0a3/src/schemapack/__main__.py` & `schemapack-2.0.0a4/src/schemapack/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -10,7 +10,12 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Entrypoint of the package"""
+
+from schemapack._internals.cli import cli
+
+if __name__ == "__main__":
+    cli()
```

### Comparing `schemapack-2.0.0a3/src/schemapack/_internals/__init__.py` & `schemapack-2.0.0a4/src/schemapack/_internals/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `schemapack-2.0.0a3/src/schemapack/_internals/dump.py` & `schemapack-2.0.0a4/src/schemapack/_internals/dump.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -16,21 +16,21 @@
 
 """Logic for dumping schemapacks."""
 
 import json
 from pathlib import Path
 from typing import Any
 
-import ruamel.yaml
-
+from schemapack._internals.spec.datapack import DataPack
 from schemapack._internals.spec.schemapack import SchemaPack
-
-yaml = ruamel.yaml.YAML(typ="safe")
-yaml.indent(mapping=2, sequence=4, offset=2)
-yaml.default_flow_style = False
+from schemapack._internals.utils import (
+    dumps_model,
+    model_to_serializable_dict,
+    write_dict,
+)
 
 
 def get_content_schema_path(*, class_name: str, content_schema_dir: Path) -> Path:
     """Get the path to a content schema file in the provided directory for a class with
     the provided name.
     """
     return content_schema_dir / f"{class_name}.schema.json"
@@ -55,42 +55,64 @@
         }
         for class_name, class_ in schemapack_dict["classes"].items()
     }
 
     return {**schemapack_dict, "classes": modified_classes}
 
 
-def write_schemapack_dict(
-    schemapack_dict: dict, *, path: Path, yaml_format: bool
-) -> None:
-    """Writes the provided schemapack dictionary to a file at the provided path."""
-    if yaml_format:
-        with open(path, "w", encoding="utf-8") as file:
-            yaml.dump(schemapack_dict, file)
-    else:
-        with open(path, "w", encoding="utf-8") as file:
-            json.dump(schemapack_dict, file, indent=2)
-
-
 def write_content_schemas(
     *, schemapack: SchemaPack, content_schema_dir: Path, relative_to: Path
 ) -> None:
     """Writes the content schemas of individual classes defined in the provided
     schemapack as separate files to the provided directory `content_schema_dir`
     which is relative to `relative_to`.
     """
     abs_content_schema_dir = relative_to / content_schema_dir
     abs_content_schema_dir.mkdir(parents=True, exist_ok=True)
 
     for class_name, class_ in schemapack.classes.items():
         content_schema_path = get_content_schema_path(
             class_name=class_name, content_schema_dir=abs_content_schema_dir
         )
+        class_dict = json.loads(class_.model_dump_json())
         with open(content_schema_path, "w", encoding="utf-8") as file:
-            file.write(class_.content.json_schema)
+            json.dump(class_dict["content"], file)
+
+
+def dumps_schemapack(
+    schemapack: SchemaPack,
+    *,
+    yaml_format: bool = True,
+) -> str:
+    """Dumps a condensed version of the provided schemapack as a JSON or YAML-formatted
+    string.
+
+    Args:
+        schemapack:
+            The schemapack to dump.
+        yaml_format:
+            Whether to dump as YAML (`True`) or JSON (`False`).
+    """
+    return dumps_model(schemapack, yaml_format=yaml_format)
+
+
+def dumps_datapack(
+    datapack: DataPack,
+    *,
+    yaml_format: bool = True,
+) -> str:
+    """Dumps the provided datapack as a JSON or YAML-formatted string.
+
+    Args:
+        datapack:
+            The datapack to dump.
+        yaml_format:
+            Whether to dump as YAML (`True`) or JSON (`False`).
+    """
+    return dumps_model(datapack, yaml_format=yaml_format)
 
 
 def dump_schemapack(
     schemapack: SchemaPack,
     *,
     path: Path,
     condensed: bool = True,
@@ -122,20 +144,20 @@
         FileNotFoundError:
             If the parent directory of the provided `path` does not exist.
     """
     parent_dir = path.parent
     if not parent_dir.exists():
         raise FileNotFoundError(f"The parent directory of '{path}' does not exist.")
 
-    schemapack_dict = json.loads(schemapack.model_dump_json(exclude_defaults=True))
+    schemapack_dict = model_to_serializable_dict(schemapack)
 
     if not condensed:
         schemapack_dict = set_content_schema_paths(
             schemapack_dict=schemapack_dict, content_schema_dir=content_schema_dir
         )
         write_content_schemas(
             schemapack=schemapack,
             content_schema_dir=content_schema_dir,
             relative_to=parent_dir,
         )
 
-    write_schemapack_dict(schemapack_dict, path=path, yaml_format=yaml_format)
+    write_dict(schemapack_dict, path=path, yaml_format=yaml_format)
```

### Comparing `schemapack-2.0.0a3/src/schemapack/_internals/exceptions.py` & `schemapack-2.0.0a4/src/schemapack/_internals/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -14,19 +14,27 @@
 # limitations under the License.
 #
 
 """Collection of package-specific exceptions"""
 
 from abc import ABC
 from dataclasses import dataclass
+from enum import Enum
 from typing import Optional
 
 import pydantic_core
 
 
+class SpecType(str, Enum):
+    """An enumeration of the types of specs."""
+
+    SCHEMAPACK = "schemapack"
+    DATAPACK = "datapack"
+
+
 class BaseError(ABC, Exception):
     """Base class for all schemapack errors."""
 
 
 class ParsingError(BaseError, ValueError):
     """Raised when parsing JSON or YAML data fails."""
 
@@ -132,15 +140,15 @@
     """Translate a ValidationErrorRecords into a human-readable message
     to be displayed to the user on the terminal.
     """
     if record.subject_class:
         if record.subject_resource:
             context = f"resource '{record.subject_class}.{record.subject_resource}'"
         else:
-            context = "class '{record.subject_class}'"
+            context = f"class '{record.subject_class}'"
     else:
         context = "global datapack"
 
     return (
         f"Error in {context}:"
         + f"\n\tType: {record.type}"
         + f"\n\tMessage: {record.message}"
@@ -200,7 +208,45 @@
         self.message = message
 
 
 class CircularRelationError(BaseError, ValueError):
     """Raised when a circular relation between resources is detected, but the requested
     operation cannot be performed on datapacks with circular relations.
     """
+
+
+class ClassNotFoundError(BaseError, KeyError):
+    """Raised when a class was not found in a schemapack or datapack."""
+
+    def __init__(self, *, class_name: str, spec_type: SpecType):
+        """Initiate a ClassNotFoundError.
+
+        Args:
+            class_name:
+                The name of the class that was not found.
+            spec_type:
+                The type of spec that the class was not found in.
+        """
+        message = f"Class '{class_name}' not found in the provided {spec_type.value}."
+        super().__init__(message)
+        self.class_name = class_name
+
+
+class ResourceNotFoundError(BaseError, KeyError):
+    """Raised when a resource was not found in a datapack."""
+
+    def __init__(self, *, class_name: str, resource_id: str):
+        """Initiate a ResourceNotFoundError.
+
+        Args:
+            class_name:
+                The name of the class of the resource that was not found.
+            resource_id:
+                The ID of the resource that was not found.
+        """
+        message = (
+            f"Resource of class '{class_name}' with id '{resource_id}' not found in"
+            + " the provided datapack."
+        )
+        super().__init__(message)
+        self.class_name = class_name
+        self.resource_id = resource_id
```

### Comparing `schemapack-2.0.0a3/src/schemapack/_internals/isolate.py` & `schemapack-2.0.0a4/src/schemapack/_internals/isolate.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -19,21 +19,26 @@
 Warning: This is an internal part of the library and might change without notice.
 """
 
 from collections import defaultdict
 from collections.abc import Mapping
 from typing import Optional
 
+from schemapack._internals.exceptions import (
+    ClassNotFoundError,
+    ResourceNotFoundError,
+    SpecType,
+)
 from schemapack.exceptions import ValidationAssumptionError
 from schemapack.spec.custom_types import ClassName, ResourceId
 from schemapack.spec.datapack import DataPack, Resource
 from schemapack.spec.schemapack import SchemaPack
 
 
-def identify_dependencies(
+def identify_dependencies(  # noqa: C901, PLR0912
     *,
     datapack: DataPack,
     class_name: ClassName,
     resource_id: ResourceId,
     schemapack: SchemaPack,
     include_target: bool = False,
     _resource_blacklist: Optional[Mapping[ClassName, set[ResourceId]]] = None,
@@ -59,23 +64,33 @@
             not appear in the result. This is only used internally for recursion.
 
     Returns:
         A mapping containing resource ids (values) of dependencies by class names
         (keys).
 
     Raises:
-        KeyError:
-            If the resource_class or the resource_id does not exist in the schemapack
-            or datapack.
+        schemapack.Exceptions.ClassNotFoundError:
+            If the class_name does not exist in the schemapack or datapack.
+        schemapack.Exceptions.ResourceNotFoundError:
+            If the resource_id does not exist in the schemapack or datapack.
         schemapack.Exceptions.ValidationAssumptionError:
             If it became apparent that the datapack was not already validated against
             the schemapack.
     """
-    target_resource = datapack.resources[class_name][resource_id]
-    target_class_definition = schemapack.classes[class_name]
+    target_class_resources = datapack.resources.get(class_name)
+    if target_class_resources is None:
+        raise ClassNotFoundError(class_name=class_name, spec_type=SpecType.DATAPACK)
+
+    target_resource = target_class_resources.get(resource_id)
+    if target_resource is None:
+        raise ResourceNotFoundError(class_name=class_name, resource_id=resource_id)
+
+    target_class_definition = schemapack.classes.get(class_name)
+    if target_class_definition is None:
+        raise ClassNotFoundError(class_name=class_name, spec_type=SpecType.SCHEMAPACK)
 
     # Define a blacklist of resources to avoid getting lost in infinity loop for
     # circular dependencies:
     resource_blacklist: dict[ClassName, set[ResourceId]] = defaultdict(set)
     resource_blacklist[class_name].add(resource_id)
     if _resource_blacklist:
         for class_name, resource_ids in _resource_blacklist.items():
@@ -139,15 +154,14 @@
             datapack. If set to `True`, these resources will be ignored. If set to
             `False` (default), a KeyError will be raised.
 
     Raises:
         KeyError:
             If a resource from the resource_map is not in the datapack and
             ignore_non_existing is set to `False`.
-
     """
     resources: dict[ClassName, dict[ResourceId, Resource]] = defaultdict(dict)
 
     for class_name, resource_ids in resource_map.items():
         try:
             existing_resources = datapack.resources[class_name]
         except KeyError as error:
@@ -178,29 +192,47 @@
     """Isolate a resource from a non-rooted datapack to created a rooted datapack. I.e.
     the resulting datapack will only contain resources referenced by the root resource
     as well as the root resource itself.
 
     Please note:
         The returned rooted datapack will not be compatible anymore with the original
         non-rooted schemapack.
+
+    Raises:
+        schemapack.Exceptions.ClassNotFoundError:
+            If the class_name does not exist in the schemapack or datapack.
+        schemapack.Exceptions.ResourceNotFoundError:
+            If the resource_id does not exist in the schemapack or datapack.
+        schemapack.Exceptions.ValidationAssumptionError:
+            If it became apparent that the datapack was not already validated against
+            the schemapack.
     """
     dependency_map = identify_dependencies(
         datapack=datapack,
         class_name=class_name,
         resource_id=resource_id,
         schemapack=schemapack,
         include_target=True,
     )
     rooted_datapack = downscope_datapack(datapack=datapack, resource_map=dependency_map)
-    rooted_datapack.rootResource = resource_id
+    rooted_datapack = rooted_datapack.model_copy(update={"rootResource": resource_id})
     return rooted_datapack
 
 
 def isolate_class(*, class_name: ClassName, schemapack: SchemaPack) -> SchemaPack:
-    """Return a copy of the provided schemapack that is rooted to the specified class."""
+    """Return a copy of the provided schemapack that is rooted to the specified class.
+
+
+    Raises:
+        schemapack.Exceptions.ClassNotFoundError:
+            If the class_name does not exist in the schemapack or datapack.
+    """
+    if class_name not in schemapack.classes:
+        raise ClassNotFoundError(class_name=class_name, spec_type=SpecType.SCHEMAPACK)
+
     return schemapack.model_copy(update={"rootClass": class_name})
 
 
 def isolate(
     *,
     class_name: ClassName,
     resource_id: ResourceId,
@@ -209,14 +241,23 @@
 ) -> tuple[SchemaPack, DataPack]:
     """Create copies of the provided schemapacks and datapacks that are rooted towards
     the specified class and resource. I.e. the resulting datapack will only contain
     resources referenced by the root resource as well as the root resource itself.
 
     Returns:
         A tuple containing both the rooted schemapack and the rooted datapack.
+
+    Raises:
+        schemapack.Exceptions.ClassNotFoundError:
+            If the class_name does not exist in the schemapack or datapack.
+        schemapack.Exceptions.ResourceNotFoundError:
+            If the resource_id does not exist in the schemapack or datapack.
+        schemapack.Exceptions.ValidationAssumptionError:
+            If it became apparent that the datapack was not already validated against
+            the schemapack.
     """
     rooted_schemapack = isolate_class(class_name=class_name, schemapack=schemapack)
     rooted_datapack = isolate_resource(
         datapack=datapack,
         class_name=class_name,
         resource_id=resource_id,
         schemapack=schemapack,
```

### Comparing `schemapack-2.0.0a3/src/schemapack/_internals/load.py` & `schemapack-2.0.0a4/src/schemapack/_internals/load.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `schemapack-2.0.0a3/src/schemapack/_internals/main.py` & `schemapack-2.0.0a4/src/schemapack/_internals/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `schemapack-2.0.0a3/src/schemapack/_internals/normalize.py` & `schemapack-2.0.0a4/src/schemapack/_internals/normalize.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -108,15 +108,15 @@
         try:
             relation_definition = root_class_definition.relations[relation_name]
         except KeyError as error:
             raise ValidationAssumptionError(context="relation resolution") from error
 
         target_class_name = relation_definition.targetClass
 
-        if isinstance(target_ids, set):
+        if isinstance(target_ids, frozenset):
             denormalized_object[relation_name] = []
 
             # make the output predictable:
             sorted_target_ids = sorted(target_ids)
 
             for target_id in sorted_target_ids:
                 if (
```

### Comparing `schemapack-2.0.0a3/src/schemapack/_internals/spec/__init__.py` & `schemapack-2.0.0a4/src/schemapack/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-#
 
-"""Models representing the schemapack and datapack specs."""
+"""Details on the command line interface."""
+
+from schemapack._internals.cli import exit_codes
+
+__all__ = ["exit_codes"]
```

### Comparing `schemapack-2.0.0a3/src/schemapack/_internals/spec/datapack.py` & `schemapack-2.0.0a4/src/schemapack/_internals/spec/datapack.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -20,30 +20,36 @@
 """
 
 import typing
 from collections import Counter
 from collections.abc import Iterable
 from typing import Annotated, Any, Literal, Optional, Union
 
-from pydantic import BaseModel, BeforeValidator, ConfigDict, Field, WrapSerializer
+from arcticfreeze import FrozenDict, freeze
+from pydantic import BeforeValidator, Field, WrapSerializer
 from pydantic_core import PydanticCustomError
 from typing_extensions import TypeAlias
 
-from ...spec.custom_types import ClassName, RelationPropertyName, ResourceId
+from schemapack._internals.spec.base import _FrozenNoExtraBaseModel
+from schemapack._internals.spec.custom_types import (
+    ClassName,
+    RelationPropertyName,
+    ResourceId,
+)
 
 SupportedDataPackVersions = Literal["0.3.0"]
 SUPPORTED_DATA_PACK_VERSIONS = typing.get_args(SupportedDataPackVersions)
 
 
 def validate_duplicate_target_ids(iterable: Iterable) -> Any:
     """Checks that the given iterable of target IDs does not contain duplicates. If it
     does, a PydanticCustomError with name "DuplicateTargetIdError" is raised. Otherwise,
     the given iterable is returned.
     """
-    if isinstance(iterable, set):
+    if isinstance(iterable, frozenset):
         return iterable
 
     try:
         target_id_list = list(iterable)
     except TypeError as error:
         raise PydanticCustomError(
             "TargetIdsParsingError",
@@ -61,45 +67,45 @@
             {"duplicates": duplicates},
         )
 
     return iterable
 
 
 ResourceIdSet: TypeAlias = Annotated[
-    set[str],
+    frozenset[str],
     # Upon serialization, assert that the provided sequence does not contain duplicates:
     BeforeValidator(validate_duplicate_target_ids),
     # Upon serialization, produce predictablily sorted lists:
     WrapSerializer(lambda v, next_: sorted(next_(v))),
 ]
 
-
-class _NoExtraBaseModel(BaseModel):
-    """A BaseModel that does not allow any extra fields."""
-
-    model_config = ConfigDict(use_enum_values=True, extra="forbid")
+ContentPropertyValue: TypeAlias = Annotated[
+    Any,
+    # the value of a content property is deeply frozen:
+    BeforeValidator(lambda obj: freeze(obj, by_superclass=True)),
+]
 
 
-class Resource(_NoExtraBaseModel):
+class Resource(_FrozenNoExtraBaseModel):
     """A model defining content and relations of a resource
     of a specific class.
     """
 
-    content: dict[str, Any] = Field(
+    content: FrozenDict[str, ContentPropertyValue] = Field(
         ...,
         description=(
             "The content of the resource that complies with the content schema defined"
             + " in the corresponding schemapack."
         ),
     )
 
-    relations: dict[
+    relations: FrozenDict[
         RelationPropertyName, Union[Optional[ResourceId], ResourceIdSet]
     ] = Field(
-        {},
+        FrozenDict(),
         description=(
             "A dictionary containing the relations of the resource to other resources."
             + " Each key correspond to the name of a relation property as per the"
             + " schemapack definition. Each value could be one of the following types"
             + " depending on the corresponding schemapack definition:"
             + " (1) a id of a single target resource (multiple.target is False),"
             + " (2) None (multiple.target and mandatory.target are both False),"
@@ -107,15 +113,15 @@
             + " (4) an empty set (multiple.target is True and mandatory.target is"
             + " False)."
         ),
     )
 
     def get_target_id_set(
         self, relation_name: RelationPropertyName, do_not_raise: bool = False
-    ) -> set[ResourceId]:
+    ) -> frozenset[ResourceId]:
         """Get the target ids for the given relation always represented as a set.
         This is even the case if the actual value in the relations dict is a single
         string (translated into a list of length one) or None (translated into an
         empty set). If do_not_raise is True, the method will return an empty set
         even if the relation name does not exist in the relations dict.
 
         Raises:
@@ -123,37 +129,37 @@
                 If the given relation name does not exist in the relations dict and
                 do_not_raise is False.
         """
         try:
             targets = self.relations[relation_name]
         except KeyError:
             if do_not_raise:
-                return set()
+                return frozenset()
             raise
 
         if targets is None:
-            return set()
-        if isinstance(targets, set):
+            return frozenset()
+        if isinstance(targets, frozenset):
             return targets
-        return {targets}
+        return frozenset({targets})
 
 
-class DataPack(_NoExtraBaseModel):
+class DataPack(_FrozenNoExtraBaseModel):
     """A model for describing a schemapack definition."""
 
     datapack: SupportedDataPackVersions = Field(
         ...,
         description=(
             "Has two purposes: (1) it clearly identifies a YAML/JSON document as"
             + " a datapack definition and (2) it specifies the used version of the"
             + " datapack specification."
         ),
     )
 
-    resources: dict[ClassName, dict[ResourceId, Resource]] = Field(
+    resources: FrozenDict[ClassName, FrozenDict[ResourceId, Resource]] = Field(
         ...,
         description=(
             "A nested dictionary containing resources per class name (keys on the first"
             + " level) and resource ID (keys on the second level). Each class defined"
             + " in the schemapack must be present even if no resources are defined for"
             + " it in this datapack."
         ),
```

### Comparing `schemapack-2.0.0a3/src/schemapack/_internals/spec/schemapack.py` & `schemapack-2.0.0a4/src/schemapack/_internals/spec/schemapack.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -14,99 +14,69 @@
 # limitations under the License.
 #
 """Models representing the schemapack spec.
 
 Warning: This is an internal part of the library and might change without notice.
 """
 
-import json
 import typing
-from functools import cached_property
+from collections.abc import Mapping
 from pathlib import Path
-from typing import Any, Literal, Optional, Union
+from typing import Any, Literal, Optional, Union, cast
 
+from arcticfreeze import FrozenDict, freeze
 from immutabledict import immutabledict
 from pydantic import (
-    BaseModel,
-    ConfigDict,
     Field,
-    field_serializer,
     field_validator,
     model_validator,
 )
 from pydantic_core import PydanticCustomError
 
-from schemapack._internals.spec.custom_types import FrozenDict
+from schemapack._internals.spec.base import _FrozenNoExtraBaseModel
 from schemapack._internals.utils import JsonSchemaError, assert_valid_json_schema
 from schemapack.exceptions import ParsingError
 from schemapack.spec.custom_types import (
     ClassName,
     ContentPropertyName,
     IdPropertyName,
     RelationPropertyName,
 )
 from schemapack.utils import read_json_or_yaml_mapping
 
 SupportedSchemaPackVersions = Literal["0.3.0"]
 SUPPORTED_SCHEMA_PACK_VERSIONS = typing.get_args(SupportedSchemaPackVersions)
 
 
-class _FrozenBaseModel(BaseModel):
-    """A BaseModel that cannot be changed after initialization."""
+def validate_object_json_schema(value: Mapping[str, Any]):
+    """Check if the given dict represents a valid JSON Schema for object types.
 
-    model_config = ConfigDict(frozen=True, use_enum_values=True, extra="forbid")
-
-
-class ContentSchema(_FrozenBaseModel):
-    """A model for describing a schemapack content schema."""
-
-    json_schema: str = Field(
-        ...,
-        description=(
-            "String representation of JSON schema (as a JSON-formatted string)"
-            + " describing the content of the class instances."
-        ),
-    )
-
-    # cannot be cached because pydantic includes cached properties in the hash and this
-    # is unhashable:
-    @property
-    def json_schema_dict(self) -> dict[str, Any]:
-        """A dict representation of the JSON schema."""
-        return json.loads(self.json_schema)
-
-    @cached_property
-    def properties(self) -> frozenset[ContentPropertyName]:
-        """Returns a set of the content properties. If the content schema is not a
-        JSON Schema Object (but e.g. a list), an empty set is returned.
-        """
-        return frozenset(self.json_schema_dict.get("properties", {}))
+    Raises:
+        PydanticCustomError:
+            If the value is not a valid JSON Schema for object types.
+    """
+    try:
+        assert_valid_json_schema(value)
+    except JsonSchemaError as error:
+        raise PydanticCustomError(
+            "InvalidContentSchemaError",
+            "The content schema is not a valid JSON schema: {error_message}",
+            {"error_message": str(error)},
+        ) from error
 
-    @model_validator(mode="after")
-    def validate_schema(self) -> "ContentSchema":
-        """Make sure that the schema is a  valid JSON Schema."""
-        try:
-            assert_valid_json_schema(self.json_schema)
-        except JsonSchemaError as error:
-            raise PydanticCustomError(
-                "InvalidContentSchemaError",
-                "The content schema is not a valid JSON schema: {error_message}",
-                {"error_message": str(error)},
-            ) from error
+    if value.get("type") != "object":
+        raise PydanticCustomError(
+            "InvalidContentSchemaError",
+            "The content schema must be an object.",
+        )
 
-        if self.json_schema_dict.get("type") != "object":
-            raise PydanticCustomError(
-                "InvalidContentSchemaError",
-                "The content schema must be an object.",
-            )
+    return value
 
-        return self
 
-
-class MandatoryRelationSpec(_FrozenBaseModel):
+class MandatoryRelationSpec(_FrozenNoExtraBaseModel):
     """A model for describing the modality of a relation. It describes the minimum
     number of instances the origin and the target end must contribute to the relation.
     """
 
     origin: bool = Field(
         ...,
         description=(
@@ -127,15 +97,15 @@
             + " If false, the participation of the target is optional."
             + " I.e. an instance of the origin class may be connected to zero or more"
             + " instances of the target class trough this relation."
         ),
     )
 
 
-class MultipleRelationSpec(_FrozenBaseModel):
+class MultipleRelationSpec(_FrozenNoExtraBaseModel):
     """A model for describing the cardinality of a relation. It describes the maximum
     number of instances the origin and the target end may contribute to the relation.
 
     For instance, if the origin is `True` and target is `False`, the origin may
     contribute multiple instances to the relation, while the target may at most
     contribute a single instance to the relation. This is equivalent to a 'many-to-one'
     """
@@ -156,15 +126,15 @@
             + " This is equivalent to a '*-to-many' cardinality."
             + " If false, the target may at most contribute a single instance to the"
             + " relation. This is equivalent to a '*-to-one' cardinality."
         ),
     )
 
 
-class Relation(_FrozenBaseModel):
+class Relation(_FrozenNoExtraBaseModel):
     """A model for describing a schemapack relation definition."""
 
     description: Optional[str] = Field(
         None,
         description="A description of the relation.",
     )
     targetClass: str = Field(  # noqa: N815 - align with the schemapack naming scheme
@@ -187,15 +157,15 @@
             + " may contribute multiple instances to the relation, while the target may"
             + " at most contribute a single instance to the relation."
             + " This is equivalent to a 'many-to-one' cardinality."
         ),
     )
 
 
-class IDSpec(_FrozenBaseModel):
+class IDSpec(_FrozenNoExtraBaseModel):
     """A model for describing the ID property of a class definition."""
 
     propertyName: IdPropertyName = Field(  # noqa: N815 - align with the schemapack naming scheme
         ...,
         description=(
             "The name of the ID property. It must not collide with content or relations"
             + " properties."
@@ -205,99 +175,111 @@
     )
     description: Optional[str] = Field(
         None,
         description="A description of the ID property.",
     )
 
 
-class ClassDefinition(_FrozenBaseModel):
+class ClassDefinition(_FrozenNoExtraBaseModel):
     """A model for describing a schemapack class definition."""
 
     description: Optional[str] = Field(
         None,
         description=("A description of the class definition."),
     )
     id: IDSpec = Field(
         ...,
         description="The ID property of the class definition.",
     )
-    content: ContentSchema
+    content: FrozenDict[str, Any] = Field(
+        ...,
+        description=(
+            "The content schema of the class definition. It must be a valid JSON schema"
+            + " object for object types. You may also provide the path to a JSON or YAML"
+            + " file containing the schema. It will be automatically loaded."
+        ),
+    )
     relations: FrozenDict[RelationPropertyName, Relation] = Field(
         immutabledict(),
         description=(
             "A mapping of relation names to relation definitions. Relation names"
             + " should use snake_case and may only contain alphanumeric characters and"
             + " underscores. They must start with a letter."
         ),
     )
 
+    def get_content_properties(self) -> frozenset[ContentPropertyName]:
+        """Returns a set of the content properties."""
+        return frozenset(self.content.get("properties", {}))
+
     @field_validator("content", mode="before")
     @classmethod
-    def content_schema_validator(
-        cls, v: Union[ContentSchema, Path, str, dict[str, Any]]
-    ) -> ContentSchema:
-        """Validate and convert the type of the content schema.
-
-        If a str is provided, it must be a path to the JSON schema file and not the
-        JSON-formatted string representation of the JSON schema itself.
+    def load_and_validate_content_schema(
+        cls, value: Union[str, Path, Mapping]
+    ) -> FrozenDict:
+        """A validator function for content schemas that:
+        - loads a JSON or YAML file if a path is provided
+        - checks if the value is a valid JSON schema object
+        - freezes the dict representation of the schema
         """
-        if isinstance(v, ContentSchema):
-            return v
-
-        if isinstance(v, str):
+        if isinstance(value, str):
             # assume that the string is a path to a JSON or YAML file
-            v = Path(v)
+            value = Path(value)
 
-        if isinstance(v, Path):
-            if not v.is_file():
-                absolute_path = v.absolute().resolve()
+        if isinstance(value, Path):
+            if not value.is_file():
+                absolute_path = value.absolute().resolve()
                 raise PydanticCustomError(
                     "ContentSchemaNotFoundError",
                     (
                         "Content schema path does not exist or is not a file."
                         + " Absolute path: {absolute_path}"
                     ),
                     {
                         "absolute_path": absolute_path,
                     },
                 )
 
             try:
-                json_schema_dict = read_json_or_yaml_mapping(v)
+                value = read_json_or_yaml_mapping(value)
             except ParsingError as error:
                 raise PydanticCustomError(
                     "InvalidContentSchemaError",
                     (
                         "Content schema at the specified path could not be parsed as"
                         + " valid JSON or YAML."
                     ),
                 ) from error
 
-            return ContentSchema(json_schema=json.dumps(json_schema_dict))
+        if not isinstance(value, Mapping):
+            raise PydanticCustomError(
+                "InvalidContentSchemaError",
+                (
+                    "Expected a Mapping or a"
+                    + " path (pathlib.Path or str) to a JSON or"
+                    + " YAML file."
+                ),
+            )
 
-        if isinstance(v, dict):
-            return ContentSchema(json_schema=json.dumps(v))
+        try:
+            assert_valid_json_schema(value)
+        except JsonSchemaError as error:
+            raise PydanticCustomError(
+                "InvalidContentSchemaError",
+                "The content schema is not a valid JSON schema: {error_message}",
+                {"error_message": str(error)},
+            ) from error
 
-        raise PydanticCustomError(
-            "InvalidContentSchemaError",
-            (
-                "Expected an instance of class ContentSchema, a dict[str, Any], or a"
-                + " path (pathlib.Path or str) to a JSON or"
-                + " YAML file."
-            ),
-        )
+        if value.get("type") != "object":
+            raise PydanticCustomError(
+                "InvalidContentSchemaError",
+                "The content schema must be an object.",
+            )
 
-    @field_serializer("content")
-    def content_schema_serializer(
-        self, content: ContentSchema, _info
-    ) -> dict[str, Any]:
-        """Serialize the content schema by representing it as dictionary containing the
-        JSON schema itself.
-        """
-        return self.content.json_schema_dict
+        return cast(FrozenDict, freeze(value, by_superclass=True))
 
     @field_validator("relations", mode="after")
     @classmethod
     def relation_name_validator(
         cls, v: FrozenDict[str, Relation]
     ) -> FrozenDict[str, Relation]:
         """Validate relation names."""
@@ -320,15 +302,16 @@
             )
 
         return v
 
     @model_validator(mode="after")
     def relation_content_property_collisions(self) -> "ClassDefinition":
         """Check for collisions between relations and content properties."""
-        collisions = self.content.properties.intersection(set(self.relations))
+        content_properties = self.get_content_properties()
+        collisions = content_properties.intersection(set(self.relations))
 
         if collisions:
             raise PydanticCustomError(
                 "RelationsContentPropertyCollisionError",
                 (
                     "The following properties occur both in the content and the"
                     + " relations: {collisions}"
@@ -340,15 +323,15 @@
             )
 
         return self
 
     @model_validator(mode="after")
     def id_content_property_collisions(self) -> "ClassDefinition":
         """Check for collisions between the id property and content properties."""
-        if self.id.propertyName in self.content.properties:
+        if self.id.propertyName in self.get_content_properties():
             raise PydanticCustomError(
                 "IdContentPropertyCollisionError",
                 ("The id property '{id_property}' also occurs in the content."),
                 {
                     "id_property": self.id.propertyName,
                 },
             )
@@ -366,15 +349,15 @@
                     "id_property": self.id.propertyName,
                 },
             )
 
         return self
 
 
-class SchemaPack(_FrozenBaseModel):
+class SchemaPack(_FrozenNoExtraBaseModel):
     """A model for describing a schemapack definition."""
 
     schemapack: SupportedSchemaPackVersions = Field(
         ...,
         description=(
             "Has two purposes: (1) it clearly identifies a YAML/JSON document as"
             + " a schemapack definition and (2) it specifies the used version of the"
@@ -406,17 +389,17 @@
     )
 
     @model_validator(mode="before")
     @classmethod
     def check_schemapack_field_exists(cls, data: Any) -> Any:
         """Checks that the schemapack field exists and points to a supported version
         before doing anything else. Please note, this validation only takes place if the
-        data is passed as dict. However, the data can be pretty much anything.
+        data is passed as Mapping. However, the data can be pretty much anything.
         """
-        if isinstance(data, dict):
+        if isinstance(data, Mapping):
             if "schemapack" not in data:
                 raise PydanticCustomError(
                     "MissingSchemaPackVersionError",
                     (
                         "Missing a `schemapack` field. Are you sure you have passed a"
                         + " schemapack definition?"
                     ),
```

### Comparing `schemapack-2.0.0a3/src/schemapack/_internals/utils.py` & `schemapack-2.0.0a4/src/schemapack/_internals/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -17,27 +17,32 @@
 """Utility functions.
 
 Warning: This is an internal part of the library and might change without notice.
 """
 
 import json
 import os
+from collections.abc import Mapping
 from contextlib import contextmanager
-from functools import lru_cache
+from io import StringIO
 from pathlib import Path
+from typing import Any
 
 import jsonschema
 import jsonschema.exceptions
 import jsonschema.protocols
 import jsonschema.validators
 import ruamel.yaml
+from pydantic import BaseModel
 
 from schemapack.exceptions import ParsingError
 
-yaml = ruamel.yaml.YAML(typ="safe")
+yaml = ruamel.yaml.YAML(typ="rt")
+yaml.indent(mapping=2, sequence=4, offset=2)
+yaml.default_flow_style = False
 
 
 def read_json_or_yaml_mapping(path: Path) -> dict:
     """Reads a JSON object or YAML mapping from file.
 
     Raises:
         ParsingError:
@@ -61,22 +66,20 @@
     return data
 
 
 class JsonSchemaError(ValueError):
     """Raised when a JSON schema is invalid."""
 
 
-@lru_cache
-def assert_valid_json_schema(schema_str: str) -> None:
-    """Asserts that the given string is a valid JSON Schema.
+def assert_valid_json_schema(schema: Mapping[str, Any]) -> None:
+    """Asserts that the given mapping is a valid JSON Schema.
 
     Raises:
         JsonSchemaError: If the schema is invalid.
     """
-    schema = json.loads(schema_str)
     cls: type[jsonschema.protocols.Validator] = jsonschema.validators.validator_for(
         schema
     )
 
     try:
         cls.check_schema(schema)
     except jsonschema.exceptions.SchemaError as error:
@@ -89,7 +92,51 @@
     original_cwd = os.getcwd()
     os.chdir(path)
 
     try:
         yield
     finally:
         os.chdir(original_cwd)
+
+
+def model_to_serializable_dict(
+    model: BaseModel,
+) -> dict[str, Any]:
+    """Converts the provided pydantic model to a JSON-serializable dictionary.
+
+    Returns:
+        A dictionary representation of the provided model.
+    """
+    return json.loads(model.model_dump_json(exclude_defaults=True))
+
+
+def dumps_model(
+    model: BaseModel,
+    *,
+    yaml_format: bool = True,
+) -> str:
+    """Dumps the provided pydantic model as a JSON or YAML-formatted string.
+
+    Args:
+        model:
+            The model to dump.
+        yaml_format:
+            Whether to dump as YAML (`True`) or JSON (`False`).
+    """
+    model_dict = model_to_serializable_dict(model)
+
+    if yaml_format:
+        with StringIO() as buffer:
+            yaml.dump(model_dict, buffer)
+            return buffer.getvalue().strip()
+
+    return json.dumps(model_dict, indent=2)
+
+
+def write_dict(dict_: dict, *, path: Path, yaml_format: bool) -> None:
+    """Writes the provided dictionary to a file at the provided path."""
+    if yaml_format:
+        with open(path, "w", encoding="utf-8") as file:
+            yaml.dump(dict_, file)
+    else:
+        with open(path, "w", encoding="utf-8") as file:
+            json.dump(dict_, file, indent=2)
```

### Comparing `schemapack-2.0.0a3/src/schemapack/_internals/validation/__init__.py` & `schemapack-2.0.0a4/src/schemapack/_internals/validation/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `schemapack-2.0.0a3/src/schemapack/_internals/validation/_main.py` & `schemapack-2.0.0a4/src/schemapack/_internals/validation/_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `schemapack-2.0.0a3/src/schemapack/_internals/validation/base.py` & `schemapack-2.0.0a4/src/schemapack/_internals/validation/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `schemapack-2.0.0a3/src/schemapack/_internals/validation/default.py` & `schemapack-2.0.0a4/src/schemapack/_internals/validation/default.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `schemapack-2.0.0a3/src/schemapack/_internals/validation/plugins/__init__.py` & `schemapack-2.0.0a4/src/schemapack/_internals/validation/plugins/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `schemapack-2.0.0a3/src/schemapack/_internals/validation/plugins/content_schema.py` & `schemapack-2.0.0a4/src/schemapack/_internals/validation/plugins/content_schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -13,32 +13,35 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """A validation plugin."""
 
 import json
+from collections.abc import Mapping
+from typing import Any
 
 import jsonschema.exceptions
 import jsonschema.protocols
 import jsonschema.validators
 
 from schemapack._internals.validation.base import ResourceValidationPlugin
 from schemapack.exceptions import ValidationPluginError
 from schemapack.spec.custom_types import ResourceId
 from schemapack.spec.datapack import DataPack, Resource
 from schemapack.spec.schemapack import ClassDefinition
 
 
-def _get_json_schema_validator(schema_str: str) -> jsonschema.protocols.Validator:
-    """Get a JSON Schema validator for the given schema formatted as JSON string.
+def _get_json_schema_validator(
+    schema: Mapping[str, Any],
+) -> jsonschema.protocols.Validator:
+    """Get a JSON Schema validator for the given schema.
     It is assumed that the schema has already been checked for validity against the
     JSON Schema specs.
     """
-    schema = json.loads(schema_str)
     cls: type[jsonschema.protocols.Validator] = jsonschema.validators.validator_for(
         schema
     )
     return cls(schema)
 
 
 class ContentSchemaValidationPlugin(ResourceValidationPlugin):
@@ -54,26 +57,25 @@
         Returns: True if this plugin is relevant for the given class definition.
         """
         # Is always relevant since all resources must have a content schema:
         return True
 
     def __init__(self, *, class_: ClassDefinition):
         """This plugin is configured with one specific class definition of a schemapack."""
-        self._json_schema_validator = _get_json_schema_validator(
-            class_.content.json_schema
-        )
+        self._json_schema_validator = _get_json_schema_validator(class_.content)
 
     def validate(
         self, *, resource: Resource, resource_id: ResourceId, datapack: DataPack
     ):
         """Validates a specific resource of the defined class. The entire datapack is
         provided for resolving relations to resources of other classes.
 
         Raises:
             schemapack.exceptions.ValidationPluginError: If validation fails.
         """
+        json_compatible_content = json.loads(resource.model_dump_json())["content"]
         try:
-            self._json_schema_validator.validate(resource.content)
+            self._json_schema_validator.validate(json_compatible_content)
         except jsonschema.exceptions.ValidationError as error:
             raise ValidationPluginError(
                 type_="ContentValidationError", message=error.message
             ) from error
```

### Comparing `schemapack-2.0.0a3/src/schemapack/_internals/validation/plugins/expected_root.py` & `schemapack-2.0.0a4/src/schemapack/_internals/validation/plugins/expected_root.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `schemapack-2.0.0a3/src/schemapack/_internals/validation/plugins/missing_class.py` & `schemapack-2.0.0a4/src/schemapack/_internals/validation/plugins/missing_class.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `schemapack-2.0.0a3/src/schemapack/_internals/validation/plugins/missing_origin.py` & `schemapack-2.0.0a4/src/schemapack/_internals/validation/plugins/missing_origin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -85,13 +85,13 @@
 
         if any(not_referenced_target_id_by_relation.values()):
             raise ValidationPluginError(
                 type_="MissingMandatoryOriginError",
                 message=(
                     "For the following relations that are mandatory on the origin end"
                     + " the specified targets are not referenced by any origin:"
-                    + " {not_referenced_target_by_relation}"
+                    + f"{not_referenced_target_id_by_relation}"
                 ),
                 details={
                     "not_referenced_target_by_relation": not_referenced_target_id_by_relation
                 },
             )
```

### Comparing `schemapack-2.0.0a3/src/schemapack/_internals/validation/plugins/missing_relations.py` & `schemapack-2.0.0a4/src/schemapack/_internals/validation/plugins/missing_relations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `schemapack-2.0.0a3/src/schemapack/_internals/validation/plugins/missing_target.py` & `schemapack-2.0.0a4/src/schemapack/_internals/validation/plugins/missing_target.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `schemapack-2.0.0a3/src/schemapack/_internals/validation/plugins/multiple_target.py` & `schemapack-2.0.0a4/src/schemapack/_internals/validation/plugins/multiple_target.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -50,15 +50,15 @@
         provided for resolving relations to resources of other classes.
 
         Raises:
             schemapack.exceptions.ValidationPluginError: If validation fails.
         """
         wrong_relations: set[str] = set()
         for relation_name, relation in resource.relations.items():
-            is_set = isinstance(relation, set)
+            is_set = isinstance(relation, frozenset)
 
             try:
                 expected_set = self._relations[relation_name].multiple.target
             except KeyError:
                 # Unknown relations are handled in a different plugin:
                 continue
```

### Comparing `schemapack-2.0.0a3/src/schemapack/_internals/validation/plugins/one_to_many_overlap.py` & `schemapack-2.0.0a4/src/schemapack/_internals/validation/plugins/one_to_many_overlap.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `schemapack-2.0.0a3/src/schemapack/_internals/validation/plugins/target_id.py` & `schemapack-2.0.0a4/src/schemapack/_internals/validation/plugins/target_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `schemapack-2.0.0a3/src/schemapack/_internals/validation/plugins/unexpected_root.py` & `schemapack-2.0.0a4/src/schemapack/_internals/validation/plugins/unexpected_root.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `schemapack-2.0.0a3/src/schemapack/_internals/validation/plugins/unknown_class.py` & `schemapack-2.0.0a4/src/schemapack/_internals/validation/plugins/unknown_class.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `schemapack-2.0.0a3/src/schemapack/_internals/validation/plugins/unknown_relations.py` & `schemapack-2.0.0a4/src/schemapack/_internals/validation/plugins/unknown_relations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `schemapack-2.0.0a3/src/schemapack/_internals/validation/plugins/unkown_root_resource.py` & `schemapack-2.0.0a4/src/schemapack/_internals/validation/plugins/unkown_root_resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `schemapack-2.0.0a3/src/schemapack/exceptions.py` & `schemapack-2.0.0a4/src/schemapack/exceptions.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -15,16 +15,18 @@
 #
 
 """Collection of package-specific exceptions"""
 
 from schemapack._internals.exceptions import (
     BaseError,
     CircularRelationError,
+    ClassNotFoundError,
     DataPackSpecError,
     ParsingError,
+    ResourceNotFoundError,
     SchemaPackSpecError,
     SpecError,
     ValidationAssumptionError,
     ValidationError,
     ValidationErrorRecord,
     ValidationPluginError,
 )
@@ -36,8 +38,10 @@
     "ValidationError",
     "ValidationErrorRecord",
     "DataPackSpecError",
     "SchemaPackSpecError",
     "CircularRelationError",
     "ValidationPluginError",
     "ValidationAssumptionError",
+    "ResourceNotFoundError",
+    "ClassNotFoundError",
 ]
```

### Comparing `schemapack-2.0.0a3/src/schemapack/plugins.py` & `schemapack-2.0.0a4/src/schemapack/plugins.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `schemapack-2.0.0a3/src/schemapack/spec/__init__.py` & `schemapack-2.0.0a4/src/schemapack/_internals/spec/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `schemapack-2.0.0a3/src/schemapack/spec/custom_types.py` & `schemapack-2.0.0a4/src/schemapack/spec/custom_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `schemapack-2.0.0a3/src/schemapack/spec/datapack.py` & `schemapack-2.0.0a4/src/schemapack/spec/datapack.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `schemapack-2.0.0a3/src/schemapack/spec/schemapack.py` & `schemapack-2.0.0a4/src/schemapack/spec/schemapack.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -15,27 +15,25 @@
 #
 
 """Models representing the schemapack spec (part of the public API of this package)."""
 
 from schemapack._internals.spec.schemapack import (
     SUPPORTED_SCHEMA_PACK_VERSIONS,
     ClassDefinition,
-    ContentSchema,
     IDSpec,
     MandatoryRelationSpec,
     MultipleRelationSpec,
     Relation,
     SchemaPack,
     SupportedSchemaPackVersions,
 )
 
 __all__ = [
     "SUPPORTED_SCHEMA_PACK_VERSIONS",
     "SchemaPack",
     "ClassDefinition",
-    "ContentSchema",
     "IDSpec",
     "MandatoryRelationSpec",
     "MultipleRelationSpec",
     "Relation",
     "SupportedSchemaPackVersions",
 ]
```

### Comparing `schemapack-2.0.0a3/src/schemapack/utils.py` & `schemapack-2.0.0a4/src/schemapack/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -13,10 +13,13 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 
 """Utility functions."""
 
-from schemapack._internals.utils import read_json_or_yaml_mapping
+from schemapack._internals.utils import (
+    model_to_serializable_dict,
+    read_json_or_yaml_mapping,
+)
 
-__all__ = ["read_json_or_yaml_mapping"]
+__all__ = ["read_json_or_yaml_mapping", "model_to_serializable_dict"]
```

### Comparing `schemapack-2.0.0a3/src/schemapack.egg-info/PKG-INFO` & `schemapack-2.0.0a4/src/schemapack.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: schemapack
-Version: 2.0.0a3
+Version: 2.0.0a4
 Summary: Make your JSON Schemas sociable and create linked data model.
 Author-email: "German Human Genome Phenome Archive (GHGA)" <contact@ghga.de>
 License: Apache 2.0
 Project-URL: Repository, https://github.com/ghga-de/schemapack
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic<3,>=2
 Requires-Dist: pydantic_settings<3,>=2
 Requires-Dist: ruamel.yaml~=0.18.6
 Requires-Dist: jsonschema<5,>=4.19.2
-Requires-Dist: immutabledict<4,>=3.0.0
+Requires-Dist: arcticfreeze~=0.1.1
+Requires-Dist: rich<14,>13
 
 ![tests](https://github.com/ghga-de/schemapack/actions/workflows/tests.yaml/badge.svg)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/schemapack.svg)](https://pypi.python.org/pypi/schemapack/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/schemapack.svg)](https://pypi.python.org/pypi/schemapack/)
 [![Coverage Status](https://coveralls.io/repos/github/ghga-de/schemapack/badge.svg?branch=main)](https://coveralls.io/github/ghga-de/schemapack?branch=main)
 
 # schemapack
```

### Comparing `schemapack-2.0.0a3/src/schemapack.egg-info/SOURCES.txt` & `schemapack-2.0.0a4/src/schemapack.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 LICENSE
 README.md
 pyproject.toml
 src/schemapack/__init__.py
 src/schemapack/__main__.py
+src/schemapack/cli.py
 src/schemapack/exceptions.py
 src/schemapack/plugins.py
+src/schemapack/py.typed
 src/schemapack/utils.py
 src/schemapack.egg-info/PKG-INFO
 src/schemapack.egg-info/SOURCES.txt
 src/schemapack.egg-info/dependency_links.txt
+src/schemapack.egg-info/entry_points.txt
 src/schemapack.egg-info/requires.txt
 src/schemapack.egg-info/top_level.txt
 src/schemapack/_internals/__init__.py
 src/schemapack/_internals/dump.py
+src/schemapack/_internals/erd.py
 src/schemapack/_internals/exceptions.py
 src/schemapack/_internals/isolate.py
 src/schemapack/_internals/load.py
 src/schemapack/_internals/main.py
 src/schemapack/_internals/normalize.py
 src/schemapack/_internals/utils.py
+src/schemapack/_internals/cli/__init__.py
+src/schemapack/_internals/cli/exception_handling.py
+src/schemapack/_internals/cli/exit_codes.py
+src/schemapack/_internals/cli/main.py
+src/schemapack/_internals/cli/printing.py
 src/schemapack/_internals/spec/__init__.py
+src/schemapack/_internals/spec/base.py
 src/schemapack/_internals/spec/custom_types.py
 src/schemapack/_internals/spec/datapack.py
 src/schemapack/_internals/spec/schemapack.py
 src/schemapack/_internals/validation/__init__.py
 src/schemapack/_internals/validation/_main.py
 src/schemapack/_internals/validation/base.py
 src/schemapack/_internals/validation/default.py
@@ -41,13 +51,15 @@
 src/schemapack/_internals/validation/plugins/unknown_class.py
 src/schemapack/_internals/validation/plugins/unknown_relations.py
 src/schemapack/_internals/validation/plugins/unkown_root_resource.py
 src/schemapack/spec/__init__.py
 src/schemapack/spec/custom_types.py
 src/schemapack/spec/datapack.py
 src/schemapack/spec/schemapack.py
+tests/test_cli.py
 tests/test_denormalize.py
 tests/test_dump.py
+tests/test_export_mermaid.py
 tests/test_isolate.py
 tests/test_load.py
 tests/test_main.py
 tests/test_spec.py
```

### Comparing `schemapack-2.0.0a3/tests/test_denormalize.py` & `schemapack-2.0.0a4/tests/test_denormalize.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `schemapack-2.0.0a3/tests/test_load.py` & `schemapack-2.0.0a4/tests/test_load.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `schemapack-2.0.0a3/tests/test_main.py` & `schemapack-2.0.0a4/tests/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `schemapack-2.0.0a3/tests/test_spec.py` & `schemapack-2.0.0a4/tests/test_spec.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -17,19 +17,21 @@
 """Tests the models module."""
 
 import json
 
 from immutabledict import immutabledict
 
 from schemapack import load_schemapack
+from schemapack._internals.load import load_datapack
+from schemapack._internals.utils import read_json_or_yaml_mapping
 from schemapack.spec.datapack import (
     SUPPORTED_DATA_PACK_VERSIONS,
     DataPack,
 )
-from tests.fixtures.examples import VALID_SCHEMAPACK_PATHS
+from tests.fixtures.examples import VALID_DATAPACK_PATHS, VALID_SCHEMAPACK_PATHS
 
 
 def test_schemapack_is_hashable():
     """Test that instances of SchemaPack are hashable."""
     schemapack = load_schemapack(VALID_SCHEMAPACK_PATHS["simple_relations"])
     _ = hash(schemapack)
 
@@ -66,24 +68,33 @@
 
     assert hash(schemapack) != hash(schemapack_modified)
     assert schemapack != schemapack_modified
 
 
 def test_content_schema_serialization():
     """Test that content schemas of a schemapack are serialized as dicts."""
-    schemapack = load_schemapack(VALID_SCHEMAPACK_PATHS["simple_relations"])
+    schemapack_path = VALID_SCHEMAPACK_PATHS["simple_relations_condensed"]
+    schemapack = load_schemapack(schemapack_path)
+    expected_schemapack_dict = read_json_or_yaml_mapping(schemapack_path)
+
     serialized_schemapack = json.loads(schemapack.model_dump_json())
 
-    for class_name, class_ in schemapack.classes.items():
+    for class_name in schemapack.classes:
         assert (
             serialized_schemapack["classes"][class_name]["content"]
-            == class_.content.json_schema_dict
+            == expected_schemapack_dict["classes"][class_name]["content"]
         )
 
 
+def test_datapack_is_hashable():
+    """Test that instances of DataPack are hashable."""
+    datapack = load_datapack(VALID_DATAPACK_PATHS["simple_relations.simple_resources"])
+    _ = hash(datapack)
+
+
 def test_datapack_target_id_ordering_upon_dump():
     """Test that target_ids of a resource relation are sorted (i.e. the output is
     predictable) when serializing a datapack.
     """
     unsorted_target_ids = ["c", "a", "b"]
     sorted_target_ids = sorted(unsorted_target_ids)
```

