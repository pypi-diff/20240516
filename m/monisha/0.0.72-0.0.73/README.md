# Comparing `tmp/monisha-0.0.72.tar.gz` & `tmp/monisha-0.0.73.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monisha-0.0.72.tar", last modified: Thu May 16 16:02:22 2024, max compression
+gzip compressed data, was "monisha-0.0.73.tar", last modified: Thu May 16 16:14:00 2024, max compression
```

## Comparing `monisha-0.0.72.tar` & `monisha-0.0.73.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:02:22.577378 monisha-0.0.72/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-16 16:02:18.000000 monisha-0.0.72/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:02:22.569378 monisha-0.0.72/Monisha/
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-16 16:02:18.000000 monisha-0.0.72/Monisha/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:02:22.573378 monisha-0.0.72/Monisha/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-16 16:02:18.000000 monisha-0.0.72/Monisha/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-16 16:02:18.000000 monisha-0.0.72/Monisha/functions/function01.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-16 16:02:18.000000 monisha-0.0.72/Monisha/functions/function02.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-16 16:02:18.000000 monisha-0.0.72/Monisha/functions/function03.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-16 16:02:18.000000 monisha-0.0.72/Monisha/functions/function04.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-16 16:02:18.000000 monisha-0.0.72/Monisha/functions/function05.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-16 16:02:18.000000 monisha-0.0.72/Monisha/functions/function06.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-16 16:02:18.000000 monisha-0.0.72/Monisha/functions/function07.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-16 16:02:18.000000 monisha-0.0.72/Monisha/functions/function08.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-16 16:02:18.000000 monisha-0.0.72/Monisha/functions/function09.py
--rw-r--r--   0 runner    (1001) docker     (127)    60666 2024-05-16 16:02:18.000000 monisha-0.0.72/Monisha/functions/function10.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-16 16:02:18.000000 monisha-0.0.72/Monisha/functions/function11.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-16 16:02:18.000000 monisha-0.0.72/Monisha/functions/function12.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-16 16:02:18.000000 monisha-0.0.72/Monisha/functions/function13.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-16 16:02:18.000000 monisha-0.0.72/Monisha/functions/function14.py
--rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-05-16 16:02:18.000000 monisha-0.0.72/Monisha/functions/function15.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-16 16:02:18.000000 monisha-0.0.72/Monisha/functions/function16.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-16 16:02:18.000000 monisha-0.0.72/Monisha/functions/function17.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-16 16:02:18.000000 monisha-0.0.72/Monisha/functions/function18.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-16 16:02:18.000000 monisha-0.0.72/Monisha/functions/function19.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-16 16:02:18.000000 monisha-0.0.72/Monisha/functions/function20.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:02:22.573378 monisha-0.0.72/Monisha/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-16 16:02:18.000000 monisha-0.0.72/Monisha/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-16 16:02:18.000000 monisha-0.0.72/Monisha/scripts/en.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-16 16:02:18.000000 monisha-0.0.72/Monisha/scripts/eo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-16 16:02:18.000000 monisha-0.0.72/Monisha/scripts/es.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-16 16:02:18.000000 monisha-0.0.72/Monisha/scripts/eu.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-16 16:02:22.577378 monisha-0.0.72/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-16 16:02:18.000000 monisha-0.0.72/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:02:22.577378 monisha-0.0.72/monisha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-16 16:02:22.000000 monisha-0.0.72/monisha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-16 16:02:22.000000 monisha-0.0.72/monisha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 16:02:22.000000 monisha-0.0.72/monisha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-16 16:02:22.000000 monisha-0.0.72/monisha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-16 16:02:22.000000 monisha-0.0.72/monisha.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 16:02:22.577378 monisha-0.0.72/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-16 16:02:18.000000 monisha-0.0.72/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:14:00.302676 monisha-0.0.73/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-16 16:13:56.000000 monisha-0.0.73/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:14:00.298676 monisha-0.0.73/Monisha/
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-16 16:13:56.000000 monisha-0.0.73/Monisha/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:14:00.302676 monisha-0.0.73/Monisha/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-16 16:13:56.000000 monisha-0.0.73/Monisha/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-16 16:13:56.000000 monisha-0.0.73/Monisha/functions/function01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-16 16:13:56.000000 monisha-0.0.73/Monisha/functions/function02.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-16 16:13:56.000000 monisha-0.0.73/Monisha/functions/function03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-16 16:13:56.000000 monisha-0.0.73/Monisha/functions/function04.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-16 16:13:56.000000 monisha-0.0.73/Monisha/functions/function05.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-16 16:13:56.000000 monisha-0.0.73/Monisha/functions/function06.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-16 16:13:56.000000 monisha-0.0.73/Monisha/functions/function07.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-16 16:13:56.000000 monisha-0.0.73/Monisha/functions/function08.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-16 16:13:56.000000 monisha-0.0.73/Monisha/functions/function09.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60666 2024-05-16 16:13:56.000000 monisha-0.0.73/Monisha/functions/function10.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-16 16:13:56.000000 monisha-0.0.73/Monisha/functions/function11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-16 16:13:56.000000 monisha-0.0.73/Monisha/functions/function12.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-16 16:13:56.000000 monisha-0.0.73/Monisha/functions/function13.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-16 16:13:56.000000 monisha-0.0.73/Monisha/functions/function14.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-05-16 16:13:56.000000 monisha-0.0.73/Monisha/functions/function15.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-16 16:13:56.000000 monisha-0.0.73/Monisha/functions/function16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-16 16:13:56.000000 monisha-0.0.73/Monisha/functions/function17.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-16 16:13:56.000000 monisha-0.0.73/Monisha/functions/function18.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-16 16:13:56.000000 monisha-0.0.73/Monisha/functions/function19.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-16 16:13:56.000000 monisha-0.0.73/Monisha/functions/function20.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:14:00.302676 monisha-0.0.73/Monisha/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-16 16:13:56.000000 monisha-0.0.73/Monisha/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-16 16:13:56.000000 monisha-0.0.73/Monisha/scripts/en.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-16 16:13:56.000000 monisha-0.0.73/Monisha/scripts/eo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-16 16:13:56.000000 monisha-0.0.73/Monisha/scripts/es.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-16 16:13:56.000000 monisha-0.0.73/Monisha/scripts/eu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-16 16:14:00.302676 monisha-0.0.73/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-16 16:13:56.000000 monisha-0.0.73/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:14:00.302676 monisha-0.0.73/monisha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-16 16:14:00.000000 monisha-0.0.73/monisha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-16 16:14:00.000000 monisha-0.0.73/monisha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 16:14:00.000000 monisha-0.0.73/monisha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-16 16:14:00.000000 monisha-0.0.73/monisha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-16 16:14:00.000000 monisha-0.0.73/monisha.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 16:14:00.302676 monisha-0.0.73/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-16 16:13:56.000000 monisha-0.0.73/setup.py
```

### Comparing `monisha-0.0.72/LICENSE` & `monisha-0.0.73/LICENSE`

 * *Files identical despite different names*

### Comparing `monisha-0.0.72/Monisha/__init__.py` & `monisha-0.0.73/Monisha/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 appname = "monisha"
-version = "0.0.72"
+version = "0.0.73"
 
 install = ["hachoir",
            "requests",
            "beautifulsoup4"]
 
 DATA01 = "clintonabrahamc@gmail.com"
 DATA02 = ['Natural Language :: English',
```

### Comparing `monisha-0.0.72/Monisha/functions/__init__.py` & `monisha-0.0.73/Monisha/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.72/Monisha/functions/function01.py` & `monisha-0.0.73/Monisha/functions/function01.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.72/Monisha/functions/function02.py` & `monisha-0.0.73/Monisha/functions/function02.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.72/Monisha/functions/function03.py` & `monisha-0.0.73/Monisha/functions/function03.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.72/Monisha/functions/function04.py` & `monisha-0.0.73/Monisha/functions/function04.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.72/Monisha/functions/function06.py` & `monisha-0.0.73/Monisha/functions/function06.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.72/Monisha/functions/function07.py` & `monisha-0.0.73/Monisha/functions/function07.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.72/Monisha/functions/function10.py` & `monisha-0.0.73/Monisha/functions/function10.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.72/Monisha/functions/function14.py` & `monisha-0.0.73/Monisha/functions/function14.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.72/Monisha/functions/function15.py` & `monisha-0.0.73/Monisha/functions/function15.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,35 +11,26 @@
         self.allfiles = kwargs.get('allfiles', None)
         self.location = kwargs.get('location', None)
 
 #=================================================================================================
 
 class Location:
 
-    async def get05(directory, stored=[], skip=Eimes.DATA00):
+    async def get04(directory, stored=[], skip=Eimes.DATA00):
         for patho in directory:
             if patho.upper().endswith(skip):
                 continue
             else:
                 stored.append(patho)
 
         stored.sort()
         return Messages(allfiles=stored, numfiles=len(stored))
 
 #=================================================================================================
     
-    async def get04(directory, stored=[]):
-        for item in directory:
-            stored.append(str(item))
-
-        stored.sort()
-        return Messages(allfiles=stored, numfiles=len(stored))
-
-#=================================================================================================
-    
     async def get03(directory, stored=[]):
         for item in Path(directory).rglob('*'):
             if os.path.isdir(item):
                 continue
             else:
                 stored.append(str(item))
```

### Comparing `monisha-0.0.72/Monisha/functions/function16.py` & `monisha-0.0.73/Monisha/functions/function16.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.72/Monisha/functions/function17.py` & `monisha-0.0.73/Monisha/functions/function17.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.72/Monisha/functions/function18.py` & `monisha-0.0.73/Monisha/functions/function18.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.72/Monisha/functions/function19.py` & `monisha-0.0.73/Monisha/functions/function19.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.72/Monisha/functions/function20.py` & `monisha-0.0.73/Monisha/functions/function20.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.72/Monisha/scripts/es.py` & `monisha-0.0.73/Monisha/scripts/es.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.72/PKG-INFO` & `monisha-0.0.73/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monisha
-Version: 0.0.72
+Version: 0.0.73
 Summary: ㅤ
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,clinton,abraham
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: monisha Version: 0.0.72 Summary: ã¤ Home-page:
+Metadata-Version: 2.1 Name: monisha Version: 0.0.73 Summary: ã¤ Home-page:
 https://github.com/Clinton-Abraham Author: Clinton-Abraham Author-email:
 clintonabrahamc@gmail.com License: MIT Keywords: python,clinton,abraham
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
```

### Comparing `monisha-0.0.72/monisha.egg-info/PKG-INFO` & `monisha-0.0.73/monisha.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monisha
-Version: 0.0.72
+Version: 0.0.73
 Summary: ㅤ
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,clinton,abraham
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: monisha Version: 0.0.72 Summary: ã¤ Home-page:
+Metadata-Version: 2.1 Name: monisha Version: 0.0.73 Summary: ã¤ Home-page:
 https://github.com/Clinton-Abraham Author: Clinton-Abraham Author-email:
 clintonabrahamc@gmail.com License: MIT Keywords: python,clinton,abraham
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
```

### Comparing `monisha-0.0.72/monisha.egg-info/SOURCES.txt` & `monisha-0.0.73/monisha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `monisha-0.0.72/setup.py` & `monisha-0.0.73/setup.py`

 * *Files identical despite different names*

