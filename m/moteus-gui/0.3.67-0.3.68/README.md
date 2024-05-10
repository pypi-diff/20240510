# Comparing `tmp/moteus_gui-0.3.67-py3-none-any.whl.zip` & `tmp/moteus_gui-0.3.68-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 13956 bytes, number of entries: 9
--rw-r--r--  2.0 unx        0 b- defN 23-May-23 14:59 moteus_gui/__init__.py
--rw-r--r--  2.0 unx    40032 b- defN 23-Oct-17 17:01 moteus_gui/tview.py
--rw-rw-r--  2.0 unx     5556 b- defN 23-Aug-03 02:51 moteus_gui/tview_main_window.ui
--rw-r--r--  2.0 unx      627 b- defN 24-Jan-12 20:26 moteus_gui/version.py
--rw-r--r--  2.0 unx     1072 b- defN 24-Jan-12 20:26 moteus_gui-0.3.67.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Jan-12 20:26 moteus_gui-0.3.67.dist-info/WHEEL
--rw-r--r--  2.0 unx       48 b- defN 24-Jan-12 20:26 moteus_gui-0.3.67.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 24-Jan-12 20:26 moteus_gui-0.3.67.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      731 b- defN 24-Jan-12 20:26 moteus_gui-0.3.67.dist-info/RECORD
-9 files, 48169 bytes uncompressed, 12688 bytes compressed:  73.7%
+Zip file size: 14432 bytes, number of entries: 9
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-26 18:29 moteus_gui/__init__.py
+-rw-r--r--  2.0 unx    42094 b- defN 24-Apr-30 01:49 moteus_gui/tview.py
+-rw-rw-r--  2.0 unx     5556 b- defN 24-Feb-26 18:29 moteus_gui/tview_main_window.ui
+-rw-r--r--  2.0 unx      627 b- defN 24-Apr-30 11:46 moteus_gui/version.py
+-rw-r--r--  2.0 unx     1077 b- defN 24-May-10 18:16 moteus_gui-0.3.68.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-10 18:16 moteus_gui-0.3.68.dist-info/WHEEL
+-rw-r--r--  2.0 unx       48 b- defN 24-May-10 18:16 moteus_gui-0.3.68.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 24-May-10 18:16 moteus_gui-0.3.68.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      731 b- defN 24-May-10 18:16 moteus_gui-0.3.68.dist-info/RECORD
+9 files, 50236 bytes uncompressed, 13164 bytes compressed:  73.8%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: moteus_gui/tview_main_window.ui
 Comment: 
 
 Filename: moteus_gui/version.py
 Comment: 
 
-Filename: moteus_gui-0.3.67.dist-info/METADATA
+Filename: moteus_gui-0.3.68.dist-info/METADATA
 Comment: 
 
-Filename: moteus_gui-0.3.67.dist-info/WHEEL
+Filename: moteus_gui-0.3.68.dist-info/WHEEL
 Comment: 
 
-Filename: moteus_gui-0.3.67.dist-info/entry_points.txt
+Filename: moteus_gui-0.3.68.dist-info/entry_points.txt
 Comment: 
 
-Filename: moteus_gui-0.3.67.dist-info/top_level.txt
+Filename: moteus_gui-0.3.68.dist-info/top_level.txt
 Comment: 
 
-Filename: moteus_gui-0.3.67.dist-info/RECORD
+Filename: moteus_gui-0.3.68.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## moteus_gui/tview.py

```diff
@@ -607,14 +607,18 @@
         self._data_tree_item = data_tree_item
 
         self._telemetry_records = {}
         self._schema_name = None
         self._config_tree_items = {}
         self._config_callback = None
 
+        self._events = {}
+        self._data_update_time = {}
+        self._data = {}
+
         self._updating_config = False
 
     async def start(self):
         # Stop the spew.
         self.write('\r\ntel stop\r\n'.encode('latin1'))
 
         # Make sure we've actually had a chance to write and poll.
@@ -760,14 +764,34 @@
 
         record = self._telemetry_records[name]
         if record:
             struct = record.archive.read(reader.Stream(io.BytesIO(data)))
             record.update(struct)
             _set_tree_widget_data(record.tree_item, struct, record.archive)
 
+            self._data[name] = struct
+            if name not in self._events:
+                self._events[name] = asyncio.Event()
+            self._events[name].set()
+            self._data_update_time[name] = time.time()
+
+    async def wait_for_data(self, name):
+        if name not in self._events:
+            self._events[name] = asyncio.Event()
+
+        await self._events[name].wait()
+        self._events[name].clear()
+        return self._data[name]
+
+    async def ensure_record_active(self, name):
+        now = time.time()
+        if (now - self._data_update_time.get(name, 0.0)) > 0.2:
+            print(f"trying to enable {name}")
+            self.write_line(f'tel rate {name} 100\r\n')
+
     async def read_sized_block(self):
         return await self._stream.read_sized_block()
 
     async def process_message(self, message):
         any_data_read = await self._stream.process_message(message)
 
         return any_data_read
@@ -898,14 +922,16 @@
 class TviewMainWindow():
     def __init__(self, options, parent=None):
         self.options = options
         self.port = None
         self.devices = []
         self.default_rate = 100
 
+        self.user_task = None
+
         current_script_dir = os.path.dirname(os.path.abspath(__file__))
         uifilename = os.path.join(current_script_dir, "tview_main_window.ui")
 
         loader = QtUiTools.QUiLoader()
         uifile = QtCore.QFile(uifilename)
         uifile.open(QtCore.QFile.ReadOnly)
         self.ui = loader.load(uifile, parent)
@@ -1062,38 +1088,78 @@
         def write():
             for device in devices:
                 device.write((line + '\n').encode('latin1'))
 
         return write
 
     def _handle_user_input(self, line):
-        device_lines = [x.strip() for x in line.split('&&')]
-        now = time.time()
-        current_delay_ms = 0
-        for line in device_lines:
-            delay_re = re.search(r"^:(\d+)$", line)
-            device_re = re.search(r"^(A|\d+)>(.*)$", line)
-            if delay_re:
-                current_delay_ms += int(delay_re.group(1))
-                continue
-            elif device_re:
-                if device_re.group(1) == 'A':
-                    device_nums = [x.number for x in self.devices]
-                else:
-                    device_nums = [int(device_re.group(1))]
-                line = device_re.group(2)
-            else:
-                device_nums = [self.devices[0].number]
-            devices = [x for x in self.devices if x.number in device_nums]
-            writer = self.make_writer(devices, line)
+        if self.user_task is not None:
+            # We have an outstanding one, so cancel it.
+            self.user_task.cancel()
+            self.user_task = None
+
+        self.user_task = asyncio.create_task(
+            self._run_user_command_line(line))
+
+    async def _run_user_command_line(self, line):
+        try:
+            for command in [x.strip() for x in line.split('&&')]:
+                await self._run_user_command(command)
+        except Exception as e:
+            print("Error:", str(e))
+
+            # Otherwise ignore problems so that tview keeps running.
 
-            if current_delay_ms > 0:
-                QtCore.QTimer.singleShot(current_delay_ms, writer)
+    async def _wait_user_query(self, maybe_id):
+        device_nums = [self.devices[0].number]
+        if maybe_id:
+            device_nums = [int(maybe_id)]
+
+        devices = [x for x in self.devices if x.number in device_nums]
+
+        record = 'servo_stats'
+
+        if len(devices) == 0:
+            # Nothing to wait on, so return immediately
+            return
+
+        for d in devices:
+            await d.ensure_record_active(record)
+            await d.wait_for_data(record)
+            await d.wait_for_data(record)
+
+        while True:
+            # Now look for at least to have trajectory_done == True
+            for d in devices:
+                servo_stats = await d.wait_for_data(record)
+                if getattr(servo_stats, 'trajectory_done', False):
+                    return
+
+    async def _run_user_command(self, command):
+        delay_re = re.search(r"^:(\d+)$", command)
+        device_re = re.search(r"^(A|\d+)>(.*)$", command)
+        traj_re = re.search(r"^(\?(\d+)?)$", command)
+
+        device_nums = [self.devices[0].number]
+
+        if traj_re:
+            await self._wait_user_query(traj_re.group(2))
+            return
+        if delay_re:
+            await asyncio.sleep(int(delay_re.group(2)) / 1000.0)
+            return
+        elif device_re:
+            command = device_re.group(2)
+            if device_re.group(1) == 'A':
+                device_nums = [x.number for x in self.devices]
             else:
-                writer()
+                device_nums = [int(device_re.group(1))]
+
+        for device in [x for x in self.devices if x.number in device_nums]:
+            device.write((command + '\n').encode('latin1'))
 
     def _handle_tree_expanded(self, item):
         self.ui.telemetryTreeWidget.resizeColumnToContents(0)
         user_data = item.data(0, QtCore.Qt.UserRole)
         if user_data:
             user_data.expand()
```

## moteus_gui/version.py

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-VERSION="0.3.67"
+VERSION="0.3.68"
```

## Comparing `moteus_gui-0.3.67.dist-info/METADATA` & `moteus_gui-0.3.68.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moteus-gui
-Version: 0.3.67
+Version: 0.3.68
 Summary: moteus brushless controller graphical user interfaces
 Home-page: https://github.com/mjbots/moteus
 Author: mjbots Robotic Systems
 Author-email: info@mjbots.com
 Keywords: moteus
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -14,15 +14,15 @@
 Description-Content-Type: text/markdown
 Requires-Dist: asyncqt >=0.8
 Requires-Dist: moteus >=0.3.26
 Requires-Dist: matplotlib >=3.5
 Requires-Dist: numpy
 Requires-Dist: qtconsole >=0.5.2
 Requires-Dist: qtpy >=2.0.1
-Requires-Dist: PySide6 >=6.2 ; platform_system != "Linux"
+Requires-Dist: PySide6 <6.7,>=6.2 ; platform_system != "Linux"
 Requires-Dist: PySide2 ; platform_system == "Linux"
 Requires-Dist: msvc-runtime ; platform_system == "Windows" and python_version < "3.12"
 
 # moteus GUI tools #
 
 This package contains the `tview` graphical tool for interacting with
 moteus controllers.
```

## Comparing `moteus_gui-0.3.67.dist-info/RECORD` & `moteus_gui-0.3.68.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 moteus_gui/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-moteus_gui/tview.py,sha256=njykSaZC1urR0g3KEOuNvwVojJcxbk1J17P91sDi_7I,40032
+moteus_gui/tview.py,sha256=IUYQOuB9dE_00bN9wB6mjE50CfaoKkXtyrMYp5CTZ2k,42094
 moteus_gui/tview_main_window.ui,sha256=q_qA1sooIWzprVT8eYAe0EH9lfu7zg-QP1diETCNFh8,5556
-moteus_gui/version.py,sha256=q4LPxNY63TQcpoLc62l1hxxwO8yOooz5ORImA1Tw6io,627
-moteus_gui-0.3.67.dist-info/METADATA,sha256=gYq-S3H_9XeKKBbc2ftl0OPR9lHAWdP960hvJxjXeYg,1072
-moteus_gui-0.3.67.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-moteus_gui-0.3.67.dist-info/entry_points.txt,sha256=Y9PnhK_gNxr8CO7_POHieVaK1U_4fgu2EYoS6TyzSgk,48
-moteus_gui-0.3.67.dist-info/top_level.txt,sha256=oPOkXR-zpPFhGiDcbnDY6scvNqQQAXWzV7oPD_GHMns,11
-moteus_gui-0.3.67.dist-info/RECORD,,
+moteus_gui/version.py,sha256=8rx1YUinZCom0pzbiJ3IcLDXrj5FEja3M79tr75nJJM,627
+moteus_gui-0.3.68.dist-info/METADATA,sha256=rUBEN94YcDg8VZuRIVXA0TWtpl96o_Wy14rL1KFViHU,1077
+moteus_gui-0.3.68.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+moteus_gui-0.3.68.dist-info/entry_points.txt,sha256=Y9PnhK_gNxr8CO7_POHieVaK1U_4fgu2EYoS6TyzSgk,48
+moteus_gui-0.3.68.dist-info/top_level.txt,sha256=oPOkXR-zpPFhGiDcbnDY6scvNqQQAXWzV7oPD_GHMns,11
+moteus_gui-0.3.68.dist-info/RECORD,,
```

