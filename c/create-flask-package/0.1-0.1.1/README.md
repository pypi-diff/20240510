# Comparing `tmp/create_flask_package-0.1.tar.gz` & `tmp/create_flask_package-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "create_flask_package-0.1.tar", last modified: Fri May 10 06:27:10 2024, max compression
+gzip compressed data, was "create_flask_package-0.1.1.tar", last modified: Fri May 10 08:00:37 2024, max compression
```

## Comparing `create_flask_package-0.1.tar` & `create_flask_package-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 06:27:10.524105 create_flask_package-0.1/
--rw-rw-rw-   0        0        0      120 2024-05-10 06:27:10.523114 create_flask_package-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-10 06:27:10.500137 create_flask_package-0.1/create_flask_package/
--rw-rw-rw-   0        0        0        0 2024-05-10 05:38:02.000000 create_flask_package-0.1/create_flask_package/__init__.py
--rw-rw-rw-   0        0        0     1518 2024-05-10 06:26:54.000000 create_flask_package-0.1/create_flask_package/create_flask_package.py
-drwxrwxrwx   0        0        0        0 2024-05-10 06:27:10.522109 create_flask_package-0.1/create_flask_package.egg-info/
--rw-rw-rw-   0        0        0      120 2024-05-10 06:27:10.000000 create_flask_package-0.1/create_flask_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-05-10 06:27:10.000000 create_flask_package-0.1/create_flask_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 06:27:10.000000 create_flask_package-0.1/create_flask_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-05-10 06:27:10.000000 create_flask_package-0.1/create_flask_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-05-10 06:27:10.000000 create_flask_package-0.1/create_flask_package.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 06:27:10.524105 create_flask_package-0.1/setup.cfg
--rw-rw-rw-   0        0        0      222 2024-05-10 06:25:49.000000 create_flask_package-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:00:37.768267 create_flask_package-0.1.1/
+-rw-rw-rw-   0        0        0      228 2024-05-10 08:00:37.767265 create_flask_package-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-10 08:00:37.735265 create_flask_package-0.1.1/create_flask_package/
+-rw-rw-rw-   0        0        0        0 2024-05-10 05:38:02.000000 create_flask_package-0.1.1/create_flask_package/__init__.py
+-rw-rw-rw-   0        0        0     3794 2024-05-10 07:51:58.000000 create_flask_package-0.1.1/create_flask_package/create_flask_package.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:00:37.766265 create_flask_package-0.1.1/create_flask_package.egg-info/
+-rw-rw-rw-   0        0        0      228 2024-05-10 08:00:37.000000 create_flask_package-0.1.1/create_flask_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2024-05-10 08:00:37.000000 create_flask_package-0.1.1/create_flask_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 08:00:37.000000 create_flask_package-0.1.1/create_flask_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      107 2024-05-10 08:00:37.000000 create_flask_package-0.1.1/create_flask_package.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       60 2024-05-10 08:00:37.000000 create_flask_package-0.1.1/create_flask_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-05-10 08:00:37.000000 create_flask_package-0.1.1/create_flask_package.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 08:00:37.768267 create_flask_package-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      496 2024-05-10 08:00:05.000000 create_flask_package-0.1.1/setup.py
```

