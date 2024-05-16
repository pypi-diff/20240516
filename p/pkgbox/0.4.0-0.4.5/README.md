# Comparing `tmp/pkgbox-0.4.0-py3-none-any.whl.zip` & `tmp/pkgbox-0.4.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 40916 bytes, number of entries: 22
+Zip file size: 41144 bytes, number of entries: 22
 -rw-r--r--  2.0 unx      192 b- defN 24-Feb-10 09:04 joolbox/__init__.py
 -rw-r--r--  2.0 unx      198 b- defN 22-Aug-19 09:13 joolbox/authtokens.py
 -rw-r--r--  2.0 unx     1393 b- defN 22-May-01 13:25 joolbox/blogger.py
 -rw-r--r--  2.0 unx    11568 b- defN 23-Mar-01 10:36 joolbox/charts.py
 -rw-r--r--  2.0 unx     5168 b- defN 22-Jun-27 21:40 joolbox/date_fn.py
 -rw-r--r--  2.0 unx    38024 b- defN 24-Feb-10 09:15 joolbox/fn.py
 -rw-r--r--  2.0 unx    11653 b- defN 24-Jan-02 07:38 joolbox/gd.py
 -rw-r--r--  2.0 unx     5503 b- defN 24-Jan-19 06:00 joolbox/gs.py
 -rw-r--r--  2.0 unx     1163 b- defN 24-Feb-10 10:52 joolbox/islack.py
 -rw-r--r--  2.0 unx     2416 b- defN 23-Mar-15 21:14 joolbox/num_fn.py
 -rw-r--r--  2.0 unx      133 b- defN 24-Feb-10 12:38 pkgbox/__init__.py
 -rw-r--r--  2.0 unx     1393 b- defN 22-May-01 13:25 pkgbox/blogger.py
 -rw-r--r--  2.0 unx    11568 b- defN 23-Mar-01 10:36 pkgbox/charts.py
 -rw-r--r--  2.0 unx     5168 b- defN 22-Jun-27 21:40 pkgbox/date_fn.py
--rw-r--r--  2.0 unx    38955 b- defN 24-Mar-02 07:44 pkgbox/fn.py
+-rw-r--r--  2.0 unx    39840 b- defN 24-Mar-20 13:07 pkgbox/fn.py
 -rw-r--r--  2.0 unx     1002 b- defN 24-Feb-10 12:09 pkgbox/islack.py
 -rw-r--r--  2.0 unx     2416 b- defN 23-Mar-15 21:14 pkgbox/num_fn.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-02 07:48 pkgbox-0.4.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      584 b- defN 24-Mar-02 07:48 pkgbox-0.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-02 07:48 pkgbox-0.4.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-Mar-02 07:48 pkgbox-0.4.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1625 b- defN 24-Mar-02 07:48 pkgbox-0.4.0.dist-info/RECORD
-22 files, 140221 bytes uncompressed, 38358 bytes compressed:  72.6%
+-rw-r--r--  2.0 unx        0 b- defN 24-Mar-20 13:09 pkgbox-0.4.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx      558 b- defN 24-Mar-20 13:09 pkgbox-0.4.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Mar-20 13:09 pkgbox-0.4.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-Mar-20 13:09 pkgbox-0.4.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1625 b- defN 24-Mar-20 13:09 pkgbox-0.4.5.dist-info/RECORD
+22 files, 141080 bytes uncompressed, 38586 bytes compressed:  72.6%
```

## zipnote {}

```diff
@@ -45,23 +45,23 @@
 
 Filename: pkgbox/islack.py
 Comment: 
 
 Filename: pkgbox/num_fn.py
 Comment: 
 
-Filename: pkgbox-0.4.0.dist-info/LICENSE
+Filename: pkgbox-0.4.5.dist-info/LICENSE
 Comment: 
 
-Filename: pkgbox-0.4.0.dist-info/METADATA
+Filename: pkgbox-0.4.5.dist-info/METADATA
 Comment: 
 
-Filename: pkgbox-0.4.0.dist-info/WHEEL
+Filename: pkgbox-0.4.5.dist-info/WHEEL
 Comment: 
 
-Filename: pkgbox-0.4.0.dist-info/top_level.txt
+Filename: pkgbox-0.4.5.dist-info/top_level.txt
 Comment: 
 
-Filename: pkgbox-0.4.0.dist-info/RECORD
+Filename: pkgbox-0.4.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pkgbox/fn.py

```diff
@@ -30,24 +30,24 @@
         from datetime import datetime
         from datetime import timedelta
         from pytz import timezone
         import time
         pd.set_option('display.max_columns', None)
         pd.set_option('display.max_rows', None)
         pd.set_option('display.float_format', lambda x: '%.5f' % x)
-        from sklearn.cluster import KMeans
-        from scipy.stats import zscore
+        # from sklearn.cluster import KMeans
+        # from scipy.stats import zscore
         from numpy import asarray
-        from sklearn.preprocessing import MinMaxScaler
+        # from sklearn.preprocessing import MinMaxScaler
         # from IPython.display import display
         import os, sys
         import json
         from typing import Callable
         from functools import partial
-        from scipy.stats import linregress
+        # from scipy.stats import linregress
         import math
         import matplotlib.ticker as mtick
         import papermill as pm
         import shutil
         import requests
         from tabulate import tabulate
         from babel.numbers import format_currency
@@ -187,14 +187,38 @@
     
     return duplicate_rows
 
 # Example usage:
 # Assuming you have a DataFrame 'your_dataframe' and a list of columns 'your_columns'
 # duplicate_rows = find_duplicate_rows(your_dataframe, your_columns)
 # print(duplicate_rows)
+def ensure_dict(param):
+    """Ensure the parameter is a dictionary.
+
+    Args:
+        param: The input parameter to check and possibly convert to a dictionary.
+
+    Returns:
+        dict: The original dictionary, a converted dictionary from a string,
+              or an empty dictionary if conversion fails or if the input is not a dictionary or string.
+    """
+    if isinstance(param, dict):
+        # The parameter is already a dictionary
+        return param
+    elif isinstance(param, str):
+        # The parameter is a string, attempt to convert it to a dictionary
+        try:
+            return json.loads(param)
+        except json.JSONDecodeError:
+            # Return an empty dictionary if conversion fails
+            return {}
+    else:
+        # Return an empty dictionary if the parameter is neither a dictionary nor a string
+        return {}
+
 
 def pbx(string, op_name=None, params={}, channel_id=None) -> str:
     if op_name is None:
         notebook = "paper_run.ipynb"
         output_notebook = "paper_run_out.ipynb"
     else:
         notebook = f"{op_name}.ipynb"
@@ -209,15 +233,15 @@
                 if k.startswith('#raw_'):
                     x = f'''-r {k.replace('#raw_', '')} "{v}"'''
                 else:
                     x = f'''-p {k} "{v}"'''
                 yield x
         return " ".join(list(ml(dic)))
 
-    params = dicToparam(params)
+    params = dicToparam(ensure_dict(params))
 
     if output_notebook is None:
         command = f'''papermill "{notebook}" "{notebook}" {params}'''
     else:
         command = f'''papermill "{notebook}" "{output_notebook}" {params}'''
 
     os.system(command.strip())
```

## Comparing `pkgbox-0.4.0.dist-info/METADATA` & `pkgbox-0.4.5.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: pkgbox
-Version: 0.4.0
+Version: 0.4.5
 Summary: Frequently Used Packages for Analytics
 Author: alex
 Author-email: alex.mathew2k@gmail.com
 Keywords: pip,pkgbox
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: matplotlib
 Requires-Dist: seaborn
-Requires-Dist: sklearn (==0.0)
-Requires-Dist: scipy
+Requires-Dist: scikit-learn
 Requires-Dist: typing
-Requires-Dist: openpyxl (==3.1.2)
+Requires-Dist: openpyxl ==3.1.2
 Requires-Dist: papermill
 Requires-Dist: ipywidgets
 Requires-Dist: six
 Requires-Dist: tabulate
 Requires-Dist: oauth2client
 Requires-Dist: polars
 Requires-Dist: typing ; python_version < "3.5"
```

## Comparing `pkgbox-0.4.0.dist-info/RECORD` & `pkgbox-0.4.5.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 joolbox/gs.py,sha256=Byyw6RvoSmD7aMAHk8SlY5jvzBjXXfLAZTIWVEb3zA8,5503
 joolbox/islack.py,sha256=KolhZ6KwzwKKkUxjtcpSbrZzmXzBI_SqKNbLvSbiLRE,1163
 joolbox/num_fn.py,sha256=F842Ucn6ykDF8MyLW8ps8YnCFI6KYAQDigFfFqhu74g,2416
 pkgbox/__init__.py,sha256=cBTvmy_c5SwFAK9JAbypaGJCfyYQ0zj0HoI99T3FREo,133
 pkgbox/blogger.py,sha256=-XXA8xAGkuBjnlx7J1a2ASWvFZfWs3alhj_ITJFYvW0,1393
 pkgbox/charts.py,sha256=GFRaQIzRAvoSnnvicJds_k-suWmfqcdZr8hVk8hc06Q,11568
 pkgbox/date_fn.py,sha256=hRdkUBWCbxzXj1g2qytnkmyItB1u8LDJHuXmyhD0C44,5168
-pkgbox/fn.py,sha256=pOPSjwecpIU20RunMoOQh9HfJGa72xpeGgNWl2FgC-w,38955
+pkgbox/fn.py,sha256=DhQf_iUYd_xz3LZj9QwtXNCx8ECFhCQxRFPh7Q8XSWM,39840
 pkgbox/islack.py,sha256=SgKe0DmNLpcwwnZoEG9hf_VYewvTr8lJD_r3E9rn5yw,1002
 pkgbox/num_fn.py,sha256=F842Ucn6ykDF8MyLW8ps8YnCFI6KYAQDigFfFqhu74g,2416
-pkgbox-0.4.0.dist-info/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pkgbox-0.4.0.dist-info/METADATA,sha256=SzPxNoRySELOPVZ9kRnb2M7PLpeG06_CK4XeS3G3VKU,584
-pkgbox-0.4.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pkgbox-0.4.0.dist-info/top_level.txt,sha256=Yv9bzumcjJ3AFO1tpLOy8R70aKiKHpDEeFs-GuffKMQ,7
-pkgbox-0.4.0.dist-info/RECORD,,
+pkgbox-0.4.5.dist-info/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+pkgbox-0.4.5.dist-info/METADATA,sha256=eDhAU7ZMXd3oIcYrzaY7bkZA-P6H-BP-WSIIcBs2PpU,558
+pkgbox-0.4.5.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+pkgbox-0.4.5.dist-info/top_level.txt,sha256=Yv9bzumcjJ3AFO1tpLOy8R70aKiKHpDEeFs-GuffKMQ,7
+pkgbox-0.4.5.dist-info/RECORD,,
```

