# Comparing `tmp/lytix_py-1.3.4.tar.gz` & `tmp/lytix_py-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lytix_py-1.3.4.tar", last modified: Wed May 15 17:31:35 2024, max compression
+gzip compressed data, was "lytix_py-1.4.0.tar", last modified: Thu May 16 18:27:57 2024, max compression
```

## Comparing `lytix_py-1.3.4.tar` & `lytix_py-1.4.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-15 17:31:35.025112 lytix_py-1.3.4/
--rw-r--r--   0 sidpremkumar   (501) staff       (20)     1081 2024-05-05 21:16:18.000000 lytix_py-1.3.4/LICENSE.md
--rw-r--r--   0 sidpremkumar   (501) staff       (20)     1008 2024-05-15 17:31:35.024877 lytix_py-1.3.4/PKG-INFO
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      450 2024-05-05 21:16:53.000000 lytix_py-1.3.4/README.md
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      625 2024-05-15 17:31:09.000000 lytix_py-1.3.4/pyproject.toml
--rw-r--r--   0 sidpremkumar   (501) staff       (20)       38 2024-05-15 17:31:35.025156 lytix_py-1.3.4/setup.cfg
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-15 17:31:35.022989 lytix_py-1.3.4/src/
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-15 17:31:35.023706 lytix_py-1.3.4/src/lytix_py/
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-15 17:31:35.024376 lytix_py-1.3.4/src/lytix_py/LLLogger/
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      886 2024-05-06 00:20:17.000000 lytix_py-1.3.4/src/lytix_py/LLLogger/LLLogger.py
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-15 17:31:35.024505 lytix_py-1.3.4/src/lytix_py/MetricCollector/
--rw-r--r--   0 sidpremkumar   (501) staff       (20)     2815 2024-05-15 17:30:42.000000 lytix_py-1.3.4/src/lytix_py/MetricCollector/MetricCollector.py
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      133 2024-05-13 18:41:07.000000 lytix_py-1.3.4/src/lytix_py/__init__.py
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      658 2024-05-13 18:47:25.000000 lytix_py-1.3.4/src/lytix_py/envVars.py
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-15 17:31:35.024679 lytix_py-1.3.4/src/lytix_py.egg-info/
--rw-r--r--   0 sidpremkumar   (501) staff       (20)     1008 2024-05-15 17:31:35.000000 lytix_py-1.3.4/src/lytix_py.egg-info/PKG-INFO
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      345 2024-05-15 17:31:35.000000 lytix_py-1.3.4/src/lytix_py.egg-info/SOURCES.txt
--rw-r--r--   0 sidpremkumar   (501) staff       (20)        1 2024-05-15 17:31:35.000000 lytix_py-1.3.4/src/lytix_py.egg-info/dependency_links.txt
--rw-r--r--   0 sidpremkumar   (501) staff       (20)       32 2024-05-15 17:31:35.000000 lytix_py-1.3.4/src/lytix_py.egg-info/requires.txt
--rw-r--r--   0 sidpremkumar   (501) staff       (20)        9 2024-05-15 17:31:35.000000 lytix_py-1.3.4/src/lytix_py.egg-info/top_level.txt
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-16 18:27:57.167312 lytix_py-1.4.0/
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)     1081 2024-05-05 21:16:18.000000 lytix_py-1.4.0/LICENSE.md
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)     1008 2024-05-16 18:27:57.167096 lytix_py-1.4.0/PKG-INFO
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      450 2024-05-05 21:16:53.000000 lytix_py-1.4.0/README.md
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      625 2024-05-16 18:27:02.000000 lytix_py-1.4.0/pyproject.toml
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)       38 2024-05-16 18:27:57.167377 lytix_py-1.4.0/setup.cfg
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-16 18:27:57.164723 lytix_py-1.4.0/src/
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-16 18:27:57.165586 lytix_py-1.4.0/src/lytix_py/
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-16 18:27:57.166472 lytix_py-1.4.0/src/lytix_py/LLLogger/
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      886 2024-05-06 00:20:17.000000 lytix_py-1.4.0/src/lytix_py/LLLogger/LLLogger.py
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-16 18:27:57.166686 lytix_py-1.4.0/src/lytix_py/MetricCollector/
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)     3012 2024-05-16 18:27:48.000000 lytix_py-1.4.0/src/lytix_py/MetricCollector/MetricCollector.py
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      133 2024-05-13 18:41:07.000000 lytix_py-1.4.0/src/lytix_py/__init__.py
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      658 2024-05-13 18:47:25.000000 lytix_py-1.4.0/src/lytix_py/envVars.py
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-16 18:27:57.166875 lytix_py-1.4.0/src/lytix_py.egg-info/
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)     1008 2024-05-16 18:27:57.000000 lytix_py-1.4.0/src/lytix_py.egg-info/PKG-INFO
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      345 2024-05-16 18:27:57.000000 lytix_py-1.4.0/src/lytix_py.egg-info/SOURCES.txt
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)        1 2024-05-16 18:27:57.000000 lytix_py-1.4.0/src/lytix_py.egg-info/dependency_links.txt
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)       32 2024-05-16 18:27:57.000000 lytix_py-1.4.0/src/lytix_py.egg-info/requires.txt
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)        9 2024-05-16 18:27:57.000000 lytix_py-1.4.0/src/lytix_py.egg-info/top_level.txt
```

### Comparing `lytix_py-1.3.4/LICENSE.md` & `lytix_py-1.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lytix_py-1.3.4/PKG-INFO` & `lytix_py-1.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lytix-py
-Version: 1.3.4
+Version: 1.4.0
 Summary: Official Lytix Client Packages
 Author-email: Lytix <support@lytix.com>
 Project-URL: Homepage, https://github.com/Lytix-Labs/lytix-py
 Project-URL: Issues, https://github.com/Lytix-Labs/lytix-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lytix_py-1.3.4/pyproject.toml` & `lytix_py-1.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lytix-py"
-version = "1.3.4"
+version = "1.4.0"
 authors = [
   { name="Lytix", email="support@lytix.com" },
 ]
 description = "Official Lytix Client Packages"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `lytix_py-1.3.4/src/lytix_py/LLLogger/LLLogger.py` & `lytix_py-1.4.0/src/lytix_py/LLLogger/LLLogger.py`

 * *Files identical despite different names*

### Comparing `lytix_py-1.3.4/src/lytix_py/MetricCollector/MetricCollector.py` & `lytix_py-1.4.0/src/lytix_py/MetricCollector/MetricCollector.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,43 +45,45 @@
             "metadata": metricMetadata
         }
         self._sendPostRequest("increment", body)
 
     """
     Capture a model input/output
     """
-    def captureModelIO(self, modelName: str, userInput: str, modelOutput: str, metricMetadata: dict = None):
+    def captureModelIO(self, modelName: str, modelInput: str, modelOutput: str, metricMetadata: dict = None, userIdentifier = None, sessionId = None):
         if LytixCreds.LX_API_KEY is None: 
             return 
 
         if metricMetadata is None:
             metricMetadata = {}
         body = {
             "modelName": modelName,
-            "userInput": userInput,
+            "modelInput": modelInput,
             "modelOutput": modelOutput,
-            "metricMetadata": metricMetadata
+            "metricMetadata": metricMetadata,
+            "userIdentifier": userIdentifier,
+            "sessionId": sessionId
         }
         self._sendPostRequest("modelIO", body)
 
     """
     Capture a model io event while also capturing the time to respond
     """
-    def captureModelTrace(self, modelName: str, userInput: str, callback, metricMetadata: dict = {}):
+    def captureModelTrace(self, modelName: str, modelInput: str, callback, metricMetadata: dict = {}, userIdentifier = None, sessionId = None):
         if LytixCreds.LX_API_KEY is None: 
             return callback()
 
         startTime = time.time()
         modelOutput = callback()
         try:
             responseTime = int((time.time() - startTime) * 1000)  # Convert to milliseconds
             # Capture modelIO event along with the response time
-            self.captureModelIO(modelName, userInput, modelOutput, metricMetadata)
+            self.captureModelIO(modelName, modelInput, modelOutput, metricMetadata, userIdentifier, sessionId)
             self.increment("model.responseTime", responseTime, {"modelName": modelName}.update(metricMetadata))
         except Exception as err:
-            self.logger.error(f"Failed to capture model trace: {err}", err, modelName, userInput)
+            self.logger.error(f"Failed to capture model trace: {err}", err, modelName, modelInput)
             raise err
         finally:
             return modelOutput
 
 MetricCollector = _MetricCollector()
```

### Comparing `lytix_py-1.3.4/src/lytix_py/envVars.py` & `lytix_py-1.4.0/src/lytix_py/envVars.py`

 * *Files identical despite different names*

### Comparing `lytix_py-1.3.4/src/lytix_py.egg-info/PKG-INFO` & `lytix_py-1.4.0/src/lytix_py.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lytix-py
-Version: 1.3.4
+Version: 1.4.0
 Summary: Official Lytix Client Packages
 Author-email: Lytix <support@lytix.com>
 Project-URL: Homepage, https://github.com/Lytix-Labs/lytix-py
 Project-URL: Issues, https://github.com/Lytix-Labs/lytix-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

