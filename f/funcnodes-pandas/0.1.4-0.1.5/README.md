# Comparing `tmp/funcnodes_pandas-0.1.4.tar.gz` & `tmp/funcnodes_pandas-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcnodes_pandas-0.1.4.tar", max compression
+gzip compressed data, was "funcnodes_pandas-0.1.5.tar", max compression
```

## Comparing `funcnodes_pandas-0.1.4.tar` & `funcnodes_pandas-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1902 2024-05-16 11:50:52.243624 funcnodes_pandas-0.1.4/funcnodes_pandas/__init__.py
--rw-r--r--   0        0        0    11879 2024-05-16 11:29:16.973080 funcnodes_pandas-0.1.4/funcnodes_pandas/dataframe.py
--rw-r--r--   0        0        0     2568 2024-03-22 12:12:52.232463 funcnodes_pandas-0.1.4/funcnodes_pandas/dataseries.py
--rw-r--r--   0        0        0      451 2024-05-16 11:52:09.103511 funcnodes_pandas-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-22 16:14:38.723499 funcnodes_pandas-0.1.4/README.md
--rw-r--r--   0        0        0      587 1970-01-01 00:00:00.000000 funcnodes_pandas-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     2109 2024-05-16 12:46:46.897413 funcnodes_pandas-0.1.5/funcnodes_pandas/__init__.py
+-rw-r--r--   0        0        0    15739 2024-05-16 12:46:06.759849 funcnodes_pandas-0.1.5/funcnodes_pandas/dataframe.py
+-rw-r--r--   0        0        0     2568 2024-03-22 12:12:52.232463 funcnodes_pandas-0.1.5/funcnodes_pandas/dataseries.py
+-rw-r--r--   0        0        0      451 2024-05-16 12:46:35.692296 funcnodes_pandas-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-22 16:14:38.723499 funcnodes_pandas-0.1.5/README.md
+-rw-r--r--   0        0        0      587 1970-01-01 00:00:00.000000 funcnodes_pandas-0.1.5/PKG-INFO
```

### Comparing `funcnodes_pandas-0.1.4/funcnodes_pandas/__init__.py` & `funcnodes_pandas-0.1.5/funcnodes_pandas/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,19 @@
     DfFromExcelNode,
     dropna,
     ffill,
     bfill,
     fillna,
     drop_duplicates,
     corr,
+    numeric_only,
+    drop_columns,
+    drop_rows,
+    DropColumnNode as drop_column,
+    DropRowNode as drop_row,
 )
 
 from .dataseries import (
     ser_to_dict,
     ser_values,
     ser_to_list,
     ser_loc,
@@ -61,15 +66,15 @@
 FUNCNODES_RENDER_OPTIONS: fn.RenderOptions = {
     "typemap": {
         type_to_string(pd.DataFrame): "table",
         type_to_string(pd.Series): "list",
     },
 }
 
-__version__ = "0.1.4"
+__version__ = "0.1.5"
 
 __all__ = [
     "NODE_SHELF",
     "to_dict",
     "from_dict",
     "from_csv_str",
     "get_column",
@@ -91,8 +96,13 @@
     "DfFromExcelNode",
     "dropna",
     "ffill",
     "bfill",
     "fillna",
     "drop_duplicates",
     "corr",
+    "numeric_only",
+    "drop_columns",
+    "drop_rows",
+    "drop_column",
+    "drop_row",
 ]
```

### Comparing `funcnodes_pandas-0.1.4/funcnodes_pandas/dataframe.py` & `funcnodes_pandas-0.1.5/funcnodes_pandas/dataframe.py`

 * *Files 14% similar despite different names*

```diff
@@ -414,14 +414,169 @@
     df: pandas.DataFrame,
     method: Literal["pearson", "kendall", "spearman"] = "pearson",
     numeric_only: bool = False,
 ) -> pandas.DataFrame:
     return df.corr(method=method, numeric_only=numeric_only)
 
 
+@fn.NodeDecorator(
+    node_id="pd.numeric_only",
+    name="Numeric Only",
+)
+def numeric_only(df: pandas.DataFrame, label_encode=False) -> pandas.DataFrame:
+    """
+    Converts a DataFrame to only hold numeric values.
+    Optionally, non-numeric values can be converted to numeric labels.
+
+    Parameters:
+    - df: pandas DataFrame
+    - label_encode: bool, if True, convert non-numeric values to numeric labels
+
+    Returns:
+    - A new DataFrame containing only numeric values
+    """
+
+    if label_encode:
+        df = df.copy()
+        for column in df.select_dtypes(exclude=[np.number]):
+            try:
+                df[column] = pandas.to_numeric(df[column])
+            except ValueError:
+                pass
+        for column in df.select_dtypes(include=["object", "category"]):
+            df[column] = df[column].astype("category").cat.codes
+
+    numeric_df = df.select_dtypes(include=[np.number])
+    return numeric_df
+
+
+class DropColumnNode(fn.Node):
+    node_id = "pd.drop_column"
+    node_name = "Drop Column"
+    df = fn.NodeInput(
+        "DataFrame",
+        type=pandas.DataFrame,
+        uuid="df",
+    )
+
+    column = fn.NodeInput(
+        "Column",
+        type=str,
+        uuid="column",
+    )
+
+    out = fn.NodeOutput(
+        "New DataFrame",
+        type=pandas.DataFrame,
+        uuid="out",
+    )
+
+    def __init__(self):
+        super().__init__()
+        self.get_input("df").on("after_set_value", self._update_columns)
+
+    def _update_columns(self, **kwargs):
+        try:
+            df = self.get_input("df").value
+            col = self.get_input("column")
+        except KeyError:
+            return
+        try:
+            col.update_value_options(options=list(df.columns))
+        except Exception:
+            col.update_value_options(options=[])
+
+    async def func(
+        self,
+        df: pandas.DataFrame,
+        column: str,
+    ) -> pandas.DataFrame:
+        df = df.drop(column, axis=1)
+        self.get_output("out").value = df
+        return df
+
+
+class DropRowNode(fn.Node):
+    node_id = "pd.drop_row"
+    node_name = "Drop Row"
+    df = fn.NodeInput(
+        "DataFrame",
+        type=pandas.DataFrame,
+        uuid="df",
+    )
+
+    row = fn.NodeInput(
+        "Row",
+        type=str,
+        uuid="row",
+    )
+
+    out = fn.NodeOutput(
+        "New DataFrame",
+        type=pandas.DataFrame,
+        uuid="out",
+    )
+
+    def __init__(self):
+        super().__init__()
+        self.get_input("df").on("after_set_value", self._update_rows)
+
+    def _update_rows(self, **kwargs):
+        try:
+            df = self.get_input("df").value
+            row = self.get_input("row")
+        except KeyError:
+            return
+        try:
+            row.update_value_options(options=list(df.index))
+        except Exception:
+            row.update_value_options(options=[])
+
+    async def func(
+        self,
+        df: pandas.DataFrame,
+        row: str,
+    ) -> pandas.DataFrame:
+        df = df.drop(row, axis=0)
+        self.get_output("out").value = df
+        return df
+
+
+@fn.NodeDecorator(
+    node_id="pd.drop_columns",
+    name="Drop Columns",
+    description="Drops columns from a DataFrame.",
+)
+def drop_columns(
+    df: pandas.DataFrame,
+    columns: str,
+) -> pandas.DataFrame:
+    columns = [s.strip() for s in columns.split(",")]
+    return df.drop(columns, axis=1)
+
+
+@fn.NodeDecorator(
+    node_id="pd.drop_rows",
+    name="Drop Rows",
+    description="Drops rows from a DataFrame.",
+)
+def drop_rows(
+    df: pandas.DataFrame,
+    rows: str,
+) -> pandas.DataFrame:
+    rows = [s.strip() for s in rows.split(",")]
+
+    if len(df.index) == 0:
+        return df
+    cls = df.index.to_list()[0].__class__
+    rows = [cls(row) for row in rows]
+
+    return df.drop(rows, axis=0)
+
+
 NODE_SHELF = fn.Shelf(
     nodes=[
         to_dict,
         from_dict,
         from_csv_str,
         to_csv_str,
         GetColumnNode,
@@ -433,12 +588,17 @@
         DfFromExcelNode,
         dropna,
         fillna,
         bfill,
         ffill,
         drop_duplicates,
         corr,
+        numeric_only,
+        DropColumnNode,
+        DropRowNode,
+        drop_columns,
+        drop_rows,
     ],
     name="Datataframe",
     description="Pandas DataFrame nodes",
     subshelves=[],
 )
```

### Comparing `funcnodes_pandas-0.1.4/funcnodes_pandas/dataseries.py` & `funcnodes_pandas-0.1.5/funcnodes_pandas/dataseries.py`

 * *Files identical despite different names*

### Comparing `funcnodes_pandas-0.1.4/PKG-INFO` & `funcnodes_pandas-0.1.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcnodes-pandas
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 License: MIT
 Author: Julian Kimmig
 Author-email: julian.kimmig@gmx.net
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

