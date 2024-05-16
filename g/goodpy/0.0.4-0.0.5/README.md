# Comparing `tmp/goodpy-0.0.4-py2.py3-none-any.whl.zip` & `tmp/goodpy-0.0.5-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 9182 bytes, number of entries: 24
+Zip file size: 11064 bytes, number of entries: 25
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 goodpy/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 goodpy/f/__init__.py
 -rw-r--r--  2.0 unx       54 b- defN 20-Feb-02 00:00 goodpy/f/date/__init__.py
 -rw-r--r--  2.0 unx      789 b- defN 20-Feb-02 00:00 goodpy/f/date/get_date_last_friday.py
 -rw-r--r--  2.0 unx       31 b- defN 20-Feb-02 00:00 goodpy/f/dict_key_and_value/__init__.py
 -rw-r--r--  2.0 unx      127 b- defN 20-Feb-02 00:00 goodpy/f/dict_key_and_value/update.py
 -rw-r--r--  2.0 unx       29 b- defN 20-Feb-02 00:00 goodpy/f/dirpath/__init__.py
@@ -12,15 +12,16 @@
 -rw-r--r--  2.0 unx       61 b- defN 20-Feb-02 00:00 goodpy/f/num1_and_num2/__init__.py
 -rw-r--r--  2.0 unx       75 b- defN 20-Feb-02 00:00 goodpy/f/num1_and_num2/check_if_greater_than.py
 -rw-r--r--  2.0 unx       43 b- defN 20-Feb-02 00:00 goodpy/f/row_and_keys/__init__.py
 -rw-r--r--  2.0 unx      205 b- defN 20-Feb-02 00:00 goodpy/f/row_and_keys/get_keys_row.py
 -rw-r--r--  2.0 unx       33 b- defN 20-Feb-02 00:00 goodpy/f/row_key_and_value/__init__.py
 -rw-r--r--  2.0 unx      355 b- defN 20-Feb-02 00:00 goodpy/f/row_key_and_value/add_key.py
 -rw-r--r--  2.0 unx        1 b- defN 20-Feb-02 00:00 goodpy/k/__init__.py
--rw-r--r--  2.0 unx     8222 b- defN 20-Feb-02 00:00 goodpy/k/dataframe.py
+-rw-r--r--  2.0 unx     9448 b- defN 20-Feb-02 00:00 goodpy/k/dataframe.py
 -rw-r--r--  2.0 unx     1539 b- defN 20-Feb-02 00:00 goodpy/k/spark_conf.py
 -rw-r--r--  2.0 unx      973 b- defN 20-Feb-02 00:00 goodpy/k/spark_context.py
 -rw-r--r--  2.0 unx      870 b- defN 20-Feb-02 00:00 goodpy/k/spark_session.py
-?rw-r--r--  2.0 unx       50 b- defN 20-Feb-02 00:00 goodpy-0.0.4.dist-info/METADATA
-?rw-r--r--  2.0 unx      105 b- defN 20-Feb-02 00:00 goodpy-0.0.4.dist-info/WHEEL
-?rw-r--r--  2.0 unx     2018 b- defN 20-Feb-02 00:00 goodpy-0.0.4.dist-info/RECORD
-24 files, 16295 bytes uncompressed, 5856 bytes compressed:  64.1%
+-rw-r--r--  2.0 unx     6024 b- defN 20-Feb-02 00:00 goodpy/k/time_series_standard_scaler.py
+?rw-r--r--  2.0 unx       50 b- defN 20-Feb-02 00:00 goodpy-0.0.5.dist-info/METADATA
+?rw-r--r--  2.0 unx      105 b- defN 20-Feb-02 00:00 goodpy-0.0.5.dist-info/WHEEL
+?rw-r--r--  2.0 unx     2114 b- defN 20-Feb-02 00:00 goodpy-0.0.5.dist-info/RECORD
+25 files, 23641 bytes uncompressed, 7584 bytes compressed:  67.9%
```

## zipnote {}

```diff
@@ -57,17 +57,20 @@
 
 Filename: goodpy/k/spark_context.py
 Comment: 
 
 Filename: goodpy/k/spark_session.py
 Comment: 
 
-Filename: goodpy-0.0.4.dist-info/METADATA
+Filename: goodpy/k/time_series_standard_scaler.py
 Comment: 
 
-Filename: goodpy-0.0.4.dist-info/WHEEL
+Filename: goodpy-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: goodpy-0.0.4.dist-info/RECORD
+Filename: goodpy-0.0.5.dist-info/WHEEL
+Comment: 
+
+Filename: goodpy-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## goodpy/k/dataframe.py

```diff
@@ -1,19 +1,25 @@
 from pyspark.sql.dataframe import DataFrame as PySparkDataFrame
 from goodpy.f.iterable_and_seperator.concat import f as concat
 from pyspark.sql.functions import collect_list as collect
 from pyspark.ml.feature import VectorAssembler as V
 from pyspark.testing import assertDataFrameEqual
+from sklearn.preprocessing import StandardScaler
+from pyspark.ml.linalg import DenseMatrix as DM
+from pyspark.ml.linalg import DenseVector as DV
 from goodpy.k.spark_session import SparkSession
+from sklearn.preprocessing import RobustScaler
 from pyspark.sql.types import BooleanType
 from pyspark.sql.functions import explode
-from pyspark.ml.linalg import DenseVector
+
 from pyspark.sql.functions import struct
 from pyspark.sql.functions import array
+from numpy import array as numpy_array
 from pyspark.sql.types import ArrayType
+from pyspark.ml.linalg import MatrixUDT
 from pyspark.sql.types import LongType
 from pyspark.sql.functions import udf
 from pyspark.sql.functions import lit
 from pyspark.sql.functions import col
 from typing_extensions import Self
 from pyspark.sql import Column
 from functools import partial
@@ -22,32 +28,40 @@
 from typing import List
 
 shift = udf(lambda x, n: x + n, LongType())
 gen_window = udf(lambda x, n: [x + i for i in range(n)], ArrayType(LongType()))
 check_len  = udf(lambda x, n: len(x) == n, BooleanType())
 c = partial(concat, seperator='-')
 
+@udf(returnType=MatrixUDT())
+def to_dense_matrix(x: list[list[float]]):
+  x = numpy_array(x)
+  return DM(x.shape[0], x.shape[1], x.T.flatten().tolist())
+
 class DataFrame(PySparkDataFrame):
   def __init__(
     self,
     data: Union[list, tuple, dict, PySparkDataFrame, 'DataFrame'],
     spark_session: SparkSession):
     if type(data) in [PySparkDataFrame, DataFrame]: df = data
     else: df = spark_session.createDataFrame(data)
     super().__init__(df._jdf, df.sparkSession)
     
   def add_vector_col(
     s: Self,
     in_cols: List[Union[Column, str]],
     out_col_name: str
   ) -> 'DataFrame':
-    return V(inputCols=in_cols, outputCol=out_col_name).transform(s)
+    return DataFrame(
+      V(inputCols=in_cols, outputCol=out_col_name).transform(s),
+      s.sparkSession
+    )
   
   def add_col(s: Self, col_name: str, col: Column ) -> 'DataFrame':
-    return super().withColumn(col_name, col)
+    return DataFrame(super().withColumn(col_name, col), s.sparkSession)
 
   def add_array_col(
     s: Self,
     in_cols: List[Union[Column, str]],
     out_col_name: str
   ) -> 'DataFrame':
     return DataFrame(s.add_col(out_col_name, array(*in_cols)), s.sparkSession)
@@ -65,24 +79,28 @@
     shift_size: int,
     out_col_name: str
   ) -> 'DataFrame':
     shifted_df = s.add_col('id', shift('id', lit(shift_size)))
     shifted_df = shifted_df.select('id', col(in_col).alias(out_col_name))
     return DataFrame(s.join(shifted_df, on='id', how='inner'), s.sparkSession)
   
-  def add_sliding_col(
+  def add_ts_col(
     s: Self,
     in_col: Union[str, Column],
     window_size: int,
     out_col_name: str
   ) -> 'DataFrame':
-    df_flatmap = s.add_col('id', explode(gen_window('id', lit(window_size))))
-    df_sliding = df_flatmap.groupBy('id').agg(collect(in_col).alias(out_col_name))
-    df_sliding = df_sliding.filter(check_len(out_col_name, lit(window_size)))
-    return DataFrame(s.join(df_sliding, on='id', how='inner'), s.sparkSession)
+    df = s.add_vector_col([in_col], 'vector')
+    df_flatmap = df.add_col('id', explode(gen_window('id', lit(window_size))))
+    df_ts = df_flatmap.groupBy('id').agg(collect('vector').alias(out_col_name))
+    df_ts = DataFrame(df_ts.filter(check_len(out_col_name, lit(window_size))), s.sparkSession)
+    df_ts = df_ts.add_col(out_col_name, to_dense_matrix(out_col_name))
+    return DataFrame(s.join(df_ts, on='id', how='inner'), s.sparkSession)
+  
+  add_time_series_col = add_ts_col
   
   def add_shifted_cols(
     s: Self,
     in_cols: list[Union[str, Column]],
     shift_size: int,
     out_col_names: list[str]
   ) -> 'DataFrame':
@@ -92,170 +110,183 @@
     s = s.add_array_col(in_cols, array_col_name)
     shifted_array_col_name = c([array_col_name] + ['shift', str(shift_size)])
     s = s.add_shifted_col(array_col_name, shift_size, shifted_array_col_name)
     shifted_col = col(shifted_array_col_name)
     cols += [shifted_col[i].alias(out_col_names[i]) for i in range(len(in_cols))]
     return DataFrame(s.select(cols), s.sparkSession)
   
-  def add_sliding_cols(
-    s: Self,
-    in_cols: list[Union[str, Column]],
-    shift_size: int,
-    out_col_names: list[str]
-  ) -> 'DataFrame':
-    cols = s.columns
-    array_col_name = c(in_cols)
-    s = s.add_array_col(in_cols, array_col_name)
-    sliding_array_col_name = c([array_col_name] + ['sliding', str(shift_size)])
-    s = s.add_sliding_col(array_col_name, shift_size, sliding_array_col_name)
-    sliding_col = col(sliding_array_col_name)
-    cols += [sliding_col[i].alias(out_col_names[i]) for i in range(len(in_cols))]
-    return DataFrame(s.select(cols), s.sparkSession)
+  # def add_ts_cols(
+  #   s: Self,
+  #   in_cols: list[Union[str, Column]],
+  #   shift_size: int,
+  #   out_col_names: list[str]
+  # ) -> 'DataFrame':
+  #   cols = s.columns
+  #   array_col_name = c(in_cols)
+  #   s = s.add_array_col(in_cols, array_col_name)
+  #   ts_array_col_name = c([array_col_name] + ['ts', str(shift_size)])
+  #   s = s.add_ts_col(array_col_name, shift_size, ts_array_col_name)
+  #   ts_col = col(ts_array_col_name)
+  #   cols += [ts_col[i].alias(out_col_names[i]) for i in range(len(in_cols))]
+  #   return DataFrame(s.select(cols), s.sparkSession)
   
+
 def f(x: dict): return DataFrame(**x)
 
 def t_add_vector_col(x: DataFrame) -> bool:
-  z = x.add_vector_col(['id', 'open'], 'vector')
+  z = x.add_vector_col(['o', 'o_and_c'], 'o_and_o_and_c')
   y = DataFrame(
     data=[
-      {'id': 1, 'open': 1, 'vector': DenseVector([1.0, 1.0])},                       
-      {'id': 2, 'open': 2, 'vector': DenseVector([2.0, 2.0])},
-      {'id': 3, 'open': 3, 'vector': DenseVector([3.0, 3.0])},
-      {'id': 4, 'open': 4, 'vector': DenseVector([4.0, 4.0])}
+      Row(id=1, o=1, c=4, o_and_c=DV([1, 4]), o_and_o_and_c = DV([1, 1, 4])),
+      Row(id=2, o=2, c=5, o_and_c=DV([2, 5]), o_and_o_and_c = DV([2, 2, 5])),
+      Row(id=3, o=3, c=6, o_and_c=DV([3, 6]), o_and_o_and_c = DV([3, 3, 6])),
+      Row(id=4, o=4, c=7, o_and_c=DV([4, 7]), o_and_o_and_c = DV([4, 4, 7]))
     ],
-    spark_session=x.sparkSession
+    spark_session=SparkSession()
   )
+  assertDataFrameEqual(z, y)
   return True
 
 def t_add_array_col(x: DataFrame) -> bool:
-  z = x.add_array_col(['id', 'open'], 'array')
+  z = x.add_array_col(['id', 'o'], 'array')
   y = DataFrame(
     [
-      Row(id=1, open=1, array=[1, 1]),
-      Row(id=2, open=2, array=[2, 2]),
-      Row(id=4, open=4, array=[4, 4]),
-      Row(id=3, open=3, array=[3, 3])
+      Row(id=1, o=1, c=4, o_and_c=DV([1, 4]), array=[1, 1]),
+      Row(id=2, o=2, c=5, o_and_c=DV([2, 5]), array=[2, 2]),
+      Row(id=3, o=3, c=6, o_and_c=DV([3, 6]), array=[3, 3]),
+      Row(id=4, o=4, c=7, o_and_c=DV([4, 7]), array=[4, 4]),
     ],
     x.sparkSession
   )
   assertDataFrameEqual(z, y)
   return True
 
 def t_add_struct_col(x: DataFrame) -> bool:
-  z = x.add_struct_col(['id', 'open'], 'struct')
+  z = x.add_struct_col(['id', 'o'], 'struct')
   y = DataFrame(
     [
-      Row(id=1, open=1, struct=Row(id=1, open=1)),                                   
-      Row(id=2, open=2, struct=Row(id=2, open=2)),
-      Row(id=3, open=3, struct=Row(id=3, open=3)),
-      Row(id=4, open=4, struct=Row(id=4, open=4))
+      Row(id=1, o=1, c=4, o_and_c=DV([1, 4]), struct=Row(id=1, o=1)),                      
+      Row(id=2, o=2, c=5, o_and_c=DV([2, 5]), struct=Row(id=2, o=2)),
+      Row(id=3, o=3, c=6, o_and_c=DV([3, 6]), struct=Row(id=3, o=3)),
+      Row(id=4, o=4, c=7, o_and_c=DV([4, 7]), struct=Row(id=4, o=4))
     ],
     x.sparkSession
   )
   assertDataFrameEqual(z, y)
   return True
 
-def t_add_shifted_col(x: DataFrame) -> bool:
-  
-  def t_add_shifted_col_shift_up(x: DataFrame) -> bool:
-    z = x.add_shifted_col('open', 2, 'shifted_open').sort('id')
+def t_add_shifted_col_shift_up(x: DataFrame) -> bool:
+    z = x.add_shifted_col('o', 2, 'shifted_o').sort('id')
     y = DataFrame(
       [
-        {'id': 3, 'open': 3, 'shifted_open': 1},                                       
-        {'id': 4, 'open': 4, 'shifted_open': 2}
+        Row(id=3, o=3, c=6, o_and_c=DV([3, 6]), shifted_o=1),
+        Row(id=4, o=4, c=7, o_and_c=DV([4, 7]), shifted_o=2)
       ],
       x.sparkSession
     )
     assertDataFrameEqual(z, y)
     return True
   
-  def t_add_shifted_col_shift_down(x: DataFrame) -> bool:
-    z = x.add_shifted_col('open', -2, 'shifted_open').sort('id')
-    y = DataFrame(
-      [
-        {'id': 1, 'open': 1, 'shifted_open': 3},
-        {'id': 2, 'open': 2, 'shifted_open': 4}
-      ],
-      x.sparkSession
-    )
-    assertDataFrameEqual(z, y)
-    return True
+def t_add_shifted_col_shift_down(x: DataFrame) -> bool:
+  z = x.add_shifted_col('o', -2, 'shifted_o').sort('id')
+  y = DataFrame(
+    [
+      Row(id=1, o=1, c=4, o_and_c=DV([1, 4]), shifted_o=3),                      
+      Row(id=2, o=2, c=5, o_and_c=DV([2, 5]), shifted_o=4)
+    ],
+    x.sparkSession
+  )
+  assertDataFrameEqual(z, y)
+  return True
   
+def t_add_shifted_col(x: DataFrame) -> bool:
   return all([t_add_shifted_col_shift_up(x), t_add_shifted_col_shift_down(x)])
 
-def t_add_sliding_col(x: DataFrame) -> bool:
+def t_add_ts_col_1(x: DataFrame) -> bool:
   y = DataFrame(
     [
-      Row(id=2, open=2, sliding_open=[1, 2]),                                        
-      Row(id=3, open=3, sliding_open=[2, 3]),
-      Row(id=4, open=4, sliding_open=[3, 4])
+      Row(id=2, o=2, c=5, o_and_c=DV([2, 5]), ts_o=DM(2, 1, [1, 2])),                                        
+      Row(id=3, o=3, c=6, o_and_c=DV([3, 6]), ts_o=DM(2, 1, [2, 3])),
+      Row(id=4, o=4, c=7, o_and_c=DV([4, 7]), ts_o=DM(2, 1, [3, 4]))
     ],
     x.sparkSession
   )
-  z = x.add_sliding_col('open', 2, 'sliding_open')
+  z = x.add_ts_col('o', 2, 'ts_o')
   assertDataFrameEqual(z, y)
   return True
 
-def t_single_column_tests():
-  x = DataFrame(
-    data=[
-      {'id': 1, 'open': 1},
-      {'id': 2, 'open': 2},
-      {'id': 3, 'open': 3},
-      {'id': 4, 'open': 4}
+def add_ts_col_2(x: DataFrame) -> bool:
+  z = x.add_ts_col('o_and_c', 2, 'ts_o_and_c')
+  y = DataFrame(
+    [
+      Row(id=2, o=2, c=5, o_and_c=DV([2, 5]), ts_o_and_c=DM(2, 2, [1, 2, 4, 5])),                                        
+      Row(id=3, o=3, c=6, o_and_c=DV([3, 6]), ts_o_and_c=DM(2, 2, [2, 3, 5, 6])),
+      Row(id=4, o=4, c=7, o_and_c=DV([4, 7]), ts_o_and_c=DM(2, 2, [3, 4, 6, 7]))
     ],
-    spark_session=SparkSession()
+    x.sparkSession
   )
+  assertDataFrameEqual(y, z)
+  return True
+  
+def t_add_ts_col(x: DataFrame) -> bool:
+  return all([t_add_ts_col_1(x), add_ts_col_2(x)])
 
+def t_single_column_tests(x):
   return all(
     [
       t_add_vector_col(x),
       t_add_array_col(x),
       t_add_struct_col(x),
       t_add_shifted_col(x),
-      t_add_sliding_col(x)
+      t_add_ts_col(x)
     ]
   )
   
 def t_add_shifted_cols(x: DataFrame):
-  z = x.add_shifted_cols(['open', 'close'], 2, ['shifted_open', 'shifted_close'])
+  z = x.add_shifted_cols(['o', 'c'], 2, ['shifted_o', 'shifted_c'])
   y = DataFrame(
     data=[
-      Row(id=3, open=3, close=4, shifted_open=1, shifted_close=2),
-      Row(id=4, open=4, close=5, shifted_open=2, shifted_close=3)
+      Row(id=3, o=3, c=6, o_and_c = DV([3, 6]), shifted_o=1, shifted_c=4),
+      Row(id=4, o=4, c=7, o_and_c = DV([4, 7]), shifted_o=2, shifted_c=5)
     ],
     spark_session=SparkSession()
   )
   assertDataFrameEqual(z, y)
   return True
 
-def t_add_sliding_cols(x: DataFrame):
-  z = x.add_sliding_cols(['open', 'close'], 2, ['sliding_open', 'sliding_close'])
+def t_add_ts_cols(x: DataFrame):
+  z = x.add_ts_cols(['o', 'c'], 2, ['ts_o', 'ts_c'])
   y = DataFrame(
     data=[
-      Row(id=2, open=2, close=3, sliding_open=[1, 2], sliding_close=[2, 3]),
-      Row(id=3, open=3, close=4, sliding_open=[2, 3], sliding_close=[3, 4]),
-      Row(id=4, open=4, close=5, sliding_open=[3, 4], sliding_close=[4, 5])
+      Row(id=2, o=2, c=3, ts_o=[1, 2], ts_c=[2, 3]),
+      Row(id=3, o=3, c=4, ts_o=[2, 3], ts_c=[3, 4]),
+      Row(id=4, o=4, c=5, ts_o=[3, 4], ts_c=[4, 5])
     ],
     spark_session=SparkSession()
   )
   assertDataFrameEqual(z, y)
   return True
   
-def t_multi_columns_tests():
+def t_multi_columns_tests(x):
+  return all(
+    [
+      t_add_shifted_cols(x),
+      # t_add_ts_cols(x)
+    ]
+  )
+  
+def t():
   x = DataFrame(
     data=[
-      Row(id=1, open=1, close=2),
-      Row(id=2, open=2, close=3),
-      Row(id=3, open=3, close=4),
-      Row(id=4, open=4, close=5)
+      Row(id=1, o=1, c=4, o_and_c=DV([1, 4])),
+      Row(id=2, o=2, c=5, o_and_c=DV([2, 5])),
+      Row(id=3, o=3, c=6, o_and_c=DV([3, 6])),
+      Row(id=4, o=4, c=7, o_and_c=DV([4, 7]))
     ],
     spark_session=SparkSession()
   )
   return all(
     [
-      t_add_shifted_cols(x),
-      t_add_sliding_cols(x)
+      t_single_column_tests(x),
+      t_multi_columns_tests(x)
     ]
   )
-  
-def t(): return all([t_single_column_tests(), t_multi_columns_tests()])
```

## Comparing `goodpy-0.0.4.dist-info/RECORD` & `goodpy-0.0.5.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 goodpy/f/num1_and_num2/__init__.py,sha256=6IQwo48SoTNvAQvveZho8aaFrbh2M9hQGLjXd6qNjj8,61
 goodpy/f/num1_and_num2/check_if_greater_than.py,sha256=RMnfD1UGEEVvtSG1rP3wgUr79tepprvGCkzHsHRvfks,75
 goodpy/f/row_and_keys/__init__.py,sha256=CGe-Uswik2tSH4Zph6SOLYW143AJlSo8AeO9k36aLvs,43
 goodpy/f/row_and_keys/get_keys_row.py,sha256=oXPz4Bxvuc5bt6abbd4QEL_IzydL8zq-YF8qFcKC8NU,205
 goodpy/f/row_key_and_value/__init__.py,sha256=Bg_ieuYVK61m1hZdEb5pkhpQK6ndhjTg_AL8Kd4IxiU,33
 goodpy/f/row_key_and_value/add_key.py,sha256=36dKFkdGvrpwvCUz00zYT4-f6uNxRGcukhk1cP-Ll8E,355
 goodpy/k/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-goodpy/k/dataframe.py,sha256=C3eoCU9gBYvD6Sr4Pz2MLAxnUx65mTB0D8_vfWLPiXM,8222
+goodpy/k/dataframe.py,sha256=QZIxmi6iR4PUcG6TkQRI81-LMTEUZcNY1HHuzaG6_qY,9448
 goodpy/k/spark_conf.py,sha256=h3a_qubJKHAC3-DkfvzjYgaHpf5pd3rkE-64FdkQyJM,1539
 goodpy/k/spark_context.py,sha256=V1-KtsXfzzuyXG4WMw6RGZPVygkClQvS_RXgmZnrxiM,973
 goodpy/k/spark_session.py,sha256=hmltKLoHKDae1VFBff0sF3RMq_gI3tZi1ECLIBpz66A,870
-goodpy-0.0.4.dist-info/METADATA,sha256=X-w7RSXdfT4AoiDNiUv7eY5Yd-meJbenRO-5ay_Mi8U,50
-goodpy-0.0.4.dist-info/WHEEL,sha256=cDcbFFSNXOE-241I5PFuLkIYfR_FM7WTlPEi33njInY,105
-goodpy-0.0.4.dist-info/RECORD,,
+goodpy/k/time_series_standard_scaler.py,sha256=7P2m8VBkHptJ8lTJ440OIppQIO1N3zDj6HhpofUf63s,6024
+goodpy-0.0.5.dist-info/METADATA,sha256=X3A5y7-_5w8GqZCBxx-pD9A_aPnc4yQbuzmsjxMH5gE,50
+goodpy-0.0.5.dist-info/WHEEL,sha256=cDcbFFSNXOE-241I5PFuLkIYfR_FM7WTlPEi33njInY,105
+goodpy-0.0.5.dist-info/RECORD,,
```

