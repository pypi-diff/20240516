# Comparing `tmp/iclean-0.0.3.tar.gz` & `tmp/iclean-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iclean-0.0.3.tar", last modified: Wed May 15 10:26:26 2024, max compression
+gzip compressed data, was "iclean-0.0.4.tar", last modified: Thu May 16 06:23:46 2024, max compression
```

## Comparing `iclean-0.0.3.tar` & `iclean-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 kaliv0    (1000) kaliv0    (1000)        0 2024-05-15 10:26:26.268011 iclean-0.0.3/
--rw-rw-r--   0 kaliv0    (1000) kaliv0    (1000)    35149 2024-05-08 18:25:37.000000 iclean-0.0.3/LICENSE
--rw-r--r--   0 kaliv0    (1000) kaliv0    (1000)    41205 2024-05-15 10:26:26.268011 iclean-0.0.3/PKG-INFO
--rw-rw-r--   0 kaliv0    (1000) kaliv0    (1000)      478 2024-05-14 16:22:30.000000 iclean-0.0.3/README.md
--rw-rw-r--   0 kaliv0    (1000) kaliv0    (1000)    10937 2024-05-15 10:26:13.000000 iclean-0.0.3/clean.py
-drwxrwxr-x   0 kaliv0    (1000) kaliv0    (1000)        0 2024-05-15 10:26:26.264011 iclean-0.0.3/iclean.egg-info/
--rw-r--r--   0 kaliv0    (1000) kaliv0    (1000)    41205 2024-05-15 10:26:26.000000 iclean-0.0.3/iclean.egg-info/PKG-INFO
--rw-rw-r--   0 kaliv0    (1000) kaliv0    (1000)      194 2024-05-15 10:26:26.000000 iclean-0.0.3/iclean.egg-info/SOURCES.txt
--rw-rw-r--   0 kaliv0    (1000) kaliv0    (1000)        1 2024-05-15 10:26:26.000000 iclean-0.0.3/iclean.egg-info/dependency_links.txt
--rw-rw-r--   0 kaliv0    (1000) kaliv0    (1000)       38 2024-05-15 10:26:26.000000 iclean-0.0.3/iclean.egg-info/entry_points.txt
--rw-rw-r--   0 kaliv0    (1000) kaliv0    (1000)        6 2024-05-15 10:26:26.000000 iclean-0.0.3/iclean.egg-info/top_level.txt
--rw-rw-r--   0 kaliv0    (1000) kaliv0    (1000)      392 2024-05-10 20:37:30.000000 iclean-0.0.3/pyproject.toml
--rw-rw-r--   0 kaliv0    (1000) kaliv0    (1000)       38 2024-05-15 10:26:26.268011 iclean-0.0.3/setup.cfg
+drwxrwxr-x   0 kaliv0    (1000) kaliv0    (1000)        0 2024-05-16 06:23:46.402310 iclean-0.0.4/
+-rw-rw-r--   0 kaliv0    (1000) kaliv0    (1000)    35149 2024-05-08 18:25:37.000000 iclean-0.0.4/LICENSE
+-rw-r--r--   0 kaliv0    (1000) kaliv0    (1000)    41213 2024-05-16 06:23:46.402310 iclean-0.0.4/PKG-INFO
+-rw-rw-r--   0 kaliv0    (1000) kaliv0    (1000)      478 2024-05-14 16:22:30.000000 iclean-0.0.4/README.md
+-rw-rw-r--   0 kaliv0    (1000) kaliv0    (1000)    11114 2024-05-16 06:22:42.000000 iclean-0.0.4/clean.py
+drwxrwxr-x   0 kaliv0    (1000) kaliv0    (1000)        0 2024-05-16 06:23:46.402310 iclean-0.0.4/iclean.egg-info/
+-rw-r--r--   0 kaliv0    (1000) kaliv0    (1000)    41213 2024-05-16 06:23:46.000000 iclean-0.0.4/iclean.egg-info/PKG-INFO
+-rw-rw-r--   0 kaliv0    (1000) kaliv0    (1000)      194 2024-05-16 06:23:46.000000 iclean-0.0.4/iclean.egg-info/SOURCES.txt
+-rw-rw-r--   0 kaliv0    (1000) kaliv0    (1000)        1 2024-05-16 06:23:46.000000 iclean-0.0.4/iclean.egg-info/dependency_links.txt
+-rw-rw-r--   0 kaliv0    (1000) kaliv0    (1000)       38 2024-05-16 06:23:46.000000 iclean-0.0.4/iclean.egg-info/entry_points.txt
+-rw-rw-r--   0 kaliv0    (1000) kaliv0    (1000)        6 2024-05-16 06:23:46.000000 iclean-0.0.4/iclean.egg-info/top_level.txt
+-rw-rw-r--   0 kaliv0    (1000) kaliv0    (1000)      401 2024-05-16 06:19:20.000000 iclean-0.0.4/pyproject.toml
+-rw-rw-r--   0 kaliv0    (1000) kaliv0    (1000)       38 2024-05-16 06:23:46.402310 iclean-0.0.4/setup.cfg
```

### Comparing `iclean-0.0.3/LICENSE` & `iclean-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `iclean-0.0.3/PKG-INFO` & `iclean-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: iclean
-Version: 0.0.3
-Summary: Import cleaner
+Version: 0.0.4
+Summary: Unused imports cleaner
 Author: kaliv0
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `iclean-0.0.3/clean.py` & `iclean-0.0.4/clean.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 import logging
 import os
 import re
 from dataclasses import dataclass
 from enum import Enum, auto
 from typing import TextIO
 
-
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 
 # ### constants ###
 @dataclass(frozen=True)
 class Patterns:
     LOG_FORMAT = "%(levelname)s: %(message)s"
     TEMP = "{file}.swap"
@@ -122,15 +121,17 @@
         # load file in memory
         with open(file, "r") as f:
             self.lines = f.readlines()
         self.line_num = -1
         self.import_lines = []
 
     # ### main logic ###
-    def process_paths(self, path_list: list[str], dir_level: str, verbose: bool) -> None:
+    def process_paths(
+        self, path_list: list[str], dir_level: str, verbose: bool
+    ) -> None:
         for path in path_list:
             if path != Tokens.CWD:
                 path = os.path.join(dir_level, path)
 
             if os.path.exists(path) is False:
                 self.logger.warning(Messages.NON_EXISTENT_PATH.format(path=path))
                 continue
@@ -199,19 +200,21 @@
                 self.line_num = i
                 break
 
     def _get_multiline_imports(self, i: int) -> tuple[int, list[str]]:
         imported = []
         i += 1
         while (line := self.lines[i]) != Tokens.RIGHT_PAREN:
-            imported.append(line.strip().rstrip(","))  # FIXME
+            imported.append(line.strip().rstrip(","))
             i += 1
         return i, imported
 
-    def _handle_non_analysed_imports(self, line_literal: str, line_type: ImportLineType) -> None:
+    def _handle_non_analysed_imports(
+        self, line_literal: str, line_type: ImportLineType
+    ) -> None:
         self.import_lines.append(
             ImportLine(
                 literal=line_literal,
                 import_data=[],
                 import_list=[],
                 type=line_type,
             )
@@ -237,15 +240,19 @@
         self._handle_import_line(line_literal, import_list)
 
     def _handle_import_line(self, line_literal: str, import_list: list[str]) -> None:
         import_line = ImportLine(
             literal=line_literal,
             import_data=[],
             import_list=[],
-            type=ImportLineType.MULTI_IMPORT if len(import_list) > 1 else ImportLineType.REGULAR,
+            type=(
+                ImportLineType.MULTI_IMPORT
+                if len(import_list) > 1
+                else ImportLineType.REGULAR
+            ),
         )
         for import_literal in import_list:
             import_data = ImportData(name=import_literal.strip(), count=0)
             import_line.import_data.append(import_data)
         self.import_lines.append(import_line)
 
     def read_rest_of_file(self) -> None:
@@ -288,22 +295,25 @@
         return should_process_line
 
     def _write_import_line(self, file_writer: TextIO, line: ImportLine) -> int:
         if line.import_list or self._should_write_import_line(line):
             if line.type in (ImportLineType.ALIAS, ImportLineType.COMMENT):
                 file_writer.write(line.literal)
             else:
-                file_writer.write(self._prepare_import_line(line.literal, line.import_list))
+                file_writer.write(
+                    self._prepare_import_line(line.literal, line.import_list)
+                )
             return 1  # returns number of written lines
         return 0
 
     @staticmethod
     def _should_write_import_line(line: ImportLine) -> bool:
         return line.type == ImportLineType.COMMENT or not (
-            line.type == ImportLineType.MULTI_IMPORT or line.type == ImportLineType.NEW_LINE
+            line.type == ImportLineType.MULTI_IMPORT
+            or line.type == ImportLineType.NEW_LINE
         )
 
     @staticmethod
     def _prepare_import_line(line_literal: str, import_list: list[str]) -> str:
         return line_literal + f"{Tokens.DELIMITER} ".join(import_list) + Tokens.NEW_LINE
 
     def write_rest_of_file(self, file_writer: TextIO) -> None:
@@ -317,19 +327,25 @@
 
 
 def read_input() -> tuple[list[str], list[str], bool]:
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "target", nargs="+", help="path or list of paths to file or directory to parse"
     )
-    parser.add_argument("--skip", nargs="*", default=(), help="target path or paths to skip")
     parser.add_argument(
-        "--verbose", action="store_true", help="verbose output that includes skipping paths"
+        "--skip", nargs="*", default=(), help="target path or paths to skip"
+    )
+    parser.add_argument(
+        "--verbose",
+        action="store_true",
+        help="verbose output that includes skipping paths",
+    )
+    parser.add_argument(
+        "-v", "--version", action="version", version=f"%(prog)s {__version__}"
     )
-    parser.add_argument("-v", "--version", action="version", version=f"%(prog)s {__version__}")
 
     args = parser.parse_args()
     path_list = args.target
     skip_list = args.skip
     verbose = args.verbose
     return path_list, skip_list, verbose
```

### Comparing `iclean-0.0.3/iclean.egg-info/PKG-INFO` & `iclean-0.0.4/iclean.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: iclean
-Version: 0.0.3
-Summary: Import cleaner
+Version: 0.0.4
+Summary: Unused imports cleaner
 Author: kaliv0
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

