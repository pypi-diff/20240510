# Comparing `tmp/jeedomdaemon-0.8.0.tar.gz` & `tmp/jeedomdaemon-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeedomdaemon-0.8.0.tar", last modified: Fri May 10 08:42:53 2024, max compression
+gzip compressed data, was "jeedomdaemon-0.8.1.tar", last modified: Fri May 10 14:53:44 2024, max compression
```

## Comparing `jeedomdaemon-0.8.0.tar` & `jeedomdaemon-0.8.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:42:53.686906 jeedomdaemon-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-10 08:42:49.000000 jeedomdaemon-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4607 2024-05-10 08:42:53.686906 jeedomdaemon-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-05-10 08:42:49.000000 jeedomdaemon-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:42:53.686906 jeedomdaemon-0.8.0/jeedomdaemon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 08:42:49.000000 jeedomdaemon-0.8.0/jeedomdaemon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-05-10 08:42:49.000000 jeedomdaemon-0.8.0/jeedomdaemon/aio_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-05-10 08:42:49.000000 jeedomdaemon-0.8.0/jeedomdaemon/base_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5120 2024-05-10 08:42:49.000000 jeedomdaemon-0.8.0/jeedomdaemon/base_daemon.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-10 08:42:49.000000 jeedomdaemon-0.8.0/jeedomdaemon/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:42:53.686906 jeedomdaemon-0.8.0/jeedomdaemon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4607 2024-05-10 08:42:53.000000 jeedomdaemon-0.8.0/jeedomdaemon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-10 08:42:53.000000 jeedomdaemon-0.8.0/jeedomdaemon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 08:42:53.000000 jeedomdaemon-0.8.0/jeedomdaemon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-10 08:42:53.000000 jeedomdaemon-0.8.0/jeedomdaemon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-10 08:42:53.000000 jeedomdaemon-0.8.0/jeedomdaemon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 08:42:53.686906 jeedomdaemon-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-10 08:42:49.000000 jeedomdaemon-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:42:53.686906 jeedomdaemon-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 08:42:49.000000 jeedomdaemon-0.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-10 08:42:49.000000 jeedomdaemon-0.8.0/tests/base_config_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-10 08:42:49.000000 jeedomdaemon-0.8.0/tests/base_daemon_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:53:44.447498 jeedomdaemon-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-10 14:53:40.000000 jeedomdaemon-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4607 2024-05-10 14:53:44.447498 jeedomdaemon-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-05-10 14:53:40.000000 jeedomdaemon-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:53:44.443498 jeedomdaemon-0.8.1/jeedomdaemon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:53:40.000000 jeedomdaemon-0.8.1/jeedomdaemon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-05-10 14:53:40.000000 jeedomdaemon-0.8.1/jeedomdaemon/aio_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-05-10 14:53:40.000000 jeedomdaemon-0.8.1/jeedomdaemon/base_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-05-10 14:53:40.000000 jeedomdaemon-0.8.1/jeedomdaemon/base_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-10 14:53:40.000000 jeedomdaemon-0.8.1/jeedomdaemon/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:53:44.447498 jeedomdaemon-0.8.1/jeedomdaemon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4607 2024-05-10 14:53:44.000000 jeedomdaemon-0.8.1/jeedomdaemon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-10 14:53:44.000000 jeedomdaemon-0.8.1/jeedomdaemon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 14:53:44.000000 jeedomdaemon-0.8.1/jeedomdaemon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-10 14:53:44.000000 jeedomdaemon-0.8.1/jeedomdaemon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-10 14:53:44.000000 jeedomdaemon-0.8.1/jeedomdaemon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 14:53:44.447498 jeedomdaemon-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-10 14:53:40.000000 jeedomdaemon-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:53:44.447498 jeedomdaemon-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:53:40.000000 jeedomdaemon-0.8.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-10 14:53:40.000000 jeedomdaemon-0.8.1/tests/base_config_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-10 14:53:40.000000 jeedomdaemon-0.8.1/tests/base_daemon_test.py
```

### Comparing `jeedomdaemon-0.8.0/LICENSE` & `jeedomdaemon-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.8.0/PKG-INFO` & `jeedomdaemon-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jeedomdaemon
-Version: 0.8.0
+Version: 0.8.1
 Summary: A base to implement Jeedom daemon in python
 Home-page: https://github.com/Mips2648/jeedom-daemon-py
 Author: Mips
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
```

### Comparing `jeedomdaemon-0.8.0/README.md` & `jeedomdaemon-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.8.0/jeedomdaemon/aio_connector.py` & `jeedomdaemon-0.8.1/jeedomdaemon/aio_connector.py`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.8.0/jeedomdaemon/base_config.py` & `jeedomdaemon-0.8.1/jeedomdaemon/base_config.py`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.8.0/jeedomdaemon/base_daemon.py` & `jeedomdaemon-0.8.1/jeedomdaemon/base_daemon.py`

 * *Files 12% similar despite different names*

```diff
@@ -50,14 +50,15 @@
         try:
             self._logger.info('Starting daemon with log level: %s', self._config.log_level)
             Utils.write_pid(str(self._config.pid_filename))
 
             asyncio.run(self.__run())
         except Exception as e: # pylint: disable=broad-exception-caught
             self._logger.error('Fatal error: %s', e)
+            self.stop()
         finally:
             self._logger.info("Shutdown")
             try:
                 self._logger.debug("Removing PID file %s", self._config.pid_filename)
                 os.remove(self._config.pid_filename)
             except: # pylint: disable=bare-except
                 pass
@@ -86,22 +87,20 @@
             await self.__add_signal_handler()
             await asyncio.sleep(1) # allow  all tasks to start
 
             await self.__listen_task
 
     def stop(self):
         """ Stop your daemon if need be"""
+
         if self.__on_stop_cb is not None:
-            future = asyncio.run_coroutine_threadsafe(self.__on_stop_cb(), self._loop)
-            try:
-                future.result(2)
-            except asyncio.TimeoutError:
-                self._logger.warning('The on_stop coroutine took too long')
-            except Exception as exc:
-                self._logger.error('The on_stop coroutine raised an exception: %s', exc)
+            self._logger.info("create on stop callback task")
+            stop_task = asyncio.create_task(self.__on_stop_cb)
+            asyncio.gather(stop_task)
+            self._logger.info("on stop callback task done")
 
         tasks = [t for t in asyncio.all_tasks() if t is not asyncio.current_task()]
         tasks = asyncio.all_tasks()
         self._logger.info("Cancelling %i outstanding tasks", len(tasks))
         for task in tasks:
             task.cancel()
         try:
```

### Comparing `jeedomdaemon-0.8.0/jeedomdaemon/utils.py` & `jeedomdaemon-0.8.1/jeedomdaemon/utils.py`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.8.0/jeedomdaemon.egg-info/PKG-INFO` & `jeedomdaemon-0.8.1/jeedomdaemon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jeedomdaemon
-Version: 0.8.0
+Version: 0.8.1
 Summary: A base to implement Jeedom daemon in python
 Home-page: https://github.com/Mips2648/jeedom-daemon-py
 Author: Mips
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
```

### Comparing `jeedomdaemon-0.8.0/setup.py` & `jeedomdaemon-0.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     author='Mips',
     # author_email='',
     # Needed to actually package something
     packages=find_packages(),
     # Needed for dependencies
     install_requires=['aiohttp'],
     # *strongly* suggested for sharing
-    version='0.8.0',
+    version='0.8.1',
     # The license can be anything you like
     license='MIT',
     description='A base to implement Jeedom daemon in python',
     # We will also need a readme eventually (there will be a warning)
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
 )
```

### Comparing `jeedomdaemon-0.8.0/tests/base_config_test.py` & `jeedomdaemon-0.8.1/tests/base_config_test.py`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.8.0/tests/base_daemon_test.py` & `jeedomdaemon-0.8.1/tests/base_daemon_test.py`

 * *Files identical despite different names*

