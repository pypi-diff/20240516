# Comparing `tmp/fun_things-0.5.0.tar.gz` & `tmp/fun_things-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fun_things-0.5.0.tar", max compression
+gzip compressed data, was "fun_things-0.5.1.tar", max compression
```

## Comparing `fun_things-0.5.0.tar` & `fun_things-0.5.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2024-04-15 03:49:51.312592 fun_things-0.5.0/README.md
--rw-r--r--   0        0        0      120 2024-05-16 00:42:36.895945 fun_things-0.5.0/fun_things/__init__.py
--rw-r--r--   0        0        0      330 2024-04-30 06:36:45.297965 fun_things-0.5.0/fun_things/generic_json_encoder.py
--rw-r--r--   0        0        0     1268 2024-04-17 08:24:16.933684 fun_things-0.5.0/fun_things/lazy.py
--rw-r--r--   0        0        0       57 2024-05-16 00:42:22.693915 fun_things-0.5.0/fun_things/math/__init__.py
--rw-r--r--   0        0        0     1048 2024-05-16 00:42:12.599276 fun_things-0.5.0/fun_things/math/weighted_distribution.py
--rw-r--r--   0        0        0     1193 2024-05-13 02:47:22.745222 fun_things-0.5.0/fun_things/proxy_uri.py
--rw-r--r--   0        0        0      277 2024-05-16 00:42:42.122014 fun_things-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 fun_things-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-15 03:49:51.312592 fun_things-0.5.1/README.md
+-rw-r--r--   0        0        0      120 2024-05-16 00:42:36.895945 fun_things-0.5.1/fun_things/__init__.py
+-rw-r--r--   0        0        0      330 2024-04-30 06:36:45.297965 fun_things-0.5.1/fun_things/generic_json_encoder.py
+-rw-r--r--   0        0        0     1268 2024-04-17 08:24:16.933684 fun_things-0.5.1/fun_things/lazy.py
+-rw-r--r--   0        0        0       57 2024-05-16 00:42:22.693915 fun_things-0.5.1/fun_things/math/__init__.py
+-rw-r--r--   0        0        0     1022 2024-05-16 00:44:10.180926 fun_things-0.5.1/fun_things/math/weighted_distribution.py
+-rw-r--r--   0        0        0     1193 2024-05-13 02:47:22.745222 fun_things-0.5.1/fun_things/proxy_uri.py
+-rw-r--r--   0        0        0      277 2024-05-16 00:44:18.859476 fun_things-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 fun_things-0.5.1/PKG-INFO
```

### Comparing `fun_things-0.5.0/fun_things/lazy.py` & `fun_things-0.5.1/fun_things/lazy.py`

 * *Files identical despite different names*

### Comparing `fun_things-0.5.0/fun_things/math/weighted_distribution.py` & `fun_things-0.5.1/fun_things/math/weighted_distribution.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,14 @@
         {
             "item": item,
             "weight": weight_selector(item),
         }
         for item in items
     ]
     weighted_items.sort(key=lambda item: item["weight"])
-    print(weighted_items)
 
     max_weight = reduce(
         lambda value, item: value + item["weight"],
         weighted_items,
         0,
     )
```

### Comparing `fun_things-0.5.0/fun_things/proxy_uri.py` & `fun_things-0.5.1/fun_things/proxy_uri.py`

 * *Files identical despite different names*

