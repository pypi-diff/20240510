# Comparing `tmp/dreamhack-1.0.3.tar.gz` & `tmp/dreamhack-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreamhack-1.0.3.tar", last modified: Thu May  9 21:18:45 2024, max compression
+gzip compressed data, was "dreamhack-1.0.4.tar", last modified: Fri May 10 15:56:50 2024, max compression
```

## Comparing `dreamhack-1.0.3.tar` & `dreamhack-1.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-09 21:18:45.127898 dreamhack-1.0.3/
--rw-r--r--   0 runner    (1000) runner    (1000)     1400 2024-05-09 21:18:45.127898 dreamhack-1.0.3/PKG-INFO
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-09 21:18:45.123898 dreamhack-1.0.3/dreamhack/
--rw-r--r--   0 runner    (1000) runner    (1000)      805 2024-05-09 21:06:53.000000 dreamhack-1.0.3/dreamhack/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      865 2024-05-09 14:39:14.000000 dreamhack-1.0.3/dreamhack/colorcodes.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1007 2024-05-09 20:31:28.000000 dreamhack-1.0.3/dreamhack/downloads.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2460 2024-05-09 20:51:18.000000 dreamhack-1.0.3/dreamhack/encryption.py
--rw-r--r--   0 runner    (1000) runner    (1000)      350 2024-05-09 20:40:34.000000 dreamhack-1.0.3/dreamhack/filepaths.py
--rw-r--r--   0 runner    (1000) runner    (1000)      695 2024-05-09 21:01:14.000000 dreamhack-1.0.3/dreamhack/gui.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1414 2024-05-09 18:30:04.000000 dreamhack-1.0.3/dreamhack/logging.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1446 2024-05-09 18:41:27.000000 dreamhack-1.0.3/dreamhack/networking.py
--rw-r--r--   0 runner    (1000) runner    (1000)      594 2024-05-09 18:46:07.000000 dreamhack-1.0.3/dreamhack/randoms.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3483 2024-05-09 21:08:32.000000 dreamhack-1.0.3/dreamhack/windows.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1596 2024-05-09 21:12:36.000000 dreamhack-1.0.3/dreamhack/zipfiles.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-09 21:18:45.127898 dreamhack-1.0.3/dreamhack.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1400 2024-05-09 21:18:44.000000 dreamhack-1.0.3/dreamhack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      414 2024-05-09 21:18:44.000000 dreamhack-1.0.3/dreamhack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-09 21:18:44.000000 dreamhack-1.0.3/dreamhack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      101 2024-05-09 21:18:44.000000 dreamhack-1.0.3/dreamhack.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       10 2024-05-09 21:18:44.000000 dreamhack-1.0.3/dreamhack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-09 21:18:45.127898 dreamhack-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)     1626 2024-05-09 21:06:25.000000 dreamhack-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-10 15:56:50.290179 dreamhack-1.0.4/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1463 2024-05-10 15:56:50.290179 dreamhack-1.0.4/PKG-INFO
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-10 15:56:50.286179 dreamhack-1.0.4/dreamhack/
+-rw-r--r--   0 runner    (1000) runner    (1000)      805 2024-05-09 21:06:53.000000 dreamhack-1.0.4/dreamhack/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      916 2024-05-10 15:50:24.000000 dreamhack-1.0.4/dreamhack/colorcodes.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1039 2024-05-10 15:50:32.000000 dreamhack-1.0.4/dreamhack/downloads.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2502 2024-05-10 15:02:31.000000 dreamhack-1.0.4/dreamhack/encryption.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      385 2024-05-10 15:50:41.000000 dreamhack-1.0.4/dreamhack/filepaths.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      759 2024-05-10 15:50:57.000000 dreamhack-1.0.4/dreamhack/gui.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1488 2024-05-10 15:51:14.000000 dreamhack-1.0.4/dreamhack/logging.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1541 2024-05-10 15:51:32.000000 dreamhack-1.0.4/dreamhack/networking.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      629 2024-05-10 15:51:48.000000 dreamhack-1.0.4/dreamhack/randoms.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3741 2024-05-10 15:52:40.000000 dreamhack-1.0.4/dreamhack/windows.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1637 2024-05-10 15:53:29.000000 dreamhack-1.0.4/dreamhack/zipfiles.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-10 15:56:50.290179 dreamhack-1.0.4/dreamhack.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1463 2024-05-10 15:56:50.000000 dreamhack-1.0.4/dreamhack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      414 2024-05-10 15:56:50.000000 dreamhack-1.0.4/dreamhack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-10 15:56:50.000000 dreamhack-1.0.4/dreamhack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      101 2024-05-10 15:56:50.000000 dreamhack-1.0.4/dreamhack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       10 2024-05-10 15:56:50.000000 dreamhack-1.0.4/dreamhack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-10 15:56:50.290179 dreamhack-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)     1692 2024-05-10 15:56:22.000000 dreamhack-1.0.4/setup.py
```

### Comparing `dreamhack-1.0.3/PKG-INFO` & `dreamhack-1.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamhack
-Version: 1.0.3
+Version: 1.0.4
 Summary: The ultimate PyPi package for cyber-security and many other things.
 Author: Jack Burr
 Author-email: BurrJ22@Outlook.com
 Keywords: python,windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Dist: cryptography
@@ -16,18 +16,25 @@
 Requires-Dist: keyboard
 Requires-Dist: pyautogui
 Requires-Dist: customtkinter
 Requires-Dist: CTkMessagebox
 
 The ultimate PyPi package for cyber-security, encryption, and many other things to simplify your code and make more advanced programs.
 
-*DISCLAIMER* I am not responsible for any damages caused by this package. Please do not use any features of this package for any bad purposes.
+*DISCLAIMER:* I am not responsible for any damages caused by this package. Please do not use any features of this package for any bad purposes.
 
 RELEASE NOTES: 
 
+v1.0.4: 
+
+- Fixed a few bugs 
+
+- Added a few more features 
+
+
 v1.0.3: 
 
 - Added logging content 
 
 - Added the ability to get the public ip of the current machine 
 
 - Added lots of new features
```

### Comparing `dreamhack-1.0.3/dreamhack/__init__.py` & `dreamhack-1.0.4/dreamhack/__init__.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.0.3/dreamhack/colorcodes.py` & `dreamhack-1.0.4/dreamhack/colorcodes.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,16 +19,20 @@
   BOLD = "\033[1m"
   FAINT = "\033[2m"
   ITALIC = "\033[3m"
   UNDERLINE = "\033[4m"
   BLINK = "\033[5m"
   NEGATIVE = "\033[7m"
   CROSSED = "\033[9m"
+  
+  @staticmethod
   def red(text):
     return colorcodes.RED + text + colorcodes.NO_COLOR #type:ignore
 
+  @staticmethod
   def green(text):
     return colorcodes.GREEN + text + colorcodes.NO_COLOR #type:ignore
 
+  @staticmethod
   def color(text, color):
     return color + text + colorcodes.NO_COLOR #type:ignore
```

### Comparing `dreamhack-1.0.3/dreamhack/downloads.py` & `dreamhack-1.0.4/dreamhack/downloads.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 class downloads:
+  @staticmethod
   def download_file_from_github(url, save_path): #type:ignore
     import ssl
     import urllib.request
     import shutil #type:ignore
     try:
       ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLS_CLIENT)
       ssl_context.check_hostname = False
@@ -11,14 +12,15 @@
         with open(save_path, 'wb') as out_file:
           shutil.copyfileobj(response, out_file)
     except Exception as e:
       raise e
     else:
       return url, save_path
 
+  @staticmethod
   def download_webpage_content(url, save_path): #type:ignore
     import requests
     try:
       cont = requests.get(url).text #type:ignore
     except Exception:
       raise Exception('Invalid URL.') #type:ignore
     else:
```

### Comparing `dreamhack-1.0.3/dreamhack/encryption.py` & `dreamhack-1.0.4/dreamhack/encryption.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 class encryption():
+  @staticmethod
   def generate_salt(size=16):
     import secrets
     return secrets.token_bytes(size)#type:ignore
-    
+
+  @staticmethod
   def derive_key(salt, password):
     from cryptography.hazmat.primitives.kdf.scrypt import Scrypt
     kdf = Scrypt(salt=salt, length=32, n=2**14, r=8, p=1)#type:ignore
     return kdf.derive(password.encode())
 
+  @staticmethod
   def load_salt(custom_salt_filename = None):
     if custom_salt_filename is None:
       custom_salt_filename = "salt.salt"
     return open(custom_salt_filename, "rb").read()#type:ignore
-
+    
+  @staticmethod
   def generate_key(password, salt_size=16, load_existing_salt=False, save_salt=True, custom_salt_filename = 'salt.salt'):
     import base64
     salt = ""
     if load_existing_salt:
         salt = encryption.load_salt(custom_salt_filename=custom_salt_filename)#type:ignore
     elif save_salt:
         salt = encryption.generate_salt(salt_size)#type:ignore
@@ -25,44 +29,47 @@
     if salt is not None:
       derived_key = encryption.derive_key(salt, password) #type:ignore
       encode = base64.urlsafe_b64encode(derived_key)
       return encode
     else: 
       return -1 
 
+  @staticmethod
   def encrypt(filename, key):
     from cryptography.fernet import Fernet
     f = Fernet(key)
     try:
-      with open(filename, "rb") as file: #type:ignore
+      with open(filename, "rb") as file: 
           file_data = file.read()
       encrypted_data = f.encrypt(file_data)
-      with open(filename, "wb") as file: #type:ignore
+      with open(filename, "wb") as file:
           file.write(encrypted_data)
           file.close()
     except PermissionError as pe:
       return -1, f"Permission Denied to file {filename}.", pe
     except Exception as e:
       return -2, e
     else:  
       return 1
-      
+
+  @staticmethod
   def encrypt_folder(directory, key, folders_to_exclude = []):
     import os
     from .filepaths import filepaths as fp
     #type:ignore
     if folders_to_exclude is not None and directory in folders_to_exclude:
       return
-    dirlist = fp.get_all_files_in_directory(directory) #type:ignore
+    dirlist = fp.get_all_files_in_directory(directory)
     for file in dirlist:
       file = os.path.join(str(directory), str(file))
       if os.path.isfile(file):
-        encryption.encrypt(file, key) #type:ignore
+        encryption.encrypt(file, key)
       else:
-        encryption.encrypt_folder(file, key) #type:ignore
+        encryption.encrypt_folder(file, key)
 
+  @staticmethod
   def encrypt_folders_in_list(directory_list, key, whitelist=[]):
     for folder in directory_list:#type:ignore
       if folder in whitelist:
         pass
       else:
         encryption.encrypt_folder(folder, key, folders_to_exclude=whitelist)
```

### Comparing `dreamhack-1.0.3/dreamhack/gui.py` & `dreamhack-1.0.4/dreamhack/gui.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 class gui():
+  @staticmethod
   def get_tkinter_root(): #type:ignore
     import tkinter
     return tkinter.Tk()
 
+  @staticmethod
   def tk_geometry(root, width, height): #type:ignore
     try:
       return root.geometry(f'{width}x{height}') #type:ignore
     except Exception:
       raise Exception('Invalid Root.') #type:ignore
 
 # ----------------------------------CUSTOMTKINTER---------------------------------------
+  @staticmethod
   def get_customtkinter_root(): #type:ignore
     import customtkinter #type:ignore
     return customtkinter.CTk()
 
+  @staticmethod
   def ctk_geometry(root, width, height): #type:ignore
     try:
       return root.geometry(f'{width}x{height}') #type:ignore
     except Exception:
       raise Exception('Invalid Root.') #type:ignore
```

### Comparing `dreamhack-1.0.3/dreamhack/logging.py` & `dreamhack-1.0.4/dreamhack/logging.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 class logging():
+  @staticmethod
   def create_log_file(log_path): #type:ignore
     from datetime import datetime
     now = datetime.now()
     yr = now.year
     mo = now.month
     dy = now.day
     hr = now.hour
@@ -13,14 +14,15 @@
         f.write(f"[{yr}_{mo}_{dy}_{hr}_{min}_{se}] \n \n")
         f.close()
     except FileExistsError:
       raise FileExistsError('Log file already exists.') #type:ignore
     except Exception as e:
       raise e
 
+  @staticmethod
   def log(log_path, message, symbol='*'): #type:ignore
     from datetime import datetime
     now = datetime.now()
     yr = now.year
     mo = now.month
     dy = now.day
     hr = now.hour
@@ -35,13 +37,15 @@
           logging.create_log_file(log_path)
         except Exception:
           raise FileNotFoundError('Invalid Log Path.') #type:ignore
         else:
           logging.log(log_path, message)
     except Exception as e:
       raise Exception(f'Error creating log file: {e}') #type:ignore
-
+      
+  @staticmethod
   def error(log_path, message): #type:ignore
     logging.log(log_path, message, symbol='!')
-
+    
+  @staticmethod
   def warning(log_path, message): #type:ignore
     logging.log(log_path, message, symbol='#')
```

### Comparing `dreamhack-1.0.3/dreamhack/networking.py` & `dreamhack-1.0.4/dreamhack/networking.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,49 @@
 class networking():
+  
+  @staticmethod
   def ping(ip): #type:ignore
     import os
     return os.system(f'ping {ip}') #type:ignore
-  
+
+  @staticmethod
   def get_public_ip(): #type:ignore
     import public_ip as ip #type:ignore
     return ip.get()
-  
+
+  @staticmethod
   def get_private_ip_address(): #type:ignore
     import socket
     return socket.gethostbyname(socket.gethostname())
 
+  @staticmethod
   def stop_wifi_network(): #type:ignore
     import subprocess
     try:
         # Stop the hosted network
         subprocess.run(['netsh', 'wlan', 'stop', 'hostednetwork'], check=True)
     except subprocess.CalledProcessError as ex:
       raise ex
     except Exception as e:
       raise e
 
+  @staticmethod
   def start_wifi_network(): #type:ignore
     import subprocess
     import atexit
     #type:ignore
     try:
       # Start the hosted network
       subprocess.run(['netsh', 'wlan', 'start', 'hostednetwork'], check=True)
     except Exception as e:
       raise e
     else:
       atexit.register(networking.stop_wifi_network)
 
+  @staticmethod
   def create_wifi_network(ssid, password, auto_start=True):
     import os 
     import subprocess
     import atexit
     #type:ignore
     try:
         # Create the hosted network
```

### Comparing `dreamhack-1.0.3/dreamhack/randoms.py` & `dreamhack-1.0.4/dreamhack/randoms.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 class randoms():
+  
+  @staticmethod
   def random_string_generator(length): #type:ignore
     import random
     characters = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789"
     master = ""
     for x in range(int(length)): #type:ignore
       master = master + random.choice(characters)
     return master 
 
+  @staticmethod
   def random_number_in_range(min,max): #type:ignore
     import random
     try:
       return random.randrange(int(min), int(max)) #type:ignore
     except ValueError:
       raise ValueError('One or more of the numbers are invalid integers.') #type:ignore
     except Exception as e:
```

### Comparing `dreamhack-1.0.3/dreamhack/windows.py` & `dreamhack-1.0.4/dreamhack/windows.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,109 +1,127 @@
 class windows():
+
+  @staticmethod
   def block_mouse_input(on): #type:ignore
     import ctypes
     try:
       ctypes.windll.user32.BlockInput(on) #type:ignore
     except Exception as e:
       return -1, e
     else:
       return 1, on
 
+  @staticmethod
   def block_keyboard_key(key): #type:ignore
     import keyboard #type:ignore
     try:
       keyboard.block_key(key) #type:ignore
     except Exception:
       raise Exception('Invalid Keyboard Key.') #type:ignore
     else:
       return key
 
+  
+  @staticmethod
   def unblock_keyboard_key(key): #type:ignore
     import keyboard #type:ignore
     try:
       keyboard.unblock_key(key) #type:ignore
     except Exception:
       raise Exception('Invalid Keyboard Key.') #type:ignore
     else:
       return key
 
+  @staticmethod
   def disable_all_keyboard_keys(): #type:ignore
     keys_list = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789!@#"
     for key in keys_list:
       windows.block_keyboard_key(key) #type:ignore
 
+  @staticmethod
   def enable_all_keyboard_keys(): #type:ignore
     keys_list = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789!@#"
     for key in keys_list:
       windows.unblock_keyboard_key(key) #type:ignore
 
+  @staticmethod
   def shutdown(timeout): #type:ignore
     import os
     try:
       timeout = int(timeout) #type:ignore
     except Exception as e:
       raise e
     else:
       os.system(f'shutdown /s /f /t {timeout}')
-  
+
+  @staticmethod
   def get_windows_user_directory(): #type:ignore
     import os
     return os.path.expanduser('~')
 
+  @staticmethod
   def get_folder_in_user_dir(foldername): #type:ignore
     import os
     return os.path.join(os.path.expanduser('~'), str(foldername)) #type:ignore
 
+  @staticmethod
   def get_desktop_path(): #type:ignore
     return windows.get_folder_in_user_dir('Desktop') #type:ignore
 
+  @staticmethod
   def get_documents_path(): #type:ignore
     return windows.get_folder_in_user_dir('Documents') #type:ignore
-  
+
+  @staticmethod
   def create_windows_account(username, password): #type:ignore
     import subprocess
     command = f"net user {username} {password} /add /Y"
     try:
       subprocess.run(command, shell=False, check=True)
     except Exception as e: 
       raise e
     else:
       return username, password
 
+  @staticmethod
   def multi_account_create(accounts, username=None, password=None): #type:ignore
     from .randoms import randoms as r
     for x in range(int(accounts)): #type:ignore
       if username is None:
         username = r.random_string_generator(14) #type:ignore
       if password is None:
         password = r.random_string_generator(14) #type:ignore
       windows.create_windows_account(username, password) #type:ignore
 
+  @staticmethod
   def run_shell_command(command): #type:ignore
     import subprocess
     try:
       subprocess.Popen([command]) #type:ignore
     except Exception as e:
       return -1, e
     else:
       return 1, None
 
+  @staticmethod
   def taskkill(process): #type:ignore
     windows.run_shell_command(f"taskkill /f /im {process}") #type:ignore
 
+  @staticmethod
   def refresh_windows_explorer(timeout_seconds=5): #type:ignore
     import time
     windows.taskkill('explorer.exe') #type:ignore
     try:
       time.sleep(int(timeout_seconds)) #type:ignore
     except Exception:
       time.sleep(5)
     windows.run_shell_command('explorer.exe') #type:ignore
 
-
+  
+  @staticmethod
   def allow_in_windows_defender(file): #type:ignore
     import os
     base = os.path.basename(file) #type:ignore
     try:
       split = base.split(".")[0]
     except Exception:
       split = base
```

### Comparing `dreamhack-1.0.3/dreamhack/zipfiles.py` & `dreamhack-1.0.4/dreamhack/zipfiles.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 class zipfiles():
+  @staticmethod
   def extract(zip_path, target_folder, pwd=None): #type:ignore
     from zipfile import ZipFile
     if pwd is None:
         try:
             with ZipFile(zip_path) as zf: #type:ignore
                 zf.extractall(path=target_folder)
         except Exception as e:
@@ -13,17 +14,18 @@
         try:
             with ZipFile(zip_path) as zf: #type:ignore
                 zf.extractall(path=target_folder, pwd=pwd)
         except Exception as e:
             raise Exception(f'Error extracting zip file: {e}') #type:ignore
         else:
             return target_folder
-    
+
+  @staticmethod
   def crack_using_wordlist(zip_file, wordlist_path): #type:ignore
-    from tqdm import tqdm
+    from tqdm import tqdm #type:ignore
     import zipfile
     from .colorcodes import colorcodes
     import os
     #type:ignore
     if not os.path.exists(wordlist_path):
         raise FileNotFoundError(colorcodes.red('Invalid Wordlist Path.'))#type:ignore
     zip_file = zipfile.ZipFile(zip_file) #type:ignore
```

### Comparing `dreamhack-1.0.3/dreamhack.egg-info/PKG-INFO` & `dreamhack-1.0.4/dreamhack.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamhack
-Version: 1.0.3
+Version: 1.0.4
 Summary: The ultimate PyPi package for cyber-security and many other things.
 Author: Jack Burr
 Author-email: BurrJ22@Outlook.com
 Keywords: python,windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Dist: cryptography
@@ -16,18 +16,25 @@
 Requires-Dist: keyboard
 Requires-Dist: pyautogui
 Requires-Dist: customtkinter
 Requires-Dist: CTkMessagebox
 
 The ultimate PyPi package for cyber-security, encryption, and many other things to simplify your code and make more advanced programs.
 
-*DISCLAIMER* I am not responsible for any damages caused by this package. Please do not use any features of this package for any bad purposes.
+*DISCLAIMER:* I am not responsible for any damages caused by this package. Please do not use any features of this package for any bad purposes.
 
 RELEASE NOTES: 
 
+v1.0.4: 
+
+- Fixed a few bugs 
+
+- Added a few more features 
+
+
 v1.0.3: 
 
 - Added logging content 
 
 - Added the ability to get the public ip of the current machine 
 
 - Added lots of new features
```

### Comparing `dreamhack-1.0.3/setup.py` & `dreamhack-1.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.3' 
+VERSION = '1.0.4' 
 DESCRIPTION = 'The ultimate PyPi package for cyber-security and many other things.'
 LONG_DESCRIPTION = '''The ultimate PyPi package for cyber-security, encryption, and many other things to simplify your code and make more advanced programs.
 
-*DISCLAIMER* I am not responsible for any damages caused by this package. Please do not use any features of this package for any bad purposes.
+*DISCLAIMER:* I am not responsible for any damages caused by this package. Please do not use any features of this package for any bad purposes.
 
 RELEASE NOTES: \n
+v1.0.4: \n
+- Fixed a few bugs \n
+- Added a few more features \n
+
 v1.0.3: \n
 - Added logging content \n
 - Added the ability to get the public ip of the current machine \n
 - Added lots of new features \n
 - A few bug fixes
 
 v1.0.2: \n
```

