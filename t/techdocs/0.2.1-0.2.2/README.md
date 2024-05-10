# Comparing `tmp/techdocs-0.2.1.tar.gz` & `tmp/techdocs-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "techdocs-0.2.1.tar", last modified: Sat Nov  4 16:34:53 2023, max compression
+gzip compressed data, was "techdocs-0.2.2.tar", last modified: Fri May 10 19:47:14 2024, max compression
```

## Comparing `techdocs-0.2.1.tar` & `techdocs-0.2.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-11-04 16:34:53.151632 techdocs-0.2.1/
--rw-rw-rw-   0        0        0     8891 2023-11-04 16:34:53.151632 techdocs-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     8636 2023-10-26 08:30:54.000000 techdocs-0.2.1/README.md
--rw-rw-rw-   0        0        0      595 2023-11-04 16:30:16.000000 techdocs-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0      233 2023-11-04 16:34:53.154635 techdocs-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      628 2023-11-04 16:30:30.000000 techdocs-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-11-04 16:34:53.125489 techdocs-0.2.1/techdocs/
--rw-rw-rw-   0        0        0       21 2023-11-04 16:29:39.000000 techdocs-0.2.1/techdocs/__init__.py
--rw-rw-rw-   0        0        0      863 2023-10-26 08:30:54.000000 techdocs-0.2.1/techdocs/cli.py
--rw-rw-rw-   0        0        0      131 2023-10-02 18:20:15.000000 techdocs-0.2.1/techdocs/dtypes.py
--rw-rw-rw-   0        0        0     4146 2023-10-26 08:30:54.000000 techdocs-0.2.1/techdocs/ops.py
-drwxrwxrwx   0        0        0        0 2023-11-04 16:34:53.145551 techdocs-0.2.1/techdocs/signatures/
--rw-rw-rw-   0        0        0     1904 2023-10-02 18:20:15.000000 techdocs-0.2.1/techdocs/signatures/subcommand_signatures.json
-drwxrwxrwx   0        0        0        0 2023-11-04 16:34:53.149550 techdocs-0.2.1/techdocs/utils/
--rw-rw-rw-   0        0        0     2787 2023-10-26 08:30:54.000000 techdocs-0.2.1/techdocs/utils/LoggingManager.py
--rw-rw-rw-   0        0        0        0 2023-10-02 18:20:15.000000 techdocs-0.2.1/techdocs/utils/__init__.py
--rw-rw-rw-   0        0        0     2989 2023-11-04 16:27:57.000000 techdocs-0.2.1/techdocs/utils/functools.py
--rw-rw-rw-   0        0        0     1897 2023-10-26 08:30:54.000000 techdocs-0.2.1/techdocs/utils/parse.py
-drwxrwxrwx   0        0        0        0 2023-11-04 16:34:53.144551 techdocs-0.2.1/techdocs.egg-info/
--rw-rw-rw-   0        0        0     8891 2023-11-04 16:34:53.000000 techdocs-0.2.1/techdocs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      468 2023-11-04 16:34:53.000000 techdocs-0.2.1/techdocs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-04 16:34:53.000000 techdocs-0.2.1/techdocs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-11-04 16:34:53.000000 techdocs-0.2.1/techdocs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-11-04 16:34:53.000000 techdocs-0.2.1/techdocs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-11-04 16:34:53.000000 techdocs-0.2.1/techdocs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 19:47:14.216700 techdocs-0.2.2/
+-rw-rw-rw-   0        0        0     8877 2024-05-10 19:47:14.216700 techdocs-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8636 2024-01-07 10:33:13.000000 techdocs-0.2.2/README.md
+-rw-rw-rw-   0        0        0      581 2024-05-10 19:46:45.000000 techdocs-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0      233 2024-05-10 19:47:14.218703 techdocs-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      628 2024-05-10 19:46:06.000000 techdocs-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 19:47:14.185835 techdocs-0.2.2/techdocs/
+-rw-rw-rw-   0        0        0       21 2024-05-10 19:46:50.000000 techdocs-0.2.2/techdocs/__init__.py
+-rw-rw-rw-   0        0        0      863 2024-01-06 17:05:28.000000 techdocs-0.2.2/techdocs/cli.py
+-rw-rw-rw-   0        0        0      131 2024-01-06 17:05:28.000000 techdocs-0.2.2/techdocs/dtypes.py
+-rw-rw-rw-   0        0        0     4146 2024-01-06 17:05:28.000000 techdocs-0.2.2/techdocs/ops.py
+drwxrwxrwx   0        0        0        0 2024-05-10 19:47:14.208804 techdocs-0.2.2/techdocs/signatures/
+-rw-rw-rw-   0        0        0     1904 2024-01-06 17:05:28.000000 techdocs-0.2.2/techdocs/signatures/subcommand_signatures.json
+drwxrwxrwx   0        0        0        0 2024-05-10 19:47:14.213804 techdocs-0.2.2/techdocs/utils/
+-rw-rw-rw-   0        0        0     2787 2024-01-06 17:05:28.000000 techdocs-0.2.2/techdocs/utils/LoggingManager.py
+-rw-rw-rw-   0        0        0        0 2024-01-06 17:05:28.000000 techdocs-0.2.2/techdocs/utils/__init__.py
+-rw-rw-rw-   0        0        0     2802 2024-05-10 19:05:39.000000 techdocs-0.2.2/techdocs/utils/functools.py
+-rw-rw-rw-   0        0        0     1902 2024-05-10 19:33:09.000000 techdocs-0.2.2/techdocs/utils/parse.py
+drwxrwxrwx   0        0        0        0 2024-05-10 19:47:14.215153 techdocs-0.2.2/techdocs.egg-info/
+-rw-rw-rw-   0        0        0     8877 2024-05-10 19:47:14.000000 techdocs-0.2.2/techdocs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2024-05-10 19:47:14.000000 techdocs-0.2.2/techdocs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 19:47:14.000000 techdocs-0.2.2/techdocs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-05-10 19:47:14.000000 techdocs-0.2.2/techdocs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2024-05-10 19:47:14.000000 techdocs-0.2.2/techdocs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-10 19:47:14.000000 techdocs-0.2.2/techdocs.egg-info/top_level.txt
```

### Comparing `techdocs-0.2.1/PKG-INFO` & `techdocs-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: techdocs
-Version: 0.2.1
+Version: 0.2.2
 Summary: Code documentation generation CLI App
-Author-email: Caffiene Crew <caffienecrewhacks@gmail.com>
+Author-email: test <alfatrion123@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 
 ## Inspiration
 **Techdocs** really started as a passion project due to our indolent nature towards documenting our own codebases. We are currently working as core backend-microservice developers for an open-source organization - [Heritians](https://github.com/Heritians) at our University.
```

### Comparing `techdocs-0.2.1/README.md` & `techdocs-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `techdocs-0.2.1/setup.py` & `techdocs-0.2.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 from setuptools import setup
 import glob
 
 setup(
 	name='techdocs',
-	version='0.2.1',
+	version='0.2.2',
     # To provide executable scripts, use entry points in preference to the
     # "scripts" keyword. Entry points provide cross-platform support and allow
     # pip to create the appropriate form of executable for the target platform.
     entry_points={
         'console_scripts': [
             'techdocs=techdocs.cli:main'
         ],
```

### Comparing `techdocs-0.2.1/techdocs/cli.py` & `techdocs-0.2.2/techdocs/cli.py`

 * *Files identical despite different names*

### Comparing `techdocs-0.2.1/techdocs/ops.py` & `techdocs-0.2.2/techdocs/ops.py`

 * *Files identical despite different names*

### Comparing `techdocs-0.2.1/techdocs/signatures/subcommand_signatures.json` & `techdocs-0.2.2/techdocs/signatures/subcommand_signatures.json`

 * *Files identical despite different names*

### Comparing `techdocs-0.2.1/techdocs/utils/LoggingManager.py` & `techdocs-0.2.2/techdocs/utils/LoggingManager.py`

 * *Files identical despite different names*

### Comparing `techdocs-0.2.1/techdocs/utils/functools.py` & `techdocs-0.2.2/techdocs/utils/functools.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 import json
 import requests
 
 BASE_URL = "https://caffeinecrew-techdocs.hf.space"
 # BASE_URL = "http://127.0.0.1:8000"
 
 
+
 def get_access_token(data, return_refresh_token=False):
     try:
         url = BASE_URL + "/auth/login"
         headers = {
             "accept": "application/json",
         }
         data = json.dumps(data)
         response = requests.post(url, data=data, headers=headers)
         access_token = response.json()['access_token']
         if return_refresh_token:
             refresh_token = response.json()['refresh_token']
             return access_token, refresh_token
         return access_token
     except Exception as e:
-        if response.json() == "exception.InvalidCredentialsException()":  
-            print("Please check your credentials")
-        else:
-            print("Please verify your email before logging in")
+        print("Invlaid Credentials")
         return None
 
 
+
+
 def request_inference(config, code_block, max_retries=1):
 
     if max_retries == 0:
         return None
 
     url = BASE_URL+"/api/inference"
     headers={"accept":"application/json", "Authorization": f"Bearer {config['access_token']}"}
@@ -49,14 +49,15 @@
     
 
 def update_file(file_path, docstr_code):
     with open(file_path, "w",errors='ignore') as file:
         file.write(docstr_code)
 
 
+
 def issue_api_key(config):
     try:
         headers={"accept":"application/json", "Authorization": f"Bearer {config['access_token']}"}
         response = requests.put(url=BASE_URL + "/auth/regenerate_api_key", headers=headers, 
                                 data=json.dumps({"username": config['username']})
                                 )
         if (response.status_code!=200):
@@ -71,11 +72,11 @@
         headers={"accept":"application/json"}
         response = requests.post(url=BASE_URL + "/auth/signup", headers=headers, data=json.dumps(config))
         if (response.status_code==226):
             raise Exception("username or email already exists")
         elif (response.status_code!=200):
             raise Exception("Something went wrong, please try again later")
     
-        print(response.json()["message"][0].replace('\\n','\n'), "Then issue a new `API_KEY` to continue")
+        print("Signed up successfully, please issue a new `API_KEY` to continue")
 
     except Exception as e:
         print(e)
```

### Comparing `techdocs-0.2.1/techdocs/utils/parse.py` & `techdocs-0.2.2/techdocs/utils/parse.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     
     if isinstance(node, ast.FunctionDef):
         function_def = ast.unparse(node)
         response = request_inference(config=config, code_block=function_def)
         if response is not None:
             try:
                 docstr = response.split('"""')
-                docstring = ast.Expr(value=ast.Str(s=docstr[1]))
+                docstring = ast.Expr(value=ast.Constant(s=docstr[1]))
                 # print(f"Docstring generated for def {node.name}")
                 logging_manager = config.get("logging_manager")
                 logging_manager.set_log_handlers = [logging_manager.file_handler]
                 logging_manager.LOGGER.info(f"Docstring generated for def {node.name}")
                 node.body.insert(0, docstring)
             except IndexError:
                 pass
```

### Comparing `techdocs-0.2.1/techdocs.egg-info/PKG-INFO` & `techdocs-0.2.2/techdocs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: techdocs
-Version: 0.2.1
+Version: 0.2.2
 Summary: Code documentation generation CLI App
-Author-email: Caffiene Crew <caffienecrewhacks@gmail.com>
+Author-email: test <alfatrion123@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 
 ## Inspiration
 **Techdocs** really started as a passion project due to our indolent nature towards documenting our own codebases. We are currently working as core backend-microservice developers for an open-source organization - [Heritians](https://github.com/Heritians) at our University.
```

