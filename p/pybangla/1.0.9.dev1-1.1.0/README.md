# Comparing `tmp/pybangla-1.0.9.dev1.tar.gz` & `tmp/pybangla-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybangla-1.0.9.dev1.tar", last modified: Thu May 16 18:48:33 2024, max compression
+gzip compressed data, was "pybangla-1.1.0.tar", last modified: Thu May 16 18:52:07 2024, max compression
```

## Comparing `pybangla-1.0.9.dev1.tar` & `pybangla-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:48:33.663015 pybangla-1.0.9.dev1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:48:29.000000 pybangla-1.0.9.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    20323 2024-05-16 18:48:33.663015 pybangla-1.0.9.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19700 2024-05-16 18:48:29.000000 pybangla-1.0.9.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:48:33.659016 pybangla-1.0.9.dev1/pybangla/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-16 18:48:29.000000 pybangla-1.0.9.dev1/pybangla/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-16 18:48:29.000000 pybangla-1.0.9.dev1/pybangla/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:48:33.663015 pybangla-1.0.9.dev1/pybangla/module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:48:29.000000 pybangla-1.0.9.dev1/pybangla/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19949 2024-05-16 18:48:29.000000 pybangla-1.0.9.dev1/pybangla/module/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-05-16 18:48:29.000000 pybangla-1.0.9.dev1/pybangla/module/date_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-05-16 18:48:29.000000 pybangla-1.0.9.dev1/pybangla/module/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    17040 2024-05-16 18:48:29.000000 pybangla-1.0.9.dev1/pybangla/module/number_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    27661 2024-05-16 18:48:29.000000 pybangla-1.0.9.dev1/pybangla/module/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    22922 2024-05-16 18:48:29.000000 pybangla-1.0.9.dev1/pybangla/module/word_to_number.py
--rw-r--r--   0 runner    (1001) docker     (127)    17489 2024-05-16 18:48:29.000000 pybangla-1.0.9.dev1/pybangla/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:48:33.663015 pybangla-1.0.9.dev1/pybangla.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20323 2024-05-16 18:48:33.000000 pybangla-1.0.9.dev1/pybangla.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-16 18:48:33.000000 pybangla-1.0.9.dev1/pybangla.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:48:33.000000 pybangla-1.0.9.dev1/pybangla.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-16 18:48:33.000000 pybangla-1.0.9.dev1/pybangla.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-16 18:48:33.000000 pybangla-1.0.9.dev1/pybangla.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 18:48:33.663015 pybangla-1.0.9.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-16 18:48:29.000000 pybangla-1.0.9.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:48:33.663015 pybangla-1.0.9.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-05-16 18:48:29.000000 pybangla-1.0.9.dev1/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:52:07.635449 pybangla-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:52:03.000000 pybangla-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    20318 2024-05-16 18:52:07.635449 pybangla-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19700 2024-05-16 18:52:03.000000 pybangla-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:52:07.635449 pybangla-1.1.0/pybangla/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-16 18:52:03.000000 pybangla-1.1.0/pybangla/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-16 18:52:03.000000 pybangla-1.1.0/pybangla/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:52:07.635449 pybangla-1.1.0/pybangla/module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:52:03.000000 pybangla-1.1.0/pybangla/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19949 2024-05-16 18:52:03.000000 pybangla-1.1.0/pybangla/module/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-05-16 18:52:03.000000 pybangla-1.1.0/pybangla/module/date_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-05-16 18:52:03.000000 pybangla-1.1.0/pybangla/module/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17040 2024-05-16 18:52:03.000000 pybangla-1.1.0/pybangla/module/number_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27661 2024-05-16 18:52:03.000000 pybangla-1.1.0/pybangla/module/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22922 2024-05-16 18:52:03.000000 pybangla-1.1.0/pybangla/module/word_to_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17489 2024-05-16 18:52:03.000000 pybangla-1.1.0/pybangla/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:52:07.635449 pybangla-1.1.0/pybangla.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20318 2024-05-16 18:52:07.000000 pybangla-1.1.0/pybangla.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-16 18:52:07.000000 pybangla-1.1.0/pybangla.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:52:07.000000 pybangla-1.1.0/pybangla.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-16 18:52:07.000000 pybangla-1.1.0/pybangla.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-16 18:52:07.000000 pybangla-1.1.0/pybangla.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 18:52:07.639449 pybangla-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-16 18:52:03.000000 pybangla-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:52:07.635449 pybangla-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-05-16 18:52:03.000000 pybangla-1.1.0/tests/test.py
```

### Comparing `pybangla-1.0.9.dev1/PKG-INFO` & `pybangla-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybangla
-Version: 1.0.9.dev1
+Version: 1.1.0
 Summary: pybangla is the bangla text normalizer tool, it use for text normalization like word to number and date formating purposes
 Home-page: https://github.com/saiful9379/pybangla
 Author: saiful
 Author-email: saifulbrur79@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pybangla-1.0.9.dev1/README.md` & `pybangla-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pybangla-1.0.9.dev1/pybangla/matching.py` & `pybangla-1.1.0/pybangla/matching.py`

 * *Files identical despite different names*

### Comparing `pybangla-1.0.9.dev1/pybangla/module/config.py` & `pybangla-1.1.0/pybangla/module/config.py`

 * *Files identical despite different names*

### Comparing `pybangla-1.0.9.dev1/pybangla/module/date_extractor.py` & `pybangla-1.1.0/pybangla/module/date_extractor.py`

 * *Files identical despite different names*

### Comparing `pybangla-1.0.9.dev1/pybangla/module/main.py` & `pybangla-1.1.0/pybangla/module/main.py`

 * *Files identical despite different names*

### Comparing `pybangla-1.0.9.dev1/pybangla/module/number_parser.py` & `pybangla-1.1.0/pybangla/module/number_parser.py`

 * *Files identical despite different names*

### Comparing `pybangla-1.0.9.dev1/pybangla/module/parser.py` & `pybangla-1.1.0/pybangla/module/parser.py`

 * *Files identical despite different names*

### Comparing `pybangla-1.0.9.dev1/pybangla/module/word_to_number.py` & `pybangla-1.1.0/pybangla/module/word_to_number.py`

 * *Files identical despite different names*

### Comparing `pybangla-1.0.9.dev1/pybangla/test.py` & `pybangla-1.1.0/pybangla/test.py`

 * *Files identical despite different names*

### Comparing `pybangla-1.0.9.dev1/pybangla.egg-info/PKG-INFO` & `pybangla-1.1.0/pybangla.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybangla
-Version: 1.0.9.dev1
+Version: 1.1.0
 Summary: pybangla is the bangla text normalizer tool, it use for text normalization like word to number and date formating purposes
 Home-page: https://github.com/saiful9379/pybangla
 Author: saiful
 Author-email: saifulbrur79@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pybangla-1.0.9.dev1/setup.py` & `pybangla-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import codecs
 from setuptools import setup, find_packages
 
 setup(
     name='pybangla',
-    version='1.0.9-dev1',
+    version='1.1.0',
     packages=find_packages(),
     # entry_points={
     #     'console_scripts': [
     #         'pybangla = pybangla.main:Normalizer'
     #     ]
     # },
     author='saiful',
```

### Comparing `pybangla-1.0.9.dev1/tests/test.py` & `pybangla-1.1.0/tests/test.py`

 * *Files identical despite different names*

