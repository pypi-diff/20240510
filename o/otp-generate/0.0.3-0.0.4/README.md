# Comparing `tmp/otp_generate-0.0.3.tar.gz` & `tmp/otp_generate-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otp_generate-0.0.3.tar", last modified: Thu May  9 05:36:06 2024, max compression
+gzip compressed data, was "otp_generate-0.0.4.tar", last modified: Fri May 10 10:53:52 2024, max compression
```

## Comparing `otp_generate-0.0.3.tar` & `otp_generate-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 marimuthu  (1000) marimuthu  (1000)        0 2024-05-09 05:36:06.291741 otp_generate-0.0.3/
--rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)     1083 2024-05-08 11:06:07.000000 otp_generate-0.0.3/LICENSE
--rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)      370 2024-05-09 05:36:06.291741 otp_generate-0.0.3/PKG-INFO
--rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)       39 2024-05-08 11:06:07.000000 otp_generate-0.0.3/README.md
-drwxr-xr-x   0 marimuthu  (1000) marimuthu  (1000)        0 2024-05-09 05:36:06.290742 otp_generate-0.0.3/otp_generate/
--rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)       39 2024-05-08 13:44:02.000000 otp_generate-0.0.3/otp_generate/__init__.py
--rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)      619 2024-05-08 13:44:02.000000 otp_generate-0.0.3/otp_generate/main.py
-drwxr-xr-x   0 marimuthu  (1000) marimuthu  (1000)        0 2024-05-09 05:36:06.291741 otp_generate-0.0.3/otp_generate.egg-info/
--rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)      370 2024-05-09 05:36:06.000000 otp_generate-0.0.3/otp_generate.egg-info/PKG-INFO
--rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)      290 2024-05-09 05:36:06.000000 otp_generate-0.0.3/otp_generate.egg-info/SOURCES.txt
--rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)        1 2024-05-09 05:36:06.000000 otp_generate-0.0.3/otp_generate.egg-info/dependency_links.txt
--rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)       61 2024-05-09 05:36:06.000000 otp_generate-0.0.3/otp_generate.egg-info/entry_points.txt
--rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)       13 2024-05-09 05:36:06.000000 otp_generate-0.0.3/otp_generate.egg-info/requires.txt
--rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)       13 2024-05-09 05:36:06.000000 otp_generate-0.0.3/otp_generate.egg-info/top_level.txt
--rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)       38 2024-05-09 05:36:06.291741 otp_generate-0.0.3/setup.cfg
--rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)      852 2024-05-09 05:35:57.000000 otp_generate-0.0.3/setup.py
+drwxr-xr-x   0 marimuthu  (1000) marimuthu  (1000)        0 2024-05-10 10:53:52.100913 otp_generate-0.0.4/
+-rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)     1083 2024-05-08 11:06:07.000000 otp_generate-0.0.4/LICENSE
+-rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)     2653 2024-05-10 10:53:52.100913 otp_generate-0.0.4/PKG-INFO
+-rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)     1979 2024-05-10 10:47:22.000000 otp_generate-0.0.4/README.md
+drwxr-xr-x   0 marimuthu  (1000) marimuthu  (1000)        0 2024-05-10 10:53:52.100913 otp_generate-0.0.4/otp_generate/
+-rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)       46 2024-05-10 07:45:12.000000 otp_generate-0.0.4/otp_generate/__init__.py
+-rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)      840 2024-05-10 10:01:27.000000 otp_generate-0.0.4/otp_generate/main.py
+drwxr-xr-x   0 marimuthu  (1000) marimuthu  (1000)        0 2024-05-10 10:53:52.100913 otp_generate-0.0.4/otp_generate.egg-info/
+-rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)     2653 2024-05-10 10:53:52.000000 otp_generate-0.0.4/otp_generate.egg-info/PKG-INFO
+-rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)      255 2024-05-10 10:53:52.000000 otp_generate-0.0.4/otp_generate.egg-info/SOURCES.txt
+-rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)        1 2024-05-10 10:53:52.000000 otp_generate-0.0.4/otp_generate.egg-info/dependency_links.txt
+-rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)       61 2024-05-10 10:53:52.000000 otp_generate-0.0.4/otp_generate.egg-info/entry_points.txt
+-rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)       13 2024-05-10 10:53:52.000000 otp_generate-0.0.4/otp_generate.egg-info/top_level.txt
+-rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)       38 2024-05-10 10:53:52.100913 otp_generate-0.0.4/setup.cfg
+-rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)     1222 2024-05-10 10:53:25.000000 otp_generate-0.0.4/setup.py
```

### Comparing `otp_generate-0.0.3/LICENSE` & `otp_generate-0.0.4/LICENSE`

 * *Files identical despite different names*

