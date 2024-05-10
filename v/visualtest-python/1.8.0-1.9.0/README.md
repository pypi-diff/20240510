# Comparing `tmp/visualtest_python-1.8.0-py3-none-any.whl.zip` & `tmp/visualtest_python-1.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 28160 bytes, number of entries: 12
--rw-r--r--  2.0 unx      121 b- defN 24-Mar-22 15:35 sbvt/__init__.py
--rw-r--r--  2.0 unx    12158 b- defN 24-Mar-12 12:03 sbvt/api.py
--rw-r--r--  2.0 unx    10229 b- defN 24-Mar-12 12:03 sbvt/app.py
--rw-r--r--  2.0 unx    48182 b- defN 24-Mar-12 12:03 sbvt/browser.py
+Zip file size: 29105 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      121 b- defN 24-May-10 16:02 sbvt/__init__.py
+-rw-r--r--  2.0 unx    12832 b- defN 24-May-09 10:07 sbvt/api.py
+-rw-r--r--  2.0 unx    11350 b- defN 24-May-10 16:02 sbvt/app.py
+-rw-r--r--  2.0 unx    50235 b- defN 24-May-09 10:06 sbvt/browser.py
 -rw-r--r--  2.0 unx     7465 b- defN 24-Mar-12 12:03 sbvt/imagetools.py
 -rw-r--r--  2.0 unx      548 b- defN 23-May-11 09:06 sbvt/timer.py
--rw-r--r--  2.0 unx    21344 b- defN 24-Mar-12 12:03 sbvt/visualtest.py
--rw-r--r--  2.0 unx     1073 b- defN 24-Mar-22 15:36 visualtest_python-1.8.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3898 b- defN 24-Mar-22 15:36 visualtest_python-1.8.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-22 15:36 visualtest_python-1.8.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 24-Mar-22 15:36 visualtest_python-1.8.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      938 b- defN 24-Mar-22 15:36 visualtest_python-1.8.0.dist-info/RECORD
-12 files, 106053 bytes uncompressed, 26604 bytes compressed:  74.9%
+-rw-r--r--  2.0 unx    22097 b- defN 24-May-09 10:07 sbvt/visualtest.py
+-rw-r--r--  2.0 unx     1073 b- defN 24-May-10 16:03 visualtest_python-1.9.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3898 b- defN 24-May-10 16:03 visualtest_python-1.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-10 16:03 visualtest_python-1.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-May-10 16:03 visualtest_python-1.9.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      938 b- defN 24-May-10 16:03 visualtest_python-1.9.0.dist-info/RECORD
+12 files, 110654 bytes uncompressed, 27549 bytes compressed:  75.1%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: sbvt/timer.py
 Comment: 
 
 Filename: sbvt/visualtest.py
 Comment: 
 
-Filename: visualtest_python-1.8.0.dist-info/LICENSE
+Filename: visualtest_python-1.9.0.dist-info/LICENSE
 Comment: 
 
-Filename: visualtest_python-1.8.0.dist-info/METADATA
+Filename: visualtest_python-1.9.0.dist-info/METADATA
 Comment: 
 
-Filename: visualtest_python-1.8.0.dist-info/WHEEL
+Filename: visualtest_python-1.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: visualtest_python-1.8.0.dist-info/top_level.txt
+Filename: visualtest_python-1.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: visualtest_python-1.8.0.dist-info/RECORD
+Filename: visualtest_python-1.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sbvt/__init__.py

```diff
@@ -1,4 +1,4 @@
 # this import statement is here for context.py in tests folder
 from .visualtest import VisualTest
 
-__version__ = '1.8.0'
+__version__ = '1.9.0'
```

## sbvt/api.py

```diff
@@ -70,14 +70,16 @@
             api.headers.update({
                 'Authorization': f'Bearer {projectToken}',
                 'sbvt-client': 'sdk',
                 'sbvt-sdk': 'python',
                 'sbvt-sdk-version': sbvt.__version__
             })
         self.testRun = None
+        self.scmCommitId = None
+        self.scmBranch = None
 
     def getDeviceInfo(self, userAgentInfo, driverCapabilities):
 
         url = f'{Api.baseUrl}/device-info/'
         log.info(f'calling API to get device info at: {url}')
         response = api.post(url, json={'userAgentInfo': userAgentInfo, 'driverCapabilities': driverCapabilities})
         if response.status_code in range(200, 300):
@@ -118,14 +120,21 @@
         else:
             jsonObject = {
                 'testRunName': testRunName,
                 'testGroupId': testGroupId,
                 'sdk': 'python',
                 'sdkVersion': sbvt.__version__,
             }
+            
+        if self.scmCommitId:
+            jsonObject['scmCommitId'] = self.scmCommitId
+            
+        if self.scmBranch:
+            jsonObject['scmBranch'] = self.scmBranch
+        
         response = api.post(url, json=jsonObject)
         if response.status_code in range(200, 300):
             return response.json()
         else:
             log.error(f'Failed to create testRun. HTTP Response: {response.json()}')
             raise Exception(f'Failed to create testRun. HTTP Response: {response.json()}')
 
@@ -244,14 +253,24 @@
             url = f'{Api.cdnUrl}/{scriptName}.min.js'
             response = api.get(url)
             return response.text
         else:
             log.error(f'Invalid scriptName for getToolkit from cdn: {scriptName}')
             raise Exception(f'Invalid scriptName for getToolkit from cdn: {scriptName}')
 
+    @staticmethod
+    def getDevicesList(scriptName=None):
+        if scriptName in ['apple-devices']:
+            url = f'{Api.cdnUrl}/{scriptName}.json'
+            response = api.get(url)
+            return response.text
+        else:
+            log.error(f'Invalid scriptName for getToolkit from cdn: {scriptName}')
+            raise Exception(f'Invalid scriptName for getToolkit from cdn: {scriptName}')
+
     def getTestRunResult(self, timeout=3):
         if not self.testRun:
             raise Exception("Cannot run get testrun result without first taking a capture()")
         i = 0
         comparisons = { 'pending': 1 }
         while comparisons['pending'] > 0 and i < timeout * 4 * 60:
             url = f'{Api.baseUrl}/projects/{self.projectId}/testruns/{self.testRun["testRunId"]}?expand=comparison-totals'
```

## sbvt/app.py

```diff
@@ -1,7 +1,8 @@
+import json
 import os
 import logging
 from .imagetools import ImageTools
 from .timer import StopWatch
 from .api import Api
 
 log = logging.getLogger(f'vt.{os.path.basename(__file__)}')
@@ -23,30 +24,44 @@
     Returns:
         Class instance
     """
 
     def __init__(self, driver, limits: dict = {}):
 
         # setup api
+        self.devicePixelRatio = 1
+        self.statusbarHeight = 0
+        self.bottomBarHeight = 0
         self._api = Api()
         log.info(f'Capabilities from driver: {driver.capabilities}')
         self._driver = driver
+        if self._driver.capabilities['platformName'] == 'Android':
+            self.devicePixelRatio = float(self._driver.capabilities['pixelRatio'])
+            self.statusbarHeight = self._driver.capabilities['statBarHeight']
+        else:
+            self._appleDevicesList = Api.getDevicesList('apple-devices')
+            data = json.loads(self._appleDevicesList)
+            for device in data:
+                if device["name"] == self._driver.capabilities.get("deviceName"):
+                    self.devicePixelRatio = device["scale"]
+                    self.statusbarHeight = device["statusBar"]["portrait"]*self.devicePixelRatio
         self._userAgentInfo = {
-            'appPackage':self._driver.capabilities["appPackage"],
-            'appActivity':self._driver.capabilities["appActivity"] if "appActivity" in self._driver.capabilities else None,
-            'appiumDriverType':self._driver.capabilities["automationName"],
+            'appPackage': self._driver.capabilities["appPackage"] if "appActivity" in self._driver.capabilities else self._driver.capabilities["bundleId"],
+            'appActivity':self._driver.capabilities["appActivity"] if "appActivity" in self._driver.capabilities else self._driver.capabilities["bundleId"],
+            'appiumDriverType':self._driver.capabilities["automationName"].lower(),
             'driverType':'Appium',
-            'deviceName': self._driver.capabilities.get("deviceModel"),
-            'devicePixelRatio':self._driver.capabilities["pixelRatio"],
+            'deviceName': self._driver.capabilities.get("deviceModel") or self._driver.capabilities.get("deviceName"),
+            'devicePixelRatio':self.devicePixelRatio,
             'deviceType':'mobile',
             'orientation':'portrait',
             'osName':self._driver.capabilities["platformName"],
             'osVersion':self._driver.capabilities["platformVersion"],
-            'screenHeight':self._driver.capabilities["deviceScreenSize"].split("x")[1],
-            'screenWidth':self._driver.capabilities["deviceScreenSize"].split("x")[0],}
+            'screenHeight':self._driver.get_window_size()["height"]*self.devicePixelRatio,
+            'screenWidth':self._driver.get_window_size()["width"]*self.devicePixelRatio
+        }
         if "deviceManufacturer" in self._driver.capabilities:
             self._userAgentInfo["deviceName"] = self._driver.capabilities["deviceManufacturer"].capitalize() + " " + self._userAgentInfo["deviceName"].capitalize()
         self._deviceInfo = self._api.getDeviceInfo(self._userAgentInfo, driver.capabilities)
         self._deviceInfo['deviceName'] = self._userAgentInfo["deviceName"]
         
         log.info(f'limits: {limits}')
         if 'MAX_IMAGE_PIXELS' in limits:
@@ -101,16 +116,15 @@
         if type(minutes) != int:
             raise Exception(f'MAX_TIME_MIN must be an integer')
         if minutes not in range(0, 11):
             raise Exception(f'MAX_TIME_MIN must be between 0 and 10 minutes')
         self._MAX_TIME_MIN = minutes
  
     def _getPageDimensions(self):
-        specialDevices = ['Pixel 3a']
-        if int(self._driver.capabilities['platformVersion'].split('.')[0]) < 11 or self._driver.capabilities['deviceModel'] in specialDevices :
+        if int(self._driver.capabilities['platformVersion'].split('.')[0]) < 11 and self._driver.capabilities['platformName'] == 'Android':
             jsonDimensions = self._driver.capabilities['viewportRect']
         else:
             jsonDimensions = self._driver.get_window_size()
             if 'orientation' in self.capabilities and self.capabilities['orientation'] == 'LANDSCAPE':
                 jsonDimensions['width'] = float(self.capabilities['deviceScreenSize'].split('x')[1]) 
             
         height = jsonDimensions['height']
@@ -128,15 +142,15 @@
                     "height": height,
                     "width":  width
                 },
                 "fullpage": {
                     "height": height,
                     "width": width
                 },
-                "devicePixelRatio": float(self._driver.capabilities['pixelRatio']),
+                "devicePixelRatio": self.devicePixelRatio,
                 "initialScroll": {
                     'x': 0, 
                     'y': 0
                 }
             }
 
         # for now, take the window.inner dimensions as viewport
@@ -154,20 +168,22 @@
         log.info(f'Size Test: image dimensions: {testImageWidth}x{testImageHeight}')
 
         self._cropEachBottom = None
         self._cropEachTop = None
         self._cropEachLeft = None
 
         if 'orientation' in self.capabilities and self._driver.capabilities['orientation'] == 'LANDSCAPE':
-            if int(self._driver.capabilities['platformVersion'].split('.')[0]) < 11 or self._driver.capabilities['deviceModel'] in specialDevices :
+            if int(self._driver.capabilities['platformVersion'].split('.')[0]) < 11:
                 jsonDimensions = self._driver.capabilities['viewportRect']
             else:
                 jsonDimensions = self._driver.get_window_size()
-        self._cropEachBottom = testImageHeight - (jsonDimensions['height'] ) - self._driver.capabilities['statBarHeight']
-        self._cropEachTop = self._driver.capabilities['statBarHeight']
+                
+        if self._driver.capabilities['platformName'] == 'Android':
+            self._cropEachBottom = testImageHeight - (jsonDimensions['height']) - self.statusbarHeight
+        self._cropEachTop = self.statusbarHeight
         self._cropEachLeft = testImageWidth - (jsonDimensions['width'] )
         log.info(
             f'Size Test: Appium Android device has {self._cropEachBottom}px extra pixels to crop on each image at the bottom')
 
     
     def takeAppiumViewportScreenshot(self, name, options):
         """
@@ -221,17 +237,19 @@
         if self._debug:
             debugImageName = f'{name}-aftercut.png'
             debugImagePath = os.path.join(debugImageDir, debugImageName)
             with open(debugImagePath, 'wb') as outfile:
                 outfile.write(imageBinary)
                 outfile.close()
 
-        expectedImageWidth = self.viewportWidth / self.devicePixelRatio
-        expectedImageHeight = self.viewportHeight / self.devicePixelRatio
-        
+        expectedImageWidth = self.viewportWidth 
+        expectedImageHeight = self.viewportHeight - (self.bottomBarHeight/self.devicePixelRatio) - (self.statusbarHeight/self.devicePixelRatio)
+        if self._driver.capabilities['platformName'] == 'Android':
+            expectedImageWidth = self.viewportWidth / self.devicePixelRatio 
+            expectedImageHeight = (self.viewportHeight - self.bottomBarHeight)/self.devicePixelRatio
 
         totalTime = self.watch.stop()
         log.info(f'Total viewport capture time duration: {totalTime} seconds')
         self.url = ""
         result = {
             'imagePath': None,
             'imageSize': {
```

## sbvt/browser.py

```diff
@@ -3,14 +3,15 @@
 import math
 import logging
 import json
 import colour
 from io import BytesIO
 from PIL import Image
 from sys import getsizeof
+from axe_selenium_python import Axe
 from .imagetools import ImageTools
 from .timer import StopWatch
 from .api import Api
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.wait import WebDriverWait
 
 log = logging.getLogger(f'vt.{os.path.basename(__file__)}')
@@ -1012,14 +1013,67 @@
         }
 
         log.info(f'Result: {result}')
         result['dom'] = self.dom #add dom after logging result
         result['imageBinary'] = imageBinary
         return result
 
+    def getAccessibilityViolationRules(self):
+        # Instantiate Axe and run accessibility checks
+        log.info(f'Instantiate Axe and running accessibility checks')
+        axe = Axe(self._driver)
+        axe.inject()
+        results = axe.run()
+
+        # If there are violations found
+        if len(results["violations"]) > 0:
+            log.info(f'Accessibility violations found.')
+            violationRules = []
+            for violation in results["violations"]:
+                for node in violation["nodes"]:
+                    # Get violation summary for each violation
+                    violationRuleSummary = self.getAccessibilityViolationSummary(violation, node)
+                    violationRules.append(violationRuleSummary)
+            log.info(f'Accessibility violations rules:{violationRules}')
+            return violationRules
+        else:
+            log.info(f'No accessibility violations found.')
+            return None
+
+    def getBoundingBox(self, node):
+        # Get bounding box of the element
+        try:
+            element = self._driver.find_element(by=By.CSS_SELECTOR, value=node["target"][0])
+            if element:
+                rect = element.rect
+                return {
+                    "x": rect["x"],
+                    "y": rect["y"],
+                    "width": rect["width"],
+                    "height": rect["height"],
+                    "target": node["target"][0],
+                    "html": node["html"]
+                }
+            return None
+        except:
+            return None
+    
+
+    def getAccessibilityViolationSummary(self, violation, node):
+        # Get violation rule along with its bounding box
+        boundingBox = self.getBoundingBox(node)
+        return {
+            "description": violation["description"],
+            "help": violation["help"],
+            "helpUrl": violation["helpUrl"],
+            "id": violation["id"],
+            "impact": violation["impact"],
+            "boundingBox": boundingBox
+        }
+
     def page_has_loaded(self):
         page_state = self._driver.execute_script('return document.readyState;')
         while page_state != 'complete':
             time.sleep(1)
             page_state = self._driver.execute_script(
                 'return document.readyState;')
```

## sbvt/visualtest.py

```diff
@@ -104,14 +104,19 @@
         self._api.isValidProjectToken()
         if type(driver).__module__ == 'appium.webdriver.webdriver':
             if driver.capabilities['platformName'] == 'Android':
                 if driver.capabilities['automationName'] == 'uiautomator2':
                     self.appium = True
                 else:
                     raise Exception('Appium driver must use uiautomator2 automationName.')
+            elif driver.capabilities['platformName'] == 'iOS':
+                if driver.capabilities['automationName'] == 'XCUITest':
+                    self.appium = True
+                else:
+                    raise Exception('Appium driver must use XCUITest automationName.')
             else:
                 raise Exception('Appium is only supported for Android devices.')
         else:
             self.appium = False
 
         if self.appium:
             self.driverManager = App(driver, limits)
@@ -153,14 +158,19 @@
 
         if "testRunId" in settings:
             if isinstance(settings['testRunId'], str):
                 self._api.testRun = {'testRunId': settings['testRunId']}
             else:
                 raise Exception('"testRunId" should be a str type.')
         
+        if 'SBVT_SCM_COMMIT_ID' in os.environ.keys():
+            self._api.scmCommitId = os.environ['SBVT_SCM_COMMIT_ID']
+        if 'SBVT_SCM_BRANCH' in os.environ.keys():
+            self._api.scmBranch = os.environ['SBVT_SCM_BRANCH']
+        
         log.info(f'final instance settings: {self._settings}')
 
     @property
     def projectToken(self):
         """
         Get projectToken (str)
         """
@@ -369,14 +379,15 @@
             'imageHeight': screenshotResult['imageSize']['height'],
             'ignoredElements': json.dumps(ignoreElements),
             'comparisonMode': comparisonMode,
             'sensitivity': sensitivity,
             'headless': headless,
             'driverType': driverType,
             'sdkDomUpload': True, # SDKs will upload dom to S3 directly and receive presigned URL if this flag is set
+            'violations': json.dumps(screenshotResult['violations']) if not self.appium else None
         }
         if self.appium:
             imageData['appiumDriverType'] = self.driverManager._userAgentInfo['appiumDriverType']
         
         imageData.update(self.driverManager._deviceInfo) # required information about device/os/browser
 
         # these two are informational and just used to store - not required
@@ -426,14 +437,16 @@
             if len(elementsNotFound) > 0:
                 raise Exception(f'Some ignoreElements were not found on the page: {",".join(elementsNotFound)}')
             else:
                 self.driverManager._injectIgnoreElements(options['ignoreElements'])
 
         if 'freezePage' in options and not isinstance(options['freezePage'], bool):
                 raise Exception(f'freezePage must be of type "bool"')
+
+        violationRules = self.driverManager.getAccessibilityViolationRules()
         
         if 'element' in options:
             screenshotResult = self.driverManager.takeElementScreenshot(options)
             imageType = 'element'
         elif 'viewport' in options and options['viewport'] == True:
 
             screenshotResult = self.driverManager.takeViewportScreenshot(options)
@@ -441,15 +454,15 @@
         else:
             if 'lazyload' in options and type(options['lazyload']) != int or ('lazyload' in options and (options['lazyload'] < 0 or options['lazyload'] > 10000)):
                     raise Exception('"lazyload" value must be an integer between 0 and 10000 ms!')
 
             screenshotResult = self.driverManager.takeFullpageScreenshot(name, options)
 
             imageType = 'fullpage'
-        
+        screenshotResult['violations'] = violationRules
         return screenshotResult, imageType
 
     def printReport(self):
         
         comparisons = self._api.getTestRunResult()
         imageCount = comparisons["total"]
         print(f'View your {imageCount} {"capture" if imageCount == 1 else "captures"} here: ' + Fore.BLUE + self._api.testRun['appUrl'] + Style.RESET_ALL)
```

## Comparing `visualtest_python-1.8.0.dist-info/LICENSE` & `visualtest_python-1.9.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `visualtest_python-1.8.0.dist-info/METADATA` & `visualtest_python-1.9.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visualtest-python
-Version: 1.8.0
+Version: 1.9.0
 Summary: Python SDK for SmartBear VisualTest via Selenium WebDriver
 Home-page: https://github.com/SmartBear/visualtest-python
 Author: Luke Kende
 Author-email: luke.kende@smartbear.com
 Keywords: visual testing,UI testing,GUI testing,UX testing,screenshots,full page screenshots,image comparisons,regression testing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

