# Comparing `tmp/sheetcode-0.0.3.tar.gz` & `tmp/sheetcode-0.0.4.tar.gz`

## Comparing `sheetcode-0.0.3.tar` & `sheetcode-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 sheetcode-0.0.3/SheetCode.code-workspace
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 sheetcode-0.0.3/.vscode/launch.json
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 sheetcode-0.0.3/example/UTest.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 sheetcode-0.0.3/example/run_all_scripts.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 sheetcode-0.0.3/example/run_one_script.py
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 sheetcode-0.0.3/example/scripts/BUTTONS_LIGHTS_Phase_1.py
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 sheetcode-0.0.3/example/scripts/BUTTONS_LIGHTS_Phase_2.py
--rw-r--r--   0        0        0     9895 2020-02-02 00:00:00.000000 sheetcode-0.0.3/example/sheets/FCT_BUTTONS_LIGHTS_Phase_1_1A.xlsx
--rw-r--r--   0        0        0     9999 2020-02-02 00:00:00.000000 sheetcode-0.0.3/example/sheets/FCT_BUTTONS_LIGHTS_Phase_2_1A.xlsx
--rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 sheetcode-0.0.3/example/traceability/parameters.xlsx
--rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 sheetcode-0.0.3/example/traceability/requirements.xlsx
--rw-r--r--   0        0        0   404967 2020-02-02 00:00:00.000000 sheetcode-0.0.3/screenshots/Phase1.png
--rw-r--r--   0        0        0    33450 2020-02-02 00:00:00.000000 sheetcode-0.0.3/screenshots/Phase1_XLS.png
--rw-r--r--   0        0        0   710107 2020-02-02 00:00:00.000000 sheetcode-0.0.3/screenshots/Phase2.png
--rw-r--r--   0        0        0    37177 2020-02-02 00:00:00.000000 sheetcode-0.0.3/screenshots/Phase2_XLS.png
--rw-r--r--   0        0        0    50813 2020-02-02 00:00:00.000000 sheetcode-0.0.3/screenshots/Traca1.png
--rw-r--r--   0        0        0    20333 2020-02-02 00:00:00.000000 sheetcode-0.0.3/screenshots/Traca2.png
--rw-r--r--   0        0        0    26660 2020-02-02 00:00:00.000000 sheetcode-0.0.3/screenshots/Traca3.png
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 sheetcode-0.0.3/src/SheetCode/Formatters.py
--rw-r--r--   0        0        0    10243 2020-02-02 00:00:00.000000 sheetcode-0.0.3/src/SheetCode/Sheet.py
--rw-r--r--   0        0        0     6325 2020-02-02 00:00:00.000000 sheetcode-0.0.3/src/SheetCode/Traceability.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sheetcode-0.0.3/src/SheetCode/__init__.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 sheetcode-0.0.3/LICENSE
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 sheetcode-0.0.3/README.md
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 sheetcode-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 sheetcode-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 sheetcode-0.0.4/BUTTONS_LIGHTS_Phase_2.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 sheetcode-0.0.4/SheetCode.code-workspace
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 sheetcode-0.0.4/.vscode/launch.json
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 sheetcode-0.0.4/example/UTest.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 sheetcode-0.0.4/example/run_all_scripts.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 sheetcode-0.0.4/example/run_one_script.py
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 sheetcode-0.0.4/example/scripts/BUTTONS_LIGHTS_Phase_1.py
+-rw-r--r--   0        0        0     9895 2020-02-02 00:00:00.000000 sheetcode-0.0.4/example/sheets/FCT_BUTTONS_LIGHTS_Phase_1_1A.xlsx
+-rw-r--r--   0        0        0     9999 2020-02-02 00:00:00.000000 sheetcode-0.0.4/example/sheets/FCT_BUTTONS_LIGHTS_Phase_2_1A.xlsx
+-rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 sheetcode-0.0.4/example/traceability/parameters.xlsx
+-rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 sheetcode-0.0.4/example/traceability/requirements.xlsx
+-rw-r--r--   0        0        0   404967 2020-02-02 00:00:00.000000 sheetcode-0.0.4/screenshots/Phase1.png
+-rw-r--r--   0        0        0    33450 2020-02-02 00:00:00.000000 sheetcode-0.0.4/screenshots/Phase1_XLS.png
+-rw-r--r--   0        0        0   710107 2020-02-02 00:00:00.000000 sheetcode-0.0.4/screenshots/Phase2.png
+-rw-r--r--   0        0        0    37177 2020-02-02 00:00:00.000000 sheetcode-0.0.4/screenshots/Phase2_XLS.png
+-rw-r--r--   0        0        0    50813 2020-02-02 00:00:00.000000 sheetcode-0.0.4/screenshots/Traca1.png
+-rw-r--r--   0        0        0    20333 2020-02-02 00:00:00.000000 sheetcode-0.0.4/screenshots/Traca2.png
+-rw-r--r--   0        0        0    26660 2020-02-02 00:00:00.000000 sheetcode-0.0.4/screenshots/Traca3.png
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 sheetcode-0.0.4/src/SheetCode/Formatters.py
+-rw-r--r--   0        0        0    10262 2020-02-02 00:00:00.000000 sheetcode-0.0.4/src/SheetCode/Sheet.py
+-rw-r--r--   0        0        0     6325 2020-02-02 00:00:00.000000 sheetcode-0.0.4/src/SheetCode/Traceability.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sheetcode-0.0.4/src/SheetCode/__init__.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 sheetcode-0.0.4/LICENSE
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 sheetcode-0.0.4/README.md
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 sheetcode-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 sheetcode-0.0.4/PKG-INFO
```

### Comparing `sheetcode-0.0.3/example/run_all_scripts.py` & `sheetcode-0.0.4/example/run_all_scripts.py`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.3/example/run_one_script.py` & `sheetcode-0.0.4/example/run_one_script.py`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.3/example/scripts/BUTTONS_LIGHTS_Phase_1.py` & `sheetcode-0.0.4/example/scripts/BUTTONS_LIGHTS_Phase_1.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from SheetCode import Sheet
+from src.SheetCode import Sheet
 
 sheet = Sheet("FCT", __file__)
 
 sheet.Name = "Buttons and lights"
 sheet.Version = "1A"
 sheet.Description = ["This test sheets covers the buttons and lights of all colors",
                         "We will test each button and check that the expected lights are lit on"]
```

### Comparing `sheetcode-0.0.3/example/scripts/BUTTONS_LIGHTS_Phase_2.py` & `sheetcode-0.0.4/BUTTONS_LIGHTS_Phase_2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from SheetCode import Sheet
-import UTest
+import example.UTest as UTest
 
 sheet = Sheet("FCT", __file__)
 
 sheet.Name = "Buttons and lights"
 sheet.Version = "1A"
 sheet.Description = ["This test sheets covers the buttons and lights of all colors",
                         "We will test each button and check that the expected lights are lit on"]
```

### Comparing `sheetcode-0.0.3/example/sheets/FCT_BUTTONS_LIGHTS_Phase_1_1A.xlsx` & `sheetcode-0.0.4/example/sheets/FCT_BUTTONS_LIGHTS_Phase_1_1A.xlsx`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.3/example/sheets/FCT_BUTTONS_LIGHTS_Phase_2_1A.xlsx` & `sheetcode-0.0.4/example/sheets/FCT_BUTTONS_LIGHTS_Phase_2_1A.xlsx`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.3/example/traceability/parameters.xlsx` & `sheetcode-0.0.4/example/traceability/parameters.xlsx`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.3/example/traceability/requirements.xlsx` & `sheetcode-0.0.4/example/traceability/requirements.xlsx`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.3/screenshots/Phase1.png` & `sheetcode-0.0.4/screenshots/Phase1.png`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.3/screenshots/Phase1_XLS.png` & `sheetcode-0.0.4/screenshots/Phase1_XLS.png`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.3/screenshots/Phase2.png` & `sheetcode-0.0.4/screenshots/Phase2.png`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.3/screenshots/Phase2_XLS.png` & `sheetcode-0.0.4/screenshots/Phase2_XLS.png`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.3/screenshots/Traca1.png` & `sheetcode-0.0.4/screenshots/Traca1.png`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.3/screenshots/Traca2.png` & `sheetcode-0.0.4/screenshots/Traca2.png`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.3/screenshots/Traca3.png` & `sheetcode-0.0.4/screenshots/Traca3.png`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.3/src/SheetCode/Formatters.py` & `sheetcode-0.0.4/src/SheetCode/Formatters.py`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.3/src/SheetCode/Sheet.py` & `sheetcode-0.0.4/src/SheetCode/Sheet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from openpyxl.workbook import Workbook # need pip install openpyxl
 from pathlib import Path
 from src.SheetCode import Traceability as Traceability
 from termcolor import colored # need pip install termcolor
-import Formatters as Formatters
+from src.SheetCode import Formatters as Formatters
 from enum import Enum
 
 
 class Sheet:
     global TsWorkbook
     global Ts
```

### Comparing `sheetcode-0.0.3/src/SheetCode/Traceability.py` & `sheetcode-0.0.4/src/SheetCode/Traceability.py`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.3/LICENSE` & `sheetcode-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.3/pyproject.toml` & `sheetcode-0.0.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "pandas", "openpyxl", "termcolor", "tabulate"]
 build-backend = "hatchling.build"
 
 [project]
 name = "SheetCode"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Thomas MARIN", email="thomas.marin@gmx.com" },
 ]
 description = "Generate Excel test sheets procedurally and verify traceability against requirements."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `sheetcode-0.0.3/PKG-INFO` & `sheetcode-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: SheetCode
-Version: 0.0.3
+Version: 0.0.4
 Summary: Generate Excel test sheets procedurally and verify traceability against requirements.
 Project-URL: Homepage, https://github.com/befr4ctal/SheetCode
 Project-URL: Issues, https://github.com/befr4ctal/SheetCode/issues
 Author-email: Thomas MARIN <thomas.marin@gmx.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

