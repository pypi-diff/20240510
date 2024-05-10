# Comparing `tmp/superblocks-types-0.0.1.tar.gz` & `tmp/superblocks-types-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superblocks-types-0.0.1.tar", last modified: Fri May 10 20:49:05 2024, max compression
+gzip compressed data, was "superblocks-types-0.0.2.tar", last modified: Fri May 10 20:51:09 2024, max compression
```

## Comparing `superblocks-types-0.0.1.tar` & `superblocks-types-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-10 20:49:05.909990 superblocks-types-0.0.1/
--rw-r--r--   0 joeygreco   (501) staff       (20)     3181 2024-05-10 20:49:05.909802 superblocks-types-0.0.1/PKG-INFO
--rw-r--r--   0 joeygreco   (501) staff       (20)     2857 2023-10-13 17:42:57.000000 superblocks-types-0.0.1/README.md
--rw-r--r--   0 joeygreco   (501) staff       (20)       38 2024-05-10 20:49:05.910062 superblocks-types-0.0.1/setup.cfg
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-10 20:49:05.909530 superblocks-types-0.0.1/superblocks_types.egg-info/
--rw-r--r--   0 joeygreco   (501) staff       (20)     3181 2024-05-10 20:49:05.000000 superblocks-types-0.0.1/superblocks_types.egg-info/PKG-INFO
--rw-r--r--   0 joeygreco   (501) staff       (20)      173 2024-05-10 20:49:05.000000 superblocks-types-0.0.1/superblocks_types.egg-info/SOURCES.txt
--rw-r--r--   0 joeygreco   (501) staff       (20)        1 2024-05-10 20:49:05.000000 superblocks-types-0.0.1/superblocks_types.egg-info/dependency_links.txt
--rw-r--r--   0 joeygreco   (501) staff       (20)        1 2024-05-10 20:49:05.000000 superblocks-types-0.0.1/superblocks_types.egg-info/top_level.txt
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-10 20:51:09.923549 superblocks-types-0.0.2/
+-rw-r--r--   0 joeygreco   (501) staff       (20)      694 2024-05-10 20:51:09.923365 superblocks-types-0.0.2/PKG-INFO
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2857 2023-10-13 17:42:57.000000 superblocks-types-0.0.2/README.md
+-rw-r--r--   0 joeygreco   (501) staff       (20)       38 2024-05-10 20:51:09.923657 superblocks-types-0.0.2/setup.cfg
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-10 20:51:09.923120 superblocks-types-0.0.2/superblocks_types.egg-info/
+-rw-r--r--   0 joeygreco   (501) staff       (20)      694 2024-05-10 20:51:09.000000 superblocks-types-0.0.2/superblocks_types.egg-info/PKG-INFO
+-rw-r--r--   0 joeygreco   (501) staff       (20)      173 2024-05-10 20:51:09.000000 superblocks-types-0.0.2/superblocks_types.egg-info/SOURCES.txt
+-rw-r--r--   0 joeygreco   (501) staff       (20)        1 2024-05-10 20:51:09.000000 superblocks-types-0.0.2/superblocks_types.egg-info/dependency_links.txt
+-rw-r--r--   0 joeygreco   (501) staff       (20)        1 2024-05-10 20:51:09.000000 superblocks-types-0.0.2/superblocks_types.egg-info/top_level.txt
```

### Comparing `superblocks-types-0.0.1/PKG-INFO` & `superblocks-types-0.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: superblocks-types
-Version: 0.0.1
-Summary: The Official Python Types for Superblocks
-Home-page: https://github.com/superblocksteam/types
-Author: Joey Greco
-Author-email: joeyagreco@gmail.com
-License: MIT
-Keywords: superblocks types
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-
 # types
 
 [![default](https://github.com/superblocksteam/types/actions/workflows/default.yaml/badge.svg)](https://github.com/superblocksteam/types/actions/workflows/default.yaml)
 
 ## About
 
 This is the **NEW HOME** for Superblocks types as we migrate to Protobuf! Unsure if you're type should live here? If you answer **yes** to any of the following, it should live here! Still not sure? Ask Frank!
```

