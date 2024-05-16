# Comparing `tmp/pyselenscrapr-0.0.2.tar.gz` & `tmp/pyselenscrapr-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyselenscrapr-0.0.2.tar", last modified: Thu May 16 20:36:30 2024, max compression
+gzip compressed data, was "pyselenscrapr-0.0.3.tar", last modified: Thu May 16 20:43:42 2024, max compression
```

## Comparing `pyselenscrapr-0.0.2.tar` & `pyselenscrapr-0.0.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:36:30.110030 pyselenscrapr-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:36:30.102029 pyselenscrapr-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:36:30.106029 pyselenscrapr-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-16 20:36:30.110030 pyselenscrapr-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:36:30.106029 pyselenscrapr-0.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:36:30.106029 pyselenscrapr-0.0.2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/docs/source/pyselenscrapr.rst
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:36:30.110030 pyselenscrapr-0.0.2/pyselenscrapr/
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/pyselenscrapr/ScrapingBackend.py
--rw-r--r--   0 runner    (1001) docker     (127)    13087 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/pyselenscrapr/ScrapingBot.py
--rw-r--r--   0 runner    (1001) docker     (127)    12269 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/pyselenscrapr/ScrapingLogic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/pyselenscrapr/ScrapingStep.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/pyselenscrapr/ScrapingStepGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/pyselenscrapr/ScrapingStepLoop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/pyselenscrapr/ScrapingStepPagination.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/pyselenscrapr/ValidationError.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/pyselenscrapr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:36:30.110030 pyselenscrapr-0.0.2/pyselenscrapr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-16 20:36:30.000000 pyselenscrapr-0.0.2/pyselenscrapr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-16 20:36:30.000000 pyselenscrapr-0.0.2/pyselenscrapr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 20:36:30.000000 pyselenscrapr-0.0.2/pyselenscrapr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-16 20:36:30.000000 pyselenscrapr-0.0.2/pyselenscrapr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-16 20:36:30.000000 pyselenscrapr-0.0.2/pyselenscrapr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 20:36:30.110030 pyselenscrapr-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:43:42.634869 pyselenscrapr-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:43:42.626869 pyselenscrapr-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:43:42.630869 pyselenscrapr-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-16 20:43:31.000000 pyselenscrapr-0.0.3/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-16 20:43:31.000000 pyselenscrapr-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-16 20:43:31.000000 pyselenscrapr-0.0.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-16 20:43:31.000000 pyselenscrapr-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-16 20:43:42.634869 pyselenscrapr-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-16 20:43:31.000000 pyselenscrapr-0.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:43:42.630869 pyselenscrapr-0.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-16 20:43:31.000000 pyselenscrapr-0.0.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-16 20:43:31.000000 pyselenscrapr-0.0.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-16 20:43:31.000000 pyselenscrapr-0.0.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:43:42.630869 pyselenscrapr-0.0.3/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-16 20:43:31.000000 pyselenscrapr-0.0.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-16 20:43:31.000000 pyselenscrapr-0.0.3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-16 20:43:31.000000 pyselenscrapr-0.0.3/docs/source/pyselenscrapr.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-16 20:43:31.000000 pyselenscrapr-0.0.3/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-16 20:43:31.000000 pyselenscrapr-0.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:43:42.634869 pyselenscrapr-0.0.3/pyselenscrapr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-16 20:43:31.000000 pyselenscrapr-0.0.3/pyselenscrapr/ScrapingBackend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13217 2024-05-16 20:43:31.000000 pyselenscrapr-0.0.3/pyselenscrapr/ScrapingBot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12269 2024-05-16 20:43:31.000000 pyselenscrapr-0.0.3/pyselenscrapr/ScrapingLogic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-05-16 20:43:31.000000 pyselenscrapr-0.0.3/pyselenscrapr/ScrapingStep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-16 20:43:31.000000 pyselenscrapr-0.0.3/pyselenscrapr/ScrapingStepGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-16 20:43:31.000000 pyselenscrapr-0.0.3/pyselenscrapr/ScrapingStepLoop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-16 20:43:31.000000 pyselenscrapr-0.0.3/pyselenscrapr/ScrapingStepPagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-16 20:43:31.000000 pyselenscrapr-0.0.3/pyselenscrapr/ValidationError.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 20:43:31.000000 pyselenscrapr-0.0.3/pyselenscrapr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:43:42.634869 pyselenscrapr-0.0.3/pyselenscrapr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-16 20:43:42.000000 pyselenscrapr-0.0.3/pyselenscrapr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-16 20:43:42.000000 pyselenscrapr-0.0.3/pyselenscrapr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 20:43:42.000000 pyselenscrapr-0.0.3/pyselenscrapr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-16 20:43:42.000000 pyselenscrapr-0.0.3/pyselenscrapr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-16 20:43:42.000000 pyselenscrapr-0.0.3/pyselenscrapr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-05-16 20:43:31.000000 pyselenscrapr-0.0.3/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 20:43:42.634869 pyselenscrapr-0.0.3/setup.cfg
```

### Comparing `pyselenscrapr-0.0.2/.github/workflows/pypi.yml` & `pyselenscrapr-0.0.3/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.2/LICENSE` & `pyselenscrapr-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.2/PKG-INFO` & `pyselenscrapr-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyselenscrapr
-Version: 0.0.2
+Version: 0.0.3
 Summary: A web scraping library for selenium and beautifulsoup
 Author-email: donnercody <donnercody86@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: beautifulsoup4
```

### Comparing `pyselenscrapr-0.0.2/README.rst` & `pyselenscrapr-0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.2/docs/Makefile` & `pyselenscrapr-0.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.2/docs/make.bat` & `pyselenscrapr-0.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.2/docs/source/conf.py` & `pyselenscrapr-0.0.3/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import sys
 sys.path.insert(0, os.path.abspath(os.path.join("..", "..")))
 
 project = 'PySelenScrapr'
 copyright = '2024, Thoren Lederer'
 author = 'donnercody'
 
-release = '0.0.2'
-version = '0.0.2'
+release = '0.0.3'
+version = '0.0.3'
 
 # -- General configuration
 
 extensions = [
     'sphinx.ext.duration',
     'sphinx.ext.doctest',
     'sphinx.ext.autodoc',
```

### Comparing `pyselenscrapr-0.0.2/docs/source/index.rst` & `pyselenscrapr-0.0.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.2/docs/source/pyselenscrapr.rst` & `pyselenscrapr-0.0.3/docs/source/pyselenscrapr.rst`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.2/docs/source/usage.rst` & `pyselenscrapr-0.0.3/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.2/pyselenscrapr/ScrapingBackend.py` & `pyselenscrapr-0.0.3/pyselenscrapr/ScrapingBackend.py`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.2/pyselenscrapr/ScrapingBot.py` & `pyselenscrapr-0.0.3/pyselenscrapr/ScrapingBot.py`

 * *Files 1% similar despite different names*

```diff
@@ -313,14 +313,18 @@
         try:
             if self._backend is not None:
                 d_converted = self.get_converted_data(data)
                 self._backend.saveData(d_converted)
         except Exception as e:
             self._on_warning(e)
 
+    def send_error_to_backend(self, error):
+        if self._backend is not None:
+            self._backend.errorHandling(error)
+
     def send_data_to_backend(self, key=None, data=None):
         if data is None:
             data = self._data
         if key is not None:
             data = data[key]
 
         self.save_backend_data(data)
```

### Comparing `pyselenscrapr-0.0.2/pyselenscrapr/ScrapingLogic.py` & `pyselenscrapr-0.0.3/pyselenscrapr/ScrapingLogic.py`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.2/pyselenscrapr/ScrapingStep.py` & `pyselenscrapr-0.0.3/pyselenscrapr/ScrapingStep.py`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.2/pyselenscrapr/ScrapingStepLoop.py` & `pyselenscrapr-0.0.3/pyselenscrapr/ScrapingStepLoop.py`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.2/pyselenscrapr/ScrapingStepPagination.py` & `pyselenscrapr-0.0.3/pyselenscrapr/ScrapingStepPagination.py`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.2/pyselenscrapr.egg-info/PKG-INFO` & `pyselenscrapr-0.0.3/pyselenscrapr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyselenscrapr
-Version: 0.0.2
+Version: 0.0.3
 Summary: A web scraping library for selenium and beautifulsoup
 Author-email: donnercody <donnercody86@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: beautifulsoup4
```

### Comparing `pyselenscrapr-0.0.2/pyselenscrapr.egg-info/SOURCES.txt` & `pyselenscrapr-0.0.3/pyselenscrapr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.2/sample.py` & `pyselenscrapr-0.0.3/sample.py`

 * *Files identical despite different names*

