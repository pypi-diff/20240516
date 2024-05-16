# Comparing `tmp/journeylib-2.0.4.tar.gz` & `tmp/journeylib-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "journeylib-2.0.4.tar", last modified: Mon May 13 23:26:57 2024, max compression
+gzip compressed data, was "journeylib-2.0.6.tar", last modified: Thu May 16 08:39:39 2024, max compression
```

## Comparing `journeylib-2.0.4.tar` & `journeylib-2.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-05-13 23:26:57.955112 journeylib-2.0.4/
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)     1471 2024-05-13 23:26:57.947128 journeylib-2.0.4/PKG-INFO
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)     1147 2024-05-06 08:54:27.000000 journeylib-2.0.4/README.md
-drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-05-13 23:26:57.680741 journeylib-2.0.4/journeylib/
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)       24 2024-04-25 11:14:41.000000 journeylib-2.0.4/journeylib/__init__.py
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)     1485 2024-05-13 23:26:23.000000 journeylib-2.0.4/journeylib/funciones.py
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)     2772 2024-05-13 17:14:25.000000 journeylib-2.0.4/journeylib/tests.py
-drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-05-13 23:26:57.911214 journeylib-2.0.4/journeylib.egg-info/
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)     1471 2024-05-13 23:26:57.000000 journeylib-2.0.4/journeylib.egg-info/PKG-INFO
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)      254 2024-05-13 23:26:57.000000 journeylib-2.0.4/journeylib.egg-info/SOURCES.txt
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)        1 2024-05-13 23:26:57.000000 journeylib-2.0.4/journeylib.egg-info/dependency_links.txt
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)       17 2024-05-13 23:26:57.000000 journeylib-2.0.4/journeylib.egg-info/requires.txt
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)       11 2024-05-13 23:26:57.000000 journeylib-2.0.4/journeylib.egg-info/top_level.txt
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)       38 2024-05-13 23:26:57.959865 journeylib-2.0.4/setup.cfg
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)     1361 2024-05-13 23:26:32.000000 journeylib-2.0.4/setup.py
+drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-05-16 08:39:39.936967 journeylib-2.0.6/
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)     1471 2024-05-16 08:39:39.936967 journeylib-2.0.6/PKG-INFO
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)     1147 2024-05-06 08:54:27.000000 journeylib-2.0.6/README.md
+drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-05-16 08:39:39.735877 journeylib-2.0.6/journeylib/
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)       24 2024-04-25 11:14:41.000000 journeylib-2.0.6/journeylib/__init__.py
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)     5052 2024-05-16 08:39:30.000000 journeylib-2.0.6/journeylib/funciones.py
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)     2772 2024-05-13 17:14:25.000000 journeylib-2.0.6/journeylib/tests.py
+drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-05-16 08:39:39.920217 journeylib-2.0.6/journeylib.egg-info/
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)     1471 2024-05-16 08:39:39.000000 journeylib-2.0.6/journeylib.egg-info/PKG-INFO
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)      254 2024-05-16 08:39:39.000000 journeylib-2.0.6/journeylib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)        1 2024-05-16 08:39:39.000000 journeylib-2.0.6/journeylib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)       17 2024-05-16 08:39:39.000000 journeylib-2.0.6/journeylib.egg-info/requires.txt
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)       11 2024-05-16 08:39:39.000000 journeylib-2.0.6/journeylib.egg-info/top_level.txt
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)       38 2024-05-16 08:39:39.936967 journeylib-2.0.6/setup.cfg
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)     1361 2024-05-16 08:38:53.000000 journeylib-2.0.6/setup.py
```

### Comparing `journeylib-2.0.4/PKG-INFO` & `journeylib-2.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: journeylib
-Version: 2.0.4
+Version: 2.0.6
 Summary: Libreria para gestionar datos del historico del proyecto GPTravel
 Home-page: https://ismigit.fi.upm.es/gptravel-2024/ai-squad/journeygenai
 Author: Equipo JourneyGen UPM
 Author-email: f.gonzalez.lopez@alumnos.upm.es
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `journeylib-2.0.4/README.md` & `journeylib-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `journeylib-2.0.4/journeylib/tests.py` & `journeylib-2.0.6/journeylib/tests.py`

 * *Files identical despite different names*

### Comparing `journeylib-2.0.4/journeylib.egg-info/PKG-INFO` & `journeylib-2.0.6/journeylib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: journeylib
-Version: 2.0.4
+Version: 2.0.6
 Summary: Libreria para gestionar datos del historico del proyecto GPTravel
 Home-page: https://ismigit.fi.upm.es/gptravel-2024/ai-squad/journeygenai
 Author: Equipo JourneyGen UPM
 Author-email: f.gonzalez.lopez@alumnos.upm.es
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `journeylib-2.0.4/setup.py` & `journeylib-2.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '2.0.4' #Numero de version que decidamos, cambiarlo al añadir nuevas funcionalidades o cambios
+VERSION = '2.0.6' #Numero de version que decidamos, cambiarlo al añadir nuevas funcionalidades o cambios
 PACKAGE_NAME = 'journeylib' #Nombre de la libreria
 AUTHOR = 'Equipo JourneyGen UPM' #Modificar con vuestros datos
 AUTHOR_EMAIL = 'f.gonzalez.lopez@alumnos.upm.es' #Modificar con vuestros datos
 URL = 'https://ismigit.fi.upm.es/gptravel-2024/ai-squad/journeygenai' #Modificar con vuestros datos
 
 LICENSE = 'MIT' #Tipo de licencia
 DESCRIPTION = 'Libreria para gestionar datos del historico del proyecto GPTravel' #Descripción corta
```

