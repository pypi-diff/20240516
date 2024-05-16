# Comparing `tmp/pyqi_api-1.0.0.tar.gz` & `tmp/pyqi_api-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqi_api-1.0.0.tar", last modified: Mon May 13 19:26:01 2024, max compression
+gzip compressed data, was "pyqi_api-1.0.1.tar", last modified: Wed May 15 11:00:58 2024, max compression
```

## Comparing `pyqi_api-1.0.0.tar` & `pyqi_api-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 19:26:01.612146 pyqi_api-1.0.0/
--rw-rw-rw-   0        0        0     3238 2024-05-13 16:50:43.000000 pyqi_api-1.0.0/.gitignore
--rw-rw-rw-   0        0        0    11558 2024-05-13 16:50:43.000000 pyqi_api-1.0.0/LICENSE.md
--rw-rw-rw-   0        0        0      552 2024-05-13 19:26:01.609084 pyqi_api-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      274 2024-05-13 16:50:43.000000 pyqi_api-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 19:26:01.579374 pyqi_api-1.0.0/pyQi/
--rw-rw-rw-   0        0        0      412 2024-05-13 19:23:32.000000 pyqi_api-1.0.0/pyQi/__init__.py
--rw-rw-rw-   0        0        0     9761 2024-05-13 16:50:43.000000 pyqi_api-1.0.0/pyQi/pyQi.py
--rw-rw-rw-   0        0        0    10952 2024-05-13 16:50:43.000000 pyqi_api-1.0.0/pyQi/pyQi_async.py
--rw-rw-rw-   0        0        0     3627 2024-05-13 16:50:43.000000 pyqi_api-1.0.0/pyQi/xltojson.py
--rw-rw-rw-   0        0        0      740 2024-05-13 19:21:42.000000 pyqi_api-1.0.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-13 19:26:01.609084 pyqi_api-1.0.0/pyqi_api.egg-info/
--rw-rw-rw-   0        0        0      552 2024-05-13 19:26:01.000000 pyqi_api-1.0.0/pyqi_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2024-05-13 19:26:01.000000 pyqi_api-1.0.0/pyqi_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 19:26:01.000000 pyqi_api-1.0.0/pyqi_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-13 19:26:01.000000 pyqi_api-1.0.0/pyqi_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 19:26:01.612146 pyqi_api-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-15 11:00:58.352117 pyqi_api-1.0.1/
+-rw-rw-rw-   0        0        0     3238 2024-05-13 16:50:43.000000 pyqi_api-1.0.1/.gitignore
+-rw-rw-rw-   0        0        0    11558 2024-05-13 16:50:43.000000 pyqi_api-1.0.1/LICENSE.md
+-rw-rw-rw-   0        0        0      552 2024-05-15 11:00:58.352117 pyqi_api-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2024-05-13 16:50:43.000000 pyqi_api-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 11:00:58.305125 pyqi_api-1.0.1/pyQi/
+-rw-rw-rw-   0        0        0      412 2024-05-13 19:23:32.000000 pyqi_api-1.0.1/pyQi/__init__.py
+-rw-rw-rw-   0        0        0     9761 2024-05-13 16:50:43.000000 pyqi_api-1.0.1/pyQi/pyQi_api.py
+-rw-rw-rw-   0        0        0    10952 2024-05-13 16:50:43.000000 pyqi_api-1.0.1/pyQi/pyQi_async.py
+-rw-rw-rw-   0        0        0     3627 2024-05-13 16:50:43.000000 pyqi_api-1.0.1/pyQi/xltojson.py
+-rw-rw-rw-   0        0        0      740 2024-05-15 10:59:39.000000 pyqi_api-1.0.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-15 11:00:58.352117 pyqi_api-1.0.1/pyqi_api.egg-info/
+-rw-rw-rw-   0        0        0      552 2024-05-15 11:00:57.000000 pyqi_api-1.0.1/pyqi_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2024-05-15 11:00:58.000000 pyqi_api-1.0.1/pyqi_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 11:00:57.000000 pyqi_api-1.0.1/pyqi_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-15 11:00:57.000000 pyqi_api-1.0.1/pyqi_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 11:00:58.352117 pyqi_api-1.0.1/setup.cfg
```

### Comparing `pyqi_api-1.0.0/.gitignore` & `pyqi_api-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyqi_api-1.0.0/LICENSE.md` & `pyqi_api-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyqi_api-1.0.0/PKG-INFO` & `pyqi_api-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqi_api
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python Module for QI Content and Collections Management System by Keepthinking
 Author-email: Christopher Prince <c.pj.prince@gmail.com>
 Project-URL: Homepage, https://github.com/CPJPRINCE/pyqi
 Project-URL: Issues, https://github.com/CPJPRINCE/pyqi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyqi_api-1.0.0/pyQi/pyQi.py` & `pyqi_api-1.0.1/pyQi/pyQi_api.py`

 * *Files identical despite different names*

### Comparing `pyqi_api-1.0.0/pyQi/pyQi_async.py` & `pyqi_api-1.0.1/pyQi/pyQi_async.py`

 * *Files identical despite different names*

### Comparing `pyqi_api-1.0.0/pyQi/xltojson.py` & `pyqi_api-1.0.1/pyQi/xltojson.py`

 * *Files identical despite different names*

### Comparing `pyqi_api-1.0.0/pyproject.toml` & `pyqi_api-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 00000020: 7570 746f 6f6c 7322 2c20 2273 6574 7570  uptools", "setup
 00000030: 746f 6f6c 732d 7363 6d22 5d0d 0a62 7569  tools-scm"]..bui
 00000040: 6c64 2d62 6163 6b65 6e64 203d 2022 7365  ld-backend = "se
 00000050: 7475 7074 6f6f 6c73 2e62 7569 6c64 5f6d  tuptools.build_m
 00000060: 6574 6122 0d0a 0d0a 5b70 726f 6a65 6374  eta"....[project
 00000070: 5d0d 0a6e 616d 6520 3d20 2270 7971 695f  ]..name = "pyqi_
 00000080: 6170 6922 0d0a 7665 7273 696f 6e20 3d20  api"..version = 
-00000090: 2231 2e30 2e30 220d 0a61 7574 686f 7273  "1.0.0"..authors
+00000090: 2231 2e30 2e31 220d 0a61 7574 686f 7273  "1.0.1"..authors
 000000a0: 203d 205b 0d0a 2020 2020 7b6e 616d 653d   = [..    {name=
 000000b0: 2243 6872 6973 746f 7068 6572 2050 7269  "Christopher Pri
 000000c0: 6e63 6522 2c20 656d 6169 6c3d 2263 2e70  nce", email="c.p
 000000d0: 6a2e 7072 696e 6365 4067 6d61 696c 2e63  j.prince@gmail.c
 000000e0: 6f6d 227d 0d0a 2020 2020 5d0d 0a64 6573  om"}..    ]..des
 000000f0: 6372 6970 7469 6f6e 203d 2022 5079 7468  cription = "Pyth
 00000100: 6f6e 204d 6f64 756c 6520 666f 7220 5149  on Module for QI
```

### Comparing `pyqi_api-1.0.0/pyqi_api.egg-info/PKG-INFO` & `pyqi_api-1.0.1/pyqi_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqi_api
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python Module for QI Content and Collections Management System by Keepthinking
 Author-email: Christopher Prince <c.pj.prince@gmail.com>
 Project-URL: Homepage, https://github.com/CPJPRINCE/pyqi
 Project-URL: Issues, https://github.com/CPJPRINCE/pyqi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

