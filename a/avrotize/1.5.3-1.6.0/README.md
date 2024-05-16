# Comparing `tmp/avrotize-1.5.3.tar.gz` & `tmp/avrotize-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avrotize-1.5.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "avrotize-1.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `avrotize-1.5.3.tar` & `avrotize-1.6.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0    30034 2024-05-14 18:52:03.138231 avrotize-1.5.3/README.md
--rw-r--r--   0        0        0     1673 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/__init__.py
--rw-r--r--   0        0        0       88 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/__main__.py
--rw-r--r--   0        0        0      411 2024-05-14 18:52:07.602216 avrotize-1.5.3/avrotize/_version.py
--rw-r--r--   0        0        0     8386 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/asn1toavro.py
--rw-r--r--   0        0        0    16902 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/avrotize.py
--rw-r--r--   0        0        0    48409 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/avrotocsharp.py
--rw-r--r--   0        0        0    58275 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/avrotojava.py
--rw-r--r--   0        0        0    12117 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/avrotojs.py
--rw-r--r--   0        0        0    18104 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/avrotojsons.py
--rw-r--r--   0        0        0     6501 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/avrotokusto.py
--rw-r--r--   0        0        0     5481 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/avrotoparquet.py
--rw-r--r--   0        0        0    22200 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/avrotoproto.py
--rw-r--r--   0        0        0    13360 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/avrotopython.py
--rw-r--r--   0        0        0    10166 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/avrotots.py
--rw-r--r--   0        0        0     9514 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/avrototsql.py
--rw-r--r--   0        0        0    16313 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/avrotoxsd.py
--rw-r--r--   0        0        0    13758 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/common.py
--rw-r--r--   0        0        0      112 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/constants.py
--rw-r--r--   0        0        0    19374 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/dependency_resolver.py
--rw-r--r--   0        0        0     1272 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/generic/generic.avsc
--rw-r--r--   0        0        0    95346 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/jsonstoavro.py
--rw-r--r--   0        0        0     2112 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/kconnect.json
--rw-r--r--   0        0        0     2537 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/kstructtoavro.py
--rw-r--r--   0        0        0    20738 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/kustotoavro.py
--rw-r--r--   0        0        0    19742 2024-05-14 18:52:03.142231 avrotize-1.5.3/avrotize/proto2parser.py
--rw-r--r--   0        0        0    15536 2024-05-14 18:52:03.142231 avrotize-1.5.3/avrotize/proto3parser.py
--rw-r--r--   0        0        0     8722 2024-05-14 18:52:03.142231 avrotize-1.5.3/avrotize/prototoavro.py
--rw-r--r--   0        0        0     3390 2024-05-14 18:52:03.142231 avrotize-1.5.3/avrotize/prototypes/any.avsc
--rw-r--r--   0        0        0     6521 2024-05-14 18:52:03.142231 avrotize-1.5.3/avrotize/prototypes/api.avsc
--rw-r--r--   0        0        0     1629 2024-05-14 18:52:03.142231 avrotize-1.5.3/avrotize/prototypes/duration.avsc
--rw-r--r--   0        0        0     3558 2024-05-14 18:52:03.142231 avrotize-1.5.3/avrotize/prototypes/field_mask.avsc
--rw-r--r--   0        0        0     2394 2024-05-14 18:52:03.142231 avrotize-1.5.3/avrotize/prototypes/struct.avsc
--rw-r--r--   0        0        0      792 2024-05-14 18:52:03.142231 avrotize-1.5.3/avrotize/prototypes/timestamp.avsc
--rw-r--r--   0        0        0     6296 2024-05-14 18:52:03.142231 avrotize-1.5.3/avrotize/prototypes/type.avsc
--rw-r--r--   0        0        0     2571 2024-05-14 18:52:03.142231 avrotize-1.5.3/avrotize/prototypes/wrappers.avsc
--rw-r--r--   0        0        0    17371 2024-05-14 18:52:03.142231 avrotize-1.5.3/avrotize/xsdtoavro.py
--rw-r--r--   0        0        0     1169 2024-05-14 18:52:03.142231 avrotize-1.5.3/pyproject.toml
--rw-r--r--   0        0        0    30740 1970-01-01 00:00:00.000000 avrotize-1.5.3/PKG-INFO
+-rw-r--r--   0        0        0    30034 2024-05-15 18:02:40.993092 avrotize-1.6.0/README.md
+-rw-r--r--   0        0        0     1817 2024-05-15 18:02:40.993092 avrotize-1.6.0/avrotize/__init__.py
+-rw-r--r--   0        0        0       88 2024-05-15 18:02:40.993092 avrotize-1.6.0/avrotize/__main__.py
+-rw-r--r--   0        0        0      411 2024-05-15 18:02:47.637059 avrotize-1.6.0/avrotize/_version.py
+-rw-r--r--   0        0        0     8386 2024-05-15 18:02:40.993092 avrotize-1.6.0/avrotize/asn1toavro.py
+-rw-r--r--   0        0        0    17971 2024-05-15 18:02:40.993092 avrotize-1.6.0/avrotize/avrotize.py
+-rw-r--r--   0        0        0    48409 2024-05-15 18:02:40.993092 avrotize-1.6.0/avrotize/avrotocsharp.py
+-rw-r--r--   0        0        0    58275 2024-05-15 18:02:40.993092 avrotize-1.6.0/avrotize/avrotojava.py
+-rw-r--r--   0        0        0    12117 2024-05-15 18:02:40.993092 avrotize-1.6.0/avrotize/avrotojs.py
+-rw-r--r--   0        0        0    18104 2024-05-15 18:02:40.993092 avrotize-1.6.0/avrotize/avrotojsons.py
+-rw-r--r--   0        0        0     9677 2024-05-15 18:02:40.993092 avrotize-1.6.0/avrotize/avrotokusto.py
+-rw-r--r--   0        0        0     5481 2024-05-15 18:02:40.993092 avrotize-1.6.0/avrotize/avrotoparquet.py
+-rw-r--r--   0        0        0    22200 2024-05-15 18:02:40.993092 avrotize-1.6.0/avrotize/avrotoproto.py
+-rw-r--r--   0        0        0    13360 2024-05-15 18:02:40.993092 avrotize-1.6.0/avrotize/avrotopython.py
+-rw-r--r--   0        0        0    10166 2024-05-15 18:02:40.993092 avrotize-1.6.0/avrotize/avrotots.py
+-rw-r--r--   0        0        0     9514 2024-05-15 18:02:40.993092 avrotize-1.6.0/avrotize/avrototsql.py
+-rw-r--r--   0        0        0    16313 2024-05-15 18:02:40.993092 avrotize-1.6.0/avrotize/avrotoxsd.py
+-rw-r--r--   0        0        0    13758 2024-05-15 18:02:40.993092 avrotize-1.6.0/avrotize/common.py
+-rw-r--r--   0        0        0      112 2024-05-15 18:02:40.993092 avrotize-1.6.0/avrotize/constants.py
+-rw-r--r--   0        0        0    19374 2024-05-15 18:02:40.993092 avrotize-1.6.0/avrotize/dependency_resolver.py
+-rw-r--r--   0        0        0     1272 2024-05-15 18:02:40.993092 avrotize-1.6.0/avrotize/generic/generic.avsc
+-rw-r--r--   0        0        0    95346 2024-05-15 18:02:40.993092 avrotize-1.6.0/avrotize/jsonstoavro.py
+-rw-r--r--   0        0        0     2112 2024-05-15 18:02:40.993092 avrotize-1.6.0/avrotize/kconnect.json
+-rw-r--r--   0        0        0     2537 2024-05-15 18:02:40.993092 avrotize-1.6.0/avrotize/kstructtoavro.py
+-rw-r--r--   0        0        0    20901 2024-05-15 18:02:40.993092 avrotize-1.6.0/avrotize/kustotoavro.py
+-rw-r--r--   0        0        0    19742 2024-05-15 18:02:40.997092 avrotize-1.6.0/avrotize/proto2parser.py
+-rw-r--r--   0        0        0    15536 2024-05-15 18:02:40.997092 avrotize-1.6.0/avrotize/proto3parser.py
+-rw-r--r--   0        0        0     8722 2024-05-15 18:02:40.997092 avrotize-1.6.0/avrotize/prototoavro.py
+-rw-r--r--   0        0        0     3390 2024-05-15 18:02:40.997092 avrotize-1.6.0/avrotize/prototypes/any.avsc
+-rw-r--r--   0        0        0     6521 2024-05-15 18:02:40.997092 avrotize-1.6.0/avrotize/prototypes/api.avsc
+-rw-r--r--   0        0        0     1629 2024-05-15 18:02:40.997092 avrotize-1.6.0/avrotize/prototypes/duration.avsc
+-rw-r--r--   0        0        0     3558 2024-05-15 18:02:40.997092 avrotize-1.6.0/avrotize/prototypes/field_mask.avsc
+-rw-r--r--   0        0        0     2394 2024-05-15 18:02:40.997092 avrotize-1.6.0/avrotize/prototypes/struct.avsc
+-rw-r--r--   0        0        0      792 2024-05-15 18:02:40.997092 avrotize-1.6.0/avrotize/prototypes/timestamp.avsc
+-rw-r--r--   0        0        0     6296 2024-05-15 18:02:40.997092 avrotize-1.6.0/avrotize/prototypes/type.avsc
+-rw-r--r--   0        0        0     2571 2024-05-15 18:02:40.997092 avrotize-1.6.0/avrotize/prototypes/wrappers.avsc
+-rw-r--r--   0        0        0    17371 2024-05-15 18:02:40.997092 avrotize-1.6.0/avrotize/xsdtoavro.py
+-rw-r--r--   0        0        0     1198 2024-05-15 18:02:40.997092 avrotize-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0    30740 1970-01-01 00:00:00.000000 avrotize-1.6.0/PKG-INFO
```

### Comparing `avrotize-1.5.3/README.md` & `avrotize-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.3/avrotize/__init__.py` & `avrotize-1.6.0/avrotize/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 # __init__.py
 
 from .jsonstoavro import convert_jsons_to_avro
+from .kustotoavro import convert_kusto_to_avro
 from .kstructtoavro import convert_kafka_struct_to_avro_schema
 from .asn1toavro import convert_asn1_to_avro
 from .xsdtoavro import convert_xsd_to_avro
 from .prototoavro import  convert_proto_to_avro
 from .avrotojsons import convert_avro_to_json_schema
-from .avrotokusto import convert_avro_to_kusto
+from .avrotokusto import convert_avro_to_kusto_file, convert_avro_to_kusto_db
 from .avrotoparquet import convert_avro_to_parquet
 from .avrotoproto import convert_avro_to_proto
 from .avrototsql import convert_avro_to_tsql
 from .avrotoxsd import convert_avro_to_xsd
 from .avrotojava import convert_avro_to_java, convert_avro_schema_to_java
 from .avrotocsharp import convert_avro_to_csharp, convert_avro_schema_to_csharp
 from .avrotopython import convert_avro_to_python, convert_avro_schema_to_python
 from .avrotots import convert_avro_to_typescript, convert_avro_schema_to_typescript
 from .avrotojs import convert_avro_to_javascript, convert_avro_schema_to_javascript
 
 __all__ = [
     "convert_proto_to_avro",
     "convert_jsons_to_avro",
     "convert_kafka_struct_to_avro_schema",
+    "convert_kusto_to_avro",
     "convert_asn1_to_avro",
     "convert_xsd_to_avro",
     "convert_proto_to_avro",
     "convert_avro_to_json_schema",
-    "convert_avro_to_kusto",
+    "convert_avro_to_kusto_file",
+    "convert_avro_to_kusto_db",
     "convert_avro_to_parquet",
     "convert_avro_to_proto",
     "convert_avro_to_tsql",
     "convert_avro_to_xsd",
     "convert_avro_to_java",
     "convert_avro_schema_to_java",
     "convert_avro_to_csharp",
```

### Comparing `avrotize-1.5.3/avrotize/asn1toavro.py` & `avrotize-1.6.0/avrotize/asn1toavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.3/avrotize/avrotize.py` & `avrotize-1.6.0/avrotize/avrotize.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse
 from avrotize.asn1toavro import convert_asn1_to_avro
 from avrotize.avrotocsharp import convert_avro_to_csharp
 from avrotize.avrotojava import convert_avro_to_java
 from avrotize.avrotojs import convert_avro_to_javascript
 from avrotize.avrotojsons import convert_avro_to_json_schema
-from avrotize.avrotokusto import convert_avro_to_kusto
+from avrotize.avrotokusto import convert_avro_to_kusto_db, convert_avro_to_kusto_file
 from avrotize.avrotoparquet import convert_avro_to_parquet
 from avrotize.avrotoproto import convert_avro_to_proto
 from avrotize.avrotopython import convert_avro_to_python
 from avrotize.avrotots import convert_avro_to_typescript
 from avrotize.avrototsql import convert_avro_to_tsql
 from avrotize.jsonstoavro import convert_jsons_to_avro
 from avrotize.kstructtoavro import convert_kafka_struct_to_avro_schema
@@ -46,17 +46,19 @@
     x2a_parser.add_argument('--avsc', type=str, help='Path to the Avro schema file', required=True)
     x2a_parser.add_argument('--namespace', type=str, help='Namespace for the Avro schema', required=False)
 
     a2x_parser = subparsers.add_parser('a2x', help='Convert Avro schema to XSD schema')
     a2x_parser.add_argument('--avsc', type=str, help='Path to the Avro schema file', required=True)
     a2x_parser.add_argument('--xsd', type=str, help='Path to the XSD schema file', required=True)
 
-    a2k_parser = subparsers.add_parser('a2k', help='Convert Avro schema to Kusto schema')
+    a2k_parser = subparsers.add_parser('a2k', help='Convert Avro schema to Kusto table schemas')
     a2k_parser.add_argument('--avsc', type=str, help='Path to the Avro schema file', required=True)
-    a2k_parser.add_argument('--kusto', type=str, help='Path to the Kusto table', required=True)
+    a2k_parser.add_argument('--kusto', type=str, help='Path to the Kusto table', required=False)
+    a2k_parser.add_argument('--kusto-uri', type=str, help='Kusto Cluster URI to apply the generated schema to.', required=False)
+    a2k_parser.add_argument('--kusto-database', type=str, help='Kusto database name to apply the generated schema to', required=False)
     a2k_parser.add_argument('--record-type', type=str, help='Record type in the Avro schema', required=False)
     a2k_parser.add_argument('--emit-cloudevents-columns', action='store_true', help='Add CloudEvents columns to the Kusto table', default=False)
     
     k2a_parser = subparsers.add_parser('k2a', help='Convert Kusto schema to Avro schema')
     k2a_parser.add_argument('--kusto-uri', type=str, help='Kusto URI', required=True)
     k2a_parser.add_argument('--kusto-database', type=str, help='Kusto database', required=True)
     k2a_parser.add_argument('--avsc', type=str, help='Path to the Avro schema file', required=True)
@@ -157,17 +159,31 @@
         xsd_schema_file_path = args.xsd
         print(f'Converting Avro {avro_schema_path} to XSD {xsd_schema_file_path}')
         convert_xsd_to_avro(avro_schema_path, xsd_schema_file_path)
     elif args.command == 'a2k':
         avro_schema_path = args.avsc
         avro_record_type = args.record_type
         kusto_file_path = args.kusto
+        kusto_uri = args.kusto_uri
+        kusto_database = args.kusto_database
+        if kusto_file_path is None and kusto_uri is None:
+            print("Please specify either the Kusto table schema file (--kusto) or the Kusto URI (--kusto-uri and --kusto-database)")
+            exit(1)
+        if kusto_uri and not kusto_database:
+            print("Please specify the Kusto database name --kusto-database")
+            exit(1)
+        if kusto_database and not kusto_uri:
+            print("Please specify the Kusto URI --kusto-uri")
+            exit(1)
         emit_cloud_events_columns = args.emit_cloudevents_columns
         print(f'Converting Avro {avro_schema_path} to Kusto {kusto_file_path}')
-        convert_avro_to_kusto(avro_schema_path, avro_record_type, kusto_file_path, emit_cloud_events_columns)
+        if kusto_file_path:
+            convert_avro_to_kusto_file(avro_schema_path, avro_record_type, kusto_file_path, emit_cloud_events_columns)
+        if kusto_uri and kusto_database:
+             convert_avro_to_kusto_db(avro_schema_path, avro_record_type, kusto_uri, kusto_database, emit_cloud_events_columns)
     elif args.command == 'k2a':
         kusto_uri = args.kusto_uri
         kusto_database = args.kusto_database
         avro_schema_path = args.avsc
         namespace = args.namespace
         emit_cloudevents_xregistry = args.emit_cloudevents_xregistry
         print(f'Converting Kusto {kusto_uri} to Avro {avro_schema_path}')
```

### Comparing `avrotize-1.5.3/avrotize/avrotocsharp.py` & `avrotize-1.6.0/avrotize/avrotocsharp.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.3/avrotize/avrotojava.py` & `avrotize-1.6.0/avrotize/avrotojava.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.3/avrotize/avrotojs.py` & `avrotize-1.6.0/avrotize/avrotojs.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.3/avrotize/avrotojsons.py` & `avrotize-1.6.0/avrotize/avrotojsons.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.3/avrotize/avrotoparquet.py` & `avrotize-1.6.0/avrotize/avrotoparquet.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.3/avrotize/avrotoproto.py` & `avrotize-1.6.0/avrotize/avrotoproto.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.3/avrotize/avrotopython.py` & `avrotize-1.6.0/avrotize/avrotopython.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.3/avrotize/avrotots.py` & `avrotize-1.6.0/avrotize/avrotots.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.3/avrotize/avrototsql.py` & `avrotize-1.6.0/avrotize/avrototsql.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.3/avrotize/avrotoxsd.py` & `avrotize-1.6.0/avrotize/avrotoxsd.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.3/avrotize/common.py` & `avrotize-1.6.0/avrotize/common.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.3/avrotize/dependency_resolver.py` & `avrotize-1.6.0/avrotize/dependency_resolver.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.3/avrotize/generic/generic.avsc` & `avrotize-1.6.0/avrotize/generic/generic.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.3/avrotize/jsonstoavro.py` & `avrotize-1.6.0/avrotize/jsonstoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.3/avrotize/kconnect.json` & `avrotize-1.6.0/avrotize/kconnect.json`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.3/avrotize/kstructtoavro.py` & `avrotize-1.6.0/avrotize/kstructtoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.3/avrotize/kustotoavro.py` & `avrotize-1.6.0/avrotize/kustotoavro.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,17 @@
 
 JsonNode = Dict[str, 'JsonNode'] | List['JsonNode'] | str | bool | int | None
 
 
 class KustoToAvro:
     """ Converts Kusto table schemas to Avro schema format."""
 
-    def __init__(self, kusto_uri, kusto_database, avro_namespace: str, avro_schema_path, emit_cloudevents_xregistry: bool):
+    def __init__(self, kusto_uri, kusto_database, avro_namespace: str, avro_schema_path, emit_cloudevents_xregistry: bool, token_provider=None):
         """ Initializes the KustoToAvro class with the Kusto URI and database name. """
-        kcsb = KustoConnectionStringBuilder.with_az_cli_authentication(
-            kusto_uri)
+        kcsb = KustoConnectionStringBuilder.with_az_cli_authentication(kusto_uri) if not token_provider else KustoConnectionStringBuilder.with_token_provider(kusto_uri, token_provider)
         self.client = KustoClient(kcsb)
         self.kusto_database = kusto_database
         self.avro_namespace = avro_namespace
         self.avro_schema_path = avro_schema_path
         self.emit_cloudevents_xregistry = emit_cloudevents_xregistry
         if self.emit_cloudevents_xregistry:
             if not self.avro_namespace:
@@ -426,12 +425,12 @@
         base_dir = os.path.dirname(self.avro_schema_path)
         if base_dir and not os.path.exists(base_dir):
             os.makedirs(base_dir)
         with open(self.avro_schema_path, 'w', encoding='utf-8') as avro_file:
             json.dump(output, avro_file, indent=4)
 
 
-def convert_kusto_to_avro(kusto_uri: str, kusto_database: str, avro_namespace: str, avro_schema_file: str, emit_cloudevents_xregistry: bool):
+def convert_kusto_to_avro(kusto_uri: str, kusto_database: str, avro_namespace: str, avro_schema_file: str, emit_cloudevents_xregistry: bool, token_provider=None):
     """ Converts Kusto table schemas to Avro schema format."""
     kusto_to_avro = KustoToAvro(
-        kusto_uri, kusto_database, avro_namespace, avro_schema_file, emit_cloudevents_xregistry)
+        kusto_uri, kusto_database, avro_namespace, avro_schema_file, emit_cloudevents_xregistry, token_provider=token_provider)
     return kusto_to_avro.process_all_tables()
```

### Comparing `avrotize-1.5.3/avrotize/proto2parser.py` & `avrotize-1.6.0/avrotize/proto2parser.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.3/avrotize/proto3parser.py` & `avrotize-1.6.0/avrotize/proto3parser.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.3/avrotize/prototoavro.py` & `avrotize-1.6.0/avrotize/prototoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.3/avrotize/prototypes/any.avsc` & `avrotize-1.6.0/avrotize/prototypes/any.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.3/avrotize/prototypes/api.avsc` & `avrotize-1.6.0/avrotize/prototypes/api.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.3/avrotize/prototypes/duration.avsc` & `avrotize-1.6.0/avrotize/prototypes/duration.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.3/avrotize/prototypes/field_mask.avsc` & `avrotize-1.6.0/avrotize/prototypes/field_mask.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.3/avrotize/prototypes/struct.avsc` & `avrotize-1.6.0/avrotize/prototypes/struct.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.3/avrotize/prototypes/timestamp.avsc` & `avrotize-1.6.0/avrotize/prototypes/timestamp.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.3/avrotize/prototypes/type.avsc` & `avrotize-1.6.0/avrotize/prototypes/type.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.3/avrotize/prototypes/wrappers.avsc` & `avrotize-1.6.0/avrotize/prototypes/wrappers.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.3/avrotize/xsdtoavro.py` & `avrotize-1.6.0/avrotize/xsdtoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.3/pyproject.toml` & `avrotize-1.6.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     "xmlschema>=3.0.2",
     "xmlunittest>=0.5.0",
     "pylint>=3.1.0",
     "dataclasses_json>0.6.4",
     "dataclasses>=0.6",
     "pydantic>=2.7.1",
     "avro>=1.11.3",
+    "testcontainers>=4.4.1",
 ]
 
 [project.scripts]
 avrotize = "avrotize.avrotize:main"
 
 [tool.setuptools_scm]
 write_to = "avrotize/_version.py"
```

### Comparing `avrotize-1.5.3/PKG-INFO` & `avrotize-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avrotize
-Version: 1.5.3
+Version: 1.6.0
 Summary: Tools to convert from and to Avro Schema from various other schema languages.
 Author-email: Clemens Vasters <clemensv@microsoft.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

