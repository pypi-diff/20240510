# Comparing `tmp/truedata-6.0.3.tar.gz` & `tmp/truedata-6.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truedata-6.0.3.tar", last modified: Sat Feb  3 10:05:53 2024, max compression
+gzip compressed data, was "truedata-6.0.4.tar", last modified: Fri May 10 15:47:23 2024, max compression
```

## Comparing `truedata-6.0.3.tar` & `truedata-6.0.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-02-03 10:05:53.358312 truedata-6.0.3/
--rw-rw-rw-   0        0        0    35821 2021-12-02 19:45:54.000000 truedata-6.0.3/LICENSE
--rw-rw-rw-   0        0        0    16117 2024-02-03 10:05:53.355315 truedata-6.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    15395 2024-02-03 10:02:30.000000 truedata-6.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-02-03 10:05:53.358312 truedata-6.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1025 2023-12-19 06:16:33.000000 truedata-6.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-03 10:05:53.274370 truedata-6.0.3/truedata/
--rw-rw-rw-   0        0        0      213 2024-02-03 10:02:30.000000 truedata-6.0.3/truedata/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-03 10:05:53.320327 truedata-6.0.3/truedata/analytics/
--rw-rw-rw-   0        0        0    12230 2024-01-16 15:53:26.000000 truedata-6.0.3/truedata/analytics/TD_analytics.py
--rw-rw-rw-   0        0        0       40 2023-12-19 06:16:33.000000 truedata-6.0.3/truedata/analytics/__init__.py
--rw-rw-rw-   0        0        0      313 2023-12-19 06:16:33.000000 truedata-6.0.3/truedata/analytics/decorators.py
-drwxrwxrwx   0        0        0        0 2024-02-03 10:05:53.330322 truedata-6.0.3/truedata/history/
--rw-rw-rw-   0        0        0     7367 2024-01-12 05:25:55.000000 truedata-6.0.3/truedata/history/Historical_REST.py
--rw-rw-rw-   0        0        0     6123 2024-01-16 15:45:54.000000 truedata-6.0.3/truedata/history/TD_hist.py
--rw-rw-rw-   0        0        0       31 2023-12-19 06:16:33.000000 truedata-6.0.3/truedata/history/__init__.py
--rw-rw-rw-   0        0        0     2051 2023-12-19 06:16:33.000000 truedata-6.0.3/truedata/history/utils.py
-drwxrwxrwx   0        0        0        0 2024-02-03 10:05:53.334319 truedata-6.0.3/truedata/tests/
--rw-rw-rw-   0        0        0       64 2023-12-19 06:16:33.000000 truedata-6.0.3/truedata/tests/__init__.py
--rw-rw-rw-   0        0        0      214 2023-12-19 06:16:33.000000 truedata-6.0.3/truedata/tests/defaults.py
-drwxrwxrwx   0        0        0        0 2024-02-03 10:05:53.350319 truedata-6.0.3/truedata/websocket/
--rw-rw-rw-   0        0        0     4825 2023-12-19 06:16:33.000000 truedata-6.0.3/truedata/websocket/TD_chain.py
--rw-rw-rw-   0        0        0     7347 2024-02-03 10:02:30.000000 truedata-6.0.3/truedata/websocket/TD_live.py
--rw-rw-rw-   0        0        0    15359 2024-02-03 10:02:30.000000 truedata-6.0.3/truedata/websocket/TD_ws.py
--rw-rw-rw-   0        0        0       30 2023-12-19 06:16:33.000000 truedata-6.0.3/truedata/websocket/__init__.py
--rw-rw-rw-   0        0        0     2229 2024-02-01 17:01:54.000000 truedata-6.0.3/truedata/websocket/constants.py
--rw-rw-rw-   0        0        0      554 2023-12-19 06:16:34.000000 truedata-6.0.3/truedata/websocket/exceptions.py
--rw-rw-rw-   0        0        0    13749 2024-02-01 17:01:54.000000 truedata-6.0.3/truedata/websocket/utils.py
-drwxrwxrwx   0        0        0        0 2024-02-03 10:05:53.353315 truedata-6.0.3/truedata.egg-info/
--rw-rw-rw-   0        0        0    16117 2024-02-03 10:05:53.000000 truedata-6.0.3/truedata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      691 2024-02-03 10:05:53.000000 truedata-6.0.3/truedata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-03 10:05:53.000000 truedata-6.0.3/truedata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      106 2024-02-03 10:05:53.000000 truedata-6.0.3/truedata.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-02-03 10:05:53.000000 truedata-6.0.3/truedata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 15:47:23.529683 truedata-6.0.4/
+-rw-rw-rw-   0        0        0    35821 2021-12-02 19:45:54.000000 truedata-6.0.4/LICENSE
+-rw-rw-rw-   0        0        0    16201 2024-05-10 15:47:23.529683 truedata-6.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    15479 2024-05-10 15:45:15.000000 truedata-6.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-10 15:47:23.529683 truedata-6.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1025 2023-12-19 06:16:33.000000 truedata-6.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 15:47:23.451143 truedata-6.0.4/truedata/
+-rw-rw-rw-   0        0        0      213 2024-05-10 15:46:03.000000 truedata-6.0.4/truedata/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 15:47:23.482803 truedata-6.0.4/truedata/analytics/
+-rw-rw-rw-   0        0        0    12230 2024-02-18 14:49:37.000000 truedata-6.0.4/truedata/analytics/TD_analytics.py
+-rw-rw-rw-   0        0        0       40 2023-12-19 06:16:33.000000 truedata-6.0.4/truedata/analytics/__init__.py
+-rw-rw-rw-   0        0        0      313 2023-12-19 06:16:33.000000 truedata-6.0.4/truedata/analytics/decorators.py
+drwxrwxrwx   0        0        0        0 2024-05-10 15:47:23.498432 truedata-6.0.4/truedata/history/
+-rw-rw-rw-   0        0        0     7367 2024-01-12 05:25:55.000000 truedata-6.0.4/truedata/history/Historical_REST.py
+-rw-rw-rw-   0        0        0     6123 2024-01-16 15:45:54.000000 truedata-6.0.4/truedata/history/TD_hist.py
+-rw-rw-rw-   0        0        0       31 2023-12-19 06:16:33.000000 truedata-6.0.4/truedata/history/__init__.py
+-rw-rw-rw-   0        0        0     2051 2023-12-19 06:16:33.000000 truedata-6.0.4/truedata/history/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-10 15:47:23.498432 truedata-6.0.4/truedata/tests/
+-rw-rw-rw-   0        0        0       64 2023-12-19 06:16:33.000000 truedata-6.0.4/truedata/tests/__init__.py
+-rw-rw-rw-   0        0        0      214 2023-12-19 06:16:33.000000 truedata-6.0.4/truedata/tests/defaults.py
+drwxrwxrwx   0        0        0        0 2024-05-10 15:47:23.514073 truedata-6.0.4/truedata/websocket/
+-rw-rw-rw-   0        0        0     4825 2023-12-19 06:16:33.000000 truedata-6.0.4/truedata/websocket/TD_chain.py
+-rw-rw-rw-   0        0        0     7347 2024-05-10 15:42:46.000000 truedata-6.0.4/truedata/websocket/TD_live.py
+-rw-rw-rw-   0        0        0    15390 2024-05-10 15:43:49.000000 truedata-6.0.4/truedata/websocket/TD_ws.py
+-rw-rw-rw-   0        0        0       30 2023-12-19 06:16:33.000000 truedata-6.0.4/truedata/websocket/__init__.py
+-rw-rw-rw-   0        0        0     2229 2024-04-22 05:48:36.000000 truedata-6.0.4/truedata/websocket/constants.py
+-rw-rw-rw-   0        0        0      554 2023-12-19 06:16:34.000000 truedata-6.0.4/truedata/websocket/exceptions.py
+-rw-rw-rw-   0        0        0    13749 2024-05-10 15:42:27.000000 truedata-6.0.4/truedata/websocket/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-10 15:47:23.514073 truedata-6.0.4/truedata.egg-info/
+-rw-rw-rw-   0        0        0    16201 2024-05-10 15:47:22.000000 truedata-6.0.4/truedata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      691 2024-05-10 15:47:23.000000 truedata-6.0.4/truedata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 15:47:22.000000 truedata-6.0.4/truedata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      106 2024-05-10 15:47:22.000000 truedata-6.0.4/truedata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-10 15:47:22.000000 truedata-6.0.4/truedata.egg-info/top_level.txt
```

### Comparing `truedata-6.0.3/LICENSE` & `truedata-6.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `truedata-6.0.3/PKG-INFO` & `truedata-6.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: truedata
-Version: 6.0.3
+Version: 6.0.4
 Summary: Truedata's Official Python Package
 Home-page: https://github.com/kapilmar/truedata-ws
 Author: Nahas N
 Author-email: nahas@truedata.in
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -403,14 +403,18 @@
 * gainers , losers function takes following arguments:
   * segment (string) : NSEEQ, NSEFUT, NSEOPT, MCX
   * topn (int) : default 10 , top n number  
 
 ----
 # Release Notes
 
+Version 6.0.4
+*   removing automatic reconnection after manual disconnection 
+
+
 Version 6.0.3
 *   lz4 version released to latest one without prebuild
 
 Version 6.0.2
 *   analytics new methods added 
 
 Version 6.0.0
```

### Comparing `truedata-6.0.3/README.md` & `truedata-6.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -382,14 +382,18 @@
 * gainers , losers function takes following arguments:
   * segment (string) : NSEEQ, NSEFUT, NSEOPT, MCX
   * topn (int) : default 10 , top n number  
 
 ----
 # Release Notes
 
+Version 6.0.4
+*   removing automatic reconnection after manual disconnection 
+
+
 Version 6.0.3
 *   lz4 version released to latest one without prebuild
 
 Version 6.0.2
 *   analytics new methods added 
 
 Version 6.0.0
```

### Comparing `truedata-6.0.3/setup.py` & `truedata-6.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `truedata-6.0.3/truedata/analytics/TD_analytics.py` & `truedata-6.0.4/truedata/analytics/TD_analytics.py`

 * *Files identical despite different names*

### Comparing `truedata-6.0.3/truedata/history/Historical_REST.py` & `truedata-6.0.4/truedata/history/Historical_REST.py`

 * *Files identical despite different names*

### Comparing `truedata-6.0.3/truedata/history/TD_hist.py` & `truedata-6.0.4/truedata/history/TD_hist.py`

 * *Files identical despite different names*

### Comparing `truedata-6.0.3/truedata/history/utils.py` & `truedata-6.0.4/truedata/history/utils.py`

 * *Files identical despite different names*

### Comparing `truedata-6.0.3/truedata/websocket/TD_chain.py` & `truedata-6.0.4/truedata/websocket/TD_chain.py`

 * *Files identical despite different names*

### Comparing `truedata-6.0.3/truedata/websocket/TD_live.py` & `truedata-6.0.4/truedata/websocket/TD_live.py`

 * *Files identical despite different names*

### Comparing `truedata-6.0.3/truedata/websocket/TD_ws.py` & `truedata-6.0.4/truedata/websocket/TD_ws.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,14 +254,14 @@
                 self.logger.debug(f'{restart_symbols} needs resuming here.')
                 self.parent_app.start_live_data(restart_symbols, restart_flag = True )
                 self.logger.info(f'All streaming symbols have been resumed.')
 
     def ws_close(self, *args):
         self.sock.close() if self.sock is not None else 0
         self.sock = None
-        if (self.last_ping_tm == 0 and self.last_pong_tm == 0) or (self.last_ping_tm > self.last_pong_tm) :
+        if not self.disconnect_flag and ((self.last_ping_tm == 0 and self.last_pong_tm == 0) or (self.last_ping_tm > self.last_pong_tm)) :
             self.logger.debug('DISCONNECTED FROM SERVER. RETRYING IN 5 SEC......')
             try:
                 time.sleep(5)
                 self.run_forever(ping_interval=10, ping_timeout=5)
             except Exception as e:
                 self.logger.error(f'{type(e)} in reconnection => {e}')
```

### Comparing `truedata-6.0.3/truedata/websocket/constants.py` & `truedata-6.0.4/truedata/websocket/constants.py`

 * *Files identical despite different names*

### Comparing `truedata-6.0.3/truedata/websocket/exceptions.py` & `truedata-6.0.4/truedata/websocket/exceptions.py`

 * *Files identical despite different names*

### Comparing `truedata-6.0.3/truedata/websocket/utils.py` & `truedata-6.0.4/truedata/websocket/utils.py`

 * *Files identical despite different names*

### Comparing `truedata-6.0.3/truedata.egg-info/PKG-INFO` & `truedata-6.0.4/truedata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: truedata
-Version: 6.0.3
+Version: 6.0.4
 Summary: Truedata's Official Python Package
 Home-page: https://github.com/kapilmar/truedata-ws
 Author: Nahas N
 Author-email: nahas@truedata.in
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -403,14 +403,18 @@
 * gainers , losers function takes following arguments:
   * segment (string) : NSEEQ, NSEFUT, NSEOPT, MCX
   * topn (int) : default 10 , top n number  
 
 ----
 # Release Notes
 
+Version 6.0.4
+*   removing automatic reconnection after manual disconnection 
+
+
 Version 6.0.3
 *   lz4 version released to latest one without prebuild
 
 Version 6.0.2
 *   analytics new methods added 
 
 Version 6.0.0
```

### Comparing `truedata-6.0.3/truedata.egg-info/SOURCES.txt` & `truedata-6.0.4/truedata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

