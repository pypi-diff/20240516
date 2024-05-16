# Comparing `tmp/journeylib-2.0.7.tar.gz` & `tmp/journeylib-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "journeylib-2.0.7.tar", last modified: Thu May 16 10:54:55 2024, max compression
+gzip compressed data, was "journeylib-2.0.8.tar", last modified: Thu May 16 10:59:09 2024, max compression
```

## Comparing `journeylib-2.0.7.tar` & `journeylib-2.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-05-16 10:54:55.805629 journeylib-2.0.7/
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)     2578 2024-05-16 10:54:55.802623 journeylib-2.0.7/PKG-INFO
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)     2278 2024-05-16 08:40:19.000000 journeylib-2.0.7/README.md
-drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-05-16 10:54:55.621908 journeylib-2.0.7/journeylib/
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)       24 2024-04-25 11:14:41.000000 journeylib-2.0.7/journeylib/__init__.py
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)     5188 2024-05-16 10:53:40.000000 journeylib-2.0.7/journeylib/funciones.py
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)     2772 2024-05-13 17:14:25.000000 journeylib-2.0.7/journeylib/tests.py
-drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-05-16 10:54:55.785908 journeylib-2.0.7/journeylib.egg-info/
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)     2578 2024-05-16 10:54:55.000000 journeylib-2.0.7/journeylib.egg-info/PKG-INFO
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)      254 2024-05-16 10:54:55.000000 journeylib-2.0.7/journeylib.egg-info/SOURCES.txt
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)        1 2024-05-16 10:54:55.000000 journeylib-2.0.7/journeylib.egg-info/dependency_links.txt
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)       17 2024-05-16 10:54:55.000000 journeylib-2.0.7/journeylib.egg-info/requires.txt
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)       11 2024-05-16 10:54:55.000000 journeylib-2.0.7/journeylib.egg-info/top_level.txt
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)       38 2024-05-16 10:54:55.806639 journeylib-2.0.7/setup.cfg
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)     1361 2024-05-16 10:54:02.000000 journeylib-2.0.7/setup.py
+drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-05-16 10:59:09.103240 journeylib-2.0.8/
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)     2578 2024-05-16 10:59:09.102071 journeylib-2.0.8/PKG-INFO
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)     2278 2024-05-16 08:40:19.000000 journeylib-2.0.8/README.md
+drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-05-16 10:59:08.992492 journeylib-2.0.8/journeylib/
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)       24 2024-04-25 11:14:41.000000 journeylib-2.0.8/journeylib/__init__.py
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)     5211 2024-05-16 10:58:48.000000 journeylib-2.0.8/journeylib/funciones.py
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)     2772 2024-05-13 17:14:25.000000 journeylib-2.0.8/journeylib/tests.py
+drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-05-16 10:59:09.082934 journeylib-2.0.8/journeylib.egg-info/
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)     2578 2024-05-16 10:59:08.000000 journeylib-2.0.8/journeylib.egg-info/PKG-INFO
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)      254 2024-05-16 10:59:08.000000 journeylib-2.0.8/journeylib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)        1 2024-05-16 10:59:08.000000 journeylib-2.0.8/journeylib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)       17 2024-05-16 10:59:08.000000 journeylib-2.0.8/journeylib.egg-info/requires.txt
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)       11 2024-05-16 10:59:08.000000 journeylib-2.0.8/journeylib.egg-info/top_level.txt
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)       38 2024-05-16 10:59:09.104248 journeylib-2.0.8/setup.cfg
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)     1361 2024-05-16 10:58:55.000000 journeylib-2.0.8/setup.py
```

### Comparing `journeylib-2.0.7/PKG-INFO` & `journeylib-2.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: journeylib
-Version: 2.0.7
+Version: 2.0.8
 Summary: Libreria para gestionar datos del historico del proyecto GPTravel
 Home-page: https://ismigit.fi.upm.es/gptravel-2024/ai-squad/journeygenai
 Author: Equipo JourneyGen UPM
 Author-email: f.gonzalez.lopez@alumnos.upm.es
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `journeylib-2.0.7/README.md` & `journeylib-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `journeylib-2.0.7/journeylib/funciones.py` & `journeylib-2.0.8/journeylib/funciones.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #Imports necesarios para las funciones de la libreria
 import requests
+from enum import Enum
 
 class tipoIA(Enum):
     PASADO = 'PASADO'
     PRESENTE = 'PRESENTE'
     FUTURO = 'FUTURO'
     COMPRA = 'COMPRA'
```

### Comparing `journeylib-2.0.7/journeylib/tests.py` & `journeylib-2.0.8/journeylib/tests.py`

 * *Files identical despite different names*

### Comparing `journeylib-2.0.7/journeylib.egg-info/PKG-INFO` & `journeylib-2.0.8/journeylib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: journeylib
-Version: 2.0.7
+Version: 2.0.8
 Summary: Libreria para gestionar datos del historico del proyecto GPTravel
 Home-page: https://ismigit.fi.upm.es/gptravel-2024/ai-squad/journeygenai
 Author: Equipo JourneyGen UPM
 Author-email: f.gonzalez.lopez@alumnos.upm.es
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `journeylib-2.0.7/setup.py` & `journeylib-2.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '2.0.7' #Numero de version que decidamos, cambiarlo al añadir nuevas funcionalidades o cambios
+VERSION = '2.0.8' #Numero de version que decidamos, cambiarlo al añadir nuevas funcionalidades o cambios
 PACKAGE_NAME = 'journeylib' #Nombre de la libreria
 AUTHOR = 'Equipo JourneyGen UPM' #Modificar con vuestros datos
 AUTHOR_EMAIL = 'f.gonzalez.lopez@alumnos.upm.es' #Modificar con vuestros datos
 URL = 'https://ismigit.fi.upm.es/gptravel-2024/ai-squad/journeygenai' #Modificar con vuestros datos
 
 LICENSE = 'MIT' #Tipo de licencia
 DESCRIPTION = 'Libreria para gestionar datos del historico del proyecto GPTravel' #Descripción corta
```

