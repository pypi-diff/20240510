# Comparing `tmp/bme680-1.1.1.tar.gz` & `tmp/bme680-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bme680-1.1.1.tar", last modified: Tue May 11 10:16:46 2021, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `bme680-1.1.1.tar` & `bme680-2.0.0.tar`

### file list

```diff
@@ -1,17 +1,25 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2021-05-11 10:16:46.000000 bme680-1.1.1/
--rwxr-xr-x   0 pi        (1000) pi        (1000)     1388 2021-05-10 09:50:50.000000 bme680-1.1.1/setup.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2021-05-11 10:16:46.000000 bme680-1.1.1/bme680/
--rw-r--r--   0 pi        (1000) pi        (1000)    19993 2021-05-11 10:15:56.000000 bme680-1.1.1/bme680/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)    10792 2021-05-11 10:15:21.000000 bme680-1.1.1/bme680/constants.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1195 2021-05-11 10:16:46.000000 bme680-1.1.1/setup.cfg
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2021-05-11 10:16:46.000000 bme680-1.1.1/bme680.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)      254 2021-05-11 10:16:46.000000 bme680-1.1.1/bme680.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2021-05-11 10:16:46.000000 bme680-1.1.1/bme680.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        7 2021-05-11 10:16:46.000000 bme680-1.1.1/bme680.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        6 2021-05-11 10:16:46.000000 bme680-1.1.1/bme680.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)     4298 2021-05-11 10:16:46.000000 bme680-1.1.1/bme680.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      690 2021-05-11 10:15:44.000000 bme680-1.1.1/CHANGELOG.txt
--rw-r--r--   0 pi        (1000) pi        (1000)     1069 2021-05-10 08:15:02.000000 bme680-1.1.1/LICENSE.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      107 2021-05-10 09:50:50.000000 bme680-1.1.1/MANIFEST.in
--rw-r--r--   0 pi        (1000) pi        (1000)     4298 2021-05-11 10:16:46.000000 bme680-1.1.1/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)     2643 2021-05-11 10:16:44.000000 bme680-1.1.1/README.md
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 bme680-2.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 bme680-2.0.0/Makefile
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 bme680-2.0.0/README.md
+-rwxr-xr-x   0        0        0     2050 2020-02-02 00:00:00.000000 bme680-2.0.0/check.sh
+-rwxr-xr-x   0        0        0     9720 2020-02-02 00:00:00.000000 bme680-2.0.0/install.sh
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 bme680-2.0.0/requirements-dev.txt
+-rw-r--r--   0        0        0    64262 2020-02-02 00:00:00.000000 bme680-2.0.0/terminal.jpg
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 bme680-2.0.0/tox.ini
+-rwxr-xr-x   0        0        0     1283 2020-02-02 00:00:00.000000 bme680-2.0.0/uninstall.sh
+-rw-r--r--   0        0        0    19974 2020-02-02 00:00:00.000000 bme680-2.0.0/bme680/__init__.py
+-rw-r--r--   0        0        0    10792 2020-02-02 00:00:00.000000 bme680-2.0.0/bme680/constants.py
+-rwxr-xr-x   0        0        0     1690 2020-02-02 00:00:00.000000 bme680-2.0.0/examples/compensated-temperature.py
+-rwxr-xr-x   0        0        0     3320 2020-02-02 00:00:00.000000 bme680-2.0.0/examples/indoor-air-quality.py
+-rwxr-xr-x   0        0        0     1960 2020-02-02 00:00:00.000000 bme680-2.0.0/examples/read-all.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 bme680-2.0.0/examples/setup.cfg
+-rwxr-xr-x   0        0        0     1159 2020-02-02 00:00:00.000000 bme680-2.0.0/examples/temperature-offset.py
+-rwxr-xr-x   0        0        0     1007 2020-02-02 00:00:00.000000 bme680-2.0.0/examples/temperature-pressure-humidity.py
+-rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 bme680-2.0.0/tests/conftest.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 bme680-2.0.0/tests/setup.cfg
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 bme680-2.0.0/tests/test_compensation.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 bme680-2.0.0/tests/test_setup.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 bme680-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 bme680-2.0.0/LICENSE
+-rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 bme680-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5222 2020-02-02 00:00:00.000000 bme680-2.0.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `bme680-1.1.1/setup.py` & `bme680-2.0.0/LICENSE`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,21 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-"""
-Copyright (c) 2016 Pimoroni
+MIT License
 
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
-of the Software, and to permit persons to whom the Software is furnished to do
-so, subject to the following conditions:
+Copyright (c) 2018 Pimoroni Ltd
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
-"""
-
-from setuptools import setup, __version__
-from pkg_resources import parse_version
-
-minimum_version = parse_version('30.4.0')
-
-if parse_version(__version__) < minimum_version:
-    raise RuntimeError("Package setuptools must be at least version {}".format(minimum_version))
-
-setup()
```

### Comparing `bme680-1.1.1/bme680/__init__.py` & `bme680-2.0.0/bme680/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """BME680 Temperature, Pressure, Humidity & Gas Sensor."""
-from .constants import lookupTable1, lookupTable2
-from .constants import BME680Data
-from . import constants
 import math
 import time
 
-__version__ = '1.1.1'
+from . import constants
+from .constants import BME680Data, lookupTable1, lookupTable2
+
+__version__ = '2.0.0'
 
 
 # Export constants to global namespace
 # so end-users can "from BME680 import NAME"
 if hasattr(constants, '__dict__'):
     for key in constants.__dict__:
         value = constants.__dict__[key]
@@ -35,16 +35,16 @@
 
         """
         BME680Data.__init__(self)
 
         self.i2c_addr = i2c_addr
         self._i2c = i2c_device
         if self._i2c is None:
-            import smbus
-            self._i2c = smbus.SMBus(1)
+            import smbus2
+            self._i2c = smbus2.SMBus(1)
 
         try:
             self.chip_id = self._get_regs(constants.CHIP_ID_ADDR, 1)
             if self.chip_id != constants.CHIP_ID:
                 raise RuntimeError('BME680 Not Found. Invalid CHIP ID: 0x{0:02x}'.format(self.chip_id))
         except IOError:
             raise RuntimeError("Unable to identify BME680 at 0x{:02x} (IOError)".format(self.i2c_addr))
```

### Comparing `bme680-1.1.1/bme680/constants.py` & `bme680-2.0.0/bme680/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,24 +235,24 @@
                 255744255, 127110228, 64000000, 32258064,
                 16016016, 8000000, 4000000, 2000000,
                 1000000, 500000, 250000, 125000]
 
 
 def bytes_to_word(msb, lsb, bits=16, signed=False):
     """Convert a most and least significant byte into a word."""
-    # TODO: Reimpliment with struct
+    # TODO: Reimplement with struct
     word = (msb << 8) | lsb
     if signed:
         word = twos_comp(word, bits)
     return word
 
 
 def twos_comp(val, bits=16):
     """Convert two bytes into a two's compliment signed word."""
-    # TODO: Reimpliment with struct
+    # TODO: Reimplement with struct
     if val & (1 << (bits - 1)) != 0:
         val = val - (1 << bits)
     return val
 
 
 class FieldData:
     """Structure for storing BME680 sensor data."""
@@ -308,15 +308,15 @@
         self.res_heat_range = None
         # Variable to store heater resistance value
         self.res_heat_val = None
         # Variable to store error range
         self.range_sw_err = None
 
     def set_from_array(self, calibration):
-        """Set paramaters from an array of bytes."""
+        """Set parameters from an array of bytes."""
         # Temperature related coefficients
         self.par_t1 = bytes_to_word(calibration[T1_MSB_REG], calibration[T1_LSB_REG])
         self.par_t2 = bytes_to_word(calibration[T2_MSB_REG], calibration[T2_LSB_REG], bits=16, signed=True)
         self.par_t3 = twos_comp(calibration[T3_REG], bits=8)
 
         # Pressure related coefficients
         self.par_p1 = bytes_to_word(calibration[P1_MSB_REG], calibration[P1_LSB_REG])
```

### Comparing `bme680-1.1.1/CHANGELOG.txt` & `bme680-2.0.0/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+2.0.0
+-----
+
+* Repackage to hatch/pyproject.toml
+* Drop Python 2.7 support
+* Switch from smbu2 to smbus2
+
 1.1.1
 -----
 
 * New: constants to clarify heater on/off states
 
 1.1.0
 -----
```

### Comparing `bme680-1.1.1/README.md` & `bme680-2.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # BME680
 
-[![Build Status](https://travis-ci.org/pimoroni/bme680-python.svg?branch=master)](https://travis-ci.org/pimoroni/bme680-python)
-[![Coverage Status](https://coveralls.io/repos/github/pimoroni/bme680-python/badge.svg?branch=master)](https://coveralls.io/github/pimoroni/bme680-python?branch=master)
+[![Build Status](https://img.shields.io/github/actions/workflow/status/pimoroni/bme680-python/test.yml?branch=main)](https://github.com/pimoroni/bme680-python/actions/workflows/test.yml)
+[![Coverage Status](https://coveralls.io/repos/github/pimoroni/bme680-python/badge.svg?branch=main)](https://coveralls.io/github/pimoroni/bme680-python?branch=main)
 [![PyPi Package](https://img.shields.io/pypi/v/bme680.svg)](https://pypi.python.org/pypi/bme680)
 [![Python Versions](https://img.shields.io/pypi/pyversions/bme680.svg)](https://pypi.python.org/pypi/bme680)
 
 https://shop.pimoroni.com/products/bme680
 
 The state-of-the-art BME680 breakout lets you measure temperature, pressure, humidity, and indoor air quality.
 
@@ -18,84 +18,39 @@
 on your Raspberry Pi desktop, as illustrated below:
 
 ![Finding the terminal](http://get.pimoroni.com/resources/github-repo-terminal.png)
 
 In the new terminal window type the command exactly as it appears below (check for typos) and follow the on-screen instructions:
 
 ```bash
-curl https://get.pimoroni.com/bme680 | bash
+git clone https://github.com/pimoroni/bme680-python
+cd bme680-python
+./install.sh
 ```
 
-### Manual install:
+**Note** Libraries will be installed in the "pimoroni" virtual environment, you will need to activate it to run examples:
 
-#### Library install for Python 3:
-
-```bash
-sudo pip3 install bme680
 ```
-
-#### Library install for Python 2:
-
-```bash
-sudo pip2 install bme680
+source ~/.virtualenvs/pimoroni/bin/activate
 ```
 
 ### Development:
 
-If you want to contribute, or like living on the edge of your seat by having the latest code, you should clone this repository, `cd` to the library directory, and run:
+If you want to contribute, or like living on the edge of your seat by having the latest code, you can install the development version like so:
 
 ```bash
-sudo python3 setup.py install
+git clone https://github.com/pimoroni/bme680-python
+cd bme680-python
+./install.sh --unstable
 ```
-(or `sudo python setup.py install` whichever your primary Python environment may be)
 
-In all cases you will have to enable the i2c bus.
+In all cases you will have to enable the i2c bus:
+
+```
+sudo raspi-config nonint do_i2c 0
+```
 
 ## Documentation & Support
 
 * Guides and tutorials - https://learn.pimoroni.com/bme680-breakout
 * Get help - http://forums.pimoroni.com/c/support
 
-# Changelog
-1.1.1
------
-
-* New: constants to clarify heater on/off states
-
-1.1.0
------
-
-* New: support for BME688 "high" gas resistance variant
-* New: set/get gas heater disable bit
-* Enhancement: fail with descriptive RuntimeError when chip is not detected
-
-1.0.5
------
-
-* New: set_temp_offset to calibrate temperature offset in degrees C
-
-1.0.4
------
-
-* Fix to range_sw_err for extremely high gas readings
-* Convert to unsigned int to fix negative gas readings
-
-1.0.3
------
-
-* Merged temperature compensation fix from Bosch's BME680_driver 3.5.3
-
-1.0.2
------
-
-* Fixed set_gas_heater_temperature to avoid i2c TypeError
-
-1.0.1
------
-
-* Added Manifest to Python package
-
-1.0.0
------
-
-* Initial release
-
```

