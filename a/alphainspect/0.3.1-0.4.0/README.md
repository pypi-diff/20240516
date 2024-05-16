# Comparing `tmp/alphainspect-0.3.1.tar.gz` & `tmp/alphainspect-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphainspect-0.3.1.tar", last modified: Thu Apr 18 03:37:59 2024, max compression
+gzip compressed data, was "alphainspect-0.4.0.tar", last modified: Wed May 15 16:45:54 2024, max compression
```

## Comparing `alphainspect-0.3.1.tar` & `alphainspect-0.4.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:37:59.239461 alphainspect-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-18 03:37:54.000000 alphainspect-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-04-18 03:37:59.239461 alphainspect-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-18 03:37:54.000000 alphainspect-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:37:59.235461 alphainspect-0.3.1/alphainspect/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-18 03:37:54.000000 alphainspect-0.3.1/alphainspect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-04-18 03:37:54.000000 alphainspect-0.3.1/alphainspect/_nb.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-18 03:37:54.000000 alphainspect-0.3.1/alphainspect/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-04-18 03:37:54.000000 alphainspect-0.3.1/alphainspect/dtree.py
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-04-18 03:37:54.000000 alphainspect-0.3.1/alphainspect/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-04-18 03:37:54.000000 alphainspect-0.3.1/alphainspect/ic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7639 2024-04-18 03:37:54.000000 alphainspect-0.3.1/alphainspect/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-04-18 03:37:54.000000 alphainspect-0.3.1/alphainspect/reports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-18 03:37:54.000000 alphainspect-0.3.1/alphainspect/returns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-18 03:37:54.000000 alphainspect-0.3.1/alphainspect/selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-18 03:37:54.000000 alphainspect-0.3.1/alphainspect/turnover.py
--rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-04-18 03:37:54.000000 alphainspect-0.3.1/alphainspect/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:37:59.239461 alphainspect-0.3.1/alphainspect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-04-18 03:37:59.000000 alphainspect-0.3.1/alphainspect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-18 03:37:59.000000 alphainspect-0.3.1/alphainspect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 03:37:59.000000 alphainspect-0.3.1/alphainspect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-18 03:37:59.000000 alphainspect-0.3.1/alphainspect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-18 03:37:59.000000 alphainspect-0.3.1/alphainspect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-18 03:37:54.000000 alphainspect-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 03:37:59.239461 alphainspect-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:45:54.876057 alphainspect-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-15 16:45:50.000000 alphainspect-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-05-15 16:45:54.876057 alphainspect-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-15 16:45:50.000000 alphainspect-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:45:54.876057 alphainspect-0.4.0/alphainspect/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-15 16:45:50.000000 alphainspect-0.4.0/alphainspect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-05-15 16:45:50.000000 alphainspect-0.4.0/alphainspect/_nb.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-15 16:45:50.000000 alphainspect-0.4.0/alphainspect/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-15 16:45:50.000000 alphainspect-0.4.0/alphainspect/dtree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-15 16:45:50.000000 alphainspect-0.4.0/alphainspect/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-05-15 16:45:50.000000 alphainspect-0.4.0/alphainspect/ic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8832 2024-05-15 16:45:50.000000 alphainspect-0.4.0/alphainspect/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-05-15 16:45:50.000000 alphainspect-0.4.0/alphainspect/reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-15 16:45:50.000000 alphainspect-0.4.0/alphainspect/returns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-15 16:45:50.000000 alphainspect-0.4.0/alphainspect/selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-15 16:45:50.000000 alphainspect-0.4.0/alphainspect/turnover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-05-15 16:45:50.000000 alphainspect-0.4.0/alphainspect/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:45:54.876057 alphainspect-0.4.0/alphainspect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-05-15 16:45:54.000000 alphainspect-0.4.0/alphainspect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-15 16:45:54.000000 alphainspect-0.4.0/alphainspect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 16:45:54.000000 alphainspect-0.4.0/alphainspect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-15 16:45:54.000000 alphainspect-0.4.0/alphainspect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-15 16:45:54.000000 alphainspect-0.4.0/alphainspect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-15 16:45:50.000000 alphainspect-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 16:45:54.876057 alphainspect-0.4.0/setup.cfg
```

### Comparing `alphainspect-0.3.1/LICENSE` & `alphainspect-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alphainspect-0.3.1/PKG-INFO` & `alphainspect-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphainspect
-Version: 0.3.1
+Version: 0.4.0
 Summary: factor performance visualization
 Author-email: wukan <wu-kan@163.com>
 License: MIT License
         
         Copyright (c) 2024 wukan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -96,21 +96,21 @@
     1. `alphalens`的各参数要弄懂还是很麻烦的，初学者如绩效达不到要求就得深入研究源代码找原因
     2. `alphainspect`用户在外可以一次性全计算好，如`F1_ORG, F1_ZS, F1_NEUT`，然后在分别传不同因子进行比较即可
 3. 资金分配只用等权
     1. `alphalens`有因子加权、多空等设置
     2. `alphainspect`只提供等权一种计算方法，实现简单
 4. 收益率计算方法不同
     1. `alphalens`多期简单收益率几何平均成1期，然后+1累乘
-    2. `alphainspect`由用户提供1期简单收益率，然后根据要求持有或调仓，得到新的权益，循环迭代下去。更精确
+    2. ~~`alphainspect`由用户提供1期简单收益率，然后根据要求持有或调仓，得到新的权益，循环迭代下去。更精确~~
+    3. `alphainspect`由用户提供每期收益率(也可以使用多期收益率的几何平均),然后累加。（分层计算速度提高1倍）
 
 ## `alphainspect`与`alphalens`的相同
 
 1. 数据组织方式相同。都是长表，都是因子不移动，收益率计算，然后后移到与因子产生时间对齐
-2. 累计收益计算模式类似。每期产生因子，持有时长超过一期，都是将资金分成多份分别入场
-3. 不考虑滑点和手续费。单因子是用来合成多因子的，因手续费和滑点而错过部分单因子就可惜了，应当在因子合成后的回测阶段才考虑手续费
+2. 不考虑滑点和手续费。单因子是用来合成多因子的，因手续费和滑点而错过部分单因子就可惜了，应当在因子合成后的回测阶段才考虑手续费
 
 ## 二次开发
 
 ```commandline
 git --clone https://github.com/wukan1986/alphainspect.git
 cd alphainspect
 pip install -e .
```

### Comparing `alphainspect-0.3.1/README.md` & `alphainspect-0.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -51,21 +51,21 @@
     1. `alphalens`的各参数要弄懂还是很麻烦的，初学者如绩效达不到要求就得深入研究源代码找原因
     2. `alphainspect`用户在外可以一次性全计算好，如`F1_ORG, F1_ZS, F1_NEUT`，然后在分别传不同因子进行比较即可
 3. 资金分配只用等权
     1. `alphalens`有因子加权、多空等设置
     2. `alphainspect`只提供等权一种计算方法，实现简单
 4. 收益率计算方法不同
     1. `alphalens`多期简单收益率几何平均成1期，然后+1累乘
-    2. `alphainspect`由用户提供1期简单收益率，然后根据要求持有或调仓，得到新的权益，循环迭代下去。更精确
+    2. ~~`alphainspect`由用户提供1期简单收益率，然后根据要求持有或调仓，得到新的权益，循环迭代下去。更精确~~
+    3. `alphainspect`由用户提供每期收益率(也可以使用多期收益率的几何平均),然后累加。（分层计算速度提高1倍）
 
 ## `alphainspect`与`alphalens`的相同
 
 1. 数据组织方式相同。都是长表，都是因子不移动，收益率计算，然后后移到与因子产生时间对齐
-2. 累计收益计算模式类似。每期产生因子，持有时长超过一期，都是将资金分成多份分别入场
-3. 不考虑滑点和手续费。单因子是用来合成多因子的，因手续费和滑点而错过部分单因子就可惜了，应当在因子合成后的回测阶段才考虑手续费
+2. 不考虑滑点和手续费。单因子是用来合成多因子的，因手续费和滑点而错过部分单因子就可惜了，应当在因子合成后的回测阶段才考虑手续费
 
 ## 二次开发
 
 ```commandline
 git --clone https://github.com/wukan1986/alphainspect.git
 cd alphainspect
 pip install -e .
```

### Comparing `alphainspect-0.3.1/alphainspect/_nb.py` & `alphainspect-0.4.0/alphainspect/_nb.py`

 * *Files identical despite different names*

### Comparing `alphainspect-0.3.1/alphainspect/dtree.py` & `alphainspect-0.4.0/alphainspect/dtree.py`

 * *Files identical despite different names*

### Comparing `alphainspect-0.3.1/alphainspect/events.py` & `alphainspect-0.4.0/alphainspect/events.py`

 * *Files identical despite different names*

### Comparing `alphainspect-0.3.1/alphainspect/ic.py` & `alphainspect-0.4.0/alphainspect/ic.py`

 * *Files identical despite different names*

### Comparing `alphainspect-0.3.1/alphainspect/portfolio.py` & `alphainspect-0.4.0/alphainspect/portfolio.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-from typing import Optional
+from typing import Tuple
 
 import numpy as np
 import pandas as pd
 import polars as pl
+import polars.selectors as cs
 from loguru import logger
 from matplotlib import pyplot as plt
 
 from alphainspect import _QUANTILE_, _DATE_, _ASSET_, _WEIGHT_
 from alphainspect.utils import cumulative_returns, plot_heatmap
 
 
-def calc_cum_return_by_quantile(df_pl: pl.DataFrame, fwd_ret_1: str, period: int = 5, factor_quantile: str = _QUANTILE_) -> pd.DataFrame:
+def _calc_cum_return_by_quantile(df_pl: pl.DataFrame, fwd_ret_1: str, period: int = 5, factor_quantile: str = _QUANTILE_) -> pd.DataFrame:
     """分层计算收益。分成N层，层内等权"""
     q_max = df_pl.select(pl.max(factor_quantile)).to_series(0)[0]
     rr = df_pl.pivot(index=_DATE_, columns=_ASSET_, values=fwd_ret_1, aggregate_function='first', sort_columns=True).sort(_DATE_)
     qq = df_pl.pivot(index=_DATE_, columns=_ASSET_, values=factor_quantile, aggregate_function='first', sort_columns=True).sort(_DATE_)
 
     out = pd.DataFrame(index=rr[_DATE_])
     rr = rr.select(pl.exclude(_DATE_)).to_numpy() + 1  # 日收益
@@ -31,14 +32,33 @@
         out[f'G{i}'] = cumulative_returns(rr, w, funds=period, freq=period)
     # !!!直接减是错误的，因为两资金是独立的，资金减少的一份由于资金不足对冲比例已经不再是1:1
     # out['spread'] = out[f'G{q_max}'] - out[f'G0']
     logger.info('累计收益计算完成,period={}\n{}', period, out.tail(1).to_string())
     return out
 
 
+def calc_cum_return_by_quantile(df_pl: pl.DataFrame, fwd_ret_1: str, factor_quantile: str = _QUANTILE_) -> Tuple[pd.DataFrame, pd.DataFrame, pd.DataFrame, pd.DataFrame]:
+    """分层计算收益。分成N层，层内等权
+
+    单利不加仓。不考虑手续费，不考虑资金不足，资金也不分多份。每天入场每天出场。
+    此项目只为了评价因子是否有效，在累计收益计算时是否精确并不重要，这里的目的只是为了分层清晰，更精确计算请用其它工具
+
+    在输入收益率时，即可以输入日频收益率，也可以输入几何平均后的收益率。
+
+    """
+    x = df_pl.filter(pl.col(factor_quantile) >= 0).group_by(factor_quantile, _DATE_).agg(pl.mean(fwd_ret_1))
+    y = x.pivot(index=_DATE_, columns=factor_quantile, values=fwd_ret_1, aggregate_function='first', sort_columns=True).sort(_DATE_)
+    ret = y.with_columns(cs.numeric().fill_nan(None))
+    cum = ret.with_columns(cs.numeric().fill_null(0).cum_sum()).to_pandas().set_index(_DATE_)
+    avg = ret.select(cs.numeric().mean()).to_pandas().iloc[0]
+    std = ret.select(cs.numeric().std(ddof=0)).to_pandas().iloc[0]
+    ret = ret.to_pandas().set_index(_DATE_)
+    return ret, cum, avg, std
+
+
 def calc_cum_return_spread(df_pl: pl.DataFrame, fwd_ret_1: str, period: int = 5, factor_quantile: str = _QUANTILE_) -> pd.DataFrame:
     """分层计算收益。分成N层，层内等权。
     取Top层和Bottom层。比较不同的计算方法多空收益的区别"""
 
     q_max = df_pl.select(pl.max(factor_quantile)).to_series(0)[0]
     rr = df_pl.pivot(index=_DATE_, columns=_ASSET_, values=fwd_ret_1, aggregate_function='first', sort_columns=True).sort(_DATE_).fill_nan(0)
     qq = df_pl.pivot(index=_DATE_, columns=_ASSET_, values=factor_quantile, aggregate_function='first', sort_columns=True).sort(_DATE_).fill_nan(-1)
@@ -93,18 +113,18 @@
     # 由于是每天换仓，所以不存在空头计算不准的问题
     out[:] = np.cumprod(rr * ww + 1, axis=0)
 
     logger.info('权重收益计算完成,period={}\n{}', period, out.tail(1).to_string())
     return out
 
 
-def plot_quantile_portfolio(df_pd: pd.DataFrame, fwd_ret_1: str, period: int = 5,
+def plot_quantile_portfolio(df_pd: pd.DataFrame, fwd_ret_1: str,
                             *,
                             axvlines=None, ax=None) -> None:
-    ax = df_pd.plot(ax=ax, title=f'{fwd_ret_1}, period={period}', cmap='coolwarm', lw=1, grid=True)
+    ax = df_pd.plot(ax=ax, title=f'{fwd_ret_1}', cmap='coolwarm', lw=1, grid=True)
     ax.legend(loc='upper left')
     ax.set_xlabel('')
     for v in axvlines:
         ax.axvline(x=v, c="b", ls="--", lw=1)
 
 
 def plot_portfolio_heatmap_monthly(df_pd: pd.DataFrame,
@@ -119,49 +139,50 @@
     out = out.groupby(by=['year', 'month']).agg({'first': 'first', 'last': 'last'})
     out['cum_ret'] = out['last'] / out['first'] - 1
     plot_heatmap(out['cum_ret'].unstack(), title=f"{group},Monthly Return", ax=ax)
 
 
 def create_portfolio1_sheet(df_pl: pl.DataFrame,
                             fwd_ret_1: str,
-                            period=5,
                             factor_quantile: str = _QUANTILE_,
                             *,
                             axvlines=()) -> None:
     """分层累计收益图"""
     # 分层累计收益
-    df_cum_ret = calc_cum_return_by_quantile(df_pl, fwd_ret_1, period, factor_quantile)
+    ret, cum, avg, std = calc_cum_return_by_quantile(df_pl, fwd_ret_1, factor_quantile)
 
     fig, axes = plt.subplots(2, 1, figsize=(12, 9))
-    plot_quantile_portfolio(df_cum_ret, fwd_ret_1, period, axvlines=axvlines, ax=axes[0])
-    groups = df_cum_ret.columns[[0, -1]]
+    plot_quantile_portfolio(cum, fwd_ret_1, axvlines=axvlines, ax=axes[0])
+    groups = cum.columns[[0, -1]]
     for i, g in enumerate(groups):
         ax = plt.subplot(223 + i)
         # 月度收益
-        plot_portfolio_heatmap_monthly(df_cum_ret, group=g, ax=ax)
+        plot_portfolio_heatmap_monthly(cum, group=g, ax=ax)
     fig.tight_layout()
 
     # 多空累计收益
-    df_spread = calc_cum_return_spread(df_pl, fwd_ret_1, period, factor_quantile=factor_quantile)
+    df_spread = ret.iloc[:, [0, -1]].copy()
+    df_spread['LS'] = df_spread.iloc[:, -1] - df_spread.iloc[:, 0]
+    df_spread = df_spread.cumsum()
     fig, axes = plt.subplots(1, 1, figsize=(12, 9))
-    plot_quantile_portfolio(df_spread, fwd_ret_1, period, axvlines=axvlines, ax=axes)
+    plot_quantile_portfolio(df_spread, fwd_ret_1, axvlines=axvlines, ax=axes)
     fig.tight_layout()
 
 
 def create_portfolio2_sheet(df_pl: pl.DataFrame,
                             fwd_ret_1: str,
                             *,
                             axvlines=()) -> None:
     """分资产收益。权重由外部指定，资金是隔离"""
     # 各资产收益，如果资产数量过多，图会比较卡顿
     df_cum_ret = calc_cum_return_weights(df_pl, fwd_ret_1, 1)
 
     fig, axes = plt.subplots(2, 1, figsize=(12, 9), squeeze=False)
     axes = axes.flatten()
     # 分资产收益
-    plot_quantile_portfolio(df_cum_ret, fwd_ret_1, 1, axvlines=axvlines, ax=axes[0])
+    plot_quantile_portfolio(df_cum_ret, fwd_ret_1, axvlines=axvlines, ax=axes[0])
 
     # 资产平均收益，相当于等权
     s = df_cum_ret.mean(axis=1)
     s.name = 'portfolio'
-    plot_quantile_portfolio(s, fwd_ret_1, 1, axvlines=axvlines, ax=axes[1])
+    plot_quantile_portfolio(s, fwd_ret_1, axvlines=axvlines, ax=axes[1])
     fig.tight_layout()
```

### Comparing `alphainspect-0.3.1/alphainspect/reports.py` & `alphainspect-0.4.0/alphainspect/reports.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,17 +10,16 @@
 
 有不同观点的朋友可以提issue
 
 """
 import base64
 import io
 import os
-from math import ceil
 from pathlib import Path
-from typing import Sequence, Tuple, Any, Optional
+from typing import Sequence, Tuple, Any
 
 import polars as pl
 from loguru import logger  # noqa
 from matplotlib import pyplot as plt
 
 from alphainspect import _QUANTILE_
 from alphainspect.ic import calc_ic, plot_ic_ts, plot_ic_heatmap_monthly
@@ -117,30 +116,27 @@
     return ret
 
 
 def create_2x2_sheet(df_pl: pl.DataFrame,
                      factor: str,
                      forward_return: str, fwd_ret_1: str,
                      *,
-                     period: int = 5,
                      factor_quantile: str = _QUANTILE_,
                      figsize=(12, 9),
                      axvlines: Sequence[str] = ()) -> None:
     """画2*2的图表。含IC时序、IC直方图、IC热力图、累积收益图
 
     Parameters
     ----------
     df_pl
     factor
     forward_return: str
         用于记算IC的远期收益率
     fwd_ret_1:str
         用于记算累计收益的1期远期收益率
-    period: int
-        累计收益时持仓天数与资金份数
     factor_quantile:str
     figsize
 
     axvlines
 
     """
     fig, axes = plt.subplots(2, 2, figsize=figsize, squeeze=False)
@@ -153,40 +149,37 @@
     plot_ic_ts(df_ic, col, axvlines=axvlines, ax=axes[0])
     plot_ic_heatmap_monthly(df_ic, col, ax=axes[1])
 
     # 画因子直方图
     plot_hist(df_pl, factor, ax=axes[2])
 
     # 画累计收益
-    df_cum_ret = calc_cum_return_by_quantile(df_pl, fwd_ret_1, period, factor_quantile)
-    plot_quantile_portfolio(df_cum_ret, fwd_ret_1, period, axvlines=axvlines, ax=axes[3])
+    ret, cum, avg, std = calc_cum_return_by_quantile(df_pl, fwd_ret_1, factor_quantile)
+    plot_quantile_portfolio(cum, fwd_ret_1, axvlines=axvlines, ax=axes[3])
 
     fig.tight_layout()
 
 
 def create_1x3_sheet(df_pl: pl.DataFrame,
                      factor: str,
                      forward_return: str, fwd_ret_1: str,
                      *,
-                     period: int = 5,
                      factor_quantile: str = _QUANTILE_,
                      figsize=(12, 4),
-                     axvlines: Sequence[str] = ()) -> Tuple[Any, Any, Any, Any]:
+                     axvlines: Sequence[str] = ()) -> Tuple[Any, Any, Any, Any, Any, Any]:
     """画2*2的图表。含IC时序、IC直方图、IC热力图、累积收益图
 
     Parameters
     ----------
     df_pl
     factor
     forward_return: str
         用于记算IC的远期收益率
     fwd_ret_1:str
         用于记算累计收益的1期远期收益率
-    period: int
-        累计收益时持仓天数与资金份数
     factor_quantile:str
     figsize
 
     axvlines
 
     """
     fig, axes = plt.subplots(1, 3, figsize=figsize, squeeze=False)
@@ -195,91 +188,44 @@
     # 画IC信息
     # logger.info('计算IC')
     df_ic = calc_ic(df_pl, [factor], [forward_return])
     col = df_ic.columns[1]
     ic_dict = plot_ic_ts(df_ic, col, axvlines=axvlines, ax=axes[0])
 
     # 画累计收益
-    df_cum_ret = calc_cum_return_by_quantile(df_pl, fwd_ret_1, period, factor_quantile)
-    plot_quantile_portfolio(df_cum_ret, fwd_ret_1, period, axvlines=axvlines, ax=axes[1])
+    ret, cum, avg, std = calc_cum_return_by_quantile(df_pl, fwd_ret_1, factor_quantile)
+
+    plot_quantile_portfolio(cum, fwd_ret_1, axvlines=axvlines, ax=axes[1])
 
     # 画因子直方图
     hist_dict = plot_hist(df_pl, factor, ax=axes[2])
 
     fig.tight_layout()
 
-    return fig, ic_dict, hist_dict, df_cum_ret
-
-
-def create_2x3_sheet(df_pl: pl.DataFrame,
-                     factor: str,
-                     forward_return: str, fwd_ret_1: str,
-                     *,
-                     periods: Tuple = (2, 5, 10),
-                     factor_quantile: str = _QUANTILE_,
-                     figsize=(12, 9),
-                     axvlines: Sequence[str] = ()) -> None:
-    """画2*2的图表。含IC时序、IC直方图、IC热力图、累积收益图
-
-    Parameters
-    ----------
-    df_pl
-    factor
-    forward_return: str
-        用于记算IC的远期收益率
-    fwd_ret_1:str
-        用于记算累计收益的1期远期收益率
-    periods:Tuple
-        累计收益时持仓天数与资金份数
-    factor_quantile: str
-    axvlines
-
-    """
-    count = len(periods) + 3
-    fig, axes = plt.subplots(2, ceil(count / 2), figsize=figsize, squeeze=False)
-    axes = axes.flatten()
-
-    # 画IC信息
-    # logger.info('计算IC')
-    df_ic = calc_ic(df_pl, [factor], [forward_return])
-    col = df_ic.columns[1]
-    plot_ic_ts(df_ic, col, axvlines=axvlines, ax=axes[0])
-    plot_hist(df_ic, col, ax=axes[1])
-    plot_ic_heatmap_monthly(df_ic, col, ax=axes[2])
-
-    # 画累计收益
-    # logger.info('计算累计收益')
-    for i, period in enumerate(periods):
-        df_cum_ret = calc_cum_return_by_quantile(df_pl, fwd_ret_1, period, factor_quantile)
-        plot_quantile_portfolio(df_cum_ret, fwd_ret_1, period, axvlines=axvlines, ax=axes[3 + i])
-
-    fig.tight_layout()
+    return fig, ic_dict, hist_dict, cum, avg, std
 
 
 def create_3x2_sheet(df_pl: pl.DataFrame,
                      factor: str,
                      forward_return: str, fwd_ret_1: str,
                      *,
-                     period: int = 5,
                      factor_quantile: str = _QUANTILE_,
                      periods: Sequence[int] = (1, 5, 10, 20),
                      figsize=(12, 14),
                      axvlines: Sequence[str] = ()) -> None:
     """画2*3图
 
     Parameters
     ----------
     df_pl
     factor
     forward_return: str
         用于记算IC的远期收益率
     fwd_ret_1:str
         用于记算累计收益的1期远期收益率
-    period: int
-        累计收益时持仓天数与资金份数
     periods:
         换手率，多期比较
     factor_quantile:str
     axvlines
 
     """
     fig, axes = plt.subplots(3, 2, figsize=figsize)
@@ -290,16 +236,16 @@
     col = df_ic.columns[1]
     plot_ic_ts(df_ic, col, axvlines=axvlines, ax=axes[0, 0])
     plot_hist(df_ic, col, ax=axes[0, 1])
     plot_ic_heatmap_monthly(df_ic, col, ax=axes[1, 0])
 
     # 画净值曲线
     # logger.info('计算累计收益')
-    df_cum_ret = calc_cum_return_by_quantile(df_pl, fwd_ret_1, period, factor_quantile)
-    plot_quantile_portfolio(df_cum_ret, fwd_ret_1, period, axvlines=axvlines, ax=axes[1, 1])
+    ret, cum, avg, std = calc_cum_return_by_quantile(df_pl, fwd_ret_1, factor_quantile)
+    plot_quantile_portfolio(cum, fwd_ret_1, axvlines=axvlines, ax=axes[1, 1])
 
     # 画换手率
     # logger.info('计算换手率')
     df_auto_corr = calc_auto_correlation(df_pl, factor, periods=periods)
     df_turnover = calc_quantile_turnover(df_pl, periods=periods, factor_quantile=factor_quantile)
     plot_factor_auto_correlation(df_auto_corr, axvlines=axvlines, ax=axes[2, 0])
```

### Comparing `alphainspect-0.3.1/alphainspect/returns.py` & `alphainspect-0.4.0/alphainspect/returns.py`

 * *Files identical despite different names*

### Comparing `alphainspect-0.3.1/alphainspect/selection.py` & `alphainspect-0.4.0/alphainspect/selection.py`

 * *Files identical despite different names*

### Comparing `alphainspect-0.3.1/alphainspect/turnover.py` & `alphainspect-0.4.0/alphainspect/turnover.py`

 * *Files identical despite different names*

### Comparing `alphainspect-0.3.1/alphainspect/utils.py` & `alphainspect-0.4.0/alphainspect/utils.py`

 * *Files identical despite different names*

### Comparing `alphainspect-0.3.1/alphainspect.egg-info/PKG-INFO` & `alphainspect-0.4.0/alphainspect.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphainspect
-Version: 0.3.1
+Version: 0.4.0
 Summary: factor performance visualization
 Author-email: wukan <wu-kan@163.com>
 License: MIT License
         
         Copyright (c) 2024 wukan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -96,21 +96,21 @@
     1. `alphalens`的各参数要弄懂还是很麻烦的，初学者如绩效达不到要求就得深入研究源代码找原因
     2. `alphainspect`用户在外可以一次性全计算好，如`F1_ORG, F1_ZS, F1_NEUT`，然后在分别传不同因子进行比较即可
 3. 资金分配只用等权
     1. `alphalens`有因子加权、多空等设置
     2. `alphainspect`只提供等权一种计算方法，实现简单
 4. 收益率计算方法不同
     1. `alphalens`多期简单收益率几何平均成1期，然后+1累乘
-    2. `alphainspect`由用户提供1期简单收益率，然后根据要求持有或调仓，得到新的权益，循环迭代下去。更精确
+    2. ~~`alphainspect`由用户提供1期简单收益率，然后根据要求持有或调仓，得到新的权益，循环迭代下去。更精确~~
+    3. `alphainspect`由用户提供每期收益率(也可以使用多期收益率的几何平均),然后累加。（分层计算速度提高1倍）
 
 ## `alphainspect`与`alphalens`的相同
 
 1. 数据组织方式相同。都是长表，都是因子不移动，收益率计算，然后后移到与因子产生时间对齐
-2. 累计收益计算模式类似。每期产生因子，持有时长超过一期，都是将资金分成多份分别入场
-3. 不考虑滑点和手续费。单因子是用来合成多因子的，因手续费和滑点而错过部分单因子就可惜了，应当在因子合成后的回测阶段才考虑手续费
+2. 不考虑滑点和手续费。单因子是用来合成多因子的，因手续费和滑点而错过部分单因子就可惜了，应当在因子合成后的回测阶段才考虑手续费
 
 ## 二次开发
 
 ```commandline
 git --clone https://github.com/wukan1986/alphainspect.git
 cd alphainspect
 pip install -e .
```

### Comparing `alphainspect-0.3.1/pyproject.toml` & `alphainspect-0.4.0/pyproject.toml`

 * *Files identical despite different names*

