# Comparing `tmp/caroa04-1.0.2.tar.gz` & `tmp/caroa04-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caroa04-1.0.2.tar", last modified: Sat Apr 27 16:47:24 2024, max compression
+gzip compressed data, was "caroa04-1.0.3.tar", last modified: Fri May 10 06:41:50 2024, max compression
```

## Comparing `caroa04-1.0.2.tar` & `caroa04-1.0.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 16:47:24.782580 caroa04-1.0.2/
--rw-rw-rw-   0        0        0      179 2024-04-14 17:26:49.000000 caroa04-1.0.2/AUTHORS.rst
--rw-rw-rw-   0        0        0     3870 2024-04-14 17:26:49.000000 caroa04-1.0.2/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2024-04-14 17:26:49.000000 caroa04-1.0.2/HISTORY.rst
--rw-rw-rw-   0        0        0     1102 2024-04-14 17:26:49.000000 caroa04-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      273 2024-04-14 17:26:49.000000 caroa04-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4975 2024-04-27 16:47:24.781580 caroa04-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3824 2024-04-27 16:31:01.000000 caroa04-1.0.2/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-27 16:47:24.774575 caroa04-1.0.2/docs/
--rw-rw-rw-   0        0        0      628 2024-04-14 17:26:49.000000 caroa04-1.0.2/docs/Makefile
--rw-rw-rw-   0        0        0       29 2024-04-14 17:26:49.000000 caroa04-1.0.2/docs/authors.rst
--rw-rw-rw-   0        0        0     4990 2024-04-14 19:01:23.000000 caroa04-1.0.2/docs/conf.py
--rw-rw-rw-   0        0        0       34 2024-04-14 17:26:49.000000 caroa04-1.0.2/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2024-04-14 17:26:49.000000 caroa04-1.0.2/docs/history.rst
--rw-rw-rw-   0        0        0      324 2024-04-14 17:26:49.000000 caroa04-1.0.2/docs/index.rst
--rw-rw-rw-   0        0        0     1169 2024-04-14 17:26:49.000000 caroa04-1.0.2/docs/installation.rst
--rwxrwxrwx   0        0        0      805 2024-04-14 17:26:49.000000 caroa04-1.0.2/docs/make.bat
--rw-rw-rw-   0        0        0       28 2024-04-14 17:26:49.000000 caroa04-1.0.2/docs/readme.rst
--rw-rw-rw-   0        0        0       76 2024-04-14 17:26:49.000000 caroa04-1.0.2/docs/usage.rst
--rw-rw-rw-   0        0        0     1598 2024-04-27 16:46:40.000000 caroa04-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-27 16:47:24.782580 caroa04-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-27 16:47:24.762294 caroa04-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-27 16:47:24.775580 caroa04-1.0.2/src/caroa04/
--rw-rw-rw-   0        0        0      140 2024-04-14 17:26:49.000000 caroa04-1.0.2/src/caroa04/__init__.py
--rw-rw-rw-   0        0        0    14337 2024-04-26 10:46:42.000000 caroa04-1.0.2/src/caroa04/canmessage.py
--rw-rw-rw-   0        0        0     5974 2024-04-27 16:46:35.000000 caroa04-1.0.2/src/caroa04/caroa04.py
-drwxrwxrwx   0        0        0        0 2024-04-27 16:47:24.780579 caroa04-1.0.2/src/caroa04.egg-info/
--rw-rw-rw-   0        0        0     4975 2024-04-27 16:47:24.000000 caroa04-1.0.2/src/caroa04.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      538 2024-04-27 16:47:24.000000 caroa04-1.0.2/src/caroa04.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 16:47:24.000000 caroa04-1.0.2/src/caroa04.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-04-27 16:47:24.000000 caroa04-1.0.2/src/caroa04.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-27 16:47:24.000000 caroa04-1.0.2/src/caroa04.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-27 16:47:24.779580 caroa04-1.0.2/tests/
--rw-rw-rw-   0        0        0       38 2024-04-14 17:26:49.000000 caroa04-1.0.2/tests/__init__.py
--rw-rw-rw-   0        0        0     6897 2024-04-27 16:31:01.000000 caroa04-1.0.2/tests/test_caroa04.py
+drwxrwxrwx   0        0        0        0 2024-05-10 06:41:50.553155 caroa04-1.0.3/
+-rw-rw-rw-   0        0        0      179 2024-04-14 17:26:49.000000 caroa04-1.0.3/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3870 2024-04-14 17:26:49.000000 caroa04-1.0.3/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2024-04-14 17:26:49.000000 caroa04-1.0.3/HISTORY.rst
+-rw-rw-rw-   0        0        0     1102 2024-04-14 17:26:49.000000 caroa04-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0      273 2024-04-14 17:26:49.000000 caroa04-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4975 2024-05-10 06:41:50.552137 caroa04-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3824 2024-04-27 16:31:01.000000 caroa04-1.0.3/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-10 06:41:50.533149 caroa04-1.0.3/docs/
+-rw-rw-rw-   0        0        0      628 2024-04-14 17:26:49.000000 caroa04-1.0.3/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2024-04-14 17:26:49.000000 caroa04-1.0.3/docs/authors.rst
+-rw-rw-rw-   0        0        0     4990 2024-04-14 19:01:23.000000 caroa04-1.0.3/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2024-04-14 17:26:49.000000 caroa04-1.0.3/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2024-04-14 17:26:49.000000 caroa04-1.0.3/docs/history.rst
+-rw-rw-rw-   0        0        0      324 2024-04-14 17:26:49.000000 caroa04-1.0.3/docs/index.rst
+-rw-rw-rw-   0        0        0     1169 2024-04-14 17:26:49.000000 caroa04-1.0.3/docs/installation.rst
+-rwxrwxrwx   0        0        0      805 2024-04-14 17:26:49.000000 caroa04-1.0.3/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2024-04-14 17:26:49.000000 caroa04-1.0.3/docs/readme.rst
+-rw-rw-rw-   0        0        0       76 2024-04-14 17:26:49.000000 caroa04-1.0.3/docs/usage.rst
+-rw-rw-rw-   0        0        0     1598 2024-05-10 06:39:24.000000 caroa04-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-10 06:41:50.553155 caroa04-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-10 06:41:50.473579 caroa04-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-10 06:41:50.540115 caroa04-1.0.3/src/caroa04/
+-rw-rw-rw-   0        0        0      140 2024-04-14 17:26:49.000000 caroa04-1.0.3/src/caroa04/__init__.py
+-rw-rw-rw-   0        0        0    14337 2024-04-26 10:46:42.000000 caroa04-1.0.3/src/caroa04/canmessage.py
+-rw-rw-rw-   0        0        0     6254 2024-05-10 06:39:24.000000 caroa04-1.0.3/src/caroa04/caroa04.py
+drwxrwxrwx   0        0        0        0 2024-05-10 06:41:50.552137 caroa04-1.0.3/src/caroa04.egg-info/
+-rw-rw-rw-   0        0        0     4975 2024-05-10 06:41:50.000000 caroa04-1.0.3/src/caroa04.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      538 2024-05-10 06:41:50.000000 caroa04-1.0.3/src/caroa04.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 06:41:50.000000 caroa04-1.0.3/src/caroa04.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-05-10 06:41:50.000000 caroa04-1.0.3/src/caroa04.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-10 06:41:50.000000 caroa04-1.0.3/src/caroa04.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 06:41:50.551170 caroa04-1.0.3/tests/
+-rw-rw-rw-   0        0        0       38 2024-04-14 17:26:49.000000 caroa04-1.0.3/tests/__init__.py
+-rw-rw-rw-   0        0        0     6897 2024-04-27 16:31:01.000000 caroa04-1.0.3/tests/test_caroa04.py
```

### Comparing `caroa04-1.0.2/CONTRIBUTING.rst` & `caroa04-1.0.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `caroa04-1.0.2/LICENSE` & `caroa04-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `caroa04-1.0.2/PKG-INFO` & `caroa04-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caroa04
-Version: 1.0.2
+Version: 1.0.3
 Summary: Library to control the CAROA04 CAN-IO expander device from eletechsup.
 Author-email: Rodolphe Mete Soyding <r.soyding@gmail.com>
 Maintainer-email: Rodolphe Mete Soyding <r.soyding@gmail.com>
 License: MIT license
 Project-URL: bugs, https://github.com/supermete/caroa04/issues
 Project-URL: changelog, https://github.com/supermete/caroa04/blob/master/changelog.md
 Project-URL: homepage, https://github.com/supermete/caroa04
```

### Comparing `caroa04-1.0.2/README.rst` & `caroa04-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `caroa04-1.0.2/docs/Makefile` & `caroa04-1.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `caroa04-1.0.2/docs/conf.py` & `caroa04-1.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `caroa04-1.0.2/docs/installation.rst` & `caroa04-1.0.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `caroa04-1.0.2/docs/make.bat` & `caroa04-1.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `caroa04-1.0.2/pyproject.toml` & `caroa04-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "caroa04"
-version = "1.0.2"
+version = "1.0.3"
 description = "Library to control the CAROA04 CAN-IO expander device from eletechsup."
 readme = "README.rst"
 requires-python = ">=3.8"
 authors = [
   {name = "Rodolphe Mete Soyding", email = "r.soyding@gmail.com"}
 ]
 maintainers = [
```

### Comparing `caroa04-1.0.2/src/caroa04/canmessage.py` & `caroa04-1.0.3/src/caroa04/canmessage.py`

 * *Files identical despite different names*

### Comparing `caroa04-1.0.2/src/caroa04/caroa04.py` & `caroa04-1.0.3/src/caroa04/caroa04.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 sys.path.append(str(pathlib.Path(__file__).parent))
 
 from canmessage import CanMessageRW, XCanSignal, BOOL, ENUM
 
 logging.basicConfig(level=logging.INFO)
 
 __author__ = "R. Soyding"
-__version__ = "1.0.2"
+__version__ = "1.0.3"
 
 MSGID_DO_WRITE = 0x100
 MSGID_DO_READ = 0x200
 MSGID_DI_READ = 0x300
 MSGID_PARAM = 0x700
 DEFAULT_NODEID = 0xE0
 
@@ -126,14 +126,24 @@
             self.notifier = can.Notifier(self.bus, [self.listener], timeout=2.0)
 
         self.message_do.bus = self.bus
         self.message_di.bus = self.bus
         self.message_nodeid.bus = self.bus
         self.message_bitrate.bus = self.bus
 
+        self._init_outputs()
+
+    def _init_outputs(self):
+        """
+        To avoid overwriting the state of already set outputs, initialize by reading the current
+        state of the outputs first.
+        :return: None
+        """
+        self.message_do.read()
+
     def listener(self, msg):
         if msg.arbitration_id in (self.message_do.read_id, self.message_do.write_id):
             logging.debug(msg)
             self.message_do.update_payload(msg.data)
         elif msg.arbitration_id in (self.message_di.read_id, self.message_di.write_id):
             logging.debug(msg)
             self.message_di.update_payload(msg.data)
```

### Comparing `caroa04-1.0.2/src/caroa04.egg-info/PKG-INFO` & `caroa04-1.0.3/src/caroa04.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caroa04
-Version: 1.0.2
+Version: 1.0.3
 Summary: Library to control the CAROA04 CAN-IO expander device from eletechsup.
 Author-email: Rodolphe Mete Soyding <r.soyding@gmail.com>
 Maintainer-email: Rodolphe Mete Soyding <r.soyding@gmail.com>
 License: MIT license
 Project-URL: bugs, https://github.com/supermete/caroa04/issues
 Project-URL: changelog, https://github.com/supermete/caroa04/blob/master/changelog.md
 Project-URL: homepage, https://github.com/supermete/caroa04
```

### Comparing `caroa04-1.0.2/src/caroa04.egg-info/SOURCES.txt` & `caroa04-1.0.3/src/caroa04.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `caroa04-1.0.2/tests/test_caroa04.py` & `caroa04-1.0.3/tests/test_caroa04.py`

 * *Files identical despite different names*

