# Comparing `tmp/funcnodes_pandas-0.1.5.tar.gz` & `tmp/funcnodes_pandas-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcnodes_pandas-0.1.5.tar", max compression
+gzip compressed data, was "funcnodes_pandas-0.1.6.tar", max compression
```

## Comparing `funcnodes_pandas-0.1.5.tar` & `funcnodes_pandas-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     2109 2024-05-16 12:46:46.897413 funcnodes_pandas-0.1.5/funcnodes_pandas/__init__.py
--rw-r--r--   0        0        0    15739 2024-05-16 12:46:06.759849 funcnodes_pandas-0.1.5/funcnodes_pandas/dataframe.py
--rw-r--r--   0        0        0     2568 2024-03-22 12:12:52.232463 funcnodes_pandas-0.1.5/funcnodes_pandas/dataseries.py
--rw-r--r--   0        0        0      451 2024-05-16 12:46:35.692296 funcnodes_pandas-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-22 16:14:38.723499 funcnodes_pandas-0.1.5/README.md
--rw-r--r--   0        0        0      587 1970-01-01 00:00:00.000000 funcnodes_pandas-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     2448 2024-05-16 14:35:27.867746 funcnodes_pandas-0.1.6/funcnodes_pandas/__init__.py
+-rw-r--r--   0        0        0    16412 2024-05-16 14:34:21.802071 funcnodes_pandas-0.1.6/funcnodes_pandas/dataframe.py
+-rw-r--r--   0        0        0     2568 2024-03-22 12:12:52.232463 funcnodes_pandas-0.1.6/funcnodes_pandas/dataseries.py
+-rw-r--r--   0        0        0     5338 2024-05-16 14:35:00.950159 funcnodes_pandas-0.1.6/funcnodes_pandas/grouping.py
+-rw-r--r--   0        0        0      451 2024-05-16 14:35:19.549860 funcnodes_pandas-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-22 16:14:38.723499 funcnodes_pandas-0.1.6/README.md
+-rw-r--r--   0        0        0      587 1970-01-01 00:00:00.000000 funcnodes_pandas-0.1.6/PKG-INFO
```

### Comparing `funcnodes_pandas-0.1.5/funcnodes_pandas/__init__.py` & `funcnodes_pandas-0.1.6/funcnodes_pandas/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,27 +24,45 @@
     drop_duplicates,
     corr,
     numeric_only,
     drop_columns,
     drop_rows,
     DropColumnNode as drop_column,
     DropRowNode as drop_row,
+    add_column,
+    add_row,
 )
 
 from .dataseries import (
     ser_to_dict,
     ser_values,
     ser_to_list,
     ser_loc,
     ser_iloc,
     ser_from_dict,
     ser_from_list,
     NODE_SHELF as SERIES_SHELF,
 )
 
+from .grouping import (
+    GroupByColumnNode as group_by_column,
+    group_by,
+    mean,
+    sum,
+    max,
+    min,
+    std,
+    var,
+    count,
+    describe,
+    group_to_list,
+    GetDFfromGroupNode as get_df_from_group,
+    NODE_SHELF as GROUPING_SHELF,
+)
+
 
 def encode_pdDf(obj, preview=False):
     if isinstance(obj, pd.DataFrame):
         if preview:
             return obj.head().to_dict(orient="split"), True
         else:
             return obj.to_dict(orient="split"), True
@@ -54,27 +72,27 @@
 
 
 fn.JSONEncoder.add_encoder(encode_pdDf)
 
 
 NODE_SHELF = fn.Shelf(
     nodes=[],
-    subshelves=[DF_SHELF, SERIES_SHELF],
+    subshelves=[DF_SHELF, SERIES_SHELF, GROUPING_SHELF],
     name="Pandas",
     description="Pandas nodes",
 )
 
 FUNCNODES_RENDER_OPTIONS: fn.RenderOptions = {
     "typemap": {
         type_to_string(pd.DataFrame): "table",
         type_to_string(pd.Series): "list",
     },
 }
 
-__version__ = "0.1.5"
+__version__ = "0.1.6"
 
 __all__ = [
     "NODE_SHELF",
     "to_dict",
     "from_dict",
     "from_csv_str",
     "get_column",
@@ -101,8 +119,10 @@
     "drop_duplicates",
     "corr",
     "numeric_only",
     "drop_columns",
     "drop_rows",
     "drop_column",
     "drop_row",
+    "add_column",
+    "add_row",
 ]
```

### Comparing `funcnodes_pandas-0.1.5/funcnodes_pandas/dataframe.py` & `funcnodes_pandas-0.1.6/funcnodes_pandas/dataframe.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from typing import TypedDict, List, Union, Literal
+from typing import TypedDict, List, Union, Literal, Any
 import funcnodes as fn
 from funcnodes.triggerstack import TriggerStack
-import pandas
+import pandas as pd
 import exposedfunctionality.function_parser.types as exf_types
 import enum
 from io import StringIO
 import numpy as np
 
 
 class DataFrameDict(TypedDict):
@@ -20,44 +20,44 @@
 @fn.NodeDecorator(
     node_id="pd.df_to_dict",
     name="To Dictionary",
     description="Converts a DataFrame to a dictionary.",
     outputs=[{"name": "dict", "type": DataFrameDict}],
 )
 def to_dict(
-    df: pandas.DataFrame,
+    df: pd.DataFrame,
 ) -> dict:
     return df.to_dict(orient="split")
 
 
 @fn.NodeDecorator(
     node_id="pd.df_to_orient_dict",
     name="To Dictionary with Orientation",
     description="Converts a DataFrame to a dictionary with a specific orientation.",
     outputs=[{"name": "dict", "type": DataFrameDict}],
 )
 def to_orient_dict(
-    df: pandas.DataFrame,
+    df: pd.DataFrame,
     orient: Literal["dict", "list", "split", "tight", "records", "index"] = "split",
 ) -> dict:
     return df.to_dict(orient=orient)
 
 
 @fn.NodeDecorator(
     node_id="pd.df_from_dict",
     name="From Dictionary",
     description="Converts a dictionary to a DataFrame.",
-    outputs=[{"name": "df", "type": pandas.DataFrame}],
+    outputs=[{"name": "df", "type": pd.DataFrame}],
 )
 def from_dict(
     data: dict,
-) -> pandas.DataFrame:
+) -> pd.DataFrame:
     # from "split" orientation or from "thight" orientation
     if "columns" in data and "index" in data and "data" in data:
-        df = pandas.DataFrame(
+        df = pd.DataFrame(
             data["data"],
             columns=data["columns"],
             index=data["index"],
         )
         idxnames = data.get("index_names")
         if idxnames is not None and len(idxnames) == len(df.index):
             df.index.names = idxnames
@@ -66,49 +66,49 @@
             df.columns.names = colnames
         return df
 
     # by default we cannot distringuise between "dict" and "index" orientation since both have the same structure of
     # {column: {index: value}} or {index: {column: value}}
     # a small heuristic is to check if the first key is a string or not to determine the orientation
     if isinstance(data, list):
-        return pandas.DataFrame(data)
+        return pd.DataFrame(data)
     if len(data) == 0:
-        return pandas.DataFrame()
+        return pd.DataFrame()
     if isinstance(next(iter(data)), str):
-        return pandas.DataFrame(data)
+        return pd.DataFrame(data)
     else:
-        return pandas.DataFrame(data).T
+        return pd.DataFrame(data).T
 
 
 @fn.NodeDecorator(
     node_id="pd.df_from_orient_dict",
     name="From Dictionary with Orientation",
     description="Converts a dictionary with a specific orientation to a DataFrame.",
-    outputs=[{"name": "df", "type": pandas.DataFrame}],
+    outputs=[{"name": "df", "type": pd.DataFrame}],
 )
 def from_orient_dict(
     data: dict,
     orient: Literal["dict", "list", "split", "tight", "records", "index"] = "split",
-) -> pandas.DataFrame:
+) -> pd.DataFrame:
     if orient == "split":
-        return pandas.DataFrame(
+        return pd.DataFrame(
             data.get("data"), columns=data.get("columns"), index=data.get("index")
         )
     elif orient in ["dict", "list", "records"]:
-        return pandas.DataFrame(data)
+        return pd.DataFrame(data)
     elif orient == "tight":
-        df = pandas.DataFrame(
+        df = pd.DataFrame(
             data.get("data"), columns=data.get("columns"), index=data.get("index")
         )
         df.columns.names = data.get("column_names")
         df.index.names = data.get("index_names")
         return df
     elif orient == "index":
-        return pandas.DataFrame(data).T
-    return pandas.DataFrame(data)
+        return pd.DataFrame(data).T
+    return pd.DataFrame(data)
 
 
 class SepEnum(enum.Enum):
     COMMA = ","
     SEMICOLON = ";"
     TAB = "\t"
     SPACE = " "
@@ -130,21 +130,21 @@
 exf_types.add_type("pd.DecimalEnum", DecimalEnum)
 
 
 @fn.NodeDecorator(
     node_id="pd.df_from_csv_str",
     name="From CSV",
     description="Reads a CSV file into a DataFrame.",
-    outputs=[{"name": "df", "type": pandas.DataFrame}],
+    outputs=[{"name": "df", "type": pd.DataFrame}],
 )
 def from_csv_str(
     source: str,
     sep: SepEnum = ",",
     decimal: DecimalEnum = ".",
-) -> pandas.DataFrame:
+) -> pd.DataFrame:
     if "SepEnum." in sep:
         sep = sep.replace("SepEnum.", "")
 
     if "DecimalEnum." in decimal:
         decimal = decimal.replace("DecimalEnum.", "")
     # Check if sep is a string that matches an enum member's name, then get its value
 
@@ -155,15 +155,15 @@
 
     # Similar check and conversion for decimal
     if isinstance(decimal, str) and decimal in DecimalEnum.__members__:
         decimal = DecimalEnum[decimal].value
     elif isinstance(decimal, DecimalEnum):  # Direct instance of DecimalEnum
         decimal = decimal.value
 
-    return pandas.read_csv(StringIO(source), sep=sep, decimal=decimal)
+    return pd.read_csv(StringIO(source), sep=sep, decimal=decimal)
 
 
 class DfFromExcelNode(fn.Node):
     node_id = "pd.df_from_xlsx"
     node_name = "From Excel"
 
     data = fn.NodeInput(
@@ -173,34 +173,34 @@
     sheet = fn.NodeInput(
         id="sheet",
         type=str,
         default=None,
         required=False,
     )
 
-    df = fn.NodeOutput(id="df", type=pandas.DataFrame)
+    df = fn.NodeOutput(id="df", type=pd.DataFrame)
 
     async def func(self, data: bytes, sheet: str = None):
         # get sheet names
-        sheets = pandas.ExcelFile(data).sheet_names
+        sheets = pd.ExcelFile(data).sheet_names
         self.inputs["sheet"].value_options = {s: s for s in sheets}
         if sheet is None or sheet not in sheets:
             sheet = sheets[0]
         self.inputs["sheet"].set_value(sheet, does_trigger=False)
-        self.outputs["df"].value = pandas.read_excel(data, sheet_name=sheet)
+        self.outputs["df"].value = pd.read_excel(data, sheet_name=sheet)
 
 
 @fn.NodeDecorator(
     node_id="pd.df_to_csv_str",
     name="To CSV",
     description="Writes a DataFrame to a CSV string.",
     outputs=[{"name": "csv", "type": str}],
 )
 def to_csv_str(
-    df: pandas.DataFrame,
+    df: pd.DataFrame,
     sep: SepEnum = ",",
     decimal: DecimalEnum = ".",
     index: bool = False,
 ) -> str:
     if "SepEnum." in sep:
         sep = sep.replace("SepEnum.", "")
 
@@ -223,27 +223,27 @@
 
 
 class GetColumnNode(fn.Node):
     node_id = "pd.get_column"
     node_name = "Get Column"
     df = fn.NodeInput(
         "DataFrame",
-        type=pandas.DataFrame,
+        type=pd.DataFrame,
         uuid="df",
     )
 
     column = fn.NodeInput(
         "Column",
         type=str,
         uuid="column",
     )
 
     series = fn.NodeOutput(
         "Series",
-        type=pandas.Series,
+        type=pd.Series,
         uuid="series",
     )
 
     def __init__(self):
         super().__init__()
         self.get_input("df").on("after_set_value", self._update_columns)
 
@@ -256,40 +256,40 @@
         try:
             col.update_value_options(options=list(df.columns))
         except Exception:
             col.update_value_options(options=[])
 
     async def func(
         self,
-        df: pandas.DataFrame,
+        df: pd.DataFrame,
         column: str,
-    ) -> pandas.Series:
+    ) -> pd.Series:
         self.get_output("series").value = df[column]
         return df[column]
 
 
 class GetRowNode(fn.Node):
     node_id = "pd.df_loc"
     node_name = "Get Row"
     description = "Gets a row from a DataFrame by label."
     df = fn.NodeInput(
         "DataFrame",
-        type=pandas.DataFrame,
+        type=pd.DataFrame,
         uuid="df",
     )
 
     row = fn.NodeInput(
         "Row",
         type=str,
         uuid="row",
     )
 
     series = fn.NodeOutput(
         "Series",
-        type=pandas.Series,
+        type=pd.Series,
         uuid="series",
     )
 
     def __init__(self):
         super().__init__()
         self.get_input("df").on("after_set_value", self._update_rows)
 
@@ -302,131 +302,131 @@
         try:
             row.update_value_options(options=list(df.index))
         except Exception:
             row.update_value_options(options=[])
 
     async def func(
         self,
-        df: pandas.DataFrame,
+        df: pd.DataFrame,
         row: str,
-    ) -> pandas.Series:
+    ) -> pd.Series:
         if len(df.index) == 0:
-            return pandas.Series(index=df.columns)
+            return pd.Series(index=df.columns)
         label = df.index.to_list()[0].__class__(row)
         ser = df.loc[label]
         self.get_output("series").value = ser
         return ser
 
 
 @fn.NodeDecorator(
     node_id="pd.df_iloc",
     name="Get Row by Index",
     description="Gets a row from a DataFrame by index.",
-    outputs=[{"name": "row", "type": pandas.Series}],
+    outputs=[{"name": "row", "type": pd.Series}],
 )
 def df_iloc(
-    df: pandas.DataFrame,
+    df: pd.DataFrame,
     index: Union[int],
-) -> pandas.Series:
+) -> pd.Series:
     return df.iloc[index]
 
 
 @fn.NodeDecorator(
     node_id="pd.df_from_array",
     name="From Array",
     description="Creates a DataFrame from an array.",
-    outputs=[{"name": "df", "type": pandas.DataFrame}],
+    outputs=[{"name": "df", "type": pd.DataFrame}],
 )
 def df_from_array(
     data: Union[list[list[Union[str, int, float]]], np.ndarray],
     columns: List[str] = None,
     index: List[Union[str, int, float]] = None,
-) -> pandas.DataFrame:
+) -> pd.DataFrame:
     if columns is None:
         columns = [f"Col {i+1}" for i in range(len(data[0]))]
-    return pandas.DataFrame(data, columns=columns, index=index)
+    return pd.DataFrame(data, columns=columns, index=index)
 
 
 @fn.NodeDecorator(
     node_id="pd.dropna",
     name="Drop NA",
     description="Drops rows or columns with NA values.",
 )
 def dropna(
-    df: pandas.DataFrame,
+    df: pd.DataFrame,
     axis: Literal["index", "columns"] = "index",
     how: Literal["any", "all"] = "any",
-) -> pandas.DataFrame:
+) -> pd.DataFrame:
     return df.dropna(axis=axis, how=how)
 
 
 @fn.NodeDecorator(
     node_id="pd.fillna",
     name="Fill NA",
     description="Fills NA values with a specified value.",
 )
 def fillna(
-    df: pandas.DataFrame,
+    df: pd.DataFrame,
     value: Union[str, int, float] = 0,
-) -> pandas.DataFrame:
+) -> pd.DataFrame:
     return df.fillna(value)
 
 
 @fn.NodeDecorator(
     node_id="pd.bfill",
     name="Backfill",
     description="Backfills NA values.",
 )
 def bfill(
-    df: pandas.DataFrame,
-) -> pandas.DataFrame:
+    df: pd.DataFrame,
+) -> pd.DataFrame:
     return df.bfill()
 
 
 @fn.NodeDecorator(
     node_id="pd.ffill",
     name="Forwardfill",
     description="Forwardfills NA values.",
 )
 def ffill(
-    df: pandas.DataFrame,
-) -> pandas.DataFrame:
+    df: pd.DataFrame,
+) -> pd.DataFrame:
     return df.ffill()
 
 
 @fn.NodeDecorator(
     node_id="pd.drop_duplicates",
     name="Drop Duplicates",
     description="Drops duplicate rows.",
 )
 def drop_duplicates(
-    df: pandas.DataFrame,
-) -> pandas.DataFrame:
+    df: pd.DataFrame,
+) -> pd.DataFrame:
     return df.drop_duplicates()
 
 
 @fn.NodeDecorator(
     node_id="pd.corr",
     name="Correlation",
     description="Calculates the correlation between columns.",
-    outputs=[{"name": "correlation", "type": pandas.DataFrame}],
+    outputs=[{"name": "correlation", "type": pd.DataFrame}],
 )
 def corr(
-    df: pandas.DataFrame,
+    df: pd.DataFrame,
     method: Literal["pearson", "kendall", "spearman"] = "pearson",
     numeric_only: bool = False,
-) -> pandas.DataFrame:
+) -> pd.DataFrame:
     return df.corr(method=method, numeric_only=numeric_only)
 
 
 @fn.NodeDecorator(
     node_id="pd.numeric_only",
     name="Numeric Only",
 )
-def numeric_only(df: pandas.DataFrame, label_encode=False) -> pandas.DataFrame:
+def numeric_only(df: pd.DataFrame, label_encode: bool = False) -> pd.DataFrame:
     """
     Converts a DataFrame to only hold numeric values.
     Optionally, non-numeric values can be converted to numeric labels.
 
     Parameters:
     - df: pandas DataFrame
     - label_encode: bool, if True, convert non-numeric values to numeric labels
@@ -435,42 +435,42 @@
     - A new DataFrame containing only numeric values
     """
 
     if label_encode:
         df = df.copy()
         for column in df.select_dtypes(exclude=[np.number]):
             try:
-                df[column] = pandas.to_numeric(df[column])
+                df[column] = pd.to_numeric(df[column])
             except ValueError:
                 pass
         for column in df.select_dtypes(include=["object", "category"]):
             df[column] = df[column].astype("category").cat.codes
 
     numeric_df = df.select_dtypes(include=[np.number])
     return numeric_df
 
 
 class DropColumnNode(fn.Node):
     node_id = "pd.drop_column"
     node_name = "Drop Column"
     df = fn.NodeInput(
         "DataFrame",
-        type=pandas.DataFrame,
+        type=pd.DataFrame,
         uuid="df",
     )
 
     column = fn.NodeInput(
         "Column",
         type=str,
         uuid="column",
     )
 
     out = fn.NodeOutput(
         "New DataFrame",
-        type=pandas.DataFrame,
+        type=pd.DataFrame,
         uuid="out",
     )
 
     def __init__(self):
         super().__init__()
         self.get_input("df").on("after_set_value", self._update_columns)
 
@@ -483,40 +483,40 @@
         try:
             col.update_value_options(options=list(df.columns))
         except Exception:
             col.update_value_options(options=[])
 
     async def func(
         self,
-        df: pandas.DataFrame,
+        df: pd.DataFrame,
         column: str,
-    ) -> pandas.DataFrame:
+    ) -> pd.DataFrame:
         df = df.drop(column, axis=1)
         self.get_output("out").value = df
         return df
 
 
 class DropRowNode(fn.Node):
     node_id = "pd.drop_row"
     node_name = "Drop Row"
     df = fn.NodeInput(
         "DataFrame",
-        type=pandas.DataFrame,
+        type=pd.DataFrame,
         uuid="df",
     )
 
     row = fn.NodeInput(
         "Row",
         type=str,
         uuid="row",
     )
 
     out = fn.NodeOutput(
         "New DataFrame",
-        type=pandas.DataFrame,
+        type=pd.DataFrame,
         uuid="out",
     )
 
     def __init__(self):
         super().__init__()
         self.get_input("df").on("after_set_value", self._update_rows)
 
@@ -529,54 +529,92 @@
         try:
             row.update_value_options(options=list(df.index))
         except Exception:
             row.update_value_options(options=[])
 
     async def func(
         self,
-        df: pandas.DataFrame,
+        df: pd.DataFrame,
         row: str,
-    ) -> pandas.DataFrame:
+    ) -> pd.DataFrame:
         df = df.drop(row, axis=0)
         self.get_output("out").value = df
         return df
 
 
 @fn.NodeDecorator(
     node_id="pd.drop_columns",
     name="Drop Columns",
     description="Drops columns from a DataFrame.",
 )
 def drop_columns(
-    df: pandas.DataFrame,
+    df: pd.DataFrame,
     columns: str,
-) -> pandas.DataFrame:
+) -> pd.DataFrame:
     columns = [s.strip() for s in columns.split(",")]
     return df.drop(columns, axis=1)
 
 
 @fn.NodeDecorator(
     node_id="pd.drop_rows",
     name="Drop Rows",
     description="Drops rows from a DataFrame.",
 )
 def drop_rows(
-    df: pandas.DataFrame,
+    df: pd.DataFrame,
     rows: str,
-) -> pandas.DataFrame:
+) -> pd.DataFrame:
     rows = [s.strip() for s in rows.split(",")]
 
     if len(df.index) == 0:
         return df
     cls = df.index.to_list()[0].__class__
     rows = [cls(row) for row in rows]
 
     return df.drop(rows, axis=0)
 
 
+@fn.NodeDecorator(
+    node_id="pd.add_column",
+    name="Add Column",
+    description="Adds a column from a DataFrame.",
+)
+def add_column(
+    df: pd.DataFrame,
+    column: str,
+    data: Any,
+) -> pd.DataFrame:
+    df = df.copy()
+    df[column] = data
+    return df
+
+
+@fn.NodeDecorator(
+    node_id="pd.add_row",
+    name="Add Row",
+    description="Adds a row to a DataFrame.",
+)
+def add_row(
+    df: pd.DataFrame,
+    row: Union[dict, list],
+) -> pd.DataFrame:
+    if not isinstance(row, dict):
+        try:
+            row = {c: row[c] for c in df.columns}
+        except Exception:
+            pass
+        if len(row) != len(df.columns):
+            raise ValueError(
+                "Row must have the same number of columns as the DataFrame"
+            )
+        row = {c: [v] for c, v in zip(df.columns, row)}
+    df = pd.concat([df, pd.DataFrame(row)])
+    return df
+
+
 NODE_SHELF = fn.Shelf(
     nodes=[
         to_dict,
         from_dict,
         from_csv_str,
         to_csv_str,
         GetColumnNode,
@@ -593,12 +631,14 @@
         drop_duplicates,
         corr,
         numeric_only,
         DropColumnNode,
         DropRowNode,
         drop_columns,
         drop_rows,
+        add_column,
+        add_row,
     ],
     name="Datataframe",
     description="Pandas DataFrame nodes",
     subshelves=[],
 )
```

### Comparing `funcnodes_pandas-0.1.5/funcnodes_pandas/dataseries.py` & `funcnodes_pandas-0.1.6/funcnodes_pandas/dataseries.py`

 * *Files identical despite different names*

### Comparing `funcnodes_pandas-0.1.5/PKG-INFO` & `funcnodes_pandas-0.1.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcnodes-pandas
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 License: MIT
 Author: Julian Kimmig
 Author-email: julian.kimmig@gmx.net
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

