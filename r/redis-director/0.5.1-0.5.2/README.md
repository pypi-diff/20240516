# Comparing `tmp/redis_director-0.5.1.tar.gz` & `tmp/redis_director-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_director-0.5.1.tar", max compression
+gzip compressed data, was "redis_director-0.5.2.tar", max compression
```

## Comparing `redis_director-0.5.1.tar` & `redis_director-0.5.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2024-05-16 07:13:28.480156 redis_director-0.5.1/README.md
--rw-r--r--   0        0        0      320 2024-05-16 07:46:55.926525 redis_director-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      131 2024-05-16 07:14:20.616944 redis_director-0.5.1/redis_director/__init__.py
--rw-r--r--   0        0        0      568 2024-05-16 07:42:23.997303 redis_director-0.5.1/redis_director/constants.py
--rw-r--r--   0        0        0      457 2024-05-16 07:36:15.466756 redis_director-0.5.1/redis_director/handler.py
--rw-r--r--   0        0        0     2342 2024-05-16 07:46:49.594320 redis_director-0.5.1/redis_director/publisher.py
--rw-r--r--   0        0        0     2427 2024-05-16 07:41:50.028080 redis_director-0.5.1/redis_director/subscriber.py
--rw-r--r--   0        0        0      583 1970-01-01 00:00:00.000000 redis_director-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     2114 2024-05-16 07:58:15.583107 redis_director-0.5.2/README.md
+-rw-r--r--   0        0        0      320 2024-05-16 07:58:23.375332 redis_director-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      131 2024-05-16 07:14:20.616944 redis_director-0.5.2/redis_director/__init__.py
+-rw-r--r--   0        0        0      568 2024-05-16 07:42:23.997303 redis_director-0.5.2/redis_director/constants.py
+-rw-r--r--   0        0        0      457 2024-05-16 07:36:15.466756 redis_director-0.5.2/redis_director/handler.py
+-rw-r--r--   0        0        0     2342 2024-05-16 07:46:49.594320 redis_director-0.5.2/redis_director/publisher.py
+-rw-r--r--   0        0        0     2427 2024-05-16 07:41:50.028080 redis_director-0.5.2/redis_director/subscriber.py
+-rw-r--r--   0        0        0     2697 1970-01-01 00:00:00.000000 redis_director-0.5.2/PKG-INFO
```

### Comparing `redis_director-0.5.1/redis_director/constants.py` & `redis_director-0.5.2/redis_director/constants.py`

 * *Files identical despite different names*

### Comparing `redis_director-0.5.1/redis_director/publisher.py` & `redis_director-0.5.2/redis_director/publisher.py`

 * *Files identical despite different names*

### Comparing `redis_director-0.5.1/redis_director/subscriber.py` & `redis_director-0.5.2/redis_director/subscriber.py`

 * *Files identical despite different names*

