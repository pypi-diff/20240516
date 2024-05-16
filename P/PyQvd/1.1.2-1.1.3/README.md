# Comparing `tmp/pyqvd-1.1.2.tar.gz` & `tmp/pyqvd-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqvd-1.1.2.tar", last modified: Mon Apr 22 10:52:48 2024, max compression
+gzip compressed data, was "pyqvd-1.1.3.tar", last modified: Thu May 16 15:06:05 2024, max compression
```

## Comparing `pyqvd-1.1.2.tar` & `pyqvd-1.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 10:52:48.066031 pyqvd-1.1.2/
--rw-rw-rw-   0        0        0     1096 2024-03-27 12:50:40.000000 pyqvd-1.1.2/LICENSE.md
--rw-rw-rw-   0        0        0    12492 2024-04-22 10:52:48.066031 pyqvd-1.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-22 10:52:48.066031 pyqvd-1.1.2/PyQvd.egg-info/
--rw-rw-rw-   0        0        0    12492 2024-04-22 10:52:48.000000 pyqvd-1.1.2/PyQvd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2024-04-22 10:52:48.000000 pyqvd-1.1.2/PyQvd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 10:52:48.000000 pyqvd-1.1.2/PyQvd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-04-22 10:52:48.000000 pyqvd-1.1.2/PyQvd.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-22 10:52:48.000000 pyqvd-1.1.2/PyQvd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10282 2024-04-07 10:48:20.000000 pyqvd-1.1.2/README.md
--rw-rw-rw-   0        0        0     1288 2024-04-22 10:50:26.000000 pyqvd-1.1.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-22 10:52:48.066031 pyqvd-1.1.2/pyqvd/
--rw-rw-rw-   0        0        0       88 2024-04-02 10:45:55.000000 pyqvd-1.1.2/pyqvd/__init__.py
--rw-rw-rw-   0        0        0    37201 2024-04-22 10:50:09.000000 pyqvd-1.1.2/pyqvd/qvd.py
--rw-rw-rw-   0        0        0       42 2024-04-22 10:52:48.066031 pyqvd-1.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-16 15:06:05.127341 pyqvd-1.1.3/
+-rw-rw-rw-   0        0        0     1096 2024-03-27 12:50:40.000000 pyqvd-1.1.3/LICENSE.md
+-rw-rw-rw-   0        0        0    12492 2024-05-16 15:06:05.126342 pyqvd-1.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-16 15:06:05.125334 pyqvd-1.1.3/PyQvd.egg-info/
+-rw-rw-rw-   0        0        0    12492 2024-05-16 15:06:05.000000 pyqvd-1.1.3/PyQvd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2024-05-16 15:06:05.000000 pyqvd-1.1.3/PyQvd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 15:06:05.000000 pyqvd-1.1.3/PyQvd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-05-16 15:06:05.000000 pyqvd-1.1.3/PyQvd.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-16 15:06:05.000000 pyqvd-1.1.3/PyQvd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10282 2024-04-07 10:48:20.000000 pyqvd-1.1.3/README.md
+-rw-rw-rw-   0        0        0     1288 2024-05-16 15:04:02.000000 pyqvd-1.1.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-16 15:06:05.123551 pyqvd-1.1.3/pyqvd/
+-rw-rw-rw-   0        0        0       88 2024-04-02 10:45:55.000000 pyqvd-1.1.3/pyqvd/__init__.py
+-rw-rw-rw-   0        0        0    38233 2024-05-16 15:03:41.000000 pyqvd-1.1.3/pyqvd/qvd.py
+-rw-rw-rw-   0        0        0       42 2024-05-16 15:06:05.128312 pyqvd-1.1.3/setup.cfg
```

### Comparing `pyqvd-1.1.2/LICENSE.md` & `pyqvd-1.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyqvd-1.1.2/PKG-INFO` & `pyqvd-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQvd
-Version: 1.1.2
+Version: 1.1.3
 Summary: Utility library for reading/writing Qlik View Data (QVD) files in Python.
 Author-email: Constantin Müller <info@mueller-constantin.de>
 License: MIT License
         
         Copyright (c) 2024 Constantin Müller
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyqvd-1.1.2/PyQvd.egg-info/PKG-INFO` & `pyqvd-1.1.3/PyQvd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQvd
-Version: 1.1.2
+Version: 1.1.3
 Summary: Utility library for reading/writing Qlik View Data (QVD) files in Python.
 Author-email: Constantin Müller <info@mueller-constantin.de>
 License: MIT License
         
         Copyright (c) 2024 Constantin Müller
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyqvd-1.1.2/README.md` & `pyqvd-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyqvd-1.1.2/pyproject.toml` & `pyqvd-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyQvd"
-version = "1.1.2"
+version = "1.1.3"
 description = "Utility library for reading/writing Qlik View Data (QVD) files in Python."
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE.md"}
 authors = [
     {name = "Constantin Müller", email = "info@mueller-constantin.de"},
 ]
 keywords = ["qlik", "qvd", "qlik sense", "qlik view", "pandas"]
```

### Comparing `pyqvd-1.1.2/pyqvd/qvd.py` & `pyqvd-1.1.3/pyqvd/qvd.py`

 * *Files 2% similar despite different names*

```diff
@@ -798,26 +798,33 @@
         self._symbol_buffer = b""
 
         for column_index, _ in enumerate(self._df.columns):
             # Uses a dictionary over a set to preserve the order of the values and over a loop for performance reasons
             unique_values = list(dict.fromkeys([row[column_index] for row in self._df.data]).keys())
 
             symbols = {}
+            contains_none = False
 
             for value in unique_values:
                 symbol = self._convert_raw_to_symbol(value)
+
+                # Skip None values, they are represented by bias shifted negative indices
+                if symbol is None:
+                    contains_none = True
+                    continue
+
                 symbols[symbol] = len(symbols)
 
             current_symbol_buffer = b"".join([symbol.to_byte_representation() for symbol in symbols])
             self._symbol_buffer += current_symbol_buffer
 
             symbols_length = len(current_symbol_buffer)
             symbols_offset = sum([self._symbol_table_metadata[index][1] for index in range(column_index)])
 
-            self._symbol_table_metadata[column_index] = (symbols_offset, symbols_length)
+            self._symbol_table_metadata[column_index] = (symbols_offset, symbols_length, contains_none)
             self._symbol_table[column_index] = symbols
 
     def _build_index_table(self):
         """
         Builds the index table of the QVD file.
         """
 
@@ -870,30 +877,42 @@
         for row_index, row in enumerate(self._df.data):
             indices = [None] * len(self._df.columns)
 
             for column_index, _ in enumerate(self._df.columns):
                 # Convert the raw values to indices referring to the symbol table
                 value = row[column_index]
                 symbol = self._convert_raw_to_symbol(value)
-                symbol_index = self._symbol_table[column_index][symbol]
+                field_contains_none = self._symbol_table_metadata[column_index][2]
+
+                # None values are represented by bias shifted negative indices
+                if symbol is None:
+                    symbol_index = 0
+                else:
+                    # In order to represent None values, the indices are shifted by the bias value of the column
+                    if field_contains_none:
+                        symbol_index = self._symbol_table[column_index][symbol] + 2
+                    else:
+                        symbol_index = self._symbol_table[column_index][symbol]
 
                 # Convert the integer indices to binary representation
                 index_bits = format(symbol_index, "b")
                 indices[column_index] = index_bits
 
             self._index_table[row_index] = indices
 
         # Normalize the bit representation of the indices by padding with zeros
         for column_index, _ in enumerate(self._df.columns):
+            field_contains_none = self._symbol_table_metadata[column_index][2]
             # Bit offset is the sum of the bit widths of all previous columns
             bit_offset = sum([self._index_table_metadata[index][1] for index in range(column_index)
                               if self._index_table_metadata[index] is not None])
             # Bit width is the maximum bit width of all indices of the column
             bit_width = max([len(bit_indices[column_index]) for bit_indices in self._index_table])
-            bias = 0
+            # Bias is used to shift the indices to represent None values
+            bias = -2 if field_contains_none else 0
             self._index_table_metadata[column_index] = (bit_offset, bit_width, bias)
 
             # Pad the bit representation of the indices with zeros to match the bit width
             for bit_indices in self._index_table:
                 bit_indices[column_index] = bit_indices[column_index].rjust(bit_width, "0")
 
         # Concatenate the bit representation of the indices of each row to a single binary string per row
@@ -914,14 +933,17 @@
     def _convert_raw_to_symbol(raw: any) -> QvdSymbol:
         """
         Converts a raw value to a QVD symbol.
 
         :param raw: The raw value.
         :return: The QVD symbol.
         """
+        if raw is None:
+            return None
+
         if isinstance(raw, int):
             return QvdSymbol.from_int_value(raw)
 
         if isinstance(raw, float):
             return QvdSymbol.from_double_value(raw)
 
         if isinstance(raw, str):
```

