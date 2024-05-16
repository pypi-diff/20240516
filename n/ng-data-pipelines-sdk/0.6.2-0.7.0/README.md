# Comparing `tmp/ng_data_pipelines_sdk-0.6.2.tar.gz` & `tmp/ng_data_pipelines_sdk-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ng_data_pipelines_sdk-0.6.2.tar", max compression
+gzip compressed data, was "ng_data_pipelines_sdk-0.7.0.tar", max compression
```

## Comparing `ng_data_pipelines_sdk-0.6.2.tar` & `ng_data_pipelines_sdk-0.7.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      106 2024-05-14 17:47:38.473033 ng_data_pipelines_sdk-0.6.2/README.md
--rw-r--r--   0        0        0        0 2024-05-14 17:47:38.506033 ng_data_pipelines_sdk-0.6.2/ng_data_pipelines_sdk/__init__.py
--rw-r--r--   0        0        0     9155 2024-05-14 17:47:38.473033 ng_data_pipelines_sdk-0.6.2/ng_data_pipelines_sdk/aws_interface.py
--rw-r--r--   0        0        0      231 2024-05-14 17:47:38.473033 ng_data_pipelines_sdk-0.6.2/ng_data_pipelines_sdk/custom_logger.py
--rw-r--r--   0        0        0    27137 2024-05-14 17:47:38.474033 ng_data_pipelines_sdk-0.6.2/ng_data_pipelines_sdk/dataframe_manager.py
--rw-r--r--   0        0        0    15575 2024-05-14 17:47:38.474033 ng_data_pipelines_sdk-0.6.2/ng_data_pipelines_sdk/interfaces.py
--rw-r--r--   0        0        0     5093 2024-05-14 17:47:38.474033 ng_data_pipelines_sdk-0.6.2/ng_data_pipelines_sdk/spark_manager.py
--rw-r--r--   0        0        0     1453 2024-05-14 17:47:38.474033 ng_data_pipelines_sdk-0.6.2/ng_data_pipelines_sdk/utils.py
--rw-r--r--   0        0        0      695 2024-05-14 17:47:38.477033 ng_data_pipelines_sdk-0.6.2/pyproject.toml
--rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0      106 2024-05-16 12:33:29.095550 ng_data_pipelines_sdk-0.7.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-16 12:33:29.131551 ng_data_pipelines_sdk-0.7.0/ng_data_pipelines_sdk/__init__.py
+-rw-r--r--   0        0        0     9155 2024-05-16 12:33:29.095550 ng_data_pipelines_sdk-0.7.0/ng_data_pipelines_sdk/aws_interface.py
+-rw-r--r--   0        0        0      231 2024-05-16 12:33:29.095550 ng_data_pipelines_sdk-0.7.0/ng_data_pipelines_sdk/custom_logger.py
+-rw-r--r--   0        0        0    28114 2024-05-16 12:33:29.095550 ng_data_pipelines_sdk-0.7.0/ng_data_pipelines_sdk/dataframe_manager.py
+-rw-r--r--   0        0        0    15903 2024-05-16 12:33:29.095550 ng_data_pipelines_sdk-0.7.0/ng_data_pipelines_sdk/interfaces.py
+-rw-r--r--   0        0        0     5093 2024-05-16 12:33:29.096551 ng_data_pipelines_sdk-0.7.0/ng_data_pipelines_sdk/spark_manager.py
+-rw-r--r--   0        0        0     1453 2024-05-16 12:33:29.096551 ng_data_pipelines_sdk-0.7.0/ng_data_pipelines_sdk/utils.py
+-rw-r--r--   0        0        0      695 2024-05-16 12:33:29.100551 ng_data_pipelines_sdk-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-0.7.0/PKG-INFO
```

### Comparing `ng_data_pipelines_sdk-0.6.2/ng_data_pipelines_sdk/aws_interface.py` & `ng_data_pipelines_sdk-0.7.0/ng_data_pipelines_sdk/aws_interface.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.6.2/ng_data_pipelines_sdk/dataframe_manager.py` & `ng_data_pipelines_sdk-0.7.0/ng_data_pipelines_sdk/dataframe_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     DataFrameReadWriteParams,
     FileType,
     FnKind,
     InputDataFrameParams,
     InputDataFrameParamsDict,
     OutputDataFrameParams,
     OutputDataFrameParamsDict,
+    ReadPreviousDayException,
     S3BucketParams,
     S3ReadJsonParams,
     StepParams,
     StepParamsDict,
     TransformParams,
     TransformParamsDict,
     DataFrameDict,
@@ -191,20 +192,33 @@
         elif df_params.s3_schema_path_params:
             schema = self.retrieve_schema_from_s3(df_params.s3_schema_path_params)
         else:
             schema = None
 
         logger.info(f"Reading DataFrame from {path}...")
 
-        df = self.spark_manager.read(
-            env=read_params.bucket_params.env,
-            path=path,
-            file_type=df_params.df_params.file_type,
-            schema=schema,
-        )
+        if df_params.df_params.is_previous_date:
+            logger.info("Previous date flag is set. Attempting to read DataFrame from previous date.")
+            try:
+                df = self.spark_manager.read(
+                    env=read_params.bucket_params.env,
+                    path=path,
+                    file_type=df_params.df_params.file_type,
+                    schema=schema,
+                )
+            except Exception as e:
+                logger.error(f"Error reading DataFrame from previous date: {e}.")
+                raise ReadPreviousDayException
+        else:
+            df = self.spark_manager.read(
+                env=read_params.bucket_params.env,
+                path=path,
+                file_type=df_params.df_params.file_type,
+                schema=schema,
+            )
 
         return df
 
     def write_schema(
         self, df: DataFrame, write_params: DataFrameReadWriteParams
     ) -> None:
         """
@@ -399,15 +413,23 @@
         self, input_df_params_dict: InputDataFrameParamsDict
     ) -> DataFrameDict:
         """Reads multiple input dataframes based on the provided configuration."""
         dfs: DataFrameDict = {}
 
         for df_name, input_df_params in input_df_params_dict.items():
             logger.info(f"Starting read operation for DataFrame '{df_name}'...")
-            dfs[df_name] = self.read_dataframe(df_params=input_df_params)
+
+            try:
+                dfs[df_name] = self.read_dataframe(df_params=input_df_params)
+            except ReadPreviousDayException:
+                logger.warning(
+                    f"DataFrame '{df_name}' not found for previous date. Skipping..."
+                )
+                continue
+
             logger.info(f"Dataframe '{df_name}' read successfully.\n")
 
         return dfs
 
     def _select_transformation_function(self, transform_params: TransformParams):
         """Select the transformation function based on direct or indirect reference."""
         if transform_params.transform_function:
@@ -485,19 +507,21 @@
 
     def inject_processing_date_into_dataframe_params(
         self,
         params: Union[DataFrameReadWriteParams, DataFrameReadWriteParams],
         processing_date: datetime,
     ) -> Union[DataFrameReadWriteParams, DataFrameReadWriteParams]:
         modified_params = params
+        modified_params.is_previous_date = False
 
         if params.processing_date == "{{processing_date}}":
             modified_params.processing_date = processing_date
         elif params.processing_date == "{{processing_date_previous}}":
             modified_params.processing_date = processing_date - timedelta(days=1)
+            modified_params.is_previous_date = True
 
         return modified_params
 
     def inject_processing_date_into_step_params(
         self, step_params: StepParams, processing_date: datetime
     ) -> StepParams:
         modified_step_params = step_params
```

### Comparing `ng_data_pipelines_sdk-0.6.2/ng_data_pipelines_sdk/interfaces.py` & `ng_data_pipelines_sdk-0.7.0/ng_data_pipelines_sdk/interfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,25 @@
 DATE_FORMATTER = {
     "year": lambda x: str(x.year),
     "month": lambda x: str(x.month).zfill(2),
     "day": lambda x: str(x.day).zfill(2),
 }
 
 
+class ReadPreviousDayException(Exception):
+    """
+    Exception raised when the dataframe from the previous day is not found.
+    """
+
+    def __init__(self, message: str = "Dataframe from the previous day not found"):
+        self.message = message
+        super().__init__(self.message)
+
+
+
 class FileType(str, Enum):
     """
     Represents the type of file used in data pipelines.
 
     Attributes:
         CSV (str): Represents a CSV file.
         JSON (str): Represents a JSON file.
@@ -220,14 +231,15 @@
         datetime,
         Literal["{{processing_date}}"],
         Literal["{{processing_date_previous}}"],
     ] = "{{processing_date}}"
     processing_date_partitions: Optional[List[DatePartition]] = None
     processing_date_partitions_first: bool = True
     column_partitions: Optional[List[str]] = None
+    is_previous_date: bool = False
 
     @model_validator(mode="before")
     def xor_specific_path_and_path_to_dataframe_root(cls, data):
         """
         Validates that 'specific_path' and 'path_to_dataframe_root' are not passed together.
 
         Args:
```

### Comparing `ng_data_pipelines_sdk-0.6.2/ng_data_pipelines_sdk/spark_manager.py` & `ng_data_pipelines_sdk-0.7.0/ng_data_pipelines_sdk/spark_manager.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.6.2/ng_data_pipelines_sdk/utils.py` & `ng_data_pipelines_sdk-0.7.0/ng_data_pipelines_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.6.2/pyproject.toml` & `ng_data_pipelines_sdk-0.7.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ng-data-pipelines-sdk"
-version = "0.6.2"
+version = "0.7.0"
 description = "A library for facilitating the development of data engineering pipelines using pyspark. Compatible with MWAA running airflow 2.8.1."
 authors = ["ng.cash"]
 readme = "README.md"
 exclude = [".git/", ".gitignore", "tests/", "docs/", "*.yml", "__pycache__/", "*.pyc", "*.ipynb", "playground/", "poetry.lock", "dist/", "build/"]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
```

### Comparing `ng_data_pipelines_sdk-0.6.2/PKG-INFO` & `ng_data_pipelines_sdk-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ng-data-pipelines-sdk
-Version: 0.6.2
+Version: 0.7.0
 Summary: A library for facilitating the development of data engineering pipelines using pyspark. Compatible with MWAA running airflow 2.8.1.
 Author: ng.cash
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

