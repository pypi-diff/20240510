# Comparing `tmp/pyais-2.6.4.tar.gz` & `tmp/pyais-2.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyais-2.6.4.tar", last modified: Sat Apr 27 11:13:07 2024, max compression
+gzip compressed data, was "pyais-2.6.5.tar", last modified: Fri May 10 10:39:56 2024, max compression
```

## Comparing `pyais-2.6.4.tar` & `pyais-2.6.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 11:13:07.777566 pyais-2.6.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-27 11:12:58.000000 pyais-2.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    25573 2024-04-27 11:13:07.777566 pyais-2.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22895 2024-04-27 11:12:58.000000 pyais-2.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 11:13:07.773566 pyais-2.6.4/pyais/
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-27 11:12:58.000000 pyais-2.6.4/pyais/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-27 11:12:58.000000 pyais-2.6.4/pyais/ais_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    17381 2024-04-27 11:12:58.000000 pyais-2.6.4/pyais/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-27 11:12:58.000000 pyais-2.6.4/pyais/decode.py
--rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-04-27 11:12:58.000000 pyais-2.6.4/pyais/encode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-27 11:12:58.000000 pyais-2.6.4/pyais/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8296 2024-04-27 11:12:58.000000 pyais-2.6.4/pyais/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4961 2024-04-27 11:12:58.000000 pyais-2.6.4/pyais/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    64771 2024-04-27 11:12:58.000000 pyais-2.6.4/pyais/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 11:12:58.000000 pyais-2.6.4/pyais/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-04-27 11:12:58.000000 pyais-2.6.4/pyais/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    13014 2024-04-27 11:12:58.000000 pyais-2.6.4/pyais/tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)    16770 2024-04-27 11:12:58.000000 pyais-2.6.4/pyais/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 11:13:07.777566 pyais-2.6.4/pyais.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    25573 2024-04-27 11:13:07.000000 pyais-2.6.4/pyais.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-27 11:13:07.000000 pyais-2.6.4/pyais.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 11:13:07.000000 pyais-2.6.4/pyais.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-27 11:13:07.000000 pyais-2.6.4/pyais.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-27 11:13:07.000000 pyais-2.6.4/pyais.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-27 11:13:07.000000 pyais-2.6.4/pyais.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-27 11:12:58.000000 pyais-2.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 11:13:07.777566 pyais-2.6.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 11:13:07.777566 pyais-2.6.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-04-27 11:12:58.000000 pyais-2.6.4/tests/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    61986 2024-04-27 11:12:58.000000 pyais-2.6.4/tests/test_decode.py
--rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-04-27 11:12:58.000000 pyais-2.6.4/tests/test_decode_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)    32404 2024-04-27 11:12:58.000000 pyais-2.6.4/tests/test_encode.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-27 11:12:58.000000 pyais-2.6.4/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     9064 2024-04-27 11:12:58.000000 pyais-2.6.4/tests/test_file_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    10026 2024-04-27 11:12:58.000000 pyais-2.6.4/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-27 11:12:58.000000 pyais-2.6.4/tests/test_flags.py
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-27 11:12:58.000000 pyais-2.6.4/tests/test_generic_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-27 11:12:58.000000 pyais-2.6.4/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-04-27 11:12:58.000000 pyais-2.6.4/tests/test_nmea.py
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-27 11:12:58.000000 pyais-2.6.4/tests/test_socket.py
--rw-r--r--   0 runner    (1001) docker     (127)     7837 2024-04-27 11:12:58.000000 pyais-2.6.4/tests/test_tag_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-27 11:12:58.000000 pyais-2.6.4/tests/test_talker_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-27 11:12:58.000000 pyais-2.6.4/tests/test_tcp_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    12042 2024-04-27 11:12:58.000000 pyais-2.6.4/tests/test_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-27 11:12:58.000000 pyais-2.6.4/tests/test_udp_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:39:56.226860 pyais-2.6.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-10 10:39:51.000000 pyais-2.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    25573 2024-05-10 10:39:56.226860 pyais-2.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22895 2024-05-10 10:39:51.000000 pyais-2.6.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:39:56.222860 pyais-2.6.5/pyais/
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-10 10:39:51.000000 pyais-2.6.5/pyais/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-10 10:39:51.000000 pyais-2.6.5/pyais/ais_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17381 2024-05-10 10:39:51.000000 pyais-2.6.5/pyais/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-05-10 10:39:51.000000 pyais-2.6.5/pyais/decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-05-10 10:39:51.000000 pyais-2.6.5/pyais/encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-10 10:39:51.000000 pyais-2.6.5/pyais/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8296 2024-05-10 10:39:51.000000 pyais-2.6.5/pyais/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4961 2024-05-10 10:39:51.000000 pyais-2.6.5/pyais/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65172 2024-05-10 10:39:51.000000 pyais-2.6.5/pyais/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 10:39:51.000000 pyais-2.6.5/pyais/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-10 10:39:51.000000 pyais-2.6.5/pyais/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13014 2024-05-10 10:39:51.000000 pyais-2.6.5/pyais/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16771 2024-05-10 10:39:51.000000 pyais-2.6.5/pyais/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:39:56.226860 pyais-2.6.5/pyais.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    25573 2024-05-10 10:39:56.000000 pyais-2.6.5/pyais.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-10 10:39:56.000000 pyais-2.6.5/pyais.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 10:39:56.000000 pyais-2.6.5/pyais.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-10 10:39:56.000000 pyais-2.6.5/pyais.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-10 10:39:56.000000 pyais-2.6.5/pyais.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 10:39:56.000000 pyais-2.6.5/pyais.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-10 10:39:51.000000 pyais-2.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 10:39:56.226860 pyais-2.6.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:39:56.226860 pyais-2.6.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-05-10 10:39:51.000000 pyais-2.6.5/tests/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63783 2024-05-10 10:39:51.000000 pyais-2.6.5/tests/test_decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-05-10 10:39:51.000000 pyais-2.6.5/tests/test_decode_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32404 2024-05-10 10:39:51.000000 pyais-2.6.5/tests/test_encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-10 10:39:51.000000 pyais-2.6.5/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9064 2024-05-10 10:39:51.000000 pyais-2.6.5/tests/test_file_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10026 2024-05-10 10:39:51.000000 pyais-2.6.5/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-10 10:39:51.000000 pyais-2.6.5/tests/test_flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-05-10 10:39:51.000000 pyais-2.6.5/tests/test_generic_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-05-10 10:39:51.000000 pyais-2.6.5/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-05-10 10:39:51.000000 pyais-2.6.5/tests/test_nmea.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-10 10:39:51.000000 pyais-2.6.5/tests/test_socket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7837 2024-05-10 10:39:51.000000 pyais-2.6.5/tests/test_tag_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-10 10:39:51.000000 pyais-2.6.5/tests/test_talker_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-10 10:39:51.000000 pyais-2.6.5/tests/test_tcp_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12042 2024-05-10 10:39:51.000000 pyais-2.6.5/tests/test_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-10 10:39:51.000000 pyais-2.6.5/tests/test_udp_stream.py
```

### Comparing `pyais-2.6.4/LICENSE` & `pyais-2.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyais-2.6.4/PKG-INFO` & `pyais-2.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyais
-Version: 2.6.4
+Version: 2.6.5
 Summary: AIS message decoding
 Author-email: Leon Morten Richter <misc@leonmortenrichter.de>
 Maintainer-email: Leon Morten Richter <misc@leonmortenrichter.de>
 License: MIT License
         
         Copyright (c) 2019 M0r13n
```

### Comparing `pyais-2.6.4/README.md` & `pyais-2.6.5/README.md`

 * *Files identical despite different names*

### Comparing `pyais-2.6.4/pyais/ais_types.py` & `pyais-2.6.5/pyais/ais_types.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.4/pyais/constants.py` & `pyais-2.6.5/pyais/constants.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.4/pyais/decode.py` & `pyais-2.6.5/pyais/decode.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.4/pyais/encode.py` & `pyais-2.6.5/pyais/encode.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.4/pyais/exceptions.py` & `pyais-2.6.5/pyais/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.4/pyais/filter.py` & `pyais-2.6.5/pyais/filter.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.4/pyais/main.py` & `pyais-2.6.5/pyais/main.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.4/pyais/messages.py` & `pyais-2.6.5/pyais/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -793,18 +793,22 @@
     """
     Mixin class to access Communication State values by applicable messages.
 
     You may refer to 3.3.7.2.1 of:
     https://www.itu.int/dms_pubrec/itu-r/rec/m/R-REC-M.1371-1-200108-S!!PDF-E.pdf
     """
 
+    msg_type: int  # Type hint to make mypy happy
     radio: int  # Type hint to make mypy happy
 
     MAX_COMM_STATE_VALUE = 0x7ffff
 
+    SOTDMA_TYPES = (1, 2, 4, 11)
+    SOTDMA_ITDMA_TYPES = (9, 18, 26)
+
     def get_communication_state(self) -> Dict[str, typing.Optional[int]]:
         """Returns information used by the slot allocation algorithm as a dict."""
         result: Dict[str, typing.Optional[int]] = {
             'received_stations': None,
             'slot_number': None,
             'utc_hour': None,
             'utc_minute': None,
@@ -821,21 +825,29 @@
         else:
             result.update(get_itdma_comm_state(self.communication_state_raw))
 
         return result
 
     @property
     def is_sotdma(self) -> bool:
-        """The radio status field has it's 20th bit (MSB) set to 0 or has less than 20 bits"""
-        return self.radio <= self.MAX_COMM_STATE_VALUE
+        """Messages of type 1, 2, 4, 11 use SOTDMA or 9, 18, 26 if 20th bit is set."""
+        if self.msg_type in self.SOTDMA_TYPES:
+            return True
+        if self.msg_type in self.SOTDMA_ITDMA_TYPES:
+            return self.radio <= self.MAX_COMM_STATE_VALUE
+        return False
 
     @property
     def is_itdma(self) -> bool:
-        """The radio status field has it's 20th bit (MSB) set to 1"""
-        return self.radio > self.MAX_COMM_STATE_VALUE
+        """Messages of type 3 use ITDMA or 9, 18, 26 if 20th bit is set."""
+        if self.msg_type == 3:
+            return True
+        if self.msg_type in self.SOTDMA_ITDMA_TYPES:
+            return self.radio > self.MAX_COMM_STATE_VALUE
+        return False
 
     @property
     def communication_state_raw(self) -> int:
         """Get the raw radio status except 20th bit - if present"""
         try:
             return self.radio & self.MAX_COMM_STATE_VALUE
         except AttributeError as err:
```

### Comparing `pyais-2.6.4/pyais/stream.py` & `pyais-2.6.5/pyais/stream.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.4/pyais/tracker.py` & `pyais-2.6.5/pyais/tracker.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.4/pyais/util.py` & `pyais-2.6.5/pyais/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -368,15 +368,15 @@
     sync_state = (radio >> 17) & SYNC_MASK  # First two (2) bits
     slot_timeout = (radio >> 14) & TIMEOUT_MASK  # Next three (3) bits
     sub_msg = radio & MSG_MASK  # Last 14 bits
 
     if slot_timeout == 0:
         result['slot_offset'] = sub_msg
     elif slot_timeout == 1:
-        result['utc_hour'] = (sub_msg >> 9) & 0xf
+        result['utc_hour'] = (sub_msg >> 9) & 0x1f
         result['utc_minute'] = (sub_msg >> 2) & 0x3f
     elif slot_timeout in (2, 4, 6):
         result['slot_number'] = sub_msg
     elif slot_timeout in (3, 5, 7):
         result['received_stations'] = sub_msg
     else:
         raise ValueError("Slot timeout can only be an integer between 0 and 7")
```

### Comparing `pyais-2.6.4/pyais.egg-info/PKG-INFO` & `pyais-2.6.5/pyais.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyais
-Version: 2.6.4
+Version: 2.6.5
 Summary: AIS message decoding
 Author-email: Leon Morten Richter <misc@leonmortenrichter.de>
 Maintainer-email: Leon Morten Richter <misc@leonmortenrichter.de>
 License: MIT License
         
         Copyright (c) 2019 M0r13n
```

### Comparing `pyais-2.6.4/pyais.egg-info/SOURCES.txt` & `pyais-2.6.5/pyais.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyais-2.6.4/pyproject.toml` & `pyais-2.6.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyais-2.6.4/tests/test_constants.py` & `pyais-2.6.5/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.4/tests/test_decode.py` & `pyais-2.6.5/tests/test_decode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1381,14 +1381,22 @@
         assert decode(b"!AIVDM,1,1,,A,14QIG<5620KF@Gl:L9DI4o8N0P00,0*28").turn == 26.0
         assert decode(b"!AIVDM,1,1,,B,13u><=gsQj0mQW:Q1<wRL28P0@:4,0*32").turn == -14.0
         assert decode(b"!AIVDM,1,1,,A,14SSRt021O0?bK@MO7H6QUA600Rg,0*12").turn == 3.0
         assert decode(b"!AIVDM,1,1,,2,13aB:Hhuh0PHjEFNKJg@11sH08J=,0*1E").turn == -4.0
         assert decode(b"!AIVDM,1,1,,A,16:VFv0k0I`KQPpFATG4SgvT40:v,0*7B").turn == -121.0
         assert decode(b"!AIVDM,1,1,,B,16:D3F0:15`5ogh<O?bk>1Dd2L1<,0*0B").turn == 71.0
 
+    def test_sotdma_time_conversion(self):
+        """Prevent regressions for: https://github.com/M0r13n/pyais/pull/135"""
+        decoded = decode('!AIVDM,1,1,,B,133ga6PP0lPPE>4M3G@DpOwTR61p,0*33')
+        cs = decoded.get_communication_state()
+
+        assert cs['utc_hour'] == 16
+        assert cs['utc_minute'] == 30
+
     def test_get_sotdma_comm_state_utc_direct(self):
         msg = "!AIVDM,1,1,,A,13HOI:0P0000VOHLCnHQKwvL05Ip,0*23"
         decoded = decode(msg)
         actual = decoded.get_communication_state()
 
         assert decoded.is_sotdma
         assert not decoded.is_itdma
@@ -1453,14 +1461,40 @@
                 "sync_state": SyncState.UTC_DIRECT,
                 "keep_flag": None,
                 "slot_increment": None,
                 "num_slots": None,
             },
         )
 
+    def test_is_sotdma_or_itdma(self):
+        """ Verify that messages are correctly identified as either ITDMA or SOTDMA.
+        Details: https://github.com/M0r13n/pyais/issues/136."""
+
+        # 1
+        assert decode(b"!AIVDM,1,1,,A,13n3aW0PCkPJS8>Qhc2<urG02D13,0*18").is_sotdma
+        assert not decode(b"!AIVDM,1,1,,A,13n3aW0PCkPJS8>Qhc2<urG02D13,0*18").is_itdma
+        # 2
+        assert decode(b"!AIVDM,1,1,,A,23aFfl0P00PCR?0MEB@h0?w020S7,0*68").is_sotdma
+        assert not decode(b"!AIVDM,1,1,,A,23aFfl0P00PCR?0MEB@h0?w020S7,0*68").is_itdma
+        # 3
+        assert not decode(b"!AIVDM,1,1,,B,33UTPD5000G<@aTL3:?0010j0000,0*2A").is_sotdma
+        assert decode(b"!AIVDM,1,1,,B,33UTPD5000G<@aTL3:?0010j0000,0*2A").is_itdma
+        # 4
+        assert decode(b"!AIVDM,1,1,,B,4h2=aCAuho;QNOUQrvQ6?a1000S:,0*5D").is_sotdma
+        assert not decode(b"!AIVDM,1,1,,B,4h2=aCAuho;QNOUQrvQ6?a1000S:,0*5D").is_itdma
+        # 9
+        assert decode(b"!AIVDM,1,1,,A,91b55vRCQvOo4PLLww<3cGh20@Br,0*79").is_sotdma
+        assert not decode(b"!AIVDM,1,1,,A,91b55vRCQvOo4PLLww<3cGh20@Br,0*79").is_itdma
+        # 11
+        assert decode(b"!AIVDM,1,1,,A,;03t=KQuho;QM`d:WFAtwnW00000,0*7C").is_sotdma
+        assert not decode(b"!AIVDM,1,1,,A,;03t=KQuho;QM`d:WFAtwnW00000,0*7C").is_itdma
+        # 18
+        assert decode(b" !AIVDM,1,1,,A,B6:a?;03wk?8mP=18D3Q3wP61P06,0*7F").is_sotdma
+        assert not decode(b" !AIVDM,1,1,,A,B6:a?;03wk?8mP=18D3Q3wP61P06,0*7F").is_itdma
+
     def test_get_comm_state_type_18_itdma_base_indirect(self):
         msg = "!AIVDM,1,1,,A,B5NJ;PP005l4ot5Isbl03wsUkP06,0*76"
         decoded = decode(msg)
 
         assert decoded.communication_state_raw == 393222
         assert decoded.is_itdma
         assert not decoded.is_sotdma
```

### Comparing `pyais-2.6.4/tests/test_decode_raw.py` & `pyais-2.6.5/tests/test_decode_raw.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.4/tests/test_encode.py` & `pyais-2.6.5/tests/test_encode.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.4/tests/test_examples.py` & `pyais-2.6.5/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.4/tests/test_file_stream.py` & `pyais-2.6.5/tests/test_file_stream.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.4/tests/test_filters.py` & `pyais-2.6.5/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.4/tests/test_flags.py` & `pyais-2.6.5/tests/test_flags.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.4/tests/test_generic_stream.py` & `pyais-2.6.5/tests/test_generic_stream.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.4/tests/test_main.py` & `pyais-2.6.5/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.4/tests/test_nmea.py` & `pyais-2.6.5/tests/test_nmea.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.4/tests/test_socket.py` & `pyais-2.6.5/tests/test_socket.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.4/tests/test_tag_block.py` & `pyais-2.6.5/tests/test_tag_block.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.4/tests/test_talker_ids.py` & `pyais-2.6.5/tests/test_talker_ids.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.4/tests/test_tcp_stream.py` & `pyais-2.6.5/tests/test_tcp_stream.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.4/tests/test_tracker.py` & `pyais-2.6.5/tests/test_tracker.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.4/tests/test_udp_stream.py` & `pyais-2.6.5/tests/test_udp_stream.py`

 * *Files identical despite different names*

