# Comparing `tmp/DeFiPy-0.0.8.tar.gz` & `tmp/DeFiPy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeFiPy-0.0.8.tar", last modified: Fri Jan 26 17:16:07 2024, max compression
+gzip compressed data, was "DeFiPy-0.0.9.tar", last modified: Fri Jan 26 17:24:12 2024, max compression
```

## Comparing `DeFiPy-0.0.8.tar` & `DeFiPy-0.0.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-01-26 17:16:07.410937 DeFiPy-0.0.8/
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-01-26 17:16:07.408231 DeFiPy-0.0.8/DeFiPy.egg-info/
--rw-r--r--   0 ian_moore   (501) staff       (20)      905 2024-01-26 17:16:07.000000 DeFiPy-0.0.8/DeFiPy.egg-info/PKG-INFO
--rw-r--r--   0 ian_moore   (501) staff       (20)      942 2024-01-26 17:16:07.000000 DeFiPy-0.0.8/DeFiPy.egg-info/SOURCES.txt
--rw-r--r--   0 ian_moore   (501) staff       (20)        1 2024-01-26 17:16:07.000000 DeFiPy-0.0.8/DeFiPy.egg-info/dependency_links.txt
--rw-r--r--   0 ian_moore   (501) staff       (20)        1 2024-01-25 16:23:18.000000 DeFiPy-0.0.8/DeFiPy.egg-info/not-zip-safe
--rw-r--r--   0 ian_moore   (501) staff       (20)       81 2024-01-26 17:16:07.000000 DeFiPy-0.0.8/DeFiPy.egg-info/requires.txt
--rw-r--r--   0 ian_moore   (501) staff       (20)        7 2024-01-26 17:16:07.000000 DeFiPy-0.0.8/DeFiPy.egg-info/top_level.txt
--rw-r--r--   0 ian_moore   (501) staff       (20)     1065 2023-10-11 21:49:49.000000 DeFiPy-0.0.8/LICENSE.txt
--rw-r--r--   0 ian_moore   (501) staff       (20)      905 2024-01-26 17:16:07.410859 DeFiPy-0.0.8/PKG-INFO
--rw-r--r--   0 ian_moore   (501) staff       (20)      500 2024-01-26 04:54:59.000000 DeFiPy-0.0.8/README.md
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-01-26 17:16:07.405740 DeFiPy-0.0.8/python/
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-01-26 17:16:07.408629 DeFiPy-0.0.8/python/prod/
--rw-r--r--   0 ian_moore   (501) staff       (20)      973 2024-01-26 03:57:07.000000 DeFiPy-0.0.8/python/prod/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-01-26 17:16:07.408759 DeFiPy-0.0.8/python/prod/erc/
--rw-r--r--   0 ian_moore   (501) staff       (20)       27 2024-01-26 02:19:35.000000 DeFiPy-0.0.8/python/prod/erc/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-01-26 17:16:07.406345 DeFiPy-0.0.8/python/prod/math/
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-01-26 17:16:07.408890 DeFiPy-0.0.8/python/prod/math/basic/
--rw-r--r--   0 ian_moore   (501) staff       (20)       34 2024-01-26 02:17:11.000000 DeFiPy-0.0.8/python/prod/math/basic/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-01-26 17:16:07.409022 DeFiPy-0.0.8/python/prod/math/interest/
--rw-r--r--   0 ian_moore   (501) staff       (20)       37 2024-01-26 02:16:13.000000 DeFiPy-0.0.8/python/prod/math/interest/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-01-26 17:16:07.409146 DeFiPy-0.0.8/python/prod/math/interest/ips/
--rw-r--r--   0 ian_moore   (501) staff       (20)       41 2024-01-26 02:16:35.000000 DeFiPy-0.0.8/python/prod/math/interest/ips/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-01-26 17:16:07.409273 DeFiPy-0.0.8/python/prod/math/interest/ips/aggregate/
--rw-r--r--   0 ian_moore   (501) staff       (20)       51 2024-01-26 02:16:46.000000 DeFiPy-0.0.8/python/prod/math/interest/ips/aggregate/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-01-26 17:16:07.409401 DeFiPy-0.0.8/python/prod/math/model/
--rw-r--r--   0 ian_moore   (501) staff       (20)       35 2024-01-26 02:15:54.000000 DeFiPy-0.0.8/python/prod/math/model/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-01-26 17:16:07.409527 DeFiPy-0.0.8/python/prod/math/risk/
--rw-r--r--   0 ian_moore   (501) staff       (20)       33 2024-01-26 02:15:27.000000 DeFiPy-0.0.8/python/prod/math/risk/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-01-26 17:16:07.409657 DeFiPy-0.0.8/python/prod/process/
--rw-r--r--   0 ian_moore   (501) staff       (20)       31 2024-01-26 02:09:47.000000 DeFiPy-0.0.8/python/prod/process/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-01-26 17:16:07.409781 DeFiPy-0.0.8/python/prod/process/burn/
--rw-r--r--   0 ian_moore   (501) staff       (20)       37 2024-01-26 02:09:55.000000 DeFiPy-0.0.8/python/prod/process/burn/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-01-26 17:16:07.409905 DeFiPy-0.0.8/python/prod/process/deposit/
--rw-r--r--   0 ian_moore   (501) staff       (20)       39 2024-01-26 02:10:08.000000 DeFiPy-0.0.8/python/prod/process/deposit/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-01-26 17:16:07.410046 DeFiPy-0.0.8/python/prod/process/liquidity/
--rw-r--r--   0 ian_moore   (501) staff       (20)       41 2024-01-26 02:10:21.000000 DeFiPy-0.0.8/python/prod/process/liquidity/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-01-26 17:16:07.410186 DeFiPy-0.0.8/python/prod/process/mint/
--rw-r--r--   0 ian_moore   (501) staff       (20)       36 2024-01-26 02:10:48.000000 DeFiPy-0.0.8/python/prod/process/mint/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-01-26 17:16:07.410310 DeFiPy-0.0.8/python/prod/process/swap/
--rw-r--r--   0 ian_moore   (501) staff       (20)       36 2024-01-26 02:10:58.000000 DeFiPy-0.0.8/python/prod/process/swap/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-01-26 17:16:07.410456 DeFiPy-0.0.8/python/prod/simulate/
--rw-r--r--   0 ian_moore   (501) staff       (20)       33 2024-01-26 02:09:34.000000 DeFiPy-0.0.8/python/prod/simulate/__init__.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       79 2024-01-26 17:16:07.411242 DeFiPy-0.0.8/setup.cfg
--rw-r--r--   0 ian_moore   (501) staff       (20)     1183 2024-01-26 17:15:26.000000 DeFiPy-0.0.8/setup.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-01-26 17:24:12.030180 DeFiPy-0.0.9/
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-01-26 17:24:12.027438 DeFiPy-0.0.9/DeFiPy.egg-info/
+-rw-r--r--   0 ian_moore   (501) staff       (20)      905 2024-01-26 17:24:11.000000 DeFiPy-0.0.9/DeFiPy.egg-info/PKG-INFO
+-rw-r--r--   0 ian_moore   (501) staff       (20)      942 2024-01-26 17:24:11.000000 DeFiPy-0.0.9/DeFiPy.egg-info/SOURCES.txt
+-rw-r--r--   0 ian_moore   (501) staff       (20)        1 2024-01-26 17:24:11.000000 DeFiPy-0.0.9/DeFiPy.egg-info/dependency_links.txt
+-rw-r--r--   0 ian_moore   (501) staff       (20)        1 2024-01-25 16:23:18.000000 DeFiPy-0.0.9/DeFiPy.egg-info/not-zip-safe
+-rw-r--r--   0 ian_moore   (501) staff       (20)       81 2024-01-26 17:24:11.000000 DeFiPy-0.0.9/DeFiPy.egg-info/requires.txt
+-rw-r--r--   0 ian_moore   (501) staff       (20)        7 2024-01-26 17:24:11.000000 DeFiPy-0.0.9/DeFiPy.egg-info/top_level.txt
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1065 2023-10-11 21:49:49.000000 DeFiPy-0.0.9/LICENSE.txt
+-rw-r--r--   0 ian_moore   (501) staff       (20)      905 2024-01-26 17:24:12.030112 DeFiPy-0.0.9/PKG-INFO
+-rw-r--r--   0 ian_moore   (501) staff       (20)      500 2024-01-26 17:22:51.000000 DeFiPy-0.0.9/README.md
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-01-26 17:24:12.024936 DeFiPy-0.0.9/python/
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-01-26 17:24:12.027887 DeFiPy-0.0.9/python/prod/
+-rw-r--r--   0 ian_moore   (501) staff       (20)      973 2024-01-26 03:57:07.000000 DeFiPy-0.0.9/python/prod/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-01-26 17:24:12.028016 DeFiPy-0.0.9/python/prod/erc/
+-rw-r--r--   0 ian_moore   (501) staff       (20)       27 2024-01-26 02:19:35.000000 DeFiPy-0.0.9/python/prod/erc/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-01-26 17:24:12.025514 DeFiPy-0.0.9/python/prod/math/
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-01-26 17:24:12.028172 DeFiPy-0.0.9/python/prod/math/basic/
+-rw-r--r--   0 ian_moore   (501) staff       (20)       34 2024-01-26 02:17:11.000000 DeFiPy-0.0.9/python/prod/math/basic/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-01-26 17:24:12.028317 DeFiPy-0.0.9/python/prod/math/interest/
+-rw-r--r--   0 ian_moore   (501) staff       (20)       37 2024-01-26 02:16:13.000000 DeFiPy-0.0.9/python/prod/math/interest/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-01-26 17:24:12.028456 DeFiPy-0.0.9/python/prod/math/interest/ips/
+-rw-r--r--   0 ian_moore   (501) staff       (20)       41 2024-01-26 02:16:35.000000 DeFiPy-0.0.9/python/prod/math/interest/ips/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-01-26 17:24:12.028603 DeFiPy-0.0.9/python/prod/math/interest/ips/aggregate/
+-rw-r--r--   0 ian_moore   (501) staff       (20)       51 2024-01-26 02:16:46.000000 DeFiPy-0.0.9/python/prod/math/interest/ips/aggregate/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-01-26 17:24:12.028728 DeFiPy-0.0.9/python/prod/math/model/
+-rw-r--r--   0 ian_moore   (501) staff       (20)       35 2024-01-26 02:15:54.000000 DeFiPy-0.0.9/python/prod/math/model/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-01-26 17:24:12.028853 DeFiPy-0.0.9/python/prod/math/risk/
+-rw-r--r--   0 ian_moore   (501) staff       (20)       33 2024-01-26 02:15:27.000000 DeFiPy-0.0.9/python/prod/math/risk/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-01-26 17:24:12.028983 DeFiPy-0.0.9/python/prod/process/
+-rw-r--r--   0 ian_moore   (501) staff       (20)       31 2024-01-26 02:09:47.000000 DeFiPy-0.0.9/python/prod/process/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-01-26 17:24:12.029107 DeFiPy-0.0.9/python/prod/process/burn/
+-rw-r--r--   0 ian_moore   (501) staff       (20)       37 2024-01-26 02:09:55.000000 DeFiPy-0.0.9/python/prod/process/burn/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-01-26 17:24:12.029228 DeFiPy-0.0.9/python/prod/process/deposit/
+-rw-r--r--   0 ian_moore   (501) staff       (20)       39 2024-01-26 02:10:08.000000 DeFiPy-0.0.9/python/prod/process/deposit/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-01-26 17:24:12.029348 DeFiPy-0.0.9/python/prod/process/liquidity/
+-rw-r--r--   0 ian_moore   (501) staff       (20)       41 2024-01-26 02:10:21.000000 DeFiPy-0.0.9/python/prod/process/liquidity/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-01-26 17:24:12.029472 DeFiPy-0.0.9/python/prod/process/mint/
+-rw-r--r--   0 ian_moore   (501) staff       (20)       36 2024-01-26 02:10:48.000000 DeFiPy-0.0.9/python/prod/process/mint/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-01-26 17:24:12.029598 DeFiPy-0.0.9/python/prod/process/swap/
+-rw-r--r--   0 ian_moore   (501) staff       (20)       36 2024-01-26 02:10:58.000000 DeFiPy-0.0.9/python/prod/process/swap/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-01-26 17:24:12.029721 DeFiPy-0.0.9/python/prod/simulate/
+-rw-r--r--   0 ian_moore   (501) staff       (20)       33 2024-01-26 02:09:34.000000 DeFiPy-0.0.9/python/prod/simulate/__init__.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       79 2024-01-26 17:24:12.030463 DeFiPy-0.0.9/setup.cfg
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1183 2024-01-26 17:22:48.000000 DeFiPy-0.0.9/setup.py
```

### Comparing `DeFiPy-0.0.8/DeFiPy.egg-info/PKG-INFO` & `DeFiPy-0.0.9/DeFiPy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: DeFiPy
-Version: 0.0.8
+Version: 0.0.9
 Summary: DeFi for Python
 Home-page: http://github.com/icmoore/defipy
 Author: icmoore
 Author-email: utiliwire@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: scipy>=1.7.3
 Requires-Dist: gmpy2>=2.0.8
 Requires-Dist: uniswappy>=1.1.2
-Requires-Dist: stableswappy>=0.0.4
+Requires-Dist: stableswappy>=0.0.6
 Requires-Dist: balancerpy>=0.0.6
 
 # defipy
 Python package for DeFi modelling
-* Currently in Beta (version 0.0.7) until fully tested and analyzed
+* Currently in Beta (version 0.0.9) until fully tested and analyzed
 * Decoupled into sub-repos, which include: [UniswapPy](https://github.com/icmoore/uniswappy), 
 [BalancerPy](https://github.com/icmoore/balancerpy), and [StableSwapPy](https://github.com/icmoore/stableswappy)
 
 ## Install
 To install package:
 ```
 > git clone https://github.com/icmoore/defipy
```

### Comparing `DeFiPy-0.0.8/DeFiPy.egg-info/SOURCES.txt` & `DeFiPy-0.0.9/DeFiPy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DeFiPy-0.0.8/LICENSE.txt` & `DeFiPy-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `DeFiPy-0.0.8/PKG-INFO` & `DeFiPy-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: DeFiPy
-Version: 0.0.8
+Version: 0.0.9
 Summary: DeFi for Python
 Home-page: http://github.com/icmoore/defipy
 Author: icmoore
 Author-email: utiliwire@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: scipy>=1.7.3
 Requires-Dist: gmpy2>=2.0.8
 Requires-Dist: uniswappy>=1.1.2
-Requires-Dist: stableswappy>=0.0.4
+Requires-Dist: stableswappy>=0.0.6
 Requires-Dist: balancerpy>=0.0.6
 
 # defipy
 Python package for DeFi modelling
-* Currently in Beta (version 0.0.7) until fully tested and analyzed
+* Currently in Beta (version 0.0.9) until fully tested and analyzed
 * Decoupled into sub-repos, which include: [UniswapPy](https://github.com/icmoore/uniswappy), 
 [BalancerPy](https://github.com/icmoore/balancerpy), and [StableSwapPy](https://github.com/icmoore/stableswappy)
 
 ## Install
 To install package:
 ```
 > git clone https://github.com/icmoore/defipy
```

### Comparing `DeFiPy-0.0.8/python/prod/__init__.py` & `DeFiPy-0.0.9/python/prod/__init__.py`

 * *Files identical despite different names*

### Comparing `DeFiPy-0.0.8/setup.py` & `DeFiPy-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(name='DeFiPy',
-      version='0.0.8',
+      version='0.0.9',
       description='DeFi for Python',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='http://github.com/icmoore/defipy',
       author = "icmoore",
       author_email = "utiliwire@gmail.com",
       license='MIT',
@@ -30,11 +30,11 @@
           'defipy.process.swap',
           'defipy.simulate'          
       ],
       install_requires=[
         'scipy >= 1.7.3', 
         'gmpy2 >= 2.0.8',
         'uniswappy >= 1.1.2', 
-        'stableswappy >= 0.0.4',
+        'stableswappy >= 0.0.6',
         'balancerpy >= 0.0.6'  
       ],      
       zip_safe=False)
```

