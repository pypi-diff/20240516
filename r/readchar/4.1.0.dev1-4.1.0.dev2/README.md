# Comparing `tmp/readchar-4.1.0.dev1.tar.gz` & `tmp/readchar-4.1.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readchar-4.1.0.dev1.tar", last modified: Wed Nov 16 09:52:21 2022, max compression
+gzip compressed data, was "readchar-4.1.0.dev2.tar", last modified: Thu May 16 15:54:01 2024, max compression
```

## Comparing `readchar-4.1.0.dev1.tar` & `readchar-4.1.0.dev2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 09:52:21.974347 readchar-4.1.0.dev1/
--rw-r--r--   0 runner    (1001) docker     (121)     1076 2022-11-16 09:52:13.000000 readchar-4.1.0.dev1/LICENCE
--rw-r--r--   0 runner    (1001) docker     (121)     6133 2022-11-16 09:52:21.974347 readchar-4.1.0.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4717 2022-11-16 09:52:13.000000 readchar-4.1.0.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 09:52:21.974347 readchar-4.1.0.dev1/readchar/
--rw-r--r--   0 runner    (1001) docker     (121)      535 2022-11-16 09:52:20.000000 readchar-4.1.0.dev1/readchar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      487 2022-11-16 09:52:13.000000 readchar-4.1.0.dev1/readchar/_base_key.py
--rw-r--r--   0 runner    (1001) docker     (121)      365 2022-11-16 09:52:13.000000 readchar-4.1.0.dev1/readchar/_config.py
--rw-r--r--   0 runner    (1001) docker     (121)      837 2022-11-16 09:52:13.000000 readchar-4.1.0.dev1/readchar/_posix_key.py
--rw-r--r--   0 runner    (1001) docker     (121)     1370 2022-11-16 09:52:13.000000 readchar-4.1.0.dev1/readchar/_posix_read.py
--rw-r--r--   0 runner    (1001) docker     (121)     1062 2022-11-16 09:52:13.000000 readchar-4.1.0.dev1/readchar/_win_key.py
--rw-r--r--   0 runner    (1001) docker     (121)      732 2022-11-16 09:52:13.000000 readchar-4.1.0.dev1/readchar/_win_read.py
--rw-r--r--   0 runner    (1001) docker     (121)      384 2022-11-16 09:52:13.000000 readchar-4.1.0.dev1/readchar/key.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 09:52:21.974347 readchar-4.1.0.dev1/readchar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6133 2022-11-16 09:52:21.000000 readchar-4.1.0.dev1/readchar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      364 2022-11-16 09:52:21.000000 readchar-4.1.0.dev1/readchar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-16 09:52:21.000000 readchar-4.1.0.dev1/readchar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-11-16 09:52:21.000000 readchar-4.1.0.dev1/readchar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-11-16 09:52:21.000000 readchar-4.1.0.dev1/readchar.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1852 2022-11-16 09:52:21.974347 readchar-4.1.0.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      279 2022-11-16 09:52:13.000000 readchar-4.1.0.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:54:01.994288 readchar-4.1.0.dev2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-16 15:53:52.000000 readchar-4.1.0.dev2/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-05-16 15:54:01.994288 readchar-4.1.0.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-05-16 15:53:52.000000 readchar-4.1.0.dev2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-16 15:53:59.000000 readchar-4.1.0.dev2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:54:01.994288 readchar-4.1.0.dev2/readchar/
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-16 15:53:52.000000 readchar-4.1.0.dev2/readchar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-16 15:53:52.000000 readchar-4.1.0.dev2/readchar/_base_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-16 15:53:52.000000 readchar-4.1.0.dev2/readchar/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-16 15:53:52.000000 readchar-4.1.0.dev2/readchar/_posix_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-16 15:53:52.000000 readchar-4.1.0.dev2/readchar/_posix_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-16 15:53:52.000000 readchar-4.1.0.dev2/readchar/_win_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-16 15:53:52.000000 readchar-4.1.0.dev2/readchar/_win_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-16 15:53:52.000000 readchar-4.1.0.dev2/readchar/key.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 15:53:52.000000 readchar-4.1.0.dev2/readchar/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:54:01.994288 readchar-4.1.0.dev2/readchar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-05-16 15:54:01.000000 readchar-4.1.0.dev2/readchar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-16 15:54:01.000000 readchar-4.1.0.dev2/readchar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 15:54:01.000000 readchar-4.1.0.dev2/readchar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-16 15:54:01.000000 readchar-4.1.0.dev2/readchar.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 15:54:01.994288 readchar-4.1.0.dev2/setup.cfg
```

### Comparing `readchar-4.1.0.dev1/LICENCE` & `readchar-4.1.0.dev2/LICENCE`

 * *Files identical despite different names*

### Comparing `readchar-4.1.0.dev1/PKG-INFO` & `readchar-4.1.0.dev2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,66 @@
 Metadata-Version: 2.1
 Name: readchar
-Version: 4.1.0.dev1
+Version: 4.1.0.dev2
 Summary: Library to easily read single chars and key strokes
-Home-page: https://github.com/magmax/python-readchar
 Author: Miguel Ángel García
-Author-email: miguelangel.garcia@gmail.com
-License: MIT
-Project-URL: Download, https://pypi.org/project/readchar/#files
-Project-URL: Bug Tracker, https://github.com/magmax/python-readchar/issues
-Project-URL: Source Code, https://github.com/magmax/python-readchar
-Keywords: charaters,keystrokes,stdin,command line
+Author-email: Jan Wille <mail@janwille.de>
+Maintainer-email: Jan Wille <mail@janwille.de>
+License: MIT Licence
+        
+        Copyright (c) 2022 Miguel Angel Garcia
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicence, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://pypi.org/project/readchar
+Project-URL: Repository, https://github.com/magmax/python-readchar
+Project-URL: Issues, https://github.com/magmax/python-readchar/issues
+Project-URL: Changelog, https://github.com/magmax/python-readchar/releases
+Keywords: characters,keystrokes,stdin,command line
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: User Interfaces
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 [![GitHub Repository](https://img.shields.io/badge/-GitHub-%230D0D0D?logo=github&labelColor=gray)](https://github.com/magmax/python-readchar)
 [![Latest PyPi version](https://img.shields.io/pypi/v/readchar.svg)](https://pypi.python.org/pypi/readchar)
 [![supported Python versions](https://img.shields.io/pypi/pyversions/readchar)](https://pypi.python.org/pypi/readchar)
 [![Project licence](https://img.shields.io/pypi/l/readchar?color=blue)](LICENCE) <br>
-[![Automated testing results](https://img.shields.io/github/workflow/status/magmax/python-readchar/Tests/master?label=Tests)](https://github.com/magmax/python-readchar/actions/workflows/run-tests.yaml?query=branch%3Amaster)
+[![Automated testing results](https://img.shields.io/github/actions/workflow/status/magmax/python-readchar/run-tests.yaml?branch=master)](https://github.com/magmax/python-readchar/actions/workflows/run-tests.yaml?query=branch%3Amaster)
 [![Coveralls results](https://coveralls.io/repos/github/magmax/python-readchar/badge.svg?branch=master)](https://coveralls.io/github/magmax/python-readchar?branch=master)
 [![Number of PyPi downloads](https://img.shields.io/pypi/dd/readchar.svg)](https://pypi.python.org/pypi/readchar)
 
 # python-readchar
 
 Library to easily read single chars and keystrokes.
 
@@ -108,15 +130,15 @@
   - navigation keys: <kbd>INSERT</kbd>, <kbd>HOME</kbd>,...
   - function keys: <kbd>F1</kbd> to <kbd>F12</kbd>
   - combinations with <kbd>ALT</kbd>: <kbd>ALT</kbd>+<kbd>A</kbd>,...
   - combinations with <kbd>CTRL</kbd> and <kbd>ALT</kbd>:
     <kbd>CTRL</kbd>+<kbd>ALT</kbd>+<kbd>SUPR</kbd>,...
 
 > **Note** <kbd>CTRL</kbd>+<kbd>C</kbd> will not be returned by `readkey()`, but instead
-> raise a `KeyboardInterupt`. If you what to handle it yourself, use `readchar()`.
+> raise a `KeyboardInterupt`. If you want to handle it yourself, use `readchar()`.
 
 ### `readchar.key` module
 
 This submodule contains a list of available keys to compare against. The constants are
 defined depending on your operating system, so it should be fully portable. If a key is
 listed here for your platform, `readkey()` can read it, and you can compare against it.
 
@@ -142,15 +164,15 @@
 
 - Linux
 - Windows
 
 Some operating systems are enabled, but not actively tested or supported:
 
 - macOS
-- FreeBSD
+- FreeBSD / OpenBSD
 
 Theoretically every Unix based system should work, but they will not be actively tested.
 It is also required that somebody provides initial test results before the OS is enabled
 and added to the list. Feel free to open a PR for that.
 
 Thank you!
```

### Comparing `readchar-4.1.0.dev1/README.md` & `readchar-4.1.0.dev2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [![GitHub Repository](https://img.shields.io/badge/-GitHub-%230D0D0D?logo=github&labelColor=gray)](https://github.com/magmax/python-readchar)
 [![Latest PyPi version](https://img.shields.io/pypi/v/readchar.svg)](https://pypi.python.org/pypi/readchar)
 [![supported Python versions](https://img.shields.io/pypi/pyversions/readchar)](https://pypi.python.org/pypi/readchar)
 [![Project licence](https://img.shields.io/pypi/l/readchar?color=blue)](LICENCE) <br>
-[![Automated testing results](https://img.shields.io/github/workflow/status/magmax/python-readchar/Tests/master?label=Tests)](https://github.com/magmax/python-readchar/actions/workflows/run-tests.yaml?query=branch%3Amaster)
+[![Automated testing results](https://img.shields.io/github/actions/workflow/status/magmax/python-readchar/run-tests.yaml?branch=master)](https://github.com/magmax/python-readchar/actions/workflows/run-tests.yaml?query=branch%3Amaster)
 [![Coveralls results](https://coveralls.io/repos/github/magmax/python-readchar/badge.svg?branch=master)](https://coveralls.io/github/magmax/python-readchar?branch=master)
 [![Number of PyPi downloads](https://img.shields.io/pypi/dd/readchar.svg)](https://pypi.python.org/pypi/readchar)
 
 # python-readchar
 
 Library to easily read single chars and keystrokes.
 
@@ -76,15 +76,15 @@
   - navigation keys: <kbd>INSERT</kbd>, <kbd>HOME</kbd>,...
   - function keys: <kbd>F1</kbd> to <kbd>F12</kbd>
   - combinations with <kbd>ALT</kbd>: <kbd>ALT</kbd>+<kbd>A</kbd>,...
   - combinations with <kbd>CTRL</kbd> and <kbd>ALT</kbd>:
     <kbd>CTRL</kbd>+<kbd>ALT</kbd>+<kbd>SUPR</kbd>,...
 
 > **Note** <kbd>CTRL</kbd>+<kbd>C</kbd> will not be returned by `readkey()`, but instead
-> raise a `KeyboardInterupt`. If you what to handle it yourself, use `readchar()`.
+> raise a `KeyboardInterupt`. If you want to handle it yourself, use `readchar()`.
 
 ### `readchar.key` module
 
 This submodule contains a list of available keys to compare against. The constants are
 defined depending on your operating system, so it should be fully portable. If a key is
 listed here for your platform, `readkey()` can read it, and you can compare against it.
 
@@ -110,15 +110,15 @@
 
 - Linux
 - Windows
 
 Some operating systems are enabled, but not actively tested or supported:
 
 - macOS
-- FreeBSD
+- FreeBSD / OpenBSD
 
 Theoretically every Unix based system should work, but they will not be actively tested.
 It is also required that somebody provides initial test results before the OS is enabled
 and added to the list. Feel free to open a PR for that.
 
 Thank you!
```

### Comparing `readchar-4.1.0.dev1/readchar/_posix_key.py` & `readchar-4.1.0.dev2/readchar/_posix_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 INSERT = "\x1b\x5b\x32\x7e"
 SUPR = "\x1b\x5b\x33\x7e"
 HOME = "\x1b\x5b\x48"
 END = "\x1b\x5b\x46"
 PAGE_UP = "\x1b\x5b\x35\x7e"
 PAGE_DOWN = "\x1b\x5b\x36\x7e"
 
-# funcion keys
+# function keys
 F1 = "\x1b\x4f\x50"
 F2 = "\x1b\x4f\x51"
 F3 = "\x1b\x4f\x52"
 F4 = "\x1b\x4f\x53"
 F5 = "\x1b\x5b\x31\x35\x7e"
 F6 = "\x1b\x5b\x31\x37\x7e"
 F7 = "\x1b\x5b\x31\x38\x7e"
```

### Comparing `readchar-4.1.0.dev1/readchar/_posix_read.py` & `readchar-4.1.0.dev2/readchar/_posix_read.py`

 * *Files identical despite different names*

### Comparing `readchar-4.1.0.dev1/readchar/_win_key.py` & `readchar-4.1.0.dev2/readchar/_win_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 INSERT = "\x00\x52"
 SUPR = "\x00\x53"
 HOME = "\x00\x47"
 END = "\x00\x4f"
 PAGE_UP = "\x00\x49"
 PAGE_DOWN = "\x00\x51"
 
-# funcion keys
+# function keys
 F1 = "\x00\x3b"
 F2 = "\x00\x3c"
 F3 = "\x00\x3d"
 F4 = "\x00\x3e"
 F5 = "\x00\x3f"
 F6 = "\x00\x40"
 F7 = "\x00\x41"
```

### Comparing `readchar-4.1.0.dev1/readchar/_win_read.py` & `readchar-4.1.0.dev2/readchar/_win_read.py`

 * *Files identical despite different names*

### Comparing `readchar-4.1.0.dev1/readchar.egg-info/PKG-INFO` & `readchar-4.1.0.dev2/readchar.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,66 @@
 Metadata-Version: 2.1
 Name: readchar
-Version: 4.1.0.dev1
+Version: 4.1.0.dev2
 Summary: Library to easily read single chars and key strokes
-Home-page: https://github.com/magmax/python-readchar
 Author: Miguel Ángel García
-Author-email: miguelangel.garcia@gmail.com
-License: MIT
-Project-URL: Download, https://pypi.org/project/readchar/#files
-Project-URL: Bug Tracker, https://github.com/magmax/python-readchar/issues
-Project-URL: Source Code, https://github.com/magmax/python-readchar
-Keywords: charaters,keystrokes,stdin,command line
+Author-email: Jan Wille <mail@janwille.de>
+Maintainer-email: Jan Wille <mail@janwille.de>
+License: MIT Licence
+        
+        Copyright (c) 2022 Miguel Angel Garcia
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicence, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://pypi.org/project/readchar
+Project-URL: Repository, https://github.com/magmax/python-readchar
+Project-URL: Issues, https://github.com/magmax/python-readchar/issues
+Project-URL: Changelog, https://github.com/magmax/python-readchar/releases
+Keywords: characters,keystrokes,stdin,command line
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: User Interfaces
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 [![GitHub Repository](https://img.shields.io/badge/-GitHub-%230D0D0D?logo=github&labelColor=gray)](https://github.com/magmax/python-readchar)
 [![Latest PyPi version](https://img.shields.io/pypi/v/readchar.svg)](https://pypi.python.org/pypi/readchar)
 [![supported Python versions](https://img.shields.io/pypi/pyversions/readchar)](https://pypi.python.org/pypi/readchar)
 [![Project licence](https://img.shields.io/pypi/l/readchar?color=blue)](LICENCE) <br>
-[![Automated testing results](https://img.shields.io/github/workflow/status/magmax/python-readchar/Tests/master?label=Tests)](https://github.com/magmax/python-readchar/actions/workflows/run-tests.yaml?query=branch%3Amaster)
+[![Automated testing results](https://img.shields.io/github/actions/workflow/status/magmax/python-readchar/run-tests.yaml?branch=master)](https://github.com/magmax/python-readchar/actions/workflows/run-tests.yaml?query=branch%3Amaster)
 [![Coveralls results](https://coveralls.io/repos/github/magmax/python-readchar/badge.svg?branch=master)](https://coveralls.io/github/magmax/python-readchar?branch=master)
 [![Number of PyPi downloads](https://img.shields.io/pypi/dd/readchar.svg)](https://pypi.python.org/pypi/readchar)
 
 # python-readchar
 
 Library to easily read single chars and keystrokes.
 
@@ -108,15 +130,15 @@
   - navigation keys: <kbd>INSERT</kbd>, <kbd>HOME</kbd>,...
   - function keys: <kbd>F1</kbd> to <kbd>F12</kbd>
   - combinations with <kbd>ALT</kbd>: <kbd>ALT</kbd>+<kbd>A</kbd>,...
   - combinations with <kbd>CTRL</kbd> and <kbd>ALT</kbd>:
     <kbd>CTRL</kbd>+<kbd>ALT</kbd>+<kbd>SUPR</kbd>,...
 
 > **Note** <kbd>CTRL</kbd>+<kbd>C</kbd> will not be returned by `readkey()`, but instead
-> raise a `KeyboardInterupt`. If you what to handle it yourself, use `readchar()`.
+> raise a `KeyboardInterupt`. If you want to handle it yourself, use `readchar()`.
 
 ### `readchar.key` module
 
 This submodule contains a list of available keys to compare against. The constants are
 defined depending on your operating system, so it should be fully portable. If a key is
 listed here for your platform, `readkey()` can read it, and you can compare against it.
 
@@ -142,15 +164,15 @@
 
 - Linux
 - Windows
 
 Some operating systems are enabled, but not actively tested or supported:
 
 - macOS
-- FreeBSD
+- FreeBSD / OpenBSD
 
 Theoretically every Unix based system should work, but they will not be actively tested.
 It is also required that somebody provides initial test results before the OS is enabled
 and added to the list. Feel free to open a PR for that.
 
 Thank you!
```

