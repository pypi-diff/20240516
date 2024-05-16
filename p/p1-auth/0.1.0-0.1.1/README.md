# Comparing `tmp/p1_auth-0.1.0.tar.gz` & `tmp/p1_auth-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p1_auth-0.1.0.tar", last modified: Thu May 16 16:15:57 2024, max compression
+gzip compressed data, was "p1_auth-0.1.1.tar", last modified: Thu May 16 16:39:52 2024, max compression
```

## Comparing `p1_auth-0.1.0.tar` & `p1_auth-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2024-05-16 16:15:57.972551 p1_auth-0.1.0/
--rw-r--r--   0 jametobin   (502) staff       (20)     4458 2024-05-16 16:15:57.972322 p1_auth-0.1.0/PKG-INFO
--rw-r--r--   0 jametobin   (502) staff       (20)     3482 2024-05-15 15:17:01.000000 p1_auth-0.1.0/README.md
-drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2024-05-16 16:15:57.968436 p1_auth-0.1.0/p1_auth/
--rw-r--r--   0 jametobin   (502) staff       (20)        0 2024-05-15 15:17:01.000000 p1_auth-0.1.0/p1_auth/__init__.py
--rw-r--r--   0 jametobin   (502) staff       (20)      849 2024-05-15 15:17:01.000000 p1_auth-0.1.0/p1_auth/admin.py
--rw-r--r--   0 jametobin   (502) staff       (20)      145 2024-05-15 15:17:01.000000 p1_auth-0.1.0/p1_auth/apps.py
--rw-r--r--   0 jametobin   (502) staff       (20)     5676 2024-05-15 15:17:01.000000 p1_auth-0.1.0/p1_auth/backends.py
--rw-r--r--   0 jametobin   (502) staff       (20)      460 2024-05-15 15:17:01.000000 p1_auth-0.1.0/p1_auth/middleware.py
--rw-r--r--   0 jametobin   (502) staff       (20)     3599 2024-05-15 15:17:01.000000 p1_auth-0.1.0/p1_auth/models.py
--rw-r--r--   0 jametobin   (502) staff       (20)       60 2024-05-15 15:17:01.000000 p1_auth-0.1.0/p1_auth/tests.py
--rw-r--r--   0 jametobin   (502) staff       (20)      613 2024-05-15 15:17:01.000000 p1_auth-0.1.0/p1_auth/views.py
-drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2024-05-16 16:15:57.971657 p1_auth-0.1.0/p1_auth.egg-info/
--rw-r--r--   0 jametobin   (502) staff       (20)     4458 2024-05-16 16:15:57.000000 p1_auth-0.1.0/p1_auth.egg-info/PKG-INFO
--rw-r--r--   0 jametobin   (502) staff       (20)      329 2024-05-16 16:15:57.000000 p1_auth-0.1.0/p1_auth.egg-info/SOURCES.txt
--rw-r--r--   0 jametobin   (502) staff       (20)        1 2024-05-16 16:15:57.000000 p1_auth-0.1.0/p1_auth.egg-info/dependency_links.txt
--rw-r--r--   0 jametobin   (502) staff       (20)       41 2024-05-16 16:15:57.000000 p1_auth-0.1.0/p1_auth.egg-info/requires.txt
--rw-r--r--   0 jametobin   (502) staff       (20)        8 2024-05-16 16:15:57.000000 p1_auth-0.1.0/p1_auth.egg-info/top_level.txt
--rw-r--r--   0 jametobin   (502) staff       (20)     1032 2024-05-16 16:15:57.973079 p1_auth-0.1.0/setup.cfg
--rw-r--r--   0 jametobin   (502) staff       (20)       95 2024-05-15 15:17:01.000000 p1_auth-0.1.0/setup.py
+drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2024-05-16 16:39:52.185956 p1_auth-0.1.1/
+-rw-r--r--   0 jametobin   (502) staff       (20)     4458 2024-05-16 16:39:52.185748 p1_auth-0.1.1/PKG-INFO
+-rw-r--r--   0 jametobin   (502) staff       (20)     3482 2024-05-15 15:17:01.000000 p1_auth-0.1.1/README.md
+drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2024-05-16 16:39:52.180709 p1_auth-0.1.1/p1_auth/
+-rw-r--r--   0 jametobin   (502) staff       (20)        0 2024-05-15 15:17:01.000000 p1_auth-0.1.1/p1_auth/__init__.py
+-rw-r--r--   0 jametobin   (502) staff       (20)      849 2024-05-15 15:17:01.000000 p1_auth-0.1.1/p1_auth/admin.py
+-rw-r--r--   0 jametobin   (502) staff       (20)      145 2024-05-15 15:17:01.000000 p1_auth-0.1.1/p1_auth/apps.py
+-rw-r--r--   0 jametobin   (502) staff       (20)     5676 2024-05-15 15:17:01.000000 p1_auth-0.1.1/p1_auth/backends.py
+-rw-r--r--   0 jametobin   (502) staff       (20)      460 2024-05-15 15:17:01.000000 p1_auth-0.1.1/p1_auth/middleware.py
+drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2024-05-16 16:39:52.184499 p1_auth-0.1.1/p1_auth/migrations/
+-rw-r--r--   0 jametobin   (502) staff       (20)     1250 2024-05-15 15:17:01.000000 p1_auth-0.1.1/p1_auth/migrations/0001_initial.py
+-rw-r--r--   0 jametobin   (502) staff       (20)        0 2024-05-15 15:17:01.000000 p1_auth-0.1.1/p1_auth/migrations/__init__.py
+-rw-r--r--   0 jametobin   (502) staff       (20)     3599 2024-05-15 15:17:01.000000 p1_auth-0.1.1/p1_auth/models.py
+-rw-r--r--   0 jametobin   (502) staff       (20)       60 2024-05-15 15:17:01.000000 p1_auth-0.1.1/p1_auth/tests.py
+-rw-r--r--   0 jametobin   (502) staff       (20)      613 2024-05-15 15:17:01.000000 p1_auth-0.1.1/p1_auth/views.py
+drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2024-05-16 16:39:52.184925 p1_auth-0.1.1/p1_auth.egg-info/
+-rw-r--r--   0 jametobin   (502) staff       (20)     4458 2024-05-16 16:39:52.000000 p1_auth-0.1.1/p1_auth.egg-info/PKG-INFO
+-rw-r--r--   0 jametobin   (502) staff       (20)      395 2024-05-16 16:39:52.000000 p1_auth-0.1.1/p1_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 jametobin   (502) staff       (20)        1 2024-05-16 16:39:52.000000 p1_auth-0.1.1/p1_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 jametobin   (502) staff       (20)       41 2024-05-16 16:39:52.000000 p1_auth-0.1.1/p1_auth.egg-info/requires.txt
+-rw-r--r--   0 jametobin   (502) staff       (20)        8 2024-05-16 16:39:52.000000 p1_auth-0.1.1/p1_auth.egg-info/top_level.txt
+-rw-r--r--   0 jametobin   (502) staff       (20)     1053 2024-05-16 16:39:52.186441 p1_auth-0.1.1/setup.cfg
+-rw-r--r--   0 jametobin   (502) staff       (20)       95 2024-05-15 15:17:01.000000 p1_auth-0.1.1/setup.py
```

### Comparing `p1_auth-0.1.0/PKG-INFO` & `p1_auth-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p1-auth
-Version: 0.1.0
+Version: 0.1.1
 Summary: Installable Django Authentication that adds support for Platform One
 Home-page: https://github.com/OpenLXP/p1-auth/
 Author: OpenLXP
 Author-email: openlxphost@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `p1_auth-0.1.0/README.md` & `p1_auth-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `p1_auth-0.1.0/p1_auth/admin.py` & `p1_auth-0.1.1/p1_auth/admin.py`

 * *Files identical despite different names*

### Comparing `p1_auth-0.1.0/p1_auth/backends.py` & `p1_auth-0.1.1/p1_auth/backends.py`

 * *Files identical despite different names*

### Comparing `p1_auth-0.1.0/p1_auth/models.py` & `p1_auth-0.1.1/p1_auth/models.py`

 * *Files identical despite different names*

### Comparing `p1_auth-0.1.0/p1_auth/views.py` & `p1_auth-0.1.1/p1_auth/views.py`

 * *Files identical despite different names*

### Comparing `p1_auth-0.1.0/p1_auth.egg-info/PKG-INFO` & `p1_auth-0.1.1/p1_auth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p1-auth
-Version: 0.1.0
+Version: 0.1.1
 Summary: Installable Django Authentication that adds support for Platform One
 Home-page: https://github.com/OpenLXP/p1-auth/
 Author: OpenLXP
 Author-email: openlxphost@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `p1_auth-0.1.0/setup.cfg` & `p1_auth-0.1.1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = p1-auth
-version = 0.1.0
+version = 0.1.1
 description = Installable Django Authentication that adds support for Platform One
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/OpenLXP/p1-auth/
 author = OpenLXP
 author_email = openlxphost@gmail.com
 license = MIT
@@ -19,15 +19,15 @@
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: Implementation :: CPython
 	Topic :: Software Development :: Libraries :: Application Frameworks
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 include_package_data = true
-packages = p1_auth
+packages = p1_auth, p1_auth.migrations,
 python_requires = >=3.7
 setup_requires = 
 	setuptools >= 38.3.0
 install_requires = 
 	PyJWT>=2.0.0
 	djangorestframework>=3.13.0
```

