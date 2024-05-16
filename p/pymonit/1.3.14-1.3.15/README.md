# Comparing `tmp/pymonit-1.3.14.tar.gz` & `tmp/pymonit-1.3.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymonit-1.3.14.tar", last modified: Wed May 15 22:43:22 2024, max compression
+gzip compressed data, was "pymonit-1.3.15.tar", last modified: Thu May 16 12:51:54 2024, max compression
```

## Comparing `pymonit-1.3.14.tar` & `pymonit-1.3.15.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-15 22:43:22.387285 pymonit-1.3.14/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1064 2024-04-22 01:06:10.000000 pymonit-1.3.14/LICENSE
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2390 2024-05-15 22:43:22.387285 pymonit-1.3.14/PKG-INFO
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1754 2024-05-15 22:37:05.000000 pymonit-1.3.14/README.md
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-15 22:43:22.387285 pymonit-1.3.14/monit/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:06:10.000000 pymonit-1.3.14/monit/__init__.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      922 2024-04-30 01:09:27.000000 pymonit-1.3.14/monit/config.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      780 2024-05-15 22:37:15.000000 pymonit-1.3.14/monit/core.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1592 2024-05-15 22:37:27.000000 pymonit-1.3.14/monit/database.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      227 2024-04-25 22:34:06.000000 pymonit-1.3.14/monit/error.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     3145 2024-05-15 22:37:36.000000 pymonit-1.3.14/monit/func.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1831 2024-04-22 23:15:08.000000 pymonit-1.3.14/monit/log2file.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2569 2024-04-22 23:04:24.000000 pymonit-1.3.14/monit/logger.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      272 2024-05-15 21:55:05.000000 pymonit-1.3.14/monit/verify_env.py
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-15 22:43:22.387285 pymonit-1.3.14/pymonit.egg-info/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2390 2024-05-15 22:43:22.000000 pymonit-1.3.14/pymonit.egg-info/PKG-INFO
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      329 2024-05-15 22:43:22.000000 pymonit-1.3.14/pymonit.egg-info/SOURCES.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        1 2024-05-15 22:43:22.000000 pymonit-1.3.14/pymonit.egg-info/dependency_links.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-05-15 22:43:22.000000 pymonit-1.3.14/pymonit.egg-info/requires.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        6 2024-05-15 22:43:22.000000 pymonit-1.3.14/pymonit.egg-info/top_level.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       38 2024-05-15 22:43:22.387285 pymonit-1.3.14/setup.cfg
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      866 2024-05-15 22:43:02.000000 pymonit-1.3.14/setup.py
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-16 12:51:54.224986 pymonit-1.3.15/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1064 2024-04-22 01:06:10.000000 pymonit-1.3.15/LICENSE
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2556 2024-05-16 12:51:54.224986 pymonit-1.3.15/PKG-INFO
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1920 2024-05-16 12:50:29.000000 pymonit-1.3.15/README.md
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-16 12:51:54.221653 pymonit-1.3.15/monit/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:06:10.000000 pymonit-1.3.15/monit/__init__.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      922 2024-04-30 01:09:27.000000 pymonit-1.3.15/monit/config.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      725 2024-05-16 12:44:15.000000 pymonit-1.3.15/monit/core.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1594 2024-05-16 12:44:25.000000 pymonit-1.3.15/monit/database.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      227 2024-04-25 22:34:06.000000 pymonit-1.3.15/monit/error.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     3128 2024-05-16 12:41:20.000000 pymonit-1.3.15/monit/func.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1831 2024-04-22 23:15:08.000000 pymonit-1.3.15/monit/log2file.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2569 2024-04-22 23:04:24.000000 pymonit-1.3.15/monit/logger.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      272 2024-05-15 21:55:05.000000 pymonit-1.3.15/monit/verify_env.py
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-16 12:51:54.224986 pymonit-1.3.15/pymonit.egg-info/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2556 2024-05-16 12:51:54.000000 pymonit-1.3.15/pymonit.egg-info/PKG-INFO
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      329 2024-05-16 12:51:54.000000 pymonit-1.3.15/pymonit.egg-info/SOURCES.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        1 2024-05-16 12:51:54.000000 pymonit-1.3.15/pymonit.egg-info/dependency_links.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-05-16 12:51:54.000000 pymonit-1.3.15/pymonit.egg-info/requires.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        6 2024-05-16 12:51:54.000000 pymonit-1.3.15/pymonit.egg-info/top_level.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       38 2024-05-16 12:51:54.224986 pymonit-1.3.15/setup.cfg
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      866 2024-05-16 12:50:53.000000 pymonit-1.3.15/setup.py
```

### Comparing `pymonit-1.3.14/LICENSE` & `pymonit-1.3.15/LICENSE`

 * *Files identical despite different names*

### Comparing `pymonit-1.3.14/PKG-INFO` & `pymonit-1.3.15/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymonit
-Version: 1.3.14
+Version: 1.3.15
 Summary: Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados
 Home-page: https://github.com/arktnld/monit
 Author: arktnld
 Author-email: arktnld@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -19,14 +19,18 @@
 
 ### Monit
 
 **Instalação:**
 ```bash
 pip install pymonit
 ```
+**Atualização:**
+```bash
+pip install -U pymonit
+```
 **Exemplo arquivo `.monit`:**
 ```bash
 # Project info
 # Informações obrigatórias
 PROJECT=sample_project
 COMPANY=acme
 DEV=coder
@@ -43,40 +47,57 @@
 EMAIL=
 EMAIL_PASSWORD=
 ```
 ### Exemplo de Uso:
 
 **Utilização do Monit para notificação de erros**
 ```python
+#
+#  IMPORTANTE: importar OS e entrar na pasta atual é obrigatório
+#
+import os
+
+script_path = os.path.abspath(__file__)
+os.chdir(os.path.dirname(script_path))
+
 import time
 
 from monit.core import Monitor as monit
 from monit.error import SetupError
 
 def main():
 
     try:
         time.sleep(5)
         raise ValueError("This is a sample error.")
 
     except Exception as e:
         print("Erro: Ocorreu um erro inesperado.")
-        monit.notify_and_exit(SetupError, e)
+        monit.notify_and_exit(e)
 
 
 if __name__ == "__main__":
     main()
 ```
 
 **Utilização do Monit para notificação de erros que
 não são grandes o suficientes para exigir que o
 processo seja interrompido.**
 
 ```Python
 # sample.py
+
+#
+#  IMPORTANTE: importar OS e entrar na pasta atual é obrigatório
+#
+import os
+
+script_path = os.path.abspath(__file__)
+os.chdir(os.path.dirname(script_path))
+
 import time
 
 from monit.core import Monitor as monit
 from monit.error import SetupError
 # from monit.logger import Logger
 # from monit.log2file import Log2File
 
@@ -90,28 +111,14 @@
     try:
         # Your code that might raise exceptions
         time.sleep(5)
         raise ValueError("This is a sample error.")
 
     except Exception as e:
         print("Erro: Ocorreu um erro inesperado.")
-        monit.notify(SetupError, e)
-        # monit.notify_and_exit(SetupError, e)
+        monit.notify(e)
 
     monit.end()
 
 
 if __name__ == "__main__":
     main()
-```
-**Tipos de erros:**
-```bash
-SetupError
-DatabaseError
-HTTPError
-FileError
-FolderError
-TooManyRequests
-DataCreateError
-DataUpdateError
-
-```
```

### Comparing `pymonit-1.3.14/monit/config.py` & `pymonit-1.3.15/monit/config.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.3.14/monit/database.py` & `pymonit-1.3.15/monit/database.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 class Table(Base):
     __tablename__ = 'monit'
 
     id = Column(Integer, primary_key=True)
     project = Column(String(255))
     company = Column(String(255))
     dev = Column(String(255))
-    type = Column(String(255))
+    # type = Column(String(255))
     stderr = Column(Boolean)
     error = Column(Text)
     runtime = Column(Integer)
     date_init = Column(DateTime)
     date_end = Column(DateTime)
     cpu = Column(String(255))
     mem = Column(String(255))
```

### Comparing `pymonit-1.3.14/monit/func.py` & `pymonit-1.3.15/monit/func.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from datetime import datetime
 import smtplib
 from email.message import EmailMessage
 
 from monit import config
 
 
-def build_table(type, err, table, init_time):
+def build_table(err, table, init_time):
 
         table.project = config.project
         table.company = config.company
         table.dev = config.dev
         table.stderr = bool(err)
 
         fim = datetime.now()
@@ -31,29 +31,29 @@
         table.disk = _get_disk_usage()
         table.ping = _ping_host()
         table.system = platform.system()
 
         if err:
             error = str(err).replace('\n', '')
 
-            table.type = type
+            # table.type = type
             table.error = error
 
-            _print_error_to_console(type, err)
+            _print_error_to_console(err)
             _send_email_notification(error)
 
         return table
 
-def _print_error_to_console(type, err):
+def _print_error_to_console(err):
     # Imprime o erro no console.
     if err:
         # error_type = type(err).__name__
         tb = traceback.extract_tb(err.__traceback__)
         filename, line, func, text = tb[-1]
-        strerror = f"File \"{filename}\", line {line}\n\t{text}\n\n{type}: {err}"
+        strerror = f"File \"{filename}\", line {line}\n\t{text}\n\nError: {err}"
         print(strerror)
 
 def _send_email_notification(err):
     # Envia um e-mail com o erro.
     if config.email and config.email_password:
         message = f"{config.company}\n{config.project}\n\n{err}"
```

### Comparing `pymonit-1.3.14/monit/log2file.py` & `pymonit-1.3.15/monit/log2file.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.3.14/monit/logger.py` & `pymonit-1.3.15/monit/logger.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.3.14/pymonit.egg-info/PKG-INFO` & `pymonit-1.3.15/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,17 @@
-Metadata-Version: 2.1
-Name: pymonit
-Version: 1.3.14
-Summary: Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados
-Home-page: https://github.com/arktnld/monit
-Author: arktnld
-Author-email: arktnld@gmail.com
-License: MIT
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: sqlalchemy
-Requires-Dist: pymysql
-Requires-Dist: psutil
-Requires-Dist: python-dotenv
-
 ### Monit
 
 **Instalação:**
 ```bash
 pip install pymonit
 ```
+**Atualização:**
+```bash
+pip install -U pymonit
+```
 **Exemplo arquivo `.monit`:**
 ```bash
 # Project info
 # Informações obrigatórias
 PROJECT=sample_project
 COMPANY=acme
 DEV=coder
@@ -43,40 +28,57 @@
 EMAIL=
 EMAIL_PASSWORD=
 ```
 ### Exemplo de Uso:
 
 **Utilização do Monit para notificação de erros**
 ```python
+#
+#  IMPORTANTE: importar OS e entrar na pasta atual é obrigatório
+#
+import os
+
+script_path = os.path.abspath(__file__)
+os.chdir(os.path.dirname(script_path))
+
 import time
 
 from monit.core import Monitor as monit
 from monit.error import SetupError
 
 def main():
 
     try:
         time.sleep(5)
         raise ValueError("This is a sample error.")
 
     except Exception as e:
         print("Erro: Ocorreu um erro inesperado.")
-        monit.notify_and_exit(SetupError, e)
+        monit.notify_and_exit(e)
 
 
 if __name__ == "__main__":
     main()
 ```
 
 **Utilização do Monit para notificação de erros que
 não são grandes o suficientes para exigir que o
 processo seja interrompido.**
 
 ```Python
 # sample.py
+
+#
+#  IMPORTANTE: importar OS e entrar na pasta atual é obrigatório
+#
+import os
+
+script_path = os.path.abspath(__file__)
+os.chdir(os.path.dirname(script_path))
+
 import time
 
 from monit.core import Monitor as monit
 from monit.error import SetupError
 # from monit.logger import Logger
 # from monit.log2file import Log2File
 
@@ -90,28 +92,14 @@
     try:
         # Your code that might raise exceptions
         time.sleep(5)
         raise ValueError("This is a sample error.")
 
     except Exception as e:
         print("Erro: Ocorreu um erro inesperado.")
-        monit.notify(SetupError, e)
-        # monit.notify_and_exit(SetupError, e)
+        monit.notify(e)
 
     monit.end()
 
 
 if __name__ == "__main__":
     main()
-```
-**Tipos de erros:**
-```bash
-SetupError
-DatabaseError
-HTTPError
-FileError
-FolderError
-TooManyRequests
-DataCreateError
-DataUpdateError
-
-```
```

### Comparing `pymonit-1.3.14/setup.py` & `pymonit-1.3.15/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import pathlib
 
 setup(
     name='pymonit',
-    version='1.3.14',
+    version='1.3.15',
     description='Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados',
     long_description=pathlib.Path('README.md').read_text(),
     long_description_content_type='text/markdown',
     author='arktnld',
     author_email='arktnld@gmail.com',
     url='https://github.com/arktnld/monit',
     license='MIT',
```

