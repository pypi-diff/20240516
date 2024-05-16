# Comparing `tmp/redis_director-0.3.0.tar.gz` & `tmp/redis_director-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_director-0.3.0.tar", max compression
+gzip compressed data, was "redis_director-0.4.0.tar", max compression
```

## Comparing `redis_director-0.3.0.tar` & `redis_director-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2024-05-16 07:13:28.480156 redis_director-0.3.0/README.md
--rw-r--r--   0        0        0      320 2024-05-16 07:36:48.424197 redis_director-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      131 2024-05-16 07:14:20.616944 redis_director-0.3.0/redis_director/__init__.py
--rw-r--r--   0        0        0      487 2024-05-16 07:30:43.675914 redis_director-0.3.0/redis_director/constants.py
--rw-r--r--   0        0        0      457 2024-05-16 07:36:15.466756 redis_director-0.3.0/redis_director/handler.py
--rw-r--r--   0        0        0     2061 2024-05-16 07:32:12.354873 redis_director-0.3.0/redis_director/publisher.py
--rw-r--r--   0        0        0     2247 2024-05-16 07:33:07.949815 redis_director-0.3.0/redis_director/subscriber.py
--rw-r--r--   0        0        0      583 1970-01-01 00:00:00.000000 redis_director-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-16 07:13:28.480156 redis_director-0.4.0/README.md
+-rw-r--r--   0        0        0      320 2024-05-16 07:42:43.914011 redis_director-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      131 2024-05-16 07:14:20.616944 redis_director-0.4.0/redis_director/__init__.py
+-rw-r--r--   0        0        0      568 2024-05-16 07:42:23.997303 redis_director-0.4.0/redis_director/constants.py
+-rw-r--r--   0        0        0      457 2024-05-16 07:36:15.466756 redis_director-0.4.0/redis_director/handler.py
+-rw-r--r--   0        0        0     2061 2024-05-16 07:32:12.354873 redis_director-0.4.0/redis_director/publisher.py
+-rw-r--r--   0        0        0     2427 2024-05-16 07:41:50.028080 redis_director-0.4.0/redis_director/subscriber.py
+-rw-r--r--   0        0        0      583 1970-01-01 00:00:00.000000 redis_director-0.4.0/PKG-INFO
```

### Comparing `redis_director-0.3.0/redis_director/publisher.py` & `redis_director-0.4.0/redis_director/publisher.py`

 * *Files identical despite different names*

### Comparing `redis_director-0.3.0/redis_director/subscriber.py` & `redis_director-0.4.0/redis_director/subscriber.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,33 +16,40 @@
     """
     default_score: float
     """
     The default score.
     """
     min_score: float
     """
+    The minimum score.
+    """
+    max_score: float
+    """
+    The maximum score.
     """
     handler: Callable[["Subscriber", Any], None]  # type: ignore
     increment_script: Script
 
     @staticmethod
     def new(
         redis: Redis,
         score_key: str = None,  # type: ignore
         score_member: str = None,  # type: ignore
         default_score: float = 0,
         min_score: float = 1,
+        max_score: float = 100,
         handler: Callable[["Subscriber", Any], None] = None,  # type: ignore
     ):
         return Subscriber(
             redis=redis,
             score_key=score_key,
             score_member=score_member,
             default_score=default_score,
             min_score=min_score,
+            max_score=max_score,
             handler=handler,
             increment_script=redis.register_script(
                 INCREMENT_LUA_SCRIPT,
             ),  # type: ignore
         )
 
     @property
@@ -69,14 +76,15 @@
         return self.increment_script(
             (self.score_key,),
             (
                 self.score_member,
                 value,
                 self.default_score,
                 self.min_score,
+                self.max_score,
             ),
         )
 
     def set_score(self, value: float):
         self.redis.zadd(
             self.score_key,
             {
```

### Comparing `redis_director-0.3.0/PKG-INFO` & `redis_director-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-director
-Version: 0.3.0
+Version: 0.4.0
 Summary: 
 Author: MisterNyan
 Author-email: michael.edmund.wong@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

