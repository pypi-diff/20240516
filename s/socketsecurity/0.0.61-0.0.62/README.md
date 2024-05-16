# Comparing `tmp/socketsecurity-0.0.61.tar.gz` & `tmp/socketsecurity-0.0.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketsecurity-0.0.61.tar", last modified: Thu May 16 10:20:06 2024, max compression
+gzip compressed data, was "socketsecurity-0.0.62.tar", last modified: Thu May 16 10:26:20 2024, max compression
```

## Comparing `socketsecurity-0.0.61.tar` & `socketsecurity-0.0.62.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 10:20:06.134788 socketsecurity-0.0.61/
--rw-r--r--   0 douglascoburn   (501) staff       (20)      771 2024-05-16 10:20:06.134618 socketsecurity-0.0.61/PKG-INFO
--rw-r--r--   0 douglascoburn   (501) staff       (20)       21 2024-05-15 04:22:36.000000 socketsecurity-0.0.61/README.md
--rw-r--r--   0 douglascoburn   (501) staff       (20)     1025 2024-05-16 10:20:01.000000 socketsecurity-0.0.61/pyproject.toml
--rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-16 10:20:06.134825 socketsecurity-0.0.61/setup.cfg
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 10:20:06.121586 socketsecurity-0.0.61/socketsecurity/
--rw-r--r--   0 douglascoburn   (501) staff       (20)       98 2024-05-16 10:04:37.000000 socketsecurity-0.0.61/socketsecurity/__init__.py
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 10:20:06.132870 socketsecurity-0.0.61/socketsecurity/core/
--rw-r--r--   0 douglascoburn   (501) staff       (20)    26034 2024-05-16 10:19:58.000000 socketsecurity-0.0.61/socketsecurity/core/__init__.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)     9282 2024-05-16 08:29:16.000000 socketsecurity-0.0.61/socketsecurity/core/classes.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)      626 2024-04-29 13:52:20.000000 socketsecurity-0.0.61/socketsecurity/core/exceptions.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    11342 2024-05-16 07:53:25.000000 socketsecurity-0.0.61/socketsecurity/core/github.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    11021 2024-05-16 10:19:43.000000 socketsecurity-0.0.61/socketsecurity/core/gitlab.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    68147 2024-05-16 10:03:15.000000 socketsecurity-0.0.61/socketsecurity/core/issues.py
--rw-r--r--   0 douglascoburn   (501) staff       (20) 17442610 2024-05-06 19:45:31.000000 socketsecurity-0.0.61/socketsecurity/core/licenses.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    11849 2024-05-15 05:15:37.000000 socketsecurity-0.0.61/socketsecurity/core/messages.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)     5975 2024-05-16 10:18:06.000000 socketsecurity-0.0.61/socketsecurity/socketcli.py
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 10:20:06.134427 socketsecurity-0.0.61/socketsecurity.egg-info/
--rw-r--r--   0 douglascoburn   (501) staff       (20)      771 2024-05-16 10:20:06.000000 socketsecurity-0.0.61/socketsecurity.egg-info/PKG-INFO
--rw-r--r--   0 douglascoburn   (501) staff       (20)      560 2024-05-16 10:20:06.000000 socketsecurity-0.0.61/socketsecurity.egg-info/SOURCES.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)        1 2024-05-16 10:20:06.000000 socketsecurity-0.0.61/socketsecurity.egg-info/dependency_links.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)       59 2024-05-16 10:20:06.000000 socketsecurity-0.0.61/socketsecurity.egg-info/entry_points.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-16 10:20:06.000000 socketsecurity-0.0.61/socketsecurity.egg-info/requires.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)       15 2024-05-16 10:20:06.000000 socketsecurity-0.0.61/socketsecurity.egg-info/top_level.txt
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 10:26:20.298168 socketsecurity-0.0.62/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      771 2024-05-16 10:26:20.297960 socketsecurity-0.0.62/PKG-INFO
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       21 2024-05-15 04:22:36.000000 socketsecurity-0.0.62/README.md
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     1025 2024-05-16 10:26:04.000000 socketsecurity-0.0.62/pyproject.toml
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-16 10:26:20.298211 socketsecurity-0.0.62/setup.cfg
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 10:26:20.279313 socketsecurity-0.0.62/socketsecurity/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       98 2024-05-16 10:04:37.000000 socketsecurity-0.0.62/socketsecurity/__init__.py
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 10:26:20.289067 socketsecurity-0.0.62/socketsecurity/core/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    26034 2024-05-16 10:26:06.000000 socketsecurity-0.0.62/socketsecurity/core/__init__.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     9282 2024-05-16 08:29:16.000000 socketsecurity-0.0.62/socketsecurity/core/classes.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      626 2024-04-29 13:52:20.000000 socketsecurity-0.0.62/socketsecurity/core/exceptions.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    11342 2024-05-16 07:53:25.000000 socketsecurity-0.0.62/socketsecurity/core/github.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    11021 2024-05-16 10:19:43.000000 socketsecurity-0.0.62/socketsecurity/core/gitlab.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    68147 2024-05-16 10:03:15.000000 socketsecurity-0.0.62/socketsecurity/core/issues.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20) 17442610 2024-05-06 19:45:31.000000 socketsecurity-0.0.62/socketsecurity/core/licenses.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    11849 2024-05-15 05:15:37.000000 socketsecurity-0.0.62/socketsecurity/core/messages.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     5975 2024-05-16 10:18:06.000000 socketsecurity-0.0.62/socketsecurity/socketcli.py
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 10:26:20.297706 socketsecurity-0.0.62/socketsecurity.egg-info/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      771 2024-05-16 10:26:20.000000 socketsecurity-0.0.62/socketsecurity.egg-info/PKG-INFO
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      560 2024-05-16 10:26:20.000000 socketsecurity-0.0.62/socketsecurity.egg-info/SOURCES.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)        1 2024-05-16 10:26:20.000000 socketsecurity-0.0.62/socketsecurity.egg-info/dependency_links.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       59 2024-05-16 10:26:20.000000 socketsecurity-0.0.62/socketsecurity.egg-info/entry_points.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-16 10:26:20.000000 socketsecurity-0.0.62/socketsecurity.egg-info/requires.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       15 2024-05-16 10:26:20.000000 socketsecurity-0.0.62/socketsecurity.egg-info/top_level.txt
```

### Comparing `socketsecurity-0.0.61/PKG-INFO` & `socketsecurity-0.0.62/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketsecurity
-Version: 0.0.61
+Version: 0.0.62
 Summary: Socket Security CLI for CI/CD
 Author-email: Douglas Coburn <douglas@socket.dev>
 Maintainer-email: Douglas Coburn <douglas@socket.dev>
 Project-URL: Homepage, https://socket.dev
 Keywords: socketsecurity,socket.dev,sca,oss,security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `socketsecurity-0.0.61/pyproject.toml` & `socketsecurity-0.0.62/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "socketsecurity"
-version = "0.0.61"
+version = "0.0.62"
 requires-python = ">= 3.9"
 dependencies = [
     'requests',
     'mdutils',
     'prettytable',
     'argparse'
 ]
```

### Comparing `socketsecurity-0.0.61/socketsecurity/core/__init__.py` & `socketsecurity-0.0.62/socketsecurity/core/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 )
 import platform
 from glob import glob
 import time
 
 
 __author__ = 'socket.dev'
-__version__ = '0.0.61'
+__version__ = '0.0.62'
 __all__ = [
     "Core",
     "log",
     "__version__"
 ]
```

### Comparing `socketsecurity-0.0.61/socketsecurity/core/classes.py` & `socketsecurity-0.0.62/socketsecurity/core/classes.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.61/socketsecurity/core/exceptions.py` & `socketsecurity-0.0.62/socketsecurity/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.61/socketsecurity/core/github.py` & `socketsecurity-0.0.62/socketsecurity/core/github.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.61/socketsecurity/core/gitlab.py` & `socketsecurity-0.0.62/socketsecurity/core/gitlab.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.61/socketsecurity/core/issues.py` & `socketsecurity-0.0.62/socketsecurity/core/issues.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.61/socketsecurity/core/licenses.py` & `socketsecurity-0.0.62/socketsecurity/core/licenses.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.61/socketsecurity/core/messages.py` & `socketsecurity-0.0.62/socketsecurity/core/messages.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.61/socketsecurity/socketcli.py` & `socketsecurity-0.0.62/socketsecurity/socketcli.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.61/socketsecurity.egg-info/PKG-INFO` & `socketsecurity-0.0.62/socketsecurity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketsecurity
-Version: 0.0.61
+Version: 0.0.62
 Summary: Socket Security CLI for CI/CD
 Author-email: Douglas Coburn <douglas@socket.dev>
 Maintainer-email: Douglas Coburn <douglas@socket.dev>
 Project-URL: Homepage, https://socket.dev
 Keywords: socketsecurity,socket.dev,sca,oss,security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `socketsecurity-0.0.61/socketsecurity.egg-info/SOURCES.txt` & `socketsecurity-0.0.62/socketsecurity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

