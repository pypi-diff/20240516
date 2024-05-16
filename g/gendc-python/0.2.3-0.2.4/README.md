# Comparing `tmp/gendc_python-0.2.3-py3-none-any.whl.zip` & `tmp/gendc_python-0.2.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,13 @@
-Zip file size: 5107 bytes, number of entries: 8
--rw-r--r--  2.0 unx       51 b- defN 24-May-14 20:43 gendc_python/__init__.py
--rw-r--r--  2.0 unx       28 b- defN 24-May-14 20:43 gendc_python/gendc_separator/__init__.py
--rw-r--r--  2.0 unx     8736 b- defN 24-May-14 20:43 gendc_python/gendc_separator/descriptor.py
--rw-r--r--  2.0 unx     1070 b- defN 24-May-14 20:43 gendc_python-0.2.3.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     2008 b- defN 24-May-14 20:43 gendc_python-0.2.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-14 20:43 gendc_python-0.2.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 24-May-14 20:43 gendc_python-0.2.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      688 b- defN 24-May-14 20:43 gendc_python-0.2.3.dist-info/RECORD
-8 files, 12686 bytes uncompressed, 3889 bytes compressed:  69.3%
+Zip file size: 8017 bytes, number of entries: 11
+-rw-r--r--  2.0 unx       52 b- defN 24-May-16 18:29 gendc_python/__init__.py
+-rw-r--r--  2.0 unx       34 b- defN 24-May-16 18:29 gendc_python/gendc_separator/__init__.py
+-rw-r--r--  2.0 unx     2534 b- defN 24-May-16 18:29 gendc_python/gendc_separator/component.py
+-rw-r--r--  2.0 unx     3798 b- defN 24-May-16 18:29 gendc_python/gendc_separator/descriptor.py
+-rw-r--r--  2.0 unx     3540 b- defN 24-May-16 18:29 gendc_python/gendc_separator/part.py
+-rw-r--r--  2.0 unx     1313 b- defN 24-May-16 18:29 gendc_python/gendc_separator/utils.py
+-rw-r--r--  2.0 unx     1070 b- defN 24-May-16 18:29 gendc_python-0.2.4.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     8712 b- defN 24-May-16 18:29 gendc_python-0.2.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-16 18:29 gendc_python-0.2.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 24-May-16 18:29 gendc_python-0.2.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      973 b- defN 24-May-16 18:29 gendc_python-0.2.4.dist-info/RECORD
+11 files, 22131 bytes uncompressed, 6343 bytes compressed:  71.3%
```

## zipnote {}

```diff
@@ -1,25 +1,34 @@
 Filename: gendc_python/__init__.py
 Comment: 
 
 Filename: gendc_python/gendc_separator/__init__.py
 Comment: 
 
+Filename: gendc_python/gendc_separator/component.py
+Comment: 
+
 Filename: gendc_python/gendc_separator/descriptor.py
 Comment: 
 
-Filename: gendc_python-0.2.3.dist-info/LICENSE.txt
+Filename: gendc_python/gendc_separator/part.py
+Comment: 
+
+Filename: gendc_python/gendc_separator/utils.py
+Comment: 
+
+Filename: gendc_python-0.2.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: gendc_python-0.2.3.dist-info/METADATA
+Filename: gendc_python-0.2.4.dist-info/METADATA
 Comment: 
 
-Filename: gendc_python-0.2.3.dist-info/WHEEL
+Filename: gendc_python-0.2.4.dist-info/WHEEL
 Comment: 
 
-Filename: gendc_python-0.2.3.dist-info/top_level.txt
+Filename: gendc_python-0.2.4.dist-info/top_level.txt
 Comment: 
 
-Filename: gendc_python-0.2.3.dist-info/RECORD
+Filename: gendc_python-0.2.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gendc_python/__init__.py

```diff
@@ -1,2 +1,2 @@
-__version__ = '0.2.3'
-from . import gendc_separator
+__version__ = '0.2.4'
+from . import gendc_separator
```

## gendc_python/gendc_separator/__init__.py

```diff
@@ -1,2 +1 @@
-from . import descriptor
-  
+from .descriptor import Container
```

## gendc_python/gendc_separator/descriptor.py

```diff
@@ -1,214 +1,92 @@
-import json
-import copy
-import sys
-import os
-
-container_header_template = {
-    "Signature" : {"size": 4, "offset": 0, "value" : "GNDC"},
-    "Version" : {"size": 3, "offset": 4, "value" : 0},
-    "Reserved" : {"size": 1, "offset": 7, "value" : 0},
-    # ---------------------------------------- 8
-    "HeaderType" : {"size": 2, "offset": 8, "value" : 4096},
-    "Flags" : {"size": 2, "offset": 10, "value" : 0},
-    "HeaderSize" : {"size": 4, "offset": 12, "value" : 0},
-    # ---------------------------------------- 16
-    "Id" : {"size": 8, "offset": 16, "value" : 0},
-    # ---------------------------------------- 24
-    "VariableFields" : {"size": 2, "offset": 24, "value" : 0},
-    "Reserved2" : {"size": 6, "offset": 26, "value" : 0},
-    # ---------------------------------------- 32
-    "DataSize" : {"size": 8, "offset": 32, "value" : 0},
-    # ---------------------------------------- 40
-    "DataOffset" : {"size": 8, "offset": 40, "value" : 0},
-    # ---------------------------------------- 48
-    "DescriptorSize" : {"size": 4, "offset": 48, "value" : 0},
-    "ComponentCount" : {"size": 4, "offset": 52, "value" : 0},
-    # ---------------------------------------- 56
-    "ComponentOffset" : {"size": 8, "offset": [56], "value" : []},
-}
-
-component_header_template = {
-    "HeaderType" : {"size": 2, "offset": 0, "value" : 8192},
-    "Flags" : {"size": 2, "offset": 2, "value" : 0},
-    "HeaderSize" : {"size": 4, "offset": 4, "value" : 0},
-    # ---------------------------------------- 8
-    "Reserved" : {"size": 2, "offset": 8, "value" : 0},
-    "GroupId" : {"size": 2, "offset": 10, "value" : 0},
-    "SourceId" : {"size": 2, "offset": 12, "value" : 0},
-    "RegionId" : {"size": 2, "offset": 14, "value" : 0},
-    # ---------------------------------------- 16
-    "RegionOffsetX" : {"size": 4, "offset": 16, "value" : 0},
-    "RegionOffsetY" : {"size": 4, "offset": 20, "value" : 0},
-    # ---------------------------------------- 24
-    "Timestamp" : {"size": 8, "offset": 24, "value" : 0},
-    # ---------------------------------------- 32
-    "TypeId" : {"size": 8, "offset": 32, "value" : 0},
-    # ---------------------------------------- 40
-    "Format" : {"size": 4, "offset": 40, "value" : 0},
-    "Reserved2" : {"size": 2, "offset": 44, "value" : 0},
-    "PartCount" : {"size": 2, "offset": 46, "value" : 0},
-    # ---------------------------------------- 48
-    "PartOffset" : {"size": 8, "offset": [48], "value" : []},
-}
-
-part_header_template = {
-    "HeaderType" : {"size": 2, "offset": 0, "value" : 0},
-    "Flags" : {"size": 2, "offset": 2, "value" : 0},
-    "HeaderSize" : {"size": 4, "offset": 4, "value" : 0},
-    # ---------------------------------------- 8
-    "Format" : {"size": 4, "offset": 8, "value" : 0},
-    "Reserved" : {"size": 2, "offset": 12, "value" : 0},
-    "FlowId" : {"size": 2, "offset": 14, "value" : 0},
-    # ---------------------------------------- 16
-    "FlowOffset" : {"size": 8, "offset": 16, "value" : 0},
-    # ---------------------------------------- 24
-    "DataSize" : {"size": 8, "offset": 24, "value" : 0},
-    # ---------------------------------------- 32
-    "DataOffset" : {"size": 8, "offset": 32, "value" : 0},
-    # ---------------------------------------- 40
-    "TypeSpecific" : {"size": 8, "offset": [40], "value" : []},
-    # Note:
-    # # ---------------------------------------- 40
-    # "Dimension" : {"size": 8, "offset": 40, "value" : 0},
-    # # ---------------------------------------- 48
-    # "Padding" : {"size": 4, "offset": 48, "value" : 0},
-    # "InfoReserved" : {"size": 4, "offset": 52, "value" : 0},
-    # # ---------------------------------------- 56
-    # ...
-}
-
-def is_valid_key(header_info, key):
-    return key in header_info
-
-# read and write
-def get_offset(header_info, key):
-    if not is_valid_key(header_info, key):
-        raise Exception("Invalid key used")
-    return header_info[key]["offset"]
-
-def set_offset(header_info, key, offset):
-    if not is_valid_key(header_info, key):
-        raise Exception("Invalid key used")
-    header_info[key]["offset"] = offset
-
-# read only
-def get_size(header_info, key):
-    if not is_valid_key(header_info, key):
-        raise Exception("Invalid key used")
-    return header_info[key]["size"]
-
-# read and write
-def get_value(header_info, key):
-    if not is_valid_key(header_info, key):
-        raise Exception("Invalid key used")
-    return header_info[key]["value"]
-
-def set_value(header_info, key, value):
-    if not is_valid_key(header_info, key):
-        raise Exception("Invalid key used")
-    header_info[key]["value"] = value 
-
-def load_from_binary(header_info, binary_info, key, cursor=0):
-    offset = get_offset(header_info, key)
-    size = get_size(header_info, key)
-    if type(offset) is list:
-        return [int.from_bytes(binary_info[cursor+off:cursor+off+size], "little") for off in offset]
-    else:
-        return int.from_bytes(binary_info[cursor+offset:cursor+offset+size], "little")
+from .component import Component
+from .utils import *
+
 
 class Container:
     def __init__(self, binary_info):
         self.component_headers = []
-        self.header = copy.deepcopy(container_header_template)
+        self.header = {
+            "Signature": {"size": 4, "offset": 0, "value": "GNDC"},
+            "Version": {"size": 3, "offset": 4, "value": 0},
+            "Reserved": {"size": 1, "offset": 7, "value": 0},
+            # ---------------------------------------- 8
+            "HeaderType": {"size": 2, "offset": 8, "value": 4096},
+            "Flags": {"size": 2, "offset": 10, "value": 0},
+            "HeaderSize": {"size": 4, "offset": 12, "value": 0},
+            # ---------------------------------------- 16
+            "Id": {"size": 8, "offset": 16, "value": 0},
+            # ---------------------------------------- 24
+            "VariableFields": {"size": 2, "offset": 24, "value": 0},
+            "Reserved2": {"size": 6, "offset": 26, "value": 0},
+            # ---------------------------------------- 32
+            "DataSize": {"size": 8, "offset": 32, "value": 0},
+            # ---------------------------------------- 40
+            "DataOffset": {"size": 8, "offset": 40, "value": 0},
+            # ---------------------------------------- 48
+            "DescriptorSize": {"size": 4, "offset": 48, "value": 0},
+            "ComponentCount": {"size": 4, "offset": 52, "value": 0},
+            # ---------------------------------------- 56
+            "ComponentOffset": {"size": 8, "offset": [56], "value": []},
+        }
 
         if not self.is_gendc_descriptor(binary_info):
             raise Exception("This is not valid GenDC")
 
         for key in self.header:
             if key == "ComponentOffset":
-                set_offset(self.header, "ComponentOffset", [56 + 8 * i for i in range(self.header["ComponentCount"]["value"])])
+                set_offset(self.header, "ComponentOffset",
+                           [56 + 8 * i for i in range(self.header["ComponentCount"]["value"])])
             set_value(self.header, key, load_from_binary(self.header, binary_info, key))
 
         for cursor in self.header["ComponentOffset"]["value"]:
             self.component_headers.append(Component(binary_info, cursor))
-    
+
     def is_gendc_descriptor(self, binary_info):
-        if load_from_binary(self.header, binary_info, "Signature") == 0x43444E47:
-            return True
-        return False
+        return load_from_binary(self.header, binary_info, "Signature") == 0x43444E47
 
     def get_container_size(self):
         return get_value(self.header, "DataSize") + get_value(self.header, "DescriptorSize")
 
+    def get_data_size(self):
+        return get_value(self.header, "DataSize")
+
+    def get_descriptor_size(self):
+        return get_value(self.header, "DescriptorSize")
+
+    def get_component_count(self):
+        return get_value(self.header, "ComponentCount")
+
     # search component #########################################################
-    def get_first_component_datatype_of(self, target_type):
+    def get_1st_component_idx_by_typeid(self, target_type):
         # 1 : intensity
         # 0x0000000000008001 : GDC_METADATA
 
         for ith, ch in enumerate(self.component_headers):
             if ch.is_valid():
-                if ch.get_datatype() == target_type:
+                if ch.get_type_id() == target_type:
                     return ith
-                
         return -1
 
-    def get_first_component_sourceid_of(self, target_sourceid):
+    def get_1st_component_idx_by_sourceid(self, target_sourceid):
         for ith, ch in enumerate(self.component_headers):
             if ch.is_valid():
                 if ch.get("SourceId", -1) == target_sourceid:
                     return ith
-                
         return -1
-    ############################################################################
-
-    def get(self, key, ith_component=-1, jth_part=-1):
-        if ith_component != -1:
-            return (self.component_headers[ith_component]).get(key, jth_part)
-        else:
-            return get_value(self.header, key)
-
-class Component:
-    def __init__(self, binary_info, component_cursor):
 
-        self.part_headers = []
-        self.header = copy.deepcopy(component_header_template)
-
-        for key in self.header:
-            if key == "PartOffset":
-                set_offset(self.header, key, [component_cursor + 48 + 8 * i for i in range(get_value(self.header, "PartCount"))])
-            else:
-                set_offset(self.header, key, component_cursor + get_offset(self.header, key))
-            set_value(self.header, key, load_from_binary(self.header, binary_info, key))
-
-        for cursor in self.header["PartOffset"]["value"]:
-            self.part_headers.append(Part(binary_info, cursor))
-
-
-    def is_valid(self):
-        return get_value(self.header, "Flags") == 0
-
-    def get_datatype(self):
-        return get_value(self.header, "TypeId")
+    ############################################################################
 
-    def get(self, key, jth_part=-1):
-        if jth_part != -1:
-            return self.part_headers[jth_part].get(key)
-        else:
-            return get_value(self.header, key)
+    def get_component_by_index(self, ith_component):
+        return self.component_headers[ith_component]
 
-class Part:
-    def __init__(self, binary_info, part_cursor):
 
-        self.header = copy.deepcopy(part_header_template)
+    def get_component_header_value(self, key, ith_component):
+        return self.component_headers[ith_component].get(key)
 
-        for key in self.header:
-            if not key == "TypeSpecific":
-                set_offset(self.header, key, part_cursor + get_offset(self.header, key))
-            set_value(self.header, key, load_from_binary(self.header, binary_info, key))
 
-        num_typespecific = int((get_value(self.header, "HeaderSize") - 40) / 8)
-        set_offset(self.header, "TypeSpecific", [part_cursor + 40 + 8 * i for i in range(num_typespecific)])
-        set_value(self.header, "TypeSpecific", load_from_binary(self.header, binary_info, "TypeSpecific"))
+    def get_part_header_value(self, key, ith_component, jth_part):
+        return self.component_headers[ith_component].get_part_header_value(key, jth_part)
 
     def get(self, key):
         return get_value(self.header, key)
+
```

## Comparing `gendc_python-0.2.3.dist-info/LICENSE.txt` & `gendc_python-0.2.4.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `gendc_python-0.2.3.dist-info/RECORD` & `gendc_python-0.2.4.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-gendc_python/__init__.py,sha256=38XYrXB505eN4TGl8ModvXGXE9K3aQtZ9V3IYOOYqeo,51
-gendc_python/gendc_separator/__init__.py,sha256=sHTWDRH57ahFgvwJGFMns871Lortp-YaQS_QFLmt8HA,28
-gendc_python/gendc_separator/descriptor.py,sha256=6hJbjkJtmqFubH139ZUhkoFDJrfQxC5p--yrLOVZ_eM,8736
-gendc_python-0.2.3.dist-info/LICENSE.txt,sha256=CdcZBY54Kse8cbohyUThE2zeK7lXwOiIEh8CGNa18Cw,1070
-gendc_python-0.2.3.dist-info/METADATA,sha256=C6WMCQGK_WpwVXylWrDggJFCdAMhrEBmWDeKQSfZLWs,2008
-gendc_python-0.2.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-gendc_python-0.2.3.dist-info/top_level.txt,sha256=HKTB6hISpv3f-3THLIPKPYvaZzcHVGNM1hznVOVy0bY,13
-gendc_python-0.2.3.dist-info/RECORD,,
+gendc_python/__init__.py,sha256=znVyvV6yIT02mjenHAJyBN7zO2aE-v_EScvQpPsqHCY,52
+gendc_python/gendc_separator/__init__.py,sha256=ENTmzRdCKWv0RfDY8WnzaiwvZ0tEitTsYDQJiXArU9w,34
+gendc_python/gendc_separator/component.py,sha256=OXVtRtW33xWbRyb_eQZC_q0KNdmAn-fzMpgOK0KnOe8,2534
+gendc_python/gendc_separator/descriptor.py,sha256=ZHdePtY6pWZPbOHeoGq3TEIm2lrTOS5eusZDx7w4V0Y,3798
+gendc_python/gendc_separator/part.py,sha256=JPz9WuZGRqvmAk1WhqQGohG7Cr6zqMpUBkhyX9Bwr1I,3540
+gendc_python/gendc_separator/utils.py,sha256=3F6DcNJjYrcWBWMAx9KEEanDOVOnoVK9oZtavIhv57w,1313
+gendc_python-0.2.4.dist-info/LICENSE.txt,sha256=CdcZBY54Kse8cbohyUThE2zeK7lXwOiIEh8CGNa18Cw,1070
+gendc_python-0.2.4.dist-info/METADATA,sha256=xY9-OnTX3elDR-7AbMsxcVcHRmf0LP0Z0OXp_E_5INA,8712
+gendc_python-0.2.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+gendc_python-0.2.4.dist-info/top_level.txt,sha256=HKTB6hISpv3f-3THLIPKPYvaZzcHVGNM1hznVOVy0bY,13
+gendc_python-0.2.4.dist-info/RECORD,,
```

