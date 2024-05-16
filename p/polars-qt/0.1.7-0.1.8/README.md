# Comparing `tmp/polars_qt-0.1.7.tar.gz` & `tmp/polars_qt-0.1.8.tar.gz`

## Comparing `polars_qt-0.1.7.tar` & `polars_qt-0.1.8.tar`

### file list

```diff
@@ -1,28 +1,30 @@
--rw-r--r--   0        0        0      808 1970-01-01 00:00:00.000000 polars_qt-0.1.7/Cargo.toml
--rw-r--r--   0     1001      127     3716 2024-04-18 01:26:04.000000 polars_qt-0.1.7/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0     1001      127      111 2024-04-18 01:26:04.000000 polars_qt-0.1.7/.gitignore
--rw-r--r--   0     1001      127        8 2024-04-18 01:26:04.000000 polars_qt-0.1.7/.python-version
--rw-r--r--   0     1001      127      665 2024-04-18 01:26:04.000000 polars_qt-0.1.7/Makefile
--rw-r--r--   0     1001      127     1786 2024-04-18 01:26:04.000000 polars_qt-0.1.7/README.md
--rw-r--r--   0     1001      127       62 2024-04-18 01:26:04.000000 polars_qt-0.1.7/polars_qt/__init__.py
--rw-r--r--   0     1001      127     2898 2024-04-18 01:26:04.000000 polars_qt-0.1.7/polars_qt/funcs.py
--rw-r--r--   0     1001      127     3357 2024-04-18 01:26:04.000000 polars_qt-0.1.7/polars_qt/qt.py
--rw-r--r--   0     1001      127     6413 2024-04-18 01:26:04.000000 polars_qt-0.1.7/polars_qt/strategy.py
--rw-r--r--   0     1001      127     2567 2024-04-18 01:26:04.000000 polars_qt-0.1.7/polars_qt/utils.py
--rw-r--r--   0     1001      127       34 2024-04-18 01:26:04.000000 polars_qt-0.1.7/requirements.txt
--rw-r--r--   0     1001      127       42 2024-04-18 01:26:04.000000 polars_qt-0.1.7/rust-toolchain.toml
--rw-r--r--   0     1001      127     2054 2024-04-18 01:26:04.000000 polars_qt-0.1.7/src/equity.rs
--rw-r--r--   0     1001      127      649 2024-04-18 01:26:04.000000 polars_qt-0.1.7/src/if_then.rs
--rw-r--r--   0     1001      127      319 2024-04-18 01:26:04.000000 polars_qt-0.1.7/src/lib.rs
--rw-r--r--   0     1001      127     3250 2024-04-18 01:26:04.000000 polars_qt-0.1.7/src/rolling_rank.rs
--rw-r--r--   0     1001      127     1151 2024-04-18 01:26:04.000000 polars_qt-0.1.7/src/strategy/boll.rs
--rw-r--r--   0     1001      127      580 2024-04-18 01:26:04.000000 polars_qt-0.1.7/src/strategy/from_input.rs
--rw-r--r--   0     1001      127      672 2024-04-18 01:26:04.000000 polars_qt-0.1.7/src/strategy/martingale.rs
--rw-r--r--   0     1001      127       42 2024-04-18 01:26:04.000000 polars_qt-0.1.7/src/strategy/mod.rs
--rw-r--r--   0     1001      127     1375 2024-04-18 01:26:04.000000 polars_qt-0.1.7/tests/test_equity.py
--rw-r--r--   0     1001      127      867 2024-04-18 01:26:04.000000 polars_qt-0.1.7/tests/test_if_then.py
--rw-r--r--   0     1001      127      662 2024-04-18 01:26:04.000000 polars_qt-0.1.7/tests/test_rolling_rank.py
--rw-r--r--   0     1001      127     1919 2024-04-18 01:26:04.000000 polars_qt-0.1.7/tests/test_strategy.py
--rw-r--r--   0     1001      127    43211 2024-04-18 01:26:19.000000 polars_qt-0.1.7/Cargo.lock
--rw-r--r--   0     1001      127     1773 2024-04-18 01:26:04.000000 polars_qt-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2192 1970-01-01 00:00:00.000000 polars_qt-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      646 1970-01-01 00:00:00.000000 polars_qt-0.1.8/Cargo.toml
+-rw-r--r--   0     1001      127     3716 2024-04-23 07:29:12.000000 polars_qt-0.1.8/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0     1001      127      111 2024-04-23 07:29:12.000000 polars_qt-0.1.8/.gitignore
+-rw-r--r--   0     1001      127        8 2024-04-23 07:29:12.000000 polars_qt-0.1.8/.python-version
+-rw-r--r--   0     1001      127      665 2024-04-23 07:29:12.000000 polars_qt-0.1.8/Makefile
+-rw-r--r--   0     1001      127     1786 2024-04-23 07:29:12.000000 polars_qt-0.1.8/README.md
+-rw-r--r--   0     1001      127       62 2024-04-23 07:29:12.000000 polars_qt-0.1.8/polars_qt/__init__.py
+-rw-r--r--   0     1001      127     3143 2024-04-23 07:29:12.000000 polars_qt-0.1.8/polars_qt/funcs.py
+-rw-r--r--   0     1001      127     3429 2024-04-23 07:29:12.000000 polars_qt-0.1.8/polars_qt/qt.py
+-rw-r--r--   0     1001      127     6413 2024-04-23 07:29:12.000000 polars_qt-0.1.8/polars_qt/strategy.py
+-rw-r--r--   0     1001      127     2567 2024-04-23 07:29:12.000000 polars_qt-0.1.8/polars_qt/utils.py
+-rw-r--r--   0     1001      127       34 2024-04-23 07:29:12.000000 polars_qt-0.1.8/requirements.txt
+-rw-r--r--   0     1001      127       42 2024-04-23 07:29:12.000000 polars_qt-0.1.8/rust-toolchain.toml
+-rw-r--r--   0     1001      127     1993 2024-04-23 07:29:12.000000 polars_qt-0.1.8/src/compose.rs
+-rw-r--r--   0     1001      127     1598 2024-04-23 07:29:12.000000 polars_qt-0.1.8/src/equity.rs
+-rw-r--r--   0     1001      127      649 2024-04-23 07:29:12.000000 polars_qt-0.1.8/src/if_then.rs
+-rw-r--r--   0     1001      127      332 2024-04-23 07:29:12.000000 polars_qt-0.1.8/src/lib.rs
+-rw-r--r--   0     1001      127     3250 2024-04-23 07:29:12.000000 polars_qt-0.1.8/src/rolling_rank.rs
+-rw-r--r--   0     1001      127     1151 2024-04-23 07:29:12.000000 polars_qt-0.1.8/src/strategy/boll.rs
+-rw-r--r--   0     1001      127      580 2024-04-23 07:29:12.000000 polars_qt-0.1.8/src/strategy/from_input.rs
+-rw-r--r--   0     1001      127      672 2024-04-23 07:29:12.000000 polars_qt-0.1.8/src/strategy/martingale.rs
+-rw-r--r--   0     1001      127       42 2024-04-23 07:29:12.000000 polars_qt-0.1.8/src/strategy/mod.rs
+-rw-r--r--   0     1001      127      521 2024-04-23 07:29:12.000000 polars_qt-0.1.8/tests/test_compose_by.py
+-rw-r--r--   0     1001      127     1375 2024-04-23 07:29:12.000000 polars_qt-0.1.8/tests/test_equity.py
+-rw-r--r--   0     1001      127      867 2024-04-23 07:29:12.000000 polars_qt-0.1.8/tests/test_if_then.py
+-rw-r--r--   0     1001      127      662 2024-04-23 07:29:12.000000 polars_qt-0.1.8/tests/test_rolling_rank.py
+-rw-r--r--   0     1001      127     1919 2024-04-23 07:29:12.000000 polars_qt-0.1.8/tests/test_strategy.py
+-rw-r--r--   0     1001      127    43442 2024-04-23 07:29:28.000000 polars_qt-0.1.8/Cargo.lock
+-rw-r--r--   0     1001      127     1773 2024-04-23 07:29:12.000000 polars_qt-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2192 1970-01-01 00:00:00.000000 polars_qt-0.1.8/PKG-INFO
```

### Comparing `polars_qt-0.1.7/Cargo.toml` & `polars_qt-0.1.8/Cargo.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "polars-qt"
-version = "0.1.7"
+version = "0.1.8"
 edition = "2021"
 
 [lib]
 name = "polars_qt"
 crate-type= ["cdylib"]
 
 [features]
@@ -15,20 +15,12 @@
 [dependencies]
 itertools = "0.12.1"
 pyo3 = { version = "0.20.0", features = ["extension-module", "abi3-py38"] }
 pyo3-polars = { version = "0.12.0", features = ["derive"] }
 serde = { version = "1", features = ["derive"] }
 polars = { version = "0.38", default-features = false, features=["rolling_window", "temporal"] }
 
-# [dependencies.tevec]
-# git = "https://github.com/Teamon9161/tevec.git"
-# # rev = "4e89266"
-# branch = "master"
-# default-features = false
-# features = ["pl"]
-
-
 [dependencies.tea_strategy]
 git = "https://github.com/Teamon9161/tea_strategy.git"
-rev = "0c1e2fe"
+rev = "577932f"
 default-features = false
 features = ['pl']
```

### Comparing `polars_qt-0.1.7/.github/workflows/publish_to_pypi.yml` & `polars_qt-0.1.8/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.7/Makefile` & `polars_qt-0.1.8/Makefile`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.7/README.md` & `polars_qt-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.7/polars_qt/funcs.py` & `polars_qt-0.1.8/polars_qt/funcs.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,14 +39,23 @@
     expr2 = parse_into_expr(expr2)
     return register_plugin(
         args=[flag_expr, expr1, expr2],
         symbol="if_then",
         is_elementwise=False,
     )
 
+def compose_by(expr: IntoExpr, by: IntoExpr) -> pl.Expr:
+    expr = parse_into_expr(expr).diff()
+    by = parse_into_expr(by)
+    return register_plugin(
+        args=[expr, by],
+        symbol="compose_by",
+        is_elementwise=False,
+    )
+
 
 def calc_future_ret(
     signal: IntoExpr,
     open: IntoExpr,
     close: IntoExpr,
     *,
     is_signal: bool = True,
```

### Comparing `polars_qt-0.1.7/polars_qt/qt.py` & `polars_qt-0.1.8/polars_qt/qt.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,17 @@
         return rolling_rank(
             self.expr, window=window, min_periods=min_periods, pct=pct, rev=rev
         )
 
     def if_then(self, flag, then):
         return if_then(flag, then, self.expr)
 
+    def compose_by(self, by):
+        return compose_by(self.expr, by)
+
     def calc_future_ret(
         self,
         open: IntoExpr,
         close: IntoExpr,
         *,
         is_signal: bool = True,
         init_cash: int = 10_000_000,
```

### Comparing `polars_qt-0.1.7/polars_qt/strategy.py` & `polars_qt-0.1.8/polars_qt/strategy.py`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.7/polars_qt/utils.py` & `polars_qt-0.1.8/polars_qt/utils.py`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.7/src/equity.rs` & `polars_qt-0.1.8/src/equity.rs`

 * *Files 17% similar despite different names*

```diff
@@ -2,36 +2,14 @@
 use polars::prelude::*;
 use pyo3_polars::derive::polars_expr;
 // use serde::Deserialize;
 
 use tea_strategy::equity;
 use tea_strategy::equity::{FutureRetKwargs, FutureRetSpreadKwargs};
 
-// #[derive(Deserialize)]
-// struct FutureRetKwargs {
-//     init_cash: usize,
-//     multiplier: f64,
-//     leverage: f64,
-//     slippage: f64,
-//     ticksize: f64,
-//     c_rate: f64,
-//     blowup: bool,
-//     commision_type: String,
-// }
-
-// #[derive(Deserialize)]
-// struct FutureRetSpreadKwargs {
-//     init_cash: usize,
-//     multiplier: f64,
-//     leverage: f64,
-//     c_rate: f64,
-//     blowup: bool,
-//     commision_type: String,
-// }
-
 #[polars_expr(output_type=Float64)]
 fn calc_future_ret(inputs: &[Series], kwargs: FutureRetKwargs) -> PolarsResult<Series> {
     let (pos, opening_cost, closing_cost) = (&inputs[0], &inputs[1], &inputs[2]);
     let pos = pos.f64()?;
     let opening_cost = opening_cost.f64()?;
     let closing_cost = closing_cost.f64()?;
     let contract_chg_signal = if inputs.len() == 3 {
```

### Comparing `polars_qt-0.1.7/src/if_then.rs` & `polars_qt-0.1.8/src/if_then.rs`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.7/src/rolling_rank.rs` & `polars_qt-0.1.8/src/rolling_rank.rs`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.7/src/strategy/boll.rs` & `polars_qt-0.1.8/src/strategy/boll.rs`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.7/src/strategy/from_input.rs` & `polars_qt-0.1.8/src/strategy/from_input.rs`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.7/src/strategy/martingale.rs` & `polars_qt-0.1.8/src/strategy/martingale.rs`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.7/tests/test_equity.py` & `polars_qt-0.1.8/tests/test_equity.py`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.7/tests/test_if_then.py` & `polars_qt-0.1.8/tests/test_if_then.py`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.7/tests/test_rolling_rank.py` & `polars_qt-0.1.8/tests/test_rolling_rank.py`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.7/tests/test_strategy.py` & `polars_qt-0.1.8/tests/test_strategy.py`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.7/Cargo.lock` & `polars_qt-0.1.8/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -135,20 +135,21 @@
 name = "bytes"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cc"
-version = "1.0.94"
+version = "1.0.95"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "17f6e324229dc011159fcc089755d1e2e216a90d43a7dea6853ca740b84f35e7"
+checksum = "d32a725bc159af97c3e629873bb9f88fb8cf8a4867175f76dc987815ea07c83b"
 dependencies = [
  "jobserver",
  "libc",
+ "once_cell",
 ]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
@@ -371,17 +372,17 @@
 name = "itoa"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "jobserver"
-version = "0.1.30"
+version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "685a7d121ee3f65ae4fddd72b25a04bb36b6af81bc0828f7d5434c0fe60fa3a2"
+checksum = "d2b099aaa34a9751c5bf0878add70444e1ed2dd73f347be99003d4577277de6e"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "js-sys"
 version = "0.3.69"
@@ -854,15 +855,15 @@
  "smartstring",
  "strum_macros",
  "version_check",
 ]
 
 [[package]]
 name = "polars-qt"
-version = "0.1.7"
+version = "0.1.8"
 dependencies = [
  "itertools",
  "polars",
  "pyo3",
  "pyo3-polars",
  "serde",
  "tea_strategy",
@@ -1290,17 +1291,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "sysinfo"
-version = "0.30.10"
+version = "0.30.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26d7c217777061d5a2d652aea771fb9ba98b6dade657204b08c4b9604d11555b"
+checksum = "87341a165d73787554941cd5ef55ad728011566fe714e987d1b976c15dbc3a83"
 dependencies = [
  "cfg-if",
  "core-foundation-sys",
  "libc",
  "ntapi",
  "once_cell",
  "windows",
@@ -1316,75 +1317,85 @@
 name = "target-lexicon"
 version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "tea-core"
-version = "0.1.1"
-source = "git+https://github.com/Teamon9161/tevec.git?branch=master#3abf4cd9a3e775d724585be4c503a205b99113a2"
+version = "0.1.2"
+source = "git+https://github.com/Teamon9161/tevec.git?branch=master#2fe153b8e1c3de7188f15881532e868435da6ca1"
 dependencies = [
  "num-traits",
  "polars",
  "polars-arrow",
  "serde",
  "tea-dtype",
 ]
 
 [[package]]
 name = "tea-dtype"
-version = "0.1.1"
-source = "git+https://github.com/Teamon9161/tevec.git?branch=master#3abf4cd9a3e775d724585be4c503a205b99113a2"
+version = "0.1.2"
+source = "git+https://github.com/Teamon9161/tevec.git?branch=master#2fe153b8e1c3de7188f15881532e868435da6ca1"
+dependencies = [
+ "num-traits",
+]
+
+[[package]]
+name = "tea-map"
+version = "0.1.2"
+source = "git+https://github.com/Teamon9161/tevec.git?branch=master#2fe153b8e1c3de7188f15881532e868435da6ca1"
 dependencies = [
  "num-traits",
+ "tea-core",
 ]
 
 [[package]]
 name = "tea-rolling"
-version = "0.1.1"
-source = "git+https://github.com/Teamon9161/tevec.git?branch=master#3abf4cd9a3e775d724585be4c503a205b99113a2"
+version = "0.1.2"
+source = "git+https://github.com/Teamon9161/tevec.git?branch=master#2fe153b8e1c3de7188f15881532e868435da6ca1"
 dependencies = [
  "num-traits",
  "tea-core",
 ]
 
 [[package]]
 name = "tea_strategy"
 version = "0.1.0"
-source = "git+https://github.com/Teamon9161/tea_strategy.git?rev=0c1e2fe#0c1e2fe8f66bc887f9a172645635158223aa0249"
+source = "git+https://github.com/Teamon9161/tea_strategy.git?rev=577932f#577932f9989c4df65a815a5b514cb7a036ccaa4c"
 dependencies = [
  "itertools",
  "serde",
  "tevec",
 ]
 
 [[package]]
 name = "tevec"
-version = "0.1.1"
-source = "git+https://github.com/Teamon9161/tevec.git?branch=master#3abf4cd9a3e775d724585be4c503a205b99113a2"
+version = "0.1.2"
+source = "git+https://github.com/Teamon9161/tevec.git?branch=master#2fe153b8e1c3de7188f15881532e868435da6ca1"
 dependencies = [
  "tea-core",
  "tea-dtype",
+ "tea-map",
  "tea-rolling",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.58"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
+checksum = "f0126ad08bff79f29fc3ae6a55cc72352056dfff61e3ff8bb7129476d44b23aa"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.58"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
+checksum = "d1cd413b5d558b4c5bf3680e324a6fa5014e7b7c067a51e69dbdf47eb7148b66"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.60",
 ]
 
 [[package]]
```

### Comparing `polars_qt-0.1.7/pyproject.toml` & `polars_qt-0.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.7/PKG-INFO` & `polars_qt-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: polars-qt
-Version: 0.1.7
+Version: 0.1.8
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: polars >=0.20.16
 Author-email: Teamon9161 <teamon9161@163.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

