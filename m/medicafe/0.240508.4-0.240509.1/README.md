# Comparing `tmp/medicafe-0.240508.4.tar.gz` & `tmp/medicafe-0.240509.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medicafe-0.240508.4.tar", last modified: Thu May  9 04:56:40 2024, max compression
+gzip compressed data, was "medicafe-0.240509.1.tar", last modified: Thu May  9 06:54:05 2024, max compression
```

## Comparing `medicafe-0.240508.4.tar` & `medicafe-0.240509.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 04:56:40.453000 medicafe-0.240508.4/
--rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240508.4/LICENSE
--rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240508.4/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-09 04:56:39.900000 medicafe-0.240508.4/MediBot/
--rwxrwxrwx   0        0        0     3614 2024-05-09 04:40:39.000000 medicafe-0.240508.4/MediBot/MediBot.bat
--rw-rw-rw-   0        0        0    16642 2024-05-09 04:47:15.000000 medicafe-0.240508.4/MediBot/MediBot.py
--rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240508.4/MediBot/MediBot_Charges.py
--rw-rw-rw-   0        0        0    32227 2024-05-09 04:18:08.000000 medicafe-0.240508.4/MediBot/MediBot_Preprocessor.py
--rw-rw-rw-   0        0        0     4652 2024-05-02 02:13:23.000000 medicafe-0.240508.4/MediBot/MediBot_Preprocessor_lib.py
--rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240508.4/MediBot/MediBot_UI.py
--rw-rw-rw-   0        0        0     6801 2024-05-09 04:53:21.000000 medicafe-0.240508.4/MediBot/MediBot_dataformat_library.py
--rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240508.4/MediBot/MediPost.py
--rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240508.4/MediBot/PDF_to_CSV_Cleaner.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240508.4/MediBot/__init__.py
--rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240508.4/MediBot/update_json.py
--rw-rw-rw-   0        0        0     1118 2024-05-09 02:39:09.000000 medicafe-0.240508.4/MediBot/update_medicafe.py
-drwxrwxrwx   0        0        0        0 2024-05-09 04:56:40.287000 medicafe-0.240508.4/MediLink/
--rw-rw-rw-   0        0        0    18174 2024-05-08 01:57:26.000000 medicafe-0.240508.4/MediLink/MediLink.py
--rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240508.4/MediLink/MediLink_277_decoder.py
--rw-rw-rw-   0        0        0    19946 2024-05-08 01:52:49.000000 medicafe-0.240508.4/MediLink/MediLink_837p_encoder.py
--rw-rw-rw-   0        0        0    35258 2024-05-09 01:32:35.000000 medicafe-0.240508.4/MediLink/MediLink_837p_encoder_library.py
--rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240508.4/MediLink/MediLink_ConfigLoader.py
--rw-rw-rw-   0        0        0    11166 2024-05-08 01:54:15.000000 medicafe-0.240508.4/MediLink/MediLink_DataMgmt.py
--rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240508.4/MediLink/MediLink_Down.py
--rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240508.4/MediLink/MediLink_ERA_decoder.py
--rw-rw-rw-   0        0        0     7063 2024-05-08 21:34:31.000000 medicafe-0.240508.4/MediLink/MediLink_Gmail.py
--rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240508.4/MediLink/MediLink_Scheduler.py
--rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240508.4/MediLink/MediLink_StatusCheck.py
--rw-rw-rw-   0        0        0     4942 2024-05-07 17:08:35.000000 medicafe-0.240508.4/MediLink/MediLink_UI.py
--rw-rw-rw-   0        0        0     5904 2024-05-08 01:58:53.000000 medicafe-0.240508.4/MediLink/MediLink_Up.py
--rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240508.4/MediLink/MediLink_batch.bat
--rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240508.4/MediLink/Soumit_api.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240508.4/MediLink/__init__.py
--rw-rw-rw-   0        0        0      730 2024-05-09 04:56:40.437000 medicafe-0.240508.4/PKG-INFO
--rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240508.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 04:56:40.422000 medicafe-0.240508.4/medicafe.egg-info/
--rw-rw-rw-   0        0        0      730 2024-05-09 04:56:39.000000 medicafe-0.240508.4/medicafe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1006 2024-05-09 04:56:39.000000 medicafe-0.240508.4/medicafe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 04:56:39.000000 medicafe-0.240508.4/medicafe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240508.4/medicafe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       60 2024-05-09 04:56:39.000000 medicafe-0.240508.4/medicafe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-09 04:56:39.000000 medicafe-0.240508.4/medicafe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 04:56:40.449000 medicafe-0.240508.4/setup.cfg
--rw-rw-rw-   0        0        0     1164 2024-05-09 04:56:38.000000 medicafe-0.240508.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 06:54:05.258000 medicafe-0.240509.1/
+-rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240509.1/LICENSE
+-rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240509.1/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-09 06:54:04.292000 medicafe-0.240509.1/MediBot/
+-rwxrwxrwx   0        0        0     3705 2024-05-09 05:26:10.000000 medicafe-0.240509.1/MediBot/MediBot.bat
+-rw-rw-rw-   0        0        0    17252 2024-05-09 06:49:38.000000 medicafe-0.240509.1/MediBot/MediBot.py
+-rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240509.1/MediBot/MediBot_Charges.py
+-rw-rw-rw-   0        0        0    33163 2024-05-09 06:49:01.000000 medicafe-0.240509.1/MediBot/MediBot_Preprocessor.py
+-rw-rw-rw-   0        0        0     4652 2024-05-02 02:13:23.000000 medicafe-0.240509.1/MediBot/MediBot_Preprocessor_lib.py
+-rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240509.1/MediBot/MediBot_UI.py
+-rw-rw-rw-   0        0        0     6840 2024-05-09 06:50:25.000000 medicafe-0.240509.1/MediBot/MediBot_dataformat_library.py
+-rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240509.1/MediBot/MediPost.py
+-rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240509.1/MediBot/PDF_to_CSV_Cleaner.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240509.1/MediBot/__init__.py
+-rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240509.1/MediBot/update_json.py
+-rw-rw-rw-   0        0        0     1118 2024-05-09 02:39:09.000000 medicafe-0.240509.1/MediBot/update_medicafe.py
+drwxrwxrwx   0        0        0        0 2024-05-09 06:54:04.964000 medicafe-0.240509.1/MediLink/
+-rw-rw-rw-   0        0        0    18174 2024-05-08 01:57:26.000000 medicafe-0.240509.1/MediLink/MediLink.py
+-rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240509.1/MediLink/MediLink_277_decoder.py
+-rw-rw-rw-   0        0        0    19946 2024-05-08 01:52:49.000000 medicafe-0.240509.1/MediLink/MediLink_837p_encoder.py
+-rw-rw-rw-   0        0        0    35258 2024-05-09 01:32:35.000000 medicafe-0.240509.1/MediLink/MediLink_837p_encoder_library.py
+-rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240509.1/MediLink/MediLink_ConfigLoader.py
+-rw-rw-rw-   0        0        0    11166 2024-05-08 01:54:15.000000 medicafe-0.240509.1/MediLink/MediLink_DataMgmt.py
+-rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240509.1/MediLink/MediLink_Down.py
+-rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240509.1/MediLink/MediLink_ERA_decoder.py
+-rw-rw-rw-   0        0        0     7063 2024-05-08 21:34:31.000000 medicafe-0.240509.1/MediLink/MediLink_Gmail.py
+-rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240509.1/MediLink/MediLink_Scheduler.py
+-rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240509.1/MediLink/MediLink_StatusCheck.py
+-rw-rw-rw-   0        0        0     4942 2024-05-07 17:08:35.000000 medicafe-0.240509.1/MediLink/MediLink_UI.py
+-rw-rw-rw-   0        0        0     5904 2024-05-08 01:58:53.000000 medicafe-0.240509.1/MediLink/MediLink_Up.py
+-rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240509.1/MediLink/MediLink_batch.bat
+-rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240509.1/MediLink/Soumit_api.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240509.1/MediLink/__init__.py
+-rw-rw-rw-   0        0        0      730 2024-05-09 06:54:05.240000 medicafe-0.240509.1/PKG-INFO
+-rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240509.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 06:54:05.219000 medicafe-0.240509.1/medicafe.egg-info/
+-rw-rw-rw-   0        0        0      730 2024-05-09 06:54:03.000000 medicafe-0.240509.1/medicafe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1006 2024-05-09 06:54:03.000000 medicafe-0.240509.1/medicafe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 06:54:03.000000 medicafe-0.240509.1/medicafe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240509.1/medicafe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       60 2024-05-09 06:54:03.000000 medicafe-0.240509.1/medicafe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-09 06:54:03.000000 medicafe-0.240509.1/medicafe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 06:54:05.254000 medicafe-0.240509.1/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2024-05-09 06:54:02.000000 medicafe-0.240509.1/setup.py
```

### Comparing `medicafe-0.240508.4/LICENSE` & `medicafe-0.240509.1/LICENSE`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.4/MediBot/MediBot.bat` & `medicafe-0.240509.1/MediBot/MediBot.bat`

 * *Files 6% similar despite different names*

```diff
@@ -29,34 +29,38 @@
     set "year=%%c"
 )
 set "datestamp=!month!!day!!year:~2,2!"
 
 :: Check if last update was performed today
 if "%last_update%"=="!datestamp!" (
     echo The Medicafe package was already updated today.
-    timeout /t 1 /nobreak >nul
+    ping -n 2 127.0.0.1 >nul
     goto :SKIP_UPDATE
 )
 
 :: Prompt user to check for update
 set /p check_update="Do you want to check for an update? (yes/no): "
 if /i "%check_update%"=="no" goto :SKIP_UPDATE
 
 :: Set PYTHONWARNINGS environment variable to ignore deprecation warnings
 set PYTHONWARNINGS=ignore
 
 :: Upgrade Medicafe package in a separate process and keep the window open after completion
 start "Upgrade Medicafe" cmd /k py "%upgrade_medicafe%" > upgrade_log.txt 2>&1
+
+:: Update the timestamp file with the current datestamp
+echo !datestamp! > "%temp_file%"
+
 exit /b
 
 :SKIP_UPDATE
 
 :: Check if user wants to force an update during the waiting period
 echo Press any key within 3 seconds to force an update anyway...
-timeout /t 3 /nobreak >nul
+ping -n 4 127.0.0.1 >nul
 if not errorlevel 1 (
     echo Forcing update...
     goto :FORCE_UPDATE
 )
 
 :: Continue script if no key pressed within 3 seconds
 echo Continuing script...
```

### Comparing `medicafe-0.240508.4/MediBot/MediBot.py` & `medicafe-0.240509.1/MediBot/MediBot.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,26 +99,29 @@
     try:
         value = ''
         if medisoft_field in parsed_address_components:
             value = parsed_address_components.get(medisoft_field, '')
         elif medisoft_field in fixed_values:
             value = fixed_values[medisoft_field][0]  # Use the fixed value
         elif medisoft_field in reverse_mapping:
+            if medisoft_field == "Ins1 Insurance ID" or reverse_mapping[medisoft_field] == "Primary Insurance Company":
+                MediLink_ConfigLoader.log("Detected {} or {}: {}".format(medisoft_field, reverse_mapping[medisoft_field], value))
             csv_header = reverse_mapping[medisoft_field]
             value = csv_row.get(csv_header, '')
 
         formatted_value = MediBot_dataformat_library.format_data(medisoft_field, value, csv_data, reverse_mapping, parsed_address_components) if value else 'Send, {Enter}'
         run_ahk_script(formatted_value)
 
         last_processed_entry = (medisoft_field, value)
         return 'continue', last_processed_entry
     except Exception as e:
         return handle_error(e, medisoft_field, last_processed_entry, csv_data)
 
 def handle_error(error, medisoft_field, last_processed_entry, csv_data):
+    MediLink_ConfigLoader.log("Error in process_field: ", e)
     print("An error occurred while processing {0}: {1}".format(medisoft_field, error))
     # Assuming the interaction mode is 'error' in this case
     interaction_mode = 'error'
     response = user_interaction(csv_data, interaction_mode, error, reverse_mapping)
     return response, last_processed_entry
 
 # iterating through each field defined in the field_mapping.
@@ -160,14 +163,15 @@
         action = iterate_fields(row, field_mapping, parsed_address_components, reverse_mapping, csv_data, fixed_values)
         # TODO (Low) add a feature here where if you accidentally started overwriting a patient that you could go back 2 patients.
         # Need to tell the user which patient we're talking about because it won't be obvious anymore.
         if action == -1:  # Retry
             continue  # Remain on the current row. 
         elif action == 1:  # Skip
             if current_row_index == len(csv_data) - 1:  # If it's the last row
+                MediLink_ConfigLoader.log("Reached the end of the patient list.")
                 print("Reached the end of the patient list. Looping back to the beginning.")
                 current_row_index = 0  # Reset to the first row
             else:
                 current_row_index += 1 # Move to the next row
             continue
         elif action == -2:  # Go back two patients and redo
             current_row_index = max(0, current_row_index - 2)  # Go back two rows, but not below 0
@@ -237,27 +241,29 @@
         else:
             # If no arguments are provided, use default paths
             config_path = default_config_path
             crosswalk_path = default_crosswalk_path
         
         e_state = ExecutionState(config_path, crosswalk_path)
         
-        #print("Loading CSV Data...")
+        MediLink_ConfigLoader.log("Loading CSV Data...")
         csv_data = MediBot_Preprocessor_lib.load_csv_data(CSV_FILE_PATH)
         
-        #print("Pre-processing CSV Data...")
-        MediBot_Preprocessor.preprocess_csv_data(csv_data, e_state.crosswalk)  # Pre-process CSV data to add combined fields & crosswalk values.
-        headers = csv_data[0].keys() # Including Patient Name and Patient Address
+        # Pre-process CSV data to add combined fields & crosswalk values.
+        MediLink_ConfigLoader.log("Pre-processing CSV Data...")
+        MediBot_Preprocessor.preprocess_csv_data(csv_data, e_state.crosswalk)  
+        headers = csv_data[0].keys() # Make sure all the headers are in place
         
-        #print("Performing Intake Scan...")
+        MediLink_ConfigLoader.log("Performing Intake Scan...")
         # identified_fields is an OrderedDict
         identified_fields = MediBot_Preprocessor.intake_scan(headers, field_mapping)
         
         # Reverse the identified_fields mapping for lookup
         reverse_mapping = {v: k for k, v in identified_fields.items()}
+        # MediLink_ConfigLoader.log("Reverse Mapping: {}".format(reverse_mapping))
 
         # CSV Patient Triage
         interaction_mode = 'triage'  # Start in triage mode
         error_message = ""  # This will be filled if an error has occurred
         #print("Debug - Identified fields mapping (main): {}".format(identified_fields)) # Debug Line
         
         proceed, selected_patient_ids, selected_indices, fixed_values = user_interaction(csv_data, interaction_mode, error_message, reverse_mapping)
@@ -302,14 +308,15 @@
             #        exit(1)
 
                 print("\nRemember, when in Medisoft:")
                 print("  Press 'F8'  to create a New Patient.")
                 print("  Press 'F12' to begin data entry.")
                 print("  Press 'F11' at any time to Pause.")
                 input("\n*** Press [Enter] when ready to begin! ***\n")
+                MediLink_ConfigLoader.log("Opening Medisoft...")
                 open_medisoft(app_control.get_medisoft_shortcut())
                 app_control.set_pause_status(True)
                 _ = manage_script_pause(csv_data, error_message, reverse_mapping)
                 data_entry_loop(csv_data, field_mapping, reverse_mapping, fixed_values)
                 cleanup()                
             else:
                 print("Data entry canceled by user. Exiting MediBot.")
```

### Comparing `medicafe-0.240508.4/MediBot/MediBot_Charges.py` & `medicafe-0.240509.1/MediBot/MediBot_Charges.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.4/MediBot/MediBot_Preprocessor.py` & `medicafe-0.240509.1/MediBot/MediBot_Preprocessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -413,14 +413,20 @@
         return False
 
     return True
 
 # CSV Preprocessor built for Carol
 def preprocess_csv_data(csv_data, crosswalk):
     try:
+        
+        # Add the "Ins1 Insurance ID" column header to the CSV data
+        # TODO Consider where all of this is getting done. I'm not sure this is the right place
+        for row in csv_data:
+            row['Ins1 Insurance ID'] = ''  # Initialize the column with empty values
+        
         # Filter out rows without a Patient ID
         csv_data[:] = [row for row in csv_data if row.get('Patient ID', '').strip()]
         
         # Remove Patients (rows) that are Primary Insurance: 'AETNA', 'AETNA MEDICARE', or 'HUMANA MED HMO'.
         csv_data[:] = [row for row in csv_data if row.get('Primary Insurance', '').strip() not in ['AETNA', 'AETNA MEDICARE', 'HUMANA MED HMO']]
                 
         # Convert 'Surgery Date' to datetime objects for sorting
@@ -482,24 +488,28 @@
                 elif row.get('Primary Insurance', '') == old_value:
                     row['Primary Insurance'] = new_value
 
             # TODO (Crosswalk Refactor) This is probably the wrong place to implement this? 
             # TODO (Crosswalk Bot Med) Also check to see if it's not overwriting the Medicare '1' assginment within triage.
             # Add a column with header "Ins1 Insurance ID" based on crosswalk and "Ins1 Payer ID" column for each row
             ins1_payer_id = row.get('Ins1 Payer ID', '').strip()  # Get the Ins1 Payer ID from the row
+            
+            MediLink_ConfigLoader.log("Ins1 Payer ID '{}' associated with Patient ID {}.".format(ins1_payer_id, row.get('Patient ID', "None")))
+            
             if ins1_payer_id:  # Check if Ins1 Payer ID is not empty
                 if ins1_payer_id in crosswalk.get('payer_id', {}):  # Check if Ins1 Payer ID exists in the crosswalk
                     # Get the corresponding medisoft_id(s) for the Ins1 Payer ID from the crosswalk
                     medisoft_ids = crosswalk['payer_id'][ins1_payer_id].get('medisoft_id', [])
                     if medisoft_ids:  # Check if medisoft_ids exist
                         # Convert medisoft_ids from strings to integers
                         medisoft_ids = [int(id) for id in medisoft_ids]
                         # TODO (Crosswalk Med) Default now is always Assign the first medisoft_id to the "Ins1 Insurance ID" column.
                         # This needs to be updated so try to match against Carol's naming convention to get a better match
                         row['Ins1 Insurance ID'] = medisoft_ids[0]
+                        MediLink_ConfigLoader.log("Ins1 Insurance ID '{}' used for Payer ID {} in crosswalk.".format(row.get('Ins1 Insurance ID', ''), ins1_payer_id))
                 else:
                     # TODO (Crosswalk Low) If Ins1 Payer ID is not found in the crosswalk then we should make a crosswalk_update entry for the new payer_id
                     # and then it should be passively looking for when the user updates one of these patients in Medisoft. This behavior
                     # should already be covered by the way crosswalk_update works or by the initializer or something, but the initialization
                     # is still pretty janky and I think it will miss older assignments if it doesn't basically do a full re-initialize each time. 
                     # Obviously diminishing returns on age of CSV.
                     MediLink_ConfigLoader.log("Ins1 Payer ID '{}' not found in the crosswalk.".format(ins1_payer_id))
@@ -534,21 +544,25 @@
     return existing_patients, patients_to_process
 
 def intake_scan(csv_headers, field_mapping):
     identified_fields = OrderedDict()
     missing_fields_warnings = []
     required_fields = config["required_fields"]
     
+    # MediLink_ConfigLoader.log("Intake Scan - Field Mapping: {}".format(field_mapping))
+    # MediLink_ConfigLoader.log("Intake Scan - CSV Headers: {}".format(csv_headers))
+    
     # Iterate over the Medisoft fields defined in field_mapping
     for medisoft_field in field_mapping.keys():
         for pattern in field_mapping[medisoft_field]:
             matched_headers = [header for header in csv_headers if re.search(pattern, header, re.IGNORECASE)]
             if matched_headers:
                 # Assuming the first matched header is the desired one
                 identified_fields[matched_headers[0]] = medisoft_field
+                # MediLink_ConfigLoader.log("Found Header: {}".format(identified_fields[matched_headers[0]]))
                 break
         else:
             # Check if the missing field is a required field before appending the warning
             if medisoft_field in required_fields:
                 missing_fields_warnings.append("WARNING: No matching CSV header found for Medisoft field '{0}'".format(medisoft_field))
    
    #-----------------------
```

### Comparing `medicafe-0.240508.4/MediBot/MediBot_Preprocessor_lib.py` & `medicafe-0.240509.1/MediBot/MediBot_Preprocessor_lib.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.4/MediBot/MediBot_UI.py` & `medicafe-0.240509.1/MediBot/MediBot_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.4/MediBot/MediBot_dataformat_library.py` & `medicafe-0.240509.1/MediBot/MediBot_dataformat_library.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,12 +148,12 @@
     elif medisoft_field == 'Secondary Policy Number':
         formatted_value = format_policy(value)
     elif medisoft_field == 'Primary Group Number':
         formatted_value = format_policy(value)
     elif medisoft_field == 'Secondary Group Number':
         formatted_value = format_policy(value)
     else:
-        formatted_value = value
+        formatted_value = str(value) # Ensure value is always a string
 
     formatted_value = formatted_value.replace(',', '{,}').replace(' ', '{Space}')
     ahk_command = 'SendInput, {}{{Enter}}'.format(formatted_value)
     return ahk_command
```

### Comparing `medicafe-0.240508.4/MediBot/PDF_to_CSV_Cleaner.py` & `medicafe-0.240509.1/MediBot/PDF_to_CSV_Cleaner.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.4/MediBot/update_json.py` & `medicafe-0.240509.1/MediBot/update_json.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.4/MediBot/update_medicafe.py` & `medicafe-0.240509.1/MediBot/update_medicafe.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.4/MediLink/MediLink.py` & `medicafe-0.240509.1/MediLink/MediLink.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.4/MediLink/MediLink_277_decoder.py` & `medicafe-0.240509.1/MediLink/MediLink_277_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.4/MediLink/MediLink_837p_encoder.py` & `medicafe-0.240509.1/MediLink/MediLink_837p_encoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.4/MediLink/MediLink_837p_encoder_library.py` & `medicafe-0.240509.1/MediLink/MediLink_837p_encoder_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.4/MediLink/MediLink_ConfigLoader.py` & `medicafe-0.240509.1/MediLink/MediLink_ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.4/MediLink/MediLink_DataMgmt.py` & `medicafe-0.240509.1/MediLink/MediLink_DataMgmt.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.4/MediLink/MediLink_Down.py` & `medicafe-0.240509.1/MediLink/MediLink_Down.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.4/MediLink/MediLink_ERA_decoder.py` & `medicafe-0.240509.1/MediLink/MediLink_ERA_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.4/MediLink/MediLink_Gmail.py` & `medicafe-0.240509.1/MediLink/MediLink_Gmail.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.4/MediLink/MediLink_Scheduler.py` & `medicafe-0.240509.1/MediLink/MediLink_Scheduler.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.4/MediLink/MediLink_UI.py` & `medicafe-0.240509.1/MediLink/MediLink_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.4/MediLink/MediLink_Up.py` & `medicafe-0.240509.1/MediLink/MediLink_Up.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.4/PKG-INFO` & `medicafe-0.240509.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240508.4
+Version: 0.240509.1
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240508.4/README.md` & `medicafe-0.240509.1/README.md`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.4/medicafe.egg-info/PKG-INFO` & `medicafe-0.240509.1/medicafe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240508.4
+Version: 0.240509.1
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240508.4/medicafe.egg-info/SOURCES.txt` & `medicafe-0.240509.1/medicafe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.4/setup.py` & `medicafe-0.240509.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medicafe',
-    version="0.240508.4",
+    version="0.240509.1",
     description='MediCafe',
     long_description='This module ensures that MediCafe remains up-to-date by performing version checks for its dependencies on startup. It utilizes PyPI, the official repository for Python packages, to retrieve information about the latest available versions of the required packages. When an internet connection is available, MediUpdate automatically installs any available updates using pip, the package installer for Python.',
     long_description_content_type='text/markdown',
     keywords = 'medicafe python34 medibot medilink',
     url='https://github.com/katanada2',
     author='Daniel Vidaud',
     author_email='daniel@personalizedtransformation.com',
```

