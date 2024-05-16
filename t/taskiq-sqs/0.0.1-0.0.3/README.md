# Comparing `tmp/taskiq_sqs-0.0.1.tar.gz` & `tmp/taskiq_sqs-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq_sqs-0.0.1.tar", last modified: Thu May 16 00:50:56 2024, max compression
+gzip compressed data, was "taskiq_sqs-0.0.3.tar", last modified: Thu May 16 02:45:06 2024, max compression
```

## Comparing `taskiq_sqs-0.0.1.tar` & `taskiq_sqs-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2024-05-16 00:50:56.304428 taskiq_sqs-0.0.1/
-drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2024-05-16 00:50:56.297761 taskiq_sqs-0.0.1/.github/
-drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2024-05-16 00:50:56.301095 taskiq_sqs-0.0.1/.github/workflows/
--rw-r--r--   0 mike      (1000) mike      (1000)     1338 2024-05-15 22:46:26.000000 taskiq_sqs-0.0.1/.github/workflows/release.yaml
--rw-r--r--   0 mike      (1000) mike      (1000)     1941 2024-05-15 22:46:26.000000 taskiq_sqs-0.0.1/.github/workflows/test.yaml
--rw-r--r--   0 mike      (1000) mike      (1000)     1729 2024-05-15 22:45:27.000000 taskiq_sqs-0.0.1/.gitignore
--rw-r--r--   0 mike      (1000) mike      (1000)    11342 2024-05-15 22:45:35.000000 taskiq_sqs-0.0.1/LICENSE
--rw-r--r--   0 mike      (1000) mike      (1000)    14563 2024-05-16 00:50:56.304428 taskiq_sqs-0.0.1/PKG-INFO
--rw-r--r--   0 mike      (1000) mike      (1000)      210 2024-05-15 23:01:42.000000 taskiq_sqs-0.0.1/README.md
--rw-r--r--   0 mike      (1000) mike      (1000)     1897 2024-05-16 00:50:50.000000 taskiq_sqs-0.0.1/pyproject.toml
--rw-r--r--   0 mike      (1000) mike      (1000)      284 2024-05-16 00:50:56.304428 taskiq_sqs-0.0.1/setup.cfg
--rw-r--r--   0 mike      (1000) mike      (1000)       54 2024-05-15 22:45:16.000000 taskiq_sqs-0.0.1/setup.py
-drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2024-05-16 00:50:56.301095 taskiq_sqs-0.0.1/taskiq_redis/
--rw-r--r--   0 mike      (1000) mike      (1000)       67 2024-05-15 22:48:43.000000 taskiq_sqs-0.0.1/taskiq_redis/__init__.py
--rw-r--r--   0 mike      (1000) mike      (1000)     4163 2024-05-15 22:52:20.000000 taskiq_sqs-0.0.1/taskiq_redis/broker.py
-drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2024-05-16 00:50:56.301095 taskiq_sqs-0.0.1/taskiq_sqs.egg-info/
--rw-r--r--   0 mike      (1000) mike      (1000)    14563 2024-05-16 00:50:56.000000 taskiq_sqs-0.0.1/taskiq_sqs.egg-info/PKG-INFO
--rw-r--r--   0 mike      (1000) mike      (1000)      338 2024-05-16 00:50:56.000000 taskiq_sqs-0.0.1/taskiq_sqs.egg-info/SOURCES.txt
--rw-r--r--   0 mike      (1000) mike      (1000)        1 2024-05-16 00:50:56.000000 taskiq_sqs-0.0.1/taskiq_sqs.egg-info/dependency_links.txt
--rw-r--r--   0 mike      (1000) mike      (1000)      222 2024-05-16 00:50:56.000000 taskiq_sqs-0.0.1/taskiq_sqs.egg-info/requires.txt
--rw-r--r--   0 mike      (1000) mike      (1000)       13 2024-05-16 00:50:56.000000 taskiq_sqs-0.0.1/taskiq_sqs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:45:06.844354 taskiq_sqs-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:45:06.840353 taskiq_sqs-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:45:06.840353 taskiq_sqs-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-16 02:44:34.000000 taskiq_sqs-0.0.3/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-16 02:44:34.000000 taskiq_sqs-0.0.3/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-16 02:44:34.000000 taskiq_sqs-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-16 02:44:34.000000 taskiq_sqs-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15423 2024-05-16 02:45:06.844354 taskiq_sqs-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-16 02:44:34.000000 taskiq_sqs-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-16 02:44:34.000000 taskiq_sqs-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-16 02:45:06.844354 taskiq_sqs-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-16 02:44:34.000000 taskiq_sqs-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:45:06.840353 taskiq_sqs-0.0.3/taskiq_sqs/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-16 02:44:34.000000 taskiq_sqs-0.0.3/taskiq_sqs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-05-16 02:44:34.000000 taskiq_sqs-0.0.3/taskiq_sqs/broker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:45:06.844354 taskiq_sqs-0.0.3/taskiq_sqs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15423 2024-05-16 02:45:06.000000 taskiq_sqs-0.0.3/taskiq_sqs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-16 02:45:06.000000 taskiq_sqs-0.0.3/taskiq_sqs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 02:45:06.000000 taskiq_sqs-0.0.3/taskiq_sqs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-16 02:45:06.000000 taskiq_sqs-0.0.3/taskiq_sqs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-16 02:45:06.000000 taskiq_sqs-0.0.3/taskiq_sqs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:45:06.844354 taskiq_sqs-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-16 02:44:34.000000 taskiq_sqs-0.0.3/tests/test_broker.py
```

### Comparing `taskiq_sqs-0.0.1/.github/workflows/release.yaml` & `taskiq_sqs-0.0.3/.github/workflows/release.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 on:
   release:
     types: [published]
 
+env:
+  AWS_DEFAULT_REGION: "us-east-1"
+
 jobs:
   test:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v2
       - uses: actions/setup-python@v2
         with:
```

### Comparing `taskiq_sqs-0.0.1/.github/workflows/test.yaml` & `taskiq_sqs-0.0.3/.github/workflows/test.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 concurrency:
   # Cancel older, in-progress jobs from the same PR, same workflow.
   # use run_id if the job is triggered by a push to ensure
   # push-triggered jobs to not get canceled.
   group: ${{ github.workflow }}-${{ github.head_ref || github.run_id }}
   cancel-in-progress: true
 
+env:
+  AWS_DEFAULT_REGION: "us-east-1"
+
 jobs:
     linting:
         runs-on: ubuntu-latest
 
         steps:
         - uses: actions/checkout@v3
 
@@ -57,15 +60,15 @@
 
     test:
         runs-on: ${{ matrix.os }}
 
         strategy:
             matrix:
                 os: [ubuntu-latest, macos-latest]   # eventually add `windows-latest`
-                python-version: ["3.8", "3.9", "3.10", "3.11"]
+                python-version: ["3.10", "3.11", "3.12"]
 
         steps:
         - uses: actions/checkout@v3
           with:
             fetch-depth: 0
 
         - name: Setup Python
```

### Comparing `taskiq_sqs-0.0.1/.gitignore` & `taskiq_sqs-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `taskiq_sqs-0.0.1/LICENSE` & `taskiq_sqs-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `taskiq_sqs-0.0.1/PKG-INFO` & `taskiq_sqs-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskiq-sqs
-Version: 0.0.1
+Version: 0.0.3
 Summary: SQS Broker for TaskIQ
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -214,31 +214,61 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: asyncer~=0.0.5
 Requires-Dist: boto3~=1.34.34
 Provides-Extra: dev
 Requires-Dist: black~=23.12.1; extra == "dev"
 Requires-Dist: boto3-stubs[essential]~=1.34.84; extra == "dev"
 Requires-Dist: build~=1.0.3; extra == "dev"
 Requires-Dist: flake8~=7.0.0; extra == "dev"
 Requires-Dist: isort~=5.13.2; extra == "dev"
 Requires-Dist: mypy~=1.8.0; extra == "dev"
 Requires-Dist: pytest~=7.4.4; extra == "dev"
 Requires-Dist: requests~=2.31.0; extra == "dev"
 Requires-Dist: setuptools-scm~=8.0.4; extra == "dev"
+Requires-Dist: taskiq<1,>=0.10.3; extra == "dev"
 Requires-Dist: types-requests>=2.31.0.20240106; extra == "dev"
 
 # TaskIQ SQS Broker
 
 Mostly generic SQS async broker for TaskIQ. 
 
 ## Expiration
 
 If you set the `sqs_expiry` label to a unix timestamp, the message will be discarded if the worker receives it after that time.
+
+```python
+import asyncio
+from taskiq_sqs import SQSBroker
+
+broker = SQSBroker("http://sqs.us-east-1.localhost.localstack.cloud:4566/000000000000/my-queue")
+
+@broker.task
+async def add_one(value: int) -> int:
+    return value + 1
+
+
+async def main() -> None:
+    # Never forget to call startup in the beginning.
+    await broker.startup()
+    # Send the task to the broker.
+    task = await add_one.kiq(1)
+    # Wait for the result. (result backend must be configured)
+    result = await task.wait_result(timeout=2)
+    print(f"Task execution took: {result.execution_time} seconds.")
+    if not result.is_err:
+        print(f"Returned value: {result.return_value}")
+    else:
+        print("Error found while executing task.")
+    await broker.shutdown()
+
+if __name__ == "__main__":
+    asyncio.run(main())
+```
```

### Comparing `taskiq_sqs-0.0.1/pyproject.toml` & `taskiq_sqs-0.0.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "taskiq-sqs"
 description = "SQS Broker for TaskIQ"
 urls = {source = "https://github.com/ApeWorx/taskiq-sqs"}
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 keywords = ["taskiq", "broker", "aws", "sqs"]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Intended Audience :: End Users/Desktop",
     "License :: OSI Approved :: MIT License",
@@ -24,36 +24,35 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
     "asyncer~=0.0.5",
     "boto3~=1.34.34",
 ]
-version = "0.0.1"
-#dynamic = ["version"]
+dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
     "black~=23.12.1",
     "boto3-stubs[essential]~=1.34.84",
     "build~=1.0.3",
     "flake8~=7.0.0",
     "isort~=5.13.2",
     "mypy~=1.8.0",
     "pytest~=7.4.4",
     "requests~=2.31.0",
     "setuptools-scm~=8.0.4",
+    "taskiq>=0.10.3,<1",
     "types-requests>=2.31.0.20240106",
 ]
 
 [tool.mypy]
 exclude = "build/"
 
 [tool.setuptools_scm]
-#write_to = "taskiq_sqs/_meta.py"
 
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
 [tool.black]
```

### Comparing `taskiq_sqs-0.0.1/taskiq_redis/broker.py` & `taskiq_sqs-0.0.3/taskiq_sqs/broker.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 import asyncio
 import logging
 from datetime import datetime, timezone
-from typing import (
-    AsyncGenerator,
-    Callable,
-    Optional,
-    Union,
-)
+from typing import AsyncGenerator, Callable, Optional, Union
 
 import boto3
-from ape.logging import logger
 from asyncer import asyncify
 from mypy_boto3_sqs.service_resource import Queue
 from taskiq import AsyncBroker
 from taskiq.abc.result_backend import AsyncResultBackend
 from taskiq.acks import AckableMessage
 from taskiq.message import BrokerMessage
 
 logger = logging.getLogger(__name__)
-stamp = lambda: int(datetime.now(tz=timezone.utc).timestamp())
+
+
+def stamp() -> int:
+    return int(datetime.now(tz=timezone.utc).timestamp())
 
 
 class SQSBroker(AsyncBroker):
     """AWS SQS TaskIQ broker."""
 
     def __init__(
         self,
@@ -35,15 +32,17 @@
         self._sqs = boto3.resource("sqs")
         self._sqs_queue: Optional[Queue] = None
 
     async def _get_queue(self) -> Queue:
         queue_name = self.sqs_queue_url.split("/")[-1]
 
         if not self._sqs_queue:
-            self._sqs_queue = await asyncify(self._sqs.get_queue_by_name)(QueueName=queue_name)
+            self._sqs_queue = await asyncify(self._sqs.get_queue_by_name)(
+                QueueName=queue_name
+            )
 
             if not self._sqs_queue:
                 raise Exception("SQS Queue not found")
 
         return self._sqs_queue
 
     async def kick(
@@ -59,26 +58,24 @@
         You don't need to send broker message. It's helper for brokers,
         please send only bytes from message.message.
 
         :param message: name of a task.
         """
         queue = await self._get_queue()
         # Must be explicitly set as a label to a unix timestamp
-        expiry = message.labels.pop("sqs_expiry", None)
-
-        # SQS structured message attributes
-        message_attributes = dict()
-        if expiry:
-            message_attributes["expiry"] = {
-                "StringValue": str(expiry),
-                "DataType": "Number",
-            }
+        expiry = message.labels.pop("sqs_expiry", 0)
 
         await asyncify(queue.send_message)(
-            MessageAttributes=message_attributes,
+            # SQS structured message attributes
+            MessageAttributes={
+                "expiry": {
+                    "StringValue": str(expiry),
+                    "DataType": "Number",
+                }
+            },
             MessageBody=message.message.decode("utf-8"),
             MessageGroupId=message.task_name,
         )
 
     async def listen(self) -> AsyncGenerator[Union[bytes, AckableMessage], None]:
         """
         This function listens to new messages and yields them.
@@ -98,22 +95,28 @@
 
         queue = await self._get_queue()
 
         # TODO: Consider using AckableMessage and confirm with the queue to reduce lost messages
         while True:
             last_had_message = False
 
-            for message in await asyncify(queue.receive_messages)():
+            for message in await asyncify(queue.receive_messages)(
+                MessageAttributeNames=[".*"]
+            ):
                 try:
                     if message.message_attributes:
                         # if expiry was set as a message attribute, respect it
-                        if expiry := message.message_attributes.get("expiry"):
-                            diff = stamp() - expiry
-                            if diff > 0:
-                                logger.debug(f"Message expired {diff} seconds ago. Skipping.")
+                        if expiry_typed := message.message_attributes.get("expiry"):
+                            expiry = int(expiry_typed.get("StringValue", 0))
+                            now = stamp()
+                            if 0 < expiry < now:
+                                logger.warn(
+                                    f"Message expired {now - expiry} seconds ago. Skipping."
+                                )
+                                await asyncify(message.delete)()
                                 continue
                 except TypeError:
                     # Ignore weird expiries.  Not critical.
                     pass
 
                 yield message.body.encode("utf-8")
                 await asyncify(message.delete)()
```

### Comparing `taskiq_sqs-0.0.1/taskiq_sqs.egg-info/PKG-INFO` & `taskiq_sqs-0.0.3/taskiq_sqs.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskiq-sqs
-Version: 0.0.1
+Version: 0.0.3
 Summary: SQS Broker for TaskIQ
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -214,31 +214,61 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: asyncer~=0.0.5
 Requires-Dist: boto3~=1.34.34
 Provides-Extra: dev
 Requires-Dist: black~=23.12.1; extra == "dev"
 Requires-Dist: boto3-stubs[essential]~=1.34.84; extra == "dev"
 Requires-Dist: build~=1.0.3; extra == "dev"
 Requires-Dist: flake8~=7.0.0; extra == "dev"
 Requires-Dist: isort~=5.13.2; extra == "dev"
 Requires-Dist: mypy~=1.8.0; extra == "dev"
 Requires-Dist: pytest~=7.4.4; extra == "dev"
 Requires-Dist: requests~=2.31.0; extra == "dev"
 Requires-Dist: setuptools-scm~=8.0.4; extra == "dev"
+Requires-Dist: taskiq<1,>=0.10.3; extra == "dev"
 Requires-Dist: types-requests>=2.31.0.20240106; extra == "dev"
 
 # TaskIQ SQS Broker
 
 Mostly generic SQS async broker for TaskIQ. 
 
 ## Expiration
 
 If you set the `sqs_expiry` label to a unix timestamp, the message will be discarded if the worker receives it after that time.
+
+```python
+import asyncio
+from taskiq_sqs import SQSBroker
+
+broker = SQSBroker("http://sqs.us-east-1.localhost.localstack.cloud:4566/000000000000/my-queue")
+
+@broker.task
+async def add_one(value: int) -> int:
+    return value + 1
+
+
+async def main() -> None:
+    # Never forget to call startup in the beginning.
+    await broker.startup()
+    # Send the task to the broker.
+    task = await add_one.kiq(1)
+    # Wait for the result. (result backend must be configured)
+    result = await task.wait_result(timeout=2)
+    print(f"Task execution took: {result.execution_time} seconds.")
+    if not result.is_err:
+        print(f"Returned value: {result.return_value}")
+    else:
+        print("Error found while executing task.")
+    await broker.shutdown()
+
+if __name__ == "__main__":
+    asyncio.run(main())
+```
```

