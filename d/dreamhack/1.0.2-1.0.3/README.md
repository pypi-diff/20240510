# Comparing `tmp/dreamhack-1.0.2.tar.gz` & `tmp/dreamhack-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreamhack-1.0.2.tar", last modified: Thu May  9 17:10:03 2024, max compression
+gzip compressed data, was "dreamhack-1.0.3.tar", last modified: Thu May  9 21:18:45 2024, max compression
```

## Comparing `dreamhack-1.0.2.tar` & `dreamhack-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-09 17:10:03.105242 dreamhack-1.0.2/
--rw-r--r--   0 runner    (1000) runner    (1000)      904 2024-05-09 17:10:03.105242 dreamhack-1.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-09 17:10:03.097242 dreamhack-1.0.2/dreamhack/
--rw-r--r--   0 runner    (1000) runner    (1000)      506 2024-05-09 17:00:39.000000 dreamhack-1.0.2/dreamhack/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      865 2024-05-09 14:39:14.000000 dreamhack-1.0.2/dreamhack/colorcodes.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2599 2024-05-09 16:57:17.000000 dreamhack-1.0.2/dreamhack/encryption.py
--rw-r--r--   0 runner    (1000) runner    (1000)       23 2024-05-09 14:39:58.000000 dreamhack-1.0.2/dreamhack/logging.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1243 2024-05-09 17:07:51.000000 dreamhack-1.0.2/dreamhack/networking.py
--rw-r--r--   0 runner    (1000) runner    (1000)      923 2024-05-09 13:41:32.000000 dreamhack-1.0.2/dreamhack/windows.py
--rw-r--r--   0 runner    (1000) runner    (1000)      892 2024-05-09 14:50:05.000000 dreamhack-1.0.2/dreamhack/zipfiles.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-09 17:10:03.105242 dreamhack-1.0.2/dreamhack.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      904 2024-05-09 17:10:02.000000 dreamhack-1.0.2/dreamhack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      330 2024-05-09 17:10:02.000000 dreamhack-1.0.2/dreamhack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-09 17:10:02.000000 dreamhack-1.0.2/dreamhack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       44 2024-05-09 17:10:02.000000 dreamhack-1.0.2/dreamhack.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       10 2024-05-09 17:10:02.000000 dreamhack-1.0.2/dreamhack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-09 17:10:03.105242 dreamhack-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)     1184 2024-05-09 17:09:45.000000 dreamhack-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-09 21:18:45.127898 dreamhack-1.0.3/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1400 2024-05-09 21:18:45.127898 dreamhack-1.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-09 21:18:45.123898 dreamhack-1.0.3/dreamhack/
+-rw-r--r--   0 runner    (1000) runner    (1000)      805 2024-05-09 21:06:53.000000 dreamhack-1.0.3/dreamhack/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      865 2024-05-09 14:39:14.000000 dreamhack-1.0.3/dreamhack/colorcodes.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1007 2024-05-09 20:31:28.000000 dreamhack-1.0.3/dreamhack/downloads.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2460 2024-05-09 20:51:18.000000 dreamhack-1.0.3/dreamhack/encryption.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      350 2024-05-09 20:40:34.000000 dreamhack-1.0.3/dreamhack/filepaths.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      695 2024-05-09 21:01:14.000000 dreamhack-1.0.3/dreamhack/gui.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1414 2024-05-09 18:30:04.000000 dreamhack-1.0.3/dreamhack/logging.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1446 2024-05-09 18:41:27.000000 dreamhack-1.0.3/dreamhack/networking.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      594 2024-05-09 18:46:07.000000 dreamhack-1.0.3/dreamhack/randoms.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3483 2024-05-09 21:08:32.000000 dreamhack-1.0.3/dreamhack/windows.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1596 2024-05-09 21:12:36.000000 dreamhack-1.0.3/dreamhack/zipfiles.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-09 21:18:45.127898 dreamhack-1.0.3/dreamhack.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1400 2024-05-09 21:18:44.000000 dreamhack-1.0.3/dreamhack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      414 2024-05-09 21:18:44.000000 dreamhack-1.0.3/dreamhack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-09 21:18:44.000000 dreamhack-1.0.3/dreamhack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      101 2024-05-09 21:18:44.000000 dreamhack-1.0.3/dreamhack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       10 2024-05-09 21:18:44.000000 dreamhack-1.0.3/dreamhack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-09 21:18:45.127898 dreamhack-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)     1626 2024-05-09 21:06:25.000000 dreamhack-1.0.3/setup.py
```

### Comparing `dreamhack-1.0.2/PKG-INFO` & `dreamhack-1.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,59 @@
 Metadata-Version: 2.1
 Name: dreamhack
-Version: 1.0.2
+Version: 1.0.3
 Summary: The ultimate PyPi package for cyber-security and many other things.
 Author: Jack Burr
 Author-email: BurrJ22@Outlook.com
 Keywords: python,windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Dist: cryptography
 Requires-Dist: tqdm
 Requires-Dist: setuptools
 Requires-Dist: pyuac
 Requires-Dist: requests
+Requires-Dist: public-ip
+Requires-Dist: keyboard
+Requires-Dist: pyautogui
+Requires-Dist: customtkinter
+Requires-Dist: CTkMessagebox
 
 The ultimate PyPi package for cyber-security, encryption, and many other things to simplify your code and make more advanced programs.
 
+*DISCLAIMER* I am not responsible for any damages caused by this package. Please do not use any features of this package for any bad purposes.
+
 RELEASE NOTES: 
 
+v1.0.3: 
+
+- Added logging content 
+
+- Added the ability to get the public ip of the current machine 
+
+- Added lots of new features 
+
+- A few bug fixes
+
 v1.0.2: 
 
 - First official stable version, DO NOT USE PREVIOUS VERSIONS 
 
 - Added content to encryption and logging 
 
 - Created networking 
 
 
+
+WARNING: VERSIONS BELOW THIS NOTE ARE UNSTABLE. DO NOT USE THEM.
+
+
 v1.0.1: 
 
-- Fixed critical error from v1.0.1 
+- Fixed critical error from v1.0.0 
 
 - Working on new version 
 
 
 v1.0.0: 
 
 - Initial release
```

### Comparing `dreamhack-1.0.2/dreamhack/colorcodes.py` & `dreamhack-1.0.3/dreamhack/colorcodes.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.0.2/dreamhack/encryption.py` & `dreamhack-1.0.3/dreamhack/encryption.py`

 * *Files 18% similar despite different names*

```diff
@@ -44,25 +44,19 @@
     except Exception as e:
       return -2, e
     else:  
       return 1
       
   def encrypt_folder(directory, key, folders_to_exclude = []):
     import os
-    def get_all_files_in_directory(directory):
-      try:
-        return os.listdir(directory)
-      except PermissionError as pe:  
-        return [], pe 
-      except Exception as e:
-        return [], e
-        
+    from .filepaths import filepaths as fp
+    #type:ignore
     if folders_to_exclude is not None and directory in folders_to_exclude:
       return
-    dirlist = get_all_files_in_directory(directory)
+    dirlist = fp.get_all_files_in_directory(directory) #type:ignore
     for file in dirlist:
       file = os.path.join(str(directory), str(file))
       if os.path.isfile(file):
         encryption.encrypt(file, key) #type:ignore
       else:
         encryption.encrypt_folder(file, key) #type:ignore
```

### Comparing `dreamhack-1.0.2/dreamhack/networking.py` & `dreamhack-1.0.3/dreamhack/networking.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 class networking():
+  def ping(ip): #type:ignore
+    import os
+    return os.system(f'ping {ip}') #type:ignore
+  
+  def get_public_ip(): #type:ignore
+    import public_ip as ip #type:ignore
+    return ip.get()
   
   def get_private_ip_address(): #type:ignore
     import socket
     return socket.gethostbyname(socket.gethostname())
 
-  def stop_wifi_network():
+  def stop_wifi_network(): #type:ignore
     import subprocess
     try:
         # Stop the hosted network
         subprocess.run(['netsh', 'wlan', 'stop', 'hostednetwork'], check=True)
     except subprocess.CalledProcessError as ex:
       raise ex
     except Exception as e:
```

### Comparing `dreamhack-1.0.2/dreamhack/zipfiles.py` & `dreamhack-1.0.3/dreamhack/zipfiles.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,27 @@
 class zipfiles():
+  def extract(zip_path, target_folder, pwd=None): #type:ignore
+    from zipfile import ZipFile
+    if pwd is None:
+        try:
+            with ZipFile(zip_path) as zf: #type:ignore
+                zf.extractall(path=target_folder)
+        except Exception as e:
+            raise Exception(f'Error extracting zip file: {e}') #type:ignore
+        else:
+            return target_folder
+    else:
+        try:
+            with ZipFile(zip_path) as zf: #type:ignore
+                zf.extractall(path=target_folder, pwd=pwd)
+        except Exception as e:
+            raise Exception(f'Error extracting zip file: {e}') #type:ignore
+        else:
+            return target_folder
+    
   def crack_using_wordlist(zip_file, wordlist_path): #type:ignore
     from tqdm import tqdm
     import zipfile
     from .colorcodes import colorcodes
     import os
     #type:ignore
     if not os.path.exists(wordlist_path):
@@ -14,12 +33,12 @@
         for word in tqdm(wordlist, total=n_words, unit="word"):
             try:
                 zip_file.extractall(pwd=word.strip())
             except Exception:
                 continue
             else:
                 print("[+] Password found:", word.decode().strip())
-                exit(0)
+                return word.decode().strip()
         print("[!] Password not found, try other wordlist.")
```

### Comparing `dreamhack-1.0.2/dreamhack.egg-info/PKG-INFO` & `dreamhack-1.0.3/dreamhack.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,59 @@
 Metadata-Version: 2.1
 Name: dreamhack
-Version: 1.0.2
+Version: 1.0.3
 Summary: The ultimate PyPi package for cyber-security and many other things.
 Author: Jack Burr
 Author-email: BurrJ22@Outlook.com
 Keywords: python,windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Dist: cryptography
 Requires-Dist: tqdm
 Requires-Dist: setuptools
 Requires-Dist: pyuac
 Requires-Dist: requests
+Requires-Dist: public-ip
+Requires-Dist: keyboard
+Requires-Dist: pyautogui
+Requires-Dist: customtkinter
+Requires-Dist: CTkMessagebox
 
 The ultimate PyPi package for cyber-security, encryption, and many other things to simplify your code and make more advanced programs.
 
+*DISCLAIMER* I am not responsible for any damages caused by this package. Please do not use any features of this package for any bad purposes.
+
 RELEASE NOTES: 
 
+v1.0.3: 
+
+- Added logging content 
+
+- Added the ability to get the public ip of the current machine 
+
+- Added lots of new features 
+
+- A few bug fixes
+
 v1.0.2: 
 
 - First official stable version, DO NOT USE PREVIOUS VERSIONS 
 
 - Added content to encryption and logging 
 
 - Created networking 
 
 
+
+WARNING: VERSIONS BELOW THIS NOTE ARE UNSTABLE. DO NOT USE THEM.
+
+
 v1.0.1: 
 
-- Fixed critical error from v1.0.1 
+- Fixed critical error from v1.0.0 
 
 - Working on new version 
 
 
 v1.0.0: 
 
 - Initial release
```

### Comparing `dreamhack-1.0.2/setup.py` & `dreamhack-1.0.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,46 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.2' 
+VERSION = '1.0.3' 
 DESCRIPTION = 'The ultimate PyPi package for cyber-security and many other things.'
 LONG_DESCRIPTION = '''The ultimate PyPi package for cyber-security, encryption, and many other things to simplify your code and make more advanced programs.
 
+*DISCLAIMER* I am not responsible for any damages caused by this package. Please do not use any features of this package for any bad purposes.
+
 RELEASE NOTES: \n
+v1.0.3: \n
+- Added logging content \n
+- Added the ability to get the public ip of the current machine \n
+- Added lots of new features \n
+- A few bug fixes
+
 v1.0.2: \n
 - First official stable version, DO NOT USE PREVIOUS VERSIONS \n
 - Added content to encryption and logging \n
 - Created networking \n
-
+\n
+WARNING: VERSIONS BELOW THIS NOTE ARE UNSTABLE. DO NOT USE THEM.
+\n
 v1.0.1: \n
-- Fixed critical error from v1.0.1 \n
+- Fixed critical error from v1.0.0 \n
 - Working on new version \n
 
 v1.0.0: \n
 - Initial release \n
 - NOTE: Encryption and logging are both empty for the first few versions. \n
 '''
 
-# Setting up
 setup(
         name="dreamhack", 
         version=VERSION,
         author="Jack Burr",
         author_email="BurrJ22@Outlook.com",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
-        install_requires=['cryptography', 'tqdm', 'setuptools', 'pyuac', 'requests'], 
+        install_requires=['cryptography', 'tqdm', 'setuptools', 'pyuac', 'requests', 'public-ip', 'keyboard', 'pyautogui', 'customtkinter', 'CTkMessagebox'],  #type:ignore
         keywords=['python', 'windows'],
         classifiers= [
             "Programming Language :: Python :: 3",
             "Operating System :: Microsoft :: Windows",
         ]
 )
```

