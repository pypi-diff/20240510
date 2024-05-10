# Comparing `tmp/ilo-0.0.23.tar.gz` & `tmp/ilo-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ilo-0.0.23.tar", last modified: Fri May 10 15:40:54 2024, max compression
+gzip compressed data, was "ilo-0.0.9.tar", last modified: Thu Dec 16 12:00:24 2021, max compression
```

## Comparing `ilo-0.0.23.tar` & `ilo-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 15:40:54.307328 ilo-0.0.23/
--rw-rw-rw-   0        0        0     2156 2024-05-10 15:40:54.306286 ilo-0.0.23/PKG-INFO
--rw-rw-rw-   0        0        0     1589 2024-05-02 14:19:59.000000 ilo-0.0.23/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 15:40:54.276057 ilo-0.0.23/libname/
-drwxrwxrwx   0        0        0        0 2024-05-10 15:40:54.304692 ilo-0.0.23/libname/ilo.egg-info/
--rw-rw-rw-   0        0        0     2156 2024-05-10 15:40:54.000000 ilo-0.0.23/libname/ilo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2024-05-10 15:40:54.000000 ilo-0.0.23/libname/ilo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 15:40:54.000000 ilo-0.0.23/libname/ilo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-10 15:40:54.000000 ilo-0.0.23/libname/ilo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-10 15:40:54.000000 ilo-0.0.23/libname/ilo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    21836 2024-05-10 15:38:16.000000 ilo-0.0.23/libname/ilo.py
--rw-rw-rw-   0        0        0       42 2024-05-10 15:40:54.307328 ilo-0.0.23/setup.cfg
--rw-rw-rw-   0        0        0      936 2024-05-10 09:24:15.000000 ilo-0.0.23/setup.py
+drwxrwxrwx   0        0        0        0 2021-12-16 12:00:24.592552 ilo-0.0.9/
+-rw-rw-rw-   0        0        0      665 2021-12-16 12:00:24.592552 ilo-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       59 2021-12-15 07:37:41.000000 ilo-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2021-12-16 12:00:24.592552 ilo-0.0.9/libname/
+drwxrwxrwx   0        0        0        0 2021-12-16 12:00:24.592552 ilo-0.0.9/libname/ilo.egg-info/
+-rw-rw-rw-   0        0        0      665 2021-12-16 12:00:24.000000 ilo-0.0.9/libname/ilo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2021-12-16 12:00:24.000000 ilo-0.0.9/libname/ilo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-12-16 12:00:24.000000 ilo-0.0.9/libname/ilo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2021-12-16 12:00:24.000000 ilo-0.0.9/libname/ilo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    14837 2021-12-16 11:58:01.000000 ilo-0.0.9/libname/ilo.py
+-rw-rw-rw-   0        0        0       42 2021-12-16 12:00:24.592552 ilo-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      902 2021-12-16 12:00:18.000000 ilo-0.0.9/setup.py
```

