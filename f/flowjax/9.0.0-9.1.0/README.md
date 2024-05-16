# Comparing `tmp/flowjax-9.0.0.tar.gz` & `tmp/flowjax-9.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowjax-9.0.0.tar", last modified: Thu May  4 19:01:03 2023, max compression
+gzip compressed data, was "flowjax-9.1.0.tar", last modified: Mon May 22 16:42:03 2023, max compression
```

## Comparing `flowjax-9.0.0.tar` & `flowjax-9.1.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:01:03.688014 flowjax-9.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-04 19:00:52.000000 flowjax-9.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-04 19:01:03.688014 flowjax-9.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-04 19:00:52.000000 flowjax-9.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:01:03.684014 flowjax-9.0.0/flowjax/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:01:03.684014 flowjax-9.0.0/flowjax/bijections/
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/bijections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/bijections/affine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/bijections/bijection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/bijections/block_autoregressive_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/bijections/chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/bijections/concatenate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/bijections/coupling.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/bijections/exp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7381 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/bijections/jax_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/bijections/masked_autoregressive.py
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/bijections/rational_quadratic_spline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/bijections/tanh.py
--rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/bijections/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20455 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12644 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/flows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/masks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:01:03.684014 flowjax-9.0.0/flowjax/nn/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/nn/block_autoregressive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/nn/masked_autoregressive.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:01:03.684014 flowjax-9.0.0/flowjax/train/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/train/data_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/train/train_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/train/variational_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-05-04 19:00:52.000000 flowjax-9.0.0/flowjax/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:01:03.684014 flowjax-9.0.0/flowjax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-04 19:01:03.000000 flowjax-9.0.0/flowjax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-04 19:01:03.000000 flowjax-9.0.0/flowjax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 19:01:03.000000 flowjax-9.0.0/flowjax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-04 19:01:03.000000 flowjax-9.0.0/flowjax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 19:01:03.000000 flowjax-9.0.0/flowjax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 19:01:03.688014 flowjax-9.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-04 19:00:52.000000 flowjax-9.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:01:03.688014 flowjax-9.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-05-04 19:00:52.000000 flowjax-9.0.0/tests/test_distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-04 19:00:52.000000 flowjax-9.0.0/tests/test_flows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-04 19:00:52.000000 flowjax-9.0.0/tests/test_masks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-04 19:00:52.000000 flowjax-9.0.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:42:03.136579 flowjax-9.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-22 16:41:54.000000 flowjax-9.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-05-22 16:42:03.136579 flowjax-9.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-22 16:41:54.000000 flowjax-9.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:42:03.132578 flowjax-9.1.0/flowjax/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-22 16:41:54.000000 flowjax-9.1.0/flowjax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:42:03.132578 flowjax-9.1.0/flowjax/bijections/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-22 16:41:54.000000 flowjax-9.1.0/flowjax/bijections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-05-22 16:41:54.000000 flowjax-9.1.0/flowjax/bijections/affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-05-22 16:41:54.000000 flowjax-9.1.0/flowjax/bijections/bijection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-05-22 16:41:54.000000 flowjax-9.1.0/flowjax/bijections/block_autoregressive_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-05-22 16:41:54.000000 flowjax-9.1.0/flowjax/bijections/chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-05-22 16:41:54.000000 flowjax-9.1.0/flowjax/bijections/concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-05-22 16:41:54.000000 flowjax-9.1.0/flowjax/bijections/coupling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-22 16:41:54.000000 flowjax-9.1.0/flowjax/bijections/exp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-05-22 16:41:54.000000 flowjax-9.1.0/flowjax/bijections/jax_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-05-22 16:41:54.000000 flowjax-9.1.0/flowjax/bijections/masked_autoregressive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-05-22 16:41:54.000000 flowjax-9.1.0/flowjax/bijections/rational_quadratic_spline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-05-22 16:41:54.000000 flowjax-9.1.0/flowjax/bijections/tanh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-05-22 16:41:54.000000 flowjax-9.1.0/flowjax/bijections/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20492 2023-05-22 16:41:54.000000 flowjax-9.1.0/flowjax/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12697 2023-05-22 16:41:54.000000 flowjax-9.1.0/flowjax/flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-22 16:41:54.000000 flowjax-9.1.0/flowjax/masks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:42:03.132578 flowjax-9.1.0/flowjax/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-22 16:41:54.000000 flowjax-9.1.0/flowjax/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-05-22 16:41:54.000000 flowjax-9.1.0/flowjax/nn/block_autoregressive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-05-22 16:41:54.000000 flowjax-9.1.0/flowjax/nn/masked_autoregressive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-22 16:41:54.000000 flowjax-9.1.0/flowjax/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:42:03.132578 flowjax-9.1.0/flowjax/train/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-22 16:41:54.000000 flowjax-9.1.0/flowjax/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-05-22 16:41:54.000000 flowjax-9.1.0/flowjax/train/data_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-22 16:41:54.000000 flowjax-9.1.0/flowjax/train/train_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-05-22 16:41:54.000000 flowjax-9.1.0/flowjax/train/variational_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-22 16:41:54.000000 flowjax-9.1.0/flowjax/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:42:03.132578 flowjax-9.1.0/flowjax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-05-22 16:42:03.000000 flowjax-9.1.0/flowjax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-22 16:42:03.000000 flowjax-9.1.0/flowjax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:42:03.000000 flowjax-9.1.0/flowjax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-22 16:42:03.000000 flowjax-9.1.0/flowjax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-22 16:42:03.000000 flowjax-9.1.0/flowjax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 16:42:03.136579 flowjax-9.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-22 16:41:54.000000 flowjax-9.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:42:03.136579 flowjax-9.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-05-22 16:41:54.000000 flowjax-9.1.0/tests/test_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-22 16:41:54.000000 flowjax-9.1.0/tests/test_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-22 16:41:54.000000 flowjax-9.1.0/tests/test_masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-22 16:41:54.000000 flowjax-9.1.0/tests/test_utils.py
```

### Comparing `flowjax-9.0.0/LICENSE` & `flowjax-9.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flowjax-9.0.0/PKG-INFO` & `flowjax-9.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: flowjax
-Version: 9.0.0
+Version: 9.1.0
 Summary: Normalizing flow implementations in jax.
 Home-page: https://github.com/danielward27/flowjax.git
 Author: Daniel Ward
 Author-email: danielward27@outlook.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
 <img src="./images/flowjax_logo.png?raw=true" alt="logo" width="500" ></img>
 </div>
@@ -62,15 +62,14 @@
 
 ## Warning
 This package is new and may have substantial breaking changes between major releases.
 
 ## TODO
 A few limitations / things that could be worth including in the future:
 - Add ability to "reshape" bijections.
-- Ability to "stack" bijections on a given (or new) axis.
 
 ## Related
 We make use of the [Equinox](https://arxiv.org/abs/2111.00254) package, which facilitates object-oriented programming with Jax. 
 
 ## Authors
 `flowjax` was written by `Daniel Ward <danielward27@outlook.com>`.
```

### Comparing `flowjax-9.0.0/README.md` & `flowjax-9.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 
 ## Warning
 This package is new and may have substantial breaking changes between major releases.
 
 ## TODO
 A few limitations / things that could be worth including in the future:
 - Add ability to "reshape" bijections.
-- Ability to "stack" bijections on a given (or new) axis.
 
 ## Related
 We make use of the [Equinox](https://arxiv.org/abs/2111.00254) package, which facilitates object-oriented programming with Jax. 
 
 ## Authors
 `flowjax` was written by `Daniel Ward <danielward27@outlook.com>`.
```

### Comparing `flowjax-9.0.0/flowjax/bijections/__init__.py` & `flowjax-9.1.0/flowjax/bijections/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Bijections from ``flowjax.bijections``"""
 
-from .affine import AdditiveLinearCondition, Affine, TriangularAffine
+from .affine import AdditiveLinearCondition, Affine, TriangularAffine, AdditiveCondition
 from .bijection import Bijection
 from .block_autoregressive_network import BlockAutoregressiveNetwork
 from .chain import Chain
 from .concatenate import Concatenate, Stack
 from .coupling import Coupling
 from .exp import Exp
 from .jax_transforms import Scan, Batch
@@ -27,13 +27,14 @@
     "Chain",
     "Scan",
     "Batch",
     "Invert",
     "Flip",
     "Permute",
     "AdditiveLinearCondition",
+    "AdditiveCondition",
     "Partial",
     "EmbedCondition",
     "RationalQuadraticSpline",
     "Concatenate",
     "Stack",
 ]
```

### Comparing `flowjax-9.0.0/flowjax/bijections/affine.py` & `flowjax-9.1.0/flowjax/bijections/affine.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 """Affine bijections."""
 
+from typing import Callable
 import jax.numpy as jnp
 from jax import Array
 from jax.experimental import checkify
 from jax.scipy.linalg import solve_triangular
 from jax.typing import ArrayLike
+import warnings
+from flowjax.utils import arraylike_to_array
 
 from flowjax.bijections.bijection import Bijection
 
 
 class Affine(Bijection):
     """Elementwise affine transformation ``y = a*x + b``. loc and scale should broadcast
     to the desired shape of the bijection.
@@ -16,38 +19,38 @@
 
     loc: Array
     log_scale: Array
 
     def __init__(self, loc: ArrayLike = 0, scale: ArrayLike = 1):
         """
         Args:
-            loc (int): Location parameter. Defaults to 0.
-            scale (int): Scale parameter. Defaults to 1.
+            loc (ArrayLike): Location parameter. Defaults to 0.
+            scale (ArrayLike): Scale parameter. Defaults to 1.
         """
-        loc, scale = [jnp.asarray(a, dtype=jnp.float32) for a in (loc, scale)]
+        loc, scale = [arraylike_to_array(a, dtype=float) for a in (loc, scale)]
         self.shape = jnp.broadcast_shapes(jnp.shape(loc), jnp.shape(scale))
         self.cond_shape = None
 
         self.loc = jnp.broadcast_to(loc, self.shape)
         self.log_scale = jnp.broadcast_to(jnp.log(scale), self.shape)
 
     def transform(self, x, condition=None):
-        self._argcheck(x)
+        x, _ = self._argcheck_and_cast(x)
         return x * self.scale + self.loc
 
     def transform_and_log_det(self, x, condition=None):
-        self._argcheck(x)
+        x, _ = self._argcheck_and_cast(x)
         return x * self.scale + self.loc, self.log_scale.sum()
 
     def inverse(self, y, condition=None):
-        self._argcheck(y)
+        y, _ = self._argcheck_and_cast(y)
         return (y - self.loc) / self.scale
 
     def inverse_and_log_det(self, y, condition=None):
-        self._argcheck(y)
+        y, _ = self._argcheck_and_cast(y)
         return (y - self.loc) / self.scale, -self.log_scale.sum()
 
     @property
     def scale(self):
         """The scale parameter of the affine transformation."""
         return jnp.exp(self.log_scale)
 
@@ -61,28 +64,29 @@
     lower: bool
     weight_log_scale: Array | None
     _arr: Array
     _log_diag: Array
 
     def __init__(
         self,
-        loc: Array,
-        arr: Array,
+        loc: ArrayLike,
+        arr: ArrayLike,
         lower: bool = True,
         weight_normalisation: bool = False,
     ):
         """
         Args:
-            loc (Array): Location parameter.
-            arr (Array): Triangular matrix.
+            loc (ArrayLike): Location parameter.
+            arr (ArrayLike): Triangular matrix.
             lower (bool): Whether the mask should select the lower or upper
                 triangular matrix (other elements ignored). Defaults to True.
             weight_log_scale (Array | None): If provided, carry out weight
                 normalisation.
         """
+        loc, arr = [arraylike_to_array(a, dtype=float) for a in (loc, arr)]
         if (arr.ndim != 2) or (arr.shape[0] != arr.shape[1]):
             raise ValueError("arr must be a square, 2-dimensional matrix.")
         checkify.check(
             jnp.all(jnp.diag(arr) > 0),
             "arr diagonal entries must be greater than 0",
         )
         dim = arr.shape[0]
@@ -110,57 +114,124 @@
         if self.weight_log_scale is not None:
             norms = jnp.linalg.norm(arr, axis=1, keepdims=True)
             arr = jnp.exp(self.weight_log_scale) * arr / norms
 
         return arr
 
     def transform(self, x, condition=None):
-        self._argcheck(x)
+        x, _ = self._argcheck_and_cast(x)
         return self.arr @ x + self.loc
 
     def transform_and_log_det(self, x, condition=None):
-        self._argcheck(x)
+        x, _ = self._argcheck_and_cast(x)
         arr = self.arr
         return arr @ x + self.loc, jnp.log(jnp.diag(arr)).sum()
 
     def inverse(self, y, condition=None):
-        self._argcheck(y)
+        y, _ = self._argcheck_and_cast(y)
         return solve_triangular(self.arr, y - self.loc, lower=self.lower)
 
     def inverse_and_log_det(self, y, condition=None):
-        self._argcheck(y)
+        y, _ = self._argcheck_and_cast(y)
         arr = self.arr
         x = solve_triangular(arr, y - self.loc, lower=self.lower)
         return x, -jnp.log(jnp.diag(arr)).sum()
 
 
+class AdditiveCondition(Bijection):
+    """Given a callable ``f``, carries out ``y = x + f(condition)`` as the forward
+    transformation and ``x = y - f(condition)`` as the inverse transformation. Note that
+    the callable can be a callable module with trainable parameters if desired.
+
+    If used to transform a distribution, this allows the "location" to be changed as a
+    function of the conditioning variables.
+    """
+
+    module: Callable[[ArrayLike], ArrayLike]
+
+    def __init__(
+        self,
+        module: Callable[[ArrayLike], ArrayLike],
+        shape: tuple[int, ...],
+        cond_shape: tuple[int, ...],
+    ):
+        """
+        Args:
+            module (Callable[[ArrayLike], ArrayLike]): A callable (e.g. a function or
+                callable module) that maps array with shape cond_shape, to a shape
+                that is broadcastable with the shape of the bijection.
+            shape (tuple[int, ...]): The shape of the bijection.
+            cond_shape (tuple[int, ...]): The condition shape of the bijection.
+
+        Example:
+            Conditioning using a linear transformation
+
+            .. doctest::
+
+                >>> from flowjax.bijections import AdditiveCondition
+                >>> from equinox.nn import Linear
+                >>> import jax.numpy as jnp
+                >>> import jax.random as jr
+                >>> bijection = AdditiveCondition(
+                ...     Linear(2, 3, key=jr.PRNGKey(0)), shape=(3,), cond_shape=(2,)
+                ...     )
+                >>> bijection.transform(jnp.ones(3), condition=jnp.ones(2))
+                Array([1.9670618, 0.8156546, 1.7763454], dtype=float32)
+        """
+        self.module = module
+        self.shape = shape
+        self.cond_shape = cond_shape
+
+    def transform(self, x, condition=None):
+        x, condition = self._argcheck_and_cast(x, condition)
+        return x + self.module(condition)  # type: ignore - validated in argcheck
+
+    def transform_and_log_det(self, x, condition=None):
+        x, condition = self._argcheck_and_cast(x, condition)
+        return self.transform(x, condition), jnp.array(0)
+
+    def inverse(self, y, condition=None):
+        y, condition = self._argcheck_and_cast(y, condition)
+        return y - self.module(condition)  # type: ignore
+
+    def inverse_and_log_det(self, y, condition=None):
+        y, condition = self._argcheck_and_cast(y, condition)
+        return self.inverse(y, condition), jnp.array(0)  # type: ignore
+
+
 class AdditiveLinearCondition(Bijection):
-    """Carries out ``y = x + W @ condition``, as the forward transformation and
+    """Deprecated as of v9.1.0. Use ``AdditiveCondition`` bijection instead.
+
+    Carries out ``y = x + W @ condition``, as the forward transformation and
     ``x = y - W @ condition`` as the inverse.
     """
 
     W: Array
 
     def __init__(self, arr: Array):
         """
         Args:
             arr (Array): Array (``W`` in the description.)
         """
+        warnings.warn(
+            "AdditiveLinearCondition is deprecated in favour of the more general "
+            "AdditiveCondition as of v9.1.0."
+        )
         self.W = arr
         self.shape = (arr.shape[-2],)
         self.cond_shape = (arr.shape[-1],)
 
     def transform(self, x, condition=None):
-        self._argcheck(x, condition)
+        x, condition = self._argcheck_and_cast(x, condition)
         return x + self.W @ condition
 
     def transform_and_log_det(self, x, condition=None):
-        self._argcheck(x, condition)
+        x, condition = self._argcheck_and_cast(x, condition)
         return self.transform(x, condition), jnp.array(0)
 
     def inverse(self, y, condition=None):
-        self._argcheck(y, condition)
+        y, condition = self._argcheck_and_cast(y, condition)
         return y - self.W @ condition
 
     def inverse_and_log_det(self, y, condition=None):
-        self._argcheck(y, condition)
+        y, condition = self._argcheck_and_cast(y, condition)
         return self.inverse(y, condition), jnp.array(0)
```

### Comparing `flowjax-9.0.0/flowjax/bijections/bijection.py` & `flowjax-9.1.0/flowjax/bijections/bijection.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,73 +6,81 @@
 of flows).
 """
 
 from abc import abstractmethod
 
 from equinox import Module
 from jax import Array
+from jax.typing import ArrayLike
+
+from flowjax.utils import arraylike_to_array
 
 
 class Bijection(Module):
     """Bijection base class. Similar to :py:class:`~flowjax.distributions.Distribution`,
     bijections have a ``shape`` and a ``cond_shape`` attribute. To allow easy composing
     of bijections, all bijections support passing of conditioning variables (even if
-    ignored). Unlike distributions, the ``shape`` attribute can be None, for cases where
-    the shape may be unknown, or unimportant (e.g. the
-    :py:class:`~flowjax.bijections.tanh.Tanh` bijection is compatible with any shape of
-    input).
+    ignored).
 
     The methods of bijections do not generally support passing of additional batch
     dimensions, however, ``jax.vmap`` or ``eqx.filter_vmap`` can be used to vmap
     specific methods if desired, and a bijection can be explicitly vectorised using the
     :py:class:`~flowjax.bijections.jax_transforms.Batch` bijection.
 
     Bijections are registered as Jax PyTrees (as they are equinox modules), so are
     compatible with normal jax operations.
 
-    Implementing a bijection
+    **Implementing a bijection**
 
         (1) Inherit from ``Bijection``.
-        (2) Define the attributes ``shape`` and ``cond_shape``
+        (2) Define the attributes ``shape`` and ``cond_shape``. A ``cond_shape`` of
+            ``None`` is used to represent unconditional bijections.
         (3) Implement the abstract methods ``transform``, ``transform_and_log_det``,
             ``inverse`` and ``inverse_and_log_det``. These should act on
             inputs compatible with the shapes ``shape`` for ``x``, and ``cond_shape``
             for ``condition``.
 
     """
 
     shape: tuple[int, ...]
     cond_shape: tuple[int, ...] | None
 
     @abstractmethod
-    def transform(self, x: Array, condition: Array | None = None) -> Array:
+    def transform(self, x: ArrayLike, condition: ArrayLike | None = None) -> Array:
         """Apply transformation."""
 
     @abstractmethod
     def transform_and_log_det(
-        self, x: Array, condition: Array | None = None
+        self, x: ArrayLike, condition: ArrayLike | None = None
     ) -> tuple[Array, Array]:
         """Apply transformation and compute log absolute value of the Jacobian determinant."""
 
     @abstractmethod
-    def inverse(self, y: Array, condition: Array | None = None) -> Array:
+    def inverse(self, y: ArrayLike, condition: ArrayLike | None = None) -> Array:
         """Invert the transformation."""
 
     @abstractmethod
     def inverse_and_log_det(
-        self, y: Array, condition: Array | None = None
+        self, y: ArrayLike, condition: ArrayLike | None = None
     ) -> tuple[Array, Array]:
         """Invert the transformation and compute log absolute value of the Jacobian determinant."""
 
-    def _argcheck(self, x: Array, condition: Array | None = None):
-        """Utility argcheck that can be added to bijection methods as required."""
-        if self.shape is not None:
-            if x.shape != self.shape:
-                raise ValueError(f"Expected x.shape {self.shape}, got {x.shape}")
-
-        if self.cond_shape is not None:
-            if condition is None:
-                raise ValueError("Condition should be provided")
-            if condition.shape != self.cond_shape:
+    def _argcheck_and_cast(
+        self, x: ArrayLike, condition: ArrayLike | None = None
+    ) -> tuple[Array, Array | None]:
+        """Utility function that checks input shapes against the bijection shapes,
+        and casts inputs to arrays if required. Note this permits passing a condition
+        in the case when bijection.cond_shape is None."""
+        x = arraylike_to_array(x, err_name="x")
+
+        if x.shape != self.shape:
+            raise ValueError(f"Expected x.shape {self.shape}; got {x.shape}")
+
+        if condition is not None:
+            condition = arraylike_to_array(condition, err_name="condition")
+
+            if self.cond_shape is not None and condition.shape != self.cond_shape:
                 raise ValueError(
-                    f"Expected condition.shape {self.cond_shape}, got {condition.shape}"
+                    f"Expected condition.shape {self.cond_shape}; got {condition.shape}"
                 )
+
+        return x, condition
```

### Comparing `flowjax-9.0.0/flowjax/bijections/block_autoregressive_network.py` & `flowjax-9.1.0/flowjax/bijections/block_autoregressive_network.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,22 +66,22 @@
         self.layers = layers
         self.block_dim = block_dim
         self.activation = activation
         self.shape = (dim,)
         self.cond_shape = (cond_dim,) if cond_dim is not None else None
 
     def transform(self, x, condition=None):
-        self._argcheck(x, condition)
+        x, condition = self._argcheck_and_cast(x, condition)
         x = self.layers[0](x, condition)[0]
         for layer in self.layers[1:]:
             x = layer(x)[0]
         return x
 
     def transform_and_log_det(self, x, condition=None):
-        self._argcheck(x, condition)
+        x, condition = self._argcheck_and_cast(x, condition)
         x, log_jacobian_3d_0 = self.layers[0](x, condition)
         log_jacobian_3ds = [log_jacobian_3d_0]
         for layer in self.layers[1:]:
             x, log_det_3d = layer(x)
             log_jacobian_3ds.append(log_det_3d)
 
         log_det = log_jacobian_3ds[-1]
```

### Comparing `flowjax-9.0.0/flowjax/bijections/chain.py` & `flowjax-9.1.0/flowjax/bijections/chain.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     def transform_and_log_det(self, x, condition=None):
         log_abs_det_jac = 0
         for bijection in self.bijections:
             x, log_abs_det_jac_i = bijection.transform_and_log_det(x, condition)
             log_abs_det_jac += log_abs_det_jac_i.sum()
         return x, log_abs_det_jac
 
-    def inverse(self, y: Array, condition=None):
+    def inverse(self, y, condition=None):
         for bijection in reversed(self.bijections):
             y = bijection.inverse(y, condition)
         return y
 
     def inverse_and_log_det(self, y, condition=None):
         log_abs_det_jac = 0
         for bijection in reversed(self.bijections):
```

### Comparing `flowjax-9.0.0/flowjax/bijections/concatenate.py` & `flowjax-9.1.0/flowjax/bijections/concatenate.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,44 +34,44 @@
         self.shape = (
             shapes[0][:axis] + (sum(s[axis] for s in shapes),) + shapes[0][axis + 1 :]
         )
         self.split_idxs = jnp.array([s[axis] for s in shapes[:-1]])
         self.cond_shape = merge_cond_shapes([b.cond_shape for b in bijections])
 
     def transform(self, x, condition=None):
-        self._argcheck(x, condition)
+        x, condition = self._argcheck_and_cast(x, condition)
         x_parts = jnp.array_split(x, self.split_idxs, axis=self.axis)
         y_parts = [
             b.transform(x_part, condition)
             for b, x_part in zip(self.bijections, x_parts)
         ]
         return jnp.concatenate(y_parts, axis=self.axis)
 
     def transform_and_log_det(self, x, condition=None):
-        self._argcheck(x, condition)
+        x, condition = self._argcheck_and_cast(x, condition)
         x_parts = jnp.array_split(x, self.split_idxs, axis=self.axis)
 
         ys_log_dets = [
             b.transform_and_log_det(x, condition)
             for b, x in zip(self.bijections, x_parts)
         ]
 
         y_parts, log_dets = zip(*ys_log_dets)
         return jnp.concatenate(y_parts, self.axis), sum(log_dets)
 
     def inverse(self, y, condition=None):
-        self._argcheck(y, condition)
+        y, condition = self._argcheck_and_cast(y, condition)
         y_parts = jnp.array_split(y, self.split_idxs, axis=self.axis)
         x_parts = [
             b.inverse(y_part, condition) for b, y_part in zip(self.bijections, y_parts)
         ]
         return jnp.concatenate(x_parts, axis=self.axis)
 
     def inverse_and_log_det(self, y, condition=None):
-        self._argcheck(y, condition)
+        y, condition = self._argcheck_and_cast(y, condition)
         y_parts = jnp.array_split(y, self.split_idxs, axis=self.axis)
 
         xs_log_dets = [
             b.inverse_and_log_det(y, condition)
             for b, y in zip(self.bijections, y_parts)
         ]
 
@@ -110,40 +110,40 @@
         shapes = [b.shape for b in bijections]
         check_shapes_match(shapes)
 
         self.shape = shapes[0][:axis] + (len(bijections),) + shapes[0][axis:]
         self.cond_shape = merge_cond_shapes([b.cond_shape for b in bijections])
 
     def transform(self, x, condition=None):
-        self._argcheck(x, condition)
+        x, condition = self._argcheck_and_cast(x, condition)
         x_parts = self._split_and_squeeze(x)
         y_parts = [
             b.transform(x, condition) for (b, x) in zip(self.bijections, x_parts)
         ]
         return jnp.stack(y_parts, self.axis)
 
     def transform_and_log_det(self, x, condition=None):
-        self._argcheck(x, condition)
+        x, condition = self._argcheck_and_cast(x, condition)
         x_parts = self._split_and_squeeze(x)
         ys_log_det = [
             b.transform_and_log_det(x, condition)
             for b, x in zip(self.bijections, x_parts)
         ]
 
         y_parts, log_dets = zip(*ys_log_det)
         return jnp.stack(y_parts, self.axis), sum(log_dets)
 
     def inverse(self, y, condition=None):
-        self._argcheck(y, condition)
+        y, condition = self._argcheck_and_cast(y, condition)
         y_parts = self._split_and_squeeze(y)
         x_parts = [b.inverse(y, condition) for (b, y) in zip(self.bijections, y_parts)]
         return jnp.stack(x_parts, self.axis)
 
     def inverse_and_log_det(self, y, condition=None):
-        self._argcheck(y, condition)
+        y, condition = self._argcheck_and_cast(y, condition)
         y_parts = self._split_and_squeeze(y)
         xs_log_det = [
             b.inverse_and_log_det(y, condition)
             for b, y in zip(self.bijections, y_parts)
         ]
         x_parts, log_dets = zip(*xs_log_det)
         return jnp.stack(x_parts, self.axis), sum(log_dets)
```

### Comparing `flowjax-9.0.0/flowjax/bijections/coupling.py` & `flowjax-9.1.0/flowjax/bijections/coupling.py`

 * *Files identical despite different names*

### Comparing `flowjax-9.0.0/flowjax/bijections/exp.py` & `flowjax-9.1.0/flowjax/bijections/exp.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,22 +13,22 @@
             shape (tuple[int, ...] | None): Shape of the bijection.
                 Defaults to None.
         """
         self.shape = shape
         self.cond_shape = None
 
     def transform(self, x, condition=None):
-        self._argcheck(x)
+        x, _ = self._argcheck_and_cast(x)
         return jnp.exp(x)
 
     def transform_and_log_det(self, x, condition=None):
-        self._argcheck(x)
+        x, _ = self._argcheck_and_cast(x)
         return jnp.exp(x), x.sum()
 
     def inverse(self, y, condition=None):
-        self._argcheck(y)
+        y, _ = self._argcheck_and_cast(y)
         return jnp.log(y)
 
     def inverse_and_log_det(self, y, condition=None):
-        self._argcheck(y)
+        y, _ = self._argcheck_and_cast(y)
         x = jnp.log(y)
         return x, -x.sum()
```

### Comparing `flowjax-9.0.0/flowjax/bijections/jax_transforms.py` & `flowjax-9.1.0/flowjax/bijections/jax_transforms.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,25 +8,14 @@
 from flowjax.bijections.bijection import Bijection
 
 
 class Batch(Bijection):
     """Add batch dimensions to a bijection, such that the new shape is
     batch_shape + bijection.shape. The batch dimensions are added using multiple
     applications of eqx.filter_vmap.
-
-    Example:
-
-    .. doctest::
-
-        >>> import jax.numpy as jnp
-        >>> from flowjax.bijections import Batch, Affine
-        >>> x = jnp.ones(2)
-        >>> batched = Batch(Affine(1), (2,), vectorize_bijection=False)
-        >>> batched.transform(x)
-        Array([2., 2.], dtype=float32)
     """
 
     bijection: Bijection
     in_axes: tuple
     batch_shape: tuple[int, ...]
 
     def __init__(
@@ -37,24 +26,34 @@
         vectorize_condition: bool | None = None,
     ):
         """
         Args:
             bijection (Bijection): Bijection to add batch dimensions to.
             batch_shape (tuple[int, ...]): The shape of the batch dimension.
             vectorize_bijection (bool): Whether to vectorise bijection parameters.
-                * If True: we vectorize across the leading dimensions in the array
+                If True, we vectorize across the leading dimensions in the array
                 leaves of the bijection. In this case, the array leaves must
                 have leading dimensions equal to batch_shape. For construction of
-                compatible bijections, see eqx.filter_vmap.
-                * If False: we broadcast the parameters, meaning
-                the same bijection parameters are used for each x.
+                compatible bijections, see ``eqx.filter_vmap``. If False: we broadcast
+                the parameters, i.e. the same bijection parameters are used for each x.
             vectorize_condition (bool | None): Whether to vectorize or broadcast the
                 conditioning variables. If broadcasting, the condition shape is
                 unchanged. If vectorising, the condition shape will be
                 ``batch_shape + bijection.cond_shape``. Defaults to None.
+
+        Example:
+
+            .. doctest::
+
+                >>> import jax.numpy as jnp
+                >>> from flowjax.bijections import Batch, Affine
+                >>> x = jnp.ones(2)
+                >>> batched = Batch(Affine(1), (2,), vectorize_bijection=False)
+                >>> batched.transform(x)
+                Array([2., 2.], dtype=float32)
         """
         if vectorize_condition is None and bijection.cond_shape is not None:
             raise ValueError(
                 "vectorize_condition must be specified for conditional bijections."
             )
 
         self.in_axes = (
@@ -70,42 +69,42 @@
             self.cond_shape = None
         elif vectorize_condition:
             self.cond_shape = batch_shape + self.bijection.cond_shape
         else:
             self.cond_shape = self.bijection.cond_shape
 
     def transform(self, x, condition=None):
-        self._argcheck(x, condition)
+        x, condition = self._argcheck_and_cast(x, condition)
 
         def _transform(bijection, x, condition):
             return bijection.transform(x, condition)
 
         return self.multi_vmap(_transform)(self.bijection, x, condition)
 
     def transform_and_log_det(self, x, condition=None):
-        self._argcheck(x, condition)
+        x, condition = self._argcheck_and_cast(x, condition)
 
         def _transform_and_log_det(bijection, x, condition):
             return bijection.transform_and_log_det(x, condition)
 
         y, log_det = self.multi_vmap(_transform_and_log_det)(
             self.bijection, x, condition
         )
         return y, jnp.sum(log_det)
 
     def inverse(self, y, condition=None):
-        self._argcheck(y, condition)
+        y, condition = self._argcheck_and_cast(y, condition)
 
         def _inverse(bijection, x, condition):
             return bijection.inverse(x, condition)
 
         return self.multi_vmap(_inverse)(self.bijection, y, condition)
 
     def inverse_and_log_det(self, y, condition=None):
-        self._argcheck(y, condition)
+        y, condition = self._argcheck_and_cast(y, condition)
 
         def _inverse_and_log_det(bijection, x, condition):
             return bijection.inverse_and_log_det(x, condition)
 
         x, log_det = self.multi_vmap(_inverse_and_log_det)(self.bijection, y, condition)
         return x, jnp.sum(log_det)
 
@@ -147,52 +146,52 @@
 
         """
         self.params, self.static = eqx.partition(bijection, eqx.is_array)  # type: ignore
         self.shape = bijection.shape
         self.cond_shape = bijection.cond_shape
 
     def transform(self, x, condition=None):
-        self._argcheck(x, condition)
+        x, condition = self._argcheck_and_cast(x, condition)
 
         def step(x, params, condition=None):
             bijection = eqx.combine(self.static, params)
             result = bijection.transform(x, condition)  # type: ignore
             return (result, None)
 
         step = partial(step, condition=condition)
         y, _ = scan(step, x, self.params)
         return y
 
     def transform_and_log_det(self, x, condition=None):
-        self._argcheck(x, condition)
+        x, condition = self._argcheck_and_cast(x, condition)
 
         def step(carry, params, condition):
             x, log_det = carry
             bijection = eqx.combine(self.static, params)
             y, log_det_i = bijection.transform_and_log_det(x, condition)  # type: ignore
             return ((y, log_det + log_det_i.sum()), None)
 
         step = partial(step, condition=condition)
         (y, log_det), _ = scan(step, (x, 0), self.params)
         return y, log_det
 
     def inverse(self, y, condition=None):
-        self._argcheck(y, condition)
+        y, _ = self._argcheck_and_cast(y, condition)
 
         def step(y, params, condition):
             bijection = eqx.combine(self.static, params)
             x = bijection.inverse(y, condition)  # type: ignore
             return (x, None)
 
         step = partial(step, condition=condition)
         x, _ = scan(step, y, self.params, reverse=True)
         return x
 
     def inverse_and_log_det(self, y, condition=None):
-        self._argcheck(y, condition)
+        y, _ = self._argcheck_and_cast(y, condition)
 
         def step(carry, params, condition):
             y, log_det = carry
             bijection = eqx.combine(self.static, params)
             x, log_det_i = bijection.inverse_and_log_det(y, condition)  # type: ignore
             return ((x, log_det + log_det_i.sum()), None)
```

### Comparing `flowjax-9.0.0/flowjax/bijections/masked_autoregressive.py` & `flowjax-9.1.0/flowjax/bijections/masked_autoregressive.py`

 * *Files identical despite different names*

### Comparing `flowjax-9.0.0/flowjax/bijections/rational_quadratic_spline.py` & `flowjax-9.1.0/flowjax/bijections/rational_quadratic_spline.py`

 * *Files identical despite different names*

### Comparing `flowjax-9.0.0/flowjax/bijections/tanh.py` & `flowjax-9.1.0/flowjax/bijections/tanh.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,27 +20,27 @@
         Args:
             shape (tuple[int, ...] | None): Shape of the bijection. Defaults to None.
         """
         self.shape = shape
         self.cond_shape = None
 
     def transform(self, x, condition=None):
-        self._argcheck(x)
+        x, _ = self._argcheck_and_cast(x)
         return jnp.tanh(x)
 
     def transform_and_log_det(self, x, condition=None):
-        self._argcheck(x)
+        x, _ = self._argcheck_and_cast(x)
         return jnp.tanh(x), jnp.sum(_tanh_log_grad(x))
 
     def inverse(self, y, condition=None):
-        self._argcheck(y)
+        y, _ = self._argcheck_and_cast(y)
         return jnp.arctanh(y)
 
     def inverse_and_log_det(self, y, condition=None):
-        self._argcheck(y)
+        y, _ = self._argcheck_and_cast(y)
         x = jnp.arctanh(y)
         return x, -jnp.sum(_tanh_log_grad(x))
 
 
 class TanhLinearTails(Bijection):
     """
     Tanh bijection, with linear "tails" beyond +/- max_val. Note due to the linear
@@ -65,37 +65,37 @@
         self.max_val = max_val
         self.linear_grad = math.exp(_tanh_log_grad(max_val))
         self.intercept = math.tanh(max_val) - self.linear_grad * max_val
         self.shape = shape
         self.cond_shape = None
 
     def transform(self, x, condition=None):
-        self._argcheck(x)
+        x, _ = self._argcheck_and_cast(x)
         is_linear = jnp.abs(x) >= self.max_val
         linear_y = self.linear_grad * x + jnp.sign(x) * self.intercept
         tanh_y = jnp.tanh(x)
         return jnp.where(is_linear, linear_y, tanh_y)
 
     def transform_and_log_det(self, x, condition=None):
-        self._argcheck(x)
+        x, _ = self._argcheck_and_cast(x)
         y = self.transform(x)
         log_grads = jnp.where(
             jnp.abs(x) >= self.max_val, jnp.log(self.linear_grad), _tanh_log_grad(x)
         )
         return y, jnp.sum(log_grads)  # type: ignore
 
     def inverse(self, y, condition=None):
-        self._argcheck(y)
+        y, _ = self._argcheck_and_cast(y)
         is_linear = jnp.abs(y) >= jnp.tanh(self.max_val)
         x_linear = (y - jnp.sign(y) * self.intercept) / self.linear_grad
         x_arctan = jnp.arctanh(y)
         return jnp.where(is_linear, x_linear, x_arctan)
 
     def inverse_and_log_det(self, y, condition=None):
-        self._argcheck(y)
+        y, _ = self._argcheck_and_cast(y)
         x = self.inverse(y)
         log_grads = jnp.where(
             jnp.abs(y) >= jnp.tanh(self.max_val),
             jnp.log(self.linear_grad),
             _tanh_log_grad(x),
         )
         return x, -jnp.sum(log_grads)  # type: ignore
```

### Comparing `flowjax-9.0.0/flowjax/bijections/utils.py` & `flowjax-9.1.0/flowjax/bijections/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Utility bijections (embedding network, permutations, inversion etc.)"""
 from typing import Callable
 
 import jax.numpy as jnp
 from jax import Array
 from jax.experimental import checkify
-
+from jax.typing import ArrayLike
 from flowjax.bijections.bijection import Bijection
 
 
 class Invert(Bijection):
     """Invert a bijection, such that the transform methods become the inverse
     methods and vice versa. Note that in general, we define bijections such that
     the forward methods are preffered, i.e. faster/actually implemented. For
@@ -43,21 +43,22 @@
 
 class Permute(Bijection):
     """Permutation transformation."""
 
     permutation: tuple[Array, ...]
     inverse_permutation: tuple[Array, ...]
 
-    def __init__(self, permutation: Array):
+    def __init__(self, permutation: ArrayLike):
         """
         Args:
-            permutation (Array): An array with shape matching the array to transform,
+            permutation (ArrayLike): An array with shape matching the array to transform,
                 with elements 0-(array.size-1) representing the new order based on the
                 flattened array (uses, C-like ordering).
         """
+        permutation = jnp.asarray(permutation)
         checkify.check(
             (permutation.ravel().sort() == jnp.arange(permutation.size)).all(),
             "Invalid permutation array provided.",
         )
         self.shape = permutation.shape
         self.cond_shape = None
 
@@ -68,25 +69,27 @@
             jnp.argsort(permutation.ravel()), permutation.shape
         )
         self.inverse_permutation = tuple(
             jnp.reshape(i, permutation.shape) for i in inv_indices
         )
 
     def transform(self, x, condition=None):
-        self._argcheck(x)
+        x, _ = self._argcheck_and_cast(x)
         return x[self.permutation]
 
     def transform_and_log_det(self, x, condition=None):
+        x, _ = self._argcheck_and_cast(x)
         return x[self.permutation], jnp.array(0)
 
     def inverse(self, y, condition=None):
-        self._argcheck(y)
+        y, _ = self._argcheck_and_cast(y)
         return y[self.inverse_permutation]
 
     def inverse_and_log_det(self, y, condition=None):
+        x, _ = self._argcheck_and_cast(y)
         return y[self.inverse_permutation], jnp.array(0)
 
 
 class Flip(Bijection):
     """Flip the input array. Condition argument is ignored."""
 
     def __init__(self, shape: tuple[int, ...]) -> None:
@@ -94,27 +97,27 @@
         Args:
             shape (tuple[int, ...] | None): The shape of the bijection. Defaults to None.
         """
         self.shape = shape
         self.cond_shape = None
 
     def transform(self, x, condition=None):
-        self._argcheck(x)
+        x, _ = self._argcheck_and_cast(x)
         return jnp.flip(x)
 
     def transform_and_log_det(self, x, condition=None):
-        self._argcheck(x)
+        x, _ = self._argcheck_and_cast(x)
         return jnp.flip(x), jnp.array(0)
 
     def inverse(self, y, condition=None):
-        self._argcheck(y)
+        y, _ = self._argcheck_and_cast(y)
         return jnp.flip(y)
 
     def inverse_and_log_det(self, y, condition=None):
-        self._argcheck(y)
+        y, _ = self._argcheck_and_cast(y)
         return jnp.flip(y), jnp.array(0)
 
 
 class Partial(Bijection):
     """Applies bijection to specific indices of an input."""
 
     bijection: Bijection
@@ -136,31 +139,31 @@
         if jnp.zeros(shape)[idxs].shape != bijection.shape:
             raise ValueError(
                 f"The bijection shape is incompatible with the subset of the input "
                 f"indexed by 'idxs'. The bijection has a shape of {bijection.shape}, "
                 f"while the subset has a shape of {jnp.zeros(shape)[idxs].shape}."
             )
 
-    def transform(self, x: Array, condition=None):
-        self._argcheck(x)
+    def transform(self, x, condition=None):
+        x, condition = self._argcheck_and_cast(x, condition)
         y = self.bijection.transform(x[self.idxs], condition)
         return x.at[self.idxs].set(y)
 
-    def transform_and_log_det(self, x: Array, condition=None):
-        self._argcheck(x)
+    def transform_and_log_det(self, x, condition=None):
+        x, condition = self._argcheck_and_cast(x, condition)
         y, log_det = self.bijection.transform_and_log_det(x[self.idxs], condition)
         return x.at[self.idxs].set(y), log_det
 
-    def inverse(self, y: Array, condition=None):
-        self._argcheck(y)
+    def inverse(self, y, condition=None):
+        y, condition = self._argcheck_and_cast(y, condition)
         x = self.bijection.inverse(y[self.idxs], condition)
         return y.at[self.idxs].set(x)
 
-    def inverse_and_log_det(self, y: Array, condition=None):
-        self._argcheck(y)
+    def inverse_and_log_det(self, y, condition=None):
+        y, condition = self._argcheck_and_cast(y, condition)
         x, log_det = self.bijection.inverse_and_log_det(y[self.idxs], condition)
         return y.at[self.idxs].set(x), log_det
 
 
 class EmbedCondition(Bijection):
     """Use an embedding network to reduce the dimensionality of the conditioning variable.
     The returned bijection has cond_dim equal to the raw condition size.
@@ -187,25 +190,25 @@
         self.bijection = bijection
         self.embedding_net = embedding_net
 
         self.shape = bijection.shape
         self.cond_shape = raw_cond_shape
 
     def transform(self, x, condition=None):
-        self._argcheck(x, condition)
+        x, condition = self._argcheck_and_cast(x, condition)
         condition = self.embedding_net(condition)
         return self.bijection.transform(x, condition)
 
     def transform_and_log_det(self, x, condition=None):
-        self._argcheck(x, condition)
+        x, condition = self._argcheck_and_cast(x, condition)
         condition = self.embedding_net(condition)
         return self.bijection.transform_and_log_det(x, condition)
 
     def inverse(self, y, condition=None):
-        self._argcheck(y, condition)
+        y, condition = self._argcheck_and_cast(y, condition)
         condition = self.embedding_net(condition)
         return self.bijection.inverse(y, condition)
 
     def inverse_and_log_det(self, y, condition=None):
-        self._argcheck(y, condition)
+        y, condition = self._argcheck_and_cast(y, condition)
         condition = self.embedding_net(condition)
         return self.bijection.inverse_and_log_det(y, condition)
```

### Comparing `flowjax-9.0.0/flowjax/distributions.py` & `flowjax-9.1.0/flowjax/distributions.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from jax.experimental import checkify
 from jax.scipy import stats as jstats
 from jax.typing import ArrayLike
 
 from flowjax.bijections import Affine, Bijection
 from flowjax.utils import _get_ufunc_signature, merge_cond_shapes
 
+from flowjax.utils import arraylike_to_array
+
 
 class Distribution(eqx.Module):
     """Distribution base class. Distributions all have an attribute ``shape``,
     denoting the shape of a single sample from the distribution. This corresponds to the
     ``batch_shape + event_shape`` in torch/numpyro distributions. Similarly, the
     ``cond_shape`` attribute denotes the shape of the conditioning variable.
     This attribute is None for unconditional distributions. For example
@@ -31,19 +33,19 @@
         (2,)
         >>> dist.cond_shape is None
         True
 
     Distributions are registered as jax PyTrees (as they are equinox modules), and as such
     they are compatible with normal jax operations.
 
-    Implementing a distribution
+    **Implementing a distribution**
 
         (1) Inherit from ``Distribution``.
-        (2) Define attributes ``shape`` and ``cond_shape`` (cond shape should be None
-            for unconditional distributions).
+        (2) Define attributes ``shape`` and ``cond_shape``. ``cond_shape`` should be
+            ``None`` for unconditional distributions.
         (3) Define the ``_sample`` method, which samples a point with a shape of
             ``shape``, (given a conditioning variable with shape ``cond_shape`` for
             conditional distributions).
         (4) Define the ``_log_prob`` method, which evaluates the log probability,
             given an input of shape ``shape`` (and a conditioning variable with shape
             ``cond_shape`` for conditional distributions).
 
@@ -64,32 +66,33 @@
         """Sample a point from the distribution."""
 
     def _sample_and_log_prob(
         self, key: jr.KeyArray, condition: Array | None = None
     ) -> tuple[Array, Array]:
         """Sample a point from the distribution, and return its log probability.
         Subclasses can reimplement this method in cases where more efficient methods
-        exists (e.g. see Transformed).
+        exists (e.g. for :class:`Transformed` distributions).
         """
         x = self._sample(key, condition)
         log_prob = self._log_prob(x, condition)
         return x, log_prob
 
-    def log_prob(self, x: Array, condition: Array | None = None) -> Array:
+    def log_prob(self, x: ArrayLike, condition: ArrayLike | None = None) -> Array:
         """Evaluate the log probability. Uses numpy like broadcasting if additional
         leading dimensions are passed.
 
         Args:
-            x (Array): Points at which to evaluate density.
-            condition (Array | None): Conditioning variables. Defaults to None.
+            x (ArrayLike): Points at which to evaluate density.
+            condition (ArrayLike | None): Conditioning variables. Defaults to None.
 
         Returns:
             Array: Jax array of log probabilities.
         """
-        self._argcheck(x, condition)
+        x = self._argcheck_and_cast_x(x)
+        condition = self._argcheck_and_cast_condition(condition)
         if condition is None:
             sig = _get_ufunc_signature([self.shape], [()])
             exclude = frozenset([1])
         else:
             sig = _get_ufunc_signature([self.shape, self.cond_shape], [()])
             exclude = frozenset()
 
@@ -98,20 +101,30 @@
         )
         return jnp.where(jnp.isnan(lps), -jnp.inf, lps)  # type: ignore
 
     def sample(
         self,
         key: jr.KeyArray,
         sample_shape: tuple[int, ...] = (),
-        condition: Array | None = None,
+        condition: ArrayLike | None = None,
     ) -> Array:
         """Sample from the distribution. For unconditional distributions, the output will
-        be of shape ``sample_shape + dist.shape``.
+        be of shape ``sample_shape + dist.shape``. For conditional distributions,
+        a batch dimension in the condition is supported, and the output shape will be
+        sample_shape + condition_batch_shape + dist.shape. See the example for more
+        information.
+
+        Args:
+            key (jr.KeyArray): Jax random key.
+            condition (ArrayLike | None): Conditioning variables. Defaults to None.
+            sample_shape (tuple[int, ...]): Sample shape. Defaults to ().
 
         Example:
+            The below example shows the behaviour of sampling, for an unconditional
+            and a conditional distribution.
 
             .. testsetup::
 
                 from flowjax.distributions import StandardNormal
                 import jax.random as jr
                 import jax.numpy as jnp
                 from flowjax.flows import CouplingFlow
@@ -151,47 +164,41 @@
                 >>> samples.shape
                 (5, 2)
                 >>> # Sample 10 times for each of 5 conditioning variables
                 >>> samples = cond_dist.sample(key, (10,), condition=jnp.ones((5, 3)))
                 >>> samples.shape
                 (10, 5, 2)
 
-        Args:
-            key (jr.KeyArray): Jax random key.
-            condition (Array | None): Conditioning variables. Defaults to None.
-            sample_shape (tuple[int, ...]): Sample shape. Defaults to ().
 
         """
-        self._argcheck(condition=condition)
+        condition = self._argcheck_and_cast_condition(condition)
         excluded, signature = self._vectorize_sample_args()
         keys = self._get_sample_keys(key, sample_shape, condition)
         return jnp.vectorize(self._sample, excluded=excluded, signature=signature)(
             keys, condition
         )  # type: ignore
 
     def sample_and_log_prob(
         self,
         key: jr.KeyArray,
         sample_shape: tuple[int, ...] = (),
-        condition: Array | None = None,
+        condition: ArrayLike | None = None,
     ):
         """Sample the distribution and return the samples and corresponding log probabilities.
         For transformed distributions (especially flows), this will generally be more efficient
-        than calling the methods seperately.
-
-        Refer to the :py:meth:`~flowjax.distributions.Distribution.sample` and
-        Refer to the :py:meth:`~flowjax.distributions.Distribution.log_prob` documentation
-        for more information.
+        than calling the methods seperately. Refer to the
+        :py:meth:`~flowjax.distributions.Distribution.sample` documentation for more
+        information.
 
         Args:
             key (jr.KeyArray): Jax random key.
-            condition (Array | None): Conditioning variables. Defaults to None.
+            condition (ArrayLike | None): Conditioning variables. Defaults to None.
             sample_shape (tuple[int, ...]): Sample shape. Defaults to ().
         """
-        self._argcheck(condition=condition)
+        condition = self._argcheck_and_cast_condition(condition)
 
         excluded, signature = self._vectorize_sample_args(sample_and_log_prob=True)
         keys = self._get_sample_keys(key, sample_shape, condition)
 
         return jnp.vectorize(
             self._sample_and_log_prob, excluded=excluded, signature=signature
         )(keys, condition)
@@ -221,45 +228,42 @@
             )
             key_shape = sample_shape + leading_cond_shape
 
         key_size = max(1, prod(key_shape))  # Still need 1 key for scalar sample
         keys = jnp.reshape(jr.split(key, key_size), key_shape + (2,))  # type: ignore
         return keys
 
-    def _argcheck(self, x=None, condition=None):
-        # jnp.vectorize would catch ndim mismatches, but it doesn't check axis lengths.
-        if x is not None:
-            x_trailing = x.shape[-self.ndim :] if self.ndim > 0 else ()
-            if x_trailing != self.shape:
-                raise ValueError(
-                    "Expected trailing dimensions in input x to match the distribution "
-                    f"shape, but got x shape {x.shape}, and distribution shape "
-                    f"{self.shape}."
-                )
-
-        if condition is None and self.cond_shape is not None:
+    def _argcheck_and_cast_x(self, x) -> Array:
+        x = arraylike_to_array(x, err_name="x")
+        x_trailing = x.shape[-self.ndim :] if self.ndim > 0 else ()
+        if x_trailing != self.shape:
             raise ValueError(
-                f"Conditioning variable was not provided. "
-                f"Expected conditioning variable with trailing shape {self.cond_shape}."
+                "Expected trailing dimensions in x to match the distribution shape "
+                f"{self.shape}; got x shape {x.shape}."
             )
+        return x
 
-        if condition is not None:
-            if self.cond_shape is None:
+    def _argcheck_and_cast_condition(self, condition) -> Array | None:
+        if self.cond_shape is None:
+            if condition is not None:
                 raise ValueError(
-                    "condition should not be provided for unconditional distribution."
+                    "Expected condition to be None for unconditional distribution; "
+                    f"got {condition}."
                 )
-            condition_trailing = (
-                condition.shape[-len(self.cond_shape) :] if self.cond_ndim > 0 else ()  # type: ignore
+            return None
+        condition = arraylike_to_array(condition, err_name="condition")
+        condition_trailing = (
+            condition.shape[-len(self.cond_shape) :] if self.cond_ndim > 0 else ()  # type: ignore
+        )
+        if condition_trailing != self.cond_shape:
+            raise ValueError(
+                "Expected trailing dimensions in condition to match cond_shape "
+                f"{self.cond_shape}, but got condition shape {condition.shape}."
             )
-            if condition_trailing != self.cond_shape:
-                raise ValueError(
-                    "Expected trailing dimensions in the condition to match "
-                    "distribution.cond_shape, but got condition shape "
-                    f"{condition.shape}, and distribution.cond_shape {self.cond_shape}."
-                )
+        return condition
 
     @property
     def ndim(self):
         """The number of dimensions in the distribution (the length of the shape)."""
         return len(self.shape)
 
     @property
@@ -309,63 +313,65 @@
         self.base_dist = base_dist
         self.bijection = bijection
         self.shape = self.base_dist.shape
         self.cond_shape = merge_cond_shapes(
             (self.bijection.cond_shape, self.base_dist.cond_shape)
         )
 
-    def _log_prob(self, x: Array, condition: Array | None = None):
+    def _log_prob(self, x, condition=None):
         z, log_abs_det = self.bijection.inverse_and_log_det(x, condition)
         p_z = self.base_dist._log_prob(z, condition)  # pylint: disable W0212
         return p_z + log_abs_det
 
-    def _sample(self, key: jr.KeyArray, condition: Array | None = None):
+    def _sample(self, key, condition=None):
         base_sample = self.base_dist._sample(key, condition)
         return self.bijection.transform(base_sample, condition)
 
-    def _sample_and_log_prob(self, key: jr.KeyArray, condition: Array | None = None):
+    def _sample_and_log_prob(self, key: jr.KeyArray, condition=None):
         # We overwrite the naive implementation of calling both methods seperately to
         # avoid computing the inverse transformation.
         base_sample, log_prob_base = self.base_dist._sample_and_log_prob(key, condition)
         sample, forward_log_dets = self.bijection.transform_and_log_det(
             base_sample, condition
         )
         return sample, log_prob_base - forward_log_dets
 
 
 class StandardNormal(Distribution):
-    """Implements a standard normal distribution, condition is ignored."""
+    """Implements a standard normal distribution, condition is ignored. Unlike
+    :class:`Normal`, this has no trainable parameters.
+    """
 
     def __init__(self, shape: tuple[int, ...] = ()):
         """
         Args:
             shape (tuple[int, ...]): The shape of the normal distribution. Defaults to ().
         """
         self.shape = shape
         self.cond_shape = None
 
-    def _log_prob(self, x: Array, condition: Array | None = None):
+    def _log_prob(self, x, condition=None):
         return jstats.norm.logpdf(x).sum()
 
-    def _sample(self, key: jr.KeyArray, condition: Array | None = None):
+    def _sample(self, key, condition=None):
         return jr.normal(key, self.shape)
 
 
 class Normal(Transformed):
     """Implements an independent Normal distribution with mean and std for
     each dimension. `loc` and `scale` should be broadcastable.
     """
 
     bijection: Affine
 
     def __init__(self, loc: ArrayLike = 0, scale: ArrayLike = 1):
         """
         Args:
-            loc (Array): Means. Defaults to 0.
-            scale (Array): Standard deviations. Defaults to 1.
+            loc (ArrayLike): Means. Defaults to 0.
+            scale (ArrayLike): Standard deviations. Defaults to 1.
         """
         shape = jnp.broadcast_shapes(jnp.shape(loc), jnp.shape(scale))
         base_dist = StandardNormal(shape)
         bijection = Affine(loc=loc, scale=scale)
         super().__init__(base_dist, bijection)
 
     @property
@@ -382,36 +388,36 @@
 class _StandardUniform(Distribution):
     """Implements a standard independent Uniform distribution, ie X ~ Uniform([0, 1]^dim)."""
 
     def __init__(self, shape: tuple[int, ...] = ()):
         self.shape = shape
         self.cond_shape = None
 
-    def _log_prob(self, x: Array, condition: Array | None = None):
+    def _log_prob(self, x, condition=None):
         return jstats.uniform.logpdf(x).sum()
 
-    def _sample(self, key: jr.KeyArray, condition: Array | None = None):
+    def _sample(self, key, condition=None):
         return jr.uniform(key, shape=self.shape)
 
 
 class Uniform(Transformed):
     """Implements an independent uniform distribution between min and max for each
     dimension. `minval` and `maxval` should be broadcastable.
     """
 
     bijection: Affine
 
     def __init__(self, minval: ArrayLike, maxval: ArrayLike):
         """
         Args:
-            minval (Array): Minimum values.
-            maxval (Array): Maximum values.
+            minval (ArrayLike): Minimum values.
+            maxval (ArrayLike): Maximum values.
         """
-        shape = jnp.broadcast_shapes(jnp.shape(minval), jnp.shape(maxval))
-        minval, maxval = jnp.array(minval), jnp.array(maxval)
+        minval, maxval = arraylike_to_array(minval), arraylike_to_array(maxval)
+        shape = jnp.broadcast_shapes(minval.shape, maxval.shape)
         checkify.check(
             jnp.all(maxval >= minval),
             "Minimums must be less than the maximums.",
         )
 
         base_dist = _StandardUniform(shape)
         bijection = Affine(loc=minval, scale=maxval - minval)
@@ -431,33 +437,33 @@
 class _StandardGumbel(Distribution):
     """Standard gumbel distribution (https://en.wikipedia.org/wiki/Gumbel_distribution)."""
 
     def __init__(self, shape: tuple[int, ...] = ()):
         self.shape = shape
         self.cond_shape = None
 
-    def _log_prob(self, x: Array, condition: Array | None = None):
+    def _log_prob(self, x, condition=None):
         return -(x + jnp.exp(-x)).sum()
 
-    def _sample(self, key: jr.KeyArray, condition: Array | None = None):
+    def _sample(self, key, condition=None):
         return jr.gumbel(key, shape=self.shape)
 
 
 class Gumbel(Transformed):
     """Gumbel distribution (https://en.wikipedia.org/wiki/Gumbel_distribution)"""
 
     bijection: Affine
 
     def __init__(self, loc: ArrayLike = 0, scale: ArrayLike = 1):
         """
         `loc` and `scale` should broadcast to the dimension of the distribution.
 
         Args:
-            loc (Array): Location paramter.
-            scale (Array): Scale parameter. Defaults to 1.0.
+            loc (ArrayLike): Location paramter.
+            scale (ArrayLike): Scale parameter. Defaults to 1.0.
         """
         shape = jnp.broadcast_shapes(jnp.shape(loc), jnp.shape(scale))
         base_dist = _StandardGumbel(shape)
         bijection = Affine(loc, scale)
 
         super().__init__(base_dist, bijection)
 
@@ -478,33 +484,33 @@
     Ref: https://en.wikipedia.org/wiki/Cauchy_distribution
     """
 
     def __init__(self, shape: tuple[int, ...] = ()):
         self.shape = shape
         self.cond_shape = None
 
-    def _log_prob(self, x: Array, condition: Array | None = None):
+    def _log_prob(self, x, condition=None):
         return jstats.cauchy.logpdf(x).sum()
 
-    def _sample(self, key: jr.KeyArray, condition: Array | None = None):
+    def _sample(self, key, condition=None):
         return jr.cauchy(key, shape=self.shape)
 
 
 class Cauchy(Transformed):
     """Cauchy distribution (https://en.wikipedia.org/wiki/Cauchy_distribution)."""
 
     bijection: Affine
 
     def __init__(self, loc: ArrayLike = 0, scale: ArrayLike = 1):
         """
         `loc` and `scale` should broadcast to the dimension of the distribution.
 
         Args:
-            loc (Array): Location paramter.
-            scale (Array): Scale parameter. Defaults to 1.0.
+            loc (ArrayLike): Location paramter.
+            scale (ArrayLike): Scale parameter. Defaults to 1.0.
         """
         shape = jnp.broadcast_shapes(jnp.shape(loc), jnp.shape(scale))
         base_dist = _StandardCauchy(shape)
         bijection = Affine(loc, scale)
         super().__init__(base_dist, bijection)
 
     @property
@@ -519,45 +525,45 @@
 
 
 class _StandardStudentT(Distribution):
     """Implements student T distribution with specified degrees of freedom."""
 
     log_df: Array
 
-    def __init__(self, df: Array):
-        self.shape = df.shape
+    def __init__(self, df: ArrayLike):
+        self.shape = jnp.shape(df)
         self.cond_shape = None
         self.log_df = jnp.log(df)
 
-    def _log_prob(self, x: Array, condition: Array | None = None):
+    def _log_prob(self, x, condition=None):
         return jstats.t.logpdf(x, df=self.df).sum()
 
-    def _sample(self, key: jr.KeyArray, condition: Array | None = None):
+    def _sample(self, key, condition=None):
         return jr.t(key, df=self.df, shape=self.shape)
 
     @property
     def df(self):
         """The degrees of freedom of the distibution."""
         return jnp.exp(self.log_df)
 
 
 class StudentT(Transformed):
     """Student T distribution (https://en.wikipedia.org/wiki/Student%27s_t-distribution)."""
 
     bijection: Affine
     base_dist: _StandardStudentT
 
-    def __init__(self, df: Array, loc: ArrayLike = 0, scale: ArrayLike = 1):
+    def __init__(self, df: ArrayLike, loc: ArrayLike = 0, scale: ArrayLike = 1):
         """
         `df`, `loc` and `scale` broadcast to the dimension of the distribution.
 
         Args:
-            df (Array): The degrees of freedom.
-            loc (Array): Location parameter. Defaults to 0.0.
-            scale (Array): Scale parameter. Defaults to 1.0.
+            df (ArrayLike): The degrees of freedom.
+            loc (ArrayLike): Location parameter. Defaults to 0.0.
+            scale (ArrayLike): Scale parameter. Defaults to 1.0.
         """
         df, loc, scale = jnp.broadcast_arrays(df, loc, scale)
         base_dist = _StandardStudentT(df)
         bijection = Affine(loc, scale)
         super().__init__(base_dist, bijection)
 
     @property
```

### Comparing `flowjax-9.0.0/flowjax/flows.py` & `flowjax-9.1.0/flowjax/flows.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,29 +9,30 @@
 import jax.nn as jnn
 import jax.numpy as jnp
 from jax import random
 from jax.nn.initializers import glorot_uniform
 from jax.random import KeyArray
 
 from flowjax.bijections import (
-    AdditiveLinearCondition,
+    AdditiveCondition,
     Bijection,
     BlockAutoregressiveNetwork,
     Chain,
     Coupling,
     Flip,
     Invert,
     MaskedAutoregressive,
     Permute,
     RationalQuadraticSpline,
     Scan,
     TanhLinearTails,
     TriangularAffine,
 )
 from flowjax.distributions import Distribution, Transformed
+from equinox.nn import Linear
 
 
 class CouplingFlow(Transformed):
     """Coupling flow (https://arxiv.org/abs/1605.08803)."""
 
     flow_layers: int
     nn_width: int
@@ -288,32 +289,34 @@
         if len(base_dist.shape) != 1:
             raise ValueError(f"Expected base_dist.ndim==1, got {base_dist.ndim}")
 
         dim = base_dist.shape[-1]
         permute_strategy = _default_permute_strategy(dim)
 
         def make_layer(key):
-            lt_key, perm_key = random.split(key)
-            c_dim = 0 if cond_dim is None else cond_dim
-            weights = init(lt_key, (dim, dim + c_dim))
-            lt_weights = weights[:, :dim].at[jnp.diag_indices(dim)].set(1)
-            cond_weights = weights[:, dim:]
+            lt_key, perm_key, cond_key = random.split(key, 3)
+            weights = init(lt_key, (dim, dim))
+            lt_weights = weights.at[jnp.diag_indices(dim)].set(1)
             lower_tri = TriangularAffine(
                 jnp.zeros(dim), lt_weights, weight_normalisation=True
             )
 
             bijections = [
                 TanhLinearTails(tanh_max_val, (dim,)),
                 RationalQuadraticSpline(knots, interval=1, shape=(dim,)),
                 Invert(TanhLinearTails(tanh_max_val, (dim,))),
                 lower_tri,
             ]
 
             if cond_dim is not None:
-                linear_condition = AdditiveLinearCondition(cond_weights)
+                linear_condition = AdditiveCondition(
+                    Linear(cond_dim, dim, use_bias=False, key=cond_key),
+                    (dim,),
+                    (cond_dim,),
+                )
                 bijections.append(linear_condition)
 
             if permute_strategy == "flip":
                 bijections.append(Flip((dim,)))
             elif permute_strategy == "random":
                 bijections.append(
                     Permute(random.permutation(perm_key, jnp.arange(dim)))
```

### Comparing `flowjax-9.0.0/flowjax/masks.py` & `flowjax-9.1.0/flowjax/masks.py`

 * *Files identical despite different names*

### Comparing `flowjax-9.0.0/flowjax/nn/block_autoregressive.py` & `flowjax-9.1.0/flowjax/nn/block_autoregressive.py`

 * *Files identical despite different names*

### Comparing `flowjax-9.0.0/flowjax/nn/masked_autoregressive.py` & `flowjax-9.1.0/flowjax/nn/masked_autoregressive.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,45 +2,48 @@
 from typing import Callable
 
 import jax.nn as jnn
 from equinox import Module
 from equinox.nn import Linear
 from jax import Array, random
 from jax.random import KeyArray
-
+from jax.typing import ArrayLike
+import jax.numpy as jnp
 from flowjax.masks import rank_based_mask
 
 
 def _identity(x):
     return x
 
 
 class MaskedLinear(Module):
     """Masked linear neural network layer."""
 
     linear: Linear
     mask: Array
 
-    def __init__(self, mask: Array, use_bias: bool = True, *, key: KeyArray):
+    def __init__(self, mask: ArrayLike, use_bias: bool = True, *, key: KeyArray):
         """
 
         Args:
-            mask (Array): Mask with shape (out_features, in_features).
+            mask (ArrayLike): Mask with shape (out_features, in_features).
             key (KeyArray): Jax PRNGKey
             use_bias (bool): Whether to include bias terms. Defaults to True.
         """
+        mask = jnp.asarray(mask)
         self.linear = Linear(mask.shape[1], mask.shape[0], use_bias, key=key)
         self.mask = mask
 
-    def __call__(self, x: Array):
+    def __call__(self, x: ArrayLike):
         """Run the masked linear layer
 
         Args:
-            x (Array): Array with shape ``(mask.shape[1], )``
+            x (ArrayLike): Array with shape ``(mask.shape[1], )``
         """
+        x = jnp.asarray(x)
         x = self.linear.weight * self.mask @ x
         if self.linear.bias is not None:
             x = x + self.linear.bias
         return x
 
 
 class AutoregressiveMLP(Module):
@@ -57,33 +60,36 @@
     hidden_ranks: Array
     layers: list[MaskedLinear]
     activation: Callable
     final_activation: Callable
 
     def __init__(
         self,
-        in_ranks: Array,
-        hidden_ranks: Array,
-        out_ranks: Array,
+        in_ranks: ArrayLike,
+        hidden_ranks: ArrayLike,
+        out_ranks: ArrayLike,
         depth: int,
         activation: Callable = jnn.relu,
         final_activation: Callable = _identity,
         *,
         key
     ) -> None:
         """
         Args:
-            in_ranks (Array): Ranks of the inputs.
-            hidden_ranks (Array): Ranks of the hidden layer(s).
-            out_ranks (Array): Ranks of the outputs.
+            in_ranks (ArrayLike): Ranks of the inputs.
+            hidden_ranks (ArrayLike): Ranks of the hidden layer(s).
+            out_ranks (ArrayLike): Ranks of the outputs.
             depth (int): Number of hidden layers.
             activation (Callable): Activation function. Defaults to jnn.relu.
             final_activation (Callable): Final activation function. Defaults to _identity.
             key (KeyArray): Jax PRNGKey.
         """
+        in_ranks, hidden_ranks, out_ranks = [
+            jnp.asarray(a) for a in [in_ranks, hidden_ranks, out_ranks]
+        ]
         masks = []
         if depth == 0:
             masks.append(rank_based_mask(in_ranks, out_ranks, eq=False))
         else:
             masks.append(rank_based_mask(in_ranks, hidden_ranks, eq=True))
             for _ in range(depth - 1):
                 masks.append(rank_based_mask(hidden_ranks, hidden_ranks, eq=True))
```

### Comparing `flowjax-9.0.0/flowjax/train/data_fit.py` & `flowjax-9.1.0/flowjax/train/data_fit.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,21 +25,21 @@
     learning_rate: float = 5e-4,
     clip_norm: float = 0.5,
     optimizer: optax.GradientTransformation | None = None,
     filter_spec: Callable | PyTree = eqx.is_inexact_array,
     show_progress: bool = True,
 ):
     """Train a distribution (e.g. a flow) to samples by maximum likelihood. Note that
-        the last batch in each epoch is dropped if truncated.
+    the last batch in each epoch is dropped if truncated.
 
     Args:
         key (KeyArray): Jax PRNGKey.
         dist (Distribution): Distribution object.
-        x (Array): Samples from target distribution.
-        condition (Array | None): Conditioning variables. Defaults to None.
+        x (ArrayLike): Samples from target distribution.
+        condition (ArrayLike | None): Conditioning variables. Defaults to None.
         max_epochs (int): Maximum number of epochs. Defaults to 50.
         max_patience (int): Number of consecutive epochs with no validation
             loss improvement after which training is terminated. Defaults to 5.
         batch_size (int): Batch size. Defaults to 256.
         val_prop (float): Proportion of data to use in validation set. Defaults to 0.1.
         learning_rate (float): Adam learning rate. Defaults to 5e-4.
         clip_norm (float): Maximum gradient norm before clipping occurs. Defaults to 0.5.
```

### Comparing `flowjax-9.0.0/flowjax/train/train_utils.py` & `flowjax-9.1.0/flowjax/train/train_utils.py`

 * *Files identical despite different names*

### Comparing `flowjax-9.0.0/flowjax/train/variational_fit.py` & `flowjax-9.1.0/flowjax/train/variational_fit.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from tqdm import tqdm
 
 from flowjax.distributions import Distribution
 
 PyTree = Any
 
 
-@eqx.filter_jit
 def elbo_loss(
     dist: Distribution,
     target: Callable[[Array], Array],
     key: jr.KeyArray,
     num_samples: int,
 ) -> Array:
     """The evidence lower bound loss function."""
@@ -40,23 +39,23 @@
     show_progress: bool = True,
 ):
     """
     Train a distribution (e.g. a flow) by variational inference to a target
     (e.g. an unnormalized density).
 
     Args:
-        key (KeyArray): Jax PRNGKey.
+        key (jr.KeyArray): Jax PRNGKey.
         dist (Distribution): Distribution object, trainable parameters are found
             using equinox.is_inexact_array.
-        target (Callable): The variational target (this is usually the unormalized log
+        target (Callable[[Array], Array]): The variational target (this is usually the unormalized log
             posterior)
-        loss_fn (Callable): The loss function to optimize. The loss function
-            should take a random key, the distribution, a callable that maps samples
-            from the distribution to a scalar loss, and a number of samples to use.
-            Defaults to elbo_loss.
+        loss_fn (Callable[[Distribution, Callable, jr.KeyArray, int], Array]): The loss
+            function to optimize. The loss function should take the distribution to train,
+            the target function, key and an int (number of samples) and map to a scalar
+            loss. Defaults to elbo_loss.
         steps (int): The number of training steps to run. Defaults to 100.
         samples_per_step (int): number of samples to use at each step.
             Defaults to 500.
         learning_rate (float): Adam learning rate. Defaults to 5e-4.
         clip_norm (float): Maximum gradient norm before clipping occurs.
             Defaults to 0.5.
         optimizer (optax.GradientTransformation | None): Optax optimizer. If provided,
```

### Comparing `flowjax-9.0.0/flowjax/utils.py` & `flowjax-9.1.0/flowjax/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 from typing import Sequence
 
 import equinox as eqx
 import jax
 import jax.numpy as jnp
 from jax import Array
 from jax.flatten_util import ravel_pytree
-
-from flowjax.bijections.bijection import Bijection
+from jax.typing import ArrayLike
 
 
 def real_to_increasing_on_interval(
     arr: Array, B: float = 1, softmax_adjust: float = 1e-2
 ):
     """Transform unconstrained parameter vector to monotonically increasing positions on [-B, B].
 
@@ -75,17 +74,15 @@
         return ",".join(result).replace(" ", "")
 
     in_shapes_str = _shapes_to_str(in_shapes)
     out_shapes_str = _shapes_to_str(out_shapes)
     return f"{in_shapes_str}->{out_shapes_str}"
 
 
-def get_ravelled_bijection_constructor(
-    bijection: Bijection, filter_spec=eqx.is_inexact_array
-):
+def get_ravelled_bijection_constructor(bijection, filter_spec=eqx.is_inexact_array):
     """Given a bijection, returns a tuple containing
     1) a constructor for the bijection from a flattened array; 2) the current flattened
     parameters.
 
     Args:
         bijection (Bijection): Bijection.
         filter_spec: Filter function. Defaults to eqx.is_inexact_array.
@@ -94,7 +91,25 @@
     current, unravel = ravel_pytree(params)
 
     def constructor(ravelled_params: Array):
         params = unravel(ravelled_params)
         return eqx.combine(params, static)
 
     return constructor, current
+
+
+def arraylike_to_array(arr, err_name: str = "input", **kwargs) -> Array:
+    """Combines jnp.asarray, with an isinstance(arr, ArrayLike) check. This
+    allows inputs to be jax.numpy arrays, numpy arrays, python built in numeric types
+    (float, int) etc, but does not allow list or tuple inputs (which are not arraylike
+    and can introduce overhead and confusing behaviour in certain cases).
+
+    Args:
+        arr: Arraylike input to convert to a jax array.
+        err_name (str, optional): Name of the input in the error message. Defaults to "input".
+        **kwargs: Key word arguments passed to jnp.asarray.
+    """
+    if not isinstance(arr, ArrayLike):
+        raise ValueError(
+            f"Expected {err_name} to be arraylike; got {type(arr).__name__}."
+        )
+    return jnp.asarray(arr, **kwargs)
```

### Comparing `flowjax-9.0.0/flowjax.egg-info/PKG-INFO` & `flowjax-9.1.0/flowjax.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: flowjax
-Version: 9.0.0
+Version: 9.1.0
 Summary: Normalizing flow implementations in jax.
 Home-page: https://github.com/danielward27/flowjax.git
 Author: Daniel Ward
 Author-email: danielward27@outlook.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
 <img src="./images/flowjax_logo.png?raw=true" alt="logo" width="500" ></img>
 </div>
@@ -62,15 +62,14 @@
 
 ## Warning
 This package is new and may have substantial breaking changes between major releases.
 
 ## TODO
 A few limitations / things that could be worth including in the future:
 - Add ability to "reshape" bijections.
-- Ability to "stack" bijections on a given (or new) axis.
 
 ## Related
 We make use of the [Equinox](https://arxiv.org/abs/2111.00254) package, which facilitates object-oriented programming with Jax. 
 
 ## Authors
 `flowjax` was written by `Daniel Ward <danielward27@outlook.com>`.
```

### Comparing `flowjax-9.0.0/flowjax.egg-info/SOURCES.txt` & `flowjax-9.1.0/flowjax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flowjax-9.0.0/setup.py` & `flowjax-9.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     text_type = type("")
     with io.open(filename, mode="r", encoding="utf-8") as fd:
         return re.sub(text_type(r":[a-z]+:`~?(.*?)`"), text_type(r"``\1``"), fd.read())
 
 
 setup(
     name="flowjax",
-    version="9.0.0",
+    version="9.1.0",
     url="https://github.com/danielward27/flowjax.git",
     license="MIT",
     author="Daniel Ward",
     author_email="danielward27@outlook.com",
     description="Normalizing flow implementations in jax.",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
@@ -26,15 +26,15 @@
     install_requires=[
         "jax",
         "jaxlib>=0.3",
         "equinox>=0.10",
         "tqdm",
         "optax",
     ],
-    python_requires=">=3.7",
+    python_requires=">=3.10",
     extras_require={"dev": ["pytest"]},
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.10",
```

### Comparing `flowjax-9.0.0/tests/test_distributions.py` & `flowjax-9.1.0/tests/test_distributions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import jax.numpy as jnp
 import jax.random as jr
+import numpy as np
 import pytest
 
 from flowjax.distributions import (
     Cauchy,
     Distribution,
     Gumbel,
     Normal,
@@ -43,31 +44,37 @@
 @pytest.mark.parametrize("distribution", _test_distributions)
 @pytest.mark.parametrize("shape", _test_shapes)
 def test_sample(distribution, shape):
     d = distribution(shape=shape)
     sample = d.sample(jr.PRNGKey(0))
     assert sample.shape == shape
 
-    sample_shape = (2, 2)
+    sample_shape = (1, 2)
     sample = d.sample(jr.PRNGKey(0), sample_shape)
     assert sample.shape == sample_shape + shape
 
 
 @pytest.mark.parametrize("distribution", _test_distributions)
 @pytest.mark.parametrize("shape", _test_shapes)
 def test_log_prob(distribution, shape):
     d = distribution(shape=shape)
     x = d.sample(jr.PRNGKey(0))
 
     assert d.log_prob(x).shape == ()
 
-    sample_shape = (2, 3)
+    sample_shape = (1, 2)
     x = d.sample(jr.PRNGKey(0), sample_shape)
     assert d.log_prob(x).shape == sample_shape
 
+    # test arraylike input
+    assert jnp.all(d.log_prob(np.array(x)) == d.log_prob(x))
+
+    if d.shape == ():
+        assert d.log_prob(jnp.array(0)) == d.log_prob(0)
+
 
 @pytest.mark.parametrize("distribution", _test_distributions)
 def test_log_prob_shape_mismatch(distribution):
     d = distribution(shape=(3,))
 
     with pytest.raises(ValueError):
         d.log_prob(jnp.ones((3, 2)))
```

### Comparing `flowjax-9.0.0/tests/test_flows.py` & `flowjax-9.1.0/tests/test_flows.py`

 * *Files identical despite different names*

### Comparing `flowjax-9.0.0/tests/test_masks.py` & `flowjax-9.1.0/tests/test_masks.py`

 * *Files identical despite different names*

### Comparing `flowjax-9.0.0/tests/test_utils.py` & `flowjax-9.1.0/tests/test_utils.py`

 * *Files identical despite different names*

