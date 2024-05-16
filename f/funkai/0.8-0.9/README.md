# Comparing `tmp/funkai-0.8.tar.gz` & `tmp/funkai-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funkai-0.8.tar", last modified: Tue May 14 06:00:52 2024, max compression
+gzip compressed data, was "funkai-0.9.tar", last modified: Thu May 16 04:28:59 2024, max compression
```

## Comparing `funkai-0.8.tar` & `funkai-0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 sameer     (502) staff       (20)        0 2024-05-14 06:00:52.192613 funkai-0.8/
--rw-r--r--   0 sameer     (502) staff       (20)     4898 2024-05-14 06:00:52.192350 funkai-0.8/PKG-INFO
--rw-r--r--   0 sameer     (502) staff       (20)     4486 2024-05-14 06:00:28.000000 funkai-0.8/README.md
-drwxr-xr-x   0 sameer     (502) staff       (20)        0 2024-05-14 06:00:52.190957 funkai-0.8/funkai/
--rw-r--r--   0 sameer     (502) staff       (20)       61 2024-05-14 06:00:28.000000 funkai-0.8/funkai/__init__.py
--rw-r--r--   0 sameer     (502) staff       (20)      199 2024-05-14 06:00:28.000000 funkai-0.8/funkai/claude.py
--rw-r--r--   0 sameer     (502) staff       (20)    10838 2024-03-01 12:09:36.000000 funkai-0.8/funkai/examples.py
--rw-r--r--   0 sameer     (502) staff       (20)     6471 2024-05-14 06:00:28.000000 funkai-0.8/funkai/funk.py
--rw-r--r--   0 sameer     (502) staff       (20)     1639 2024-05-14 06:00:28.000000 funkai-0.8/funkai/manager.py
--rw-r--r--   0 sameer     (502) staff       (20)      190 2024-05-14 06:00:28.000000 funkai-0.8/funkai/openai.py
-drwxr-xr-x   0 sameer     (502) staff       (20)        0 2024-05-14 06:00:52.191852 funkai-0.8/funkai.egg-info/
--rw-r--r--   0 sameer     (502) staff       (20)     4898 2024-05-14 06:00:52.000000 funkai-0.8/funkai.egg-info/PKG-INFO
--rw-r--r--   0 sameer     (502) staff       (20)      272 2024-05-14 06:00:52.000000 funkai-0.8/funkai.egg-info/SOURCES.txt
--rw-r--r--   0 sameer     (502) staff       (20)        1 2024-05-14 06:00:52.000000 funkai-0.8/funkai.egg-info/dependency_links.txt
--rw-r--r--   0 sameer     (502) staff       (20)       24 2024-05-14 06:00:52.000000 funkai-0.8/funkai.egg-info/requires.txt
--rw-r--r--   0 sameer     (502) staff       (20)        7 2024-05-14 06:00:52.000000 funkai-0.8/funkai.egg-info/top_level.txt
--rw-r--r--   0 sameer     (502) staff       (20)       38 2024-05-14 06:00:52.192664 funkai-0.8/setup.cfg
--rw-r--r--   0 sameer     (502) staff       (20)      567 2024-05-14 06:00:28.000000 funkai-0.8/setup.py
+drwxr-xr-x   0 sameer     (502) staff       (20)        0 2024-05-16 04:28:59.442736 funkai-0.9/
+-rw-r--r--   0 sameer     (502) staff       (20)     4898 2024-05-16 04:28:59.442476 funkai-0.9/PKG-INFO
+-rw-r--r--   0 sameer     (502) staff       (20)     4486 2024-05-14 06:00:28.000000 funkai-0.9/README.md
+drwxr-xr-x   0 sameer     (502) staff       (20)        0 2024-05-16 04:28:59.441020 funkai-0.9/funkai/
+-rw-r--r--   0 sameer     (502) staff       (20)       61 2024-05-14 06:00:28.000000 funkai-0.9/funkai/__init__.py
+-rw-r--r--   0 sameer     (502) staff       (20)      199 2024-05-14 06:00:28.000000 funkai-0.9/funkai/claude.py
+-rw-r--r--   0 sameer     (502) staff       (20)    10838 2024-03-01 12:09:36.000000 funkai-0.9/funkai/examples.py
+-rw-r--r--   0 sameer     (502) staff       (20)     6471 2024-05-14 06:00:28.000000 funkai-0.9/funkai/funk.py
+-rw-r--r--   0 sameer     (502) staff       (20)     1639 2024-05-14 06:00:28.000000 funkai-0.9/funkai/manager.py
+-rw-r--r--   0 sameer     (502) staff       (20)      190 2024-05-14 06:00:28.000000 funkai-0.9/funkai/openai.py
+drwxr-xr-x   0 sameer     (502) staff       (20)        0 2024-05-16 04:28:59.441983 funkai-0.9/funkai.egg-info/
+-rw-r--r--   0 sameer     (502) staff       (20)     4898 2024-05-16 04:28:59.000000 funkai-0.9/funkai.egg-info/PKG-INFO
+-rw-r--r--   0 sameer     (502) staff       (20)      272 2024-05-16 04:28:59.000000 funkai-0.9/funkai.egg-info/SOURCES.txt
+-rw-r--r--   0 sameer     (502) staff       (20)        1 2024-05-16 04:28:59.000000 funkai-0.9/funkai.egg-info/dependency_links.txt
+-rw-r--r--   0 sameer     (502) staff       (20)       24 2024-05-16 04:28:59.000000 funkai-0.9/funkai.egg-info/requires.txt
+-rw-r--r--   0 sameer     (502) staff       (20)        7 2024-05-16 04:28:59.000000 funkai-0.9/funkai.egg-info/top_level.txt
+-rw-r--r--   0 sameer     (502) staff       (20)       38 2024-05-16 04:28:59.442805 funkai-0.9/setup.cfg
+-rw-r--r--   0 sameer     (502) staff       (20)      567 2024-05-16 04:28:58.000000 funkai-0.9/setup.py
```

### Comparing `funkai-0.8/PKG-INFO` & `funkai-0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funkai
-Version: 0.8
+Version: 0.9
 Summary: Easily create and deploy placeholder functions powered by OpenAI for rapid prototyping, diverse linguistic tasks, and quick insights.
 Home-page: https://github.com/ciaraadkins/funkai
 Author: Ciara Adkins
 Author-email: adkins.ciara@gmail.com.com
 Description-Content-Type: text/markdown
 Requires-Dist: openai
 Requires-Dist: llmonitor
```

### Comparing `funkai-0.8/README.md` & `funkai-0.9/README.md`

 * *Files identical despite different names*

### Comparing `funkai-0.8/funkai/examples.py` & `funkai-0.9/funkai/examples.py`

 * *Files identical despite different names*

### Comparing `funkai-0.8/funkai/funk.py` & `funkai-0.9/funkai/funk.py`

 * *Files identical despite different names*

### Comparing `funkai-0.8/funkai/manager.py` & `funkai-0.9/funkai/manager.py`

 * *Files identical despite different names*

### Comparing `funkai-0.8/funkai.egg-info/PKG-INFO` & `funkai-0.9/funkai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funkai
-Version: 0.8
+Version: 0.9
 Summary: Easily create and deploy placeholder functions powered by OpenAI for rapid prototyping, diverse linguistic tasks, and quick insights.
 Home-page: https://github.com/ciaraadkins/funkai
 Author: Ciara Adkins
 Author-email: adkins.ciara@gmail.com.com
 Description-Content-Type: text/markdown
 Requires-Dist: openai
 Requires-Dist: llmonitor
```

### Comparing `funkai-0.8/setup.py` & `funkai-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="funkai",
-    version="0.8",
+    version="0.9",
     packages=find_packages(),
     install_requires=[
         "openai",  'llmonitor', 'claude'
     ],
     author="Ciara Adkins",
     author_email="adkins.ciara@gmail.com.com",
     description="Easily create and deploy placeholder functions powered by OpenAI for rapid prototyping, diverse linguistic tasks, and quick insights.",
```

