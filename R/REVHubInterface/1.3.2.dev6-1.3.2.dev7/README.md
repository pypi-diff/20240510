# Comparing `tmp/revhubinterface-1.3.2.dev6.tar.gz` & `tmp/revhubinterface-1.3.2.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revhubinterface-1.3.2.dev6.tar", last modified: Wed May  8 01:50:26 2024, max compression
+gzip compressed data, was "revhubinterface-1.3.2.dev7.tar", last modified: Wed May  8 01:55:06 2024, max compression
```

## Comparing `revhubinterface-1.3.2.dev6.tar` & `revhubinterface-1.3.2.dev7.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:50:26.196462 revhubinterface-1.3.2.dev6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:50:26.188462 revhubinterface-1.3.2.dev6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:50:26.192462 revhubinterface-1.3.2.dev6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-08 01:50:19.000000 revhubinterface-1.3.2.dev6/.github/workflows/pyinstaller.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-08 01:50:19.000000 revhubinterface-1.3.2.dev6/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-08 01:50:19.000000 revhubinterface-1.3.2.dev6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-08 01:50:19.000000 revhubinterface-1.3.2.dev6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-05-08 01:50:26.196462 revhubinterface-1.3.2.dev6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-05-08 01:50:19.000000 revhubinterface-1.3.2.dev6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:50:26.192462 revhubinterface-1.3.2.dev6/REVHubInterface/
--rw-r--r--   0 runner    (1001) docker     (127)    20812 2024-05-08 01:50:19.000000 revhubinterface-1.3.2.dev6/REVHubInterface/REV2mSensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-08 01:50:19.000000 revhubinterface-1.3.2.dev6/REVHubInterface/REVADC.py
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-08 01:50:19.000000 revhubinterface-1.3.2.dev6/REVHubInterface/REVColorSensorV3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-08 01:50:19.000000 revhubinterface-1.3.2.dev6/REVHubInterface/REVComPorts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-08 01:50:19.000000 revhubinterface-1.3.2.dev6/REVHubInterface/REVDIO.py
--rw-r--r--   0 runner    (1001) docker     (127)    15925 2024-05-08 01:50:19.000000 revhubinterface-1.3.2.dev6/REVHubInterface/REVI2C.py
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-08 01:50:19.000000 revhubinterface-1.3.2.dev6/REVHubInterface/REVModule.py
--rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-05-08 01:50:19.000000 revhubinterface-1.3.2.dev6/REVHubInterface/REVMotor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-08 01:50:19.000000 revhubinterface-1.3.2.dev6/REVHubInterface/REVServo.py
--rw-r--r--   0 runner    (1001) docker     (127)    16892 2024-05-08 01:50:19.000000 revhubinterface-1.3.2.dev6/REVHubInterface/REVcomm.py
--rw-r--r--   0 runner    (1001) docker     (127)    73523 2024-05-08 01:50:19.000000 revhubinterface-1.3.2.dev6/REVHubInterface/REVmessages.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:50:19.000000 revhubinterface-1.3.2.dev6/REVHubInterface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    73572 2024-05-08 01:50:19.000000 revhubinterface-1.3.2.dev6/REVHubInterface/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-08 01:50:19.000000 revhubinterface-1.3.2.dev6/REVHubInterface-mac.spec
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:50:26.196462 revhubinterface-1.3.2.dev6/REVHubInterface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-05-08 01:50:26.000000 revhubinterface-1.3.2.dev6/REVHubInterface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-08 01:50:26.000000 revhubinterface-1.3.2.dev6/REVHubInterface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 01:50:26.000000 revhubinterface-1.3.2.dev6/REVHubInterface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-08 01:50:26.000000 revhubinterface-1.3.2.dev6/REVHubInterface.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-08 01:50:26.000000 revhubinterface-1.3.2.dev6/REVHubInterface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-08 01:50:26.000000 revhubinterface-1.3.2.dev6/REVHubInterface.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-05-08 01:50:19.000000 revhubinterface-1.3.2.dev6/REVHubInterface.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-08 01:50:19.000000 revhubinterface-1.3.2.dev6/REVHubInterface.spec
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:50:26.192462 revhubinterface-1.3.2.dev6/flatpak/
--rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-05-08 01:50:19.000000 revhubinterface-1.3.2.dev6/flatpak/flatpak-pip-generator
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-08 01:50:19.000000 revhubinterface-1.3.2.dev6/flatpak/org.unofficialrevport.REVHubInterface.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-08 01:50:19.000000 revhubinterface-1.3.2.dev6/flatpak/python3-requirements.json
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-08 01:50:19.000000 revhubinterface-1.3.2.dev6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-08 01:50:19.000000 revhubinterface-1.3.2.dev6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 01:50:26.196462 revhubinterface-1.3.2.dev6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:55:06.815960 revhubinterface-1.3.2.dev7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:55:06.811960 revhubinterface-1.3.2.dev7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:55:06.811960 revhubinterface-1.3.2.dev7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/.github/workflows/pyinstaller.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-05-08 01:55:06.815960 revhubinterface-1.3.2.dev7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:55:06.815960 revhubinterface-1.3.2.dev7/REVHubInterface/
+-rw-r--r--   0 runner    (1001) docker     (127)    20812 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/REVHubInterface/REV2mSensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/REVHubInterface/REVADC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/REVHubInterface/REVColorSensorV3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/REVHubInterface/REVComPorts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/REVHubInterface/REVDIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15925 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/REVHubInterface/REVI2C.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/REVHubInterface/REVModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/REVHubInterface/REVMotor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/REVHubInterface/REVServo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16892 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/REVHubInterface/REVcomm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73523 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/REVHubInterface/REVmessages.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/REVHubInterface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73572 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/REVHubInterface/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/REVHubInterface-mac.spec
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:55:06.815960 revhubinterface-1.3.2.dev7/REVHubInterface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-05-08 01:55:06.000000 revhubinterface-1.3.2.dev7/REVHubInterface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-08 01:55:06.000000 revhubinterface-1.3.2.dev7/REVHubInterface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 01:55:06.000000 revhubinterface-1.3.2.dev7/REVHubInterface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-08 01:55:06.000000 revhubinterface-1.3.2.dev7/REVHubInterface.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-08 01:55:06.000000 revhubinterface-1.3.2.dev7/REVHubInterface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-08 01:55:06.000000 revhubinterface-1.3.2.dev7/REVHubInterface.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/REVHubInterface.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/REVHubInterface.spec
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:55:06.815960 revhubinterface-1.3.2.dev7/flatpak/
+-rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/flatpak/flatpak-pip-generator
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/flatpak/org.unofficialrevport.REVHubInterface.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/flatpak/python3-requirements.json
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 01:55:06.815960 revhubinterface-1.3.2.dev7/setup.cfg
```

### Comparing `revhubinterface-1.3.2.dev6/.github/workflows/pyinstaller.yml` & `revhubinterface-1.3.2.dev7/.github/workflows/pyinstaller.yml`

 * *Files 8% similar despite different names*

```diff
@@ -10,41 +10,46 @@
       - name: Create Executable
         uses: sayyid5416/pyinstaller@v1
         with:
           python_ver: '3.12'
           pyinstaller_ver: '==6.6.0'
           spec: 'REVHubInterface-mac.spec'
           requirements: 'requirements.txt'
-          upload_exe_with_name: 'REVHubInterfaceMacBinary'
+          upload_exe_with_name: 'REVHubInterface_Mac_Binary'
           options: --onefile, --name "REVHubInterface", --windowed,
       - name: Make DMG
         uses: QQxiaoming/create-dmg-action@v0.0.2
         with:
-          name: 'REVHubInterfaceMacDMG.dmg'
+          name: 'REVHubInterface_Mac_DMG'
           srcdir: './dist'
+      - name: Upload DMG
+        uses: actions/upload-artifact@v4
+        with:
+          name: 'REVHubInterface_Mac_DMG'
+          path: './REVHubInterface_Mac_DMG.dmg'
   pyinstaller-build-win:
     runs-on: windows-latest
     steps:
       - name: Create Executable
         uses: sayyid5416/pyinstaller@v1
         with:
           python_ver: '3.12'
           pyinstaller_ver: '==6.6.0'
           spec: 'REVHubInterface.spec'
           requirements: 'requirements.txt'
-          upload_exe_with_name: 'REVHubInterface Windows'
+          upload_exe_with_name: 'REVHubInterface_Windows'
           options: --onefile, --name "REVHubInterface", --windowed,
   pyinstaller-build-linux:
     runs-on: ubuntu-latest
     steps:
       - name: Create Executable
         uses: sayyid5416/pyinstaller@v1
         with:
           python_ver: '3.12'
           pyinstaller_ver: '==6.6.0'
           spec: 'REVHubInterface.spec'
           requirements: 'requirements.txt'
-          upload_exe_with_name: 'REVHubInterface Linux'
+          upload_exe_with_name: 'REVHubInterface_Linux'
           options: --onefile, --name "REVHubInterface", --windowed,
```

### Comparing `revhubinterface-1.3.2.dev6/.github/workflows/python-publish.yml` & `revhubinterface-1.3.2.dev7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev6/LICENSE.txt` & `revhubinterface-1.3.2.dev7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev6/PKG-INFO` & `revhubinterface-1.3.2.dev7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: REVHubInterface
-Version: 1.3.2.dev6
+Version: 1.3.2.dev7
 Summary: GUI program for manual control of REV Robotics Expansion Hub from a PC. Unofficial "Community Edition". 
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyft232==0.12
 Requires-Dist: pyserial==3.5
 Requires-Dist: sv-ttk==2.6.0
```

### Comparing `revhubinterface-1.3.2.dev6/README.md` & `revhubinterface-1.3.2.dev7/README.md`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev6/REVHubInterface/REV2mSensor.py` & `revhubinterface-1.3.2.dev7/REVHubInterface/REV2mSensor.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev6/REVHubInterface/REVADC.py` & `revhubinterface-1.3.2.dev7/REVHubInterface/REVADC.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev6/REVHubInterface/REVColorSensorV3.py` & `revhubinterface-1.3.2.dev7/REVHubInterface/REVColorSensorV3.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev6/REVHubInterface/REVComPorts.py` & `revhubinterface-1.3.2.dev7/REVHubInterface/REVComPorts.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev6/REVHubInterface/REVDIO.py` & `revhubinterface-1.3.2.dev7/REVHubInterface/REVDIO.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev6/REVHubInterface/REVI2C.py` & `revhubinterface-1.3.2.dev7/REVHubInterface/REVI2C.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev6/REVHubInterface/REVModule.py` & `revhubinterface-1.3.2.dev7/REVHubInterface/REVModule.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev6/REVHubInterface/REVMotor.py` & `revhubinterface-1.3.2.dev7/REVHubInterface/REVMotor.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev6/REVHubInterface/REVServo.py` & `revhubinterface-1.3.2.dev7/REVHubInterface/REVServo.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev6/REVHubInterface/REVcomm.py` & `revhubinterface-1.3.2.dev7/REVHubInterface/REVcomm.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev6/REVHubInterface/REVmessages.py` & `revhubinterface-1.3.2.dev7/REVHubInterface/REVmessages.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev6/REVHubInterface/__main__.py` & `revhubinterface-1.3.2.dev7/REVHubInterface/__main__.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev6/REVHubInterface-mac.spec` & `revhubinterface-1.3.2.dev7/REVHubInterface-mac.spec`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev6/REVHubInterface.egg-info/PKG-INFO` & `revhubinterface-1.3.2.dev7/REVHubInterface.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: REVHubInterface
-Version: 1.3.2.dev6
+Version: 1.3.2.dev7
 Summary: GUI program for manual control of REV Robotics Expansion Hub from a PC. Unofficial "Community Edition". 
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyft232==0.12
 Requires-Dist: pyserial==3.5
 Requires-Dist: sv-ttk==2.6.0
```

### Comparing `revhubinterface-1.3.2.dev6/REVHubInterface.egg-info/SOURCES.txt` & `revhubinterface-1.3.2.dev7/REVHubInterface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev6/REVHubInterface.spec` & `revhubinterface-1.3.2.dev7/REVHubInterface.spec`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev6/flatpak/flatpak-pip-generator` & `revhubinterface-1.3.2.dev7/flatpak/flatpak-pip-generator`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev6/flatpak/org.unofficialrevport.REVHubInterface.yml` & `revhubinterface-1.3.2.dev7/flatpak/org.unofficialrevport.REVHubInterface.yml`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev6/flatpak/python3-requirements.json` & `revhubinterface-1.3.2.dev7/flatpak/python3-requirements.json`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev6/pyproject.toml` & `revhubinterface-1.3.2.dev7/pyproject.toml`

 * *Files identical despite different names*

