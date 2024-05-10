# Comparing `tmp/openai-cost-logger-0.3.1.tar.gz` & `tmp/openai-cost-logger-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai-cost-logger-0.3.1.tar", last modified: Sat Apr 27 13:48:23 2024, max compression
+gzip compressed data, was "openai-cost-logger-0.4.1.tar", last modified: Fri May 10 08:58:19 2024, max compression
```

## Comparing `openai-cost-logger-0.3.1.tar` & `openai-cost-logger-0.4.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:48:23.868429 openai-cost-logger-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-27 13:48:20.000000 openai-cost-logger-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-27 13:48:23.868429 openai-cost-logger-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-27 13:48:20.000000 openai-cost-logger-0.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:48:23.868429 openai-cost-logger-0.3.1/openai_cost_logger/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-27 13:48:20.000000 openai-cost-logger-0.3.1/openai_cost_logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-27 13:48:20.000000 openai-cost-logger-0.3.1/openai_cost_logger/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7398 2024-04-27 13:48:20.000000 openai-cost-logger-0.3.1/openai_cost_logger/openai_cost_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-27 13:48:20.000000 openai-cost-logger-0.3.1/openai_cost_logger/openai_cost_logger_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-04-27 13:48:20.000000 openai-cost-logger-0.3.1/openai_cost_logger/openai_cost_logger_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:48:23.868429 openai-cost-logger-0.3.1/openai_cost_logger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-27 13:48:23.000000 openai-cost-logger-0.3.1/openai_cost_logger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-27 13:48:23.000000 openai-cost-logger-0.3.1/openai_cost_logger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 13:48:23.000000 openai-cost-logger-0.3.1/openai_cost_logger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-27 13:48:23.000000 openai-cost-logger-0.3.1/openai_cost_logger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-27 13:48:23.000000 openai-cost-logger-0.3.1/openai_cost_logger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 13:48:23.868429 openai-cost-logger-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-27 13:48:20.000000 openai-cost-logger-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:58:19.515247 openai-cost-logger-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-10 08:58:15.000000 openai-cost-logger-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-10 08:58:19.515247 openai-cost-logger-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-10 08:58:15.000000 openai-cost-logger-0.4.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:58:19.515247 openai-cost-logger-0.4.1/openai_cost_logger/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-10 08:58:15.000000 openai-cost-logger-0.4.1/openai_cost_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-10 08:58:15.000000 openai-cost-logger-0.4.1/openai_cost_logger/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7398 2024-05-10 08:58:15.000000 openai-cost-logger-0.4.1/openai_cost_logger/openai_cost_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-10 08:58:15.000000 openai-cost-logger-0.4.1/openai_cost_logger/openai_cost_logger_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-05-10 08:58:15.000000 openai-cost-logger-0.4.1/openai_cost_logger/openai_cost_logger_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:58:19.515247 openai-cost-logger-0.4.1/openai_cost_logger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-10 08:58:19.000000 openai-cost-logger-0.4.1/openai_cost_logger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-10 08:58:19.000000 openai-cost-logger-0.4.1/openai_cost_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 08:58:19.000000 openai-cost-logger-0.4.1/openai_cost_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-10 08:58:19.000000 openai-cost-logger-0.4.1/openai_cost_logger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-10 08:58:19.000000 openai-cost-logger-0.4.1/openai_cost_logger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 08:58:19.515247 openai-cost-logger-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-10 08:58:15.000000 openai-cost-logger-0.4.1/setup.py
```

### Comparing `openai-cost-logger-0.3.1/LICENSE` & `openai-cost-logger-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openai-cost-logger-0.3.1/PKG-INFO` & `openai-cost-logger-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-cost-logger
-Version: 0.3.1
+Version: 0.4.1
 Summary: OpenAI Cost Logger
 Home-page: https://github.com/drudilorenzo/openai-cost-tracker
 Author: Lorenzo Drudi | Mikolaj Boronski | Ivan Zakazov
 Author-email: lorenzodrudi11@gmail.com
 License: MIT
 Keywords: openai,cost,logger,tracker,viz,llms
 Platform: UNKNOWN
```

### Comparing `openai-cost-logger-0.3.1/README.rst` & `openai-cost-logger-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `openai-cost-logger-0.3.1/openai_cost_logger/constants.py` & `openai-cost-logger-0.4.1/openai_cost_logger/constants.py`

 * *Files identical despite different names*

### Comparing `openai-cost-logger-0.3.1/openai_cost_logger/openai_cost_logger.py` & `openai-cost-logger-0.4.1/openai_cost_logger/openai_cost_logger.py`

 * *Files identical despite different names*

### Comparing `openai-cost-logger-0.3.1/openai_cost_logger/openai_cost_logger_viz.py` & `openai-cost-logger-0.4.1/openai_cost_logger/openai_cost_logger_viz.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,8 +115,27 @@
                                   This method reads all the files in the specified directory.
             last_n_days (int, optional): The number of last days to plot. Defaults to None.
         """
         OpenAICostLoggerViz.plot_cost_by_strftime(
             path=path,
             strftime_aggregator="%Y-%m-%d", 
             last_n_days=last_n_days
-        )
+        )
+        
+
+    @staticmethod
+    def print_experiment_cost(experiment: str, path: str = DEFAULT_LOG_PATH) -> None:
+        """Print the cost of the specified experiment. The name is case-insensitive.
+
+        Args:
+            experiment (str): The experiment name.
+            path (str, optional): Cost logs directory. Defaults to DEFAULT_LOG_PATH.
+                                  This method reads all the files in the specified directory.
+        """
+        cost = 0
+        for filename in os.listdir(path):
+            if filename.endswith(".json"):
+                with open(Path(path, filename), mode='r') as file:
+                    data = json.load(file)
+                    if "experiment_name" in data and data["experiment_name"].lower() == experiment.lower():
+                        cost += data["total_cost"]
+        print(f"Cost of '{experiment}': {round(cost, 6)} (USD)")
```

### Comparing `openai-cost-logger-0.3.1/openai_cost_logger.egg-info/PKG-INFO` & `openai-cost-logger-0.4.1/openai_cost_logger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-cost-logger
-Version: 0.3.1
+Version: 0.4.1
 Summary: OpenAI Cost Logger
 Home-page: https://github.com/drudilorenzo/openai-cost-tracker
 Author: Lorenzo Drudi | Mikolaj Boronski | Ivan Zakazov
 Author-email: lorenzodrudi11@gmail.com
 License: MIT
 Keywords: openai,cost,logger,tracker,viz,llms
 Platform: UNKNOWN
```

### Comparing `openai-cost-logger-0.3.1/setup.py` & `openai-cost-logger-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 # Read the README file (reStructuredText format)
 with open('README.rst') as f:
     long_description = f.read()
 
-version_number = '0.3.1'
+version_number = '0.4.1'
 
 setup(
     name='openai-cost-logger',
     version=version_number,
     author='Lorenzo Drudi | Mikolaj Boronski | Ivan Zakazov',
     description='OpenAI Cost Logger',
     author_email='lorenzodrudi11@gmail.com',
```

