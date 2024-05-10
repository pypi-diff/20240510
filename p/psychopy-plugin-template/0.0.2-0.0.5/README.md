# Comparing `tmp/psychopy_plugin_template-0.0.2.tar.gz` & `tmp/psychopy_plugin_template-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychopy_plugin_template-0.0.2.tar", last modified: Thu Apr 25 13:43:47 2024, max compression
+gzip compressed data, was "psychopy_plugin_template-0.0.5.tar", last modified: Fri May 10 09:29:38 2024, max compression
```

## Comparing `psychopy_plugin_template-0.0.2.tar` & `psychopy_plugin_template-0.0.5.tar`

### file list

```diff
@@ -1,38 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:43:47.744127 psychopy_plugin_template-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-25 13:43:47.744127 psychopy_plugin_template-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:43:36.000000 psychopy_plugin_template-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:43:47.740127 psychopy_plugin_template-0.0.2/psychopy_plugin_template/
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-25 13:43:36.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:43:47.744127 psychopy_plugin_template-0.0.2/psychopy_plugin_template/components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:43:36.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:43:47.744127 psychopy_plugin_template-0.0.2/psychopy_plugin_template/components/exampleComponent/
--rw-r--r--   0 runner    (1001) docker     (127)     6537 2024-04-25 13:43:36.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template/components/exampleComponent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:43:47.744127 psychopy_plugin_template-0.0.2/psychopy_plugin_template/components/exampleComponent/classic/
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-25 13:43:36.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template/components/exampleComponent/classic/example.png
--rw-r--r--   0 runner    (1001) docker     (127)     9490 2024-04-25 13:43:36.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template/components/exampleComponent/classic/example@2x.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:43:47.744127 psychopy_plugin_template-0.0.2/psychopy_plugin_template/components/exampleComponent/dark/
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-25 13:43:36.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template/components/exampleComponent/dark/example.png
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-25 13:43:36.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template/components/exampleComponent/dark/example@2x.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:43:47.744127 psychopy_plugin_template-0.0.2/psychopy_plugin_template/components/exampleComponent/light/
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-25 13:43:36.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template/components/exampleComponent/light/example.png
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-25 13:43:36.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template/components/exampleComponent/light/example@2x.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:43:47.744127 psychopy_plugin_template-0.0.2/psychopy_plugin_template/hardware/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-25 13:43:36.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template/hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-25 13:43:36.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template/hardware/exampleDevice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-25 13:43:36.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template/hardware/exampleResponseDevice.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:43:47.744127 psychopy_plugin_template-0.0.2/psychopy_plugin_template/routines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:43:36.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template/routines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:43:47.744127 psychopy_plugin_template-0.0.2/psychopy_plugin_template/routines/exampleStandaloneRoutine/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-25 13:43:36.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template/routines/exampleStandaloneRoutine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:43:47.744127 psychopy_plugin_template-0.0.2/psychopy_plugin_template/visual/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:43:36.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template/visual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-25 13:43:36.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template/visual/exampleVisualStim.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:43:47.744127 psychopy_plugin_template-0.0.2/psychopy_plugin_template.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-25 13:43:47.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-25 13:43:47.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 13:43:47.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-25 13:43:47.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-25 13:43:47.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-25 13:43:47.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-25 13:43:36.000000 psychopy_plugin_template-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 13:43:47.744127 psychopy_plugin_template-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:29:38.352162 psychopy_plugin_template-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-05-10 09:29:38.352162 psychopy_plugin_template-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-05-10 09:29:30.000000 psychopy_plugin_template-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:29:38.344161 psychopy_plugin_template-0.0.5/psychopy_plugin_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-10 09:29:30.000000 psychopy_plugin_template-0.0.5/psychopy_plugin_template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:29:38.348161 psychopy_plugin_template-0.0.5/psychopy_plugin_template/app/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-10 09:29:30.000000 psychopy_plugin_template-0.0.5/psychopy_plugin_template/app/ribbon.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:29:38.348161 psychopy_plugin_template-0.0.5/psychopy_plugin_template/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 09:29:30.000000 psychopy_plugin_template-0.0.5/psychopy_plugin_template/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:29:38.348161 psychopy_plugin_template-0.0.5/psychopy_plugin_template/components/exampleComponent/
+-rw-r--r--   0 runner    (1001) docker     (127)     6537 2024-05-10 09:29:30.000000 psychopy_plugin_template-0.0.5/psychopy_plugin_template/components/exampleComponent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:29:38.348161 psychopy_plugin_template-0.0.5/psychopy_plugin_template/components/exampleComponent/classic/
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-05-10 09:29:30.000000 psychopy_plugin_template-0.0.5/psychopy_plugin_template/components/exampleComponent/classic/example.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9490 2024-05-10 09:29:30.000000 psychopy_plugin_template-0.0.5/psychopy_plugin_template/components/exampleComponent/classic/example@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:29:38.348161 psychopy_plugin_template-0.0.5/psychopy_plugin_template/components/exampleComponent/dark/
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-10 09:29:30.000000 psychopy_plugin_template-0.0.5/psychopy_plugin_template/components/exampleComponent/dark/example.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-10 09:29:30.000000 psychopy_plugin_template-0.0.5/psychopy_plugin_template/components/exampleComponent/dark/example@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:29:38.348161 psychopy_plugin_template-0.0.5/psychopy_plugin_template/components/exampleComponent/light/
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-10 09:29:30.000000 psychopy_plugin_template-0.0.5/psychopy_plugin_template/components/exampleComponent/light/example.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-10 09:29:30.000000 psychopy_plugin_template-0.0.5/psychopy_plugin_template/components/exampleComponent/light/example@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:29:38.348161 psychopy_plugin_template-0.0.5/psychopy_plugin_template/hardware/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-10 09:29:30.000000 psychopy_plugin_template-0.0.5/psychopy_plugin_template/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-10 09:29:30.000000 psychopy_plugin_template-0.0.5/psychopy_plugin_template/hardware/exampleDevice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-10 09:29:30.000000 psychopy_plugin_template-0.0.5/psychopy_plugin_template/hardware/exampleResponseDevice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:29:38.344161 psychopy_plugin_template-0.0.5/psychopy_plugin_template/icons/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:29:38.348161 psychopy_plugin_template-0.0.5/psychopy_plugin_template/icons/example/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 09:29:30.000000 psychopy_plugin_template-0.0.5/psychopy_plugin_template/icons/example/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:29:38.348161 psychopy_plugin_template-0.0.5/psychopy_plugin_template/icons/example/classic/
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-10 09:29:30.000000 psychopy_plugin_template-0.0.5/psychopy_plugin_template/icons/example/classic/example.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-05-10 09:29:30.000000 psychopy_plugin_template-0.0.5/psychopy_plugin_template/icons/example/classic/example@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:29:38.348161 psychopy_plugin_template-0.0.5/psychopy_plugin_template/icons/example/dark/
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-10 09:29:30.000000 psychopy_plugin_template-0.0.5/psychopy_plugin_template/icons/example/dark/example.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-10 09:29:30.000000 psychopy_plugin_template-0.0.5/psychopy_plugin_template/icons/example/dark/example@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:29:38.348161 psychopy_plugin_template-0.0.5/psychopy_plugin_template/icons/example/light/
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-10 09:29:30.000000 psychopy_plugin_template-0.0.5/psychopy_plugin_template/icons/example/light/example.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-10 09:29:30.000000 psychopy_plugin_template-0.0.5/psychopy_plugin_template/icons/example/light/example@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:29:38.352162 psychopy_plugin_template-0.0.5/psychopy_plugin_template/routines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 09:29:30.000000 psychopy_plugin_template-0.0.5/psychopy_plugin_template/routines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:29:38.352162 psychopy_plugin_template-0.0.5/psychopy_plugin_template/routines/exampleStandaloneRoutine/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-10 09:29:30.000000 psychopy_plugin_template-0.0.5/psychopy_plugin_template/routines/exampleStandaloneRoutine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:29:38.352162 psychopy_plugin_template-0.0.5/psychopy_plugin_template/visual/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 09:29:30.000000 psychopy_plugin_template-0.0.5/psychopy_plugin_template/visual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-10 09:29:30.000000 psychopy_plugin_template-0.0.5/psychopy_plugin_template/visual/exampleVisualStim.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:29:38.352162 psychopy_plugin_template-0.0.5/psychopy_plugin_template.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-05-10 09:29:38.000000 psychopy_plugin_template-0.0.5/psychopy_plugin_template.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-10 09:29:38.000000 psychopy_plugin_template-0.0.5/psychopy_plugin_template.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 09:29:38.000000 psychopy_plugin_template-0.0.5/psychopy_plugin_template.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-10 09:29:38.000000 psychopy_plugin_template-0.0.5/psychopy_plugin_template.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-10 09:29:38.000000 psychopy_plugin_template-0.0.5/psychopy_plugin_template.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-10 09:29:38.000000 psychopy_plugin_template-0.0.5/psychopy_plugin_template.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-05-10 09:29:30.000000 psychopy_plugin_template-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 09:29:38.352162 psychopy_plugin_template-0.0.5/setup.cfg
```

### Comparing `psychopy_plugin_template-0.0.2/psychopy_plugin_template/components/exampleComponent/__init__.py` & `psychopy_plugin_template-0.0.5/psychopy_plugin_template/components/exampleComponent/__init__.py`

 * *Files identical despite different names*

### Comparing `psychopy_plugin_template-0.0.2/psychopy_plugin_template/components/exampleComponent/classic/example.png` & `psychopy_plugin_template-0.0.5/psychopy_plugin_template/components/exampleComponent/classic/example.png`

 * *Files identical despite different names*

### Comparing `psychopy_plugin_template-0.0.2/psychopy_plugin_template/components/exampleComponent/classic/example@2x.png` & `psychopy_plugin_template-0.0.5/psychopy_plugin_template/components/exampleComponent/classic/example@2x.png`

 * *Files identical despite different names*

### Comparing `psychopy_plugin_template-0.0.2/psychopy_plugin_template/components/exampleComponent/dark/example.png` & `psychopy_plugin_template-0.0.5/psychopy_plugin_template/components/exampleComponent/dark/example.png`

 * *Files identical despite different names*

### Comparing `psychopy_plugin_template-0.0.2/psychopy_plugin_template/components/exampleComponent/dark/example@2x.png` & `psychopy_plugin_template-0.0.5/psychopy_plugin_template/components/exampleComponent/dark/example@2x.png`

 * *Files identical despite different names*

### Comparing `psychopy_plugin_template-0.0.2/psychopy_plugin_template/components/exampleComponent/light/example.png` & `psychopy_plugin_template-0.0.5/psychopy_plugin_template/components/exampleComponent/light/example.png`

 * *Files identical despite different names*

### Comparing `psychopy_plugin_template-0.0.2/psychopy_plugin_template/components/exampleComponent/light/example@2x.png` & `psychopy_plugin_template-0.0.5/psychopy_plugin_template/components/exampleComponent/light/example@2x.png`

 * *Files identical despite different names*

### Comparing `psychopy_plugin_template-0.0.2/psychopy_plugin_template/hardware/exampleResponseDevice.py` & `psychopy_plugin_template-0.0.5/psychopy_plugin_template/hardware/exampleResponseDevice.py`

 * *Files identical despite different names*

### Comparing `psychopy_plugin_template-0.0.2/psychopy_plugin_template/visual/exampleVisualStim.py` & `psychopy_plugin_template-0.0.5/psychopy_plugin_template/visual/exampleVisualStim.py`

 * *Files identical despite different names*

### Comparing `psychopy_plugin_template-0.0.2/psychopy_plugin_template.egg-info/SOURCES.txt` & `psychopy_plugin_template-0.0.5/psychopy_plugin_template.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -3,22 +3,30 @@
 psychopy_plugin_template/__init__.py
 psychopy_plugin_template.egg-info/PKG-INFO
 psychopy_plugin_template.egg-info/SOURCES.txt
 psychopy_plugin_template.egg-info/dependency_links.txt
 psychopy_plugin_template.egg-info/entry_points.txt
 psychopy_plugin_template.egg-info/requires.txt
 psychopy_plugin_template.egg-info/top_level.txt
+psychopy_plugin_template/app/ribbon.py
 psychopy_plugin_template/components/__init__.py
 psychopy_plugin_template/components/exampleComponent/__init__.py
 psychopy_plugin_template/components/exampleComponent/classic/example.png
 psychopy_plugin_template/components/exampleComponent/classic/example@2x.png
 psychopy_plugin_template/components/exampleComponent/dark/example.png
 psychopy_plugin_template/components/exampleComponent/dark/example@2x.png
 psychopy_plugin_template/components/exampleComponent/light/example.png
 psychopy_plugin_template/components/exampleComponent/light/example@2x.png
 psychopy_plugin_template/hardware/__init__.py
 psychopy_plugin_template/hardware/exampleDevice.py
 psychopy_plugin_template/hardware/exampleResponseDevice.py
+psychopy_plugin_template/icons/example/__init__.py
+psychopy_plugin_template/icons/example/classic/example.png
+psychopy_plugin_template/icons/example/classic/example@2x.png
+psychopy_plugin_template/icons/example/dark/example.png
+psychopy_plugin_template/icons/example/dark/example@2x.png
+psychopy_plugin_template/icons/example/light/example.png
+psychopy_plugin_template/icons/example/light/example@2x.png
 psychopy_plugin_template/routines/__init__.py
 psychopy_plugin_template/routines/exampleStandaloneRoutine/__init__.py
 psychopy_plugin_template/visual/__init__.py
 psychopy_plugin_template/visual/exampleVisualStim.py
```

### Comparing `psychopy_plugin_template-0.0.2/pyproject.toml` & `psychopy_plugin_template-0.0.5/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 [project]
 # the name of your plugin (required)
 name = "psychopy-plugin-template"
 # the current version of the plugin (required)
-version = "0.0.2" 
+version = "0.0.5" 
 # a brief description of what your plugin does
 description = "Tutorial on how to create a plugin component for both PsychoPy and PsychoJS"
+# link to the README.md file for a longer description of the project
+readme = "README.md"
 # contact information for yourself and anyone else who worked on the plugin 
 authors = [
   { name = "OST Science Team", email = "science@opensceincetools.org" },
 ]
 # a license tells other people how to use your code and protects you from stealing
 license = { text = "MIT" }
 # add any packages which your plugin needs in order to run
@@ -30,29 +32,45 @@
 tests = [
   "psychopy",
   "pytest",
 ]
 
 [project.entry-points."psychopy.experiment.components"]
 # if you want a Component to appear in the "Components" panel, add its class here
-ExampleComponent = "psychopy_example_plugin.components.exampleComponent:ExampleComponent"
+ExampleComponent = "psychopy_plugin_template.components.exampleComponent:ExampleComponent"
 
 [project.entry-points."psychopy.experiment.routines"]
 # if you want a Standalone Routine to appear in the "Components" panel, add its class here
-ExampleStandaloneRoutine = "psychopy_example_plugin.routines.exampleStandaloneRoutine:ExampleStandaloneRoutine"
+ExampleStandaloneRoutine = "psychopy_plugin_template.routines.exampleStandaloneRoutine:ExampleStandaloneRoutine"
 
 [project.entry-points."psychopy.visual"]
 # if you want something to be importable from psychopy.visual, add it here
-ExampleVisualStim = "psychopy_example_plugin.visual.exampleVisualStim:ExampleVisualStim"
+ExampleVisualStim = "psychopy_plugin_template.visual.exampleVisualStim:ExampleVisualStim"
 
 [project.entry-points."psychopy.hardware"]
 # if you want something to be importable from psychopy.hardware, add it here
-ExampleDevice = "psychopy_example_plugin.hardware.exampleDevice:ExampleDevice"
-ExampleResponseDevice = "psychopy_example_plugin.hardware.exampleResponseDevice:ExampleResponseDevice"
+ExampleDevice = "psychopy_plugin_template.hardware.exampleDevice:ExampleDevice"
+ExampleResponseDevice = "psychopy_plugin_template.hardware.exampleResponseDevice:ExampleResponseDevice"
+
+[project.entry-points."psychopy.app.builder"]
+# if you want to add a section to the PsychoPy Builder ribbon, add it here
+ExamplePluginRibbonSection = "psychopy_plugin_template.app.ribbon:ExamplePluginRibbonSection"
+
+[project.entry-points."psychopy.app.coder"]
+# if you want to add a section to the PsychoPy Coder ribbon, add it here
+ExamplePluginRibbonSection = "psychopy_plugin_template.app.ribbon:ExamplePluginRibbonSection"
+
+[project.entry-points."psychopy.app.runner"]
+# if you want to add a section to the PsychoPy Runner ribbon, add it here
+ExamplePluginRibbonSection = "psychopy_plugin_template.app.ribbon:ExamplePluginRibbonSection"
+
+[project.entry-points."psychopy.app.themes.icons"]
+# if you want to add icons to the PsychoPy app, add them here
+example = "psychopy_plugin_template.icons.example"
 
 [tool.setuptools.package-data]
 # any resources you want including in the package, add their file extensions here (e.g. "*.wav" if you want audio files)
 "*" = ["*.png"] 
 
 [tool.setuptools.packages.find]
 # any folders to ignore when building the Python package for this plugin
-exclude = ["docs*", "docs_src*", "tests*"]
+exclude = ["docs*", "docs_src*", "tests*"]
```

