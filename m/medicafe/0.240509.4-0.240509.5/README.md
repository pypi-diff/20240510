# Comparing `tmp/medicafe-0.240509.4.tar.gz` & `tmp/medicafe-0.240509.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medicafe-0.240509.4.tar", last modified: Fri May 10 03:20:32 2024, max compression
+gzip compressed data, was "medicafe-0.240509.5.tar", last modified: Fri May 10 03:28:40 2024, max compression
```

## Comparing `medicafe-0.240509.4.tar` & `medicafe-0.240509.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 03:20:32.788000 medicafe-0.240509.4/
--rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240509.4/LICENSE
--rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240509.4/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-10 03:20:32.192000 medicafe-0.240509.4/MediBot/
--rwxrwxrwx   0        0        0     4134 2024-05-10 02:57:24.000000 medicafe-0.240509.4/MediBot/MediBot.bat
--rw-rw-rw-   0        0        0    17252 2024-05-09 06:49:38.000000 medicafe-0.240509.4/MediBot/MediBot.py
--rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240509.4/MediBot/MediBot_Charges.py
--rw-rw-rw-   0        0        0    33163 2024-05-09 06:49:01.000000 medicafe-0.240509.4/MediBot/MediBot_Preprocessor.py
--rw-rw-rw-   0        0        0     4652 2024-05-02 02:13:23.000000 medicafe-0.240509.4/MediBot/MediBot_Preprocessor_lib.py
--rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240509.4/MediBot/MediBot_UI.py
--rw-rw-rw-   0        0        0     6840 2024-05-09 06:50:25.000000 medicafe-0.240509.4/MediBot/MediBot_dataformat_library.py
--rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240509.4/MediBot/MediPost.py
--rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240509.4/MediBot/PDF_to_CSV_Cleaner.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240509.4/MediBot/__init__.py
--rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240509.4/MediBot/update_json.py
--rw-rw-rw-   0        0        0     2201 2024-05-10 01:26:20.000000 medicafe-0.240509.4/MediBot/update_medicafe.py
-drwxrwxrwx   0        0        0        0 2024-05-10 03:20:32.610000 medicafe-0.240509.4/MediLink/
--rw-rw-rw-   0        0        0    18174 2024-05-08 01:57:26.000000 medicafe-0.240509.4/MediLink/MediLink.py
--rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240509.4/MediLink/MediLink_277_decoder.py
--rw-rw-rw-   0        0        0    19946 2024-05-08 01:52:49.000000 medicafe-0.240509.4/MediLink/MediLink_837p_encoder.py
--rw-rw-rw-   0        0        0    35258 2024-05-09 01:32:35.000000 medicafe-0.240509.4/MediLink/MediLink_837p_encoder_library.py
--rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240509.4/MediLink/MediLink_ConfigLoader.py
--rw-rw-rw-   0        0        0    11166 2024-05-08 01:54:15.000000 medicafe-0.240509.4/MediLink/MediLink_DataMgmt.py
--rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240509.4/MediLink/MediLink_Down.py
--rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240509.4/MediLink/MediLink_ERA_decoder.py
--rw-rw-rw-   0        0        0     6363 2024-05-10 03:19:23.000000 medicafe-0.240509.4/MediLink/MediLink_Gmail.py
--rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240509.4/MediLink/MediLink_Scheduler.py
--rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240509.4/MediLink/MediLink_StatusCheck.py
--rw-rw-rw-   0        0        0     4942 2024-05-07 17:08:35.000000 medicafe-0.240509.4/MediLink/MediLink_UI.py
--rw-rw-rw-   0        0        0     5904 2024-05-08 01:58:53.000000 medicafe-0.240509.4/MediLink/MediLink_Up.py
--rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240509.4/MediLink/MediLink_batch.bat
--rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240509.4/MediLink/Soumit_api.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240509.4/MediLink/__init__.py
--rw-rw-rw-   0        0        0      730 2024-05-10 03:20:32.774000 medicafe-0.240509.4/PKG-INFO
--rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240509.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 03:20:32.746000 medicafe-0.240509.4/medicafe.egg-info/
--rw-rw-rw-   0        0        0      730 2024-05-10 03:20:31.000000 medicafe-0.240509.4/medicafe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1006 2024-05-10 03:20:31.000000 medicafe-0.240509.4/medicafe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 03:20:31.000000 medicafe-0.240509.4/medicafe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240509.4/medicafe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       60 2024-05-10 03:20:31.000000 medicafe-0.240509.4/medicafe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-10 03:20:31.000000 medicafe-0.240509.4/medicafe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 03:20:32.783000 medicafe-0.240509.4/setup.cfg
--rw-rw-rw-   0        0        0     1164 2024-05-10 03:20:30.000000 medicafe-0.240509.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:28:40.073000 medicafe-0.240509.5/
+-rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240509.5/LICENSE
+-rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240509.5/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-10 03:28:39.306000 medicafe-0.240509.5/MediBot/
+-rwxrwxrwx   0        0        0     4134 2024-05-10 02:57:24.000000 medicafe-0.240509.5/MediBot/MediBot.bat
+-rw-rw-rw-   0        0        0    17252 2024-05-09 06:49:38.000000 medicafe-0.240509.5/MediBot/MediBot.py
+-rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240509.5/MediBot/MediBot_Charges.py
+-rw-rw-rw-   0        0        0    33163 2024-05-09 06:49:01.000000 medicafe-0.240509.5/MediBot/MediBot_Preprocessor.py
+-rw-rw-rw-   0        0        0     4652 2024-05-02 02:13:23.000000 medicafe-0.240509.5/MediBot/MediBot_Preprocessor_lib.py
+-rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240509.5/MediBot/MediBot_UI.py
+-rw-rw-rw-   0        0        0     6840 2024-05-09 06:50:25.000000 medicafe-0.240509.5/MediBot/MediBot_dataformat_library.py
+-rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240509.5/MediBot/MediPost.py
+-rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240509.5/MediBot/PDF_to_CSV_Cleaner.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240509.5/MediBot/__init__.py
+-rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240509.5/MediBot/update_json.py
+-rw-rw-rw-   0        0        0     2201 2024-05-10 01:26:20.000000 medicafe-0.240509.5/MediBot/update_medicafe.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:28:39.855000 medicafe-0.240509.5/MediLink/
+-rw-rw-rw-   0        0        0    18174 2024-05-08 01:57:26.000000 medicafe-0.240509.5/MediLink/MediLink.py
+-rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240509.5/MediLink/MediLink_277_decoder.py
+-rw-rw-rw-   0        0        0    19946 2024-05-08 01:52:49.000000 medicafe-0.240509.5/MediLink/MediLink_837p_encoder.py
+-rw-rw-rw-   0        0        0    35258 2024-05-09 01:32:35.000000 medicafe-0.240509.5/MediLink/MediLink_837p_encoder_library.py
+-rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240509.5/MediLink/MediLink_ConfigLoader.py
+-rw-rw-rw-   0        0        0    11166 2024-05-08 01:54:15.000000 medicafe-0.240509.5/MediLink/MediLink_DataMgmt.py
+-rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240509.5/MediLink/MediLink_Down.py
+-rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240509.5/MediLink/MediLink_ERA_decoder.py
+-rw-rw-rw-   0        0        0     8074 2024-05-10 03:28:07.000000 medicafe-0.240509.5/MediLink/MediLink_Gmail.py
+-rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240509.5/MediLink/MediLink_Scheduler.py
+-rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240509.5/MediLink/MediLink_StatusCheck.py
+-rw-rw-rw-   0        0        0     4942 2024-05-07 17:08:35.000000 medicafe-0.240509.5/MediLink/MediLink_UI.py
+-rw-rw-rw-   0        0        0     5904 2024-05-08 01:58:53.000000 medicafe-0.240509.5/MediLink/MediLink_Up.py
+-rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240509.5/MediLink/MediLink_batch.bat
+-rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240509.5/MediLink/Soumit_api.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240509.5/MediLink/__init__.py
+-rw-rw-rw-   0        0        0      730 2024-05-10 03:28:40.057000 medicafe-0.240509.5/PKG-INFO
+-rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240509.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 03:28:40.038000 medicafe-0.240509.5/medicafe.egg-info/
+-rw-rw-rw-   0        0        0      730 2024-05-10 03:28:38.000000 medicafe-0.240509.5/medicafe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1006 2024-05-10 03:28:38.000000 medicafe-0.240509.5/medicafe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 03:28:38.000000 medicafe-0.240509.5/medicafe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240509.5/medicafe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       60 2024-05-10 03:28:38.000000 medicafe-0.240509.5/medicafe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-10 03:28:38.000000 medicafe-0.240509.5/medicafe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 03:28:40.068000 medicafe-0.240509.5/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2024-05-10 03:28:37.000000 medicafe-0.240509.5/setup.py
```

### Comparing `medicafe-0.240509.4/LICENSE` & `medicafe-0.240509.5/LICENSE`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.4/MediBot/MediBot.bat` & `medicafe-0.240509.5/MediBot/MediBot.bat`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.4/MediBot/MediBot.py` & `medicafe-0.240509.5/MediBot/MediBot.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.4/MediBot/MediBot_Charges.py` & `medicafe-0.240509.5/MediBot/MediBot_Charges.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.4/MediBot/MediBot_Preprocessor.py` & `medicafe-0.240509.5/MediBot/MediBot_Preprocessor.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.4/MediBot/MediBot_Preprocessor_lib.py` & `medicafe-0.240509.5/MediBot/MediBot_Preprocessor_lib.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.4/MediBot/MediBot_UI.py` & `medicafe-0.240509.5/MediBot/MediBot_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.4/MediBot/MediBot_dataformat_library.py` & `medicafe-0.240509.5/MediBot/MediBot_dataformat_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.4/MediBot/PDF_to_CSV_Cleaner.py` & `medicafe-0.240509.5/MediBot/PDF_to_CSV_Cleaner.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.4/MediBot/update_json.py` & `medicafe-0.240509.5/MediBot/update_json.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.4/MediBot/update_medicafe.py` & `medicafe-0.240509.5/MediBot/update_medicafe.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.4/MediLink/MediLink.py` & `medicafe-0.240509.5/MediLink/MediLink.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.4/MediLink/MediLink_277_decoder.py` & `medicafe-0.240509.5/MediLink/MediLink_277_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.4/MediLink/MediLink_837p_encoder.py` & `medicafe-0.240509.5/MediLink/MediLink_837p_encoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.4/MediLink/MediLink_837p_encoder_library.py` & `medicafe-0.240509.5/MediLink/MediLink_837p_encoder_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.4/MediLink/MediLink_ConfigLoader.py` & `medicafe-0.240509.5/MediLink/MediLink_ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.4/MediLink/MediLink_DataMgmt.py` & `medicafe-0.240509.5/MediLink/MediLink_DataMgmt.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.4/MediLink/MediLink_Down.py` & `medicafe-0.240509.5/MediLink/MediLink_Down.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.4/MediLink/MediLink_ERA_decoder.py` & `medicafe-0.240509.5/MediLink/MediLink_ERA_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.4/MediLink/MediLink_Gmail.py` & `medicafe-0.240509.5/MediLink/MediLink_Gmail.py`

 * *Files 19% similar despite different names*

```diff
@@ -61,40 +61,71 @@
 import subprocess
 import webbrowser
 from MediLink_ConfigLoader import log
 
 def open_browser_with_executable(url, browser_path=None):
     """
     Tries to open a browser with the specified URL using a provided browser executable path or the default browser.
+    Enhanced with more detailed error handling and logging for various methods of opening a browser.
     """
     try:
         if browser_path:
-            # Use the provided executable path to open the browser
-            subprocess.Popen([browser_path, url])
-            log("Browser opened with provided executable path.")
+            # Log the path and URL attempting to be opened
+            log("Attempting to open URL with provided executable: {} {}".format(browser_path, url))
+            
+            # Attempt to use subprocess.Popen to open the browser
+            try:
+                process = subprocess.Popen([browser_path, url], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+                stdout, stderr = process.communicate()
+                if process.returncode != 0:
+                    log("Browser failed to open using subprocess.Popen. Return code: {}. Stderr: {}".format(process.returncode, stderr))
+                else:
+                    log("Browser opened with provided executable path using subprocess.Popen.")
+            except Exception as e:
+                log("subprocess.Popen failed: {}".format(e))
+                
+            # Attempt to use os.system as a fallback method if Popen fails
+            try:
+                import os
+                os_system_command = '"{}" {}'.format(browser_path, url)
+                os_system_result = os.system(os_system_command)
+                if os_system_result != 0:
+                    log("Browser failed to open using os.system. Command result code: {}".format(os_system_result))
+                else:
+                    log("Browser opened with provided executable path using os.system.")
+            except Exception as e:
+                log("os.system failed: {}".format(e))
+
         else:
             # Fall back to the default browser
-            webbrowser.open(url)
-            log("Default browser opened.")
+            log("No browser path provided. Attempting to open URL with default browser: {}".format(url))
+            try:
+                webbrowser.open(url)
+                log("Default browser opened.")
+            except Exception as e:
+                log("webbrowser.open failed: {}".format(e))
+
     except Exception as e:
-        log("Failed to open browser: {}".format(e))
+        log("Failed to open browser: Overall exception: {}".format(e))
+
 
 def initiate_link_retrieval():
     """
     Sends a request to initiate the 'get_link' action, which handles the selection of emails
     and link retrieval through the web application.
     """
     log("Initiating link retrieval process.")
     url = "https://script.google.com/macros/s/AKfycbzlq8d32mDlLdtFxgL_zvLJernlGPB64ftyxyH8F1nNlr3P-VBH6Yd0NGa1pbBc5AozvQ/exec"
     params = {'action': 'get_link'}
     try:
         response = requests.get(url, params=params)
         if response.status_code == 200:
             # Assuming the server redirects to the URL or provides it in the response for opening in the browser
             link_url = response.text  # You might need to parse this if it's in JSON or a different format
+            log("Link retrieved successfully: {}".format(link_url))
             browser_path = sys.argv[1] if len(sys.argv) > 1 else None
             open_browser_with_executable(link_url, browser_path)
         else:
             log("Failed to initiate link retrieval: HTTP status {}".format(response.status_code))
     except Exception as e:
         log("Error during link retrieval initiation: {}".format(e))
```

### Comparing `medicafe-0.240509.4/MediLink/MediLink_Scheduler.py` & `medicafe-0.240509.5/MediLink/MediLink_Scheduler.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.4/MediLink/MediLink_UI.py` & `medicafe-0.240509.5/MediLink/MediLink_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.4/MediLink/MediLink_Up.py` & `medicafe-0.240509.5/MediLink/MediLink_Up.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.4/PKG-INFO` & `medicafe-0.240509.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240509.4
+Version: 0.240509.5
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240509.4/README.md` & `medicafe-0.240509.5/README.md`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.4/medicafe.egg-info/PKG-INFO` & `medicafe-0.240509.5/medicafe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240509.4
+Version: 0.240509.5
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240509.4/medicafe.egg-info/SOURCES.txt` & `medicafe-0.240509.5/medicafe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.4/setup.py` & `medicafe-0.240509.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medicafe',
-    version="0.240509.4",
+    version="0.240509.5",
     description='MediCafe',
     long_description='This module ensures that MediCafe remains up-to-date by performing version checks for its dependencies on startup. It utilizes PyPI, the official repository for Python packages, to retrieve information about the latest available versions of the required packages. When an internet connection is available, MediUpdate automatically installs any available updates using pip, the package installer for Python.',
     long_description_content_type='text/markdown',
     keywords = 'medicafe python34 medibot medilink',
     url='https://github.com/katanada2',
     author='Daniel Vidaud',
     author_email='daniel@personalizedtransformation.com',
```

