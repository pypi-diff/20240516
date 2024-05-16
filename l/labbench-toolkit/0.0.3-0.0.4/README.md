# Comparing `tmp/labbench_toolkit-0.0.3.tar.gz` & `tmp/labbench_toolkit-0.0.4.tar.gz`

## Comparing `labbench_toolkit-0.0.3.tar` & `labbench_toolkit-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rwxr-xr-x   0        0        0       25 2020-02-02 00:00:00.000000 labbench_toolkit-0.0.3/clean.bat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 labbench_toolkit-0.0.3/src/labbench_toolkit/__init__.py
--rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 labbench_toolkit-0.0.3/src/labbench_toolkit/io.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 labbench_toolkit-0.0.3/src/labbench_toolkit/psychophysics.py
--rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 labbench_toolkit-0.0.3/src/labbench_toolkit/result.py
--rw-r--r--   0        0        0     6291 2020-02-02 00:00:00.000000 labbench_toolkit-0.0.3/src/labbench_toolkit/protocols/stop_signal_task.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 labbench_toolkit-0.0.3/src/labbench_toolkit/protocols/threshold_tracking.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 labbench_toolkit-0.0.3/tests/basictest.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 labbench_toolkit-0.0.3/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 labbench_toolkit-0.0.3/LICENSE
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 labbench_toolkit-0.0.3/README.md
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 labbench_toolkit-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 labbench_toolkit-0.0.3/PKG-INFO
+-rwxr-xr-x   0        0        0       11 2020-02-02 00:00:00.000000 labbench_toolkit-0.0.4/build.bat
+-rwxr-xr-x   0        0        0       25 2020-02-02 00:00:00.000000 labbench_toolkit-0.0.4/clean.bat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 labbench_toolkit-0.0.4/src/labbench_toolkit/__init__.py
+-rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 labbench_toolkit-0.0.4/src/labbench_toolkit/io.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 labbench_toolkit-0.0.4/src/labbench_toolkit/psychophysics.py
+-rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 labbench_toolkit-0.0.4/src/labbench_toolkit/result.py
+-rw-r--r--   0        0        0     6338 2020-02-02 00:00:00.000000 labbench_toolkit-0.0.4/src/labbench_toolkit/protocols/stop_signal_task.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 labbench_toolkit-0.0.4/src/labbench_toolkit/protocols/threshold_tracking.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 labbench_toolkit-0.0.4/tests/basictest.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 labbench_toolkit-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 labbench_toolkit-0.0.4/LICENSE
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 labbench_toolkit-0.0.4/README.md
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 labbench_toolkit-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 labbench_toolkit-0.0.4/PKG-INFO
```

### Comparing `labbench_toolkit-0.0.3/src/labbench_toolkit/io.py` & `labbench_toolkit-0.0.4/src/labbench_toolkit/io.py`

 * *Files identical despite different names*

### Comparing `labbench_toolkit-0.0.3/src/labbench_toolkit/psychophysics.py` & `labbench_toolkit-0.0.4/src/labbench_toolkit/psychophysics.py`

 * *Files identical despite different names*

### Comparing `labbench_toolkit-0.0.3/src/labbench_toolkit/result.py` & `labbench_toolkit-0.0.4/src/labbench_toolkit/result.py`

 * *Files identical despite different names*

### Comparing `labbench_toolkit-0.0.3/src/labbench_toolkit/protocols/stop_signal_task.py` & `labbench_toolkit-0.0.4/src/labbench_toolkit/protocols/stop_signal_task.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,20 +24,24 @@
         self._lambda = 0.02
         self._gamma = 0.00
         self._sessionId = result.SessionID
         self._displayPlot = False
         self._savePlot = False
         self._name = name
               
-    def Configure(self, display: bool, save: bool):
-        self._displayPlot = display
-        self._savePlot = save
+    def SaveFiles(self, enable: bool):
+        self._savePlot = enable
 
         return self
-    
+
+    def Display(self, enable: bool):
+        self._displayPlot = enable
+
+        return self
+
     @property
     def ReactionTime(self):
         return statistics.mean(self.GetReactionTimes())
 
     def GetReactionTimes(self):
         return [time for time, answer in zip(self._gtTime, self._gtAnswer) if answer == 1]
```

### Comparing `labbench_toolkit-0.0.3/.gitignore` & `labbench_toolkit-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `labbench_toolkit-0.0.3/LICENSE` & `labbench_toolkit-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `labbench_toolkit-0.0.3/pyproject.toml` & `labbench_toolkit-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "labbench-toolkit"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Kristian Hennings", email="help@inventors.dk" },
 ]
 description = "Toolkit for analysing data from the LabBench software for psychophysical and neuroscience experiments"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `labbench_toolkit-0.0.3/PKG-INFO` & `labbench_toolkit-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: labbench-toolkit
-Version: 0.0.3
+Version: 0.0.4
 Summary: Toolkit for analysing data from the LabBench software for psychophysical and neuroscience experiments
 Project-URL: Homepage, https://github.com/Inventors-Way/labbench.toolkit
 Project-URL: Issues, https://github.com/Inventors-Way/labbench.toolkit/issues
 Author-email: Kristian Hennings <help@inventors.dk>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

