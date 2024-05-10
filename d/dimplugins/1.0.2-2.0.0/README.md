# Comparing `tmp/dimplugins-1.0.2.tar.gz` & `tmp/dimplugins-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dimplugins-1.0.2.tar", last modified: Thu Nov  2 06:51:11 2023, max compression
+gzip compressed data, was "dist/dimplugins-2.0.0.tar", last modified: Fri May 10 15:46:42 2024, max compression
```

## Comparing `dimplugins-1.0.2.tar` & `dimplugins-2.0.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-11-02 06:51:11.000000 dimplugins-1.0.2/
--rw-r--r--   0 moky       (501) staff       (20)     1068 2023-11-02 06:51:11.000000 dimplugins-1.0.2/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      560 2022-12-11 05:05:26.000000 dimplugins-1.0.2/README.md
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-11-02 06:51:11.000000 dimplugins-1.0.2/dimplugins/
--rw-r--r--   0 moky       (501) staff       (20)     2962 2023-10-13 09:06:28.000000 dimplugins-1.0.2/dimplugins/__init__.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-11-02 06:51:11.000000 dimplugins-1.0.2/dimplugins/crypto/
--rw-r--r--   0 moky       (501) staff       (20)     3458 2023-10-13 08:46:10.000000 dimplugins-1.0.2/dimplugins/crypto/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6242 2023-10-13 08:45:12.000000 dimplugins-1.0.2/dimplugins/crypto/aes.py
--rw-r--r--   0 moky       (501) staff       (20)     2708 2023-01-31 05:24:56.000000 dimplugins-1.0.2/dimplugins/crypto/digest.py
--rw-r--r--   0 moky       (501) staff       (20)     7066 2023-10-29 07:55:53.000000 dimplugins-1.0.2/dimplugins/crypto/ecc.py
--rw-r--r--   0 moky       (501) staff       (20)     2462 2023-10-13 08:42:17.000000 dimplugins-1.0.2/dimplugins/crypto/plain.py
--rw-r--r--   0 moky       (501) staff       (20)     6840 2023-10-13 08:42:48.000000 dimplugins-1.0.2/dimplugins/crypto/rsa.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-11-02 06:51:11.000000 dimplugins-1.0.2/dimplugins/format/
--rw-r--r--   0 moky       (501) staff       (20)     2071 2023-10-13 09:01:38.000000 dimplugins-1.0.2/dimplugins/format/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3287 2023-10-13 08:59:35.000000 dimplugins-1.0.2/dimplugins/format/coder.py
--rw-r--r--   0 moky       (501) staff       (20)     5024 2023-10-12 12:42:46.000000 dimplugins-1.0.2/dimplugins/format/pnf.py
--rw-r--r--   0 moky       (501) staff       (20)     3009 2023-10-12 12:28:33.000000 dimplugins-1.0.2/dimplugins/format/ted.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-11-02 06:51:11.000000 dimplugins-1.0.2/dimplugins/mkm/
--rw-r--r--   0 moky       (501) staff       (20)     2273 2023-10-12 11:19:28.000000 dimplugins-1.0.2/dimplugins/mkm/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3639 2023-10-29 10:46:00.000000 dimplugins-1.0.2/dimplugins/mkm/address.py
--rw-r--r--   0 moky       (501) staff       (20)     3967 2023-10-12 11:09:42.000000 dimplugins-1.0.2/dimplugins/mkm/btc.py
--rw-r--r--   0 moky       (501) staff       (20)     3953 2023-10-29 08:07:14.000000 dimplugins-1.0.2/dimplugins/mkm/docs.py
--rw-r--r--   0 moky       (501) staff       (20)     4659 2023-10-12 11:09:53.000000 dimplugins-1.0.2/dimplugins/mkm/eth.py
--rw-r--r--   0 moky       (501) staff       (20)     4863 2023-10-12 11:18:46.000000 dimplugins-1.0.2/dimplugins/mkm/identifier.py
--rw-r--r--   0 moky       (501) staff       (20)     8519 2023-10-17 14:28:21.000000 dimplugins-1.0.2/dimplugins/mkm/meta.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-11-02 06:51:11.000000 dimplugins-1.0.2/dimplugins.egg-info/
--rw-r--r--   0 moky       (501) staff       (20)     1068 2023-11-02 06:51:11.000000 dimplugins-1.0.2/dimplugins.egg-info/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      649 2023-11-02 06:51:11.000000 dimplugins-1.0.2/dimplugins.egg-info/SOURCES.txt
--rw-r--r--   0 moky       (501) staff       (20)        1 2023-11-02 06:51:11.000000 dimplugins-1.0.2/dimplugins.egg-info/dependency_links.txt
--rw-r--r--   0 moky       (501) staff       (20)       60 2023-11-02 06:51:11.000000 dimplugins-1.0.2/dimplugins.egg-info/requires.txt
--rw-r--r--   0 moky       (501) staff       (20)       11 2023-11-02 06:51:11.000000 dimplugins-1.0.2/dimplugins.egg-info/top_level.txt
--rw-r--r--   0 moky       (501) staff       (20)       38 2023-11-02 06:51:11.000000 dimplugins-1.0.2/setup.cfg
--rw-r--r--   0 moky       (501) staff       (20)     1179 2023-10-29 10:37:59.000000 dimplugins-1.0.2/setup.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:46:42.000000 dimplugins-2.0.0/
+-rw-r--r--   0 moky       (501) staff       (20)     1068 2024-05-10 15:46:42.000000 dimplugins-2.0.0/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      560 2022-12-11 05:05:26.000000 dimplugins-2.0.0/README.md
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:46:42.000000 dimplugins-2.0.0/dimplugins/
+-rw-r--r--   0 moky       (501) staff       (20)     2962 2023-10-13 09:06:28.000000 dimplugins-2.0.0/dimplugins/__init__.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:46:42.000000 dimplugins-2.0.0/dimplugins/crypto/
+-rw-r--r--   0 moky       (501) staff       (20)     3458 2023-10-13 08:46:10.000000 dimplugins-2.0.0/dimplugins/crypto/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6242 2023-10-13 08:45:12.000000 dimplugins-2.0.0/dimplugins/crypto/aes.py
+-rw-r--r--   0 moky       (501) staff       (20)     2708 2023-01-31 05:24:56.000000 dimplugins-2.0.0/dimplugins/crypto/digest.py
+-rw-r--r--   0 moky       (501) staff       (20)     7066 2023-10-29 07:55:53.000000 dimplugins-2.0.0/dimplugins/crypto/ecc.py
+-rw-r--r--   0 moky       (501) staff       (20)     2462 2023-10-13 08:42:17.000000 dimplugins-2.0.0/dimplugins/crypto/plain.py
+-rw-r--r--   0 moky       (501) staff       (20)     6840 2023-10-13 08:42:48.000000 dimplugins-2.0.0/dimplugins/crypto/rsa.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:46:42.000000 dimplugins-2.0.0/dimplugins/format/
+-rw-r--r--   0 moky       (501) staff       (20)     2071 2023-10-13 09:01:38.000000 dimplugins-2.0.0/dimplugins/format/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3287 2023-10-13 08:59:35.000000 dimplugins-2.0.0/dimplugins/format/coder.py
+-rw-r--r--   0 moky       (501) staff       (20)     5024 2023-10-12 12:42:46.000000 dimplugins-2.0.0/dimplugins/format/pnf.py
+-rw-r--r--   0 moky       (501) staff       (20)     3009 2023-10-12 12:28:33.000000 dimplugins-2.0.0/dimplugins/format/ted.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:46:42.000000 dimplugins-2.0.0/dimplugins/mkm/
+-rw-r--r--   0 moky       (501) staff       (20)     2273 2023-10-12 11:19:28.000000 dimplugins-2.0.0/dimplugins/mkm/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3639 2023-10-29 10:46:00.000000 dimplugins-2.0.0/dimplugins/mkm/address.py
+-rw-r--r--   0 moky       (501) staff       (20)     3967 2023-10-12 11:09:42.000000 dimplugins-2.0.0/dimplugins/mkm/btc.py
+-rw-r--r--   0 moky       (501) staff       (20)     3953 2023-10-29 08:07:14.000000 dimplugins-2.0.0/dimplugins/mkm/docs.py
+-rw-r--r--   0 moky       (501) staff       (20)     4659 2023-10-12 11:09:53.000000 dimplugins-2.0.0/dimplugins/mkm/eth.py
+-rw-r--r--   0 moky       (501) staff       (20)     4863 2023-10-12 11:18:46.000000 dimplugins-2.0.0/dimplugins/mkm/identifier.py
+-rw-r--r--   0 moky       (501) staff       (20)     8519 2023-10-17 14:28:21.000000 dimplugins-2.0.0/dimplugins/mkm/meta.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:46:42.000000 dimplugins-2.0.0/dimplugins.egg-info/
+-rw-r--r--   0 moky       (501) staff       (20)     1068 2024-05-10 15:46:42.000000 dimplugins-2.0.0/dimplugins.egg-info/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      649 2024-05-10 15:46:42.000000 dimplugins-2.0.0/dimplugins.egg-info/SOURCES.txt
+-rw-r--r--   0 moky       (501) staff       (20)        1 2024-05-10 15:46:42.000000 dimplugins-2.0.0/dimplugins.egg-info/dependency_links.txt
+-rw-r--r--   0 moky       (501) staff       (20)       60 2024-05-10 15:46:42.000000 dimplugins-2.0.0/dimplugins.egg-info/requires.txt
+-rw-r--r--   0 moky       (501) staff       (20)       11 2024-05-10 15:46:42.000000 dimplugins-2.0.0/dimplugins.egg-info/top_level.txt
+-rw-r--r--   0 moky       (501) staff       (20)       38 2024-05-10 15:46:42.000000 dimplugins-2.0.0/setup.cfg
+-rw-r--r--   0 moky       (501) staff       (20)     1179 2024-05-10 15:43:11.000000 dimplugins-2.0.0/setup.py
```

### Comparing `dimplugins-1.0.2/PKG-INFO` & `dimplugins-2.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimplugins
-Version: 1.0.2
+Version: 2.0.0
 Summary: Decentralized Instant Messaging (Python Plugins)
 Home-page: https://github.com/dimchat/sdk-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # Decentralized Instant Messaging (Python Plugins)
```

### Comparing `dimplugins-1.0.2/README.md` & `dimplugins-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `dimplugins-1.0.2/dimplugins/__init__.py` & `dimplugins-2.0.0/dimplugins/__init__.py`

 * *Files identical despite different names*

### Comparing `dimplugins-1.0.2/dimplugins/crypto/__init__.py` & `dimplugins-2.0.0/dimplugins/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `dimplugins-1.0.2/dimplugins/crypto/aes.py` & `dimplugins-2.0.0/dimplugins/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `dimplugins-1.0.2/dimplugins/crypto/digest.py` & `dimplugins-2.0.0/dimplugins/crypto/digest.py`

 * *Files identical despite different names*

### Comparing `dimplugins-1.0.2/dimplugins/crypto/ecc.py` & `dimplugins-2.0.0/dimplugins/crypto/ecc.py`

 * *Files identical despite different names*

### Comparing `dimplugins-1.0.2/dimplugins/crypto/plain.py` & `dimplugins-2.0.0/dimplugins/crypto/plain.py`

 * *Files identical despite different names*

### Comparing `dimplugins-1.0.2/dimplugins/crypto/rsa.py` & `dimplugins-2.0.0/dimplugins/crypto/rsa.py`

 * *Files identical despite different names*

### Comparing `dimplugins-1.0.2/dimplugins/format/__init__.py` & `dimplugins-2.0.0/dimplugins/format/__init__.py`

 * *Files identical despite different names*

### Comparing `dimplugins-1.0.2/dimplugins/format/coder.py` & `dimplugins-2.0.0/dimplugins/format/coder.py`

 * *Files identical despite different names*

### Comparing `dimplugins-1.0.2/dimplugins/format/pnf.py` & `dimplugins-2.0.0/dimplugins/format/pnf.py`

 * *Files identical despite different names*

### Comparing `dimplugins-1.0.2/dimplugins/format/ted.py` & `dimplugins-2.0.0/dimplugins/format/ted.py`

 * *Files identical despite different names*

### Comparing `dimplugins-1.0.2/dimplugins/mkm/__init__.py` & `dimplugins-2.0.0/dimplugins/mkm/__init__.py`

 * *Files identical despite different names*

### Comparing `dimplugins-1.0.2/dimplugins/mkm/address.py` & `dimplugins-2.0.0/dimplugins/mkm/address.py`

 * *Files identical despite different names*

### Comparing `dimplugins-1.0.2/dimplugins/mkm/btc.py` & `dimplugins-2.0.0/dimplugins/mkm/btc.py`

 * *Files identical despite different names*

### Comparing `dimplugins-1.0.2/dimplugins/mkm/docs.py` & `dimplugins-2.0.0/dimplugins/mkm/docs.py`

 * *Files identical despite different names*

### Comparing `dimplugins-1.0.2/dimplugins/mkm/eth.py` & `dimplugins-2.0.0/dimplugins/mkm/eth.py`

 * *Files identical despite different names*

### Comparing `dimplugins-1.0.2/dimplugins/mkm/identifier.py` & `dimplugins-2.0.0/dimplugins/mkm/identifier.py`

 * *Files identical despite different names*

### Comparing `dimplugins-1.0.2/dimplugins/mkm/meta.py` & `dimplugins-2.0.0/dimplugins/mkm/meta.py`

 * *Files identical despite different names*

### Comparing `dimplugins-1.0.2/dimplugins.egg-info/PKG-INFO` & `dimplugins-2.0.0/dimplugins.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimplugins
-Version: 1.0.2
+Version: 2.0.0
 Summary: Decentralized Instant Messaging (Python Plugins)
 Home-page: https://github.com/dimchat/sdk-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # Decentralized Instant Messaging (Python Plugins)
```

### Comparing `dimplugins-1.0.2/dimplugins.egg-info/SOURCES.txt` & `dimplugins-2.0.0/dimplugins.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dimplugins-1.0.2/setup.py` & `dimplugins-2.0.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Plugins for MingKeMing module
 """
 
 import io
 
 from setuptools import setup, find_packages
 
-__version__ = '1.0.2'
+__version__ = '2.0.0'
 __author__ = 'Albert Moky'
 __contact__ = 'albert.moky@gmail.com'
 
 with io.open('README.md', 'r', encoding='utf-8') as fh:
     readme = fh.read()
 
 setup(
@@ -35,16 +35,16 @@
     },
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     install_requires=[
-        'dimp>=1.0.2',
-        'dkd>=1.0.2',
-        'mkm>=1.0.2',
+        'dimp>=2.0.0',
+        'dkd>=2.0.0',
+        'mkm>=2.0.0',
 
         'pycryptodome',  # 3.14.1
         'base58',  # 1.0.3
         'ecdsa',   # 0.16.1
     ]
 )
```

