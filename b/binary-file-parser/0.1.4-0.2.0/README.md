# Comparing `tmp/binary_file_parser-0.1.4.tar.gz` & `tmp/binary_file_parser-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binary_file_parser-0.1.4.tar", last modified: Tue May 14 12:27:38 2024, max compression
+gzip compressed data, was "binary_file_parser-0.2.0.tar", last modified: Thu May 16 07:58:28 2024, max compression
```

## Comparing `binary_file_parser-0.1.4.tar` & `binary_file_parser-0.2.0.tar`

### file list

```diff
@@ -1,41 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 12:27:38.032729 binary_file_parser-0.1.4/
--rw-rw-rw-   0        0        0     1084 2022-12-14 12:48:09.000000 binary_file_parser-0.1.4/LICENSE
--rw-rw-rw-   0        0        0        0 2022-12-15 05:10:52.000000 binary_file_parser-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     6028 2024-05-14 12:27:38.029729 binary_file_parser-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     3865 2023-08-26 05:31:53.000000 binary_file_parser-0.1.4/README.md
--rw-rw-rw-   0        0        0      908 2024-05-14 12:15:10.000000 binary_file_parser-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-14 12:27:38.032729 binary_file_parser-0.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-14 12:27:37.922728 binary_file_parser-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2024-05-14 12:27:37.937742 binary_file_parser-0.1.4/src/binary_file_parser/
--rw-rw-rw-   0        0        0      290 2023-05-02 04:00:31.000000 binary_file_parser-0.1.4/src/binary_file_parser/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 12:27:37.963729 binary_file_parser-0.1.4/src/binary_file_parser/errors/
--rw-rw-rw-   0        0        0      118 2022-12-15 18:24:53.000000 binary_file_parser-0.1.4/src/binary_file_parser/errors/CompressionError.py
--rw-rw-rw-   0        0        0      119 2023-08-30 11:43:12.000000 binary_file_parser-0.1.4/src/binary_file_parser/errors/DefaultValueError.py
--rw-rw-rw-   0        0        0       42 2022-12-15 07:13:59.000000 binary_file_parser-0.1.4/src/binary_file_parser/errors/ParsingError.py
--rw-rw-rw-   0        0        0      114 2022-12-15 18:24:20.000000 binary_file_parser-0.1.4/src/binary_file_parser/errors/VersionError.py
--rw-rw-rw-   0        0        0      178 2023-08-30 11:43:12.000000 binary_file_parser-0.1.4/src/binary_file_parser/errors/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 12:27:37.981724 binary_file_parser-0.1.4/src/binary_file_parser/retrievers/
--rw-rw-rw-   0        0        0     2647 2024-05-08 01:30:59.000000 binary_file_parser-0.1.4/src/binary_file_parser/retrievers/MapValidate.py
--rw-rw-rw-   0        0        0     2272 2023-04-24 11:23:48.000000 binary_file_parser-0.1.4/src/binary_file_parser/retrievers/RetreiverCombiner.py
--rw-rw-rw-   0        0        0     1518 2023-04-24 11:16:38.000000 binary_file_parser-0.1.4/src/binary_file_parser/retrievers/RetreiverRef.py
--rw-rw-rw-   0        0        0    12480 2024-05-14 12:10:26.000000 binary_file_parser-0.1.4/src/binary_file_parser/retrievers/Retriever.py
--rw-rw-rw-   0        0        0      199 2023-04-21 01:37:15.000000 binary_file_parser-0.1.4/src/binary_file_parser/retrievers/__init__.py
--rw-rw-rw-   0        0        0    16362 2024-05-13 08:16:58.000000 binary_file_parser-0.1.4/src/binary_file_parser/retrievers/base_struct.py
-drwxrwxrwx   0        0        0        0 2024-05-14 12:27:38.020727 binary_file_parser-0.1.4/src/binary_file_parser/types/
--rw-rw-rw-   0        0        0     6438 2023-04-21 03:06:40.000000 binary_file_parser-0.1.4/src/binary_file_parser/types/Array.py
--rw-rw-rw-   0        0        0      928 2023-04-18 12:21:20.000000 binary_file_parser-0.1.4/src/binary_file_parser/types/Bool.py
--rw-rw-rw-   0        0        0     2796 2022-11-29 16:43:10.000000 binary_file_parser-0.1.4/src/binary_file_parser/types/ByteStream.py
--rw-rw-rw-   0        0        0      855 2023-04-18 12:21:20.000000 binary_file_parser-0.1.4/src/binary_file_parser/types/Bytes.py
--rw-rw-rw-   0        0        0      867 2023-04-18 12:21:20.000000 binary_file_parser-0.1.4/src/binary_file_parser/types/Float.py
--rw-rw-rw-   0        0        0      987 2023-04-18 12:21:20.000000 binary_file_parser-0.1.4/src/binary_file_parser/types/Int.py
--rw-rw-rw-   0        0        0     1345 2023-04-21 02:01:03.000000 binary_file_parser-0.1.4/src/binary_file_parser/types/Parseable.py
--rw-rw-rw-   0        0        0     3274 2024-05-14 11:58:19.000000 binary_file_parser-0.1.4/src/binary_file_parser/types/RefList.py
--rw-rw-rw-   0        0        0     3037 2023-04-18 12:21:20.000000 binary_file_parser-0.1.4/src/binary_file_parser/types/Str.py
--rw-rw-rw-   0        0        0      564 2023-09-09 10:18:09.000000 binary_file_parser-0.1.4/src/binary_file_parser/types/__init__.py
--rw-rw-rw-   0        0        0      894 2024-05-09 12:18:33.000000 binary_file_parser-0.1.4/src/binary_file_parser/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-14 12:27:38.024726 binary_file_parser-0.1.4/src/binary_file_parser.egg-info/
--rw-rw-rw-   0        0        0     6028 2024-05-14 12:27:37.000000 binary_file_parser-0.1.4/src/binary_file_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1260 2024-05-14 12:27:37.000000 binary_file_parser-0.1.4/src/binary_file_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 12:27:37.000000 binary_file_parser-0.1.4/src/binary_file_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2024-05-14 12:27:37.000000 binary_file_parser-0.1.4/src/binary_file_parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-14 12:27:37.000000 binary_file_parser-0.1.4/src/binary_file_parser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 07:58:28.963245 binary_file_parser-0.2.0/
+-rw-rw-rw-   0        0        0     1084 2022-12-14 12:48:09.000000 binary_file_parser-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0        0 2022-12-15 05:10:52.000000 binary_file_parser-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5950 2024-05-16 07:58:28.962268 binary_file_parser-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3787 2024-05-16 07:54:09.000000 binary_file_parser-0.2.0/README.md
+-rw-rw-rw-   0        0        0      908 2024-05-16 07:54:09.000000 binary_file_parser-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-16 07:58:28.963245 binary_file_parser-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-16 07:58:28.906767 binary_file_parser-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-16 07:58:28.916270 binary_file_parser-0.2.0/src/binary_file_parser/
+-rw-rw-rw-   0        0        0      533 2024-05-16 07:54:09.000000 binary_file_parser-0.2.0/src/binary_file_parser/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 07:58:28.931226 binary_file_parser-0.2.0/src/binary_file_parser/errors/
+-rw-rw-rw-   0        0        0      183 2024-05-16 07:54:09.000000 binary_file_parser-0.2.0/src/binary_file_parser/errors/__init__.py
+-rw-rw-rw-   0        0        0      119 2024-05-16 07:54:09.000000 binary_file_parser-0.2.0/src/binary_file_parser/errors/compression_error.py
+-rw-rw-rw-   0        0        0      120 2024-05-16 07:54:09.000000 binary_file_parser-0.2.0/src/binary_file_parser/errors/default_value_error.py
+-rw-rw-rw-   0        0        0       42 2024-05-16 07:54:09.000000 binary_file_parser-0.2.0/src/binary_file_parser/errors/parsing_error.py
+-rw-rw-rw-   0        0        0      115 2024-05-16 07:54:09.000000 binary_file_parser-0.2.0/src/binary_file_parser/errors/version_error.py
+drwxrwxrwx   0        0        0        0 2024-05-16 07:58:28.938223 binary_file_parser-0.2.0/src/binary_file_parser/retrievers/
+-rw-rw-rw-   0        0        0      167 2024-05-16 07:54:09.000000 binary_file_parser-0.2.0/src/binary_file_parser/retrievers/__init__.py
+-rw-rw-rw-   0        0        0     2647 2024-05-16 07:54:09.000000 binary_file_parser-0.2.0/src/binary_file_parser/retrievers/map_validate.py
+-rw-rw-rw-   0        0        0    12781 2024-05-16 07:54:09.000000 binary_file_parser-0.2.0/src/binary_file_parser/retrievers/retriever.py
+-rw-rw-rw-   0        0        0     2271 2024-05-16 07:54:09.000000 binary_file_parser-0.2.0/src/binary_file_parser/retrievers/retriever_combiner.py
+-rw-rw-rw-   0        0        0     1514 2024-05-16 07:54:09.000000 binary_file_parser-0.2.0/src/binary_file_parser/retrievers/retriever_ref.py
+drwxrwxrwx   0        0        0        0 2024-05-16 07:58:28.947224 binary_file_parser-0.2.0/src/binary_file_parser/types/
+-rw-rw-rw-   0        0        0      192 2024-05-16 07:54:09.000000 binary_file_parser-0.2.0/src/binary_file_parser/types/__init__.py
+-rw-rw-rw-   0        0        0    15924 2024-05-16 07:54:09.000000 binary_file_parser-0.2.0/src/binary_file_parser/types/base_struct.py
+-rw-rw-rw-   0        0        0     2796 2024-05-16 07:54:09.000000 binary_file_parser-0.2.0/src/binary_file_parser/types/byte_stream.py
+drwxrwxrwx   0        0        0        0 2024-05-16 07:58:28.958224 binary_file_parser-0.2.0/src/binary_file_parser/types/le/
+-rw-rw-rw-   0        0        0      471 2024-05-16 07:54:09.000000 binary_file_parser-0.2.0/src/binary_file_parser/types/le/__init__.py
+-rw-rw-rw-   0        0        0     6186 2024-05-16 07:54:09.000000 binary_file_parser-0.2.0/src/binary_file_parser/types/le/array.py
+-rw-rw-rw-   0        0        0      939 2024-05-16 07:54:09.000000 binary_file_parser-0.2.0/src/binary_file_parser/types/le/bool.py
+-rw-rw-rw-   0        0        0      864 2024-05-16 07:54:09.000000 binary_file_parser-0.2.0/src/binary_file_parser/types/le/bytes.py
+-rw-rw-rw-   0        0        0      879 2024-05-16 07:54:09.000000 binary_file_parser-0.2.0/src/binary_file_parser/types/le/float.py
+-rw-rw-rw-   0        0        0      996 2024-05-16 07:54:09.000000 binary_file_parser-0.2.0/src/binary_file_parser/types/le/int.py
+-rw-rw-rw-   0        0        0     3046 2024-05-16 07:54:09.000000 binary_file_parser-0.2.0/src/binary_file_parser/types/le/string.py
+-rw-rw-rw-   0        0        0      645 2024-05-16 07:54:09.000000 binary_file_parser-0.2.0/src/binary_file_parser/types/parseable.py
+-rw-rw-rw-   0        0        0     3445 2024-05-16 07:54:09.000000 binary_file_parser-0.2.0/src/binary_file_parser/types/ref_list.py
+-rw-rw-rw-   0        0        0      784 2024-05-16 07:54:09.000000 binary_file_parser-0.2.0/src/binary_file_parser/types/version.py
+-rw-rw-rw-   0        0        0      108 2024-05-16 07:54:09.000000 binary_file_parser-0.2.0/src/binary_file_parser/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-16 07:58:28.960224 binary_file_parser-0.2.0/src/binary_file_parser.egg-info/
+-rw-rw-rw-   0        0        0     5950 2024-05-16 07:58:28.000000 binary_file_parser-0.2.0/src/binary_file_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1370 2024-05-16 07:58:28.000000 binary_file_parser-0.2.0/src/binary_file_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 07:58:28.000000 binary_file_parser-0.2.0/src/binary_file_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2024-05-16 07:58:28.000000 binary_file_parser-0.2.0/src/binary_file_parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-16 07:58:28.000000 binary_file_parser-0.2.0/src/binary_file_parser.egg-info/top_level.txt
```

### Comparing `binary_file_parser-0.1.4/LICENSE` & `binary_file_parser-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `binary_file_parser-0.1.4/PKG-INFO` & `binary_file_parser-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binary-file-parser
-Version: 0.1.4
+Version: 0.2.0
 Summary: Read/Write binary files after describing their specifications in code (similar to an ORM table schema)
 Author-email: Divy1211 <divy1211.dc@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Alian713
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -65,19 +65,19 @@
 
 ## Getting Started
 
 This is a very basic script to give you an idea of how to use this library. Check out the API Reference (coming soon™) for documentation containing more details on how to use this library.
 
 ```py
 from binary_file_parser import BaseStruct, Retriever
-from binary_file_parser.types import uint32, uint64, str32, FixedLenStr
+from binary_file_parser.types import int32, uint64, str32, FixedLenStr
 
 class Spam(BaseStruct):
-    file_version: str = Retriever(FixedLenStr[4], default = 0)
-    creator_name: str = Retriever(str32, default = 0)
+    file_version: str = Retriever(FixedLenStr[4], default = "1.00")
+    creator_name: str = Retriever(str32, default = "bfp")
     saved_timestamp: int = Retriever(uint64, default = 0)
     eggs: int = Retriever(int32, default = 0)
 
 # read a binary file that has the above format
 file = Spam.from_file("path/to/file")
 
 # modify the creator name
@@ -94,15 +94,15 @@
 1. You can use your own structs within another struct
 2. Event hooks help you keep any interdependencies in the file structure synchronised:
 
 ```py
 from __future__ import annotations
 
 from binary_file_parser import BaseStruct, Retriever
-from binary_file_parser.types import FixedLenArray, uint8
+from binary_file_parser.types import FixedLenArray, uint32, uint8
 
 
 class Pixel(BaseStruct):
     red: int = Retriever(uint8, default = 0)
     green: int = Retriever(uint8, default = 0)
     blue: int = Retriever(uint8, default = 0)
     alpha: int = Retriever(uint8, default = 0)
@@ -116,14 +116,15 @@
     ):
         super().__init__(initialise_defaults = False)
         self.red = red
         self.green = green
         self.blue = blue
         self.alpha = alpha
 
+
 class Img(BaseStruct):
     @staticmethod
     def _set_width(retriever: Retriever, obj: Img):
         # here Img.pixels.dtype refers to FixedLenArray
         Img.pixels.dtype.length = obj._width
 
     @staticmethod
@@ -133,33 +134,33 @@
 
     @staticmethod
     def _update_dims(retriever: Retriever, obj: Img):
         # this ensures that when the file is written back, the height and width being written back to file are
         # up to date
         obj._height = obj.height
         Img.pixels.dtype.length = obj._width = obj.width
-    
+
     _width: int = Retriever(uint32, default = 100, on_read = [_set_width], on_write = [_update_dims])
     _height: int = Retriever(uint32, default = 200, on_set = [_set_height])
     pixels: list[list[Pixel]] = Retriever(
-        FixedLenArray[Pixel, 100], default = [Pixel(0, 0, 0) for _ in range(100)], repeat = 200
+        FixedLenArray[Pixel, 100], default_factory = lambda _, __: [Pixel(0, 0, 0) for _ in range(100)], repeat = 200
     )
 
     @property
     def width(self) -> int:
         return len(self.pixels[0])
 
     @property
     def height(self) -> int:
         return len(self.pixels)
 
+
 # Make a new image from all defaults
 a = Img()
-# Note: Mutable defaults will be shallow copied, (this means all rows of pixels in the above example are the same!)
-# If you have larger structs or nested structs, use default_factory (coming soon:tm:) instead
+# Note: Mutable defaults will be shallow copied, use default_factory when such is not intended
 ```
 
 ## About the Author
 
 If you have any questions, suggestions or feedback regarding the library, feel free to send me a message on discord!
 
 | Author   | Discord       |
```

### Comparing `binary_file_parser-0.1.4/README.md` & `binary_file_parser-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -20,19 +20,19 @@
 
 ## Getting Started
 
 This is a very basic script to give you an idea of how to use this library. Check out the API Reference (coming soon™) for documentation containing more details on how to use this library.
 
 ```py
 from binary_file_parser import BaseStruct, Retriever
-from binary_file_parser.types import uint32, uint64, str32, FixedLenStr
+from binary_file_parser.types import int32, uint64, str32, FixedLenStr
 
 class Spam(BaseStruct):
-    file_version: str = Retriever(FixedLenStr[4], default = 0)
-    creator_name: str = Retriever(str32, default = 0)
+    file_version: str = Retriever(FixedLenStr[4], default = "1.00")
+    creator_name: str = Retriever(str32, default = "bfp")
     saved_timestamp: int = Retriever(uint64, default = 0)
     eggs: int = Retriever(int32, default = 0)
 
 # read a binary file that has the above format
 file = Spam.from_file("path/to/file")
 
 # modify the creator name
@@ -49,15 +49,15 @@
 1. You can use your own structs within another struct
 2. Event hooks help you keep any interdependencies in the file structure synchronised:
 
 ```py
 from __future__ import annotations
 
 from binary_file_parser import BaseStruct, Retriever
-from binary_file_parser.types import FixedLenArray, uint8
+from binary_file_parser.types import FixedLenArray, uint32, uint8
 
 
 class Pixel(BaseStruct):
     red: int = Retriever(uint8, default = 0)
     green: int = Retriever(uint8, default = 0)
     blue: int = Retriever(uint8, default = 0)
     alpha: int = Retriever(uint8, default = 0)
@@ -71,14 +71,15 @@
     ):
         super().__init__(initialise_defaults = False)
         self.red = red
         self.green = green
         self.blue = blue
         self.alpha = alpha
 
+
 class Img(BaseStruct):
     @staticmethod
     def _set_width(retriever: Retriever, obj: Img):
         # here Img.pixels.dtype refers to FixedLenArray
         Img.pixels.dtype.length = obj._width
 
     @staticmethod
@@ -88,33 +89,33 @@
 
     @staticmethod
     def _update_dims(retriever: Retriever, obj: Img):
         # this ensures that when the file is written back, the height and width being written back to file are
         # up to date
         obj._height = obj.height
         Img.pixels.dtype.length = obj._width = obj.width
-    
+
     _width: int = Retriever(uint32, default = 100, on_read = [_set_width], on_write = [_update_dims])
     _height: int = Retriever(uint32, default = 200, on_set = [_set_height])
     pixels: list[list[Pixel]] = Retriever(
-        FixedLenArray[Pixel, 100], default = [Pixel(0, 0, 0) for _ in range(100)], repeat = 200
+        FixedLenArray[Pixel, 100], default_factory = lambda _, __: [Pixel(0, 0, 0) for _ in range(100)], repeat = 200
     )
 
     @property
     def width(self) -> int:
         return len(self.pixels[0])
 
     @property
     def height(self) -> int:
         return len(self.pixels)
 
+
 # Make a new image from all defaults
 a = Img()
-# Note: Mutable defaults will be shallow copied, (this means all rows of pixels in the above example are the same!)
-# If you have larger structs or nested structs, use default_factory (coming soon:tm:) instead
+# Note: Mutable defaults will be shallow copied, use default_factory when such is not intended
 ```
 
 ## About the Author
 
 If you have any questions, suggestions or feedback regarding the library, feel free to send me a message on discord!
 
 | Author   | Discord       |
```

### Comparing `binary_file_parser-0.1.4/pyproject.toml` & `binary_file_parser-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=57.4.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "binary-file-parser"
-version = "0.1.4"
+version = "0.2.0"
 description = "Read/Write binary files after describing their specifications in code (similar to an ORM table schema)"
 readme = "README.md"
 authors = [{ name = "Divy1211", email = "divy1211.dc@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `binary_file_parser-0.1.4/src/binary_file_parser/retrievers/MapValidate.py` & `binary_file_parser-0.2.0/src/binary_file_parser/retrievers/map_validate.py`

 * *Files identical despite different names*

### Comparing `binary_file_parser-0.1.4/src/binary_file_parser/retrievers/RetreiverCombiner.py` & `binary_file_parser-0.2.0/src/binary_file_parser/retrievers/retriever_combiner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from __future__ import annotations
 
 from contextlib import suppress
-from typing import Type, TypeVar, Generic
+from typing import Generic, Type, TypeVar
 
-from binary_file_parser.utils import Version
 from binary_file_parser.errors import VersionError
-
-from binary_file_parser.retrievers.base_struct import BaseStruct
-from binary_file_parser.retrievers.Retriever import Retriever
-
+from binary_file_parser.retrievers.retriever import Retriever
+from binary_file_parser.types.base_struct import BaseStruct
+from binary_file_parser.types.version import Version
 
 T = TypeVar("T")
 
 
 class RetrieverCombiner(Generic[T]):
     """
     Creates a single attribute to access values from multiple retrievers which are mutually exclusive among different
```

### Comparing `binary_file_parser-0.1.4/src/binary_file_parser/retrievers/RetreiverRef.py` & `binary_file_parser-0.2.0/src/binary_file_parser/retrievers/retriever_ref.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 from contextlib import suppress
 from typing import Type, TypeVar, Generic
 
 from binary_file_parser.errors import VersionError
 
-from binary_file_parser.retrievers.base_struct import BaseStruct
-from binary_file_parser.retrievers.Retriever import Retriever
-from binary_file_parser.retrievers.RetreiverCombiner import RetrieverCombiner
+from binary_file_parser.types.base_struct import BaseStruct
+from binary_file_parser.retrievers.retriever import Retriever
+from binary_file_parser.retrievers.retriever_combiner import RetrieverCombiner
 
 
 T = TypeVar("T")
 
 
 class RetrieverRef(Generic[T]):
     """
```

### Comparing `binary_file_parser-0.1.4/src/binary_file_parser/retrievers/Retriever.py` & `binary_file_parser-0.2.0/src/binary_file_parser/retrievers/retriever.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,41 @@
 from __future__ import annotations
 
 import sys
 from io import BytesIO
-from typing import Any, Type, Callable, TypeVar
+from typing import Any, Callable, Type, TypeVar
 
-from binary_file_parser.errors import VersionError, DefaultValueError
-from binary_file_parser.types import ByteStream
-from binary_file_parser.types import Parseable
-
-from binary_file_parser.retrievers.MapValidate import MapValidate
-from binary_file_parser.retrievers.base_struct import BaseStruct
-from binary_file_parser.types.RefList import RefList
-from binary_file_parser.utils import Version
+from binary_file_parser.errors import DefaultValueError, VersionError
+from binary_file_parser.types import BaseStruct, ByteStream, Parseable, Version
+from binary_file_parser.retrievers.map_validate import MapValidate
 
 T = TypeVar("T")
 RetrieverSub = TypeVar("RetrieverSub", bound = "Retriever")
 BaseStructSub = TypeVar("BaseStructSub", bound = BaseStruct)
 
 
 class Retriever(MapValidate):
     """
     Represents a binary object in a struct and the restrictions/dependencies associated with it
     """
     __slots__ = (
-        "atype", "dtype", "min_ver", "max_ver", "default", "default_factory",
+        "dtype", "min_ver", "max_ver", "default", "default_factory",
         "_repeat", "remaining_compressed", "on_read", "on_write"
     )
 
     def __init__(
         self,
         dtype: Parseable | Type[Parseable],
         min_ver: Version = Version((-1,)),
         max_ver: Version = Version((sys.maxsize,)),
         *,
         default = None,
         default_factory: Callable[[Version, BaseStruct], Any] = None,
         repeat: int = 1,
-        atype: Type[RefList] = RefList,
+        # atype: Type[RefList] = RefList,
         remaining_compressed: bool = False,
         on_read: list[Callable[[RetrieverSub, BaseStructSub], None]] | None = None,  # todo: add implementations for common on_x operations
         on_write: list[Callable[[RetrieverSub, BaseStructSub], None]] | None = None,
         mappers: list[Callable[[RetrieverSub, BaseStructSub, T], T]] | None = None,
         validators: list[Callable[[RetrieverSub, BaseStructSub, T], tuple[bool, str]]] | None = None,
         on_get: list[Callable[[RetrieverSub, BaseStructSub], None]] | None = None,
         on_set: list[Callable[[RetrieverSub, BaseStructSub], None]] | None = None,
@@ -79,15 +74,15 @@
         :param on_get: A list of functions that are called when this retriever property is accessed
         :param on_set: A list of functions that are called when this retriever property is set
 
         :raises DefaultValueError: If a mutable type is used for providing default values instead of default_factory
         """
         super().__init__(mappers, validators, on_get, on_set)
         self.dtype = dtype
-        self.atype = atype
+        # self.atype = atype
         self.min_ver = min_ver
         self.max_ver = max_ver
 
         if (
             isinstance(default, list)
             or default is not None
             and isinstance(default, BaseStruct)
@@ -136,19 +131,30 @@
 
     def __set__(self, instance: BaseStruct, value: T) -> None:
         if not self.supported(instance.struct_ver):
             raise VersionError(
                 f"{self.p_name!r} is not supported in your scenario version {instance.struct_ver}"
             )
 
-        if not isinstance(value, list):
-            super().__set__(instance, value)
-            return
+        # if not isinstance(value, list):
+        #     super().__set__(instance, value)
+        #     return
+        #
+        # if not isinstance(value, RefList):
+        #     value = self.atype(value, instance.struct_ver, instance.parent)
+        #
+        # if len(value) == 0:
+        #     super().__set__(instance, value)
+        #     return
+        #
+        # if id(getattr(value[0], "parent", instance.parent)) != id(instance.parent):
+        #     value.parent = instance.parent
+        # if getattr(value[0], "struct_ver", instance.struct_ver) != instance.struct_ver:
+        #     value.struct_ver = instance.struct_ver
 
-        value = self.atype(value, instance.struct_ver, instance.parent)
         super().__set__(instance, value)
 
     def __get__(self, instance: BaseStruct, owner: Type[BaseStruct]) -> Retriever | T:
         if instance is None:
             return self
 
         if not self.supported(instance.struct_ver):
@@ -195,37 +201,40 @@
         repeat = self.repeat(instance)
         if repeat == -1:
             return None
 
         if self.default is not None:
             if repeat == 1:
                 return self.default
-            return self.atype(
-                [self.default]*repeat,
-                instance.struct_ver, instance
-            )
+            return [self.default]*repeat
+
+            # return self.atype(
+            #     [self.default]*repeat,
+            #     instance.struct_ver, instance
+            # )
 
         if self.default_factory is not None:
             if repeat == 1:
                 val = self.default_factory(instance.struct_ver, instance)
-                if isinstance(val, list):
-                    return self.atype(val, instance.struct_ver, instance)
+                # if isinstance(val, list):
+                #     return self.atype(val, instance.struct_ver, instance)
                 return val
-            return self.atype(
-                (self.default_factory(instance.struct_ver, instance) for _ in range(repeat)),
-                instance.struct_ver, instance
-            )
-
-        if self.dtype.is_struct:
-            if repeat == 1:
-                return self.dtype(struct_ver = instance.struct_ver, parent = instance).map()
-            return self.atype(
-                (self.dtype(struct_ver = instance.struct_ver, parent = instance).map() for _ in range(repeat)),
-                instance.struct_ver, instance
-            )
+            return [self.default_factory(instance.struct_ver, instance) for _ in range(repeat)]
+            # return self.atype(
+            #     (self.default_factory(instance.struct_ver, instance) for _ in range(repeat)),
+            #     instance.struct_ver, instance
+            # )
+
+        # if self.dtype.is_struct:
+        #     if repeat == 1:
+        #         return self.dtype(struct_ver = instance.struct_ver, parent = instance).map()
+        #     return self.atype(
+        #         (self.dtype(struct_ver = instance.struct_ver, parent = instance).map() for _ in range(repeat)),
+        #         instance.struct_ver, instance
+        #     )
 
         raise DefaultValueError(
             f"Unable to auto-initialise '{self.p_name}' as a default value is not provided"
         )
 
     def from_stream(self, instance: BaseStruct, stream: ByteStream) -> None:
         """
@@ -239,28 +248,26 @@
 
         repeat = self.repeat(instance)
         if repeat == -1:
             setattr(instance, self.p_name, None)
             return
 
         def getobj():
-            if self.dtype.is_struct:
-                self.dtype: BaseStruct  # type: ignore
-                return self.dtype.from_stream(stream, struct_ver = instance.struct_ver, parent = instance)
             return self.dtype.from_stream(stream, struct_ver = instance.struct_ver)
 
         is_not_dynamic_repeat = not hasattr(instance, self.r_name)
         if repeat == 1 and is_not_dynamic_repeat:
             setattr(instance, self.p_name, getobj())
             return
 
         ls: list = [None] * repeat
         for i in range(repeat):
             ls[i] = getobj()
-        setattr(instance, self.p_name, self.atype(ls, instance.struct_ver, instance))
+        # setattr(instance, self.p_name, self.atype(ls, instance.struct_ver, instance))
+        setattr(instance, self.p_name, ls)
 
         for func in self.on_read:
             func(self, instance)
 
     def to_bytes(self, instance: BaseStruct) -> bytes:
         """
         Convert this retriever property to bytes
```

### Comparing `binary_file_parser-0.1.4/src/binary_file_parser/retrievers/base_struct.py` & `binary_file_parser-0.2.0/src/binary_file_parser/types/base_struct.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 from __future__ import annotations
 
 import copy
-from io import StringIO
 from contextlib import suppress
+from io import StringIO
 from typing import TYPE_CHECKING
 
 from alive_progress import alive_it
 
-from binary_file_parser.errors import CompressionError
-from binary_file_parser.errors import ParsingError
-from binary_file_parser.errors import VersionError
-from binary_file_parser.types import ByteStream, RefList
-from binary_file_parser.types import Parseable
-from binary_file_parser.utils import indentify, Version
+from binary_file_parser.errors import CompressionError, ParsingError, VersionError
+from binary_file_parser.types.parseable import Parseable
+from binary_file_parser.types.byte_stream import ByteStream
+# from binary_file_parser.types.ref_list import RefList
+from binary_file_parser.types.version import Version
+from binary_file_parser.utils import indentify
 
 if TYPE_CHECKING:
-    from binary_file_parser.retrievers.Retriever import Retriever
-    from binary_file_parser.retrievers.RetreiverCombiner import RetrieverCombiner
-    from binary_file_parser.retrievers.RetreiverRef import RetrieverRef
+    from binary_file_parser.retrievers import Retriever, RetrieverCombiner, RetrieverRef
 
 
 class BaseStruct(Parseable):
     """
     Base class for defining a file format as a structure
     """
-    __slots__ = "_struct_ver", "_parent", "idx"
+    __slots__ = "_struct_ver", "idx"
 
     _retrievers: list[Retriever] = []
     _refs: list[RetrieverRef] = []
     _combiners: list[RetrieverCombiner] = []
 
     @classmethod
     def _add_retriever(cls, retriever: Retriever):
@@ -38,35 +36,24 @@
     def _add_ref(cls, ref: RetrieverRef):
         cls._refs.append(ref)
 
     @classmethod
     def _add_combiner(cls, combiner: RetrieverCombiner):
         cls._combiners.append(combiner)
 
-    def __init__(
-        self,
-        struct_ver: Version = Version((0,)),
-        parent: BaseStruct = None,
-        idx: int = -1,
-        initialise_defaults: bool = True,
-        **retriever_inits,
-    ):
+    def __init__(self, struct_ver: Version = Version((0,)), initialise_defaults: bool = True, **retriever_inits):
         """
-        :param idx:
         :param struct_ver: The struct version to create
-        :param parent: If this struct is nested within another, define the containing struct as parent
         :param initialise_defaults:
             If set to false, skip initialisation of struct values from default. This is only set to false when reading
             a file
         :param retriever_inits:
             Use this to provide initial values to retrievers
         """
         self._struct_ver = struct_ver
-        self._parent = parent
-        self.idx = idx
 
         size = 0
         if not initialise_defaults:
             super().__init__(size)
             return
 
         for retriever in self._retrievers:
@@ -91,35 +78,32 @@
 
     def __deepcopy__(self, memo):
         cls = self.__class__
         cloned_struct = cls.__new__(cls)
         memo[id(self)] = cloned_struct
 
         for attr in list(self.__slots__) + list(self.__dict__):
-            if attr == '_parent':
-                value = None
-            else:
-                value = copy.deepcopy(getattr(self, attr), memo)
+            value = copy.deepcopy(getattr(self, attr), memo)
             setattr(cloned_struct, attr, value)
 
         return cloned_struct
 
     @property
     def is_struct(self) -> bool:
         return True
 
-    @property
-    def root(self) -> BaseStruct:
-        """
-        The top level object of which this struct is a part of
-        """
-        child = self
-        while child.parent is not None:
-            child = self.parent
-        return child
+    # @property
+    # def root(self) -> BaseStruct:
+    #     """
+    #     The top level object of which this struct is a part of
+    #     """
+    #     child = self
+    #     while child.parent is not None:
+    #         child = self.parent
+    #     return child
 
     def on_struct_ver_change(self, new_struct_ver: Version):
         """
         This method is called when a struct's version is changed. Use this to implement any custom logic required to
         support a version change on a struct. The default method implements a trial and error algorithm where if an
         unsupported retriever after the version change used to have the same value as its default, then it is discarded
         without any errors, However, if a value other than the default was assigned to it, an error is raised
@@ -127,57 +111,65 @@
         :param new_struct_ver: The new struct version (the self.struct_ver attribute will automatically be updated)
 
         :raises VersionError: When the version change causes a non default valued retriever to become unsupported
         """
         pass
 
     @property
-    def struct_ver(self):
+    def struct_ver(self) -> Version:
         return self._struct_ver
 
-    @struct_ver.setter
-    def struct_ver(self, new_struct_ver: Version):
-        for retriever in self._retrievers:
-            if (
-                not retriever.supported(self.struct_ver)
-                or not (retriever.dtype.is_struct or retriever.dtype.is_iterable)
-                or retriever.is_self_versioned
-            ):
-                continue
-            if (obj := getattr(self, retriever.p_name)) is not None:
-                obj.struct_ver = new_struct_ver
-        self.on_struct_ver_change(new_struct_ver)
-        self._struct_ver = new_struct_ver
-
-    @property
-    def parent(self):
-        return self._parent
-
-    @parent.setter
-    def parent(self, new_parent: BaseStruct):
-        for retriever in self._retrievers:
-            if (
-                not retriever.supported(self.struct_ver)
-                or not (retriever.dtype.is_struct or retriever.dtype.is_iterable)
-            ):
-                continue
-            if (obj := getattr(self, retriever.p_name)) is not None:
-                obj.parent = new_parent
-        self._parent = new_parent
+    # @struct_ver.setter
+    # def struct_ver(self, value: Version):
+    #     self._struct_ver = value
+
+    # @property
+    # def struct_ver(self):
+    #     return self._struct_ver
+    #
+    # @struct_ver.setter
+    # def struct_ver(self, new_struct_ver: Version):
+    #     for retriever in self._retrievers:
+    #         if (
+    #             not retriever.supported(self.struct_ver)
+    #             or not (retriever.dtype.is_struct or retriever.dtype.is_iterable)
+    #             or retriever.is_self_versioned
+    #         ):
+    #             continue
+    #         if (obj := getattr(self, retriever.p_name)) is not None:
+    #             obj.struct_ver = new_struct_ver
+    #     self.on_struct_ver_change(new_struct_ver)
+    #     self._struct_ver = new_struct_ver
+    #
+    # @property
+    # def parent(self):
+    #     return self._parent
+    #
+    # @parent.setter
+    # def parent(self, new_parent: BaseStruct):
+    #     for retriever in self._retrievers:
+    #         if (
+    #             not retriever.supported(self.struct_ver)
+    #             or not (retriever.dtype.is_struct or retriever.dtype.is_iterable)
+    #         ):
+    #             continue
+    #         if (obj := getattr(self, retriever.p_name)) is not None:
+    #             obj.parent = new_parent
+    #     self._parent = new_parent
 
     @property
     def retriever_name_value_map(self) -> dict[str]:
         map_ = {}
         for retriever in self._retrievers:
             if retriever.supported(self.struct_ver):
                 map_[retriever.p_name] = getattr(self, retriever.p_name)
         return map_
 
     @classmethod
-    def get_version(cls, stream: ByteStream, struct_ver: Version = Version((0,)), parent: BaseStruct = None) -> Version:
+    def get_version(cls, stream: ByteStream, struct_ver: Version = Version((0,))) -> Version:
         """
         If defined, the struct will be versioned and values in the struct which are not supported in the version that is
         read will be skipped
 
         :param stream: The stream to read the struct version from
         :param struct_ver: The struct version of the parent
         :param parent:
@@ -223,30 +215,29 @@
         :return: A BaseStruct instance
         """
         return self
 
     @classmethod
     def from_stream(
         cls, stream: ByteStream, *, struct_ver: Version = Version((0,)), strict: bool = False,
-        show_progress: bool = False, parent: BaseStruct = None
+        show_progress: bool = False
     ) -> BaseStruct:
         """
         Create a struct object from a ByteStream
 
         :param stream: The stream to create the struct object from
         :param struct_ver: The version of the structure to create. Overwritten if `get_version` is defined
         :param strict: Raise an error if struct parsing finishes successfully but the stream has left over bytes
         :param show_progress: When true, display a progress bar
-        :param parent: If this struct is nested within another, define the containing struct as parent
         :return: An instance of a subtype of BaseStruct
         """
         with suppress(VersionError):
-            struct_ver = cls.get_version(stream, struct_ver, parent)
+            struct_ver = cls.get_version(stream, struct_ver)
 
-        instance = cls(struct_ver = struct_ver, parent = parent, initialise_defaults = False)
+        instance = cls(struct_ver = struct_ver, initialise_defaults = False)
         retriever_ls = cls._retrievers
         if show_progress:
             retriever_ls = alive_it(
                 retriever_ls,
                 dual_line = True,
                 title = "         Reading File",
                 stats = False,
@@ -364,15 +355,15 @@
 
         diff_retrievers: list[Retriever] = []
         for retriever in self._retrievers:
             if not retriever.supported(self.struct_ver):
                 continue
             if (val1 := getattr(self, retriever.p_name)) == (val2 := getattr(other, retriever.p_name)):
                 continue
-            if retriever.dtype.is_struct and not isinstance(val1, RefList): # todo: implement a diff on reflists
+            if isinstance(val1, BaseStruct):
                 diff_retrievers.extend(val1.diff(val2))
             else:
                 diff_retrievers.append(retriever)
         return diff_retrievers
 
     def __repr__(self) -> str:
         repr_builder = StringIO()
```

### Comparing `binary_file_parser-0.1.4/src/binary_file_parser/types/Array.py` & `binary_file_parser-0.2.0/src/binary_file_parser/types/le/array.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,33 @@
 from __future__ import annotations
 
 import struct
-from typing import Type
+from typing import Type, TYPE_CHECKING
 
-from binary_file_parser.types.ByteStream import ByteStream
-from binary_file_parser.types.Parseable import Parseable
-from binary_file_parser.types.RefList import RefList
-from binary_file_parser.utils import Version
+from binary_file_parser.types.parseable import Parseable
+from binary_file_parser.types.version import Version
+from binary_file_parser.types.byte_stream import ByteStream
 
-ParseableType = Type[Parseable] | Parseable
+if TYPE_CHECKING:
+    ParseableType = Type[Parseable] | Parseable
 
 class BaseArray(Parseable):
-    __slots__ = ("atype", "dtype", "struct_symbol", "length")
+    __slots__ = ("dtype", "struct_symbol", "length")
 
-    @property
-    def is_iterable(self) -> bool:
-        return True
-
-    def __init__(self, size: int, dtype: ParseableType, struct_symbol: str, atype: Type[RefList] = RefList):
+    def __init__(self, size: int, dtype: ParseableType, struct_symbol: str):
         super().__init__(size)
         self.dtype = dtype
-        self.atype = atype
         self.struct_symbol = struct_symbol
         self.length = -1
 
     def from_stream(self, stream: ByteStream, *, struct_ver: Version = Version((0,))) -> list:
         ls = [None] * self.length
         for i in range(self.length):
             ls[i] = self.dtype.from_stream(stream, struct_ver = struct_ver)
-        return self.atype(ls)
+        return ls
 
     def from_bytes(self, bytes_: bytes, *, struct_ver: Version = Version((0,))) -> list:
         return self.from_stream(ByteStream.from_bytes(bytes_), struct_ver = struct_ver)
 
     def to_bytes(self, value: list) -> bytes:
         ls = [b""]*self.length
         for i, val in enumerate(value):
@@ -76,16 +71,16 @@
     def __class_getitem__(cls, item: ParseableType) -> Array64:
         return cls(8, item, '<Q')
 
 
 class FixedLenArray(BaseArray):
     __slots__ = ()
 
-    def __init__(self, size: int, dtype: ParseableType, struct_symbol: str, length: int, atype: Type[RefList] = RefList):
-        super().__init__(size, dtype, struct_symbol, atype)
+    def __init__(self, size: int, dtype: ParseableType, struct_symbol: str, length: int):
+        super().__init__(size, dtype, struct_symbol)
         self.length = length
 
     def is_valid(self, value: list) -> tuple[bool, str]:
         if len(value) == self.length:
             return True, ""
         return False, f"%s must have a fixed length of {value}"
 
@@ -98,16 +93,16 @@
     def __class_getitem__(cls, item: tuple[ParseableType, int]) -> FixedLenArray:
         return cls(4, item[0], '<I', item[1])
 
 
 class StackedArrays(BaseArray):
     __slots__ = "num_arrays"
 
-    def __init__(self, size: int, dtype: ParseableType, struct_symbol: str, num_arrays: int = -1, atype: Type[RefList] = RefList):
-        super().__init__(size, dtype, struct_symbol, atype)
+    def __init__(self, size: int, dtype: ParseableType, struct_symbol: str, num_arrays: int = -1):
+        super().__init__(size, dtype, struct_symbol)
         self.num_arrays = num_arrays
 
     def is_valid(self, value: list[list]) -> tuple[bool, str]:
         if self.num_arrays == -1:
             return True, ""
 
         num_arrays = len(value)
@@ -123,15 +118,15 @@
         lengths: list[int] = [struct.unpack(self.struct_symbol, stream.get(self.size))[0] for _ in range(num_arrays)]
         ls: list[list] = [[] for _ in range(num_arrays)]
 
         for i, length in enumerate(lengths):
             self.length = length
             ls[i] = super().from_stream(stream, struct_ver = struct_ver)
 
-        return self.atype(ls)
+        return ls
 
     def to_bytes(self, value: list[list]) -> bytes:
         valid, msg = self.is_valid(value)
         if not valid:
             raise TypeError(msg)
 
         length_bytes = b""
```

### Comparing `binary_file_parser-0.1.4/src/binary_file_parser/types/Bool.py` & `binary_file_parser-0.2.0/src/binary_file_parser/types/le/int.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 import struct
 
-from binary_file_parser.types.ByteStream import ByteStream
-from binary_file_parser.types.Parseable import Parseable
-from binary_file_parser.utils import Version
+from binary_file_parser.types.parseable import Parseable
+from binary_file_parser.types.byte_stream import ByteStream
+from binary_file_parser.types.version import Version
 
 
-class Bool(Parseable):
+class Int(Parseable):
     __slots__ = "struct_symbol"
 
     def __init__(self, size: int, struct_symbol: str):
         super().__init__(size)
         self.struct_symbol = struct_symbol
 
-    def from_stream(self, stream: ByteStream, *, struct_ver: Version = Version((0,))) -> bool:
+    def from_stream(self, stream: ByteStream, *, struct_ver: Version = Version((0,))) -> int:
         return self.from_bytes(stream.get(self.size), struct_ver = struct_ver)
 
-    def from_bytes(self, bytes_: bytes, *, struct_ver: Version = Version((0,))) -> bool:
-        return not not struct.unpack(self.struct_symbol, bytes_)[0]
+    def from_bytes(self, bytes_: bytes, *, struct_ver: Version = Version((0,))) -> int:
+        return struct.unpack(self.struct_symbol, bytes_)[0]
 
-    def to_bytes(self, value: bool) -> bytes:
-        return struct.pack(self.struct_symbol, 1 if value else 0)
+    def to_bytes(self, value: int) -> bytes:
+        return struct.pack(self.struct_symbol, value)
 
-bool8 = Bool(1, "<B")
-bool16 = Bool(2, "<H")
-bool32 = Bool(4, "<I")
-bool64 = Bool(8, "<Q")
+int8 = Int(1, "<b")
+int16 = Int(2, "<h")
+int32 = Int(4, "<i")
+int64 = Int(8, "<q")
+uint8 = Int(1, "<B")
+uint16 = Int(2, "<H")
+uint32 = Int(4, "<I")
+uint64 = Int(8, "<Q")
```

### Comparing `binary_file_parser-0.1.4/src/binary_file_parser/types/ByteStream.py` & `binary_file_parser-0.2.0/src/binary_file_parser/types/byte_stream.py`

 * *Files identical despite different names*

### Comparing `binary_file_parser-0.1.4/src/binary_file_parser/types/Bytes.py` & `binary_file_parser-0.2.0/src/binary_file_parser/types/le/bool.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-from __future__ import annotations
+import struct
 
-from binary_file_parser.types.ByteStream import ByteStream
-from binary_file_parser.types.Parseable import Parseable
-from binary_file_parser.utils import Version
+from binary_file_parser.types.byte_stream import ByteStream
+from binary_file_parser.types.parseable import Parseable
+from binary_file_parser.types.version import Version
 
 
-class Bytes(Parseable):
-    __slots__ = ()
+class Bool(Parseable):
+    __slots__ = "struct_symbol"
 
-    def is_valid(self, value: bytes) -> tuple[bool, str]:
-        if len(value) == self.size:
-            return True, ""
-        return False, f"number of bytes in %s must equal {self.size}"
+    def __init__(self, size: int, struct_symbol: str):
+        super().__init__(size)
+        self.struct_symbol = struct_symbol
 
-    def from_stream(self, stream: ByteStream, *, struct_ver: Version = Version((0,))) -> bytes:
-        return stream.get(self.size)
+    def from_stream(self, stream: ByteStream, *, struct_ver: Version = Version((0,))) -> bool:
+        return self.from_bytes(stream.get(self.size), struct_ver = struct_ver)
 
-    def from_bytes(self, bytes_: bytes, *, struct_ver: Version = Version((0,))) -> bytes:
-        return bytes_
+    def from_bytes(self, bytes_: bytes, *, struct_ver: Version = Version((0,))) -> bool:
+        return not not struct.unpack(self.struct_symbol, bytes_)[0]
 
-    def to_bytes(self, value: bytes) -> bytes:
-        return value
+    def to_bytes(self, value: bool) -> bytes:
+        return struct.pack(self.struct_symbol, 1 if value else 0)
 
-    def __class_getitem__(cls, item: int) -> Bytes:
-        return cls(item)
+
+bool8 = Bool(1, "<B")
+bool16 = Bool(2, "<H")
+bool32 = Bool(4, "<I")
+bool64 = Bool(8, "<Q")
```

### Comparing `binary_file_parser-0.1.4/src/binary_file_parser/types/Float.py` & `binary_file_parser-0.2.0/src/binary_file_parser/types/le/float.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import struct
 
-from binary_file_parser.types.ByteStream import ByteStream
-from binary_file_parser.types.Parseable import Parseable
-from binary_file_parser.utils import Version
+from binary_file_parser.types.parseable import Parseable
+from binary_file_parser.types.byte_stream import ByteStream
+from binary_file_parser.types.version import Version
 
 
 class Float(Parseable):
     __slots__ = "struct_symbol"
 
     def __init__(self, size: int, struct_symbol: str):
         super().__init__(size)
@@ -17,10 +17,10 @@
 
     def from_bytes(self, bytes_: bytes, *, struct_ver: Version = Version((0,))) -> float:
         return struct.unpack(self.struct_symbol, bytes_)[0]
 
     def to_bytes(self, value: float) -> bytes:
         return struct.pack(self.struct_symbol, value)
 
-float16 = Float(2, "e")
-float32 = Float(4, "f")
-float64 = Float(8, "d")
+float16 = Float(2, "<e")
+float32 = Float(4, "<f")
+float64 = Float(8, "<d")
```

### Comparing `binary_file_parser-0.1.4/src/binary_file_parser/types/RefList.py` & `binary_file_parser-0.2.0/src/binary_file_parser/types/ref_list.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,100 +1,99 @@
-from __future__ import annotations
-
-import copy
-from typing import Callable, Generic, Iterable, overload, Type, TYPE_CHECKING, TypeVar, SupportsIndex
-
-from binary_file_parser.utils import Version
-
-if TYPE_CHECKING:
-    from binary_file_parser.retrievers import BaseStruct
-
-T = TypeVar("T")
-
-
-def ref_listify(cls: Type[RefList], struct_ver: Version, parent: BaseStruct) -> Callable[[T], T]:
-    def listify(i):
-        if not isinstance(i, list):
-            return i
-        return cls(i, struct_ver, parent)
-
-    return listify
-
-
-class RefList(list, Generic[T]):
-    def __init__(self, iterable: Iterable[T], struct_ver = Version((0,)), parent: BaseStruct = None):
-        # todo: set idxs on structs where relevant
-        # todo: set own idx for nested lists
-        # todo: stop recursive set struct vers and parents if same
-        iterable = map(ref_listify(self.__class__, struct_ver, parent), iterable)
-        super().__init__(iterable)
-        self._struct_ver = struct_ver
-        self._parent = parent
-
-    def __deepcopy__(self, memo):
-        cls = self.__class__
-
-        cloned_list = copy.deepcopy(list(self), memo)
-
-        reflist = cls(cloned_list, copy.deepcopy(self.struct_ver), None)
-        memo[id(self)] = reflist
-
-        return reflist
-
-    def set_sub_attrs(self, obj: T):
-        if getattr(obj, 'is_struct', False) or isinstance(obj, RefList):
-            obj.parent = self.parent
-            obj.struct_ver = self.struct_ver
-
-    @property
-    def struct_ver(self) -> Version:
-        return self._struct_ver
-
-    @struct_ver.setter
-    def struct_ver(self, new_struct_ver: Version):
-        self._struct_ver = new_struct_ver
-        for obj in self:
-            if getattr(obj, 'is_struct', False) or isinstance(obj, RefList):
-                obj.struct_ver = self.struct_ver
-
-    @property
-    def parent(self) -> BaseStruct:
-        return self._parent
-
-    @parent.setter
-    def parent(self, new_parent: BaseStruct):
-        self._parent = new_parent
-        for obj in self:
-            if getattr(obj, 'is_struct', False) or isinstance(obj, RefList):
-                obj.parent = self.parent
-
-    def append(self, obj: T) -> None:
-        super().append(obj)
-        self.set_sub_attrs(obj)
-
-    def extend(self, iterable: Iterable[T]) -> None:
-        super().extend(iterable)
-        for obj in iterable:
-            self.set_sub_attrs(obj)
-
-    def insert(self, index: SupportsIndex, obj: T) -> None:
-        super().insert(index, obj)
-        self.set_sub_attrs(obj)
-
-    @overload
-    def __setitem__(self, i: SupportsIndex, o: T) -> None: ...
-
-    @overload
-    def __setitem__(self, s: slice, o: Iterable[T]) -> None: ...
-
-    def __setitem__(self, i: SupportsIndex | slice, o: T | Iterable[T]) -> None:
-        self.set_sub_attrs(o)
-        super().__setitem__(i, o)
-
-    def __add__(self, x: RefList[T]) -> RefList[T]:
-        return RefList(super().__add__(x), self.struct_ver, self.parent)
-
-    def __iadd__(self: RefList[T], x: Iterable[T]) -> RefList[T]:
-        return RefList(super().__iadd__(x), self.struct_ver, self.parent)
-
-    def __radd__(self, other: RefList[T]) -> RefList[T]:
-        return self.__add__(other)
+# from __future__ import annotations
+#
+# import copy
+# from typing import Callable, Generic, Iterable, overload, Type, TYPE_CHECKING, TypeVar, SupportsIndex
+#
+# from binary_file_parser.types.version import Version
+#
+# if TYPE_CHECKING:
+#     from binary_file_parser.types.base_struct import BaseStruct
+#
+# T = TypeVar("T")
+#
+#
+# def ref_listify(cls: Type[RefList], struct_ver: Version, parent: BaseStruct) -> Callable[[T], T]:
+#     def listify(i):
+#         if not isinstance(i, list):
+#             return i
+#         return cls(i, struct_ver, parent)
+#
+#     return listify
+#
+# class RefList(list, Generic[T]):
+#     def __init__(self, iterable: Iterable[T], struct_ver: Version, parent: BaseStruct):
+#         # todo: set idxs on structs where relevant
+#         # todo: set own idx for nested lists
+#         # todo: stop recursive set struct vers and parents if same
+#         iterable = map(ref_listify(self.__class__, struct_ver, parent), iterable)
+#         super().__init__(iterable)
+#         self._struct_ver = struct_ver
+#         self._parent = parent
+#
+#     def __deepcopy__(self, memo):
+#         cls = self.__class__
+#
+#         cloned_list = copy.deepcopy(list(self), memo)
+#
+#         reflist = cls(cloned_list, copy.deepcopy(self.struct_ver), None)
+#         memo[id(self)] = reflist
+#
+#         return reflist
+#
+#     def set_sub_attrs(self, obj: T):
+#         if getattr(obj, 'is_struct', False) or isinstance(obj, RefList):
+#             obj.parent = self.parent
+#             obj.struct_ver = self.struct_ver
+#
+#     @property
+#     def struct_ver(self) -> Version:
+#         return self._struct_ver
+#
+#     @struct_ver.setter
+#     def struct_ver(self, new_struct_ver: Version):
+#         self._struct_ver = new_struct_ver
+#         for obj in self:
+#             if getattr(obj, 'is_struct', False) or isinstance(obj, RefList):
+#                 obj.struct_ver = self.struct_ver
+#
+#     @property
+#     def parent(self) -> BaseStruct:
+#         return self._parent
+#
+#     @parent.setter
+#     def parent(self, new_parent: BaseStruct):
+#         self._parent = new_parent
+#         for obj in self:
+#             if getattr(obj, 'is_struct', False) or isinstance(obj, RefList):
+#                 obj.parent = self.parent
+#
+#     def append(self, obj: T) -> None:
+#         super().append(obj)
+#         self.set_sub_attrs(obj)
+#
+#     def extend(self, iterable: Iterable[T]) -> None:
+#         super().extend(iterable)
+#         for obj in iterable:
+#             self.set_sub_attrs(obj)
+#
+#     def insert(self, index: SupportsIndex, obj: T) -> None:
+#         super().insert(index, obj)
+#         self.set_sub_attrs(obj)
+#
+#     @overload
+#     def __setitem__(self, i: SupportsIndex, o: T) -> None: ...
+#
+#     @overload
+#     def __setitem__(self, s: slice, o: Iterable[T]) -> None: ...
+#
+#     def __setitem__(self, i: SupportsIndex | slice, o: T | Iterable[T]) -> None:
+#         self.set_sub_attrs(o)
+#         super().__setitem__(i, o)
+#
+#     def __add__(self, x: RefList[T]) -> RefList[T]:
+#         return RefList(super().__add__(x), self.struct_ver, self.parent)
+#
+#     def __iadd__(self: RefList[T], x: Iterable[T]) -> RefList[T]:
+#         return RefList(super().__iadd__(x), self.struct_ver, self.parent)
+#
+#     def __radd__(self, other: RefList[T]) -> RefList[T]:
+#         return self.__add__(other)
```

### Comparing `binary_file_parser-0.1.4/src/binary_file_parser/types/Str.py` & `binary_file_parser-0.2.0/src/binary_file_parser/types/le/string.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import struct
 from abc import ABC
 
-from binary_file_parser.types.ByteStream import ByteStream
-from binary_file_parser.types.Parseable import Parseable
-from binary_file_parser.utils import Version
+from binary_file_parser.types.byte_stream import ByteStream
+from binary_file_parser.types.parseable import Parseable
+from binary_file_parser.types.version import Version
 
 
 class BaseStr(Parseable, ABC):
     __slots__ = ()
 
     def from_bytes(self, bytes_: bytes, *, struct_ver: Version = Version((0,))) -> str:
         try:
```

### Comparing `binary_file_parser-0.1.4/src/binary_file_parser/utils.py` & `binary_file_parser-0.2.0/src/binary_file_parser/types/version.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,10 +20,7 @@
 
     @classmethod
     def from_str(cls, version_str: str) -> Version:
         return Version(map(int, version_str.split('.')))
 
     def __init__(self, tup: Iterable[int]):
         ...
-
-def indentify(repr_str: str, indent = 4) -> str:
-    return f"\n{' '*indent}".join(repr_str.splitlines())
```

### Comparing `binary_file_parser-0.1.4/src/binary_file_parser.egg-info/PKG-INFO` & `binary_file_parser-0.2.0/src/binary_file_parser.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binary-file-parser
-Version: 0.1.4
+Version: 0.2.0
 Summary: Read/Write binary files after describing their specifications in code (similar to an ORM table schema)
 Author-email: Divy1211 <divy1211.dc@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Alian713
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -65,19 +65,19 @@
 
 ## Getting Started
 
 This is a very basic script to give you an idea of how to use this library. Check out the API Reference (coming soon™) for documentation containing more details on how to use this library.
 
 ```py
 from binary_file_parser import BaseStruct, Retriever
-from binary_file_parser.types import uint32, uint64, str32, FixedLenStr
+from binary_file_parser.types import int32, uint64, str32, FixedLenStr
 
 class Spam(BaseStruct):
-    file_version: str = Retriever(FixedLenStr[4], default = 0)
-    creator_name: str = Retriever(str32, default = 0)
+    file_version: str = Retriever(FixedLenStr[4], default = "1.00")
+    creator_name: str = Retriever(str32, default = "bfp")
     saved_timestamp: int = Retriever(uint64, default = 0)
     eggs: int = Retriever(int32, default = 0)
 
 # read a binary file that has the above format
 file = Spam.from_file("path/to/file")
 
 # modify the creator name
@@ -94,15 +94,15 @@
 1. You can use your own structs within another struct
 2. Event hooks help you keep any interdependencies in the file structure synchronised:
 
 ```py
 from __future__ import annotations
 
 from binary_file_parser import BaseStruct, Retriever
-from binary_file_parser.types import FixedLenArray, uint8
+from binary_file_parser.types import FixedLenArray, uint32, uint8
 
 
 class Pixel(BaseStruct):
     red: int = Retriever(uint8, default = 0)
     green: int = Retriever(uint8, default = 0)
     blue: int = Retriever(uint8, default = 0)
     alpha: int = Retriever(uint8, default = 0)
@@ -116,14 +116,15 @@
     ):
         super().__init__(initialise_defaults = False)
         self.red = red
         self.green = green
         self.blue = blue
         self.alpha = alpha
 
+
 class Img(BaseStruct):
     @staticmethod
     def _set_width(retriever: Retriever, obj: Img):
         # here Img.pixels.dtype refers to FixedLenArray
         Img.pixels.dtype.length = obj._width
 
     @staticmethod
@@ -133,33 +134,33 @@
 
     @staticmethod
     def _update_dims(retriever: Retriever, obj: Img):
         # this ensures that when the file is written back, the height and width being written back to file are
         # up to date
         obj._height = obj.height
         Img.pixels.dtype.length = obj._width = obj.width
-    
+
     _width: int = Retriever(uint32, default = 100, on_read = [_set_width], on_write = [_update_dims])
     _height: int = Retriever(uint32, default = 200, on_set = [_set_height])
     pixels: list[list[Pixel]] = Retriever(
-        FixedLenArray[Pixel, 100], default = [Pixel(0, 0, 0) for _ in range(100)], repeat = 200
+        FixedLenArray[Pixel, 100], default_factory = lambda _, __: [Pixel(0, 0, 0) for _ in range(100)], repeat = 200
     )
 
     @property
     def width(self) -> int:
         return len(self.pixels[0])
 
     @property
     def height(self) -> int:
         return len(self.pixels)
 
+
 # Make a new image from all defaults
 a = Img()
-# Note: Mutable defaults will be shallow copied, (this means all rows of pixels in the above example are the same!)
-# If you have larger structs or nested structs, use default_factory (coming soon:tm:) instead
+# Note: Mutable defaults will be shallow copied, use default_factory when such is not intended
 ```
 
 ## About the Author
 
 If you have any questions, suggestions or feedback regarding the library, feel free to send me a message on discord!
 
 | Author   | Discord       |
```

### Comparing `binary_file_parser-0.1.4/src/binary_file_parser.egg-info/SOURCES.txt` & `binary_file_parser-0.2.0/src/binary_file_parser.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,30 @@
 src/binary_file_parser/__init__.py
 src/binary_file_parser/utils.py
 src/binary_file_parser.egg-info/PKG-INFO
 src/binary_file_parser.egg-info/SOURCES.txt
 src/binary_file_parser.egg-info/dependency_links.txt
 src/binary_file_parser.egg-info/requires.txt
 src/binary_file_parser.egg-info/top_level.txt
-src/binary_file_parser/errors/CompressionError.py
-src/binary_file_parser/errors/DefaultValueError.py
-src/binary_file_parser/errors/ParsingError.py
-src/binary_file_parser/errors/VersionError.py
 src/binary_file_parser/errors/__init__.py
-src/binary_file_parser/retrievers/MapValidate.py
-src/binary_file_parser/retrievers/RetreiverCombiner.py
-src/binary_file_parser/retrievers/RetreiverRef.py
-src/binary_file_parser/retrievers/Retriever.py
+src/binary_file_parser/errors/compression_error.py
+src/binary_file_parser/errors/default_value_error.py
+src/binary_file_parser/errors/parsing_error.py
+src/binary_file_parser/errors/version_error.py
 src/binary_file_parser/retrievers/__init__.py
-src/binary_file_parser/retrievers/base_struct.py
-src/binary_file_parser/types/Array.py
-src/binary_file_parser/types/Bool.py
-src/binary_file_parser/types/ByteStream.py
-src/binary_file_parser/types/Bytes.py
-src/binary_file_parser/types/Float.py
-src/binary_file_parser/types/Int.py
-src/binary_file_parser/types/Parseable.py
-src/binary_file_parser/types/RefList.py
-src/binary_file_parser/types/Str.py
-src/binary_file_parser/types/__init__.py
+src/binary_file_parser/retrievers/map_validate.py
+src/binary_file_parser/retrievers/retriever.py
+src/binary_file_parser/retrievers/retriever_combiner.py
+src/binary_file_parser/retrievers/retriever_ref.py
+src/binary_file_parser/types/__init__.py
+src/binary_file_parser/types/base_struct.py
+src/binary_file_parser/types/byte_stream.py
+src/binary_file_parser/types/parseable.py
+src/binary_file_parser/types/ref_list.py
+src/binary_file_parser/types/version.py
+src/binary_file_parser/types/le/__init__.py
+src/binary_file_parser/types/le/array.py
+src/binary_file_parser/types/le/bool.py
+src/binary_file_parser/types/le/bytes.py
+src/binary_file_parser/types/le/float.py
+src/binary_file_parser/types/le/int.py
+src/binary_file_parser/types/le/string.py
```

