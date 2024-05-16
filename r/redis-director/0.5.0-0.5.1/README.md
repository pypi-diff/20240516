# Comparing `tmp/redis_director-0.5.0.tar.gz` & `tmp/redis_director-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_director-0.5.0.tar", max compression
+gzip compressed data, was "redis_director-0.5.1.tar", max compression
```

## Comparing `redis_director-0.5.0.tar` & `redis_director-0.5.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2024-05-16 07:13:28.480156 redis_director-0.5.0/README.md
--rw-r--r--   0        0        0      320 2024-05-16 07:45:36.499921 redis_director-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      131 2024-05-16 07:14:20.616944 redis_director-0.5.0/redis_director/__init__.py
--rw-r--r--   0        0        0      568 2024-05-16 07:42:23.997303 redis_director-0.5.0/redis_director/constants.py
--rw-r--r--   0        0        0      457 2024-05-16 07:36:15.466756 redis_director-0.5.0/redis_director/handler.py
--rw-r--r--   0        0        0     2295 2024-05-16 07:45:31.223746 redis_director-0.5.0/redis_director/publisher.py
--rw-r--r--   0        0        0     2427 2024-05-16 07:41:50.028080 redis_director-0.5.0/redis_director/subscriber.py
--rw-r--r--   0        0        0      583 1970-01-01 00:00:00.000000 redis_director-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-16 07:13:28.480156 redis_director-0.5.1/README.md
+-rw-r--r--   0        0        0      320 2024-05-16 07:46:55.926525 redis_director-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      131 2024-05-16 07:14:20.616944 redis_director-0.5.1/redis_director/__init__.py
+-rw-r--r--   0        0        0      568 2024-05-16 07:42:23.997303 redis_director-0.5.1/redis_director/constants.py
+-rw-r--r--   0        0        0      457 2024-05-16 07:36:15.466756 redis_director-0.5.1/redis_director/handler.py
+-rw-r--r--   0        0        0     2342 2024-05-16 07:46:49.594320 redis_director-0.5.1/redis_director/publisher.py
+-rw-r--r--   0        0        0     2427 2024-05-16 07:41:50.028080 redis_director-0.5.1/redis_director/subscriber.py
+-rw-r--r--   0        0        0      583 1970-01-01 00:00:00.000000 redis_director-0.5.1/PKG-INFO
```

### Comparing `redis_director-0.5.0/redis_director/constants.py` & `redis_director-0.5.1/redis_director/constants.py`

 * *Files identical despite different names*

### Comparing `redis_director-0.5.0/redis_director/publisher.py` & `redis_director-0.5.1/redis_director/publisher.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,28 +38,29 @@
         self,
         score_member: str,
         handler: Callable[[Subscriber, Any], None],
         default_score: float = 100,
         min_score: float = 1,
         max_score: float = 100,
     ):
-        return self.add_subscriber(
+        return self.add_subscribers(
             Subscriber.new(
                 redis=self.__redis,
                 score_key=self.__score_key,
                 score_member=score_member,
                 default_score=default_score,
                 min_score=min_score,
                 max_score=max_score,
                 handler=handler,
             )
         )
 
-    def add_subscriber(self, subscriber: Subscriber):
-        self.__subscribers[subscriber.score_member] = subscriber
+    def add_subscribers(self, *subscribers: Subscriber):
+        for subscriber in subscribers:
+            self.__subscribers[subscriber.score_member] = subscriber
 
         return self
 
     def get_subscriber(self, member: str) -> Subscriber:
         if member not in self.__subscribers:
             return None  # type: ignore
```

### Comparing `redis_director-0.5.0/redis_director/subscriber.py` & `redis_director-0.5.1/redis_director/subscriber.py`

 * *Files identical despite different names*

### Comparing `redis_director-0.5.0/PKG-INFO` & `redis_director-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-director
-Version: 0.5.0
+Version: 0.5.1
 Summary: 
 Author: MisterNyan
 Author-email: michael.edmund.wong@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

