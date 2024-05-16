# Comparing `tmp/dalpha-0.5.1.tar.gz` & `tmp/dalpha-0.5.2rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dalpha-0.5.1.tar", max compression
+gzip compressed data, was "dalpha-0.5.2rc0.tar", max compression
```

## Comparing `dalpha-0.5.1.tar` & `dalpha-0.5.2rc0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      578 2023-12-18 04:10:26.318635 dalpha-0.5.1/README.md
--rw-r--r--   0        0        0     2028 2024-05-15 07:56:58.860556 dalpha-0.5.1/dalpha/__init__.py
--rw-r--r--   0        0        0     8194 2024-05-13 09:40:01.895738 dalpha-0.5.1/dalpha/agent.py
--rw-r--r--   0        0        0     7019 2024-05-10 10:54:52.512416 dalpha-0.5.1/dalpha/backend_cli.py
--rw-r--r--   0        0        0      555 2024-05-08 06:25:10.211719 dalpha-0.5.1/dalpha/cobra_cls.py
--rw-r--r--   0        0        0      573 2024-02-28 08:10:55.063883 dalpha-0.5.1/dalpha/context.py
--rw-r--r--   0        0        0     3036 2024-05-02 07:23:00.795089 dalpha-0.5.1/dalpha/data_update_cls.py
--rw-r--r--   0        0        0      940 2024-05-02 07:23:00.795089 dalpha-0.5.1/dalpha/dto.py
--rw-r--r--   0        0        0      579 2024-05-10 10:54:52.512416 dalpha-0.5.1/dalpha/exception.py
--rw-r--r--   0        0        0     6022 2024-05-13 09:17:22.448483 dalpha-0.5.1/dalpha/inference_cls.py
--rw-r--r--   0        0        0      233 2024-03-25 02:37:47.094337 dalpha-0.5.1/dalpha/kafka_cli.py
--rw-r--r--   0        0        0     1861 2024-03-11 02:52:37.986799 dalpha-0.5.1/dalpha/logging/__init__.py
--rw-r--r--   0        0        0      229 2024-02-28 08:10:55.063883 dalpha-0.5.1/dalpha/logging/events.py
--rw-r--r--   0        0        0     1116 2024-02-28 08:10:55.063883 dalpha-0.5.1/dalpha/logging/log_formatter.py
--rw-r--r--   0        0        0     1817 2024-02-28 08:10:55.063883 dalpha-0.5.1/dalpha/logging/utils.py
--rw-r--r--   0        0        0     6625 2024-05-13 09:40:01.895738 dalpha-0.5.1/dalpha/message_consumer.py
--rw-r--r--   0        0        0     1703 2024-05-10 10:54:52.512416 dalpha-0.5.1/dalpha/openai_cls.py
--rw-r--r--   0        0        0     6079 2024-05-02 07:23:00.795089 dalpha-0.5.1/dalpha/redis_cli.py
--rw-r--r--   0        0        0     1886 2024-05-02 07:23:00.795089 dalpha-0.5.1/dalpha/redis_cls.py
--rw-r--r--   0        0        0      776 2024-05-10 10:54:52.512416 dalpha-0.5.1/dalpha/request.py
--rw-r--r--   0        0        0     2689 2024-05-10 10:54:52.512416 dalpha-0.5.1/dalpha/s3.py
--rw-r--r--   0        0        0      497 2024-02-28 08:10:55.063883 dalpha-0.5.1/dalpha/signal_handler.py
--rw-r--r--   0        0        0      767 2024-05-10 10:54:52.512416 dalpha-0.5.1/dalpha/slack.py
--rw-r--r--   0        0        0     2355 2024-05-10 10:54:52.512416 dalpha-0.5.1/dalpha/update_agent.py
--rw-r--r--   0        0        0      946 2024-05-15 07:56:58.860556 dalpha-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     1359 1970-01-01 00:00:00.000000 dalpha-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      578 2023-12-18 04:10:26.318635 dalpha-0.5.2rc0/README.md
+-rw-r--r--   0        0        0     2077 2024-05-16 07:16:07.976796 dalpha-0.5.2rc0/dalpha/__init__.py
+-rw-r--r--   0        0        0     8184 2024-05-16 07:16:07.980796 dalpha-0.5.2rc0/dalpha/agent.py
+-rw-r--r--   0        0        0     7019 2024-05-10 10:54:52.512416 dalpha-0.5.2rc0/dalpha/backend_cli.py
+-rw-r--r--   0        0        0      555 2024-05-08 06:25:10.211719 dalpha-0.5.2rc0/dalpha/cobra_cls.py
+-rw-r--r--   0        0        0      573 2024-02-28 08:10:55.063883 dalpha-0.5.2rc0/dalpha/context.py
+-rw-r--r--   0        0        0     3036 2024-05-02 07:23:00.795089 dalpha-0.5.2rc0/dalpha/data_update_cls.py
+-rw-r--r--   0        0        0      940 2024-05-02 07:23:00.795089 dalpha-0.5.2rc0/dalpha/dto.py
+-rw-r--r--   0        0        0      616 2024-05-16 07:16:07.980796 dalpha-0.5.2rc0/dalpha/exception.py
+-rw-r--r--   0        0        0     5954 2024-05-16 07:16:07.980796 dalpha-0.5.2rc0/dalpha/inference_cls.py
+-rw-r--r--   0        0        0      233 2024-03-25 02:37:47.094337 dalpha-0.5.2rc0/dalpha/kafka_cli.py
+-rw-r--r--   0        0        0     1861 2024-03-11 02:52:37.986799 dalpha-0.5.2rc0/dalpha/logging/__init__.py
+-rw-r--r--   0        0        0      229 2024-02-28 08:10:55.063883 dalpha-0.5.2rc0/dalpha/logging/events.py
+-rw-r--r--   0        0        0     1116 2024-02-28 08:10:55.063883 dalpha-0.5.2rc0/dalpha/logging/log_formatter.py
+-rw-r--r--   0        0        0     1817 2024-02-28 08:10:55.063883 dalpha-0.5.2rc0/dalpha/logging/utils.py
+-rw-r--r--   0        0        0     6625 2024-05-13 09:40:01.895738 dalpha-0.5.2rc0/dalpha/message_consumer.py
+-rw-r--r--   0        0        0     1703 2024-05-10 10:54:52.512416 dalpha-0.5.2rc0/dalpha/openai_cls.py
+-rw-r--r--   0        0        0     6079 2024-05-02 07:23:00.795089 dalpha-0.5.2rc0/dalpha/redis_cli.py
+-rw-r--r--   0        0        0     1886 2024-05-02 07:23:00.795089 dalpha-0.5.2rc0/dalpha/redis_cls.py
+-rw-r--r--   0        0        0      776 2024-05-10 10:54:52.512416 dalpha-0.5.2rc0/dalpha/request.py
+-rw-r--r--   0        0        0     2689 2024-05-10 10:54:52.512416 dalpha-0.5.2rc0/dalpha/s3.py
+-rw-r--r--   0        0        0      497 2024-02-28 08:10:55.063883 dalpha-0.5.2rc0/dalpha/signal_handler.py
+-rw-r--r--   0        0        0      767 2024-05-10 10:54:52.512416 dalpha-0.5.2rc0/dalpha/slack.py
+-rw-r--r--   0        0        0     2355 2024-05-10 10:54:52.512416 dalpha-0.5.2rc0/dalpha/update_agent.py
+-rw-r--r--   0        0        0      952 2024-05-16 07:16:07.980796 dalpha-0.5.2rc0/pyproject.toml
+-rw-r--r--   0        0        0     1362 1970-01-01 00:00:00.000000 dalpha-0.5.2rc0/PKG-INFO
```

### Comparing `dalpha-0.5.1/README.md` & `dalpha-0.5.2rc0/README.md`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.1/dalpha/__init__.py` & `dalpha-0.5.2rc0/dalpha/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,8 +47,9 @@
 from dalpha.agent import Agent
 from dalpha.cobra_cls import Cobra
 from dalpha.data_update_cls import DalphaDataUpdater
 from dalpha.inference_cls import DalphaAI
 from dalpha.redis_cls import DalphaRedis
 from dalpha.openai_cls import DalphaOpenAI
 from dalpha.backend_cli import BackendCli, internal_call
+from dalpha.message_consumer import EvaluateItem
 import dalpha.s3 as s3
```

### Comparing `dalpha-0.5.1/dalpha/agent.py` & `dalpha-0.5.2rc0/dalpha/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,36 +137,37 @@
             return self.mock
 
         ret: List[EvaluateItem] = self.message_consumer.poll()
         if len(ret) == 0:
             # 가져온 메세지가 없으면 None 반환
             return None
         elif len(ret) == 1:
+            print(ret)
             # 가져온 메세지가 1개면 list 형태가 아닌 낱개로 반환
             logger.info(
                 message = f"return evaluate item: {ret[0]}",
                 event = Event.POLL,
                 data = ret[0]
             )
             set_context_evaluate(
                 evaluate_id=ret[0].id,
                 account_id=ret[0].accountId
             )
             sentry_sdk.set_context("context",asdict(get_context()))
             self.poll_time = time.time()
-            return ret[0].dict()
+            return ret[0]
         else:
             # 가져온 메세지가 여러개면 list 형태로 반환
             logger.info(
                 message = f"return evaluate item: {ret}",
                 event = Event.POLL,
                 data = ret
             )
             self.poll_time = time.time()
-            return [item.dict() for item in ret]
+            return ret
         
     def validate(self, evaluate_id, output, mock=True, log=True, inference_time=None, usage=1):
         try:
             if mock:
                 logger.info(message = f"validate payload - {output}")
                 return
             if inference_time == None and self.poll_time != None:
```

### Comparing `dalpha-0.5.1/dalpha/backend_cli.py` & `dalpha-0.5.2rc0/dalpha/backend_cli.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.1/dalpha/cobra_cls.py` & `dalpha-0.5.2rc0/dalpha/cobra_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.1/dalpha/context.py` & `dalpha-0.5.2rc0/dalpha/context.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.1/dalpha/data_update_cls.py` & `dalpha-0.5.2rc0/dalpha/data_update_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.1/dalpha/dto.py` & `dalpha-0.5.2rc0/dalpha/dto.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.1/dalpha/exception.py` & `dalpha-0.5.2rc0/dalpha/exception.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,7 +14,8 @@
         super().__init__(message)
 
 
 class ExpectedError(Exception):
     def __init__(self, error_json: Dict, error_code: BaseStatusCode = BaseStatusCode.INTERNAL_ERROR, message: str = "Expected Error occured"):
         super().__init__(message)
         self.error_json = error_json
+        self.error_code = error_code
```

### Comparing `dalpha-0.5.1/dalpha/inference_cls.py` & `dalpha-0.5.2rc0/dalpha/inference_cls.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,21 +5,22 @@
 from copy import deepcopy
 from typing import Callable, Dict, List, Literal, Optional, Tuple, Union
 
 from dalpha.agent import Agent
 from dalpha.dto import InferenceResult
 from dalpha.exception import ExpectedError, WaitException
 from dalpha.logging import logger
+from dalpha.message_consumer import EvaluateItem
 
 
 class DalphaAI:
     def __init__(
         self,
         api_id: int,
-        inference: Callable[[Agent, Dict, Dict, int, int], InferenceResult],
+        inference: Callable[[Dict, EvaluateItem], InferenceResult],
         load_globals: Callable[[], Dict],
         mock_file: Optional[str],
         mocks_file: Optional[str],
     ):
         self.wait_flag = True
 
         self.agent = Agent(api_id=api_id)
@@ -108,36 +109,33 @@
         logger.info(f"\n\033[31m\n\t| MOCK DATA : {self.mock_info}\n\033[0m")
         logger.info("processing...")
 
         try:
             # read input.
             # dynamic-type 으로 만든 경우 metadata가 input과 같습니다.
             eval_id, account_id, metadata = (
-                input_json["id"],
-                input_json["accountId"],
-                input_json["metadata"],
+                input_json.id,
+                input_json.accountId,
+                input_json.metadata
             )
         except KeyError as e:
             logger.warning(f"input_json format is not correct!")
             error_json = {"reason": f"input_json format is not correct!\n{e}"}
             self.agent.validate_error(evaluate_id=eval_id, output=error_json, mock=self.is_mock)
             self.wait_flag = True
             return
 
         # inference
         try:
             logger.info("AI inference starts...")
             inference_start_time = time.time()
 
             inference_result: InferenceResult = self.inference(
-                agent=self.agent,
                 globals=self.globals,
-                metadata=metadata,
-                eval_id=eval_id,
-                account_id=account_id
+                evaluate_item=input_json,
             )
             inference_end_time = time.time()
             logger.info(f"AI inference is done. Time taken: {inference_end_time - inference_start_time:.2f} sec")
         except ExpectedError as expected_error:
             self.agent.validate_error(evaluate_id=eval_id, output=expected_error.error_json, mock=self.is_mock, error_code=expected_error.error_code)
             self.wait_flag = True
             return
```

### Comparing `dalpha-0.5.1/dalpha/logging/__init__.py` & `dalpha-0.5.2rc0/dalpha/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.1/dalpha/logging/log_formatter.py` & `dalpha-0.5.2rc0/dalpha/logging/log_formatter.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.1/dalpha/logging/utils.py` & `dalpha-0.5.2rc0/dalpha/logging/utils.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.1/dalpha/message_consumer.py` & `dalpha-0.5.2rc0/dalpha/message_consumer.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.1/dalpha/openai_cls.py` & `dalpha-0.5.2rc0/dalpha/openai_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.1/dalpha/redis_cli.py` & `dalpha-0.5.2rc0/dalpha/redis_cli.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.1/dalpha/redis_cls.py` & `dalpha-0.5.2rc0/dalpha/redis_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.1/dalpha/request.py` & `dalpha-0.5.2rc0/dalpha/request.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.1/dalpha/s3.py` & `dalpha-0.5.2rc0/dalpha/s3.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.1/dalpha/slack.py` & `dalpha-0.5.2rc0/dalpha/slack.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.1/dalpha/update_agent.py` & `dalpha-0.5.2rc0/dalpha/update_agent.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.1/PKG-INFO` & `dalpha-0.5.2rc0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalpha
-Version: 0.5.1
+Version: 0.5.2rc0
 Summary: 
 Author: devops
 Author-email: devops@dalpha.so
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

