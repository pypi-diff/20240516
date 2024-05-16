# Comparing `tmp/libpyinfinite-0.1.0.tar.gz` & `tmp/libpyinfinite-0.1.1.tar.gz`

## Comparing `libpyinfinite-0.1.0.tar` & `libpyinfinite-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 libpyinfinite-0.1.0/libpyinfinite/__init__.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 libpyinfinite-0.1.0/libpyinfinite/module/__init__.py
--rw-r--r--   0        0        0     3770 2020-02-02 00:00:00.000000 libpyinfinite-0.1.0/libpyinfinite/module/module.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 libpyinfinite-0.1.0/libpyinfinite/module/moduleBlockHeader.py
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 libpyinfinite-0.1.0/libpyinfinite/module/moduleFile.py
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 libpyinfinite-0.1.0/libpyinfinite/module/moduleHeader.py
--rw-r--r--   0        0        0     3834 2020-02-02 00:00:00.000000 libpyinfinite-0.1.0/libpyinfinite/module/oodle/oodleDecompressor.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 libpyinfinite-0.1.0/libpyinfinite/reader/__init__.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 libpyinfinite-0.1.0/libpyinfinite/reader/common.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 libpyinfinite-0.1.0/libpyinfinite/tag/__init__.py
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 libpyinfinite-0.1.0/libpyinfinite/tag/tag.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 libpyinfinite-0.1.0/libpyinfinite/tag/tagDataBlock.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 libpyinfinite-0.1.0/libpyinfinite/tag/tagDataReference.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 libpyinfinite-0.1.0/libpyinfinite/tag/tagDependency.py
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 libpyinfinite-0.1.0/libpyinfinite/tag/tagHeader.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 libpyinfinite-0.1.0/libpyinfinite/tag/tagReference.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 libpyinfinite-0.1.0/libpyinfinite/tag/tagStruct.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 libpyinfinite-0.1.0/libpyinfinite/tag/tagTypes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 libpyinfinite-0.1.0/libpyinfinite/tag/zonesets/__init__.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 libpyinfinite-0.1.0/libpyinfinite/tag/zonesets/zonesetHeader.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 libpyinfinite-0.1.0/libpyinfinite/tag/zonesets/zonesetInstance.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 libpyinfinite-0.1.0/libpyinfinite/tag/zonesets/zonesetInstanceHeader.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 libpyinfinite-0.1.0/libpyinfinite/tag/zonesets/zonesetTag.py
--rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 libpyinfinite-0.1.0/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 libpyinfinite-0.1.0/LICENSE
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 libpyinfinite-0.1.0/README.md
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 libpyinfinite-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    42974 2020-02-02 00:00:00.000000 libpyinfinite-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 libpyinfinite-0.1.1/libpyinfinite/__init__.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 libpyinfinite-0.1.1/libpyinfinite/module/__init__.py
+-rw-r--r--   0        0        0     3770 2020-02-02 00:00:00.000000 libpyinfinite-0.1.1/libpyinfinite/module/module.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 libpyinfinite-0.1.1/libpyinfinite/module/moduleBlockHeader.py
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 libpyinfinite-0.1.1/libpyinfinite/module/moduleFile.py
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 libpyinfinite-0.1.1/libpyinfinite/module/moduleHeader.py
+-rw-r--r--   0        0        0     3834 2020-02-02 00:00:00.000000 libpyinfinite-0.1.1/libpyinfinite/module/oodle/oodleDecompressor.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 libpyinfinite-0.1.1/libpyinfinite/reader/__init__.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 libpyinfinite-0.1.1/libpyinfinite/reader/common.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 libpyinfinite-0.1.1/libpyinfinite/tag/__init__.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 libpyinfinite-0.1.1/libpyinfinite/tag/tag.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 libpyinfinite-0.1.1/libpyinfinite/tag/tagDataBlock.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 libpyinfinite-0.1.1/libpyinfinite/tag/tagDataReference.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 libpyinfinite-0.1.1/libpyinfinite/tag/tagDependency.py
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 libpyinfinite-0.1.1/libpyinfinite/tag/tagHeader.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 libpyinfinite-0.1.1/libpyinfinite/tag/tagReference.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 libpyinfinite-0.1.1/libpyinfinite/tag/tagStruct.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 libpyinfinite-0.1.1/libpyinfinite/tag/tagTypes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 libpyinfinite-0.1.1/libpyinfinite/tag/zonesets/__init__.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 libpyinfinite-0.1.1/libpyinfinite/tag/zonesets/zonesetHeader.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 libpyinfinite-0.1.1/libpyinfinite/tag/zonesets/zonesetInstance.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 libpyinfinite-0.1.1/libpyinfinite/tag/zonesets/zonesetInstanceHeader.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 libpyinfinite-0.1.1/libpyinfinite/tag/zonesets/zonesetTag.py
+-rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 libpyinfinite-0.1.1/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 libpyinfinite-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 libpyinfinite-0.1.1/README.md
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 libpyinfinite-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    42975 2020-02-02 00:00:00.000000 libpyinfinite-0.1.1/PKG-INFO
```

### Comparing `libpyinfinite-0.1.0/libpyinfinite/module/module.py` & `libpyinfinite-0.1.1/libpyinfinite/module/module.py`

 * *Files identical despite different names*

### Comparing `libpyinfinite-0.1.0/libpyinfinite/module/moduleBlockHeader.py` & `libpyinfinite-0.1.1/libpyinfinite/module/moduleBlockHeader.py`

 * *Files identical despite different names*

### Comparing `libpyinfinite-0.1.0/libpyinfinite/module/moduleFile.py` & `libpyinfinite-0.1.1/libpyinfinite/module/moduleFile.py`

 * *Files identical despite different names*

### Comparing `libpyinfinite-0.1.0/libpyinfinite/module/moduleHeader.py` & `libpyinfinite-0.1.1/libpyinfinite/module/moduleHeader.py`

 * *Files identical despite different names*

### Comparing `libpyinfinite-0.1.0/libpyinfinite/module/oodle/oodleDecompressor.py` & `libpyinfinite-0.1.1/libpyinfinite/module/oodle/oodleDecompressor.py`

 * *Files identical despite different names*

### Comparing `libpyinfinite-0.1.0/libpyinfinite/reader/common.py` & `libpyinfinite-0.1.1/libpyinfinite/reader/common.py`

 * *Files identical despite different names*

### Comparing `libpyinfinite-0.1.0/libpyinfinite/tag/tag.py` & `libpyinfinite-0.1.1/libpyinfinite/tag/tag.py`

 * *Files identical despite different names*

### Comparing `libpyinfinite-0.1.0/libpyinfinite/tag/tagDataBlock.py` & `libpyinfinite-0.1.1/libpyinfinite/tag/tagDataBlock.py`

 * *Files identical despite different names*

### Comparing `libpyinfinite-0.1.0/libpyinfinite/tag/tagDataReference.py` & `libpyinfinite-0.1.1/libpyinfinite/tag/tagDataReference.py`

 * *Files identical despite different names*

### Comparing `libpyinfinite-0.1.0/libpyinfinite/tag/tagDependency.py` & `libpyinfinite-0.1.1/libpyinfinite/tag/tagDependency.py`

 * *Files identical despite different names*

### Comparing `libpyinfinite-0.1.0/libpyinfinite/tag/tagHeader.py` & `libpyinfinite-0.1.1/libpyinfinite/tag/tagHeader.py`

 * *Files identical despite different names*

### Comparing `libpyinfinite-0.1.0/libpyinfinite/tag/tagReference.py` & `libpyinfinite-0.1.1/libpyinfinite/tag/tagReference.py`

 * *Files identical despite different names*

### Comparing `libpyinfinite-0.1.0/libpyinfinite/tag/tagStruct.py` & `libpyinfinite-0.1.1/libpyinfinite/tag/tagStruct.py`

 * *Files identical despite different names*

### Comparing `libpyinfinite-0.1.0/libpyinfinite/tag/zonesets/zonesetHeader.py` & `libpyinfinite-0.1.1/libpyinfinite/tag/zonesets/zonesetHeader.py`

 * *Files identical despite different names*

### Comparing `libpyinfinite-0.1.0/libpyinfinite/tag/zonesets/zonesetInstance.py` & `libpyinfinite-0.1.1/libpyinfinite/tag/zonesets/zonesetInstance.py`

 * *Files identical despite different names*

### Comparing `libpyinfinite-0.1.0/libpyinfinite/tag/zonesets/zonesetInstanceHeader.py` & `libpyinfinite-0.1.1/libpyinfinite/tag/zonesets/zonesetInstanceHeader.py`

 * *Files identical despite different names*

### Comparing `libpyinfinite-0.1.0/libpyinfinite/tag/zonesets/zonesetTag.py` & `libpyinfinite-0.1.1/libpyinfinite/tag/zonesets/zonesetTag.py`

 * *Files identical despite different names*

### Comparing `libpyinfinite-0.1.0/.gitignore` & `libpyinfinite-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `libpyinfinite-0.1.0/LICENSE` & `libpyinfinite-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `libpyinfinite-0.1.0/README.md` & `libpyinfinite-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 decompressor = OodleDecompressor("./oo2core_8_win64.dll")
 ```
 
 #### Reading the third tag from a module instance:
 ```python
 from libpyinfinite.tag.tag import HiTag
 
-tagData = moduleInstance.readTag(file, 3, decompressor)
+tagData = moduleInstance.read_tag(file, 3, decompressor)
 tagInstance = HiTag()
 tagInstance.read(tagData)
 ```
 
 #### Accessing values from a tag:
 ```python
 print(tagInstance.Header.magic)
```

### Comparing `libpyinfinite-0.1.0/pyproject.toml` & `libpyinfinite-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "libpyinfinite"
-version = "0.1.0"
+version = "0.1.1"
 description = "Python library for dealing with binary files from Halo Infinite"
 license = {file = "LICENSE"}
 authors = [{ name = "Surasia"}]
 requires-python = ">= 3.11.0"
 readme = "README.md"
 keywords = ["Halo", "Halo Infinite", "Module", "Tags", "Module"]
 classifiers = [
```

### Comparing `libpyinfinite-0.1.0/PKG-INFO` & `libpyinfinite-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: libpyinfinite
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python library for dealing with binary files from Halo Infinite
 Project-URL: Repository, https://github.com/Surasia/libpyinfinite
 Project-URL: Issues, https://github.com/Surasia/libpyinfinite/issues
 Author: Surasia
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -721,15 +721,15 @@
 decompressor = OodleDecompressor("./oo2core_8_win64.dll")
 ```
 
 #### Reading the third tag from a module instance:
 ```python
 from libpyinfinite.tag.tag import HiTag
 
-tagData = moduleInstance.readTag(file, 3, decompressor)
+tagData = moduleInstance.read_tag(file, 3, decompressor)
 tagInstance = HiTag()
 tagInstance.read(tagData)
 ```
 
 #### Accessing values from a tag:
 ```python
 print(tagInstance.Header.magic)
```

