# Comparing `tmp/chiasmodon-2.0.2.tar.gz` & `tmp/chiasmodon-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chiasmodon-2.0.2.tar", last modified: Mon May  6 23:51:19 2024, max compression
+gzip compressed data, was "chiasmodon-2.0.3.tar", last modified: Fri May 10 10:42:45 2024, max compression
```

## Comparing `chiasmodon-2.0.2.tar` & `chiasmodon-2.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-05-06 23:51:19.982908 chiasmodon-2.0.2/
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1053 2024-04-16 18:26:16.000000 chiasmodon-2.0.2/LICENSE.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)    12235 2024-05-06 23:51:19.982908 chiasmodon-2.0.2/PKG-INFO
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)    11584 2024-04-30 19:12:19.000000 chiasmodon-2.0.2/README.md
-drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-05-06 23:51:19.982908 chiasmodon-2.0.2/chiasmodon.egg-info/
--rw-r--r--   0 mhm       (1000) mhm       (1000)    12235 2024-05-06 23:51:19.000000 chiasmodon-2.0.2/chiasmodon.egg-info/PKG-INFO
--rw-r--r--   0 mhm       (1000) mhm       (1000)      237 2024-05-06 23:51:19.000000 chiasmodon-2.0.2/chiasmodon.egg-info/SOURCES.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-05-06 23:51:19.000000 chiasmodon-2.0.2/chiasmodon.egg-info/dependency_links.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)       39 2024-05-06 23:51:19.000000 chiasmodon-2.0.2/chiasmodon.egg-info/requires.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-05-06 23:51:19.000000 chiasmodon-2.0.2/chiasmodon.egg-info/top_level.txt
-drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-05-06 23:51:19.982908 chiasmodon-2.0.2/cli/
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)    21908 2024-05-06 23:50:44.000000 chiasmodon-2.0.2/cli/chiasmodon_cli.py
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)    27918 2024-05-06 23:50:24.000000 chiasmodon-2.0.2/pychiasmodon.py
--rw-r--r--   0 mhm       (1000) mhm       (1000)       38 2024-05-06 23:51:19.982908 chiasmodon-2.0.2/setup.cfg
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1262 2024-05-06 23:50:36.000000 chiasmodon-2.0.2/setup.py
+drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-05-10 10:42:45.491759 chiasmodon-2.0.3/
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1053 2024-04-16 18:26:16.000000 chiasmodon-2.0.3/LICENSE.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)    12235 2024-05-10 10:42:45.491759 chiasmodon-2.0.3/PKG-INFO
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)    11584 2024-04-30 19:12:19.000000 chiasmodon-2.0.3/README.md
+drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-05-10 10:42:45.491759 chiasmodon-2.0.3/chiasmodon.egg-info/
+-rw-r--r--   0 mhm       (1000) mhm       (1000)    12235 2024-05-10 10:42:45.000000 chiasmodon-2.0.3/chiasmodon.egg-info/PKG-INFO
+-rw-r--r--   0 mhm       (1000) mhm       (1000)      237 2024-05-10 10:42:45.000000 chiasmodon-2.0.3/chiasmodon.egg-info/SOURCES.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-05-10 10:42:45.000000 chiasmodon-2.0.3/chiasmodon.egg-info/dependency_links.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)       39 2024-05-10 10:42:45.000000 chiasmodon-2.0.3/chiasmodon.egg-info/requires.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-05-10 10:42:45.000000 chiasmodon-2.0.3/chiasmodon.egg-info/top_level.txt
+drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-05-10 10:42:45.491759 chiasmodon-2.0.3/cli/
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)    21908 2024-05-10 10:42:35.000000 chiasmodon-2.0.3/cli/chiasmodon_cli.py
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)    29376 2024-05-10 10:42:25.000000 chiasmodon-2.0.3/pychiasmodon.py
+-rw-r--r--   0 mhm       (1000) mhm       (1000)       38 2024-05-10 10:42:45.491759 chiasmodon-2.0.3/setup.cfg
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1262 2024-05-10 10:42:28.000000 chiasmodon-2.0.3/setup.py
```

### Comparing `chiasmodon-2.0.2/LICENSE.txt` & `chiasmodon-2.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chiasmodon-2.0.2/PKG-INFO` & `chiasmodon-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chiasmodon
-Version: 2.0.2
+Version: 2.0.3
 Summary: Chiasmodon is an OSINT tool that allows users to gather information from various sources and conduct targeted searches based on domains, Google Play applications, email addresses, IP addresses, organizations, URLs, and more. It provides comprehensive scanning capabilities, customizable output formats, and additional options for enhanced data analysis and customization.
 Home-page: https://github.com/chiasmod0n/chiasmodon
 Author: chiasmod0n
 License: UNKNOWN
 Keywords: intelligence osint credentials emails asn cidr bugbounty subdomains information-gathering intelligence-analysis reconnaissance attack-surface subdomain-enumeration reconnaissance-framework bugbounty-tool email-enumeration chiasmodon
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `chiasmodon-2.0.2/README.md` & `chiasmodon-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `chiasmodon-2.0.2/chiasmodon.egg-info/PKG-INFO` & `chiasmodon-2.0.3/chiasmodon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chiasmodon
-Version: 2.0.2
+Version: 2.0.3
 Summary: Chiasmodon is an OSINT tool that allows users to gather information from various sources and conduct targeted searches based on domains, Google Play applications, email addresses, IP addresses, organizations, URLs, and more. It provides comprehensive scanning capabilities, customizable output formats, and additional options for enhanced data analysis and customization.
 Home-page: https://github.com/chiasmod0n/chiasmodon
 Author: chiasmod0n
 License: UNKNOWN
 Keywords: intelligence osint credentials emails asn cidr bugbounty subdomains information-gathering intelligence-analysis reconnaissance attack-surface subdomain-enumeration reconnaissance-framework bugbounty-tool email-enumeration chiasmodon
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `chiasmodon-2.0.2/cli/chiasmodon_cli.py` & `chiasmodon-2.0.3/cli/chiasmodon_cli.py`

 * *Files identical despite different names*

### Comparing `chiasmodon-2.0.2/pychiasmodon.py` & `chiasmodon-2.0.3/pychiasmodon.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
+import re
 import os 
 import sys
 import time
 import requests
-import tldextract
 from yaspin import Spinner 
 
-VERSION = "2.0.2"
+VERSION = "2.0.3"
 _API_URL = 'https://chiasmodon.com/v2/api/beta'
 _API_HEADERS = {'user-agent':'cli/python'}
 _VIEW_TYPE = {
     'full':[
         'cred.username',
         'cred.phone',
         'cred.password',
@@ -277,19 +277,45 @@
             else:
                 try:os.remove(conf_file)
                 except:pass
 
                 self.print(f'{T.RED}{self.msg}{T.RESET}')
                 return
     
-    def filter_domain(self,d) -> str:
-        domain = d.split()[0]
-        x = tldextract.extract(domain)
-        if x.subdomain:return '{}.{}.{}'.format(x.subdomain,x.domain, x.suffix)
-        else:return '{}.{}'.format(x.domain, x.suffix)
+    def filter(self,query:str,method:str):
+
+        if 'domain' in method:
+            self.print(f'{T.RED}Your format query is wrong!\nThis is not domain.{T.RESET}')
+            return query if re.match(r"^(?!.*\d+\.\d+\.\d+\.\d+$)[a-zA-Z0-9-]+\.[a-zA-Z0-9-.]+$", query) else False 
+
+        elif method == 'ip':
+            self.print(f'{T.RED}Your format query is wrong!\nAccept only ipv4.{T.RESET}')
+            return query if re.match(r"\b(?:\d{1,3}\.){3}\d{1,3}\b", query) else False 
+        
+        elif method == 'ip.asn':
+            self.print(f'{T.RED}Your format query is wrong!\nThe ASN starts with AS\nLike this: AS1234.{T.RESET}')
+            return query if query.lower().startswith('as') else False
+        
+        elif method in ['ip.port', 'url.port']:
+            self.print(f'{T.RED}Your format query is wrong!\nThis is not port.{T.RESET}')
+            return query if re.match(r":(\d+)", query) else False
+        
+        elif method == 'cred.email':
+            self.print(f'{T.RED}Your format query is wrong!\nAccept only country code.{T.RESET}')
+            return query if re.match(r'^[\w\.-]+@[\w\.-]+\.\w+$', query) else False   
+        
+        elif method == 'cred.country' or method == 'ip.country':
+            self.print(f'{T.RED}Your format query is wrong!\nAccept only country code.{T.RESET}')
+            return query if len(query) == 2 else False
+        
+        elif method == 'url.path':
+            self.print(f'{T.RED}Your format query is wrong!\nThe url path moset be like: /somthing{T.RESET}')
+            return query if query[0] == '/' else False
+        
+        return query
 
     def print(self,text, ys=None, ys_err=False) -> None:
         if text == None:return 
         if self.debug:
             if ys:
                 if not ys_err:
                     ys.write(text)
@@ -480,20 +506,23 @@
         
         
         if method not in _METHODS:
             raise Exception(f"{T.RED}not found this method: {method}.{T.RESET}")
         
         if method not in _VIEW_TYPE[view_type]:
             raise Exception(f"{T.RED}{view_type} doesn't support ({method}).{T.RESET}")
-
+        
+        
         self.err = False
         self.msg = ''
 
-        if method == 'domain':query = self.filter_domain(query)
-
+        query = self.filter(query, method)
+        if query == False:
+            return
+        
         result = self.__proc_query(
             query=query,
             method=method,
             view_type=view_type,
             sort=sort,
             timeout=timeout,
             limit=limit,
```

### Comparing `chiasmodon-2.0.2/setup.py` & `chiasmodon-2.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from distutils.core import setup
 from os import path
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='chiasmodon',
-      version='2.0.2',
+      version='2.0.3',
       description='Chiasmodon is an OSINT tool that allows users to gather information from various sources and conduct targeted searches based on domains, Google Play applications, email addresses, IP addresses, organizations, URLs, and more. It provides comprehensive scanning capabilities, customizable output formats, and additional options for enhanced data analysis and customization.',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='chiasmod0n',
       keywords='intelligence osint credentials emails asn cidr bugbounty subdomains information-gathering intelligence-analysis reconnaissance attack-surface subdomain-enumeration reconnaissance-framework bugbounty-tool email-enumeration chiasmodon',
       url='https://github.com/chiasmod0n/chiasmodon',
       packages=['.'],
```

