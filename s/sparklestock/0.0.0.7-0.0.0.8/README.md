# Comparing `tmp/sparklestock-0.0.0.7.tar.gz` & `tmp/sparklestock-0.0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparklestock-0.0.0.7.tar", last modified: Thu May  9 02:24:10 2024, max compression
+gzip compressed data, was "sparklestock-0.0.0.8.tar", last modified: Thu May  9 07:59:02 2024, max compression
```

## Comparing `sparklestock-0.0.0.7.tar` & `sparklestock-0.0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 seyong     (501) staff       (20)        0 2024-05-09 02:24:10.715556 sparklestock-0.0.0.7/
--rw-r--r--   0 seyong     (501) staff       (20)      462 2024-05-09 02:24:10.715482 sparklestock-0.0.0.7/PKG-INFO
--rw-r--r--   0 seyong     (501) staff       (20)       45 2024-05-09 01:53:19.000000 sparklestock-0.0.0.7/README.md
--rw-r--r--   0 seyong     (501) staff       (20)      270 2024-04-05 11:07:26.000000 sparklestock-0.0.0.7/pyproject.toml
--rw-r--r--   0 seyong     (501) staff       (20)       79 2024-05-09 02:24:10.715863 sparklestock-0.0.0.7/setup.cfg
--rw-r--r--   0 seyong     (501) staff       (20)      720 2024-05-09 02:23:54.000000 sparklestock-0.0.0.7/setup.py
-drwxr-xr-x   0 seyong     (501) staff       (20)        0 2024-05-09 02:24:10.714160 sparklestock-0.0.0.7/sparklestock/
--rw-r--r--   0 seyong     (501) staff       (20)     2300 2024-05-09 02:23:54.000000 sparklestock-0.0.0.7/sparklestock/Stock.py
--rw-r--r--   0 seyong     (501) staff       (20)       58 2024-05-08 13:55:13.000000 sparklestock-0.0.0.7/sparklestock/__init__.py
--rw-r--r--   0 seyong     (501) staff       (20)       23 2024-05-09 02:23:54.000000 sparklestock-0.0.0.7/sparklestock/__version__.py
-drwxr-xr-x   0 seyong     (501) staff       (20)        0 2024-05-09 02:24:10.715247 sparklestock-0.0.0.7/sparklestock.egg-info/
--rw-r--r--   0 seyong     (501) staff       (20)      462 2024-05-09 02:24:10.000000 sparklestock-0.0.0.7/sparklestock.egg-info/PKG-INFO
--rw-r--r--   0 seyong     (501) staff       (20)      297 2024-05-09 02:24:10.000000 sparklestock-0.0.0.7/sparklestock.egg-info/SOURCES.txt
--rw-r--r--   0 seyong     (501) staff       (20)        1 2024-05-09 02:24:10.000000 sparklestock-0.0.0.7/sparklestock.egg-info/dependency_links.txt
--rw-r--r--   0 seyong     (501) staff       (20)        9 2024-05-09 02:24:10.000000 sparklestock-0.0.0.7/sparklestock.egg-info/requires.txt
--rw-r--r--   0 seyong     (501) staff       (20)       13 2024-05-09 02:24:10.000000 sparklestock-0.0.0.7/sparklestock.egg-info/top_level.txt
+drwxr-xr-x   0 seyong     (501) staff       (20)        0 2024-05-09 07:59:02.510781 sparklestock-0.0.0.8/
+-rw-r--r--   0 seyong     (501) staff       (20)      462 2024-05-09 07:59:02.510711 sparklestock-0.0.0.8/PKG-INFO
+-rw-r--r--   0 seyong     (501) staff       (20)       45 2024-05-09 01:53:19.000000 sparklestock-0.0.0.8/README.md
+-rw-r--r--   0 seyong     (501) staff       (20)      270 2024-04-05 11:07:26.000000 sparklestock-0.0.0.8/pyproject.toml
+-rw-r--r--   0 seyong     (501) staff       (20)       79 2024-05-09 07:59:02.511219 sparklestock-0.0.0.8/setup.cfg
+-rw-r--r--   0 seyong     (501) staff       (20)      720 2024-05-09 07:58:59.000000 sparklestock-0.0.0.8/setup.py
+drwxr-xr-x   0 seyong     (501) staff       (20)        0 2024-05-09 07:59:02.509587 sparklestock-0.0.0.8/sparklestock/
+-rw-r--r--   0 seyong     (501) staff       (20)     2310 2024-05-09 07:58:50.000000 sparklestock-0.0.0.8/sparklestock/Stock.py
+-rw-r--r--   0 seyong     (501) staff       (20)       58 2024-05-08 13:55:13.000000 sparklestock-0.0.0.8/sparklestock/__init__.py
+-rw-r--r--   0 seyong     (501) staff       (20)       23 2024-05-09 07:58:59.000000 sparklestock-0.0.0.8/sparklestock/__version__.py
+drwxr-xr-x   0 seyong     (501) staff       (20)        0 2024-05-09 07:59:02.510474 sparklestock-0.0.0.8/sparklestock.egg-info/
+-rw-r--r--   0 seyong     (501) staff       (20)      462 2024-05-09 07:59:02.000000 sparklestock-0.0.0.8/sparklestock.egg-info/PKG-INFO
+-rw-r--r--   0 seyong     (501) staff       (20)      297 2024-05-09 07:59:02.000000 sparklestock-0.0.0.8/sparklestock.egg-info/SOURCES.txt
+-rw-r--r--   0 seyong     (501) staff       (20)        1 2024-05-09 07:59:02.000000 sparklestock-0.0.0.8/sparklestock.egg-info/dependency_links.txt
+-rw-r--r--   0 seyong     (501) staff       (20)        9 2024-05-09 07:59:02.000000 sparklestock-0.0.0.8/sparklestock.egg-info/requires.txt
+-rw-r--r--   0 seyong     (501) staff       (20)       13 2024-05-09 07:59:02.000000 sparklestock-0.0.0.8/sparklestock.egg-info/top_level.txt
```

### Comparing `sparklestock-0.0.0.7/setup.py` & `sparklestock-0.0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sparklestock", ## 소문자 영단어
-    version="0.0.0.7", ##
+    version="0.0.0.8", ##
     author="Seyong Ahn", ## ex) Sunkyeong Lee
     author_email="hiseyong1008@gmail.com", ##
     description="sparkle stock package", ##
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hiseyong", ##
     install_requires=['requests'],
```

### Comparing `sparklestock-0.0.0.7/sparklestock/Stock.py` & `sparklestock-0.0.0.8/sparklestock/Stock.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,25 +40,25 @@
         self.history = eval(price_history)
         return self.history
 
 
     def buy_stock(self, amount:int):
         self.check_login()
 
-        buying_status = post(self.address+'/api/buy', json={'id':self.id, 'pw':self.pw, 'amount':str(amount)}).text
+        buying_status = post(self.address+'/api/buy', json={'id':self.id, 'pw':self.pw, 'amount':str(int(amount))}).text
         if buying_status == 'true':
             print("매수에 성공했습니다.")
         else:
             raise ConnectionError(buying_status)
 
 
     def sell_stock(self, amount:int):
         self.check_login()
 
-        selling_status = post(self.address+'/api/sell', json={'id':self.id, 'pw':self.pw, 'amount':str(amount)}).text
+        selling_status = post(self.address+'/api/sell', json={'id':self.id, 'pw':self.pw, 'amount':str(int(amount))}).text
         if selling_status == 'true':
             print("매도에 성공했습니다.")
         else:
             raise ConnectionError(selling_status)
 
 
     def check_my_asset(self):
```

