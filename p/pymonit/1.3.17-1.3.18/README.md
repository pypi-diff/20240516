# Comparing `tmp/pymonit-1.3.17.tar.gz` & `tmp/pymonit-1.3.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymonit-1.3.17.tar", last modified: Thu May 16 12:55:36 2024, max compression
+gzip compressed data, was "pymonit-1.3.18.tar", last modified: Thu May 16 12:57:10 2024, max compression
```

## Comparing `pymonit-1.3.17.tar` & `pymonit-1.3.18.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-16 12:55:36.240225 pymonit-1.3.17/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1064 2024-04-22 01:06:10.000000 pymonit-1.3.17/LICENSE
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2594 2024-05-16 12:55:36.236892 pymonit-1.3.17/PKG-INFO
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1958 2024-05-16 12:54:50.000000 pymonit-1.3.17/README.md
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-16 12:55:36.236892 pymonit-1.3.17/monit/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:06:10.000000 pymonit-1.3.17/monit/__init__.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      922 2024-04-30 01:09:27.000000 pymonit-1.3.17/monit/config.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      725 2024-05-16 12:44:15.000000 pymonit-1.3.17/monit/core.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1594 2024-05-16 12:44:25.000000 pymonit-1.3.17/monit/database.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      227 2024-04-25 22:34:06.000000 pymonit-1.3.17/monit/error.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     3128 2024-05-16 12:41:20.000000 pymonit-1.3.17/monit/func.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1831 2024-04-22 23:15:08.000000 pymonit-1.3.17/monit/log2file.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2569 2024-04-22 23:04:24.000000 pymonit-1.3.17/monit/logger.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      272 2024-05-15 21:55:05.000000 pymonit-1.3.17/monit/verify_env.py
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-16 12:55:36.236892 pymonit-1.3.17/pymonit.egg-info/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2594 2024-05-16 12:55:36.000000 pymonit-1.3.17/pymonit.egg-info/PKG-INFO
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      329 2024-05-16 12:55:36.000000 pymonit-1.3.17/pymonit.egg-info/SOURCES.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        1 2024-05-16 12:55:36.000000 pymonit-1.3.17/pymonit.egg-info/dependency_links.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-05-16 12:55:36.000000 pymonit-1.3.17/pymonit.egg-info/requires.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        6 2024-05-16 12:55:36.000000 pymonit-1.3.17/pymonit.egg-info/top_level.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       38 2024-05-16 12:55:36.240225 pymonit-1.3.17/setup.cfg
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      866 2024-05-16 12:54:55.000000 pymonit-1.3.17/setup.py
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-16 12:57:10.451567 pymonit-1.3.18/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1064 2024-04-22 01:06:10.000000 pymonit-1.3.18/LICENSE
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2598 2024-05-16 12:57:10.451567 pymonit-1.3.18/PKG-INFO
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1962 2024-05-16 12:56:36.000000 pymonit-1.3.18/README.md
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-16 12:57:10.451567 pymonit-1.3.18/monit/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:06:10.000000 pymonit-1.3.18/monit/__init__.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      922 2024-04-30 01:09:27.000000 pymonit-1.3.18/monit/config.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      725 2024-05-16 12:44:15.000000 pymonit-1.3.18/monit/core.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1594 2024-05-16 12:44:25.000000 pymonit-1.3.18/monit/database.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      227 2024-04-25 22:34:06.000000 pymonit-1.3.18/monit/error.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     3128 2024-05-16 12:41:20.000000 pymonit-1.3.18/monit/func.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1831 2024-04-22 23:15:08.000000 pymonit-1.3.18/monit/log2file.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2569 2024-04-22 23:04:24.000000 pymonit-1.3.18/monit/logger.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      272 2024-05-15 21:55:05.000000 pymonit-1.3.18/monit/verify_env.py
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-16 12:57:10.451567 pymonit-1.3.18/pymonit.egg-info/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2598 2024-05-16 12:57:10.000000 pymonit-1.3.18/pymonit.egg-info/PKG-INFO
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      329 2024-05-16 12:57:10.000000 pymonit-1.3.18/pymonit.egg-info/SOURCES.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        1 2024-05-16 12:57:10.000000 pymonit-1.3.18/pymonit.egg-info/dependency_links.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-05-16 12:57:10.000000 pymonit-1.3.18/pymonit.egg-info/requires.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        6 2024-05-16 12:57:10.000000 pymonit-1.3.18/pymonit.egg-info/top_level.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       38 2024-05-16 12:57:10.451567 pymonit-1.3.18/setup.cfg
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      866 2024-05-16 12:57:06.000000 pymonit-1.3.18/setup.py
```

### Comparing `pymonit-1.3.17/LICENSE` & `pymonit-1.3.18/LICENSE`

 * *Files identical despite different names*

### Comparing `pymonit-1.3.17/PKG-INFO` & `pymonit-1.3.18/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymonit
-Version: 1.3.17
+Version: 1.3.18
 Summary: Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados
 Home-page: https://github.com/arktnld/monit
 Author: arktnld
 Author-email: arktnld@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -48,15 +48,15 @@
 EMAIL_PASSWORD=
 ```
 ### Exemplo de Uso:
 
 **Utilização do Monit para notificação de erros**
 ```python
 #
-#  IMPORTANTE: importar OS entrar na pasta atual é obrigatório no inicio do arquivo
+#  IMPORTANTE: importar OS e entrar na pasta atual é obrigatório no inicio do arquivo
 #
 import os
 
 script_path = os.path.abspath(__file__)
 os.chdir(os.path.dirname(script_path))
 
 import time
@@ -83,15 +83,15 @@
 não são grandes o suficientes para exigir que o
 processo seja interrompido.**
 
 ```Python
 # sample.py
 
 #
-#  IMPORTANTE: importar OS entrar na pasta atual é obrigatório no inicio do arquivo
+#  IMPORTANTE: importar OS e entrar na pasta atual é obrigatório no inicio do arquivo
 #
 import os
 
 script_path = os.path.abspath(__file__)
 os.chdir(os.path.dirname(script_path))
 
 import time
```

### Comparing `pymonit-1.3.17/README.md` & `pymonit-1.3.18/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 EMAIL_PASSWORD=
 ```
 ### Exemplo de Uso:
 
 **Utilização do Monit para notificação de erros**
 ```python
 #
-#  IMPORTANTE: importar OS entrar na pasta atual é obrigatório no inicio do arquivo
+#  IMPORTANTE: importar OS e entrar na pasta atual é obrigatório no inicio do arquivo
 #
 import os
 
 script_path = os.path.abspath(__file__)
 os.chdir(os.path.dirname(script_path))
 
 import time
@@ -64,15 +64,15 @@
 não são grandes o suficientes para exigir que o
 processo seja interrompido.**
 
 ```Python
 # sample.py
 
 #
-#  IMPORTANTE: importar OS entrar na pasta atual é obrigatório no inicio do arquivo
+#  IMPORTANTE: importar OS e entrar na pasta atual é obrigatório no inicio do arquivo
 #
 import os
 
 script_path = os.path.abspath(__file__)
 os.chdir(os.path.dirname(script_path))
 
 import time
```

### Comparing `pymonit-1.3.17/monit/config.py` & `pymonit-1.3.18/monit/config.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.3.17/monit/core.py` & `pymonit-1.3.18/monit/core.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.3.17/monit/database.py` & `pymonit-1.3.18/monit/database.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.3.17/monit/func.py` & `pymonit-1.3.18/monit/func.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.3.17/monit/log2file.py` & `pymonit-1.3.18/monit/log2file.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.3.17/monit/logger.py` & `pymonit-1.3.18/monit/logger.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.3.17/pymonit.egg-info/PKG-INFO` & `pymonit-1.3.18/pymonit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymonit
-Version: 1.3.17
+Version: 1.3.18
 Summary: Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados
 Home-page: https://github.com/arktnld/monit
 Author: arktnld
 Author-email: arktnld@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -48,15 +48,15 @@
 EMAIL_PASSWORD=
 ```
 ### Exemplo de Uso:
 
 **Utilização do Monit para notificação de erros**
 ```python
 #
-#  IMPORTANTE: importar OS entrar na pasta atual é obrigatório no inicio do arquivo
+#  IMPORTANTE: importar OS e entrar na pasta atual é obrigatório no inicio do arquivo
 #
 import os
 
 script_path = os.path.abspath(__file__)
 os.chdir(os.path.dirname(script_path))
 
 import time
@@ -83,15 +83,15 @@
 não são grandes o suficientes para exigir que o
 processo seja interrompido.**
 
 ```Python
 # sample.py
 
 #
-#  IMPORTANTE: importar OS entrar na pasta atual é obrigatório no inicio do arquivo
+#  IMPORTANTE: importar OS e entrar na pasta atual é obrigatório no inicio do arquivo
 #
 import os
 
 script_path = os.path.abspath(__file__)
 os.chdir(os.path.dirname(script_path))
 
 import time
```

### Comparing `pymonit-1.3.17/setup.py` & `pymonit-1.3.18/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import pathlib
 
 setup(
     name='pymonit',
-    version='1.3.17',
+    version='1.3.18',
     description='Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados',
     long_description=pathlib.Path('README.md').read_text(),
     long_description_content_type='text/markdown',
     author='arktnld',
     author_email='arktnld@gmail.com',
     url='https://github.com/arktnld/monit',
     license='MIT',
```

