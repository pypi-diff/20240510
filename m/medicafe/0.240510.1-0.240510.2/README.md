# Comparing `tmp/medicafe-0.240510.1.tar.gz` & `tmp/medicafe-0.240510.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medicafe-0.240510.1.tar", last modified: Fri May 10 17:30:22 2024, max compression
+gzip compressed data, was "medicafe-0.240510.2.tar", last modified: Fri May 10 17:48:43 2024, max compression
```

## Comparing `medicafe-0.240510.1.tar` & `medicafe-0.240510.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 17:30:22.215000 medicafe-0.240510.1/
--rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240510.1/LICENSE
--rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240510.1/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-10 17:30:21.470000 medicafe-0.240510.1/MediBot/
--rwxrwxrwx   0        0        0     4417 2024-05-10 13:17:05.000000 medicafe-0.240510.1/MediBot/MediBot.bat
--rw-rw-rw-   0        0        0    17252 2024-05-09 06:49:38.000000 medicafe-0.240510.1/MediBot/MediBot.py
--rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240510.1/MediBot/MediBot_Charges.py
--rw-rw-rw-   0        0        0    33448 2024-05-10 17:00:40.000000 medicafe-0.240510.1/MediBot/MediBot_Preprocessor.py
--rw-rw-rw-   0        0        0     4652 2024-05-02 02:13:23.000000 medicafe-0.240510.1/MediBot/MediBot_Preprocessor_lib.py
--rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240510.1/MediBot/MediBot_UI.py
--rw-rw-rw-   0        0        0     6985 2024-05-10 14:14:44.000000 medicafe-0.240510.1/MediBot/MediBot_dataformat_library.py
--rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240510.1/MediBot/MediPost.py
--rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240510.1/MediBot/PDF_to_CSV_Cleaner.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240510.1/MediBot/__init__.py
--rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240510.1/MediBot/update_json.py
--rw-rw-rw-   0        0        0     2249 2024-05-10 14:22:15.000000 medicafe-0.240510.1/MediBot/update_medicafe.py
-drwxrwxrwx   0        0        0        0 2024-05-10 17:30:21.995000 medicafe-0.240510.1/MediLink/
--rw-rw-rw-   0        0        0    18174 2024-05-08 01:57:26.000000 medicafe-0.240510.1/MediLink/MediLink.py
--rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240510.1/MediLink/MediLink_277_decoder.py
--rw-rw-rw-   0        0        0    20091 2024-05-10 16:47:58.000000 medicafe-0.240510.1/MediLink/MediLink_837p_encoder.py
--rw-rw-rw-   0        0        0    35283 2024-05-10 17:28:21.000000 medicafe-0.240510.1/MediLink/MediLink_837p_encoder_library.py
--rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240510.1/MediLink/MediLink_ConfigLoader.py
--rw-rw-rw-   0        0        0    11166 2024-05-08 01:54:15.000000 medicafe-0.240510.1/MediLink/MediLink_DataMgmt.py
--rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240510.1/MediLink/MediLink_Down.py
--rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240510.1/MediLink/MediLink_ERA_decoder.py
--rw-rw-rw-   0        0        0     6236 2024-05-10 16:45:40.000000 medicafe-0.240510.1/MediLink/MediLink_Gmail.py
--rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240510.1/MediLink/MediLink_Scheduler.py
--rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240510.1/MediLink/MediLink_StatusCheck.py
--rw-rw-rw-   0        0        0     4942 2024-05-07 17:08:35.000000 medicafe-0.240510.1/MediLink/MediLink_UI.py
--rw-rw-rw-   0        0        0     5904 2024-05-08 01:58:53.000000 medicafe-0.240510.1/MediLink/MediLink_Up.py
--rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240510.1/MediLink/MediLink_batch.bat
--rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240510.1/MediLink/Soumit_api.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240510.1/MediLink/__init__.py
--rw-rw-rw-   0        0        0      730 2024-05-10 17:30:22.198000 medicafe-0.240510.1/PKG-INFO
--rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240510.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 17:30:22.179000 medicafe-0.240510.1/medicafe.egg-info/
--rw-rw-rw-   0        0        0      730 2024-05-10 17:30:20.000000 medicafe-0.240510.1/medicafe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1006 2024-05-10 17:30:20.000000 medicafe-0.240510.1/medicafe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 17:30:20.000000 medicafe-0.240510.1/medicafe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240510.1/medicafe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       60 2024-05-10 17:30:20.000000 medicafe-0.240510.1/medicafe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-10 17:30:20.000000 medicafe-0.240510.1/medicafe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 17:30:22.211000 medicafe-0.240510.1/setup.cfg
--rw-rw-rw-   0        0        0     1164 2024-05-10 17:30:19.000000 medicafe-0.240510.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 17:48:43.908000 medicafe-0.240510.2/
+-rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240510.2/LICENSE
+-rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240510.2/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-10 17:48:42.620000 medicafe-0.240510.2/MediBot/
+-rwxrwxrwx   0        0        0     4812 2024-05-10 17:47:09.000000 medicafe-0.240510.2/MediBot/MediBot.bat
+-rw-rw-rw-   0        0        0    17252 2024-05-09 06:49:38.000000 medicafe-0.240510.2/MediBot/MediBot.py
+-rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240510.2/MediBot/MediBot_Charges.py
+-rw-rw-rw-   0        0        0    33448 2024-05-10 17:00:40.000000 medicafe-0.240510.2/MediBot/MediBot_Preprocessor.py
+-rw-rw-rw-   0        0        0     4652 2024-05-02 02:13:23.000000 medicafe-0.240510.2/MediBot/MediBot_Preprocessor_lib.py
+-rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240510.2/MediBot/MediBot_UI.py
+-rw-rw-rw-   0        0        0     6985 2024-05-10 14:14:44.000000 medicafe-0.240510.2/MediBot/MediBot_dataformat_library.py
+-rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240510.2/MediBot/MediPost.py
+-rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240510.2/MediBot/PDF_to_CSV_Cleaner.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240510.2/MediBot/__init__.py
+-rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240510.2/MediBot/update_json.py
+-rw-rw-rw-   0        0        0     2249 2024-05-10 17:47:37.000000 medicafe-0.240510.2/MediBot/update_medicafe.py
+drwxrwxrwx   0        0        0        0 2024-05-10 17:48:43.455000 medicafe-0.240510.2/MediLink/
+-rw-rw-rw-   0        0        0    18174 2024-05-08 01:57:26.000000 medicafe-0.240510.2/MediLink/MediLink.py
+-rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240510.2/MediLink/MediLink_277_decoder.py
+-rw-rw-rw-   0        0        0    20091 2024-05-10 16:47:58.000000 medicafe-0.240510.2/MediLink/MediLink_837p_encoder.py
+-rw-rw-rw-   0        0        0    35996 2024-05-10 17:43:20.000000 medicafe-0.240510.2/MediLink/MediLink_837p_encoder_library.py
+-rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240510.2/MediLink/MediLink_ConfigLoader.py
+-rw-rw-rw-   0        0        0    11166 2024-05-08 01:54:15.000000 medicafe-0.240510.2/MediLink/MediLink_DataMgmt.py
+-rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240510.2/MediLink/MediLink_Down.py
+-rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240510.2/MediLink/MediLink_ERA_decoder.py
+-rw-rw-rw-   0        0        0     6236 2024-05-10 16:45:40.000000 medicafe-0.240510.2/MediLink/MediLink_Gmail.py
+-rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240510.2/MediLink/MediLink_Scheduler.py
+-rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240510.2/MediLink/MediLink_StatusCheck.py
+-rw-rw-rw-   0        0        0     4942 2024-05-07 17:08:35.000000 medicafe-0.240510.2/MediLink/MediLink_UI.py
+-rw-rw-rw-   0        0        0     5904 2024-05-08 01:58:53.000000 medicafe-0.240510.2/MediLink/MediLink_Up.py
+-rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240510.2/MediLink/MediLink_batch.bat
+-rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240510.2/MediLink/Soumit_api.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240510.2/MediLink/__init__.py
+-rw-rw-rw-   0        0        0      730 2024-05-10 17:48:43.886000 medicafe-0.240510.2/PKG-INFO
+-rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240510.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 17:48:43.853000 medicafe-0.240510.2/medicafe.egg-info/
+-rw-rw-rw-   0        0        0      730 2024-05-10 17:48:41.000000 medicafe-0.240510.2/medicafe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1006 2024-05-10 17:48:41.000000 medicafe-0.240510.2/medicafe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 17:48:41.000000 medicafe-0.240510.2/medicafe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240510.2/medicafe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       60 2024-05-10 17:48:41.000000 medicafe-0.240510.2/medicafe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-10 17:48:41.000000 medicafe-0.240510.2/medicafe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 17:48:43.903000 medicafe-0.240510.2/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2024-05-10 17:48:40.000000 medicafe-0.240510.2/setup.py
```

### Comparing `medicafe-0.240510.1/LICENSE` & `medicafe-0.240510.2/LICENSE`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.1/MediBot/MediBot.bat` & `medicafe-0.240510.2/MediBot/MediBot.bat`

 * *Files 7% similar despite different names*

```diff
@@ -28,21 +28,32 @@
 )
 
 :: Check for internet connectivity
 ping -n 1 google.com > nul 2>&1
 set "internet_available=%ERRORLEVEL%"
 
 :: Common pre-menu setup
+:: This move isn't being made, need to fix
 echo Setting up the environment...
 if not exist "%config_file%" (
     echo Configuration file missing.
     goto end_script
 )
+
+:: Check if the file exists and attempt to move it
 if exist "C:\Python34\Lib\site-packages\MediBot\upgrade_medicafe.py" (
+    echo Completing Previous Upgrade: Attempting to move upgrade_medicafe.py...
     move "C:\Python34\Lib\site-packages\MediBot\upgrade_medicafe.py" "F:\Medibot\upgrade_medicafe.py" /y
+    if errorlevel 1 (
+        echo Failed to move upgrade_medicafe.py. Error Level: %errorlevel%
+    ) else (
+        echo File moved successfully.
+    )
+) else (
+    echo New upgrade_medicafe not detected...
 )
 
 :: Main menu, ECHO is Off is whats showing up.
 :main_menu
 cls
 echo. !package_version!
 echo ---------------------------------------------
```

### Comparing `medicafe-0.240510.1/MediBot/MediBot.py` & `medicafe-0.240510.2/MediBot/MediBot.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.1/MediBot/MediBot_Charges.py` & `medicafe-0.240510.2/MediBot/MediBot_Charges.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.1/MediBot/MediBot_Preprocessor.py` & `medicafe-0.240510.2/MediBot/MediBot_Preprocessor.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.1/MediBot/MediBot_Preprocessor_lib.py` & `medicafe-0.240510.2/MediBot/MediBot_Preprocessor_lib.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.1/MediBot/MediBot_UI.py` & `medicafe-0.240510.2/MediBot/MediBot_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.1/MediBot/MediBot_dataformat_library.py` & `medicafe-0.240510.2/MediBot/MediBot_dataformat_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.1/MediBot/PDF_to_CSV_Cleaner.py` & `medicafe-0.240510.2/MediBot/PDF_to_CSV_Cleaner.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.1/MediBot/update_json.py` & `medicafe-0.240510.2/MediBot/update_json.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.1/MediBot/update_medicafe.py` & `medicafe-0.240510.2/MediBot/update_medicafe.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,16 +35,16 @@
                     print("Error: Upgrade failed. Details:")
                     print("stdout:", stdout)
                     print("stderr:", stderr)
                     sys.exit(1)
                 
                 progress_bar.update(total_progress // 2)  # Update progress bar
                 
-                # Add a 5-second sleep between runs
-                time.sleep(5)
+                # Add a 3-second sleep between runs
+                time.sleep(3)
                 
             progress_bar.update(total_progress // 2)  # Update progress bar
             print("stdout:", stdout_accumulator.decode("utf-8"))
             print("stderr:", stderr_accumulator.decode("utf-8"))
             time.sleep(1)
     except Exception as e:
         # Log any other exceptions
```

### Comparing `medicafe-0.240510.1/MediLink/MediLink.py` & `medicafe-0.240510.2/MediLink/MediLink.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.1/MediLink/MediLink_277_decoder.py` & `medicafe-0.240510.2/MediLink/MediLink_277_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.1/MediLink/MediLink_837p_encoder.py` & `medicafe-0.240510.2/MediLink/MediLink_837p_encoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.1/MediLink/MediLink_837p_encoder_library.py` & `medicafe-0.240510.2/MediLink/MediLink_837p_encoder_library.py`

 * *Files 1% similar despite different names*

```diff
@@ -406,43 +406,60 @@
         error_msg = "Failed to retrieve access token: {0}. Response status: {1}".format(str(e), response.status_code if response else 'No response')
         raise Exception(error_msg)
     except ValueError as e:
         # Handle specific errors like missing access token
         raise Exception("Configuration or server response error: {0}".format(str(e)))
 
 def fetch_payer_name_from_api(payer_id, config, endpoint):
+    """
+    TODO This is default configured for Availity
     
+    Fetches the payer name corresponding to a given payer ID from an API endpoint.
+    
+    Parameters:
+    - payer_id: The unique identifier for the payer whose name is to be fetched.
+    - config: Configuration dictionary including endpoint-specific settings.
+    - endpoint: The specific endpoint for which the payer name is being fetched.
+    
+    Returns:
+    - The payer name corresponding to the payer ID.
+    
+    Raises:
+    - requests.RequestException if there's an error in fetching the payer name from the API.
+    - ValueError if no payer is found for the given ID.
+    """
     endpoint_config = config['endpoints'].get(endpoint.upper(), {})
-    # Currently configured for Availity
     token = get_access_token(endpoint_config)  # Get the access token using the function above
        
     api_url = endpoint_config.get("api_url", "")
     headers = {
         'Authorization': 'Bearer {0}'.format(token),
         'Accept': 'application/json'
     }
     params = {'payerId': payer_id}
-    # print(params) DEBUG
 
     try:
         response = requests.get(api_url, headers=headers, params=params)
-        response.raise_for_status()  # This will raise an HTTPError if the HTTP request returned an unsuccessful status code
+        response.raise_for_status()  # Raises an HTTPError if the request was unsuccessful
+        
         data = response.json()
-        # print(data) DEBUG
                 
-        # Check if 'payers' key exists and has at least one item
         if 'payers' in data and data['payers']:
             payer = data['payers'][0]
             payer_name = payer.get('displayName') or payer.get('name', 'No name available')
             MediLink_ConfigLoader.log("Resolved payer name {} via {} API for Payer ID: {}".format(payer_name, endpoint, payer_id), config, level="INFO")
             return payer_name
         else:
             raise ValueError("No payer found for ID: {0}".format(payer_id))
     except requests.RequestException as e:
-        print("Error fetching payer name: {0}".format(e))
+        # Log the error with API response if available
+        error_msg = "Error fetching payer name: {0}".format(e)
+        if response and response.text:
+            error_msg += ". API response: {0}".format(response.text)
+        MediLink_ConfigLoader.log(error_msg, config, level="ERROR")
         raise
 
 # Test Case for API fetch
 #payer_id = "11347"
 #config = load_configuration() 
 #payer_name = fetch_payer_name_from_api(payer_id, config, endpoint='AVAILITY')
 #print(payer_id, payer_name)
```

### Comparing `medicafe-0.240510.1/MediLink/MediLink_ConfigLoader.py` & `medicafe-0.240510.2/MediLink/MediLink_ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.1/MediLink/MediLink_DataMgmt.py` & `medicafe-0.240510.2/MediLink/MediLink_DataMgmt.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.1/MediLink/MediLink_Down.py` & `medicafe-0.240510.2/MediLink/MediLink_Down.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.1/MediLink/MediLink_ERA_decoder.py` & `medicafe-0.240510.2/MediLink/MediLink_ERA_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.1/MediLink/MediLink_Gmail.py` & `medicafe-0.240510.2/MediLink/MediLink_Gmail.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.1/MediLink/MediLink_Scheduler.py` & `medicafe-0.240510.2/MediLink/MediLink_Scheduler.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.1/MediLink/MediLink_UI.py` & `medicafe-0.240510.2/MediLink/MediLink_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.1/MediLink/MediLink_Up.py` & `medicafe-0.240510.2/MediLink/MediLink_Up.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.1/PKG-INFO` & `medicafe-0.240510.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240510.1
+Version: 0.240510.2
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240510.1/README.md` & `medicafe-0.240510.2/README.md`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.1/medicafe.egg-info/PKG-INFO` & `medicafe-0.240510.2/medicafe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240510.1
+Version: 0.240510.2
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240510.1/medicafe.egg-info/SOURCES.txt` & `medicafe-0.240510.2/medicafe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.1/setup.py` & `medicafe-0.240510.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medicafe',
-    version="0.240510.1",
+    version="0.240510.2",
     description='MediCafe',
     long_description='This module ensures that MediCafe remains up-to-date by performing version checks for its dependencies on startup. It utilizes PyPI, the official repository for Python packages, to retrieve information about the latest available versions of the required packages. When an internet connection is available, MediUpdate automatically installs any available updates using pip, the package installer for Python.',
     long_description_content_type='text/markdown',
     keywords = 'medicafe python34 medibot medilink',
     url='https://github.com/katanada2',
     author='Daniel Vidaud',
     author_email='daniel@personalizedtransformation.com',
```

