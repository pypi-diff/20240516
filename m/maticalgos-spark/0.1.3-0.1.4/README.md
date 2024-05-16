# Comparing `tmp/maticalgos-spark-0.1.3.tar.gz` & `tmp/maticalgos-spark-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maticalgos-spark-0.1.3.tar", last modified: Thu May 16 08:47:05 2024, max compression
+gzip compressed data, was "maticalgos-spark-0.1.4.tar", last modified: Thu May 16 08:59:45 2024, max compression
```

## Comparing `maticalgos-spark-0.1.3.tar` & `maticalgos-spark-0.1.4.tar`

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
+drwxrwxrwx   0        0        0        0 2024-05-16 08:59:45.331716 maticalgos-spark-0.1.4/
+-rw-rw-rw-   0        0        0      241 2024-05-16 08:21:15.000000 maticalgos-spark-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    34971 2024-05-16 08:59:45.331716 maticalgos-spark-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0    34444 2024-05-16 08:58:21.000000 maticalgos-spark-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 08:59:45.326497 maticalgos-spark-0.1.4/maticalgos_spark.egg-info/
+-rw-rw-rw-   0        0        0    34971 2024-05-16 08:59:45.000000 maticalgos-spark-0.1.4/maticalgos_spark.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2024-05-16 08:59:45.000000 maticalgos-spark-0.1.4/maticalgos_spark.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 08:59:45.000000 maticalgos-spark-0.1.4/maticalgos_spark.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-16 08:59:45.000000 maticalgos-spark-0.1.4/maticalgos_spark.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 08:59:45.326497 maticalgos-spark-0.1.4/maticalgospy/
+-rw-rw-rw-   0        0        0       45 2024-05-16 08:57:44.000000 maticalgos-spark-0.1.4/maticalgospy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 08:59:45.331716 maticalgos-spark-0.1.4/maticalgospy/sparkLib/
+-rw-rw-rw-   0        0        0       72 2024-05-16 07:33:27.000000 maticalgos-spark-0.1.4/maticalgospy/sparkLib/__init__.py
+-rw-rw-rw-   0        0        0     4206 2024-05-16 07:20:34.000000 maticalgos-spark-0.1.4/maticalgospy/sparkLib/order_websocket.py
+-rw-rw-rw-   0        0        0    19695 2024-05-16 08:42:53.000000 maticalgos-spark-0.1.4/maticalgospy/sparkLib/sparkLib.py
+-rw-rw-rw-   0        0        0       58 2024-05-16 07:20:34.000000 maticalgos-spark-0.1.4/requirementx.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 08:59:45.331716 maticalgos-spark-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      763 2024-05-16 08:59:33.000000 maticalgos-spark-0.1.4/setup.py
+-rw-rw-rw-   0        0        0      739 2024-05-16 08:42:59.000000 maticalgos-spark-0.1.4/testWS.py
```

### Comparing `maticalgos-spark-0.1.3/PKG-INFO` & `maticalgos-spark-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: maticalgos-spark
-Version: 0.1.3
+Version: 0.1.4
 Summary: SparkLib is a Python client library for interacting with https://spark.maticalgos.com . It provides functionalities to manage accounts, strategies, place orders, and much more.
-Author: MaticAlgos
+Author: Niraj Munot
 Author-email: nirajmunot28@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
@@ -123,15 +123,15 @@
 
 
 ## Getting an Access Token
 
 1. **Import the Spark library**
 
 ```python
-from maticalgos import SparkLib, order_websocket
+from maticalgospy import SparkLib, order_websocket
 ```
 
 2. **Create a Spark object**
 ```python
 spark_object = SparkLib(userid = "Your Emailid", 
                          password = "Your Password")
 
@@ -702,15 +702,15 @@
 - **Continuous Monitoring**: The websocket continuously listens for incoming order messages, ensuring that users are always up-to-date with their trading activity.
 
 ### Usage:
 To use the order websocket, users need to establish a connection to the Spark platform using their access token. Once connected, the websocket will start receiving order messages from the platform. Users can define callback functions to handle incoming order messages, error notifications, connection status changes, and more.
 
 ### Sample Code:
 ```python
-from maticalgos import SparkLib, order_websocket
+from maticalgospy import SparkLib, order_websocket
 
 # Define callback functions
 def on_order(message):
     print('Order', message)
 
 def on_error(error):
     print('Error', error)
```

### Comparing `maticalgos-spark-0.1.3/README.md` & `maticalgos-spark-0.1.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 
 
 ## Getting an Access Token
 
 1. **Import the Spark library**
 
 ```python
-from maticalgos import SparkLib, order_websocket
+from maticalgospy import SparkLib, order_websocket
 ```
 
 2. **Create a Spark object**
 ```python
 spark_object = SparkLib(userid = "Your Emailid", 
                          password = "Your Password")
 
@@ -690,15 +690,15 @@
 - **Continuous Monitoring**: The websocket continuously listens for incoming order messages, ensuring that users are always up-to-date with their trading activity.
 
 ### Usage:
 To use the order websocket, users need to establish a connection to the Spark platform using their access token. Once connected, the websocket will start receiving order messages from the platform. Users can define callback functions to handle incoming order messages, error notifications, connection status changes, and more.
 
 ### Sample Code:
 ```python
-from maticalgos import SparkLib, order_websocket
+from maticalgospy import SparkLib, order_websocket
 
 # Define callback functions
 def on_order(message):
     print('Order', message)
 
 def on_error(error):
     print('Error', error)
```

### Comparing `maticalgos-spark-0.1.3/maticalgos/sparkLib/order_websocket.py` & `maticalgos-spark-0.1.4/maticalgospy/sparkLib/order_websocket.py`

 * *Files identical despite different names*

### Comparing `maticalgos-spark-0.1.3/maticalgos/sparkLib/sparkLib.py` & `maticalgos-spark-0.1.4/maticalgospy/sparkLib/sparkLib.py`

 * *Files identical despite different names*

### Comparing `maticalgos-spark-0.1.3/maticalgos_spark.egg-info/PKG-INFO` & `maticalgos-spark-0.1.4/maticalgos_spark.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: maticalgos-spark
-Version: 0.1.3
+Version: 0.1.4
 Summary: SparkLib is a Python client library for interacting with https://spark.maticalgos.com . It provides functionalities to manage accounts, strategies, place orders, and much more.
-Author: MaticAlgos
+Author: Niraj Munot
 Author-email: nirajmunot28@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
@@ -123,15 +123,15 @@
 
 
 ## Getting an Access Token
 
 1. **Import the Spark library**
 
 ```python
-from maticalgos import SparkLib, order_websocket
+from maticalgospy import SparkLib, order_websocket
 ```
 
 2. **Create a Spark object**
 ```python
 spark_object = SparkLib(userid = "Your Emailid", 
                          password = "Your Password")
 
@@ -702,15 +702,15 @@
 - **Continuous Monitoring**: The websocket continuously listens for incoming order messages, ensuring that users are always up-to-date with their trading activity.
 
 ### Usage:
 To use the order websocket, users need to establish a connection to the Spark platform using their access token. Once connected, the websocket will start receiving order messages from the platform. Users can define callback functions to handle incoming order messages, error notifications, connection status changes, and more.
 
 ### Sample Code:
 ```python
-from maticalgos import SparkLib, order_websocket
+from maticalgospy import SparkLib, order_websocket
 
 # Define callback functions
 def on_order(message):
     print('Order', message)
 
 def on_error(error):
     print('Error', error)
```

### Comparing `maticalgos-spark-0.1.3/setup.py` & `maticalgos-spark-0.1.4/setup.py`

 * *Files 19% similar despite different names*

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
+version='0.1.4',
+author='Niraj Munot',
 author_email='nirajmunot28@gmail.com',
 description='SparkLib is a Python client library for interacting with https://spark.maticalgos.com . It provides functionalities to manage accounts, strategies, place orders, and much more.',
 long_description=long_description,
 long_description_content_type='text/markdown',
 packages=find_packages(),
 classifiers=[
 'Programming Language :: Python :: 3',
```

### Comparing `maticalgos-spark-0.1.3/testWS.py` & `maticalgos-spark-0.1.4/testWS.py`

 * *Files identical despite different names*

