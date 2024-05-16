# Comparing `tmp/http_file_streamer-0.1.0.tar.gz` & `tmp/http_file_streamer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "http_file_streamer-0.1.0.tar", last modified: Thu May 16 11:35:41 2024, max compression
+gzip compressed data, was "http_file_streamer-0.1.1.tar", last modified: Thu May 16 11:53:46 2024, max compression
```

## Comparing `http_file_streamer-0.1.0.tar` & `http_file_streamer-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 11:35:41.446121 http_file_streamer-0.1.0/
--rw-rw-rw-   0        0        0     1093 2024-05-16 11:21:47.000000 http_file_streamer-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     2307 2024-05-16 11:35:41.445117 http_file_streamer-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1712 2024-05-16 11:29:23.000000 http_file_streamer-0.1.0/README.md
--rw-rw-rw-   0        0        0       97 2024-05-16 11:35:15.000000 http_file_streamer-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-16 11:35:41.446121 http_file_streamer-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      786 2024-05-16 11:34:39.000000 http_file_streamer-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 11:35:41.431699 http_file_streamer-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-16 11:35:41.444120 http_file_streamer-0.1.0/src/http_file_streamer.egg-info/
--rw-rw-rw-   0        0        0     2307 2024-05-16 11:35:41.000000 http_file_streamer-0.1.0/src/http_file_streamer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2024-05-16 11:35:41.000000 http_file_streamer-0.1.0/src/http_file_streamer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 11:35:41.000000 http_file_streamer-0.1.0/src/http_file_streamer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-16 11:35:41.000000 http_file_streamer-0.1.0/src/http_file_streamer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 11:35:41.000000 http_file_streamer-0.1.0/src/http_file_streamer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 11:53:46.591782 http_file_streamer-0.1.1/
+-rw-rw-rw-   0        0        0     1093 2024-05-16 11:21:47.000000 http_file_streamer-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2336 2024-05-16 11:53:46.590781 http_file_streamer-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1741 2024-05-16 11:52:27.000000 http_file_streamer-0.1.1/README.md
+-rw-rw-rw-   0        0        0       97 2024-05-16 11:35:15.000000 http_file_streamer-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-16 11:53:46.591782 http_file_streamer-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      786 2024-05-16 11:53:10.000000 http_file_streamer-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 11:53:46.582704 http_file_streamer-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-16 11:53:46.589783 http_file_streamer-0.1.1/src/http_file_streamer.egg-info/
+-rw-rw-rw-   0        0        0     2336 2024-05-16 11:53:46.000000 http_file_streamer-0.1.1/src/http_file_streamer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2024-05-16 11:53:46.000000 http_file_streamer-0.1.1/src/http_file_streamer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 11:53:46.000000 http_file_streamer-0.1.1/src/http_file_streamer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-16 11:53:46.000000 http_file_streamer-0.1.1/src/http_file_streamer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 11:53:46.000000 http_file_streamer-0.1.1/src/http_file_streamer.egg-info/top_level.txt
```

### Comparing `http_file_streamer-0.1.0/LICENSE` & `http_file_streamer-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `http_file_streamer-0.1.0/PKG-INFO` & `http_file_streamer-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: http_file_streamer
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for streaming and receiving files.
 Home-page: https://github.com/babakzarrinbal/httpfilestreamer.git
 Author: Babak Zarrinbal
 Author-email: babak.zarrinbal@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,25 +25,25 @@
 - Configurable logging.
 
 ## Installation
 
 You can install the package using `pip`:
 
 ```bash
-pip install my_streamer_package
+pip install http-file-streamer
 ```
 
 ## Usage
 
 ### Streamer
 
 The `Streamer` class is used to stream files to a specified URL.
 
 ```python
-from src import Streamer
+from http_file_streamer import Streamer
 import logging
 
 url = "http://example.com/upload"
 file_path = "/path/to/your/file.txt"
 metadata = {"key1": "value1", "key2": "value2"}
 
 streamer = Streamer(url, file_path, metadata=metadata, logging_level=logging.INFO)
@@ -54,15 +54,15 @@
 ```
 
 ### Receiver
 
 The `Receiver` class is used to receive files from a stream.
 
 ```python
-from src import Receiver
+from http_file_streamer import Receiver
 import logging
 
 headers = {"X-Metadata-key1": "value1", "X-Metadata-key2": "value2"}
 stream = some_stream_source()  # This should be an iterable yielding byte chunks
 
 receiver = Receiver(headers, stream, save_path="/path/to/save/file.txt", logging_level=logging.INFO)
```

### Comparing `http_file_streamer-0.1.0/README.md` & `http_file_streamer-0.1.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -10,25 +10,25 @@
 - Configurable logging.
 
 ## Installation
 
 You can install the package using `pip`:
 
 ```bash
-pip install my_streamer_package
+pip install http-file-streamer
 ```
 
 ## Usage
 
 ### Streamer
 
 The `Streamer` class is used to stream files to a specified URL.
 
 ```python
-from src import Streamer
+from http_file_streamer import Streamer
 import logging
 
 url = "http://example.com/upload"
 file_path = "/path/to/your/file.txt"
 metadata = {"key1": "value1", "key2": "value2"}
 
 streamer = Streamer(url, file_path, metadata=metadata, logging_level=logging.INFO)
@@ -39,15 +39,15 @@
 ```
 
 ### Receiver
 
 The `Receiver` class is used to receive files from a stream.
 
 ```python
-from src import Receiver
+from http_file_streamer import Receiver
 import logging
 
 headers = {"X-Metadata-key1": "value1", "X-Metadata-key2": "value2"}
 stream = some_stream_source()  # This should be an iterable yielding byte chunks
 
 receiver = Receiver(headers, stream, save_path="/path/to/save/file.txt", logging_level=logging.INFO)
```

### Comparing `http_file_streamer-0.1.0/setup.py` & `http_file_streamer-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="http_file_streamer",
-    version="0.1.0",
+    version="0.1.1",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     install_requires=[
         "requests",
     ],
     author="Babak Zarrinbal",
     author_email="babak.zarrinbal@gmail.com",
```

### Comparing `http_file_streamer-0.1.0/src/http_file_streamer.egg-info/PKG-INFO` & `http_file_streamer-0.1.1/src/http_file_streamer.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: http_file_streamer
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for streaming and receiving files.
 Home-page: https://github.com/babakzarrinbal/httpfilestreamer.git
 Author: Babak Zarrinbal
 Author-email: babak.zarrinbal@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,25 +25,25 @@
 - Configurable logging.
 
 ## Installation
 
 You can install the package using `pip`:
 
 ```bash
-pip install my_streamer_package
+pip install http-file-streamer
 ```
 
 ## Usage
 
 ### Streamer
 
 The `Streamer` class is used to stream files to a specified URL.
 
 ```python
-from src import Streamer
+from http_file_streamer import Streamer
 import logging
 
 url = "http://example.com/upload"
 file_path = "/path/to/your/file.txt"
 metadata = {"key1": "value1", "key2": "value2"}
 
 streamer = Streamer(url, file_path, metadata=metadata, logging_level=logging.INFO)
@@ -54,15 +54,15 @@
 ```
 
 ### Receiver
 
 The `Receiver` class is used to receive files from a stream.
 
 ```python
-from src import Receiver
+from http_file_streamer import Receiver
 import logging
 
 headers = {"X-Metadata-key1": "value1", "X-Metadata-key2": "value2"}
 stream = some_stream_source()  # This should be an iterable yielding byte chunks
 
 receiver = Receiver(headers, stream, save_path="/path/to/save/file.txt", logging_level=logging.INFO)
```

