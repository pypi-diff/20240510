# Comparing `tmp/hexkit-3.0.1.tar.gz` & `tmp/hexkit-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hexkit-3.0.1.tar", last modified: Mon May  6 16:04:18 2024, max compression
+gzip compressed data, was "hexkit-3.0.2.tar", last modified: Fri May 10 13:41:08 2024, max compression
```

## Comparing `hexkit-3.0.1.tar` & `hexkit-3.0.2.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:04:18.910359 hexkit-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11452 2024-05-06 16:04:15.000000 hexkit-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-06 16:04:15.000000 hexkit-3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7634 2024-05-06 16:04:18.910359 hexkit-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5728 2024-05-06 16:04:15.000000 hexkit-3.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-05-06 16:04:15.000000 hexkit-3.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 16:04:18.910359 hexkit-3.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:04:18.898359 hexkit-3.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:04:18.898359 hexkit-3.0.1/src/hexkit/
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/correlation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:04:18.902359 hexkit-3.0.1/src/hexkit/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16935 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/protocols/dao.py
--rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/protocols/daopub.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/protocols/daosub.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/protocols/eventpub.py
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/protocols/eventsub.py
--rw-r--r--   0 runner    (1001) docker     (127)    24781 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/protocols/objstorage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:04:18.902359 hexkit-3.0.1/src/hexkit/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:04:18.902359 hexkit-3.0.1/src/hexkit/providers/akafka/
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/akafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/akafka/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:04:18.902359 hexkit-3.0.1/src/hexkit/providers/akafka/provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/akafka/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/akafka/provider/daosub.py
--rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/akafka/provider/eventpub.py
--rw-r--r--   0 runner    (1001) docker     (127)     9274 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/akafka/provider/eventsub.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/akafka/provider/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/akafka/testcontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)    19083 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/akafka/testutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:04:18.906359 hexkit-3.0.1/src/hexkit/providers/mongodb/
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/mongodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18352 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/mongodb/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/mongodb/testutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:04:18.906359 hexkit-3.0.1/src/hexkit/providers/mongokafka/
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/mongokafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16185 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/mongokafka/provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:04:18.906359 hexkit-3.0.1/src/hexkit/providers/s3/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33195 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/s3/provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:04:18.906359 hexkit-3.0.1/src/hexkit/providers/s3/test_files/
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/s3/test_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/s3/test_files/test_file1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/s3/test_files/test_file2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/s3/test_files/test_file3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/s3/test_files/test_file4.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    15760 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/s3/testutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:04:18.906359 hexkit-3.0.1/src/hexkit/providers/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/testing/eventpub.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:04:18.906359 hexkit-3.0.1/src/hexkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7634 2024-05-06 16:04:18.000000 hexkit-3.0.1/src/hexkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-06 16:04:18.000000 hexkit-3.0.1/src/hexkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:04:18.000000 hexkit-3.0.1/src/hexkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-06 16:04:18.000000 hexkit-3.0.1/src/hexkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-06 16:04:18.000000 hexkit-3.0.1/src/hexkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:41:08.899418 hexkit-3.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11452 2024-05-10 13:41:02.000000 hexkit-3.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-10 13:41:02.000000 hexkit-3.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7634 2024-05-10 13:41:08.895418 hexkit-3.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5728 2024-05-10 13:41:02.000000 hexkit-3.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-05-10 13:41:02.000000 hexkit-3.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 13:41:08.899418 hexkit-3.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:41:08.883418 hexkit-3.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:41:08.887418 hexkit-3.0.2/src/hexkit/
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:41:08.891418 hexkit-3.0.2/src/hexkit/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16932 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/protocols/dao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/protocols/daopub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/protocols/daosub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/protocols/eventpub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/protocols/eventsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24781 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/protocols/objstorage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:41:08.891418 hexkit-3.0.2/src/hexkit/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:41:08.891418 hexkit-3.0.2/src/hexkit/providers/akafka/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/akafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/akafka/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:41:08.891418 hexkit-3.0.2/src/hexkit/providers/akafka/provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/akafka/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/akafka/provider/daosub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/akafka/provider/eventpub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9274 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/akafka/provider/eventsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/akafka/provider/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/akafka/testcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19083 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/akafka/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:41:08.891418 hexkit-3.0.2/src/hexkit/providers/mongodb/
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/mongodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18349 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/mongodb/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/mongodb/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:41:08.891418 hexkit-3.0.2/src/hexkit/providers/mongokafka/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/mongokafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16534 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/mongokafka/provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:41:08.895418 hexkit-3.0.2/src/hexkit/providers/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33195 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/s3/provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:41:08.895418 hexkit-3.0.2/src/hexkit/providers/s3/test_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/s3/test_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/s3/test_files/test_file1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/s3/test_files/test_file2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/s3/test_files/test_file3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/s3/test_files/test_file4.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    15760 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/s3/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:41:08.895418 hexkit-3.0.2/src/hexkit/providers/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/providers/testing/eventpub.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-10 13:41:02.000000 hexkit-3.0.2/src/hexkit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:41:08.895418 hexkit-3.0.2/src/hexkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7634 2024-05-10 13:41:08.000000 hexkit-3.0.2/src/hexkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-10 13:41:08.000000 hexkit-3.0.2/src/hexkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 13:41:08.000000 hexkit-3.0.2/src/hexkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-10 13:41:08.000000 hexkit-3.0.2/src/hexkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 13:41:08.000000 hexkit-3.0.2/src/hexkit.egg-info/top_level.txt
```

### Comparing `hexkit-3.0.1/LICENSE` & `hexkit-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.1/PKG-INFO` & `hexkit-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hexkit
-Version: 3.0.1
+Version: 3.0.2
 Summary: A Toolkit for Building Microservices using the Hexagonal Architecture
 Author-email: "German Human Genome Phenome Archive (GHGA)" <contact@ghga.de>
 License: Apache 2.0
 Project-URL: Repository, https://github.com/ghga-de/hexkit
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `hexkit-3.0.1/README.md` & `hexkit-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.1/pyproject.toml` & `hexkit-3.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: Apache Software License",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Software Development :: Libraries",
     "Intended Audience :: Developers",
 ]
 name = "hexkit"
-version = "3.0.1"
+version = "3.0.2"
 description = "A Toolkit for Building Microservices using the Hexagonal Architecture"
 dependencies = [
     "pydantic >=2, <3",
     "pydantic_settings >=2, <3",
     "PyYAML >=6.0, <7",
 ]
```

### Comparing `hexkit-3.0.1/src/hexkit/__init__.py` & `hexkit-3.0.2/src/hexkit/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.1/src/hexkit/__main__.py` & `hexkit-3.0.2/src/hexkit/__main__.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.1/src/hexkit/base.py` & `hexkit-3.0.2/src/hexkit/base.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.1/src/hexkit/config.py` & `hexkit-3.0.2/src/hexkit/config.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.1/src/hexkit/correlation.py` & `hexkit-3.0.2/src/hexkit/correlation.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.1/src/hexkit/custom_types.py` & `hexkit-3.0.2/src/hexkit/custom_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from collections.abc import Mapping, Sequence
 from typing import Any, Literal, Union
 
 # This is intended to type objects that could be a potential output of `json.loads`.
 # (Scalar types as well as arrays are excluded from the above assumption.)
 JsonObject = Mapping[
-    str, Union[int, float, str, bool, Sequence[Any], Mapping[str, Any]]
+    str, Union[int, float, str, bool, Sequence[Any], Mapping[str, Any], None]
 ]
 
 
 # A type indicating that a string should be ascii-compatible.
 # Technically it is an alias for `str` so it only serves documention purposes.
 Ascii = str
```

### Comparing `hexkit-3.0.1/src/hexkit/log.py` & `hexkit-3.0.2/src/hexkit/log.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.1/src/hexkit/protocols/__init__.py` & `hexkit-3.0.2/src/hexkit/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.1/src/hexkit/protocols/dao.py` & `hexkit-3.0.2/src/hexkit/protocols/dao.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
 
         Raises:
             ResourceNotFoundError:
                 when resource with the id specified in the dto was not found
         """
         ...
 
-    async def delete(self, *, id_: str) -> None:
+    async def delete(self, id_: str) -> None:
         """Delete a resource by providing its ID.
 
         Args:
             id_: The ID of the resource.
 
         Raises:
             ResourceNotFoundError: when resource with the specified id_ was not found
```

### Comparing `hexkit-3.0.1/src/hexkit/protocols/daopub.py` & `hexkit-3.0.2/src/hexkit/protocols/daopub.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.1/src/hexkit/protocols/daosub.py` & `hexkit-3.0.2/src/hexkit/protocols/daosub.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.1/src/hexkit/protocols/eventpub.py` & `hexkit-3.0.2/src/hexkit/protocols/eventpub.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.1/src/hexkit/protocols/eventsub.py` & `hexkit-3.0.2/src/hexkit/protocols/eventsub.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.1/src/hexkit/protocols/objstorage.py` & `hexkit-3.0.2/src/hexkit/protocols/objstorage.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.1/src/hexkit/providers/__init__.py` & `hexkit-3.0.2/src/hexkit/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.1/src/hexkit/providers/akafka/__init__.py` & `hexkit-3.0.2/src/hexkit/providers/akafka/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.1/src/hexkit/providers/akafka/config.py` & `hexkit-3.0.2/src/hexkit/providers/akafka/config.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.1/src/hexkit/providers/akafka/provider/__init__.py` & `hexkit-3.0.2/src/hexkit/providers/akafka/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.1/src/hexkit/providers/akafka/provider/daosub.py` & `hexkit-3.0.2/src/hexkit/providers/akafka/provider/daosub.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.1/src/hexkit/providers/akafka/provider/eventpub.py` & `hexkit-3.0.2/src/hexkit/providers/akafka/provider/eventpub.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.1/src/hexkit/providers/akafka/provider/eventsub.py` & `hexkit-3.0.2/src/hexkit/providers/akafka/provider/eventsub.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.1/src/hexkit/providers/akafka/provider/utils.py` & `hexkit-3.0.2/src/hexkit/providers/akafka/provider/utils.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.1/src/hexkit/providers/akafka/testcontainer.py` & `hexkit-3.0.2/src/hexkit/providers/akafka/testcontainer.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.1/src/hexkit/providers/akafka/testutils.py` & `hexkit-3.0.2/src/hexkit/providers/akafka/testutils.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.1/src/hexkit/providers/mongodb/__init__.py` & `hexkit-3.0.2/src/hexkit/providers/mongodb/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.1/src/hexkit/providers/mongodb/provider.py` & `hexkit-3.0.2/src/hexkit/providers/mongodb/provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,15 +197,15 @@
 
         if result.matched_count == 0:
             raise ResourceNotFoundError(id_=document["_id"])
 
         # (trusting MongoDB that matching on the _id field can only yield one or
         # zero matches)
 
-    async def delete(self, *, id_: str) -> None:
+    async def delete(self, id_: str) -> None:
         """Delete a resource by providing its ID.
 
         Args:
             id_: The ID of the resource.
 
         Raises:
             ResourceNotFoundError: when resource with the specified id_ was not found
```

### Comparing `hexkit-3.0.1/src/hexkit/providers/mongodb/testutils.py` & `hexkit-3.0.2/src/hexkit/providers/mongodb/testutils.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.1/src/hexkit/providers/mongokafka/__init__.py` & `hexkit-3.0.2/src/hexkit/providers/mongokafka/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.1/src/hexkit/providers/mongokafka/provider.py` & `hexkit-3.0.2/src/hexkit/providers/mongokafka/provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,15 @@
             payload={},
             type_=DELETE_EVENT_TYPE,
             key=id_,
             topic=event_topic,
         )
 
         document = {"_id": id_, "__metadata__": {"deleted": True, "published": True}}
-        await collection.replace_one({"_id": document["_id"]}, document, upsert=True)
+        await collection.replace_one({"_id": document["_id"]}, document)
 
     return publish_deletion
 
 
 @contextmanager
 def assert_not_deleted():
     """A context manager that translates ResourceDeletedError into ResourceNotFoundError."""
@@ -229,33 +229,42 @@
                 The updated resource content as a pydantic-based data transfer object
                 including the resource ID.
 
         Raises:
             ResourceNotFoundError:
                 when resource with the id specified in the dto was not found
         """
-        with assert_not_deleted():
-            await self._dao.update(dto)
+        document = self._dao._dto_to_document(dto)
+        result = await self._collection.replace_one(
+            {"_id": document["_id"], "__metadata__.deleted": False}, document
+        )
+        if result.matched_count == 0:
+            raise ResourceNotFoundError(id_=document["_id"])
 
         if self._autopublish:
             await self._publish_change(dto)
 
-    async def delete(self, *, id_: str) -> None:
+    async def delete(self, id_: str) -> None:
         """Delete a resource by providing its ID.
 
         Args:
             id_: The ID of the resource.
 
         Raises:
             ResourceNotFoundError: when resource with the specified id_ was not found
         """
-        document = {"_id": id_, "__metadata__": {"deleted": True, "published": False}}
-        await self._collection.replace_one(
-            {"_id": document["_id"]}, document, upsert=True
+        document = {
+            "_id": id_,
+            "__metadata__": {"deleted": True, "published": False},
+        }
+        result = await self._collection.replace_one(
+            {"_id": document["_id"], "__metadata__.deleted": False}, document
         )
+        if result.matched_count == 0:
+            raise ResourceNotFoundError(id_=id_)
 
         if self._autopublish:
             await self._publish_delete(id_)
 
     async def find_one(self, *, mapping: Mapping[str, Any]) -> Dto:
         """Find the resource that matches the specified mapping. It is expected that
         at most one resource matches the constraints. An exception is raised if no or
```

### Comparing `hexkit-3.0.1/src/hexkit/providers/s3/__init__.py` & `hexkit-3.0.2/src/hexkit/providers/s3/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.1/src/hexkit/providers/s3/provider.py` & `hexkit-3.0.2/src/hexkit/providers/s3/provider.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.1/src/hexkit/providers/s3/test_files/__init__.py` & `hexkit-3.0.2/src/hexkit/providers/s3/test_files/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.1/src/hexkit/providers/s3/testutils.py` & `hexkit-3.0.2/src/hexkit/providers/s3/testutils.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.1/src/hexkit/providers/testing/__init__.py` & `hexkit-3.0.2/src/hexkit/providers/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.1/src/hexkit/providers/testing/eventpub.py` & `hexkit-3.0.2/src/hexkit/providers/testing/eventpub.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.1/src/hexkit/utils.py` & `hexkit-3.0.2/src/hexkit/utils.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.1/src/hexkit.egg-info/PKG-INFO` & `hexkit-3.0.2/src/hexkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hexkit
-Version: 3.0.1
+Version: 3.0.2
 Summary: A Toolkit for Building Microservices using the Hexagonal Architecture
 Author-email: "German Human Genome Phenome Archive (GHGA)" <contact@ghga.de>
 License: Apache 2.0
 Project-URL: Repository, https://github.com/ghga-de/hexkit
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `hexkit-3.0.1/src/hexkit.egg-info/SOURCES.txt` & `hexkit-3.0.2/src/hexkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

