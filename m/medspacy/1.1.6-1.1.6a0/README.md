# Comparing `tmp/medspacy-1.1.6.tar.gz` & `tmp/medspacy-1.1.6a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medspacy-1.1.6.tar", last modified: Fri May 10 15:23:10 2024, max compression
+gzip compressed data, was "medspacy-1.1.6a0.tar", last modified: Thu May  2 06:35:54 2024, max compression
```

## Comparing `medspacy-1.1.6.tar` & `medspacy-1.1.6a0.tar`

### file list

```diff
@@ -1,149 +1,149 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:10.972508 medspacy-1.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-10 15:23:06.000000 medspacy-1.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-05-10 15:23:10.968508 medspacy-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6654 2024-05-10 15:23:06.000000 medspacy-1.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:10.948508 medspacy-1.1.6/medspacy/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9481 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:10.964508 medspacy-1.1.6/medspacy/common/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/common/base_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     5859 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/common/medspacy_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     6700 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/common/regex_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     6151 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/common/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/components.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:10.964508 medspacy-1.1.6/medspacy/context/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13456 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/context/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/context/context_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    15026 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/context/context_modifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    11407 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/context/context_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/context/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/custom_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:10.964508 medspacy-1.1.6/medspacy/io/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/io/config_example.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/io/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/io/db_connect.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/io/db_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/io/db_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12075 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/io/doc_consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/io/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/ner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:10.968508 medspacy-1.1.6/medspacy/postprocess/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/postprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8673 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/postprocess/postprocessing_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/postprocess/postprocessing_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/postprocess/postprocessing_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/postprocess/postprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:10.968508 medspacy-1.1.6/medspacy/preprocess/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/preprocess/preprocessing_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/preprocess/preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:10.968508 medspacy-1.1.6/medspacy/section_detection/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/section_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/section_detection/section.py
--rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/section_detection/section_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    21792 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/section_detection/sectionizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/section_detection/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/sentence_splitting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:10.968508 medspacy-1.1.6/medspacy/target_matcher/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/target_matcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/target_matcher/concept_tagger.py
--rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/target_matcher/target_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/target_matcher/target_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     8550 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-05-10 15:23:06.000000 medspacy-1.1.6/medspacy/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:10.968508 medspacy-1.1.6/medspacy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-05-10 15:23:10.000000 medspacy-1.1.6/medspacy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9264 2024-05-10 15:23:10.000000 medspacy-1.1.6/medspacy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 15:23:10.000000 medspacy-1.1.6/medspacy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-10 15:23:10.000000 medspacy-1.1.6/medspacy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-10 15:23:10.000000 medspacy-1.1.6/medspacy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-10 15:23:06.000000 medspacy-1.1.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:10.968508 medspacy-1.1.6/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-10 15:23:06.000000 medspacy-1.1.6/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-10 15:23:06.000000 medspacy-1.1.6/requirements/requirements_tests.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:10.952508 medspacy-1.1.6/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    28435 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/context_rules.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:10.944507 medspacy-1.1.6/resources/quickumls/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:10.952508 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:10.952508 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/
--rw-r--r--   0 runner    (1001) docker     (127)    12288 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/cui.unqlite
--rw-r--r--   0 runner    (1001) docker     (127)    12288 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/semtypes.unqlite
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/database_backend.flag
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/language.flag
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/lowercase.flag
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/normalize-unicode.flag
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:10.956508 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/
--rw-r--r--   0 runner    (1001) docker     (127)     6116 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring
--rw-r--r--   0 runner    (1001) docker     (127)     6892 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:10.960508 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:10.960508 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/
--rw-r--r--   0 runner    (1001) docker     (127)    20480 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/cui.unqlite
--rw-r--r--   0 runner    (1001) docker     (127)    12288 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/semtypes.unqlite
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/database_backend.flag
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/language.flag
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/lowercase.flag
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/normalize-unicode.flag
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:10.964508 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring
--rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb
--rw-r--r--   0 runner    (1001) docker     (127)    23496 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/rush_rules.tsv
--rw-r--r--   0 runner    (1001) docker     (127)    12073 2024-05-10 15:23:06.000000 medspacy-1.1.6/resources/section_patterns.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 15:23:10.972508 medspacy-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-10 15:23:06.000000 medspacy-1.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:10.968508 medspacy-1.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-05-10 15:23:06.000000 medspacy-1.1.6/tests/test_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7324 2024-05-10 15:23:06.000000 medspacy-1.1.6/tests/test_medspacy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-05-10 15:23:06.000000 medspacy-1.1.6/tests/test_notebooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:54.783316 medspacy-1.1.6a0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8414 2024-05-02 06:35:54.783316 medspacy-1.1.6a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6654 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:54.763316 medspacy-1.1.6a0/medspacy/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9481 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:54.775316 medspacy-1.1.6a0/medspacy/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/common/base_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5859 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/common/medspacy_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6700 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/common/regex_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6151 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/common/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/components.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:54.779316 medspacy-1.1.6a0/medspacy/context/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13456 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/context/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/context/context_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15026 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/context/context_modifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11407 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/context/context_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/context/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/custom_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:54.779316 medspacy-1.1.6a0/medspacy/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/io/config_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/io/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/io/db_connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/io/db_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/io/db_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12075 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/io/doc_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/io/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/ner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:54.779316 medspacy-1.1.6a0/medspacy/postprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/postprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8673 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/postprocess/postprocessing_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/postprocess/postprocessing_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/postprocess/postprocessing_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/postprocess/postprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:54.779316 medspacy-1.1.6a0/medspacy/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/preprocess/preprocessing_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/preprocess/preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:54.779316 medspacy-1.1.6a0/medspacy/section_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/section_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/section_detection/section.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/section_detection/section_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21792 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/section_detection/sectionizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/section_detection/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/sentence_splitting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:54.783316 medspacy-1.1.6a0/medspacy/target_matcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/target_matcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/target_matcher/concept_tagger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/target_matcher/target_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/target_matcher/target_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8550 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:54.783316 medspacy-1.1.6a0/medspacy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8414 2024-05-02 06:35:54.000000 medspacy-1.1.6a0/medspacy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9264 2024-05-02 06:35:54.000000 medspacy-1.1.6a0/medspacy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 06:35:54.000000 medspacy-1.1.6a0/medspacy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-02 06:35:54.000000 medspacy-1.1.6a0/medspacy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-02 06:35:54.000000 medspacy-1.1.6a0/medspacy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:54.783316 medspacy-1.1.6a0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/requirements/requirements_tests.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:54.763316 medspacy-1.1.6a0/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    28435 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/context_rules.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:54.759316 medspacy-1.1.6a0/resources/quickumls/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:54.763316 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:54.763316 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/
+-rw-r--r--   0 runner    (1001) docker     (127)    12288 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/cui.unqlite
+-rw-r--r--   0 runner    (1001) docker     (127)    12288 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/semtypes.unqlite
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/database_backend.flag
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/language.flag
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/lowercase.flag
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/normalize-unicode.flag
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:54.771316 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/
+-rw-r--r--   0 runner    (1001) docker     (127)     6116 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring
+-rw-r--r--   0 runner    (1001) docker     (127)     6892 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:54.771316 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:54.771316 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/
+-rw-r--r--   0 runner    (1001) docker     (127)    20480 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/cui.unqlite
+-rw-r--r--   0 runner    (1001) docker     (127)    12288 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/semtypes.unqlite
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/database_backend.flag
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/language.flag
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/lowercase.flag
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/normalize-unicode.flag
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:54.775316 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring
+-rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)    23496 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/rush_rules.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)    12073 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/section_patterns.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 06:35:54.783316 medspacy-1.1.6a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:54.783316 medspacy-1.1.6a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/tests/test_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7324 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/tests/test_medspacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/tests/test_notebooks.py
```

### Comparing `medspacy-1.1.6/LICENSE` & `medspacy-1.1.6a0/LICENSE`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/PKG-INFO` & `medspacy-1.1.6a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medspacy
-Version: 1.1.6
+Version: 1.1.6a0
 Summary: Library for clinical NLP with spaCy.
 Author: medSpaCy
 License: MIT License
         
         Copyright (c) 2020 medspacy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `medspacy-1.1.6/README.md` & `medspacy-1.1.6a0/README.md`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/medspacy/_extensions.py` & `medspacy-1.1.6a0/medspacy/_extensions.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/medspacy/common/base_rule.py` & `medspacy-1.1.6a0/medspacy/common/base_rule.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/medspacy/common/medspacy_matcher.py` & `medspacy-1.1.6a0/medspacy/common/medspacy_matcher.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/medspacy/common/regex_matcher.py` & `medspacy-1.1.6a0/medspacy/common/regex_matcher.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/medspacy/common/util.py` & `medspacy-1.1.6a0/medspacy/common/util.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/medspacy/context/context.py` & `medspacy-1.1.6a0/medspacy/context/context.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/medspacy/context/context_graph.py` & `medspacy-1.1.6a0/medspacy/context/context_graph.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/medspacy/context/context_modifier.py` & `medspacy-1.1.6a0/medspacy/context/context_modifier.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/medspacy/context/context_rule.py` & `medspacy-1.1.6a0/medspacy/context/context_rule.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/medspacy/context/util.py` & `medspacy-1.1.6a0/medspacy/context/util.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/medspacy/custom_tokenizer.py` & `medspacy-1.1.6a0/medspacy/custom_tokenizer.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/medspacy/io/config_example.py` & `medspacy-1.1.6a0/medspacy/io/config_example.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/medspacy/io/db_connect.py` & `medspacy-1.1.6a0/medspacy/io/db_connect.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/medspacy/io/db_reader.py` & `medspacy-1.1.6a0/medspacy/io/db_reader.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/medspacy/io/db_writer.py` & `medspacy-1.1.6a0/medspacy/io/db_writer.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/medspacy/io/doc_consumer.py` & `medspacy-1.1.6a0/medspacy/io/doc_consumer.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/medspacy/io/pipeline.py` & `medspacy-1.1.6a0/medspacy/io/pipeline.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/medspacy/postprocess/postprocessing_functions.py` & `medspacy-1.1.6a0/medspacy/postprocess/postprocessing_functions.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/medspacy/postprocess/postprocessing_pattern.py` & `medspacy-1.1.6a0/medspacy/postprocess/postprocessing_pattern.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/medspacy/postprocess/postprocessing_rule.py` & `medspacy-1.1.6a0/medspacy/postprocess/postprocessing_rule.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/medspacy/postprocess/postprocessor.py` & `medspacy-1.1.6a0/medspacy/postprocess/postprocessor.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/medspacy/preprocess/preprocessing_rule.py` & `medspacy-1.1.6a0/medspacy/preprocess/preprocessing_rule.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/medspacy/preprocess/preprocessor.py` & `medspacy-1.1.6a0/medspacy/preprocess/preprocessor.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/medspacy/section_detection/section.py` & `medspacy-1.1.6a0/medspacy/section_detection/section.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/medspacy/section_detection/section_rule.py` & `medspacy-1.1.6a0/medspacy/section_detection/section_rule.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/medspacy/section_detection/sectionizer.py` & `medspacy-1.1.6a0/medspacy/section_detection/sectionizer.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/medspacy/section_detection/util.py` & `medspacy-1.1.6a0/medspacy/section_detection/util.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/medspacy/sentence_splitting.py` & `medspacy-1.1.6a0/medspacy/sentence_splitting.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/medspacy/target_matcher/concept_tagger.py` & `medspacy-1.1.6a0/medspacy/target_matcher/concept_tagger.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/medspacy/target_matcher/target_matcher.py` & `medspacy-1.1.6a0/medspacy/target_matcher/target_matcher.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/medspacy/target_matcher/target_rule.py` & `medspacy-1.1.6a0/medspacy/target_matcher/target_rule.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/medspacy/util.py` & `medspacy-1.1.6a0/medspacy/util.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/medspacy/visualization.py` & `medspacy-1.1.6a0/medspacy/visualization.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/medspacy.egg-info/PKG-INFO` & `medspacy-1.1.6a0/medspacy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medspacy
-Version: 1.1.6
+Version: 1.1.6a0
 Summary: Library for clinical NLP with spaCy.
 Author: medSpaCy
 License: MIT License
         
         Copyright (c) 2020 medspacy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `medspacy-1.1.6/medspacy.egg-info/SOURCES.txt` & `medspacy-1.1.6a0/medspacy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/pyproject.toml` & `medspacy-1.1.6a0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/context_rules.json` & `medspacy-1.1.6a0/resources/context_rules.json`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/cui.unqlite` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/cui.unqlite`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/semtypes.unqlite` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/semtypes.unqlite`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/cui.unqlite` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/cui.unqlite`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/semtypes.unqlite` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/semtypes.unqlite`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/rush_rules.tsv` & `medspacy-1.1.6a0/resources/rush_rules.tsv`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/resources/section_patterns.json` & `medspacy-1.1.6a0/resources/section_patterns.json`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/setup.py` & `medspacy-1.1.6a0/setup.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/tests/test_extensions.py` & `medspacy-1.1.6a0/tests/test_extensions.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/tests/test_medspacy.py` & `medspacy-1.1.6a0/tests/test_medspacy.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.6/tests/test_notebooks.py` & `medspacy-1.1.6a0/tests/test_notebooks.py`

 * *Files identical despite different names*

