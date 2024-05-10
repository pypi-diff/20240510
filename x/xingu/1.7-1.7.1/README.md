# Comparing `tmp/xingu-1.7.tar.gz` & `tmp/xingu-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xingu-1.7.tar", last modified: Wed May  8 21:51:48 2024, max compression
+gzip compressed data, was "xingu-1.7.1.tar", last modified: Fri May 10 13:22:03 2024, max compression
```

## Comparing `xingu-1.7.tar` & `xingu-1.7.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-05-08 21:51:48.616026 xingu-1.7/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7652 2024-01-03 19:20:34.000000 xingu-1.7/LICENSE
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    21759 2024-05-08 21:51:48.616026 xingu-1.7/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11571 2024-01-10 19:09:00.000000 xingu-1.7/README.md
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1275 2024-05-08 21:50:45.000000 xingu-1.7/pyproject.toml
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2024-05-08 21:51:48.616026 xingu-1.7/setup.cfg
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-05-08 21:51:48.616026 xingu-1.7/xingu/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      434 2024-01-24 19:13:14.000000 xingu-1.7/xingu/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    18963 2024-02-08 01:10:52.000000 xingu-1.7/xingu/__main__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    50476 2024-05-08 14:27:16.000000 xingu-1.7/xingu/coach.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7378 2024-01-03 19:20:34.000000 xingu-1.7/xingu/config_manager.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    22307 2024-01-24 22:47:35.000000 xingu-1.7/xingu/dataprovider.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     5498 2024-01-03 19:20:34.000000 xingu-1.7/xingu/dataproviderfactory.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2506 2024-01-03 19:20:34.000000 xingu-1.7/xingu/estimator.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-05-08 21:51:48.616026 xingu-1.7/xingu/estimators/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    12628 2024-01-03 19:20:34.000000 xingu-1.7/xingu/estimators/catboost.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)   101841 2024-05-08 21:46:31.000000 xingu-1.7/xingu/model.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-05-08 21:51:48.616026 xingu-1.7/xingu.egg-info/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    21759 2024-05-08 21:51:48.000000 xingu-1.7/xingu.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      397 2024-05-08 21:51:48.000000 xingu-1.7/xingu.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2024-05-08 21:51:48.000000 xingu-1.7/xingu.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       46 2024-05-08 21:51:48.000000 xingu-1.7/xingu.egg-info/entry_points.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      115 2024-05-08 21:51:48.000000 xingu-1.7/xingu.egg-info/requires.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        6 2024-05-08 21:51:48.000000 xingu-1.7/xingu.egg-info/top_level.txt
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-05-10 13:22:03.640466 xingu-1.7.1/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7652 2024-01-03 19:20:34.000000 xingu-1.7.1/LICENSE
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    21761 2024-05-10 13:22:03.640466 xingu-1.7.1/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11571 2024-01-10 19:09:00.000000 xingu-1.7.1/README.md
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1277 2024-05-10 13:21:14.000000 xingu-1.7.1/pyproject.toml
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2024-05-10 13:22:03.640466 xingu-1.7.1/setup.cfg
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-05-10 13:22:03.636466 xingu-1.7.1/xingu/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      434 2024-01-24 19:13:14.000000 xingu-1.7.1/xingu/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    19409 2024-05-09 20:29:57.000000 xingu-1.7.1/xingu/__main__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    50497 2024-05-10 13:13:55.000000 xingu-1.7.1/xingu/coach.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7378 2024-01-03 19:20:34.000000 xingu-1.7.1/xingu/config_manager.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    22328 2024-05-09 20:54:52.000000 xingu-1.7.1/xingu/dataprovider.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     5498 2024-01-03 19:20:34.000000 xingu-1.7.1/xingu/dataproviderfactory.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2523 2024-05-09 20:50:35.000000 xingu-1.7.1/xingu/estimator.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-05-10 13:22:03.636466 xingu-1.7.1/xingu/estimators/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    12628 2024-01-03 19:20:34.000000 xingu-1.7.1/xingu/estimators/catboost.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)   101862 2024-05-10 13:13:05.000000 xingu-1.7.1/xingu/model.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-05-10 13:22:03.636466 xingu-1.7.1/xingu.egg-info/
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    21761 2024-05-10 13:22:03.000000 xingu-1.7.1/xingu.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      397 2024-05-10 13:22:03.000000 xingu-1.7.1/xingu.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2024-05-10 13:22:03.000000 xingu-1.7.1/xingu.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       46 2024-05-10 13:22:03.000000 xingu-1.7.1/xingu.egg-info/entry_points.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      115 2024-05-10 13:22:03.000000 xingu-1.7.1/xingu.egg-info/requires.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        6 2024-05-10 13:22:03.000000 xingu-1.7.1/xingu.egg-info/top_level.txt
```

### Comparing `xingu-1.7/LICENSE` & `xingu-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xingu-1.7/PKG-INFO` & `xingu-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xingu
-Version: 1.7
+Version: 1.7.1
 Summary: Automated ML model training and packaging
 Author-email: Avi Alkalay <avi@unix.sh>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `xingu-1.7/README.md` & `xingu-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `xingu-1.7/pyproject.toml` & `xingu-1.7.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xingu"
-version = '1.7'
+version = '1.7.1'
 description = "Automated ML model training and packaging"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
 authors = [
     { name = "Avi Alkalay", email = "avi@unix.sh" },
 ]
```

### Comparing `xingu-1.7/xingu/__main__.py` & `xingu-1.7.1/xingu/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,33 @@
 from . import ConfigManager
 
 
 
 def prepare_logging(level=logging.INFO):
     # Switch between INFO/DEBUG while running in production/developping:
 
-    # Configure logging for PanModel
+    # Configure logging for the command line
+
+    FORMATTER = logging.Formatter("%(asctime)s|%(levelname)s|%(name)s|%(message)s")
+    HANDLER = logging.StreamHandler()
+    HANDLER.setFormatter(FORMATTER)
+
+    logger = logging.getLogger()
+    logger.addHandler(HANDLER)
+    logger.setLevel(level)
+
+    return logger
+
+
+
+
+def prepare_logging_OLD(level=logging.INFO):
+    # Switch between INFO/DEBUG while running in production/developping:
+
+    # Configure logging for the command line
 
     FORMATTER = logging.Formatter("%(asctime)s|%(levelname)s|%(name)s|%(message)s")
     HANDLER = logging.StreamHandler()
     HANDLER.setFormatter(FORMATTER)
 
     loggers=[
         logging.getLogger('__main__'),
```

### Comparing `xingu-1.7/xingu/coach.py` & `xingu-1.7.1/xingu/coach.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 
 
     def __init__(self, dp_factory: DataProviderFactory = DataProviderFactory()):
         self.config=ConfigManager()
 
         # Setup logging
-        self.logger = logging.getLogger(__name__ + '.' + self.__class__.__name__)
+        self.logger = logging.getLogger(self.__class__.__module__ + '.' + self.__class__.__qualname__)
 
         # Turn attribute `databases` into a private copy
         self.databases=dict()
 
         try:
             import pygit2
             self.git_repo=pygit2.Repository(self.get_config('PROJECT_HOME'))
```

### Comparing `xingu-1.7/xingu/config_manager.py` & `xingu-1.7.1/xingu/config_manager.py`

 * *Files identical despite different names*

### Comparing `xingu-1.7/xingu/dataprovider.py` & `xingu-1.7.1/xingu/dataprovider.py`

 * *Files 1% similar despite different names*

```diff
@@ -373,15 +373,15 @@
     ###   of them.
     ###
     ###########################################################
 
 
     def get_logger(self):
         if not hasattr(self,'logger'):
-            self.logger = logging.getLogger(__name__ + '.' + self.__class__.__name__)
+            self.logger = logging.getLogger(self.__class__.__module__ + '.' + self.__class__.__qualname__)
 
         return self.logger
 
 
 
     def log(self, message='', level=logging.INFO):
         self.get_logger().log(
```

### Comparing `xingu-1.7/xingu/dataproviderfactory.py` & `xingu-1.7.1/xingu/dataproviderfactory.py`

 * *Files identical despite different names*

### Comparing `xingu-1.7/xingu/estimator.py` & `xingu-1.7.1/xingu/estimator.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         pass
 
 
 
     def is_classifier(self):
         pass
 
-    
+
 
     def __repr__(self):
         return '{klass}()'.format(klass=type(self).__name__)
 
 
 
     def __getstate__(self):
@@ -88,15 +88,15 @@
         )
 
 
 
     def setup_logger(self):
         if not hasattr(self,'logger'):
             # Setup logging
-            self.logger = logging.getLogger(__name__ + '.' + self.__class__.__name__)
+            self.logger = logging.getLogger(self.__class__.__module__ + '.' + self.__class__.__qualname__)
 
 
 
     def log(self, message='', level=logging.INFO):
         self.setup_logger()
         self.logger.log(
             level,
```

### Comparing `xingu-1.7/xingu/estimators/catboost.py` & `xingu-1.7.1/xingu/estimators/catboost.py`

 * *Files identical despite different names*

### Comparing `xingu-1.7/xingu/model.py` & `xingu-1.7.1/xingu/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
             - None - use Estimator object internal defaults
 
         - delayed_prereq_binding: If DP specifies pre-req models, do not load them too.
         Instead, a later call to self.load_pre_req_model() will be necessary.
         """
 
         # Setup logging
-        self.logger = logging.getLogger(__name__ + '.' + self.__class__.__name__)
+        self.logger = logging.getLogger(self.__class__.__module__ + '.' + self.__class__.__qualname__)
 
         # Setup coach
         self.coach=coach
 
         # What type of context I'm in? Might be None, "train" or "batch_predict"
         self.context=None
```

### Comparing `xingu-1.7/xingu.egg-info/PKG-INFO` & `xingu-1.7.1/xingu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xingu
-Version: 1.7
+Version: 1.7.1
 Summary: Automated ML model training and packaging
 Author-email: Avi Alkalay <avi@unix.sh>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

