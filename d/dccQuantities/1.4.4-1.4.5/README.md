# Comparing `tmp/dccquantities-1.4.4.tar.gz` & `tmp/dccquantities-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dccquantities-1.4.4.tar", last modified: Tue Apr 30 10:53:58 2024, max compression
+gzip compressed data, was "dccquantities-1.4.5.tar", last modified: Thu May 16 17:23:12 2024, max compression
```

## Comparing `dccquantities-1.4.4.tar` & `dccquantities-1.4.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 seeger01  (1000) seeger01  (1000)        0 2024-04-30 10:53:58.616882 dccquantities-1.4.4/
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)    26516 2024-04-29 13:28:01.000000 dccquantities-1.4.4/LICENSE
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)     1939 2024-04-30 10:53:58.616882 dccquantities-1.4.4/PKG-INFO
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)     1129 2024-04-30 07:44:37.000000 dccquantities-1.4.4/README.md
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)       80 2023-10-04 11:27:28.000000 dccquantities-1.4.4/pyproject.toml
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)      633 2024-04-30 10:53:58.616882 dccquantities-1.4.4/setup.cfg
-drwxr-xr-x   0 seeger01  (1000) seeger01  (1000)        0 2024-04-30 10:53:58.615882 dccquantities-1.4.4/src/
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)        0 2024-04-29 13:28:01.000000 dccquantities-1.4.4/src/__init__.py
-drwxr-xr-x   0 seeger01  (1000) seeger01  (1000)        0 2024-04-30 10:53:58.616882 dccquantities-1.4.4/src/dccQuantities.egg-info/
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)     1939 2024-04-30 10:53:58.000000 dccquantities-1.4.4/src/dccQuantities.egg-info/PKG-INFO
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)      398 2024-04-30 10:53:58.000000 dccquantities-1.4.4/src/dccQuantities.egg-info/SOURCES.txt
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)        1 2024-04-30 10:53:58.000000 dccquantities-1.4.4/src/dccQuantities.egg-info/dependency_links.txt
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)      162 2024-04-30 10:53:58.000000 dccquantities-1.4.4/src/dccQuantities.egg-info/requires.txt
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)       68 2024-04-30 10:53:58.000000 dccquantities-1.4.4/src/dccQuantities.egg-info/top_level.txt
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)    68685 2024-04-30 10:30:04.000000 dccquantities-1.4.4/src/dccQuantities.py
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)     1931 2024-04-30 07:43:13.000000 dccquantities-1.4.4/src/dccQuantitiesConfiguration.py
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)    12041 2024-04-30 10:20:10.000000 dccquantities-1.4.4/src/dccQuantitiesPlot.py
-drwxr-xr-x   0 seeger01  (1000) seeger01  (1000)        0 2024-04-30 10:53:58.616882 dccquantities-1.4.4/tests/
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)    17811 2024-04-30 10:53:26.000000 dccquantities-1.4.4/tests/test_dccQuantsAndTabs.py
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)     2393 2024-04-30 07:43:13.000000 dccquantities-1.4.4/tests/test_tollerance.py
+drwxr-xr-x   0 seeger01  (1000) seeger01  (1000)        0 2024-05-16 17:23:12.619917 dccquantities-1.4.5/
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)    26516 2024-04-29 13:28:01.000000 dccquantities-1.4.5/LICENSE
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)     1711 2024-05-16 17:23:12.619917 dccquantities-1.4.5/PKG-INFO
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)      901 2024-05-16 17:21:14.000000 dccquantities-1.4.5/README.md
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)       80 2023-10-04 11:27:28.000000 dccquantities-1.4.5/pyproject.toml
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)      633 2024-05-16 17:23:12.619917 dccquantities-1.4.5/setup.cfg
+drwxr-xr-x   0 seeger01  (1000) seeger01  (1000)        0 2024-05-16 17:23:12.618917 dccquantities-1.4.5/src/
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)        0 2024-04-29 13:28:01.000000 dccquantities-1.4.5/src/__init__.py
+drwxr-xr-x   0 seeger01  (1000) seeger01  (1000)        0 2024-05-16 17:23:12.619917 dccquantities-1.4.5/src/dccQuantities.egg-info/
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)     1711 2024-05-16 17:23:12.000000 dccquantities-1.4.5/src/dccQuantities.egg-info/PKG-INFO
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)      398 2024-05-16 17:23:12.000000 dccquantities-1.4.5/src/dccQuantities.egg-info/SOURCES.txt
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)        1 2024-05-16 17:23:12.000000 dccquantities-1.4.5/src/dccQuantities.egg-info/dependency_links.txt
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)      162 2024-05-16 17:23:12.000000 dccquantities-1.4.5/src/dccQuantities.egg-info/requires.txt
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)       68 2024-05-16 17:23:12.000000 dccquantities-1.4.5/src/dccQuantities.egg-info/top_level.txt
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)    69914 2024-05-16 17:21:14.000000 dccquantities-1.4.5/src/dccQuantities.py
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)     1931 2024-04-30 07:43:13.000000 dccquantities-1.4.5/src/dccQuantitiesConfiguration.py
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)    12041 2024-04-30 10:56:11.000000 dccquantities-1.4.5/src/dccQuantitiesPlot.py
+drwxr-xr-x   0 seeger01  (1000) seeger01  (1000)        0 2024-05-16 17:23:12.619917 dccquantities-1.4.5/tests/
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)    20301 2024-05-16 17:21:14.000000 dccquantities-1.4.5/tests/test_dccQuantsAndTabs.py
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)     2393 2024-04-30 07:43:13.000000 dccquantities-1.4.5/tests/test_tollerance.py
```

### Comparing `dccquantities-1.4.4/LICENSE` & `dccquantities-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dccquantities-1.4.4/PKG-INFO` & `dccquantities-1.4.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dccQuantities
-Version: 1.4.4
+Version: 1.4.5
 Summary: Python classes for working with DDC calibration data
 Home-page: https://gitlab1.ptb.de/digitaldynamicmeasurement/dccQuantities
 Author: Benedikt Seeger, Vanessa Stehr, Thomas Bruns
 Author-email: benedikt.seeger@ptb.de
 License: LGPL-2.1-or-later
 Requires-Python: >=3.10
 License-File: LICENSE
@@ -20,17 +20,14 @@
 Requires-Dist: dccXMLJSONConv
 Provides-Extra: dccquantitiesplot
 Requires-Dist: bokeh; extra == "dccquantitiesplot"
 Provides-Extra: testing
 Requires-Dist: pytest==7.4.1; extra == "testing"
 Requires-Dist: pytest-cov==4.1.0; extra == "testing"
 
-![pipeline](https://gitlab1.ptb.de/digitaldynamicmeasurement/py-dsi-vectors-and-tables/badges/main/pipeline.svg)
-![coverage](https://gitlab1.ptb.de/digitaldynamicmeasurement/py-dsi-vectors-and-tables/badges/main/coverage.svg) 
-
 ## Content
 This repo contains a collection of tools for working with DSI Quantitys (Vectors [even with only on value]) and list of DSI Quantitys (Tables).
 As well as the tools needed to generate visualisations of the data. Using Bokeh
 # Visualisation
 ![Image of DSI Multivectorplot showing Gui Elements to change language, lin/log axis and selected Index](/doc/mvPloter.png)
 
 ## Installation
```

### Comparing `dccquantities-1.4.4/README.md` & `dccquantities-1.4.5/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-![pipeline](https://gitlab1.ptb.de/digitaldynamicmeasurement/py-dsi-vectors-and-tables/badges/main/pipeline.svg)
-![coverage](https://gitlab1.ptb.de/digitaldynamicmeasurement/py-dsi-vectors-and-tables/badges/main/coverage.svg) 
-
 ## Content
 This repo contains a collection of tools for working with DSI Quantitys (Vectors [even with only on value]) and list of DSI Quantitys (Tables).
 As well as the tools needed to generate visualisations of the data. Using Bokeh
 # Visualisation
 ![Image of DSI Multivectorplot showing Gui Elements to change language, lin/log axis and selected Index](/doc/mvPloter.png)
 
 ## Installation
```

### Comparing `dccquantities-1.4.4/setup.cfg` & `dccquantities-1.4.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dccQuantities
-version = 1.4.4
+version = 1.4.5
 description = Python classes for working with DDC calibration data
 long_description = file: README.md
 license = LGPL-2.1-or-later
 author = Benedikt Seeger, Vanessa Stehr, Thomas Bruns
 author_email = benedikt.seeger@ptb.de
 url = https://gitlab1.ptb.de/digitaldynamicmeasurement/dccQuantities
```

### Comparing `dccquantities-1.4.4/src/dccQuantities.egg-info/PKG-INFO` & `dccquantities-1.4.5/src/dccQuantities.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dccQuantities
-Version: 1.4.4
+Version: 1.4.5
 Summary: Python classes for working with DDC calibration data
 Home-page: https://gitlab1.ptb.de/digitaldynamicmeasurement/dccQuantities
 Author: Benedikt Seeger, Vanessa Stehr, Thomas Bruns
 Author-email: benedikt.seeger@ptb.de
 License: LGPL-2.1-or-later
 Requires-Python: >=3.10
 License-File: LICENSE
@@ -20,17 +20,14 @@
 Requires-Dist: dccXMLJSONConv
 Provides-Extra: dccquantitiesplot
 Requires-Dist: bokeh; extra == "dccquantitiesplot"
 Provides-Extra: testing
 Requires-Dist: pytest==7.4.1; extra == "testing"
 Requires-Dist: pytest-cov==4.1.0; extra == "testing"
 
-![pipeline](https://gitlab1.ptb.de/digitaldynamicmeasurement/py-dsi-vectors-and-tables/badges/main/pipeline.svg)
-![coverage](https://gitlab1.ptb.de/digitaldynamicmeasurement/py-dsi-vectors-and-tables/badges/main/coverage.svg) 
-
 ## Content
 This repo contains a collection of tools for working with DSI Quantitys (Vectors [even with only on value]) and list of DSI Quantitys (Tables).
 As well as the tools needed to generate visualisations of the data. Using Bokeh
 # Visualisation
 ![Image of DSI Multivectorplot showing Gui Elements to change language, lin/log axis and selected Index](/doc/mvPloter.png)
 
 ## Installation
```

### Comparing `dccquantities-1.4.4/src/dccQuantities.py` & `dccquantities-1.4.5/src/dccQuantities.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,14 +269,15 @@
     languages = set(first.keys()) | set(second.keys())
     for lang in languages:
         try:
             resultDict[lang]=str(first[lang])+' '+str(operator)+' '+str(second[lang])
         except KeyError:
             warnings.warn("Key Error in Multilang name creation for language "+str(lang))
     return resultDict
+
 class dccQuantity:
     """represents a value vector with uncer, can be serialized to both JSON and XML"""
 
     supportedUncerTypes = ["absolute", "rel", "relPercent", "relPPM"]
 
     def __init__(
         self,
@@ -320,29 +321,36 @@
         elif type(unit) == str:
             self.unit = dsiUnit(unit)
         else:
             self.unit = dsiUnit(str(unit))
         if refTypes is not None:
             try:
                 self.refTypes = list(refTypes.split(" "))
+
             except:
-                self.refTypes = list(refTypes)
+                try:
+                    self.refTypes = list(refTypes)
+                except Exception as E:
+                    warnings.warn(
+                        "refTypes could not be converted to a list due to,"+str(E)+" using None"
+                    )
+                    self.refTypes=None
         else:
             self.refTypes = None
         self.multilangnames = name
         #TODO implement better handling for uncerParams
         if type(values) == int or type(values) == float:
             values = np.array([values])
         if type(uncer) == int or type(uncer) == float:
             uncer = np.array([uncer])
         if values.dtype == 'O':
             self.uarray = values
             try:
-                self.values = unumpy.nominal_values(self.uarray)
-                self.uncer = unumpy.std_devs(self.uarray)
+                self.values = unumpy.nominal_values(self.uarray)#TODO remove this variables and use only the uncerFlaot data
+                self.uncer = unumpy.std_devs(self.uarray)#TODO remove this variables and use only the uncerFlaot data
                 self.originalUncerType = "absolute" #uncertanies from uarray are always absolute
                 self.uncerParams=uncerParams # set to default uncer params since we don't know beeter
             except Exception as e:
                 new_message = f"An error occurred while extracting nominal values and uncertainties Mostlikly the valus havent been an ufloat/uarray : {str(e)}"
                 raise type(e)(new_message) from e
         else:
             self.uncerParams = {}
@@ -352,15 +360,15 @@
                 self.values = values
             else:
                 self.values = np.array(values)
             if type(uncer) == type(None):
                 self.originalUncerType = None
                 self.uncer = (
                     np.zeros_like(values) * np.NaN
-                )  # TODO some how this is changed to None when copied why ? WTF
+                )
             else:
                 # TODO better uncer handling with function dict
                 if (
                     type(uncer) != np.array
                 ):  # if its not an array try to convert in np.ndarray
                     uncer = np.array(uncer)
                 # __uncer__ handling
@@ -752,14 +760,33 @@
             )
             return new_vector
         else:
             raise ValueError(
                 "newVecFromIdx only possible with a slice, np.ndarray (dtype int), or list of ints, not with " + str(
                     type(idx)))
 
+    def convertToUnit(self, newUnit: [str,dsiUnit]):
+        """converts the values and uncer to a new unit
+        Args:
+            newUnit (str): new unit
+        """
+        if type(newUnit) == str:
+            newUnit = dsiUnit(newUnit)
+        if self.unit == newUnit:
+            return
+        scaleFactor,baseUnit = newUnit.isScalablyEqualTo(self.unit) # n*self.unit =1 other.unit
+        if baseUnit is not None:
+            self.uarray = self.uarray * scaleFactor
+            self.values = unumpy.nominal_values(
+                self.uarray)  # TODO remove this variables and use only the uncerFlaot data
+            self.uncer = unumpy.std_devs(self.uarray)  # TODO remove this variables and use only the uncerFlaot data
+            self.unit = newUnit
+        else:
+            raise ValueError("Actual unit "+str(self.unit.toUTF8())+" and new unit"+str(newUnit.toUTF8())+" are not scalably equal")
+
     def __getitem__(self, item):
         """See pyDCCToolsExamplesNoteBook.ipynb for detailed indexing Examples"""
         # print(key)
         if type(item) == int:
             if self.originalUncerType is not None:
                 return (self.values[item], self.uncer[item])
             else:
```

### Comparing `dccquantities-1.4.4/src/dccQuantitiesConfiguration.py` & `dccquantities-1.4.5/src/dccQuantitiesConfiguration.py`

 * *Files identical despite different names*

### Comparing `dccquantities-1.4.4/src/dccQuantitiesPlot.py` & `dccquantities-1.4.5/src/dccQuantitiesPlot.py`

 * *Files identical despite different names*

### Comparing `dccquantities-1.4.4/tests/test_dccQuantsAndTabs.py` & `dccquantities-1.4.5/tests/test_dccQuantsAndTabs.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 import json
 import os
 import re
 import pytest
 import numpy as np
 from dccQuantities import dccQuantity,dccQuantityTable,dsiJSONEncoder
+from dsiUnits import dsiUnit
 def remove_whitespacesFromXML(s):
     # Replace all whitespace chars except newline
     s = re.sub(r'[\t\r\f\v]+', '', s)
     # Remove all spaces around newlines
     s = re.sub(r' *\n *', '\n', s)
     # Remove empty lines
     s = re.sub(r'\n\n', '\n', s)
@@ -63,14 +64,37 @@
     assert np.all(testVector['uncer',5:10] == 0.1 / 100 * testVector['values',5:10])
     np.testing.assert_allclose(testVector['values',10:12], np.array([5.5,6.0]))
     with pytest.raises(IndexError) as idxError:
         testVector['uncer_relPercent', 1000]
     assert str(idxError.value) == "index 1000 is out of bounds for axis 0 with size 20"
     assert testVector['refTypes'] == ["vib_Test"]
 
+def test_singelVectorWithNanRefTypes():
+    testVector=dccQuantity((np.arange(20) + 1) * 0.5, np.ones(20) * 0.1, 'Frequency', r'\hertz', uncerType="relPercent",
+                           refTypes=np.NAN, name={'EN': 'Frequency', 'DE': 'Frequenz'})
+    assert testVector.length == 20
+    assert len(testVector) == 20
+    assert str(testVector['unit']) == r'\hertz'
+    assert testVector[9] == (5 , 0.005)
+    assert testVector[4] == (2.5, 0.0025)
+    np.testing.assert_allclose(testVector['values'], (np.arange(20) + 1) * 0.5)
+    assert testVector['quantity'] == 'Frequency'
+    assert testVector['uncer_relPercent',5] == 0.1
+    assert testVector['uncer_relPercent'][5] == 0.1
+    assert testVector['uncer_rel',5] == 0.1/100
+    assert testVector['uncer_rel'][5] == 0.1/100
+    assert testVector['uncer'][5] == 0.1 / 100*testVector['values'][5]
+    assert np.all(testVector['uncer'][5:10] == 0.1 / 100*testVector['values'][5:10])
+    assert np.all(testVector['uncer',5:10] == 0.1 / 100 * testVector['values',5:10])
+    np.testing.assert_allclose(testVector['values',10:12], np.array([5.5,6.0]))
+    with pytest.raises(IndexError) as idxError:
+        testVector['uncer_relPercent', 1000]
+    assert str(idxError.value) == "index 1000 is out of bounds for axis 0 with size 20"
+    assert testVector['refTypes'] == None
+
 def test_multiVector():
     testDSiVectorFreq = dccQuantity((np.arange(20) + 1) * 0.5, np.ones(20) * 0.1, 'Frequency', r'\hertz', uncerType="relPercent", refTypes=["vib_Test"], name={'EN': 'Frequency', 'DE': 'Frequenz'})
     testDsiVectorMag = dccQuantity((np.arange(20) + 1) * 5, np.ones(20) * 0.1, 'Magnitude', r'\volt', uncerType="relPercent")
     testDsiVectorPhase = dccQuantity((np.arange(20) + 1) * 0.1 * np.pi, np.ones(20) * 0.1, 'Phase', r'\radian', uncerType="relPercent")
     testMultVectorMultiIndex = dccQuantityTable([testDSiVectorFreq], [testDsiVectorMag, testDsiVectorPhase])
     assert testMultVectorMultiIndex['index'][0]['quantity'] == 'Frequency'
     assert testMultVectorMultiIndex['index'][0] == testDSiVectorFreq
@@ -273,7 +297,26 @@
 
 def test_additionWithSiPrfix2():
     testDsiVectorMag1 = dccQuantity((np.arange(20) + 1) * 5, np.ones(20) * 0.1, 'Magnitude', r'\volt', uncerType="relPercent", name={'EN': 'Magnitude', 'DE': 'Magnitude'})
     testDsiVectorMag2 = dccQuantity(1.0, 0.1, 'Magnitude Offset', r'\kilo\volt',
                                     uncerType="relPercent", name={'EN': 'Magnitude', 'DE': 'Magnitude'})
     additionResult=testDsiVectorMag1+testDsiVectorMag2
     assert additionResult['values'][5] == 1030.0
+
+def test_toUnitConversion():
+    testCountsPerSecond = dccQuantity((np.arange(20) + 1) * 5, np.ones(20) * 0.1, 'Counts per Second', r'\second\tothe{-1}', uncerType="relPercent", name={'EN': 'Counts per Second', 'DE': 'Zählungen pro Sekunde'})
+    testCountsPerSecond.convertToUnit(r'\hertz')
+    assert testCountsPerSecond['unit'] == dsiUnit(r'\hertz')
+    assert testCountsPerSecond['values'][3] == 20
+    assert testCountsPerSecond['uncer'][3] == 0.02
+    testCountsPerSecond.convertToUnit(r'\kilo\hertz')
+    assert testCountsPerSecond['unit'] == dsiUnit(r'\kilo\hertz')
+    assert testCountsPerSecond['values'][3] == 20/1000
+    assert testCountsPerSecond['uncer'][3] == 0.02/1000
+    testCountsPerSecond.convertToUnit(r'\becquerel')
+    assert testCountsPerSecond['unit'] == dsiUnit(r'\becquerel')
+    assert testCountsPerSecond['values'][3] == 20
+    assert testCountsPerSecond['uncer'][3] == 0.02
+    testCountsPerSecond.convertToUnit(r'\kilo\becquerel')
+    assert testCountsPerSecond['unit'] == dsiUnit(r'\kilo\becquerel')
+    assert testCountsPerSecond['values'][3] == 0.020
+    assert testCountsPerSecond['uncer'][3] == 0.00002
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dccquantities-1.4.4/tests/test_tollerance.py` & `dccquantities-1.4.5/tests/test_tollerance.py`

 * *Files identical despite different names*

