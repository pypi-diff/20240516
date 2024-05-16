# Comparing `tmp/goodpy-0.0.5-py2.py3-none-any.whl.zip` & `tmp/goodpy-0.0.6-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 11064 bytes, number of entries: 25
+Zip file size: 11081 bytes, number of entries: 25
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 goodpy/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 goodpy/f/__init__.py
 -rw-r--r--  2.0 unx       54 b- defN 20-Feb-02 00:00 goodpy/f/date/__init__.py
 -rw-r--r--  2.0 unx      789 b- defN 20-Feb-02 00:00 goodpy/f/date/get_date_last_friday.py
 -rw-r--r--  2.0 unx       31 b- defN 20-Feb-02 00:00 goodpy/f/dict_key_and_value/__init__.py
 -rw-r--r--  2.0 unx      127 b- defN 20-Feb-02 00:00 goodpy/f/dict_key_and_value/update.py
 -rw-r--r--  2.0 unx       29 b- defN 20-Feb-02 00:00 goodpy/f/dirpath/__init__.py
@@ -12,16 +12,16 @@
 -rw-r--r--  2.0 unx       61 b- defN 20-Feb-02 00:00 goodpy/f/num1_and_num2/__init__.py
 -rw-r--r--  2.0 unx       75 b- defN 20-Feb-02 00:00 goodpy/f/num1_and_num2/check_if_greater_than.py
 -rw-r--r--  2.0 unx       43 b- defN 20-Feb-02 00:00 goodpy/f/row_and_keys/__init__.py
 -rw-r--r--  2.0 unx      205 b- defN 20-Feb-02 00:00 goodpy/f/row_and_keys/get_keys_row.py
 -rw-r--r--  2.0 unx       33 b- defN 20-Feb-02 00:00 goodpy/f/row_key_and_value/__init__.py
 -rw-r--r--  2.0 unx      355 b- defN 20-Feb-02 00:00 goodpy/f/row_key_and_value/add_key.py
 -rw-r--r--  2.0 unx        1 b- defN 20-Feb-02 00:00 goodpy/k/__init__.py
--rw-r--r--  2.0 unx     9448 b- defN 20-Feb-02 00:00 goodpy/k/dataframe.py
+-rw-r--r--  2.0 unx     9447 b- defN 20-Feb-02 00:00 goodpy/k/dataframe.py
 -rw-r--r--  2.0 unx     1539 b- defN 20-Feb-02 00:00 goodpy/k/spark_conf.py
 -rw-r--r--  2.0 unx      973 b- defN 20-Feb-02 00:00 goodpy/k/spark_context.py
 -rw-r--r--  2.0 unx      870 b- defN 20-Feb-02 00:00 goodpy/k/spark_session.py
--rw-r--r--  2.0 unx     6024 b- defN 20-Feb-02 00:00 goodpy/k/time_series_standard_scaler.py
-?rw-r--r--  2.0 unx       50 b- defN 20-Feb-02 00:00 goodpy-0.0.5.dist-info/METADATA
-?rw-r--r--  2.0 unx      105 b- defN 20-Feb-02 00:00 goodpy-0.0.5.dist-info/WHEEL
-?rw-r--r--  2.0 unx     2114 b- defN 20-Feb-02 00:00 goodpy-0.0.5.dist-info/RECORD
-25 files, 23641 bytes uncompressed, 7584 bytes compressed:  67.9%
+-rw-r--r--  2.0 unx     6821 b- defN 20-Feb-02 00:00 goodpy/k/time_series_standard_scaler.py
+?rw-r--r--  2.0 unx       50 b- defN 20-Feb-02 00:00 goodpy-0.0.6.dist-info/METADATA
+?rw-r--r--  2.0 unx      105 b- defN 20-Feb-02 00:00 goodpy-0.0.6.dist-info/WHEEL
+?rw-r--r--  2.0 unx     2114 b- defN 20-Feb-02 00:00 goodpy-0.0.6.dist-info/RECORD
+25 files, 24437 bytes uncompressed, 7601 bytes compressed:  68.9%
```

## zipnote {}

```diff
@@ -60,17 +60,17 @@
 
 Filename: goodpy/k/spark_session.py
 Comment: 
 
 Filename: goodpy/k/time_series_standard_scaler.py
 Comment: 
 
-Filename: goodpy-0.0.5.dist-info/METADATA
+Filename: goodpy-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: goodpy-0.0.5.dist-info/WHEEL
+Filename: goodpy-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: goodpy-0.0.5.dist-info/RECORD
+Filename: goodpy-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## goodpy/k/dataframe.py

```diff
@@ -6,15 +6,14 @@
 from sklearn.preprocessing import StandardScaler
 from pyspark.ml.linalg import DenseMatrix as DM
 from pyspark.ml.linalg import DenseVector as DV
 from goodpy.k.spark_session import SparkSession
 from sklearn.preprocessing import RobustScaler
 from pyspark.sql.types import BooleanType
 from pyspark.sql.functions import explode
-
 from pyspark.sql.functions import struct
 from pyspark.sql.functions import array
 from numpy import array as numpy_array
 from pyspark.sql.types import ArrayType
 from pyspark.ml.linalg import MatrixUDT
 from pyspark.sql.types import LongType
 from pyspark.sql.functions import udf
```

## goodpy/k/time_series_standard_scaler.py

```diff
@@ -33,22 +33,17 @@
     StructField('mean_', ArrayType(FloatType()), nullable=False),
     StructField('scale_', ArrayType(FloatType()), nullable=True),
     StructField('var_', ArrayType(FloatType()), nullable=True),
   ]
 )
 
 @udf(returnType=schema)
-def fit_ts(
-  x: DM,
-  with_mean: bool,
-  with_std: bool
-)->SS:
+def fit_ts(x: DM, with_mean: bool, with_std: bool)->SS:
   scaler = SS(with_mean=with_mean, with_std=with_std)
-  x = x.toArray()
-  scaler.fit(x if len(x.shape) > 1 else x.reshape(-1, 1))
+  scaler.fit(x.toArray())
   dict_params = scaler.__dict__
   dict_params['n_features_in'] = int(scaler.n_features_in_)
   dict_params['n_samples_seen_'] = int(scaler.n_samples_seen_)
   dict_params['mean_'] = scaler.mean_.tolist()
   dict_params['var_'] = scaler.var_.tolist()
   dict_params['scale_'] = scaler.scale_.tolist()
   return dict_params
@@ -63,15 +58,15 @@
   scaler.n_features_in_ = array(scaler_dict['n_features_in_'])
   scaler.n_samples_seen_ = array(scaler_dict['n_samples_seen_'])
   scaler.mean_ = array(scaler_dict['mean_'])
   scaler.var_ = array(scaler_dict['var_'])
   scaler.scale_ = array(scaler_dict['scale_'])
   z = DM(x.numRows, x.numCols, scaler.transform(x.toArray()).T.flatten().tolist())
   return z
-  
+
 @udf(returnType=MatrixUDT())
 def inverse_transform_ts(x: DM, scaler_dict: dict):
   scaler = SS(
     copy=True,
     with_mean=scaler_dict['with_mean'],
     with_std=scaler_dict['with_std']
   )
@@ -79,41 +74,47 @@
   scaler.n_samples_seen_ = array(scaler_dict['n_samples_seen_'])
   scaler.mean_ = array(scaler_dict['mean_'])
   scaler.var_ = array(scaler_dict['var_'])
   scaler.scale_ = array(scaler_dict['scale_'])
   z_numpy = scaler.inverse_transform(x.toArray())
   z = DM(x.numRows, x.numCols, z_numpy.T.flatten().tolist())
   return z
+
+@udf(returnType=MatrixUDT())
+def fit_transform_ts(x: DM, with_mean: bool, with_std: bool) -> SS:
+  scaler = SS(with_mean=with_mean, with_std=with_std)
+  z_numpy = scaler.fit_transform(x.toArray())
+  return DM(x.numRows, x.numCols, z_numpy.T.flatten().tolist())
   
 @dataclass 
 class TimeSeriesStandardScaler:
   in_col      : str
   out_col     : str
   with_mean   : bool = True
   with_std    : bool = True
    
-  wm = property(lambda s: s.with_mean)
-  ws = property(lambda s: s.with_std)
+  wm = property(lambda s: lit(s.with_mean))
+  ws = property(lambda s: lit(s.with_std))
   
   def fit(s: Self, df: DataFrame):
     x = df.select('id', s.in_col)
-    s.parameters = df.add_col(
-      'parameters',
-      fit_ts(s.in_col, lit(s.wm), lit(s.ws))
-    )
+    s.parameters = df.add_col('parameters', fit_ts(s.in_col, s.wm, s.ws))
     s.parameters = s.parameters.select('id', 'parameters')
     s.parameters = DataFrame(s.parameters, s.parameters.sparkSession)
     return s
   
   def transform(s: Self, df: DataFrame):
     df = DataFrame(df.join(s.parameters, on='id', how='inner'), df.sparkSession)
     df = df.add_col(s.out_col, transform_ts(s.in_col, 'parameters'))
     df = df.drop('parameters')
     return DataFrame(df, df.sparkSession)
   
+  def fit_transform(s: Self, df: DataFrame):
+    return df.add_col(s.out_col, fit_transform_ts(s.in_col, s.wm, s.ws))
+  
   def inverse_transform(s: Self, df: DataFrame):
     df = DataFrame(df.join(s.parameters, on='id', how='inner'), df.sparkSession)
     inverse_name = concat([s.in_col, 'recreated'], '_')
     df = df.add_col(
       inverse_name,
       inverse_transform_ts(s.out_col, 'parameters')
     )
@@ -144,14 +145,27 @@
       Row(id=2, s_ts=DM(2, 2, [-1, 1, -1, 1]), ts_recreated=DM(2, 2, [1, 2, 4, 5])),                                        
       Row(id=3, s_ts=DM(2, 2, [-1, 1, -1, 1]), ts_recreated=DM(2, 2, [2, 3, 5, 6])),
       Row(id=4, s_ts=DM(2, 2, [-1, 1, -1, 1]), ts_recreated=DM(2, 2, [3, 4, 6, 7]))
     ],
     SparkSession()
   )
   assertDataFrameEqual(y, z)
+  
+def t_fit_transform(x: DataFrame, scaler: TimeSeriesStandardScaler):
+  z = scaler.fit_transform(x)
+  y = DataFrame(
+    [
+      Row(id=2, ts=DM(2, 2, [1, 2, 4, 5]), s_ts=DM(2, 2, [-1, 1, -1, 1])),                                        
+      Row(id=3, ts=DM(2, 2, [2, 3, 5, 6]), s_ts=DM(2, 2, [-1, 1, -1, 1])),
+      Row(id=4, ts=DM(2, 2, [3, 4, 6, 7]), s_ts=DM(2, 2, [-1, 1, -1, 1]))
+    ],
+    SparkSession()
+  )
+  assertDataFrameEqual(y, z)
+  return True
 
 def t():
   x1 = DataFrame(
     [
       Row(id=2, ts=DM(2, 2, [1, 2, 4, 5])),                                        
       Row(id=3, ts=DM(2, 2, [2, 3, 5, 6])),
       Row(id=4, ts=DM(2, 2, [3, 4, 6, 7]))
@@ -166,9 +180,10 @@
     ],
     SparkSession()
   )
   
   scaler = t_fit(x1, TimeSeriesStandardScaler('ts', 's_ts'))
   t_transform(x1, scaler)
   t_inverse_transform(x2, scaler)
+  t_fit_transform(x1, scaler)
   return True
```

## Comparing `goodpy-0.0.5.dist-info/RECORD` & `goodpy-0.0.6.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 goodpy/f/num1_and_num2/__init__.py,sha256=6IQwo48SoTNvAQvveZho8aaFrbh2M9hQGLjXd6qNjj8,61
 goodpy/f/num1_and_num2/check_if_greater_than.py,sha256=RMnfD1UGEEVvtSG1rP3wgUr79tepprvGCkzHsHRvfks,75
 goodpy/f/row_and_keys/__init__.py,sha256=CGe-Uswik2tSH4Zph6SOLYW143AJlSo8AeO9k36aLvs,43
 goodpy/f/row_and_keys/get_keys_row.py,sha256=oXPz4Bxvuc5bt6abbd4QEL_IzydL8zq-YF8qFcKC8NU,205
 goodpy/f/row_key_and_value/__init__.py,sha256=Bg_ieuYVK61m1hZdEb5pkhpQK6ndhjTg_AL8Kd4IxiU,33
 goodpy/f/row_key_and_value/add_key.py,sha256=36dKFkdGvrpwvCUz00zYT4-f6uNxRGcukhk1cP-Ll8E,355
 goodpy/k/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-goodpy/k/dataframe.py,sha256=QZIxmi6iR4PUcG6TkQRI81-LMTEUZcNY1HHuzaG6_qY,9448
+goodpy/k/dataframe.py,sha256=HtkDHQOzb-igPCsgo72ZJQhqHozTqfB-1ULmf7klbj8,9447
 goodpy/k/spark_conf.py,sha256=h3a_qubJKHAC3-DkfvzjYgaHpf5pd3rkE-64FdkQyJM,1539
 goodpy/k/spark_context.py,sha256=V1-KtsXfzzuyXG4WMw6RGZPVygkClQvS_RXgmZnrxiM,973
 goodpy/k/spark_session.py,sha256=hmltKLoHKDae1VFBff0sF3RMq_gI3tZi1ECLIBpz66A,870
-goodpy/k/time_series_standard_scaler.py,sha256=7P2m8VBkHptJ8lTJ440OIppQIO1N3zDj6HhpofUf63s,6024
-goodpy-0.0.5.dist-info/METADATA,sha256=X3A5y7-_5w8GqZCBxx-pD9A_aPnc4yQbuzmsjxMH5gE,50
-goodpy-0.0.5.dist-info/WHEEL,sha256=cDcbFFSNXOE-241I5PFuLkIYfR_FM7WTlPEi33njInY,105
-goodpy-0.0.5.dist-info/RECORD,,
+goodpy/k/time_series_standard_scaler.py,sha256=jucJ1nbbozxNcByRlCxcEUpsmOcb0XDTRYGKhMTZDAs,6821
+goodpy-0.0.6.dist-info/METADATA,sha256=elj_qvyf7hZSf8u60VFhbCf44pCTbBvBwX_8TgnMKII,50
+goodpy-0.0.6.dist-info/WHEEL,sha256=cDcbFFSNXOE-241I5PFuLkIYfR_FM7WTlPEi33njInY,105
+goodpy-0.0.6.dist-info/RECORD,,
```

