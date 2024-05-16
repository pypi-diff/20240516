# Comparing `tmp/configureout-1.3.tar.gz` & `tmp/configureout-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configureout-1.3.tar", last modified: Mon Apr  1 17:31:19 2024, max compression
+gzip compressed data, was "configureout-1.4.tar", last modified: Thu May 16 14:02:14 2024, max compression
```

## Comparing `configureout-1.3.tar` & `configureout-1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 17:31:19.252904 configureout-1.3/
--rw-rw-rw-   0        0        0     2193 2024-04-01 17:31:19.251906 configureout-1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1792 2024-04-01 13:08:22.000000 configureout-1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 17:31:19.230253 configureout-1.3/configureout/
--rw-rw-rw-   0        0        0     1058 2024-04-01 17:30:46.000000 configureout-1.3/configureout/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 17:31:19.250934 configureout-1.3/configureout.egg-info/
--rw-rw-rw-   0        0        0     2193 2024-04-01 17:31:19.000000 configureout-1.3/configureout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2024-04-01 17:31:19.000000 configureout-1.3/configureout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 17:31:19.000000 configureout-1.3/configureout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-01 17:31:19.000000 configureout-1.3/configureout.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-01 17:31:19.000000 configureout-1.3/configureout.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-01 17:31:19.252904 configureout-1.3/setup.cfg
--rw-rw-rw-   0        0        0      671 2024-04-01 17:31:06.000000 configureout-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 14:02:14.759927 configureout-1.4/
+-rw-rw-rw-   0        0        0     2193 2024-05-16 14:02:14.759927 configureout-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1792 2024-04-01 13:08:22.000000 configureout-1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 14:02:14.736928 configureout-1.4/configureout/
+-rw-rw-rw-   0        0        0     1265 2024-05-16 13:55:13.000000 configureout-1.4/configureout/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 14:02:14.757928 configureout-1.4/configureout.egg-info/
+-rw-rw-rw-   0        0        0     2193 2024-05-16 14:02:14.000000 configureout-1.4/configureout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2024-05-16 14:02:14.000000 configureout-1.4/configureout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 14:02:14.000000 configureout-1.4/configureout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-16 14:02:14.000000 configureout-1.4/configureout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-16 14:02:14.000000 configureout-1.4/configureout.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 14:02:14.759927 configureout-1.4/setup.cfg
+-rw-rw-rw-   0        0        0      671 2024-05-16 14:01:03.000000 configureout-1.4/setup.py
```

### Comparing `configureout-1.3/PKG-INFO` & `configureout-1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configureout
-Version: 1.3
+Version: 1.4
 Summary: A simple configuration module
 Home-page: https://github.com/EightShift/configureout
 Author: EightShift
 Author-email: the8shift@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `configureout-1.3/README.md` & `configureout-1.4/README.md`

 * *Files identical despite different names*

### Comparing `configureout-1.3/configureout.egg-info/PKG-INFO` & `configureout-1.4/configureout.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configureout
-Version: 1.3
+Version: 1.4
 Summary: A simple configuration module
 Home-page: https://github.com/EightShift/configureout
 Author: EightShift
 Author-email: the8shift@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `configureout-1.3/setup.py` & `configureout-1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='configureout',
-    version='1.3',
+    version='1.4',
     description='A simple configuration module',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='EightShift',
     author_email='the8shift@gmail.com',
     url='https://github.com/EightShift/configureout',
     packages=find_packages(),
```

