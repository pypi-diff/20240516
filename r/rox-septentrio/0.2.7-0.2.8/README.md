# Comparing `tmp/rox_septentrio-0.2.7.tar.gz` & `tmp/rox_septentrio-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rox_septentrio-0.2.7.tar", last modified: Thu May 16 10:52:08 2024, max compression
+gzip compressed data, was "rox_septentrio-0.2.8.tar", last modified: Thu May 16 14:14:29 2024, max compression
```

## Comparing `rox_septentrio-0.2.7.tar` & `rox_septentrio-0.2.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:52:08.899072 rox_septentrio-0.2.7/
--rw-rw-rw-   0 root         (0) root         (0)     1106 2024-05-16 10:51:45.000000 rox_septentrio-0.2.7/LICENCE
--rw-r--r--   0 root         (0) root         (0)     2994 2024-05-16 10:52:08.899072 rox_septentrio-0.2.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2089 2024-05-16 10:51:45.000000 rox_septentrio-0.2.7/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1685 2024-05-16 10:51:45.000000 rox_septentrio-0.2.7/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-16 10:52:08.899072 rox_septentrio-0.2.7/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:52:08.894072 rox_septentrio-0.2.7/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:52:08.897072 rox_septentrio-0.2.7/src/rox_septentrio/
--rw-rw-rw-   0 root         (0) root         (0)       46 2024-05-16 10:51:45.000000 rox_septentrio-0.2.7/src/rox_septentrio/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      291 2024-05-16 10:51:45.000000 rox_septentrio-0.2.7/src/rox_septentrio/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)      598 2024-05-16 10:51:45.000000 rox_septentrio-0.2.7/src/rox_septentrio/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1745 2024-05-16 10:51:45.000000 rox_septentrio-0.2.7/src/rox_septentrio/converters.py
--rw-rw-rw-   0 root         (0) root         (0)     2211 2024-05-16 10:51:45.000000 rox_septentrio-0.2.7/src/rox_septentrio/gps_node.py
--rw-rw-rw-   0 root         (0) root         (0)     2486 2024-05-16 10:51:45.000000 rox_septentrio-0.2.7/src/rox_septentrio/nmea.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 10:51:45.000000 rox_septentrio-0.2.7/src/rox_septentrio/py.typed
--rw-rw-rw-   0 root         (0) root         (0)      241 2024-05-16 10:51:45.000000 rox_septentrio-0.2.7/src/rox_septentrio/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:52:08.898072 rox_septentrio-0.2.7/src/rox_septentrio.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2994 2024-05-16 10:52:08.000000 rox_septentrio-0.2.7/src/rox_septentrio.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      546 2024-05-16 10:52:08.000000 rox_septentrio-0.2.7/src/rox_septentrio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 10:52:08.000000 rox_septentrio-0.2.7/src/rox_septentrio.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-05-16 10:52:08.000000 rox_septentrio-0.2.7/src/rox_septentrio.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       87 2024-05-16 10:52:08.000000 rox_septentrio-0.2.7/src/rox_septentrio.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-05-16 10:52:08.000000 rox_septentrio-0.2.7/src/rox_septentrio.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:52:08.898072 rox_septentrio-0.2.7/tests/
--rw-rw-rw-   0 root         (0) root         (0)      111 2024-05-16 10:51:45.000000 rox_septentrio-0.2.7/tests/test_smoke.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 14:14:29.905375 rox_septentrio-0.2.8/
+-rw-rw-rw-   0 root         (0) root         (0)     1106 2024-05-16 14:14:06.000000 rox_septentrio-0.2.8/LICENCE
+-rw-r--r--   0 root         (0) root         (0)     2994 2024-05-16 14:14:29.905375 rox_septentrio-0.2.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2089 2024-05-16 14:14:06.000000 rox_septentrio-0.2.8/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1679 2024-05-16 14:14:06.000000 rox_septentrio-0.2.8/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-16 14:14:29.905375 rox_septentrio-0.2.8/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 14:14:29.900375 rox_septentrio-0.2.8/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 14:14:29.903375 rox_septentrio-0.2.8/src/rox_septentrio/
+-rw-rw-rw-   0 root         (0) root         (0)       46 2024-05-16 14:14:06.000000 rox_septentrio-0.2.8/src/rox_septentrio/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      291 2024-05-16 14:14:06.000000 rox_septentrio-0.2.8/src/rox_septentrio/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      598 2024-05-16 14:14:06.000000 rox_septentrio-0.2.8/src/rox_septentrio/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1745 2024-05-16 14:14:06.000000 rox_septentrio-0.2.8/src/rox_septentrio/converters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2211 2024-05-16 14:14:06.000000 rox_septentrio-0.2.8/src/rox_septentrio/gps_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     2486 2024-05-16 14:14:06.000000 rox_septentrio-0.2.8/src/rox_septentrio/nmea.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 14:14:06.000000 rox_septentrio-0.2.8/src/rox_septentrio/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)      241 2024-05-16 14:14:06.000000 rox_septentrio-0.2.8/src/rox_septentrio/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 14:14:29.904375 rox_septentrio-0.2.8/src/rox_septentrio.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2994 2024-05-16 14:14:29.000000 rox_septentrio-0.2.8/src/rox_septentrio.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      546 2024-05-16 14:14:29.000000 rox_septentrio-0.2.8/src/rox_septentrio.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 14:14:29.000000 rox_septentrio-0.2.8/src/rox_septentrio.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2024-05-16 14:14:29.000000 rox_septentrio-0.2.8/src/rox_septentrio.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       87 2024-05-16 14:14:29.000000 rox_septentrio-0.2.8/src/rox_septentrio.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-16 14:14:29.000000 rox_septentrio-0.2.8/src/rox_septentrio.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 14:14:29.904375 rox_septentrio-0.2.8/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      111 2024-05-16 14:14:06.000000 rox_septentrio-0.2.8/tests/test_smoke.py
```

### Comparing `rox_septentrio-0.2.7/LICENCE` & `rox_septentrio-0.2.8/LICENCE`

 * *Files identical despite different names*

### Comparing `rox_septentrio-0.2.7/PKG-INFO` & `rox_septentrio-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rox-septentrio
-Version: 0.2.7
+Version: 0.2.8
 Summary: Driver for Septentrio GPS, posting messages to mqtt
 Author-email: Jev Kuznetsov <jev@roxautomation.com>
 License: MIT
 Project-URL: Homepage, https://gitlab.com/roxautomation/components/septentrio-gps
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `rox_septentrio-0.2.7/README.md` & `rox_septentrio-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `rox_septentrio-0.2.7/pyproject.toml` & `rox_septentrio-0.2.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #-----------------pyproject.toml configuration----------------
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rox-septentrio"
-version = "0.2.7"
+version = "0.2.8"
 description = "Driver for Septentrio GPS, posting messages to mqtt"
 authors = [
     {name = "Jev Kuznetsov", email = "jev@roxautomation.com"},
 ]
 license = {text = "MIT"}
 readme = "README.md"
 classifiers = [
@@ -34,15 +34,15 @@
 ]
 requires-python = ">=3.10"
 
 [project.urls]
 Homepage = "https://gitlab.com/roxautomation/components/septentrio-gps"
 
 [project.scripts]
-septentrio_gps = "septentrio_gps.__main__:main"
+gps_node = "rox_septentrio.__main__:main"
 
 # optiona depnedencies are defined in requirements_dev.txt
 
 #--------------mypy configuration----------------
 [tool.mypy]
 # Global options can be specified here
 disallow_untyped_defs = true
```

### Comparing `rox_septentrio-0.2.7/src/rox_septentrio/config.py` & `rox_septentrio-0.2.8/src/rox_septentrio/config.py`

 * *Files identical despite different names*

### Comparing `rox_septentrio-0.2.7/src/rox_septentrio/converters.py` & `rox_septentrio-0.2.8/src/rox_septentrio/converters.py`

 * *Files identical despite different names*

### Comparing `rox_septentrio-0.2.7/src/rox_septentrio/gps_node.py` & `rox_septentrio-0.2.8/src/rox_septentrio/gps_node.py`

 * *Files identical despite different names*

### Comparing `rox_septentrio-0.2.7/src/rox_septentrio/nmea.py` & `rox_septentrio-0.2.8/src/rox_septentrio/nmea.py`

 * *Files identical despite different names*

### Comparing `rox_septentrio-0.2.7/src/rox_septentrio.egg-info/PKG-INFO` & `rox_septentrio-0.2.8/src/rox_septentrio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rox-septentrio
-Version: 0.2.7
+Version: 0.2.8
 Summary: Driver for Septentrio GPS, posting messages to mqtt
 Author-email: Jev Kuznetsov <jev@roxautomation.com>
 License: MIT
 Project-URL: Homepage, https://gitlab.com/roxautomation/components/septentrio-gps
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `rox_septentrio-0.2.7/src/rox_septentrio.egg-info/SOURCES.txt` & `rox_septentrio-0.2.8/src/rox_septentrio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

