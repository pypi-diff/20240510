# Comparing `tmp/natanstanek-0.14.0.tar.gz` & `tmp/natanstanek-0.14.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "natanstanek-0.14.0.tar", last modified: Fri May 10 09:35:58 2024, max compression
+gzip compressed data, was "natanstanek-0.14.1.tar", last modified: Fri May 10 09:43:03 2024, max compression
```

## Comparing `natanstanek-0.14.0.tar` & `natanstanek-0.14.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 09:35:58.508044 natanstanek-0.14.0/
-drwxrwxrwx   0        0        0        0 2024-05-10 09:35:58.444048 natanstanek-0.14.0/NatanStanek/
--rw-rw-rw-   0        0        0      233 2024-05-10 09:35:54.000000 natanstanek-0.14.0/NatanStanek/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 09:35:58.502325 natanstanek-0.14.0/NatanStanek.egg-info/
--rw-rw-rw-   0        0        0      250 2024-05-10 09:35:58.000000 natanstanek-0.14.0/NatanStanek.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2024-05-10 09:35:58.000000 natanstanek-0.14.0/NatanStanek.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 09:35:58.000000 natanstanek-0.14.0/NatanStanek.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-08 12:52:30.000000 natanstanek-0.14.0/NatanStanek.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2024-05-10 09:35:58.000000 natanstanek-0.14.0/NatanStanek.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      250 2024-05-10 09:35:58.504721 natanstanek-0.14.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-10 09:35:58.508461 natanstanek-0.14.0/setup.cfg
--rw-rw-rw-   0        0        0      388 2024-05-10 09:35:50.000000 natanstanek-0.14.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:43:03.063538 natanstanek-0.14.1/
+drwxrwxrwx   0        0        0        0 2024-05-10 09:43:03.025382 natanstanek-0.14.1/NatanStanek/
+-rw-rw-rw-   0        0        0      673 2024-05-10 09:42:57.000000 natanstanek-0.14.1/NatanStanek/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:43:03.057946 natanstanek-0.14.1/NatanStanek.egg-info/
+-rw-rw-rw-   0        0        0      250 2024-05-10 09:43:02.000000 natanstanek-0.14.1/NatanStanek.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      206 2024-05-10 09:43:02.000000 natanstanek-0.14.1/NatanStanek.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 09:43:02.000000 natanstanek-0.14.1/NatanStanek.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-08 12:52:30.000000 natanstanek-0.14.1/NatanStanek.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2024-05-10 09:43:02.000000 natanstanek-0.14.1/NatanStanek.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      250 2024-05-10 09:43:03.060366 natanstanek-0.14.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-10 09:43:03.064371 natanstanek-0.14.1/setup.cfg
+-rw-rw-rw-   0        0        0      388 2024-05-10 09:42:56.000000 natanstanek-0.14.1/setup.py
```

