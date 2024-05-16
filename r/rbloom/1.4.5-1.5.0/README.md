# Comparing `tmp/rbloom-1.4.5.tar.gz` & `tmp/rbloom-1.5.0.tar.gz`

## Comparing `rbloom-1.4.5.tar` & `rbloom-1.5.0.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0      341 1970-01-01 00:00:00.000000 rbloom-1.4.5/Cargo.toml
--rw-r--r--   0     1001      123     1665 2023-06-10 08:09:20.000000 rbloom-1.4.5/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      699 2023-06-10 08:09:20.000000 rbloom-1.4.5/.gitignore
--rw-r--r--   0     1001      123     1103 2023-06-10 08:09:20.000000 rbloom-1.4.5/LICENSE
--rw-r--r--   0     1001      123    10890 2023-06-10 08:09:20.000000 rbloom-1.4.5/README.md
--rw-r--r--   0     1001      123      536 2023-06-10 08:09:20.000000 rbloom-1.4.5/pyproject.toml
--rw-r--r--   0     1001      123     2896 2023-06-10 08:09:20.000000 rbloom-1.4.5/rbloom.pyi
--rwxr-xr-x   0     1001      123     1058 2023-06-10 08:10:22.000000 rbloom-1.4.5/run-maturin-action.sh
--rw-r--r--   0     1001      123    17789 2023-06-10 08:09:20.000000 rbloom-1.4.5/src/lib.rs
--rwxr-xr-x   0     1001      123     2681 2023-06-10 08:09:20.000000 rbloom-1.4.5/tests/api_test.py
--rw-r--r--   0        0        0     7419 2023-06-10 08:10:51.000000 rbloom-1.4.5/Cargo.lock
--rw-r--r--   0        0        0    11387 1970-01-01 00:00:00.000000 rbloom-1.4.5/PKG-INFO
+-rw-r--r--   0        0        0      351 1970-01-01 00:00:00.000000 rbloom-1.5.0/Cargo.toml
+-rw-r--r--   0     1001      127     1665 2024-01-19 17:06:51.000000 rbloom-1.5.0/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      699 2024-01-19 17:06:51.000000 rbloom-1.5.0/.gitignore
+-rw-r--r--   0     1001      127     1136 2024-01-19 17:06:51.000000 rbloom-1.5.0/LICENSE
+-rw-r--r--   0     1001      127    11326 2024-01-19 17:06:51.000000 rbloom-1.5.0/README.md
+-rw-r--r--   0     1001      127      536 2024-01-19 17:06:51.000000 rbloom-1.5.0/pyproject.toml
+-rw-r--r--   0     1001      127     3140 2024-01-19 17:06:51.000000 rbloom-1.5.0/rbloom.pyi
+-rw-r--r--   0     1001      127    19719 2024-01-19 17:06:51.000000 rbloom-1.5.0/src/lib.rs
+-rwxr-xr-x   0     1001      127     2893 2024-01-19 17:06:51.000000 rbloom-1.5.0/tests/api_test.py
+-rw-r--r--   0        0        0     7616 2024-01-19 17:07:57.000000 rbloom-1.5.0/Cargo.lock
+-rw-r--r--   0        0        0    11823 1970-01-01 00:00:00.000000 rbloom-1.5.0/PKG-INFO
```

### Comparing `rbloom-1.4.5/.github/workflows/CI.yml` & `rbloom-1.5.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `rbloom-1.4.5/.gitignore` & `rbloom-1.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `rbloom-1.4.5/LICENSE` & `rbloom-1.5.0/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 MIT License
 
 Copyright (c) 2023 Kenan Hanke
 Copyright (c) 2023 Zachary Dremann
+Copyright (c) 2023 Rory McNamara
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `rbloom-1.4.5/README.md` & `rbloom-1.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -149,18 +149,21 @@
     def hash_func(self) -> Callable[[Any], int]   # retrieve the hash_func
                                                   # given to __init__
 
     @property
     def approx_items(self) -> float    # estimated number of items in
                                        # the filter
 
+    # see section "Persistence" for more information on these four methods
     @classmethod
-    def load(cls, filepath: str, hash_func) -> Bloom      # see "Persistence"
-
-    def save(self, filepath: str)                 # see section "Persistence"
+    def load(cls, filepath: str, hash_func) -> Bloom
+    def save(self, filepath: str)
+    @classmethod
+    def load_bytes(cls, data: bytes, hash_func) -> Bloom
+    def save_bytes(self) -> bytes
 
     #####################################################################
     #                    ALL SUBSEQUENT METHODS ARE                     #
     #              EQUIVALENT TO THE CORRESPONDING METHODS              #
     #                     OF THE BUILT-IN SET TYPE                      #
     #####################################################################
 
@@ -235,30 +238,40 @@
 you from shooting yourself in the foot.
 
 Also note that using a custom hash will incur a performance penalty over
 using the built-in hash.
 
 ## Persistence
 
-The `save` and `load` methods allow you to save and load filters to and
-from disk. However, as the built-in hash function's salt changes between
-invocations of Python, they only work on filters with custom hash
-functions. Note that it is your responsibility to ensure that the hash
-function you supply to `load` is the same as the one originally used by
-the filter you're loading!
+The `save` and `load` methods, along with their byte-oriented counterparts
+`save_bytes` and `load_bytes`, allow you to save and load filters to and
+from disk/Python `bytes` objects. However, as the built-in hash function's
+salt changes between invocations of Python, they only work on filters with
+custom hash functions. Note that it is your responsibility to ensure that
+the hash function you supply to the loading functions is the same as the
+one originally used by the filter you're loading!
 
 ```python
 bf = Bloom(10_000, 0.01, some_hash_func)
 bf.add("hello")
 bf.add("world")
 
+# saving to a file
 bf.save("bf.bloom")
 
+# loading from a file
 loaded_bf = Bloom.load("bf.bloom", some_hash_func)
 assert loaded_bf == bf
+
+# saving to bytes
+bf_bytes = bf.save_bytes()
+
+# loading from bytes
+loaded_bf_from_bytes = Bloom.load_bytes(bf_bytes, some_hash_func)
+assert loaded_bf_from_bytes == bf
 ```
 
 The size of the file is `bf.size_in_bits / 8 + 8` bytes.
 
 ---
 
 **Statement of attribution:** Bloom filters were originally proposed in
```

### Comparing `rbloom-1.4.5/pyproject.toml` & `rbloom-1.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rbloom-1.4.5/rbloom.pyi` & `rbloom-1.5.0/rbloom.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -22,17 +22,24 @@
     @property
     def approx_items(self) -> float: ...
 
     # load from file, see section "Persistence"
     @classmethod
     def load(cls, filepath: str, hash_func: Callable[[Any], int]) -> Bloom: ...
 
+    # load from bytes(), see section "Persistence"
+    @classmethod
+    def load_bytes(cls, data: bytes, hash_func: Callable[[Any], int]) -> Bloom: ...
+
     # save to file, see section "Persistence"
     def save(self, filepath: str) -> None: ...
 
+    # save to a bytes(), see section "Persistence"
+    def save_bytes(self) -> bytes: ...
+
     #####################################################################
     #                    ALL SUBSEQUENT METHODS ARE                     #
     #              EQUIVALENT TO THE CORRESPONDING METHODS              #
     #                     OF THE BUILT-IN SET TYPE                      #
     #####################################################################
 
     def add(self, obj: Any, /) -> None: ...
```

### Comparing `rbloom-1.4.5/src/lib.rs` & `rbloom-1.5.0/src/lib.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 use bitline::BitLine;
 use pyo3::exceptions::{PyTypeError, PyValueError};
 use pyo3::types::PyType;
-use pyo3::{basic::CompareOp, prelude::*, types::PyTuple};
+use pyo3::{basic::CompareOp, prelude::*, types::PyBytes, types::PyTuple};
 use std::fs::File;
 use std::io::{Read, Write};
 use std::mem;
 
 #[pyclass(module = "rbloom")]
 #[derive(Clone)]
 struct Bloom {
@@ -274,26 +274,68 @@
         Ok(Bloom {
             filter,
             k,
             hash_func,
         })
     }
 
+    /// Load from a bytes(), see "Persistence" section in the README
+    #[classmethod]
+    fn load_bytes(_cls: &PyType, bytes: &[u8], hash_func: &PyAny) -> PyResult<Bloom> {
+        // check that the hash_func is callable
+        if !hash_func.is_callable() {
+            return Err(PyTypeError::new_err("hash_func must be callable"));
+        }
+        // check that the hash_func isn't the built-in hash function
+        if hash_func.is(get_builtin_hash_func(hash_func.py())?) {
+            return Err(PyValueError::new_err(
+                "Cannot load a bloom filter that uses the built-in hash function",
+            ));
+        }
+        let hash_func = Some(hash_func.to_object(hash_func.py()));
+
+        let k_bytes: [u8; mem::size_of::<u64>()] = bytes[0..mem::size_of::<u64>()]
+            .try_into()
+            .expect("slice with incorrect length");
+        let k = u64::from_le_bytes(k_bytes);
+
+        let filter = BitLine::load_bytes(&bytes[mem::size_of::<u64>()..])?;
+
+        Ok(Bloom {
+            filter,
+            k,
+            hash_func,
+        })
+    }
+
     /// Save to a file, see "Persistence" section in the README
     fn save(&self, filepath: &str) -> PyResult<()> {
         if self.hash_func.is_none() {
             return Err(PyValueError::new_err(
                 "Cannot save a bloom filter that uses the built-in hash function",
             ));
         }
         let mut file = File::create(filepath)?;
         file.write_all(&self.k.to_le_bytes())?;
         self.filter.save(&mut file)?;
         Ok(())
     }
+
+    /// Save to a byte(), see "Persistence" section in the README
+    fn save_bytes(&self, py: Python<'_>) -> PyResult<PyObject> {
+        if self.hash_func.is_none() {
+            return Err(PyValueError::new_err(
+                "Cannot save a bloom filter that uses the built-in hash function",
+            ));
+        }
+
+        let serialized: Vec<u8> = [&self.k.to_le_bytes(), self.filter.bits() as &[u8]].concat();
+
+        Ok(PyBytes::new(py, &serialized).into())
+    }
 }
 
 // Non-python methods
 impl Bloom {
     fn hash_fn_clone(&self, py: Python<'_>) -> Option<PyObject> {
         self.hash_func.as_ref().map(|f| f.clone_ref(py))
     }
@@ -414,19 +456,32 @@
             let mut bits = Vec::new();
             file.read_to_end(&mut bits)?;
             Ok(Self {
                 bits: bits.into_boxed_slice(),
             })
         }
 
+        /// Given the provided [u8]
+        /// returns a BitLine containing the data.
+        pub fn load_bytes(bytes: &[u8]) -> PyResult<Self> {
+            let bits = bytes.to_vec();
+            Ok(Self {
+                bits: bits.into_boxed_slice(),
+            })
+        }
+
         /// Writes the BitLine to the given file from the current position.
         pub fn save(&self, file: &mut File) -> PyResult<()> {
             file.write_all(&self.bits)?;
             Ok(())
         }
+
+        pub fn bits(&self) -> &[u8] {
+            &self.bits
+        }
     }
 
     fn all_pairs(lhs: &BitLine, rhs: &BitLine, mut f: impl FnMut(u8, u8) -> bool) -> bool {
         lhs.bits
             .iter()
             .zip(rhs.bits.iter())
             .all(move |(&lhs, &rhs)| f(lhs, rhs))
```

### Comparing `rbloom-1.4.5/tests/api_test.py` & `rbloom-1.5.0/tests/api_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,14 +83,20 @@
             bloom.save(filename)
             bloom2 = Bloom.load(filename, bloom.hash_func)
             assert bloom == bloom2
         finally:
             # remove the file
             os.remove(filename)
 
+        # TEST bytes PERSISTENCE
+        bloom_bytes = bloom.save_bytes()
+        assert type(bloom_bytes) == bytes
+        bloom3 = Bloom.load_bytes(bloom_bytes, bloom.hash_func)
+        assert bloom == bloom3
+
 
 def sha_based(obj):
     h = sha256(dumps(obj)).digest()
     return int.from_bytes(h[:16], "big") - 2**127
 
 
 def api_suite():
```

### Comparing `rbloom-1.4.5/Cargo.lock` & `rbloom-1.5.0/Cargo.lock`

 * *Files 22% similar despite different names*

```diff
@@ -17,30 +17,36 @@
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
+name = "heck"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
+
+[[package]]
 name = "indoc"
-version = "1.0.9"
+version = "2.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
+checksum = "1e186cfbae8084e513daff4240b4797e342f988cecda4fb6c939150f96315fd8"
 
 [[package]]
 name = "libc"
-version = "0.2.146"
+version = "0.2.152"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
+checksum = "13e3bf6590cbc649f4d1a3eefc9d5d6eb746f5200ffb04e5e142700b8faa56e7"
 
 [[package]]
 name = "lock_api"
-version = "0.4.10"
+version = "0.4.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
+checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "memoffset"
@@ -49,225 +55,226 @@
 checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.18.0"
+version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
+checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.8"
+version = "0.9.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
+checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-targets",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.60"
+version = "1.0.76"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
+checksum = "95fc56cda0b5c3325f5fbbd7ff9fda9e02bb00bb3dac51252d2f1bfa1cb8cc8c"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.19.0"
+version = "0.20.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cffef52f74ec3b1a1baf295d9b8fcc3070327aefc39a6d00656b13c1d0b8885c"
+checksum = "9a89dc7a5850d0e983be1ec2a463a171d20990487c3cfcd68b5363f1ee3d6fe0"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.19.0"
+version = "0.20.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "713eccf888fb05f1a96eb78c0dbc51907fee42b3377272dc902eb38985f418d5"
+checksum = "07426f0d8fe5a601f26293f300afd1a7b1ed5e78b2a705870c5f30893c5163be"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.19.0"
+version = "0.20.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b2ecbdcfb01cbbf56e179ce969a048fd7305a66d4cdf3303e0da09d69afe4c3"
+checksum = "dbb7dec17e17766b46bca4f1a4215a85006b4c2ecde122076c562dd058da6cf1"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.19.0"
+version = "0.20.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b78fdc0899f2ea781c463679b20cb08af9247febc8d052de941951024cd8aea0"
+checksum = "05f738b4e40d50b5711957f142878cfa0f28e054aa0ebdfc3fd137a843f74ed3"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.19.0"
+version = "0.20.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "60da7b84f1227c3e2fe7593505de274dcf4c8928b4e0a1c23d551a14e4e80a0f"
+checksum = "0fc910d4851847827daf9d6cdd4a823fbdaab5b8818325c5e97a86da79e8881f"
 dependencies = [
+ "heck",
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.28"
+version = "1.0.35"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
+checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rbloom"
-version = "1.4.5"
+version = "1.5.0"
 dependencies = [
  "pyo3",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.3.5"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
+checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "scopeguard"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
+checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "smallvec"
-version = "1.10.0"
+version = "1.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+checksum = "e6ecd384b10a64542d77071bd64bd7b231f4ed5940fba55e98c3de13824cf3d7"
 
 [[package]]
 name = "syn"
-version = "1.0.109"
+version = "2.0.48"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
+checksum = "0f3531638e407dfc0814761abb7c00a5b54992b849452a0646b7f65c9f770f3f"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.7"
+version = "0.12.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
+checksum = "69758bda2e78f098e4ccb393021a0963bb3442eac05f135c30f61b7370bbafae"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.9"
+version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
+checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
 name = "unindent"
-version = "0.1.11"
+version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
+checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
 name = "windows-targets"
-version = "0.48.0"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
+checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.48.0"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
+checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.48.0"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
+checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.48.0"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
+checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.48.0"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
+checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.48.0"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
+checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.48.0"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
+checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.48.0"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
+checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
```

### Comparing `rbloom-1.4.5/PKG-INFO` & `rbloom-1.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rbloom
-Version: 1.4.5
+Version: 1.5.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Highly optimized Bloom filter that mimics the Python set API, written in Rust
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
@@ -161,18 +161,21 @@
     def hash_func(self) -> Callable[[Any], int]   # retrieve the hash_func
                                                   # given to __init__
 
     @property
     def approx_items(self) -> float    # estimated number of items in
                                        # the filter
 
+    # see section "Persistence" for more information on these four methods
     @classmethod
-    def load(cls, filepath: str, hash_func) -> Bloom      # see "Persistence"
-
-    def save(self, filepath: str)                 # see section "Persistence"
+    def load(cls, filepath: str, hash_func) -> Bloom
+    def save(self, filepath: str)
+    @classmethod
+    def load_bytes(cls, data: bytes, hash_func) -> Bloom
+    def save_bytes(self) -> bytes
 
     #####################################################################
     #                    ALL SUBSEQUENT METHODS ARE                     #
     #              EQUIVALENT TO THE CORRESPONDING METHODS              #
     #                     OF THE BUILT-IN SET TYPE                      #
     #####################################################################
 
@@ -247,30 +250,40 @@
 you from shooting yourself in the foot.
 
 Also note that using a custom hash will incur a performance penalty over
 using the built-in hash.
 
 ## Persistence
 
-The `save` and `load` methods allow you to save and load filters to and
-from disk. However, as the built-in hash function's salt changes between
-invocations of Python, they only work on filters with custom hash
-functions. Note that it is your responsibility to ensure that the hash
-function you supply to `load` is the same as the one originally used by
-the filter you're loading!
+The `save` and `load` methods, along with their byte-oriented counterparts
+`save_bytes` and `load_bytes`, allow you to save and load filters to and
+from disk/Python `bytes` objects. However, as the built-in hash function's
+salt changes between invocations of Python, they only work on filters with
+custom hash functions. Note that it is your responsibility to ensure that
+the hash function you supply to the loading functions is the same as the
+one originally used by the filter you're loading!
 
 ```python
 bf = Bloom(10_000, 0.01, some_hash_func)
 bf.add("hello")
 bf.add("world")
 
+# saving to a file
 bf.save("bf.bloom")
 
+# loading from a file
 loaded_bf = Bloom.load("bf.bloom", some_hash_func)
 assert loaded_bf == bf
+
+# saving to bytes
+bf_bytes = bf.save_bytes()
+
+# loading from bytes
+loaded_bf_from_bytes = Bloom.load_bytes(bf_bytes, some_hash_func)
+assert loaded_bf_from_bytes == bf
 ```
 
 The size of the file is `bf.size_in_bits / 8 + 8` bytes.
 
 ---
 
 **Statement of attribution:** Bloom filters were originally proposed in
```

