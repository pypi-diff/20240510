# Comparing `tmp/sparklestock-0.0.0.9.tar.gz` & `tmp/sparklestock-0.0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparklestock-0.0.0.9.tar", last modified: Fri May 10 03:58:27 2024, max compression
+gzip compressed data, was "sparklestock-0.0.1.0.tar", last modified: Fri May 10 04:01:36 2024, max compression
```

## Comparing `sparklestock-0.0.0.9.tar` & `sparklestock-0.0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 seyong     (501) staff       (20)        0 2024-05-10 03:58:27.172683 sparklestock-0.0.0.9/
--rw-r--r--   0 seyong     (501) staff       (20)      462 2024-05-10 03:58:27.172603 sparklestock-0.0.0.9/PKG-INFO
--rw-r--r--   0 seyong     (501) staff       (20)       45 2024-05-09 01:53:19.000000 sparklestock-0.0.0.9/README.md
--rw-r--r--   0 seyong     (501) staff       (20)      270 2024-04-05 11:07:26.000000 sparklestock-0.0.0.9/pyproject.toml
--rw-r--r--   0 seyong     (501) staff       (20)       79 2024-05-10 03:58:27.173042 sparklestock-0.0.0.9/setup.cfg
--rw-r--r--   0 seyong     (501) staff       (20)      720 2024-05-10 03:58:12.000000 sparklestock-0.0.0.9/setup.py
-drwxr-xr-x   0 seyong     (501) staff       (20)        0 2024-05-10 03:58:27.171296 sparklestock-0.0.0.9/sparklestock/
--rw-r--r--   0 seyong     (501) staff       (20)     2294 2024-05-10 03:58:06.000000 sparklestock-0.0.0.9/sparklestock/Stock.py
--rw-r--r--   0 seyong     (501) staff       (20)       58 2024-05-08 13:55:13.000000 sparklestock-0.0.0.9/sparklestock/__init__.py
--rw-r--r--   0 seyong     (501) staff       (20)       23 2024-05-10 03:58:12.000000 sparklestock-0.0.0.9/sparklestock/__version__.py
-drwxr-xr-x   0 seyong     (501) staff       (20)        0 2024-05-10 03:58:27.172335 sparklestock-0.0.0.9/sparklestock.egg-info/
--rw-r--r--   0 seyong     (501) staff       (20)      462 2024-05-10 03:58:27.000000 sparklestock-0.0.0.9/sparklestock.egg-info/PKG-INFO
--rw-r--r--   0 seyong     (501) staff       (20)      297 2024-05-10 03:58:27.000000 sparklestock-0.0.0.9/sparklestock.egg-info/SOURCES.txt
--rw-r--r--   0 seyong     (501) staff       (20)        1 2024-05-10 03:58:27.000000 sparklestock-0.0.0.9/sparklestock.egg-info/dependency_links.txt
--rw-r--r--   0 seyong     (501) staff       (20)        9 2024-05-10 03:58:27.000000 sparklestock-0.0.0.9/sparklestock.egg-info/requires.txt
--rw-r--r--   0 seyong     (501) staff       (20)       13 2024-05-10 03:58:27.000000 sparklestock-0.0.0.9/sparklestock.egg-info/top_level.txt
+drwxr-xr-x   0 seyong     (501) staff       (20)        0 2024-05-10 04:01:36.342685 sparklestock-0.0.1.0/
+-rw-r--r--   0 seyong     (501) staff       (20)      462 2024-05-10 04:01:36.342612 sparklestock-0.0.1.0/PKG-INFO
+-rw-r--r--   0 seyong     (501) staff       (20)       45 2024-05-09 01:53:19.000000 sparklestock-0.0.1.0/README.md
+-rw-r--r--   0 seyong     (501) staff       (20)      270 2024-04-05 11:07:26.000000 sparklestock-0.0.1.0/pyproject.toml
+-rw-r--r--   0 seyong     (501) staff       (20)       79 2024-05-10 04:01:36.342966 sparklestock-0.0.1.0/setup.cfg
+-rw-r--r--   0 seyong     (501) staff       (20)      720 2024-05-10 04:01:32.000000 sparklestock-0.0.1.0/setup.py
+drwxr-xr-x   0 seyong     (501) staff       (20)        0 2024-05-10 04:01:36.341485 sparklestock-0.0.1.0/sparklestock/
+-rw-r--r--   0 seyong     (501) staff       (20)     2509 2024-05-10 04:01:21.000000 sparklestock-0.0.1.0/sparklestock/Stock.py
+-rw-r--r--   0 seyong     (501) staff       (20)       58 2024-05-08 13:55:13.000000 sparklestock-0.0.1.0/sparklestock/__init__.py
+-rw-r--r--   0 seyong     (501) staff       (20)       23 2024-05-10 04:01:32.000000 sparklestock-0.0.1.0/sparklestock/__version__.py
+drwxr-xr-x   0 seyong     (501) staff       (20)        0 2024-05-10 04:01:36.342377 sparklestock-0.0.1.0/sparklestock.egg-info/
+-rw-r--r--   0 seyong     (501) staff       (20)      462 2024-05-10 04:01:36.000000 sparklestock-0.0.1.0/sparklestock.egg-info/PKG-INFO
+-rw-r--r--   0 seyong     (501) staff       (20)      297 2024-05-10 04:01:36.000000 sparklestock-0.0.1.0/sparklestock.egg-info/SOURCES.txt
+-rw-r--r--   0 seyong     (501) staff       (20)        1 2024-05-10 04:01:36.000000 sparklestock-0.0.1.0/sparklestock.egg-info/dependency_links.txt
+-rw-r--r--   0 seyong     (501) staff       (20)        9 2024-05-10 04:01:36.000000 sparklestock-0.0.1.0/sparklestock.egg-info/requires.txt
+-rw-r--r--   0 seyong     (501) staff       (20)       13 2024-05-10 04:01:36.000000 sparklestock-0.0.1.0/sparklestock.egg-info/top_level.txt
```

### Comparing `sparklestock-0.0.0.9/setup.py` & `sparklestock-0.0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sparklestock", ## 소문자 영단어
-    version="0.0.0.9", ##
+    version="0.0.1.0", ##
     author="Seyong Ahn", ## ex) Sunkyeong Lee
     author_email="hiseyong1008@gmail.com", ##
     description="sparkle stock package", ##
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hiseyong", ##
     install_requires=['requests'],
```

### Comparing `sparklestock-0.0.0.9/sparklestock/Stock.py` & `sparklestock-0.0.1.0/sparklestock/Stock.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,16 +21,21 @@
             self.is_logged = True
         else:
             raise ValueError("비밀번호가 틀렸습니다.")
 
 
     def get_current_price(self) -> float:
         self.check_login()
-
-        response = get(self.address+'/api/getprice').text
+        while True:
+            try:
+                response = get(self.address + '/api/getprice').text
+                break
+            except:
+                print("가격을 불러오는 중 에러가 발생했습니다. 재시도합니다.")
+                continue
         if response == '"close"':
             print("폐장되었습니다.")
         self.price = float(response)
         return self.price
 
 
     def get_price_history(self) -> list:
```

