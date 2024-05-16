# Comparing `tmp/robotcode_runner-0.82.3.tar.gz` & `tmp/robotcode_runner-0.83.0.tar.gz`

## Comparing `robotcode_runner-0.82.3.tar` & `robotcode_runner-0.83.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_runner-0.82.3/src/robotcode/runner/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_runner-0.82.3/src/robotcode/runner/__version__.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 robotcode_runner-0.82.3/src/robotcode/runner/hooks.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_runner-0.82.3/src/robotcode/runner/py.typed
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 robotcode_runner-0.82.3/src/robotcode/runner/cli/__init__.py
--rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 robotcode_runner-0.82.3/src/robotcode/runner/cli/libdoc.py
--rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 robotcode_runner-0.82.3/src/robotcode/runner/cli/rebot.py
--rw-r--r--   0        0        0     6306 2020-02-02 00:00:00.000000 robotcode_runner-0.82.3/src/robotcode/runner/cli/robot.py
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 robotcode_runner-0.82.3/src/robotcode/runner/cli/testdoc.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 robotcode_runner-0.82.3/src/robotcode/runner/cli/discover/__init__.py
--rw-r--r--   0        0        0    29986 2020-02-02 00:00:00.000000 robotcode_runner-0.82.3/src/robotcode/runner/cli/discover/discover.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_runner-0.82.3/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_runner-0.82.3/LICENSE.txt
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 robotcode_runner-0.82.3/README.md
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 robotcode_runner-0.82.3/pyproject.toml
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 robotcode_runner-0.82.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_runner-0.83.0/src/robotcode/runner/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_runner-0.83.0/src/robotcode/runner/__version__.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 robotcode_runner-0.83.0/src/robotcode/runner/hooks.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_runner-0.83.0/src/robotcode/runner/py.typed
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 robotcode_runner-0.83.0/src/robotcode/runner/cli/__init__.py
+-rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 robotcode_runner-0.83.0/src/robotcode/runner/cli/libdoc.py
+-rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 robotcode_runner-0.83.0/src/robotcode/runner/cli/rebot.py
+-rw-r--r--   0        0        0     6306 2020-02-02 00:00:00.000000 robotcode_runner-0.83.0/src/robotcode/runner/cli/robot.py
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 robotcode_runner-0.83.0/src/robotcode/runner/cli/testdoc.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 robotcode_runner-0.83.0/src/robotcode/runner/cli/discover/__init__.py
+-rw-r--r--   0        0        0    29986 2020-02-02 00:00:00.000000 robotcode_runner-0.83.0/src/robotcode/runner/cli/discover/discover.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_runner-0.83.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_runner-0.83.0/LICENSE.txt
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 robotcode_runner-0.83.0/README.md
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 robotcode_runner-0.83.0/pyproject.toml
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 robotcode_runner-0.83.0/PKG-INFO
```

### Comparing `robotcode_runner-0.82.3/src/robotcode/runner/cli/libdoc.py` & `robotcode_runner-0.83.0/src/robotcode/runner/cli/libdoc.py`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.82.3/src/robotcode/runner/cli/rebot.py` & `robotcode_runner-0.83.0/src/robotcode/runner/cli/rebot.py`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.82.3/src/robotcode/runner/cli/robot.py` & `robotcode_runner-0.83.0/src/robotcode/runner/cli/robot.py`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.82.3/src/robotcode/runner/cli/testdoc.py` & `robotcode_runner-0.83.0/src/robotcode/runner/cli/testdoc.py`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.82.3/src/robotcode/runner/cli/discover/discover.py` & `robotcode_runner-0.83.0/src/robotcode/runner/cli/discover/discover.py`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.82.3/.gitignore` & `robotcode_runner-0.83.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.82.3/LICENSE.txt` & `robotcode_runner-0.83.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.82.3/README.md` & `robotcode_runner-0.83.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.82.3/pyproject.toml` & `robotcode_runner-0.83.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -24,18 +24,18 @@
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dynamic = ["version"]
 dependencies = [
   "robotframework>=4.1.0",
-  "robotcode-robot==0.82.3",
-  "robotcode-modifiers==0.82.3",
-  "robotcode-plugin==0.82.3",
-  "robotcode==0.82.3",
+  "robotcode-robot==0.83.0",
+  "robotcode-modifiers==0.83.0",
+  "robotcode-plugin==0.83.0",
+  "robotcode==0.83.0",
 ]
 
 [project.entry-points.robotcode]
 runner = "robotcode.runner.hooks"
 
 [project.urls]
 Homepage = "https://robotcode.io"
```

### Comparing `robotcode_runner-0.82.3/PKG-INFO` & `robotcode_runner-0.83.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: robotcode-runner
-Version: 0.82.3
+Version: 0.83.0
 Summary: RobotCode runner plugin for Robot Framework
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://opencollective.com/robotcode
 Project-URL: Documentation, https://github.com/robotcodedev/robotcode#readme
 Project-URL: Changelog, https://github.com/robotcodedev/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/robotcodedev/robotcode/issues
 Project-URL: Source, https://github.com/robotcodedev/robotcode
@@ -21,18 +21,18 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-modifiers==0.82.3
-Requires-Dist: robotcode-plugin==0.82.3
-Requires-Dist: robotcode-robot==0.82.3
-Requires-Dist: robotcode==0.82.3
+Requires-Dist: robotcode-modifiers==0.83.0
+Requires-Dist: robotcode-plugin==0.83.0
+Requires-Dist: robotcode-robot==0.83.0
+Requires-Dist: robotcode==0.83.0
 Requires-Dist: robotframework>=4.1.0
 Description-Content-Type: text/markdown
 
 # robotcode-runner
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-runner.svg)](https://pypi.org/project/robotcode-runner)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/robotcode-runner.svg)](https://pypi.org/project/robotcode-runner)
```

