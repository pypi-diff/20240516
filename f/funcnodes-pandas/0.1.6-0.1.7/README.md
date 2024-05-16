# Comparing `tmp/funcnodes_pandas-0.1.6.tar.gz` & `tmp/funcnodes_pandas-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcnodes_pandas-0.1.6.tar", max compression
+gzip compressed data, was "funcnodes_pandas-0.1.7.tar", max compression
```

## Comparing `funcnodes_pandas-0.1.6.tar` & `funcnodes_pandas-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2448 2024-05-16 14:35:27.867746 funcnodes_pandas-0.1.6/funcnodes_pandas/__init__.py
--rw-r--r--   0        0        0    16412 2024-05-16 14:34:21.802071 funcnodes_pandas-0.1.6/funcnodes_pandas/dataframe.py
--rw-r--r--   0        0        0     2568 2024-03-22 12:12:52.232463 funcnodes_pandas-0.1.6/funcnodes_pandas/dataseries.py
--rw-r--r--   0        0        0     5338 2024-05-16 14:35:00.950159 funcnodes_pandas-0.1.6/funcnodes_pandas/grouping.py
--rw-r--r--   0        0        0      451 2024-05-16 14:35:19.549860 funcnodes_pandas-0.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-22 16:14:38.723499 funcnodes_pandas-0.1.6/README.md
--rw-r--r--   0        0        0      587 1970-01-01 00:00:00.000000 funcnodes_pandas-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     2629 2024-05-16 15:03:18.425559 funcnodes_pandas-0.1.7/funcnodes_pandas/__init__.py
+-rw-r--r--   0        0        0    16412 2024-05-16 14:34:21.802071 funcnodes_pandas-0.1.7/funcnodes_pandas/dataframe.py
+-rw-r--r--   0        0        0     2568 2024-03-22 12:12:52.232463 funcnodes_pandas-0.1.7/funcnodes_pandas/dataseries.py
+-rw-r--r--   0        0        0     5337 2024-05-16 14:57:02.135799 funcnodes_pandas-0.1.7/funcnodes_pandas/grouping.py
+-rw-r--r--   0        0        0      451 2024-05-16 15:03:22.069083 funcnodes_pandas-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-22 16:14:38.723499 funcnodes_pandas-0.1.7/README.md
+-rw-r--r--   0        0        0      587 1970-01-01 00:00:00.000000 funcnodes_pandas-0.1.7/PKG-INFO
```

### Comparing `funcnodes_pandas-0.1.6/funcnodes_pandas/__init__.py` & `funcnodes_pandas-0.1.7/funcnodes_pandas/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 FUNCNODES_RENDER_OPTIONS: fn.RenderOptions = {
     "typemap": {
         type_to_string(pd.DataFrame): "table",
         type_to_string(pd.Series): "list",
     },
 }
 
-__version__ = "0.1.6"
+__version__ = "0.1.7"
 
 __all__ = [
     "NODE_SHELF",
     "to_dict",
     "from_dict",
     "from_csv_str",
     "get_column",
@@ -121,8 +121,20 @@
     "numeric_only",
     "drop_columns",
     "drop_rows",
     "drop_column",
     "drop_row",
     "add_column",
     "add_row",
+    "group_by_column",
+    "group_by",
+    "mean",
+    "sum",
+    "max",
+    "min",
+    "std",
+    "var",
+    "count",
+    "describe",
+    "group_to_list",
+    "get_df_from_group",
 ]
```

### Comparing `funcnodes_pandas-0.1.6/funcnodes_pandas/dataframe.py` & `funcnodes_pandas-0.1.7/funcnodes_pandas/dataframe.py`

 * *Files identical despite different names*

### Comparing `funcnodes_pandas-0.1.6/funcnodes_pandas/dataseries.py` & `funcnodes_pandas-0.1.7/funcnodes_pandas/dataseries.py`

 * *Files identical despite different names*

### Comparing `funcnodes_pandas-0.1.6/funcnodes_pandas/grouping.py` & `funcnodes_pandas-0.1.7/funcnodes_pandas/grouping.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,15 +193,15 @@
         "DataFrame",
         type=pd.DataFrame,
         uuid="df",
     )
 
     def __init__(self):
         super().__init__()
-        self.get_input("df").on("after_set_value", self._update_groups)
+        self.get_input("group").on("after_set_value", self._update_groups)
 
     def _update_groups(self, **kwargs):
         try:
             group = self.get_input("group").value
             name = self.get_input("name")
         except KeyError:
             return
@@ -209,17 +209,17 @@
             name.update_value_options(options=list(group.groups.keys()))
         except Exception:
             name.update_value_options(options=[])
 
     async def func(
         self,
         group: DataFrameGroupBy,
-        column: str,
+        name: str,
     ) -> pd.DataFrame:
-        df = group.get_group(column).copy()
+        df = group.get_group(name).copy()
         self.get_output("df").value = df
         return df
 
 
 NODE_SHELF = fn.Shelf(
     nodes=[
         GroupByColumnNode,
```

### Comparing `funcnodes_pandas-0.1.6/PKG-INFO` & `funcnodes_pandas-0.1.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcnodes-pandas
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 License: MIT
 Author: Julian Kimmig
 Author-email: julian.kimmig@gmx.net
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

