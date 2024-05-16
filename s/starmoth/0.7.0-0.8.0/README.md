# Comparing `tmp/starmoth-0.7.0.tar.gz` & `tmp/starmoth-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starmoth-0.7.0.tar", last modified: Fri Apr 26 17:12:38 2024, max compression
+gzip compressed data, was "starmoth-0.8.0.tar", last modified: Thu May 16 14:53:46 2024, max compression
```

## Comparing `starmoth-0.7.0.tar` & `starmoth-0.8.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 17:12:37.998340 starmoth-0.7.0/
--rw-r--r--   0 root         (0) root         (0)     3921 2024-04-26 17:12:37.998340 starmoth-0.7.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3549 2024-04-23 20:53:43.000000 starmoth-0.7.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 17:12:37.994340 starmoth-0.7.0/moth/
--rw-rw-rw-   0 root         (0) root         (0)     4670 2024-04-23 20:53:43.000000 starmoth-0.7.0/moth/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 17:12:37.994340 starmoth-0.7.0/moth/cli/
--rw-rw-rw-   0 root         (0) root         (0)     1925 2024-04-23 20:53:43.000000 starmoth-0.7.0/moth/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 17:12:37.994340 starmoth-0.7.0/moth/driver/
--rw-rw-rw-   0 root         (0) root         (0)     2121 2024-04-23 20:53:43.000000 starmoth-0.7.0/moth/driver/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 17:12:37.994340 starmoth-0.7.0/moth/message/
--rw-rw-rw-   0 root         (0) root         (0)     9396 2024-04-26 17:11:22.000000 starmoth-0.7.0/moth/message/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      156 2024-04-23 20:53:43.000000 starmoth-0.7.0/moth/message/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 17:12:37.994340 starmoth-0.7.0/moth/server/
--rw-rw-rw-   0 root         (0) root         (0)     5976 2024-04-23 20:53:43.000000 starmoth-0.7.0/moth/server/__init__.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-26 17:12:37.998340 starmoth-0.7.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      853 2024-04-23 20:53:43.000000 starmoth-0.7.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 17:12:37.998340 starmoth-0.7.0/starmoth.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3921 2024-04-26 17:12:37.000000 starmoth-0.7.0/starmoth.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      350 2024-04-26 17:12:37.000000 starmoth-0.7.0/starmoth.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 17:12:37.000000 starmoth-0.7.0/starmoth.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-26 17:12:37.000000 starmoth-0.7.0/starmoth.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-04-26 17:12:37.000000 starmoth-0.7.0/starmoth.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-04-26 17:12:37.000000 starmoth-0.7.0/starmoth.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 14:53:46.441616 starmoth-0.8.0/
+-rw-r--r--   0 root         (0) root         (0)     3921 2024-05-16 14:53:46.441616 starmoth-0.8.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3549 2024-04-23 20:53:43.000000 starmoth-0.8.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 14:53:46.433615 starmoth-0.8.0/moth/
+-rw-rw-rw-   0 root         (0) root         (0)     4670 2024-04-23 20:53:43.000000 starmoth-0.8.0/moth/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 14:53:46.433615 starmoth-0.8.0/moth/cli/
+-rw-rw-rw-   0 root         (0) root         (0)     1925 2024-04-23 20:53:43.000000 starmoth-0.8.0/moth/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 14:53:46.437616 starmoth-0.8.0/moth/driver/
+-rw-rw-rw-   0 root         (0) root         (0)     2121 2024-04-23 20:53:43.000000 starmoth-0.8.0/moth/driver/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 14:53:46.437616 starmoth-0.8.0/moth/message/
+-rw-rw-rw-   0 root         (0) root         (0)     9395 2024-04-29 12:15:07.000000 starmoth-0.8.0/moth/message/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      156 2024-04-23 20:53:43.000000 starmoth-0.8.0/moth/message/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 14:53:46.437616 starmoth-0.8.0/moth/server/
+-rw-rw-rw-   0 root         (0) root         (0)     5976 2024-04-23 20:53:43.000000 starmoth-0.8.0/moth/server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-16 14:53:46.441616 starmoth-0.8.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      853 2024-04-23 20:53:43.000000 starmoth-0.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 14:53:46.441616 starmoth-0.8.0/starmoth.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3921 2024-05-16 14:53:46.000000 starmoth-0.8.0/starmoth.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      350 2024-05-16 14:53:46.000000 starmoth-0.8.0/starmoth.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 14:53:46.000000 starmoth-0.8.0/starmoth.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-16 14:53:46.000000 starmoth-0.8.0/starmoth.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-05-16 14:53:46.000000 starmoth-0.8.0/starmoth.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-05-16 14:53:46.000000 starmoth-0.8.0/starmoth.egg-info/top_level.txt
```

### Comparing `starmoth-0.7.0/PKG-INFO` & `starmoth-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starmoth
-Version: 0.7.0
+Version: 0.8.0
 Summary: A small wrapper library to help test systems using STAR
 Author: Gudjon Magnusson
 Author-email: gmagnusson@fraunhofer.org
 Keywords: Fraunhofer,STAR,testing
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 Requires-Dist: pyzmq>=25.0.0
```

### Comparing `starmoth-0.7.0/README.md` & `starmoth-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `starmoth-0.7.0/moth/__init__.py` & `starmoth-0.8.0/moth/__init__.py`

 * *Files identical despite different names*

### Comparing `starmoth-0.7.0/moth/cli/__init__.py` & `starmoth-0.8.0/moth/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `starmoth-0.7.0/moth/driver/__init__.py` & `starmoth-0.8.0/moth/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `starmoth-0.7.0/moth/message/__init__.py` & `starmoth-0.8.0/moth/message/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
             self.id = str(uuid.uuid4())
         else:
             self.id = id
 
     def serialize(self):
         # Convert the image to bytes
         with io.BytesIO() as output:
-            self.image.save(output, format="JPEG")
+            self.image.save(output, format="PNG")
             img_bytes = output.getvalue()
 
         obj = {
             "id": self.id,
             "imageBytes": img_bytes,
         }
```

### Comparing `starmoth-0.7.0/moth/server/__init__.py` & `starmoth-0.8.0/moth/server/__init__.py`

 * *Files identical despite different names*

### Comparing `starmoth-0.7.0/setup.py` & `starmoth-0.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `starmoth-0.7.0/starmoth.egg-info/PKG-INFO` & `starmoth-0.8.0/starmoth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starmoth
-Version: 0.7.0
+Version: 0.8.0
 Summary: A small wrapper library to help test systems using STAR
 Author: Gudjon Magnusson
 Author-email: gmagnusson@fraunhofer.org
 Keywords: Fraunhofer,STAR,testing
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 Requires-Dist: pyzmq>=25.0.0
```

