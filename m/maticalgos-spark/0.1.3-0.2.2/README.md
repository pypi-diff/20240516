# Comparing `tmp/maticalgos-spark-0.1.3.tar.gz` & `tmp/maticalgos-spark-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maticalgos-spark-0.1.3.tar", last modified: Thu May 16 08:47:05 2024, max compression
+gzip compressed data, was "maticalgos-spark-0.2.2.tar", last modified: Thu May 16 08:52:23 2024, max compression
```

## Comparing `maticalgos-spark-0.1.3.tar` & `maticalgos-spark-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 08:47:05.501586 maticalgos-spark-0.1.3/
--rw-rw-rw-   0        0        0      241 2024-05-16 08:21:15.000000 maticalgos-spark-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0    34966 2024-05-16 08:47:05.501586 maticalgos-spark-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0    34440 2024-05-16 08:46:39.000000 maticalgos-spark-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 08:47:05.476201 maticalgos-spark-0.1.3/maticalgos/
--rw-rw-rw-   0        0        0       45 2024-05-16 08:45:35.000000 maticalgos-spark-0.1.3/maticalgos/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 08:47:05.479810 maticalgos-spark-0.1.3/maticalgos/sparkLib/
--rw-rw-rw-   0        0        0       72 2024-05-16 07:33:27.000000 maticalgos-spark-0.1.3/maticalgos/sparkLib/__init__.py
--rw-rw-rw-   0        0        0     4206 2024-05-16 07:20:34.000000 maticalgos-spark-0.1.3/maticalgos/sparkLib/order_websocket.py
--rw-rw-rw-   0        0        0    19695 2024-05-16 08:42:53.000000 maticalgos-spark-0.1.3/maticalgos/sparkLib/sparkLib.py
-drwxrwxrwx   0        0        0        0 2024-05-16 08:47:05.499290 maticalgos-spark-0.1.3/maticalgos_spark.egg-info/
--rw-rw-rw-   0        0        0    34966 2024-05-16 08:47:05.000000 maticalgos-spark-0.1.3/maticalgos_spark.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      353 2024-05-16 08:47:05.000000 maticalgos-spark-0.1.3/maticalgos_spark.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 08:47:05.000000 maticalgos-spark-0.1.3/maticalgos_spark.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-16 08:47:05.000000 maticalgos-spark-0.1.3/maticalgos_spark.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       58 2024-05-16 07:20:34.000000 maticalgos-spark-0.1.3/requirementx.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 08:47:05.501586 maticalgos-spark-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      762 2024-05-16 08:39:13.000000 maticalgos-spark-0.1.3/setup.py
--rw-rw-rw-   0        0        0      739 2024-05-16 08:42:59.000000 maticalgos-spark-0.1.3/testWS.py
+drwxrwxrwx   0        0        0        0 2024-05-16 08:52:23.309285 maticalgos-spark-0.2.2/
+-rw-rw-rw-   0        0        0      241 2024-05-16 08:21:15.000000 maticalgos-spark-0.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    34967 2024-05-16 08:52:23.306372 maticalgos-spark-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0    34440 2024-05-16 08:46:39.000000 maticalgos-spark-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 08:52:23.292467 maticalgos-spark-0.2.2/maticalgos/
+-rw-rw-rw-   0        0        0       45 2024-05-16 08:45:35.000000 maticalgos-spark-0.2.2/maticalgos/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 08:52:23.297198 maticalgos-spark-0.2.2/maticalgos/sparkLib/
+-rw-rw-rw-   0        0        0       72 2024-05-16 07:33:27.000000 maticalgos-spark-0.2.2/maticalgos/sparkLib/__init__.py
+-rw-rw-rw-   0        0        0     4206 2024-05-16 07:20:34.000000 maticalgos-spark-0.2.2/maticalgos/sparkLib/order_websocket.py
+-rw-rw-rw-   0        0        0    19695 2024-05-16 08:42:53.000000 maticalgos-spark-0.2.2/maticalgos/sparkLib/sparkLib.py
+drwxrwxrwx   0        0        0        0 2024-05-16 08:52:23.306372 maticalgos-spark-0.2.2/maticalgos_spark.egg-info/
+-rw-rw-rw-   0        0        0    34967 2024-05-16 08:52:23.000000 maticalgos-spark-0.2.2/maticalgos_spark.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      353 2024-05-16 08:52:23.000000 maticalgos-spark-0.2.2/maticalgos_spark.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 08:52:23.000000 maticalgos-spark-0.2.2/maticalgos_spark.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-16 08:52:23.000000 maticalgos-spark-0.2.2/maticalgos_spark.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       58 2024-05-16 07:20:34.000000 maticalgos-spark-0.2.2/requirementx.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 08:52:23.309285 maticalgos-spark-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      763 2024-05-16 08:51:36.000000 maticalgos-spark-0.2.2/setup.py
+-rw-rw-rw-   0        0        0      739 2024-05-16 08:42:59.000000 maticalgos-spark-0.2.2/testWS.py
```

### Comparing `maticalgos-spark-0.1.3/PKG-INFO` & `maticalgos-spark-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: maticalgos-spark
-Version: 0.1.3
+Version: 0.2.2
 Summary: SparkLib is a Python client library for interacting with https://spark.maticalgos.com . It provides functionalities to manage accounts, strategies, place orders, and much more.
-Author: MaticAlgos
+Author: Niraj Munot
 Author-email: nirajmunot28@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `maticalgos-spark-0.1.3/README.md` & `maticalgos-spark-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `maticalgos-spark-0.1.3/maticalgos/sparkLib/order_websocket.py` & `maticalgos-spark-0.2.2/maticalgos/sparkLib/order_websocket.py`

 * *Files identical despite different names*

### Comparing `maticalgos-spark-0.1.3/maticalgos/sparkLib/sparkLib.py` & `maticalgos-spark-0.2.2/maticalgos/sparkLib/sparkLib.py`

 * *Files identical despite different names*

### Comparing `maticalgos-spark-0.1.3/maticalgos_spark.egg-info/PKG-INFO` & `maticalgos-spark-0.2.2/maticalgos_spark.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: maticalgos-spark
-Version: 0.1.3
+Version: 0.2.2
 Summary: SparkLib is a Python client library for interacting with https://spark.maticalgos.com . It provides functionalities to manage accounts, strategies, place orders, and much more.
-Author: MaticAlgos
+Author: Niraj Munot
 Author-email: nirajmunot28@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `maticalgos-spark-0.1.3/setup.py` & `maticalgos-spark-0.2.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "readme.md").read_text()
 
 setup(
 name='maticalgos-spark',
-version='0.1.3',
-author='MaticAlgos',
+version='0.2.2',
+author='Niraj Munot',
 author_email='nirajmunot28@gmail.com',
 description='SparkLib is a Python client library for interacting with https://spark.maticalgos.com . It provides functionalities to manage accounts, strategies, place orders, and much more.',
 long_description=long_description,
 long_description_content_type='text/markdown',
 packages=find_packages(),
 classifiers=[
 'Programming Language :: Python :: 3',
```

### Comparing `maticalgos-spark-0.1.3/testWS.py` & `maticalgos-spark-0.2.2/testWS.py`

 * *Files identical despite different names*

