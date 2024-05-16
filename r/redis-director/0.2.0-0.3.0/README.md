# Comparing `tmp/redis_director-0.2.0.tar.gz` & `tmp/redis_director-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_director-0.2.0.tar", max compression
+gzip compressed data, was "redis_director-0.3.0.tar", max compression
```

## Comparing `redis_director-0.2.0.tar` & `redis_director-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2024-05-16 07:13:28.480156 redis_director-0.2.0/README.md
--rw-r--r--   0        0        0      320 2024-05-16 07:33:04.865656 redis_director-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      131 2024-05-16 07:14:20.616944 redis_director-0.2.0/redis_director/__init__.py
--rw-r--r--   0        0        0      487 2024-05-16 07:30:43.675914 redis_director-0.2.0/redis_director/constants.py
--rw-r--r--   0        0        0      319 2024-05-16 07:32:28.239730 redis_director-0.2.0/redis_director/handler.py
--rw-r--r--   0        0        0     2061 2024-05-16 07:32:12.354873 redis_director-0.2.0/redis_director/publisher.py
--rw-r--r--   0        0        0     2247 2024-05-16 07:33:07.949815 redis_director-0.2.0/redis_director/subscriber.py
--rw-r--r--   0        0        0      583 1970-01-01 00:00:00.000000 redis_director-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-16 07:13:28.480156 redis_director-0.3.0/README.md
+-rw-r--r--   0        0        0      320 2024-05-16 07:36:48.424197 redis_director-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      131 2024-05-16 07:14:20.616944 redis_director-0.3.0/redis_director/__init__.py
+-rw-r--r--   0        0        0      487 2024-05-16 07:30:43.675914 redis_director-0.3.0/redis_director/constants.py
+-rw-r--r--   0        0        0      457 2024-05-16 07:36:15.466756 redis_director-0.3.0/redis_director/handler.py
+-rw-r--r--   0        0        0     2061 2024-05-16 07:32:12.354873 redis_director-0.3.0/redis_director/publisher.py
+-rw-r--r--   0        0        0     2247 2024-05-16 07:33:07.949815 redis_director-0.3.0/redis_director/subscriber.py
+-rw-r--r--   0        0        0      583 1970-01-01 00:00:00.000000 redis_director-0.3.0/PKG-INFO
```

### Comparing `redis_director-0.2.0/redis_director/publisher.py` & `redis_director-0.3.0/redis_director/publisher.py`

 * *Files identical despite different names*

### Comparing `redis_director-0.2.0/redis_director/subscriber.py` & `redis_director-0.3.0/redis_director/subscriber.py`

 * *Files identical despite different names*

### Comparing `redis_director-0.2.0/PKG-INFO` & `redis_director-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-director
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 Author: MisterNyan
 Author-email: michael.edmund.wong@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

