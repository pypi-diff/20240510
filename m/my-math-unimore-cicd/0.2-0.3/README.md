# Comparing `tmp/my_math_unimore_cicd-0.2.tar.gz` & `tmp/my_math_unimore_cicd-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_math_unimore_cicd-0.2.tar", last modified: Fri May 10 08:45:30 2024, max compression
+gzip compressed data, was "my_math_unimore_cicd-0.3.tar", last modified: Fri May 10 08:46:13 2024, max compression
```

## Comparing `my_math_unimore_cicd-0.2.tar` & `my_math_unimore_cicd-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:45:30.084434 my_math_unimore_cicd-0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-10 08:45:30.080434 my_math_unimore_cicd-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-10 08:45:21.000000 my_math_unimore_cicd-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:45:30.080434 my_math_unimore_cicd-0.2/my_math_unimore_cicd/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-10 08:45:21.000000 my_math_unimore_cicd-0.2/my_math_unimore_cicd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-10 08:45:21.000000 my_math_unimore_cicd-0.2/my_math_unimore_cicd/unimore_math.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:45:30.080434 my_math_unimore_cicd-0.2/my_math_unimore_cicd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-10 08:45:30.000000 my_math_unimore_cicd-0.2/my_math_unimore_cicd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-10 08:45:30.000000 my_math_unimore_cicd-0.2/my_math_unimore_cicd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 08:45:30.000000 my_math_unimore_cicd-0.2/my_math_unimore_cicd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 08:45:30.000000 my_math_unimore_cicd-0.2/my_math_unimore_cicd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-10 08:45:30.000000 my_math_unimore_cicd-0.2/my_math_unimore_cicd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 08:45:30.084434 my_math_unimore_cicd-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-10 08:45:21.000000 my_math_unimore_cicd-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:46:13.127537 my_math_unimore_cicd-0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-10 08:46:13.127537 my_math_unimore_cicd-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-10 08:46:06.000000 my_math_unimore_cicd-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:46:13.123537 my_math_unimore_cicd-0.3/my_math_unimore_cicd/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-10 08:46:06.000000 my_math_unimore_cicd-0.3/my_math_unimore_cicd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-10 08:46:06.000000 my_math_unimore_cicd-0.3/my_math_unimore_cicd/unimore_math.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:46:13.127537 my_math_unimore_cicd-0.3/my_math_unimore_cicd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-10 08:46:13.000000 my_math_unimore_cicd-0.3/my_math_unimore_cicd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-10 08:46:13.000000 my_math_unimore_cicd-0.3/my_math_unimore_cicd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 08:46:13.000000 my_math_unimore_cicd-0.3/my_math_unimore_cicd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 08:46:13.000000 my_math_unimore_cicd-0.3/my_math_unimore_cicd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-10 08:46:13.000000 my_math_unimore_cicd-0.3/my_math_unimore_cicd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 08:46:13.127537 my_math_unimore_cicd-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-10 08:46:06.000000 my_math_unimore_cicd-0.3/setup.py
```

