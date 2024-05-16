# Comparing `tmp/maticalgos-spark-0.1.0.tar.gz` & `tmp/maticalgos-spark-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maticalgos-spark-0.1.0.tar", last modified: Thu May 16 07:54:45 2024, max compression
+gzip compressed data, was "maticalgos-spark-0.1.1.tar", last modified: Thu May 16 08:03:41 2024, max compression
```

## Comparing `maticalgos-spark-0.1.0.tar` & `maticalgos-spark-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 07:54:45.320065 maticalgos-spark-0.1.0/
--rw-rw-rw-   0        0        0    35061 2024-05-16 07:54:45.320065 maticalgos-spark-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-16 07:54:45.309859 maticalgos-spark-0.1.0/maticalgos_spark.egg-info/
--rw-rw-rw-   0        0        0    35061 2024-05-16 07:54:45.000000 maticalgos-spark-0.1.0/maticalgos_spark.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2024-05-16 07:54:45.000000 maticalgos-spark-0.1.0/maticalgos_spark.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 07:54:45.000000 maticalgos-spark-0.1.0/maticalgos_spark.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-16 07:54:45.000000 maticalgos-spark-0.1.0/maticalgos_spark.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 07:54:45.323666 maticalgos-spark-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      757 2024-05-16 07:53:49.000000 maticalgos-spark-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 07:54:45.317568 maticalgos-spark-0.1.0/sparkLib/
--rw-rw-rw-   0        0        0       72 2024-05-16 07:33:27.000000 maticalgos-spark-0.1.0/sparkLib/__init__.py
--rw-rw-rw-   0        0        0     4206 2024-05-16 07:20:34.000000 maticalgos-spark-0.1.0/sparkLib/order_websocket.py
--rw-rw-rw-   0        0        0    19695 2024-05-16 07:33:15.000000 maticalgos-spark-0.1.0/sparkLib/sparkLib.py
+drwxrwxrwx   0        0        0        0 2024-05-16 08:03:41.365073 maticalgos-spark-0.1.1/
+-rw-rw-rw-   0        0        0    34957 2024-05-16 08:03:41.365073 maticalgos-spark-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-16 08:03:41.359162 maticalgos-spark-0.1.1/maticalgos_spark.egg-info/
+-rw-rw-rw-   0        0        0    34957 2024-05-16 08:03:41.000000 maticalgos-spark-0.1.1/maticalgos_spark.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-05-16 08:03:41.000000 maticalgos-spark-0.1.1/maticalgos_spark.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 08:03:41.000000 maticalgos-spark-0.1.1/maticalgos_spark.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-16 08:03:41.000000 maticalgos-spark-0.1.1/maticalgos_spark.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 08:03:41.367673 maticalgos-spark-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      757 2024-05-16 08:03:33.000000 maticalgos-spark-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 08:03:41.363708 maticalgos-spark-0.1.1/sparkLib/
+-rw-rw-rw-   0        0        0       72 2024-05-16 07:33:27.000000 maticalgos-spark-0.1.1/sparkLib/__init__.py
+-rw-rw-rw-   0        0        0     4206 2024-05-16 07:20:34.000000 maticalgos-spark-0.1.1/sparkLib/order_websocket.py
+-rw-rw-rw-   0        0        0    19695 2024-05-16 07:33:15.000000 maticalgos-spark-0.1.1/sparkLib/sparkLib.py
```

### Comparing `maticalgos-spark-0.1.0/PKG-INFO` & `maticalgos-spark-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: maticalgos-spark
-Version: 0.1.0
+Version: 0.1.1
 Summary: SparkLib is a Python client library for interacting with https://spark.maticalgos.com . It provides functionalities to manage accounts, strategies, place orders, and much more.
 Author: Niraj
 Author-email: nirajmunot28@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-# SparkLib - Matic Algos Python Client
+# SparkLib - MaticAlgos Python Client
 
 SparkLib is a Python client library for interacting with https://spark.maticalgos.com . It provides functionalities to manage accounts, strategies, place orders, and much more.
 
 ## Installation
 
 You can install the pre release via pip
 
 ```
-pip install SparkLib
+pip install maticalgos-spark
 ```
 
 <!-- # Basic Introduction to Spark by MaticAlgos
 ## Spark Platform: Empowering Multi-Account Trading with Diverse Strategies -->
 
 <!-- At SparkMatic, our main aim is to revolutionize the landscape of algorithmic trading by offering a comprehensive platform that enables traders to execute strategies across multiple accounts seamlessly. With our innovative approach, traders can harness the power of diverse trading strategies, allocate varying amounts of capital, and utilize custom multipliers to optimize their trading performance.
 
@@ -40,53 +40,53 @@
 5. **Order Slicing:** In addition to multi-account trading, SparkMatic offers advanced order slicing capabilities, allowing traders to split large orders into smaller segments and execute them gradually. By breaking down big orders into manageable chunks, traders can minimize market impact, improve execution quality, and enhance overall trading performance.
 
 With SparkMatic, traders can take their algorithmic trading strategies to the next level, leveraging cutting-edge technology and sophisticated tools to achieve their financial goals with confidence and precision. -->
 
 
 # Setup Guide
 
-Follow these steps to set up and start trading with Spark Matic Algos:
+Follow these steps to set up and start trading with Spark:
 
 ## Prerequisites for Trading
 
-Before you can begin trading on Spark Matic Algos, ensure you've completed the following steps:
+Before you can begin trading on Spark, ensure you've completed the following steps:
 
 1. **Account Creation**:
-   - Sign up for an account on [Spark Matic Algos](https://spark.maticalgos.com/login).
+   - Sign up for an account on [Spark](https://spark.maticalgos.com/login).
 
 2. **Broker Account Setup**:
    - Have an active broker account with one of the supported brokers.
 
 3. **Connection Establishment**:
-   - Connect your broker account to Spark Matic Algos seamlessly.
+   - Connect your broker account to Spark seamlessly.
 
 4. **Strategy Creation**:
-   - Develop your trading strategy within the Spark Matic Algos platform.
+   - Develop your trading strategy within the Spark platform.
 
 5. **Strategy Linking**:
-   - Associate your created strategy with your broker account on Spark Matic Algos.
+   - Associate your created strategy with your broker account on Spark.
 
 6. **Strategy Activation**:
-   - Activate your linked strategy within the Spark Matic Algos interface.
+   - Activate your linked strategy within the Spark interface.
 
 7. **Trading Activation**:
-   - Enable trading on your broker account within Spark Matic Algos by specifying the Capital Deployed and Multiplier.
+   - Enable trading on your broker account within Spark by specifying the Capital Deployed and Multiplier.
 
 8. **Access Token Generation**:
    - Generate an access token to initiate trading activities securely.
 
 9. **Commence Trading**:
-   - Once all setup steps are completed, you're ready to commence trading using Spark Matic Algos.
+   - Once all setup steps are completed, you're ready to commence trading using Spark.
 
 
 
 ## Control Flow
 
 1. **Login to Your Account**
-   - Visit [Spark Matic Algos](https://spark.maticalgos.com/login) and log in using your user ID and password.
+   - Visit [Spark](https://spark.maticalgos.com/login) and log in using your user ID and password.
 
 2. **Add a Broker Account**
    - Navigate to 'Connections' -> 'ACCOUNTS' -> 'Add Account'.
    - Choose your preferred broker.
    - Provide a unique account name and your client ID.
    - Optionally, add your Telegram bot key and chat ID.
    - Click on 'Add Account'.
@@ -113,25 +113,25 @@
    - Navigate to 'Connections' -> 'ACCOUNTS'.
    - Generate an access token by clicking on 'Generate Token' for the respective account.
    - Click on the 'Trade' button for the respective account.
    - Choose the strategy name and click on 'Activate Now'.
 
 ## Getting API Keys
 api key is unique for each and every account.
-1. Login to yout Matic Algos [account](https://spark.maticalgos.com/login).
+1. Login to your Spark [account](https://spark.maticalgos.com/login).
 1. Click on 'Account Name' -> 'Settings'.
 1. Copy the 'App Key'. You will need this to generate a session ID.
 
 
 ## Getting an Access Token
 
 1. **Import the Spark library**
 
 ```python
-from sparkLib import SparkLib
+from sparkLib import SparkLib, order_websocket
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
-from Sparklib.order_websocket import OrderSocket
+from sparkLib import SparkLib, order_websocket
 
 # Define callback functions
 def on_order(message):
     print('Order', message)
 
 def on_error(error):
     print('Error', error)
```

### Comparing `maticalgos-spark-0.1.0/maticalgos_spark.egg-info/PKG-INFO` & `maticalgos-spark-0.1.1/maticalgos_spark.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: maticalgos-spark
-Version: 0.1.0
+Version: 0.1.1
 Summary: SparkLib is a Python client library for interacting with https://spark.maticalgos.com . It provides functionalities to manage accounts, strategies, place orders, and much more.
 Author: Niraj
 Author-email: nirajmunot28@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-# SparkLib - Matic Algos Python Client
+# SparkLib - MaticAlgos Python Client
 
 SparkLib is a Python client library for interacting with https://spark.maticalgos.com . It provides functionalities to manage accounts, strategies, place orders, and much more.
 
 ## Installation
 
 You can install the pre release via pip
 
 ```
-pip install SparkLib
+pip install maticalgos-spark
 ```
 
 <!-- # Basic Introduction to Spark by MaticAlgos
 ## Spark Platform: Empowering Multi-Account Trading with Diverse Strategies -->
 
 <!-- At SparkMatic, our main aim is to revolutionize the landscape of algorithmic trading by offering a comprehensive platform that enables traders to execute strategies across multiple accounts seamlessly. With our innovative approach, traders can harness the power of diverse trading strategies, allocate varying amounts of capital, and utilize custom multipliers to optimize their trading performance.
 
@@ -40,53 +40,53 @@
 5. **Order Slicing:** In addition to multi-account trading, SparkMatic offers advanced order slicing capabilities, allowing traders to split large orders into smaller segments and execute them gradually. By breaking down big orders into manageable chunks, traders can minimize market impact, improve execution quality, and enhance overall trading performance.
 
 With SparkMatic, traders can take their algorithmic trading strategies to the next level, leveraging cutting-edge technology and sophisticated tools to achieve their financial goals with confidence and precision. -->
 
 
 # Setup Guide
 
-Follow these steps to set up and start trading with Spark Matic Algos:
+Follow these steps to set up and start trading with Spark:
 
 ## Prerequisites for Trading
 
-Before you can begin trading on Spark Matic Algos, ensure you've completed the following steps:
+Before you can begin trading on Spark, ensure you've completed the following steps:
 
 1. **Account Creation**:
-   - Sign up for an account on [Spark Matic Algos](https://spark.maticalgos.com/login).
+   - Sign up for an account on [Spark](https://spark.maticalgos.com/login).
 
 2. **Broker Account Setup**:
    - Have an active broker account with one of the supported brokers.
 
 3. **Connection Establishment**:
-   - Connect your broker account to Spark Matic Algos seamlessly.
+   - Connect your broker account to Spark seamlessly.
 
 4. **Strategy Creation**:
-   - Develop your trading strategy within the Spark Matic Algos platform.
+   - Develop your trading strategy within the Spark platform.
 
 5. **Strategy Linking**:
-   - Associate your created strategy with your broker account on Spark Matic Algos.
+   - Associate your created strategy with your broker account on Spark.
 
 6. **Strategy Activation**:
-   - Activate your linked strategy within the Spark Matic Algos interface.
+   - Activate your linked strategy within the Spark interface.
 
 7. **Trading Activation**:
-   - Enable trading on your broker account within Spark Matic Algos by specifying the Capital Deployed and Multiplier.
+   - Enable trading on your broker account within Spark by specifying the Capital Deployed and Multiplier.
 
 8. **Access Token Generation**:
    - Generate an access token to initiate trading activities securely.
 
 9. **Commence Trading**:
-   - Once all setup steps are completed, you're ready to commence trading using Spark Matic Algos.
+   - Once all setup steps are completed, you're ready to commence trading using Spark.
 
 
 
 ## Control Flow
 
 1. **Login to Your Account**
-   - Visit [Spark Matic Algos](https://spark.maticalgos.com/login) and log in using your user ID and password.
+   - Visit [Spark](https://spark.maticalgos.com/login) and log in using your user ID and password.
 
 2. **Add a Broker Account**
    - Navigate to 'Connections' -> 'ACCOUNTS' -> 'Add Account'.
    - Choose your preferred broker.
    - Provide a unique account name and your client ID.
    - Optionally, add your Telegram bot key and chat ID.
    - Click on 'Add Account'.
@@ -113,25 +113,25 @@
    - Navigate to 'Connections' -> 'ACCOUNTS'.
    - Generate an access token by clicking on 'Generate Token' for the respective account.
    - Click on the 'Trade' button for the respective account.
    - Choose the strategy name and click on 'Activate Now'.
 
 ## Getting API Keys
 api key is unique for each and every account.
-1. Login to yout Matic Algos [account](https://spark.maticalgos.com/login).
+1. Login to your Spark [account](https://spark.maticalgos.com/login).
 1. Click on 'Account Name' -> 'Settings'.
 1. Copy the 'App Key'. You will need this to generate a session ID.
 
 
 ## Getting an Access Token
 
 1. **Import the Spark library**
 
 ```python
-from sparkLib import SparkLib
+from sparkLib import SparkLib, order_websocket
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
-from Sparklib.order_websocket import OrderSocket
+from sparkLib import SparkLib, order_websocket
 
 # Define callback functions
 def on_order(message):
     print('Order', message)
 
 def on_error(error):
     print('Error', error)
```

### Comparing `maticalgos-spark-0.1.0/setup.py` & `maticalgos-spark-0.1.1/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "readme.md").read_text()
 
 setup(
 name='maticalgos-spark',
-version='0.1.0',
+version='0.1.1',
 author='Niraj',
 author_email='nirajmunot28@gmail.com',
 description='SparkLib is a Python client library for interacting with https://spark.maticalgos.com . It provides functionalities to manage accounts, strategies, place orders, and much more.',
 long_description=long_description,
 long_description_content_type='text/markdown',
 packages=find_packages(),
 classifiers=[
```

### Comparing `maticalgos-spark-0.1.0/sparkLib/order_websocket.py` & `maticalgos-spark-0.1.1/sparkLib/order_websocket.py`

 * *Files identical despite different names*

### Comparing `maticalgos-spark-0.1.0/sparkLib/sparkLib.py` & `maticalgos-spark-0.1.1/sparkLib/sparkLib.py`

 * *Files identical despite different names*

