# Comparing `tmp/natanstanek-0.13.1.tar.gz` & `tmp/natanstanek-0.14.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "natanstanek-0.13.1.tar", last modified: Fri May 10 09:32:13 2024, max compression
+gzip compressed data, was "natanstanek-0.14.0.tar", last modified: Fri May 10 09:35:58 2024, max compression
```

## Comparing `natanstanek-0.13.1.tar` & `natanstanek-0.14.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 09:32:13.667252 natanstanek-0.13.1/
-drwxrwxrwx   0        0        0        0 2024-05-10 09:32:13.600211 natanstanek-0.13.1/NatanStanek/
--rw-rw-rw-   0        0        0      193 2024-05-10 09:31:53.000000 natanstanek-0.13.1/NatanStanek/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 09:32:13.658304 natanstanek-0.13.1/NatanStanek.egg-info/
--rw-rw-rw-   0        0        0      250 2024-05-10 09:32:13.000000 natanstanek-0.13.1/NatanStanek.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2024-05-10 09:32:13.000000 natanstanek-0.13.1/NatanStanek.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 09:32:13.000000 natanstanek-0.13.1/NatanStanek.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-08 12:52:30.000000 natanstanek-0.13.1/NatanStanek.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2024-05-10 09:32:13.000000 natanstanek-0.13.1/NatanStanek.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      250 2024-05-10 09:32:13.661754 natanstanek-0.13.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-10 09:32:13.667654 natanstanek-0.13.1/setup.cfg
--rw-rw-rw-   0        0        0      388 2024-05-10 09:32:09.000000 natanstanek-0.13.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:35:58.508044 natanstanek-0.14.0/
+drwxrwxrwx   0        0        0        0 2024-05-10 09:35:58.444048 natanstanek-0.14.0/NatanStanek/
+-rw-rw-rw-   0        0        0      233 2024-05-10 09:35:54.000000 natanstanek-0.14.0/NatanStanek/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:35:58.502325 natanstanek-0.14.0/NatanStanek.egg-info/
+-rw-rw-rw-   0        0        0      250 2024-05-10 09:35:58.000000 natanstanek-0.14.0/NatanStanek.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      206 2024-05-10 09:35:58.000000 natanstanek-0.14.0/NatanStanek.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 09:35:58.000000 natanstanek-0.14.0/NatanStanek.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-08 12:52:30.000000 natanstanek-0.14.0/NatanStanek.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2024-05-10 09:35:58.000000 natanstanek-0.14.0/NatanStanek.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      250 2024-05-10 09:35:58.504721 natanstanek-0.14.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-10 09:35:58.508461 natanstanek-0.14.0/setup.cfg
+-rw-rw-rw-   0        0        0      388 2024-05-10 09:35:50.000000 natanstanek-0.14.0/setup.py
```

