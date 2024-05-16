# Comparing `tmp/inferent-0.0.8.tar.gz` & `tmp/inferent-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inferent-0.0.8.tar", last modified: Sat Mar  2 13:55:13 2024, max compression
+gzip compressed data, was "inferent-0.0.9.tar", last modified: Sat Mar  2 13:58:48 2024, max compression
```

## Comparing `inferent-0.0.8.tar` & `inferent-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 olives     (501) staff       (20)        0 2024-03-02 13:55:13.803070 inferent-0.0.8/
--rw-r--r--   0 olives     (501) staff       (20)     1065 2024-01-02 14:59:37.000000 inferent-0.0.8/LICENSE
--rw-r--r--   0 olives     (501) staff       (20)      675 2024-03-02 13:55:13.802744 inferent-0.0.8/PKG-INFO
--rw-r--r--   0 olives     (501) staff       (20)       65 2024-01-04 12:11:54.000000 inferent-0.0.8/README.md
--rw-r--r--   0 olives     (501) staff       (20)      651 2024-03-02 13:55:09.000000 inferent-0.0.8/pyproject.toml
--rw-r--r--   0 olives     (501) staff       (20)       38 2024-03-02 13:55:13.803132 inferent-0.0.8/setup.cfg
-drwxr-xr-x   0 olives     (501) staff       (20)        0 2024-03-02 13:55:13.798685 inferent-0.0.8/src/
--rw-r--r--   0 olives     (501) staff       (20)        1 2024-01-02 14:59:37.000000 inferent-0.0.8/src/__init__.py
-drwxr-xr-x   0 olives     (501) staff       (20)        0 2024-03-02 13:55:13.800163 inferent-0.0.8/src/inferent/
--rw-r--r--   0 olives     (501) staff       (20)       38 2024-02-17 03:11:59.000000 inferent-0.0.8/src/inferent/__init__.py
--rw-r--r--   0 olives     (501) staff       (20)     3188 2024-01-04 12:18:25.000000 inferent-0.0.8/src/inferent/base_scraper.py
--rw-r--r--   0 olives     (501) staff       (20)    14601 2024-02-23 05:01:24.000000 inferent-0.0.8/src/inferent/training.py
--rw-r--r--   0 olives     (501) staff       (20)     1977 2024-03-02 13:54:51.000000 inferent-0.0.8/src/inferent/utils.py
-drwxr-xr-x   0 olives     (501) staff       (20)        0 2024-03-02 13:55:13.802423 inferent-0.0.8/src/inferent.egg-info/
--rw-r--r--   0 olives     (501) staff       (20)      675 2024-03-02 13:55:13.000000 inferent-0.0.8/src/inferent.egg-info/PKG-INFO
--rw-r--r--   0 olives     (501) staff       (20)      401 2024-03-02 13:55:13.000000 inferent-0.0.8/src/inferent.egg-info/SOURCES.txt
--rw-r--r--   0 olives     (501) staff       (20)        1 2024-03-02 13:55:13.000000 inferent-0.0.8/src/inferent.egg-info/dependency_links.txt
--rw-r--r--   0 olives     (501) staff       (20)       48 2024-03-02 13:55:13.000000 inferent-0.0.8/src/inferent.egg-info/requires.txt
--rw-r--r--   0 olives     (501) staff       (20)       24 2024-03-02 13:55:13.000000 inferent-0.0.8/src/inferent.egg-info/top_level.txt
-drwxr-xr-x   0 olives     (501) staff       (20)        0 2024-03-02 13:55:13.802001 inferent-0.0.8/src/tests/
--rw-r--r--   0 olives     (501) staff       (20)        0 2024-02-17 01:09:51.000000 inferent-0.0.8/src/tests/__init__.py
--rw-r--r--   0 olives     (501) staff       (20)      646 2024-02-20 04:16:50.000000 inferent-0.0.8/src/tests/test_training.py
--rw-r--r--   0 olives     (501) staff       (20)      612 2024-02-17 01:04:25.000000 inferent-0.0.8/src/tests/test_utils.py
+drwxr-xr-x   0 olives     (501) staff       (20)        0 2024-03-02 13:58:48.260329 inferent-0.0.9/
+-rw-r--r--   0 olives     (501) staff       (20)     1065 2024-01-02 14:59:37.000000 inferent-0.0.9/LICENSE
+-rw-r--r--   0 olives     (501) staff       (20)      675 2024-03-02 13:58:48.260047 inferent-0.0.9/PKG-INFO
+-rw-r--r--   0 olives     (501) staff       (20)       65 2024-01-04 12:11:54.000000 inferent-0.0.9/README.md
+-rw-r--r--   0 olives     (501) staff       (20)      651 2024-03-02 13:58:42.000000 inferent-0.0.9/pyproject.toml
+-rw-r--r--   0 olives     (501) staff       (20)       38 2024-03-02 13:58:48.260383 inferent-0.0.9/setup.cfg
+drwxr-xr-x   0 olives     (501) staff       (20)        0 2024-03-02 13:58:48.256031 inferent-0.0.9/src/
+-rw-r--r--   0 olives     (501) staff       (20)        1 2024-01-02 14:59:37.000000 inferent-0.0.9/src/__init__.py
+drwxr-xr-x   0 olives     (501) staff       (20)        0 2024-03-02 13:58:48.257580 inferent-0.0.9/src/inferent/
+-rw-r--r--   0 olives     (501) staff       (20)       38 2024-02-17 03:11:59.000000 inferent-0.0.9/src/inferent/__init__.py
+-rw-r--r--   0 olives     (501) staff       (20)     3188 2024-01-04 12:18:25.000000 inferent-0.0.9/src/inferent/base_scraper.py
+-rw-r--r--   0 olives     (501) staff       (20)    14601 2024-02-23 05:01:24.000000 inferent-0.0.9/src/inferent/training.py
+-rw-r--r--   0 olives     (501) staff       (20)     1967 2024-03-02 13:58:33.000000 inferent-0.0.9/src/inferent/utils.py
+drwxr-xr-x   0 olives     (501) staff       (20)        0 2024-03-02 13:58:48.259755 inferent-0.0.9/src/inferent.egg-info/
+-rw-r--r--   0 olives     (501) staff       (20)      675 2024-03-02 13:58:48.000000 inferent-0.0.9/src/inferent.egg-info/PKG-INFO
+-rw-r--r--   0 olives     (501) staff       (20)      401 2024-03-02 13:58:48.000000 inferent-0.0.9/src/inferent.egg-info/SOURCES.txt
+-rw-r--r--   0 olives     (501) staff       (20)        1 2024-03-02 13:58:48.000000 inferent-0.0.9/src/inferent.egg-info/dependency_links.txt
+-rw-r--r--   0 olives     (501) staff       (20)       48 2024-03-02 13:58:48.000000 inferent-0.0.9/src/inferent.egg-info/requires.txt
+-rw-r--r--   0 olives     (501) staff       (20)       24 2024-03-02 13:58:48.000000 inferent-0.0.9/src/inferent.egg-info/top_level.txt
+drwxr-xr-x   0 olives     (501) staff       (20)        0 2024-03-02 13:58:48.259370 inferent-0.0.9/src/tests/
+-rw-r--r--   0 olives     (501) staff       (20)        0 2024-02-17 01:09:51.000000 inferent-0.0.9/src/tests/__init__.py
+-rw-r--r--   0 olives     (501) staff       (20)      646 2024-02-20 04:16:50.000000 inferent-0.0.9/src/tests/test_training.py
+-rw-r--r--   0 olives     (501) staff       (20)      612 2024-02-17 01:04:25.000000 inferent-0.0.9/src/tests/test_utils.py
```

### Comparing `inferent-0.0.8/LICENSE` & `inferent-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `inferent-0.0.8/PKG-INFO` & `inferent-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inferent
-Version: 0.0.8
+Version: 0.0.9
 Summary: Inferent Ventures
 Author-email: Inferent Ventures <inferentventures@gmail.com>
 Project-URL: Homepage, https://github.com/inferent
 Project-URL: Issues, https://github.com/inferent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `inferent-0.0.8/pyproject.toml` & `inferent-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "inferent"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Inferent Ventures", email="inferentventures@gmail.com" },
 ]
 description = "Inferent Ventures"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `inferent-0.0.8/src/inferent/base_scraper.py` & `inferent-0.0.9/src/inferent/base_scraper.py`

 * *Files identical despite different names*

### Comparing `inferent-0.0.8/src/inferent/training.py` & `inferent-0.0.9/src/inferent/training.py`

 * *Files identical despite different names*

### Comparing `inferent-0.0.8/src/inferent/utils.py` & `inferent-0.0.9/src/inferent/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
     flat_circular:
     ==============
     Inverse of steep circular for the two sides.
 
     """
     if curve == "spline":
-        return functools.partial(interpolate.splev, tck=interpolate.splrep(x, y, k=2))
+        return partial(interpolate.splev, tck=interpolate.splrep(x, y, k=2))
     elif curve == "steep_circular":
         x1, x2, x3 = x
         y1, y2, y3 = y
         def _eval(x):
             if  x < x2:
                 return y1 - (y1 - y2) * math.sqrt(1 - ((x - x2)/(x2 - x1))**2)
             elif x > x2:
```

### Comparing `inferent-0.0.8/src/inferent.egg-info/PKG-INFO` & `inferent-0.0.9/src/inferent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inferent
-Version: 0.0.8
+Version: 0.0.9
 Summary: Inferent Ventures
 Author-email: Inferent Ventures <inferentventures@gmail.com>
 Project-URL: Homepage, https://github.com/inferent
 Project-URL: Issues, https://github.com/inferent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `inferent-0.0.8/src/tests/test_training.py` & `inferent-0.0.9/src/tests/test_training.py`

 * *Files identical despite different names*

### Comparing `inferent-0.0.8/src/tests/test_utils.py` & `inferent-0.0.9/src/tests/test_utils.py`

 * *Files identical despite different names*

