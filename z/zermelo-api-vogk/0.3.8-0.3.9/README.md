# Comparing `tmp/zermelo_api_vogk-0.3.8.tar.gz` & `tmp/zermelo_api_vogk-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zermelo_api_vogk-0.3.8.tar", last modified: Tue Jan 16 11:13:01 2024, max compression
+gzip compressed data, was "zermelo_api_vogk-0.3.9.tar", last modified: Tue Jan 16 14:50:00 2024, max compression
```

## Comparing `zermelo_api_vogk-0.3.8.tar` & `zermelo_api_vogk-0.3.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-01-16 11:13:01.823599 zermelo_api_vogk-0.3.8/
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     1068 2024-01-09 08:31:30.000000 zermelo_api_vogk-0.3.8/LICENSE
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     3300 2024-01-16 11:13:01.823599 zermelo_api_vogk-0.3.8/PKG-INFO
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     2751 2024-01-16 11:13:00.000000 zermelo_api_vogk-0.3.8/README.md
-drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-01-16 11:13:01.811599 zermelo_api_vogk-0.3.8/app/
-drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-01-16 11:13:01.811599 zermelo_api_vogk-0.3.8/app/zermelo_api/
--rw-rw-r--   0 klaas     (1000) klaas     (1000)      442 2024-01-16 10:27:33.000000 zermelo_api_vogk-0.3.8/app/zermelo_api/__init__.py
-drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-01-16 11:13:01.819599 zermelo_api_vogk-0.3.8/app/zermelo_api/src/
--rw-rw-r--   0 klaas     (1000) klaas     (1000)        0 2024-01-09 08:31:30.000000 zermelo_api_vogk-0.3.8/app/zermelo_api/src/__init__.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     3019 2024-01-09 08:31:30.000000 zermelo_api_vogk-0.3.8/app/zermelo_api/src/appointments.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     3465 2024-01-16 10:51:53.000000 zermelo_api_vogk-0.3.8/app/zermelo_api/src/branches.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     1437 2024-01-09 08:31:30.000000 zermelo_api_vogk-0.3.8/app/zermelo_api/src/config.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)      644 2024-01-09 08:31:30.000000 zermelo_api_vogk-0.3.8/app/zermelo_api/src/credentials.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)      941 2024-01-09 08:31:30.000000 zermelo_api_vogk-0.3.8/app/zermelo_api/src/groepen.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     1216 2024-01-09 08:31:30.000000 zermelo_api_vogk-0.3.8/app/zermelo_api/src/leerjaren.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     8417 2024-01-09 08:31:30.000000 zermelo_api_vogk-0.3.8/app/zermelo_api/src/lesgroepen.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     1192 2024-01-09 09:30:53.000000 zermelo_api_vogk-0.3.8/app/zermelo_api/src/logger.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)      841 2024-01-16 10:27:33.000000 zermelo_api_vogk-0.3.8/app/zermelo_api/src/lokalen.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)      446 2024-01-09 08:31:30.000000 zermelo_api_vogk-0.3.8/app/zermelo_api/src/time_utils.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     3696 2024-01-09 08:31:30.000000 zermelo_api_vogk-0.3.8/app/zermelo_api/src/users.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     1941 2024-01-16 11:13:00.000000 zermelo_api_vogk-0.3.8/app/zermelo_api/src/vakken.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     2159 2024-01-16 11:13:00.000000 zermelo_api_vogk-0.3.8/app/zermelo_api/src/vaklokdoc.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     4256 2024-01-16 10:27:33.000000 zermelo_api_vogk-0.3.8/app/zermelo_api/src/zermelo_api.py
-drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-01-16 11:13:01.823599 zermelo_api_vogk-0.3.8/app/zermelo_api_vogk.egg-info/
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     3300 2024-01-16 11:13:01.000000 zermelo_api_vogk-0.3.8/app/zermelo_api_vogk.egg-info/PKG-INFO
--rw-rw-r--   0 klaas     (1000) klaas     (1000)      758 2024-01-16 11:13:01.000000 zermelo_api_vogk-0.3.8/app/zermelo_api_vogk.egg-info/SOURCES.txt
--rw-rw-r--   0 klaas     (1000) klaas     (1000)        1 2024-01-16 11:13:01.000000 zermelo_api_vogk-0.3.8/app/zermelo_api_vogk.egg-info/dependency_links.txt
--rw-rw-r--   0 klaas     (1000) klaas     (1000)       16 2024-01-16 11:13:01.000000 zermelo_api_vogk-0.3.8/app/zermelo_api_vogk.egg-info/requires.txt
--rw-rw-r--   0 klaas     (1000) klaas     (1000)       12 2024-01-16 11:13:01.000000 zermelo_api_vogk-0.3.8/app/zermelo_api_vogk.egg-info/top_level.txt
--rw-rw-r--   0 klaas     (1000) klaas     (1000)       38 2024-01-16 11:13:01.823599 zermelo_api_vogk-0.3.8/setup.cfg
--rw-rw-r--   0 klaas     (1000) klaas     (1000)      875 2024-01-16 11:13:00.000000 zermelo_api_vogk-0.3.8/setup.py
+drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-01-16 14:50:00.127700 zermelo_api_vogk-0.3.9/
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     1068 2024-01-09 08:31:30.000000 zermelo_api_vogk-0.3.9/LICENSE
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     3333 2024-01-16 14:50:00.127700 zermelo_api_vogk-0.3.9/PKG-INFO
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     2784 2024-01-16 14:49:59.000000 zermelo_api_vogk-0.3.9/README.md
+drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-01-16 14:50:00.115700 zermelo_api_vogk-0.3.9/app/
+drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-01-16 14:50:00.115700 zermelo_api_vogk-0.3.9/app/zermelo_api/
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)      442 2024-01-16 10:27:33.000000 zermelo_api_vogk-0.3.9/app/zermelo_api/__init__.py
+drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-01-16 14:50:00.123700 zermelo_api_vogk-0.3.9/app/zermelo_api/src/
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)        0 2024-01-09 08:31:30.000000 zermelo_api_vogk-0.3.9/app/zermelo_api/src/__init__.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     3019 2024-01-09 08:31:30.000000 zermelo_api_vogk-0.3.9/app/zermelo_api/src/appointments.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     3465 2024-01-16 10:51:53.000000 zermelo_api_vogk-0.3.9/app/zermelo_api/src/branches.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     1437 2024-01-09 08:31:30.000000 zermelo_api_vogk-0.3.9/app/zermelo_api/src/config.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)      644 2024-01-09 08:31:30.000000 zermelo_api_vogk-0.3.9/app/zermelo_api/src/credentials.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)      941 2024-01-09 08:31:30.000000 zermelo_api_vogk-0.3.9/app/zermelo_api/src/groepen.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     1216 2024-01-09 08:31:30.000000 zermelo_api_vogk-0.3.9/app/zermelo_api/src/leerjaren.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     8415 2024-01-16 14:49:59.000000 zermelo_api_vogk-0.3.9/app/zermelo_api/src/lesgroepen.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     1192 2024-01-09 09:30:53.000000 zermelo_api_vogk-0.3.9/app/zermelo_api/src/logger.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)      841 2024-01-16 10:27:33.000000 zermelo_api_vogk-0.3.9/app/zermelo_api/src/lokalen.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)      446 2024-01-09 08:31:30.000000 zermelo_api_vogk-0.3.9/app/zermelo_api/src/time_utils.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     3696 2024-01-09 08:31:30.000000 zermelo_api_vogk-0.3.9/app/zermelo_api/src/users.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     1941 2024-01-16 11:13:00.000000 zermelo_api_vogk-0.3.9/app/zermelo_api/src/vakken.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     2159 2024-01-16 11:13:00.000000 zermelo_api_vogk-0.3.9/app/zermelo_api/src/vaklokdoc.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     4256 2024-01-16 10:27:33.000000 zermelo_api_vogk-0.3.9/app/zermelo_api/src/zermelo_api.py
+drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-01-16 14:50:00.127700 zermelo_api_vogk-0.3.9/app/zermelo_api_vogk.egg-info/
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     3333 2024-01-16 14:49:59.000000 zermelo_api_vogk-0.3.9/app/zermelo_api_vogk.egg-info/PKG-INFO
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)      758 2024-01-16 14:49:59.000000 zermelo_api_vogk-0.3.9/app/zermelo_api_vogk.egg-info/SOURCES.txt
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)        1 2024-01-16 14:49:59.000000 zermelo_api_vogk-0.3.9/app/zermelo_api_vogk.egg-info/dependency_links.txt
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)       16 2024-01-16 14:49:59.000000 zermelo_api_vogk-0.3.9/app/zermelo_api_vogk.egg-info/requires.txt
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)       12 2024-01-16 14:49:59.000000 zermelo_api_vogk-0.3.9/app/zermelo_api_vogk.egg-info/top_level.txt
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)       38 2024-01-16 14:50:00.127700 zermelo_api_vogk-0.3.9/setup.cfg
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)      875 2024-01-16 14:49:59.000000 zermelo_api_vogk-0.3.9/setup.py
```

### Comparing `zermelo_api_vogk-0.3.8/LICENSE` & `zermelo_api_vogk-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-0.3.8/PKG-INFO` & `zermelo_api_vogk-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zermelo_api_vogk
-Version: 0.3.8
+Version: 0.3.9
 Summary: A small module to create a Zermelo accesstoken and put some data from Zermelo in dataclasses
 Home-page: https://github.com/KlaasVogel/zermelo_api_vogk
 Author: Klaas Vogel
 Author-email: zermelo_api@klaasvogel.nl
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
@@ -13,14 +13,17 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 ## zermelo_api_vogk
 A small module to create a Zermelo accesstoken and put some data from Zermelo in dataclasses
 
+# V0.3.9
+ - change lesgroepnaam
+
 # V0.3.5 -> V0.3.8
  - added lokalen, removed debug from zermelo_api
  - added vakdocloks
  - bugfix: added lokalen to dataclass of branch
  - bugfix: subject in data vakdocloks is str not int
 
 # V0.3.1 -> 0.3.4
```

### Comparing `zermelo_api_vogk-0.3.8/README.md` & `zermelo_api_vogk-0.3.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 ## zermelo_api_vogk
 A small module to create a Zermelo accesstoken and put some data from Zermelo in dataclasses
 
+# V0.3.9
+ - change lesgroepnaam
+
 # V0.3.5 -> V0.3.8
  - added lokalen, removed debug from zermelo_api
  - added vakdocloks
  - bugfix: added lokalen to dataclass of branch
  - bugfix: subject in data vakdocloks is str not int
 
 # V0.3.1 -> 0.3.4
```

### Comparing `zermelo_api_vogk-0.3.8/app/zermelo_api/src/appointments.py` & `zermelo_api_vogk-0.3.9/app/zermelo_api/src/appointments.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-0.3.8/app/zermelo_api/src/branches.py` & `zermelo_api_vogk-0.3.9/app/zermelo_api/src/branches.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-0.3.8/app/zermelo_api/src/config.py` & `zermelo_api_vogk-0.3.9/app/zermelo_api/src/config.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-0.3.8/app/zermelo_api/src/credentials.py` & `zermelo_api_vogk-0.3.9/app/zermelo_api/src/credentials.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-0.3.8/app/zermelo_api/src/groepen.py` & `zermelo_api_vogk-0.3.9/app/zermelo_api/src/groepen.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-0.3.8/app/zermelo_api/src/leerjaren.py` & `zermelo_api_vogk-0.3.9/app/zermelo_api/src/leerjaren.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-0.3.8/app/zermelo_api/src/lesgroepen.py` & `zermelo_api_vogk-0.3.9/app/zermelo_api/src/lesgroepen.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 logger = makeLogger("LESGROEP")
 
 
 def createLesgroepNaam(vak: Vak, groep: Groep) -> str:
     leerjaar, groepnaam = groep.extendedName.split(".")
     jaarnaam = leerjaar[2:].upper()
     if vak.subjectCode in groepnaam:
-        return f"{jaarnaam}.{groepnaam}"
+        return f"{jaarnaam}{groepnaam}"
     else:
-        return f"{jaarnaam}.{vak.subjectCode}{groepnaam[-1]}"
+        return f"{jaarnaam}{vak.subjectCode}{groepnaam[-1]}"
 
 
 def find_groepen(vak: Vak, groepen: Groepen) -> list[Groep]:
     result = []
     logger.debug(f"finding groep for vak: {vak.subjectCode}")
     for groep in groepen.get_department_groups(vak.departmentOfBranch):
         if groep in result:
```

### Comparing `zermelo_api_vogk-0.3.8/app/zermelo_api/src/logger.py` & `zermelo_api_vogk-0.3.9/app/zermelo_api/src/logger.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-0.3.8/app/zermelo_api/src/lokalen.py` & `zermelo_api_vogk-0.3.9/app/zermelo_api/src/lokalen.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-0.3.8/app/zermelo_api/src/users.py` & `zermelo_api_vogk-0.3.9/app/zermelo_api/src/users.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-0.3.8/app/zermelo_api/src/vakken.py` & `zermelo_api_vogk-0.3.9/app/zermelo_api/src/vakken.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-0.3.8/app/zermelo_api/src/vaklokdoc.py` & `zermelo_api_vogk-0.3.9/app/zermelo_api/src/vaklokdoc.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-0.3.8/app/zermelo_api/src/zermelo_api.py` & `zermelo_api_vogk-0.3.9/app/zermelo_api/src/zermelo_api.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-0.3.8/app/zermelo_api_vogk.egg-info/PKG-INFO` & `zermelo_api_vogk-0.3.9/app/zermelo_api_vogk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zermelo-api-vogk
-Version: 0.3.8
+Version: 0.3.9
 Summary: A small module to create a Zermelo accesstoken and put some data from Zermelo in dataclasses
 Home-page: https://github.com/KlaasVogel/zermelo_api_vogk
 Author: Klaas Vogel
 Author-email: zermelo_api@klaasvogel.nl
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
@@ -13,14 +13,17 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 ## zermelo_api_vogk
 A small module to create a Zermelo accesstoken and put some data from Zermelo in dataclasses
 
+# V0.3.9
+ - change lesgroepnaam
+
 # V0.3.5 -> V0.3.8
  - added lokalen, removed debug from zermelo_api
  - added vakdocloks
  - bugfix: added lokalen to dataclass of branch
  - bugfix: subject in data vakdocloks is str not int
 
 # V0.3.1 -> 0.3.4
```

### Comparing `zermelo_api_vogk-0.3.8/app/zermelo_api_vogk.egg-info/SOURCES.txt` & `zermelo_api_vogk-0.3.9/app/zermelo_api_vogk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-0.3.8/setup.py` & `zermelo_api_vogk-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="zermelo_api_vogk",
-    version="0.3.8",
+    version="0.3.9",
     description="A small module to create a Zermelo accesstoken and put some data from Zermelo in dataclasses",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/KlaasVogel/zermelo_api_vogk",
     author="Klaas Vogel",
```

