# Comparing `tmp/medicafe-0.240509.6.tar.gz` & `tmp/medicafe-0.240510.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medicafe-0.240509.6.tar", last modified: Fri May 10 03:47:41 2024, max compression
+gzip compressed data, was "medicafe-0.240510.0.tar", last modified: Fri May 10 14:15:41 2024, max compression
```

## Comparing `medicafe-0.240509.6.tar` & `medicafe-0.240510.0.tar`

### file list

```diff
@@ -1,44 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 03:47:41.942000 medicafe-0.240509.6/
--rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240509.6/LICENSE
--rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240509.6/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-10 03:47:40.812000 medicafe-0.240509.6/MediBot/
--rwxrwxrwx   0        0        0     4257 2024-05-10 03:47:04.000000 medicafe-0.240509.6/MediBot/MediBot.bat
--rw-rw-rw-   0        0        0    17252 2024-05-09 06:49:38.000000 medicafe-0.240509.6/MediBot/MediBot.py
--rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240509.6/MediBot/MediBot_Charges.py
--rw-rw-rw-   0        0        0    33163 2024-05-09 06:49:01.000000 medicafe-0.240509.6/MediBot/MediBot_Preprocessor.py
--rw-rw-rw-   0        0        0     4652 2024-05-02 02:13:23.000000 medicafe-0.240509.6/MediBot/MediBot_Preprocessor_lib.py
--rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240509.6/MediBot/MediBot_UI.py
--rw-rw-rw-   0        0        0     6840 2024-05-09 06:50:25.000000 medicafe-0.240509.6/MediBot/MediBot_dataformat_library.py
--rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240509.6/MediBot/MediPost.py
--rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240509.6/MediBot/PDF_to_CSV_Cleaner.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240509.6/MediBot/__init__.py
--rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240509.6/MediBot/update_json.py
--rw-rw-rw-   0        0        0     2201 2024-05-10 01:26:20.000000 medicafe-0.240509.6/MediBot/update_medicafe.py
-drwxrwxrwx   0        0        0        0 2024-05-10 03:47:41.541000 medicafe-0.240509.6/MediLink/
--rw-rw-rw-   0        0        0    18174 2024-05-08 01:57:26.000000 medicafe-0.240509.6/MediLink/MediLink.py
--rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240509.6/MediLink/MediLink_277_decoder.py
--rw-rw-rw-   0        0        0    19946 2024-05-08 01:52:49.000000 medicafe-0.240509.6/MediLink/MediLink_837p_encoder.py
--rw-rw-rw-   0        0        0    35258 2024-05-09 01:32:35.000000 medicafe-0.240509.6/MediLink/MediLink_837p_encoder_library.py
--rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240509.6/MediLink/MediLink_ConfigLoader.py
--rw-rw-rw-   0        0        0    11166 2024-05-08 01:54:15.000000 medicafe-0.240509.6/MediLink/MediLink_DataMgmt.py
--rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240509.6/MediLink/MediLink_Down.py
--rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240509.6/MediLink/MediLink_ERA_decoder.py
--rw-rw-rw-   0        0        0     6466 2024-05-10 03:43:36.000000 medicafe-0.240509.6/MediLink/MediLink_Gmail.py
--rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240509.6/MediLink/MediLink_Scheduler.py
--rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240509.6/MediLink/MediLink_StatusCheck.py
--rw-rw-rw-   0        0        0     4942 2024-05-07 17:08:35.000000 medicafe-0.240509.6/MediLink/MediLink_UI.py
--rw-rw-rw-   0        0        0     5904 2024-05-08 01:58:53.000000 medicafe-0.240509.6/MediLink/MediLink_Up.py
--rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240509.6/MediLink/MediLink_batch.bat
--rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240509.6/MediLink/Soumit_api.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240509.6/MediLink/__init__.py
--rw-rw-rw-   0        0        0      730 2024-05-10 03:47:41.921000 medicafe-0.240509.6/PKG-INFO
--rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240509.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 03:47:41.837000 medicafe-0.240509.6/medicafe.egg-info/
--rw-rw-rw-   0        0        0      730 2024-05-10 03:47:39.000000 medicafe-0.240509.6/medicafe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1006 2024-05-10 03:47:40.000000 medicafe-0.240509.6/medicafe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 03:47:39.000000 medicafe-0.240509.6/medicafe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240509.6/medicafe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       60 2024-05-10 03:47:39.000000 medicafe-0.240509.6/medicafe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-10 03:47:39.000000 medicafe-0.240509.6/medicafe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 03:47:41.935000 medicafe-0.240509.6/setup.cfg
--rw-rw-rw-   0        0        0     1164 2024-05-10 03:47:38.000000 medicafe-0.240509.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 14:15:41.926000 medicafe-0.240510.0/
+-rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240510.0/LICENSE
+-rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240510.0/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-10 14:15:41.266000 medicafe-0.240510.0/MediBot/
+-rwxrwxrwx   0        0        0     4417 2024-05-10 13:17:05.000000 medicafe-0.240510.0/MediBot/MediBot.bat
+-rw-rw-rw-   0        0        0    17252 2024-05-09 06:49:38.000000 medicafe-0.240510.0/MediBot/MediBot.py
+-rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240510.0/MediBot/MediBot_Charges.py
+-rw-rw-rw-   0        0        0    33163 2024-05-09 06:49:01.000000 medicafe-0.240510.0/MediBot/MediBot_Preprocessor.py
+-rw-rw-rw-   0        0        0     4652 2024-05-02 02:13:23.000000 medicafe-0.240510.0/MediBot/MediBot_Preprocessor_lib.py
+-rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240510.0/MediBot/MediBot_UI.py
+-rw-rw-rw-   0        0        0     6985 2024-05-10 14:14:44.000000 medicafe-0.240510.0/MediBot/MediBot_dataformat_library.py
+-rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240510.0/MediBot/MediPost.py
+-rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240510.0/MediBot/PDF_to_CSV_Cleaner.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240510.0/MediBot/__init__.py
+-rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240510.0/MediBot/update_json.py
+-rw-rw-rw-   0        0        0     2201 2024-05-10 01:26:20.000000 medicafe-0.240510.0/MediBot/update_medicafe.py
+drwxrwxrwx   0        0        0        0 2024-05-10 14:15:41.707000 medicafe-0.240510.0/MediLink/
+-rw-rw-rw-   0        0        0    18174 2024-05-08 01:57:26.000000 medicafe-0.240510.0/MediLink/MediLink.py
+-rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240510.0/MediLink/MediLink_277_decoder.py
+-rw-rw-rw-   0        0        0    19946 2024-05-08 01:52:49.000000 medicafe-0.240510.0/MediLink/MediLink_837p_encoder.py
+-rw-rw-rw-   0        0        0    35258 2024-05-09 01:32:35.000000 medicafe-0.240510.0/MediLink/MediLink_837p_encoder_library.py
+-rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240510.0/MediLink/MediLink_ConfigLoader.py
+-rw-rw-rw-   0        0        0    11166 2024-05-08 01:54:15.000000 medicafe-0.240510.0/MediLink/MediLink_DataMgmt.py
+-rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240510.0/MediLink/MediLink_Down.py
+-rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240510.0/MediLink/MediLink_ERA_decoder.py
+-rw-rw-rw-   0        0        0     6466 2024-05-10 03:43:36.000000 medicafe-0.240510.0/MediLink/MediLink_Gmail.py
+-rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240510.0/MediLink/MediLink_Scheduler.py
+-rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240510.0/MediLink/MediLink_StatusCheck.py
+-rw-rw-rw-   0        0        0     4942 2024-05-07 17:08:35.000000 medicafe-0.240510.0/MediLink/MediLink_UI.py
+-rw-rw-rw-   0        0        0     5904 2024-05-08 01:58:53.000000 medicafe-0.240510.0/MediLink/MediLink_Up.py
+-rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240510.0/MediLink/Soumit_api.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240510.0/MediLink/__init__.py
+-rw-rw-rw-   0        0        0      730 2024-05-10 14:15:41.909000 medicafe-0.240510.0/PKG-INFO
+-rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240510.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 14:15:41.892000 medicafe-0.240510.0/medicafe.egg-info/
+-rw-rw-rw-   0        0        0      730 2024-05-10 14:15:40.000000 medicafe-0.240510.0/medicafe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      978 2024-05-10 14:15:40.000000 medicafe-0.240510.0/medicafe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 14:15:40.000000 medicafe-0.240510.0/medicafe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240510.0/medicafe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       60 2024-05-10 14:15:40.000000 medicafe-0.240510.0/medicafe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-10 14:15:40.000000 medicafe-0.240510.0/medicafe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 14:15:41.922000 medicafe-0.240510.0/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2024-05-10 14:15:36.000000 medicafe-0.240510.0/setup.py
```

### Comparing `medicafe-0.240509.6/LICENSE` & `medicafe-0.240510.0/LICENSE`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.6/MediBot/MediBot.bat` & `medicafe-0.240510.0/MediBot/MediBot.bat`

 * *Files 3% similar despite different names*

```diff
@@ -37,18 +37,18 @@
     echo Configuration file missing.
     goto end_script
 )
 if exist "C:\Python34\Lib\site-packages\MediBot\upgrade_medicafe.py" (
     move "C:\Python34\Lib\site-packages\MediBot\upgrade_medicafe.py" "F:\Medibot\upgrade_medicafe.py" /y
 )
 
-:: Main menu
+:: Main menu, ECHO is Off is whats showing up.
 :main_menu
 cls
-echo !package_version!
+echo. !package_version!
 echo ---------------------------------------------
 echo         .//*  Welcome to MediCafe  *\\. 
 echo ---------------------------------------------
 echo.
 echo Please select an option:
 if "!internet_available!"=="0" (
     echo 1. Check for MediCafe Package Updates
@@ -88,14 +88,15 @@
     goto main_menu
 )
 echo Downloading emails...
 py "../MediLink/MediLink_Gmail.py" "%firefox_path%"
 if errorlevel 1 (
     echo Failed to download emails.
 ) else (
+    echo Calling CSV Processor...
     call :process_csvs
 )
 goto main_menu
 
 :: Run MediBot Flow
 :medibot_flow
 call :process_csvs
@@ -121,23 +122,26 @@
     set "minute=%%b"
     set "second=%%c"
 )
 set "timestamp=%DATE:~-4%%DATE:~3,2%%DATE:~0,2%_%hour%%minute%"
 set "latest_csv="
 for /f "delims=" %%a in ('dir /b /a-d /o-d "%source_folder%\*.csv" 2^>nul') do (
     set "latest_csv=%%a"
+    echo Found New CSV Files...
     goto process_found_csv
 )
 echo No new CSV files found.
 goto :eof
 
 :process_found_csv
+echo Processing CSVs...
 move "%source_folder%\!latest_csv!" "%target_folder%\SX_CSV_!timestamp!.csv"
 set "new_csv_path=%target_folder%\SX_CSV_!timestamp!.csv"
 py "%python_script%" "%config_file%" "!new_csv_path!"
+echo CSV Processor Complete...
 goto :eof
 
 :: Exit Script
 :end_script
 echo Exiting MediCafe.
 pause
 exit /b
```

### Comparing `medicafe-0.240509.6/MediBot/MediBot.py` & `medicafe-0.240510.0/MediBot/MediBot.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.6/MediBot/MediBot_Charges.py` & `medicafe-0.240510.0/MediBot/MediBot_Charges.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.6/MediBot/MediBot_Preprocessor.py` & `medicafe-0.240510.0/MediBot/MediBot_Preprocessor.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.6/MediBot/MediBot_Preprocessor_lib.py` & `medicafe-0.240510.0/MediBot/MediBot_Preprocessor_lib.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.6/MediBot/MediBot_UI.py` & `medicafe-0.240510.0/MediBot/MediBot_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.6/MediBot/MediBot_dataformat_library.py` & `medicafe-0.240510.0/MediBot/MediBot_dataformat_library.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,14 +60,17 @@
 
 def format_street(value, csv_data, reverse_mapping, parsed_address_components):
     app_control.set_pause_status(False)
     
     # Remove periods from the input (seems to be an XP-only issue?)
     value = value.replace('.', '')
     
+    # Remove APT for room, unique ident by using lead & trail space (TODO Consider alternatives)
+    value = value.replace(' APT ', ' ')
+    
     # Only proceed with parsing if a comma is present in the value
     if ',' in value:
         try:
             # Access the common cities from the loaded configuration
             common_cities = config.get('cities', [])
 
             # Convert cities to a case-insensitive regex pattern
```

### Comparing `medicafe-0.240509.6/MediBot/PDF_to_CSV_Cleaner.py` & `medicafe-0.240510.0/MediBot/PDF_to_CSV_Cleaner.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.6/MediBot/update_json.py` & `medicafe-0.240510.0/MediBot/update_json.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.6/MediBot/update_medicafe.py` & `medicafe-0.240510.0/MediBot/update_medicafe.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.6/MediLink/MediLink.py` & `medicafe-0.240510.0/MediLink/MediLink.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.6/MediLink/MediLink_277_decoder.py` & `medicafe-0.240510.0/MediLink/MediLink_277_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.6/MediLink/MediLink_837p_encoder.py` & `medicafe-0.240510.0/MediLink/MediLink_837p_encoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.6/MediLink/MediLink_837p_encoder_library.py` & `medicafe-0.240510.0/MediLink/MediLink_837p_encoder_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.6/MediLink/MediLink_ConfigLoader.py` & `medicafe-0.240510.0/MediLink/MediLink_ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.6/MediLink/MediLink_DataMgmt.py` & `medicafe-0.240510.0/MediLink/MediLink_DataMgmt.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.6/MediLink/MediLink_Down.py` & `medicafe-0.240510.0/MediLink/MediLink_Down.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.6/MediLink/MediLink_ERA_decoder.py` & `medicafe-0.240510.0/MediLink/MediLink_ERA_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.6/MediLink/MediLink_Gmail.py` & `medicafe-0.240510.0/MediLink/MediLink_Gmail.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.6/MediLink/MediLink_Scheduler.py` & `medicafe-0.240510.0/MediLink/MediLink_Scheduler.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.6/MediLink/MediLink_UI.py` & `medicafe-0.240510.0/MediLink/MediLink_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.6/MediLink/MediLink_Up.py` & `medicafe-0.240510.0/MediLink/MediLink_Up.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.6/PKG-INFO` & `medicafe-0.240510.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240509.6
+Version: 0.240510.0
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240509.6/README.md` & `medicafe-0.240510.0/README.md`

 * *Files identical despite different names*

### Comparing `medicafe-0.240509.6/medicafe.egg-info/PKG-INFO` & `medicafe-0.240510.0/medicafe.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240509.6
+Version: 0.240510.0
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240509.6/medicafe.egg-info/SOURCES.txt` & `medicafe-0.240510.0/medicafe.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 MediLink/MediLink_Down.py
 MediLink/MediLink_ERA_decoder.py
 MediLink/MediLink_Gmail.py
 MediLink/MediLink_Scheduler.py
 MediLink/MediLink_StatusCheck.py
 MediLink/MediLink_UI.py
 MediLink/MediLink_Up.py
-MediLink/MediLink_batch.bat
 MediLink/Soumit_api.py
 MediLink/__init__.py
 medicafe.egg-info/PKG-INFO
 medicafe.egg-info/SOURCES.txt
 medicafe.egg-info/dependency_links.txt
 medicafe.egg-info/not-zip-safe
 medicafe.egg-info/requires.txt
```

### Comparing `medicafe-0.240509.6/setup.py` & `medicafe-0.240510.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medicafe',
-    version="0.240509.6",
+    version="0.240510.0",
     description='MediCafe',
     long_description='This module ensures that MediCafe remains up-to-date by performing version checks for its dependencies on startup. It utilizes PyPI, the official repository for Python packages, to retrieve information about the latest available versions of the required packages. When an internet connection is available, MediUpdate automatically installs any available updates using pip, the package installer for Python.',
     long_description_content_type='text/markdown',
     keywords = 'medicafe python34 medibot medilink',
     url='https://github.com/katanada2',
     author='Daniel Vidaud',
     author_email='daniel@personalizedtransformation.com',
```

