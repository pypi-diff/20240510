# Comparing `tmp/medicafe-0.240509.2.tar.gz` & `tmp/medicafe-0.240509.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medicafe-0.240509.2.tar", last modified: Fri May 10 01:04:02 2024, max compression
+gzip compressed data, was "medicafe-0.240509.3.tar", last modified: Fri May 10 02:47:24 2024, max compression
```

## Comparing `medicafe-0.240509.2.tar` & `medicafe-0.240509.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 01:04:02.710000 medicafe-0.240509.2/
--rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240509.2/LICENSE
--rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240509.2/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-10 01:04:01.972000 medicafe-0.240509.2/MediBot/
--rwxrwxrwx   0        0        0     3556 2024-05-10 01:01:06.000000 medicafe-0.240509.2/MediBot/MediBot.bat
--rw-rw-rw-   0        0        0    17252 2024-05-09 06:49:38.000000 medicafe-0.240509.2/MediBot/MediBot.py
--rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240509.2/MediBot/MediBot_Charges.py
--rw-rw-rw-   0        0        0    33163 2024-05-09 06:49:01.000000 medicafe-0.240509.2/MediBot/MediBot_Preprocessor.py
--rw-rw-rw-   0        0        0     4652 2024-05-02 02:13:23.000000 medicafe-0.240509.2/MediBot/MediBot_Preprocessor_lib.py
--rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240509.2/MediBot/MediBot_UI.py
--rw-rw-rw-   0        0        0     6840 2024-05-09 06:50:25.000000 medicafe-0.240509.2/MediBot/MediBot_dataformat_library.py
--rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240509.2/MediBot/MediPost.py
--rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240509.2/MediBot/PDF_to_CSV_Cleaner.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240509.2/MediBot/__init__.py
--rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240509.2/MediBot/update_json.py
--rw-rw-rw-   0        0        0     1118 2024-05-09 02:39:09.000000 medicafe-0.240509.2/MediBot/update_medicafe.py
-drwxrwxrwx   0        0        0        0 2024-05-10 01:04:02.461000 medicafe-0.240509.2/MediLink/
--rw-rw-rw-   0        0        0    18174 2024-05-08 01:57:26.000000 medicafe-0.240509.2/MediLink/MediLink.py
--rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240509.2/MediLink/MediLink_277_decoder.py
--rw-rw-rw-   0        0        0    19946 2024-05-08 01:52:49.000000 medicafe-0.240509.2/MediLink/MediLink_837p_encoder.py
--rw-rw-rw-   0        0        0    35258 2024-05-09 01:32:35.000000 medicafe-0.240509.2/MediLink/MediLink_837p_encoder_library.py
--rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240509.2/MediLink/MediLink_ConfigLoader.py
--rw-rw-rw-   0        0        0    11166 2024-05-08 01:54:15.000000 medicafe-0.240509.2/MediLink/MediLink_DataMgmt.py
--rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240509.2/MediLink/MediLink_Down.py
--rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240509.2/MediLink/MediLink_ERA_decoder.py
--rw-rw-rw-   0        0        0     5654 2024-05-09 22:53:45.000000 medicafe-0.240509.2/MediLink/MediLink_Gmail.py
--rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240509.2/MediLink/MediLink_Scheduler.py
--rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240509.2/MediLink/MediLink_StatusCheck.py
--rw-rw-rw-   0        0        0     4942 2024-05-07 17:08:35.000000 medicafe-0.240509.2/MediLink/MediLink_UI.py
--rw-rw-rw-   0        0        0     5904 2024-05-08 01:58:53.000000 medicafe-0.240509.2/MediLink/MediLink_Up.py
--rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240509.2/MediLink/MediLink_batch.bat
--rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240509.2/MediLink/Soumit_api.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240509.2/MediLink/__init__.py
--rw-rw-rw-   0        0        0      730 2024-05-10 01:04:02.692000 medicafe-0.240509.2/PKG-INFO
--rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240509.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 01:04:02.674000 medicafe-0.240509.2/medicafe.egg-info/
--rw-rw-rw-   0        0        0      730 2024-05-10 01:04:01.000000 medicafe-0.240509.2/medicafe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1006 2024-05-10 01:04:01.000000 medicafe-0.240509.2/medicafe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 01:04:01.000000 medicafe-0.240509.2/medicafe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240509.2/medicafe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       60 2024-05-10 01:04:01.000000 medicafe-0.240509.2/medicafe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-10 01:04:01.000000 medicafe-0.240509.2/medicafe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 01:04:02.705000 medicafe-0.240509.2/setup.cfg
--rw-rw-rw-   0        0        0     1164 2024-05-10 01:03:57.000000 medicafe-0.240509.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 02:47:24.391000 medicafe-0.240509.3/
+-rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240509.3/LICENSE
+-rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240509.3/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-10 02:47:23.479000 medicafe-0.240509.3/MediBot/
+-rwxrwxrwx   0        0        0     4197 2024-05-10 02:34:04.000000 medicafe-0.240509.3/MediBot/MediBot.bat
+-rw-rw-rw-   0        0        0    17252 2024-05-09 06:49:38.000000 medicafe-0.240509.3/MediBot/MediBot.py
+-rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240509.3/MediBot/MediBot_Charges.py
+-rw-rw-rw-   0        0        0    33163 2024-05-09 06:49:01.000000 medicafe-0.240509.3/MediBot/MediBot_Preprocessor.py
+-rw-rw-rw-   0        0        0     4652 2024-05-02 02:13:23.000000 medicafe-0.240509.3/MediBot/MediBot_Preprocessor_lib.py
+-rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240509.3/MediBot/MediBot_UI.py
+-rw-rw-rw-   0        0        0     6840 2024-05-09 06:50:25.000000 medicafe-0.240509.3/MediBot/MediBot_dataformat_library.py
+-rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240509.3/MediBot/MediPost.py
+-rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240509.3/MediBot/PDF_to_CSV_Cleaner.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240509.3/MediBot/__init__.py
+-rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240509.3/MediBot/update_json.py
+-rw-rw-rw-   0        0        0     2201 2024-05-10 01:26:20.000000 medicafe-0.240509.3/MediBot/update_medicafe.py
+drwxrwxrwx   0        0        0        0 2024-05-10 02:47:24.070000 medicafe-0.240509.3/MediLink/
+-rw-rw-rw-   0        0        0    18174 2024-05-08 01:57:26.000000 medicafe-0.240509.3/MediLink/MediLink.py
+-rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240509.3/MediLink/MediLink_277_decoder.py
+-rw-rw-rw-   0        0        0    19946 2024-05-08 01:52:49.000000 medicafe-0.240509.3/MediLink/MediLink_837p_encoder.py
+-rw-rw-rw-   0        0        0    35258 2024-05-09 01:32:35.000000 medicafe-0.240509.3/MediLink/MediLink_837p_encoder_library.py
+-rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240509.3/MediLink/MediLink_ConfigLoader.py
+-rw-rw-rw-   0        0        0    11166 2024-05-08 01:54:15.000000 medicafe-0.240509.3/MediLink/MediLink_DataMgmt.py
+-rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240509.3/MediLink/MediLink_Down.py
+-rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240509.3/MediLink/MediLink_ERA_decoder.py
+-rw-rw-rw-   0        0        0     5966 2024-05-10 02:15:32.000000 medicafe-0.240509.3/MediLink/MediLink_Gmail.py
+-rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240509.3/MediLink/MediLink_Scheduler.py
+-rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240509.3/MediLink/MediLink_StatusCheck.py
+-rw-rw-rw-   0        0        0     4942 2024-05-07 17:08:35.000000 medicafe-0.240509.3/MediLink/MediLink_UI.py
+-rw-rw-rw-   0        0        0     5904 2024-05-08 01:58:53.000000 medicafe-0.240509.3/MediLink/MediLink_Up.py
+-rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240509.3/MediLink/MediLink_batch.bat
+-rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240509.3/MediLink/Soumit_api.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240509.3/MediLink/__init__.py
+-rw-rw-rw-   0        0        0      730 2024-05-10 02:47:24.366000 medicafe-0.240509.3/PKG-INFO
+-rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240509.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 02:47:24.281000 medicafe-0.240509.3/medicafe.egg-info/
+-rw-rw-rw-   0        0        0      730 2024-05-10 02:47:22.000000 medicafe-0.240509.3/medicafe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1006 2024-05-10 02:47:22.000000 medicafe-0.240509.3/medicafe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 02:47:22.000000 medicafe-0.240509.3/medicafe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240509.3/medicafe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       60 2024-05-10 02:47:22.000000 medicafe-0.240509.3/medicafe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-10 02:47:22.000000 medicafe-0.240509.3/medicafe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 02:47:24.384000 medicafe-0.240509.3/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2024-05-10 02:47:21.000000 medicafe-0.240509.3/setup.py
```

### Comparing `medicafe-0.240509.2/LICENSE` & `medicafe-0.240509.3/LICENSE`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.2/MediBot/MediBot.bat` & `medicafe-0.240509.3/MediBot/MediBot.bat`

 * *Files 9% similar despite different names*

```diff
@@ -6,53 +6,66 @@
 set "target_folder=C:\MEDIANSI\MediCare\CSV"
 set "config_file=F:\Medibot\json\config.json"
 set "python_script=C:\Python34\Lib\site-packages\MediBot\update_json.py"
 set "python_script2=C:\Python34\Lib\site-packages\MediBot\Medibot.py"
 set "medicafe_package=medicafe"
 set "upgrade_medicafe=F:\Medibot\update_medicafe.py"
 set "temp_file=F:\Medibot\last_update_timestamp.txt"
+set "firefox_path=C:\Program Files\Mozilla Firefox\firefox.exe"
+set "package_version="
 set PYTHONWARNINGS=ignore
 
+:: Check if the medicafe package is installed
+echo Checking installed MediCafe package version...
+python -c "import pkg_resources" > nul 2>&1
+if %errorlevel% neq 0 (
+    echo Medicafe package is not installed.
+) else (
+    echo Medicafe package is installed.
+    for /f "tokens=2 delims==" %%a in ('python -c "import pkg_resources; print(pkg_resources.get_distribution('medicafe').version)"') do set package_version=%%a
+)
+
 :: Check for internet connectivity
 ping -n 1 google.com > nul 2>&1
 set "internet_available=%ERRORLEVEL%"
 
 :: Common pre-menu setup
 echo Setting up the environment...
 if not exist "%config_file%" (
     echo Configuration file missing.
     goto end_script
 )
 if exist "C:\Python34\Lib\site-packages\MediBot\upgrade_medicafe.py" (
     move "C:\Python34\Lib\site-packages\MediBot\upgrade_medicafe.py" "F:\Medibot\upgrade_medicafe.py" /y
 )
 
-:: Main menu
+:: Main menu, it would be good to have the version number show up somewhere.
 :main_menu
 cls
+echo v%package_version%
 echo ---------------------------------------------
 echo         .//*  Welcome to MediCafe  *\\. 
 echo ---------------------------------------------
-echo Please select an option:
 echo.
+echo Please select an option:
 if "!internet_available!"=="0" (
     echo 1. Check for MediCafe Package Updates
     echo 2. Download Email de Carol
     echo 3. MediLink Claims
 )
 echo 4. Run MediBot
 echo 5. Exit
 echo.
-choice /C 12345 /N /M "Enter your choice:"
+set /p choice=Enter your choice: 
 
-if errorlevel 5 goto end_script
-if errorlevel 4 goto medibot_flow
-if errorlevel 3 goto medilink_flow
-if errorlevel 2 goto download_emails
-if errorlevel 1 goto check_updates
+if "%choice%"=="5" goto end_script
+if "%choice%"=="4" goto medibot_flow
+if "%choice%"=="3" goto medilink_flow
+if "%choice%"=="2" goto download_emails
+if "%choice%"=="1" goto check_updates
 
 :: Medicafe Update
 :check_updates
 if "!internet_available!" neq "0" (
     echo No internet connection available.
     goto main_menu
 )
@@ -68,15 +81,15 @@
 :: Download Carol's Emails
 :download_emails
 if "!internet_available!" neq "0" (
     echo No internet connection available.
     goto main_menu
 )
 echo Downloading emails...
-py "../MediLink/MediLink_Gmail.py"
+py "../MediLink/MediLink_Gmail.py" "%firefox_path%"
 if errorlevel 1 (
     echo Failed to download emails.
 ) else (
     call :process_csvs
 )
 goto main_menu
 
@@ -119,8 +132,9 @@
 set "new_csv_path=%target_folder%\SX_CSV_!timestamp!.csv"
 py "%python_script%" "%config_file%" "!new_csv_path!"
 goto :eof
 
 :: Exit Script
 :end_script
 echo Exiting MediCafe.
+pause
 exit /b
```

### Comparing `medicafe-0.240509.2/MediBot/MediBot.py` & `medicafe-0.240509.3/MediBot/MediBot.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.2/MediBot/MediBot_Charges.py` & `medicafe-0.240509.3/MediBot/MediBot_Charges.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.2/MediBot/MediBot_Preprocessor.py` & `medicafe-0.240509.3/MediBot/MediBot_Preprocessor.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.2/MediBot/MediBot_Preprocessor_lib.py` & `medicafe-0.240509.3/MediBot/MediBot_Preprocessor_lib.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.2/MediBot/MediBot_UI.py` & `medicafe-0.240509.3/MediBot/MediBot_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.2/MediBot/MediBot_dataformat_library.py` & `medicafe-0.240509.3/MediBot/MediBot_dataformat_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.2/MediBot/PDF_to_CSV_Cleaner.py` & `medicafe-0.240509.3/MediBot/PDF_to_CSV_Cleaner.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.2/MediBot/update_json.py` & `medicafe-0.240509.3/MediBot/update_json.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.2/MediLink/MediLink.py` & `medicafe-0.240509.3/MediLink/MediLink.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.2/MediLink/MediLink_277_decoder.py` & `medicafe-0.240509.3/MediLink/MediLink_277_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.2/MediLink/MediLink_837p_encoder.py` & `medicafe-0.240509.3/MediLink/MediLink_837p_encoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.2/MediLink/MediLink_837p_encoder_library.py` & `medicafe-0.240509.3/MediLink/MediLink_837p_encoder_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.2/MediLink/MediLink_ConfigLoader.py` & `medicafe-0.240509.3/MediLink/MediLink_ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.2/MediLink/MediLink_DataMgmt.py` & `medicafe-0.240509.3/MediLink/MediLink_DataMgmt.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.2/MediLink/MediLink_Down.py` & `medicafe-0.240509.3/MediLink/MediLink_Down.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.2/MediLink/MediLink_ERA_decoder.py` & `medicafe-0.240509.3/MediLink/MediLink_ERA_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.2/MediLink/MediLink_Gmail.py` & `medicafe-0.240509.3/MediLink/MediLink_Gmail.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 Notes: So the XP system can't do auth natively outside a browser and the libraries available wouldnt be
 able to do auth on the fly so we'd basically be stuck getting tokens manually that only last an hour and 
 then copy pasting those into the script like a rotating key which is not very UX friendly. So, any of the interactions 
 necessary should move to an HTML page that's served by Google Apps Script so there's no "interaction" that has to 
 happen outside of the webapp/browser. The only thing XP can do is send pre-defined actions. So, basically the XP client-side 
 has to pretty much just be a URL to open. There essentially can't be any communication.
 """
+import sys
 import requests
 import webbrowser
 from MediLink_ConfigLoader import log
 
 def initiate_link_retrieval():
     """
     Sends a request to initiate the 'get_link' action, which handles the selection of emails
@@ -69,16 +70,21 @@
     url = "https://script.google.com/macros/s/AKfycbzlq8d32mDlLdtFxgL_zvLJernlGPB64ftyxyH8F1nNlr3P-VBH6Yd0NGa1pbBc5AozvQ/exec"
     params = {'action': 'get_link'}
     try:
         response = requests.get(url, params=params)
         if response.status_code == 200:
             # Assuming the server redirects to the URL or provides it in the response for opening in the browser
             link_url = response.text  # You might need to parse this if it's in JSON or a different format
-            webbrowser.open(link_url)
+            browser_path = sys.argv[1] if len(sys.argv) > 1 else None
+            if browser_path:
+                browser = webbrowser.get(browser_path)
+                browser.open(link_url)  # Specify the browser application
+            else:
+                webbrowser.open(link_url)  # Use default browser if no path provided
             log("Web application launched successfully.")
         else:
             log("Failed to initiate link retrieval: HTTP status {}".format(response.status_code))
     except Exception as e:
         log("Error during link retrieval initiation: {}".format(e))
 
 if __name__ == "__main__":
-    initiate_link_retrieval()
+    initiate_link_retrieval()
```

### Comparing `medicafe-0.240509.2/MediLink/MediLink_Scheduler.py` & `medicafe-0.240509.3/MediLink/MediLink_Scheduler.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.2/MediLink/MediLink_UI.py` & `medicafe-0.240509.3/MediLink/MediLink_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.2/MediLink/MediLink_Up.py` & `medicafe-0.240509.3/MediLink/MediLink_Up.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.2/PKG-INFO` & `medicafe-0.240509.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240509.2
+Version: 0.240509.3
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240509.2/README.md` & `medicafe-0.240509.3/README.md`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.2/medicafe.egg-info/PKG-INFO` & `medicafe-0.240509.3/medicafe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240509.2
+Version: 0.240509.3
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240509.2/medicafe.egg-info/SOURCES.txt` & `medicafe-0.240509.3/medicafe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.2/setup.py` & `medicafe-0.240509.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medicafe',
-    version="0.240509.2",
+    version="0.240509.3",
     description='MediCafe',
     long_description='This module ensures that MediCafe remains up-to-date by performing version checks for its dependencies on startup. It utilizes PyPI, the official repository for Python packages, to retrieve information about the latest available versions of the required packages. When an internet connection is available, MediUpdate automatically installs any available updates using pip, the package installer for Python.',
     long_description_content_type='text/markdown',
     keywords = 'medicafe python34 medibot medilink',
     url='https://github.com/katanada2',
     author='Daniel Vidaud',
     author_email='daniel@personalizedtransformation.com',
```

