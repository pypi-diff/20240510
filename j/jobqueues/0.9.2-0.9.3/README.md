# Comparing `tmp/jobqueues-0.9.2.tar.gz` & `tmp/jobqueues-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jobqueues-0.9.2.tar", last modified: Mon Mar  4 08:40:16 2024, max compression
+gzip compressed data, was "jobqueues-0.9.3.tar", last modified: Fri May 10 08:43:43 2024, max compression
```

## Comparing `jobqueues-0.9.2.tar` & `jobqueues-0.9.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 08:40:16.304880 jobqueues-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-04 08:38:59.000000 jobqueues-0.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-03-04 08:40:16.304880 jobqueues-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-04 08:38:59.000000 jobqueues-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 08:40:16.304880 jobqueues-0.9.2/jobqueues/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-03-04 08:38:59.000000 jobqueues-0.9.2/jobqueues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-04 08:40:16.304880 jobqueues-0.9.2/jobqueues/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 08:40:16.304880 jobqueues-0.9.2/jobqueues/celeryfiles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 08:38:59.000000 jobqueues-0.9.2/jobqueues/celeryfiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-04 08:38:59.000000 jobqueues-0.9.2/jobqueues/celeryfiles/celery.py
--rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-03-04 08:38:59.000000 jobqueues-0.9.2/jobqueues/celeryfiles/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6538 2024-03-04 08:38:59.000000 jobqueues-0.9.2/jobqueues/celeryqueue.py
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-03-04 08:38:59.000000 jobqueues-0.9.2/jobqueues/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-04 08:38:59.000000 jobqueues-0.9.2/jobqueues/config_lsf.yml
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-04 08:38:59.000000 jobqueues-0.9.2/jobqueues/config_slurm.yml
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-04 08:38:59.000000 jobqueues-0.9.2/jobqueues/home.py
--rw-r--r--   0 runner    (1001) docker     (127)    14057 2024-03-04 08:38:59.000000 jobqueues-0.9.2/jobqueues/localqueue.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-03-04 08:38:59.000000 jobqueues-0.9.2/jobqueues/logging.ini
--rw-r--r--   0 runner    (1001) docker     (127)    14566 2024-03-04 08:38:59.000000 jobqueues-0.9.2/jobqueues/lsfqueue.py
--rw-r--r--   0 runner    (1001) docker     (127)    10228 2024-03-04 08:38:59.000000 jobqueues-0.9.2/jobqueues/pbsqueue.py
--rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-03-04 08:38:59.000000 jobqueues-0.9.2/jobqueues/playqueue.py
--rw-r--r--   0 runner    (1001) docker     (127)    12161 2024-03-04 08:38:59.000000 jobqueues-0.9.2/jobqueues/sgequeue.py
--rw-r--r--   0 runner    (1001) docker     (127)     7067 2024-03-04 08:38:59.000000 jobqueues-0.9.2/jobqueues/simqueue.py
--rw-r--r--   0 runner    (1001) docker     (127)    26717 2024-03-04 08:38:59.000000 jobqueues-0.9.2/jobqueues/slurmqueue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 08:40:16.304880 jobqueues-0.9.2/jobqueues/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-04 08:38:59.000000 jobqueues-0.9.2/jobqueues/templates/SGE_job.sh.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-03-04 08:38:59.000000 jobqueues-0.9.2/jobqueues/templates/SLURM_job.sh.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-03-04 08:38:59.000000 jobqueues-0.9.2/jobqueues/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 08:40:16.304880 jobqueues-0.9.2/jobqueues.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-03-04 08:40:16.000000 jobqueues-0.9.2/jobqueues.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-03-04 08:40:16.000000 jobqueues-0.9.2/jobqueues.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 08:40:16.000000 jobqueues-0.9.2/jobqueues.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 08:40:09.000000 jobqueues-0.9.2/jobqueues.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-04 08:40:16.000000 jobqueues-0.9.2/jobqueues.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-04 08:40:16.000000 jobqueues-0.9.2/jobqueues.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-03-04 08:38:59.000000 jobqueues-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-04 08:40:16.304880 jobqueues-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-03-04 08:38:59.000000 jobqueues-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:43:43.813156 jobqueues-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-10 08:42:48.000000 jobqueues-0.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-10 08:43:43.813156 jobqueues-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-10 08:42:48.000000 jobqueues-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:43:43.813156 jobqueues-0.9.3/jobqueues/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-10 08:42:48.000000 jobqueues-0.9.3/jobqueues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-10 08:43:43.813156 jobqueues-0.9.3/jobqueues/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:43:43.813156 jobqueues-0.9.3/jobqueues/celeryfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 08:42:48.000000 jobqueues-0.9.3/jobqueues/celeryfiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-10 08:42:48.000000 jobqueues-0.9.3/jobqueues/celeryfiles/celery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-05-10 08:42:48.000000 jobqueues-0.9.3/jobqueues/celeryfiles/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6538 2024-05-10 08:42:48.000000 jobqueues-0.9.3/jobqueues/celeryqueue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-10 08:42:48.000000 jobqueues-0.9.3/jobqueues/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-10 08:42:48.000000 jobqueues-0.9.3/jobqueues/config_lsf.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-10 08:42:48.000000 jobqueues-0.9.3/jobqueues/config_slurm.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-10 08:42:48.000000 jobqueues-0.9.3/jobqueues/home.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14057 2024-05-10 08:42:48.000000 jobqueues-0.9.3/jobqueues/localqueue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-10 08:42:48.000000 jobqueues-0.9.3/jobqueues/logging.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    14566 2024-05-10 08:42:48.000000 jobqueues-0.9.3/jobqueues/lsfqueue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10228 2024-05-10 08:42:48.000000 jobqueues-0.9.3/jobqueues/pbsqueue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-05-10 08:42:48.000000 jobqueues-0.9.3/jobqueues/playqueue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12161 2024-05-10 08:42:48.000000 jobqueues-0.9.3/jobqueues/sgequeue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7067 2024-05-10 08:42:48.000000 jobqueues-0.9.3/jobqueues/simqueue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26717 2024-05-10 08:42:48.000000 jobqueues-0.9.3/jobqueues/slurmqueue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:43:43.813156 jobqueues-0.9.3/jobqueues/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-10 08:42:48.000000 jobqueues-0.9.3/jobqueues/templates/SGE_job.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-05-10 08:42:48.000000 jobqueues-0.9.3/jobqueues/templates/SLURM_job.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-10 08:42:48.000000 jobqueues-0.9.3/jobqueues/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:43:43.813156 jobqueues-0.9.3/jobqueues.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-10 08:43:43.000000 jobqueues-0.9.3/jobqueues.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-10 08:43:43.000000 jobqueues-0.9.3/jobqueues.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 08:43:43.000000 jobqueues-0.9.3/jobqueues.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 08:43:35.000000 jobqueues-0.9.3/jobqueues.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-10 08:43:43.000000 jobqueues-0.9.3/jobqueues.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-10 08:43:43.000000 jobqueues-0.9.3/jobqueues.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-10 08:42:48.000000 jobqueues-0.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-10 08:43:43.813156 jobqueues-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-10 08:42:48.000000 jobqueues-0.9.3/setup.py
```

### Comparing `jobqueues-0.9.2/PKG-INFO` & `jobqueues-0.9.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jobqueues
-Version: 0.9.2
+Version: 0.9.3
 Summary: Wrappers for various queueing systems in python
 Author-email: Acellera <info@acellera.com>
 Project-URL: Homepage, https://github.com/Acellera/jobqueues
 Project-URL: Bug Tracker, https://github.com/Acellera/jobqueues/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
```

### Comparing `jobqueues-0.9.2/jobqueues/celeryfiles/tasks.py` & `jobqueues-0.9.3/jobqueues/celeryfiles/tasks.py`

 * *Files identical despite different names*

### Comparing `jobqueues-0.9.2/jobqueues/celeryqueue.py` & `jobqueues-0.9.3/jobqueues/celeryqueue.py`

 * *Files identical despite different names*

### Comparing `jobqueues-0.9.2/jobqueues/config.py` & `jobqueues-0.9.3/jobqueues/config.py`

 * *Files identical despite different names*

### Comparing `jobqueues-0.9.2/jobqueues/home.py` & `jobqueues-0.9.3/jobqueues/home.py`

 * *Files identical despite different names*

### Comparing `jobqueues-0.9.2/jobqueues/localqueue.py` & `jobqueues-0.9.3/jobqueues/localqueue.py`

 * *Files identical despite different names*

### Comparing `jobqueues-0.9.2/jobqueues/lsfqueue.py` & `jobqueues-0.9.3/jobqueues/lsfqueue.py`

 * *Files identical despite different names*

### Comparing `jobqueues-0.9.2/jobqueues/pbsqueue.py` & `jobqueues-0.9.3/jobqueues/pbsqueue.py`

 * *Files identical despite different names*

### Comparing `jobqueues-0.9.2/jobqueues/playqueue.py` & `jobqueues-0.9.3/jobqueues/playqueue.py`

 * *Files identical despite different names*

### Comparing `jobqueues-0.9.2/jobqueues/sgequeue.py` & `jobqueues-0.9.3/jobqueues/sgequeue.py`

 * *Files identical despite different names*

### Comparing `jobqueues-0.9.2/jobqueues/simqueue.py` & `jobqueues-0.9.3/jobqueues/simqueue.py`

 * *Files identical despite different names*

### Comparing `jobqueues-0.9.2/jobqueues/slurmqueue.py` & `jobqueues-0.9.3/jobqueues/slurmqueue.py`

 * *Files identical despite different names*

### Comparing `jobqueues-0.9.2/jobqueues/templates/SGE_job.sh.j2` & `jobqueues-0.9.3/jobqueues/templates/SGE_job.sh.j2`

 * *Files identical despite different names*

### Comparing `jobqueues-0.9.2/jobqueues/templates/SLURM_job.sh.j2` & `jobqueues-0.9.3/jobqueues/templates/SLURM_job.sh.j2`

 * *Files identical despite different names*

### Comparing `jobqueues-0.9.2/jobqueues/util.py` & `jobqueues-0.9.3/jobqueues/util.py`

 * *Files identical despite different names*

### Comparing `jobqueues-0.9.2/jobqueues.egg-info/PKG-INFO` & `jobqueues-0.9.3/jobqueues.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jobqueues
-Version: 0.9.2
+Version: 0.9.3
 Summary: Wrappers for various queueing systems in python
 Author-email: Acellera <info@acellera.com>
 Project-URL: Homepage, https://github.com/Acellera/jobqueues
 Project-URL: Bug Tracker, https://github.com/Acellera/jobqueues/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
```

### Comparing `jobqueues-0.9.2/jobqueues.egg-info/SOURCES.txt` & `jobqueues-0.9.3/jobqueues.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jobqueues-0.9.2/pyproject.toml` & `jobqueues-0.9.3/pyproject.toml`

 * *Files identical despite different names*

