# Comparing `tmp/journeylib-2.0.6.tar.gz` & `tmp/journeylib-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "journeylib-2.0.6.tar", last modified: Thu May 16 08:39:39 2024, max compression
+gzip compressed data, was "journeylib-2.0.7.tar", last modified: Thu May 16 10:54:55 2024, max compression
```

## Comparing `journeylib-2.0.6.tar` & `journeylib-2.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-05-16 08:39:39.936967 journeylib-2.0.6/
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)     1471 2024-05-16 08:39:39.936967 journeylib-2.0.6/PKG-INFO
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)     1147 2024-05-06 08:54:27.000000 journeylib-2.0.6/README.md
-drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-05-16 08:39:39.735877 journeylib-2.0.6/journeylib/
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)       24 2024-04-25 11:14:41.000000 journeylib-2.0.6/journeylib/__init__.py
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)     5052 2024-05-16 08:39:30.000000 journeylib-2.0.6/journeylib/funciones.py
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)     2772 2024-05-13 17:14:25.000000 journeylib-2.0.6/journeylib/tests.py
-drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-05-16 08:39:39.920217 journeylib-2.0.6/journeylib.egg-info/
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)     1471 2024-05-16 08:39:39.000000 journeylib-2.0.6/journeylib.egg-info/PKG-INFO
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)      254 2024-05-16 08:39:39.000000 journeylib-2.0.6/journeylib.egg-info/SOURCES.txt
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)        1 2024-05-16 08:39:39.000000 journeylib-2.0.6/journeylib.egg-info/dependency_links.txt
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)       17 2024-05-16 08:39:39.000000 journeylib-2.0.6/journeylib.egg-info/requires.txt
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)       11 2024-05-16 08:39:39.000000 journeylib-2.0.6/journeylib.egg-info/top_level.txt
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)       38 2024-05-16 08:39:39.936967 journeylib-2.0.6/setup.cfg
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)     1361 2024-05-16 08:38:53.000000 journeylib-2.0.6/setup.py
+drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-05-16 10:54:55.805629 journeylib-2.0.7/
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)     2578 2024-05-16 10:54:55.802623 journeylib-2.0.7/PKG-INFO
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)     2278 2024-05-16 08:40:19.000000 journeylib-2.0.7/README.md
+drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-05-16 10:54:55.621908 journeylib-2.0.7/journeylib/
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)       24 2024-04-25 11:14:41.000000 journeylib-2.0.7/journeylib/__init__.py
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)     5188 2024-05-16 10:53:40.000000 journeylib-2.0.7/journeylib/funciones.py
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)     2772 2024-05-13 17:14:25.000000 journeylib-2.0.7/journeylib/tests.py
+drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-05-16 10:54:55.785908 journeylib-2.0.7/journeylib.egg-info/
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)     2578 2024-05-16 10:54:55.000000 journeylib-2.0.7/journeylib.egg-info/PKG-INFO
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)      254 2024-05-16 10:54:55.000000 journeylib-2.0.7/journeylib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)        1 2024-05-16 10:54:55.000000 journeylib-2.0.7/journeylib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)       17 2024-05-16 10:54:55.000000 journeylib-2.0.7/journeylib.egg-info/requires.txt
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)       11 2024-05-16 10:54:55.000000 journeylib-2.0.7/journeylib.egg-info/top_level.txt
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)       38 2024-05-16 10:54:55.806639 journeylib-2.0.7/setup.cfg
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)     1361 2024-05-16 10:54:02.000000 journeylib-2.0.7/setup.py
```

### Comparing `journeylib-2.0.6/journeylib/funciones.py` & `journeylib-2.0.7/journeylib/funciones.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 #Imports necesarios para las funciones de la libreria
 import requests
 
+class tipoIA(Enum):
+    PASADO = 'PASADO'
+    PRESENTE = 'PRESENTE'
+    FUTURO = 'FUTURO'
+    COMPRA = 'COMPRA' 
+
 #Metodo de prueba para el despliege de la libreria
 def hola_journey():
     print('Holitaa, esta es una librería diseñada y publicada por JourneyGen para el proyecto GPTravel.')
 
 """
 Endpoint para insertar:
 http://ismi.fi.upm.es:8080/insertar/chat
@@ -34,15 +40,15 @@
 """
 
 #Implementacion de las funciones necesarias para la libreria
 """
 METODO INSERTAR HISTORICO
 Descripcion: Inserta un nuevo par de mensajes a la bd de CASH
 """
-def ins_historico(usr, tipoIA, num_chat, lista_msg, contexto, cerrado=False, url='http://195.35.1.47:8080/insertar/chat'):
+def ins_historico(usr, tipoIA: tipoIA, num_chat, lista_msg, contexto, cerrado=False, url='http://195.35.1.47:8080/insertar/chat'):
     """
     PRE:
         usr es un nombre de usuario valido
         tipoIA es un string de entre la lista ['PASADO', 'PRESENTE', 'FUTURO', 'COMPRA']
         num_chat es un int coherente con una de las siguientes descripciones:
             1. identificador de chat existente
             2. None (en este caso crearía un chat nuevo)
@@ -68,15 +74,15 @@
             n_chat = response.json()['num_chat'] # Obtenemos el numero de chat devuelto al hacer la solicitud
             return n_chat
         else:
             raise ValueError(f"ins_historico, codigo de respuesta {response.status_code}") # Codigo de respuesta distinto de 200 (no exitoso)
     except Exception as e: # Excepcion ocurrida al hacer la peticion
         raise e
 
-def get_historico(usr, tipoIA, num_chat, url='http://195.35.1.47:8080/read/chats'):
+def get_historico(usr, tipoIA: tipoIA, num_chat, url='http://195.35.1.47:8080/read/chats'):
     """
     PRE:
         usr es un nombre de usuario valido
         tipoIA es un string de entre la lista ['PASADO', 'PRESENTE', 'FUTURO', 'COMPRA']
         num_chat es un int correspondiente a un identificador de chat existente
     DEVUELVE:
         una lista de diccionarios (json) con el siguiente formato:
```

### Comparing `journeylib-2.0.6/journeylib/tests.py` & `journeylib-2.0.7/journeylib/tests.py`

 * *Files identical despite different names*

### Comparing `journeylib-2.0.6/setup.py` & `journeylib-2.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '2.0.6' #Numero de version que decidamos, cambiarlo al añadir nuevas funcionalidades o cambios
+VERSION = '2.0.7' #Numero de version que decidamos, cambiarlo al añadir nuevas funcionalidades o cambios
 PACKAGE_NAME = 'journeylib' #Nombre de la libreria
 AUTHOR = 'Equipo JourneyGen UPM' #Modificar con vuestros datos
 AUTHOR_EMAIL = 'f.gonzalez.lopez@alumnos.upm.es' #Modificar con vuestros datos
 URL = 'https://ismigit.fi.upm.es/gptravel-2024/ai-squad/journeygenai' #Modificar con vuestros datos
 
 LICENSE = 'MIT' #Tipo de licencia
 DESCRIPTION = 'Libreria para gestionar datos del historico del proyecto GPTravel' #Descripción corta
```

