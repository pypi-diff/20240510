# Comparing `tmp/medicafe-0.240510.0.tar.gz` & `tmp/medicafe-0.240510.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medicafe-0.240510.0.tar", last modified: Fri May 10 14:15:41 2024, max compression
+gzip compressed data, was "medicafe-0.240510.1.tar", last modified: Fri May 10 17:30:22 2024, max compression
```

## Comparing `medicafe-0.240510.0.tar` & `medicafe-0.240510.1.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 14:15:41.926000 medicafe-0.240510.0/
--rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240510.0/LICENSE
--rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240510.0/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-10 14:15:41.266000 medicafe-0.240510.0/MediBot/
--rwxrwxrwx   0        0        0     4417 2024-05-10 13:17:05.000000 medicafe-0.240510.0/MediBot/MediBot.bat
--rw-rw-rw-   0        0        0    17252 2024-05-09 06:49:38.000000 medicafe-0.240510.0/MediBot/MediBot.py
--rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240510.0/MediBot/MediBot_Charges.py
--rw-rw-rw-   0        0        0    33163 2024-05-09 06:49:01.000000 medicafe-0.240510.0/MediBot/MediBot_Preprocessor.py
--rw-rw-rw-   0        0        0     4652 2024-05-02 02:13:23.000000 medicafe-0.240510.0/MediBot/MediBot_Preprocessor_lib.py
--rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240510.0/MediBot/MediBot_UI.py
--rw-rw-rw-   0        0        0     6985 2024-05-10 14:14:44.000000 medicafe-0.240510.0/MediBot/MediBot_dataformat_library.py
--rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240510.0/MediBot/MediPost.py
--rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240510.0/MediBot/PDF_to_CSV_Cleaner.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240510.0/MediBot/__init__.py
--rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240510.0/MediBot/update_json.py
--rw-rw-rw-   0        0        0     2201 2024-05-10 01:26:20.000000 medicafe-0.240510.0/MediBot/update_medicafe.py
-drwxrwxrwx   0        0        0        0 2024-05-10 14:15:41.707000 medicafe-0.240510.0/MediLink/
--rw-rw-rw-   0        0        0    18174 2024-05-08 01:57:26.000000 medicafe-0.240510.0/MediLink/MediLink.py
--rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240510.0/MediLink/MediLink_277_decoder.py
--rw-rw-rw-   0        0        0    19946 2024-05-08 01:52:49.000000 medicafe-0.240510.0/MediLink/MediLink_837p_encoder.py
--rw-rw-rw-   0        0        0    35258 2024-05-09 01:32:35.000000 medicafe-0.240510.0/MediLink/MediLink_837p_encoder_library.py
--rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240510.0/MediLink/MediLink_ConfigLoader.py
--rw-rw-rw-   0        0        0    11166 2024-05-08 01:54:15.000000 medicafe-0.240510.0/MediLink/MediLink_DataMgmt.py
--rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240510.0/MediLink/MediLink_Down.py
--rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240510.0/MediLink/MediLink_ERA_decoder.py
--rw-rw-rw-   0        0        0     6466 2024-05-10 03:43:36.000000 medicafe-0.240510.0/MediLink/MediLink_Gmail.py
--rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240510.0/MediLink/MediLink_Scheduler.py
--rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240510.0/MediLink/MediLink_StatusCheck.py
--rw-rw-rw-   0        0        0     4942 2024-05-07 17:08:35.000000 medicafe-0.240510.0/MediLink/MediLink_UI.py
--rw-rw-rw-   0        0        0     5904 2024-05-08 01:58:53.000000 medicafe-0.240510.0/MediLink/MediLink_Up.py
--rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240510.0/MediLink/Soumit_api.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240510.0/MediLink/__init__.py
--rw-rw-rw-   0        0        0      730 2024-05-10 14:15:41.909000 medicafe-0.240510.0/PKG-INFO
--rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240510.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 14:15:41.892000 medicafe-0.240510.0/medicafe.egg-info/
--rw-rw-rw-   0        0        0      730 2024-05-10 14:15:40.000000 medicafe-0.240510.0/medicafe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      978 2024-05-10 14:15:40.000000 medicafe-0.240510.0/medicafe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 14:15:40.000000 medicafe-0.240510.0/medicafe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240510.0/medicafe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       60 2024-05-10 14:15:40.000000 medicafe-0.240510.0/medicafe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-10 14:15:40.000000 medicafe-0.240510.0/medicafe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 14:15:41.922000 medicafe-0.240510.0/setup.cfg
--rw-rw-rw-   0        0        0     1164 2024-05-10 14:15:36.000000 medicafe-0.240510.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 17:30:22.215000 medicafe-0.240510.1/
+-rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240510.1/LICENSE
+-rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240510.1/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-10 17:30:21.470000 medicafe-0.240510.1/MediBot/
+-rwxrwxrwx   0        0        0     4417 2024-05-10 13:17:05.000000 medicafe-0.240510.1/MediBot/MediBot.bat
+-rw-rw-rw-   0        0        0    17252 2024-05-09 06:49:38.000000 medicafe-0.240510.1/MediBot/MediBot.py
+-rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240510.1/MediBot/MediBot_Charges.py
+-rw-rw-rw-   0        0        0    33448 2024-05-10 17:00:40.000000 medicafe-0.240510.1/MediBot/MediBot_Preprocessor.py
+-rw-rw-rw-   0        0        0     4652 2024-05-02 02:13:23.000000 medicafe-0.240510.1/MediBot/MediBot_Preprocessor_lib.py
+-rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240510.1/MediBot/MediBot_UI.py
+-rw-rw-rw-   0        0        0     6985 2024-05-10 14:14:44.000000 medicafe-0.240510.1/MediBot/MediBot_dataformat_library.py
+-rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240510.1/MediBot/MediPost.py
+-rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240510.1/MediBot/PDF_to_CSV_Cleaner.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240510.1/MediBot/__init__.py
+-rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240510.1/MediBot/update_json.py
+-rw-rw-rw-   0        0        0     2249 2024-05-10 14:22:15.000000 medicafe-0.240510.1/MediBot/update_medicafe.py
+drwxrwxrwx   0        0        0        0 2024-05-10 17:30:21.995000 medicafe-0.240510.1/MediLink/
+-rw-rw-rw-   0        0        0    18174 2024-05-08 01:57:26.000000 medicafe-0.240510.1/MediLink/MediLink.py
+-rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240510.1/MediLink/MediLink_277_decoder.py
+-rw-rw-rw-   0        0        0    20091 2024-05-10 16:47:58.000000 medicafe-0.240510.1/MediLink/MediLink_837p_encoder.py
+-rw-rw-rw-   0        0        0    35283 2024-05-10 17:28:21.000000 medicafe-0.240510.1/MediLink/MediLink_837p_encoder_library.py
+-rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240510.1/MediLink/MediLink_ConfigLoader.py
+-rw-rw-rw-   0        0        0    11166 2024-05-08 01:54:15.000000 medicafe-0.240510.1/MediLink/MediLink_DataMgmt.py
+-rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240510.1/MediLink/MediLink_Down.py
+-rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240510.1/MediLink/MediLink_ERA_decoder.py
+-rw-rw-rw-   0        0        0     6236 2024-05-10 16:45:40.000000 medicafe-0.240510.1/MediLink/MediLink_Gmail.py
+-rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240510.1/MediLink/MediLink_Scheduler.py
+-rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240510.1/MediLink/MediLink_StatusCheck.py
+-rw-rw-rw-   0        0        0     4942 2024-05-07 17:08:35.000000 medicafe-0.240510.1/MediLink/MediLink_UI.py
+-rw-rw-rw-   0        0        0     5904 2024-05-08 01:58:53.000000 medicafe-0.240510.1/MediLink/MediLink_Up.py
+-rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240510.1/MediLink/MediLink_batch.bat
+-rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240510.1/MediLink/Soumit_api.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240510.1/MediLink/__init__.py
+-rw-rw-rw-   0        0        0      730 2024-05-10 17:30:22.198000 medicafe-0.240510.1/PKG-INFO
+-rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240510.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 17:30:22.179000 medicafe-0.240510.1/medicafe.egg-info/
+-rw-rw-rw-   0        0        0      730 2024-05-10 17:30:20.000000 medicafe-0.240510.1/medicafe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1006 2024-05-10 17:30:20.000000 medicafe-0.240510.1/medicafe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 17:30:20.000000 medicafe-0.240510.1/medicafe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240510.1/medicafe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       60 2024-05-10 17:30:20.000000 medicafe-0.240510.1/medicafe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-10 17:30:20.000000 medicafe-0.240510.1/medicafe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 17:30:22.211000 medicafe-0.240510.1/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2024-05-10 17:30:19.000000 medicafe-0.240510.1/setup.py
```

### Comparing `medicafe-0.240510.0/LICENSE` & `medicafe-0.240510.1/LICENSE`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.0/MediBot/MediBot.bat` & `medicafe-0.240510.1/MediBot/MediBot.bat`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.0/MediBot/MediBot.py` & `medicafe-0.240510.1/MediBot/MediBot.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.0/MediBot/MediBot_Charges.py` & `medicafe-0.240510.1/MediBot/MediBot_Charges.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.0/MediBot/MediBot_Preprocessor.py` & `medicafe-0.240510.1/MediBot/MediBot_Preprocessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 - [ ] Implement logic to verify and match Patient IDs across different files to ensure data integrity before consolidation. (Catching errors between source data)
 - [ ] Optimize the preprocessing of surgery dates and diagnosis codes for use in patient billing and scheduling systems.
 - [ ] Read Surgery Schedule doc and parse out a Patient ID : Diagnosis Code table.
 - [ ] The Minutes & Cancellation data with logic to consolidate into one table in memory.
 - [ ] Dynamically list the endpoint for a new Payer ID via API or user interaction to update the crosswalk.json efficiently.
 - [ ] Pull listed addresses of insurance from the CSV. (Not really necessary)
 - [ ] Retroactively learn Medisoft insurance name and payerID from the provided data sources.
+- [ ] Middle Names should all be single letters. Make sure it gets truncated before submitting.
 
 Development Roadmap for crosswalk_update():
 - [X] Automation required for updating the crosswalk.json when new Medisoft insurance is discovered.
 - [X] New Medisoft insurances are identified based on the payer ID number.
 - [X] Check the existence of the payer ID in crosswalk.json under existing endpoints.
 - [X] Facilitate grouping of IDs for insurances like CIGNA with multiple addresses but few payer IDs.
 - [X] Retroactive learning based on selected insurances in Medisoft 
@@ -74,14 +75,16 @@
 - [ ] Integrate API checks to verify payer ID availability and related information.
 - [ ] Implement "Fax/Mail or Other" endpoint for unavailable payer IDs.
 - [ ] Present user with a list of top insurances for selection based on fuzzy search scores.
 - [ ] Establish payer ID to insurance ID relationship based on user selection.
 - [ ] Implicitly establish payer ID to endpoint mapping based on user selection.
 - [ ] Implement validation mechanisms to prevent incorrect mappings and ensure data integrity.
 - [ ] Considerations for extracting insurance addresses (if necessary)
+- [ ] Handle better the case where a payer_id doesn't exist (When Carol's CSV doesn't bring the Payer ID).
+        Maybe ask the user what the payer ID is for that patient? I dont know.
 """
 # Load configuration
 # Should this also take args? Path for ./MediLink needed to be added for this to resolve
 config, crosswalk = MediLink_ConfigLoader.load_configuration()
 
 class InitializationError(Exception):
     def __init__(self, message):
```

### Comparing `medicafe-0.240510.0/MediBot/MediBot_Preprocessor_lib.py` & `medicafe-0.240510.1/MediBot/MediBot_Preprocessor_lib.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.0/MediBot/MediBot_UI.py` & `medicafe-0.240510.1/MediBot/MediBot_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.0/MediBot/MediBot_dataformat_library.py` & `medicafe-0.240510.1/MediBot/MediBot_dataformat_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.0/MediBot/PDF_to_CSV_Cleaner.py` & `medicafe-0.240510.1/MediBot/PDF_to_CSV_Cleaner.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.0/MediBot/update_json.py` & `medicafe-0.240510.1/MediBot/update_json.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.0/MediBot/update_medicafe.py` & `medicafe-0.240510.1/MediBot/update_medicafe.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,21 +35,23 @@
                     print("Error: Upgrade failed. Details:")
                     print("stdout:", stdout)
                     print("stderr:", stderr)
                     sys.exit(1)
                 
                 progress_bar.update(total_progress // 2)  # Update progress bar
                 
-                # Add a one-second sleep between runs
-                time.sleep(1)
+                # Add a 5-second sleep between runs
+                time.sleep(5)
                 
             progress_bar.update(total_progress // 2)  # Update progress bar
             print("stdout:", stdout_accumulator.decode("utf-8"))
             print("stderr:", stderr_accumulator.decode("utf-8"))
+            time.sleep(1)
     except Exception as e:
         # Log any other exceptions
         print("Error:", e)
+        time.sleep(3)
         sys.exit(1)
 
 if __name__ == "__main__":
     medicafe_package = "medicafe"
     upgrade_medicafe(medicafe_package)
```

### Comparing `medicafe-0.240510.0/MediLink/MediLink.py` & `medicafe-0.240510.1/MediLink/MediLink.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.0/MediLink/MediLink_277_decoder.py` & `medicafe-0.240510.1/MediLink/MediLink_277_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.0/MediLink/MediLink_837p_encoder.py` & `medicafe-0.240510.1/MediLink/MediLink_837p_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 1. File Path Management: Enhance the handling of input paths to efficiently manage both individual files and directories, accommodating a range of file processing scenarios.
 2. User Interface Improvement: Advance the CLI for intuitive user interaction, offering clear options for file processing and real-time progress updates.
 3. Validation and Logging: Strengthen validation processes for input data, incorporating thorough checks against business rules and enhanced detailed logging for improved traceability and troubleshooting.
 4. Batch Processing and Output Handling: Enhance output file management to support efficient batch operations, including systematic naming and organization for output files.
 5. Comprehensive Documentation: Maintain up-to-date and detailed documentation within the codebase, ensuring all functions and complex logic are clearly explained.
 6. De-persisting Intermediate Files.
+7. Determination of Relationship to Patient for insurance holder. Can Compare Insured Name & closeness of DOB (usually spouse [2], child [3]). 
 """
 def create_interchange_elements(config, endpoint, transaction_set_control_number):
     """
     Create interchange headers and trailers for an 837P document.
 
     Parameters:
     - config: Configuration settings loaded from a JSON file.
```

### Comparing `medicafe-0.240510.0/MediLink/MediLink_837p_encoder_library.py` & `medicafe-0.240510.1/MediLink/MediLink_837p_encoder_library.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 """
 1. Code Refactoring: Increase modularity and clarity, particularly in segment creation functions (e.g., `create_st_segment`, `create_nm1_billing_provider_segment`), for better maintenance and readability.
 2. Endpoint Support: Extend support within segment creation for additional endpoints with attention to their unique claim submission requirements.
 3. Payer Identification Mechanism: Refine the mechanism for dynamically identifying payers, leveraging payer mappings and integrating with external APIs like Availity for precise payer information retrieval.
 4. Adherence to Endpoint-Specific Standards: Implement and verify the compliance of claim data formatting and inclusion based on the specific demands of each target endpoint within the segment creation logic.
 5. De-persisting Intermediate Files.
 6. Get an API for Optum "Entered As". 
+7. Authorization Number
 """
 
 # Converts date format from one format to another.
 def convert_date_format(date_str):
     # Parse the input date string into a datetime object using the input format    
     # Determine the input date format based on the length of the input string
     input_format = "%m-%d-%Y" if len(date_str) == 10 else "%m-%d-%y"
@@ -222,15 +223,16 @@
         if "JSON" in str(e) and "decode" in str(e):
             raise ValueError("Error decoding the crosswalk JSON file")
         else:
             raise e
 
 def fetch_payer_name_from_crosswalk(payer_id, config, endpoint):
     """
-    TODO (Low Crosswalk) This is the backup function for when Availity cant resolve the payer name.
+    TODO (Low Prioirty Crosswalk) This is the backup function for when Availity cant 
+    resolve the payer name.
     The best thing to do here would probably be to pull from Carol's CSV but maybe we 
     can start with trying to pull from MAINS and just use that as the default for now.
     For now, this is not make-work because Availity can resolve what we want right now.
     
     Retrieves the payer name corresponding to a given payer ID from a crosswalk mapping.
     
     Parameters:
@@ -238,37 +240,33 @@
     - config: Configuration dictionary including the path to the crosswalk JSON.
     
     Returns:
     - The payer name corresponding to the payer ID.
     
     Raises:
     - ValueError if the payer ID is not found in the crosswalk mapping.
-    """
-    # Ensure the 'crosswalkPath' key exists in config and contains the path to the crosswalk JSON file
-    if 'crosswalkPath' not in config:
-        raise ValueError("Crosswalk path not defined in configuration.")
-
-    crosswalk_path = config.get('crosswalkPath')
+    """   
+    # BUG this needs to be fully implemented. This is bad.
+    
     try:
-        with open(crosswalk_path, 'r') as file:
-            crosswalk_mappings = json.load(file) 
-            # BUG (Low ConfigLoader) This should be using ConfigLoader.
-        # Select the endpoint-specific section from the mappings
-        # This whole thing needs to be re-worked. Why again? I forgot.
-        endpoint_mappings = crosswalk_mappings['payer_id'].get(endpoint, {})
-        payer_name = endpoint_mappings.get(payer_id)
+        # _, crosswalk = MediLink_ConfigLoader.load_configuration()
+        
+        # This whole thing needs to be re-worked because there's no payer id names anymore in the crosswalk
+        # endpoint_mappings = crosswalk['payer_id']
+        payer_name = '' # endpoint_mappings.get(payer_id)
 
         if not payer_name:
-            raise ValueError("Payer name not found for payer ID: {} in {} mappings.".format(payer_id, endpoint))
-
+            # Prompt the user to input the payer name
+            payer_name = input("Payer name not found for payer ID {}. Please enter an approximate payer name: ".format(payer_id))
+            if not payer_name:
+                raise ValueError("No payer name provided.")
+        
         return payer_name
-    except FileNotFoundError:
-        raise FileNotFoundError("Crosswalk file not found at {}".format(crosswalk_path))
-    except json.JSONDecodeError as e:
-        raise ValueError("Error decoding the crosswalk JSON file: {}".format(e))
+    except ValueError as e:
+        raise ValueError("Error in fetch payer name: {}".format(e))
 
 def create_2010BB_payer_information_segment(parsed_data, config, endpoint):
     """
     Dynamically generates the NM1 segment for the payer in the 2010BB loop of an 837P transaction.
     This process involves mapping the insurance name to the correct payer ID and then resolving the payer name.
     The function prioritizes the Availity API for payer name resolution (currently the only API integrated) 
     and falls back to crosswalk mapping if necessary or when additional APIs are not available.
@@ -298,26 +296,26 @@
 
     payer_name = ''
     # Step 2: Attempt to Retrieve Payer Name from Availity API (current API integration)
     endpoint = 'availity' # Force availity API because none of the other ones are connected BUG
     if True: #endpoint.lower() == 'availity':
         try:
             payer_name = fetch_payer_name_from_api(payer_id, config, endpoint)
-            MediLink_ConfigLoader.log("Resolved payer name {} via {} API for Payer ID: {}".format(payer_name, endpoint, payer_id), config, level="INFO")
         except Exception as api_error:
             print("{} API call failed for Payer ID '{}': {}".format(endpoint, payer_id, api_error))
 
     # Placeholder for future API integrations with other endpoints
     # elif endpoint.lower() == 'optum':
     #     payer_name = fetch_payer_name_from_optum_api(payer_id, config)
     # elif endpoint.lower() == 'pnt_data':
     #     payer_name = fetch_payer_name_from_pnt_data_api(payer_id, config)
 
     # Step 3: Fallback to Crosswalk Mapping if API resolution fails or is not applicable
     if not payer_name:
+        MediLink_ConfigLoader.log("{} API call unresolved for Payer ID '{}', fetching from backup...".format(endpoint, payer_id))
         payer_name = fetch_payer_name_from_crosswalk(payer_id, config, endpoint)
 
     # Construct and return the NM1*PR segment for the 2010BB loop with the payer name and ID
     # Is this supposed to be PI instead of PR?
     return "NM1*PR*2*{}*****PI*{}~".format(payer_name, payer_id)
 
 def create_nm1_payto_address_segments(config):
@@ -431,14 +429,15 @@
         data = response.json()
         # print(data) DEBUG
                 
         # Check if 'payers' key exists and has at least one item
         if 'payers' in data and data['payers']:
             payer = data['payers'][0]
             payer_name = payer.get('displayName') or payer.get('name', 'No name available')
+            MediLink_ConfigLoader.log("Resolved payer name {} via {} API for Payer ID: {}".format(payer_name, endpoint, payer_id), config, level="INFO")
             return payer_name
         else:
             raise ValueError("No payer found for ID: {0}".format(payer_id))
     except requests.RequestException as e:
         print("Error fetching payer name: {0}".format(e))
         raise
 
@@ -478,14 +477,16 @@
 
     return sbr_segment
 
 def insurance_type_selection():
     """
     TODO (Med SBR09) Finish making this function. This should integrate into a menu for now and then figure 
     out the automated/API method to getting this.
+    This menu flow probably needs to be alongside the suggested endpoint flow and with default 
+    PPO (12), then CI, then FI as most common, followed by the rest. 
     
     11 - Other Non-Federal Programs
     12 - Preferred Provider Organization (PPO)
     13 - Point of Service (POS)
     14 - Exclusive Provider Organization (EPO)
     15 - Indemnity Insurance
     16 - Health Maintenance Organization (HMO) Medicare Risk
```

### Comparing `medicafe-0.240510.0/MediLink/MediLink_ConfigLoader.py` & `medicafe-0.240510.1/MediLink/MediLink_ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.0/MediLink/MediLink_DataMgmt.py` & `medicafe-0.240510.1/MediLink/MediLink_DataMgmt.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.0/MediLink/MediLink_Down.py` & `medicafe-0.240510.1/MediLink/MediLink_Down.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.0/MediLink/MediLink_ERA_decoder.py` & `medicafe-0.240510.1/MediLink/MediLink_ERA_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.0/MediLink/MediLink_Gmail.py` & `medicafe-0.240510.1/MediLink/MediLink_Gmail.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,63 @@
 """
-TODO All of this needs to get re-written to match the current implementation and the lessons learned.
-
-NOTE: Also download the surgery schedule. So sometimes it doesn't need the OTP.
-
-This script facilitates the process of accessing a notification email from Outlook 365, which contains a secure link to view a message. The script automates the retrieval of this link and the OTP sent by email to authenticate and access the content securely.
-
-**Challenges:**
-1. Extracting a 'Read the message' link from an email notification sent via Outlook 365.
-2. Monitoring Gmail programmatically for an OTP email sent as part of Microsoft's secure email authentication process.
-3. Using the OTP to authenticate and access the secured email content.
-4. Securely downloading an attachment (e.g., Carol's CSV with PHI data) directly from Microsoft's servers to the client machine without it ever passing through Google's servers.
-5. Handling potential errors and edge cases, such as delays in receiving the OTP email or issues with the link extraction.
-6. Ensuring HIPAA compliance in handling PHI data, especially during data transfer directly from Microsoft's secured environment.
-
-**Suggested Approach:**
-1. **Authentication and Accessing Gmail**: Use the Gmail API in a client-side Python script to monitor and extract necessary details (links and OTPs) from emails.
-2. **Extracting the 'Read the Message' Link**: Identify and extract the URL from the notification email which navigates to Microsoft's secure email portal.
-3. **Monitoring for the OTP**: Continuously check the Gmail inbox for an incoming OTP email following the initiation of the authentication process through the extracted link.
-4. **Using the OTP**: Use the OTP to complete the authentication process on the Microsoft portal and gain access to the secure content.
-5. **Downloading the Attachment**: Once authenticated, directly download the PHI-containing document from the Microsoft portal to the client machine, ensuring encryption and security throughout the transfer process.
-
-**Steps Involved:**
-1. Set up the Python client to monitor Gmail and interact with the Google Apps Script for initial link extraction.
-2. Extract the 'Read the message' link from the relevant email using the Google Apps Script.
-3. Use the Python client to handle user interactions required to navigate the Microsoft authentication portal, enter the OTP, and download the secured content.
-4. Ensure secure handling of all PHI data, with strong emphasis on HIPAA compliance throughout the process.
-
-**Breakdown:**
-
-**Python Script (Client Side)**
-- **Functionality**:
-    - Interface with the user to initiate the process.
-    - Monitor Gmail for emails that contain the secure link and OTP.
-    - Handle the navigation to the secure Microsoft portal and input the OTP.
-    - Directly download the secure content once access is granted.
-- **Libraries and APIs**:
-    - Google API Python Client to interact with Gmail.
-    - Requests for HTTP requests to handle link extraction and OTP monitoring.
-    - OS and Sys libraries for local system interactions.
-
-**Google Apps Script (Server Side)**
-- **Functionality**:
-    - Authenticate and access Gmail to extract the 'Read the message' link.
-    - Provide support for initial email filtering and link extraction.
-    - Not involved in the decryption or direct handling of PHI data to ensure compliance with HIPAA.
-
-This architecture ensures the system handles sensitive PHI data in compliance with HIPAA regulations while maintaining robust and reliable email processing and file handling mechanisms. All sensitive data transfers occur directly from Microsoft's secure environment, minimizing the risk of unauthorized access during transit.
-
-TODO (High GMail)
-
-Notes: So the XP system can't do auth natively outside a browser and the libraries available wouldnt be
-able to do auth on the fly so we'd basically be stuck getting tokens manually that only last an hour and 
-then copy pasting those into the script like a rotating key which is not very UX friendly. So, any of the interactions 
-necessary should move to an HTML page that's served by Google Apps Script so there's no "interaction" that has to 
-happen outside of the webapp/browser. The only thing XP can do is send pre-defined actions. So, basically the XP client-side 
-has to pretty much just be a URL to open. There essentially can't be any communication.
+This documentation outlines the current functionality and development insights of a Google Apps Script and associated 
+client-side Python script designed to facilitate the automated retrieval of secured content from emails. The system 
+enables users to extract links and one-time passwords (OTPs) from emails, initiating and managing secure email interactions 
+without manual intervention.
+
+**Current Functionality:**
+1. **Google Apps Script (Server-side)**:
+    - Handles HTTP GET requests, routing them based on the 'action' parameter to perform tasks like retrieving stored 
+        OTPs, extracting links from emails, and retrieving email subjects for user selection.
+    - Utilizes Gmail search queries to find relevant emails based on sender and date criteria, then extracts data like 
+        subjects or specific links contained within these emails.
+    - Supports interactive selection of emails via a web app, allowing users to choose an email from a list and extract 
+        a specific link.
+    - Employs properties service to store and retrieve data like links and OTPs securely.
+
+2. **HTML Client (Server-side)**:
+    - Provides a user interface for selecting emails from a list, triggered by server-side scripts.
+    - Includes JavaScript to handle client-server communication and user interactions, such as selecting an email and 
+        extracting a link.
+
+3. **Python Script (Client-side)**:
+    - Interfaces with the server-side web app to initiate processes like link retrieval.
+    - Manages opening URLs in the user's browser, allowing for interaction with the web app directly from the client-side 
+        environment.
+
+**Future Work:**
+- [ ] Implement and troubleshoot the OTP extraction and validation system to fully automate the secured content retrieval process.
+- [X] Gmail Server-side Authentication flow & Webapp build
+- [X] Upgrade to handle multiple possible emails selection
+- [ ] Augment to detect Surgery Schedule emails with doc attachments that don't require OTP.
+- [X] Upgrade Gmail query to only get emails with the protected links.
+- [ ] Something that goes here that I forgot.
+
+**Technical Challenges and Solutions:**
+1. **Authentication Limitations on XP Systems:**
+    - **Challenge:** The XP operating system could not perform authentication natively outside a browser, and available 
+        libraries were not capable of handling dynamic authentication.
+    - **Solution:** We centralized all user interactions within an HTML page served by Google Apps Script, thereby 
+        eliminating the need for complex client-side operations. The client-side script was simplified to merely opening URLs, reducing the complexity and potential for errors.
+
+2. **Secure Data Handling:**
+    - **Challenge:** Initially, handling sensitive data such as OTPs and integrating with O365 protected emails was complex 
+        due to security requirements and the transient nature of such data. The solution had to accommodate the specific 
+        security protocols of Microsoft's environment without direct interaction.
+    - **Solution:** Utilizing Google Apps Script’s property service to store OTPs temporarily and securely. Additionally, 
+        we addressed O365 integration by ensuring the browser handled email links directly, respecting Microsoft's security 
+        constraints like x-frame options, thus maintaining functionality without compromising security.
+
+3. **User Interaction and Workflow Streamlining:**
+    - **Challenge:** Managing the workflow from email selection to secure content access required multiple steps that could 
+        potentially confuse the user. The application also had to be efficient under low-bandwidth constraints, and initially, 
+        XP could not download attachments directly, requiring manual user intervention.
+    - **Solution:** The introduction of an interactive web app interface enabled users to select emails directly through a 
+        user-friendly list, significantly simplifying the workflow and minimizing user errors. This method also streamlined 
+        the process, making it suitable for low-bandwidth environments and circumventing the need for full email client loads.
 """
 import sys
 import subprocess
 import webbrowser
 from MediLink_ConfigLoader import log
 
 def open_browser_with_executable(url, browser_path=None):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `medicafe-0.240510.0/MediLink/MediLink_Scheduler.py` & `medicafe-0.240510.1/MediLink/MediLink_Scheduler.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.0/MediLink/MediLink_UI.py` & `medicafe-0.240510.1/MediLink/MediLink_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.0/MediLink/MediLink_Up.py` & `medicafe-0.240510.1/MediLink/MediLink_Up.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.0/PKG-INFO` & `medicafe-0.240510.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240510.0
+Version: 0.240510.1
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240510.0/README.md` & `medicafe-0.240510.1/README.md`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.0/medicafe.egg-info/PKG-INFO` & `medicafe-0.240510.1/medicafe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240510.0
+Version: 0.240510.1
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240510.0/medicafe.egg-info/SOURCES.txt` & `medicafe-0.240510.1/medicafe.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 MediLink/MediLink_Down.py
 MediLink/MediLink_ERA_decoder.py
 MediLink/MediLink_Gmail.py
 MediLink/MediLink_Scheduler.py
 MediLink/MediLink_StatusCheck.py
 MediLink/MediLink_UI.py
 MediLink/MediLink_Up.py
+MediLink/MediLink_batch.bat
 MediLink/Soumit_api.py
 MediLink/__init__.py
 medicafe.egg-info/PKG-INFO
 medicafe.egg-info/SOURCES.txt
 medicafe.egg-info/dependency_links.txt
 medicafe.egg-info/not-zip-safe
 medicafe.egg-info/requires.txt
```

### Comparing `medicafe-0.240510.0/setup.py` & `medicafe-0.240510.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medicafe',
-    version="0.240510.0",
+    version="0.240510.1",
     description='MediCafe',
     long_description='This module ensures that MediCafe remains up-to-date by performing version checks for its dependencies on startup. It utilizes PyPI, the official repository for Python packages, to retrieve information about the latest available versions of the required packages. When an internet connection is available, MediUpdate automatically installs any available updates using pip, the package installer for Python.',
     long_description_content_type='text/markdown',
     keywords = 'medicafe python34 medibot medilink',
     url='https://github.com/katanada2',
     author='Daniel Vidaud',
     author_email='daniel@personalizedtransformation.com',
```

