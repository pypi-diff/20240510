# Comparing `tmp/pyneurotrace-0.8.0.tar.gz` & `tmp/pyneurotrace-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyneurotrace-0.8.0.tar", last modified: Fri May 10 06:19:27 2024, max compression
+gzip compressed data, was "pyneurotrace-0.9.5.tar", last modified: Fri May 10 18:50:58 2024, max compression
```

## Comparing `pyneurotrace-0.8.0.tar` & `pyneurotrace-0.9.5.tar`

### file list

```diff
@@ -1,24 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:19:27.254667 pyneurotrace-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-10 06:19:23.000000 pyneurotrace-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-10 06:19:27.254667 pyneurotrace-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-05-10 06:19:23.000000 pyneurotrace-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:19:27.254667 pyneurotrace-0.8.0/pyNeuroTrace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-10 06:19:27.000000 pyneurotrace-0.8.0/pyNeuroTrace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-10 06:19:27.000000 pyneurotrace-0.8.0/pyNeuroTrace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-10 06:19:27.000000 pyneurotrace-0.8.0/pyNeuroTrace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-10 06:19:27.000000 pyneurotrace-0.8.0/pyNeuroTrace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-10 06:19:27.000000 pyneurotrace-0.8.0/pyNeuroTrace.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:19:27.254667 pyneurotrace-0.8.0/pyneurotrace/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 06:19:23.000000 pyneurotrace-0.8.0/pyneurotrace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-10 06:19:23.000000 pyneurotrace-0.8.0/pyneurotrace/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-05-10 06:19:23.000000 pyneurotrace-0.8.0/pyneurotrace/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     9838 2024-05-10 06:19:23.000000 pyneurotrace-0.8.0/pyneurotrace/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-05-10 06:19:23.000000 pyneurotrace-0.8.0/pyneurotrace/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-05-10 06:19:23.000000 pyneurotrace-0.8.0/pyneurotrace/morphology.py
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-05-10 06:19:23.000000 pyneurotrace-0.8.0/pyneurotrace/nndFilter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-05-10 06:19:23.000000 pyneurotrace-0.8.0/pyneurotrace/notebook.py
--rw-r--r--   0 runner    (1001) docker     (127)    27263 2024-05-10 06:19:23.000000 pyneurotrace-0.8.0/pyneurotrace/viz.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-10 06:19:23.000000 pyneurotrace-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-10 06:19:23.000000 pyneurotrace-0.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 06:19:27.254667 pyneurotrace-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8457 2024-05-10 06:19:23.000000 pyneurotrace-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:50:58.451461 pyneurotrace-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-10 18:50:52.000000 pyneurotrace-0.9.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-05-10 18:50:58.451461 pyneurotrace-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-05-10 18:50:52.000000 pyneurotrace-0.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:50:58.451461 pyneurotrace-0.9.5/pyNeuroTrace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-05-10 18:50:58.000000 pyneurotrace-0.9.5/pyNeuroTrace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-10 18:50:58.000000 pyneurotrace-0.9.5/pyNeuroTrace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-10 18:50:58.000000 pyneurotrace-0.9.5/pyNeuroTrace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-10 18:50:58.000000 pyneurotrace-0.9.5/pyNeuroTrace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-10 18:50:58.000000 pyneurotrace-0.9.5/pyNeuroTrace.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:50:58.451461 pyneurotrace-0.9.5/pyneurotrace/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-10 18:50:52.000000 pyneurotrace-0.9.5/pyneurotrace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-10 18:50:52.000000 pyneurotrace-0.9.5/pyneurotrace/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-05-10 18:50:52.000000 pyneurotrace-0.9.5/pyneurotrace/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9838 2024-05-10 18:50:52.000000 pyneurotrace-0.9.5/pyneurotrace/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-05-10 18:50:52.000000 pyneurotrace-0.9.5/pyneurotrace/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:50:58.451461 pyneurotrace-0.9.5/pyneurotrace/gpu/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-10 18:50:52.000000 pyneurotrace-0.9.5/pyneurotrace/gpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-05-10 18:50:52.000000 pyneurotrace-0.9.5/pyneurotrace/gpu/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-05-10 18:50:52.000000 pyneurotrace-0.9.5/pyneurotrace/gpu/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-05-10 18:50:52.000000 pyneurotrace-0.9.5/pyneurotrace/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-05-10 18:50:52.000000 pyneurotrace-0.9.5/pyneurotrace/nndFilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-05-10 18:50:52.000000 pyneurotrace-0.9.5/pyneurotrace/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27263 2024-05-10 18:50:52.000000 pyneurotrace-0.9.5/pyneurotrace/viz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-10 18:50:52.000000 pyneurotrace-0.9.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-10 18:50:52.000000 pyneurotrace-0.9.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 18:50:58.451461 pyneurotrace-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8477 2024-05-10 18:50:52.000000 pyneurotrace-0.9.5/setup.py
```

### Comparing `pyneurotrace-0.8.0/PKG-INFO` & `pyneurotrace-0.9.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyNeuroTrace
-Version: 0.8.0
+Version: 0.9.5
 Summary: Python code for neural time series
 Home-page: https://github.com/padster/pyNeuroTrace
 Author: Pat Coleman
 Author-email: Pat Coleman <padsterpat@gmail.com>, Peter Hogg <peter.hogg@ubc.ca>
 Project-URL: Homepage, https://github.com/padster/pyNeuroTrace
 Project-URL: Issues, https://github.com/padster/pyNeuroTrace/issues
 Keywords: neuron,analysis,timeseries,neuroscience
@@ -19,14 +19,19 @@
 Requires-Dist: scikit-image
 Provides-Extra: gpu
 Requires-Dist: cupy; extra == "gpu"
 
 # PyNeuroTrace: Python code for Neural Timeseries
 
 ## Installation
+'pyNeuroTrace' can be installed with pip:
+
+```
+pip install pyNeuroTrace
+```
 
 This library can be installed directly from github, using pip:
 ```
 pip install --upgrade "git+https://github.com/padster/pyNeuroTrace#egg=pyneurotrace&subdirectory=pyneurotrace"
 ```
 
 ## Vizualization
```

### Comparing `pyneurotrace-0.8.0/README.md` & `pyneurotrace-0.9.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 # PyNeuroTrace: Python code for Neural Timeseries
 
 ## Installation
+'pyNeuroTrace' can be installed with pip:
+
+```
+pip install pyNeuroTrace
+```
 
 This library can be installed directly from github, using pip:
 ```
 pip install --upgrade "git+https://github.com/padster/pyNeuroTrace#egg=pyneurotrace&subdirectory=pyneurotrace"
 ```
 
 ## Vizualization
```

### Comparing `pyneurotrace-0.8.0/pyNeuroTrace.egg-info/PKG-INFO` & `pyneurotrace-0.9.5/pyNeuroTrace.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyNeuroTrace
-Version: 0.8.0
+Version: 0.9.5
 Summary: Python code for neural time series
 Home-page: https://github.com/padster/pyNeuroTrace
 Author: Pat Coleman
 Author-email: Pat Coleman <padsterpat@gmail.com>, Peter Hogg <peter.hogg@ubc.ca>
 Project-URL: Homepage, https://github.com/padster/pyNeuroTrace
 Project-URL: Issues, https://github.com/padster/pyNeuroTrace/issues
 Keywords: neuron,analysis,timeseries,neuroscience
@@ -19,14 +19,19 @@
 Requires-Dist: scikit-image
 Provides-Extra: gpu
 Requires-Dist: cupy; extra == "gpu"
 
 # PyNeuroTrace: Python code for Neural Timeseries
 
 ## Installation
+'pyNeuroTrace' can be installed with pip:
+
+```
+pip install pyNeuroTrace
+```
 
 This library can be installed directly from github, using pip:
 ```
 pip install --upgrade "git+https://github.com/padster/pyNeuroTrace#egg=pyneurotrace&subdirectory=pyneurotrace"
 ```
 
 ## Vizualization
```

### Comparing `pyneurotrace-0.8.0/pyneurotrace/events.py` & `pyneurotrace-0.9.5/pyneurotrace/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,7 +98,10 @@
         isEvent = np.zeros(n)
         for i in range(n):
             below = trace[i] < threshold
             isEvent[i] = (not below and numBelowBefore >= minBelowBefore)
             numBelowBefore = numBelowBefore + 1 if below else 0
         return isEvent
     return _forEachTimeseries(data, _singleRowThreshold)
+
+
+__all__ = ["ewma", "cusum", "thresholdEvents", "matchedFilter"]
```

### Comparing `pyneurotrace-0.8.0/pyneurotrace/files.py` & `pyneurotrace-0.9.5/pyneurotrace/files.py`

 * *Files identical despite different names*

### Comparing `pyneurotrace-0.8.0/pyneurotrace/filters.py` & `pyneurotrace-0.9.5/pyneurotrace/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,7 +101,9 @@
         for i in iterFunc(range(data.shape[0])):
             result[i] = func(data[i])
     elif dim == 3: # (x, y, timeseries)
         for i in iterFunc(range(data.shape[0])):
             for j in iterFunc(range(data.shape[1])):
                 result[i, j] = func(data[i, j])
     return result
+
+__all__ = ["nndSmooth", "okada", "deltaFOverF0", "_forEachTimeseries"]
```

### Comparing `pyneurotrace-0.8.0/pyneurotrace/morphology.py` & `pyneurotrace-0.9.5/pyneurotrace/morphology.py`

 * *Files identical despite different names*

### Comparing `pyneurotrace-0.8.0/pyneurotrace/nndFilter.py` & `pyneurotrace-0.9.5/pyneurotrace/nndFilter.py`

 * *Files identical despite different names*

### Comparing `pyneurotrace-0.8.0/pyneurotrace/notebook.py` & `pyneurotrace-0.9.5/pyneurotrace/notebook.py`

 * *Files identical despite different names*

### Comparing `pyneurotrace-0.8.0/pyneurotrace/viz.py` & `pyneurotrace-0.9.5/pyneurotrace/viz.py`

 * *Files identical despite different names*

### Comparing `pyneurotrace-0.8.0/pyproject.toml` & `pyneurotrace-0.9.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools >= 41.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "pyNeuroTrace"
-version = "0.8.0"
+version = "0.9.5"
 dependencies = [
     "numpy",
     "scipy",
     "h5py",
     "scikit-image",
 ]
 requires-python = ">=3.9"
```

### Comparing `pyneurotrace-0.8.0/setup.py` & `pyneurotrace-0.9.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
     # Alternatively, if you just want to distribute a single Python file, use
     # the `py_modules` argument instead as follows, which will expect a file
     # called `my_module.py` to exist:
     #
     #   py_modules=["my_module"],
     #
   
-    packages=['pyneurotrace'],
+    packages=['pyneurotrace', 'pyneurotrace.gpu'],
     #packages=find_packages(include=['pyneurotrace'], exclude=['contrib', 'docs', 'tests', 'paper']),  # Required
 
     # This field lists other packages that your project depends on to run.
     # Any package you put here will be installed by pip when your project is
     # installed, so they must be valid existing projects.
     #
     # For an analysis of "install_requires" vs pip's requirements files see:
```

