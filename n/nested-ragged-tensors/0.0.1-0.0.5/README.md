# Comparing `tmp/nested_ragged_tensors-0.0.1.tar.gz` & `tmp/nested_ragged_tensors-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nested_ragged_tensors-0.0.1.tar", last modified: Mon Jan 22 02:03:40 2024, max compression
+gzip compressed data, was "nested_ragged_tensors-0.0.5.tar", last modified: Thu May 16 12:44:29 2024, max compression
```

## Comparing `nested_ragged_tensors-0.0.1.tar` & `nested_ragged_tensors-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 mmd       (1000) mmd       (1000)        0 2024-01-22 02:03:40.662811 nested_ragged_tensors-0.0.1/
--rw-rw-r--   0 mmd       (1000) mmd       (1000)     1074 2023-12-16 16:57:29.000000 nested_ragged_tensors-0.0.1/LICENSE
--rw-r--r--   0 mmd       (1000) mmd       (1000)    16294 2024-01-22 02:03:40.662811 nested_ragged_tensors-0.0.1/PKG-INFO
--rw-rw-r--   0 mmd       (1000) mmd       (1000)    15231 2024-01-22 02:00:24.000000 nested_ragged_tensors-0.0.1/README.md
--rw-rw-r--   0 mmd       (1000) mmd       (1000)      894 2024-01-20 18:38:06.000000 nested_ragged_tensors-0.0.1/pyproject.toml
--rw-rw-r--   0 mmd       (1000) mmd       (1000)       38 2024-01-22 02:03:40.662811 nested_ragged_tensors-0.0.1/setup.cfg
-drwxrwxr-x   0 mmd       (1000) mmd       (1000)        0 2024-01-22 02:03:40.662811 nested_ragged_tensors-0.0.1/src/
-drwxrwxr-x   0 mmd       (1000) mmd       (1000)        0 2024-01-22 02:03:40.662811 nested_ragged_tensors-0.0.1/src/nested_ragged_tensors/
--rw-rw-r--   0 mmd       (1000) mmd       (1000)        0 2023-12-20 20:50:36.000000 nested_ragged_tensors-0.0.1/src/nested_ragged_tensors/__init__.py
--rw-rw-r--   0 mmd       (1000) mmd       (1000)    30337 2024-01-20 18:33:35.000000 nested_ragged_tensors-0.0.1/src/nested_ragged_tensors/ragged_numpy.py
-drwxrwxr-x   0 mmd       (1000) mmd       (1000)        0 2024-01-22 02:03:40.662811 nested_ragged_tensors-0.0.1/src/nested_ragged_tensors.egg-info/
--rw-r--r--   0 mmd       (1000) mmd       (1000)    16294 2024-01-22 02:03:40.000000 nested_ragged_tensors-0.0.1/src/nested_ragged_tensors.egg-info/PKG-INFO
--rw-rw-r--   0 mmd       (1000) mmd       (1000)      356 2024-01-22 02:03:40.000000 nested_ragged_tensors-0.0.1/src/nested_ragged_tensors.egg-info/SOURCES.txt
--rw-rw-r--   0 mmd       (1000) mmd       (1000)        1 2024-01-22 02:03:40.000000 nested_ragged_tensors-0.0.1/src/nested_ragged_tensors.egg-info/dependency_links.txt
--rw-rw-r--   0 mmd       (1000) mmd       (1000)      105 2024-01-22 02:03:40.000000 nested_ragged_tensors-0.0.1/src/nested_ragged_tensors.egg-info/requires.txt
--rw-rw-r--   0 mmd       (1000) mmd       (1000)       22 2024-01-22 02:03:40.000000 nested_ragged_tensors-0.0.1/src/nested_ragged_tensors.egg-info/top_level.txt
+drwxrwxr-x   0 mmd       (1000) mmd       (1000)        0 2024-05-16 12:44:29.882503 nested_ragged_tensors-0.0.5/
+-rw-rw-r--   0 mmd       (1000) mmd       (1000)     1074 2023-12-16 16:57:29.000000 nested_ragged_tensors-0.0.5/LICENSE
+-rw-r--r--   0 mmd       (1000) mmd       (1000)    16551 2024-05-16 12:44:29.882503 nested_ragged_tensors-0.0.5/PKG-INFO
+-rw-rw-r--   0 mmd       (1000) mmd       (1000)    15488 2024-05-16 12:44:05.000000 nested_ragged_tensors-0.0.5/README.md
+-rw-rw-r--   0 mmd       (1000) mmd       (1000)      894 2024-05-16 12:42:39.000000 nested_ragged_tensors-0.0.5/pyproject.toml
+-rw-rw-r--   0 mmd       (1000) mmd       (1000)       38 2024-05-16 12:44:29.882503 nested_ragged_tensors-0.0.5/setup.cfg
+drwxrwxr-x   0 mmd       (1000) mmd       (1000)        0 2024-05-16 12:44:29.882503 nested_ragged_tensors-0.0.5/src/
+drwxrwxr-x   0 mmd       (1000) mmd       (1000)        0 2024-05-16 12:44:29.882503 nested_ragged_tensors-0.0.5/src/nested_ragged_tensors/
+-rw-rw-r--   0 mmd       (1000) mmd       (1000)        0 2023-12-20 20:50:36.000000 nested_ragged_tensors-0.0.5/src/nested_ragged_tensors/__init__.py
+-rw-rw-r--   0 mmd       (1000) mmd       (1000)    37277 2024-05-04 20:43:51.000000 nested_ragged_tensors-0.0.5/src/nested_ragged_tensors/ragged_numpy.py
+drwxrwxr-x   0 mmd       (1000) mmd       (1000)        0 2024-05-16 12:44:29.882503 nested_ragged_tensors-0.0.5/src/nested_ragged_tensors.egg-info/
+-rw-r--r--   0 mmd       (1000) mmd       (1000)    16551 2024-05-16 12:44:29.000000 nested_ragged_tensors-0.0.5/src/nested_ragged_tensors.egg-info/PKG-INFO
+-rw-rw-r--   0 mmd       (1000) mmd       (1000)      356 2024-05-16 12:44:29.000000 nested_ragged_tensors-0.0.5/src/nested_ragged_tensors.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmd       (1000) mmd       (1000)        1 2024-05-16 12:44:29.000000 nested_ragged_tensors-0.0.5/src/nested_ragged_tensors.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmd       (1000) mmd       (1000)      105 2024-05-16 12:44:29.000000 nested_ragged_tensors-0.0.5/src/nested_ragged_tensors.egg-info/requires.txt
+-rw-rw-r--   0 mmd       (1000) mmd       (1000)       22 2024-05-16 12:44:29.000000 nested_ragged_tensors-0.0.5/src/nested_ragged_tensors.egg-info/top_level.txt
```

### Comparing `nested_ragged_tensors-0.0.1/LICENSE` & `nested_ragged_tensors-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nested_ragged_tensors-0.0.1/PKG-INFO` & `nested_ragged_tensors-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nested_ragged_tensors
-Version: 0.0.1
+Version: 0.0.5
 Summary: Utilities for efficiently working with, saving, and loading, collections of connected nested ragged tensors in PyTorch
 Author-email: Matthew McDermott <mattmcdermott8@gmail.com>
 Project-URL: Homepage, https://github.com/mmcdermott/nested_ragged_tensors
 Project-URL: Issues, https://github.com/mmcdermott/nested_ragged_tensors/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,40 +22,42 @@
 Requires-Dist: torch; extra == "tests"
 Requires-Dist: rootutils; extra == "tests"
 Requires-Dist: hydra-core; extra == "tests"
 Requires-Dist: humanize; extra == "tests"
 
 # Nested Ragged Tensors
 
+Install with `pip install nested-ragged-tensors`
+
 This package contains utilities for efficiently working with, saving, and loading, collections of connected
 nested ragged tensors in numpy. For example:
 
 ```python
 >>> from nested_ragged_tensors.ragged_numpy import *
 >>> import tempfile
 >>> J = JointNestedRaggedTensorDict({
 ...     "T":   [[1,           2,        3       ], [4,   5          ], [6,  7]],
 ...     "id":  [[[1, 2,   3], [3,   4], [1, 2  ]], [[3], [3,   2, 2]], [[], [8,  9]]],
 ...     "val": [[[1, 0.2, 0], [3.1, 0], [1, 2.2]], [[3], [3.3, 2, 0]], [[], [1., 0]]],
 ... }, schema={"T": int, "id": int, "val": float})
 >>> len(J)
 3
 >>> as_dense = J[1].to_dense()
->>> assert dense_dict.keys() == {'T', 'id', 'val', 'dim1/mask'}
+>>> assert as_dense.keys() == {'T', 'id', 'val', 'dim1/mask'}
 >>> as_dense['T']
 array([4, 5])
 >>> as_dense['id']
 array([[3, 0, 0],
        [3, 2, 2]])
 >>> as_dense['val']
 array([[3. , 0. , 0. ],
        [3.3, 2. , 0. ]])
 >>> as_dense['dim1/mask']
 array([[True, False, False],
-       [True,  True, False]])
+       [True,  True,  True]])
 >>> as_dense = J[2].to_dense()
 >>> as_dense['T']
 array([6, 7])
 >>> as_dense['id']
 array([[0, 0],
        [8, 9]])
 >>> as_dense['val']
@@ -171,14 +173,17 @@
         [3. , 0. , 0. ]]])
 ```
 
 Numpy was chosen as it proved to be significantly faster to work with than was PyTorch. I make no guarantees
 about the absence of better solutions for the driving problem here. I have not yet found any such better
 solutions, but that does not imply they do not exist.
 
+Tensors stored in this format on disk can also be partially loaded from disk using the `load_slice` method,
+which relies on Hugging Face `safetensors` partial loading capability internally and is quite fast.
+
 ## The Problem
 
 The problem this package solves is how to work with tensors that contain nested collections of data of
 different lengths that will eventually be padded to a dense shape. For example, suppose we are working with
 patient level data in medicine. There are 2 patients total and patient 1 has 3 clinic visits while patient 2
 has only 1 clinic visit. Patient 1's visits have 2, 4, and 1 diagnosis codes recorded, respectively, and
 patient 2's visit has 3 codes recorded. If we were to record these diagnostic codes in a dense tensor, with
```

### Comparing `nested_ragged_tensors-0.0.1/README.md` & `nested_ragged_tensors-0.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 # Nested Ragged Tensors
 
+Install with `pip install nested-ragged-tensors`
+
 This package contains utilities for efficiently working with, saving, and loading, collections of connected
 nested ragged tensors in numpy. For example:
 
 ```python
 >>> from nested_ragged_tensors.ragged_numpy import *
 >>> import tempfile
 >>> J = JointNestedRaggedTensorDict({
 ...     "T":   [[1,           2,        3       ], [4,   5          ], [6,  7]],
 ...     "id":  [[[1, 2,   3], [3,   4], [1, 2  ]], [[3], [3,   2, 2]], [[], [8,  9]]],
 ...     "val": [[[1, 0.2, 0], [3.1, 0], [1, 2.2]], [[3], [3.3, 2, 0]], [[], [1., 0]]],
 ... }, schema={"T": int, "id": int, "val": float})
 >>> len(J)
 3
 >>> as_dense = J[1].to_dense()
->>> assert dense_dict.keys() == {'T', 'id', 'val', 'dim1/mask'}
+>>> assert as_dense.keys() == {'T', 'id', 'val', 'dim1/mask'}
 >>> as_dense['T']
 array([4, 5])
 >>> as_dense['id']
 array([[3, 0, 0],
        [3, 2, 2]])
 >>> as_dense['val']
 array([[3. , 0. , 0. ],
        [3.3, 2. , 0. ]])
 >>> as_dense['dim1/mask']
 array([[True, False, False],
-       [True,  True, False]])
+       [True,  True,  True]])
 >>> as_dense = J[2].to_dense()
 >>> as_dense['T']
 array([6, 7])
 >>> as_dense['id']
 array([[0, 0],
        [8, 9]])
 >>> as_dense['val']
@@ -145,14 +147,17 @@
         [3. , 0. , 0. ]]])
 ```
 
 Numpy was chosen as it proved to be significantly faster to work with than was PyTorch. I make no guarantees
 about the absence of better solutions for the driving problem here. I have not yet found any such better
 solutions, but that does not imply they do not exist.
 
+Tensors stored in this format on disk can also be partially loaded from disk using the `load_slice` method,
+which relies on Hugging Face `safetensors` partial loading capability internally and is quite fast.
+
 ## The Problem
 
 The problem this package solves is how to work with tensors that contain nested collections of data of
 different lengths that will eventually be padded to a dense shape. For example, suppose we are working with
 patient level data in medicine. There are 2 patients total and patient 1 has 3 clinic visits while patient 2
 has only 1 clinic visit. Patient 1's visits have 2, 4, and 1 diagnosis codes recorded, respectively, and
 patient 2's visit has 3 codes recorded. If we were to record these diagnostic codes in a dense tensor, with
```

### Comparing `nested_ragged_tensors-0.0.1/pyproject.toml` & `nested_ragged_tensors-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nested_ragged_tensors"
-version = "0.0.1"
+version = "0.0.5"
 authors = [
   { name="Matthew McDermott", email="mattmcdermott8@gmail.com" },
 ]
 description = "Utilities for efficiently working with, saving, and loading, collections of connected nested ragged tensors in PyTorch"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `nested_ragged_tensors-0.0.1/src/nested_ragged_tensors/ragged_numpy.py` & `nested_ragged_tensors-0.0.5/src/nested_ragged_tensors/ragged_numpy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
 
 import itertools
+from collections import defaultdict
 from collections.abc import Sequence
 from pathlib import Path
 
 import numpy as np
+from safetensors import safe_open
 from safetensors.numpy import load_file, save_file
 
 NP_FLOAT_TYPES = (np.float16, np.float32, np.float64)
 NP_INT_TYPES = (np.int8, np.int16, np.int32, np.int64)
 NP_UINT_TYPES = (np.uint8, np.uint16, np.uint32, np.uint64)
 
 NUM_T = int | float
@@ -193,19 +195,20 @@
         """Returns the tensors with flat values."""
         return {k: v if isinstance(v, np.ndarray) else np.concatenate(v, 0) for k, v in self.tensors.items()}
 
     @classmethod
     def load(cls, fp: Path) -> JointNestedRaggedTensorDict:
         """Loads the tensors saved at the given filepath. Does not validate tensor structure.
 
+        Note ``load_slice`` for a more efficient alternative if you only want to access part of the tensor
+        dictionary.
+
         Args:
             The path from which to load
 
-        TODO(mmd): Look into using `safetensors.safe_open`
-
         Examples:
             >>> import tempfile
             >>> J = JointNestedRaggedTensorDict({
             ...     "T":   [[1,           2,        3       ], [4,   5          ]],
             ...     "id":  [[[1, 2,   3], [3,   4], [1, 2  ]], [[3], [3,   2, 2]]],
             ...     "val": [[[1, 0.2, 0], [3.1, 0], [1, 2.2]], [[3], [3.3, 2, 0]]],
             ... })
@@ -222,15 +225,15 @@
             ...         for i, (v1, v2) in enumerate(zip(J.tensors[k], J2.tensors[k])):
             ...             assert (v1 == v2).all(), f"Tensors at {k}[{i}] unequal!"
         """
         flat_vals_tensors = load_file(fp)
         tensors = {}
         schema = {}
         for k, v in flat_vals_tensors.items():
-            if k.endswith("/lengths") or k.endswith("/bounds"):
+            if cls._is_meta_key(k):
                 tensors[k] = v
             else:
                 schema[k] = v.dtype
                 dim_str = k.split("/")[0]
                 if dim_str == "dim0":
                     tensors[k] = v
                 else:
@@ -276,19 +279,44 @@
             >>> J = JointNestedRaggedTensorDict({
             ...     "T":   [[1,           2,        3       ], [4,   5          ]],
             ...     "id":  [[[1, 2,   3], [3,   4], [1, 2  ]], [[3], [3,   2, 2]]],
             ...     "val": [[[1, 0.2, 0], [3.1, 0], [1, 2.2]], [[3], [3.3, 2, 0]]],
             ... })
             >>> assert J.keys() == {'id', 'T', 'val'}
         """
-        return {
-            k.split("/")[1]
-            for k in self.tensors.keys()
-            if not (k.endswith("lengths") or k.endswith("bounds"))
-        }
+        return {k.split("/")[1] for k in self.tensors.keys() if not self._is_meta_key(k)}
+
+    @classmethod
+    def _is_meta_key(cls, k: str) -> bool:
+        """Returns `True` if and only if ``k`` is a meta-key, rather than a data-key.
+
+        Examples:
+            >>> JointNestedRaggedTensorDict._is_meta_key("dim1/T")
+            False
+            >>> JointNestedRaggedTensorDict._is_meta_key("dim1/lengths")
+            True
+            >>> JointNestedRaggedTensorDict._is_meta_key("dim1/bounds")
+            True
+            >>> JointNestedRaggedTensorDict._is_meta_key("dim1/mask")
+            True
+        """
+        return k.endswith("/lengths") or k.endswith("/bounds") or k.endswith("/mask")
+
+    @classmethod
+    def _get_dim_from_key_str(self, full_key_str: str) -> int:
+        """Gets the dimensionality associated with this key.
+
+        Examples:
+            >>> JointNestedRaggedTensorDict._get_dim_from_key_str("dim1/T")
+            1
+            >>> JointNestedRaggedTensorDict._get_dim_from_key_str("dim2/id")
+            2
+        """
+        dim_part, key_part = full_key_str.split("/")
+        return int(dim_part[3:])
 
     def _get_dim(self, key: str) -> int:
         """Gets the dimensionality associated with this key.
 
         Examples:
             >>> J = JointNestedRaggedTensorDict({
             ...     "T":   [[1,           2,        3       ], [4,   5          ]],
@@ -298,15 +326,15 @@
             >>> J._get_dim("T")
             1
             >>> J._get_dim("id")
             2
         """
         for k in self.tensors.keys():
             if k.endswith(f"/{key}"):
-                return int(k.split("/")[0][3:])
+                return self._get_dim_from_key_str(k)
 
         raise KeyError(f"Key {key} not found in {', '.join(self.tensors.keys())}")
 
     def keys_at_dim(self, dim: int) -> set[str]:
         """Returns the keys for tensors that are at that dimensionality.
 
         Examples:
@@ -750,7 +778,127 @@
                     )
 
                 for key in out_keys_at_dim[dim]:
                     out_tensors[f"dim{dim}/{key}"] = (
                         out_tensors[f"dim{dim}/{key}"] + T.tensors[f"dim{dim}/{key}"]
                     )
         return cls(out_tensors, pre_raggedified=True, schema=out_schema)
+
+    @classmethod
+    def load_slice(cls, fp: Path, idx: int | slice | np.ndarray) -> JointNestedRaggedTensorDict:
+        """Loads the specified slice of the tensors saved at the given filepath.
+
+        This method uses ``safetensors`` to fetch only the requested slice from the underlying file in an
+        efficient, optimized manner that significantly preserves the resources required to load the entire
+        file.
+
+        Args:
+            fp: The path from which to load
+            idx: The slice to read.
+
+        Returns
+            * If ``idx`` is an `int` or a `slice` object, this returns a `JointNestedRaggedTensorDict`
+              representing the tensors saved at ``fp`` as though they were sliced according to ``idx`` in the
+              first dimension. With an `int` index, the resulting tensors will have their dimensionality
+              reduced by one, and this cannot be called on a collection that already has some tensors that are
+              of dimensionality 1 in it.
+            * If ``idx`` is a numpy array of integers, this returns a `JointNestedRaggedTensorDict`
+              that consists of tensors saved at ``fp`` sliced at the integer indices in ``idx`` and
+              then re-stacked together. Dimensionality will not be reduced. This behavior is consistent with
+              how the tensors would be sliced under ``idx`` were they dense numpy arrays.
+
+        Examples:
+            >>> import tempfile
+            >>> J = JointNestedRaggedTensorDict({
+            ...     "T":   [[1,           2,        3       ], [4,   5          ]],
+            ...     "id":  [[[1, 2,   3], [3,   4], [1, 2  ]], [[3], [3,   2, 2]]],
+            ...     "val": [[[1, 0.2, 0], [3.1, 0], [1, 2.2]], [[3], [3.3, 2, 0]]],
+            ... })
+            >>> with tempfile.TemporaryDirectory() as dirpath:
+            ...     fp = Path(dirpath) / "tensors.pt"
+            ...     J.save(fp)
+            ...     J2 = JointNestedRaggedTensorDict.load_slice(fp, slice(None, 1))
+            >>> J = J[:1]
+            >>> assert J.keys() == J2.keys(), f"Keys unequal: {J.keys()} != {J2.keys()}"
+            >>> J_dense = J.to_dense()
+            >>> J2_dense = J2.to_dense()
+            >>> for k in J_dense.keys():
+            ...     assert (J_dense[k] == J2_dense[k]).all(), f"Tensors at {k} unequal!"
+            >>> J = JointNestedRaggedTensorDict({
+            ...     "T":   [[1,           2,        3       ], [4,   5          ]],
+            ...     "id":  [[[1, 2,   3], [3,   4], [1, 2  ]], [[3], [3,   2, 2]]],
+            ...     "val": [[[1, 0.2, 0], [3.1, 0], [1, 2.2]], [[3], [3.3, 2, 0]]],
+            ... })
+            >>> with tempfile.TemporaryDirectory() as dirpath:
+            ...     fp = Path(dirpath) / "tensors.pt"
+            ...     J.save(fp)
+            ...     J2 = JointNestedRaggedTensorDict.load_slice(fp, 1)
+            >>> J = J[1]
+            >>> assert J.keys() == J2.keys(), f"Keys unequal: {J.keys()} != {J2.keys()}"
+            >>> J_dense = J.to_dense()
+            >>> J2_dense = J2.to_dense()
+            >>> for k in J_dense.keys():
+            ...     assert (J_dense[k] == J2_dense[k]).all(), f"Tensors at {k} unequal!"
+        """
+
+        match idx:
+            case np.ndarray() as arr if arr.dtype in (NP_INT_TYPES + NP_UINT_TYPES) and arr.ndim == 1:
+                return cls.vstack([cls.load_slice(fp, int(i)) for i in arr])
+            case int() as i:
+                return cls.load_slice(fp, slice(i, i + 1))[0]
+            case slice() as S:
+                st_i = 0 if S.start is None else S.start
+                end_i = S.stop
+
+                if S.step not in (None, 1):
+                    raise ValueError("Only slices with step size of None or 1 are supported; got {S.step}")
+
+                tensors = {}
+                schema = {}
+                with safe_open(fp, framework="np") as f:
+                    keys_by_dim = defaultdict(list)
+
+                    for k in f.keys():
+                        if cls._is_meta_key(k):
+                            continue
+
+                        keys_by_dim[cls._get_dim_from_key_str(k)].append(k)
+
+                    max_n_dims = max(keys_by_dim.keys()) + 1
+
+                    for key in keys_by_dim[0]:
+                        v = f.get_slice(k)[st_i:end_i]
+                        schema[k] = v.dtype
+                        tensors[k] = v
+
+                    for dim in range(1, max_n_dims):
+                        try:
+                            tensors[f"dim{dim}/lengths"] = f.get_slice(f"dim{dim}/lengths")[st_i:end_i]
+                        except SystemError as e:
+                            raise ValueError(
+                                f"Error loading lengths for dim {dim} with st_i={st_i} and end_i={end_i}"
+                            ) from e
+
+                        if st_i == 0:
+                            offset = 0
+                            B = f.get_slice(f"dim{dim}/bounds")[st_i:end_i]
+                        else:
+                            B = f.get_slice(f"dim{dim}/bounds")[st_i - 1 : end_i]
+                            offset = B[0]
+                            B = B[1:] - offset
+
+                        vals_start = offset
+                        vals_end = B[-1] + offset
+
+                        tensors[f"dim{dim}/bounds"] = B
+
+                        for k in keys_by_dim[dim]:
+                            v = f.get_slice(k)[vals_start:vals_end]
+                            schema[k] = v.dtype
+                            tensors[k] = np.split(v, B[:-1])
+
+                        st_i = 0 if st_i == 0 else offset
+                        end_i = B[-1] + offset
+
+                return cls(tensors, schema=schema, pre_raggedified=True)
+            case _:
+                raise TypeError(f"{type(idx)} not supported for {cls.__name__}.load_slice")
```

### Comparing `nested_ragged_tensors-0.0.1/src/nested_ragged_tensors.egg-info/PKG-INFO` & `nested_ragged_tensors-0.0.5/src/nested_ragged_tensors.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nested_ragged_tensors
-Version: 0.0.1
+Version: 0.0.5
 Summary: Utilities for efficiently working with, saving, and loading, collections of connected nested ragged tensors in PyTorch
 Author-email: Matthew McDermott <mattmcdermott8@gmail.com>
 Project-URL: Homepage, https://github.com/mmcdermott/nested_ragged_tensors
 Project-URL: Issues, https://github.com/mmcdermott/nested_ragged_tensors/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,40 +22,42 @@
 Requires-Dist: torch; extra == "tests"
 Requires-Dist: rootutils; extra == "tests"
 Requires-Dist: hydra-core; extra == "tests"
 Requires-Dist: humanize; extra == "tests"
 
 # Nested Ragged Tensors
 
+Install with `pip install nested-ragged-tensors`
+
 This package contains utilities for efficiently working with, saving, and loading, collections of connected
 nested ragged tensors in numpy. For example:
 
 ```python
 >>> from nested_ragged_tensors.ragged_numpy import *
 >>> import tempfile
 >>> J = JointNestedRaggedTensorDict({
 ...     "T":   [[1,           2,        3       ], [4,   5          ], [6,  7]],
 ...     "id":  [[[1, 2,   3], [3,   4], [1, 2  ]], [[3], [3,   2, 2]], [[], [8,  9]]],
 ...     "val": [[[1, 0.2, 0], [3.1, 0], [1, 2.2]], [[3], [3.3, 2, 0]], [[], [1., 0]]],
 ... }, schema={"T": int, "id": int, "val": float})
 >>> len(J)
 3
 >>> as_dense = J[1].to_dense()
->>> assert dense_dict.keys() == {'T', 'id', 'val', 'dim1/mask'}
+>>> assert as_dense.keys() == {'T', 'id', 'val', 'dim1/mask'}
 >>> as_dense['T']
 array([4, 5])
 >>> as_dense['id']
 array([[3, 0, 0],
        [3, 2, 2]])
 >>> as_dense['val']
 array([[3. , 0. , 0. ],
        [3.3, 2. , 0. ]])
 >>> as_dense['dim1/mask']
 array([[True, False, False],
-       [True,  True, False]])
+       [True,  True,  True]])
 >>> as_dense = J[2].to_dense()
 >>> as_dense['T']
 array([6, 7])
 >>> as_dense['id']
 array([[0, 0],
        [8, 9]])
 >>> as_dense['val']
@@ -171,14 +173,17 @@
         [3. , 0. , 0. ]]])
 ```
 
 Numpy was chosen as it proved to be significantly faster to work with than was PyTorch. I make no guarantees
 about the absence of better solutions for the driving problem here. I have not yet found any such better
 solutions, but that does not imply they do not exist.
 
+Tensors stored in this format on disk can also be partially loaded from disk using the `load_slice` method,
+which relies on Hugging Face `safetensors` partial loading capability internally and is quite fast.
+
 ## The Problem
 
 The problem this package solves is how to work with tensors that contain nested collections of data of
 different lengths that will eventually be padded to a dense shape. For example, suppose we are working with
 patient level data in medicine. There are 2 patients total and patient 1 has 3 clinic visits while patient 2
 has only 1 clinic visit. Patient 1's visits have 2, 4, and 1 diagnosis codes recorded, respectively, and
 patient 2's visit has 3 codes recorded. If we were to record these diagnostic codes in a dense tensor, with
```

