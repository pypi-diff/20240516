# Comparing `tmp/gnssanalysis-0.0.9.tar.gz` & `tmp/gnssanalysis-0.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gnssanalysis-0.0.9.tar", last modified: Tue Oct 11 19:32:15 2022, max compression
+gzip compressed data, was "gnssanalysis-0.54.tar", last modified: Thu May 16 21:32:43 2024, max compression
```

## Comparing `gnssanalysis-0.0.9.tar` & `gnssanalysis-0.54.tar`

### file list

```diff
@@ -1,41 +1,53 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-11 19:32:15.000000 gnssanalysis-0.0.9/
--rw-r--r--   0 root         (0) root         (0)      244 2022-10-11 19:32:15.000000 gnssanalysis-0.0.9/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-11 19:32:15.000000 gnssanalysis-0.0.9/gnssanalysis/
--rw-rw-rw-   0 root         (0) root         (0)      146 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6300 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/create_erp_file.py
--rw-rw-rw-   0 root         (0) root         (0)     8315 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_aux.py
--rw-rw-rw-   0 root         (0) root         (0)     8211 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_combi.py
--rw-rw-rw-   0 root         (0) root         (0)     3980 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_const.py
--rw-rw-rw-   0 root         (0) root         (0)     9526 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_datetime.py
--rw-rw-rw-   0 root         (0) root         (0)    23938 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_diffaux.py
--rw-rw-rw-   0 root         (0) root         (0)    26839 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_download.py
--rw-rw-rw-   0 root         (0) root         (0)     8403 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_frame.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-11 19:32:15.000000 gnssanalysis-0.0.9/gnssanalysis/gn_io/
--rw-rw-rw-   0 root         (0) root         (0)      382 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17825 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_io/aux_dicts.py
--rw-rw-rw-   0 root         (0) root         (0)     5228 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_io/clk.py
--rw-rw-rw-   0 root         (0) root         (0)     2469 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_io/common.py
--rw-rw-rw-   0 root         (0) root         (0)     1595 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_io/discon.py
--rw-rw-rw-   0 root         (0) root         (0)    21394 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_io/igslog.py
--rw-rw-rw-   0 root         (0) root         (0)     2835 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_io/ionex.py
--rw-rw-rw-   0 root         (0) root         (0)      753 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_io/pea.py
--rw-rw-rw-   0 root         (0) root         (0)     1030 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_io/pod.py
--rw-rw-rw-   0 root         (0) root         (0)      707 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_io/psd.py
--rw-rw-rw-   0 root         (0) root         (0)     3394 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_io/rinex.py
--rw-rw-rw-   0 root         (0) root         (0)    19228 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_io/sinex.py
--rw-rw-rw-   0 root         (0) root         (0)    13602 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_io/sp3.py
--rw-rw-rw-   0 root         (0) root         (0)      700 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_io/stec.py
--rw-rw-rw-   0 root         (0) root         (0)     8553 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_io/trace.py
--rw-rw-rw-   0 root         (0) root         (0)     1889 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_io/trop.py
--rw-rw-rw-   0 root         (0) root         (0)     5895 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_plot.py
--rw-rw-rw-   0 root         (0) root         (0)     8557 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_transform.py
--rw-rw-rw-   0 root         (0) root         (0)    12710 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/gnssanalysis/gn_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-11 19:32:15.000000 gnssanalysis-0.0.9/gnssanalysis.egg-info/
--rw-r--r--   0 root         (0) root         (0)      244 2022-10-11 19:32:15.000000 gnssanalysis-0.0.9/gnssanalysis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      988 2022-10-11 19:32:15.000000 gnssanalysis-0.0.9/gnssanalysis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-11 19:32:15.000000 gnssanalysis-0.0.9/gnssanalysis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      229 2022-10-11 19:32:15.000000 gnssanalysis-0.0.9/gnssanalysis.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       88 2022-10-11 19:32:15.000000 gnssanalysis-0.0.9/gnssanalysis.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2022-10-11 19:32:15.000000 gnssanalysis-0.0.9/gnssanalysis.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-10-11 19:32:15.000000 gnssanalysis-0.0.9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      872 2022-10-11 19:31:58.000000 gnssanalysis-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:32:43.551659 gnssanalysis-0.54/
+-rw-r--r--   0 runner    (1001) docker     (127)    10173 2024-05-16 21:32:36.000000 gnssanalysis-0.54/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8081 2024-05-16 21:32:43.547659 gnssanalysis-0.54/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7523 2024-05-16 21:32:36.000000 gnssanalysis-0.54/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:32:43.543659 gnssanalysis-0.54/gnssanalysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-16 21:32:36.000000 gnssanalysis-0.54/gnssanalysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23680 2024-05-16 21:32:36.000000 gnssanalysis-0.54/gnssanalysis/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33920 2024-05-16 21:32:36.000000 gnssanalysis-0.54/gnssanalysis/filenames.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16174 2024-05-16 21:32:36.000000 gnssanalysis-0.54/gnssanalysis/gn_aux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9733 2024-05-16 21:32:36.000000 gnssanalysis-0.54/gnssanalysis/gn_combi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-05-16 21:32:36.000000 gnssanalysis-0.54/gnssanalysis/gn_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14302 2024-05-16 21:32:36.000000 gnssanalysis-0.54/gnssanalysis/gn_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29073 2024-05-16 21:32:36.000000 gnssanalysis-0.54/gnssanalysis/gn_diffaux.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35375 2024-05-16 21:32:36.000000 gnssanalysis-0.54/gnssanalysis/gn_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8610 2024-05-16 21:32:36.000000 gnssanalysis-0.54/gnssanalysis/gn_frame.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:32:43.547659 gnssanalysis-0.54/gnssanalysis/gn_io/
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-16 21:32:36.000000 gnssanalysis-0.54/gnssanalysis/gn_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21394 2024-05-16 21:32:36.000000 gnssanalysis-0.54/gnssanalysis/gn_io/aux_dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6181 2024-05-16 21:32:36.000000 gnssanalysis-0.54/gnssanalysis/gn_io/bia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-16 21:32:36.000000 gnssanalysis-0.54/gnssanalysis/gn_io/blq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-05-16 21:32:36.000000 gnssanalysis-0.54/gnssanalysis/gn_io/clk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-05-16 21:32:36.000000 gnssanalysis-0.54/gnssanalysis/gn_io/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-16 21:32:36.000000 gnssanalysis-0.54/gnssanalysis/gn_io/discon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25260 2024-05-16 21:32:36.000000 gnssanalysis-0.54/gnssanalysis/gn_io/erp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21560 2024-05-16 21:32:36.000000 gnssanalysis-0.54/gnssanalysis/gn_io/igslog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-16 21:32:36.000000 gnssanalysis-0.54/gnssanalysis/gn_io/ionex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6536 2024-05-16 21:32:36.000000 gnssanalysis-0.54/gnssanalysis/gn_io/nanu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-16 21:32:36.000000 gnssanalysis-0.54/gnssanalysis/gn_io/pea.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-16 21:32:36.000000 gnssanalysis-0.54/gnssanalysis/gn_io/pod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-16 21:32:36.000000 gnssanalysis-0.54/gnssanalysis/gn_io/psd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-05-16 21:32:36.000000 gnssanalysis-0.54/gnssanalysis/gn_io/rinex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44653 2024-05-16 21:32:36.000000 gnssanalysis-0.54/gnssanalysis/gn_io/sinex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22964 2024-05-16 21:32:36.000000 gnssanalysis-0.54/gnssanalysis/gn_io/sp3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-16 21:32:36.000000 gnssanalysis-0.54/gnssanalysis/gn_io/stec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9118 2024-05-16 21:32:36.000000 gnssanalysis-0.54/gnssanalysis/gn_io/trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-16 21:32:36.000000 gnssanalysis-0.54/gnssanalysis/gn_io/trop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-05-16 21:32:36.000000 gnssanalysis-0.54/gnssanalysis/gn_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17816 2024-05-16 21:32:36.000000 gnssanalysis-0.54/gnssanalysis/gn_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24875 2024-05-16 21:32:36.000000 gnssanalysis-0.54/gnssanalysis/gn_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 21:32:36.000000 gnssanalysis-0.54/gnssanalysis/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:32:43.547659 gnssanalysis-0.54/gnssanalysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8081 2024-05-16 21:32:43.000000 gnssanalysis-0.54/gnssanalysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-16 21:32:43.000000 gnssanalysis-0.54/gnssanalysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 21:32:43.000000 gnssanalysis-0.54/gnssanalysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-16 21:32:43.000000 gnssanalysis-0.54/gnssanalysis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-16 21:32:43.000000 gnssanalysis-0.54/gnssanalysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 21:32:43.000000 gnssanalysis-0.54/gnssanalysis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-16 21:32:43.551659 gnssanalysis-0.54/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-16 21:32:41.000000 gnssanalysis-0.54/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:32:43.547659 gnssanalysis-0.54/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-16 21:32:36.000000 gnssanalysis-0.54/tests/test_aux.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-16 21:32:36.000000 gnssanalysis-0.54/tests/test_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6205 2024-05-16 21:32:36.000000 gnssanalysis-0.54/tests/test_transform.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `gnssanalysis-0.0.9/gnssanalysis/gn_combi.py` & `gnssanalysis-0.54/gnssanalysis/gn_combi.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,187 +1,207 @@
 import numpy as _np
 import pandas as _pd
 import logging as _logging
 
 # from .gn_io.sinex import _get_snx_matrix, _get_snx_vector, get_variance_factor
-from gnssanalysis import gn_io as _gn_io
-from gnssanalysis import gn_transform as _gn_transform
+from . import gn_io as _gn_io
+from . import gn_transform as _gn_transform
 
-def cova2neq(cova:_np.ndarray, variance_factor):
+
+def cova2neq(cova: _np.ndarray, variance_factor):
     """Function to convert COVA matrix to NEQ matrix as per Bernese ADDNEQ"""
     neqm = _np.linalg.inv(cova / variance_factor)
+    # TODO could move neq = neq_est - neq_apr # N_total - N_constr from get_neq to here
     # neqv = neqm @ (vec.EST.values - vec.APR.values)
     # return neqm, neqv
     return neqm
 
-def corr2cova(corr:_np.ndarray) -> _np.ndarray:
+
+def corr2cova(corr: _np.ndarray) -> _np.ndarray:
     """Converts sinex CORR matrix to COVA using the diagonal STD values"""
-    D = corr.diagonal() * corr.diagonal()[:,None]
-    _np.fill_diagonal(corr,1) # fill COVA diagonal with 1 so we only multiply with D to get COVA
+    D = corr.diagonal() * corr.diagonal()[:, None]
+    _np.fill_diagonal(corr, 1)  # fill COVA diagonal with 1 so we only multiply with D to get COVA
     return corr * D
 
 
 def get_neq(path_or_bytes):
     snx_bytes = _gn_io.common.path2bytes(path_or_bytes)
     # TODO read and parse sinex header
 
     neq = _gn_io.sinex._get_snx_matrix(path_or_bytes=snx_bytes, stypes=["NEQ"], verbose=False)
 
     vec = b""  # to silence the pylance
     if neq is not None:
         vec = _gn_io.sinex._get_snx_vector(
-            path_or_bytes=snx_bytes, stypes=["APR", "EST", "NEQ"], verbose=False,snx_format=None
+            path_or_bytes=snx_bytes, stypes=["APR", "EST", "NEQ"], verbose=False, format="wide"
         )
         # revisit this vec thing
         return neq[0][0], vec  # NEQ matrix and vector are present so just return
     # return N and N_vec if they exist, else -> magic
-    _logging.warning(
-        msg="No NEQ was found. Generating from COVA/CORR as not strict"
-    )
+    _logging.warning(msg="No NEQ was found. Generating from COVA/CORR as not strict")
 
     apr_est = _gn_io.sinex._get_snx_matrix(path_or_bytes=snx_bytes, stypes=["APR", "EST"], verbose=False)
 
     if apr_est is not None:
         matrices, stype_dict = apr_est
     else:
         raise ValueError
 
     variance_factor = _gn_io.sinex.get_variance_factor(path_or_bytes)
-    
+
     if variance_factor is None:
         variance_factor = 1
-        _logging.warning(
-            msg="No variance factor found. Considering it 1"
-        )
+        _logging.warning(msg="No variance factor found. Considering it 1")
 
-    a_e = _gn_io.sinex._get_snx_vector(path_or_bytes = snx_bytes, stypes=["EST", "APR"], verbose=False,snx_format=None)
+    a_e = _gn_io.sinex._get_snx_vector(path_or_bytes=snx_bytes, stypes=["EST", "APR"], verbose=False, format="wide")
     if a_e is None:
         raise ValueError
 
-    if not 'APR' in stype_dict.keys():
+    if not "APR" in stype_dict.keys():
         std = a_e.STD.values
         mat_apr = _np.identity(std.shape[0])
-        _np.fill_diagonal(mat_apr,std*std)
-        neq_apr = cova2neq(mat_apr,variance_factor)
+        _np.fill_diagonal(mat_apr, std * std)
+        neq_apr = cova2neq(mat_apr, variance_factor)
     else:
-        if stype_dict['APR'] == 'CORR':
-            neq_apr = cova2neq(corr2cova(matrices[list(stype_dict.keys()).index('APR')]),variance_factor=variance_factor)
-        elif stype_dict['APR'] == 'COVA': # K_constr
-            neq_apr = cova2neq(matrices[list(stype_dict.keys()).index('APR')],variance_factor=variance_factor)
-        elif stype_dict['APR'] == 'INFO': # N_constr
-            neq_apr = matrices[list(stype_dict.keys()).index('APR')]
+        if stype_dict["APR"] == "CORR":
+            neq_apr = cova2neq(
+                corr2cova(matrices[list(stype_dict.keys()).index("APR")]), variance_factor=variance_factor
+            )
+        elif stype_dict["APR"] == "COVA":  # K_constr
+            neq_apr = cova2neq(matrices[list(stype_dict.keys()).index("APR")], variance_factor=variance_factor)
+        elif stype_dict["APR"] == "INFO":  # N_constr
+            neq_apr = matrices[list(stype_dict.keys()).index("APR")]
         else:
             raise ValueError
 
-    if stype_dict['EST'] == 'CORR':
-        neq_est = cova2neq(corr2cova(matrices[list(stype_dict.keys()).index('EST')]),variance_factor=variance_factor)
-    elif stype_dict['EST'] == 'COVA': # K_xx
-        print('cova2neq')
-        neq_est = cova2neq(corr2cova(matrices[list(stype_dict.keys()).index('EST')]),variance_factor=variance_factor)
-    elif stype_dict['EST'] == 'INFO': # N_total
-        neq_est = matrices[list(stype_dict.keys()).index('EST')]
+    if stype_dict["EST"] == "CORR":
+        neq_est = cova2neq(corr2cova(matrices[list(stype_dict.keys()).index("EST")]), variance_factor=variance_factor)
+    elif stype_dict["EST"] == "COVA":  # K_xx
+        print("cova2neq")
+        neq_est = cova2neq(corr2cova(matrices[list(stype_dict.keys()).index("EST")]), variance_factor=variance_factor)
+    elif stype_dict["EST"] == "INFO":  # N_total
+        neq_est = matrices[list(stype_dict.keys()).index("EST")]
     else:
         raise ValueError
 
-    neq = neq_est - neq_apr # N_total - N_constr
+    neq = neq_est - neq_apr  # N_total - N_constr
 
-    neqv = neq @ (a_e.EST.values - a_e.APR.values) # (a.APR + _np.linalg.solve(a=neqm,b=neqv)) - a.EST # to check
-    a_e['NEQ'] = neqv
+    neqv = neq @ (a_e.EST.values - a_e.APR.values)  # (a.APR + _np.linalg.solve(a=neqm,b=neqv)) - a.EST # to check
+    a_e["NEQ"] = neqv
     return neq, a_e
 
+
 def neq_elim_dim(neq_mat: _np.ndarray, neq_vec: _np.ndarray, i: int):
     """Eliminates 'i' dimension in NEQ system"""
     elim_row = neq_mat[i][_np.newaxis]
     elim_col = neq_mat[:, i]
     elim_centr = elim_col[i]
-    neq_mat -= (
-        elim_row * (elim_col / elim_centr)[:, _np.newaxis]
-    )  # division done on 1dim vector first
+    neq_mat -= elim_row * (elim_col / elim_centr)[:, _np.newaxis]  # division done on 1dim vector first
     neq_vec -= elim_col * neq_vec[i] / elim_centr
 
 
 def prepare_neq(neq_m, vec_apr_neq, frame_of_day):
     """Eliminate the non-XYZ parameters from the NEQ system and align a priori XYZ values to the frame of choice if frame_of_day is given"""
     neq_mat = neq_m.copy()
     vec_apr_neq = vec_apr_neq.copy()
     neq_vec = vec_apr_neq.NEQ.values
     xyz_mask = _np.isin(vec_apr_neq.TYPE.values, ["STAX", "STAY", "STAZ"])
+    _logging.info(f"{xyz_mask.shape[0]} parameters present")
+
+    soln_nums = vec_apr_neq.SOLN[xyz_mask].unique()  # XYZ only
+    if soln_nums.shape[0] > 1:  # more than one solution present e.g. CODE snx -> select central
+        mid_soln = soln_nums[soln_nums.shape[0] // 2]
+        mid_soln_mask = vec_apr_neq.SOLN.values == mid_soln
+        _logging.info(f"selecting solution No {mid_soln}")
+        xyz_mask &= mid_soln_mask
+
     idx2elim = vec_apr_neq.index.values[~xyz_mask]
 
-    # neq_mat,neq_vec = neq, neq_vec
-    for i in range(
-        idx2elim.shape[0]
-    ):  # need to be positive and sorted from bigger to smaller
-        neq_elim_dim(neq_mat, neq_vec, idx2elim[i])
+    n_elim = idx2elim.shape[0]
+    if n_elim > 0:
+        _logging.info(f"eliminating {n_elim} parameters")
+        for i in range(n_elim):  # need to be positive and sorted from bigger to smaller
+            neq_elim_dim(neq_mat, neq_vec, idx2elim[i])
 
     neq_mat_elim = neq_mat[xyz_mask, :][:, xyz_mask]
     neq_vec_elim = neq_vec[xyz_mask]
     vec_apr_neq = vec_apr_neq[xyz_mask]
 
     aprioris = vec_apr_neq.APR
     index_combo = _pd.MultiIndex.from_arrays(
         [vec_apr_neq.CODE.values + "_" + vec_apr_neq.PT.values.astype(str), vec_apr_neq.TYPE]
     )
     aprioris.index = index_combo
+
     aprioris = aprioris.unstack(level=1)
     aprioris_missing_mask = aprioris.STAX.values == 0
     aprioris_vals_mask = ~aprioris_missing_mask
 
     if aprioris_missing_mask.sum() > 0:
         estimates = vec_apr_neq.EST
         estimates.index = index_combo
         aprioris[aprioris_missing_mask] += estimates.unstack(level=1).values[aprioris_missing_mask]
 
     if frame_of_day is not None:
         common = _np.intersect1d(aprioris[aprioris_vals_mask].index.values, frame_of_day.index.values)
-        hlm = _gn_transform.get_helmert7(pt1=frame_of_day.loc[common].iloc[:, :3].values, pt2=aprioris[aprioris_vals_mask].loc[common].values)  # could not work if the order of XYZ is changed to YXZ etc
+        hlm = _gn_transform.get_helmert7(
+            pt1=frame_of_day.loc[common].iloc[:, :3].values, pt2=aprioris[aprioris_vals_mask].loc[common].values
+        )  # could not work if the order of XYZ is changed to YXZ etc
         # copy over estimate values to 0-aprioris here and rotate them using the computed hlm coeff
-        new_aprioris = _pd.DataFrame(data = _gn_transform.transform7(xyz_in=aprioris.values, helmert_list=hlm[0][0] * -1),
-                                     index = aprioris.index, columns = aprioris.columns)
+        new_aprioris = _pd.DataFrame(
+            data=_gn_transform.transform7(xyz_in=aprioris.values, hlm_params=hlm[0] * -1),
+            index=aprioris.index,
+            columns=aprioris.columns,
+        )
     else:
-        new_aprioris = aprioris # we later use substr with a mask and fill_value 0 to make all masked values 0
+        new_aprioris = aprioris  # we later use substr with a mask and fill_value 0 to make all masked values 0
 
-    d_apr = new_aprioris.subtract(aprioris[aprioris_vals_mask],fill_value=0).stack()[index_combo].values  # the aprioris index is sorted, so need to align with original index
+    d_apr = (
+        new_aprioris.subtract(aprioris[aprioris_vals_mask], fill_value=0).stack()[index_combo].values
+    )  # the aprioris index is sorted, so need to align with original index
 
     neq_vec_elim -= neq_mat_elim @ d_apr
-    vec_apr_neq[["APR", "NEQ"]] = _np.vstack([new_aprioris.stack()[index_combo].values, neq_vec_elim]).T # index_combo is needed to preserve the order that may have been changed by stack()
+    vec_apr_neq[["APR", "NEQ"]] = _np.vstack(
+        [new_aprioris.stack()[index_combo].values, neq_vec_elim]
+    ).T  # index_combo is needed to preserve the order that may have been changed by stack()
     return neq_mat_elim, vec_apr_neq
 
 
 def insert_neq(master_neq, master_vec_neq, ind, neq, neq_vec):
-
     bool_arr = _np.zeros(shape=master_neq.shape[0], dtype=bool)
     bool_arr[ind] = 1
     mask = bool_arr[_np.newaxis] * bool_arr[:, _np.newaxis]
     master_neq[mask] += neq.flatten()  # check the flatten order. Could change to +=1
-    master_vec_neq[
-        bool_arr
-    ] += neq_vec  # Could chage to +=1 for number of solutions plot
+    master_vec_neq[bool_arr] += neq_vec  # Could chage to +=1 for number of solutions plot
 
 
 def vec2comboind(vec):
     return vec.CODE.values + vec.PT.values + vec.TYPE.values.astype(str)
 
 
 def get_uniind(vec_list):
     buf = []
     for vec in vec_list:
-        buf.append(
-            vec.set_index(
-                vec.CODE.values + vec.PT.values.astype(str) + vec.TYPE.values.astype(str)
-            ).APR
-        )
-    combo_uni = (
-        _pd.concat(buf, axis=1).groupby(level=0, axis=1).mean()
-    )  # need to specify level to stay in df
+        buf.append(vec.set_index(vec.CODE.values + vec.PT.values.astype(str) + vec.TYPE.values.astype(str)).APR)
+    combo_uni = _pd.concat(buf, axis=1).groupby(level=0, axis=1).mean()  # need to specify level to stay in df
     combo_uni["IND"] = _np.arange(combo_uni.shape[0])  # for further stacking
     return combo_uni, buf
 
 
 def addneq(snx_filelist, frame_of_day):
+    """
+    This is the main combination function - extracts normal equation matrix+vector or converts available COVA/CORR to normal eq. counterparts. Only STAX/Y/Z values are being combined, hence rest must be eliminated before combining. All the solution values are first aligned to the ITRF/IGS frame to get close a priori values as required.
+    Care is needed with MIT, mig* specifically, and SIO solution files as available matrices are frequently singular. Singular matrices require additional treatment before inversion which has not been implemented yet.
+    Usage examples:
+    1. daily combination. Note than frame_of_day here is of midday of the day being processed:
+        daily_comb_neq = addneq(snx_filelist=_glob.glob('/data/cddis/2160/[!sio][!mig]*0.snx.Z'),frame_of_day=frame_of_day)
+    2. Weekly combination with frame_of_day centered at week's center:
+        weekly_comb_neq = addneq(snx_filelist=_glob.glob('/data/cddis/2160/[!sio][!mig]*.snx.Z'),frame_of_day=frame_of_day)
+
+    """
     buf_neq, buf_vec = [], []
     for file in snx_filelist:
         neq, vec = get_neq(file)
         neq, vec = prepare_neq(neq, vec, frame_of_day)
         buf_neq.append(neq)
         buf_vec.append(vec)
```

### Comparing `gnssanalysis-0.0.9/gnssanalysis/gn_const.py` & `gnssanalysis-0.54/gnssanalysis/gn_const.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,82 +1,69 @@
 """Constants to be declared here"""
 import numpy as _np
-from pandas import CategoricalDtype as _CategoricalDtype, DataFrame as _DataFrame
+import pandas as _pd
 
 MJD_ORIGIN = _np.datetime64("1858-11-17 00:00:00")
 GPS_ORIGIN = _np.datetime64("1980-01-06 00:00:00")
 J2000_ORIGIN = _np.datetime64("2000-01-01 12:00:00")
 
-SEC_IN_WEEK  = 604800
-SEC_IN_DAY   = 86400
-SEC_IN_YEAR  = 31557600
+SEC_IN_MINUTE = 60
+SEC_IN_HOUR = 60 * SEC_IN_MINUTE
+# SEC_IN_HOUR = 3600
+SEC_IN_12_HOURS = 12 * SEC_IN_HOUR
+# SEC_IN_12_HOURS = 43200
+SEC_IN_DAY = 24 * SEC_IN_HOUR
+# SEC_IN_DAY = 86400
+SEC_IN_WEEK = 7 * SEC_IN_DAY
+# SEC_IN_WEEK = 604800
+# YEAR is ambiguous, below is 365.25 * SEC_IN_DAY
+SEC_IN_YEAR = 31557600
 
-C_LIGHT = 299792458.0     # speed of light (m/s)
-OMEGA_E = 7.2921151467E-5 # rad/sec WGS84 value of earth's rotation rate
+C_LIGHT = 299792458.0  # speed of light (m/s)
+OMEGA_E = 7.2921151467e-5  # rad/sec WGS84 value of earth's rotation rate
 
 # https://www.iers.org/SharedDocs/Publikationen/EN/IERS/Documents/ac/sinex/sinex_v201_appendix1_pdf.pdf
-TYPE_CATEGORY = object # tmp fix to get rid of Categorical in the future
-# TYPE_CATEGORY       = _CategoricalDtype(categories = [
-#         'STAX','STAY','STAZ','VELX','VELY','VELZ','XGC','YGC','ZGC','RS_RA','RS_DE','RS_RAR',
-#         'RS_DER','RS_PL','LOD','UT','XPO','YPO','XPOR','YPOR','NUT_LN','NUT_OB','NUTRLN','NUTROB',
-#         'SAT__X','SAT__Y','SAT__Z','SAT_VX','SAT_VY','SAT_VZ','SAT_RP','SAT_GX','SAT_GZ','SATYBI',
-#         'TROTOT','TRODRY','TROWET','TGNTOT','TGNWET','TGNDRY','TGETOT','TGEWET','TGEDRY','RBIAS',
-#         'TBIAS','SBIAS','ZBIAS','AXI_OF','SATA_Z','SATA_X','SATA_Y',
-#         'ALOG_E','TLOG_E','ALOG_N','TLOG_N','ALOG_H','TLOG_H',
-#         'AEXP_E','TEXP_E','AEXP_N','TEXP_N','AEXP_H','TEXP_H'])
 
-TECHNIQUE_CATEGORY = _CategoricalDtype(categories=["C", "D", "L", "M", "P", "R"])
+TECHNIQUE_CATEGORY = _pd.CategoricalDtype(categories=["C", "D", "L", "M", "P", "R"])
 
-UNIT_CATEGORY = _CategoricalDtype(
+UNIT_CATEGORY = _pd.CategoricalDtype(
     categories=["m", "m/y", "m/s2", "ppb", "ms", "msd2", "mas", "ma/d", "rad", "rd/y", "rd/d"]
 )
 
-PT_CATEGORY = _CategoricalDtype(categories=list("ABCDEFGHIJKLMNOPQRSTUVWXYZ"))
+PT_CATEGORY = _pd.CategoricalDtype(categories=list("ABCDEFGHIJKLMNOPQRSTUVWXYZ"))
 
 GNSS = _np.asarray(["G", "E", "R", "C", "J"], dtype=object)
 
-PRN_CATEGORY = _CategoricalDtype(
+PRN_CATEGORY = _pd.CategoricalDtype(
     categories=(
-        GNSS
-        + _np.asarray(list("0123456789"))[:, None]
-        + _np.asarray(list("0123456789"))[:, None, None]
-    ).flatten(order="F") # generating a list of SVs for each constellation N01:N99
+        GNSS + _np.asarray(list("0123456789"))[:, None] + _np.asarray(list("0123456789"))[:, None, None]
+    ).flatten(
+        order="F"
+    )  # generating a list of SVs for each constellation N01:N99
 )
 
-CLK_TYPE_CATEGORY = _CategoricalDtype(categories=["CR", "DR", "AR", "AS", "MS"])
+CLK_TYPE_CATEGORY = _pd.CategoricalDtype(categories=["CR", "DR", "AR", "AS", "MS"])
 
-STATE_TYPES_CATEGORY = _CategoricalDtype(
-    categories=[
-        "PHASE_BIAS",
-        "REC_POS",
-        "REC_CLOCK",
-        "REC_SYS_BIAS",
-        "TROP",
-        "TROP_GM",
-        "SAT_CLOCK",
-        "AMBIGUITY",
-        "EOP",
-        "EOP_RATE",
-        "DCB",
-        "IONOSPHERIC",
-    ]
-)  # 'ONE' removed
 
 # GeodePy
 class Ellipsoid:
-    __doc__ = 'ellipsoid class doc placeholder'
+    __doc__ = "ellipsoid class doc placeholder"
+
     def __init__(self, semimaj, inversef):
-        self.semimaj    = float(semimaj) # a
-        self.semimajsq  = semimaj * semimaj # a**2
-        self.inversef   = inversef # inverse of the first flattening factor
-        self.flatten    = 1 / self.inversef # first flattening factor
-        self.semimin    = self.semimaj * (1 - self.flatten) # b
-        self.semiminsq  = self.semimin * self.semimin # b**2
-        self.ecc1sq     = self.flatten * (2 - self.flatten)
-        self.ecc2sq     = self.ecc1sq  / (1 - self.ecc1sq)
+        self.semimaj = float(semimaj)  # a
+        self.semimajsq = semimaj * semimaj  # a**2
+        self.inversef = inversef  # inverse of the first flattening factor
+        self.flatten = 1 / self.inversef  # first flattening factor
+        self.semimin = self.semimaj * (1 - self.flatten)  # b
+        self.semiminsq = self.semimin * self.semimin  # b**2
+        self.ecc1sq = self.flatten * (2 - self.flatten)
+        self.ecc1 = self.ecc1sq**0.5
+        self.ecc2sq = self.ecc1sq / (1 - self.ecc1sq)
+
+
 #         self.ecc1       = sqrt(self.ecc1sq)
 #         self.n          = float(self.f / (2 - self.f))
 #         self.n2         = self.n ** 2
 #         self.meanradius = (2 * self.semimaj + self.semimin)/3
 
 # Geodetic Reference System 1980
 # www.epsg-registry.org/export.htm?gml=urn:ogc:def:ellipsoid:EPSG::7019
@@ -90,11 +77,25 @@
 # www.epsg-registry.org/export.htm?gml=urn:ogc:def:ellipsoid:EPSG::7003
 ANS = Ellipsoid(6378160, 298.25)
 
 # International (Hayford) 1924
 # www.epsg-registry.org/export.htm?gml=urn:ogc:def:ellipsoid:EPSG::7022
 INTL24 = Ellipsoid(6378388, 297)
 
-SISRE_COEF_DF = _DataFrame(     data = [[0.99,	0.98,	0.98,	0.98,	0.98],
-                                        [127,	54,	49,	45,	61  ]],
-                                columns=['C_IGSO','C','G','R','E'],
-                                index = ['alpha','beta'])
+SISRE_COEF_DF = _pd.DataFrame(
+    data=[[0.99, 0.98, 0.98, 0.98, 0.98], [127, 54, 49, 45, 61]],
+    columns=["C_IGSO", "C", "G", "R", "E"],
+    index=["alpha", "beta"],
+)
+
+
+GNSS_IF_BIAS_C = _pd.DataFrame(
+    [
+        [1.00000000e00, 1.57542000e03, 2.54572778e00],
+        [2.00000000e00, 1.22760000e03, -1.54572778e00],
+        [1.00000000e00, 1.57542000e03, 2.93115808e00],
+        [2.00000000e00, 1.27875000e03, -1.93115808e00],
+    ],
+    columns=["PAIR_IDX", "F", "C"],
+    index=_pd.MultiIndex.from_tuples([("G", 1), ("G", 2), ("E", 1), ("E", 5)], names=["GNSS", "BAND"]),
+)
+# This table could be regenerated with get_gnss_IF_corr function in gn_io.bia. Same function could be extended to other GNSS/BANDS
```

### Comparing `gnssanalysis-0.0.9/gnssanalysis/gn_diffaux.py` & `gnssanalysis-0.54/gnssanalysis/gn_diffaux.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,318 +7,407 @@
 from . import gn_aux as _gn_aux
 from . import gn_const as _gn_const
 from . import gn_datetime as _gn_datetime
 from . import gn_io as _gn_io
 from . import gn_plot as _gn_plot
 
 
-def _valvar2diffstd(valvar1,valvar2,trace=True,std_coeff=1):
+def _valvar2diffstd(valvar1, valvar2, std_coeff=1):
     """Auxiliary function to efficiently difference two dataframes,
     each of them consisting of value-variance pairs"""
-    df = _pd.concat([valvar1,valvar2],axis=0,keys=['valvar1','valvar2']).unstack(0) #fastest\
-    df_nd = df.values
-    diff = df_nd[:,0] - df_nd[:,1]
-    nan_mask = ~_np.isnan(diff)
-
-    diff = diff[nan_mask]
-    std = std_coeff*_np.sqrt((df_nd[:,3] + df_nd[:,2])[nan_mask])
-    df_combo = _pd.DataFrame(_np.vstack([diff,std]).T,columns=['DIFF','STD'],index=df.index[nan_mask])
-
-    if trace:
-        sats = df.index.get_level_values('SAT')
-        sats_mask = ~sats.isna()
-        sats_df = sats[sats_mask].unique()
-        
-        df_combo.attrs['SAT_MASK'] = sats_mask[nan_mask]
-        sats_common = sats[sats_mask & nan_mask]#.unique()
-        df_combo.attrs['EXTRA_SATS'] = sats_df[~sats_df.isin(sats_common)].to_list() # is [] if none
+    df = _pd.concat([valvar1, valvar2], axis=0, keys=["valvar1", "valvar2"]).unstack(0)  # fastest\
+    df_nd = df.values.astype(float)
+    diff = df_nd[:, 0] - df_nd[:, 1]
+
+    std = std_coeff * _np.sqrt((df_nd[:, 3] + df_nd[:, 2]))
+    df_combo = _pd.DataFrame(_np.vstack([diff, std]).T, columns=["DIFF", "STD"], index=df.index)
     return df_combo
 
-def _diff2msg(diff, tol = None, dt_as_gpsweek=False):
+
+def _diff2msg(diff, tol=None, dt_as_gpsweek=False):
     _pd.set_option("display.max_colwidth", 10000)
-    from_valvar = _np.all(_np.isin(['DIFF','STD'],diff.columns.get_level_values(0).values))
+    from_valvar = _np.all(_np.isin(["DIFF", "STD"], diff.columns.get_level_values(0).values))
 
-    if from_valvar: #if from_valvar else diff.values
+    if from_valvar:  # if from_valvar else diff.values
         diff_df = diff.DIFF
-        std_df  = diff.STD
+        std_df = diff.STD
         std_vals = std_df.values if tol is None else tol
     else:
         diff_df = diff
         if tol is None:
             _logging.error(msg="tol can not be None if STD info is missing, skipping for now")
             return None
         std_vals = tol
 
     count_total = (~_np.isnan(diff_df.values)).sum(axis=0)
     mask2d_over_threshold = _np.abs(diff_df) > std_vals
 
     diff_count = mask2d_over_threshold.sum(axis=0)
-    
+
     mask = diff_count.astype(bool)
     if mask.sum() == 0:
         return None
     mask_some_vals = mask[mask.values].index
 
     diff_over = diff_df[mask2d_over_threshold][mask_some_vals]
     idx_max = diff_over.idxmax()
-    diff_max = _pd.Series(_np.diag(diff_over.loc[idx_max.values].values),index=idx_max.index)
+    diff_max = _pd.Series(_np.diag(diff_over.loc[idx_max.values].values), index=idx_max.index)
     idx_min = diff_over.idxmin()
-    diff_min = _pd.Series(_np.diag(diff_over.loc[idx_min.values].values),index=idx_min.index)
+    diff_min = _pd.Series(_np.diag(diff_over.loc[idx_min.values].values), index=idx_min.index)
 
     if from_valvar:
-        std_over  =  std_df[mask2d_over_threshold][mask_some_vals]
-        std_max = _pd.Series(_np.diag(std_over.loc[idx_max.values].values),index=idx_max.index)
-        std_min = _pd.Series(_np.diag(std_over.loc[idx_min.values].values),index=idx_min.index)
+        std_over = std_df[mask2d_over_threshold][mask_some_vals]
+        std_max = _pd.Series(_np.diag(std_over.loc[idx_max.values].values), index=idx_max.index)
+        std_min = _pd.Series(_np.diag(std_over.loc[idx_min.values].values), index=idx_min.index)
 
     msg = _pd.DataFrame()
-    msg['RATIO'] =  (diff_count[mask].astype(str).astype(object) + '/' + count_total[mask].astype(str) 
-    + ('(' + (diff_count[mask]/count_total[mask] * 100).round(2).astype(str)).str.ljust(5,fillchar='0') +'%)')
+    msg["RATIO"] = (
+        diff_count[mask].astype(str).astype(object)
+        + "/"
+        + count_total[mask].astype(str)
+        + ("(" + (diff_count[mask] / count_total[mask] * 100).round(2).astype(str)).str.ljust(5, fillchar="0")
+        + "%)"
+    )
+
+    msg["DIFF/MIN_DIFF"] = diff_min.round(4).astype(str) + (
+        "±" + std_min.round(4).astype(str).str.ljust(6, fillchar="0") if from_valvar else ""
+    )
+    if dt_as_gpsweek is not None:
+        datetime = (
+            (_gn_datetime.datetime2gpsweeksec(idx_min.values, as_decimal=True) + 1e-7).astype("<U11")
+            if dt_as_gpsweek
+            else _gn_datetime.j20002datetime(idx_min.values).astype(str)
+        )
+        msg["DIFF/MIN_DIFF"] += "@" + datetime.astype(object)
+
+    if (diff_count[mask] > 1).sum() > 0:
+        msg["MAX_DIFF"] = diff_max.round(4).astype(str).str.rjust(7) + (
+            "±" + std_max.round(4).astype(str).str.ljust(6, fillchar="0") if from_valvar else ""
+        )
+        if dt_as_gpsweek is not None:
+            datetime = (
+                (_gn_datetime.datetime2gpsweeksec(idx_max.values, as_decimal=True) + 1e-7).astype("<U11")
+                if dt_as_gpsweek
+                else _gn_datetime.j20002datetime(idx_max.values).astype(str)
+            )
+            msg["MAX_DIFF"] += "@" + datetime.astype(object)
+
+        msg["MEAN_DIFF"] = (
+            diff_over.mean(axis=0).round(4).astype(str)
+            + "±"
+            + diff_over.std(axis=0).round(4).astype(str).str.ljust(6, fillchar="0")
+        )
 
-    msg['DIFF/MIN_DIFF'] = (diff_min.round(4).astype(str)
-    +('±' + std_min.round(4).astype(str).str.ljust(6,fillchar='0') if from_valvar else '') 
-    +' @' + ( (_gn_datetime.datetime2gpsweeksec(idx_min.values,as_decimal=True)+1E-7).astype('<U11') if dt_as_gpsweek else _gn_datetime.j20002datetime(idx_min.values).astype(str)))
-
-    if (diff_count[mask]>1).sum()>0:
-        msg['MAX_DIFF'] = (diff_max.round(4).astype(str).str.rjust(7) 
-        +('±' + std_max.round(4).astype(str).str.ljust(6,fillchar='0') if from_valvar else '') 
-        +' @' + ( (_gn_datetime.datetime2gpsweeksec(idx_min.values,as_decimal=True)+1E-7).astype('<U11') if dt_as_gpsweek else _gn_datetime.j20002datetime(idx_min.values).astype(str))) * (diff_count[mask]>1)
-        
-        msg['MEAN_DIFF'] = (diff_over.mean(axis=0).round(4).astype(str)
-        +'±' + diff_over.std(axis=0).round(4).astype(str).str.ljust(6,fillchar='0'))* (diff_count[mask]>1)
+        msg.loc[diff_count[mask] <= 1, ["MAX_DIFF", "MEAN_DIFF"]] = ""
 
     return msg
 
 
-def _compare_sv_states(diffstd,log_lvl,tol=None,plot=False):
-    diff_sv = diffstd[diffstd.attrs['SAT_MASK']].droplevel('NUM',axis=0).unstack(['TYPE','SITE','SAT','BLK'])
-    if diff_sv.empty:
-        _logging.warning(msg=f':diffutil SVs states not present. Skipping')
+def _compare_states(diffstd: _pd.DataFrame, log_lvl: int, tol: _Union[float, None] = None, plot: bool = False) -> int:
+    """_summary_
+
+    Args:
+        diffstd (_pd.DataFrame): a difference DataFrame to assess
+        log_lvl (int): logging level of the produced messages
+        tol (_Union[float, None], optional): Either a float threshold or None to use the present STD values. Defaults to None.
+        plot (bool, optional): So you want a simple plot to terminal? Defaults to False.
+
+    Returns:
+        int: status (0 means differences within threshold)
+    """
+    diff_states = diffstd.unstack(["TYPE", "SITE", "SAT", "BLK", "NUM"])
+    # we remove the '.droplevel("NUM", axis=0)' due to ORBIT_PTS non-uniqueness. Changing to ORBIT_PTS_blah might be a better solution
+    if diff_states.empty:
+        _logging.warning(msg=f":diffutil states not present. Skipping")
         return 0
     if plot:
         # a standard scatter plot
-        _gn_plot.diff2plot(diff_sv.DIFF.PHASE_BIAS)
+        _gn_plot.diff2plot(diff_states.DIFF.PHASE_BIAS, kind=None, title="PHASE BIAS DIFF")
 
         # a bar plot of mean values
-        diffstd_mean = diff_sv.DIFF.PHASE_BIAS.mean(axis=0)
+        diffstd_mean = diff_states.DIFF.PHASE_BIAS.mean(axis=0)
         diffstd_mean.index = diffstd_mean.index.to_series().astype(str)
-        _gn_plot.diff2plot(diffstd_mean,kind='bar')
-    bad_sv_states = _diff2msg(diff_sv,tol)
-    if bad_sv_states is not None:
-        _logging.log(msg=f':diffutil found SV states diffs above {"the extracted STDs" if tol is None else f"{tol:.1E} tolerance"}:\n{bad_sv_states.to_string(justify="center")}\n',level=log_lvl)
-        return -1
-    _logging.log(msg=f':diffutil [OK] SVs states diffs within the {"extracted STDs" if tol is None else f"{tol:.1E} tolerance"}',level=_logging.INFO)
-    return 0
-    
-def _compare_nonsv_states(diffstd,log_lvl,tol=None):
-    diff_nonsv = diffstd[~diffstd.attrs['SAT_MASK']].droplevel('SAT',axis=0).unstack(['TYPE','SITE','NUM','BLK'])
-    if diff_nonsv.empty:
-        _logging.warning(msg=f':diffutil non-SVs states not present. Skipping')
-        return 0
-    bad_nonsv_states = _diff2msg(diff_nonsv,tol=tol)
-    if bad_nonsv_states is not None:
-        _logging.log(msg=f':diffutil non-SVs states diffs above {"the extracted STDs" if tol is None else f"{tol:.1E} tolerance"}:\n{bad_nonsv_states.to_string(justify="center")}\n',level=log_lvl)
+        _gn_plot.diff2plot(diffstd_mean, kind="bar", title="MEAN PHASE BIAS DIFF")
+    bad_states = _diff2msg(diff_states, tol)
+    if bad_states is not None:
+        _logging.log(
+            msg=f':diffutil found states diffs above {"the extracted STDs" if tol is None else f"{tol:.1E} tolerance"}:\n{bad_states.to_string(justify="center")}\n',
+            level=log_lvl,
+        )
         return -1
-    _logging.log(msg=f':diffutil [OK] non-SVs states diffs within the {"extracted STDs" if tol is None else f"{tol:.1E} tolerance"}',level=_logging.INFO)
+    _logging.log(
+        msg=f':diffutil [OK] states diffs within the {"extracted STDs" if tol is None else f"{tol:.1E} tolerance"}',
+        level=_logging.INFO,
+    )
     return 0
 
 
-def _compare_sat_postfit_residuals(diffstd, log_lvl, tol=None):
-    diff_count = diffstd[diffstd.attrs["SAT_MASK"]].unstack(["TYPE", "NUM", "SAT", "SITE", "BLK"])
-    if diff_count.empty:
-        _logging.warning(f':diffutil SVs residuals not present. Skipping')
-        return 0
-    bad_sv_residuals = _diff2msg(diff_count,tol=tol)
-    if bad_sv_residuals is not None:
-        _logging.log(msg=f':diffutil found SVs residuals diffs above {"the extracted STDs" if tol is None else f"{tol:.1E} tolerance"}:\n{bad_sv_residuals.to_string(justify="center")}\n',level=log_lvl)
-        return -1
-    _logging.log(msg=f':diffutil [OK] SVs residuals diffs within the {"extracted STDs" if tol is None else f"{tol:.1E} tolerance"}',level=_logging.INFO)
-    return 0
+def _compare_residuals(diffstd: _pd.DataFrame, log_lvl: int, tol: _Union[float, None] = None):
+    """Compares extracted POSTFIT residuals from the trace file and generates a comprehensive statistics on the present differences. Alternatively logs an OK message.
+
+    Args:
+        diffstd (_pd.DataFrame): a difference DataFrame to assess
+        log_lvl (int): logging level of the produced messages
+        tol (_Union[float, None], optional): Either a float threshold or None to use the present STD values. Defaults to None.
 
-def _compare_nonsat_postfit_residuals(diffstd,log_lvl,tol=None):
-    diff_count = diffstd[~diffstd.attrs['SAT_MASK']]
-    if diff_count.empty: #no non-sat records found such as Zamb
-        _logging.warning(f':diffutil non-SVs residuals not present. Skipping')
+    Returns:
+        int: status (0 means differences within threshold)
+    """
+    idx_names_to_unstack = list(diffstd.index.names)  # ['TIME', 'SITE', 'TYPE', 'SAT', 'NUM', 'It', 'BLK']
+    idx_names_to_unstack.remove("TIME")  # all but TIME: ['SITE', 'TYPE', 'SAT', 'NUM', 'It', 'BLK']
+    diff_residuals = diffstd.unstack(idx_names_to_unstack)
+    if diff_residuals.empty:
+        _logging.warning(f":diffutil residuals not present. Skipping")
         return 0
-    diff_count =  diff_count.droplevel('SAT').unstack(['TYPE','NUM','SITE','BLK'])
-    bad_nonsv_residuals = _diff2msg(diff_count,tol=tol)
-    if bad_nonsv_residuals is not None:
-        _logging.log(msg=f':diffutil found non-SVs residuals diffs above {"the extracted STDs" if tol is None else f"{tol:.1E} tolerance"}:\n{bad_nonsv_residuals.to_string(justify="center")}\n',level=log_lvl)
+    bad_residuals = _diff2msg(diff_residuals, tol=tol)
+    if bad_residuals is not None:
+        _logging.log(
+            msg=f':diffutil found residuals diffs above {"the extracted STDs" if tol is None else f"{tol:.1E} tolerance"}:\n{bad_residuals.to_string(justify="center")}\n',
+            level=log_lvl,
+        )
         return -1
-    _logging.log(msg=f':diffutil [OK] non-SVs residuals diffs within the {"extracted STDs" if tol is None else f"{tol:.1E} tolerance"}',level=_logging.INFO)
+    _logging.log(
+        msg=f':diffutil [OK] residuals diffs within the {"extracted STDs" if tol is None else f"{tol:.1E} tolerance"}',
+        level=_logging.INFO,
+    )
     return 0
 
-def _compare_stec(diffstd,log_lvl,tol=None):
-    stec_diff = diffstd.unstack(level = ('SITE','SAT','LAYER'))
+
+def _compare_stec(diffstd, log_lvl, tol=None):
+    stec_diff = diffstd.unstack(level=("SITE", "SAT", "LAYER"))
     if stec_diff.empty:
-        _logging.warning(f':diffutil stec states not present. Skipping')
+        _logging.warning(f":diffutil stec states not present. Skipping")
         return 0
-    bad_sv_states = _diff2msg(stec_diff,tol,dt_as_gpsweek=True)
+    bad_sv_states = _diff2msg(stec_diff, tol, dt_as_gpsweek=True)
     if bad_sv_states is not None:
-        _logging.log(msg=f':diffutil found stec states diffs above {"the extracted STDs" if tol is None else f"{tol:.1E} tolerance"}:\n{bad_sv_states.to_string(justify="center")}\n',level=log_lvl)
+        _logging.log(
+            msg=f':diffutil found stec states diffs above {"the extracted STDs" if tol is None else f"{tol:.1E} tolerance"}:\n{bad_sv_states.to_string(justify="center")}\n',
+            level=log_lvl,
+        )
         return -1
-    _logging.log(msg=f':diffutil [OK] stec states diffs within the {"extracted STDs" if tol is None else f"{tol:.1E} tolerance"}',level=_logging.INFO)
+    _logging.log(
+        msg=f':diffutil [OK] stec states diffs within the {"extracted STDs" if tol is None else f"{tol:.1E} tolerance"}',
+        level=_logging.INFO,
+    )
     return 0
 
-def difftrace(trace1_path,trace2_path,tol,std_coeff,log_lvl,plot):
-    '''Compares two trace/sum files'''
+
+def difftrace(trace1_path, trace2_path, tol, std_coeff, log_lvl, plot):
+    """Compares two trace/sum files
+    Only POSTFIT residuals are compared"""
     trace1 = _gn_io.common.path2bytes(trace1_path)
     trace2 = _gn_io.common.path2bytes(trace2_path)
 
-    _logging.info(msg=f':diffutil -----testing trace states-----')
-    states1 = _gn_io.trace._read_trace_states(trace1)
-    states2 = _gn_io.trace._read_trace_states(trace2)
+    _logging.info(msg=f":diffutil -----testing trace states-----")
+    states1 = _gn_io.trace._read_trace_states(trace1, throw_if_nans=True)
+    states2 = _gn_io.trace._read_trace_states(trace2, throw_if_nans=True)
+
     status = 0
     if (states1 is None) and (states2 is None):
-        _logging.log(msg=f':diffutil both compared files are missing states data -> OK',level=log_lvl)
+        _logging.log(msg=f":diffutil both compared files are missing states data -> OK", level=log_lvl)
     elif (states1 is None) or (states2 is None):
-        status += -1 # don't wait, throw error right away as smth bad happened, errors have been logged
+        status += -1  # don't wait, throw error right away as smth bad happened, errors have been logged
     else:
-        diffstd_states    = _valvar2diffstd(states1.iloc[:,:2],states2.iloc[:,:2],std_coeff=std_coeff,trace=True)
-        if diffstd_states.attrs['EXTRA_SATS'] != []:
-            _logging.warning(msg=f':diffutil found no counterpart for: {sorted(diffstd_states.attrs["EXTRA_SATS"])}')
-        status += _compare_sv_states(diffstd_states,tol=tol,log_lvl=log_lvl,plot=plot)
-        status += _compare_nonsv_states(diffstd_states,tol=tol,log_lvl=log_lvl)
-
-    _logging.info(msg=f':diffutil -----testing trace residuals-----')
-    resids1 = _gn_io.trace._read_trace_residuals(trace1)
-    resids2 = _gn_io.trace._read_trace_residuals(trace2)
+        _gn_aux.throw_if_index_duplicates(states1)
+        _gn_aux.throw_if_index_duplicates(states2)
+
+        diffstd_states = _valvar2diffstd(states1.iloc[:, :2], states2.iloc[:, :2], std_coeff=std_coeff)
+        sats = diffstd_states.index.get_level_values("SAT")
+        sats_with_nans = (
+            sats.notna() & diffstd_states.DIFF.isna().values
+        )  # if there are SVs with nans at this stage, this means that files' indices are different
+        if sats_with_nans.any():
+            _logging.error(msg=f":diffutil found no counterpart for:\n{diffstd_states.index[sats_with_nans]}")
+            status -= 1
+        else:
+            status += _compare_states(diffstd_states, tol=tol, log_lvl=log_lvl, plot=plot)
+
+    _logging.info(msg=f":diffutil -----testing trace residuals-----")
+    resids1 = _gn_io.trace._read_trace_residuals(trace1, throw_if_nans=True)
+    resids2 = _gn_io.trace._read_trace_residuals(trace2, throw_if_nans=True)
+
     if (resids1 is None) and (resids2 is None):
-        _logging.log(msg=f':diffutil both compared files are missing residuals data -> OK',level=log_lvl)
-    elif (resids1 is None) or (resids2 is None): 
-        status += -1 # don't wait, throw error right away as smth bad happened, errors have been logged
-    else:
-        diffstd_residuals = _valvar2diffstd(resids1.iloc[:,2:],resids2.iloc[:,2:],std_coeff=std_coeff,trace=True)
-        status += _compare_sat_postfit_residuals(diffstd_residuals,tol=tol,log_lvl=log_lvl)
-        status += _compare_nonsat_postfit_residuals(diffstd_residuals,tol=tol,log_lvl=log_lvl)
+        _logging.log(msg=f":diffutil both compared files are missing residuals data -> OK", level=log_lvl)
+    elif (resids1 is None) or (resids2 is None):
+        status += -1  # don't wait, throw error right away as smth bad happened, errors have been logged
+    else:
+        _gn_aux.throw_if_index_duplicates(resids1)
+        _gn_aux.throw_if_index_duplicates(resids2)
+        diffstd_residuals = _valvar2diffstd(
+            resids1[["POSTFIT", "STD"]], resids2[["POSTFIT", "STD"]], std_coeff=std_coeff
+        )
+        status += _compare_residuals(diffstd_residuals, tol=tol, log_lvl=log_lvl)
 
     return status
 
-def diffsnx(snx1_path,snx2_path,tol,std_coeff,log_lvl):
-    '''Compares two sinex files '''
-    snx1_df = _gn_io.sinex._get_snx_vector(path_or_bytes=snx1_path,stypes=('EST',),snx_format=True,verbose=True)
-    snx2_df = _gn_io.sinex._get_snx_vector(path_or_bytes=snx2_path,stypes=('EST',),snx_format=True,verbose=True)
 
-    if (snx1_df is None) or (snx2_df is None): return -1 # don't wait, throw error right away as smth bad happened, errors have been logged
+def diffsnx(snx1_path, snx2_path, tol, std_coeff, log_lvl):
+    """Compares two sinex files"""
+    snx1_df = _gn_io.sinex._get_snx_vector(path_or_bytes=snx1_path, stypes=("EST",), format="long", verbose=True)
+    snx2_df = _gn_io.sinex._get_snx_vector(path_or_bytes=snx2_path, stypes=("EST",), format="long", verbose=True)
+
+    if (snx1_df is None) or (snx2_df is None):
+        return -1  # don't wait, throw error right away as smth bad happened, errors have been logged
 
     status = 0
-    diff_snx = _valvar2diffstd(snx1_df,snx2_df,trace=False,std_coeff=std_coeff).unstack(['CODE_PT','TYPE'])
+    diff_snx = _valvar2diffstd(snx1_df, snx2_df, std_coeff=std_coeff).unstack(["CODE_PT", "TYPE"])
     assert diff_snx.size != 0, "no corresponding data to compare"
 
-    bad_snx_vals = _diff2msg(diff_snx,tol=tol)
+    bad_snx_vals = _diff2msg(diff_snx, tol=tol)
     if bad_snx_vals is not None:
-        _logging.log(msg=f':diffutil found estimates diffs above {"the extracted STDs" if tol is None else f"{tol:.1E} tolerance"}:\n{bad_snx_vals.to_string(justify="center")}\n',level=log_lvl)
+        _logging.log(
+            msg=f':diffutil found estimates diffs above {"the extracted STDs" if tol is None else f"{tol:.1E} tolerance"}:\n{bad_snx_vals.to_string(justify="center")}\n',
+            level=log_lvl,
+        )
         status = -1
     else:
-        _logging.log(msg=f':diffutil [OK] estimates diffs within {"the extracted STDs" if tol is None else f"{tol:.1E} tolerance"}',level=_logging.INFO)
+        _logging.log(
+            msg=f':diffutil [OK] estimates diffs within {"the extracted STDs" if tol is None else f"{tol:.1E} tolerance"}',
+            level=_logging.INFO,
+        )
     return status
 
-def diffstec(path1,path2,tol,std_coeff,log_lvl):
-    '''Compares two stec files '''
-    stec1,stec2 = _gn_io.stec.read_stec(path1), _gn_io.stec.read_stec(path2)
+
+def diffstec(path1, path2, tol, std_coeff, log_lvl):
+    """Compares two stec files"""
+    stec1, stec2 = _gn_io.stec.read_stec(path1), _gn_io.stec.read_stec(path2)
     status = 0
-    diffstd = _valvar2diffstd(stec1,stec2,std_coeff=std_coeff)
-    status = _compare_stec(diffstd=diffstd,tol=tol,log_lvl=log_lvl)
+    diffstd = _valvar2diffstd(stec1, stec2, std_coeff=std_coeff)
+    status = _compare_stec(diffstd=diffstd, tol=tol, log_lvl=log_lvl)
     return status
 
-def diffionex(ionex1_path,ionex2_path,tol,std_coeff,log_lvl):
-    '''Compares two ionex files '''
+
+def diffionex(ionex1_path, ionex2_path, tol, std_coeff, log_lvl):
+    """Compares two ionex files"""
 
     ionex1_df = _gn_io.ionex.read_ionex(path_or_bytes=ionex1_path)
     ionex2_df = _gn_io.ionex.read_ionex(path_or_bytes=ionex2_path)
 
-    tol = 10**min(ionex1_df.attrs['EXPONENT'],ionex2_df.attrs['EXPONENT'])*std_coeff if tol is None else tol
+    tol = 10 ** min(ionex1_df.attrs["EXPONENT"], ionex2_df.attrs["EXPONENT"]) * std_coeff if tol is None else tol
 
     status = 0
-    diff_ionex = (ionex1_df.unstack(level=('Type','Lat')) - ionex2_df.unstack(level=('Type','Lat'))).swaplevel('Lon','Type',axis=1) # type:ignore output looks cleaner this way
+    diff_ionex = (ionex1_df.unstack(level=("Type", "Lat")) - ionex2_df.unstack(level=("Type", "Lat"))).swaplevel(
+        "Lon", "Type", axis=1
+    )  # type:ignore output looks cleaner this way
 
-    bad_ionex_vals = _diff2msg(diff_ionex,tol=tol)
+    bad_ionex_vals = _diff2msg(diff_ionex, tol=tol)
     if bad_ionex_vals is not None:
-        _logging.log(msg=f':diffutil found IONEX diffs above {f"10^min(exp1,exp2)*std_coeff = {tol:.1E} tolerance" if tol is None else f"{tol:.1E} tolerance"}:\n{bad_ionex_vals.to_string(justify="center")}\n',level=log_lvl)
+        _logging.log(
+            msg=f':diffutil found IONEX diffs above {f"10^min(exp1,exp2)*std_coeff = {tol:.1E} tolerance" if tol is None else f"{tol:.1E} tolerance"}:\n{bad_ionex_vals.to_string(justify="center")}\n',
+            level=log_lvl,
+        )
         status = -1
     else:
-        _logging.log(msg=f':diffutil [OK] estimates diffs within {f"10^min(exp1,exp2) = {tol:.1E} tolerance" if tol is None else f"{tol:.1E} tolerance"}',level=_logging.INFO)
+        _logging.log(
+            msg=f':diffutil [OK] estimates diffs within {f"10^min(exp1,exp2) = {tol:.1E} tolerance" if tol is None else f"{tol:.1E} tolerance"}',
+            level=_logging.INFO,
+        )
     return status
 
-def _compare_clk(clk_a:_pd.DataFrame,clk_b:_pd.DataFrame,
-                 norm_type:str='both',
-                 ext_dt :_Union[_np.ndarray,_pd.Index,None]=None,
-                 ext_svs:_Union[_np.ndarray,_pd.Index,None]=None)->_pd.DataFrame:
-    """
-    clk DataFrames are the output of read_clk. sp3_a and sp3_b are the
-    DataFrames produced by read_sp3 function. Outputs a DataFrame of
-    signal-in-space range error (SISRE). The SISRE units are meters
+
+def compare_clk(
+    clk_a: _pd.DataFrame,
+    clk_b: _pd.DataFrame,
+    norm_types: list = ["daily", "epoch"],
+    ext_dt: _Union[_np.ndarray, _pd.Index, None] = None,
+    ext_svs: _Union[_np.ndarray, _pd.Index, None] = None,
+) -> _pd.DataFrame:
+    """Compares clock dataframes, removed common mode.
+
+    :param _pd.DataFrame clk_a: clk dataframe 1
+    :param _pd.DataFrame clk_b: clk dataframe 2
+    :param str norm_type: normalization to apply, defaults to "both"
+    :param _Union[_np.ndarray, _pd.Index, None] ext_dt: external datetime values to filter the clk dfs, defaults to None
+    :param _Union[_np.ndarray, _pd.Index, None] ext_svs: external satellites to filter the clk dfs, defaults to None
+    :raises ValueError: if no common epochs between clk_a and external datetime were found
+    :raises ValueError: if no common epochs between files were found
+    :return _pd.DataFrame: clk differences in the same units as input clk dfs (usually seconds)
     """
 
     clk_a = _gn_io.clk.get_AS_entries(clk_a)
     clk_b = _gn_io.clk.get_AS_entries(clk_b)
 
+    if not isinstance(norm_types, list):  # need list for 'sv' to be correctly converted to array of SVs to use for norm
+        norm_types = list(norm_types)
+
     if ext_dt is None:
         common_dt = clk_a.index.levels[0]
     else:
         common_dt = clk_a.index.levels[0].intersection(ext_dt)
-        if len(common_dt) == 0: raise ValueError("no common epochs between clk_a and external dt")
+        if len(common_dt) == 0:
+            raise ValueError("no common epochs between clk_a and external dt")
 
     common_dt = common_dt.intersection(clk_b.index.levels[0])
-    if len(common_dt) == 0:raise ValueError("no common epochs between clk_a and clk_b")
+    if len(common_dt) == 0:
+        raise ValueError("no common epochs between clk_a and clk_b")
 
     clk_a_unst = _gn_aux.rm_duplicates_df(clk_a.loc[common_dt]).unstack(1)
     clk_b_unst = _gn_aux.rm_duplicates_df(clk_b.loc[common_dt]).unstack(1)
 
-
     if ext_svs is None:
-        common_svs = clk_a_unst.columns # assuming ext_svs is lots smaller than count of svs in 
+        common_svs = clk_a_unst.columns  # assuming ext_svs is lots smaller than count of svs in
     else:
         common_svs = clk_a_unst.columns.intersection(ext_svs)
-    if not _gn_aux.array_equal_unordered(common_svs,clk_b_unst.columns.values):
+    if not _gn_aux.array_equal_unordered(common_svs, clk_b_unst.columns.values):
         common_svs = common_svs.intersection(clk_b_unst.columns)
         clk_a_unst = clk_a_unst[common_svs]
         clk_b_unst = clk_b_unst[common_svs]
     else:
-        _logging.debug('_compare_clk: skipping svs sync for clk_b_unst as the same as common_svs')
-        if not _gn_aux.array_equal_unordered(common_svs,clk_a_unst.columns.values):
-            _logging.debug('_compare_clk: syncing clk_a_unst with common_svs as not equal')
+        _logging.debug("compare_clk: skipping svs sync for clk_b_unst as the same as common_svs")
+        if not _gn_aux.array_equal_unordered(common_svs, clk_a_unst.columns.values):
+            _logging.debug("compare_clk: syncing clk_a_unst with common_svs as not equal")
             clk_a_unst = clk_a_unst[common_svs]
 
-
-    if norm_type == 'sv':
-        norm_type = _gn_io.clk.select_norm_svs_per_gnss(clk_a_unst=clk_a_unst,clk_b_unst=clk_b_unst)
-        #get the sv to use for norm and overwrite norm_type value with sv prn code
-    _gn_io.clk.rm_clk_bias(clk_a_unst,norm_type=norm_type)
-    _gn_io.clk.rm_clk_bias(clk_b_unst,norm_type=norm_type)
-
-    clk_diff = (clk_a_unst - clk_b_unst)*_gn_const.C_LIGHT
-    return clk_diff
-
-
-def sisre(sp3_a: _pd.DataFrame, sp3_b: _pd.DataFrame, 
-          clk_a: _Union[_pd.DataFrame, None] = None,
-          clk_b: _Union[_pd.DataFrame, None] = None,
-          norm_type: str = 'both', output_mode: str = 'rms',
-          clean: bool = True, cutoff: _Union[int, float, None] = None,
-          use_rms: bool = False,
-          hlm_mode=None,
-          plot=False):
+    if len(norm_types) != 0:
+        _logging.info(f":_clk_compare:using {norm_types} clk normalization")
+        if "sv" in norm_types:
+            norm_types[norm_types.index("sv")] = _gn_io.clk.select_norm_svs_per_gnss(
+                clk_a_unst=clk_a_unst, clk_b_unst=clk_b_unst
+            )
+
+            # get the sv to use for norm and overwrite norm_type value with sv prn code
+        _logging.info("---removing common mode from clk 1---")
+        _gn_io.clk.rm_clk_bias(clk_a_unst, norm_types=norm_types)
+        _logging.info("---removing common mode from clk 2---")
+        _gn_io.clk.rm_clk_bias(clk_b_unst, norm_types=norm_types)
+    return clk_a_unst - clk_b_unst
+
+
+def sisre(
+    sp3_a: _pd.DataFrame,
+    sp3_b: _pd.DataFrame,
+    clk_a: _Union[_pd.DataFrame, None] = None,
+    clk_b: _Union[_pd.DataFrame, None] = None,
+    norm_type: str = "both",
+    output_mode: str = "rms",
+    clean: bool = True,
+    cutoff: _Union[int, float, None] = None,
+    use_rms: bool = False,
+    hlm_mode=None,
+    plot=False,
+    write_rac_file=False,
+):
     """
     Computes SISRE metric for the combination of orbits and clock offsets. Note,
     if clock offsets were not provided computes orbit SISRE. Ignores clock
-    offset values which could available in the orbit files (sp3). 
-    TODO Add support for sp3 clock offset values, that could be overridden 
+    offset values which could available in the orbit files (sp3).
+    TODO Add support for sp3 clock offset values, that could be overridden
     TODO by proper clk input. Add a 'force' option to use sp3 clock offsets.
 
     Returns SISRE metric computed using the equation of Steigenberger &
     Montenbruck (2020) SISRE = sqrt( (w₁²R² - 2w₁RT + T²) + w₂²(A² + C²) )
-    according to  which is the same as sqrt((αR - cT)² + (A² + C²)/β), with 
+    according to  which is the same as sqrt((αR - cT)² + (A² + C²)/β), with
     w₁ = α and w₂ = sqrt(1/β).
     α and β are given in the table below:
         BDS(GEO/IGSO)   BDS(MEO)    GPS     GLO     GAL
     α   0.99            0.98        0.98    0.98    0.98
     β   127             54          49      45      61
     *QZSS (J) is being ignored
     *BeiDou different coeffs for MEO/GEO not implemented yet
-        
+
     Parameters
     ----------
     sp3_a : sp3 DataFrame a
         Output of read_sp3 function or a similar sp3 DataFrame.
     sp3_b : sp3 DataFrame b
         Output of read_sp3 function or a similar sp3 DataFrame.
     clk_a : clk DataFrame a (optinal)
@@ -341,122 +430,239 @@
         computing SISRE.
 
     Returns
     -------
     sisre : DataFrame or Series depending in the output_mode selection
         output_mode = 'rms'  : Series of RMS SISRE values, value per GNSS.
         output_mode = 'gnss' : DataFrame of epoch-wise RMS SISRE values per GNSS.
-        output_mode = 'sv'   : DataFrame of epoch-wise SISRE values per SV.
+        output_mode = 'sv'   : DataFrame of epoch-wise SISRE values per SV. NOTE: SV here refers to Satellite
+                               Vehicle ID (1-1 mappable to Pseudo-Random Noise identifier i.e. PRN). It does NOT
+                               refer to Satellite Vehicle Number (which is permanent).
     """
-    if output_mode not in ['rms', 'sv', 'gnss']:
-        raise ValueError('incorrect output_mode given: %s' % output_mode)
+    if output_mode not in ["rms", "sv", "gnss"]:
+        raise ValueError("incorrect output_mode given: %s" % output_mode)
+
+    rac = _gn_io.sp3.diff_sp3_rac(
+        _gn_aux.rm_duplicates_df(sp3_a, rm_nan_level=1),
+        _gn_aux.rm_duplicates_df(sp3_b, rm_nan_level=1),
+        hlm_mode=hlm_mode,
+    )
+
+    if write_rac_file:
+        rtn_filename = rac.attrs["sp3_a"] + " - " + rac.attrs["sp3_b"] + hlm_mode if hlm_mode is not None else ""
+        print(rtn_filename)
+        rac.to_csv(path_or_buf=rtn_filename, header=True, index=True)
 
-    rac = _gn_io.sp3.diff_sp3_rac(_gn_aux.rm_duplicates_df(sp3_a, rm_nan_level=1),
-                                 _gn_aux.rm_duplicates_df(sp3_b, rm_nan_level=1),
-                                 hlm_mode=hlm_mode)
-                                 
     rac_unstack = rac.EST_RAC.unstack() * 1000  # km to meters,
-                                 # sync is being done within the function. 
-                                 # Filters with std over XYZ separately and all satellites together
+    # sync is being done within the function.
+    # Filters with std over XYZ separately and all satellites together
     rac_unstack.attrs = rac.attrs
     if clean:
         if cutoff is not None:
             rac_unstack = rac_unstack[rac_unstack.abs() < cutoff]
-        rac_unstack = rac_unstack[rac_unstack.abs() < _gn_aux.get_std_bounds(
-            rac_unstack, axis=0, sigma_coeff=3)]
+        rac_unstack = rac_unstack[rac_unstack.abs() < _gn_aux.get_std_bounds(rac_unstack, axis=0, sigma_coeff=3)]
     if plot:
-        _logging.info(msg='plotting RAC difference')
+        _logging.info(msg="plotting RAC difference")
         _gn_plot.racplot(rac_unstack=rac_unstack, output=plot if isinstance(plot, str) else None)
 
     if (clk_a is not None) & (clk_b is not None):  # check if clk data is present
-        clk_diff = _compare_clk(clk_a, clk_b, norm_type=norm_type,
-                                ext_dt=rac_unstack.index, ext_svs=rac_unstack.columns.levels[1])  # units are meters
+        clk_diff = (
+            compare_clk(
+                clk_a, clk_b, norm_types=norm_type, ext_dt=rac_unstack.index, ext_svs=rac_unstack.columns.levels[1]
+            )
+            * _gn_const.C_LIGHT
+        )  # units are meters
         if clean:
             if cutoff is not None:
                 clk_diff = clk_diff[clk_diff.abs() < cutoff]
-            clk_diff = clk_diff[clk_diff.abs() < _gn_aux.get_std_bounds(
-                clk_diff, axis=0, sigma_coeff=3)]
+            clk_diff = clk_diff[clk_diff.abs() < _gn_aux.get_std_bounds(clk_diff, axis=0, sigma_coeff=3)]
         common_epochs_RAC_T = rac_unstack.index.intersection(
-            clk_diff.index.values)  # RAC epochs not present in clk_diff
-        common_svs = rac_unstack.columns.levels[1].intersection(
-            clk_diff.columns)   # RAC SVs not present in clk_diff
+            clk_diff.index.values
+        )  # RAC epochs not present in clk_diff
+
+        # NOTE: SV here refers to Satellite Vehicle ID, not to be confused with the *permanent* Satellite
+        # Vehicle Number.
+        # The columns here have been cleared of unused levels in sp3.diff_sp3_rac(). If this were not done, we would
+        # see failures here when baseline and test SP3 files have different SVs present.
+        common_svs = rac_unstack.columns.levels[1].intersection(clk_diff.columns)  # RAC SVs not present in clk_diff
+
         # common_epochs_RAC_T here might be not required. TODO
         clk_diff = clk_diff.loc[common_epochs_RAC_T][common_svs]
         rac_unstack = rac_unstack.loc[common_epochs_RAC_T].loc(axis=1)[:, common_svs]
     else:
         clk_diff = 0
-        _logging.debug(msg='computing orbit SISRE as clk offsets not given')
+        _logging.debug(msg="computing orbit SISRE as clk offsets not given")
 
     if use_rms:  # compute rms over each constellation svs at each epoch before moving on
-        rac_unstack.columns = [rac_unstack.columns.droplevel(
-            1), rac_unstack.columns.droplevel(0).values.astype('<U1')]
-        clk_diff.columns = clk_diff.columns.values.astype('<U1')
+        rac_unstack.columns = [rac_unstack.columns.droplevel(1), rac_unstack.columns.droplevel(0).values.astype("<U1")]
+        clk_diff.columns = clk_diff.columns.values.astype("<U1")
         rac_unstack = _gn_aux.rms(arr=rac_unstack, axis=1, level=[0, 1])
         clk_diff = _gn_aux.rms(clk_diff, axis=1, level=0)
 
     radial, along, cross = _np.hsplit(rac_unstack.values, 3)
-    coeffs_df = _gn_const.SISRE_COEF_DF.reindex(
-        columns=rac_unstack.Radial.columns.values.astype('<U1'))
+    coeffs_df = _gn_const.SISRE_COEF_DF.reindex(columns=rac_unstack.Radial.columns.values.astype("<U1"))
     alpha, beta = _np.vsplit(coeffs_df.values, indices_or_sections=2)
 
-    sisre = _pd.DataFrame(data=_np.sqrt((alpha*radial + clk_diff)**2 + (along**2 + cross**2)/beta),
-                          index=rac_unstack.index, columns=rac_unstack.Radial.columns)
-    if output_mode == 'sv':
+    sisre = _pd.DataFrame(
+        data=_np.sqrt((alpha * radial + clk_diff) ** 2 + (along**2 + cross**2) / beta),
+        index=rac_unstack.index,
+        columns=rac_unstack.Radial.columns,
+    )
+    if output_mode == "sv":
         return sisre  # returns per gnss if use_rms was selected
-    if output_mode in ['gnss', 'rms']:
+    if output_mode in ["gnss", "rms"]:
         if not use_rms:  # with use_rms, cols are already GNSS capitals
-            sisre.columns = sisre.columns.values.astype('<U1')
+            sisre.columns = sisre.columns.values.astype("<U1")
         # rms over all SVs of each constellation
         rms_sisre = _gn_aux.rms(sisre, axis=1, level=0)
-        if output_mode == 'gnss':
+        if output_mode == "gnss":
             return rms_sisre
         # rms over all epochs, a single value per constellation
         return _gn_aux.rms(rms_sisre, axis=0)
 
-def diffsp3(sp3_a_path, sp3_b_path, tol, log_lvl, clk_a_path, clk_b_path, hlm_mode=None, plot=False):
+
+def diffsp3(
+    sp3_a_path, sp3_b_path, tol, log_lvl, clk_a_path, clk_b_path, hlm_mode=None, plot=False, write_rac_file=False
+):
     """Compares two sp3 files and outputs a dataframe of differences above tolerance if such were found"""
     sp3_a, sp3_b = _gn_io.sp3.read_sp3(sp3_a_path), _gn_io.sp3.read_sp3(sp3_b_path)
 
-    as_sisre = False # the switch only needed for logging msg
+    as_sisre = False  # the switch only needed for logging msg
     clk_a = clk_b = None
     if (clk_a_path is not None) and (clk_b_path is not None):
         clk_a, clk_b = _gn_io.clk.read_clk(clk_a_path), _gn_io.clk.read_clk(clk_b_path)
         as_sisre = True
 
     status = 0
-    diff_rac = sisre(sp3_a=sp3_a.iloc[:,:3],sp3_b=sp3_b.iloc[:,:3],clk_a=clk_a,clk_b=clk_b,norm_type='both',output_mode='sv',clean=False,hlm_mode=hlm_mode, plot=plot)
+    diff_rac = sisre(
+        sp3_a=sp3_a.iloc[:, :3],
+        sp3_b=sp3_b.iloc[:, :3],
+        clk_a=clk_a,
+        clk_b=clk_b,
+        norm_type="both",
+        output_mode="sv",
+        clean=False,
+        hlm_mode=hlm_mode,
+        plot=plot,
+        write_rac_file=write_rac_file,
+    )
 
-    bad_rac_vals = _diff2msg(diff_rac,tol=tol)
+    bad_rac_vals = _diff2msg(diff_rac, tol=tol)
     if bad_rac_vals is not None:
-        _logging.log(msg=f':diffutil found {"SISRE values" if as_sisre else "estimates"} estimates diffs above {"the extracted STDs" if tol is None else f"{tol:.1E} tolerance"}:\n{bad_rac_vals.to_string(justify="center")}\n',level=log_lvl)
+        _logging.log(
+            msg=f':diffutil found {"SISRE values" if as_sisre else "estimates"} estimates diffs above {"the extracted STDs" if tol is None else f"{tol:.1E} tolerance"}:\n{bad_rac_vals.to_string(justify="center")}\n',
+            level=log_lvl,
+        )
         status = -1
     else:
-        _logging.log(msg=f':diffutil [OK] {"SISRE values" if as_sisre else "estimates"} diffs within {"the extracted STDs" if tol is None else f"{tol:.1E} tolerance"}',level=_logging.INFO)
+        _logging.log(
+            msg=f':diffutil [OK] {"SISRE values" if as_sisre else "estimates"} diffs within {"the extracted STDs" if tol is None else f"{tol:.1E} tolerance"}',
+            level=_logging.INFO,
+        )
     return status
 
+
 def diffpodout(pod_out_a_path, pod_out_b_path, tol, log_lvl):
     pod_out_a, pod_out_b = _gn_io.pod.read_pod_out(pod_out_a_path), _gn_io.pod.read_pod_out(pod_out_b_path)
     status = 0
-    diff_pod_out = (pod_out_a - pod_out_b)
+    diff_pod_out = pod_out_a - pod_out_b
 
-    bad_rac_vals = _diff2msg(diff_pod_out.unstack(1),tol=tol)
+    bad_rac_vals = _diff2msg(diff_pod_out.unstack(1), tol=tol)
     if bad_rac_vals is not None:
-        _logging.log(msg=f':diffutil found estimates diffs above {"the extracted STDs" if tol is None else f"{tol:.1E} tolerance"}:\n{bad_rac_vals.to_string(justify="center")}\n',level=log_lvl)
+        _logging.log(
+            msg=f':diffutil found estimates diffs above {"the extracted STDs" if tol is None else f"{tol:.1E} tolerance"}:\n{bad_rac_vals.to_string(justify="center")}\n',
+            level=log_lvl,
+        )
+        status = -1
+    else:
+        _logging.log(
+            msg=f':diffutil [OK] estimates diffs within {"the extracted STDs" if tol is None else f"{tol:.1E} tolerance"}',
+            level=_logging.INFO,
+        )
+    return status
+
+
+def diffblq(blq_a_path, blq_b_path, tol, log_lvl):
+    if tol is None:
+        _logging.error(":diffutil STD [tol=None] is not supported for the blq files")
+        return 0
+
+    blq_a, blq_b = _gn_io.blq.read_blq(blq_a_path), _gn_io.blq.read_blq(blq_b_path)
+    status = 0
+    diff = blq_a - blq_b
+    bad_blq_vals = _diff2msg(diff.abs().T, tol=tol, dt_as_gpsweek=None)
+    if bad_blq_vals is not None:
+        _logging.log(
+            msg=f':diffutil found diff magnitudes above {tol:.1E} tolerance:\n{bad_blq_vals.to_string(justify="center")}\n',
+            level=log_lvl,
+        )
         status = -1
     else:
-        _logging.log(msg=f':diffutil [OK] estimates diffs within {"the extracted STDs" if tol is None else f"{tol:.1E} tolerance"}',level=_logging.INFO)
+        _logging.log(
+            msg=f":diffutil [OK] estimates diffs within  {tol:.1E} tolerance",
+            level=_logging.INFO,
+        )
     return status
 
-def diffclk(clk_a_path, clk_b_path, tol, log_lvl):
+
+def diffclk(clk_a_path, clk_b_path, tol, log_lvl, norm_type="both"):
     """Compares two clk files and provides a difference above atol if present. If sp3 orbits provided - does analysis using the SISRE values"""
     clk_a, clk_b = _gn_io.clk.read_clk(clk_a_path), _gn_io.clk.read_clk(clk_b_path)
 
     status = 0
-    diff_clk = _compare_clk(clk_a=clk_a,clk_b=clk_b,norm_type='both')
+    diff_clk = compare_clk(clk_a=clk_a, clk_b=clk_b, norm_types=norm_type) * _gn_const.C_LIGHT
 
-    bad_clk_vals = _diff2msg(diff_clk,tol=tol)
+    bad_clk_vals = _diff2msg(diff_clk, tol=tol)
     if bad_clk_vals is not None:
-        _logging.log(msg=f':diffutil found norm clk diffs above {"the extracted STDs" if tol is None else f"{tol:.1E} tolerance"}:\n{bad_clk_vals.to_string(justify="center")}\n',level=log_lvl)
+        _logging.log(
+            msg=f':diffutil found norm clk diffs above {"the extracted STDs" if tol is None else f"{tol:.1E} tolerance"}:\n{bad_clk_vals.to_string(justify="center")}\n',
+            level=log_lvl,
+        )
         status -= 1
     else:
-        _logging.log(msg=f':diffutil [OK] norm clk diffs within the {"extracted STDs" if tol is None else f"{tol:.1E} tolerance"}',level=_logging.INFO)
-    return status
+        _logging.log(
+            msg=f':diffutil [OK] norm clk diffs within the {"extracted STDs" if tol is None else f"{tol:.1E} tolerance"}',
+            level=_logging.INFO,
+        )
+    return status
+
+
+def rac_df_to_rms_df(rac_df):
+    """Produces statistics over the input RAC dataframe and XYZ difference dataframe stored as an attribute:
+    RMS of dX, dY, dZ and R (Radial), A (Along-track), C (Cross-track) per satellite (PRN).
+    Additionally, a 1D mean difference, (dX + dY + dZ)/3, and 3D difference, sqrt(R^2 + A^2 + C^2), are computed for each PRN.
+    """
+    merged_data = rac_df.join(rac_df.attrs["diff_eci"])
+    rms_df = merged_data.pow(2).groupby("PRN").mean().pow(0.5)
+    std_df = merged_data.groupby("PRN").std(ddof=0)
+
+    rms_df["EST", "MEAN"] = rms_df.EST.mean(axis=1).groupby("PRN").mean()
+    rms_df["EST", "AVG"] = rac_df.attrs["diff_eci"].EST.mean(axis=1).groupby("PRN").mean()
+    std_df["EST", "3D_RMS"] = rac_df.attrs["diff_eci"].EST.pow(2).sum(axis=1).pow(0.5).groupby("PRN").std(ddof=0)
+    rms_df["EST", "3D_RMS"] = rac_df.attrs["diff_eci"].EST.pow(2).sum(axis=1).groupby("PRN").mean().pow(0.5)
+    rms_df = rms_df.droplevel(0, axis=1).rename(
+        columns={
+            "Radial": "R_RMS",
+            "Along-track": "A_RMS",
+            "Cross-track": "C_RMS",
+            "X": "dX_RMS",
+            "Y": "dY_RMS",
+            "Z": "dZ_RMS",
+        }
+    )
+    std_df = std_df.droplevel(0, axis=1).rename(
+        columns={
+            "Radial": "R_RMS",
+            "Along-track": "A_RMS",
+            "Cross-track": "C_RMS",
+            "X": "dX_RMS",
+            "Y": "dY_RMS",
+            "Z": "dZ_RMS",
+        }
+    )
+    # summarising over all SVs
+    summary_df = _pd.DataFrame(
+        [rms_df.mean(axis=0), std_df.mean(axis=0), rms_df.pow(2).mean(axis=0).pow(0.5)], index=["AVG", "STD", "RMS"]
+    )
+
+    rms_df.attrs["summary"] = summary_df
+    return rms_df
```

### Comparing `gnssanalysis-0.0.9/gnssanalysis/gn_frame.py` & `gnssanalysis-0.54/gnssanalysis/gn_frame.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,207 +1,209 @@
-'''frame of day generation module'''
+"""frame of day generation module"""
 import logging
+from typing import Union as _Union
 
 import numpy as _np
 import pandas as _pd
 
-from gnssanalysis import gn_datetime as _gn_datetime
-from gnssanalysis.gn_const import SEC_IN_YEAR as _SEC_IN_YEAR
-from gnssanalysis import gn_io as _gn_io
-from gnssanalysis import gn_transform as _gn_transform
+from . import gn_datetime as _gn_datetime
+from . import gn_const as _gn_const
+from . import gn_io as _gn_io
+from . import gn_transform as _gn_transform
 
 
 def _get_core_list(core_list_path):
-    '''itrf2014_to_itrf2008_stations '''
+    """itrf2014_to_itrf2008_stations"""
     # need to check if solution numbers are consistent with discontinuities selection
-    core_df = _pd.read_csv(core_list_path,
-                           delim_whitespace=True,
-                           skiprows=4,
-                           comment='-',
-                           usecols=[0, 1, 2, 3],
-                           names=['CODE', 'DOMES_NO', 'SOLN', 'TECH'])
+    core_df = _pd.read_csv(
+        core_list_path,
+        delim_whitespace=True,
+        skiprows=4,
+        comment="-",
+        usecols=[0, 1, 2, 3],
+        names=["CODE", "DOMES_NO", "SOLN", "TECH"],
+    )
     return core_df
 
 
-def get_frame_of_day(date_or_j2000, itrf_path_or_df, discon_path_or_df, psd_path_or_df=None, list_path_or_df=None):
-    '''Main function to propagate frame into datetime of interest
-    tech_name is one of ['GPS', 'VLBI', 'SLR', 'DORIS']'''
-    # assert tech_name in ['GPS', 'VLBI', 'SLR',
-    #                      'DORIS'], f'{tech_name} not in the TECH list'
+def get_frame_of_day(
+    date_or_j2000,
+    itrf_path_or_df: _Union[_pd.DataFrame, str],
+    discon_path_or_df: _Union[_pd.DataFrame, str],
+    psd_path_or_df: _Union[None, _pd.DataFrame, str] = None,
+    list_path_or_df: _Union[None, _pd.DataFrame, str, _np.ndarray] = None,
+):
+    """Main function to propagate frame into datetime of interest"""
 
-    if isinstance(date_or_j2000, int):
+    if isinstance(date_or_j2000, (int, _np.int64)):
         date_J2000 = date_or_j2000
     else:
         date_J2000 = _gn_datetime.datetime2j2000(_np.datetime64(date_or_j2000))
 
     # discontinuities file
-    if isinstance(discon_path_or_df,_pd.DataFrame):
+    if isinstance(discon_path_or_df, _pd.DataFrame):
         discon_df = discon_path_or_df
-    elif isinstance(discon_path_or_df,str):
+    elif isinstance(discon_path_or_df, str):
         discon_df = _gn_io.discon._read_discontinuities(discon_path_or_df)
     else:
-        logging.error(msg='check discon_path_or_df')
+        raise ValueError(f"discon_path_or_df must be a pandas DataFrame or str, got: {type(discon_path_or_df)}")
 
-    #itrf sinex file
+    # itrf sinex file
     if isinstance(itrf_path_or_df, _pd.DataFrame):
         output = itrf_path_or_df
     elif isinstance(itrf_path_or_df, str):
-        output = _gn_io.sinex._get_snx_vector_gzchunks(
-            filename=itrf_path_or_df, block_name='SOLUTION/ESTIMATE')
+        output = _gn_io.sinex._get_snx_vector_gzchunks(filename=itrf_path_or_df, block_name="SOLUTION/ESTIMATE")
     else:
-        logging.error(msg='check itrf_path_or_df')
+        raise ValueError(f"itrf_path_or_df must be a pandas DataFrame or str, got: {type(itrf_path_or_df)}")
 
-    discon_valid = discon_df[(discon_df.MODEL == 'P')
-                           & (discon_df.BEGIN != -999999999)
-                           & (discon_df.BEGIN < date_J2000)
-                           & (discon_df.END > date_J2000)]
-
-    comboindex = _pd.Index(output.CODE.values + '_' + output.PT.values.astype(object)
-                           + output.SOLN.values.astype(object))
-
-    itrf_code_pt = _pd.Index(output.CODE.values + '_' +
-                             output.PT.values.astype(object), name=None).unique()
-    soln_series = _pd.Series(index=itrf_code_pt, data='1')
+    discon_valid = discon_df[(discon_df.MODEL == "P") & (discon_df.START <= date_J2000) & (discon_df.END > date_J2000)]
+
+    itrf_code_pt_index = output.index.get_level_values("CODE_PT")
+    comboindex = itrf_code_pt_index + "_" + output.index.get_level_values("SOLN").astype("str")
+    itrf_code_pt_uniques = itrf_code_pt_index.unique()
+    soln_series = _pd.Series(data=0, index=itrf_code_pt_uniques, dtype=int)
 
     # clean discontinuities file from stations missing in the frame
-    comboindex_dv = _pd.Index(
-        discon_valid.CODE.values + '_' + discon_valid.PT.values)
-    dv_mask = comboindex_dv.isin(itrf_code_pt)
+    comboindex_dv = _pd.Index(discon_valid.CODE.values + "_" + discon_valid.PT.values)
+    dv_mask = comboindex_dv.isin(itrf_code_pt_uniques)
 
     # overwrite indices on discont
     soln_series.loc[comboindex_dv[dv_mask]] = discon_valid[dv_mask].SOLN
-    out = output[_pd.Index(comboindex).isin(
-        soln_series.index.values + soln_series.values)]
+    # remove all the stations that do not have a valid solution
+    soln_series = soln_series[soln_series.values.astype(bool)]
+    if not soln_series.values.nonzero()[0].size:
+        logging.error(msg="list stations are not in frame sinex")
+    # TODO cite specific page/line of the standard
+    soln_comboindex = soln_series.index.values + "_" + soln_series.values.astype(str)
+    out = output[comboindex.isin(soln_comboindex)]
 
     if list_path_or_df is not None:
-        if isinstance(list_path_or_df,_pd.DataFrame):
+        if isinstance(list_path_or_df, _pd.DataFrame):
             core_df = list_path_or_df
             core_list = core_df.CODE.values
-        elif isinstance(list_path_or_df,str):
+        elif isinstance(list_path_or_df, str):
             core_df = _get_core_list(list_path_or_df)
             core_list = core_df.CODE.values
-        elif isinstance(list_path_or_df,_np.ndarray) or isinstance(list_path_or_df,list):
+        elif isinstance(list_path_or_df, _np.ndarray) or isinstance(list_path_or_df, list):
             core_list = list_path_or_df
         else:
-            logging.error(msg='check list_path_or_df')
-        out_mask = out.CODE.isin(core_list)
-        if out_mask.sum()>0:
-            out = out[out_mask] 
+            raise ValueError(
+                f"list_path_or_df must be a pandas DataFrame, str or numpy ndarray, got: {type(list_path_or_df)}"
+            )
+        out_mask = out.index.get_level_values("CODE_PT").str[:4].isin(core_list)
+
+        if out_mask.any():
+            out = out[out_mask]
         else:
-            logging.error(msg='list stations are not in frame')
+            logging.error(msg="list stations not present in frame file")
             return None
 
-    # test3 =  test3[~test3.index.str.contains(pat='P\d{3}.')] #remove thise weird sites P104 etc
-
-    combo_index = out.CODE.values + '_' + out.PT.values.astype(object)
-    combo_index = _pd.MultiIndex.from_arrays([combo_index,out.TYPE])
+    out_xyzvel = _pd.Series(
+        data=out.VAL.EST.values,
+        index=_pd.MultiIndex.from_arrays([out.index.get_level_values("CODE_PT"), out.index.get_level_values("TYPE")]),
+    ).unstack(1)
 
-    duplicated_mask = combo_index.duplicated()
-    if duplicated_mask.sum() > 0:
-        logging.warning(msg=f'Removed duplicates of stations: {combo_index[duplicated_mask].get_level_values(0).unique().tolist()}')
-        out_xyzvel = out.EST[~duplicated_mask].copy()
-        out_xyzvel.index = combo_index[~duplicated_mask]
-    else:
-        out_xyzvel = out.EST.copy()
-        out_xyzvel.index = combo_index
-        
-    out_xyzvel = out_xyzvel.unstack(level=1)
-    itrf_reference = out['REF_EPOCH'].unique()[0]
+    # all values in the frame are relative to frame origin reference time (2010-01-02T00:00:00)
+    itrf_reference = out.index.get_level_values("REF_EPOCH")[0]
     time_seconds = date_J2000 - itrf_reference
 
     position = out_xyzvel.iloc[:, :3]
     velocities = out_xyzvel.iloc[:, 3:6]
-    out = position + velocities.values * (time_seconds/_SEC_IN_YEAR)
-    out.columns = out.columns.astype(str)
-    out['SOLN'] = ''
-    out['SOLN'] += soln_series
-    out.attrs['REF_EPOCH'] = date_J2000
+    out = position + velocities.values * (time_seconds / _gn_const.SEC_IN_YEAR)
 
+    out["SOLN"] = 0
+    out["SOLN"] += soln_series
+    out.attrs["REF_EPOCH"] = date_J2000
     if psd_path_or_df is not None:
-        if isinstance(psd_path_or_df,_pd.DataFrame):
+        if isinstance(psd_path_or_df, _pd.DataFrame):
+            logging.info(msg="reading postseismic from the dataframe provided")
             psd_df = psd_path_or_df
-        elif isinstance(psd_path_or_df,str):
+        elif isinstance(psd_path_or_df, str):
+            logging.info(msg=f"reading postseismic from {psd_path_or_df}")
             psd_df = _gn_io.psd._get_psd_df(psd_path_or_df)
         else:
-            logging.error(msg='check psd_path_or_df')
+            raise ValueError(f"psd_path_or_df must be a pandas DataFrame or str, got: {type(psd_path_or_df)}")
+        logging.info(msg="applying the computed postseismic deformations")
         out = psd2frame(frame_of_day=out, psd_df=psd_df)
     return out
 
 
 def psd2frame(frame_of_day, psd_df):
-    '''ref_epoch is extracted from frame_of_day attribute
+    """ref_epoch is extracted from frame_of_day attribute
     Outputs EST
-    |STAX|STAY|STAZ|'''
-    psd_df_ref = _get_psd_enu(psd_df=psd_df,
-                          date_J2000=frame_of_day.attrs['REF_EPOCH'])
-    frame_codes = frame_of_day.index.str.split(
-        '_', expand=True).get_level_values(level=0)
+    |STAX|STAY|STAZ|"""
+    psd_df_ref = _get_psd_enu(psd_df=psd_df.VAL, date_J2000=frame_of_day.attrs["REF_EPOCH"])
+    frame_codes = frame_of_day.index.str.split("_", expand=True).get_level_values(level=0)
 
     # if site has more than one monument - all monuments use same psd
-    psd_enu = _pd.DataFrame(index=frame_codes).join(
-        other=psd_df_ref).set_index(frame_of_day.index)
+    psd_enu = _pd.DataFrame(index=frame_codes).join(other=psd_df_ref).set_index(frame_of_day.index)
     # select only those sites that have psd event
     psd_enu = psd_enu[psd_enu.any(axis=1)]
 
-    llh = _gn_transform.xyz2llh_heik(xyz_array=frame_of_day[['STAX','STAY','STAZ']].loc[psd_enu.index].values)
+    llh = _gn_transform.xyz2llh(xyz_array=frame_of_day[["STAX", "STAY", "STAZ"]].loc[psd_enu.index].values)
     phi, lam = llh[:, 0], llh[:, 1]
-    rot = _gn_transform.llh2rot(phi=phi, lamb=lam)
+    rot = _gn_transform.llh2rot(phi=phi, lamb=lam, enu_to_ecef=True)
 
-    psd_xyz = _pd.DataFrame(data=_np.squeeze(psd_enu.values[:, _np.newaxis] @ rot, axis=1),
-                            index=psd_enu.index, columns=['STAX', 'STAY', 'STAZ'])
-    psd_xyz['SOLN'] = ''
+    psd_xyz = _pd.DataFrame(
+        data=(rot @ psd_enu.values[:, :, None]).reshape((-1, 3)),
+        index=psd_enu.index,
+        columns=["STAX", "STAY", "STAZ"],
+    )
+    psd_xyz["SOLN"] = ""
     frame_of_day.loc[psd_xyz.index] += psd_xyz
     return frame_of_day
 
 
 def _get_psd_enu(psd_df, date_J2000):
-    '''Reads psd file and computes psd values at each of east, north and up components for the data_J2000
-    Ignores the monument information as should be the same for different monuments of the same stations'''
+    """Reads psd file and computes psd values at each of east, north and up components for the data_J2000
+    Ignores the monument information as should be the same for different monuments of the same stations"""
     ref_epochs = psd_df.index.get_level_values(level=1)
     valid_mask = ref_epochs < date_J2000
 
     psd_coeff = psd_df[valid_mask].copy()
-    psd_coeff['dt_years'] = (date_J2000 - ref_epochs[valid_mask])/_SEC_IN_YEAR
+    psd_coeff["dt_years"] = (date_J2000 - ref_epochs[valid_mask]) / _gn_const.SEC_IN_YEAR
 
-    log_part = psd_coeff['ALOG'] * \
-        _np.log(1 + psd_coeff[['dt_years']].values / psd_coeff['TLOG'].values)
-    exp_part = psd_coeff['AEXP'] * \
-        (1 - _np.exp(-(psd_coeff[['dt_years']
-                                 ].values / psd_coeff['TEXP'].values)))
+    log_part = psd_coeff["ALOG"] * _np.log(1 + psd_coeff[["dt_years"]].values / psd_coeff["TLOG"].values)
+    exp_part = psd_coeff["AEXP"] * (1 - _np.exp(-(psd_coeff[["dt_years"]].values / psd_coeff["TEXP"].values)))
     log_part_grouped = log_part.groupby(axis=0, level=0).sum()
     exp_part_grouped = exp_part.groupby(axis=0, level=0).sum()
 
-    out = log_part_grouped.add(exp_part_grouped, fill_value=0)/1000
+    out = log_part_grouped.add(exp_part_grouped, fill_value=0) / 1000
     # if log or exp part is missing for the component, .add should take care of the nans being added
-    # .rename(columns={'E':'EAST','N':'NORTH','H':'UP'})
-    return out[['E', 'N', 'H']]
+    out.rename(columns={"E": "EAST", "N": "NORTH", "H": "UP", "U": "UP"}, inplace=True, errors="ignore")
+    return out[["EAST", "NORTH", "UP"]]
+
 
 # gather_reader
-def read_frame_snx_all(*file_paths,core_sites=None):
-    buf=[]
+def read_frame_snx_all(*file_paths, core_sites=None):
+    buf = []
     for path in file_paths:
-        buf.append(_gn_io.sinex._get_snx_vector_gzchunks(filename=path,block_name='SOLUTION/ESTIMATE'))
+        buf.append(
+            _gn_io.sinex._get_snx_vector_gzchunks(filename=path, block_name="SOLUTION/ESTIMATE"), snx_format="raw"
+        )
     all_frame = _pd.concat(buf)
     if core_sites is not None:
         return all_frame[all_frame.CODE.isin(core_sites)]
     return all_frame
 
-def read_disc_all(*file_paths,core_sites=None):
-    buf=[]
+
+def read_disc_all(*file_paths, core_sites=None):
+    buf = []
     for path in file_paths:
         buf.append(_gn_io.discon._read_discontinuities(path))
     all_discon = _pd.concat(buf)
-    all_discon = all_discon[all_discon.MODEL.values =='P']
-    
+    all_discon = all_discon[all_discon.MODEL.values == "P"]
+
     if core_sites is not None:
         return all_discon[all_discon.CODE.isin(core_sites)]
-    return all_discon 
+    return all_discon
 
-def read_psd_all(*file_paths,core_sites=None):
-    buf=[]
+
+def read_psd_all(*file_paths, core_sites=None):
+    buf = []
     for path in file_paths:
         buf.append(_gn_io.psd._get_psd_df(path))
     all_psd = _pd.concat(buf)
-    if core_sites is not None:   
+    if core_sites is not None:
         psd_sites = all_psd.index.levels[0]
         return all_psd.loc[psd_sites[psd_sites.isin(core_sites)]]
     return all_psd
```

### Comparing `gnssanalysis-0.0.9/gnssanalysis/gn_io/discon.py` & `gnssanalysis-0.54/gnssanalysis/gn_io/discon.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-'''Parser of frame discontinuity file'''
+"""Parser of frame discontinuity file"""
 from io import BytesIO as _BytesIO
 
 import pandas as _pd
 from pandas import CategoricalDtype as _CategoricalDtype
 
-from gnssanalysis import gn_datetime as _gn_datetime
-from gnssanalysis import gn_io as _gn_io
+from .. import gn_datetime as _gn_datetime
+from .. import gn_io as _gn_io
+
+MODEL_CATEGORY = _CategoricalDtype(categories=["P", "V", "A", "S", "E", "X"])
 
-MODEL_CATEGORY  = _CategoricalDtype(categories = ['P','V','A','S','E','X'])
 
 def _read_discontinuities(path):
+    """Reads ITRF/IGS frame discontinuity file into a dataframe changing zero datetime values to +/-999999999 depending if it's END of the solution (+) or START (-)"""
     snx_bytes = _gn_io.common.path2bytes(path)
-    block = _gn_io.sinex._snx_extract_blk(
-        snx_bytes=snx_bytes, blk_name='SOLUTION/DISCONTINUITY', remove_header=True)[0]
-    out_df = _pd.read_csv(filepath_or_buffer=_BytesIO(block),
-                          usecols=[0, 1, 2, 4, 5, 6],
-                          delim_whitespace=True,
-                          header=None,
-                          names=['CODE', 'PT', 'SOLN',
-                                 'BEGIN', 'END', 'MODEL'],
-                          dtype={
-        0: object, 1: object, 2: object,
-        4: object, 5: object, 6: MODEL_CATEGORY})
-
-    begin_j2000 = _gn_datetime.yydoysec2datetime(out_df['BEGIN'],as_j2000=True,recenter=False)
-    begin_j2000[begin_j2000 == -129600] = -999999999
-    #overwriting 00:000:00000 values with new boundaries
-
-    end_j2000 = _gn_datetime.yydoysec2datetime(out_df['END'],as_j2000=True,recenter=False)
-    end_j2000[end_j2000 == -129600] = 999999999
-
-    out_df['BEGIN'] = begin_j2000
-    out_df['END'] = end_j2000
-    #     return out_df
-    #     return out_df.set_index(out_df.CODE.values + out_df.PT.values + out_df.SOLN.values.astype(str))
-    return out_df.set_index(out_df.CODE.values + '_' + out_df.PT.values)
+    block = _gn_io.sinex._snx_extract_blk(snx_bytes=snx_bytes, blk_name="SOLUTION/DISCONTINUITY", remove_header=True)[0]
+    out_df = _pd.read_csv(
+        filepath_or_buffer=_BytesIO(block),
+        usecols=[0, 1, 2, 4, 5, 6],
+        delim_whitespace=True,
+        header=None,
+        names=["CODE", "PT", "SOLN", "START", "END", "MODEL"],
+        dtype={0: object, 1: object, 2: int, 4: object, 5: object, 6: MODEL_CATEGORY},
+        comment="*",
+        skip_blank_lines=True,
+    )
+
+    begin_j2000 = _gn_datetime.yydoysec2datetime(out_df["START"], as_j2000=True, recenter=False)
+    begin_j2000[begin_j2000 == -43200] = -999999999
+    # overwriting 00:000:00000 values with new boundaries
+
+    end_j2000 = _gn_datetime.yydoysec2datetime(out_df["END"], as_j2000=True, recenter=False)
+    end_j2000[end_j2000 == -43200] = 999999999
+
+    out_df["START"] = begin_j2000
+    out_df["END"] = end_j2000
+    return out_df.set_index(out_df.CODE.values + "_" + out_df.PT.values)
```

### Comparing `gnssanalysis-0.0.9/gnssanalysis/gn_io/igslog.py` & `gnssanalysis-0.54/gnssanalysis/gn_io/igslog.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,63 @@
-'''IGS log files parser'''
+"""IGS log files parser"""
 import glob as _glob
 import re as _re
 from multiprocessing import Pool as _Pool
 
 import numpy as _np
 import pandas as _pd
-from gnssanalysis import gn_datetime as _gn_datetime
-from gnssanalysis import gn_frame as _gn_frame
-from gnssanalysis import gn_io as _gn_io
-from gnssanalysis import gn_transform as _gn_transform
+from .. import gn_const as _gn_const
+from .. import gn_datetime as _gn_datetime
+from .. import gn_frame as _gn_frame
+from .. import gn_io as _gn_io
+from .. import gn_transform as _gn_transform
 from tqdm import tqdm
 
-_REGEX_ID  = _re.compile(rb'''
+_REGEX_ID = _re.compile(
+    rb"""
     (?:Four\sCharacter\sID|Site\sID)\s+\:\s*(\w{4}).*\W+
     .*\W+
     (?:\s{25}.+\W+|)
     IERS.+\:\s*(\w{9}|)
-    ''', _re.IGNORECASE|_re.VERBOSE)
+    """,
+    _re.IGNORECASE | _re.VERBOSE,
+)
 
-_REGEX_LOC = _re.compile(rb'''
+_REGEX_LOC = _re.compile(
+    rb"""
     2.+\W+City\sor\sTown\s+\:\s*(\w[^\(\n\,/\?]+|).*\W+
     State.+\W+Country\s+\:\s*([^\(\n\,\d]+|).*\W+(?:\s{25}.+\W+|)
     Tectonic.+\W+(?:\s{25}.+\W+|).+\W+
     X.{22}\:?\s*([\d\-\+\.\,]+|).*\W+
     Y.{22}\:?\s*([\d\-\+\.\,]+|).*\W+
     Z.{22}\:?\s*([\d\-\+\.\,]+|).*\W+
     Latitude.+\:\s*([\d\.\,\-\+]+|).*\W+
     Longitud.+\:\s*([\d\.\,\-\+]+|).*\W+
     Elevatio.+\:\s*([\d\.\,\-\+]+|).*
-    ''', _re.IGNORECASE|_re.VERBOSE)
+    """,
+    _re.IGNORECASE | _re.VERBOSE,
+)
 
 
-_REGEX_REC = _re.compile(  rb'''
+_REGEX_REC = _re.compile(
+    rb"""
     3\.\d+[ ]+Receiver[ ]Type\W+\:[ ]*([\+\-\w\ ]+|)\W+                           # Receiver Type line
     (?:Satellite[ ]System[ ]+\:[ ]*(?:(.+|)[ ]*[\r\n ]+[ ]+)|)      # Satellite System (normally present)
     Serial[ ]Number[ ]+\:[ ]*(\w+|).*\W+                                              # Receiver S/N line
     Firmware[ ]Version[ ]+\:[ ]*([\w\.\/ ]+|).*\W+                     # Receiver Firmware Version line
     ()()()                                             # 3 empty groups to align with antenna block
     (?:Elevation[ ]Cutoff\sSetting[ ]*\:[ ]*(?:.+|)|)\W+ # Elevation Cutoff Setting (normally present)
     Date[ ]Installed\W+\:[ ]*(\d{4}.+|).*\W+                                    # Date Installed line
     (?:Date[ ]Removed\W+\:(?:[ ]*(\d{4}.+|))|)                 # Date Removed line (normally present)
-    ''', _re.IGNORECASE|_re.VERBOSE)
+    """,
+    _re.IGNORECASE | _re.VERBOSE,
+)
 
-_REGEX_ANT = _re.compile(  rb'''
+_REGEX_ANT = _re.compile(
+    rb"""
     4\.\d+[ ]+Antenna[ ]Type\W+:[\t ]*([\/\_\S]+|)[ \t]*(\w+|)[\,?.]*\W+            # Antenna Type line
     Serial[ ]Number[ ]+:[ ]*(\S+|\S+[ ]\S+|\S+[ ]\S+[ ]\S+|).*\W+                      # Antenna S/N line
     (?:Antenna[ ]Height.+\W+|)                                        # Antenna H (normally present)
     (?:Antenna[ ]Ref.+\W+|)                                  # Antenna Ref. Point (normally present)
     (?:Degree.+\W+|)                                             # Degree offset line (rarely used)
     (?:Marker->ARP[ ]Up.+\:[ ]*([\-\d\.]+|).*\W+
     Marker->ARP[ ]North.+\:[ ]*([\-\d\.]+|).*\W+
@@ -54,414 +65,511 @@
     (?:Alignment.+[\n\r](?:[ ]{25}.+[\r\n]+|)\W+|)   # Alignment from True N line (normally present)
     Antenna[ ]Rad.+\:[ ]?(.+|)(?:\(.+\)|)\W+                               # Antenna Radome Type line
     (?:(?:(?:Rad|Antenna[ ]Rad).+\W+|)         # Radome S/N or Antenna Radome S/N (normally present)
     Ant.+[\n\r]+(?:[ ]{25}.+[\r\n]+|)\W+                                   # Antenna Cable Type line
     Ant.+[\n\r]+(?:[ ]{25}.+[\r\n]+|)\W+|)                               # Antenna Cable Length line
     Date[ ]Installed[ ]+\:[ ]*(\d{4}.+|).*\W+                                    # Date Installed line
     (?:Date[ ]Removed[ ]+\:(?:[ ]*(\d{4}.+|))|)                 # Date Removed line (normally present)
-    ''', _re.IGNORECASE|_re.VERBOSE)
+    """,
+    _re.IGNORECASE | _re.VERBOSE,
+)
 
-_REGEX_LOGNAME = r'(?:.*\/)(\w{4})(?:\w+_(\d{8})|_(\d{8})\-?\w?|(\d{8})|_.*|\d+|)'
+_REGEX_LOGNAME = r"(?:.*\/)(\w{4})(?:\w+_(\d{8})|_(\d{8})\-?\w?|(\d{8})|_.*|\d+|)"
 
-def find_recent_logs(logs_glob_path:str,rnx_glob_path=None)->_pd.DataFrame:
-    '''Takes glob expression to get the list of log files,
+
+def find_recent_logs(logs_glob_path: str, rnx_glob_path=None) -> _pd.DataFrame:
+    """Takes glob expression to get the list of log files,
      parses names into site and date and selects the ones
      with most recent date
     /data/station_logs/station_logs_IGS/*/*.log
-    /data/acs/pea/proc/exs/data/*.rnx'''
-    paths  = _pd.Series(_glob.glob(pathname=logs_glob_path,recursive=False),name='PATH')
+    /data/acs/pea/proc/exs/data/*.rnx"""
+    paths = _pd.Series(_glob.glob(pathname=logs_glob_path, recursive=False), name="PATH")
 
-    logs_df  = paths.str.extract(expand=True,pat=_REGEX_LOGNAME)
-    logs_df = _pd.concat([  logs_df[0].str.upper(),
-                            logs_df.iloc[:,1:].astype(float).sum(axis=1),
-                            paths],axis=1)
-    logs_df.columns = ['CODE','DATE','PATH']
-    logs_df = logs_df[~logs_df.CODE.isna()].sort_values(['CODE','DATE'])
-    recent_logs_df = logs_df[~logs_df.CODE.duplicated(keep='last')]
+    logs_df = paths.str.extract(expand=True, pat=_REGEX_LOGNAME)
+    logs_df = _pd.concat([logs_df[0].str.upper(), logs_df.iloc[:, 1:].astype(float).sum(axis=1), paths], axis=1)
+    logs_df.columns = ["CODE", "DATE", "PATH"]
+    logs_df = logs_df[~logs_df.CODE.isna()].sort_values(["CODE", "DATE"])
+    recent_logs_df = logs_df[~logs_df.CODE.duplicated(keep="last")]
     if rnx_glob_path is not None:
-        if isinstance(rnx_glob_path,list):
+        if isinstance(rnx_glob_path, list):
             rnx_stations = rnx_glob_path
-        if isinstance(rnx_glob_path,str):
+        if isinstance(rnx_glob_path, str):
             rnx_files = sorted(_glob.glob(rnx_glob_path))
-            assert len(rnx_files)!=0, f"No rnx files were found using '{rnx_glob_path}'"
-            rnx_stations =  _pd.Series(rnx_files).str.extract(r'(\w{4})[^\/]+$',expand=False).to_list()
+            assert len(rnx_files) != 0, f"No rnx files were found using '{rnx_glob_path}'"
+            rnx_stations = _pd.Series(rnx_files).str.extract(r"(\w{4})[^\/]+$", expand=False).to_list()
         return recent_logs_df[recent_logs_df.CODE.isin(rnx_stations).values]
     return recent_logs_df
 
-def parse_igs_log(filename_array:_np.ndarray)->_np.ndarray:
-    '''Parses igs log and outputs ndarray with parsed data
-    Expects ndarray of the form [CODE DATE PATH]'''
+
+def parse_igs_log(filename_array: _np.ndarray) -> _np.ndarray:
+    """Parses igs log and outputs ndarray with parsed data
+    Expects ndarray of the form [CODE DATE PATH]"""
     file_code, __, file_path = filename_array
 
-    with open(file_path, 'rb') as file:
+    with open(file_path, "rb") as file:
         data = file.read()
 
     blk_id = _REGEX_ID.search(data)
     if blk_id is None:
-        tqdm.write(f'ID rejected from {file_path}')
-        return _np.array([]).reshape(0,12)
+        tqdm.write(f"ID rejected from {file_path}")
+        return _np.array([]).reshape(0, 12)
 
-    blk_id = [blk_id[1].decode().upper(),blk_id[2].decode().upper()] #no .groups() thus 1 and 2
+    blk_id = [blk_id[1].decode().upper(), blk_id[2].decode().upper()]  # no .groups() thus 1 and 2
     code = blk_id[0]
-    if code!=file_code:
-        tqdm.write(f'{code}!={file_code} at {file_path}')
-        return _np.array([]).reshape(0,12)
+    if code != file_code:
+        tqdm.write(f"{code}!={file_code} at {file_path}")
+        return _np.array([]).reshape(0, 12)
 
     blk_loc = _REGEX_LOC.search(data)
     if blk_loc is None:
-        tqdm.write(f'LOC rejected from {file_path}')
-        return _np.array([]).reshape(0,12)
+        tqdm.write(f"LOC rejected from {file_path}")
+        return _np.array([]).reshape(0, 12)
 
     blk_rec = _REGEX_REC.findall(data)
     if blk_rec == []:
-        tqdm.write(f'REC rejected from {file_path}')
-        return _np.array([]).reshape(0,12)
+        tqdm.write(f"REC rejected from {file_path}")
+        return _np.array([]).reshape(0, 12)
 
     blk_ant = _REGEX_ANT.findall(data)
     if blk_ant == []:
-        tqdm.write(f'ANT rejected from {file_path}')
-        return _np.array([]).reshape(0,12)
+        tqdm.write(f"ANT rejected from {file_path}")
+        return _np.array([]).reshape(0, 12)
 
-    blk_loc = [group.decode(encoding='utf8',errors='ignore') for group in blk_loc.groups()]
-    blk_rec = _np.asarray(blk_rec,dtype=str)
-    blk_ant = _np.asarray(blk_ant,dtype=str)
+    blk_loc = [group.decode(encoding="utf8", errors="ignore") for group in blk_loc.groups()]
+    blk_rec = _np.asarray(blk_rec, dtype=str)
+    blk_ant = _np.asarray(blk_ant, dtype=str)
 
     len_recs = blk_rec.shape[0]
     len_ants = blk_ant.shape[0]
 
-    blk_id_loc = _np.asarray([0] + blk_id + blk_loc,dtype=object)[_np.newaxis]
+    blk_id_loc = _np.asarray([0] + blk_id + blk_loc, dtype=object)[_np.newaxis]
 
     code = [code]
-    blk_rec = _np.concatenate([_np.asarray([1]*len_recs,dtype=object)[:,_np.newaxis],
-                               _np.asarray(code*len_recs,dtype=object)[:,_np.newaxis],
-                               blk_rec,],axis=1)
-    blk_ant = _np.concatenate([_np.asarray([2]*len_ants,dtype=object)[:,_np.newaxis],
-                               _np.asarray(code*len_ants,dtype=object)[:,_np.newaxis],
-                               blk_ant,],axis=1)
-    blk_uni = _np.concatenate([blk_id_loc,blk_rec,blk_ant],axis=0)
-    file_path_arr = _np.asarray([file_path]*(1+len_ants+len_recs))[:,_np.newaxis]
-    return _np.concatenate([blk_uni,file_path_arr],axis=1)
-
-
-def igslogdate2datetime64(stacked_rec_ant_dt:_np.ndarray):
-    '''2010-01-01T00:00
-    - can be any non-space character. If parsing fails - None'''
-    dt_array_float = (_pd.Series(stacked_rec_ant_dt)
-                      .str.extract(pat=r'(\d{4})\S?(\d{2})\S?(\d+)\D?(?:(\d{1,2})\:(\d{1,2})\D?|)')
-                      .values.astype(float))
-
-    dt_array_float[_np.isnan(dt_array_float[:,0])] = [2100.,1.,1.,0.,0.]
-    hh_mm = dt_array_float[:,[3,4]]
-    hh_mm[_np.isnan(hh_mm[:,0])] = [0,0]
-    dt_array_float[:,[3,4]] = hh_mm
+    blk_rec = _np.concatenate(
+        [
+            _np.asarray([1] * len_recs, dtype=object)[:, _np.newaxis],
+            _np.asarray(code * len_recs, dtype=object)[:, _np.newaxis],
+            blk_rec,
+        ],
+        axis=1,
+    )
+    blk_ant = _np.concatenate(
+        [
+            _np.asarray([2] * len_ants, dtype=object)[:, _np.newaxis],
+            _np.asarray(code * len_ants, dtype=object)[:, _np.newaxis],
+            blk_ant,
+        ],
+        axis=1,
+    )
+    blk_uni = _np.concatenate([blk_id_loc, blk_rec, blk_ant], axis=0)
+    file_path_arr = _np.asarray([file_path] * (1 + len_ants + len_recs))[:, _np.newaxis]
+    return _np.concatenate([blk_uni, file_path_arr], axis=1)
+
+
+def igslogdate2datetime64(stacked_rec_ant_dt: _np.ndarray):
+    """2010-01-01T00:00
+    - can be any non-space character. If parsing fails - None"""
+    dt_array_float = (
+        _pd.Series(stacked_rec_ant_dt)
+        .str.extract(pat=r"(\d{4})\S?(\d{2})\S?(\d+)\D?(?:(\d{1,2})\:(\d{1,2})\D?|)")
+        .values.astype(float)
+    )
+
+    dt_array_float[_np.isnan(dt_array_float[:, 0])] = [2100.0, 1.0, 1.0, 0.0, 0.0]
+    hh_mm = dt_array_float[:, [3, 4]]
+    hh_mm[_np.isnan(hh_mm[:, 0])] = [0, 0]
+    dt_array_float[:, [3, 4]] = hh_mm
     dt_array_int = dt_array_float.astype(int)
 
-    wrong_31 = (_pd.Series(dt_array_int[:,1]).isin([4,6,9,11]).values) & (dt_array_int[:,2] > 30)
-    wrong_30 = (dt_array_int[:,1]==2) & (_pd.Series(dt_array_int[:,2]) > 29)
+    wrong_31 = (_pd.Series(dt_array_int[:, 1]).isin([4, 6, 9, 11]).values) & (dt_array_int[:, 2] > 30)
+    wrong_30 = (dt_array_int[:, 1] == 2) & (_pd.Series(dt_array_int[:, 2]) > 29)
 
-    valid_mask =  ((dt_array_int[:,3]<24)
-                & (dt_array_int[:,4] < 60)
-                & (dt_array_int[:,2] < 32)
-                & (dt_array_int[:,2] > 0)
-                & (dt_array_int[:,1] < 13)
-                & (dt_array_int[:,1] > 0)
-                & ~wrong_31
-                & ~wrong_30).values
-
-
-    dt_datetime64 = _np.empty(dt_array_int.shape[0],dtype='datetime64[m]')
-    dt_datetime64.fill(_np.NaN)
-
-    df_dt_valid = _pd.DataFrame(dt_array_int[valid_mask],dtype=str)
-    dt_datetime64[valid_mask] = (df_dt_valid[0].str.zfill(4)
-                            + '-'+ df_dt_valid[1].str.zfill(2)
-                            + '-'+ df_dt_valid[2].str.zfill(2)
-                            + ' '+ df_dt_valid[3].str.zfill(2)
-                            + ':'+ df_dt_valid[4].str.zfill(2) ).values.astype('datetime64')
+    valid_mask = (
+        (dt_array_int[:, 3] < 24)
+        & (dt_array_int[:, 4] < 60)
+        & (dt_array_int[:, 2] < 32)
+        & (dt_array_int[:, 2] > 0)
+        & (dt_array_int[:, 1] < 13)
+        & (dt_array_int[:, 1] > 0)
+        & ~wrong_31
+        & ~wrong_30
+    ).values
+
+    dt_datetime64 = _np.full(dt_array_int.shape[0], _np.datetime64("nat"), dtype="datetime64[m]")
+
+    df_dt_valid = _pd.DataFrame(dt_array_int[valid_mask], dtype=str)
+    dt_datetime64[valid_mask] = (
+        df_dt_valid[0].str.zfill(4)
+        + "-"
+        + df_dt_valid[1].str.zfill(2)
+        + "-"
+        + df_dt_valid[2].str.zfill(2)
+        + " "
+        + df_dt_valid[3].str.zfill(2)
+        + ":"
+        + df_dt_valid[4].str.zfill(2)
+    ).values.astype("datetime64")
     return dt_datetime64
 
 
-
-def translate_series(series,translation):
-    '''changes values in the series according to the dictionary of old_value-new_value'''
+def translate_series(series, translation):
+    """changes values in the series according to the dictionary of old_value-new_value"""
     series = series.copy()
     series.index = series.values
     series.update(translation)
     return series
 
-def gather_metadata(logs_glob_path = '/data/station_logs/station_logs_IGS/*/*.log',
-                    rnx_glob_path=None,
-                    num_threads=1):
-    '''parses logiles found with glob expression'''
-    parsed_filenames = find_recent_logs(logs_glob_path=logs_glob_path,
-                                        rnx_glob_path=rnx_glob_path).values
+
+def gather_metadata(logs_glob_path="/data/station_logs/station_logs_IGS/*/*.log", rnx_glob_path=None, num_threads=1):
+    """parses logiles found with glob expression"""
+    parsed_filenames = find_recent_logs(logs_glob_path=logs_glob_path, rnx_glob_path=rnx_glob_path).values
 
     total = parsed_filenames.shape[0]
     if num_threads == 1:
         gather = []
-        for file in tqdm(parsed_filenames,miniters=total//100,total=total):
+        for file in tqdm(parsed_filenames, miniters=total // 100, total=total):
             gather.append(parse_igs_log(file))
     else:
         with _Pool(processes=num_threads) as pool:
-            gather = list(tqdm(pool.imap_unordered(parse_igs_log, parsed_filenames),
-                               total=total, miniters=total//100))
+            gather = list(
+                tqdm(pool.imap_unordered(parse_igs_log, parsed_filenames), total=total, miniters=total // 100)
+            )
 
     gather_raw = _np.concatenate(gather)
 
     rec_ant_mask = gather_raw[:, 0] != 0  # id_loc = 0, rec = 1, ant = 2
     gather_id_loc = gather_raw[~rec_ant_mask][:, 1:]
     gather = gather_raw[rec_ant_mask]
 
-    stacked_rec_ant_dt = _np.concatenate(
-        [gather[:, -3], gather[:, -2]], axis=0)
+    stacked_rec_ant_dt = _np.concatenate([gather[:, -3], gather[:, -2]], axis=0)
 
     stacked_rec_ant_dt = igslogdate2datetime64(stacked_rec_ant_dt)
     snx_date = _gn_datetime.datetime2yydoysec(stacked_rec_ant_dt)
 
     gather = _np.concatenate([gather, snx_date.reshape(2, gather.shape[0]).T], axis=1)
     stacked_rec_ant_dt_beg_end = stacked_rec_ant_dt.reshape(2, gather.shape[0])  # also deals with nans as no equal sign
     # same foes for station start being empty as it becomes year 2100
     valid_mask_dt = stacked_rec_ant_dt_beg_end[0] < stacked_rec_ant_dt_beg_end[1]
 
     bad_dt_stations = _np.unique(gather[~valid_mask_dt][:, 1])
 
     rec_mask = gather[:, 0] == 1
-    rec_df = _pd.DataFrame( _np.delete(arr=gather[rec_mask], axis=1, obj=[0, 6, 7, 8]),
-                            columns=['CODE','RECEIVER','GNSS','S/N','FW','BEGIN_RAW','END_RAW',
-                                    'PATH','BEGIN_SNX','END_SNX'])
-    ant_df = _pd.DataFrame( gather[~rec_mask][:, 1:],
-                            columns=['CODE','ANTENNA','RADOME','S/N','EccU','EccN','EccE',
-                                    'RADOME2','BEGIN_RAW','END_RAW','PATH','BEGIN_SNX', 'END_SNX'])
+    rec_df = _pd.DataFrame(
+        _np.delete(arr=gather[rec_mask], axis=1, obj=[0, 6, 7, 8]),
+        columns=["CODE", "RECEIVER", "GNSS", "S/N", "FW", "BEGIN_RAW", "END_RAW", "PATH", "BEGIN_SNX", "END_SNX"],
+    )
+    ant_df = _pd.DataFrame(
+        gather[~rec_mask][:, 1:],
+        columns=[
+            "CODE",
+            "ANTENNA",
+            "RADOME",
+            "S/N",
+            "EccU",
+            "EccN",
+            "EccE",
+            "RADOME2",
+            "BEGIN_RAW",
+            "END_RAW",
+            "PATH",
+            "BEGIN_SNX",
+            "END_SNX",
+        ],
+    )
 
     # ID LOC
-    id_loc_df = _pd.DataFrame(gather_id_loc,columns=['CODE','DOMES_N','CITY','COUNTRY',
-                                                    'X','Y','Z','LAT','LON','HEI','PATH'])
+    id_loc_df = _pd.DataFrame(
+        gather_id_loc, columns=["CODE", "DOMES_N", "CITY", "COUNTRY", "X", "Y", "Z", "LAT", "LON", "HEI", "PATH"]
+    )
 
-    id_loc_df.CITY[id_loc_df.CITY == ''] = 'N/A'
+    id_loc_df.CITY[id_loc_df.CITY == ""] = "N/A"
     id_loc_df.CITY = id_loc_df.CITY.str.rstrip().str.upper()
-    id_loc_df.COUNTRY = translate_series(id_loc_df.COUNTRY.str.rstrip().str.upper(),
-                                        _gn_io.aux_dicts.translation_country).values
-    id_loc_df.DOMES_N[id_loc_df.DOMES_N == ''] = '---------'
-
-
-    xyz_array = (id_loc_df[['X','Y','Z']].stack()
-                            .str.replace(',','.')
-                            .replace({'':None})
-                            .unstack().values.astype(float))
-
+    id_loc_df.COUNTRY = translate_series(
+        id_loc_df.COUNTRY.str.rstrip().str.upper(), _gn_io.aux_dicts.translation_country
+    ).values
+    id_loc_df.DOMES_N[id_loc_df.DOMES_N == ""] = "---------"
 
-    valid_mask = _np.all((( xyz_array != 0) & ~_np.isnan(xyz_array)),axis=1)
+    xyz_array = (
+        id_loc_df[["X", "Y", "Z"]].stack().str.replace(",", ".").replace({"": None}).unstack().values.astype(float)
+    )
 
-    xyz_norm = (xyz_array[valid_mask] ** 2).sum(axis=1) **0.5
-    valid_mask[valid_mask] = (xyz_norm > 6000000) &(xyz_norm < 6500000)
+    valid_mask = _np.all(((xyz_array != 0) & ~_np.isnan(xyz_array)), axis=1)
 
+    xyz_norm = (xyz_array[valid_mask] ** 2).sum(axis=1) ** 0.5
+    valid_mask[valid_mask] = (xyz_norm > 6000000) & (xyz_norm < 6500000)
 
-    llh = _gn_transform.xyz2llh_heik(xyz_array[valid_mask],deg=True)
+    llh = _gn_transform.xyz2llh(xyz_array[valid_mask], method="heikkinen", ellipsoid=_gn_const.WGS84, latlon_as_deg=True)
     llh_snx = _gn_io.sinex.llh2snxdms(llh)
 
-    llh2  = id_loc_df[~valid_mask][['LAT','LON','HEI']]
+    llh2 = id_loc_df[~valid_mask][["LAT", "LON", "HEI"]]
     llh2_snx = _gn_io.sinex.logllh2snxdms(llh2)
-    snxdms = _np.empty(valid_mask.shape,dtype=object)
+    snxdms = _np.empty(valid_mask.shape, dtype=object)
     snxdms[valid_mask] = llh_snx
     # snxdms[valid_mask] =' 000 00 00.0  00 00 00.0   000.0'
-    snxdms[~valid_mask] = llh2_snx#
+    snxdms[~valid_mask] = llh2_snx  #
     # snxdms[~valid_mask] = ' 000 00 00.0  00 00 00.0   000.0'#llh2_snx
     # bad_loc_stations = id_loc_df.CODE[snxdms == ''].values
-    id_loc_df['LOC'] = snxdms
+    id_loc_df["LOC"] = snxdms
 
-    ecc = ant_df[['EccU','EccN','EccE']].values
-    ecc[ecc == ''] = 0
-    ant_df[['EccU','EccN','EccE']] = ecc.astype(float)
+    ecc = ant_df[["EccU", "EccN", "EccE"]].values
+    ecc[ecc == ""] = 0
+    ant_df[["EccU", "EccN", "EccE"]] = ecc.astype(float)
 
     rec_df.RECEIVER = rec_df.RECEIVER.str.rstrip().str.upper()
-    ant_df.ANTENNA  = ant_df.ANTENNA.str.rstrip().str.upper()
-    ant_df.RADOME   = ant_df.RADOME.str.rstrip().str.upper()
-    ant_df.RADOME2  = ant_df.RADOME2.str.rstrip().str.upper()
+    ant_df.ANTENNA = ant_df.ANTENNA.str.rstrip().str.upper()
+    ant_df.RADOME = ant_df.RADOME.str.rstrip().str.upper()
+    ant_df.RADOME2 = ant_df.RADOME2.str.rstrip().str.upper()
 
     no_rad2_mask = ~ant_df.RADOME.isin(_gn_io.aux_dicts.atx_rad_tbl)
     ant_df.RADOME[no_rad2_mask] = ant_df.RADOME2[no_rad2_mask]
     # translation_ant.index.name= None
-    antennas = translate_series(ant_df.ANTENNA,_gn_io.aux_dicts.translation_ant)
+    antennas = translate_series(ant_df.ANTENNA, _gn_io.aux_dicts.translation_ant)
     invalid_ant_mask = ~antennas.index.isin(_gn_io.aux_dicts.atx_ant_tbl)
-    bad_antenna_stations = ant_df[invalid_ant_mask]['CODE'].unique()
+    bad_antenna_stations = ant_df[invalid_ant_mask]["CODE"].unique()
 
-    receivers = translate_series(rec_df.RECEIVER,_gn_io.aux_dicts.translation_rec)
+    receivers = translate_series(rec_df.RECEIVER, _gn_io.aux_dicts.translation_rec)
     invalid_rec_mask = ~receivers.index.isin(_gn_io.aux_dicts.igs_rec_tbl)
-    bad_rec_stations = rec_df[invalid_rec_mask]['CODE'].unique()
+    bad_rec_stations = rec_df[invalid_rec_mask]["CODE"].unique()
 
-    radomes = translate_series(ant_df.RADOME,_gn_io.aux_dicts.translation_rad)
+    radomes = translate_series(ant_df.RADOME, _gn_io.aux_dicts.translation_rad)
 
     invalid_radomes_mask = ~radomes.index.isin(_gn_io.aux_dicts.atx_rad_tbl)
-    bad_radome_stations = ant_df[invalid_radomes_mask]['CODE'].unique()
+    bad_radome_stations = ant_df[invalid_radomes_mask]["CODE"].unique()
 
-    ant_df.ANTENNA  = antennas.values
-    ant_df.RADOME   = radomes.values
+    ant_df.ANTENNA = antennas.values
+    ant_df.RADOME = radomes.values
     rec_df.RECEIVER = receivers.values
 
-    bad_stations = _np.unique(bad_dt_stations.tolist()
-                              + bad_radome_stations.tolist()
-                              + bad_antenna_stations.tolist()
-                              + bad_rec_stations.tolist())
+    bad_stations = _np.unique(
+        bad_dt_stations.tolist()
+        + bad_radome_stations.tolist()
+        + bad_antenna_stations.tolist()
+        + bad_rec_stations.tolist()
+    )
 
     rec_df = rec_df[~rec_df.CODE.isin(bad_stations)].copy()
     ant_df = ant_df[~ant_df.CODE.isin(bad_stations)].copy()
     id_loc_df = id_loc_df[~id_loc_df.CODE.isin(bad_stations)].copy()
 
-    return id_loc_df,rec_df,ant_df
+    return id_loc_df, rec_df, ant_df
+
 
 def frame2snx_string(frame_of_day):
-    '''frame_of_day dataframe to ESTIMATE sinex block'''
-    code_pt =frame_of_day.index.to_series().str.split('_',expand=True)#.to_frame().values
-    code_pt.columns = ['CODE','PT']
-    frame_dt = _gn_datetime.j20002datetime(frame_of_day.attrs['REF_EPOCH'])
-    frame = _pd.concat([frame_of_day,code_pt],axis=1)#.reindex()
-    frame_est = frame[['STAX','STAY','STAZ']].stack(0).to_frame().reset_index(level=1)
-    frame_est.columns = ['TYPE','EST']
-    frame = frame_est.join(frame[['SOLN','CODE','PT']])
+    """frame_of_day dataframe to ESTIMATE sinex block"""
+    code_pt = frame_of_day.index.to_series().str.split("_", expand=True)  # .to_frame().values
+    code_pt.columns = ["CODE", "PT"]
+    frame_dt = _gn_datetime.j20002datetime(frame_of_day.attrs["REF_EPOCH"])
+    frame = _pd.concat([frame_of_day, code_pt], axis=1)  # .reindex()
+    frame_est = frame[["STAX", "STAY", "STAZ"]].stack(0).to_frame().reset_index(level=1)
+    frame_est.columns = ["TYPE", "EST"]
+    frame = frame_est.join(frame[["SOLN", "CODE", "PT"]])
 
     dt_snx = _gn_datetime.datetime2yydoysec(frame_dt)
 
-    frame.reset_index(drop=True,inplace=True)
-    frame['STD'] = 0
-    frame['INDEX'] = (frame.index +1)
-    frame.SOLN =  frame.SOLN.apply(r'{:>4}'.format)
-
-    epoch_str_series = (' ' + frame.CODE + '  ' + frame.PT + ' ' + frame.SOLN
-    + ' C 00:000:00000 00:000:00000 ' + dt_snx + '\n').to_list()
-
-    frame_str_series =(frame.INDEX.apply(r'{:6} '.format)
-    + frame.TYPE + '   ' + frame.CODE + '  ' + frame.PT + ' '
-    + frame.SOLN + ' ' + dt_snx + ' m    2 '
-    + frame.EST.apply(r'{:>21.14E}'.format) + ' 0.00000E+00\n').to_list()
+    frame.reset_index(drop=True, inplace=True)
+    frame["STD"] = 0
+    frame["INDEX"] = frame.index + 1
+    frame.SOLN = frame.SOLN.apply(r"{:>4}".format)
+
+    epoch_str_series = (
+        " " + frame.CODE + "  " + frame.PT + " " + frame.SOLN + " C 00:000:00000 00:000:00000 " + dt_snx + "\n"
+    ).to_list()
+
+    frame_str_series = (
+        frame.INDEX.apply(r"{:6} ".format)
+        + frame.TYPE
+        + "   "
+        + frame.CODE
+        + "  "
+        + frame.PT
+        + " "
+        + frame.SOLN
+        + " "
+        + dt_snx
+        + " m    2 "
+        + frame.EST.apply(r"{:>21.14E}".format)
+        + " 0.00000E+00\n"
+    ).to_list()
 
     buf = (
-      ['*-------------------------------------------------------------------------------\n']
-    + ['+SOLUTION/EPOCHS\n']
-    + ['*CODE PT SOLN T _DATA_START_ __DATA_END__ _MEAN_EPOCH_\n']
-    + epoch_str_series
-    + ['-SOLUTION/EPOCHS\n']
-    + ['*-------------------------------------------------------------------------------\n']
-    + ['+SOLUTION/ESTIMATE\n']
-    + ['*INDEX _TYPE_ CODE PT SOLN _REF_EPOCH__ UNIT S ___ESTIMATED_VALUE___ __STD_DEV__\n']
-    + frame_str_series
-    + ['-SOLUTION/ESTIMATE\n'])
+        ["*-------------------------------------------------------------------------------\n"]
+        + ["+SOLUTION/EPOCHS\n"]
+        + ["*CODE PT SOLN T _DATA_START_ __DATA_END__ _MEAN_EPOCH_\n"]
+        + epoch_str_series
+        + ["-SOLUTION/EPOCHS\n"]
+        + ["*-------------------------------------------------------------------------------\n"]
+        + ["+SOLUTION/ESTIMATE\n"]
+        + ["*INDEX _TYPE_ CODE PT SOLN _REF_EPOCH__ UNIT S ___ESTIMATED_VALUE___ __STD_DEV__\n"]
+        + frame_str_series
+        + ["-SOLUTION/ESTIMATE\n"]
+    )
 
     return buf
 
-def meta2sting(id_loc_df,rec_df,ant_df):
-    '''Converts three metadata dataframe to sinex blocks (string)'''
-    rec_df['S/N'] = rec_df['S/N'].str.slice(0,5)
-    rec_df['FW']  = rec_df['FW'].str.slice(0,11)
-
-    ant_df['S/N'] = ant_df['S/N'].str.slice(0,5)
-    ant_df.ANTENNA = ant_df.ANTENNA.str.ljust(15)#(r'{:15s}'.format)
-    ant_df.RADOME = ant_df.RADOME.str.ljust(4)
-    ant_df[['EccU','EccN','EccE']] = ant_df[['EccU','EccN','EccE']].applymap(r'{0:8.4f}'.format)
 
-    location = (id_loc_df.CITY.str.slice(0,16).str.rstrip() + ', '
-                + id_loc_df.COUNTRY).str.slice(0,22).str.ljust(22,' ').values
+def meta2sting(id_loc_df, rec_df, ant_df):
+    """Converts three metadata dataframe to sinex blocks (string)"""
+    rec_df["S/N"] = rec_df["S/N"].str.slice(0, 5)
+    rec_df["FW"] = rec_df["FW"].str.slice(0, 11)
 
-    id_str_list = (' ' + id_loc_df.CODE.values + '  A ' + id_loc_df.DOMES_N.values + ' P '
-                   + location + id_loc_df.LOC.values + '\n').tolist()
+    ant_df["S/N"] = ant_df["S/N"].str.slice(0, 5)
+    ant_df.ANTENNA = ant_df.ANTENNA.str.ljust(15)  # (r'{:15s}'.format)
+    ant_df.RADOME = ant_df.RADOME.str.ljust(4)
+    ant_df[["EccU", "EccN", "EccE"]] = ant_df[["EccU", "EccN", "EccE"]].applymap(r"{0:8.4f}".format)
 
-    rec_str_list = (' ' + rec_df.CODE + '  A ---- P '
-                    + rec_df.BEGIN_SNX + ' ' + rec_df.END_SNX + ' ' +
-                    + rec_df.RECEIVER.str.ljust(20,' ') + ' '
-                    + rec_df['S/N'].str.ljust(5,' ') + ' ' + rec_df.FW+'\n').to_list()
-
-    ant_str_list = (' ' + ant_df.CODE + '  A ---- P '
-                    + ant_df.BEGIN_SNX + ' ' + ant_df.END_SNX + ' '
-                    + ant_df.ANTENNA   + ' ' + ant_df.RADOME  + ' '
-                    + ant_df['S/N'] +'\n').to_list()
-
-    ecc_str_list = (' ' + ant_df.CODE + '  A ---- P '
-                    + ant_df.BEGIN_SNX + ' ' + ant_df.END_SNX
-                    + ' UNE ' + ant_df.EccU +' '+ ant_df.EccN +' ' + ant_df.EccE +'\n').to_list()
+    location = (
+        (id_loc_df.CITY.str.slice(0, 16).str.rstrip() + ", " + id_loc_df.COUNTRY)
+        .str.slice(0, 22)
+        .str.ljust(22, " ")
+        .values
+    )
+
+    id_str_list = (
+        " " + id_loc_df.CODE.values + "  A " + id_loc_df.DOMES_N.values + " P " + location + id_loc_df.LOC.values + "\n"
+    ).tolist()
+
+    rec_str_list = (
+        " "
+        + rec_df.CODE
+        + "  A ---- P "
+        + rec_df.BEGIN_SNX
+        + " "
+        + rec_df.END_SNX
+        + " "
+        + +rec_df.RECEIVER.str.ljust(20, " ")
+        + " "
+        + rec_df["S/N"].str.ljust(5, " ")
+        + " "
+        + rec_df.FW
+        + "\n"
+    ).to_list()
+
+    ant_str_list = (
+        " "
+        + ant_df.CODE
+        + "  A ---- P "
+        + ant_df.BEGIN_SNX
+        + " "
+        + ant_df.END_SNX
+        + " "
+        + ant_df.ANTENNA
+        + " "
+        + ant_df.RADOME
+        + " "
+        + ant_df["S/N"]
+        + "\n"
+    ).to_list()
+
+    ecc_str_list = (
+        " "
+        + ant_df.CODE
+        + "  A ---- P "
+        + ant_df.BEGIN_SNX
+        + " "
+        + ant_df.END_SNX
+        + " UNE "
+        + ant_df.EccU
+        + " "
+        + ant_df.EccN
+        + " "
+        + ant_df.EccE
+        + "\n"
+    ).to_list()
 
     buf = (
-      ['*-------------------------------------------------------------------------------\n']
-    + ['+SITE/ID\n']
-    + ['*CODE PT __DOMES__ T _STATION DESCRIPTION__ APPROX_LON_ APPROX_LAT_ _APP_H_\n']
-    + id_str_list + ['-SITE/ID\n']
-
-    + ['*-------------------------------------------------------------------------------\n']
-    + ['+SITE/RECEIVER\n']
-    + ['*SITE PT SOLN T DATA_START__ DATA_END____ DESCRIPTION_________ S/N__ FIRMWARE___\n']
-    + rec_str_list + ['-SITE/RECEIVER\n']
-
-    + ['*-------------------------------------------------------------------------------\n']
-    + ['+SITE/ANTENNA\n' ]
-    + ['*SITE PT SOLN T DATA_START__ DATA_END____ DESCRIPTION_________ S/N__\n']
-    + ant_str_list + ['-SITE/ANTENNA\n' ]
-
-    + ['*-------------------------------------------------------------------------------\n']
-    + ['+SITE/ECCENTRICITY\n']
-    + ['*SITE PT SOLN T DATA_START__ DATA_END____ AXE UP______ NORTH___ EAST____\n']
-    + ecc_str_list + ['-SITE/ECCENTRICITY\n'])
+        ["*-------------------------------------------------------------------------------\n"]
+        + ["+SITE/ID\n"]
+        + ["*CODE PT __DOMES__ T _STATION DESCRIPTION__ APPROX_LON_ APPROX_LAT_ _APP_H_\n"]
+        + id_str_list
+        + ["-SITE/ID\n"]
+        + ["*-------------------------------------------------------------------------------\n"]
+        + ["+SITE/RECEIVER\n"]
+        + ["*SITE PT SOLN T DATA_START__ DATA_END____ DESCRIPTION_________ S/N__ FIRMWARE___\n"]
+        + rec_str_list
+        + ["-SITE/RECEIVER\n"]
+        + ["*-------------------------------------------------------------------------------\n"]
+        + ["+SITE/ANTENNA\n"]
+        + ["*SITE PT SOLN T DATA_START__ DATA_END____ DESCRIPTION_________ S/N__\n"]
+        + ant_str_list
+        + ["-SITE/ANTENNA\n"]
+        + ["*-------------------------------------------------------------------------------\n"]
+        + ["+SITE/ECCENTRICITY\n"]
+        + ["*SITE PT SOLN T DATA_START__ DATA_END____ AXE UP______ NORTH___ EAST____\n"]
+        + ecc_str_list
+        + ["-SITE/ECCENTRICITY\n"]
+    )
 
     return buf
 
-def write_meta_gather_master(logs_glob_path='/data/station_logs/*/*.log',
-                             rnx_glob_path='/data/acs/pea/proc/exs/data/*.rnx',
-                             frame_datetime=None,
-                             frame_snx_path='/data/ITRF/itrf2014/ITRF2014-IGS-TRF.SNX.gz',
-                             frame_soln_path='/data/ITRF/itrf2014/ITRF2014-soln-gnss.snx',
-                             frame_psd_path='/data/ITRF/itrf2014/ITRF2014-psd-gnss.snx',
-                             out_path = '/data/meta_gather.snx',
-                             num_threads = None):
 
+def write_meta_gather_master(
+    logs_glob_path="/data/station_logs/*/*.log",
+    rnx_glob_path="/data/acs/pea/proc/exs/data/*.rnx",
+    frame_datetime=None,
+    frame_snx_path="/data/ITRF/itrf2014/ITRF2014-IGS-TRF.SNX.gz",
+    frame_soln_path="/data/ITRF/itrf2014/ITRF2014-soln-gnss.snx",
+    frame_psd_path="/data/ITRF/itrf2014/ITRF2014-psd-gnss.snx",
+    out_path="/data/meta_gather.snx",
+    num_threads=None,
+):
     if frame_datetime is None:
-        frame_datetime = _np.datetime64('today')
-    else: frame_datetime =_np.datetime64(frame_datetime)
+        frame_datetime = _np.datetime64("today")
+    else:
+        frame_datetime = _np.datetime64(frame_datetime)
 
-    id_loc_df, rec_df, ant_df = gather_metadata(logs_glob_path=logs_glob_path,
-                                                rnx_glob_path=rnx_glob_path,
-                                                num_threads=num_threads)
+    id_loc_df, rec_df, ant_df = gather_metadata(
+        logs_glob_path=logs_glob_path, rnx_glob_path=rnx_glob_path, num_threads=num_threads
+    )
 
     sites_meta = rec_df.CODE.unique()
 
     gather_itrf = None
     if (frame_snx_path is not None) and (frame_soln_path is not None):
-        gather_itrf = _gn_frame.get_frame_of_day(frame_datetime,
-                        itrf_path_or_df=frame_snx_path,
-                        list_path_or_df=sites_meta,
-                        discon_path_or_df = frame_soln_path,
-                        psd_path_or_df    = frame_psd_path)
-
+        gather_itrf = _gn_frame.get_frame_of_day(
+            frame_datetime,
+            itrf_path_or_df=frame_snx_path,
+            list_path_or_df=sites_meta,
+            discon_path_or_df=frame_soln_path,
+            psd_path_or_df=frame_psd_path,
+        )
 
     buf = []
-    #gen header
-    gather_dt = _gn_datetime.datetime2yydoysec(frame_datetime)
-    trf_header = ''
+    # gen header
+    gather_dt = _gn_datetime.datetime2yydoysec(frame_datetime)[0]
+    trf_header = ""
     if gather_itrf is not None:
         trf_header += (
-            f'of which {gather_itrf.shape[0]} were projected to {frame_datetime} using:\n'
-            +f'Frame: {frame_snx_path}\n'
-            +f'Discon:{frame_soln_path}\n'
-            +f'PSD:   {frame_psd_path}\n')
-
-
-    buf.extend([f'%=SNX 2.01 IGS {gather_dt} IGS 00:000:00000 00:000:00000 P 00000 0\n'
-            +'+FILE/REFERENCE\n'
-            +'DESCRIPTION        merged metadata\n'
-            +'OUTPUT             historical sinex header file\n'
-            +'CONTACT            bogdan.matviichuk@ga.gov.au\n'
-            +'SOFTWARE           LOG2SNX v0.1.2\n'
-            +'HARDWARE           AWS\n'
-            +'INPUT              igs ftp site logs\n'
-            +'-FILE/REFERENCE\n'
-            +'+FILE/COMMENT\n'
-            +f'Metadata extracted from {sites_meta.shape[0]} station logs\n'
+            f"of which {gather_itrf.shape[0]} were projected to {frame_datetime} using:\n"
+            + f"Frame: {frame_snx_path}\n"
+            + f"Discon:{frame_soln_path}\n"
+            + f"PSD:   {frame_psd_path}\n"
+        )
+
+    buf.extend(
+        [
+            f"%=SNX 2.01 IGS {gather_dt} IGS 00:000:00000 00:000:00000 P 00000 0\n"
+            + "+FILE/REFERENCE\n"
+            + "DESCRIPTION        merged metadata\n"
+            + "OUTPUT             historical sinex header file\n"
+            + "CONTACT            bogdan.matviichuk@ga.gov.au\n"
+            + "SOFTWARE           LOG2SNX v0.1.2\n"
+            + "HARDWARE           AWS\n"
+            + "INPUT              igs ftp site logs\n"
+            + "-FILE/REFERENCE\n"
+            + "+FILE/COMMENT\n"
+            + f"Metadata extracted from {sites_meta.shape[0]} station logs\n"
             + trf_header
-            +'-FILE/COMMENT\n'
-            +'+INPUT/ACKNOWLEDGMENTS\n'
-            +'IGS International GNSS Service, GA\n'
-            +'-INPUT/ACKNOWLEDGMENTS\n'])
-    #ant/rec
-    buf.extend(meta2sting(id_loc_df,rec_df,ant_df))
-    #projected coordinates
+            + "-FILE/COMMENT\n"
+            + "+INPUT/ACKNOWLEDGMENTS\n"
+            + "IGS International GNSS Service, GA\n"
+            + "-INPUT/ACKNOWLEDGMENTS\n"
+        ]
+    )
+    # ant/rec
+    buf.extend(meta2sting(id_loc_df, rec_df, ant_df))
+    # projected coordinates
     if gather_itrf is not None:
         buf.extend(frame2snx_string(gather_itrf))
-    buf.extend([f'%ENDSNX\n'])
+    buf.extend([f"%ENDSNX\n"])
 
-    with open(out_path,'w') as file:
-        file.write(''.join(buf))
+    with open(out_path, "w") as file:
+        file.write("".join(buf))
```

### Comparing `gnssanalysis-0.0.9/gnssanalysis/gn_io/ionex.py` & `gnssanalysis-0.54/gnssanalysis/gn_io/ionex.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,73 +1,78 @@
 import re as _re
+import logging as _logging
 
 import numpy as _np
 import pandas as _pd
 
-from gnssanalysis import gn_io as _gn_io
-from gnssanalysis import gn_datetime as _gn_datetime
+from .. import gn_datetime as _gn_datetime
+from .. import gn_io as _gn_io
 
-_RE_BLKS= _re.compile(rb'H\n((?:[ \-\d]+\n)+)',_re.MULTILINE)
+_RE_IONEX_BLK = _re.compile(rb"H\n((?:[ \-\d]+\n)+)", _re.MULTILINE)
 
-def gen_range(head,param_name):
-    '''Extracts a group of three parameters as "LAT1 / LAT2 / DLAT" and constructs a range'''
+
+def gen_range(head, param_name):
+    """Extracts a group of three parameters as "LAT1 / LAT2 / DLAT" and constructs a range"""
     head_lon = head.find(param_name)
-    head_lon_lineb = head[:head.find(param_name)].rfind(b'\n') + 1
+    head_lon_lineb = head[: head.find(param_name)].rfind(b"\n") + 1
     lon1, lon2, dlon = head[head_lon_lineb:head_lon].split()
-    lon1 = float(lon1); lon2 = float(lon2); dlon = float(dlon)
-    return _np.arange(lon1,lon2+(0.1 if dlon>0 else -0.1),dlon)
+    lon1, lon2, dlon = float(lon1), float(lon2), float(dlon)
+    return _np.arange(lon1, lon2 + (0.1 if dlon > 0 else -0.1), dlon)
+
 
-def get_param(head,param_name):
-    '''Extracts single parameter (first) from the header'''
+def get_param(head, param_name):
+    """Extracts single parameter (first) from the header"""
     param_loc = head.find(param_name)
-    param_line_begin = head[:head.find(param_name)].rfind(b'\n') + 1
+    param_line_begin = head[: head.find(param_name)].rfind(b"\n") + 1
     return float(head[param_line_begin:param_loc].split()[0])
 
+
 def read_ionex(path_or_bytes):
-    '''Exponent is extracted into dataframe attribute'''
+    """Exponent is extracted into dataframe attribute"""
     data = _gn_io.common.path2bytes(path_or_bytes)
-    end_of_head = data.find(b'END OF HEADER') + 13
+    end_of_head = data.find(b"END OF HEADER")
+    if end_of_head == -1:
+        raise ValueError ('IONEX header missing')
+    end_of_head += 13
 
     head = data[:end_of_head]
     data = data[end_of_head:]
 
-    maps_heads = find_all(data,b'START',window=[9,60]) # type + epoch info
-    maps_heads_arr = _np.asarray(b''.join(maps_heads).split()).reshape(len(maps_heads),-1)
+    maps_heads = find_all(data, b"START", window=[9, 60])  # type + epoch info
+    if not maps_heads:
+        raise ValueError ('IONEX maps not found')
+    maps_heads_arr = _np.asarray(b"".join(maps_heads).split()).reshape(len(maps_heads), -1)
     # return maps_heads
-    datetime = strdatetime2datetime(maps_heads_arr[:,2:],as_j2000=True)
-    maps_type = maps_heads_arr[:,0].astype(str)
+    datetime = _gn_datetime.strdatetime2datetime(maps_heads_arr[:, 2:], as_j2000=True)
+    maps_type = maps_heads_arr[:, 0].astype(str)
 
-    exp = get_param(head,b'EXPONENT')
-    
-    maps_arr = _np.asarray(b''.join(_RE_BLKS.findall(data)).replace(b'\n',b''))[_np.newaxis].view('S5').astype(int) * 10**exp
-
-    lon_arr = gen_range(head,b'LON1 ')
-    lat_arr = gen_range(head,b'LAT1 ')
-    df = _pd.DataFrame(data  = maps_arr.reshape(-1,lon_arr.shape[0]),
-                         index = [_np.repeat(datetime,lat_arr.shape[0]),_np.repeat(maps_type,lat_arr.shape[0]),_np.tile(lat_arr,maps_type.shape[0])],
-                         columns = lon_arr)
-    df.index.names = ['DateTime','Type','Lat'] #for convenience + nice to have in the diff util output
-    df.columns.names = ['Lon']
-    df.attrs['EXPONENT'] = exp
+    exp = get_param(head, b"EXPONENT")
+
+    maps_arr = (
+        _np.asarray(b"".join(_RE_IONEX_BLK.findall(data)).replace(b"\n", b""))[_np.newaxis].view("S5").astype(int)
+        * 10**exp
+    )
+
+    lon_arr = gen_range(head, b"LON1 ")
+    lat_arr = gen_range(head, b"LAT1 ")
+    df = _pd.DataFrame(
+        data=maps_arr.reshape(-1, lon_arr.shape[0]),
+        index=[
+            _np.repeat(datetime, lat_arr.shape[0]),
+            _np.repeat(maps_type, lat_arr.shape[0]),
+            _np.tile(lat_arr, maps_type.shape[0]),
+        ],
+        columns=lon_arr,
+    )
+    df.index.names = ["DateTime", "Type", "Lat"]  # for convenience + nice to have in the diff util output
+    df.columns.names = ["Lon"]
+    df.attrs["EXPONENT"] = exp
     return df
 
-def find_all(data,pat,window):
+
+def find_all(data, pat, window):
     buf = []
     find = data.find(pat)
-    while find!=-1:
-        buf.append(data[find+window[0]:find+window[1]])
-        find = data.find(pat,find+len(pat))
+    while find != -1:
+        buf.append(data[find + window[0] : find + window[1]])
+        find = data.find(pat, find + len(pat))
     return buf
-
-def strdatetime2datetime(dt_arr, as_j2000=True):
-    '''ndarray of Y M D h m s to datetime64'''
-    datetime = (dt_arr[:,0].astype('datetime64[M]') 
-    + (dt_arr[:,1].astype('timedelta64[M]') - 1) 
-    + (dt_arr[:,2].astype('timedelta64[D]') - 1)
-
-    + (dt_arr[:,3].astype('timedelta64[h]'))
-    + (dt_arr[:,4].astype('timedelta64[m]'))
-    + (dt_arr[:,5].astype('timedelta64[s]')))
-
-    if as_j2000:
-        return _gn_datetime.datetime2j2000(datetime)
-    return datetime
```

### Comparing `gnssanalysis-0.0.9/gnssanalysis/gn_io/pea.py` & `gnssanalysis-0.54/gnssanalysis/gn_io/pea.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 from io import BytesIO as _BytesIO
 
 import pandas as _pd
-from gnssanalysis import gn_const as _gn_const
-from gnssanalysis import gn_datetime as _gn_datetime
-from gnssanalysis import gn_io as _gn_io
+
+from .. import gn_const as _gn_const
+from .. import gn_datetime as _gn_datetime
+from .. import gn_io as _gn_io
 
 
 def read_pea_partials(path):
     partials = _gn_io.common.path2bytes(path)
     begin = partials.find(b"End_of_Header") + 13
-    df = _pd.read_csv(_BytesIO(partials[begin:]),header=None,delim_whitespace=True,usecols=[0,1,2,9,10,11],names=[None,'MJD','TOD','X','Y','Z'])
-    df_done = df[['X','Y','Z']].set_index([_gn_datetime.mjd2j2000(df.MJD.values,df.TOD.values,pea_partials=True),df.iloc[:,0].astype(_gn_const.PRN_CATEGORY)])
-    df_partials = _pd.concat([df_done],keys=['EST'],axis=1)/1000
-    df_partials.attrs['path'] = path
+    df = _pd.read_csv(
+        _BytesIO(partials[begin:]),
+        header=None,
+        delim_whitespace=True,
+        usecols=[0, 1, 2, 9, 10, 11],
+        names=[None, "MJD", "TOD", "X", "Y", "Z"],
+    )
+    df_done = df[["X", "Y", "Z"]].set_index(
+        [_gn_datetime.mjd2j2000(df.MJD.values, df.TOD.values, pea_partials=True), df.iloc[:, 0]]
+    )
+    df_partials = _pd.concat([df_done], keys=["EST"], axis=1) / 1000
+    df_partials.attrs["path"] = path
     return df_partials
```

### Comparing `gnssanalysis-0.0.9/gnssanalysis/gn_io/pod.py` & `gnssanalysis-0.54/gnssanalysis/gn_io/pod.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import re as _re
 
 import numpy as _np
 import pandas as _pd
 
-from gnssanalysis import gn_const as _gn_const
-from gnssanalysis import gn_io as _gn_io
+from .. import gn_const as _gn_const
+from .. import gn_io as _gn_io
 
 _POD_ITRF_RMS = _re.compile(r"RMS-XYZ ITRF CMP[ ]*([A-Z\d]+)[ ]+([\d\.]+)[ ]+([\d\.]+)[ ]+([\d\.]+)")
 
-def pod_get_IC_dt(pod_out:bytes)->int:
+
+def pod_get_IC_dt(pod_out: bytes) -> int:
     begin = pod_out.find(b"IC Epoch:") + 9
-    end = pod_out.find(b"\n",begin)
+    end = pod_out.find(b"\n", begin)
     date = _pd.Series(pod_out[begin:end].strip().decode()).str.split(pat=r"\s+")
-    year,month,day,frac = date.tolist()[0]
-    dt_value = (_np.datetime64('-'.join([year,month.zfill(2),day])) - _gn_const.J2000_ORIGIN).astype(int) 
-    return dt_value + int(86400*float(frac))
+    year, month, day, frac = date.tolist()[0]
+    dt_value = (_np.datetime64("-".join([year, month.zfill(2), day])) - _gn_const.J2000_ORIGIN).astype(int)
+    return dt_value + int(86400 * float(frac))
+
 
 def read_pod_out(path):
     """reads pod.out file. No SV categories implemented as file is small"""
     content = _gn_io.common.path2bytes(path)
     df = _pd.DataFrame(
-        data=_POD_ITRF_RMS.findall(content.decode()), #working with string not bytes
-        columns=['SV','X','Y','Z']
-        )
-    return df.set_index([[pod_get_IC_dt(content)]*df.shape[0],'SV']).astype(float)
-
+        data=_POD_ITRF_RMS.findall(content.decode()), columns=["SV", "X", "Y", "Z"]  # working with string not bytes
+    )
+    return df.set_index([[pod_get_IC_dt(content)] * df.shape[0], "SV"]).astype(float)
```

### Comparing `gnssanalysis-0.0.9/gnssanalysis/gn_io/stec.py` & `gnssanalysis-0.54/gnssanalysis/gn_io/stec.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 from io import BytesIO as _BytesIO
 
 import pandas as _pd
-from gnssanalysis import gn_const as _gn_const
-from gnssanalysis import gn_datetime as _gn_datetime
-from gnssanalysis import gn_io as _gn_io
+
+from .. import gn_const as _gn_const
+from .. import gn_datetime as _gn_datetime
+from .. import gn_io as _gn_io
 
 
 def read_stec(path_or_bytes):
-    stec = _pd.read_csv(_BytesIO(_gn_io.common.path2bytes(path_or_bytes)),comment='#',header=None,usecols=[1,2,3,4,5,6,7],names=['WEEK','TOW','SITE','SAT','VAL','VAR','LAYER'], # type:ignore
-    dtype={1:int,2:int,3:object,4:_gn_const.PRN_CATEGORY,5:float,6:float,7:int}) # type:ignore
-    datetime = _gn_datetime.gpsweeksec2datetime(stec.WEEK.values,stec.TOW.values,as_j2000=True)
-    return stec.drop(columns=['WEEK','TOW']).set_index([datetime,'SITE','SAT','LAYER'])
+    stec = _pd.read_csv(
+        _BytesIO(_gn_io.common.path2bytes(path_or_bytes)),
+        comment="#",
+        header=None,
+        usecols=[1, 2, 3, 4, 5, 6, 8],
+        names=["WEEK", "TOW", "SITE", "SAT", "VAL", "VAR", "LAYER"],  # type:ignore
+        dtype={1: int, 2: int, 3: object, 4: object, 5: float, 6: float, 8: int},
+    )  # type:ignore
+    datetime = _gn_datetime.gpsweeksec2datetime(stec.WEEK.values, stec.TOW.values, as_j2000=True)
+    return stec.drop(columns=["WEEK", "TOW"]).set_index([datetime, "SITE", "SAT", "LAYER"])
```

### Comparing `gnssanalysis-0.0.9/gnssanalysis/gn_io/trace.py` & `gnssanalysis-0.54/gnssanalysis/gn_io/trace.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,136 +1,187 @@
-'''TRACE file parser. Note the separate functions for values and residuals'''
+"""TRACE file parser. Note the separate functions for values and residuals"""
 import logging as _logging
 import os as _os
 import re as _re
 from io import BytesIO as _BytesIO
 
-import numpy as _np
 import pandas as _pd
 
-from gnssanalysis import gn_const as _gn_const
-from gnssanalysis import gn_datetime as _gn_datetime
-from gnssanalysis import gn_io as _gn_io
-from gnssanalysis import gn_aux as _gn_aux
+from .. import gn_aux as _gn_aux
+from .. import gn_const as _gn_const
+from .. import gn_datetime as _gn_datetime
+from .. import gn_io as _gn_io
 
 
-def _trace_extract(path_or_bytes,blk_name):
-    trace_bytes = _gn_io.common.path2bytes(path_or_bytes) #path2bytes passes through bytes 
+def _trace_extract(path_or_bytes, blk_name):
+    trace_bytes = _gn_io.common.path2bytes(path_or_bytes)  # path2bytes passes through bytes
 
     begin = end = 0
-    buf=[]
+    buf = []
 
-    blk_begin = (f'+{blk_name}').encode()
-    blk_end   = (f'-{blk_name}').encode()
+    blk_begin = (f"+{blk_name}").encode()
+    blk_end = (f"-{blk_name}").encode()
 
     while True:
-        begin = trace_bytes.find(blk_begin,end)
-        begin_full =  trace_bytes.find(b'\n',begin)
-        if begin==-1:
+        begin = trace_bytes.find(blk_begin, end)
+        begin_full = trace_bytes.find(b"\n", begin)
+        if begin == -1:
             break
-        end = trace_bytes.find(blk_end,begin_full)
+        end = trace_bytes.find(blk_end, begin_full)
 
-        blk_content = trace_bytes[begin_full+1:end]         # needs +1 not to start with '\n'
-        blk_type = b'\t' + trace_bytes[begin+1:begin_full] + b'\n'	# needs +2 to remove ' +'
+        blk_content = trace_bytes[begin_full + 1 : end]  # needs +1 not to start with '\n'
+        blk_type = b"\t" + trace_bytes[begin + 1 : begin_full] + b"\n"  # needs +2 to remove ' +'
         blk_content_w_type = blk_type.join(blk_content.splitlines()) + blk_type
         buf.append(blk_content_w_type)
 
-    content = b''.join(buf)
+    content = b"".join(buf)
     if len(content) == 0:
         _logging.error(f'"{blk_name}" data not found')
         return None
     return content
 
-def _read_trace_states(path_or_bytes):
-    states = _trace_extract(path_or_bytes,blk_name='STATES')
+
+def _read_trace_states(path_or_bytes, throw_if_nans=False):
+    states = _trace_extract(path_or_bytes, blk_name="STATES")
+
     if states is None:
         return None
-    df = _pd.read_csv(_BytesIO(states),delimiter='\t',usecols=[1,2,3,4,5,6,7,8,10],skipinitialspace=True,dtype={'SAT':_gn_const.PRN_CATEGORY,'TYPE':_gn_const.STATE_TYPES_CATEGORY},keep_default_na=False,
-                    comment='#',header=None,names = ['TIME','TYPE','SITE','SAT','NUM','EST','VAR','ADJ','BLK'],parse_dates=['TIME']) # type:ignore
+    
+    if throw_if_nans:
+        _gn_aux.throw_if_nans(states)
+    
+    df = _pd.read_csv(
+        _BytesIO(states),
+        delimiter="\t",
+        usecols=[1, 2, 3, 4, 5, 6, 7, 8, 10],
+        skipinitialspace=True,
+        comment="#",
+        header=None,
+        names=["TIME", "TYPE", "SITE", "SAT", "NUM", "EST", "VAR", "ADJ", "BLK"],
+        dtype={
+            "TYPE": object,
+            "SITE": object,
+            "SAT": object,
+            "NUM": int,
+            "EST": float,
+            "VAR": float,
+            "ADJ": float,
+            "BLK": object,
+        },
+        parse_dates=["TIME"],
+    )
 
     if df.size == 0:
         _logging.error("STATES* blocks present but empty")
         return None
 
     df.TIME = _gn_datetime.datetime2j2000(df.TIME.values)
 
-    empty_mask = df.TYPE.values.notna() # dropping ONE type
-    if (~empty_mask).sum()>0:
+    empty_mask = df.TYPE.notna()  # dropping ONE type
+    if (~empty_mask).sum() > 0:
         df = df[empty_mask]
 
-    return df.set_index(['TIME','SITE','TYPE','SAT','NUM','BLK'])
+    return df.set_index(["TIME", "SITE", "TYPE", "SAT", "NUM", "BLK"])
+
+
+def _read_trace_residuals(path_or_bytes, it_max_only=True, throw_if_nans=False):
+    residuals = _trace_extract(path_or_bytes, blk_name="RESIDUALS")
 
-def _read_trace_residuals(path_or_bytes,it_max_only=True):
-    residuals = _trace_extract(path_or_bytes,blk_name='RESIDUALS')
     if residuals is None:
         return None
+    
+    if throw_if_nans:
+        _gn_aux.throw_if_nans(residuals)
 
-    df = _pd.read_csv(_BytesIO(residuals),delimiter='\t',comment='#',header=None,usecols=[1,2,3,4,5,6,7,8,9,10],skipinitialspace=True,keep_default_na=False,
-            names = ['It','TIME','TYPE','SAT','SITE','NUM','PREFIT','POSTFIT','STD','BLK'],parse_dates=['TIME'],dtype={'It':int,'NUM':int,'SAT':_gn_const.PRN_CATEGORY}) # type:ignore
-    if df.size == 0: # blocks are present bu empty
+    df = _pd.read_csv(
+        _BytesIO(residuals),
+        delimiter="\t",
+        comment="#",
+        header=None,
+        usecols=[1, 2, 3, 4, 5, 6, 7, 8, 9, 11],
+        skipinitialspace=True,
+        na_values="NONE",
+        names=["It", "TIME", "TYPE", "SAT", "SITE", "NUM", "PREFIT", "POSTFIT", "STD", "BLK"],
+        dtype={
+            "It": int,
+            "TYPE": object,
+            "SAT": object,
+            "SITE": object,
+            "NUM": int,
+            "PREFIT": float,
+            "POSTFIT": float,
+            "STD": float,
+            "BLK": object,
+        },
+        parse_dates=["TIME"],
+    )
+    if df.empty:  # blocks are present but empty
         _logging.error("RESIDUALS* blocks present but empty")
         return None
 
     df.TIME = _gn_datetime.datetime2j2000(df.TIME.values)
 
-    empty_mask = df.SITE.values.astype(bool) # may be removed in the future when the pivot is removed from PEA
-    if (~empty_mask).sum()>0:
-        df = df[empty_mask]
-        
     if not it_max_only:
-        return df.set_index(['TIME','SITE','TYPE','NUM','SAT','BLK'])
+        return df.set_index(["TIME", "SITE", "TYPE", "NUM", "SAT", "BLK"])
     # to get max_ind values pandas >= 1.1 is required
-    it_max_ind=df[['TIME','It']].groupby(['TIME']).max().reset_index().values.tolist()
-    return df.set_index(['TIME','It']).loc[it_max_ind].reset_index().set_index(['TIME','SITE','TYPE','SAT','NUM','BLK'])
-
+    it_max_ind = df[["TIME", "It"]].groupby(["TIME"]).max().reset_index().values.tolist()
+    return (
+        df.set_index(["TIME", "It"])
+        .loc[it_max_ind]
+        .reset_index()
+        .set_index(["TIME", "SITE", "TYPE", "SAT", "NUM", "It", "BLK"])
+    )
 
 
 _RE_TRACE_HEAD = _re.compile(
-    rb'station\s*\:\s*(.{4})\n\w+\s*\:\s*(.+|)\n\w+\s*\:\s*(.+|)\n\w+\s*\:\s*(\d)\n\w+\s*\:\s*(.+)')
-_RE_TRACE_LC = _re.compile(rb'PDE\sform\sLC.+((?:\n.+)+)')
-_RE_EL = _re.compile(rb'\*2 PDE-CS GPST\s+\w+\s+(\d+)\s+(\d+).0\s+(\w\d\d)\s+(\d+.\d+)')
+    rb"station\s*\:\s*(.{4})\n\w+\s*\:\s*(.+|)\n\w+\s*\:\s*(.+|)\n\w+\s*\:\s*(\d)\n\w+\s*\:\s*(.+)"
+)
+_RE_TRACE_LC = _re.compile(rb"PDE\sform\sLC.+((?:\n.+)+)")
+_RE_EL = _re.compile(rb"\*2 PDE-CS GPST\s+\w+\s+(\d+)\s+(\d+).0\s+(\w\d\d)\s+(\d+.\d+)")
+
 
 def _find_trace(output_path: str) -> tuple:
-    '''Scans output path for TRACE files'''
+    """Scans output path for TRACE files"""
     station_names = set()
     trace_paths = []
-    _re_station_name = _re.compile(r'\-(.{4})\d+.TRACE')
+    _re_station_name = _re.compile(r"\-(.{4})\d+.TRACE")
 
     for file in _os.scandir(path=output_path):
-        if file.path.endswith('TRACE'):
+        if file.path.endswith("TRACE"):
             station_names.add(_re_station_name.findall(file.path)[0])
             trace_paths.append(file.path)
 
     station_names = sorted(station_names)
     trace_paths = sorted(trace_paths)
     return station_names, trace_paths
 
+
 # def _read_trace_LC(path_or_bytes):
 #     '''Parses the LC combo block of the trace files producing
-#      a single dataframe. WORK-IN-PROGRESS'''    
+#      a single dataframe. WORK-IN-PROGRESS'''
 #     # regex search string
 #     if isinstance(path_or_bytes, str):
 #         trace_content = _gn_io.common.path2bytes(path_or_bytes) # will accept .trace.Z also
 #     else:
 #         trace_content = path_or_bytes
 #     trace_LC_list = _RE_TRACE_LC.findall(string=trace_content)
 #     LC_bytes = b''.join(trace_LC_list)
 #     LC_bytes = LC_bytes.replace(b'=',b'') #getting rif of '='
-    
+
 #     df_LC = _pd.read_csv(_BytesIO(LC_bytes),delim_whitespace=True,header=None,usecols=[1,2,4,6,8,9,10,11,12,13]).astype(
 #         {
 #             1: _np.int16, 2:_np.int32, 4: '<U3',
 #             6: '<U1', 8: '<U4',
 #             9: _np.float_, 10: '<U4', 11: _np.float_,
 #             12: '<U4', 13: _np.float_
 #         })
-    
+
 #     df_LC.columns = ['W','S','PRN','LP',8,9,10,11,12,13]
-#     df_LC['time'] = _gn_datetime.gpsweeksec2datetime(gps_week = df_LC.W, 
-#                                                 tow = df_LC.S, 
+#     df_LC['time'] = _gn_datetime.gpsweeksec2datetime(gps_week = df_LC.W,
+#                                                 tow = df_LC.S,
 #                                                 as_j2000=True)
 #     df_LC.drop(columns=['W','S'],inplace=True)
 
 #     df1 = df_LC[['time','PRN','LP',8,9]]
 #     df1.columns = ['time','PRN','LP','combo','value']
 
 #     df2 = df_LC[['time','PRN','LP',10,11]]
@@ -145,55 +196,61 @@
 # def _read_trace_el(path_or_bytes):
 #     "Get elevation angles for satellites from trace file"
 #     if isinstance(path_or_bytes, str):
 #         trace_content = _gn_io.common.path2bytes(path_or_bytes) # will accept .trace.Z also
 #     else:
 #         trace_content = path_or_bytes
 #     trace_EL_list = _RE_EL.findall(string=trace_content)
-    
+
 #     el_df = _pd.DataFrame(trace_EL_list).astype({0:_np.int16, 1:_np.int32, 2:bytes, 3:_np.float})
 #     el_df[2] = el_df[2].str.decode("utf-8")
 #     el_df['time'] = _gn_datetime.gpsweeksec2datetime(gps_week=el_df[0], tow=el_df[1], as_j2000=True)
 #     el_df.drop(columns=[0,1],inplace=True)
 #     el_df.columns = ['PRN','el','time']
 #     return el_df.set_index(['time'])
 
 
 def squeeze_column_names(df, delimiter=None):
     cols_frame = df.columns.to_frame(index=None).astype(str)
     if delimiter is not None:
-        cols_frame.iloc[:,:-1]+=delimiter
+        cols_frame.iloc[:, :-1] += delimiter
     df.columns = cols_frame.sum(axis=1)
 
-def states2eda(states_df:_pd.DataFrame):
-    df = states_df.rename(columns = {'EST':'x','VAR':'P','ADJ':'dx'})
-    states_mask = _gn_aux.df_quick_select(df, 'BLK', 'STATES',as_mask=True)
+
+def states2eda(states_df: _pd.DataFrame):
+    df = states_df.rename(columns={"EST": "x", "VAR": "P", "ADJ": "dx"})
+    states_mask = _gn_aux.df_quick_select(df, "BLK", "STATES", as_mask=True)
     eda_records = []
     if states_mask is not None:
-        pos_trop_mask = _gn_aux.df_quick_select(df, 'TYPE',['REC_POS','TROP'],as_mask=True)
+        pos_trop_mask = _gn_aux.df_quick_select(df, "TYPE", ["REC_POS", "TROP"], as_mask=True)
         if pos_trop_mask is not None:
-            df_pos_trop = df[states_mask & pos_trop_mask].unstack('NUM')
+            df_pos_trop = df[states_mask & pos_trop_mask].unstack("NUM")
             squeeze_column_names(df_pos_trop)
-            df_pos_trop.reset_index(level=['SITE','TYPE','TIME'], inplace=True)
+            df_pos_trop.reset_index(level=["SITE", "TYPE", "TIME"], inplace=True)
             df_pos_trop.TIME = _gn_datetime.j20002datetime(df_pos_trop.TIME.values, as_datetime=True)
-            df_pos_trop.rename(columns={'TYPE':'States','Site':'Site','TIME':'Epoch'})
-            eda_records += df_pos_trop.to_dict('records')
+            df_pos_trop.rename(columns={"TYPE": "States", "Site": "Site", "TIME": "Epoch"})
+            eda_records += df_pos_trop.to_dict("records")
 
-        rclk_mask = _gn_aux.df_quick_select(df, 'TYPE','REC_CLOCK',as_mask=True)
+        rclk_mask = _gn_aux.df_quick_select(df, "TYPE", "REC_CLOCK", as_mask=True)
         if rclk_mask is not None:
-            df_rclk = df[states_mask & rclk_mask].unstack('NUM')
+            df_rclk = df[states_mask & rclk_mask].unstack("NUM")
             squeeze_column_names(df_rclk)
-            df_rclk.reset_index(level=['SITE','TYPE','TIME'], inplace=True)
+            df_rclk.reset_index(level=["SITE", "TYPE", "TIME"], inplace=True)
             df_rclk.TIME = _gn_datetime.j20002datetime(df_rclk.TIME.values, as_datetime=True)
-            df_rclk.rename(columns={'TYPE':'States','Site':'Site','TIME':'Epoch'})
-            eda_records += df_rclk.to_dict('records')
+            df_rclk.rename(columns={"TYPE": "States", "Site": "Site", "TIME": "Epoch"})
+            eda_records += df_rclk.to_dict("records")
 
     return eda_records
 
-def residuals2eda(residuals_df:_pd.DataFrame):
+
+def residuals2eda(residuals_df: _pd.DataFrame):
     """ """
-    b = residuals_df.drop(columns='It').rename(columns={'PREFIT':'Prefit','POSTFIT':'Postfit','STD':'Variance'}).unstack(['TYPE','NUM'])
-    squeeze_column_names(b, delimiter='-')
+    b = (
+        residuals_df.drop(columns="It")
+        .rename(columns={"PREFIT": "Prefit", "POSTFIT": "Postfit", "STD": "Variance"})
+        .unstack(["TYPE", "NUM"])
+    )
+    squeeze_column_names(b, delimiter="-")
 
-    b.reset_index(['TIME','SITE','SAT'],inplace=True)
+    b.reset_index(["TIME", "SITE", "SAT"], inplace=True)
     b.TIME = _gn_datetime.j20002datetime(b.TIME.values, as_datetime=True)
-    return b.rename(columns={'TIME':'Epoch','SITE':'Site','SAT':'Sat'}).to_dict('records')
+    return b.rename(columns={"TIME": "Epoch", "SITE": "Site", "SAT": "Sat"}).to_dict("records")
```

### Comparing `gnssanalysis-0.0.9/gnssanalysis/gn_io/trop.py` & `gnssanalysis-0.54/gnssanalysis/gn_io/trop.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,49 @@
-'''Trop sinex files reader/parser'''
+"""Trop sinex files reader/parser"""
 from io import BytesIO as _BytesIO
 
 import numpy as _np
 import pandas as _pd
-from gnssanalysis import gn_datetime as _gn_datetime
-from gnssanalysis import gn_io as _gn_io
 from tqdm import tqdm as _tqdm
 
+from .. import gn_datetime as _gn_datetime
+from .. import gn_io as _gn_io
+
 
 def _read_tro_solution(path: str, recenter: bool = True) -> _pd.DataFrame:
-    '''Parses tro snx file into a dataframe.
-    Enabling recenter overrides the default SOD values to 43200 s'''
+    """Parses tro snx file into a dataframe.
+    Enabling recenter overrides the default SOD values to 43200 s"""
     snx_bytes = _gn_io.common.path2bytes(path)
-    tro_estimate = _gn_io._snx_extract_blk(snx_bytes=snx_bytes,blk_name='TROP/SOLUTION',remove_header=True)
+    tro_estimate = _gn_io._snx_extract_blk(snx_bytes=snx_bytes, blk_name="TROP/SOLUTION", remove_header=True)
     if tro_estimate is None:
-        _tqdm.write(f'bounds not found in {path}. Skipping.', end=' | ')
+        _tqdm.write(f"bounds not found in {path}. Skipping.", end=" | ")
         return None
-    tro_estimate = tro_estimate[0] #only single block is in tro so bytes only
+    tro_estimate = tro_estimate[0]  # only single block is in tro so bytes only
 
     try:
-        solution_df = _pd.read_csv(_BytesIO(tro_estimate), delim_whitespace=True,
-                                   comment=b'*', index_col=False, header=None,
-                                   names=['CODE', 'REF_EPOCH',
-                                          2, 3, 4, 5, 6, 7],
-                                   dtype={0: 'category',  1: object,
-                                          2: _np.float_,  3: _np.float32,
-                                          4: _np.float32, 5: _np.float32,
-                                          6: _np.float32, 7: _np.float32, })
+        solution_df = _pd.read_csv(
+            _BytesIO(tro_estimate),
+            delim_whitespace=True,
+            comment=b"*",
+            index_col=False,
+            header=None,
+            names=["CODE", "REF_EPOCH", 2, 3, 4, 5, 6, 7],
+            dtype={
+                0: "category",
+                1: object,
+                2: _np.float_,
+                3: _np.float32,
+                4: _np.float32,
+                5: _np.float32,
+                6: _np.float32,
+                7: _np.float32,
+            },
+        )
     except ValueError as _e:
-        if _e.args[0][:33] == 'could not convert string to float':
-            _tqdm.write(f'{path} data corrupted. Skipping', end=' | ')
+        if _e.args[0][:33] == "could not convert string to float":
+            _tqdm.write(f"{path} data corrupted. Skipping", end=" | ")
             return None
 
-    solution_df.REF_EPOCH = _gn_datetime.yydoysec2datetime(
-        solution_df.REF_EPOCH, recenter=recenter, as_j2000=True)
-    solution_df.set_index(['CODE', 'REF_EPOCH'], inplace=True)
-    solution_df.columns = _pd.MultiIndex.from_product(
-        [['TROTOT', 'TGNTOT', 'TGETOT'], ['VAL', 'STD']])
-    return solution_df
+    solution_df.REF_EPOCH = _gn_datetime.yydoysec2datetime(solution_df.REF_EPOCH, recenter=recenter, as_j2000=True)
+    solution_df.set_index(["CODE", "REF_EPOCH"], inplace=True)
+    solution_df.columns = _pd.MultiIndex.from_product([["TROTOT", "TGNTOT", "TGETOT"], ["VAL", "STD"]])
+    return solution_df
```

### Comparing `gnssanalysis-0.0.9/gnssanalysis/gn_plot.py` & `gnssanalysis-0.54/gnssanalysis/gn_plot.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,126 +1,164 @@
-import os as _os
 import logging as _logging
+import os as _os
 
 import matplotlib.dates as _mdates
 import matplotlib.units as _munits
 import numpy as _np
 import pandas as _pd
 import plotext as plx
 from matplotlib import cm as _cm
 
-from gnssanalysis.gn_const import J2000_ORIGIN as _J2000_ORIGIN
-from gnssanalysis.gn_datetime import j20002datetime as _j20002datetime
+from . import gn_datetime as _gn_datetime
 
 
-def plot_vec(df:_pd.DataFrame, axes:list, axes_idx:list,legend:bool=True):
-    '''Function to plot columnar (single-lvl column names) dataframe to axes list 
-    according to axes index provided (needed in case of non-alphabetic order of column names and axes desired). 
+def plot_vec(df: _pd.DataFrame, axes: list, axes_idx: list, legend: bool = True):
+    """Function to plot columnar (single-lvl column names) dataframe to axes list
+    according to axes index provided (needed in case of non-alphabetic order of column names and axes desired).
     Example snippet below:
 
     fig = plt.figure(figsize=(10,5)
     gs = fig.add_gridspec(3, hspace=0.2)
     ax = gs.subplots(sharex=True, sharey=False)
     plot_vec(axes=ax,df=a,axes_idx=[1,2,0])
-    fig.savefig('blah.png') 
-    '''
+    fig.savefig('blah.png')
+    """
     converter = _mdates.DateConverter()
     _munits.registry[_np.datetime64] = converter
-    hours = (df.index.values[-1] - df.index.values[0])//3600
-    locator = _mdates.HourLocator(interval=(hours//24 + 1)*3)
-    formatter = _mdates.ConciseDateFormatter(locator,show_offset=True) # offset with date at the bottom
-    formatter.zero_formats[3] = '%d-%b' # the 00:00 label formatter
+    hours = (df.index.values[-1] - df.index.values[0]) // 3600
+    locator = _mdates.HourLocator(interval=(hours // 24 + 1) * 3)
+    formatter = _mdates.ConciseDateFormatter(locator, show_offset=True)  # offset with date at the bottom
+    formatter.zero_formats[3] = "%d-%b"  # the 00:00 label formatter
 
-    df.index = _j20002datetime(df.index.values) # converting J2000 seconds to datetime64
+    df.index = _gn_datetime.j20002datetime(df.index.values)  # converting J2000 seconds to datetime64
     components = df.columns.levels[0]
     sv_list = df.columns.levels[1]
-    
-    styl_list=['solid','dotted','dashed','dashdot']
 
-    cmap = _cm.gist_rainbow #hsv in the original plotting script
+    styl_list = ["solid", "dotted", "dashed", "dashdot"]
+
+    cmap = _cm.gist_rainbow  # hsv in the original plotting script
     for i in range(len(axes_idx)):
         df_c = df[components[i]]
         for j in range(len(sv_list)):
-            axes[axes_idx[i]].plot(df_c[sv_list[j]],label=sv_list[j] if (i==0 and legend)else '',
-                       ls=styl_list[j % 4],color=cmap(j/len(sv_list)))
+            axes[axes_idx[i]].plot(
+                df_c[sv_list[j]],
+                label=sv_list[j] if (i == 0 and legend) else "",
+                ls=styl_list[j % 4],
+                color=cmap(j / len(sv_list)),
+            )
 
-        axes[axes_idx[i]].set_ylabel(f'{components[i]} (cm)')
+        axes[axes_idx[i]].set_ylabel(f"{components[i]} (cm)")
 
     axes[0].xaxis.set_major_locator(locator)
     axes[0].xaxis.set_major_formatter(formatter)
 
-def diff2plot(diff, kind=None,title='Unnamed plot'):
+
+def diff2plot(diff, kind=None, title="Unnamed plot"):
     """Function to plot graph to the terminal. Can be scatter or bar plot (Initial test functionality)
     Works only with plotext 4.2, not above"""
     # try:
     #     import plotext as plt
     # except ModuleNotFoundError:
     #     # Error handling
     #     pass
     plx.clear_plot()
     diff = diff.round(2)
-    if kind == 'bar':
+    if kind == "bar":
         # expects a series with index being string names
         mask0 = (diff.values != 0) & ~_np.isnan(diff.values)
         if mask0.any():
-            plx.bar(diff.index.values[mask0].tolist(), diff.values[mask0].tolist(),orientation = "h",width=0.3)
-            plx.vertical_line(coordinate = 0)
-            plx.plotsize(100,diff.shape[0]*2 + 3)
+            plx.bar(diff.index.values[mask0].tolist(), diff.values[mask0].tolist(), orientation="h", width=0.3)
+            plx.vertical_line(coordinate=0)
+            plx.plotsize(100, diff.shape[0] * 2 + 3)
         else:
             return None
     else:
         mask0 = ((diff.values != 0) & ~_np.isnan(diff.values)).any(axis=0)
         if mask0.any():
             cols = diff.columns[mask0]
-            x1 = plx.datetime.datetime_to_string(diff.index.astype('timedelta64[ns]')*1000000000 + _J2000_ORIGIN)
+            x1 = _gn_datetime.j20002datetime(diff.index.values).astype(str)
+            plx.datetime._datetime_form = "%Y-%m-%dT%H:%M:%S" # change parsed format to numpy-like
             for i in range(cols.shape[0]):
-                plx.scatter_date(x1, diff[cols[i]].to_list(), color=i,marker = "hd",label=diff.columns[i])
-                plx.plotsize(100,30 + 3)
+                plx.scatter_date(x1, diff[cols[i]].to_list(), color=i, marker="hd", label=diff.columns[i])
+                plx.plotsize(100, 30 + 3)
         else:
             return None
 
     plx.title(title)
-    plx.limit_size(limit_xsize=False,limit_ysize=False)
+    plx.limit_size(limit_xsize=False, limit_ysize=False)
     plx.show()
 
-def id_df2html(id_df,outdir=None,verbose=False):
+
+def id_df2html(id_df, outdir=None, verbose=False):
     import plotly.express as px
-    fig = px.scatter_geo(id_df, lon="LON",lat="LAT",title=id_df.attrs['infomsg'],
-                    size="SIZE",color="PATH",size_max=18,
-                    hover_name="CODE", # column added to hover information
-                    hover_data = ["PT","DOMES"],
-                    projection="natural earth")
-    filename = ("gather_map" if len(id_df.attrs['info'])>1 else _os.path.basename(list(id_df.attrs['info'])[0]))+".html"
-    save_path = _os.path.join(_os.path.curdir if outdir is None else outdir,filename)
-    if verbose:_logging.info(msg=f"saving html to {_os.path.abspath(save_path)}")
+
+    fig = px.scatter_geo(
+        id_df,
+        lon="LON",
+        lat="LAT",
+        title=id_df.attrs["infomsg"],
+        size="SIZE",
+        color="PATH",
+        size_max=18,
+        hover_name="CODE",  # column added to hover information
+        hover_data=["PT", "DOMES"],
+        projection="natural earth",
+    )
+    filename = (
+        "gather_map" if len(id_df.attrs["info"]) > 1 else _os.path.basename(list(id_df.attrs["info"])[0])
+    ) + ".html"
+    save_path = _os.path.join(_os.path.curdir if outdir is None else outdir, filename)
+    if verbose:
+        _logging.info(msg=f"saving html to {_os.path.abspath(save_path)}")
     fig.write_html(save_path)
 
-def racplot(rac_unstack,output=None):
+
+def racplot(rac_unstack, output=None):
     import matplotlib.pyplot as plt
+
     extended_plot = rac_unstack.attrs["hlm_mode"] is not None
-    fig = plt.figure(figsize=(10, 5+5*extended_plot),dpi=100)
-    gs = fig.add_gridspec(3+3*extended_plot, hspace=0.2)
+    fig = plt.figure(figsize=(10, 5 + 5 * extended_plot), dpi=100)
+    gs = fig.add_gridspec(3 + 3 * extended_plot, hspace=0.2)
     ax = gs.subplots(sharex=True, sharey=False)
-    plot_vec(axes=ax,df=rac_unstack*100,axes_idx=[1,2,0]) # meter to cm
+    plot_vec(axes=ax, df=rac_unstack * 100, axes_idx=[1, 2, 0])  # meter to cm
 
-    if extended_plot: # append hlm residuals plot if transformation has been selected 
-        line = plt.Line2D([0,1],[0.49,0.49], transform=fig.transFigure, color="black",ls="--")
-        plt.text(0.015,0.485,va = "top",
-        s=f"{rac_unstack.attrs['sp3_b']} - {rac_unstack.attrs['sp3_b']}" + f" (HLM in {rac_unstack.attrs['hlm_mode']})\nResiduals shown are in ECI frame",
-        rotation=90, transform=fig.transFigure, fontfamily="monospace")
+    if extended_plot:  # append hlm residuals plot if transformation has been selected
+        line = plt.Line2D([0, 1], [0.49, 0.49], transform=fig.transFigure, color="black", ls="--")
+        plt.text(
+            0.015,
+            0.485,
+            va="top",
+            s=f"{rac_unstack.attrs['sp3_b']} - {rac_unstack.attrs['sp3_b']}"
+            + f" (HLM in {rac_unstack.attrs['hlm_mode']})\nResiduals shown are in ECI frame",
+            rotation=90,
+            transform=fig.transFigure,
+            fontfamily="monospace",
+        )
         fig.add_artist(line)
 
-        plot_vec(axes=ax,df=rac_unstack.attrs["hlm"][1].RES.unstack() * 100000,axes_idx=[3,4,5],legend=False)
+        plot_vec(axes=ax, df=rac_unstack.attrs["hlm"][1].RES.unstack() * 100000, axes_idx=[3, 4, 5], legend=False)
 
         hlm = rac_unstack.attrs["hlm"][0][0].reshape(-1).tolist()
-        hlm_txt = ("HLM coeffiecients:\n\n" 
-                    + f"Tx {hlm[0]:13.5e}\nTy {hlm[1]:13.5e}\nTz {hlm[2]:13.5e}\n"
-                    + f"Rx {hlm[0]:13.5e}\nRy {hlm[1]:13.5e}\nRz {hlm[2]:13.5e}\n"
-                    + f"μ  {hlm[0]:13.5e}")
-        plt.text(0.815,0.485,s=hlm_txt,va = "top", transform=fig.transFigure, fontfamily="monospace")
-
-    fig.suptitle(rac_unstack.attrs['sp3_a'] + " - " + rac_unstack.attrs['sp3_b'] + (f" (HLM in {rac_unstack.attrs['hlm_mode']})" if extended_plot else ""),y=0.92)
-    fig.patch.set_facecolor("w") #white background (non-transparent)
-    fig.legend(bbox_to_anchor = (.955,.89),ncol=2,fontsize=8)
+        hlm_txt = (
+            "HLM coeffiecients:\n\n"
+            + f"Tx {hlm[0]:13.5e}\nTy {hlm[1]:13.5e}\nTz {hlm[2]:13.5e}\n"
+            + f"Rx {hlm[0]:13.5e}\nRy {hlm[1]:13.5e}\nRz {hlm[2]:13.5e}\n"
+            + f"μ  {hlm[0]:13.5e}"
+        )
+        plt.text(0.815, 0.485, s=hlm_txt, va="top", transform=fig.transFigure, fontfamily="monospace")
+
+    fig.suptitle(
+        rac_unstack.attrs["sp3_a"]
+        + " - "
+        + rac_unstack.attrs["sp3_b"]
+        + (f" (HLM in {rac_unstack.attrs['hlm_mode']})" if extended_plot else ""),
+        y=0.92,
+    )
+    fig.patch.set_facecolor("w")  # white background (non-transparent)
+    fig.legend(bbox_to_anchor=(0.955, 0.89), ncol=2, fontsize=8)
     plt.subplots_adjust(right=0.8)
 
-    fig.savefig(f"{rac_unstack.attrs['sp3_a'].split('.')[0]}-{rac_unstack.attrs['sp3_b'].split('.')[0]}.pdf" if output is None else output)
+    fig.savefig(
+        f"{rac_unstack.attrs['sp3_a'].split('.')[0]}-{rac_unstack.attrs['sp3_b'].split('.')[0]}.pdf"
+        if output is None
+        else output
+    )
```

### Comparing `gnssanalysis-0.0.9/gnssanalysis.egg-info/SOURCES.txt` & `gnssanalysis-0.54/gnssanalysis.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,47 @@
+LICENSE
+README.md
+setup.cfg
 setup.py
 gnssanalysis/__init__.py
-gnssanalysis/create_erp_file.py
+gnssanalysis/_version.py
+gnssanalysis/filenames.py
 gnssanalysis/gn_aux.py
 gnssanalysis/gn_combi.py
 gnssanalysis/gn_const.py
 gnssanalysis/gn_datetime.py
 gnssanalysis/gn_diffaux.py
 gnssanalysis/gn_download.py
 gnssanalysis/gn_frame.py
 gnssanalysis/gn_plot.py
 gnssanalysis/gn_transform.py
 gnssanalysis/gn_utils.py
+gnssanalysis/py.typed
 gnssanalysis.egg-info/PKG-INFO
 gnssanalysis.egg-info/SOURCES.txt
 gnssanalysis.egg-info/dependency_links.txt
 gnssanalysis.egg-info/entry_points.txt
 gnssanalysis.egg-info/requires.txt
 gnssanalysis.egg-info/top_level.txt
 gnssanalysis/gn_io/__init__.py
 gnssanalysis/gn_io/aux_dicts.py
+gnssanalysis/gn_io/bia.py
+gnssanalysis/gn_io/blq.py
 gnssanalysis/gn_io/clk.py
 gnssanalysis/gn_io/common.py
 gnssanalysis/gn_io/discon.py
+gnssanalysis/gn_io/erp.py
 gnssanalysis/gn_io/igslog.py
 gnssanalysis/gn_io/ionex.py
+gnssanalysis/gn_io/nanu.py
 gnssanalysis/gn_io/pea.py
 gnssanalysis/gn_io/pod.py
 gnssanalysis/gn_io/psd.py
 gnssanalysis/gn_io/rinex.py
 gnssanalysis/gn_io/sinex.py
 gnssanalysis/gn_io/sp3.py
 gnssanalysis/gn_io/stec.py
 gnssanalysis/gn_io/trace.py
-gnssanalysis/gn_io/trop.py
+gnssanalysis/gn_io/trop.py
+tests/test_aux.py
+tests/test_datetime.py
+tests/test_transform.py
```

