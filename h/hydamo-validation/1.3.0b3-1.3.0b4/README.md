# Comparing `tmp/hydamo_validation-1.3.0b3.tar.gz` & `tmp/hydamo_validation-1.3.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydamo_validation-1.3.0b3.tar", last modified: Thu Apr 18 15:35:12 2024, max compression
+gzip compressed data, was "hydamo_validation-1.3.0b4.tar", last modified: Thu May 16 20:31:43 2024, max compression
```

## Comparing `hydamo_validation-1.3.0b3.tar` & `hydamo_validation-1.3.0b4.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 15:35:12.229684 hydamo_validation-1.3.0b3/
--rw-rw-rw-   0        0        0     1098 2024-04-05 13:12:36.000000 hydamo_validation-1.3.0b3/LICENSE
--rw-rw-rw-   0        0        0     1808 2024-04-18 15:35:12.228693 hydamo_validation-1.3.0b3/PKG-INFO
--rw-rw-rw-   0        0        0     1239 2024-04-16 10:17:00.000000 hydamo_validation-1.3.0b3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 15:35:11.952207 hydamo_validation-1.3.0b3/hydamo_validation/
--rw-rw-rw-   0        0        0      701 2024-04-18 15:19:58.000000 hydamo_validation-1.3.0b3/hydamo_validation/__init__.py
--rw-rw-rw-   0        0        0    15508 2024-04-16 09:43:08.000000 hydamo_validation-1.3.0b3/hydamo_validation/datamodel.py
--rw-rw-rw-   0        0        0     3846 2024-04-05 13:12:36.000000 hydamo_validation-1.3.0b3/hydamo_validation/datasets.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:35:11.983527 hydamo_validation-1.3.0b3/hydamo_validation/functions/
--rw-rw-rw-   0        0        0        0 2024-04-05 13:12:36.000000 hydamo_validation-1.3.0b3/hydamo_validation/functions/__init__.py
--rw-rw-rw-   0        0        0     9408 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b3/hydamo_validation/functions/general.py
--rw-rw-rw-   0        0        0     8811 2024-04-16 09:43:08.000000 hydamo_validation-1.3.0b3/hydamo_validation/functions/logic.py
--rw-rw-rw-   0        0        0    21123 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b3/hydamo_validation/functions/topologic.py
--rw-rw-rw-   0        0        0     5682 2024-04-16 09:43:08.000000 hydamo_validation-1.3.0b3/hydamo_validation/geometry.py
--rw-rw-rw-   0        0        0    14791 2024-04-16 09:43:08.000000 hydamo_validation-1.3.0b3/hydamo_validation/logical_validation.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:35:11.931073 hydamo_validation-1.3.0b3/hydamo_validation/schemas/
-drwxrwxrwx   0        0        0        0 2024-04-18 15:35:12.197028 hydamo_validation-1.3.0b3/hydamo_validation/schemas/hydamo/
--rw-rw-rw-   0        0        0   137034 2024-04-05 13:12:36.000000 hydamo_validation-1.3.0b3/hydamo_validation/schemas/hydamo/HyDAMO_2.2.json
--rw-rw-rw-   0        0        0   148047 2024-04-11 08:31:48.000000 hydamo_validation-1.3.0b3/hydamo_validation/schemas/hydamo/HyDAMO_2.3.json
-drwxrwxrwx   0        0        0        0 2024-04-18 15:35:12.204752 hydamo_validation-1.3.0b3/hydamo_validation/schemas/rules/
--rw-rw-rw-   0        0        0    19418 2024-04-05 13:12:36.000000 hydamo_validation-1.3.0b3/hydamo_validation/schemas/rules/rules_1.0.json
--rw-rw-rw-   0        0        0    19418 2024-04-05 13:12:36.000000 hydamo_validation-1.3.0b3/hydamo_validation/schemas/rules/rules_1.1.json
--rw-rw-rw-   0        0        0    19314 2024-04-05 13:12:36.000000 hydamo_validation-1.3.0b3/hydamo_validation/schemas/rules/rules_1.2.json
--rw-rw-rw-   0        0        0    19321 2024-04-11 08:40:23.000000 hydamo_validation-1.3.0b3/hydamo_validation/schemas/rules/rules_1.3.json
-drwxrwxrwx   0        0        0        0 2024-04-18 15:35:12.207743 hydamo_validation-1.3.0b3/hydamo_validation/styles/
--rw-rw-rw-   0        0        0    25514 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b3/hydamo_validation/styles/hydroobject.qml
--rw-rw-rw-   0        0        0      772 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b3/hydamo_validation/styles/hydroobject.sld
--rw-rw-rw-   0        0        0     2980 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b3/hydamo_validation/styles.py
--rw-rw-rw-   0        0        0     8330 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b3/hydamo_validation/summaries.py
--rw-rw-rw-   0        0        0    10757 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b3/hydamo_validation/syntax_validation.py
--rw-rw-rw-   0        0        0     2170 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b3/hydamo_validation/utils.py
--rw-rw-rw-   0        0        0    12709 2024-04-16 10:18:20.000000 hydamo_validation-1.3.0b3/hydamo_validation/validator.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:35:12.227689 hydamo_validation-1.3.0b3/hydamo_validation.egg-info/
--rw-rw-rw-   0        0        0     1808 2024-04-18 15:35:11.000000 hydamo_validation-1.3.0b3/hydamo_validation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1514 2024-04-18 15:35:11.000000 hydamo_validation-1.3.0b3/hydamo_validation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 15:35:11.000000 hydamo_validation-1.3.0b3/hydamo_validation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2024-04-18 15:35:11.000000 hydamo_validation-1.3.0b3/hydamo_validation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-18 15:35:11.000000 hydamo_validation-1.3.0b3/hydamo_validation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 10:11:43.000000 hydamo_validation-1.3.0b3/hydamo_validation.egg-info/zip-safe
--rw-rw-rw-   0        0        0      985 2024-04-18 14:05:36.000000 hydamo_validation-1.3.0b3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-18 15:35:12.230681 hydamo_validation-1.3.0b3/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-03-09 11:35:36.000000 hydamo_validation-1.3.0b3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:35:12.225696 hydamo_validation-1.3.0b3/tests/
--rw-rw-rw-   0        0        0     1069 2024-04-16 09:33:08.000000 hydamo_validation-1.3.0b3/tests/test_datasets.py
--rw-rw-rw-   0        0        0      970 2024-04-16 09:33:08.000000 hydamo_validation-1.3.0b3/tests/test_dommelerwaard.py
--rw-rw-rw-   0        0        0     4812 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b3/tests/test_general_functions.py
--rw-rw-rw-   0        0        0     3468 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b3/tests/test_hydamo_2_2.py
--rw-rw-rw-   0        0        0      823 2024-04-16 09:33:08.000000 hydamo_validation-1.3.0b3/tests/test_init.py
--rw-rw-rw-   0        0        0     2638 2024-04-16 09:33:08.000000 hydamo_validation-1.3.0b3/tests/test_logic_functions.py
--rw-rw-rw-   0        0        0     3205 2024-04-05 13:12:36.000000 hydamo_validation-1.3.0b3/tests/test_not_overlapping.py
--rw-rw-rw-   0        0        0     2572 2024-04-16 10:23:56.000000 hydamo_validation-1.3.0b3/tests/test_productie.py
--rw-rw-rw-   0        0        0      991 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b3/tests/test_structures_at_interersections.py
--rw-rw-rw-   0        0        0     3003 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b3/tests/test_summaries.py
--rw-rw-rw-   0        0        0     4660 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b3/tests/test_topologic_functions.py
--rw-rw-rw-   0        0        0     1592 2024-04-05 13:12:36.000000 hydamo_validation-1.3.0b3/tests/test_validationrules.py
--rw-rw-rw-   0        0        0     4597 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b3/tests/test_wrij.py
--rw-rw-rw-   0        0        0      761 2024-04-05 13:12:36.000000 hydamo_validation-1.3.0b3/tests/test_wrij_profielen.py
+drwxrwxrwx   0        0        0        0 2024-05-16 20:31:43.648918 hydamo_validation-1.3.0b4/
+-rw-rw-rw-   0        0        0     1098 2024-04-05 13:12:36.000000 hydamo_validation-1.3.0b4/LICENSE
+-rw-rw-rw-   0        0        0     1808 2024-05-16 20:31:43.647909 hydamo_validation-1.3.0b4/PKG-INFO
+-rw-rw-rw-   0        0        0     1239 2024-04-16 10:17:00.000000 hydamo_validation-1.3.0b4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 20:31:43.314275 hydamo_validation-1.3.0b4/hydamo_validation/
+-rw-rw-rw-   0        0        0      855 2024-05-16 20:30:27.000000 hydamo_validation-1.3.0b4/hydamo_validation/__init__.py
+-rw-rw-rw-   0        0        0    15508 2024-04-16 09:43:08.000000 hydamo_validation-1.3.0b4/hydamo_validation/datamodel.py
+-rw-rw-rw-   0        0        0     3846 2024-04-05 13:12:36.000000 hydamo_validation-1.3.0b4/hydamo_validation/datasets.py
+drwxrwxrwx   0        0        0        0 2024-05-16 20:31:43.435894 hydamo_validation-1.3.0b4/hydamo_validation/functions/
+-rw-rw-rw-   0        0        0        0 2024-04-05 13:12:36.000000 hydamo_validation-1.3.0b4/hydamo_validation/functions/__init__.py
+-rw-rw-rw-   0        0        0     9408 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b4/hydamo_validation/functions/general.py
+-rw-rw-rw-   0        0        0     8811 2024-04-16 09:43:08.000000 hydamo_validation-1.3.0b4/hydamo_validation/functions/logic.py
+-rw-rw-rw-   0        0        0    21123 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b4/hydamo_validation/functions/topologic.py
+-rw-rw-rw-   0        0        0     5682 2024-04-16 09:43:08.000000 hydamo_validation-1.3.0b4/hydamo_validation/geometry.py
+-rw-rw-rw-   0        0        0    14878 2024-05-16 20:21:54.000000 hydamo_validation-1.3.0b4/hydamo_validation/logical_validation.py
+drwxrwxrwx   0        0        0        0 2024-05-16 20:31:43.267973 hydamo_validation-1.3.0b4/hydamo_validation/schemas/
+drwxrwxrwx   0        0        0        0 2024-05-16 20:31:43.452180 hydamo_validation-1.3.0b4/hydamo_validation/schemas/hydamo/
+-rw-rw-rw-   0        0        0   137034 2024-04-05 13:12:36.000000 hydamo_validation-1.3.0b4/hydamo_validation/schemas/hydamo/HyDAMO_2.2.json
+-rw-rw-rw-   0        0        0   148047 2024-04-11 08:31:48.000000 hydamo_validation-1.3.0b4/hydamo_validation/schemas/hydamo/HyDAMO_2.3.json
+drwxrwxrwx   0        0        0        0 2024-05-16 20:31:43.541985 hydamo_validation-1.3.0b4/hydamo_validation/schemas/rules/
+-rw-rw-rw-   0        0        0    19418 2024-04-05 13:12:36.000000 hydamo_validation-1.3.0b4/hydamo_validation/schemas/rules/rules_1.0.json
+-rw-rw-rw-   0        0        0    19418 2024-04-05 13:12:36.000000 hydamo_validation-1.3.0b4/hydamo_validation/schemas/rules/rules_1.1.json
+-rw-rw-rw-   0        0        0    19314 2024-04-05 13:12:36.000000 hydamo_validation-1.3.0b4/hydamo_validation/schemas/rules/rules_1.2.json
+-rw-rw-rw-   0        0        0    19321 2024-04-11 08:40:23.000000 hydamo_validation-1.3.0b4/hydamo_validation/schemas/rules/rules_1.3.json
+drwxrwxrwx   0        0        0        0 2024-05-16 20:31:43.623257 hydamo_validation-1.3.0b4/hydamo_validation/styles/
+-rw-rw-rw-   0        0        0    25514 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b4/hydamo_validation/styles/hydroobject.qml
+-rw-rw-rw-   0        0        0      772 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b4/hydamo_validation/styles/hydroobject.sld
+-rw-rw-rw-   0        0        0     2980 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b4/hydamo_validation/styles.py
+-rw-rw-rw-   0        0        0     8359 2024-05-16 20:28:54.000000 hydamo_validation-1.3.0b4/hydamo_validation/summaries.py
+-rw-rw-rw-   0        0        0    10757 2024-05-16 16:10:01.000000 hydamo_validation-1.3.0b4/hydamo_validation/syntax_validation.py
+-rw-rw-rw-   0        0        0     2170 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b4/hydamo_validation/utils.py
+-rw-rw-rw-   0        0        0    13351 2024-05-16 20:26:37.000000 hydamo_validation-1.3.0b4/hydamo_validation/validator.py
+drwxrwxrwx   0        0        0        0 2024-05-16 20:31:43.646853 hydamo_validation-1.3.0b4/hydamo_validation.egg-info/
+-rw-rw-rw-   0        0        0     1808 2024-05-16 20:31:42.000000 hydamo_validation-1.3.0b4/hydamo_validation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1514 2024-05-16 20:31:42.000000 hydamo_validation-1.3.0b4/hydamo_validation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 20:31:42.000000 hydamo_validation-1.3.0b4/hydamo_validation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2024-05-16 20:31:42.000000 hydamo_validation-1.3.0b4/hydamo_validation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-16 20:31:42.000000 hydamo_validation-1.3.0b4/hydamo_validation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 10:11:43.000000 hydamo_validation-1.3.0b4/hydamo_validation.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      985 2024-04-18 14:05:36.000000 hydamo_validation-1.3.0b4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-16 20:31:43.649433 hydamo_validation-1.3.0b4/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-03-09 11:35:36.000000 hydamo_validation-1.3.0b4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 20:31:43.644815 hydamo_validation-1.3.0b4/tests/
+-rw-rw-rw-   0        0        0     1069 2024-04-16 09:33:08.000000 hydamo_validation-1.3.0b4/tests/test_datasets.py
+-rw-rw-rw-   0        0        0      970 2024-04-16 09:33:08.000000 hydamo_validation-1.3.0b4/tests/test_dommelerwaard.py
+-rw-rw-rw-   0        0        0     4812 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b4/tests/test_general_functions.py
+-rw-rw-rw-   0        0        0     3468 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b4/tests/test_hydamo_2_2.py
+-rw-rw-rw-   0        0        0      823 2024-04-16 09:33:08.000000 hydamo_validation-1.3.0b4/tests/test_init.py
+-rw-rw-rw-   0        0        0     2638 2024-04-16 09:33:08.000000 hydamo_validation-1.3.0b4/tests/test_logic_functions.py
+-rw-rw-rw-   0        0        0     3205 2024-04-05 13:12:36.000000 hydamo_validation-1.3.0b4/tests/test_not_overlapping.py
+-rw-rw-rw-   0        0        0     2572 2024-04-16 10:23:56.000000 hydamo_validation-1.3.0b4/tests/test_productie.py
+-rw-rw-rw-   0        0        0      991 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b4/tests/test_structures_at_interersections.py
+-rw-rw-rw-   0        0        0     3003 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b4/tests/test_summaries.py
+-rw-rw-rw-   0        0        0     4660 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b4/tests/test_topologic_functions.py
+-rw-rw-rw-   0        0        0     1592 2024-04-05 13:12:36.000000 hydamo_validation-1.3.0b4/tests/test_validationrules.py
+-rw-rw-rw-   0        0        0     4597 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b4/tests/test_wrij.py
+-rw-rw-rw-   0        0        0      761 2024-04-05 13:12:36.000000 hydamo_validation-1.3.0b4/tests/test_wrij_profielen.py
```

### Comparing `hydamo_validation-1.3.0b3/LICENSE` & `hydamo_validation-1.3.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b3/PKG-INFO` & `hydamo_validation-1.3.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydamo_validation
-Version: 1.3.0b3
+Version: 1.3.0b4
 Summary: Validation module for HyDAMO data
 Author-email: Daniel Tollenaar <daniel@d2hydro.nl>
 License: MIT
 Project-URL: Source, https://github.com/HetWaterschapshuis/HyDAMOValidatieModule
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `hydamo_validation-1.3.0b3/README.md` & `hydamo_validation-1.3.0b4/README.md`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b3/hydamo_validation/datamodel.py` & `hydamo_validation-1.3.0b4/hydamo_validation/datamodel.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b3/hydamo_validation/datasets.py` & `hydamo_validation-1.3.0b4/hydamo_validation/datasets.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b3/hydamo_validation/functions/general.py` & `hydamo_validation-1.3.0b4/hydamo_validation/functions/general.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b3/hydamo_validation/functions/logic.py` & `hydamo_validation-1.3.0b4/hydamo_validation/functions/logic.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b3/hydamo_validation/functions/topologic.py` & `hydamo_validation-1.3.0b4/hydamo_validation/functions/topologic.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b3/hydamo_validation/geometry.py` & `hydamo_validation-1.3.0b4/hydamo_validation/geometry.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b3/hydamo_validation/logical_validation.py` & `hydamo_validation-1.3.0b4/hydamo_validation/logical_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,33 +123,36 @@
     """Execute the logical validation."""
 
     object_rules_sets = (
         i
         for i in validation_rules_sets["objects"]
         if i["object"] in datamodel.data_layers
     )
+    logger.info(
+        rf"lagen met valide objecten én regels: {[i["object"] for i in object_rules_sets]}"
+    )
     for object_rules in object_rules_sets:
         col_translation: dict = {}
 
         object_layer = object_rules["object"]
-        logger.info(f"start logical validations of layer: {object_layer}")
+        logger.info(f"{object_layer}: start")
         object_gdf = getattr(datamodel, object_layer).copy()
 
         # add summary columns
         object_gdf["rating"] = 10
         for col in SUMMARY_COLUMNS:
             object_gdf[col] = ""
 
         # general rule section
         if "general_rules" in object_rules.keys():
             general_rules = object_rules["general_rules"]
             general_rules_sorted = sorted(general_rules, key=lambda k: k["id"])
             for rule in general_rules_sorted:
                 logger.info(
-                    f"{object_layer}: executing general-rule with id {rule['id']}"
+                    f"{object_layer}: uitvoeren general-rule met id {rule['id']}"
                 )
                 try:
                     result_variable = rule["result_variable"]
                     result_variable_name = (
                         f"general_{rule['id']:03d}_{rule['result_variable']}"
                     )
 
@@ -220,15 +223,15 @@
         ]
         validation_rules_sorted = sorted(validation_rules, key=lambda k: k["id"])
         # validation rules section
         for rule in validation_rules_sorted:
             try:
                 rule_id = rule["id"]
                 logger.info(
-                    f"{object_layer}: executing validation-rule with id {rule_id} ({rule['name']})"
+                    f"{object_layer}: uitvoeren validatieregel met id {rule_id} ({rule['name']})"
                 )
                 result_variable = rule["result_variable"]
                 if "exceptions" in rule.keys():
                     exceptions = rule["exceptions"]
                     indices = object_gdf.loc[
                         ~object_gdf[EXCEPTION_COL].isin(exceptions)
                     ].index
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hydamo_validation-1.3.0b3/hydamo_validation/schemas/hydamo/HyDAMO_2.2.json` & `hydamo_validation-1.3.0b4/hydamo_validation/schemas/hydamo/HyDAMO_2.2.json`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b3/hydamo_validation/schemas/hydamo/HyDAMO_2.3.json` & `hydamo_validation-1.3.0b4/hydamo_validation/schemas/hydamo/HyDAMO_2.3.json`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b3/hydamo_validation/schemas/rules/rules_1.0.json` & `hydamo_validation-1.3.0b4/hydamo_validation/schemas/rules/rules_1.0.json`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b3/hydamo_validation/schemas/rules/rules_1.1.json` & `hydamo_validation-1.3.0b4/hydamo_validation/schemas/rules/rules_1.1.json`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b3/hydamo_validation/schemas/rules/rules_1.2.json` & `hydamo_validation-1.3.0b4/hydamo_validation/schemas/rules/rules_1.2.json`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b3/hydamo_validation/schemas/rules/rules_1.3.json` & `hydamo_validation-1.3.0b4/hydamo_validation/schemas/rules/rules_1.3.json`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b3/hydamo_validation/styles/hydroobject.qml` & `hydamo_validation-1.3.0b4/hydamo_validation/styles/hydroobject.qml`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b3/hydamo_validation/styles/hydroobject.sld` & `hydamo_validation-1.3.0b4/hydamo_validation/styles/hydroobject.sld`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b3/hydamo_validation/styles.py` & `hydamo_validation-1.3.0b4/hydamo_validation/styles.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b3/hydamo_validation/summaries.py` & `hydamo_validation-1.3.0b4/hydamo_validation/summaries.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,23 +138,23 @@
                     if output_type == "geojson":
                         file_path = results_path.joinpath(
                             output_type, f"{object_layer}.geojson"
                         )
                         gdf_out = gdf.copy()
                         if gdf_out.crs:
                             gdf_out.to_crs("epsg:4326", inplace=True)
-                        gdf_out.to_file(file_path, driver="GeoJSON")
+                        gdf_out.to_file(file_path, driver="GeoJSON", engine="pyogrio")
 
                     # drop geometry for writing to csv
                     elif output_type == "csv":
                         file_path = results_path.joinpath(
                             output_type, f"{object_layer}.csv"
                         )
                         df = gdf.drop("geometry", axis=1)
-                        df.to_csv(file_path)
+                        df.to_csv(file_path, index=False)
 
                     # write to geopackage as is
                     elif output_type == "geopackage":
                         file_path = results_path.joinpath("results.gpkg")
 
                         gdf.to_file(
                             file_path,
@@ -178,15 +178,15 @@
         self.status = "Initialization"
         self.dataset_layers = []
         self.result_layers = []
         self.missing_layers = []
         self.error_layers = []
         self.syntax_result = []
         self.validation_result = []
-        self.error = None
+        self.error = []
         self.errors = None
         self.warnings = None
 
     def _append_to_list(self, message, property):
         """Append a a message to a list."""
         if getattr(self, property) is None:
             setattr(self, property, [])
```

### Comparing `hydamo_validation-1.3.0b3/hydamo_validation/syntax_validation.py` & `hydamo_validation-1.3.0b4/hydamo_validation/syntax_validation.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b3/hydamo_validation/utils.py` & `hydamo_validation-1.3.0b4/hydamo_validation/utils.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b3/hydamo_validation/validator.py` & `hydamo_validation-1.3.0b4/hydamo_validation/validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     missing_layers,
     fields_syntax,
 )
 import traceback
 
 OUTPUT_TYPES = ["geopackage", "geojson", "csv"]
 LOG_LEVELS = Literal["INFO", "DEBUG"]
-INCLUDE_COLUMNS = ["code"]
+INCLUDE_COLUMNS = ["nen3610id", "code"]
 SCHEMAS_PATH = Path(__file__).parent.joinpath(r"./schemas")
 HYDAMO_SCHEMAS_PATH = SCHEMAS_PATH.joinpath("hydamo")
 RULES_SCHEMAS_PATH = SCHEMAS_PATH.joinpath("rules")
 
 
 def _read_schema(version, schemas_path):
     schema_json = schemas_path.joinpath(rf"rules/rules_{version}.json").resolve()
@@ -50,14 +50,21 @@
         logging.Formatter("%(asctime)s %(name)s %(levelname)s - %(message)s")
     )
     fh.setLevel(logging.DEBUG)
     logger.addHandler(fh)
     return logger
 
 
+def _close_log_file(logger):
+    """Remove log-file from existing logger"""
+    for h in logger.handlers:
+        h.close()
+        logger.removeHandler(h)
+
+
 def _log_to_results(log_file, result_summary):
     result_summary.log = log_file.read_text().split("\n")
 
 
 def read_validation_rules(
     validation_rules_json: Path,
     result_summary: Union[ResultSummary, None] = None,
@@ -176,59 +183,62 @@
     try:
         results_path = None
         dir_path = Path(directory)
         logger = _init_logger(
             log_level=log_level,
         )
 
-        logger.info("validator start")
+        logger.info("init validatie")
         date_check = pd.Timestamp.now().isoformat()
         result_summary = ResultSummary(date_check=date_check)
         layers_summary = LayersSummary(date_check=date_check)
         # check if all files are present
         # create a results_path
+        permission_error = False
         if dir_path.exists():
             results_path = dir_path.joinpath("results")
             if results_path.exists():
                 try:
                     shutil.rmtree(results_path)
                 except PermissionError:
-                    logger.warning(
-                        f"Cannot remove {results_path}. This may lead to write-issues later!"
-                    )
-                    pass
+                    permission_error = True
             results_path.mkdir(parents=True, exist_ok=True)
         else:
             raise FileNotFoundError(f"{dir_path.absolute().resolve()} does not exist")
 
         log_file = results_path.joinpath("validator.log")
         logger = _add_log_file(logger, log_file=log_file)
+        logger.info("start validatie")
+        if permission_error:
+            logger.warning(
+                f"Kan pad {results_path} niet verwijderen. Dit kan later tot problemen leiden!"
+            )
         dataset_path = dir_path.joinpath("datasets")
         validation_rules_json = dir_path.joinpath("validationrules.json")
         missing_paths = []
         for path in [dataset_path, validation_rules_json]:
             if not path.exists():
                 missing_paths += [str(path)]
         if missing_paths:
-            result_summary.error = [f'missing_paths: {",".join(missing_paths)}']
+            result_summary.error += [f'missing_paths: {",".join(missing_paths)}']
             raise FileNotFoundError(f'missing_paths: {",".join(missing_paths)}')
         else:
             validation_rules_sets = read_validation_rules(
-                validation_rules_json, SCHEMAS_PATH
+                validation_rules_json, result_summary
             )
 
         # check if output-files are supported
         unsupported_output_types = [
             item for item in output_types if item not in OUTPUT_TYPES
         ]
         if unsupported_output_types:
             error_message = (
                 r"unsupported output types: " f'{",".join(unsupported_output_types)}'
             )
-            result_summary.error = [error_message]
+            result_summary.error += [error_message]
             raise TypeError(error_message)
 
         # set coverages
         if coverages:
             for key, item in coverages.items():
                 logical_validation.general_functions._set_coverage(key, item)
 
@@ -245,15 +255,15 @@
         # validate dataset syntax
         result_summary.status = "syntax-validation (layers)"
         datasets = DataSets(dataset_path)
 
         result_summary.dataset_layers = datasets.layers
 
         ## validate syntax of datasets on layers-level and append to result
-        logger.info("start syntax-validation of object-layers")
+        logger.info("start syntax-validatie van object-lagen")
         valid_layers = datamodel_layers(datamodel.layers, datasets.layers)
         result_summary.missing_layers = missing_layers(
             datamodel.layers, datasets.layers
         )
 
         ## validate valid_layers on fields-level and add them to data_model
         result_summary.status = "syntax-validation (fields)"
@@ -261,62 +271,67 @@
 
         ## get status_object if any
         status_object = None
         if "status_object" in validation_rules_sets.keys():
             status_object = validation_rules_sets["status_object"]
 
         for layer in valid_layers:
-            logger.info(f"read layer {layer}")
+            logger.info(f"{layer}: inlezen")
 
             # read layer
             gdf, schema = datasets.read_layer(
                 layer, result_summary=result_summary, status_object=status_object
             )
             if (
                 gdf.empty
             ):  # pass if gdf is empty. Most likely due to mall-formed or ill-specifiec status_object
                 logger.warning(
-                    f"layer {layer} is empty. Be aware only values of {status_object} in field 'statusobject' are read!"
+                    f"{layer}: geen objecten ingelezen. Zorg dat alle waarden in de kolom 'status_object' voorkomen in {status_object}"
                 )
                 continue
 
             layer = layer.lower()
             for col in INCLUDE_COLUMNS:
                 if col not in gdf.columns:
                     gdf[col] = None
                     schema["properties"][col] = "str"
 
-            logger.info(f"syntax-validation of fields in layer {layer}")
+            logger.info(f"{layer}: syntax-validatie")
             gdf, result_gdf = fields_syntax(
                 gdf,
-                schema,
-                datamodel.validation_schemas[layer],
+                schema=schema,
+                validation_schema=datamodel.validation_schemas[layer],
                 keep_columns=INCLUDE_COLUMNS,
             )
 
             # Add the syntax-validation result to the results_summary
             layers_summary.set_data(result_gdf, layer, schema["geometry"])
             # Add the corrected datasets_layer data to the datamodel.
-            datamodel.set_data(gdf, layer, index_col=None)
+            if gdf.empty:
+                logger.warning(
+                    f"{layer}: geen valide objecten na syntax-validatie. Inspecteer 'syntax_oordeel' in de resultaten; deze is false voor alle objecten. De laag zal genegeerd worden in de (topo)logische validatie."
+                )
+            else:
+                datamodel.set_data(gdf, layer, index_col=None)
             syntax_result += [layer]
 
         # do logical validation: append result to layers_summary
         result_summary.status = "logical validation"
-        logger.info("start (topo)logical-validation")
+        logger.info("start (topo)logische validatie van object-lagen")
         layers_summary, result_summary = logical_validation.execute(
             datamodel,
             validation_rules_sets,
             layers_summary,
             result_summary,
             logger,
             raise_error,
         )
 
         # finish validation and export results
-        logger.info("exporting results")
+        logger.info("exporteren resultaten")
         result_summary.status = "export results"
         result_layers = layers_summary.export(results_path, output_types)
         result_summary.result_layers = result_layers
         result_summary.error_layers = [
             i for i in datasets.layers if i.lower() not in result_layers
         ]
         result_summary.syntax_result = syntax_result
@@ -324,32 +339,34 @@
             i["object"]
             for i in validation_rules_sets["objects"]
             if i["object"] in result_layers
         ]
         result_summary.success = True
         result_summary.status = "finished"
         result_summary.duration = timer.report()
-        logger.info(f"finished in {result_summary.duration:.2f} seconds")
+        logger.info(f"klaar in {result_summary.duration:.2f} seconden")
 
         _log_to_results(log_file, result_summary)
         result_summary.to_json(results_path)
 
+        _close_log_file(logger)
+
         return datamodel, layers_summary, result_summary
 
     except Exception as e:
-        e_str = str(e).replace("\n", " ")
-        e_str = " ".join(e_str.split())
-        stacktrace = rf"{traceback.format_exc(limit=2)}".split("\n")
+        stacktrace = rf"\n{traceback.format_exc(limit=0, chain=False)}".split("\n")
         if result_summary.error is not None:
-            result_summary.error += [stacktrace]
+            result_summary.error += stacktrace
         else:
-            result_summary.error = [stacktrace]
+            result_summary.error = stacktrace
         if results_path is not None:
             result_layers = layers_summary.export(results_path, output_types)
             _log_to_results(log_file, result_summary)
             result_summary.to_json(results_path)
         if raise_error:
             raise e
         else:
             result_summary.to_dict()
 
+        _close_log_file(logger)
+
         return None
```

### Comparing `hydamo_validation-1.3.0b3/hydamo_validation.egg-info/PKG-INFO` & `hydamo_validation-1.3.0b4/hydamo_validation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydamo_validation
-Version: 1.3.0b3
+Version: 1.3.0b4
 Summary: Validation module for HyDAMO data
 Author-email: Daniel Tollenaar <daniel@d2hydro.nl>
 License: MIT
 Project-URL: Source, https://github.com/HetWaterschapshuis/HyDAMOValidatieModule
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `hydamo_validation-1.3.0b3/hydamo_validation.egg-info/SOURCES.txt` & `hydamo_validation-1.3.0b4/hydamo_validation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b3/pyproject.toml` & `hydamo_validation-1.3.0b4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b3/tests/test_datasets.py` & `hydamo_validation-1.3.0b4/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b3/tests/test_dommelerwaard.py` & `hydamo_validation-1.3.0b4/tests/test_dommelerwaard.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b3/tests/test_general_functions.py` & `hydamo_validation-1.3.0b4/tests/test_general_functions.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b3/tests/test_hydamo_2_2.py` & `hydamo_validation-1.3.0b4/tests/test_hydamo_2_2.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b3/tests/test_init.py` & `hydamo_validation-1.3.0b4/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b3/tests/test_logic_functions.py` & `hydamo_validation-1.3.0b4/tests/test_logic_functions.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b3/tests/test_not_overlapping.py` & `hydamo_validation-1.3.0b4/tests/test_not_overlapping.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b3/tests/test_productie.py` & `hydamo_validation-1.3.0b4/tests/test_productie.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b3/tests/test_structures_at_interersections.py` & `hydamo_validation-1.3.0b4/tests/test_structures_at_interersections.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b3/tests/test_summaries.py` & `hydamo_validation-1.3.0b4/tests/test_summaries.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b3/tests/test_topologic_functions.py` & `hydamo_validation-1.3.0b4/tests/test_topologic_functions.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b3/tests/test_validationrules.py` & `hydamo_validation-1.3.0b4/tests/test_validationrules.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b3/tests/test_wrij.py` & `hydamo_validation-1.3.0b4/tests/test_wrij.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b3/tests/test_wrij_profielen.py` & `hydamo_validation-1.3.0b4/tests/test_wrij_profielen.py`

 * *Files identical despite different names*

