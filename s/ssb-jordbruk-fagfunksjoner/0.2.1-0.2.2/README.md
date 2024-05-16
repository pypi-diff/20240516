# Comparing `tmp/ssb_jordbruk_fagfunksjoner-0.2.1.tar.gz` & `tmp/ssb_jordbruk_fagfunksjoner-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_jordbruk_fagfunksjoner-0.2.1.tar", max compression
+gzip compressed data, was "ssb_jordbruk_fagfunksjoner-0.2.2.tar", max compression
```

## Comparing `ssb_jordbruk_fagfunksjoner-0.2.1.tar` & `ssb_jordbruk_fagfunksjoner-0.2.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2024-05-07 06:04:31.155311 ssb_jordbruk_fagfunksjoner-0.2.1/LICENSE
--rw-r--r--   0        0        0     3215 2024-05-07 06:04:31.155311 ssb_jordbruk_fagfunksjoner-0.2.1/README.md
--rw-r--r--   0        0        0     4169 2024-05-07 06:04:40.739339 ssb_jordbruk_fagfunksjoner-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       34 2024-05-07 06:04:31.155311 ssb_jordbruk_fagfunksjoner-0.2.1/src/ssb_jordbruk_fagfunksjoner/__init__.py
--rw-r--r--   0        0        0      243 2024-05-07 06:04:31.155311 ssb_jordbruk_fagfunksjoner-0.2.1/src/ssb_jordbruk_fagfunksjoner/__main__.py
--rw-r--r--   0        0        0    14857 2024-05-07 06:04:40.739339 ssb_jordbruk_fagfunksjoner-0.2.1/src/ssb_jordbruk_fagfunksjoner/produksjonstilskudd.py
--rw-r--r--   0        0        0        0 2024-05-07 06:04:31.155311 ssb_jordbruk_fagfunksjoner-0.2.1/src/ssb_jordbruk_fagfunksjoner/py.typed
--rw-r--r--   0        0        0     4133 1970-01-01 00:00:00.000000 ssb_jordbruk_fagfunksjoner-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-16 09:26:03.343689 ssb_jordbruk_fagfunksjoner-0.2.2/LICENSE
+-rw-r--r--   0        0        0     3215 2024-05-16 09:26:03.343689 ssb_jordbruk_fagfunksjoner-0.2.2/README.md
+-rw-r--r--   0        0        0     4169 2024-05-16 09:26:13.059789 ssb_jordbruk_fagfunksjoner-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       34 2024-05-16 09:26:03.343689 ssb_jordbruk_fagfunksjoner-0.2.2/src/ssb_jordbruk_fagfunksjoner/__init__.py
+-rw-r--r--   0        0        0      243 2024-05-16 09:26:03.343689 ssb_jordbruk_fagfunksjoner-0.2.2/src/ssb_jordbruk_fagfunksjoner/__main__.py
+-rw-r--r--   0        0        0    15304 2024-05-16 09:26:13.059789 ssb_jordbruk_fagfunksjoner-0.2.2/src/ssb_jordbruk_fagfunksjoner/produksjonstilskudd.py
+-rw-r--r--   0        0        0        0 2024-05-16 09:26:03.347689 ssb_jordbruk_fagfunksjoner-0.2.2/src/ssb_jordbruk_fagfunksjoner/py.typed
+-rw-r--r--   0        0        0     4133 1970-01-01 00:00:00.000000 ssb_jordbruk_fagfunksjoner-0.2.2/PKG-INFO
```

### Comparing `ssb_jordbruk_fagfunksjoner-0.2.1/LICENSE` & `ssb_jordbruk_fagfunksjoner-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ssb_jordbruk_fagfunksjoner-0.2.1/README.md` & `ssb_jordbruk_fagfunksjoner-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `ssb_jordbruk_fagfunksjoner-0.2.1/pyproject.toml` & `ssb_jordbruk_fagfunksjoner-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssb-jordbruk-fagfunksjoner"
-version = "0.2.1"
+version = "0.2.2"
 description = "SSB Jordbruk Fagfunksjoner"
 authors = ["Magnus Theodor Engh <dor@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/statisticsnorway/ssb-jordbruk-fagfunksjoner"
 repository = "https://github.com/statisticsnorway/ssb-jordbruk-fagfunksjoner"
 documentation = "https://statisticsnorway.github.io/ssb-jordbruk-fagfunksjoner"
```

### Comparing `ssb_jordbruk_fagfunksjoner-0.2.1/src/ssb_jordbruk_fagfunksjoner/produksjonstilskudd.py` & `ssb_jordbruk_fagfunksjoner-0.2.2/src/ssb_jordbruk_fagfunksjoner/produksjonstilskudd.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         _setup_dynamic_attributes: Dynamically assigns categorized code groups and combinations as attributes for direct access.
         _extract_from_codelist(numbers): Utility method to extract codes based on provided criteria.
         get_codes(attributes, prefix): Retrieves a list of codes, optionally filtered by attributes and/or prefixed.
 
     Example:
         >>> pt = Produksjonstilskudd()
         >>> print(pt.get_codes('frukt_avling', prefix=True))
-        ['PK_001', 'PK_002', 'PK_003', 'PK_004', 'PK_005', 'PK_006']
+        ['pk_001', 'pk_002', 'pk_003', 'pk_004', 'pk_005', 'pk_006']
 
     Note:
         The class is designed with immutability in mind for the 'codes' attribute to ensure consistent and error-free usage.
     """
 
     codes: ClassVar[dict[str, str]] = {
         "001": "Epler",
@@ -248,83 +248,91 @@
             "fjørfe_og_rugeegg",
             "pelsdyr",
             "andre_husdyr",
         ],
         "frukt_baer_groennsaker": ["frukt", "baer", "groennsaker"],
     }
 
-    statbank_groups: ClassVar[dict[str, list[str]]] = {
-        "statbank_storfe": ["119", "120", "121"],
-        "statbank_ku": ["120", "121"],
-        "statbank_sau": ["145", "146", "139"],
-        "statbank_avlssvin": ["155", "156", "158", "159"],
-        "statbank_svin": ["154", "155", "156", "157", "158", "159"],
+    table_groups: ClassVar[dict[str, list[str]]] = {
+        "tabell_storfe": ["119", "120", "121"],  # brukes i statbank
+        "tabell_ku": ["120", "121"],  # brukes i statbank
+        "tabell_sau": ["145", "146", "139"],  # brukes i statbank
+        "tabell_avlssvin": ["155", "156", "158", "159"],  # brukes i statbank
+        "tabell_svin": ["154", "155", "156", "157", "158", "159"],  # brukes i statbank
+        "tabell_purker": ["155", "158"],  # brukes i statbank
+        "tabell_geit": ["140", "142", "144"],
+        "tabell_hest": ["115", "116"],
+        "tabell_pelsdyr": ["170", "171"],
+        "tabell_hjort": ["178", "179"],
+        "tabell_ok_storfe": ["801", "158", "803"],
+        "tabell_ok_ku": ["801", "802"],
+        "tabell_ok_mageit": ["810", "811"],
     }
 
     def __init__(self) -> None:
         """Initializes an instance of the Produksjonstilskudd class.
 
         This constructor method dynamically sets up class attributes based on predefined code groups and combinations. It organizes various agricultural product codes, including fruits, vegetables, and livestock, into easily accessible class attributes for further processing or querying.
         Upon instantiation, it calls the _setup_dynamic_attributes method to dynamically assign attributes to the instance based on the `code_groups` and `combinations` class variables. This setup allows for flexible manipulation and access to specific subsets of product codes.
-        Attributes are set up to facilitate extraction of codes with the option to prefix them with 'PK_', indicating a primary key or unique identifier, which can be used for database operations or internal logic.
+        Attributes are set up to facilitate extraction of codes with the option to prefix them with 'pk_', indicating a primary key or unique identifier, which can be used for database operations or internal logic.
 
         Example usage:
             pt = Produksjonstilskudd()
             print(pt.get_codes('frukt_avling', prefix=True))
 
-        The example above will print all fruit harvesting codes, prefixed with 'PK_', indicating that these codes are treated as unique identifiers.
+        The example above will print all fruit harvesting codes, prefixed with 'pk_', indicating that these codes are treated as unique identifiers.
         """
         self._setup_dynamic_attributes()
 
     def _setup_dynamic_attributes(self) -> None:
         # Set attributes for each code group
         for group_name, codes in self.code_groups.items():
             setattr(self, group_name, self._extract_from_codelist(codes))
 
         for combo_name, groups in self.combinations.items():
             combined_dict: dict[str, str] = {}
             for group in groups:
                 combined_dict.update(getattr(self, group, {}))
             setattr(self, combo_name, combined_dict)
 
-        for statbank_name, codes in self.statbank_groups.items():
-            setattr(self, statbank_name, self._extract_from_codelist(codes))
+        for table_name, codes in self.table_groups.items():
+            setattr(self, table_name, self._extract_from_codelist(codes))
 
     def _extract_from_codelist(self, numbers: list[str]) -> dict[str, str]:
         result = {}
         for code in numbers:
             if code not in self.codes:
                 raise ValueError(f"Code {code} not found in codes dictionary.")
             result[code] = self.codes[code]
         return result
 
     def get_codes(
         self, attributes: str | list[str] | None = None, prefix: bool | None = False
     ) -> list[str]:
         """Returns a list of 3-digit codes from the specified attributes.
 
-        If no attributes are specified, this method returns all 3-digit codes available. Optionally, a 'PK_' prefix can be added to each code.
+        If no attributes are specified, this method returns all 3-digit codes available. Optionally, a 'pk_' prefix can be added to each code.
 
         Parameters
         ----------
         attributes : None, str, or list of str, optional
             The attribute or list of attributes for which codes are to be retrieved. If `None`, codes for all attributes are returned.
         prefix : bool, optional
-            Indicates whether to add a 'PK_' prefix to each code. Default is `False`.
+            Indicates whether to add a 'pk_' prefix to each code. Default is `False`.
 
         Returns:
         -------
         list of str
-            A list containing the requested 3-digit codes, optionally prefixed with 'PK_'.
+            A list containing the requested 3-digit codes, optionally prefixed with 'pk_'.
 
         Examples:
         --------
         >>> pt = Produksjonstilskudd()
         >>> pt.get_codes('frukt_avling', prefix=True)
-        ['PK_001', 'PK_002', 'PK_003', 'PK_004', 'PK_005', 'PK_006']
+        ['pk_001', 'pk_002', 'pk_003', 'pk_004', 'pk_005', 'pk_006']
 
         >>> pt.get_codes()
         ['001', '002', '003', '004', '005', '006', '011', '012', '013', '014', '016', '021', '022', '031', '032', '033', '060', '115', '116', '118', '119', '120', '121', '139', '140', '142', '144', '145', '146', '154', '155', '156', '157', '158', '159', '161', '162', '168', '170', '171', '174', '175', '176', '178', '179', '180', '181', '183', '185', '192', '193', '194', '196', '197', '210', '211', '212', '213', '223', '230', '231', '235', '236', '237', '238', '239', '240', '242', '243', '245', '247', '264', '271', '272', '273', '274', '280', '282', '283', '285', '290', '292', '293', '294', '410', '411', '420', '422', '431', '432', '440', '445', '450', '455', '480', '481', '486', '487', '488', '521', '522', '523', '720', '721', '722', '723', '724', '725', '801', '802', '803', '810', '811', '821', '830', '833', '841', '852', '855', '861', '863', '864', '870', '871', '875', '876', '880', '881', '882']
         """
         if attributes:
             if isinstance(attributes, str):  # Single attribute name
                 attributes = [attributes]  # Convert to list for consistency
@@ -333,10 +341,10 @@
                 attribute_dict = getattr(self, attribute_name, {})
                 codes.extend(list(attribute_dict.keys()))
         else:
             # No specific attributes provided, return all 3-digit codes
             codes = list(self.codes.keys())
 
         if prefix:
-            return ["PK_" + code for code in codes]
+            return ["pk_" + code for code in codes]
         else:
             return codes
```

### Comparing `ssb_jordbruk_fagfunksjoner-0.2.1/PKG-INFO` & `ssb_jordbruk_fagfunksjoner-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssb-jordbruk-fagfunksjoner
-Version: 0.2.1
+Version: 0.2.2
 Summary: SSB Jordbruk Fagfunksjoner
 Home-page: https://github.com/statisticsnorway/ssb-jordbruk-fagfunksjoner
 License: MIT
 Author: Magnus Theodor Engh
 Author-email: dor@ssb.no
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

