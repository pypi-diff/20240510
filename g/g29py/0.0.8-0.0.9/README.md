# Comparing `tmp/g29py-0.0.8.tar.gz` & `tmp/g29py-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g29py-0.0.8.tar", max compression
+gzip compressed data, was "g29py-0.0.9.tar", max compression
```

## Comparing `g29py-0.0.8.tar` & `g29py-0.0.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2024-03-04 03:51:49.145823 g29py-0.0.8/LICENSE
--rw-r--r--   0        0        0     3064 2024-03-06 01:48:05.314185 g29py-0.0.8/README.md
--rw-r--r--   0        0        0       61 2024-03-01 03:50:11.664385 g29py-0.0.8/g29py/__init__.py
--rw-r--r--   0        0        0    11643 2024-03-07 05:21:22.969174 g29py-0.0.8/g29py/g29.py
--rw-r--r--   0        0        0      994 2024-03-07 05:05:53.997490 g29py-0.0.8/g29py/params.py
--rw-r--r--   0        0        0      423 2024-03-07 05:22:16.741612 g29py-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3777 1970-01-01 00:00:00.000000 g29py-0.0.8/setup.py
--rw-r--r--   0        0        0     3563 1970-01-01 00:00:00.000000 g29py-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-03-04 03:51:49.145823 g29py-0.0.9/LICENSE
+-rw-r--r--   0        0        0     3057 2024-05-10 04:30:43.941674 g29py-0.0.9/README.md
+-rw-r--r--   0        0        0       61 2024-05-10 04:45:42.314086 g29py-0.0.9/g29py/__init__.py
+-rw-r--r--   0        0        0    11985 2024-05-10 04:44:55.741859 g29py-0.0.9/g29py/g29.py
+-rw-r--r--   0        0        0      994 2024-03-07 05:05:53.997490 g29py-0.0.9/g29py/params.py
+-rw-r--r--   0        0        0      423 2024-05-10 04:45:52.610136 g29py-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3770 1970-01-01 00:00:00.000000 g29py-0.0.9/setup.py
+-rw-r--r--   0        0        0     3556 1970-01-01 00:00:00.000000 g29py-0.0.9/PKG-INFO
```

### Comparing `g29py-0.0.8/LICENSE` & `g29py-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `g29py-0.0.8/README.md` & `g29py-0.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # write 
 g29.set_range(500)
 g29.set_friction(0.5)
 ```
 
 ```python
 # read
-g29.start_pumping() # thread
+g29.listen() # thread
 while 1:
     state = g29.get_state()
     print("steering:", state["steering"])
     print("brake:", state["brake"])
     print("accelerator", state["accelerator"])
 ```
```

### Comparing `g29py-0.0.8/g29py/g29.py` & `g29py-0.0.9/g29py/g29.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import hid
 import time
 import threading
 import logging as log
 from .params import *
 
 class G29:
+    connected = False
     cache = None
     state = {
         "steering": 0.0,
         "accelerator": -1.0,
         "clutch": -1.0,
         "brake": -1.0,
         "buttons": {
@@ -46,14 +47,15 @@
         try:
             device = hid.Device(VENDOR_ID, PRODUCT_ID)
         except:
             raise Exception("Device not found. Is it plugged in?")
         log.debug(f'Device manufacturer: {device.manufacturer}')
         log.debug(f'Product: {device.product}')
         self.device = device
+        self.connected = True
 
     # TODO(seanp): Why is reset not working?
     def reset(self):
         # wheel calibration
         self.device.write(bytes([0xf8, 0x0a, 0x00, 0x00, 0x00, 0x00, 0x00]))
         self.device.write(bytes([0xf8, 0x09, 0x05, 0x01, 0x01, 0x00, 0x00]))
         time.sleep(5) # wait for calibration
@@ -188,38 +190,47 @@
             raise ValueError("force_off slot must be between 0 and 4 or 0xf3")
         log.debug(f'force_off: {slot}')
         msg = [slot, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00]
         self.device.write(bytes(msg))
 
     # READ
 
-    def pump(self, timeout=10):
-        dat = self.device.read(16, timeout)
+    def read(self, timeout=10):
+        try:
+            dat = self.device.read(16, timeout)
+        except Exception as e:
+            print(f"G29 disconneted: {e}")
+            self.connected = False
+            self.stop_pumping()
+            return
 
         # only handle 12 byte msgs
         byte_array = bytearray(dat)
         if len(byte_array) >= 12:
             self.update_state(byte_array)
             self.cache = byte_array
             
         return dat
 
-    def start_pumping(self, timeout=10):
-        self.pump_thread = threading.Thread(target=self.pump_forever, args=(timeout,))
+    def listen(self, timeout=10):
+        self.pump_thread = threading.Thread(target=self.pump, args=(timeout,))
         self.pump_thread.start()
 
-    def pump_forever(self, timeout=10):
-        while 1:
-            self.pump(timeout)
+    def pump(self, timeout=10):
+        while self.connected:
+            time.sleep(0.01) # 100 hz
+            self.read(timeout)
     
     def stop_pumping(self):
-        if self.thread is not None:
+        if self.pump_thread is not None:
             self.pump_thread.join()
     
     def get_state(self):
+        if not self.connected:
+            raise Exception("G29 not connected")
         return self.state
     
     def update_state(self, byte_array):
         if self.cache is None:
             log.warn("cache not available")
             return
```

### Comparing `g29py-0.0.8/g29py/params.py` & `g29py-0.0.9/g29py/params.py`

 * *Files identical despite different names*

### Comparing `g29py-0.0.8/setup.py` & `g29py-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['hid==1.0.4']
 
 setup_kwargs = {
     'name': 'g29py',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'python driver for g29 wheel/pedals',
-    'long_description': '# g29py\n> python driver for logitech g29 wheel/pedals\n\n> :warning: **Warning**: g29py is alpha software. This repository is under heavy development and subject to breaking changes. :warning:\n\n![](etc/g29py.jpg)\n\n## Install\n```bash\npip install g29py\n```\n\n## Use\n\n```python\nfrom g29py import G29\ng29 = G29()\n```\n\n```python\n# write \ng29.set_range(500)\ng29.set_friction(0.5)\n```\n\n```python\n# read\ng29.start_pumping() # thread\nwhile 1:\n    state = g29.get_state()\n    print("steering:", state["steering"])\n    print("brake:", state["brake"])\n    print("accelerator", state["accelerator"])\n```\n\n## Read\n\n### Pedals/Steering\n\n| Pedal         | Value Range      | Neutral Position |\n|---------------|------------------|------------------|\n| `steering`    | Float: -1 to 1   | 0 (Centered)     |\n| `accelerator` | Float: -1 to 1   | -1 (Not pressed) |\n| `clutch`      | Float: -1 to 1   | -1 (Not pressed) |\n| `brake`       | Float: -1 to 1   | -1 (Not pressed) |\n\n### Buttons\n\n| Button  | Value |\n|---------|-------|\n| `up`    | 0/1   |\n| `down`  | 0/1   |\n| `left`  | 0/1   |\n| `right` | 0/1   |\n| `X`     | 0/1   |\n| `O`     | 0/1   |\n| `S`     | 0/1   |\n| `T`     | 0/1   |\n| `R2`    | 0/1   |\n| `R3`    | 0/1   |\n| `L2`    | 0/1   |\n| `L3`    | 0/1   |\n| `Share` | 0/1   |\n| `Options` | 0/1 |\n| `+`     | 0/1   |\n| `-`     | 0/1   |\n| `track` | -1/1  |\n| `back`  | 0/1   |\n| `PS`    | 0/1   |\n\n## Write\n\n| Method Name       | Default Parameters                         | Parameter Types                  |\n|-------------------|--------------------------------------------|----------------------------------|\n| `force_constant`  | `val=0.5`                                  | `val`: float                     |\n| `set_friction`    | `val=0.5`                                  | `val`: float                     |\n| `set_range`       | `val=400`                                  | `val`: int                       |\n| `set_autocenter`  | `strength=0.5, rate=0.05`                  | `strength`: float, `rate`: float |\n| `set_anticenter`  | `angle1=180, angle2=180, strength=0.5, reverse=0x0, force=0.5` | `angle1`: int, `angle2`: int, `strength`: float, `reverse`: hexadecimal, `force`: float |\n| `autocenter_off`  | None                                       | None                             |\n| `force_off`       | `slot=0xf3`                                | `slot`: hexadecimal              |\n\n## Sources\n\n- Commands based on nightmode\'s [logitech-g29](https://github.com/nightmode/logitech-g29) node.js driver.\n- Interface uses libhidapi ctype bindings from apmorton\'s [pyhidapi](https://github.com/apmorton/pyhidapi).\n- Reference [wiki-brew](https://wiibrew.org/wiki/Logitech_USB_steering_wheel) for effects API.\n\n## Support\n\nOnly Logitech G29 Driving Force Racing Wheels & Pedals kit supported on linux in ps3 mode.\n\nOn linux, remove sudo requirements by adding udev rule.\n\n```bash\necho \'KERNEL=="hidraw*", SUBSYSTEM=="hidraw", MODE="0664", GROUP="plugdev"\' \\\n    | sudo tee /etc/udev/rules.d/99-hidraw-permissions.rules\nsudo udevadm control --reload-rules\n```\n',
+    'long_description': '# g29py\n> python driver for logitech g29 wheel/pedals\n\n> :warning: **Warning**: g29py is alpha software. This repository is under heavy development and subject to breaking changes. :warning:\n\n![](etc/g29py.jpg)\n\n## Install\n```bash\npip install g29py\n```\n\n## Use\n\n```python\nfrom g29py import G29\ng29 = G29()\n```\n\n```python\n# write \ng29.set_range(500)\ng29.set_friction(0.5)\n```\n\n```python\n# read\ng29.listen() # thread\nwhile 1:\n    state = g29.get_state()\n    print("steering:", state["steering"])\n    print("brake:", state["brake"])\n    print("accelerator", state["accelerator"])\n```\n\n## Read\n\n### Pedals/Steering\n\n| Pedal         | Value Range      | Neutral Position |\n|---------------|------------------|------------------|\n| `steering`    | Float: -1 to 1   | 0 (Centered)     |\n| `accelerator` | Float: -1 to 1   | -1 (Not pressed) |\n| `clutch`      | Float: -1 to 1   | -1 (Not pressed) |\n| `brake`       | Float: -1 to 1   | -1 (Not pressed) |\n\n### Buttons\n\n| Button  | Value |\n|---------|-------|\n| `up`    | 0/1   |\n| `down`  | 0/1   |\n| `left`  | 0/1   |\n| `right` | 0/1   |\n| `X`     | 0/1   |\n| `O`     | 0/1   |\n| `S`     | 0/1   |\n| `T`     | 0/1   |\n| `R2`    | 0/1   |\n| `R3`    | 0/1   |\n| `L2`    | 0/1   |\n| `L3`    | 0/1   |\n| `Share` | 0/1   |\n| `Options` | 0/1 |\n| `+`     | 0/1   |\n| `-`     | 0/1   |\n| `track` | -1/1  |\n| `back`  | 0/1   |\n| `PS`    | 0/1   |\n\n## Write\n\n| Method Name       | Default Parameters                         | Parameter Types                  |\n|-------------------|--------------------------------------------|----------------------------------|\n| `force_constant`  | `val=0.5`                                  | `val`: float                     |\n| `set_friction`    | `val=0.5`                                  | `val`: float                     |\n| `set_range`       | `val=400`                                  | `val`: int                       |\n| `set_autocenter`  | `strength=0.5, rate=0.05`                  | `strength`: float, `rate`: float |\n| `set_anticenter`  | `angle1=180, angle2=180, strength=0.5, reverse=0x0, force=0.5` | `angle1`: int, `angle2`: int, `strength`: float, `reverse`: hexadecimal, `force`: float |\n| `autocenter_off`  | None                                       | None                             |\n| `force_off`       | `slot=0xf3`                                | `slot`: hexadecimal              |\n\n## Sources\n\n- Commands based on nightmode\'s [logitech-g29](https://github.com/nightmode/logitech-g29) node.js driver.\n- Interface uses libhidapi ctype bindings from apmorton\'s [pyhidapi](https://github.com/apmorton/pyhidapi).\n- Reference [wiki-brew](https://wiibrew.org/wiki/Logitech_USB_steering_wheel) for effects API.\n\n## Support\n\nOnly Logitech G29 Driving Force Racing Wheels & Pedals kit supported on linux in ps3 mode.\n\nOn linux, remove sudo requirements by adding udev rule.\n\n```bash\necho \'KERNEL=="hidraw*", SUBSYSTEM=="hidraw", MODE="0664", GROUP="plugdev"\' \\\n    | sudo tee /etc/udev/rules.d/99-hidraw-permissions.rules\nsudo udevadm control --reload-rules\n```\n',
     'author': 'sean pollock',
     'author_email': 'seanap@protonmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `g29py-0.0.8/PKG-INFO` & `g29py-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g29py
-Version: 0.0.8
+Version: 0.0.9
 Summary: python driver for g29 wheel/pedals
 Author: sean pollock
 Author-email: seanap@protonmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -36,15 +36,15 @@
 # write 
 g29.set_range(500)
 g29.set_friction(0.5)
 ```
 
 ```python
 # read
-g29.start_pumping() # thread
+g29.listen() # thread
 while 1:
     state = g29.get_state()
     print("steering:", state["steering"])
     print("brake:", state["brake"])
     print("accelerator", state["accelerator"])
 ```
```

