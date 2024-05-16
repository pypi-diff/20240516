# Comparing `tmp/journeylib-2.0.8.tar.gz` & `tmp/journeylib-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "journeylib-2.0.8.tar", last modified: Thu May 16 10:59:09 2024, max compression
+gzip compressed data, was "journeylib-2.0.9.tar", last modified: Thu May 16 11:07:23 2024, max compression
```

## Comparing `journeylib-2.0.8.tar` & `journeylib-2.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-05-16 10:59:09.103240 journeylib-2.0.8/
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)     2578 2024-05-16 10:59:09.102071 journeylib-2.0.8/PKG-INFO
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)     2278 2024-05-16 08:40:19.000000 journeylib-2.0.8/README.md
-drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-05-16 10:59:08.992492 journeylib-2.0.8/journeylib/
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)       24 2024-04-25 11:14:41.000000 journeylib-2.0.8/journeylib/__init__.py
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)     5211 2024-05-16 10:58:48.000000 journeylib-2.0.8/journeylib/funciones.py
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)     2772 2024-05-13 17:14:25.000000 journeylib-2.0.8/journeylib/tests.py
-drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-05-16 10:59:09.082934 journeylib-2.0.8/journeylib.egg-info/
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)     2578 2024-05-16 10:59:08.000000 journeylib-2.0.8/journeylib.egg-info/PKG-INFO
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)      254 2024-05-16 10:59:08.000000 journeylib-2.0.8/journeylib.egg-info/SOURCES.txt
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)        1 2024-05-16 10:59:08.000000 journeylib-2.0.8/journeylib.egg-info/dependency_links.txt
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)       17 2024-05-16 10:59:08.000000 journeylib-2.0.8/journeylib.egg-info/requires.txt
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)       11 2024-05-16 10:59:08.000000 journeylib-2.0.8/journeylib.egg-info/top_level.txt
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)       38 2024-05-16 10:59:09.104248 journeylib-2.0.8/setup.cfg
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)     1361 2024-05-16 10:58:55.000000 journeylib-2.0.8/setup.py
+drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-05-16 11:07:23.104109 journeylib-2.0.9/
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)     2578 2024-05-16 11:07:23.100725 journeylib-2.0.9/PKG-INFO
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)     2278 2024-05-16 08:40:19.000000 journeylib-2.0.9/README.md
+drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-05-16 11:07:22.966642 journeylib-2.0.9/journeylib/
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)       24 2024-04-25 11:14:41.000000 journeylib-2.0.9/journeylib/__init__.py
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)     5229 2024-05-16 11:07:04.000000 journeylib-2.0.9/journeylib/funciones.py
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)     2772 2024-05-13 17:14:25.000000 journeylib-2.0.9/journeylib/tests.py
+drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-05-16 11:07:23.076310 journeylib-2.0.9/journeylib.egg-info/
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)     2578 2024-05-16 11:07:22.000000 journeylib-2.0.9/journeylib.egg-info/PKG-INFO
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)      254 2024-05-16 11:07:22.000000 journeylib-2.0.9/journeylib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)        1 2024-05-16 11:07:22.000000 journeylib-2.0.9/journeylib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)       17 2024-05-16 11:07:22.000000 journeylib-2.0.9/journeylib.egg-info/requires.txt
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)       11 2024-05-16 11:07:22.000000 journeylib-2.0.9/journeylib.egg-info/top_level.txt
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)       38 2024-05-16 11:07:23.104109 journeylib-2.0.9/setup.cfg
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)     1361 2024-05-16 11:07:11.000000 journeylib-2.0.9/setup.py
```

### Comparing `journeylib-2.0.8/PKG-INFO` & `journeylib-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: journeylib
-Version: 2.0.8
+Version: 2.0.9
 Summary: Libreria para gestionar datos del historico del proyecto GPTravel
 Home-page: https://ismigit.fi.upm.es/gptravel-2024/ai-squad/journeygenai
 Author: Equipo JourneyGen UPM
 Author-email: f.gonzalez.lopez@alumnos.upm.es
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `journeylib-2.0.8/README.md` & `journeylib-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `journeylib-2.0.8/journeylib/funciones.py` & `journeylib-2.0.9/journeylib/funciones.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
             n_chat = response.json()['num_chat'] # Obtenemos el numero de chat devuelto al hacer la solicitud
             return n_chat
         else:
             raise ValueError(f"ins_historico, codigo de respuesta {response.status_code}") # Codigo de respuesta distinto de 200 (no exitoso)
     except Exception as e: # Excepcion ocurrida al hacer la peticion
         raise e
 
-def get_historico(usr, tipoIA: tipoIA, num_chat, url='http://195.35.1.47:8080/read/chats'):
+def get_historico(usr, tipoIA, num_chat, url='http://195.35.1.47:8080/read/chats'):
     """
     PRE:
         usr es un nombre de usuario valido
         tipoIA es un string de entre la lista ['PASADO', 'PRESENTE', 'FUTURO', 'COMPRA']
         num_chat es un int correspondiente a un identificador de chat existente
     DEVUELVE:
         una lista de diccionarios (json) con el siguiente formato:
@@ -95,14 +95,15 @@
 
     try:
         datos_get = { # Formato con el que se consume la api
             'username': usr,
             'chat': num_chat,
             'tipoIA': tipoIA
         }
+        print(datos_get)
         response = requests.get(url, json=datos_get)
 
         if response.status_code == 200:
             """
              Obtenemos cuerpo, lista de dict tq: {
                 'fecha': mensaje.fecha.strftime("%Y-%m-%d %H:%M"),
                 'input': mensaje.input,
```

### Comparing `journeylib-2.0.8/journeylib/tests.py` & `journeylib-2.0.9/journeylib/tests.py`

 * *Files identical despite different names*

### Comparing `journeylib-2.0.8/journeylib.egg-info/PKG-INFO` & `journeylib-2.0.9/journeylib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: journeylib
-Version: 2.0.8
+Version: 2.0.9
 Summary: Libreria para gestionar datos del historico del proyecto GPTravel
 Home-page: https://ismigit.fi.upm.es/gptravel-2024/ai-squad/journeygenai
 Author: Equipo JourneyGen UPM
 Author-email: f.gonzalez.lopez@alumnos.upm.es
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `journeylib-2.0.8/setup.py` & `journeylib-2.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '2.0.8' #Numero de version que decidamos, cambiarlo al añadir nuevas funcionalidades o cambios
+VERSION = '2.0.9' #Numero de version que decidamos, cambiarlo al añadir nuevas funcionalidades o cambios
 PACKAGE_NAME = 'journeylib' #Nombre de la libreria
 AUTHOR = 'Equipo JourneyGen UPM' #Modificar con vuestros datos
 AUTHOR_EMAIL = 'f.gonzalez.lopez@alumnos.upm.es' #Modificar con vuestros datos
 URL = 'https://ismigit.fi.upm.es/gptravel-2024/ai-squad/journeygenai' #Modificar con vuestros datos
 
 LICENSE = 'MIT' #Tipo de licencia
 DESCRIPTION = 'Libreria para gestionar datos del historico del proyecto GPTravel' #Descripción corta
```

