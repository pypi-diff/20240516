# Comparing `tmp/patchwork-client-kafka-0.2.7.tar.gz` & `tmp/patchwork-client-kafka-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/patchwork-client-kafka-0.2.7.tar", last modified: Wed Feb 14 22:39:26 2024, max compression
+gzip compressed data, was "dist/patchwork-client-kafka-0.2.8.tar", last modified: Wed May 15 19:57:34 2024, max compression
```

## Comparing `patchwork-client-kafka-0.2.7.tar` & `patchwork-client-kafka-0.2.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 22:39:26.000000 patchwork-client-kafka-0.2.7/
--rw-rw-rw-   0 root         (0) root         (0)     1056 2024-02-14 22:39:15.000000 patchwork-client-kafka-0.2.7/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       58 2024-02-14 22:39:15.000000 patchwork-client-kafka-0.2.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1032 2024-02-14 22:39:26.000000 patchwork-client-kafka-0.2.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      316 2024-02-14 22:39:15.000000 patchwork-client-kafka-0.2.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 22:39:26.000000 patchwork-client-kafka-0.2.7/int/
--rw-rw-rw-   0 root         (0) root         (0)     2410 2024-02-14 22:39:15.000000 patchwork-client-kafka-0.2.7/int/test_integration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 22:39:26.000000 patchwork-client-kafka-0.2.7/patchwork/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 22:39:26.000000 patchwork-client-kafka-0.2.7/patchwork/client/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 22:39:26.000000 patchwork-client-kafka-0.2.7/patchwork/client/kafka/
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-02-14 22:39:15.000000 patchwork-client-kafka-0.2.7/patchwork/client/kafka/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3623 2024-02-14 22:39:15.000000 patchwork-client-kafka-0.2.7/patchwork/client/kafka/common.py
--rw-rw-rw-   0 root         (0) root         (0)    10484 2024-02-14 22:39:15.000000 patchwork-client-kafka-0.2.7/patchwork/client/kafka/publisher.py
--rw-rw-rw-   0 root         (0) root         (0)    19723 2024-02-14 22:39:15.000000 patchwork-client-kafka-0.2.7/patchwork/client/kafka/subscriber.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 22:39:26.000000 patchwork-client-kafka-0.2.7/patchwork_client_kafka.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1032 2024-02-14 22:39:26.000000 patchwork-client-kafka-0.2.7/patchwork_client_kafka.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      556 2024-02-14 22:39:26.000000 patchwork-client-kafka-0.2.7/patchwork_client_kafka.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-14 22:39:26.000000 patchwork-client-kafka-0.2.7/patchwork_client_kafka.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-14 22:39:26.000000 patchwork-client-kafka-0.2.7/patchwork_client_kafka.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       57 2024-02-14 22:39:26.000000 patchwork-client-kafka-0.2.7/patchwork_client_kafka.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2024-02-14 22:39:26.000000 patchwork-client-kafka-0.2.7/patchwork_client_kafka.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       56 2024-02-14 22:39:15.000000 patchwork-client-kafka-0.2.7/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-14 22:39:26.000000 patchwork-client-kafka-0.2.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1676 2024-02-14 22:39:15.000000 patchwork-client-kafka-0.2.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 22:39:26.000000 patchwork-client-kafka-0.2.7/tests/
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-02-14 22:39:15.000000 patchwork-client-kafka-0.2.7/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      314 2024-02-14 22:39:15.000000 patchwork-client-kafka-0.2.7/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)      421 2024-02-14 22:39:15.000000 patchwork-client-kafka-0.2.7/tests/test_clientkafka.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 19:57:34.000000 patchwork-client-kafka-0.2.8/
+-rw-rw-rw-   0 root         (0) root         (0)     1056 2024-05-15 19:57:21.000000 patchwork-client-kafka-0.2.8/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       58 2024-05-15 19:57:21.000000 patchwork-client-kafka-0.2.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1032 2024-05-15 19:57:34.000000 patchwork-client-kafka-0.2.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      316 2024-05-15 19:57:21.000000 patchwork-client-kafka-0.2.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 19:57:34.000000 patchwork-client-kafka-0.2.8/int/
+-rw-rw-rw-   0 root         (0) root         (0)     2410 2024-05-15 19:57:21.000000 patchwork-client-kafka-0.2.8/int/test_integration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 19:57:34.000000 patchwork-client-kafka-0.2.8/patchwork/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 19:57:34.000000 patchwork-client-kafka-0.2.8/patchwork/client/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 19:57:34.000000 patchwork-client-kafka-0.2.8/patchwork/client/kafka/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-05-15 19:57:21.000000 patchwork-client-kafka-0.2.8/patchwork/client/kafka/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3623 2024-05-15 19:57:21.000000 patchwork-client-kafka-0.2.8/patchwork/client/kafka/common.py
+-rw-rw-rw-   0 root         (0) root         (0)    10551 2024-05-15 19:57:21.000000 patchwork-client-kafka-0.2.8/patchwork/client/kafka/publisher.py
+-rw-rw-rw-   0 root         (0) root         (0)    19797 2024-05-15 19:57:21.000000 patchwork-client-kafka-0.2.8/patchwork/client/kafka/subscriber.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 19:57:34.000000 patchwork-client-kafka-0.2.8/patchwork_client_kafka.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1032 2024-05-15 19:57:34.000000 patchwork-client-kafka-0.2.8/patchwork_client_kafka.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      556 2024-05-15 19:57:34.000000 patchwork-client-kafka-0.2.8/patchwork_client_kafka.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 19:57:34.000000 patchwork-client-kafka-0.2.8/patchwork_client_kafka.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 19:57:34.000000 patchwork-client-kafka-0.2.8/patchwork_client_kafka.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       57 2024-05-15 19:57:34.000000 patchwork-client-kafka-0.2.8/patchwork_client_kafka.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2024-05-15 19:57:34.000000 patchwork-client-kafka-0.2.8/patchwork_client_kafka.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       56 2024-05-15 19:57:21.000000 patchwork-client-kafka-0.2.8/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 19:57:34.000000 patchwork-client-kafka-0.2.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1676 2024-05-15 19:57:21.000000 patchwork-client-kafka-0.2.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 19:57:34.000000 patchwork-client-kafka-0.2.8/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-05-15 19:57:21.000000 patchwork-client-kafka-0.2.8/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      314 2024-05-15 19:57:21.000000 patchwork-client-kafka-0.2.8/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)      421 2024-05-15 19:57:21.000000 patchwork-client-kafka-0.2.8/tests/test_clientkafka.py
```

### Comparing `patchwork-client-kafka-0.2.7/LICENSE` & `patchwork-client-kafka-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `patchwork-client-kafka-0.2.7/PKG-INFO` & `patchwork-client-kafka-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patchwork-client-kafka
-Version: 0.2.7
+Version: 0.2.8
 Summary: Kafka client for Patchwork - The distributed asynchronous microframework
 Home-page: 
 Author: Pawel Pecio
 Author-email: 
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `patchwork-client-kafka-0.2.7/int/test_integration.py` & `patchwork-client-kafka-0.2.8/int/test_integration.py`

 * *Files identical despite different names*

### Comparing `patchwork-client-kafka-0.2.7/patchwork/client/kafka/common.py` & `patchwork-client-kafka-0.2.8/patchwork/client/kafka/common.py`

 * *Files identical despite different names*

### Comparing `patchwork-client-kafka-0.2.7/patchwork/client/kafka/publisher.py` & `patchwork-client-kafka-0.2.8/patchwork/client/kafka/publisher.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,25 +33,27 @@
             Setup producer ACK (acknowledges) policy
         :cvar default_topic:
             Set default topic for all tasks which don't have `queue_name` specified in their metadata
         :cvar postpone_queue_name:
             Kafka does not support postponed messages, so to avoid re-taking them all time until not_before time,
             producer may put postponed messages to the special queue which handles messages rolling and re-sending
             to destination queue when their time comes up (see Patchwork Kafka Scheduler package)
+        :cvar reconnect_time_s:
+            reconnect time in seconds
         """
         kafka_hosts: List[str]
         missing_topic: MissingTopicBehaviour = MissingTopicBehaviour.ERROR
         default_partitions_count: Optional[int] = None
         default_replication_factor: Optional[int] = None
         compression_type: CompressionType = CompressionType.NONE
         request_timeout_ms: int = 30*SECOND
         ack_policy: AckPolicy = AckPolicy.ACK_ALL
         default_topic: Optional[str] = None
         postpone_queue_name: Optional[str] = None
-        reconnect_time: int = 30*SECOND
+        reconnect_time_s: int = 30
 
         @field_validator('default_partitions_count')
         @classmethod
         def validate_dpc(cls, v):
             if v is not None and v <= 0:
                 raise ValueError("default_partitions_count must be a positive number")
             return v
@@ -241,15 +243,15 @@
 
         self.logger.debug("producer created")
 
         while True:
             try:
                 await self._producer.start()
             except KafkaConnectionError:
-                await asyncio.sleep(self.settings.reconnect_time)
+                await asyncio.sleep(self.settings.reconnect_time_s)
             except Exception as exc:
                 self.logger.exception(f"unable to start Kafka producer: {exc.__class__.__name__}({exc})", exc_info=True)
                 await self._kill_producer()
                 raise
 
             break
```

### Comparing `patchwork-client-kafka-0.2.7/patchwork/client/kafka/subscriber.py` & `patchwork-client-kafka-0.2.8/patchwork/client/kafka/subscriber.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,24 +68,26 @@
             Low value cause frequent metadata updates which may affect performance, however long period cause that
             new topics will be discovered later.
         :cvar health_check_ms:
             Determines how often Kafka broker should make a health-check calls to make sure that consumer is alive
             (in miliseconds)
         :cvar poll_interval_ms:
             Determine how ofter consumer should make a poll requests to Kafka broker (in miliseconds)
+        :cvar reconnect_time_s:
+            reconnect time in seconds
         """
         kafka_hosts: List[str]
         topics: List[str]
         consumer_group: str
         request_timeout_ms: int = 30*SECOND
         metadata_validity_ms: int = 5*MINUTE
         health_check_ms: int = 3*SECOND
         poll_interval_ms: int = 10*SECOND
         freeze_time: Optional[float] = None
-        reconnect_time: int = 30 * SECOND
+        reconnect_time_s: int = 30
 
         @model_validator(mode='after')
         @classmethod
         def validate_freeze(cls, values):
             if values.freeze_time is None:
                 values.freeze_time = randint(
                     int(min(values.poll_interval_ms * MAX_TIME_MULTIPLIER / 0.5, 10 * SECOND)),
@@ -394,23 +396,23 @@
             max_poll_interval_ms=self.max_poll_interval_ms,
             # set session timeout 10 times greater than health-check
             session_timeout_ms=self.session_timeout,
             heartbeat_interval_ms=self.settings.health_check_ms,
             consumer_timeout_ms=self.settings.request_timeout_ms,
             # request timeout must be greater than session timeout
             request_timeout_ms=self.session_timeout*2,
-            retry_backoff_ms=self.settings.reconnect_time
+            retry_backoff_ms=self.settings.reconnect_time_s*SECOND
         )
         self.logger.debug("consumer created")
 
         while True:
             try:
                 await self.consumer.start()
             except KafkaConnectionError:
-                await asyncio.sleep(self.settings.reconnect_time)
+                await asyncio.sleep(self.settings.reconnect_time_s)
             except Exception as exc:
                 self.logger.exception(f"unable to start Kafka consumer: {exc.__class__.__name__}({exc})", exc_info=True)
                 await self._kill_consumer()
                 raise
 
             break
```

### Comparing `patchwork-client-kafka-0.2.7/patchwork_client_kafka.egg-info/PKG-INFO` & `patchwork-client-kafka-0.2.8/patchwork_client_kafka.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patchwork-client-kafka
-Version: 0.2.7
+Version: 0.2.8
 Summary: Kafka client for Patchwork - The distributed asynchronous microframework
 Home-page: 
 Author: Pawel Pecio
 Author-email: 
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `patchwork-client-kafka-0.2.7/patchwork_client_kafka.egg-info/SOURCES.txt` & `patchwork-client-kafka-0.2.8/patchwork_client_kafka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `patchwork-client-kafka-0.2.7/setup.py` & `patchwork-client-kafka-0.2.8/setup.py`

 * *Files identical despite different names*

