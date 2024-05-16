# Comparing `tmp/dagster-openai-0.23.5.tar.gz` & `tmp/dagster-openai-0.23.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-openai-0.23.5.tar", last modified: Thu May  9 17:57:26 2024, max compression
+gzip compressed data, was "dagster-openai-0.23.6.tar", last modified: Thu May 16 20:13:53 2024, max compression
```

## Comparing `dagster-openai-0.23.5.tar` & `dagster-openai-0.23.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:57:26.748161 dagster-openai-0.23.5/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-05-09 17:47:35.000000 dagster-openai-0.23.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       66 2024-05-09 17:47:35.000000 dagster-openai-0.23.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      640 2024-05-09 17:57:26.748161 dagster-openai-0.23.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      128 2024-05-09 17:47:35.000000 dagster-openai-0.23.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:57:26.748161 dagster-openai-0.23.5/dagster_openai/
--rw-r--r--   0 root         (0) root         (0)      270 2024-05-09 17:47:35.000000 dagster-openai-0.23.5/dagster_openai/__init__.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-09 17:47:35.000000 dagster-openai-0.23.5/dagster_openai/py.typed
--rw-r--r--   0 root         (0) root         (0)    15015 2024-05-09 17:47:35.000000 dagster-openai-0.23.5/dagster_openai/resources.py
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-09 17:47:35.000000 dagster-openai-0.23.5/dagster_openai/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:57:26.748161 dagster-openai-0.23.5/dagster_openai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      640 2024-05-09 17:57:26.000000 dagster-openai-0.23.5/dagster_openai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      379 2024-05-09 17:57:26.000000 dagster-openai-0.23.5/dagster_openai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 17:57:26.000000 dagster-openai-0.23.5/dagster_openai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 17:57:26.000000 dagster-openai-0.23.5/dagster_openai.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 17:57:26.000000 dagster-openai-0.23.5/dagster_openai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-05-09 17:57:26.000000 dagster-openai-0.23.5/dagster_openai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      161 2024-05-09 17:57:26.748161 dagster-openai-0.23.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1207 2024-05-09 17:47:35.000000 dagster-openai-0.23.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:13:53.328116 dagster-openai-0.23.6/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-05-16 20:06:23.000000 dagster-openai-0.23.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       66 2024-05-16 20:06:23.000000 dagster-openai-0.23.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      640 2024-05-16 20:13:53.328116 dagster-openai-0.23.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      128 2024-05-16 20:06:23.000000 dagster-openai-0.23.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:13:53.328116 dagster-openai-0.23.6/dagster_openai/
+-rw-r--r--   0 root         (0) root         (0)      270 2024-05-16 20:06:23.000000 dagster-openai-0.23.6/dagster_openai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-16 20:06:23.000000 dagster-openai-0.23.6/dagster_openai/py.typed
+-rw-r--r--   0 root         (0) root         (0)    15015 2024-05-16 20:06:23.000000 dagster-openai-0.23.6/dagster_openai/resources.py
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-16 20:06:23.000000 dagster-openai-0.23.6/dagster_openai/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:13:53.328116 dagster-openai-0.23.6/dagster_openai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      640 2024-05-16 20:13:53.000000 dagster-openai-0.23.6/dagster_openai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      379 2024-05-16 20:13:53.000000 dagster-openai-0.23.6/dagster_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 20:13:53.000000 dagster-openai-0.23.6/dagster_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 20:13:53.000000 dagster-openai-0.23.6/dagster_openai.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-16 20:13:53.000000 dagster-openai-0.23.6/dagster_openai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-16 20:13:53.000000 dagster-openai-0.23.6/dagster_openai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      161 2024-05-16 20:13:53.332116 dagster-openai-0.23.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1207 2024-05-16 20:06:23.000000 dagster-openai-0.23.6/setup.py
```

### Comparing `dagster-openai-0.23.5/LICENSE` & `dagster-openai-0.23.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-openai-0.23.5/PKG-INFO` & `dagster-openai-0.23.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-openai
-Version: 0.23.5
+Version: 0.23.6
 Summary: A Open AI client resource for interacting with Open AI API.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-openai
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-openai-0.23.5/dagster_openai/resources.py` & `dagster-openai-0.23.6/dagster_openai/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-openai-0.23.5/dagster_openai.egg-info/PKG-INFO` & `dagster-openai-0.23.6/dagster_openai.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-openai
-Version: 0.23.5
+Version: 0.23.6
 Summary: A Open AI client resource for interacting with Open AI API.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-openai
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-openai-0.23.5/setup.py` & `dagster-openai-0.23.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,12 +28,12 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_openai_tests*"]),
     install_requires=[
-        "dagster==1.7.5",
+        "dagster==1.7.6",
         "openai",
     ],
     zip_safe=False,
 )
```

