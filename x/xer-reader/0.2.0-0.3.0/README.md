# Comparing `tmp/xer_reader-0.2.0.tar.gz` & `tmp/xer_reader-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xer_reader-0.2.0.tar", max compression
+gzip compressed data, was "xer_reader-0.3.0.tar", max compression
```

## Comparing `xer_reader-0.2.0.tar` & `xer_reader-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2024-01-28 14:15:18.462715 xer_reader-0.2.0/LICENSE
--rw-r--r--   0        0        0     3484 2024-02-02 14:00:39.102685 xer_reader-0.2.0/README.md
--rw-r--r--   0        0        0      628 2024-02-01 03:49:02.308306 xer_reader-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      134 2024-02-01 03:49:20.864637 xer_reader-0.2.0/xer_reader/__init__.py
--rw-r--r--   0        0        0     9469 2024-02-01 03:47:45.531027 xer_reader-0.2.0/xer_reader/src/reader.py
--rw-r--r--   0        0        0     1008 2024-01-28 15:07:24.444772 xer_reader-0.2.0/xer_reader/src/table.py
--rw-r--r--   0        0        0     9037 2024-01-28 14:15:18.462715 xer_reader-0.2.0/xer_reader/src/table_data.py
--rw-r--r--   0        0        0     4361 1970-01-01 00:00:00.000000 xer_reader-0.2.0/setup.py
--rw-r--r--   0        0        0     4211 1970-01-01 00:00:00.000000 xer_reader-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-01-28 14:15:18.462715 xer_reader-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3484 2024-02-02 14:00:39.102685 xer_reader-0.3.0/README.md
+-rw-r--r--   0        0        0      628 2024-05-16 14:42:29.117116 xer_reader-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      137 2024-05-16 14:42:49.537221 xer_reader-0.3.0/xer_reader/__init__.py
+-rw-r--r--   0        0        0     8691 2024-03-06 14:12:50.215444 xer_reader-0.3.0/xer_reader/src/reader.py
+-rw-r--r--   0        0        0     4130 2024-05-16 13:57:14.961422 xer_reader-0.3.0/xer_reader/src/table.py
+-rw-r--r--   0        0        0     9037 2024-01-28 14:15:18.462715 xer_reader-0.3.0/xer_reader/src/table_data.py
+-rw-r--r--   0        0        0     4361 1970-01-01 00:00:00.000000 xer_reader-0.3.0/setup.py
+-rw-r--r--   0        0        0     4211 1970-01-01 00:00:00.000000 xer_reader-0.3.0/PKG-INFO
```

### Comparing `xer_reader-0.2.0/LICENSE` & `xer_reader-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xer_reader-0.2.0/README.md` & `xer_reader-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `xer_reader-0.2.0/pyproject.toml` & `xer_reader-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xer-reader"
-version = "0.2.0"
+version = "0.3.0"
 description = "Read and parse a Primavera P6 xer file."
 authors = ["Jesse Jones <code@seqmanagement.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 keywords = ["primavera", "p6", "xer", "schedule", "scheduling", "planning", "project management", "project controls"]
 repository = "https://github.com/jjCode01/xer-reader"
```

### Comparing `xer_reader-0.2.0/xer_reader/src/reader.py` & `xer_reader-0.3.0/xer_reader/src/reader.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,44 +10,40 @@
 from datetime import datetime
 from pathlib import Path
 from typing import BinaryIO
 
 from openpyxl import Workbook
 from openpyxl.worksheet.table import Table
 
-from xer_reader.src.table import Table as XerTable
+from xer_reader.src.table import XerTable
 from xer_reader.src.table_data import table_data
 
-REQUIRED_TABLES = {"CALENDAR", "CURRTYPE", "PROJECT", "PROJWBS"}
 DATE_FORMAT = "%Y-%m-%d"
+REQUIRED_TABLES = {"CALENDAR", "CURRTYPE", "PROJECT", "PROJWBS"}
 
 
 class XerReader:
-    """Open a XER file exported from Primavera P6 and read its contents."""
+    """Open an XER file exported from Primavera P6 and read its contents."""
 
     CODEC = "cp1252"
     file_name: str
     """XER file name"""
-
     data: str
-    """XER file data as tab seperated text"""
+    """XER file raw data as tab seperated text"""
 
     def __init__(self, file: str | Path | BinaryIO) -> None:
         self.file_name, self.data = _read_file(file)
 
         _file_info = _parse_file_info(self.data)
         self.currency: str = _file_info[7]
         """(str) Currency type set in P6"""
-
         self.export_version: str = _file_info[0]
         """(str) P6 Version"""
-
         self.export_date: datetime = datetime.strptime(_file_info[1], DATE_FORMAT)
         """(datetime) Date the XER file was exported"""
-
         self.export_user: str = _file_info[4]
         """(str) P6 user name that exported the XER file"""
 
     def check_errors(self) -> list[str]:
         """Check XER file for missing tables and orphan data
 
         Returns:
@@ -55,39 +51,39 @@
         """
         errors = set()
 
         id_map = {
             data["key"]: table for table, data in table_data.items() if data["key"]
         }
 
-        tables = self.parse_tables()
+        tables = self.to_dict()
 
         # Check for minimum tables required to be in the XER
         for name in REQUIRED_TABLES:
             if name not in tables:
                 errors.add(f"Missing Required Table {name}")
 
         # Check for required table pairs
         for table in tables.values():
             for table2 in table.depends:
                 if table2 not in tables:
                     errors.add(f"Missing Table {table2} Required for Table {table}")
 
-            for row in table.entries:
+            for row in table.entries():
                 for key, val in row.items():
                     if val == "":
                         continue
                     if not key.endswith("_id"):
                         continue
                     if key == "parent_wbs_id" and row["proj_node_flag"] == "Y":
                         continue
                     clean_key = key if key in id_map else _clean_foreign_key_label(key)
                     if clean_key:
                         if check_table := tables.get(id_map[clean_key]):
-                            for entry in check_table.entries:
+                            for entry in check_table.entries():
                                 if entry.get(clean_key, "") == val:
                                     break
                             else:
                                 errors.add(
                                     f"Orphan data {key} [{val}] in table {table}"
                                 )
 
@@ -143,80 +139,79 @@
             table_name (str): table name
 
         Returns:
             bool: True if found; False if not found
         """
         return f"%T\t{table_name.upper()}" in self.data
 
-    def parse_tables(self) -> dict[str, XerTable]:
+    def to_dict(self) -> dict[str, XerTable]:
         """
         Parse tables into a dictionary with the table name as the key
         and a `Table` object as the value.
 
         Returns:
             dict[str, Table]: dict of XER Tables
         """
         tables = {}
         for table_str in self.data.split("%T\t")[1:]:
-            name, table = _parse_table(table_str)
-            tables[name] = table
+            table = XerTable(table_str)
+            tables[table.name] = table
         return tables
 
     def to_csv(self, file_directory: str | Path = Path.cwd()) -> None:
         """
         Generate a CSV file for each table in the XER file.
         Uses `tab` as the delimiter.
 
         Args:
             file_directory (str | Path, optional): Directory to save CSV files.
             Defaults to current working directory.
         """
-        for table in self.parse_tables().values():
+        for table in self.to_dict().values():
             _write_table_to_csv(
                 f"{self.file_name}_{table.name}", table, Path(file_directory)
             )
 
-    def to_excel(self) -> None:
+    def to_excel(self, file_directory: str | Path = Path.cwd()) -> None:
         """
         Generate an Excel file with each table in the XER file on a seperate worksheet.
 
         """
         wb = Workbook()
         ws = wb.active
         ws.title = "ERMHDR"
         ws.append(_parse_file_info(self.data))
 
-        for name, table in self.parse_tables().items():
+        for name, table in self.to_dict().items():
             new_ws = wb.create_sheet(name)
             new_ws.append(table.labels)
-            for entry in table.entries:
-                new_ws.append(list(entry.values()))
+            for entry in table.rows:
+                new_ws.append(entry)
 
             tab = Table(displayName=name, ref=new_ws.calculate_dimension())
 
             new_ws.add_table(tab)
 
-        wb.save(f"{self.file_name}.xlsx")
+        wb.save(Path(file_directory, f"{self.file_name}.xlsx"))
 
     def to_json(self, *tables: str) -> str:
         """Generate a json compliant string representation of tables in the XER file
 
         Returns:
             str: json compliant string representation of XER tables
         """
         out_data = {}
         if not tables:
             out_data = {
-                name: _entry_by_key(table)
-                for name, table in self.parse_tables().items()
+                name: _entry_by_key(table) for name, table in self.to_dict().items()
             }
         else:
             out_data = {
                 name: _entry_by_key(table)
-                for name, table in self.parse_tables().items()
+                for name, table in self.to_dict().items()
                 if name in tables
             }
         json_data = {self.file_name: {**out_data}}
         return json.dumps(json_data, indent=2)
 
 
 def _clean_foreign_key_label(label: str) -> str | None:
@@ -225,36 +220,26 @@
         if label.startswith(prefix):
             return label.replace(prefix, "")
     return
 
 
 def _entry_by_key(table: XerTable) -> dict | list:
     if not table.key:
-        return table.entries
-    return {entry[table.key]: entry for entry in table.entries}
+        return table.entries(serialize=True)
+    return {entry[table.key]: entry for entry in table.entries(serialize=True)}
 
 
 def _parse_file_info(data: str) -> list[str]:
     """Parse file header"""
     ermhdr = re.search(r"(?<=ERMHDR\t).+", data)
     if not ermhdr:
         raise ValueError("Invalid XER File")
     return ermhdr.group().split("\t")
 
 
-def _parse_table(table_data: str) -> tuple[str, XerTable]:
-    """Parse table name, columns, and rows"""
-
-    lines: list[str] = table_data.split("\n")
-    name = lines.pop(0).strip()  # First line is the table name
-    cols = lines.pop(0).strip().split("\t")[1:]  # Second line is the column labels
-    data = [dict(zip(cols, _split_row(row))) for row in lines if row.startswith("%R")]
-    return name, XerTable(name, cols, data)
-
-
 def _read_file(file: str | Path | BinaryIO) -> tuple[str, str]:
     file_contents = ""
     file_name = ""
     if isinstance(file, (str, Path)):
         # Path directory to file
         file_name = Path(file).stem
         with open(file, encoding=XerReader.CODEC, errors="ignore") as f:
@@ -266,29 +251,14 @@
 
     if not file_contents.startswith("ERMHDR"):
         raise ValueError("ValueError: invalid XER file")
 
     return file_name, file_contents
 
 
-def _split_row(row: str) -> list[str]:
-    """Splits row into values."""
-    row_values = row.split("\t")[1:]
-    if row_values:
-        row_values[-1] = _strip_value(row_values[-1])
-    return row_values
-
-
-def _strip_value(val: str) -> str:
-    """Strips white space from a value"""
-    if val == "":
-        return ""
-    return val.strip()
-
-
 def _write_table_to_csv(name: str, table: XerTable, file_directory: Path) -> None:
     with file_directory.joinpath(f"{name}.csv").open("w") as f:
-        writer = csv.DictWriter(f, fieldnames=table.labels, delimiter="\t")
-        writer.writeheader()
-        for row in table.entries:
+        writer = csv.writer(f, delimiter="\t")
+        writer.writerow(table.labels)
+        for row in table.rows:
             writer.writerow(row)
     f.close()
```

### Comparing `xer_reader-0.2.0/xer_reader/src/table_data.py` & `xer_reader-0.3.0/xer_reader/src/table_data.py`

 * *Files identical despite different names*

### Comparing `xer_reader-0.2.0/setup.py` & `xer_reader-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['openpyxl>=3.1.2,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['test = scripts:test']}
 
 setup_kwargs = {
     'name': 'xer-reader',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': 'Read and parse a Primavera P6 xer file.',
     'long_description': '# Xer-Reader\n\nRead the contents of a Primavera P6 XER file using Python.  \n\nXer-Reader makes it easy to read, parse, and convert the data in a XER file to other formats.\n\n*Refer to the [Oracle Documentation]( https://docs.oracle.com/cd/F25600_01/English/Mapping_and_Schema/xer_import_export_data_map_project/index.htm) for more information regarding how data is mapped to the XER format.  \nTested on XER files exported as versions 15.2 through 19.12.*  \n\n## Install\n\n**Windows**:\n\n```bash\npip install xer-reader\n```\n\n**Linux/Mac**:\n\n```bash\npip3 install xer-reader\n```\n\n## Usage  \n\nImport the `XerReader` class from `xer_reader`.\n```python\nfrom xer_reader import XerReader\n```\n\nCreate a new instance of an `XerReader` object by passing in the XER file as an argument. `XerReader` can accept the file path represented as a `str` or pathlib `Path` object, or a Binary file received as a response from requests, Flask, FastAPI, etc...\n\n```python\nfile = r"/path/to/file.xer"\nreader = XerReader(file)\n```\n\n### Attributes  \n\n* `data` [str] - *The contents of the XER file as a string.*\n* `export_date` [datetime] - *The date the XER file was exported.*\n* `export_user` [str] - *The P6 user who export the XER file.*\n* `export_version` [str] - *The P6 verison used to export the XER file.*\n* `file_name` [str] - *The name of the file without the \'.xer\' extension.*\n\n### Methods\n\n**`check_errors()`** -> *list[str]*  \nChecks the XER file for missing tables and orphan data, and returns the results as a list of errors.  \n\n* Missing tables can occur when an entry in *Table 1* points to an entry in *Table 2* but *Table 2* does not exist at all.\n* Orphan data occurs when an entry in *Table 1* points to an entry *Table 2* but the entry in *Table 2* does not exist.\n\n**`delete_tables(*table_names: str)`** -> *str*  \nDelete a variable number of tables (*table_names*) from the XER file data and returns a new string (*Does not modify `XerReader.data` attribute*).  \n\nIn the following example the tables associated with User Defined Fields are removed from the XER file contents and stored in a new variable `new_xer_data`, which can then be written to a new XER file:\n```python\nnew_xer_data = reader.delete_tables("UDFTYPE", "UDFVALUE")\n\nwith open("New_XER.xer", "w", encoding=XerReader.CODEC) as new_xer_file:\n    new_xer_file.write(new_xer_data)\n```\n\n**`get_table_names()`** -> *list[str]*  \nReturns a list of table names included in the XER file.  \n\n**`get_table_str(table_name: str)`** -> *str*  \nReturns the tab seperated text for a specific table in the XER file.\n\n**`has_table(table_name: str)`** -> *bool*  \nReturn True if table (`table_name`) if found in the XER file.\n\n**`parse_tables()`** -> *dict[str, Table]*  \nReturns a dictionary with the table name as the key and a `Table` object as the value.  \n\n**`to_csv(file_directory: str | Path)`** -> *None*  \nGenerate a CSV file for each table in the XER file using \'tab\' as the delimiter. CSV files will be created in the current working directory.   \nOptional: Pass a string or Path object (`file_directory`) to speficy a folder to store the CSV files in.  \n\n**`to_excel()`** -> *None*  \nGenerate an Excel (.xlsx) file with each table in the XER file on its own spreadsheet. The Excel file will be create in the \ncurrent working directory.  \n\n**`to_json(*tables: str)`** -> *str*  \nGenerate a json compliant string representation of the tables in the XER file.  \nOptional: Pass in specific table names to include in the json string.\n',
     'author': 'Jesse Jones',
     'author_email': 'code@seqmanagement.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/jjCode01/xer-reader',
```

### Comparing `xer_reader-0.2.0/PKG-INFO` & `xer_reader-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xer-reader
-Version: 0.2.0
+Version: 0.3.0
 Summary: Read and parse a Primavera P6 xer file.
 Home-page: https://github.com/jjCode01/xer-reader
 License: GPL-3.0-only
 Keywords: primavera,p6,xer,schedule,scheduling,planning,project management,project controls
 Author: Jesse Jones
 Author-email: code@seqmanagement.com
 Requires-Python: >=3.10,<4.0
```

