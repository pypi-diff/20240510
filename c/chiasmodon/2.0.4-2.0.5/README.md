# Comparing `tmp/chiasmodon-2.0.4.tar.gz` & `tmp/chiasmodon-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chiasmodon-2.0.4.tar", last modified: Fri May 10 10:46:23 2024, max compression
+gzip compressed data, was "chiasmodon-2.0.5.tar", last modified: Fri May 10 10:48:48 2024, max compression
```

## Comparing `chiasmodon-2.0.4.tar` & `chiasmodon-2.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-05-10 10:46:23.251737 chiasmodon-2.0.4/
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1053 2024-04-16 18:26:16.000000 chiasmodon-2.0.4/LICENSE.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)    12235 2024-05-10 10:46:23.251737 chiasmodon-2.0.4/PKG-INFO
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)    11584 2024-04-30 19:12:19.000000 chiasmodon-2.0.4/README.md
-drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-05-10 10:46:23.251737 chiasmodon-2.0.4/chiasmodon.egg-info/
--rw-r--r--   0 mhm       (1000) mhm       (1000)    12235 2024-05-10 10:46:23.000000 chiasmodon-2.0.4/chiasmodon.egg-info/PKG-INFO
--rw-r--r--   0 mhm       (1000) mhm       (1000)      237 2024-05-10 10:46:23.000000 chiasmodon-2.0.4/chiasmodon.egg-info/SOURCES.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-05-10 10:46:23.000000 chiasmodon-2.0.4/chiasmodon.egg-info/dependency_links.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)       39 2024-05-10 10:46:23.000000 chiasmodon-2.0.4/chiasmodon.egg-info/requires.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-05-10 10:46:23.000000 chiasmodon-2.0.4/chiasmodon.egg-info/top_level.txt
-drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-05-10 10:46:23.251737 chiasmodon-2.0.4/cli/
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)    21908 2024-05-10 10:42:35.000000 chiasmodon-2.0.4/cli/chiasmodon_cli.py
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)    29319 2024-05-10 10:46:13.000000 chiasmodon-2.0.4/pychiasmodon.py
--rw-r--r--   0 mhm       (1000) mhm       (1000)       38 2024-05-10 10:46:23.251737 chiasmodon-2.0.4/setup.cfg
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1262 2024-05-10 10:46:15.000000 chiasmodon-2.0.4/setup.py
+drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-05-10 10:48:48.301711 chiasmodon-2.0.5/
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1053 2024-04-16 18:26:16.000000 chiasmodon-2.0.5/LICENSE.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)    12235 2024-05-10 10:48:48.301711 chiasmodon-2.0.5/PKG-INFO
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)    11584 2024-04-30 19:12:19.000000 chiasmodon-2.0.5/README.md
+drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-05-10 10:48:48.301711 chiasmodon-2.0.5/chiasmodon.egg-info/
+-rw-r--r--   0 mhm       (1000) mhm       (1000)    12235 2024-05-10 10:48:48.000000 chiasmodon-2.0.5/chiasmodon.egg-info/PKG-INFO
+-rw-r--r--   0 mhm       (1000) mhm       (1000)      237 2024-05-10 10:48:48.000000 chiasmodon-2.0.5/chiasmodon.egg-info/SOURCES.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-05-10 10:48:48.000000 chiasmodon-2.0.5/chiasmodon.egg-info/dependency_links.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)       39 2024-05-10 10:48:48.000000 chiasmodon-2.0.5/chiasmodon.egg-info/requires.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-05-10 10:48:48.000000 chiasmodon-2.0.5/chiasmodon.egg-info/top_level.txt
+drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-05-10 10:48:48.301711 chiasmodon-2.0.5/cli/
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)    21908 2024-05-10 10:42:35.000000 chiasmodon-2.0.5/cli/chiasmodon_cli.py
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)    29469 2024-05-10 10:48:28.000000 chiasmodon-2.0.5/pychiasmodon.py
+-rw-r--r--   0 mhm       (1000) mhm       (1000)       38 2024-05-10 10:48:48.301711 chiasmodon-2.0.5/setup.cfg
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1262 2024-05-10 10:48:30.000000 chiasmodon-2.0.5/setup.py
```

### Comparing `chiasmodon-2.0.4/LICENSE.txt` & `chiasmodon-2.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chiasmodon-2.0.4/PKG-INFO` & `chiasmodon-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chiasmodon
-Version: 2.0.4
+Version: 2.0.5
 Summary: Chiasmodon is an OSINT tool that allows users to gather information from various sources and conduct targeted searches based on domains, Google Play applications, email addresses, IP addresses, organizations, URLs, and more. It provides comprehensive scanning capabilities, customizable output formats, and additional options for enhanced data analysis and customization.
 Home-page: https://github.com/chiasmod0n/chiasmodon
 Author: chiasmod0n
 License: UNKNOWN
 Keywords: intelligence osint credentials emails asn cidr bugbounty subdomains information-gathering intelligence-analysis reconnaissance attack-surface subdomain-enumeration reconnaissance-framework bugbounty-tool email-enumeration chiasmodon
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `chiasmodon-2.0.4/README.md` & `chiasmodon-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `chiasmodon-2.0.4/chiasmodon.egg-info/PKG-INFO` & `chiasmodon-2.0.5/chiasmodon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chiasmodon
-Version: 2.0.4
+Version: 2.0.5
 Summary: Chiasmodon is an OSINT tool that allows users to gather information from various sources and conduct targeted searches based on domains, Google Play applications, email addresses, IP addresses, organizations, URLs, and more. It provides comprehensive scanning capabilities, customizable output formats, and additional options for enhanced data analysis and customization.
 Home-page: https://github.com/chiasmod0n/chiasmodon
 Author: chiasmod0n
 License: UNKNOWN
 Keywords: intelligence osint credentials emails asn cidr bugbounty subdomains information-gathering intelligence-analysis reconnaissance attack-surface subdomain-enumeration reconnaissance-framework bugbounty-tool email-enumeration chiasmodon
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `chiasmodon-2.0.4/cli/chiasmodon_cli.py` & `chiasmodon-2.0.5/cli/chiasmodon_cli.py`

 * *Files identical despite different names*

### Comparing `chiasmodon-2.0.4/pychiasmodon.py` & `chiasmodon-2.0.5/pychiasmodon.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 import os 
 import sys
 import time
 import requests
 from yaspin import Spinner 
 
-VERSION = "2.0.4"
+VERSION = "2.0.5"
 _API_URL = 'https://chiasmodon.com/v2/api/beta'
 _API_HEADERS = {'user-agent':'cli/python'}
 _VIEW_TYPE = {
     'full':[
         'cred.username',
         'cred.phone',
         'cred.password',
@@ -292,30 +292,35 @@
             if not re.match(r"\b(?:\d{1,3}\.){3}\d{1,3}\b", query):
                 self.print(f'{T.RED}Your format query is wrong!\nAccept only ipv4.{T.RESET}')
                 return False
         
         elif method == 'ip.asn':
             if not query.lower().startswith('as'):
                 self.print(f'{T.RED}Your format query is wrong!\nThe ASN starts with AS\nLike this: AS1234.{T.RESET}')
+                return False
         
         elif method in ['ip.port', 'url.port']:
             if not re.match(r":(\d+)", query):
                 self.print(f'{T.RED}Your format query is wrong!\nThis is not port.{T.RESET}')
+                return False
         
         elif method == 'cred.email':
             if not re.match(r'^[\w\.-]+@[\w\.-]+\.\w+$', query):
                 self.print(f'{T.RED}Your format query is wrong!\nThis is not email.{T.RESET}')
+                return False
         
         elif method == 'cred.country' or method == 'ip.country':
             if not len(query) == 2:
                 self.print(f'{T.RED}Your format query is wrong!\nAccept only country code.{T.RESET}')
+                return False
         
         elif method == 'url.path':
             if not query[0] == '/':
                 self.print(f'{T.RED}Your format query is wrong!\nThe url path moset be like: /somthing{T.RESET}')
+                return False
         
         return query
 
     def print(self,text, ys=None, ys_err=False) -> None:
         if text == None:return 
         if self.debug:
             if ys:
```

### Comparing `chiasmodon-2.0.4/setup.py` & `chiasmodon-2.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from distutils.core import setup
 from os import path
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='chiasmodon',
-      version='2.0.4',
+      version='2.0.5',
       description='Chiasmodon is an OSINT tool that allows users to gather information from various sources and conduct targeted searches based on domains, Google Play applications, email addresses, IP addresses, organizations, URLs, and more. It provides comprehensive scanning capabilities, customizable output formats, and additional options for enhanced data analysis and customization.',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='chiasmod0n',
       keywords='intelligence osint credentials emails asn cidr bugbounty subdomains information-gathering intelligence-analysis reconnaissance attack-surface subdomain-enumeration reconnaissance-framework bugbounty-tool email-enumeration chiasmodon',
       url='https://github.com/chiasmod0n/chiasmodon',
       packages=['.'],
```

