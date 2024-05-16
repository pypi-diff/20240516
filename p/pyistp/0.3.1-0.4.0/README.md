# Comparing `tmp/pyistp-0.3.1.tar.gz` & `tmp/pyistp-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyistp-0.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyistp-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyistp-0.3.1.tar` & `pyistp-0.4.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1552 2023-09-05 14:25:20.044407 pyistp-0.3.1/COPYING
--rw-r--r--   0        0        0      895 2023-09-05 14:25:20.044407 pyistp-0.3.1/README.rst
--rw-r--r--   0        0        0      296 2023-09-05 14:25:20.132408 pyistp-0.3.1/pyistp/__init__.py
--rw-r--r--   0        0        0     4720 2023-09-05 14:25:20.132408 pyistp-0.3.1/pyistp/_impl.py
--rw-r--r--   0        0        0      487 2023-09-05 14:25:20.132408 pyistp-0.3.1/pyistp/data_variable.py
--rw-r--r--   0        0        0      686 2023-09-05 14:25:20.132408 pyistp-0.3.1/pyistp/drivers/__init__.py
--rw-r--r--   0        0        0     1120 2023-09-05 14:25:20.132408 pyistp-0.3.1/pyistp/drivers/pycdfpp.py
--rw-r--r--   0        0        0     1408 2023-09-05 14:25:20.132408 pyistp-0.3.1/pyistp/drivers/spacepy.py
--rw-r--r--   0        0        0      566 2023-09-05 14:25:20.132408 pyistp-0.3.1/pyistp/loader.py
--rw-r--r--   0        0        0      493 2023-09-05 14:25:20.132408 pyistp-0.3.1/pyistp/support_data_variable.py
--rw-r--r--   0        0        0     1135 2023-09-05 14:25:20.132408 pyistp-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1912 1970-01-01 00:00:00.000000 pyistp-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1552 2023-10-19 08:54:55.463163 pyistp-0.4.0/COPYING
+-rw-r--r--   0        0        0      895 2023-10-19 08:54:55.463163 pyistp-0.4.0/README.rst
+-rw-r--r--   0        0        0      296 2023-10-19 08:54:55.543165 pyistp-0.4.0/pyistp/__init__.py
+-rw-r--r--   0        0        0     4747 2023-10-19 08:54:55.543165 pyistp-0.4.0/pyistp/_impl.py
+-rw-r--r--   0        0        0      487 2023-10-19 08:54:55.543165 pyistp-0.4.0/pyistp/data_variable.py
+-rw-r--r--   0        0        0      686 2023-10-19 08:54:55.547165 pyistp-0.4.0/pyistp/drivers/__init__.py
+-rw-r--r--   0        0        0     1641 2023-10-19 08:54:55.547165 pyistp-0.4.0/pyistp/drivers/pycdfpp.py
+-rw-r--r--   0        0        0     1436 2023-10-19 08:54:55.547165 pyistp-0.4.0/pyistp/drivers/spacepy.py
+-rw-r--r--   0        0        0      566 2023-10-19 08:54:55.547165 pyistp-0.4.0/pyistp/loader.py
+-rw-r--r--   0        0        0      493 2023-10-19 08:54:55.547165 pyistp-0.4.0/pyistp/support_data_variable.py
+-rw-r--r--   0        0        0     1181 2023-10-19 08:54:55.547165 pyistp-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1963 1970-01-01 00:00:00.000000 pyistp-0.4.0/PKG-INFO
```

### Comparing `pyistp-0.3.1/COPYING` & `pyistp-0.4.0/COPYING`

 * *Files identical despite different names*

### Comparing `pyistp-0.3.1/README.rst` & `pyistp-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `pyistp-0.3.1/pyistp/_impl.py` & `pyistp-0.4.0/pyistp/_impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 def _get_attributes(cdf: object, var: str):
     attrs = {}
     for attr in cdf.variable_attributes(var):
         value = cdf.variable_attribute_value(var, attr)
         if attr.endswith("_PTR") or attr[:-1].endswith("_PTR_"):
             if cdf.has_variable(value):
-                value = cdf.values(value)
+                value = cdf.values(value, is_metadata_variable=True)
                 if hasattr(value, 'tolist'):
                     attrs[attr] = value.tolist()
                 else:
                     attrs[attr] = value
             else:
                 log.warning(
                     f"{ISTP_NOT_COMPLIANT_W}: variable {var} has {attr} attribute which points to variable {value} which does not exist")
```

### Comparing `pyistp-0.3.1/pyistp/drivers/__init__.py` & `pyistp-0.4.0/pyistp/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyistp-0.3.1/pyistp/drivers/pycdfpp.py` & `pyistp-0.4.0/pyistp/drivers/spacepy.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,51 @@
-import pycdfpp
+from spacepy import pycdf
+import numpy as np
+from tempfile import NamedTemporaryFile
 
 
 class Driver:
     def __init__(self, file):
-        self.cdf = pycdfpp.load(file)
+        if type(file) is bytes:
+            self._tmpfile = NamedTemporaryFile()
+            self._tmpfile.write(file)
+            self._tmpfile.flush()
+            self.cdf = pycdf.CDF(self._tmpfile.name)
+        else:
+            self.cdf = pycdf.CDF(file)
 
     def attributes(self):
         if self.cdf:
-            return self.cdf.attributes.keys()
+            return self.cdf.attrs.keys()
         return []
 
     def attribute(self, key):
         if self.cdf:
-            return self.cdf.attributes[key]
+            return self.cdf.attrs[key]
         return None
 
     def variables(self):
         if self.cdf:
-            return list(self.cdf)
+            return self.cdf.keys()
         return []
 
     def has_variable(self, name):
         return name in self.cdf
 
-    def is_char(self, var):
-        return self.cdf[var].type == pycdfpp.CDF_CHAR
-
     def variable_attributes(self, var):
         if self.cdf:
-            return self.cdf[var].attributes.keys()
+            return self.cdf[var].attrs.keys()
         return []
 
+    def is_char(self,var):
+        return self.cdf[var].type() == pycdf.const.CDF_CHAR
+
     def variable_attribute_value(self, var, attr):
-        if self.cdf and var in self.cdf and attr in self.cdf[var].attributes:
-            return self.cdf[var].attributes[attr][0]
+        if self.cdf and var in self.cdf and attr in self.cdf[var].attrs:
+            return self.cdf[var].attrs[attr]
         return None
 
-    def values(self, var):
+    def values(self, var, is_metadata_variable=False):
         v = self.cdf[var]
-        if v.type in (pycdfpp.CDF_EPOCH, pycdfpp.CDF_EPOCH16, pycdfpp.CDF_TIME_TT2000):
-            return pycdfpp.to_datetime64(v)
-        return v.values
+        if v.type() in (pycdf.const.CDF_EPOCH, pycdf.const.CDF_EPOCH16, pycdf.const.CDF_TIME_TT2000):
+            return np.vectorize(np.datetime64)(v[:])
+        return v[:]
```

### Comparing `pyistp-0.3.1/pyistp/loader.py` & `pyistp-0.4.0/pyistp/loader.py`

 * *Files identical despite different names*

### Comparing `pyistp-0.3.1/pyproject.toml` & `pyistp-0.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "flit_core.buildapi"
 requires = ["flit_core"]
 
 [project]
 name = 'pyistp'
-version = "0.3.1"
+version = "0.4.0"
 description = "An easy to use ISTP loader package."
 keywords= ["satellite", "plasma-physics", "nasa-data", "amda", "cdpp", "CDF"]
 authors = [
   {name = "Alexis Jeandet", email = "alexis.jeandet@member.fsf.org" }
 ]
 
 maintainers = [
@@ -24,13 +24,14 @@
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
-dependencies = ['pycdfpp<=0.4.6']
+dependencies = ['pycdfpp>=0.6.0']
 [project.urls]
 homepage = "https://github.com/SciQLop/PyISTP"
 repository = "https://github.com/SciQLop/PyISTP"
 documentation = "https://pyistp.readthedocs.io/en/latest/"
```

### Comparing `pyistp-0.3.1/PKG-INFO` & `pyistp-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyistp
-Version: 0.3.1
+Version: 0.4.0
 Summary: An easy to use ISTP loader package.
 Keywords: satellite,plasma-physics,nasa-data,amda,cdpp,CDF
 Author-email: Alexis Jeandet <alexis.jeandet@member.fsf.org>
 Maintainer-email: Alexis Jeandet <alexis.jeandet@member.fsf.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
@@ -12,15 +12,16 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pycdfpp<=0.4.6
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: pycdfpp>=0.6.0
 Project-URL: documentation, https://pyistp.readthedocs.io/en/latest/
 Project-URL: homepage, https://github.com/SciQLop/PyISTP
 Project-URL: repository, https://github.com/SciQLop/PyISTP
 
 ==================
 Python ISTP loader
 ==================
```

