# Comparing `tmp/wheelz_idp_validations-2.2.4.tar.gz` & `tmp/wheelz_idp_validations-2.2.5.tar.gz`

## Comparing `wheelz_idp_validations-2.2.4.tar` & `wheelz_idp_validations-2.2.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.4/LICESNSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.4/requirements.txt
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.4/src/wheelz_idp_validations/__init__.py
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.4/src/wheelz_idp_validations/id_sanitizer.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.4/src/wheelz_idp_validations/pcv1_sanitizer.py
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.4/src/wheelz_idp_validations/pcv2_sanitizer.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.4/src/wheelz_idp_validations/sanitize_exception.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.4/src/wheelz_idp_validations/exceptions/__init__.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.4/src/wheelz_idp_validations/exceptions/cif_exceptions.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.4/src/wheelz_idp_validations/exceptions/date_exceptions.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.4/src/wheelz_idp_validations/exceptions/full_name_exceptions.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.4/src/wheelz_idp_validations/exceptions/gender_exceptions.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.4/src/wheelz_idp_validations/exceptions/id_exceptions.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.4/src/wheelz_idp_validations/exceptions/plate_exceptions.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.4/src/wheelz_idp_validations/exceptions/vin_exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.4/src/wheelz_idp_validations/sanitizers/__init__.py
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.4/src/wheelz_idp_validations/sanitizers/cif.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.4/src/wheelz_idp_validations/sanitizers/date.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.4/src/wheelz_idp_validations/sanitizers/full_name.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.4/src/wheelz_idp_validations/sanitizers/gender.py
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.4/src/wheelz_idp_validations/sanitizers/id_number.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.4/src/wheelz_idp_validations/sanitizers/plate.py
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.4/src/wheelz_idp_validations/sanitizers/vin.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.4/.gitignore
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.4/pyproject.toml
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.4/readme.md
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.5/LICESNSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.5/requirements.txt
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.5/src/wheelz_idp_validations/__init__.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.5/src/wheelz_idp_validations/id_sanitizer.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.5/src/wheelz_idp_validations/pcv1_sanitizer.py
+-rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.5/src/wheelz_idp_validations/pcv2_sanitizer.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.5/src/wheelz_idp_validations/sanitize_exception.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.5/src/wheelz_idp_validations/exceptions/__init__.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.5/src/wheelz_idp_validations/exceptions/cif_exceptions.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.5/src/wheelz_idp_validations/exceptions/date_exceptions.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.5/src/wheelz_idp_validations/exceptions/full_name_exceptions.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.5/src/wheelz_idp_validations/exceptions/gender_exceptions.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.5/src/wheelz_idp_validations/exceptions/id_exceptions.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.5/src/wheelz_idp_validations/exceptions/plate_exceptions.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.5/src/wheelz_idp_validations/exceptions/vin_exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.5/src/wheelz_idp_validations/sanitizers/__init__.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.5/src/wheelz_idp_validations/sanitizers/cif.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.5/src/wheelz_idp_validations/sanitizers/date.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.5/src/wheelz_idp_validations/sanitizers/full_name.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.5/src/wheelz_idp_validations/sanitizers/gender.py
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.5/src/wheelz_idp_validations/sanitizers/id_number.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.5/src/wheelz_idp_validations/sanitizers/plate.py
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.5/src/wheelz_idp_validations/sanitizers/vin.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.5/.gitignore
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.5/pyproject.toml
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.5/readme.md
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.5/PKG-INFO
```

### Comparing `wheelz_idp_validations-2.2.4/LICESNSE` & `wheelz_idp_validations-2.2.5/LICESNSE`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.2.4/.github/workflows/python-publish.yml` & `wheelz_idp_validations-2.2.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.2.4/src/wheelz_idp_validations/id_sanitizer.py` & `wheelz_idp_validations-2.2.5/src/wheelz_idp_validations/id_sanitizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,25 +32,25 @@
             print("Error sanitizing gender:", str(e))
     else:
         print("Warning: 'gender' has not been validated because not found in the response dictionary.")
 
     # Sanitize Birth Date
     if "birthDate" in response_dict:
         try:
-            response_dict["birthDate"] = sanitize_dates(response_dict["birthDate"])
+            response_dict["birthDate"] = sanitize_dates(response_dict["birthDate"], multiple = False)
         except Exception as e:
             response_dict["birthDate"] = ""
             print("Error sanitizing birth date:", str(e))
     else:
         print("Warning: 'birthDate' has not been validated because not found in the response dictionary.")
 
     # Sanitize Expiration Date
     if "expirationDate" in response_dict:
         try:
-            response_dict["expirationDate"] = sanitize_dates(response_dict["expirationDate"])
+            response_dict["expirationDate"] = sanitize_dates(response_dict["expirationDate"], multiple = False)
         except Exception as e:
             response_dict["expirationDate"] = ""
             print("Error sanitizing expiration date:", str(e))
     else:
         print("Warning: 'expirationDate' has not been validated because not found in the response dictionary.")
 
     return response_dict
```

### Comparing `wheelz_idp_validations-2.2.4/src/wheelz_idp_validations/pcv1_sanitizer.py` & `wheelz_idp_validations-2.2.5/src/wheelz_idp_validations/pcv1_sanitizer.py`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.2.4/src/wheelz_idp_validations/pcv2_sanitizer.py` & `wheelz_idp_validations-2.2.5/src/wheelz_idp_validations/pcv2_sanitizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,45 +22,45 @@
             print("Error sanitizing field E:", str(e))
     else:
         print("Warning: 'E' has not been validated because not found in the response dictionary.")
     
     # Sanitize field fecha de primera matriculación. Campo B
     if "B" in response_dict:
         try:
-            response_dict["B"] = sanitize_dates(response_dict["B"])
+            response_dict["B"] = sanitize_dates(response_dict["B"], multiple = False)
         except Exception as e:
             response_dict["B"] = ""
             print("Error sanitizing field B:", str(e))
     else:
         print("Warning: 'B' has not been validated because not found in the response dictionary.")
 
     # Sanitize field periodo de validez del permiso. Campo H
     if "H" in response_dict:
         try:
-            response_dict["H"] = sanitize_dates(response_dict["H"])
+            response_dict["H"] = sanitize_dates(response_dict["H"], multiple = False)
         except Exception as e:
             response_dict["H"] = ""
             print("Error sanitizing field H:", str(e))
     else:
         print("Warning: 'H' has not been validated because not found in the response dictionary.")
 
     # Sanitize field fecha de matriculación a la que se refiere el presente permiso. Campo I
     if "I" in response_dict:
         try:
-            response_dict["I"] = sanitize_dates(response_dict["I"])
+            response_dict["I"] = sanitize_dates(response_dict["I"], multiple = False)
         except Exception as e:
             response_dict["I"] = ""
             print("Error sanitizing field I:", str(e))
     else:
         print("Warning: 'I' has not been validated because not found in the response dictionary.")
 
     # Sanitize field fecha de expedición. Campo I.1
     if "I.1" in response_dict:
         try:
-            response_dict["I.1"] = sanitize_dates(response_dict["I.1"])
+            response_dict["I.1"] = sanitize_dates(response_dict["I.1"], multiple = False)
         except Exception as e:
             response_dict["I.1"] = ""
             print("Error sanitizing field I.1:", str(e))
     else:
         print("Warning: 'I.1' has not been validated because not found in the response dictionary.")
 
     return response_dict
```

### Comparing `wheelz_idp_validations-2.2.4/src/wheelz_idp_validations/exceptions/cif_exceptions.py` & `wheelz_idp_validations-2.2.5/src/wheelz_idp_validations/exceptions/cif_exceptions.py`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.2.4/src/wheelz_idp_validations/exceptions/id_exceptions.py` & `wheelz_idp_validations-2.2.5/src/wheelz_idp_validations/exceptions/id_exceptions.py`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.2.4/src/wheelz_idp_validations/sanitizers/cif.py` & `wheelz_idp_validations-2.2.5/src/wheelz_idp_validations/sanitizers/cif.py`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.2.4/src/wheelz_idp_validations/sanitizers/full_name.py` & `wheelz_idp_validations-2.2.5/src/wheelz_idp_validations/sanitizers/full_name.py`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.2.4/src/wheelz_idp_validations/sanitizers/gender.py` & `wheelz_idp_validations-2.2.5/src/wheelz_idp_validations/sanitizers/gender.py`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.2.4/src/wheelz_idp_validations/sanitizers/id_number.py` & `wheelz_idp_validations-2.2.5/src/wheelz_idp_validations/sanitizers/id_number.py`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.2.4/src/wheelz_idp_validations/sanitizers/plate.py` & `wheelz_idp_validations-2.2.5/src/wheelz_idp_validations/sanitizers/plate.py`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.2.4/src/wheelz_idp_validations/sanitizers/vin.py` & `wheelz_idp_validations-2.2.5/src/wheelz_idp_validations/sanitizers/vin.py`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.2.4/pyproject.toml` & `wheelz_idp_validations-2.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/wheelz_idp_validations"]
 
 
 [project]
 name = "wheelz_idp_validations"
-version = "2.2.4"
+version = "2.2.5"
 authors = [
   { name="Lluis" },
 ]
 description = "Validation for spasnish documents"
 readme = "readme.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `wheelz_idp_validations-2.2.4/PKG-INFO` & `wheelz_idp_validations-2.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: wheelz_idp_validations
-Version: 2.2.4
+Version: 2.2.5
 Summary: Validation for spasnish documents
 Project-URL: Homepage, https://github.com/albertvazquezm/wheelz-idp-validations
 Project-URL: Issues, https://github.com/albertvazquezm/wheelz-idp-validationsissues
 Author: Lluis
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

