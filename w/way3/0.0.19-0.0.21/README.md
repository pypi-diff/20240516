# Comparing `tmp/way3-0.0.19.tar.gz` & `tmp/way3-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "way3-0.0.19.tar", last modified: Thu May 16 12:53:13 2024, max compression
+gzip compressed data, was "way3-0.0.21.tar", last modified: Thu May 16 14:43:23 2024, max compression
```

## Comparing `way3-0.0.19.tar` & `way3-0.0.21.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-05-16 12:53:13.550846 way3-0.0.19/
--rw-r--r--   0 apple      (501) staff       (20)     1063 2024-05-16 12:48:52.000000 way3-0.0.19/LICENSE
--rw-r--r--   0 apple      (501) staff       (20)     3979 2024-05-16 12:53:13.550603 way3-0.0.19/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)     3550 2024-05-16 12:21:36.000000 way3-0.0.19/README.md
--rw-r--r--   0 apple      (501) staff       (20)       38 2024-05-16 12:53:13.550902 way3-0.0.19/setup.cfg
--rw-r--r--   0 apple      (501) staff       (20)      638 2024-05-16 12:53:09.000000 way3-0.0.19/setup.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-05-16 12:53:13.548917 way3-0.0.19/tests/
--rw-r--r--   0 apple      (501) staff       (20)        0 2024-05-16 05:15:19.000000 way3-0.0.19/tests/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)      257 2024-05-16 10:20:09.000000 way3-0.0.19/tests/test_file_find.py
--rw-r--r--   0 apple      (501) staff       (20)      839 2024-05-16 12:16:17.000000 way3-0.0.19/tests/test_file_op.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-05-16 12:53:13.549054 way3-0.0.19/way3/
--rw-r--r--   0 apple      (501) staff       (20)      353 2024-05-16 10:14:38.000000 way3-0.0.19/way3/__init__.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-05-16 12:53:13.549890 way3-0.0.19/way3/file_find/
--rw-r--r--   0 apple      (501) staff       (20)        0 2024-05-16 10:07:56.000000 way3-0.0.19/way3/file_find/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)      106 2024-05-16 12:17:20.000000 way3-0.0.19/way3/file_find/current_dir.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-05-16 12:53:13.550163 way3-0.0.19/way3/file_op/
--rw-r--r--   0 apple      (501) staff       (20)        0 2024-05-16 09:34:55.000000 way3-0.0.19/way3/file_op/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     1735 2024-05-16 09:59:08.000000 way3-0.0.19/way3/file_op/create_file.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-05-16 12:53:13.550405 way3-0.0.19/way3.egg-info/
--rw-r--r--   0 apple      (501) staff       (20)     3979 2024-05-16 12:53:13.000000 way3-0.0.19/way3.egg-info/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)      329 2024-05-16 12:53:13.000000 way3-0.0.19/way3.egg-info/SOURCES.txt
--rw-r--r--   0 apple      (501) staff       (20)        1 2024-05-16 12:53:13.000000 way3-0.0.19/way3.egg-info/dependency_links.txt
--rw-r--r--   0 apple      (501) staff       (20)       11 2024-05-16 12:53:13.000000 way3-0.0.19/way3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:43:23.393344 way3-0.0.21/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-16 14:43:20.000000 way3-0.0.21/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-05-16 14:43:23.393344 way3-0.0.21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-16 14:43:20.000000 way3-0.0.21/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 14:43:23.393344 way3-0.0.21/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-16 14:43:20.000000 way3-0.0.21/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:43:23.389345 way3-0.0.21/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 14:43:20.000000 way3-0.0.21/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-16 14:43:20.000000 way3-0.0.21/tests/test_file_find.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-16 14:43:20.000000 way3-0.0.21/tests/test_file_op.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:43:23.389345 way3-0.0.21/way3/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-16 14:43:20.000000 way3-0.0.21/way3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:43:23.389345 way3-0.0.21/way3/file_find/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 14:43:20.000000 way3-0.0.21/way3/file_find/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-16 14:43:20.000000 way3-0.0.21/way3/file_find/current_dir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-16 14:43:20.000000 way3-0.0.21/way3/file_find/traverse_files_from_folder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:43:23.389345 way3-0.0.21/way3/file_op/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 14:43:20.000000 way3-0.0.21/way3/file_op/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-16 14:43:20.000000 way3-0.0.21/way3/file_op/create_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:43:23.389345 way3-0.0.21/way3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-05-16 14:43:23.000000 way3-0.0.21/way3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-16 14:43:23.000000 way3-0.0.21/way3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 14:43:23.000000 way3-0.0.21/way3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-16 14:43:23.000000 way3-0.0.21/way3.egg-info/top_level.txt
```

### Comparing `way3-0.0.19/LICENSE` & `way3-0.0.21/LICENSE`

 * *Files identical despite different names*

### Comparing `way3-0.0.19/PKG-INFO` & `way3-0.0.21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: way3
-Version: 0.0.19
+Version: 0.0.21
 Summary: Simplified file path management for Python developers
 Home-page: https://github.com/aboutmydreams/way3
 Author: aboutmydreams
 Author-email: aboutmydreams@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,16 +21,14 @@
 [![Visits](https://komarev.com/ghpvc/?username=aboutmydreams&repo=way3)](https://github.com/aboutmydreams/way3)
 [![License](https://img.shields.io/github/license/aboutmydreams/way3.svg)](https://github.com/aboutmydreams/way3/license)
 [![Stars](https://img.shields.io/github/stars/aboutmydreams/way3.svg)](https://github.com/aboutmydreams/way3/stargazers)
 [![Forks](https://img.shields.io/github/forks/aboutmydreams/way3.svg)](https://github.com/aboutmydreams/way3/network)
 [![Downloads](https://pepy.tech/badge/way3)](https://pepy.tech/project/way3)
 [![Contributors](https://img.shields.io/github/contributors/aboutmydreams/way3.svg)](https://github.com/aboutmydreams/way3/graphs/contributors)
 
-
-
 Way3 is a Python module for performing file operations such as creating, appending to, and deleting files. It provides a convenient and easy-to-use interface for performing file operations.
 
 ## Installation
 
 To install Way3, you can use pip:
 
 ```bash
```

### Comparing `way3-0.0.19/README.md` & `way3-0.0.21/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 [![Visits](https://komarev.com/ghpvc/?username=aboutmydreams&repo=way3)](https://github.com/aboutmydreams/way3)
 [![License](https://img.shields.io/github/license/aboutmydreams/way3.svg)](https://github.com/aboutmydreams/way3/license)
 [![Stars](https://img.shields.io/github/stars/aboutmydreams/way3.svg)](https://github.com/aboutmydreams/way3/stargazers)
 [![Forks](https://img.shields.io/github/forks/aboutmydreams/way3.svg)](https://github.com/aboutmydreams/way3/network)
 [![Downloads](https://pepy.tech/badge/way3)](https://pepy.tech/project/way3)
 [![Contributors](https://img.shields.io/github/contributors/aboutmydreams/way3.svg)](https://github.com/aboutmydreams/way3/graphs/contributors)
 
-
-
 Way3 is a Python module for performing file operations such as creating, appending to, and deleting files. It provides a convenient and easy-to-use interface for performing file operations.
 
 ## Installation
 
 To install Way3, you can use pip:
 
 ```bash
```

### Comparing `way3-0.0.19/setup.py` & `way3-0.0.21/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="way3",
-    version="0.0.19",
+    version="0.0.21",
     author="aboutmydreams",
     author_email="aboutmydreams@163.com",
     description="Simplified file path management for Python developers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aboutmydreams/way3",
     packages=setuptools.find_packages(),
```

### Comparing `way3-0.0.19/tests/test_file_op.py` & `way3-0.0.21/tests/test_file_op.py`

 * *Files identical despite different names*

### Comparing `way3-0.0.19/way3/file_op/create_file.py` & `way3-0.0.21/way3/file_op/create_file.py`

 * *Files identical despite different names*

### Comparing `way3-0.0.19/way3.egg-info/PKG-INFO` & `way3-0.0.21/way3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: way3
-Version: 0.0.19
+Version: 0.0.21
 Summary: Simplified file path management for Python developers
 Home-page: https://github.com/aboutmydreams/way3
 Author: aboutmydreams
 Author-email: aboutmydreams@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,16 +21,14 @@
 [![Visits](https://komarev.com/ghpvc/?username=aboutmydreams&repo=way3)](https://github.com/aboutmydreams/way3)
 [![License](https://img.shields.io/github/license/aboutmydreams/way3.svg)](https://github.com/aboutmydreams/way3/license)
 [![Stars](https://img.shields.io/github/stars/aboutmydreams/way3.svg)](https://github.com/aboutmydreams/way3/stargazers)
 [![Forks](https://img.shields.io/github/forks/aboutmydreams/way3.svg)](https://github.com/aboutmydreams/way3/network)
 [![Downloads](https://pepy.tech/badge/way3)](https://pepy.tech/project/way3)
 [![Contributors](https://img.shields.io/github/contributors/aboutmydreams/way3.svg)](https://github.com/aboutmydreams/way3/graphs/contributors)
 
-
-
 Way3 is a Python module for performing file operations such as creating, appending to, and deleting files. It provides a convenient and easy-to-use interface for performing file operations.
 
 ## Installation
 
 To install Way3, you can use pip:
 
 ```bash
```

