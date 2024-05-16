# Comparing `tmp/funcs_aux-0.1.5.tar.gz` & `tmp/funcs_aux-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcs_aux-0.1.5.tar", last modified: Thu May 16 09:08:53 2024, max compression
+gzip compressed data, was "funcs_aux-0.1.6.tar", last modified: Thu May 16 11:37:34 2024, max compression
```

## Comparing `funcs_aux-0.1.5.tar` & `funcs_aux-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 09:08:53.843238 funcs_aux-0.1.5/
--rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 funcs_aux-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     1883 2024-05-16 09:08:53.842234 funcs_aux-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      990 2024-05-16 09:08:23.000000 funcs_aux-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 09:08:53.836120 funcs_aux-0.1.5/funcs_aux/
--rw-rw-rw-   0        0        0      301 2024-05-16 09:08:23.000000 funcs_aux-0.1.5/funcs_aux/__init__.py
--rw-rw-rw-   0        0        0     1894 2024-03-01 08:49:51.000000 funcs_aux-0.1.5/funcs_aux/arrays.py
--rw-rw-rw-   0        0        0     6005 2024-03-28 14:40:09.000000 funcs_aux-0.1.5/funcs_aux/collects.py
--rw-rw-rw-   0        0        0     5211 2024-03-22 14:19:18.000000 funcs_aux-0.1.5/funcs_aux/iterables.py
--rw-rw-rw-   0        0        0     9772 2024-05-16 08:59:28.000000 funcs_aux-0.1.5/funcs_aux/results.py
--rw-rw-rw-   0        0        0     1920 2024-03-01 08:45:13.000000 funcs_aux-0.1.5/funcs_aux/strings.py
-drwxrwxrwx   0        0        0        0 2024-05-16 09:08:53.842234 funcs_aux-0.1.5/funcs_aux.egg-info/
--rw-rw-rw-   0        0        0     1883 2024-05-16 09:08:53.000000 funcs_aux-0.1.5/funcs_aux.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2024-05-16 09:08:53.000000 funcs_aux-0.1.5/funcs_aux.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 09:08:53.000000 funcs_aux-0.1.5/funcs_aux.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-16 09:08:53.000000 funcs_aux-0.1.5/funcs_aux.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 09:08:53.843238 funcs_aux-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 funcs_aux-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 11:37:34.484859 funcs_aux-0.1.6/
+-rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 funcs_aux-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     1883 2024-05-16 11:37:34.483852 funcs_aux-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      990 2024-05-16 11:37:12.000000 funcs_aux-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 11:37:34.476386 funcs_aux-0.1.6/funcs_aux/
+-rw-rw-rw-   0        0        0      301 2024-05-16 09:08:23.000000 funcs_aux-0.1.6/funcs_aux/__init__.py
+-rw-rw-rw-   0        0        0     1894 2024-03-01 08:49:51.000000 funcs_aux-0.1.6/funcs_aux/arrays.py
+-rw-rw-rw-   0        0        0     6005 2024-03-28 14:40:09.000000 funcs_aux-0.1.6/funcs_aux/collects.py
+-rw-rw-rw-   0        0        0     5211 2024-03-22 14:19:18.000000 funcs_aux-0.1.6/funcs_aux/iterables.py
+-rw-rw-rw-   0        0        0     9793 2024-05-16 11:37:12.000000 funcs_aux-0.1.6/funcs_aux/results.py
+-rw-rw-rw-   0        0        0     1920 2024-03-01 08:45:13.000000 funcs_aux-0.1.6/funcs_aux/strings.py
+drwxrwxrwx   0        0        0        0 2024-05-16 11:37:34.482940 funcs_aux-0.1.6/funcs_aux.egg-info/
+-rw-rw-rw-   0        0        0     1883 2024-05-16 11:37:34.000000 funcs_aux-0.1.6/funcs_aux.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      297 2024-05-16 11:37:34.000000 funcs_aux-0.1.6/funcs_aux.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 11:37:34.000000 funcs_aux-0.1.6/funcs_aux.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-16 11:37:34.000000 funcs_aux-0.1.6/funcs_aux.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 11:37:34.486119 funcs_aux-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 funcs_aux-0.1.6/setup.py
```

### Comparing `funcs_aux-0.1.5/LICENSE` & `funcs_aux-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.1.5/PKG-INFO` & `funcs_aux-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcs_aux
-Version: 0.1.5
+Version: 0.1.6
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
 
-# funcs_aux (v0.1.5)
+# funcs_aux (v0.1.6)
 
 ## DESCRIPTION_SHORT
 useful funcs in one place
 
 ## DESCRIPTION_LONG
 Now its just a beginning!
 Designed to collect useful funcs in one place!
```

### Comparing `funcs_aux-0.1.5/README.md` & `funcs_aux-0.1.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# funcs_aux (v0.1.5)
+# funcs_aux (v0.1.6)
 
 ## DESCRIPTION_SHORT
 useful funcs in one place
 
 ## DESCRIPTION_LONG
 Now its just a beginning!
 Designed to collect useful funcs in one place!
```

### Comparing `funcs_aux-0.1.5/funcs_aux/arrays.py` & `funcs_aux-0.1.6/funcs_aux/arrays.py`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.1.5/funcs_aux/collects.py` & `funcs_aux-0.1.6/funcs_aux/collects.py`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.1.5/funcs_aux/iterables.py` & `funcs_aux-0.1.6/funcs_aux/iterables.py`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.1.5/funcs_aux/results.py` & `funcs_aux-0.1.6/funcs_aux/results.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,15 +198,15 @@
         return self.STEP__RESULT
 
     def __str__(self) -> str:
         return "\n".join(self.MSGS)
 
     @property
     def MSG(self) -> str:
-        result = f"ResultExpect[index={self.STEP__INDEX}/result={self.STEP__RESULT}//title={self.TITLE}]"
+        result = f"ResultExpect[index={self.STEP__INDEX}/result={self.STEP__RESULT}/exx={self.STEP__EXX}//title={self.TITLE}]"
         return result
 
     @property
     def MSGS(self) -> list[str]:
         """here it is useful to keep universal access to MSGS both to STEP/CHAIN
         """
         return [self.MSG, ]
```

### Comparing `funcs_aux-0.1.5/funcs_aux/strings.py` & `funcs_aux-0.1.6/funcs_aux/strings.py`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.1.5/funcs_aux.egg-info/PKG-INFO` & `funcs_aux-0.1.6/funcs_aux.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcs_aux
-Version: 0.1.5
+Version: 0.1.6
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
 
-# funcs_aux (v0.1.5)
+# funcs_aux (v0.1.6)
 
 ## DESCRIPTION_SHORT
 useful funcs in one place
 
 ## DESCRIPTION_LONG
 Now its just a beginning!
 Designed to collect useful funcs in one place!
```

### Comparing `funcs_aux-0.1.5/setup.py` & `funcs_aux-0.1.6/setup.py`

 * *Files identical despite different names*

