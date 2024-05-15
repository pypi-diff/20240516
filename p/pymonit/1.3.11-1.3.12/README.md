# Comparing `tmp/pymonit-1.3.11.tar.gz` & `tmp/pymonit-1.3.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymonit-1.3.11.tar", last modified: Wed May 15 21:46:57 2024, max compression
+gzip compressed data, was "pymonit-1.3.12.tar", last modified: Wed May 15 22:02:45 2024, max compression
```

## Comparing `pymonit-1.3.11.tar` & `pymonit-1.3.12.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-15 21:46:57.739262 pymonit-1.3.11/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1064 2024-04-22 01:06:10.000000 pymonit-1.3.11/LICENSE
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2381 2024-05-15 21:46:57.739262 pymonit-1.3.11/PKG-INFO
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1745 2024-05-15 21:46:52.000000 pymonit-1.3.11/README.md
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-15 21:46:57.735929 pymonit-1.3.11/monit/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:06:10.000000 pymonit-1.3.11/monit/__init__.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      922 2024-04-30 01:09:27.000000 pymonit-1.3.11/monit/config.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      839 2024-05-15 21:03:06.000000 pymonit-1.3.11/monit/core.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1592 2024-04-30 01:09:10.000000 pymonit-1.3.11/monit/database.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      227 2024-04-25 22:34:06.000000 pymonit-1.3.11/monit/error.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     3145 2024-04-30 18:33:49.000000 pymonit-1.3.11/monit/func.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1831 2024-04-22 23:15:08.000000 pymonit-1.3.11/monit/log2file.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2569 2024-04-22 23:04:24.000000 pymonit-1.3.11/monit/logger.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      272 2024-04-26 01:39:16.000000 pymonit-1.3.11/monit/verify_env.py
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-15 21:46:57.739262 pymonit-1.3.11/pymonit.egg-info/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2381 2024-05-15 21:46:57.000000 pymonit-1.3.11/pymonit.egg-info/PKG-INFO
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      329 2024-05-15 21:46:57.000000 pymonit-1.3.11/pymonit.egg-info/SOURCES.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        1 2024-05-15 21:46:57.000000 pymonit-1.3.11/pymonit.egg-info/dependency_links.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-05-15 21:46:57.000000 pymonit-1.3.11/pymonit.egg-info/requires.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        6 2024-05-15 21:46:57.000000 pymonit-1.3.11/pymonit.egg-info/top_level.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       38 2024-05-15 21:46:57.739262 pymonit-1.3.11/setup.cfg
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      866 2024-05-15 21:44:01.000000 pymonit-1.3.11/setup.py
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-15 22:02:45.752447 pymonit-1.3.12/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1064 2024-04-22 01:06:10.000000 pymonit-1.3.12/LICENSE
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2398 2024-05-15 22:02:45.752447 pymonit-1.3.12/PKG-INFO
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1762 2024-05-15 22:01:11.000000 pymonit-1.3.12/README.md
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-15 22:02:45.749113 pymonit-1.3.12/pymonit/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:06:10.000000 pymonit-1.3.12/pymonit/__init__.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      922 2024-04-30 01:09:27.000000 pymonit-1.3.12/pymonit/config.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      788 2024-05-15 21:57:36.000000 pymonit-1.3.12/pymonit/core.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1594 2024-05-15 21:54:39.000000 pymonit-1.3.12/pymonit/database.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      227 2024-04-25 22:34:06.000000 pymonit-1.3.12/pymonit/error.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     3147 2024-05-15 21:54:50.000000 pymonit-1.3.12/pymonit/func.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1831 2024-04-22 23:15:08.000000 pymonit-1.3.12/pymonit/log2file.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2569 2024-04-22 23:04:24.000000 pymonit-1.3.12/pymonit/logger.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      272 2024-05-15 21:55:05.000000 pymonit-1.3.12/pymonit/verify_env.py
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-15 22:02:45.752447 pymonit-1.3.12/pymonit.egg-info/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2398 2024-05-15 22:02:45.000000 pymonit-1.3.12/pymonit.egg-info/PKG-INFO
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      347 2024-05-15 22:02:45.000000 pymonit-1.3.12/pymonit.egg-info/SOURCES.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        1 2024-05-15 22:02:45.000000 pymonit-1.3.12/pymonit.egg-info/dependency_links.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-05-15 22:02:45.000000 pymonit-1.3.12/pymonit.egg-info/requires.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        8 2024-05-15 22:02:45.000000 pymonit-1.3.12/pymonit.egg-info/top_level.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       38 2024-05-15 22:02:45.752447 pymonit-1.3.12/setup.cfg
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      866 2024-05-15 22:02:02.000000 pymonit-1.3.12/setup.py
```

### Comparing `pymonit-1.3.11/LICENSE` & `pymonit-1.3.12/LICENSE`

 * *Files identical despite different names*

### Comparing `pymonit-1.3.11/PKG-INFO` & `pymonit-1.3.12/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymonit
-Version: 1.3.11
+Version: 1.3.12
 Summary: Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados
 Home-page: https://github.com/arktnld/monit
 Author: arktnld
 Author-email: arktnld@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -45,16 +45,16 @@
 ```
 ### Exemplo de Uso:
 
 **Utilização do Monit para notificação de erros**
 ```python
 import time
 
-from monit.core import Monitor as monit
-from monit.error import SetupError
+from pymonit.core import Monitor as monit
+from pymonit.error import SetupError
 
 def main():
 
     try:
         time.sleep(5)
         raise ValueError("This is a sample error.")
 
@@ -71,16 +71,16 @@
 não são grandes o suficientes para exigir que o
 processo seja interrompido.**
 
 ```Python
 # sample.py
 import time
 
-from monit.core import Monitor
-from monit.error import SetupError
+from pymonit.core import Monitor as monit
+from pymonit.error import SetupError
 # from monit.logger import Logger
 # from monit.log2file import Log2File
 
 def main():
     # Initialize the Monitor
     monit = Monitor()
```

### Comparing `pymonit-1.3.11/README.md` & `pymonit-1.3.12/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 ```
 ### Exemplo de Uso:
 
 **Utilização do Monit para notificação de erros**
 ```python
 import time
 
-from monit.core import Monitor as monit
-from monit.error import SetupError
+from pymonit.core import Monitor as monit
+from pymonit.error import SetupError
 
 def main():
 
     try:
         time.sleep(5)
         raise ValueError("This is a sample error.")
 
@@ -52,16 +52,16 @@
 não são grandes o suficientes para exigir que o
 processo seja interrompido.**
 
 ```Python
 # sample.py
 import time
 
-from monit.core import Monitor
-from monit.error import SetupError
+from pymonit.core import Monitor as monit
+from pymonit.error import SetupError
 # from monit.logger import Logger
 # from monit.log2file import Log2File
 
 def main():
     # Initialize the Monitor
     monit = Monitor()
```

### Comparing `pymonit-1.3.11/monit/config.py` & `pymonit-1.3.12/pymonit/config.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.3.11/monit/core.py` & `pymonit-1.3.12/pymonit/core.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from datetime import datetime
 import sys
 import os
 
-from monit import config
-from monit import func
-from monit.database import Database, Table
-from monit.verify_env import verify_env
+from pymonit import config
+from pymonit import func
+from pymonit.database import Database, Table
+from pymonit.verify_env import verify_env
 
 # Ensure .env is loaded
 verify_env()
 
 # Get the initial time
 INIT_TIME = datetime.now()
 
 class Monitor:
     TYPE = list()
     ERROR = list()
 
-    def register(self, type=None, error=None):
+    @staticmethod
+    def register(type=None, error=None):
         table = func.build_table(type, error, Table(), INIT_TIME)
         Database.insert(table)
 
-    def end(self):
-        # type = ', '.join(self.TYPE)
-        # error = ', '.join(self.ERROR)
-        self.register(None, None)
-
-    def notify(self, type=None, error=None):
-        self.TYPE.append(type)
-        self.ERROR.append(error)
+    @staticmethod
+    def end():
+        Monitor().register(None, None)
+
+    @staticmethod
+    def notify(type=None, error=None):
+        Monitor().register(type, error)
 
     @staticmethod
     def notify_and_exit(type=None, error=None):
         Monitor().register(type, error)
         sys.exit(1)
```

### Comparing `pymonit-1.3.11/monit/database.py` & `pymonit-1.3.12/pymonit/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from sqlalchemy import create_engine, Column, Integer, String, DateTime, Boolean, Text
 # from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import sessionmaker
 from datetime import datetime
 from sqlalchemy.orm import declarative_base
-from monit import config
+from pymonit import config
 
 Base = declarative_base()
 
 class Table(Base):
     __tablename__ = 'monit'
 
     id = Column(Integer, primary_key=True)
```

### Comparing `pymonit-1.3.11/monit/func.py` & `pymonit-1.3.12/pymonit/func.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import traceback
 from math import floor
 import platform
 from datetime import datetime
 import smtplib
 from email.message import EmailMessage
 
-from monit import config
+from pymonit import config
 
 
 def build_table(type, err, table, init_time):
 
         table.project = config.project
         table.company = config.company
         table.dev = config.dev
```

### Comparing `pymonit-1.3.11/monit/log2file.py` & `pymonit-1.3.12/pymonit/log2file.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.3.11/monit/logger.py` & `pymonit-1.3.12/pymonit/logger.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.3.11/pymonit.egg-info/PKG-INFO` & `pymonit-1.3.12/pymonit.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymonit
-Version: 1.3.11
+Version: 1.3.12
 Summary: Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados
 Home-page: https://github.com/arktnld/monit
 Author: arktnld
 Author-email: arktnld@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -45,16 +45,16 @@
 ```
 ### Exemplo de Uso:
 
 **Utilização do Monit para notificação de erros**
 ```python
 import time
 
-from monit.core import Monitor as monit
-from monit.error import SetupError
+from pymonit.core import Monitor as monit
+from pymonit.error import SetupError
 
 def main():
 
     try:
         time.sleep(5)
         raise ValueError("This is a sample error.")
 
@@ -71,16 +71,16 @@
 não são grandes o suficientes para exigir que o
 processo seja interrompido.**
 
 ```Python
 # sample.py
 import time
 
-from monit.core import Monitor
-from monit.error import SetupError
+from pymonit.core import Monitor as monit
+from pymonit.error import SetupError
 # from monit.logger import Logger
 # from monit.log2file import Log2File
 
 def main():
     # Initialize the Monitor
     monit = Monitor()
```

### Comparing `pymonit-1.3.11/setup.py` & `pymonit-1.3.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import pathlib
 
 setup(
     name='pymonit',
-    version='1.3.11',
+    version='1.3.12',
     description='Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados',
     long_description=pathlib.Path('README.md').read_text(),
     long_description_content_type='text/markdown',
     author='arktnld',
     author_email='arktnld@gmail.com',
     url='https://github.com/arktnld/monit',
     license='MIT',
```

