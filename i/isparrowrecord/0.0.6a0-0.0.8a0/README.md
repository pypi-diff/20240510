# Comparing `tmp/isparrowrecord-0.0.6a0.tar.gz` & `tmp/isparrowrecord-0.0.8a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isparrowrecord-0.0.6a0.tar", last modified: Fri May 10 13:51:19 2024, max compression
+gzip compressed data, was "isparrowrecord-0.0.8a0.tar", last modified: Fri May 10 14:22:14 2024, max compression
```

## Comparing `isparrowrecord-0.0.6a0.tar` & `isparrowrecord-0.0.8a0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:51:19.937043 isparrowrecord-0.0.6a0/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-10 13:51:16.000000 isparrowrecord-0.0.6a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14099 2024-05-10 13:51:19.937043 isparrowrecord-0.0.6a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-10 13:51:16.000000 isparrowrecord-0.0.6a0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-10 13:51:16.000000 isparrowrecord-0.0.6a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 13:51:19.937043 isparrowrecord-0.0.6a0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:51:19.933043 isparrowrecord-0.0.6a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:51:19.933043 isparrowrecord-0.0.6a0/src/iSparrowRecord/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-10 13:51:16.000000 isparrowrecord-0.0.6a0/src/iSparrowRecord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11178 2024-05-10 13:51:16.000000 isparrowrecord-0.0.6a0/src/iSparrowRecord/audio_recording.py
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-05-10 13:51:16.000000 isparrowrecord-0.0.6a0/src/iSparrowRecord/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-05-10 13:51:16.000000 isparrowrecord-0.0.6a0/src/iSparrowRecord/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-10 13:51:16.000000 isparrowrecord-0.0.6a0/src/iSparrowRecord/set_up.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-10 13:51:16.000000 isparrowrecord-0.0.6a0/src/iSparrowRecord/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:51:19.937043 isparrowrecord-0.0.6a0/src/isparrowrecord.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14099 2024-05-10 13:51:19.000000 isparrowrecord-0.0.6a0/src/isparrowrecord.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-10 13:51:19.000000 isparrowrecord-0.0.6a0/src/isparrowrecord.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 13:51:19.000000 isparrowrecord-0.0.6a0/src/isparrowrecord.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-10 13:51:19.000000 isparrowrecord-0.0.6a0/src/isparrowrecord.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-10 13:51:19.000000 isparrowrecord-0.0.6a0/src/isparrowrecord.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-10 13:51:19.000000 isparrowrecord-0.0.6a0/src/isparrowrecord.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:22:14.481076 isparrowrecord-0.0.8a0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-10 14:22:10.000000 isparrowrecord-0.0.8a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15452 2024-05-10 14:22:14.481076 isparrowrecord-0.0.8a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-10 14:22:10.000000 isparrowrecord-0.0.8a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-10 14:22:10.000000 isparrowrecord-0.0.8a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 14:22:14.481076 isparrowrecord-0.0.8a0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:22:14.477076 isparrowrecord-0.0.8a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:22:14.481076 isparrowrecord-0.0.8a0/src/iSparrowRecord/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-10 14:22:10.000000 isparrowrecord-0.0.8a0/src/iSparrowRecord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11178 2024-05-10 14:22:10.000000 isparrowrecord-0.0.8a0/src/iSparrowRecord/audio_recording.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-05-10 14:22:10.000000 isparrowrecord-0.0.8a0/src/iSparrowRecord/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-05-10 14:22:10.000000 isparrowrecord-0.0.8a0/src/iSparrowRecord/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-10 14:22:10.000000 isparrowrecord-0.0.8a0/src/iSparrowRecord/set_up.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-10 14:22:10.000000 isparrowrecord-0.0.8a0/src/iSparrowRecord/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:22:14.481076 isparrowrecord-0.0.8a0/src/isparrowrecord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15452 2024-05-10 14:22:14.000000 isparrowrecord-0.0.8a0/src/isparrowrecord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-10 14:22:14.000000 isparrowrecord-0.0.8a0/src/isparrowrecord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 14:22:14.000000 isparrowrecord-0.0.8a0/src/isparrowrecord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-10 14:22:14.000000 isparrowrecord-0.0.8a0/src/isparrowrecord.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-10 14:22:14.000000 isparrowrecord-0.0.8a0/src/isparrowrecord.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-10 14:22:14.000000 isparrowrecord-0.0.8a0/src/isparrowrecord.egg-info/top_level.txt
```

### Comparing `isparrowrecord-0.0.6a0/LICENSE` & `isparrowrecord-0.0.8a0/LICENSE`

 * *Files identical despite different names*

### Comparing `isparrowrecord-0.0.6a0/PKG-INFO` & `isparrowrecord-0.0.8a0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isparrowrecord
-Version: 0.0.6a0
+Version: 0.0.8a0
 Summary: Audio Recording Facilities for the isparrow package
 Author-email: Inga Ulusoy <inga.ulusoy@uni-heidelberg.de>, Harald Mack <harald.mack@iwr.uni-heidelberg.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -225,10 +225,40 @@
 
 ## Summary 
 tbd
 
 ## Features 
 tbd 
 
-## Installation 
-tbd 
+## Installation
+iSparrowRecord officially only supports Linux-based operating systems and tests on Ubuntu. That being said, it has been successfully deployed on macOS, too. However, it has never been tried on Windows. Follow the following instruction to run it on Ubuntu: 
+
+- Install portaudio and python development libraries first. `iSparrowRecord` depends on pyaudio, which in turn depends on portaudio. Hence, these steps are essential. 
+```bash 
+sudo apt install python3.x-dev portaudio19-dev
+```
+Replace the `x` with the python version you want `iSparrowRecord` to run on, or leave it out and use `python3` only if you want your OS' default python version. `iSparrowRecord` has been tested on `python3.9` and `python3.12`.
+
+- Then, to get the newest release, install `iSparrowRecord` via pip: 
+```bash 
+python3.x -m pip install isparrowrecord
+```
+After this, you should be able to get the `iSparrowRecord` cli in a terminal window by typing `iSparrowRecord`. 
+
+For a development installation, install `iSparrowRecord` in editable mode: 
 
+- Clone this repository
+```bash
+ git clone https://github.com/ssciwr/iSparrowRecord.git 
+```
+or, when you're using ssh: 
+```bash
+git@github.com:ssciwr/iSparrowRecord.git
+```
+
+- then, from the root directory of the repository: 
+```bash 
+python3 -m pip install -e . && python3 -m pip install -r requirements-dev.txt
+```
+
+## Usage
+tbd
```

### Comparing `isparrowrecord-0.0.6a0/pyproject.toml` & `isparrowrecord-0.0.8a0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `isparrowrecord-0.0.6a0/src/iSparrowRecord/audio_recording.py` & `isparrowrecord-0.0.8a0/src/iSparrowRecord/audio_recording.py`

 * *Files identical despite different names*

### Comparing `isparrowrecord-0.0.6a0/src/iSparrowRecord/cli.py` & `isparrowrecord-0.0.8a0/src/iSparrowRecord/cli.py`

 * *Files identical despite different names*

### Comparing `isparrowrecord-0.0.6a0/src/iSparrowRecord/runner.py` & `isparrowrecord-0.0.8a0/src/iSparrowRecord/runner.py`

 * *Files identical despite different names*

### Comparing `isparrowrecord-0.0.6a0/src/iSparrowRecord/set_up.py` & `isparrowrecord-0.0.8a0/src/iSparrowRecord/set_up.py`

 * *Files identical despite different names*

### Comparing `isparrowrecord-0.0.6a0/src/iSparrowRecord/utils.py` & `isparrowrecord-0.0.8a0/src/iSparrowRecord/utils.py`

 * *Files identical despite different names*

### Comparing `isparrowrecord-0.0.6a0/src/isparrowrecord.egg-info/PKG-INFO` & `isparrowrecord-0.0.8a0/src/isparrowrecord.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isparrowrecord
-Version: 0.0.6a0
+Version: 0.0.8a0
 Summary: Audio Recording Facilities for the isparrow package
 Author-email: Inga Ulusoy <inga.ulusoy@uni-heidelberg.de>, Harald Mack <harald.mack@iwr.uni-heidelberg.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -225,10 +225,40 @@
 
 ## Summary 
 tbd
 
 ## Features 
 tbd 
 
-## Installation 
-tbd 
+## Installation
+iSparrowRecord officially only supports Linux-based operating systems and tests on Ubuntu. That being said, it has been successfully deployed on macOS, too. However, it has never been tried on Windows. Follow the following instruction to run it on Ubuntu: 
+
+- Install portaudio and python development libraries first. `iSparrowRecord` depends on pyaudio, which in turn depends on portaudio. Hence, these steps are essential. 
+```bash 
+sudo apt install python3.x-dev portaudio19-dev
+```
+Replace the `x` with the python version you want `iSparrowRecord` to run on, or leave it out and use `python3` only if you want your OS' default python version. `iSparrowRecord` has been tested on `python3.9` and `python3.12`.
+
+- Then, to get the newest release, install `iSparrowRecord` via pip: 
+```bash 
+python3.x -m pip install isparrowrecord
+```
+After this, you should be able to get the `iSparrowRecord` cli in a terminal window by typing `iSparrowRecord`. 
+
+For a development installation, install `iSparrowRecord` in editable mode: 
 
+- Clone this repository
+```bash
+ git clone https://github.com/ssciwr/iSparrowRecord.git 
+```
+or, when you're using ssh: 
+```bash
+git@github.com:ssciwr/iSparrowRecord.git
+```
+
+- then, from the root directory of the repository: 
+```bash 
+python3 -m pip install -e . && python3 -m pip install -r requirements-dev.txt
+```
+
+## Usage
+tbd
```

