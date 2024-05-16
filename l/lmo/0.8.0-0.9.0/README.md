# Comparing `tmp/lmo-0.8.0.tar.gz` & `tmp/lmo-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmo-0.8.0.tar", max compression
+gzip compressed data, was "lmo-0.9.0.tar", max compression
```

## Comparing `lmo-0.8.0.tar` & `lmo-0.9.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0     1505 2023-04-29 15:29:38.675734 lmo-0.8.0/LICENSE
--rw-r--r--   0        0        0     3865 2023-07-16 04:39:16.565156 lmo-0.8.0/README.md
--rw-r--r--   0        0        0      846 2023-07-23 21:29:19.935256 lmo-0.8.0/lmo/__init__.py
--rw-r--r--   0        0        0    30179 2023-07-24 01:54:40.094431 lmo-0.8.0/lmo/_lm.py
--rw-r--r--   0        0        0    12599 2023-07-23 20:30:37.618885 lmo-0.8.0/lmo/_lm_co.py
--rw-r--r--   0        0        0      160 2023-07-16 20:51:40.539410 lmo-0.8.0/lmo/_meta.py
--rw-r--r--   0        0        0     5515 2023-07-23 21:31:59.599266 lmo-0.8.0/lmo/_utils.py
--rw-r--r--   0        0        0     2249 2023-07-23 17:52:22.126379 lmo-0.8.0/lmo/diagnostic.py
--rw-r--r--   0        0        0    13577 2023-07-24 02:05:07.788837 lmo-0.8.0/lmo/linalg.py
--rw-r--r--   0        0        0     3425 2023-07-24 01:48:14.041262 lmo-0.8.0/lmo/ostats.py
--rw-r--r--   0        0        0     5125 2023-07-23 17:06:07.374009 lmo-0.8.0/lmo/pwm_beta.py
--rw-r--r--   0        0        0        0 2023-04-29 15:53:33.056174 lmo-0.8.0/lmo/py.typed
--rw-r--r--   0        0        0    15588 2023-07-23 22:10:00.392413 lmo-0.8.0/lmo/theoretical.py
--rw-r--r--   0        0        0     2185 2023-07-23 18:57:56.454838 lmo-0.8.0/lmo/typing.py
--rw-r--r--   0        0        0     3825 2023-07-24 01:58:24.855716 lmo-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     5156 1970-01-01 00:00:00.000000 lmo-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1505 2023-04-29 15:29:38.675734 lmo-0.9.0/LICENSE
+-rw-r--r--   0        0        0     4478 2023-08-09 01:52:48.157965 lmo-0.9.0/README.md
+-rw-r--r--   0        0        0      885 2023-08-09 01:52:48.165965 lmo-0.9.0/lmo/__init__.py
+-rw-r--r--   0        0        0    11579 2023-08-09 01:52:48.165965 lmo-0.9.0/lmo/_distns.py
+-rw-r--r--   0        0        0    29332 2023-08-09 01:52:48.165965 lmo-0.9.0/lmo/_lm.py
+-rw-r--r--   0        0        0    12599 2023-07-23 20:30:37.618885 lmo-0.9.0/lmo/_lm_co.py
+-rw-r--r--   0        0        0      160 2023-07-16 20:51:40.539410 lmo-0.9.0/lmo/_meta.py
+-rw-r--r--   0        0        0     3471 2023-08-09 01:52:48.165965 lmo-0.9.0/lmo/_poly.py
+-rw-r--r--   0        0        0     6304 2023-08-09 01:52:48.165965 lmo-0.9.0/lmo/_utils.py
+-rw-r--r--   0        0        0     5642 2023-08-09 01:52:48.165965 lmo-0.9.0/lmo/diagnostic.py
+-rw-r--r--   0        0        0    13942 2023-08-09 01:52:48.165965 lmo-0.9.0/lmo/linalg.py
+-rw-r--r--   0        0        0     3560 2023-08-09 01:52:48.169965 lmo-0.9.0/lmo/ostats.py
+-rw-r--r--   0        0        0     5137 2023-08-09 01:52:48.169965 lmo-0.9.0/lmo/pwm_beta.py
+-rw-r--r--   0        0        0        0 2023-04-29 15:53:33.056174 lmo-0.9.0/lmo/py.typed
+-rw-r--r--   0        0        0    15394 2023-08-09 01:52:48.169965 lmo-0.9.0/lmo/theoretical.py
+-rw-r--r--   0        0        0     9851 2023-08-09 01:52:48.169965 lmo-0.9.0/lmo/typing.py
+-rw-r--r--   0        0        0     3847 2023-08-09 01:54:38.104383 lmo-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     5769 1970-01-01 00:00:00.000000 lmo-0.9.0/PKG-INFO
```

### Comparing `lmo-0.8.0/LICENSE` & `lmo-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lmo-0.8.0/README.md` & `lmo-0.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -20,21 +20,41 @@
 
 Uniform or multi-dimensional, Lmo can summarize it all with one quick glance!
 
 ~~~
 
 Unlike the legacy [moments](https://wikipedia.org/wiki/Moment_(mathematics)),
 [L-moments](https://wikipedia.org/wiki/L-moment) **uniquely describe** a 
-probability distribution.
+probability distribution, and are more robust and efficient.
 The "L" stands for Linear; it is a linear combination of order statistics.
 So Lmo is as fast as sorting your samples (in terms of time-complexity).
 
-Even if your data is pathological like [Cauchy](https://wikipedia.org/wiki/Cauchy_distribution), 
-and the L-moments are not defined, the trimmed L-moments (TL-moments) can be 
-used instead:
+## Key Features:
+
+- Calculates trimmed L-moments and L-*co*moments, from data or a distribution
+  function.
+- Complete support for trimmed L-moment (TL-moments): 
+  `lmo.l_moment(..., trim=(1 / 137, 3.1416))`.
+- Fast estimation of L-*co*moment matrices from your multidimensional data.
+- A fully non-parametric `scipy.stats`-like distribution, `lmo.l_rv`.
+  It's very efficient, robust, fast, and requires only some L-mo's!
+- Exact (co)variance structure of the L-moment estimates.
+- Complete [docs](https://jorenham.github.io/lmo/), including overly 
+  complex $\TeX$ spaghetti equations.
+- Clean Pythonic syntax for ease of use.
+- Vectorized functions for very fast fitting.
+- Fully typed, tested, and tickled.
+
+
+## Quick example
+
+
+Even if your data is pathological like 
+[Cauchy](https://wikipedia.org/wiki/Cauchy_distribution), and the L-moments 
+are not defined, the trimmed L-moments (TL-moments) can be used instead:
 
 ```pycon
 >>> import numpy as np
 >>> import lmo
 >>> rng = np.random.default_rng(1980)
 >>> x = rng.standard_cauchy(96)  # pickle me, Lmo
 >>> x.mean(), x.std()  # don't try this at home
@@ -45,30 +65,32 @@
 
 For reference; the theoretical TL-location and TL-scale of the standard 
 Cauchy distribution are $\lambda^{(1, 1)}_{1} = 0$ and 
 $\lambda^{(1, 1)}_2 \approx 0.7$ 
 ([Elamir & Seheult, 2003](https://doi.org/10.1016/S0167-9473(02)00250-5)).
 
 
-## Key Features:
 
-- Calculates trimmed L-moments and L-*co*moments, from data and distributions.
-- Exact non-parametric variance structure of the sample estimates.
-- Coming soon: ~Robust distribution fitting; the method of L-moments~.
-- Complete [docs](https://jorenham.github.io/lmo/), including overly 
-  complex $\TeX$ spaghetti equations.
-- Clean Pythonic syntax for ease of use.
-- Vectorized functions for very fast fitting.
-- Fully typed, tested, and tickled.
+---
 
+See the [documentation](https://jorenham.github.io/lmo/) for more examples and
+the API reference.
 
----
 
-See the [documentation](https://jorenham.github.io/lmo/) for usage examples and code reference.
+## Roadmap:
 
+- Add methods to all `scipy.stats` univariate distributions, for finding 
+  the theoretical/population L-mo's.
+- Robust distribution fitting, using the (generalized) method of L-moments.
+- Theoretical L-moment variance structure calculation.
+- A generic goodness-of-fit test.
+- Automatic trim-length selection.
+- Plotting utilities (deps optional), e.g. for L-moment ratio diagrams.
+- Extended multivariate support, e.g. theoretical L-comoments, and 
+  L-regression.
 
 ## Installation
 
 Lmo is on [PyPI](https://pypi.org/project/lmo/), so you can do something like:
 
 ```shell
 pip install lmo
@@ -93,13 +115,10 @@
   sample L-moments](https://doi.org/10.1016/S0378-3758(03)00213-1)
 - [*J.R.M. Hosking* (2007) &ndash; Some theory and practical uses of trimmed 
   L-moments](https://doi.org/10.1016/j.jspi.2006.12.002)
 - [*R. Serﬂing & P. Xiao* (2007) &ndash; A contribution to multivariate 
   L-moments: L-comoment matrices](https://doi.org/10.1016/j.jmva.2007.01.008)
 - [*W.H. Asquith* (2011) &ndash; Univariate Distributional Analysis with 
   L-moment Statistics](https://hdl.handle.net/2346/ETD-TTU-2011-05-1319)
-- [*C. Dutang* (2017) &ndash; Theoretical L-moments and TL-moments Using
-  Combinatorial Identities and Finite Operators
-  ](https://doi.org/10.1080/03610926.2015.1073313)
 
 
 <!--overview-end-->
```

### Comparing `lmo-0.8.0/lmo/__init__.py` & `lmo-0.9.0/lmo/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,18 +19,21 @@
     'l_coratio',
     'l_costats',
     'l_coloc',
     'l_coscale',
     'l_corr',
     'l_coskew',
     'l_cokurtosis',
+
+    'l_rv',
 )
 
 from typing import Final as _Final
 
+from ._distns import l_rv
 from ._lm import (
     l_kurtosis,
     l_loc,
     l_moment,
     l_moment_cov,
     l_ratio,
     l_ratio_se,
```

### Comparing `lmo-0.8.0/lmo/_lm.py` & `lmo-0.9.0/lmo/_lm.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,18 +17,17 @@
 
 import sys
 from typing import Any, Final, TypeVar, cast, overload
 
 import numpy as np
 import numpy.typing as npt
 
-from . import ostats
+from . import ostats, pwm_beta
 from ._utils import clean_order, ensure_axis_at, moments_to_ratio, ordered
 from .linalg import ir_pascal, sandwich, sh_legendre, trim_matrix
-from .pwm_beta import cov, weights
 from .typing import AnyInt, IntVector, LMomentOptions, SortKind
 
 if sys.version_info < (3, 11):
     from typing_extensions import Unpack
 else:
     from typing import Unpack
 
@@ -41,77 +40,35 @@
     dict[
         tuple[int, int | float, int | float],  # (n, t_1, t_2)
         npt.NDArray[np.floating[Any]],
     ]
 ] = {}
 
 
-def _l0_weights_pwm(
-    r: int,
-    n: int,
-    /,
-    dtype: np.dtype[T] | type[T] = np.float_,
-) -> npt.NDArray[T]:
-    r"""
-    Efficiently calculates the projection matrix $P = [p_{k, i}]_{r \times n}$
-    for the order statistics $x_{i:n}$.
-    This way, the $1, 2, ..., r$-th order sample L-moments of some sample
-    vector $x$, can be estimated with `np.sort(x) @ l_weights(len(x), r)`.
-
-    Parameters:
-        r: The amount of orders to evaluate, i.e. $k = 1, \dots, r$.
-        n: Sample count.
-        dtype: Desired output floating data type.
-
-    Returns:
-        P_r: 2-D array of shape `(r, n)`.
-
-    References:
-        - [J.R.M. Hosking (2007) - Some theory and practical uses of trimmed
-            L-moments](https://doi.org/10.1016/j.jspi.2006.12.002)
-    """
-    p_r = np.empty((r, n), dtype)
-
-    if r > 0:
-        np.matmul(sh_legendre(r), weights(r, n, dtype), out=p_r)
-
-    return p_r
-
-
 def _l_weights_pwm(
     r: int,
     n: int,
     /,
     trim: tuple[int, int],
     dtype: np.dtype[T] | type[T] = np.float_,
 ) -> npt.NDArray[T]:
-    if sum(trim) == 0:
-        return _l0_weights_pwm(r, n, dtype)
-
-    p_r = np.empty((r, n), dtype)
-
-    if r == 0:
-        return p_r
-
-    # the k-th TL-(t_1, t_2) weights are a linear combination of L-weights
-    # with orders k, ..., k + t_1 + t_2
+    t1, t2 = trim
+    r0 = r + t1 + t2
 
-    np.matmul(
-        trim_matrix(r, trim),
-        _l0_weights_pwm(r + sum(trim), n),
-        out=p_r,
-    )
+    p0 = sh_legendre(r0, dtype=np.int_ if r0 < 29 else dtype)
+    w0 = p0 @ pwm_beta.weights(r0, n, dtype=dtype)  # type: ignore
+    out = trim_matrix(r, trim, dtype=dtype) @ w0 if t1 or t2 else w0
+    return cast(npt.NDArray[T], out)
 
     # remove numerical noise from the trimmings, and correct for potential
     # shifts in means
-    t1, t2 = trim
-    p_r[:, :t1] = p_r[:, n - t2:] = 0
-    p_r[1:, t1:n - t2] -= p_r[1:, t1:n - t2].mean(1, keepdims=True)
+    # p_r[:, :t1] = p_r[:, n - t2:] = 0
+    # p_r[1:, t1:n - t2] -= p_r[1:, t1:n - t2].mean(1, keepdims=True)
 
-    return p_r
+    # return p_r
 
 
 def _l_weights_ostat(
     r: int,
     N: int,  # noqa: N803
     /,
     trim: tuple[float, float],
@@ -119,15 +76,15 @@
 ) -> npt.NDArray[T]:
     s, t = trim
 
     assert 0 < r + s + t <= N, (r, N, trim)
     assert r >= 1, r
     assert s >= 0 and t >= 0, trim
 
-    c = ir_pascal(r)
+    c = ir_pascal(r, dtype=dtype)
     jnj = np.arange(N, dtype=dtype)
     jnj /= (N - jnj)
 
     out = np.zeros((r, N), dtype=dtype)
     for n in range(r):
         w0 = ostats.weights(s, s + t + n + 1, N)
         out[n] = c[n, 0] * w0
@@ -139,17 +96,18 @@
 
 
 def l_weights(
     r: int,
     n: int,
     /,
     trim: tuple[float, float] = (0, 0),
+    dtype: np.dtype[T] | type[T] = np.float_,
     *,
     cache: bool = False,
-) -> npt.NDArray[np.float_]:
+) -> npt.NDArray[T]:
     r"""
     Projection matrix of the first $r$ (T)L-moments for $n$ samples.
 
     For integer trim is the matrix is a linear combination of the Power
     Weighted Moment (PWM) weights (the sample estimator of $beta_{r_1}$), and
     the shifted Legendre polynomials.
 
@@ -196,15 +154,15 @@
         array([0.25      , 0.66666667, 0.        ])
 
     References:
         - [J.R.M. Hosking (2007) - Some theory and practical uses of trimmed
             L-moments](https://doi.org/10.1016/j.jspi.2006.12.002)
     """
     if r == 0:
-        return np.empty((r, n))
+        return np.empty((r, n), dtype=dtype)
 
     match trim:
         case s, t if s < 0 or t < 0:
             msg = f'trim orders must be >=0, got {trim}'
             raise ValueError(msg)
         case s, t:
             pass
@@ -225,32 +183,31 @@
     ):
         if w.shape[0] < r:
             w = w[:r]
 
         # ignore if r is larger that what's cached
         if w.shape[0] == r:
             assert w.shape == (r, n)
-            return w
+            return w.astype(dtype)
 
     if isinstance(s, int | np.integer) and isinstance(t, int | np.integer):
-        w = _l_weights_pwm(r, n, trim=(int(s), int(t)))
+        w = _l_weights_pwm(r, n, trim=(int(s), int(t)), dtype=dtype)
     else:
-        w = _l_weights_ostat(r, n, trim=(float(s), float(t)))
+        w = _l_weights_ostat(r, n, trim=(float(s), float(t)), dtype=dtype)
 
     if cache:
         # memoize
         _L_WEIGHTS_CACHE[cache_key] = w
 
     return w
 
 
 
 # Summary statistics
 
-
 @overload
 def l_moment(
     a: npt.ArrayLike,
     r: AnyInt,
     /,
     trim: tuple[float, float] = ...,
     *,
@@ -276,14 +233,15 @@
     fweights: IntVector | None = ...,
     aweights: npt.ArrayLike | None = ...,
     sort: SortKind | None = ...,
     cache: bool = ...,
 ) -> T:
     ...
 
+
 @overload
 def l_moment(
     a: npt.ArrayLike,
     r: AnyInt,
     /,
     trim: tuple[float, float] = ...,
     *,
@@ -306,26 +264,27 @@
     *,
     axis: int,
     dtype: np.dtype[T] | type[T],
     fweights: IntVector | None = ...,
     aweights: npt.ArrayLike | None = ...,
     sort: SortKind | None = ...,
     cache: bool = ...,
-) -> T | npt.NDArray[T]:
+) -> npt.NDArray[T] | T:
     ...
 
+
 @overload
 def l_moment(
     a: npt.ArrayLike,
     r: IntVector,
     /,
     trim: tuple[float, float] = ...,
     *,
     axis: int | None = ...,
-    dtype: type[np.float_],
+    dtype: type[np.float_] = ...,
     fweights: IntVector | None = ...,
     aweights: npt.ArrayLike | None = ...,
     sort: SortKind | None = ...,
     cache: bool = ...,
 ) -> npt.NDArray[np.float_]:
     ...
 
@@ -345,26 +304,26 @@
     cache: bool = ...,
 ) -> npt.NDArray[T]:
     ...
 
 
 def l_moment(
     a: npt.ArrayLike,
-    r: AnyInt | IntVector,
+    r: IntVector | AnyInt,
     /,
     trim: tuple[float, float] = (0, 0),
     *,
     axis: int | None = None,
     dtype: np.dtype[T] | type[T] = np.float_,
 
     fweights: IntVector | None = None,
     aweights: npt.ArrayLike | None = None,
     sort: SortKind | None = 'stable',
     cache: bool = False,
-) -> T | npt.NDArray[T]:
+) -> npt.NDArray[T] | T:
     r"""
     Estimates the generalized trimmed L-moment $\lambda^{(t_1, t_2)}_r$ from
     the samples along the specified axis. By default, this will be the regular
     L-moment, $\lambda_r = \lambda^{(0, 0)}_r$.
 
     Parameters:
         a:
@@ -439,15 +398,15 @@
         different (symmetric) trim-lengths.
 
         >>> import lmo, numpy as np
         >>> x = np.random.default_rng(12345).standard_t(2, 99)
         >>> lmo.l_moment(x, [1, 2], trim=(0, 0))
         array([-0.01412282,  0.94063132])
         >>> lmo.l_moment(x, [1, 2], trim=(1/2, 1/2))
-        array([-0.02158858,  0.57977201])
+        array([-0.02158858,  0.5796519 ])
         >>> lmo.l_moment(x, [1, 2], trim=(1, 1))
         array([-0.0124483 ,  0.40120115])
 
         The theoretical L-locations are all 0, and the the L-scale are
         `1.1107`, `0.6002` and `0.4165`, respectively.
 
     See Also:
@@ -471,22 +430,22 @@
     )
     x_k = ensure_axis_at(x_k, axis, -1)
     n = x_k.shape[-1]
 
     _r = np.asarray(r)
     r_max = clean_order(np.max(_r))
 
-    l_r = np.inner(l_weights(r_max, n, trim, cache=cache), x_k)
+    l_r = np.inner(l_weights(r_max, n, trim, cache=cache, dtype=dtype), x_k)
 
     # we like 0-based indexing; so if P_r starts at r=1, prepend all 1's
     # for r=0 (any zeroth moment is defined to be 1)
     l_r = np.r_[np.ones((1, *l_r.shape[1:]), dtype=l_r.dtype), l_r]
 
     # l[r] fails when r is e.g. a tuple (valid sequence).
-    return cast(T | npt.NDArray[T], l_r.take(_r, 0))
+    return cast(npt.NDArray[T] | T, l_r.take(_r, 0))
 
 
 def l_moment_cov(
     a: npt.ArrayLike,
     r_max: AnyInt,
     /,
     trim: tuple[int, int] = (0, 0),
@@ -530,14 +489,16 @@
 
     References:
         - [E. Elamir & A. Seheult (2003) - Trimmed L-moments](
             https://doi.org/10.1016/S0167-9473(02)00250-5)
         - [E. Elamir & A. Seheult (2004) - Exact variance structure of sample
             L-moments](https://doi.org/10.1016/S0378-3758(03)00213-1)
 
+    Todo:
+        - Use the direct (Jacobi) method from Hosking (2015).
     """
     if any(int(t) != t for t in trim):
         msg = 'l_moment_cov does not support fractional trimming (yet)'
         raise TypeError(msg)
 
     ks = int(r_max + sum(trim))
     if ks < r_max:
@@ -545,18 +506,18 @@
         raise ValueError(msg)
 
 
     # projection matrix: PWMs -> generalized trimmed L-moments
     p_l: npt.NDArray[np.floating[Any]]
     p_l = trim_matrix(int(r_max), trim=trim, dtype=dtype) @ sh_legendre(ks)
     # clean some numerical noise
-    p_l = np.round(p_l, 12) + 0.
+    # p_l = np.round(p_l, 12) + 0.
 
     # PWM covariance matrix
-    s_b = cov(a, ks, axis=axis, dtype=dtype, **kwargs)
+    s_b = pwm_beta.cov(a, ks, axis=axis, dtype=dtype, **kwargs)
 
     # tasty, eh?
     return sandwich(p_l, s_b, dtype=dtype)
 
 
 @overload
 def l_ratio(
@@ -609,15 +570,15 @@
     s: AnyInt,
     /,
     trim: tuple[float, float] = ...,
     *,
     axis: int,
     dtype: np.dtype[T] | type[T],
     **kwargs: Unpack[LMomentOptions],
-) -> T | npt.NDArray[T]:
+) -> npt.NDArray[T] | T:
     ...
 
 @overload
 def l_ratio(
     a: npt.ArrayLike,
     r: IntVector,
     s: AnyInt | IntVector,
@@ -681,15 +642,15 @@
     s: AnyInt | IntVector,
     /,
     trim: tuple[float, float] = (0, 0),
     *,
     axis: int | None = None,
     dtype: np.dtype[T] | type[T] = np.float_,
     **kwargs: Unpack[LMomentOptions],
-) -> T | npt.NDArray[T]:
+) -> npt.NDArray[T] | T:
     r"""
     Estimates the generalized L-moment ratio:
 
     $$
     \tau^{(t_1, t_2)}_{rs} = \frac{
         \lambda^{(t_1, t_2)}_r
     }{
@@ -866,32 +827,32 @@
     a: npt.ArrayLike,
     /,
     trim: tuple[float, float] = (0, 0),
     *,
     axis: int | None = None,
     dtype: np.dtype[T] | type[T] = np.float_,
     **kwargs: Unpack[LMomentOptions],
-) -> T | npt.NDArray[T]:
+) -> npt.NDArray[T] | T:
     r"""
     *L-location* (or *L-loc*): unbiased estimator of the first L-moment,
     $\lambda^{(t_1, t_2)}_1$.
 
     Alias for [`lmo.l_moment(a, 1, *, **)`][lmo.l_moment].
 
     Examples:
         >>> import lmo, numpy as np
         >>> x = np.random.default_rng(12345).standard_cauchy(99)
         >>> x.mean()
-        -7.56485034...
+        -7.5648...
         >>> lmo.l_loc(x)  # no trim; equivalent to the (arithmetic) mean
-        -7.56485034...
+        -7.5648...
         >>> lmo.l_loc(x, trim=(1, 1))  # TL-location
-        -0.15924180...
+        -0.15924...
         >>> lmo.l_loc(x, trim=(3/2, 3/2))  # Fractional trimming (only in Lmo)
-        -0.08845121...
+        -0.085845...
 
 
     Notes:
         If `trim = (0, 0)` (default), the L-location is equivalent to the
         [arithmetic mean](https://wikipedia.org/wiki/Arithmetic_mean).
 
     See Also:
@@ -905,15 +866,15 @@
     a: npt.ArrayLike,
     /,
     trim: tuple[float, float] = (0, 0),
     *,
     axis: int | None = None,
     dtype: np.dtype[T] | type[T] = np.float_,
     **kwargs: Unpack[LMomentOptions],
-) -> T | npt.NDArray[T]:
+) -> npt.NDArray[T] | T:
     r"""
     *L-scale*: unbiased estimator of the second L-moment,
     $\lambda^{(t_1, t_2)}_2$.
 
     Alias for [`lmo.l_moment(a, 2, *, **)`][lmo.l_moment].
 
     Examples:
@@ -942,15 +903,15 @@
     a: npt.ArrayLike,
     /,
     trim: tuple[float, float] = (0, 0),
     *,
     axis: int | None = None,
     dtype: np.dtype[T] | type[T] = np.float_,
     **kwargs: Unpack[LMomentOptions],
-) -> T | npt.NDArray[T]:
+) -> npt.NDArray[T] | T:
     r"""
     The *coefficient of L-variation* (or *L-CV*) unbiased sample estimator:
 
     $$
     \tau^{(t_1, t_2)} = \frac{
         \lambda^{(t_1, t_2)}_2
     }{
@@ -988,15 +949,15 @@
     a: npt.ArrayLike,
     /,
     trim: tuple[float, float] = (0, 0),
     *,
     axis: int | None = None,
     dtype: np.dtype[T] | type[T] = np.float_,
     **kwargs: Unpack[LMomentOptions],
-) -> T | npt.NDArray[T]:
+) -> npt.NDArray[T] | T:
     r"""
     Unbiased sample estimator of the *coefficient of L-skewness*, or *L-skew*
     for short:
 
     $$
     \tau^{(t_1, t_2)}_3
         = \frac{
@@ -1027,15 +988,15 @@
     a: npt.ArrayLike,
     /,
     trim: tuple[float, float] = (0, 0),
     *,
     axis: int | None = None,
     dtype: np.dtype[T] | type[T] = np.float_,
     **kwargs: Unpack[LMomentOptions],
-) -> T | npt.NDArray[T]:
+) -> npt.NDArray[T] | T:
     r"""
     L-kurtosis coefficient; the 4th sample L-moment ratio.
 
     $$
     \tau^{(t_1, t_2)}_4
         = \frac{
             \lambda^{(t_1, t_2)}_4
```

### Comparing `lmo-0.8.0/lmo/_lm_co.py` & `lmo-0.9.0/lmo/_lm_co.py`

 * *Files identical despite different names*

### Comparing `lmo-0.8.0/lmo/_utils.py` & `lmo-0.9.0/lmo/_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,28 @@
 __all__ = (
-    'clean_order',
     'ensure_axis_at',
     'as_float_array',
     'ordered',
+
+    'clean_order',
+    'clean_trim',
     'moments_to_ratio',
 )
 
 from typing import Any, SupportsIndex, TypeVar
 
 import numpy as np
 import numpy.typing as npt
 
-from .typing import IndexOrder, IntVector, SortKind
+from .typing import AnyTrim, IndexOrder, IntVector, SortKind
 
 T = TypeVar('T', bound=np.generic)
 FT = TypeVar('FT', bound=np.floating[Any])
 
 
-def clean_order(
-    order: SupportsIndex,
-    /,
-    name: str = 'r',
-    strict: bool = False,
-) -> int:
-    if (r := order.__index__()) < (r0 := int(strict)):
-        msg = f'expected {name} >= {r0}, got {r}'
-        raise TypeError(msg)
-
-    return r
-
-
 def ensure_axis_at(
     a: npt.NDArray[T],
     /,
     source: int | None,
     destination: int,
     order: IndexOrder = 'C',
 ) -> npt.NDArray[T]:
@@ -162,14 +151,58 @@
     if aweights is None:
         return x_k
 
     w_k = _sort_like(_clean_array(aweights))
     return _apply_aweights(x_k, w_k, axis=axis or 0)
 
 
+def clean_order(
+    r: SupportsIndex,
+    /,
+    name: str = 'r',
+    rmin: SupportsIndex = 0,
+) -> int:
+    if (_r := r.__index__()) < (_rmin := r.__index__()):
+        msg = f'expected {name} >= {_rmin}, got {_r}'
+        raise TypeError(msg)
+
+    return _r
+
+def clean_trim(trim: AnyTrim) -> tuple[int, int] | tuple[float, float]:
+    _trim = np.asarray_chkfinite(trim)
+
+    if not np.isrealobj(_trim):
+        msg = 'trim must be real'
+        raise TypeError(msg)
+
+    if _trim.ndim > 1:
+        msg = 'trim cannot be vectorized'
+        raise TypeError(trim)
+
+    n = _trim.size
+    if n == 0:
+        _trim = np.array([0, 0])
+    if n == 1:
+        _trim = np.repeat(_trim, 2)
+    elif n > 2:
+        msg = f'expected two trim values, got {n} instead'
+        raise TypeError(msg)
+
+    s, t = _trim
+
+    if s < 0 or t < 0:
+        msg = f'trim must be positive, got {(s, t)}'
+        raise TypeError(msg)
+
+    if s.is_integer() and t.is_integer():
+        return int(s), int(t)
+
+    return float(s), float(t)
+
+
 def moments_to_ratio(
     rs: npt.NDArray[np.integer[Any]],
     l_rs: npt.NDArray[FT],
     /,
 ) -> FT | npt.NDArray[FT]:
     assert rs.shape == l_rs.shape, [rs.shape, l_rs.shape]
     assert len(rs) == 2
```

### Comparing `lmo-0.8.0/lmo/linalg.py` & `lmo-0.9.0/lmo/linalg.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,27 +9,27 @@
     'sh_jacobi',
     'succession_matrix',
     'trim_matrix',
 )
 
 import sys
 from math import comb, lgamma
-from typing import Any, TypeVar
+from typing import Any, TypeVar, cast
 
 if sys.version_info >= (3, 11):
     from typing import assert_never
 else:
     from typing_extensions import assert_never
 
 import numpy as np
 import numpy.typing as npt
 
-from .typing import AnyInt
+from .typing import AnyFloat, AnyInt
 
-T = TypeVar('T', bound=np.integer[Any] | np.floating[Any])
+T = TypeVar('T', bound=np.object_ | np.integer[Any] | np.floating[Any])
 
 
 def sandwich(
     A: npt.NDArray[np.number[Any]],
     X: npt.NDArray[T | np.number[Any]],
     /,
     dtype: np.dtype[T] | type[T] = np.float_,
@@ -124,28 +124,39 @@
 
     out[:, 0] = 1
     if inv:
         # 1337 matrix inversion
         out[1::2, 0] = -1
 
     jj = np.arange(1, k, dtype=np.int_)
-    for i in range(1, k):
+    for i in jj:
         out[i, 1:i+1] = i * out[i - 1, :i] // jj[:i]
 
     return out
 
 
-def ir_pascal(k: int, /) -> npt.NDArray[np.float_]:
+def ir_pascal(
+    k: int,
+    /,
+    dtype: np.dtype[T] | type[T] = np.float_,
+) -> npt.NDArray[np.float_]:
     r"""
     Inverse regulatized lower-diagonal Pascal matrix,
     $\bar{L}_{ij} = L^{-1}_ij / i$.
 
     Used to linearly combine order statistics order statistics into L-moments.
     """
-    return pascal(k, np.float_, inv=True) / np.arange(1, k + 1)[:, None]
+    # use native ints to reduce the effect of over-/underflows
+    dtype_native = k > 62
+    _dtype = np.object_ if dtype_native else np.int_
+
+    p = pascal(k, dtype=_dtype, inv=True)
+    out = p / np.arange(1, k + 1, dtype=_dtype)[:, None]  # type: ignore
+
+    return np.asarray(out, dtype)
 
 
 def sh_legendre(
     k : int,
     /,
     dtype: np.dtype[T] | type[T] = np.int_,
 ) -> npt.NDArray[T]:
@@ -182,15 +193,15 @@
                [  1,  -6,   6,   0],
                [ -1,  12, -30,  20]])
 
     See Also:
         - https://wikipedia.org/wiki/Legendre_polynomials
         - https://wikipedia.org/wiki/Pascal_matrix
     """
-    return sh_jacobi(k, 0, 0).astype(dtype)
+    return _sh_jacobi_i(k, 0, 0, dtype=dtype)
 
 
 def _sh_jacobi_i(
     k: int,
     a: int,
     b: int,
     /,
@@ -234,16 +245,16 @@
                 - log_rab_fpow_a,
             )
     return out
 
 
 def sh_jacobi(
     k: AnyInt,
-    a: T | int,
-    b: T | int,
+    a: AnyFloat,
+    b: AnyFloat,
     /,
     dtype: np.dtype[T] | type[T] | None = None,
 ) -> npt.NDArray[T | np.int_]:
     r"""
     Shifted Jacobi polynomial coefficient matrix $\widetilde{P}^{(a,b)}$ of
     shape `(k, k)`.
 
@@ -299,18 +310,18 @@
         - [`scipy.special.jacobi`][scipy.special.jacobi]
     """
     if k < 0 or a < 0 or b < 0:
         msg = 'k, a, and b must be >= 0'
         raise ValueError(msg)
 
     _dtype = dtype or np.asarray([a, b]).dtype.type
-    if np.issubdtype(_dtype, np.integer):
-        return _sh_jacobi_i(int(k), int(a), int(b), _dtype)
+    if np.issubdtype(_dtype, np.integer) or np.issubdtype(_dtype, np.bool_):
+        return _sh_jacobi_i(int(k), int(a), int(b), dtype=_dtype)
 
-    return _sh_jacobi_f(int(k), float(a), float(b), _dtype)
+    return _sh_jacobi_f(int(k), float(a), float(b), dtype=_dtype)
 
 
 
 def succession_matrix(c: npt.NDArray[T], /) -> npt.NDArray[T]:
     r"""
     A toeplitz-like transformation matrix construction, that prepends $i$
     zeroes to $i$-th row, so that the input shape is mapped from `(n, k)`
@@ -343,15 +354,15 @@
 
 
 def trim_matrix(
     r: int,
     /,
     trim: tuple[int, int],
     dtype: np.dtype[T] | type[T] = np.float_,
-) -> npt.NDArray[np.floating[Any]]:
+) -> npt.NDArray[T]:
     r"""
     Linearization of the trimmed L-moment recurrence relations, following
     the (corrected) derivation by Hosking (2007) from the (shifted) Jacobi
     Polynomials.
 
     This constructs a $r \times r + t_1 + t_2$ matrix $T^{(t_1, t_2)}$ that
     "trims" conventional L-moments. E.g. the first 3 $(1, 1)$ trimmed
@@ -397,40 +408,42 @@
             L-moments](https://doi.org/10.1016/j.jspi.2006.12.002)
     """
     assert r >= 0
 
     if r == 0:
         return np.empty((0, 0), dtype=dtype)
 
-    rr = np.linspace(1, r, r, dtype=np.int64)
+    rr = np.arange(1, r + 1, dtype=np.int_)
 
     t1, t2 = trim
     nc = t1 + t2 - 1 + 2 * rr
     c0 = (t1 + t2 + rr) / nc
 
     match t1, t2:
         case (0, 0):
-            return np.eye(r, dtype=dtype)
+            out = np.eye(r, dtype=dtype)
         case (0, 1) | (1, 0):
             # (r + 1) / (2 r) * (l_r +/- l_{r+1})
             # = (r + s + t) / (2r + s + t - 1) * (l_r +/- l_{r+1})
-            return succession_matrix(np.outer(c0, [1, t1 - t2]))
+            out = succession_matrix(np.outer(c0, [1, t1 - t2]))
         case (1, 1):
             # (r + 1)(r + 2) / (2 r (2r + 1)) * (l_r +/- l_{r+2})
             # and (r + 1)(r + 2) / (2 r (2r + 1)) = c0 * (r + 1) / (2 r)
-            return succession_matrix(np.outer(c0 * (.5 + .5 / rr), [1, 0, -1]))
+            out = succession_matrix(np.outer(c0 * (.5 + .5 / rr), [1, 0, -1]))
         case (s, t) if s < t:
             # ((r+s+t) * _[r+0] - (r+1) * (r+s) * _[r+1] / r) / (2r+s+t-1)
             c1 = -(rr + 1) * (rr + s) / (rr * nc)
             m0 = succession_matrix(np.c_[c0, c1])
             m1 = trim_matrix(r + 1, (s, t - 1), dtype)
-            return m0 @ m1
+            out = m0 @ m1
         case (s, t) if s >= t:
             c1 = (rr + 1) * (rr + t) / (rr * nc)
             m0 = succession_matrix(np.c_[c0, c1])
             m1 = trim_matrix(r + 1, (s - 1, t), dtype)
-            return m0 @ m1
+            out =  m0 @ m1
         case (int(), int()):
             msg = 'trim values must be non-negative'
             raise ValueError(msg)
         case _ as wtf:  # type: ignore [reportUnnecessaryComparison]
             assert_never(wtf)
+
+    return cast(npt.NDArray[T], out)
```

### Comparing `lmo-0.8.0/lmo/ostats.py` & `lmo-0.9.0/lmo/ostats.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,19 +7,19 @@
     [H.A. David & H.N. Nagaraja (2004) &ndash; Order statistics
     ](https://books.google.com/books?id=bdhzFXg6xFkC)
 """
 
 import functools
 from collections.abc import Sequence
 from math import floor
-from typing import Any, overload
+from typing import Any, cast, overload
 
 import numpy as np
 import numpy.typing as npt
-from scipy.special import beta, betainc  # type: ignore
+from scipy.special import betainc, betaln  # type: ignore
 
 from .typing import AnyNDArray
 
 
 def _weights(
     i: float,
     n: float,
@@ -28,18 +28,23 @@
 ) -> npt.NDArray[np.float_]:
     assert 0 <= i < n <= N
 
     j = np.arange(floor(i), N)
 
     return np.r_[
         np.zeros(j[0]),
-        beta(j + 1, N - j)
-        / beta(i + 1, n - i)
-        / beta(j - i + 1, N - j - (n - i) + 1)
-        / (N - n + 1),
+        np.exp(
+            cast(
+                float,
+                betaln(j + 1, N - j)
+                - betaln(i + 1, n - i)
+                - betaln(j - i + 1, N - j - (n - i) + 1)
+                - np.log(N - n + 1),
+            ),
+        ),
     ]
 
 
 _weights_cached = functools.lru_cache(1 << 10)(_weights)
 
 
 def weights(
```

### Comparing `lmo-0.8.0/lmo/pwm_beta.py` & `lmo-0.9.0/lmo/pwm_beta.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,27 +45,27 @@
                [0.        , 0.        , 0.        , 0.05      , 0.2       ]])
 
     """
     if not (0 <= r <= n):
         msg = f'expected 0 <= r <= n, got {r=} and {n=}'
         raise ValueError(msg)
 
-    i1 = np.arange(1, n + 1)
+    i1 = np.arange(1, n + 1, dtype=dtype)
 
     w_r = np.zeros((r, n), dtype)
     if w_r.size == 0:
         return w_r
 
-    w_r[0] = 1.
+    w_r[0] = 1 / n
 
     for k in range(1, r):
         w_r[k, k:] = w_r[k - 1, k:] * i1[:-k] / (n - k)
 
     # the + 0. eliminates negative zeros
-    return cast(npt.NDArray[T], w_r / n + 0.)
+    return cast(npt.NDArray[T], w_r + 0.)
 
 
 def cov(
     a: npt.ArrayLike,
     r: int,
     /,
     axis: int | None = None,
```

### Comparing `lmo-0.8.0/lmo/theoretical.py` & `lmo-0.9.0/lmo/theoretical.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 import warnings
 from collections.abc import Callable
 from math import exp, gamma, lgamma
 from typing import Any, TypeAlias, cast, overload
 
 import numpy as np
 import numpy.typing as npt
+import scipy.integrate as sci  # type: ignore
+import scipy.special as scs  # type: ignore
 
 from ._utils import moments_to_ratio
 from .linalg import sh_jacobi
 from .typing import AnyFloat, AnyInt, IntVector
 
 _QuadFullOutput: TypeAlias = (
     tuple[float, float, dict[str, Any]]
@@ -37,54 +39,77 @@
     return (
         exp(lgamma(r + s + t + 1) - lgamma(r + s) - lgamma(r + t))
         * gamma(r - k)
         / r
     )
 
 
+def _quad(
+    integrand: Callable[[float], float],
+    support: tuple[AnyFloat, AnyFloat],
+    limit: int,
+    atol: float,
+    rtol: float,
+) -> float:
+    quad_val, _, _, *quad_tail = sci.quad(  # type: ignore
+        integrand,
+        *support,
+        full_output=True,
+        limit=limit,
+        epsabs=atol,
+        epsrel=rtol,
+    )
+    if quad_tail:
+        msg = f"'scipy.integrate.quad' failed: \n{quad_tail[0]}"
+        warnings.warn(msg, sci.IntegrationWarning, stacklevel=2)
+        return np.nan
+
+    return cast(float, quad_val)
+
+
 @overload
 def l_moment_from_cdf(
     cdf: Callable[[float], float],
     r: AnyInt,
     /,
     trim: tuple[AnyFloat, AnyFloat] = ...,
     *,
     support: tuple[AnyFloat, AnyFloat] = ...,
     rtol: float = ...,
     atol: float = ...,
-    limit: float = ...,
+    limit: int = ...,
 ) -> np.float_:
     ...
 
 
 @overload
 def l_moment_from_cdf(
     cdf: Callable[[float], float],
     r: IntVector,
     /,
     trim: tuple[AnyFloat, AnyFloat] = ...,
     *,
     support: tuple[AnyFloat, AnyFloat] = ...,
     rtol: float = ...,
     atol: float = ...,
-    limit: float = ...,
+    limit: int = ...,
 ) -> npt.NDArray[np.float_]:
     ...
 
 
-def l_moment_from_cdf(
+def l_moment_from_cdf(  # noqa: C901
     cdf: Callable[[float], float],
     r: AnyInt | IntVector,
     /,
     trim: tuple[AnyFloat, AnyFloat] = (0, 0),
     *,
     support: tuple[AnyFloat, AnyFloat] = (-np.inf, np.inf),
     rtol: float = 1.49e-8,
     atol: float = 1.49e-8,
-    limit: float = 100,
+    limit: int = 100,
 ) -> np.float_ | npt.NDArray[np.float_]:
     r"""
     Evaluate the population L-moment of a continuous probability distribution,
     using its Cumulative Distribution Function (CDF) $F_X(x) = P(X \le x)$.
 
     Notes:
         Numerical integration is performed with
@@ -146,68 +171,60 @@
     if _r.size == 0:
         return np.empty(_r.shape)
 
     r_vals, r_idxs = np.unique(_r, return_inverse=True)
     s, t = np.asanyarray(trim)
     trimmed = s != 0 or t != 0
 
-    j = sh_jacobi(r_vals[-1] - 1, t + 1, s + 1)
+    j = sh_jacobi(min(12, r_vals[-1]) - 1, t + 1, s + 1)
 
     # caching F(x) function only makes sense for multiple quad calls
     _cdf = functools.cache(cdf) if np.count_nonzero(r_vals) > 1 else cdf
 
-    # lazy import (don't worry; python imports are cached)
-    from scipy.integrate import IntegrationWarning, quad  # type: ignore
-
-    quad_kwargs = {'epsabs': atol, 'epsrel': rtol, 'limit': limit}
-
     l_r = np.empty(r_vals.shape)
     for i, r_val in np.ndenumerate(r_vals):
         if r_val == 0:
             # zeroth l-moment is always 1
             l_r[i] = 1
             continue
 
         if r_val == 1:
-            from scipy.special import betainc  # type: ignore
-
             def integrand(x: float, *args: Any) -> float:
                 # equivalent to E[X_{s+1 : s+t+1}]
                 # see Wiley (2003) eq. 2.1.5
-                p = _cdf(x, *args)
-                i_p = cast(float, betainc(s + 1, t + 1, p)) if trimmed else p
+                i_p = p = _cdf(x, *args)
+                if trimmed:
+                    i_p = scs.betainc(s + 1, t + 1, p)  # type: ignore
+
                 return (x >= 0) - i_p
 
         else:
-            # prepare the powers to use for evaluating the polynomial
-            k = cast(npt.NDArray[np.int_], np.arange(r_val - 1))
-            # grab the non-zero jacobi polynomial coefficients for k=r-1
-            j_k = j[r_val - 2, :r_val - 1]
+            k_val = r_val - 2
+
+            if r_val <= 12:
+                c_k, lb = j[k_val, :k_val + 1], 0
+            else:
+                _j_k = scs.jacobi(k_val, t + 1, s + 1)  # type: ignore
+                c_k, lb = _j_k.coef[::-1], -1
+
+            j_k = np.polynomial.Polynomial(c_k, domain=[0, 1], window=[lb, 1])
+
+            # avoid overflows: split in sign and log, and recombine later
+            # j_k_sgn = np.sign(j_k)
+            # j_k_ln = np.log(np.abs(j_k))
 
             def integrand(x: float, *args: Any) -> float:
-                # evaluate the jacobi polynomial for p at r-1 with (t, s)
-                # and multiply by the weight function
+                """
+                Evaluate the jacobi polynomial for p at r-1 with (t, s)
+                and multiply by the weight function.
+                """
                 p = _cdf(x, *args)
-                return p ** (s + 1) * (1 - p) ** (t + 1) * (j_k @ p**k)
-
-        # numerical integration
-        quad_val, _, _, *quad_tail = cast(
-            _QuadFullOutput,
-            quad(integrand, *support, full_output=True, **quad_kwargs),
-        )
-
-        if quad_tail:
-            quad_msg = quad_tail[0]
-            warnings.warn(
-                f"'scipy.integrate.quad' failed: \n{quad_msg}",
-                cast(type[UserWarning], IntegrationWarning),
-                stacklevel=2,
-            )
-            quad_val = np.nan
+                return p**(s + 1) * (1 - p)**(t + 1) * j_k(p)  # type: ignore
 
+        quad_val = _quad(integrand, support, limit, atol, rtol)
         l_r[i] = _l_moment_const(r_val, s, t, 1) * quad_val
 
     return (np.round(l_r, 12) + .0)[r_idxs].reshape(_r.shape)[()]
 
 
 @overload
 def l_moment_from_ppf(
@@ -215,44 +232,44 @@
     r: AnyInt,
     /,
     trim: tuple[AnyFloat, AnyFloat] = ...,
     *,
     support: tuple[AnyFloat, AnyFloat] = ...,
     rtol: float = ...,
     atol: float = ...,
-    limit: float = ...,
+    limit: int = ...,
 ) -> np.float_:
     ...
 
 
 @overload
 def l_moment_from_ppf(
     ppf: Callable[[float], float],
     r: IntVector,
     /,
     trim: tuple[AnyFloat, AnyFloat] = ...,
     *,
     support: tuple[AnyFloat, AnyFloat] = ...,
     rtol: float = ...,
     atol: float = ...,
-    limit: float = ...,
+    limit: int = ...,
 ) -> npt.NDArray[np.float_]:
     ...
 
 
 def l_moment_from_ppf(
     ppf: Callable[[float], float],
     r: AnyInt | IntVector,
     /,
     trim: tuple[AnyFloat, AnyFloat] = (0, 0),
     *,
     support: tuple[AnyFloat, AnyFloat] = (0, 1),
     rtol: float = 1.49e-8,
     atol: float = 1.49e-8,
-    limit: float = 100,
+    limit: int = 100,
 ) -> np.float_ | npt.NDArray[np.float_]:
     """
     Evaluate the population L-moment of a continuous probability distribution,
     using its Percentile Function (PPF) $Q_X(p) = F^{-1}_X(p)$,
     i.e. the inverse of the CDF, commonly known as the quantile function.
 
     Notes:
@@ -314,59 +331,49 @@
 
     if _r.size == 0:
         return np.empty(_r.shape)
 
     r_vals, r_idxs = np.unique(_r, return_inverse=True)
     s, t = np.asanyarray(trim)
 
-    j = sh_jacobi(r_vals[-1], t, s)
+    j = sh_jacobi(min(r_vals[-1], 12), t, s)
 
     def w(p: float, *args: Any) -> float:
         return p**s * (1 - p)**t * ppf(p, *args)
 
     # caching the weight function only makes sense for multiple quad calls
     _w = functools.cache(w) if len(r_vals) > 1 else w
 
     # lazy import (don't worry; python imports are cached)
-    from scipy.integrate import IntegrationWarning, quad  # type: ignore
-
-    quad_kwargs = {'epsabs': atol, 'epsrel': rtol, 'limit': limit}
+    from scipy.special import jacobi  # type: ignore
 
     l_r = np.empty(r_vals.shape)
     for i, r_val in np.ndenumerate(r_vals):
         if r_val == 0:
             # zeroth l-moment is always 1
             l_r[i] = 1
             continue
 
-        # prepare the powers to use for evaluating the polynomial
-        k = cast(npt.NDArray[np.int_], np.arange(r_val))
-        # grab the non-zero jacobi polynomial coefficients for k=r-1
-        j_k = j[r_val - 1, :r_val]
+        if r_val <= 12:
+            j_k = np.polynomial.Polynomial(
+                j[r_val - 1, :r_val],
+                domain=[0, 1],
+                window=[0, 1],
+            )
+        else:
+            j_k = np.polynomial.Polynomial(
+                jacobi(r_val - 1, t, s).coef[::-1],  # type: ignore
+                domain=[0, 1],
+                window=[-1, 1],
+            )
 
         def integrand(p: float) -> float:
-            # evaluate the jacobi polynomial for p at r-1 with (t, s)
-            # and multiply by the weight function
-            return _w(p) * (j_k @ p**k)  # type: ignore
-
-        # numerical integration
-        quad_val, _, _, *quad_tail = cast(
-            _QuadFullOutput,
-            quad(integrand, *support, full_output=True, **quad_kwargs),
-        )
-        if quad_tail:
-            quad_msg = quad_tail[0]
-            warnings.warn(
-                f"'scipy.integrate.quad' failed: \n{quad_msg}",
-                cast(type[UserWarning], IntegrationWarning),
-                stacklevel=2,
-            )
-            l_r[i] = np.nan
-            continue
+            return _w(p) * j_k(p)  # type: ignore
 
+        quad_val = _quad(integrand, support, limit, atol, rtol)
         l_r[i] = _l_moment_const(r_val, s, t, 0) * quad_val
 
     return (np.round(l_r, 12) + .0)[r_idxs].reshape(_r.shape)[()]
 
 
 @overload
 def l_ratio_from_cdf(
```

### Comparing `lmo-0.8.0/pyproject.toml` & `lmo-0.9.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core", "oldest-supported-numpy"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "lmo"
-version = "0.8.0"
+version = "0.9.0"
 description = "L-Moments for robust statistics."
 authors = ["Joren Hammudoglu <jhammudoglu@gmail.com>"]
 readme = "README.md"
 license = "BSD-3-Clause"
 homepage = "https://jorenham.github.io/lmo/"
 repository = "https://github.com/jorenham/lmo/"
 classifiers = [
@@ -40,24 +40,27 @@
 ]
 typing_extensions = { version = "^4.1", python = "<3.11"}
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4"
 hypothesis = {extras = ["numpy"], version = "^6.80"}
 pyright = "^1.1"
-ruff = ">=0.0.277,<1.0"
+ruff = ">=0.0.283,<1.0"
 
 [tool.poetry.group.docs.dependencies]
-mkdocs = "^1.4"
+mkdocs = "^1.5"
 mkdocs-material = "^9.1"
-mkdocs-include-markdown-plugin = { version = ">=4.0", python = "<3.12" }
+mkdocs-include-markdown-plugin = { version = ">=5.0", python = "<3.12" }
 mkdocstrings = {extras = ["python"], version = ">=0.22,<1.0"}
 
 [tool.poetry.group.debug.dependencies]
 ipython = "^8.14"
+ipykernel = "^6.25.0"
+matplotlib = "^3.7.2"
+line-profiler = "^4.0.3"
 
 
 [tool.pytest.ini_options]
 minversion = "7.0"
 addopts = [
     "-ra",
     "-W error",
@@ -78,15 +81,14 @@
 exclude = [
     "**/__pycache__",
     "**/.pytest_cache",
     "**/.hypothesis",
     "**/.pytest_cache",
     "**/.ruff_cache",
     "**/.vscode",
-    "**/.idea",
     ".git",
     ".github",
     "dist",
     "docs",
     "site",
     "tests",
 ]
@@ -97,15 +99,14 @@
 reportMissingImports = true
 reportMissingTypeStubs = true
 reportUnusedImport = true
 reportUnusedClass = true
 reportUnusedFunction = true
 reportUnusedVariable = true
 reportDuplicateImport = true
-useLibraryCodeForTypes = false
 
 
 [tool.ruff]
 target-version = "py310"
 
 src = ["lmo"]
 extend-exclude = ["tests"]
```

### Comparing `lmo-0.8.0/PKG-INFO` & `lmo-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmo
-Version: 0.8.0
+Version: 0.9.0
 Summary: L-Moments for robust statistics.
 Home-page: https://jorenham.github.io/lmo/
 License: BSD-3-Clause
 Author: Joren Hammudoglu
 Author-email: jhammudoglu@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -51,21 +51,41 @@
 
 Uniform or multi-dimensional, Lmo can summarize it all with one quick glance!
 
 ~~~
 
 Unlike the legacy [moments](https://wikipedia.org/wiki/Moment_(mathematics)),
 [L-moments](https://wikipedia.org/wiki/L-moment) **uniquely describe** a 
-probability distribution.
+probability distribution, and are more robust and efficient.
 The "L" stands for Linear; it is a linear combination of order statistics.
 So Lmo is as fast as sorting your samples (in terms of time-complexity).
 
-Even if your data is pathological like [Cauchy](https://wikipedia.org/wiki/Cauchy_distribution), 
-and the L-moments are not defined, the trimmed L-moments (TL-moments) can be 
-used instead:
+## Key Features:
+
+- Calculates trimmed L-moments and L-*co*moments, from data or a distribution
+  function.
+- Complete support for trimmed L-moment (TL-moments): 
+  `lmo.l_moment(..., trim=(1 / 137, 3.1416))`.
+- Fast estimation of L-*co*moment matrices from your multidimensional data.
+- A fully non-parametric `scipy.stats`-like distribution, `lmo.l_rv`.
+  It's very efficient, robust, fast, and requires only some L-mo's!
+- Exact (co)variance structure of the L-moment estimates.
+- Complete [docs](https://jorenham.github.io/lmo/), including overly 
+  complex $\TeX$ spaghetti equations.
+- Clean Pythonic syntax for ease of use.
+- Vectorized functions for very fast fitting.
+- Fully typed, tested, and tickled.
+
+
+## Quick example
+
+
+Even if your data is pathological like 
+[Cauchy](https://wikipedia.org/wiki/Cauchy_distribution), and the L-moments 
+are not defined, the trimmed L-moments (TL-moments) can be used instead:
 
 ```pycon
 >>> import numpy as np
 >>> import lmo
 >>> rng = np.random.default_rng(1980)
 >>> x = rng.standard_cauchy(96)  # pickle me, Lmo
 >>> x.mean(), x.std()  # don't try this at home
@@ -76,30 +96,32 @@
 
 For reference; the theoretical TL-location and TL-scale of the standard 
 Cauchy distribution are $\lambda^{(1, 1)}_{1} = 0$ and 
 $\lambda^{(1, 1)}_2 \approx 0.7$ 
 ([Elamir & Seheult, 2003](https://doi.org/10.1016/S0167-9473(02)00250-5)).
 
 
-## Key Features:
 
-- Calculates trimmed L-moments and L-*co*moments, from data and distributions.
-- Exact non-parametric variance structure of the sample estimates.
-- Coming soon: ~Robust distribution fitting; the method of L-moments~.
-- Complete [docs](https://jorenham.github.io/lmo/), including overly 
-  complex $\TeX$ spaghetti equations.
-- Clean Pythonic syntax for ease of use.
-- Vectorized functions for very fast fitting.
-- Fully typed, tested, and tickled.
+---
 
+See the [documentation](https://jorenham.github.io/lmo/) for more examples and
+the API reference.
 
----
 
-See the [documentation](https://jorenham.github.io/lmo/) for usage examples and code reference.
+## Roadmap:
 
+- Add methods to all `scipy.stats` univariate distributions, for finding 
+  the theoretical/population L-mo's.
+- Robust distribution fitting, using the (generalized) method of L-moments.
+- Theoretical L-moment variance structure calculation.
+- A generic goodness-of-fit test.
+- Automatic trim-length selection.
+- Plotting utilities (deps optional), e.g. for L-moment ratio diagrams.
+- Extended multivariate support, e.g. theoretical L-comoments, and 
+  L-regression.
 
 ## Installation
 
 Lmo is on [PyPI](https://pypi.org/project/lmo/), so you can do something like:
 
 ```shell
 pip install lmo
@@ -124,14 +146,11 @@
   sample L-moments](https://doi.org/10.1016/S0378-3758(03)00213-1)
 - [*J.R.M. Hosking* (2007) &ndash; Some theory and practical uses of trimmed 
   L-moments](https://doi.org/10.1016/j.jspi.2006.12.002)
 - [*R. Serﬂing & P. Xiao* (2007) &ndash; A contribution to multivariate 
   L-moments: L-comoment matrices](https://doi.org/10.1016/j.jmva.2007.01.008)
 - [*W.H. Asquith* (2011) &ndash; Univariate Distributional Analysis with 
   L-moment Statistics](https://hdl.handle.net/2346/ETD-TTU-2011-05-1319)
-- [*C. Dutang* (2017) &ndash; Theoretical L-moments and TL-moments Using
-  Combinatorial Identities and Finite Operators
-  ](https://doi.org/10.1080/03610926.2015.1073313)
 
 
 <!--overview-end-->
```

