# Comparing `tmp/pymonit-1.3.19.tar.gz` & `tmp/pymonit-1.3.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymonit-1.3.19.tar", last modified: Thu May 16 13:02:20 2024, max compression
+gzip compressed data, was "pymonit-1.3.20.tar", last modified: Thu May 16 13:25:58 2024, max compression
```

## Comparing `pymonit-1.3.19.tar` & `pymonit-1.3.20.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-16 13:02:20.671758 pymonit-1.3.19/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1064 2024-04-22 01:06:10.000000 pymonit-1.3.19/LICENSE
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2585 2024-05-16 13:02:20.671758 pymonit-1.3.19/PKG-INFO
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1949 2024-05-16 13:01:46.000000 pymonit-1.3.19/README.md
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-16 13:02:20.668425 pymonit-1.3.19/monit/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:06:10.000000 pymonit-1.3.19/monit/__init__.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      922 2024-04-30 01:09:27.000000 pymonit-1.3.19/monit/config.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      725 2024-05-16 12:44:15.000000 pymonit-1.3.19/monit/core.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1594 2024-05-16 12:44:25.000000 pymonit-1.3.19/monit/database.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      227 2024-04-25 22:34:06.000000 pymonit-1.3.19/monit/error.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     3128 2024-05-16 12:41:20.000000 pymonit-1.3.19/monit/func.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1831 2024-04-22 23:15:08.000000 pymonit-1.3.19/monit/log2file.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2569 2024-04-22 23:04:24.000000 pymonit-1.3.19/monit/logger.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      272 2024-05-15 21:55:05.000000 pymonit-1.3.19/monit/verify_env.py
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-16 13:02:20.671758 pymonit-1.3.19/pymonit.egg-info/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2585 2024-05-16 13:02:20.000000 pymonit-1.3.19/pymonit.egg-info/PKG-INFO
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      329 2024-05-16 13:02:20.000000 pymonit-1.3.19/pymonit.egg-info/SOURCES.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        1 2024-05-16 13:02:20.000000 pymonit-1.3.19/pymonit.egg-info/dependency_links.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-05-16 13:02:20.000000 pymonit-1.3.19/pymonit.egg-info/requires.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        6 2024-05-16 13:02:20.000000 pymonit-1.3.19/pymonit.egg-info/top_level.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       38 2024-05-16 13:02:20.671758 pymonit-1.3.19/setup.cfg
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      866 2024-05-16 13:01:55.000000 pymonit-1.3.19/setup.py
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-16 13:25:58.725876 pymonit-1.3.20/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1064 2024-04-22 01:06:10.000000 pymonit-1.3.20/LICENSE
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2761 2024-05-16 13:25:58.725876 pymonit-1.3.20/PKG-INFO
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2125 2024-05-16 13:25:36.000000 pymonit-1.3.20/README.md
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-16 13:25:58.725876 pymonit-1.3.20/monit/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:06:10.000000 pymonit-1.3.20/monit/__init__.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      922 2024-04-30 01:09:27.000000 pymonit-1.3.20/monit/config.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      725 2024-05-16 12:44:15.000000 pymonit-1.3.20/monit/core.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1594 2024-05-16 12:44:25.000000 pymonit-1.3.20/monit/database.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      227 2024-04-25 22:34:06.000000 pymonit-1.3.20/monit/error.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     3128 2024-05-16 12:41:20.000000 pymonit-1.3.20/monit/func.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1831 2024-04-22 23:15:08.000000 pymonit-1.3.20/monit/log2file.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2569 2024-04-22 23:04:24.000000 pymonit-1.3.20/monit/logger.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      272 2024-05-15 21:55:05.000000 pymonit-1.3.20/monit/verify_env.py
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-16 13:25:58.725876 pymonit-1.3.20/pymonit.egg-info/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2761 2024-05-16 13:25:58.000000 pymonit-1.3.20/pymonit.egg-info/PKG-INFO
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      329 2024-05-16 13:25:58.000000 pymonit-1.3.20/pymonit.egg-info/SOURCES.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        1 2024-05-16 13:25:58.000000 pymonit-1.3.20/pymonit.egg-info/dependency_links.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-05-16 13:25:58.000000 pymonit-1.3.20/pymonit.egg-info/requires.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        6 2024-05-16 13:25:58.000000 pymonit-1.3.20/pymonit.egg-info/top_level.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       38 2024-05-16 13:25:58.725876 pymonit-1.3.20/setup.cfg
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      866 2024-05-16 13:25:43.000000 pymonit-1.3.20/setup.py
```

### Comparing `pymonit-1.3.19/LICENSE` & `pymonit-1.3.20/LICENSE`

 * *Files identical despite different names*

### Comparing `pymonit-1.3.19/PKG-INFO` & `pymonit-1.3.20/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymonit
-Version: 1.3.19
+Version: 1.3.20
 Summary: Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados
 Home-page: https://github.com/arktnld/monit
 Author: arktnld
 Author-email: arktnld@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -48,15 +48,16 @@
 EMAIL_PASSWORD=
 ```
 ### Exemplo de Uso:
 
 **Utilização do Monit para notificação de erros**
 ```python
 #
-#  IMPORTANTE: importar OS e entrar na pasta atual é obrigatório no inicio do arquivo
+#  IMPORTANTE: importar OS e entrar na pasta atual é obrigatório no inicio do arquivo,
+#              para que o script seja executado corretamente em agendadores de tarefa.
 #
 import os
 
 script_path = os.path.abspath(__file__)
 os.chdir(os.path.dirname(script_path))
 
 import time
@@ -81,15 +82,16 @@
 
 **Utilização do Monit para notificação de erros que
 não são grandes o suficientes para exigir que o
 processo seja interrompido.**
 
 ```Python
 #
-#  IMPORTANTE: importar OS e entrar na pasta atual é obrigatório no inicio do arquivo
+#  IMPORTANTE: importar OS e entrar na pasta atual é obrigatório no inicio do arquivo,
+#              para que o script seja executado corretamente em agendadores de tarefa.
 #
 import os
 
 script_path = os.path.abspath(__file__)
 os.chdir(os.path.dirname(script_path))
 
 import time
```

### Comparing `pymonit-1.3.19/README.md` & `pymonit-1.3.20/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -29,15 +29,16 @@
 EMAIL_PASSWORD=
 ```
 ### Exemplo de Uso:
 
 **Utilização do Monit para notificação de erros**
 ```python
 #
-#  IMPORTANTE: importar OS e entrar na pasta atual é obrigatório no inicio do arquivo
+#  IMPORTANTE: importar OS e entrar na pasta atual é obrigatório no inicio do arquivo,
+#              para que o script seja executado corretamente em agendadores de tarefa.
 #
 import os
 
 script_path = os.path.abspath(__file__)
 os.chdir(os.path.dirname(script_path))
 
 import time
@@ -62,15 +63,16 @@
 
 **Utilização do Monit para notificação de erros que
 não são grandes o suficientes para exigir que o
 processo seja interrompido.**
 
 ```Python
 #
-#  IMPORTANTE: importar OS e entrar na pasta atual é obrigatório no inicio do arquivo
+#  IMPORTANTE: importar OS e entrar na pasta atual é obrigatório no inicio do arquivo,
+#              para que o script seja executado corretamente em agendadores de tarefa.
 #
 import os
 
 script_path = os.path.abspath(__file__)
 os.chdir(os.path.dirname(script_path))
 
 import time
```

### Comparing `pymonit-1.3.19/monit/config.py` & `pymonit-1.3.20/monit/config.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.3.19/monit/core.py` & `pymonit-1.3.20/monit/core.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.3.19/monit/database.py` & `pymonit-1.3.20/monit/database.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.3.19/monit/func.py` & `pymonit-1.3.20/monit/func.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.3.19/monit/log2file.py` & `pymonit-1.3.20/monit/log2file.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.3.19/monit/logger.py` & `pymonit-1.3.20/monit/logger.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.3.19/pymonit.egg-info/PKG-INFO` & `pymonit-1.3.20/pymonit.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymonit
-Version: 1.3.19
+Version: 1.3.20
 Summary: Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados
 Home-page: https://github.com/arktnld/monit
 Author: arktnld
 Author-email: arktnld@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -48,15 +48,16 @@
 EMAIL_PASSWORD=
 ```
 ### Exemplo de Uso:
 
 **Utilização do Monit para notificação de erros**
 ```python
 #
-#  IMPORTANTE: importar OS e entrar na pasta atual é obrigatório no inicio do arquivo
+#  IMPORTANTE: importar OS e entrar na pasta atual é obrigatório no inicio do arquivo,
+#              para que o script seja executado corretamente em agendadores de tarefa.
 #
 import os
 
 script_path = os.path.abspath(__file__)
 os.chdir(os.path.dirname(script_path))
 
 import time
@@ -81,15 +82,16 @@
 
 **Utilização do Monit para notificação de erros que
 não são grandes o suficientes para exigir que o
 processo seja interrompido.**
 
 ```Python
 #
-#  IMPORTANTE: importar OS e entrar na pasta atual é obrigatório no inicio do arquivo
+#  IMPORTANTE: importar OS e entrar na pasta atual é obrigatório no inicio do arquivo,
+#              para que o script seja executado corretamente em agendadores de tarefa.
 #
 import os
 
 script_path = os.path.abspath(__file__)
 os.chdir(os.path.dirname(script_path))
 
 import time
```

### Comparing `pymonit-1.3.19/setup.py` & `pymonit-1.3.20/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import pathlib
 
 setup(
     name='pymonit',
-    version='1.3.19',
+    version='1.3.20',
     description='Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados',
     long_description=pathlib.Path('README.md').read_text(),
     long_description_content_type='text/markdown',
     author='arktnld',
     author_email='arktnld@gmail.com',
     url='https://github.com/arktnld/monit',
     license='MIT',
```

