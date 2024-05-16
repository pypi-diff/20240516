# Comparing `tmp/tqdm_multiprocessing-0.1.1.tar.gz` & `tmp/tqdm_multiprocessing-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tqdm_multiprocessing-0.1.1.tar", last modified: Thu May 16 16:05:55 2024, max compression
+gzip compressed data, was "tqdm_multiprocessing-0.1.2.tar", last modified: Thu May 16 16:26:26 2024, max compression
```

## Comparing `tqdm_multiprocessing-0.1.1.tar` & `tqdm_multiprocessing-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxr-x   0 tim       (1001) tim       (1001)        0 2024-05-16 16:05:55.933450 tqdm_multiprocessing-0.1.1/
--rw-rw-r--   0 tim       (1001) tim       (1001)    11357 2024-03-03 15:31:53.000000 tqdm_multiprocessing-0.1.1/LICENSE
--rw-r--r--   0 tim       (1001) tim       (1001)      744 2024-05-16 16:05:55.933450 tqdm_multiprocessing-0.1.1/PKG-INFO
--rw-rw-r--   0 tim       (1001) tim       (1001)      410 2024-03-03 15:31:53.000000 tqdm_multiprocessing-0.1.1/README.md
--rw-rw-r--   0 tim       (1001) tim       (1001)      542 2024-05-16 15:59:37.000000 tqdm_multiprocessing-0.1.1/pyproject.toml
--rw-rw-r--   0 tim       (1001) tim       (1001)      480 2024-05-16 16:05:55.933450 tqdm_multiprocessing-0.1.1/setup.cfg
--rw-rw-r--   0 tim       (1001) tim       (1001)      116 2024-03-03 15:31:53.000000 tqdm_multiprocessing-0.1.1/setup.py
-drwxrwxr-x   0 tim       (1001) tim       (1001)        0 2024-05-16 16:05:55.929450 tqdm_multiprocessing-0.1.1/tests/
--rw-rw-r--   0 tim       (1001) tim       (1001)     4774 2024-03-03 15:31:53.000000 tqdm_multiprocessing-0.1.1/tests/test_mapper.py
-drwxrwxr-x   0 tim       (1001) tim       (1001)        0 2024-05-16 16:05:55.929450 tqdm_multiprocessing-0.1.1/tqdm_multiprocessing/
--rw-rw-r--   0 tim       (1001) tim       (1001)      208 2024-03-03 15:31:53.000000 tqdm_multiprocessing-0.1.1/tqdm_multiprocessing/__init__.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     8820 2024-05-16 15:54:42.000000 tqdm_multiprocessing-0.1.1/tqdm_multiprocessing/mapper.py
--rw-rw-r--   0 tim       (1001) tim       (1001)       22 2024-03-04 07:10:35.000000 tqdm_multiprocessing-0.1.1/tqdm_multiprocessing/version.py
-drwxrwxr-x   0 tim       (1001) tim       (1001)        0 2024-05-16 16:05:55.929450 tqdm_multiprocessing-0.1.1/tqdm_multiprocessing.egg-info/
--rw-r--r--   0 tim       (1001) tim       (1001)      744 2024-05-16 16:05:55.000000 tqdm_multiprocessing-0.1.1/tqdm_multiprocessing.egg-info/PKG-INFO
--rw-rw-r--   0 tim       (1001) tim       (1001)      387 2024-05-16 16:05:55.000000 tqdm_multiprocessing-0.1.1/tqdm_multiprocessing.egg-info/SOURCES.txt
--rw-rw-r--   0 tim       (1001) tim       (1001)        1 2024-05-16 16:05:55.000000 tqdm_multiprocessing-0.1.1/tqdm_multiprocessing.egg-info/dependency_links.txt
--rw-rw-r--   0 tim       (1001) tim       (1001)      121 2024-05-16 16:05:55.000000 tqdm_multiprocessing-0.1.1/tqdm_multiprocessing.egg-info/requires.txt
--rw-rw-r--   0 tim       (1001) tim       (1001)       21 2024-05-16 16:05:55.000000 tqdm_multiprocessing-0.1.1/tqdm_multiprocessing.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 16:26:26.103662 tqdm_multiprocessing-0.1.2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2024-05-16 16:25:10.000000 tqdm_multiprocessing-0.1.2/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      744 2024-05-16 16:26:26.103662 tqdm_multiprocessing-0.1.2/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      410 2024-05-16 16:25:10.000000 tqdm_multiprocessing-0.1.2/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      542 2024-05-16 16:25:10.000000 tqdm_multiprocessing-0.1.2/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      480 2024-05-16 16:26:26.103662 tqdm_multiprocessing-0.1.2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      116 2024-05-16 16:25:10.000000 tqdm_multiprocessing-0.1.2/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 16:26:26.099662 tqdm_multiprocessing-0.1.2/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4774 2024-05-16 16:25:10.000000 tqdm_multiprocessing-0.1.2/tests/test_mapper.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 16:26:26.099662 tqdm_multiprocessing-0.1.2/tqdm_multiprocessing/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      208 2024-05-16 16:25:10.000000 tqdm_multiprocessing-0.1.2/tqdm_multiprocessing/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8820 2024-05-16 16:25:10.000000 tqdm_multiprocessing-0.1.2/tqdm_multiprocessing/mapper.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 16:26:26.099662 tqdm_multiprocessing-0.1.2/tqdm_multiprocessing.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      744 2024-05-16 16:26:26.000000 tqdm_multiprocessing-0.1.2/tqdm_multiprocessing.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      355 2024-05-16 16:26:26.000000 tqdm_multiprocessing-0.1.2/tqdm_multiprocessing.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-16 16:26:26.000000 tqdm_multiprocessing-0.1.2/tqdm_multiprocessing.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      121 2024-05-16 16:26:26.000000 tqdm_multiprocessing-0.1.2/tqdm_multiprocessing.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2024-05-16 16:26:26.000000 tqdm_multiprocessing-0.1.2/tqdm_multiprocessing.egg-info/top_level.txt
```

### Comparing `tqdm_multiprocessing-0.1.1/LICENSE` & `tqdm_multiprocessing-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tqdm_multiprocessing-0.1.1/PKG-INFO` & `tqdm_multiprocessing-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tqdm_multiprocessing
-Version: 0.1.1
+Version: 0.1.2
 Home-page: https://github.com/medcognetics/tqdm-multiprocessing
 Author: Scott Chase Waggener
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: tqdm
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
```

### Comparing `tqdm_multiprocessing-0.1.1/pyproject.toml` & `tqdm_multiprocessing-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tqdm_multiprocessing-0.1.1/tests/test_mapper.py` & `tqdm_multiprocessing-0.1.2/tests/test_mapper.py`

 * *Files identical despite different names*

### Comparing `tqdm_multiprocessing-0.1.1/tqdm_multiprocessing/mapper.py` & `tqdm_multiprocessing-0.1.2/tqdm_multiprocessing/mapper.py`

 * *Files identical despite different names*

### Comparing `tqdm_multiprocessing-0.1.1/tqdm_multiprocessing.egg-info/PKG-INFO` & `tqdm_multiprocessing-0.1.2/tqdm_multiprocessing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tqdm_multiprocessing
-Version: 0.1.1
+Version: 0.1.2
 Home-page: https://github.com/medcognetics/tqdm-multiprocessing
 Author: Scott Chase Waggener
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: tqdm
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
```

