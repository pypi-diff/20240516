# Comparing `tmp/socketsecurity-0.0.56.tar.gz` & `tmp/socketsecurity-0.0.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketsecurity-0.0.56.tar", last modified: Thu May 16 09:14:14 2024, max compression
+gzip compressed data, was "socketsecurity-0.0.57.tar", last modified: Thu May 16 09:20:28 2024, max compression
```

## Comparing `socketsecurity-0.0.56.tar` & `socketsecurity-0.0.57.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 09:14:14.142366 socketsecurity-0.0.56/
--rw-r--r--   0 douglascoburn   (501) staff       (20)      771 2024-05-16 09:14:14.142180 socketsecurity-0.0.56/PKG-INFO
--rw-r--r--   0 douglascoburn   (501) staff       (20)       21 2024-05-15 04:22:36.000000 socketsecurity-0.0.56/README.md
--rw-r--r--   0 douglascoburn   (501) staff       (20)     1025 2024-05-16 09:14:10.000000 socketsecurity-0.0.56/pyproject.toml
--rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-16 09:14:14.142405 socketsecurity-0.0.56/setup.cfg
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 09:14:14.131884 socketsecurity-0.0.56/socketsecurity/
--rw-r--r--   0 douglascoburn   (501) staff       (20)       49 2024-05-16 09:14:10.000000 socketsecurity-0.0.56/socketsecurity/__init__.py
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 09:14:14.141772 socketsecurity-0.0.56/socketsecurity/core/
--rw-r--r--   0 douglascoburn   (501) staff       (20)    26034 2024-05-16 09:14:10.000000 socketsecurity-0.0.56/socketsecurity/core/__init__.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)     9282 2024-05-16 08:29:16.000000 socketsecurity-0.0.56/socketsecurity/core/classes.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)      626 2024-04-29 13:52:20.000000 socketsecurity-0.0.56/socketsecurity/core/exceptions.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    11342 2024-05-16 07:53:25.000000 socketsecurity-0.0.56/socketsecurity/core/github.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    10906 2024-05-16 08:32:33.000000 socketsecurity-0.0.56/socketsecurity/core/glitlab.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    67547 2024-05-05 17:36:53.000000 socketsecurity-0.0.56/socketsecurity/core/issues.py
--rw-r--r--   0 douglascoburn   (501) staff       (20) 17442610 2024-05-06 19:45:31.000000 socketsecurity-0.0.56/socketsecurity/core/licenses.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    11849 2024-05-15 05:15:37.000000 socketsecurity-0.0.56/socketsecurity/core/messages.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)     5780 2024-05-16 09:12:39.000000 socketsecurity-0.0.56/socketsecurity/socketcli.py
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 09:14:14.141972 socketsecurity-0.0.56/socketsecurity.egg-info/
--rw-r--r--   0 douglascoburn   (501) staff       (20)      771 2024-05-16 09:14:14.000000 socketsecurity-0.0.56/socketsecurity.egg-info/PKG-INFO
--rw-r--r--   0 douglascoburn   (501) staff       (20)      561 2024-05-16 09:14:14.000000 socketsecurity-0.0.56/socketsecurity.egg-info/SOURCES.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)        1 2024-05-16 09:14:14.000000 socketsecurity-0.0.56/socketsecurity.egg-info/dependency_links.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)       59 2024-05-16 09:14:14.000000 socketsecurity-0.0.56/socketsecurity.egg-info/entry_points.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-16 09:14:14.000000 socketsecurity-0.0.56/socketsecurity.egg-info/requires.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)       15 2024-05-16 09:14:14.000000 socketsecurity-0.0.56/socketsecurity.egg-info/top_level.txt
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 09:20:28.587131 socketsecurity-0.0.57/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      771 2024-05-16 09:20:28.586958 socketsecurity-0.0.57/PKG-INFO
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       21 2024-05-15 04:22:36.000000 socketsecurity-0.0.57/README.md
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     1025 2024-05-16 09:18:18.000000 socketsecurity-0.0.57/pyproject.toml
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-16 09:20:28.587184 socketsecurity-0.0.57/setup.cfg
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 09:20:28.571095 socketsecurity-0.0.57/socketsecurity/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       49 2024-05-16 09:18:28.000000 socketsecurity-0.0.57/socketsecurity/__init__.py
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 09:20:28.581506 socketsecurity-0.0.57/socketsecurity/core/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    26034 2024-05-16 09:18:22.000000 socketsecurity-0.0.57/socketsecurity/core/__init__.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     9282 2024-05-16 08:29:16.000000 socketsecurity-0.0.57/socketsecurity/core/classes.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      626 2024-04-29 13:52:20.000000 socketsecurity-0.0.57/socketsecurity/core/exceptions.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    11342 2024-05-16 07:53:25.000000 socketsecurity-0.0.57/socketsecurity/core/github.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    10906 2024-05-16 08:32:33.000000 socketsecurity-0.0.57/socketsecurity/core/glitlab.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    67547 2024-05-05 17:36:53.000000 socketsecurity-0.0.57/socketsecurity/core/issues.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20) 17442610 2024-05-06 19:45:31.000000 socketsecurity-0.0.57/socketsecurity/core/licenses.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    11849 2024-05-15 05:15:37.000000 socketsecurity-0.0.57/socketsecurity/core/messages.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     5787 2024-05-16 09:18:13.000000 socketsecurity-0.0.57/socketsecurity/socketcli.py
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 09:20:28.586772 socketsecurity-0.0.57/socketsecurity.egg-info/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      771 2024-05-16 09:20:28.000000 socketsecurity-0.0.57/socketsecurity.egg-info/PKG-INFO
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      561 2024-05-16 09:20:28.000000 socketsecurity-0.0.57/socketsecurity.egg-info/SOURCES.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)        1 2024-05-16 09:20:28.000000 socketsecurity-0.0.57/socketsecurity.egg-info/dependency_links.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       59 2024-05-16 09:20:28.000000 socketsecurity-0.0.57/socketsecurity.egg-info/entry_points.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-16 09:20:28.000000 socketsecurity-0.0.57/socketsecurity.egg-info/requires.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       15 2024-05-16 09:20:28.000000 socketsecurity-0.0.57/socketsecurity.egg-info/top_level.txt
```

### Comparing `socketsecurity-0.0.56/PKG-INFO` & `socketsecurity-0.0.57/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketsecurity
-Version: 0.0.56
+Version: 0.0.57
 Summary: Socket Security CLI for CI/CD
 Author-email: Douglas Coburn <douglas@socket.dev>
 Maintainer-email: Douglas Coburn <douglas@socket.dev>
 Project-URL: Homepage, https://socket.dev
 Keywords: socketsecurity,socket.dev,sca,oss,security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `socketsecurity-0.0.56/pyproject.toml` & `socketsecurity-0.0.57/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "socketsecurity"
-version = "0.0.56"
+version = "0.0.57"
 requires-python = ">= 3.9"
 dependencies = [
     'requests',
     'mdutils',
     'prettytable',
     'argparse'
 ]
```

### Comparing `socketsecurity-0.0.56/socketsecurity/core/__init__.py` & `socketsecurity-0.0.57/socketsecurity/core/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 )
 import platform
 from glob import glob
 import time
 
 
 __author__ = 'socket.dev'
-__version__ = '0.0.56'
+__version__ = '0.0.57'
 __all__ = [
     "Core",
     "log",
     "__version__"
 ]
```

### Comparing `socketsecurity-0.0.56/socketsecurity/core/classes.py` & `socketsecurity-0.0.57/socketsecurity/core/classes.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.56/socketsecurity/core/exceptions.py` & `socketsecurity-0.0.57/socketsecurity/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.56/socketsecurity/core/github.py` & `socketsecurity-0.0.57/socketsecurity/core/github.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.56/socketsecurity/core/glitlab.py` & `socketsecurity-0.0.57/socketsecurity/core/glitlab.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.56/socketsecurity/core/issues.py` & `socketsecurity-0.0.57/socketsecurity/core/issues.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.56/socketsecurity/core/licenses.py` & `socketsecurity-0.0.57/socketsecurity/core/licenses.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.56/socketsecurity/core/messages.py` & `socketsecurity-0.0.57/socketsecurity/core/messages.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.56/socketsecurity/socketcli.py` & `socketsecurity-0.0.57/socketsecurity/socketcli.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     required=False
 )
 
 parser.add_argument(
     '-v',
     '--version',
     action="version",
-    version=f'%(prog)s 0.0.55',
+    version=f'%(prog)s {__version__}',
     help='Display the version',
 )
 
 
 def output_console_comments(diff_report) -> None:
     console_security_comment = Messages.create_console_security_alert_table(diff_report)
     if len(diff_report.new_alerts) > 0:
```

### Comparing `socketsecurity-0.0.56/socketsecurity.egg-info/PKG-INFO` & `socketsecurity-0.0.57/socketsecurity.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketsecurity
-Version: 0.0.56
+Version: 0.0.57
 Summary: Socket Security CLI for CI/CD
 Author-email: Douglas Coburn <douglas@socket.dev>
 Maintainer-email: Douglas Coburn <douglas@socket.dev>
 Project-URL: Homepage, https://socket.dev
 Keywords: socketsecurity,socket.dev,sca,oss,security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `socketsecurity-0.0.56/socketsecurity.egg-info/SOURCES.txt` & `socketsecurity-0.0.57/socketsecurity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

