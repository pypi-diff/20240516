# Comparing `tmp/swagger2jsonschema-0.1.0-py3-none-any.whl.zip` & `tmp/swagger2jsonschema-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 9572 bytes, number of entries: 13
+Zip file size: 9570 bytes, number of entries: 13
 -rw-r--r--  2.0 unx        0 b- defN 24-Mar-30 04:09 swagger2jsonschema/__init__.py
 -rw-r--r--  2.0 unx    10217 b- defN 24-May-03 03:02 swagger2jsonschema/command.py
 -rw-r--r--  2.0 unx      707 b- defN 24-Mar-30 04:09 swagger2jsonschema/definitions.py
 -rw-r--r--  2.0 unx       68 b- defN 24-Mar-30 04:09 swagger2jsonschema/errors.py
 -rw-r--r--  2.0 unx      247 b- defN 24-Mar-30 04:09 swagger2jsonschema/log.py
 -rw-r--r--  2.0 unx     6161 b- defN 24-Mar-30 04:09 swagger2jsonschema/test_command.py
--rw-r--r--  2.0 unx     7841 b- defN 24-May-03 03:10 swagger2jsonschema/util.py
--rw-r--r--  2.0 unx      654 b- defN 24-May-03 06:14 swagger2jsonschema-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1486 b- defN 24-May-03 06:14 swagger2jsonschema-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-03 06:14 swagger2jsonschema-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       74 b- defN 24-May-03 06:14 swagger2jsonschema-0.1.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       28 b- defN 24-May-03 06:14 swagger2jsonschema-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1144 b- defN 24-May-03 06:14 swagger2jsonschema-0.1.0.dist-info/RECORD
-13 files, 28719 bytes uncompressed, 7622 bytes compressed:  73.5%
+-rw-r--r--  2.0 unx     7841 b- defN 24-May-16 02:01 swagger2jsonschema/util.py
+-rw-r--r--  2.0 unx      654 b- defN 24-May-16 02:20 swagger2jsonschema-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1486 b- defN 24-May-16 02:20 swagger2jsonschema-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-16 02:20 swagger2jsonschema-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       74 b- defN 24-May-16 02:20 swagger2jsonschema-0.1.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       28 b- defN 24-May-16 02:20 swagger2jsonschema-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1144 b- defN 24-May-16 02:20 swagger2jsonschema-0.1.1.dist-info/RECORD
+13 files, 28719 bytes uncompressed, 7620 bytes compressed:  73.5%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: swagger2jsonschema/test_command.py
 Comment: 
 
 Filename: swagger2jsonschema/util.py
 Comment: 
 
-Filename: swagger2jsonschema-0.1.0.dist-info/LICENSE
+Filename: swagger2jsonschema-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: swagger2jsonschema-0.1.0.dist-info/METADATA
+Filename: swagger2jsonschema-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: swagger2jsonschema-0.1.0.dist-info/WHEEL
+Filename: swagger2jsonschema-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: swagger2jsonschema-0.1.0.dist-info/entry_points.txt
+Filename: swagger2jsonschema-0.1.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: swagger2jsonschema-0.1.0.dist-info/top_level.txt
+Filename: swagger2jsonschema-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: swagger2jsonschema-0.1.0.dist-info/RECORD
+Filename: swagger2jsonschema-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## swagger2jsonschema/util.py

```diff
@@ -136,15 +136,15 @@
 
 
 def get_body_file_prefix(path, http_method):
     name_prefix_fmt = "paths_{:s}_{:s}_{{:s}}_".format(
         # Paths "/" and "/root" will conflict,
         # no idea how to solve this elegantly.
         path.lstrip("/").replace("/", "_") or "root",
-        http_method.upper(),
+        http_method,
     )
     return re.sub(
         r"\{([^:\}]+)\}",
         r"_\1_",
         name_prefix_fmt,
     )
 
@@ -194,15 +194,15 @@
                     component["required"] = required
             if "requestBody" in http_method_definition:
                 content = http_method_definition["requestBody"]["content"]
                 schema = content["application/json"]["schema"]
                 if "$ref" in schema:
                     tmp = schema["$ref"]
                     tmp = tmp.replace("#/components/schemas/", "") + ".json"
-                    component["requestBody"] = tmp
+                    component["requestBody"] = tmp.lower()
                 else:
                     prefix_fmt = get_body_file_prefix(path, http_method)
                     prefix = prefix_fmt.format("request")
                     component["requestBody"] = prefix + "json.json"
             operation_id = http_method_definition["operationId"]
             components[operation_id] = component
```

## Comparing `swagger2jsonschema-0.1.0.dist-info/LICENSE` & `swagger2jsonschema-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `swagger2jsonschema-0.1.0.dist-info/METADATA` & `swagger2jsonschema-0.1.1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swagger2jsonschema
-Version: 0.1.0
+Version: 0.1.1
 Requires-Python: >=3.10
 License-File: LICENSE
 Requires-Dist: attrs ==23.2.0
 Requires-Dist: click ==8.1.7
 Requires-Dist: jsonref ==1.1.0
 Requires-Dist: jsonschema ==4.21.1
 Requires-Dist: jsonschema-specifications ==2023.12.1
```

## Comparing `swagger2jsonschema-0.1.0.dist-info/RECORD` & `swagger2jsonschema-0.1.1.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 swagger2jsonschema/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 swagger2jsonschema/command.py,sha256=2HPZW9u5T02ruVn5OwkPtay4yVpR_zhVbxgtFdyzElw,10217
 swagger2jsonschema/definitions.py,sha256=INDqIV7rCuRtjV73Va5TlGp5sZUPVJY2PodQbcuj600,707
 swagger2jsonschema/errors.py,sha256=T7VZfl3FnHPHoqXFn-QmAXwlwOnPnyo3lcbCYXI_jpQ,68
 swagger2jsonschema/log.py,sha256=TVtGYLJkLhZpgQqe6PUxtSbGVg0RKZvMEvPcsAr0htQ,247
 swagger2jsonschema/test_command.py,sha256=oItmY5OAehwwhGonkD-XTXhEpskt9dp83E_aZrDVk6I,6161
-swagger2jsonschema/util.py,sha256=JefJz8h2IUOgBVy9hQeLnQMbWlSFJE0uDz1QeboVRTg,7841
-swagger2jsonschema-0.1.0.dist-info/LICENSE,sha256=6nn0TvfOBUFH__8Aqqhe6RfDCI_--Js0Jab8oZkAipE,654
-swagger2jsonschema-0.1.0.dist-info/METADATA,sha256=j43PwDMiPnyZsG6jyjoOine3sNpi1vYItI4kcm4iQlI,1486
-swagger2jsonschema-0.1.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-swagger2jsonschema-0.1.0.dist-info/entry_points.txt,sha256=LXKu_O5s2NeA6Ga5NQ0N4quSMB52LTXs0580KiO6a5s,74
-swagger2jsonschema-0.1.0.dist-info/top_level.txt,sha256=T3u6MolDviqt4JENl6aZ0civpLecmX1vds1ASwe_n80,28
-swagger2jsonschema-0.1.0.dist-info/RECORD,,
+swagger2jsonschema/util.py,sha256=FSt0-PNVjGtjAaLMCVRIR8f7fBGUjZTVm-w35ranUw0,7841
+swagger2jsonschema-0.1.1.dist-info/LICENSE,sha256=6nn0TvfOBUFH__8Aqqhe6RfDCI_--Js0Jab8oZkAipE,654
+swagger2jsonschema-0.1.1.dist-info/METADATA,sha256=wJZwmgvjRXTHxE1zHpre-1TdRscB42ohNg7bYour1pk,1486
+swagger2jsonschema-0.1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+swagger2jsonschema-0.1.1.dist-info/entry_points.txt,sha256=LXKu_O5s2NeA6Ga5NQ0N4quSMB52LTXs0580KiO6a5s,74
+swagger2jsonschema-0.1.1.dist-info/top_level.txt,sha256=T3u6MolDviqt4JENl6aZ0civpLecmX1vds1ASwe_n80,28
+swagger2jsonschema-0.1.1.dist-info/RECORD,,
```

