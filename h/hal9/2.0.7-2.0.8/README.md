# Comparing `tmp/hal9-2.0.7.tar.gz` & `tmp/hal9-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hal9-2.0.7.tar", max compression
+gzip compressed data, was "hal9-2.0.8.tar", max compression
```

## Comparing `hal9-2.0.7.tar` & `hal9-2.0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     2951 2024-05-15 22:12:07.073053 hal9-2.0.7/README.md
--rw-r--r--   0        0        0       86 2024-05-15 22:12:07.005053 hal9-2.0.7/hal9/__init__.py
--rw-r--r--   0        0        0     1220 2024-05-15 22:12:07.005053 hal9-2.0.7/hal9/cli.py
--rw-r--r--   0        0        0      634 2024-05-15 22:12:07.005053 hal9-2.0.7/hal9/create.py
--rw-r--r--   0        0        0      574 2024-05-15 22:12:07.005053 hal9-2.0.7/hal9/deploy.py
--rw-r--r--   0        0        0      531 2024-05-15 22:12:07.005053 hal9-2.0.7/hal9/run.py
--rw-r--r--   0        0        0      352 2024-05-15 22:12:07.005053 hal9-2.0.7/hal9/targets/docker.py
--rw-r--r--   0        0        0     2061 2024-05-15 22:12:07.005053 hal9-2.0.7/hal9/targets/hal9.py
--rw-r--r--   0        0        0       42 2024-05-15 22:12:07.005053 hal9-2.0.7/hal9/templates/docker/Dockerfile
--rw-r--r--   0        0        0       70 2024-05-15 22:12:07.005053 hal9-2.0.7/hal9/templates/openai/app.py
--rw-r--r--   0        0        0      434 2024-05-15 22:12:07.005053 hal9-2.0.7/pyproject.toml
--rw-r--r--   0        0        0     3589 1970-01-01 00:00:00.000000 hal9-2.0.7/PKG-INFO
+-rw-r--r--   0        0        0     2951 2024-05-15 22:21:29.132043 hal9-2.0.8/README.md
+-rw-r--r--   0        0        0       86 2024-05-15 22:21:29.064042 hal9-2.0.8/hal9/__init__.py
+-rw-r--r--   0        0        0     1220 2024-05-15 22:21:29.064042 hal9-2.0.8/hal9/cli.py
+-rw-r--r--   0        0        0      634 2024-05-15 22:21:29.064042 hal9-2.0.8/hal9/create.py
+-rw-r--r--   0        0        0      574 2024-05-15 22:21:29.064042 hal9-2.0.8/hal9/deploy.py
+-rw-r--r--   0        0        0      531 2024-05-15 22:21:29.064042 hal9-2.0.8/hal9/run.py
+-rw-r--r--   0        0        0      352 2024-05-15 22:21:29.064042 hal9-2.0.8/hal9/targets/docker.py
+-rw-r--r--   0        0        0     2061 2024-05-15 22:21:29.064042 hal9-2.0.8/hal9/targets/hal9.py
+-rw-r--r--   0        0        0       42 2024-05-15 22:21:29.064042 hal9-2.0.8/hal9/templates/docker/Dockerfile
+-rw-r--r--   0        0        0       70 2024-05-15 22:21:29.064042 hal9-2.0.8/hal9/templates/openai/app.py
+-rw-r--r--   0        0        0      434 2024-05-15 22:21:29.064042 hal9-2.0.8/pyproject.toml
+-rw-r--r--   0        0        0     3589 1970-01-01 00:00:00.000000 hal9-2.0.8/PKG-INFO
```

### Comparing `hal9-2.0.7/README.md` & `hal9-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `hal9-2.0.7/hal9/cli.py` & `hal9-2.0.8/hal9/cli.py`

 * *Files identical despite different names*

### Comparing `hal9-2.0.7/hal9/create.py` & `hal9-2.0.8/hal9/create.py`

 * *Files identical despite different names*

### Comparing `hal9-2.0.7/hal9/deploy.py` & `hal9-2.0.8/hal9/deploy.py`

 * *Files identical despite different names*

### Comparing `hal9-2.0.7/hal9/run.py` & `hal9-2.0.8/hal9/run.py`

 * *Files identical despite different names*

### Comparing `hal9-2.0.7/hal9/targets/hal9.py` & `hal9-2.0.8/hal9/targets/hal9.py`

 * *Files identical despite different names*

### Comparing `hal9-2.0.7/PKG-INFO` & `hal9-2.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hal9
-Version: 2.0.7
+Version: 2.0.8
 Summary: 
 Author: Javier Luraschi
 Author-email: javier@hal9.ai
 Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

