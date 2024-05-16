# Comparing `tmp/ebb_time_series-0.1.0.tar.gz` & `tmp/ebb_time_series-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebb_time_series-0.1.0.tar", max compression
+gzip compressed data, was "ebb_time_series-0.2.0.tar", max compression
```

## Comparing `ebb_time_series-0.1.0.tar` & `ebb_time_series-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1067 2024-05-10 22:25:27.000848 ebb_time_series-0.1.0/LICENSE
--rw-r--r--   0        0        0     2264 2024-05-13 22:11:05.101506 ebb_time_series-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-10 22:25:27.006306 ebb_time_series-0.1.0/ebb_time_series/__init__.py
--rw-r--r--   0        0        0      399 2024-05-16 16:14:33.959351 ebb_time_series-0.1.0/ebb_time_series/constants.py
--rw-r--r--   0        0        0      233 2024-05-16 16:14:33.959702 ebb_time_series-0.1.0/ebb_time_series/data_schema.py
--rw-r--r--   0        0        0     1195 2024-05-16 16:14:33.959938 ebb_time_series-0.1.0/ebb_time_series/event_parser_helpers.py
--rw-r--r--   0        0        0      259 2024-05-16 16:14:33.960286 ebb_time_series-0.1.0/ebb_time_series/exceptions.py
--rw-r--r--   0        0        0     9389 2024-05-16 16:14:33.960644 ebb_time_series-0.1.0/ebb_time_series/writers/aws_timestream_data_writer.py
--rw-r--r--   0        0        0     2110 2024-05-16 16:14:33.960966 ebb_time_series-0.1.0/ebb_time_series/writers/base_data_writer.py
--rw-r--r--   0        0        0      551 2024-05-16 16:14:33.961799 ebb_time_series-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2791 1970-01-01 00:00:00.000000 ebb_time_series-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-10 22:25:27.000848 ebb_time_series-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2264 2024-05-13 22:11:05.101506 ebb_time_series-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-10 22:25:27.006306 ebb_time_series-0.2.0/ebb_time_series/__init__.py
+-rw-r--r--   0        0        0      399 2024-05-16 16:14:33.959351 ebb_time_series-0.2.0/ebb_time_series/constants.py
+-rw-r--r--   0        0        0      233 2024-05-16 16:14:33.959702 ebb_time_series-0.2.0/ebb_time_series/data_schema.py
+-rw-r--r--   0        0        0     1195 2024-05-16 16:14:33.959938 ebb_time_series-0.2.0/ebb_time_series/event_parser_helpers.py
+-rw-r--r--   0        0        0      259 2024-05-16 16:14:33.960286 ebb_time_series-0.2.0/ebb_time_series/exceptions.py
+-rw-r--r--   0        0        0     9582 2024-05-16 17:01:44.194983 ebb_time_series-0.2.0/ebb_time_series/writers/aws_timestream_data_writer.py
+-rw-r--r--   0        0        0     2110 2024-05-16 16:14:33.960966 ebb_time_series-0.2.0/ebb_time_series/writers/base_data_writer.py
+-rw-r--r--   0        0        0      551 2024-05-16 17:01:44.195330 ebb_time_series-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2791 1970-01-01 00:00:00.000000 ebb_time_series-0.2.0/PKG-INFO
```

### Comparing `ebb_time_series-0.1.0/LICENSE` & `ebb_time_series-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ebb_time_series-0.1.0/README.md` & `ebb_time_series-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ebb_time_series-0.1.0/ebb_time_series/event_parser_helpers.py` & `ebb_time_series-0.2.0/ebb_time_series/event_parser_helpers.py`

 * *Files identical despite different names*

### Comparing `ebb_time_series-0.1.0/ebb_time_series/writers/aws_timestream_data_writer.py` & `ebb_time_series-0.2.0/ebb_time_series/writers/aws_timestream_data_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
     MEASURENAME = "MeasureName"
     MEASURVALUES = "MeasureValues"
     MEASUREVALUETYPE = "MeasureValueType"
     TIME = "Time"
     TIMEUNIT = "TimeUnit"
     DIMENSIONS = "Dimensions"
+    DIMENSION_TYPE = "DimensionValueType"
     VALUE = "Value"
     NAME = "Name"
     TYPE = "Type"
 
 
 class AwsTimestreamValueTypes(Enum):
     """
@@ -92,15 +93,15 @@
         dimensions = []
         for field_name, field_value in dimensions_dict.items():
             if field_value is not None:
                 dimensions.append(
                     {
                         AwsTimestreamFields.NAME.value: field_name,
                         AwsTimestreamFields.VALUE.value: field_value,
-                        AwsTimestreamFields.TYPE.value: AwsTimestreamValueTypes.VARCHAR.value,
+                        AwsTimestreamFields.DIMENSION_TYPE.value: AwsTimestreamValueTypes.VARCHAR.value,
                     }
                 )
             else:
                 logging.info(
                     f"Skipping field: {field_name} in _build_aws_dimensions because value is None."
                 )
         return dimensions
@@ -140,17 +141,18 @@
                 f"Payload data does not match expected data schema: {str(error)}."
             )
             raise
 
         # key structure = "variable_name", value structure = {"value": ___, "units": ___}
         for key, value in event_data.items():
             key_unit_slug = slugify_name_and_units(variable_name=key, data_dict=value)
+            # Value must be cast as string for boto3 write even though it's a DOUBLE type
             record = {
                 AwsTimestreamFields.NAME.value: key_unit_slug,
-                AwsTimestreamFields.VALUE.value: value.get(DATA_VALUE_FIELDNAME),
+                AwsTimestreamFields.VALUE.value: str(value.get(DATA_VALUE_FIELDNAME)),
                 AwsTimestreamFields.TYPE.value: AwsTimestreamValueTypes.DOUBLE.value,
             }
             list_of_records.append(record)
 
         return [
             {
                 AwsTimestreamFields.MEASURENAME.value: "measurement",
@@ -176,31 +178,31 @@
             region_name=self.aws_region,
             read_timeout=READ_TIMEOUT,
             max_pool_connections=MAX_POOL_CONNECTIONS,
             retries={"max_attempts": MAX_ATTEMPTS},
         )
         try:
             event_id = event_consumer.get_event_id()
-            # Timestamp in milliseconds
-            timestamp = event_consumer.get_event_time().timestamp() * 1000
+            # Timestamp in milliseconds - must be string for boto3 write
+            timestamp_str = str(event_consumer.get_event_time().timestamp() * 1000)
 
             # Build dimension data dict from event_envelope fields and values
             dimensions_data = {
                 ORGANIZATION_FIELDNAME: event_consumer.get_event_organization(),
                 SYSTEM_FIELDNAME: event_consumer.get_event_system_id(),
                 SUBSYSTEM_FIELDNAME: event_consumer.get_event_subsystem_id(),
                 DEVICE_FIELDNAME: event_consumer.get_event_device_id(),
                 SERIAL_NUMBER_FIELDNAME: event_consumer.get_device_serial_number(),
             }
             dimensions = self._build_aws_dimensions(dimensions_dict=dimensions_data)
 
             # Build common attributes dict for aws timestream writer
             common_attributes = {
                 AwsTimestreamFields.DIMENSIONS.value: dimensions,
-                AwsTimestreamFields.TIME.value: timestamp,
+                AwsTimestreamFields.TIME.value: timestamp_str,
                 AwsTimestreamFields.TIMEUNIT.value: AwsTimestreamTimeUnitTypes.MILLISECONDS.value,
             }
 
             # Parse event message data to build records
             records = self._parse_event_data(event_consumer=event_consumer)
             # Initialize the timestream writer and write to database
             timestream_writer = boto3.client("timestream-write", config=config)
```

### Comparing `ebb_time_series-0.1.0/ebb_time_series/writers/base_data_writer.py` & `ebb_time_series-0.2.0/ebb_time_series/writers/base_data_writer.py`

 * *Files identical despite different names*

### Comparing `ebb_time_series-0.1.0/pyproject.toml` & `ebb_time_series-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ebb-time-series"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["Ryan Bloom <ryan.bloom@ebbcarbon.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 ebb-events = "^0.3.2"
```

### Comparing `ebb_time_series-0.1.0/PKG-INFO` & `ebb_time_series-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebb-time-series
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: Ryan Bloom
 Author-email: ryan.bloom@ebbcarbon.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

