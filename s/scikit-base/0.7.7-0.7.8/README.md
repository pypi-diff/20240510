# Comparing `tmp/scikit_base-0.7.7.tar.gz` & `tmp/scikit_base-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit_base-0.7.7.tar", last modified: Wed Apr 17 07:54:23 2024, max compression
+gzip compressed data, was "scikit_base-0.7.8.tar", last modified: Fri May 10 00:43:19 2024, max compression
```

## Comparing `scikit_base-0.7.7.tar` & `scikit_base-0.7.8.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:54:23.743414 scikit_base-0.7.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-17 07:54:16.000000 scikit_base-0.7.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8774 2024-04-17 07:54:23.743414 scikit_base-0.7.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-04-17 07:54:16.000000 scikit_base-0.7.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:54:23.727414 scikit_base-0.7.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:54:23.731413 scikit_base-0.7.7/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-04-17 07:54:16.000000 scikit_base-0.7.7/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-17 07:54:16.000000 scikit_base-0.7.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:54:23.743414 scikit_base-0.7.7/scikit_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8774 2024-04-17 07:54:23.000000 scikit_base-0.7.7/scikit_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-17 07:54:23.000000 scikit_base-0.7.7/scikit_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 07:54:23.000000 scikit_base-0.7.7/scikit_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-17 07:54:23.000000 scikit_base-0.7.7/scikit_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-17 07:54:23.000000 scikit_base-0.7.7/scikit_base.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 07:54:20.000000 scikit_base-0.7.7/scikit_base.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-17 07:54:23.743414 scikit_base-0.7.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:54:23.735413 scikit_base-0.7.7/skbase/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/_nopytest_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:54:23.735413 scikit_base-0.7.7/skbase/base/
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    53490 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/base/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    38815 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/base/_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:54:23.735413 scikit_base-0.7.7/skbase/base/_pretty_printing/
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/base/_pretty_printing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11677 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/base/_pretty_printing/_object_html_repr.py
--rw-r--r--   0 runner    (1001) docker     (127)    15634 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/base/_pretty_printing/_pprint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:54:23.735413 scikit_base-0.7.7/skbase/base/_pretty_printing/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/base/_pretty_printing/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/base/_pretty_printing/tests/test_pprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/base/_tagmanager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:54:23.735413 scikit_base-0.7.7/skbase/lookup/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/lookup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39864 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/lookup/_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:54:23.735413 scikit_base-0.7.7/skbase/lookup/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/lookup/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38218 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/lookup/tests/test_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:54:23.735413 scikit_base-0.7.7/skbase/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36166 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/testing/test_all_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:54:23.735413 scikit_base-0.7.7/skbase/testing/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/testing/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9890 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/testing/utils/_conditional_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/testing/utils/inspect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:54:23.735413 scikit_base-0.7.7/skbase/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9297 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:54:23.739414 scikit_base-0.7.7/skbase/tests/mock_package/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/tests/mock_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/tests/mock_package/test_mock_package.py
--rw-r--r--   0 runner    (1001) docker     (127)    50648 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4731 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/tests/test_baseestimator.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/tests/test_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:54:23.739414 scikit_base-0.7.7/skbase/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/utils/_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     7653 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/utils/_iter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/utils/_nested_iter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/utils/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:54:23.739414 scikit_base-0.7.7/skbase/utils/deep_equals/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/utils/deep_equals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/utils/deep_equals/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    18331 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/utils/deep_equals/_deep_equals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:54:23.739414 scikit_base-0.7.7/skbase/utils/dependencies/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/utils/dependencies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14502 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/utils/dependencies/_dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:54:23.739414 scikit_base-0.7.7/skbase/utils/dependencies/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/utils/dependencies/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/utils/dependencies/tests/test_check_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/utils/random_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:54:23.739414 scikit_base-0.7.7/skbase/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/utils/tests/test_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/utils/tests/test_deep_equals.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/utils/tests/test_iter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/utils/tests/test_nested_iter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/utils/tests/test_random_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/utils/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:54:23.739414 scikit_base-0.7.7/skbase/validate/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12957 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/validate/_named_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)    12121 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/validate/_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:54:23.739414 scikit_base-0.7.7/skbase/validate/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/validate/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/validate/tests/test_iterable_named_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)    14131 2024-04-17 07:54:16.000000 scikit_base-0.7.7/skbase/validate/tests/test_type_validations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:43:19.117724 scikit_base-0.7.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-10 00:43:13.000000 scikit_base-0.7.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8774 2024-05-10 00:43:19.117724 scikit_base-0.7.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-05-10 00:43:13.000000 scikit_base-0.7.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:43:19.101724 scikit_base-0.7.8/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:43:19.105724 scikit_base-0.7.8/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-05-10 00:43:13.000000 scikit_base-0.7.8/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-05-10 00:43:13.000000 scikit_base-0.7.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:43:19.113724 scikit_base-0.7.8/scikit_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8774 2024-05-10 00:43:19.000000 scikit_base-0.7.8/scikit_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-10 00:43:19.000000 scikit_base-0.7.8/scikit_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 00:43:19.000000 scikit_base-0.7.8/scikit_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-10 00:43:19.000000 scikit_base-0.7.8/scikit_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-10 00:43:19.000000 scikit_base-0.7.8/scikit_base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 00:43:16.000000 scikit_base-0.7.8/scikit_base.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-10 00:43:19.117724 scikit_base-0.7.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:43:19.105724 scikit_base-0.7.8/skbase/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/_nopytest_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:43:19.105724 scikit_base-0.7.8/skbase/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53490 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/base/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38815 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/base/_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:43:19.105724 scikit_base-0.7.8/skbase/base/_pretty_printing/
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/base/_pretty_printing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11677 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/base/_pretty_printing/_object_html_repr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15634 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/base/_pretty_printing/_pprint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:43:19.109724 scikit_base-0.7.8/skbase/base/_pretty_printing/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/base/_pretty_printing/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/base/_pretty_printing/tests/test_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/base/_tagmanager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:43:19.109724 scikit_base-0.7.8/skbase/lookup/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/lookup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39864 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/lookup/_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:43:19.109724 scikit_base-0.7.8/skbase/lookup/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/lookup/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38218 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/lookup/tests/test_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:43:19.109724 scikit_base-0.7.8/skbase/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36166 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/testing/test_all_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:43:19.109724 scikit_base-0.7.8/skbase/testing/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/testing/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9890 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/testing/utils/_conditional_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/testing/utils/inspect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:43:19.109724 scikit_base-0.7.8/skbase/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:43:19.109724 scikit_base-0.7.8/skbase/tests/mock_package/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/tests/mock_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/tests/mock_package/test_mock_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50648 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4731 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/tests/test_baseestimator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/tests/test_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:43:19.109724 scikit_base-0.7.8/skbase/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/utils/_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7653 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/utils/_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/utils/_nested_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/utils/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:43:19.113724 scikit_base-0.7.8/skbase/utils/deep_equals/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/utils/deep_equals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/utils/deep_equals/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19151 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/utils/deep_equals/_deep_equals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:43:19.113724 scikit_base-0.7.8/skbase/utils/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/utils/dependencies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14502 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/utils/dependencies/_dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:43:19.113724 scikit_base-0.7.8/skbase/utils/dependencies/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/utils/dependencies/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/utils/dependencies/tests/test_check_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/utils/random_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:43:19.113724 scikit_base-0.7.8/skbase/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/utils/tests/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/utils/tests/test_deep_equals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/utils/tests/test_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/utils/tests/test_nested_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/utils/tests/test_random_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/utils/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:43:19.113724 scikit_base-0.7.8/skbase/validate/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12957 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/validate/_named_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12121 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/validate/_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:43:19.113724 scikit_base-0.7.8/skbase/validate/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/validate/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/validate/tests/test_iterable_named_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14131 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/validate/tests/test_type_validations.py
```

### Comparing `scikit_base-0.7.7/LICENSE` & `scikit_base-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.7/PKG-INFO` & `scikit_base-0.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-base
-Version: 0.7.7
+Version: 0.7.8
 Summary: Base classes for sklearn-like parametric objects
 Author-email: sktime developers <sktime.toolbox@gmail.com>
 Maintainer: Franz Király
 Maintainer-email: sktime developers <sktime.toolbox@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, skbase Developers
@@ -86,15 +86,15 @@
 Provides-Extra: docs
 Requires-Dist: jupyter; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: nbsphinx>=0.8.6; extra == "docs"
 Requires-Dist: numpydoc; extra == "docs"
 Requires-Dist: pydata-sphinx-theme; extra == "docs"
 Requires-Dist: sphinx-issues<5.0.0; extra == "docs"
-Requires-Dist: sphinx-gallery<0.16.0; extra == "docs"
+Requires-Dist: sphinx-gallery<0.17.0; extra == "docs"
 Requires-Dist: sphinx-panels; extra == "docs"
 Requires-Dist: sphinx-design<0.6.0; extra == "docs"
 Requires-Dist: Sphinx!=7.2.0,<8.0.0; extra == "docs"
 Requires-Dist: tabulate; extra == "docs"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: coverage; extra == "test"
@@ -110,15 +110,15 @@
 # Welcome to skbase
 
 > A framework factory for scikit-learn-like and sktime-like parametric objects
 
 `skbase` provides base classes for creating scikit-learn-like parametric objects,
 along with tools to make it easier to build your own packages that follow these design patterns.
 
-:rocket: Version 0.7.7 is now available. Check out our
+:rocket: Version 0.7.8 is now available. Check out our
 [release notes](https://skbase.readthedocs.io/en/latest/changelog.html).
 
 | Overview | |
 |---|---|
 | **CI/CD** | [![Tests](https://github.com/sktime/skbase/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/sktime/skbase/actions/workflows/test.yml) [![codecov](https://codecov.io/gh/sktime/skbase/branch/main/graph/badge.svg?token=2J424NLO82)](https://codecov.io/gh/sktime/skbase) [![Documentation Status](https://readthedocs.org/projects/skbase/badge/?version=latest)](https://skbase.readthedocs.io/en/latest/?badge=latest) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sktime/skbase/main.svg)](https://results.pre-commit.ci/latest/github/sktime/skbase/main) |
 | **Code** |  [![!pypi](https://img.shields.io/pypi/v/scikit-base?color=orange)](https://pypi.org/project/scikit-base/)  [![!python-versions](https://img.shields.io/pypi/pyversions/scikit-base)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit) |
 | **Downloads** | [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/scikit-base) |
```

### Comparing `scikit_base-0.7.7/README.md` & `scikit_base-0.7.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Welcome to skbase
 
 > A framework factory for scikit-learn-like and sktime-like parametric objects
 
 `skbase` provides base classes for creating scikit-learn-like parametric objects,
 along with tools to make it easier to build your own packages that follow these design patterns.
 
-:rocket: Version 0.7.7 is now available. Check out our
+:rocket: Version 0.7.8 is now available. Check out our
 [release notes](https://skbase.readthedocs.io/en/latest/changelog.html).
 
 | Overview | |
 |---|---|
 | **CI/CD** | [![Tests](https://github.com/sktime/skbase/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/sktime/skbase/actions/workflows/test.yml) [![codecov](https://codecov.io/gh/sktime/skbase/branch/main/graph/badge.svg?token=2J424NLO82)](https://codecov.io/gh/sktime/skbase) [![Documentation Status](https://readthedocs.org/projects/skbase/badge/?version=latest)](https://skbase.readthedocs.io/en/latest/?badge=latest) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sktime/skbase/main.svg)](https://results.pre-commit.ci/latest/github/sktime/skbase/main) |
 | **Code** |  [![!pypi](https://img.shields.io/pypi/v/scikit-base?color=orange)](https://pypi.org/project/scikit-base/)  [![!python-versions](https://img.shields.io/pypi/pyversions/scikit-base)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit) |
 | **Downloads** | [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/scikit-base) |
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_s_k_t_i_m_e_/_s_k_b_a_s_e_/_b_l_o_b_/_m_a_i_n_/_d_o_c_s_/_s_o_u_r_c_e_/_i_m_a_g_e_s_/_s_k_b_a_s_e_-_l_o_g_o_-
 _w_i_t_h_-_n_a_m_e_._p_n_g_]# Welcome to skbase > A framework factory for scikit-learn-like
 and sktime-like parametric objects `skbase` provides base classes for creating
 scikit-learn-like parametric objects, along with tools to make it easier to
 build your own packages that follow these design patterns. :rocket: Version
-0.7.7 is now available. Check out our [release notes](https://
+0.7.8 is now available. Check out our [release notes](https://
 skbase.readthedocs.io/en/latest/changelog.html). | Overview | | |---|---| |
 **CI/CD** | [![Tests](https://github.com/sktime/skbase/actions/workflows/
 test.yml/badge.svg?branch=main)](https://github.com/sktime/skbase/actions/
 workflows/test.yml) [![codecov](https://codecov.io/gh/sktime/skbase/branch/
 main/graph/badge.svg?token=2J424NLO82)](https://codecov.io/gh/sktime/skbase) [!
 [Documentation Status](https://readthedocs.org/projects/skbase/badge/
 ?version=latest)](https://skbase.readthedocs.io/en/latest/?badge=latest) [!
```

### Comparing `scikit_base-0.7.7/docs/source/conf.py` & `scikit_base-0.7.8/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.7/pyproject.toml` & `scikit_base-0.7.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "scikit-base"
-version = "0.7.7"
+version = "0.7.8"
 description = "Base classes for sklearn-like parametric objects"
 authors = [
     {name = "sktime developers", email = "sktime.toolbox@gmail.com"},
 ]
 maintainers = [
     {name = "sktime developers", email = "sktime.toolbox@gmail.com"},
     {name = "Franz Király"},
@@ -67,15 +67,15 @@
 docs = [
     "jupyter",
     "myst-parser",
     "nbsphinx>=0.8.6",
     "numpydoc",
     "pydata-sphinx-theme",
     "sphinx-issues<5.0.0",
-    "sphinx-gallery<0.16.0",
+    "sphinx-gallery<0.17.0",
     "sphinx-panels",
     "sphinx-design<0.6.0",
     "Sphinx<8.0.0,!=7.2.0",
     "tabulate",
 ]
 
 test = [
```

### Comparing `scikit_base-0.7.7/scikit_base.egg-info/PKG-INFO` & `scikit_base-0.7.8/scikit_base.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-base
-Version: 0.7.7
+Version: 0.7.8
 Summary: Base classes for sklearn-like parametric objects
 Author-email: sktime developers <sktime.toolbox@gmail.com>
 Maintainer: Franz Király
 Maintainer-email: sktime developers <sktime.toolbox@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, skbase Developers
@@ -86,15 +86,15 @@
 Provides-Extra: docs
 Requires-Dist: jupyter; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: nbsphinx>=0.8.6; extra == "docs"
 Requires-Dist: numpydoc; extra == "docs"
 Requires-Dist: pydata-sphinx-theme; extra == "docs"
 Requires-Dist: sphinx-issues<5.0.0; extra == "docs"
-Requires-Dist: sphinx-gallery<0.16.0; extra == "docs"
+Requires-Dist: sphinx-gallery<0.17.0; extra == "docs"
 Requires-Dist: sphinx-panels; extra == "docs"
 Requires-Dist: sphinx-design<0.6.0; extra == "docs"
 Requires-Dist: Sphinx!=7.2.0,<8.0.0; extra == "docs"
 Requires-Dist: tabulate; extra == "docs"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: coverage; extra == "test"
@@ -110,15 +110,15 @@
 # Welcome to skbase
 
 > A framework factory for scikit-learn-like and sktime-like parametric objects
 
 `skbase` provides base classes for creating scikit-learn-like parametric objects,
 along with tools to make it easier to build your own packages that follow these design patterns.
 
-:rocket: Version 0.7.7 is now available. Check out our
+:rocket: Version 0.7.8 is now available. Check out our
 [release notes](https://skbase.readthedocs.io/en/latest/changelog.html).
 
 | Overview | |
 |---|---|
 | **CI/CD** | [![Tests](https://github.com/sktime/skbase/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/sktime/skbase/actions/workflows/test.yml) [![codecov](https://codecov.io/gh/sktime/skbase/branch/main/graph/badge.svg?token=2J424NLO82)](https://codecov.io/gh/sktime/skbase) [![Documentation Status](https://readthedocs.org/projects/skbase/badge/?version=latest)](https://skbase.readthedocs.io/en/latest/?badge=latest) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sktime/skbase/main.svg)](https://results.pre-commit.ci/latest/github/sktime/skbase/main) |
 | **Code** |  [![!pypi](https://img.shields.io/pypi/v/scikit-base?color=orange)](https://pypi.org/project/scikit-base/)  [![!python-versions](https://img.shields.io/pypi/pyversions/scikit-base)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit) |
 | **Downloads** | [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/scikit-base) |
```

### Comparing `scikit_base-0.7.7/scikit_base.egg-info/SOURCES.txt` & `scikit_base-0.7.8/scikit_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.7/scikit_base.egg-info/requires.txt` & `scikit_base-0.7.8/scikit_base.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [docs]
 jupyter
 myst-parser
 nbsphinx>=0.8.6
 numpydoc
 pydata-sphinx-theme
 sphinx-issues<5.0.0
-sphinx-gallery<0.16.0
+sphinx-gallery<0.17.0
 sphinx-panels
 sphinx-design<0.6.0
 Sphinx!=7.2.0,<8.0.0
 tabulate
 
 [linters]
 mypy
```

### Comparing `scikit_base-0.7.7/skbase/_exceptions.py` & `scikit_base-0.7.8/skbase/_exceptions.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.7/skbase/_nopytest_tests.py` & `scikit_base-0.7.8/skbase/_nopytest_tests.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.7/skbase/base/__init__.py` & `scikit_base-0.7.8/skbase/base/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.7/skbase/base/_base.py` & `scikit_base-0.7.8/skbase/base/_base.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.7/skbase/base/_meta.py` & `scikit_base-0.7.8/skbase/base/_meta.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.7/skbase/base/_pretty_printing/_object_html_repr.py` & `scikit_base-0.7.8/skbase/base/_pretty_printing/_object_html_repr.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.7/skbase/base/_pretty_printing/_pprint.py` & `scikit_base-0.7.8/skbase/base/_pretty_printing/_pprint.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.7/skbase/base/_pretty_printing/tests/test_pprint.py` & `scikit_base-0.7.8/skbase/base/_pretty_printing/tests/test_pprint.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.7/skbase/base/_tagmanager.py` & `scikit_base-0.7.8/skbase/base/_tagmanager.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.7/skbase/lookup/__init__.py` & `scikit_base-0.7.8/skbase/lookup/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.7/skbase/lookup/_lookup.py` & `scikit_base-0.7.8/skbase/lookup/_lookup.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.7/skbase/lookup/tests/test_lookup.py` & `scikit_base-0.7.8/skbase/lookup/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.7/skbase/testing/test_all_objects.py` & `scikit_base-0.7.8/skbase/testing/test_all_objects.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.7/skbase/testing/utils/_conditional_fixtures.py` & `scikit_base-0.7.8/skbase/testing/utils/_conditional_fixtures.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.7/skbase/testing/utils/inspect.py` & `scikit_base-0.7.8/skbase/testing/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.7/skbase/tests/conftest.py` & `scikit_base-0.7.8/skbase/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,14 +233,15 @@
             "_fh_equals_plugin",
             "_is_npnan",
             "_is_npndarray",
             "_is_pandas",
             "_numpy_equals_plugin",
             "_pandas_equals",
             "_pandas_equals_plugin",
+            "_safe_any_unequal",
             "_safe_len",
             "_softdep_available",
             "_tuple_equals",
             "deep_equals",
             "deep_equals_custom",
         ),
         "skbase.utils.dependencies._dependencies": (
```

### Comparing `scikit_base-0.7.7/skbase/tests/mock_package/test_mock_package.py` & `scikit_base-0.7.8/skbase/tests/mock_package/test_mock_package.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.7/skbase/tests/test_base.py` & `scikit_base-0.7.8/skbase/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.7/skbase/tests/test_baseestimator.py` & `scikit_base-0.7.8/skbase/tests/test_baseestimator.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.7/skbase/tests/test_exceptions.py` & `scikit_base-0.7.8/skbase/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.7/skbase/tests/test_meta.py` & `scikit_base-0.7.8/skbase/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.7/skbase/utils/__init__.py` & `scikit_base-0.7.8/skbase/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.7/skbase/utils/_check.py` & `scikit_base-0.7.8/skbase/utils/_check.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.7/skbase/utils/_iter.py` & `scikit_base-0.7.8/skbase/utils/_iter.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.7/skbase/utils/_nested_iter.py` & `scikit_base-0.7.8/skbase/utils/_nested_iter.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.7/skbase/utils/_utils.py` & `scikit_base-0.7.8/skbase/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.7/skbase/utils/deep_equals/_common.py` & `scikit_base-0.7.8/skbase/utils/deep_equals/_common.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.7/skbase/utils/deep_equals/_deep_equals.py` & `scikit_base-0.7.8/skbase/utils/deep_equals/_deep_equals.py`

 * *Files 6% similar despite different names*

```diff
@@ -499,26 +499,58 @@
         )
 
     # this if covers case where != is boolean
     # some types return a vector upon !=, this is covered in the next elif
     if isinstance(x == y, bool):
         return ret(x == y, f" !=, {x} != {y}")
 
-    # check if numpy is available
-    numpy_available = _softdep_available("numpy")
-    if numpy_available:
-        import numpy as np
-
     # deal with the case where != returns a vector
-    if numpy_available and np.any(x != y) or np.any(_coerce_list(x != y)):
+    if _safe_any_unequal(x, y):
         return ret(False, f" !=, {x} != {y}")
 
     return ret(True, "")
 
 
+def _safe_any_unequal(x, y):
+    """Return whether any of x != y, if != results in iterable, False on exception.
+
+    Written very defensively to avoid exceptions, as exceptions may be raised
+    since any(x != y) or the safer np.any(x != y) may not be boolean,
+    e.g., in pathological cases of nested objects.
+    """
+    try:
+        unequal = x != y
+    except Exception:
+        return False
+
+    # check if numpy is available
+    numpy_available = _softdep_available("numpy")
+
+    if not numpy_available:
+        try:
+            any_un = any(unequal)
+            if isinstance(any_un, bool):
+                return any_un
+            else:
+                return False
+        except Exception:
+            return False
+
+    import numpy as np
+
+    try:
+        any_un = np.any(x != y) or np.any(_coerce_list(x != y))
+        if isinstance(any_un, bool) or any_un.dtype == "bool":
+            return any_un
+        else:
+            return False
+    except Exception:
+        return False
+
+
 def _safe_len(x):
     """Return length of x if len(x) does not result in exception, else -1."""
     if hasattr(x, "__len__"):
         try:
             x_len = len(x)
             return x_len
         except Exception:
```

### Comparing `scikit_base-0.7.7/skbase/utils/dependencies/_dependencies.py` & `scikit_base-0.7.8/skbase/utils/dependencies/_dependencies.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.7/skbase/utils/dependencies/tests/test_check_dependencies.py` & `scikit_base-0.7.8/skbase/utils/dependencies/tests/test_check_dependencies.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.7/skbase/utils/random_state.py` & `scikit_base-0.7.8/skbase/utils/random_state.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.7/skbase/utils/tests/test_check.py` & `scikit_base-0.7.8/skbase/utils/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.7/skbase/utils/tests/test_deep_equals.py` & `scikit_base-0.7.8/skbase/utils/tests/test_deep_equals.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.7/skbase/utils/tests/test_iter.py` & `scikit_base-0.7.8/skbase/utils/tests/test_iter.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.7/skbase/utils/tests/test_nested_iter.py` & `scikit_base-0.7.8/skbase/utils/tests/test_nested_iter.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.7/skbase/utils/tests/test_random_state.py` & `scikit_base-0.7.8/skbase/utils/tests/test_random_state.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.7/skbase/utils/tests/test_utils.py` & `scikit_base-0.7.8/skbase/utils/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.7/skbase/validate/__init__.py` & `scikit_base-0.7.8/skbase/validate/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.7/skbase/validate/_named_objects.py` & `scikit_base-0.7.8/skbase/validate/_named_objects.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.7/skbase/validate/_types.py` & `scikit_base-0.7.8/skbase/validate/_types.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.7/skbase/validate/tests/test_iterable_named_objects.py` & `scikit_base-0.7.8/skbase/validate/tests/test_iterable_named_objects.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.7/skbase/validate/tests/test_type_validations.py` & `scikit_base-0.7.8/skbase/validate/tests/test_type_validations.py`

 * *Files identical despite different names*

