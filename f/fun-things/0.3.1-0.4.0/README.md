# Comparing `tmp/fun_things-0.3.1.tar.gz` & `tmp/fun_things-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fun_things-0.3.1.tar", max compression
+gzip compressed data, was "fun_things-0.4.0.tar", max compression
```

## Comparing `fun_things-0.3.1.tar` & `fun_things-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0        0 2024-04-15 03:49:51.312592 fun_things-0.3.1/README.md
--rw-r--r--   0        0        0      108 2024-05-13 02:40:55.982879 fun_things-0.3.1/fun_things/__init__.py
--rw-r--r--   0        0        0      330 2024-04-30 06:36:45.297965 fun_things-0.3.1/fun_things/generic_json_encoder.py
--rw-r--r--   0        0        0     1268 2024-04-17 08:24:16.933684 fun_things-0.3.1/fun_things/lazy.py
--rw-r--r--   0        0        0     1193 2024-05-13 02:47:22.745222 fun_things-0.3.1/fun_things/proxy_uri.py
--rw-r--r--   0        0        0      277 2024-05-13 02:47:31.385193 fun_things-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 fun_things-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-15 03:49:51.312592 fun_things-0.4.0/README.md
+-rw-r--r--   0        0        0      170 2024-05-16 00:29:32.057244 fun_things-0.4.0/fun_things/__init__.py
+-rw-r--r--   0        0        0      330 2024-04-30 06:36:45.297965 fun_things-0.4.0/fun_things/generic_json_encoder.py
+-rw-r--r--   0        0        0     1268 2024-04-17 08:24:16.933684 fun_things-0.4.0/fun_things/lazy.py
+-rw-r--r--   0        0        0      935 2024-05-16 00:36:16.884375 fun_things-0.4.0/fun_things/math/weighted_distribution.py
+-rw-r--r--   0        0        0     1193 2024-05-13 02:47:22.745222 fun_things-0.4.0/fun_things/proxy_uri.py
+-rw-r--r--   0        0        0      277 2024-05-16 00:36:56.064455 fun_things-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 fun_things-0.4.0/PKG-INFO
```

### Comparing `fun_things-0.3.1/fun_things/lazy.py` & `fun_things-0.4.0/fun_things/lazy.py`

 * *Files identical despite different names*

### Comparing `fun_things-0.3.1/fun_things/proxy_uri.py` & `fun_things-0.4.0/fun_things/proxy_uri.py`

 * *Files identical despite different names*

