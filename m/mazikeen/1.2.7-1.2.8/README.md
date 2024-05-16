# Comparing `tmp/mazikeen-1.2.7.tar.gz` & `tmp/mazikeen-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mazikeen-1.2.7.tar", last modified: Tue Aug  1 23:56:49 2023, max compression
+gzip compressed data, was "mazikeen-1.2.8.tar", last modified: Wed May 15 21:54:10 2024, max compression
```

## Comparing `mazikeen-1.2.7.tar` & `mazikeen-1.2.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:56:49.470538 mazikeen-1.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-01 23:56:39.000000 mazikeen-1.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-08-01 23:56:49.470538 mazikeen-1.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-08-01 23:56:39.000000 mazikeen-1.2.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:56:49.470538 mazikeen-1.2.7/mazikeen/
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-08-01 23:56:39.000000 mazikeen-1.2.7/mazikeen/ConsolePrinter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-01 23:56:39.000000 mazikeen-1.2.7/mazikeen/DiffBlock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-08-01 23:56:39.000000 mazikeen-1.2.7/mazikeen/GeneratorDiffBlock.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-01 23:56:39.000000 mazikeen-1.2.7/mazikeen/GeneratorException.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-08-01 23:56:39.000000 mazikeen-1.2.7/mazikeen/GeneratorLooper.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-08-01 23:56:39.000000 mazikeen-1.2.7/mazikeen/GeneratorMakedirs.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-01 23:56:39.000000 mazikeen-1.2.7/mazikeen/GeneratorRmdir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-08-01 23:56:39.000000 mazikeen-1.2.7/mazikeen/GeneratorRunBlock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-08-01 23:56:39.000000 mazikeen-1.2.7/mazikeen/GeneratorUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-08-01 23:56:39.000000 mazikeen-1.2.7/mazikeen/Loopers.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-08-01 23:56:39.000000 mazikeen-1.2.7/mazikeen/MakedirsBlock.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-08-01 23:56:39.000000 mazikeen-1.2.7/mazikeen/RmdirBlock.py
--rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-08-01 23:56:39.000000 mazikeen-1.2.7/mazikeen/RunBlock.py
--rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-08-01 23:56:39.000000 mazikeen-1.2.7/mazikeen/ScriptDataProcessor.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-08-01 23:56:39.000000 mazikeen-1.2.7/mazikeen/ScriptReader.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-08-01 23:56:39.000000 mazikeen-1.2.7/mazikeen/SignalHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-08-01 23:56:39.000000 mazikeen-1.2.7/mazikeen/Utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9513 2023-08-01 23:56:39.000000 mazikeen-1.2.7/mazikeen/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 23:56:39.000000 mazikeen-1.2.7/mazikeen/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:56:49.470538 mazikeen-1.2.7/mazikeen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-08-01 23:56:49.000000 mazikeen-1.2.7/mazikeen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-08-01 23:56:49.000000 mazikeen-1.2.7/mazikeen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 23:56:49.000000 mazikeen-1.2.7/mazikeen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-01 23:56:49.000000 mazikeen-1.2.7/mazikeen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-01 23:56:49.000000 mazikeen-1.2.7/mazikeen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-01 23:56:49.000000 mazikeen-1.2.7/mazikeen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 23:56:49.470538 mazikeen-1.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-08-01 23:56:39.000000 mazikeen-1.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 21:54:10.663919 mazikeen-1.2.8/
+-rw-rw-rw-   0        0        0     1088 2024-05-15 07:42:50.000000 mazikeen-1.2.8/LICENSE
+-rw-rw-rw-   0        0        0     3240 2024-05-15 21:54:10.662917 mazikeen-1.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2086 2024-05-15 07:42:50.000000 mazikeen-1.2.8/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-15 21:54:10.657918 mazikeen-1.2.8/mazikeen/
+-rw-rw-rw-   0        0        0     2411 2024-05-15 07:42:50.000000 mazikeen-1.2.8/mazikeen/ConsolePrinter.py
+-rw-rw-rw-   0        0        0     1090 2024-05-15 07:42:50.000000 mazikeen-1.2.8/mazikeen/DiffBlock.py
+-rw-rw-rw-   0        0        0     2240 2024-05-15 07:42:50.000000 mazikeen-1.2.8/mazikeen/GeneratorDiffBlock.py
+-rw-rw-rw-   0        0        0       48 2024-05-15 07:42:50.000000 mazikeen-1.2.8/mazikeen/GeneratorException.py
+-rw-rw-rw-   0        0        0     4009 2024-05-15 07:42:50.000000 mazikeen-1.2.8/mazikeen/GeneratorLooper.py
+-rw-rw-rw-   0        0        0      275 2024-05-15 07:42:50.000000 mazikeen-1.2.8/mazikeen/GeneratorMakedirs.py
+-rw-rw-rw-   0        0        0      324 2024-05-15 07:42:50.000000 mazikeen-1.2.8/mazikeen/GeneratorRmdir.py
+-rw-rw-rw-   0        0        0     1166 2024-05-15 07:42:50.000000 mazikeen-1.2.8/mazikeen/GeneratorRunBlock.py
+-rw-rw-rw-   0        0        0     1371 2024-05-15 07:42:50.000000 mazikeen-1.2.8/mazikeen/GeneratorUtils.py
+-rw-rw-rw-   0        0        0     4349 2024-05-15 07:42:50.000000 mazikeen-1.2.8/mazikeen/Loopers.py
+-rw-rw-rw-   0        0        0      502 2024-05-15 07:42:50.000000 mazikeen-1.2.8/mazikeen/MakedirsBlock.py
+-rw-rw-rw-   0        0        0      455 2024-05-15 07:42:50.000000 mazikeen-1.2.8/mazikeen/RmdirBlock.py
+-rw-rw-rw-   0        0        0     9106 2024-05-15 07:42:50.000000 mazikeen-1.2.8/mazikeen/RunBlock.py
+-rw-rw-rw-   0        0        0     6901 2024-05-15 07:42:50.000000 mazikeen-1.2.8/mazikeen/ScriptDataProcessor.py
+-rw-rw-rw-   0        0        0      558 2024-05-15 07:42:50.000000 mazikeen-1.2.8/mazikeen/ScriptReader.py
+-rw-rw-rw-   0        0        0      695 2024-05-15 07:42:50.000000 mazikeen-1.2.8/mazikeen/SignalHandler.py
+-rw-rw-rw-   0        0        0     8271 2024-05-15 07:42:50.000000 mazikeen-1.2.8/mazikeen/Utils.py
+-rw-rw-rw-   0        0        0     9737 2024-05-15 20:51:27.000000 mazikeen-1.2.8/mazikeen/__main__.py
+-rw-rw-rw-   0        0        0       23 2024-05-15 20:51:27.000000 mazikeen-1.2.8/mazikeen/version.py
+drwxrwxrwx   0        0        0        0 2024-05-15 21:54:10.661918 mazikeen-1.2.8/mazikeen.egg-info/
+-rw-rw-rw-   0        0        0     3240 2024-05-15 21:54:10.000000 mazikeen-1.2.8/mazikeen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      706 2024-05-15 21:54:10.000000 mazikeen-1.2.8/mazikeen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 21:54:10.000000 mazikeen-1.2.8/mazikeen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-05-15 21:54:10.000000 mazikeen-1.2.8/mazikeen.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       53 2024-05-15 21:54:10.000000 mazikeen-1.2.8/mazikeen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-15 21:54:10.000000 mazikeen-1.2.8/mazikeen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 21:54:10.663919 mazikeen-1.2.8/setup.cfg
+-rw-rw-rw-   0        0        0     1275 2024-05-15 07:42:50.000000 mazikeen-1.2.8/setup.py
```

### Comparing `mazikeen-1.2.7/LICENSE` & `mazikeen-1.2.8/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) [year] [fullname]
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
+MIT License
+
+Copyright (c) [year] [fullname]
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
 SOFTWARE.
```

### Comparing `mazikeen-1.2.7/PKG-INFO` & `mazikeen-1.2.8/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-Metadata-Version: 2.1
-Name: mazikeen
-Version: 1.2.7
-Summary: Test enviroment for CLI application
-Home-page: https://github.com/hanniballar/mazikeen
-Author: Neaga Septimiu
-Author-email: neagas@gmail.com
-License: MIT
-Project-URL: Bug Tracker, https://github.com/hanniballar/mazikeen/issues
-Description: `mazikeen` is a test framework for command line applications.
-        `mazikeen` was created to facilitae testing of CLI application that have a predictable output. It facilitates testing on different operating systems by provideing a diff method that is agnostic to newline and make / remove directory. For `mazikeen` every test has it's own directory helping debugging and organizing tests.
-        `mazikeen` empathise parralel testing.
-        
-        The test structure looks like:
-        ::
-        
-            Testsuit1
-            ├── Testcase1
-            │   └── script.yaml
-            ├── . . .
-            └──TestcaseN
-                └── script.yaml
-            Testsuit2
-            ├── Testcase1
-            │   └── script.yaml
-            ├── ...
-            └──TestcaseN
-                └── script.yaml
-        		
-        An example of a simple test:
-        
-        .. code-block:: yaml
-        
-            # content of script.yaml
-          ---
-          steps:
-            - rmdir: Output
-            - makedirs: Output
-            - run: echo "Hello World" > Output/hello.txt
-            - diff: Output/hello.txt Expected/hello.txt
-        
-        To execute it::
-        
-            $ mazikeen
-            [RUN       ] --- simple
-            [    PASSED] --- simple
-            ----------------------------------------------------------------
-            Total test cases: 1 passed: 1 skipped: 0 error: 0 failed: 0
-            ----------------------------------------------------------------
-            process time: 0.02 execution time: 0.01
-        
-        Features
-        --------
-        - Provides diff functions agnostic to newline and other common operations for different operating systems like make and remove directory. 
-        - Every test case is a directory. Making it easy to debug a failing test as all relevant data is stored in one place.
-        - Parallel execution support. Testscases can be executed in parallel. A testcase can call multiple CLI applications in parallel.
-        
-        
-        Documentation
-        -------------
-        
-        For full documentation, please see https://github.com/hanniballar/mazikeen/blob/master/Documentation/Mazikeen.rst .
-        
-        
-        Bugs/Requests
-        -------------
-        
-        Please use the `GitHub issue tracker <https://github.com/hanniballar/mazikeen/issues>`_ to submit bugs or request features.
-        
-        
-Platform: UNKNOWN
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: Utilities
-Description-Content-Type: text/x-rst
-Provides-Extra: testing
+Metadata-Version: 2.1
+Name: mazikeen
+Version: 1.2.8
+Summary: Test enviroment for CLI application
+Home-page: https://github.com/hanniballar/mazikeen
+Author: Neaga Septimiu
+Author-email: neagas@gmail.com
+License: MIT
+Project-URL: Bug Tracker, https://github.com/hanniballar/mazikeen/issues
+Description: `mazikeen` is a test framework for command line applications.
+        `mazikeen` was created to facilitae testing of CLI application that have a predictable output. It facilitates testing on different operating systems by provideing a diff method that is agnostic to newline and make / remove directory. For `mazikeen` every test has it's own directory helping debugging and organizing tests.
+        `mazikeen` empathise parralel testing.
+        
+        The test structure looks like:
+        ::
+        
+            Testsuit1
+            ├── Testcase1
+            │   └── script.yaml
+            ├── . . .
+            └──TestcaseN
+                └── script.yaml
+            Testsuit2
+            ├── Testcase1
+            │   └── script.yaml
+            ├── ...
+            └──TestcaseN
+                └── script.yaml
+        		
+        An example of a simple test:
+        
+        .. code-block:: yaml
+        
+            # content of script.yaml
+          ---
+          steps:
+            - rmdir: Output
+            - makedirs: Output
+            - run: echo "Hello World" > Output/hello.txt
+            - diff: Output/hello.txt Expected/hello.txt
+        
+        To execute it::
+        
+            $ mazikeen
+            [RUN       ] --- simple
+            [    PASSED] --- simple
+            ----------------------------------------------------------------
+            Total test cases: 1 passed: 1 skipped: 0 error: 0 failed: 0
+            ----------------------------------------------------------------
+            process time: 0.02 execution time: 0.01
+        
+        Features
+        --------
+        - Provides diff functions agnostic to newline and other common operations for different operating systems like make and remove directory. 
+        - Every test case is a directory. Making it easy to debug a failing test as all relevant data is stored in one place.
+        - Parallel execution support. Testscases can be executed in parallel. A testcase can call multiple CLI applications in parallel.
+        
+        
+        Documentation
+        -------------
+        
+        For full documentation, please see https://github.com/hanniballar/mazikeen/blob/master/Documentation/Mazikeen.rst .
+        
+        
+        Bugs/Requests
+        -------------
+        
+        Please use the `GitHub issue tracker <https://github.com/hanniballar/mazikeen/issues>`_ to submit bugs or request features.
+        
+        
+Platform: UNKNOWN
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Utilities
+Description-Content-Type: text/x-rst
+Provides-Extra: testing
```

### Comparing `mazikeen-1.2.7/README.rst` & `mazikeen-1.2.8/README.rst`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-`mazikeen` is a test framework for command line applications.
-`mazikeen` was created to facilitae testing of CLI application that have a predictable output. It facilitates testing on different operating systems by provideing a diff method that is agnostic to newline and make / remove directory. For `mazikeen` every test has it's own directory helping debugging and organizing tests.
-`mazikeen` empathise parralel testing.
-
-The test structure looks like:
-::
-
-    Testsuit1
-    ├── Testcase1
-    │   └── script.yaml
-    ├── . . .
-    └──TestcaseN
-        └── script.yaml
-    Testsuit2
-    ├── Testcase1
-    │   └── script.yaml
-    ├── ...
-    └──TestcaseN
-        └── script.yaml
-		
-An example of a simple test:
-
-.. code-block:: yaml
-
-    # content of script.yaml
-  ---
-  steps:
-    - rmdir: Output
-    - makedirs: Output
-    - run: echo "Hello World" > Output/hello.txt
-    - diff: Output/hello.txt Expected/hello.txt
-
-To execute it::
-
-    $ mazikeen
-    [RUN       ] --- simple
-    [    PASSED] --- simple
-    ----------------------------------------------------------------
-    Total test cases: 1 passed: 1 skipped: 0 error: 0 failed: 0
-    ----------------------------------------------------------------
-    process time: 0.02 execution time: 0.01
-
-Features
---------
-- Provides diff functions agnostic to newline and other common operations for different operating systems like make and remove directory. 
-- Every test case is a directory. Making it easy to debug a failing test as all relevant data is stored in one place.
-- Parallel execution support. Testscases can be executed in parallel. A testcase can call multiple CLI applications in parallel.
-
-
-Documentation
--------------
-
-For full documentation, please see https://github.com/hanniballar/mazikeen/blob/master/Documentation/Mazikeen.rst .
-
-
-Bugs/Requests
--------------
-
-Please use the `GitHub issue tracker <https://github.com/hanniballar/mazikeen/issues>`_ to submit bugs or request features.
-
+`mazikeen` is a test framework for command line applications.
+`mazikeen` was created to facilitae testing of CLI application that have a predictable output. It facilitates testing on different operating systems by provideing a diff method that is agnostic to newline and make / remove directory. For `mazikeen` every test has it's own directory helping debugging and organizing tests.
+`mazikeen` empathise parralel testing.
+
+The test structure looks like:
+::
+
+    Testsuit1
+    ├── Testcase1
+    │   └── script.yaml
+    ├── . . .
+    └──TestcaseN
+        └── script.yaml
+    Testsuit2
+    ├── Testcase1
+    │   └── script.yaml
+    ├── ...
+    └──TestcaseN
+        └── script.yaml
+		
+An example of a simple test:
+
+.. code-block:: yaml
+
+    # content of script.yaml
+  ---
+  steps:
+    - rmdir: Output
+    - makedirs: Output
+    - run: echo "Hello World" > Output/hello.txt
+    - diff: Output/hello.txt Expected/hello.txt
+
+To execute it::
+
+    $ mazikeen
+    [RUN       ] --- simple
+    [    PASSED] --- simple
+    ----------------------------------------------------------------
+    Total test cases: 1 passed: 1 skipped: 0 error: 0 failed: 0
+    ----------------------------------------------------------------
+    process time: 0.02 execution time: 0.01
+
+Features
+--------
+- Provides diff functions agnostic to newline and other common operations for different operating systems like make and remove directory. 
+- Every test case is a directory. Making it easy to debug a failing test as all relevant data is stored in one place.
+- Parallel execution support. Testscases can be executed in parallel. A testcase can call multiple CLI applications in parallel.
+
+
+Documentation
+-------------
+
+For full documentation, please see https://github.com/hanniballar/mazikeen/blob/master/Documentation/Mazikeen.rst .
+
+
+Bugs/Requests
+-------------
+
+Please use the `GitHub issue tracker <https://github.com/hanniballar/mazikeen/issues>`_ to submit bugs or request features.
+
```

### Comparing `mazikeen-1.2.7/mazikeen/ConsolePrinter.py` & `mazikeen-1.2.8/mazikeen/ConsolePrinter.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-import io
-import threading
-
-class Printer():
-    printerCnt = 0
-    printLock = threading.Lock()
-    errorLock = threading.Lock()
-    def __init__(self, verbose = False):
-        self._verbose = verbose
-        self.__printerCnt = Printer.printerCnt
-        Printer.printerCnt += 1
-        self.errorOutput = ""
-
-    def __repr__(self):
-        return f"{self.__class__.__name__} {self.__printerCnt}"
-
-    def __str__(self):
-        return self.__repr__()
-
-    def verbose(self, *args, **kwargs):
-        if self._verbose:
-            self.print(*args, **kwargs, flush = True)
-    
-    def getBufferedPrinter(self):
-        bp = BufferedPrinter(verbose = self._verbose)
-        bp.errorOutput = self.errorOutput
-        return bp
-    
-    def print(self, *args, **kwargs):
-        with Printer.printLock:
-            print(*args, **kwargs)
-    
-    def debug(self, *args, **kwargs):
-        self.print("debug: ", end ="", flush = False) 
-        self.print(*args, **kwargs, flush = True)
-
-    def error(self, *args, **kwargs):
-        with Printer.errorLock:
-            with io.StringIO() as _errorMsg:
-                print("Error: ", file=_errorMsg, end = "", flush = False)
-                print(*args, **kwargs, file=_errorMsg, flush = True)
-                self.errorOutput +=_errorMsg.getvalue()
-            self.print("Error: ", end = "", flush = False)
-            self.print(*args, **kwargs, flush = True)
-        
-    def flush(self):
-        return
-        
-    def isVerbose(self):
-        return self._verbose
-        
-class BufferedPrinter(Printer):
-    def __init__(self, verbose = False):
-        super().__init__(verbose)
-        self.__buffer = None
-        
-    def print(self, *args, **kwargs):
-        output = io.StringIO()
-        print(*args, file=output, **kwargs)
-        outputStr = output.getvalue()
-        if not self.__buffer:
-            self.__buffer = outputStr
-        else :
-            self.__buffer += outputStr
-        
-    def verbose(self, *args, **kwargs):
-        if self._verbose:
-            self.print(*args, **kwargs, flush = True)
-
-    def flush(self):
-        if self.__buffer:
-            super().print(self.__buffer, end="", flush = True)
-        self.__buffer = None
-        
-    def getBufferedPrinter(self):
-        return self
-    
-    def __del__(self):
-        self.flush()
+import io
+import threading
+
+class Printer():
+    printerCnt = 0
+    printLock = threading.Lock()
+    errorLock = threading.Lock()
+    def __init__(self, verbose = False):
+        self._verbose = verbose
+        self.__printerCnt = Printer.printerCnt
+        Printer.printerCnt += 1
+        self.errorOutput = ""
+
+    def __repr__(self):
+        return f"{self.__class__.__name__} {self.__printerCnt}"
+
+    def __str__(self):
+        return self.__repr__()
+
+    def verbose(self, *args, **kwargs):
+        if self._verbose:
+            self.print(*args, **kwargs, flush = True)
+    
+    def getBufferedPrinter(self):
+        bp = BufferedPrinter(verbose = self._verbose)
+        bp.errorOutput = self.errorOutput
+        return bp
+    
+    def print(self, *args, **kwargs):
+        with Printer.printLock:
+            print(*args, **kwargs)
+    
+    def debug(self, *args, **kwargs):
+        self.print("debug: ", end ="", flush = False) 
+        self.print(*args, **kwargs, flush = True)
+
+    def error(self, *args, **kwargs):
+        with Printer.errorLock:
+            with io.StringIO() as _errorMsg:
+                print("Error: ", file=_errorMsg, end = "", flush = False)
+                print(*args, **kwargs, file=_errorMsg, flush = True)
+                self.errorOutput +=_errorMsg.getvalue()
+            self.print("Error: ", end = "", flush = False)
+            self.print(*args, **kwargs, flush = True)
+        
+    def flush(self):
+        return
+        
+    def isVerbose(self):
+        return self._verbose
+        
+class BufferedPrinter(Printer):
+    def __init__(self, verbose = False):
+        super().__init__(verbose)
+        self.__buffer = None
+        
+    def print(self, *args, **kwargs):
+        output = io.StringIO()
+        print(*args, file=output, **kwargs)
+        outputStr = output.getvalue()
+        if not self.__buffer:
+            self.__buffer = outputStr
+        else :
+            self.__buffer += outputStr
+        
+    def verbose(self, *args, **kwargs):
+        if self._verbose:
+            self.print(*args, **kwargs, flush = True)
+
+    def flush(self):
+        if self.__buffer:
+            super().print(self.__buffer, end="", flush = True)
+        self.__buffer = None
+        
+    def getBufferedPrinter(self):
+        return self
+    
+    def __del__(self):
+        self.flush()
```

### Comparing `mazikeen-1.2.7/mazikeen/DiffBlock.py` & `mazikeen-1.2.8/mazikeen/DiffBlock.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-import pathlib
-
-from mazikeen.Utils import replaceVariables, ensure_dir, diffStrategy, diff
-from mazikeen.ConsolePrinter import Printer, BufferedPrinter
-
-
-class DiffBlock:
-    def __init__(self, paths, binarycompare  = False, strategy = diffStrategy.All, ignore = []):
-        assert len(paths) == 2
-        self.paths = paths
-        self.binarycompare = binarycompare
-        self.strategy = strategy
-        self.ignore = ignore
-
-    def run(self, workingDir ="", variables = {}, printer = Printer()):
-        printer.verbose("Diff:", self.paths)
-        _leftpath = replaceVariables(self.paths[0], variables, printer)
-        _rightpath = replaceVariables(self.paths[1], variables, printer)
-        _ignore = []
-        for ignoreLine in self.ignore:
-            _ignoreline = replaceVariables(ignoreLine, variables, printer)
-            _ignore.append(_ignoreline)
-        workingDirPath = pathlib.Path(workingDir)
-        return diff(workingDirPath.joinpath(_leftpath), workingDirPath.joinpath(_rightpath), self.binarycompare, self.strategy, _ignore, printer)
+import pathlib
+
+from mazikeen.Utils import replaceVariables, ensure_dir, diffStrategy, diff
+from mazikeen.ConsolePrinter import Printer, BufferedPrinter
+
+
+class DiffBlock:
+    def __init__(self, paths, binarycompare  = False, strategy = diffStrategy.All, ignore = []):
+        assert len(paths) == 2
+        self.paths = paths
+        self.binarycompare = binarycompare
+        self.strategy = strategy
+        self.ignore = ignore
+
+    def run(self, workingDir ="", variables = {}, printer = Printer()):
+        printer.verbose("Diff:", self.paths)
+        _leftpath = replaceVariables(self.paths[0], variables, printer)
+        _rightpath = replaceVariables(self.paths[1], variables, printer)
+        _ignore = []
+        for ignoreLine in self.ignore:
+            _ignoreline = replaceVariables(ignoreLine, variables, printer)
+            _ignore.append(_ignoreline)
+        workingDirPath = pathlib.Path(workingDir)
+        return diff(workingDirPath.joinpath(_leftpath), workingDirPath.joinpath(_rightpath), self.binarycompare, self.strategy, _ignore, printer)
```

### Comparing `mazikeen-1.2.7/mazikeen/GeneratorDiffBlock.py` & `mazikeen-1.2.8/mazikeen/GeneratorDiffBlock.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-import shlex
-
-from mazikeen.GeneratorUtils import getYamlString, getYamlInt, getYamlBool
-from mazikeen.GeneratorException import GeneratorException
-from mazikeen.DiffBlock import DiffBlock
-from mazikeen.Utils import diffStrategy
-from mazikeen.GeneratorUtils import getYamlString, getYamlList
-from mazikeen.ConsolePrinter import Printer, BufferedPrinter
-
-def _parseStrategy(data, line, field):
-    strStrat = getYamlString(data, line, field)
-    if not any(x for x in diffStrategy if x.name == strStrat):
-        raise GeneratorException(f"Invalid value '{strStrat}' for field '{field}' at line {line}")
-    
-    return diffStrategy[data]
-
-def _parseignore(data, line, field):
-    listignore = getYamlList(data, line, field)
-    for ignoreline in listignore:
-        if (not isinstance(ignoreline, str)):
-            raise GeneratorException(f"Field '{field}' expects a list of strings at line {line}")
-    return listignore
-
-def getYamlPaths(data, line = None, field = None):
-    if isinstance(data, str):
-        dirs = shlex.split(data)
-        if (len(dirs) == 2): 
-            return dirs
-    if (line and field):
-        raise GeneratorException(f"Field '{field}' expects two paths at line {line}")
-    else:
-        raise GeneratorException(f"'diff' block not recognized")
-
-def generateDiffBlock(data):
-    if isinstance(data, str):
-        return DiffBlock(paths = getYamlPaths(data))
-    if not isinstance(data, dict):
-        raise DiffBlock(f"'diff' block not recognized")
-    args = {}
-    key = ""
-    knownkeys = {'paths': lambda _data: getYamlPaths(_data, data['__line__'], key),
-                 'binarycompare': lambda _data: getYamlBool(_data, data['__line__'], key),
-                 'strategy': lambda _data: _parseStrategy(_data, data['__line__'], key),
-                 'ignore': lambda _data: _parseignore(_data, data['__line__'], key)}
-    for key in data:
-        if key == "__line__": continue
-        if not key.lower() in knownkeys.keys():
-            raise GeneratorException(f"Only one of the following keys are allowed: {[*knownkeys.keys()]} at line {data['__line__']}")
-        args[key.lower()] = knownkeys[key.lower()](data[key])
+import shlex
+
+from mazikeen.GeneratorUtils import getYamlString, getYamlInt, getYamlBool
+from mazikeen.GeneratorException import GeneratorException
+from mazikeen.DiffBlock import DiffBlock
+from mazikeen.Utils import diffStrategy
+from mazikeen.GeneratorUtils import getYamlString, getYamlList
+from mazikeen.ConsolePrinter import Printer, BufferedPrinter
+
+def _parseStrategy(data, line, field):
+    strStrat = getYamlString(data, line, field)
+    if not any(x for x in diffStrategy if x.name == strStrat):
+        raise GeneratorException(f"Invalid value '{strStrat}' for field '{field}' at line {line}")
+    
+    return diffStrategy[data]
+
+def _parseignore(data, line, field):
+    listignore = getYamlList(data, line, field)
+    for ignoreline in listignore:
+        if (not isinstance(ignoreline, str)):
+            raise GeneratorException(f"Field '{field}' expects a list of strings at line {line}")
+    return listignore
+
+def getYamlPaths(data, line = None, field = None):
+    if isinstance(data, str):
+        dirs = shlex.split(data)
+        if (len(dirs) == 2): 
+            return dirs
+    if (line and field):
+        raise GeneratorException(f"Field '{field}' expects two paths at line {line}")
+    else:
+        raise GeneratorException(f"'diff' block not recognized")
+
+def generateDiffBlock(data):
+    if isinstance(data, str):
+        return DiffBlock(paths = getYamlPaths(data))
+    if not isinstance(data, dict):
+        raise DiffBlock(f"'diff' block not recognized")
+    args = {}
+    key = ""
+    knownkeys = {'paths': lambda _data: getYamlPaths(_data, data['__line__'], key),
+                 'binarycompare': lambda _data: getYamlBool(_data, data['__line__'], key),
+                 'strategy': lambda _data: _parseStrategy(_data, data['__line__'], key),
+                 'ignore': lambda _data: _parseignore(_data, data['__line__'], key)}
+    for key in data:
+        if key == "__line__": continue
+        if not key.lower() in knownkeys.keys():
+            raise GeneratorException(f"Only one of the following keys are allowed: {[*knownkeys.keys()]} at line {data['__line__']}")
+        args[key.lower()] = knownkeys[key.lower()](data[key])
     return DiffBlock(**args)
```

### Comparing `mazikeen-1.2.7/mazikeen/GeneratorLooper.py` & `mazikeen-1.2.8/mazikeen/GeneratorLooper.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-import itertools
-
-from mazikeen.Loopers import Serial, Parallel
-from mazikeen.GeneratorException import GeneratorException
-from mazikeen.GeneratorRunBlock import generateRunBlock
-from mazikeen.GeneratorMakedirs import generateMakedirs
-from mazikeen.GeneratorRmdir import generateRmdir
-from mazikeen.GeneratorDiffBlock import generateDiffBlock
-from mazikeen.GeneratorUtils import getYamlInt, getYamlBool
-from mazikeen.ConsolePrinter import Printer, BufferedPrinter
-
-def _getVariables(data):
-    dictVar = {}
-    for key in data:
-        if key == "__line__": continue
-        dictVar[key] = data[key]
-    return dictVar
-def _dict_product(dicts):
-    return (dict(zip(dicts, x)) for x in itertools.product(*dicts.values()))
-def __dict_zip_longest(dicts):
-    return (dict(zip(dicts, x)) for x in itertools.zip_longest(*dicts.values()))
-def _dict_zip(dicts):
-    return (dict(zip(dicts, x)) for x in zip(*dicts.values()))
-def _parseProduct(data):
-    dictVar = _getVariables(data)
-    return _dict_product(dictVar)
-def _parseZip(data):
-    dictVar = _getVariables(data)
-    for curDic in __dict_zip_longest(dictVar):
-        yield { k:v for k, v in curDic.items() if v }
-def _parseEntries(data):
-    if data == None: return []
-    knownkeys = {'product':_parseProduct, 'zip':_parseZip}
-    entries = []
-    for key in data:
-        if key == "__line__": continue
-        if not key.lower() in knownkeys.keys():
-            raise GeneratorException(f"Only one of the following keys are allowed: {[*knownkeys.keys()]} at line {data['__line__']}")
-        entries.extend(knownkeys[key](data[key]))
-    return entries
-def _parseSteps(data, line):
-    steps = list()
-    knownkeys = {'serial':generateSerialBlock, 
-                 'parallel':generateParallelBlock, 
-                 'run':generateRunBlock,
-                 'diff':generateDiffBlock,
-                 'makedirs':generateMakedirs,
-                 'rmdir':generateRmdir}
-    for yamlSteps in data:
-        for key in yamlSteps:
-            if key == "__line__": continue
-            if not key.lower() in knownkeys.keys():
-                if (isinstance(data, dict)):
-                    raise GeneratorException(f"Error: Key '{key}' not allowed. Only one of the following keys are allowed :{[*knownkeys.keys()]} at line {data['__line__']}")
-                else:
-                    raise GeneratorException(f"Error: Key '{key}' not allowed. Only one of the following keys are allowed :{[*knownkeys.keys()]} at line {line}")
-            steps.append(knownkeys[key.lower()](yamlSteps[key]))
-    return steps
-def generateSerialBlock(data):
-    if data == None: return
-    args = {}
-    knownkeys = {'entries': lambda data: list(_parseEntries(data)),
-                 'failfast': lambda _data: getYamlBool(_data, data['__line__'], key),
-                 'steps': lambda _data: list(_parseSteps(_data, data['__line__']))}
-    for key in data:
-        if key == "__line__": continue
-        if not key.lower() in knownkeys.keys():
-            raise GeneratorException(f"Only one of the following keys are allowed: {[*knownkeys.keys()]} at line {data['__line__']}")
-        args[key.lower()] = knownkeys[key.lower()](data[key])
-    return Serial(**args)
-
-def generateParallelBlock(data):
-    args = {}
-    key = ""
-    knownkeys = {'entries': lambda data: list(_parseEntries(data)), 
-                 'steps': lambda _data: list(_parseSteps(_data, data['__line__'])),
-                 'failfast': lambda _data: getYamlBool(_data, data['__line__'], key),
-                 'max_workers': lambda _data: getYamlInt(_data, data['__line__'], key)}
-    for key in data:
-        if key == "__line__": continue
-        if not key.lower() in knownkeys.keys():
-            raise GeneratorException(f"Only one of the following keys are allowed: {[*knownkeys.keys()]} at line {data['__line__']}")
-        args[key.lower()] = knownkeys[key.lower()](data[key])
+import itertools
+
+from mazikeen.Loopers import Serial, Parallel
+from mazikeen.GeneratorException import GeneratorException
+from mazikeen.GeneratorRunBlock import generateRunBlock
+from mazikeen.GeneratorMakedirs import generateMakedirs
+from mazikeen.GeneratorRmdir import generateRmdir
+from mazikeen.GeneratorDiffBlock import generateDiffBlock
+from mazikeen.GeneratorUtils import getYamlInt, getYamlBool
+from mazikeen.ConsolePrinter import Printer, BufferedPrinter
+
+def _getVariables(data):
+    dictVar = {}
+    for key in data:
+        if key == "__line__": continue
+        dictVar[key] = data[key]
+    return dictVar
+def _dict_product(dicts):
+    return (dict(zip(dicts, x)) for x in itertools.product(*dicts.values()))
+def __dict_zip_longest(dicts):
+    return (dict(zip(dicts, x)) for x in itertools.zip_longest(*dicts.values()))
+def _dict_zip(dicts):
+    return (dict(zip(dicts, x)) for x in zip(*dicts.values()))
+def _parseProduct(data):
+    dictVar = _getVariables(data)
+    return _dict_product(dictVar)
+def _parseZip(data):
+    dictVar = _getVariables(data)
+    for curDic in __dict_zip_longest(dictVar):
+        yield { k:v for k, v in curDic.items() if v }
+def _parseEntries(data):
+    if data == None: return []
+    knownkeys = {'product':_parseProduct, 'zip':_parseZip}
+    entries = []
+    for key in data:
+        if key == "__line__": continue
+        if not key.lower() in knownkeys.keys():
+            raise GeneratorException(f"Only one of the following keys are allowed: {[*knownkeys.keys()]} at line {data['__line__']}")
+        entries.extend(knownkeys[key](data[key]))
+    return entries
+def _parseSteps(data, line):
+    steps = list()
+    knownkeys = {'serial':generateSerialBlock, 
+                 'parallel':generateParallelBlock, 
+                 'run':generateRunBlock,
+                 'diff':generateDiffBlock,
+                 'makedirs':generateMakedirs,
+                 'rmdir':generateRmdir}
+    for yamlSteps in data:
+        for key in yamlSteps:
+            if key == "__line__": continue
+            if not key.lower() in knownkeys.keys():
+                if (isinstance(data, dict)):
+                    raise GeneratorException(f"Error: Key '{key}' not allowed. Only one of the following keys are allowed :{[*knownkeys.keys()]} at line {data['__line__']}")
+                else:
+                    raise GeneratorException(f"Error: Key '{key}' not allowed. Only one of the following keys are allowed :{[*knownkeys.keys()]} at line {line}")
+            steps.append(knownkeys[key.lower()](yamlSteps[key]))
+    return steps
+def generateSerialBlock(data):
+    if data == None: return
+    args = {}
+    knownkeys = {'entries': lambda data: list(_parseEntries(data)),
+                 'failfast': lambda _data: getYamlBool(_data, data['__line__'], key),
+                 'steps': lambda _data: list(_parseSteps(_data, data['__line__']))}
+    for key in data:
+        if key == "__line__": continue
+        if not key.lower() in knownkeys.keys():
+            raise GeneratorException(f"Only one of the following keys are allowed: {[*knownkeys.keys()]} at line {data['__line__']}")
+        args[key.lower()] = knownkeys[key.lower()](data[key])
+    return Serial(**args)
+
+def generateParallelBlock(data):
+    args = {}
+    key = ""
+    knownkeys = {'entries': lambda data: list(_parseEntries(data)), 
+                 'steps': lambda _data: list(_parseSteps(_data, data['__line__'])),
+                 'failfast': lambda _data: getYamlBool(_data, data['__line__'], key),
+                 'max_workers': lambda _data: getYamlInt(_data, data['__line__'], key)}
+    for key in data:
+        if key == "__line__": continue
+        if not key.lower() in knownkeys.keys():
+            raise GeneratorException(f"Only one of the following keys are allowed: {[*knownkeys.keys()]} at line {data['__line__']}")
+        args[key.lower()] = knownkeys[key.lower()](data[key])
     return Parallel(**args)
```

### Comparing `mazikeen-1.2.7/mazikeen/GeneratorRunBlock.py` & `mazikeen-1.2.8/mazikeen/GeneratorRunBlock.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from mazikeen.GeneratorUtils import getYamlString, getYamlInt
-from mazikeen.RunBlock import RunBlock
-from mazikeen.GeneratorException import GeneratorException
-
-def generateRunBlock(data):
-    if isinstance(data, str):
-        return RunBlock(cmd = data)
-    if not isinstance(data, dict):
-        raise GeneratorException(f"'run' block not recognized")
-    args = {}
-    key = ""
-    knownkeys = {'cmd': lambda _data: getYamlString(_data, data['__line__'], key), 
-                 'outputfile': lambda _data: getYamlString(_data, data['__line__'], key),
-                 'inputfile': lambda _data: getYamlString(_data, data['__line__'], key),
-                 'exitcode': lambda _data: getYamlInt(_data, data['__line__'], key),
-                 'shell': lambda _data: getYamlString(_data, data['__line__'], key)}
-    for key in data:
-        if key == "__line__": continue
-        if not key.lower() in knownkeys.keys():
-            raise GeneratorException(f"Only one of the following keys are allowed: {[*knownkeys.keys()]} at line {data['__line__']}")
-        args[key.lower()] = knownkeys[key.lower()](data[key])
+from mazikeen.GeneratorUtils import getYamlString, getYamlInt
+from mazikeen.RunBlock import RunBlock
+from mazikeen.GeneratorException import GeneratorException
+
+def generateRunBlock(data):
+    if isinstance(data, str):
+        return RunBlock(cmd = data)
+    if not isinstance(data, dict):
+        raise GeneratorException(f"'run' block not recognized")
+    args = {}
+    key = ""
+    knownkeys = {'cmd': lambda _data: getYamlString(_data, data['__line__'], key), 
+                 'outputfile': lambda _data: getYamlString(_data, data['__line__'], key),
+                 'inputfile': lambda _data: getYamlString(_data, data['__line__'], key),
+                 'exitcode': lambda _data: getYamlInt(_data, data['__line__'], key),
+                 'shell': lambda _data: getYamlString(_data, data['__line__'], key)}
+    for key in data:
+        if key == "__line__": continue
+        if not key.lower() in knownkeys.keys():
+            raise GeneratorException(f"Only one of the following keys are allowed: {[*knownkeys.keys()]} at line {data['__line__']}")
+        args[key.lower()] = knownkeys[key.lower()](data[key])
     return RunBlock(**args)
```

### Comparing `mazikeen-1.2.7/mazikeen/GeneratorUtils.py` & `mazikeen-1.2.8/mazikeen/GeneratorUtils.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from mazikeen.GeneratorException import GeneratorException
-
-def getYamlInt(data, line, field):
-    if data == None: return None
-    if (not isinstance(data, int)):
-        if (isinstance(data, dict)):
-            raise GeneratorException(f"field '{field}' expects an integer at line {data['__line__']}")
-        raise GeneratorException(f"field '{field}' expects an integer at line {line}")
-
-    return data
-
-def getYamlBool(data, line, field):
-    if (not isinstance(data, bool)):
-        if (isinstance(data, dict)):
-            raise GeneratorException(f"field '{field}' expects a bool at line {data['__line__']}")
-        raise GeneratorException(f"field '{field}' expects a bool at line {line}")
-    return data
-
-def getYamlString(data, line, field):
-    if (not isinstance(data, str)):
-        if (isinstance(data, dict)):
-            raise GeneratorException(f"field '{field}' expects an integer at line {data['__line__']}")
-        raise GeneratorException(f"field '{field}' expects a string at line {line}")
-    return data
-
-def getYamlList(data, line, field):
-    if (not isinstance(data, list)):
-        if (isinstance(data, dict)):
-            raise GeneratorException(f"field '{field}' expects a list at line {data['__line__']}")
-        raise GeneratorException(f"field '{field}' expects a list at line {line}")
+from mazikeen.GeneratorException import GeneratorException
+
+def getYamlInt(data, line, field):
+    if data == None: return None
+    if (not isinstance(data, int)):
+        if (isinstance(data, dict)):
+            raise GeneratorException(f"field '{field}' expects an integer at line {data['__line__']}")
+        raise GeneratorException(f"field '{field}' expects an integer at line {line}")
+
+    return data
+
+def getYamlBool(data, line, field):
+    if (not isinstance(data, bool)):
+        if (isinstance(data, dict)):
+            raise GeneratorException(f"field '{field}' expects a bool at line {data['__line__']}")
+        raise GeneratorException(f"field '{field}' expects a bool at line {line}")
+    return data
+
+def getYamlString(data, line, field):
+    if (not isinstance(data, str)):
+        if (isinstance(data, dict)):
+            raise GeneratorException(f"field '{field}' expects an integer at line {data['__line__']}")
+        raise GeneratorException(f"field '{field}' expects a string at line {line}")
+    return data
+
+def getYamlList(data, line, field):
+    if (not isinstance(data, list)):
+        if (isinstance(data, dict)):
+            raise GeneratorException(f"field '{field}' expects a list at line {data['__line__']}")
+        raise GeneratorException(f"field '{field}' expects a list at line {line}")
     return data
```

### Comparing `mazikeen-1.2.7/mazikeen/RunBlock.py` & `mazikeen-1.2.8/mazikeen/RunBlock.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,175 +1,175 @@
-import shlex
-import subprocess
-import os
-import pathlib
-import sys
-import platform
-import threading
-
-from mazikeen.ConsolePrinter import Printer
-from mazikeen.Utils import replaceVariables, ensure_dir
-
-__pythonPath = None
-__pythonPath3 = None
-__searchedForPython = False
-__searchedForPythonLock = threading.Lock()
-
-class RunBlock:
-    def __init__(self, cmd, outputfile = None, inputfile = None, exitcode = None, shell = None):
-        self.cmd = cmd
-        self.outputfile = outputfile
-        self.inputfile = inputfile
-        self.exitcode = exitcode
-        self.shell = shell
-        
-    def run(self, workingDir = ".", variables = {}, printer = Printer()):
-
-        printer.verbose("Run:", self.cmd)
-        replCmd = replaceVariables(self.cmd, variables)
-        printer.verbose("cwd:", os.path.abspath(workingDir))
-        printer.verbose("call:", replCmd)
-        cmdNArgs = shlex.split(replCmd)
-
-        if self.shell == "powershell": return self.__run_powershell(replCmd, workingDir, variables, printer)
-        elif self.shell == "cmd": return self.__run_cmd(replCmd, workingDir, variables, printer)
-        elif self.shell == "sh": return self.__run_sh(replCmd, workingDir, variables, printer)
-        elif self.shell == "python": return self.__run_pythonX(replCmd, "python", workingDir, variables, printer)
-        elif self.shell == "python3": return self.__run_pythonX(replCmd, "python3", workingDir, variables, printer)
-        elif self.shell != None: 
-            printer.error("unknown shell ", self.shell)
-            return false;
-
-        inputfileData = None
-        if self.inputfile:
-            with open(pathlib.PurePath(workingDir).joinpath(replaceVariables(self.inputfile, variables)), "rb") as fh:
-                inputfileData = fh.read()
-        shell = (sys.platform == "win32")
-        subProcessRes = subprocess.run(cmdNArgs, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, input=inputfileData, cwd = workingDir, shell = shell)
-        if self.outputfile:
-            outputfileFullPath = str(pathlib.PurePath(workingDir).joinpath(replaceVariables(self.outputfile, variables)))
-            ensure_dir(outputfileFullPath)
-            with open(outputfileFullPath, "wb") as fh:
-                fh.write(subProcessRes.stdout)
-        
-        res = True
-        if (self.exitcode != None):
-            res = subProcessRes.returncode == self.exitcode
-            if not res:
-                printer.error("different exitcode received:", subProcessRes.returncode, "!=", self.exitcode, "for command '"+ str(replCmd) +"'")
-        return res
-
-    def __run_powershell(self, replCmd, workingDir = ".", variables = {}, printer = Printer()):
-        if self.inputfile:
-            printer.error("inputfile not allowed when shell = ", self.shell)
-            return false;
-        inputData = str.encode(replCmd)
-        subProcessRes = subprocess.run(["powershell", "-NonInteractive", "-NoLogo"], stdout=subprocess.PIPE, stderr=subprocess.STDOUT, input=inputData, cwd = workingDir, shell = False)
-        if self.outputfile:
-            outputfileFullPath = str(pathlib.PurePath(workingDir).joinpath(replaceVariables(self.outputfile, variables)))
-            ensure_dir(outputfileFullPath)
-            with open(outputfileFullPath, "wb") as fh:
-                fh.write(subProcessRes.stdout)
-
-        res = True
-        if (self.exitcode != None):
-            res = subProcessRes.returncode == self.exitcode
-            if not res:
-                printer.error("different exitcode received:", subProcessRes.returncode, "!=", self.exitcode, "for command '"+ str(replCmd) +"'")
-        return res
-
-    def __run_pythonX(self, replCmd, pythonType = "python3", workingDir = ".", variables = {}, printer = Printer()):
-        pythonPath = getPythonPath(pythonType)
-        if pythonPath == None:
-            printer.error(f"{pythonType} could not be found")
-            return false;
-        if self.inputfile:
-            printer.error("inputfile not allowed when shell = ", self.shell)
-            return false;
-        inputData = str.encode(replCmd)
-        subProcessRes = subprocess.run([pythonPath], stdout=subprocess.PIPE, stderr=subprocess.STDOUT, input=inputData, cwd = workingDir, shell = False)
-        if self.outputfile:
-            outputfileFullPath = str(pathlib.PurePath(workingDir).joinpath(replaceVariables(self.outputfile, variables)))
-            ensure_dir(outputfileFullPath)
-            with open(outputfileFullPath, "wb") as fh:
-                fh.write(subProcessRes.stdout)
-
-        res = True
-        if (self.exitcode != None):
-            res = subProcessRes.returncode == self.exitcode
-            if not res:
-                printer.error("different exitcode received:", subProcessRes.returncode, "!=", self.exitcode, "for command '"+ str(replCmd) +"'")
-        return res
-
-    def __run_sh(self, replCmd, workingDir = ".", variables = {}, printer = Printer()):
-        if self.inputfile:
-            printer.error("inputfile not allowed when shell = ", self.shell)
-            return false;
-        inputData = str.encode(replCmd)
-        subProcessRes = subprocess.run(["sh"], stdout=subprocess.PIPE, stderr=subprocess.STDOUT, input=inputData, cwd = workingDir, shell = False)
-        if self.outputfile:
-            outputfileFullPath = str(pathlib.PurePath(workingDir).joinpath(replaceVariables(self.outputfile, variables)))
-            ensure_dir(outputfileFullPath)
-            with open(outputfileFullPath, "wb") as fh:
-                fh.write(subProcessRes.stdout)
-
-        res = True
-        if (self.exitcode != None):
-            res = subProcessRes.returncode == self.exitcode
-            if not res:
-                printer.error("different exitcode received:", subProcessRes.returncode, "!=", self.exitcode, "for command '"+ str(replCmd) +"'")
-        return res
-
-    def __run_cmd(self, replCmd, workingDir = ".", variables = {}, printer = Printer()):
-        if self.inputfile:
-            printer.error("inputfile not allowed when shell = ", self.shell)
-            return false;
-
-        if replCmd.endswith("/n"): 
-            inputData = str.encode(replCmd)
-        else: 
-            inputData = str.encode(replCmd + "\n")
-        
-        subProcessRes = subprocess.run(["cmd"], stdout=subprocess.PIPE, stderr=subprocess.STDOUT, input=inputData, cwd = workingDir, shell = False)
-        if self.outputfile:
-            outputfileFullPath = str(pathlib.PurePath(workingDir).joinpath(replaceVariables(self.outputfile, variables)))
-            ensure_dir(outputfileFullPath)
-            with open(outputfileFullPath, "wb") as fh:
-                fh.write(subProcessRes.stdout)
-
-        res = True
-        if (self.exitcode != None):
-            res = subProcessRes.returncode == self.exitcode
-            if not res:
-                printer.error("different exitcode received:", subProcessRes.returncode, "!=", self.exitcode, "for command '"+ str(replCmd) +"'")
-        return res
-
-def getPythonPath(pythonType):
-    with __searchedForPythonLock:
-        if __searchedForPython == False:
-            if platform.system().lower() == "windows":
-                process = subprocess.run(["where", "python"], stdout=subprocess.PIPE, shell = False)
-                pythonPaths = process.stdout.decode("utf-8").split("\r\n")
-                pythonPaths = list(filter (("").__ne__, pythonPaths))
-                for pythonPath in pythonPaths:
-                    process = subprocess.run([pythonPath, "--version"], stdout=subprocess.PIPE, stderr=subprocess.STDOUT, shell = False)
-                    pythonVersion = process.stdout.decode("utf-8")
-                    if pythonVersion.startswith("Python 3"):
-                        __pythonPath3 = pythonPath
-                    elif pythonVersion.startswith("Python 2"):
-                        __pythonPath = pythonPath
-            if platform.system().lower() == "linux":
-                process = subprocess.run(["which", "python"], stdout=subprocess.PIPE, shell = False)
-                pythonPaths = process.stdout.decode("utf-8").split("\n")
-                process = subprocess.run(["which", "python3"], stdout=subprocess.PIPE, shell = False)
-                pythonPaths.extend(process.stdout.decode("utf-8").split("\n"))
-                pythonPaths = list(filter (("").__ne__, pythonPaths))
-                for pythonPath in pythonPaths:
-                    process = subprocess.run([pythonPath, "--version"], stdout=subprocess.PIPE, stderr=subprocess.STDOUT, shell = False)
-                    pythonVersion = process.stdout.decode("utf-8")
-                    if pythonVersion.startswith("Python 3"):
-                        __pythonPath3 = pythonPath
-                    elif pythonVersion.startswith("Python 2"):
-                        __pythonPath = pythonPath
-        if pythonType == "python": return __pythonPath
-        elif pythonType == "python3": return __pythonPath3
+import shlex
+import subprocess
+import os
+import pathlib
+import sys
+import platform
+import threading
+
+from mazikeen.ConsolePrinter import Printer
+from mazikeen.Utils import replaceVariables, ensure_dir
+
+__pythonPath = None
+__pythonPath3 = None
+__searchedForPython = False
+__searchedForPythonLock = threading.Lock()
+
+class RunBlock:
+    def __init__(self, cmd, outputfile = None, inputfile = None, exitcode = None, shell = None):
+        self.cmd = cmd
+        self.outputfile = outputfile
+        self.inputfile = inputfile
+        self.exitcode = exitcode
+        self.shell = shell
+        
+    def run(self, workingDir = ".", variables = {}, printer = Printer()):
+
+        printer.verbose("Run:", self.cmd)
+        replCmd = replaceVariables(self.cmd, variables)
+        printer.verbose("cwd:", os.path.abspath(workingDir))
+        printer.verbose("call:", replCmd)
+        cmdNArgs = shlex.split(replCmd)
+
+        if self.shell == "powershell": return self.__run_powershell(replCmd, workingDir, variables, printer)
+        elif self.shell == "cmd": return self.__run_cmd(replCmd, workingDir, variables, printer)
+        elif self.shell == "sh": return self.__run_sh(replCmd, workingDir, variables, printer)
+        elif self.shell == "python": return self.__run_pythonX(replCmd, "python", workingDir, variables, printer)
+        elif self.shell == "python3": return self.__run_pythonX(replCmd, "python3", workingDir, variables, printer)
+        elif self.shell != None: 
+            printer.error("unknown shell ", self.shell)
+            return false;
+
+        inputfileData = None
+        if self.inputfile:
+            with open(pathlib.PurePath(workingDir).joinpath(replaceVariables(self.inputfile, variables)), "rb") as fh:
+                inputfileData = fh.read()
+        shell = (sys.platform == "win32")
+        subProcessRes = subprocess.run(cmdNArgs, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, input=inputfileData, cwd = workingDir, shell = shell)
+        if self.outputfile:
+            outputfileFullPath = str(pathlib.PurePath(workingDir).joinpath(replaceVariables(self.outputfile, variables)))
+            ensure_dir(outputfileFullPath)
+            with open(outputfileFullPath, "wb") as fh:
+                fh.write(subProcessRes.stdout)
+        
+        res = True
+        if (self.exitcode != None):
+            res = subProcessRes.returncode == self.exitcode
+            if not res:
+                printer.error("different exitcode received:", subProcessRes.returncode, "!=", self.exitcode, "for command '"+ str(replCmd) +"'")
+        return res
+
+    def __run_powershell(self, replCmd, workingDir = ".", variables = {}, printer = Printer()):
+        if self.inputfile:
+            printer.error("inputfile not allowed when shell = ", self.shell)
+            return false;
+        inputData = str.encode(replCmd)
+        subProcessRes = subprocess.run(["powershell", "-NonInteractive", "-NoLogo"], stdout=subprocess.PIPE, stderr=subprocess.STDOUT, input=inputData, cwd = workingDir, shell = False)
+        if self.outputfile:
+            outputfileFullPath = str(pathlib.PurePath(workingDir).joinpath(replaceVariables(self.outputfile, variables)))
+            ensure_dir(outputfileFullPath)
+            with open(outputfileFullPath, "wb") as fh:
+                fh.write(subProcessRes.stdout)
+
+        res = True
+        if (self.exitcode != None):
+            res = subProcessRes.returncode == self.exitcode
+            if not res:
+                printer.error("different exitcode received:", subProcessRes.returncode, "!=", self.exitcode, "for command '"+ str(replCmd) +"'")
+        return res
+
+    def __run_pythonX(self, replCmd, pythonType = "python3", workingDir = ".", variables = {}, printer = Printer()):
+        pythonPath = getPythonPath(pythonType)
+        if pythonPath == None:
+            printer.error(f"{pythonType} could not be found")
+            return false;
+        if self.inputfile:
+            printer.error("inputfile not allowed when shell = ", self.shell)
+            return false;
+        inputData = str.encode(replCmd)
+        subProcessRes = subprocess.run([pythonPath], stdout=subprocess.PIPE, stderr=subprocess.STDOUT, input=inputData, cwd = workingDir, shell = False)
+        if self.outputfile:
+            outputfileFullPath = str(pathlib.PurePath(workingDir).joinpath(replaceVariables(self.outputfile, variables)))
+            ensure_dir(outputfileFullPath)
+            with open(outputfileFullPath, "wb") as fh:
+                fh.write(subProcessRes.stdout)
+
+        res = True
+        if (self.exitcode != None):
+            res = subProcessRes.returncode == self.exitcode
+            if not res:
+                printer.error("different exitcode received:", subProcessRes.returncode, "!=", self.exitcode, "for command '"+ str(replCmd) +"'")
+        return res
+
+    def __run_sh(self, replCmd, workingDir = ".", variables = {}, printer = Printer()):
+        if self.inputfile:
+            printer.error("inputfile not allowed when shell = ", self.shell)
+            return false;
+        inputData = str.encode(replCmd)
+        subProcessRes = subprocess.run(["sh"], stdout=subprocess.PIPE, stderr=subprocess.STDOUT, input=inputData, cwd = workingDir, shell = False)
+        if self.outputfile:
+            outputfileFullPath = str(pathlib.PurePath(workingDir).joinpath(replaceVariables(self.outputfile, variables)))
+            ensure_dir(outputfileFullPath)
+            with open(outputfileFullPath, "wb") as fh:
+                fh.write(subProcessRes.stdout)
+
+        res = True
+        if (self.exitcode != None):
+            res = subProcessRes.returncode == self.exitcode
+            if not res:
+                printer.error("different exitcode received:", subProcessRes.returncode, "!=", self.exitcode, "for command '"+ str(replCmd) +"'")
+        return res
+
+    def __run_cmd(self, replCmd, workingDir = ".", variables = {}, printer = Printer()):
+        if self.inputfile:
+            printer.error("inputfile not allowed when shell = ", self.shell)
+            return false;
+
+        if replCmd.endswith("/n"): 
+            inputData = str.encode(replCmd)
+        else: 
+            inputData = str.encode(replCmd + "\n")
+        
+        subProcessRes = subprocess.run(["cmd"], stdout=subprocess.PIPE, stderr=subprocess.STDOUT, input=inputData, cwd = workingDir, shell = False)
+        if self.outputfile:
+            outputfileFullPath = str(pathlib.PurePath(workingDir).joinpath(replaceVariables(self.outputfile, variables)))
+            ensure_dir(outputfileFullPath)
+            with open(outputfileFullPath, "wb") as fh:
+                fh.write(subProcessRes.stdout)
+
+        res = True
+        if (self.exitcode != None):
+            res = subProcessRes.returncode == self.exitcode
+            if not res:
+                printer.error("different exitcode received:", subProcessRes.returncode, "!=", self.exitcode, "for command '"+ str(replCmd) +"'")
+        return res
+
+def getPythonPath(pythonType):
+    with __searchedForPythonLock:
+        if __searchedForPython == False:
+            if platform.system().lower() == "windows":
+                process = subprocess.run(["where", "python"], stdout=subprocess.PIPE, shell = False)
+                pythonPaths = process.stdout.decode("utf-8").split("\r\n")
+                pythonPaths = list(filter (("").__ne__, pythonPaths))
+                for pythonPath in pythonPaths:
+                    process = subprocess.run([pythonPath, "--version"], stdout=subprocess.PIPE, stderr=subprocess.STDOUT, shell = False)
+                    pythonVersion = process.stdout.decode("utf-8")
+                    if pythonVersion.startswith("Python 3"):
+                        __pythonPath3 = pythonPath
+                    elif pythonVersion.startswith("Python 2"):
+                        __pythonPath = pythonPath
+            if platform.system().lower() == "linux":
+                process = subprocess.run(["which", "python"], stdout=subprocess.PIPE, shell = False)
+                pythonPaths = process.stdout.decode("utf-8").split("\n")
+                process = subprocess.run(["which", "python3"], stdout=subprocess.PIPE, shell = False)
+                pythonPaths.extend(process.stdout.decode("utf-8").split("\n"))
+                pythonPaths = list(filter (("").__ne__, pythonPaths))
+                for pythonPath in pythonPaths:
+                    process = subprocess.run([pythonPath, "--version"], stdout=subprocess.PIPE, stderr=subprocess.STDOUT, shell = False)
+                    pythonVersion = process.stdout.decode("utf-8")
+                    if pythonVersion.startswith("Python 3"):
+                        __pythonPath3 = pythonPath
+                    elif pythonVersion.startswith("Python 2"):
+                        __pythonPath = pythonPath
+        if pythonType == "python": return __pythonPath
+        elif pythonType == "python3": return __pythonPath3
         return None
```

### Comparing `mazikeen-1.2.7/mazikeen/ScriptDataProcessor.py` & `mazikeen-1.2.8/mazikeen/ScriptDataProcessor.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,195 +1,195 @@
-import copy
-import yaml
-from yaml.loader import SafeLoader
-
-from mazikeen.ConsolePrinter import Printer
-
-class SafeLineLoader(SafeLoader):
-    def construct_mapping(self, node, deep=False):
-        mapping = super(SafeLineLoader, self).construct_mapping(node, deep=deep)
-        # Add 1 so line numbering starts at 1
-        mapping['__line__'] = node.start_mark.line + 1
-        return mapping
-
-class Version():
-    def __init__(self, versionStr): 
-        (self.major, self.minor, self.patch) = ("", "", "")
-        if versionStr == None or versionStr == "": 
-            return
-
-        versionTupl = versionStr.split('.')
-        if len(versionTupl) > 3: 
-            raise Exception("Invalid version. Version is too long")
-        try:
-            if len(versionTupl) >= 1: 
-                self.major = int(versionTupl[0])
-            if len(versionTupl) >= 2: 
-                self.minor = int(versionTupl[1])
-            if len(versionTupl) == 3: 
-                self.patch = int(versionTupl[2])
-        except ValueError as e:
-            raise ValueError("Invalid version. Version may only contain numbers")
-
-    def __hash__(self):
-        return self.major * 10000 + self.minor * 100 + self.patch
-
-    def __eq__(self, other):
-        return (self.major == self.major and
-                self.minor == self.minor and
-                self.patch == self.patch)
-
-    def __lt__(self, other):
-        if self.major == "" and other.major != "": return True;
-        if self.major < other.major: return True;
-        if self.minor == "" and other.minor != "": return True;
-        if self.minor < other.minor: return True;
-        if self.patch == "" and other.patch != "": return True;
-        if self.patch < other.patch: return True;
-
-    def __str__(self):
-        return f"{str(self.major)}.{str(self.minor)}.{str(self.patch)}"
-
-
-def __upgradeScript1_0_0(data):
-    def fixDiffBlock(data):
-        if not isinstance(data, dict): 
-            return data
-        leftpath = ""
-        rightpath = ""
-        leftpathkey = None
-        rightpathkey = None
-        for key in data:
-            if key.lower() == "leftpath":
-                leftpath = data[key]
-                leftpathkey = key
-            elif key.lower() == "rightpath":
-                rightpath = data[key]
-                rightpathkey = key
-        if leftpathkey: data.pop(leftpathkey, None)
-        if rightpathkey: data.pop(rightpathkey, None)
-        if (leftpath == "" and rightpath == ""):
-            return data
-        data["paths"] = "\"" + leftpath + "\" \"" + rightpath + "\""
-        return data
-    
-    def fixRunBlock(data):
-        if isinstance(data, str):
-            return {'__line__': -1, 'cmd' : data, 'exitcode': 0}
-        if not isinstance(data, dict): 
-            return data
-        for key in data:
-            exitcode = None
-            if key.lower() == "exitCode":
-                exitcode = data[key]
-        if exitcode == None:
-            data["exitcode"] = 0
-        return data
-
-    def fixLooperData(data):
-        for key in data:
-            if key.lower() == "steps":
-                fixStepsData(data[key])
-
-    def fixStepsData(data):
-        if data == None: return
-        if not isinstance(data, list): 
-            raise Exception("Scriptfile can not be upgraded")
-
-        for step in data:
-            for key in step:
-                if key.lower() == "steps":
-                    fixStepsData(step[key])
-                if key.lower() == "run":
-                    step[key] = fixRunBlock(step[key])
-                if key.lower() == "diff":
-                    step[key] = fixDiffBlock(step[key])
-
-    data["version"]="1.1.0"
-    fixLooperData(data)
-    return (data, Version("1.1.0"))
-
-def __upgradeScript1_1_0(data):
-    def fixLooperData(data):
-        for key in data:
-            if key.lower() == "steps":
-                fixStepsData(data[key])
-
-    def fixStepsData(data):
-        if data == None: return
-        if not isinstance(data, list): 
-            raise Exception("Scriptfile can not be upgraded")
-
-        for step in data:
-            for key in step:
-                if key.lower() == "steps":
-                    fixStepsData(step[key])
-                if key.lower() == "diff":
-                    step[key] = fixDiffBlock(step[key])
-                if key.lower() == "run":
-                    step[key] = fixRunBlock(step[key])
-
-    def fixRunBlock(data):
-        if not isinstance(data, dict): 
-            return data
-        for key in data:
-            if key.lower() == "exitcode":
-                if data[key] == 'None':
-                    data.pop(key, None)
-                break
-        return data
-
-    def fixDiffBlock(data):
-        if not isinstance(data, dict): 
-            return data
-        for key in data:
-            if key.lower() == "ignorelines":
-                data['ignore'] = data[key]
-                data.pop(key, None)
-                break
-        return data
-
-    data["version"]="1.2.0"
-    fixLooperData(data)
-    return (data, Version("1.2.0"))
-
-__upgradeDic = {Version("1.0.0"): __upgradeScript1_0_0,
-                Version("1.1.0"): __upgradeScript1_1_0,}
-__workingVersion = Version("1.2.0")
-
-def __upgradeScriptData(data_, printer):
-    if data_ == None: return (False, data_)
-    data = data_.copy()
-
-    upgraded = False
-    currentVersion = Version(data.get("version", str(__workingVersion)))
-    if (currentVersion < __workingVersion): 
-        printer.verbose(f"Warning: script file needs to be upgraded to version: {str(__workingVersion)}. Use --upgradeScriptFile to save upgraded script file")
-        upgraded = True
-    while(currentVersion < __workingVersion):
-        (data, currentVersion) = __upgradeDic[currentVersion](data)
-    return (upgraded, data)
-
-def __removeLineInfo(data):
-    if isinstance(data, dict):
-        data.pop("__line__", None)
-    if isinstance(data, list):
-        for item in data:
-            if isinstance(item, dict) or isinstance(item, list):
-                __removeLineInfo(item)
-    if isinstance(data, dict):
-        for key in data:
-            if isinstance(data[key], dict) or isinstance(data[key], list): 
-                __removeLineInfo(data[key])
-
-def processScriptData(file, saveUpgradedScript = False, printer = Printer()):
-    with open(file) as f:
-        data = yaml.load(f, Loader=SafeLineLoader)
-    if data == None: return data
-    (upgradedScript, data) = __upgradeScriptData(data, printer)
-    if saveUpgradedScript and upgradedScript:
-        dumpData = copy.deepcopy(data)
-        __removeLineInfo(dumpData)
-        with open(file, "w") as f:
-            yaml.dump(dumpData, f, sort_keys=False)
-    data.pop("version", None)
-    return data
+import copy
+import yaml
+from yaml.loader import SafeLoader
+
+from mazikeen.ConsolePrinter import Printer
+
+class SafeLineLoader(SafeLoader):
+    def construct_mapping(self, node, deep=False):
+        mapping = super(SafeLineLoader, self).construct_mapping(node, deep=deep)
+        # Add 1 so line numbering starts at 1
+        mapping['__line__'] = node.start_mark.line + 1
+        return mapping
+
+class Version():
+    def __init__(self, versionStr): 
+        (self.major, self.minor, self.patch) = ("", "", "")
+        if versionStr == None or versionStr == "": 
+            return
+
+        versionTupl = versionStr.split('.')
+        if len(versionTupl) > 3: 
+            raise Exception("Invalid version. Version is too long")
+        try:
+            if len(versionTupl) >= 1: 
+                self.major = int(versionTupl[0])
+            if len(versionTupl) >= 2: 
+                self.minor = int(versionTupl[1])
+            if len(versionTupl) == 3: 
+                self.patch = int(versionTupl[2])
+        except ValueError as e:
+            raise ValueError("Invalid version. Version may only contain numbers")
+
+    def __hash__(self):
+        return self.major * 10000 + self.minor * 100 + self.patch
+
+    def __eq__(self, other):
+        return (self.major == self.major and
+                self.minor == self.minor and
+                self.patch == self.patch)
+
+    def __lt__(self, other):
+        if self.major == "" and other.major != "": return True;
+        if self.major < other.major: return True;
+        if self.minor == "" and other.minor != "": return True;
+        if self.minor < other.minor: return True;
+        if self.patch == "" and other.patch != "": return True;
+        if self.patch < other.patch: return True;
+
+    def __str__(self):
+        return f"{str(self.major)}.{str(self.minor)}.{str(self.patch)}"
+
+
+def __upgradeScript1_0_0(data):
+    def fixDiffBlock(data):
+        if not isinstance(data, dict): 
+            return data
+        leftpath = ""
+        rightpath = ""
+        leftpathkey = None
+        rightpathkey = None
+        for key in data:
+            if key.lower() == "leftpath":
+                leftpath = data[key]
+                leftpathkey = key
+            elif key.lower() == "rightpath":
+                rightpath = data[key]
+                rightpathkey = key
+        if leftpathkey: data.pop(leftpathkey, None)
+        if rightpathkey: data.pop(rightpathkey, None)
+        if (leftpath == "" and rightpath == ""):
+            return data
+        data["paths"] = "\"" + leftpath + "\" \"" + rightpath + "\""
+        return data
+    
+    def fixRunBlock(data):
+        if isinstance(data, str):
+            return {'__line__': -1, 'cmd' : data, 'exitcode': 0}
+        if not isinstance(data, dict): 
+            return data
+        for key in data:
+            exitcode = None
+            if key.lower() == "exitCode":
+                exitcode = data[key]
+        if exitcode == None:
+            data["exitcode"] = 0
+        return data
+
+    def fixLooperData(data):
+        for key in data:
+            if key.lower() == "steps":
+                fixStepsData(data[key])
+
+    def fixStepsData(data):
+        if data == None: return
+        if not isinstance(data, list): 
+            raise Exception("Scriptfile can not be upgraded")
+
+        for step in data:
+            for key in step:
+                if key.lower() == "steps":
+                    fixStepsData(step[key])
+                if key.lower() == "run":
+                    step[key] = fixRunBlock(step[key])
+                if key.lower() == "diff":
+                    step[key] = fixDiffBlock(step[key])
+
+    data["version"]="1.1.0"
+    fixLooperData(data)
+    return (data, Version("1.1.0"))
+
+def __upgradeScript1_1_0(data):
+    def fixLooperData(data):
+        for key in data:
+            if key.lower() == "steps":
+                fixStepsData(data[key])
+
+    def fixStepsData(data):
+        if data == None: return
+        if not isinstance(data, list): 
+            raise Exception("Scriptfile can not be upgraded")
+
+        for step in data:
+            for key in step:
+                if key.lower() == "steps":
+                    fixStepsData(step[key])
+                if key.lower() == "diff":
+                    step[key] = fixDiffBlock(step[key])
+                if key.lower() == "run":
+                    step[key] = fixRunBlock(step[key])
+
+    def fixRunBlock(data):
+        if not isinstance(data, dict): 
+            return data
+        for key in data:
+            if key.lower() == "exitcode":
+                if data[key] == 'None':
+                    data.pop(key, None)
+                break
+        return data
+
+    def fixDiffBlock(data):
+        if not isinstance(data, dict): 
+            return data
+        for key in data:
+            if key.lower() == "ignorelines":
+                data['ignore'] = data[key]
+                data.pop(key, None)
+                break
+        return data
+
+    data["version"]="1.2.0"
+    fixLooperData(data)
+    return (data, Version("1.2.0"))
+
+__upgradeDic = {Version("1.0.0"): __upgradeScript1_0_0,
+                Version("1.1.0"): __upgradeScript1_1_0,}
+__workingVersion = Version("1.2.0")
+
+def __upgradeScriptData(data_, printer):
+    if data_ == None: return (False, data_)
+    data = data_.copy()
+
+    upgraded = False
+    currentVersion = Version(data.get("version", str(__workingVersion)))
+    if (currentVersion < __workingVersion): 
+        printer.verbose(f"Warning: script file needs to be upgraded to version: {str(__workingVersion)}. Use --upgradeScriptFile to save upgraded script file")
+        upgraded = True
+    while(currentVersion < __workingVersion):
+        (data, currentVersion) = __upgradeDic[currentVersion](data)
+    return (upgraded, data)
+
+def __removeLineInfo(data):
+    if isinstance(data, dict):
+        data.pop("__line__", None)
+    if isinstance(data, list):
+        for item in data:
+            if isinstance(item, dict) or isinstance(item, list):
+                __removeLineInfo(item)
+    if isinstance(data, dict):
+        for key in data:
+            if isinstance(data[key], dict) or isinstance(data[key], list): 
+                __removeLineInfo(data[key])
+
+def processScriptData(file, saveUpgradedScript = False, printer = Printer()):
+    with open(file) as f:
+        data = yaml.load(f, Loader=SafeLineLoader)
+    if data == None: return data
+    (upgradedScript, data) = __upgradeScriptData(data, printer)
+    if saveUpgradedScript and upgradedScript:
+        dumpData = copy.deepcopy(data)
+        __removeLineInfo(dumpData)
+        with open(file, "w") as f:
+            yaml.dump(dumpData, f, sort_keys=False)
+    data.pop("version", None)
+    return data
```

### Comparing `mazikeen-1.2.7/mazikeen/ScriptReader.py` & `mazikeen-1.2.8/mazikeen/ScriptReader.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import yaml
-from yaml.loader import SafeLoader
-
-from mazikeen.GeneratorLooper import serialReadYaml
-
-class SafeLineLoader(SafeLoader):
-    def construct_mapping(self, node, deep=False):
-        mapping = super(SafeLineLoader, self).construct_mapping(node, deep=deep)
-        # Add 1 so line numbering starts at 1
-        mapping['__line__'] = node.start_mark.line + 1
-        return mapping
-
-with open('script_test.yaml') as f:
-    data = yaml.load(f, Loader=SafeLineLoader)
-    print ("data = ", data)
-    res = serialReadYaml(data)
+import yaml
+from yaml.loader import SafeLoader
+
+from mazikeen.GeneratorLooper import serialReadYaml
+
+class SafeLineLoader(SafeLoader):
+    def construct_mapping(self, node, deep=False):
+        mapping = super(SafeLineLoader, self).construct_mapping(node, deep=deep)
+        # Add 1 so line numbering starts at 1
+        mapping['__line__'] = node.start_mark.line + 1
+        return mapping
+
+with open('script_test.yaml') as f:
+    data = yaml.load(f, Loader=SafeLineLoader)
+    print ("data = ", data)
+    res = serialReadYaml(data)
     pass
```

### Comparing `mazikeen-1.2.7/mazikeen/SignalHandler.py` & `mazikeen-1.2.8/mazikeen/SignalHandler.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-import signal
-
-__signal_received__ = None
-
-def failFast():
-    global __signal_received__
-    return __signal_received__ != None
-
-def init(): 
-    signal.signal(signal.SIGINT, signalHandler)
-
-def signalName():
-    global __signal_received__
-    if __signal_received__ == None: return __signal_received__
-    return str(signal.Signals(__signal_received__).name)
-
-def signalHandler(signal_received, frame):
-    global __signal_received__
-    if (__signal_received__ == None):
-        print(str(signal.Signals(signal_received).name) + " received fail fast enabled. Send signal again to force exit")
-        __signal_received__ = signal_received
-    else:
-        exit(1)
+import signal
+
+__signal_received__ = None
+
+def failFast():
+    global __signal_received__
+    return __signal_received__ != None
+
+def init(): 
+    signal.signal(signal.SIGINT, signalHandler)
+
+def signalName():
+    global __signal_received__
+    if __signal_received__ == None: return __signal_received__
+    return str(signal.Signals(__signal_received__).name)
+
+def signalHandler(signal_received, frame):
+    global __signal_received__
+    if (__signal_received__ == None):
+        print(str(signal.Signals(signal_received).name) + " received fail fast enabled. Send signal again to force exit")
+        __signal_received__ = signal_received
+    else:
+        exit(1)
```

### Comparing `mazikeen-1.2.7/mazikeen/Utils.py` & `mazikeen-1.2.8/mazikeen/Utils.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,200 +1,200 @@
-import re
-import os
-import shutil
-import stat
-import pathlib
-from enum import Enum
-
-from mazikeen.ConsolePrinter import Printer
-from mazikeen.GeneratorException import GeneratorException
-
-__replaceVariablesExp = re.compile(r'(?<!\\)\${.*?}')
-def replaceVariables(line, dictReplVar, printer = Printer()):
-    global __replaceVariablesExp
-    if line == None: return (True, line)
-    searchStart = 0
-    while (True):
-        m = __replaceVariablesExp.search(line[searchStart:])
-        if not m: 
-            break
-        foundVar = m.group()[2:-1]
-        replaceVal = dictReplVar.get(foundVar)
-        if (replaceVal):
-            strReplaceVal = str(replaceVal)
-            line = line[:searchStart + m.start()] + strReplaceVal + line[searchStart + m.end():]
-            searchStart += m.start() + len(strReplaceVal)
-        else:
-            raise GeneratorException("Variable " + str(m.group()) + " does not exist")
-    line = line.replace(r'\$', "$")
-    return line
-
-def ensure_dir(file_path):
-    directory = os.path.dirname(file_path)
-    if (directory) and (not os.path.exists(directory)):
-        os.makedirs(directory)
-
-def rmtree(path, printer = Printer()):
-    try:
-        def remove_readonly(fn, path, excinfo):
-            os.chmod(path, stat.S_IWRITE)
-            fn(path)
-        if os.path.exists(path):
-            shutil.rmtree(path, onerror=remove_readonly, ignore_errors = False)
-        return True
-    except Exception as e:
-        printer.error("rmtree:", e)
-        return False
-
-class diffStrategy(Enum):
-   IgnoreLeftOrphans = 0
-   IgnoreRightOrphans = 1
-   IgnoreOrphans = 2
-   All = 3
-
-def __listAllFilesWithoutRoot(path):
-    allFilesWithRoot = [pathlib.Path(dp) / f for dp, dn, fn in os.walk(os.path.expanduser(path)) for f in fn + dn]
-    rootMathLen = len(pathlib.Path(path).parts)
-    filesWithoutRoot = [pathlib.Path(*f.parts[rootMathLen:]) for f in allFilesWithRoot]
-    return filesWithoutRoot
-    
-def __getCompareLine(line, fh, compiledignore):
-    skipedLines = 0
-    while(True):
-        if not line: return (line, skipedLines)
-        try:
-            strLine = line.decode('utf-8')
-        except:
-            return (line, skipedLines)
-
-        lineMatchesSpan = []
-        for ignoreLine in compiledignore:
-            itMatch = ignoreLine.finditer(strLine)
-            for m in itMatch: lineMatchesSpan.append(m.span())
-        lineMatchesSpan.sort()
-
-        def concatenatelineMatches(lineMatchesSpan):
-            idx = 0
-            while idx < len(lineMatchesSpan) - 1:
-                cmpIdx = idx + 1
-                while cmpIdx < len(lineMatchesSpan):
-                    if lineMatchesSpan[idx][1] > lineMatchesSpan[cmpIdx][0]:
-                        lineMatchesSpan[idx] = (lineMatchesSpan[idx][0], max(lineMatchesSpan[idx][1], lineMatchesSpan[cmpIdx][1]))
-                        cmpIdx = idx + 1
-                        del lineMatchesSpan[cmpIdx]
-                    else: cmpIdx += 1
-                idx += 1
-        concatenatelineMatches(lineMatchesSpan)
-
-        def deleteLineMatchesFromString(strLine, lineMatchesSpan):
-            listLine = list(strLine)
-            for matchSpan in reversed(lineMatchesSpan):
-                del listLine[matchSpan[0]:matchSpan[1]]
-            return "".join(listLine)
-        newLine = deleteLineMatchesFromString(strLine, lineMatchesSpan)
-        if not newLine in ['', '\n', '\r', '\r\n']:
-            return (str.encode(newLine), skipedLines)
-        line = fh.readline()
-        skipedLines += 1
-    return (line, skipedLines)
-
-def normalizeEOL(line):
-    # Todo: can be optimized
-    if len(line) >=2 and line[-2:] == bytes('\r\n', 'utf-8'): 
-        line = line[:-2] + bytes('\n', 'utf-8')
-    elif len(line) >=1 and line[-1] == bytes('\r', 'utf-8'): 
-        line = line[:-1] + bytes('\n', 'utf-8')
-    return line
-
-def diffFiles(fileL, fileR, compiledignore = [], binaryCompare = False):
-    def areLinesIdentical(lineL, lineR, binaryCompare):
-        def normalizeEOL(line):
-            if len(line) >=2 and line[-2:] == bytes('\r\n', 'utf-8'): 
-                line = line[:-2] + bytes('\n', 'utf-8')
-            elif len(line) >=1 and line[-1] == bytes('\r', 'utf-8'): 
-                line = line[:-1] + bytes('\n', 'utf-8')
-            return line
-
-        if lineL == lineR: return True #This is the most likely scenario so it has priority
-        if binaryCompare == False:
-            return normalizeEOL(lineL) == normalizeEOL(lineR)
-        return False
-
-    with open(fileL, "rb") as fhL:
-        with open(fileR, "rb") as fhR:
-            (lineNrL, lineNrR) = (0, 0)
-            while True:
-                lineL = fhL.readline()
-                lineNrL += 1
-                lineR = fhR.readline()
-                lineNrR += 1
-                if (not lineL and not lineR): break #EOF reached
-                if areLinesIdentical(lineL, lineR, binaryCompare) == False:
-                    (lineL, skipedLines) = __getCompareLine(lineL, fhL, compiledignore)
-                    lineNrL += skipedLines
-                    (lineR, skipedLines) = __getCompareLine(lineR, fhR, compiledignore)
-                    lineNrR += skipedLines
-                    if areLinesIdentical(lineL, lineR, binaryCompare) == False:
-                        return {"lineNrL": lineNrL, 
-                                "lineNrR": lineNrR, 
-                                "lineL": lineL,
-                                "lineR": lineR}
-    return None
-
-def diff(pathL, pathR, binaryCompare = False, diffStrategy = diffStrategy.All, ignore = [], printer = Printer(verbose = True)):
-    rootM = pathlib.Path(pathL)
-    rootS = pathlib.Path(pathR)
-    compiledignore = list(map(lambda x: re.compile(x), ignore))
-    if (rootM.is_file() and rootS.is_file()):
-        diffRes = diffFiles(rootM, rootS, compiledignore = compiledignore, binaryCompare = binaryCompare)
-        if (diffRes):
-            if printer.isVerbose():
-                printer.error(f"diff failed: '{rootM}' != '{rootS}'\nwhere: {diffRes['lineNrL']}: {diffRes['lineL']} != {diffRes['lineNrR']}: {diffRes['lineR']}")
-            else:
-                printer.error(f"diff failed: '{rootM}' != '{rootS}'")
-            return False
-        return True
-
-    for file in [rootM, rootS]:
-        if not file.exists():
-            printer.error(f"diff failed: '{file}' doesn't exist")
-            return False
-
-    filesM = set(__listAllFilesWithoutRoot(pathL))
-    filesS = set(__listAllFilesWithoutRoot(pathR))
-    
-    swapFiles = False
-    if diffStrategy == diffStrategy.IgnoreLeftOrphans:
-        swapFiles = True
-        filesM, filesS = filesS, filesM
-        rootM, rootS = rootS, rootM
-    
-    if diffStrategy != diffStrategy.IgnoreOrphans:
-        for file in (filesM - filesS):
-            printer.error(f"diff failed: '{str(rootM/file)}' not in '{rootS / file.parent}'")
-            return False
-    
-    if diffStrategy == diffStrategy.All:
-        for file in (filesS - filesM):
-            printer.error(f"diff failed: '{str(rootS/file)}' not in '{rootM / file.parent}'")
-            return False
-    
-    comPaths =[(rootM/path, rootS/path) for path in (filesM & filesS)]
-    
-    for pathM, pathS in comPaths:
-        if (pathM.is_file() != pathS.is_file()):
-            (pathL_, pathR_) = (pathM, pathS) if not swapFiles else (pathS, pathM)
-            printer.error(f"diff failed: '{pathL_}' != '{pathR_}'")
-            return False
-
-    comFiles = [(pathM, pathS) for pathM, pathS in comPaths if pathM.is_file()]
-    for fileM, fileS in comFiles:
-        diffRes = diffFiles(fileM, fileS, binaryCompare = binaryCompare, compiledignore = compiledignore)
-        if (diffRes):
-            (fileL, fileR) = (fileM, fileS) if not swapFiles else (fileS, fileM)
-            if printer.isVerbose():
-                printer.error(f"diff failed: '{fileL}' != '{fileR}'\nwhere: {diffRes['lineNrL']}: {diffRes['lineL']} != {diffRes['lineNrR']}: {diffRes['lineR']}")
-            else:
-                printer.error(f"diff failed: '{fileL}' != '{fileR}'")
-            return False
-    return True
-
+import re
+import os
+import shutil
+import stat
+import pathlib
+from enum import Enum
+
+from mazikeen.ConsolePrinter import Printer
+from mazikeen.GeneratorException import GeneratorException
+
+__replaceVariablesExp = re.compile(r'(?<!\\)\${.*?}')
+def replaceVariables(line, dictReplVar, printer = Printer()):
+    global __replaceVariablesExp
+    if line == None: return (True, line)
+    searchStart = 0
+    while (True):
+        m = __replaceVariablesExp.search(line[searchStart:])
+        if not m: 
+            break
+        foundVar = m.group()[2:-1]
+        replaceVal = dictReplVar.get(foundVar)
+        if (replaceVal):
+            strReplaceVal = str(replaceVal)
+            line = line[:searchStart + m.start()] + strReplaceVal + line[searchStart + m.end():]
+            searchStart += m.start() + len(strReplaceVal)
+        else:
+            raise GeneratorException("Variable " + str(m.group()) + " does not exist")
+    line = line.replace(r'\$', "$")
+    return line
+
+def ensure_dir(file_path):
+    directory = os.path.dirname(file_path)
+    if (directory) and (not os.path.exists(directory)):
+        os.makedirs(directory)
+
+def rmtree(path, printer = Printer()):
+    try:
+        def remove_readonly(fn, path, excinfo):
+            os.chmod(path, stat.S_IWRITE)
+            fn(path)
+        if os.path.exists(path):
+            shutil.rmtree(path, onerror=remove_readonly, ignore_errors = False)
+        return True
+    except Exception as e:
+        printer.error("rmtree:", e)
+        return False
+
+class diffStrategy(Enum):
+   IgnoreLeftOrphans = 0
+   IgnoreRightOrphans = 1
+   IgnoreOrphans = 2
+   All = 3
+
+def __listAllFilesWithoutRoot(path):
+    allFilesWithRoot = [pathlib.Path(dp) / f for dp, dn, fn in os.walk(os.path.expanduser(path)) for f in fn + dn]
+    rootMathLen = len(pathlib.Path(path).parts)
+    filesWithoutRoot = [pathlib.Path(*f.parts[rootMathLen:]) for f in allFilesWithRoot]
+    return filesWithoutRoot
+    
+def __getCompareLine(line, fh, compiledignore):
+    skipedLines = 0
+    while(True):
+        if not line: return (line, skipedLines)
+        try:
+            strLine = line.decode('utf-8')
+        except:
+            return (line, skipedLines)
+
+        lineMatchesSpan = []
+        for ignoreLine in compiledignore:
+            itMatch = ignoreLine.finditer(strLine)
+            for m in itMatch: lineMatchesSpan.append(m.span())
+        lineMatchesSpan.sort()
+
+        def concatenatelineMatches(lineMatchesSpan):
+            idx = 0
+            while idx < len(lineMatchesSpan) - 1:
+                cmpIdx = idx + 1
+                while cmpIdx < len(lineMatchesSpan):
+                    if lineMatchesSpan[idx][1] > lineMatchesSpan[cmpIdx][0]:
+                        lineMatchesSpan[idx] = (lineMatchesSpan[idx][0], max(lineMatchesSpan[idx][1], lineMatchesSpan[cmpIdx][1]))
+                        cmpIdx = idx + 1
+                        del lineMatchesSpan[cmpIdx]
+                    else: cmpIdx += 1
+                idx += 1
+        concatenatelineMatches(lineMatchesSpan)
+
+        def deleteLineMatchesFromString(strLine, lineMatchesSpan):
+            listLine = list(strLine)
+            for matchSpan in reversed(lineMatchesSpan):
+                del listLine[matchSpan[0]:matchSpan[1]]
+            return "".join(listLine)
+        newLine = deleteLineMatchesFromString(strLine, lineMatchesSpan)
+        if not newLine in ['', '\n', '\r', '\r\n']:
+            return (str.encode(newLine), skipedLines)
+        line = fh.readline()
+        skipedLines += 1
+    return (line, skipedLines)
+
+def normalizeEOL(line):
+    # Todo: can be optimized
+    if len(line) >=2 and line[-2:] == bytes('\r\n', 'utf-8'): 
+        line = line[:-2] + bytes('\n', 'utf-8')
+    elif len(line) >=1 and line[-1] == bytes('\r', 'utf-8'): 
+        line = line[:-1] + bytes('\n', 'utf-8')
+    return line
+
+def diffFiles(fileL, fileR, compiledignore = [], binaryCompare = False):
+    def areLinesIdentical(lineL, lineR, binaryCompare):
+        def normalizeEOL(line):
+            if len(line) >=2 and line[-2:] == bytes('\r\n', 'utf-8'): 
+                line = line[:-2] + bytes('\n', 'utf-8')
+            elif len(line) >=1 and line[-1] == bytes('\r', 'utf-8'): 
+                line = line[:-1] + bytes('\n', 'utf-8')
+            return line
+
+        if lineL == lineR: return True #This is the most likely scenario so it has priority
+        if binaryCompare == False:
+            return normalizeEOL(lineL) == normalizeEOL(lineR)
+        return False
+
+    with open(fileL, "rb") as fhL:
+        with open(fileR, "rb") as fhR:
+            (lineNrL, lineNrR) = (0, 0)
+            while True:
+                lineL = fhL.readline()
+                lineNrL += 1
+                lineR = fhR.readline()
+                lineNrR += 1
+                if (not lineL and not lineR): break #EOF reached
+                if areLinesIdentical(lineL, lineR, binaryCompare) == False:
+                    (lineL, skipedLines) = __getCompareLine(lineL, fhL, compiledignore)
+                    lineNrL += skipedLines
+                    (lineR, skipedLines) = __getCompareLine(lineR, fhR, compiledignore)
+                    lineNrR += skipedLines
+                    if areLinesIdentical(lineL, lineR, binaryCompare) == False:
+                        return {"lineNrL": lineNrL, 
+                                "lineNrR": lineNrR, 
+                                "lineL": lineL,
+                                "lineR": lineR}
+    return None
+
+def diff(pathL, pathR, binaryCompare = False, diffStrategy = diffStrategy.All, ignore = [], printer = Printer(verbose = True)):
+    rootM = pathlib.Path(pathL)
+    rootS = pathlib.Path(pathR)
+    compiledignore = list(map(lambda x: re.compile(x), ignore))
+    if (rootM.is_file() and rootS.is_file()):
+        diffRes = diffFiles(rootM, rootS, compiledignore = compiledignore, binaryCompare = binaryCompare)
+        if (diffRes):
+            if printer.isVerbose():
+                printer.error(f"diff failed: '{rootM}' != '{rootS}'\nwhere: {diffRes['lineNrL']}: {diffRes['lineL']} != {diffRes['lineNrR']}: {diffRes['lineR']}")
+            else:
+                printer.error(f"diff failed: '{rootM}' != '{rootS}'")
+            return False
+        return True
+
+    for file in [rootM, rootS]:
+        if not file.exists():
+            printer.error(f"diff failed: '{file}' doesn't exist")
+            return False
+
+    filesM = set(__listAllFilesWithoutRoot(pathL))
+    filesS = set(__listAllFilesWithoutRoot(pathR))
+    
+    swapFiles = False
+    if diffStrategy == diffStrategy.IgnoreLeftOrphans:
+        swapFiles = True
+        filesM, filesS = filesS, filesM
+        rootM, rootS = rootS, rootM
+    
+    if diffStrategy != diffStrategy.IgnoreOrphans:
+        for file in (filesM - filesS):
+            printer.error(f"diff failed: '{str(rootM/file)}' not in '{rootS / file.parent}'")
+            return False
+    
+    if diffStrategy == diffStrategy.All:
+        for file in (filesS - filesM):
+            printer.error(f"diff failed: '{str(rootS/file)}' not in '{rootM / file.parent}'")
+            return False
+    
+    comPaths =[(rootM/path, rootS/path) for path in (filesM & filesS)]
+    
+    for pathM, pathS in comPaths:
+        if (pathM.is_file() != pathS.is_file()):
+            (pathL_, pathR_) = (pathM, pathS) if not swapFiles else (pathS, pathM)
+            printer.error(f"diff failed: '{pathL_}' != '{pathR_}'")
+            return False
+
+    comFiles = [(pathM, pathS) for pathM, pathS in comPaths if pathM.is_file()]
+    for fileM, fileS in comFiles:
+        diffRes = diffFiles(fileM, fileS, binaryCompare = binaryCompare, compiledignore = compiledignore)
+        if (diffRes):
+            (fileL, fileR) = (fileM, fileS) if not swapFiles else (fileS, fileM)
+            if printer.isVerbose():
+                printer.error(f"diff failed: '{fileL}' != '{fileR}'\nwhere: {diffRes['lineNrL']}: {diffRes['lineL']} != {diffRes['lineNrR']}: {diffRes['lineR']}")
+            else:
+                printer.error(f"diff failed: '{fileL}' != '{fileR}'")
+            return False
+    return True
+
```

### Comparing `mazikeen-1.2.7/mazikeen/__main__.py` & `mazikeen-1.2.8/mazikeen/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,206 +1,206 @@
-import os
-import io
-import glob
-import yaml
-import time
-import pathlib
-import argparse
-import multiprocessing
-import copy
-import re
-
-from pathlib import Path, PurePath
-from junit_xml import TestSuite, TestCase
-
-import mazikeen.SignalHandler as SignalHandler
-from mazikeen.GeneratorLooper import generateSerialBlock, generateParallelBlock
-from mazikeen.Loopers import Serial, Parallel
-from mazikeen.ConsolePrinter import Printer, BufferedPrinter
-from mazikeen.version import __version__
-from mazikeen.Utils import ensure_dir
-from mazikeen.ScriptDataProcessor import processScriptData
-
-def getScriptFiles(dir, scriptName, maxLevel=-1):
-    curLevel = 0
-    curLevelDirs = [Path(dir)]
-    scriptFiles = []
-    while(curLevelDirs and (curLevel != maxLevel)):
-        nextLevelDir = []
-        for curDir in curLevelDirs:
-            tmpNextLevelDir = []
-            dirContent = os.listdir(curDir)
-            for curFile in map(lambda path: Path(curDir).joinpath(path),dirContent): 
-                if curFile.is_dir(): 
-                    tmpNextLevelDir.append(curFile)
-                elif Path(curFile).name == scriptName:
-                    tmpNextLevelDir.clear()
-                    scriptFiles.append(str(curFile))
-                    break
-            nextLevelDir.extend(tmpNextLevelDir)
-        curLevelDirs = nextLevelDir
-        curLevel += 1
-    scriptFiles.sort()
-    return scriptFiles
-
-def createTestSuits(scriptFiles, root):
-    lenRootParts = len(Path(root).parts)
-    testSuits = []
-    for scriptFile in map(Path, scriptFiles):
-        tc = TestCase(scriptFile.parent.name, file = scriptFile)
-        tsName = scriptFile.parts[-3] if len(scriptFile.parts) - lenRootParts > 2 else ""
-        ts = next((testSuit for testSuit in testSuits if testSuit.name == tsName), None)
-        if ts == None:
-            testSuits.append(TestSuite(tsName, [tc]))
-        else:
-            ts.test_cases.append(tc)
-
-    return testSuits
-
-def parseArguments():
-    parser = argparse.ArgumentParser(description='Mazikeen test enviroment')
-     
-    parser.add_argument( '-p','--pattern', metavar='PATTERN', type=str,
-                        help='Only run tests which match pattern. Does support also negative patterns "-PATTERN"')
-    parser.add_argument( '-f','--failfast', action='store_true', 
-                        help='stop on first faild test as quickly as possible')
-    parser.add_argument( '--upgradeScriptFile', action='store_true', 
-                        help='save upgraded script file. Script files are upgraded if their version is lower that latest version')
-    parser.add_argument( '--scriptName', metavar='NAME', type=str, default="script.yaml",
-                        help='Mazikeen script name (`script.yaml` default)')
-    parser.add_argument( '-s','--start-directory', dest='start', metavar='DIR', type=pathlib.Path, default=".",
-                         help="Directory to start discovering tests ('.' default)")
-    parser.add_argument('-v', '--verbose', dest='verbose', action='count',
-                         help='Verbose output')
-    parser.add_argument('-j', '--jobs', dest='jobs', type=int, default = None, const = multiprocessing.cpu_count(), nargs='?',
-                         help='Specifies the number of jobs to run simultaneously')
-    parser.add_argument('-r', '--report', dest='reportfile', type=pathlib.Path,
-                         help='Create junit test report')
-    parser.add_argument('--version', action='version', version='%(prog)s ' + __version__)
-
-    return parser.parse_args()
-
-def markTestSkipedByPattern(testSuits, pattern):
-    if not isinstance(pattern,str): return
-    _pattern = copy.copy(pattern)
-    isNegativePatern = _pattern.startswith("-")
-    if isNegativePatern: _pattern = _pattern[1:]
-    try:
-        p = re.compile(_pattern)
-    except Exception as e:
-        print("Invalid --pattern argument \""+pattern+"\":",str(e))
-        exit(1)
-    for ts in testSuits: 
-        for tc in ts.test_cases:
-            if ( (p.match(tc.name) != None) == isNegativePatern):
-                tc.add_skipped_info("skipped because of --pattern argumet")
-
-def getReport(testSuits, processTime, executionTime):
-    tcPassed = 0
-    tcSkipped = 0
-    tcFailed = 0 
-    tcError = 0
-    reportTxt = io.StringIO()
-
-    for ts in testSuits:
-        for tc in ts.test_cases:
-            if tc.is_error(): tcError += 1
-            elif tc.is_failure(): tcFailed += 1
-            elif tc.is_skipped(): tcSkipped += 1
-            else: tcPassed += 1
-
-    print("----------------------------------------------------------------", file = reportTxt)
-    print("Total test cases:", tcPassed + tcSkipped + tcError + tcFailed, "passed:", tcPassed, "skipped:", tcSkipped, "error:", tcError, "failed:", tcFailed, file = reportTxt)
-    if (tcSkipped > 0):
-        print("----------------------------------------------------------------", file = reportTxt)
-        print("Skipped:", file = reportTxt)
-        for ts in testSuits:
-            for tc in ts.test_cases:
-                if tc.is_skipped(): print("\t"+ts.name+("/" if ts.name != "" else "")+tc.name, file = reportTxt)
-
-    if (tcError > 0):
-        print("----------------------------------------------------------------", file = reportTxt)
-        print("Error:", file = reportTxt)
-        for ts in testSuits:
-            for tc in ts.test_cases:
-                if tc.is_error(): print("\t"+ts.name+("/" if ts.name != "" else "")+tc.name, file = reportTxt)
-
-    if (tcFailed > 0):
-        print("----------------------------------------------------------------", file = reportTxt)
-        print("Failed:", file = reportTxt)
-        for ts in testSuits:
-            for tc in ts.test_cases:
-                if tc.is_failure(): print("\t"+ts.name+("/" if ts.name != "" else "") +tc.name, file = reportTxt)
-
-    print("----------------------------------------------------------------", file = reportTxt)
-    print("process time:",  '%.2f' % processTime, "execution time:",  '%.2f' % executionTime, file = reportTxt)
-
-    return {"text" : reportTxt.getvalue(), "passed" : tcPassed, "skipped" : tcSkipped, "error" : tcError, "failed" : tcFailed }
-
-class TestExecuter:
-    def __init__(self, testSuite, testCase, upgradeScriptFile):
-        self.testSuite = testSuite
-        self.testCase = testCase
-        self.upgradeScriptFile = upgradeScriptFile
-
-    def run(self, workingDir, variables = {}, printer = Printer()):
-        curDir = os.getcwd()
-        printer.print("["+"RUN".ljust(10) + "] ---", self.testSuite.name + ("/" if self.testSuite.name != "" else "") + self.testCase.name)
-        try:
-            startTime = time.time()
-            processStartTime = time.process_time()
-            data = processScriptData(self.testCase.file, saveUpgradedScript = self.upgradeScriptFile, printer = printer)
-            block = generateSerialBlock(data)
-            if block == None: return
-            res = block.run(workingDir = str(PurePath(self.testCase.file).parent), printer = printer)
-            if (not res):
-                self.testCase.add_failure_info(printer.errorOutput or "failed")
-        except Exception as e:
-            self.testCase.add_error_info(str(e))
-            printer.print(str(e))
-        finally:
-            self.testCase.elapsed_sec = time.time() - startTime
-            testResStr = "PASSED"
-            if self.testCase.is_error(): 
-                testResStr = "ERROR"
-            elif self.testCase.is_failure(): 
-                testResStr = "FAILED"
-            printStr = "["+testResStr.rjust(10) + "] --- " + self.testSuite.name + ("/" if self.testSuite.name != "" else "") + self.testCase.name
-            if (printer.isVerbose()): 
-                printStr += " --- process time: "+  '%.2f' % (time.process_time() - processStartTime) + " execution time: "+  '%.2f' % (time.time() - startTime)
-            printer.print(printStr)
-        return testResStr == "PASSED"
-
-def main():
-    SignalHandler.init()
-    args = parseArguments()
-    scriptFiles = getScriptFiles(args.start, args.scriptName)
-    testSuits = createTestSuits(scriptFiles, args.start)
-    markTestSkipedByPattern(testSuits, args.pattern)
-    genTestExecuter = [TestExecuter(ts, tc, args.upgradeScriptFile) for ts in testSuits for tc in ts.test_cases if not tc.is_skipped()]
-    if (args.jobs == None): 
-        runner = Serial(genTestExecuter, failfast=args.failfast)
-    else: 
-        runner = Parallel(genTestExecuter, failfast=args.failfast, max_workers = args.jobs)
-    startTime = time.time()
-    processStartTime = time.process_time()
-    res = runner.run(".", printer = Printer(args.verbose != None))
-    processTime = time.process_time() - processStartTime
-    executionTime = time.time() - startTime
-    if (args.failfast and res == False) or SignalHandler.failFast(): 
-        for ts in testSuits: 
-            for tc in ts.test_cases:
-                if tc.elapsed_sec == None:
-                    if (SignalHandler.failFast()):
-                        tc.add_skipped_info("skipped due to " + SignalHandler.signalName())
-                    else:
-                        tc.add_skipped_info("skipped due to --failfast argument")
-    report = getReport(testSuits, processTime, executionTime)
-    Printer(args.verbose != None).print(report["text"])
-    if (args.reportfile):
-        ensure_dir(args.reportfile)
-        with open(args.reportfile, "w") as fw:
-            fw.write(TestSuite.to_xml_string(testSuits))
-    exit(report["error"] > 0)
-    
-if __name__ == '__main__':
+import os
+import io
+import glob
+import yaml
+import time
+import pathlib
+import argparse
+import multiprocessing
+import copy
+import re
+
+from pathlib import Path, PurePath
+from junit_xml import TestSuite, TestCase
+
+import mazikeen.SignalHandler as SignalHandler
+from mazikeen.GeneratorLooper import generateSerialBlock, generateParallelBlock
+from mazikeen.Loopers import Serial, Parallel
+from mazikeen.ConsolePrinter import Printer, BufferedPrinter
+from mazikeen.version import __version__
+from mazikeen.Utils import ensure_dir
+from mazikeen.ScriptDataProcessor import processScriptData
+
+def getScriptFiles(dir, scriptName, maxLevel=-1):
+    curLevel = 0
+    curLevelDirs = [Path(dir)]
+    scriptFiles = []
+    while(curLevelDirs and (curLevel != maxLevel)):
+        nextLevelDir = []
+        for curDir in curLevelDirs:
+            tmpNextLevelDir = []
+            dirContent = os.listdir(curDir)
+            for curFile in map(lambda path: Path(curDir).joinpath(path),dirContent): 
+                if curFile.is_dir(): 
+                    tmpNextLevelDir.append(curFile)
+                elif Path(curFile).name == scriptName:
+                    tmpNextLevelDir.clear()
+                    scriptFiles.append(str(curFile))
+                    break
+            nextLevelDir.extend(tmpNextLevelDir)
+        curLevelDirs = nextLevelDir
+        curLevel += 1
+    scriptFiles.sort()
+    return scriptFiles
+
+def createTestSuits(scriptFiles, root):
+    lenRootParts = len(Path(root).parts)
+    testSuits = []
+    for scriptFile in map(Path, scriptFiles):
+        tc = TestCase(scriptFile.parent.name, file = scriptFile)
+        tsName = scriptFile.parts[-3] if len(scriptFile.parts) - lenRootParts > 2 else ""
+        ts = next((testSuit for testSuit in testSuits if testSuit.name == tsName), None)
+        if ts == None:
+            testSuits.append(TestSuite(tsName, [tc]))
+        else:
+            ts.test_cases.append(tc)
+
+    return testSuits
+
+def parseArguments():
+    parser = argparse.ArgumentParser(description='Mazikeen test enviroment')
+     
+    parser.add_argument( '-p','--pattern', metavar='PATTERN', type=str,
+                        help='Only run tests which match pattern. Does support also negative patterns "-PATTERN"')
+    parser.add_argument( '-f','--failfast', action='store_true', 
+                        help='stop on first faild test as quickly as possible')
+    parser.add_argument( '--upgradeScriptFile', action='store_true', 
+                        help='save upgraded script file. Script files are upgraded if their version is lower that latest version')
+    parser.add_argument( '--scriptName', metavar='NAME', type=str, default="script.yaml",
+                        help='Mazikeen script name (`script.yaml` default)')
+    parser.add_argument( '-s','--start-directory', dest='start', metavar='DIR', type=pathlib.Path, default=".",
+                         help="Directory to start discovering tests ('.' default)")
+    parser.add_argument('-v', '--verbose', dest='verbose', action='count',
+                         help='Verbose output')
+    parser.add_argument('-j', '--jobs', dest='jobs', type=int, default = None, const = multiprocessing.cpu_count(), nargs='?',
+                         help='Specifies the number of jobs to run simultaneously')
+    parser.add_argument('-r', '--report', dest='reportfile', type=pathlib.Path,
+                         help='Create junit test report')
+    parser.add_argument('--version', action='version', version='%(prog)s ' + __version__)
+
+    return parser.parse_args()
+
+def markTestSkipedByPattern(testSuits, pattern):
+    if not isinstance(pattern,str): return
+    _pattern = copy.copy(pattern)
+    isNegativePatern = _pattern.startswith("-")
+    if isNegativePatern: _pattern = _pattern[1:]
+    try:
+        p = re.compile(_pattern)
+    except Exception as e:
+        print("Invalid --pattern argument \""+pattern+"\":",str(e))
+        exit(1)
+    for ts in testSuits: 
+        for tc in ts.test_cases:
+            if ( (p.match(tc.name) != None) == isNegativePatern):
+                tc.add_skipped_info("skipped because of --pattern argumet")
+
+def getReport(testSuits, processTime, executionTime):
+    tcPassed = 0
+    tcSkipped = 0
+    tcFailed = 0 
+    tcError = 0
+    reportTxt = io.StringIO()
+
+    for ts in testSuits:
+        for tc in ts.test_cases:
+            if tc.is_error(): tcError += 1
+            elif tc.is_failure(): tcFailed += 1
+            elif tc.is_skipped(): tcSkipped += 1
+            else: tcPassed += 1
+
+    print("----------------------------------------------------------------", file = reportTxt)
+    print("Total test cases:", tcPassed + tcSkipped + tcError + tcFailed, "passed:", tcPassed, "skipped:", tcSkipped, "error:", tcError, "failed:", tcFailed, file = reportTxt)
+    if (tcSkipped > 0):
+        print("----------------------------------------------------------------", file = reportTxt)
+        print("Skipped:", file = reportTxt)
+        for ts in testSuits:
+            for tc in ts.test_cases:
+                if tc.is_skipped(): print("\t"+ts.name+("/" if ts.name != "" else "")+tc.name, file = reportTxt)
+
+    if (tcError > 0):
+        print("----------------------------------------------------------------", file = reportTxt)
+        print("Error:", file = reportTxt)
+        for ts in testSuits:
+            for tc in ts.test_cases:
+                if tc.is_error(): print("\t"+ts.name+("/" if ts.name != "" else "")+tc.name, file = reportTxt)
+
+    if (tcFailed > 0):
+        print("----------------------------------------------------------------", file = reportTxt)
+        print("Failed:", file = reportTxt)
+        for ts in testSuits:
+            for tc in ts.test_cases:
+                if tc.is_failure(): print("\t"+ts.name+("/" if ts.name != "" else "") +tc.name, file = reportTxt)
+
+    print("----------------------------------------------------------------", file = reportTxt)
+    print("process time:",  '%.2f' % processTime, "execution time:",  '%.2f' % executionTime, file = reportTxt)
+
+    return {"text" : reportTxt.getvalue(), "passed" : tcPassed, "skipped" : tcSkipped, "error" : tcError, "failed" : tcFailed }
+
+class TestExecuter:
+    def __init__(self, testSuite, testCase, upgradeScriptFile):
+        self.testSuite = testSuite
+        self.testCase = testCase
+        self.upgradeScriptFile = upgradeScriptFile
+
+    def run(self, workingDir, variables = {}, printer = Printer()):
+        curDir = os.getcwd()
+        printer.print("["+"RUN".ljust(10) + "] ---", self.testSuite.name + ("/" if self.testSuite.name != "" else "") + self.testCase.name)
+        try:
+            startTime = time.time()
+            processStartTime = time.process_time()
+            data = processScriptData(self.testCase.file, saveUpgradedScript = self.upgradeScriptFile, printer = printer)
+            block = generateSerialBlock(data)
+            if block == None: return
+            res = block.run(workingDir = str(PurePath(self.testCase.file).parent), printer = printer)
+            if (not res):
+                self.testCase.add_failure_info(printer.errorOutput or "failed")
+        except Exception as e:
+            self.testCase.add_error_info(str(e))
+            printer.print(str(e))
+        finally:
+            self.testCase.elapsed_sec = time.time() - startTime
+            testResStr = "PASSED"
+            if self.testCase.is_error(): 
+                testResStr = "ERROR"
+            elif self.testCase.is_failure(): 
+                testResStr = "FAILED"
+            printStr = "["+testResStr.rjust(10) + "] --- " + self.testSuite.name + ("/" if self.testSuite.name != "" else "") + self.testCase.name
+            if (printer.isVerbose()): 
+                printStr += " --- process time: "+  '%.2f' % (time.process_time() - processStartTime) + " execution time: "+  '%.2f' % (time.time() - startTime)
+            printer.print(printStr)
+        return testResStr == "PASSED"
+
+def main():
+    SignalHandler.init()
+    args = parseArguments()
+    scriptFiles = getScriptFiles(args.start, args.scriptName)
+    testSuits = createTestSuits(scriptFiles, args.start)
+    markTestSkipedByPattern(testSuits, args.pattern)
+    genTestExecuter = [TestExecuter(ts, tc, args.upgradeScriptFile) for ts in testSuits for tc in ts.test_cases if not tc.is_skipped()]
+    if (args.jobs == None): 
+        runner = Serial(genTestExecuter, failfast=args.failfast)
+    else: 
+        runner = Parallel(genTestExecuter, failfast=args.failfast, max_workers = args.jobs)
+    startTime = time.time()
+    processStartTime = time.process_time()
+    res = runner.run(".", printer = Printer(args.verbose != None))
+    processTime = time.process_time() - processStartTime
+    executionTime = time.time() - startTime
+    if (args.failfast and res == False) or SignalHandler.failFast(): 
+        for ts in testSuits: 
+            for tc in ts.test_cases:
+                if tc.elapsed_sec == None:
+                    if (SignalHandler.failFast()):
+                        tc.add_skipped_info("skipped due to " + SignalHandler.signalName())
+                    else:
+                        tc.add_skipped_info("skipped due to --failfast argument")
+    report = getReport(testSuits, processTime, executionTime)
+    Printer(args.verbose != None).print(report["text"])
+    if (args.reportfile):
+        ensure_dir(args.reportfile)
+        with open(args.reportfile, "w") as fw:
+            fw.write(TestSuite.to_xml_string(testSuits))
+    exit(report["error"] + report["failed"] > 0)
+    
+if __name__ == '__main__':
     main()
```

### Comparing `mazikeen-1.2.7/mazikeen.egg-info/PKG-INFO` & `mazikeen-1.2.8/mazikeen.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-Metadata-Version: 2.1
-Name: mazikeen
-Version: 1.2.7
-Summary: Test enviroment for CLI application
-Home-page: https://github.com/hanniballar/mazikeen
-Author: Neaga Septimiu
-Author-email: neagas@gmail.com
-License: MIT
-Project-URL: Bug Tracker, https://github.com/hanniballar/mazikeen/issues
-Description: `mazikeen` is a test framework for command line applications.
-        `mazikeen` was created to facilitae testing of CLI application that have a predictable output. It facilitates testing on different operating systems by provideing a diff method that is agnostic to newline and make / remove directory. For `mazikeen` every test has it's own directory helping debugging and organizing tests.
-        `mazikeen` empathise parralel testing.
-        
-        The test structure looks like:
-        ::
-        
-            Testsuit1
-            ├── Testcase1
-            │   └── script.yaml
-            ├── . . .
-            └──TestcaseN
-                └── script.yaml
-            Testsuit2
-            ├── Testcase1
-            │   └── script.yaml
-            ├── ...
-            └──TestcaseN
-                └── script.yaml
-        		
-        An example of a simple test:
-        
-        .. code-block:: yaml
-        
-            # content of script.yaml
-          ---
-          steps:
-            - rmdir: Output
-            - makedirs: Output
-            - run: echo "Hello World" > Output/hello.txt
-            - diff: Output/hello.txt Expected/hello.txt
-        
-        To execute it::
-        
-            $ mazikeen
-            [RUN       ] --- simple
-            [    PASSED] --- simple
-            ----------------------------------------------------------------
-            Total test cases: 1 passed: 1 skipped: 0 error: 0 failed: 0
-            ----------------------------------------------------------------
-            process time: 0.02 execution time: 0.01
-        
-        Features
-        --------
-        - Provides diff functions agnostic to newline and other common operations for different operating systems like make and remove directory. 
-        - Every test case is a directory. Making it easy to debug a failing test as all relevant data is stored in one place.
-        - Parallel execution support. Testscases can be executed in parallel. A testcase can call multiple CLI applications in parallel.
-        
-        
-        Documentation
-        -------------
-        
-        For full documentation, please see https://github.com/hanniballar/mazikeen/blob/master/Documentation/Mazikeen.rst .
-        
-        
-        Bugs/Requests
-        -------------
-        
-        Please use the `GitHub issue tracker <https://github.com/hanniballar/mazikeen/issues>`_ to submit bugs or request features.
-        
-        
-Platform: UNKNOWN
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: Utilities
-Description-Content-Type: text/x-rst
-Provides-Extra: testing
+Metadata-Version: 2.1
+Name: mazikeen
+Version: 1.2.8
+Summary: Test enviroment for CLI application
+Home-page: https://github.com/hanniballar/mazikeen
+Author: Neaga Septimiu
+Author-email: neagas@gmail.com
+License: MIT
+Project-URL: Bug Tracker, https://github.com/hanniballar/mazikeen/issues
+Description: `mazikeen` is a test framework for command line applications.
+        `mazikeen` was created to facilitae testing of CLI application that have a predictable output. It facilitates testing on different operating systems by provideing a diff method that is agnostic to newline and make / remove directory. For `mazikeen` every test has it's own directory helping debugging and organizing tests.
+        `mazikeen` empathise parralel testing.
+        
+        The test structure looks like:
+        ::
+        
+            Testsuit1
+            ├── Testcase1
+            │   └── script.yaml
+            ├── . . .
+            └──TestcaseN
+                └── script.yaml
+            Testsuit2
+            ├── Testcase1
+            │   └── script.yaml
+            ├── ...
+            └──TestcaseN
+                └── script.yaml
+        		
+        An example of a simple test:
+        
+        .. code-block:: yaml
+        
+            # content of script.yaml
+          ---
+          steps:
+            - rmdir: Output
+            - makedirs: Output
+            - run: echo "Hello World" > Output/hello.txt
+            - diff: Output/hello.txt Expected/hello.txt
+        
+        To execute it::
+        
+            $ mazikeen
+            [RUN       ] --- simple
+            [    PASSED] --- simple
+            ----------------------------------------------------------------
+            Total test cases: 1 passed: 1 skipped: 0 error: 0 failed: 0
+            ----------------------------------------------------------------
+            process time: 0.02 execution time: 0.01
+        
+        Features
+        --------
+        - Provides diff functions agnostic to newline and other common operations for different operating systems like make and remove directory. 
+        - Every test case is a directory. Making it easy to debug a failing test as all relevant data is stored in one place.
+        - Parallel execution support. Testscases can be executed in parallel. A testcase can call multiple CLI applications in parallel.
+        
+        
+        Documentation
+        -------------
+        
+        For full documentation, please see https://github.com/hanniballar/mazikeen/blob/master/Documentation/Mazikeen.rst .
+        
+        
+        Bugs/Requests
+        -------------
+        
+        Please use the `GitHub issue tracker <https://github.com/hanniballar/mazikeen/issues>`_ to submit bugs or request features.
+        
+        
+Platform: UNKNOWN
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Utilities
+Description-Content-Type: text/x-rst
+Provides-Extra: testing
```

### Comparing `mazikeen-1.2.7/mazikeen.egg-info/SOURCES.txt` & `mazikeen-1.2.8/mazikeen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mazikeen-1.2.7/setup.py` & `mazikeen-1.2.8/setup.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-import setuptools
-import mazikeen.version
-
-with open("README.rst", "r", encoding="utf-8") as fh:
-    long_description = fh.read()
-    
-with open("LICENSE", "r", encoding="utf-8") as fh:
-    LICENSE = fh.read()
-
-setuptools.setup(
-    name="mazikeen",
-    version=mazikeen.version.__version__,
-    author="Neaga Septimiu",
-    author_email="neagas@gmail.com",
-    description="Test enviroment for CLI application",
-    long_description=long_description,
-    long_description_content_type="text/x-rst",
-    url="https://github.com/hanniballar/mazikeen",
-    project_urls={
-        "Bug Tracker": "https://github.com/hanniballar/mazikeen/issues",
-    },
-    license_file = LICENSE,
-    license="MIT",
-    classifiers=[
-        "Intended Audience :: Developers",
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-        "Topic :: Software Development :: Testing",
-        "Topic :: Utilities"
-    ],
-    packages=["mazikeen"],
-    install_requires=["junit_xml>=1.8", "pyyaml>=5.4.1"],
-    extras_require={
-        'testing': [
-            "xmldiff==2.4"
-        ]
-    },
-    entry_points={"console_scripts": ["mazikeen=mazikeen.__main__:main"]},
+import setuptools
+import mazikeen.version
+
+with open("README.rst", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+    
+with open("LICENSE", "r", encoding="utf-8") as fh:
+    LICENSE = fh.read()
+
+setuptools.setup(
+    name="mazikeen",
+    version=mazikeen.version.__version__,
+    author="Neaga Septimiu",
+    author_email="neagas@gmail.com",
+    description="Test enviroment for CLI application",
+    long_description=long_description,
+    long_description_content_type="text/x-rst",
+    url="https://github.com/hanniballar/mazikeen",
+    project_urls={
+        "Bug Tracker": "https://github.com/hanniballar/mazikeen/issues",
+    },
+    license_file = LICENSE,
+    license="MIT",
+    classifiers=[
+        "Intended Audience :: Developers",
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+        "Topic :: Software Development :: Testing",
+        "Topic :: Utilities"
+    ],
+    packages=["mazikeen"],
+    install_requires=["junit_xml>=1.8", "pyyaml>=5.4.1"],
+    extras_require={
+        'testing': [
+            "xmldiff==2.4"
+        ]
+    },
+    entry_points={"console_scripts": ["mazikeen=mazikeen.__main__:main"]},
 )
```

