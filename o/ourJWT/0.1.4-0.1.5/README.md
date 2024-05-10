# Comparing `tmp/ourJWT-0.1.4.tar.gz` & `tmp/ourJWT-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ourJWT-0.1.4.tar", last modified: Fri May 10 20:47:02 2024, max compression
+gzip compressed data, was "ourJWT-0.1.5.tar", last modified: Fri May 10 21:08:05 2024, max compression
```

## Comparing `ourJWT-0.1.4.tar` & `ourJWT-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 gd-harco  (1000) gd-harco  (1000)        0 2024-05-10 20:47:02.399181 ourJWT-0.1.4/
--rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      258 2024-05-10 20:47:02.399181 ourJWT-0.1.4/PKG-INFO
-drwxr-xr-x   0 gd-harco  (1000) gd-harco  (1000)        0 2024-05-10 20:47:02.399181 ourJWT-0.1.4/ourJWT/
--rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)     3404 2024-05-10 20:10:21.000000 ourJWT-0.1.4/ourJWT/OUR_class.py
--rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      374 2024-04-12 19:02:23.000000 ourJWT-0.1.4/ourJWT/OUR_exception.py
--rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      153 2024-04-12 21:30:49.000000 ourJWT-0.1.4/ourJWT/__init__.py
--rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      873 2024-05-10 20:40:34.000000 ourJWT-0.1.4/ourJWT/decorators.py
-drwxr-xr-x   0 gd-harco  (1000) gd-harco  (1000)        0 2024-05-10 20:47:02.399181 ourJWT-0.1.4/ourJWT.egg-info/
--rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      258 2024-05-10 20:47:02.000000 ourJWT-0.1.4/ourJWT.egg-info/PKG-INFO
--rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      241 2024-05-10 20:47:02.000000 ourJWT-0.1.4/ourJWT.egg-info/SOURCES.txt
--rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)        1 2024-05-10 20:47:02.000000 ourJWT-0.1.4/ourJWT.egg-info/dependency_links.txt
--rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      134 2024-05-10 20:47:02.000000 ourJWT-0.1.4/ourJWT.egg-info/requires.txt
--rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)        7 2024-05-10 20:47:02.000000 ourJWT-0.1.4/ourJWT.egg-info/top_level.txt
--rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)       38 2024-05-10 20:47:02.399181 ourJWT-0.1.4/setup.cfg
--rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      599 2024-05-10 20:46:59.000000 ourJWT-0.1.4/setup.py
+drwxr-xr-x   0 gd-harco  (1000) gd-harco  (1000)        0 2024-05-10 21:08:05.373160 ourJWT-0.1.5/
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      258 2024-05-10 21:08:05.363160 ourJWT-0.1.5/PKG-INFO
+drwxr-xr-x   0 gd-harco  (1000) gd-harco  (1000)        0 2024-05-10 21:08:05.363160 ourJWT-0.1.5/ourJWT/
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)     3438 2024-05-10 21:07:20.000000 ourJWT-0.1.5/ourJWT/OUR_class.py
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      374 2024-04-12 19:02:23.000000 ourJWT-0.1.5/ourJWT/OUR_exception.py
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      153 2024-04-12 21:30:49.000000 ourJWT-0.1.5/ourJWT/__init__.py
+drwxr-xr-x   0 gd-harco  (1000) gd-harco  (1000)        0 2024-05-10 21:08:05.363160 ourJWT-0.1.5/ourJWT.egg-info/
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      258 2024-05-10 21:08:05.000000 ourJWT-0.1.5/ourJWT.egg-info/PKG-INFO
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      220 2024-05-10 21:08:05.000000 ourJWT-0.1.5/ourJWT.egg-info/SOURCES.txt
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)        1 2024-05-10 21:08:05.000000 ourJWT-0.1.5/ourJWT.egg-info/dependency_links.txt
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      134 2024-05-10 21:08:05.000000 ourJWT-0.1.5/ourJWT.egg-info/requires.txt
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)        7 2024-05-10 21:08:05.000000 ourJWT-0.1.5/ourJWT.egg-info/top_level.txt
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)       38 2024-05-10 21:08:05.373160 ourJWT-0.1.5/setup.cfg
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      599 2024-05-10 21:07:39.000000 ourJWT-0.1.5/setup.py
```

### Comparing `ourJWT-0.1.4/ourJWT/OUR_class.py` & `ourJWT-0.1.5/ourJWT/OUR_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,25 +47,25 @@
             raise OUR_exception.ExpiredToken()
         if token["sub"] != "auth" and token["sub"] != "refresh":
             raise OUR_exception.BadSubject
         return token
 
     def check_auth():
         def decorator(function):
-            def wrapper(request: HttpRequest):
+            def wrapper(request: HttpRequest, *args, **kwargs):
                 auth: str = request.COOKIES.get("auth_token", None)
                 if auth is None:
                     return response.HttpResponseBadRequest(reason="No auth cookie sent")
                 try:
                     auth_decoded = Decoder.decode(auth)
                 except (OUR_exception.BadSubject,
                         OUR_exception.RefusedToken,
                         OUR_exception.ExpiredToken):
                     return HttpResponseUnauthorized(reason="Bad auth token")
-                return function(request, token=auth_decoded)
+                return function(request, *args, token=auth_decoded, **kwargs)
             return wrapper
         return decorator
 
 
 
 
 class Encoder:
```

### Comparing `ourJWT-0.1.4/setup.py` & `ourJWT-0.1.5/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     include_package_data=True,
     name='ourJWT',
-    version='0.1.4',
+    version='0.1.5',
     description='repackaging of pyJWT package, adding fonction required for our_transcendence',
     author="gd-harco",
     author_email="gd-harco@student.42lyon.fr",
     py_modules=['ourJWT'],
     packages=find_packages(),
     install_requires=[
         'asgiref==3.8.1',
```

