# Comparing `tmp/lvm_read-1.21.tar.gz` & `tmp/lvm_read-1.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lvm_read-1.21.tar", last modified: Sat Jul  1 05:22:08 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `lvm_read-1.21.tar` & `lvm_read-1.23.tar`

### file list

```diff
@@ -1,12 +1,6 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 05:22:08.727992 lvm_read-1.21/
--rw-rw-rw-   0        0        0     1091 2023-07-01 04:57:49.000000 lvm_read-1.21/LICENSE
--rw-rw-rw-   0        0        0      520 2023-07-01 05:22:08.727992 lvm_read-1.21/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-01 05:22:08.727992 lvm_read-1.21/lvm_read.egg-info/
--rw-rw-rw-   0        0        0      520 2023-07-01 05:22:08.000000 lvm_read-1.21/lvm_read.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      187 2023-07-01 05:22:08.000000 lvm_read-1.21/lvm_read.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 05:22:08.000000 lvm_read-1.21/lvm_read.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-01 05:22:08.000000 lvm_read-1.21/lvm_read.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-01 05:22:08.000000 lvm_read-1.21/lvm_read.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6816 2023-07-01 05:13:12.000000 lvm_read-1.21/lvm_read.py
--rw-rw-rw-   0        0        0       42 2023-07-01 05:22:08.727992 lvm_read-1.21/setup.cfg
--rw-rw-rw-   0        0        0      724 2023-07-01 05:21:06.000000 lvm_read-1.21/setup.py
+-rw-r--r--   0        0        0     7034 2020-02-02 00:00:00.000000 lvm_read-1.23/lvm_read.py
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 lvm_read-1.23/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 lvm_read-1.23/LICENSE
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 lvm_read-1.23/pyproject.toml
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 lvm_read-1.23/readme.rst
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 lvm_read-1.23/PKG-INFO
```

### Comparing `lvm_read-1.21/LICENSE` & `lvm_read-1.23/LICENSE`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2018 - 2023 Ladisk
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2018 - 2023 Ladisk
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

