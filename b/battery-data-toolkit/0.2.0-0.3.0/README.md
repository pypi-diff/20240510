# Comparing `tmp/battery-data-toolkit-0.2.0.tar.gz` & `tmp/battery_data_toolkit-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "battery-data-toolkit-0.2.0.tar", last modified: Mon Feb  5 20:58:10 2024, max compression
+gzip compressed data, was "battery_data_toolkit-0.3.0.tar", last modified: Mon Apr 22 12:31:54 2024, max compression
```

## Comparing `battery-data-toolkit-0.2.0.tar` & `battery_data_toolkit-0.3.0.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 20:58:10.684926 battery-data-toolkit-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-05 20:58:03.000000 battery-data-toolkit-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15117 2024-02-05 20:58:10.684926 battery-data-toolkit-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-02-05 20:58:03.000000 battery-data-toolkit-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 20:58:10.680926 battery-data-toolkit-0.2.0/batdata/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-05 20:58:03.000000 battery-data-toolkit-0.2.0/batdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-02-05 20:58:03.000000 battery-data-toolkit-0.2.0/batdata/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-02-05 20:58:03.000000 battery-data-toolkit-0.2.0/batdata/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 20:58:10.684926 battery-data-toolkit-0.2.0/batdata/extractors/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-05 20:58:03.000000 battery-data-toolkit-0.2.0/batdata/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-02-05 20:58:03.000000 battery-data-toolkit-0.2.0/batdata/extractors/arbin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-02-05 20:58:03.000000 battery-data-toolkit-0.2.0/batdata/extractors/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-02-05 20:58:03.000000 battery-data-toolkit-0.2.0/batdata/extractors/batteryarchive.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-02-05 20:58:03.000000 battery-data-toolkit-0.2.0/batdata/extractors/maccor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-02-05 20:58:03.000000 battery-data-toolkit-0.2.0/batdata/extractors/tIVT.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 20:58:10.684926 battery-data-toolkit-0.2.0/batdata/postprocess/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-05 20:58:03.000000 battery-data-toolkit-0.2.0/batdata/postprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-02-05 20:58:03.000000 battery-data-toolkit-0.2.0/batdata/postprocess/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-02-05 20:58:03.000000 battery-data-toolkit-0.2.0/batdata/postprocess/cycle_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-02-05 20:58:03.000000 battery-data-toolkit-0.2.0/batdata/postprocess/integral.py
--rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-02-05 20:58:03.000000 battery-data-toolkit-0.2.0/batdata/postprocess/tagging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 20:58:10.684926 battery-data-toolkit-0.2.0/batdata/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-02-05 20:58:03.000000 battery-data-toolkit-0.2.0/batdata/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-02-05 20:58:03.000000 battery-data-toolkit-0.2.0/batdata/schemas/battery.py
--rw-r--r--   0 runner    (1001) docker     (127)     9193 2024-02-05 20:58:03.000000 battery-data-toolkit-0.2.0/batdata/schemas/cycling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-02-05 20:58:03.000000 battery-data-toolkit-0.2.0/batdata/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-02-05 20:58:03.000000 battery-data-toolkit-0.2.0/batdata/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 20:58:10.684926 battery-data-toolkit-0.2.0/battery_data_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15117 2024-02-05 20:58:10.000000 battery-data-toolkit-0.2.0/battery_data_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-02-05 20:58:10.000000 battery-data-toolkit-0.2.0/battery_data_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 20:58:10.000000 battery-data-toolkit-0.2.0/battery_data_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-05 20:58:10.000000 battery-data-toolkit-0.2.0/battery_data_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-05 20:58:10.000000 battery-data-toolkit-0.2.0/battery_data_toolkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-02-05 20:58:03.000000 battery-data-toolkit-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-02-05 20:58:10.684926 battery-data-toolkit-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 20:58:10.684926 battery-data-toolkit-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-02-05 20:58:03.000000 battery-data-toolkit-0.2.0/tests/test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:31:54.813714 battery_data_toolkit-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-22 12:31:49.000000 battery_data_toolkit-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15094 2024-04-22 12:31:54.813714 battery_data_toolkit-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-22 12:31:49.000000 battery_data_toolkit-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:31:54.809714 battery_data_toolkit-0.3.0/batdata/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-22 12:31:49.000000 battery_data_toolkit-0.3.0/batdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-22 12:31:49.000000 battery_data_toolkit-0.3.0/batdata/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14136 2024-04-22 12:31:49.000000 battery_data_toolkit-0.3.0/batdata/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:31:54.809714 battery_data_toolkit-0.3.0/batdata/extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-22 12:31:49.000000 battery_data_toolkit-0.3.0/batdata/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-04-22 12:31:49.000000 battery_data_toolkit-0.3.0/batdata/extractors/arbin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-22 12:31:49.000000 battery_data_toolkit-0.3.0/batdata/extractors/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-22 12:31:49.000000 battery_data_toolkit-0.3.0/batdata/extractors/batteryarchive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6518 2024-04-22 12:31:49.000000 battery_data_toolkit-0.3.0/batdata/extractors/batterydata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-04-22 12:31:49.000000 battery_data_toolkit-0.3.0/batdata/extractors/maccor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-22 12:31:49.000000 battery_data_toolkit-0.3.0/batdata/extractors/tIVT.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:31:54.809714 battery_data_toolkit-0.3.0/batdata/postprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-22 12:31:49.000000 battery_data_toolkit-0.3.0/batdata/postprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-22 12:31:49.000000 battery_data_toolkit-0.3.0/batdata/postprocess/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-22 12:31:49.000000 battery_data_toolkit-0.3.0/batdata/postprocess/cycle_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-04-22 12:31:49.000000 battery_data_toolkit-0.3.0/batdata/postprocess/integral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-04-22 12:31:49.000000 battery_data_toolkit-0.3.0/batdata/postprocess/tagging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:31:54.809714 battery_data_toolkit-0.3.0/batdata/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-22 12:31:49.000000 battery_data_toolkit-0.3.0/batdata/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-22 12:31:49.000000 battery_data_toolkit-0.3.0/batdata/schemas/battery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10717 2024-04-22 12:31:49.000000 battery_data_toolkit-0.3.0/batdata/schemas/cycling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-22 12:31:49.000000 battery_data_toolkit-0.3.0/batdata/schemas/eis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-22 12:31:49.000000 battery_data_toolkit-0.3.0/batdata/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-22 12:31:49.000000 battery_data_toolkit-0.3.0/batdata/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:31:54.813714 battery_data_toolkit-0.3.0/battery_data_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15094 2024-04-22 12:31:54.000000 battery_data_toolkit-0.3.0/battery_data_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-22 12:31:54.000000 battery_data_toolkit-0.3.0/battery_data_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 12:31:54.000000 battery_data_toolkit-0.3.0/battery_data_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-22 12:31:54.000000 battery_data_toolkit-0.3.0/battery_data_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-22 12:31:54.000000 battery_data_toolkit-0.3.0/battery_data_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-22 12:31:49.000000 battery_data_toolkit-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-22 12:31:54.813714 battery_data_toolkit-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:31:54.813714 battery_data_toolkit-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-22 12:31:49.000000 battery_data_toolkit-0.3.0/tests/test_data.py
```

### Comparing `battery-data-toolkit-0.2.0/LICENSE` & `battery_data_toolkit-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `battery-data-toolkit-0.2.0/PKG-INFO` & `battery_data_toolkit-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: battery-data-toolkit
-Version: 0.2.0
+Version: 0.3.0
 Summary: Utilities for reading and manipulating battery testing data
 Author-email: Logan Ward <lward@anl.gov>, Noah Paulson <lward@anl.gov>, Joseph Kubal <kubal@anl.gov>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -212,24 +212,25 @@
 License-File: LICENSE
 Requires-Dist: pandas>1.0
 Requires-Dist: scipy>1.3
 Requires-Dist: pydantic==2.*
 Requires-Dist: tables>3.6
 Requires-Dist: h5py==3.*
 Requires-Dist: scythe-extractors>=0.1
+Requires-Dist: pyarrow>=15
 Requires-Dist: xlrd
 Provides-Extra: test
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 
 # Battery Data Toolkit
 
-[![Python Package](https://github.com/materials-data-facility/battery-data-toolkit/actions/workflows/python-package.yml/badge.svg)](https://github.com/materials-data-facility/battery-data-toolkit/actions/workflows/python-package.yml)
-[![Coverage Status](https://coveralls.io/repos/github/materials-data-facility/battery-data-toolkit/badge.svg)](https://coveralls.io/github/materials-data-facility/battery-data-toolkit?branch=master)
+[![Python Package](https://github.com/rovi-org/battery-data-toolkit/actions/workflows/python-package.yml/badge.svg)](https://github.com/rovi-org/battery-data-toolkit/actions/workflows/python-package.yml)
+[![Coverage Status](https://coveralls.io/repos/github/ROVI-org/battery-data-toolkit/badge.svg?branch=main)](https://coveralls.io/github/ROVI-org/battery-data-toolkit?branch=main)
 [![PyPI version](https://badge.fury.io/py/battery-data-toolkit.svg)](https://badge.fury.io/py/battery-data-toolkit)
 
 The battery-data-toolkit, `batdata`, converts battery testing data from native formats to a standardized HDF5 file.
 These HDF5 files contain the metadata needed to understand the source of the data, 
 and can be easily manipulated by common analysis libraries (e.g., Pandas).
 
 This repository also contains [example scripts](./scripts) for converting datasets to the HDF5 format.
```

### Comparing `battery-data-toolkit-0.2.0/batdata/cli.py` & `battery_data_toolkit-0.3.0/batdata/cli.py`

 * *Files identical despite different names*

### Comparing `battery-data-toolkit-0.2.0/batdata/extractors/arbin.py` & `battery_data_toolkit-0.3.0/batdata/extractors/arbin.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         df_out = pd.DataFrame()
 
         # Convert the column names
         df_out['cycle_number'] = df['Cycle_Index'] + start_cycle - df['Cycle_Index'].min()
         df_out['cycle_number'] = df_out['cycle_number'].astype('int64')
         df_out['file_number'] = file_number  # df_out['cycle_number']*0
         df_out['test_time'] = np.array(df['test_time'] - df['test_time'][0] + start_time, dtype=float)
-        df_out['current'] = df['Current']
+        df_out['current'] = -df['Current']
         df_out['temperature'] = df['Temperature']
         df_out['internal_resistance'] = df['Internal_Resistance']
         df_out['voltage'] = df['Voltage']
 
         # Drop the duplicate rows
         df_out = drop_cycles(df_out)
```

### Comparing `battery-data-toolkit-0.2.0/batdata/extractors/base.py` & `battery_data_toolkit-0.3.0/batdata/extractors/base.py`

 * *Files identical despite different names*

### Comparing `battery-data-toolkit-0.2.0/batdata/extractors/batteryarchive.py` & `battery_data_toolkit-0.3.0/batdata/extractors/batteryarchive.py`

 * *Files identical despite different names*

### Comparing `battery-data-toolkit-0.2.0/batdata/extractors/maccor.py` & `battery_data_toolkit-0.3.0/batdata/extractors/maccor.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
         # fill in new dataframe
         df_out['cycle_number'] = df['Cyc#'] + start_cycle - df['Cyc#'].min()
         df_out['cycle_number'] = df_out['cycle_number'].astype('int64')
         df_out['file_number'] = file_number  # df_out['cycle_number']*0
         df_out['test_time'] = df['Test (Min)'] * 60 - df['Test (Min)'].iloc[0] * 60 + start_time
         df_out['state'] = df['State']
-        df_out['current'] = df['Amps']
+        df_out['current'] = -df['Amps']
         df_out['current'] = np.where(df['State'] == 'D', -1 * df_out['current'], df_out['current'])
         #   0 is rest, 1 is charge, -1 is discharge
         df_out.loc[df_out['state'] == 'R', 'state'] = ChargingState.hold
         df_out.loc[df_out['state'] == 'C', 'state'] = ChargingState.charging
         df_out.loc[df_out['state'] == 'D', 'state'] = ChargingState.discharging
         df_out.loc[df_out['state'] == 'O', 'state'] = ChargingState.unknown
         df_out.loc[df_out['state'] == 'S', 'state'] = ChargingState.unknown
```

### Comparing `battery-data-toolkit-0.2.0/batdata/extractors/tIVT.py` & `battery_data_toolkit-0.3.0/batdata/extractors/tIVT.py`

 * *Files identical despite different names*

### Comparing `battery-data-toolkit-0.2.0/batdata/postprocess/base.py` & `battery_data_toolkit-0.3.0/batdata/postprocess/base.py`

 * *Files identical despite different names*

### Comparing `battery-data-toolkit-0.2.0/batdata/postprocess/tagging.py` & `battery_data_toolkit-0.3.0/batdata/postprocess/tagging.py`

 * *Files identical despite different names*

### Comparing `battery-data-toolkit-0.2.0/batdata/schemas/__init__.py` & `battery_data_toolkit-0.3.0/batdata/schemas/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,7 +38,8 @@
     associated_ids: Optional[List[AnyUrl]] = Field(None, description="Any identifiers associated with this data file."
                                                                      " Identifiers can be any URI, such as DOIs of associated"
                                                                      " paper or HTTP addresses of associated websites")
 
     # Description of additional columns
     raw_data_columns: Dict[str, str] = Field(default_factory=dict, description='Descriptions of non-standard columns in the raw data')
     cycle_stats_columns: Dict[str, str] = Field(default_factory=dict, description='Descriptions of non-standard columns in the cycle stats')
+    eis_data_columns: Dict[str, str] = Field(default_factory=dict, description='Descriptions of non-standard columns in the EIS data')
```

### Comparing `battery-data-toolkit-0.2.0/batdata/schemas/battery.py` & `battery_data_toolkit-0.3.0/batdata/schemas/battery.py`

 * *Files identical despite different names*

### Comparing `battery-data-toolkit-0.2.0/batdata/schemas/cycling.py` & `battery_data_toolkit-0.3.0/batdata/schemas/cycling.py`

 * *Files 10% similar despite different names*

```diff
@@ -134,14 +134,15 @@
                                                     " or resting.")
     file_number: List[int] = Field(None, description="Used if test data is stored in multiple files. Number represents "
                                                      "the index of the file. All indices should be nonnegative and "
                                                      "monotonically increasing", monotonic=True)
     test_time: List[float] = Field(..., description="Time from the beginning of the cycling test. Times must be "
                                                     "nonnegative and monotonically increasing. Units: s",
                                    monotonic=True)
+    time: List[float] = Field(None, description="Time as a UNIX timestamp. Assumed to be in UTC")
     voltage: List[float] = Field(..., description="Measured voltage of the system. Units: V")
     current: List[float] = Field(..., description="Measured current of the system. Positive current represents "
                                                   "the battery discharging and negative represents the battery"
                                                   "charging. Units: A")
     state: List[ChargingState] = Field(None, description="Determination of whether the battery is being charged, "
                                                          "discharged or held at a constant charge")
     method: List[ControlMethod] = Field(None, description="List of the method used to control "
@@ -149,31 +150,48 @@
     temperature: List[float] = Field(None, description="Temperature of the battery. Units: C")
     internal_resistance: List[float] = Field(None, description="Internal resistance of the battery. Units: ohm")
     substep_index: List[int] = Field(None, description="Index of the substep within a testing cycle. A substep"
                                                        " change is defined by a change of the charging or discharging"
                                                        " method, such as change from constant voltage to"
                                                        " constant current")
 
+    # Derived quantities
+    cycle_capacity: List[float] = Field(None,
+                                        description="Cumulative change in amount of charge transferred from a battery since the start of a cycle. "
+                                                    "Positive values indicate the battery has discharged since the start of the cycle."
+                                        )
+    cycle_energy: List[float] = Field(None,
+                                      description="Cumulative change in amount of energy transferred from a battery the start of a cycle. "
+                                                  "Positive values indicate the battery has discharged more than since the start of the cycle."
+                                      )
+
 
 class CycleLevelData(ColumnSchema):
     """Statistics about the performance of a cell over a certain cycle"""
 
     # Related to time
     cycle_number: List[int] = Field(..., description='Index of the cycle', monotonic=True)
+    cycle_start: List[float] = Field(None, description='Time since the first data point recorded for this battery for the start of this cycle. Units: s')
+    cycle_duration: List[float] = Field(None, description='Duration of this cycle. Units: s')
 
     # Related to the total amount of energy or electrons moved
-    discharge_capacity: List[float] = Field(None, description='Total amount of electrons moved during discharge. Units: A-hr')
-    discharge_energy: List[float] = Field(None, description='Total amount of energy released during discharge. Units: A-hr')
-    charge_capacity: List[float] = Field(None, description='Total amount of electrons moved during charge. Units: J')
-    charge_energy: List[float] = Field(None, description='Total amount of energy stored during charge. Units: J')
-    coulomb_efficiency: List[float] = Field(None, description='Fraction of electrons that are lost during charge and recharge. Units: %')
+    capacity_discharge: List[float] = Field(None, description='Total amount of electrons released during discharge. Units: A-hr')
+    energy_discharge: List[float] = Field(None, description='Total amount of energy released during discharge. Units: W-hr')
+    capacity_charge: List[float] = Field(None, description='Total amount of electrons stored during charge. Units: A-hr')
+    energy_charge: List[float] = Field(None, description='Total amount of energy stored during charge. Units: W-hr')
+    coulomb_efficiency: List[float] = Field(None, description='Fraction of electric charge that is lost during charge and recharge. Units: %')
     energy_efficiency: List[float] = Field(None, description='Amount of energy lost during charge and discharge')
 
     # Related to voltage
     discharge_V_average: List[float] = Field(None, description='Average voltage during discharging. Units: V')
     charge_V_average: List[float] = Field(None, description='Average voltage during charge. Units: V')
     V_maximum: List[float] = Field(None, description='Maximum voltage during cycle. Units: V')
     V_minimum: List[float] = Field(None, description='Minimum voltage during cycle. Units: V')
 
     # Related to current
     discharge_I_average: List[float] = Field(None, description='Average current during discharge. Units: A')
     charge_I_average: List[float] = Field(None, description='Average current during charge. Units: A')
+
+    # Temperature
+    temperature_minimum: List[float] = Field(None, description='Minimum observed battery temperature during cycle. Units: C')
+    temperature_maximum: List[float] = Field(None, description='Maximum observed battery temperature during cycle. Units: C')
+    temperature_average: List[float] = Field(None, description='Average observed battery temperature during cycle. Units: C')
```

### Comparing `battery-data-toolkit-0.2.0/batdata/utils.py` & `battery_data_toolkit-0.3.0/batdata/utils.py`

 * *Files identical despite different names*

### Comparing `battery-data-toolkit-0.2.0/battery_data_toolkit.egg-info/PKG-INFO` & `battery_data_toolkit-0.3.0/battery_data_toolkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: battery-data-toolkit
-Version: 0.2.0
+Version: 0.3.0
 Summary: Utilities for reading and manipulating battery testing data
 Author-email: Logan Ward <lward@anl.gov>, Noah Paulson <lward@anl.gov>, Joseph Kubal <kubal@anl.gov>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -212,24 +212,25 @@
 License-File: LICENSE
 Requires-Dist: pandas>1.0
 Requires-Dist: scipy>1.3
 Requires-Dist: pydantic==2.*
 Requires-Dist: tables>3.6
 Requires-Dist: h5py==3.*
 Requires-Dist: scythe-extractors>=0.1
+Requires-Dist: pyarrow>=15
 Requires-Dist: xlrd
 Provides-Extra: test
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 
 # Battery Data Toolkit
 
-[![Python Package](https://github.com/materials-data-facility/battery-data-toolkit/actions/workflows/python-package.yml/badge.svg)](https://github.com/materials-data-facility/battery-data-toolkit/actions/workflows/python-package.yml)
-[![Coverage Status](https://coveralls.io/repos/github/materials-data-facility/battery-data-toolkit/badge.svg)](https://coveralls.io/github/materials-data-facility/battery-data-toolkit?branch=master)
+[![Python Package](https://github.com/rovi-org/battery-data-toolkit/actions/workflows/python-package.yml/badge.svg)](https://github.com/rovi-org/battery-data-toolkit/actions/workflows/python-package.yml)
+[![Coverage Status](https://coveralls.io/repos/github/ROVI-org/battery-data-toolkit/badge.svg?branch=main)](https://coveralls.io/github/ROVI-org/battery-data-toolkit?branch=main)
 [![PyPI version](https://badge.fury.io/py/battery-data-toolkit.svg)](https://badge.fury.io/py/battery-data-toolkit)
 
 The battery-data-toolkit, `batdata`, converts battery testing data from native formats to a standardized HDF5 file.
 These HDF5 files contain the metadata needed to understand the source of the data, 
 and can be easily manipulated by common analysis libraries (e.g., Pandas).
 
 This repository also contains [example scripts](./scripts) for converting datasets to the HDF5 format.
```

### Comparing `battery-data-toolkit-0.2.0/battery_data_toolkit.egg-info/SOURCES.txt` & `battery_data_toolkit-0.3.0/battery_data_toolkit.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -7,23 +7,25 @@
 batdata/data.py
 batdata/utils.py
 batdata/version.py
 batdata/extractors/__init__.py
 batdata/extractors/arbin.py
 batdata/extractors/base.py
 batdata/extractors/batteryarchive.py
+batdata/extractors/batterydata.py
 batdata/extractors/maccor.py
 batdata/extractors/tIVT.py
 batdata/postprocess/__init__.py
 batdata/postprocess/base.py
 batdata/postprocess/cycle_stats.py
 batdata/postprocess/integral.py
 batdata/postprocess/tagging.py
 batdata/schemas/__init__.py
 batdata/schemas/battery.py
 batdata/schemas/cycling.py
+batdata/schemas/eis.py
 battery_data_toolkit.egg-info/PKG-INFO
 battery_data_toolkit.egg-info/SOURCES.txt
 battery_data_toolkit.egg-info/dependency_links.txt
 battery_data_toolkit.egg-info/requires.txt
 battery_data_toolkit.egg-info/top_level.txt
 tests/test_data.py
```

### Comparing `battery-data-toolkit-0.2.0/pyproject.toml` & `battery_data_toolkit-0.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "battery-data-toolkit"
-version = "0.2.0"
+version = "0.3.0"
 description = "Utilities for reading and manipulating battery testing data"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = 'LICENSE'}
 keywords = ["batteries", "science", "data science"]
 authors = [
     {name = "Logan Ward", email = "lward@anl.gov"},
@@ -14,14 +14,15 @@
 dependencies = [
     "pandas > 1.0",
     "scipy > 1.3",
     "pydantic == 2.*",
     "tables > 3.6",
     "h5py == 3.*",
     "scythe-extractors >= 0.1",
+    "pyarrow >= 15",
     "xlrd"
 ]
 
 [tool.setuptools.packages.find]
 include = ["batdata*"]
 
 [project.optional-dependencies]
```

