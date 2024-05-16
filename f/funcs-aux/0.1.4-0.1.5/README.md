# Comparing `tmp/funcs_aux-0.1.4.tar.gz` & `tmp/funcs_aux-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcs_aux-0.1.4.tar", last modified: Thu May 16 09:01:22 2024, max compression
+gzip compressed data, was "funcs_aux-0.1.5.tar", last modified: Thu May 16 09:08:53 2024, max compression
```

## Comparing `funcs_aux-0.1.4.tar` & `funcs_aux-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 09:01:22.971678 funcs_aux-0.1.4/
--rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 funcs_aux-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     1883 2024-05-16 09:01:22.970678 funcs_aux-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      990 2024-05-16 09:00:23.000000 funcs_aux-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 09:01:22.962048 funcs_aux-0.1.4/funcs_aux/
--rw-rw-rw-   0        0        0      282 2024-03-28 09:55:47.000000 funcs_aux-0.1.4/funcs_aux/__init__.py
--rw-rw-rw-   0        0        0     1894 2024-03-01 08:49:51.000000 funcs_aux-0.1.4/funcs_aux/arrays.py
--rw-rw-rw-   0        0        0     6005 2024-03-28 14:40:09.000000 funcs_aux-0.1.4/funcs_aux/collects.py
--rw-rw-rw-   0        0        0     5211 2024-03-22 14:19:18.000000 funcs_aux-0.1.4/funcs_aux/iterables.py
--rw-rw-rw-   0        0        0     9772 2024-05-16 08:59:28.000000 funcs_aux-0.1.4/funcs_aux/results.py
--rw-rw-rw-   0        0        0     1920 2024-03-01 08:45:13.000000 funcs_aux-0.1.4/funcs_aux/strings.py
-drwxrwxrwx   0        0        0        0 2024-05-16 09:01:22.969617 funcs_aux-0.1.4/funcs_aux.egg-info/
--rw-rw-rw-   0        0        0     1883 2024-05-16 09:01:22.000000 funcs_aux-0.1.4/funcs_aux.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2024-05-16 09:01:22.000000 funcs_aux-0.1.4/funcs_aux.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 09:01:22.000000 funcs_aux-0.1.4/funcs_aux.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-16 09:01:22.000000 funcs_aux-0.1.4/funcs_aux.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 09:01:22.971678 funcs_aux-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 funcs_aux-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:08:53.843238 funcs_aux-0.1.5/
+-rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 funcs_aux-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     1883 2024-05-16 09:08:53.842234 funcs_aux-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      990 2024-05-16 09:08:23.000000 funcs_aux-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 09:08:53.836120 funcs_aux-0.1.5/funcs_aux/
+-rw-rw-rw-   0        0        0      301 2024-05-16 09:08:23.000000 funcs_aux-0.1.5/funcs_aux/__init__.py
+-rw-rw-rw-   0        0        0     1894 2024-03-01 08:49:51.000000 funcs_aux-0.1.5/funcs_aux/arrays.py
+-rw-rw-rw-   0        0        0     6005 2024-03-28 14:40:09.000000 funcs_aux-0.1.5/funcs_aux/collects.py
+-rw-rw-rw-   0        0        0     5211 2024-03-22 14:19:18.000000 funcs_aux-0.1.5/funcs_aux/iterables.py
+-rw-rw-rw-   0        0        0     9772 2024-05-16 08:59:28.000000 funcs_aux-0.1.5/funcs_aux/results.py
+-rw-rw-rw-   0        0        0     1920 2024-03-01 08:45:13.000000 funcs_aux-0.1.5/funcs_aux/strings.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:08:53.842234 funcs_aux-0.1.5/funcs_aux.egg-info/
+-rw-rw-rw-   0        0        0     1883 2024-05-16 09:08:53.000000 funcs_aux-0.1.5/funcs_aux.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      297 2024-05-16 09:08:53.000000 funcs_aux-0.1.5/funcs_aux.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 09:08:53.000000 funcs_aux-0.1.5/funcs_aux.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-16 09:08:53.000000 funcs_aux-0.1.5/funcs_aux.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 09:08:53.843238 funcs_aux-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 funcs_aux-0.1.5/setup.py
```

### Comparing `funcs_aux-0.1.4/LICENSE` & `funcs_aux-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.1.4/PKG-INFO` & `funcs_aux-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcs_aux
-Version: 0.1.4
+Version: 0.1.5
 Summary: useful funcs in one place
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/funcs_aux
 Keywords: functions,auxiliary,auxiliary funcs,np funcs,collections funcs,strings funcs,result object
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# funcs_aux (v0.1.4)
+# funcs_aux (v0.1.5)
 
 ## DESCRIPTION_SHORT
 useful funcs in one place
 
 ## DESCRIPTION_LONG
 Now its just a beginning!
 Designed to collect useful funcs in one place!
```

### Comparing `funcs_aux-0.1.4/README.md` & `funcs_aux-0.1.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# funcs_aux (v0.1.4)
+# funcs_aux (v0.1.5)
 
 ## DESCRIPTION_SHORT
 useful funcs in one place
 
 ## DESCRIPTION_LONG
 Now its just a beginning!
 Designed to collect useful funcs in one place!
```

### Comparing `funcs_aux-0.1.4/funcs_aux/arrays.py` & `funcs_aux-0.1.5/funcs_aux/arrays.py`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.1.4/funcs_aux/collects.py` & `funcs_aux-0.1.5/funcs_aux/collects.py`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.1.4/funcs_aux/iterables.py` & `funcs_aux-0.1.5/funcs_aux/iterables.py`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.1.4/funcs_aux/results.py` & `funcs_aux-0.1.5/funcs_aux/results.py`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.1.4/funcs_aux/strings.py` & `funcs_aux-0.1.5/funcs_aux/strings.py`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.1.4/funcs_aux.egg-info/PKG-INFO` & `funcs_aux-0.1.5/funcs_aux.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcs_aux
-Version: 0.1.4
+Version: 0.1.5
 Summary: useful funcs in one place
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/funcs_aux
 Keywords: functions,auxiliary,auxiliary funcs,np funcs,collections funcs,strings funcs,result object
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# funcs_aux (v0.1.4)
+# funcs_aux (v0.1.5)
 
 ## DESCRIPTION_SHORT
 useful funcs in one place
 
 ## DESCRIPTION_LONG
 Now its just a beginning!
 Designed to collect useful funcs in one place!
```

### Comparing `funcs_aux-0.1.4/setup.py` & `funcs_aux-0.1.5/setup.py`

 * *Files identical despite different names*

