# Comparing `tmp/smartbetsapi-1.3.0.tar.gz` & `tmp/smartbetsapi-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartbetsapi-1.3.0.tar", last modified: Mon May  6 09:17:00 2024, max compression
+gzip compressed data, was "smartbetsapi-1.3.1.tar", last modified: Fri May 10 14:31:51 2024, max compression
```

## Comparing `smartbetsapi-1.3.0.tar` & `smartbetsapi-1.3.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:17:00.955186 smartbetsapi-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-06 09:16:52.000000 smartbetsapi-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11610 2024-05-06 09:17:00.955186 smartbetsapi-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-05-06 09:16:52.000000 smartbetsapi-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 09:17:00.955186 smartbetsapi-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-06 09:16:52.000000 smartbetsapi-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:17:00.955186 smartbetsapi-1.3.0/smartbetsAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11610 2024-05-06 09:17:00.000000 smartbetsapi-1.3.0/smartbetsAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-06 09:17:00.000000 smartbetsapi-1.3.0/smartbetsAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 09:17:00.000000 smartbetsapi-1.3.0/smartbetsAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-06 09:17:00.000000 smartbetsapi-1.3.0/smartbetsAPI.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-06 09:17:00.000000 smartbetsapi-1.3.0/smartbetsAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-06 09:17:00.000000 smartbetsapi-1.3.0/smartbetsAPI.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:17:00.955186 smartbetsapi-1.3.0/smartbets_API/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-06 09:16:52.000000 smartbetsapi-1.3.0/smartbets_API/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-06 09:16:52.000000 smartbetsapi-1.3.0/smartbets_API/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-06 09:16:52.000000 smartbetsapi-1.3.0/smartbets_API/bet_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-06 09:16:52.000000 smartbetsapi-1.3.0/smartbets_API/bet_at_rest_api_level.py
--rw-r--r--   0 runner    (1001) docker     (127)    11318 2024-05-06 09:16:52.000000 smartbetsapi-1.3.0/smartbets_API/bet_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-06 09:16:52.000000 smartbetsapi-1.3.0/smartbets_API/configuration_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6613 2024-05-06 09:16:52.000000 smartbetsapi-1.3.0/smartbets_API/figure_harvester.py
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-06 09:16:52.000000 smartbetsapi-1.3.0/smartbets_API/googler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-05-06 09:16:52.000000 smartbetsapi-1.3.0/smartbets_API/html_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     6773 2024-05-06 09:16:52.000000 smartbetsapi-1.3.0/smartbets_API/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-05-06 09:16:52.000000 smartbetsapi-1.3.0/smartbets_API/predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-06 09:16:52.000000 smartbetsapi-1.3.0/smartbets_API/proxyh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-06 09:16:52.000000 smartbetsapi-1.3.0/smartbets_API/tertiary_bet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:31:51.403237 smartbetsapi-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-10 14:31:47.000000 smartbetsapi-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11646 2024-05-10 14:31:51.403237 smartbetsapi-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-05-10 14:31:47.000000 smartbetsapi-1.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 14:31:51.403237 smartbetsapi-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-10 14:31:47.000000 smartbetsapi-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:31:51.403237 smartbetsapi-1.3.1/smartbetsAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11646 2024-05-10 14:31:51.000000 smartbetsapi-1.3.1/smartbetsAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-10 14:31:51.000000 smartbetsapi-1.3.1/smartbetsAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 14:31:51.000000 smartbetsapi-1.3.1/smartbetsAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-10 14:31:51.000000 smartbetsapi-1.3.1/smartbetsAPI.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-10 14:31:51.000000 smartbetsapi-1.3.1/smartbetsAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-10 14:31:51.000000 smartbetsapi-1.3.1/smartbetsAPI.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:31:51.403237 smartbetsapi-1.3.1/smartbets_API/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-10 14:31:47.000000 smartbetsapi-1.3.1/smartbets_API/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-10 14:31:47.000000 smartbetsapi-1.3.1/smartbets_API/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-10 14:31:47.000000 smartbetsapi-1.3.1/smartbets_API/bet_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-10 14:31:47.000000 smartbetsapi-1.3.1/smartbets_API/bet_at_rest_api_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11318 2024-05-10 14:31:47.000000 smartbetsapi-1.3.1/smartbets_API/bet_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-10 14:31:47.000000 smartbetsapi-1.3.1/smartbets_API/configuration_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6613 2024-05-10 14:31:47.000000 smartbetsapi-1.3.1/smartbets_API/figure_harvester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-10 14:31:47.000000 smartbetsapi-1.3.1/smartbets_API/googler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6391 2024-05-10 14:31:47.000000 smartbetsapi-1.3.1/smartbets_API/html_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6773 2024-05-10 14:31:47.000000 smartbetsapi-1.3.1/smartbets_API/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-05-10 14:31:47.000000 smartbetsapi-1.3.1/smartbets_API/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-10 14:31:47.000000 smartbetsapi-1.3.1/smartbets_API/proxyh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-10 14:31:47.000000 smartbetsapi-1.3.1/smartbets_API/tertiary_bet.py
```

### Comparing `smartbetsapi-1.3.0/LICENSE` & `smartbetsapi-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `smartbetsapi-1.3.0/PKG-INFO` & `smartbetsapi-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartbetsAPI
-Version: 1.3.0
+Version: 1.3.1
 Summary: Simple football prediction API
 Home-page: https://github.com/Simatwa/smartbetsAPI
 Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa Caleb
 Maintainer-email: smartwacaleb@gmail.com
 License: GPL-3.0
@@ -35,14 +35,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: appdirs==1.4.4
 Requires-Dist: requests[socks]==2.31.0
 Requires-Dist: colorama==0.4.6
 Requires-Dist: bs4==0.0.1
 Requires-Dist: Faker==15.3.4
+Requires-Dist: pyfreeproxies==0.1.1
 Provides-Extra: api
 Requires-Dist: fastapi[all]==0.110.1; extra == "api"
 
 <h1 align="center">smartbetsAPI</h1>
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: smartbetsAPI Version: 1.3.0 Summary: Simple
+Metadata-Version: 2.1 Name: smartbetsAPI Version: 1.3.1 Summary: Simple
 football prediction API Home-page: https://github.com/Simatwa/smartbetsAPI
 Author: Smartwa Caleb Author-email: smartwacaleb@gmail.com Maintainer: Smartwa
 Caleb Maintainer-email: smartwacaleb@gmail.com License: GPL-3.0 Project-URL:
 Bug Report, https://github.com/Simatwa/smartbetsAPI/issues/new Project-URL:
 Homepage, https://github.com/Simatwa/smartbetsAPI Project-URL: Source Code,
 https://github.com/Simatwa/smartbetsAPI Project-URL: Issue Tracker, https://
 github.com/Simatwa/smartbetsAPI/issues Project-URL: Download, https://
@@ -18,16 +18,17 @@
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Games/Entertainment Requires-Python: >=3.9 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: appdirs==1.4.4
 Requires-Dist: requests[socks]==2.31.0 Requires-Dist: colorama==0.4.6 Requires-
-Dist: bs4==0.0.1 Requires-Dist: Faker==15.3.4 Provides-Extra: api Requires-
-Dist: fastapi[all]==0.110.1; extra == "api"
+Dist: bs4==0.0.1 Requires-Dist: Faker==15.3.4 Requires-Dist:
+pyfreeproxies==0.1.1 Provides-Extra: api Requires-Dist: fastapi[all]==0.110.1;
+extra == "api"
                           ************ ssmmaarrttbbeettssAAPPII ************
      _[_G_i_t_h_u_b_]_[_L_i_c_e_n_s_e_]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_A_c_c_u_r_a_c_y_]_[_P_a_s_s_i_n_g_]_[_c_o_v_e_r_a_g_e_]_[_P_r_o_g_r_e_s_s_]
                                   _[_D_o_w_n_l_o_a_d_s_]
 
 > "Punter's choice" Worldwide soccer-matches predictor with Fast-API and a
 package for integrating the scripts in your own [Python](https://python.org)
 code. ## Features - REST-API - Script integration (package) - Non-ML ##
```

### Comparing `smartbetsapi-1.3.0/README.md` & `smartbetsapi-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `smartbetsapi-1.3.0/setup.py` & `smartbetsapi-1.3.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,17 +22,20 @@
     long_description_content_type="text/markdown",
     install_requires=[
         "appdirs==1.4.4",
         "requests[socks]==2.31.0",
         "colorama==0.4.6",
         "bs4==0.0.1",
         "Faker==15.3.4",
+        "pyfreeproxies==0.1.1",
     ],
     extras_require={
-        'api' : ["fastapi[all]==0.110.1",]
+        "api": [
+            "fastapi[all]==0.110.1",
+        ]
     },
     python_requires=">=3.9",
     project_urls={
         "Bug Report": "https://github.com/Simatwa/smartbetsAPI/issues/new",
         "Homepage": "https://github.com/Simatwa/smartbetsAPI",
         "Source Code": "https://github.com/Simatwa/smartbetsAPI",
         "Issue Tracker": "https://github.com/Simatwa/smartbetsAPI/issues",
```

### Comparing `smartbetsapi-1.3.0/smartbetsAPI.egg-info/PKG-INFO` & `smartbetsapi-1.3.1/smartbetsAPI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartbetsAPI
-Version: 1.3.0
+Version: 1.3.1
 Summary: Simple football prediction API
 Home-page: https://github.com/Simatwa/smartbetsAPI
 Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa Caleb
 Maintainer-email: smartwacaleb@gmail.com
 License: GPL-3.0
@@ -35,14 +35,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: appdirs==1.4.4
 Requires-Dist: requests[socks]==2.31.0
 Requires-Dist: colorama==0.4.6
 Requires-Dist: bs4==0.0.1
 Requires-Dist: Faker==15.3.4
+Requires-Dist: pyfreeproxies==0.1.1
 Provides-Extra: api
 Requires-Dist: fastapi[all]==0.110.1; extra == "api"
 
 <h1 align="center">smartbetsAPI</h1>
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: smartbetsAPI Version: 1.3.0 Summary: Simple
+Metadata-Version: 2.1 Name: smartbetsAPI Version: 1.3.1 Summary: Simple
 football prediction API Home-page: https://github.com/Simatwa/smartbetsAPI
 Author: Smartwa Caleb Author-email: smartwacaleb@gmail.com Maintainer: Smartwa
 Caleb Maintainer-email: smartwacaleb@gmail.com License: GPL-3.0 Project-URL:
 Bug Report, https://github.com/Simatwa/smartbetsAPI/issues/new Project-URL:
 Homepage, https://github.com/Simatwa/smartbetsAPI Project-URL: Source Code,
 https://github.com/Simatwa/smartbetsAPI Project-URL: Issue Tracker, https://
 github.com/Simatwa/smartbetsAPI/issues Project-URL: Download, https://
@@ -18,16 +18,17 @@
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Games/Entertainment Requires-Python: >=3.9 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: appdirs==1.4.4
 Requires-Dist: requests[socks]==2.31.0 Requires-Dist: colorama==0.4.6 Requires-
-Dist: bs4==0.0.1 Requires-Dist: Faker==15.3.4 Provides-Extra: api Requires-
-Dist: fastapi[all]==0.110.1; extra == "api"
+Dist: bs4==0.0.1 Requires-Dist: Faker==15.3.4 Requires-Dist:
+pyfreeproxies==0.1.1 Provides-Extra: api Requires-Dist: fastapi[all]==0.110.1;
+extra == "api"
                           ************ ssmmaarrttbbeettssAAPPII ************
      _[_G_i_t_h_u_b_]_[_L_i_c_e_n_s_e_]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_A_c_c_u_r_a_c_y_]_[_P_a_s_s_i_n_g_]_[_c_o_v_e_r_a_g_e_]_[_P_r_o_g_r_e_s_s_]
                                   _[_D_o_w_n_l_o_a_d_s_]
 
 > "Punter's choice" Worldwide soccer-matches predictor with Fast-API and a
 package for integrating the scripts in your own [Python](https://python.org)
 code. ## Features - REST-API - Script integration (package) - Non-ML ##
```

### Comparing `smartbetsapi-1.3.0/smartbetsAPI.egg-info/SOURCES.txt` & `smartbetsapi-1.3.1/smartbetsAPI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `smartbetsapi-1.3.0/smartbets_API/bet_analyzer.py` & `smartbetsapi-1.3.1/smartbets_API/bet_analyzer.py`

 * *Files identical despite different names*

### Comparing `smartbetsapi-1.3.0/smartbets_API/bet_at_rest_api_level.py` & `smartbetsapi-1.3.1/smartbets_API/bet_at_rest_api_level.py`

 * *Files identical despite different names*

### Comparing `smartbetsapi-1.3.0/smartbets_API/bet_common.py` & `smartbetsapi-1.3.1/smartbets_API/bet_common.py`

 * *Files identical despite different names*

### Comparing `smartbetsapi-1.3.0/smartbets_API/configuration_handler.py` & `smartbetsapi-1.3.1/smartbets_API/configuration_handler.py`

 * *Files identical despite different names*

### Comparing `smartbetsapi-1.3.0/smartbets_API/figure_harvester.py` & `smartbetsapi-1.3.1/smartbets_API/figure_harvester.py`

 * *Files identical despite different names*

### Comparing `smartbetsapi-1.3.0/smartbets_API/googler.py` & `smartbetsapi-1.3.1/smartbets_API/googler.py`

 * *Files identical despite different names*

### Comparing `smartbetsapi-1.3.0/smartbets_API/html_fetcher.py` & `smartbetsapi-1.3.1/smartbets_API/html_fetcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from faker import Faker
 from .proxyh import hunter45
 
 
 class web:
     def __init__(self):
         self.used, self.exc, self.user_agent, self.ref = [], [], [], []
-        self.hunter = hunter45(req)
+        self.hunter = hunter45()
         pr = self.hunter.get_proxy()
         if pr[0]:
             self.proxies = pr[1]
         else:
             logging.error(pr[1])
             self.proxies = []
```

### Comparing `smartbetsapi-1.3.0/smartbets_API/interface.py` & `smartbetsapi-1.3.1/smartbets_API/interface.py`

 * *Files identical despite different names*

### Comparing `smartbetsapi-1.3.0/smartbets_API/predictor.py` & `smartbetsapi-1.3.1/smartbets_API/predictor.py`

 * *Files identical despite different names*

### Comparing `smartbetsapi-1.3.0/smartbets_API/tertiary_bet.py` & `smartbetsapi-1.3.1/smartbets_API/tertiary_bet.py`

 * *Files identical despite different names*

