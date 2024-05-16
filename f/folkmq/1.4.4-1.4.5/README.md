# Comparing `tmp/folkmq-1.4.4.tar.gz` & `tmp/folkmq-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "folkmq-1.4.4.tar", last modified: Mon May 13 00:12:56 2024, max compression
+gzip compressed data, was "folkmq-1.4.5.tar", last modified: Thu May 16 09:11:27 2024, max compression
```

## Comparing `folkmq-1.4.4.tar` & `folkmq-1.4.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-05-13 00:12:56.811900 folkmq-1.4.4/
--rw-r--r--   0 noear      (501) staff       (20)      590 2024-05-13 00:12:56.811408 folkmq-1.4.4/PKG-INFO
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-05-13 00:12:56.801099 folkmq-1.4.4/folkmq/
--rw-r--r--   0 noear      (501) staff       (20)      504 2024-05-12 15:23:34.000000 folkmq-1.4.4/folkmq/FolkMQ.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-05-13 00:12:56.805958 folkmq-1.4.4/folkmq/client/
--rw-r--r--   0 noear      (501) staff       (20)      163 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/client/MqAlarm.py
--rw-r--r--   0 noear      (501) staff       (20)     4015 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/client/MqClient.py
--rw-r--r--   0 noear      (501) staff       (20)    15358 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/client/MqClientDefault.py
--rw-r--r--   0 noear      (501) staff       (20)     5518 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/client/MqClientListener.py
--rw-r--r--   0 noear      (501) staff       (20)     3807 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/client/MqMessage.py
--rw-r--r--   0 noear      (501) staff       (20)     3386 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/client/MqMessageReceived.py
--rw-r--r--   0 noear      (501) staff       (20)     1091 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/client/MqRouter.py
--rw-r--r--   0 noear      (501) staff       (20)      883 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/client/MqSubscription.py
--rw-r--r--   0 noear      (501) staff       (20)     1071 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/client/MqTransaction.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/client/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-05-13 00:12:56.809294 folkmq-1.4.4/folkmq/common/
--rw-r--r--   0 noear      (501) staff       (20)      315 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/common/MqApis.py
--rw-r--r--   0 noear      (501) staff       (20)     1054 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/common/MqAssert.py
--rw-r--r--   0 noear      (501) staff       (20)     2372 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/common/MqConstants.py
--rw-r--r--   0 noear      (501) staff       (20)     2510 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/common/MqMetasResolver.py
--rw-r--r--   0 noear      (501) staff       (20)     4772 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/common/MqMetasResolverV1.py
--rw-r--r--   0 noear      (501) staff       (20)     4985 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/common/MqMetasResolverV2.py
--rw-r--r--   0 noear      (501) staff       (20)      773 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/common/MqMetasV1.py
--rw-r--r--   0 noear      (501) staff       (20)      999 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/common/MqMetasV2.py
--rw-r--r--   0 noear      (501) staff       (20)      419 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/common/MqTopicHelper.py
--rw-r--r--   0 noear      (501) staff       (20)     1178 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/common/MqUtils.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/common/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-05-13 00:12:56.810492 folkmq-1.4.4/folkmq/exception/
--rw-r--r--   0 noear      (501) staff       (20)      185 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/exception/FolkmqException.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-30 10:37:05.000000 folkmq-1.4.4/folkmq/exception/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-05-13 00:12:56.810854 folkmq-1.4.4/folkmq.egg-info/
--rw-r--r--   0 noear      (501) staff       (20)      590 2024-05-13 00:12:56.000000 folkmq-1.4.4/folkmq.egg-info/PKG-INFO
--rw-r--r--   0 noear      (501) staff       (20)      896 2024-05-13 00:12:56.000000 folkmq-1.4.4/folkmq.egg-info/SOURCES.txt
--rw-r--r--   0 noear      (501) staff       (20)        1 2024-05-13 00:12:56.000000 folkmq-1.4.4/folkmq.egg-info/dependency_links.txt
--rw-r--r--   0 noear      (501) staff       (20)       50 2024-05-13 00:12:56.000000 folkmq-1.4.4/folkmq.egg-info/requires.txt
--rw-r--r--   0 noear      (501) staff       (20)        7 2024-05-13 00:12:56.000000 folkmq-1.4.4/folkmq.egg-info/top_level.txt
--rw-r--r--   0 noear      (501) staff       (20)        1 2024-05-13 00:12:56.000000 folkmq-1.4.4/folkmq.egg-info/zip-safe
--rw-r--r--   0 noear      (501) staff       (20)       38 2024-05-13 00:12:56.812004 folkmq-1.4.4/setup.cfg
--rw-r--r--   0 noear      (501) staff       (20)      913 2024-05-13 00:12:34.000000 folkmq-1.4.4/setup.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-05-16 09:11:27.569109 folkmq-1.4.5/
+-rw-r--r--   0 noear      (501) staff       (20)      588 2024-05-16 09:11:27.567897 folkmq-1.4.5/PKG-INFO
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-05-16 09:11:27.553023 folkmq-1.4.5/folkmq/
+-rw-r--r--   0 noear      (501) staff       (20)      511 2024-05-16 09:10:32.000000 folkmq-1.4.5/folkmq/FolkMQ.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-30 10:37:05.000000 folkmq-1.4.5/folkmq/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-05-16 09:11:27.559505 folkmq-1.4.5/folkmq/client/
+-rw-r--r--   0 noear      (501) staff       (20)      163 2024-04-30 10:37:05.000000 folkmq-1.4.5/folkmq/client/MqAlarm.py
+-rw-r--r--   0 noear      (501) staff       (20)     4021 2024-05-16 09:02:11.000000 folkmq-1.4.5/folkmq/client/MqClient.py
+-rw-r--r--   0 noear      (501) staff       (20)    15624 2024-05-16 09:10:32.000000 folkmq-1.4.5/folkmq/client/MqClientDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)     5655 2024-05-16 09:02:11.000000 folkmq-1.4.5/folkmq/client/MqClientListener.py
+-rw-r--r--   0 noear      (501) staff       (20)     3879 2024-05-16 09:02:11.000000 folkmq-1.4.5/folkmq/client/MqMessage.py
+-rw-r--r--   0 noear      (501) staff       (20)     3425 2024-05-16 09:07:21.000000 folkmq-1.4.5/folkmq/client/MqMessageReceived.py
+-rw-r--r--   0 noear      (501) staff       (20)     1094 2024-05-16 09:07:21.000000 folkmq-1.4.5/folkmq/client/MqRouter.py
+-rw-r--r--   0 noear      (501) staff       (20)      890 2024-05-16 09:02:11.000000 folkmq-1.4.5/folkmq/client/MqSubscription.py
+-rw-r--r--   0 noear      (501) staff       (20)     1073 2024-05-16 09:02:11.000000 folkmq-1.4.5/folkmq/client/MqTransaction.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-30 10:37:05.000000 folkmq-1.4.5/folkmq/client/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-05-16 09:11:27.564914 folkmq-1.4.5/folkmq/common/
+-rw-r--r--   0 noear      (501) staff       (20)      315 2024-04-30 10:37:05.000000 folkmq-1.4.5/folkmq/common/MqApis.py
+-rw-r--r--   0 noear      (501) staff       (20)     1079 2024-05-16 09:07:21.000000 folkmq-1.4.5/folkmq/common/MqAssert.py
+-rw-r--r--   0 noear      (501) staff       (20)     2372 2024-04-30 10:37:05.000000 folkmq-1.4.5/folkmq/common/MqConstants.py
+-rw-r--r--   0 noear      (501) staff       (20)     2532 2024-05-16 09:07:21.000000 folkmq-1.4.5/folkmq/common/MqMetasResolver.py
+-rw-r--r--   0 noear      (501) staff       (20)     4811 2024-05-16 09:07:21.000000 folkmq-1.4.5/folkmq/common/MqMetasResolverV1.py
+-rw-r--r--   0 noear      (501) staff       (20)     5026 2024-05-16 09:10:32.000000 folkmq-1.4.5/folkmq/common/MqMetasResolverV2.py
+-rw-r--r--   0 noear      (501) staff       (20)      773 2024-04-30 10:37:05.000000 folkmq-1.4.5/folkmq/common/MqMetasV1.py
+-rw-r--r--   0 noear      (501) staff       (20)      999 2024-04-30 10:37:05.000000 folkmq-1.4.5/folkmq/common/MqMetasV2.py
+-rw-r--r--   0 noear      (501) staff       (20)      422 2024-05-16 09:07:21.000000 folkmq-1.4.5/folkmq/common/MqTopicHelper.py
+-rw-r--r--   0 noear      (501) staff       (20)     1184 2024-05-16 09:07:21.000000 folkmq-1.4.5/folkmq/common/MqUtils.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-30 10:37:05.000000 folkmq-1.4.5/folkmq/common/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-05-16 09:11:27.565969 folkmq-1.4.5/folkmq/exception/
+-rw-r--r--   0 noear      (501) staff       (20)      185 2024-04-30 10:37:05.000000 folkmq-1.4.5/folkmq/exception/FolkmqException.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-30 10:37:05.000000 folkmq-1.4.5/folkmq/exception/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-05-16 09:11:27.566547 folkmq-1.4.5/folkmq.egg-info/
+-rw-r--r--   0 noear      (501) staff       (20)      588 2024-05-16 09:11:27.000000 folkmq-1.4.5/folkmq.egg-info/PKG-INFO
+-rw-r--r--   0 noear      (501) staff       (20)      896 2024-05-16 09:11:27.000000 folkmq-1.4.5/folkmq.egg-info/SOURCES.txt
+-rw-r--r--   0 noear      (501) staff       (20)        1 2024-05-16 09:11:27.000000 folkmq-1.4.5/folkmq.egg-info/dependency_links.txt
+-rw-r--r--   0 noear      (501) staff       (20)       48 2024-05-16 09:11:27.000000 folkmq-1.4.5/folkmq.egg-info/requires.txt
+-rw-r--r--   0 noear      (501) staff       (20)        7 2024-05-16 09:11:27.000000 folkmq-1.4.5/folkmq.egg-info/top_level.txt
+-rw-r--r--   0 noear      (501) staff       (20)        1 2024-05-16 09:11:27.000000 folkmq-1.4.5/folkmq.egg-info/zip-safe
+-rw-r--r--   0 noear      (501) staff       (20)       38 2024-05-16 09:11:27.569505 folkmq-1.4.5/setup.cfg
+-rw-r--r--   0 noear      (501) staff       (20)      911 2024-05-16 08:22:47.000000 folkmq-1.4.5/setup.py
```

### Comparing `folkmq-1.4.4/PKG-INFO` & `folkmq-1.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: folkmq
-Version: 1.4.4
+Version: 1.4.5
 Summary: @noear/folkmq python project
 Home-page: https://folkmq.noear.org/
 Author: noear
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.10
 Requires-Dist: loguru>=0.7.2
 Requires-Dist: websockets>=12.0
-Requires-Dist: socket.d>=2.4.16.1
+Requires-Dist: socket.d>=2.4.17
```

### Comparing `folkmq-1.4.4/folkmq/client/MqClient.py` & `folkmq-1.4.5/folkmq/client/MqClient.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,25 +17,25 @@
 class MqClient(ABC):
     @abstractmethod
     def name(self) -> str:
         """名字（即，默认消费者组）"""
         ...
 
     @abstractmethod
-    def nameAs(self, name: str) -> 'MqClient':
+    def name_as(self, name: str) -> 'MqClient':
         """名字取为（即，默认消费者组）"""
         ...
 
     @abstractmethod
     def namespace(self) -> str:
         """命名空间"""
         ...
 
     @abstractmethod
-    def namespaceAs(self, namespace: str) -> 'MqClient':
+    def namespace_as(self, namespace: str) -> 'MqClient':
         """命名空间"""
         ...
 
     @abstractmethod
     async def connect(self) -> 'MqClient':
         """连接"""
         ...
@@ -47,15 +47,15 @@
 
     @abstractmethod
     def config(self, configHandler: Callable[[ClientConfig], None]) -> 'MqClient':
         """客户端配置"""
         ...
 
     @abstractmethod
-    def autoAcknowledge(self, auto: bool) -> 'MqClient':
+    def auto_acknowledge(self, auto: bool) -> 'MqClient':
         """
         自动回执
         :param auto: 自动（默认为 true）
         """
         ...
 
     @abstractmethod
@@ -83,15 +83,15 @@
         """
         同步发布消息
         :param topic:   主题
         :param message: 消息
         """
         ...
 
-    def publishAsync(self, topic: str, message: MqMessage) -> CompletableFuture:
+    def publish_async(self, topic: str, message: MqMessage) -> CompletableFuture:
         """
         异步发布消息
         :param topic:   主题
         :param message: 消息
         """
         ...
 
@@ -121,23 +121,23 @@
         :param message:消息
         :param toName:发送目标名字
         :param timeout:超时（单位毫秒）
         """
         ...
 
     @abstractmethod
-    def transactionCheckback(self, transactionCheckback: Callable[[MqMessageReceived], None]) -> 'MqClient':
+    def transaction_checkback(self, transactionCheckback: Callable[[MqMessageReceived], None]) -> 'MqClient':
         """事务回查
         :param transactionCheckback: 事务回查处理
         """
         ...
 
 
     @abstractmethod
-    def newTransaction(self) -> MqTransaction:
+    def new_transaction(self) -> MqTransaction:
         """新建事务"""
         ...
 
 
 class MqClientInternal(MqClient):
     @abstractmethod
     async def publish2(self, tmid: str, keyAry: [str], isRollback: bool):
```

### Comparing `folkmq-1.4.4/folkmq/client/MqClientDefault.py` & `folkmq-1.4.5/folkmq/client/MqClientDefault.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Callable, Dict
 
 from socketd import SocketD
 from socketd.cluster.ClusterClientSession import ClusterClientSession
 from socketd.exception.SocketDExecption import SocketDConnectionException, SocketDException
 from socketd.transport.client.ClientConfig import ClientConfig
 from socketd.transport.core import Entity
+from socketd.transport.core.EntityMetas import EntityMetas
 from socketd.transport.core.Message import Message
 from socketd.transport.core.Session import Session
 from socketd.transport.core.Entity import Reply
 from socketd.transport.core.entity.EntityDefault import EntityDefault
 from socketd.transport.core.entity.StringEntity import StringEntity
 from socketd.transport.stream.RequestStream import RequestStream
 from socketd.utils.CompletableFuture import CompletableFuture
@@ -54,44 +55,45 @@
         self._listenHandler:Callable[[MqMessageReceived],None] = None
 
 
 
     def name(self) -> str:
         return self._name
 
-    def nameAs(self, name: str) -> 'MqClient':
+    def name_as(self, name: str) -> 'MqClient':
         self._name = name
         return self
 
     def namespace(self) -> str:
         return self._namespace
 
-    def namespaceAs(self, namespace: str) -> 'MqClient':
+    def namespace_as(self, namespace: str) -> 'MqClient':
         self._namespace = namespace
         return self
 
     async def connect(self) -> 'MqClient':
         serverUrls:[str] = []
 
         for url in self._urls:
             url = url.replace("folkmq:ws://", "sd:ws://")
+            url = url.replace("folkmq:wss://", "sd:wss://")
             url = url.replace("folkmq://", "sd:tcp://")
             serverUrls.append(url)
 
         self._clientSession = await (SocketD.create_cluster_client(*serverUrls)
             .config(self.__config_handle)
             .listen(self._clientListener)
             .open())
 
         return self
 
     def __config_handle(self, c:ClientConfig):
         from folkmq.FolkMQ import FolkMQ
 
-        (c.meta_put(MqConstants.FOLKMQ_VERSION, FolkMQ.versionCodeAsString())
+        (c.meta_put(MqConstants.FOLKMQ_VERSION, FolkMQ.version_code_as_string())
           .heartbeat_interval(6_000)
           .io_threads(1)
           .codec_threads(1)
           .exchange_threads(1))
 
         if self._name:
             c.meta_put("@", self._name)
@@ -105,62 +107,63 @@
     async def disconnect(self):
         await self._clientSession.close()
 
     def config(self, configHandler: Callable[[ClientConfig], None]) -> 'MqClient':
         self._clientConfigHandler = configHandler
         return self
 
-    def autoAcknowledge(self, auto: bool) -> 'MqClient':
+    def auto_acknowledge(self, auto: bool) -> 'MqClient':
         self._autoAcknowledge = auto
         return self
 
     async def subscribe(self, topic: str, consumerGroup: str | None, autoAck: bool | None,
                   consumerHandler: Callable[[MqMessageReceived], None]):
         if consumerGroup is None:
             consumerGroup = self.name()
 
         if autoAck is None:
             autoAck = self._autoAcknowledge
 
-        MqAssert.requireNonNull(topic, "Param 'topic' can't be null")
-        MqAssert.requireNonNull(consumerGroup, "Param 'consumerGroup' can't be null")
-        MqAssert.requireNonNull(consumerHandler, "Param 'consumerHandler' can't be null")
+        MqAssert.require_non_null(topic, "Param 'topic' can't be null")
+        MqAssert.require_non_null(consumerGroup, "Param 'consumerGroup' can't be null")
+        MqAssert.require_non_null(consumerHandler, "Param 'consumerHandler' can't be null")
 
-        MqAssert.assertMeta(topic, "topic")
-        MqAssert.assertMeta(consumerGroup, "consumerGroup")
+        MqAssert.assert_meta(topic, "topic")
+        MqAssert.assert_meta(consumerGroup, "consumerGroup")
 
         #支持命名空间
-        topic = MqTopicHelper.getFullTopic(self._namespace, topic)
+        topic = MqTopicHelper.get_full_topic(self._namespace, topic)
 
         subscription = MqSubscription(topic, consumerGroup, autoAck, consumerHandler)
-        self._subscriptionMap[subscription.getQueueName()] = subscription
+        self._subscriptionMap[subscription.get_queue_name()] = subscription
 
         if self._clientSession is not None:
             for session in self._clientSession.get_session_all():
                 #如果有连接会话，则执行订阅
                 entity = (StringEntity("")
-                          .meta_put(MqConstants.MQ_META_TOPIC, subscription.getTopic())
-                          .meta_put(MqConstants.MQ_META_CONSUMER_GROUP, subscription.getConsumerGroup())
+                          .meta_put(MqConstants.MQ_META_TOPIC, subscription.get_topic())
+                          .meta_put(MqConstants.MQ_META_CONSUMER_GROUP, subscription.get_consumer_group())
+                          .meta_put(EntityMetas.META_X_UNLIMITED, "1")
                           .at(MqConstants.BROKER_AT_SERVER_ALL))
                 #使用 Qos1
                 await session.send_and_request(MqConstants.MQ_EVENT_SUBSCRIBE, entity, 30_000).waiter()
                 log.info(f"Client subscribe successfully: {topic}#{consumerGroup}, sessionId={session.session_id()}")
 
     async def unsubscribe(self, topic: str, consumerGroup: str | None):
         if consumerGroup is None:
             consumerGroup = self.name()
 
-        MqAssert.requireNonNull(topic, "Param 'topic' can't be null")
-        MqAssert.requireNonNull(consumerGroup, "Param 'consumerGroup' can't be null")
+        MqAssert.require_non_null(topic, "Param 'topic' can't be null")
+        MqAssert.require_non_null(consumerGroup, "Param 'consumerGroup' can't be null")
 
-        MqAssert.assertMeta(topic, "topic")
-        MqAssert.assertMeta(consumerGroup, "consumerGroup")
+        MqAssert.assert_meta(topic, "topic")
+        MqAssert.assert_meta(consumerGroup, "consumerGroup")
 
         #支持命名空间
-        topic = MqTopicHelper.getFullTopic(self._namespace, topic)
+        topic = MqTopicHelper.get_full_topic(self._namespace, topic)
 
         queueName = topic + MqConstants.SEPARATOR_TOPIC_CONSUMER_GROUP + consumerGroup
         self._subscriptionMap.pop(queueName)
 
         if self._clientSession is not None:
             for session in self._clientSession.get_session_all():
                 #如果有连接会话，则执行订阅
@@ -169,59 +172,59 @@
                           .meta_put(MqConstants.MQ_META_CONSUMER_GROUP, consumerGroup)
                           .at(MqConstants.BROKER_AT_SERVER_ALL))
                 #使用 Qos1
                 await session.send_and_request(MqConstants.MQ_EVENT_UNSUBSCRIBE, entity, 30_000).waiter()
                 log.info(f"Client unsubscribe successfully: {topic}#{consumerGroup}， sessionId={session.session_id()}")
 
     async def publish(self, topic: str, message: MqMessage):
-        MqAssert.requireNonNull(topic, "Param 'topic' can't be null")
-        MqAssert.requireNonNull(message, "Param 'message' can't be null")
+        MqAssert.require_non_null(topic, "Param 'topic' can't be null")
+        MqAssert.require_non_null(message, "Param 'message' can't be null")
 
-        MqAssert.assertMeta(topic, "topic")
+        MqAssert.assert_meta(topic, "topic")
 
         if self._clientSession is None:
             raise SocketDConnectionException("Not connected!")
 
         # 支持命名空间
-        topic = MqTopicHelper.getFullTopic(self._namespace, topic)
+        topic = MqTopicHelper.get_full_topic(self._namespace, topic)
         session = self._clientSession.get_session_any(self._diversionOrNull(topic, message))
 
         if session is None or session.is_valid() == False:
             raise SocketDException("No session is available!")
 
-        entity = MqUtils.getOf(session).publishEntityBuild(topic, message)
+        entity = MqUtils.get_of(session).publish_entity_build(topic, message)
 
-        if message.getQos() > 0:
+        if message.get_qos() > 0:
             resp = await session.send_and_request(MqConstants.MQ_EVENT_PUBLISH, entity, 0).waiter()
             confirm = int(resp.meta_or_default(MqConstants.MQ_META_CONFIRM, "0"))
             if confirm != 1:
                 messsage = "Client message publish confirm failed: " + resp.data_as_string()
                 raise FolkmqException(messsage)
         else:
             session.send(MqConstants.MQ_EVENT_PUBLISH, entity)
 
-    def publishAsync(self, topic: str, message: MqMessage) -> CompletableFuture:
-        MqAssert.requireNonNull(topic, "Param 'topic' can't be null")
-        MqAssert.requireNonNull(message, "Param 'message' can't be null")
+    def publish_async(self, topic: str, message: MqMessage) -> CompletableFuture:
+        MqAssert.require_non_null(topic, "Param 'topic' can't be null")
+        MqAssert.require_non_null(message, "Param 'message' can't be null")
 
-        MqAssert.assertMeta(topic, "topic")
+        MqAssert.assert_meta(topic, "topic")
 
         if self._clientSession is None:
             raise SocketDConnectionException("Not connected!")
 
         # 支持命名空间
-        topic = MqTopicHelper.getFullTopic(self._namespace, topic)
+        topic = MqTopicHelper.get_full_topic(self._namespace, topic)
         session = self._clientSession.get_session_any(self._diversionOrNull(topic, message))
 
         if session is None or session.is_valid() == False:
             raise SocketDException("No session is available!")
 
-        entity = MqUtils.getOf(session).publishEntityBuild(topic, message)
+        entity = MqUtils.get_of(session).publish_entity_build(topic, message)
 
-        if message.getQos() > 0:
+        if message.get_qos() > 0:
             _future :CompletableFuture  = CompletableFuture()
             def _then_reply_do(resp:Reply):
                 confirm = int(resp.meta_or_default(MqConstants.MQ_META_CONFIRM, "0"))
                 if confirm != 1:
                     messsage = "Client message publish confirm failed: " + resp.data_as_string()
                     _future.set_e(FolkmqException(messsage))
                     _future.accept(False)
@@ -239,25 +242,25 @@
             return _future
 
         else:
             session.send(MqConstants.MQ_EVENT_PUBLISH, entity)
             return None
 
     async def unpublish(self, topic: str, key: str):
-        MqAssert.requireNonNull(topic, "Param 'topic' can't be null")
-        MqAssert.requireNonNull(key, "Param 'key' can't be null")
+        MqAssert.require_non_null(topic, "Param 'topic' can't be null")
+        MqAssert.require_non_null(key, "Param 'key' can't be null")
 
-        MqAssert.assertMeta(topic, "topic")
-        MqAssert.assertMeta(key, "key")
+        MqAssert.assert_meta(topic, "topic")
+        MqAssert.assert_meta(key, "key")
 
         if self._clientSession is None:
             raise SocketDConnectionException("Not connected!")
 
         #支持命名空间
-        topic = MqTopicHelper.getFullTopic(self._namespace, topic)
+        topic = MqTopicHelper.get_full_topic(self._namespace, topic)
         session = self._clientSession.get_session_any(None)
         if session is None or session.is_valid() == False:
             raise SocketDException("No session is available!")
 
         entity = (StringEntity("")
                   .meta_put(MqConstants.MQ_META_TOPIC, topic)
                   .meta_put(MqConstants.MQ_META_KEY, key)
@@ -280,43 +283,43 @@
 
     def send(self, message: MqMessage, toName: str, timeout: int | None = None) -> RequestStream | None:
         # 检查必要条件
         if self._name is None:
             return FolkmqException("Client 'name' can't be empty")
 
         # 检查参数
-        MqAssert.requireNonNull(toName, "Param 'toName' can't be null")
-        MqAssert.requireNonNull(message, "Param 'message' can't be null")
+        MqAssert.require_non_null(toName, "Param 'toName' can't be null")
+        MqAssert.require_non_null(message, "Param 'message' can't be null")
 
-        MqAssert.assertMeta(toName, "toName")
+        MqAssert.assert_meta(toName, "toName")
 
         if self._clientSession is None:
             raise SocketDConnectionException("Not connected!")
 
         session = self._clientSession.get_session_any(None)
         if session is None or session.is_valid() == False:
             raise SocketDException("No session is available!")
 
-        message.internalSender(self.name())
-        entity = MqUtils.getOf(session).publishEntityBuild("", message)
+        message.internal_sender(self.name())
+        entity = MqUtils.get_of(session).publish_entity_build("", message)
         entity.put_meta(MqMetasV2.MQ_META_CONSUMER_GROUP, toName)
         entity.at(toName)
 
-        if message.getQos() > 0:
+        if message.get_qos() > 0:
             return session.send_and_request(MqConstants.MQ_EVENT_REQUEST, entity, timeout)
         else:
             session.send(MqConstants.MQ_EVENT_REQUEST, entity)
             return None
 
-    def transactionCheckback(self, transactionCheckback: Callable[[MqMessageReceived], None]):
+    def transaction_checkback(self, transactionCheckback: Callable[[MqMessageReceived], None]):
         if transactionCheckback is not None:
             self._transactionCheckback = transactionCheckback
         return self
 
-    def newTransaction(self) -> MqTransaction:
+    def new_transaction(self) -> MqTransaction:
         if self._name is None:
             return FolkmqException("Client 'name' can't be empty")
 
         return MqTransactionImpl(self)
 
     async def publish2(self, tmid: str, keyAry: [str], isRollback: bool):
         if keyAry is None or len(keyAry) == 0:
@@ -340,29 +343,29 @@
         if confirm != 1:
             messsage = "Client message publish2 confirm failed: " + resp.data_as_string()
             raise FolkmqException(messsage)
 
 
     def reply(self, session: Session, f: Message, message: MqMessageReceivedImpl, isOk: bool, entity: Entity):
         """发送“回执”，向服务端反馈消费情况"""
-        if message.getQos() > 0:
+        if message.get_qos() > 0:
             if session.is_valid():
                 if entity is None:
                     entity = EntityDefault()
 
                 if isinstance(entity, MqAlarm):
                     RunUtils.taskTry(session.send_alarm(f, entity.data_as_string()))
                 else:
                     entity.put_meta(MqConstants.MQ_META_ACK, "1" if isOk else "0")
                     RunUtils.taskTry(session.reply_end(f, entity))
 
     def _diversionOrNull(self, fullTopic: str, message: MqMessage) -> str | None:
-        if message.isTransaction():
-            return message.getTmid()
-        elif message.isSequence():
+        if message.is_transaction():
+            return message.get_tmid()
+        elif message.is_sequence():
             if message.getSequenceSharding():
                 return message.getSequenceSharding()
             else:
                 return fullTopic
         else:
             return None
```

### Comparing `folkmq-1.4.4/folkmq/client/MqClientListener.py` & `folkmq-1.4.5/folkmq/client/MqClientListener.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import traceback
 
 from socketd.exception.SocketDExecption import SocketDAlarmException
+from socketd.transport.core.EntityMetas import EntityMetas
 from socketd.transport.core.Message import Message
 from socketd.transport.core.Session import Session
 from socketd.transport.core.entity.StringEntity import StringEntity
 from socketd.transport.core.listener.EventListener import EventListener
 from socketd.utils.LogConfig import log
 
 from folkmq.client.MqMessageReceived import MqMessageReceivedImpl
@@ -36,82 +37,83 @@
             e_msg = traceback.format_exc()
             log.warning(f"Client consume handle error, sid={m.sid()} \n{e_msg}")
 
     def onReceive(self, s: Session, m: Message, message: MqMessageReceivedImpl, isRequest: bool):
         """接收时"""
         if isRequest:
             try:
-                if message.isTransaction():
+                if message.is_transaction():
                     if self._client._transactionCheckback is not None:
                         self._client._transactionCheckback(message)
                     else:
                         s.send_alarm(m, "Client no checkback handler!")
                 else:
                     if self._client._listenHandler is not None:
                         self._client._listenHandler(message)
                     else:
                         s.send_alarm(m, "Client no request handler!")
             except Exception as e:
                 try:
                     e_msg = traceback.format_exc()
                     if s.is_valid():
                         s.send_alarm(m, "Client request handle error:" + e)
-                    log.warning(f"Client request handle error, key={message.getKey()} \n{e_msg}")
+                    log.warning(f"Client request handle error, key={message.get_key()} \n{e_msg}")
                 except Exception as err:
                     err_msg = traceback.format_exc()
-                    log.warning(f"Client request handle error, key={message.getKey()} \n{err_msg}")
+                    log.warning(f"Client request handle error, key={message.get_key()} \n{err_msg}")
         else:
-            subscription = self._client.getSubscription(message.getFullTopic(), message.getConsumerGroup())
+            subscription = self._client.getSubscription(message.getFullTopic(), message.get_consumer_group())
 
             try:
                 if subscription is not None:
                     # 有订阅
                     subscription.consume(message)
-                    if subscription.isAutoAck():
+                    if subscription.is_auto_ack():
                         self._client.reply(s, m, message, True, None)
                 else:
                     # 没有订阅
                     self._client.reply(s, m, message, False, None)
             except Exception as e:
                 try:
                     if subscription is not None:
                         # 有订阅
-                        if subscription.isAutoAck():
+                        if subscription.is_auto_ack():
                             self._client.reply(s, m, message, False, None)
                     else:
                         # 没有订阅
                         self._client.reply(s, m, message, False, None)
 
                     e_msg = traceback.format_exc()
-                    log.warning(f"Client consume handle error, key={message.getKey()} \n{e_msg}")
+                    log.warning(f"Client consume handle error, key={message.get_key()} \n{e_msg}")
                 except Exception as err:
                     err_msg = traceback.format_exc()
-                    log.warning(f"Client consume handle error, key={message.getKey()} \n{err_msg}")
+                    log.warning(f"Client consume handle error, key={message.get_key()} \n{err_msg}")
 
     async def on_open(self, session:Session):
         """会话打开时"""
         await super().on_open(session)
 
         log.info(f"Client session opened, sessionId={session.session_id()}")
 
         if self._client.getSubscriptionSize() == 0:
             return
 
         subscribeData:dict[str,str] = {}
         for subscription in self._client.getSubscriptionAll():
-            queueNameSet = subscribeData.get(subscription.getTopic())
+            queueNameSet = subscribeData.get(subscription.get_topic())
             if queueNameSet is None:
                 queueNameSet = set()
-                subscribeData[subscription.getTopic()] = queueNameSet
+                subscribeData[subscription.get_topic()] = queueNameSet
 
-            queueNameSet.add(subscription.getQueueName())
+            queueNameSet.add(subscription.get_queue_name())
 
         jsonStr = json.dumps(subscribeData)
         entity = (StringEntity(jsonStr)
                   .meta_put(MqConstants.MQ_META_BATCH, "1")
+                  .meta_put(EntityMetas.META_X_UNLIMITED, "1")
                   .meta_put("@", MqConstants.BROKER_AT_SERVER))
 
         await session.send_and_request(MqConstants.MQ_EVENT_SUBSCRIBE, entity).waiter()
 
         log.info(f"Client onOpen batch subscribe successfully, sessionId={session.session_id()}")
 
     def on_close(self, session: Session):
```

### Comparing `folkmq-1.4.4/folkmq/client/MqMessage.py` & `folkmq-1.4.5/folkmq/client/MqMessage.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,50 +1,51 @@
+from abc import abstractmethod
 from datetime import datetime
 
 from socketd.utils.StrUtils import StrUtils
 
 from folkmq.client.MqTransaction import MqTransaction
 
 
 class MqMessageBase:
     #发送人
-    @staticmethod
-    def getSender(self) -> str | None: ...
+    @abstractmethod
+    def get_sender(self) -> str | None: ...
 
     #主建
-    @staticmethod
-    def getKey(self) -> str: ...
+    @abstractmethod
+    def get_key(self) -> str: ...
 
     #标签
-    @staticmethod
-    def getTag(self) -> str: ...
+    @abstractmethod
+    def get_tag(self) -> str: ...
 
     #内容
-    @staticmethod
-    def getBody(self) -> bytes: ...
+    @abstractmethod
+    def get_body(self) -> bytes: ...
 
     #过期时间
-    @staticmethod
-    def getExpiration(self) -> datetime | None: ...
+    @abstractmethod
+    def get_expiration(self) -> datetime | None: ...
 
     #是否事务
-    @staticmethod
-    def isTransaction(self) -> bool: ...
+    @abstractmethod
+    def is_transaction(self) -> bool: ...
 
     #是否有序
-    @staticmethod
-    def isSequence(self) -> bool: ...
+    @abstractmethod
+    def is_sequence(self) -> bool: ...
 
     #质量等级
-    @staticmethod
-    def getQos(self) -> int: ...
+    @abstractmethod
+    def get_qos(self) -> int: ...
 
     #获取属性
-    @staticmethod
-    def getAttr(self, name: str) -> str | None: ...
+    @abstractmethod
+    def get_attr(self, name: str) -> str | None: ...
 
 
 class MqMessage(MqMessageBase):
     def __init__(self, body: str|bytes, key:str|None = None) :
         if key:
             self.__key = key
         else:
@@ -62,49 +63,49 @@
         self.__sequence:bool = False
         self.__sequenceSharding: str | None = None
         self.__qos:int = 1
 
         self.__attrMap: dict[str, str] = {}
         self.__transaction:MqTransaction = None
 
-    def getSender(self) -> str | None:
+    def get_sender(self) -> str | None:
         return self.__sender
 
-    def getKey(self) -> str:
+    def get_key(self) -> str:
         return self.__key
 
-    def getTag(self) -> str | None:
+    def get_tag(self) -> str | None:
         return self.__tag
 
-    def getBody(self) -> bytes:
+    def get_body(self) -> bytes:
         return self.__body
 
     def getScheduled(self) -> datetime:
         return self.__scheduled
 
-    def getExpiration(self) -> datetime:
+    def get_expiration(self) -> datetime:
         return self.__expiration
 
-    def isTransaction(self) -> bool:
+    def is_transaction(self) -> bool:
         return self.__transaction is not None
 
-    def isSequence(self) -> bool:
+    def is_sequence(self) -> bool:
         return self.__sequence
 
     def getSequenceSharding(self)->str:
         return self.__sequenceSharding
 
-    def getQos(self) -> int:
+    def get_qos(self) -> int:
         return self.__qos
 
     def tag(self, tag: str)->'MqMessage':
         self.__tag = tag
         return self
 
-    def asJson(self)-> 'MqMessage':
+    def as_json(self)-> 'MqMessage':
         self.attr("Content-Type", "application/json")
         return self;
 
 
 
     def scheduled(self, scheduled: datetime)-> 'MqMessage':
         self.__scheduled = scheduled
@@ -128,34 +129,34 @@
     def transaction(self, transaction: MqTransaction|None)-> 'MqMessage':
         if transaction is not None:
             self.__transaction = transaction
             transaction.binding(self)
 
         return self
 
-    def getTmid(self)-> str | None:
+    def get_tmid(self)-> str | None:
         if self.__transaction is None:
             return None
         else:
             return self.__transaction.tmid()
 
-    def internalSender(self, sender: str)-> 'MqMessage':
+    def internal_sender(self, sender: str)-> 'MqMessage':
         self.__sender = sender
         return self
 
     def qos(self, qos: int)-> 'MqMessage':
         self.__qos = qos
         return self
 
-    def getAttr(self, name: str)-> str | None:
+    def get_attr(self, name: str)-> str | None:
         tmp = self.__attrMap.get(name);
         return tmp;
 
 
-    def getAttrMap(self)-> dict[str,str]:
+    def get_attr_map(self)-> dict[str,str]:
         return self.__attrMap
 
 
     def attr(self, name: str, value: str)-> 'MqMessage':
         self.__attrMap.set(name, value)
         return self
```

### Comparing `folkmq-1.4.4/folkmq/client/MqMessageReceived.py` & `folkmq-1.4.5/folkmq/client/MqMessageReceived.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,30 +10,30 @@
 from folkmq.common.MqTopicHelper import MqTopicHelper
 from folkmq.common.MqUtils import MqUtils
 
 
 class MqMessageReceived(MqMessageBase):
     # 主题
     @abstractmethod
-    def getTopic(self) -> str:
+    def get_topic(self) -> str:
         ...
 
     # 内容
     @abstractmethod
-    def getBodyAsString(self) -> str:
+    def get_body_as_string(self) -> str:
         ...
 
     # 消费者组
     @abstractmethod
-    def getConsumerGroup(self) -> str:
+    def get_consumer_group(self) -> str:
         ...
 
     # 已派发次数
     @abstractmethod
-    def getTimes(self) -> int:
+    def get_times(self) -> int:
         ...
 
     # 回执
     @abstractmethod
     def acknowledge(self, isOk: bool):
         ...
 
@@ -44,84 +44,84 @@
 
 class MqMessageReceivedImpl(MqMessageReceived):
     def __init__(self, clientInternal:'MqClientInternal', session:Session, source:Message):
         self._clientInternal = clientInternal
         self._session = session
         self._source = source
 
-        mr  = MqUtils.getOf(source)
+        mr  = MqUtils.get_of(source)
 
-        self._sender = mr.getSender(source)
+        self._sender = mr.get_sender(source)
 
-        self._key = mr.getKey(source)
-        self._tag = mr.getTag(source)
-        self._fullTopic = mr.getTopic(source)
-        self._topic = MqTopicHelper.getTopic(self._fullTopic)
-        self._consumerGroup = mr.getConsumerGroup(source)
-
-        self._qos = mr.getQos(source)
-        self._times = mr.getTimes(source)
-        self._sequence = mr.isSequence(source)
-        self._transaction = mr.isTransaction(source)
+        self._key = mr.get_key(source)
+        self._tag = mr.get_tag(source)
+        self._fullTopic = mr.get_topic(source)
+        self._topic = MqTopicHelper.get_topic(self._fullTopic)
+        self._consumerGroup = mr.get_consumer_group(source)
+
+        self._qos = mr.get_qos(source)
+        self._times = mr.get_times(source)
+        self._sequence = mr.is_sequence(source)
+        self._transaction = mr.is_transaction(source)
 
-        self._expirationL = mr.getExpiration(source)
+        self._expirationL = mr.get_expiration(source)
         self._expiration = self._expirationL
 
     def getSource(self) -> Message:
         return self._source
 
-    def getSender(self) -> str | None:
+    def get_sender(self) -> str | None:
         return self._sender
 
-    def getKey(self) -> str:
+    def get_key(self) -> str:
         return self._key
 
-    def getTag(self) -> str:
+    def get_tag(self) -> str:
         return self._tag
 
-    def getTopic(self) -> str:
+    def get_topic(self) -> str:
         return self._topic
 
     def getFullTopic(self)->str:
         return self._fullTopic
 
-    def getConsumerGroup(self) -> str:
+    def get_consumer_group(self) -> str:
         return self._consumerGroup
 
-    def getBody(self) -> bytes:
+    def get_body(self) -> bytes:
         return self._source.data_as_bytes()
-    def getBodyAsString(self) -> str:
+    def get_body_as_string(self) -> str:
         return self._source.data_as_string()
 
-    def getQos(self) -> int:
+    def get_qos(self) -> int:
         return self._qos
 
-    def getAttr(self, name: str) -> str | None:
+    def get_attr(self, name: str) -> str | None:
         return self._source.meta(MqConstants.MQ_ATTR_PREFIX + name)
 
-    def getExpiration(self) -> datetime | None:
+    def get_expiration(self) -> datetime | None:
         return self._expiration
 
-    def isTransaction(self) -> bool:
+    def is_transaction(self) -> bool:
         return self._transaction
 
-    def isSequence(self) -> bool:
+    def is_sequence(self) -> bool:
         return self._sequence
 
-    def getTimes(self) -> int:
+    def get_times(self) -> int:
         return self._times
 
     def acknowledge(self, isOk: bool):
         self._clientInternal.reply(self._session, self._source, self, isOk, None)
 
     def response(self, entity:Entity):
         self._clientInternal.reply(self._session, self._source, self, True, entity)
 
     def __str__(self) ->str:
         return "MqMessageReceived{" + \
             "key='" + self._key + '\'' + \
             ", tag='" + self._tag + '\'' + \
             ", topic='" + self._topic + '\'' + \
-            ", body='" + self.getBodyAsString() + '\'' + \
+            ", body='" + self.get_body_as_string() + '\'' + \
             '}'
```

### Comparing `folkmq-1.4.4/folkmq/client/MqRouter.py` & `folkmq-1.4.5/folkmq/client/MqRouter.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 class MqRouter:
     def __init__(self, mappingHandler: Callable[[MqMessageReceived], str]):
         self._mappingHandler:Callable[[MqMessageReceived], str] = mappingHandler
         self._mappingMap:Dict[str,str] = {}
         self._consumeHandler:Union[Callable[[MqMessageReceived], None], None] = None
 
     # 添加映射处理
-    def doOn(self, mapping:str, consumeHandler:Callable[[MqMessageReceived], None]) -> 'MqRouter':
+    def do_on(self, mapping:str, consumeHandler:Callable[[MqMessageReceived], None]) -> 'MqRouter':
         self._mappingMap[mapping] = consumeHandler
         return self
 
     # 添加消费处理
-    def doOnConsume(self, consumeHandler:Callable[[MqMessageReceived], None]) -> 'MqRouter':
+    def do_on_consume(self, consumeHandler:Callable[[MqMessageReceived], None]) -> 'MqRouter':
         self._consumeHandler = consumeHandler
         return self
 
     # 消费
     def consume(self, message:MqMessageReceived):
         if self._consumeHandler:
             self._consumeHandler(message)
```

### Comparing `folkmq-1.4.4/folkmq/client/MqSubscription.py` & `folkmq-1.4.5/folkmq/client/MqSubscription.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,21 +8,21 @@
     def __init__(self, topic: str, consumerGroup: str, autoAck: bool, consumeHandler:Callable[[MqMessageReceived], None]):
         self._topic = topic
         self._consumerGroup = consumerGroup
         self._autoAck = autoAck
         self._queueName = topic + MqConstants.SEPARATOR_TOPIC_CONSUMER_GROUP + consumerGroup
         self._consumeHandler = consumeHandler
 
-    def getTopic(self) -> str:
+    def get_topic(self) -> str:
         return self._topic
 
-    def getConsumerGroup(self) -> str:
+    def get_consumer_group(self) -> str:
         return self._consumerGroup
 
-    def isAutoAck(self) -> bool:
+    def is_auto_ack(self) -> bool:
         return self._autoAck
 
-    def getQueueName(self) -> str:
+    def get_queue_name(self) -> str:
         return self._queueName
 
     def consume(self, message:MqMessageReceived):
         self._consumeHandler(message)
```

### Comparing `folkmq-1.4.4/folkmq/client/MqTransaction.py` & `folkmq-1.4.5/folkmq/client/MqTransaction.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         self._keyAry:[str] = []
         self._tmid:str = StrUtils.guid()
 
     def tmid(self) -> str:
         return self._tmid
 
     def binding(self, message: 'MqMessage'):
-        self._keyAry.append(message.getKey())
-        message.internalSender(self._client.name())
+        self._keyAry.append(message.get_key())
+        message.internal_sender(self._client.name())
 
     async def commit(self):
         await self._client.publish2(self._tmid, self._keyAry, False)
 
     async def rollback(self):
         await self._client.publish2(self._tmid, self._keyAry, True)
```

### Comparing `folkmq-1.4.4/folkmq/common/MqAssert.py` & `folkmq-1.4.5/folkmq/common/MqAssert.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 class MqAssert:
     @staticmethod
-    def requireNonNull(obj, message:str):
+    def require_non_null(obj, message:str):
         if obj is None:
             raise Exception(message)
         else:
             return obj
     @staticmethod
-    def assertMeta(str:str, paramName:str):
-        MqAssert.assertMetaSymbols(str, paramName, '?', "?")
-        MqAssert.assertMetaSymbols(str, paramName, '&', "&")
-        MqAssert.assertMetaSymbols(str, paramName, '=', "=")
-        MqAssert.assertMetaSymbols(str, paramName, '!', "!")
+    def assert_meta(str:str, paramName:str):
+        MqAssert.assert_meta_symbols(str, paramName, '?', "?")
+        MqAssert.assert_meta_symbols(str, paramName, '&', "&")
+        MqAssert.assert_meta_symbols(str, paramName, '=', "=")
+        MqAssert.assert_meta_symbols(str, paramName, '!', "!")
 
-        MqAssert.assertMetaSymbols(str, paramName, '@', "@")
-        MqAssert.assertMetaSymbols(str, paramName, '#', "#")
-        MqAssert.assertMetaSymbols(str, paramName, '$', "$")
-        MqAssert.assertMetaSymbols(str, paramName, '%', "%")
-        MqAssert.assertMetaSymbols(str, paramName, '^', "^")
-        MqAssert.assertMetaSymbols(str, paramName, '*', "*")
+        MqAssert.assert_meta_symbols(str, paramName, '@', "@")
+        MqAssert.assert_meta_symbols(str, paramName, '#', "#")
+        MqAssert.assert_meta_symbols(str, paramName, '$', "$")
+        MqAssert.assert_meta_symbols(str, paramName, '%', "%")
+        MqAssert.assert_meta_symbols(str, paramName, '^', "^")
+        MqAssert.assert_meta_symbols(str, paramName, '*', "*")
 
     @staticmethod
-    def assertMetaSymbols(str: str, paramName: str, c:str, cS:str):
+    def assert_meta_symbols(str: str, paramName: str, c:str, cS:str):
         if str.find(c) >= 0:
             raise Exception("Param '" + paramName + "' can't have symbols: '" + cS + "'");
```

### Comparing `folkmq-1.4.4/folkmq/common/MqConstants.py` & `folkmq-1.4.5/folkmq/common/MqConstants.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.4/folkmq/common/MqMetasResolver.py` & `folkmq-1.4.5/folkmq/common/MqMetasResolver.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,116 +14,116 @@
     @abc.abstractmethod
     def version(self)-> int:...
 
     #
     # 获取发送人
     #
     @abc.abstractmethod
-    def getSender(self, m: Entity)-> str:...
+    def get_sender(self, m: Entity)-> str:...
 
     #
     # 获取主建
     #
     @abc.abstractmethod
-    def getKey(self, m: Entity)-> str:...
+    def get_key(self, m: Entity)-> str:...
 
     #
     # 获取标签
     #
     @abc.abstractmethod
-    def getTag(self, m: Entity)-> str:...
+    def get_tag(self, m: Entity)-> str:...
 
     #
     # 获取主题
     #
     @abc.abstractmethod
-    def getTopic(self, m: Entity)-> str:...
+    def get_topic(self, m: Entity)-> str:...
 
     #
     # 获取消费者组
     #
     @abc.abstractmethod
-    def getConsumerGroup(self, m: Entity)-> str:...
+    def get_consumer_group(self, m: Entity)-> str:...
 
     #
     # 设置消费者组
     #
     @abc.abstractmethod
-    def setConsumerGroup(self, m: Entity, consumerGroup: str):...
+    def set_consumer_group(self, m: Entity, consumerGroup: str):...
 
     #
     # 获取质量等级（0或1）
     #
     @abc.abstractmethod
-    def getQos(self, m: Entity)-> int:...
+    def get_qos(self, m: Entity)-> int:...
 
     #
     # 获取派发次数
     #
     @abc.abstractmethod
-    def getTimes(self, m: Entity)-> int:...
+    def get_times(self, m: Entity)-> int:...
 
     #
     # 设置派发次数
     #
     @abc.abstractmethod
-    def setTimes(self, m: Entity, times: int):...
+    def set_times(self, m: Entity, times: int):...
 
     #
     # 获取过期时间
     #
     @abc.abstractmethod
-    def getExpiration(self, m: Entity)->float:...
+    def get_expiration(self, m: Entity)->float:...
 
     #
     # 设置过期时间
     #
     @abc.abstractmethod
-    def setExpiration(self, m: Entity, expiration: int):...
+    def set_expiration(self, m: Entity, expiration: int):...
 
     #
     # 获取定时时间
     #
     @abc.abstractmethod
-    def getScheduled(self, m: Entity)-> int:...
+    def get_scheduled(self, m: Entity)-> int:...
 
     #
     # 设置定时时间
     #
     @abc.abstractmethod
-    def setScheduled(self, m: Entity, scheduled: int):...
+    def set_scheduled(self, m: Entity, scheduled: int):...
 
     #
     # 是否有序
     #
     @abc.abstractmethod
-    def isSequence(self, m: Entity)->bool:...
+    def is_sequence(self, m: Entity)->bool:...
 
     #
     # 是否事务
     #
     @abc.abstractmethod
-    def isTransaction(self, m: Entity)->bool:...
+    def is_transaction(self, m: Entity)->bool:...
 
     #
     # 设置事务
     #
     @abc.abstractmethod
-    def setTransaction(self, m: Entity, isTransaction: bool):...
+    def set_transaction(self, m: Entity, isTransaction: bool):...
 
     #
     # 发布实体构建
     #
     # @param topic   主题
     # @param message 消息
     #
     @abc.abstractmethod
-    def publishEntityBuild(self, topic: str, message: MqMessage)-> EntityDefault:...
+    def publish_entity_build(self, topic: str, message: MqMessage)-> EntityDefault:...
 
     #
     # 路由消息构建
     #
     # @param topic   主题
     # @param message 消息
     #
     @abc.abstractmethod
-    def routingMessageBuild(self, topic: str, message: MqMessage)-> Message:...
+    def routing_message_build(self, topic: str, message: MqMessage)-> Message:...
```

### Comparing `folkmq-1.4.4/folkmq/common/MqMetasResolverV1.py` & `folkmq-1.4.5/folkmq/common/MqMetasResolverV1.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,114 +14,114 @@
 from folkmq.common.MqMetasV2 import MqMetasV2
 
 
 class MqMetasResolverV1(MqMetasResolver):
     def version(self) -> int:
         return 1
 
-    def getSender(self, m: Entity) -> str:
+    def get_sender(self, m: Entity) -> str:
         return m.meta_or_default(MqMetasV2.MQ_META_SENDER, "");
 
-    def getKey(self, m: Entity) -> str:
+    def get_key(self, m: Entity) -> str:
         return m.meta_or_default(MqMetasV1.MQ_META_KEY, "");
 
-    def getTag(self, m: Entity) -> str:
+    def get_tag(self, m: Entity) -> str:
         return m.meta_or_default(MqMetasV2.MQ_META_TAG, "");
 
-    def getTopic(self, m: Entity) -> str:
+    def get_topic(self, m: Entity) -> str:
         return m.meta_or_default(MqMetasV1.MQ_META_TOPIC, "");
 
-    def getConsumerGroup(self, m: Entity) -> str:
+    def get_consumer_group(self, m: Entity) -> str:
         return m.meta_or_default(MqMetasV1.MQ_META_CONSUMER_GROUP, "");
 
-    def setConsumerGroup(self, m: Entity, consumerGroup: str):
+    def set_consumer_group(self, m: Entity, consumerGroup: str):
         m.put_meta(MqMetasV1.MQ_META_CONSUMER_GROUP, consumerGroup);
 
-    def getQos(self, m: Entity) -> int:
+    def get_qos(self, m: Entity) -> int:
         return 0 if "0" == m.meta(MqMetasV1.MQ_META_QOS) else 1;
 
-    def getTimes(self, m: Entity) -> int:
+    def get_times(self, m: Entity) -> int:
         return int(m.meta_or_default(MqMetasV1.MQ_META_TIMES, "0"));
 
-    def setTimes(self, m: Entity, times: int):
+    def set_times(self, m: Entity, times: int):
         m.put_meta(MqMetasV1.MQ_META_TIMES, times.toString());
 
-    def getExpiration(self, m: Entity) -> float:
+    def get_expiration(self, m: Entity) -> float:
         return float(m.meta_or_default(MqMetasV1.MQ_META_EXPIRATION, "0"));
 
-    def setExpiration(self, m: Entity, expiration: int|None):
+    def set_expiration(self, m: Entity, expiration: int | None):
         if expiration is None:
             m.delMeta(MqMetasV1.MQ_META_EXPIRATION)
         else:
             m.put_meta(MqMetasV1.MQ_META_EXPIRATION, expiration.toString())
 
-    def getScheduled(self, m: Entity) -> int:
+    def get_scheduled(self, m: Entity) -> int:
         return int(m.meta_or_default(MqMetasV1.MQ_META_SCHEDULED, "0"))
 
-    def setScheduled(self, m: Entity, scheduled: int):
+    def set_scheduled(self, m: Entity, scheduled: int):
         m.put_meta(MqMetasV1.MQ_META_SCHEDULED, scheduled.toString())
 
-    def isSequence(self, m: Entity) -> bool:
+    def is_sequence(self, m: Entity) -> bool:
         return "1" == (m.meta_or_default(MqMetasV1.MQ_META_SEQUENCE, "0"))
 
-    def isTransaction(self, m: Entity) -> bool:
+    def is_transaction(self, m: Entity) -> bool:
         return "1" == (m.meta(MqMetasV2.MQ_META_TRANSACTION))
 
-    def setTransaction(self, m: Entity, isTransaction: bool):
+    def set_transaction(self, m: Entity, isTransaction: bool):
         m.put_meta(MqMetasV2.MQ_META_TRANSACTION, ( "1" if isTransaction else "0"))
 
-    def publishEntityBuild(self, topic: str, message: MqMessage) -> EntityDefault:
+    def publish_entity_build(self, topic: str, message: MqMessage) -> EntityDefault:
         # 构建消息实体
-        entity = EntityDefault().data_set(message.getBody())
+        entity = EntityDefault().data_set(message.get_body())
 
-        entity.meta_put(MqMetasV1.MQ_META_KEY, message.getKey())
+        entity.meta_put(MqMetasV1.MQ_META_KEY, message.get_key())
         entity.meta_put(MqMetasV1.MQ_META_TOPIC, topic)
-        entity.meta_put(MqMetasV1.MQ_META_QOS, ("0" if message.getQos() == 0 else "1"))
+        entity.meta_put(MqMetasV1.MQ_META_QOS, ("0" if message.get_qos() == 0 else "1"))
 
         # 标签
-        if message.getTag():
-            entity.meta_put(MqMetasV2.MQ_META_TAG, message.getTag())
+        if message.get_tag():
+            entity.meta_put(MqMetasV2.MQ_META_TAG, message.get_tag())
 
 
         # 定时派发
         if message.getScheduled():
             entity.meta_put(MqMetasV1.MQ_META_SCHEDULED, str(message.getScheduled().getTime()))
         else:
             entity.meta_put(MqMetasV1.MQ_META_SCHEDULED, "0")
 
         # 过期时间
-        if message.getExpiration() is not None:
-            entity.meta_put(MqMetasV1.MQ_META_EXPIRATION, str(message.getExpiration().getTime()))
+        if message.get_expiration() is not None:
+            entity.meta_put(MqMetasV1.MQ_META_EXPIRATION, str(message.get_expiration().getTime()))
 
 
-        if  message.isTransaction():
+        if  message.is_transaction():
             entity.meta_put(MqMetasV2.MQ_META_TRANSACTION, "1")
 
 
-        if message.getSender():
-            entity.meta_put(MqMetasV2.MQ_META_SENDER, message.getSender())
+        if message.get_sender():
+            entity.meta_put(MqMetasV2.MQ_META_SENDER, message.get_sender())
 
 
         # 是否有序
-        if  message.isSequence() or message.isTransaction():
+        if  message.is_sequence() or message.is_transaction():
             entity.at(MqConstants.BROKER_AT_SERVER_HASH)
 
-        if message.isSequence():
+        if message.is_sequence():
             entity.meta_put(MqMetasV1.MQ_META_SEQUENCE, "1")
         else:
             entity.at(MqConstants.BROKER_AT_SERVER)
 
         # 用户属性
         #message.getAttrMap().forEach((value, key, map) = > {
         #    entity.put_meta(MqConstants.MQ_ATTR_PREFIX + key, value)
         #})
 
         return entity
 
-    def routingMessageBuild(self, topic: str, message: MqMessage) -> Message:
-        entity = self.publishEntityBuild(topic, message).at(MqConstants.BROKER_AT_SERVER)
+    def routing_message_build(self, topic: str, message: MqMessage) -> Message:
+        entity = self.publish_entity_build(topic, message).at(MqConstants.BROKER_AT_SERVER)
         messageDefault =  MessageBuilder().flag(Flags.Message) \
                                 .sid(StrUtils.guid()) \
                                 .event(MqConstants.MQ_EVENT_PUBLISH) \
                                 .entity(entity) \
                                 .build()
         return messageDefault
```

### Comparing `folkmq-1.4.4/folkmq/common/MqMetasResolverV2.py` & `folkmq-1.4.5/folkmq/common/MqMetasResolverV2.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,116 +14,116 @@
 from folkmq.common.MqMetasV2 import MqMetasV2
 
 
 class MqMetasResolverV2(MqMetasResolver):
     def version(self) -> int:
         return 2
 
-    def getSender(self, m: Entity) -> str:
+    def get_sender(self, m: Entity) -> str:
         return m.meta_or_default(MqMetasV2.MQ_META_SENDER, "")
 
-    def getKey(self, m: Entity) -> str:
+    def get_key(self, m: Entity) -> str:
         return m.meta_or_default(MqMetasV2.MQ_META_KEY, "")
 
-    def getTag(self, m: Entity) -> str:
+    def get_tag(self, m: Entity) -> str:
         return m.meta_or_default(MqMetasV2.MQ_META_TAG, "")
 
-    def getTopic(self, m: Entity) -> str:
+    def get_topic(self, m: Entity) -> str:
         return m.meta_or_default(MqMetasV2.MQ_META_TOPIC, "")
 
-    def getConsumerGroup(self, m: Entity) -> str:
+    def get_consumer_group(self, m: Entity) -> str:
         return m.meta_or_default(MqMetasV2.MQ_META_CONSUMER_GROUP, "")
 
-    def setConsumerGroup(self, m: Entity, consumerGroup: str):
+    def set_consumer_group(self, m: Entity, consumerGroup: str):
         m.put_meta(MqMetasV2.MQ_META_CONSUMER_GROUP, consumerGroup)
 
-    def getQos(self, m: Entity) -> int:
+    def get_qos(self, m: Entity) -> int:
         return  0 if "0" == (m.meta(MqMetasV2.MQ_META_QOS)) else 1
 
-    def getTimes(self, m: Entity) -> int:
+    def get_times(self, m: Entity) -> int:
         return int(m.meta_or_default(MqMetasV2.MQ_META_TIMES, "0"))
 
-    def setTimes(self, m: Entity, times: int):
+    def set_times(self, m: Entity, times: int):
         m.put_meta(MqMetasV2.MQ_META_TIMES, str(times))
 
-    def getExpiration(self, m: Entity) -> float:
+    def get_expiration(self, m: Entity) -> float:
         return float(m.meta_or_default(MqMetasV2.MQ_META_EXPIRATION, "0"))
 
-    def setExpiration(self, m: Entity, expiration: int):
+    def set_expiration(self, m: Entity, expiration: int):
         if  expiration is None:
             m.del_meta(MqMetasV2.MQ_META_EXPIRATION)
         else:
             m.put_meta(MqMetasV2.MQ_META_EXPIRATION, str(expiration))
 
-    def getScheduled(self, m: Entity) -> int:
+    def get_scheduled(self, m: Entity) -> int:
         return int(m.meta_or_default(MqMetasV2.MQ_META_SCHEDULED, "0"))
 
-    def setScheduled(self, m: Entity, scheduled: int):
+    def set_scheduled(self, m: Entity, scheduled: int):
         m.put_meta(MqMetasV2.MQ_META_SCHEDULED, str(scheduled))
 
-    def isSequence(self, m: Entity) -> bool:
+    def is_sequence(self, m: Entity) -> bool:
         return "1" == (m.meta(MqMetasV2.MQ_META_SEQUENCE))
 
-    def isTransaction(self, m: Entity) -> bool:
+    def is_transaction(self, m: Entity) -> bool:
         return "1" == (m.meta(MqMetasV2.MQ_META_TRANSACTION))
 
-    def setTransaction(self, m: Entity, isTransaction: bool):
+    def set_transaction(self, m: Entity, isTransaction: bool):
         m.put_meta(MqMetasV2.MQ_META_TRANSACTION, ("1" if isTransaction else "0"))
 
-    def publishEntityBuild(self, topic: str, message: MqMessage) -> EntityDefault:
+    def publish_entity_build(self, topic: str, message: MqMessage) -> EntityDefault:
         #构建消息实体
-        entity = EntityDefault().data_set(message.getBody())
+        entity = EntityDefault().data_set(message.get_body())
 
-        entity.meta_put(MqMetasV2.MQ_META_KEY, message.getKey())
+        entity.meta_put(MqMetasV2.MQ_META_KEY, message.get_key())
         entity.meta_put(MqMetasV2.MQ_META_TOPIC, topic)
-        entity.meta_put(MqMetasV2.MQ_META_QOS, ("0" if message.getQos() == 0 else "1"))
+        entity.meta_put(MqMetasV2.MQ_META_QOS, ("0" if message.get_qos() == 0 else "1"))
 
         # 标签
-        if message.getTag():
-            entity.meta_put(MqMetasV2.MQ_META_TAG, message.getTag())
+        if message.get_tag():
+            entity.meta_put(MqMetasV2.MQ_META_TAG, message.get_tag())
 
         #定时派发
         if message.getScheduled() is None:
             entity.meta_put(MqMetasV2.MQ_META_SCHEDULED, "0")
         else:
             entity.meta_put(MqMetasV2.MQ_META_SCHEDULED, str(message.getScheduled()))
 
         # 过期时间
-        if message.getExpiration() is not None:
-            entity.meta_put(MqMetasV2.MQ_META_EXPIRATION, str(message.getExpiration()))
+        if message.get_expiration() is not None:
+            entity.meta_put(MqMetasV2.MQ_META_EXPIRATION, str(message.get_expiration()))
 
-        if message.isTransaction():
+        if message.is_transaction():
             entity.meta_put(MqMetasV2.MQ_META_TRANSACTION, "1")
 
-        if message.getSender():
-            entity.meta_put(MqMetasV2.MQ_META_SENDER, message.getSender())
+        if message.get_sender():
+            entity.meta_put(MqMetasV2.MQ_META_SENDER, message.get_sender())
 
         # 是否有序
-        if message.isSequence() or message.isTransaction():
+        if message.is_sequence() or message.is_transaction():
             entity.at(MqConstants.BROKER_AT_SERVER_HASH)
-            if message.isSequence():
+            if message.is_sequence():
                 entity.meta_put(MqMetasV2.MQ_META_SEQUENCE, "1");
 
-                if message.isTransaction() == False and message.getSequenceSharding():
+                if message.is_transaction() == False and message.getSequenceSharding():
                     # 不是事务，并且有顺序分片
-                    entity.meta_put(EntityMetas.META_X_Hash, message.getSequenceSharding())
+                    entity.meta_put(EntityMetas.META_X_HASH, message.getSequenceSharding())
         else:
             entity.at(MqConstants.BROKER_AT_SERVER)
 
         from folkmq.FolkMQ import FolkMQ
-        entity.meta_put(MqMetasV2.MQ_META_VID, str(FolkMQ.versionCode()))
+        entity.meta_put(MqMetasV2.MQ_META_VID, str(FolkMQ.version_code()))
 
         #用户属性
-        for kv in message.getAttrMap():
+        for kv in message.get_attr_map():
             entity.put_meta(MqConstants.MQ_ATTR_PREFIX + kv[0], kv[1])
 
         return entity
 
-    def routingMessageBuild(self, topic: str, message: MqMessage) -> Message:
-        entity = self.publishEntityBuild(topic, message)
+    def routing_message_build(self, topic: str, message: MqMessage) -> Message:
+        entity = self.publish_entity_build(topic, message)
         messageDefault = (MessageBuilder()
                           .flag(Flags.Message)
                           .sid(StrUtils.guid())
                           .event(MqConstants.MQ_EVENT_PUBLISH)
                           .entity(entity)
                           .build())
         return messageDefault
```

### Comparing `folkmq-1.4.4/folkmq/common/MqMetasV1.py` & `folkmq-1.4.5/folkmq/common/MqMetasV1.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.4/folkmq/common/MqMetasV2.py` & `folkmq-1.4.5/folkmq/common/MqMetasV2.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.4/folkmq/common/MqUtils.py` & `folkmq-1.4.5/folkmq/common/MqUtils.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # 消息工具类
 class MqUtils:
     __v1 = MqMetasResolverV1()
     __v2 = MqMetasResolverV2()
 
     @staticmethod
-    def getOf(t:Session|Message|None) -> MqMetasResolver:
+    def get_of(t: Session | Message | None) -> MqMetasResolver:
         if t is None:
             return MqUtils.__v2
         else:
             if isinstance(t, MessageDefault):
                 ver = t.meta_or_default(MqMetasV2.MQ_META_VID, "1")
                 if "1" == ver:
                     return MqUtils.__v1
```

### Comparing `folkmq-1.4.4/folkmq.egg-info/PKG-INFO` & `folkmq-1.4.5/folkmq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: folkmq
-Version: 1.4.4
+Version: 1.4.5
 Summary: @noear/folkmq python project
 Home-page: https://folkmq.noear.org/
 Author: noear
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.10
 Requires-Dist: loguru>=0.7.2
 Requires-Dist: websockets>=12.0
-Requires-Dist: socket.d>=2.4.16.1
+Requires-Dist: socket.d>=2.4.17
```

### Comparing `folkmq-1.4.4/folkmq.egg-info/SOURCES.txt` & `folkmq-1.4.5/folkmq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.4/setup.py` & `folkmq-1.4.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*_
 from setuptools import setup,find_packages
 
 setup(
     name='folkmq',
-    version='1.4.4',
+    version='1.4.5',
     description='@noear/folkmq python project',
     author='noear',
     url='https://folkmq.noear.org/',
     packages=find_packages(exclude=['*folkmq-test*']),   # 包内不需要引用的文件夹
     install_requires=[                          # 依赖包
         'loguru>=0.7.2',
         'websockets>=12.0',
-        'socket.d>=2.4.16.1'
+        'socket.d>=2.4.17'
     ],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
```

