# Comparing `tmp/xingu-1.7.1.tar.gz` & `tmp/xingu-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xingu-1.7.1.tar", last modified: Fri May 10 13:22:03 2024, max compression
+gzip compressed data, was "xingu-1.7.2.tar", last modified: Thu May 16 01:22:08 2024, max compression
```

## Comparing `xingu-1.7.1.tar` & `xingu-1.7.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-05-10 13:22:03.640466 xingu-1.7.1/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7652 2024-01-03 19:20:34.000000 xingu-1.7.1/LICENSE
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    21761 2024-05-10 13:22:03.640466 xingu-1.7.1/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11571 2024-01-10 19:09:00.000000 xingu-1.7.1/README.md
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1277 2024-05-10 13:21:14.000000 xingu-1.7.1/pyproject.toml
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2024-05-10 13:22:03.640466 xingu-1.7.1/setup.cfg
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-05-10 13:22:03.636466 xingu-1.7.1/xingu/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      434 2024-01-24 19:13:14.000000 xingu-1.7.1/xingu/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    19409 2024-05-09 20:29:57.000000 xingu-1.7.1/xingu/__main__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    50497 2024-05-10 13:13:55.000000 xingu-1.7.1/xingu/coach.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7378 2024-01-03 19:20:34.000000 xingu-1.7.1/xingu/config_manager.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    22328 2024-05-09 20:54:52.000000 xingu-1.7.1/xingu/dataprovider.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     5498 2024-01-03 19:20:34.000000 xingu-1.7.1/xingu/dataproviderfactory.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2523 2024-05-09 20:50:35.000000 xingu-1.7.1/xingu/estimator.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-05-10 13:22:03.636466 xingu-1.7.1/xingu/estimators/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    12628 2024-01-03 19:20:34.000000 xingu-1.7.1/xingu/estimators/catboost.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)   101862 2024-05-10 13:13:05.000000 xingu-1.7.1/xingu/model.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-05-10 13:22:03.636466 xingu-1.7.1/xingu.egg-info/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    21761 2024-05-10 13:22:03.000000 xingu-1.7.1/xingu.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      397 2024-05-10 13:22:03.000000 xingu-1.7.1/xingu.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2024-05-10 13:22:03.000000 xingu-1.7.1/xingu.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       46 2024-05-10 13:22:03.000000 xingu-1.7.1/xingu.egg-info/entry_points.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      115 2024-05-10 13:22:03.000000 xingu-1.7.1/xingu.egg-info/requires.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        6 2024-05-10 13:22:03.000000 xingu-1.7.1/xingu.egg-info/top_level.txt
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-05-16 01:22:08.088120 xingu-1.7.2/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7652 2024-01-03 19:20:34.000000 xingu-1.7.2/LICENSE
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    21761 2024-05-16 01:22:08.088120 xingu-1.7.2/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11571 2024-01-10 19:09:00.000000 xingu-1.7.2/README.md
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1277 2024-05-16 01:21:25.000000 xingu-1.7.2/pyproject.toml
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2024-05-16 01:22:08.088120 xingu-1.7.2/setup.cfg
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-05-16 01:22:08.088120 xingu-1.7.2/xingu/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      434 2024-01-24 19:13:14.000000 xingu-1.7.2/xingu/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    19715 2024-05-16 01:21:08.000000 xingu-1.7.2/xingu/__main__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    50497 2024-05-10 13:13:55.000000 xingu-1.7.2/xingu/coach.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7378 2024-01-03 19:20:34.000000 xingu-1.7.2/xingu/config_manager.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    22328 2024-05-09 20:54:52.000000 xingu-1.7.2/xingu/dataprovider.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     5498 2024-01-03 19:20:34.000000 xingu-1.7.2/xingu/dataproviderfactory.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2523 2024-05-09 20:50:35.000000 xingu-1.7.2/xingu/estimator.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-05-16 01:22:08.088120 xingu-1.7.2/xingu/estimators/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    12628 2024-01-03 19:20:34.000000 xingu-1.7.2/xingu/estimators/catboost.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)   101862 2024-05-16 01:14:37.000000 xingu-1.7.2/xingu/model.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-05-16 01:22:08.088120 xingu-1.7.2/xingu.egg-info/
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    21761 2024-05-16 01:22:08.000000 xingu-1.7.2/xingu.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      397 2024-05-16 01:22:08.000000 xingu-1.7.2/xingu.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2024-05-16 01:22:08.000000 xingu-1.7.2/xingu.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       46 2024-05-16 01:22:08.000000 xingu-1.7.2/xingu.egg-info/entry_points.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      115 2024-05-16 01:22:08.000000 xingu-1.7.2/xingu.egg-info/requires.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        6 2024-05-16 01:22:08.000000 xingu-1.7.2/xingu.egg-info/top_level.txt
```

### Comparing `xingu-1.7.1/LICENSE` & `xingu-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xingu-1.7.1/PKG-INFO` & `xingu-1.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xingu
-Version: 1.7.1
+Version: 1.7.2
 Summary: Automated ML model training and packaging
 Author-email: Avi Alkalay <avi@unix.sh>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `xingu-1.7.1/README.md` & `xingu-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `xingu-1.7.1/pyproject.toml` & `xingu-1.7.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xingu"
-version = '1.7.1'
+version = '1.7.2'
 description = "Automated ML model training and packaging"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
 authors = [
     { name = "Avi Alkalay", email = "avi@unix.sh" },
 ]
```

### Comparing `xingu-1.7.1/xingu/__main__.py` & `xingu-1.7.2/xingu/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,27 @@
     HANDLER = logging.StreamHandler()
     HANDLER.setFormatter(FORMATTER)
 
     logger = logging.getLogger()
     logger.addHandler(HANDLER)
     logger.setLevel(level)
 
+    # Suppress well known very annoying modules
+    annoying="""
+        aiobotocore
+        boto3
+        botocore
+        s3fs
+        fsspec
+    """.split()
+
+    for stop_annoying in annoying:
+        annoying_logger = logging.getLogger(stop_annoying)
+        annoying_logger.setLevel(logging.WARNING)
+
     return logger
 
 
 
 
 def prepare_logging_OLD(level=logging.INFO):
     # Switch between INFO/DEBUG while running in production/developping:
```

### Comparing `xingu-1.7.1/xingu/coach.py` & `xingu-1.7.2/xingu/coach.py`

 * *Files identical despite different names*

### Comparing `xingu-1.7.1/xingu/config_manager.py` & `xingu-1.7.2/xingu/config_manager.py`

 * *Files identical despite different names*

### Comparing `xingu-1.7.1/xingu/dataprovider.py` & `xingu-1.7.2/xingu/dataprovider.py`

 * *Files identical despite different names*

### Comparing `xingu-1.7.1/xingu/dataproviderfactory.py` & `xingu-1.7.2/xingu/dataproviderfactory.py`

 * *Files identical despite different names*

### Comparing `xingu-1.7.1/xingu/estimator.py` & `xingu-1.7.2/xingu/estimator.py`

 * *Files identical despite different names*

### Comparing `xingu-1.7.1/xingu/estimators/catboost.py` & `xingu-1.7.2/xingu/estimators/catboost.py`

 * *Files identical despite different names*

### Comparing `xingu-1.7.1/xingu/model.py` & `xingu-1.7.2/xingu/model.py`

 * *Files identical despite different names*

### Comparing `xingu-1.7.1/xingu.egg-info/PKG-INFO` & `xingu-1.7.2/xingu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xingu
-Version: 1.7.1
+Version: 1.7.2
 Summary: Automated ML model training and packaging
 Author-email: Avi Alkalay <avi@unix.sh>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

