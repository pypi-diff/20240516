# Comparing `tmp/scores-0.8.tar.gz` & `tmp/scores-0.8.1.tar.gz`

## Comparing `scores-0.8.tar` & `scores-0.8.1.tar`

### file list

```diff
@@ -1,51 +1,52 @@
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 scores-0.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 scores-0.8/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 scores-0.8/environment.yml
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 scores-0.8/mkdocs.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scores-0.8/py.typed
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 scores-0.8/readthedocs.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scores-0.8/setup.cfg
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 scores-0.8/.binder/postBuild
--rw-r--r--   0        0        0     7409 2020-02-02 00:00:00.000000 scores-0.8/.binder/requirements.txt
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 scores-0.8/.github/pull_request_template.md
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 scores-0.8/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 scores-0.8/.github/ISSUE_TEMPLATE/new_score.md
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 scores-0.8/.github/workflows/python-app.yml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 scores-0.8/.github/workflows/run-pre-commit.yml
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 scores-0.8/src/scores/__init__.py
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 scores-0.8/src/scores/functions.py
--rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 scores-0.8/src/scores/sample_data.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 scores-0.8/src/scores/typing.py
--rw-r--r--   0        0        0    12735 2020-02-02 00:00:00.000000 scores-0.8/src/scores/utils.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 scores-0.8/src/scores/categorical/__init__.py
--rw-r--r--   0        0        0     6646 2020-02-02 00:00:00.000000 scores-0.8/src/scores/categorical/binary_impl.py
--rw-r--r--   0        0        0    21466 2020-02-02 00:00:00.000000 scores-0.8/src/scores/categorical/contingency_impl.py
--rw-r--r--   0        0        0    11009 2020-02-02 00:00:00.000000 scores-0.8/src/scores/categorical/multicategorical_impl.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 scores-0.8/src/scores/continuous/__init__.py
--rw-r--r--   0        0        0    18015 2020-02-02 00:00:00.000000 scores-0.8/src/scores/continuous/flip_flop_impl.py
--rw-r--r--   0        0        0    12571 2020-02-02 00:00:00.000000 scores-0.8/src/scores/continuous/murphy_impl.py
--rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 scores-0.8/src/scores/continuous/quantile_loss_impl.py
--rw-r--r--   0        0        0    16768 2020-02-02 00:00:00.000000 scores-0.8/src/scores/continuous/standard_impl.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 scores-0.8/src/scores/pandas/__init__.py
--rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 scores-0.8/src/scores/pandas/continuous.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 scores-0.8/src/scores/pandas/typing.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 scores-0.8/src/scores/probability/__init__.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 scores-0.8/src/scores/probability/brier_impl.py
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 scores-0.8/src/scores/probability/checks.py
--rw-r--r--   0        0        0    37967 2020-02-02 00:00:00.000000 scores-0.8/src/scores/probability/crps_impl.py
--rw-r--r--   0        0        0     6092 2020-02-02 00:00:00.000000 scores-0.8/src/scores/probability/roc_impl.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 scores-0.8/src/scores/processing/__init__.py
--rw-r--r--   0        0        0    12458 2020-02-02 00:00:00.000000 scores-0.8/src/scores/processing/discretise.py
--rw-r--r--   0        0        0    29482 2020-02-02 00:00:00.000000 scores-0.8/src/scores/processing/isoreg_impl.py
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 scores-0.8/src/scores/processing/matching.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 scores-0.8/src/scores/processing/cdf/__init__.py
--rw-r--r--   0        0        0    16430 2020-02-02 00:00:00.000000 scores-0.8/src/scores/processing/cdf/cdf_functions.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 scores-0.8/src/scores/stats/__init__.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 scores-0.8/src/scores/stats/statistical_tests/__init__.py
--rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 scores-0.8/src/scores/stats/statistical_tests/acovf.py
--rw-r--r--   0        0        0    17540 2020-02-02 00:00:00.000000 scores-0.8/src/scores/stats/statistical_tests/diebold_mariano_impl.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 scores-0.8/.gitignore
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 scores-0.8/LICENSE
--rw-r--r--   0        0        0     6670 2020-02-02 00:00:00.000000 scores-0.8/README.md
--rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 scores-0.8/pyproject.toml
--rw-r--r--   0        0        0     9392 2020-02-02 00:00:00.000000 scores-0.8/PKG-INFO
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 scores-0.8.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 scores-0.8.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 scores-0.8.1/environment.yml
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 scores-0.8.1/mkdocs.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scores-0.8.1/py.typed
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 scores-0.8.1/readthedocs.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scores-0.8.1/setup.cfg
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 scores-0.8.1/.binder/postBuild
+-rw-r--r--   0        0        0     7409 2020-02-02 00:00:00.000000 scores-0.8.1/.binder/requirements.txt
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 scores-0.8.1/.github/pull_request_template.md
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 scores-0.8.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 scores-0.8.1/.github/ISSUE_TEMPLATE/new_score.md
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 scores-0.8.1/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 scores-0.8.1/.github/workflows/run-pre-commit.yml
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/__init__.py
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/functions.py
+-rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/sample_data.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/typing.py
+-rw-r--r--   0        0        0    12725 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/utils.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/categorical/__init__.py
+-rw-r--r--   0        0        0     6646 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/categorical/binary_impl.py
+-rw-r--r--   0        0        0    21558 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/categorical/contingency_impl.py
+-rw-r--r--   0        0        0    11009 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/categorical/multicategorical_impl.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/continuous/__init__.py
+-rw-r--r--   0        0        0    18015 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/continuous/flip_flop_impl.py
+-rw-r--r--   0        0        0    12571 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/continuous/murphy_impl.py
+-rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/continuous/quantile_loss_impl.py
+-rw-r--r--   0        0        0    16768 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/continuous/standard_impl.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/emerging/__init__.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/pandas/__init__.py
+-rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/pandas/continuous.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/pandas/typing.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/probability/__init__.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/probability/brier_impl.py
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/probability/checks.py
+-rw-r--r--   0        0        0    37967 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/probability/crps_impl.py
+-rw-r--r--   0        0        0     6092 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/probability/roc_impl.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/processing/__init__.py
+-rw-r--r--   0        0        0    12438 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/processing/discretise.py
+-rw-r--r--   0        0        0    29482 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/processing/isoreg_impl.py
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/processing/matching.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/processing/cdf/__init__.py
+-rw-r--r--   0        0        0    16430 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/processing/cdf/cdf_functions.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/stats/__init__.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/stats/statistical_tests/__init__.py
+-rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/stats/statistical_tests/acovf.py
+-rw-r--r--   0        0        0    17540 2020-02-02 00:00:00.000000 scores-0.8.1/src/scores/stats/statistical_tests/diebold_mariano_impl.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 scores-0.8.1/.gitignore
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 scores-0.8.1/LICENSE
+-rw-r--r--   0        0        0     6776 2020-02-02 00:00:00.000000 scores-0.8.1/README.md
+-rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 scores-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     9500 2020-02-02 00:00:00.000000 scores-0.8.1/PKG-INFO
```

### Comparing `scores-0.8/.pre-commit-config.yaml` & `scores-0.8.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scores-0.8/CODE_OF_CONDUCT.md` & `scores-0.8.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `scores-0.8/readthedocs.yaml` & `scores-0.8.1/readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `scores-0.8/.binder/requirements.txt` & `scores-0.8.1/.binder/requirements.txt`

 * *Files identical despite different names*

### Comparing `scores-0.8/.github/pull_request_template.md` & `scores-0.8.1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `scores-0.8/.github/ISSUE_TEMPLATE/feature_request.md` & `scores-0.8.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `scores-0.8/.github/ISSUE_TEMPLATE/new_score.md` & `scores-0.8.1/.github/ISSUE_TEMPLATE/new_score.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ---
-name: New Score or Metric
-about: Suggest a new score or metric which could be added to the repository
+name: Request a new metric, statistical test, or tool
+about: Suggest a new metric, statistical test, or tool which could be added to the repository
 
 ---
 
-**I would like the following metric or statistical test to be considered for addition to the `scores` repository**  
-Please briefly describe the metric or statistical test and why you think it would be useful.
+**I would like the following metric, statistical test or data processing tool to be considered for addition to the `scores` repository**  
+Please briefly describe the metric, statistical test, or tool and why you think it would be useful.
 
-**Please provide a reference that describes the metric or statistical test**  
+**Please provide a reference that describes the metric, statistical test or data processing tool**  
 Note: if the reference includes multiple versions of the metric, and you are interested in a specific version, please note that (e.g. specify which theorem or corollary). 
 
-**(Please delete this section if not applicable) I intend to submit a pull request for the new metric or statistical test**
-- [ ] Please read the [Contributing Guide,](https://scores.readthedocs.io/en/develop/contributing.html#contributing-guide) in particular the [Development Process for a New Score or Metric](https://scores.readthedocs.io/en/develop/contributing.html#development-process-for-a-new-score-or-metric) section
+**(Please delete this section if not applicable) I intend to submit a pull request for the new metric, statistical test or data processing tool**
+- [ ] Please read the [Contributing Guide](https://scores.readthedocs.io/en/latest/contributing.html#contributing-guide), in particular the [Development Process for a New Score or Metric](https://scores.readthedocs.io/en/latest/contributing.html#development-process-for-a-new-score-or-metric) section
 - [ ] Please read the [pull request checklist](https://github.com/nci/scores/blob/develop/.github/pull_request_template.md)
 - [ ] I understand that, due to practical constraints, it may not always be possible for a metric or statistical test to be added
```

### Comparing `scores-0.8/.github/workflows/python-app.yml` & `scores-0.8.1/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `scores-0.8/.github/workflows/run-pre-commit.yml` & `scores-0.8.1/.github/workflows/run-pre-commit.yml`

 * *Files identical despite different names*

### Comparing `scores-0.8/src/scores/__init__.py` & `scores-0.8.1/src/scores/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import scores.functions
 import scores.pandas
 import scores.probability
 import scores.processing
 import scores.sample_data
 import scores.stats.statistical_tests  # noqa: F401
 
-__version__ = "0.8"
+__version__ = "0.8.1"
 
 __all__ = [
     "scores.categorical",
     "scores.contingency",
     "scores.continuous",
     "scores.functions",
     "scores.pandas",
```

### Comparing `scores-0.8/src/scores/functions.py` & `scores-0.8.1/src/scores/functions.py`

 * *Files identical despite different names*

### Comparing `scores-0.8/src/scores/sample_data.py` & `scores-0.8.1/src/scores/sample_data.py`

 * *Files identical despite different names*

### Comparing `scores-0.8/src/scores/typing.py` & `scores-0.8.1/src/scores/typing.py`

 * *Files identical despite different names*

### Comparing `scores-0.8/src/scores/utils.py` & `scores-0.8.1/src/scores/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Contains frequently-used functions of a general nature within scores
 """
 
 import warnings
-from collections.abc import Hashable, Iterable, Sequence
+from collections.abc import Hashable, Iterable
 from typing import Optional, Union
 
 import numpy as np
 import pandas as pd
 import xarray as xr
 
 from scores.typing import FlexibleDimensionTypes, XarrayLike
```

### Comparing `scores-0.8/src/scores/categorical/__init__.py` & `scores-0.8.1/src/scores/categorical/__init__.py`

 * *Files identical despite different names*

### Comparing `scores-0.8/src/scores/categorical/binary_impl.py` & `scores-0.8.1/src/scores/categorical/binary_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8/src/scores/categorical/contingency_impl.py` & `scores-0.8.1/src/scores/categorical/contingency_impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 import scores.utils
 from scores.typing import FlexibleArrayType, FlexibleDimensionTypes
 
 DEFAULT_PRECISION = 8
 
 
-class BasicContingencyManager:
+class BasicContingencyManager:  # pylint: disable=too-many-public-methods
     """
     A BasicContingencyManager is produced when a BinaryContingencyManager is transformed.
 
     A basic contingency table is built only from the event counts, losing the connection
     to the actual event tables in their full dimensionality.
 
     The event count data is much smaller than the full event tables, particularly when
@@ -508,24 +508,24 @@
     Base class for event operators which can be used in deriving contingency
     tables. This will be expanded as additional use cases are incorporated
     beyond the ThresholdEventOperator.
     """
 
     @abstractmethod
     def make_event_tables(
-        self, forecast: FlexibleArrayType, observed: FlexibleArrayType, *, event_threshold=None, op_fn=operator.gt
+        self, forecast: FlexibleArrayType, observed: FlexibleArrayType, *, event_threshold=None, op_fn=None
     ):
         """
         This method should be over-ridden to return forecast and observed event tables
         """
         ...  # pragma: no cover # pylint: disable=unnecessary-ellipsis
 
     @abstractmethod
     def make_contingency_manager(
-        self, forecast: FlexibleArrayType, observed: FlexibleArrayType, *, event_threshold=None, op_fn=operator.gt
+        self, forecast: FlexibleArrayType, observed: FlexibleArrayType, *, event_threshold=None, op_fn=None
     ):
         """
         This method should be over-ridden to return a contingency table.
         """
         ...  # pragma: no cover # pylint: disable=unnecessary-ellipsis
 
 
@@ -553,41 +553,44 @@
         tutorial to review more complex use cases, including on multivariate gridded model
         data, and on station data structures.
         """
 
         if not event_threshold:
             event_threshold = self.default_event_threshold
 
-        if not op_fn:
+        if op_fn is None:
             op_fn = self.default_op_fn
 
         forecast_events = op_fn(forecast, event_threshold)
         observed_events = op_fn(observed, event_threshold)
 
         # Bring back NaNs
         forecast_events = forecast_events.where(~np.isnan(forecast))
         observed_events = observed_events.where(~np.isnan(observed))
 
         return (forecast_events, observed_events)
 
     def make_contingency_manager(
-        self, forecast: FlexibleArrayType, observed: FlexibleArrayType, *, event_threshold=None, op_fn=operator.gt
+        self, forecast: FlexibleArrayType, observed: FlexibleArrayType, *, event_threshold=None, op_fn=None
     ):
         """
         Using this function requires a careful understanding of the structure of the data
         and the use of the operator function. The default operator is a simple greater-than
         operator, so this will work on a simple DataArray. To work on a DataSet, a richer
         understanding is required. It is recommended to work through the Contingency Table
         tutorial to review more complex use cases, including on multivariate gridded model
         data, and on station data structures.
         """
 
         if not event_threshold:
             event_threshold = self.default_event_threshold
 
+        if op_fn is None:
+            op_fn = self.default_op_fn
+
         forecast_events = op_fn(forecast, event_threshold)
         observed_events = op_fn(observed, event_threshold)
 
         # Bring back NaNs
         forecast_events = forecast_events.where(~np.isnan(forecast))
         observed_events = observed_events.where(~np.isnan(observed))
```

### Comparing `scores-0.8/src/scores/categorical/multicategorical_impl.py` & `scores-0.8.1/src/scores/categorical/multicategorical_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8/src/scores/continuous/__init__.py` & `scores-0.8.1/src/scores/continuous/__init__.py`

 * *Files identical despite different names*

### Comparing `scores-0.8/src/scores/continuous/flip_flop_impl.py` & `scores-0.8.1/src/scores/continuous/flip_flop_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8/src/scores/continuous/murphy_impl.py` & `scores-0.8.1/src/scores/continuous/murphy_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8/src/scores/continuous/quantile_loss_impl.py` & `scores-0.8.1/src/scores/continuous/quantile_loss_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8/src/scores/continuous/standard_impl.py` & `scores-0.8.1/src/scores/continuous/standard_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8/src/scores/pandas/continuous.py` & `scores-0.8.1/src/scores/pandas/continuous.py`

 * *Files identical despite different names*

### Comparing `scores-0.8/src/scores/probability/__init__.py` & `scores-0.8.1/src/scores/probability/__init__.py`

 * *Files identical despite different names*

### Comparing `scores-0.8/src/scores/probability/brier_impl.py` & `scores-0.8.1/src/scores/probability/brier_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8/src/scores/probability/checks.py` & `scores-0.8.1/src/scores/probability/checks.py`

 * *Files identical despite different names*

### Comparing `scores-0.8/src/scores/probability/crps_impl.py` & `scores-0.8.1/src/scores/probability/crps_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8/src/scores/probability/roc_impl.py` & `scores-0.8.1/src/scores/probability/roc_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8/src/scores/processing/__init__.py` & `scores-0.8.1/src/scores/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `scores-0.8/src/scores/processing/discretise.py` & `scores-0.8.1/src/scores/processing/discretise.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Tools for discretising data for verification"""
 
 import operator
 from collections.abc import Iterable
 from typing import Optional, Union
 
 import numpy as np
-import pandas as pd
 import xarray as xr
 
 from scores.typing import FlexibleDimensionTypes, XarrayLike
 from scores.utils import gather_dimensions
 
 INEQUALITY_MODES = {
     ">=": (operator.ge, -1),
```

### Comparing `scores-0.8/src/scores/processing/isoreg_impl.py` & `scores-0.8.1/src/scores/processing/isoreg_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8/src/scores/processing/matching.py` & `scores-0.8.1/src/scores/processing/matching.py`

 * *Files identical despite different names*

### Comparing `scores-0.8/src/scores/processing/cdf/cdf_functions.py` & `scores-0.8.1/src/scores/processing/cdf/cdf_functions.py`

 * *Files identical despite different names*

### Comparing `scores-0.8/src/scores/stats/statistical_tests/acovf.py` & `scores-0.8.1/src/scores/stats/statistical_tests/acovf.py`

 * *Files identical despite different names*

### Comparing `scores-0.8/src/scores/stats/statistical_tests/diebold_mariano_impl.py` & `scores-0.8.1/src/scores/stats/statistical_tests/diebold_mariano_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8/.gitignore` & `scores-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `scores-0.8/LICENSE` & `scores-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scores-0.8/README.md` & `scores-0.8.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 
 ## Overview
 Here is a **curated selection** of the metrics, tools and statistical tests included in `scores`:
 
 |                       	| **Description** 	| **Selection of Included Functions** 	|
 |-----------------------	|-----------------	|--------------	|
 | **[Continuous](https://scores.readthedocs.io/en/latest/included.html#continuous)**        	|Scores for evaluating single-valued continuous forecasts.                  	|Mean Absolute Error (MAE), Mean Squared Error (MSE), Root Mean Squared Error (RMSE), Additive Bias, Multiplicative Bias, Pearson's Correlation Coefficient, Flip-Flop Index, Quantile loss, Murphy score.              	|
-| **[Probability](https://scores.readthedocs.io/en/latest/included.html#probability)**       	|Scores for evaluating forecasts that are expressed as predictive distributions, ensembles, and probabilities of binary events.                 	|Brier Score, Continuous Ranked Probability Score (CRPS) for Cumulative Density Function (CDF), Threshold weighted CRPS for CDF, CRPS for ensemble, Receiver Operating Characteristic (ROC), Isotonic Regression (reliability diagrams).              	|
+| **[Probability](https://scores.readthedocs.io/en/latest/included.html#probability)**       	|Scores for evaluating forecasts that are expressed as predictive distributions, ensembles, and probabilities of binary events.                 	|Brier Score, Continuous Ranked Probability Score (CRPS) for Cumulative Density Function (CDF), Threshold weighted CRPS for CDF, CRPS for ensembles, Receiver Operating Characteristic (ROC), Isotonic Regression (reliability diagrams).              	|
 | **[Categorical](https://scores.readthedocs.io/en/latest/included.html#categorical)**       	|Scores for evaluating forecasts based on categories.                	|Probability of Detection (POD), False Alarm Rate (FAR), Probability of False Detection (POFD), Success Ratio, Accuracy, Peirce's Skill Score, Critical Success Index (CSI), Gilbert Skill Score, Heidke Skill Score, Odds Ratio, Odds Ratio Skill Score, F1 score, FIxed Risk Multicategorical (FIRM) Score.               	|
 | **[Statistical Tests](https://scores.readthedocs.io/en/latest/included.html#statistical-tests)** 	|Tools to conduct statistical tests and generate confidence intervals.                 	|Diebold Mariano.              	|
-| **[Processing tools](https://scores.readthedocs.io/en/latest/included.html#processing-tools-for-preparing-data)**        	|Tools to pre-process data.                 	|Data matching, Discretization, Cumulative Density Function Manipulation.              	|
+| **[Processing Tools](https://scores.readthedocs.io/en/latest/included.html#processing-tools-for-preparing-data)**        	|Tools to pre-process data.                 	|Data matching, Discretization, Cumulative Density Function Manipulation.              	|
 
 
 `scores` not only includes common scores (e.g. MAE, RMSE), it includes novel scores not commonly found elsewhere (e.g. FIRM, Flip-Flop Index), complex scores (e.g. threshold weighted CRPS), and statistical tests (such as the Diebold Mariano test). Additionally, it provides pre-processing tools for preparing data for scores in a variety of formats including cumulative distribution functions (CDF). `scores` provides its own implementations where relevant to avoid extensive dependencies.
 
 `scores` primarily supports xarray datatypes for Earth system data allowing it to work with NetCDF4, hdf5, Zarr and GRIB data sources among others. `scores` uses Dask for scaling and performance. Some metrics work with pandas and we will aim to expand this capability. 
 
 All of the scores and metrics in this package have undergone a thorough scientific review. Every score has a companion Jupyter Notebook tutorial that demonstrates its use in practice.
@@ -59,14 +59,14 @@
 
 To install the mathematical functions ONLY (no tutorial notebooks, no developer libraries), use the *minimal* installation option. *minimal* is a stable version with limited dependencies and can be installed from the Python Package Index.
 
 ```bash
 > pip install scores
 ```
 
-## Finding and Downloading Data
+## Finding, Downloading and Working With Data
 
-Other than very small files to support automated testing, this repository does not contain significant data for tutorials and demonstrations. The tutorials demonstrate how to easily download sample data and generate synthetic data.
+`scores` can be used with a broad variety of data sources. See the [Data Sources](https://scores.readthedocs.io/en/latest/data.html) page and this [tutorial](https://scores.readthedocs.io/en/latest/tutorials/First_Data_Fetching.html) for more information on finding, downloading and working with different sources of data.
 
 ## Acknowledging This Work
 
 If you find this work useful, please consider citing or acknowledging it. A citable DOI is coming soon. This section will be updated in the coming weeks to include the correct citation.
```

### Comparing `scores-0.8/pyproject.toml` & `scores-0.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scores-0.8/PKG-INFO` & `scores-0.8.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: scores
-Version: 0.8
+Version: 0.8.1
 Summary: Scores is a package containing mathematical functions for the verification, evaluation and optimisation of model outputs and predictions.
 Project-URL: Homepage, http://www.bom.gov.au
 Author-email: Tennessee Leeuwenburg <tennessee.leeuwenburg@bom.gov.au>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -79,18 +79,18 @@
 
 ## Overview
 Here is a **curated selection** of the metrics, tools and statistical tests included in `scores`:
 
 |                       	| **Description** 	| **Selection of Included Functions** 	|
 |-----------------------	|-----------------	|--------------	|
 | **[Continuous](https://scores.readthedocs.io/en/latest/included.html#continuous)**        	|Scores for evaluating single-valued continuous forecasts.                  	|Mean Absolute Error (MAE), Mean Squared Error (MSE), Root Mean Squared Error (RMSE), Additive Bias, Multiplicative Bias, Pearson's Correlation Coefficient, Flip-Flop Index, Quantile loss, Murphy score.              	|
-| **[Probability](https://scores.readthedocs.io/en/latest/included.html#probability)**       	|Scores for evaluating forecasts that are expressed as predictive distributions, ensembles, and probabilities of binary events.                 	|Brier Score, Continuous Ranked Probability Score (CRPS) for Cumulative Density Function (CDF), Threshold weighted CRPS for CDF, CRPS for ensemble, Receiver Operating Characteristic (ROC), Isotonic Regression (reliability diagrams).              	|
+| **[Probability](https://scores.readthedocs.io/en/latest/included.html#probability)**       	|Scores for evaluating forecasts that are expressed as predictive distributions, ensembles, and probabilities of binary events.                 	|Brier Score, Continuous Ranked Probability Score (CRPS) for Cumulative Density Function (CDF), Threshold weighted CRPS for CDF, CRPS for ensembles, Receiver Operating Characteristic (ROC), Isotonic Regression (reliability diagrams).              	|
 | **[Categorical](https://scores.readthedocs.io/en/latest/included.html#categorical)**       	|Scores for evaluating forecasts based on categories.                	|Probability of Detection (POD), False Alarm Rate (FAR), Probability of False Detection (POFD), Success Ratio, Accuracy, Peirce's Skill Score, Critical Success Index (CSI), Gilbert Skill Score, Heidke Skill Score, Odds Ratio, Odds Ratio Skill Score, F1 score, FIxed Risk Multicategorical (FIRM) Score.               	|
 | **[Statistical Tests](https://scores.readthedocs.io/en/latest/included.html#statistical-tests)** 	|Tools to conduct statistical tests and generate confidence intervals.                 	|Diebold Mariano.              	|
-| **[Processing tools](https://scores.readthedocs.io/en/latest/included.html#processing-tools-for-preparing-data)**        	|Tools to pre-process data.                 	|Data matching, Discretization, Cumulative Density Function Manipulation.              	|
+| **[Processing Tools](https://scores.readthedocs.io/en/latest/included.html#processing-tools-for-preparing-data)**        	|Tools to pre-process data.                 	|Data matching, Discretization, Cumulative Density Function Manipulation.              	|
 
 
 `scores` not only includes common scores (e.g. MAE, RMSE), it includes novel scores not commonly found elsewhere (e.g. FIRM, Flip-Flop Index), complex scores (e.g. threshold weighted CRPS), and statistical tests (such as the Diebold Mariano test). Additionally, it provides pre-processing tools for preparing data for scores in a variety of formats including cumulative distribution functions (CDF). `scores` provides its own implementations where relevant to avoid extensive dependencies.
 
 `scores` primarily supports xarray datatypes for Earth system data allowing it to work with NetCDF4, hdf5, Zarr and GRIB data sources among others. `scores` uses Dask for scaling and performance. Some metrics work with pandas and we will aim to expand this capability. 
 
 All of the scores and metrics in this package have undergone a thorough scientific review. Every score has a companion Jupyter Notebook tutorial that demonstrates its use in practice.
@@ -126,14 +126,14 @@
 
 To install the mathematical functions ONLY (no tutorial notebooks, no developer libraries), use the *minimal* installation option. *minimal* is a stable version with limited dependencies and can be installed from the Python Package Index.
 
 ```bash
 > pip install scores
 ```
 
-## Finding and Downloading Data
+## Finding, Downloading and Working With Data
 
-Other than very small files to support automated testing, this repository does not contain significant data for tutorials and demonstrations. The tutorials demonstrate how to easily download sample data and generate synthetic data.
+`scores` can be used with a broad variety of data sources. See the [Data Sources](https://scores.readthedocs.io/en/latest/data.html) page and this [tutorial](https://scores.readthedocs.io/en/latest/tutorials/First_Data_Fetching.html) for more information on finding, downloading and working with different sources of data.
 
 ## Acknowledging This Work
 
 If you find this work useful, please consider citing or acknowledging it. A citable DOI is coming soon. This section will be updated in the coming weeks to include the correct citation.
```

