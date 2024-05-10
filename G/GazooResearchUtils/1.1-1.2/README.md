# Comparing `tmp/GazooResearchUtils-1.1.tar.gz` & `tmp/GazooResearchUtils-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GazooResearchUtils-1.1.tar", last modified: Fri May 10 21:16:46 2024, max compression
+gzip compressed data, was "GazooResearchUtils-1.2.tar", last modified: Fri May 10 21:32:41 2024, max compression
```

## Comparing `GazooResearchUtils-1.1.tar` & `GazooResearchUtils-1.2.tar`

### file list

```diff
@@ -1,19 +1,16 @@
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-10 21:16:46.530693 GazooResearchUtils-1.1/
--rw-r--r--   0 andrewlim   (501) staff       (20)      331 2024-05-10 21:16:46.530458 GazooResearchUtils-1.1/PKG-INFO
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-10 21:16:46.528116 GazooResearchUtils-1.1/app/
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-10 21:16:46.528582 GazooResearchUtils-1.1/app/GazooResearchUtils/
--rw-r--r--   0 andrewlim   (501) staff       (20)      242 2024-05-10 21:10:14.000000 GazooResearchUtils-1.1/app/GazooResearchUtils/__init__.py
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-10 21:16:46.530200 GazooResearchUtils-1.1/app/GazooResearchUtils/src/
--rw-r--r--   0 andrewlim   (501) staff       (20)    13006 2024-05-10 21:10:14.000000 GazooResearchUtils-1.1/app/GazooResearchUtils/src/Analysis.py
--rw-r--r--   0 andrewlim   (501) staff       (20)     1322 2024-05-10 21:10:14.000000 GazooResearchUtils-1.1/app/GazooResearchUtils/src/DB.py
--rw-r--r--   0 andrewlim   (501) staff       (20)    39864 2024-05-10 21:10:14.000000 GazooResearchUtils-1.1/app/GazooResearchUtils/src/Database.py
--rw-r--r--   0 andrewlim   (501) staff       (20)     4380 2024-05-10 21:10:14.000000 GazooResearchUtils-1.1/app/GazooResearchUtils/src/TableOne.py
--rw-r--r--   0 andrewlim   (501) staff       (20)        0 2024-05-10 21:10:14.000000 GazooResearchUtils-1.1/app/GazooResearchUtils/src/__init__.py
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-10 21:16:46.529338 GazooResearchUtils-1.1/app/GazooResearchUtils.egg-info/
--rw-r--r--   0 andrewlim   (501) staff       (20)      331 2024-05-10 21:16:46.000000 GazooResearchUtils-1.1/app/GazooResearchUtils.egg-info/PKG-INFO
--rw-r--r--   0 andrewlim   (501) staff       (20)      461 2024-05-10 21:16:46.000000 GazooResearchUtils-1.1/app/GazooResearchUtils.egg-info/SOURCES.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)        1 2024-05-10 21:16:46.000000 GazooResearchUtils-1.1/app/GazooResearchUtils.egg-info/dependency_links.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)       46 2024-05-10 21:16:46.000000 GazooResearchUtils-1.1/app/GazooResearchUtils.egg-info/requires.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)       19 2024-05-10 21:16:46.000000 GazooResearchUtils-1.1/app/GazooResearchUtils.egg-info/top_level.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)       38 2024-05-10 21:16:46.530750 GazooResearchUtils-1.1/setup.cfg
--rw-r--r--   0 andrewlim   (501) staff       (20)      458 2024-05-10 21:12:39.000000 GazooResearchUtils-1.1/setup.py
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-10 21:32:41.244994 GazooResearchUtils-1.2/
+-rw-r--r--   0 andrewlim   (501) staff       (20)      331 2024-05-10 21:32:41.244715 GazooResearchUtils-1.2/PKG-INFO
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-10 21:32:41.242711 GazooResearchUtils-1.2/app/
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-10 21:32:41.243182 GazooResearchUtils-1.2/app/GazooResearchUtils/
+-rw-r--r--   0 andrewlim   (501) staff       (20)       70 2024-05-10 21:31:29.000000 GazooResearchUtils-1.2/app/GazooResearchUtils/__init__.py
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-10 21:32:41.244339 GazooResearchUtils-1.2/app/GazooResearchUtils/src/
+-rw-r--r--   0 andrewlim   (501) staff       (20)     4498 2024-05-10 21:30:10.000000 GazooResearchUtils-1.2/app/GazooResearchUtils/src/Analysis.py
+-rw-r--r--   0 andrewlim   (501) staff       (20)        0 2024-05-10 21:10:14.000000 GazooResearchUtils-1.2/app/GazooResearchUtils/src/__init__.py
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-10 21:32:41.243961 GazooResearchUtils-1.2/app/GazooResearchUtils.egg-info/
+-rw-r--r--   0 andrewlim   (501) staff       (20)      331 2024-05-10 21:32:41.000000 GazooResearchUtils-1.2/app/GazooResearchUtils.egg-info/PKG-INFO
+-rw-r--r--   0 andrewlim   (501) staff       (20)      350 2024-05-10 21:32:41.000000 GazooResearchUtils-1.2/app/GazooResearchUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)        1 2024-05-10 21:32:41.000000 GazooResearchUtils-1.2/app/GazooResearchUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)       46 2024-05-10 21:32:41.000000 GazooResearchUtils-1.2/app/GazooResearchUtils.egg-info/requires.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)       19 2024-05-10 21:32:41.000000 GazooResearchUtils-1.2/app/GazooResearchUtils.egg-info/top_level.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)       38 2024-05-10 21:32:41.245055 GazooResearchUtils-1.2/setup.cfg
+-rw-r--r--   0 andrewlim   (501) staff       (20)      458 2024-05-10 21:30:25.000000 GazooResearchUtils-1.2/setup.py
```

