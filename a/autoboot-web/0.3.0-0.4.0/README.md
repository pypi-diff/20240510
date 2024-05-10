# Comparing `tmp/autoboot-web-0.3.0.tar.gz` & `tmp/autoboot-web-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoboot-web-0.3.0.tar", last modified: Thu Nov 30 02:22:33 2023, max compression
+gzip compressed data, was "autoboot-web-0.4.0.tar", last modified: Thu Nov 30 10:44:10 2023, max compression
```

## Comparing `autoboot-web-0.3.0.tar` & `autoboot-web-0.4.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 02:22:33.006081 autoboot-web-0.3.0/
--rw-r--r--   0 yizzuide   (501) staff       (20)     1065 2023-11-29 06:50:51.000000 autoboot-web-0.3.0/LICENSE.txt
--rw-r--r--   0 yizzuide   (501) staff       (20)        0 2023-11-29 06:50:51.000000 autoboot-web-0.3.0/MANIFEST.in
--rw-r--r--   0 yizzuide   (501) staff       (20)      659 2023-11-30 02:22:33.011469 autoboot-web-0.3.0/PKG-INFO
--rw-r--r--   0 yizzuide   (501) staff       (20)       76 2023-11-29 06:50:51.000000 autoboot-web-0.3.0/README.md
-drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 02:22:32.996500 autoboot-web-0.3.0/autoboot_web/
--rw-r--r--   0 yizzuide   (501) staff       (20)       55 2023-11-29 06:50:51.000000 autoboot-web-0.3.0/autoboot_web/__init__.py
--rw-r--r--   0 yizzuide   (501) staff       (20)     1105 2023-11-29 07:56:56.000000 autoboot-web-0.3.0/autoboot_web/http_properties.py
-drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 02:22:32.999939 autoboot-web-0.3.0/autoboot_web/middleware/
--rw-r--r--   0 yizzuide   (501) staff       (20)       80 2023-11-29 06:50:51.000000 autoboot-web-0.3.0/autoboot_web/middleware/__init__.py
--rw-r--r--   0 yizzuide   (501) staff       (20)      340 2023-11-29 06:50:51.000000 autoboot-web-0.3.0/autoboot_web/middleware/uniform.py
-drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 02:22:33.001036 autoboot-web-0.3.0/autoboot_web/mvc/
--rw-r--r--   0 yizzuide   (501) staff       (20)       91 2023-11-29 06:50:51.000000 autoboot-web-0.3.0/autoboot_web/mvc/__init__.py
-drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 02:22:33.004681 autoboot-web-0.3.0/autoboot_web/mvc/annotation/
--rw-r--r--   0 yizzuide   (501) staff       (20)      133 2023-11-29 06:50:51.000000 autoboot-web-0.3.0/autoboot_web/mvc/annotation/__init__.py
--rw-r--r--   0 yizzuide   (501) staff       (20)     3391 2023-11-29 06:50:51.000000 autoboot-web-0.3.0/autoboot_web/mvc/annotation/controller.py
--rw-r--r--   0 yizzuide   (501) staff       (20)     3540 2023-11-29 06:50:51.000000 autoboot-web-0.3.0/autoboot_web/mvc/apply_router.py
--rw-r--r--   0 yizzuide   (501) staff       (20)     2960 2023-11-29 07:57:38.000000 autoboot-web-0.3.0/autoboot_web/runner.py
--rw-r--r--   0 yizzuide   (501) staff       (20)     1658 2023-11-29 07:17:27.000000 autoboot-web-0.3.0/autoboot_web/web_properties.py
-drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 02:22:32.999147 autoboot-web-0.3.0/autoboot_web.egg-info/
--rw-r--r--   0 yizzuide   (501) staff       (20)      659 2023-11-30 02:22:32.000000 autoboot-web-0.3.0/autoboot_web.egg-info/PKG-INFO
--rw-r--r--   0 yizzuide   (501) staff       (20)      572 2023-11-30 02:22:32.000000 autoboot-web-0.3.0/autoboot_web.egg-info/SOURCES.txt
--rw-r--r--   0 yizzuide   (501) staff       (20)        1 2023-11-30 02:22:32.000000 autoboot-web-0.3.0/autoboot_web.egg-info/dependency_links.txt
--rw-r--r--   0 yizzuide   (501) staff       (20)       48 2023-11-30 02:22:32.000000 autoboot-web-0.3.0/autoboot_web.egg-info/requires.txt
--rw-r--r--   0 yizzuide   (501) staff       (20)       13 2023-11-30 02:22:32.000000 autoboot-web-0.3.0/autoboot_web.egg-info/top_level.txt
--rw-r--r--   0 yizzuide   (501) staff       (20)     1313 2023-11-29 06:50:51.000000 autoboot-web-0.3.0/pyproject.toml
--rw-r--r--   0 yizzuide   (501) staff       (20)      106 2023-11-30 02:22:33.016764 autoboot-web-0.3.0/setup.cfg
--rw-r--r--   0 yizzuide   (501) staff       (20)     1153 2023-11-30 02:20:02.000000 autoboot-web-0.3.0/setup.py
+drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 10:44:10.553017 autoboot-web-0.4.0/
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1065 2023-11-29 06:50:51.000000 autoboot-web-0.4.0/LICENSE.txt
+-rw-r--r--   0 yizzuide   (501) staff       (20)        0 2023-11-29 06:50:51.000000 autoboot-web-0.4.0/MANIFEST.in
+-rw-r--r--   0 yizzuide   (501) staff       (20)      659 2023-11-30 10:44:10.553126 autoboot-web-0.4.0/PKG-INFO
+-rw-r--r--   0 yizzuide   (501) staff       (20)       76 2023-11-29 06:50:51.000000 autoboot-web-0.4.0/README.md
+drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 10:44:10.548539 autoboot-web-0.4.0/autoboot_web/
+-rw-r--r--   0 yizzuide   (501) staff       (20)       55 2023-11-29 06:50:51.000000 autoboot-web-0.4.0/autoboot_web/__init__.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1105 2023-11-29 07:56:56.000000 autoboot-web-0.4.0/autoboot_web/http_properties.py
+drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 10:44:10.550975 autoboot-web-0.4.0/autoboot_web/middleware/
+-rw-r--r--   0 yizzuide   (501) staff       (20)       80 2023-11-29 06:50:51.000000 autoboot-web-0.4.0/autoboot_web/middleware/__init__.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      340 2023-11-29 06:50:51.000000 autoboot-web-0.4.0/autoboot_web/middleware/uniform.py
+drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 10:44:10.551638 autoboot-web-0.4.0/autoboot_web/mvc/
+-rw-r--r--   0 yizzuide   (501) staff       (20)       91 2023-11-29 06:50:51.000000 autoboot-web-0.4.0/autoboot_web/mvc/__init__.py
+drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 10:44:10.552542 autoboot-web-0.4.0/autoboot_web/mvc/annotation/
+-rw-r--r--   0 yizzuide   (501) staff       (20)      133 2023-11-29 06:50:51.000000 autoboot-web-0.4.0/autoboot_web/mvc/annotation/__init__.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)     3391 2023-11-29 06:50:51.000000 autoboot-web-0.4.0/autoboot_web/mvc/annotation/controller.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)     3540 2023-11-29 06:50:51.000000 autoboot-web-0.4.0/autoboot_web/mvc/apply_router.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)     2797 2023-11-30 09:33:54.000000 autoboot-web-0.4.0/autoboot_web/runner.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1658 2023-11-29 07:17:27.000000 autoboot-web-0.4.0/autoboot_web/web_properties.py
+drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 10:44:10.550336 autoboot-web-0.4.0/autoboot_web.egg-info/
+-rw-r--r--   0 yizzuide   (501) staff       (20)      659 2023-11-30 10:44:10.000000 autoboot-web-0.4.0/autoboot_web.egg-info/PKG-INFO
+-rw-r--r--   0 yizzuide   (501) staff       (20)      572 2023-11-30 10:44:10.000000 autoboot-web-0.4.0/autoboot_web.egg-info/SOURCES.txt
+-rw-r--r--   0 yizzuide   (501) staff       (20)        1 2023-11-30 10:44:10.000000 autoboot-web-0.4.0/autoboot_web.egg-info/dependency_links.txt
+-rw-r--r--   0 yizzuide   (501) staff       (20)       48 2023-11-30 10:44:10.000000 autoboot-web-0.4.0/autoboot_web.egg-info/requires.txt
+-rw-r--r--   0 yizzuide   (501) staff       (20)       13 2023-11-30 10:44:10.000000 autoboot-web-0.4.0/autoboot_web.egg-info/top_level.txt
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1313 2023-11-29 06:50:51.000000 autoboot-web-0.4.0/pyproject.toml
+-rw-r--r--   0 yizzuide   (501) staff       (20)      106 2023-11-30 10:44:10.553628 autoboot-web-0.4.0/setup.cfg
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1153 2023-11-30 10:14:00.000000 autoboot-web-0.4.0/setup.py
```

### Comparing `autoboot-web-0.3.0/LICENSE.txt` & `autoboot-web-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `autoboot-web-0.3.0/PKG-INFO` & `autoboot-web-0.4.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoboot-web
-Version: 0.3.0
+Version: 0.4.0
 Summary: Web starter build with autoboot and FastAPI
 Home-page: https://github.com/yizzuide/autoboot_data
 Author: yizzuide
 Author-email: fu837014586@163.com
 Keywords: autoboot,web,FastAPI
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
```

### Comparing `autoboot-web-0.3.0/autoboot_web/http_properties.py` & `autoboot-web-0.4.0/autoboot_web/http_properties.py`

 * *Files identical despite different names*

### Comparing `autoboot-web-0.3.0/autoboot_web/mvc/annotation/controller.py` & `autoboot-web-0.4.0/autoboot_web/mvc/annotation/controller.py`

 * *Files identical despite different names*

### Comparing `autoboot-web-0.3.0/autoboot_web/mvc/apply_router.py` & `autoboot-web-0.4.0/autoboot_web/mvc/apply_router.py`

 * *Files identical despite different names*

### Comparing `autoboot-web-0.3.0/autoboot_web/runner.py` & `autoboot-web-0.4.0/autoboot_web/runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,43 @@
 from typing import Optional
 from importlib import import_module
 from autoboot import AutoBoot
-from autoboot.plugin import AppPlugin, Runner
+from autoboot.plugin import AppPlugin
 from fastapi import FastAPI
 from fastapi.middleware.gzip import GZipMiddleware
 from starlette.middleware.sessions import SessionMiddleware
 from .http_properties import HttpProperties
 from .web_properties import WebProperties
 
-class WebRunner(AppPlugin):
+class WebRunner(AppPlugin[FastAPI]):
   
-  __ctx__ = "FastAPI"
+  # custom context name, default is class name
+  #context_name = "WebRunner"
   
   def __init__(self, scan_controllers: Optional[str | list[str]] = None) -> None:
     self._scan_controllers = scan_controllers
   
-  @staticmethod
-  def get_context() -> FastAPI:
-    return AutoBoot.get_context(WebRunner.__ctx__)
-  
-  def install(self) -> Runner:
-    app = FastAPI()
-    return (WebRunner.__ctx__, app)
+  def install(self) -> FastAPI:
+    return FastAPI()
   
   def env_prepared(self) -> None:
-    packages: list[str] = []
+    self.packages: list[str] = []
     if self._scan_controllers:
-      packages.extend([self._scan_controllers] if isinstance(self._scan_controllers, str) else self._scan_controllers)
+      self.packages.extend([self._scan_controllers] if isinstance(self._scan_controllers, str) else self._scan_controllers)
     
     if WebProperties.scan_controller_packages():
-      packages.extend(WebProperties.scan_controller_packages()) 
-    
-    for package in packages:
-      #__import__(packages)
+      self.packages.extend(WebProperties.scan_controller_packages()) 
+      
+  
+  def app_started(self) -> None:
+    for package in self.packages:
       import_module(package)
-    
+      
     app = self.get_context()
-    
+
     if HttpProperties.gzip_enable():
       AutoBoot.logger.info("GZIP is enabled.")
       app.add_middleware(GZipMiddleware, minimum_size=HttpProperties.gzip_minimum_size())
       
     if HttpProperties.session_enable():
       AutoBoot.logger.info("Session is enabled.")
       app.add_middleware(
@@ -73,14 +70,8 @@
     
       app.add_middleware(
         UniformCSRFMiddleware, 
         secret=WebProperties.csrf_secret(), 
         cookie_name=WebProperties.csrf_cookie_name(),
         cookie_domain=WebProperties.csrf_cookie_domain(),
         header_name=WebProperties.csrf_header_name()
-      )
-    
-    return super().env_prepared()
-  
-  def app_started(self) -> None:
-    return super().app_started()
-  
+      )
```

### Comparing `autoboot-web-0.3.0/autoboot_web/web_properties.py` & `autoboot-web-0.4.0/autoboot_web/web_properties.py`

 * *Files identical despite different names*

### Comparing `autoboot-web-0.3.0/autoboot_web.egg-info/PKG-INFO` & `autoboot-web-0.4.0/autoboot_web.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoboot-web
-Version: 0.3.0
+Version: 0.4.0
 Summary: Web starter build with autoboot and FastAPI
 Home-page: https://github.com/yizzuide/autoboot_data
 Author: yizzuide
 Author-email: fu837014586@163.com
 Keywords: autoboot,web,FastAPI
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
```

### Comparing `autoboot-web-0.3.0/autoboot_web.egg-info/SOURCES.txt` & `autoboot-web-0.4.0/autoboot_web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autoboot-web-0.3.0/pyproject.toml` & `autoboot-web-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autoboot-web-0.3.0/setup.py` & `autoboot-web-0.4.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = '0.3.0'
+VERSION = '0.4.0'
 
 with open('README.md', 'r', encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(
     name='autoboot-web',
     version=VERSION,
@@ -14,15 +14,15 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/yizzuide/autoboot_data',
     keywords=['autoboot', 'web', 'FastAPI'],
     packages=find_packages(exclude=['tests*']),
     include_package_data=True,
     install_requires=[
-        'autoboot>=0.6.0',
+        'autoboot>=0.7.0',
         'fastapi>=0.70.1',
         'uvicorn>=0.16.0'
     ],
     extra_require={
         'all': ['starlette-csrf>=1.4.0']
     },
     tests_require=[
```

