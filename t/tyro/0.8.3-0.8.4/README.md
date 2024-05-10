# Comparing `tmp/tyro-0.8.3.tar.gz` & `tmp/tyro-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tyro-0.8.3.tar", last modified: Tue Apr  9 19:25:26 2024, max compression
+gzip compressed data, was "tyro-0.8.4.tar", last modified: Fri May 10 11:56:40 2024, max compression
```

## Comparing `tyro-0.8.3.tar` & `tyro-0.8.4.tar`

### file list

```diff
@@ -1,78 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:25:26.033469 tyro-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-09 19:24:55.000000 tyro-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7851 2024-04-09 19:25:26.033469 tyro-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-04-09 19:25:23.000000 tyro-0.8.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-04-09 19:24:55.000000 tyro-0.8.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 19:25:26.033469 tyro-0.8.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:25:26.017469 tyro-0.8.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:25:26.021469 tyro-0.8.3/src/tyro/
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   101735 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/_argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    54903 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/_argparse_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    22874 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/_arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)    10584 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/_calling.py
--rw-r--r--   0 runner    (1001) docker     (127)    18609 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)    12909 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (127)    42889 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    24359 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/_instantiators.py
--rw-r--r--   0 runner    (1001) docker     (127)    25693 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)    13315 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/_singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/_strings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/_subcommand_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/_unsafe_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:25:26.021469 tyro-0.8.3/src/tyro/conf/
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/conf/_confstruct.py
--rw-r--r--   0 runner    (1001) docker     (127)     6403 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/conf/_markers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:25:26.021469 tyro-0.8.3/src/tyro/extras/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/extras/_base_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/extras/_choices_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/extras/_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/extras/_subcommand_cli_from_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:25:26.029469 tyro-0.8.3/src/tyro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7851 2024-04-09 19:25:26.000000 tyro-0.8.3/src/tyro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-09 19:25:26.000000 tyro-0.8.3/src/tyro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 19:25:26.000000 tyro-0.8.3/src/tyro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-09 19:25:26.000000 tyro-0.8.3/src/tyro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-09 19:25:26.000000 tyro-0.8.3/src/tyro.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:25:26.029469 tyro-0.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_attrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_base_configs_nested.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_boolean_optional.py
--rw-r--r--   0 runner    (1001) docker     (127)    14186 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_completion.py
--rw-r--r--   0 runner    (1001) docker     (127)    40475 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    18741 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_dcargs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18509 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_dict_namedtuple.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_dynamic_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (127)    14602 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_flax_min_py38.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_forward_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_functools.py
--rw-r--r--   0 runner    (1001) docker     (127)    12768 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_generics_and_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)    25731 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_helptext.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_initvar_min_py38.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_is_nested_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_missing.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_missing_optional_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_mixed_unions.py
--rw-r--r--   0 runner    (1001) docker     (127)    33891 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_nested.py
--rw-r--r--   0 runner    (1001) docker     (127)     9753 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_nested_in_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_new_style_annotations_min_py310.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_new_style_annotations_min_py312.py
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_new_style_annotations_min_py39.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_partial.py
--rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_positional_min_py38.py
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_pydantic_with_newtype.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_self_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_strings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_tuple_with_subcommands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_union_from_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_unsafe_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_unsupported_but_should_work.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:56:40.230034 tyro-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-10 11:56:08.000000 tyro-0.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7851 2024-05-10 11:56:40.230034 tyro-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-05-10 11:56:38.000000 tyro-0.8.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-10 11:56:08.000000 tyro-0.8.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 11:56:40.230034 tyro-0.8.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:56:40.214034 tyro-0.8.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:56:40.218034 tyro-0.8.4/src/tyro/
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-10 11:56:08.000000 tyro-0.8.4/src/tyro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101735 2024-05-10 11:56:08.000000 tyro-0.8.4/src/tyro/_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55445 2024-05-10 11:56:08.000000 tyro-0.8.4/src/tyro/_argparse_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22874 2024-05-10 11:56:08.000000 tyro-0.8.4/src/tyro/_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10584 2024-05-10 11:56:08.000000 tyro-0.8.4/src/tyro/_calling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19489 2024-05-10 11:56:08.000000 tyro-0.8.4/src/tyro/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-10 11:56:08.000000 tyro-0.8.4/src/tyro/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12929 2024-05-10 11:56:08.000000 tyro-0.8.4/src/tyro/_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42909 2024-05-10 11:56:08.000000 tyro-0.8.4/src/tyro/_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24374 2024-05-10 11:56:08.000000 tyro-0.8.4/src/tyro/_instantiators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25765 2024-05-10 11:56:08.000000 tyro-0.8.4/src/tyro/_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13315 2024-05-10 11:56:08.000000 tyro-0.8.4/src/tyro/_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-10 11:56:08.000000 tyro-0.8.4/src/tyro/_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-05-10 11:56:08.000000 tyro-0.8.4/src/tyro/_strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-05-10 11:56:08.000000 tyro-0.8.4/src/tyro/_subcommand_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-10 11:56:08.000000 tyro-0.8.4/src/tyro/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-10 11:56:08.000000 tyro-0.8.4/src/tyro/_unsafe_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:56:40.218034 tyro-0.8.4/src/tyro/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-10 11:56:08.000000 tyro-0.8.4/src/tyro/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-05-10 11:56:08.000000 tyro-0.8.4/src/tyro/conf/_confstruct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6403 2024-05-10 11:56:08.000000 tyro-0.8.4/src/tyro/conf/_markers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:56:40.218034 tyro-0.8.4/src/tyro/extras/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-10 11:56:08.000000 tyro-0.8.4/src/tyro/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-10 11:56:08.000000 tyro-0.8.4/src/tyro/extras/_base_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-10 11:56:08.000000 tyro-0.8.4/src/tyro/extras/_choices_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-05-10 11:56:08.000000 tyro-0.8.4/src/tyro/extras/_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-05-10 11:56:08.000000 tyro-0.8.4/src/tyro/extras/_subcommand_cli_from_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 11:56:08.000000 tyro-0.8.4/src/tyro/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:56:40.226034 tyro-0.8.4/src/tyro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7851 2024-05-10 11:56:40.000000 tyro-0.8.4/src/tyro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-10 11:56:40.000000 tyro-0.8.4/src/tyro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 11:56:40.000000 tyro-0.8.4/src/tyro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-10 11:56:40.000000 tyro-0.8.4/src/tyro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-10 11:56:40.000000 tyro-0.8.4/src/tyro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:56:40.226034 tyro-0.8.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-05-10 11:56:08.000000 tyro-0.8.4/tests/test_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-05-10 11:56:08.000000 tyro-0.8.4/tests/test_base_configs_nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-10 11:56:08.000000 tyro-0.8.4/tests/test_boolean_optional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14186 2024-05-10 11:56:08.000000 tyro-0.8.4/tests/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-10 11:56:08.000000 tyro-0.8.4/tests/test_completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40619 2024-05-10 11:56:08.000000 tyro-0.8.4/tests/test_conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18741 2024-05-10 11:56:08.000000 tyro-0.8.4/tests/test_dcargs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18509 2024-05-10 11:56:08.000000 tyro-0.8.4/tests/test_dict_namedtuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-10 11:56:08.000000 tyro-0.8.4/tests/test_dynamic_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15028 2024-05-10 11:56:08.000000 tyro-0.8.4/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-10 11:56:08.000000 tyro-0.8.4/tests/test_flax_min_py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-10 11:56:08.000000 tyro-0.8.4/tests/test_forward_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-10 11:56:08.000000 tyro-0.8.4/tests/test_functools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12768 2024-05-10 11:56:08.000000 tyro-0.8.4/tests/test_generics_and_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26403 2024-05-10 11:56:08.000000 tyro-0.8.4/tests/test_helptext.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-10 11:56:08.000000 tyro-0.8.4/tests/test_initvar_min_py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-10 11:56:08.000000 tyro-0.8.4/tests/test_is_nested_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-10 11:56:08.000000 tyro-0.8.4/tests/test_missing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-10 11:56:08.000000 tyro-0.8.4/tests/test_missing_optional_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-10 11:56:08.000000 tyro-0.8.4/tests/test_mixed_unions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33915 2024-05-10 11:56:08.000000 tyro-0.8.4/tests/test_nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9753 2024-05-10 11:56:08.000000 tyro-0.8.4/tests/test_nested_in_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-10 11:56:08.000000 tyro-0.8.4/tests/test_new_style_annotations_generics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-10 11:56:08.000000 tyro-0.8.4/tests/test_new_style_annotations_min_py310.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-10 11:56:08.000000 tyro-0.8.4/tests/test_new_style_annotations_min_py312.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-10 11:56:08.000000 tyro-0.8.4/tests/test_new_style_annotations_min_py39.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-10 11:56:08.000000 tyro-0.8.4/tests/test_new_style_annotations_unions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-10 11:56:08.000000 tyro-0.8.4/tests/test_partial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-05-10 11:56:08.000000 tyro-0.8.4/tests/test_positional_min_py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-05-10 11:56:08.000000 tyro-0.8.4/tests/test_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-10 11:56:08.000000 tyro-0.8.4/tests/test_pydantic_with_newtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-10 11:56:08.000000 tyro-0.8.4/tests/test_self_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-10 11:56:08.000000 tyro-0.8.4/tests/test_strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-05-10 11:56:08.000000 tyro-0.8.4/tests/test_tuple_with_subcommands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-10 11:56:08.000000 tyro-0.8.4/tests/test_union_from_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-10 11:56:08.000000 tyro-0.8.4/tests/test_unsafe_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-10 11:56:08.000000 tyro-0.8.4/tests/test_unsupported_but_should_work.py
```

### Comparing `tyro-0.8.3/LICENSE` & `tyro-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tyro-0.8.3/PKG-INFO` & `tyro-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tyro
-Version: 0.8.3
+Version: 0.8.4
 Summary: Strongly typed, zero-effort CLI interfaces
 Author-email: brentyi <brentyi@berkeley.edu>
 License: MIT
 Project-URL: GitHub, https://github.com/brentyi/tyro
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tyro Version: 0.8.3 Summary: Strongly typed, zero-
+Metadata-Version: 2.1 Name: tyro Version: 0.8.4 Summary: Strongly typed, zero-
 effort CLI interfaces Author-email: brentyi
 berkeley.edu> License: MIT Project-URL: GitHub, https://github.com/brentyi/tyro
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Classifier: License :: OSI
```

### Comparing `tyro-0.8.3/README.md` & `tyro-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `tyro-0.8.3/pyproject.toml` & `tyro-0.8.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tyro"
 authors = [
     {name = "brentyi", email = "brentyi@berkeley.edu"},
 ]
-version = "0.8.3"  # TODO: currently needs to be synchronized manually with __init__.py.
+version = "0.8.4"  # TODO: currently needs to be synchronized manually with __init__.py.
 description = "Strongly typed, zero-effort CLI interfaces"
 readme = "README.md"
 license = { text="MIT" }
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
```

### Comparing `tyro-0.8.3/src/tyro/_argparse.py` & `tyro-0.8.4/src/tyro/_argparse.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.3/src/tyro/_argparse_formatter.py` & `tyro-0.8.4/src/tyro/_argparse_formatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,17 +232,17 @@
         # No-op when the context manager is nested.
         yield
 
 
 def str_from_rich(
     renderable: RenderableType, width: Optional[int] = None, soft_wrap: bool = False
 ) -> str:
-    console = Console(width=width, theme=THEME.as_rich_theme())
-    with console.capture() as out:
-        console.print(renderable, soft_wrap=soft_wrap)
+    dummy_console = Console(width=width, theme=THEME.as_rich_theme())
+    with dummy_console.capture() as out:
+        dummy_console.print(renderable, soft_wrap=soft_wrap)
     return out.get().rstrip("\n")
 
 
 @dataclasses.dataclass(frozen=True)
 class _ArgumentInfo:
     option_strings: Tuple[str, ...]
     metavar: Optional[str]
@@ -268,20 +268,30 @@
 
 
 # We inherit from both our local mirror of argparse and the upstream one.
 # Including the latter is purely for `isinstance()`-style checks.
 class TyroArgumentParser(argparse.ArgumentParser, argparse_sys.ArgumentParser):  # type: ignore
     _parser_specification: ParserSpecification
     _parsing_known_args: bool
+    _console_outputs: bool
     _args: List[str]
 
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
 
     @override
+    def _print_message(self, message, file=None):
+        if message and self._console_outputs:
+            file = file or sys.stderr
+            try:
+                file.write(message)
+            except (AttributeError, OSError):  # pragma: no cover
+                pass
+
+    @override
     def _parse_known_args(self, arg_strings, namespace):  # pragma: no cover
         """We override _parse_known_args() to improve error messages in the presence of
         subcommands. Difference is marked with <new>...</new> below."""
 
         # <new>
         # Reset the unused argument list in the root parser.
         # Subparsers will have spaces in self.prog.
@@ -567,16 +577,14 @@
         Prints a usage message incorporating the message to stderr and
         exits.
 
         If you override this in a subclass, it should not return -- it
         should either exit or raise an exception.
         """
 
-        console = Console(theme=THEME.as_rich_theme())
-
         extra_info: List[RenderableType] = []
         global global_unrecognized_args
         if len(global_unrecognized_args) == 0 and message.startswith(
             "unrecognized options: "
         ):
             global_unrecognized_args = message.partition(":")[2].strip().split(" ")
 
@@ -823,28 +831,32 @@
                     extra_info.append(
                         Padding(
                             f"in [green]{maybe_arg.usage_hint}[/green]",
                             (0, 0, 0, 12),
                         )
                     )
 
-        console.print(
-            Panel(
-                Group(
-                    f"{message[0].upper() + message[1:]}" if len(message) > 0 else "",
-                    *extra_info,
-                    Rule(style=Style(color="red")),
-                    f"For full helptext, run [bold]{self.prog} --help[/bold]",
-                ),
-                title=f"[bold]{message_title}[/bold]",
-                title_align="left",
-                border_style=Style(color="bright_red"),
-                expand=False,
+        if self._console_outputs:
+            console = Console(theme=THEME.as_rich_theme(), stderr=True)
+            console.print(
+                Panel(
+                    Group(
+                        f"{message[0].upper() + message[1:]}"
+                        if len(message) > 0
+                        else "",
+                        *extra_info,
+                        Rule(style=Style(color="red")),
+                        f"For full helptext, run [bold]{self.prog} --help[/bold]",
+                    ),
+                    title=f"[bold]{message_title}[/bold]",
+                    title_align="left",
+                    border_style=Style(color="bright_red"),
+                    expand=False,
+                )
             )
-        )
         sys.exit(2)
 
 
 class TyroArgparseHelpFormatter(argparse.RawDescriptionHelpFormatter):
     def __init__(self, prog: str):
         indent_increment = 4
         width = shutil.get_terminal_size().columns - 2
@@ -939,16 +951,18 @@
         def format_help(self):
             if self.parent is None:
                 return self._tyro_format_root()
             else:
                 return self._tyro_format_nonroot()
 
         def _tyro_format_root(self):
-            console = Console(width=self.formatter._width, theme=THEME.as_rich_theme())
-            with console.capture() as capture:
+            dummy_console = Console(
+                width=self.formatter._width, theme=THEME.as_rich_theme()
+            )
+            with dummy_console.capture() as capture:
                 # Get rich renderables from items.
                 top_parts = []
                 column_parts = []
                 column_parts_lines = []
                 for func, args in self.items:
                     item_content = func(*args)
                     if item_content is None:
@@ -1004,16 +1018,16 @@
                     column_lines[chosen_column] += l
                 columns = Columns(
                     [Group(*g) for g in column_parts_grouped],
                     column_first=True,
                     width=column_width,
                 )
 
-                console.print(Group(*top_parts))
-                console.print(columns)
+                dummy_console.print(Group(*top_parts))
+                dummy_console.print(columns)
             return capture.get()
 
         def _format_action(self, action: argparse.Action):
             invocation = self.formatter._format_action_invocation(action)
             indent = self.formatter._current_indent
             help_position = min(
                 self.formatter._action_max_length + 4,
```

### Comparing `tyro-0.8.3/src/tyro/_arguments.py` & `tyro-0.8.4/src/tyro/_arguments.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.3/src/tyro/_calling.py` & `tyro-0.8.4/src/tyro/_calling.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.3/src/tyro/_cli.py` & `tyro-0.8.4/src/tyro/_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,77 +48,82 @@
     *,
     prog: Optional[str] = None,
     description: Optional[str] = None,
     args: Optional[Sequence[str]] = None,
     default: Optional[OutT] = None,
     return_unknown_args: Literal[False] = False,
     use_underscores: bool = False,
+    console_outputs: bool = True,
 ) -> OutT: ...
 
 
 @overload
 def cli(
     f: TypeForm[OutT],
     *,
     prog: Optional[str] = None,
     description: Optional[str] = None,
     args: Optional[Sequence[str]] = None,
     default: Optional[OutT] = None,
     return_unknown_args: Literal[True],
     use_underscores: bool = False,
+    console_outputs: bool = True,
 ) -> Tuple[OutT, List[str]]: ...
 
 
 @overload
 def cli(
     f: Callable[..., OutT],
     *,
     prog: Optional[str] = None,
     description: Optional[str] = None,
     args: Optional[Sequence[str]] = None,
-    # Note that passing a default makes sense for things like dataclasses, but are not
-    # supported for general callables. These can, however, be specified in the signature
-    # of the callable itself.
+    # Passing a default makes sense for things like dataclasses, but are not
+    # supported for general callables. These can, however, be specified in the
+    # signature of the callable itself.
     default: None = None,
     return_unknown_args: Literal[False] = False,
     use_underscores: bool = False,
+    console_outputs: bool = True,
 ) -> OutT: ...
 
 
 @overload
 def cli(
     f: Callable[..., OutT],
     *,
     prog: Optional[str] = None,
     description: Optional[str] = None,
     args: Optional[Sequence[str]] = None,
-    # Note that passing a default makes sense for things like dataclasses, but are not
-    # supported for general callables. These can, however, be specified in the signature
-    # of the callable itself.
+    # Passing a default makes sense for things like dataclasses, but are not
+    # supported for general callables. These can, however, be specified in the
+    # signature of the callable itself.
     default: None = None,
     return_unknown_args: Literal[True],
     use_underscores: bool = False,
+    console_outputs: bool = True,
 ) -> Tuple[OutT, List[str]]: ...
 
 
 def cli(
     f: Union[TypeForm[OutT], Callable[..., OutT]],
     *,
     prog: Optional[str] = None,
     description: Optional[str] = None,
     args: Optional[Sequence[str]] = None,
     default: Optional[OutT] = None,
     return_unknown_args: bool = False,
     use_underscores: bool = False,
+    console_outputs: bool = True,
     **deprecated_kwargs,
 ) -> Union[OutT, Tuple[OutT, List[str]]]:
     """Call or instantiate `f`, with inputs populated from an automatically generated
     CLI interface.
 
-    `f` should have type-annotated inputs, and can be a function or type. Note that if
+    `f` should have type-annotated inputs, and can be a function or type. If
     `f` is a type, `tyro.cli()` returns an instance.
 
     The parser is generated by populating helptext from docstrings and types from
     annotations; a broad range of core type annotations are supported.
     - Types natively accepted by `argparse`: str, int, float, pathlib.Path, etc.
     - Default values for optional parameters.
     - Booleans, which are automatically converted to flags when provided a default
@@ -155,24 +160,30 @@
             `argparse.ArgumentParser()`.
         description: Description text for the parser, displayed when the --help flag is
             passed in. If not specified, `f`'s docstring is used. Mirrors argument from
             `argparse.ArgumentParser()`.
         args: If set, parse arguments from a sequence of strings instead of the
             commandline. Mirrors argument from `argparse.ArgumentParser.parse_args()`.
         default: An instance of `OutT` to use for default values; supported if `f` is a
-            type like a dataclass or dictionary, but not if `f` is a general callable like
-            a function or standard class. Helpful for merging CLI arguments with values
-            loaded from elsewhere. (for example, a config object loaded from a yaml file)
+            type like a dataclass or dictionary, but not if `f` is a general callable
+            like a function or standard class. Helpful for merging CLI arguments with
+            values loaded from elsewhere. (for example, a config object loaded from a
+            yaml file)
         return_unknown_args: If True, return a tuple of the output of `f` and a list of
             unknown arguments. Mirrors the unknown arguments returned from
             `argparse.ArgumentParser.parse_known_args()`.
         use_underscores: If True, use underscores as a word delimeter instead of hyphens.
-            This primarily impacts helptext; underscores and hyphens are treated equivalently
-            when parsing happens. We default helptext to hyphens to follow the GNU style guide.
+            This primarily impacts helptext; underscores and hyphens are treated
+            equivalently when parsing happens. We default helptext to hyphens to follow
+            the GNU style guide.
             https://www.gnu.org/software/libc/manual/html_node/Argument-Syntax.html
+        console_outputs: If set to `False`, parsing errors and help messages will be
+            supressed. This can be useful for distributed settings, where `tyro.cli()`
+            is called from multiple workers but we only want console outputs from the
+            main one.
 
     Returns:
         The output of `f(...)` or an instance `f`. If `f` is a class, the two are
         equivalent. If `return_unknown_args` is True, returns a tuple of the output of
         `f(...)` and a list of unknown arguments.
     """
 
@@ -186,14 +197,15 @@
             prog=prog,
             description=description,
             args=args,
             default=default,
             return_parser=False,
             return_unknown_args=return_unknown_args,
             use_underscores=use_underscores,
+            console_outputs=console_outputs,
             **deprecated_kwargs,
         )
 
     # Prevent unnecessary memory usage.
     _unsafe_cache.clear_cache()
 
     if return_unknown_args:
@@ -206,37 +218,40 @@
 def get_parser(
     f: TypeForm[OutT],
     *,
     prog: Optional[str] = None,
     description: Optional[str] = None,
     default: Optional[OutT] = None,
     use_underscores: bool = False,
+    console_outputs: bool = True,
 ) -> argparse.ArgumentParser: ...
 
 
 @overload
 def get_parser(
     f: Callable[..., OutT],
     *,
     prog: Optional[str] = None,
     description: Optional[str] = None,
     default: Optional[OutT] = None,
     use_underscores: bool = False,
+    console_outputs: bool = True,
 ) -> argparse.ArgumentParser: ...
 
 
 def get_parser(
     f: Union[TypeForm[OutT], Callable[..., OutT]],
     *,
-    # Note that we have no `args` argument, since this is only used when
+    # We have no `args` argument, since this is only used when
     # parser.parse_args() is called.
     prog: Optional[str] = None,
     description: Optional[str] = None,
     default: Optional[OutT] = None,
     use_underscores: bool = False,
+    console_outputs: bool = True,
 ) -> argparse.ArgumentParser:
     """Get the `argparse.ArgumentParser` object generated under-the-hood by
     `tyro.cli()`. Useful for tools like `sphinx-argparse`, `argcomplete`, etc.
 
     For tab completion, we recommend using `tyro.cli()`'s built-in `--tyro-write-completion`
     flag."""
     with _strings.delimeter_context("_" if use_underscores else "-"):
@@ -247,27 +262,29 @@
                 prog=prog,
                 description=description,
                 args=None,
                 default=default,
                 return_parser=True,
                 return_unknown_args=False,
                 use_underscores=use_underscores,
+                console_outputs=console_outputs,
             ),
         )
 
 
 def _cli_impl(
     f: Union[TypeForm[OutT], Callable[..., OutT]],
     *,
     prog: Optional[str] = None,
     description: Optional[str],
     args: Optional[Sequence[str]],
     default: Optional[OutT],
     return_parser: bool,
     return_unknown_args: bool,
+    console_outputs: bool,
     **deprecated_kwargs,
 ) -> Union[
     OutT,
     argparse.ArgumentParser,
     Tuple[OutT, List[str]],
 ]:
     """Helper for stitching the `tyro` pipeline together."""
@@ -382,14 +399,15 @@
         parser = _argparse_formatter.TyroArgumentParser(
             prog=prog,
             formatter_class=_argparse_formatter.TyroArgparseHelpFormatter,
             allow_abbrev=False,
         )
         parser._parser_specification = parser_spec
         parser._parsing_known_args = return_unknown_args
+        parser._console_outputs = console_outputs
         parser._args = args
         parser_spec.apply(parser)
 
         # Print help message when no arguments are passed in. (but arguments are
         # expected)
         # if len(args) == 0 and parser_spec.has_required_args:
         #     args = ["--help"]
@@ -458,47 +476,48 @@
         from rich.padding import Padding
         from rich.panel import Panel
         from rich.rule import Rule
         from rich.style import Style
 
         from ._argparse_formatter import THEME
 
-        console = Console(theme=THEME.as_rich_theme())
-        console.print(
-            Panel(
-                Group(
-                    "[bright_red][bold]Error parsing"
-                    f" {e.arg.lowered.name_or_flag if isinstance(e.arg, _arguments.ArgumentDefinition) else e.arg}[/bold]:[/bright_red] {e.message}",
-                    *cast(  # Cast to appease mypy...
-                        List[RenderableType],
-                        (
-                            []
-                            if not isinstance(e.arg, _arguments.ArgumentDefinition)
-                            or e.arg.lowered.help is None
-                            else [
-                                Rule(style=Style(color="red")),
-                                "Argument helptext:",
-                                Padding(
-                                    Group(
-                                        f"{e.arg.lowered.name_or_flag} [bold]{e.arg.lowered.metavar}[/bold]",
-                                        e.arg.lowered.help,
+        if console_outputs:
+            console = Console(theme=THEME.as_rich_theme(), stderr=True)
+            console.print(
+                Panel(
+                    Group(
+                        "[bright_red][bold]Error parsing"
+                        f" {e.arg.lowered.name_or_flag if isinstance(e.arg, _arguments.ArgumentDefinition) else e.arg}[/bold]:[/bright_red] {e.message}",
+                        *cast(  # Cast to appease mypy...
+                            List[RenderableType],
+                            (
+                                []
+                                if not isinstance(e.arg, _arguments.ArgumentDefinition)
+                                or e.arg.lowered.help is None
+                                else [
+                                    Rule(style=Style(color="red")),
+                                    "Argument helptext:",
+                                    Padding(
+                                        Group(
+                                            f"{e.arg.lowered.name_or_flag} [bold]{e.arg.lowered.metavar}[/bold]",
+                                            e.arg.lowered.help,
+                                        ),
+                                        pad=(0, 0, 0, 4),
                                     ),
-                                    pad=(0, 0, 0, 4),
-                                ),
-                                Rule(style=Style(color="red")),
-                                f"For full helptext, see [bold]{parser.prog} --help[/bold]",
-                            ]
+                                    Rule(style=Style(color="red")),
+                                    f"For full helptext, see [bold]{parser.prog} --help[/bold]",
+                                ]
+                            ),
                         ),
                     ),
-                ),
-                title="[bold]Value error[/bold]",
-                title_align="left",
-                border_style=Style(color="red"),
+                    title="[bold]Value error[/bold]",
+                    title_align="left",
+                    border_style=Style(color="red"),
+                )
             )
-        )
         sys.exit(2)
 
     assert len(value_from_prefixed_field_name.keys() - consumed_keywords) == 0, (
         f"Parsed {value_from_prefixed_field_name.keys()}, but only consumed"
         f" {consumed_keywords}"
     )
```

### Comparing `tyro-0.8.3/src/tyro/_docstrings.py` & `tyro-0.8.4/src/tyro/_docstrings.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import collections.abc
 import dataclasses
 import functools
 import inspect
 import io
 import itertools
 import tokenize
-from typing import Callable, Dict, Generic, Hashable, List, Optional, Type, TypeVar
+from typing import Callable, Dict, Generic, Hashable, List, Optional, Set, Type, TypeVar
 
 import docstring_parser
 from typing_extensions import get_origin, is_typeddict
 
 from . import _resolver, _strings, _unsafe_cache
 
 T = TypeVar("T", bound=Callable)
@@ -277,15 +277,15 @@
 
     if len(comments) > 0 and not (is_sphinx_doc_comment and not directly_above_field):
         return _strings.remove_single_line_breaks("\n".join(reversed(comments)))
 
     return None
 
 
-_callable_description_blocklist = set(
+_callable_description_blocklist: Set[Hashable] = set(
     filter(
         lambda x: isinstance(x, Hashable),  # type: ignore
         itertools.chain(__builtins__.values(), vars(collections.abc).values()),  # type: ignore
     )
 )
```

### Comparing `tyro-0.8.3/src/tyro/_fields.py` & `tyro-0.8.4/src/tyro/_fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     Callable,
     Dict,
     FrozenSet,
     Hashable,
     Iterable,
     List,
     Optional,
+    Set,
     Tuple,
     TypeVar,
     Union,
     cast,
 )
 
 import docstring_parser
@@ -357,15 +358,15 @@
 # Implementation details below.
 
 
 DefaultInstance = Union[
     Any, PropagatingMissingType, NonpropagatingMissingType, ExcludeFromCallType
 ]
 
-_known_parsable_types = set(
+_known_parsable_types: Set[type] = set(
     filter(
         lambda x: isinstance(x, Hashable),  # type: ignore
         itertools.chain(
             __builtins__.values(),  # type: ignore
             vars(typing).values(),
             vars(typing_extensions).values(),
             vars(collections.abc).values(),
```

### Comparing `tyro-0.8.3/src/tyro/_instantiators.py` & `tyro-0.8.4/src/tyro/_instantiators.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
             raise ValueError(f"invalid choice: {strings} (choose from {self.choices}))")
 
 
 class UnsupportedTypeAnnotationError(Exception):
     """Exception raised when an unsupported type annotation is detected."""
 
 
-_builtin_set = set(
+_builtin_set: Set[Hashable] = set(
     filter(
         lambda x: isinstance(x, Hashable),  # type: ignore
         __builtins__.values(),  # type: ignore
     )
 )
```

### Comparing `tyro-0.8.3/src/tyro/_parsers.py` & `tyro-0.8.4/src/tyro/_parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -625,14 +625,15 @@
             )
 
             # Attributes used for error message generation.
             assert isinstance(subparser, _argparse_formatter.TyroArgumentParser)
             assert isinstance(parent_parser, _argparse_formatter.TyroArgumentParser)
             subparser._parsing_known_args = parent_parser._parsing_known_args
             subparser._parser_specification = parent_parser._parser_specification
+            subparser._console_outputs = parent_parser._console_outputs
             subparser._args = parent_parser._args
 
             subparser_tree_leaves.extend(subparser_def.apply(subparser))
 
         return tuple(subparser_tree_leaves)
```

### Comparing `tyro-0.8.3/src/tyro/_resolver.py` & `tyro-0.8.4/src/tyro/_resolver.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.3/src/tyro/_strings.py` & `tyro-0.8.4/src/tyro/_strings.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.3/src/tyro/_subcommand_matching.py` & `tyro-0.8.4/src/tyro/_subcommand_matching.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.3/src/tyro/_typing.py` & `tyro-0.8.4/src/tyro/_typing.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.3/src/tyro/_unsafe_cache.py` & `tyro-0.8.4/src/tyro/_unsafe_cache.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.3/src/tyro/conf/__init__.py` & `tyro-0.8.4/src/tyro/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.3/src/tyro/conf/_confstruct.py` & `tyro-0.8.4/src/tyro/conf/_confstruct.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.3/src/tyro/conf/_markers.py` & `tyro-0.8.4/src/tyro/conf/_markers.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.3/src/tyro/extras/__init__.py` & `tyro-0.8.4/src/tyro/extras/__init__.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.3/src/tyro/extras/_base_configs.py` & `tyro-0.8.4/src/tyro/extras/_base_configs.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.3/src/tyro/extras/_choices_type.py` & `tyro-0.8.4/src/tyro/extras/_choices_type.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.3/src/tyro/extras/_serialization.py` & `tyro-0.8.4/src/tyro/extras/_serialization.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.3/src/tyro/extras/_subcommand_cli_from_dict.py` & `tyro-0.8.4/src/tyro/extras/_subcommand_cli_from_dict.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.3/src/tyro.egg-info/PKG-INFO` & `tyro-0.8.4/src/tyro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tyro
-Version: 0.8.3
+Version: 0.8.4
 Summary: Strongly typed, zero-effort CLI interfaces
 Author-email: brentyi <brentyi@berkeley.edu>
 License: MIT
 Project-URL: GitHub, https://github.com/brentyi/tyro
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tyro Version: 0.8.3 Summary: Strongly typed, zero-
+Metadata-Version: 2.1 Name: tyro Version: 0.8.4 Summary: Strongly typed, zero-
 effort CLI interfaces Author-email: brentyi
 berkeley.edu> License: MIT Project-URL: GitHub, https://github.com/brentyi/tyro
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Classifier: License :: OSI
```

### Comparing `tyro-0.8.3/src/tyro.egg-info/SOURCES.txt` & `tyro-0.8.4/src/tyro.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -50,17 +50,19 @@
 tests/test_initvar_min_py38.py
 tests/test_is_nested_type.py
 tests/test_missing.py
 tests/test_missing_optional_packages.py
 tests/test_mixed_unions.py
 tests/test_nested.py
 tests/test_nested_in_containers.py
+tests/test_new_style_annotations_generics.py
 tests/test_new_style_annotations_min_py310.py
 tests/test_new_style_annotations_min_py312.py
 tests/test_new_style_annotations_min_py39.py
+tests/test_new_style_annotations_unions.py
 tests/test_partial.py
 tests/test_positional_min_py38.py
 tests/test_pydantic.py
 tests/test_pydantic_with_newtype.py
 tests/test_self_type.py
 tests/test_strings.py
 tests/test_tuple_with_subcommands.py
```

### Comparing `tyro-0.8.3/src/tyro.egg-info/requires.txt` & `tyro-0.8.4/src/tyro.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tyro-0.8.3/tests/test_attrs.py` & `tyro-0.8.4/tests/test_attrs.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.3/tests/test_base_configs_nested.py` & `tyro-0.8.4/tests/test_base_configs_nested.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.3/tests/test_boolean_optional.py` & `tyro-0.8.4/tests/test_boolean_optional.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.3/tests/test_collections.py` & `tyro-0.8.4/tests/test_collections.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     class A:
         x: tyro.conf.Positional[Tuple[Literal[1, 2, 3], ...]] = (1, 2)
 
     assert tyro.cli(A, args=["1", "2", "3"]) == A(x=(1, 2, 3))
     assert tyro.cli(A, args=[]) == A(x=(1, 2))
 
     target = io.StringIO()
-    with pytest.raises(SystemExit), contextlib.redirect_stdout(target):
+    with pytest.raises(SystemExit), contextlib.redirect_stderr(target):
         tyro.cli(A, args=["1", "2", "3", "4"])
     assert "invalid choice" in target.getvalue()
 
 
 def test_tuples_fixed_multitype() -> None:
     @dataclasses.dataclass
     class A:
```

### Comparing `tyro-0.8.3/tests/test_completion.py` & `tyro-0.8.4/tests/test_completion.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.3/tests/test_conf.py` & `tyro-0.8.4/tests/test_conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import io
 import json as json_
 import shlex
 import sys
 from typing import Any, Dict, Generic, List, Tuple, Type, TypeVar, Union
 
 import pytest
-from helptext_utils import get_helptext
+from helptext_utils import get_helptext_with_checks
 from typing_extensions import Annotated
 
 import tyro
 
 
 def test_suppress_subcommand() -> None:
     @dataclasses.dataclass
@@ -28,15 +28,15 @@
     class DefaultInstanceSubparser:
         x: int
         # bc: Union[DefaultInstanceHTTPServer, DefaultInstanceSMTPServer]
         bc: tyro.conf.Suppress[
             Union[DefaultInstanceHTTPServer, DefaultInstanceSMTPServer]
         ] = dataclasses.field(default_factory=DefaultInstanceHTTPServer)
 
-    assert "bc" not in get_helptext(DefaultInstanceSubparser)
+    assert "bc" not in get_helptext_with_checks(DefaultInstanceSubparser)
 
 
 def test_omit_subcommand_prefix() -> None:
     @dataclasses.dataclass
     class DefaultInstanceHTTPServer:
         y: int = 0
         flag: bool = True
@@ -410,27 +410,27 @@
             Annotated[B, tyro.conf.subcommand("three", default=default_three)],
         ]
 
     # Match by hash.
     def main_one(x: Nested = Nested(default_one)) -> None:
         pass
 
-    assert "default: x.subcommand:one" in get_helptext(main_one)
+    assert "default: x.subcommand:one" in get_helptext_with_checks(main_one)
 
     # Match by value.
     def main_two(x: Nested = Nested(B(9))) -> None:
         pass
 
-    assert "default: x.subcommand:three" in get_helptext(main_two)
+    assert "default: x.subcommand:three" in get_helptext_with_checks(main_two)
 
     # Match by type.
     def main_three(x: Nested = Nested(B(15))) -> None:
         pass
 
-    assert "default: x.subcommand:one" in get_helptext(main_three)
+    assert "default: x.subcommand:one" in get_helptext_with_checks(main_three)
 
 
 def test_flag() -> None:
     """When boolean flags have no default value, they must be explicitly specified."""
 
     @dataclasses.dataclass
     class A:
@@ -547,42 +547,42 @@
     class Struct:
         a: int = 5
         b: tyro.conf.Suppress[str] = "7"
 
     def main(x: Any = Struct()):
         pass
 
-    helptext = get_helptext(main)
+    helptext = get_helptext_with_checks(main)
     assert "--x.a" in helptext
     assert "--x.b" not in helptext
 
 
 def test_suppress_manual_fixed() -> None:
     @dataclasses.dataclass
     class Struct:
         a: int = 5
         b: tyro.conf.SuppressFixed[tyro.conf.Fixed[str]] = "7"
 
     def main(x: Any = Struct()):
         pass
 
-    helptext = get_helptext(main)
+    helptext = get_helptext_with_checks(main)
     assert "--x.a" in helptext
     assert "--x.b" not in helptext
 
 
 def test_suppress_manual_fixed_one_arg_only() -> None:
     @dataclasses.dataclass
     class Struct:
         b: tyro.conf.SuppressFixed[tyro.conf.Fixed[str]] = "7"
 
     def main(x: Any = Struct()):
         pass
 
-    helptext = get_helptext(main)
+    helptext = get_helptext_with_checks(main)
     assert "--x.a" not in helptext
     assert "--x.b" not in helptext
 
 
 def test_suppress_auto_fixed() -> None:
     @dataclasses.dataclass
     class Struct:
@@ -590,15 +590,15 @@
 
         def b(self, x):
             return 5
 
     def main(x: tyro.conf.SuppressFixed[Any] = Struct()):
         pass
 
-    helptext = get_helptext(main)
+    helptext = get_helptext_with_checks(main)
     assert "--x.a" in helptext
     assert "--x.b" not in helptext
 
 
 def test_argconf_help() -> None:
     @dataclasses.dataclass
     class Struct:
@@ -606,15 +606,15 @@
             int, tyro.conf.arg(name="nice", help="Hello world", metavar="NUMBER")
         ] = 5
         b: tyro.conf.Suppress[str] = "7"
 
     def main(x: Any = Struct()) -> int:
         return x.a
 
-    helptext = get_helptext(main)
+    helptext = get_helptext_with_checks(main)
     assert "Hello world" in helptext
     assert "INT" not in helptext
     assert "NUMBER" in helptext
     assert "--x.a" not in helptext
     assert "--x.nice" in helptext
     assert "--x.b" not in helptext
 
@@ -632,15 +632,15 @@
             ),
         ] = 5
         b: tyro.conf.Suppress[str] = "7"
 
     def main(x: Any = Struct()) -> int:
         return x.a
 
-    helptext = get_helptext(main)
+    helptext = get_helptext_with_checks(main)
     assert "Hello world" in helptext
     assert "INT" not in helptext
     assert "NUMBER" in helptext
     assert "--x.a" not in helptext
     assert "--x.nice" not in helptext
     assert "--nice" in helptext
     assert "--x.b" not in helptext
@@ -1046,15 +1046,15 @@
         ]
 
     assert tyro.cli(
         Config, args=shlex.split('--x.json \'{"hello": "world"}\'')
     ) == Config(x={"hello": "world"})
 
     target = io.StringIO()
-    with pytest.raises(SystemExit), contextlib.redirect_stdout(target):
+    with pytest.raises(SystemExit), contextlib.redirect_stderr(target):
         tyro.cli(Config, args="--x.json 5".split(" "))
 
     error = target.getvalue()
     assert "Error parsing x: 5 is not a dict!" in error
 
 
 def test_custom_constructor_4() -> None:
@@ -1101,15 +1101,15 @@
 
     # --x.b is required!
     with pytest.raises(SystemExit):
         tyro.cli(Config, args="5".split(" "))
 
     # --x.a and --x.b are required!
     target = io.StringIO()
-    with pytest.raises(SystemExit), contextlib.redirect_stdout(target):
+    with pytest.raises(SystemExit), contextlib.redirect_stderr(target):
         tyro.cli(Config, args="--x.c 5".split(" "))
     error = target.getvalue()
     assert "We're missing" in error
 
 
 def test_custom_constructor_7() -> None:
     @dataclasses.dataclass
@@ -1135,15 +1135,15 @@
 
     # --x.struct.b is required!
     with pytest.raises(SystemExit):
         tyro.cli(Config, args="--x.struct.a 5".split(" "))
 
     # --x.struct.a and --x.struct.b are required!
     target = io.StringIO()
-    with pytest.raises(SystemExit), contextlib.redirect_stdout(target):
+    with pytest.raises(SystemExit), contextlib.redirect_stderr(target):
         tyro.cli(Config, args="--x.struct.c 5".split(" "))
     error = target.getvalue()
     assert "We're missing arguments" in error
     assert "'b'" in error
     assert "'a'" in error  # The 5 is parsed into `a`.
 
 
@@ -1169,15 +1169,15 @@
 
     # --x.struct.b is required!
     with pytest.raises(SystemExit):
         tyro.cli(Config, args="5".split(" "))
 
     # --x.struct.a and --x.struct.b are required!
     target = io.StringIO()
-    with pytest.raises(SystemExit), contextlib.redirect_stdout(target):
+    with pytest.raises(SystemExit), contextlib.redirect_stderr(target):
         tyro.cli(Config, args="--x.struct.b 5".split(" "))
     error = target.getvalue()
     assert "We're missing arguments" in error
     assert "'a'" in error
     assert "'b'" not in error
 
 
@@ -1213,22 +1213,22 @@
 
     # --x.struct.b is required!
     with pytest.raises(SystemExit):
         tyro.cli(Config, args="--x.struct.a 5".split(" "))
 
     # --x.struct.a and --x.struct.b are required!
     target = io.StringIO()
-    with pytest.raises(SystemExit), contextlib.redirect_stdout(target):
+    with pytest.raises(SystemExit), contextlib.redirect_stderr(target):
         tyro.cli(Config, args="--x.struct.b 5".split(" "))
     error = target.getvalue()
     assert "We're missing arguments" in error
     assert "'a'" in error
     assert "'b'" not in error
 
-    assert "--x.struct.a INT, --all INT, -d INT" in get_helptext(Config)
+    assert "--x.struct.a INT, --all INT, -d INT" in get_helptext_with_checks(Config)
 
 
 def test_positional_alias() -> None:
     """Positional arguments with aliases (which will be ignored)."""
 
     @dataclasses.dataclass
     class Struct:
```

### Comparing `tyro-0.8.3/tests/test_dcargs.py` & `tyro-0.8.4/tests/test_dcargs.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.3/tests/test_dict_namedtuple.py` & `tyro-0.8.4/tests/test_dict_namedtuple.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.3/tests/test_errors.py` & `tyro-0.8.4/tests/test_errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,40 +163,57 @@
         track: bool
 
     @dataclasses.dataclass
     class Class:
         reward: RewardConfig
 
     target = io.StringIO()
-    with pytest.raises(SystemExit), contextlib.redirect_stdout(target):
+    with pytest.raises(SystemExit), contextlib.redirect_stderr(target):
         tyro.cli(Class, args="--reward.trac".split(" "))
 
     error = target.getvalue()
     assert "Unrecognized option" in error
     assert "Perhaps you meant:" in error
 
     assert error.count("--reward.track") == 1
     assert error.count("--help") == 1
 
 
+def test_suppress_console_outputs() -> None:
+    @dataclasses.dataclass
+    class RewardConfig:
+        track: bool
+
+    @dataclasses.dataclass
+    class Class:
+        reward: RewardConfig
+
+    target = io.StringIO()
+    with pytest.raises(SystemExit), contextlib.redirect_stderr(target):
+        tyro.cli(Class, args="--reward.trac".split(" "), console_outputs=False)
+
+    error = target.getvalue()
+    assert error == ""
+
+
 def test_similar_arguments_subcommands() -> None:
     @dataclasses.dataclass
     class RewardConfig:
         track: bool
 
     @dataclasses.dataclass
     class ClassA:
         reward: RewardConfig
 
     @dataclasses.dataclass
     class ClassB:
         reward: RewardConfig
 
     target = io.StringIO()
-    with pytest.raises(SystemExit), contextlib.redirect_stdout(target):
+    with pytest.raises(SystemExit), contextlib.redirect_stderr(target):
         tyro.cli(Union[ClassA, ClassB], args="--reward.trac".split(" "))  # type: ignore
 
     error = target.getvalue()
     assert "Unrecognized option" in error
     assert "Perhaps you meant:" in error
     assert error.count("--reward.track") == 1
     assert error.count("--help") == 3
@@ -213,15 +230,15 @@
         reward: RewardConfig
 
     @dataclasses.dataclass
     class ClassB:
         reward: RewardConfig
 
     target = io.StringIO()
-    with pytest.raises(SystemExit), contextlib.redirect_stdout(target):
+    with pytest.raises(SystemExit), contextlib.redirect_stderr(target):
         tyro.cli(Union[ClassA, ClassB], args="--fjdkslaj --reward.trac".split(" "))  # type: ignore
 
     error = target.getvalue()
     assert "Unrecognized option" in error
     assert "Arguments similar to --reward.trac" in error
     assert error.count("--reward.track {True,False}") == 1
     assert error.count("--reward.trace INT") == 1
@@ -239,15 +256,15 @@
         reward: RewardConfig
 
     @dataclasses.dataclass
     class ClassB:
         reward: RewardConfig
 
     target = io.StringIO()
-    with pytest.raises(SystemExit), contextlib.redirect_stdout(target):
+    with pytest.raises(SystemExit), contextlib.redirect_stderr(target):
         tyro.cli(Union[ClassA, ClassB], args="--rd.trac".split(" "))  # type: ignore
 
     error = target.getvalue()
     assert "Unrecognized option" in error
     assert "Perhaps you meant:" in error
     assert error.count("--reward.track {True,False}") == 1
     assert error.count("--reward.trace INT") == 1
@@ -265,15 +282,15 @@
         reward: RewardConfig
 
     @dataclasses.dataclass
     class ClassB:
         reward: RewardConfig
 
     target = io.StringIO()
-    with pytest.raises(SystemExit), contextlib.redirect_stdout(target):
+    with pytest.raises(SystemExit), contextlib.redirect_stderr(target):
         tyro.cli(Union[ClassA, ClassB], args="--track".split(" "))  # type: ignore
 
     error = target.getvalue()
     assert "Unrecognized option" in error
     assert "Perhaps you meant:" in error
     assert error.count("--reward.track {True,False}") == 1
     assert (
@@ -307,26 +324,26 @@
         reward: RewardConfig
 
     @dataclasses.dataclass
     class ClassB:
         reward: RewardConfig
 
     target = io.StringIO()
-    with pytest.raises(SystemExit), contextlib.redirect_stdout(target):
+    with pytest.raises(SystemExit), contextlib.redirect_stderr(target):
         tyro.cli(Union[ClassA, ClassB], args="--track".split(" "))  # type: ignore
 
     error = target.getvalue()
     assert "Unrecognized option" in error
     assert "Perhaps you meant:" in error
     assert error.count("--reward.track") == 10
     assert "[...]" not in error
     assert error.count("--help") == 21
 
     target = io.StringIO()
-    with pytest.raises(SystemExit), contextlib.redirect_stdout(target):
+    with pytest.raises(SystemExit), contextlib.redirect_stderr(target):
         # --tracked is intentionally between 0.8 ~ 0.9 similarity to track{i} for test
         # coverage.
         tyro.cli(RewardConfig, args="--tracked".split(" "))  # type: ignore
 
     # Usage print should be clipped.
     error = target.getvalue()
     assert "For full helptext, run" in error
@@ -370,15 +387,15 @@
         reward: RewardConfig
 
     @dataclasses.dataclass
     class ClassI:
         reward: RewardConfig
 
     target = io.StringIO()
-    with pytest.raises(SystemExit), contextlib.redirect_stdout(target):
+    with pytest.raises(SystemExit), contextlib.redirect_stderr(target):
         tyro.cli(  # type: ignore
             Union[
                 ClassA, ClassB, ClassC, ClassD, ClassE, ClassF, ClassG, ClassH, ClassI
             ],
             args="--track".split(" "),
         )
 
@@ -429,15 +446,15 @@
         reward: RewardConfig
 
     @dataclasses.dataclass
     class ClassI:
         reward: RewardConfig
 
     target = io.StringIO()
-    with pytest.raises(SystemExit), contextlib.redirect_stdout(target):
+    with pytest.raises(SystemExit), contextlib.redirect_stderr(target):
         tyro.cli(  # type: ignore
             Union[
                 ClassA, ClassB, ClassC, ClassD, ClassE, ClassF, ClassG, ClassH, ClassI
             ],
             args="--track --ffff".split(" "),
         )
 
@@ -452,15 +469,15 @@
 
 def test_similar_flag() -> None:
     @dataclasses.dataclass
     class Args:
         flag: bool = False
 
     target = io.StringIO()
-    with pytest.raises(SystemExit), contextlib.redirect_stdout(target):
+    with pytest.raises(SystemExit), contextlib.redirect_stderr(target):
         tyro.cli(
             Args,
             args="--lag".split(" "),
         )
 
     error = target.getvalue()
```

### Comparing `tyro-0.8.3/tests/test_flax_min_py38.py` & `tyro-0.8.4/tests/test_flax_min_py38.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Tests initializing flax modules directly via tyro."""
 
 from typing import cast
 
 import jax
 import pytest
 from flax import linen as nn
-from helptext_utils import get_helptext
+from helptext_utils import get_helptext_with_checks
 from jax import numpy as jnp
 
 import tyro
 
 
 class Classifier(nn.Module):
     layers: int
@@ -46,15 +46,15 @@
         ],
     )
 
     x = jnp.zeros((10, 4))
     params = network.init(jax.random.PRNGKey(0), x)
     assert cast(jax.Array, network.apply(params, x)).shape == (10, 3)
 
-    helptext = get_helptext(Classifier)
+    helptext = get_helptext_with_checks(Classifier)
     assert "parent" not in helptext
     assert "name" not in helptext
 
 
 def test_missing():
     with pytest.raises(SystemExit):
         tyro.cli(
```

### Comparing `tyro-0.8.3/tests/test_forward_ref.py` & `tyro-0.8.4/tests/test_forward_ref.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.3/tests/test_functools.py` & `tyro-0.8.4/tests/test_functools.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import dataclasses
 import functools
 
 import pytest
-from helptext_utils import get_helptext
+from helptext_utils import get_helptext_with_checks
 
 import tyro
 
 
 def test_partial_func() -> None:
     def main(a: int, b: str) -> str:
         return b * a
@@ -25,28 +25,28 @@
 
 
 def test_partial_helptext_func() -> None:
     def main(a: int, b: str) -> str:
         """Hello!"""
         return b * a
 
-    helptext = get_helptext(functools.partial(main, b="hello world"))
+    helptext = get_helptext_with_checks(functools.partial(main, b="hello world"))
     assert "partial" not in helptext
     assert "Hello!" in helptext
     assert "hello world" in helptext
 
 
 def test_partial_helptext_class() -> None:
     class Main:
         """Hello!"""
 
         def __init__(self, a: int, b: str) -> None:
             self.inner = b * a
 
-    helptext = get_helptext(functools.partial(Main, b="3"))
+    helptext = get_helptext_with_checks(functools.partial(Main, b="3"))
     assert "partial" not in helptext
     assert "Hello!" in helptext
 
 
 def test_wraps_func() -> None:
     def main(a: int, b: str) -> str:
         return b * a
@@ -72,15 +72,15 @@
 
     @functools.wraps(main)
     def wrapper(*args, **kwargs) -> int:
         return kwargs["a"]
 
     assert tyro.cli(functools.partial(wrapper, a=3), args=["--b", "hi"]) == 3
 
-    helptext = get_helptext(functools.partial(wrapper, b="3"))
+    helptext = get_helptext_with_checks(functools.partial(wrapper, b="3"))
     assert "wraps" not in helptext
     assert "Hello!" in helptext
     assert "Argument." in helptext
 
 
 def test_wraps_partial_class_helptext() -> None:
     class Main:
@@ -91,15 +91,15 @@
 
     @functools.wraps(Main)
     def wrapper(*args, **kwargs) -> int:
         return kwargs["a"]
 
     assert tyro.cli(functools.partial(wrapper, a=3), args=["--b", "hi"]) == 3
 
-    helptext = get_helptext(functools.partial(wrapper, b="3"))
+    helptext = get_helptext_with_checks(functools.partial(wrapper, b="3"))
     assert "wraps" not in helptext
     assert "Hello!" in helptext
 
 
 @dataclasses.dataclass
 class WrappedDataclass:
     """Hello!"""
@@ -123,11 +123,11 @@
         == "hihihi"
     )
     assert (
         tyro.cli(functools.partial(functools.partial(wrapper, a=3), b="hello"), args=[])
         == "hellohellohello"
     )
 
-    helptext = get_helptext(functools.partial(wrapper, b="3"))
+    helptext = get_helptext_with_checks(functools.partial(wrapper, b="3"))
     assert "wraps" not in helptext
     assert "Hello!" in helptext
     assert "Second field." in helptext
```

### Comparing `tyro-0.8.3/tests/test_generics_and_serialization.py` & `tyro-0.8.4/tests/test_generics_and_serialization.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.3/tests/test_helptext.py` & `tyro-0.8.4/tests/test_helptext.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import enum
 import json
 import os
 import pathlib
 from collections.abc import Callable
 from typing import Any, Dict, Generic, List, Optional, Tuple, TypeVar, Union, cast
 
-from helptext_utils import get_helptext
+from helptext_utils import get_helptext_with_checks
 from torch import nn
 from typing_extensions import Annotated, Literal, NotRequired, TypedDict
 
 import tyro
 
 
 def test_helptext() -> None:
@@ -22,15 +22,15 @@
 
         # Documentation 2
         y: Annotated[int, "ignored"]
 
         z: int = 3
         """Documentation 3"""
 
-    helptext = get_helptext(Helptext)
+    helptext = get_helptext_with_checks(Helptext)
     assert cast(str, helptext) in helptext
     assert "x INT" in helptext
     assert "y INT" in helptext
     assert "z INT" in helptext
     assert "Documentation 1 (required)" in helptext
     assert "Documentation 2 (required)" in helptext
     assert "Documentation 3 (default: 3)" in helptext
@@ -43,15 +43,15 @@
 
         x: int  #: Documentation 1
 
         #:Documentation 2
         y: Annotated[int, "ignored"]
         z: int = 3
 
-    helptext = get_helptext(Helptext)
+    helptext = get_helptext_with_checks(Helptext)
     assert cast(str, helptext) in helptext
     assert "x INT" in helptext
     assert "y INT" in helptext
     assert "z INT" in helptext
     assert "Documentation 1 (required)" in helptext
     assert ": Documentation 1" not in helptext
     assert "Documentation 2 (required)" in helptext
@@ -72,15 +72,15 @@
             z: Documentation 3
         """
 
         x: int
         y: Annotated[int, "ignored"]
         z: int = 3
 
-    helptext = get_helptext(Helptext2)
+    helptext = get_helptext_with_checks(Helptext2)
     assert "This docstring should be printed as a description" in helptext
     assert "Attributes" not in helptext
     assert "x INT" in helptext
     assert "y INT" in helptext
     assert "z INT" in helptext
     assert "Documentation 1 (required)" in helptext
     assert "Documentation 2 (required)" in helptext
@@ -98,15 +98,15 @@
             z: Documentation 3
         """
 
         x: int
         y: Annotated[int, "ignored"]
         z: int = 3
 
-    helptext = get_helptext(Helptext3)
+    helptext = get_helptext_with_checks(Helptext3)
     assert "This docstring should be printed as a description" in helptext
     assert "Args" not in helptext
     assert "x INT" in helptext
     assert "y INT" in helptext
     assert "z INT" in helptext
     assert "Documentation 1 (required)" in helptext
     assert "Documentation 2 (required)" in helptext
@@ -133,15 +133,15 @@
             """Coverage stress test."""
         # fmt: on
 
     @dataclasses.dataclass
     class ChildClass(UnrelatedParentClass, ActualParentClass):
         pass
 
-    helptext = get_helptext(ChildClass)
+    helptext = get_helptext_with_checks(ChildClass)
     assert "Documentation 1" in helptext
     assert "Documentation 2" in helptext
 
 
 def test_helptext_inherited_default_override() -> None:
     @dataclasses.dataclass
     class ParentClass:
@@ -163,15 +163,15 @@
     class ChildClass(ParentClass):
         """This docstring should be printed as a description."""
 
     def main(x: ParentClass = ChildClass(x=5, y=5)) -> Any:
         """Main function."""
         return x
 
-    helptext = get_helptext(main)
+    helptext = get_helptext_with_checks(main)
     assert "Main function." in helptext
     assert "Documentation 1" in helptext
     assert "Documentation 2" in helptext
     assert "__not__" not in helptext
     assert helptext.count("should be printed") == 1
 
 
@@ -193,22 +193,22 @@
         Args:
             a: Documented in function.
         """
 
     def main_no_docstring(a: Inner) -> None:
         """main_no_docstring."""
 
-    helptext = get_helptext(main_with_docstring)
+    helptext = get_helptext_with_checks(main_with_docstring)
     assert "Documented in function" in helptext and str(Inner.__doc__) not in helptext
     assert "main_with_docstring." in helptext
     assert "Args:" not in helptext
     assert "Args:" not in helptext
     assert "Hello world!" in helptext
 
-    helptext = get_helptext(main_no_docstring)
+    helptext = get_helptext_with_checks(main_no_docstring)
     assert "Something" in helptext
     assert "main_no_docstring." in helptext
     assert "Args:" not in helptext
     assert "Hello world!" in helptext
 
 
 def test_helptext_defaults() -> None:
@@ -219,15 +219,15 @@
 
     @dataclasses.dataclass
     class HelptextWithVariousDefaults:
         x: pathlib.Path = pathlib.Path("/some/path/to/a/file")
         y: Color = Color.RED
         z: str = "%"
 
-    helptext = get_helptext(HelptextWithVariousDefaults)
+    helptext = get_helptext_with_checks(HelptextWithVariousDefaults)
     assert "show this help message and exit" in helptext
     assert "--x PATH" in helptext
     assert "(default: /some/path/to/a/file)" in helptext
     assert "--y {RED,GREEN,BLUE}" in helptext
     assert "(default: RED)" in helptext
     assert "--z STR" in helptext
     assert "(default: %)" in helptext
@@ -244,15 +244,15 @@
         # Next line of documentation 2
         y: int
 
         z: int = 3
         """Documentation 3
         Next line of documentation 3"""
 
-    helptext = get_helptext(HelptextMultiline)
+    helptext = get_helptext_with_checks(HelptextMultiline)
     assert "Documentation 1 (required)" in helptext
     assert "Documentation 2" in helptext
     assert "documentation 2" in helptext
     assert "Documentation 3" in helptext
     assert "documentation 3" in helptext
 
 
@@ -260,27 +260,27 @@
     @dataclasses.dataclass
     class HelptextGrouped:
         x: int  # Documentation 1
         # Description of both y and z.
         y: int
         z: int = 3
 
-    helptext = get_helptext(HelptextGrouped)
+    helptext = get_helptext_with_checks(HelptextGrouped)
     assert "Documentation 1 (required)" in helptext
     assert "Description of both y and z. (required)" in helptext
     assert "Description of both y and z. (default: 3)" in helptext
 
 
 def test_none_default_value_helptext() -> None:
     @dataclasses.dataclass
     class Config:
         x: Optional[int] = None
         """An optional variable."""
 
-    helptext = get_helptext(Config)
+    helptext = get_helptext_with_checks(Config)
     assert "--x {None}|INT" in helptext
     assert "An optional variable. (default: None)" in helptext
 
 
 def test_helptext_hard_bool() -> None:
     @dataclasses.dataclass
     class HelptextHardString:
@@ -290,15 +290,15 @@
         )
         """Helptext. 2% milk."""
         # fmt: on
 
     # Note that the percent symbol needs some extra handling in argparse.
     # https://stackoverflow.com/questions/21168120/python-argparse-errors-with-in-help-string
 
-    helptext = get_helptext(HelptextHardString)
+    helptext = get_helptext_with_checks(HelptextHardString)
     assert "--x" in helptext
     assert "2% milk." in helptext
 
 
 def test_helptext_with_inheritance() -> None:
     @dataclasses.dataclass
     class Parent:
@@ -309,15 +309,15 @@
         """Helptext."""
         # fmt: on
 
     @dataclasses.dataclass
     class Child(Parent):
         pass
 
-    helptext = get_helptext(Child)
+    helptext = get_helptext_with_checks(Child)
     assert "--x STR" in helptext
     assert "Helptext." in helptext
     assert "(default: 'This docstring" in helptext
 
 
 def test_helptext_with_inheritance_overriden() -> None:
     @dataclasses.dataclass
@@ -334,89 +334,89 @@
         # fmt: off
         x: str = (
             "This docstring may be tougher to parse?"
         )
         """Helptext!"""
         # fmt: on
 
-    helptext = get_helptext(Child2)
+    helptext = get_helptext_with_checks(Child2)
     assert "--x STR" in helptext
     assert "Helptext! (default: 'This" in helptext
 
 
 def test_tuple_helptext() -> None:
     @dataclasses.dataclass
     class TupleHelptext:
         x: Tuple[int, str, float]
 
-    helptext = get_helptext(TupleHelptext)
+    helptext = get_helptext_with_checks(TupleHelptext)
     assert "--x INT STR FLOAT" in helptext
 
 
 def test_tuple_helptext_defaults() -> None:
     @dataclasses.dataclass
     class TupleHelptextDefaults:
         x: Tuple[int, str, str] = (5, "hello world", "hello")
 
-    helptext = get_helptext(TupleHelptextDefaults)
+    helptext = get_helptext_with_checks(TupleHelptextDefaults)
     assert "--x INT STR STR" in helptext
     assert "(default: 5 'hello world' hello)" in helptext
 
 
 def test_generic_helptext() -> None:
     T = TypeVar("T")
 
     @dataclasses.dataclass
     class GenericTupleHelptext(Generic[T]):
         x: T
 
-    helptext = get_helptext(GenericTupleHelptext[int])
+    helptext = get_helptext_with_checks(GenericTupleHelptext[int])
     assert "--x INT" in helptext
 
 
 def test_generic_tuple_helptext() -> None:
     T = TypeVar("T")
 
     @dataclasses.dataclass
     class GenericTupleHelptext(Generic[T]):
         x: Tuple[T, T, T]
 
-    helptext = get_helptext(GenericTupleHelptext[int])
+    helptext = get_helptext_with_checks(GenericTupleHelptext[int])
     assert "--x INT INT INT" in helptext
 
 
 def test_generic_list_helptext() -> None:
     T = TypeVar("T")
 
     @dataclasses.dataclass
     class GenericTupleHelptext(Generic[T]):
         x: List[T]
 
-    helptext = get_helptext(GenericTupleHelptext[int])
+    helptext = get_helptext_with_checks(GenericTupleHelptext[int])
     assert "--x [INT [INT ...]]" in helptext
 
 
 def test_literal_helptext() -> None:
     @dataclasses.dataclass
     class LiteralHelptext:
         x: Literal[1, 2, 3]
         """A number."""
 
-    helptext = get_helptext(LiteralHelptext)
+    helptext = get_helptext_with_checks(LiteralHelptext)
     assert "--x {1,2,3}" in helptext
     assert "A number. (required)" in helptext
 
 
 def test_optional_literal_helptext() -> None:
     @dataclasses.dataclass
     class OptionalLiteralHelptext:
         x: Optional[Literal[1, 2, 3]] = None
         """A number."""
 
-    helptext = get_helptext(OptionalLiteralHelptext)
+    helptext = get_helptext_with_checks(OptionalLiteralHelptext)
     assert "--x {None,1,2,3}" in helptext
     assert "A number. (default: None)" in helptext
 
 
 def test_multiple_subparsers_helptext() -> None:
     @dataclasses.dataclass
     class Subcommand1:
@@ -441,26 +441,26 @@
         # Field c description.
         c: Union[Subcommand1, Subcommand2, Subcommand3] = dataclasses.field(
             default_factory=Subcommand3
         )
 
         d: bool = False
 
-    helptext = get_helptext(MultipleSubparsers)
+    helptext = get_helptext_with_checks(MultipleSubparsers)
 
     assert "2% milk." in helptext
     assert "Field a description." in helptext
     assert "Field b description." not in helptext
     assert "Field c description." not in helptext
 
     # Not enough args for usage shortening to kick in.
     assert "[OPTIONS]" not in helptext
     assert "[B:SUBCOMMAND2 OPTIONS]" not in helptext
 
-    helptext = get_helptext(
+    helptext = get_helptext_with_checks(
         MultipleSubparsers, args=["a:subcommand1", "b:subcommand1", "--help"]
     )
 
     assert "2% milk." in helptext
     assert "Field a description." not in helptext
     assert "Field b description." not in helptext
     assert "Field c description." in helptext
@@ -512,25 +512,25 @@
 
         d: bool = False
         f: bool = False
         g: bool = False
         h: bool = False
         i: bool = False
 
-    helptext = get_helptext(MultipleSubparsers)
+    helptext = get_helptext_with_checks(MultipleSubparsers)
 
     assert "2% milk." in helptext
     assert "Field a description." in helptext
     assert "Field b description." not in helptext
     assert "Field c description." not in helptext
 
     assert "[OPTIONS]" in helptext
     assert "[B:SUBCOMMAND2 OPTIONS]" not in helptext
 
-    helptext = get_helptext(
+    helptext = get_helptext_with_checks(
         MultipleSubparsers, args=["a:subcommand1", "b:subcommand1", "--help"]
     )
 
     assert "2% milk." in helptext
     assert "Field a description." not in helptext
     assert "Field b description." not in helptext
     assert "Field c description." in helptext
@@ -550,100 +550,100 @@
 
         # Documentation 2
         y: List[Optional[int]]
 
         z: Optional[int] = 3
         """Documentation 3"""
 
-    helptext = get_helptext(OptionalHelptext)
+    helptext = get_helptext_with_checks(OptionalHelptext)
     assert cast(str, cast(str, OptionalHelptext.__doc__)[:20]) in helptext
     assert "2% milk" in helptext
     assert "--x {None}|INT" in helptext
     assert "--y [{None}|INT [{None}|INT ...]]" in helptext
     assert "[--z {None}|INT]" in helptext
 
 
 def test_metavar_0() -> None:
     def main(x: Union[Literal[0, 1, 2, 3], Tuple[int, int]]) -> None:
         pass
 
-    helptext = get_helptext(main)
+    helptext = get_helptext_with_checks(main)
     assert "--x {0,1,2,3}|{INT INT}" in helptext
 
 
 def test_metavar_1() -> None:
     def main(
         x: Union[
             Literal[0, 1, 2, 3],
             Literal["hey,there", "hello"],
             List[int],
         ],
     ) -> None:
         pass
 
     # The comma formatting is unfortunate, but matches argparse's default behavior.
-    helptext = get_helptext(main)
+    helptext = get_helptext_with_checks(main)
     assert "--x {0,1,2,3,hey,there,hello}|{[INT [INT ...]]}" in helptext
 
 
 def test_metavar_2() -> None:
     def main(
         x: Tuple[
             Literal[0, 1, 2, 3],
             Union[int, str],
         ],
     ) -> None:
         pass
 
-    helptext = get_helptext(main)
+    helptext = get_helptext_with_checks(main)
     assert "--x {0,1,2,3} INT|STR" in helptext
 
 
 def test_metavar_3() -> None:
     def main(
         x: Union[
             Literal[0, 1, 2, 3],
             Union[Tuple[int, int], Tuple[str]],
         ],
     ) -> None:
         pass
 
-    helptext = get_helptext(main)
+    helptext = get_helptext_with_checks(main)
     assert "--x {0,1,2,3}|{INT INT}|STR" in helptext
 
 
 def test_metavar_4() -> None:
     def main(
         x: Union[
             Literal[0, 1, 2, 3],
             Union[Tuple[int, int], Tuple[str, str, str]],
             Literal[True],
         ],
     ) -> None:
         pass
 
-    helptext = get_helptext(main)
+    helptext = get_helptext_with_checks(main)
     assert "--x {0,1,2,3}|{INT INT}|{STR STR STR}|{True}" in helptext
 
 
 def test_metavar_5() -> None:
     def main(
         x: List[Union[Tuple[int, int], Tuple[str, str]]] = [(1, 1), (2, 2)],
     ) -> None:
         pass
 
-    helptext = get_helptext(main)
+    helptext = get_helptext_with_checks(main)
     assert "[--x [{INT INT}|{STR STR} [{INT INT}|{STR STR} ...]]]" in helptext
 
 
 def test_metavar_6() -> None:
     def main(x: Dict[Union[Tuple[int, int], Tuple[str, str]], Tuple[int, int]]) -> dict:
         return x
 
-    helptext = get_helptext(main)
+    helptext = get_helptext_with_checks(main)
     assert (
         "--x [{INT INT}|{STR STR} INT INT [{INT INT}|{STR STR} INT INT ...]]"
         in helptext
     )
 
 
 def test_comment_in_subclass_list() -> None:
@@ -653,56 +653,56 @@
         object,
     ):
         a: int
 
         # But this text should!
         b: int
 
-    helptext = get_helptext(Something)
+    helptext = get_helptext_with_checks(Something)
     assert "This text should not" not in helptext
     assert "But this text should!" in helptext
 
 
 def test_unparsable() -> None:
     class Struct:
         a: int = 5
         b: str = "7"
 
     def main(x: Any = Struct()):
         pass
 
-    helptext = get_helptext(main)
+    helptext = get_helptext_with_checks(main)
     assert "--x {fixed}" in helptext
 
     def main2(x: Callable = nn.ReLU):
         pass
 
-    helptext = get_helptext(main2)
+    helptext = get_helptext_with_checks(main2)
     assert "--x {fixed}" in helptext
     assert "(fixed to:" in helptext
     assert "torch" in helptext
 
 
 def test_pathlike() -> None:
     def main(x: os.PathLike) -> None:
         pass
 
-    helptext = get_helptext(main)
+    helptext = get_helptext_with_checks(main)
     assert "--x PATH " in helptext
 
 
 def test_nested_bool() -> None:
     @dataclasses.dataclass
     class Child:
         x: bool = False
 
     def main(child: Child) -> None:
         pass
 
-    helptext = get_helptext(main)
+    helptext = get_helptext_with_checks(main)
     assert "--child.x | --child.no-x" in helptext
 
 
 def test_multiple_subparsers_helptext_hyphens() -> None:
     @dataclasses.dataclass
     class SubcommandOne:
         """2% milk."""  # % symbol is prone to bugs in argparse.
@@ -725,22 +725,22 @@
         # Field b description.
         b: Union[SubcommandOne, SubcommandTwo, SubcommandThree]
         # Field c description.
         c: Union[SubcommandOne, SubcommandTwo, SubcommandThree] = dataclasses.field(
             default_factory=SubcommandThree
         )
 
-    helptext = get_helptext(MultipleSubparsers)
+    helptext = get_helptext_with_checks(MultipleSubparsers)
 
     assert "2% milk." in helptext
     assert "Field a description." in helptext
     assert "Field b description." not in helptext
     assert "Field c description." not in helptext
 
-    helptext = get_helptext(
+    helptext = get_helptext_with_checks(
         MultipleSubparsers, args=["a:subcommand-one", "b:subcommand-one", "--help"]
     )
 
     assert "2% milk." in helptext
     assert "Field a description." not in helptext
     assert "Field b description." not in helptext
     assert "Field c description." in helptext
@@ -773,22 +773,22 @@
         # Field b description.
         b: Union[SubcommandOne, SubcommandTwo, SubcommandThree]
         # Field c description.
         c: Union[SubcommandOne, SubcommandTwo, SubcommandThree] = dataclasses.field(
             default_factory=SubcommandThree
         )
 
-    helptext = get_helptext(MultipleSubparsers, use_underscores=True)
+    helptext = get_helptext_with_checks(MultipleSubparsers, use_underscores=True)
 
     assert "2% milk." in helptext
     assert "Field a description." in helptext
     assert "Field b description." not in helptext
     assert "Field c description." not in helptext
 
-    helptext = get_helptext(
+    helptext = get_helptext_with_checks(
         MultipleSubparsers,
         args=["a:subcommand_one", "b:subcommand_one", "--help"],
         use_underscores=True,
     )
 
     assert "2% milk." in helptext
     assert "Field a description." not in helptext
@@ -809,15 +809,15 @@
 
     @dataclasses.dataclass
     class CheckoutCompletion:
         """Help message."""
 
         y: int
 
-    help = get_helptext(Union[A, CheckoutCompletion])  # type: ignore
+    help = get_helptext_with_checks(Union[A, CheckoutCompletion])  # type: ignore
     assert help.count("checkout-completion") == 3
 
 
 def test_subparsers_wrapping1() -> None:
     @dataclasses.dataclass
     class A:
         """Help message."""
@@ -826,15 +826,15 @@
 
     @dataclasses.dataclass
     class CheckoutCompletio:
         """Help message."""
 
         y: int
 
-    help = get_helptext(Union[A, CheckoutCompletio])  # type: ignore
+    help = get_helptext_with_checks(Union[A, CheckoutCompletio])  # type: ignore
     assert help.count("checkout-completio") == 3
 
 
 def test_subparsers_wrapping2() -> None:
     @dataclasses.dataclass
     class A:
         """Help message."""
@@ -843,15 +843,15 @@
 
     @dataclasses.dataclass
     class CheckoutCompletionn:
         """Help message."""
 
         y: int
 
-    help = get_helptext(Union[A, CheckoutCompletionn])  # type: ignore
+    help = get_helptext_with_checks(Union[A, CheckoutCompletionn])  # type: ignore
     assert help.count("checkout-completionn") == 3
 
 
 def test_subparsers_wrapping3() -> None:
     @dataclasses.dataclass
     class A:
         """Help message."""
@@ -860,41 +860,41 @@
 
     @dataclasses.dataclass
     class CmdCheckout012:
         """Help message."""
 
         y: int
 
-    help = get_helptext(Union[A, CmdCheckout012])  # type: ignore
+    help = get_helptext_with_checks(Union[A, CmdCheckout012])  # type: ignore
     assert help.count("cmd-checkout012") == 3
 
 
 def test_tuple_default() -> None:
     @dataclasses.dataclass
     class A:
         """Help message."""
 
         x: Tuple[str, str] = ("hello", "world")
 
-    help = get_helptext(A)
+    help = get_helptext_with_checks(A)
     assert "STR STR" in help
     assert "hello world" in help
     assert "('hello', 'world')" not in help
 
 
 def test_argconf_constructor() -> None:
     @dataclasses.dataclass
     class A:
         """Help message."""
 
         x: Annotated[
             Tuple[str, str], tyro.conf.arg(constructor=lambda x: ("a", "b"))
         ] = ("hello", "world")
 
-    help = get_helptext(A)
+    help = get_helptext_with_checks(A)
     assert "STR STR" not in help
     # Unlike case above, should not be converted to 'hello world'.
     assert "('hello', 'world')" in help  # JSON special case.
 
 
 def test_argconf_constructor_json_special_case() -> None:
     @dataclasses.dataclass
@@ -904,15 +904,15 @@
         x: Annotated[
             Tuple[str, str], tyro.conf.arg(constructor=json.loads, metavar="JSON")
         ] = ("hello", "world")
         y: Annotated[
             Tuple[int, int], tyro.conf.arg(constructor=json.loads, metavar="JSON")
         ] = (3, 5)
 
-    help = get_helptext(A)
+    help = get_helptext_with_checks(A)
     assert "STR STR" not in help
     assert "JSON" in help
     assert '["hello", "world"]' in help  # JSON special case.
     assert "[3, 5]" in help, help  # JSON special case.
 
 
 def test_optional_group() -> None:
@@ -921,54 +921,54 @@
             Tuple[str, str], tyro.conf.arg(constructor=json.loads, metavar="JSON")
         ] = ("hello", "world"),
         y: int = 3,
     ) -> int:
         del x, y
         return 5
 
-    help = get_helptext(f, default=3)
+    help = get_helptext_with_checks(f, default=3)
     assert 'default if used: ["hello", "world"]' in help
     assert "default if used: 3" in help
 
 
 def test_append_fixed() -> None:
     def f(
         x: tyro.conf.UseAppendAction[Tuple[str, str]],
         y: int = 3,
     ) -> int:
         del x, y
         return 5
 
-    help = get_helptext(f)
+    help = get_helptext_with_checks(f)
     assert "repeatable" not in help, help
 
 
 def test_append_good() -> None:
     def f(
         x: tyro.conf.UseAppendAction[Tuple[str, ...]],
         y: int = 3,
     ) -> int:
         del x, y
         return 5
 
-    help = get_helptext(f)
+    help = get_helptext_with_checks(f)
     assert "repeatable" in help, help
 
 
 def test_append_with_default() -> None:
     def f(
         x: tyro.conf.UseAppendAction[Tuple[str, ...]] = ("hello world", "hello"),
         y: int = 3,
     ) -> int:
         del x, y
         return 5
 
-    help = get_helptext(f)
+    help = get_helptext_with_checks(f)
     assert "repeatable, appends to: 'hello world' hello" in help, help
 
 
 def test_typeddict_exclude() -> None:
     class Special(TypedDict):
         x: NotRequired[int]
 
-    help = get_helptext(Special)
+    help = get_helptext_with_checks(Special)
     assert "unset by default" in help, help
```

### Comparing `tyro-0.8.3/tests/test_initvar_min_py38.py` & `tyro-0.8.4/tests/test_initvar_min_py38.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.3/tests/test_is_nested_type.py` & `tyro-0.8.4/tests/test_is_nested_type.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.3/tests/test_missing.py` & `tyro-0.8.4/tests/test_missing.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 def test_missing() -> None:
     def main(a: int = 5, b: int = tyro.MISSING, c: int = 3) -> Tuple[int, int, int]:
         return a, b, c
 
     target = io.StringIO()
-    with pytest.raises(SystemExit), contextlib.redirect_stdout(target):
+    with pytest.raises(SystemExit), contextlib.redirect_stderr(target):
         tyro.cli(main, args=[])
     message = target.getvalue()
     assert "Required options" in message
     assert "Argument helptext" in message
     assert "--a INT" not in message
     assert "--b INT" in message
     assert "(required)" in message
```

### Comparing `tyro-0.8.3/tests/test_missing_optional_packages.py` & `tyro-0.8.4/tests/test_missing_optional_packages.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.3/tests/test_mixed_unions.py` & `tyro-0.8.4/tests/test_mixed_unions.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.3/tests/test_nested.py` & `tyro-0.8.4/tests/test_nested.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import dataclasses
 from typing import Any, Generic, Mapping, NewType, Optional, Tuple, TypeVar, Union
 
 import pytest
 from frozendict import frozendict  # type: ignore
-from helptext_utils import get_helptext
+from helptext_utils import get_helptext_with_checks
 from typing_extensions import Annotated, Literal
 
 import tyro
 
 
 def test_nested() -> None:
     @dataclasses.dataclass
@@ -1157,8 +1157,8 @@
     @dataclasses.dataclass
     class Args:
         inner: Union[
             Annotated[A, tyro.conf.subcommand(name="alt", default=A(5))], A
         ] = A("hello")
 
     assert tyro.cli(Args, args=[]) == Args(A("hello"))
-    assert "default: inner:alt" in get_helptext(Args)
+    assert "default: inner:alt" in get_helptext_with_checks(Args)
```

### Comparing `tyro-0.8.3/tests/test_nested_in_containers.py` & `tyro-0.8.4/tests/test_nested_in_containers.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.3/tests/test_new_style_annotations_min_py310.py` & `tyro-0.8.4/tests/test_new_style_annotations_min_py310.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.3/tests/test_new_style_annotations_min_py312.py` & `tyro-0.8.4/tests/test_new_style_annotations_min_py312.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.3/tests/test_new_style_annotations_min_py39.py` & `tyro-0.8.4/tests/test_new_style_annotations_min_py39.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.3/tests/test_partial.py` & `tyro-0.8.4/tests/test_partial.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import dataclasses
 import functools
 
-from helptext_utils import get_helptext
+from helptext_utils import get_helptext_with_checks
 
 import tyro
 
 
 def test_partial_func() -> None:
     def main(a: int, b: str) -> str:
         return b * a
@@ -24,27 +24,27 @@
 
 
 def test_partial_helptext_func() -> None:
     def main(a: int, b: str) -> str:
         """Hello!"""
         return b * a
 
-    helptext = get_helptext(functools.partial(main, b="3"))
+    helptext = get_helptext_with_checks(functools.partial(main, b="3"))
     assert "partial" not in helptext
     assert "Hello!" in helptext
 
 
 def test_partial_helptext_class() -> None:
     class Main:
         """Hello!"""
 
         def __init__(self, a: int, b: str) -> None:
             self.inner = b * a
 
-    helptext = get_helptext(functools.partial(Main, b="3"))
+    helptext = get_helptext_with_checks(functools.partial(Main, b="3"))
     assert "partial" not in helptext
     assert "Hello!" in helptext
 
 
 def test_partial_helptext_dataclass() -> None:
     @dataclasses.dataclass
     class Config:
@@ -52,10 +52,10 @@
         b: int
         """Hello!"""
         c: int
 
     ConfigWithDefaults = functools.partial(functools.partial(Config, a=3), c=5)
     assert tyro.cli(ConfigWithDefaults, args=["--b", "4"]) == Config(3, 4, 5)
 
-    helptext = get_helptext(ConfigWithDefaults)
+    helptext = get_helptext_with_checks(ConfigWithDefaults)
     assert "partial" not in helptext
     assert "Hello!" in helptext
```

### Comparing `tyro-0.8.3/tests/test_positional_min_py38.py` & `tyro-0.8.4/tests/test_positional_min_py38.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.3/tests/test_pydantic.py` & `tyro-0.8.4/tests/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.3/tests/test_pydantic_with_newtype.py` & `tyro-0.8.4/tests/test_pydantic_with_newtype.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.3/tests/test_self_type.py` & `tyro-0.8.4/tests/test_self_type.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.3/tests/test_strings.py` & `tyro-0.8.4/tests/test_strings.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.3/tests/test_tuple_with_subcommands.py` & `tyro-0.8.4/tests/test_tuple_with_subcommands.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.3/tests/test_union_from_mapping.py` & `tyro-0.8.4/tests/test_union_from_mapping.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.3/tests/test_unsupported_but_should_work.py` & `tyro-0.8.4/tests/test_unsupported_but_should_work.py`

 * *Files identical despite different names*

