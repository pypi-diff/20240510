# Comparing `tmp/pactman-2.8.0.tar.gz` & `tmp/pactman-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pactman-2.8.0.tar", last modified: Thu Dec 20 22:42:58 2018, max compression
+gzip compressed data, was "dist/pactman-2.9.0.tar", last modified: Wed Jan  2 00:21:22 2019, max compression
```

## Comparing `pactman-2.8.0.tar` & `pactman-2.9.0.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxr-xr-x   0 joneri   (216308880) REECENET\Domain Users (1793904685)        0 2018-12-20 22:42:58.000000 pactman-2.8.0/
-drwxr-xr-x   0 joneri   (216308880) REECENET\Domain Users (1793904685)        0 2018-12-20 22:42:58.000000 pactman-2.8.0/pactman.egg-info/
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)    20508 2018-12-20 22:42:57.000000 pactman-2.8.0/pactman.egg-info/PKG-INFO
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     1505 2018-12-20 22:42:58.000000 pactman-2.8.0/pactman.egg-info/SOURCES.txt
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)       91 2018-12-20 22:42:57.000000 pactman-2.8.0/pactman.egg-info/entry_points.txt
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)       46 2018-12-20 22:42:57.000000 pactman-2.8.0/pactman.egg-info/requires.txt
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)        8 2018-12-20 22:42:57.000000 pactman-2.8.0/pactman.egg-info/top_level.txt
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)        1 2018-12-20 22:42:57.000000 pactman-2.8.0/pactman.egg-info/dependency_links.txt
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)    20508 2018-12-20 22:42:58.000000 pactman-2.8.0/PKG-INFO
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     2243 2018-08-13 01:19:24.000000 pactman-2.8.0/LICENSE
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)       43 2018-08-13 02:04:41.000000 pactman-2.8.0/MANIFEST.in
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)    16196 2018-12-20 22:42:52.000000 pactman-2.8.0/README.md
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     1448 2018-08-31 00:55:11.000000 pactman-2.8.0/setup.py
-drwxr-xr-x   0 joneri   (216308880) REECENET\Domain Users (1793904685)        0 2018-12-20 22:42:58.000000 pactman-2.8.0/pactman/
-drwxr-xr-x   0 joneri   (216308880) REECENET\Domain Users (1793904685)        0 2018-12-20 22:42:58.000000 pactman-2.8.0/pactman/test/
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)      670 2018-08-13 01:19:24.000000 pactman-2.8.0/pactman/test/test_result.py
-drwxr-xr-x   0 joneri   (216308880) REECENET\Domain Users (1793904685)        0 2018-12-20 22:42:58.000000 pactman-2.8.0/pactman/test/pact_serialisation/
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     2291 2018-12-19 21:40:58.000000 pactman-2.8.0/pactman/test/pact_serialisation/test_full_payload.py
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     1292 2018-12-20 04:57:19.000000 pactman-2.8.0/pactman/test/pact_serialisation/test_body.py
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)        0 2018-12-19 21:40:58.000000 pactman-2.8.0/pactman/test/pact_serialisation/__init__.py
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     5301 2018-12-19 21:40:58.000000 pactman-2.8.0/pactman/test/pact_serialisation/test_request_query.py
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     3209 2018-12-19 21:40:58.000000 pactman-2.8.0/pactman/test/pact_serialisation/test_given.py
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)      279 2018-08-13 01:19:24.000000 pactman-2.8.0/pactman/test/test_mock_provider.py
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     4107 2018-12-19 21:40:58.000000 pactman-2.8.0/pactman/test/test_pact_generation.py
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)        0 2018-08-13 01:19:24.000000 pactman-2.8.0/pactman/test/__init__.py
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)      764 2018-08-13 01:19:24.000000 pactman-2.8.0/pactman/test/test_mock_response.py
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)      826 2018-08-13 01:19:24.000000 pactman-2.8.0/pactman/test/test_parse_header.py
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     1896 2018-08-13 01:19:24.000000 pactman-2.8.0/pactman/test/test_mock_consumer.py
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     2378 2018-11-30 01:01:03.000000 pactman-2.8.0/pactman/test/test_mock_request.py
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)    16834 2018-12-13 21:33:44.000000 pactman-2.8.0/pactman/test/test_verifier.py
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     9597 2018-12-19 21:40:58.000000 pactman-2.8.0/pactman/test/test_mock_pact.py
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     7360 2018-08-13 01:19:24.000000 pactman-2.8.0/pactman/test/test_mock_matchers.py
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     3074 2018-12-20 22:42:52.000000 pactman-2.8.0/pactman/test/test_mock_urlopen.py
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     5990 2018-12-13 21:33:44.000000 pactman-2.8.0/pactman/test/test_matching_rules.py
-drwxr-xr-x   0 joneri   (216308880) REECENET\Domain Users (1793904685)        0 2018-12-20 22:42:58.000000 pactman-2.8.0/pactman/mock/
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     3006 2018-12-20 22:42:52.000000 pactman-2.8.0/pactman/mock/mock_urlopen.py
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)      360 2018-08-13 01:19:24.000000 pactman-2.8.0/pactman/mock/provider.py
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     4736 2018-12-20 22:42:52.000000 pactman-2.8.0/pactman/mock/mock_server.py
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     5258 2018-12-20 22:42:52.000000 pactman-2.8.0/pactman/mock/pact_request_handler.py
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     3695 2018-12-19 21:40:58.000000 pactman-2.8.0/pactman/mock/request.py
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)        0 2018-08-13 01:19:24.000000 pactman-2.8.0/pactman/mock/__init__.py
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     2028 2018-08-21 23:25:22.000000 pactman-2.8.0/pactman/mock/response.py
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     4494 2018-08-13 04:07:01.000000 pactman-2.8.0/pactman/mock/consumer.py
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)    10313 2018-12-18 21:31:53.000000 pactman-2.8.0/pactman/mock/matchers.py
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)    11596 2018-12-19 21:40:58.000000 pactman-2.8.0/pactman/mock/pact.py
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)      326 2018-08-13 01:19:24.000000 pactman-2.8.0/pactman/__init__.py
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)       22 2018-12-20 22:42:52.000000 pactman-2.8.0/pactman/__version__.py
-drwxr-xr-x   0 joneri   (216308880) REECENET\Domain Users (1793904685)        0 2018-12-20 22:42:58.000000 pactman-2.8.0/pactman/verifier/
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)      185 2018-08-13 01:19:24.000000 pactman-2.8.0/pactman/verifier/paths.py
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     3169 2018-11-30 01:01:03.000000 pactman-2.8.0/pactman/verifier/broker_pact.py
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     5567 2018-11-30 01:01:03.000000 pactman-2.8.0/pactman/verifier/command_line.py
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)        0 2018-08-13 01:19:24.000000 pactman-2.8.0/pactman/verifier/__init__.py
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     1176 2018-08-13 01:19:24.000000 pactman-2.8.0/pactman/verifier/result.py
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     1783 2018-12-20 22:42:52.000000 pactman-2.8.0/pactman/verifier/parse_header.py
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)    19763 2018-12-20 22:42:52.000000 pactman-2.8.0/pactman/verifier/verify.py
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)    13674 2018-12-13 21:33:44.000000 pactman-2.8.0/pactman/verifier/matching_rule.py
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)      237 2018-08-13 01:19:24.000000 pactman-2.8.0/pactman/verifier/pytest_plugin.py
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     1094 2018-12-19 21:40:58.000000 pactman-2.8.0/CONTRIBUTING.md
--rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)      450 2018-12-20 22:42:58.000000 pactman-2.8.0/setup.cfg
+drwxr-xr-x   0 joneri   (216308880) REECENET\Domain Users (1793904685)        0 2019-01-02 00:21:22.000000 pactman-2.9.0/
+drwxr-xr-x   0 joneri   (216308880) REECENET\Domain Users (1793904685)        0 2019-01-02 00:21:22.000000 pactman-2.9.0/pactman.egg-info/
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)    22081 2019-01-02 00:21:22.000000 pactman-2.9.0/pactman.egg-info/PKG-INFO
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     1525 2019-01-02 00:21:22.000000 pactman-2.9.0/pactman.egg-info/SOURCES.txt
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)       91 2019-01-02 00:21:22.000000 pactman-2.9.0/pactman.egg-info/entry_points.txt
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)       46 2019-01-02 00:21:22.000000 pactman-2.9.0/pactman.egg-info/requires.txt
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)        8 2019-01-02 00:21:22.000000 pactman-2.9.0/pactman.egg-info/top_level.txt
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)        1 2019-01-02 00:21:22.000000 pactman-2.9.0/pactman.egg-info/dependency_links.txt
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)    22081 2019-01-02 00:21:22.000000 pactman-2.9.0/PKG-INFO
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     2243 2018-08-13 01:19:24.000000 pactman-2.9.0/LICENSE
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)       43 2018-08-13 02:04:41.000000 pactman-2.9.0/MANIFEST.in
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)    17553 2019-01-02 00:03:40.000000 pactman-2.9.0/README.md
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     1448 2018-12-30 23:38:57.000000 pactman-2.9.0/setup.py
+drwxr-xr-x   0 joneri   (216308880) REECENET\Domain Users (1793904685)        0 2019-01-02 00:21:22.000000 pactman-2.9.0/pactman/
+drwxr-xr-x   0 joneri   (216308880) REECENET\Domain Users (1793904685)        0 2019-01-02 00:21:22.000000 pactman-2.9.0/pactman/test/
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)      670 2018-08-13 01:19:24.000000 pactman-2.9.0/pactman/test/test_result.py
+drwxr-xr-x   0 joneri   (216308880) REECENET\Domain Users (1793904685)        0 2019-01-02 00:21:22.000000 pactman-2.9.0/pactman/test/pact_serialisation/
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     1992 2018-12-31 04:10:34.000000 pactman-2.9.0/pactman/test/pact_serialisation/test_full_payload.py
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     1096 2018-12-31 04:10:34.000000 pactman-2.9.0/pactman/test/pact_serialisation/test_body.py
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)        0 2018-12-19 21:40:58.000000 pactman-2.9.0/pactman/test/pact_serialisation/__init__.py
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     4693 2018-12-31 04:10:34.000000 pactman-2.9.0/pactman/test/pact_serialisation/test_request_query.py
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     3576 2019-01-02 00:03:40.000000 pactman-2.9.0/pactman/test/pact_serialisation/test_given.py
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)      279 2018-08-13 01:19:24.000000 pactman-2.9.0/pactman/test/test_mock_provider.py
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     5298 2019-01-02 00:09:01.000000 pactman-2.9.0/pactman/test/test_pact_generation.py
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)        0 2018-08-13 01:19:24.000000 pactman-2.9.0/pactman/test/__init__.py
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)      764 2018-08-13 01:19:24.000000 pactman-2.9.0/pactman/test/test_mock_response.py
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)      825 2018-12-31 04:10:34.000000 pactman-2.9.0/pactman/test/test_parse_header.py
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     1896 2019-01-02 00:03:40.000000 pactman-2.9.0/pactman/test/test_mock_consumer.py
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     2378 2019-01-02 00:09:01.000000 pactman-2.9.0/pactman/test/test_mock_request.py
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)    16872 2018-12-31 04:10:34.000000 pactman-2.9.0/pactman/test/test_verifier.py
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     9634 2018-12-31 04:10:34.000000 pactman-2.9.0/pactman/test/test_mock_pact.py
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     7391 2018-12-31 04:10:34.000000 pactman-2.9.0/pactman/test/test_mock_matchers.py
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     3069 2018-12-31 04:10:34.000000 pactman-2.9.0/pactman/test/test_mock_urlopen.py
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     6268 2018-12-31 04:10:34.000000 pactman-2.9.0/pactman/test/test_matching_rules.py
+drwxr-xr-x   0 joneri   (216308880) REECENET\Domain Users (1793904685)        0 2019-01-02 00:21:22.000000 pactman-2.9.0/pactman/mock/
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     3002 2018-12-31 04:10:34.000000 pactman-2.9.0/pactman/mock/mock_urlopen.py
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)      360 2018-08-13 01:19:24.000000 pactman-2.9.0/pactman/mock/provider.py
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     4698 2018-12-31 04:10:34.000000 pactman-2.9.0/pactman/mock/mock_server.py
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     4058 2019-01-02 00:03:40.000000 pactman-2.9.0/pactman/mock/pact_request_handler.py
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     3720 2019-01-02 00:03:40.000000 pactman-2.9.0/pactman/mock/request.py
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)        0 2018-08-13 01:19:24.000000 pactman-2.9.0/pactman/mock/__init__.py
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     2053 2018-12-31 04:10:34.000000 pactman-2.9.0/pactman/mock/response.py
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     4503 2019-01-02 00:03:40.000000 pactman-2.9.0/pactman/mock/consumer.py
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)    10313 2018-12-18 21:31:53.000000 pactman-2.9.0/pactman/mock/matchers.py
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)    13120 2019-01-02 00:03:40.000000 pactman-2.9.0/pactman/mock/pact.py
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)      326 2018-08-13 01:19:24.000000 pactman-2.9.0/pactman/__init__.py
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)       22 2018-12-31 03:35:34.000000 pactman-2.9.0/pactman/__version__.py
+drwxr-xr-x   0 joneri   (216308880) REECENET\Domain Users (1793904685)        0 2019-01-02 00:21:22.000000 pactman-2.9.0/pactman/verifier/
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)      185 2018-08-13 01:19:24.000000 pactman-2.9.0/pactman/verifier/paths.py
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     3168 2018-12-31 04:10:34.000000 pactman-2.9.0/pactman/verifier/broker_pact.py
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     5567 2018-11-30 01:01:03.000000 pactman-2.9.0/pactman/verifier/command_line.py
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)        0 2018-08-13 01:19:24.000000 pactman-2.9.0/pactman/verifier/__init__.py
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     1175 2018-12-31 04:10:34.000000 pactman-2.9.0/pactman/verifier/result.py
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     1783 2018-12-20 22:42:52.000000 pactman-2.9.0/pactman/verifier/parse_header.py
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)    19790 2018-12-31 04:10:34.000000 pactman-2.9.0/pactman/verifier/verify.py
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)    13673 2018-12-31 04:10:34.000000 pactman-2.9.0/pactman/verifier/matching_rule.py
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)      237 2018-08-13 01:19:24.000000 pactman-2.9.0/pactman/verifier/pytest_plugin.py
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)       49 2019-01-02 00:03:40.000000 pactman-2.9.0/pactman/__main__.py
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)     1094 2018-12-19 21:40:58.000000 pactman-2.9.0/CONTRIBUTING.md
+-rw-r--r--   0 joneri   (216308880) REECENET\Domain Users (1793904685)      450 2019-01-02 00:21:22.000000 pactman-2.9.0/setup.cfg
```

### Comparing `pactman-2.8.0/pactman.egg-info/PKG-INFO` & `pactman-2.9.0/pactman.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: pactman
-Version: 2.8.0
+Version: 2.9.0
 Summary: Tools for creating and verifying consumer driven contracts using the Pact framework.
 Home-page: https://github.com/reecetech/pactman
 Author: ReeceTech
 Author-email: richard.jones@reece.com.au
 License: MIT, Copyright (c) 2018 ReeceTech
 Description: # pactman
         
+        [![](https://img.shields.io/pypi/v/pactman.svg)](https://pypi.org/project/pactman/)
+        
         Python version of Pact mocking, generation and verification.
         
         Enables [consumer driven contract testing], providing unit test mocking of provider services
         and DSL for the consumer project, and interaction playback and verification for the service
         provider project. Currently supports versions 1.1, 2 and 3 of the [Pact specification].
         
         For more information about what Pact is, and how it can help you
@@ -25,14 +27,29 @@
         ## pactman vs pact-python
         
         The key difference is all functionality is implemented in Python, rather than shelling out or forking
         to the ruby implementation. This allows for a much nicer mocking user experience (it mocks urllib3
         directly), is faster, less messy configuration (multiple providers means multiple ruby processes spawned
         on different ports).
         
+        Where `pact-python` required management of a background Ruby server, and manually starting and stopping
+        it, `pactman` allows a much nicer usage like:
+        
+        ```python
+        import requests
+        from pactman import Consumer, Provider
+        
+        def test_interaction():
+            pact = Consumer('Consumer').has_pact_with(Provider('Provider')) \
+                .given("some data exists").upon_receiving("a request") \
+                .with_request("get", "/", query={"foo": ["bar"]}).will_respond_with(200)
+            with pact:
+                requests.get(pact.uri, params={"foo": ["bar"]})
+        ```
+        
         It also supports a broader set of the pact specification (versions 1.1 through to 3).
         
         The pact verifier has been engineered from the start to talk to a pact broker (both to discover pacts
         and to return verification results).
         
         There’s a few other quality of life improvements, but those are the big ones.
         
@@ -67,63 +84,57 @@
             response = requests.get(f'http://service.example/users/{user_name}')
             return response.json()
         ```
         
         Then `Consumer`'s contract test might look something like this:
         
         ```python
-        import atexit
         import unittest
-        
         from pactman import Consumer, Provider
         
         
-        pact = Consumer('Consumer').has_pact_with(Provider('Provider'))
-        pact.start_mocking()
-        atexit.register(pact.stop_mocking)
-        
-        
         class GetUserInfoContract(unittest.TestCase):
           def test_get_user(self):
             expected = {
               'username': 'UserA',
               'id': 123,
               'groups': ['Editors']
             }
         
-            pact.given(
+            Consumer('Consumer').has_pact_with(Provider('Provider')).given(
                 'UserA exists and is not an administrator'
             ).upon_receiving(
                 'a request for UserA'
             ).with_request(
                 'GET', '/users/UserA'
             ) .will_respond_with(200, body=expected)
         
             with pact:
               result = get_user('UserA')
         
             self.assertEqual(result, expected)
-        
         ```
         
         This does a few important things:
         
          - Defines the Consumer and Provider objects that describe our product and our service under test
          - Uses `given` to define the setup criteria for the Provider `UserA exists and is not an administrator`
          - Defines what the request that is expected to be made by the consumer will contain
          - Defines how the server is expected to respond
         
         Using the Pact object as a [context manager], we call our method under test
         which will then communicate with the Pact mock service. The mock service will respond with
         the items we defined, allowing us to assert that the method processed the response and
-        returned the expected value. If you want more control over when the mock service is
-        configured and the interactions verified, use the `setup` and `verify` methods, respectively:
+        returned the expected value.
+        
+        If you want more control over when the mock service is configured and the interactions verified,
+        use the `setup` and `verify` methods, respectively:
         
         ```python
-            pact.given(
+            Consumer('Consumer').has_pact_with(Provider('Provider')).given(
                 'UserA exists and is not an administrator'
             ).upon_receiving(
                 'a request for UserA'
             ).with_request(
                 'GET', '/users/UserA'
             ) .will_respond_with(200, body=expected)
         
@@ -180,20 +191,27 @@
         
         `use_mocking_server` defaults to `False` and controls the mocking method used by `pactman`. The default is to
         patch `urllib3`, which is the library underpinning `requests` and is also used by some other projects. If you
         are using a different library to make your HTTP requests which does not use `urllib3` underneath then you will need
         to set the `use_mocking_server` argument to `True`. This causes `pactman` to run an actual HTTP server to mock the
         requests (the server is listening on `pact.uri` - use that to redirect your HTTP requests to the mock server.) You
         may also set the `PACT_USE_MOCKING_SERVER` environment variable to "yes" to force your entire suite to use the server
-        approach.
+        approach. You should declare the pact particpants (consumer and provider) outside of your tests and will need
+        to start and stop the mocking service outside of your tests too. The code below shows what using the server might
+        look like:
         
         ```python
+        import atexit
         from pactman import Consumer, Provider
         pact = Consumer('Consumer').has_pact_with(Provider('Provider'), use_mocking_server=True)
-        ```
+        pact.start_mocking()
+        atexit.register(pact.stop_mocking)
+        ``````
+        
+        You'd then use `pact` to declare pacts between those participants.
         
         ### Some words about given()
         You use `given()` to indicate to the provider that they should have some state in order to
         be able to satisfy the interaction. You should agree upon the state and its specification
         in discussion with the provider.
         
         If you are defining a version 3 pact you may define provider states more richly, for example:
@@ -355,14 +373,23 @@
         
         This creates a `dist/pactman-N.N.N.tar.gz` file, where the Ns are the current version.
         From there you can use pip to install it:
         `pip install ./dist/pactman-N.N.N.tar.gz`
         
         ## Release History
         
+        2.9.0
+        
+        - Fix `with_request` when called with a dict query (thanks Cong)
+        - Make `start_mocking()` and `stop_mocking()` optional with non-server mocking
+        - Add shortcut so `python -m pactman.verifier.command_line` is just `python -m pactman`
+          (mostly used in testing before release)
+        - Handle the `None` provider state
+        - Ensure pact spec versions are consistent across all mocks used to generate a pact file
+        
         2.8.0
         
         - Close up some edge cases in body content during mocking, and document in README
         
         2.7.0
         
         - Added `and_given()` as a method of defining additonal provider states for v3+ pacts
```

### Comparing `pactman-2.8.0/pactman.egg-info/SOURCES.txt` & `pactman-2.9.0/pactman.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 pactman/__init__.py
+pactman/__main__.py
 pactman/__version__.py
 pactman.egg-info/PKG-INFO
 pactman.egg-info/SOURCES.txt
 pactman.egg-info/dependency_links.txt
 pactman.egg-info/entry_points.txt
 pactman.egg-info/requires.txt
 pactman.egg-info/top_level.txt
```

### Comparing `pactman-2.8.0/PKG-INFO` & `pactman-2.9.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: pactman
-Version: 2.8.0
+Version: 2.9.0
 Summary: Tools for creating and verifying consumer driven contracts using the Pact framework.
 Home-page: https://github.com/reecetech/pactman
 Author: ReeceTech
 Author-email: richard.jones@reece.com.au
 License: MIT, Copyright (c) 2018 ReeceTech
 Description: # pactman
         
+        [![](https://img.shields.io/pypi/v/pactman.svg)](https://pypi.org/project/pactman/)
+        
         Python version of Pact mocking, generation and verification.
         
         Enables [consumer driven contract testing], providing unit test mocking of provider services
         and DSL for the consumer project, and interaction playback and verification for the service
         provider project. Currently supports versions 1.1, 2 and 3 of the [Pact specification].
         
         For more information about what Pact is, and how it can help you
@@ -25,14 +27,29 @@
         ## pactman vs pact-python
         
         The key difference is all functionality is implemented in Python, rather than shelling out or forking
         to the ruby implementation. This allows for a much nicer mocking user experience (it mocks urllib3
         directly), is faster, less messy configuration (multiple providers means multiple ruby processes spawned
         on different ports).
         
+        Where `pact-python` required management of a background Ruby server, and manually starting and stopping
+        it, `pactman` allows a much nicer usage like:
+        
+        ```python
+        import requests
+        from pactman import Consumer, Provider
+        
+        def test_interaction():
+            pact = Consumer('Consumer').has_pact_with(Provider('Provider')) \
+                .given("some data exists").upon_receiving("a request") \
+                .with_request("get", "/", query={"foo": ["bar"]}).will_respond_with(200)
+            with pact:
+                requests.get(pact.uri, params={"foo": ["bar"]})
+        ```
+        
         It also supports a broader set of the pact specification (versions 1.1 through to 3).
         
         The pact verifier has been engineered from the start to talk to a pact broker (both to discover pacts
         and to return verification results).
         
         There’s a few other quality of life improvements, but those are the big ones.
         
@@ -67,63 +84,57 @@
             response = requests.get(f'http://service.example/users/{user_name}')
             return response.json()
         ```
         
         Then `Consumer`'s contract test might look something like this:
         
         ```python
-        import atexit
         import unittest
-        
         from pactman import Consumer, Provider
         
         
-        pact = Consumer('Consumer').has_pact_with(Provider('Provider'))
-        pact.start_mocking()
-        atexit.register(pact.stop_mocking)
-        
-        
         class GetUserInfoContract(unittest.TestCase):
           def test_get_user(self):
             expected = {
               'username': 'UserA',
               'id': 123,
               'groups': ['Editors']
             }
         
-            pact.given(
+            Consumer('Consumer').has_pact_with(Provider('Provider')).given(
                 'UserA exists and is not an administrator'
             ).upon_receiving(
                 'a request for UserA'
             ).with_request(
                 'GET', '/users/UserA'
             ) .will_respond_with(200, body=expected)
         
             with pact:
               result = get_user('UserA')
         
             self.assertEqual(result, expected)
-        
         ```
         
         This does a few important things:
         
          - Defines the Consumer and Provider objects that describe our product and our service under test
          - Uses `given` to define the setup criteria for the Provider `UserA exists and is not an administrator`
          - Defines what the request that is expected to be made by the consumer will contain
          - Defines how the server is expected to respond
         
         Using the Pact object as a [context manager], we call our method under test
         which will then communicate with the Pact mock service. The mock service will respond with
         the items we defined, allowing us to assert that the method processed the response and
-        returned the expected value. If you want more control over when the mock service is
-        configured and the interactions verified, use the `setup` and `verify` methods, respectively:
+        returned the expected value.
+        
+        If you want more control over when the mock service is configured and the interactions verified,
+        use the `setup` and `verify` methods, respectively:
         
         ```python
-            pact.given(
+            Consumer('Consumer').has_pact_with(Provider('Provider')).given(
                 'UserA exists and is not an administrator'
             ).upon_receiving(
                 'a request for UserA'
             ).with_request(
                 'GET', '/users/UserA'
             ) .will_respond_with(200, body=expected)
         
@@ -180,20 +191,27 @@
         
         `use_mocking_server` defaults to `False` and controls the mocking method used by `pactman`. The default is to
         patch `urllib3`, which is the library underpinning `requests` and is also used by some other projects. If you
         are using a different library to make your HTTP requests which does not use `urllib3` underneath then you will need
         to set the `use_mocking_server` argument to `True`. This causes `pactman` to run an actual HTTP server to mock the
         requests (the server is listening on `pact.uri` - use that to redirect your HTTP requests to the mock server.) You
         may also set the `PACT_USE_MOCKING_SERVER` environment variable to "yes" to force your entire suite to use the server
-        approach.
+        approach. You should declare the pact particpants (consumer and provider) outside of your tests and will need
+        to start and stop the mocking service outside of your tests too. The code below shows what using the server might
+        look like:
         
         ```python
+        import atexit
         from pactman import Consumer, Provider
         pact = Consumer('Consumer').has_pact_with(Provider('Provider'), use_mocking_server=True)
-        ```
+        pact.start_mocking()
+        atexit.register(pact.stop_mocking)
+        ``````
+        
+        You'd then use `pact` to declare pacts between those participants.
         
         ### Some words about given()
         You use `given()` to indicate to the provider that they should have some state in order to
         be able to satisfy the interaction. You should agree upon the state and its specification
         in discussion with the provider.
         
         If you are defining a version 3 pact you may define provider states more richly, for example:
@@ -355,14 +373,23 @@
         
         This creates a `dist/pactman-N.N.N.tar.gz` file, where the Ns are the current version.
         From there you can use pip to install it:
         `pip install ./dist/pactman-N.N.N.tar.gz`
         
         ## Release History
         
+        2.9.0
+        
+        - Fix `with_request` when called with a dict query (thanks Cong)
+        - Make `start_mocking()` and `stop_mocking()` optional with non-server mocking
+        - Add shortcut so `python -m pactman.verifier.command_line` is just `python -m pactman`
+          (mostly used in testing before release)
+        - Handle the `None` provider state
+        - Ensure pact spec versions are consistent across all mocks used to generate a pact file
+        
         2.8.0
         
         - Close up some edge cases in body content during mocking, and document in README
         
         2.7.0
         
         - Added `and_given()` as a method of defining additonal provider states for v3+ pacts
```

### Comparing `pactman-2.8.0/LICENSE` & `pactman-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pactman-2.8.0/README.md` & `pactman-2.9.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # pactman
 
+[![](https://img.shields.io/pypi/v/pactman.svg)](https://pypi.org/project/pactman/)
+
 Python version of Pact mocking, generation and verification.
 
 Enables [consumer driven contract testing], providing unit test mocking of provider services
 and DSL for the consumer project, and interaction playback and verification for the service
 provider project. Currently supports versions 1.1, 2 and 3 of the [Pact specification].
 
 For more information about what Pact is, and how it can help you
@@ -17,14 +19,29 @@
 ## pactman vs pact-python
 
 The key difference is all functionality is implemented in Python, rather than shelling out or forking
 to the ruby implementation. This allows for a much nicer mocking user experience (it mocks urllib3
 directly), is faster, less messy configuration (multiple providers means multiple ruby processes spawned
 on different ports).
 
+Where `pact-python` required management of a background Ruby server, and manually starting and stopping
+it, `pactman` allows a much nicer usage like:
+
+```python
+import requests
+from pactman import Consumer, Provider
+
+def test_interaction():
+    pact = Consumer('Consumer').has_pact_with(Provider('Provider')) \
+        .given("some data exists").upon_receiving("a request") \
+        .with_request("get", "/", query={"foo": ["bar"]}).will_respond_with(200)
+    with pact:
+        requests.get(pact.uri, params={"foo": ["bar"]})
+```
+
 It also supports a broader set of the pact specification (versions 1.1 through to 3).
 
 The pact verifier has been engineered from the start to talk to a pact broker (both to discover pacts
 and to return verification results).
 
 There’s a few other quality of life improvements, but those are the big ones.
 
@@ -59,63 +76,57 @@
     response = requests.get(f'http://service.example/users/{user_name}')
     return response.json()
 ```
 
 Then `Consumer`'s contract test might look something like this:
 
 ```python
-import atexit
 import unittest
-
 from pactman import Consumer, Provider
 
 
-pact = Consumer('Consumer').has_pact_with(Provider('Provider'))
-pact.start_mocking()
-atexit.register(pact.stop_mocking)
-
-
 class GetUserInfoContract(unittest.TestCase):
   def test_get_user(self):
     expected = {
       'username': 'UserA',
       'id': 123,
       'groups': ['Editors']
     }
 
-    pact.given(
+    Consumer('Consumer').has_pact_with(Provider('Provider')).given(
         'UserA exists and is not an administrator'
     ).upon_receiving(
         'a request for UserA'
     ).with_request(
         'GET', '/users/UserA'
     ) .will_respond_with(200, body=expected)
 
     with pact:
       result = get_user('UserA')
 
     self.assertEqual(result, expected)
-
 ```
 
 This does a few important things:
 
  - Defines the Consumer and Provider objects that describe our product and our service under test
  - Uses `given` to define the setup criteria for the Provider `UserA exists and is not an administrator`
  - Defines what the request that is expected to be made by the consumer will contain
  - Defines how the server is expected to respond
 
 Using the Pact object as a [context manager], we call our method under test
 which will then communicate with the Pact mock service. The mock service will respond with
 the items we defined, allowing us to assert that the method processed the response and
-returned the expected value. If you want more control over when the mock service is
-configured and the interactions verified, use the `setup` and `verify` methods, respectively:
+returned the expected value.
+
+If you want more control over when the mock service is configured and the interactions verified,
+use the `setup` and `verify` methods, respectively:
 
 ```python
-    pact.given(
+    Consumer('Consumer').has_pact_with(Provider('Provider')).given(
         'UserA exists and is not an administrator'
     ).upon_receiving(
         'a request for UserA'
     ).with_request(
         'GET', '/users/UserA'
     ) .will_respond_with(200, body=expected)
 
@@ -172,20 +183,27 @@
 
 `use_mocking_server` defaults to `False` and controls the mocking method used by `pactman`. The default is to
 patch `urllib3`, which is the library underpinning `requests` and is also used by some other projects. If you
 are using a different library to make your HTTP requests which does not use `urllib3` underneath then you will need
 to set the `use_mocking_server` argument to `True`. This causes `pactman` to run an actual HTTP server to mock the
 requests (the server is listening on `pact.uri` - use that to redirect your HTTP requests to the mock server.) You
 may also set the `PACT_USE_MOCKING_SERVER` environment variable to "yes" to force your entire suite to use the server
-approach.
+approach. You should declare the pact particpants (consumer and provider) outside of your tests and will need
+to start and stop the mocking service outside of your tests too. The code below shows what using the server might
+look like:
 
 ```python
+import atexit
 from pactman import Consumer, Provider
 pact = Consumer('Consumer').has_pact_with(Provider('Provider'), use_mocking_server=True)
-```
+pact.start_mocking()
+atexit.register(pact.stop_mocking)
+``````
+
+You'd then use `pact` to declare pacts between those participants.
 
 ### Some words about given()
 You use `given()` to indicate to the provider that they should have some state in order to
 be able to satisfy the interaction. You should agree upon the state and its specification
 in discussion with the provider.
 
 If you are defining a version 3 pact you may define provider states more richly, for example:
@@ -347,14 +365,23 @@
 
 This creates a `dist/pactman-N.N.N.tar.gz` file, where the Ns are the current version.
 From there you can use pip to install it:
 `pip install ./dist/pactman-N.N.N.tar.gz`
 
 ## Release History
 
+2.9.0
+
+- Fix `with_request` when called with a dict query (thanks Cong)
+- Make `start_mocking()` and `stop_mocking()` optional with non-server mocking
+- Add shortcut so `python -m pactman.verifier.command_line` is just `python -m pactman`
+  (mostly used in testing before release)
+- Handle the `None` provider state
+- Ensure pact spec versions are consistent across all mocks used to generate a pact file
+
 2.8.0
 
 - Close up some edge cases in body content during mocking, and document in README
 
 2.7.0
 
 - Added `and_given()` as a method of defining additonal provider states for v3+ pacts
```

### Comparing `pactman-2.8.0/setup.py` & `pactman-2.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `pactman-2.8.0/pactman/test/test_result.py` & `pactman-2.9.0/pactman/test/test_result.py`

 * *Files identical despite different names*

### Comparing `pactman-2.8.0/pactman/test/pact_serialisation/test_full_payload.py` & `pactman-2.9.0/pactman/test/pact_serialisation/test_full_payload.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,18 @@
-from unittest.mock import Mock
-
 from pactman import Consumer, Provider
-from pactman.mock.pact_request_handler import construct_pact
 
 
 def test_full_payload_v2():
     pact = Consumer('consumer').has_pact_with(Provider('provider'), version='2.0.0')
     (pact
         .given('UserA exists and is not an administrator')
         .upon_receiving('a request for UserA')
         .with_request('get', '/users/UserA')
         .will_respond_with(200, body={'username': 'UserA'}))
-    result = construct_pact(Mock(consumer_name='consumer', provider_name='provider',
-                                 version='2.0.0'), pact._interactions[0])
+    result = pact.construct_pact(pact._interactions[0])
     assert result == {
         'consumer': {'name': 'consumer'},
         'provider': {'name': 'provider'},
         'interactions': [
             {
                 'description': 'a request for UserA',
                 'providerState': 'UserA exists and is not an administrator',
@@ -31,16 +27,15 @@
 def test_full_payload_v3():
     pact = Consumer('consumer').has_pact_with(Provider('provider'), version='3.0.0')
     (pact
      .given([{"name": "User exists and is not an administrator", "params": {"username": "UserA"}}])
      .upon_receiving('a request for UserA')
      .with_request('get', '/users/UserA')
      .will_respond_with(200, body={'username': 'UserA'}))
-    result = construct_pact(Mock(consumer_name='consumer', provider_name='provider',
-                                 version='3.0.0'), pact._interactions[0])
+    result = pact.construct_pact(pact._interactions[0])
     assert result == {
         'consumer': {'name': 'consumer'},
         'provider': {'name': 'provider'},
         'interactions': [
             {
                 'description': 'a request for UserA',
                 'providerStates': [{
```

### Comparing `pactman-2.8.0/pactman/test/pact_serialisation/test_body.py` & `pactman-2.9.0/pactman/test/pact_serialisation/test_body.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,20 @@
-from unittest.mock import Mock
-
-from pactman import Consumer, Provider, EachLike
-from pactman.mock.pact_request_handler import construct_pact
+from pactman import Consumer, EachLike, Provider
 
 
 def test_eachlike():
     pact = (
         Consumer('consumer').has_pact_with(Provider('provider'), version='2.0.0')
         .given("the condition exists")
         .upon_receiving("a request")
         .with_request("POST", "/path", body=EachLike(1))
         .will_respond_with(200, body={"results": EachLike(1)})
     )
 
-    result = construct_pact(Mock(consumer_name='consumer', provider_name='provider',
-                                 version='2.0.0'), pact._interactions[0])
+    result = pact.construct_pact(pact._interactions[0])
     assert result == {
         'consumer': {'name': 'consumer'},
         'provider': {'name': 'provider'},
         'interactions': [
             {
                 'description': 'a request',
                 'providerState': 'the condition exists',
```

### Comparing `pactman-2.8.0/pactman/test/pact_serialisation/test_request_query.py` & `pactman-2.9.0/pactman/test/pact_serialisation/test_request_query.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,17 @@
-from unittest.mock import Mock
-
-from pactman import Consumer, Provider, Like
-from pactman.mock.pact_request_handler import construct_pact
+from pactman import Consumer, Like, Provider
 
 
 def test_v2():
     pact = Consumer('consumer').has_pact_with(Provider('provider'), version='2.0.0')
 
     pact.given("the condition exists").upon_receiving("a request") \
         .with_request("GET", "/path", query="fields=first,second").will_respond_with(200, body='ok')
 
-    result = construct_pact(Mock(consumer_name='consumer', provider_name='provider',
-                                 version='2.0.0'), pact._interactions[0])
+    result = pact.construct_pact(pact._interactions[0])
     assert result == {
         'consumer': {'name': 'consumer'},
         'provider': {'name': 'provider'},
         'interactions': [
             {
                 'description': 'a request',
                 'providerState': 'the condition exists',
@@ -29,16 +25,15 @@
 
 
 def test_v3():
     pact = Consumer('consumer').has_pact_with(Provider('provider'), version='3.0.0')
     pact.given([{'name': "the condition exists", 'params': {}}]).upon_receiving("a request") \
         .with_request("GET", "/path", query=dict(fields='first,second')).will_respond_with(200, body='ok')
 
-    result = construct_pact(Mock(consumer_name='consumer', provider_name='provider',
-                                 version='3.0.0'), pact._interactions[0])
+    result = pact.construct_pact(pact._interactions[0])
     assert result == {
         'consumer': {'name': 'consumer'},
         'provider': {'name': 'provider'},
         'interactions': [
             {
                 'description': 'a request',
                 'providerStates': [{'name': 'the condition exists', 'params': {}}],
@@ -53,16 +48,15 @@
 
 def test_like_v2():
     pact = Consumer('consumer').has_pact_with(Provider('provider'), version='2.0.0')
 
     pact.given("the condition exists").upon_receiving("a request") \
         .with_request("GET", "/path", query=Like("fields=first,second")).will_respond_with(200, body='ok')
 
-    result = construct_pact(Mock(consumer_name='consumer', provider_name='provider',
-                                 version='2.0.0'), pact._interactions[0])
+    result = pact.construct_pact(pact._interactions[0])
     assert result == {
         'consumer': {'name': 'consumer'},
         'provider': {'name': 'provider'},
         'interactions': [
             {
                 'description': 'a request',
                 'providerState': 'the condition exists',
@@ -81,16 +75,15 @@
         Consumer('consumer').has_pact_with(Provider('provider'), version='3.0.0')
         .given("the condition exists")
         .upon_receiving("a request")
         .with_request("GET", "/path", query=dict(fields=Like(['first,second'])))
         .will_respond_with(200, body='ok')
     )
 
-    result = construct_pact(Mock(consumer_name='consumer', provider_name='provider',
-                                 version='3.0.0'), pact._interactions[0])
+    result = pact.construct_pact(pact._interactions[0])
     assert result == {
         'consumer': {'name': 'consumer'},
         'provider': {'name': 'provider'},
         'interactions': [
             {
                 'description': 'a request',
                 'providerStates': [{'name': 'the condition exists', 'params': {}}],
@@ -109,16 +102,15 @@
         Consumer('consumer').has_pact_with(Provider('provider'), version='3.0.0')
         .given("the condition exists")
         .upon_receiving("a request")
         .with_request("GET", "/path", query=Like(dict(fields=['first,second'])))
         .will_respond_with(200, body='ok')
     )
 
-    result = construct_pact(Mock(consumer_name='consumer', provider_name='provider',
-                                 version='3.0.0'), pact._interactions[0])
+    result = pact.construct_pact(pact._interactions[0])
     assert result == {
         'consumer': {'name': 'consumer'},
         'provider': {'name': 'provider'},
         'interactions': [
             {
                 'description': 'a request',
                 'providerStates': [{'name': 'the condition exists', 'params': {}}],
```

### Comparing `pactman-2.8.0/pactman/test/pact_serialisation/test_given.py` & `pactman-2.9.0/pactman/test/pact_serialisation/test_given.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,40 @@
-from unittest.mock import Mock
+import pytest
 
 from pactman import Consumer, Provider
-from pactman.mock.pact_request_handler import construct_pact
+
+
+@pytest.mark.parametrize('version', ['2.0.0', '3.0.0'])
+def test_null(version):
+    pact = Consumer('consumer').has_pact_with(Provider('provider'), version=version)
+    pact.given(None).upon_receiving("a request").with_request("GET", "/path") \
+        .will_respond_with(200, body='ok')
+
+    result = pact.construct_pact(pact._interactions[0])
+    assert result == {
+        'consumer': {'name': 'consumer'},
+        'provider': {'name': 'provider'},
+        'interactions': [
+            {
+                'description': 'a request',
+                'request': dict(method='GET', path='/path'),
+                'response': dict(status=200, body='ok'),
+
+            }
+        ],
+        'metadata': dict(pactSpecification=dict(version=version))
+    }
 
 
 def test_v2():
     pact = Consumer('consumer').has_pact_with(Provider('provider'), version='2.0.0')
     pact.given("the condition exists").upon_receiving("a request").with_request("GET", "/path") \
         .will_respond_with(200, body='ok')
 
-    result = construct_pact(Mock(consumer_name='consumer', provider_name='provider',
-                                 version='2.0.0'), pact._interactions[0])
+    result = pact.construct_pact(pact._interactions[0])
     assert result == {
         'consumer': {'name': 'consumer'},
         'provider': {'name': 'provider'},
         'interactions': [
             {
                 'description': 'a request',
                 'providerState': 'the condition exists',
@@ -30,16 +50,15 @@
 def test_v3():
     pact = Consumer('consumer').has_pact_with(Provider('provider'), version='3.0.0')
     pact.given([
         dict(name="the condition exists", params={}),
         dict(name="the user exists", params=dict(username='alex')),
     ]).upon_receiving("a request").with_request("GET", "/path").will_respond_with(200, body='ok')
 
-    result = construct_pact(Mock(consumer_name='consumer', provider_name='provider',
-                                 version='3.0.0'), pact._interactions[0])
+    result = pact.construct_pact(pact._interactions[0])
     assert result == {
         'consumer': {'name': 'consumer'},
         'provider': {'name': 'provider'},
         'interactions': [
             {
                 'description': 'a request',
                 'providerStates': [
@@ -60,16 +79,15 @@
         Consumer('consumer').has_pact_with(Provider('provider'), version='3.0.0')
         .given("the condition exists")
         .and_given("the user exists", username='alex')
         .upon_receiving("a request").with_request("GET", "/path")
         .will_respond_with(200, body='ok')
     )
 
-    result = construct_pact(Mock(consumer_name='consumer', provider_name='provider',
-                                 version='3.0.0'), pact._interactions[0])
+    result = pact.construct_pact(pact._interactions[0])
     assert result == {
         'consumer': {'name': 'consumer'},
         'provider': {'name': 'provider'},
         'interactions': [
             {
                 'description': 'a request',
                 'providerStates': [
```

### Comparing `pactman-2.8.0/pactman/test/test_pact_generation.py` & `pactman-2.9.0/pactman/test/test_pact_generation.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,107 +1,133 @@
+import json
+import os
+import requests
+from unittest.mock import Mock, mock_open, patch
+
+import pactman.mock.pact
 import pytest
 import semver
-from unittest.mock import Mock, mock_open, patch
-import os
-from pactman.mock import pact_request_handler
-from pactman.mock.pact_request_handler import Config, MockPact, PactRequestHandler
+from pactman.mock.consumer import Consumer
+from pactman.mock.pact import Pact
+from pactman.mock.pact_request_handler import PactRequestHandler, PactVersionConflict
+from pactman.mock.provider import Provider
 
 
 @pytest.fixture
-def config_patched(monkeypatch):
-    monkeypatch.setattr(Config, "allocate_port", Mock())
-    monkeypatch.setattr(os, "remove", Mock())
-    monkeypatch.setattr(os.path, "exists", Mock())
-    os.path.exists.return_value = True
-    consumer_name = "CONSUMER"
-    provider_name = "PROVIDER"
-    log_dir = "/tmp/a"
-    pact_dir = "/tmp/pact"
-    version = "2.0.0"
-    my_conf = Config(consumer_name, provider_name, log_dir, pact_dir, None, version)
-    return my_conf
+def mock_pact(monkeypatch):
+    def f(file_write_mode=None, version='2.0.0'):
+        monkeypatch.setattr(Pact, "allocate_port", Mock())
+        monkeypatch.setattr(os, "remove", Mock())
+        monkeypatch.setattr(os.path, "exists", Mock(return_value=True))
+        log_dir = "/tmp/a"
+        pact_dir = "/tmp/pact"
+        return Pact(Consumer("CONSUMER"), Provider("PROVIDER"), log_dir=log_dir, pact_dir=pact_dir, version=version,
+                    file_write_mode=file_write_mode)
+    return f
 
 
 @pytest.mark.parametrize("file_write_mode", [None, "overwrite"])
-def test_config_init(monkeypatch, file_write_mode):
-    monkeypatch.setattr(Config, "allocate_port", Mock())
-    monkeypatch.setattr(Config, "pact_filename", Mock())
-    file_name = "/tmp/pact/JSON"
-    Config.pact_filename.return_value = file_name
-    monkeypatch.setattr(os, "remove", Mock())
-    monkeypatch.setattr(os.path, "exists", Mock(return_value=True))
-    monkeypatch.setattr(pact_request_handler, "ensure_pact_dir", Mock())
-
-    consumer_name = "CONSUMER"
-    provider_name = "PROVIDER"
-    log_dir = "/tmp/a"
-    pact_dir = "/tmp/pact"
-    version = "2.0.0"
-    my_conf = Config(consumer_name, provider_name, log_dir, pact_dir, file_write_mode, version)
-
-    assert(my_conf.consumer_name == consumer_name)
-    assert(my_conf.provider_name == provider_name)
-    assert(my_conf.log_dir == log_dir)
-    assert(my_conf.file_write_mode == file_write_mode)
-    assert(my_conf.version == version)
-    assert(my_conf.semver == semver.parse(version))
-    my_conf.allocate_port.assert_called_once_with()
-    assert(my_conf.PORT_NUMBER == 8150)
-    pact_request_handler.ensure_pact_dir.assert_called_once_with(pact_dir)
+def test_pact_init(monkeypatch, file_write_mode, mock_pact):
+    monkeypatch.setattr(pactman.mock.pact, 'ensure_pact_dir', Mock(return_value=True))
+    mock_pact = mock_pact(file_write_mode)
+    mock_pact.pact_filename()
+
+    assert(mock_pact.consumer.name == "CONSUMER")
+    assert(mock_pact.provider.name == "PROVIDER")
+    assert(mock_pact.log_dir == "/tmp/a")
+    assert(mock_pact.version == "2.0.0")
+    assert(mock_pact.semver == semver.parse("2.0.0"))
+    mock_pact.allocate_port.assert_called_once_with()
+    assert(mock_pact.BASE_PORT_NUMBER >= 8150)
+    pactman.mock.pact.ensure_pact_dir.assert_called_once_with("/tmp/pact")
     if file_write_mode == "overwrite":
-        my_conf.pact_filename.assert_called_once_with()
-        os.path.exists.assert_called_once_with(file_name)
-        os.remove.assert_called_once_with(file_name)
+        os.path.exists.assert_called_once_with("/tmp/pact/CONSUMER-PROVIDER-pact.json")
+        os.remove.assert_called_once_with("/tmp/pact/CONSUMER-PROVIDER-pact.json")
     else:
-        my_conf.pact_filename.assert_not_called()
+        os.path.exists.assert_not_called()
+        os.remove.assert_not_called()
 
 
-def test_config_pact_filename(config_patched):
-    res = config_patched.pact_filename()
-    assert(res == os.path.join(config_patched.pact_dir, "CONSUMER-PROVIDER-pact.json"))
+def test_config_pact_filename(mock_pact):
+    mock_pact = mock_pact()
+    res = mock_pact.pact_filename()
+    assert(res == os.path.join(mock_pact.pact_dir, "CONSUMER-PROVIDER-pact.json"))
 
 
 def test_ensure_pact_dir_when_exists(monkeypatch):
     monkeypatch.setattr(os.path, 'exists', Mock(side_effect=[True]))
     monkeypatch.setattr(os, 'mkdir', Mock())
-    pact_request_handler.ensure_pact_dir('/tmp/pacts')
+    pactman.mock.pact.ensure_pact_dir('/tmp/pacts')
     os.mkdir.assert_not_called()
 
 
 def test_ensure_pact_dir_when_parent_exists(monkeypatch):
     monkeypatch.setattr(os.path, 'exists', Mock(side_effect=[False, True]))
     monkeypatch.setattr(os, 'mkdir', Mock())
-    pact_request_handler.ensure_pact_dir('/tmp/pacts')
+    pactman.mock.pact.ensure_pact_dir('/tmp/pacts')
     os.mkdir.assert_called_once_with('/tmp/pacts')
 
 
-def test_mock_init(config_patched):
-    my_pact = MockPact(config_patched)
-    assert(my_pact.provider == config_patched.provider_name)
-    assert(my_pact.version == config_patched.version)
-    assert(my_pact.semver == config_patched.semver)
-
-
-def test_pact_request_handler_init(config_patched):
-    my_pact = PactRequestHandler(config_patched)
-    assert(my_pact.config == config_patched)
-
-
-@pytest.mark.parametrize("version", ["2.0.0", "3.0.0"])
-@patch("builtins.open", new_callable=mock_open, read_data="data")
-def test_pact_request_handler_write_pact(monkeypatch, config_patched, version):
-    config_patched.version = version
-    config_patched.semver = semver.parse(version)
-    my_pact = PactRequestHandler(config_patched)
-    os.path.exists.return_value = False
-    expected_pact = {
+def generate_pact(version):
+    return {
         "consumer": {"name": "CONSUMER"},
         "provider": {"name": "PROVIDER"},
-        "interactions": [None],
+        "interactions": [dict(description='spam')],
         "metadata": {
             'pactSpecification': {'version': version}
         }
     }
+
+
+@pytest.mark.parametrize("version", ["2.0.0", "3.0.0"])
+@patch("builtins.open", new_callable=mock_open, read_data="data")
+def test_pact_request_handler_write_pact(mock_open, monkeypatch, mock_pact, version):
+    monkeypatch.setattr(pactman.mock.pact, 'ensure_pact_dir', Mock(return_value=True))
+    mock_pact = mock_pact(version=version)
+    mock_pact.semver = semver.parse(version)
+    my_pact = PactRequestHandler(mock_pact)
+    os.path.exists.return_value = False
     with patch("json.dump", Mock()) as json_mock:
-        my_pact.write_pact(None)
-        open.assert_called_once_with(my_pact.config.pact_filename(), "w")
-        json_mock.assert_called_once_with(expected_pact, open(), indent=2)
+        my_pact.write_pact(dict(description='spam'))
+        mock_open.assert_called_once_with(mock_pact.pact_filename(), "w")
+        json_mock.assert_called_once_with(generate_pact(version), mock_open(), indent=2)
+
+
+@patch("builtins.open", new_callable=mock_open, read_data="data")
+def test_versions_are_consistent(mock_open, monkeypatch, mock_pact):
+    monkeypatch.setattr(pactman.mock.pact, 'ensure_pact_dir', Mock(return_value=True))
+    monkeypatch.setattr(json, 'dump', Mock())
+    monkeypatch.setattr(json, 'load', lambda f: generate_pact('2.0.0'))
+
+    # write the v2 pact
+    pact = mock_pact()
+    pact.semver = semver.parse(pact.version)
+    hdlr = PactRequestHandler(pact)
+    hdlr.write_pact(dict(description='spam'))
+
+    # try to add the v3 pact
+    pact = mock_pact(version='3.0.0')
+    pact.semver = semver.parse(pact.version)
+    hdlr = PactRequestHandler(pact)
+    with pytest.raises(PactVersionConflict):
+        hdlr.write_pact(dict(description='spam'))
+
+
+@patch("builtins.open", new_callable=mock_open, read_data="data")
+def test_immediate_pact_usage(mock_open):
+    pact = Consumer('C').has_pact_with(Provider('P')) \
+        .given("g").upon_receiving("r").with_request("get", "/", query={"foo": ["bar"]}).will_respond_with(200)
+    with pact:
+        requests.get(pact.uri, params={"foo": ["bar"]})
+
+    # force a failure
+    pact = Consumer('C').has_pact_with(Provider('P')) \
+        .given("g").upon_receiving("r").with_request("get", "/", query={"bar": ["foo"]}).will_respond_with(200)
+    with pytest.raises(AssertionError):
+        with pact:
+            requests.get(pact.uri, params={"foo": ["bar"]})
+
+    # make sure mocking still works
+    pact = Consumer('C').has_pact_with(Provider('P')) \
+        .given("g").upon_receiving("r").with_request("get", "/", query={"bar": ["foo"]}).will_respond_with(400)
+    with pact:
+        requests.get(pact.uri, params={"bar": ["foo"]})
```

### Comparing `pactman-2.8.0/pactman/test/test_mock_response.py` & `pactman-2.9.0/pactman/test/test_mock_response.py`

 * *Files identical despite different names*

### Comparing `pactman-2.8.0/pactman/test/test_parse_header.py` & `pactman-2.9.0/pactman/test/test_parse_header.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from pactman.verifier.parse_header import Part, parse_header
 
 
 def test_comma_whitespace_ignored():
     assert list(parse_header('spam, ham')) == list(parse_header('spam,ham'))
```

### Comparing `pactman-2.8.0/pactman/test/test_mock_consumer.py` & `pactman-2.9.0/pactman/test/test_mock_consumer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from unittest import TestCase
 from unittest.mock import Mock
 
 from pactman.mock.consumer import Consumer
-from pactman.mock.provider import Provider
 from pactman.mock.pact import Pact
+from pactman.mock.provider import Provider
 
 
 class ConsumerTestCase(TestCase):
     def setUp(self):
         self.mock_service = Mock(Pact)
         self.provider = Mock(Provider)
         self.consumer = Consumer('TestConsumer', service_cls=self.mock_service)
@@ -19,15 +19,15 @@
         self.assertIs(result.service_cls, Pact)
 
     def test_has_pact_with(self):
         result = self.consumer.has_pact_with(self.provider)
         self.assertIs(result, self.mock_service.return_value)
         self.mock_service.assert_called_once_with(
             consumer=self.consumer, provider=self.provider,
-            host_name='localhost', port=1234,
+            host_name='localhost', port=None,
             log_dir=None, ssl=False, sslcert=None, sslkey=None,
             pact_dir=None, version='2.0.0', use_mocking_server=False)
 
     def test_has_pact_with_customer_all_options(self):
         result = self.consumer.has_pact_with(
             self.provider, host_name='example.com', port=1111,
             log_dir='/logs', ssl=True,  sslcert='/ssl.cert', sslkey='ssl.pem',
```

### Comparing `pactman-2.8.0/pactman/test/test_mock_request.py` & `pactman-2.9.0/pactman/test/test_mock_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from unittest import TestCase
 
-from pactman import Term, Like
+from pactman import Like, Term
 from pactman.mock.request import Request
 
 
 class RequestTestCase(TestCase):
     def test_sparse(self):
         target = Request('GET', '/path')
         result = target.json('2.0.0')
```

### Comparing `pactman-2.8.0/pactman/test/test_verifier.py` & `pactman-2.9.0/pactman/test/test_verifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import json
 import pathlib
 from itertools import chain
 from unittest.mock import Mock
 
-import pytest
 import requests
-import semver
-from restnavigator import Navigator
 
+import pytest
+import semver
 from pactman.verifier.broker_pact import BrokerPact, BrokerPacts, pact_id
 from pactman.verifier.result import Result
-from pactman.verifier.verify import Interaction, RequestVerifier, ResponseVerifier
-
+from pactman.verifier.verify import (Interaction, RequestVerifier,
+                                     ResponseVerifier)
+from restnavigator import Navigator
 
 BASE_DIR = pathlib.Path(__file__).absolute().parents[0]
 
 
 def all_testcases(path, version):
     for entry in path.iterdir():
         if entry.is_file() and entry.suffix == '.json':
```

### Comparing `pactman-2.8.0/pactman/test/test_mock_pact.py` & `pactman-2.9.0/pactman/test/test_mock_pact.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import os
 from unittest import TestCase
-from unittest.mock import patch, call
+from unittest.mock import call, patch
 
 from pactman.mock.consumer import Consumer
-from pactman.mock.provider import Provider
 from pactman.mock.pact import Pact
+from pactman.mock.provider import Provider
 
 
 class PactTestCase(TestCase):
     def setUp(self):
         self.consumer = Consumer('TestConsumer')
         self.provider = Provider('TestProvider')
 
     def test_init_defaults(self):
         target = Pact(self.consumer, self.provider)
         self.assertIs(target.consumer, self.consumer)
         self.assertEqual(target.host_name, 'localhost')
         self.assertEqual(target.log_dir, os.getcwd())
         self.assertEqual(target.pact_dir, os.getcwd())
-        self.assertEqual(target.port, 1234)
+        self.assertEqual(target.port, Pact.BASE_PORT_NUMBER)
         self.assertIs(target.provider, self.provider)
         self.assertIs(target.ssl, False)
         self.assertIsNone(target.sslcert)
         self.assertIsNone(target.sslkey)
-        self.assertEqual(target.uri, 'http://localhost:1234')
+        self.assertEqual(target.uri, f'http://localhost:{Pact.BASE_PORT_NUMBER}')
         self.assertEqual(target.version, '2.0.0')
         self.assertEqual(len(target._interactions), 0)
 
     def test_init_custom_mock_service(self):
         target = Pact(
             self.consumer, self.provider, host_name='192.168.1.1', port=8000,
             log_dir='/logs', ssl=True, sslcert='/ssl.cert', sslkey='/ssl.pem',
```

### Comparing `pactman-2.8.0/pactman/test/test_mock_matchers.py` & `pactman-2.9.0/pactman/test/test_mock_matchers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from unittest import TestCase
 
-from pactman.mock.matchers import EachLike, Like, Matcher, SomethingLike, \
-    Term, from_term, get_generated_values
+from pactman.mock.matchers import (EachLike, Like, Matcher, SomethingLike,
+                                   Term, from_term, get_generated_values)
 
 
 class MatcherTestCase(TestCase):
     def test_generate(self):
         with self.assertRaises(NotImplementedError):
             Matcher().generate()
```

### Comparing `pactman-2.8.0/pactman/test/test_mock_urlopen.py` & `pactman-2.9.0/pactman/test/test_mock_urlopen.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # -*- encoding: utf8 -*-
-import urllib3
-from urllib3.response import HTTPResponse
 from unittest.mock import Mock, call, patch
+
+import urllib3
 import urllib3.poolmanager
+from urllib3.response import HTTPResponse
 
-from pactman.mock.mock_urlopen import patcher, MockURLOpenHandler
+from pactman.mock.mock_urlopen import MockURLOpenHandler, patcher
 
 
 def test_patched_urlopen_calls_service_with_request_parameters():
-    config = Mock(port=1234)
-    mock_service = Mock(config=config, return_value=HTTPResponse())
+    pact = Mock(port=1234)
+    mock_service = Mock(pact=pact, return_value=HTTPResponse())
     try:
         patcher.add_service(mock_service)
         http = urllib3.PoolManager()
         response = http.request('GET', 'http://api.test:1234/path')
     finally:
         patcher.remove_service(mock_service)
     assert mock_service.call_args == call('GET', '/path', body=None, headers={})
```

### Comparing `pactman-2.8.0/pactman/test/test_matching_rules.py` & `pactman-2.9.0/pactman/test/test_matching_rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import collections
 from unittest.mock import Mock
 
 import pytest
-
-from pactman.verifier.matching_rule import (
-    Matcher,
-    RuleFailed,
-    fold_type,
-    split_path,
-    weight_path,
-    MatchType, MatchNull, MatchInclude, MatchEquality, MatchNumber, MatchDecimal, MatchInteger, MatchRegex,
-    InvalidMatcher, log, rule_matchers_v3, rule_matchers_v2)
+from pactman.verifier.matching_rule import (InvalidMatcher, MatchDecimal,
+                                            MatchEquality, Matcher,
+                                            MatchInclude, MatchInteger,
+                                            MatchNull, MatchNumber, MatchRegex,
+                                            MatchType, RuleFailed, fold_type,
+                                            log, rule_matchers_v2,
+                                            rule_matchers_v3, split_path,
+                                            weight_path)
 
 
 def test_stringify():
     r = MatchType('$', {'match': 'type'})
     assert str(r) == "Rule match by {'match': 'type'} at $"
     assert repr(r) == "<MatchType path='$' rule={'match': 'type'}>"
```

### Comparing `pactman-2.8.0/pactman/mock/mock_urlopen.py` & `pactman-2.9.0/pactman/mock/mock_urlopen.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import io
 import logging
+
 import urllib3.connectionpool
 import urllib3.poolmanager
-
 from urllib3.response import HTTPResponse
 
 from .pact_request_handler import PactRequestHandler
 
 _providers = {}
 
 
@@ -14,19 +14,19 @@
 
 
 class MockPool:
     mocks = {}
 
     @classmethod
     def add_mock(cls, mock):
-        cls.mocks[mock.config.port] = mock
+        cls.mocks[mock.pact.port] = mock
 
     @classmethod
     def remove_mock(cls, mock):
-        del cls.mocks[mock.config.port]
+        del cls.mocks[mock.pact.port]
 
 
 class MockConnectionPool(urllib3.connectionpool.HTTPConnectionPool, MockPool):
     def urlopen(self, method, url, body=None, headers=None, *args, **kwargs):
         if self.port not in self.mocks:
             return super().urlopen(method, url, body, headers, *args, **kwargs)
         return self.mocks[self.port](method, url, body=body, headers=headers)
```

### Comparing `pactman-2.8.0/pactman/mock/mock_server.py` & `pactman-2.9.0/pactman/mock/mock_server.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import logging
 import queue
 import traceback
-from http.server import HTTPServer, BaseHTTPRequestHandler
+from http.server import BaseHTTPRequestHandler, HTTPServer
 from multiprocessing import Process, Queue
 
 from .pact_request_handler import PactRequestHandler
 
 _providers = {}
 
 
 log = logging.getLogger(__name__)
 
 
-def getMockServer(config):
-    if config.provider_name not in _providers:
-        _providers[config.provider_name] = Server(config)
-    return _providers[config.provider_name]
+def getMockServer(pact):
+    if pact.provider.name not in _providers:
+        _providers[pact.provider.name] = Server(pact)
+    return _providers[pact.provider.name]
 
 
 class Server:
-    def __init__(self, config):
-        self.config = config
+    def __init__(self, pact):
+        self.pact = pact
         self.interactions = Queue()
         self.results = Queue()
-        self.process = Process(target=run_server, args=(config, self.interactions, self.results))
+        self.process = Process(target=run_server, args=(pact, self.interactions, self.results))
         self.process.start()
 
     def setup(self, interactions):
         for interaction in interactions:
             self.interactions.put_nowait(interaction)
 
     def verify(self):
@@ -38,42 +38,42 @@
             if result['status'] == 'failed':
                 raise AssertionError(result['reason'])
 
     def terminate(self):
         self.process.terminate()
 
 
-def run_server(config, interactions, results):
-    httpd = MockServer(config, interactions, results)
+def run_server(pact, interactions, results):
+    httpd = MockServer(pact, interactions, results)
     httpd.serve_forever()
 
 
 class MockServer(HTTPServer):
-    def __init__(self, config, interactions, results):
-        self.config = config
+    def __init__(self, pact, interactions, results):
+        self.pact = pact
         self.incoming_interactions = interactions
         self.outgoing_results = results
-        server_address = ('', config.port)
+        server_address = ('', pact.port)
         super().__init__(server_address, MockHTTPRequestHandler)
         self.interactions = []
-        self.log = logging.getLogger(__name__ + '.' + config.provider_name)
-        self.log.addHandler(logging.FileHandler(f'{config.log_dir}/{config.provider_name}.log'))
+        self.log = logging.getLogger(__name__ + '.' + pact.provider.name)
+        self.log.addHandler(logging.FileHandler(f'{pact.log_dir}/{pact.provider.name}.log'))
         self.log.setLevel(logging.DEBUG)
         self.log.propagate = False
 
     class Error(Exception):
         pass
 
 
 class MockHTTPRequestHandler(BaseHTTPRequestHandler, PactRequestHandler):
     def __init__(self, request, client_address, server):
         self.response_status_code = None
         self.response_headers = {}
         self.response_body = None
-        PactRequestHandler.__init__(self, server.config)
+        PactRequestHandler.__init__(self, server.pact)
         BaseHTTPRequestHandler.__init__(self, request, client_address, server)
 
     def error_result(self, message, content='', status='error', status_code=500):
         self.server.outgoing_results.put({'status': status, 'reason': message})
         self.response_status_code = status_code
         self.response_headers = {'Content-Type': 'text/plain; charset=utf-8'}
         self.response_body = (content or message).encode('utf8')
```

### Comparing `pactman-2.8.0/pactman/mock/request.py` & `pactman-2.9.0/pactman/mock/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from .matchers import get_generated_values, get_matching_rules_v2, get_matching_rules_v3
+from .matchers import (get_generated_values, get_matching_rules_v2,
+                       get_matching_rules_v3)
 
 
 class Request:
     """Represents an HTTP request and supports Matchers on its properties."""
 
     def __init__(self, method, path, body=None, headers=None, query=''):
         """
```

### Comparing `pactman-2.8.0/pactman/mock/response.py` & `pactman-2.9.0/pactman/mock/response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from .matchers import get_generated_values, get_matching_rules_v2, get_matching_rules_v3
+from .matchers import (get_generated_values, get_matching_rules_v2,
+                       get_matching_rules_v3)
 
 
 class Response:
     """Represents an HTTP response and supports Matchers on its properties."""
 
     def __init__(self, status, headers=None, body=None):
         """
```

### Comparing `pactman-2.8.0/pactman/mock/consumer.py` & `pactman-2.9.0/pactman/mock/consumer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Classes and methods to describe contract Consumers."""
 import os
 
 from .pact import Pact
 from .provider import Provider
 
-
 USE_MOCKING_SERVER = os.environ.get('PACT_USE_MOCKING_SERVER', 'no') == 'yes'
 
 
 class Consumer(object):
     """
     A Pact consumer.
 
@@ -32,15 +31,15 @@
             for your mock service and want to use the same value on all of
             your contracts.
         :type service_cls: pact.Pact
         """
         self.name = name
         self.service_cls = service_cls
 
-    def has_pact_with(self, provider, host_name='localhost', port=1234,
+    def has_pact_with(self, provider, host_name='localhost', port=None,
                       log_dir=None, ssl=False, sslcert=None, sslkey=None,
                       pact_dir=None, version='2.0.0', use_mocking_server=USE_MOCKING_SERVER):
         """
         Create a contract between the `provider` and this consumer.
 
         If you are running the Pact mock service in a non-default location,
         you can provide the host name and port here:
@@ -57,15 +56,15 @@
         :param host_name: An optional host name to use when contacting the
             Pact mock service. This will need to be the same host name used by
             your code under test to contact the mock service. It defaults to:
             `localhost`.
         :type host_name: str
         :param port: The TCP port to use when contacting the Pact mock service.
             This will need to tbe the same port used by your code under test
-            to contact the mock service. It defaults to: 1234
+            to contact the mock service. It defaults to a port >= 8050.
         :type port: int
         :param log_dir: The directory where logs should be written. Defaults to
             the current directory.
         :type log_dir: str
         :param ssl: Flag to control the use of a self-signed SSL cert to run
             the server over HTTPS , defaults to False.
         :type ssl: bool
```

### Comparing `pactman-2.8.0/pactman/mock/matchers.py` & `pactman-2.9.0/pactman/mock/matchers.py`

 * *Files identical despite different names*

### Comparing `pactman-2.8.0/pactman/mock/pact.py` & `pactman-2.9.0/pactman/mock/pact.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 """API for creating a contract and configuring the mock service."""
 from __future__ import unicode_literals
 
 import os
 
 import semver
-from pactman.mock.request import Request
-from pactman.mock.response import Response
+
+from ..mock.request import Request
+from ..mock.response import Response
 from .mock_server import getMockServer
 from .mock_urlopen import MockURLOpenHandler
-from .pact_request_handler import Config
-
 
 USE_MOCKING_SERVER = os.environ.get('PACT_USE_MOCKING_SERVER', 'no') == 'yes'
 
 
+def ensure_pact_dir(pact_dir):
+    if not os.path.exists(pact_dir):
+        parent_dir = os.path.dirname(pact_dir)
+        if not os.path.exists(parent_dir):
+            raise ValueError(f'Pact destination directory {pact_dir} does not exist')
+        os.mkdir(pact_dir)
+
+
 class Pact(object):
     """
     Represents a contract between a consumer and provider.
 
     Provides Python context handlers to configure the Pact mock service to
     perform tests on a Python consumer. For example:
 
@@ -34,28 +41,29 @@
     was a GET to /echo with a query string with a key named `text` and its
     value is `Hello!`. If the request does not match an error is raised, if it
     does match the defined interaction, it will respond with the text `Hello!`.
     """
 
     HEADERS = {'X-Pact-Mock-Service': 'true'}
 
-    def __init__(self, consumer, provider, host_name='localhost', port=1234,
+    def __init__(self, consumer, provider, host_name='localhost', port=None,
                  log_dir=None, ssl=False, sslcert=None, sslkey=None,
                  pact_dir=None, version='2.0.0',
                  file_write_mode='overwrite', use_mocking_server=USE_MOCKING_SERVER):
         """
         Constructor for Pact.
 
         :param consumer: The consumer for this contract.
         :type consumer: pact.Consumer
         :param provider: The provider for this contract.
         :type provider: pact.Provider
         :param host_name: The host name where the mock service is running.
         :type host_name: str
-        :param port: The port number where the mock service is running.
+        :param port: The port number where the mock service is running. Defaults
+            to a port >= 8050.
         :type port: int
         :param log_dir: The directory where logs should be written. Defaults to
             the current directory.
         :type log_dir: str
         :param ssl: Flag to control the use of a self-signed SSL cert to run
             the server over HTTPS , defaults to False.
         :type ssl: bool
@@ -85,15 +93,15 @@
         """
         self.scheme = 'https' if ssl else 'http'
         self.consumer = consumer
         self.file_write_mode = file_write_mode
         self.host_name = host_name
         self.log_dir = log_dir or os.getcwd()
         self.pact_dir = pact_dir or os.getcwd()
-        self.port = port
+        self.port = port or self.allocate_port()
         self.provider = provider
         # TODO implement SSL
         self.ssl = ssl
         self.sslcert = sslcert
         self.sslkey = sslkey
         self.version = version
         self.semver = semver.parse(self.version)
@@ -101,14 +109,30 @@
         self._interactions = []
         self._mock_handler = None
 
     @property
     def uri(self):
         return '{scheme}://{host_name}:{port}'.format(host_name=self.host_name, port=self.port, scheme=self.scheme)
 
+    BASE_PORT_NUMBER = 8150
+
+    @classmethod
+    def allocate_port(cls):
+        cls.BASE_PORT_NUMBER += 5
+        return cls.BASE_PORT_NUMBER
+
+    def pact_filename(self):
+        # ensure destination directory exists
+        ensure_pact_dir(self.pact_dir)
+        filename = os.path.join(self.pact_dir, f'{self.consumer.name}-{self.provider.name}-pact.json')
+        if self.file_write_mode == 'overwrite':
+            if os.path.exists(filename):
+                os.remove(filename)
+        return filename
+
     def given(self, provider_state, **params):
         """
         Define the provider state for this pact.
 
         When the provider verifies this contract, they will use this field to
         setup pre-defined data that will satisfy the response expectations.
 
@@ -135,18 +159,26 @@
         provider state, with params taken from keyword arguments like so:
 
             .given("an alligator with the given name exists", name="Mary")
 
         If additional provider states are required for a v3 pact you may either use the list
         form above, or make an additional call to `.and_given()`.
 
+        If you don't have control over the provider, and they cannot implement a provider
+        state, you may use an explicit `None` for the provider state value. This is
+        discouraged as it introduces fragile external dependencies in your tests.
+
         :param provider_state: The state as described above.
         :type provider_state: string or list as above
         :rtype: Pact
         """
+        if provider_state is None:
+            self._interactions.insert(0, {})
+            return self
+
         if self.semver["major"] < 3:
             provider_state_key = 'providerState'
             if not isinstance(provider_state, str):
                 raise ValueError('pact v2 provider states must be strings')
         else:
             provider_state_key = 'providerStates'
             if isinstance(provider_state, str):
@@ -175,23 +207,19 @@
         self._interactions[-1]['providerStates'].append({'name': provider_state, 'params': params})
         return self
 
     def setup(self):
         self._mock_handler.setup(self._interactions)
 
     def start_mocking(self):
-        # TODO hmm, the config is looking a lot like this Pact instance...
-        config = Config(self.consumer.name, self.provider.name, self.log_dir, self.pact_dir, self.file_write_mode,
-                        self.version)
-        self.port = config.port
         if self.use_mocking_server:
-            self._mock_handler = getMockServer(config)
+            self._mock_handler = getMockServer(self)
         else:
             # ain't no port, we're monkey-patching (but the URLs we generate still need to look correct)
-            self._mock_handler = MockURLOpenHandler(config)
+            self._mock_handler = MockURLOpenHandler(self)
 
     def stop_mocking(self):
         self._mock_handler.terminate()
 
     # legacy pact-python API support
     start_service = start_mocking
     stop_service = stop_mocking
@@ -260,26 +288,45 @@
         :rtype: Pact
         """
         self._interactions[0]['response'] = Response(status,
                                                      headers=headers,
                                                      body=body).json(self.version)
         return self
 
+    _auto_mocked = False
+
     def __enter__(self):
         """
         Handler for entering a Python context.
 
         Sets up the mock service to expect the client requests.
         """
+        if not self.use_mocking_server and not self._mock_handler:
+            self._auto_mocked = True
+            self.start_mocking()
+
         self.setup()
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         """
         Handler for exiting a Python context.
 
         Calls the mock service to verify that all interactions occurred as
         expected, and has it write out the contracts to disk.
         """
         if (exc_type, exc_val, exc_tb) != (None, None, None):
             return
 
         self.verify()
+
+        if not self.use_mocking_server and self._auto_mocked:
+            self.stop_mocking()
+
+    def construct_pact(self, interaction):
+        """Construct a pact JSON data structure for the interaction.
+        """
+        return dict(
+            consumer={"name": self.consumer.name},
+            provider={"name": self.provider.name},
+            interactions=[interaction],
+            metadata=dict(pactSpecification=dict(version=self.version)),
+        )
```

### Comparing `pactman-2.8.0/pactman/verifier/broker_pact.py` & `pactman-2.9.0/pactman/verifier/broker_pact.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 import semver
 from restnavigator import Navigator
 
 from .result import LoggedResult
 from .verify import Interaction
 
-
 log = logging.getLogger(__name__)
 log.setLevel(logging.DEBUG)
 
 
 def pact_id(param):
     return repr(param)
```

### Comparing `pactman-2.8.0/pactman/verifier/command_line.py` & `pactman-2.9.0/pactman/verifier/command_line.py`

 * *Files identical despite different names*

### Comparing `pactman-2.8.0/pactman/verifier/result.py` & `pactman-2.9.0/pactman/verifier/result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import logging
 
-
 log = logging.getLogger(__name__)
 
 
 class Result:
     PASS = True
     FAIL = False
     success = PASS
```

### Comparing `pactman-2.8.0/pactman/verifier/parse_header.py` & `pactman-2.9.0/pactman/verifier/parse_header.py`

 * *Files identical despite different names*

### Comparing `pactman-2.8.0/pactman/verifier/verify.py` & `pactman-2.9.0/pactman/verifier/verify.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import logging
 from urllib.parse import parse_qs, urljoin
 
 import requests
 
-from .matching_rule import fold_type, nice_type, rule_matchers_v2, rule_matchers_v3, RuleFailed
+from .matching_rule import (RuleFailed, fold_type, nice_type, rule_matchers_v2,
+                            rule_matchers_v3)
 from .parse_header import parse_header
 from .paths import format_path
 
-
 log = logging.getLogger(__name__)
 log.setLevel(logging.DEBUG)
 
 
 class ProviderStateError(Exception):
     pass
 
@@ -397,15 +397,15 @@
                 return self.result.fail(f'Request path {request.path!r} does not match expected {self.path!r}')
         if self.query is not MISSING:
             if not self.verify_query(self.query, request):
                 return False
         return super().verify(request)
 
     def verify_query(self, spec_query, request):
-        if self.pact.semver['major'] < 3:
+        if isinstance(spec_query, str):
             spec_query = parse_qs(spec_query)
         request_query = request.query
         if isinstance(request_query, str):
             request_query = parse_qs(request_query)
         if self.pact.semver['major'] > 1 and self.matching_rules.get('query'):
             if not self.apply_rules(request_query, spec_query, ['query']):
                 return self.result.fail(f'Request query params {request_query} do not match '
```

### Comparing `pactman-2.8.0/pactman/verifier/matching_rule.py` & `pactman-2.9.0/pactman/verifier/matching_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 """
 import logging
 import re
 from collections import OrderedDict, defaultdict
 
 from .paths import format_path
 
-
 log = logging.getLogger(__name__)
 
 
 class RuleFailed(Exception):
     def __init__(self, path, message):
         if isinstance(path, list):
             path = format_path(path)
```

### Comparing `pactman-2.8.0/CONTRIBUTING.md` & `pactman-2.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

