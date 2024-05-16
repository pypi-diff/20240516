# Comparing `tmp/funkai-0.9.tar.gz` & `tmp/funkai-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funkai-0.9.tar", last modified: Thu May 16 04:28:59 2024, max compression
+gzip compressed data, was "funkai-1.0.tar", last modified: Thu May 16 04:42:27 2024, max compression
```

## Comparing `funkai-0.9.tar` & `funkai-1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 sameer     (502) staff       (20)        0 2024-05-16 04:28:59.442736 funkai-0.9/
--rw-r--r--   0 sameer     (502) staff       (20)     4898 2024-05-16 04:28:59.442476 funkai-0.9/PKG-INFO
--rw-r--r--   0 sameer     (502) staff       (20)     4486 2024-05-14 06:00:28.000000 funkai-0.9/README.md
-drwxr-xr-x   0 sameer     (502) staff       (20)        0 2024-05-16 04:28:59.441020 funkai-0.9/funkai/
--rw-r--r--   0 sameer     (502) staff       (20)       61 2024-05-14 06:00:28.000000 funkai-0.9/funkai/__init__.py
--rw-r--r--   0 sameer     (502) staff       (20)      199 2024-05-14 06:00:28.000000 funkai-0.9/funkai/claude.py
--rw-r--r--   0 sameer     (502) staff       (20)    10838 2024-03-01 12:09:36.000000 funkai-0.9/funkai/examples.py
--rw-r--r--   0 sameer     (502) staff       (20)     6471 2024-05-14 06:00:28.000000 funkai-0.9/funkai/funk.py
--rw-r--r--   0 sameer     (502) staff       (20)     1639 2024-05-14 06:00:28.000000 funkai-0.9/funkai/manager.py
--rw-r--r--   0 sameer     (502) staff       (20)      190 2024-05-14 06:00:28.000000 funkai-0.9/funkai/openai.py
-drwxr-xr-x   0 sameer     (502) staff       (20)        0 2024-05-16 04:28:59.441983 funkai-0.9/funkai.egg-info/
--rw-r--r--   0 sameer     (502) staff       (20)     4898 2024-05-16 04:28:59.000000 funkai-0.9/funkai.egg-info/PKG-INFO
--rw-r--r--   0 sameer     (502) staff       (20)      272 2024-05-16 04:28:59.000000 funkai-0.9/funkai.egg-info/SOURCES.txt
--rw-r--r--   0 sameer     (502) staff       (20)        1 2024-05-16 04:28:59.000000 funkai-0.9/funkai.egg-info/dependency_links.txt
--rw-r--r--   0 sameer     (502) staff       (20)       24 2024-05-16 04:28:59.000000 funkai-0.9/funkai.egg-info/requires.txt
--rw-r--r--   0 sameer     (502) staff       (20)        7 2024-05-16 04:28:59.000000 funkai-0.9/funkai.egg-info/top_level.txt
--rw-r--r--   0 sameer     (502) staff       (20)       38 2024-05-16 04:28:59.442805 funkai-0.9/setup.cfg
--rw-r--r--   0 sameer     (502) staff       (20)      567 2024-05-16 04:28:58.000000 funkai-0.9/setup.py
+drwxr-xr-x   0 sameer     (502) staff       (20)        0 2024-05-16 04:42:27.339614 funkai-1.0/
+-rw-r--r--   0 sameer     (502) staff       (20)     4901 2024-05-16 04:42:27.339399 funkai-1.0/PKG-INFO
+-rw-r--r--   0 sameer     (502) staff       (20)     4486 2024-05-14 06:00:28.000000 funkai-1.0/README.md
+drwxr-xr-x   0 sameer     (502) staff       (20)        0 2024-05-16 04:42:27.338410 funkai-1.0/funkai/
+-rw-r--r--   0 sameer     (502) staff       (20)       61 2024-05-14 06:00:28.000000 funkai-1.0/funkai/__init__.py
+-rw-r--r--   0 sameer     (502) staff       (20)      199 2024-05-14 06:00:28.000000 funkai-1.0/funkai/claude.py
+-rw-r--r--   0 sameer     (502) staff       (20)    10838 2024-03-01 12:09:36.000000 funkai-1.0/funkai/examples.py
+-rw-r--r--   0 sameer     (502) staff       (20)     6471 2024-05-14 06:00:28.000000 funkai-1.0/funkai/funk.py
+-rw-r--r--   0 sameer     (502) staff       (20)     1639 2024-05-14 06:00:28.000000 funkai-1.0/funkai/manager.py
+-rw-r--r--   0 sameer     (502) staff       (20)      190 2024-05-14 06:00:28.000000 funkai-1.0/funkai/openai.py
+drwxr-xr-x   0 sameer     (502) staff       (20)        0 2024-05-16 04:42:27.339108 funkai-1.0/funkai.egg-info/
+-rw-r--r--   0 sameer     (502) staff       (20)     4901 2024-05-16 04:42:27.000000 funkai-1.0/funkai.egg-info/PKG-INFO
+-rw-r--r--   0 sameer     (502) staff       (20)      272 2024-05-16 04:42:27.000000 funkai-1.0/funkai.egg-info/SOURCES.txt
+-rw-r--r--   0 sameer     (502) staff       (20)        1 2024-05-16 04:42:27.000000 funkai-1.0/funkai.egg-info/dependency_links.txt
+-rw-r--r--   0 sameer     (502) staff       (20)       27 2024-05-16 04:42:27.000000 funkai-1.0/funkai.egg-info/requires.txt
+-rw-r--r--   0 sameer     (502) staff       (20)        7 2024-05-16 04:42:27.000000 funkai-1.0/funkai.egg-info/top_level.txt
+-rw-r--r--   0 sameer     (502) staff       (20)       38 2024-05-16 04:42:27.339661 funkai-1.0/setup.cfg
+-rw-r--r--   0 sameer     (502) staff       (20)      570 2024-05-16 04:42:20.000000 funkai-1.0/setup.py
```

### Comparing `funkai-0.9/PKG-INFO` & `funkai-1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: funkai
-Version: 0.9
+Version: 1.0
 Summary: Easily create and deploy placeholder functions powered by OpenAI for rapid prototyping, diverse linguistic tasks, and quick insights.
 Home-page: https://github.com/ciaraadkins/funkai
 Author: Ciara Adkins
 Author-email: adkins.ciara@gmail.com.com
 Description-Content-Type: text/markdown
 Requires-Dist: openai
 Requires-Dist: llmonitor
-Requires-Dist: claude
+Requires-Dist: anthropic
 
 # Funkai Library
 
 Funkai is a Python library that encapsulates linguistic operations and uses OpenAI to perform them based on user inputs.
 
 ## Features
```

### Comparing `funkai-0.9/README.md` & `funkai-1.0/README.md`

 * *Files identical despite different names*

### Comparing `funkai-0.9/funkai/examples.py` & `funkai-1.0/funkai/examples.py`

 * *Files identical despite different names*

### Comparing `funkai-0.9/funkai/funk.py` & `funkai-1.0/funkai/funk.py`

 * *Files identical despite different names*

### Comparing `funkai-0.9/funkai/manager.py` & `funkai-1.0/funkai/manager.py`

 * *Files identical despite different names*

### Comparing `funkai-0.9/funkai.egg-info/PKG-INFO` & `funkai-1.0/funkai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: funkai
-Version: 0.9
+Version: 1.0
 Summary: Easily create and deploy placeholder functions powered by OpenAI for rapid prototyping, diverse linguistic tasks, and quick insights.
 Home-page: https://github.com/ciaraadkins/funkai
 Author: Ciara Adkins
 Author-email: adkins.ciara@gmail.com.com
 Description-Content-Type: text/markdown
 Requires-Dist: openai
 Requires-Dist: llmonitor
-Requires-Dist: claude
+Requires-Dist: anthropic
 
 # Funkai Library
 
 Funkai is a Python library that encapsulates linguistic operations and uses OpenAI to perform them based on user inputs.
 
 ## Features
```

### Comparing `funkai-0.9/setup.py` & `funkai-1.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name="funkai",
-    version="0.9",
+    version="1.0",
     packages=find_packages(),
     install_requires=[
-        "openai",  'llmonitor', 'claude'
+        "openai",  'llmonitor', 'anthropic'
     ],
     author="Ciara Adkins",
     author_email="adkins.ciara@gmail.com.com",
     description="Easily create and deploy placeholder functions powered by OpenAI for rapid prototyping, diverse linguistic tasks, and quick insights.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/ciaraadkins/funkai",
```

