# Comparing `tmp/radical.gtod-1.6.7.tar.gz` & `tmp/radical_gtod-1.60.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/radical.gtod-1.6.7.tar", last modified: Fri Jul  9 08:02:35 2021, max compression
+gzip compressed data, was "radical_gtod-1.60.0.tar", last modified: Fri May 10 13:13:57 2024, max compression
```

## Comparing `radical.gtod-1.6.7.tar` & `radical_gtod-1.60.0.tar`

### file list

```diff
@@ -1,27 +1,31 @@
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-09 08:02:35.629757 radical.gtod-1.6.7/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     1104 2021-07-09 07:58:07.000000 radical.gtod-1.6.7/CHANGES.md
--rw-r--r--   0 merzky    (1001) merzky    (1001)     8365 2020-07-21 20:11:05.000000 radical.gtod-1.6.7/LICENSE.md
--rw-r--r--   0 merzky    (1001) merzky    (1001)       79 2020-07-21 20:11:05.000000 radical.gtod-1.6.7/MANIFEST.in
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     1029 2021-07-09 08:02:35.629757 radical.gtod-1.6.7/PKG-INFO
--rw-r--r--   0 merzky    (1001) merzky    (1001)      640 2020-07-21 20:17:36.000000 radical.gtod-1.6.7/README.md
--rw-rw-r--   0 merzky    (1001) merzky    (1001)        6 2021-07-09 07:57:01.000000 radical.gtod-1.6.7/VERSION
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-09 08:02:35.629757 radical.gtod-1.6.7/bin/
--rwxr-xr-x   0 merzky    (1001) merzky    (1001)      140 2020-07-21 20:29:35.000000 radical.gtod-1.6.7/bin/radical-gtod-version
--rw-r--r--   0 merzky    (1001) merzky    (1001)       67 2021-07-09 08:02:35.629757 radical.gtod-1.6.7/setup.cfg
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    11093 2021-07-09 08:02:01.000000 radical.gtod-1.6.7/setup.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-09 08:02:35.629757 radical.gtod-1.6.7/src/
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-09 08:02:35.629757 radical.gtod-1.6.7/src/radical/
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-09 08:02:35.629757 radical.gtod-1.6.7/src/radical/gtod/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)       40 2021-07-09 08:02:35.000000 radical.gtod-1.6.7/src/radical/gtod/SDIST
--rw-rw-r--   0 merzky    (1001) merzky    (1001)       20 2021-07-09 08:02:35.000000 radical.gtod-1.6.7/src/radical/gtod/VERSION
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      532 2020-10-07 18:41:21.000000 radical.gtod-1.6.7/src/radical/gtod/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      196 2020-08-04 23:56:19.000000 radical.gtod-1.6.7/src/radical/gtod/gtod.c
--rw-r--r--   0 merzky    (1001) merzky    (1001)      422 2020-07-21 20:11:05.000000 radical.gtod-1.6.7/src/radical/gtod/gtod_module.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     8448 2021-07-09 08:02:35.000000 radical.gtod-1.6.7/src/radical/gtod/radical-gtod
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-09 08:02:35.629757 radical.gtod-1.6.7/src/radical.gtod.egg-info/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     1029 2021-07-09 08:02:35.000000 radical.gtod-1.6.7/src/radical.gtod.egg-info/PKG-INFO
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      506 2021-07-09 08:02:35.000000 radical.gtod-1.6.7/src/radical.gtod.egg-info/SOURCES.txt
--rw-rw-r--   0 merzky    (1001) merzky    (1001)        1 2021-07-09 08:02:35.000000 radical.gtod-1.6.7/src/radical.gtod.egg-info/dependency_links.txt
--rw-rw-r--   0 merzky    (1001) merzky    (1001)        8 2021-07-09 08:02:35.000000 radical.gtod-1.6.7/src/radical.gtod.egg-info/namespace_packages.txt
--rw-rw-r--   0 merzky    (1001) merzky    (1001)        1 2021-07-09 08:02:35.000000 radical.gtod-1.6.7/src/radical.gtod.egg-info/not-zip-safe
--rw-rw-r--   0 merzky    (1001) merzky    (1001)        8 2021-07-09 08:02:35.000000 radical.gtod-1.6.7/src/radical.gtod.egg-info/top_level.txt
+drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:13:57.706955 radical_gtod-1.60.0/
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     3241 2024-05-10 13:13:25.000000 radical_gtod-1.60.0/CHANGES.md
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     8361 2022-12-16 11:50:15.000000 radical_gtod-1.60.0/LICENSE.md
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)      213 2022-12-16 13:11:13.000000 radical_gtod-1.60.0/MANIFEST.in
+-rw-r--r--   0 merzky    (1000) merzky    (1000)     1990 2024-05-10 13:13:57.706955 radical_gtod-1.60.0/PKG-INFO
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)      640 2021-09-24 08:24:02.000000 radical_gtod-1.60.0/README.md
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)        7 2024-05-10 13:13:25.000000 radical_gtod-1.60.0/VERSION
+drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:13:57.706955 radical_gtod-1.60.0/bin/
+-rwxrwxr-x   0 merzky    (1000) merzky    (1000)      140 2021-09-24 08:24:02.000000 radical_gtod-1.60.0/bin/radical-gtod-version
+drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:13:57.706955 radical_gtod-1.60.0/examples/
+-rwxrwxr-x   0 merzky    (1000) merzky    (1000)      268 2021-09-24 08:24:02.000000 radical_gtod-1.60.0/examples/00_gtod.py
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)       88 2024-05-10 13:12:49.000000 radical_gtod-1.60.0/pyproject.toml
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)       58 2022-12-16 11:50:15.000000 radical_gtod-1.60.0/requirements-docs.txt
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)       71 2022-12-16 11:50:15.000000 radical_gtod-1.60.0/requirements-tests.txt
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)       22 2024-05-10 13:13:36.000000 radical_gtod-1.60.0/requirements.txt
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)       72 2024-05-10 13:13:57.706955 radical_gtod-1.60.0/setup.cfg
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     8805 2024-05-10 13:12:49.000000 radical_gtod-1.60.0/setup.py
+drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:13:57.706955 radical_gtod-1.60.0/src/
+drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:13:57.706955 radical_gtod-1.60.0/src/radical/
+drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:13:57.706955 radical_gtod-1.60.0/src/radical/gtod/
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)       51 2024-05-10 13:13:57.000000 radical_gtod-1.60.0/src/radical/gtod/VERSION
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)      923 2024-05-10 13:12:49.000000 radical_gtod-1.60.0/src/radical/gtod/__init__.py
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)      196 2021-09-24 08:24:02.000000 radical_gtod-1.60.0/src/radical/gtod/gtod.c
+-rwxrwxr-x   0 merzky    (1000) merzky    (1000)    16096 2024-05-10 13:13:57.000000 radical_gtod-1.60.0/src/radical/gtod/radical-gtod
+drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:13:57.706955 radical_gtod-1.60.0/src/radical.gtod.egg-info/
+-rw-r--r--   0 merzky    (1000) merzky    (1000)     1990 2024-05-10 13:13:57.000000 radical_gtod-1.60.0/src/radical.gtod.egg-info/PKG-INFO
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)      538 2024-05-10 13:13:57.000000 radical_gtod-1.60.0/src/radical.gtod.egg-info/SOURCES.txt
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)        1 2024-05-10 13:13:57.000000 radical_gtod-1.60.0/src/radical.gtod.egg-info/dependency_links.txt
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)        1 2024-05-10 13:13:57.000000 radical_gtod-1.60.0/src/radical.gtod.egg-info/not-zip-safe
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)       20 2024-05-10 13:13:57.000000 radical_gtod-1.60.0/src/radical.gtod.egg-info/requires.txt
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)        8 2024-05-10 13:13:57.000000 radical_gtod-1.60.0/src/radical.gtod.egg-info/top_level.txt
```

### Comparing `radical.gtod-1.6.7/LICENSE.md` & `radical_gtod-1.60.0/LICENSE.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 
 ================================================================================
       The GNU Lesser General Public License, version 3.0 (LGPL-3.0)
                             [OSI Approved License]
 ================================================================================
 
-This license is a set of additional permissions added to version 3 of the GNU 
+This license is a set of additional permissions added to version 3 of the GNU
 General Public License.
 
 
 GNU LESSER GENERAL PUBLIC LICENSE
 =================================
 
 Version 3, 29 June 2007
@@ -65,18 +65,18 @@
 -------------------------------
 
 If you modify a copy of the Library, and, in your modifications, a facility
 refers to a function or data to be supplied by an Application that uses the
 facility (other than as an argument passed when the facility is invoked), then
 you may convey a copy of the modified version:
 
-  a) under this License, provided that you make a good faith effort to ensure 
+  a) under this License, provided that you make a good faith effort to ensure
      that, in the event an Application does not supply the function or data, the
      facility still operates, and performs whatever part of its purpose remains
-     meaningful, or 
+     meaningful, or
 
   b) under the GNU GPL, with none of the additional permissions of this License
      applicable to that copy.
 
 
 3. Object Code Incorporating Material from Library Header Files.
 ----------------------------------------------------------------
@@ -146,15 +146,15 @@
 Applications and are not covered by this License, and convey such a combined
 library under terms of your choice, if you do both of the following:
 
   a) Accompany the combined library with a copy of the same work based on the
      Library, uncombined with any other library facilities, conveyed under the
      terms of this License.  
      
-  b) Give prominent notice with the combined library that part of it is a work 
+  b) Give prominent notice with the combined library that part of it is a work
      based on the Library, and explaining where to find the accompanying
      uncombined form of the same work.
 
 
 6. Revised Versions of the GNU Lesser General Public License.
 -------------------------------------------------------------
```

### Comparing `radical.gtod-1.6.7/README.md` & `radical_gtod-1.60.0/README.md`

 * *Files identical despite different names*

