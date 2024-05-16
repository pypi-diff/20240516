# Comparing `tmp/ensure_packages-0.1.1.tar.gz` & `tmp/ensure_packages-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensure_packages-0.1.1.tar", last modified: Thu May 16 04:29:59 2024, max compression
+gzip compressed data, was "ensure_packages-0.1.2.tar", last modified: Thu May 16 04:50:44 2024, max compression
```

## Comparing `ensure_packages-0.1.1.tar` & `ensure_packages-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 04:29:59.094003 ensure_packages-0.1.1/
--rw-rw-rw-   0        0        0      578 2024-05-16 04:29:59.094003 ensure_packages-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      126 2024-05-15 07:47:47.000000 ensure_packages-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 04:29:59.094003 ensure_packages-0.1.1/ensure_packages.egg-info/
--rw-rw-rw-   0        0        0      578 2024-05-16 04:29:56.000000 ensure_packages-0.1.1/ensure_packages.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      174 2024-05-16 04:29:57.000000 ensure_packages-0.1.1/ensure_packages.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 04:29:56.000000 ensure_packages-0.1.1/ensure_packages.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 04:29:57.000000 ensure_packages-0.1.1/ensure_packages.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 04:29:59.094003 ensure_packages-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      789 2024-05-16 04:28:29.000000 ensure_packages-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 04:50:44.138148 ensure_packages-0.1.2/
+-rw-rw-rw-   0        0        0      578 2024-05-16 04:50:44.138148 ensure_packages-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      126 2024-05-15 07:47:47.000000 ensure_packages-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 04:50:44.037863 ensure_packages-0.1.2/ensure_packages/
+-rw-rw-rw-   0        0        0       44 2024-05-16 04:43:19.000000 ensure_packages-0.1.2/ensure_packages/__init__.py
+-rw-rw-rw-   0        0        0     1203 2024-05-15 07:46:23.000000 ensure_packages-0.1.2/ensure_packages/ensure_package.py
+drwxrwxrwx   0        0        0        0 2024-05-16 04:50:44.122521 ensure_packages-0.1.2/ensure_packages.egg-info/
+-rw-rw-rw-   0        0        0      578 2024-05-16 04:50:43.000000 ensure_packages-0.1.2/ensure_packages.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2024-05-16 04:50:43.000000 ensure_packages-0.1.2/ensure_packages.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 04:50:43.000000 ensure_packages-0.1.2/ensure_packages.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-16 04:50:43.000000 ensure_packages-0.1.2/ensure_packages.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 04:50:44.138148 ensure_packages-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      789 2024-05-16 04:44:47.000000 ensure_packages-0.1.2/setup.py
```

### Comparing `ensure_packages-0.1.1/PKG-INFO` & `ensure_packages-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ensure_packages
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package to ensure other packages are installed its created by vinoth cse-B. a laternate for using pip
 Author: vinothjs
 Author-email: jeyashreenarayan@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `ensure_packages-0.1.1/ensure_packages.egg-info/PKG-INFO` & `ensure_packages-0.1.2/ensure_packages.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ensure-packages
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package to ensure other packages are installed its created by vinoth cse-B. a laternate for using pip
 Author: vinothjs
 Author-email: jeyashreenarayan@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `ensure_packages-0.1.1/setup.py` & `ensure_packages-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="ensure_packages",  # Replace with your own package name
-    version="0.1.1",
+    version="0.1.2",
     author="vinothjs",
     author_email="jeyashreenarayan@gmail.com",
     description="A package to ensure other packages are installed its created by vinoth cse-B. a laternate for using pip",
     long_description=long_description,
     long_description_content_type="text/markdown",
  # Replace with your own URL
     packages=find_packages(),
```

