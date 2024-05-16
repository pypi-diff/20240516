# Comparing `tmp/karnak-3.3.7-py3-none-any.whl.zip` & `tmp/karnak-3.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,34 +1,34 @@
-Zip file size: 73737 bytes, number of entries: 54
+Zip file size: 74048 bytes, number of entries: 54
 -rw-r--r--  2.0 unx    38872 b- defN 23-Jul-17 17:42 karnak/fetcher/karnak_sqs_fetcher.py
 -rw-r--r--  2.0 unx    19733 b- defN 23-Nov-25 23:31 karnak/fetcher/sqs_fetcher.py
 -rw-r--r--  2.0 unx      951 b- defN 23-Jul-17 17:42 karnak/util/argparse.py
 -rw-r--r--  2.0 unx     5988 b- defN 23-Jul-17 17:42 karnak/util/athena.py
 -rw-r--r--  2.0 unx     2112 b- defN 23-Jul-17 17:42 karnak/util/db.py
 -rw-r--r--  2.0 unx     3029 b- defN 23-Jul-17 17:42 karnak/util/log.py
 -rw-r--r--  2.0 unx      625 b- defN 23-Jul-17 17:42 karnak/util/path.py
 -rw-r--r--  2.0 unx     5318 b- defN 23-Jul-17 17:42 karnak/util/profiling.py
 -rw-r--r--  2.0 unx     2556 b- defN 23-Jul-17 17:42 karnak/util/redshift.py
 -rw-r--r--  2.0 unx     4112 b- defN 23-Jul-17 17:42 karnak/util/aws/sqs.py
 -rw-r--r--  2.0 unx      235 b- defN 23-Jul-17 17:42 karnak3/cloud/__init__.py
 -rw-r--r--  2.0 unx     1284 b- defN 23-Jul-17 17:42 karnak3/cloud/aws/__init__.py
--rw-r--r--  2.0 unx    10848 b- defN 23-Nov-26 00:11 karnak3/cloud/aws/athena.py
+-rw-r--r--  2.0 unx    10848 b- defN 24-May-16 11:10 karnak3/cloud/aws/athena.py
 -rw-r--r--  2.0 unx     2707 b- defN 23-Jul-17 17:42 karnak3/cloud/aws/s3.py
 -rw-r--r--  2.0 unx     9908 b- defN 23-Jul-17 17:42 karnak3/cloud/aws/sqs.py
 -rw-r--r--  2.0 unx     1310 b- defN 23-Jul-17 17:42 karnak3/cloud/aws/ssm.py
 -rw-r--r--  2.0 unx      551 b- defN 23-Jul-17 17:42 karnak3/cloud/aws/sts.py
--rw-r--r--  2.0 unx     1894 b- defN 23-Jul-17 17:42 karnak3/cloud/aws/redshift/__init__.py
+-rw-r--r--  2.0 unx     2096 b- defN 24-May-16 19:13 karnak3/cloud/aws/redshift/__init__.py
 -rw-r--r--  2.0 unx     1021 b- defN 23-Jul-17 17:42 karnak3/cloud/aws/redshift/legacy.py
 -rw-r--r--  2.0 unx     8645 b- defN 23-Jul-17 17:42 karnak3/core/arg.py
 -rw-r--r--  2.0 unx     1212 b- defN 23-Nov-25 22:34 karnak3/core/config.py
 -rw-r--r--  2.0 unx     1374 b- defN 23-Jul-17 17:42 karnak3/core/dataframe.py
 -rw-r--r--  2.0 unx     6409 b- defN 23-Jul-17 17:42 karnak3/core/engine_registry.py
 -rw-r--r--  2.0 unx     7790 b- defN 23-Jul-17 17:42 karnak3/core/profiling.py
 -rw-r--r--  2.0 unx    18331 b- defN 23-Jul-17 17:42 karnak3/core/time_window.py
--rw-r--r--  2.0 unx    10105 b- defN 24-May-07 15:42 karnak3/core/db/__init__.py
+-rw-r--r--  2.0 unx    12898 b- defN 24-May-16 19:16 karnak3/core/db/__init__.py
 -rw-r--r--  2.0 unx     5155 b- defN 23-Jul-17 17:42 karnak3/core/log/__init__.py
 -rw-r--r--  2.0 unx     2310 b- defN 23-Jul-17 17:42 karnak3/core/log/legacy.py
 -rw-r--r--  2.0 unx     4604 b- defN 23-Jul-17 17:42 karnak3/core/store/__init__.py
 -rw-r--r--  2.0 unx     2770 b- defN 23-Jul-17 17:42 karnak3/core/store/file.py
 -rw-r--r--  2.0 unx     1143 b- defN 23-Jul-17 17:42 karnak3/core/util/__init__.py
 -rw-r--r--  2.0 unx     1687 b- defN 23-Nov-25 23:30 karnak3/core/util/collections.py
 -rw-r--r--  2.0 unx     1062 b- defN 23-Jul-17 17:42 karnak3/core/util/compression.py
@@ -44,13 +44,13 @@
 -rw-r--r--  2.0 unx    16487 b- defN 23-Nov-25 23:29 karnak3/fetch/sqs_fetcher.py
 -rw-r--r--  2.0 unx     1099 b- defN 23-Jul-17 17:42 test/integration/util/athena/run_athena_select.py
 -rw-r--r--  2.0 unx      490 b- defN 23-Jul-17 17:42 test/unit/karnak3/core/arg.py
 -rw-r--r--  2.0 unx     1593 b- defN 23-Jul-17 17:42 test/unit/karnak3/core/test_log.py
 -rw-r--r--  2.0 unx     8498 b- defN 23-Jul-17 17:42 test/unit/karnak3/core/test_time_window.py
 -rw-r--r--  2.0 unx      680 b- defN 23-Jul-17 17:42 test/unit/karnak3/core/util/test_datetime.py
 -rw-r--r--  2.0 unx      622 b- defN 23-Jul-17 17:42 test/unit/karnak3/core/util/test_path.py
--rw-r--r--  2.0 unx     1058 b- defN 24-May-07 15:43 karnak-3.3.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     1771 b- defN 24-May-07 15:43 karnak-3.3.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-07 15:43 karnak-3.3.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       35 b- defN 24-May-07 15:43 karnak-3.3.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     4547 b- defN 24-May-07 15:43 karnak-3.3.7.dist-info/RECORD
-54 files, 265765 bytes uncompressed, 66543 bytes compressed:  75.0%
+-rw-r--r--  2.0 unx     1058 b- defN 24-May-16 19:37 karnak-3.4.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1789 b- defN 24-May-16 19:37 karnak-3.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-16 19:37 karnak-3.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       35 b- defN 24-May-16 19:37 karnak-3.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     4547 b- defN 24-May-16 19:37 karnak-3.4.0.dist-info/RECORD
+54 files, 268778 bytes uncompressed, 66854 bytes compressed:  75.1%
```

## zipnote {}

```diff
@@ -141,23 +141,23 @@
 
 Filename: test/unit/karnak3/core/util/test_datetime.py
 Comment: 
 
 Filename: test/unit/karnak3/core/util/test_path.py
 Comment: 
 
-Filename: karnak-3.3.7.dist-info/LICENSE
+Filename: karnak-3.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: karnak-3.3.7.dist-info/METADATA
+Filename: karnak-3.4.0.dist-info/METADATA
 Comment: 
 
-Filename: karnak-3.3.7.dist-info/WHEEL
+Filename: karnak-3.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: karnak-3.3.7.dist-info/top_level.txt
+Filename: karnak-3.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: karnak-3.3.7.dist-info/RECORD
+Filename: karnak-3.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## karnak3/cloud/aws/redshift/__init__.py

```diff
@@ -1,9 +1,11 @@
 from typing import Optional, Dict
 import pandas as pd
+import pyarrow as pa
+import polars as pl
 
 import redshift_connector
 import sqlalchemy.pool
 
 from karnak3.core.db import KSqlAlchemyEngine
 import karnak3.core.arg as karg
 
@@ -36,14 +38,19 @@
                                           database=self.config.database,
                                           user=self.config.user,
                                           password=self.config.password)
 
     def _result_pd(self, cursor, result) -> Optional[pd.DataFrame]:
         return cursor.fetch_dataframe()
 
+    def _result_pl(self, cursor, result) -> Optional[pl.DataFrame]:
+        df = cursor.fetch_dataframe()
+        pl_df = pl.DataFrame(df)
+        return pl_df
+
 
 def get_runtime_config(args: Optional[Dict[str, str]] = None):
     """read configuration from arguments or environment"""
 
     host = karg.best_arg('redshift_host', args)
     database = karg.best_arg('redshift_database', args)
     user = karg.best_arg('redshift_user', args)
```

## karnak3/core/db/__init__.py

```diff
@@ -1,20 +1,21 @@
 import contextlib
 import numbers
-from abc import abstractmethod
+from abc import abstractmethod, ABC
 from concurrent.futures import Future, ThreadPoolExecutor
 from typing import Union, Optional, Tuple, Any
 import collections.abc
 import re
 import datetime
 
 import sqlalchemy.pool
 import sqlparams
 import pandas as pd
 import pyarrow as pa
+import polars as pl
 
 import karnak3.core.log as kl
 import karnak3.core.util as ku
 
 _logger = kl.KLog(__name__)
 
 
@@ -115,23 +116,44 @@
 
     def to_df(self, timeout=None, save_memory: bool = False) -> Optional[pd.DataFrame]:
         return self.df
 
 
 class KArrowTableFuture(KPandasDataFrameFuture):
     @abstractmethod
-    def to_table(self, timeout=None) -> Optional[pd.DataFrame]:
+    def to_table(self, timeout=None) -> Optional[pa.Table]:
+        pass
+
+
+class KPolarsDataFrameFuture(KArrowTableFuture):
+    @abstractmethod
+    def to_pl(self, timeout=None) -> Optional[pl.DataFrame]:
         pass
 
 
+class KPolarsDataFrameFutureArrowWrapper(KPolarsDataFrameFuture):
+
+    def __init__(self, k_arrow_table_future: KArrowTableFuture):
+        self.k_arrow_table_future = k_arrow_table_future
+
+    def to_pl(self, timeout=None) -> Optional[pl.DataFrame]:
+        pat = self.to_table(timeout=timeout)
+        return pl.DataFrame(pat) if pat is not None else None
+
+    def to_table(self, timeout=None) -> Optional[pd.DataFrame]:
+        return self.k_arrow_table_future.to_table(timeout=timeout)
+
+    def to_df(self, timeout=None, save_memory: bool = False) -> Optional[pd.DataFrame]:
+        return self.k_arrow_table_future.to_df(timeout=timeout, save_memory=save_memory)
+
+
 class KarnakDBException(ku.KarnakException):
     pass
 
 
-
 class KSqlAlchemyEngine:
     def __init__(self, engine_name: str,
                  paramstyle_client: str,
                  paramstyle_driver: str,
                  async_enabled: bool = False):
         self.engine_name = engine_name
         self.paramstyle_client = paramstyle_client
@@ -161,20 +183,29 @@
     @abstractmethod
     def _result_pd(self, cursor, result) -> Optional[pd.DataFrame]:
         pass
 
     def _result_pa(self, cursor, result) -> Optional[pa.Table]:
         raise ku.KarnakInternalError('method not implememented: _result_pa')
 
+    def _result_pl(self, cursor, result) -> Optional[pl.DataFrame]:
+        pat = self._result_pa(cursor=cursor, result=result)
+        return pl.DataFrame(pat) if pat is not None else None
+
     def _result_pd_async(self, cursor, result) -> KPandasDataFrameFuture:
         raise ku.KarnakInternalError('method not implememented: _result_pd_async')
 
     def _result_pa_async(self, cursor, result) -> KArrowTableFuture:
         raise ku.KarnakInternalError('method not implememented: _result_pa_async')
 
+    def _result_pl_async(self, cursor, result) -> KPolarsDataFrameFuture:
+        wrapped_future_arrow: KArrowTableFuture = self._result_pa_async(cursor, result)
+        wrapped_future_polars = KPolarsDataFrameFutureArrowWrapper(wrapped_future_arrow)
+        return wrapped_future_polars
+
     # TEST compatibility with other libs
     def test_libs_compatibility(self):
         from sklearn.preprocessing import MinMaxScaler, PowerTransformer
         data = [[-1, 2], [-0.5, 6], [0, 10], [1, 18]]
         scaler = MinMaxScaler()
         xpto = scaler.fit(data)
         kl.trace('****** test_libs compatibility ok ****** ')
@@ -213,14 +244,32 @@
         with contextlib.closing(self._connection()) as conn:
             with conn.cursor() as cursor:
                 result = self._cursor_execute(cursor, _sql, _params)
                 result_pa = self._result_pa(cursor, result)
                 del result
                 return result_pa
 
+    def select_pl(self, sql: str,
+                  params: Union[dict, list, None] = None,
+                  paramstyle: str = None) -> pl.DataFrame:
+        _sql, _params = self._convert_sql(sql=sql, params=params, paramstyle=paramstyle)
+        with contextlib.closing(self._connection()) as conn:
+            with conn.cursor() as cursor:
+                result = self._cursor_execute(cursor, _sql, _params)
+                result_pl = self._result_pl(cursor, result)
+                del result
+                return result_pl
+
+    #
+    # def select_pl(self, sql: str,
+    #               params: Union[dict, list, None] = None,
+    #               paramstyle: str = None) -> pl.DataFrame:
+    #     pat = self.select_pa(sql=sql, params=params, paramstyle=paramstyle)
+    #     return pl.DataFrame(pat) if pat is not None else None
+
     def select_pd(self, sql: str,
                   params: Union[dict, list, None] = None,
                   paramstyle: str = None) -> pd.DataFrame:
         _sql, _params = self._convert_sql(sql=sql, params=params, paramstyle=paramstyle)
         with contextlib.closing(self._connection()) as conn:
             with conn.cursor() as cursor:
                 result = self._cursor_execute(cursor, _sql, _params)
@@ -261,7 +310,19 @@
         _cursor_params = self._cursor_params()
         with contextlib.closing(self._connection()) as conn:
             with conn.cursor(**_cursor_params) as cursor:
                 result = self._cursor_execute(cursor, _sql, _params)
                 wrapped_future = self._result_pd_async(cursor, result)
                 del result
                 return wrapped_future
+
+    def select_pl_async(self, sql: str,
+                        params: Union[dict, list, None] = None,
+                        paramstyle: str = None) -> KPolarsDataFrameFuture:
+        _sql, _params = self._convert_sql(sql=sql, params=params, paramstyle=paramstyle)
+        _cursor_params = self._cursor_params()
+        with contextlib.closing(self._connection()) as conn:
+            with conn.cursor(**_cursor_params) as cursor:
+                result = self._cursor_execute(cursor, _sql, _params)
+                wrapped_future = self._result_pl_async(cursor, result)
+                del result
+                return wrapped_future
```

## Comparing `karnak-3.3.7.dist-info/LICENSE` & `karnak-3.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `karnak-3.3.7.dist-info/METADATA` & `karnak-3.4.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: karnak
-Version: 3.3.7
+Version: 3.4.0
 Summary: Karnak Data Platform Community Edition
 Home-page: https://github.com/cogitaslabs/karnak-community
 Author: Leonardo Rossi
 Author-email: leorossi@cogitaslabs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -20,23 +20,24 @@
 Requires-Dist: python-dateutil
 Requires-Dist: orjson
 Requires-Dist: brotli
 Requires-Dist: sqlparams
 Requires-Dist: sqlalchemy
 Requires-Dist: tzlocal
 Requires-Dist: pyarrow
+Requires-Dist: polars
 Provides-Extra: aws
 Requires-Dist: boto3 ; extra == 'aws'
 Requires-Dist: redshift-connector ; extra == 'aws'
-Requires-Dist: PyAthena (>=2.4.1) ; extra == 'aws'
+Requires-Dist: PyAthena >=2.4.1 ; extra == 'aws'
 Requires-Dist: PyAthenaJDBC[sqlalchemy] ; extra == 'aws'
 Provides-Extra: full
 Requires-Dist: boto3 ; extra == 'full'
 Requires-Dist: redshift-connector ; extra == 'full'
-Requires-Dist: PyAthena (>=2.4.1) ; extra == 'full'
+Requires-Dist: PyAthena >=2.4.1 ; extra == 'full'
 Requires-Dist: PyAthenaJDBC[sqlalchemy] ; extra == 'full'
 Provides-Extra: gcp
 
 # Karnak Data Platform Community Edition
 
 Karnak Data Platform is an opinionated framework for building big data and machine learning systems.
```

## Comparing `karnak-3.3.7.dist-info/RECORD` & `karnak-3.4.0.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 karnak3/cloud/__init__.py,sha256=G0mG9bcvLSw3d5bVp9kL90FAlttrLqGOXJWYbjn1k1c,235
 karnak3/cloud/aws/__init__.py,sha256=7vwwVXhwdyfjVKm5-ot9w39O1OksTmxP71lIyd_ukFU,1284
 karnak3/cloud/aws/athena.py,sha256=msM5k98bWrd8L-6xpghqOZ-SmmTkVtY9N4hoxySDG_8,10848
 karnak3/cloud/aws/s3.py,sha256=A7To1AhY1MzvMhKhyEDH5pMTE-FmvzmpBq8okANEBcs,2707
 karnak3/cloud/aws/sqs.py,sha256=Oha6RM7yIgy-_AFRgBkjy-DHILsUdEqqPhA-pb3Wxys,9908
 karnak3/cloud/aws/ssm.py,sha256=LPPX2MKhXKrnwQbmbchFEWuliodYBQQazBlGGpn76w0,1310
 karnak3/cloud/aws/sts.py,sha256=9Fe_UN78dDp0zQobrok-UU8IlIST9g4aE4WFTi1wKFs,551
-karnak3/cloud/aws/redshift/__init__.py,sha256=_v8plG6t90gnt8JgYjcriuJ4Ep-CX4mPgh-O-Rx3KIQ,1894
+karnak3/cloud/aws/redshift/__init__.py,sha256=JgRea1XB1jPiCmkUrsp3YpiqcDsrre27HpkBOPwfasg,2096
 karnak3/cloud/aws/redshift/legacy.py,sha256=qkr2kkCn8q5vEec2mnY00N53SRsr7ABE6ZioOkm-8no,1021
 karnak3/core/arg.py,sha256=Av49aOIaWVEKchsAZPKp2axrqq437q1w5joJQ-rRs-o,8645
 karnak3/core/config.py,sha256=H1G2HUJ5bOhHvjm3Sc1ndL94euu8HI4l1jzuSe3ThoY,1212
 karnak3/core/dataframe.py,sha256=144HV2UJS8R_wcVVdjl9GcBap1q0f-NIgH7YAR_pOgU,1374
 karnak3/core/engine_registry.py,sha256=srbZnpUm1SRfEkL1XzQEIHCq7Xs3ab-T_yuO2NNjPqQ,6409
 karnak3/core/profiling.py,sha256=XbU1hTj3raykwTJUAWbeYPN7GH6Ss0uTbeg1eju3AZw,7790
 karnak3/core/time_window.py,sha256=KHh0w1CqdZABDuXOSNp511Za0tt8n-qtbKxLlOLkhB4,18331
-karnak3/core/db/__init__.py,sha256=R94ek7xU--Gb4RCNWlzQIFQzOLLdjPNRoc2_gXPmiRo,10105
+karnak3/core/db/__init__.py,sha256=jqSmm2zbvvDFX6FIm7OlIi0kz2ZrQ8aAhtH6b0OC_kA,12898
 karnak3/core/log/__init__.py,sha256=fcpJ7rXdYAQxzF0x9LGeLaEMTtr2itMeW8tgiRvMz54,5155
 karnak3/core/log/legacy.py,sha256=EpvAed7ycl-gmjl9vC61JPuFzciBZa0R_1Rd2Y9PBuA,2310
 karnak3/core/store/__init__.py,sha256=VoPhR2ZO53H8nNxli3UFIeQFncJ6ZYFMVMsQQmpLiqg,4604
 karnak3/core/store/file.py,sha256=OgylCRxQIoHdQfXrzFoDSiEBTfYboESeKAMtB37pAHg,2770
 karnak3/core/util/__init__.py,sha256=ygoPFAurAe_p3zW5MeKb4hL7ZJCU_svVvO0lZRKCo60,1143
 karnak3/core/util/collections.py,sha256=agsxryST6lTuWU_IOM_YyS0uB6O8lQG2C1vjCkXU20o,1687
 karnak3/core/util/compression.py,sha256=MdaXPeQHn1P6rFfaZQLvO2z0JUR5xjdSqDuwcq7DURg,1062
@@ -43,12 +43,12 @@
 karnak3/fetch/sqs_fetcher.py,sha256=GNnTeh5vKnXv3MUogE_CSOWCBJdQof09ewyma79LVMI,16487
 test/integration/util/athena/run_athena_select.py,sha256=4JiG8F1iF6irBQhVF_itpEqAgfRc9_jhWlhT8o-A8WU,1099
 test/unit/karnak3/core/arg.py,sha256=XB58Y6jnGYjnZP17sE1i3ftY9MQhh7OdJb9p5kkTyzE,490
 test/unit/karnak3/core/test_log.py,sha256=tibA_RXtWCSSJ-M8KnH1L5pOBUfVMDgp8NNo4QqCBeg,1593
 test/unit/karnak3/core/test_time_window.py,sha256=a_lohoUx9kI9YmsWOgaXZGzVTMQLtPr61oc5JU7poZM,8498
 test/unit/karnak3/core/util/test_datetime.py,sha256=g3zm9lP7EPrRxMimZ6ZaK0XLJq3exRkUzs4-e_uHpto,680
 test/unit/karnak3/core/util/test_path.py,sha256=FMWcRflis24jIMjkm0OdNBkdc0uanf5fJuNMXkP4DU8,622
-karnak-3.3.7.dist-info/LICENSE,sha256=4M2c90jCYvZC9PotaItvu3gvjJOx4i7Q27nU-xmcN3Q,1058
-karnak-3.3.7.dist-info/METADATA,sha256=76EJIugV5U-eDs_O7EgQk-7v6YFRgLLXKxPZRIbVQag,1771
-karnak-3.3.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-karnak-3.3.7.dist-info/top_level.txt,sha256=h0dMxkNxnWjYhhpe-J_0UUh38FGFb80r6KdXDXbKgbM,35
-karnak-3.3.7.dist-info/RECORD,,
+karnak-3.4.0.dist-info/LICENSE,sha256=4M2c90jCYvZC9PotaItvu3gvjJOx4i7Q27nU-xmcN3Q,1058
+karnak-3.4.0.dist-info/METADATA,sha256=eeAB_aifJhmf7_RAQxWUpuICBuaxzzrm4xkxdc0HMEM,1789
+karnak-3.4.0.dist-info/WHEEL,sha256=Xo9-1PvkuimrydujYJAjF7pCkriuXBpUPEjma1nZyJ0,92
+karnak-3.4.0.dist-info/top_level.txt,sha256=h0dMxkNxnWjYhhpe-J_0UUh38FGFb80r6KdXDXbKgbM,35
+karnak-3.4.0.dist-info/RECORD,,
```

