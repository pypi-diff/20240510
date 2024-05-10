# Comparing `tmp/fastapi-tusd-0.100.1.tar.gz` & `tmp/fastapi-tusd-0.100.1.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/fastapi-tusd/fastapi-tusd/dist/.tmp-xh6n_k3e/fastapi-tusd-0.100.1.tar", last modified: Fri Jul 14 07:35:45 2023, max compression
+gzip compressed data, was "/home/runner/work/fastapi-tusd/fastapi-tusd/dist/.tmp-xne8xgwq/fastapi-tusd-0.100.1.post0.tar", last modified: Fri May 10 09:16:16 2024, max compression
```

## Comparing `fastapi-tusd-0.100.1.tar` & `fastapi-tusd-0.100.1.post0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:35:45.000000 fastapi-tusd-0.100.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:35:45.000000 fastapi-tusd-0.100.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:35:45.000000 fastapi-tusd-0.100.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-14 07:35:32.000000 fastapi-tusd-0.100.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-14 07:35:32.000000 fastapi-tusd-0.100.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-14 07:35:32.000000 fastapi-tusd-0.100.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-14 07:35:32.000000 fastapi-tusd-0.100.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-14 07:35:45.000000 fastapi-tusd-0.100.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-14 07:35:32.000000 fastapi-tusd-0.100.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:35:45.000000 fastapi-tusd-0.100.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-14 07:35:32.000000 fastapi-tusd-0.100.1/examples/app_tusd.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-14 07:35:32.000000 fastapi-tusd-0.100.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-14 07:35:32.000000 fastapi-tusd-0.100.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-14 07:35:45.000000 fastapi-tusd-0.100.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-14 07:35:32.000000 fastapi-tusd-0.100.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:35:45.000000 fastapi-tusd-0.100.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:35:45.000000 fastapi-tusd-0.100.1/src/fastapi_tusd/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-14 07:35:32.000000 fastapi-tusd-0.100.1/src/fastapi_tusd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-14 07:35:32.000000 fastapi-tusd-0.100.1/src/fastapi_tusd/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-14 07:35:32.000000 fastapi-tusd-0.100.1/src/fastapi_tusd/filestore.py
--rw-r--r--   0 runner    (1001) docker     (123)    11091 2023-07-14 07:35:32.000000 fastapi-tusd-0.100.1/src/fastapi_tusd/tusd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:35:45.000000 fastapi-tusd-0.100.1/src/fastapi_tusd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-14 07:35:45.000000 fastapi-tusd-0.100.1/src/fastapi_tusd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-14 07:35:45.000000 fastapi-tusd-0.100.1/src/fastapi_tusd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 07:35:45.000000 fastapi-tusd-0.100.1/src/fastapi_tusd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 07:35:44.000000 fastapi-tusd-0.100.1/src/fastapi_tusd.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-14 07:35:45.000000 fastapi-tusd-0.100.1/src/fastapi_tusd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-14 07:35:45.000000 fastapi-tusd-0.100.1/src/fastapi_tusd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:16:16.000000 fastapi-tusd-0.100.1.post0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:16:16.000000 fastapi-tusd-0.100.1.post0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:16:16.000000 fastapi-tusd-0.100.1.post0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-10 09:16:10.000000 fastapi-tusd-0.100.1.post0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-10 09:16:10.000000 fastapi-tusd-0.100.1.post0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-10 09:16:10.000000 fastapi-tusd-0.100.1.post0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-10 09:16:10.000000 fastapi-tusd-0.100.1.post0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-10 09:16:16.000000 fastapi-tusd-0.100.1.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-10 09:16:10.000000 fastapi-tusd-0.100.1.post0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:16:16.000000 fastapi-tusd-0.100.1.post0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-10 09:16:10.000000 fastapi-tusd-0.100.1.post0/examples/app_tusd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-10 09:16:10.000000 fastapi-tusd-0.100.1.post0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-10 09:16:10.000000 fastapi-tusd-0.100.1.post0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-10 09:16:16.000000 fastapi-tusd-0.100.1.post0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-10 09:16:10.000000 fastapi-tusd-0.100.1.post0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:16:16.000000 fastapi-tusd-0.100.1.post0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:16:16.000000 fastapi-tusd-0.100.1.post0/src/fastapi_tusd/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-10 09:16:10.000000 fastapi-tusd-0.100.1.post0/src/fastapi_tusd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-10 09:16:10.000000 fastapi-tusd-0.100.1.post0/src/fastapi_tusd/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-05-10 09:16:10.000000 fastapi-tusd-0.100.1.post0/src/fastapi_tusd/filestore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11091 2024-05-10 09:16:10.000000 fastapi-tusd-0.100.1.post0/src/fastapi_tusd/tusd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:16:16.000000 fastapi-tusd-0.100.1.post0/src/fastapi_tusd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-10 09:16:16.000000 fastapi-tusd-0.100.1.post0/src/fastapi_tusd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-10 09:16:16.000000 fastapi-tusd-0.100.1.post0/src/fastapi_tusd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 09:16:16.000000 fastapi-tusd-0.100.1.post0/src/fastapi_tusd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 09:16:15.000000 fastapi-tusd-0.100.1.post0/src/fastapi_tusd.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-10 09:16:16.000000 fastapi-tusd-0.100.1.post0/src/fastapi_tusd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-10 09:16:16.000000 fastapi-tusd-0.100.1.post0/src/fastapi_tusd.egg-info/top_level.txt
```

### Comparing `fastapi-tusd-0.100.1/.github/workflows/publish.yml` & `fastapi-tusd-0.100.1.post0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fastapi-tusd-0.100.1/.gitignore` & `fastapi-tusd-0.100.1.post0/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi-tusd-0.100.1/LICENSE` & `fastapi-tusd-0.100.1.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-tusd-0.100.1/PKG-INFO` & `fastapi-tusd-0.100.1.post0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: fastapi-tusd
-Version: 0.100.1
+Version: 0.100.1.post0
 Summary: FastAPI extention implementing the tus server
 Home-page: https://github.com/liviaerxin/fastapi_tusd
 Author: Frank
 Author-email: 1yue8haogaoqi@gmail.com
 License: MIT license
-Keywords: fastapi_tusd
+Keywords: fastapi-tusd
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development
 Classifier: Framework :: FastAPI
 Classifier: Framework :: Pydantic
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
@@ -26,36 +26,51 @@
 Provides-Extra: format
 Provides-Extra: dev
 License-File: LICENSE
 License-File: AUTHORS.md
 
 # FastAPI Server for Tus Protocol
 
-A file upload server of the tus resumable upload protocol is implemented on FastAPI framework.  
+A file upload server of the tus resumable upload protocol is implemented on **FastAPI** framework.  
+
+Thanks to [tusd](https://github.com/tus/tusd), it provides great ideas and a sensible design pattern to implement `Tus` protocol to support multiple backend storage implementations.
+
+**Features**:
+
+- [x] Basic operations to support Core Protocol such as **HEAD**, **POST**, **PATCH**, **DELETE**
+  - [x] Creation With Upload
+  - [ ] Checksum such as md5
+  - [ ] Expiration
+  - [ ] Concatenation
+- [x] File storage
+- [ ] S3 storage
+
 
 ## Getting started
 
 Import `TusRouter` to your application,
 
 ```py title=main.py
 from fastapi import FastAPI
 from fastapi_tusd import TusRouter
 
 app = FastAPI()
 
+# `store_dir`: the folder to store uploaded files
+#  `location`: the API endpoint to serve, like `http://127.0.0.1:8000/files` or relative path `files` (TODO: induced from `prefix` in default)
 app.include_router(TusRouter(store_dir="./files", location="/files"), prefix="/files")
 ```
 
 Then the tus upload endpoints will be served at `http://127.0.0.1:8000/files`, more information is available at `http://127.0.0.1:8000/docs`
 
 ### Examples
 
-There a simple example with web file upload client supporting for `Tus` protocol, thanks to `Uppy`!
+There is a simple example with a web file upload client supporting for `Tus` protocol, thanks to `Uppy`!
 
-Enter the `example/` folder, run(`pip install uvicorn` if no `uvicorn`!)
+Enter the `example/` folder, and run(`pip install `uvicorn` if no `uvicorn`!)
 
 ```sh
 uvicorn app_tusd:app --reload
 ```
 
 Then visit `https://127.0.0.1:8000/upload.thml`
```

### Comparing `fastapi-tusd-0.100.1/examples/app_tusd.py` & `fastapi-tusd-0.100.1.post0/examples/app_tusd.py`

 * *Files identical despite different names*

### Comparing `fastapi-tusd-0.100.1/setup.cfg` & `fastapi-tusd-0.100.1.post0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = fastapi-tusd
 version = attr: fastapi_tusd.__version__
 author = Frank
 author_email = 1yue8haogaoqi@gmail.com
 description = FastAPI extention implementing the tus server
 long_description = file: README.md, License
 long_description_content_type = text/markdown
-keywords = fastapi_tusd
+keywords = fastapi-tusd
 url = https://github.com/liviaerxin/fastapi_tusd
 license = MIT license
 classifiers = 
 	Topic :: Software Development :: Libraries :: Python Modules
 	Topic :: Software Development :: Libraries
 	Topic :: Software Development
 	Framework :: FastAPI
```

### Comparing `fastapi-tusd-0.100.1/src/fastapi_tusd/filestore.py` & `fastapi-tusd-0.100.1.post0/src/fastapi_tusd/filestore.py`

 * *Files identical despite different names*

### Comparing `fastapi-tusd-0.100.1/src/fastapi_tusd/tusd.py` & `fastapi-tusd-0.100.1.post0/src/fastapi_tusd/tusd.py`

 * *Files identical despite different names*

### Comparing `fastapi-tusd-0.100.1/src/fastapi_tusd.egg-info/PKG-INFO` & `fastapi-tusd-0.100.1.post0/src/fastapi_tusd.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: fastapi-tusd
-Version: 0.100.1
+Version: 0.100.1.post0
 Summary: FastAPI extention implementing the tus server
 Home-page: https://github.com/liviaerxin/fastapi_tusd
 Author: Frank
 Author-email: 1yue8haogaoqi@gmail.com
 License: MIT license
-Keywords: fastapi_tusd
+Keywords: fastapi-tusd
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development
 Classifier: Framework :: FastAPI
 Classifier: Framework :: Pydantic
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
@@ -26,36 +26,51 @@
 Provides-Extra: format
 Provides-Extra: dev
 License-File: LICENSE
 License-File: AUTHORS.md
 
 # FastAPI Server for Tus Protocol
 
-A file upload server of the tus resumable upload protocol is implemented on FastAPI framework.  
+A file upload server of the tus resumable upload protocol is implemented on **FastAPI** framework.  
+
+Thanks to [tusd](https://github.com/tus/tusd), it provides great ideas and a sensible design pattern to implement `Tus` protocol to support multiple backend storage implementations.
+
+**Features**:
+
+- [x] Basic operations to support Core Protocol such as **HEAD**, **POST**, **PATCH**, **DELETE**
+  - [x] Creation With Upload
+  - [ ] Checksum such as md5
+  - [ ] Expiration
+  - [ ] Concatenation
+- [x] File storage
+- [ ] S3 storage
+
 
 ## Getting started
 
 Import `TusRouter` to your application,
 
 ```py title=main.py
 from fastapi import FastAPI
 from fastapi_tusd import TusRouter
 
 app = FastAPI()
 
+# `store_dir`: the folder to store uploaded files
+#  `location`: the API endpoint to serve, like `http://127.0.0.1:8000/files` or relative path `files` (TODO: induced from `prefix` in default)
 app.include_router(TusRouter(store_dir="./files", location="/files"), prefix="/files")
 ```
 
 Then the tus upload endpoints will be served at `http://127.0.0.1:8000/files`, more information is available at `http://127.0.0.1:8000/docs`
 
 ### Examples
 
-There a simple example with web file upload client supporting for `Tus` protocol, thanks to `Uppy`!
+There is a simple example with a web file upload client supporting for `Tus` protocol, thanks to `Uppy`!
 
-Enter the `example/` folder, run(`pip install uvicorn` if no `uvicorn`!)
+Enter the `example/` folder, and run(`pip install `uvicorn` if no `uvicorn`!)
 
 ```sh
 uvicorn app_tusd:app --reload
 ```
 
 Then visit `https://127.0.0.1:8000/upload.thml`
```

