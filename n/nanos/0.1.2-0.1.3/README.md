# Comparing `tmp/nanos-0.1.2.tar.gz` & `tmp/nanos-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanos-0.1.2.tar", max compression
+gzip compressed data, was "nanos-0.1.3.tar", max compression
```

## Comparing `nanos-0.1.2.tar` & `nanos-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2024-04-08 18:09:24.196396 nanos-0.1.2/LICENSE
--rw-r--r--   0        0        0      112 2024-04-08 18:09:24.196396 nanos-0.1.2/README.md
--rw-r--r--   0        0        0       66 2024-04-08 18:09:24.196396 nanos-0.1.2/nanos/__init__.py
--rw-r--r--   0        0        0     2500 2024-04-08 18:09:24.196396 nanos-0.1.2/nanos/data.py
--rw-r--r--   0        0        0      814 2024-04-08 18:09:24.196396 nanos-0.1.2/nanos/dt.py
--rw-r--r--   0        0        0      408 2024-04-08 18:09:24.196396 nanos-0.1.2/nanos/fmt.py
--rw-r--r--   0        0        0      294 2024-04-08 18:09:24.196396 nanos-0.1.2/nanos/logging.py
--rw-r--r--   0        0        0     1021 2024-04-08 18:09:24.196396 nanos-0.1.2/nanos/time.py
--rw-r--r--   0        0        0     1449 2024-04-08 18:09:24.196396 nanos-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      854 1970-01-01 00:00:00.000000 nanos-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-16 07:34:40.282580 nanos-0.1.3/LICENSE
+-rw-r--r--   0        0        0      112 2024-05-16 07:34:40.282580 nanos-0.1.3/README.md
+-rw-r--r--   0        0        0       66 2024-05-16 07:34:40.282580 nanos-0.1.3/nanos/__init__.py
+-rw-r--r--   0        0        0     2500 2024-05-16 07:34:40.282580 nanos-0.1.3/nanos/data.py
+-rw-r--r--   0        0        0      814 2024-05-16 07:34:40.282580 nanos-0.1.3/nanos/dt.py
+-rw-r--r--   0        0        0      408 2024-05-16 07:34:40.282580 nanos-0.1.3/nanos/fmt.py
+-rw-r--r--   0        0        0      294 2024-05-16 07:34:40.282580 nanos-0.1.3/nanos/logging.py
+-rw-r--r--   0        0        0     1413 2024-05-16 07:34:40.282580 nanos-0.1.3/nanos/time.py
+-rw-r--r--   0        0        0     1449 2024-05-16 07:34:40.282580 nanos-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      854 1970-01-01 00:00:00.000000 nanos-0.1.3/PKG-INFO
```

### Comparing `nanos-0.1.2/LICENSE` & `nanos-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nanos-0.1.2/nanos/data.py` & `nanos-0.1.3/nanos/data.py`

 * *Files identical despite different names*

### Comparing `nanos-0.1.2/nanos/dt.py` & `nanos-0.1.3/nanos/dt.py`

 * *Files identical despite different names*

### Comparing `nanos-0.1.2/nanos/time.py` & `nanos-0.1.3/nanos/time.py`

 * *Files 24% similar despite different names*

```diff
@@ -24,16 +24,24 @@
     def __str__(self) -> str:
         return self.verbose()
 
     def __repr__(self) -> str:
         return f"<Timer [start={self.start}, end={self.end}]>"
 
     def verbose(self) -> str:
-        ms, seconds = math.modf(self.elapsed)
-        ms_part = round(ms, self.precision) * 10**self.precision
-        return f"{datetime.timedelta(seconds=seconds)}.{int(ms_part)}"
+        fraction_seconds, whole_seconds = math.modf(self.elapsed)
+        rounded_fraction = round(fraction_seconds, self.precision)
+        if rounded_fraction >= 1:
+            whole_seconds += 1
+            formatted_fraction = "0" * self.precision
+        elif fraction_seconds == 0:
+            formatted_fraction = "0" * self.precision
+        else:
+            fraction = int(rounded_fraction * 10**self.precision)
+            formatted_fraction = str(fraction).zfill(self.precision)
+        return f"{datetime.timedelta(seconds=whole_seconds)}.{formatted_fraction}"
 
     @property
     def elapsed(self) -> float:
         if not self.start:
             return 0.0
         return (self.end or time.time()) - self.start
```

### Comparing `nanos-0.1.2/pyproject.toml` & `nanos-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nanos"
-version = "0.1.2"
+version = "0.1.3"
 description = "Collection of small utility-functions"
 authors = ["Alex <aleosd@gmail.com>"]
 license = "Apache-2.0"
 homepage = "https://github.com/aleosd/nanos"
 repository = "https://github.com/aleosd/nanos"
 documentation = "https://github.com/aleosd/nanos"
 readme = "README.md"
```

### Comparing `nanos-0.1.2/PKG-INFO` & `nanos-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanos
-Version: 0.1.2
+Version: 0.1.3
 Summary: Collection of small utility-functions
 Home-page: https://github.com/aleosd/nanos
 License: Apache-2.0
 Author: Alex
 Author-email: aleosd@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

