# Comparing `tmp/pymonit-1.3.13.tar.gz` & `tmp/pymonit-1.3.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymonit-1.3.13.tar", last modified: Wed May 15 22:20:13 2024, max compression
+gzip compressed data, was "pymonit-1.3.14.tar", last modified: Wed May 15 22:43:22 2024, max compression
```

## Comparing `pymonit-1.3.13.tar` & `pymonit-1.3.14.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-15 22:20:13.145824 pymonit-1.3.13/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1064 2024-04-22 01:06:10.000000 pymonit-1.3.13/LICENSE
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2398 2024-05-15 22:20:13.145824 pymonit-1.3.13/PKG-INFO
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1762 2024-05-15 22:01:11.000000 pymonit-1.3.13/README.md
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-15 22:20:13.145824 pymonit-1.3.13/pymonit/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:06:10.000000 pymonit-1.3.13/pymonit/__init__.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      922 2024-04-30 01:09:27.000000 pymonit-1.3.13/pymonit/config.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      788 2024-05-15 21:57:36.000000 pymonit-1.3.13/pymonit/core.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1594 2024-05-15 21:54:39.000000 pymonit-1.3.13/pymonit/database.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      227 2024-04-25 22:34:06.000000 pymonit-1.3.13/pymonit/error.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     3147 2024-05-15 21:54:50.000000 pymonit-1.3.13/pymonit/func.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1831 2024-04-22 23:15:08.000000 pymonit-1.3.13/pymonit/log2file.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2569 2024-04-22 23:04:24.000000 pymonit-1.3.13/pymonit/logger.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      272 2024-05-15 21:55:05.000000 pymonit-1.3.13/pymonit/verify_env.py
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-15 22:20:13.145824 pymonit-1.3.13/pymonit.egg-info/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2398 2024-05-15 22:20:12.000000 pymonit-1.3.13/pymonit.egg-info/PKG-INFO
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      347 2024-05-15 22:20:13.000000 pymonit-1.3.13/pymonit.egg-info/SOURCES.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        1 2024-05-15 22:20:12.000000 pymonit-1.3.13/pymonit.egg-info/dependency_links.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-05-15 22:20:12.000000 pymonit-1.3.13/pymonit.egg-info/requires.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        8 2024-05-15 22:20:12.000000 pymonit-1.3.13/pymonit.egg-info/top_level.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       38 2024-05-15 22:20:13.145824 pymonit-1.3.13/setup.cfg
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      866 2024-05-15 22:17:54.000000 pymonit-1.3.13/setup.py
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-15 22:43:22.387285 pymonit-1.3.14/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1064 2024-04-22 01:06:10.000000 pymonit-1.3.14/LICENSE
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2390 2024-05-15 22:43:22.387285 pymonit-1.3.14/PKG-INFO
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1754 2024-05-15 22:37:05.000000 pymonit-1.3.14/README.md
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-15 22:43:22.387285 pymonit-1.3.14/monit/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:06:10.000000 pymonit-1.3.14/monit/__init__.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      922 2024-04-30 01:09:27.000000 pymonit-1.3.14/monit/config.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      780 2024-05-15 22:37:15.000000 pymonit-1.3.14/monit/core.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1592 2024-05-15 22:37:27.000000 pymonit-1.3.14/monit/database.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      227 2024-04-25 22:34:06.000000 pymonit-1.3.14/monit/error.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     3145 2024-05-15 22:37:36.000000 pymonit-1.3.14/monit/func.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1831 2024-04-22 23:15:08.000000 pymonit-1.3.14/monit/log2file.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2569 2024-04-22 23:04:24.000000 pymonit-1.3.14/monit/logger.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      272 2024-05-15 21:55:05.000000 pymonit-1.3.14/monit/verify_env.py
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-15 22:43:22.387285 pymonit-1.3.14/pymonit.egg-info/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2390 2024-05-15 22:43:22.000000 pymonit-1.3.14/pymonit.egg-info/PKG-INFO
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      329 2024-05-15 22:43:22.000000 pymonit-1.3.14/pymonit.egg-info/SOURCES.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        1 2024-05-15 22:43:22.000000 pymonit-1.3.14/pymonit.egg-info/dependency_links.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-05-15 22:43:22.000000 pymonit-1.3.14/pymonit.egg-info/requires.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        6 2024-05-15 22:43:22.000000 pymonit-1.3.14/pymonit.egg-info/top_level.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       38 2024-05-15 22:43:22.387285 pymonit-1.3.14/setup.cfg
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      866 2024-05-15 22:43:02.000000 pymonit-1.3.14/setup.py
```

### Comparing `pymonit-1.3.13/LICENSE` & `pymonit-1.3.14/LICENSE`

 * *Files identical despite different names*

### Comparing `pymonit-1.3.13/PKG-INFO` & `pymonit-1.3.14/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymonit
-Version: 1.3.13
+Version: 1.3.14
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
 
-from pymonit.core import Monitor as monit
-from pymonit.error import SetupError
+from monit.core import Monitor as monit
+from monit.error import SetupError
 
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
 
-from pymonit.core import Monitor as monit
-from pymonit.error import SetupError
+from monit.core import Monitor as monit
+from monit.error import SetupError
 # from monit.logger import Logger
 # from monit.log2file import Log2File
 
 def main():
     # Initialize the Monitor
     monit = Monitor()
```

### Comparing `pymonit-1.3.13/README.md` & `pymonit-1.3.14/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 ```
 ### Exemplo de Uso:
 
 **Utilização do Monit para notificação de erros**
 ```python
 import time
 
-from pymonit.core import Monitor as monit
-from pymonit.error import SetupError
+from monit.core import Monitor as monit
+from monit.error import SetupError
 
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
 
-from pymonit.core import Monitor as monit
-from pymonit.error import SetupError
+from monit.core import Monitor as monit
+from monit.error import SetupError
 # from monit.logger import Logger
 # from monit.log2file import Log2File
 
 def main():
     # Initialize the Monitor
     monit = Monitor()
```

### Comparing `pymonit-1.3.13/pymonit/config.py` & `pymonit-1.3.14/monit/config.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.3.13/pymonit/core.py` & `pymonit-1.3.14/monit/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from datetime import datetime
 import sys
 import os
 
-from pymonit import config
-from pymonit import func
-from pymonit.database import Database, Table
-from pymonit.verify_env import verify_env
+from monit import config
+from monit import func
+from monit.database import Database, Table
+from monit.verify_env import verify_env
 
 # Ensure .env is loaded
 verify_env()
 
 # Get the initial time
 INIT_TIME = datetime.now()
```

### Comparing `pymonit-1.3.13/pymonit/database.py` & `pymonit-1.3.14/monit/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from sqlalchemy import create_engine, Column, Integer, String, DateTime, Boolean, Text
 # from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import sessionmaker
 from datetime import datetime
 from sqlalchemy.orm import declarative_base
-from pymonit import config
+from monit import config
 
 Base = declarative_base()
 
 class Table(Base):
     __tablename__ = 'monit'
 
     id = Column(Integer, primary_key=True)
```

### Comparing `pymonit-1.3.13/pymonit/func.py` & `pymonit-1.3.14/monit/func.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import traceback
 from math import floor
 import platform
 from datetime import datetime
 import smtplib
 from email.message import EmailMessage
 
-from pymonit import config
+from monit import config
 
 
 def build_table(type, err, table, init_time):
 
         table.project = config.project
         table.company = config.company
         table.dev = config.dev
```

### Comparing `pymonit-1.3.13/pymonit/log2file.py` & `pymonit-1.3.14/monit/log2file.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.3.13/pymonit/logger.py` & `pymonit-1.3.14/monit/logger.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.3.13/pymonit.egg-info/PKG-INFO` & `pymonit-1.3.14/pymonit.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymonit
-Version: 1.3.13
+Version: 1.3.14
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
 
-from pymonit.core import Monitor as monit
-from pymonit.error import SetupError
+from monit.core import Monitor as monit
+from monit.error import SetupError
 
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
 
-from pymonit.core import Monitor as monit
-from pymonit.error import SetupError
+from monit.core import Monitor as monit
+from monit.error import SetupError
 # from monit.logger import Logger
 # from monit.log2file import Log2File
 
 def main():
     # Initialize the Monitor
     monit = Monitor()
```

### Comparing `pymonit-1.3.13/setup.py` & `pymonit-1.3.14/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import pathlib
 
 setup(
     name='pymonit',
-    version='1.3.13',
+    version='1.3.14',
     description='Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados',
     long_description=pathlib.Path('README.md').read_text(),
     long_description_content_type='text/markdown',
     author='arktnld',
     author_email='arktnld@gmail.com',
     url='https://github.com/arktnld/monit',
     license='MIT',
```

