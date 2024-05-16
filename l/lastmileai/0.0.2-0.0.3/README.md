# Comparing `tmp/lastmileai-0.0.2.tar.gz` & `tmp/lastmileai-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lastmileai-0.0.2.tar", last modified: Fri Oct 13 16:11:43 2023, max compression
+gzip compressed data, was "lastmileai-0.0.3.tar", last modified: Thu May 16 18:56:53 2024, max compression
```

## Comparing `lastmileai-0.0.2.tar` & `lastmileai-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 suyogsonwalkar   (501) staff       (20)        0 2023-10-13 16:11:43.491016 lastmileai-0.0.2/
--rw-r--r--   0 suyogsonwalkar   (501) staff       (20)     1074 2023-08-16 15:15:55.000000 lastmileai-0.0.2/LICENSE
--rw-r--r--   0 suyogsonwalkar   (501) staff       (20)     2440 2023-10-13 16:11:43.490865 lastmileai-0.0.2/PKG-INFO
--rw-r--r--   0 suyogsonwalkar   (501) staff       (20)     1928 2023-10-13 15:54:44.000000 lastmileai-0.0.2/README.md
--rw-r--r--   0 suyogsonwalkar   (501) staff       (20)      597 2023-10-13 15:40:34.000000 lastmileai-0.0.2/pyproject.toml
--rw-r--r--   0 suyogsonwalkar   (501) staff       (20)       38 2023-10-13 16:11:43.491043 lastmileai-0.0.2/setup.cfg
-drwxr-xr-x   0 suyogsonwalkar   (501) staff       (20)        0 2023-10-13 16:11:43.489570 lastmileai-0.0.2/src/
-drwxr-xr-x   0 suyogsonwalkar   (501) staff       (20)        0 2023-10-13 16:11:43.490009 lastmileai-0.0.2/src/lastmileai/
--rw-r--r--   0 suyogsonwalkar   (501) staff       (20)    10883 2023-10-13 15:51:22.000000 lastmileai-0.0.2/src/lastmileai/__init__.py
-drwxr-xr-x   0 suyogsonwalkar   (501) staff       (20)        0 2023-10-13 16:11:43.490557 lastmileai-0.0.2/src/lastmileai.egg-info/
--rw-r--r--   0 suyogsonwalkar   (501) staff       (20)     2440 2023-10-13 16:11:43.000000 lastmileai-0.0.2/src/lastmileai.egg-info/PKG-INFO
--rw-r--r--   0 suyogsonwalkar   (501) staff       (20)      265 2023-10-13 16:11:43.000000 lastmileai-0.0.2/src/lastmileai.egg-info/SOURCES.txt
--rw-r--r--   0 suyogsonwalkar   (501) staff       (20)        1 2023-10-13 16:11:43.000000 lastmileai-0.0.2/src/lastmileai.egg-info/dependency_links.txt
--rw-r--r--   0 suyogsonwalkar   (501) staff       (20)       17 2023-10-13 16:11:43.000000 lastmileai-0.0.2/src/lastmileai.egg-info/requires.txt
--rw-r--r--   0 suyogsonwalkar   (501) staff       (20)       11 2023-10-13 16:11:43.000000 lastmileai-0.0.2/src/lastmileai.egg-info/top_level.txt
-drwxr-xr-x   0 suyogsonwalkar   (501) staff       (20)        0 2023-10-13 16:11:43.490674 lastmileai-0.0.2/test/
--rw-r--r--   0 suyogsonwalkar   (501) staff       (20)     1084 2023-08-16 15:15:55.000000 lastmileai-0.0.2/test/test_api.py
+drwxr-xr-x   0 ankush     (501) staff       (20)        0 2024-05-16 18:56:53.158526 lastmileai-0.0.3/
+-rw-r--r--   0 ankush     (501) staff       (20)     1074 2024-05-16 18:52:55.000000 lastmileai-0.0.3/LICENSE
+-rw-r--r--   0 ankush     (501) staff       (20)     2440 2024-05-16 18:56:53.158255 lastmileai-0.0.3/PKG-INFO
+-rw-r--r--   0 ankush     (501) staff       (20)     1928 2024-05-16 18:52:55.000000 lastmileai-0.0.3/README.md
+-rw-r--r--   0 ankush     (501) staff       (20)      597 2024-05-16 18:53:54.000000 lastmileai-0.0.3/pyproject.toml
+-rw-r--r--   0 ankush     (501) staff       (20)       38 2024-05-16 18:56:53.158577 lastmileai-0.0.3/setup.cfg
+drwxr-xr-x   0 ankush     (501) staff       (20)        0 2024-05-16 18:56:53.156339 lastmileai-0.0.3/src/
+drwxr-xr-x   0 ankush     (501) staff       (20)        0 2024-05-16 18:56:53.156910 lastmileai-0.0.3/src/lastmileai/
+-rw-r--r--   0 ankush     (501) staff       (20)    10883 2024-05-16 18:52:55.000000 lastmileai-0.0.3/src/lastmileai/__init__.py
+drwxr-xr-x   0 ankush     (501) staff       (20)        0 2024-05-16 18:56:53.157958 lastmileai-0.0.3/src/lastmileai.egg-info/
+-rw-r--r--   0 ankush     (501) staff       (20)     2440 2024-05-16 18:56:53.000000 lastmileai-0.0.3/src/lastmileai.egg-info/PKG-INFO
+-rw-r--r--   0 ankush     (501) staff       (20)      265 2024-05-16 18:56:53.000000 lastmileai-0.0.3/src/lastmileai.egg-info/SOURCES.txt
+-rw-r--r--   0 ankush     (501) staff       (20)        1 2024-05-16 18:56:53.000000 lastmileai-0.0.3/src/lastmileai.egg-info/dependency_links.txt
+-rw-r--r--   0 ankush     (501) staff       (20)       17 2024-05-16 18:56:53.000000 lastmileai-0.0.3/src/lastmileai.egg-info/requires.txt
+-rw-r--r--   0 ankush     (501) staff       (20)       11 2024-05-16 18:56:53.000000 lastmileai-0.0.3/src/lastmileai.egg-info/top_level.txt
+drwxr-xr-x   0 ankush     (501) staff       (20)        0 2024-05-16 18:56:53.157745 lastmileai-0.0.3/test/
+-rw-r--r--   0 ankush     (501) staff       (20)     1084 2024-05-16 18:52:55.000000 lastmileai-0.0.3/test/test_api.py
```

### Comparing `lastmileai-0.0.2/LICENSE` & `lastmileai-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lastmileai-0.0.2/PKG-INFO` & `lastmileai-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lastmileai
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python library for LastMile AI API
 Author-email: Suyog Sonwalkar <flux159@gmail.com>
 Project-URL: Homepage, https://github.com/lastmile-ai/lastmileai-python
 Project-URL: Bug Tracker, https://github.com/lastmile-ai/lastmileai-python/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `lastmileai-0.0.2/README.md` & `lastmileai-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `lastmileai-0.0.2/pyproject.toml` & `lastmileai-0.0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lastmileai"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Suyog Sonwalkar", email="flux159@gmail.com" },
 ]
 description = "Python library for LastMile AI API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `lastmileai-0.0.2/src/lastmileai/__init__.py` & `lastmileai-0.0.3/src/lastmileai/__init__.py`

 * *Files identical despite different names*

### Comparing `lastmileai-0.0.2/src/lastmileai.egg-info/PKG-INFO` & `lastmileai-0.0.3/src/lastmileai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lastmileai
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python library for LastMile AI API
 Author-email: Suyog Sonwalkar <flux159@gmail.com>
 Project-URL: Homepage, https://github.com/lastmile-ai/lastmileai-python
 Project-URL: Bug Tracker, https://github.com/lastmile-ai/lastmileai-python/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `lastmileai-0.0.2/test/test_api.py` & `lastmileai-0.0.3/test/test_api.py`

 * *Files identical despite different names*

