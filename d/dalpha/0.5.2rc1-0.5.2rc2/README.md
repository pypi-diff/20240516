# Comparing `tmp/dalpha-0.5.2rc1.tar.gz` & `tmp/dalpha-0.5.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dalpha-0.5.2rc1.tar", max compression
+gzip compressed data, was "dalpha-0.5.2rc2.tar", max compression
```

## Comparing `dalpha-0.5.2rc1.tar` & `dalpha-0.5.2rc2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      578 2023-12-18 04:10:26.318635 dalpha-0.5.2rc1/README.md
--rw-r--r--   0        0        0     2077 2024-05-16 07:16:07.976796 dalpha-0.5.2rc1/dalpha/__init__.py
--rw-r--r--   0        0        0     8238 2024-05-16 13:20:42.129689 dalpha-0.5.2rc1/dalpha/agent.py
--rw-r--r--   0        0        0     7019 2024-05-10 10:54:52.512416 dalpha-0.5.2rc1/dalpha/backend_cli.py
--rw-r--r--   0        0        0      555 2024-05-08 06:25:10.211719 dalpha-0.5.2rc1/dalpha/cobra_cls.py
--rw-r--r--   0        0        0      573 2024-02-28 08:10:55.063883 dalpha-0.5.2rc1/dalpha/context.py
--rw-r--r--   0        0        0     3036 2024-05-02 07:23:00.795089 dalpha-0.5.2rc1/dalpha/data_update_cls.py
--rw-r--r--   0        0        0      940 2024-05-02 07:23:00.795089 dalpha-0.5.2rc1/dalpha/dto.py
--rw-r--r--   0        0        0      616 2024-05-16 07:16:07.980796 dalpha-0.5.2rc1/dalpha/exception.py
--rw-r--r--   0        0        0     5954 2024-05-16 07:16:07.980796 dalpha-0.5.2rc1/dalpha/inference_cls.py
--rw-r--r--   0        0        0      233 2024-03-25 02:37:47.094337 dalpha-0.5.2rc1/dalpha/kafka_cli.py
--rw-r--r--   0        0        0     1861 2024-03-11 02:52:37.986799 dalpha-0.5.2rc1/dalpha/logging/__init__.py
--rw-r--r--   0        0        0      229 2024-02-28 08:10:55.063883 dalpha-0.5.2rc1/dalpha/logging/events.py
--rw-r--r--   0        0        0     1116 2024-02-28 08:10:55.063883 dalpha-0.5.2rc1/dalpha/logging/log_formatter.py
--rw-r--r--   0        0        0     1817 2024-02-28 08:10:55.063883 dalpha-0.5.2rc1/dalpha/logging/utils.py
--rw-r--r--   0        0        0     6625 2024-05-13 09:40:01.895738 dalpha-0.5.2rc1/dalpha/message_consumer.py
--rw-r--r--   0        0        0     1703 2024-05-10 10:54:52.512416 dalpha-0.5.2rc1/dalpha/openai_cls.py
--rw-r--r--   0        0        0     6079 2024-05-02 07:23:00.795089 dalpha-0.5.2rc1/dalpha/redis_cli.py
--rw-r--r--   0        0        0     1886 2024-05-02 07:23:00.795089 dalpha-0.5.2rc1/dalpha/redis_cls.py
--rw-r--r--   0        0        0      776 2024-05-10 10:54:52.512416 dalpha-0.5.2rc1/dalpha/request.py
--rw-r--r--   0        0        0     2689 2024-05-10 10:54:52.512416 dalpha-0.5.2rc1/dalpha/s3.py
--rw-r--r--   0        0        0      497 2024-02-28 08:10:55.063883 dalpha-0.5.2rc1/dalpha/signal_handler.py
--rw-r--r--   0        0        0      767 2024-05-10 10:54:52.512416 dalpha-0.5.2rc1/dalpha/slack.py
--rw-r--r--   0        0        0     2355 2024-05-10 10:54:52.512416 dalpha-0.5.2rc1/dalpha/update_agent.py
--rw-r--r--   0        0        0      952 2024-05-16 13:20:42.129689 dalpha-0.5.2rc1/pyproject.toml
--rw-r--r--   0        0        0     1362 1970-01-01 00:00:00.000000 dalpha-0.5.2rc1/PKG-INFO
+-rw-r--r--   0        0        0      578 2023-12-18 04:10:26.318635 dalpha-0.5.2rc2/README.md
+-rw-r--r--   0        0        0     2077 2024-05-16 07:16:07.976796 dalpha-0.5.2rc2/dalpha/__init__.py
+-rw-r--r--   0        0        0     8284 2024-05-16 13:46:33.629942 dalpha-0.5.2rc2/dalpha/agent.py
+-rw-r--r--   0        0        0     7019 2024-05-10 10:54:52.512416 dalpha-0.5.2rc2/dalpha/backend_cli.py
+-rw-r--r--   0        0        0      555 2024-05-08 06:25:10.211719 dalpha-0.5.2rc2/dalpha/cobra_cls.py
+-rw-r--r--   0        0        0      573 2024-02-28 08:10:55.063883 dalpha-0.5.2rc2/dalpha/context.py
+-rw-r--r--   0        0        0     3036 2024-05-02 07:23:00.795089 dalpha-0.5.2rc2/dalpha/data_update_cls.py
+-rw-r--r--   0        0        0      940 2024-05-02 07:23:00.795089 dalpha-0.5.2rc2/dalpha/dto.py
+-rw-r--r--   0        0        0      616 2024-05-16 07:16:07.980796 dalpha-0.5.2rc2/dalpha/exception.py
+-rw-r--r--   0        0        0     5954 2024-05-16 07:16:07.980796 dalpha-0.5.2rc2/dalpha/inference_cls.py
+-rw-r--r--   0        0        0      233 2024-03-25 02:37:47.094337 dalpha-0.5.2rc2/dalpha/kafka_cli.py
+-rw-r--r--   0        0        0     1861 2024-03-11 02:52:37.986799 dalpha-0.5.2rc2/dalpha/logging/__init__.py
+-rw-r--r--   0        0        0      229 2024-02-28 08:10:55.063883 dalpha-0.5.2rc2/dalpha/logging/events.py
+-rw-r--r--   0        0        0     1116 2024-02-28 08:10:55.063883 dalpha-0.5.2rc2/dalpha/logging/log_formatter.py
+-rw-r--r--   0        0        0     1817 2024-02-28 08:10:55.063883 dalpha-0.5.2rc2/dalpha/logging/utils.py
+-rw-r--r--   0        0        0     6625 2024-05-13 09:40:01.895738 dalpha-0.5.2rc2/dalpha/message_consumer.py
+-rw-r--r--   0        0        0     1703 2024-05-10 10:54:52.512416 dalpha-0.5.2rc2/dalpha/openai_cls.py
+-rw-r--r--   0        0        0     6079 2024-05-02 07:23:00.795089 dalpha-0.5.2rc2/dalpha/redis_cli.py
+-rw-r--r--   0        0        0     1886 2024-05-02 07:23:00.795089 dalpha-0.5.2rc2/dalpha/redis_cls.py
+-rw-r--r--   0        0        0      776 2024-05-10 10:54:52.512416 dalpha-0.5.2rc2/dalpha/request.py
+-rw-r--r--   0        0        0     2689 2024-05-10 10:54:52.512416 dalpha-0.5.2rc2/dalpha/s3.py
+-rw-r--r--   0        0        0      497 2024-02-28 08:10:55.063883 dalpha-0.5.2rc2/dalpha/signal_handler.py
+-rw-r--r--   0        0        0      767 2024-05-10 10:54:52.512416 dalpha-0.5.2rc2/dalpha/slack.py
+-rw-r--r--   0        0        0     2355 2024-05-10 10:54:52.512416 dalpha-0.5.2rc2/dalpha/update_agent.py
+-rw-r--r--   0        0        0      952 2024-05-16 13:46:33.629942 dalpha-0.5.2rc2/pyproject.toml
+-rw-r--r--   0        0        0     1362 1970-01-01 00:00:00.000000 dalpha-0.5.2rc2/PKG-INFO
```

### Comparing `dalpha-0.5.2rc1/README.md` & `dalpha-0.5.2rc2/README.md`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc1/dalpha/__init__.py` & `dalpha-0.5.2rc2/dalpha/__init__.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc1/dalpha/agent.py` & `dalpha-0.5.2rc2/dalpha/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,16 +127,16 @@
             )
             self.message_consumer.close()
             sys.exit(0)
         if not isinstance(max_number_of_messages,int): TypeError("max_number_of_messages is not a int")
         if not isinstance(mock, bool): TypeError("mock is not a bool")
         if mock:
             logger.info(
-                "return mock",
-                data = to_evaluate_item(self.mock)
+                f"return mock: {to_evaluate_item(self.mock).dict()}",
+                data = to_evaluate_item(self.mock).dict()
             )
             return to_evaluate_item(self.mock)
 
         ret: List[EvaluateItem] = self.message_consumer.poll()
         if len(ret) == 0:
             # 가져온 메세지가 없으면 None 반환
             return None
```

### Comparing `dalpha-0.5.2rc1/dalpha/backend_cli.py` & `dalpha-0.5.2rc2/dalpha/backend_cli.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc1/dalpha/cobra_cls.py` & `dalpha-0.5.2rc2/dalpha/cobra_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc1/dalpha/context.py` & `dalpha-0.5.2rc2/dalpha/context.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc1/dalpha/data_update_cls.py` & `dalpha-0.5.2rc2/dalpha/data_update_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc1/dalpha/dto.py` & `dalpha-0.5.2rc2/dalpha/dto.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc1/dalpha/exception.py` & `dalpha-0.5.2rc2/dalpha/exception.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc1/dalpha/inference_cls.py` & `dalpha-0.5.2rc2/dalpha/inference_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc1/dalpha/logging/__init__.py` & `dalpha-0.5.2rc2/dalpha/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc1/dalpha/logging/log_formatter.py` & `dalpha-0.5.2rc2/dalpha/logging/log_formatter.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc1/dalpha/logging/utils.py` & `dalpha-0.5.2rc2/dalpha/logging/utils.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc1/dalpha/message_consumer.py` & `dalpha-0.5.2rc2/dalpha/message_consumer.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc1/dalpha/openai_cls.py` & `dalpha-0.5.2rc2/dalpha/openai_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc1/dalpha/redis_cli.py` & `dalpha-0.5.2rc2/dalpha/redis_cli.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc1/dalpha/redis_cls.py` & `dalpha-0.5.2rc2/dalpha/redis_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc1/dalpha/request.py` & `dalpha-0.5.2rc2/dalpha/request.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc1/dalpha/s3.py` & `dalpha-0.5.2rc2/dalpha/s3.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc1/dalpha/slack.py` & `dalpha-0.5.2rc2/dalpha/slack.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc1/dalpha/update_agent.py` & `dalpha-0.5.2rc2/dalpha/update_agent.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.2rc1/pyproject.toml` & `dalpha-0.5.2rc2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dalpha"
-version = "0.5.2rc1"
+version = "0.5.2rc2"
 description = ""
 authors = ["devops <devops@dalpha.so>"]
 readme = "README.md"
 packages = [{include = "dalpha"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -17,15 +17,15 @@
 pydantic = "^2.7.1"
 
 [tool.poetry.group.dev.dependencies]
 twine = "^4.0.2"
 
 [project]
 name = "dalpha"
-version = "0.5.2rc1"
+version = "0.5.2rc2"
 authors = [
   { name="Beomseok", email="beomseok.kim@dalpha.so" },
   { name="Gideok", email="gideok.kim@dalpha.so" },
 ]
 description = "Dalpha internal sdk"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `dalpha-0.5.2rc1/PKG-INFO` & `dalpha-0.5.2rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalpha
-Version: 0.5.2rc1
+Version: 0.5.2rc2
 Summary: 
 Author: devops
 Author-email: devops@dalpha.so
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

