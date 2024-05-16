# Comparing `tmp/JustDeepIt-0.2.1.tar.gz` & `tmp/JustDeepIt-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "justdeepit-0.2.1.tar", last modified: Sat May  4 20:25:12 2024, max compression
+gzip compressed data, was "JustDeepIt-0.2.2.tar", last modified: Thu May 16 06:15:03 2024, max compression
```

## Comparing `JustDeepIt-0.2.1.tar` & `JustDeepIt-0.2.2.tar`

### file list

```diff
@@ -1,58 +1,53 @@
-drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-05-04 20:25:12.150634 justdeepit-0.2.1/
-drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-05-04 20:25:12.150049 justdeepit-0.2.1/JustDeepIt.egg-info/
--rw-r--r--   0 sonk414    (501) staff       (20)     2103 2024-05-04 20:25:12.000000 justdeepit-0.2.1/JustDeepIt.egg-info/PKG-INFO
--rw-r--r--   0 sonk414    (501) staff       (20)     1315 2024-05-04 20:25:12.000000 justdeepit-0.2.1/JustDeepIt.egg-info/SOURCES.txt
--rw-r--r--   0 sonk414    (501) staff       (20)        1 2024-05-04 20:25:12.000000 justdeepit-0.2.1/JustDeepIt.egg-info/dependency_links.txt
--rw-r--r--   0 sonk414    (501) staff       (20)       58 2024-05-04 20:25:12.000000 justdeepit-0.2.1/JustDeepIt.egg-info/entry_points.txt
--rw-r--r--   0 sonk414    (501) staff       (20)      145 2024-05-04 20:25:12.000000 justdeepit-0.2.1/JustDeepIt.egg-info/requires.txt
--rw-r--r--   0 sonk414    (501) staff       (20)       11 2024-05-04 20:25:12.000000 justdeepit-0.2.1/JustDeepIt.egg-info/top_level.txt
--rw-r--r--   0 sonk414    (501) staff       (20)        1 2024-05-04 20:23:49.000000 justdeepit-0.2.1/JustDeepIt.egg-info/zip-safe
--rw-r--r--   0 sonk414    (501) staff       (20)     1070 2024-05-04 20:22:08.000000 justdeepit-0.2.1/LICENSE
--rw-r--r--   0 sonk414    (501) staff       (20)      122 2024-05-04 20:22:31.000000 justdeepit-0.2.1/MANIFEST.in
--rw-r--r--   0 sonk414    (501) staff       (20)     2103 2024-05-04 20:25:12.150374 justdeepit-0.2.1/PKG-INFO
--rw-r--r--   0 sonk414    (501) staff       (20)     1426 2024-05-04 20:22:08.000000 justdeepit-0.2.1/README.md
-drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-05-04 20:25:12.132894 justdeepit-0.2.1/justdeepit/
--rw-r--r--   0 sonk414    (501) staff       (20)       95 2024-05-04 20:23:07.000000 justdeepit-0.2.1/justdeepit/__init__.py
-drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-05-04 20:25:12.137290 justdeepit-0.2.1/justdeepit/app/
--rw-r--r--   0 sonk414    (501) staff       (20)      162 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/app/__init__.py
--rw-r--r--   0 sonk414    (501) staff       (20)    25983 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/app/app.py
--rw-r--r--   0 sonk414    (501) staff       (20)     5692 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/app/appbase.py
--rw-r--r--   0 sonk414    (501) staff       (20)      554 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/app/appis.py
--rw-r--r--   0 sonk414    (501) staff       (20)    10048 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/app/appod.py
--rw-r--r--   0 sonk414    (501) staff       (20)    22300 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/app/appsod.py
-drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-05-04 20:25:12.141555 justdeepit-0.2.1/justdeepit/app/static/
--rw-r--r--   0 sonk414    (501) staff       (20)    89501 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/app/static/jquery-3.6.0.min.js
--rw-r--r--   0 sonk414    (501) staff       (20)   137972 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/app/static/jquery-3.6.0.min.map
--rw-r--r--   0 sonk414    (501) staff       (20)    14483 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/app/static/styles.css
--rw-r--r--   0 sonk414    (501) staff       (20)    58702 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/app/static/tree.jquery.js
--rw-r--r--   0 sonk414    (501) staff       (20)   174878 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/app/static/tree.jquery.js.map
--rw-r--r--   0 sonk414    (501) staff       (20)    22813 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/app/static/utils.js
-drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-05-04 20:25:12.142487 justdeepit-0.2.1/justdeepit/app/templates/
--rw-r--r--   0 sonk414    (501) staff       (20)     1187 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/app/templates/index.html
--rw-r--r--   0 sonk414    (501) staff       (20)    17293 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/app/templates/module.html
--rw-r--r--   0 sonk414    (501) staff       (20)      560 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/app/templates/shutdown.html
-drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-05-04 20:25:12.144447 justdeepit-0.2.1/justdeepit/models/
--rw-r--r--   0 sonk414    (501) staff       (20)      184 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/models/__init__.py
--rw-r--r--   0 sonk414    (501) staff       (20)      309 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/models/abstract.py
--rw-r--r--   0 sonk414    (501) staff       (20)    12931 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/models/instance_segment.py
--rw-r--r--   0 sonk414    (501) staff       (20)    13500 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/models/object_detect.py
--rw-r--r--   0 sonk414    (501) staff       (20)    12227 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/models/salient_object_detect.py
-drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-05-04 20:25:12.146013 justdeepit-0.2.1/justdeepit/models/utils/
--rw-r--r--   0 sonk414    (501) staff       (20)        0 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/models/utils/__init__.py
--rw-r--r--   0 sonk414    (501) staff       (20)     6720 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/models/utils/data.py
--rw-r--r--   0 sonk414    (501) staff       (20)    11507 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/models/utils/mmdetbase.py
--rw-r--r--   0 sonk414    (501) staff       (20)    36052 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/models/utils/u2net.py
--rw-r--r--   0 sonk414    (501) staff       (20)    10173 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/models/utils/unet.py
-drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-05-04 20:25:12.130293 justdeepit-0.2.1/justdeepit/src/
-drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-05-04 20:25:12.148009 justdeepit-0.2.1/justdeepit/src/font/
--rw-r--r--   0 sonk414    (501) staff       (20)   555264 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/src/font/NotoSans-Medium.ttf
--rw-r--r--   0 sonk414    (501) staff       (20)     4449 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/src/font/OFL.txt
--rw-r--r--   0 sonk414    (501) staff       (20)    56860 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/utils.py
--rw-r--r--   0 sonk414    (501) staff       (20)      151 2024-05-04 20:22:08.000000 justdeepit-0.2.1/requirements.txt
--rw-r--r--   0 sonk414    (501) staff       (20)       38 2024-05-04 20:25:12.150692 justdeepit-0.2.1/setup.cfg
--rw-r--r--   0 sonk414    (501) staff       (20)     2649 2024-05-04 20:22:08.000000 justdeepit-0.2.1/setup.py
-drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-05-04 20:25:12.149549 justdeepit-0.2.1/tests/
--rw-r--r--   0 sonk414    (501) staff       (20)     3656 2024-05-04 20:22:08.000000 justdeepit-0.2.1/tests/test_det.py
--rw-r--r--   0 sonk414    (501) staff       (20)     2304 2024-05-04 20:22:08.000000 justdeepit-0.2.1/tests/test_segm.py
--rw-r--r--   0 sonk414    (501) staff       (20)     3139 2024-05-04 20:22:08.000000 justdeepit-0.2.1/tests/test_sodmodels.py
--rw-r--r--   0 sonk414    (501) staff       (20)     6933 2024-05-04 20:22:08.000000 justdeepit-0.2.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:15:03.257052 JustDeepIt-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:15:03.253052 JustDeepIt-0.2.2/JustDeepIt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-16 06:15:03.000000 JustDeepIt-0.2.2/JustDeepIt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-16 06:15:03.000000 JustDeepIt-0.2.2/JustDeepIt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 06:15:03.000000 JustDeepIt-0.2.2/JustDeepIt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-16 06:15:03.000000 JustDeepIt-0.2.2/JustDeepIt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-16 06:15:03.000000 JustDeepIt-0.2.2/JustDeepIt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-16 06:15:03.000000 JustDeepIt-0.2.2/JustDeepIt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 06:15:03.000000 JustDeepIt-0.2.2/JustDeepIt.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-16 06:15:03.257052 JustDeepIt-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:15:03.253052 JustDeepIt-0.2.2/justdeepit/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:15:03.253052 JustDeepIt-0.2.2/justdeepit/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25983 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/app/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/app/appbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/app/appis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10048 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/app/appod.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22300 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/app/appsod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:15:03.253052 JustDeepIt-0.2.2/justdeepit/app/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    89501 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/app/static/jquery-3.6.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   137972 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/app/static/jquery-3.6.0.min.map
+-rw-r--r--   0 runner    (1001) docker     (127)    14483 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/app/static/styles.css
+-rw-r--r--   0 runner    (1001) docker     (127)    58702 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/app/static/tree.jquery.js
+-rw-r--r--   0 runner    (1001) docker     (127)   174878 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/app/static/tree.jquery.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    22813 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/app/static/utils.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:15:03.253052 JustDeepIt-0.2.2/justdeepit/app/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/app/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    17293 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/app/templates/module.html
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/app/templates/shutdown.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:15:03.257052 JustDeepIt-0.2.2/justdeepit/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/models/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12931 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/models/instance_segment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13500 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/models/object_detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12227 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/models/salient_object_detect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:15:03.257052 JustDeepIt-0.2.2/justdeepit/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/models/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13883 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/models/utils/mmdetbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36052 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/models/utils/u2net.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10173 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/models/utils/unet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:15:03.249052 JustDeepIt-0.2.2/justdeepit/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:15:03.257052 JustDeepIt-0.2.2/justdeepit/src/font/
+-rw-r--r--   0 runner    (1001) docker     (127)   555264 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/src/font/NotoSans-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/src/font/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    56860 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/justdeepit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 06:15:03.257052 JustDeepIt-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-16 06:13:09.000000 JustDeepIt-0.2.2/setup.py
```

### Comparing `justdeepit-0.2.1/JustDeepIt.egg-info/SOURCES.txt` & `JustDeepIt-0.2.2/JustDeepIt.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -34,12 +34,8 @@
 justdeepit/models/salient_object_detect.py
 justdeepit/models/utils/__init__.py
 justdeepit/models/utils/data.py
 justdeepit/models/utils/mmdetbase.py
 justdeepit/models/utils/u2net.py
 justdeepit/models/utils/unet.py
 justdeepit/src/font/NotoSans-Medium.ttf
-justdeepit/src/font/OFL.txt
-tests/test_det.py
-tests/test_segm.py
-tests/test_sodmodels.py
-tests/test_utils.py
+justdeepit/src/font/OFL.txt
```

### Comparing `justdeepit-0.2.1/LICENSE` & `JustDeepIt-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.1/README.md` & `JustDeepIt-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.1/justdeepit/app/app.py` & `JustDeepIt-0.2.2/justdeepit/app/app.py`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.1/justdeepit/app/appbase.py` & `JustDeepIt-0.2.2/justdeepit/app/appbase.py`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.1/justdeepit/app/appis.py` & `JustDeepIt-0.2.2/justdeepit/app/appis.py`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.1/justdeepit/app/appod.py` & `JustDeepIt-0.2.2/justdeepit/app/appod.py`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.1/justdeepit/app/appsod.py` & `JustDeepIt-0.2.2/justdeepit/app/appsod.py`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.1/justdeepit/app/static/jquery-3.6.0.min.js` & `JustDeepIt-0.2.2/justdeepit/app/static/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.1/justdeepit/app/static/jquery-3.6.0.min.map` & `JustDeepIt-0.2.2/justdeepit/app/static/jquery-3.6.0.min.map`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.1/justdeepit/app/static/styles.css` & `JustDeepIt-0.2.2/justdeepit/app/static/styles.css`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.1/justdeepit/app/static/tree.jquery.js` & `JustDeepIt-0.2.2/justdeepit/app/static/tree.jquery.js`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.1/justdeepit/app/static/tree.jquery.js.map` & `JustDeepIt-0.2.2/justdeepit/app/static/tree.jquery.js.map`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.1/justdeepit/app/static/utils.js` & `JustDeepIt-0.2.2/justdeepit/app/static/utils.js`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.1/justdeepit/app/templates/index.html` & `JustDeepIt-0.2.2/justdeepit/app/templates/index.html`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.1/justdeepit/app/templates/module.html` & `JustDeepIt-0.2.2/justdeepit/app/templates/module.html`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.1/justdeepit/app/templates/shutdown.html` & `JustDeepIt-0.2.2/justdeepit/app/templates/shutdown.html`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.1/justdeepit/models/instance_segment.py` & `JustDeepIt-0.2.2/justdeepit/models/instance_segment.py`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.1/justdeepit/models/object_detect.py` & `JustDeepIt-0.2.2/justdeepit/models/object_detect.py`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.1/justdeepit/models/salient_object_detect.py` & `JustDeepIt-0.2.2/justdeepit/models/salient_object_detect.py`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.1/justdeepit/models/utils/data.py` & `JustDeepIt-0.2.2/justdeepit/models/utils/data.py`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.1/justdeepit/models/utils/mmdetbase.py` & `JustDeepIt-0.2.2/justdeepit/models/utils/mmdetbase.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import glob
 import math
 import tqdm
 import tempfile
 import logging
 import datetime
 import numpy as np
+import pandas as pd
 import skimage
 import skimage.measure
 import PIL
 import torch
 import torch.multiprocessing
 from justdeepit.models.abstract import ModuleTemplate, JDIError
 from justdeepit.utils import ImageAnnotation, ImageAnnotations, load_images
@@ -55,28 +56,28 @@
                  model_arch=None,
                  model_config=None,
                  model_weight=None,
                  model_class=None,
                  workspace=None,
                  seed=None):
         
-        # model settings
-        self.model_arch = model_arch
-        self.class_labels = DataClass(class_labels)
-        self.model_class = model_class
-        self.cfg_fpath = model_config
-        self.cfg = self.__set_config(model_config, model_weight, self.class_labels.class_labels)
-        
         # workspace
         self.tempd = None
         if workspace is None:
             self.tempd = tempfile.TemporaryDirectory()
             self.workspace = self.tempd.name
         else:
             self.workspace = workspace
+
+        # model settings
+        self.model_arch = model_arch
+        self.class_labels = DataClass(class_labels)
+        self.model_class = model_class
+        self.cfg_fpath = model_config
+        self.cfg = self.__set_config(model_config, model_weight, self.class_labels.class_labels)
         self.cfg.work_dir = os.path.abspath(self.workspace)
         logger.info(f'The workspace is set to `{self.workspace}`. '
                     f'Please locate the intermediate and final results '
                     f'within this workspace.')
         
         # random seed
         if seed is None:
@@ -170,30 +171,30 @@
         
         # CPU/GPUs
         self.__set_device(gpu)
 
         # training params
         self.__set_optimizer(optimizer)
         self.__set_scheduler(scheduler)
-       
+        
         # datasets
         if self.model_class == 'od':
             dataloader = DataLoader(self.cfg,
                                     train_dataset, valid_dataset, test_dataset,
                                     batchsize, epoch, cpu,
                                     with_bbox=True, with_mask=False)
         elif self.model_class == 'is':
             dataloader = DataLoader(self.cfg,
                                     train_dataset, valid_dataset, test_dataset,
                                     batchsize, epoch, cpu,
                                     with_bbox=True, with_mask=True)
         else:
             raise ValueError('The model class is not supported.')
         self.cfg.merge_from_dict(dataloader.cfg)
-        self.cfg.default_hooks.checkpoint.interval = 20
+        self.cfg.default_hooks.checkpoint.interval = 10
 
         # training
         runner = mmengine.runner.Runner.from_cfg(self.cfg)
         runner.train()
     
     
     
@@ -204,40 +205,97 @@
         gpu = gpu if torch.cuda.is_available() else 0
         gpu = torch.cuda.device_count() if torch.cuda.device_count() < gpu else gpu
         self.cfg.device = 'cuda:0' if gpu > 0 else 'cpu'
     
 
     
     def __set_optimizer(self, optimizer):
-        if optimizer is not None and optimizer.replace(' ', '') != '':
-            if optimizer[0] != '{' or optimizer[0:4] != 'dict':
-                optimizer = 'dict(' + optimizer + ')'
-            self.cfg.optimizer = eval(optimizer)
+        if optimizer is not None:
+            if isinstance(optimizer, dict):
+                opt_dict = optimizer
+            elif isinstance(optimizer, str) and optimizer.replace(' ', '') != '':
+                if optimizer[0] != '{' and optimizer[0:4] != 'dict':
+                    optimizer = 'dict(' + optimizer + ')'
+                opt_dict = eval(optimizer)
+            self.cfg.optim_wrapper = dict(optimizer=opt_dict, type='OptimWrapper')
     
     
 
     def __set_scheduler(self, scheduler):
-        if scheduler is not None and scheduler.replace(' ', '') != '':
-            if scheduler[0] != '{' or scheduler[0:4] != 'dict':
-                scheduler = 'dict(' + scheduler + ')'
-            self.cfg.scheduler = eval(scheduler)
+        if scheduler is not None:
+            if isinstance(scheduler, list) or isinstance(scheduler, tuple):
+                scheduler_dict = scheduler
+            elif isinstance(scheduler, str) and scheduler.replace(' ', '') != '':
+                if scheduler[0] == '[':
+                    pass
+                else:
+                    if scheduler[0] == '{' or scheduler[0:4] == 'dict':
+                        scheduler = '[' + scheduler + ']'
+                    else:
+                        scheduler = '[dict(' + scheduler + ')]'
+                scheduler_dict = eval(scheduler)
+            self.cfg.param_scheduler = scheduler_dict
     
 
 
     def save(self, weight_fpath, config_fpath=None):
         # weight
         if not weight_fpath.endswith('.pth'):
             weight_fpath + '.pth'
         with open(os.path.join(self.cfg.work_dir, 'last_checkpoint')) as chkf:
-            last_chk = chkf.readline().strip()
-            shutil.copy2(last_chk, weight_fpath)
+            shutil.copy2(chkf.readline().strip(), weight_fpath)
         # config
         if config_fpath is None:
             config_fpath = os.path.splitext(weight_fpath)[0] + '.py'
         self.cfg.dump(config_fpath)
+        # train log
+        self.parse_trainlog(os.path.splitext(weight_fpath)[0] + '.log')
+
+
+
+    def parse_trainlog(self, output_prefix=None):
+        # get the latest log files
+        latest_log_dpath = self.__get_latest_trainlog(self.cfg.work_dir)
+        
+        train_log = []
+        valid_log = []
+        test_log = []
+
+        with open(latest_log_dpath) as fh:
+            for log_line in fh:
+                if 'coco/bbox_mAP' in log_line:
+                    valid_log.append(log_line)
+                else:
+                    train_log.append(log_line)
+
+        train_log = pd.DataFrame(json.loads('[' + ','.join(train_log) + ']')).groupby('epoch').sum().drop(columns=['iter', 'step'])
+
+        if output_prefix is not None:
+            train_log.to_csv(output_prefix + '.train.txt',
+                header=True, index=True, sep='\t')
+
+        if output_prefix is not None and len(valid_log) > 0:
+            pd.DataFrame(json.loads('[' + ','.join(valid_log) + ']')).to_csv(output_prefix + '.valid.txt',
+                header=True, index=False, sep='\t')
+
+
+
+    def __get_latest_trainlog(self, log_dpath):
+        latest_log_dpath = None
+        max_timestamp_ = 0
+        for fpath in glob.glob(os.path.join(log_dpath, '*')):
+            if os.path.isdir(fpath):
+                log_dpath = os.path.basename(fpath)
+                if len(os.path.basename(log_dpath)) == 15 and log_dpath[8] == '_':
+                    timesamp_ = int(log_dpath[0:8] + log_dpath[9:])
+                    if timesamp_ > max_timestamp_:
+                        max_timestamp_ = timesamp_
+                        latest_log_dpath = os.path.join(self.cfg.work_dir, log_dpath,
+                            'vis_data', 'scalars.json')
+        return latest_log_dpath
 
 
 
     def inference(self,
                   images,
                   score_cutoff=0.5,
                   batchsize=8,
@@ -251,33 +309,32 @@
         assert len(target_images) > 0, 'No images found in {}'.format(images)
         
         # set params
         pipeline = DataPipeline()
         self.cfg.merge_from_dict(
             dict(test_dataloader=dict(
                 _delete_=True,
-                batch_size=1,
+                batch_size=batchsize,
                 num_workers=cpu,
                 persistent_workers=True,
                 drop_last=False,
                 sampler=dict(type='DefaultSampler', shuffle=False),
                 dataset=dict(
                     type='CocoDataset',
                     pipeline = pipeline.inference,
                     metainfo=self.cfg.metainfo))))
 
-
         # load model
         model = mmdet.apis.init_detector(self.cfg,
                                          self.cfg.load_from,
                                          device=self.cfg.device)
         
         # inference
         outputs = mmdet.apis.inference_detector(model, target_images)
-
+        
         # format
         outputs_fmt = []
         for target_image, output in zip(target_images, outputs):
             outputs_fmt.append(
                 ImageAnnotation(target_image,
                                 self.__format_annotation(output,
                                                          score_cutoff)))
```

### Comparing `justdeepit-0.2.1/justdeepit/models/utils/u2net.py` & `JustDeepIt-0.2.2/justdeepit/models/utils/u2net.py`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.1/justdeepit/models/utils/unet.py` & `JustDeepIt-0.2.2/justdeepit/models/utils/unet.py`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.1/justdeepit/src/font/NotoSans-Medium.ttf` & `JustDeepIt-0.2.2/justdeepit/src/font/NotoSans-Medium.ttf`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.1/justdeepit/src/font/OFL.txt` & `JustDeepIt-0.2.2/justdeepit/src/font/OFL.txt`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.1/justdeepit/utils.py` & `JustDeepIt-0.2.2/justdeepit/utils.py`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.1/setup.py` & `JustDeepIt-0.2.2/setup.py`

 * *Files identical despite different names*

