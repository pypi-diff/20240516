# Comparing `tmp/hygpytools-0.2.0.tar.gz` & `tmp/hygpytools-6.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hygpytools-0.2.0.tar", last modified: Wed May 15 22:14:15 2024, max compression
+gzip compressed data, was "hygpytools-6.6.6.tar", last modified: Wed May 15 22:13:53 2024, max compression
```

## Comparing `hygpytools-0.2.0.tar` & `hygpytools-6.6.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 22:14:15.149798 hygpytools-0.2.0/
--rw-rw-rw-   0        0        0      662 2024-05-15 22:14:15.149798 hygpytools-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       24 2024-05-15 20:47:34.000000 hygpytools-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 22:14:15.139172 hygpytools-0.2.0/hygpytools/
--rw-rw-rw-   0        0        0      662 2024-05-15 21:30:51.000000 hygpytools-0.2.0/hygpytools/__init__.py
--rw-rw-rw-   0        0        0       50 2024-05-15 20:46:43.000000 hygpytools-0.2.0/hygpytools/example.py
-drwxrwxrwx   0        0        0        0 2024-05-15 22:14:15.149798 hygpytools-0.2.0/hygpytools.egg-info/
--rw-rw-rw-   0        0        0      662 2024-05-15 22:14:15.000000 hygpytools-0.2.0/hygpytools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2024-05-15 22:14:15.000000 hygpytools-0.2.0/hygpytools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 22:14:15.000000 hygpytools-0.2.0/hygpytools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-15 22:14:15.000000 hygpytools-0.2.0/hygpytools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      707 2024-05-15 22:14:06.000000 hygpytools-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-15 22:14:15.149798 hygpytools-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-15 22:13:53.576238 hygpytools-6.6.6/
+-rw-rw-rw-   0        0        0      662 2024-05-15 22:13:53.576238 hygpytools-6.6.6/PKG-INFO
+-rw-rw-rw-   0        0        0       24 2024-05-15 20:47:34.000000 hygpytools-6.6.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 22:13:53.566494 hygpytools-6.6.6/hygpytools/
+-rw-rw-rw-   0        0        0      662 2024-05-15 21:30:51.000000 hygpytools-6.6.6/hygpytools/__init__.py
+-rw-rw-rw-   0        0        0       50 2024-05-15 20:46:43.000000 hygpytools-6.6.6/hygpytools/example.py
+drwxrwxrwx   0        0        0        0 2024-05-15 22:13:53.575177 hygpytools-6.6.6/hygpytools.egg-info/
+-rw-rw-rw-   0        0        0      662 2024-05-15 22:13:53.000000 hygpytools-6.6.6/hygpytools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2024-05-15 22:13:53.000000 hygpytools-6.6.6/hygpytools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 22:13:53.000000 hygpytools-6.6.6/hygpytools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-15 22:13:53.000000 hygpytools-6.6.6/hygpytools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      707 2024-05-15 22:03:34.000000 hygpytools-6.6.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-15 22:13:53.576238 hygpytools-6.6.6/setup.cfg
```

### Comparing `hygpytools-0.2.0/PKG-INFO` & `hygpytools-6.6.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hygpytools
-Version: 0.2.0
+Version: 6.6.6
 Summary: A simple example Python package.
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `hygpytools-0.2.0/hygpytools/__init__.py` & `hygpytools-6.6.6/hygpytools/__init__.py`

 * *Files identical despite different names*

### Comparing `hygpytools-0.2.0/hygpytools.egg-info/PKG-INFO` & `hygpytools-6.6.6/hygpytools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hygpytools
-Version: 0.2.0
+Version: 6.6.6
 Summary: A simple example Python package.
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `hygpytools-0.2.0/pyproject.toml` & `hygpytools-6.6.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hygpytools"
-version = "0.2.0"
+version = "6.6.6"
 description = "A simple example Python package."
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
```

