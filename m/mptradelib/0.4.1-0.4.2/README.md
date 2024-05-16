# Comparing `tmp/mptradelib-0.4.1.tar.gz` & `tmp/mptradelib-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mptradelib-0.4.1.tar", max compression
+gzip compressed data, was "mptradelib-0.4.2.tar", max compression
```

## Comparing `mptradelib-0.4.1.tar` & `mptradelib-0.4.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     3137 2024-05-03 13:20:41.913077 mptradelib-0.4.1/README.md
--rw-r--r--   0        0        0        0 2024-04-30 08:23:49.256174 mptradelib-0.4.1/mptradelib/__init__.py
--rw-r--r--   0        0        0     4662 2024-05-10 19:46:01.019193 mptradelib-0.4.1/mptradelib/backtest.py
--rw-r--r--   0        0        0        0 2024-04-30 08:23:49.266753 mptradelib-0.4.1/mptradelib/broker/__init__.py
--rw-r--r--   0        0        0    11073 2024-05-09 18:27:16.773912 mptradelib-0.4.1/mptradelib/broker/broker.py
--rw-r--r--   0        0        0     5808 2024-05-09 18:04:15.841857 mptradelib-0.4.1/mptradelib/broker/session.py
--rw-r--r--   0        0        0    34066 2024-05-01 10:05:54.173058 mptradelib-0.4.1/mptradelib/broker/shoonya.py
--rw-r--r--   0        0        0     2683 2024-05-01 14:36:23.728530 mptradelib-0.4.1/mptradelib/broker/ticker.py
--rw-r--r--   0        0        0        0 2024-05-03 11:19:20.268249 mptradelib-0.4.1/mptradelib/cli/__init__.py
--rw-r--r--   0        0        0     2342 2024-05-09 18:05:58.447254 mptradelib-0.4.1/mptradelib/cli/new.py
--rw-r--r--   0        0        0      953 2024-05-09 18:11:12.323673 mptradelib-0.4.1/mptradelib/cli/templates/strategy/__init__.py.jinja
--rw-r--r--   0        0        0     2984 2024-05-04 12:28:56.516490 mptradelib-0.4.1/mptradelib/cli/templates/strategy/backtest.ipynb.jinja
--rw-r--r--   0        0        0      614 2024-05-03 12:29:43.201283 mptradelib-0.4.1/mptradelib/cli/templates/strategy/livetrade.py.jinja
--rw-r--r--   0        0        0     5394 2024-05-09 18:03:46.504439 mptradelib-0.4.1/mptradelib/feed.py
--rw-r--r--   0        0        0     2007 2024-05-09 18:25:26.040938 mptradelib-0.4.1/mptradelib/livetrade.py
--rw-r--r--   0        0        0       36 2024-05-11 12:09:46.778908 mptradelib-0.4.1/mptradelib/optimizers/__init__.py
--rw-r--r--   0        0        0     5103 2024-05-11 12:09:34.052370 mptradelib-0.4.1/mptradelib/optimizers/walkforward.py
--rw-r--r--   0        0        0     1313 2024-04-30 08:23:49.272908 mptradelib-0.4.1/mptradelib/test_renko.py
--rw-r--r--   0        0        0       77 2024-05-06 16:16:12.200968 mptradelib-0.4.1/mptradelib/utils/__init__.py
--rw-r--r--   0        0        0      902 2024-05-06 16:14:19.221626 mptradelib-0.4.1/mptradelib/utils/simulated_trades.py
--rw-r--r--   0        0        0     6878 2024-05-10 13:29:58.164902 mptradelib-0.4.1/mptradelib/utils/tearsheet.py
--rw-r--r--   0        0        0      910 2024-05-06 16:15:09.786235 mptradelib-0.4.1/mptradelib/utils/utils.py
--rw-r--r--   0        0        0      846 2024-05-11 12:09:58.305379 mptradelib-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     4041 1970-01-01 00:00:00.000000 mptradelib-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     3137 2024-05-03 13:20:41.913077 mptradelib-0.4.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-30 08:23:49.256174 mptradelib-0.4.2/mptradelib/__init__.py
+-rw-r--r--   0        0        0     5335 2024-05-16 04:46:22.453847 mptradelib-0.4.2/mptradelib/backtest.py
+-rw-r--r--   0        0        0        0 2024-04-30 08:23:49.266753 mptradelib-0.4.2/mptradelib/broker/__init__.py
+-rw-r--r--   0        0        0    11073 2024-05-09 18:27:16.773912 mptradelib-0.4.2/mptradelib/broker/broker.py
+-rw-r--r--   0        0        0     5808 2024-05-09 18:04:15.841857 mptradelib-0.4.2/mptradelib/broker/session.py
+-rw-r--r--   0        0        0    34066 2024-05-01 10:05:54.173058 mptradelib-0.4.2/mptradelib/broker/shoonya.py
+-rw-r--r--   0        0        0     2683 2024-05-01 14:36:23.728530 mptradelib-0.4.2/mptradelib/broker/ticker.py
+-rw-r--r--   0        0        0        0 2024-05-03 11:19:20.268249 mptradelib-0.4.2/mptradelib/cli/__init__.py
+-rw-r--r--   0        0        0     2342 2024-05-09 18:05:58.447254 mptradelib-0.4.2/mptradelib/cli/new.py
+-rw-r--r--   0        0        0      953 2024-05-09 18:11:12.323673 mptradelib-0.4.2/mptradelib/cli/templates/strategy/__init__.py.jinja
+-rw-r--r--   0        0        0     2984 2024-05-04 12:28:56.516490 mptradelib-0.4.2/mptradelib/cli/templates/strategy/backtest.ipynb.jinja
+-rw-r--r--   0        0        0      614 2024-05-03 12:29:43.201283 mptradelib-0.4.2/mptradelib/cli/templates/strategy/livetrade.py.jinja
+-rw-r--r--   0        0        0     5394 2024-05-09 18:03:46.504439 mptradelib-0.4.2/mptradelib/feed.py
+-rw-r--r--   0        0        0     2007 2024-05-09 18:25:26.040938 mptradelib-0.4.2/mptradelib/livetrade.py
+-rw-r--r--   0        0        0       36 2024-05-11 12:09:46.778908 mptradelib-0.4.2/mptradelib/optimizers/__init__.py
+-rw-r--r--   0        0        0     6149 2024-05-12 18:13:43.345085 mptradelib-0.4.2/mptradelib/optimizers/walkforward.py
+-rw-r--r--   0        0        0     1313 2024-04-30 08:23:49.272908 mptradelib-0.4.2/mptradelib/test_renko.py
+-rw-r--r--   0        0        0       77 2024-05-06 16:16:12.200968 mptradelib-0.4.2/mptradelib/utils/__init__.py
+-rw-r--r--   0        0        0      902 2024-05-06 16:14:19.221626 mptradelib-0.4.2/mptradelib/utils/simulated_trades.py
+-rw-r--r--   0        0        0     6887 2024-05-12 12:25:21.588670 mptradelib-0.4.2/mptradelib/utils/tearsheet.py
+-rw-r--r--   0        0        0      910 2024-05-06 16:15:09.786235 mptradelib-0.4.2/mptradelib/utils/utils.py
+-rw-r--r--   0        0        0      846 2024-05-16 04:46:40.912078 mptradelib-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     4041 1970-01-01 00:00:00.000000 mptradelib-0.4.2/PKG-INFO
```

### Comparing `mptradelib-0.4.1/README.md` & `mptradelib-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `mptradelib-0.4.1/mptradelib/broker/broker.py` & `mptradelib-0.4.2/mptradelib/broker/broker.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.4.1/mptradelib/broker/session.py` & `mptradelib-0.4.2/mptradelib/broker/session.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.4.1/mptradelib/broker/shoonya.py` & `mptradelib-0.4.2/mptradelib/broker/shoonya.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.4.1/mptradelib/broker/ticker.py` & `mptradelib-0.4.2/mptradelib/broker/ticker.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.4.1/mptradelib/cli/new.py` & `mptradelib-0.4.2/mptradelib/cli/new.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.4.1/mptradelib/cli/templates/strategy/__init__.py.jinja` & `mptradelib-0.4.2/mptradelib/cli/templates/strategy/__init__.py.jinja`

 * *Files identical despite different names*

### Comparing `mptradelib-0.4.1/mptradelib/cli/templates/strategy/backtest.ipynb.jinja` & `mptradelib-0.4.2/mptradelib/cli/templates/strategy/backtest.ipynb.jinja`

 * *Files identical despite different names*

### Comparing `mptradelib-0.4.1/mptradelib/cli/templates/strategy/livetrade.py.jinja` & `mptradelib-0.4.2/mptradelib/cli/templates/strategy/livetrade.py.jinja`

 * *Files identical despite different names*

### Comparing `mptradelib-0.4.1/mptradelib/feed.py` & `mptradelib-0.4.2/mptradelib/feed.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.4.1/mptradelib/livetrade.py` & `mptradelib-0.4.2/mptradelib/livetrade.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.4.1/mptradelib/optimizers/walkforward.py` & `mptradelib-0.4.2/mptradelib/optimizers/walkforward.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,36 @@
 import json
 import pandas as pd
 from tqdm import tqdm
 import os
 import plotly.graph_objects as go
-from ..utils import Tearsheet
-from ..backtest import Backtest
+from mptradelib.utils import Tearsheet
+from mptradelib.backtest import Backtest
 from typing import Callable
+import datetime as dt
+import multiprocessing as mp
+from functools import partial
 
 
 class WalkForward:
-    def __init__(self, df: pd.DataFrame, compute: Callable[[pd.DataFrame, dict], None], optimization_params: dict, freq='W', cache_path = ".") -> None:
+    def __init__(self, 
+                 df: pd.DataFrame, 
+                 compute: Callable[[pd.DataFrame, dict], None], 
+                 optimization_params: dict, 
+                 freq='W', 
+                 cache_path = ".", 
+                 intraday_exit_time: dt.time = dt.time(15,10,0),
+                 intraday=True,
+        ) -> None:
         self.df = df
         self._compute = compute
         self._oparam = optimization_params
         self._freq = freq
+        self._intraday = intraday
+        self._intraday_exit_time = intraday_exit_time
         self._cache_path = os.path.join(cache_path, 'walkforward-reports')
         if not os.path.exists(self._cache_path):
             os.mkdir(self._cache_path)
 
     def _get_date(self, d, index):
         return d.datetime.iloc[index].strftime("%Y-%m-%d")
 
@@ -52,71 +65,89 @@
             if dirname == '.DS_Store':
                 continue
             try:
                 filepath = os.path.join(self._cache_path, dirname, "report.csv")
             except Exception as e:
                 print(f'reading {filepath}')
                 raise e
-            dff = pd.read_csv(filepath)
-            dflist.append(dff)
+            
+            if os.path.exists(filepath):
+                try:
+                    dff = pd.read_csv(filepath)
+                except Exception as e:
+                    print(f'file {filepath}: {e}')
+                    continue
+
+                dflist.append(dff)
 
         fdf = pd.concat(dflist)
         fdf = fdf.sort_values(by=['entry_time']).drop_duplicates().reset_index(drop='index')
         fdf.entry_time = pd.to_datetime(fdf.entry_time)
         fdf.exit_time = pd.to_datetime(fdf.exit_time)
         fdf.to_csv('result.csv', index=False)
 
         t = Tearsheet(fdf)
         t.print()
         t.plot()
 
-    def _optimize(self, df, runs=5, show_progress=False):
-        b = Backtest(df, self._compute, sl=1, tp=2, intraday=True)
+    def _optimize(self, df, opt_param='profit'):
+        b = Backtest(df, self._compute, sl=1, tp=2, intraday_exit_time=self._intraday_exit_time, intraday=self._intraday)
         r = b.optimize(
-            runs=runs,
-            show_progress=show_progress,
-            **self._oparam
+            self._oparam,
+            opt_param=opt_param
         )
-        return r[0]
+        return r[0] if r is not None else None
 
-    def _create_optimization_worker(self, params, runs=5):
+    def _create_optimization_worker(self, opt_param, params):
         dfopt, dftest, reports_path = params
 
         filename = f'{dftest.iloc[0].datetime.strftime("%Y-%m-%d")}-{dftest.iloc[-1].datetime.strftime("%Y-%m-%d")}'
         dirpath = os.path.join(reports_path, filename)
         if not os.path.exists(dirpath):
             os.mkdir(dirpath)
         
         param_path = os.path.join(dirpath, 'params.json')
         report_path = os.path.join(dirpath, 'report.csv')
 
         if os.path.exists(report_path):
-            return pd.read_csv(report_path)
+            try:
+                t = pd.read_csv(report_path)
+                return t
+            except Exception as e:
+                print(e)
+                return
 
-        r = self._optimize(dfopt, runs)
+        r = self._optimize(dfopt, opt_param=opt_param)
+        if r is None:
+            return r
+        
         with open(param_path, 'w') as f:
             f.write(json.dumps(r))
 
-        c = Backtest(dftest, self._compute, sl=1, tp=2, intraday=True)
+        c = Backtest(dftest, self._compute, sl=1, tp=2, intraday_exit_time=self._intraday_exit_time, intraday=True)
         out = c.run(**{k: int(v) for k, v in r.items()})
-        out[0].to_csv(report_path, index=False)
-        return out[0]
+        if out is not None:
+            out[0].to_csv(report_path, index=False)
 
 
-    def run(self, train_size, test_size, step=1, runs=5):
+    def run(self, train_size, test_size, step=1, opt_param='profit'):
         splits = self.data_splitter(train_size, test_size, step)
-        self._plot_splits(splits)
-        self._optimize_splits(splits, runs)
+        try:
+            self._plot_splits(splits)
+        except Exception:
+            pass
+        self._optimize_splits(splits, opt_param)
         self._calculate_result()
 
-    def _optimize_splits(self, splits, runs):
+    def _optimize_splits(self, splits, opt_param):
         with tqdm(total=len(splits)) as pbar:
-            for p in splits:
-                self._create_optimization_worker(p, runs)
-                pbar.update()
+            with mp.Pool(mp.cpu_count()) as p:
+                f = partial(self._create_optimization_worker, opt_param)
+                for _ in p.imap(f, splits):
+                    pbar.update()
 
     def _plot_splits(self, splits):
         fig = go.Figure()
         for i in range(len(splits)):
             s = splits[i]
             opt_set, test_set, _ = s
             fig.add_trace(go.Scatter(
```

### Comparing `mptradelib-0.4.1/mptradelib/test_renko.py` & `mptradelib-0.4.2/mptradelib/test_renko.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.4.1/mptradelib/utils/simulated_trades.py` & `mptradelib-0.4.2/mptradelib/utils/simulated_trades.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.4.1/mptradelib/utils/tearsheet.py` & `mptradelib-0.4.2/mptradelib/utils/tearsheet.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     
     def long_short_composition(self):
         positive = self.df[self.df.profit > 0].groupby('direction').agg({'profit': 'sum'})
         negative = self.df[self.df.profit < 0].groupby('direction').agg({'profit': 'sum'}).rename(columns={'profit': 'loss'})
         return pd.concat([positive, negative], axis=1).round(2).rename(index={1: 'long', -1: 'short'})
     
     def fund_growth(self):
-        s = SimulateTrades(self.df, initial_cash=self._seed, leverage=self._leverage)
+        s = SimulateTrades(self.df.dropna(), initial_cash=self._seed, leverage=self._leverage)
         return s.simple(), s.compound()
 
     def print(self):
         mdd, _ = self.max_drawdown()
         ncom, com = self.fund_growth()
         output = f'''
 Performance metrics (From: {self.df.iloc[0].entry_time.date()} To: {self.df.iloc[-1].entry_time.date()})
```

### Comparing `mptradelib-0.4.1/mptradelib/utils/utils.py` & `mptradelib-0.4.2/mptradelib/utils/utils.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.4.1/pyproject.toml` & `mptradelib-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mptradelib"
-version = "0.4.1"
+version = "0.4.2"
 description = ""
 authors = ["Abhilash Nanda <wishabhilash@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "2.7.1"
```

### Comparing `mptradelib-0.4.1/PKG-INFO` & `mptradelib-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mptradelib
-Version: 0.4.1
+Version: 0.4.2
 Summary: 
 Author: Abhilash Nanda
 Author-email: wishabhilash@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

