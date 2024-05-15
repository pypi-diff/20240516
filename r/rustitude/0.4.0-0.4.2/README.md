# Comparing `tmp/rustitude-0.4.0.tar.gz` & `tmp/rustitude-0.4.2.tar.gz`

## Comparing `rustitude-0.4.0.tar` & `rustitude-0.4.2.tar`

### file list

```diff
@@ -1,50 +1,65 @@
--rw-r--r--   0     1001      127      843 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-core/Cargo.toml
--rw-r--r--   0     1001      127      316 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-core/.github/workflows/rust.yml
--rw-r--r--   0     1001      127       66 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-core/.gitignore
--rw-r--r--   0     1001      127    15381 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-core/CHANGELOG.md
--rw-r--r--   0     1001      127     1509 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-core/LICENSE
--rw-r--r--   0     1001      127    11271 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-core/README.md
--rw-r--r--   0     1001      127     2773 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-core/bacon.toml
--rw-r--r--   0     1001      127    32108 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-core/media/logo.png
--rw-r--r--   0     1001      127    37710 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-core/src/amplitude.rs
--rw-r--r--   0     1001      127    25986 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-core/src/dataset.rs
--rw-r--r--   0     1001      127     1596 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-core/src/docs-header.html
--rw-r--r--   0     1001      127    10542 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-core/src/four_momentum.rs
--rw-r--r--   0     1001      127      826 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-core/src/lib.rs
--rw-r--r--   0     1001      127     2334 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-core/src/manager.rs
--rw-r--r--   0     1001      127      566 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-gluex/Cargo.toml
--rw-r--r--   0     1001      127      316 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-gluex/.github/workflows/rust.yml
--rw-r--r--   0     1001      127       14 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-gluex/.gitignore
--rw-r--r--   0     1001      127     5364 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-gluex/CHANGELOG.md
--rw-r--r--   0     1001      127     1507 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-gluex/LICENSE
--rw-r--r--   0     1001      127    14640 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-gluex/README.md
--rw-r--r--   0     1001      127     2773 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-gluex/bacon.toml
--rw-r--r--   0     1001      127    24055 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-gluex/media/logo.png
--rw-r--r--   0     1001      127     3086 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-gluex/src/dalitz.rs
--rw-r--r--   0     1001      127     8462 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-gluex/src/harmonics.rs
--rw-r--r--   0     1001      127       85 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-gluex/src/lib.rs
--rw-r--r--   0     1001      127    22294 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-gluex/src/resonances.rs
--rw-r--r--   0     1001      127     7565 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-gluex/src/sdmes.rs
--rw-r--r--   0     1001      127     7940 2024-05-15 00:01:52.000000 rustitude-0.4.0/crates/rustitude-gluex/src/utils.rs
--rw-r--r--   0        0        0      732 1970-01-01 00:00:00.000000 rustitude-0.4.0/Cargo.toml
--rw-r--r--   0     1001      127     3469 2024-05-15 00:01:52.000000 rustitude-0.4.0/.github/workflows/maturin.yml
--rw-r--r--   0     1001      127      316 2024-05-15 00:01:52.000000 rustitude-0.4.0/.github/workflows/rust.yml
--rw-r--r--   0     1001      127     3144 2024-05-15 00:01:52.000000 rustitude-0.4.0/.gitignore
--rw-r--r--   0     1001      127      159 2024-05-15 00:01:52.000000 rustitude-0.4.0/.justfile
--rw-r--r--   0     1001      127    13263 2024-05-15 00:01:52.000000 rustitude-0.4.0/CHANGELOG.md
--rw-r--r--   0     1001      127     1507 2024-05-15 00:01:52.000000 rustitude-0.4.0/LICENSE
--rw-r--r--   0     1001      127    10688 2024-05-15 00:01:52.000000 rustitude-0.4.0/README.md
--rw-r--r--   0     1001      127     2846 2024-05-15 00:01:52.000000 rustitude-0.4.0/bacon.toml
--rw-r--r--   0     1001      127    32108 2024-05-15 00:01:52.000000 rustitude-0.4.0/media/logo.png
--rw-r--r--   0     1001      127     1841 2024-05-15 00:01:52.000000 rustitude-0.4.0/rustitude/__init__.py
--rw-r--r--   0     1001      127     4013 2024-05-15 00:01:52.000000 rustitude-0.4.0/rustitude/__init__.pyi
--rw-r--r--   0     1001      127       90 2024-05-15 00:01:52.000000 rustitude-0.4.0/rustitude/gluex/__init__.pyi
--rw-r--r--   0     1001      127       75 2024-05-15 00:01:52.000000 rustitude-0.4.0/rustitude/gluex/dalitz.pyi
--rw-r--r--   0     1001      127     3778 2024-05-15 00:01:52.000000 rustitude-0.4.0/rustitude/gluex/harmonics.pyi
--rw-r--r--   0     1001      127      535 2024-05-15 00:01:52.000000 rustitude-0.4.0/rustitude/gluex/resonances.pyi
--rw-r--r--   0     1001      127      336 2024-05-15 00:01:52.000000 rustitude-0.4.0/rustitude/gluex/sdmes.pyi
--rw-r--r--   0     1001      127        0 2024-05-15 00:01:52.000000 rustitude-0.4.0/rustitude/py.typed
--rw-r--r--   0     1001      127     1654 2024-05-15 00:01:52.000000 rustitude-0.4.0/src/lib.rs
--rw-r--r--   0     1001      127    38250 2024-05-15 00:01:52.000000 rustitude-0.4.0/Cargo.lock
--rw-r--r--   0     1001      127     1029 2024-05-15 00:01:52.000000 rustitude-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    11471 1970-01-01 00:00:00.000000 rustitude-0.4.0/PKG-INFO
+-rw-r--r--   0     1001      127      838 2024-05-15 23:43:39.000000 rustitude-0.4.2/crates/rustitude-core/Cargo.toml
+-rw-r--r--   0     1001      127      316 2024-05-15 23:43:39.000000 rustitude-0.4.2/crates/rustitude-core/.github/workflows/rust.yml
+-rw-r--r--   0     1001      127       66 2024-05-15 23:43:39.000000 rustitude-0.4.2/crates/rustitude-core/.gitignore
+-rw-r--r--   0     1001      127    15381 2024-05-15 23:43:39.000000 rustitude-0.4.2/crates/rustitude-core/CHANGELOG.md
+-rw-r--r--   0     1001      127    10767 2024-05-15 23:43:39.000000 rustitude-0.4.2/crates/rustitude-core/README.md
+-rw-r--r--   0     1001      127    32108 2024-05-15 23:43:39.000000 rustitude-0.4.2/crates/rustitude-core/media/logo.png
+-rw-r--r--   0     1001      127    37710 2024-05-15 23:43:39.000000 rustitude-0.4.2/crates/rustitude-core/src/amplitude.rs
+-rw-r--r--   0     1001      127    25986 2024-05-15 23:43:39.000000 rustitude-0.4.2/crates/rustitude-core/src/dataset.rs
+-rw-r--r--   0     1001      127     1596 2024-05-15 23:43:39.000000 rustitude-0.4.2/crates/rustitude-core/src/docs-header.html
+-rw-r--r--   0     1001      127    10542 2024-05-15 23:43:39.000000 rustitude-0.4.2/crates/rustitude-core/src/four_momentum.rs
+-rw-r--r--   0     1001      127      826 2024-05-15 23:43:39.000000 rustitude-0.4.2/crates/rustitude-core/src/lib.rs
+-rw-r--r--   0     1001      127     2334 2024-05-15 23:43:39.000000 rustitude-0.4.2/crates/rustitude-core/src/manager.rs
+-rw-r--r--   0     1001      127      500 2024-05-15 23:43:39.000000 rustitude-0.4.2/crates/rustitude/Cargo.toml
+-rw-r--r--   0     1001      127    14891 2024-05-15 23:43:39.000000 rustitude-0.4.2/crates/rustitude/CHANGELOG.md
+-rw-r--r--   0     1001      127    32108 2024-05-15 23:43:39.000000 rustitude-0.4.2/crates/rustitude/media/logo.png
+-rw-r--r--   0     1001      127     1029 2024-05-15 23:43:39.000000 rustitude-0.4.2/crates/rustitude/pyproject.toml
+-rw-r--r--   0     1001      127     1841 2024-05-15 23:43:39.000000 rustitude-0.4.2/crates/rustitude/rustitude/__init__.py
+-rw-r--r--   0     1001      127     4013 2024-05-15 23:43:39.000000 rustitude-0.4.2/crates/rustitude/rustitude/__init__.pyi
+-rw-r--r--   0     1001      127       90 2024-05-15 23:43:39.000000 rustitude-0.4.2/crates/rustitude/rustitude/gluex/__init__.pyi
+-rw-r--r--   0     1001      127       75 2024-05-15 23:43:39.000000 rustitude-0.4.2/crates/rustitude/rustitude/gluex/dalitz.pyi
+-rw-r--r--   0     1001      127     3778 2024-05-15 23:43:39.000000 rustitude-0.4.2/crates/rustitude/rustitude/gluex/harmonics.pyi
+-rw-r--r--   0     1001      127      535 2024-05-15 23:43:39.000000 rustitude-0.4.2/crates/rustitude/rustitude/gluex/resonances.pyi
+-rw-r--r--   0     1001      127      336 2024-05-15 23:43:39.000000 rustitude-0.4.2/crates/rustitude/rustitude/gluex/sdmes.pyi
+-rw-r--r--   0     1001      127        0 2024-05-15 23:43:39.000000 rustitude-0.4.2/crates/rustitude/rustitude/py.typed
+-rw-r--r--   0     1001      127      137 2024-05-15 23:43:39.000000 rustitude-0.4.2/crates/rustitude/src/lib.rs
+-rw-r--r--   0     1001      127    10267 2024-05-15 23:43:39.000000 rustitude-0.4.2/README.md
+-rw-r--r--   0     1001      127      504 2024-05-15 23:43:39.000000 rustitude-0.4.2/crates/rustitude-gluex/Cargo.toml
+-rw-r--r--   0     1001      127      316 2024-05-15 23:43:39.000000 rustitude-0.4.2/crates/rustitude-gluex/.github/workflows/rust.yml
+-rw-r--r--   0     1001      127       14 2024-05-15 23:43:39.000000 rustitude-0.4.2/crates/rustitude-gluex/.gitignore
+-rw-r--r--   0     1001      127     7243 2024-05-15 23:43:39.000000 rustitude-0.4.2/crates/rustitude-gluex/CHANGELOG.md
+-rw-r--r--   0     1001      127    14640 2024-05-15 23:43:39.000000 rustitude-0.4.2/crates/rustitude-gluex/README.md
+-rw-r--r--   0     1001      127    24055 2024-05-15 23:43:39.000000 rustitude-0.4.2/crates/rustitude-gluex/media/logo.png
+-rw-r--r--   0     1001      127     3086 2024-05-15 23:43:39.000000 rustitude-0.4.2/crates/rustitude-gluex/src/dalitz.rs
+-rw-r--r--   0     1001      127     8462 2024-05-15 23:43:39.000000 rustitude-0.4.2/crates/rustitude-gluex/src/harmonics.rs
+-rw-r--r--   0     1001      127       85 2024-05-15 23:43:39.000000 rustitude-0.4.2/crates/rustitude-gluex/src/lib.rs
+-rw-r--r--   0     1001      127    22294 2024-05-15 23:43:39.000000 rustitude-0.4.2/crates/rustitude-gluex/src/resonances.rs
+-rw-r--r--   0     1001      127     7565 2024-05-15 23:43:39.000000 rustitude-0.4.2/crates/rustitude-gluex/src/sdmes.rs
+-rw-r--r--   0     1001      127     7940 2024-05-15 23:43:39.000000 rustitude-0.4.2/crates/rustitude-gluex/src/utils.rs
+-rw-r--r--   0        0        0      428 1970-01-01 00:00:00.000000 rustitude-0.4.2/py-rustitude/Cargo.toml
+-rw-r--r--   0     1001      127    13135 2024-05-15 23:43:39.000000 rustitude-0.4.2/py-rustitude/CHANGELOG.md
+-rw-r--r--   0     1001      127     1507 2024-05-15 23:43:39.000000 rustitude-0.4.2/py-rustitude/LICENSE
+-rw-r--r--   0     1001      127    10267 2024-05-15 23:43:39.000000 rustitude-0.4.2/py-rustitude/README.md
+-rw-r--r--   0     1001      127     2846 2024-05-15 23:43:39.000000 rustitude-0.4.2/py-rustitude/bacon.toml
+-rw-r--r--   0     1001      127     1841 2024-05-15 23:43:39.000000 rustitude-0.4.2/py-rustitude/rustitude/__init__.py
+-rw-r--r--   0     1001      127     4013 2024-05-15 23:43:39.000000 rustitude-0.4.2/py-rustitude/rustitude/__init__.pyi
+-rw-r--r--   0     1001      127       90 2024-05-15 23:43:39.000000 rustitude-0.4.2/py-rustitude/rustitude/gluex/__init__.pyi
+-rw-r--r--   0     1001      127       75 2024-05-15 23:43:39.000000 rustitude-0.4.2/py-rustitude/rustitude/gluex/dalitz.pyi
+-rw-r--r--   0     1001      127     3778 2024-05-15 23:43:39.000000 rustitude-0.4.2/py-rustitude/rustitude/gluex/harmonics.pyi
+-rw-r--r--   0     1001      127      535 2024-05-15 23:43:39.000000 rustitude-0.4.2/py-rustitude/rustitude/gluex/resonances.pyi
+-rw-r--r--   0     1001      127      336 2024-05-15 23:43:39.000000 rustitude-0.4.2/py-rustitude/rustitude/gluex/sdmes.pyi
+-rw-r--r--   0     1001      127        0 2024-05-15 23:43:39.000000 rustitude-0.4.2/py-rustitude/rustitude/py.typed
+-rw-r--r--   0     1001      127     1487 2024-05-15 23:43:39.000000 rustitude-0.4.2/py-rustitude/src/lib.rs
+-rw-r--r--   0     1001      127    44937 2024-05-15 23:43:39.000000 rustitude-0.4.2/Cargo.lock
+-rw-r--r--   0        0        0     1107 1970-01-01 00:00:00.000000 rustitude-0.4.2/Cargo.toml
+-rw-r--r--   0        0        0     1071 1970-01-01 00:00:00.000000 rustitude-0.4.2/pyproject.toml
+-rw-r--r--   0     1001      127     1841 2024-05-15 23:43:39.000000 rustitude-0.4.2/rustitude/__init__.py
+-rw-r--r--   0     1001      127        0 2024-05-15 23:43:39.000000 rustitude-0.4.2/rustitude/py.typed
+-rw-r--r--   0     1001      127     4013 2024-05-15 23:43:39.000000 rustitude-0.4.2/rustitude/__init__.pyi
+-rw-r--r--   0     1001      127       75 2024-05-15 23:43:39.000000 rustitude-0.4.2/rustitude/gluex/dalitz.pyi
+-rw-r--r--   0     1001      127      535 2024-05-15 23:43:39.000000 rustitude-0.4.2/rustitude/gluex/resonances.pyi
+-rw-r--r--   0     1001      127       90 2024-05-15 23:43:39.000000 rustitude-0.4.2/rustitude/gluex/__init__.pyi
+-rw-r--r--   0     1001      127      336 2024-05-15 23:43:39.000000 rustitude-0.4.2/rustitude/gluex/sdmes.pyi
+-rw-r--r--   0     1001      127     3778 2024-05-15 23:43:39.000000 rustitude-0.4.2/rustitude/gluex/harmonics.pyi
+-rw-r--r--   0     1001      127     1507 2024-05-15 23:43:39.000000 rustitude-0.4.2/LICENSE
+-rw-r--r--   0        0        0    10997 1970-01-01 00:00:00.000000 rustitude-0.4.2/PKG-INFO
```

### Comparing `rustitude-0.4.0/crates/rustitude-core/CHANGELOG.md` & `rustitude-0.4.2/crates/rustitude-core/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `rustitude-0.4.0/crates/rustitude-core/LICENSE` & `rustitude-0.4.2/py-rustitude/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2023, Nathaniel Dene Hoffman
+Copyright (c) 2024, Nathaniel D. Hoffman
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `rustitude-0.4.0/crates/rustitude-core/README.md` & `rustitude-0.4.2/crates/rustitude-core/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -34,22 +34,14 @@
 
 This crate contains all of the core mechanics
 
 - `rustitude` will automatically parallelize amplitudes over the events in a dataset. There's no reason for a developer to ever write parallelized code themselves.
 - Implementing [`Node`](https://docs.rs/rustitude-core/latest/rustitude_core/amplitude/trait.Node.html) on a struct is all that is needed to use it as an amplitude. This means developers need only write two to three total methods to describe the entire functionality of their amplitude, and one of these just gives the names and order of the amplitude's input parameters.
 - A major goal of `rustitude` was to increase processing speed by sacrificing memory. This is done by precalculating parts of amplitudes which don't change when the free parameter inputs change. The simplest example of this is the `Ylm` amplitude (spherical harmonic), which can be entirely precalculated given the value of `l` and `m`. To calculate this amplitude at evaluation time, `rustitude` just needs to look up a value in an array!
 
-# Theory
-
-Amplitudes are registered into a named `sum` and `group`. Similar to [`AmpTools`](https://github.com/mashephe/AmpTools), the typical calculation for any event $e$ and list of parameters $\overrightarrow{p}$ will then be:
-
-```math
-I(\overrightarrow{p}, e) = \sum_{\text{groups} \in \text{sums}}\left|\sum_{\text{amplitudes} \in \text{groups}} \prod_{\text{amp} \in \text{amplitudes}} \text{amp}(\overrightarrow{p}, e)\right|^2
-```
-
 # Installation
 
 Cargo provides the usual command for including this crate in a project:
 
 ```shell
 cargo add rustitude-core
 ```
@@ -72,15 +64,15 @@
 pub struct OmegaDalitz {
     dalitz_z: Vec<f64>,
     dalitz_sin3theta: Vec<f64>,
     lambda: Vec<f64>,
 }
 
 impl Node for OmegaDalitz {
-    fn precalculate(&mut self, dataset: &Dataset) {
+    fn precalculate(&mut self, dataset: &Dataset) -> Result<(), NodeError> {
         (self.dalitz_z, (self.dalitz_sin3theta, self.lambda)) = dataset
             .events
             .read()
             .par_iter()
             .map(|event| {
                 let pi0 = event.daughter_p4s[0];
                 let pip = event.daughter_p4s[1];
@@ -106,82 +98,82 @@
 
                 let lambda = (4.0 / 3.0) * f64::abs(pi_cross.dot(&pi_cross))
                     / ((1.0 / 9.0) * (omega.m2() - (2.0 * pip.m() + pi0.m()).powi(2)).powi(2));
 
                 (dalitz_z, (dalitz_sin3theta, lambda))
             })
             .unzip();
+        Ok(())
     }
 
-    fn calculate(&self, parameters: &[f64], event: &Event) -> Complex64 {
+    fn calculate(&self, parameters: &[f64], event: &Event) -> Result<Complex64, NodeError> {
         let dalitz_z = self.dalitz_z[event.index];
         let dalitz_sin3theta = self.dalitz_sin3theta[event.index];
         let lambda = self.lambda[event.index];
         let alpha = parameters[0];
         let beta = parameters[1];
         let gamma = parameters[2];
         let delta = parameters[3];
-        f64::sqrt(f64::abs(
+        Ok(f64::sqrt(f64::abs(
             lambda
                 * (1.0
                     + 2.0 * alpha * dalitz_z
                     + 2.0 * beta * dalitz_z.powf(3.0 / 2.0) * dalitz_sin3theta
                     + 2.0 * gamma * dalitz_z.powi(2)
                     + 2.0 * delta * dalitz_z.powf(5.0 / 2.0) * dalitz_sin3theta),
         ))
-        .into()
+        .into())
     }
 
-    fn parameters(&self) -> Option<Vec<String>> {
-        Some(vec![
+    fn parameters(&self) -> Vec<String> {
+        vec![
             "alpha".to_string(),
             "beta".to_string(),
             "gamma".to_string(),
             "delta".to_string(),
-        ])
+        ]
     }
 }
 ```
 
-Let's walk through this code. First, we need to define a `struct` which has all of the general information about the amplitude, and in this case some kind of `Vec` for storing precalculated data. We consider this precalculated data to correspond to a single dataset, and each dataset gets its own copy of the amplitude `struct`. Because this particular amplitude doesn't have any input parameters, we can `#[derive(Default)]` on it to make a default constructor, which allows the amplitude to be initialized with something like `let amp = OmegaDalitz::default();`. If we wanted a parameterized constructor, we have to define our own, and while Rust has no default name for constructors, `pub fn new(...) -> Self` is preferred.
+Let's walk through this code. First, we need to define a `struct` which has all of the general information about the amplitude, and in this case some kind of `Vec` for storing precalculated data. We consider this precalculated data to correspond to a single dataset, and each dataset gets its own copy of the amplitude `struct`. Because this particular amplitude doesn't have any input parameters, we can `#[derive(Default)]` on it to make a default constructor, which allows the amplitude to be initialized with something like `let amp = OmegaDalitz::default();`. If we wanted a parameterized constructor, we have to define our own, and while Rust has no default name for constructors, `pub fn new(...) -> rustitude_core::AmpOp` is preferred.
 
-Next, we implement the `Node` trait for the `struct`. Traits in Rust are kind of like abstract classes or interfaces in object-oriented languages, they provide some set of methods which a `struct` must implement. The first of these methods is `fn precalculate(&mut self, dataset: &Dataset)`. As the signature suggests, it takes a `Dataset` and mutates the `struct` in some way. The intended usage of this function is to precalculate some terms in the amplitude's mathematical expression, things which don't change when you update the free parameter inputs to the amplitude. In this case, the four input parameters, $`\alpha`$, $`\beta`$, $`\gamma`$, and $`\delta`$, are independent from `dalitz_z`, `dalitz_sin3theta`, and `lambda`, so we can safely calculate those ahead of time and just pull from their respective `Vec`s when needed later. I won't go too far into Rust's syntax here, but typical precalculation functions will start by iterating over the dataset's events in parallel (the line `use rayon::prelude::*;` is needed to use `par_iter` here) and collecting or unzipping that iterator into a `Vec` or group of `Vec`s.
+Next, we implement the `Node` trait for the `struct`. Traits in Rust are kind of like abstract classes or interfaces in object-oriented languages, they provide some set of methods which a `struct` must implement. The first of these methods is `fn precalculate(&mut self, dataset: &Dataset) -> Result<(), NodeError>`. As the signature suggests, it takes a `Dataset` and mutates the `struct` in some way. It should raise a `NodeError` if anything goes wrong in the evaluation. The intended usage of this function is to precalculate some terms in the amplitude's mathematical expression, things which don't change when you update the free parameter inputs to the amplitude. In this case, the four input parameters, $`\alpha`$, $`\beta`$, $`\gamma`$, and $`\delta`$, are independent from `dalitz_z`, `dalitz_sin3theta`, and `lambda`, so we can safely calculate those ahead of time and just pull from their respective `Vec`s when needed later. I won't go too far into Rust's syntax here, but typical precalculation functions will start by iterating over the dataset's events in parallel (the line `use rayon::prelude::*;` is needed to use `par_iter` here) and collecting or unzipping that iterator into a `Vec` or group of `Vec`s.
 
-The calculate step has the signature `fn calculate(&self, parameters: &[f64], event: &Event) -> Complex64`. This means we need to take a list of parameters and a single event and turn them into a complex value. The `Event` struct contains an `index` field which can be used to access the precalculated storage arrays made in the previous step.
+The calculate step has the signature `fn calculate(&self, parameters: &[f64], event: &Event) -> Result<Complex64, NodeError>`. This means we need to take a list of parameters and a single event and turn them into a complex value. The `Event` struct contains an `index` field which can be used to access the precalculated storage arrays made in the previous step.
 
-Finally, the `parameters` function just returns a list of the parameter names in the order they are expected to be input into `calculate`. In the event that an amplitude doesn't have any free parameters (like [my implementation of the `Ylm` and `Zlm` amplitudes](https://github.com/denehoffman/rustitude/blob/main/crates/rustitude-gluex/src/harmonics.rs)), we can just return `None` (the `Some` is required because this function returns an `Option`).
+Finally, the `parameters` function just returns a list of the parameter names in the order they are expected to be input into `calculate`. In the event that an amplitude doesn't have any free parameters (like [my implementation of the `Ylm` and `Zlm` amplitudes](https://github.com/denehoffman/rustitude/blob/main/crates/rustitude-gluex/src/harmonics.rs)), we can omit this function entirely, as the default implementation returns `vec![]`.
 
 And that's it! However, it is important to be aware of the steps which need to be taken to allow this amplitude to be used through the Python interface.
 
 ## Python Bindings
 
 To make Python bindings, `pyo3` needs to be included as a dependency:
 
 ```rust
 use pyo3::prelude::*;
 
 // OmegaDalitz code here
 
 #[pyfunction(name = "OmegaDalitz")]
-fn omega_dalitz(name: &str) -> Amplitude {
-    Amplitude::new(name, Box::<OmegaDalitz>::default())
+fn omega_dalitz(name: &str) -> PyAmpOp {
+    Amplitude::new(name, Box::<OmegaDalitz>::default()).into()
 }
 
 pub fn pyo3_module(m: &Bound<'_, PyModule>) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(omega_dalitz, m)?)?;
     Ok(())
 }
 ```
 
-Rather than bind the `struct` directly, we prefer to bind a function which returns an `Amplitude`, a wrapper struct that implements `#[pyclass]` and can be used in the Python interface. The `pyo3_module` function will then need to be added to the `rustitude` crate's [`lib.rs`](https://github.com/denehoffman/rustitude/blob/main/src/lib.rs) file. This step is a bit problematic, since it means new amplitudes cannot be added without modifying `rustitude` itself. For this reason, developers may want to work with their own fork of the repository rather than using the one installed by `cargo` if they wish to use Python. This is a limitation of `pyo3`, which doesn't recognize class bindings across crates.
+Rather than bind the `struct` directly, we prefer to bind a function which returns a `PyAmpOp`, a wrapper struct that implements `#[pyclass]` and can be used in the Python interface. The `pyo3_module` function will then need to be added to the `rustitude` crate's [`lib.rs`](https://github.com/denehoffman/rustitude/blob/main/src/lib.rs) file. This step is a bit problematic, since it means new amplitudes cannot be added without modifying `rustitude` itself. For this reason, developers may want to work with their own fork of the repository rather than using the one installed by `cargo` if they wish to use Python. This is a limitation of `pyo3`, which doesn't recognize class bindings across crates.
 
 # TODOs
 
 In no particular order, here is a list of what (probably) needs to be done before I will stop making any breaking changes:
 
 - Pure Rust parsing of ROOT files without the `uproot` backend (I have some moderate success with `oxyroot`, but there are still a few issues reading larger files)
 - Add plotting methods
 - A way to check if the number of parameters matches the input at compile time would be nice, not sure if it's possible though
-- Give managers a way to apply amplitudes to new datasets, like using the result from a fit to weight some generated Monte-Carlo for plotting the result. This is possible to do through Python, but a convenience method is probably needed
 - Amplitude serialization (I want to be able to send and share an amplitude configuration just like an `AmpTools` config file, but with the amplitude itself included)
 - Lots of documentation
 - Lots of tests
```

#### html2text {}

```diff
@@ -17,116 +17,108 @@
 of their amplitude, and one of these just gives the names and order of the
 amplitude's input parameters. - A major goal of `rustitude` was to increase
 processing speed by sacrificing memory. This is done by precalculating parts of
 amplitudes which don't change when the free parameter inputs change. The
 simplest example of this is the `Ylm` amplitude (spherical harmonic), which can
 be entirely precalculated given the value of `l` and `m`. To calculate this
 amplitude at evaluation time, `rustitude` just needs to look up a value in an
-array! # Theory Amplitudes are registered into a named `sum` and `group`.
-Similar to [`AmpTools`](https://github.com/mashephe/AmpTools), the typical
-calculation for any event $e$ and list of parameters $\overrightarrow{p}$ will
-then be: ```math I(\overrightarrow{p}, e) = \sum_{\text{groups} \in \text
-{sums}}\left|\sum_{\text{amplitudes} \in \text{groups}} \prod_{\text{amp} \in
-\text{amplitudes}} \text{amp}(\overrightarrow{p}, e)\right|^2 ``` #
-Installation Cargo provides the usual command for including this crate in a
-project: ```shell cargo add rustitude-core ``` However, this project is best-
-used with some pre-made amplitudes (see [`rustitude-gluex`](https://github.com/
-denehoffman/rustitude/tree/main/crates/rustitude-gluex/), and these come
-bundled with the [`rustitude`](https://github.com/denehoffman/rustitude/) meta-
-crate, which also re-exports this crate's prelude. This can be installed via
-the same command: ```shell cargo add rustitude ``` # Implementing an Amplitude
-While typical usage might be to use pre-made amplitudes in various
+array! # Installation Cargo provides the usual command for including this crate
+in a project: ```shell cargo add rustitude-core ``` However, this project is
+best-used with some pre-made amplitudes (see [`rustitude-gluex`](https://
+github.com/denehoffman/rustitude/tree/main/crates/rustitude-gluex/), and these
+come bundled with the [`rustitude`](https://github.com/denehoffman/rustitude/
+) meta-crate, which also re-exports this crate's prelude. This can be installed
+via the same command: ```shell cargo add rustitude ``` # Implementing an
+Amplitude While typical usage might be to use pre-made amplitudes in various
 combinations, it is important to know how to design an amplitude which will
 work seamlessly with this crate. Let's write down the `rustitude` version of
 the [OmegaDalitz](https://github.com/JeffersonLab/halld_sim/blob/
 6544f01ac1514b0b9a53ad241cf2e8a63e1d3dfa/src/libraries/AMPTOOLS_AMPS/
 OmegaDalitz.cc) amplitude: ```rust use rayon::prelude::*; use rustitude_core::
 prelude::*; #[derive(Default)] pub struct OmegaDalitz { dalitz_z: Vec,
 dalitz_sin3theta: Vec, lambda: Vec, } impl Node for OmegaDalitz { fn
-precalculate(&mut self, dataset: &Dataset) { (self.dalitz_z,
-(self.dalitz_sin3theta, self.lambda)) = dataset .events .read() .par_iter()
-.map(|event| { let pi0 = event.daughter_p4s[0]; let pip = event.daughter_p4s
-[1]; let pim = event.daughter_p4s[2]; let omega = pi0 + pip + pim; let dalitz_s
-= (pip + pim).m2(); let dalitz_t = (pip + pi0).m2(); let dalitz_u = (pim +
-pi0).m2(); let m3pi = (2.0 * pip.m()) + pi0.m(); let dalitz_d = 2.0 * omega.m()
-* (omega.m() - m3pi); let dalitz_sc = (1.0 / 3.0) * (omega.m2() + pip.m2() +
-pim.m2() + pi0.m2()); let dalitz_x = f64::sqrt(3.0) * (dalitz_t - dalitz_u) /
-dalitz_d; let dalitz_y = 3.0 * (dalitz_sc - dalitz_s) / dalitz_d; let dalitz_z
-= dalitz_x * dalitz_x + dalitz_y * dalitz_y; let dalitz_sin3theta = f64::sin
-(3.0 * f64::asin(dalitz_y / f64::sqrt(dalitz_z))); let pip_omega =
+precalculate(&mut self, dataset: &Dataset) -> Result<(), NodeError> {
+(self.dalitz_z, (self.dalitz_sin3theta, self.lambda)) = dataset .events .read()
+.par_iter() .map(|event| { let pi0 = event.daughter_p4s[0]; let pip =
+event.daughter_p4s[1]; let pim = event.daughter_p4s[2]; let omega = pi0 + pip +
+pim; let dalitz_s = (pip + pim).m2(); let dalitz_t = (pip + pi0).m2(); let
+dalitz_u = (pim + pi0).m2(); let m3pi = (2.0 * pip.m()) + pi0.m(); let dalitz_d
+= 2.0 * omega.m() * (omega.m() - m3pi); let dalitz_sc = (1.0 / 3.0) * (omega.m2
+() + pip.m2() + pim.m2() + pi0.m2()); let dalitz_x = f64::sqrt(3.0) * (dalitz_t
+- dalitz_u) / dalitz_d; let dalitz_y = 3.0 * (dalitz_sc - dalitz_s) / dalitz_d;
+let dalitz_z = dalitz_x * dalitz_x + dalitz_y * dalitz_y; let dalitz_sin3theta
+= f64::sin(3.0 * f64::asin(dalitz_y / f64::sqrt(dalitz_z))); let pip_omega =
 pip.boost_along(ω); let pim_omega = pim.boost_along(ω); let pi_cross =
 pip_omega.momentum().cross(&pim_omega.momentum()); let lambda = (4.0 / 3.0) *
 f64::abs(pi_cross.dot(π_cross)) / ((1.0 / 9.0) * (omega.m2() - (2.0 * pip.m() +
 pi0.m()).powi(2)).powi(2)); (dalitz_z, (dalitz_sin3theta, lambda)) }) .unzip();
-} fn calculate(&self, parameters: &[f64], event: &Event) -> Complex64 { let
-dalitz_z = self.dalitz_z[event.index]; let dalitz_sin3theta =
+Ok(()) } fn calculate(&self, parameters: &[f64], event: &Event) -> Result
+ NodeError> { let dalitz_z = self.dalitz_z[event.index]; let dalitz_sin3theta =
 self.dalitz_sin3theta[event.index]; let lambda = self.lambda[event.index]; let
 alpha = parameters[0]; let beta = parameters[1]; let gamma = parameters[2]; let
-delta = parameters[3]; f64::sqrt(f64::abs( lambda * (1.0 + 2.0 * alpha *
+delta = parameters[3]; Ok(f64::sqrt(f64::abs( lambda * (1.0 + 2.0 * alpha *
 dalitz_z + 2.0 * beta * dalitz_z.powf(3.0 / 2.0) * dalitz_sin3theta + 2.0 *
 gamma * dalitz_z.powi(2) + 2.0 * delta * dalitz_z.powf(5.0 / 2.0) *
-dalitz_sin3theta), )) .into() } fn parameters(&self) -> Option
-String>> { Some(vec![ "alpha".to_string(), "beta".to_string(),
-"gamma".to_string(), "delta".to_string(), ]) } } ``` Let's walk through this
-code. First, we need to define a `struct` which has all of the general
-information about the amplitude, and in this case some kind of `Vec` for
-storing precalculated data. We consider this precalculated data to correspond
-to a single dataset, and each dataset gets its own copy of the amplitude
-`struct`. Because this particular amplitude doesn't have any input parameters,
-we can `#[derive(Default)]` on it to make a default constructor, which allows
-the amplitude to be initialized with something like `let amp = OmegaDalitz::
-default();`. If we wanted a parameterized constructor, we have to define our
-own, and while Rust has no default name for constructors, `pub fn new(...) -
-> Self` is preferred. Next, we implement the `Node` trait for the `struct`.
-Traits in Rust are kind of like abstract classes or interfaces in object-
-oriented languages, they provide some set of methods which a `struct` must
-implement. The first of these methods is `fn precalculate(&mut self, dataset:
-&Dataset)`. As the signature suggests, it takes a `Dataset` and mutates the
-`struct` in some way. The intended usage of this function is to precalculate
-some terms in the amplitude's mathematical expression, things which don't
-change when you update the free parameter inputs to the amplitude. In this
-case, the four input parameters, $`\alpha`$, $`\beta`$, $`\gamma`$, and
-$`\delta`$, are independent from `dalitz_z`, `dalitz_sin3theta`, and `lambda`,
-so we can safely calculate those ahead of time and just pull from their
-respective `Vec`s when needed later. I won't go too far into Rust's syntax
-here, but typical precalculation functions will start by iterating over the
-dataset's events in parallel (the line `use rayon::prelude::*;` is needed to
-use `par_iter` here) and collecting or unzipping that iterator into a `Vec` or
-group of `Vec`s. The calculate step has the signature `fn calculate(&self,
-parameters: &[f64], event: &Event) -> Complex64`. This means we need to take a
-list of parameters and a single event and turn them into a complex value. The
-`Event` struct contains an `index` field which can be used to access the
-precalculated storage arrays made in the previous step. Finally, the
-`parameters` function just returns a list of the parameter names in the order
-they are expected to be input into `calculate`. In the event that an amplitude
-doesn't have any free parameters (like [my implementation of the `Ylm` and
-`Zlm` amplitudes](https://github.com/denehoffman/rustitude/blob/main/crates/
-rustitude-gluex/src/harmonics.rs)), we can just return `None` (the `Some` is
-required because this function returns an `Option`). And that's it! However, it
-is important to be aware of the steps which need to be taken to allow this
-amplitude to be used through the Python interface. ## Python Bindings To make
-Python bindings, `pyo3` needs to be included as a dependency: ```rust use
-pyo3::prelude::*; // OmegaDalitz code here #[pyfunction(name = "OmegaDalitz")]
-fn omega_dalitz(name: &str) -> Amplitude { Amplitude::new(name, Box::::default
-()) } pub fn pyo3_module(m: &Bound<'_, PyModule>) -> PyResult<()>
-{ m.add_function(wrap_pyfunction!(omega_dalitz, m)?)?; Ok(()) } ``` Rather than
-bind the `struct` directly, we prefer to bind a function which returns an
-`Amplitude`, a wrapper struct that implements `#[pyclass]` and can be used in
-the Python interface. The `pyo3_module` function will then need to be added to
-the `rustitude` crate's [`lib.rs`](https://github.com/denehoffman/rustitude/
-blob/main/src/lib.rs) file. This step is a bit problematic, since it means new
-amplitudes cannot be added without modifying `rustitude` itself. For this
-reason, developers may want to work with their own fork of the repository
-rather than using the one installed by `cargo` if they wish to use Python. This
-is a limitation of `pyo3`, which doesn't recognize class bindings across
-crates. # TODOs In no particular order, here is a list of what (probably) needs
-to be done before I will stop making any breaking changes: - Pure Rust parsing
-of ROOT files without the `uproot` backend (I have some moderate success with
-`oxyroot`, but there are still a few issues reading larger files) - Add
-plotting methods - A way to check if the number of parameters matches the input
-at compile time would be nice, not sure if it's possible though - Give managers
-a way to apply amplitudes to new datasets, like using the result from a fit to
-weight some generated Monte-Carlo for plotting the result. This is possible to
-do through Python, but a convenience method is probably needed - Amplitude
-serialization (I want to be able to send and share an amplitude configuration
-just like an `AmpTools` config file, but with the amplitude itself included) -
-Lots of documentation - Lots of tests
+dalitz_sin3theta), )) .into()) } fn parameters(&self) -> Vec { vec!
+[ "alpha".to_string(), "beta".to_string(), "gamma".to_string(),
+"delta".to_string(), ] } } ``` Let's walk through this code. First, we need to
+define a `struct` which has all of the general information about the amplitude,
+and in this case some kind of `Vec` for storing precalculated data. We consider
+this precalculated data to correspond to a single dataset, and each dataset
+gets its own copy of the amplitude `struct`. Because this particular amplitude
+doesn't have any input parameters, we can `#[derive(Default)]` on it to make a
+default constructor, which allows the amplitude to be initialized with
+something like `let amp = OmegaDalitz::default();`. If we wanted a
+parameterized constructor, we have to define our own, and while Rust has no
+default name for constructors, `pub fn new(...) -> rustitude_core::AmpOp` is
+preferred. Next, we implement the `Node` trait for the `struct`. Traits in Rust
+are kind of like abstract classes or interfaces in object-oriented languages,
+they provide some set of methods which a `struct` must implement. The first of
+these methods is `fn precalculate(&mut self, dataset: &Dataset) -> Result<(),
+NodeError>`. As the signature suggests, it takes a `Dataset` and mutates the
+`struct` in some way. It should raise a `NodeError` if anything goes wrong in
+the evaluation. The intended usage of this function is to precalculate some
+terms in the amplitude's mathematical expression, things which don't change
+when you update the free parameter inputs to the amplitude. In this case, the
+four input parameters, $`\alpha`$, $`\beta`$, $`\gamma`$, and $`\delta`$, are
+independent from `dalitz_z`, `dalitz_sin3theta`, and `lambda`, so we can safely
+calculate those ahead of time and just pull from their respective `Vec`s when
+needed later. I won't go too far into Rust's syntax here, but typical
+precalculation functions will start by iterating over the dataset's events in
+parallel (the line `use rayon::prelude::*;` is needed to use `par_iter` here)
+and collecting or unzipping that iterator into a `Vec` or group of `Vec`s. The
+calculate step has the signature `fn calculate(&self, parameters: &[f64],
+event: &Event) -> Result
+ NodeError>`. This means we need to take a list of parameters and a single
+event and turn them into a complex value. The `Event` struct contains an
+`index` field which can be used to access the precalculated storage arrays made
+in the previous step. Finally, the `parameters` function just returns a list of
+the parameter names in the order they are expected to be input into
+`calculate`. In the event that an amplitude doesn't have any free parameters
+(like [my implementation of the `Ylm` and `Zlm` amplitudes](https://github.com/
+denehoffman/rustitude/blob/main/crates/rustitude-gluex/src/harmonics.rs)), we
+can omit this function entirely, as the default implementation returns `vec!
+[]`. And that's it! However, it is important to be aware of the steps which
+need to be taken to allow this amplitude to be used through the Python
+interface. ## Python Bindings To make Python bindings, `pyo3` needs to be
+included as a dependency: ```rust use pyo3::prelude::*; // OmegaDalitz code
+here #[pyfunction(name = "OmegaDalitz")] fn omega_dalitz(name: &str) -> PyAmpOp
+{ Amplitude::new(name, Box::::default()).into() } pub fn pyo3_module(m:
+&Bound<'_, PyModule>) -> PyResult<()> { m.add_function(wrap_pyfunction!
+(omega_dalitz, m)?)?; Ok(()) } ``` Rather than bind the `struct` directly, we
+prefer to bind a function which returns a `PyAmpOp`, a wrapper struct that
+implements `#[pyclass]` and can be used in the Python interface. The
+`pyo3_module` function will then need to be added to the `rustitude` crate's
+[`lib.rs`](https://github.com/denehoffman/rustitude/blob/main/src/lib.rs) file.
+This step is a bit problematic, since it means new amplitudes cannot be added
+without modifying `rustitude` itself. For this reason, developers may want to
+work with their own fork of the repository rather than using the one installed
+by `cargo` if they wish to use Python. This is a limitation of `pyo3`, which
+doesn't recognize class bindings across crates. # TODOs In no particular order,
+here is a list of what (probably) needs to be done before I will stop making
+any breaking changes: - Pure Rust parsing of ROOT files without the `uproot`
+backend (I have some moderate success with `oxyroot`, but there are still a few
+issues reading larger files) - Add plotting methods - A way to check if the
+number of parameters matches the input at compile time would be nice, not sure
+if it's possible though - Amplitude serialization (I want to be able to send
+and share an amplitude configuration just like an `AmpTools` config file, but
+with the amplitude itself included) - Lots of documentation - Lots of tests
```

### Comparing `rustitude-0.4.0/crates/rustitude-core/bacon.toml` & `rustitude-0.4.2/py-rustitude/bacon.toml`

 * *Files 3% similar despite different names*

```diff
@@ -38,18 +38,20 @@
 # - the tests of a package: bacon test -- -- -p config
 [jobs.test]
 command = [
     "cargo",
     "test",
     "--color",
     "always",
+    "-F",
+    "intel-mkl-static",
     "--",
     "--nocapture",
     "--color",
-    "always",      # see https://github.com/Canop/bacon/issues/124
+    "always",           # see https://github.com/Canop/bacon/issues/124
 ]
 need_stdout = true
 
 [jobs.doc]
 command = ["cargo", "doc", "--color", "always", "--no-deps"]
 need_stdout = false
 
@@ -70,14 +72,16 @@
 [jobs.run]
 command = [
     "cargo",
     "run",
     "--release",
     "--color",
     "always",
+    "-F",
+    "intel-mkl-static",
     "--timings",
     # put launch parameters for your program behind a `--` separator
 ]
 need_stdout = true
 allow_warnings = true
 background = true
```

### Comparing `rustitude-0.4.0/crates/rustitude-core/media/logo.png` & `rustitude-0.4.2/crates/rustitude-core/media/logo.png`

 * *Files identical despite different names*

### Comparing `rustitude-0.4.0/crates/rustitude-core/src/amplitude.rs` & `rustitude-0.4.2/crates/rustitude-core/src/amplitude.rs`

 * *Files identical despite different names*

### Comparing `rustitude-0.4.0/crates/rustitude-core/src/dataset.rs` & `rustitude-0.4.2/crates/rustitude-core/src/dataset.rs`

 * *Files identical despite different names*

### Comparing `rustitude-0.4.0/crates/rustitude-core/src/docs-header.html` & `rustitude-0.4.2/crates/rustitude-core/src/docs-header.html`

 * *Files identical despite different names*

### Comparing `rustitude-0.4.0/crates/rustitude-core/src/four_momentum.rs` & `rustitude-0.4.2/crates/rustitude-core/src/four_momentum.rs`

 * *Files identical despite different names*

### Comparing `rustitude-0.4.0/crates/rustitude-core/src/lib.rs` & `rustitude-0.4.2/crates/rustitude-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rustitude-0.4.0/crates/rustitude-core/src/manager.rs` & `rustitude-0.4.2/crates/rustitude-core/src/manager.rs`

 * *Files identical despite different names*

### Comparing `rustitude-0.4.0/crates/rustitude-gluex/CHANGELOG.md` & `rustitude-0.4.2/crates/rustitude-gluex/CHANGELOG.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,76 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## v0.2.1 (2024-05-15)
+
+### Refactor
+
+ - <csr-id-9089c84e481124ff764b24f42507ab14913fef07/> major move required to have rustitude function properly as a Rust crate. I set this up very wrong the first time
+
+### Commit Statistics
+
+<csr-read-only-do-not-edit/>
+
+ - 1 commit contributed to the release.
+ - 1 commit was understood as [conventional](https://www.conventionalcommits.org).
+ - 0 issues like '(#ID)' were seen in commit messages
+
+### Commit Details
+
+<csr-read-only-do-not-edit/>
+
+<details><summary>view details</summary>
+
+ * **Uncategorized**
+    - Major move required to have rustitude function properly as a Rust crate. I set this up very wrong the first time ([`9089c84`](https://github.com/denehoffman/rustitude/commit/9089c84e481124ff764b24f42507ab14913fef07))
+</details>
+
 ## v0.2.0 (2024-05-15)
 
+<csr-id-9617a27322460b378fb022ef28561f31197fc86f/>
+
 ### Documentation
 
  - <csr-id-93dc0d6cfeb57f655c81f30c1e55b1c6b0460ccc/> update links for rustitude-gluex readme
  - <csr-id-95f85ed6b16400c882e7535c7fa113ead9876353/> update links in readmes
 
 ### Other
 
  - <csr-id-9617a27322460b378fb022ef28561f31197fc86f/> merge rustitude-core to crates subdirectory
 
+### Bug Fixes
+
+ - <csr-id-2495107c77f483b84a926090cd868ccec8296052/> need to set some dependency versions...
+ - <csr-id-ee48e4039e40bbf2c5b23d230bbcd0213c41e888/> need to set some dependency versions...properly
+
 ### Commit Statistics
 
 <csr-read-only-do-not-edit/>
 
- - 3 commits contributed to the release.
- - 3 commits were understood as [conventional](https://www.conventionalcommits.org).
+ - 8 commits contributed to the release.
+ - 5 commits were understood as [conventional](https://www.conventionalcommits.org).
  - 0 issues like '(#ID)' were seen in commit messages
 
 ### Commit Details
 
 <csr-read-only-do-not-edit/>
 
 <details><summary>view details</summary>
 
  * **Uncategorized**
+    - Release rustitude-gluex v0.2.0, rustitude v0.4.0 ([`bc38f3a`](https://github.com/denehoffman/rustitude/commit/bc38f3af06807d8e6e1c3ca3a38581461ef934b8))
+    - Need to set some dependency versions...properly ([`ee48e40`](https://github.com/denehoffman/rustitude/commit/ee48e4039e40bbf2c5b23d230bbcd0213c41e888))
+    - Release rustitude-gluex v0.2.0, rustitude v0.4.0 ([`1369408`](https://github.com/denehoffman/rustitude/commit/1369408a7352be0e5b5fb675b0127e8e69a10c59))
+    - Need to set some dependency versions... ([`2495107`](https://github.com/denehoffman/rustitude/commit/2495107c77f483b84a926090cd868ccec8296052))
+    - Release rustitude-core v1.0.0, rustitude-gluex v0.2.0, rustitude v0.4.0, safety bump 2 crates ([`23a8807`](https://github.com/denehoffman/rustitude/commit/23a880783702368ee873ce4839310f4b392c6862))
     - Update links for rustitude-gluex readme ([`93dc0d6`](https://github.com/denehoffman/rustitude/commit/93dc0d6cfeb57f655c81f30c1e55b1c6b0460ccc))
     - Update links in readmes ([`95f85ed`](https://github.com/denehoffman/rustitude/commit/95f85ed6b16400c882e7535c7fa113ead9876353))
     - Merge rustitude-core to crates subdirectory ([`9617a27`](https://github.com/denehoffman/rustitude/commit/9617a27322460b378fb022ef28561f31197fc86f))
 </details>
 
 ## v0.1.5 (2024-05-06)
```

### Comparing `rustitude-0.4.0/crates/rustitude-gluex/LICENSE` & `rustitude-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rustitude-0.4.0/crates/rustitude-gluex/README.md` & `rustitude-0.4.2/crates/rustitude-gluex/README.md`

 * *Files identical despite different names*

### Comparing `rustitude-0.4.0/crates/rustitude-gluex/media/logo.png` & `rustitude-0.4.2/crates/rustitude-gluex/media/logo.png`

 * *Files identical despite different names*

### Comparing `rustitude-0.4.0/crates/rustitude-gluex/src/dalitz.rs` & `rustitude-0.4.2/crates/rustitude-gluex/src/dalitz.rs`

 * *Files identical despite different names*

### Comparing `rustitude-0.4.0/crates/rustitude-gluex/src/harmonics.rs` & `rustitude-0.4.2/crates/rustitude-gluex/src/harmonics.rs`

 * *Files identical despite different names*

### Comparing `rustitude-0.4.0/crates/rustitude-gluex/src/resonances.rs` & `rustitude-0.4.2/crates/rustitude-gluex/src/resonances.rs`

 * *Files identical despite different names*

### Comparing `rustitude-0.4.0/crates/rustitude-gluex/src/sdmes.rs` & `rustitude-0.4.2/crates/rustitude-gluex/src/sdmes.rs`

 * *Files identical despite different names*

### Comparing `rustitude-0.4.0/crates/rustitude-gluex/src/utils.rs` & `rustitude-0.4.2/crates/rustitude-gluex/src/utils.rs`

 * *Files identical despite different names*

### Comparing `rustitude-0.4.0/CHANGELOG.md` & `rustitude-0.4.2/py-rustitude/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,66 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
-## 0.4.0 (2024-05-15)
+## 0.4.1 (2024-05-15)
 
 ### Bug Fixes
 
- - <csr-id-b71f07c33445f310969e445e7b158bdeef726a8d/> make add_submodule public
+ - <csr-id-740a0186ae22bdab87f514a5e035f3917a531c86/> add package info into workspace
 
 ### Other
 
- - <csr-id-f39aab03b7160ba3817614170d67bfcfdb22642b/> reorganize crate structure
+ - <csr-id-9617a27322460b378fb022ef28561f31197fc86f/> merge rustitude-core to crates subdirectory
+ - <csr-id-64ec5097cc99eb9bb6d73376e6d3b2788f637d9d/> more Cargo.lock and readme updates
+ - <csr-id-78b96b94097670af64886abb84ed263048e91e62/> update Cargo.tomls
+ - <csr-id-8f2f28c972c20c0b8cef2869ab08fc4abaec5cf7/> move rustitude to crates subdirectory
+
+### Refactor
+
+ - <csr-id-097311224630f5a4d98381a11d2917ca6378ad46/> move rustitude into the crates directory and add to workspace
 
 ### Commit Statistics
 
 <csr-read-only-do-not-edit/>
 
- - 2 commits contributed to the release over the course of 1 calendar day.
- - 8 days passed between releases.
- - 2 commits were understood as [conventional](https://www.conventionalcommits.org).
+ - 6 commits contributed to the release over the course of 1 calendar day.
+ - 6 commits were understood as [conventional](https://www.conventionalcommits.org).
  - 0 issues like '(#ID)' were seen in commit messages
 
 ### Commit Details
 
 <csr-read-only-do-not-edit/>
 
 <details><summary>view details</summary>
 
  * **Uncategorized**
-    - Reorganize crate structure ([`f39aab0`](https://github.com/denehoffman/rustitude/commit/f39aab03b7160ba3817614170d67bfcfdb22642b))
-    - Make add_submodule public ([`b71f07c`](https://github.com/denehoffman/rustitude/commit/b71f07c33445f310969e445e7b158bdeef726a8d))
+    - Add package info into workspace ([`740a018`](https://github.com/denehoffman/rustitude/commit/740a0186ae22bdab87f514a5e035f3917a531c86))
+    - Move rustitude into the crates directory and add to workspace ([`0973112`](https://github.com/denehoffman/rustitude/commit/097311224630f5a4d98381a11d2917ca6378ad46))
+    - Merge rustitude-core to crates subdirectory ([`9617a27`](https://github.com/denehoffman/rustitude/commit/9617a27322460b378fb022ef28561f31197fc86f))
+    - More Cargo.lock and readme updates ([`64ec509`](https://github.com/denehoffman/rustitude/commit/64ec5097cc99eb9bb6d73376e6d3b2788f637d9d))
+    - Update Cargo.tomls ([`78b96b9`](https://github.com/denehoffman/rustitude/commit/78b96b94097670af64886abb84ed263048e91e62))
+    - Move rustitude to crates subdirectory ([`8f2f28c`](https://github.com/denehoffman/rustitude/commit/8f2f28c972c20c0b8cef2869ab08fc4abaec5cf7))
 </details>
 
+## 0.4.0 (2024-05-15)
+
+<csr-id-f39aab03b7160ba3817614170d67bfcfdb22642b/>
+
+### Bug Fixes
+
+ - <csr-id-b71f07c33445f310969e445e7b158bdeef726a8d/> make add_submodule public
+
+### Other
+
+ - <csr-id-f39aab03b7160ba3817614170d67bfcfdb22642b/> reorganize crate structure
+
 ## 0.3.4 (2024-05-06)
 
 <csr-id-475682fc30d7dc6a817030dd754cc4fb7dd295cc/>
 <csr-id-f64c86d2e21c17fe6bc5638240293a774185159a/>
 <csr-id-4a88e2b13fb01de2812f91ef4d55eea6b37fe7b2/>
 <csr-id-1747d5dc4a63bf47f2f5cbc479f879459e900c4c/>
 <csr-id-42f29669736bb72ed4d85f4669df1a48288a2db8/>
@@ -68,33 +90,14 @@
  - <csr-id-f64c86d2e21c17fe6bc5638240293a774185159a/> update Cargo.lock
  - <csr-id-4a88e2b13fb01de2812f91ef4d55eea6b37fe7b2/> re-enable tag check
  - <csr-id-1747d5dc4a63bf47f2f5cbc479f879459e900c4c/> temporarily disable tag check so we can push to pypi through an action
  - <csr-id-42f29669736bb72ed4d85f4669df1a48288a2db8/> re-enable on-push and on-PR workflow conditions
    A release only happens with a new tag
  - <csr-id-d94179156007fd86b69b8efbfd2f1799d0bb71b8/> update pyproject.toml version
 
-### Commit Statistics
-
-<csr-read-only-do-not-edit/>
-
- - 1 commit contributed to the release over the course of 1 calendar day.
- - 3 days passed between releases.
- - 1 commit was understood as [conventional](https://www.conventionalcommits.org).
- - 0 issues like '(#ID)' were seen in commit messages
-
-### Commit Details
-
-<csr-read-only-do-not-edit/>
-
-<details><summary>view details</summary>
-
- * **Uncategorized**
-    - Add type checking and re-export rustitude-core and rustitude-gluex as their own submodules ([`6fc5c77`](https://github.com/denehoffman/rustitude/commit/6fc5c77477602403f3b892b240064de9f717d406))
-</details>
-
 ## 0.3.3 (2024-05-03)
 
 <csr-id-e0c32f773b601e2703a0803849a1a2db130e2ffc/>
 <csr-id-158ddc248dc8463e08eb14b7f633952fc28abcd6/>
 <csr-id-f8370544ef666930bfd5f3a1b555e34e53525b6f/>
 <csr-id-db8b1a32563700203f896c0d357ed96d1144d202/>
 
@@ -156,33 +159,14 @@
 
 ### Style
 
  - <csr-id-aaa07cd742e03461449269e8261e7f326600b2a0/> add local notes
  - <csr-id-e2cb6e54946744299506a39a5d3559ee099378fb/> Create LICENSE
  - <csr-id-310f89c2a2da584beabad3e208484be186e8f7fd/> update .gitignore
 
-### Commit Statistics
-
-<csr-read-only-do-not-edit/>
-
- - 2 commits contributed to the release over the course of 1 calendar day.
- - 2 commits were understood as [conventional](https://www.conventionalcommits.org).
- - 0 issues like '(#ID)' were seen in commit messages
-
-### Commit Details
-
-<csr-read-only-do-not-edit/>
-
-<details><summary>view details</summary>
-
- * **Uncategorized**
-    - Opt for implementing all pyo3 bindings in their own submodules - this package will be very lightweight! ([`3126b7a`](https://github.com/denehoffman/rustitude/commit/3126b7a26b835ee24d112883ca540c172d97dd82))
-    - Initial commit to rustitude meta-crate ([`157c864`](https://github.com/denehoffman/rustitude/commit/157c8648dbcc1a6111d8c262a31139990ab09f3b))
-</details>
-
 ## 0.3.1 (2024-04-10)
 
 <csr-id-35fd81ade394522801d288e4a2d084b581d5e5a5/>
 <csr-id-1d91ee9b2928b9761b0568104ea5e8b7841bf24c/>
 <csr-id-73067f2c6f657ba3b35a197a0ab2ea8029e359e6/>
 <csr-id-55443f6454e0072abc3cfc41d38e5fa297cdb9cd/>
 <csr-id-aa9d91971816ff3d99a47e928be5bfb2360c0694/>
```

### Comparing `rustitude-0.4.0/README.md` & `rustitude-0.4.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,14 @@
   <a href="https://docs.rs/rustitude" alt="Rustitude documentation on docs.rs">
     <img src="https://img.shields.io/docsrs/rustitude" /></a>
 </p>
 
 ### Table of Contents:
 
 - [Introduction](#Introduction)
-- [Theory](#Theory)
 - [Installation](#Installation)
 - [Usage](#Usage)
 - [TODOs](#TODOs)
 
 # Introduction
 
 This project began with a desire to make a fast but easy to use interface for fitting amplitudes to particle physics data. That being said, there are performant methods such as [`AmpTools`](https://github.com/mashephe/AmpTools), which is written in C++, but in my personal experience, it can be a bit tricky to use and extend, and it generally requires a lot of boilerplate code to generate new amplitudes or plotting scripts. On the other hand, there are also libraries like [`PyPWA`](https://github.com/JeffersonLab/PyPWA/) (written in Python) which seem like they could be easy to use, but often fail in this aspect due to Python's limiting syntax, speed issues, and a general lack of documentation and ongoing development. There have been attempts to bridge the gap between AmpTools and Python, most recently (and successfully) [`PyAmpTools`](https://github.com/lan13005/PyAmpTools). The difficulty with this method is that it relies on PyROOT, which also means you need ROOT installed (and built with your version of Python). For now, I'll spare you the anti-ROOT rant and just say that ROOT should be an opt-in, not a requirement. So where does that leave `rustitude`?
@@ -38,22 +37,14 @@
 Now I've covered why I don't like some of the existing solutions, and why I chose to use Rust, but what does this project have that makes it stand out? Here are some reasons to entice you:
 
 - `rustitude` will automatically parallelize amplitudes over the events in a dataset. There's no reason for a developer to ever write parallelized code themselves.
 - Implementing [`Node`](https://docs.rs/rustitude-core/latest/rustitude_core/amplitude/trait.Node.html) on a struct is all that is needed to use it as an amplitude. This means developers need only write two to three total methods to describe the entire functionality of their amplitude, and one of these just gives the names and order of the amplitude's input parameters.
 - A major goal of `rustitude` was to increase processing speed by sacrificing memory. This is done by precalculating parts of amplitudes which don't change when the free parameter inputs change. `AmpTools` supports a version of this, but only on the level of each general amplitude rather than on an individual basis. The simplest example of this is the `Ylm` amplitude (spherical harmonic), which can be entirely precalculated given the value of `l` and `m`. In `AmpTools`, different instances of `Ylm` with different `l`s and `m`s share precalculated data, whereas in `rustitude`, they don't. The `AmpTools` implementation of `Ylm` needs to calculate a spherical harmonic for every event on every function call, while `rustitude` just needs to look up a value in an array!
 - The majority of the library (the public interface) has Python bindings, so if there is no need for custom amplitudes, a developer never actually has to write any Rust code, and the resulting calculations will be as performant as if they were written in Rust.
 
-# Theory
-
-Amplitudes are registered into a named `sum` and `group`. Similar to `AmpTools`, the typical calculation for any event $e$ and list of parameters $\overrightarrow{p}$ will then be:
-
-```math
-I(\overrightarrow{p}, e) = \sum_{\text{groups} \in \text{sums}}\left|\sum_{\text{amplitudes} \in \text{groups}} \prod_{\text{amp} \in \text{amplitudes}} \text{amp}(\overrightarrow{p}, e)\right|^2
-```
-
 # Installation
 
 Adding `rustitude` to an existing Rust project is as simple as
 
 ```shell
 cargo add rustitude
 ```
```

#### html2text {}

```diff
@@ -1,105 +1,99 @@
  [https://raw.githubusercontent.com/denehoffman/rustitude/main/media/logo.png]
                  ************ DDeemmyyssttiiffyyiinngg AAmmpplliittuuddee AAnnaallyyssiiss ************
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_a_s_t_-_c_o_m_m_i_t_/_d_e_n_e_h_o_f_f_m_a_n_/_r_u_s_t_i_t_u_d_e_/_m_a_i_n_]_[_h_t_t_p_s_:_/_/
  _i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_/_s_t_a_t_u_s_/_d_e_n_e_h_o_f_f_m_a_n_/_r_u_s_t_i_t_u_d_e_/_r_u_s_t_._y_m_l_]
     _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_i_c_e_n_s_e_/_d_e_n_e_h_o_f_f_m_a_n_/_r_u_s_t_i_t_u_d_e_]_[_h_t_t_p_s_:_/_/
   _i_m_g_._s_h_i_e_l_d_s_._i_o_/_c_r_a_t_e_s_/_v_/_r_u_s_t_i_t_u_d_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_d_o_c_s_r_s_/_r_u_s_t_i_t_u_d_e_]
-### Table of Contents: - [Introduction](#Introduction) - [Theory](#Theory) -
-[Installation](#Installation) - [Usage](#Usage) - [TODOs](#TODOs) #
-Introduction This project began with a desire to make a fast but easy to use
-interface for fitting amplitudes to particle physics data. That being said,
-there are performant methods such as [`AmpTools`](https://github.com/mashephe/
-AmpTools), which is written in C++, but in my personal experience, it can be a
-bit tricky to use and extend, and it generally requires a lot of boilerplate
-code to generate new amplitudes or plotting scripts. On the other hand, there
-are also libraries like [`PyPWA`](https://github.com/JeffersonLab/PyPWA/)
-(written in Python) which seem like they could be easy to use, but often fail
-in this aspect due to Python's limiting syntax, speed issues, and a general
-lack of documentation and ongoing development. There have been attempts to
-bridge the gap between AmpTools and Python, most recently (and successfully)
-[`PyAmpTools`](https://github.com/lan13005/PyAmpTools). The difficulty with
-this method is that it relies on PyROOT, which also means you need ROOT
-installed (and built with your version of Python). For now, I'll spare you the
-anti-ROOT rant and just say that ROOT should be an opt-in, not a requirement.
-So where does that leave `rustitude`? As the name suggests, `rustitude` was
-written in Rust, so let's get the obvious downside out of the way: not many
-particle physicists know how to write Rust code. Hopefully, this will change
-over the next decade (and there has already been some [support](https://
-www.whitehouse.gov/oncd/briefing-room/2024/02/26/memory-safety-statements-of-
-support/) from the US government, of all places). While Rust carries the
-disadvantage of relative obscurity compared to C++, it also has many benefits.
-No `null` means no null references (Tony Hoare's ["billion dollar mistake"]
-(https://web.archive.org/web/20090628071208/http://qconlondon.com/london-2009/
-speaker/Tony+Hoare)). Pointers (called references in Rust) are always valid, a
-guarantee made by a very helpful and only occasionally frustrating borrow
-checker. Rust "crates" are set up in a way which encourages documentation (see
-[`rustitude-core`'s documentation](https://docs.rs/rustitude-core/)), and the
-basic syntax is fairly easy to learn for people who have been using optional
-type checking in Python. Perhaps one of the biggest benefits of Rust is how
-easy it is to employ [parallelization](https://crates.io/crates/rayon), but the
-two reasons I like it most are that it's incredibly easy to write Python
-bindings (that's what this library is after all) and it has a package manager.
-This second point is important -- unlike C/C++, where a developer is swamped
-with some menagerie `Makefile`, `CMakeLists.txt`, or some `scons` monstrosity
-which may only work on "X" system and only if you install and use `make`,
-`cmake`, `g++`, or whatever (oh yeah, and you made sure all your external
-dependencies are linked correctly, right? Right?), Rust supports adding a
-package by simply adding a line to `Cargo.toml` (or using the `cargo add`
-command). In many ways, package management in Rust is actually simpler than
-Python, since there's only one prefered method of creating and managing
-projects, formatting, linting, and compiling. Now I've covered why I don't like
-some of the existing solutions, and why I chose to use Rust, but what does this
-project have that makes it stand out? Here are some reasons to entice you: -
-`rustitude` will automatically parallelize amplitudes over the events in a
-dataset. There's no reason for a developer to ever write parallelized code
-themselves. - Implementing [`Node`](https://docs.rs/rustitude-core/latest/
-rustitude_core/amplitude/trait.Node.html) on a struct is all that is needed to
-use it as an amplitude. This means developers need only write two to three
-total methods to describe the entire functionality of their amplitude, and one
-of these just gives the names and order of the amplitude's input parameters. -
-A major goal of `rustitude` was to increase processing speed by sacrificing
-memory. This is done by precalculating parts of amplitudes which don't change
-when the free parameter inputs change. `AmpTools` supports a version of this,
-but only on the level of each general amplitude rather than on an individual
-basis. The simplest example of this is the `Ylm` amplitude (spherical
-harmonic), which can be entirely precalculated given the value of `l` and `m`.
-In `AmpTools`, different instances of `Ylm` with different `l`s and `m`s share
-precalculated data, whereas in `rustitude`, they don't. The `AmpTools`
-implementation of `Ylm` needs to calculate a spherical harmonic for every event
-on every function call, while `rustitude` just needs to look up a value in an
-array! - The majority of the library (the public interface) has Python
-bindings, so if there is no need for custom amplitudes, a developer never
-actually has to write any Rust code, and the resulting calculations will be as
-performant as if they were written in Rust. # Theory Amplitudes are registered
-into a named `sum` and `group`. Similar to `AmpTools`, the typical calculation
-for any event $e$ and list of parameters $\overrightarrow{p}$ will then be:
-```math I(\overrightarrow{p}, e) = \sum_{\text{groups} \in \text
-{sums}}\left|\sum_{\text{amplitudes} \in \text{groups}} \prod_{\text{amp} \in
-\text{amplitudes}} \text{amp}(\overrightarrow{p}, e)\right|^2 ``` #
-Installation Adding `rustitude` to an existing Rust project is as simple as
-```shell cargo add rustitude ``` The Python installation is equally
-straightforward: ```shell pip install rustitude ``` # Usage See the
-[`rustitude-core`](https://github.com/denehoffman/rustitude/tree/main/crates/
-rustitude-core) crate for a more in-depth tutorial on writing custom amplitudes
-in Rust. This package is mostly focused on the Python side of things. Here is
-the setup for an example analysis: ```python import rustitude as rt from
-rustitude import gluex import numpy as np # Start by creating some amplitudes:
-f0p = gluex.resonances.KMatrixF0('f0+', channel=2) f0n =
-gluex.resonances.KMatrixF0('f0-', channel=2) f2 = gluex.resonances.KMatrixF2
-('f2', channel=2) a0p = gluex.resonances.KMatrixA0('a0+', channel=1) a0n =
-gluex.resonances.KMatrixA0('a0-', channel=1) a2 = gluex.resonances.KMatrixA2
-('a2', channel=1) s0p = gluex.harmonics.Zlm('Z00+', 0, 0, reflectivity='+') s0n
-= gluex.harmonics.Zlm('Z00-', 0, 0, reflectivity='-') d2p = gluex.harmonics.Zlm
-('Z22+', 2, 2, reflectivity='+') # Next, let's put them together into a model #
-The API supports addition, and multiplication and has additional methods for
-the absolute-square (`norm_sqr`), real part (`real`) and imaginary part
-(`imag`). pos_re_sum = (f0p + a0p) * s0p.real() + (f2 + a2) * d2p.real()
-pos_im_sum = (f0p + a0p) * s0p.imag() + (f2 + a2) * d2p.imag() neg_re_sum =
-(f0n + a0n) * s0n.real() neg_im_sum = (f0n + a0n) * s0n.imag() mod = rt.Model
+### Table of Contents: - [Introduction](#Introduction) - [Installation]
+(#Installation) - [Usage](#Usage) - [TODOs](#TODOs) # Introduction This project
+began with a desire to make a fast but easy to use interface for fitting
+amplitudes to particle physics data. That being said, there are performant
+methods such as [`AmpTools`](https://github.com/mashephe/AmpTools), which is
+written in C++, but in my personal experience, it can be a bit tricky to use
+and extend, and it generally requires a lot of boilerplate code to generate new
+amplitudes or plotting scripts. On the other hand, there are also libraries
+like [`PyPWA`](https://github.com/JeffersonLab/PyPWA/) (written in Python)
+which seem like they could be easy to use, but often fail in this aspect due to
+Python's limiting syntax, speed issues, and a general lack of documentation and
+ongoing development. There have been attempts to bridge the gap between
+AmpTools and Python, most recently (and successfully) [`PyAmpTools`](https://
+github.com/lan13005/PyAmpTools). The difficulty with this method is that it
+relies on PyROOT, which also means you need ROOT installed (and built with your
+version of Python). For now, I'll spare you the anti-ROOT rant and just say
+that ROOT should be an opt-in, not a requirement. So where does that leave
+`rustitude`? As the name suggests, `rustitude` was written in Rust, so let's
+get the obvious downside out of the way: not many particle physicists know how
+to write Rust code. Hopefully, this will change over the next decade (and there
+has already been some [support](https://www.whitehouse.gov/oncd/briefing-room/
+2024/02/26/memory-safety-statements-of-support/) from the US government, of all
+places). While Rust carries the disadvantage of relative obscurity compared to
+C++, it also has many benefits. No `null` means no null references (Tony
+Hoare's ["billion dollar mistake"](https://web.archive.org/web/20090628071208/
+http://qconlondon.com/london-2009/speaker/Tony+Hoare)). Pointers (called
+references in Rust) are always valid, a guarantee made by a very helpful and
+only occasionally frustrating borrow checker. Rust "crates" are set up in a way
+which encourages documentation (see [`rustitude-core`'s documentation](https://
+docs.rs/rustitude-core/)), and the basic syntax is fairly easy to learn for
+people who have been using optional type checking in Python. Perhaps one of the
+biggest benefits of Rust is how easy it is to employ [parallelization](https://
+crates.io/crates/rayon), but the two reasons I like it most are that it's
+incredibly easy to write Python bindings (that's what this library is after
+all) and it has a package manager. This second point is important -- unlike C/
+C++, where a developer is swamped with some menagerie `Makefile`,
+`CMakeLists.txt`, or some `scons` monstrosity which may only work on "X" system
+and only if you install and use `make`, `cmake`, `g++`, or whatever (oh yeah,
+and you made sure all your external dependencies are linked correctly, right?
+Right?), Rust supports adding a package by simply adding a line to `Cargo.toml`
+(or using the `cargo add` command). In many ways, package management in Rust is
+actually simpler than Python, since there's only one prefered method of
+creating and managing projects, formatting, linting, and compiling. Now I've
+covered why I don't like some of the existing solutions, and why I chose to use
+Rust, but what does this project have that makes it stand out? Here are some
+reasons to entice you: - `rustitude` will automatically parallelize amplitudes
+over the events in a dataset. There's no reason for a developer to ever write
+parallelized code themselves. - Implementing [`Node`](https://docs.rs/
+rustitude-core/latest/rustitude_core/amplitude/trait.Node.html) on a struct is
+all that is needed to use it as an amplitude. This means developers need only
+write two to three total methods to describe the entire functionality of their
+amplitude, and one of these just gives the names and order of the amplitude's
+input parameters. - A major goal of `rustitude` was to increase processing
+speed by sacrificing memory. This is done by precalculating parts of amplitudes
+which don't change when the free parameter inputs change. `AmpTools` supports a
+version of this, but only on the level of each general amplitude rather than on
+an individual basis. The simplest example of this is the `Ylm` amplitude
+(spherical harmonic), which can be entirely precalculated given the value of
+`l` and `m`. In `AmpTools`, different instances of `Ylm` with different `l`s
+and `m`s share precalculated data, whereas in `rustitude`, they don't. The
+`AmpTools` implementation of `Ylm` needs to calculate a spherical harmonic for
+every event on every function call, while `rustitude` just needs to look up a
+value in an array! - The majority of the library (the public interface) has
+Python bindings, so if there is no need for custom amplitudes, a developer
+never actually has to write any Rust code, and the resulting calculations will
+be as performant as if they were written in Rust. # Installation Adding
+`rustitude` to an existing Rust project is as simple as ```shell cargo add
+rustitude ``` The Python installation is equally straightforward: ```shell pip
+install rustitude ``` # Usage See the [`rustitude-core`](https://github.com/
+denehoffman/rustitude/tree/main/crates/rustitude-core) crate for a more in-
+depth tutorial on writing custom amplitudes in Rust. This package is mostly
+focused on the Python side of things. Here is the setup for an example
+analysis: ```python import rustitude as rt from rustitude import gluex import
+numpy as np # Start by creating some amplitudes: f0p =
+gluex.resonances.KMatrixF0('f0+', channel=2) f0n = gluex.resonances.KMatrixF0
+('f0-', channel=2) f2 = gluex.resonances.KMatrixF2('f2', channel=2) a0p =
+gluex.resonances.KMatrixA0('a0+', channel=1) a0n = gluex.resonances.KMatrixA0
+('a0-', channel=1) a2 = gluex.resonances.KMatrixA2('a2', channel=1) s0p =
+gluex.harmonics.Zlm('Z00+', 0, 0, reflectivity='+') s0n = gluex.harmonics.Zlm
+('Z00-', 0, 0, reflectivity='-') d2p = gluex.harmonics.Zlm('Z22+', 2, 2,
+reflectivity='+') # Next, let's put them together into a model # The API
+supports addition, and multiplication and has additional methods for the
+absolute-square (`norm_sqr`), real part (`real`) and imaginary part (`imag`).
+pos_re_sum = (f0p + a0p) * s0p.real() + (f2 + a2) * d2p.real() pos_im_sum =
+(f0p + a0p) * s0p.imag() + (f2 + a2) * d2p.imag() neg_re_sum = (f0n + a0n) *
+s0n.real() neg_im_sum = (f0n + a0n) * s0n.imag() mod = rt.Model
 (pos_re_sum.norm_sqr() + pos_im_sum.norm_sqr() + neg_re_sum.norm_sqr() +
 neg_im_sum.norm_sqr()) # There is no need to constrain amplitudes, since each
 named amplitude is only ever evaluated once and a cached value gets pulled if
 we run across an amplitude by the same name! # We should, however, fix some of
 the values to make the fit less ambiguous. For instance, suppose we are above
 the threshold for the f_0(500) which is included in the F0 K-Matrix: mod.fix
 ("f0+", "f0_500 re", 0.0) mod.fix("f0+", "f0_500 im", 0.0) mod.fix("f0-",
```

### Comparing `rustitude-0.4.0/media/logo.png` & `rustitude-0.4.2/crates/rustitude/media/logo.png`

 * *Files identical despite different names*

### Comparing `rustitude-0.4.0/rustitude/__init__.py` & `rustitude-0.4.2/crates/rustitude/rustitude/__init__.py`

 * *Files identical despite different names*

### Comparing `rustitude-0.4.0/rustitude/__init__.pyi` & `rustitude-0.4.2/crates/rustitude/rustitude/__init__.pyi`

 * *Files identical despite different names*

### Comparing `rustitude-0.4.0/rustitude/gluex/harmonics.pyi` & `rustitude-0.4.2/crates/rustitude/rustitude/gluex/harmonics.pyi`

 * *Files identical despite different names*

### Comparing `rustitude-0.4.0/rustitude/gluex/resonances.pyi` & `rustitude-0.4.2/crates/rustitude/rustitude/gluex/resonances.pyi`

 * *Files identical despite different names*

### Comparing `rustitude-0.4.0/Cargo.lock` & `rustitude-0.4.2/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,26 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
+name = "anes"
+version = "0.1.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4b46cbb362ab8752921c97e041f5e366ee6297bd428a31275b9fcf1e380f7299"
+
+[[package]]
+name = "anstyle"
+version = "1.0.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "038dfcf04a5feb68e9c60b21c9625a54c2c0616e79b72b0fd87075a056ae1d1b"
+
+[[package]]
 name = "approx"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cab112f0a86d568ea0e627cc1d6be74a1e9cd55214684db5561995f6dad897c6"
 dependencies = [
  "num-complex",
  "num-traits",
@@ -239,14 +251,20 @@
 [[package]]
 name = "bytes"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
+name = "cast"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "37b2a672a2cb129a2e41c10b1224bb368f9f37a2b16b612598138befd7b37eb5"
+
+[[package]]
 name = "cc"
 version = "1.0.97"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "099a5357d84c4c61eb35fc8eafa9a79a902c2f76911e5747ced4e032edd8d9b4"
 dependencies = [
  "jobserver",
  "libc",
@@ -270,14 +288,66 @@
  "js-sys",
  "num-traits",
  "wasm-bindgen",
  "windows-targets",
 ]
 
 [[package]]
+name = "ciborium"
+version = "0.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "42e69ffd6f0917f5c029256a24d0161db17cea3997d185db0d35926308770f0e"
+dependencies = [
+ "ciborium-io",
+ "ciborium-ll",
+ "serde",
+]
+
+[[package]]
+name = "ciborium-io"
+version = "0.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "05afea1e0a06c9be33d539b876f1ce3692f4afea2cb41f740e7743225ed1c757"
+
+[[package]]
+name = "ciborium-ll"
+version = "0.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "57663b653d948a338bfb3eeba9bb2fd5fcfaecb9e199e87e1eda4d9e8b240fd9"
+dependencies = [
+ "ciborium-io",
+ "half",
+]
+
+[[package]]
+name = "clap"
+version = "4.5.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "90bc066a67923782aa8515dbaea16946c5bcc5addbd668bb80af688e53e548a0"
+dependencies = [
+ "clap_builder",
+]
+
+[[package]]
+name = "clap_builder"
+version = "4.5.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ae129e2e766ae0ec03484e609954119f123cc1fe650337e155d03b022f24f7b4"
+dependencies = [
+ "anstyle",
+ "clap_lex",
+]
+
+[[package]]
+name = "clap_lex"
+version = "0.7.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "98cc8fbded0c607b7ba9dd60cd98df59af97e84d24e49c8557331cfc26d301ce"
+
+[[package]]
 name = "const-random"
 version = "0.1.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87e00182fe74b066627d63b85fd550ac2998d4b0bd86bfed477a0ae4c7c71359"
 dependencies = [
  "const-random-macro",
 ]
@@ -305,14 +375,50 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b3855a8a784b474f333699ef2bbca9db2c4a1f6d9088a90a2d25b1eb53111eaa"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
+name = "criterion"
+version = "0.5.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f2b12d017a929603d80db1831cd3a24082f8137ce19c69e6447f54f5fc8d692f"
+dependencies = [
+ "anes",
+ "cast",
+ "ciborium",
+ "clap",
+ "criterion-plot",
+ "is-terminal",
+ "itertools 0.10.5",
+ "num-traits",
+ "once_cell",
+ "oorandom",
+ "plotters",
+ "rayon",
+ "regex",
+ "serde",
+ "serde_derive",
+ "serde_json",
+ "tinytemplate",
+ "walkdir",
+]
+
+[[package]]
+name = "criterion-plot"
+version = "0.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6b50826342786a51a89e2da3a28f1c32b06e387201bc2d19791f622c673706b1"
+dependencies = [
+ "cast",
+ "itertools 0.10.5",
+]
+
+[[package]]
 name = "crossbeam-deque"
 version = "0.8.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "613f8cc01fe9cf1a3eb3d7f488fd2fa8388403e97039e2f73692932e291a770d"
 dependencies = [
  "crossbeam-epoch",
  "crossbeam-utils",
@@ -424,14 +530,20 @@
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
+name = "hermit-abi"
+version = "0.3.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d231dfb89cfffdbc30e7fc41579ed6066ad03abda9e567ccafae602b97ec5024"
+
+[[package]]
 name = "iana-time-zone"
 version = "0.1.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e7ffbb5a1b541ea2561f8c41c087286cc091e21e556a4f09a8f6cbf17b69b141"
 dependencies = [
  "android_system_properties",
  "core-foundation-sys",
@@ -469,23 +581,49 @@
 [[package]]
 name = "integer-encoding"
 version = "3.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8bb03732005da905c88227371639bf1ad885cc712789c011c31c5fb3ab3ccf02"
 
 [[package]]
+name = "is-terminal"
+version = "0.4.12"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f23ff5ef2b80d608d61efee834934d862cd92461afc0560dedf493e4c033738b"
+dependencies = [
+ "hermit-abi",
+ "libc",
+ "windows-sys",
+]
+
+[[package]]
+name = "itertools"
+version = "0.10.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
+dependencies = [
+ "either",
+]
+
+[[package]]
 name = "itertools"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ba291022dbbd398a455acf126c1e341954079855bc60dfdda641363bd6922569"
 dependencies = [
  "either",
 ]
 
 [[package]]
+name = "itoa"
+version = "1.0.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
+
+[[package]]
 name = "jobserver"
 version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2b099aaa34a9751c5bf0878add70444e1ed2dd73f347be99003d4577277de6e"
 dependencies = [
  "libc",
 ]
@@ -786,14 +924,20 @@
 [[package]]
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
+name = "oorandom"
+version = "11.1.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
+
+[[package]]
 name = "ordered-float"
 version = "2.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "68f19d67e5a2795c94e73e0bb1cc1a7edeb2e28efd39e2e1c9b7a40c1108b11c"
 dependencies = [
  "num-traits",
 ]
@@ -803,15 +947,15 @@
 version = "0.1.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "375243dc9999fb931dfec482422763bdcac44f4980615afff91e999f3c40498c"
 dependencies = [
  "chrono",
  "downcast",
  "flate2",
- "itertools",
+ "itertools 0.12.1",
  "lazy_static",
  "log",
  "lz4",
  "num",
  "num-derive",
  "num-traits",
  "paste",
@@ -885,14 +1029,42 @@
 [[package]]
 name = "pkg-config"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d231b230927b5e4ad203db57bbcbee2802f6bce620b1e4a9024a07d94e2907ec"
 
 [[package]]
+name = "plotters"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d2c224ba00d7cadd4d5c660deaf2098e5e80e07846537c51f9cfa4be50c1fd45"
+dependencies = [
+ "num-traits",
+ "plotters-backend",
+ "plotters-svg",
+ "wasm-bindgen",
+ "web-sys",
+]
+
+[[package]]
+name = "plotters-backend"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9e76628b4d3a7581389a35d5b6e2139607ad7c75b17aed325f210aa91f4a9609"
+
+[[package]]
+name = "plotters-svg"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "38f6d39893cca0701371e3c27294f09797214b86f1fb951b89ade8ec04e2abab"
+dependencies = [
+ "plotters-backend",
+]
+
+[[package]]
 name = "portable-atomic"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
 
 [[package]]
 name = "primal-bit"
@@ -926,14 +1098,25 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8ad3d49ab951a01fbaafe34f2ec74122942fe18a3f9814c3268f1bb72042131b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
+name = "py-rustitude"
+version = "0.4.1"
+dependencies = [
+ "pyo3",
+ "rayon",
+ "rustitude",
+ "rustitude-core",
+ "rustitude-gluex",
+]
+
+[[package]]
 name = "pyo3"
 version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
 dependencies = [
  "cfg-if",
  "indoc",
@@ -1072,29 +1255,28 @@
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustitude"
-version = "0.4.0"
+version = "0.4.2"
 dependencies = [
- "pyo3",
- "rayon",
+ "criterion",
  "rustitude-core",
  "rustitude-gluex",
 ]
 
 [[package]]
 name = "rustitude-core"
 version = "1.0.0"
 dependencies = [
  "approx",
  "indexmap",
- "itertools",
+ "itertools 0.12.1",
  "nalgebra",
  "num",
  "num-complex",
  "num-traits",
  "oxyroot",
  "parking_lot",
  "parquet",
@@ -1102,15 +1284,15 @@
  "rayon",
  "sphrs",
  "thiserror",
 ]
 
 [[package]]
 name = "rustitude-gluex"
-version = "0.2.0"
+version = "0.2.1"
 dependencies = [
  "factorial",
  "nalgebra",
  "num-complex",
  "pyo3",
  "rayon",
  "rustitude-core",
@@ -1129,14 +1311,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f398075ce1e6a179b46f51bd88d0598b92b00d3551f1a2d4ac49e771b56ac354"
 dependencies = [
  "bytemuck",
 ]
 
 [[package]]
+name = "same-file"
+version = "1.0.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
+dependencies = [
+ "winapi-util",
+]
+
+[[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "semver"
@@ -1147,14 +1338,45 @@
 [[package]]
 name = "seq-macro"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a3f0bf26fd526d2a95683cd0f87bf103b8539e2ca1ef48ce002d67aad59aa0b4"
 
 [[package]]
+name = "serde"
+version = "1.0.202"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "226b61a0d411b2ba5ff6d7f73a476ac4f8bb900373459cd00fab8512828ba395"
+dependencies = [
+ "serde_derive",
+]
+
+[[package]]
+name = "serde_derive"
+version = "1.0.202"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6048858004bcff69094cd972ed40a32500f153bd3be9f716b2eed2e8217c4838"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.63",
+]
+
+[[package]]
+name = "serde_json"
+version = "1.0.117"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "455182ea6142b14f93f4bc5320a2b31c1f266b66a4a5c858b013302a5d8cbfc3"
+dependencies = [
+ "itoa",
+ "ryu",
+ "serde",
+]
+
+[[package]]
 name = "simba"
 version = "0.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "061507c94fc6ab4ba1c9a0305018408e312e17c041eb63bef8aa726fa33aceae"
 dependencies = [
  "approx",
  "num-complex",
@@ -1257,14 +1479,24 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2c9d3793400a45f954c52e73d068316d76b6f4e36977e3fcebb13a2721e80237"
 dependencies = [
  "crunchy",
 ]
 
 [[package]]
+name = "tinytemplate"
+version = "1.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "be4d6b5f19ff7664e8c98d03e2139cb510db9b0a60b55f8e8709b689d939b6bc"
+dependencies = [
+ "serde",
+ "serde_json",
+]
+
+[[package]]
 name = "trait-set"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b79e2e9c9ab44c6d7c20d5976961b47e8f49ac199154daa514b77cd1ab536625"
 dependencies = [
  "proc-macro2",
  "quote",
@@ -1308,14 +1540,24 @@
 [[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
+name = "walkdir"
+version = "2.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "29790946404f91d9c5d06f9874efddea1dc06c5efe94541a7d6863108e3a5e4b"
+dependencies = [
+ "same-file",
+ "winapi-util",
+]
+
+[[package]]
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
@@ -1368,33 +1610,61 @@
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "af190c94f2773fdb3729c55b007a722abb5384da03bc0986df4c289bf5567e96"
 
 [[package]]
+name = "web-sys"
+version = "0.3.69"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "77afa9a11836342370f4817622a2f0f418b134426d91a82dfb48f532d2ec13ef"
+dependencies = [
+ "js-sys",
+ "wasm-bindgen",
+]
+
+[[package]]
 name = "wide"
 version = "0.7.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aab6594190de06d718a5dbc5fa781ab62f8903797056480e549ca74add6b7065"
 dependencies = [
  "bytemuck",
  "safe_arch",
 ]
 
 [[package]]
+name = "winapi-util"
+version = "0.1.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4d4cc384e1e73b93bafa6fb4f1df8c41695c8a91cf9c4c64358067d15a7b6c6b"
+dependencies = [
+ "windows-sys",
+]
+
+[[package]]
 name = "windows-core"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
 dependencies = [
  "windows-targets",
 ]
 
 [[package]]
+name = "windows-sys"
+version = "0.52.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
+dependencies = [
+ "windows-targets",
+]
+
+[[package]]
 name = "windows-targets"
 version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
```

### Comparing `rustitude-0.4.0/pyproject.toml` & `rustitude-0.4.2/crates/rustitude/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rustitude-0.4.0/PKG-INFO` & `rustitude-0.4.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.3
 Name: rustitude
-Version: 0.4.0
+Version: 0.4.2
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Dist: uproot
 Requires-Dist: numpy
 License-File: LICENSE
+License-File: LICENSE
 Summary: Python bindings for the Rustitude library
 Keywords: physics,math,rust
-Home-Page: https://github.com/denehoffman/rustitude/
 Author: Nathaniel Dene Hoffman
 Author-email: dene@cmu.edu
 Maintainer-email: Nathaniel Dene Hoffman <dene@cmu.edu>
-License: BSD-3-Clause
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: homepage, https://github.com/denehoffman/rustitude
 Project-URL: repository, https://github.com/denehoffman/rustitude
 Project-URL: changelog, https://github.com/denehoffman/rustitude/blob/main/CHANGELOG.md
 
 <p align="center">
@@ -41,15 +40,14 @@
   <a href="https://docs.rs/rustitude" alt="Rustitude documentation on docs.rs">
     <img src="https://img.shields.io/docsrs/rustitude" /></a>
 </p>
 
 ### Table of Contents:
 
 - [Introduction](#Introduction)
-- [Theory](#Theory)
 - [Installation](#Installation)
 - [Usage](#Usage)
 - [TODOs](#TODOs)
 
 # Introduction
 
 This project began with a desire to make a fast but easy to use interface for fitting amplitudes to particle physics data. That being said, there are performant methods such as [`AmpTools`](https://github.com/mashephe/AmpTools), which is written in C++, but in my personal experience, it can be a bit tricky to use and extend, and it generally requires a lot of boilerplate code to generate new amplitudes or plotting scripts. On the other hand, there are also libraries like [`PyPWA`](https://github.com/JeffersonLab/PyPWA/) (written in Python) which seem like they could be easy to use, but often fail in this aspect due to Python's limiting syntax, speed issues, and a general lack of documentation and ongoing development. There have been attempts to bridge the gap between AmpTools and Python, most recently (and successfully) [`PyAmpTools`](https://github.com/lan13005/PyAmpTools). The difficulty with this method is that it relies on PyROOT, which also means you need ROOT installed (and built with your version of Python). For now, I'll spare you the anti-ROOT rant and just say that ROOT should be an opt-in, not a requirement. So where does that leave `rustitude`?
@@ -59,22 +57,14 @@
 Now I've covered why I don't like some of the existing solutions, and why I chose to use Rust, but what does this project have that makes it stand out? Here are some reasons to entice you:
 
 - `rustitude` will automatically parallelize amplitudes over the events in a dataset. There's no reason for a developer to ever write parallelized code themselves.
 - Implementing [`Node`](https://docs.rs/rustitude-core/latest/rustitude_core/amplitude/trait.Node.html) on a struct is all that is needed to use it as an amplitude. This means developers need only write two to three total methods to describe the entire functionality of their amplitude, and one of these just gives the names and order of the amplitude's input parameters.
 - A major goal of `rustitude` was to increase processing speed by sacrificing memory. This is done by precalculating parts of amplitudes which don't change when the free parameter inputs change. `AmpTools` supports a version of this, but only on the level of each general amplitude rather than on an individual basis. The simplest example of this is the `Ylm` amplitude (spherical harmonic), which can be entirely precalculated given the value of `l` and `m`. In `AmpTools`, different instances of `Ylm` with different `l`s and `m`s share precalculated data, whereas in `rustitude`, they don't. The `AmpTools` implementation of `Ylm` needs to calculate a spherical harmonic for every event on every function call, while `rustitude` just needs to look up a value in an array!
 - The majority of the library (the public interface) has Python bindings, so if there is no need for custom amplitudes, a developer never actually has to write any Rust code, and the resulting calculations will be as performant as if they were written in Rust.
 
-# Theory
-
-Amplitudes are registered into a named `sum` and `group`. Similar to `AmpTools`, the typical calculation for any event $e$ and list of parameters $\overrightarrow{p}$ will then be:
-
-```math
-I(\overrightarrow{p}, e) = \sum_{\text{groups} \in \text{sums}}\left|\sum_{\text{amplitudes} \in \text{groups}} \prod_{\text{amp} \in \text{amplitudes}} \text{amp}(\overrightarrow{p}, e)\right|^2
-```
-
 # Installation
 
 Adding `rustitude` to an existing Rust project is as simple as
 
 ```shell
 cargo add rustitude
 ```
```

#### html2text {}

```diff
@@ -1,116 +1,110 @@
-Metadata-Version: 2.3 Name: rustitude Version: 0.4.0 Classifier: Development
+Metadata-Version: 2.3 Name: rustitude Version: 0.4.2 Classifier: Development
 Status :: 4 - Beta Classifier: Programming Language :: Python Requires-Dist:
-uproot Requires-Dist: numpy License-File: LICENSE Summary: Python bindings for
-the Rustitude library Keywords: physics,math,rust Home-Page: https://
-github.com/denehoffman/rustitude/ Author: Nathaniel Dene Hoffman Author-email:
-dene@cmu.edu Maintainer-email: Nathaniel Dene Hoffman
-cmu.edu> License: BSD-3-Clause Requires-Python: >=3.7 Description-Content-Type:
-text/markdown; charset=UTF-8; variant=GFM Project-URL: homepage, https://
-github.com/denehoffman/rustitude Project-URL: repository, https://github.com/
-denehoffman/rustitude Project-URL: changelog, https://github.com/denehoffman/
-rustitude/blob/main/CHANGELOG.md
+uproot Requires-Dist: numpy License-File: LICENSE License-File: LICENSE
+Summary: Python bindings for the Rustitude library Keywords: physics,math,rust
+Author: Nathaniel Dene Hoffman Author-email: dene@cmu.edu Maintainer-email:
+Nathaniel Dene Hoffman
+cmu.edu> Requires-Python: >=3.7 Description-Content-Type: text/markdown;
+charset=UTF-8; variant=GFM Project-URL: homepage, https://github.com/
+denehoffman/rustitude Project-URL: repository, https://github.com/denehoffman/
+rustitude Project-URL: changelog, https://github.com/denehoffman/rustitude/
+blob/main/CHANGELOG.md
  [https://raw.githubusercontent.com/denehoffman/rustitude/main/media/logo.png]
                  ************ DDeemmyyssttiiffyyiinngg AAmmpplliittuuddee AAnnaallyyssiiss ************
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_a_s_t_-_c_o_m_m_i_t_/_d_e_n_e_h_o_f_f_m_a_n_/_r_u_s_t_i_t_u_d_e_/_m_a_i_n_]_[_h_t_t_p_s_:_/_/
  _i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_/_s_t_a_t_u_s_/_d_e_n_e_h_o_f_f_m_a_n_/_r_u_s_t_i_t_u_d_e_/_r_u_s_t_._y_m_l_]
     _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_i_c_e_n_s_e_/_d_e_n_e_h_o_f_f_m_a_n_/_r_u_s_t_i_t_u_d_e_]_[_h_t_t_p_s_:_/_/
   _i_m_g_._s_h_i_e_l_d_s_._i_o_/_c_r_a_t_e_s_/_v_/_r_u_s_t_i_t_u_d_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_d_o_c_s_r_s_/_r_u_s_t_i_t_u_d_e_]
-### Table of Contents: - [Introduction](#Introduction) - [Theory](#Theory) -
-[Installation](#Installation) - [Usage](#Usage) - [TODOs](#TODOs) #
-Introduction This project began with a desire to make a fast but easy to use
-interface for fitting amplitudes to particle physics data. That being said,
-there are performant methods such as [`AmpTools`](https://github.com/mashephe/
-AmpTools), which is written in C++, but in my personal experience, it can be a
-bit tricky to use and extend, and it generally requires a lot of boilerplate
-code to generate new amplitudes or plotting scripts. On the other hand, there
-are also libraries like [`PyPWA`](https://github.com/JeffersonLab/PyPWA/)
-(written in Python) which seem like they could be easy to use, but often fail
-in this aspect due to Python's limiting syntax, speed issues, and a general
-lack of documentation and ongoing development. There have been attempts to
-bridge the gap between AmpTools and Python, most recently (and successfully)
-[`PyAmpTools`](https://github.com/lan13005/PyAmpTools). The difficulty with
-this method is that it relies on PyROOT, which also means you need ROOT
-installed (and built with your version of Python). For now, I'll spare you the
-anti-ROOT rant and just say that ROOT should be an opt-in, not a requirement.
-So where does that leave `rustitude`? As the name suggests, `rustitude` was
-written in Rust, so let's get the obvious downside out of the way: not many
-particle physicists know how to write Rust code. Hopefully, this will change
-over the next decade (and there has already been some [support](https://
-www.whitehouse.gov/oncd/briefing-room/2024/02/26/memory-safety-statements-of-
-support/) from the US government, of all places). While Rust carries the
-disadvantage of relative obscurity compared to C++, it also has many benefits.
-No `null` means no null references (Tony Hoare's ["billion dollar mistake"]
-(https://web.archive.org/web/20090628071208/http://qconlondon.com/london-2009/
-speaker/Tony+Hoare)). Pointers (called references in Rust) are always valid, a
-guarantee made by a very helpful and only occasionally frustrating borrow
-checker. Rust "crates" are set up in a way which encourages documentation (see
-[`rustitude-core`'s documentation](https://docs.rs/rustitude-core/)), and the
-basic syntax is fairly easy to learn for people who have been using optional
-type checking in Python. Perhaps one of the biggest benefits of Rust is how
-easy it is to employ [parallelization](https://crates.io/crates/rayon), but the
-two reasons I like it most are that it's incredibly easy to write Python
-bindings (that's what this library is after all) and it has a package manager.
-This second point is important -- unlike C/C++, where a developer is swamped
-with some menagerie `Makefile`, `CMakeLists.txt`, or some `scons` monstrosity
-which may only work on "X" system and only if you install and use `make`,
-`cmake`, `g++`, or whatever (oh yeah, and you made sure all your external
-dependencies are linked correctly, right? Right?), Rust supports adding a
-package by simply adding a line to `Cargo.toml` (or using the `cargo add`
-command). In many ways, package management in Rust is actually simpler than
-Python, since there's only one prefered method of creating and managing
-projects, formatting, linting, and compiling. Now I've covered why I don't like
-some of the existing solutions, and why I chose to use Rust, but what does this
-project have that makes it stand out? Here are some reasons to entice you: -
-`rustitude` will automatically parallelize amplitudes over the events in a
-dataset. There's no reason for a developer to ever write parallelized code
-themselves. - Implementing [`Node`](https://docs.rs/rustitude-core/latest/
-rustitude_core/amplitude/trait.Node.html) on a struct is all that is needed to
-use it as an amplitude. This means developers need only write two to three
-total methods to describe the entire functionality of their amplitude, and one
-of these just gives the names and order of the amplitude's input parameters. -
-A major goal of `rustitude` was to increase processing speed by sacrificing
-memory. This is done by precalculating parts of amplitudes which don't change
-when the free parameter inputs change. `AmpTools` supports a version of this,
-but only on the level of each general amplitude rather than on an individual
-basis. The simplest example of this is the `Ylm` amplitude (spherical
-harmonic), which can be entirely precalculated given the value of `l` and `m`.
-In `AmpTools`, different instances of `Ylm` with different `l`s and `m`s share
-precalculated data, whereas in `rustitude`, they don't. The `AmpTools`
-implementation of `Ylm` needs to calculate a spherical harmonic for every event
-on every function call, while `rustitude` just needs to look up a value in an
-array! - The majority of the library (the public interface) has Python
-bindings, so if there is no need for custom amplitudes, a developer never
-actually has to write any Rust code, and the resulting calculations will be as
-performant as if they were written in Rust. # Theory Amplitudes are registered
-into a named `sum` and `group`. Similar to `AmpTools`, the typical calculation
-for any event $e$ and list of parameters $\overrightarrow{p}$ will then be:
-```math I(\overrightarrow{p}, e) = \sum_{\text{groups} \in \text
-{sums}}\left|\sum_{\text{amplitudes} \in \text{groups}} \prod_{\text{amp} \in
-\text{amplitudes}} \text{amp}(\overrightarrow{p}, e)\right|^2 ``` #
-Installation Adding `rustitude` to an existing Rust project is as simple as
-```shell cargo add rustitude ``` The Python installation is equally
-straightforward: ```shell pip install rustitude ``` # Usage See the
-[`rustitude-core`](https://github.com/denehoffman/rustitude/tree/main/crates/
-rustitude-core) crate for a more in-depth tutorial on writing custom amplitudes
-in Rust. This package is mostly focused on the Python side of things. Here is
-the setup for an example analysis: ```python import rustitude as rt from
-rustitude import gluex import numpy as np # Start by creating some amplitudes:
-f0p = gluex.resonances.KMatrixF0('f0+', channel=2) f0n =
-gluex.resonances.KMatrixF0('f0-', channel=2) f2 = gluex.resonances.KMatrixF2
-('f2', channel=2) a0p = gluex.resonances.KMatrixA0('a0+', channel=1) a0n =
-gluex.resonances.KMatrixA0('a0-', channel=1) a2 = gluex.resonances.KMatrixA2
-('a2', channel=1) s0p = gluex.harmonics.Zlm('Z00+', 0, 0, reflectivity='+') s0n
-= gluex.harmonics.Zlm('Z00-', 0, 0, reflectivity='-') d2p = gluex.harmonics.Zlm
-('Z22+', 2, 2, reflectivity='+') # Next, let's put them together into a model #
-The API supports addition, and multiplication and has additional methods for
-the absolute-square (`norm_sqr`), real part (`real`) and imaginary part
-(`imag`). pos_re_sum = (f0p + a0p) * s0p.real() + (f2 + a2) * d2p.real()
-pos_im_sum = (f0p + a0p) * s0p.imag() + (f2 + a2) * d2p.imag() neg_re_sum =
-(f0n + a0n) * s0n.real() neg_im_sum = (f0n + a0n) * s0n.imag() mod = rt.Model
+### Table of Contents: - [Introduction](#Introduction) - [Installation]
+(#Installation) - [Usage](#Usage) - [TODOs](#TODOs) # Introduction This project
+began with a desire to make a fast but easy to use interface for fitting
+amplitudes to particle physics data. That being said, there are performant
+methods such as [`AmpTools`](https://github.com/mashephe/AmpTools), which is
+written in C++, but in my personal experience, it can be a bit tricky to use
+and extend, and it generally requires a lot of boilerplate code to generate new
+amplitudes or plotting scripts. On the other hand, there are also libraries
+like [`PyPWA`](https://github.com/JeffersonLab/PyPWA/) (written in Python)
+which seem like they could be easy to use, but often fail in this aspect due to
+Python's limiting syntax, speed issues, and a general lack of documentation and
+ongoing development. There have been attempts to bridge the gap between
+AmpTools and Python, most recently (and successfully) [`PyAmpTools`](https://
+github.com/lan13005/PyAmpTools). The difficulty with this method is that it
+relies on PyROOT, which also means you need ROOT installed (and built with your
+version of Python). For now, I'll spare you the anti-ROOT rant and just say
+that ROOT should be an opt-in, not a requirement. So where does that leave
+`rustitude`? As the name suggests, `rustitude` was written in Rust, so let's
+get the obvious downside out of the way: not many particle physicists know how
+to write Rust code. Hopefully, this will change over the next decade (and there
+has already been some [support](https://www.whitehouse.gov/oncd/briefing-room/
+2024/02/26/memory-safety-statements-of-support/) from the US government, of all
+places). While Rust carries the disadvantage of relative obscurity compared to
+C++, it also has many benefits. No `null` means no null references (Tony
+Hoare's ["billion dollar mistake"](https://web.archive.org/web/20090628071208/
+http://qconlondon.com/london-2009/speaker/Tony+Hoare)). Pointers (called
+references in Rust) are always valid, a guarantee made by a very helpful and
+only occasionally frustrating borrow checker. Rust "crates" are set up in a way
+which encourages documentation (see [`rustitude-core`'s documentation](https://
+docs.rs/rustitude-core/)), and the basic syntax is fairly easy to learn for
+people who have been using optional type checking in Python. Perhaps one of the
+biggest benefits of Rust is how easy it is to employ [parallelization](https://
+crates.io/crates/rayon), but the two reasons I like it most are that it's
+incredibly easy to write Python bindings (that's what this library is after
+all) and it has a package manager. This second point is important -- unlike C/
+C++, where a developer is swamped with some menagerie `Makefile`,
+`CMakeLists.txt`, or some `scons` monstrosity which may only work on "X" system
+and only if you install and use `make`, `cmake`, `g++`, or whatever (oh yeah,
+and you made sure all your external dependencies are linked correctly, right?
+Right?), Rust supports adding a package by simply adding a line to `Cargo.toml`
+(or using the `cargo add` command). In many ways, package management in Rust is
+actually simpler than Python, since there's only one prefered method of
+creating and managing projects, formatting, linting, and compiling. Now I've
+covered why I don't like some of the existing solutions, and why I chose to use
+Rust, but what does this project have that makes it stand out? Here are some
+reasons to entice you: - `rustitude` will automatically parallelize amplitudes
+over the events in a dataset. There's no reason for a developer to ever write
+parallelized code themselves. - Implementing [`Node`](https://docs.rs/
+rustitude-core/latest/rustitude_core/amplitude/trait.Node.html) on a struct is
+all that is needed to use it as an amplitude. This means developers need only
+write two to three total methods to describe the entire functionality of their
+amplitude, and one of these just gives the names and order of the amplitude's
+input parameters. - A major goal of `rustitude` was to increase processing
+speed by sacrificing memory. This is done by precalculating parts of amplitudes
+which don't change when the free parameter inputs change. `AmpTools` supports a
+version of this, but only on the level of each general amplitude rather than on
+an individual basis. The simplest example of this is the `Ylm` amplitude
+(spherical harmonic), which can be entirely precalculated given the value of
+`l` and `m`. In `AmpTools`, different instances of `Ylm` with different `l`s
+and `m`s share precalculated data, whereas in `rustitude`, they don't. The
+`AmpTools` implementation of `Ylm` needs to calculate a spherical harmonic for
+every event on every function call, while `rustitude` just needs to look up a
+value in an array! - The majority of the library (the public interface) has
+Python bindings, so if there is no need for custom amplitudes, a developer
+never actually has to write any Rust code, and the resulting calculations will
+be as performant as if they were written in Rust. # Installation Adding
+`rustitude` to an existing Rust project is as simple as ```shell cargo add
+rustitude ``` The Python installation is equally straightforward: ```shell pip
+install rustitude ``` # Usage See the [`rustitude-core`](https://github.com/
+denehoffman/rustitude/tree/main/crates/rustitude-core) crate for a more in-
+depth tutorial on writing custom amplitudes in Rust. This package is mostly
+focused on the Python side of things. Here is the setup for an example
+analysis: ```python import rustitude as rt from rustitude import gluex import
+numpy as np # Start by creating some amplitudes: f0p =
+gluex.resonances.KMatrixF0('f0+', channel=2) f0n = gluex.resonances.KMatrixF0
+('f0-', channel=2) f2 = gluex.resonances.KMatrixF2('f2', channel=2) a0p =
+gluex.resonances.KMatrixA0('a0+', channel=1) a0n = gluex.resonances.KMatrixA0
+('a0-', channel=1) a2 = gluex.resonances.KMatrixA2('a2', channel=1) s0p =
+gluex.harmonics.Zlm('Z00+', 0, 0, reflectivity='+') s0n = gluex.harmonics.Zlm
+('Z00-', 0, 0, reflectivity='-') d2p = gluex.harmonics.Zlm('Z22+', 2, 2,
+reflectivity='+') # Next, let's put them together into a model # The API
+supports addition, and multiplication and has additional methods for the
+absolute-square (`norm_sqr`), real part (`real`) and imaginary part (`imag`).
+pos_re_sum = (f0p + a0p) * s0p.real() + (f2 + a2) * d2p.real() pos_im_sum =
+(f0p + a0p) * s0p.imag() + (f2 + a2) * d2p.imag() neg_re_sum = (f0n + a0n) *
+s0n.real() neg_im_sum = (f0n + a0n) * s0n.imag() mod = rt.Model
 (pos_re_sum.norm_sqr() + pos_im_sum.norm_sqr() + neg_re_sum.norm_sqr() +
 neg_im_sum.norm_sqr()) # There is no need to constrain amplitudes, since each
 named amplitude is only ever evaluated once and a cached value gets pulled if
 we run across an amplitude by the same name! # We should, however, fix some of
 the values to make the fit less ambiguous. For instance, suppose we are above
 the threshold for the f_0(500) which is included in the F0 K-Matrix: mod.fix
 ("f0+", "f0_500 re", 0.0) mod.fix("f0+", "f0_500 im", 0.0) mod.fix("f0-",
```

