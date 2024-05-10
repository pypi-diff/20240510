# Comparing `tmp/mangorest-0.13100000000000003.tar.gz` & `tmp/mangorest-0.13200000000000003.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mangorest-0.13100000000000003.tar", last modified: Sun Mar 24 20:35:01 2024, max compression
+gzip compressed data, was "mangorest-0.13200000000000003.tar", last modified: Fri May 10 18:49:31 2024, max compression
```

## Comparing `mangorest-0.13100000000000003.tar` & `mangorest-0.13200000000000003.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2024-03-24 20:35:01.069268 mangorest-0.13100000000000003/
--rw-r--r--   0 snarayan   (501) wheel        (0)    11357 2020-09-20 16:46:27.000000 mangorest-0.13100000000000003/LICENSE
--rw-r--r--   0 snarayan   (501) wheel        (0)      820 2024-03-24 20:35:01.068878 mangorest-0.13100000000000003/PKG-INFO
--rw-r--r--   0 snarayan   (501) wheel        (0)     2449 2022-07-26 01:13:10.000000 mangorest-0.13100000000000003/README.md
-drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2024-03-24 20:35:01.066321 mangorest-0.13100000000000003/mangorest/
--rw-r--r--   0 snarayan   (501) wheel        (0)        0 2020-09-20 16:51:18.000000 mangorest-0.13100000000000003/mangorest/__init__.py
--rw-r--r--   0 snarayan   (501) wheel        (0)     1310 2020-09-26 18:35:34.000000 mangorest-0.13100000000000003/mangorest/dirlist.py
--rwxr-xr-x   0 snarayan   (501) wheel        (0)    14676 2023-09-04 10:51:45.000000 mangorest-0.13100000000000003/mangorest/mango.py
--rw-r--r--   0 snarayan   (501) wheel        (0)       27 2024-03-24 20:35:00.000000 mangorest-0.13100000000000003/mangorest/version.txt
-drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2024-03-24 20:35:01.068555 mangorest-0.13100000000000003/mangorest.egg-info/
--rw-r--r--   0 snarayan   (501) wheel        (0)      820 2024-03-24 20:35:01.000000 mangorest-0.13100000000000003/mangorest.egg-info/PKG-INFO
--rw-r--r--   0 snarayan   (501) wheel        (0)      319 2024-03-24 20:35:01.000000 mangorest-0.13100000000000003/mangorest.egg-info/SOURCES.txt
--rw-r--r--   0 snarayan   (501) wheel        (0)        1 2024-03-24 20:35:01.000000 mangorest-0.13100000000000003/mangorest.egg-info/dependency_links.txt
--rw-r--r--   0 snarayan   (501) wheel        (0)        1 2020-09-26 14:25:00.000000 mangorest-0.13100000000000003/mangorest.egg-info/not-zip-safe
--rw-r--r--   0 snarayan   (501) wheel        (0)        7 2024-03-24 20:35:01.000000 mangorest-0.13100000000000003/mangorest.egg-info/requires.txt
--rw-r--r--   0 snarayan   (501) wheel        (0)       10 2024-03-24 20:35:01.000000 mangorest-0.13100000000000003/mangorest.egg-info/top_level.txt
--rw-r--r--   0 snarayan   (501) wheel        (0)       38 2024-03-24 20:35:01.069346 mangorest-0.13100000000000003/setup.cfg
--rw-r--r--   0 snarayan   (501) wheel        (0)     1698 2024-03-24 20:35:00.000000 mangorest-0.13100000000000003/setup.py
-drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2024-03-24 20:35:01.068261 mangorest-0.13100000000000003/test/
--rwxrwxr-x   0 snarayan   (501) wheel        (0)      653 2022-07-20 11:34:26.000000 mangorest-0.13100000000000003/test/test.py
+drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2024-05-10 18:49:31.037272 mangorest-0.13200000000000003/
+-rw-r--r--   0 snarayan   (501) wheel        (0)    11357 2020-09-20 16:46:27.000000 mangorest-0.13200000000000003/LICENSE
+-rw-r--r--   0 snarayan   (501) wheel        (0)      820 2024-05-10 18:49:31.036862 mangorest-0.13200000000000003/PKG-INFO
+-rw-r--r--   0 snarayan   (501) wheel        (0)     2449 2022-07-26 01:13:10.000000 mangorest-0.13200000000000003/README.md
+drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2024-05-10 18:49:31.033138 mangorest-0.13200000000000003/mangorest/
+-rw-r--r--   0 snarayan   (501) wheel        (0)        0 2020-09-20 16:51:18.000000 mangorest-0.13200000000000003/mangorest/__init__.py
+-rw-r--r--   0 snarayan   (501) wheel        (0)     1310 2020-09-26 18:35:34.000000 mangorest-0.13200000000000003/mangorest/dirlist.py
+-rwxr-xr-x   0 snarayan   (501) wheel        (0)    14814 2024-05-10 18:48:38.000000 mangorest-0.13200000000000003/mangorest/mango.py
+-rw-r--r--   0 snarayan   (501) wheel        (0)       27 2024-05-10 18:49:30.000000 mangorest-0.13200000000000003/mangorest/version.txt
+drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2024-05-10 18:49:31.036316 mangorest-0.13200000000000003/mangorest.egg-info/
+-rw-r--r--   0 snarayan   (501) wheel        (0)      820 2024-05-10 18:49:30.000000 mangorest-0.13200000000000003/mangorest.egg-info/PKG-INFO
+-rw-r--r--   0 snarayan   (501) wheel        (0)      319 2024-05-10 18:49:30.000000 mangorest-0.13200000000000003/mangorest.egg-info/SOURCES.txt
+-rw-r--r--   0 snarayan   (501) wheel        (0)        1 2024-05-10 18:49:30.000000 mangorest-0.13200000000000003/mangorest.egg-info/dependency_links.txt
+-rw-r--r--   0 snarayan   (501) wheel        (0)        1 2020-09-26 14:25:00.000000 mangorest-0.13200000000000003/mangorest.egg-info/not-zip-safe
+-rw-r--r--   0 snarayan   (501) wheel        (0)        7 2024-05-10 18:49:30.000000 mangorest-0.13200000000000003/mangorest.egg-info/requires.txt
+-rw-r--r--   0 snarayan   (501) wheel        (0)       10 2024-05-10 18:49:30.000000 mangorest-0.13200000000000003/mangorest.egg-info/top_level.txt
+-rw-r--r--   0 snarayan   (501) wheel        (0)       38 2024-05-10 18:49:31.037369 mangorest-0.13200000000000003/setup.cfg
+-rw-r--r--   0 snarayan   (501) wheel        (0)     1698 2024-05-10 18:49:30.000000 mangorest-0.13200000000000003/setup.py
+drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2024-05-10 18:49:31.035379 mangorest-0.13200000000000003/test/
+-rwxrwxr-x   0 snarayan   (501) wheel        (0)      653 2022-07-20 11:34:26.000000 mangorest-0.13200000000000003/test/test.py
```

### Comparing `mangorest-0.13100000000000003/LICENSE` & `mangorest-0.13200000000000003/LICENSE`

 * *Files identical despite different names*

### Comparing `mangorest-0.13100000000000003/PKG-INFO` & `mangorest-0.13200000000000003/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mangorest
-Version: 0.13100000000000003
+Version: 0.13200000000000003
 Summary: Very simple quick way to deploy Django Webservices
 Home-page: https://github.com/meyers007/mangorest.git
 Author: Wan Bae, Seattle University
 Author-email: baew@seattleu.edu
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `mangorest-0.13100000000000003/README.md` & `mangorest-0.13200000000000003/README.md`

 * *Files identical despite different names*

### Comparing `mangorest-0.13100000000000003/mangorest/dirlist.py` & `mangorest-0.13200000000000003/mangorest/dirlist.py`

 * *Files identical despite different names*

### Comparing `mangorest-0.13100000000000003/mangorest/mango.py` & `mangorest-0.13200000000000003/mangorest/mango.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from django.core.management import execute_from_command_line
 import numpy as np
 from proxy.views import proxy_view
 import pandas as pd
 
 from django.conf import settings
 from django.contrib.staticfiles import finders
+from django.contrib.staticfiles import views
 from django.http import Http404
 from django.views import static
 
 
 import logging
 logging.basicConfig( level=logging.INFO,
         format='%(asctime)s %(name)s %(levelname)s: %(message)s',
@@ -57,15 +58,15 @@
     pyModule = rpath;
     
     logp(f"{template} Requested")
     getlist = [ c for c in request.GET.items()]
     ret = f''' <pre>\n Response Object: \n{os.getcwd()} path_info:{request.path_info}: final:{rpath}
                Page exists:  {template} : {os.path.exists(template)}
                Page exists:  {pyModule} : {os.path.exists(pyModule)}
-               {getlist} </pre> '''
+           L    {getlist} </pre> '''
     return HttpResponse(ret);
 #--------------------------------------------------------------------------------
 class myEncoder(DjangoJSONEncoder):
     def default(self, obj):
         if isinstance(obj, np.int64):
             return int(obj)
         elif isinstance(obj, pd._libs.tslibs.timestamps.Timestamp):
@@ -128,33 +129,33 @@
     return HttpResponse(ret) #, content_type="text/plain")
 #--------------------------------------------------------------------------------
 def TryRunPyMethod(request):
     rpaths = [c for c in request.path.split("/") if (c) ];
     pyMethod = rpaths[-1];
  
     if ( pyMethod.find("modules.") < 0 ):
-        return HttpResponse(f"{pyMethod} not understood 0")
+        return HttpResponse(f"error: {pyMethod} not understood 0")
         
     spl = pyMethod.split('.');
  
     if ( len(spl) < 2):
         logp("Hmmm ... May be not what is intended!! module name")
-        return HttpResponse(f"{pyMethod} not understood 2");
+        return HttpResponse(f"error: {pyMethod} not understood 2");
     
     modName = ".".join(spl[:-1])
     __import__(modName, fromlist="dummy")
     
     funName = spl[-1]
     for v in sys.modules:
         if (v.startswith(modName)):
             method= getattr(sys.modules[v], funName)
             logp("==>", v, type(v), funName, method, type(method), callable(method))
             return CallMethod(method, request)
         
-    return HttpResponse(f"{pyMethod} not understood3 ");
+    return HttpResponse(f"error: {pyMethod} not understood3 ");
     
 #--------------------------------------------------------------------------------
 '''
 USE following methods to pass in AUTH Key:
     curl -i -H "APK: 123"  http://localhost:9000
 '''
 def AuthorizeAPIKEY(request):
@@ -254,14 +255,15 @@
             ret = open(f, "rb").read()
             break;
     
     return HttpResponse(ret, content_type=mtype) #request.content_type)    
 
 
 def serveStatic(request, path, **kwargs):
+    #return views.serve(request, path, insecure=True, **kwargs)
     file=path[8:]
     #LOG = 0
     #if str(path).find("bootstrap.min.js.map") > 1:
     #    LOG=1
     #if LOG: logger.info(f"================>serveStatic: {file} {request.content_type}")
 
     normalized_path = os.path.normpath(file).lstrip("/")
@@ -342,15 +344,15 @@
         return CommonSecured(request, rpath)
     elif ( os.path.exists(template) and rpath.strip()):
         return render(request, rpath)
     elif rpaths[-1].find("modules.") >= 0: #Must be a python module call
         logger.debug("**** Getting python Module")
         return TryRunPyMethod(request)
     
-    return HttpResponse(f"{path} not understood");
+    return HttpResponse(f"error: {path} not understood");
     
 #--------------------------------------------------------------------------------
 _WEBAPI_ROUTES={}
 def webapi(url, auth=None, **kwargs):
     if auth and not inspect.isfunction(auth):
         auth = AuthorizeAPIKEY
```

### Comparing `mangorest-0.13100000000000003/mangorest.egg-info/PKG-INFO` & `mangorest-0.13200000000000003/mangorest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mangorest
-Version: 0.13100000000000003
+Version: 0.13200000000000003
 Summary: Very simple quick way to deploy Django Webservices
 Home-page: https://github.com/meyers007/mangorest.git
 Author: Wan Bae, Seattle University
 Author-email: baew@seattleu.edu
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `mangorest-0.13100000000000003/setup.py` & `mangorest-0.13200000000000003/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version=0.13100000000000003
+version=0.13200000000000003
 
 setup(name='mangorest', 
       version=str(version), 
       description='Very simple quick way to deploy Django Webservices',
       url='https://github.com/meyers007/mangorest.git',
       author='Wan Bae, Seattle University',
       author_email='baew@seattleu.edu',
```

### Comparing `mangorest-0.13100000000000003/test/test.py` & `mangorest-0.13200000000000003/test/test.py`

 * *Files identical despite different names*

