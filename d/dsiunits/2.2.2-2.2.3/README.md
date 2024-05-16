# Comparing `tmp/dsiunits-2.2.2.tar.gz` & `tmp/dsiunits-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsiunits-2.2.2.tar", last modified: Tue May  7 13:06:51 2024, max compression
+gzip compressed data, was "dsiunits-2.2.3.tar", last modified: Thu May 16 16:54:44 2024, max compression
```

## Comparing `dsiunits-2.2.2.tar` & `dsiunits-2.2.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 seeger01  (1000) seeger01  (1000)        0 2024-05-07 13:06:51.199603 dsiunits-2.2.2/
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)    26516 2024-04-25 08:43:02.000000 dsiunits-2.2.2/LICENSE
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)    33557 2024-05-07 13:06:51.199603 dsiunits-2.2.2/PKG-INFO
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)     2403 2024-04-25 09:18:30.000000 dsiunits-2.2.2/README.md
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)      764 2024-05-07 13:06:33.000000 dsiunits-2.2.2/pyproject.toml
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)      376 2024-05-07 13:06:51.199603 dsiunits-2.2.2/setup.cfg
-drwxr-xr-x   0 seeger01  (1000) seeger01  (1000)        0 2024-05-07 13:06:51.198603 dsiunits-2.2.2/src/
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)        0 2024-04-25 08:36:12.000000 dsiunits-2.2.2/src/__init__.py
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)    40343 2024-05-07 13:04:53.000000 dsiunits-2.2.2/src/dsiUnits.py
-drwxr-xr-x   0 seeger01  (1000) seeger01  (1000)        0 2024-05-07 13:06:51.199603 dsiunits-2.2.2/src/dsiunits.egg-info/
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)    33557 2024-05-07 13:06:51.000000 dsiunits-2.2.2/src/dsiunits.egg-info/PKG-INFO
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)      241 2024-05-07 13:06:51.000000 dsiunits-2.2.2/src/dsiunits.egg-info/SOURCES.txt
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)        1 2024-05-07 13:06:51.000000 dsiunits-2.2.2/src/dsiunits.egg-info/dependency_links.txt
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)       18 2024-05-07 13:06:51.000000 dsiunits-2.2.2/src/dsiunits.egg-info/top_level.txt
-drwxr-xr-x   0 seeger01  (1000) seeger01  (1000)        0 2024-05-07 13:06:51.198603 dsiunits-2.2.2/tests/
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)    18195 2024-05-07 13:04:53.000000 dsiunits-2.2.2/tests/test_dsiUnits.py
+drwxr-xr-x   0 seeger01  (1000) seeger01  (1000)        0 2024-05-16 16:54:44.914838 dsiunits-2.2.3/
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)    26516 2024-04-25 08:43:02.000000 dsiunits-2.2.3/LICENSE
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)    33313 2024-05-16 16:54:44.914838 dsiunits-2.2.3/PKG-INFO
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)     2033 2024-05-16 16:54:24.000000 dsiunits-2.2.3/README.md
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)      764 2024-05-16 16:54:24.000000 dsiunits-2.2.3/pyproject.toml
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)      447 2024-05-16 16:54:44.915838 dsiunits-2.2.3/setup.cfg
+drwxr-xr-x   0 seeger01  (1000) seeger01  (1000)        0 2024-05-16 16:54:44.914838 dsiunits-2.2.3/src/
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)        0 2024-04-25 08:36:12.000000 dsiunits-2.2.3/src/__init__.py
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)    43577 2024-05-16 16:54:24.000000 dsiunits-2.2.3/src/dsiUnits.py
+drwxr-xr-x   0 seeger01  (1000) seeger01  (1000)        0 2024-05-16 16:54:44.914838 dsiunits-2.2.3/src/dsiunits.egg-info/
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)    33313 2024-05-16 16:54:44.000000 dsiunits-2.2.3/src/dsiunits.egg-info/PKG-INFO
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)      276 2024-05-16 16:54:44.000000 dsiunits-2.2.3/src/dsiunits.egg-info/SOURCES.txt
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)        1 2024-05-16 16:54:44.000000 dsiunits-2.2.3/src/dsiunits.egg-info/dependency_links.txt
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)       43 2024-05-16 16:54:44.000000 dsiunits-2.2.3/src/dsiunits.egg-info/requires.txt
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)       18 2024-05-16 16:54:44.000000 dsiunits-2.2.3/src/dsiunits.egg-info/top_level.txt
+drwxr-xr-x   0 seeger01  (1000) seeger01  (1000)        0 2024-05-16 16:54:44.914838 dsiunits-2.2.3/tests/
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)    24345 2024-05-16 16:54:24.000000 dsiunits-2.2.3/tests/test_dsiUnits.py
```

### Comparing `dsiunits-2.2.2/LICENSE` & `dsiunits-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dsiunits-2.2.2/PKG-INFO` & `dsiunits-2.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsiunits
-Version: 2.2.2
+Version: 2.2.3
 Summary: This is a Python module for handling the SI units as objects in Python, parsing them from strings and converting them to Latex and Unicode, as well as performing math operations and calculating scale factors.
 Author-email: Benedikt Seeger <benedikt.seeger@ptb.de>, Vanessa Stehr <vanessa.stehr@ptb.de>
 License:                   GNU LESSER GENERAL PUBLIC LICENSE
                                Version 2.1, February 1999
         
          Copyright (C) 1991, 1999 Free Software Foundation, Inc.
          51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
@@ -510,58 +510,61 @@
         
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Provides-Extra: testing
+Requires-Dist: pytest>=7.4.1; extra == "testing"
+Requires-Dist: pytest-cov>=4.1.0; extra == "testing"
 
-[![pipeline status](https://gitlab1.ptb.de/digitaldynamicmeasurement/dsiUnits/badges/main/pipeline.svg)](https://gitlab1.ptb.de/digitaldynamicmeasurement/dsiUnits/-/commits/branch)
-[![coverage report](https://gitlab1.ptb.de/digitaldynamicmeasurement/dsiUnits/badges/amin/coverage.svg)](https://gitlab1.ptb.de/digitaldynamicmeasurement/dsiUnits/-/blob/branch/coverage.xml)
 # D-SI Parser
 
 This library converts D-SI unit strings to Latex.
-And is able to perform math operatins *, / and power with the D-SI units as well as checken weather teh can be converted into each other with scalar multiplication
+And is able to perform math operations *, / and power with the D-SI units as well as checken weather teh can be converted into each other with scalar multiplication
 
-## Instalaltion
+## Installation
 
 ```bash
 pip install dsiUnits
 ```
+
 ## Usage
-the Constructor `dsiUnit(str)` will parse the string and create a dsiUnit object.
+The Constructor `dsiUnit(str)` will parse the string and create a dsiUnit object.
 The dsiUnit object has the following methods:
 - `toLatex()`: returns the Latex representation of the unit
 - `toUTF8()`: returns the UTF8 representation of the unit
-- `isScalablyEqualTo(other)`: checks weather the unit is equal to another unit with scalar multiplication
-And following magic functions 
+- `isScalablyEqualTo(other)`: checks whether the unit is equal to another unit with scalar multiplication
+  
+And following magic functions: 
 - `__mul__(other)`: "*" multiplies the unit with another unit or a scalar
-- `__truediv__(other)`:"/" divides the unit by another unit or a scalar
+- `__truediv__(other)`: "/" divides the unit by another unit or a scalar
 - `__pow__(other)`: "**" raises the unit to the power of another unit or a scalar
-- `__eq__(other)`: "==" checks weather the unit is equal to another unit
+- `__eq__(other)`: "==" checks whether the unit is equal to another unit
 - `__str__`: "str()" returns the string representation of the unit
 - `__repr__`: returns the string representation of the unit
 
 - `toBaseUnitTree()`: returns the base unit tree of the unit
-- `reduceFraction()`: reduces the fraction of the unit by resolving all pers and the combinig same units by exponent addition 
+- `reduceFraction()`: reduces the fraction of the unit by resolving all `\per` and combining same units by exponent addition 
 - `sortTree()`: sorts the base unit tree of the unit
+- 
 ```python
 from dsiUnits import dsiUnit
 
 unit = dsiUnit('\metre\second\tothe{-1}')
 latexStr=unit.toLatex()
 print(latexStr)
 ```
+
 ```python
 from dsiUnits import dsiUnit
 
 mps = dsiUnit(r'\metre\second\tothe{-1}')
 kmh = dsiUnit(r'\kilo\metre\per\hour')
-scalfactor,baseUnit=mps.isScalablyEqualTo(kmh)
-print("The unit "+str(mps)+" is equal to "+str(kmh)+"with a factor of ",scalfactor," and base unit ",str(baseUnit))
-```
-```python
+scaleFactor, baseUnit = mps.isScalablyEqualTo(kmh)
+print("The unit "+str(mps)+" is equal to "+str(kmh)+" with a factor of "+scaleFactor+" and base unit "+str(baseUnit))
 ```
 
-For more usage Examples see the [Example Notebook](https://gitlab1.ptb.de/digitaldynamicmeasurement/dsiUnits/-/blob/main/doc/examples.ipynb).
-As well as the [pytest file](https://gitlab1.ptb.de/digitaldynamicmeasurement/dsiUnits/-/blob/main/src/dsiUnits.py).
+For more usage examples see the [Example Notebook](https://gitlab1.ptb.de/digitaldynamicmeasurement/dsiUnits/-/blob/main/doc/examples.ipynb),
+as well as the [pytest file](https://gitlab1.ptb.de/digitaldynamicmeasurement/dsiUnits/-/blob/main/src/dsiUnits.py).
```

### Comparing `dsiunits-2.2.2/pyproject.toml` & `dsiunits-2.2.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dsiunits"  # Ensure this is correctly specified
-version = "2.2.2"
+version = "2.2.3"
 description = "This is a Python module for handling the SI units as objects in Python, parsing them from strings and converting them to Latex and Unicode, as well as performing math operations and calculating scale factors."
 authors = [
     { name="Benedikt Seeger", email="benedikt.seeger@ptb.de" },
     { name="Vanessa Stehr", email="vanessa.stehr@ptb.de" }
 ]
 license = { file="LICENSE" }
 readme = "README.md"
```

### Comparing `dsiunits-2.2.2/src/dsiUnits.py` & `dsiunits-2.2.3/src/dsiUnits.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,24 +16,40 @@
 import re
 import warnings
 import difflib
 from typing import List
 from copy import deepcopy
 import math
 from fractions import Fraction
+from decimal import Decimal, InvalidOperation
 import numbers
 
+# config.py
+class dsiConfigConfig:
+    #Singelton Pattern this class can only have one instance all constructors will return this instance
+    _instance = None
+
+    def __new__(cls):
+        if cls._instance is None:
+            cls._instance = super(dsiConfigConfig, cls).__new__(cls)
+            # Initialize configuration options
+            cls._instance.createPerByDivision = True
+            cls._instance.maxDenominator = 10000
+        return cls._instance
+
+
+dsiConfigConfiginstance = dsiConfigConfig()
 
 def _dsiStrFromNodes(nodeList):
     """Converts a list of nodes to a D-SI string."""
     dsiStr = ""
-    for i, fraction in enumerate(nodeList):
+    for i, unitFraction in enumerate(nodeList):
         if i > 0:
             dsiStr += r"\per"
-        for node in fraction:
+        for node in unitFraction:
             dsiStr += str(node)
     return dsiStr
 
 
 class dsiParser:
     __dsiVersion = "2.2.0"
     __dsiSchemaUrl = "https://www.ptb.de/si/v2.2.0/SI_Format.xsd"
@@ -155,27 +171,22 @@
                     item = ''
             if item in _dsiUnitsLatex:
                 unit = item
                 try:
                     item = items.pop(0)
                 except IndexError:
                     item = ''
-            if re.match(r'tothe\{-?\d+\.?\d?\}', item):
-                exponent = item.split('{')[1].split('}')[0]
-                try:
-                    item = items.pop(0)
-                except IndexError:
-                    item = ''
-            elif re.match(r'tothe\{.*\}', item):
-                exponent = item.split('{')[1].split('}')[0]
+            if re.match(r'tothe\{[^{}]*\}', item): # used to be elif
+                exponentStr = item.split('{')[1].split('}')[0]
                 try:
-                    floatCast = float(exponent)
+                    exponent = Fraction(exponentStr).limit_denominator()
                 except ValueError:
                     warningMessages.append(_warn(f"The exponent «{exponent}» is not a number!", RuntimeWarning))
                     valid=False
+                    exponent = exponentStr
                 try:
                     item = items.pop(0)
                 except IndexError:
                     item = ''
             if (prefix, unit, exponent) == ('', '', ''):
                 unit = item
                 try:
@@ -195,15 +206,15 @@
                         _warn(fr"The identifier «{unit}» does not match any D-SI units!", RuntimeWarning))
                     valid=False
             elif unit == '':
                 itemStr = ""
                 if prefix != "":
                     itemStr = itemStr + "\\" + prefix
                 if exponent != "":
-                    itemStr = itemStr + r"\tothe{" + exponent + r"}"
+                    itemStr = itemStr + r"\tothe{" + str(exponent) + r"}"
                 warningMessages.append(
                     _warn(f"This D-SI unit seems to be missing the base unit! «{itemStr}»", RuntimeWarning))
                 valid=False
             nodes.append(_node(prefix, unit, exponent, valid=valid))
             if (len(items) == 0) and (item == ''): break
             (prefix, unit, exponent) = ('', '', '')
             valid=True
@@ -218,31 +229,32 @@
 
 dsiDefaultParser=dsiParser()
 
 class dsiUnit:
     """D-SI representation in tree form, also includes validity check and warnings about D-SI string.
        Tree format: list of lists:
            List format:
-           First layer: items of the fraction
+           First layer: items of the unit fraction
            Second layer: nodes containing prefix, unit, power
     """
 
     def __init__(self, dsiString: str, dsiTree=[], warningMessages=[], latexDefaultWrapper='$$', latexDefaultPrefix='',
                  latexDefaultSuffix=''):
         """
         Args:
             dsiString (str): the D-SI unit string to be parsed
-            optional dsiTree (list): List of lists of nodes as tuples containing (prefix: str,unit: str,exponent: float=1.0,scaleFactor: float = 1.0)
+            optional dsiTree (list): List of lists of nodes as tuples containing (prefix: str,unit: str,exponent: Fraction=Fraction(1),scaleFactor: float = 1.0)
             like [('metre', 1.0, 1.0), ('second', -1.0, 1.0)] to generate ms^-1 when usign this construction method no str can be given
         """
         # we have got a tree so we dont need to parse the string
         if dsiString == "" and dsiTree != []:
             dsiString=_dsiStrFromNodes(dsiTree)
         if dsiString != "" and dsiTree == []:
             try:
+                # TODO Why do we parse twice?
                 dsiTree = dsiDefaultParser.parse(dsiString).tree
                 warningMessages = dsiDefaultParser.parse(dsiString).warnings
             except Exception as e:
                 warnings.warn(e)
         if dsiString == "" and dsiTree == []:
             warnings.warn("Given D-SI string is empty!")
             dsiTree = dsiDefaultParser.parse(dsiString).tree
@@ -312,21 +324,20 @@
         def exponent_to_utf8(exp):
             """Converts numerical exponents to UTF-8 subscript."""
             # Mapping for common exponents to UTF-8
             superscripts = {"1": "¹", "2": "²", "3": "³", "4": "⁴", "5": "⁵",
                             "6": "⁶", "7": "⁷", "8": "⁸", "9": "⁹", "0": "⁰",
                             "-": "⁻",".": "˙"}
             # Convert fractional exponents to a more readable format if needed
-            exp_str = str(exp).rstrip('.0')  # Remove trailing '.0' for whole numbers
-            return ''.join(superscripts.get(char, char) for char in exp_str)
+            return ''.join(superscripts.get(char, char) for char in str(exp))
 
         utf8Array = []
-        for fraction in self.tree:
+        for unitFraction in self.tree:
             fractionUtf8Array = []
-            for node in fraction:
+            for node in unitFraction:
                 # Fetch UTF-8 unit representation
                 unitStr = _dsiUnitsUTF8.get(node.unit,'⚠'+node.unit+'⚠')#second arg is returend on itemError
 
                 # Handle prefix (if any) and unit
                 prefixStr = _dsiPrefixesUTF8.get(node.prefix, '⚠'+node.prefix+'⚠') if node.prefix else ""
                 utf8Str = f"{prefixStr}{unitStr}"  # Direct concatenation for compactness
 
@@ -345,40 +356,37 @@
 
 
     def toBaseUnitTree(self,complete=False):
         """
         Converts the entire D-SI tree to its base unit representation.
         """
         baseUnitTree = []
-        for fraction in self.tree:
+        for unitFraction in self.tree:
             baseFraction = []
-            for node in fraction:
+            for node in unitFraction:
                 baseFraction.extend(node.toBaseUnits())
             baseUnitTree.append(baseFraction)
         unconsolidatedTree = dsiUnit(self.dsiString, baseUnitTree, self.warnings, self._latexDefaultWrapper, self._latexDefaultPrefix, self._latexDefaultSuffix)
         reduced=unconsolidatedTree.reduceFraction()
         # if kgms True we do a second round but resolve volt ampere mole this round
         if complete:
             baseUnitTree = []
-            for fraction in self.tree:
+            for unitFraction in self.tree:
                 baseFraction = []
-                for node in fraction:
+                for node in unitFraction:
                     baseFraction.extend(node.toBaseUnits(complete=complete))
                 baseUnitTree.append(baseFraction)
             unconsolidatedTree = dsiUnit(self.dsiString, baseUnitTree, self.warnings, self._latexDefaultWrapper,
                                          self._latexDefaultPrefix, self._latexDefaultSuffix)
             reduced = unconsolidatedTree.reduceFraction()
         return reduced
 
     def reduceFraction(self):
         """
         Creates a new _dsiTree instance with reduced fractions.
-        - For a single node: Simply copies it to the consolidated list.
-        - For two nodes: Copies the first node and adds the second node with its exponent multiplied by -1.
-        - For more than two nodes: Raises a RuntimeError.
         - Consolidates nodes with the same base unit by multiplying scales and summing exponents.
         - Sorts the nodes alphabetically by unit.
         - The first node carries the overall scale factor.
         """
         if len(self.tree) > 2:
             raise RuntimeError("D-SI tree with more than two fractions cannot be reduced.")
 
@@ -415,109 +423,144 @@
             i += 1
 
         # Calculate overall scale factor and apply it to the first node
         overall_scale_factor = 1.0
         for node in consolidated_nodes:
             overall_scale_factor *= node.scaleFactor
             node.scaleFactor = 1.0  # Reset scale factor for individual nodes
-
-
-
         # Sort nodes alphabetically by unit
         consolidated_nodes.sort(key=lambda x: x.unit)
         # Apply overall scale factor to the first node, if it exists
         if consolidated_nodes:
             consolidated_nodes[0].scaleFactor = overall_scale_factor
-        nodesWithOutpowerZero=[]
+        nodesWOPowerZero=[]
         for node in consolidated_nodes:
             if node.exponent != 0:
-                nodesWithOutpowerZero.append(node)
-        if len(nodesWithOutpowerZero) == 0: # ok all noes have ben power of zero so we deleted them so we end up with one as unit and 1.0 as exponent
-            nodesWithOutpowerZero.append(_node("", "one", 1.0,scaleFactor=overall_scale_factor))
-        consolidated_nodes=nodesWithOutpowerZero
+                nodesWOPowerZero.append(node)
+        if len(nodesWOPowerZero) == 0: # ok all nodes have ben power of zero so we deleted them so we end up with one as unit and 1.0 as exponent
+            nodesWOPowerZero.append(_node("", "one", 1.0,scaleFactor=overall_scale_factor))
+        consolidated_nodes=nodesWOPowerZero
+        # Check for ones and delete them if they are not the only node ad set there exponent to 1.0 since 1^x = 1
+        if len(consolidated_nodes) > 1:
+            consolidated_nodes = [node for node in consolidated_nodes if node.unit != "one"]
+        else:
+            if consolidated_nodes[0].unit == "one":
+                consolidated_nodes[0].exponent=1.0
         # Create and return a new instance of _dsiTree with consolidated nodes
         return dsiUnit(self.dsiString, [consolidated_nodes], self.warnings, self._latexDefaultWrapper,
                        self._latexDefaultPrefix, self._latexDefaultSuffix)
+
+    def _removePer(self):
+        if len(self.tree)==2:
+            for i,node in enumerate(self.tree[1]):
+                #invert exponent node.
+                node.exponent=node.exponent*-1
+                self.tree[0].append(node)
+                self.tree[1].pop(i)
+            self.tree.pop(1)
+
+    def negExponentsToPer(self):
+        """Converts negative exponents to the denominator of the fraction."""
+        for node in self.tree[0]: # numerator
+            if node.exponent < 0:
+                node.exponent = -node.exponent
+                try:
+                    self.tree[1].append(_node("", node.unit, node.exponent))
+                except IndexError:# if we have only the numerator list we need to add the denominator list
+                    self.tree.append([_node("", node.unit, node.exponent)])
+                self.tree[0].remove(node)
+        if len(self.tree) ==2: # we have a numerator and a denominator so we must treat the denominator as well
+            for node in self.tree[1]: # numerator
+                if node.exponent < 0:
+                    node.exponent = -node.exponent
+                    self.tree[0].append(_node("", node.unit, node.exponent))
+                    self.tree[1].remove(node)
+        if len(self.tree[0]) == 0:
+            self.tree[0].append(_node("", "one", 1.0))
+        return self
+
+
     def sortTree(self):
         """Sorts each fraction's nodes alphabetically by their units."""
-        for fraction in self.tree:
-            fraction.sort(key=lambda node: node.unit)
+        for unitFraction in self.tree:
+            unitFraction.sort(key=lambda node: node.unit)
     def __eq__(self, other):
         """Checks if two D-SI trees are identical after sorting their nodes alphabetically."""
         if not isinstance(other, dsiUnit):
             return False
 
         # Sort both trees before comparison
         selfCopy = deepcopy(self)
         otherCopy = deepcopy(other)
         selfCopy.sortTree()
         otherCopy.sortTree()
         if selfCopy.tree == otherCopy.tree:
             return True
         else:
-            scalfactor,baseunit=selfCopy.isScalablyEqualTo(otherCopy)
-            if scalfactor == 1.0:
+            selfCopy._removePer()
+            otherCopy._removePer()
+            if selfCopy.tree==otherCopy.tree:
                 return True
             else:
                 return False
 
     def isScalablyEqualTo(self, other,complete=False):
         """Checks if two D-SI trees are scalably equal.
 
         Returns:
             (bool, float): Tuple of a boolean indicating if trees are scalably equal, and the scale factor.
         """
         if not isinstance(other, dsiUnit):
             return (math.nan, None)
 
 
-        sortedself=deepcopy(self)
-        sortedself.sortTree()
-        sortedother=deepcopy(other)
-        sortedother.sortTree()
+        sortedSelf=deepcopy(self)
+        sortedSelf.sortTree()
+        sortedOther=deepcopy(other)
+        sortedOther.sortTree()
         # okay now check if is identical
-        if sortedself.tree == sortedother.tree:
+        if sortedSelf.tree == sortedOther.tree:
             return (1.0,self)
-        scalefactor=1
-        for fracIdx,fraction in enumerate(sortedself.tree):
+        scaleFactor=1
+        for fracIdx,unitFraction in enumerate(sortedSelf.tree):
             try:
-                if len(fraction) != len(sortedother.tree[fracIdx]):
-                    scalefactor=math.nan
+                if len(unitFraction) != len(sortedOther.tree[fracIdx]):
+                    scaleFactor=math.nan
                     break
-                for nodeIDX,node in enumerate(fraction):
-                    scalefactor *= node.isScaled(sortedother.tree[fracIdx][nodeIDX])
+                for nodeIDX,node in enumerate(unitFraction):
+                    scaleFactor *= node.isScaled(sortedOther.tree[fracIdx][nodeIDX])
             except IndexError:
                 # if we get here we have a fraction in one tree that is not in the other in this case we resolve to base units and compare
-                scalefactor=math.nan
+                scaleFactor=math.nan
                 break
-        if not math.isnan(scalefactor):
-            return (scalefactor,self)
+        if not math.isnan(scaleFactor):
+            return (scaleFactor,self)
         # Convert both trees to their base unit representations
         selfBaseUnitTree = self.toBaseUnitTree(complete=complete)
         otherBaseUnitTree = other.toBaseUnitTree(complete=complete)
 
         # Sort both trees
         selfBaseUnitTree.sortTree()
         otherBaseUnitTree.sortTree()
-        # Check ifunits match
+        # Check if units match
         if len(selfBaseUnitTree.tree) != len(otherBaseUnitTree.tree):
             return (math.nan, None)
         # Calculate scale factor
         scaleFactor = 1.0
         if len(selfBaseUnitTree.tree) != 1 or len(otherBaseUnitTree.tree) != 1:
-            raise RuntimeError("D-SI tree with more than one fraction cannot be compared. And should not existhere since we consolidatet earlyer")
+            raise RuntimeError("D-SI tree with more than one fraction cannot be compared. And should not exist here since we consolidated earlier")
         for selfNode, otherNode in zip(selfBaseUnitTree.tree[0], otherBaseUnitTree.tree[0]):
             if selfNode.unit != otherNode.unit:
                 return (math.nan, None)
-            if float(selfNode.exponent) != float(otherNode.exponent):
+            if selfNode.exponent != otherNode.exponent:
                 return (math.nan, None)
             scaleFactor *= otherNode.scaleFactor / selfNode.scaleFactor
-        # reseting scalfactor to 1.0
-        for fraction in selfBaseUnitTree.tree:
-            for node in fraction:
+        # resetting scaleFactor to 1.0
+        for unitFraction in selfBaseUnitTree.tree:
+            for node in unitFraction:
                 node.scaleFactor = 1.0
         return (scaleFactor,selfBaseUnitTree)
 
     def __str__(self):
         result = ""
         for node in self.tree[0]:
             result += str(node)
@@ -537,54 +580,65 @@
         return f"{contentStr}"
 
 
     def __pow__(self, other):
         if not isinstance(other, numbers.Real):
             raise TypeError("Exponent must be a real number")
         resultNodeLIst = deepcopy(self.tree)
-        for fraction in resultNodeLIst:
-            for node in fraction:
+        for unitFraction in resultNodeLIst:
+            for node in unitFraction:
                 node.exponent *= other
         resultTree =dsiUnit("", resultNodeLIst, self.warnings, self._latexDefaultWrapper, self._latexDefaultPrefix, self._latexDefaultSuffix)
         resultTree = resultTree.reduceFraction()
+        if len(self.tree)==2: # check if we had a per representation
+            resultTree.negExponentsToPer()
         return resultTree
 
     def __mul__(self, other):
+        if len(self.tree) + len(other.tree) > 2:
+            convertToPer=True
+        else:
+            convertToPer=False
         resultNodeLIst=deepcopy(self.tree)
-        for i,fraction in enumerate(other.tree):
+        for i,unitFraction in enumerate(other.tree):
             if i>1:
                 raise RuntimeError("D-SI tree with more than one fraction cannot be multiplied")
             try:
-                resultNodeLIst[i].extend(deepcopy(fraction))
+                resultNodeLIst[i].extend(deepcopy(unitFraction))
             except IndexError:
-                resultNodeLIst.append(deepcopy(fraction))# there was no fraction so we add it
+                resultNodeLIst.append(deepcopy(unitFraction))# there was no fraction so we add it
 
         resultTree =dsiUnit("", resultNodeLIst, self.warnings, self._latexDefaultWrapper, self._latexDefaultPrefix, self._latexDefaultSuffix)
         resultTree = resultTree.reduceFraction()
+        if convertToPer:
+            resultTree = resultTree.negExponentsToPer()
         return resultTree
 
     def __truediv__(self, other):
-        return self * other**-1
+        if dsiConfigConfiginstance.createPerByDivision:
+            return (self * (other**-1)).negExponentsToPer()
+        else:
+            return self * (other ** -1)
 
 
 class _node:
     """one node of the D-SI tree, containing prefix, unit, power
     """
-    def __init__(self, prefix: str,unit: str,exponent: float=1.0, valid:bool=True,scaleFactor: float = 1.0  ):# Adding scale factor with default value 1.0
+    def __init__(self, prefix: str,unit: str,exponent: Fraction=Fraction(1), valid:bool=True,scaleFactor: float = 1.0  ):# Adding scale factor with default value 1.0
         self.prefix=prefix
         self.unit=unit
         self.valid=valid
-        if isinstance(exponent,float) or isinstance(exponent,int):
-            self.exponent=float(exponent)
+        if isinstance(exponent,Fraction) or isinstance(exponent,int):
+            self.exponent=Fraction(exponent)
         if isinstance(exponent,str):
             if exponent== '':
-                exponent= 1.0
+                exponent= Fraction(1)
             else:
                 try:
-                    exponent=float(exponent)
+                    exponent = Fraction(exponent).limit_denominator(dsiConfigConfiginstance.maxDenominator)
                 except ValueError:
                     exponent=exponent
                     warnings.warn(f"Exponent «{exponent}» is not a number!", RuntimeWarning)
         self.exponent=exponent
         self.scaleFactor=scaleFactor  # Adding scale factor with default value 1.0
 
     def toLatex(self):
@@ -599,37 +653,30 @@
         try:
             latexString += _dsiUnitsLatex[self.unit]
         except KeyError:
             latexString += r'{\color{red}\mathrm{'+self.unit+r'}}'
             if self.valid==True:
                 raise RuntimeError("Found invalid unit in valid node, this should not happen! Report this incident at: https://gitlab1.ptb.de/digitaldynamicmeasurement/dsiUnits/-/issues/new")
         if isinstance(self.exponent,str):
-            #exponet is str this souldnt happen!
+            # exponent is str this shouldn't happen!
             latexString += r'^{{\color{red}\mathrm{'+self.exponent+r'}}}'
             if self.valid==True:
                 raise RuntimeError("Found invalid unit in valid node, this should not happen! Report this incident at: https://gitlab1.ptb.de/digitaldynamicmeasurement/dsiUnits/-/issues/new")
-        elif self.exponent != 1.0:
-            if not self.exponent.is_integer():
-                if self.exponent == 0.5:
-                    latexString = r'\sqrt{' + latexString + r'}'
-                else:
-                    exponent_fraction = Fraction(self.exponent).limit_denominator()
-                    if exponent_fraction.denominator == 1:
-                        # If the denominator is 1, it's effectively an integer
-                        latexString += r'\sqrt['+str(int(exponent_fraction.numerator))+']{' + latexString + r'}'
-                    else:
-                        # For non-integer exponents, display as fractions
-                        if int(exponent_fraction.numerator) == 1:
-                            latexString += r'\sqrt[' + str(int(exponent_fraction.denominator)) + ']{' + latexString + r'}'
-                        else:
-                            latexString += r'\sqrt[' + str(
-                                int(exponent_fraction.denominator)) + ']{' + latexString + '^{' + str(int(exponent_fraction.numerator)) + '}' + r'}'
+        elif self.exponent != 1:
+            if not self.exponent.denominator == 1: # exponent is not an integer
+                if self.exponent.denominator == 2: # square root
+                    latexString = r'\sqrt{' + latexString 
+                else: # higher roots need an extra argument
+                    latexString = r'\sqrt[' + str(self.exponent.denominator) + ']{' + latexString
+                    if self.exponent.numerator != 1: # keep anything in the numerator of the exponent in the exponent
+                        latexString += '^{' + str(self.exponent.numerator) + '}'
+                latexString += r'}'
+                    
             else:
-                #TODO better formating
-                latexString += r'^{' + str(int(self.exponent)) + r'}'
+                latexString += r'^{' + str(self.exponent) + r'}'
 
         
         if self.unit == "":
             latexString = r'{\color{red}'+latexString+r'}'
             if self.valid==True:
                 raise RuntimeError("Found invalid unit in valid node, this should not happen! Report this incident at: https://gitlab1.ptb.de/digitaldynamicmeasurement/dsiUnits/-/issues/new")
 
@@ -644,15 +691,15 @@
         Args:
             kgs (bool): If true, also resolves volt to kg, s, and m units.
 
         Returns:
             List['_node']: List of nodes representing the base units or kg, s, m equivalents.
         """
         # Adjust the scale factor for the prefix
-        prefixScale = _dsiPrefixsScales.get(self.prefix, 1)  # Default to 1 if no prefix
+        prefixScale = _dsiPrefixesScales.get(self.prefix, 1)  # Default to 1 if no prefix
         adjustedScaleFactor = self.scaleFactor * prefixScale
 
         # Convert to base units if it's a derived unit
         if self.unit in _derivedToBaseUnits:
             baseUnitsInfo = _derivedToBaseUnits[self.unit]
             baseUnits = []
             for i, (baseUnit, exponent, scaleFactor) in enumerate(baseUnitsInfo):
@@ -679,22 +726,22 @@
 
     def __str__(self):
         result=''
 
         if self.prefix !='':
             result+='\\'+self.prefix
         result = result + '\\' + self.unit
-        if self.exponent != 1.0:
-            result =result + r'\tothe{' + '{:g}'.format(self.exponent) + '}'
+        if self.exponent != 1:
+            result = result + r'\tothe{' + '{:g}'.format(float(self.exponent)) + '}'
         return result
 
     def isScaled(self,other):
         """Checks if two nodes are scaled equal."""
         if self.unit == other.unit and self.exponent == other.exponent:
-            return _dsiPrefixsScales[other.prefix]/_dsiPrefixsScales[self.prefix]
+            return _dsiPrefixesScales[other.prefix]/_dsiPrefixesScales[self.prefix]
         else:
             return math.nan
 
 def _warn(message: str, warningClass):
     """Output warning on command line and return warning message
 
     Args:
@@ -703,26 +750,26 @@
 
     Returns:
         str: message
     """
     warnings.warn(message, warningClass)
     return message
 
-def _getClosestStr(unkownStr):
+def _getClosestStr(unknownStr):
     """returns the closest string and type of the given string
 
     Args:
         unknownStr (str): string to be compared
 
     Returns:
         str: closest string
         str: type of closest string
     """
     possibleDsiKeys = _dsiPrefixesLatex.keys() | _dsiUnitsLatex.keys() | _dsiKeyWords.keys()
-    closestStr = difflib.get_close_matches(unkownStr, possibleDsiKeys, n=3,cutoff=0.66)
+    closestStr = difflib.get_close_matches(unknownStr, possibleDsiKeys, n=3,cutoff=0.66)
     return closestStr
 # mapping D-SI prefixes to latex
 _dsiPrefixesLatex = {
     'deca': r'\mathrm{da}',
     'hecto': r'\mathrm{h}',
     'kilo': r'\mathrm{k}',
     'mega': r'\mathrm{M}',
@@ -737,19 +784,27 @@
     'milli': r'\mathrm{m}',
     'micro': r'\micro', 
     'nano': r'\mathrm{n}',
     'pico': r'\mathrm{p}',
     'femto': r'\mathrm{f}',
     'atto': r'\mathrm{a}',
     'zepto': r'\mathrm{z}',
-    'yocto': r'\mathrm{y}'
+    'yocto': r'\mathrm{y}',
+    'kibi': r'\mathrm{Ki}',
+    'mebi': r'\mathrm{Mi}',
+    'gibi': r'\mathrm{Gi}',
+    'tebi': r'\mathrm{Ti}',
+    'pebi': r'\mathrm{Pi}',
+    'exbi': r'\mathrm{Ei}',
+    'zebi': r'\mathrm{Zi}',
+    'yobi': r'\mathrm{Yi}'
 }
 #TODO maybe directlusing the exponents is better
 # mapping D-SI prefixes to scale factors
-_dsiPrefixsScales = {
+_dsiPrefixesScales = {
     'yotta': 1e24,
     'zetta': 1e21,
     'exa': 1e18,
     'peta': 1e15,
     'tera': 1e12,
     'giga': 1e9,
     'mega': 1e6,
@@ -762,15 +817,23 @@
     'milli': 1e-3,
     'micro': 1e-6,
     'nano': 1e-9,
     'pico': 1e-12,
     'femto': 1e-15,
     'atto': 1e-18,
     'zepto': 1e-21,
-    'yocto': 1e-24
+    'yocto': 1e-24,
+    'kibi': 1024,                       #2^10
+    'mebi': 1048576,                    #2^20
+    'gibi': 1073741824,                 #2^30
+    'tebi': 1099511627776,              #2^40
+    'pebi': 1125899906842624,           #2^50
+    'exbi': 1152921504606846976,        #2^60 larger than 2^53 so quantization error is possible
+    'zebi': 1180591620717411303424,     #2^70 larger than 2^53 so quantization error is possible
+    'yobi': 1208925819614629174706176   #2^80 larger than 2^53 so quantization error is possible
 }
 # UTF-8 equivalents for SI prefixes
 _dsiPrefixesUTF8 = {
     'deca': 'da',
     'hecto': 'h',
     'kilo': 'k',
     'mega': 'M',
@@ -786,15 +849,23 @@
     # Unicode character for micro: 'µ' (U+00B5)
     'micro': 'µ',
     'nano': 'n',
     'pico': 'p',
     'femto': 'f',
     'atto': 'a',
     'zepto': 'z',
-    'yocto': 'y'
+    'yocto': 'y',
+    'kibi': 'Ki',
+    'mebi': 'Mi',
+    'gibi': 'Gi',
+    'tebi': 'Ti',
+    'pebi': 'Pi',
+    'exbi': 'Ei',
+    'zebi': 'Zi',
+    'yobi': 'Yi'
 }
 # mapping D-SI units to latex
 _dsiUnitsLatex = {
     'metre': r'\mathrm{m}',
     'kilogram': r'\mathrm{kg}',
     'second': r'\mathrm{s}',
     'ampere': r'\mathrm{A}',
@@ -836,15 +907,17 @@
     'tonne': r'\mathrm{t}',
     'electronvolt': r'\mathrm{eV}',
     'dalton': r'\mathrm{Da}',
     'astronomicalunit': r'\mathrm{au}',
     'neper': r'\mathrm{Np}',
     'bel': r'\mathrm{B}',
     'decibel': r'\mathrm{dB}',
-    'percent':r'\%'
+    'percent':r'\%',
+    'byte': r'\byte',
+    'bit': r'\bit',
 }
 # Comprehensive mapping from ASCII/UTF-8 representations to D-SI LaTeX strings
 ascii_to_dsi_unit_map = {
     'kg': 'kilogram',
     'm': 'metre',
     's': 'second',
     'A': 'ampere',
@@ -870,15 +943,18 @@
     '°C': 'degreecelsius',
     'lm': 'lumen',
     'lx': 'lux',
     'Bq': 'becquerel',
     'Gy': 'gray',
     'Sv': 'sievert',
     'kat': 'katal',
-    '%': 'percent'
+    '%': 'percent',
+    'ppm' : 'ppm',
+    'B': 'byte',
+    'bit': 'bit',
     # Add more units as needed
 }
 
 _dsiUnitsUTF8 = {
     'metre': 'm',
     'kilogram': 'kg',
     'second': 's',
@@ -921,27 +997,30 @@
     'tonne': 't',
     'electronvolt': 'eV',
     'dalton': 'Da',
     'astronomicalunit': 'au',
     'neper': 'Np',
     'bel': 'B',
     'decibel': 'dB',
-    'percent': '%'
+    'percent': '%',
+    'ppm' : 'ppm',
+    'byte': 'B',
+    'bit': 'bit',
 }
 
 _derivedToBaseUnits = {
     # Time units
     'day': [('second', 1, 86400)],         # 1 day = 86400 seconds
     'hour': [('second', 1, 3600)],         # 1 hour = 3600 seconds
     'minute': [('second', 1, 60)],         # 1 minute = 60 seconds
 
     # Angle units
-    'degree': [('radian', 1, 0.01745329252)], # 1 degree = π/180 radians
-    'arcminute': [('radian', 1, 0.0002908882086657216)], # 1 arcminute = π/10800 radians
-    'arcsecond': [('radian', 1, 0.00000484813681109536)], # 1 arcsecond = π/648000 radians
+    'degree': [('radian', 1, math.pi/180)], # 1 degree = π/180 radians
+    'arcminute': [('radian', 1, math.pi/10800)], # 1 arcminute = π/10800 radians
+    'arcsecond': [('radian', 1, math.pi/648000)], # 1 arcsecond = π/648000 radians
 
     # Mass units
     'gram': [('kilogram', 1, 0.001)],  # 1 gram = 0.001 kilograms
 
     # Derived units
     'hertz': [('second', -1,1)],  # 1 Hz = 1/s
     'newton': [('kilogram', 1, 1), ('metre', 1, 1), ('second',-2, 1)],  # 1 N = 1 kg·m/s²
@@ -953,35 +1032,38 @@
     'farad': [('kilogram',-1, 1), ('metre',-2, 1), ('second', 4, 1), ('ampere',2, 1)],# 1 F = 1 kg⁻¹·m⁻²·s⁴·A²
     'ohm': [('kilogram', 1, 1), ('metre',2, 1), ('second',-3, 1), ('ampere',-2, 1)],  # 1 Ω = 1 kg·m²/s³·A⁻²
     'siemens': [('kilogram',-1, 1), ('metre',-2, 1), ('second',3, 1), ('ampere',2, 1)],# 1 S = 1 kg⁻¹·m⁻²·s³·A²
     'weber': [('kilogram', 1, 1), ('metre',2, 1), ('second',-2, 1), ('ampere',-1, 1)],  # 1 Wb = 1 kg·m²/s²·A
     'tesla': [('kilogram', 1, 1), ('second',-2, 1), ('ampere',-1, 1)],  # 1 T = 1 kg/s²·A
     'henry': [('kilogram', 1, 1), ('metre',2, 1), ('second',-2, 1), ('ampere',-2, 1)],  # 1 H = 1 kg·m²/s²·A²
     #'degreecelsius': [('kelvin', 1, 1)], # Degree Celsius is a scale, not a unit; the unit is Kelvin
-    'lumen': [('candela', 1, 1), ('steradian', 1, 1)], # 1 lm = 1 cd·sr
-    'lux': [('candela', 1, 1), ('steradian', 1, 1), ('metre',-2, 1)], # 1 lx = 1 cd·sr/m²
+    'lumen': [('candela', 1, 1), ('steradian', 1, 1)], # 1 lm = 1 cd·sr #TODO full conversion to base units
+    'lux': [('candela', 1, 1), ('steradian', 1, 1), ('metre',-2, 1)], # 1 lx = 1 cd·sr/m² #TODO full conversion to base units
     'becquerel': [('second',-1, 1)], # 1 Bq = 1/s
     'sievert': [('metre',2, 1), ('second',-2, 1)], # 1 Sv = 1 m²/s²
     'gray': [('metre',2, 1), ('second',-2, 1)], # 1 Gy = 1 m²/s²
     'katal': [('mole', 1, 1), ('second',-1, 1)], # 1 kat = 1 mol/s
     # Other units
     'hectare': [('metre',2, 10000)],  # 1 ha = 10000 m²
     'litre': [('metre',3, 0.001)],  # 1 L = 0.001 m³
     'tonne': [('kilogram', 1, 1000)],  # 1 t = 1000 kg
     'electronvolt': [('joule', 1, 1.602176634e-19)],  # 1 eV = 1.602176634 × 10⁻¹⁹ J
     'dalton': [('kilogram', 1, 1.66053906660e-27)],  # 1 Da = 1.66053906660 × 10⁻²⁷ kg
     'astronomicalunit': [('metre', 1, 149597870700)],  # 1 AU = 149597870700 m
     'neper': [('one', 1,1)],  # Neper is a logarithmic unit for ratios of measurements, not directly convertible
     'bel': [('one', 1,1)],  # Bel is a logarithmic unit for ratios of power, not directly convertible
     'decibel': [('one', 1,1)],  # Decibel is a logarithmic unit for ratios of power, not directly convertible
-
+    'byte':[('bit',1,8)], ## TODO overthink this
 # Note: For logarithmic units like neper, bel, and decibel, conversion to base units is not straightforward due to their nature.
 }
 _additionalConversions = {
     # Conversions for ampere, volt, and mole into kg, s, m equivalents
     'volt': [('metre', 2, 1), ('kilogram', 1, 1), ('second', -3, 1), ('ampere', -1, 1)],  # V = kg·m²/s³·A⁻¹
-    'percent':[('one',1,0.01)]
+    'percent':[('one',1,0.01)],
+    'ppm':[('one',1,1e-6)],
+    'byte':[('one',1,8)],
+    'bit':[('one',1,1)],
     # Note: These are placeholders and need to be adjusted to reflect accurate conversions.
 }
 _dsiKeyWords = {
     'tothe': r'\tothe',
     'per': r'\per'}
```

### Comparing `dsiunits-2.2.2/src/dsiunits.egg-info/PKG-INFO` & `dsiunits-2.2.3/src/dsiunits.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsiunits
-Version: 2.2.2
+Version: 2.2.3
 Summary: This is a Python module for handling the SI units as objects in Python, parsing them from strings and converting them to Latex and Unicode, as well as performing math operations and calculating scale factors.
 Author-email: Benedikt Seeger <benedikt.seeger@ptb.de>, Vanessa Stehr <vanessa.stehr@ptb.de>
 License:                   GNU LESSER GENERAL PUBLIC LICENSE
                                Version 2.1, February 1999
         
          Copyright (C) 1991, 1999 Free Software Foundation, Inc.
          51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
@@ -510,58 +510,61 @@
         
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Provides-Extra: testing
+Requires-Dist: pytest>=7.4.1; extra == "testing"
+Requires-Dist: pytest-cov>=4.1.0; extra == "testing"
 
-[![pipeline status](https://gitlab1.ptb.de/digitaldynamicmeasurement/dsiUnits/badges/main/pipeline.svg)](https://gitlab1.ptb.de/digitaldynamicmeasurement/dsiUnits/-/commits/branch)
-[![coverage report](https://gitlab1.ptb.de/digitaldynamicmeasurement/dsiUnits/badges/amin/coverage.svg)](https://gitlab1.ptb.de/digitaldynamicmeasurement/dsiUnits/-/blob/branch/coverage.xml)
 # D-SI Parser
 
 This library converts D-SI unit strings to Latex.
-And is able to perform math operatins *, / and power with the D-SI units as well as checken weather teh can be converted into each other with scalar multiplication
+And is able to perform math operations *, / and power with the D-SI units as well as checken weather teh can be converted into each other with scalar multiplication
 
-## Instalaltion
+## Installation
 
 ```bash
 pip install dsiUnits
 ```
+
 ## Usage
-the Constructor `dsiUnit(str)` will parse the string and create a dsiUnit object.
+The Constructor `dsiUnit(str)` will parse the string and create a dsiUnit object.
 The dsiUnit object has the following methods:
 - `toLatex()`: returns the Latex representation of the unit
 - `toUTF8()`: returns the UTF8 representation of the unit
-- `isScalablyEqualTo(other)`: checks weather the unit is equal to another unit with scalar multiplication
-And following magic functions 
+- `isScalablyEqualTo(other)`: checks whether the unit is equal to another unit with scalar multiplication
+  
+And following magic functions: 
 - `__mul__(other)`: "*" multiplies the unit with another unit or a scalar
-- `__truediv__(other)`:"/" divides the unit by another unit or a scalar
+- `__truediv__(other)`: "/" divides the unit by another unit or a scalar
 - `__pow__(other)`: "**" raises the unit to the power of another unit or a scalar
-- `__eq__(other)`: "==" checks weather the unit is equal to another unit
+- `__eq__(other)`: "==" checks whether the unit is equal to another unit
 - `__str__`: "str()" returns the string representation of the unit
 - `__repr__`: returns the string representation of the unit
 
 - `toBaseUnitTree()`: returns the base unit tree of the unit
-- `reduceFraction()`: reduces the fraction of the unit by resolving all pers and the combinig same units by exponent addition 
+- `reduceFraction()`: reduces the fraction of the unit by resolving all `\per` and combining same units by exponent addition 
 - `sortTree()`: sorts the base unit tree of the unit
+- 
 ```python
 from dsiUnits import dsiUnit
 
 unit = dsiUnit('\metre\second\tothe{-1}')
 latexStr=unit.toLatex()
 print(latexStr)
 ```
+
 ```python
 from dsiUnits import dsiUnit
 
 mps = dsiUnit(r'\metre\second\tothe{-1}')
 kmh = dsiUnit(r'\kilo\metre\per\hour')
-scalfactor,baseUnit=mps.isScalablyEqualTo(kmh)
-print("The unit "+str(mps)+" is equal to "+str(kmh)+"with a factor of ",scalfactor," and base unit ",str(baseUnit))
-```
-```python
+scaleFactor, baseUnit = mps.isScalablyEqualTo(kmh)
+print("The unit "+str(mps)+" is equal to "+str(kmh)+" with a factor of "+scaleFactor+" and base unit "+str(baseUnit))
 ```
 
-For more usage Examples see the [Example Notebook](https://gitlab1.ptb.de/digitaldynamicmeasurement/dsiUnits/-/blob/main/doc/examples.ipynb).
-As well as the [pytest file](https://gitlab1.ptb.de/digitaldynamicmeasurement/dsiUnits/-/blob/main/src/dsiUnits.py).
+For more usage examples see the [Example Notebook](https://gitlab1.ptb.de/digitaldynamicmeasurement/dsiUnits/-/blob/main/doc/examples.ipynb),
+as well as the [pytest file](https://gitlab1.ptb.de/digitaldynamicmeasurement/dsiUnits/-/blob/main/src/dsiUnits.py).
```

### Comparing `dsiunits-2.2.2/tests/test_dsiUnits.py` & `dsiunits-2.2.3/tests/test_dsiUnits.py`

 * *Files 19% similar despite different names*

```diff
@@ -130,32 +130,32 @@
     assert dsiUnit(r'\metre').toLatex(wrapper='$', prefix=r'\mathrm{Unit: }', suffix=r'\mathrm{(generated from D-SI string)}') == r'$\mathrm{Unit: }\mathrm{m}\mathrm{(generated from D-SI string)}$'
     parserWrapper = dsiParser(latexDefaultWrapper="&")
     assert parserWrapper.parse(r'\metre').toLatex() == r'&\mathrm{m}&'
     parserFull = dsiParser(latexDefaultWrapper='@', latexDefaultPrefix=r'\mathrm{Prefix}', latexDefaultSuffix=r'\mathrm{Suffix}')
     assert parserFull.parse(r'\metre').toLatex() == r'@\mathrm{Prefix}\mathrm{m}\mathrm{Suffix}@'
 
 def test_getClosestMatch():
-    closestMatch = _getClosestStr('\kiilo')
+    closestMatch = _getClosestStr(r'\kiilo')
     assert closestMatch == (['kilo'])
-    closestMatch = _getClosestStr('\mettre')
+    closestMatch = _getClosestStr(r'\mettre')
     assert closestMatch == (['metre'])
     closestMatch = _getClosestStr(r'\ttothe')
     assert closestMatch == (['tothe'])
 
 def test_info():
     p=dsiParser()
     infoStr, dsiVersion, dsiSchemaUrl, dsiRepositoryURL =p.info()
     #assert infoStr == "D-SI Parser Version: "+ str(dsiParser)+ "using D-SI Schema Version: "+ str(dsiParser._dsiParser__dsiVersion)+ "from: "+ str(dsiParser._dsiParser__dsiRepositoryURL)+ "using D-SI Schema: "+ str(dsiParser._dsiParser__dsiSchemaUrl)
     assert dsiVersion == dsiParser._dsiParser__dsiVersion
     assert dsiSchemaUrl == dsiParser._dsiParser__dsiSchemaUrl
     assert dsiRepositoryURL == dsiParser._dsiParser__dsiRepositoryURL
 
 def test_fractionalPowers():
-    assert dsiUnit(r'\metre\tothe{0.3333333333333333333}').toLatex(wrapper='') == r'\mathrm{m}\sqrt[3]{\mathrm{m}}'
-    assert dsiUnit(r'\metre\tothe{0.666666666666666}').toLatex(wrapper='') == r'\mathrm{m}\sqrt[3]{\mathrm{m}^{2}}'
+    assert dsiUnit(r'\metre\tothe{0.3333333333333333333}').toLatex(wrapper='') == r'\sqrt[3]{\mathrm{m}}'
+    assert dsiUnit(r'\metre\tothe{0.666666666666666}').toLatex(wrapper='') == r'\sqrt[3]{\mathrm{m}^{2}}'
 
 def test_baseUnitConversion():
     # Test conversion of a single derived unit to its base unit
     derivedUnitTree = dsiUnit(r'\kilo\metre')
     baseUnitTree = derivedUnitTree.toBaseUnitTree()
     assert baseUnitTree.tree == [[_node('', 'metre', '', scaleFactor=1000.0)]]
     assert baseUnitTree.toLatex() == '$$\\mathrm{m}$$'
@@ -385,8 +385,141 @@
     V=dsiUnit(r'\volt')
     mV = dsiUnit(r'\milli\volt')
     assert (V==mV)==False
     assert mV.isScalablyEqualTo(V)[0]==1000,dsiUnit(r'\volt')
     min=dsiUnit(r'\minute')
     s = dsiUnit(r'\second')
     assert (min==s)==False
-    assert s.isScalablyEqualTo(min)[0]==60,dsiUnit(r'\second')
+    assert s.isScalablyEqualTo(min)[0]==60,dsiUnit(r'\second')
+
+def test_oneMultiplication():
+    one=dsiUnit(r'\one')
+    m=dsiUnit(r'\metre')
+    assert one*m==m
+    assert m*one==m
+    assert m * one*one == m
+    assert m/one==m
+    assert m/one/one==m
+
+def test_onePower():
+    one=dsiUnit(r'\one')
+    m=dsiUnit(r'\metre')
+    assert one**2==one
+    assert one**0==one
+    assert m**0==one
+    assert m*one**1==m
+    assert m*one**2==m
+    assert m*one**3==m
+
+def test_negExponentToPer():
+    msToTheNegOne=dsiUnit(r'\metre\second\tothe{-1}')
+    mps=dsiUnit(r'\metre\per\second')
+    assert mps == msToTheNegOne.negExponentsToPer()
+
+def test_str_bits_bytes():
+    assert str(dsiUnit(r'\bit')) == r'\bit'
+    assert str(dsiUnit(r'\byte')) == r'\byte'
+    assert str(dsiUnit(r'\kibi\bit')) == r'\kibi\bit'
+    assert str(dsiUnit(r'\kibi\byte')) == r'\kibi\byte'
+    assert str(dsiUnit(r'\kibi\bit\tothe{2}')) == r'\kibi\bit\tothe{2}'
+    assert str(dsiUnit(r'\kibi\byte\tothe{2}')) == r'\kibi\byte\tothe{2}'
+    assert str(dsiUnit(r'\mebi\bit')) == r'\mebi\bit'
+    assert str(dsiUnit(r'\mebi\byte')) == r'\mebi\byte'
+    assert str(dsiUnit(r'\gibi\bit')) == r'\gibi\bit'
+    assert str(dsiUnit(r'\gibi\byte')) == r'\gibi\byte'
+    assert str(dsiUnit(r'\tebi\bit')) == r'\tebi\bit'
+    assert str(dsiUnit(r'\tebi\byte')) == r'\tebi\byte'
+    assert str(dsiUnit(r'\pebi\bit')) == r'\pebi\bit'
+    assert str(dsiUnit(r'\pebi\byte')) == r'\pebi\byte'
+    assert str(dsiUnit(r'\exbi\bit')) == r'\exbi\bit'
+    assert str(dsiUnit(r'\exbi\byte')) == r'\exbi\byte'
+    assert str(dsiUnit(r'\zebi\bit')) == r'\zebi\bit'
+    assert str(dsiUnit(r'\zebi\byte')) == r'\zebi\byte'
+    assert str(dsiUnit(r'\yobi\bit')) == r'\yobi\bit'
+    assert str(dsiUnit(r'\yobi\byte')) == r'\yobi\byte'
+    assert str(dsiUnit(r'\kibi\bit\tothe{2}\per\byte')) == r'\kibi\bit\tothe{2}\per\byte'
+    assert str(dsiUnit(r'\kibi\byte\tothe{-2}')) == r'\kibi\byte\tothe{-2}'
+    assert str(dsiUnit(r'\mebi\bit\tothe{0.5}')) == r'\mebi\bit\tothe{0.5}'
+    assert str(dsiUnit(r'\gibi\byte\tothe{0.333333333333333}')) == r'\gibi\byte\tothe{0.333333}'
+    assert str(dsiUnit(r'\tebi\bit\tothe{0.666666666666666}')) == r'\tebi\bit\tothe{0.666667}'
+    assert str(dsiUnit(r'\pebi\byte\tothe{1337}')) == r'\pebi\byte\tothe{1337}'
+
+def test_digitalUnitsScalebility():
+    bit=dsiUnit(r'\bit')
+    byte=dsiUnit(r'\byte')
+    kibiBit=dsiUnit(r'\kibi\bit')
+    kibiByte=dsiUnit(r'\kibi\byte')
+    mebiBit=dsiUnit(r'\mebi\bit')
+    mebiByte=dsiUnit(r'\mebi\byte')
+    gibiBit=dsiUnit(r'\gibi\bit')
+    gibiByte=dsiUnit(r'\gibi\byte')
+    tebiBit=dsiUnit(r'\tebi\bit')
+    tebiByte=dsiUnit(r'\tebi\byte')
+    pebiBit=dsiUnit(r'\pebi\bit')
+    pebiByte=dsiUnit(r'\pebi\byte')
+    exbiBit=dsiUnit(r'\exbi\bit')
+    exbiByte=dsiUnit(r'\exbi\byte')
+    zebiBit=dsiUnit(r'\zebi\bit')
+    zebiByte=dsiUnit(r'\zebi\byte')
+    yobiBit=dsiUnit(r'\yobi\bit')
+    yobiByte=dsiUnit(r'\yobi\byte')
+    assert bit.isScalablyEqualTo(byte)[0]==8
+    assert kibiBit.isScalablyEqualTo(kibiByte)[0]==8
+    assert mebiBit.isScalablyEqualTo(mebiByte)[0]==8
+    assert gibiBit.isScalablyEqualTo(gibiByte)[0]==8
+    assert tebiBit.isScalablyEqualTo(tebiByte)[0]==8
+    assert pebiBit.isScalablyEqualTo(pebiByte)[0]==8
+    assert exbiBit.isScalablyEqualTo(exbiByte)[0]==8
+    assert zebiBit.isScalablyEqualTo(zebiByte)[0]==8
+    assert yobiBit.isScalablyEqualTo(yobiByte)[0]==8
+    assert bit.isScalablyEqualTo(kibiBit)[0]==1024
+    assert bit.isScalablyEqualTo(mebiBit)[0]==1048576
+    assert bit.isScalablyEqualTo(gibiBit)[0]==1073741824
+    assert bit.isScalablyEqualTo(tebiBit)[0]==1099511627776
+    assert bit.isScalablyEqualTo(pebiBit)[0]==1125899906842624
+    assert bit.isScalablyEqualTo(exbiBit)[0]==1152921504606846976
+    assert bit.isScalablyEqualTo(zebiBit)[0]==1180591620717411303424
+    assert bit.isScalablyEqualTo(yobiBit)[0]==1208925819614629174706176
+    assert byte.isScalablyEqualTo(kibiByte)[0]==1024
+    assert byte.isScalablyEqualTo(mebiByte)[0]==1048576
+    assert byte.isScalablyEqualTo(gibiByte)[0]==1073741824
+    assert byte.isScalablyEqualTo(tebiByte)[0]==1099511627776
+    assert byte.isScalablyEqualTo(pebiByte)[0]==1125899906842624
+    assert byte.isScalablyEqualTo(exbiByte)[0]==1152921504606846976
+    assert byte.isScalablyEqualTo(zebiByte)[0]==1180591620717411303424
+    assert byte.isScalablyEqualTo(yobiByte)[0]==1208925819614629174706176
+    assert kibiBit.isScalablyEqualTo(mebiBit)[0]==1024
+    assert kibiBit.isScalablyEqualTo(gibiBit)[0]==1048576
+    assert kibiBit.isScalablyEqualTo(tebiBit)[0]==1073741824
+    assert kibiBit.isScalablyEqualTo(pebiBit)[0]==1099511627776
+    assert kibiBit.isScalablyEqualTo(exbiBit)[0]==1125899906842624
+    assert kibiBit.isScalablyEqualTo(zebiBit)[0]==1152921504606846976
+    assert kibiBit.isScalablyEqualTo(yobiBit)[0]==1180591620717411303424
+    assert mebiBit.isScalablyEqualTo(kibiByte)[0]==1/128
+    assert mebiBit.isScalablyEqualTo(kibiBit)[0] == 1 / 1024
+
+
+def test_scalability_relative_units():
+    percent = dsiUnit(r'\percent')
+    ppm = dsiUnit(r'\ppm')
+    one = dsiUnit(r'\one')
+
+    # Check scalability between percent and one
+    assert percent.isScalablyEqualTo(one, complete=True)[0] == 100
+    assert one.isScalablyEqualTo(percent, complete=True)[0] == 0.01
+
+    # Check scalability between ppm and one
+    assert ppm.isScalablyEqualTo(one, complete=True)[0] == 1e6
+    assert one.isScalablyEqualTo(ppm, complete=True)[0] == 1e-6
+
+    # Check scalability between percent and ppm
+    assert percent.isScalablyEqualTo(ppm, complete=True)[0]-1e-4<epsilon # damned 9.999999999999999e-05 != 0.0001
+    assert ppm.isScalablyEqualTo(percent, complete=True)[0] == 10000
+
+    # Additional checks to ensure conversions are precise
+    assert percent.isScalablyEqualTo(one, complete=True)[1] == dsiUnit(r'\one')
+    assert one.isScalablyEqualTo(percent, complete=True)[1] == dsiUnit(r'\one')
+    assert ppm.isScalablyEqualTo(one, complete=True)[1] == dsiUnit(r'\one')
+    assert one.isScalablyEqualTo(ppm, complete=True)[1] == dsiUnit(r'\one')
+    assert percent.isScalablyEqualTo(ppm, complete=True)[1] == dsiUnit(r'\one')
+    assert ppm.isScalablyEqualTo(percent, complete=True)[1] == dsiUnit(r'\one')
+
```

