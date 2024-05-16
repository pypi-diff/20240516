# Comparing `tmp/medicafe-0.240515.2.tar.gz` & `tmp/medicafe-0.240515.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medicafe-0.240515.2.tar", last modified: Wed May 15 19:54:10 2024, max compression
+gzip compressed data, was "medicafe-0.240515.3.tar", last modified: Wed May 15 20:15:20 2024, max compression
```

## Comparing `medicafe-0.240515.2.tar` & `medicafe-0.240515.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 19:54:10.661000 medicafe-0.240515.2/
--rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240515.2/LICENSE
--rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240515.2/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-15 19:54:09.639000 medicafe-0.240515.2/MediBot/
--rwxrwxrwx   0        0        0     5972 2024-05-12 18:02:44.000000 medicafe-0.240515.2/MediBot/MediBot.bat
--rw-rw-rw-   0        0        0    17490 2024-05-15 17:01:43.000000 medicafe-0.240515.2/MediBot/MediBot.py
--rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240515.2/MediBot/MediBot_Charges.py
--rw-rw-rw-   0        0        0    14538 2024-05-15 19:07:33.000000 medicafe-0.240515.2/MediBot/MediBot_Crosswalk_Library.py
--rw-rw-rw-   0        0        0    14906 2024-05-15 16:48:28.000000 medicafe-0.240515.2/MediBot/MediBot_Preprocessor.py
--rw-rw-rw-   0        0        0    17184 2024-05-15 17:38:32.000000 medicafe-0.240515.2/MediBot/MediBot_Preprocessor_lib.py
--rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240515.2/MediBot/MediBot_UI.py
--rw-rw-rw-   0        0        0     8965 2024-05-15 19:49:49.000000 medicafe-0.240515.2/MediBot/MediBot_dataformat_library.py
--rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240515.2/MediBot/MediPost.py
--rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240515.2/MediBot/PDF_to_CSV_Cleaner.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240515.2/MediBot/__init__.py
--rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240515.2/MediBot/update_json.py
--rw-rw-rw-   0        0        0     2249 2024-05-10 17:47:37.000000 medicafe-0.240515.2/MediBot/update_medicafe.py
-drwxrwxrwx   0        0        0        0 2024-05-15 19:54:10.415000 medicafe-0.240515.2/MediLink/
--rw-rw-rw-   0        0        0    20303 2024-05-15 19:29:00.000000 medicafe-0.240515.2/MediLink/MediLink.py
--rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240515.2/MediLink/MediLink_277_decoder.py
--rw-rw-rw-   0        0        0    25315 2024-05-14 15:17:10.000000 medicafe-0.240515.2/MediLink/MediLink_837p_encoder.py
--rw-rw-rw-   0        0        0    41978 2024-05-15 18:52:35.000000 medicafe-0.240515.2/MediLink/MediLink_837p_encoder_library.py
--rw-rw-rw-   0        0        0     6166 2024-05-15 17:49:28.000000 medicafe-0.240515.2/MediLink/MediLink_APIs.py
--rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240515.2/MediLink/MediLink_ConfigLoader.py
--rw-rw-rw-   0        0        0    12235 2024-05-14 15:14:04.000000 medicafe-0.240515.2/MediLink/MediLink_DataMgmt.py
--rw-rw-rw-   0        0        0     7248 2024-05-15 07:47:12.000000 medicafe-0.240515.2/MediLink/MediLink_Down.py
--rw-rw-rw-   0        0        0     8710 2024-05-15 13:36:03.000000 medicafe-0.240515.2/MediLink/MediLink_ERA_decoder.py
--rw-rw-rw-   0        0        0     6236 2024-05-10 16:45:40.000000 medicafe-0.240515.2/MediLink/MediLink_Gmail.py
--rw-rw-rw-   0        0        0      370 2024-05-14 22:24:45.000000 medicafe-0.240515.2/MediLink/MediLink_Mailer.py
--rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240515.2/MediLink/MediLink_Scheduler.py
--rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240515.2/MediLink/MediLink_StatusCheck.py
--rw-rw-rw-   0        0        0     5181 2024-05-12 16:36:09.000000 medicafe-0.240515.2/MediLink/MediLink_UI.py
--rw-rw-rw-   0        0        0    19252 2024-05-15 13:35:59.000000 medicafe-0.240515.2/MediLink/MediLink_Up.py
--rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240515.2/MediLink/MediLink_batch.bat
--rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240515.2/MediLink/Soumit_api.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240515.2/MediLink/__init__.py
--rw-rw-rw-   0        0        0     3108 2024-05-13 04:52:22.000000 medicafe-0.240515.2/MediLink/test.py
--rw-rw-rw-   0        0        0     4396 2024-05-15 19:54:10.641000 medicafe-0.240515.2/PKG-INFO
--rw-rw-rw-   0        0        0     2960 2024-05-13 07:31:39.000000 medicafe-0.240515.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 19:54:10.620000 medicafe-0.240515.2/medicafe.egg-info/
--rw-rw-rw-   0        0        0     4396 2024-05-15 19:54:08.000000 medicafe-0.240515.2/medicafe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1114 2024-05-15 19:54:08.000000 medicafe-0.240515.2/medicafe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 19:54:08.000000 medicafe-0.240515.2/medicafe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240515.2/medicafe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       60 2024-05-15 19:54:08.000000 medicafe-0.240515.2/medicafe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-15 19:54:08.000000 medicafe-0.240515.2/medicafe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 19:54:10.656000 medicafe-0.240515.2/setup.cfg
--rw-rw-rw-   0        0        0     4834 2024-05-15 19:54:07.000000 medicafe-0.240515.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 20:15:20.564000 medicafe-0.240515.3/
+-rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240515.3/LICENSE
+-rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240515.3/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-15 20:15:19.613000 medicafe-0.240515.3/MediBot/
+-rwxrwxrwx   0        0        0     5972 2024-05-12 18:02:44.000000 medicafe-0.240515.3/MediBot/MediBot.bat
+-rw-rw-rw-   0        0        0    17490 2024-05-15 17:01:43.000000 medicafe-0.240515.3/MediBot/MediBot.py
+-rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240515.3/MediBot/MediBot_Charges.py
+-rw-rw-rw-   0        0        0    14538 2024-05-15 19:07:33.000000 medicafe-0.240515.3/MediBot/MediBot_Crosswalk_Library.py
+-rw-rw-rw-   0        0        0    14906 2024-05-15 16:48:28.000000 medicafe-0.240515.3/MediBot/MediBot_Preprocessor.py
+-rw-rw-rw-   0        0        0    17184 2024-05-15 17:38:32.000000 medicafe-0.240515.3/MediBot/MediBot_Preprocessor_lib.py
+-rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240515.3/MediBot/MediBot_UI.py
+-rw-rw-rw-   0        0        0     8912 2024-05-15 20:14:35.000000 medicafe-0.240515.3/MediBot/MediBot_dataformat_library.py
+-rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240515.3/MediBot/MediPost.py
+-rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240515.3/MediBot/PDF_to_CSV_Cleaner.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240515.3/MediBot/__init__.py
+-rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240515.3/MediBot/update_json.py
+-rw-rw-rw-   0        0        0     2249 2024-05-10 17:47:37.000000 medicafe-0.240515.3/MediBot/update_medicafe.py
+drwxrwxrwx   0        0        0        0 2024-05-15 20:15:20.310000 medicafe-0.240515.3/MediLink/
+-rw-rw-rw-   0        0        0    20303 2024-05-15 19:29:00.000000 medicafe-0.240515.3/MediLink/MediLink.py
+-rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240515.3/MediLink/MediLink_277_decoder.py
+-rw-rw-rw-   0        0        0    25315 2024-05-14 15:17:10.000000 medicafe-0.240515.3/MediLink/MediLink_837p_encoder.py
+-rw-rw-rw-   0        0        0    41978 2024-05-15 18:52:35.000000 medicafe-0.240515.3/MediLink/MediLink_837p_encoder_library.py
+-rw-rw-rw-   0        0        0     6166 2024-05-15 17:49:28.000000 medicafe-0.240515.3/MediLink/MediLink_APIs.py
+-rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240515.3/MediLink/MediLink_ConfigLoader.py
+-rw-rw-rw-   0        0        0    12235 2024-05-14 15:14:04.000000 medicafe-0.240515.3/MediLink/MediLink_DataMgmt.py
+-rw-rw-rw-   0        0        0     7248 2024-05-15 07:47:12.000000 medicafe-0.240515.3/MediLink/MediLink_Down.py
+-rw-rw-rw-   0        0        0     8710 2024-05-15 13:36:03.000000 medicafe-0.240515.3/MediLink/MediLink_ERA_decoder.py
+-rw-rw-rw-   0        0        0     6236 2024-05-10 16:45:40.000000 medicafe-0.240515.3/MediLink/MediLink_Gmail.py
+-rw-rw-rw-   0        0        0      370 2024-05-14 22:24:45.000000 medicafe-0.240515.3/MediLink/MediLink_Mailer.py
+-rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240515.3/MediLink/MediLink_Scheduler.py
+-rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240515.3/MediLink/MediLink_StatusCheck.py
+-rw-rw-rw-   0        0        0     5181 2024-05-12 16:36:09.000000 medicafe-0.240515.3/MediLink/MediLink_UI.py
+-rw-rw-rw-   0        0        0    19252 2024-05-15 13:35:59.000000 medicafe-0.240515.3/MediLink/MediLink_Up.py
+-rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240515.3/MediLink/MediLink_batch.bat
+-rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240515.3/MediLink/Soumit_api.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240515.3/MediLink/__init__.py
+-rw-rw-rw-   0        0        0     3108 2024-05-13 04:52:22.000000 medicafe-0.240515.3/MediLink/test.py
+-rw-rw-rw-   0        0        0     4396 2024-05-15 20:15:20.542000 medicafe-0.240515.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2960 2024-05-13 07:31:39.000000 medicafe-0.240515.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 20:15:20.525000 medicafe-0.240515.3/medicafe.egg-info/
+-rw-rw-rw-   0        0        0     4396 2024-05-15 20:15:18.000000 medicafe-0.240515.3/medicafe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1114 2024-05-15 20:15:18.000000 medicafe-0.240515.3/medicafe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 20:15:18.000000 medicafe-0.240515.3/medicafe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240515.3/medicafe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       60 2024-05-15 20:15:18.000000 medicafe-0.240515.3/medicafe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-15 20:15:18.000000 medicafe-0.240515.3/medicafe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 20:15:20.557000 medicafe-0.240515.3/setup.cfg
+-rw-rw-rw-   0        0        0     4834 2024-05-15 20:15:17.000000 medicafe-0.240515.3/setup.py
```

### Comparing `medicafe-0.240515.2/LICENSE` & `medicafe-0.240515.3/LICENSE`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.2/MediBot/MediBot.bat` & `medicafe-0.240515.3/MediBot/MediBot.bat`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.2/MediBot/MediBot.py` & `medicafe-0.240515.3/MediBot/MediBot.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.2/MediBot/MediBot_Charges.py` & `medicafe-0.240515.3/MediBot/MediBot_Charges.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.2/MediBot/MediBot_Crosswalk_Library.py` & `medicafe-0.240515.3/MediBot/MediBot_Crosswalk_Library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.2/MediBot/MediBot_Preprocessor.py` & `medicafe-0.240515.3/MediBot/MediBot_Preprocessor.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.2/MediBot/MediBot_Preprocessor_lib.py` & `medicafe-0.240515.3/MediBot/MediBot_Preprocessor_lib.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.2/MediBot/MediBot_UI.py` & `medicafe-0.240515.3/MediBot/MediBot_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.2/MediBot/MediBot_dataformat_library.py` & `medicafe-0.240515.3/MediBot/MediBot_dataformat_library.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,37 +67,37 @@
     return alphanumeric
 
 def format_gender(value):
     return value[0].upper()
 
 def enforce_significant_length(output):
     # Replace spaces with a placeholder that counts as one significant digit
-    temp_output = output.replace(' ', '{Space}')
+    temp_output = output.replace('{Space}', ' ')
     
     # Check if the number of significant digits exceeds 30
     if len(temp_output) > 30:
-        MediLink_ConfigLoader.log("Address significant length policy enforced...")
+        
         # First line of defense: Replace ' APT ' with ' #' if the original length is longer than 30 characters.
         temp_output = temp_output.replace(' APT ', ' #')
-
-        # Remove spaces in a controlled manner if still too long
+        
+        # Remove spaces in a controlled manner from right to left if still too long
         while len(temp_output) > 30:
             # Find the last space
-            last_space_index = temp_output.rfind('{Space}')
+            last_space_index = temp_output.rfind(' ')
             if last_space_index == -1:
                 break
             # Remove the last space
             temp_output = temp_output[:last_space_index] + temp_output[last_space_index+7:]
 
         # If still greater than 30, truncate to 30 characters
         if len(temp_output) > 30:
             temp_output = temp_output[:30]
 
     # Replace placeholder back with actual space for final return
-    return temp_output.replace('{Space}', ' ')
+    return temp_output.replace(' ', '{Space}')
 
 def format_street(value, csv_data, reverse_mapping, parsed_address_components):
     # Temporarily disable script pause status
     app_control.set_pause_status(False)
     
     # Remove period characters.
     value = value.replace('.', '')
```

### Comparing `medicafe-0.240515.2/MediBot/PDF_to_CSV_Cleaner.py` & `medicafe-0.240515.3/MediBot/PDF_to_CSV_Cleaner.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.2/MediBot/update_json.py` & `medicafe-0.240515.3/MediBot/update_json.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.2/MediBot/update_medicafe.py` & `medicafe-0.240515.3/MediBot/update_medicafe.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.2/MediLink/MediLink.py` & `medicafe-0.240515.3/MediLink/MediLink.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.2/MediLink/MediLink_277_decoder.py` & `medicafe-0.240515.3/MediLink/MediLink_277_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.2/MediLink/MediLink_837p_encoder.py` & `medicafe-0.240515.3/MediLink/MediLink_837p_encoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.2/MediLink/MediLink_837p_encoder_library.py` & `medicafe-0.240515.3/MediLink/MediLink_837p_encoder_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.2/MediLink/MediLink_APIs.py` & `medicafe-0.240515.3/MediLink/MediLink_APIs.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.2/MediLink/MediLink_ConfigLoader.py` & `medicafe-0.240515.3/MediLink/MediLink_ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.2/MediLink/MediLink_DataMgmt.py` & `medicafe-0.240515.3/MediLink/MediLink_DataMgmt.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.2/MediLink/MediLink_Down.py` & `medicafe-0.240515.3/MediLink/MediLink_Down.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.2/MediLink/MediLink_ERA_decoder.py` & `medicafe-0.240515.3/MediLink/MediLink_ERA_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.2/MediLink/MediLink_Gmail.py` & `medicafe-0.240515.3/MediLink/MediLink_Gmail.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.2/MediLink/MediLink_Scheduler.py` & `medicafe-0.240515.3/MediLink/MediLink_Scheduler.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.2/MediLink/MediLink_UI.py` & `medicafe-0.240515.3/MediLink/MediLink_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.2/MediLink/MediLink_Up.py` & `medicafe-0.240515.3/MediLink/MediLink_Up.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.2/MediLink/test.py` & `medicafe-0.240515.3/MediLink/test.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.2/PKG-INFO` & `medicafe-0.240515.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240515.2
+Version: 0.240515.3
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240515.2/README.md` & `medicafe-0.240515.3/README.md`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.2/medicafe.egg-info/PKG-INFO` & `medicafe-0.240515.3/medicafe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240515.2
+Version: 0.240515.3
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240515.2/medicafe.egg-info/SOURCES.txt` & `medicafe-0.240515.3/medicafe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.2/setup.py` & `medicafe-0.240515.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medicafe',
-    version="0.240515.2",
+    version="0.240515.3",
     description='MediCafe',
     long_description="""
     # Project Overview: MediCafe
 
     ## Project Description
     MediCafe is a comprehensive suite designed to automate and streamline several aspects of medical administrative tasks within Medisoft, a popular medical practice management software. The system consists of two main components: MediBot and MediLink, each serving distinct functions but integrated to enhance the workflow of medical practices.
```

