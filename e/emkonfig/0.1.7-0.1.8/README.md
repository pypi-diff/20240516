# Comparing `tmp/emkonfig-0.1.7.tar.gz` & `tmp/emkonfig-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emkonfig-0.1.7.tar", max compression
+gzip compressed data, was "emkonfig-0.1.8.tar", max compression
```

## Comparing `emkonfig-0.1.7.tar` & `emkonfig-0.1.8.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0       11 2024-02-29 13:39:01.443391 emkonfig-0.1.7/README.md
--rw-r--r--   0        0        0        0 2024-03-20 15:33:07.236309 emkonfig-0.1.7/emkonfig/__init__.py
--rw-r--r--   0        0        0     1759 2024-05-10 14:02:15.140274 emkonfig-0.1.7/emkonfig/config.py
--rw-r--r--   0        0        0    18019 2024-05-10 13:51:38.329335 emkonfig-0.1.7/emkonfig/external/hydra/instantiate.py
--rw-r--r--   0        0        0     4828 2024-05-09 13:32:22.917539 emkonfig-0.1.7/emkonfig/parsers.py
--rw-r--r--   0        0        0     1052 2024-03-21 15:44:31.173249 emkonfig-0.1.7/emkonfig/registry.py
--rw-r--r--   0        0        0     1278 2024-05-10 14:29:23.729690 emkonfig-0.1.7/emkonfig/utils.py
--rw-r--r--   0        0        0     3104 2024-05-10 14:29:31.995138 emkonfig-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 emkonfig-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       11 2024-02-29 13:39:01.443391 emkonfig-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2024-03-20 15:33:07.236309 emkonfig-0.1.8/emkonfig/__init__.py
+-rw-r--r--   0        0        0      765 2024-05-16 11:18:20.914741 emkonfig-0.1.8/emkonfig/config.py
+-rw-r--r--   0        0        0    13274 2024-05-10 13:53:23.825055 emkonfig-0.1.8/emkonfig/external/hydra/__pycache__/instantiate.cpython-310.pyc
+-rw-r--r--   0        0        0    18019 2024-05-10 13:51:38.329335 emkonfig-0.1.8/emkonfig/external/hydra/instantiate.py
+-rw-r--r--   0        0        0     6590 2024-05-16 13:24:27.519860 emkonfig-0.1.8/emkonfig/parsers.py
+-rw-r--r--   0        0        0     1052 2024-03-21 15:44:31.173249 emkonfig-0.1.8/emkonfig/registry.py
+-rw-r--r--   0        0        0     1278 2024-05-10 14:29:23.729690 emkonfig-0.1.8/emkonfig/utils.py
+-rw-r--r--   0        0        0     3104 2024-05-16 13:25:27.675012 emkonfig-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 emkonfig-0.1.8/PKG-INFO
```

### Comparing `emkonfig-0.1.7/emkonfig/external/hydra/instantiate.py` & `emkonfig-0.1.8/emkonfig/external/hydra/instantiate.py`

 * *Files identical despite different names*

### Comparing `emkonfig-0.1.7/emkonfig/registry.py` & `emkonfig-0.1.8/emkonfig/registry.py`

 * *Files identical despite different names*

### Comparing `emkonfig-0.1.7/emkonfig/utils.py` & `emkonfig-0.1.8/emkonfig/utils.py`

 * *Files identical despite different names*

### Comparing `emkonfig-0.1.7/pyproject.toml` & `emkonfig-0.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "emkonfig"
-version = "0.1.7"
+version = "0.1.8"
 description = "YAML template based configuration management tool"
 authors = ["Kıvanç Yüksel <kivanc.yuksel@emkademy.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers= [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
```

### Comparing `emkonfig-0.1.7/PKG-INFO` & `emkonfig-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emkonfig
-Version: 0.1.7
+Version: 0.1.8
 Summary: YAML template based configuration management tool
 License: MIT
 Author: Kıvanç Yüksel
 Author-email: kivanc.yuksel@emkademy.com
 Requires-Python: >=3.10
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

