# Comparing `tmp/pyselenscrapr-0.0.1.tar.gz` & `tmp/pyselenscrapr-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyselenscrapr-0.0.1.tar", last modified: Wed May 15 22:53:55 2024, max compression
+gzip compressed data, was "pyselenscrapr-0.0.2.tar", last modified: Thu May 16 20:36:30 2024, max compression
```

## Comparing `pyselenscrapr-0.0.1.tar` & `pyselenscrapr-0.0.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:53:55.647829 pyselenscrapr-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:53:55.639829 pyselenscrapr-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:53:55.643829 pyselenscrapr-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-15 22:53:41.000000 pyselenscrapr-0.0.1/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-15 22:53:41.000000 pyselenscrapr-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-15 22:53:41.000000 pyselenscrapr-0.0.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-15 22:53:41.000000 pyselenscrapr-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-05-15 22:53:55.647829 pyselenscrapr-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-15 22:53:41.000000 pyselenscrapr-0.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:53:55.643829 pyselenscrapr-0.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-15 22:53:41.000000 pyselenscrapr-0.0.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-15 22:53:41.000000 pyselenscrapr-0.0.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-15 22:53:41.000000 pyselenscrapr-0.0.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:53:55.643829 pyselenscrapr-0.0.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-15 22:53:41.000000 pyselenscrapr-0.0.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-15 22:53:41.000000 pyselenscrapr-0.0.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-15 22:53:41.000000 pyselenscrapr-0.0.1/docs/source/pyselenscrapr.rst
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-15 22:53:41.000000 pyselenscrapr-0.0.1/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-15 22:53:41.000000 pyselenscrapr-0.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:53:55.643829 pyselenscrapr-0.0.1/pyselenscrapr/
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-15 22:53:41.000000 pyselenscrapr-0.0.1/pyselenscrapr/ScrapingBackend.py
--rw-r--r--   0 runner    (1001) docker     (127)    12366 2024-05-15 22:53:41.000000 pyselenscrapr-0.0.1/pyselenscrapr/ScrapingBot.py
--rw-r--r--   0 runner    (1001) docker     (127)    12042 2024-05-15 22:53:41.000000 pyselenscrapr-0.0.1/pyselenscrapr/ScrapingLogic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-05-15 22:53:41.000000 pyselenscrapr-0.0.1/pyselenscrapr/ScrapingStep.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-15 22:53:41.000000 pyselenscrapr-0.0.1/pyselenscrapr/ScrapingStepGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-15 22:53:41.000000 pyselenscrapr-0.0.1/pyselenscrapr/ScrapingStepLoop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-15 22:53:41.000000 pyselenscrapr-0.0.1/pyselenscrapr/ScrapingStepPagination.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-15 22:53:41.000000 pyselenscrapr-0.0.1/pyselenscrapr/ValidationError.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:53:41.000000 pyselenscrapr-0.0.1/pyselenscrapr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:53:55.643829 pyselenscrapr-0.0.1/pyselenscrapr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-05-15 22:53:55.000000 pyselenscrapr-0.0.1/pyselenscrapr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-15 22:53:55.000000 pyselenscrapr-0.0.1/pyselenscrapr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 22:53:55.000000 pyselenscrapr-0.0.1/pyselenscrapr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-15 22:53:55.000000 pyselenscrapr-0.0.1/pyselenscrapr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 22:53:55.000000 pyselenscrapr-0.0.1/pyselenscrapr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-05-15 22:53:41.000000 pyselenscrapr-0.0.1/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 22:53:55.647829 pyselenscrapr-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:36:30.110030 pyselenscrapr-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:36:30.102029 pyselenscrapr-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:36:30.106029 pyselenscrapr-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-16 20:36:30.110030 pyselenscrapr-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:36:30.106029 pyselenscrapr-0.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:36:30.106029 pyselenscrapr-0.0.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/docs/source/pyselenscrapr.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:36:30.110030 pyselenscrapr-0.0.2/pyselenscrapr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/pyselenscrapr/ScrapingBackend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13087 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/pyselenscrapr/ScrapingBot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12269 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/pyselenscrapr/ScrapingLogic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/pyselenscrapr/ScrapingStep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/pyselenscrapr/ScrapingStepGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/pyselenscrapr/ScrapingStepLoop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/pyselenscrapr/ScrapingStepPagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/pyselenscrapr/ValidationError.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/pyselenscrapr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:36:30.110030 pyselenscrapr-0.0.2/pyselenscrapr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-16 20:36:30.000000 pyselenscrapr-0.0.2/pyselenscrapr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-16 20:36:30.000000 pyselenscrapr-0.0.2/pyselenscrapr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 20:36:30.000000 pyselenscrapr-0.0.2/pyselenscrapr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-16 20:36:30.000000 pyselenscrapr-0.0.2/pyselenscrapr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-16 20:36:30.000000 pyselenscrapr-0.0.2/pyselenscrapr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-05-16 20:36:19.000000 pyselenscrapr-0.0.2/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 20:36:30.110030 pyselenscrapr-0.0.2/setup.cfg
```

### Comparing `pyselenscrapr-0.0.1/.github/workflows/pypi.yml` & `pyselenscrapr-0.0.2/.github/workflows/pypi.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 name: Create pyselenscryper pypi package
 
 on:
-  workflow_dispatch:
   push:
     branches:
       - develop
-      - master
+      - main
 
 jobs:
   build-pypi:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v2
```

### Comparing `pyselenscrapr-0.0.1/LICENSE` & `pyselenscrapr-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.1/PKG-INFO` & `pyselenscrapr-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyselenscrapr
-Version: 0.0.1
+Version: 0.0.2
 Summary: A web scraping library for selenium and beautifulsoup
 Author-email: donnercody <donnercody86@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: beautifulsoup4
@@ -73,14 +73,14 @@
     finally:
        driver.quit()
 
 
 Documentation
 ~~~~~~~~~~~~~
 
-The
+The documentation is available at https://pyselenscrapr.readthedocs.io/.
 
 License
 -------
 
 This project is licensed under the MIT License - see the
 `LICENSE.md <LICENSE.md>`__ file for details
```

### Comparing `pyselenscrapr-0.0.1/README.rst` & `pyselenscrapr-0.0.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -57,14 +57,14 @@
     finally:
        driver.quit()
 
 
 Documentation
 ~~~~~~~~~~~~~
 
-The
+The documentation is available at https://pyselenscrapr.readthedocs.io/.
 
 License
 -------
 
 This project is licensed under the MIT License - see the
 `LICENSE.md <LICENSE.md>`__ file for details
```

### Comparing `pyselenscrapr-0.0.1/docs/Makefile` & `pyselenscrapr-0.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.1/docs/make.bat` & `pyselenscrapr-0.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.1/docs/source/conf.py` & `pyselenscrapr-0.0.2/docs/source/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import sys
 sys.path.insert(0, os.path.abspath(os.path.join("..", "..")))
 
 project = 'PySelenScrapr'
 copyright = '2024, Thoren Lederer'
 author = 'donnercody'
 
-release = '0.1'
-version = '0.1.0'
+release = '0.0.2'
+version = '0.0.2'
 
 # -- General configuration
 
 extensions = [
     'sphinx.ext.duration',
     'sphinx.ext.doctest',
     'sphinx.ext.autodoc',
```

### Comparing `pyselenscrapr-0.0.1/docs/source/pyselenscrapr.rst` & `pyselenscrapr-0.0.2/docs/source/pyselenscrapr.rst`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.1/docs/source/usage.rst` & `pyselenscrapr-0.0.2/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.1/pyselenscrapr/ScrapingBackend.py` & `pyselenscrapr-0.0.2/pyselenscrapr/ScrapingBackend.py`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.1/pyselenscrapr/ScrapingBot.py` & `pyselenscrapr-0.0.2/pyselenscrapr/ScrapingBot.py`

 * *Files 4% similar despite different names*

```diff
@@ -293,23 +293,48 @@
         self.sleep(1)
         return True
 
     ##############################################################################################################
     # Data handling
     ##############################################################################################################
 
-    def set_data(self, key, value):
-        self._data[key] = value
+    def get_converted_data(self, data):
+        retdata = {}
+        for key, value in data.items():
+            if isinstance(value, pd.DataFrame):
+                retdata[key] = value.to_dict(orient='records')
+            elif isinstance(value, pd.DataSeries):
+                retdata[key] = value.to_dict()
+            else:
+                retdata[key] = value
+
+        return retdata
+
+    def save_backend_data(self, data):
         try:
             if self._backend is not None:
-                self._backend.saveData(self._data, key)
+                d_converted = self.get_converted_data(data)
+                self._backend.saveData(d_converted)
         except Exception as e:
             self._on_warning(e)
 
-    def append_data(self, key, value):
+    def send_data_to_backend(self, key=None, data=None):
+        if data is None:
+            data = self._data
+        if key is not None:
+            data = data[key]
+
+        self.save_backend_data(data)
+
+    def set_data(self, key, value, send_to_backend=False):
+        self._data[key] = value
+        if send_to_backend:
+            self.save_backend_data({key: value})
+
+    def append_data(self, key, value, send_to_backend=False):
         if key in self._data:
             # pandas dataframe
             if isinstance(self._data[key], pd.DataFrame):
                 # append elements to the dataframe
                 self._data[key] = self._data[key]._append(value, ignore_index=True)
             elif isinstance(self._data[key], list):
                 self._data[key].append(value)
@@ -327,19 +352,17 @@
                 self._data[key] = [self._data[key], value]
             # pandas dataframe
             elif isinstance(self._data[key], pd.DataFrame):
                 # append elements to the dataframe
                 self._data[key] = self._data[key].append(value)
         else:
             self._data[key] = value
-        try:
-            if self._backend is not None:
-                self._backend.saveData(self._data, key)
-        except Exception as e:
-            self._on_warning(e)
+
+        if send_to_backend:
+            self.save_backend_data({key: value})
 
     def has_data(self, key):
         if key in self._data:
             return True
         return False
 
     def get_data(self, key):
```

### Comparing `pyselenscrapr-0.0.1/pyselenscrapr/ScrapingLogic.py` & `pyselenscrapr-0.0.2/pyselenscrapr/ScrapingLogic.py`

 * *Files 5% similar despite different names*

```diff
@@ -123,25 +123,28 @@
     def is_visible(self, selector):
         e = self.get_best_element(selector)
         if e is None:
             return False
         displayed = e.is_displayed()
         return displayed
 
-    def set_data(self, key, value):
-        self._bot.set_data(key, value)
+    def set_data(self, key, value, send_to_backend=False):
+        self._bot.set_data(key, value, send_to_backend=send_to_backend)
 
     def take_screenshot(self, step):
         try:
             self._bot._take_screenshot(step)
         except Exception as e:
             pass
 
-    def append_data(self, key, value):
-        self._bot.append_data(key, value)
+    def append_data(self, key, value, send_to_backend=False):
+        self._bot.append_data(key, value, send_to_backend=send_to_backend)
+
+    def send_data_to_backend(self, key=None, data=None):
+        return self._bot.send_data_to_backend(key, data)
 
     def has_data(self, key):
         return self._bot.has_data(key)
 
     def get_data(self, key):
         return self._bot.get_data(key)
```

### Comparing `pyselenscrapr-0.0.1/pyselenscrapr/ScrapingStep.py` & `pyselenscrapr-0.0.2/pyselenscrapr/ScrapingStep.py`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.1/pyselenscrapr/ScrapingStepLoop.py` & `pyselenscrapr-0.0.2/pyselenscrapr/ScrapingStepLoop.py`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.1/pyselenscrapr/ScrapingStepPagination.py` & `pyselenscrapr-0.0.2/pyselenscrapr/ScrapingStepPagination.py`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.1/pyselenscrapr.egg-info/PKG-INFO` & `pyselenscrapr-0.0.2/pyselenscrapr.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyselenscrapr
-Version: 0.0.1
+Version: 0.0.2
 Summary: A web scraping library for selenium and beautifulsoup
 Author-email: donnercody <donnercody86@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: beautifulsoup4
@@ -73,14 +73,14 @@
     finally:
        driver.quit()
 
 
 Documentation
 ~~~~~~~~~~~~~
 
-The
+The documentation is available at https://pyselenscrapr.readthedocs.io/.
 
 License
 -------
 
 This project is licensed under the MIT License - see the
 `LICENSE.md <LICENSE.md>`__ file for details
```

### Comparing `pyselenscrapr-0.0.1/pyselenscrapr.egg-info/SOURCES.txt` & `pyselenscrapr-0.0.2/pyselenscrapr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.1/sample.py` & `pyselenscrapr-0.0.2/sample.py`

 * *Files identical despite different names*

