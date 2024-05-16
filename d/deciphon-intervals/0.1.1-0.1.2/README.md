# Comparing `tmp/deciphon_intervals-0.1.1.tar.gz` & `tmp/deciphon_intervals-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deciphon_intervals-0.1.1.tar", max compression
+gzip compressed data, was "deciphon_intervals-0.1.2.tar", max compression
```

## Comparing `deciphon_intervals-0.1.1.tar` & `deciphon_intervals-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1069 2024-02-19 16:29:33.860356 deciphon_intervals-0.1.1/LICENSE
--rw-r--r--   0        0        0      567 2024-02-19 16:29:33.860356 deciphon_intervals-0.1.1/README.md
--rw-r--r--   0        0        0     2800 2024-02-19 16:29:33.860356 deciphon_intervals-0.1.1/deciphon_intervals/__init__.py
--rw-r--r--   0        0        0      367 2024-02-19 16:29:33.860356 deciphon_intervals-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1175 1970-01-01 00:00:00.000000 deciphon_intervals-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-16 11:07:19.042298 deciphon_intervals-0.1.2/LICENSE
+-rw-r--r--   0        0        0      567 2024-05-16 11:07:19.042298 deciphon_intervals-0.1.2/README.md
+-rw-r--r--   0        0        0     2776 2024-05-16 11:07:19.042298 deciphon_intervals-0.1.2/deciphon_intervals/__init__.py
+-rw-r--r--   0        0        0      365 2024-05-16 11:07:19.042298 deciphon_intervals-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1171 1970-01-01 00:00:00.000000 deciphon_intervals-0.1.2/PKG-INFO
```

### Comparing `deciphon_intervals-0.1.1/LICENSE` & `deciphon_intervals-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deciphon_intervals-0.1.1/README.md` & `deciphon_intervals-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `deciphon_intervals-0.1.1/deciphon_intervals/__init__.py` & `deciphon_intervals-0.1.2/deciphon_intervals/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,26 +7,23 @@
 
 __all__ = ["Interval", "PyInterval", "RInterval"]
 
 
 class Interval(BaseModel, ABC):
     @property
     @abstractmethod
-    def r(self) -> RInterval:
-        ...
+    def r(self) -> RInterval: ...
 
     @property
     @abstractmethod
-    def py(self) -> PyInterval:
-        ...
+    def py(self) -> PyInterval: ...
 
     @property
     @abstractmethod
-    def slice(self) -> slice:
-        ...
+    def slice(self) -> slice: ...
 
 
 class PyInterval(Interval):
     """
     Python interval.
 
     A Python interval is an 0-start, half-open one. It means that:
```

### Comparing `deciphon_intervals-0.1.1/PKG-INFO` & `deciphon_intervals-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: deciphon-intervals
-Version: 0.1.1
+Version: 0.1.2
 Summary: It helps to model the Python and R intervals seamlessly.
 License: MIT
 Author: Danilo Horta
 Author-email: danilo.horta@pm.me
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: pydantic (>=2.6.1,<3.0.0)
+Requires-Dist: pydantic (>=2.7,<3.0)
 Description-Content-Type: text/markdown
 
 # deciphon-intervals
 
 It helps to model the two primary interval definitions in the programming
 realm: 0-start, half-open interval (aka Python interval), and 1-start,
 fully-closed interval (aka R interval).
```

