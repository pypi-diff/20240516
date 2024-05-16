# Comparing `tmp/pyrage-stubs-1.1.0.tar.gz` & `tmp/pyrage_stubs-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrage-stubs-1.1.0.tar", last modified: Tue Aug  1 03:36:29 2023, max compression
+gzip compressed data, was "pyrage_stubs-1.1.1.tar", last modified: Thu May 16 20:17:58 2024, max compression
```

## Comparing `pyrage-stubs-1.1.0.tar` & `pyrage_stubs-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:36:29.067287 pyrage-stubs-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-08-01 03:35:59.000000 pyrage-stubs-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-01 03:36:29.063287 pyrage-stubs-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-01 03:35:59.000000 pyrage-stubs-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-08-01 03:35:59.000000 pyrage-stubs-1.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:36:29.063287 pyrage-stubs-1.1.0/pyrage-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-01 03:35:59.000000 pyrage-stubs-1.1.0/pyrage-stubs/passphrase.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-01 03:35:59.000000 pyrage-stubs-1.1.0/pyrage-stubs/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-01 03:35:59.000000 pyrage-stubs-1.1.0/pyrage-stubs/x25519.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:36:29.063287 pyrage-stubs-1.1.0/pyrage_stubs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-01 03:36:29.000000 pyrage-stubs-1.1.0/pyrage_stubs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-08-01 03:36:29.000000 pyrage-stubs-1.1.0/pyrage_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 03:36:29.000000 pyrage-stubs-1.1.0/pyrage_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-01 03:36:29.000000 pyrage-stubs-1.1.0/pyrage_stubs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-01 03:36:29.000000 pyrage-stubs-1.1.0/pyrage_stubs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 03:36:29.067287 pyrage-stubs-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-08-01 03:35:59.000000 pyrage-stubs-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:17:58.955646 pyrage_stubs-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-16 20:17:42.000000 pyrage_stubs-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-16 20:17:58.955646 pyrage_stubs-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-16 20:17:42.000000 pyrage_stubs-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-16 20:17:42.000000 pyrage_stubs-1.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:17:58.955646 pyrage_stubs-1.1.1/pyrage-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-16 20:17:42.000000 pyrage_stubs-1.1.1/pyrage-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-16 20:17:42.000000 pyrage_stubs-1.1.1/pyrage-stubs/passphrase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-16 20:17:42.000000 pyrage_stubs-1.1.1/pyrage-stubs/plugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-16 20:17:42.000000 pyrage_stubs-1.1.1/pyrage-stubs/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-16 20:17:42.000000 pyrage_stubs-1.1.1/pyrage-stubs/x25519.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:17:58.955646 pyrage_stubs-1.1.1/pyrage_stubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-16 20:17:58.000000 pyrage_stubs-1.1.1/pyrage_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-16 20:17:58.000000 pyrage_stubs-1.1.1/pyrage_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 20:17:58.000000 pyrage_stubs-1.1.1/pyrage_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-16 20:17:58.000000 pyrage_stubs-1.1.1/pyrage_stubs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 20:17:58.000000 pyrage_stubs-1.1.1/pyrage_stubs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 20:17:58.955646 pyrage_stubs-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-16 20:17:42.000000 pyrage_stubs-1.1.1/setup.py
```

### Comparing `pyrage-stubs-1.1.0/LICENSE` & `pyrage_stubs-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrage-stubs-1.1.0/PKG-INFO` & `pyrage_stubs-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrage-stubs
-Version: 1.1.0
+Version: 1.1.1
 Summary: A PEP 561 stub package for pyrage's types
 Author-email: William Woodruff <william@yossarian.net>
 License: The MIT License (MIT)
         
         Copyright (c) 2022 William Woodruff <william @ yossarian.net>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,22 +24,22 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
         THE SOFTWARE.
         
 Project-URL: Homepage, https://pypi.org/project/pyrage/
 Project-URL: Issues, https://github.com/woodruffw/pyrage/issues
 Project-URL: Source, https://github.com/woodruffw/pyrage/tree/main/pyrage-stubs
-Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Security :: Cryptography
 Classifier: Typing :: Stubs Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pyrage<2.0,>=1.0.0
 
 pyrage-stubs
 ============
 
 This is a [PEP 561](https://peps.python.org/pep-0561/)-compatible stubs
 package for [`pyrage`](https://github.com/woodruffw/pyrage).
```

### Comparing `pyrage-stubs-1.1.0/pyproject.toml` & `pyrage_stubs-1.1.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyrage-stubs"
-version = "1.1.0"
+version = "1.1.1"
 description = "A PEP 561 stub package for pyrage's types"
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [{ name = "William Woodruff", email = "william@yossarian.net" }]
 classifiers = [
-  "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Topic :: Security :: Cryptography",
   "Typing :: Stubs Only",
 ]
 dependencies = ["pyrage>=1.0.0,<2.0"]
-requires-python = ">= 3.7"
+requires-python = ">= 3.8"
 
 [project.urls]
 Homepage = "https://pypi.org/project/pyrage/"
 Issues = "https://github.com/woodruffw/pyrage/issues"
 Source = "https://github.com/woodruffw/pyrage/tree/main/pyrage-stubs"
+
+[tool.setuptools.package-data]
+"*" = ["*.pyi"]
```

### Comparing `pyrage-stubs-1.1.0/pyrage_stubs.egg-info/PKG-INFO` & `pyrage_stubs-1.1.1/pyrage_stubs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrage-stubs
-Version: 1.1.0
+Version: 1.1.1
 Summary: A PEP 561 stub package for pyrage's types
 Author-email: William Woodruff <william@yossarian.net>
 License: The MIT License (MIT)
         
         Copyright (c) 2022 William Woodruff <william @ yossarian.net>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,22 +24,22 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
         THE SOFTWARE.
         
 Project-URL: Homepage, https://pypi.org/project/pyrage/
 Project-URL: Issues, https://github.com/woodruffw/pyrage/issues
 Project-URL: Source, https://github.com/woodruffw/pyrage/tree/main/pyrage-stubs
-Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Security :: Cryptography
 Classifier: Typing :: Stubs Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pyrage<2.0,>=1.0.0
 
 pyrage-stubs
 ============
 
 This is a [PEP 561](https://peps.python.org/pep-0561/)-compatible stubs
 package for [`pyrage`](https://github.com/woodruffw/pyrage).
```

