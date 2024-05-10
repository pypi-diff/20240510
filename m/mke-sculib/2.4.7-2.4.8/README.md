# Comparing `tmp/mke_sculib-2.4.7.tar.gz` & `tmp/mke_sculib-2.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mke_sculib-2.4.7.tar", last modified: Thu May  9 21:17:12 2024, max compression
+gzip compressed data, was "mke_sculib-2.4.8.tar", last modified: Thu May  9 21:30:40 2024, max compression
```

## Comparing `mke_sculib-2.4.7.tar` & `mke_sculib-2.4.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 21:17:12.712926 mke_sculib-2.4.7/
--rw-rw-rw-   0        0        0    35149 2022-07-03 09:33:46.000000 mke_sculib-2.4.7/LICENSE
--rw-rw-rw-   0        0        0     4120 2024-05-09 21:17:12.712926 mke_sculib-2.4.7/PKG-INFO
--rw-rw-rw-   0        0        0     3367 2023-09-13 15:37:28.000000 mke_sculib-2.4.7/README.rst
--rw-rw-rw-   0        0        0      921 2024-05-09 21:17:12.716943 mke_sculib-2.4.7/setup.cfg
--rw-rw-rw-   0        0        0      359 2022-07-29 10:19:10.000000 mke_sculib-2.4.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-09 21:17:12.667472 mke_sculib-2.4.7/src/
-drwxrwxrwx   0        0        0        0 2024-05-09 21:17:12.706925 mke_sculib-2.4.7/src/mke_sculib/
--rw-rw-rw-   0        0        0      718 2024-05-09 21:17:00.000000 mke_sculib-2.4.7/src/mke_sculib/__init__.py
--rw-rw-rw-   0        0        0     1492 2022-07-08 13:07:16.000000 mke_sculib-2.4.7/src/mke_sculib/cam_sensors.py
--rw-rw-rw-   0        0        0    24398 2023-06-30 07:33:40.000000 mke_sculib-2.4.7/src/mke_sculib/chan_list_acu.py
--rw-rw-rw-   0        0        0     1261 2023-09-22 14:56:52.000000 mke_sculib-2.4.7/src/mke_sculib/helpers.py
--rw-rw-rw-   0        0        0     9874 2024-05-09 20:02:32.000000 mke_sculib-2.4.7/src/mke_sculib/js_helpers.py
--rw-rw-rw-   0        0        0    26166 2023-12-05 16:11:38.000000 mke_sculib-2.4.7/src/mke_sculib/mock_telescope.py
--rw-rw-rw-   0        0        0    97743 2024-05-09 21:16:52.000000 mke_sculib-2.4.7/src/mke_sculib/scu.py
--rw-rw-rw-   0        0        0    19532 2024-04-10 07:02:06.000000 mke_sculib-2.4.7/src/mke_sculib/sim.py
--rw-rw-rw-   0        0        0     9006 2024-03-13 10:18:35.000000 mke_sculib-2.4.7/src/mke_sculib/stellarium_api.py
-drwxrwxrwx   0        0        0        0 2024-05-09 21:17:12.709926 mke_sculib-2.4.7/src/mke_sculib.egg-info/
--rw-rw-rw-   0        0        0     4120 2024-05-09 21:17:12.000000 mke_sculib-2.4.7/src/mke_sculib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      483 2024-05-09 21:17:12.000000 mke_sculib-2.4.7/src/mke_sculib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 21:17:12.000000 mke_sculib-2.4.7/src/mke_sculib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-09 21:17:12.000000 mke_sculib-2.4.7/src/mke_sculib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-09 21:17:12.711933 mke_sculib-2.4.7/tests/
--rw-rw-rw-   0        0        0     9759 2024-05-09 13:27:46.000000 mke_sculib-2.4.7/tests/test_acu_sim.py
--rw-rw-rw-   0        0        0     2273 2023-12-05 16:11:38.000000 mke_sculib-2.4.7/tests/test_scu.py
+drwxrwxrwx   0        0        0        0 2024-05-09 21:30:40.662557 mke_sculib-2.4.8/
+-rw-rw-rw-   0        0        0    35149 2022-07-03 09:33:46.000000 mke_sculib-2.4.8/LICENSE
+-rw-rw-rw-   0        0        0     4120 2024-05-09 21:30:40.662557 mke_sculib-2.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3367 2023-09-13 15:37:28.000000 mke_sculib-2.4.8/README.rst
+-rw-rw-rw-   0        0        0      921 2024-05-09 21:30:40.663558 mke_sculib-2.4.8/setup.cfg
+-rw-rw-rw-   0        0        0      359 2022-07-29 10:19:10.000000 mke_sculib-2.4.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 21:30:40.646558 mke_sculib-2.4.8/src/
+drwxrwxrwx   0        0        0        0 2024-05-09 21:30:40.657556 mke_sculib-2.4.8/src/mke_sculib/
+-rw-rw-rw-   0        0        0     1124 2024-05-09 21:30:25.000000 mke_sculib-2.4.8/src/mke_sculib/__init__.py
+-rw-rw-rw-   0        0        0     1492 2022-07-08 13:07:16.000000 mke_sculib-2.4.8/src/mke_sculib/cam_sensors.py
+-rw-rw-rw-   0        0        0    24398 2023-06-30 07:33:40.000000 mke_sculib-2.4.8/src/mke_sculib/chan_list_acu.py
+-rw-rw-rw-   0        0        0     1261 2023-09-22 14:56:52.000000 mke_sculib-2.4.8/src/mke_sculib/helpers.py
+-rw-rw-rw-   0        0        0     9874 2024-05-09 20:02:32.000000 mke_sculib-2.4.8/src/mke_sculib/js_helpers.py
+-rw-rw-rw-   0        0        0    26166 2023-12-05 16:11:38.000000 mke_sculib-2.4.8/src/mke_sculib/mock_telescope.py
+-rw-rw-rw-   0        0        0    97874 2024-05-09 21:25:21.000000 mke_sculib-2.4.8/src/mke_sculib/scu.py
+-rw-rw-rw-   0        0        0    19532 2024-04-10 07:02:06.000000 mke_sculib-2.4.8/src/mke_sculib/sim.py
+-rw-rw-rw-   0        0        0     9006 2024-03-13 10:18:35.000000 mke_sculib-2.4.8/src/mke_sculib/stellarium_api.py
+drwxrwxrwx   0        0        0        0 2024-05-09 21:30:40.660556 mke_sculib-2.4.8/src/mke_sculib.egg-info/
+-rw-rw-rw-   0        0        0     4120 2024-05-09 21:30:40.000000 mke_sculib-2.4.8/src/mke_sculib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      483 2024-05-09 21:30:40.000000 mke_sculib-2.4.8/src/mke_sculib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 21:30:40.000000 mke_sculib-2.4.8/src/mke_sculib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-09 21:30:40.000000 mke_sculib-2.4.8/src/mke_sculib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 21:30:40.661557 mke_sculib-2.4.8/tests/
+-rw-rw-rw-   0        0        0     9759 2024-05-09 13:27:46.000000 mke_sculib-2.4.8/tests/test_acu_sim.py
+-rw-rw-rw-   0        0        0     2273 2023-12-05 16:11:38.000000 mke_sculib-2.4.8/tests/test_scu.py
```

### Comparing `mke_sculib-2.4.7/LICENSE` & `mke_sculib-2.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.7/PKG-INFO` & `mke_sculib-2.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mke_sculib
-Version: 2.4.7
+Version: 2.4.8
 Summary: MeerKAT Extension (SCU) (lib)rary for the MKE antennas and some basic simulators
 Home-page: https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib
 Author: Tobias Glaubach
 Author-email: tglaubach@mpifr-bonn.mpg.de
 Project-URL: Bug Tracker, https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib/-/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `mke_sculib-2.4.7/README.rst` & `mke_sculib-2.4.8/README.rst`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.7/setup.cfg` & `mke_sculib-2.4.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.7/src/mke_sculib/cam_sensors.py` & `mke_sculib-2.4.8/src/mke_sculib/cam_sensors.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.7/src/mke_sculib/chan_list_acu.py` & `mke_sculib-2.4.8/src/mke_sculib/chan_list_acu.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.7/src/mke_sculib/helpers.py` & `mke_sculib-2.4.8/src/mke_sculib/helpers.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.7/src/mke_sculib/js_helpers.py` & `mke_sculib-2.4.8/src/mke_sculib/js_helpers.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.7/src/mke_sculib/mock_telescope.py` & `mke_sculib-2.4.8/src/mke_sculib/mock_telescope.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.7/src/mke_sculib/scu.py` & `mke_sculib-2.4.8/src/mke_sculib/scu.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,14 +119,15 @@
 
 class TrackHandler(object):
     def __init__(self, scu, t, az, el, activate_logging, config_name, verb=False):
         self.scu = scu
         self.args = (t, az, el, activate_logging, config_name)
         self.t_end = Time(t[-1], format='mjd')
         self.verb=verb
+        self.influx_token = ''
 
     def get_t_remaining(self):
         """estimate of remaining time in tracking table (in seconds)"""
         return (self.t_end - self.scu.t_internal).to(u.s).value
 
     def __enter__(self):
         scu = self.scu
@@ -1892,18 +1893,21 @@
             v = tuple([v for p, v in vals.items() if p.endswith(b)])
             return v[0], v[1]
         
 
         
 
 
-    def get_from_scu_influx(self, tstart, tend, token, org = 'OHBDC', timeout=360_000, channels = None):
+    def get_from_scu_influx(self, tstart, tend, token=None, org = 'OHBDC', timeout=360_000, channels = None):
         if 'InfluxDBClient' not in locals():
             from influxdb_client import InfluxDBClient
-            
+        
+        if token is None and hasattr(self, 'influx_token') and self.influx_token:
+            token = self.influx_token
+
         base_query= """
                 from(bucket: "SCU")
                 |> range(start: {}, stop: {})
                 |> filter(fn: (r) => r["_measurement"] == "device_status")
                 |> filter(fn: (r) => r["device"] == "acu")
                 |> pivot(rowKey: ["_time"], columnKey: ["_field"], valueColumn: "_value")
                 |> keep(columns: ["_time", {}])
@@ -2215,23 +2219,22 @@
                 _log.warn('Retrying connection in {} sec (Ctrl-C to quit)'.format(sleep_time))
                 await asyncio.sleep(sleep_time)
                 continue
     
     def show_liveplot(self, channels:list=None):
         try:
             get_ipython().__class__.__name__
-            from IPython.display import display, HTML
-            from mke_sculib.js_helpers import make_livepos_page, make_liveplot_page
-            if not channels:
-                return HTML(make_livepos_page(self.ip, port = self.port))
-            else:
-                return HTML(make_liveplot_page(self.ip, channels, port = self.port))
         except NameError as err:
             raise EnvironmentError('Not running in Ipython!') 
-
+        from IPython.display import display, HTML
+        from mke_sculib.js_helpers import make_livepos_page, make_liveplot_page
+        if not channels:
+            return HTML(make_livepos_page(self.ip, port = self.port))
+        else:
+            return HTML(make_liveplot_page(self.ip, channels, port = self.port))
 
 
 def plot_tt(t, az, el, tint, do_show=True, is_simulation=False):
     if not 'plt' in locals():
         import matplotlib.pyplot as plt
 
     t_local = Time.now()
```

### Comparing `mke_sculib-2.4.7/src/mke_sculib/sim.py` & `mke_sculib-2.4.8/src/mke_sculib/sim.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.7/src/mke_sculib/stellarium_api.py` & `mke_sculib-2.4.8/src/mke_sculib/stellarium_api.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.7/src/mke_sculib.egg-info/PKG-INFO` & `mke_sculib-2.4.8/src/mke_sculib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mke-sculib
-Version: 2.4.7
+Version: 2.4.8
 Summary: MeerKAT Extension (SCU) (lib)rary for the MKE antennas and some basic simulators
 Home-page: https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib
 Author: Tobias Glaubach
 Author-email: tglaubach@mpifr-bonn.mpg.de
 Project-URL: Bug Tracker, https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib/-/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `mke_sculib-2.4.7/tests/test_acu_sim.py` & `mke_sculib-2.4.8/tests/test_acu_sim.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.7/tests/test_scu.py` & `mke_sculib-2.4.8/tests/test_scu.py`

 * *Files identical despite different names*

