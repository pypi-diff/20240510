# Comparing `tmp/rest_solace-0.0.0.tar.gz` & `tmp/rest_solace-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rest_solace-0.0.0.tar", last modified: Tue May  7 16:06:07 2024, max compression
+gzip compressed data, was "rest_solace-0.0.1.tar", last modified: Fri May 10 13:01:07 2024, max compression
```

## Comparing `rest_solace-0.0.0.tar` & `rest_solace-0.0.1.tar`

### file list

```diff
@@ -1,47 +1,46 @@
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-07 16:06:07.224731 rest_solace-0.0.0/
--rw-r--r--   0 skyler    (1000) skyler    (1000)       29 2024-05-07 12:19:34.000000 rest_solace-0.0.0/.gitignore
--rw-r--r--   0 skyler    (1000) skyler    (1000)    10178 2024-05-07 08:54:03.000000 rest_solace-0.0.0/LICENSE.txt
--rw-r--r--   0 skyler    (1000) skyler    (1000)     1260 2024-05-07 11:22:11.000000 rest_solace-0.0.0/NOTICE.txt
--rw-r--r--   0 skyler    (1000) skyler    (1000)     1720 2024-05-07 16:06:07.224731 rest_solace-0.0.0/PKG-INFO
--rw-r--r--   0 skyler    (1000) skyler    (1000)      659 2024-05-07 16:04:29.000000 rest_solace-0.0.0/README.rst
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-07 16:06:07.212731 rest_solace-0.0.0/dist/
--rw-r--r--   0 skyler    (1000) skyler    (1000)    48599 2024-05-07 13:39:36.000000 rest_solace-0.0.0/dist/rest_solace-0.0.0-py3-none-any.whl
--rw-r--r--   0 skyler    (1000) skyler    (1000)   166270 2024-05-07 13:39:29.000000 rest_solace-0.0.0/dist/rest_solace-0.0.0.tar.gz
--rw-r--r--   0 skyler    (1000) skyler    (1000)     1637 2024-05-07 14:24:24.000000 rest_solace-0.0.0/pyproject.toml
--rw-r--r--   0 skyler    (1000) skyler    (1000)       38 2024-05-07 16:06:07.224731 rest_solace-0.0.0/setup.cfg
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-07 16:06:07.204731 rest_solace-0.0.0/src/
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-07 16:06:07.212731 rest_solace-0.0.0/src/rest_solace/
--rw-r--r--   0 skyler    (1000) skyler    (1000)      520 2024-04-20 20:43:31.000000 rest_solace-0.0.0/src/rest_solace/__init__.py
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-07 16:06:07.220731 rest_solace-0.0.0/src/rest_solace/__pycache__/
--rw-r--r--   0 skyler    (1000) skyler    (1000)      359 2024-04-20 20:55:30.000000 rest_solace-0.0.0/src/rest_solace/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     2040 2024-04-07 08:23:01.000000 rest_solace-0.0.0/src/rest_solace/__pycache__/action.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     2224 2024-04-07 06:29:02.000000 rest_solace-0.0.0/src/rest_solace/__pycache__/config.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     5734 2024-04-21 05:54:01.000000 rest_solace-0.0.0/src/rest_solace/__pycache__/consumer.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     4876 2024-04-22 07:47:41.000000 rest_solace-0.0.0/src/rest_solace/__pycache__/http_client.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     4128 2024-04-07 19:18:05.000000 rest_solace-0.0.0/src/rest_solace/__pycache__/manage.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)    20533 2024-04-22 10:02:53.000000 rest_solace-0.0.0/src/rest_solace/__pycache__/manager.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     1227 2024-03-31 13:04:04.000000 rest_solace-0.0.0/src/rest_solace/__pycache__/pub_sub.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     2742 2024-04-07 20:21:55.000000 rest_solace-0.0.0/src/rest_solace/__pycache__/publish.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     4538 2024-04-21 19:21:45.000000 rest_solace-0.0.0/src/rest_solace/__pycache__/publisher.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     4246 2024-04-07 18:11:44.000000 rest_solace-0.0.0/src/rest_solace/__pycache__/semp_client.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     7341 2024-03-31 19:33:25.000000 rest_solace-0.0.0/src/rest_solace/__pycache__/semp_endpoint.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     5358 2024-04-20 19:56:40.000000 rest_solace-0.0.0/src/rest_solace/__pycache__/subscriber.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     5149 2024-05-06 18:11:03.000000 rest_solace-0.0.0/src/rest_solace/consumer.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)      125 2024-05-06 18:10:17.000000 rest_solace-0.0.0/src/rest_solace/exceptions.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)     3164 2024-05-05 14:53:10.000000 rest_solace-0.0.0/src/rest_solace/http_client.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)    29947 2024-05-06 18:13:23.000000 rest_solace-0.0.0/src/rest_solace/manager.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)    14199 2024-05-05 18:58:01.000000 rest_solace-0.0.0/src/rest_solace/publisher.py
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-07 16:06:07.224731 rest_solace-0.0.0/src/rest_solace.egg-info/
--rw-r--r--   0 skyler    (1000) skyler    (1000)     1720 2024-05-07 16:06:07.000000 rest_solace-0.0.0/src/rest_solace.egg-info/PKG-INFO
--rw-r--r--   0 skyler    (1000) skyler    (1000)     1342 2024-05-07 16:06:07.000000 rest_solace-0.0.0/src/rest_solace.egg-info/SOURCES.txt
--rw-r--r--   0 skyler    (1000) skyler    (1000)        1 2024-05-07 16:06:07.000000 rest_solace-0.0.0/src/rest_solace.egg-info/dependency_links.txt
--rw-r--r--   0 skyler    (1000) skyler    (1000)       82 2024-05-07 16:06:07.000000 rest_solace-0.0.0/src/rest_solace.egg-info/requires.txt
--rw-r--r--   0 skyler    (1000) skyler    (1000)       12 2024-05-07 16:06:07.000000 rest_solace-0.0.0/src/rest_solace.egg-info/top_level.txt
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-07 16:06:07.220731 rest_solace-0.0.0/tests/
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-07 16:06:07.220731 rest_solace-0.0.0/tests/__pycache__/
--rw-r--r--   0 skyler    (1000) skyler    (1000)     1419 2024-04-21 18:34:05.000000 rest_solace-0.0.0/tests/__pycache__/manager_unittest.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)      864 2024-05-06 18:46:43.000000 rest_solace-0.0.0/tests/consumer_test.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)     2102 2024-05-06 18:46:46.000000 rest_solace-0.0.0/tests/empty_test.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)     7223 2024-05-06 18:46:48.000000 rest_solace-0.0.0/tests/manager_test.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)     2841 2024-05-06 18:46:50.000000 rest_solace-0.0.0/tests/pub_sub_test.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)      891 2024-04-28 09:19:07.000000 rest_solace-0.0.0/tests/util.py
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-10 13:01:07.224868 rest_solace-0.0.1/
+-rw-r--r--   0 skyler    (1000) skyler    (1000)       29 2024-05-07 12:19:34.000000 rest_solace-0.0.1/.gitignore
+-rw-r--r--   0 skyler    (1000) skyler    (1000)    10178 2024-05-07 08:54:03.000000 rest_solace-0.0.1/LICENSE.txt
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     1260 2024-05-07 11:22:11.000000 rest_solace-0.0.1/NOTICE.txt
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     5760 2024-05-10 13:01:07.224868 rest_solace-0.0.1/PKG-INFO
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     4684 2024-05-10 12:47:30.000000 rest_solace-0.0.1/README.rst
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-10 13:01:07.212868 rest_solace-0.0.1/docs/
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      579 2024-05-10 11:24:36.000000 rest_solace-0.0.1/docs/development_refrences.rst
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     1761 2024-05-10 12:56:38.000000 rest_solace-0.0.1/pyproject.toml
+-rw-r--r--   0 skyler    (1000) skyler    (1000)       38 2024-05-10 13:01:07.224868 rest_solace-0.0.1/setup.cfg
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-10 13:01:07.208868 rest_solace-0.0.1/src/
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-10 13:01:07.216868 rest_solace-0.0.1/src/rest_solace/
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      520 2024-04-20 20:43:31.000000 rest_solace-0.0.1/src/rest_solace/__init__.py
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-10 13:01:07.220868 rest_solace-0.0.1/src/rest_solace/__pycache__/
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      359 2024-04-20 20:55:30.000000 rest_solace-0.0.1/src/rest_solace/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     2040 2024-04-07 08:23:01.000000 rest_solace-0.0.1/src/rest_solace/__pycache__/action.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     2224 2024-04-07 06:29:02.000000 rest_solace-0.0.1/src/rest_solace/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     5734 2024-04-21 05:54:01.000000 rest_solace-0.0.1/src/rest_solace/__pycache__/consumer.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     4876 2024-04-22 07:47:41.000000 rest_solace-0.0.1/src/rest_solace/__pycache__/http_client.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     4128 2024-04-07 19:18:05.000000 rest_solace-0.0.1/src/rest_solace/__pycache__/manage.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)    20533 2024-04-22 10:02:53.000000 rest_solace-0.0.1/src/rest_solace/__pycache__/manager.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     1227 2024-03-31 13:04:04.000000 rest_solace-0.0.1/src/rest_solace/__pycache__/pub_sub.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     2742 2024-04-07 20:21:55.000000 rest_solace-0.0.1/src/rest_solace/__pycache__/publish.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     4538 2024-04-21 19:21:45.000000 rest_solace-0.0.1/src/rest_solace/__pycache__/publisher.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     4246 2024-04-07 18:11:44.000000 rest_solace-0.0.1/src/rest_solace/__pycache__/semp_client.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     7341 2024-03-31 19:33:25.000000 rest_solace-0.0.1/src/rest_solace/__pycache__/semp_endpoint.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     5358 2024-04-20 19:56:40.000000 rest_solace-0.0.1/src/rest_solace/__pycache__/subscriber.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     5149 2024-05-06 18:11:03.000000 rest_solace-0.0.1/src/rest_solace/consumer.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      125 2024-05-06 18:10:17.000000 rest_solace-0.0.1/src/rest_solace/exceptions.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     3164 2024-05-05 14:53:10.000000 rest_solace-0.0.1/src/rest_solace/http_client.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)    29947 2024-05-06 18:13:23.000000 rest_solace-0.0.1/src/rest_solace/manager.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)    14199 2024-05-05 18:58:01.000000 rest_solace-0.0.1/src/rest_solace/publisher.py
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-10 13:01:07.224868 rest_solace-0.0.1/src/rest_solace.egg-info/
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     5760 2024-05-10 13:01:07.000000 rest_solace-0.0.1/src/rest_solace.egg-info/PKG-INFO
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     1303 2024-05-10 13:01:07.000000 rest_solace-0.0.1/src/rest_solace.egg-info/SOURCES.txt
+-rw-r--r--   0 skyler    (1000) skyler    (1000)        1 2024-05-10 13:01:07.000000 rest_solace-0.0.1/src/rest_solace.egg-info/dependency_links.txt
+-rw-r--r--   0 skyler    (1000) skyler    (1000)       82 2024-05-10 13:01:07.000000 rest_solace-0.0.1/src/rest_solace.egg-info/requires.txt
+-rw-r--r--   0 skyler    (1000) skyler    (1000)       12 2024-05-10 13:01:07.000000 rest_solace-0.0.1/src/rest_solace.egg-info/top_level.txt
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-10 13:01:07.224868 rest_solace-0.0.1/tests/
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-10 13:01:07.224868 rest_solace-0.0.1/tests/__pycache__/
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     1419 2024-04-21 18:34:05.000000 rest_solace-0.0.1/tests/__pycache__/manager_unittest.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      864 2024-05-06 18:46:43.000000 rest_solace-0.0.1/tests/consumer_test.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     2102 2024-05-06 18:46:46.000000 rest_solace-0.0.1/tests/empty_test.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     7223 2024-05-06 18:46:48.000000 rest_solace-0.0.1/tests/manager_test.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     2841 2024-05-06 18:46:50.000000 rest_solace-0.0.1/tests/pub_sub_test.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      891 2024-04-28 09:19:07.000000 rest_solace-0.0.1/tests/util.py
```

### Comparing `rest_solace-0.0.0/LICENSE.txt` & `rest_solace-0.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.0/NOTICE.txt` & `rest_solace-0.0.1/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.0/pyproject.toml` & `rest_solace-0.0.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,18 @@
 ]
 maintainers = [
   {name = "Skyler Guha", email = "skylerguha@gmail.com"}
 ]
 description = "REST based library for Solace Message Broker. Publish, Consume, & Manage!!"
 readme = "README.rst"
 requires-python = ">=3.8"
-keywords = ["solace", "rest", "REST API", "rest-solace", "rest_solace", "rest solace"]
+keywords = ["solace", "rest", 
+            "REST API", "rest-solace", 
+            "rest_solace", "rest solace", 
+            "python", "pythonic"]
 license = {text = "apache 2.0"}
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Intended Audience :: Developers"
 ]
@@ -28,22 +31,25 @@
     "datetime",
     "typing",
     "queue",
     "threading",
     "json",
     "urllib"
 ]
-version = "0.0.0"
+version = "0.0.1"
 
 [project.urls]
 homepage = "https://github.com/skyler-guha/rest-solace"
 documentation = "https://github.com/skyler-guha/rest-solace"
 repository = "https://github.com/skyler-guha/rest-solace"
 
-#Test Build command: python -m twine upload --repository testpypi dist/* --verbose
+#Build command: python -m build
+#check release: twine check dist/*
+#push release: twine upload dist/*
+#(update version number before new release)
 
 # ... other project metadata fields and resources:
 #   
 #   List of clasifiers: https://pypi.org/classifiers/
 #   packaging guide: https://www.serviceobjects.com/blog/step-by-step-guide-to-publishing-python-libraries-to-pypi/ 
 #   https://packaging.python.org/en/latest/guides/writing-pyproject-toml/
 #   https://packaging.python.org/en/latest/guides/writing-pyproject-toml/
```

### Comparing `rest_solace-0.0.0/src/rest_solace/__init__.py` & `rest_solace-0.0.1/src/rest_solace/__init__.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.0/src/rest_solace/__pycache__/action.cpython-311.pyc` & `rest_solace-0.0.1/src/rest_solace/__pycache__/action.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.0/src/rest_solace/__pycache__/config.cpython-311.pyc` & `rest_solace-0.0.1/src/rest_solace/__pycache__/config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.0/src/rest_solace/__pycache__/consumer.cpython-311.pyc` & `rest_solace-0.0.1/src/rest_solace/__pycache__/consumer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.0/src/rest_solace/__pycache__/http_client.cpython-311.pyc` & `rest_solace-0.0.1/src/rest_solace/__pycache__/http_client.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.0/src/rest_solace/__pycache__/manage.cpython-311.pyc` & `rest_solace-0.0.1/src/rest_solace/__pycache__/manage.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.0/src/rest_solace/__pycache__/manager.cpython-311.pyc` & `rest_solace-0.0.1/src/rest_solace/__pycache__/manager.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.0/src/rest_solace/__pycache__/pub_sub.cpython-311.pyc` & `rest_solace-0.0.1/src/rest_solace/__pycache__/pub_sub.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.0/src/rest_solace/__pycache__/publish.cpython-311.pyc` & `rest_solace-0.0.1/src/rest_solace/__pycache__/publish.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.0/src/rest_solace/__pycache__/publisher.cpython-311.pyc` & `rest_solace-0.0.1/src/rest_solace/__pycache__/publisher.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.0/src/rest_solace/__pycache__/semp_client.cpython-311.pyc` & `rest_solace-0.0.1/src/rest_solace/__pycache__/semp_client.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.0/src/rest_solace/__pycache__/semp_endpoint.cpython-311.pyc` & `rest_solace-0.0.1/src/rest_solace/__pycache__/semp_endpoint.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.0/src/rest_solace/__pycache__/subscriber.cpython-311.pyc` & `rest_solace-0.0.1/src/rest_solace/__pycache__/subscriber.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.0/src/rest_solace/consumer.py` & `rest_solace-0.0.1/src/rest_solace/consumer.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.0/src/rest_solace/http_client.py` & `rest_solace-0.0.1/src/rest_solace/http_client.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.0/src/rest_solace/manager.py` & `rest_solace-0.0.1/src/rest_solace/manager.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.0/src/rest_solace/publisher.py` & `rest_solace-0.0.1/src/rest_solace/publisher.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.0/src/rest_solace.egg-info/SOURCES.txt` & `rest_solace-0.0.1/src/rest_solace.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 .gitignore
 LICENSE.txt
 NOTICE.txt
 README.rst
 pyproject.toml
-dist/rest_solace-0.0.0-py3-none-any.whl
-dist/rest_solace-0.0.0.tar.gz
+docs/development_refrences.rst
 src/rest_solace/__init__.py
 src/rest_solace/consumer.py
 src/rest_solace/exceptions.py
 src/rest_solace/http_client.py
 src/rest_solace/manager.py
 src/rest_solace/publisher.py
 src/rest_solace.egg-info/PKG-INFO
```

### Comparing `rest_solace-0.0.0/tests/__pycache__/manager_unittest.cpython-311.pyc` & `rest_solace-0.0.1/tests/__pycache__/manager_unittest.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.0/tests/consumer_test.py` & `rest_solace-0.0.1/tests/consumer_test.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.0/tests/empty_test.py` & `rest_solace-0.0.1/tests/empty_test.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.0/tests/manager_test.py` & `rest_solace-0.0.1/tests/manager_test.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.0/tests/pub_sub_test.py` & `rest_solace-0.0.1/tests/pub_sub_test.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.0.0/tests/util.py` & `rest_solace-0.0.1/tests/util.py`

 * *Files identical despite different names*

