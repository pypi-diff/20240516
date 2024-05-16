# Comparing `tmp/skia_python-87.5-cp39-cp39-win_amd64.whl.zip` & `tmp/skia_python-87.6-cp310-cp310-macosx_10_9_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,9 @@
-Zip file size: 4373511 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat 11247616 b- defN 22-Nov-07 14:49 skia.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     1551 b- defN 22-Nov-07 14:49 skia_python-87.5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2891 b- defN 22-Nov-07 14:49 skia_python-87.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 22-Nov-07 14:49 skia_python-87.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 22-Nov-07 14:49 skia_python-87.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      485 b- defN 22-Nov-07 14:49 skia_python-87.5.dist-info/RECORD
-6 files, 11252648 bytes uncompressed, 4372639 bytes compressed:  61.1%
+Zip file size: 10303379 bytes, number of entries: 7
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 18:47 skia_python-87.6.dist-info/
+-rwxr-xr-x  2.0 unx 32443296 b- defN 24-May-16 18:47 skia.cpython-310-darwin.so
+-rw-rw-r--  2.0 unx      494 b- defN 24-May-16 18:47 skia_python-87.6.dist-info/RECORD
+-rw-r--r--  2.0 unx     1522 b- defN 24-May-16 18:47 skia_python-87.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx      111 b- defN 24-May-16 18:47 skia_python-87.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-May-16 18:47 skia_python-87.6.dist-info/top_level.txt
+-rw-r--r--  2.0 unx     2918 b- defN 24-May-16 18:47 skia_python-87.6.dist-info/METADATA
+7 files, 32448346 bytes uncompressed, 10302371 bytes compressed:  68.3%
```

## zipnote {}

```diff
@@ -1,19 +1,22 @@
-Filename: skia.cp39-win_amd64.pyd
+Filename: skia_python-87.6.dist-info/
 Comment: 
 
-Filename: skia_python-87.5.dist-info/LICENSE
+Filename: skia.cpython-310-darwin.so
 Comment: 
 
-Filename: skia_python-87.5.dist-info/METADATA
+Filename: skia_python-87.6.dist-info/RECORD
 Comment: 
 
-Filename: skia_python-87.5.dist-info/WHEEL
+Filename: skia_python-87.6.dist-info/LICENSE
 Comment: 
 
-Filename: skia_python-87.5.dist-info/top_level.txt
+Filename: skia_python-87.6.dist-info/WHEEL
 Comment: 
 
-Filename: skia_python-87.5.dist-info/RECORD
+Filename: skia_python-87.6.dist-info/top_level.txt
+Comment: 
+
+Filename: skia_python-87.6.dist-info/METADATA
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## Comparing `skia_python-87.5.dist-info/LICENSE` & `skia_python-87.6.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-BSD 3-Clause License
-
-Copyright (c) 2020, Kota Yamaguchi
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its
-   contributors may be used to endorse or promote products derived from
-   this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+BSD 3-Clause License
+
+Copyright (c) 2020, Kota Yamaguchi
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

## Comparing `skia_python-87.5.dist-info/METADATA` & `skia_python-87.6.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skia-python
-Version: 87.5
+Version: 87.6
 Summary: Skia python binding
 Home-page: https://github.com/kyamagu/skia-python
 Author: Kota Yamaguchi
 Author-email: KotaYamaguchi1984@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
-Requires-Dist: pybind11 (>=2.6)
+Requires-Dist: pybind11 >=2.6
 
 # Skia python binding
 
 ![Build and test](https://github.com/kyamagu/skia-python/workflows/Build%20and%20test/badge.svg)
 [![PyPI version](https://badge.fury.io/py/skia-python.svg)](https://badge.fury.io/py/skia-python)
 
 Python binding to [Skia Graphics Library](https://skia.org/).
@@ -37,15 +37,15 @@
 
 Binary package is available on PyPI:
 
 ```bash
 pip install skia-python
 ```
 
-Supported platforms:
+Supported platforms: Python 3.8-3.12 (CPython) on
 
 - Linux x86_64, aarch64
 - macOS x86_64, arm64
 - Windows x86_64
 
 For Linux platforms, there must be OpenGL and fontconfig installed:
```

