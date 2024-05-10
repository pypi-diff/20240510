# Comparing `tmp/medicafe-0.240509.1.tar.gz` & `tmp/medicafe-0.240509.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medicafe-0.240509.1.tar", last modified: Thu May  9 06:54:05 2024, max compression
+gzip compressed data, was "medicafe-0.240509.2.tar", last modified: Fri May 10 01:04:02 2024, max compression
```

## Comparing `medicafe-0.240509.1.tar` & `medicafe-0.240509.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 06:54:05.258000 medicafe-0.240509.1/
--rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240509.1/LICENSE
--rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240509.1/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-09 06:54:04.292000 medicafe-0.240509.1/MediBot/
--rwxrwxrwx   0        0        0     3705 2024-05-09 05:26:10.000000 medicafe-0.240509.1/MediBot/MediBot.bat
--rw-rw-rw-   0        0        0    17252 2024-05-09 06:49:38.000000 medicafe-0.240509.1/MediBot/MediBot.py
--rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240509.1/MediBot/MediBot_Charges.py
--rw-rw-rw-   0        0        0    33163 2024-05-09 06:49:01.000000 medicafe-0.240509.1/MediBot/MediBot_Preprocessor.py
--rw-rw-rw-   0        0        0     4652 2024-05-02 02:13:23.000000 medicafe-0.240509.1/MediBot/MediBot_Preprocessor_lib.py
--rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240509.1/MediBot/MediBot_UI.py
--rw-rw-rw-   0        0        0     6840 2024-05-09 06:50:25.000000 medicafe-0.240509.1/MediBot/MediBot_dataformat_library.py
--rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240509.1/MediBot/MediPost.py
--rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240509.1/MediBot/PDF_to_CSV_Cleaner.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240509.1/MediBot/__init__.py
--rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240509.1/MediBot/update_json.py
--rw-rw-rw-   0        0        0     1118 2024-05-09 02:39:09.000000 medicafe-0.240509.1/MediBot/update_medicafe.py
-drwxrwxrwx   0        0        0        0 2024-05-09 06:54:04.964000 medicafe-0.240509.1/MediLink/
--rw-rw-rw-   0        0        0    18174 2024-05-08 01:57:26.000000 medicafe-0.240509.1/MediLink/MediLink.py
--rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240509.1/MediLink/MediLink_277_decoder.py
--rw-rw-rw-   0        0        0    19946 2024-05-08 01:52:49.000000 medicafe-0.240509.1/MediLink/MediLink_837p_encoder.py
--rw-rw-rw-   0        0        0    35258 2024-05-09 01:32:35.000000 medicafe-0.240509.1/MediLink/MediLink_837p_encoder_library.py
--rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240509.1/MediLink/MediLink_ConfigLoader.py
--rw-rw-rw-   0        0        0    11166 2024-05-08 01:54:15.000000 medicafe-0.240509.1/MediLink/MediLink_DataMgmt.py
--rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240509.1/MediLink/MediLink_Down.py
--rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240509.1/MediLink/MediLink_ERA_decoder.py
--rw-rw-rw-   0        0        0     7063 2024-05-08 21:34:31.000000 medicafe-0.240509.1/MediLink/MediLink_Gmail.py
--rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240509.1/MediLink/MediLink_Scheduler.py
--rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240509.1/MediLink/MediLink_StatusCheck.py
--rw-rw-rw-   0        0        0     4942 2024-05-07 17:08:35.000000 medicafe-0.240509.1/MediLink/MediLink_UI.py
--rw-rw-rw-   0        0        0     5904 2024-05-08 01:58:53.000000 medicafe-0.240509.1/MediLink/MediLink_Up.py
--rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240509.1/MediLink/MediLink_batch.bat
--rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240509.1/MediLink/Soumit_api.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240509.1/MediLink/__init__.py
--rw-rw-rw-   0        0        0      730 2024-05-09 06:54:05.240000 medicafe-0.240509.1/PKG-INFO
--rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240509.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 06:54:05.219000 medicafe-0.240509.1/medicafe.egg-info/
--rw-rw-rw-   0        0        0      730 2024-05-09 06:54:03.000000 medicafe-0.240509.1/medicafe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1006 2024-05-09 06:54:03.000000 medicafe-0.240509.1/medicafe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 06:54:03.000000 medicafe-0.240509.1/medicafe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240509.1/medicafe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       60 2024-05-09 06:54:03.000000 medicafe-0.240509.1/medicafe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-09 06:54:03.000000 medicafe-0.240509.1/medicafe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 06:54:05.254000 medicafe-0.240509.1/setup.cfg
--rw-rw-rw-   0        0        0     1164 2024-05-09 06:54:02.000000 medicafe-0.240509.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 01:04:02.710000 medicafe-0.240509.2/
+-rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240509.2/LICENSE
+-rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240509.2/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-10 01:04:01.972000 medicafe-0.240509.2/MediBot/
+-rwxrwxrwx   0        0        0     3556 2024-05-10 01:01:06.000000 medicafe-0.240509.2/MediBot/MediBot.bat
+-rw-rw-rw-   0        0        0    17252 2024-05-09 06:49:38.000000 medicafe-0.240509.2/MediBot/MediBot.py
+-rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240509.2/MediBot/MediBot_Charges.py
+-rw-rw-rw-   0        0        0    33163 2024-05-09 06:49:01.000000 medicafe-0.240509.2/MediBot/MediBot_Preprocessor.py
+-rw-rw-rw-   0        0        0     4652 2024-05-02 02:13:23.000000 medicafe-0.240509.2/MediBot/MediBot_Preprocessor_lib.py
+-rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240509.2/MediBot/MediBot_UI.py
+-rw-rw-rw-   0        0        0     6840 2024-05-09 06:50:25.000000 medicafe-0.240509.2/MediBot/MediBot_dataformat_library.py
+-rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240509.2/MediBot/MediPost.py
+-rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240509.2/MediBot/PDF_to_CSV_Cleaner.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240509.2/MediBot/__init__.py
+-rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240509.2/MediBot/update_json.py
+-rw-rw-rw-   0        0        0     1118 2024-05-09 02:39:09.000000 medicafe-0.240509.2/MediBot/update_medicafe.py
+drwxrwxrwx   0        0        0        0 2024-05-10 01:04:02.461000 medicafe-0.240509.2/MediLink/
+-rw-rw-rw-   0        0        0    18174 2024-05-08 01:57:26.000000 medicafe-0.240509.2/MediLink/MediLink.py
+-rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240509.2/MediLink/MediLink_277_decoder.py
+-rw-rw-rw-   0        0        0    19946 2024-05-08 01:52:49.000000 medicafe-0.240509.2/MediLink/MediLink_837p_encoder.py
+-rw-rw-rw-   0        0        0    35258 2024-05-09 01:32:35.000000 medicafe-0.240509.2/MediLink/MediLink_837p_encoder_library.py
+-rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240509.2/MediLink/MediLink_ConfigLoader.py
+-rw-rw-rw-   0        0        0    11166 2024-05-08 01:54:15.000000 medicafe-0.240509.2/MediLink/MediLink_DataMgmt.py
+-rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240509.2/MediLink/MediLink_Down.py
+-rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240509.2/MediLink/MediLink_ERA_decoder.py
+-rw-rw-rw-   0        0        0     5654 2024-05-09 22:53:45.000000 medicafe-0.240509.2/MediLink/MediLink_Gmail.py
+-rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240509.2/MediLink/MediLink_Scheduler.py
+-rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240509.2/MediLink/MediLink_StatusCheck.py
+-rw-rw-rw-   0        0        0     4942 2024-05-07 17:08:35.000000 medicafe-0.240509.2/MediLink/MediLink_UI.py
+-rw-rw-rw-   0        0        0     5904 2024-05-08 01:58:53.000000 medicafe-0.240509.2/MediLink/MediLink_Up.py
+-rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240509.2/MediLink/MediLink_batch.bat
+-rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240509.2/MediLink/Soumit_api.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240509.2/MediLink/__init__.py
+-rw-rw-rw-   0        0        0      730 2024-05-10 01:04:02.692000 medicafe-0.240509.2/PKG-INFO
+-rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240509.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 01:04:02.674000 medicafe-0.240509.2/medicafe.egg-info/
+-rw-rw-rw-   0        0        0      730 2024-05-10 01:04:01.000000 medicafe-0.240509.2/medicafe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1006 2024-05-10 01:04:01.000000 medicafe-0.240509.2/medicafe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 01:04:01.000000 medicafe-0.240509.2/medicafe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240509.2/medicafe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       60 2024-05-10 01:04:01.000000 medicafe-0.240509.2/medicafe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-10 01:04:01.000000 medicafe-0.240509.2/medicafe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 01:04:02.705000 medicafe-0.240509.2/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2024-05-10 01:03:57.000000 medicafe-0.240509.2/setup.py
```

### Comparing `medicafe-0.240509.1/LICENSE` & `medicafe-0.240509.2/LICENSE`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.1/MediBot/MediBot.py` & `medicafe-0.240509.2/MediBot/MediBot.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.1/MediBot/MediBot_Charges.py` & `medicafe-0.240509.2/MediBot/MediBot_Charges.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.1/MediBot/MediBot_Preprocessor.py` & `medicafe-0.240509.2/MediBot/MediBot_Preprocessor.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.1/MediBot/MediBot_Preprocessor_lib.py` & `medicafe-0.240509.2/MediBot/MediBot_Preprocessor_lib.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.1/MediBot/MediBot_UI.py` & `medicafe-0.240509.2/MediBot/MediBot_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.1/MediBot/MediBot_dataformat_library.py` & `medicafe-0.240509.2/MediBot/MediBot_dataformat_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.1/MediBot/PDF_to_CSV_Cleaner.py` & `medicafe-0.240509.2/MediBot/PDF_to_CSV_Cleaner.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.1/MediBot/update_json.py` & `medicafe-0.240509.2/MediBot/update_json.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.1/MediBot/update_medicafe.py` & `medicafe-0.240509.2/MediBot/update_medicafe.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.1/MediLink/MediLink.py` & `medicafe-0.240509.2/MediLink/MediLink.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.1/MediLink/MediLink_277_decoder.py` & `medicafe-0.240509.2/MediLink/MediLink_277_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.1/MediLink/MediLink_837p_encoder.py` & `medicafe-0.240509.2/MediLink/MediLink_837p_encoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.1/MediLink/MediLink_837p_encoder_library.py` & `medicafe-0.240509.2/MediLink/MediLink_837p_encoder_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.1/MediLink/MediLink_ConfigLoader.py` & `medicafe-0.240509.2/MediLink/MediLink_ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.1/MediLink/MediLink_DataMgmt.py` & `medicafe-0.240509.2/MediLink/MediLink_DataMgmt.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.1/MediLink/MediLink_Down.py` & `medicafe-0.240509.2/MediLink/MediLink_Down.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.1/MediLink/MediLink_ERA_decoder.py` & `medicafe-0.240509.2/MediLink/MediLink_ERA_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.1/MediLink/MediLink_Gmail.py` & `medicafe-0.240509.2/MediLink/MediLink_Gmail.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """
+TODO All of this needs to get re-written to match the current implementation and the lessons learned.
+
 NOTE: Also download the surgery schedule. So sometimes it doesn't need the OTP.
 
 This script facilitates the process of accessing a notification email from Outlook 365, which contains a secure link to view a message. The script automates the retrieval of this link and the OTP sent by email to authenticate and access the content securely.
 
 **Challenges:**
 1. Extracting a 'Read the message' link from an email notification sent via Outlook 365.
 2. Monitoring Gmail programmatically for an OTP email sent as part of Microsoft's secure email authentication process.
@@ -42,96 +44,41 @@
     - Authenticate and access Gmail to extract the 'Read the message' link.
     - Provide support for initial email filtering and link extraction.
     - Not involved in the decryption or direct handling of PHI data to ensure compliance with HIPAA.
 
 This architecture ensures the system handles sensitive PHI data in compliance with HIPAA regulations while maintaining robust and reliable email processing and file handling mechanisms. All sensitive data transfers occur directly from Microsoft's secure environment, minimizing the risk of unauthorized access during transit.
 
 TODO (High GMail)
+
+Notes: So the XP system can't do auth natively outside a browser and the libraries available wouldnt be
+able to do auth on the fly so we'd basically be stuck getting tokens manually that only last an hour and 
+then copy pasting those into the script like a rotating key which is not very UX friendly. So, any of the interactions 
+necessary should move to an HTML page that's served by Google Apps Script so there's no "interaction" that has to 
+happen outside of the webapp/browser. The only thing XP can do is send pre-defined actions. So, basically the XP client-side 
+has to pretty much just be a URL to open. There essentially can't be any communication.
 """
 import requests
 import webbrowser
-import time
 from MediLink_ConfigLoader import log
 
-def initiate_process():
-    """
-    Initiates the process to retrieve the link and OTP from the Google Apps Script,
-    authenticate on Microsoft's secure email portal, and download the secured content.
-    """
-    log("Process initiated by the user.")
-    
-    # Retrieve the 'Read the message' link
-    link = retrieve_link()
-    if link:
-        log("Link retrieved: " + link)
-        webbrowser.open(link)
-        log("Please authenticate and ensure the OTP is received.")
-        
-        # Poll for the OTP rather than starting a server
-        otp = poll_for_otp()
-        if otp:
-            log("OTP retrieved: " + otp)
-            log("Complete the authentication in the opened web browser manually using the retrieved OTP.")
-            input("Press Enter after you have completed the download of the file...")
-        else:
-            log("Failed to retrieve OTP.")
-    else:
-        log("Failed to retrieve the link.")
-
-def retrieve_link():
+def initiate_link_retrieval():
     """
-    Retrieves the 'Read the message' link from the Google Apps Script.
+    Sends a request to initiate the 'get_link' action, which handles the selection of emails
+    and link retrieval through the web application.
     """
+    log("Initiating link retrieval process.")
+    url = "https://script.google.com/macros/s/AKfycbzlq8d32mDlLdtFxgL_zvLJernlGPB64ftyxyH8F1nNlr3P-VBH6Yd0NGa1pbBc5AozvQ/exec"
+    params = {'action': 'get_link'}
     try:
-        url = "https://script.google.com/macros/s/AKfycbzlq8d32mDlLdtFxgL_zvLJernlGPB64ftyxyH8F1nNlr3P-VBH6Yd0NGa1pbBc5AozvQ/exec"
-        params = {'action': 'get_link'}
         response = requests.get(url, params=params)
         if response.status_code == 200:
-            # Use the new JSON response handling method
-            link_response = handle_response(response)
-            if link_response:
-                return link_response
-            else:
-                log("Failed to retrieve link: No link available in the response.")
+            # Assuming the server redirects to the URL or provides it in the response for opening in the browser
+            link_url = response.text  # You might need to parse this if it's in JSON or a different format
+            webbrowser.open(link_url)
+            log("Web application launched successfully.")
         else:
-            log("Failed to retrieve link: HTTP status {}, Response text: {}".format(response.status_code, response.text))
+            log("Failed to initiate link retrieval: HTTP status {}".format(response.status_code))
     except Exception as e:
-        log("Error retrieving link: {}".format(str(e)))
-    return None
-
-def poll_for_otp():
-    """
-    Polls the Google Apps Script for the OTP, waiting until it is available.
-    """
-    url = "https://script.google.com/macros/s/AKfycbzlq8d32mDlLdtFxgL_zvLJernlGPB64ftyxyH8F1nNlr3P-VBH6Yd0NGa1pbBc5AozvQ/exec"
-    params = {'action': 'get_otp'}
-    timeout = time.time() + 60*1  # Poll for 1 minute max
-    while time.time() < timeout:
-        response = requests.get(url, params=params)
-        if response.status_code == 200:
-            # Use the new JSON response handling method
-            otp_response = handle_response(response)
-            if otp_response:
-                return otp_response
-        else:
-            log("Failed to retrieve OTP, HTTP status: {}".format(response.status_code))
-        time.sleep(15)  # Poll every 15 seconds
-    log("OTP not retrieved within the timeout period.")
-    return None
-
-def handle_response(response):
-    """
-    Parses the JSON response from the server and returns data if successful,
-    otherwise logs an error message.
-    """
-    try:
-        data = response.json()  # Parse the JSON string
-        if data['status'] == 'success':
-            return data['data']
-        else:
-            log("Error: " + data['message'])
-    except ValueError:
-        log("Error parsing response: Invalid JSON format.")
-    return None
+        log("Error during link retrieval initiation: {}".format(e))
 
 if __name__ == "__main__":
-    initiate_process()
+    initiate_link_retrieval()
```

### Comparing `medicafe-0.240509.1/MediLink/MediLink_Scheduler.py` & `medicafe-0.240509.2/MediLink/MediLink_Scheduler.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.1/MediLink/MediLink_UI.py` & `medicafe-0.240509.2/MediLink/MediLink_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.1/MediLink/MediLink_Up.py` & `medicafe-0.240509.2/MediLink/MediLink_Up.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.1/PKG-INFO` & `medicafe-0.240509.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240509.1
+Version: 0.240509.2
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240509.1/README.md` & `medicafe-0.240509.2/README.md`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.1/medicafe.egg-info/PKG-INFO` & `medicafe-0.240509.2/medicafe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240509.1
+Version: 0.240509.2
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240509.1/medicafe.egg-info/SOURCES.txt` & `medicafe-0.240509.2/medicafe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.1/setup.py` & `medicafe-0.240509.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medicafe',
-    version="0.240509.1",
+    version="0.240509.2",
     description='MediCafe',
     long_description='This module ensures that MediCafe remains up-to-date by performing version checks for its dependencies on startup. It utilizes PyPI, the official repository for Python packages, to retrieve information about the latest available versions of the required packages. When an internet connection is available, MediUpdate automatically installs any available updates using pip, the package installer for Python.',
     long_description_content_type='text/markdown',
     keywords = 'medicafe python34 medibot medilink',
     url='https://github.com/katanada2',
     author='Daniel Vidaud',
     author_email='daniel@personalizedtransformation.com',
```

