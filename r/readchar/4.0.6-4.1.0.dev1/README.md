# Comparing `tmp/readchar-4.0.6.tar.gz` & `tmp/readchar-4.1.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readchar-4.0.6.tar", last modified: Fri Mar 15 17:00:39 2024, max compression
+gzip compressed data, was "readchar-4.1.0.dev1.tar", last modified: Wed Nov 16 09:52:21 2022, max compression
```

## Comparing `readchar-4.0.6.tar` & `readchar-4.1.0.dev1.tar`

### file list

```diff
@@ -1,23 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 17:00:39.231788 readchar-4.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-03-15 17:00:31.000000 readchar-4.0.6/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-03-15 17:00:39.231788 readchar-4.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-03-15 17:00:31.000000 readchar-4.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 17:00:39.231788 readchar-4.0.6/readchar/
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-03-15 17:00:38.000000 readchar-4.0.6/readchar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-03-15 17:00:31.000000 readchar-4.0.6/readchar/_base_key.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-03-15 17:00:31.000000 readchar-4.0.6/readchar/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-03-15 17:00:31.000000 readchar-4.0.6/readchar/_posix_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-03-15 17:00:31.000000 readchar-4.0.6/readchar/_posix_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-03-15 17:00:31.000000 readchar-4.0.6/readchar/_win_key.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-03-15 17:00:31.000000 readchar-4.0.6/readchar/_win_read.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-15 17:00:31.000000 readchar-4.0.6/readchar/key.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 17:00:31.000000 readchar-4.0.6/readchar/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 17:00:39.231788 readchar-4.0.6/readchar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-03-15 17:00:39.000000 readchar-4.0.6/readchar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-03-15 17:00:39.000000 readchar-4.0.6/readchar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 17:00:39.000000 readchar-4.0.6/readchar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 17:00:39.000000 readchar-4.0.6/readchar.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-15 17:00:39.000000 readchar-4.0.6/readchar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-15 17:00:39.000000 readchar-4.0.6/readchar.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-03-15 17:00:39.235787 readchar-4.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-15 17:00:31.000000 readchar-4.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 09:52:21.974347 readchar-4.1.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (121)     1076 2022-11-16 09:52:13.000000 readchar-4.1.0.dev1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (121)     6133 2022-11-16 09:52:21.974347 readchar-4.1.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4717 2022-11-16 09:52:13.000000 readchar-4.1.0.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 09:52:21.974347 readchar-4.1.0.dev1/readchar/
+-rw-r--r--   0 runner    (1001) docker     (121)      535 2022-11-16 09:52:20.000000 readchar-4.1.0.dev1/readchar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      487 2022-11-16 09:52:13.000000 readchar-4.1.0.dev1/readchar/_base_key.py
+-rw-r--r--   0 runner    (1001) docker     (121)      365 2022-11-16 09:52:13.000000 readchar-4.1.0.dev1/readchar/_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)      837 2022-11-16 09:52:13.000000 readchar-4.1.0.dev1/readchar/_posix_key.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1370 2022-11-16 09:52:13.000000 readchar-4.1.0.dev1/readchar/_posix_read.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1062 2022-11-16 09:52:13.000000 readchar-4.1.0.dev1/readchar/_win_key.py
+-rw-r--r--   0 runner    (1001) docker     (121)      732 2022-11-16 09:52:13.000000 readchar-4.1.0.dev1/readchar/_win_read.py
+-rw-r--r--   0 runner    (1001) docker     (121)      384 2022-11-16 09:52:13.000000 readchar-4.1.0.dev1/readchar/key.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 09:52:21.974347 readchar-4.1.0.dev1/readchar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6133 2022-11-16 09:52:21.000000 readchar-4.1.0.dev1/readchar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      364 2022-11-16 09:52:21.000000 readchar-4.1.0.dev1/readchar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-16 09:52:21.000000 readchar-4.1.0.dev1/readchar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-11-16 09:52:21.000000 readchar-4.1.0.dev1/readchar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-11-16 09:52:21.000000 readchar-4.1.0.dev1/readchar.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1852 2022-11-16 09:52:21.974347 readchar-4.1.0.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      279 2022-11-16 09:52:13.000000 readchar-4.1.0.dev1/setup.py
```

### Comparing `readchar-4.0.6/LICENCE` & `readchar-4.1.0.dev1/LICENCE`

 * *Files identical despite different names*

### Comparing `readchar-4.0.6/PKG-INFO` & `readchar-4.1.0.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 Metadata-Version: 2.1
 Name: readchar
-Version: 4.0.6
+Version: 4.1.0.dev1
 Summary: Library to easily read single chars and key strokes
 Home-page: https://github.com/magmax/python-readchar
 Author: Miguel Ángel García
 Author-email: miguelangel.garcia@gmail.com
 License: MIT
 Project-URL: Download, https://pypi.org/project/readchar/#files
 Project-URL: Bug Tracker, https://github.com/magmax/python-readchar/issues
 Project-URL: Source Code, https://github.com/magmax/python-readchar
-Keywords: characters,keystrokes,stdin,command line
+Keywords: charaters,keystrokes,stdin,command line
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: User Interfaces
-Requires-Python: >=3.8
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE
-Requires-Dist: setuptools>=41.0
 
 [![GitHub Repository](https://img.shields.io/badge/-GitHub-%230D0D0D?logo=github&labelColor=gray)](https://github.com/magmax/python-readchar)
 [![Latest PyPi version](https://img.shields.io/pypi/v/readchar.svg)](https://pypi.python.org/pypi/readchar)
 [![supported Python versions](https://img.shields.io/pypi/pyversions/readchar)](https://pypi.python.org/pypi/readchar)
 [![Project licence](https://img.shields.io/pypi/l/readchar?color=blue)](LICENCE) <br>
-[![Automated testing results](https://img.shields.io/github/actions/workflow/status/magmax/python-readchar/run-tests.yaml?branch=master)](https://github.com/magmax/python-readchar/actions/workflows/run-tests.yaml?query=branch%3Amaster)
+[![Automated testing results](https://img.shields.io/github/workflow/status/magmax/python-readchar/Tests/master?label=Tests)](https://github.com/magmax/python-readchar/actions/workflows/run-tests.yaml?query=branch%3Amaster)
 [![Coveralls results](https://coveralls.io/repos/github/magmax/python-readchar/badge.svg?branch=master)](https://coveralls.io/github/magmax/python-readchar?branch=master)
 [![Number of PyPi downloads](https://img.shields.io/pypi/dd/readchar.svg)](https://pypi.python.org/pypi/readchar)
 
 # python-readchar
 
 Library to easily read single chars and keystrokes.
 
@@ -109,15 +108,15 @@
   - navigation keys: <kbd>INSERT</kbd>, <kbd>HOME</kbd>,...
   - function keys: <kbd>F1</kbd> to <kbd>F12</kbd>
   - combinations with <kbd>ALT</kbd>: <kbd>ALT</kbd>+<kbd>A</kbd>,...
   - combinations with <kbd>CTRL</kbd> and <kbd>ALT</kbd>:
     <kbd>CTRL</kbd>+<kbd>ALT</kbd>+<kbd>SUPR</kbd>,...
 
 > **Note** <kbd>CTRL</kbd>+<kbd>C</kbd> will not be returned by `readkey()`, but instead
-> raise a `KeyboardInterupt`. If you want to handle it yourself, use `readchar()`.
+> raise a `KeyboardInterupt`. If you what to handle it yourself, use `readchar()`.
 
 ### `readchar.key` module
 
 This submodule contains a list of available keys to compare against. The constants are
 defined depending on your operating system, so it should be fully portable. If a key is
 listed here for your platform, `readkey()` can read it, and you can compare against it.
 
@@ -143,15 +142,15 @@
 
 - Linux
 - Windows
 
 Some operating systems are enabled, but not actively tested or supported:
 
 - macOS
-- FreeBSD / OpenBSD
+- FreeBSD
 
 Theoretically every Unix based system should work, but they will not be actively tested.
 It is also required that somebody provides initial test results before the OS is enabled
 and added to the list. Feel free to open a PR for that.
 
 Thank you!
```

### Comparing `readchar-4.0.6/README.md` & `readchar-4.1.0.dev1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [![GitHub Repository](https://img.shields.io/badge/-GitHub-%230D0D0D?logo=github&labelColor=gray)](https://github.com/magmax/python-readchar)
 [![Latest PyPi version](https://img.shields.io/pypi/v/readchar.svg)](https://pypi.python.org/pypi/readchar)
 [![supported Python versions](https://img.shields.io/pypi/pyversions/readchar)](https://pypi.python.org/pypi/readchar)
 [![Project licence](https://img.shields.io/pypi/l/readchar?color=blue)](LICENCE) <br>
-[![Automated testing results](https://img.shields.io/github/actions/workflow/status/magmax/python-readchar/run-tests.yaml?branch=master)](https://github.com/magmax/python-readchar/actions/workflows/run-tests.yaml?query=branch%3Amaster)
+[![Automated testing results](https://img.shields.io/github/workflow/status/magmax/python-readchar/Tests/master?label=Tests)](https://github.com/magmax/python-readchar/actions/workflows/run-tests.yaml?query=branch%3Amaster)
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
-> raise a `KeyboardInterupt`. If you want to handle it yourself, use `readchar()`.
+> raise a `KeyboardInterupt`. If you what to handle it yourself, use `readchar()`.
 
 ### `readchar.key` module
 
 This submodule contains a list of available keys to compare against. The constants are
 defined depending on your operating system, so it should be fully portable. If a key is
 listed here for your platform, `readkey()` can read it, and you can compare against it.
 
@@ -110,15 +110,15 @@
 
 - Linux
 - Windows
 
 Some operating systems are enabled, but not actively tested or supported:
 
 - macOS
-- FreeBSD / OpenBSD
+- FreeBSD
 
 Theoretically every Unix based system should work, but they will not be actively tested.
 It is also required that somebody provides initial test results before the OS is enabled
 and added to the list. Feel free to open a PR for that.
 
 Thank you!
```

### Comparing `readchar-4.0.6/readchar/__init__.py` & `readchar-4.1.0.dev1/readchar/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Library to easily read single chars and key strokes"""
 
-__version__ = '4.0.6'
+__version__ = '4.1.0-dev1'
 __all__ = ["readchar", "readkey", "key", "config"]
 
 from sys import platform
 
 from ._config import config
 
 
-if platform.startswith(("linux", "darwin", "freebsd", "openbsd")):
+if platform.startswith(("linux", "darwin", "freebsd")):
     from . import _posix_key as key
     from ._posix_read import readchar, readkey
 elif platform in ("win32", "cygwin"):
     from . import _win_key as key
     from ._win_read import readchar, readkey
 else:
     raise NotImplementedError(f"The platform {platform} is not supported yet")
```

### Comparing `readchar-4.0.6/readchar/_posix_key.py` & `readchar-4.1.0.dev1/readchar/_posix_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 INSERT = "\x1b\x5b\x32\x7e"
 SUPR = "\x1b\x5b\x33\x7e"
 HOME = "\x1b\x5b\x48"
 END = "\x1b\x5b\x46"
 PAGE_UP = "\x1b\x5b\x35\x7e"
 PAGE_DOWN = "\x1b\x5b\x36\x7e"
 
-# function keys
+# funcion keys
 F1 = "\x1b\x4f\x50"
 F2 = "\x1b\x4f\x51"
 F3 = "\x1b\x4f\x52"
 F4 = "\x1b\x4f\x53"
 F5 = "\x1b\x5b\x31\x35\x7e"
 F6 = "\x1b\x5b\x31\x37\x7e"
 F7 = "\x1b\x5b\x31\x38\x7e"
```

### Comparing `readchar-4.0.6/readchar/_posix_read.py` & `readchar-4.1.0.dev1/readchar/_posix_read.py`

 * *Files identical despite different names*

### Comparing `readchar-4.0.6/readchar/_win_key.py` & `readchar-4.1.0.dev1/readchar/_win_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 INSERT = "\x00\x52"
 SUPR = "\x00\x53"
 HOME = "\x00\x47"
 END = "\x00\x4f"
 PAGE_UP = "\x00\x49"
 PAGE_DOWN = "\x00\x51"
 
-# function keys
+# funcion keys
 F1 = "\x00\x3b"
 F2 = "\x00\x3c"
 F3 = "\x00\x3d"
 F4 = "\x00\x3e"
 F5 = "\x00\x3f"
 F6 = "\x00\x40"
 F7 = "\x00\x41"
```

### Comparing `readchar-4.0.6/readchar/_win_read.py` & `readchar-4.1.0.dev1/readchar/_win_read.py`

 * *Files identical despite different names*

### Comparing `readchar-4.0.6/readchar.egg-info/PKG-INFO` & `readchar-4.1.0.dev1/readchar.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 Metadata-Version: 2.1
 Name: readchar
-Version: 4.0.6
+Version: 4.1.0.dev1
 Summary: Library to easily read single chars and key strokes
 Home-page: https://github.com/magmax/python-readchar
 Author: Miguel Ángel García
 Author-email: miguelangel.garcia@gmail.com
 License: MIT
 Project-URL: Download, https://pypi.org/project/readchar/#files
 Project-URL: Bug Tracker, https://github.com/magmax/python-readchar/issues
 Project-URL: Source Code, https://github.com/magmax/python-readchar
-Keywords: characters,keystrokes,stdin,command line
+Keywords: charaters,keystrokes,stdin,command line
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: User Interfaces
-Requires-Python: >=3.8
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE
-Requires-Dist: setuptools>=41.0
 
 [![GitHub Repository](https://img.shields.io/badge/-GitHub-%230D0D0D?logo=github&labelColor=gray)](https://github.com/magmax/python-readchar)
 [![Latest PyPi version](https://img.shields.io/pypi/v/readchar.svg)](https://pypi.python.org/pypi/readchar)
 [![supported Python versions](https://img.shields.io/pypi/pyversions/readchar)](https://pypi.python.org/pypi/readchar)
 [![Project licence](https://img.shields.io/pypi/l/readchar?color=blue)](LICENCE) <br>
-[![Automated testing results](https://img.shields.io/github/actions/workflow/status/magmax/python-readchar/run-tests.yaml?branch=master)](https://github.com/magmax/python-readchar/actions/workflows/run-tests.yaml?query=branch%3Amaster)
+[![Automated testing results](https://img.shields.io/github/workflow/status/magmax/python-readchar/Tests/master?label=Tests)](https://github.com/magmax/python-readchar/actions/workflows/run-tests.yaml?query=branch%3Amaster)
 [![Coveralls results](https://coveralls.io/repos/github/magmax/python-readchar/badge.svg?branch=master)](https://coveralls.io/github/magmax/python-readchar?branch=master)
 [![Number of PyPi downloads](https://img.shields.io/pypi/dd/readchar.svg)](https://pypi.python.org/pypi/readchar)
 
 # python-readchar
 
 Library to easily read single chars and keystrokes.
 
@@ -109,15 +108,15 @@
   - navigation keys: <kbd>INSERT</kbd>, <kbd>HOME</kbd>,...
   - function keys: <kbd>F1</kbd> to <kbd>F12</kbd>
   - combinations with <kbd>ALT</kbd>: <kbd>ALT</kbd>+<kbd>A</kbd>,...
   - combinations with <kbd>CTRL</kbd> and <kbd>ALT</kbd>:
     <kbd>CTRL</kbd>+<kbd>ALT</kbd>+<kbd>SUPR</kbd>,...
 
 > **Note** <kbd>CTRL</kbd>+<kbd>C</kbd> will not be returned by `readkey()`, but instead
-> raise a `KeyboardInterupt`. If you want to handle it yourself, use `readchar()`.
+> raise a `KeyboardInterupt`. If you what to handle it yourself, use `readchar()`.
 
 ### `readchar.key` module
 
 This submodule contains a list of available keys to compare against. The constants are
 defined depending on your operating system, so it should be fully portable. If a key is
 listed here for your platform, `readkey()` can read it, and you can compare against it.
 
@@ -143,15 +142,15 @@
 
 - Linux
 - Windows
 
 Some operating systems are enabled, but not actively tested or supported:
 
 - macOS
-- FreeBSD / OpenBSD
+- FreeBSD
 
 Theoretically every Unix based system should work, but they will not be actively tested.
 It is also required that somebody provides initial test results before the OS is enabled
 and added to the list. Feel free to open a PR for that.
 
 Thank you!
```

### Comparing `readchar-4.0.6/setup.cfg` & `readchar-4.1.0.dev1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -3,61 +3,56 @@
 version = attr: readchar.__version__
 description = Library to easily read single chars and key strokes
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/magmax/python-readchar
 author_email = miguelangel.garcia@gmail.com
 license = MIT
+license_file = LICENCE
 license_files = LICENCE
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Environment :: Console
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: Microsoft :: Windows
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
+	Programming Language :: Python :: 3.6
+	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
-	Programming Language :: Python :: 3.11
-	Programming Language :: Python :: 3.12
 	Programming Language :: Python :: Implementation :: CPython
 	Topic :: Software Development
 	Topic :: Software Development :: User Interfaces
 keywords = 
-	characters
+	charaters
 	keystrokes
 	stdin
 	command line
 project_urls = 
 	Download = https://pypi.org/project/readchar/#files
 	Bug Tracker = https://github.com/magmax/python-readchar/issues
 	Source Code = https://github.com/magmax/python-readchar
 
 [options]
 packages = find:
 install_requires = 
 	setuptools>=41.0
-python_requires = >=3.8
-include_package_data = True
-zip_safe = false
+python_requires = >=3.6
 
 [options.packages.find]
 exclude = 
 	.git/
 	.github/
 	.venv/
 	tests/
 
-[options.package_data]
-readchar = 
-	py.typed
-
 [tool:pytest]
 testpaths = tests
 addopts = -r fEsxwX -s --cov=readchar
 
 [flake8]
 max-complexity = 12
 max-line-length = 88
```

