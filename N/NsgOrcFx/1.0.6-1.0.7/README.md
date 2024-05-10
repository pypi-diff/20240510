# Comparing `tmp/nsgorcfx-1.0.6.tar.gz` & `tmp/nsgorcfx-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsgorcfx-1.0.6.tar", last modified: Thu May  9 13:34:56 2024, max compression
+gzip compressed data, was "nsgorcfx-1.0.7.tar", last modified: Fri May 10 12:24:46 2024, max compression
```

## Comparing `nsgorcfx-1.0.6.tar` & `nsgorcfx-1.0.7.tar`

### file list

```diff
@@ -1,27 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 13:34:56.692956 nsgorcfx-1.0.6/
--rw-rw-rw-   0        0        0     1091 2024-05-09 02:25:41.000000 nsgorcfx-1.0.6/LICENSE
--rw-rw-rw-   0        0        0      998 2024-05-09 13:34:56.687956 nsgorcfx-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      442 2024-05-09 03:09:52.000000 nsgorcfx-1.0.6/README.md
--rw-rw-rw-   0        0        0      540 2024-05-09 13:33:19.000000 nsgorcfx-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-09 13:34:56.692956 nsgorcfx-1.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-09 13:34:56.574957 nsgorcfx-1.0.6/src/
-drwxrwxrwx   0        0        0        0 2024-05-09 13:34:56.639955 nsgorcfx-1.0.6/src/NsgOrcFx/
--rw-rw-rw-   0        0        0     9822 2024-05-09 13:28:50.000000 nsgorcfx-1.0.6/src/NsgOrcFx/NsgOrcFx.py
--rw-rw-rw-   0        0        0       23 2024-05-09 10:35:25.000000 nsgorcfx-1.0.6/src/NsgOrcFx/__init__.py
--rw-rw-rw-   0        0        0     3833 2024-05-09 02:55:39.000000 nsgorcfx-1.0.6/src/NsgOrcFx/auxfuncs.py
--rw-rw-rw-   0        0        0    10518 2024-05-09 11:28:00.000000 nsgorcfx-1.0.6/src/NsgOrcFx/classes.py
--rw-rw-rw-   0        0        0      127 2024-05-08 22:12:52.000000 nsgorcfx-1.0.6/src/NsgOrcFx/constants.py
--rw-rw-rw-   0        0        0     5139 2024-05-09 03:13:23.000000 nsgorcfx-1.0.6/src/NsgOrcFx/environment.py
--rw-rw-rw-   0        0        0     9822 2024-05-09 03:13:41.000000 nsgorcfx-1.0.6/src/NsgOrcFx/modal.py
--rw-rw-rw-   0        0        0      908 2024-05-09 03:20:04.000000 nsgorcfx-1.0.6/src/NsgOrcFx/objauxfuncs.py
--rw-rw-rw-   0        0        0     6795 2024-05-09 12:07:40.000000 nsgorcfx-1.0.6/src/NsgOrcFx/params.py
--rw-rw-rw-   0        0        0     2131 2024-05-09 03:19:08.000000 nsgorcfx-1.0.6/src/NsgOrcFx/sncurves.py
--rw-rw-rw-   0        0        0     5179 2024-05-09 02:57:42.000000 nsgorcfx-1.0.6/src/NsgOrcFx/sortlines.py
--rw-rw-rw-   0        0        0     2470 2024-05-09 03:14:07.000000 nsgorcfx-1.0.6/src/NsgOrcFx/utils.py
--rw-rw-rw-   0        0        0     6108 2024-05-09 03:14:20.000000 nsgorcfx-1.0.6/src/NsgOrcFx/weight.py
--rw-rw-rw-   0        0        0     5594 2024-05-09 03:14:29.000000 nsgorcfx-1.0.6/src/NsgOrcFx/weightaux.py
-drwxrwxrwx   0        0        0        0 2024-05-09 13:34:56.685956 nsgorcfx-1.0.6/src/NsgOrcFx.egg-info/
--rw-rw-rw-   0        0        0      998 2024-05-09 13:34:56.000000 nsgorcfx-1.0.6/src/NsgOrcFx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      524 2024-05-09 13:34:56.000000 nsgorcfx-1.0.6/src/NsgOrcFx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 13:34:56.000000 nsgorcfx-1.0.6/src/NsgOrcFx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-09 13:34:56.000000 nsgorcfx-1.0.6/src/NsgOrcFx.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 12:24:46.968557 nsgorcfx-1.0.7/
+-rw-rw-rw-   0        0        0     1091 2024-05-09 02:25:41.000000 nsgorcfx-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0      998 2024-05-10 12:24:46.965554 nsgorcfx-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2024-05-09 03:09:52.000000 nsgorcfx-1.0.7/README.md
+-rw-rw-rw-   0        0        0      540 2024-05-10 12:24:08.000000 nsgorcfx-1.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-10 12:24:46.968557 nsgorcfx-1.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-10 12:24:46.850554 nsgorcfx-1.0.7/src/
+drwxrwxrwx   0        0        0        0 2024-05-10 12:24:46.926555 nsgorcfx-1.0.7/src/NsgOrcFx/
+-rw-rw-rw-   0        0        0    13496 2024-05-10 11:07:30.000000 nsgorcfx-1.0.7/src/NsgOrcFx/NsgOrcFx.py
+-rw-rw-rw-   0        0        0       61 2024-05-10 11:35:55.000000 nsgorcfx-1.0.7/src/NsgOrcFx/__init__.py
+-rw-rw-rw-   0        0        0     8532 2024-05-09 19:00:14.000000 nsgorcfx-1.0.7/src/NsgOrcFx/auxfuncs.py
+-rw-rw-rw-   0        0        0     6953 2024-05-10 11:35:05.000000 nsgorcfx-1.0.7/src/NsgOrcFx/classes.py
+-rw-rw-rw-   0        0        0      450 2024-05-09 17:34:47.000000 nsgorcfx-1.0.7/src/NsgOrcFx/constants.py
+-rw-rw-rw-   0        0        0     5139 2024-05-09 03:13:23.000000 nsgorcfx-1.0.7/src/NsgOrcFx/environment.py
+-rw-rw-rw-   0        0        0     6868 2024-05-10 12:13:31.000000 nsgorcfx-1.0.7/src/NsgOrcFx/fatigue.py
+-rw-rw-rw-   0        0        0     4713 2024-05-10 09:56:02.000000 nsgorcfx-1.0.7/src/NsgOrcFx/loadcases.py
+-rw-rw-rw-   0        0        0     9822 2024-05-09 03:13:41.000000 nsgorcfx-1.0.7/src/NsgOrcFx/modal.py
+-rw-rw-rw-   0        0        0      906 2024-05-10 11:34:59.000000 nsgorcfx-1.0.7/src/NsgOrcFx/objauxfuncs.py
+-rw-rw-rw-   0        0        0    16376 2024-05-10 11:45:36.000000 nsgorcfx-1.0.7/src/NsgOrcFx/params.py
+-rw-rw-rw-   0        0        0     2116 2024-05-10 11:45:47.000000 nsgorcfx-1.0.7/src/NsgOrcFx/sncurves.py
+-rw-rw-rw-   0        0        0     5179 2024-05-09 02:57:42.000000 nsgorcfx-1.0.7/src/NsgOrcFx/sortlines.py
+-rw-rw-rw-   0        0        0     2587 2024-05-10 11:05:59.000000 nsgorcfx-1.0.7/src/NsgOrcFx/utils.py
+-rw-rw-rw-   0        0        0     6108 2024-05-09 03:14:20.000000 nsgorcfx-1.0.7/src/NsgOrcFx/weight.py
+-rw-rw-rw-   0        0        0     5594 2024-05-09 03:14:29.000000 nsgorcfx-1.0.7/src/NsgOrcFx/weightaux.py
+drwxrwxrwx   0        0        0        0 2024-05-10 12:24:46.964554 nsgorcfx-1.0.7/src/NsgOrcFx.egg-info/
+-rw-rw-rw-   0        0        0      998 2024-05-10 12:24:46.000000 nsgorcfx-1.0.7/src/NsgOrcFx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      695 2024-05-10 12:24:46.000000 nsgorcfx-1.0.7/src/NsgOrcFx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 12:24:46.000000 nsgorcfx-1.0.7/src/NsgOrcFx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-10 12:24:46.000000 nsgorcfx-1.0.7/src/NsgOrcFx.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 12:24:46.960554 nsgorcfx-1.0.7/tests/
+-rw-rw-rw-   0        0        0      749 2024-05-10 09:58:05.000000 nsgorcfx-1.0.7/tests/test1_data-auto-complete.py
+-rw-rw-rw-   0        0        0      598 2024-05-10 10:31:22.000000 nsgorcfx-1.0.7/tests/test2_generate-loadcases.py
+-rw-rw-rw-   0        0        0      578 2024-05-10 10:51:14.000000 nsgorcfx-1.0.7/tests/test3_modal-analysis.py
+-rw-rw-rw-   0        0        0      602 2024-05-10 12:15:32.000000 nsgorcfx-1.0.7/tests/test4_fatigue.py
```

### Comparing `nsgorcfx-1.0.6/LICENSE` & `nsgorcfx-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nsgorcfx-1.0.6/PKG-INFO` & `nsgorcfx-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NsgOrcFx
-Version: 1.0.6
+Version: 1.0.7
 Summary: Package with additional tools to the OrcFxAPI package
 Author-email: NSG Engenharia <comercial@nsgeng.com>
 Project-URL: Homepage, https://github.com/NSG-Engenharia/NsgOrcFx
 Project-URL: Issues, https://github.com/NSG-Engenharia/NsgOrcFx/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `nsgorcfx-1.0.6/pyproject.toml` & `nsgorcfx-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "NsgOrcFx"
-version = "1.0.6"
+version = "1.0.7"
 authors = [
   { name="NSG Engenharia", email="comercial@nsgeng.com" },
 ]
 description = "Package with additional tools to the OrcFxAPI package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `nsgorcfx-1.0.6/src/NsgOrcFx/NsgOrcFx.py` & `nsgorcfx-1.0.7/src/NsgOrcFx/auxfuncs.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,268 +1,238 @@
-"""
-# Library of complementary tools for the OrcaFlex API (OrcFxAPI)
-#
-#
-#
-"""
-from __future__ import annotations
-
-__author__ = "NSG Engenharia"
-__copyright__ = "Copyright 2023"
-__credits__ = ["Gabriel Nascimento"]
-__license__ = "GPL"
-__version__ = "1.0.0"
-__maintainer__ = "Gabriel Nascimento"
-__email__ = "gabriel.nascimento@nsgeng.com"
-__status__ = "Development"
-
-
-from typing import Union
-# import ctypes
-# import OrcFxAPI as __ofx
-from OrcFxAPI import *
-
-# import classes as _classes
-from .classes import *
-from .sortlines import *
-from .objauxfuncs import *
-# import environment as envtools
-from .modal import *
-
-
-# ======= CONSTANTS ======== #
-requiredOrcFxVer = '11.3a'
-
-# ==== AUXILIARY METHODS ==== #
-class AuxFuncs:
-    def checkOrCreateFolder(self, path: str) -> bool:
-        """
-        Check if the folder exists and, case not, try to create
-        Returns false if don't exists and can't create
-        """
-        return afCheckOrCreateFolder(path)
-
-auxfuncs = AuxFuncs()
-
-# ==== MODEL CLASS ==== #
-class Model(orc.Model):
-    general: OrcaFlexGeneralObject
-    auxfuncs = auxfuncs
-   
-    def __checkOrcaFlexVersion(self) -> bool:
-        """Return True if the installed version of OrcaFlex is equal or newer than the required"""
-        if not checkOrcaFlexVersion(requiredOrcFxVer):
-            raise Exception(f'The OrcaFlex version is older then {requiredOrcFxVer}.')    
-
-    def getOrcaVersion() -> str:
-        """Return the installed OrcaFlex version as string"""
-        return getOrcaVersion()
-
-    def __getitem__(self, name: str) -> OrcaFlexObject:
-        return OrcaFlexObject(super().__getitem__(name)) 
-    
-    def findLineByName(self, name: str) -> OrcaFlexLineObject:
-        """Find a line object by its name"""
-        obj = self[name]
-        return OrcaFlexLineObject(obj)
+import os
+import ctypes
+import numpy as np
+import OrcFxAPI as __ofx
+from . import constants
+
+__char = ctypes.c_wchar
+__letters = 'abcdefghijklimnoprstuvwxyz'
+
+def getOrcaVersion() -> str:
+    """Return the installed OrcaFlex version as string"""
+    global __char, DLLVersion
+    _charArray16 = (__char * 16)()
+    OK = ctypes.c_long()
+    Status = ctypes.c_long()
+    __ofx._GetDLLVersion(None, 
+                        _charArray16,
+                        ctypes.byref(OK), 
+                        ctypes.byref(Status))
+    DLLVersion = str()
+    for i in range(16): 
+        c = _charArray16[i]
+        if c != '\x00': DLLVersion += c
+    return DLLVersion
+
+def __versionStrToNum(version: str):
+    vernum = str()
+    verletter = str()        
+    for c in version:
+        if __letters.find(c) < 0:
+            vernum += c
+    else:
+        verletter += c
+        letterpos = __letters.find(c)
+
+    return float(vernum + str(letterpos))
+
+def getOrcaVersionAsFloat() -> float:
+    """Return the installed OrcaFlex version as float"""
+    versionTxt = getOrcaVersion()
+    __versionStrToNum(versionTxt)
+
+def checkOrcaFlexVersion(requiredVersion: str) -> bool:
+    """Return True if the installed version of OrcaFlex is equal or newer than the required"""
+    return __isNewerOrEqualTo(requiredVersion)
+
+def __isNewerOrEqualTo(version: str) -> bool:
+    """
+    Verifies if the current version of OrcFxAPI.dll is equal or newer then the required version
+    * version: minimum required version of OrcFxAPI.dll
+    """
+    actualver = getOrcaVersion()
+    if __versionStrToNum(actualver) >= __versionStrToNum(version):
+        return True
+    else:
+        return False    
+
+
+def isConnectedToObj(connection: str) -> bool:
+    """Returns true if the connection refers to other object"""
+    if connection == 'Free' or connection == 'Fixed' or connection == 'Anchored':
+        return False
+    else:
+        return True
+
+def compareStrings(
+        strA: str, 
+        strB: str, 
+        partialMatch: bool=False
+        ) -> bool:
+    if partialMatch:
+        n = min(len(strA), len(strB))
+        strA = strA[:n]
+        strB = strB[:n]    
+    # print(f'strA={strA} | strB={strB}')
+    return strA == strB
+
+def strInStrList(
+        str: str,
+        strList: list[str],
+        partialMatch: bool=False
+        ) -> bool:    
+    for s in strList:
+        if compareStrings(s, str, partialMatch): return True
+    return False
+
+def afCheckOrCreateFolder(path: str) -> bool:
+    """
+    Check if the folder exists and, case not, try to create
+    Returns false if don't exists and can't create
+    """
+    if os.path.isdir(path):
+        return True
+    else:
+        try:
+            os.mkdir(path)
+        except Exception as error:
+            print(f'Error! Could not create the path {path}. {error}')
+            return False
+        else:
+            return True
+
+def getGlobalCoordinates(
+        line: __ofx.OrcaFlexLineObject
+        ) -> tuple[list[float], list[float]]:
+    """
+    Returns the global coordinates of a line end
+    """
+    EndAConnection = line.EndAConnection
+    EndBConnection = line.EndBConnection
+    line.EndAConnection = 'Fixed'
+    line.EndBConnection = 'Fixed'
+    endA = [line.EndAX, line.EndAY, line.EndAZ]
+    endB = [line.EndBX, line.EndBY, line.EndBZ]
+    line.EndAConnection = EndAConnection
+    line.EndBConnection = EndBConnection
+    return endA, endB
+
+def getIntermadiatePos(
+        endA: list[float], 
+        endB: list[float], 
+        positionRatio: float
+        ) -> list[float]:
+    """Returns an intermediate position based on two points and a position ratio"""
+    p1, p2 = np.array(endA), np.array(endB)
+    pos = (p2-p1)*positionRatio + p1
+    return pos.tolist().copy()
+
+
+# Searchs for the highest rise or fall for a given seastate (defined in the input OrcaFlex model)
+# Save this file in the same folder of you code and include the following line in the library section: 
+# 'from Orc_SearchWave import GetLargestRiseAndFall, SetReducedSimDuration'
+def __TxtToFloat(txt: str):
+    '''
+    convert string to float, replacing ',' by '.', if necessary
+    '''
+    txt = txt.replace(',', '.')
+    return float(txt)
+
+def isRegularWave(waveType: str) -> bool:
+    if waveType in constants.regularWaveTypes: return True
+    elif waveType in constants.irregularWaveTypes: return False
+    else:
+        print(f'Warning! Wave type {waveType} not recognized. Considered as irregular.')
+        return False
+
+def SetReducedSimDuration(
+        model: __ofx.Model, 
+        reducedDuration: float = 200., 
+        refstormduration = 10800.,
+        fallOrRise: str ='rise', # 'rise' or 'fall'
+        waveTrainIndex: int = 0,
+        extremeWavePosition: list[float] = [0.,0.]
+        ) -> None:
+    '''
+    Reduces the simulation time for irreguar wave based on the highest fall/rise
+        - model: OrcaFlex loaded model
+        - reducedDuration: The simulation time after reducing. Used for the Stage 1. 
+        - refstormduration: wave duration along which the highest rise/fall will be searched
+        - fallOrRise: if time selection is based on the largest 'fall' or 'rise' event
+        - waveTrainIndex: based on which wave train largest fall or rise must be selected
+        - extremeWavePosition: position of wave origin for search
+
+        Obs.: the Tp value defined in the model will be used for the Stage 0.
+    '''        
+    env = model.environment
+    previousWaveTrainIndex = env.SelectedWaveTrainIndex
+    env.SelectedWaveTrainIndex = waveTrainIndex
+
+    if isRegularWave(env.WaveType):
+        raise Exception(f'Reduced simulation time approach is only \
+                        valid for irregular waves. Wave type{env.WaveType} not supported.')
     
-    def getAllLines(self, includeStiffeners: bool = True) -> LineSelection:
-        """Returns a list of all line objects"""
-        lineList = LineSelection(self)
-        for obj in self.objects:
-            if obj.type == orc.ObjectType.Line:
-                lineList.append(OrcaFlexLineObject(obj))
-                
-        if not includeStiffeners: # remove the stiffeners (line internally created by OrcaFlex due to attachements)
-            stiffenerNames = []
-            for line in lineList: stiffenerNames.extend(line.AttachmentName)                
-            newList = []
-            for line in lineList:
-                if not line.name in stiffenerNames: newList.append(line)
-            lineList = newList
-            
-        return lineList
-
-    def getLineList(
-            self, 
-            groupName: Union[str, None] = None, 
-            includeSubgroups: bool = False
-            ) -> LineSelection:
-        """
-        Returns all lines in the model which belongs to the defined group with or not its subgroups
-        """            
-        # if groupName:
-        #     grouObj = self[groupName]
-        #     selectedList = list(grouObj.GroupChildren(recurse=includeSubgroups))
-        # else:
-        #     selectedList = list(self.objects)
-
-        # for obj in selectedList:
-        #     if obj.type == orc.ObjectType.Line:
-        #         result.append(OrcaFlexLineObject(obj))
-        #     # elif groupName and includeSubgroups and obj.type == orc.ObjectType.BrowserGroup:
-        #     #     result.extend(self.getLineList(obj.Name))
-        result = LineSelection(self)
-        getLinesToList(self, groupName, includeSubgroups, result)
-        return result
-    
-    def sortPathInterconnectedLines(
-            self,
-            lineList: list[OrcaFlexLineObject]
-            ) -> LineSelection:
-        """
-        Returns a sorted list of interconnected lines, based on its connections (e.g., path from first to last)
-        The result is unpredictable if not all lines are connected or if there are connection between more than two lines
-        """              
-        newList = sortPathInterconnectedLines(lineList)
-        returnList = LineSelection(self)
-        for obj in newList: returnList.append(obj)
-        return returnList
+    # env.WaveTimeOrigin = 0 # uses the value defined by user
+    # prevWavePreviewPosition = [env.WavePreviewPositionX, env.WavePreviewPositionY]
+    env.WavePreviewPositionX = extremeWavePosition[0]
+    env.WavePreviewPositionY = extremeWavePosition[1]
     
+    tRise, tFall = GetLargestRiseAndFall(model, WaveSearchDuration=refstormduration)
+    if fallOrRise == 'rise': tSel = tRise
+    elif fallOrRise == 'fall': tSel = tFall
+    else: raise Exception(f'Input {fallOrRise} not allowed to "fallOrRise".')
 
-    def getUnconnectedConstraints(self) -> list[OrcaFlexObject]:
-        """
-        Returns the list of constraints to which there is not a line connected
-        """
-        constraintChildren = {}
-        for obj in self.objects:
-            if obj.type == orc.ObjectType.Constraint:
-                constraintChildren[obj.name] = 0
-        
-        lines = self.getLineList()  
-        for line in lines:
-            for endObj in [line.EndAConnection, line.EndBConnection]:
-                if endObj in constraintChildren:
-                    constraintChildren[endObj] += 1
-
-        resultList = []
-        for constraint, n in constraintChildren.items():
-            if n == 0:
-                resultList.append(constraint)
-
-        return resultList
+    env.WaveTimeOrigin = -tSel + reducedDuration/2
     
-    def CreateLine(self, name: Optional[str] = None) -> OrcaFlexLineObject:
-        newObj = self.CreateObject(ObjectType.Line, name)
-        return OrcaFlexLineObject(newObj)    
-
-    def deleteObjs(self, objects: list[str | OrcaFlexObject]):
-        for obj in objects:
-            self.DestroyObject(obj)
-
-    def CalculateModal(
-            self, 
-            lineName: str | None = None,
-            firstMode: int = -1,
-            lastMode: int = -1            
-            ) -> Modes:
-        """
-        Performs modal analysis and returns the result (Modes object)
-        If no lineName is especified, includes all lines the analysis
-        """
-
-        # check if static calculation was performed
-        if self.state == orc.ModelState.Reset: 
-            self.CalculateStatics()
-
-        if lineName == None: includeCouped = True
-        else: includeCouped = False
-        
-        specs = orc.ModalAnalysisSpecification(True, firstMode, lastMode, includeCouped) # TODO: check other default inputs
+    general = model.general
+    Tz = env.WaveTz
+    general.StageDuration[0] = Tz
+    general.StageDuration[1] = reducedDuration
+
+    env.SelectedWaveTrainIndex = previousWaveTrainIndex
+    # env.WavePreviewPositionX, env.WavePreviewPositionY = prevWavePreviewPosition[0], prevWavePreviewPosition[1]
+
+
+def GetLargestRiseAndFall(
+        model: __ofx.Model, 
+        filename: str = 'SearchWave', 
+        WaveSearchDuration: float = 10800
+        ) -> tuple[float,float]:
+    '''
+    Inputs:
+        - model: OrcaFlex model with the defined wave (type, Tp, Hs ...)
+        - filename (optional): Temporary file that will be used in the search.
+        - WaveSearchDuration (optional): Period, in seconds, to find the highest rise or fall. Default = 10080
         
-        if lineName != None: obj = self[lineName]
-        else: obj = self
-
-        modes = _classes.Modes(obj, specs)
-
-        return modes
-
-
-
-class LineSelection(list[OrcaFlexLineObject]):
-    def __init__(self, model: Model):
-        super().__init__()
-        self.model = model
-
-    def setGroup(self, groupName: str) -> None:
-        group = self.model[groupName]
-        for line in self:
-            line.groupParent = group
-
-    def setLog(self, logResults: bool) -> None:
-        """Defines if the results of the line should be stored (logged) or not for all lines in this selection"""
-        for line in self:
-            line.setLog(logResults)
-
-    def setMeshSize(
-            self,
-            nSegs: int = None,
-            targetLength: float = None
-            ):
-        """Set the length/number of segments for all sections of all lines in this selection"""
-        for line in self:
-            line.setMeshSize(nSegs, targetLength)
-
-    def selectByName(
-            self, 
-            name: Union[str, list[str]]
-            ) -> LineSelection:
-        if type(name) == str: nameList = [name]
-        else: nameList = name
-        resultList = LineSelection(self.model)
-        for line in self:
-            if line.Name in nameList:
-                resultList.append(line)
-        return resultList
-
-    def selectByType(
-            self, lineType: Union[list[str], str], 
-            partialMatch: bool = False
-            ) -> LineSelection:
-        if type(lineType) == str: lineTypeGroup = [lineType]
-        else: lineTypeGroup = lineType
-        resultList = LineSelection(self.model)
-        for line in self:
-            for lt in line.LineType:
-                if strInStrList(lt, lineTypeGroup, partialMatch):
-                    resultList.append(line)
-        return resultList
-
-    def selectLinesByPosition(
-            self,
-            xLimits: tuple[Union[float,None], Union[float,None]] = (None, None),
-            yLimits: tuple[Union[float,None], Union[float,None]] = (None, None),
-            zLimits: tuple[Union[float,None], Union[float,None]] = (None, None)
-            ) -> LineSelection:
-        """
-        Select lines in the model based on its ends position
-        """
-        if not len(self):
-            raise Exception('Error! This selction is empty.')
-
-        # cloneModel = orc.Model() # creates a 'dummy' model (only to set fixed connections and get global coords)
-        resultList = LineSelection(self.model)
-        for line in self:
-            # clone = line.CreateClone(model=cloneModel) # copy object to 'dummy' model
-            clone = line.CreateClone() # copy object to 'dummy' model
-            clone.EndAConnection = 'Fixed' # ensures global coordinates
-            clone.EndBConnection = 'Fixed' # ensures global coordinates
-            minLimits = [xLimits[0], yLimits[0], zLimits[0]]            
-            maxLimits = [xLimits[1], yLimits[1], zLimits[1]]
-            xVls = [clone.EndAX, clone.EndBX]
-            yVls = [clone.EndAY, clone.EndBY]
-            zVls = [clone.EndAZ, clone.EndBZ]
-            values = [xVls, yVls, zVls]
-            include = True
-            for vEnds, minLim, maxLim in zip(values, minLimits, maxLimits):
-                for v in vEnds:
-                    if minLim != None: # check min
-                        if v < minLim: include = False
-                    if maxLim != None: # check max
-                        if v > maxLim: include = False
-            if include: resultList.append(line)
-            # cloneModel.DestroyObject(clone) # free memory
-            self.model.DestroyObject(clone) # free memory
-
-        return resultList
+    Outputs:
+        - tuple (t1, t2) with two values: time of highest rise and fall
+    '''        
+    env = model.environment
+
+    #assuming we want to look over the first 3hrs
+    env.WaveSearchFrom = 0.0
+    env.WaveSearchDuration = WaveSearchDuration
+    #i'm using Largest Rise as the metric to judge which wave I want
+    #so I don't actually need to report any of the individual waves 
+    #so I set the search parameters to arbitrarily high values:
+    env.WaveSearchMinHeight = 1e9
+    env.WaveSearchMinSteepness = 1e9
+
+    file = filename + '.txt'
+    try:   
+        model.SaveWaveSearchSpreadsheet(file)
+    except:
+        raise Exception(f'Error when saving temporary file {file}.')
+
+    #parse the txt file to find the line with the largest rise and fall
+    with open(file) as f:
+        for row in f:
+            if 'Largest rise' in row:
+                timeOfLargestRise = __TxtToFloat(row.split()[3]) #get the global time of the largest rise
+            elif 'Largest fall' in row:
+                timeOfLargestFall = __TxtToFloat(row.split()[3]) #get the global time of the largest fall
+    
+    os.remove(file) # delete temp file
 
+    t0 = env.WaveTimeOrigin
 
+    return timeOfLargestRise-t0, timeOfLargestFall-t0
```

### Comparing `nsgorcfx-1.0.6/src/NsgOrcFx/environment.py` & `nsgorcfx-1.0.7/src/NsgOrcFx/environment.py`

 * *Files identical despite different names*

### Comparing `nsgorcfx-1.0.6/src/NsgOrcFx/modal.py` & `nsgorcfx-1.0.7/src/NsgOrcFx/modal.py`

 * *Files identical despite different names*

### Comparing `nsgorcfx-1.0.6/src/NsgOrcFx/objauxfuncs.py` & `nsgorcfx-1.0.7/src/NsgOrcFx/objauxfuncs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# from typing import Union
+from typing import Union
 import OrcFxAPI as __ofx
 from .classes import *
 
 
 def getLinesToList(
         model: __ofx.Model, 
         groupName: Union[str, None] = None,
```

### Comparing `nsgorcfx-1.0.6/src/NsgOrcFx/sncurves.py` & `nsgorcfx-1.0.7/src/NsgOrcFx/sncurves.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,24 +17,24 @@
     N_boundary: int         # number of cycles between the low and high cycle regions
     m2: float = None        # m for the hogh cycle region (N > N_boundary)
     log_a2: float = None    # log(a) for the hogh cycle region (N > N_boundary)
 
     def setToAnalysis(
             self,
             analysis: _ofx.FatigueAnalysis,
-            tableLineNumber: int = 1
+            snCurveIndex: int = 0
             ) -> None:
         """
         Set the current curve to the Fatigue Analysis (S-N curves page)
         * analysis: FatigueAnalysis object
         * tableLineNumber: line of the table of S-N curves page where the curve will be defined
         """
-        if analysis.SNcurveCount < tableLineNumber: analysis.SNcurveCount = tableLineNumber
-        analysis.SelectedSNcurveIndex = tableLineNumber-1
-        analysis.SNcurveName[tableLineNumber-1] = self.name + ' ' + self.environment
+        if analysis.SNcurveCount < snCurveIndex+1: analysis.SNcurveCount = snCurveIndex+1
+        analysis.SelectedSNcurveIndex = snCurveIndex
+        analysis.SNcurveName[snCurveIndex] = self.name + ' ' + self.environment
         analysis.SNcurveSpecificationMethod = 'Parameters'
         analysis.SNcurvem1 = self.m1
         analysis.SNcurveloga1 = self.log_a1 + 3*self.m1 # pressure in kPa
         analysis.SNcurveRegionBoundary = self.N_boundary
         analysis.SNcurvem2 = self.m2
         analysis.SNcurveMeanStressModel = 'None'
```

### Comparing `nsgorcfx-1.0.6/src/NsgOrcFx/sortlines.py` & `nsgorcfx-1.0.7/src/NsgOrcFx/sortlines.py`

 * *Files identical despite different names*

### Comparing `nsgorcfx-1.0.6/src/NsgOrcFx/utils.py` & `nsgorcfx-1.0.7/src/NsgOrcFx/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import OrcFxAPI as __ofx
 from . import constants as __constants
 import numpy as np
 from scipy import interpolate
 
 def dofNumber(dofString: str) -> int:
     """get the dof number. Start with 'Ux' = 1"""
@@ -70,7 +71,11 @@
     yNewLists = []
     for yValues in yValueLists:
         f = interpolate.interp1d(xValues, yValues, kind)
         yNew = f(xNew)
         yNewLists.append(yNew)
 
     return xNew, yNewLists
+
+def getFileExtension(file: str) -> str:
+    _, extension = os.path.splitext(file)
+    return extension
```

### Comparing `nsgorcfx-1.0.6/src/NsgOrcFx/weight.py` & `nsgorcfx-1.0.7/src/NsgOrcFx/weight.py`

 * *Files identical despite different names*

### Comparing `nsgorcfx-1.0.6/src/NsgOrcFx/weightaux.py` & `nsgorcfx-1.0.7/src/NsgOrcFx/weightaux.py`

 * *Files identical despite different names*

### Comparing `nsgorcfx-1.0.6/src/NsgOrcFx.egg-info/PKG-INFO` & `nsgorcfx-1.0.7/src/NsgOrcFx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NsgOrcFx
-Version: 1.0.6
+Version: 1.0.7
 Summary: Package with additional tools to the OrcFxAPI package
 Author-email: NSG Engenharia <comercial@nsgeng.com>
 Project-URL: Homepage, https://github.com/NSG-Engenharia/NsgOrcFx
 Project-URL: Issues, https://github.com/NSG-Engenharia/NsgOrcFx/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

