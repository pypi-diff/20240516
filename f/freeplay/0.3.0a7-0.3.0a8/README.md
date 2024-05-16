# Comparing `tmp/freeplay-0.3.0a7.tar.gz` & `tmp/freeplay-0.3.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeplay-0.3.0a7.tar", max compression
+gzip compressed data, was "freeplay-0.3.0a8.tar", max compression
```

## Comparing `freeplay-0.3.0a7.tar` & `freeplay-0.3.0a8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1064 2024-01-12 20:28:56.461587 freeplay-0.3.0a7/LICENSE
--rw-r--r--   0        0        0      884 2024-01-30 20:26:04.166910 freeplay-0.3.0a7/README.md
--rw-r--r--   0        0        0      698 2024-05-14 19:12:33.900820 freeplay-0.3.0a7/pyproject.toml
--rw-r--r--   0        0        0      346 2024-03-25 14:26:20.961664 freeplay-0.3.0a7/src/freeplay/__init__.py
--rw-r--r--   0        0        0     2331 2024-03-14 18:04:56.167739 freeplay-0.3.0a7/src/freeplay/api_support.py
--rw-r--r--   0        0        0      631 2024-01-12 20:28:56.463431 freeplay-0.3.0a7/src/freeplay/errors.py
--rw-r--r--   0        0        0     1479 2024-03-25 14:26:20.962106 freeplay-0.3.0a7/src/freeplay/freeplay.py
--rw-r--r--   0        0        0     3460 2024-03-25 14:26:20.962659 freeplay-0.3.0a7/src/freeplay/freeplay_cli.py
--rw-r--r--   0        0        0      898 2024-01-12 20:28:56.464517 freeplay-0.3.0a7/src/freeplay/llm_parameters.py
--rw-r--r--   0        0        0      384 2024-03-25 14:26:20.963123 freeplay-0.3.0a7/src/freeplay/model.py
--rw-r--r--   0        0        0        0 2024-04-16 19:02:09.446684 freeplay-0.3.0a7/src/freeplay/py.typed
--rw-r--r--   0        0        0        0 2024-03-25 14:26:20.963202 freeplay-0.3.0a7/src/freeplay/resources/__init__.py
--rw-r--r--   0        0        0      527 2024-03-25 14:26:20.963455 freeplay-0.3.0a7/src/freeplay/resources/customer_feedback.py
--rw-r--r--   0        0        0    13352 2024-05-14 19:03:44.866443 freeplay-0.3.0a7/src/freeplay/resources/prompts.py
--rw-r--r--   0        0        0     5412 2024-04-16 19:02:09.447779 freeplay-0.3.0a7/src/freeplay/resources/recordings.py
--rw-r--r--   0        0        0      868 2024-03-25 14:26:20.963849 freeplay-0.3.0a7/src/freeplay/resources/sessions.py
--rw-r--r--   0        0        0     1452 2024-03-25 14:26:20.963926 freeplay-0.3.0a7/src/freeplay/resources/test_runs.py
--rw-r--r--   0        0        0     4532 2024-03-25 14:26:20.964330 freeplay-0.3.0a7/src/freeplay/support.py
--rw-r--r--   0        0        0     2064 2024-03-25 14:26:20.964602 freeplay-0.3.0a7/src/freeplay/utils.py
--rw-r--r--   0        0        0     1553 1970-01-01 00:00:00.000000 freeplay-0.3.0a7/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-01-12 20:28:56.461587 freeplay-0.3.0a8/LICENSE
+-rw-r--r--   0        0        0      884 2024-01-30 20:26:04.166910 freeplay-0.3.0a8/README.md
+-rw-r--r--   0        0        0      698 2024-05-16 20:58:01.670097 freeplay-0.3.0a8/pyproject.toml
+-rw-r--r--   0        0        0      346 2024-03-25 14:26:20.961664 freeplay-0.3.0a8/src/freeplay/__init__.py
+-rw-r--r--   0        0        0     2331 2024-03-14 18:04:56.167739 freeplay-0.3.0a8/src/freeplay/api_support.py
+-rw-r--r--   0        0        0      631 2024-01-12 20:28:56.463431 freeplay-0.3.0a8/src/freeplay/errors.py
+-rw-r--r--   0        0        0     1479 2024-03-25 14:26:20.962106 freeplay-0.3.0a8/src/freeplay/freeplay.py
+-rw-r--r--   0        0        0     3460 2024-03-25 14:26:20.962659 freeplay-0.3.0a8/src/freeplay/freeplay_cli.py
+-rw-r--r--   0        0        0      898 2024-01-12 20:28:56.464517 freeplay-0.3.0a8/src/freeplay/llm_parameters.py
+-rw-r--r--   0        0        0      384 2024-03-25 14:26:20.963123 freeplay-0.3.0a8/src/freeplay/model.py
+-rw-r--r--   0        0        0        0 2024-04-16 19:02:09.446684 freeplay-0.3.0a8/src/freeplay/py.typed
+-rw-r--r--   0        0        0        0 2024-03-25 14:26:20.963202 freeplay-0.3.0a8/src/freeplay/resources/__init__.py
+-rw-r--r--   0        0        0      527 2024-03-25 14:26:20.963455 freeplay-0.3.0a8/src/freeplay/resources/customer_feedback.py
+-rw-r--r--   0        0        0    13352 2024-05-14 19:03:44.866443 freeplay-0.3.0a8/src/freeplay/resources/prompts.py
+-rw-r--r--   0        0        0     5614 2024-05-16 20:45:23.454638 freeplay-0.3.0a8/src/freeplay/resources/recordings.py
+-rw-r--r--   0        0        0      868 2024-03-25 14:26:20.963849 freeplay-0.3.0a8/src/freeplay/resources/sessions.py
+-rw-r--r--   0        0        0     1612 2024-05-16 20:45:23.454944 freeplay-0.3.0a8/src/freeplay/resources/test_runs.py
+-rw-r--r--   0        0        0     4692 2024-05-16 20:45:23.455378 freeplay-0.3.0a8/src/freeplay/support.py
+-rw-r--r--   0        0        0     2064 2024-03-25 14:26:20.964602 freeplay-0.3.0a8/src/freeplay/utils.py
+-rw-r--r--   0        0        0     1553 1970-01-01 00:00:00.000000 freeplay-0.3.0a8/PKG-INFO
```

### Comparing `freeplay-0.3.0a7/LICENSE` & `freeplay-0.3.0a8/LICENSE`

 * *Files identical despite different names*

### Comparing `freeplay-0.3.0a7/README.md` & `freeplay-0.3.0a8/README.md`

 * *Files identical despite different names*

### Comparing `freeplay-0.3.0a7/pyproject.toml` & `freeplay-0.3.0a8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "freeplay"
-version = "0.3.0-alpha.7"
+version = "0.3.0-alpha.8"
 description = ""
 authors = ["FreePlay Engineering <engineering@freeplay.ai>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <4"
```

### Comparing `freeplay-0.3.0a7/src/freeplay/api_support.py` & `freeplay-0.3.0a8/src/freeplay/api_support.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.3.0a7/src/freeplay/errors.py` & `freeplay-0.3.0a8/src/freeplay/errors.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.3.0a7/src/freeplay/freeplay.py` & `freeplay-0.3.0a8/src/freeplay/freeplay.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.3.0a7/src/freeplay/freeplay_cli.py` & `freeplay-0.3.0a8/src/freeplay/freeplay_cli.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.3.0a7/src/freeplay/llm_parameters.py` & `freeplay-0.3.0a8/src/freeplay/llm_parameters.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.3.0a7/src/freeplay/resources/customer_feedback.py` & `freeplay-0.3.0a8/src/freeplay/resources/customer_feedback.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.3.0a7/src/freeplay/resources/prompts.py` & `freeplay-0.3.0a8/src/freeplay/resources/prompts.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.3.0a7/src/freeplay/resources/recordings.py` & `freeplay-0.3.0a8/src/freeplay/resources/recordings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import logging
 from dataclasses import dataclass
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
 from requests import HTTPError
 
 from freeplay import api_support
 from freeplay.errors import FreeplayClientError, FreeplayError
 from freeplay.llm_parameters import LLMParameters
 from freeplay.model import InputVariables, OpenAIFunctionCall
@@ -57,14 +57,15 @@
     inputs: InputVariables
 
     session_info: SessionInfo
     prompt_info: PromptInfo
     call_info: CallInfo
     response_info: ResponseInfo
     test_run_info: Optional[TestRunInfo] = None
+    eval_results: Optional[Dict[str, Union[bool, float]]] = None
 
 
 @dataclass
 class RecordResponse:
     completion_id: str
 
 
@@ -107,14 +108,17 @@
 
         if record_payload.test_run_info is not None:
             record_api_payload['test_run_id'] = record_payload.test_run_info.test_run_id
 
         if record_payload.test_run_info is not None:
             record_api_payload['test_case_id'] = record_payload.test_run_info.test_case_id
 
+        if record_payload.eval_results is not None:
+            record_api_payload['eval_results'] = record_payload.eval_results
+
         try:
             recorded_response = api_support.post_raw(
                 api_key=self.call_support.freeplay_api_key,
                 url=f'{self.call_support.api_base}/v1/record',
                 payload=record_api_payload
             )
             recorded_response.raise_for_status()
```

### Comparing `freeplay-0.3.0a7/src/freeplay/resources/sessions.py` & `freeplay-0.3.0a8/src/freeplay/resources/sessions.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.3.0a7/src/freeplay/resources/test_runs.py` & `freeplay-0.3.0a8/src/freeplay/resources/test_runs.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,15 +36,22 @@
         return TestRunInfo(self.test_run_id, test_case_id)
 
 
 class TestRuns:
     def __init__(self, call_support: CallSupport) -> None:
         self.call_support = call_support
 
-    def create(self, project_id: str, testlist: str, include_outputs: bool = False) -> TestRun:
-        test_run = self.call_support.create_test_run(project_id, testlist, include_outputs)
+    def create(
+            self,
+            project_id: str,
+            testlist: str,
+            include_outputs: bool = False,
+            name: Optional[str] = None,
+            description: Optional[str] = None
+    ) -> TestRun:
+        test_run = self.call_support.create_test_run(project_id, testlist, include_outputs, name, description)
         test_cases = [
             TestCase(test_case_id=test_case.id, variables=test_case.variables, output=test_case.output)
             for test_case in test_run.test_cases
         ]
 
         return TestRun(test_run.test_run_id, test_cases)
```

### Comparing `freeplay-0.3.0a7/src/freeplay/support.py` & `freeplay-0.3.0a8/src/freeplay/support.py`

 * *Files 8% similar despite different names*

```diff
@@ -119,22 +119,26 @@
         if response.status_code != 201:
             raise freeplay_response_error("Error updating customer feedback", response)
 
     def create_test_run(
             self,
             project_id: str,
             testlist: str,
-            include_test_case_outputs: bool = False
+            include_test_case_outputs: bool = False,
+            name: Optional[str] = None,
+            description: Optional[str] = None
     ) -> TestRunResponse:
         response = api_support.post_raw(
             api_key=self.freeplay_api_key,
             url=f'{self.api_base}/projects/{project_id}/test-runs-cases',
             payload={
                 'testlist_name': testlist,
                 'include_test_case_outputs': include_test_case_outputs,
+                'name': name,
+                'description': description
             },
         )
 
         if response.status_code != 201:
             raise freeplay_response_error('Error while creating a test run.', response)
 
         json_dom = response.json()
```

### Comparing `freeplay-0.3.0a7/src/freeplay/utils.py` & `freeplay-0.3.0a8/src/freeplay/utils.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.3.0a7/PKG-INFO` & `freeplay-0.3.0a8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeplay
-Version: 0.3.0a7
+Version: 0.3.0a8
 Summary: 
 License: MIT
 Author: FreePlay Engineering
 Author-email: engineering@freeplay.ai
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

