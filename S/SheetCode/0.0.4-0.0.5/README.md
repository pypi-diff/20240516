# Comparing `tmp/sheetcode-0.0.4.tar.gz` & `tmp/sheetcode-0.0.5.tar.gz`

## Comparing `sheetcode-0.0.4.tar` & `sheetcode-0.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 sheetcode-0.0.4/BUTTONS_LIGHTS_Phase_2.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 sheetcode-0.0.4/SheetCode.code-workspace
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 sheetcode-0.0.4/.vscode/launch.json
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 sheetcode-0.0.4/example/UTest.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 sheetcode-0.0.4/example/run_all_scripts.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 sheetcode-0.0.4/example/run_one_script.py
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 sheetcode-0.0.4/example/scripts/BUTTONS_LIGHTS_Phase_1.py
--rw-r--r--   0        0        0     9895 2020-02-02 00:00:00.000000 sheetcode-0.0.4/example/sheets/FCT_BUTTONS_LIGHTS_Phase_1_1A.xlsx
--rw-r--r--   0        0        0     9999 2020-02-02 00:00:00.000000 sheetcode-0.0.4/example/sheets/FCT_BUTTONS_LIGHTS_Phase_2_1A.xlsx
--rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 sheetcode-0.0.4/example/traceability/parameters.xlsx
--rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 sheetcode-0.0.4/example/traceability/requirements.xlsx
--rw-r--r--   0        0        0   404967 2020-02-02 00:00:00.000000 sheetcode-0.0.4/screenshots/Phase1.png
--rw-r--r--   0        0        0    33450 2020-02-02 00:00:00.000000 sheetcode-0.0.4/screenshots/Phase1_XLS.png
--rw-r--r--   0        0        0   710107 2020-02-02 00:00:00.000000 sheetcode-0.0.4/screenshots/Phase2.png
--rw-r--r--   0        0        0    37177 2020-02-02 00:00:00.000000 sheetcode-0.0.4/screenshots/Phase2_XLS.png
--rw-r--r--   0        0        0    50813 2020-02-02 00:00:00.000000 sheetcode-0.0.4/screenshots/Traca1.png
--rw-r--r--   0        0        0    20333 2020-02-02 00:00:00.000000 sheetcode-0.0.4/screenshots/Traca2.png
--rw-r--r--   0        0        0    26660 2020-02-02 00:00:00.000000 sheetcode-0.0.4/screenshots/Traca3.png
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 sheetcode-0.0.4/src/SheetCode/Formatters.py
--rw-r--r--   0        0        0    10262 2020-02-02 00:00:00.000000 sheetcode-0.0.4/src/SheetCode/Sheet.py
--rw-r--r--   0        0        0     6325 2020-02-02 00:00:00.000000 sheetcode-0.0.4/src/SheetCode/Traceability.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sheetcode-0.0.4/src/SheetCode/__init__.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 sheetcode-0.0.4/LICENSE
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 sheetcode-0.0.4/README.md
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 sheetcode-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 sheetcode-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 sheetcode-0.0.5/SheetCode.code-workspace
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 sheetcode-0.0.5/.vscode/launch.json
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 sheetcode-0.0.5/example/UTest.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 sheetcode-0.0.5/example/run_all_scripts.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 sheetcode-0.0.5/example/run_one_script.py
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 sheetcode-0.0.5/example/scripts/BUTTONS_LIGHTS_Phase_1.py
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 sheetcode-0.0.5/example/scripts/BUTTONS_LIGHTS_Phase_2.py
+-rw-r--r--   0        0        0     9895 2020-02-02 00:00:00.000000 sheetcode-0.0.5/example/sheets/FCT_BUTTONS_LIGHTS_Phase_1_1A.xlsx
+-rw-r--r--   0        0        0     9999 2020-02-02 00:00:00.000000 sheetcode-0.0.5/example/sheets/FCT_BUTTONS_LIGHTS_Phase_2_1A.xlsx
+-rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 sheetcode-0.0.5/example/traceability/parameters.xlsx
+-rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 sheetcode-0.0.5/example/traceability/requirements.xlsx
+-rw-r--r--   0        0        0   404967 2020-02-02 00:00:00.000000 sheetcode-0.0.5/screenshots/Phase1.png
+-rw-r--r--   0        0        0    33450 2020-02-02 00:00:00.000000 sheetcode-0.0.5/screenshots/Phase1_XLS.png
+-rw-r--r--   0        0        0   710107 2020-02-02 00:00:00.000000 sheetcode-0.0.5/screenshots/Phase2.png
+-rw-r--r--   0        0        0    37177 2020-02-02 00:00:00.000000 sheetcode-0.0.5/screenshots/Phase2_XLS.png
+-rw-r--r--   0        0        0    50813 2020-02-02 00:00:00.000000 sheetcode-0.0.5/screenshots/Traca1.png
+-rw-r--r--   0        0        0    20333 2020-02-02 00:00:00.000000 sheetcode-0.0.5/screenshots/Traca2.png
+-rw-r--r--   0        0        0    26660 2020-02-02 00:00:00.000000 sheetcode-0.0.5/screenshots/Traca3.png
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 sheetcode-0.0.5/src/SheetCode/Formatters.py
+-rw-r--r--   0        0        0    10262 2020-02-02 00:00:00.000000 sheetcode-0.0.5/src/SheetCode/Sheet.py
+-rw-r--r--   0        0        0     6325 2020-02-02 00:00:00.000000 sheetcode-0.0.5/src/SheetCode/Traceability.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 sheetcode-0.0.5/src/SheetCode/__init__.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 sheetcode-0.0.5/LICENSE
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 sheetcode-0.0.5/README.md
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 sheetcode-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 sheetcode-0.0.5/PKG-INFO
```

### Comparing `sheetcode-0.0.4/BUTTONS_LIGHTS_Phase_2.py` & `sheetcode-0.0.5/example/scripts/BUTTONS_LIGHTS_Phase_2.py`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.4/.vscode/launch.json` & `sheetcode-0.0.5/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.4/example/run_all_scripts.py` & `sheetcode-0.0.5/example/run_all_scripts.py`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.4/example/run_one_script.py` & `sheetcode-0.0.5/example/run_one_script.py`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.4/example/scripts/BUTTONS_LIGHTS_Phase_1.py` & `sheetcode-0.0.5/example/scripts/BUTTONS_LIGHTS_Phase_1.py`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.4/example/sheets/FCT_BUTTONS_LIGHTS_Phase_1_1A.xlsx` & `sheetcode-0.0.5/example/sheets/FCT_BUTTONS_LIGHTS_Phase_1_1A.xlsx`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.4/example/sheets/FCT_BUTTONS_LIGHTS_Phase_2_1A.xlsx` & `sheetcode-0.0.5/example/sheets/FCT_BUTTONS_LIGHTS_Phase_2_1A.xlsx`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.4/example/traceability/parameters.xlsx` & `sheetcode-0.0.5/example/traceability/parameters.xlsx`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.4/example/traceability/requirements.xlsx` & `sheetcode-0.0.5/example/traceability/requirements.xlsx`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.4/screenshots/Phase1.png` & `sheetcode-0.0.5/screenshots/Phase1.png`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.4/screenshots/Phase1_XLS.png` & `sheetcode-0.0.5/screenshots/Phase1_XLS.png`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.4/screenshots/Phase2.png` & `sheetcode-0.0.5/screenshots/Phase2.png`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.4/screenshots/Phase2_XLS.png` & `sheetcode-0.0.5/screenshots/Phase2_XLS.png`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.4/screenshots/Traca1.png` & `sheetcode-0.0.5/screenshots/Traca1.png`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.4/screenshots/Traca2.png` & `sheetcode-0.0.5/screenshots/Traca2.png`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.4/screenshots/Traca3.png` & `sheetcode-0.0.5/screenshots/Traca3.png`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.4/src/SheetCode/Formatters.py` & `sheetcode-0.0.5/src/SheetCode/Formatters.py`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.4/src/SheetCode/Sheet.py` & `sheetcode-0.0.5/src/SheetCode/Sheet.py`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.4/src/SheetCode/Traceability.py` & `sheetcode-0.0.5/src/SheetCode/Traceability.py`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.4/LICENSE` & `sheetcode-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.4/PKG-INFO` & `sheetcode-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: SheetCode
-Version: 0.0.4
+Version: 0.0.5
 Summary: Generate Excel test sheets procedurally and verify traceability against requirements.
 Project-URL: Homepage, https://github.com/befr4ctal/SheetCode
 Project-URL: Issues, https://github.com/befr4ctal/SheetCode/issues
 Author-email: Thomas MARIN <thomas.marin@gmx.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

