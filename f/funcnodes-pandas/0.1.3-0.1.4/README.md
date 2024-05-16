# Comparing `tmp/funcnodes_pandas-0.1.3.tar.gz` & `tmp/funcnodes_pandas-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcnodes_pandas-0.1.3.tar", max compression
+gzip compressed data, was "funcnodes_pandas-0.1.4.tar", max compression
```

## Comparing `funcnodes_pandas-0.1.3.tar` & `funcnodes_pandas-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1722 2024-04-25 11:04:06.939574 funcnodes_pandas-0.1.3/funcnodes_pandas/__init__.py
--rw-r--r--   0        0        0     9272 2024-04-12 10:54:18.814562 funcnodes_pandas-0.1.3/funcnodes_pandas/dataframe.py
--rw-r--r--   0        0        0     2568 2024-03-22 12:12:52.232463 funcnodes_pandas-0.1.3/funcnodes_pandas/dataseries.py
--rw-r--r--   0        0        0      467 2024-04-25 11:03:54.168867 funcnodes_pandas-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-22 16:14:38.723499 funcnodes_pandas-0.1.3/README.md
--rw-r--r--   0        0        0      677 1970-01-01 00:00:00.000000 funcnodes_pandas-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1902 2024-05-16 11:50:52.243624 funcnodes_pandas-0.1.4/funcnodes_pandas/__init__.py
+-rw-r--r--   0        0        0    11879 2024-05-16 11:29:16.973080 funcnodes_pandas-0.1.4/funcnodes_pandas/dataframe.py
+-rw-r--r--   0        0        0     2568 2024-03-22 12:12:52.232463 funcnodes_pandas-0.1.4/funcnodes_pandas/dataseries.py
+-rw-r--r--   0        0        0      451 2024-05-16 11:52:09.103511 funcnodes_pandas-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-22 16:14:38.723499 funcnodes_pandas-0.1.4/README.md
+-rw-r--r--   0        0        0      587 1970-01-01 00:00:00.000000 funcnodes_pandas-0.1.4/PKG-INFO
```

### Comparing `funcnodes_pandas-0.1.3/funcnodes_pandas/__init__.py` & `funcnodes_pandas-0.1.4/funcnodes_pandas/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,18 +9,24 @@
     to_dict,
     from_dict,
     from_csv_str,
     GetColumnNode as get_column,
     to_orient_dict,
     from_orient_dict,
     df_iloc,
-    df_loc,
+    GetRowNode as df_loc,
     to_csv_str,
     df_from_array,
     DfFromExcelNode,
+    dropna,
+    ffill,
+    bfill,
+    fillna,
+    drop_duplicates,
+    corr,
 )
 
 from .dataseries import (
     ser_to_dict,
     ser_values,
     ser_to_list,
     ser_loc,
@@ -55,15 +61,15 @@
 FUNCNODES_RENDER_OPTIONS: fn.RenderOptions = {
     "typemap": {
         type_to_string(pd.DataFrame): "table",
         type_to_string(pd.Series): "list",
     },
 }
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 
 __all__ = [
     "NODE_SHELF",
     "to_dict",
     "from_dict",
     "from_csv_str",
     "get_column",
@@ -79,8 +85,14 @@
     "ser_from_dict",
     "ser_from_list",
     "SERIES_SHELF",
     "DF_SHELF",
     "to_csv_str",
     "df_from_array",
     "DfFromExcelNode",
+    "dropna",
+    "ffill",
+    "bfill",
+    "fillna",
+    "drop_duplicates",
+    "corr",
 ]
```

### Comparing `funcnodes_pandas-0.1.3/funcnodes_pandas/dataframe.py` & `funcnodes_pandas-0.1.4/funcnodes_pandas/dataframe.py`

 * *Files 17% similar despite different names*

```diff
@@ -245,42 +245,80 @@
 
     def __init__(self):
         super().__init__()
         self.get_input("df").on("after_set_value", self._update_columns)
 
     def _update_columns(self, **kwargs):
         try:
-            self.get_input("column").value_options = {
-                c: c for c in self.get_input("df").value.columns
-            }
+            df = self.get_input("df").value
+            col = self.get_input("column")
+        except KeyError:
+            return
+        try:
+            col.update_value_options(options=list(df.columns))
         except Exception:
-            self.get_input("column").value_options = {}
+            col.update_value_options(options=[])
 
     async def func(
         self,
         df: pandas.DataFrame,
         column: str,
     ) -> pandas.Series:
         self.get_output("series").value = df[column]
         return df[column]
 
 
-@fn.NodeDecorator(
-    node_id="pd.df_loc",
-    name="Get Row",
-    description="Gets a row from a DataFrame by label.",
-    outputs=[{"name": "row", "type": pandas.Series}],
-)
-def df_loc(
-    df: pandas.DataFrame,
-    label: Union[str],
-) -> pandas.Series:
-    # taransform label to the correct type
-    label = df.index.to_list()[0].__class__(label)
-    return df.loc[label]
+class GetRowNode(fn.Node):
+    node_id = "pd.df_loc"
+    node_name = "Get Row"
+    description = "Gets a row from a DataFrame by label."
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
+    series = fn.NodeOutput(
+        "Series",
+        type=pandas.Series,
+        uuid="series",
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
+    ) -> pandas.Series:
+        if len(df.index) == 0:
+            return pandas.Series(index=df.columns)
+        label = df.index.to_list()[0].__class__(row)
+        ser = df.loc[label]
+        self.get_output("series").value = ser
+        return ser
 
 
 @fn.NodeDecorator(
     node_id="pd.df_iloc",
     name="Get Row by Index",
     description="Gets a row from a DataFrame by index.",
     outputs=[{"name": "row", "type": pandas.Series}],
@@ -304,25 +342,103 @@
     index: List[Union[str, int, float]] = None,
 ) -> pandas.DataFrame:
     if columns is None:
         columns = [f"Col {i+1}" for i in range(len(data[0]))]
     return pandas.DataFrame(data, columns=columns, index=index)
 
 
+@fn.NodeDecorator(
+    node_id="pd.dropna",
+    name="Drop NA",
+    description="Drops rows or columns with NA values.",
+)
+def dropna(
+    df: pandas.DataFrame,
+    axis: Literal["index", "columns"] = "index",
+    how: Literal["any", "all"] = "any",
+) -> pandas.DataFrame:
+    return df.dropna(axis=axis, how=how)
+
+
+@fn.NodeDecorator(
+    node_id="pd.fillna",
+    name="Fill NA",
+    description="Fills NA values with a specified value.",
+)
+def fillna(
+    df: pandas.DataFrame,
+    value: Union[str, int, float] = 0,
+) -> pandas.DataFrame:
+    return df.fillna(value)
+
+
+@fn.NodeDecorator(
+    node_id="pd.bfill",
+    name="Backfill",
+    description="Backfills NA values.",
+)
+def bfill(
+    df: pandas.DataFrame,
+) -> pandas.DataFrame:
+    return df.bfill()
+
+
+@fn.NodeDecorator(
+    node_id="pd.ffill",
+    name="Forwardfill",
+    description="Forwardfills NA values.",
+)
+def ffill(
+    df: pandas.DataFrame,
+) -> pandas.DataFrame:
+    return df.ffill()
+
+
+@fn.NodeDecorator(
+    node_id="pd.drop_duplicates",
+    name="Drop Duplicates",
+    description="Drops duplicate rows.",
+)
+def drop_duplicates(
+    df: pandas.DataFrame,
+) -> pandas.DataFrame:
+    return df.drop_duplicates()
+
+
+@fn.NodeDecorator(
+    node_id="pd.corr",
+    name="Correlation",
+    description="Calculates the correlation between columns.",
+    outputs=[{"name": "correlation", "type": pandas.DataFrame}],
+)
+def corr(
+    df: pandas.DataFrame,
+    method: Literal["pearson", "kendall", "spearman"] = "pearson",
+    numeric_only: bool = False,
+) -> pandas.DataFrame:
+    return df.corr(method=method, numeric_only=numeric_only)
+
+
 NODE_SHELF = fn.Shelf(
     nodes=[
         to_dict,
         from_dict,
         from_csv_str,
         to_csv_str,
         GetColumnNode,
         to_orient_dict,
         from_orient_dict,
-        df_loc,
+        GetRowNode,
         df_iloc,
         df_from_array,
         DfFromExcelNode,
+        dropna,
+        fillna,
+        bfill,
+        ffill,
+        drop_duplicates,
+        corr,
     ],
     name="Datataframe",
     description="Pandas DataFrame nodes",
     subshelves=[],
 )
```

### Comparing `funcnodes_pandas-0.1.3/funcnodes_pandas/dataseries.py` & `funcnodes_pandas-0.1.4/funcnodes_pandas/dataseries.py`

 * *Files identical despite different names*

### Comparing `funcnodes_pandas-0.1.3/PKG-INFO` & `funcnodes_pandas-0.1.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: funcnodes-pandas
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 License: MIT
 Author: Julian Kimmig
 Author-email: julian.kimmig@gmx.net
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: funcnodes (>=0.1.42,<1.0.0)
+Requires-Dist: funcnodes (>=0.1.42)
 Requires-Dist: funcnodes-numpy (>=0.1.5)
-Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
-Requires-Dist: pandas (>=2.2.1,<3.0.0)
+Requires-Dist: openpyxl
+Requires-Dist: pandas
 Description-Content-Type: text/markdown
```

