# Comparing `tmp/medicafe-0.240515.4.tar.gz` & `tmp/medicafe-0.240515.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medicafe-0.240515.4.tar", last modified: Thu May 16 00:43:24 2024, max compression
+gzip compressed data, was "medicafe-0.240515.5.tar", last modified: Thu May 16 01:38:55 2024, max compression
```

## Comparing `medicafe-0.240515.4.tar` & `medicafe-0.240515.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 00:43:24.792000 medicafe-0.240515.4/
--rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240515.4/LICENSE
--rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240515.4/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-16 00:43:23.904000 medicafe-0.240515.4/MediBot/
--rwxrwxrwx   0        0        0     5972 2024-05-12 18:02:44.000000 medicafe-0.240515.4/MediBot/MediBot.bat
--rw-rw-rw-   0        0        0    17490 2024-05-15 17:01:43.000000 medicafe-0.240515.4/MediBot/MediBot.py
--rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240515.4/MediBot/MediBot_Charges.py
--rw-rw-rw-   0        0        0    14538 2024-05-15 19:07:33.000000 medicafe-0.240515.4/MediBot/MediBot_Crosswalk_Library.py
--rw-rw-rw-   0        0        0    14906 2024-05-15 16:48:28.000000 medicafe-0.240515.4/MediBot/MediBot_Preprocessor.py
--rw-rw-rw-   0        0        0    17184 2024-05-15 17:38:32.000000 medicafe-0.240515.4/MediBot/MediBot_Preprocessor_lib.py
--rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240515.4/MediBot/MediBot_UI.py
--rw-rw-rw-   0        0        0     8912 2024-05-15 20:14:35.000000 medicafe-0.240515.4/MediBot/MediBot_dataformat_library.py
--rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240515.4/MediBot/MediPost.py
--rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240515.4/MediBot/PDF_to_CSV_Cleaner.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240515.4/MediBot/__init__.py
--rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240515.4/MediBot/update_json.py
--rw-rw-rw-   0        0        0     2249 2024-05-10 17:47:37.000000 medicafe-0.240515.4/MediBot/update_medicafe.py
-drwxrwxrwx   0        0        0        0 2024-05-16 00:43:24.534000 medicafe-0.240515.4/MediLink/
--rw-rw-rw-   0        0        0    20303 2024-05-15 19:29:00.000000 medicafe-0.240515.4/MediLink/MediLink.py
--rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240515.4/MediLink/MediLink_277_decoder.py
--rw-rw-rw-   0        0        0    25526 2024-05-16 00:37:08.000000 medicafe-0.240515.4/MediLink/MediLink_837p_encoder.py
--rw-rw-rw-   0        0        0    43551 2024-05-16 00:36:51.000000 medicafe-0.240515.4/MediLink/MediLink_837p_encoder_library.py
--rw-rw-rw-   0        0        0     6166 2024-05-15 17:49:28.000000 medicafe-0.240515.4/MediLink/MediLink_APIs.py
--rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240515.4/MediLink/MediLink_ConfigLoader.py
--rw-rw-rw-   0        0        0    12235 2024-05-14 15:14:04.000000 medicafe-0.240515.4/MediLink/MediLink_DataMgmt.py
--rw-rw-rw-   0        0        0     7248 2024-05-15 07:47:12.000000 medicafe-0.240515.4/MediLink/MediLink_Down.py
--rw-rw-rw-   0        0        0     8710 2024-05-15 13:36:03.000000 medicafe-0.240515.4/MediLink/MediLink_ERA_decoder.py
--rw-rw-rw-   0        0        0     6236 2024-05-10 16:45:40.000000 medicafe-0.240515.4/MediLink/MediLink_Gmail.py
--rw-rw-rw-   0        0        0      370 2024-05-14 22:24:45.000000 medicafe-0.240515.4/MediLink/MediLink_Mailer.py
--rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240515.4/MediLink/MediLink_Scheduler.py
--rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240515.4/MediLink/MediLink_StatusCheck.py
--rw-rw-rw-   0        0        0     5181 2024-05-12 16:36:09.000000 medicafe-0.240515.4/MediLink/MediLink_UI.py
--rw-rw-rw-   0        0        0    19252 2024-05-15 13:35:59.000000 medicafe-0.240515.4/MediLink/MediLink_Up.py
--rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240515.4/MediLink/MediLink_batch.bat
--rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240515.4/MediLink/Soumit_api.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240515.4/MediLink/__init__.py
--rw-rw-rw-   0        0        0     3108 2024-05-13 04:52:22.000000 medicafe-0.240515.4/MediLink/test.py
--rw-rw-rw-   0        0        0     4396 2024-05-16 00:43:24.775000 medicafe-0.240515.4/PKG-INFO
--rw-rw-rw-   0        0        0     2960 2024-05-13 07:31:39.000000 medicafe-0.240515.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 00:43:24.752000 medicafe-0.240515.4/medicafe.egg-info/
--rw-rw-rw-   0        0        0     4396 2024-05-16 00:43:23.000000 medicafe-0.240515.4/medicafe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1114 2024-05-16 00:43:23.000000 medicafe-0.240515.4/medicafe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 00:43:23.000000 medicafe-0.240515.4/medicafe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240515.4/medicafe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       60 2024-05-16 00:43:23.000000 medicafe-0.240515.4/medicafe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-16 00:43:23.000000 medicafe-0.240515.4/medicafe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 00:43:24.787000 medicafe-0.240515.4/setup.cfg
--rw-rw-rw-   0        0        0     4834 2024-05-16 00:43:19.000000 medicafe-0.240515.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 01:38:55.685000 medicafe-0.240515.5/
+-rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240515.5/LICENSE
+-rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240515.5/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-16 01:38:54.728000 medicafe-0.240515.5/MediBot/
+-rwxrwxrwx   0        0        0     5972 2024-05-12 18:02:44.000000 medicafe-0.240515.5/MediBot/MediBot.bat
+-rw-rw-rw-   0        0        0    17490 2024-05-15 17:01:43.000000 medicafe-0.240515.5/MediBot/MediBot.py
+-rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240515.5/MediBot/MediBot_Charges.py
+-rw-rw-rw-   0        0        0    14538 2024-05-15 19:07:33.000000 medicafe-0.240515.5/MediBot/MediBot_Crosswalk_Library.py
+-rw-rw-rw-   0        0        0    14906 2024-05-15 16:48:28.000000 medicafe-0.240515.5/MediBot/MediBot_Preprocessor.py
+-rw-rw-rw-   0        0        0    17184 2024-05-15 17:38:32.000000 medicafe-0.240515.5/MediBot/MediBot_Preprocessor_lib.py
+-rw-rw-rw-   0        0        0    10660 2024-05-16 01:23:48.000000 medicafe-0.240515.5/MediBot/MediBot_UI.py
+-rw-rw-rw-   0        0        0     8912 2024-05-15 20:14:35.000000 medicafe-0.240515.5/MediBot/MediBot_dataformat_library.py
+-rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240515.5/MediBot/MediPost.py
+-rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240515.5/MediBot/PDF_to_CSV_Cleaner.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240515.5/MediBot/__init__.py
+-rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240515.5/MediBot/update_json.py
+-rw-rw-rw-   0        0        0     2249 2024-05-10 17:47:37.000000 medicafe-0.240515.5/MediBot/update_medicafe.py
+drwxrwxrwx   0        0        0        0 2024-05-16 01:38:55.434000 medicafe-0.240515.5/MediLink/
+-rw-rw-rw-   0        0        0    20316 2024-05-16 01:29:43.000000 medicafe-0.240515.5/MediLink/MediLink.py
+-rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240515.5/MediLink/MediLink_277_decoder.py
+-rw-rw-rw-   0        0        0    25526 2024-05-16 00:37:08.000000 medicafe-0.240515.5/MediLink/MediLink_837p_encoder.py
+-rw-rw-rw-   0        0        0    43551 2024-05-16 00:36:51.000000 medicafe-0.240515.5/MediLink/MediLink_837p_encoder_library.py
+-rw-rw-rw-   0        0        0     6166 2024-05-15 17:49:28.000000 medicafe-0.240515.5/MediLink/MediLink_APIs.py
+-rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240515.5/MediLink/MediLink_ConfigLoader.py
+-rw-rw-rw-   0        0        0    12235 2024-05-14 15:14:04.000000 medicafe-0.240515.5/MediLink/MediLink_DataMgmt.py
+-rw-rw-rw-   0        0        0     7248 2024-05-15 07:47:12.000000 medicafe-0.240515.5/MediLink/MediLink_Down.py
+-rw-rw-rw-   0        0        0     8710 2024-05-15 13:36:03.000000 medicafe-0.240515.5/MediLink/MediLink_ERA_decoder.py
+-rw-rw-rw-   0        0        0     6236 2024-05-10 16:45:40.000000 medicafe-0.240515.5/MediLink/MediLink_Gmail.py
+-rw-rw-rw-   0        0        0      370 2024-05-14 22:24:45.000000 medicafe-0.240515.5/MediLink/MediLink_Mailer.py
+-rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240515.5/MediLink/MediLink_Scheduler.py
+-rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240515.5/MediLink/MediLink_StatusCheck.py
+-rw-rw-rw-   0        0        0     5181 2024-05-12 16:36:09.000000 medicafe-0.240515.5/MediLink/MediLink_UI.py
+-rw-rw-rw-   0        0        0    19286 2024-05-16 01:21:31.000000 medicafe-0.240515.5/MediLink/MediLink_Up.py
+-rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240515.5/MediLink/MediLink_batch.bat
+-rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240515.5/MediLink/Soumit_api.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240515.5/MediLink/__init__.py
+-rw-rw-rw-   0        0        0     3108 2024-05-13 04:52:22.000000 medicafe-0.240515.5/MediLink/test.py
+-rw-rw-rw-   0        0        0     4396 2024-05-16 01:38:55.664000 medicafe-0.240515.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2960 2024-05-13 07:31:39.000000 medicafe-0.240515.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 01:38:55.641000 medicafe-0.240515.5/medicafe.egg-info/
+-rw-rw-rw-   0        0        0     4396 2024-05-16 01:38:53.000000 medicafe-0.240515.5/medicafe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1114 2024-05-16 01:38:54.000000 medicafe-0.240515.5/medicafe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 01:38:53.000000 medicafe-0.240515.5/medicafe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240515.5/medicafe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       60 2024-05-16 01:38:53.000000 medicafe-0.240515.5/medicafe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-16 01:38:53.000000 medicafe-0.240515.5/medicafe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 01:38:55.680000 medicafe-0.240515.5/setup.cfg
+-rw-rw-rw-   0        0        0     4834 2024-05-16 01:38:52.000000 medicafe-0.240515.5/setup.py
```

### Comparing `medicafe-0.240515.4/LICENSE` & `medicafe-0.240515.5/LICENSE`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.4/MediBot/MediBot.bat` & `medicafe-0.240515.5/MediBot/MediBot.bat`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.4/MediBot/MediBot.py` & `medicafe-0.240515.5/MediBot/MediBot.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.4/MediBot/MediBot_Charges.py` & `medicafe-0.240515.5/MediBot/MediBot_Charges.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.4/MediBot/MediBot_Crosswalk_Library.py` & `medicafe-0.240515.5/MediBot/MediBot_Crosswalk_Library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.4/MediBot/MediBot_Preprocessor.py` & `medicafe-0.240515.5/MediBot/MediBot_Preprocessor.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.4/MediBot/MediBot_Preprocessor_lib.py` & `medicafe-0.240515.5/MediBot/MediBot_Preprocessor_lib.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.4/MediBot/MediBot_UI.py` & `medicafe-0.240515.5/MediBot/MediBot_UI.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 
             patient_id_header = reverse_mapping['Patient ID #2']
             patient_name_header = reverse_mapping['Patient Name']
             patient_id = row.get(patient_id_header, "N/A")
             patient_name = row.get(patient_name_header, "Unknown")
             surgery_date = row.get('Surgery Date', "Unknown Date")  # Access 'Surgery Date' as string directly from the row
             
-            print("{0:02d}: {3:.5s} (ID: {2}) {1} ".format(index+1, patient_name, patient_id, surgery_date))
+            print("{0:03d}: {3:.5s} (ID: {2}) {1} ".format(index+1, patient_name, patient_id, surgery_date))
 
             displayed_indices.append(index)
             displayed_patient_ids.append(patient_id)
 
         return displayed_indices, displayed_patient_ids
 
     if proceed_as_medicare:
```

### Comparing `medicafe-0.240515.4/MediBot/MediBot_dataformat_library.py` & `medicafe-0.240515.5/MediBot/MediBot_dataformat_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.4/MediBot/PDF_to_CSV_Cleaner.py` & `medicafe-0.240515.5/MediBot/PDF_to_CSV_Cleaner.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.4/MediBot/update_json.py` & `medicafe-0.240515.5/MediBot/update_json.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.4/MediBot/update_medicafe.py` & `medicafe-0.240515.5/MediBot/update_medicafe.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.4/MediLink/MediLink.py` & `medicafe-0.240515.5/MediLink/MediLink.py`

 * *Files 0% similar despite different names*

```diff
@@ -311,15 +311,15 @@
     config, crosswalk = MediLink_ConfigLoader.load_configuration() 
     
     # Check to make sure payer_id key is available in crosswalk, otherwise, go through that crosswalk initialization flow
     MediBot_Crosswalk_Library.check_and_initialize_crosswalk(config)
     
     # Check if the application is in test mode
     if config.get("MediLink_Config", {}).get("TestMode", False):
-        print("MEDILINK TEST MODE: To enable full functionality, please update the config file and set 'TestMode' to 'false'.")
+        print("\n--- MEDILINK TEST MODE --- \nTo enable full functionality, please update the config file \nand set 'TestMode' to 'false'.")
     
     # Display Welcome Message
     MediLink_UI.display_welcome()
 
     # Normalize the directory path for file operations.
     directory_path = os.path.normpath(config['MediLink_Config']['inputFilePath'])
```

### Comparing `medicafe-0.240515.4/MediLink/MediLink_277_decoder.py` & `medicafe-0.240515.5/MediLink/MediLink_277_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.4/MediLink/MediLink_837p_encoder.py` & `medicafe-0.240515.5/MediLink/MediLink_837p_encoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.4/MediLink/MediLink_837p_encoder_library.py` & `medicafe-0.240515.5/MediLink/MediLink_837p_encoder_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.4/MediLink/MediLink_APIs.py` & `medicafe-0.240515.5/MediLink/MediLink_APIs.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.4/MediLink/MediLink_ConfigLoader.py` & `medicafe-0.240515.5/MediLink/MediLink_ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.4/MediLink/MediLink_DataMgmt.py` & `medicafe-0.240515.5/MediLink/MediLink_DataMgmt.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.4/MediLink/MediLink_Down.py` & `medicafe-0.240515.5/MediLink/MediLink_Down.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.4/MediLink/MediLink_ERA_decoder.py` & `medicafe-0.240515.5/MediLink/MediLink_ERA_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.4/MediLink/MediLink_Gmail.py` & `medicafe-0.240515.5/MediLink/MediLink_Gmail.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.4/MediLink/MediLink_Scheduler.py` & `medicafe-0.240515.5/MediLink/MediLink_Scheduler.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.4/MediLink/MediLink_UI.py` & `medicafe-0.240515.5/MediLink/MediLink_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.4/MediLink/MediLink_Up.py` & `medicafe-0.240515.5/MediLink/MediLink_Up.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,24 +185,18 @@
     # Save the receipt to a text file
     save_receipt_to_file(receipt_content, config)
     
     # Probably return receipt_data since its the easier to use dictionary
     return receipt_data
 
 def prepare_receipt_data(submission_results):
-    # Perform any necessary data processing to prepare the submission results for the receipt
-    # This includes extracting from a multi-patient 837p the patient names, dates of service, amounts billed.
-    # Also the date & time of batch claim submission from the header segment. 
-    # Get the receiver name from the 1000B receiver name segment (will be common for that file).
-    # Organize the data in dictionary by endpoint (receiver name) and then patient information.
-    # This function should completely fill out the dictionary with the necessary information for the receipt. 
     """
     Prepare submission results for a receipt, including data from both successful and failed submissions.
     
-    This function extracts patient names, dates of service, and amounts billed from an 837p file.
+    This function extracts patient names, dates of service, amounts billed, and insurance names from an 837p file.
     It also includes the date and time of batch claim submission, and the receiver name from the 1000B segment.
     Data is organized by receiver name and includes both successful and failed submissions.
     
     Parameters:
     - submission_results (dict): Contains submission results grouped by endpoint, with success status.
     
     Returns:
@@ -230,15 +224,15 @@
     return receipt_data
 
 def validate_data(receipt_data):
     # Simple validation to check if data fields are correctly populated
     for endpoint, data in receipt_data.items():
         patients = data.get("patients", [])
         for index, patient in enumerate(patients, start=1):
-            missing_fields = [field for field in ('name', 'service_date', 'amount_billed', 'success') if not patient.get(field)]
+            missing_fields = [field for field in ('name', 'service_date', 'amount_billed', 'insurance_name', 'success') if not patient.get(field)]
             
             if missing_fields:
                 # Log the missing fields without revealing PHI
                 log("Receipt Data validation error for endpoint '{}', patient {}: Missing information in fields: {}".format(endpoint, index, ", ".join(missing_fields)))
     return True
 
 def parse_837p_file(file_path):
@@ -283,50 +277,68 @@
             for record in patient_records:
                 # Extract patient name
                 name_match = re.search(r'NM1\*IL\*1\*([^*]+)\*([^*]+)\*([^*]*)', record)
                 # Extract service date
                 service_date_match = re.search(r'DTP\*472\D*8\*([0-9]{8})', record)
                 # Extract claim amount
                 amount_match = re.search(r'CLM\*[^\*]*\*([0-9]+\.?[0-9]*)', record)
+                # Extract insurance name (payer_name)
+                insurance_name_match = re.search(r'NM1\*PR\*2\*([^*]+)\*', record)
                 
                 if name_match and service_date_match and amount_match:
                     # Handle optional middle name
                     middle_name = name_match.group(3).strip() if name_match.group(3) else ""
                     patient_name = "{} {} {}".format(name_match.group(2), middle_name, name_match.group(1)).strip()
                     service_date = "{}-{}-{}".format(service_date_match.group(1)[:4], service_date_match.group(1)[4:6], service_date_match.group(1)[6:])
                     amount_billed = float(amount_match.group(1))
+                    insurance_name = insurance_name_match.group(1)
                     
                     patient_details.append({
                         "name": patient_name,
                         "service_date": service_date,
-                        "amount_billed": amount_billed
+                        "amount_billed": amount_billed,
+                        "insurance_name": insurance_name
                     })
     except Exception as e:
         print("Error reading or parsing the 837p file: {0}".format(str(e)))
     
-    # Optionally, return also date_of_submission as a separate variable  
     return patient_details, date_of_submission
 
 def build_receipt_content(receipt_data):
+    """
+    Build the receipt content in a human-readable ASCII format with a tabular data presentation for patient information.
+
+    Args:
+        receipt_data (dict): Dictionary containing receipt data with patient details.
+
+    Returns:
+        str: Formatted receipt content as a string.
+    """
     # Build the receipt content in a human-readable ASCII format
-    # Improved layout with tabular data presentation for patient information
-    receipt_lines = ["Submission Receipt", "="*60, ""]  # Header
+    receipt_lines = ["Submission Receipt", "=" * 60, ""]  # Header
+
     for endpoint, data in receipt_data.items():
         header = "Endpoint: {0} (Submitted: {1})".format(endpoint, data['date_of_submission'])
-        receipt_lines.extend([header, "-"*len(header)])
+        receipt_lines.extend([header, "-" * len(header)])
         
         # Table headers
-        table_header = "{:<20} | {:<15} | {:<15} | {:<10}".format("Patient", "Service Date", "Amount Billed", "Status")
+        table_header = "{:<20} | {:<15} | {:<15} | {:<20} | {:<10}".format("Patient", "Service Date", "Amount Billed", "Insurance", "Status")
         receipt_lines.append(table_header)
-        receipt_lines.append("-"*len(table_header))
+        receipt_lines.append("-" * len(table_header))
         
         # Adding patient information in a tabular format
         for patient in data["patients"]:
             success_status = "SUCCESS" if patient['success'] else "FAILED"
-            patient_info = "{:<20} | {:<15} | ${:<14} | {:<10}".format(patient['name'], patient['service_date'], patient['amount_billed'], success_status)
+            patient_info = "{:<20} | {:<15} | ${:<14} | {:<20} | {:<10}".format(
+                patient['name'], 
+                patient['service_date'], 
+                patient['amount_billed'], 
+                patient['insurance_name'], 
+                success_status
+            )
             receipt_lines.append(patient_info)
         
         receipt_lines.append("")  # Blank line for separation
     
     receipt_content = "\n".join(receipt_lines)
     return receipt_content
```

### Comparing `medicafe-0.240515.4/MediLink/test.py` & `medicafe-0.240515.5/MediLink/test.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.4/PKG-INFO` & `medicafe-0.240515.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240515.4
+Version: 0.240515.5
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240515.4/README.md` & `medicafe-0.240515.5/README.md`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.4/medicafe.egg-info/PKG-INFO` & `medicafe-0.240515.5/medicafe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240515.4
+Version: 0.240515.5
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240515.4/medicafe.egg-info/SOURCES.txt` & `medicafe-0.240515.5/medicafe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.4/setup.py` & `medicafe-0.240515.5/setup.py`

 * *Files identical despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medicafe',
-    version="0.240515.4",
+    version="0.240515.5",
     description='MediCafe',
     long_description="""
     # Project Overview: MediCafe
 
     ## Project Description
     MediCafe is a comprehensive suite designed to automate and streamline several aspects of medical administrative tasks within Medisoft, a popular medical practice management software. The system consists of two main components: MediBot and MediLink, each serving distinct functions but integrated to enhance the workflow of medical practices.
```

