# Comparing `tmp/lsst_felis-27.2024.1800.tar.gz` & `tmp/lsst_felis-27.2024.1900.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst_felis-27.2024.1800.tar", last modified: Thu May  2 10:02:04 2024, max compression
+gzip compressed data, was "lsst_felis-27.2024.1900.tar", last modified: Thu May  9 09:47:03 2024, max compression
```

## Comparing `lsst_felis-27.2024.1800.tar` & `lsst_felis-27.2024.1900.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:02:04.694639 lsst_felis-27.2024.1800/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-02 10:01:58.000000 lsst_felis-27.2024.1800/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-02 10:01:58.000000 lsst_felis-27.2024.1800/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-02 10:02:04.694639 lsst_felis-27.2024.1800/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-05-02 10:01:58.000000 lsst_felis-27.2024.1800/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-05-02 10:01:58.000000 lsst_felis-27.2024.1800/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:02:04.690639 lsst_felis-27.2024.1800/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:02:04.690639 lsst_felis-27.2024.1800/python/felis/
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-02 10:01:58.000000 lsst_felis-27.2024.1800/python/felis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10279 2024-05-02 10:01:58.000000 lsst_felis-27.2024.1800/python/felis/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    20540 2024-05-02 10:01:58.000000 lsst_felis-27.2024.1800/python/felis/datamodel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:02:04.694639 lsst_felis-27.2024.1800/python/felis/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 10:01:58.000000 lsst_felis-27.2024.1800/python/felis/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-02 10:01:58.000000 lsst_felis-27.2024.1800/python/felis/db/_variants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5735 2024-05-02 10:01:58.000000 lsst_felis-27.2024.1800/python/felis/db/sqltypes.py
--rw-r--r--   0 runner    (1001) docker     (127)    18907 2024-05-02 10:01:58.000000 lsst_felis-27.2024.1800/python/felis/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 10:01:58.000000 lsst_felis-27.2024.1800/python/felis/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    16795 2024-05-02 10:01:58.000000 lsst_felis-27.2024.1800/python/felis/tap.py
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-05-02 10:01:58.000000 lsst_felis-27.2024.1800/python/felis/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-05-02 10:01:58.000000 lsst_felis-27.2024.1800/python/felis/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-02 10:02:04.000000 lsst_felis-27.2024.1800/python/felis/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:02:04.694639 lsst_felis-27.2024.1800/python/lsst_felis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-02 10:02:04.000000 lsst_felis-27.2024.1800/python/lsst_felis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-02 10:02:04.000000 lsst_felis-27.2024.1800/python/lsst_felis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 10:02:04.000000 lsst_felis-27.2024.1800/python/lsst_felis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-02 10:02:04.000000 lsst_felis-27.2024.1800/python/lsst_felis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-02 10:02:04.000000 lsst_felis-27.2024.1800/python/lsst_felis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-02 10:02:04.000000 lsst_felis-27.2024.1800/python/lsst_felis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 10:02:04.000000 lsst_felis-27.2024.1800/python/lsst_felis.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-02 10:02:04.694639 lsst_felis-27.2024.1800/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:02:04.694639 lsst_felis-27.2024.1800/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-05-02 10:01:58.000000 lsst_felis-27.2024.1800/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    22923 2024-05-02 10:01:58.000000 lsst_felis-27.2024.1800/tests/test_datamodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-05-02 10:01:58.000000 lsst_felis-27.2024.1800/tests/test_datatypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9328 2024-05-02 10:01:58.000000 lsst_felis-27.2024.1800/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-02 10:01:58.000000 lsst_felis-27.2024.1800/tests/test_tap.py
--rw-r--r--   0 runner    (1001) docker     (127)     9320 2024-05-02 10:01:58.000000 lsst_felis-27.2024.1800/tests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:47:03.492851 lsst_felis-27.2024.1900/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-09 09:46:57.000000 lsst_felis-27.2024.1900/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-09 09:46:57.000000 lsst_felis-27.2024.1900/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-09 09:47:03.492851 lsst_felis-27.2024.1900/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-05-09 09:46:57.000000 lsst_felis-27.2024.1900/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-05-09 09:46:57.000000 lsst_felis-27.2024.1900/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:47:03.484851 lsst_felis-27.2024.1900/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:47:03.488851 lsst_felis-27.2024.1900/python/felis/
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-09 09:46:57.000000 lsst_felis-27.2024.1900/python/felis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10279 2024-05-09 09:46:57.000000 lsst_felis-27.2024.1900/python/felis/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21351 2024-05-09 09:46:57.000000 lsst_felis-27.2024.1900/python/felis/datamodel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:47:03.488851 lsst_felis-27.2024.1900/python/felis/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 09:46:57.000000 lsst_felis-27.2024.1900/python/felis/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-09 09:46:57.000000 lsst_felis-27.2024.1900/python/felis/db/_variants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5735 2024-05-09 09:46:57.000000 lsst_felis-27.2024.1900/python/felis/db/sqltypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18907 2024-05-09 09:46:57.000000 lsst_felis-27.2024.1900/python/felis/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 09:46:57.000000 lsst_felis-27.2024.1900/python/felis/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    16795 2024-05-09 09:46:57.000000 lsst_felis-27.2024.1900/python/felis/tap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-05-09 09:46:57.000000 lsst_felis-27.2024.1900/python/felis/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-05-09 09:46:57.000000 lsst_felis-27.2024.1900/python/felis/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-09 09:47:03.000000 lsst_felis-27.2024.1900/python/felis/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:47:03.488851 lsst_felis-27.2024.1900/python/lsst_felis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-09 09:47:03.000000 lsst_felis-27.2024.1900/python/lsst_felis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-09 09:47:03.000000 lsst_felis-27.2024.1900/python/lsst_felis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 09:47:03.000000 lsst_felis-27.2024.1900/python/lsst_felis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-09 09:47:03.000000 lsst_felis-27.2024.1900/python/lsst_felis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-09 09:47:03.000000 lsst_felis-27.2024.1900/python/lsst_felis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 09:47:03.000000 lsst_felis-27.2024.1900/python/lsst_felis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 09:47:03.000000 lsst_felis-27.2024.1900/python/lsst_felis.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-09 09:47:03.492851 lsst_felis-27.2024.1900/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:47:03.488851 lsst_felis-27.2024.1900/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-05-09 09:46:57.000000 lsst_felis-27.2024.1900/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22986 2024-05-09 09:46:57.000000 lsst_felis-27.2024.1900/tests/test_datamodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-05-09 09:46:57.000000 lsst_felis-27.2024.1900/tests/test_datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9328 2024-05-09 09:46:57.000000 lsst_felis-27.2024.1900/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-09 09:46:57.000000 lsst_felis-27.2024.1900/tests/test_tap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9453 2024-05-09 09:46:57.000000 lsst_felis-27.2024.1900/tests/test_validation.py
```

### Comparing `lsst_felis-27.2024.1800/LICENSE` & `lsst_felis-27.2024.1900/LICENSE`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.1800/PKG-INFO` & `lsst_felis-27.2024.1900/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-felis
-Version: 27.2024.1800
+Version: 27.2024.1900
 Summary: A vocabulary for describing catalogs and acting on those descriptions
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Homepage, https://felis.lsst.io
 Project-URL: Source, https://github.com/lsst/felis
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
```

### Comparing `lsst_felis-27.2024.1800/README.rst` & `lsst_felis-27.2024.1900/README.rst`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.1800/pyproject.toml` & `lsst_felis-27.2024.1900/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.1800/python/felis/__init__.py` & `lsst_felis-27.2024.1900/python/felis/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.1800/python/felis/cli.py` & `lsst_felis-27.2024.1900/python/felis/cli.py`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.1800/python/felis/datamodel.py` & `lsst_felis-27.2024.1900/python/felis/datamodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,15 +174,15 @@
 
 class Column(BaseObject):
     """A column in a table."""
 
     datatype: DataType
     """The datatype of the column."""
 
-    length: int | None = None
+    length: int | None = Field(None, gt=0)
     """The length of the column."""
 
     nullable: bool = True
     """Whether the column can be ``NULL``."""
 
     value: str | int | float | bool | None = None
     """The default value of the column."""
@@ -272,14 +272,36 @@
             try:
                 units.Unit(unit)
             except ValueError as e:
                 raise ValueError(f"Invalid unit: {e}")
 
         return values
 
+    @model_validator(mode="before")
+    @classmethod
+    def check_length(cls, values: dict[str, Any]) -> dict[str, Any]:
+        """Check that a valid length is provided for sized types."""
+        datatype = values.get("datatype")
+        if datatype is None:
+            # Skip this validation if datatype is not provided
+            return values
+        length = values.get("length")
+        felis_type = FelisType.felis_type(datatype)
+        if felis_type.is_sized and length is None:
+            raise ValueError(
+                f"Length must be provided for type '{datatype}'"
+                + (f" in column '{values['@id']}'" if "@id" in values else "")
+            )
+        elif not felis_type.is_sized and length is not None:
+            logger.warning(
+                f"The datatype '{datatype}' does not support a specified length"
+                + (f" in column '{values['@id']}'" if "@id" in values else "")
+            )
+        return values
+
     @model_validator(mode="after")
     def check_datatypes(self, info: ValidationInfo) -> Column:
         """Check for redundant datatypes on columns."""
         context = info.context
         if not context or not context.get("check_redundant_datatypes", False):
             return self
         if all(getattr(self, f"{dialect}:datatype", None) is not None for dialect in _DIALECTS.keys()):
@@ -287,18 +309,15 @@
 
         datatype = self.datatype
         length: int | None = self.length or None
 
         datatype_func = get_type_func(datatype)
         felis_type = FelisType.felis_type(datatype)
         if felis_type.is_sized:
-            if length is not None:
-                datatype_obj = datatype_func(length)
-            else:
-                raise ValueError(f"Length must be provided for sized type '{datatype}' in column '{self.id}'")
+            datatype_obj = datatype_func(length)
         else:
             datatype_obj = datatype_func()
 
         for dialect_name, dialect in _DIALECTS.items():
             db_annotation = f"{dialect_name}_datatype"
             if datatype_string := self.model_dump().get(db_annotation):
                 db_datatype_obj = string_to_typeengine(datatype_string, dialect, length)
```

### Comparing `lsst_felis-27.2024.1800/python/felis/db/_variants.py` & `lsst_felis-27.2024.1900/python/felis/db/_variants.py`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.1800/python/felis/db/sqltypes.py` & `lsst_felis-27.2024.1900/python/felis/db/sqltypes.py`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.1800/python/felis/metadata.py` & `lsst_felis-27.2024.1900/python/felis/metadata.py`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.1800/python/felis/tap.py` & `lsst_felis-27.2024.1900/python/felis/tap.py`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.1800/python/felis/types.py` & `lsst_felis-27.2024.1900/python/felis/types.py`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.1800/python/felis/validation.py` & `lsst_felis-27.2024.1900/python/felis/validation.py`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.1800/python/lsst_felis.egg-info/PKG-INFO` & `lsst_felis-27.2024.1900/python/lsst_felis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-felis
-Version: 27.2024.1800
+Version: 27.2024.1900
 Summary: A vocabulary for describing catalogs and acting on those descriptions
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Homepage, https://felis.lsst.io
 Project-URL: Source, https://github.com/lsst/felis
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
```

### Comparing `lsst_felis-27.2024.1800/python/lsst_felis.egg-info/SOURCES.txt` & `lsst_felis-27.2024.1900/python/lsst_felis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.1800/tests/test_cli.py` & `lsst_felis-27.2024.1900/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.1800/tests/test_datamodel.py` & `lsst_felis-27.2024.1900/tests/test_datamodel.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,21 +69,21 @@
 
         # Setting name and id should throw an exception from missing datatype.
         with self.assertRaises(ValidationError):
             Column(name="testColumn", id="#test_id")
 
         # Setting name, id, and datatype should not throw an exception and
         # should load data correctly.
-        col = Column(name="testColumn", id="#test_id", datatype="string")
+        col = Column(name="testColumn", id="#test_id", datatype="string", length=256)
         self.assertEqual(col.name, "testColumn", "name should be 'testColumn'")
         self.assertEqual(col.id, "#test_id", "id should be '#test_id'")
         self.assertEqual(col.datatype, DataType.string, "datatype should be 'DataType.string'")
 
         # Creating from data dictionary should work and load data correctly.
-        data = {"name": "testColumn", "id": "#test_id", "datatype": "string"}
+        data = {"name": "testColumn", "id": "#test_id", "datatype": "string", "length": 256}
         col = Column(**data)
         self.assertEqual(col.name, "testColumn", "name should be 'testColumn'")
         self.assertEqual(col.id, "#test_id", "id should be '#test_id'")
         self.assertEqual(col.datatype, DataType.string, "datatype should be 'DataType.string'")
 
         # Setting a bad IVOA UCD should throw an error.
         with self.assertRaises(ValidationError):
@@ -418,15 +418,15 @@
         with self.assertRaises(ValidationError):
             Table(name="testTable")
 
         # Setting name and id should throw an exception from missing columns.
         with self.assertRaises(ValidationError):
             Index(name="testTable", id="#test_id")
 
-        testCol = Column(name="testColumn", id="#test_id", datatype="string")
+        testCol = Column(name="testColumn", id="#test_id", datatype="string", length=256)
 
         # Setting name, id, and columns should not throw an exception and
         # should load data correctly.
         tbl = Table(name="testTable", id="#test_id", columns=[testCol])
         self.assertEqual(tbl.name, "testTable", "name should be 'testTable'")
         self.assertEqual(tbl.id, "#test_id", "id should be '#test_id'")
         self.assertEqual(tbl.columns, [testCol], "columns should be ['testColumn']")
@@ -449,15 +449,15 @@
         with self.assertRaises(ValidationError):
             Schema(name="testSchema")
 
         # Setting name and id should throw an exception from missing columns.
         with self.assertRaises(ValidationError):
             Schema(name="testSchema", id="#test_id")
 
-        test_col = Column(name="testColumn", id="#test_col_id", datatype="string")
+        test_col = Column(name="testColumn", id="#test_col_id", datatype="string", length=256)
         test_tbl = Table(name="testTable", id="#test_tbl_id", columns=[test_col])
 
         # Setting name, id, and columns should not throw an exception and
         # should load data correctly.
         sch = Schema(name="testSchema", id="#test_sch_id", tables=[test_tbl])
         self.assertEqual(sch.name, "testSchema", "name should be 'testSchema'")
         self.assertEqual(sch.id, "#test_sch_id", "id should be '#test_sch_id'")
@@ -487,15 +487,15 @@
                         ],
                     )
                 ],
             )
 
     def test_schema_object_ids(self) -> None:
         """Test that the id_map is properly populated."""
-        test_col = Column(name="testColumn", id="#test_col_id", datatype="string")
+        test_col = Column(name="testColumn", id="#test_col_id", datatype="string", length=256)
         test_tbl = Table(name="testTable", id="#test_table_id", columns=[test_col])
         sch = Schema(name="testSchema", id="#test_schema_id", tables=[test_tbl])
 
         for id in ["#test_col_id", "#test_table_id", "#test_schema_id"]:
             # Test that the schema contains the expected id.
             self.assertTrue(id in sch, f"schema should contain '{id}'")
```

### Comparing `lsst_felis-27.2024.1800/tests/test_datatypes.py` & `lsst_felis-27.2024.1900/tests/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.1800/tests/test_metadata.py` & `lsst_felis-27.2024.1900/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.1800/tests/test_tap.py` & `lsst_felis-27.2024.1900/tests/test_tap.py`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.1800/tests/test_validation.py` & `lsst_felis-27.2024.1900/tests/test_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
         # Creating a valid RSP column should not throw an exception.
         col = RspColumn(
             **{
                 "name": "testColumn",
                 "@id": "#test_col_id",
                 "datatype": "string",
                 "description": "test column",
+                "length": 256,
                 "tap:principal": 1,
             }
         )
 
         # Creating an empty RSP table should throw an exception.
         with self.assertRaises(ValidationError):
             RspTable()
@@ -187,14 +188,15 @@
                             RspColumn(
                                 **{
                                     "name": "testColumn",
                                     "@id": "#test_col1_id",
                                     "datatype": "string",
                                     "description": "test column",
                                     "tap:principal": 1,
+                                    "length": 256,
                                 }
                             )
                         ],
                     }
                 ),
                 RspTable(
                     **{
@@ -206,14 +208,15 @@
                             RspColumn(
                                 **{
                                     "name": "testColumn",
                                     "@id": "#test_col2_id",
                                     "datatype": "string",
                                     "description": "test column",
                                     "tap:principal": 1,
+                                    "length": 256,
                                 }
                             )
                         ],
                     }
                 ),
             ],
         )
```

