# Comparing `tmp/kaizen_cloudcode-0.1.3.tar.gz` & `tmp/kaizen_cloudcode-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaizen_cloudcode-0.1.3.tar", max compression
+gzip compressed data, was "kaizen_cloudcode-0.1.4.tar", max compression
```

## Comparing `kaizen_cloudcode-0.1.3.tar` & `kaizen_cloudcode-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    34523 2024-05-14 14:00:21.029305 kaizen_cloudcode-0.1.3/LICENSE
--rw-r--r--   0        0        0     4135 2024-05-14 14:00:21.029305 kaizen_cloudcode-0.1.3/README.md
--rw-r--r--   0        0        0        0 2024-05-14 14:00:21.029305 kaizen_cloudcode-0.1.3/kaizen/actors/__init__.py
--rw-r--r--   0        0        0        0 2024-05-14 14:00:21.029305 kaizen_cloudcode-0.1.3/kaizen/generator/__init__.py
--rw-r--r--   0        0        0     3449 2024-05-14 14:00:21.033306 kaizen_cloudcode-0.1.3/kaizen/generator/ui.py
--rw-r--r--   0        0        0        0 2024-05-14 14:00:21.033306 kaizen_cloudcode-0.1.3/kaizen/helpers/__init__.py
--rw-r--r--   0        0        0        0 2024-05-14 14:00:21.033306 kaizen_cloudcode-0.1.3/kaizen/helpers/chunker.py
--rw-r--r--   0        0        0     1463 2024-05-14 14:00:21.033306 kaizen_cloudcode-0.1.3/kaizen/helpers/general.py
--rw-r--r--   0        0        0     3631 2024-05-14 14:00:21.033306 kaizen_cloudcode-0.1.3/kaizen/helpers/output.py
--rw-r--r--   0        0        0     1038 2024-05-14 14:00:21.033306 kaizen_cloudcode-0.1.3/kaizen/helpers/parser.py
--rw-r--r--   0        0        0        0 2024-05-14 14:00:21.033306 kaizen_cloudcode-0.1.3/kaizen/integrations/__init__.py
--rw-r--r--   0        0        0        0 2024-05-14 14:00:21.033306 kaizen_cloudcode-0.1.3/kaizen/llms/__init__.py
--rw-r--r--   0        0        0     7183 2024-05-14 14:00:21.033306 kaizen_cloudcode-0.1.3/kaizen/llms/prompts.py
--rw-r--r--   0        0        0     2217 2024-05-14 14:00:21.033306 kaizen_cloudcode-0.1.3/kaizen/llms/provider.py
--rw-r--r--   0        0        0        0 2024-05-14 14:00:21.033306 kaizen_cloudcode-0.1.3/kaizen/reviewer/__init__.py
--rw-r--r--   0        0        0     3395 2024-05-14 14:00:21.033306 kaizen_cloudcode-0.1.3/kaizen/reviewer/code_review.py
--rw-r--r--   0        0        0     1528 2024-05-14 14:00:21.033306 kaizen_cloudcode-0.1.3/kaizen/reviewer/work_summarizer.py
--rw-r--r--   0        0        0        0 2024-05-14 14:00:21.033306 kaizen_cloudcode-0.1.3/kaizen/utils/__init__.py
--rw-r--r--   0        0        0     1680 2024-05-14 14:00:21.033306 kaizen_cloudcode-0.1.3/kaizen/utils/config.py
--rw-r--r--   0        0        0      776 2024-05-14 14:00:21.033306 kaizen_cloudcode-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     5366 1970-01-01 00:00:00.000000 kaizen_cloudcode-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-16 08:16:33.344648 kaizen_cloudcode-0.1.4/LICENSE
+-rw-r--r--   0        0        0     4135 2024-05-16 08:16:33.348648 kaizen_cloudcode-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-16 08:16:33.348648 kaizen_cloudcode-0.1.4/kaizen/actors/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-16 08:16:33.348648 kaizen_cloudcode-0.1.4/kaizen/generator/__init__.py
+-rw-r--r--   0        0        0     3449 2024-05-16 08:16:33.348648 kaizen_cloudcode-0.1.4/kaizen/generator/ui.py
+-rw-r--r--   0        0        0        0 2024-05-16 08:16:33.348648 kaizen_cloudcode-0.1.4/kaizen/helpers/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-16 08:16:33.348648 kaizen_cloudcode-0.1.4/kaizen/helpers/chunker.py
+-rw-r--r--   0        0        0     1463 2024-05-16 08:16:33.348648 kaizen_cloudcode-0.1.4/kaizen/helpers/general.py
+-rw-r--r--   0        0        0     3631 2024-05-16 08:16:33.348648 kaizen_cloudcode-0.1.4/kaizen/helpers/output.py
+-rw-r--r--   0        0        0     1038 2024-05-16 08:16:33.348648 kaizen_cloudcode-0.1.4/kaizen/helpers/parser.py
+-rw-r--r--   0        0        0        0 2024-05-16 08:16:33.348648 kaizen_cloudcode-0.1.4/kaizen/integrations/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-16 08:16:33.348648 kaizen_cloudcode-0.1.4/kaizen/llms/__init__.py
+-rw-r--r--   0        0        0     7183 2024-05-16 08:16:33.352648 kaizen_cloudcode-0.1.4/kaizen/llms/prompts.py
+-rw-r--r--   0        0        0     2397 2024-05-16 08:16:33.352648 kaizen_cloudcode-0.1.4/kaizen/llms/provider.py
+-rw-r--r--   0        0        0        0 2024-05-16 08:16:33.352648 kaizen_cloudcode-0.1.4/kaizen/reviewer/__init__.py
+-rw-r--r--   0        0        0     3395 2024-05-16 08:16:33.352648 kaizen_cloudcode-0.1.4/kaizen/reviewer/code_review.py
+-rw-r--r--   0        0        0     1528 2024-05-16 08:16:33.352648 kaizen_cloudcode-0.1.4/kaizen/reviewer/work_summarizer.py
+-rw-r--r--   0        0        0        0 2024-05-16 08:16:33.352648 kaizen_cloudcode-0.1.4/kaizen/utils/__init__.py
+-rw-r--r--   0        0        0     1680 2024-05-16 08:16:33.352648 kaizen_cloudcode-0.1.4/kaizen/utils/config.py
+-rw-r--r--   0        0        0      776 2024-05-16 08:16:33.352648 kaizen_cloudcode-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5366 1970-01-01 00:00:00.000000 kaizen_cloudcode-0.1.4/PKG-INFO
```

### Comparing `kaizen_cloudcode-0.1.3/LICENSE` & `kaizen_cloudcode-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.3/README.md` & `kaizen_cloudcode-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.3/kaizen/generator/ui.py` & `kaizen_cloudcode-0.1.4/kaizen/generator/ui.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.3/kaizen/helpers/general.py` & `kaizen_cloudcode-0.1.4/kaizen/helpers/general.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.3/kaizen/helpers/output.py` & `kaizen_cloudcode-0.1.4/kaizen/helpers/output.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.3/kaizen/helpers/parser.py` & `kaizen_cloudcode-0.1.4/kaizen/helpers/parser.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.3/kaizen/llms/prompts.py` & `kaizen_cloudcode-0.1.4/kaizen/llms/prompts.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.3/kaizen/llms/provider.py` & `kaizen_cloudcode-0.1.4/kaizen/llms/provider.py`

 * *Files 7% similar despite different names*

```diff
@@ -61,7 +61,12 @@
         if total_usage is not None:
             total_usage = {
                 key: total_usage[key] + current_usage[key] for key in total_usage
             }
         else:
             total_usage = current_usage
         return total_usage
+
+    def get_usage_cost(self, total_usage):
+        return litellm.cost_per_token(
+            self.model, total_usage["prompt_tokens"], total_usage["completion_tokens"]
+        )
```

### Comparing `kaizen_cloudcode-0.1.3/kaizen/reviewer/code_review.py` & `kaizen_cloudcode-0.1.4/kaizen/reviewer/code_review.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.3/kaizen/reviewer/work_summarizer.py` & `kaizen_cloudcode-0.1.4/kaizen/reviewer/work_summarizer.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.3/kaizen/utils/config.py` & `kaizen_cloudcode-0.1.4/kaizen/utils/config.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.3/pyproject.toml` & `kaizen_cloudcode-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kaizen-cloudcode"
-version = "0.1.3"
+version = "0.1.4"
 description = "An intelligent coding companion that accelerates your development workflow by providing efficient assistance, enabling you to craft high-quality code more rapidly."
 authors = ["Saurav Panda <saurav.panda@cloudcode.ai>"]
 license = "Apache2.0"
 readme = "README.md"
 packages = [
     { include = "kaizen" }
 ]
```

### Comparing `kaizen_cloudcode-0.1.3/PKG-INFO` & `kaizen_cloudcode-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaizen-cloudcode
-Version: 0.1.3
+Version: 0.1.4
 Summary: An intelligent coding companion that accelerates your development workflow by providing efficient assistance, enabling you to craft high-quality code more rapidly.
 License: Apache2.0
 Author: Saurav Panda
 Author-email: saurav.panda@cloudcode.ai
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kaizen-cloudcode Version: 0.1.3 Summary: An
+Metadata-Version: 2.1 Name: kaizen-cloudcode Version: 0.1.4 Summary: An
 intelligent coding companion that accelerates your development workflow by
 providing efficient assistance, enabling you to craft high-quality code more
 rapidly. License: Apache2.0 Author: Saurav Panda Author-email:
 saurav.panda@cloudcode.ai Requires-Python: >=3.8.1,<4.0.0 Classifier: License
 :: Other/Proprietary License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

