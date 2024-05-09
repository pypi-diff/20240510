# Comparing `tmp/proconip-1.3.0.tar.gz` & `tmp/proconip-1.3.1.tar.gz`

## Comparing `proconip-1.3.0.tar` & `proconip-1.3.1.tar`

### file list

```diff
@@ -1,22 +1,26 @@
--rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 proconip-1.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 proconip-1.3.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 proconip-1.3.0/SECURITY.md
--rw-r--r--   0        0        0    43535 2020-02-02 00:00:00.000000 proconip-1.3.0/logo.png
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 proconip-1.3.0/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 proconip-1.3.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 proconip-1.3.0/.github/workflows/unittest.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proconip-1.3.0/src/__init__.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 proconip-1.3.0/src/requirements.txt
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 proconip-1.3.0/src/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proconip-1.3.0/src/proconip/__init__.py
--rw-r--r--   0        0        0    10022 2020-02-02 00:00:00.000000 proconip-1.3.0/src/proconip/api.py
--rw-r--r--   0        0        0    23750 2020-02-02 00:00:00.000000 proconip-1.3.0/src/proconip/definitions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proconip-1.3.0/tests/__init__.py
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 proconip-1.3.0/tests/helper.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 proconip-1.3.0/tests/requirements.txt
--rw-r--r--   0        0        0    12006 2020-02-02 00:00:00.000000 proconip-1.3.0/tests/test_definitions.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 proconip-1.3.0/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 proconip-1.3.0/LICENSE
--rw-r--r--   0        0        0     7823 2020-02-02 00:00:00.000000 proconip-1.3.0/README.md
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 proconip-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     8409 2020-02-02 00:00:00.000000 proconip-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 proconip-1.3.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 proconip-1.3.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 proconip-1.3.1/SECURITY.md
+-rw-r--r--   0        0        0    43535 2020-02-02 00:00:00.000000 proconip-1.3.1/logo.png
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 proconip-1.3.1/requirements.txt
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 proconip-1.3.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 proconip-1.3.1/.github/workflows/automerge.yml
+-rw-r--r--   0        0        0     3505 2020-02-02 00:00:00.000000 proconip-1.3.1/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 proconip-1.3.1/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 proconip-1.3.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 proconip-1.3.1/.github/workflows/unittest.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proconip-1.3.1/src/__init__.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 proconip-1.3.1/src/requirements.txt
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 proconip-1.3.1/src/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proconip-1.3.1/src/proconip/__init__.py
+-rw-r--r--   0        0        0     9929 2020-02-02 00:00:00.000000 proconip-1.3.1/src/proconip/api.py
+-rw-r--r--   0        0        0    23650 2020-02-02 00:00:00.000000 proconip-1.3.1/src/proconip/definitions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proconip-1.3.1/tests/__init__.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 proconip-1.3.1/tests/helper.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 proconip-1.3.1/tests/requirements.txt
+-rw-r--r--   0        0        0    12273 2020-02-02 00:00:00.000000 proconip-1.3.1/tests/test_definitions.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 proconip-1.3.1/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 proconip-1.3.1/LICENSE
+-rw-r--r--   0        0        0     9483 2020-02-02 00:00:00.000000 proconip-1.3.1/README.md
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 proconip-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0    10069 2020-02-02 00:00:00.000000 proconip-1.3.1/PKG-INFO
```

### Comparing `proconip-1.3.0/CODE_OF_CONDUCT.md` & `proconip-1.3.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `proconip-1.3.0/CONTRIBUTING.md` & `proconip-1.3.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `proconip-1.3.0/logo.png` & `proconip-1.3.1/logo.png`

 * *Files identical despite different names*

### Comparing `proconip-1.3.0/.github/workflows/python-publish.yml` & `proconip-1.3.1/.github/workflows/python-publish.yml`

 * *Files 14% similar despite different names*

```diff
@@ -17,23 +17,23 @@
 
 jobs:
   deploy:
 
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up Python
-      uses: actions/setup-python@v3
+      uses: actions/setup-python@v5
       with:
         python-version: '3.x'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install build
     - name: Build package
       run: python -m build
     - name: Publish package
-      uses: pypa/gh-action-pypi-publish@27b31702a0e7fc50959f5ad993c78deac1bdfc29
+      uses: pypa/gh-action-pypi-publish@81e9d935c883d0b210363ab89cf05f3894778450
       with:
         user: __token__
         password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `proconip-1.3.0/.github/workflows/unittest.yml` & `proconip-1.3.1/.github/workflows/unittest.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 name: Unittest
 
-on: [push]
+on:
+  push:
+  pull_request:
+  workflow_call:
 
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.11"]
+        python-version: ["3.12"]
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v3
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -r tests/requirements.txt
     - name: Run unit tests
```

### Comparing `proconip-1.3.0/src/proconip/api.py` & `proconip-1.3.1/src/proconip/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """GetState class to get data from the GetState.csv interface."""
+
 import asyncio
 import socket
 import async_timeout
 
 from aiohttp import (
     BasicAuth,
     ClientError,
@@ -28,18 +29,15 @@
 ) -> str:
     """Get raw data (csv string) from the GetState.csv interface."""
     url = URL(config.base_url).with_path(API_PATH_GET_STATE)
     try:
         async with async_timeout.timeout(10):
             response = await client_session.get(
                 url,
-                auth=BasicAuth(
-                    config.username,
-                    password=config.password
-                ),
+                auth=BasicAuth(config.username, password=config.password),
             )
             if response.status in (401, 403):
                 raise BadCredentialsException("Invalid credentials")
             response.raise_for_status()
             return await response.text()
     except asyncio.TimeoutError as exception:
         raise ProconipApiException(
@@ -63,39 +61,30 @@
     raw_data = await async_get_raw_state(client_session, config)
     structured_data = GetStateData(raw_data)
     return structured_data
 
 
 class GetState:
     """GetState class to get data from the GetState.csv interface."""
-    def __init__(
-        self,
-        client_session: ClientSession,
-        config: ConfigObject
-    ):
+
+    def __init__(self, client_session: ClientSession, config: ConfigObject):
         self.client_session = client_session
         self.config = config
 
     async def async_get_raw_state(
         self,
     ) -> str:
         """Get raw data (csv string) from the GetState.csv interface."""
-        return await async_get_raw_state(
-            self.client_session,
-            self.config
-        )
+        return await async_get_raw_state(self.client_session, self.config)
 
     async def async_get_state(
         self,
     ) -> GetStateData:
         """Get structured data from the GetState.csv interface."""
-        return await async_get_state(
-            self.client_session,
-            self.config
-        )
+        return await async_get_state(self.client_session, self.config)
 
 
 async def async_post_usrcfg_cgi(
     client_session: ClientSession,
     config: ConfigObject,
     payload: str,
 ) -> str:
@@ -124,58 +113,58 @@
     except Exception as exception:  # pylint: disable=broad-except
         raise BadStatusCodeException(
             "Unexpected response",
         ) from exception
 
 
 async def async_switch_on(
-        client_session: ClientSession,
-        config: ConfigObject,
-        current_state: GetStateData,
-        relay: Relay,
+    client_session: ClientSession,
+    config: ConfigObject,
+    current_state: GetStateData,
+    relay: Relay,
 ) -> str:
     """Switch on a relay using the usrcfg.cgi interface."""
     if current_state.is_dosage_relay(relay):
         raise BadRelayException(
             "Cannot permanently switch on a dosage relay",
         )
     bit_state = current_state.determine_overall_relay_bit_state()
     relay_bit_mask = relay.get_bit_mask()
     bit_state[0] |= relay_bit_mask
     bit_state[1] |= relay_bit_mask
     return await async_post_usrcfg_cgi(
         client_session=client_session,
         config=config,
-        payload=f"ENA={bit_state[0]},{bit_state[1]}&MANUAL=1"
+        payload=f"ENA={bit_state[0]},{bit_state[1]}&MANUAL=1",
     )
 
 
 async def async_switch_off(
-        client_session: ClientSession,
-        config: ConfigObject,
-        current_state: GetStateData,
-        relay: Relay,
+    client_session: ClientSession,
+    config: ConfigObject,
+    current_state: GetStateData,
+    relay: Relay,
 ) -> str:
     """Switch on a relay using the usrcfg.cgi interface."""
     bit_state = current_state.determine_overall_relay_bit_state()
     relay_bit_mask = relay.get_bit_mask()
     bit_state[0] |= relay_bit_mask
     bit_state[1] &= ~relay_bit_mask
     return await async_post_usrcfg_cgi(
         client_session=client_session,
         config=config,
         payload=f"ENA={bit_state[0]},{bit_state[1]}&MANUAL=1",
     )
 
 
 async def async_set_auto_mode(
-        client_session: ClientSession,
-        config: ConfigObject,
-        current_state: GetStateData,
-        relay: Relay,
+    client_session: ClientSession,
+    config: ConfigObject,
+    current_state: GetStateData,
+    relay: Relay,
 ) -> str:
     """Switch a relay to auto mode using the usrcfg.cgi interface."""
     bit_state = current_state.determine_overall_relay_bit_state()
     relay_bit_mask = relay.get_bit_mask()
     bit_state[0] &= ~relay_bit_mask
     bit_state[1] &= ~relay_bit_mask
     return await async_post_usrcfg_cgi(
@@ -183,14 +172,15 @@
         config=config,
         payload=f"ENA={bit_state[0]},{bit_state[1]}&MANUAL=1",
     )
 
 
 class RelaySwitch:
     """RelaySwitch class to set relay states via usrcfg.cgi interface."""
+
     def __init__(
         self,
         client_session: ClientSession,
         config: ConfigObject,
     ):
         self.client_session = client_session
         self.config = config
@@ -252,29 +242,30 @@
                     login=config.username,
                     password=config.password,
                 ),
             )
             response.raise_for_status()
             return await response.text()
     except asyncio.TimeoutError as exception:
-        raise ProconipApiException(
+        raise TimeoutException(
             "Timeout error fetching data",
         ) from exception
     except (ClientError, socket.gaierror) as exception:
         raise ProconipApiException(
             "Error fetching data",
         ) from exception
     except Exception as exception:  # pylint: disable=broad-except
         raise BadStatusCodeException(
             "Unexpected response",
         ) from exception
 
 
 class DosageControl:
     """DosageControl class to start manual dosage via Command.htm endpoint."""
+
     def __init__(
         self,
         client_session: ClientSession,
         config: ConfigObject,
     ):
         self.client_session = client_session
         self.config = config
@@ -296,33 +287,37 @@
         dosage_duration: int,
     ) -> str:
         """Start manual pH minus dosage."""
         return await async_start_dosage(
             client_session=self.client_session,
             config=self.config,
             dosage_target=DosageTarget.PH_MINUS,
-            dosage_duration=dosage_duration
+            dosage_duration=dosage_duration,
         )
 
     async def async_ph_plus_dosage(
         self,
         dosage_duration: int,
     ) -> str:
         """Start manual pH plus dosage."""
         return await async_start_dosage(
             client_session=self.client_session,
             config=self.config,
             dosage_target=DosageTarget.PH_PLUS,
-            dosage_duration=dosage_duration
+            dosage_duration=dosage_duration,
         )
 
 
 class ProconipApiException(Exception):
     """Exception to raise when an api call fails."""
 
 
 class BadCredentialsException(ProconipApiException):
     """Exception to raise when we get an 401 Unauthorized or 403 Forbidden response."""
 
 
 class BadStatusCodeException(ProconipApiException):
     """Exception to raise when we get an unknown response code."""
+
+
+class TimeoutException(ProconipApiException):
+    """Exception to raise when the connection times out."""
```

### Comparing `proconip-1.3.0/src/proconip/definitions.py` & `proconip-1.3.1/src/proconip/definitions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Defines data structures for use with and used by the GetState.csv and usercfg.cgi APIs."""
+
 import dataclasses
 from enum import IntEnum
 
 
 API_PATH_GET_STATE = "/GetState.csv"
 API_PATH_USRCFG = "/usrcfg.cgi"
 API_PATH_COMMAND = "/Command.htm"
@@ -35,14 +36,15 @@
     4: "Error (GUI warning, red)",
     65536: "NTP available",
 }
 
 
 class DosageTarget(IntEnum):
     """Helper enum for async_start_dosage."""
+
     CHLORINE = 0
     PH_MINUS = 1
     PH_PLUS = 2
 
 
 @dataclasses.dataclass
 class ConfigObject:
@@ -91,28 +93,38 @@
     _offset: float
     _gain: float
     _raw_value: float
     _value: float
     _display_value: str
 
     # pylint: disable=R0913
-    def __init__(self, column: int, name: str, unit: str, offset: float, gain: float, value: float):
+    def __init__(
+        self,
+        column: int,
+        name: str,
+        unit: str,
+        offset: float,
+        gain: float,
+        value: float,
+    ):
         self._column = column
 
         self._name = name
         self._unit = unit
         self._offset = offset
         self._gain = gain
         self._raw_value = value
         self._value = self._offset + (self._gain * self._raw_value)
 
         if column == 0:
             self._category = CATEGORY_TIME
             self._category_id = 0
-            self._display_value = f"{int(self._value / 256):02d}:{(int(self._value) % 256):02d}"
+            self._display_value = (
+                f"{int(self._value / 256):02d}:{(int(self._value) % 256):02d}"
+            )
         elif 1 <= column <= 5:
             self._category = CATEGORY_ANALOG
             self._category_id = column - 1
             self._display_value = f"{self._value:.2f} {self._unit}"
         elif 6 <= column <= 7:
             self._category = CATEGORY_ELECTRODE
             self._category_id = column - 6
@@ -214,15 +226,16 @@
     def __init__(self, data_object: DataObject):
         super().__init__(
             data_object.column,
             data_object.name,
             data_object.unit,
             data_object.offset,
             data_object.gain,
-            data_object.value)
+            data_object.value,
+        )
 
     def __str__(self):
         return f"{self._name}: {self._display_value}"
 
     @property
     def relay_id(self) -> int:
         """Returns the aggregated relays id (eg. 8 for the first external relay)."""
@@ -288,16 +301,17 @@
         self._data_names = lines[line + 1].split(",")
         self._data_units = lines[line + 2].split(",")
         self._data_offsets = [float(offset) for offset in lines[line + 3].split(",")]
         self._data_gain = [float(gain) for gain in lines[line + 4].split(",")]
         self._data_raw_values = [float(raw) for raw in lines[line + 5].split(",")]
         self._data_values: dict[int, float] = {}
         for i, value in enumerate(self._data_raw_values):
-            self._data_values[i] = (float(value) - float(self._data_offsets[i])) \
-                                   * float(self._data_gain[i])
+            self._data_values[i] = (
+                float(value) - float(self._data_offsets[i])
+            ) * float(self._data_gain[i])
 
         self._parse_system_info()
         self._parse()
         self._time = self._data_objects[0].display_value
 
     def __str__(self):
         return self._raw_data
@@ -406,18 +420,20 @@
             case 37 | 40:
                 return self._ph_minus_dosage_relay_id
             case 38 | 41:
                 return self._ph_plus_dosage_relay_id
             case _:
                 return False
 
-    def is_dosage_relay(self,
-                        relay_object: Relay = None,
-                        data_object: DataObject = None,
-                        relay_id: int = None) -> bool:
+    def is_dosage_relay(
+        self,
+        relay_object: Relay = None,
+        data_object: DataObject = None,
+        relay_id: int = None,
+    ) -> bool:
         """Returns true if the given relay_object OR data_object OR column refers to a dosage
         control relay."""
         dosage_control_relays = [
             self._chlorine_dosage_relay_id,
             self._ph_minus_dosage_relay_id,
             self._ph_plus_dosage_relay_id,
         ]
@@ -484,37 +500,49 @@
         """Returns true if the DMX extension is enabled, false otherwise."""
         return self._config_other_enable & 256 == 256
 
     def _parse(self):
         """Parse the raw data and populate the object's attributes."""
         self._data_objects = []
         for column, name in enumerate(self._data_names):
-            self._data_objects.append(DataObject(column,
-                                                 name,
-                                                 self._data_units[column],
-                                                 self._data_offsets[column],
-                                                 self._data_gain[column],
-                                                 self._data_raw_values[column]))
-
-        self._analog_objects = [obj for obj in self._data_objects
-                                if obj.category == CATEGORY_ANALOG]
-        self._electrode_objects = [obj for obj in self._data_objects
-                                   if obj.category == CATEGORY_ELECTRODE]
-        self._temperature_objects = [obj for obj in self._data_objects
-                                     if obj.category == CATEGORY_TEMPERATURE]
-        self._relay_objects = [obj for obj in self._data_objects
-                               if obj.category == CATEGORY_RELAY]
-        self._digital_objects = [obj for obj in self._data_objects
-                                 if obj.category == CATEGORY_DIGITAL_INPUT]
-        self._external_relay_objects = [obj for obj in self._data_objects
-                                        if obj.category == CATEGORY_EXTERNAL_RELAY]
-        self._canister_objects = [obj for obj in self._data_objects
-                                  if obj.category == CATEGORY_CANISTER]
-        self._consumption_objects = [obj for obj in self._data_objects
-                                     if obj.category == CATEGORY_CONSUMPTION]
+            self._data_objects.append(
+                DataObject(
+                    column,
+                    name,
+                    self._data_units[column],
+                    self._data_offsets[column],
+                    self._data_gain[column],
+                    self._data_raw_values[column],
+                )
+            )
+
+        self._analog_objects = [
+            obj for obj in self._data_objects if obj.category == CATEGORY_ANALOG
+        ]
+        self._electrode_objects = [
+            obj for obj in self._data_objects if obj.category == CATEGORY_ELECTRODE
+        ]
+        self._temperature_objects = [
+            obj for obj in self._data_objects if obj.category == CATEGORY_TEMPERATURE
+        ]
+        self._relay_objects = [
+            obj for obj in self._data_objects if obj.category == CATEGORY_RELAY
+        ]
+        self._digital_objects = [
+            obj for obj in self._data_objects if obj.category == CATEGORY_DIGITAL_INPUT
+        ]
+        self._external_relay_objects = [
+            obj for obj in self._data_objects if obj.category == CATEGORY_EXTERNAL_RELAY
+        ]
+        self._canister_objects = [
+            obj for obj in self._data_objects if obj.category == CATEGORY_CANISTER
+        ]
+        self._consumption_objects = [
+            obj for obj in self._data_objects if obj.category == CATEGORY_CONSUMPTION
+        ]
 
     @property
     def analog_objects(self) -> list[DataObject]:
         """Returns a list of DataObjects of the analog category."""
         return self._analog_objects
 
     @property
@@ -545,15 +573,16 @@
     def external_relay_objects(self) -> list[DataObject]:
         """Returns a list of DataObjects of the external relay category."""
         return self._external_relay_objects
 
     def external_relays(self) -> list[Relay]:
         """Returns external relays as a list of Relay object instances."""
         return [
-            Relay(external_relay_object) for external_relay_object in self._external_relay_objects
+            Relay(external_relay_object)
+            for external_relay_object in self._external_relay_objects
         ]
 
     @property
     def canister_objects(self) -> list[DataObject]:
         """Returns a list of DataObjects of the canister category."""
         return self._canister_objects
 
@@ -624,15 +653,15 @@
 
     def get_relay(self, relay_id: int) -> Relay:
         """Returns the Relay instance for the given id."""
         return Relay(self.aggregated_relay_objects[relay_id])
 
     def get_relays(self) -> list[Relay]:
         """Returns a list of all relays as Relay instances."""
-        return  self.relays() + self.external_relays()
+        return self.relays() + self.external_relays()
 
     def determine_overall_relay_bit_state(self) -> [int, int]:
         """Determine the overall relay bit state from the current state."""
         relays = self.relays()
         bit_state = [255, 0]
         if self.is_relay_extension_enabled():
             relays.extend(self.external_relays())
@@ -641,9 +670,10 @@
             relay_bit_mask = relay.get_bit_mask()
             if relay.is_auto_mode():
                 bit_state[0] &= ~relay_bit_mask
             if relay.is_on():
                 bit_state[1] |= relay_bit_mask
         return bit_state
 
+
 class BadRelayException(Exception):
     """Exception to raise when an invalid relay was given as parameter."""
```

### Comparing `proconip-1.3.0/tests/helper.py` & `proconip-1.3.1/tests/helper.py`

 * *Files identical despite different names*

### Comparing `proconip-1.3.0/tests/test_definitions.py` & `proconip-1.3.1/tests/test_definitions.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,35 +21,37 @@
     USERNAME,
     PASSWORD,
 )
 
 
 class ConfigObjectTestCase(unittest.TestCase):
     """Testing the ConfigObject class."""
+
     def test_initialization(self):
         """Test the initialization of the ConfigObject class."""
         actual = ConfigObject(BASE_URL, USERNAME, PASSWORD)
         self.assertEqual(actual.base_url, BASE_URL)
         self.assertEqual(actual.username, USERNAME)
         self.assertEqual(actual.password, PASSWORD)
 
 
 class GetStateDataTestCase(unittest.TestCase):
     """Testing the GetStateData class."""
+
     def setUp(self):
         """Set up the test case."""
         self.actual = GetStateData(GET_STATE_CSV)
 
     def test_initialization(self):
         """Test the initialization of the GetStateData class."""
         actual = GetStateData(GET_STATE_CSV)
         self.assertIsNotNone(actual)
 
     def test_system_info(self):
-        """"Test the system info properties of the GetStateData class."""
+        """ "Test the system info properties of the GetStateData class."""
         self.assertEqual("1.7.3", self.actual.version)
         self.assertEqual(9559698, self.actual.cpu_time)
         self.assertEqual(1, self.actual.reset_root_cause)
         self.assertEqual(3, self.actual.ntp_fault_state)
         self.assertEqual(0, self.actual.config_other_enable)
         self.assertEqual(False, self.actual.is_tcpip_boost_enabled())
         self.assertEqual(False, self.actual.is_sd_card_enabled())
@@ -64,22 +66,36 @@
         self.assertEqual(4, self.actual.ph_plus_dosage_relay_id)
         self.assertEqual(4, self.actual.ph_minus_dosage_relay_id)
         self.assertEqual(5, self.actual.chlorine_dosage_relay_id)
         self.assertEqual(True, self.actual.is_chlorine_dosage_enabled())
         self.assertEqual(False, self.actual.is_electrolysis_enabled())
         self.assertEqual(True, self.actual.is_ph_minus_dosage_enabled())
         self.assertEqual(False, self.actual.is_ph_plus_dosage_enabled())
-        self.assertEqual(True, self.actual.is_dosage_enabled(self.actual.canister_objects[0]))
-        self.assertEqual(True, self.actual.is_dosage_enabled(self.actual.canister_objects[1]))
-        self.assertEqual(False, self.actual.is_dosage_enabled(self.actual.canister_objects[2]))
-        self.assertEqual(True, self.actual.is_dosage_enabled(self.actual.consumption_objects[0]))
-        self.assertEqual(True, self.actual.is_dosage_enabled(self.actual.consumption_objects[1]))
-        self.assertEqual(False, self.actual.is_dosage_enabled(self.actual.consumption_objects[2]))
+        self.assertEqual(
+            True, self.actual.is_dosage_enabled(self.actual.canister_objects[0])
+        )
+        self.assertEqual(
+            True, self.actual.is_dosage_enabled(self.actual.canister_objects[1])
+        )
+        self.assertEqual(
+            False, self.actual.is_dosage_enabled(self.actual.canister_objects[2])
+        )
+        self.assertEqual(
+            True, self.actual.is_dosage_enabled(self.actual.consumption_objects[0])
+        )
+        self.assertEqual(
+            True, self.actual.is_dosage_enabled(self.actual.consumption_objects[1])
+        )
+        self.assertEqual(
+            False, self.actual.is_dosage_enabled(self.actual.consumption_objects[2])
+        )
         self.assertEqual("External reset", self.actual.get_reset_root_cause_as_str())
-        self.assertEqual("Warning (GUI warning, yellow)", self.actual.get_ntp_fault_state_as_str())
+        self.assertEqual(
+            "Warning (GUI warning, yellow)", self.actual.get_ntp_fault_state_as_str()
+        )
 
     def test_time(self):
         """Test the time property of the GetStateData class."""
         self.assertEqual("02:17", self.actual.time)
 
     def test_analog_objects(self):
         """Test the analog objects property of the GetStateData class."""
@@ -115,21 +131,25 @@
         self.assertEqual("pH", self.actual.ph_electrode.unit)
         self.assertIsNotNone(self.actual.ph_electrode.offset)
         self.assertIsNotNone(self.actual.ph_electrode.gain)
         self.assertIsNotNone(self.actual.ph_electrode.raw_value)
         self.assertIsNotNone(self.actual.ph_electrode.value)
         self.assertIsNotNone(self.actual.ph_electrode.display_value)
         self.assertIsNotNone(self.actual.ph_electrode.column)
-        self.assertEqual(self.actual.ph_electrode.column - 6, self.actual.ph_electrode.category_id)
+        self.assertEqual(
+            self.actual.ph_electrode.column - 6, self.actual.ph_electrode.category_id
+        )
         self.assertEqual(CATEGORY_ELECTRODE, self.actual.ph_electrode.category)
 
     def test_temperature_objects(self):
         """Test the temperature objects property of the GetStateData class."""
         self.assertEqual(len(self.actual.temperature_objects), 8)
-        for category_id, temperature_object in enumerate(self.actual.temperature_objects):
+        for category_id, temperature_object in enumerate(
+            self.actual.temperature_objects
+        ):
             self.assertIsNotNone(temperature_object.name)
             self.assertEqual(temperature_object.unit, "C")
             self.assertIsNotNone(temperature_object.offset)
             self.assertIsNotNone(temperature_object.gain)
             self.assertIsNotNone(temperature_object.raw_value)
             self.assertIsNotNone(temperature_object.value)
             self.assertIsNotNone(temperature_object.display_value)
@@ -151,30 +171,34 @@
             self.assertEqual(relay_object.column, category_id + 16)
             self.assertEqual(relay_object.category, CATEGORY_RELAY)
             self.assertEqual(relay_object.category_id, category_id)
 
     def test_digital_input_objects(self):
         """Test the digital input objects property of the GetStateData class."""
         self.assertEqual(len(self.actual.digital_input_objects), 4)
-        for category_id, digital_input_object in enumerate(self.actual.digital_input_objects):
+        for category_id, digital_input_object in enumerate(
+            self.actual.digital_input_objects
+        ):
             self.assertIsNotNone(digital_input_object.name)
             self.assertIsNotNone(digital_input_object.unit)
             self.assertIsNotNone(digital_input_object.offset)
             self.assertIsNotNone(digital_input_object.gain)
             self.assertIsNotNone(digital_input_object.raw_value)
             self.assertIsNotNone(digital_input_object.value)
             self.assertIsNotNone(digital_input_object.display_value)
             self.assertEqual(digital_input_object.column, category_id + 24)
             self.assertEqual(digital_input_object.category, CATEGORY_DIGITAL_INPUT)
             self.assertEqual(digital_input_object.category_id, category_id)
 
     def test_external_relay_objects(self):
         """Test the external relay objects property of the GetStateData class."""
         self.assertEqual(len(self.actual.external_relay_objects), 8)
-        for category_id, external_relay_object in enumerate(self.actual.external_relay_objects):
+        for category_id, external_relay_object in enumerate(
+            self.actual.external_relay_objects
+        ):
             self.assertIsNotNone(external_relay_object.name)
             self.assertEqual(external_relay_object.unit, "--")
             self.assertIsNotNone(external_relay_object.offset)
             self.assertIsNotNone(external_relay_object.gain)
             self.assertIsNotNone(external_relay_object.raw_value)
             self.assertIsNotNone(external_relay_object.value)
             self.assertIsNotNone(external_relay_object.display_value)
@@ -196,15 +220,17 @@
             self.assertEqual(canister_object.column, category_id + 36)
             self.assertEqual(canister_object.category, CATEGORY_CANISTER)
             self.assertEqual(canister_object.category_id, category_id)
 
     def test_consumption_objects(self):
         """Test the consumption objects property of the GetStateData class."""
         self.assertEqual(len(self.actual.consumption_objects), 3)
-        for category_id, consumption_object in enumerate(self.actual.consumption_objects):
+        for category_id, consumption_object in enumerate(
+            self.actual.consumption_objects
+        ):
             self.assertIsNotNone(consumption_object.name)
             self.assertIsNotNone(consumption_object.unit)
             self.assertIsNotNone(consumption_object.offset)
             self.assertIsNotNone(consumption_object.gain)
             self.assertIsNotNone(consumption_object.raw_value)
             self.assertIsNotNone(consumption_object.value)
             self.assertIsNotNone(consumption_object.display_value)
@@ -213,9 +239,9 @@
             self.assertEqual(consumption_object.category_id, category_id)
 
     def test_aggregated_relay_objects(self):
         """Test the aggregated relay objects property of the GetStateData class."""
         self.assertEqual(len(self.actual.aggregated_relay_objects), 16)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `proconip-1.3.0/.gitignore` & `proconip-1.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `proconip-1.3.0/LICENSE` & `proconip-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `proconip-1.3.0/README.md` & `proconip-1.3.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # Python package for the ProCon.IP Pool Controller
 
 [![Pylint](https://github.com/ylabonte/proconip-pypi/actions/workflows/pylint.yml/badge.svg)](https://github.com/ylabonte/proconip-pypi/actions/workflows/pylint.yml)
 [![Unittest](https://github.com/ylabonte/proconip-pypi/actions/workflows/unittest.yml/badge.svg)](https://github.com/ylabonte/proconip-pypi/actions/workflows/unittest.yml)
+[![CodeQL](https://github.com/ylabonte/proconip-pypi/actions/workflows/codeql.yml/badge.svg)](https://github.com/ylabonte/proconip-pypi/actions/workflows/codeql.yml)
 [![PyPi Package release](https://github.com/ylabonte/proconip-pypi/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ylabonte/proconip-pypi/actions/workflows/python-publish.yml)
 
 [![PyPI](https://img.shields.io/pypi/v/proconip?label=Current%20Release)](https://pypi.org/project/proconip/)
 
 ## Overview
 
 * [Introduction (_What is this library for?_)](#introduction)
 * [Installation](#installation)
 * [Usage](#usage-examples)
   * [Reading the current state](#reading-the-current-state)
   * [Switching relays](#switching-relays)
 * [A brief description of the ProCon.IP pool controller](#a-brief-description-of-the-proconip-pool-controller)
 * [Get support](#get-support)
 * [Give support](#give-support)
+* [Release Notes](#release-notes)
 * [Disclaimer](#disclaimer)
 
 ---
 ![ProCon.IP Python Library](./logo.png)
 
 ## Introduction
 
@@ -173,13 +175,62 @@
 
 If you want to support this project or my work in general, you can do so without having any coding abilities.
 Because programmers are described as machines that convert coffee (their habitual input) into code (their habitual
 output), there is a really simple way to support me:
 
 [<img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 40px !important;width: 144px !important;" >](https://www.buymeacoffee.com/ylabonte)
 
+## Release Notes
+
+### v1.3.1 (2024-05-09)
+* Add dedicated `api.TimeoutException` to raise for connection timeouts.
+* Add dependabot with `versioning-strategy: "increase"` and an auto-merge workflow for automated updates on the github 
+  `main` branch.
+* Add code scanning (CodeQL) workflow.
+
+### v1.3.0 (2023-08-16)
+* Add `GetStateData.get_relays()` to get all available Relay instances.
+
+### v1.2.7 (2023-07-04)
+* Fix calculation formula for actual values (`offset + gain * raw`).
+
+### v1.2.6 (2023-06-20)
+* Fix DosageTarget enum and return value of `DosageControl.async_ph_plus_dosage`.
+
+### v1.2.5 (2023-06-18)
+* Fix return type/value of `DosageControl.async_ph_plus_dosage()`
+
+### v1.2.4 (2023-06-18)
+* Refactor request exception handling
+
+### v1.2.3 (2023-06-17)
+* Fix api methods to produce `BadCredentialsExceptions` in case of 401 and 403 responses.
+
+### v1.2.2 (2023-06-12)
+* Fix typo in `BadStatusCodeException`
+
+### v1.2.1 (2023-06-12)
+* Avoid invalid operations regarding dosage control relays.
+
+### v1.2.0 (2023-06-12)
+* Add DosageControl abilities.
+
+### v1.1.0 (2023-05-23)
+*  Unify api methods and naming conventions:
+  * Same names for functions and class methods with same functionality.
+  * `async_` prefixes for all async functions/methods.
+
+### v1.0.0 (2023-05-21)
+* Fix post data for switching relays.
+
+### v0.0.2 (2023-05-18)
+* Add relay switching capabilities.
+
+### v0.0.1 (2023-04-23)
+* Initial release with data reading capabilities.
+
 ## Disclaimer
 
 **Just to be clear: I have nothing to do with the development, selling, marketing or support of the pool controller
 unit itself.  
 I just developed small TypeScript/JS and Python libraries as by-products of an ioBroker adapter and a Home Assistant
 integration for integrating the pool controller unit with common smart home solutions.**
```

### Comparing `proconip-1.3.0/pyproject.toml` & `proconip-1.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "proconip"
-version = "1.3.0"
+version = "1.3.1"
 authors = [
   { name="Yannic Labonte", email="yannic.labonte@gmail.com" },
 ]
 description = "Library for basic interaction with the Procon.IP pool controller unit."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `proconip-1.3.0/PKG-INFO` & `proconip-1.3.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: proconip
-Version: 1.3.0
+Version: 1.3.1
 Summary: Library for basic interaction with the Procon.IP pool controller unit.
 Project-URL: Homepage, https://github.com/ylabonte/proconip-pypi
 Project-URL: Bug Tracker, https://github.com/ylabonte/proconip-pypi/issues
 Author-email: Yannic Labonte <yannic.labonte@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -12,28 +12,30 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # Python package for the ProCon.IP Pool Controller
 
 [![Pylint](https://github.com/ylabonte/proconip-pypi/actions/workflows/pylint.yml/badge.svg)](https://github.com/ylabonte/proconip-pypi/actions/workflows/pylint.yml)
 [![Unittest](https://github.com/ylabonte/proconip-pypi/actions/workflows/unittest.yml/badge.svg)](https://github.com/ylabonte/proconip-pypi/actions/workflows/unittest.yml)
+[![CodeQL](https://github.com/ylabonte/proconip-pypi/actions/workflows/codeql.yml/badge.svg)](https://github.com/ylabonte/proconip-pypi/actions/workflows/codeql.yml)
 [![PyPi Package release](https://github.com/ylabonte/proconip-pypi/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ylabonte/proconip-pypi/actions/workflows/python-publish.yml)
 
 [![PyPI](https://img.shields.io/pypi/v/proconip?label=Current%20Release)](https://pypi.org/project/proconip/)
 
 ## Overview
 
 * [Introduction (_What is this library for?_)](#introduction)
 * [Installation](#installation)
 * [Usage](#usage-examples)
   * [Reading the current state](#reading-the-current-state)
   * [Switching relays](#switching-relays)
 * [A brief description of the ProCon.IP pool controller](#a-brief-description-of-the-proconip-pool-controller)
 * [Get support](#get-support)
 * [Give support](#give-support)
+* [Release Notes](#release-notes)
 * [Disclaimer](#disclaimer)
 
 ---
 ![ProCon.IP Python Library](./logo.png)
 
 ## Introduction
 
@@ -187,13 +189,62 @@
 
 If you want to support this project or my work in general, you can do so without having any coding abilities.
 Because programmers are described as machines that convert coffee (their habitual input) into code (their habitual
 output), there is a really simple way to support me:
 
 [<img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 40px !important;width: 144px !important;" >](https://www.buymeacoffee.com/ylabonte)
 
+## Release Notes
+
+### v1.3.1 (2024-05-09)
+* Add dedicated `api.TimeoutException` to raise for connection timeouts.
+* Add dependabot with `versioning-strategy: "increase"` and an auto-merge workflow for automated updates on the github 
+  `main` branch.
+* Add code scanning (CodeQL) workflow.
+
+### v1.3.0 (2023-08-16)
+* Add `GetStateData.get_relays()` to get all available Relay instances.
+
+### v1.2.7 (2023-07-04)
+* Fix calculation formula for actual values (`offset + gain * raw`).
+
+### v1.2.6 (2023-06-20)
+* Fix DosageTarget enum and return value of `DosageControl.async_ph_plus_dosage`.
+
+### v1.2.5 (2023-06-18)
+* Fix return type/value of `DosageControl.async_ph_plus_dosage()`
+
+### v1.2.4 (2023-06-18)
+* Refactor request exception handling
+
+### v1.2.3 (2023-06-17)
+* Fix api methods to produce `BadCredentialsExceptions` in case of 401 and 403 responses.
+
+### v1.2.2 (2023-06-12)
+* Fix typo in `BadStatusCodeException`
+
+### v1.2.1 (2023-06-12)
+* Avoid invalid operations regarding dosage control relays.
+
+### v1.2.0 (2023-06-12)
+* Add DosageControl abilities.
+
+### v1.1.0 (2023-05-23)
+*  Unify api methods and naming conventions:
+  * Same names for functions and class methods with same functionality.
+  * `async_` prefixes for all async functions/methods.
+
+### v1.0.0 (2023-05-21)
+* Fix post data for switching relays.
+
+### v0.0.2 (2023-05-18)
+* Add relay switching capabilities.
+
+### v0.0.1 (2023-04-23)
+* Initial release with data reading capabilities.
+
 ## Disclaimer
 
 **Just to be clear: I have nothing to do with the development, selling, marketing or support of the pool controller
 unit itself.  
 I just developed small TypeScript/JS and Python libraries as by-products of an ioBroker adapter and a Home Assistant
 integration for integrating the pool controller unit with common smart home solutions.**
```

