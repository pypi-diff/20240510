# Comparing `tmp/audiconnectpy-1.5.5.tar.gz` & `tmp/audiconnectpy-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiconnectpy-1.5.5.tar", last modified: Sun Apr 14 15:45:15 2024, max compression
+gzip compressed data, was "audiconnectpy-1.5.6.tar", last modified: Sun Apr 14 16:25:28 2024, max compression
```

## Comparing `audiconnectpy-1.5.5.tar` & `audiconnectpy-1.5.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:45:15.834628 audiconnectpy-1.5.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-14 15:45:04.000000 audiconnectpy-1.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-14 15:45:04.000000 audiconnectpy-1.5.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-14 15:45:15.834628 audiconnectpy-1.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-14 15:45:04.000000 audiconnectpy-1.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:45:15.834628 audiconnectpy-1.5.5/audiconnectpy/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-14 15:45:04.000000 audiconnectpy-1.5.5/audiconnectpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19481 2024-04-14 15:45:04.000000 audiconnectpy-1.5.5/audiconnectpy/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-04-14 15:45:04.000000 audiconnectpy-1.5.5/audiconnectpy/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    22856 2024-04-14 15:45:04.000000 audiconnectpy-1.5.5/audiconnectpy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-14 15:45:04.000000 audiconnectpy-1.5.5/audiconnectpy/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-14 15:45:04.000000 audiconnectpy-1.5.5/audiconnectpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-04-14 15:45:04.000000 audiconnectpy-1.5.5/audiconnectpy/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    24025 2024-04-14 15:45:04.000000 audiconnectpy-1.5.5/audiconnectpy/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    11650 2024-04-14 15:45:04.000000 audiconnectpy-1.5.5/audiconnectpy/services.py
--rw-r--r--   0 runner    (1001) docker     (127)    12482 2024-04-14 15:45:04.000000 audiconnectpy-1.5.5/audiconnectpy/vehicle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:45:15.834628 audiconnectpy-1.5.5/audiconnectpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-14 15:45:15.000000 audiconnectpy-1.5.5/audiconnectpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-14 15:45:15.000000 audiconnectpy-1.5.5/audiconnectpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 15:45:15.000000 audiconnectpy-1.5.5/audiconnectpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 15:45:15.000000 audiconnectpy-1.5.5/audiconnectpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-14 15:45:15.000000 audiconnectpy-1.5.5/audiconnectpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-14 15:45:15.000000 audiconnectpy-1.5.5/audiconnectpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-14 15:45:13.000000 audiconnectpy-1.5.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 15:45:15.834628 audiconnectpy-1.5.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:25:28.218730 audiconnectpy-1.5.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-14 16:25:15.000000 audiconnectpy-1.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-14 16:25:15.000000 audiconnectpy-1.5.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-14 16:25:28.218730 audiconnectpy-1.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-14 16:25:15.000000 audiconnectpy-1.5.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:25:28.218730 audiconnectpy-1.5.6/audiconnectpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-14 16:25:15.000000 audiconnectpy-1.5.6/audiconnectpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19481 2024-04-14 16:25:15.000000 audiconnectpy-1.5.6/audiconnectpy/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-04-14 16:25:15.000000 audiconnectpy-1.5.6/audiconnectpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22856 2024-04-14 16:25:15.000000 audiconnectpy-1.5.6/audiconnectpy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-14 16:25:15.000000 audiconnectpy-1.5.6/audiconnectpy/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-14 16:25:15.000000 audiconnectpy-1.5.6/audiconnectpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-04-14 16:25:15.000000 audiconnectpy-1.5.6/audiconnectpy/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24226 2024-04-14 16:25:15.000000 audiconnectpy-1.5.6/audiconnectpy/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11650 2024-04-14 16:25:15.000000 audiconnectpy-1.5.6/audiconnectpy/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12482 2024-04-14 16:25:15.000000 audiconnectpy-1.5.6/audiconnectpy/vehicle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:25:28.218730 audiconnectpy-1.5.6/audiconnectpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-14 16:25:28.000000 audiconnectpy-1.5.6/audiconnectpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-14 16:25:28.000000 audiconnectpy-1.5.6/audiconnectpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 16:25:28.000000 audiconnectpy-1.5.6/audiconnectpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 16:25:27.000000 audiconnectpy-1.5.6/audiconnectpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-14 16:25:28.000000 audiconnectpy-1.5.6/audiconnectpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-14 16:25:28.000000 audiconnectpy-1.5.6/audiconnectpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-14 16:25:25.000000 audiconnectpy-1.5.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 16:25:28.218730 audiconnectpy-1.5.6/setup.cfg
```

### Comparing `audiconnectpy-1.5.5/LICENSE` & `audiconnectpy-1.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.5.5/PKG-INFO` & `audiconnectpy-1.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.5.5
+Version: 1.5.6
 Summary: Provides asynchronous authentication and access to Audi Connect
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: connect,async,audi
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `audiconnectpy-1.5.5/README.md` & `audiconnectpy-1.5.6/README.md`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.5.5/audiconnectpy/actions.py` & `audiconnectpy-1.5.6/audiconnectpy/actions.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.5.5/audiconnectpy/api.py` & `audiconnectpy-1.5.6/audiconnectpy/api.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.5.5/audiconnectpy/auth.py` & `audiconnectpy-1.5.6/audiconnectpy/auth.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.5.5/audiconnectpy/helpers.py` & `audiconnectpy-1.5.6/audiconnectpy/helpers.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.5.5/audiconnectpy/models.py` & `audiconnectpy-1.5.6/audiconnectpy/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -191,32 +191,35 @@
                     odometer = raw_data.get("odometerStatus", {}).get("value", {})
                     attrs.update(
                         {
                             "measure_mileage": odometer.get("odometer"),
                             "gasoline_range": range.get("gasolineRange"),
                         }
                     )
-                case "oiLevel":
+                case "oilLevel":
                     data = raw_data.get("oilLevelStatus", {}).get("value", {})
-                    attrs.update({"oil_level_status": data.get("value")})
+                    attrs.update({"oil_level_valid": data.get("value")})
                 case "vehicleLights":
                     data = (
                         raw_data.get("lightsStatus", {})
                         .get("value", {})
                         .get("lights", [])
                     )
+                    attributes = {}
                     for light in data:
-                        attrs.update(
+                        attributes.update(
                             {
-                                f"lights_{light.get('name')}_turn_off": light.get(
-                                    "status"
-                                )
-                                == "Off"
+                                f"lights_{light.get('name')}": light.get("status")
+                                != "off"
                             }
                         )
+                    attrs.update(
+                        {**attributes, "lights_status": any(attributes.values())}
+                    )
+
                 case "vehicleHealthInspection":
                     data = raw_data.get("maintenanceStatus", {}).get("value", {})
                     attrs.update(
                         {
                             "maintenance_interval_time_to_inspection": data.get(
                                 "inspectionDue_days"
                             ),
@@ -267,87 +270,86 @@
     def windows_status(attrs: ExtendedDict) -> ExtendedDict:
         # Windows open status
         metadatas = ExtendedDict({})
         left_open = "closed" not in attrs.get("frontLeft", [])
         left_rear_open = "closed" not in attrs.get("rearLeft", [])
         right_open = "closed" not in attrs.get("frontRight", [])
         right_rear_open = "closed" not in attrs.get("rearRight", [])
-        any_window_open = (
-            left_open and left_rear_open and right_open and right_rear_open
-        )
+        windows_open = [left_open, left_rear_open, right_rear_open, right_rear_open]
         metadatas.update(
             {
                 "open_left_front_window": left_open,
                 "open_left_rear_window": left_rear_open,
                 "open_right_front_window": right_open,
                 "open_right_rear_window": right_rear_open,
-                "open_any_window": any_window_open,
+                "open_any_window": any(windows_open),
             }
         )
 
         if "unsupported" not in attrs.get("roofCover"):
-            metadatas.update(
-                {"open_roof_cover": "closed" not in attrs.get("roofCover", [])}
-            )
+            open_roof_cover = "closed" not in attrs.get("roofCover", [])
+            metadatas.update({"open_roof_cover": open_roof_cover})
+            windows_open.append(open_roof_cover)
+
         if "unsupported" not in attrs.get("sunRoof"):
-            metadatas.update(
-                {"open_sun_roof": "closed" not in attrs.get("sunRoof", [])}
-            )
+            open_sun_roof = "closed" not in attrs.get("sunRoof", [])
+            metadatas.update({"open_sun_roof": open_sun_roof})
+            windows_open.append(open_sun_roof)
+
+        metadatas.update({"open_any_window": any(windows_open)})
 
         return metadatas
 
     @staticmethod
     def doors_status(attrs: ExtendedDict) -> ExtendedDict:
         # Doors lock status
         metadatas = ExtendedDict({})
         left_unlock = "locked" not in attrs.get("frontLeft", [])
         left_rear_unlock = "locked" not in attrs.get("rearLeft", [])
         right_unlock = "locked" not in attrs.get("frontRight", [])
         right_rear_unlock = "locked" not in attrs.get("rearRight", [])
         trunk_unlock = "locked" not in attrs.get("trunk", [])
-        unlock_any_door = (
-            left_unlock and left_rear_unlock and right_unlock and right_rear_unlock
-        )
+        doors_unlock = [left_unlock, left_rear_unlock, right_unlock, right_rear_unlock]
         metadatas.update(
             {
                 "lock_left_front_door": left_unlock,
                 "lock_left_rear_door": left_rear_unlock,
                 "lock_right_front_door": right_unlock,
                 "lock_right_rear_door": right_rear_unlock,
                 "lock_trunk": trunk_unlock,
-                "lock_any_door": unlock_any_door,
-                "lock_doors_trunk": True if unlock_any_door and trunk_unlock else False,
+                "lock_any_door": any(doors_unlock),
+                "lock_doors_trunk": any(doors_unlock) and trunk_unlock,
             }
         )
 
         # Doors open status
         left_open = "closed" not in attrs.get("frontLeft", [])
         left_rear_open = "closed" not in attrs.get("rearLeft", [])
         right_open = "closed" not in attrs.get("frontRight", [])
         right_rear_open = "closed" not in attrs.get("rearRight", [])
         trunk_open = "closed" not in attrs.get("trunk", [])
         bonnet_open = "closed" not in attrs.get("bonnet", [])
-        open_any_door = (
-            left_open
-            and left_rear_open
-            and right_open
-            and right_rear_open
-            and trunk_open
-            and bonnet_open
-        )
+        doors_open = [
+            left_open,
+            left_rear_open,
+            right_open,
+            right_rear_open,
+            trunk_open,
+            bonnet_open,
+        ]
 
         metadatas.update(
             {
                 "open_left_front_door": left_open,
                 "open_left_rear_door": left_rear_open,
                 "open_right_front_door": right_open,
                 "open_right_rear_door": right_rear_open,
                 "open_trunk": trunk_open,
                 "open_bonnet": bonnet_open,
-                "open_any_door": open_any_door,
+                "open_any_door": any(doors_open),
             }
         )
 
         return metadatas
 
     @staticmethod
     def map_name_status(array: dict[str, Any]) -> dict[str, Any]:
```

### Comparing `audiconnectpy-1.5.5/audiconnectpy/services.py` & `audiconnectpy-1.5.6/audiconnectpy/services.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.5.5/audiconnectpy/vehicle.py` & `audiconnectpy-1.5.6/audiconnectpy/vehicle.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.5.5/audiconnectpy.egg-info/PKG-INFO` & `audiconnectpy-1.5.6/audiconnectpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.5.5
+Version: 1.5.6
 Summary: Provides asynchronous authentication and access to Audi Connect
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: connect,async,audi
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `audiconnectpy-1.5.5/pyproject.toml` & `audiconnectpy-1.5.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "audiconnectpy"
-version     = "1.5.5"
+version     = "1.5.6"
 license     = {text = "GPL-3"}
 description = "Provides asynchronous authentication and access to Audi Connect"
 readme      = "README.md"
 authors     = [
     {name = "Cyr-ius", email = "cyr-ius@ipocus.net"}
 ]
 keywords    = ["connect", "async", "audi"]
```

