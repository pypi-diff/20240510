# Comparing `tmp/ourJWT-0.1.3.tar.gz` & `tmp/ourJWT-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ourJWT-0.1.3.tar", last modified: Tue Apr 30 12:59:49 2024, max compression
+gzip compressed data, was "ourJWT-0.1.4.tar", last modified: Fri May 10 20:47:02 2024, max compression
```

## Comparing `ourJWT-0.1.3.tar` & `ourJWT-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 gd-harco (102195) 2022_lyon  (4222)        0 2024-04-30 12:59:49.093378 ourJWT-0.1.3/
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      258 2024-04-30 12:59:49.093378 ourJWT-0.1.3/PKG-INFO
-drwxr-xr-x   0 gd-harco (102195) 2022_lyon  (4222)        0 2024-04-30 12:59:49.093378 ourJWT-0.1.3/ourJWT/
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)     3404 2024-04-16 13:56:23.000000 ourJWT-0.1.3/ourJWT/OUR_class.py
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      374 2024-04-16 08:08:01.000000 ourJWT-0.1.3/ourJWT/OUR_exception.py
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      153 2024-04-16 08:08:01.000000 ourJWT-0.1.3/ourJWT/__init__.py
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      859 2024-04-18 13:07:16.000000 ourJWT-0.1.3/ourJWT/decorators.py
-drwxr-xr-x   0 gd-harco (102195) 2022_lyon  (4222)        0 2024-04-30 12:59:49.093378 ourJWT-0.1.3/ourJWT.egg-info/
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      258 2024-04-30 12:59:49.000000 ourJWT-0.1.3/ourJWT.egg-info/PKG-INFO
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      241 2024-04-30 12:59:49.000000 ourJWT-0.1.3/ourJWT.egg-info/SOURCES.txt
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)        1 2024-04-30 12:59:49.000000 ourJWT-0.1.3/ourJWT.egg-info/dependency_links.txt
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      134 2024-04-30 12:59:49.000000 ourJWT-0.1.3/ourJWT.egg-info/requires.txt
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)        7 2024-04-30 12:59:49.000000 ourJWT-0.1.3/ourJWT.egg-info/top_level.txt
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)       38 2024-04-30 12:59:49.093378 ourJWT-0.1.3/setup.cfg
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      599 2024-04-30 12:59:42.000000 ourJWT-0.1.3/setup.py
+drwxr-xr-x   0 gd-harco  (1000) gd-harco  (1000)        0 2024-05-10 20:47:02.399181 ourJWT-0.1.4/
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      258 2024-05-10 20:47:02.399181 ourJWT-0.1.4/PKG-INFO
+drwxr-xr-x   0 gd-harco  (1000) gd-harco  (1000)        0 2024-05-10 20:47:02.399181 ourJWT-0.1.4/ourJWT/
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)     3404 2024-05-10 20:10:21.000000 ourJWT-0.1.4/ourJWT/OUR_class.py
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      374 2024-04-12 19:02:23.000000 ourJWT-0.1.4/ourJWT/OUR_exception.py
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      153 2024-04-12 21:30:49.000000 ourJWT-0.1.4/ourJWT/__init__.py
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      873 2024-05-10 20:40:34.000000 ourJWT-0.1.4/ourJWT/decorators.py
+drwxr-xr-x   0 gd-harco  (1000) gd-harco  (1000)        0 2024-05-10 20:47:02.399181 ourJWT-0.1.4/ourJWT.egg-info/
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      258 2024-05-10 20:47:02.000000 ourJWT-0.1.4/ourJWT.egg-info/PKG-INFO
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      241 2024-05-10 20:47:02.000000 ourJWT-0.1.4/ourJWT.egg-info/SOURCES.txt
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)        1 2024-05-10 20:47:02.000000 ourJWT-0.1.4/ourJWT.egg-info/dependency_links.txt
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      134 2024-05-10 20:47:02.000000 ourJWT-0.1.4/ourJWT.egg-info/requires.txt
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)        7 2024-05-10 20:47:02.000000 ourJWT-0.1.4/ourJWT.egg-info/top_level.txt
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)       38 2024-05-10 20:47:02.399181 ourJWT-0.1.4/setup.cfg
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      599 2024-05-10 20:46:59.000000 ourJWT-0.1.4/setup.py
```

### Comparing `ourJWT-0.1.3/ourJWT/OUR_class.py` & `ourJWT-0.1.4/ourJWT/OUR_class.py`

 * *Files identical despite different names*

### Comparing `ourJWT-0.1.3/ourJWT/decorators.py` & `ourJWT-0.1.4/ourJWT/decorators.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 
 class HttpResponseUnauthorized(response.HttpResponse):
     status_code = 401
 
 
 def auth_required(decoder: OUR_class.Decoder):
     def decorator(function):
-        def wrapper(request: HttpRequest):
+        def wrapper(request: HttpRequest, *args):
             auth: str = request.COOKIES.get("auth_token", None)
             if auth is None:
                 return response.HttpResponseBadRequest(reason="No auth cookie sent")
             try:
                 auth_decoded = decoder.decode(auth)
             except (OUR_exception.BadSubject,
                     OUR_exception.RefusedToken,
                     OUR_exception.ExpiredToken):
                 return response.HttpResponse(status=469, reason="Bad auth token")
-            return function(request, token=auth_decoded)
+            return function(request, *args, token=auth_decoded)
         return wrapper
     return decorator
```

