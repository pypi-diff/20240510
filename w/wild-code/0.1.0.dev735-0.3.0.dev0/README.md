# Comparing `tmp/wild_code-0.1.0.dev735.tar.gz` & `tmp/wild_code-0.3.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wild_code-0.1.0.dev735.tar", last modified: Tue May  7 18:22:40 2024, max compression
+gzip compressed data, was "wild_code-0.3.0.dev0.tar", last modified: Thu May  9 22:33:09 2024, max compression
```

## Comparing `wild_code-0.1.0.dev735.tar` & `wild_code-0.3.0.dev0.tar`

### file list

```diff
@@ -1,57 +1,56 @@
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-07 18:20:05.768705 wild_code-0.1.0.dev735/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3286 2024-05-07 17:11:36.000000 wild_code-0.1.0.dev735/.dockerignore
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-07 18:20:04.953182 wild_code-0.1.0.dev735/.github/
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-07 18:20:04.952620 wild_code-0.1.0.dev735/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1411 2024-05-07 17:11:36.000000 wild_code-0.1.0.dev735/.github/ISSUE_TEMPLATE/buggy_contract.yml
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1461 2024-05-07 17:11:36.000000 wild_code-0.1.0.dev735/.github/ISSUE_TEMPLATE/buggy_test.yml
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)       27 2024-05-07 17:11:36.000000 wild_code-0.1.0.dev735/.github/ISSUE_TEMPLATE/config.yml
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     2177 2024-05-07 17:11:36.000000 wild_code-0.1.0.dev735/.github/ISSUE_TEMPLATE/model_eval_request.yml
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3237 2024-05-07 17:11:36.000000 wild_code-0.1.0.dev735/.gitignore
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      458 2024-05-07 17:11:36.000000 wild_code-0.1.0.dev735/.pre-commit-config.yaml
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      413 2024-05-07 17:11:36.000000 wild_code-0.1.0.dev735/CITATION.cff
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      491 2024-05-07 17:54:30.000000 wild_code-0.1.0.dev735/Dockerfile
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)    11438 2024-05-07 17:11:36.000000 wild_code-0.1.0.dev735/LICENSE
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)       39 2024-05-07 17:11:36.000000 wild_code-0.1.0.dev735/MANIFEST.in
--rw-r--r--   0 zhuoyt    (1001) zhuoyt    (1001)     9040 2024-05-07 18:20:05.762997 wild_code-0.1.0.dev735/PKG-INFO
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     8088 2024-05-07 17:11:36.000000 wild_code-0.1.0.dev735/README.md
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      246 2024-05-07 17:11:36.000000 wild_code-0.1.0.dev735/pyproject.toml
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      603 2024-05-07 17:55:37.000000 wild_code-0.1.0.dev735/release.sh
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      991 2024-05-07 17:11:36.000000 wild_code-0.1.0.dev735/requirements-wildcodebench.txt
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      155 2024-05-07 17:11:36.000000 wild_code-0.1.0.dev735/requirements.txt
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1239 2024-05-07 17:11:36.000000 wild_code-0.1.0.dev735/run.sh
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1167 2024-05-07 18:20:05.783924 wild_code-0.1.0.dev735/setup.cfg
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-07 18:20:04.958553 wild_code-0.1.0.dev735/tests/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)        7 2024-05-07 17:11:36.000000 wild_code-0.1.0.dev735/tests/requirements.txt
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      854 2024-05-07 17:11:36.000000 wild_code-0.1.0.dev735/tests/test_legacy_sanitizer.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3964 2024-05-07 17:11:36.000000 wild_code-0.1.0.dev735/tests/test_treesitter_sanitizer.py
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-07 18:20:05.740921 wild_code-0.1.0.dev735/wild_code.egg-info/
--rw-r--r--   0 zhuoyt    (1001) zhuoyt    (1001)     9040 2024-05-07 18:20:04.000000 wild_code-0.1.0.dev735/wild_code.egg-info/PKG-INFO
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1126 2024-05-07 18:20:04.000000 wild_code-0.1.0.dev735/wild_code.egg-info/SOURCES.txt
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)        1 2024-05-07 18:20:04.000000 wild_code-0.1.0.dev735/wild_code.egg-info/dependency_links.txt
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      288 2024-05-07 18:20:04.000000 wild_code-0.1.0.dev735/wild_code.egg-info/entry_points.txt
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      201 2024-05-07 18:20:04.000000 wild_code-0.1.0.dev735/wild_code.egg-info/requires.txt
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)        9 2024-05-07 18:20:04.000000 wild_code-0.1.0.dev735/wild_code.egg-info/top_level.txt
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-07 18:20:04.993840 wild_code-0.1.0.dev735/wildcode/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      120 2024-05-07 17:11:36.000000 wild_code-0.1.0.dev735/wildcode/__init__.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      428 2024-05-07 18:20:04.000000 wild_code-0.1.0.dev735/wildcode/_version.py
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-07 18:20:04.982777 wild_code-0.1.0.dev735/wildcode/data/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      163 2024-05-07 17:11:36.000000 wild_code-0.1.0.dev735/wildcode/data/__init__.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     6076 2024-05-07 17:11:36.000000 wild_code-0.1.0.dev735/wildcode/data/utils.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1647 2024-05-07 17:11:36.000000 wild_code-0.1.0.dev735/wildcode/data/wildcodebench.py
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-07 18:20:04.988105 wild_code-0.1.0.dev735/wildcode/eval/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     7014 2024-05-07 17:11:36.000000 wild_code-0.1.0.dev735/wildcode/eval/__init__.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      377 2024-05-07 17:11:36.000000 wild_code-0.1.0.dev735/wildcode/eval/_special_oracle.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     6161 2024-05-07 17:11:36.000000 wild_code-0.1.0.dev735/wildcode/eval/utils.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     8144 2024-05-07 17:11:36.000000 wild_code-0.1.0.dev735/wildcode/evaluate.py
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-07 18:20:05.002379 wild_code-0.1.0.dev735/wildcode/gen/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      753 2024-05-07 17:11:36.000000 wild_code-0.1.0.dev735/wildcode/gen/__init__.py
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-07 18:20:05.001902 wild_code-0.1.0.dev735/wildcode/gen/util/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1255 2024-05-07 17:11:36.000000 wild_code-0.1.0.dev735/wildcode/gen/util/__init__.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1439 2024-05-07 17:11:36.000000 wild_code-0.1.0.dev735/wildcode/gen/util/anthropic_request.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1813 2024-05-07 17:11:36.000000 wild_code-0.1.0.dev735/wildcode/gen/util/openai_request.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     5554 2024-05-07 17:11:36.000000 wild_code-0.1.0.dev735/wildcode/generate.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     2314 2024-05-07 17:11:36.000000 wild_code-0.1.0.dev735/wildcode/inspect.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     5724 2024-05-07 17:11:36.000000 wild_code-0.1.0.dev735/wildcode/lecacy_sanitize.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)    14088 2024-05-07 17:11:36.000000 wild_code-0.1.0.dev735/wildcode/model.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     7767 2024-05-07 17:11:36.000000 wild_code-0.1.0.dev735/wildcode/sanitize.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3466 2024-05-07 17:11:36.000000 wild_code-0.1.0.dev735/wildcode/syncheck.py
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-09 22:30:32.705349 wild_code-0.3.0.dev0/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3286 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/.dockerignore
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-09 22:30:31.925358 wild_code-0.3.0.dev0/.github/
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-09 22:30:31.924756 wild_code-0.3.0.dev0/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1411 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/.github/ISSUE_TEMPLATE/buggy_contract.yml
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1461 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/.github/ISSUE_TEMPLATE/buggy_test.yml
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)       27 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/.github/ISSUE_TEMPLATE/config.yml
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     2177 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/.github/ISSUE_TEMPLATE/model_eval_request.yml
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3237 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/.gitignore
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      458 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/.pre-commit-config.yaml
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      413 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/CITATION.cff
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      542 2024-05-09 21:30:14.000000 wild_code-0.3.0.dev0/Dockerfile
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)    11438 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/LICENSE
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)       39 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/MANIFEST.in
+-rw-r--r--   0 zhuoyt    (1001) zhuoyt    (1001)    10697 2024-05-09 22:30:32.701093 wild_code-0.3.0.dev0/PKG-INFO
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     9579 2024-05-09 21:16:41.000000 wild_code-0.3.0.dev0/README.md
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      246 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/pyproject.toml
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      639 2024-05-09 22:24:07.000000 wild_code-0.3.0.dev0/release.sh
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      155 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/requirements.txt
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1334 2024-05-09 21:29:07.000000 wild_code-0.3.0.dev0/run.sh
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1237 2024-05-09 22:30:32.722612 wild_code-0.3.0.dev0/setup.cfg
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-09 22:30:31.930281 wild_code-0.3.0.dev0/tests/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)        7 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/tests/requirements.txt
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      854 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/tests/test_legacy_sanitizer.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3964 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/tests/test_treesitter_sanitizer.py
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-09 22:30:32.682162 wild_code-0.3.0.dev0/wild_code.egg-info/
+-rw-r--r--   0 zhuoyt    (1001) zhuoyt    (1001)    10697 2024-05-09 22:30:31.000000 wild_code-0.3.0.dev0/wild_code.egg-info/PKG-INFO
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1095 2024-05-09 22:30:31.000000 wild_code-0.3.0.dev0/wild_code.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)        1 2024-05-09 22:30:31.000000 wild_code-0.3.0.dev0/wild_code.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      288 2024-05-09 22:30:31.000000 wild_code-0.3.0.dev0/wild_code.egg-info/entry_points.txt
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      264 2024-05-09 22:30:31.000000 wild_code-0.3.0.dev0/wild_code.egg-info/requires.txt
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)        9 2024-05-09 22:30:31.000000 wild_code-0.3.0.dev0/wild_code.egg-info/top_level.txt
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-09 22:30:31.959927 wild_code-0.3.0.dev0/wildcode/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      120 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/wildcode/__init__.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      424 2024-05-09 22:30:31.000000 wild_code-0.3.0.dev0/wildcode/_version.py
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-09 22:30:31.948951 wild_code-0.3.0.dev0/wildcode/data/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      163 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/wildcode/data/__init__.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     6076 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/wildcode/data/utils.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1670 2024-05-09 17:42:50.000000 wild_code-0.3.0.dev0/wildcode/data/wildcodebench.py
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-09 22:30:31.954317 wild_code-0.3.0.dev0/wildcode/eval/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     7214 2024-05-09 18:37:38.000000 wild_code-0.3.0.dev0/wildcode/eval/__init__.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      377 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/wildcode/eval/_special_oracle.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     5654 2024-05-09 20:59:10.000000 wild_code-0.3.0.dev0/wildcode/eval/utils.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     8293 2024-05-09 21:19:35.000000 wild_code-0.3.0.dev0/wildcode/evaluate.py
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-09 22:30:31.968590 wild_code-0.3.0.dev0/wildcode/gen/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      753 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/wildcode/gen/__init__.py
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-09 22:30:31.968039 wild_code-0.3.0.dev0/wildcode/gen/util/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1663 2024-05-08 23:14:51.000000 wild_code-0.3.0.dev0/wildcode/gen/util/__init__.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1439 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/wildcode/gen/util/anthropic_request.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1813 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/wildcode/gen/util/openai_request.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     5554 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/wildcode/generate.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     2314 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/wildcode/inspect.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     5724 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/wildcode/lecacy_sanitize.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)    14089 2024-05-09 02:01:13.000000 wild_code-0.3.0.dev0/wildcode/model.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     7995 2024-05-09 20:59:00.000000 wild_code-0.3.0.dev0/wildcode/sanitize.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3466 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/wildcode/syncheck.py
```

### Comparing `wild_code-0.1.0.dev735/.dockerignore` & `wild_code-0.3.0.dev0/.dockerignore`

 * *Files identical despite different names*

### Comparing `wild_code-0.1.0.dev735/.github/ISSUE_TEMPLATE/buggy_contract.yml` & `wild_code-0.3.0.dev0/.github/ISSUE_TEMPLATE/buggy_contract.yml`

 * *Files identical despite different names*

### Comparing `wild_code-0.1.0.dev735/.github/ISSUE_TEMPLATE/buggy_test.yml` & `wild_code-0.3.0.dev0/.github/ISSUE_TEMPLATE/buggy_test.yml`

 * *Files identical despite different names*

### Comparing `wild_code-0.1.0.dev735/.github/ISSUE_TEMPLATE/model_eval_request.yml` & `wild_code-0.3.0.dev0/.github/ISSUE_TEMPLATE/model_eval_request.yml`

 * *Files identical despite different names*

### Comparing `wild_code-0.1.0.dev735/.gitignore` & `wild_code-0.3.0.dev0/.gitignore`

 * *Files identical despite different names*

### Comparing `wild_code-0.1.0.dev735/LICENSE` & `wild_code-0.3.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `wild_code-0.1.0.dev735/PKG-INFO` & `wild_code-0.3.0.dev0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,30 @@
-Metadata-Version: 2.1
-Name: wild-code
-Version: 0.1.0.dev735
-Summary: "WildCode: A minimal viable package to evaluate code generation with realistic constraints in the wild"
-Home-page: https://github.com/bigcode-project/wild-code
-License: Apache-2.0
-Platform: any
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: wget>=3.2
-Requires-Dist: tempdir>=0.7.1
-Requires-Dist: multipledispatch>=0.6.0
-Requires-Dist: appdirs>=1.4.4
-Requires-Dist: numpy>=1.19.5
-Requires-Dist: tqdm>=4.56.0
-Requires-Dist: termcolor>=2.0.0
-Requires-Dist: fire>=0.6.0
-Requires-Dist: openai>=1.11.1
-Provides-Extra: perf
-Requires-Dist: Pympler>=1.0.1; extra == "perf"
-Requires-Dist: rich>=12.3.0; extra == "perf"
-Requires-Dist: tree_sitter_languages>=1.10.2; extra == "perf"
-
 # 🌳WildCodeBench
 
 > [!WARNING] 
 > The project is under active development. Please check back later for more updates.
 
 > [!WARNING]
-> WildCode framework currently only supports the Code2Code generation task. We are working on adding the NL2Code task based on NL instructions.
+> Please use WildCode with caution. Different from [EvalPlus](https://github.com/evalplus/evalplus), WildCode has a much less constrained execution environment to support tasks with diverse library dependencies. This may lead to security risks. We recommend using a sandbox such as [Docker](https://docs.docker.com/get-docker/) to run the evaluation.
+
+> [!WARNING]
+> WildCode framework currently only supports the Code2Code generation task. We are working on adding the NL2Code task.
 
 <p align="center">
+    <a href="https://pypi.org/project/wild-code/"><img src="https://img.shields.io/pypi/v/wild-code?color=g"></a>
+    <a href="https://hub.docker.com/r/terryzho/wildcode" title="Docker"><img src="https://img.shields.io/docker/image-size/terryzho/wildcode"></a>
+    <a href="https://github.com/evalplus/evalplus/blob/master/LICENSE"><img src="https://img.shields.io/pypi/l/wild-code"></a>
+</p>
+
+<p align="center">
+    <a href="#-about">🌳About</a> •
     <a href="#-quick-start">🔥Quick Start</a> •
     <a href="#-llm-generated-code">💻LLM code</a> •
-    <a href="#-useful-tools">🔨Tools</a> •
+    <a href="#-failure-inspection">🔍Failure inspection</a> •
+    <a href="#-known-issues">🐞Known issues</a> •
     <a href="#-citation">📜Citation</a> •
     <a href="#-acknowledgement">🙏Acknowledgement</a>
 </p>
 
 ## About
 
 ### WildCodeBench
@@ -54,14 +38,19 @@
 ### Why WildCode?
 
 WildCode is a rigorous evaluation framework for LLM4Code, with:
 
 * ✨ **Precise evaluation & ranking**: See [our leaderboard](https://wildcodebench.github.io/leaderboard.html) for latest LLM rankings before & after rigorous evaluation.
 * ✨ **Pre-generated samples**: WildCode accelerates code intelligence research by open-sourcing [LLM-generated samples](#-LLM-generated-code) for various models -- no need to re-run the expensive benchmarks!
 
+### Main Differences from EvalPlus
+
+We inherit the design of the EvalPlus framework, which is a flexible and extensible evaluation framework for code generation tasks. However, WildCode has the following differences:
+* Execution Environment: The execution environment in WildCode is less bounded than EvalPlus to support tasks with diverse library dependencies.
+* Test Evaluation: WildCode relies on `unittest` for evaluating the generated code, which is more suitable for the test harness in WildCodeBench.
 
 ## 🔥 Quick Start
 
 > [!Tip]
 >
 > WildCode ❤️ [bigcode-evaluation-harness](https://github.com/bigcode-project/bigcode-evaluation-harness)!
 > WildCodeBench will be integrated to bigcode-evaluation-harness, and you can also run it there!
@@ -91,15 +80,15 @@
 export PYTHONPATH=$PYTHONPATH:$(pwd)
 pip install -e .
 ```
 
 </div>
 </details>
 
-### Code generation
+### Code Generation
 
 To generate code samples from a model, you can use the following command:
 
 ```shell
 wildcode.generate --model [model_name] --dataset wildcodebench --greedy --bs [bs] --temperature [temp] --n_samples [n_samples] --resume --backend [vllm|hf|openai]
 ```
 The generated code samples will be stored in a file named `[model_name]--wildcodebench--[backend]-[temp]-[n_samples].jsonl`.
@@ -121,15 +110,15 @@
 >
 > **Expected Schema of `[model_name]--wildcodebench--[backend]-[temp]-[n_samples].jsonl`**
 >
 > 1. `task_id`: Task ID, which are the keys of `get_[human_eval|mbpp]_plus()`
 > 2. `solution` (optional): Self-contained solution (usually including the prompt)
 >    * Example: `{"task_id": "HumanEval/?", "solution": "def f():\n    return 1"}`
 
-### Code post-processing
+### Code Post-processing
 
 LLM-generated text may not be compilable code for including natural language lines or incomplete extra code.
 We provide a tool namely `wildcode.sanitize` to clean up the code:
 
 ```shell
 # 💡 If you are storing codes in jsonl:
 wildcode.sanitize --samples samples.jsonl
@@ -153,19 +142,20 @@
 wildcode.syncheck --samples /path/to/vicuna-[??]b_temp_[??] --dataset [wildcodebench]
 ```
 
 </div>
 </details>
 
 
-### Code evaluation
+### Code Evaluation
 
 You are strongly recommended to use a sandbox such as [docker](https://docs.docker.com/get-docker/):
 
 ```shell
+docker run -v $(pwd):/app terryzho/wildcode:latest --dataset [wildcodebench] --samples samples.jsonl
 ```
 
 ...Or if you want to try it locally regardless of the risks ⚠️:
 
 First, install the dependencies for WildCodeBench:
 
 ```shell
@@ -196,19 +186,19 @@
 </div>
 </details>
 
 The output should be like (below is GPT-4 greedy decoding example):
 
 ```
 Asserting the groundtruth...
-Expected outputs computed in 2400.0 seconds
+Expected outputs computed in 1200.0 seconds
 Reading samples...
-964it [30:04, 37.79it/s]
+1047it [00:00, 1901.64it/s]
 Evaluating samples...
-100%|██████████████████████████████████████████| 964/964 [00:03<00:00, 44.75it/s]
+100%|██████████████████████████████████████████| 1047/1047 [19:53<00:00, 6.75it/s]
 Base
 {'pass@1': 0.548}
 ```
 
 - `Base` is the `pass@k` for the original HumanEval
 - The "k" includes `[1, 10, 100]` where k values `<=` the sample size will be used
 - A cache file named like `samples_eval_results.jsonl` will be cached. Remove it to re-run the evaluation
@@ -227,28 +217,28 @@
 </details>
 
 ## Failure Inspection
 
 You can inspect the failed samples by using the following command:
 
 ```shell
-wildcode.inspect --dataset $DATASET --eval-results sample-sanitized_eval_results.json --in-place
+wildcode.inspect --dataset [wildcodebench] --eval-results sample-sanitized_eval_results.json --in-place
 ```
 
-## Full Script
+## Full script
 
 We provide a sample script to run the full pipeline:
 
 ```shell
 bash run.sh
 ```
 
-## 💻 LLM-generated code
+## 💻 LLM-generated Code
 
-We share pre-generated code samples from LLMs we have [evaluated](https://wildcodebench.github.io/leaderboard.html):
+We will share pre-generated code samples from LLMs we have [evaluated](https://wildcodebench.github.io/leaderboard.html):
 
 ## Known Issues
 
 - [ ] We notice that some tasks heavily use memory for scientific modeling during testing. It will lead to timeout issues on some machines. If you get an error message like `Check failed: ret == 0 (11 vs. 0)Thread creation via pthread_create() failed.` in Tensorflow, it is very likely due to the memory issue. Try to allocate more memory to the process or reduce the number of parallel processes.
 
 ## 📜 Citation
```

#### html2text {}

```diff
@@ -1,26 +1,20 @@
-Metadata-Version: 2.1 Name: wild-code Version: 0.1.0.dev735 Summary: "WildCode:
-A minimal viable package to evaluate code generation with realistic constraints
-in the wild" Home-page: https://github.com/bigcode-project/wild-code License:
-Apache-2.0 Platform: any Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
-Approved :: Apache Software License Requires-Python: >=3.8 Description-Content-
-Type: text/markdown License-File: LICENSE Requires-Dist: wget>=3.2 Requires-
-Dist: tempdir>=0.7.1 Requires-Dist: multipledispatch>=0.6.0 Requires-Dist:
-appdirs>=1.4.4 Requires-Dist: numpy>=1.19.5 Requires-Dist: tqdm>=4.56.0
-Requires-Dist: termcolor>=2.0.0 Requires-Dist: fire>=0.6.0 Requires-Dist:
-openai>=1.11.1 Provides-Extra: perf Requires-Dist: Pympler>=1.0.1; extra ==
-"perf" Requires-Dist: rich>=12.3.0; extra == "perf" Requires-Dist:
-tree_sitter_languages>=1.10.2; extra == "perf" # ð³WildCodeBench > [!WARNING]
-> The project is under active development. Please check back later for more
-updates. > [!WARNING] > WildCode framework currently only supports the
-Code2Code generation task. We are working on adding the NL2Code task based on
-NL instructions.
-      _ð___¥_Q_u_i_c_k_ _S_t_a_r_t â¢ _ð___»_L_L_M_ _c_o_d_e â¢ _ð___¨_T_o_o_l_s â¢ _ð____C_i_t_a_t_i_o_n â¢
-                              _ð____A_c_k_n_o_w_l_e_d_g_e_m_e_n_t
+# ð³WildCodeBench > [!WARNING] > The project is under active development.
+Please check back later for more updates. > [!WARNING] > Please use WildCode
+with caution. Different from [EvalPlus](https://github.com/evalplus/evalplus),
+WildCode has a much less constrained execution environment to support tasks
+with diverse library dependencies. This may lead to security risks. We
+recommend using a sandbox such as [Docker](https://docs.docker.com/get-docker/
+) to run the evaluation. > [!WARNING] > WildCode framework currently only
+supports the Code2Code generation task. We are working on adding the NL2Code
+task.
+   _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_w_i_l_d_-_c_o_d_e_?_c_o_l_o_r_=_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+ _d_o_c_k_e_r_/_i_m_a_g_e_-_s_i_z_e_/_t_e_r_r_y_z_h_o_/_w_i_l_d_c_o_d_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_l_/_w_i_l_d_-_c_o_d_e_]
+ _ð___³_A_b_o_u_t â¢ _ð___¥_Q_u_i_c_k_ _S_t_a_r_t â¢ _ð___»_L_L_M_ _c_o_d_e â¢ _ð____F_a_i_l_u_r_e_ _i_n_s_p_e_c_t_i_o_n â¢
+           _ð____K_n_o_w_n_ _i_s_s_u_e_s â¢ _ð____C_i_t_a_t_i_o_n â¢ _ð____A_c_k_n_o_w_l_e_d_g_e_m_e_n_t
 ## About ### WildCodeBench WildCodeBench is a rigorous benchmark for code
 generation with realistic constraints in the wild. It aims to evaluate the true
 programming capabilities of large language models (LLMs) in a more realistic
 setting. The benchmark is designed for HumanEval-like function-level code
 generation tasks, but with much more fine-grained descriptions and diverse tool
 use. ### WildCode To facilitate the evaluation of LLMs on WildCodeBench, we
 provide a Python package `wild-code` that includes the dataset, generation
@@ -28,41 +22,48 @@
 (https://github.com/evalplus/evalplus) framework, which is a flexible and
 extensible evaluation framework for code generation tasks. ### Why WildCode?
 WildCode is a rigorous evaluation framework for LLM4Code, with: * â¨ **Precise
 evaluation & ranking**: See [our leaderboard](https://wildcodebench.github.io/
 leaderboard.html) for latest LLM rankings before & after rigorous evaluation. *
 â¨ **Pre-generated samples**: WildCode accelerates code intelligence research
 by open-sourcing [LLM-generated samples](#-LLM-generated-code) for various
-models -- no need to re-run the expensive benchmarks! ## ð¥ Quick Start >
-[!Tip] > > WildCode â¤ï¸ [bigcode-evaluation-harness](https://github.com/
-bigcode-project/bigcode-evaluation-harness)! > WildCodeBench will be integrated
-to bigcode-evaluation-harness, and you can also run it there! To get started,
-please first set up the environment: ```shell pip install wild-code --upgrade
-``` â¬ Install nightly version :: click to expand ::
+models -- no need to re-run the expensive benchmarks! ### Main Differences from
+EvalPlus We inherit the design of the EvalPlus framework, which is a flexible
+and extensible evaluation framework for code generation tasks. However,
+WildCode has the following differences: * Execution Environment: The execution
+environment in WildCode is less bounded than EvalPlus to support tasks with
+diverse library dependencies. * Test Evaluation: WildCode relies on `unittest`
+for evaluating the generated code, which is more suitable for the test harness
+in WildCodeBench. ## ð¥ Quick Start > [!Tip] > > WildCode â¤ï¸ [bigcode-
+evaluation-harness](https://github.com/bigcode-project/bigcode-evaluation-
+harness)! > WildCodeBench will be integrated to bigcode-evaluation-harness, and
+you can also run it there! To get started, please first set up the environment:
+```shell pip install wild-code --upgrade ``` â¬ Install nightly version ::
+click to expand ::
 ```shell pip install "git+https://github.com/bigcode-project/wild-code.git" --
 upgrade ```
 â¬ Using WildCode as a local repo? :: click to expand ::
 ```shell git clone https://github.com/bigcode-project/wild-code.git cd wild-
 code export PYTHONPATH=$PYTHONPATH:$(pwd) pip install -e . ```
-### Code generation To generate code samples from a model, you can use the
+### Code Generation To generate code samples from a model, you can use the
 following command: ```shell wildcode.generate --model [model_name] --dataset
 wildcodebench --greedy --bs [bs] --temperature [temp] --n_samples [n_samples] -
 -resume --backend [vllm|hf|openai] ``` The generated code samples will be
 stored in a file named `[model_name]--wildcodebench--[backend]-[temp]-
 [n_samples].jsonl`. ð¤ Structure of `problem`? :: click to expand ::
 * `task_id` is the identifier string for the task * `entry_point` is the name
 of the function * `prompt` is the function signature with docstring *
 `instruction` is the instruction for the task completion + `canonical_solution`
 is the ground-truth implementation (re-implemented to fix bugs in HumanEval) +
 `test` is the `unittest` test case
 > [!Note] > > **Expected Schema of `[model_name]--wildcodebench--[backend]-
 [temp]-[n_samples].jsonl`** > > 1. `task_id`: Task ID, which are the keys of
 `get_[human_eval|mbpp]_plus()` > 2. `solution` (optional): Self-contained
 solution (usually including the prompt) > * Example: `{"task_id": "HumanEval/
-?", "solution": "def f():\n return 1"}` ### Code post-processing LLM-generated
+?", "solution": "def f():\n return 1"}` ### Code Post-processing LLM-generated
 text may not be compilable code for including natural language lines or
 incomplete extra code. We provide a tool namely `wildcode.sanitize` to clean up
 the code: ```shell # ð¡ If you are storing codes in jsonl: wildcode.sanitize
 --samples samples.jsonl # Sanitized code will be produced to `samples-
 sanitized.jsonl` # ð¡ If you are storing codes in directories:
 wildcode.sanitize --samples /path/to/vicuna-[??]b_temp_[??] # Sanitized code
 will be produced to `/path/to/vicuna-[??]b_temp_[??]-sanitized` ``` ð
@@ -70,48 +71,50 @@
 To double-check the post-processing results, you can use `wildcode.syncheck` to
 check the code validity before and after sanitization, which will print
 erroneous code snippets and why they are wrong: ```shell # ð¡ If you are
 storing codes in jsonl: wildcode.syncheck --samples samples.jsonl --dataset
 [wildcodebench] # ð¡ If you are storing codes in directories:
 wildcode.syncheck --samples /path/to/vicuna-[??]b_temp_[??] --dataset
 [wildcodebench] ```
-### Code evaluation You are strongly recommended to use a sandbox such as
-[docker](https://docs.docker.com/get-docker/): ```shell ``` ...Or if you want
-to try it locally regardless of the risks â ï¸: First, install the
-dependencies for WildCodeBench: ```shell pip install -r requirements-
-wildcodebench.txt ``` Then, run the evaluation: ```shell wildcode.evaluate --
-dataset [wildcodebench] --samples samples.jsonl ``` > [!Tip] > > Do you use a
-very slow machine? > > LLM solutions are regarded as **failed** on timeout (and
-OOM etc.). > Specifically, we set the dynamic timeout based on the ground-truth
-solution's runtime. > > Additionally, you are **NOT** encouraged to make your
-test-bed over stressed while running evaluation. > For example, using `--
-parallel 64` on a 4-core machine or doing something else during evaluation are
-bad ideas... â¨ï¸ More command-line flags :: click to expand ::
+### Code Evaluation You are strongly recommended to use a sandbox such as
+[docker](https://docs.docker.com/get-docker/): ```shell docker run -v $(pwd):/
+app terryzho/wildcode:latest --dataset [wildcodebench] --samples samples.jsonl
+``` ...Or if you want to try it locally regardless of the risks â ï¸: First,
+install the dependencies for WildCodeBench: ```shell pip install -
+r requirements-wildcodebench.txt ``` Then, run the evaluation: ```shell
+wildcode.evaluate --dataset [wildcodebench] --samples samples.jsonl ``` >
+[!Tip] > > Do you use a very slow machine? > > LLM solutions are regarded as
+**failed** on timeout (and OOM etc.). > Specifically, we set the dynamic
+timeout based on the ground-truth solution's runtime. > > Additionally, you are
+**NOT** encouraged to make your test-bed over stressed while running
+evaluation. > For example, using `--parallel 64` on a 4-core machine or doing
+something else during evaluation are bad ideas... â¨ï¸ More command-line
+flags :: click to expand ::
 * `--parallel`: by default half of the cores
 The output should be like (below is GPT-4 greedy decoding example): ```
-Asserting the groundtruth... Expected outputs computed in 2400.0 seconds
-Reading samples... 964it [30:04, 37.79it/s] Evaluating samples...
+Asserting the groundtruth... Expected outputs computed in 1200.0 seconds
+Reading samples... 1047it [00:00, 1901.64it/s] Evaluating samples...
 100%|ââââââââââââââââââââââââââââââââââââââââââ|
-964/964 [00:03<00:00, 44.75it/s] Base {'pass@1': 0.548} ``` - `Base` is the
+1047/1047 [19:53<00:00, 6.75it/s] Base {'pass@1': 0.548} ``` - `Base` is the
 `pass@k` for the original HumanEval - The "k" includes `[1, 10, 100]` where k
 values `<=` the sample size will be used - A cache file named like
 `samples_eval_results.jsonl` will be cached. Remove it to re-run the evaluation
 ð¤ How long it would take? :: click to expand ::
 If you do greedy decoding where there is only one sample for each task, the
 evaluation should take just a few seconds. When running 1 sample x 964 tasks x
 all tests, it can take around ??-?? minutes by using `--parallel 64` and `--
 test-details`. Here are some tips to speed up the evaluation: * Use `--parallel
 $(nproc)` * Use our pre-evaluated results (see [LLM-generated code](#-LLM-
 generated-code))
 ## Failure Inspection You can inspect the failed samples by using the following
-command: ```shell wildcode.inspect --dataset $DATASET --eval-results sample-
-sanitized_eval_results.json --in-place ``` ## Full Script We provide a sample
-script to run the full pipeline: ```shell bash run.sh ``` ## ð» LLM-generated
-code We share pre-generated code samples from LLMs we have [evaluated](https://
-wildcodebench.github.io/leaderboard.html): ## Known Issues - [ ] We notice that
-some tasks heavily use memory for scientific modeling during testing. It will
-lead to timeout issues on some machines. If you get an error message like
-`Check failed: ret == 0 (11 vs. 0)Thread creation via pthread_create() failed.`
-in Tensorflow, it is very likely due to the memory issue. Try to allocate more
-memory to the process or reduce the number of parallel processes. ## ð
-Citation ```bibtex ``` ## ð Acknowledgement - [EvalPlus](https://github.com/
-evalplus/evalplus)
+command: ```shell wildcode.inspect --dataset [wildcodebench] --eval-results
+sample-sanitized_eval_results.json --in-place ``` ## Full script We provide a
+sample script to run the full pipeline: ```shell bash run.sh ``` ## ð» LLM-
+generated Code We will share pre-generated code samples from LLMs we have
+[evaluated](https://wildcodebench.github.io/leaderboard.html): ## Known Issues
+- [ ] We notice that some tasks heavily use memory for scientific modeling
+during testing. It will lead to timeout issues on some machines. If you get an
+error message like `Check failed: ret == 0 (11 vs. 0)Thread creation via
+pthread_create() failed.` in Tensorflow, it is very likely due to the memory
+issue. Try to allocate more memory to the process or reduce the number of
+parallel processes. ## ð Citation ```bibtex ``` ## ð Acknowledgement -
+[EvalPlus](https://github.com/evalplus/evalplus)
```

### Comparing `wild_code-0.1.0.dev735/release.sh` & `wild_code-0.3.0.dev0/release.sh`

 * *Files 14% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   exit 1
 fi
 
 export PYTHONPATH=$PWD pytest tests
 
 git tag $version
 
-# docker build
-docker build . -t terryzho/wildcode:$version
-docker tag terryzho/wildcode:$version terryzho/wildcode:latest
-docker push terryzho/wildcode:$version
-docker push terryzho/wildcode:latest
+# # docker build
+# docker build . -t terryzho/wildcode:$version
+# docker tag terryzho/wildcode:$version terryzho/wildcode:latest
+# docker push terryzho/wildcode:$version
+# docker push terryzho/wildcode:latest
 
 rm -rf dist
 python3 -m build
-python3 -m twine upload dist/*
+python3 -m twine upload --skip-existing --verbose dist/*
 
 # git push
 git push
 git push --tags
```

### Comparing `wild_code-0.1.0.dev735/run.sh` & `wild_code-0.3.0.dev0/run.sh`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 #Qwen/CodeQwen1.5-7B-Chat
 #gpt-3.5-turbo-0125
-#deepseek-coder-33b-instruct
+#deepseek-ai/deepseek-coder-33b-instruct
 #bigcode/starcoder2-15b-instruct-v0.1
 #bigcode/starcoder2-15b
 #gpt-4-turbo-2024-04-09
 BS=10
-MODEL=gpt-3.5-turbo-0125
 DATASET=wildcodebench
+# MODELS=(Qwen/CodeQwen1.5-7B-Chat)
+# BACKEND=vllm
+MODELS=(gpt-3.5-turbo-0125)
 BACKEND=openai
 TEMPS=(0)
 N_SAMPLESES=(1)
 
-for TEMP in ${TEMPS[@]}; do
-  for N_SAMPLES in ${N_SAMPLESES[@]}; do
-    rm -rf $MODEL-$DATASET-$TEMP-$N_SAMPLES.jsonl
-    wildcode.generate \
-        --model $MODEL \
-        --bs $BS \
-        --temperature $TEMP \
-        --n_samples $N_SAMPLES \
-        --resume \
-        --dataset $DATASET \
-        --backend $BACKEND
+for MODEL in ${MODELS[@]}; do
+  for TEMP in ${TEMPS[@]}; do
+    for N_SAMPLES in ${N_SAMPLESES[@]}; do
+      python -m wildcode.generate \
+          --tp 1 \
+          --model $MODEL \
+          --bs $BS \
+          --temperature $TEMP \
+          --n_samples $N_SAMPLES \
+          --resume \
+          --dataset $DATASET \
+          --backend $BACKEND
 
-    # check if "/" in the model name. I
-    if [[ $MODEL == *"/"* ]]; then
-      # split the model name by "/", first part is the organization name, second part is the model name
-      ORG=$(echo $MODEL | cut -d'/' -f1)
-      MODEL=$(echo $MODEL | cut -d'/' -f2)
-      MODEL=$ORG--$MODEL
-    fi
+      if [[ $MODEL == *"/"* ]]; then
+        ORG=$(echo $MODEL | cut -d'/' -f1)
+        MODEL=$(echo $MODEL | cut -d'/' -f2)
+        MODEL=$ORG--$MODEL
+      fi
 
-    SAMPLE_FILE=$MODEL--$DATASET--$BACKEND-$TEMP-$N_SAMPLES.jsonl
-    wildcode.sanitize --samples $SAMPLE_FILE
-    wildcode.evaluate --dataset $DATASET --samples $MODEL--$DATASET--$BACKEND-$TEMP-$N_SAMPLES-sanitized.jsonl
-    wildcode.inspect --dataset $DATASET --eval-results $MODEL-$DATASET-$TEMP-$N_SAMPLES-sanitized_eval_results.json --in-place
+      SAMPLE_FILE=$MODEL--$DATASET--$BACKEND-$TEMP-$N_SAMPLES.jsonl
+      python -m wildcode.sanitize --samples $SAMPLE_FILE
+      rm -rf $MODEL--$DATASET--$BACKEND-$TEMP-$N_SAMPLES-sanitized_eval_results.json
+      python -m wildcode.evaluate --dataset $DATASET --samples $MODEL--$DATASET--$BACKEND-$TEMP-$N_SAMPLES-sanitized.jsonl
+      # python -m wildcode.inspect --dataset $DATASET --eval-results $MODEL-$DATASET-$TEMP-$N_SAMPLES-sanitized_eval_results.json --in-place
+    done
   done
 done
```

### Comparing `wild_code-0.1.0.dev735/setup.cfg` & `wild_code-0.3.0.dev0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,21 @@
 	multipledispatch>=0.6.0
 	appdirs>=1.4.4
 	numpy>=1.19.5
 	tqdm>=4.56.0
 	termcolor>=2.0.0
 	fire>=0.6.0
 	openai>=1.11.1
+	openai
+	rich
+	accelerate
+	vllm
+	anthropic
+	mistralai
+	stop-sequencer
 
 [options.entry_points]
 console_scripts = 
 	wildcode.evaluate = wildcode.evaluate:main
 	wildcode.sanitize = wildcode.sanitize:main
 	wildcode.syncheck = wildcode.syncheck:main
 	wildcode.legacy_sanitize = wildcode.legacy_sanitize:main
```

### Comparing `wild_code-0.1.0.dev735/tests/test_legacy_sanitizer.py` & `wild_code-0.3.0.dev0/tests/test_legacy_sanitizer.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.1.0.dev735/tests/test_treesitter_sanitizer.py` & `wild_code-0.3.0.dev0/tests/test_treesitter_sanitizer.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.1.0.dev735/wild_code.egg-info/PKG-INFO` & `wild_code-0.3.0.dev0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wild-code
-Version: 0.1.0.dev735
+Version: 0.3.0.dev0
 Summary: "WildCode: A minimal viable package to evaluate code generation with realistic constraints in the wild"
 Home-page: https://github.com/bigcode-project/wild-code
 License: Apache-2.0
 Platform: any
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -16,31 +16,49 @@
 Requires-Dist: multipledispatch>=0.6.0
 Requires-Dist: appdirs>=1.4.4
 Requires-Dist: numpy>=1.19.5
 Requires-Dist: tqdm>=4.56.0
 Requires-Dist: termcolor>=2.0.0
 Requires-Dist: fire>=0.6.0
 Requires-Dist: openai>=1.11.1
+Requires-Dist: openai
+Requires-Dist: rich
+Requires-Dist: accelerate
+Requires-Dist: vllm
+Requires-Dist: anthropic
+Requires-Dist: mistralai
+Requires-Dist: stop-sequencer
 Provides-Extra: perf
 Requires-Dist: Pympler>=1.0.1; extra == "perf"
 Requires-Dist: rich>=12.3.0; extra == "perf"
 Requires-Dist: tree_sitter_languages>=1.10.2; extra == "perf"
 
 # 🌳WildCodeBench
 
 > [!WARNING] 
 > The project is under active development. Please check back later for more updates.
 
 > [!WARNING]
-> WildCode framework currently only supports the Code2Code generation task. We are working on adding the NL2Code task based on NL instructions.
+> Please use WildCode with caution. Different from [EvalPlus](https://github.com/evalplus/evalplus), WildCode has a much less constrained execution environment to support tasks with diverse library dependencies. This may lead to security risks. We recommend using a sandbox such as [Docker](https://docs.docker.com/get-docker/) to run the evaluation.
+
+> [!WARNING]
+> WildCode framework currently only supports the Code2Code generation task. We are working on adding the NL2Code task.
+
+<p align="center">
+    <a href="https://pypi.org/project/wild-code/"><img src="https://img.shields.io/pypi/v/wild-code?color=g"></a>
+    <a href="https://hub.docker.com/r/terryzho/wildcode" title="Docker"><img src="https://img.shields.io/docker/image-size/terryzho/wildcode"></a>
+    <a href="https://github.com/evalplus/evalplus/blob/master/LICENSE"><img src="https://img.shields.io/pypi/l/wild-code"></a>
+</p>
 
 <p align="center">
+    <a href="#-about">🌳About</a> •
     <a href="#-quick-start">🔥Quick Start</a> •
     <a href="#-llm-generated-code">💻LLM code</a> •
-    <a href="#-useful-tools">🔨Tools</a> •
+    <a href="#-failure-inspection">🔍Failure inspection</a> •
+    <a href="#-known-issues">🐞Known issues</a> •
     <a href="#-citation">📜Citation</a> •
     <a href="#-acknowledgement">🙏Acknowledgement</a>
 </p>
 
 ## About
 
 ### WildCodeBench
@@ -54,14 +72,19 @@
 ### Why WildCode?
 
 WildCode is a rigorous evaluation framework for LLM4Code, with:
 
 * ✨ **Precise evaluation & ranking**: See [our leaderboard](https://wildcodebench.github.io/leaderboard.html) for latest LLM rankings before & after rigorous evaluation.
 * ✨ **Pre-generated samples**: WildCode accelerates code intelligence research by open-sourcing [LLM-generated samples](#-LLM-generated-code) for various models -- no need to re-run the expensive benchmarks!
 
+### Main Differences from EvalPlus
+
+We inherit the design of the EvalPlus framework, which is a flexible and extensible evaluation framework for code generation tasks. However, WildCode has the following differences:
+* Execution Environment: The execution environment in WildCode is less bounded than EvalPlus to support tasks with diverse library dependencies.
+* Test Evaluation: WildCode relies on `unittest` for evaluating the generated code, which is more suitable for the test harness in WildCodeBench.
 
 ## 🔥 Quick Start
 
 > [!Tip]
 >
 > WildCode ❤️ [bigcode-evaluation-harness](https://github.com/bigcode-project/bigcode-evaluation-harness)!
 > WildCodeBench will be integrated to bigcode-evaluation-harness, and you can also run it there!
@@ -91,15 +114,15 @@
 export PYTHONPATH=$PYTHONPATH:$(pwd)
 pip install -e .
 ```
 
 </div>
 </details>
 
-### Code generation
+### Code Generation
 
 To generate code samples from a model, you can use the following command:
 
 ```shell
 wildcode.generate --model [model_name] --dataset wildcodebench --greedy --bs [bs] --temperature [temp] --n_samples [n_samples] --resume --backend [vllm|hf|openai]
 ```
 The generated code samples will be stored in a file named `[model_name]--wildcodebench--[backend]-[temp]-[n_samples].jsonl`.
@@ -121,15 +144,15 @@
 >
 > **Expected Schema of `[model_name]--wildcodebench--[backend]-[temp]-[n_samples].jsonl`**
 >
 > 1. `task_id`: Task ID, which are the keys of `get_[human_eval|mbpp]_plus()`
 > 2. `solution` (optional): Self-contained solution (usually including the prompt)
 >    * Example: `{"task_id": "HumanEval/?", "solution": "def f():\n    return 1"}`
 
-### Code post-processing
+### Code Post-processing
 
 LLM-generated text may not be compilable code for including natural language lines or incomplete extra code.
 We provide a tool namely `wildcode.sanitize` to clean up the code:
 
 ```shell
 # 💡 If you are storing codes in jsonl:
 wildcode.sanitize --samples samples.jsonl
@@ -153,19 +176,20 @@
 wildcode.syncheck --samples /path/to/vicuna-[??]b_temp_[??] --dataset [wildcodebench]
 ```
 
 </div>
 </details>
 
 
-### Code evaluation
+### Code Evaluation
 
 You are strongly recommended to use a sandbox such as [docker](https://docs.docker.com/get-docker/):
 
 ```shell
+docker run -v $(pwd):/app terryzho/wildcode:latest --dataset [wildcodebench] --samples samples.jsonl
 ```
 
 ...Or if you want to try it locally regardless of the risks ⚠️:
 
 First, install the dependencies for WildCodeBench:
 
 ```shell
@@ -196,19 +220,19 @@
 </div>
 </details>
 
 The output should be like (below is GPT-4 greedy decoding example):
 
 ```
 Asserting the groundtruth...
-Expected outputs computed in 2400.0 seconds
+Expected outputs computed in 1200.0 seconds
 Reading samples...
-964it [30:04, 37.79it/s]
+1047it [00:00, 1901.64it/s]
 Evaluating samples...
-100%|██████████████████████████████████████████| 964/964 [00:03<00:00, 44.75it/s]
+100%|██████████████████████████████████████████| 1047/1047 [19:53<00:00, 6.75it/s]
 Base
 {'pass@1': 0.548}
 ```
 
 - `Base` is the `pass@k` for the original HumanEval
 - The "k" includes `[1, 10, 100]` where k values `<=` the sample size will be used
 - A cache file named like `samples_eval_results.jsonl` will be cached. Remove it to re-run the evaluation
@@ -227,28 +251,28 @@
 </details>
 
 ## Failure Inspection
 
 You can inspect the failed samples by using the following command:
 
 ```shell
-wildcode.inspect --dataset $DATASET --eval-results sample-sanitized_eval_results.json --in-place
+wildcode.inspect --dataset [wildcodebench] --eval-results sample-sanitized_eval_results.json --in-place
 ```
 
-## Full Script
+## Full script
 
 We provide a sample script to run the full pipeline:
 
 ```shell
 bash run.sh
 ```
 
-## 💻 LLM-generated code
+## 💻 LLM-generated Code
 
-We share pre-generated code samples from LLMs we have [evaluated](https://wildcodebench.github.io/leaderboard.html):
+We will share pre-generated code samples from LLMs we have [evaluated](https://wildcodebench.github.io/leaderboard.html):
 
 ## Known Issues
 
 - [ ] We notice that some tasks heavily use memory for scientific modeling during testing. It will lead to timeout issues on some machines. If you get an error message like `Check failed: ret == 0 (11 vs. 0)Thread creation via pthread_create() failed.` in Tensorflow, it is very likely due to the memory issue. Try to allocate more memory to the process or reduce the number of parallel processes.
 
 ## 📜 Citation
```

#### html2text {}

```diff
@@ -1,26 +1,35 @@
-Metadata-Version: 2.1 Name: wild-code Version: 0.1.0.dev735 Summary: "WildCode:
-A minimal viable package to evaluate code generation with realistic constraints
+Metadata-Version: 2.1 Name: wild-code Version: 0.3.0.dev0 Summary: "WildCode: A
+minimal viable package to evaluate code generation with realistic constraints
 in the wild" Home-page: https://github.com/bigcode-project/wild-code License:
 Apache-2.0 Platform: any Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Requires-Python: >=3.8 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: wget>=3.2 Requires-
 Dist: tempdir>=0.7.1 Requires-Dist: multipledispatch>=0.6.0 Requires-Dist:
 appdirs>=1.4.4 Requires-Dist: numpy>=1.19.5 Requires-Dist: tqdm>=4.56.0
 Requires-Dist: termcolor>=2.0.0 Requires-Dist: fire>=0.6.0 Requires-Dist:
-openai>=1.11.1 Provides-Extra: perf Requires-Dist: Pympler>=1.0.1; extra ==
-"perf" Requires-Dist: rich>=12.3.0; extra == "perf" Requires-Dist:
-tree_sitter_languages>=1.10.2; extra == "perf" # ð³WildCodeBench > [!WARNING]
-> The project is under active development. Please check back later for more
-updates. > [!WARNING] > WildCode framework currently only supports the
-Code2Code generation task. We are working on adding the NL2Code task based on
-NL instructions.
-      _ð___¥_Q_u_i_c_k_ _S_t_a_r_t â¢ _ð___»_L_L_M_ _c_o_d_e â¢ _ð___¨_T_o_o_l_s â¢ _ð____C_i_t_a_t_i_o_n â¢
-                              _ð____A_c_k_n_o_w_l_e_d_g_e_m_e_n_t
+openai>=1.11.1 Requires-Dist: openai Requires-Dist: rich Requires-Dist:
+accelerate Requires-Dist: vllm Requires-Dist: anthropic Requires-Dist:
+mistralai Requires-Dist: stop-sequencer Provides-Extra: perf Requires-Dist:
+Pympler>=1.0.1; extra == "perf" Requires-Dist: rich>=12.3.0; extra == "perf"
+Requires-Dist: tree_sitter_languages>=1.10.2; extra == "perf" #
+ð³WildCodeBench > [!WARNING] > The project is under active development.
+Please check back later for more updates. > [!WARNING] > Please use WildCode
+with caution. Different from [EvalPlus](https://github.com/evalplus/evalplus),
+WildCode has a much less constrained execution environment to support tasks
+with diverse library dependencies. This may lead to security risks. We
+recommend using a sandbox such as [Docker](https://docs.docker.com/get-docker/
+) to run the evaluation. > [!WARNING] > WildCode framework currently only
+supports the Code2Code generation task. We are working on adding the NL2Code
+task.
+   _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_w_i_l_d_-_c_o_d_e_?_c_o_l_o_r_=_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+ _d_o_c_k_e_r_/_i_m_a_g_e_-_s_i_z_e_/_t_e_r_r_y_z_h_o_/_w_i_l_d_c_o_d_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_l_/_w_i_l_d_-_c_o_d_e_]
+ _ð___³_A_b_o_u_t â¢ _ð___¥_Q_u_i_c_k_ _S_t_a_r_t â¢ _ð___»_L_L_M_ _c_o_d_e â¢ _ð____F_a_i_l_u_r_e_ _i_n_s_p_e_c_t_i_o_n â¢
+           _ð____K_n_o_w_n_ _i_s_s_u_e_s â¢ _ð____C_i_t_a_t_i_o_n â¢ _ð____A_c_k_n_o_w_l_e_d_g_e_m_e_n_t
 ## About ### WildCodeBench WildCodeBench is a rigorous benchmark for code
 generation with realistic constraints in the wild. It aims to evaluate the true
 programming capabilities of large language models (LLMs) in a more realistic
 setting. The benchmark is designed for HumanEval-like function-level code
 generation tasks, but with much more fine-grained descriptions and diverse tool
 use. ### WildCode To facilitate the evaluation of LLMs on WildCodeBench, we
 provide a Python package `wild-code` that includes the dataset, generation
@@ -28,41 +37,48 @@
 (https://github.com/evalplus/evalplus) framework, which is a flexible and
 extensible evaluation framework for code generation tasks. ### Why WildCode?
 WildCode is a rigorous evaluation framework for LLM4Code, with: * â¨ **Precise
 evaluation & ranking**: See [our leaderboard](https://wildcodebench.github.io/
 leaderboard.html) for latest LLM rankings before & after rigorous evaluation. *
 â¨ **Pre-generated samples**: WildCode accelerates code intelligence research
 by open-sourcing [LLM-generated samples](#-LLM-generated-code) for various
-models -- no need to re-run the expensive benchmarks! ## ð¥ Quick Start >
-[!Tip] > > WildCode â¤ï¸ [bigcode-evaluation-harness](https://github.com/
-bigcode-project/bigcode-evaluation-harness)! > WildCodeBench will be integrated
-to bigcode-evaluation-harness, and you can also run it there! To get started,
-please first set up the environment: ```shell pip install wild-code --upgrade
-``` â¬ Install nightly version :: click to expand ::
+models -- no need to re-run the expensive benchmarks! ### Main Differences from
+EvalPlus We inherit the design of the EvalPlus framework, which is a flexible
+and extensible evaluation framework for code generation tasks. However,
+WildCode has the following differences: * Execution Environment: The execution
+environment in WildCode is less bounded than EvalPlus to support tasks with
+diverse library dependencies. * Test Evaluation: WildCode relies on `unittest`
+for evaluating the generated code, which is more suitable for the test harness
+in WildCodeBench. ## ð¥ Quick Start > [!Tip] > > WildCode â¤ï¸ [bigcode-
+evaluation-harness](https://github.com/bigcode-project/bigcode-evaluation-
+harness)! > WildCodeBench will be integrated to bigcode-evaluation-harness, and
+you can also run it there! To get started, please first set up the environment:
+```shell pip install wild-code --upgrade ``` â¬ Install nightly version ::
+click to expand ::
 ```shell pip install "git+https://github.com/bigcode-project/wild-code.git" --
 upgrade ```
 â¬ Using WildCode as a local repo? :: click to expand ::
 ```shell git clone https://github.com/bigcode-project/wild-code.git cd wild-
 code export PYTHONPATH=$PYTHONPATH:$(pwd) pip install -e . ```
-### Code generation To generate code samples from a model, you can use the
+### Code Generation To generate code samples from a model, you can use the
 following command: ```shell wildcode.generate --model [model_name] --dataset
 wildcodebench --greedy --bs [bs] --temperature [temp] --n_samples [n_samples] -
 -resume --backend [vllm|hf|openai] ``` The generated code samples will be
 stored in a file named `[model_name]--wildcodebench--[backend]-[temp]-
 [n_samples].jsonl`. ð¤ Structure of `problem`? :: click to expand ::
 * `task_id` is the identifier string for the task * `entry_point` is the name
 of the function * `prompt` is the function signature with docstring *
 `instruction` is the instruction for the task completion + `canonical_solution`
 is the ground-truth implementation (re-implemented to fix bugs in HumanEval) +
 `test` is the `unittest` test case
 > [!Note] > > **Expected Schema of `[model_name]--wildcodebench--[backend]-
 [temp]-[n_samples].jsonl`** > > 1. `task_id`: Task ID, which are the keys of
 `get_[human_eval|mbpp]_plus()` > 2. `solution` (optional): Self-contained
 solution (usually including the prompt) > * Example: `{"task_id": "HumanEval/
-?", "solution": "def f():\n return 1"}` ### Code post-processing LLM-generated
+?", "solution": "def f():\n return 1"}` ### Code Post-processing LLM-generated
 text may not be compilable code for including natural language lines or
 incomplete extra code. We provide a tool namely `wildcode.sanitize` to clean up
 the code: ```shell # ð¡ If you are storing codes in jsonl: wildcode.sanitize
 --samples samples.jsonl # Sanitized code will be produced to `samples-
 sanitized.jsonl` # ð¡ If you are storing codes in directories:
 wildcode.sanitize --samples /path/to/vicuna-[??]b_temp_[??] # Sanitized code
 will be produced to `/path/to/vicuna-[??]b_temp_[??]-sanitized` ``` ð
@@ -70,48 +86,50 @@
 To double-check the post-processing results, you can use `wildcode.syncheck` to
 check the code validity before and after sanitization, which will print
 erroneous code snippets and why they are wrong: ```shell # ð¡ If you are
 storing codes in jsonl: wildcode.syncheck --samples samples.jsonl --dataset
 [wildcodebench] # ð¡ If you are storing codes in directories:
 wildcode.syncheck --samples /path/to/vicuna-[??]b_temp_[??] --dataset
 [wildcodebench] ```
-### Code evaluation You are strongly recommended to use a sandbox such as
-[docker](https://docs.docker.com/get-docker/): ```shell ``` ...Or if you want
-to try it locally regardless of the risks â ï¸: First, install the
-dependencies for WildCodeBench: ```shell pip install -r requirements-
-wildcodebench.txt ``` Then, run the evaluation: ```shell wildcode.evaluate --
-dataset [wildcodebench] --samples samples.jsonl ``` > [!Tip] > > Do you use a
-very slow machine? > > LLM solutions are regarded as **failed** on timeout (and
-OOM etc.). > Specifically, we set the dynamic timeout based on the ground-truth
-solution's runtime. > > Additionally, you are **NOT** encouraged to make your
-test-bed over stressed while running evaluation. > For example, using `--
-parallel 64` on a 4-core machine or doing something else during evaluation are
-bad ideas... â¨ï¸ More command-line flags :: click to expand ::
+### Code Evaluation You are strongly recommended to use a sandbox such as
+[docker](https://docs.docker.com/get-docker/): ```shell docker run -v $(pwd):/
+app terryzho/wildcode:latest --dataset [wildcodebench] --samples samples.jsonl
+``` ...Or if you want to try it locally regardless of the risks â ï¸: First,
+install the dependencies for WildCodeBench: ```shell pip install -
+r requirements-wildcodebench.txt ``` Then, run the evaluation: ```shell
+wildcode.evaluate --dataset [wildcodebench] --samples samples.jsonl ``` >
+[!Tip] > > Do you use a very slow machine? > > LLM solutions are regarded as
+**failed** on timeout (and OOM etc.). > Specifically, we set the dynamic
+timeout based on the ground-truth solution's runtime. > > Additionally, you are
+**NOT** encouraged to make your test-bed over stressed while running
+evaluation. > For example, using `--parallel 64` on a 4-core machine or doing
+something else during evaluation are bad ideas... â¨ï¸ More command-line
+flags :: click to expand ::
 * `--parallel`: by default half of the cores
 The output should be like (below is GPT-4 greedy decoding example): ```
-Asserting the groundtruth... Expected outputs computed in 2400.0 seconds
-Reading samples... 964it [30:04, 37.79it/s] Evaluating samples...
+Asserting the groundtruth... Expected outputs computed in 1200.0 seconds
+Reading samples... 1047it [00:00, 1901.64it/s] Evaluating samples...
 100%|ââââââââââââââââââââââââââââââââââââââââââ|
-964/964 [00:03<00:00, 44.75it/s] Base {'pass@1': 0.548} ``` - `Base` is the
+1047/1047 [19:53<00:00, 6.75it/s] Base {'pass@1': 0.548} ``` - `Base` is the
 `pass@k` for the original HumanEval - The "k" includes `[1, 10, 100]` where k
 values `<=` the sample size will be used - A cache file named like
 `samples_eval_results.jsonl` will be cached. Remove it to re-run the evaluation
 ð¤ How long it would take? :: click to expand ::
 If you do greedy decoding where there is only one sample for each task, the
 evaluation should take just a few seconds. When running 1 sample x 964 tasks x
 all tests, it can take around ??-?? minutes by using `--parallel 64` and `--
 test-details`. Here are some tips to speed up the evaluation: * Use `--parallel
 $(nproc)` * Use our pre-evaluated results (see [LLM-generated code](#-LLM-
 generated-code))
 ## Failure Inspection You can inspect the failed samples by using the following
-command: ```shell wildcode.inspect --dataset $DATASET --eval-results sample-
-sanitized_eval_results.json --in-place ``` ## Full Script We provide a sample
-script to run the full pipeline: ```shell bash run.sh ``` ## ð» LLM-generated
-code We share pre-generated code samples from LLMs we have [evaluated](https://
-wildcodebench.github.io/leaderboard.html): ## Known Issues - [ ] We notice that
-some tasks heavily use memory for scientific modeling during testing. It will
-lead to timeout issues on some machines. If you get an error message like
-`Check failed: ret == 0 (11 vs. 0)Thread creation via pthread_create() failed.`
-in Tensorflow, it is very likely due to the memory issue. Try to allocate more
-memory to the process or reduce the number of parallel processes. ## ð
-Citation ```bibtex ``` ## ð Acknowledgement - [EvalPlus](https://github.com/
-evalplus/evalplus)
+command: ```shell wildcode.inspect --dataset [wildcodebench] --eval-results
+sample-sanitized_eval_results.json --in-place ``` ## Full script We provide a
+sample script to run the full pipeline: ```shell bash run.sh ``` ## ð» LLM-
+generated Code We will share pre-generated code samples from LLMs we have
+[evaluated](https://wildcodebench.github.io/leaderboard.html): ## Known Issues
+- [ ] We notice that some tasks heavily use memory for scientific modeling
+during testing. It will lead to timeout issues on some machines. If you get an
+error message like `Check failed: ret == 0 (11 vs. 0)Thread creation via
+pthread_create() failed.` in Tensorflow, it is very likely due to the memory
+issue. Try to allocate more memory to the process or reduce the number of
+parallel processes. ## ð Citation ```bibtex ``` ## ð Acknowledgement -
+[EvalPlus](https://github.com/evalplus/evalplus)
```

### Comparing `wild_code-0.1.0.dev735/wild_code.egg-info/SOURCES.txt` & `wild_code-0.3.0.dev0/wild_code.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 CITATION.cff
 Dockerfile
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 release.sh
-requirements-wildcodebench.txt
 requirements.txt
 run.sh
 setup.cfg
 .github/ISSUE_TEMPLATE/buggy_contract.yml
 .github/ISSUE_TEMPLATE/buggy_test.yml
 .github/ISSUE_TEMPLATE/config.yml
 .github/ISSUE_TEMPLATE/model_eval_request.yml
```

### Comparing `wild_code-0.1.0.dev735/wildcode/data/utils.py` & `wild_code-0.3.0.dev0/wildcode/data/utils.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.1.0.dev735/wildcode/data/wildcodebench.py` & `wild_code-0.3.0.dev0/wildcode/data/wildcodebench.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         "prompt" is the prompt to be used for the task (function signature with docstrings).
         "test" is test-cases wrapped in a `check` function.
         "entry_point" is the name of the function.
     """
     # Check if open eval file exists in CACHE_DIR
     wild_code_bench_path = os.path.join(CACHE_DIR, "WildCodeBench.jsonl")
     make_cache(
-        "https://github.com/bigcode-project/open-eval/raw/main/data/open-eval.jsonl.gz",
+        "https://github.com/bigcode-project/wild-code-bench-annotation/raw/main/data/wild-code-bench.jsonl.gz",
         wild_code_bench_path,
     )
     print(wild_code_bench_path)
     wild_code_bench = open(wild_code_bench_path, "r").read().split("\n")
     wild_code_bench = [json.loads(line) for line in wild_code_bench if line]
 
     return {task["task_id"]: task for task in wild_code_bench}
```

### Comparing `wild_code-0.1.0.dev735/wildcode/eval/__init__.py` & `wild_code-0.3.0.dev0/wildcode/eval/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 # THE SOFTWARE.
 
 import itertools
 import multiprocessing
 import os
 import sys
 import time
+import types
 import unittest
 from multiprocessing import Array, Value, Manager
 from typing import Any, Dict, List, Tuple, Union
 
 import numpy as np
 
 from wildcode.eval._special_oracle import (
@@ -121,29 +122,34 @@
         rmtree = shutil.rmtree
         rmdir = os.rmdir
         chdir = os.chdir
         # Disable functionalities that can make destructive changes to the test.
         # allow only 32GB memory usage
         maximum_memory_bytes = 32 * 1024 * 1024 * 1024
         reliability_guard(maximum_memory_bytes=maximum_memory_bytes)
-        exec_globals = {
+        module_name = "__test__"
+        new_module = types.ModuleType(module_name)
+        # Set necessary attributes for the module
+        new_module.__dict__.update({
             '__builtins__': builtins,
-            '__name__': '__main__',
-            '__file__': '',  # you might specify the script's intended file path if needed
+            '__file__': f"{module_name}.py",
             '__package__': None,
             '__doc__': None,
             'sys': sys,
             'os': os,
             'environ': os.environ,
-        }
+        })
+
         try:
-            code = code + "\n\n" + test_code
+            full_code = code + "\n" + test_code
+
             with swallow_io():
-                exec(code, exec_globals)
-                TestCases = exec_globals['TestCases']
+                exec(compile(full_code, f"{module_name}.py", 'exec'), new_module.__dict__)
+                sys.modules[module_name] = new_module
+                TestCases = getattr(new_module, 'TestCases')
                 loader = unittest.TestLoader()
                 suite = loader.loadTestsFromTestCase(TestCases)
                 test_result = unittest.TestResult()
                 start_time = time.time()
                 with time_limit(timeout):
                     suite.run(test_result)
```

### Comparing `wild_code-0.1.0.dev735/wildcode/evaluate.py` & `wild_code-0.3.0.dev0/wildcode/evaluate.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,28 +30,31 @@
 from wildcode.gen.util import trusted_exec
 
 # 1st item: the status
 # 2nd item (optional): the detailed pass/fail boolean for each input
 Result = Tuple[str, List[bool]]
 
 
-def get_groundtruth(problems, hashcode):
+def get_groundtruth(problems, hashcode, check_gt_only):
     cache_file = os.path.join(CACHE_DIR, f"{hashcode}.pkl")
     if os.path.exists(cache_file):
-        print(f"Load from ground-truth from {cache_file}")
-        with open(cache_file, "rb") as f:
-            return pickle.load(f)
+        if check_gt_only:
+            os.remove(cache_file)
+        else:
+            print(f"Load from ground-truth from {cache_file}")
+            with open(cache_file, "rb") as f:
+                return pickle.load(f)
 
     os.makedirs(CACHE_DIR, exist_ok=True)
     print("\nAsserting the groundtruth...")
     tbegin = time.time()
     expected_time = {}
-    for task_id, problem in problems.items():
+    for task_id, problem in tqdm(problems.items()):
         expected_time[task_id] = trusted_exec(
-            problem["prompt"] + "\n" + problem["canonical_solution"],
+            problem["prompt"] + "\n" + problem["clean_canonical_solution"],
             problem["test"],
             problem["entry_point"],
         )
     print(f"Expected outputs computed in {time.time() - tbegin:.2f}s")
     
     with open(cache_file, "wb") as f:
         pickle.dump(expected_time, f)
@@ -72,29 +75,32 @@
         "task_id": problem["task_id"],
         "_identifier": identifier,
         "solution": solution,
     }
     ret["base"] = untrusted_check(
         dataset,
         solution,
-        # problem["prompt"] + "\n" + problem["canonical_solution"],
         problem["test"],
         problem["entry_point"],
         min_time_limit,
         gt_time_limit
     )
     return ret
 
 
 def evaluate(flags):
     if flags.parallel is None:
         n_workers = max(1, multiprocessing.cpu_count() // 2)
     else:
         n_workers = flags.parallel
 
+    if flags.check_gt_only:
+        # bypass the samples
+        flags.samples = "__dummy__.jsonl"
+        
     if os.path.isdir(flags.samples):
         result_path = os.path.join(flags.samples, "eval_results.json")
     else:
         assert flags.samples.endswith(".jsonl")
         result_path = flags.samples.replace(".jsonl", "_eval_results.json")
 
     if os.path.isfile(result_path):
@@ -102,17 +108,20 @@
         with open(result_path, "r") as f:
             results = json.load(f)
 
         results = compatible_eval_result(results)
     else:
         if flags.dataset == "wildcodebench":
             problems = get_wild_code_bench()
-            dataset_hash = get_wild_code_bench_hash()            
-            expected_time = get_groundtruth(problems, dataset_hash)
-            
+            dataset_hash = get_wild_code_bench_hash()       
+            expected_time = get_groundtruth(problems, dataset_hash, flags.check_gt_only)
+        
+        if flags.check_gt_only:
+            return
+        
         results = {
             "date": datetime.now().strftime("%Y-%m-%d %H:%M"),
             "eval": {},
         }
 
         with ProcessPoolExecutor(max_workers=n_workers) as executor:
             futures = []
@@ -140,15 +149,16 @@
                     flags.dataset,
                     completion_id[task_id],
                     problems[task_id],
                     solution,
                     # problems[task_id]["canonical_solution"],
                     sample["_identifier"],
                     flags.min_time_limit,
-                    expected_time[task_id],
+                    # expected_time[task_id],
+                    120
                 )
                 futures.append(executor.submit(check_correctness, *args))
                 completion_id[task_id] += 1
                 n_samples += 1
 
             assert n_samples == len(remainings), "Missing problems in unfinished"
             assert len(completion_id) == len(problems), "Missing problems in samples"
@@ -229,18 +239,15 @@
     parser.add_argument(
         "--dataset", required=True, type=str, choices=["wildcodebench"]
     )
     parser.add_argument("--samples", required=True, type=str)
     parser.add_argument("--parallel", default=None, type=int)
     parser.add_argument("--min-time-limit", default=1, type=float)
     parser.add_argument(
-        "--noextreme", action="store_true", help="Omit extreme test inputs"
-    )
-    parser.add_argument(
-        "--check-gt", action="store_true", help="Check the groundtruth"
+        "--check-gt-only", action="store_true", help="Check the groundtruth"
     )
     args = parser.parse_args()
 
     evaluate(args)
 
 
 if __name__ == "__main__":
```

### Comparing `wild_code-0.1.0.dev735/wildcode/gen/__init__.py` & `wild_code-0.3.0.dev0/wildcode/gen/__init__.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.1.0.dev735/wildcode/gen/util/__init__.py` & `wild_code-0.3.0.dev0/wildcode/gen/util/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,54 @@
 import time
 import os
 import sys
+import types
 import unittest
 import builtins
 
 from copy import deepcopy
 
 from wildcode.eval.utils import time_limit, swallow_io
+from wildcode.eval.utils import create_tempdir
 
-
-def trusted_exec(code, test_code, entry_point):
+def trusted_exec(code, test_code, task_id):
     """Execute trusted code in place."""
-    # Example of setting environment variables
-    # Load other necessary environment settings
-    exec_globals = {
-        '__builtins__': builtins,
-        '__name__': '__main__',
-        '__file__': 'test.py',
-        '__package__': None,
-        '__doc__': None,
-        'sys': sys,
-        'os': os,
-        'environ': os.environ,
-    }
     
-    code = code + "\n" + test_code
-    exec(code, exec_globals)
-    TestCases = exec_globals['TestCases']
-    loader = unittest.TestLoader()
-    suite = loader.loadTestsFromTestCase(TestCases)
-    test_result = unittest.TestResult()
-    start = time.time()
-    with swallow_io():
-        suite.run(test_result)
-    # assert len(test_result.failures+test_result.errors) == 0, "Test failed."
-    return time.time() - start
+    with create_tempdir():
+        module_name = "__test__"
+        new_module = types.ModuleType(module_name)
+        
+        # Set necessary attributes for the module
+        new_module.__dict__.update({
+            '__builtins__': builtins,
+            '__file__': f"{module_name}.py",
+            '__package__': None,
+            '__doc__': None,
+            'sys': sys,
+            'os': os,
+            'environ': os.environ,
+        })
+
+        # Combine the user code and the test code
+        full_code = code + "\n" + test_code
+
+        # Compile and execute the combined code within the new module
+        exec(compile(full_code, f"{module_name}.py", 'exec'), new_module.__dict__)
+        sys.modules[module_name] = new_module
+        TestCases = getattr(new_module, 'TestCases')
+        loader = unittest.TestLoader()
+        suite = loader.loadTestsFromTestCase(TestCases)
+        test_result = unittest.TestResult()
+        start = time.time()
+        with swallow_io():
+            suite.run(test_result)
+        assert len(test_result.failures+test_result.errors) == 0, f"{task_id} failed"
+        return time.time() - start
 
-def trusted_check_exec(code, inputs, entry_point):
+def trusted_check_exec(code, inputs):
     """Check trusted_exec success."""
     try:
-        with time_limit(seconds=1.0):
-            trusted_exec(code, inputs, entry_point)
+        with time_limit(seconds=120):
+            trusted_exec(code, inputs)
     except Exception:
         return False
     return True
```

### Comparing `wild_code-0.1.0.dev735/wildcode/gen/util/anthropic_request.py` & `wild_code-0.3.0.dev0/wildcode/gen/util/anthropic_request.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.1.0.dev735/wildcode/gen/util/openai_request.py` & `wild_code-0.3.0.dev0/wildcode/gen/util/openai_request.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.1.0.dev735/wildcode/generate.py` & `wild_code-0.3.0.dev0/wildcode/generate.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.1.0.dev735/wildcode/inspect.py` & `wild_code-0.3.0.dev0/wildcode/inspect.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.1.0.dev735/wildcode/lecacy_sanitize.py` & `wild_code-0.3.0.dev0/wildcode/lecacy_sanitize.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.1.0.dev735/wildcode/model.py` & `wild_code-0.3.0.dev0/wildcode/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
 class DecoderBase(ABC):
     def __init__(
         self,
         name: str,
         batch_size: int = 1,
         temperature: float = 0.8,
-        max_new_tokens: int = 512,
+        max_new_tokens: int = 1280,
         dtype: str = "bfloat16",  # default
         trust_remote_code: bool = False,
     ) -> None:
         print("Initializing a decoder model: {} ...".format(name))
         self.name = name
         self.batch_size = batch_size
         self.temperature = temperature
```

### Comparing `wild_code-0.1.0.dev735/wildcode/sanitize.py` & `wild_code-0.3.0.dev0/wildcode/sanitize.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Post-processing LLM-generated Python code implemented using tree-sitter."""
 
 import os
 import ast
-import astunparse
 import pathlib
 from typing import Dict, Generator, List, Optional, Set, Tuple
 
 from tqdm import tqdm
 from tree_sitter import Node
 from tree_sitter_languages import get_parser
 
@@ -163,18 +162,24 @@
         name, node = pair
         if entrypoint and not (name in reacheable):
             continue
         sanitized_output += code_bytes[node.start_byte : node.end_byte] + b"\n"
         
     sanitized_output = sanitized_output[:-1].decode("utf8")
     
+    # ad-hoc approach to remove unnecessary lines, but it works
     lines = sanitized_output.splitlines()
+    outer_lines = []
     for i in range(len(lines) - 1, -1, -1):
         if lines[i].startswith(" "):
-            return "\n".join(lines[:i+1])
+            break
+        if not lines[i].startswith(" ") and entrypoint in lines[i]:
+            outer_lines.append(i)
+    if outer_lines:
+        sanitized_output = "\n".join(lines[: outer_lines[-1]])
     return sanitized_output
 
 
 def script(
     samples: str, inplace: bool = False, debug_task: str = None
 ):
     # task_id -> entry_point
```

### Comparing `wild_code-0.1.0.dev735/wildcode/syncheck.py` & `wild_code-0.3.0.dev0/wildcode/syncheck.py`

 * *Files identical despite different names*

