# Comparing `tmp/http_file_streamer-0.1.1.tar.gz` & `tmp/http_file_streamer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "http_file_streamer-0.1.1.tar", last modified: Thu May 16 11:53:46 2024, max compression
+gzip compressed data, was "http_file_streamer-0.1.2.tar", last modified: Thu May 16 12:05:22 2024, max compression
```

## Comparing `http_file_streamer-0.1.1.tar` & `http_file_streamer-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 11:53:46.591782 http_file_streamer-0.1.1/
--rw-rw-rw-   0        0        0     1093 2024-05-16 11:21:47.000000 http_file_streamer-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     2336 2024-05-16 11:53:46.590781 http_file_streamer-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1741 2024-05-16 11:52:27.000000 http_file_streamer-0.1.1/README.md
--rw-rw-rw-   0        0        0       97 2024-05-16 11:35:15.000000 http_file_streamer-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-16 11:53:46.591782 http_file_streamer-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      786 2024-05-16 11:53:10.000000 http_file_streamer-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 11:53:46.582704 http_file_streamer-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-16 11:53:46.589783 http_file_streamer-0.1.1/src/http_file_streamer.egg-info/
--rw-rw-rw-   0        0        0     2336 2024-05-16 11:53:46.000000 http_file_streamer-0.1.1/src/http_file_streamer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2024-05-16 11:53:46.000000 http_file_streamer-0.1.1/src/http_file_streamer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 11:53:46.000000 http_file_streamer-0.1.1/src/http_file_streamer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-16 11:53:46.000000 http_file_streamer-0.1.1/src/http_file_streamer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 11:53:46.000000 http_file_streamer-0.1.1/src/http_file_streamer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 12:05:22.042403 http_file_streamer-0.1.2/
+-rw-rw-rw-   0        0        0     1093 2024-05-16 11:21:47.000000 http_file_streamer-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     2336 2024-05-16 12:05:22.042403 http_file_streamer-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1741 2024-05-16 11:52:27.000000 http_file_streamer-0.1.2/README.md
+-rw-rw-rw-   0        0        0       97 2024-05-16 11:35:15.000000 http_file_streamer-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-16 12:05:22.042403 http_file_streamer-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      786 2024-05-16 12:04:37.000000 http_file_streamer-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:05:22.027220 http_file_streamer-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-16 12:05:22.039979 http_file_streamer-0.1.2/src/http_file_streamer/
+-rw-rw-rw-   0        0        0       62 2024-05-16 11:17:06.000000 http_file_streamer-0.1.2/src/http_file_streamer/__init__.py
+-rw-rw-rw-   0        0        0     2762 2024-05-16 11:09:58.000000 http_file_streamer-0.1.2/src/http_file_streamer/receiver.py
+-rw-rw-rw-   0        0        0     3937 2024-05-16 11:03:48.000000 http_file_streamer-0.1.2/src/http_file_streamer/streamer.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:05:22.042403 http_file_streamer-0.1.2/src/http_file_streamer.egg-info/
+-rw-rw-rw-   0        0        0     2336 2024-05-16 12:05:21.000000 http_file_streamer-0.1.2/src/http_file_streamer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      375 2024-05-16 12:05:22.000000 http_file_streamer-0.1.2/src/http_file_streamer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 12:05:21.000000 http_file_streamer-0.1.2/src/http_file_streamer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-16 12:05:21.000000 http_file_streamer-0.1.2/src/http_file_streamer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-16 12:05:21.000000 http_file_streamer-0.1.2/src/http_file_streamer.egg-info/top_level.txt
```

### Comparing `http_file_streamer-0.1.1/LICENSE` & `http_file_streamer-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `http_file_streamer-0.1.1/PKG-INFO` & `http_file_streamer-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: http_file_streamer
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package for streaming and receiving files.
 Home-page: https://github.com/babakzarrinbal/httpfilestreamer.git
 Author: Babak Zarrinbal
 Author-email: babak.zarrinbal@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `http_file_streamer-0.1.1/README.md` & `http_file_streamer-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `http_file_streamer-0.1.1/setup.py` & `http_file_streamer-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="http_file_streamer",
-    version="0.1.1",
+    version="0.1.2",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     install_requires=[
         "requests",
     ],
     author="Babak Zarrinbal",
     author_email="babak.zarrinbal@gmail.com",
```

### Comparing `http_file_streamer-0.1.1/src/http_file_streamer.egg-info/PKG-INFO` & `http_file_streamer-0.1.2/src/http_file_streamer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: http_file_streamer
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package for streaming and receiving files.
 Home-page: https://github.com/babakzarrinbal/httpfilestreamer.git
 Author: Babak Zarrinbal
 Author-email: babak.zarrinbal@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

