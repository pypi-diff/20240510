# Comparing `tmp/pmw3901-0.1.0.tar.gz` & `tmp/pmw3901-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pmw3901-0.1.0.tar", last modified: Tue May  4 16:23:16 2021, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pmw3901-0.1.0.tar` & `pmw3901-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2021-05-04 16:23:16.000000 pmw3901-0.1.0/
--rwxr-xr-x   0 pi        (1000) pi        (1000)     2187 2021-05-04 13:54:16.000000 pmw3901-0.1.0/setup.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2021-05-04 16:23:16.000000 pmw3901-0.1.0/pmw3901.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)      251 2021-05-04 16:23:16.000000 pmw3901-0.1.0/pmw3901.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2021-05-04 16:23:16.000000 pmw3901-0.1.0/pmw3901.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        8 2021-05-04 16:23:16.000000 pmw3901-0.1.0/pmw3901.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        7 2021-05-04 16:23:16.000000 pmw3901-0.1.0/pmw3901.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)     2482 2021-05-04 16:23:16.000000 pmw3901-0.1.0/pmw3901.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      134 2021-05-04 16:23:16.000000 pmw3901-0.1.0/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      979 2021-04-30 13:45:59.000000 pmw3901-0.1.0/README.rst
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2021-05-04 16:23:16.000000 pmw3901-0.1.0/pmw3901/
--rw-r--r--   0 pi        (1000) pi        (1000)    14142 2021-05-04 13:48:45.000000 pmw3901-0.1.0/pmw3901/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)      106 2021-05-04 13:48:26.000000 pmw3901-0.1.0/CHANGELOG.txt
--rw-r--r--   0 pi        (1000) pi        (1000)     1070 2021-04-30 13:45:59.000000 pmw3901-0.1.0/LICENSE.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      108 2021-05-04 16:12:09.000000 pmw3901-0.1.0/MANIFEST.in
--rw-r--r--   0 pi        (1000) pi        (1000)     2482 2021-05-04 16:23:16.000000 pmw3901-0.1.0/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)     1315 2021-05-04 13:54:19.000000 pmw3901-0.1.0/README.md
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 pmw3901-1.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 pmw3901-1.0.0/MANIFEST.in
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 pmw3901-1.0.0/Makefile
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 pmw3901-1.0.0/README.md
+-rwxr-xr-x   0        0        0     2050 2020-02-02 00:00:00.000000 pmw3901-1.0.0/check.sh
+-rwxr-xr-x   0        0        0     9720 2020-02-02 00:00:00.000000 pmw3901-1.0.0/install.sh
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pmw3901-1.0.0/requirements-dev.txt
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 pmw3901-1.0.0/tox.ini
+-rwxr-xr-x   0        0        0     1283 2020-02-02 00:00:00.000000 pmw3901-1.0.0/uninstall.sh
+-rwxr-xr-x   0        0        0     1933 2020-02-02 00:00:00.000000 pmw3901-1.0.0/examples/frame_capture.py
+-rwxr-xr-x   0        0        0     1198 2020-02-02 00:00:00.000000 pmw3901-1.0.0/examples/motion.py
+-rw-r--r--   0        0        0    14970 2020-02-02 00:00:00.000000 pmw3901-1.0.0/pmw3901/__init__.py
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 pmw3901-1.0.0/tests/conftest.py
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 pmw3901-1.0.0/tests/test_features.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 pmw3901-1.0.0/tests/test_paa5100.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 pmw3901-1.0.0/tests/test_pmw3901.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pmw3901-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pmw3901-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 pmw3901-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 pmw3901-1.0.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pmw3901-0.1.0/pmw3901.egg-info/PKG-INFO` & `pmw3901-1.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,103 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pmw3901
-Version: 0.1.0
+Version: 1.0.0
 Summary: Python library for the PMW3901 optical flow sensor
-Home-page: http://www.pimoroni.com
-Author: Philip Howard
-Author-email: phil@pimoroni.com
-License: MIT
 Project-URL: GitHub, https://www.github.com/pimoroni/pmw3901-python
-Description: # PMW3901 / PAA5100JE 2-Dimensional Optical Flow Sensor
-        
-        [![Build Status](https://travis-ci.com/pimoroni/pmw3901-python.svg?branch=master)](https://travis-ci.com/pimoroni/pmw3901-python)
-        [![Coverage Status](https://coveralls.io/repos/github/pimoroni/pmw3901-python/badge.svg?branch=master)](https://coveralls.io/github/pimoroni/pmw3901-python?branch=master)
-        [![PyPi Package](https://img.shields.io/pypi/v/pmw3901.svg)](https://pypi.python.org/pypi/pmw3901)
-        [![Python Versions](https://img.shields.io/pypi/pyversions/pmw3901.svg)](https://pypi.python.org/pypi/pmw3901)
-        
-        
-        # Installing
-        
-        Stable library from PyPi:
-        
-        * Just run `sudo pip install pmw3901`
-        
-        Latest/development library from GitHub:
-        
-        * `git clone https://github.com/pimoroni/pmw3901-python`
-        * `cd pmw3901-python`
-        * `sudo ./install.sh`
-        
-        # Usage
-        
-        The PAA5100JE has a slightly different init routine to the PMW3901, you should use the class provided to ensure it's set up correctly:
-        
-        ```
-        from pmw3901 import PAA5100
-        ```
-        
-        And for the PMW3901, continue using the old class:
-        
-        ```
-        from pmw3901 import PMW3901
-        ```
-        
-        The example `motion.py` demonstrates setting up either sensor, and accepts a `--board` argument to specify which you'd like to use.
-        
-        # Changelog
-        0.1.0
-        -----
-        
-        * Add init support for PAA5100JE
-        * Add frame capture support
-        
-        0.0.1
-        -----
-        
-        * Initial Release
-        
-Keywords: Raspberry Pi
-Platform: UNKNOWN
+Project-URL: Homepage, https://www.pimoroni.com
+Author-email: Philip Howard <phil@pimoroni.com>
+Maintainer-email: Philip Howard <phil@pimoroni.com>
+License: MIT License
+        
+        Copyright (c) 2018 Pimoroni Ltd.
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+License-File: LICENSE
+Keywords: Pi,Raspberry
 Classifier: Development Status :: 4 - Beta
-Classifier: Operating System :: POSIX :: Linux
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 2.7
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Hardware
+Requires-Python: >=3.7
+Requires-Dist: spidev
 Description-Content-Type: text/markdown
+
+# PMW3901 / PAA5100JE 2-Dimensional Optical Flow Sensor
+
+[![Build Status](https://img.shields.io/github/actions/workflow/status/pimoroni/pmw3901-python/test.yml?branch=main)](https://github.com/pimoroni/pmw3901-python/actions/workflows/test.yml)
+[![Coverage Status](https://coveralls.io/repos/github/pimoroni/pmw3901-python/badge.svg?branch=main)](https://coveralls.io/github/pimoroni/pmw3901-python?branch=main)
+[![PyPi Package](https://img.shields.io/pypi/v/pmw3901.svg)](https://pypi.python.org/pypi/pmw3901)
+[![Python Versions](https://img.shields.io/pypi/pyversions/pmw3901.svg)](https://pypi.python.org/pypi/pmw3901)
+
+
+# Installing
+
+Stable library from PyPi:
+
+* Just run `python3 -m pip install pmw3901`
+
+Latest/development library from GitHub:
+
+* `git clone https://github.com/pimoroni/pmw3901-python`
+* `cd pmw3901-python`
+* `./install.sh`
+
+# Usage
+
+The PAA5100JE has a slightly different init routine to the PMW3901, you should use the class provided to ensure it's set up correctly:
+
+```
+from pmw3901 import PAA5100
+```
+
+And for the PMW3901, continue using the old class:
+
+```
+from pmw3901 import PMW3901
+```
+
+The example `motion.py` demonstrates setting up either sensor, and accepts a `--board` argument to specify which you'd like to use.
+
+1.0.0
+-----
+
+* Port to gpiod/gpiodevice
+* Repackage to hatch/pyproject.toml
+* BREAKING: spi_cs_gpio will not auto-detect SPI CS line, use spi_cs=(0, 1)
+* BREAKING: Constants `BG_CS_FRONT_BCM` and `BG_CS_BACK_BCM` are now CS lines, not pins
+
+0.1.0
+-----
+
+* Add init support for PAA5100JE
+* Add frame capture support
+
+0.0.1
+-----
+
+* Initial Release
```

### Comparing `pmw3901-0.1.0/pmw3901/__init__.py` & `pmw3901-1.0.0/pmw3901/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,78 @@
-import time
 import struct
+import time
+
+import gpiod
+import gpiodevice
 import spidev
-import RPi.GPIO as GPIO
+from gpiod.line import Direction, Value
 
-__version__ = '0.1.0'
+__version__ = "1.0.0"
 
 WAIT = -1
 
-BG_CS_FRONT_BCM = 7
-BG_CS_BACK_BCM = 8
+BG_CS_FRONT_BCM = 1  # GPIO 8
+BG_CS_BACK_BCM = 0   # GPIO 7
 
 REG_ID = 0x00
 REG_DATA_READY = 0x02
 REG_MOTION_BURST = 0x16
-REG_POWER_UP_RESET = 0x3a
-REG_ORIENTATION = 0x5b
-REG_RESOLUTION = 0x4e  # PAA5100 only
+REG_POWER_UP_RESET = 0x3A
+REG_ORIENTATION = 0x5B
+REG_RESOLUTION = 0x4E  # PAA5100 only
 
 REG_RAWDATA_GRAB = 0x58
 REG_RAWDATA_GRAB_STATUS = 0x59
 
+OUTL = gpiod.LineSettings(direction=Direction.OUTPUT, output_value=Value.INACTIVE)
 
-class PMW3901():
-    def __init__(self, spi_port=0, spi_cs=1, spi_cs_gpio=BG_CS_FRONT_BCM):
-        self.spi_cs_gpio = spi_cs_gpio
+
+class PMW3901:
+    _device_name = "PMW3901"
+
+    def __init__(self, spi_port=0, spi_cs=1, spi_cs_gpio=None):
         self.spi_dev = spidev.SpiDev()
+        self._spi_cs_gpio = None
+
+        if spi_cs_gpio is not None:
+            spi_cs = 0
+            self._spi_cs_gpio = gpiodevice.get_pin(spi_cs_gpio, f"{self._device_name}_cs", OUTL)
+
         self.spi_dev.open(spi_port, spi_cs)
         self.spi_dev.max_speed_hz = 400000
-        self.spi_dev.no_cs = True
-
-        GPIO.setwarnings(False)
-        GPIO.setmode(GPIO.BCM)
-        GPIO.setup(self.spi_cs_gpio, GPIO.OUT)
 
-        GPIO.output(self.spi_cs_gpio, 0)
-        time.sleep(0.05)
-        GPIO.output(self.spi_cs_gpio, 1)
+        if spi_cs_gpio is not None:
+            try:
+                # TODO: Not sure this does anything but break with an OSError?
+                self.spi_dev.no_cs = True
+            except OSError:
+                pass
+
+        if self._spi_cs_gpio:
+            self.set_pin(self._spi_cs_gpio, 0)
+            time.sleep(0.05)
+            self.set_pin(self._spi_cs_gpio, 1)
 
-        self._write(REG_POWER_UP_RESET, 0x5a)
+        self._write(REG_POWER_UP_RESET, 0x5A)
         time.sleep(0.02)
         for offset in range(5):
             self._read(REG_DATA_READY + offset)
 
         self._secret_sauce()
 
         product_id, revision = self.get_id()
-        if product_id != 0x49 or revision != 0x00:
-            raise RuntimeError("Invalid Product ID or Revision for PMW3901: 0x{:02x}/0x{:02x}".format(product_id, revision))
+        if product_id != 0x49 or revision not in (0x00, 0x01):
+            raise RuntimeError(f"Invalid Product ID or Revision for PMW3901: 0x{product_id:02x}/0x{revision:02x}")
         # print("Product ID: {}".format(ID.get_product_id()))
         # print("Revision: {}".format(ID.get_revision_id()))
 
+    def set_pin(self, pin, state):
+        lines, offset = pin
+        lines.set_value(offset, Value.ACTIVE if state else Value.INACTIVE)
+
     def get_id(self):
         """Get chip ID and revision from PMW3901."""
         return self._read(REG_ID, 2)
 
     def set_rotation(self, degrees=0):
         """Set orientation of PMW3901 in increments of 90 degrees.
 
@@ -100,24 +119,26 @@
         and magnitude.
 
         :param timeout: Timeout in seconds
 
         """
         t_start = time.time()
         while time.time() - t_start < timeout:
-            GPIO.output(self.spi_cs_gpio, 0)
+            if self._spi_cs_gpio:
+                self.set_pin(self._spi_cs_gpio, 0)
             data = self.spi_dev.xfer2([REG_MOTION_BURST] + [0 for x in range(12)])
-            GPIO.output(self.spi_cs_gpio, 1)
+            if self._spi_cs_gpio:
+                self.set_pin(self._spi_cs_gpio, 1)
             (_, dr, obs,
              x, y, quality,
              raw_sum, raw_max, raw_min,
              shutter_upper,
              shutter_lower) = struct.unpack("<BBBhhBBBBBB", bytearray(data))
 
-            if dr & 0b10000000 and not (quality < 0x19 and shutter_upper == 0x1f):
+            if dr & 0b10000000 and not (quality < 0x19 and shutter_upper == 0x1F):
                 return x, y
 
             time.sleep(0.01)
 
         raise RuntimeError("Timed out waiting for motion data.")
 
     def get_motion_slow(self, timeout=5):
@@ -136,34 +157,38 @@
             if dr & 0b10000000:
                 return x, y
             time.sleep(0.001)
 
         raise RuntimeError("Timed out waiting for motion data.")
 
     def _write(self, register, value):
-        GPIO.output(self.spi_cs_gpio, 0)
+        if self._spi_cs_gpio:
+                self.set_pin(self._spi_cs_gpio, 0)
         self.spi_dev.xfer2([register | 0x80, value])
-        GPIO.output(self.spi_cs_gpio, 1)
+        if self._spi_cs_gpio:
+                self.set_pin(self._spi_cs_gpio, 1)
 
     def _read(self, register, length=1):
         result = []
         for x in range(length):
-            GPIO.output(self.spi_cs_gpio, 0)
+            if self._spi_cs_gpio:
+                self.set_pin(self._spi_cs_gpio, 0)
             value = self.spi_dev.xfer2([register + x, 0])
-            GPIO.output(self.spi_cs_gpio, 1)
+            if self._spi_cs_gpio:
+                self.set_pin(self._spi_cs_gpio, 1)
             result.append(value[1])
 
         if length == 1:
             return result[0]
         else:
             return result
 
     def _bulk_write(self, data):
         for x in range(0, len(data), 2):
-            register, value = data[x:x + 2]
+            register, value = data[x : x + 2]
             if register == WAIT:
                 # print("Sleeping for: {:02d}ms".format(value))
                 time.sleep(value / 1000)
             else:
                 # print("Writing: {:02x} to {:02x}".format(register, value))
                 self._write(register, value)
 
@@ -172,161 +197,161 @@
 
         Don't ask what these do, the datasheet refuses to explain.
 
         They are some proprietary calibration magic.
 
         """
         self._bulk_write([
-            0x7f, 0x00,
+            0x7F, 0x00,
             0x55, 0x01,
             0x50, 0x07,
 
-            0x7f, 0x0e,
+            0x7F, 0x0E,
             0x43, 0x10
         ])
         if self._read(0x67) & 0b10000000:
             self._write(0x48, 0x04)
         else:
             self._write(0x48, 0x02)
         self._bulk_write([
-            0x7f, 0x00,
-            0x51, 0x7b,
+            0x7F, 0x00,
+            0x51, 0x7B,
 
             0x50, 0x00,
             0x55, 0x00,
-            0x7f, 0x0E
+            0x7F, 0x0E
         ])
         if self._read(0x73) == 0x00:
             c1 = self._read(0x70)
             c2 = self._read(0x71)
             if c1 <= 28:
                 c1 += 14
             if c1 > 28:
                 c1 += 11
             c1 = max(0, min(0x3F, c1))
             c2 = (c2 * 45) // 100
             self._bulk_write([
-                0x7f, 0x00,
-                0x61, 0xad,
+                0x7F, 0x00,
+                0x61, 0xAD,
                 0x51, 0x70,
-                0x7f, 0x0e
+                0x7F, 0x0E
             ])
             self._write(0x70, c1)
             self._write(0x71, c2)
         self._bulk_write([
-            0x7f, 0x00,
-            0x61, 0xad,
-            0x7f, 0x03,
+            0x7F, 0x00,
+            0x61, 0xAD,
+            0x7F, 0x03,
             0x40, 0x00,
-            0x7f, 0x05,
+            0x7F, 0x05,
 
-            0x41, 0xb3,
-            0x43, 0xf1,
+            0x41, 0xB3,
+            0x43, 0xF1,
             0x45, 0x14,
-            0x5b, 0x32,
-            0x5f, 0x34,
-            0x7b, 0x08,
-            0x7f, 0x06,
-            0x44, 0x1b,
-            0x40, 0xbf,
-            0x4e, 0x3f,
-            0x7f, 0x08,
+            0x5B, 0x32,
+            0x5F, 0x34,
+            0x7B, 0x08,
+            0x7F, 0x06,
+            0x44, 0x1B,
+            0x40, 0xBF,
+            0x4E, 0x3F,
+            0x7F, 0x08,
             0x65, 0x20,
-            0x6a, 0x18,
+            0x6A, 0x18,
 
-            0x7f, 0x09,
-            0x4f, 0xaf,
-            0x5f, 0x40,
+            0x7F, 0x09,
+            0x4F, 0xAF,
+            0x5F, 0x40,
             0x48, 0x80,
             0x49, 0x80,
 
             0x57, 0x77,
             0x60, 0x78,
             0x61, 0x78,
             0x62, 0x08,
             0x63, 0x50,
-            0x7f, 0x0a,
+            0x7F, 0x0A,
             0x45, 0x60,
-            0x7f, 0x00,
-            0x4d, 0x11,
+            0x7F, 0x00,
+            0x4D, 0x11,
 
             0x55, 0x80,
             0x74, 0x21,
-            0x75, 0x1f,
-            0x4a, 0x78,
-            0x4b, 0x78,
+            0x75, 0x1F,
+            0x4A, 0x78,
+            0x4B, 0x78,
 
             0x44, 0x08,
             0x45, 0x50,
-            0x64, 0xff,
-            0x65, 0x1f,
-            0x7f, 0x14,
+            0x64, 0xFF,
+            0x65, 0x1F,
+            0x7F, 0x14,
             0x65, 0x67,
             0x66, 0x08,
             0x63, 0x70,
-            0x7f, 0x15,
+            0x7F, 0x15,
             0x48, 0x48,
-            0x7f, 0x07,
-            0x41, 0x0d,
+            0x7F, 0x07,
+            0x41, 0x0D,
             0x43, 0x14,
 
-            0x4b, 0x0e,
-            0x45, 0x0f,
+            0x4B, 0x0E,
+            0x45, 0x0F,
             0x44, 0x42,
-            0x4c, 0x80,
-            0x7f, 0x10,
+            0x4C, 0x80,
+            0x7F, 0x10,
 
-            0x5b, 0x02,
-            0x7f, 0x07,
+            0x5B, 0x02,
+            0x7F, 0x07,
             0x40, 0x41,
             0x70, 0x00,
             WAIT, 0x0A,  # Sleep for 10ms
 
             0x32, 0x44,
-            0x7f, 0x07,
+            0x7F, 0x07,
             0x40, 0x40,
-            0x7f, 0x06,
-            0x62, 0xf0,
+            0x7F, 0x06,
+            0x62, 0xF0,
             0x63, 0x00,
-            0x7f, 0x0d,
-            0x48, 0xc0,
-            0x6f, 0xd5,
-            0x7f, 0x00,
-
-            0x5b, 0xa0,
-            0x4e, 0xa8,
-            0x5a, 0x50,
+            0x7F, 0x0D,
+            0x48, 0xC0,
+            0x6F, 0xD5,
+            0x7F, 0x00,
+
+            0x5B, 0xA0,
+            0x4E, 0xA8,
+            0x5A, 0x50,
             0x40, 0x80,
             WAIT, 0xF0,
 
-            0x7f, 0x14,  # Enable LED_N pulsing
-            0x6f, 0x1c,
-            0x7f, 0x00
+            0x7F, 0x14,  # Enable LED_N pulsing
+            0x6F, 0x1C,
+            0x7F, 0x00
         ])
 
     def frame_capture(self, timeout=10.0):
         """Capture a raw data frame.
 
         Warning: This is *very* slow and of limited usefulness.
 
         """
         self._bulk_write([
-            0x7f, 0x07,
-            0x4c, 0x00,
-            0x7f, 0x08,
-            0x6a, 0x38,
-            0x7f, 0x00,
+            0x7F, 0x07,
+            0x4C, 0x00,
+            0x7F, 0x08,
+            0x6A, 0x38,
+            0x7F, 0x00,
             0x55, 0x04,
             0x40, 0x80,
-            0x4d, 0x11,
+            0x4D, 0x11,
 
-            WAIT, 0x0a,
+            WAIT, 0x0A,
 
-            0x7f, 0x00,
-            0x58, 0xff
+            0x7F, 0x00,
+            0x58, 0xFF
         ])
 
         t_start = time.time()
 
         while True:
             status = self._read(REG_RAWDATA_GRAB_STATUS)
             if status & 0b11000000:
@@ -351,194 +376,196 @@
             if data & 0b11000000 == 0b10000000:  # Lower 2-bits
                 raw_data[x] &= ~0b00000011
                 raw_data[x] |= (data & 0b00001100) >> 2   # Held in 3:2
                 x += 1
             if x == RAW_DATA_LEN:
                 return raw_data
             if time.time() - t_start > timeout:
-                raise RuntimeError("Raw data capture timeout, got {} values".format(x))
+                raise RuntimeError(f"Raw data capture timeout, got {x} values")
 
         return None
 
 
 class PAA5100(PMW3901):
+    _device_name = "PAA5100"
+
     def _secret_sauce(self):
         """Write the secret sauce registers for the PAA5100.
 
         Don't ask what these do, we'd have to make you walk the plank.
 
         These are some proprietary calibration magic.
 
         I hate this as much as you do, dear reader.
 
         """
         self._bulk_write([
-            0x7f, 0x00,
+            0x7F, 0x00,
             0x55, 0x01,
             0x50, 0x07,
 
-            0x7f, 0x0e,
+            0x7F, 0x0E,
             0x43, 0x10
         ])
         if self._read(0x67) & 0b10000000:
             self._write(0x48, 0x04)
         else:
             self._write(0x48, 0x02)
         self._bulk_write([
-            0x7f, 0x00,
-            0x51, 0x7b,
+            0x7F, 0x00,
+            0x51, 0x7B,
             0x50, 0x00,
             0x55, 0x00,
-            0x7f, 0x0e
+            0x7F, 0x0E
         ])
         if self._read(0x73) == 0x00:
             c1 = self._read(0x70)
             c2 = self._read(0x71)
             if c1 <= 28:
                 c1 += 14
             if c1 > 28:
                 c1 += 11
             c1 = max(0, min(0x3F, c1))
             c2 = (c2 * 45) // 100
             self._bulk_write([
-                0x7f, 0x00,
-                0x61, 0xad,
+                0x7F, 0x00,
+                0x61, 0xAD,
                 0x51, 0x70,
-                0x7f, 0x0e
+                0x7F, 0x0E
             ])
             self._write(0x70, c1)
             self._write(0x71, c2)
         self._bulk_write([
-            0x7f, 0x00,
-            0x61, 0xad,
+            0x7F, 0x00,
+            0x61, 0xAD,
 
-            0x7f, 0x03,
+            0x7F, 0x03,
             0x40, 0x00,
 
-            0x7f, 0x05,
-            0x41, 0xb3,
-            0x43, 0xf1,
+            0x7F, 0x05,
+            0x41, 0xB3,
+            0x43, 0xF1,
             0x45, 0x14,
 
-            0x5f, 0x34,
-            0x7b, 0x08,
-            0x5e, 0x34,
-            0x5b, 0x11,
-            0x6d, 0x11,
+            0x5F, 0x34,
+            0x7B, 0x08,
+            0x5E, 0x34,
+            0x5B, 0x11,
+            0x6D, 0x11,
             0x45, 0x17,
-            0x70, 0xe5,
-            0x71, 0xe5,
+            0x70, 0xE5,
+            0x71, 0xE5,
 
-            0x7f, 0x06,
-            0x44, 0x1b,
-            0x40, 0xbf,
-            0x4e, 0x3f,
+            0x7F, 0x06,
+            0x44, 0x1B,
+            0x40, 0xBF,
+            0x4E, 0x3F,
 
-            0x7f, 0x08,
+            0x7F, 0x08,
             0x66, 0x44,
             0x65, 0x20,
-            0x6a, 0x3a,
+            0x6A, 0x3A,
             0x61, 0x05,
             0x62, 0x05,
 
-            0x7f, 0x09,
-            0x4f, 0xaf,
-            0x5f, 0x40,
+            0x7F, 0x09,
+            0x4F, 0xAF,
+            0x5F, 0x40,
             0x48, 0x80,
             0x49, 0x80,
             0x57, 0x77,
             0x60, 0x78,
             0x61, 0x78,
             0x62, 0x08,
             0x63, 0x50,
 
-            0x7f, 0x0a,
+            0x7F, 0x0A,
             0x45, 0x60,
 
-            0x7f, 0x00,
-            0x4d, 0x11,
+            0x7F, 0x00,
+            0x4D, 0x11,
             0x55, 0x80,
             0x74, 0x21,
-            0x75, 0x1f,
-            0x4a, 0x78,
-            0x4b, 0x78,
+            0x75, 0x1F,
+            0x4A, 0x78,
+            0x4B, 0x78,
             0x44, 0x08,
 
             0x45, 0x50,
-            0x64, 0xff,
-            0x65, 0x1f,
+            0x64, 0xFF,
+            0x65, 0x1F,
 
-            0x7f, 0x14,
+            0x7F, 0x14,
             0x65, 0x67,
             0x66, 0x08,
             0x63, 0x70,
-            0x6f, 0x1c,
+            0x6F, 0x1C,
 
-            0x7f, 0x15,
+            0x7F, 0x15,
             0x48, 0x48,
 
-            0x7f, 0x07,
-            0x41, 0x0d,
+            0x7F, 0x07,
+            0x41, 0x0D,
             0x43, 0x14,
-            0x4b, 0x0e,
-            0x45, 0x0f,
+            0x4B, 0x0E,
+            0x45, 0x0F,
             0x44, 0x42,
-            0x4c, 0x80,
+            0x4C, 0x80,
 
-            0x7f, 0x10,
-            0x5b, 0x02,
+            0x7F, 0x10,
+            0x5B, 0x02,
 
-            0x7f, 0x07,
+            0x7F, 0x07,
             0x40, 0x41,
 
-            WAIT, 0x0a,  # Wait 10ms
+            WAIT, 0x0A,  # Wait 10ms
 
-            0x7f, 0x00,
+            0x7F, 0x00,
             0x32, 0x00,
 
-            0x7f, 0x07,
+            0x7F, 0x07,
             0x40, 0x40,
 
-            0x7f, 0x06,
-            0x68, 0xf0,
+            0x7F, 0x06,
+            0x68, 0xF0,
             0x69, 0x00,
 
-            0x7f, 0x0d,
-            0x48, 0xc0,
-            0x6f, 0xd5,
-
-            0x7f, 0x00,
-            0x5b, 0xa0,
-            0x4e, 0xa8,
-            0x5a, 0x90,
+            0x7F, 0x0D,
+            0x48, 0xC0,
+            0x6F, 0xD5,
+
+            0x7F, 0x00,
+            0x5B, 0xA0,
+            0x4E, 0xA8,
+            0x5A, 0x90,
             0x40, 0x80,
-            0x73, 0x1f,
+            0x73, 0x1F,
 
-            WAIT, 0x0a,  # Wait 10ms
+            WAIT, 0x0A,  # Wait 10ms
 
             0x73, 0x00
         ])
 
 
 if __name__ == "__main__":
     import argparse
     parser = argparse.ArgumentParser()
-    parser.add_argument('--rotation', type=int,
+    parser.add_argument("--rotation", type=int,
                         default=0, choices=[0, 90, 180, 270],
-                        help='Rotation of sensor in degrees.', )
+                        help="Rotation of sensor in degrees.", )
     args = parser.parse_args()
-    flo = PMW3901(spi_port=0, spi_cs=1, spi_cs_gpio=BG_CS_FRONT_BCM)
+    flo = PMW3901(spi_port=0, spi_cs_gpio=BG_CS_FRONT_BCM)
     flo.set_rotation(args.rotation)
     tx = 0
     ty = 0
     try:
         while True:
             try:
                 x, y = flo.get_motion()
             except RuntimeError:
                 continue
             tx += x
             ty += y
-            print("Motion: {:03d} {:03d} x: {:03d} y {:03d}".format(x, y, tx, ty))
+            print(f"Motion: {x:03d} {y:03d} x: {tx:03d} y {ty:03d}")
             time.sleep(0.01)
     except KeyboardInterrupt:
         pass
```

### Comparing `pmw3901-0.1.0/LICENSE.txt` & `pmw3901-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pmw3901-0.1.0/README.md` & `pmw3901-1.0.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # PMW3901 / PAA5100JE 2-Dimensional Optical Flow Sensor
 
-[![Build Status](https://travis-ci.com/pimoroni/pmw3901-python.svg?branch=master)](https://travis-ci.com/pimoroni/pmw3901-python)
-[![Coverage Status](https://coveralls.io/repos/github/pimoroni/pmw3901-python/badge.svg?branch=master)](https://coveralls.io/github/pimoroni/pmw3901-python?branch=master)
+[![Build Status](https://img.shields.io/github/actions/workflow/status/pimoroni/pmw3901-python/test.yml?branch=main)](https://github.com/pimoroni/pmw3901-python/actions/workflows/test.yml)
+[![Coverage Status](https://coveralls.io/repos/github/pimoroni/pmw3901-python/badge.svg?branch=main)](https://coveralls.io/github/pimoroni/pmw3901-python?branch=main)
 [![PyPi Package](https://img.shields.io/pypi/v/pmw3901.svg)](https://pypi.python.org/pypi/pmw3901)
 [![Python Versions](https://img.shields.io/pypi/pyversions/pmw3901.svg)](https://pypi.python.org/pypi/pmw3901)
 
 
 # Installing
 
 Stable library from PyPi:
 
-* Just run `sudo pip install pmw3901`
+* Just run `python3 -m pip install pmw3901`
 
 Latest/development library from GitHub:
 
 * `git clone https://github.com/pimoroni/pmw3901-python`
 * `cd pmw3901-python`
-* `sudo ./install.sh`
+* `./install.sh`
 
 # Usage
 
 The PAA5100JE has a slightly different init routine to the PMW3901, you should use the class provided to ensure it's set up correctly:
 
 ```
 from pmw3901 import PAA5100
@@ -29,19 +29,7 @@
 And for the PMW3901, continue using the old class:
 
 ```
 from pmw3901 import PMW3901
 ```
 
 The example `motion.py` demonstrates setting up either sensor, and accepts a `--board` argument to specify which you'd like to use.
-
-# Changelog
-0.1.0
------
-
-* Add init support for PAA5100JE
-* Add frame capture support
-
-0.0.1
------
-
-* Initial Release
```

