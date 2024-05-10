# Comparing `tmp/acctf-0.4.2.tar.gz` & `tmp/acctf-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acctf-0.4.2.tar", last modified: Tue May  7 10:06:15 2024, max compression
+gzip compressed data, was "acctf-0.4.3.tar", last modified: Fri May 10 06:40:38 2024, max compression
```

## Comparing `acctf-0.4.2.tar` & `acctf-0.4.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-05-07 10:06:15.075126 acctf-0.4.2/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     1071 2024-02-11 09:23:25.000000 acctf-0.4.2/LICENSE
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     4667 2024-05-07 10:06:15.075126 acctf-0.4.2/PKG-INFO
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     4021 2024-04-13 14:09:09.000000 acctf-0.4.2/README.md
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-05-07 10:06:15.065126 acctf-0.4.2/acctf/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     2671 2024-04-20 09:28:03.000000 acctf-0.4.2/acctf/__init__.py
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-05-07 10:06:15.065126 acctf-0.4.2/acctf/bank/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      729 2024-04-20 09:28:03.000000 acctf-0.4.2/acctf/bank/__init__.py
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-05-07 10:06:15.065126 acctf-0.4.2/acctf/bank/mizuho/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     6328 2024-05-07 10:04:27.000000 acctf-0.4.2/acctf/bank/mizuho/__init__.py
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     1492 2024-03-17 12:13:43.000000 acctf-0.4.2/acctf/bank/model.py
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-05-07 10:06:15.065126 acctf-0.4.2/acctf/bank/sbi/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     9029 2024-05-07 10:04:27.000000 acctf-0.4.2/acctf/bank/sbi/__init__.py
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-05-07 10:06:15.065126 acctf-0.4.2/acctf/other/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)        0 2024-02-11 09:23:25.000000 acctf-0.4.2/acctf/other/__init__.py
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-05-07 10:06:15.065126 acctf-0.4.2/acctf/other/wealthnavi/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     2251 2024-05-07 10:04:27.000000 acctf-0.4.2/acctf/other/wealthnavi/__init__.py
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      216 2024-02-11 09:23:25.000000 acctf-0.4.2/acctf/other/wealthnavi/model.py
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-05-07 10:06:15.075126 acctf-0.4.2/acctf/securities/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      848 2024-04-20 09:28:03.000000 acctf-0.4.2/acctf/securities/__init__.py
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      346 2024-02-11 09:23:25.000000 acctf-0.4.2/acctf/securities/model.py
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-05-07 10:06:15.075126 acctf-0.4.2/acctf/securities/sbi/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     4131 2024-04-20 14:52:07.000000 acctf-0.4.2/acctf/securities/sbi/__init__.py
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      747 2024-02-11 09:23:25.000000 acctf-0.4.2/acctf/securities/sbi/utils.py
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-05-07 10:06:15.075126 acctf-0.4.2/acctf/utils/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)        0 2024-02-11 09:23:25.000000 acctf-0.4.2/acctf/utils/__init__.py
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      105 2024-03-17 12:13:43.000000 acctf-0.4.2/acctf/utils/format.py
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)       80 2024-04-06 13:38:11.000000 acctf-0.4.2/acctf/utils/totp.py
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-05-07 10:06:15.075126 acctf-0.4.2/acctf.egg-info/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     4667 2024-05-07 10:06:14.000000 acctf-0.4.2/acctf.egg-info/PKG-INFO
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      573 2024-05-07 10:06:14.000000 acctf-0.4.2/acctf.egg-info/SOURCES.txt
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)        1 2024-05-07 10:06:14.000000 acctf-0.4.2/acctf.egg-info/dependency_links.txt
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)       63 2024-05-07 10:06:14.000000 acctf-0.4.2/acctf.egg-info/requires.txt
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)        6 2024-05-07 10:06:14.000000 acctf-0.4.2/acctf.egg-info/top_level.txt
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)       74 2024-05-07 10:06:15.075126 acctf-0.4.2/setup.cfg
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      929 2024-05-07 10:04:27.000000 acctf-0.4.2/setup.py
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-05-10 06:40:38.206369 acctf-0.4.3/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     1071 2024-02-11 09:23:25.000000 acctf-0.4.3/LICENSE
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     4667 2024-05-10 06:40:38.206369 acctf-0.4.3/PKG-INFO
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     4021 2024-04-13 14:09:09.000000 acctf-0.4.3/README.md
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-05-10 06:40:38.196368 acctf-0.4.3/acctf/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     2671 2024-04-20 09:28:03.000000 acctf-0.4.3/acctf/__init__.py
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-05-10 06:40:38.196368 acctf-0.4.3/acctf/bank/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      729 2024-04-20 09:28:03.000000 acctf-0.4.3/acctf/bank/__init__.py
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-05-10 06:40:38.196368 acctf-0.4.3/acctf/bank/mizuho/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     6328 2024-05-07 10:04:27.000000 acctf-0.4.3/acctf/bank/mizuho/__init__.py
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     1492 2024-03-17 12:13:43.000000 acctf-0.4.3/acctf/bank/model.py
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-05-10 06:40:38.206369 acctf-0.4.3/acctf/bank/sbi/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     9089 2024-05-10 06:39:04.000000 acctf-0.4.3/acctf/bank/sbi/__init__.py
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-05-10 06:40:38.206369 acctf-0.4.3/acctf/other/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)        0 2024-02-11 09:23:25.000000 acctf-0.4.3/acctf/other/__init__.py
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-05-10 06:40:38.206369 acctf-0.4.3/acctf/other/wealthnavi/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     2251 2024-05-07 10:04:27.000000 acctf-0.4.3/acctf/other/wealthnavi/__init__.py
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      216 2024-02-11 09:23:25.000000 acctf-0.4.3/acctf/other/wealthnavi/model.py
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-05-10 06:40:38.206369 acctf-0.4.3/acctf/securities/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      848 2024-04-20 09:28:03.000000 acctf-0.4.3/acctf/securities/__init__.py
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      346 2024-02-11 09:23:25.000000 acctf-0.4.3/acctf/securities/model.py
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-05-10 06:40:38.206369 acctf-0.4.3/acctf/securities/sbi/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     4131 2024-04-20 14:52:07.000000 acctf-0.4.3/acctf/securities/sbi/__init__.py
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      747 2024-02-11 09:23:25.000000 acctf-0.4.3/acctf/securities/sbi/utils.py
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-05-10 06:40:38.206369 acctf-0.4.3/acctf/utils/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)        0 2024-02-11 09:23:25.000000 acctf-0.4.3/acctf/utils/__init__.py
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      105 2024-03-17 12:13:43.000000 acctf-0.4.3/acctf/utils/format.py
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)       80 2024-04-06 13:38:11.000000 acctf-0.4.3/acctf/utils/totp.py
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-05-10 06:40:38.206369 acctf-0.4.3/acctf.egg-info/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     4667 2024-05-10 06:40:38.000000 acctf-0.4.3/acctf.egg-info/PKG-INFO
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      573 2024-05-10 06:40:38.000000 acctf-0.4.3/acctf.egg-info/SOURCES.txt
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)        1 2024-05-10 06:40:38.000000 acctf-0.4.3/acctf.egg-info/dependency_links.txt
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)       63 2024-05-10 06:40:38.000000 acctf-0.4.3/acctf.egg-info/requires.txt
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)        6 2024-05-10 06:40:38.000000 acctf-0.4.3/acctf.egg-info/top_level.txt
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)       74 2024-05-10 06:40:38.206369 acctf-0.4.3/setup.cfg
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      929 2024-05-10 06:39:04.000000 acctf-0.4.3/setup.py
```

### Comparing `acctf-0.4.2/LICENSE` & `acctf-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `acctf-0.4.2/PKG-INFO` & `acctf-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acctf
-Version: 0.4.2
+Version: 0.4.3
 Summary: library that scrapes the data from an account such as securities, bank
 Home-page: https://github.com/hirano00o/acctf
 Author: hirano00o
 Keywords: scrape,account,development
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `acctf-0.4.2/README.md` & `acctf-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `acctf-0.4.2/acctf/__init__.py` & `acctf-0.4.3/acctf/__init__.py`

 * *Files identical despite different names*

### Comparing `acctf-0.4.2/acctf/bank/__init__.py` & `acctf-0.4.3/acctf/bank/__init__.py`

 * *Files identical despite different names*

### Comparing `acctf-0.4.2/acctf/bank/mizuho/__init__.py` & `acctf-0.4.3/acctf/bank/mizuho/__init__.py`

 * *Files identical despite different names*

### Comparing `acctf-0.4.2/acctf/bank/model.py` & `acctf-0.4.3/acctf/bank/model.py`

 * *Files identical despite different names*

### Comparing `acctf-0.4.2/acctf/bank/sbi/__init__.py` & `acctf-0.4.3/acctf/bank/sbi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,16 @@
         :param start: start date of transaction history. After the 1st of the month before the previous month.
         :param end: end date of transaction history. Until today.
         :param currency: currency of transaction history.
         """
         if account_number != "" and account_number is not None:
             self.account_number = account_number
 
+        self.wait_loading(By.CLASS_NAME, "loading-Server")
+
         details = 'm-icon-ps_details'
         elem = self.find_element_to_be_clickable(By.CLASS_NAME, details)
         elem.click()
 
         self.wait_loading(By.CLASS_NAME, "loadingServer")
 
         # 代表口座
```

### Comparing `acctf-0.4.2/acctf/other/wealthnavi/__init__.py` & `acctf-0.4.3/acctf/other/wealthnavi/__init__.py`

 * *Files identical despite different names*

### Comparing `acctf-0.4.2/acctf/securities/__init__.py` & `acctf-0.4.3/acctf/securities/__init__.py`

 * *Files identical despite different names*

### Comparing `acctf-0.4.2/acctf/securities/sbi/__init__.py` & `acctf-0.4.3/acctf/securities/sbi/__init__.py`

 * *Files identical despite different names*

### Comparing `acctf-0.4.2/acctf/securities/sbi/utils.py` & `acctf-0.4.3/acctf/securities/sbi/utils.py`

 * *Files identical despite different names*

### Comparing `acctf-0.4.2/acctf.egg-info/PKG-INFO` & `acctf-0.4.3/acctf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acctf
-Version: 0.4.2
+Version: 0.4.3
 Summary: library that scrapes the data from an account such as securities, bank
 Home-page: https://github.com/hirano00o/acctf
 Author: hirano00o
 Keywords: scrape,account,development
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `acctf-0.4.2/acctf.egg-info/SOURCES.txt` & `acctf-0.4.3/acctf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acctf-0.4.2/setup.py` & `acctf-0.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="acctf",
-    version="0.4.2",
+    version="0.4.3",
     description="library that scrapes the data from an account such as securities, bank",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hirano00o/acctf",
     author="hirano00o",
     classifiers=[
         "Programming Language :: Python :: 3",
```

