# Comparing `tmp/ouster_mapping-0.2.0.tar.gz` & `tmp/ouster_mapping-0.2.1.tar.gz`

## Comparing `ouster_mapping-0.2.0.tar` & `ouster_mapping-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    14458 2020-02-02 00:00:00.000000 ouster_mapping-0.2.0/ouster/cli/plugins/cli_mapping_impl.py
--rw-r--r--   0        0        0     3943 2020-02-02 00:00:00.000000 ouster_mapping-0.2.0/ouster/cli/plugins/cli_source_mapping.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ouster_mapping-0.2.0/ouster/mapping/__about__.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ouster_mapping-0.2.0/ouster/mapping/__init__.py
--rw-r--r--   0        0        0     5532 2020-02-02 00:00:00.000000 ouster_mapping-0.2.0/ouster/mapping/kiss_backend.py
--rw-r--r--   0        0        0     5810 2020-02-02 00:00:00.000000 ouster_mapping-0.2.0/ouster/mapping/ouster_kiss_icp.py
--rw-r--r--   0        0        0     6051 2020-02-02 00:00:00.000000 ouster_mapping-0.2.0/ouster/mapping/ply_to_png.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 ouster_mapping-0.2.0/ouster/mapping/slam.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 ouster_mapping-0.2.0/ouster/mapping/slam_backend.py
--rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 ouster_mapping-0.2.0/ouster/mapping/util.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 ouster_mapping-0.2.0/.gitignore
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 ouster_mapping-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 ouster_mapping-0.2.0/ouster/README.rst
--rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 ouster_mapping-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    14458 2020-02-02 00:00:00.000000 ouster_mapping-0.2.1/ouster/cli/plugins/cli_mapping_impl.py
+-rw-r--r--   0        0        0     3943 2020-02-02 00:00:00.000000 ouster_mapping-0.2.1/ouster/cli/plugins/cli_source_mapping.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ouster_mapping-0.2.1/ouster/mapping/__about__.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ouster_mapping-0.2.1/ouster/mapping/__init__.py
+-rw-r--r--   0        0        0     5525 2020-02-02 00:00:00.000000 ouster_mapping-0.2.1/ouster/mapping/kiss_backend.py
+-rw-r--r--   0        0        0     5820 2020-02-02 00:00:00.000000 ouster_mapping-0.2.1/ouster/mapping/ouster_kiss_icp.py
+-rw-r--r--   0        0        0     6051 2020-02-02 00:00:00.000000 ouster_mapping-0.2.1/ouster/mapping/ply_to_png.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 ouster_mapping-0.2.1/ouster/mapping/slam.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 ouster_mapping-0.2.1/ouster/mapping/slam_backend.py
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 ouster_mapping-0.2.1/ouster/mapping/util.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 ouster_mapping-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 ouster_mapping-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 ouster_mapping-0.2.1/ouster/README.rst
+-rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 ouster_mapping-0.2.1/PKG-INFO
```

### Comparing `ouster_mapping-0.2.0/ouster/cli/plugins/cli_mapping_impl.py` & `ouster_mapping-0.2.1/ouster/cli/plugins/cli_mapping_impl.py`

 * *Files identical despite different names*

### Comparing `ouster_mapping-0.2.0/ouster/cli/plugins/cli_source_mapping.py` & `ouster_mapping-0.2.1/ouster/cli/plugins/cli_source_mapping.py`

 * *Files identical despite different names*

### Comparing `ouster_mapping-0.2.0/ouster/mapping/kiss_backend.py` & `ouster_mapping-0.2.1/ouster/mapping/kiss_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
         if self.last_id != -1 and scan_mid_ts <= self.ts_pose[-1][0]:
             logger.warning(
                 "LidarScan timestamp is out of order. Use estimate timestamp instead")
             # fallback on defaults while accounting for potential skipped
             # frames
             ts_delta = abs(scan.frame_id - self.last_id) * self.frame_ts_dur
-            scan_mid_ts = self.kiss_icp.poses[-1][0] + ts_delta
+            scan_mid_ts = self.ts_pose[-1][0] + ts_delta
         self.ts_pose.append((scan_mid_ts, self.kiss_icp.poses[-1]))
 
         if len(self.ts_pose) >= 2:
             col_global_poses = util.getScanColPoseWithTs(
                 self.ts_pose[-2][1], self.ts_pose[-1][1], scan)
             scan.pose[:] = col_global_poses
         elif len(self.ts_pose) < 2:
```

### Comparing `ouster_mapping-0.2.0/ouster/mapping/ouster_kiss_icp.py` & `ouster_mapping-0.2.1/ouster/mapping/ouster_kiss_icp.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,19 +65,19 @@
 
     def _cal_ts_diff_ratio(self, ts) -> float:
         if len(self.last_two_ts) < 2:
             self.last_two_ts.append(ts)
             return 1.0
 
         ts_diff_prev = self.last_two_ts[-1] - self.last_two_ts[-2]
-        ts_diff_cur = ts - self.last_two_ts[-1]
 
-        if ts_diff_prev == 0 or ts_diff_cur < 0:
+        if ts_diff_prev == 0 or ts < self.last_two_ts[-1]:
             return 1.0
 
+        ts_diff_cur = ts - self.last_two_ts[-1]
         # calculate frame drop ratio using real timestamps
         frame_drop_ratio = ts_diff_cur / ts_diff_prev
 
         self.last_two_ts.append(ts)
         return frame_drop_ratio
 
     def register_frame(self, frame, timestamps, scan_ts):
```

### Comparing `ouster_mapping-0.2.0/ouster/mapping/ply_to_png.py` & `ouster_mapping-0.2.1/ouster/mapping/ply_to_png.py`

 * *Files identical despite different names*

### Comparing `ouster_mapping-0.2.0/ouster/mapping/slam_backend.py` & `ouster_mapping-0.2.1/ouster/mapping/slam_backend.py`

 * *Files identical despite different names*

### Comparing `ouster_mapping-0.2.0/ouster/mapping/util.py` & `ouster_mapping-0.2.1/ouster/mapping/util.py`

 * *Files identical despite different names*

### Comparing `ouster_mapping-0.2.0/pyproject.toml` & `ouster_mapping-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12"
 ]
 dependencies = [
-  "ouster-sdk ==0.11.0",
+  "ouster-sdk ==0.11.1",
   # point-cloud-utils doesn't support Linux Arm and and it depends on scipy which is not supported on Mac M1 with Mac OS < 12.0
   'point-cloud-utils >=0.30.4, <1; python_version <= "3.11" and platform_machine != "aarch64" and (platform_system != "Darwin" or platform_machine != "arm64" or platform_version >= "21.0.0")',
   'kiss-icp ==0.4.0; platform_machine != "aarch64"',
   "numpy >=1.19, <2, !=1.19.4",
   "laspy >=2.5.0, <3"
 ]
```

### Comparing `ouster_mapping-0.2.0/ouster/README.rst` & `ouster_mapping-0.2.1/ouster/README.rst`

 * *Files identical despite different names*

### Comparing `ouster_mapping-0.2.0/PKG-INFO` & `ouster_mapping-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.3
 Name: ouster-mapping
-Version: 0.2.0
+Version: 0.2.1
 Summary: Library to perform basic SLAM with Ouster lidars
 Author-email: Tomas Svarovsky <tomas.svarovsky@ouster.io>
 License-Expression: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Requires-Dist: kiss-icp==0.4.0; platform_machine != 'aarch64'
 Requires-Dist: laspy<3,>=2.5.0
 Requires-Dist: numpy!=1.19.4,<2,>=1.19
-Requires-Dist: ouster-sdk==0.11.0
+Requires-Dist: ouster-sdk==0.11.1
 Requires-Dist: point-cloud-utils<1,>=0.30.4; python_version <= '3.11' and platform_machine != 'aarch64' and (platform_system != 'Darwin' or platform_machine != 'arm64' or platform_version >= '21.0.0')
 Description-Content-Type: text/x-rst
 
 Ouster SDK Mapping
 ==================
 
 ..
```

