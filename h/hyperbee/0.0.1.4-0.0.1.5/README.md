# Comparing `tmp/hyperbee-0.0.1.4.tar.gz` & `tmp/hyperbee-0.0.1.5.tar.gz`

## Comparing `hyperbee-0.0.1.4.tar` & `hyperbee-0.0.1.5.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0     6631 2020-02-02 00:00:00.000000 hyperbee-0.0.1.4/src/hyperbee/__init__.py
--rw-r--r--   0        0        0    16826 2020-02-02 00:00:00.000000 hyperbee-0.0.1.4/src/hyperbee/_client.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 hyperbee-0.0.1.4/src/hyperbee/_version.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 hyperbee-0.0.1.4/src/hyperbee/version.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 hyperbee-0.0.1.4/src/hyperbee/resources/__init__.py
--rw-r--r--   0        0        0    30808 2020-02-02 00:00:00.000000 hyperbee-0.0.1.4/src/hyperbee/resources/completions.py
--rw-r--r--   0        0        0    10189 2020-02-02 00:00:00.000000 hyperbee-0.0.1.4/src/hyperbee/resources/models.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 hyperbee-0.0.1.4/src/hyperbee/resources/chat/__init__.py
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 hyperbee-0.0.1.4/src/hyperbee/resources/chat/chat.py
--rw-r--r--   0        0        0    36597 2020-02-02 00:00:00.000000 hyperbee-0.0.1.4/src/hyperbee/resources/chat/completions.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 hyperbee-0.0.1.4/src/hyperbee/resources/pipeline/__init__.py
--rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 hyperbee-0.0.1.4/src/hyperbee/resources/pipeline/pipeline.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 hyperbee-0.0.1.4/.gitignore
--rw-r--r--   0        0        0    11307 2020-02-02 00:00:00.000000 hyperbee-0.0.1.4/README.md
--rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 hyperbee-0.0.1.4/pyproject.toml
--rw-r--r--   0        0        0    12901 2020-02-02 00:00:00.000000 hyperbee-0.0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     6631 2020-02-02 00:00:00.000000 hyperbee-0.0.1.5/src/hyperbee/__init__.py
+-rw-r--r--   0        0        0    16885 2020-02-02 00:00:00.000000 hyperbee-0.0.1.5/src/hyperbee/_client.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 hyperbee-0.0.1.5/src/hyperbee/_version.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 hyperbee-0.0.1.5/src/hyperbee/version.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 hyperbee-0.0.1.5/src/hyperbee/resources/__init__.py
+-rw-r--r--   0        0        0    30808 2020-02-02 00:00:00.000000 hyperbee-0.0.1.5/src/hyperbee/resources/completions.py
+-rw-r--r--   0        0        0    10189 2020-02-02 00:00:00.000000 hyperbee-0.0.1.5/src/hyperbee/resources/models.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 hyperbee-0.0.1.5/src/hyperbee/resources/batch_request/__init__.py
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 hyperbee-0.0.1.5/src/hyperbee/resources/batch_request/batch_request.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 hyperbee-0.0.1.5/src/hyperbee/resources/chat/__init__.py
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 hyperbee-0.0.1.5/src/hyperbee/resources/chat/chat.py
+-rw-r--r--   0        0        0    36597 2020-02-02 00:00:00.000000 hyperbee-0.0.1.5/src/hyperbee/resources/chat/completions.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 hyperbee-0.0.1.5/src/hyperbee/resources/pipeline/__init__.py
+-rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 hyperbee-0.0.1.5/src/hyperbee/resources/pipeline/pipeline.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 hyperbee-0.0.1.5/.gitignore
+-rw-r--r--   0        0        0    11307 2020-02-02 00:00:00.000000 hyperbee-0.0.1.5/README.md
+-rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 hyperbee-0.0.1.5/pyproject.toml
+-rw-r--r--   0        0        0    12901 2020-02-02 00:00:00.000000 hyperbee-0.0.1.5/PKG-INFO
```

### Comparing `hyperbee-0.0.1.4/src/hyperbee/__init__.py` & `hyperbee-0.0.1.5/src/hyperbee/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.1.4/src/hyperbee/_client.py` & `hyperbee-0.0.1.5/src/hyperbee/_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,14 +118,15 @@
 
         self.completions = resources.Completions(self)
         self.chat = resources.Chat(self)
         self.models = resources.Models(self)
         self.with_raw_response = HiveWithRawResponse(self)
         self.with_streaming_response = HiveWithStreamedResponse(self)
         self.pipeline = resources.Pipeline(self)
+        self.batch_request = resources.batch_request(self)
 
     @property
     @override
     def qs(self) -> Querystring:
         return Querystring(array_format="comma")
 
     @property
```

### Comparing `hyperbee-0.0.1.4/src/hyperbee/resources/__init__.py` & `hyperbee-0.0.1.5/src/hyperbee/resources/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,17 @@
     CompletionsWithStreamingResponse,
     AsyncCompletionsWithStreamingResponse,
 )
 from .pipeline import (
     Pipeline,
     AsyncPipeline,
 )
+from .batch_request import (
+    batch_request,
+)
 
 __all__ = [
     "Completions",
     "AsyncCompletions",
     "CompletionsWithRawResponse",
     "AsyncCompletionsWithRawResponse",
     "CompletionsWithStreamingResponse",
@@ -45,9 +48,10 @@
     "Models",
     "AsyncModels",
     "ModelsWithRawResponse",
     "AsyncModelsWithRawResponse",
     "ModelsWithStreamingResponse",
     "AsyncModelsWithStreamingResponse",
     "Pipeline",
-    "AsyncPipeline"
+    "AsyncPipeline",
+    "batch_request"
 ]
```

### Comparing `hyperbee-0.0.1.4/src/hyperbee/resources/completions.py` & `hyperbee-0.0.1.5/src/hyperbee/resources/completions.py`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.1.4/src/hyperbee/resources/models.py` & `hyperbee-0.0.1.5/src/hyperbee/resources/models.py`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.1.4/src/hyperbee/resources/chat/__init__.py` & `hyperbee-0.0.1.5/src/hyperbee/resources/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.1.4/src/hyperbee/resources/chat/chat.py` & `hyperbee-0.0.1.5/src/hyperbee/resources/chat/chat.py`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.1.4/src/hyperbee/resources/chat/completions.py` & `hyperbee-0.0.1.5/src/hyperbee/resources/chat/completions.py`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.1.4/src/hyperbee/resources/pipeline/pipeline.py` & `hyperbee-0.0.1.5/src/hyperbee/resources/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.1.4/README.md` & `hyperbee-0.0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.1.4/pyproject.toml` & `hyperbee-0.0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "hyperbee"
-version = "0.0.1.4"
+version = "0.0.1.5"
 description = "The official Python library for the hyperbee API"
 readme = "README.md"
 license = "Apache-2.0"
 authors = [
 { name = "Hive", email = "support@hyperbee.ai" },
 ]
 dependencies = [
```

### Comparing `hyperbee-0.0.1.4/PKG-INFO` & `hyperbee-0.0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hyperbee
-Version: 0.0.1.4
+Version: 0.0.1.5
 Summary: The official Python library for the hyperbee API
 Project-URL: Homepage, https://github.com/HyperbeeAI/hive-python
 Project-URL: Repository, https://github.com/HyperbeeAI/hive-python
 Author-email: Hive <support@hyperbee.ai>
 License-Expression: Apache-2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

