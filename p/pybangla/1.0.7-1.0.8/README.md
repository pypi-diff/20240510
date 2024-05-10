# Comparing `tmp/pybangla-1.0.7.tar.gz` & `tmp/pybangla-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybangla-1.0.7.tar", last modified: Wed May  8 20:31:56 2024, max compression
+gzip compressed data, was "pybangla-1.0.8.tar", last modified: Thu May  9 12:35:48 2024, max compression
```

## Comparing `pybangla-1.0.7.tar` & `pybangla-1.0.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:31:56.322170 pybangla-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:31:52.000000 pybangla-1.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    15656 2024-05-08 20:31:56.322170 pybangla-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15098 2024-05-08 20:31:52.000000 pybangla-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:31:56.322170 pybangla-1.0.7/pybangla/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-08 20:31:52.000000 pybangla-1.0.7/pybangla/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:31:56.322170 pybangla-1.0.7/pybangla/module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:31:52.000000 pybangla-1.0.7/pybangla/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18102 2024-05-08 20:31:52.000000 pybangla-1.0.7/pybangla/module/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8359 2024-05-08 20:31:52.000000 pybangla-1.0.7/pybangla/module/date_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-05-08 20:31:52.000000 pybangla-1.0.7/pybangla/module/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    17040 2024-05-08 20:31:52.000000 pybangla-1.0.7/pybangla/module/number_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    20038 2024-05-08 20:31:52.000000 pybangla-1.0.7/pybangla/module/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    22922 2024-05-08 20:31:52.000000 pybangla-1.0.7/pybangla/module/word_to_number.py
--rw-r--r--   0 runner    (1001) docker     (127)    10137 2024-05-08 20:31:52.000000 pybangla-1.0.7/pybangla/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:31:56.322170 pybangla-1.0.7/pybangla.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15656 2024-05-08 20:31:56.000000 pybangla-1.0.7/pybangla.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-08 20:31:56.000000 pybangla-1.0.7/pybangla.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 20:31:56.000000 pybangla-1.0.7/pybangla.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-08 20:31:56.000000 pybangla-1.0.7/pybangla.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 20:31:56.000000 pybangla-1.0.7/pybangla.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 20:31:56.322170 pybangla-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-08 20:31:52.000000 pybangla-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:31:56.322170 pybangla-1.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-08 20:31:52.000000 pybangla-1.0.7/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:35:48.213289 pybangla-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 12:35:43.000000 pybangla-1.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15656 2024-05-09 12:35:48.213289 pybangla-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15098 2024-05-09 12:35:43.000000 pybangla-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:35:48.213289 pybangla-1.0.8/pybangla/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-09 12:35:43.000000 pybangla-1.0.8/pybangla/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:35:48.213289 pybangla-1.0.8/pybangla/module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 12:35:43.000000 pybangla-1.0.8/pybangla/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17190 2024-05-09 12:35:43.000000 pybangla-1.0.8/pybangla/module/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8359 2024-05-09 12:35:43.000000 pybangla-1.0.8/pybangla/module/date_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-05-09 12:35:43.000000 pybangla-1.0.8/pybangla/module/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17040 2024-05-09 12:35:43.000000 pybangla-1.0.8/pybangla/module/number_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20038 2024-05-09 12:35:43.000000 pybangla-1.0.8/pybangla/module/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22922 2024-05-09 12:35:43.000000 pybangla-1.0.8/pybangla/module/word_to_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10137 2024-05-09 12:35:43.000000 pybangla-1.0.8/pybangla/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:35:48.213289 pybangla-1.0.8/pybangla.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15656 2024-05-09 12:35:48.000000 pybangla-1.0.8/pybangla.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-09 12:35:48.000000 pybangla-1.0.8/pybangla.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 12:35:48.000000 pybangla-1.0.8/pybangla.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-09 12:35:48.000000 pybangla-1.0.8/pybangla.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-09 12:35:48.000000 pybangla-1.0.8/pybangla.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 12:35:48.213289 pybangla-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-09 12:35:43.000000 pybangla-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:35:48.213289 pybangla-1.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-09 12:35:43.000000 pybangla-1.0.8/tests/test.py
```

### Comparing `pybangla-1.0.7/PKG-INFO` & `pybangla-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybangla
-Version: 1.0.7
+Version: 1.0.8
 Summary: pybangla is the bangla text normalizer tool, it use for text normalization like word to number and date formating purposes
 Home-page: https://github.com/saiful9379/pybangla
 Author: saiful
 Author-email: saifulbrur79@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pybangla-1.0.7/README.md` & `pybangla-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pybangla-1.0.7/pybangla/module/config.py` & `pybangla-1.0.8/pybangla/module/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -126,29 +126,17 @@
                 ("হাফিঃ", "হাফিযাহুল্লাহ"),
                 ("দাঃবাঃ", "দামাত বারাকাতুহুম,দামাত বারাকাতুল্লাহ"),
                 ("মোঃ",  "মোহাম্মদ"),
                 ("মোসাঃ",  "মোসাম্মত"),
                 ("মোছাঃ", "মোছাম্মত"),
                 ("আ:" , "আব্দুর"),
                 ("ডাঃ" , "ডাক্তার"),
-                (" কিমি ", "কিলোমিটার"),
-                (" সেমি ", "সেন্টিমিটার"),
-                (" বিডি ", "বাংলাদেশ"),
-                ("আ/এ", "আবাসিক এলাকা"),  
-                (" একনেক ", "জাতীয় অর্থনৈতিক পরিষদের নির্বাহী কমিটি"),
-                (" সওজ ", "সড়ক ও জনপথ অধিদপ্তর"),
-                (" পাউবো ",  "পানি উন্নয়ন বোর্ড"),	
-
-                (" টেশিস ", "টেলিফোন শিল্প সংস্থা"),
-                (" পবিস ",  "পল্লী বিদ্যুৎ সমিতি"), 
-                (" ইউপি ", "ইউনিয়ন পরিষদ"),
-                (" ঢাবি ", "ঢাকা বিশ্ববিদ্যালয়"),
-                (" বাগ ", "বাগান"),
-                (" স. ", "সড়ক"), 
-                (" সে. ", "সেতু")
+                (" কিমি ", " কিলোমিটার "),
+                (" সেমি ", " সেন্টিমিটার "),
+                (" বিডি ", " বাংলাদেশ ")
             ]
         ]
     }
 
     _symbols = {
             "en": [
                 (re.compile(r"%s" % re.escape(x[0]), re.IGNORECASE), x[1])
```

### Comparing `pybangla-1.0.7/pybangla/module/date_extractor.py` & `pybangla-1.0.8/pybangla/module/date_extractor.py`

 * *Files identical despite different names*

### Comparing `pybangla-1.0.7/pybangla/module/main.py` & `pybangla-1.0.8/pybangla/module/main.py`

 * *Files identical despite different names*

### Comparing `pybangla-1.0.7/pybangla/module/number_parser.py` & `pybangla-1.0.8/pybangla/module/number_parser.py`

 * *Files identical despite different names*

### Comparing `pybangla-1.0.7/pybangla/module/parser.py` & `pybangla-1.0.8/pybangla/module/parser.py`

 * *Files identical despite different names*

### Comparing `pybangla-1.0.7/pybangla/module/word_to_number.py` & `pybangla-1.0.8/pybangla/module/word_to_number.py`

 * *Files identical despite different names*

### Comparing `pybangla-1.0.7/pybangla/test.py` & `pybangla-1.0.8/pybangla/test.py`

 * *Files identical despite different names*

### Comparing `pybangla-1.0.7/pybangla.egg-info/PKG-INFO` & `pybangla-1.0.8/pybangla.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybangla
-Version: 1.0.7
+Version: 1.0.8
 Summary: pybangla is the bangla text normalizer tool, it use for text normalization like word to number and date formating purposes
 Home-page: https://github.com/saiful9379/pybangla
 Author: saiful
 Author-email: saifulbrur79@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pybangla-1.0.7/setup.py` & `pybangla-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import codecs
 from setuptools import setup, find_packages
 
 setup(
     name='pybangla',
-    version='1.0.7',
+    version='1.0.8',
     packages=find_packages(),
     # entry_points={
     #     'console_scripts': [
     #         'pybangla = pybangla.main:Normalizer'
     #     ]
     # },
     author='saiful',
```

### Comparing `pybangla-1.0.7/tests/test.py` & `pybangla-1.0.8/tests/test.py`

 * *Files identical despite different names*

