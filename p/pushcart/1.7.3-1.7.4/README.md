# Comparing `tmp/pushcart-1.7.3.tar.gz` & `tmp/pushcart-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pushcart-1.7.3.tar", max compression
+gzip compressed data, was "pushcart-1.7.4.tar", max compression
```

## Comparing `pushcart-1.7.3.tar` & `pushcart-1.7.4.tar`

### file list

```diff
@@ -1,20 +1,14 @@
--rw-r--r--   0        0        0    35149 2023-07-08 07:35:44.283369 pushcart-1.7.3/LICENSE
--rw-r--r--   0        0        0     1261 2023-08-17 15:15:20.240759 pushcart-1.7.3/README.md
--rw-r--r--   0        0        0        0 2023-07-13 21:50:18.218490 pushcart-1.7.3/pushcart/__init__.py
--rw-r--r--   0        0        0      580 2023-07-13 21:50:18.218490 pushcart-1.7.3/pushcart/log_handlers/__init__.py
--rw-r--r--   0        0        0      745 2023-08-16 08:15:49.386789 pushcart-1.7.3/pushcart/log_handlers/app_insights_handler.py
--rw-r--r--   0        0        0     5969 2023-07-13 21:50:18.218490 pushcart-1.7.3/pushcart/log_handlers/delta_table_handler.py
--rw-r--r--   0        0        0      124 2023-08-16 13:41:54.897464 pushcart-1.7.3/pushcart/metadata/__init__.py
--rw-r--r--   0        0        0    15152 2023-08-16 13:41:54.900798 pushcart-1.7.3/pushcart/metadata/metadata.py
--rw-r--r--   0        0        0     6672 2023-08-17 14:53:41.054046 pushcart-1.7.3/pushcart/metadata/spark.py
--rw-r--r--   0        0        0     5295 2023-07-13 21:50:18.218490 pushcart-1.7.3/pushcart/plugins.py
--rw-r--r--   0        0        0        0 2023-07-28 10:32:58.383848 pushcart-1.7.3/pushcart/sources/rest_api/__init__.py
--rw-r--r--   0        0        0    14430 2023-08-16 08:15:49.386789 pushcart-1.7.3/pushcart/sources/rest_api/request.py
--rw-r--r--   0        0        0     3223 2023-07-28 10:32:58.383848 pushcart-1.7.3/pushcart/sources/rest_api/spark.py
--rw-r--r--   0        0        0        0 2023-08-17 14:53:41.054046 pushcart-1.7.3/pushcart/transformations/__init__.py
--rw-r--r--   0        0        0        0 2023-08-17 14:53:41.054046 pushcart-1.7.3/pushcart/transformations/split_nested/__init__.py
--rw-r--r--   0        0        0     1712 2023-08-17 14:53:41.054046 pushcart-1.7.3/pushcart/transformations/split_nested/dlt.py
--rw-r--r--   0        0        0     9707 2023-08-17 14:53:41.054046 pushcart-1.7.3/pushcart/transformations/split_nested/spark.py
--rw-r--r--   0        0        0     2544 2023-08-16 13:41:54.900798 pushcart-1.7.3/pushcart/utils.py
--rw-r--r--   0        0        0     2676 2023-08-18 07:45:00.660030 pushcart-1.7.3/pyproject.toml
--rw-r--r--   0        0        0     2477 1970-01-01 00:00:00.000000 pushcart-1.7.3/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-05-15 13:46:20.244227 pushcart-1.7.4/LICENSE.txt
+-rw-r--r--   0        0        0     1261 2024-05-15 13:46:20.244227 pushcart-1.7.4/README.md
+-rw-r--r--   0        0        0     4110 2024-05-16 08:10:55.356923 pushcart-1.7.4/pyproject.toml
+-rw-r--r--   0        0        0       51 2024-05-15 13:46:20.244227 pushcart-1.7.4/src/pushcart/__init__.py
+-rw-r--r--   0        0        0      599 2024-05-15 13:46:20.244227 pushcart-1.7.4/src/pushcart/log_handlers/__init__.py
+-rw-r--r--   0        0        0     1077 2024-05-15 13:46:20.244227 pushcart-1.7.4/src/pushcart/log_handlers/app_insights_handler.py
+-rw-r--r--   0        0        0      124 2024-05-15 13:46:20.244227 pushcart-1.7.4/src/pushcart/metadata/__init__.py
+-rw-r--r--   0        0        0    17893 2024-05-16 07:08:22.680127 pushcart-1.7.4/src/pushcart/metadata/metadata.py
+-rw-r--r--   0        0        0     6873 2024-05-15 13:46:20.244227 pushcart-1.7.4/src/pushcart/metadata/spark.py
+-rw-r--r--   0        0        0        0 2024-05-15 13:46:20.244227 pushcart-1.7.4/src/pushcart/py.typed
+-rw-r--r--   0        0        0      109 2024-05-15 13:46:20.244227 pushcart-1.7.4/src/pushcart/sources/__init__.py
+-rw-r--r--   0        0        0    19054 2024-05-15 13:46:20.244227 pushcart-1.7.4/src/pushcart/sources/rest_api.py
+-rw-r--r--   0        0        0     2615 2024-05-15 13:46:20.244227 pushcart-1.7.4/src/pushcart/utils.py
+-rw-r--r--   0        0        0     2345 1970-01-01 00:00:00.000000 pushcart-1.7.4/PKG-INFO
```

### Comparing `pushcart-1.7.3/README.md` & `pushcart-1.7.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 # pushcart
 
 Helps with moving potatoes, bricks and data around.
 
-Pushcart is a metadata-based solution accelerator running on top of Spark. It also provides a set of ready-made functionalities for data transformations which might otherwise take a lot of code to put together using only `pyspark.sql.functions`.
+Pushcart is a metadata-based solution accelerator running on top of Spark. It
+also provides a set of ready-made functionalities for data transformations which
+might otherwise take a lot of code to put together using only
+`pyspark.sql.functions`.
 
 ## Who is this for
 
 - Data engineers writing pure Spark code
 - Data engineers working with Databricks Delta Live Tables
 
 ## How does the metadata look like?
 
-Useful for transforming data from bronze to silver, a metadata specification looks as such:
+Useful for transforming data from bronze to silver, a metadata specification
+looks as such:
 
 column_order|source_column_name|source_column_type|dest_column_name|dest_column_type|transform_function|default_value|validation_rule|validation_action
 ------------|------------------|------------------|----------------|----------------|------------------|-------------|---------------|-----------------
 0|id|string|Id|int|||Id IS NOT NULL|DROP
 1|first_name|string||||||
 2|surname|string||||||
 3|||Name|string|"F.concat_ws(' ', F.col('first_name'), F.col('surname'))",F.lit('John Doe')||
```

### Comparing `pushcart-1.7.3/pushcart/log_handlers/app_insights_handler.py` & `pushcart-1.7.4/src/pushcart/log_handlers/app_insights_handler.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,37 @@
+"""Log handler for Application Insights."""
+
 import logging
 
-from azure.monitor.opentelemetry.exporter import AzureMonitorLogExporter
-from opentelemetry.sdk._logs import LoggerProvider, LoggingHandler
-from opentelemetry.sdk._logs.export import BatchLogRecordProcessor
+from azure.monitor.opentelemetry.exporter import (  # type: ignore[import-not-found]
+    AzureMonitorLogExporter,
+)
+from opentelemetry.sdk._logs import (  # type: ignore[import-not-found]
+    LoggerProvider,
+    LoggingHandler,
+)
+from opentelemetry.sdk._logs.export import (  # type: ignore[import-not-found]
+    BatchLogRecordProcessor,
+)
 
 
 class ApplicationInsightsHandler(LoggingHandler):
+    """Log handler class for Application Insights.
+
+    Args:
+    ----
+        LoggingHandler (_type_): Python SDK LoggingHandler class
+
+    """
+
     def __init__(
         self,
         connection_string: str,
         level: int = logging.NOTSET,
-        logger_provider: LoggerProvider = None,
+        logger_provider: LoggerProvider | None = None,
     ) -> None:
         logger_provider = logger_provider or LoggerProvider()
         exporter = AzureMonitorLogExporter(connection_string=connection_string)
         logger_provider.add_log_record_processor(
-            BatchLogRecordProcessor(exporter=exporter)
+            BatchLogRecordProcessor(exporter=exporter),
         )
         super().__init__(level, logger_provider)
```

### Comparing `pushcart-1.7.3/pushcart/metadata/metadata.py` & `pushcart-1.7.4/src/pushcart/metadata/metadata.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,46 @@
 """Generate and edit metadata based on an input Spark DataFrame."""
 
 from __future__ import annotations
 
 import contextlib
+from typing import TYPE_CHECKING, Any
 
+import numpy as np
 import pandas as pd
-import pyspark.sql.functions as F  # noqa: N812
-import pyspark.sql.types as T  # noqa: N812
+import pyspark.sql.functions as F
+import pyspark.sql.types as T
 from dateutil.parser import ParserError
-from ipydatagrid import DataGrid
+from ipydatagrid import DataGrid  # type: ignore[import, import-untyped]
 from IPython.display import display
-from ipywidgets import Button, HBox, VBox
+from ipywidgets import Button, HBox, VBox  # type: ignore[import, import-untyped]
 from loguru import logger
-from pandas.core.tools.datetimes import _guess_datetime_format_for_array
-from pyspark.sql import DataFrame, SparkSession
+from pandas.core.tools.datetimes import (  # type: ignore[attr-defined]
+    _guess_datetime_format_for_array,
+)
+from pyspark.sql import DataFrame, Row, SparkSession
 from pyspark.sql.window import Window
 
 from pushcart.metadata.spark import generate_code as sp_generate_code
 from pushcart.metadata.spark import transform as sp_transform
 from pushcart.utils import pandas_to_spark_datetime_pattern
 
+if TYPE_CHECKING:
+    from collections.abc import Hashable
 
-def __get_spark_session() -> SparkSession:
-    return SparkSession.getActiveSession() or SparkSession.newSession()
 
-
-def _infer_json_schema(df: DataFrame, column_name: str) -> str:
+def _infer_json_schema(
+    df: DataFrame,
+    column_name: str,
+    spark: SparkSession | None = None,
+) -> str | None:
     logger.info(f"Attempting to infer JSON schema for {column_name} column.")
 
-    spark = __get_spark_session()
+    if not spark:
+        spark = SparkSession.builder.getOrCreate()
     schema = spark.read.json(df.select(column_name).rdd.map(lambda x: x[0])).schema
 
     if schema.fieldNames() == ["_corrupt_record"]:
         logger.warning(f"Could not infer JSON schema for {column_name} column.")
         return None
 
     if "_corrupt_record" in schema.fieldNames():
@@ -41,15 +49,15 @@
                 T.StructField("_corrupt_record", T.StringType(), nullable=True),
             ),
         )
 
     return f'F.from_json(F.col("{column_name}"), schema="{schema.simpleString()}")'
 
 
-def _infer_timestamps(df: DataFrame, column_name: str) -> str:
+def _infer_timestamps(df: DataFrame, column_name: str) -> str | None:
     logger.info(f"Attempting to infer timestamp format for {column_name} column.")
 
     pd_ts_format = None
 
     with contextlib.suppress(ParserError, AttributeError, TypeError):
         pd_ts_df = df.select(column_name).dropna().limit(1).toPandas()
         # Pandas keeps the last bit of the field path as column name
@@ -62,15 +70,19 @@
         return None
 
     spark_ts_format = pandas_to_spark_datetime_pattern(pd_ts_format)
 
     return f'F.to_timestamp(F.col("{column_name}"), "{spark_ts_format}")'
 
 
-def get_unique_values(df: DataFrame, max_rows: int = None) -> DataFrame:
+def get_unique_values(
+    df: DataFrame,
+    max_rows: int | None = None,
+    spark: SparkSession | None = None,
+) -> DataFrame:
     """Get a dataframe with only per-column unique values for inference.
 
     Useful for more accurately inferring metadata for some datasets.
     Can take a long time to run, but will also reduce the runtime for
     `Metadata` generation if used as its input.
 
     This method will break the inter-column consistency of records, since
@@ -100,32 +112,38 @@
     Parameters
     ----------
     df : DataFrame
         Spark DataFrame containing data to be analyzed
     max_rows : int, optional
         Number of unique values to bring in per column, by default None.
         If not specified, max_rows will use the total record count of `df`
+    spark: SparkSession, optional
+        Optionally provide an existing SparkSession, by default None
 
     Returns
     -------
     DataFrame
         Spark DataFrame containing per-column unique data
+
     """
     if not df:
-        return None
+        msg = "Parameter `df` must be a Spark DataFrame"
+        raise ValueError(msg)
+
+    if not spark:
+        spark = SparkSession.builder.getOrCreate()
 
-    spark = __get_spark_session()
     if df.isEmpty():
         return spark.createDataFrame([], df.schema)
 
     if not max_rows:
-        max_rows - df.count()
+        max_rows = df.count() or 0
 
     unique_vals_df: DataFrame = spark.createDataFrame(
-        [{"_row_index": r} for r in range(1, max_rows)],
+        [Row(_row_index=r) for r in range(1, max_rows)],
     )
 
     for c in df.columns:
         unique_vals_df = unique_vals_df.join(
             df.select(c)
             .distinct()
             .limit(max_rows)
@@ -147,15 +165,15 @@
 
 
 class Metadata:
     """Generate metadata and transformations based on input DataFrame."""
 
     def __init__(
         self,
-        df: DataFrame,
+        df: DataFrame | None,
         infer_json_schema: bool = True,
         infer_timestamps: bool = True,
         infer_fraction: float = 0.25,
     ) -> None:
         """Generate metadata and transformations based on input DataFrame.
 
         Parameters
@@ -164,22 +182,23 @@
             PySpark DataFrame for which metadata is generated
         infer_json_schema : bool, optional
             Whether to infer the schema of JSON string columns or not, by default True
         infer_timestamps : bool, optional
             Whether to try to infer timestamp string column formats, by default True
         infer_fraction : float, optional
             The fraction of data that is sampled from the input, by default 0.25
+
         """
         self.data_df = df
 
         self.infer_json_schema = infer_json_schema
         self.infer_timestamps = infer_timestamps
         self.infer_fraction = infer_fraction
 
-        self.metadata_df: pd.DataFrame = None
+        self.metadata_df: pd.DataFrame | None = None
         self.metadata_grid: DataGrid = None
 
         self.metadata_cols = [
             "column_order",
             "source_column_name",
             "source_column_type",
             "dest_column_name",
@@ -202,22 +221,67 @@
             Optionally, attach an actual dataset to the Metadata object for running
             transformations on it automatically, by default None
 
         Returns
         -------
         Metadata
             Object allowing to visualize, edit, and generate PySpark code from metadata.
+
         """
         md = Metadata(df=None)
         md.metadata_df = pd.read_csv(path)
         md.data_df = data_df
 
         return md
 
+    @classmethod
+    def from_df(
+        cls,
+        metadata_df: pd.DataFrame | DataFrame,
+        data_df: DataFrame | None = None,
+    ) -> Metadata:
+        """Load metadata from an in-memory DataFrame, without the original dataset.
+
+        Parameters
+        ----------
+        metadata_df : pd.DataFrame | DataFrame
+            DataFrame object containing metadata and transformations.
+        data_df : DataFrame | None, optional
+            Optionally, attach an actual dataset to the Metadata object for running
+            transformations on it automatically, by default None
+
+        Returns
+        -------
+        Metadata
+            Object allowing to visualize, edit, and generate PySpark code from metadata.
+
+        Raises
+        ------
+        TypeError
+            metadata_df must be a pandas or Spark DataFrame
+
+        """
+        md = Metadata(df=None)
+        if not isinstance(metadata_df, pd.DataFrame | DataFrame):
+            msg = "metadata_df must be a pandas or Spark DataFrame"
+            raise TypeError(msg)
+        md.metadata_df = (
+            pd.DataFrame(metadata_df.toPandas()).fillna(value=np.nan)
+            if isinstance(metadata_df, DataFrame)
+            else metadata_df
+        )
+        md.data_df = data_df
+
+        return md
+
     def _infer(self, column_name: str) -> str:
+        if not self.data_df:
+            msg = "Cannot infer metadata since no Spark DataFrame has been provided."
+            raise ValueError(msg)
+
         sampled_df = self.data_df.sample(
             fraction=self.infer_fraction,
             withReplacement=False,
         )
 
         inferred_ts = None
         inferred_schema = None
@@ -230,40 +294,46 @@
         if self.infer_json_schema:
             inferred_schema = _infer_json_schema(sampled_df, column_name)
             if inferred_schema:
                 return inferred_schema
 
         return ""
 
-    def _generate_field(self, field: T.StructField, parent: str = None) -> dict:
+    def _generate_field(self, field: T.StructField, parent: str | None = None) -> dict:
         name = field.name
         dtype = field.dataType
         flat_parent = parent.replace(".", "_") if parent else None
         return {
             "source_column_name": f"{flat_parent}.{name}" if parent else name,
             "source_column_type": dtype.simpleString(),
             "dest_column_name": f"{flat_parent}_{name}" if parent else name,
-            "dest_column_type": dtype.elementType.simpleString()
-            if isinstance(dtype, T.ArrayType)
-            else dtype.simpleString(),
+            "dest_column_type": (
+                dtype.elementType.simpleString()
+                if isinstance(dtype, T.ArrayType)
+                else dtype.simpleString()
+            ),
             "transform_function": (
-                f'F.explode("{flat_parent}.{name}")'
-                if parent
-                else f'F.explode("{name}")'
-            )
-            if isinstance(dtype, T.ArrayType)
-            else self._infer(f"{parent}.{name}" if parent else name)
-            if isinstance(dtype, T.StringType)
-            else "",
+                (
+                    f'F.explode("{flat_parent}.{name}")'
+                    if parent
+                    else f'F.explode("{name}")'
+                )
+                if isinstance(dtype, T.ArrayType)
+                else (
+                    self._infer(f"{parent}.{name}" if parent else name)
+                    if isinstance(dtype, T.StringType)
+                    else ""
+                )
+            ),
             "default_value": "",
             "validation_rule": "",
             "validation_action": "",
         }
 
-    def _generate(self, schema: T.StructType, parent: str = None) -> list:
+    def _generate(self, schema: T.StructType, parent: str | None = None) -> list:
         fields = []
 
         for f in schema.fields:
             dtype = f.dataType
 
             field_name = f"{parent + '.' if parent else ''}{f.name}"
 
@@ -286,14 +356,15 @@
     def generate(self) -> pd.DataFrame:
         """Generate a Pandas DataFrame containing the metadata for the dataset being analyzed.
 
         Returns
         -------
         pd.DataFrame
             Pandas DataFrame containing proposed transformation metadata
+
         """
         if self.data_df is None:
             msg = "Cannot generate new metadata since no Spark DataFrame has been provided."
             raise ValueError(msg)
 
         metadata = pd.DataFrame(
             self._generate(self.data_df.schema, parent=None),
@@ -323,14 +394,15 @@
     def visualize(self) -> None:
         """Show the generated metadata and allow user editing.
 
         Raises
         ------
         ValueError
             Can only show the metadata if it is present in memory.
+
         """
         if self.metadata_df is None:
             msg = "Cannot visualize metadata as it has not yet been generated/loaded."
             raise ValueError(msg)
 
         self.metadata_grid = DataGrid(self.metadata_df, editable=True)
         self.metadata_grid.auto_fit_params = {"area": "all"}
@@ -343,34 +415,48 @@
         remove_row_button = Button(description="Remove Row")
         remove_row_button.on_click(self._on_remove_row)
 
         layout = VBox([HBox([add_row_button, remove_row_button]), self.metadata_grid])
 
         display(layout)
 
-    def get_metadata(self) -> None:
-        """Generate new metadata for the provided dataset and visualize it."""
+    def get_metadata(self, show: bool = True) -> None:
+        """Generate new metadata for the provided dataset and visualize it.
+
+        Parameters
+        ----------
+        show : bool
+            Display metadata editor in a notebook.
+
+        """
         self.metadata_df = self.generate()
-        self.visualize()
+
+        if show:
+            self.visualize()
 
     def save_to_csv(self, path: str) -> None:
         """Save the current version of the metadata to a CSV file.
 
         Parameters
         ----------
         path : str
             File path to save to
+
         """
+        if not self.metadata_df:
+            msg = "Cannot save metadata as it has not yet been generated/loaded."
+            raise ValueError(msg)
+
         self.metadata_df.to_csv(path)
         logger.info(f"Wrote {len(self.metadata_df.index)} lines to {path}")
 
     @staticmethod
     def _keep_dest_cols(metadata_df: pd.DataFrame) -> pd.DataFrame:
         has_dest_col = (metadata_df["dest_column_name"].isna()) | (
-            metadata_df["dest_column_name"] == ""  # noqa: PLC1901
+            metadata_df["dest_column_name"] == ""
         )
         return metadata_df.loc[~has_dest_col]
 
     @staticmethod
     def _drop_technical_cols(metadata_df: pd.DataFrame) -> pd.DataFrame:
         tech_cols = metadata_df["dest_column_name"].str.startswith("_")
 
@@ -380,44 +466,49 @@
         logger.info(f"Excluding technical columns: {excluded_columns}")
 
         return metadata_df.loc[~tech_cols]
 
     def _prepare_metadata(
         self,
         keep_technical_cols: bool = False,
-    ) -> tuple[pd.DataFrame, list[str]]:
+    ) -> tuple[list[dict[Hashable, Any]], list[str]]:
         """Parse the metadata and keep or drop technical columns (starting with underscore).
 
         Parameters
         ----------
         keep_technical_cols : bool, optional
             Generate transformations for columns whose names start with underscore, by default False
 
         Returns
         -------
         tuple[pd.DataFrame, list[str]]
-            Pandas DataFrame with the final set of pending transformations and list of columns to keep.
+            DataFrame with the final set of pending transformations and list of columns to keep.
 
         Raises
         ------
         ValueError
             Can only generate code based on metadata that is present in memory.
+
         """
         if self.metadata_df is None:
             msg = "Cannot generate PySpark code from empty metadata."
             raise ValueError(msg)
 
         mdf = self._keep_dest_cols(self.metadata_df)
 
         dest_cols = [col for col in mdf["dest_column_name"].to_list() if col] or None
         if not dest_cols:
             logger.warning(
-                "No destination columns defined in metadata. No code to generate.",
+                "No destination columns defined in metadata. Using source column names.",
             )
-            return None
+            dest_cols = [col for col in mdf["source_column_name"].to_list() if col]
+
+        if not dest_cols:
+            msg = "Cannot generate PySpark code from empty metadata."
+            raise ValueError(msg)
 
         if not keep_technical_cols:
             mdf = self._drop_technical_cols(mdf)
 
         return mdf.sort_values(by=["column_order"]).to_dict(orient="records"), dest_cols
 
     def generate_code(self, keep_technical_cols: bool = False) -> str | None:
@@ -428,14 +519,15 @@
         keep_technical_cols : bool, optional
             Generate transformations for columns whose names start with underscore, by default False
 
         Returns
         -------
         str | None
             String containing runnable PySpark code
+
         """
         transformations, dest_cols = self._prepare_metadata(keep_technical_cols)
 
         return sp_generate_code(transformations, dest_cols)
 
     def transform(self, keep_technical_cols: bool = False) -> DataFrame:
         """Perform the transformations configured in the metadata table.
@@ -445,11 +537,16 @@
         keep_technical_cols : bool, optional
             Generate transformations for columns whose names start with underscore, by default False
 
         Returns
         -------
         DataFrame
             Spark DataFrame containing the transformed data
+
         """
+        if not self.data_df:
+            msg = "Cannot perform transformations since no Spark DataFrame has been provided."
+            raise ValueError(msg)
+
         transformations, dest_cols = self._prepare_metadata(keep_technical_cols)
 
         return sp_transform(self.data_df, transformations, dest_cols)
```

### Comparing `pushcart-1.7.3/pushcart/metadata/spark.py` & `pushcart-1.7.4/src/pushcart/metadata/spark.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 """PySpark transformations and code generation."""
 
-import pandas as pd
-import pyspark.sql.functions as F  # noqa: N812
+from collections.abc import Hashable
+from typing import Any
+
+import pyspark.sql.functions as F
 from loguru import logger
 from pyspark.sql import Column, DataFrame
 
 
-def generated_col_or_transform(transformation_step: str) -> str:
+def generated_col_or_transform(transformation_step: dict[Hashable, Any]) -> str:
     """Generate column or transformation function based on the transformation step.
 
     Parameters
     ----------
     transformation_step : dict
         Dictionary containing transformation information.
 
     Returns
     -------
     str
         Column name or transformation function as a string.
+
     """
     if (
         isinstance(transformation_step["transform_function"], str)
         and len(transformation_step["transform_function"]) > 0
     ):
         return transformation_step["transform_function"]
 
     return f"F.col(\"{transformation_step['source_column_name']}\")"
 
 
 def generated_transform_with_default(
-    transformation_step: str,
+    transformation_step: dict[Hashable, Any],
     col_or_transf: str,
 ) -> str:
     """Generate transformation with default value if specified.
 
     Parameters
     ----------
     transformation_step : dict
@@ -41,14 +44,15 @@
     col_or_transf : str
         Column name or transformation function as a string.
 
     Returns
     -------
     str
         Column or transformation function with default value if specified.
+
     """
     if (
         isinstance(transformation_step["default_value"], str)
         and len(transformation_step["default_value"]) > 0
     ):
         default_value = generated_cast_or_original_dtype(
             transformation_step,
@@ -56,30 +60,31 @@
         )
         return f"F.coalesce({col_or_transf}, {default_value})"
 
     return col_or_transf
 
 
 def generated_cast_or_original_dtype(
-    transformation_step: str,
-    col_or_transf: Column,
-) -> Column:
+    transformation_step: dict[Hashable, Any],
+    col_or_transf: str,
+) -> str:
     """Cast to the destination type or return the original column based on the transformation step.
 
     Parameters
     ----------
     transformation_step : dict
         Dictionary containing transformation information.
-    col_or_transf : Column
-        PySpark Column object.
+    col_or_transf : str
+        PySpark Column name.
 
     Returns
     -------
     Column
-        PySpark Column object, casted or original.
+        PySpark Column name, casted or original.
+
     """
     if (
         transformation_step["source_column_type"]
         != transformation_step["dest_column_type"]
     ) and (
         all(
             dtype not in transformation_step["dest_column_type"]
@@ -87,28 +92,32 @@
         )
     ):
         return f"{col_or_transf}.cast(\"{transformation_step['dest_column_type']}\")"
 
     return col_or_transf
 
 
-def generate_code(transformations: pd.DataFrame, dest_cols: list[str]) -> str:
+def generate_code(
+    transformations: list[dict[Hashable, Any]],
+    dest_cols: list[str],
+) -> str:
     """Generate PySpark transformation code based on existing metadata.
 
     Parameters
     ----------
     transformations : pd.DataFrame
         Pandas DataFrame containing the transformation metadata.
     dest_cols : list of str
         List of destination column names to select in the output DataFrame.
 
     Returns
     -------
     str
         String containing runnable PySpark code
+
     """
     code_lines = ["df = (df"]
 
     for t in transformations:
         col = generated_col_or_transform(t)
         col = generated_transform_with_default(t, col)
         col = generated_cast_or_original_dtype(t, col)
@@ -119,38 +128,41 @@
     code_str = "\n" + "\n".join(code_lines)
 
     logger.info(code_str)
 
     return code_str
 
 
-def col_or_transform(transformation_step: str) -> Column:
+def col_or_transform(transformation_step: dict[Hashable, Any]) -> Column:
     """Evaluate column or transformation function based on the transformation step.
 
     Parameters
     ----------
     transformation_step : dict
         Dictionary containing transformation information.
 
     Returns
     -------
     Column
         PySpark Column object.
+
     """
     if (
         isinstance(transformation_step["transform_function"], str)
         and len(transformation_step["transform_function"]) > 0
     ):
-        return eval(transformation_step["transform_function"])  # noqa: PGH001
+        return eval(  # pylint: disable=W0123  # noqa: S307
+            transformation_step["transform_function"],
+        )
 
     return F.col(transformation_step["source_column_name"])
 
 
 def transform_with_default(
-    transformation_step: str,
+    transformation_step: dict[Hashable, Any],
     col_or_transf: Column,
 ) -> Column:
     """Apply transformation with default value if specified.
 
     Parameters
     ----------
     transformation_step : dict
@@ -158,14 +170,15 @@
     col_or_transf : Column
         PySpark Column object.
 
     Returns
     -------
     Column
         PySpark Column object with default value applied if specified.
+
     """
     if (
         isinstance(transformation_step["default_value"], str)
         and len(transformation_step["default_value"]) > 0
     ):
         return F.coalesce(
             col_or_transf,
@@ -175,15 +188,15 @@
             ),
         )
 
     return col_or_transf
 
 
 def cast_or_original_dtype(
-    transformation_step: str,
+    transformation_step: dict[Hashable, Any],
     col_or_transf: Column,
 ) -> Column:
     """Cast to the destination type or return the original column based on the transformation step.
 
     Parameters
     ----------
     transformation_step : dict
@@ -191,14 +204,15 @@
     col_or_transf : Column
         PySpark Column object.
 
     Returns
     -------
     Column
         PySpark Column object, casted or original.
+
     """
     if (
         transformation_step["source_column_type"]
         != transformation_step["dest_column_type"]
     ) and (
         all(
             dtype not in transformation_step["dest_column_type"]
@@ -208,15 +222,15 @@
         return col_or_transf.cast(transformation_step["dest_column_type"])
 
     return col_or_transf
 
 
 def transform(
     data_df: DataFrame,
-    transformations: pd.DataFrame,
+    transformations: list[dict[Hashable, Any]],
     dest_cols: list[str],
 ) -> DataFrame:
     """Perform the transformations configured in the metadata table on the input DataFrame.
 
     Parameters
     ----------
     data_df : DataFrame
@@ -226,14 +240,15 @@
     dest_cols : list of str
         List of destination column names to select in the output DataFrame.
 
     Returns
     -------
     DataFrame
         PySpark DataFrame containing the transformed data.
+
     """
     result_df = data_df
     for t in transformations:
         col = col_or_transform(t)
         col = transform_with_default(t, col)
         col = cast_or_original_dtype(t, col)
```

### Comparing `pushcart-1.7.3/pushcart/utils.py` & `pushcart-1.7.4/src/pushcart/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Utility functions for PushCart."""
+
 import re
 
 
 def _normalize_old(s: str, ignore_case: bool = False) -> str:
     return s.lower() if ignore_case else s
 
 
@@ -17,26 +19,27 @@
     ignore_case : bool, optional
         Whether to apply replacements ignoring case, by default False
 
     Returns
     -------
     str
         New string with substrings replaced
+
     """
     if not replacements:
         return string
 
     replacements = {_normalize_old(key): val for key, val in replacements.items()}
 
     # Place longer strings first to keep shorter substrings from matching where the
     # longer ones should be replaced. For instance, given the replacement map
     # {"ab": "AB", "abc", "ABC"} for the string "hey abc", it should produce
     # "hey ABC" and not "hey ABc"
     rep_sorted = sorted(replacements, key=len, reverse=True)
-    rep_escaped = map(re.escape, rep_sorted)
+    rep_escaped = [str(escaped) for escaped in map(re.escape, rep_sorted)]
 
     pattern = re.compile("|".join(rep_escaped), re.IGNORECASE if ignore_case else 0)
 
     return pattern.sub(
         lambda match: replacements[_normalize_old(match.group(0))],
         string,
     )
@@ -57,14 +60,15 @@
 
     Returns
     -------
     str
         The converted Spark datetime format pattern string.
         For example, given the input pattern "%Y-%m-%d %H:%M:%S",
         the function would return "yyyy-MM-dd HH:mm:ss".
+
     """
     replacement_map = {
         "%Y": "yyyy",
         "%y": "yy",
         "%m": "MM",
         "%B": "MMMM",
         "%b": "MMM",
```

### Comparing `pushcart-1.7.3/pyproject.toml` & `pushcart-1.7.4/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,135 +1,182 @@
+[tool.pyright]
+include = ["src", "tests"]
+ignore = ["**/.pyenv"]
+exclude = ["**/.pyenv"]
+
 [tool.black]
 line-length = 88
-target-version = ["py39"]
+target-version = ["py311"]
 exclude = '''
 (
   /(
       \.git
     | \.github
     | \.venv
   )/
 )
 '''
 
 [tool.ruff]
-select = ["ALL"]
-ignore = [
-  "ANN101", # Checks that instance method self arguments have type annotations
-  "ANN102", # Checks that class method cls arguments have type annotations
-  "D203",   # One blank line required before class docstring
-  "D213",   # Multi-line docstring summary should start at the second line
-  "E501",   # Line too long
-  "FBT001", # Boolean positional arg in function definition
-  "FBT002", # Boolean default value in function definition
-  "G004",   # Logging statement uses f-string
-  "S101",   # Use of `assert` detected
+lint.select = ["ALL"]
+lint.ignore = [
+    "ANN101", # Checks that instance method self arguments have type annotations
+    "ANN102", # Checks that class method cls arguments have type annotations
+    "D107",   # Missing docstring in __init__
+    "D203",   # One blank line required before class docstring
+    "D213",   # Multi-line docstring summary should start at the second line
+    "E501",   # Line too long
+    "FBT001", # Boolean positional arg in function definition
+    "FBT002", # Boolean default value in function definition
+    "G004",   # Logging statement uses f-string
+    "N812",   # Checks for lowercase imports that are aliased to non-lowercase names
+    "S101",   # Use of `assert` detected
 ]
-target-version = "py39"
+target-version = "py311"
 
 # Allow autofix for all enabled rules (when `--fix`) is provided.
-fixable = [
-  "A",
-  "B",
-  "C",
-  "D",
-  "E",
-  "F",
-  "G",
-  "I",
-  "N",
-  "Q",
-  "S",
-  "T",
-  "W",
-  "ANN",
-  "ARG",
-  "BLE",
-  "COM",
-  "DJ",
-  "DTZ",
-  "EM",
-  "ERA",
-  "EXE",
-  "FBT",
-  "ICN",
-  "INP",
-  "ISC",
-  "NPY",
-  "PD",
-  "PGH",
-  "PIE",
-  "PL",
-  "PT",
-  "PTH",
-  "PYI",
-  "RET",
-  "RSE",
-  "RUF",
-  "SIM",
-  "SLF",
-  "TCH",
-  "TID",
-  "TRY",
-  "UP",
-  "YTT",
+lint.fixable = [
+    "A",
+    "B",
+    "C",
+    "D",
+    "E",
+    "F",
+    "G",
+    "I",
+    "N",
+    "Q",
+    "S",
+    "T",
+    "W",
+    "ANN",
+    "ARG",
+    "BLE",
+    "COM",
+    "DJ",
+    "DTZ",
+    "EM",
+    "ERA",
+    "EXE",
+    "FBT",
+    "ICN",
+    "INP",
+    "ISC",
+    "NPY",
+    "PD",
+    "PGH",
+    "PIE",
+    "PL",
+    "PT",
+    "PTH",
+    "PYI",
+    "RET",
+    "RSE",
+    "RUF",
+    "SIM",
+    "SLF",
+    "TCH",
+    "TID",
+    "TRY",
+    "UP",
+    "YTT",
 ]
-unfixable = []
+lint.unfixable = []
 exclude = [".venv", "tests"]
+builtins = ["dbutils", "dlt", "display"]
+
+[tool.ruff.lint.per-file-ignores]
+"scratch/*" = ["D100", "E402", "ERA001", "INP001"]
+".vscode/__builtins__.pyi" = ["D100", "INP001"]
 
 [tool.poetry]
 name = "pushcart"
-version = "1.7.3"
+version = "1.7.4"
 description = "Metadata transformations for Spark"
-authors = ["Georgel Preput <georgelpreput@mailbox.org>"]
-license = "GPL-3.0-or-later"
+authors = ["Victor Blaga <victor.blaga@revodata.nl>"]
+license = "Apache-2.0"
 readme = "README.md"
 classifiers = [
-  "Programming Language :: Python :: 3.9",
-  "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
-  "Operating System :: OS Independent",
-  "Topic :: Database :: Database Engines/Servers",
-  "Topic :: Software Development :: Libraries :: Application Frameworks",
-  "Topic :: Software Development :: Libraries :: Python Modules",
+    "Programming Language :: Python :: 3.11",
+    "License :: OSI Approved :: Apache Software License",
+    "Operating System :: OS Independent",
+    "Topic :: Database :: Database Engines/Servers",
+    "Topic :: Software Development :: Libraries :: Application Frameworks",
+    "Topic :: Software Development :: Libraries :: Python Modules",
 ]
+packages = [{ include = "pushcart", from = "src" }]
 
 [tool.poetry.dependencies]
-authlib = "^1.2.1"
-httpx = "^0.24.1"
-ipydatagrid = "^1.1.16"
-ipywidgets = "^8.0.7"
-loguru = "^0.7.0"
-pandas = "^2.0.2"
-pyspark = "^3.4.1"
-python = "^3.9"
-python-dotenv = "^1.0.0"
-tqdm = "^4.65.0"
-validators = "^0.20.0"
+python-dotenv = "^1.0.1"
+python = "^3.11"
+loguru = "^0.7.2"
+azure-monitor-opentelemetry = "^1.4.0"
+opentelemetry-sdk = "^1.24.0"
+delta-spark = "^3.1.0"
+validators = "^0.28.1"
+httpx = "^0.27.0"
+authlib = "^1.3.0"
 
 [tool.poetry.group.dev.dependencies]
-black = { version = "*", allow-prereleases = true }
-bumpver = "^2023.1124"
-coverage = "^7.2.7"
-ipykernel = "^6.22.0"
-pytest = "^7.2.0"
-pytest-cov = "^4.0.0"
-pytest-mock = "^3.10.0"
-requests = "^2.31.0"
-ruff = "^0.0.265"
+# Matching DBR 15.0
+black = { version = "23.3.0", allow-prereleases = true }
+databricks-sdk = "0.20.0"
+ipykernel = "6.25.1"
+ipywidgets = "8.0.4"
+mypy-extensions = "^1.0.0"
+pandas = "2.0.3"
+pyarrow = "^14.0.1"
+pydantic = "1.10.6"
+
+# Not in DBR
+bumpver = "^2023.1129"
+coverage = "^7.5.0"
+databricks-labs-pylint = "^0.4.0"
+ipydatagrid = "^1.3.1"
+mypy = "^1.5.1"
+pandas-stubs = "^2.2.0.240218"
+pre-commit = "^3.5.0"
+pylint = "^3.1.0"
+pyspark = "^3.5.1"
+pytest = "^8.1.1"
+pytest-cov = "^5.0.0"
+pytest-mock = "^3.14.0"
+ruff = "^0.4.1"
+types-python-dateutil = "^2.9.0.20240316"
+types-decorator = "^5.1.8.20240310"
+types-protobuf = "^5.26.0.20240422"
+types-pytz = "^2024.1.0.20240417"
+types-requests = "^2.31.0.20240406"
+types-setuptools = "^69.5.0.20240423"
+types-six = "^1.16.21.20240425"
+types-ujson = "^5.9.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.bumpver]
-current_version = "1.7.3"
+current_version = "1.7.4"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
-  '^version = "{version}"$',
-  '^current_version = "{version}"$',
+    '^version = "{version}"$',
+    '^current_version = "{version}"$',
 ]
+
+[tool.mypy]
+python_version = "3.11"
+ignore_missing_imports = true
+mypy_path = "./stubs"
+files = "src/**/*.py, tests/**/*.py"
+exclude = [".venv/"]
+pretty = true
+
+[[tool.mypy.overrides]]
+module = ["dbutils", "dlt", "display"]
+ignore_missing_imports = true
+disable_error_code = ["name-defined"]
```

### Comparing `pushcart-1.7.3/PKG-INFO` & `pushcart-1.7.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 Metadata-Version: 2.1
 Name: pushcart
-Version: 1.7.3
+Version: 1.7.4
 Summary: Metadata transformations for Spark
-License: GPL-3.0-or-later
-Author: Georgel Preput
-Author-email: georgelpreput@mailbox.org
-Requires-Python: >=3.9,<4.0
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+License: Apache-2.0
+Author: Victor Blaga
+Author-email: victor.blaga@revodata.nl
+Requires-Python: >=3.11,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Database :: Database Engines/Servers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: authlib (>=1.2.1,<2.0.0)
-Requires-Dist: httpx (>=0.24.1,<0.25.0)
-Requires-Dist: ipydatagrid (>=1.1.16,<2.0.0)
-Requires-Dist: ipywidgets (>=8.0.7,<9.0.0)
-Requires-Dist: loguru (>=0.7.0,<0.8.0)
-Requires-Dist: pandas (>=2.0.2,<3.0.0)
-Requires-Dist: pyspark (>=3.4.1,<4.0.0)
-Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
-Requires-Dist: tqdm (>=4.65.0,<5.0.0)
-Requires-Dist: validators (>=0.20.0,<0.21.0)
+Requires-Dist: authlib (>=1.3.0,<2.0.0)
+Requires-Dist: azure-monitor-opentelemetry (>=1.4.0,<2.0.0)
+Requires-Dist: delta-spark (>=3.1.0,<4.0.0)
+Requires-Dist: httpx (>=0.27.0,<0.28.0)
+Requires-Dist: loguru (>=0.7.2,<0.8.0)
+Requires-Dist: opentelemetry-sdk (>=1.24.0,<2.0.0)
+Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
+Requires-Dist: validators (>=0.28.1,<0.29.0)
 Description-Content-Type: text/markdown
 
 # pushcart
 
 Helps with moving potatoes, bricks and data around.
 
-Pushcart is a metadata-based solution accelerator running on top of Spark. It also provides a set of ready-made functionalities for data transformations which might otherwise take a lot of code to put together using only `pyspark.sql.functions`.
+Pushcart is a metadata-based solution accelerator running on top of Spark. It
+also provides a set of ready-made functionalities for data transformations which
+might otherwise take a lot of code to put together using only
+`pyspark.sql.functions`.
 
 ## Who is this for
 
 - Data engineers writing pure Spark code
 - Data engineers working with Databricks Delta Live Tables
 
 ## How does the metadata look like?
 
-Useful for transforming data from bronze to silver, a metadata specification looks as such:
+Useful for transforming data from bronze to silver, a metadata specification
+looks as such:
 
 column_order|source_column_name|source_column_type|dest_column_name|dest_column_type|transform_function|default_value|validation_rule|validation_action
 ------------|------------------|------------------|----------------|----------------|------------------|-------------|---------------|-----------------
 0|id|string|Id|int|||Id IS NOT NULL|DROP
 1|first_name|string||||||
 2|surname|string||||||
 3|||Name|string|"F.concat_ws(' ', F.col('first_name'), F.col('surname'))",F.lit('John Doe')||
```

