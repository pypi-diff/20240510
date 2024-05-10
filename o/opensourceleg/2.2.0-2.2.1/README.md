# Comparing `tmp/opensourceleg-2.2.0.tar.gz` & `tmp/opensourceleg-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensourceleg-2.2.0.tar", max compression
+gzip compressed data, was "opensourceleg-2.2.1.tar", max compression
```

## Comparing `opensourceleg-2.2.0.tar` & `opensourceleg-2.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    26526 2024-03-11 16:37:38.238392 opensourceleg-2.2.0/LICENSE
--rw-r--r--   0        0        0     4158 2024-04-11 18:15:50.369362 opensourceleg-2.2.0/README.md
--rw-r--r--   0        0        0      415 2023-10-12 15:36:40.401967 opensourceleg-2.2.0/opensourceleg/__init__.py
--rw-r--r--   0        0        0        0 2023-10-20 14:42:08.002099 opensourceleg-2.2.0/opensourceleg/control/__init__.py
--rw-r--r--   0        0        0     7309 2024-04-22 16:55:56.739331 opensourceleg-2.2.0/opensourceleg/control/compiled_controller.py
--rw-r--r--   0        0        0    15826 2024-04-22 16:55:56.739869 opensourceleg-2.2.0/opensourceleg/control/state_machine.py
--rw-r--r--   0        0        0        0 2023-10-20 14:42:08.002819 opensourceleg-2.2.0/opensourceleg/hardware/__init__.py
--rw-r--r--   0        0        0    34576 2024-05-06 17:40:50.560221 opensourceleg-2.2.0/opensourceleg/hardware/actuators.py
--rw-r--r--   0        0        0    12842 2024-05-06 17:26:49.228964 opensourceleg-2.2.0/opensourceleg/hardware/joints.py
--rw-r--r--   0        0        0    19890 2024-05-06 17:36:59.460237 opensourceleg-2.2.0/opensourceleg/hardware/sensors.py
--rw-r--r--   0        0        0     6501 2024-04-22 16:55:56.743110 opensourceleg-2.2.0/opensourceleg/hardware/thermal.py
--rw-r--r--   0        0        0    14085 2024-05-06 17:36:33.700442 opensourceleg-2.2.0/opensourceleg/osl.py
--rw-r--r--   0        0        0     6352 2024-05-06 17:36:33.057100 opensourceleg-2.2.0/opensourceleg/safety/sensors.py
--rw-r--r--   0        0        0        0 2023-10-20 14:42:08.003682 opensourceleg-2.2.0/opensourceleg/tools/__init__.py
--rw-r--r--   0        0        0     5920 2024-05-06 17:18:03.548467 opensourceleg-2.2.0/opensourceleg/tools/logger.py
--rw-r--r--   0        0        0     4093 2024-04-22 16:55:56.744516 opensourceleg-2.2.0/opensourceleg/tools/units.py
--rw-r--r--   0        0        0    11696 2024-04-22 16:57:48.693201 opensourceleg-2.2.0/opensourceleg/tools/utilities.py
--rw-r--r--   0        0        0     3797 2024-05-06 17:39:28.083443 opensourceleg-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     5329 1970-01-01 00:00:00.000000 opensourceleg-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0    26526 2024-03-11 16:37:38.238392 opensourceleg-2.2.1/LICENSE
+-rw-r--r--   0        0        0     4158 2024-04-11 18:15:50.369362 opensourceleg-2.2.1/README.md
+-rw-r--r--   0        0        0      415 2024-05-09 15:50:27.884468 opensourceleg-2.2.1/opensourceleg/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-20 14:42:08.002099 opensourceleg-2.2.1/opensourceleg/control/__init__.py
+-rw-r--r--   0        0        0     7338 2024-05-09 18:06:59.695622 opensourceleg-2.2.1/opensourceleg/control/compiled_controller.py
+-rw-r--r--   0        0        0    15826 2024-05-09 17:45:46.152874 opensourceleg-2.2.1/opensourceleg/control/state_machine.py
+-rw-r--r--   0        0        0        0 2023-10-20 14:42:08.002819 opensourceleg-2.2.1/opensourceleg/hardware/__init__.py
+-rw-r--r--   0        0        0    34576 2024-05-10 16:14:44.189147 opensourceleg-2.2.1/opensourceleg/hardware/actuators.py
+-rw-r--r--   0        0        0    12842 2024-05-09 17:45:46.155321 opensourceleg-2.2.1/opensourceleg/hardware/joints.py
+-rw-r--r--   0        0        0    18657 2024-05-09 18:09:04.803763 opensourceleg-2.2.1/opensourceleg/hardware/sensors.py
+-rw-r--r--   0        0        0     6501 2024-05-09 17:45:46.156509 opensourceleg-2.2.1/opensourceleg/hardware/thermal.py
+-rw-r--r--   0        0        0    14050 2024-05-10 15:12:41.707497 opensourceleg-2.2.1/opensourceleg/osl.py
+-rw-r--r--   0        0        0        0 2023-10-20 14:42:08.003682 opensourceleg-2.2.1/opensourceleg/tools/__init__.py
+-rw-r--r--   0        0        0     6118 2024-05-09 18:03:32.381356 opensourceleg-2.2.1/opensourceleg/tools/logger.py
+-rw-r--r--   0        0        0    11152 2024-05-10 18:31:45.314381 opensourceleg-2.2.1/opensourceleg/tools/safety.py
+-rw-r--r--   0        0        0     4093 2024-05-09 17:45:46.159157 opensourceleg-2.2.1/opensourceleg/tools/units.py
+-rw-r--r--   0        0        0    11788 2024-05-09 17:45:46.159817 opensourceleg-2.2.1/opensourceleg/tools/utilities.py
+-rw-r--r--   0        0        0     3797 2024-05-10 18:32:42.115503 opensourceleg-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5329 1970-01-01 00:00:00.000000 opensourceleg-2.2.1/PKG-INFO
```

### Comparing `opensourceleg-2.2.0/LICENSE` & `opensourceleg-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opensourceleg-2.2.0/README.md` & `opensourceleg-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `opensourceleg-2.2.0/opensourceleg/control/compiled_controller.py` & `opensourceleg-2.2.1/opensourceleg/control/compiled_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,21 +11,23 @@
     This class expects that your function has the form: myFunction(*inputs, *outputs)
     where *inputs is a pointer to an inputs structure and
     *outputs is a pointer to an outputs structure.
     You can define these input and output structures however you please.
     See examples folder of repo for examples.
 
     Parameters:
+    -----------
         library_name (string): The name of the compiled library file, without the *.so
         library_path (string): The path to the directory containing the library. See examples for how to get working directory of parent script.
         main_function_name (string): Name of the main function to call within the library. This is the function that will get called via the run() method
         initialization_function_name (string): Name of an initialization function for your library. This gets called only once when the library is loaded. If you don't have an initialization function, pass None.
         cleanup_function_name (string): Name of a cleanup function for your library. This gets called when the CompiledController class has gone out of scope and is garbage collected. Again, pass None if you don't need this functionality.
 
     Authors:
+    --------
         Kevin Best, Senthur Raj Ayyappan
         Neurobionics Lab
         Robotics Department
         University of Michigan
         October 2023
     """
```

### Comparing `opensourceleg-2.2.0/opensourceleg/control/state_machine.py` & `opensourceleg-2.2.1/opensourceleg/control/state_machine.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-2.2.0/opensourceleg/hardware/actuators.py` & `opensourceleg-2.2.1/opensourceleg/hardware/actuators.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-2.2.0/opensourceleg/hardware/joints.py` & `opensourceleg-2.2.1/opensourceleg/hardware/joints.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-2.2.0/opensourceleg/hardware/sensors.py` & `opensourceleg-2.2.1/opensourceleg/hardware/sensors.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,22 +63,14 @@
         self.is_streaming = True
         self.data: list[int] = []
         self.failed_reads = 0
 
     def __repr__(self) -> str:
         return f"StrainAmp"
 
-    def read_uncompressed_strain(self):
-        """Used for an older version of the strain amp firmware (at least pre-2017)"""
-        data = []
-        for i in range(self.MEM_R_CH1_H, self.MEM_R_CH6_L + 1):
-            data.append(self._SMBus.read_byte_data(self.addr, i))
-
-        return self._unpack_uncompressed_strain(data)
-
     def _read_compressed_strain(self):
         """Used for more recent versions of strain amp firmware"""
         try:
             self.data = self._SMBus.read_i2c_block_data(self.addr, self.MEM_R_CH1_H, 10)
             self.failed_reads = 0
         except OSError as e:
             self.failed_reads += 1
@@ -117,34 +109,14 @@
                 (data[3] << 4) | ((data[4] >> 4) & 0x0F),
                 ((data[4] << 8) & 0x0F00) | data[5],
                 (data[6] << 4) | ((data[7] >> 4) & 0x0F),
                 ((data[7] << 8) & 0x0F00) | data[8],
             ]
         )
 
-    @staticmethod
-    def strain_data_to_wrench(
-        unpacked_strain, loadcell_matrix, loadcell_zero, exc=5, gain=125
-    ):
-        """Converts strain values between 0 and 4095 to a wrench in N and Nm"""
-        loadcell_signed = (unpacked_strain - 2048) / 4095 * exc
-        loadcell_coupled = loadcell_signed * 1000 / (exc * gain)
-        return np.reshape(
-            np.transpose(a=loadcell_matrix.dot(np.transpose(a=loadcell_coupled)))
-            - loadcell_zero,
-            (6,),
-        )
-
-    @staticmethod
-    def wrench_to_strain_data(measurement, loadcell_matrix, exc=5, gain=125):
-        """Wrench in N and Nm to the strain values that would give that wrench"""
-        loadcell_coupled = (np.linalg.inv(loadcell_matrix)).dot(measurement)
-        loadcell_signed = loadcell_coupled * (exc * gain) / 1000
-        return ((loadcell_signed / exc) * 4095 + 2048).round(0).astype(int)
-
 
 class Loadcell:
     def __init__(
         self,
         dephy_mode: bool = False,
         joint: Joint = None,
         amp_gain: float = 125.0,
```

### Comparing `opensourceleg-2.2.0/opensourceleg/hardware/thermal.py` & `opensourceleg-2.2.1/opensourceleg/hardware/thermal.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-2.2.0/opensourceleg/osl.py` & `opensourceleg-2.2.1/opensourceleg/osl.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         Initialize the OSL class.
 
         Parameters
         ----------
         frequency : int, optional
             The frequency of the control loop, by default 200
         file_name : str, optional
-            The name of the log file, by default "./osl.log"
+            The name of the log file (without the extension), by default "./osl"
         """
 
         self._frequency: int = frequency
 
         self._has_knee: bool = False
         self._has_ankle: bool = False
         self._has_loadcell: bool = False
@@ -322,15 +322,14 @@
                     logger=self.log,
                 )
 
             self._has_loadcell = True
 
     def update(
         self,
-        log_data: bool = False,
     ) -> None:
         if self.has_knee:
             self._knee.update()
 
             if self.knee.case_temperature > self.knee.max_temperature:
                 self.log.warning(
                     msg=f"[KNEE] Thermal limit {self.knee.max_temperature} reached. Stopping motor."
@@ -347,16 +346,15 @@
                 )
                 self.__exit__()
                 exit()
 
         if self.has_loadcell:
             self._loadcell.update()
 
-        if log_data:
-            self.log.data()
+        self.log.update()
 
         if hasattr(self, "_safety_attributes"):
             for safety_attribute_name in self._safety_attributes:
                 self.log.debug(
                     msg=f"[{self.__repr__()}] Safety mechanism in-place for {safety_attribute_name}: {getattr(self, safety_attribute_name)}"
                 )
```

### Comparing `opensourceleg-2.2.0/opensourceleg/tools/logger.py` & `opensourceleg-2.2.1/opensourceleg/tools/logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 Usage Guide:
 
 1. Create an instance of the `Logger` class.
 2. Optionally, set the logging levels for file and stream handlers using
    `set_file_level` and `set_stream_level` methods.
 3. Add class instances and attributes to log using the `add_attributes` method.
-4. Start logging data using the `data` method.
+4. Start logging data using the `update` method.
 5. Optionally, close the CSV file using the `close` method.
 
 Note:
 
 This file is referenced by the OSL class and is instantiated manually when an OSL
 is instantiated.
 
@@ -82,14 +82,17 @@
         self._stream_handler.setFormatter(fmt=self._std_formatter)
 
         self.addHandler(hdlr=self._stream_handler)
         self.addHandler(hdlr=self._file_handler)
 
         self._is_logging = False
 
+        self._header_data: list[str] = []
+        self._data: list[Any] = []
+
     def __repr__(self) -> str:
         return f"Logger"
 
     def set_file_level(self, level: str = "DEBUG") -> None:
         """
         Sets the level of the logger
 
@@ -123,52 +126,55 @@
             container (object, dict): Container can either be an object (instance of a class)
                 or a Dict containing the attributes to be logged.
             attributes (list[str]): List of attributes to log
         """
         self._containers.append(container)
         self._attributes.append(attributes)
 
-    def data(self) -> None:
+    def update(self) -> None:
         """
         Logs the attributes of the class instance to the csv file
         """
-        header_data = []
-        data = []
+        if not self._containers:
+            return
 
         if not self._is_logging:
             for container, attributes in zip(self._containers, self._attributes):
                 for attribute in attributes:
                     if type(container) is dict:
                         if "__main__" in container.values():
-                            header_data.append(f"{attribute}")
+                            self._header_data.append(f"{attribute}")
                         else:
-                            header_data.append(f"{container}:{attribute}")
+                            self._header_data.append(f"{container}:{attribute}")
                     else:
                         if type(container).__repr__ is not object.__repr__:
-                            header_data.append(f"{container}:{attribute}")
+                            self._header_data.append(f"{container}:{attribute}")
                         else:
-                            header_data.append(f"{attribute}")
+                            self._header_data.append(f"{attribute}")
 
-            self._writer.writerow(header_data)
+            self._writer.writerow(self._header_data)
             self._is_logging = True
 
         for container, attributes in zip(self._containers, self._attributes):
             if isinstance(container, dict):
                 for attribute in attributes:
-                    data.append(container.get(attribute))
+                    self._data.append(container.get(attribute))
             else:
                 for attribute in attributes:
-                    data.append(getattr(container, attribute))
+                    self._data.append(getattr(container, attribute))
+
+        self._writer.writerow(self._data)
 
-        self._writer.writerow(data)
+        self._data.clear()
+        self._header_data.clear()
         self._file.flush()
 
-    def close(self) -> None:
+    def __del__(self) -> None:
         """
-        Closes the csv file
+        Closes the file when the object is deleted
         """
         self._file.close()
 
 
 if __name__ == "__main__":
     local_logger = Logger(file_path="./test_log")
     local_variable_1 = 100
@@ -182,11 +188,9 @@
 
         def __repr__(self) -> str:
             return f"SimpleClass"
 
     simple_class = SimpleClass()
 
     local_logger.add_attributes(locals(), ["local_variable_1"])
-    # local_logger.add_attributes(simple_class, ["a", "b", "c"])
-    local_logger.data()
-
-    print(locals().__eq__)
+    local_logger.add_attributes(simple_class, ["a", "b", "c"])
+    local_logger.update()
```

### Comparing `opensourceleg-2.2.0/opensourceleg/tools/units.py` & `opensourceleg-2.2.1/opensourceleg/tools/units.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-2.2.0/opensourceleg/tools/utilities.py` & `opensourceleg-2.2.1/opensourceleg/tools/utilities.py`

 * *Files 16% similar despite different names*

```diff
@@ -44,42 +44,42 @@
 
     def handle_signal(self, signum, frame):
         self.kill_now = True
 
     def get_fade(self):
         # interpolates from 1 to zero with soft fade out
         if self._kill_soon:
-            t = time.time() - self._soft_kill_time
+            t = time.monotonic() - self._soft_kill_time
             if t >= self._fade_time:
                 return 0.0
             return 1.0 - (t / self._fade_time)
         return 1.0
 
     _kill_now = False
     _kill_soon = False
 
     @property
     def kill_now(self):
         if self._kill_now:
             return True
         if self._kill_soon:
-            t = time.time() - self._soft_kill_time
+            t = time.monotonic() - self._soft_kill_time
             if t > self._fade_time:
                 self._kill_now = True
         return self._kill_now
 
     @kill_now.setter
     def kill_now(self, val):
         if val:
             if self._kill_soon:  # if you kill twice, then it becomes immediate
                 self._kill_now = True
             else:
                 if self._fade_time > 0.0:
                     self._kill_soon = True
-                    self._soft_kill_time = time.time()
+                    self._soft_kill_time = time.monotonic()
                 else:
                     self._kill_now = True
         else:
             self._kill_now = False
             self._kill_soon = False
             self._soft_kill_time = None
 
@@ -102,15 +102,15 @@
 
     # Author: Gray C. Thomas, Ph.D
     # https://github.com/GrayThomas, https://graythomas.github.io
 
     """
 
     def __init__(self, dt=0.001, report=False, fade=0.0):
-        self.t0 = self.t1 = time.time()
+        self.t0 = self.t1 = time.monotonic()
         self.killer = LoopKiller(fade_time=fade)
         self.dt = dt
         self.ttarg = None
         self.sum_err = 0.0
         self.sum_var = 0.0
         self.sleep_t_agg = 0.0
         self.n = 0
@@ -135,70 +135,71 @@
     @property
     def fade(self):
         return self.killer.get_fade()
 
     def run(self, function_in_loop, dt=None):
         if dt is None:
             dt = self.dt
-        self.t0 = self.t1 = time.time() + dt
+        self.t0 = self.t1 = time.monotonic() + dt
         while not self.killer.kill_now:
             ret = function_in_loop()
             if ret == 0:
                 self.stop()
-            while time.time() < self.t1 and not self.killer.kill_now:
+            while time.monotonic() < self.t1 and not self.killer.kill_now:
                 if signal.sigtimedwait(
                     [signal.SIGTERM, signal.SIGINT, signal.SIGHUP], 0
                 ):
                     self.stop()
             self.t1 += dt
 
     def stop(self):
         self.killer.kill_now = True
 
     def time(self):
-        return time.time() - self.t0
+        return time.monotonic() - self.t0
 
     def time_since(self):
-        return time.time() - self.t1
+        return time.monotonic() - self.t1
 
     def __iter__(self):
-        self.t0 = self.t1 = time.time() + self.dt
+        self.t0 = self.t1 = time.monotonic() + self.dt
         return self
 
     def __next__(self):
         if self.killer.kill_now:
             raise StopIteration
 
         while (
-            time.time() < self.t1 - 2 * PRECISION_OF_SLEEP and not self.killer.kill_now
+            time.monotonic() < self.t1 - 2 * PRECISION_OF_SLEEP
+            and not self.killer.kill_now
         ):
-            t_pre_sleep = time.time()
+            t_pre_sleep = time.monotonic()
             time.sleep(
-                max(PRECISION_OF_SLEEP, self.t1 - time.time() - PRECISION_OF_SLEEP)
+                max(PRECISION_OF_SLEEP, self.t1 - time.monotonic() - PRECISION_OF_SLEEP)
             )
-            self.sleep_t_agg += time.time() - t_pre_sleep
+            self.sleep_t_agg += time.monotonic() - t_pre_sleep
 
-        while time.time() < self.t1 and not self.killer.kill_now:
+        while time.monotonic() < self.t1 and not self.killer.kill_now:
             try:
                 if signal.sigtimedwait(
                     [signal.SIGTERM, signal.SIGINT, signal.SIGHUP], 0
                 ):
                     self.stop()
             except AttributeError:
                 pass
 
         if self.killer.kill_now:
             raise StopIteration
         self.t1 += self.dt
         if self.ttarg is None:
             # inits ttarg on first call
-            self.ttarg = time.time() + self.dt
+            self.ttarg = time.monotonic() + self.dt
             # then skips the first loop
             return self.t1 - self.t0
-        error = time.time() - self.ttarg  # seconds
+        error = time.monotonic() - self.ttarg  # seconds
         self.sum_err += error
         self.sum_var += error**2
         self.n += 1
         self.ttarg += self.dt
         return self.t1 - self.t0
```

### Comparing `opensourceleg-2.2.0/pyproject.toml` & `opensourceleg-2.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "opensourceleg"
-version = "2.2.0"
+version = "2.2.1"
 description = "An open-source software library for numerical computation, data acquisition, and control of lower-limb robotic prostheses."
 readme = "README.md"
 authors = ["Open-source Leg <opensourceleg@gmail.com>"]
 license = "GNU LGPL v2.1"
 repository = "https://github.com/neurobionics/opensourceleg"
 homepage = "https://github.com/neurobionics/opensourceleg"
 
@@ -35,15 +35,15 @@
 pyserial = "^3.5"
 flexsea = "^8.0.1"
 smbus2 = "^0.4.2"
 numpy = "^1.24.3"
 
 [tool.poetry.group.dev.dependencies]
 bandit = "^1.7.1"
-black = {version = ">=22.3,<25.0", allow-prereleases = true}
+black = {version = ">=24.3,<25.0", allow-prereleases = true}
 darglint = "^1.8.1"
 isort = {extras = ["colors"], version = "^5.10.1"}
 mypy = ">=0.991,<1.1"
 mypy-extensions = "^0.4.3"
 pre-commit = "^2.15.0"
 pydocstyle = "^6.1.1"
 pylint = ">=2.13.7,<4.0.0"
@@ -51,15 +51,15 @@
 pytest-mock = "^3.12.0"
 pyupgrade = "^2.29.1"
 safety = "^2.2.0"
 coverage = "^6.1.2"
 coverage-badge = "^1.1.0"
 pytest-html = "^4.1.1"
 pytest-cov = ">=3,<5"
-click = "8.1.3"
+click = "8.1.7"
 sphinx = "^7.2.6"
 wheel = "^0.41.2"
 sphinx-book-theme = "^1.0.1"
 jinja2 = "^3.1.3"
 
 [tool.bandit]
 skips = ["B101"]
```

### Comparing `opensourceleg-2.2.0/PKG-INFO` & `opensourceleg-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensourceleg
-Version: 2.2.0
+Version: 2.2.1
 Summary: An open-source software library for numerical computation, data acquisition, and control of lower-limb robotic prostheses.
 Home-page: https://github.com/neurobionics/opensourceleg
 License: GNU LGPL v2.1
 Author: Open-source Leg
 Author-email: opensourceleg@gmail.com
 Requires-Python: >=3.9,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```

