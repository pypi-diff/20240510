# Comparing `tmp/siglyser-0.21.tar.gz` & `tmp/siglyser-0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siglyser-0.21.tar", last modified: Sun May  5 09:01:09 2024, max compression
+gzip compressed data, was "siglyser-0.22.tar", last modified: Fri May 10 07:45:17 2024, max compression
```

## Comparing `siglyser-0.21.tar` & `siglyser-0.22.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 09:01:09.821325 siglyser-0.21/
--rw-rw-rw-   0        0        0      242 2024-05-05 09:01:09.821325 siglyser-0.21/PKG-INFO
--rw-rw-rw-   0        0        0      143 2024-04-17 15:48:54.000000 siglyser-0.21/README.md
--rw-rw-rw-   0        0        0       42 2024-05-05 09:01:09.821325 siglyser-0.21/setup.cfg
--rw-rw-rw-   0        0        0      358 2024-05-05 09:00:52.000000 siglyser-0.21/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-05 09:01:09.787222 siglyser-0.21/siglyser/
--rw-rw-rw-   0        0        0       80 2024-05-05 08:58:44.000000 siglyser-0.21/siglyser/__init__.py
--rw-rw-rw-   0        0        0     4814 2024-05-05 08:55:17.000000 siglyser-0.21/siglyser/main.py
-drwxrwxrwx   0        0        0        0 2024-05-05 09:01:09.818906 siglyser-0.21/siglyser.egg-info/
--rw-rw-rw-   0        0        0      242 2024-05-05 09:01:09.000000 siglyser-0.21/siglyser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      184 2024-05-05 09:01:09.000000 siglyser-0.21/siglyser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 09:01:09.000000 siglyser-0.21/siglyser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-05 09:01:09.000000 siglyser-0.21/siglyser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 07:45:17.106674 siglyser-0.22/
+-rw-rw-rw-   0        0        0     1016 2024-05-10 07:45:17.106674 siglyser-0.22/PKG-INFO
+-rw-rw-rw-   0        0        0      821 2024-05-10 07:41:23.000000 siglyser-0.22/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-10 07:45:17.106674 siglyser-0.22/setup.cfg
+-rw-rw-rw-   0        0        0      473 2024-05-10 07:45:11.000000 siglyser-0.22/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 07:45:17.091044 siglyser-0.22/siglyser/
+-rw-rw-rw-   0        0        0       80 2024-05-05 08:58:44.000000 siglyser-0.22/siglyser/__init__.py
+-rw-rw-rw-   0        0        0     4814 2024-05-05 08:55:17.000000 siglyser-0.22/siglyser/main.py
+drwxrwxrwx   0        0        0        0 2024-05-10 07:45:17.106674 siglyser-0.22/siglyser.egg-info/
+-rw-rw-rw-   0        0        0     1016 2024-05-10 07:45:16.000000 siglyser-0.22/siglyser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      184 2024-05-10 07:45:16.000000 siglyser-0.22/siglyser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 07:45:16.000000 siglyser-0.22/siglyser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-10 07:45:16.000000 siglyser-0.22/siglyser.egg-info/top_level.txt
```

### Comparing `siglyser-0.21/siglyser/main.py` & `siglyser-0.22/siglyser/main.py`

 * *Files identical despite different names*

