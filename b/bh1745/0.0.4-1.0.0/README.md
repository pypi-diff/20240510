# Comparing `tmp/bh1745-0.0.4.tar.gz` & `tmp/bh1745-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bh1745-0.0.4.tar", last modified: Fri Sep 13 12:41:59 2019, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `bh1745-0.0.4.tar` & `bh1745-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,23 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2019-09-13 12:41:59.000000 bh1745-0.0.4/
--rw-r--r--   0 pi        (1000) pi        (1000)     1825 2019-09-13 12:41:59.000000 bh1745-0.0.4/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      108 2019-09-13 12:02:51.000000 bh1745-0.0.4/MANIFEST.in
--rw-r--r--   0 pi        (1000) pi        (1000)      451 2019-09-13 12:02:51.000000 bh1745-0.0.4/README.rst
--rw-r--r--   0 pi        (1000) pi        (1000)      290 2019-09-13 12:03:15.000000 bh1745-0.0.4/CHANGELOG.txt
--rw-r--r--   0 pi        (1000) pi        (1000)     1070 2019-09-13 12:02:51.000000 bh1745-0.0.4/LICENSE.txt
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2019-09-13 12:41:59.000000 bh1745-0.0.4/bh1745.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)        7 2019-09-13 12:41:58.000000 bh1745-0.0.4/bh1745.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)     1825 2019-09-13 12:41:58.000000 bh1745-0.0.4/bh1745.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2019-09-13 12:41:58.000000 bh1745-0.0.4/bh1745.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       17 2019-09-13 12:41:58.000000 bh1745-0.0.4/bh1745.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      235 2019-09-13 12:41:58.000000 bh1745-0.0.4/bh1745.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      165 2019-09-13 12:41:59.000000 bh1745-0.0.4/setup.cfg
--rwxr-xr-x   0 pi        (1000) pi        (1000)     2188 2019-09-13 12:03:15.000000 bh1745-0.0.4/setup.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2019-09-13 12:41:59.000000 bh1745-0.0.4/bh1745/
--rw-r--r--   0 pi        (1000) pi        (1000)    10147 2019-09-13 12:03:15.000000 bh1745-0.0.4/bh1745/__init__.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 bh1745-1.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 bh1745-1.0.0/Makefile
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 bh1745-1.0.0/README.md
+-rwxr-xr-x   0        0        0     2050 2020-02-02 00:00:00.000000 bh1745-1.0.0/check.sh
+-rwxr-xr-x   0        0        0     9720 2020-02-02 00:00:00.000000 bh1745-1.0.0/install.sh
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 bh1745-1.0.0/requirements-dev.txt
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 bh1745-1.0.0/tox.ini
+-rwxr-xr-x   0        0        0     1283 2020-02-02 00:00:00.000000 bh1745-1.0.0/uninstall.sh
+-rw-r--r--   0        0        0    10146 2020-02-02 00:00:00.000000 bh1745-1.0.0/bh1745/__init__.py
+-rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 bh1745-1.0.0/documentation/REFERENCE.md
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 bh1745-1.0.0/examples/README.md
+-rwxr-xr-x   0        0        0      320 2020-02-02 00:00:00.000000 bh1745-1.0.0/examples/detect.py
+-rwxr-xr-x   0        0        0      374 2020-02-02 00:00:00.000000 bh1745-1.0.0/examples/hex-colour.py
+-rwxr-xr-x   0        0        0      398 2020-02-02 00:00:00.000000 bh1745-1.0.0/examples/raw-colour.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 bh1745-1.0.0/examples/setup.cfg
+-rwxr-xr-x   0        0        0      553 2020-02-02 00:00:00.000000 bh1745-1.0.0/examples/two-sensors.py
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 bh1745-1.0.0/tests/test_features.py
+-rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 bh1745-1.0.0/tests/test_setup.py
+-rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 bh1745-1.0.0/tests/tools.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 bh1745-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 bh1745-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 bh1745-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4767 2020-02-02 00:00:00.000000 bh1745-1.0.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `bh1745-0.0.4/LICENSE.txt` & `bh1745-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bh1745-0.0.4/bh1745/__init__.py` & `bh1745-1.0.0/bh1745/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Library for the BH1745 colour sensor."""
 import time
 
-from i2cdevice import Device, Register, BitField
+from i2cdevice import BitField, Device, Register
 from i2cdevice.adapter import LookupAdapter, U16ByteSwapAdapter
 
-
-__version__ = '0.0.4'
+__version__ = "1.0.0"
 
 I2C_ADDRESSES = [0x38, 0x39]
 BH1745_RESET_TIMEOUT_SEC = 2
 
 
 class BH1745TimeoutError(Exception):  # noqa D101
     pass
@@ -27,102 +26,102 @@
         """
         self._i2c_addr = i2c_addr
         self._i2c_dev = i2c_dev
         self._is_setup = False
         # Device definition
         self._bh1745 = Device(I2C_ADDRESSES, i2c_dev=self._i2c_dev, bit_width=8, registers=(
             # Part ID should be 0b001011 or 0x0B
-            Register('SYSTEM_CONTROL', 0x40, fields=(
-                BitField('sw_reset', 0b10000000),
-                BitField('int_reset', 0b01000000),
-                BitField('part_id', 0b00111111, read_only=True)
+            Register("SYSTEM_CONTROL", 0x40, fields=(
+                BitField("sw_reset", 0b10000000),
+                BitField("int_reset", 0b01000000),
+                BitField("part_id", 0b00111111, read_only=True)
             )),
 
-            Register('MODE_CONTROL1', 0x41, fields=(
-                BitField('measurement_time_ms', 0b00000111, adapter=LookupAdapter({
+            Register("MODE_CONTROL1", 0x41, fields=(
+                BitField("measurement_time_ms", 0b00000111, adapter=LookupAdapter({
                     160: 0b000,
                     320: 0b001,
                     640: 0b010,
                     1280: 0b011,
                     2560: 0b100,
                     5120: 0b101
                 })),
             )),
 
-            Register('MODE_CONTROL2', 0x42, fields=(
-                BitField('valid', 0b10000000, read_only=True),
-                BitField('rgbc_en', 0b00010000),
-                BitField('adc_gain_x', 0b00000011, adapter=LookupAdapter({
+            Register("MODE_CONTROL2", 0x42, fields=(
+                BitField("valid", 0b10000000, read_only=True),
+                BitField("rgbc_en", 0b00010000),
+                BitField("adc_gain_x", 0b00000011, adapter=LookupAdapter({
                     1: 0b00, 2: 0b01, 16: 0b10}))
             )),
 
-            Register('MODE_CONTROL3', 0x44, fields=(
-                BitField('on', 0b11111111, adapter=LookupAdapter({True: 2, False: 0})),
+            Register("MODE_CONTROL3", 0x44, fields=(
+                BitField("on", 0b11111111, adapter=LookupAdapter({True: 2, False: 0})),
             )),
 
-            Register('COLOUR_DATA', 0x50, fields=(
-                BitField('red', 0xFFFF000000000000, adapter=U16ByteSwapAdapter()),
-                BitField('green', 0x0000FFFF00000000, adapter=U16ByteSwapAdapter()),
-                BitField('blue', 0x00000000FFFF0000, adapter=U16ByteSwapAdapter()),
-                BitField('clear', 0x000000000000FFFF, adapter=U16ByteSwapAdapter())
+            Register("COLOUR_DATA", 0x50, fields=(
+                BitField("red", 0xFFFF000000000000, adapter=U16ByteSwapAdapter()),
+                BitField("green", 0x0000FFFF00000000, adapter=U16ByteSwapAdapter()),
+                BitField("blue", 0x00000000FFFF0000, adapter=U16ByteSwapAdapter()),
+                BitField("clear", 0x000000000000FFFF, adapter=U16ByteSwapAdapter())
             ), bit_width=64, read_only=True),
 
-            Register('DINT_DATA', 0x58, fields=(
-                BitField('data', 0xFFFF, adapter=U16ByteSwapAdapter()),
+            Register("DINT_DATA", 0x58, fields=(
+                BitField("data", 0xFFFF, adapter=U16ByteSwapAdapter()),
             ), bit_width=16),
 
-            Register('INTERRUPT', 0x60, fields=(
-                BitField('status', 0b10000000, read_only=True),
-                BitField('latch', 0b00010000, adapter=LookupAdapter({0: 1, 1: 0})),
-                BitField('source', 0b00001100, read_only=True, adapter=LookupAdapter({
-                    'red': 0b00,
-                    'green': 0b01,
-                    'blue': 0b10,
-                    'clear': 0b11
+            Register("INTERRUPT", 0x60, fields=(
+                BitField("status", 0b10000000, read_only=True),
+                BitField("latch", 0b00010000, adapter=LookupAdapter({0: 1, 1: 0})),
+                BitField("source", 0b00001100, read_only=True, adapter=LookupAdapter({
+                    "red": 0b00,
+                    "green": 0b01,
+                    "blue": 0b10,
+                    "clear": 0b11
                 })),
-                BitField('enable', 0b00000001)
+                BitField("enable", 0b00000001)
             )),
 
             # 00: Interrupt status is toggled at each measurement end
             # 01: Interrupt status is updated at each measurement end
             # 10: Interrupt status is updated if 4 consecutive threshold judgements are the same
             # 11: Blah blah ditto above except for 8 consecutive judgements
-            Register('PERSISTENCE', 0x61, fields=(
-                BitField('mode', 0b00000011, adapter=LookupAdapter({
-                    'toggle': 0b00,
-                    'update': 0b01,
-                    'update_on_4': 0b10,
-                    'update_on_8': 0b11
+            Register("PERSISTENCE", 0x61, fields=(
+                BitField("mode", 0b00000011, adapter=LookupAdapter({
+                    "toggle": 0b00,
+                    "update": 0b01,
+                    "update_on_4": 0b10,
+                    "update_on_8": 0b11
                 })),
             )),
 
             # High threshold defaults to 0xFFFF
             # Low threshold defaults to 0x0000
-            Register('THRESHOLD', 0x62, fields=(
-                BitField('high', 0xFFFF0000, adapter=U16ByteSwapAdapter()),
-                BitField('low', 0x0000FFFF, adapter=U16ByteSwapAdapter())
+            Register("THRESHOLD", 0x62, fields=(
+                BitField("high", 0xFFFF0000, adapter=U16ByteSwapAdapter()),
+                BitField("low", 0x0000FFFF, adapter=U16ByteSwapAdapter())
             ), bit_width=32),
 
             # Default MANUFACTURER ID is 0xE0h
-            Register('MANUFACTURER', 0x92, fields=(
-                BitField('id', 0xFF),
+            Register("MANUFACTURER", 0x92, fields=(
+                BitField("id", 0xFF),
             ), read_only=True, volatile=False)
         ))
 
         self._bh1745.select_address(self._i2c_addr)
 
         # TODO : Integrate into i2cdevice so that LookupAdapter fields can always be exported to constants
         # Iterate through all register fields and export their lookup tables to constants
         for register in self._bh1745.registers:
             register = self._bh1745.registers[register]
             for field in register.fields:
                 field = register.fields[field]
                 if isinstance(field.adapter, LookupAdapter):
                     for key in field.adapter.lookup_table:
-                        name = 'BH1745_{register}_{field}_{key}'.format(
+                        name = "BH1745_{register}_{field}_{key}".format(
                             register=register.name,
                             field=field.name,
                             key=key
                         ).upper()
                         globals()[name] = key
 
         """
@@ -142,90 +141,90 @@
         :param i2c_addr: Optional i2c_addr to switch to
 
         """
         if self._is_setup:
             return True
 
         if timeout <= 0:
-            raise ValueError('Device timeout period must be greater than 0')
+            raise ValueError("Device timeout period must be greater than 0")
 
         if i2c_addr is not None:
             self._bh1745.select_address(i2c_addr)
 
         try:
-            self._bh1745.get('SYSTEM_CONTROL')
+            self._bh1745.get("SYSTEM_CONTROL")
         except IOError:
-            raise RuntimeError('BH1745 not found: IO error attempting to query device!')
+            raise RuntimeError("BH1745 not found: IO error attempting to query device!")
 
-        if self._bh1745.get('SYSTEM_CONTROL').part_id != 0b001011 or self._bh1745.get('MANUFACTURER').id != 0xE0:
-            raise RuntimeError('BH1745 not found: Manufacturer or Part ID mismatch!')
+        if self._bh1745.get("SYSTEM_CONTROL").part_id != 0b001011 or self._bh1745.get("MANUFACTURER").id != 0xE0:
+            raise RuntimeError("BH1745 not found: Manufacturer or Part ID mismatch!")
 
         self._is_setup = True
 
-        self._bh1745.set('SYSTEM_CONTROL', sw_reset=1)
+        self._bh1745.set("SYSTEM_CONTROL", sw_reset=1)
 
         t_start = time.time()
 
         pending_reset = True
 
         while time.time() - t_start < timeout:
-            if not self._bh1745.get('SYSTEM_CONTROL').sw_reset:
+            if not self._bh1745.get("SYSTEM_CONTROL").sw_reset:
                 pending_reset = False
                 break
             time.sleep(0.01)
 
         if pending_reset:
-            raise BH1745TimeoutError('Timeout waiting for BH1745 to reset.')
+            raise BH1745TimeoutError("Timeout waiting for BH1745 to reset.")
 
-        self._bh1745.set('SYSTEM_CONTROL', int_reset=0)
-        self._bh1745.set('MODE_CONTROL1', measurement_time_ms=320)
-        self._bh1745.set('MODE_CONTROL2', adc_gain_x=1, rgbc_en=1)
-        self._bh1745.set('MODE_CONTROL3', on=1)
-        self._bh1745.set('THRESHOLD', low=0xFFFF, high=0x0000)
-        self._bh1745.set('INTERRUPT', latch=1)
+        self._bh1745.set("SYSTEM_CONTROL", int_reset=0)
+        self._bh1745.set("MODE_CONTROL1", measurement_time_ms=320)
+        self._bh1745.set("MODE_CONTROL2", adc_gain_x=1, rgbc_en=1)
+        self._bh1745.set("MODE_CONTROL3", on=1)
+        self._bh1745.set("THRESHOLD", low=0xFFFF, high=0x0000)
+        self._bh1745.set("INTERRUPT", latch=1)
 
         time.sleep(0.320)
 
     def set_measurement_time_ms(self, time_ms):
         """Set the measurement time in milliseconds.
 
         :param time_ms: The time in milliseconds: 160, 320, 640, 1280, 2560, 5120
 
         """
         self.setup()
-        self._bh1745.set('MODE_CONTROL1', measurement_time_ms=time_ms)
+        self._bh1745.set("MODE_CONTROL1", measurement_time_ms=time_ms)
 
     def set_adc_gain_x(self, gain_x):
         """Set the ADC gain multiplier.
 
         :param gain_x: Must be either 1, 2 or 16
 
         """
         self.setup()
-        self._bh1745.set('MODE_CONTROL2', adc_gain_x=gain_x)
+        self._bh1745.set("MODE_CONTROL2", adc_gain_x=gain_x)
 
     def set_leds(self, state):
         """Toggle the onboard LEDs.
 
         :param state: Either 1 for on, or 0 for off
 
         """
         self.setup()
-        self._bh1745.set('INTERRUPT', enable=1 if state else 0)
+        self._bh1745.set("INTERRUPT", enable=1 if state else 0)
 
     def set_channel_compensation(self, r, g, b, c):
         """Set the channel compensation scale factors.
 
         :param r: multiplier for red channel
         :param g: multiplier for green channel
         :param b: multiplier for blue channel
         :param c: multiplier for clear channel
 
         If you intend to measure a particular class of objects, say a set of matching wooden blocks with similar reflectivity and paint finish
-        you should calibrate the channel compensation until you see colour values that broadly represent the colour of the objects you're testing.
+        you should calibrate the channel compensation until you see colour values that broadly represent the colour of the objects you"re testing.
 
         The default values were derived by testing a set of 5 Red, Green, Blue, Yellow and Orange wooden blocks.
 
         These scale factors are applied in `get_rgbc_raw` right after the raw values are read from the sensor.
 
         """
         self._channel_compensation = (r, g, b, c)
@@ -239,15 +238,15 @@
 
         """
         self._enable_channel_compensation = True if enable else False
 
     def get_rgbc_raw(self):
         """Return the raw Red, Green, Blue and Clear readings."""
         self.setup()
-        colour_data = self._bh1745.get('COLOUR_DATA')
+        colour_data = self._bh1745.get("COLOUR_DATA")
         r, g, b, c = colour_data.red, colour_data.green, colour_data.blue, colour_data.clear
 
         if self._enable_channel_compensation:
             cr, cg, cb, cc = self._channel_compensation
             r, g, b, c = r * cr, g * cg, b * cb, c * cc
 
         return (r, g, b, c)
```

