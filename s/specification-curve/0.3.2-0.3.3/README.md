# Comparing `tmp/specification_curve-0.3.2.tar.gz` & `tmp/specification_curve-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specification_curve-0.3.2.tar", max compression
+gzip compressed data, was "specification_curve-0.3.3.tar", max compression
```

## Comparing `specification_curve-0.3.2.tar` & `specification_curve-0.3.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2023-07-24 18:50:43.107216 specification_curve-0.3.2/LICENSE
--rw-r--r--   0        0        0     5238 2023-07-24 18:50:43.107216 specification_curve-0.3.2/README.md
--rw-r--r--   0        0        0     1940 2023-07-24 18:51:03.263249 specification_curve-0.3.2/pyproject.toml
--rw-r--r--   0        0        0    22827 2023-07-24 18:50:43.111216 specification_curve-0.3.2/src/specification_curve/__init__.py
--rw-r--r--   0        0        0       27 2023-07-24 18:50:43.111216 specification_curve-0.3.2/src/specification_curve/__main__.py
--rw-r--r--   0        0        0    57372 2023-07-24 18:50:43.111216 specification_curve-0.3.2/src/specification_curve/data/example_data.csv
--rw-r--r--   0        0        0     6273 1970-01-01 00:00:00.000000 specification_curve-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-16 18:10:30.961781 specification_curve-0.3.3/LICENSE
+-rw-r--r--   0        0        0     3581 2024-05-16 18:10:30.961781 specification_curve-0.3.3/README.md
+-rw-r--r--   0        0        0     1999 2024-05-16 18:10:41.337858 specification_curve-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0    24083 2024-05-16 18:10:30.965782 specification_curve-0.3.3/src/specification_curve/__init__.py
+-rw-r--r--   0        0        0       27 2024-05-16 18:10:30.965782 specification_curve-0.3.3/src/specification_curve/__main__.py
+-rw-r--r--   0        0        0    57372 2024-05-16 18:10:30.965782 specification_curve-0.3.3/src/specification_curve/data/example_data.csv
+-rw-r--r--   0        0        0     4647 1970-01-01 00:00:00.000000 specification_curve-0.3.3/PKG-INFO
```

### Comparing `specification_curve-0.3.2/LICENSE` & `specification_curve-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `specification_curve-0.3.2/README.md` & `specification_curve-0.3.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,114 +1,83 @@
+Metadata-Version: 2.1
+Name: specification_curve
+Version: 0.3.3
+Summary: Specification_Curve
+Home-page: https://aeturrell.github.io/specification_curve/
+License: MIT
+Author: aeturrell
+Author-email: mail@mail.com
+Requires-Python: >=3.9,<3.12
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: matplotlib (>=3.6.1,<4.0.0)
+Requires-Dist: numpy (>=1.26.4,<2.0.0)
+Requires-Dist: pandas (>=2.0.3,<3.0.0)
+Requires-Dist: statsmodels (>=0.14.0,<0.15.0)
+Requires-Dist: typeguard (>=4.2.1,<5.0.0)
+Requires-Dist: types-setuptools (>=67.6,<70.0)
+Project-URL: Changelog, https://github.com/aeturrell/specification_curve/releases
+Project-URL: Documentation, https://aeturrell.github.io/specification_curve/
+Project-URL: Repository, https://github.com/aeturrell/specification_curve
+Description-Content-Type: text/markdown
+
 # Specification Curve
 
-Specification Curve is a Python package that performs specification curve analysis; it helps with the problem of the "garden of forking paths" (many defensible choices) when doing analysis by running many regressions and summarising the effects in an easy to digest chart.
+Specification Curve is a Python package that performs specification curve analysis; it helps with the problem of the "garden of forking paths" (many defensible choices) when doing analysis by running many regressions and summarising the estimated coefficients in an easy to digest chart.
 
 [![PyPI](https://img.shields.io/pypi/v/specification_curve.svg)](https://pypi.org/project/specification_curve/)
 [![Status](https://img.shields.io/pypi/status/specification_curve.svg)](https://pypi.org/project/specification_curve/)
 [![Python Version](https://img.shields.io/pypi/pyversions/specification_curve)](https://pypi.org/project/specification_curve)
 [![License](https://img.shields.io/pypi/l/specification_curve)](https://opensource.org/licenses/MIT)
 [![Tests](https://github.com/aeturrell/specification_curve/workflows/Tests/badge.svg)](https://github.com/aeturrell/specification_curve/actions?workflow=Tests)
 [![Codecov](https://codecov.io/gh/aeturrell/specification_curve/branch/main/graph/badge.svg)](https://codecov.io/gh/aeturrell/specification_curve)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
-[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/aeturrell/438fb066e4471312667268669cef2c11/specification_curve-examples.ipynb)
+[![Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/aeturrell/specification_curve/blob/master/docs/features.ipynb)
 [![DOI](https://zenodo.org/badge/282989537.svg)](https://zenodo.org/badge/latestdoi/282989537)
 [![Downloads](https://static.pepy.tech/badge/specification-curve)](https://pepy.tech/project/Specification_curve)
 
 ![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
 ![macOS](https://img.shields.io/badge/mac%20os-000000?style=for-the-badge&logo=macos&logoColor=F0F0F0)
 ![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)
 
 [![Source](https://img.shields.io/badge/source%20code-github-lightgrey?style=for-the-badge)](https://github.com/aeturrell/specification_curve)
 
 [Go to the full documentation for **Specification Curve**](https://aeturrell.github.io/specification_curve/).
 
 ## Quickstart
 
-You can try out specification curve right now in [Google Colab](https://colab.research.google.com/gist/aeturrell/438fb066e4471312667268669cef2c11/specification_curve-examples.ipynb).
-
-Here's an example of using **Specification Curve**.
-
-```python
-# import specification curve
-import specification_curve as specy
-
-
-# Generate some fake data
-# ------------------------
-import numpy as np
-import pandas as pd
-# Set seed for random numbers
-seed_for_prng = 78557
-# prng=probabilistic random number generator
-prng = np.random.default_rng(seed_for_prng)
-n_samples = 400
-# Number of dimensions
-n_dim = 4
-c_rnd_vars = prng.random(size=(n_dim, n_samples))
-y_1 = (0.4*c_rnd_vars[0, :] -  # THIS IS THE TRUE VALUE OF THE COEFFICIENT
-       0.2*c_rnd_vars[1, :] +
-       0.3*prng.standard_normal(n_samples))
-# Next line causes y_2 ests to be much more noisy
-y_2 = y_1 - 0.5*np.abs(prng.standard_normal(n_samples))
-# Put data into dataframe
-df = pd.DataFrame([y_1, y_2], ['y1', 'y2']).T
-df["x_1"] = c_rnd_vars[0, :]
-df["c_1"] = c_rnd_vars[1, :]
-df["c_2"] = c_rnd_vars[2, :]
-df["c_3"] = c_rnd_vars[3, :]
-
-# Specification Curve Analysis
-#-----------------------------
-sc = specy.SpecificationCurve(
-    df,
-    y_endog=['y1', 'y2'],
-    x_exog="x_1",
-    controls=["c_1", "c_2", "c_3"])
-sc.fit()
-sc.plot()
-```
+You can try out specification curve right now in [Google Colab](https://colab.research.google.com/github/aeturrell/specification_curve/blob/master/docs/features.ipynb). To install the package in Colab, run `!pip install specification_curve` in a new code cell.
 
-Grey squares (black lines when there are many specifications) show whether a variable is included in a specification or not. Blue or red markers and error bars show whether the coefficient is positive and significant (at the 0.05 level) or red and significant, respectively.
+Alternatively you can see examples on the [features page](https://aeturrell.github.io/specification_curve/features.html) of the documentation.
 
 ## Installation
 
 You can install **Specification Curve** via pip:
 
 ```bash
-$ pip install specification-curve
+pip install specification-curve
 ```
 
 To install the development version from git, use:
 
 ```bash
-$ pip install git+https://github.com/aeturrell/specification_curve.git
+pip install git+https://github.com/aeturrell/specification_curve.git
 ```
 
 ## Citing Specification Curve
 
-```text
-@misc{aeturrell_2022_7264033,
-  author       = {Arthur Turrell},
-  title        = {Specification Curve: v0.3.1},
-  month        = oct,
-  year         = 2022,
-  publisher    = {Zenodo},
-  version      = {v0.3.1},
-  doi          = {10.5281/zenodo.7264033},
-  url          = {https://doi.org/10.5281/zenodo.7264033}
-}
-```
+You can find full citation information at the following link: [https://zenodo.org/badge/latestdoi/282989537](https://zenodo.org/badge/latestdoi/282989537).
 
 Using **Specification Curve** in your paper? Let us know by raising an issue beginning with "citation".
 
 ## License
 
 Distributed under the terms of the [MIT license](https://opensource.org/licenses/MIT).
 
-## Credits
-
-The package is built with [poetry](https://python-poetry.org/), while the documentation is built with [Jupyter Book](https://jupyterbook.org). Tests are run with [nox](https://nox.thea.codes/en/stable/).
-
 ## Similar Packages
 
 In RStats, there is [specr](https://github.com/masurp/specr) (which inspired many design choices in this package) and [spec_chart](https://github.com/ArielOrtizBobea/spec_chart). Some of the example data in this package is the same as in specr, but please note that results have not been cross-checked across packages.
+
```

### Comparing `specification_curve-0.3.2/pyproject.toml` & `specification_curve-0.3.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,64 +1,66 @@
 [tool.poetry]
 name = "specification_curve"
-version = "0.3.2"
+version = "0.3.3"
 description = "Specification_Curve"
 authors = ["aeturrell <mail@mail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://aeturrell.github.io/specification_curve/"
 repository = "https://github.com/aeturrell/specification_curve"
 documentation = "https://aeturrell.github.io/specification_curve/"
 classifiers = [
     "Development Status :: 3 - Alpha",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
 
 [tool.poetry.urls]
 Changelog = "https://github.com/aeturrell/specification_curve/releases"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
+python = ">=3.9,<3.12"
 pandas = "^2.0.3"
 statsmodels = "^0.14.0"
 matplotlib = "^3.6.1"
-types-setuptools = ">=67.6,<69.0"
+types-setuptools = ">=67.6,<70.0"
+numpy = "^1.26.4"
+typeguard = "^4.2.1"
 
 [tool.poetry.dev-dependencies]
 
 
 [tool.poetry.scripts]
 specification_curve = "specification_curve.__main__:main"
 
 
 [tool.poetry.group.dev.dependencies]
 coverage = "^7.2.7"
-black = "^23.7.0"
 pre-commit = "^3.3.3"
-Sphinx = "^4.0.0"
 typeguard = ">=3.0.2,<5.0.0"
-safety = "^2.3.4"
-pytest = "^7.4.0"
-flake8 = "^5.0.4"
+safety = ">=2.3.4,<4.0.0"
+pytest = ">=7.4,<9.0"
 pre-commit-hooks = "^4.4.0"
-nox = ">=2022.11.21,<2024.0.0"
+nox = ">=2022.11.21,<2025.0.0"
 ipykernel = "^6.22.0"
-nbstripout = "^0.6.1"
+nbstripout = ">=0.6.1,<0.8.0"
 jupyter-book = "^0.15.1"
-furo = "^2022.9.29"
+furo = ">=2022.9.29,<2024.0.0"
 ghp-import = "^2.1.0"
 xdoctest = "^1.1.1"
-mypy = "^1.2"
-reorder-python-imports = "^3.9.0"
+mypy = "1.10"
 sphinxcontrib-bibtex = "^2.5.0"
 types-pkg-resources = "^0.1.3"
-types-setuptools = ">=67.6,<69.0"
+types-setuptools = ">=67.6,<70.0"
 pandas-stubs = "^2.0.2.230605"
+ruff = "^0.4.4"
+nox-poetry = "^1.0.3"
+quartodoc = "^0.7.2"
+toml = "^0.10.2"
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
 
 [tool.coverage.run]
 branch = true
 source = ["specification_curve"]
```

### Comparing `specification_curve-0.3.2/src/specification_curve/__init__.py` & `specification_curve-0.3.3/src/specification_curve/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,51 +1,40 @@
 """
 Specification Curve
 -------------------
 A package that produces specification curve analysis.
 """
+
 import copy
 import itertools
 import os
 import typing
-from collections import Counter
-from collections import defaultdict
+from collections import Counter, defaultdict
+from importlib import resources
 from itertools import combinations
-from math import floor
-from math import log10
-from typing import DefaultDict
-from typing import Dict
-from typing import List
-from typing import Optional
-from typing import Set
-from typing import Tuple
-from typing import Union
+from math import floor, log10
+from typing import DefaultDict, List, Union
 
 import matplotlib.patches as patches
 import matplotlib.pyplot as plt
 import matplotlib.ticker as ticker
 import numpy as np
 import pandas as pd
-import pkg_resources
 import statsmodels.api as sm
+from typeguard import typeguard_ignore
 
 
-EXAMPLE_FILE = pkg_resources.resource_filename(
-    "specification_curve", os.path.join("data", "example_data.csv")
-)
-
-
-def _round_to_1(x: float) -> float:
-    """Rounds numbers to 1 s.f.
+def _round_to_2(x: float) -> float:
+    """Rounds numbers to 2 s.f.
     Args:
         x (float): input number
     Returns:
         float: number rounded
     """
-    return round(x, -int(floor(log10(abs(x)))) + 1)
+    return round(x, -int(floor(log10(abs(x)))) + 2)
 
 
 @typing.no_type_check
 def _double_list_check(XX: Union[List[str], List[List[str]]]) -> List[List[str]]:
     """Ensures that input is returned as nested list.
     Args:
         XX (Union[list[str], list[list[str]]]): Input list of (list of) strings
@@ -61,15 +50,15 @@
 def _single_list_check_str(X: Union[str, List[str]]) -> List[str]:
     """Ensures a list of strings.
     Args:
         X (Union[str, list[str]]): input string of list of strings
     Returns:
         list[str]: List of strings.
     """
-    if type(X) == str:
+    if isinstance(X, str):
         X = [X]
     return X
 
 
 def _remove_overlapping_vars(
     list_to_check: List[str], includes_list: List[str]
 ) -> List[str]:
@@ -116,18 +105,19 @@
             for comb in combinations(lst, r)
             if not any(e.issubset(comb) for e in excludes)
         ]
     else:
         return list(combinations(lst, r))
 
 
+@typeguard_ignore
 def _flatn_list(nested_list: Union[str, List[str], List[List[str]]]) -> List[str]:
     """Flattens nested list.
     Args:
-        nested_list (Union[List[str], List[List[str]]]): nested list
+        nested_list
     Returns:
         List[str]: flattened list
     """
     return list(itertools.chain.from_iterable(nested_list))
 
 
 class SpecificationCurve:
@@ -142,17 +132,17 @@
 
     def __init__(
         self,
         df: pd.DataFrame,
         y_endog: Union[str, List[str]],
         x_exog: Union[str, List[str]],
         controls: List[str],
-        exclu_grps: List[List[None]] = [[]],
-        cat_expand: Union[str, List[None]] = [],
-        always_include: List[str] = [],
+        exclu_grps: Union[List[List[None]], List[str], str, List[List[str]]] = [[None]],
+        cat_expand: Union[str, List[None], List[str], List[List[str]]] = [],
+        always_include: Union[str, List[str]] = [],
     ) -> None:
         """Specification curve object constructor.
         Args:
             df (pd.DataFrame): Data for regressions
             y_endog (Union[str, List[str]]): Endogeneous variables
             x_exog (Union[str, List[str]]): Exogeneous variables
             controls (List[str]): Conditioning variables
@@ -181,16 +171,19 @@
         self.controls = _remove_overlapping_vars(self.controls, self.always_include)
         self.x_exog = _remove_overlapping_vars(self.x_exog, self.always_include)
         self.ctrl_combs = self._compute_combinations()
         self.df_r = self._spec_curve_regression()
         print("Fit complete")
 
     def _reg_func(
-        self, y_endog: List[str], x_exog: str, reg_vars: List[str]
-    ) -> sm.regression.linear_model.RegressionResults:
+        self, y_endog: Union[str, List[str]], x_exog: str, reg_vars: List[str]
+    ) -> Union[
+        sm.regression.linear_model.RegressionResults,
+        sm.regression.linear_model.RegressionResultsWrapper,
+    ]:
         """Performs the regression.
         Args:
             y_endog (List[str]): Endogeneous variables
             x_exog (str): Exogeneous variables
             reg_vars (List[str]): Controls
         Returns:
             sm.regression.linear_model.RegressionResults: coefficients from reg
@@ -205,21 +198,17 @@
         # mypy prefers this formulation to a list comprehension
         for x in gone_cols:
             if x in reg_vars_here:
                 reg_vars_here.remove(x)
         # Ensure new cols are int so that statsmodels will run on them.
         # This is because statsmodels requires all values to be of either int or float dtype.
         # first get columns series with true or false depending on if not int or float stem to data type
-        non_int_or_float_cols = (
-            ~xf[reg_vars_here]
-            .dtypes.astype("string")
-            .str.split("[1-9][0-9]", regex=True)
-            .str[0]
-            .isin(["int", "float"])
-        )
+        non_int_or_float_cols = ~xf[reg_vars_here].dtypes.astype("string").str.split(
+            "[1-9][0-9]", regex=True
+        ).str[0].isin(["int", "float"])
         # now take only the trues from
         cols_to_convert_to_int = list(
             non_int_or_float_cols[non_int_or_float_cols].index
         )
         # convert just these columns to int
         for col_name in cols_to_convert_to_int:
             xf[col_name] = xf[col_name].astype(int)
@@ -332,26 +321,30 @@
         df_r = df_r.reset_index().drop("index", axis=1)
         df_r.index.names = ["Specification No."]
         df_r["Specification"] = df_r["Specification"].apply(lambda x: sorted(x))
         df_r["SpecificationCounts"] = df_r["Specification"].apply(lambda x: Counter(x))
         return df_r
 
     def plot(
-        self, save_path=None, pretty_plots: bool = True, preferred_spec: List[None] = []
+        self,
+        save_path=None,
+        pretty_plots: bool = True,
+        preferred_spec: Union[List[str], List[None]] = [],
     ) -> None:
         """Makes plots of fitted specification curve.
         Args:
             save_path (_type_, optional): Exported fig filename. Defaults to None.
             pretty_plots (bool, optional): whether to use this package's figure formatting. Defaults to True.
             preferred_spec (list, optional): preferred specification. Defaults to [].
         """
         if pretty_plots:
             _pretty_plots()
         # Set up blocks for showing what effects are included
         df_spec = self.df_r["SpecificationCounts"].apply(pd.Series).fillna(0.0)
+        pd.set_option("future.no_silent_downcasting", True)  # for the line below
         df_spec = df_spec.replace(0.0, False).replace(1.0, True)
         df_spec = df_spec.T
         df_spec = df_spec.sort_index()
         # Label the preferred specification as True
         self.df_r["preferred"] = False
         if preferred_spec:
             self.df_r["preferred"] = self.df_r["Specification"].apply(
@@ -476,16 +469,48 @@
                     arrowstyle="fancy", fc="0.4", ec="none", connectionstyle=cn_styl
                 ),
             )
         axarr[0].set_ylabel("Coefficient")
         axarr[0].set_title("Specification curve analysis")
         max_height = self.df_r["conf_int"].apply(lambda x: x.max()).max()
         min_height = self.df_r["conf_int"].apply(lambda x: x.min()).min()
-        ylims = (min_height / 1.2, 1.2 * max_height)
-        axarr[0].set_ylim(_round_to_1(ylims[0]), _round_to_1(ylims[1]))
+
+        def get_chart_axes_limits(height: float, max: bool) -> float:
+            """For positive numbers and max, returns height*axes_width_multiple.
+            For negative numbers and max, returns height/axes_width_multiple
+            max and max height > 0:
+            np.sign(height) = 1
+            height*exp(1*1*log(m)) = height*m
+            max and max height < 0:
+            np.sign(height) = -1
+            height*exp(-1*1*log(m)) = height/m
+            min and min height > 0:
+            np.sign(height) = 1
+            height*exp(1*-1*log(m)) = height/m
+            min and min height < 0
+            np.sign(height) = -1
+            height*exp(-1*-1*log(m)) = height*m
+
+            Args:
+                height (float): The height of the error bar
+
+            Returns:
+                float: limit
+            """
+            axes_width_multiple = 1.2
+            max_or_min_factor = 1 if max else -1
+            return height * np.exp(
+                np.sign(height) * max_or_min_factor * np.log(axes_width_multiple)
+            )
+
+        ylims = (
+            get_chart_axes_limits(min_height, False),
+            get_chart_axes_limits(max_height, True),
+        )
+        axarr[0].set_ylim(_round_to_2(ylims[0]), _round_to_2(ylims[1]))
         # Now do the blocks - each group get its own array
         wid = 0.5
         hei = wid / 2.5
         color_dict = {True: "#9B9B9B", False: "#F2F2F2"}
         if len(self.df_r) > 160:
             wid = 0.01
             color_dict = {True: "k", False: "#FFFFFF"}
@@ -511,15 +536,15 @@
                     )
                     ax.add_patch(sq)
             ax.xaxis.set_major_locator(ticker.MaxNLocator(integer=True))
             ax.yaxis.set_major_locator(ticker.MaxNLocator(integer=True))
             ax.set_yticks(range(len(list(df_sp_sl.index.values))))
             # Add text on the RHS that describes what each block is
             ax.text(
-                x=len(df_sp_sl.columns) + 1,
+                x=len(df_sp_sl.columns),
                 y=np.mean(ax.get_yticks()),
                 s=block_name_dict[
                     block_df.loc[block_df["group_index"] == ax_num, "group"].iloc[0]
                 ],
                 rotation=-90,
                 fontsize=11,
                 horizontalalignment="center",
@@ -542,15 +567,19 @@
 
 def load_example_data1() -> pd.DataFrame:
     """Retrieves example data from a file included with the package.
     Returns:
         pd.DataFrame: Example data suitable for regression.
     """
     # Example data
-    df = pd.read_csv(EXAMPLE_FILE, index_col=0)
+    ref = resources.files("specification_curve") / os.path.join(
+        "data", "example_data.csv"
+    )
+    with resources.as_file(ref) as path:
+        df = pd.read_csv(path, index_col=0)
     num_cols = [x for x in df.columns if x not in ["group1", "group2"]]
     for col in num_cols:
         df[col] = df[col].astype(np.double)
     cat_cols = [x for x in df.columns if x not in num_cols]
     for col in cat_cols:
         df[col] = df[col].astype("category")
     return df
```

### Comparing `specification_curve-0.3.2/src/specification_curve/data/example_data.csv` & `specification_curve-0.3.3/src/specification_curve/data/example_data.csv`

 * *Files identical despite different names*

