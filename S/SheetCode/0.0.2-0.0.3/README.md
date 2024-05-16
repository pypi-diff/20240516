# Comparing `tmp/sheetcode-0.0.2.tar.gz` & `tmp/sheetcode-0.0.3.tar.gz`

## Comparing `sheetcode-0.0.2.tar` & `sheetcode-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 sheetcode-0.0.2/SheetCode.code-workspace
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 sheetcode-0.0.2/.vscode/launch.json
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 sheetcode-0.0.2/example/UTest.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 sheetcode-0.0.2/example/run_all_scripts.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 sheetcode-0.0.2/example/run_one_script.py
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 sheetcode-0.0.2/example/scripts/BUTTONS_LIGHTS_Phase_1.py
--rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 sheetcode-0.0.2/example/scripts/BUTTONS_LIGHTS_Phase_2.py
--rw-r--r--   0        0        0     9895 2020-02-02 00:00:00.000000 sheetcode-0.0.2/example/sheets/FCT_BUTTONS_LIGHTS_Phase_1_1A.xlsx
--rw-r--r--   0        0        0     6114 2020-02-02 00:00:00.000000 sheetcode-0.0.2/example/sheets/FCT_BUTTONS_LIGHTS_Phase_2_1A.xlsx
--rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 sheetcode-0.0.2/example/traceability/parameters.xlsx
--rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 sheetcode-0.0.2/example/traceability/requirements.xlsx
--rw-r--r--   0        0        0   404967 2020-02-02 00:00:00.000000 sheetcode-0.0.2/screenshots/Phase1.png
--rw-r--r--   0        0        0    33450 2020-02-02 00:00:00.000000 sheetcode-0.0.2/screenshots/Phase1_XLS.png
--rw-r--r--   0        0        0   710107 2020-02-02 00:00:00.000000 sheetcode-0.0.2/screenshots/Phase2.png
--rw-r--r--   0        0        0    37177 2020-02-02 00:00:00.000000 sheetcode-0.0.2/screenshots/Phase2_XLS.png
--rw-r--r--   0        0        0    50813 2020-02-02 00:00:00.000000 sheetcode-0.0.2/screenshots/Traca1.png
--rw-r--r--   0        0        0    20333 2020-02-02 00:00:00.000000 sheetcode-0.0.2/screenshots/Traca2.png
--rw-r--r--   0        0        0    26660 2020-02-02 00:00:00.000000 sheetcode-0.0.2/screenshots/Traca3.png
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 sheetcode-0.0.2/src/SheetCode/Formatters.py
--rw-r--r--   0        0        0    10224 2020-02-02 00:00:00.000000 sheetcode-0.0.2/src/SheetCode/Sheet.py
--rw-r--r--   0        0        0     6325 2020-02-02 00:00:00.000000 sheetcode-0.0.2/src/SheetCode/Traceability.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sheetcode-0.0.2/src/SheetCode/__init__.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 sheetcode-0.0.2/LICENSE
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 sheetcode-0.0.2/README.md
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 sheetcode-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 sheetcode-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 sheetcode-0.0.3/SheetCode.code-workspace
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 sheetcode-0.0.3/.vscode/launch.json
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 sheetcode-0.0.3/example/UTest.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 sheetcode-0.0.3/example/run_all_scripts.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 sheetcode-0.0.3/example/run_one_script.py
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 sheetcode-0.0.3/example/scripts/BUTTONS_LIGHTS_Phase_1.py
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 sheetcode-0.0.3/example/scripts/BUTTONS_LIGHTS_Phase_2.py
+-rw-r--r--   0        0        0     9895 2020-02-02 00:00:00.000000 sheetcode-0.0.3/example/sheets/FCT_BUTTONS_LIGHTS_Phase_1_1A.xlsx
+-rw-r--r--   0        0        0     9999 2020-02-02 00:00:00.000000 sheetcode-0.0.3/example/sheets/FCT_BUTTONS_LIGHTS_Phase_2_1A.xlsx
+-rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 sheetcode-0.0.3/example/traceability/parameters.xlsx
+-rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 sheetcode-0.0.3/example/traceability/requirements.xlsx
+-rw-r--r--   0        0        0   404967 2020-02-02 00:00:00.000000 sheetcode-0.0.3/screenshots/Phase1.png
+-rw-r--r--   0        0        0    33450 2020-02-02 00:00:00.000000 sheetcode-0.0.3/screenshots/Phase1_XLS.png
+-rw-r--r--   0        0        0   710107 2020-02-02 00:00:00.000000 sheetcode-0.0.3/screenshots/Phase2.png
+-rw-r--r--   0        0        0    37177 2020-02-02 00:00:00.000000 sheetcode-0.0.3/screenshots/Phase2_XLS.png
+-rw-r--r--   0        0        0    50813 2020-02-02 00:00:00.000000 sheetcode-0.0.3/screenshots/Traca1.png
+-rw-r--r--   0        0        0    20333 2020-02-02 00:00:00.000000 sheetcode-0.0.3/screenshots/Traca2.png
+-rw-r--r--   0        0        0    26660 2020-02-02 00:00:00.000000 sheetcode-0.0.3/screenshots/Traca3.png
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 sheetcode-0.0.3/src/SheetCode/Formatters.py
+-rw-r--r--   0        0        0    10243 2020-02-02 00:00:00.000000 sheetcode-0.0.3/src/SheetCode/Sheet.py
+-rw-r--r--   0        0        0     6325 2020-02-02 00:00:00.000000 sheetcode-0.0.3/src/SheetCode/Traceability.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sheetcode-0.0.3/src/SheetCode/__init__.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 sheetcode-0.0.3/LICENSE
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 sheetcode-0.0.3/README.md
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 sheetcode-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 sheetcode-0.0.3/PKG-INFO
```

### Comparing `sheetcode-0.0.2/example/run_all_scripts.py` & `sheetcode-0.0.3/example/run_all_scripts.py`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.2/example/run_one_script.py` & `sheetcode-0.0.3/example/run_one_script.py`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.2/example/scripts/BUTTONS_LIGHTS_Phase_1.py` & `sheetcode-0.0.3/example/scripts/BUTTONS_LIGHTS_Phase_1.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from TestSheet import Sheet
+from SheetCode import Sheet
 
 sheet = Sheet("FCT", __file__)
 
 sheet.Name = "Buttons and lights"
 sheet.Version = "1A"
 sheet.Description = ["This test sheets covers the buttons and lights of all colors",
                         "We will test each button and check that the expected lights are lit on"]
 
 sheet.StartConditions = ["No button is pressed",
                          "No light is lit on"]
 
 # *********************************
-sheet.Case("Case A: Yellow light is managed")
+sheet.Case("Yellow light is managed")
 
 sheet.Action("Press and maintain the yellow button")
 
 sheet.ExpectedResult("The yellow lights turns on and remains on",
                         requirements = ["[SIMPLE_REQ_1]"],
                         parameters = ["parameters/yellow_light_enabled"])
 sheet.ExpectedResult("The red light remains off",
                         requirements = ["[SIMPLE_REQ_2]"])
 
 sheet.Action("Release the yellow button")
 
 sheet.ExpectedResult("The yellow light turns off")
 
 # *********************************
-sheet.Case("Case B: Red light is not managed")
+sheet.Case("Red light is not managed")
 
 sheet.Action("Press and maintain the red button")
 
 sheet.ExpectedResult("The red light turns DOES NOT turn on",
                         requirements = ["[SIMPLE_REQ_3]"],
                         parameters = ["parameters/red_light_enabled"])
```

### Comparing `sheetcode-0.0.2/example/scripts/BUTTONS_LIGHTS_Phase_2.py` & `sheetcode-0.0.3/example/scripts/BUTTONS_LIGHTS_Phase_2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from TestSheet import Sheet
+from SheetCode import Sheet
 import UTest
 
 sheet = Sheet("FCT", __file__)
 
 sheet.Name = "Buttons and lights"
 sheet.Version = "1A"
 sheet.Description = ["This test sheets covers the buttons and lights of all colors",
@@ -10,15 +10,15 @@
 
 sheet.StartConditions = ["No button is pressed",
                          "No light is lit on"]
 
 canLogFilename = UTest.StartCanLog(__file__)
 
 # *********************************
-sheet.Case("Case A: Yellow light is managed")
+sheet.Case("Yellow light is managed")
 
 sheet.Action("Press and maintain the yellow button")
 UTest.SetVariable("YELLOW_BUTTON", True)
 
 sheet.ExpectedResult("The yellow lights turns on and remains on",
                         requirements = ["[SIMPLE_REQ_1]"],
                         parameters = ["parameters/yellow_light_enabled"])
@@ -39,15 +39,15 @@
 
 sheet.ExpectedResult("The yellow light turns off")
 yellowLightState = UTest.GetVariable("YELLOW_LIGHT")
 result = yellowLightState == False
 sheet.Result(result, f"The state of Yellow light is {result}")
 
 # *********************************
-sheet.Case("Case B: Red light is not managed")
+sheet.Case("Red light is not managed")
 
 sheet.Action("Press and maintain the red button")
 
 UTest.SetVariable("RED_BUTTON", True)
 
 sheet.ExpectedResult("The red lights turns DOES NOT turn on",
                         requirements = ["[SIMPLE_REQ_3]"],
```

### Comparing `sheetcode-0.0.2/example/sheets/FCT_BUTTONS_LIGHTS_Phase_1_1A.xlsx` & `sheetcode-0.0.3/example/sheets/FCT_BUTTONS_LIGHTS_Phase_1_1A.xlsx`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.2/example/traceability/parameters.xlsx` & `sheetcode-0.0.3/example/traceability/parameters.xlsx`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.2/example/traceability/requirements.xlsx` & `sheetcode-0.0.3/example/traceability/requirements.xlsx`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.2/screenshots/Phase1.png` & `sheetcode-0.0.3/screenshots/Phase1.png`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.2/screenshots/Phase1_XLS.png` & `sheetcode-0.0.3/screenshots/Phase1_XLS.png`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.2/screenshots/Phase2.png` & `sheetcode-0.0.3/screenshots/Phase2.png`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.2/screenshots/Phase2_XLS.png` & `sheetcode-0.0.3/screenshots/Phase2_XLS.png`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.2/screenshots/Traca1.png` & `sheetcode-0.0.3/screenshots/Traca1.png`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.2/screenshots/Traca2.png` & `sheetcode-0.0.3/screenshots/Traca2.png`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.2/screenshots/Traca3.png` & `sheetcode-0.0.3/screenshots/Traca3.png`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.2/src/SheetCode/Formatters.py` & `sheetcode-0.0.3/src/SheetCode/Formatters.py`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.2/src/SheetCode/Sheet.py` & `sheetcode-0.0.3/src/SheetCode/Sheet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from openpyxl.workbook import Workbook # need pip install openpyxl
 from pathlib import Path
-import Traceability as Traceability
+from src.SheetCode import Traceability as Traceability
 from termcolor import colored # need pip install termcolor
 import Formatters as Formatters
 from enum import Enum
 
 
 class Sheet:
     global TsWorkbook
```

### Comparing `sheetcode-0.0.2/src/SheetCode/Traceability.py` & `sheetcode-0.0.3/src/SheetCode/Traceability.py`

 * *Files identical despite different names*

### Comparing `sheetcode-0.0.2/LICENSE` & `sheetcode-0.0.3/LICENSE`

 * *Files identical despite different names*

