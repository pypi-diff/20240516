# Comparing `tmp/dalpha-0.5.2rc0.tar.gz` & `tmp/dalpha-0.5.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dalpha-0.5.2rc0.tar", max compression
+gzip compressed data, was "dalpha-0.5.2rc1.tar", max compression
```

## Comparing `dalpha-0.5.2rc0.tar` & `dalpha-0.5.2rc1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      578 2023-12-18 04:10:26.318635 dalpha-0.5.2rc0/README.md
--rw-r--r--   0        0        0     2077 2024-05-16 07:16:07.976796 dalpha-0.5.2rc0/dalpha/__init__.py
--rw-r--r--   0        0        0     8184 2024-05-16 07:16:07.980796 dalpha-0.5.2rc0/dalpha/agent.py
--rw-r--r--   0        0        0     7019 2024-05-10 10:54:52.512416 dalpha-0.5.2rc0/dalpha/backend_cli.py
--rw-r--r--   0        0        0      555 2024-05-08 06:25:10.211719 dalpha-0.5.2rc0/dalpha/cobra_cls.py
--rw-r--r--   0        0        0      573 2024-02-28 08:10:55.063883 dalpha-0.5.2rc0/dalpha/context.py
--rw-r--r--   0        0        0     3036 2024-05-02 07:23:00.795089 dalpha-0.5.2rc0/dalpha/data_update_cls.py
--rw-r--r--   0        0        0      940 2024-05-02 07:23:00.795089 dalpha-0.5.2rc0/dalpha/dto.py
--rw-r--r--   0        0        0      616 2024-05-16 07:16:07.980796 dalpha-0.5.2rc0/dalpha/exception.py
--rw-r--r--   0        0        0     5954 2024-05-16 07:16:07.980796 dalpha-0.5.2rc0/dalpha/inference_cls.py
--rw-r--r--   0        0        0      233 2024-03-25 02:37:47.094337 dalpha-0.5.2rc0/dalpha/kafka_cli.py
--rw-r--r--   0        0        0     1861 2024-03-11 02:52:37.986799 dalpha-0.5.2rc0/dalpha/logging/__init__.py
--rw-r--r--   0        0        0      229 2024-02-28 08:10:55.063883 dalpha-0.5.2rc0/dalpha/logging/events.py
--rw-r--r--   0        0        0     1116 2024-02-28 08:10:55.063883 dalpha-0.5.2rc0/dalpha/logging/log_formatter.py
--rw-r--r--   0        0        0     1817 2024-02-28 08:10:55.063883 dalpha-0.5.2rc0/dalpha/logging/utils.py
--rw-r--r--   0        0        0     6625 2024-05-13 09:40:01.895738 dalpha-0.5.2rc0/dalpha/message_consumer.py
--rw-r--r--   0        0        0     1703 2024-05-10 10:54:52.512416 dalpha-0.5.2rc0/dalpha/openai_cls.py
--rw-r--r--   0        0        0     6079 2024-05-02 07:23:00.795089 dalpha-0.5.2rc0/dalpha/redis_cli.py
--rw-r--r--   0        0        0     1886 2024-05-02 07:23:00.795089 dalpha-0.5.2rc0/dalpha/redis_cls.py
--rw-r--r--   0        0        0      776 2024-05-10 10:54:52.512416 dalpha-0.5.2rc0/dalpha/request.py
--rw-r--r--   0        0        0     2689 2024-05-10 10:54:52.512416 dalpha-0.5.2rc0/dalpha/s3.py
--rw-r--r--   0        0        0      497 2024-02-28 08:10:55.063883 dalpha-0.5.2rc0/dalpha/signal_handler.py
--rw-r--r--   0        0        0      767 2024-05-10 10:54:52.512416 dalpha-0.5.2rc0/dalpha/slack.py
--rw-r--r--   0        0        0     2355 2024-05-10 10:54:52.512416 dalpha-0.5.2rc0/dalpha/update_agent.py
--rw-r--r--   0        0        0      952 2024-05-16 07:16:07.980796 dalpha-0.5.2rc0/pyproject.toml
--rw-r--r--   0        0        0     1362 1970-01-01 00:00:00.000000 dalpha-0.5.2rc0/PKG-INFO
+-rw-r--r--   0        0        0      578 2023-12-18 04:10:26.318635 dalpha-0.5.2rc1/README.md
+-rw-r--r--   0        0        0     2077 2024-05-16 07:16:07.976796 dalpha-0.5.2rc1/dalpha/__init__.py
+-rw-r--r--   0        0        0     8238 2024-05-16 13:20:42.129689 dalpha-0.5.2rc1/dalpha/agent.py
+-rw-r--r--   0        0        0     7019 2024-05-10 10:54:52.512416 dalpha-0.5.2rc1/dalpha/backend_cli.py
+-rw-r--r--   0        0        0      555 2024-05-08 06:25:10.211719 dalpha-0.5.2rc1/dalpha/cobra_cls.py
+-rw-r--r--   0        0        0      573 2024-02-28 08:10:55.063883 dalpha-0.5.2rc1/dalpha/context.py
+-rw-r--r--   0        0        0     3036 2024-05-02 07:23:00.795089 dalpha-0.5.2rc1/dalpha/data_update_cls.py
+-rw-r--r--   0        0        0      940 2024-05-02 07:23:00.795089 dalpha-0.5.2rc1/dalpha/dto.py
+-rw-r--r--   0        0        0      616 2024-05-16 07:16:07.980796 dalpha-0.5.2rc1/dalpha/exception.py
+-rw-r--r--   0        0        0     5954 2024-05-16 07:16:07.980796 dalpha-0.5.2rc1/dalpha/inference_cls.py
+-rw-r--r--   0        0        0      233 2024-03-25 02:37:47.094337 dalpha-0.5.2rc1/dalpha/kafka_cli.py
+-rw-r--r--   0        0        0     1861 2024-03-11 02:52:37.986799 dalpha-0.5.2rc1/dalpha/logging/__init__.py
+-rw-r--r--   0        0        0      229 2024-02-28 08:10:55.063883 dalpha-0.5.2rc1/dalpha/logging/events.py
+-rw-r--r--   0        0        0     1116 2024-02-28 08:10:55.063883 dalpha-0.5.2rc1/dalpha/logging/log_formatter.py
+-rw-r--r--   0        0        0     1817 2024-02-28 08:10:55.063883 dalpha-0.5.2rc1/dalpha/logging/utils.py
+-rw-r--r--   0        0        0     6625 2024-05-13 09:40:01.895738 dalpha-0.5.2rc1/dalpha/message_consumer.py
+-rw-r--r--   0        0        0     1703 2024-05-10 10:54:52.512416 dalpha-0.5.2rc1/dalpha/openai_cls.py
+-rw-r--r--   0        0        0     6079 2024-05-02 07:23:00.795089 dalpha-0.5.2rc1/dalpha/redis_cli.py
+-rw-r--r--   0        0        0     1886 2024-05-02 07:23:00.795089 dalpha-0.5.2rc1/dalpha/redis_cls.py
+-rw-r--r--   0        0        0      776 2024-05-10 10:54:52.512416 dalpha-0.5.2rc1/dalpha/request.py
+-rw-r--r--   0        0        0     2689 2024-05-10 10:54:52.512416 dalpha-0.5.2rc1/dalpha/s3.py
+-rw-r--r--   0        0        0      497 2024-02-28 08:10:55.063883 dalpha-0.5.2rc1/dalpha/signal_handler.py
+-rw-r--r--   0        0        0      767 2024-05-10 10:54:52.512416 dalpha-0.5.2rc1/dalpha/slack.py
+-rw-r--r--   0        0        0     2355 2024-05-10 10:54:52.512416 dalpha-0.5.2rc1/dalpha/update_agent.py
+-rw-r--r--   0        0        0      952 2024-05-16 13:20:42.129689 dalpha-0.5.2rc1/pyproject.toml
+-rw-r--r--   0        0        0     1362 1970-01-01 00:00:00.000000 dalpha-0.5.2rc1/PKG-INFO
```

### Comparing `dalpha-0.5.2rc0/README.md` & `dalpha-0.5.2rc1/README.md`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc0/dalpha/__init__.py` & `dalpha-0.5.2rc1/dalpha/__init__.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc0/dalpha/agent.py` & `dalpha-0.5.2rc1/dalpha/agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys, os
 import time
 import sentry_sdk
 from dataclasses import asdict
 from typing import List
 
 from dalpha.backend_cli import BackendCli
-from dalpha.message_consumer import EvaluateItem, KafkaMessageConsumer, RawMessageConsumer, SqsMessageConsumer
+from dalpha.message_consumer import EvaluateItem, KafkaMessageConsumer, RawMessageConsumer, SqsMessageConsumer, to_evaluate_item
 from dalpha.signal_handler import get_shutdown_requested
 from dalpha.context import clear_context_evaluate, set_context, set_context_evaluate, get_context, Context
 from dalpha.logging import logger
 from dalpha.logging.events import Event
 
 from dalpha.exception import BaseStatusCode
 
@@ -128,17 +128,17 @@
             self.message_consumer.close()
             sys.exit(0)
         if not isinstance(max_number_of_messages,int): TypeError("max_number_of_messages is not a int")
         if not isinstance(mock, bool): TypeError("mock is not a bool")
         if mock:
             logger.info(
                 "return mock",
-                data = self.mock
+                data = to_evaluate_item(self.mock)
             )
-            return self.mock
+            return to_evaluate_item(self.mock)
 
         ret: List[EvaluateItem] = self.message_consumer.poll()
         if len(ret) == 0:
             # 가져온 메세지가 없으면 None 반환
             return None
         elif len(ret) == 1:
             print(ret)
```

### Comparing `dalpha-0.5.2rc0/dalpha/backend_cli.py` & `dalpha-0.5.2rc1/dalpha/backend_cli.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc0/dalpha/cobra_cls.py` & `dalpha-0.5.2rc1/dalpha/cobra_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc0/dalpha/context.py` & `dalpha-0.5.2rc1/dalpha/context.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc0/dalpha/data_update_cls.py` & `dalpha-0.5.2rc1/dalpha/data_update_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc0/dalpha/dto.py` & `dalpha-0.5.2rc1/dalpha/dto.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc0/dalpha/exception.py` & `dalpha-0.5.2rc1/dalpha/exception.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc0/dalpha/inference_cls.py` & `dalpha-0.5.2rc1/dalpha/inference_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc0/dalpha/logging/__init__.py` & `dalpha-0.5.2rc1/dalpha/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc0/dalpha/logging/log_formatter.py` & `dalpha-0.5.2rc1/dalpha/logging/log_formatter.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc0/dalpha/logging/utils.py` & `dalpha-0.5.2rc1/dalpha/logging/utils.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc0/dalpha/message_consumer.py` & `dalpha-0.5.2rc1/dalpha/message_consumer.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc0/dalpha/openai_cls.py` & `dalpha-0.5.2rc1/dalpha/openai_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc0/dalpha/redis_cli.py` & `dalpha-0.5.2rc1/dalpha/redis_cli.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc0/dalpha/redis_cls.py` & `dalpha-0.5.2rc1/dalpha/redis_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc0/dalpha/request.py` & `dalpha-0.5.2rc1/dalpha/request.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc0/dalpha/s3.py` & `dalpha-0.5.2rc1/dalpha/s3.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc0/dalpha/slack.py` & `dalpha-0.5.2rc1/dalpha/slack.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc0/dalpha/update_agent.py` & `dalpha-0.5.2rc1/dalpha/update_agent.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc0/PKG-INFO` & `dalpha-0.5.2rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalpha
-Version: 0.5.2rc0
+Version: 0.5.2rc1
 Summary: 
 Author: devops
 Author-email: devops@dalpha.so
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

