# Comparing `tmp/convert-us-to-uk-0.1.7.tar.gz` & `tmp/convert-us-to-uk-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "convert-us-to-uk-0.1.7.tar", last modified: Tue May  7 08:18:42 2024, max compression
+gzip compressed data, was "convert-us-to-uk-0.1.8.tar", last modified: Fri May 10 10:24:24 2024, max compression
```

## Comparing `convert-us-to-uk-0.1.7.tar` & `convert-us-to-uk-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 08:18:42.182963 convert-us-to-uk-0.1.7/
--rw-rw-rw-   0        0        0       43 2024-04-17 15:15:06.000000 convert-us-to-uk-0.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0     1990 2024-05-07 08:18:42.178653 convert-us-to-uk-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     1660 2024-04-18 11:43:12.000000 convert-us-to-uk-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 08:18:42.157689 convert-us-to-uk-0.1.7/convert_us_to_uk/
--rw-rw-rw-   0        0        0        0 2024-04-17 12:42:42.000000 convert-us-to-uk-0.1.7/convert_us_to_uk/__init__.py
--rw-rw-rw-   0        0        0     1533 2024-04-30 10:34:39.000000 convert-us-to-uk-0.1.7/convert_us_to_uk/converter.py
--rw-rw-rw-   0        0        0    39744 2024-05-07 08:18:03.000000 convert-us-to-uk-0.1.7/convert_us_to_uk/us_to_uk_trans.csv
-drwxrwxrwx   0        0        0        0 2024-05-07 08:18:42.173776 convert-us-to-uk-0.1.7/convert_us_to_uk.egg-info/
--rw-rw-rw-   0        0        0     1990 2024-05-07 08:18:41.000000 convert-us-to-uk-0.1.7/convert_us_to_uk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2024-05-07 08:18:41.000000 convert-us-to-uk-0.1.7/convert_us_to_uk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 08:18:41.000000 convert-us-to-uk-0.1.7/convert_us_to_uk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2024-05-07 08:18:41.000000 convert-us-to-uk-0.1.7/convert_us_to_uk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-05-07 08:18:41.000000 convert-us-to-uk-0.1.7/convert_us_to_uk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 08:18:42.183439 convert-us-to-uk-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      696 2024-05-07 08:18:21.000000 convert-us-to-uk-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-07 08:18:42.175311 convert-us-to-uk-0.1.7/tests/
--rw-rw-rw-   0        0        0      296 2024-04-17 14:23:12.000000 convert-us-to-uk-0.1.7/tests/test_converter.py
+drwxrwxrwx   0        0        0        0 2024-05-10 10:24:24.339370 convert-us-to-uk-0.1.8/
+-rw-rw-rw-   0        0        0       43 2024-04-17 15:15:06.000000 convert-us-to-uk-0.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     1990 2024-05-10 10:24:24.334496 convert-us-to-uk-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1660 2024-04-18 11:43:12.000000 convert-us-to-uk-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 10:24:24.302793 convert-us-to-uk-0.1.8/convert_us_to_uk/
+-rw-rw-rw-   0        0        0        0 2024-04-17 12:42:42.000000 convert-us-to-uk-0.1.8/convert_us_to_uk/__init__.py
+-rw-rw-rw-   0        0        0     1533 2024-04-30 10:34:39.000000 convert-us-to-uk-0.1.8/convert_us_to_uk/converter.py
+-rw-rw-rw-   0        0        0    39771 2024-05-10 10:22:52.000000 convert-us-to-uk-0.1.8/convert_us_to_uk/us_to_uk_trans.csv
+drwxrwxrwx   0        0        0        0 2024-05-10 10:24:24.321925 convert-us-to-uk-0.1.8/convert_us_to_uk.egg-info/
+-rw-rw-rw-   0        0        0     1990 2024-05-10 10:24:24.000000 convert-us-to-uk-0.1.8/convert_us_to_uk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2024-05-10 10:24:24.000000 convert-us-to-uk-0.1.8/convert_us_to_uk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 10:24:24.000000 convert-us-to-uk-0.1.8/convert_us_to_uk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2024-05-10 10:24:24.000000 convert-us-to-uk-0.1.8/convert_us_to_uk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-05-10 10:24:24.000000 convert-us-to-uk-0.1.8/convert_us_to_uk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 10:24:24.339370 convert-us-to-uk-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      696 2024-05-10 10:23:45.000000 convert-us-to-uk-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 10:24:24.326975 convert-us-to-uk-0.1.8/tests/
+-rw-rw-rw-   0        0        0      296 2024-04-17 14:23:12.000000 convert-us-to-uk-0.1.8/tests/test_converter.py
```

### Comparing `convert-us-to-uk-0.1.7/PKG-INFO` & `convert-us-to-uk-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convert-us-to-uk
-Version: 0.1.7
+Version: 0.1.8
 Summary: A simple utility to convert US spelling to UK spelling.
 Home-page: https://github.com/oliverblane/convert-us-to-uk/tree/main
 Author: Oliver Blane
 Author-email: oliverblane72@gmail.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `convert-us-to-uk-0.1.7/README.md` & `convert-us-to-uk-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `convert-us-to-uk-0.1.7/convert_us_to_uk/converter.py` & `convert-us-to-uk-0.1.8/convert_us_to_uk/converter.py`

 * *Files identical despite different names*

### Comparing `convert-us-to-uk-0.1.7/convert_us_to_uk/us_to_uk_trans.csv` & `convert-us-to-uk-0.1.8/convert_us_to_uk/us_to_uk_trans.csv`

 * *Files 1% similar despite different names*

```diff
@@ -1056,14 +1056,16 @@
 offenses,offences
 omelet,omelette
 omelets,omelettes
 optimize,optimise
 optimized,optimised
 optimizes,optimises
 optimizing,optimising
+optimization, optimisation
+optimizations, optimisations
 organization,organisation
 organizational,organisational
 organizations,organisations
 organize,organise
 organized,organised
 organizer,organiser
 organizers,organisers
@@ -1466,16 +1468,14 @@
 sterilizes,sterilises
 sterilizing,sterilising
 stigmatization,stigmatisation
 stigmatize,stigmatise
 stigmatized,stigmatised
 stigmatizes,stigmatises
 stigmatizing,stigmatising
-story,storey
-stories,storeys
 subsidization,subsidisation
 subsidize,subsidise
 subsidized,subsidised
 subsidizer,subsidiser
 subsidizers,subsidisers
 subsidizes,subsidises
 subsidizing,subsidising
```

### Comparing `convert-us-to-uk-0.1.7/convert_us_to_uk.egg-info/PKG-INFO` & `convert-us-to-uk-0.1.8/convert_us_to_uk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convert-us-to-uk
-Version: 0.1.7
+Version: 0.1.8
 Summary: A simple utility to convert US spelling to UK spelling.
 Home-page: https://github.com/oliverblane/convert-us-to-uk/tree/main
 Author: Oliver Blane
 Author-email: oliverblane72@gmail.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

