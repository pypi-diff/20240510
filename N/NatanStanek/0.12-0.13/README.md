# Comparing `tmp/natanstanek-0.12.tar.gz` & `tmp/natanstanek-0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "natanstanek-0.12.tar", last modified: Wed May  8 13:13:05 2024, max compression
+gzip compressed data, was "natanstanek-0.13.tar", last modified: Fri May 10 09:29:17 2024, max compression
```

## Comparing `natanstanek-0.12.tar` & `natanstanek-0.13.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 13:13:05.396906 natanstanek-0.12/
-drwxrwxrwx   0        0        0        0 2024-05-08 13:13:05.358343 natanstanek-0.12/NatanStanek/
--rw-rw-rw-   0        0        0      131 2024-05-08 13:10:58.000000 natanstanek-0.12/NatanStanek/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 13:13:05.387882 natanstanek-0.12/NatanStanek.egg-info/
--rw-rw-rw-   0        0        0      258 2024-05-08 13:13:05.000000 natanstanek-0.12/NatanStanek.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2024-05-08 13:13:05.000000 natanstanek-0.12/NatanStanek.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 13:13:05.000000 natanstanek-0.12/NatanStanek.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-08 12:52:30.000000 natanstanek-0.12/NatanStanek.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2024-05-08 13:13:05.000000 natanstanek-0.12/NatanStanek.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      258 2024-05-08 13:13:05.391906 natanstanek-0.12/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-08 13:13:05.396906 natanstanek-0.12/setup.cfg
--rw-rw-rw-   0        0        0      396 2024-05-08 13:11:53.000000 natanstanek-0.12/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:29:17.706124 natanstanek-0.13/
+drwxrwxrwx   0        0        0        0 2024-05-10 09:29:17.663705 natanstanek-0.13/NatanStanek/
+-rw-rw-rw-   0        0        0      195 2024-05-10 09:28:53.000000 natanstanek-0.13/NatanStanek/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:29:17.700781 natanstanek-0.13/NatanStanek.egg-info/
+-rw-rw-rw-   0        0        0      258 2024-05-10 09:29:17.000000 natanstanek-0.13/NatanStanek.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      206 2024-05-10 09:29:17.000000 natanstanek-0.13/NatanStanek.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 09:29:17.000000 natanstanek-0.13/NatanStanek.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-08 12:52:30.000000 natanstanek-0.13/NatanStanek.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2024-05-10 09:29:17.000000 natanstanek-0.13/NatanStanek.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      258 2024-05-10 09:29:17.702715 natanstanek-0.13/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-10 09:29:17.706709 natanstanek-0.13/setup.cfg
+-rw-rw-rw-   0        0        0      396 2024-05-10 09:29:14.000000 natanstanek-0.13/setup.py
```

