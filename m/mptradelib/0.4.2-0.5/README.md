# Comparing `tmp/mptradelib-0.4.2.tar.gz` & `tmp/mptradelib-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mptradelib-0.4.2.tar", max compression
+gzip compressed data, was "mptradelib-0.5.tar", max compression
```

## Comparing `mptradelib-0.4.2.tar` & `mptradelib-0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     3137 2024-05-03 13:20:41.913077 mptradelib-0.4.2/README.md
--rw-r--r--   0        0        0        0 2024-04-30 08:23:49.256174 mptradelib-0.4.2/mptradelib/__init__.py
--rw-r--r--   0        0        0     5335 2024-05-16 04:46:22.453847 mptradelib-0.4.2/mptradelib/backtest.py
--rw-r--r--   0        0        0        0 2024-04-30 08:23:49.266753 mptradelib-0.4.2/mptradelib/broker/__init__.py
--rw-r--r--   0        0        0    11073 2024-05-09 18:27:16.773912 mptradelib-0.4.2/mptradelib/broker/broker.py
--rw-r--r--   0        0        0     5808 2024-05-09 18:04:15.841857 mptradelib-0.4.2/mptradelib/broker/session.py
--rw-r--r--   0        0        0    34066 2024-05-01 10:05:54.173058 mptradelib-0.4.2/mptradelib/broker/shoonya.py
--rw-r--r--   0        0        0     2683 2024-05-01 14:36:23.728530 mptradelib-0.4.2/mptradelib/broker/ticker.py
--rw-r--r--   0        0        0        0 2024-05-03 11:19:20.268249 mptradelib-0.4.2/mptradelib/cli/__init__.py
--rw-r--r--   0        0        0     2342 2024-05-09 18:05:58.447254 mptradelib-0.4.2/mptradelib/cli/new.py
--rw-r--r--   0        0        0      953 2024-05-09 18:11:12.323673 mptradelib-0.4.2/mptradelib/cli/templates/strategy/__init__.py.jinja
--rw-r--r--   0        0        0     2984 2024-05-04 12:28:56.516490 mptradelib-0.4.2/mptradelib/cli/templates/strategy/backtest.ipynb.jinja
--rw-r--r--   0        0        0      614 2024-05-03 12:29:43.201283 mptradelib-0.4.2/mptradelib/cli/templates/strategy/livetrade.py.jinja
--rw-r--r--   0        0        0     5394 2024-05-09 18:03:46.504439 mptradelib-0.4.2/mptradelib/feed.py
--rw-r--r--   0        0        0     2007 2024-05-09 18:25:26.040938 mptradelib-0.4.2/mptradelib/livetrade.py
--rw-r--r--   0        0        0       36 2024-05-11 12:09:46.778908 mptradelib-0.4.2/mptradelib/optimizers/__init__.py
--rw-r--r--   0        0        0     6149 2024-05-12 18:13:43.345085 mptradelib-0.4.2/mptradelib/optimizers/walkforward.py
--rw-r--r--   0        0        0     1313 2024-04-30 08:23:49.272908 mptradelib-0.4.2/mptradelib/test_renko.py
--rw-r--r--   0        0        0       77 2024-05-06 16:16:12.200968 mptradelib-0.4.2/mptradelib/utils/__init__.py
--rw-r--r--   0        0        0      902 2024-05-06 16:14:19.221626 mptradelib-0.4.2/mptradelib/utils/simulated_trades.py
--rw-r--r--   0        0        0     6887 2024-05-12 12:25:21.588670 mptradelib-0.4.2/mptradelib/utils/tearsheet.py
--rw-r--r--   0        0        0      910 2024-05-06 16:15:09.786235 mptradelib-0.4.2/mptradelib/utils/utils.py
--rw-r--r--   0        0        0      846 2024-05-16 04:46:40.912078 mptradelib-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     4041 1970-01-01 00:00:00.000000 mptradelib-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     3137 2024-05-03 13:20:41.913077 mptradelib-0.5/README.md
+-rw-r--r--   0        0        0        0 2024-04-30 08:23:49.256174 mptradelib-0.5/mptradelib/__init__.py
+-rw-r--r--   0        0        0     4475 2024-05-16 13:35:32.766054 mptradelib-0.5/mptradelib/backtest.py
+-rw-r--r--   0        0        0        0 2024-04-30 08:23:49.266753 mptradelib-0.5/mptradelib/broker/__init__.py
+-rw-r--r--   0        0        0    11073 2024-05-09 18:27:16.773912 mptradelib-0.5/mptradelib/broker/broker.py
+-rw-r--r--   0        0        0     5808 2024-05-09 18:04:15.841857 mptradelib-0.5/mptradelib/broker/session.py
+-rw-r--r--   0        0        0    34066 2024-05-01 10:05:54.173058 mptradelib-0.5/mptradelib/broker/shoonya.py
+-rw-r--r--   0        0        0     2683 2024-05-01 14:36:23.728530 mptradelib-0.5/mptradelib/broker/ticker.py
+-rw-r--r--   0        0        0        0 2024-05-03 11:19:20.268249 mptradelib-0.5/mptradelib/cli/__init__.py
+-rw-r--r--   0        0        0     2342 2024-05-09 18:05:58.447254 mptradelib-0.5/mptradelib/cli/new.py
+-rw-r--r--   0        0        0      953 2024-05-09 18:11:12.323673 mptradelib-0.5/mptradelib/cli/templates/strategy/__init__.py.jinja
+-rw-r--r--   0        0        0     2984 2024-05-04 12:28:56.516490 mptradelib-0.5/mptradelib/cli/templates/strategy/backtest.ipynb.jinja
+-rw-r--r--   0        0        0      614 2024-05-03 12:29:43.201283 mptradelib-0.5/mptradelib/cli/templates/strategy/livetrade.py.jinja
+-rw-r--r--   0        0        0     5394 2024-05-09 18:03:46.504439 mptradelib-0.5/mptradelib/feed.py
+-rw-r--r--   0        0        0     2007 2024-05-09 18:25:26.040938 mptradelib-0.5/mptradelib/livetrade.py
+-rw-r--r--   0        0        0       36 2024-05-11 12:09:46.778908 mptradelib-0.5/mptradelib/optimizers/__init__.py
+-rw-r--r--   0        0        0     3072 2024-05-16 13:38:31.319826 mptradelib-0.5/mptradelib/optimizers/walkforward.py
+-rw-r--r--   0        0        0     1313 2024-04-30 08:23:49.272908 mptradelib-0.5/mptradelib/test_renko.py
+-rw-r--r--   0        0        0       77 2024-05-06 16:16:12.200968 mptradelib-0.5/mptradelib/utils/__init__.py
+-rw-r--r--   0        0        0      902 2024-05-06 16:14:19.221626 mptradelib-0.5/mptradelib/utils/simulated_trades.py
+-rw-r--r--   0        0        0     6887 2024-05-12 12:25:21.588670 mptradelib-0.5/mptradelib/utils/tearsheet.py
+-rw-r--r--   0        0        0      910 2024-05-06 16:15:09.786235 mptradelib-0.5/mptradelib/utils/utils.py
+-rw-r--r--   0        0        0      844 2024-05-16 13:38:39.711749 mptradelib-0.5/pyproject.toml
+-rw-r--r--   0        0        0     4039 1970-01-01 00:00:00.000000 mptradelib-0.5/PKG-INFO
```

### Comparing `mptradelib-0.4.2/README.md` & `mptradelib-0.5/README.md`

 * *Files identical despite different names*

### Comparing `mptradelib-0.4.2/mptradelib/backtest.py` & `mptradelib-0.5/mptradelib/backtest.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,16 @@
 import datetime as dt
 import pandas as pd
-import numpy as np
 from typing import Callable
 from tqdm import tqdm
-from hyperopt import fmin, tpe, hp, STATUS_OK
-from hyperopt.pyll import scope
 from retry import retry
-import multiprocessing as mp
 from .broker.broker import Order
-from typing import List, Union
-from .utils import Tearsheet
-from pydantic import BaseModel
-from functools import partial
+from itertools import product
 
 
-class urange(BaseModel):
-    start: Union[int, float]
-    stop: Union[int, float]
-    step: Union[int, float] = 1
-
 class Backtest:
     params: dict = {
         "sl": None,
         "tp": None
     }
 
     def __init__(self, 
@@ -48,15 +36,15 @@
         
         if 'entries' not in data.columns.to_list():
             raise KeyError('column "entries" not found.')
         
         try:
             data.loc[data.entries != 0, 'entry_price'] = data.open.shift(-1)
         except Exception as e:
-            print(data)
+            print(data, '.............')
             raise e
 
         data.loc[data.entries == 1, 'sl'] = data.close * (1 - self.params['sl']/100)
         data.loc[data.entries == 1, 'tp'] = data.close * (1 + self.params['tp']/100)
 
         data.loc[data.entries == -1, 'sl'] = data.close * (1 + self.params['sl']/100)
         data.loc[data.entries == -1, 'tp'] = data.close * (1 - self.params['tp']/100)
@@ -96,54 +84,42 @@
                         position, orders = self._exit_position(row, position, orders)
 
             if row.entries != 0 and position is None and self._in_intraday_window(row):
                 position = Order(entry_time=row.trade_time, entry_price=row.entry_price, sl=row.sl, tp=row.tp, direction=row.entries)
         return orders
 
     def _define_space(self, params):
-        space = {}
+        opt_params = {}
+        constant_params = {}
         for k, v in params.items():
-            if not isinstance(v, urange):
-                raise TypeError(f"{v} is of type {type(v)}. Needs to be of type 'urange'.")
-            
-            if isinstance(v.step, int):
-                space[k] = scope.int(hp.quniform(k, v.start, v.stop, v.step))
-            elif isinstance(v.step, float):
-                space[k] = hp.quniform(k, v.start, v.stop, v.step)
+            if isinstance(v, range):
+                opt_params[k] = v
             else:
-                raise ValueError(f"step of {k} can not be {type(v.step)}")
-        return space
+                constant_params[k] = v
+        return opt_params, constant_params
+    
+    def _get_overfitting_score(self, t):
+        t['abs_profit'] = t.profit.abs()
+        ts = t.sort_values(by=['abs_profit'], ascending=False)
+        os = (ts[:int(len(ts)/100)].abs_profit.sum()/ts.abs_profit.sum())*100
+        rationalized_df = ts[int(len(ts)/100):]
+        return os, rationalized_df
 
     @retry(tries=10)
-    def optimize(self, kwargs, opt_param='profit'):
-        show_progressbar = kwargs.pop('show_progressbar', False)
-        max_evals = kwargs.pop('max_evals', 3000)
-        space = self._define_space(kwargs)
+    def optimize(self, kwargs):
+        opt_params, constant_params = self._define_space(kwargs)
         
         def objective(params):
-            r = self.run(**params)
-            if not len(r):
-                return {'loss': 0, 'status': STATUS_OK}
-            
-            if opt_param == 'profit':
-                loss = -np.sum(r[0].profit) if len(r[0]) else 0
-                return {'loss': loss, 'status': STATUS_OK}
-            elif opt_param == 'com':
-                t = Tearsheet(r[0])
-                ncom, com = t.fund_growth()
-                return {'loss': -com, 'status': STATUS_OK}
-            elif opt_param == 'winrate':
-                t = Tearsheet(r[0])
-                wr = t.win_rate()
-                return {'loss': -wr, 'status': STATUS_OK}
-        
-        best = fmin(
-            fn=objective,
-            space=space,
-            algo=tpe.suggest,
-            max_evals=max_evals,
-            show_progressbar=show_progressbar
-        )
-        p = {k: int(v) for k, v in best.items()}
-        r = self.run(**p)
-        return best, np.sum(r[0].profit)
-        
+            r, _ = self.run(**params)
+            os, rdf = self._get_overfitting_score(r.copy())
+            if os > 10:
+                r = rdf
+                print("removing event effect - ", param)
+            return {'params': params, 'trades': r}
+
+        results = []
+        for p in product(*opt_params.values()):
+            param = dict(zip(opt_params.keys(), p))
+            param.update(constant_params)
+            r = objective(param)
+            results.append(r)
+        return results
```

### Comparing `mptradelib-0.4.2/mptradelib/broker/broker.py` & `mptradelib-0.5/mptradelib/broker/broker.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.4.2/mptradelib/broker/session.py` & `mptradelib-0.5/mptradelib/broker/session.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.4.2/mptradelib/broker/shoonya.py` & `mptradelib-0.5/mptradelib/broker/shoonya.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.4.2/mptradelib/broker/ticker.py` & `mptradelib-0.5/mptradelib/broker/ticker.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.4.2/mptradelib/cli/new.py` & `mptradelib-0.5/mptradelib/cli/new.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.4.2/mptradelib/cli/templates/strategy/__init__.py.jinja` & `mptradelib-0.5/mptradelib/cli/templates/strategy/__init__.py.jinja`

 * *Files identical despite different names*

### Comparing `mptradelib-0.4.2/mptradelib/cli/templates/strategy/backtest.ipynb.jinja` & `mptradelib-0.5/mptradelib/cli/templates/strategy/backtest.ipynb.jinja`

 * *Files identical despite different names*

### Comparing `mptradelib-0.4.2/mptradelib/cli/templates/strategy/livetrade.py.jinja` & `mptradelib-0.5/mptradelib/cli/templates/strategy/livetrade.py.jinja`

 * *Files identical despite different names*

### Comparing `mptradelib-0.4.2/mptradelib/feed.py` & `mptradelib-0.5/mptradelib/feed.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.4.2/mptradelib/livetrade.py` & `mptradelib-0.5/mptradelib/livetrade.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.4.2/mptradelib/test_renko.py` & `mptradelib-0.5/mptradelib/test_renko.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.4.2/mptradelib/utils/simulated_trades.py` & `mptradelib-0.5/mptradelib/utils/simulated_trades.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.4.2/mptradelib/utils/tearsheet.py` & `mptradelib-0.5/mptradelib/utils/tearsheet.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.4.2/mptradelib/utils/utils.py` & `mptradelib-0.5/mptradelib/utils/utils.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.4.2/pyproject.toml` & `mptradelib-0.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mptradelib"
-version = "0.4.2"
+version = "0.5"
 description = ""
 authors = ["Abhilash Nanda <wishabhilash@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "2.7.1"
```

### Comparing `mptradelib-0.4.2/PKG-INFO` & `mptradelib-0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mptradelib
-Version: 0.4.2
+Version: 0.5
 Summary: 
 Author: Abhilash Nanda
 Author-email: wishabhilash@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

