# Comparing `tmp/omegi-instrumentation-python-0.0.6.tar.gz` & `tmp/omegi-instrumentation-python-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omegi-instrumentation-python-0.0.6.tar", last modified: Thu May 16 17:28:37 2024, max compression
+gzip compressed data, was "omegi-instrumentation-python-0.0.7.tar", last modified: Thu May 16 17:42:03 2024, max compression
```

## Comparing `omegi-instrumentation-python-0.0.6.tar` & `omegi-instrumentation-python-0.0.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 17:28:37.577359 omegi-instrumentation-python-0.0.6/
--rw-r--r--   0 whisenlantern   (501) staff       (20)      807 2024-05-16 17:28:37.577249 omegi-instrumentation-python-0.0.6/PKG-INFO
--rw-r--r--   0 whisenlantern   (501) staff       (20)      405 2024-05-16 15:36:10.000000 omegi-instrumentation-python-0.0.6/README.md
--rw-r--r--   0 whisenlantern   (501) staff       (20)      103 2024-05-07 06:17:54.000000 omegi-instrumentation-python-0.0.6/pyproject.toml
--rw-r--r--   0 whisenlantern   (501) staff       (20)       38 2024-05-16 17:28:37.577395 omegi-instrumentation-python-0.0.6/setup.cfg
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2436 2024-05-16 17:28:31.000000 omegi-instrumentation-python-0.0.6/setup.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 17:28:37.573791 omegi-instrumentation-python-0.0.6/src/
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 17:28:37.574244 omegi-instrumentation-python-0.0.6/src/omegi/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2906 2024-05-16 16:14:12.000000 omegi-instrumentation-python-0.0.6/src/omegi/__init__.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 17:28:37.574699 omegi-instrumentation-python-0.0.6/src/omegi/decorator/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2223 2024-05-14 06:38:33.000000 omegi-instrumentation-python-0.0.6/src/omegi/decorator/OmegiDecorator.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 00:41:28.000000 omegi-instrumentation-python-0.0.6/src/omegi/decorator/__init__.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 17:28:37.575076 omegi-instrumentation-python-0.0.6/src/omegi/exporter/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2133 2024-05-16 15:29:55.000000 omegi-instrumentation-python-0.0.6/src/omegi/exporter/OmegiSpanExporter.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 00:41:10.000000 omegi-instrumentation-python-0.0.6/src/omegi/exporter/__init__.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 17:28:37.575320 omegi-instrumentation-python-0.0.6/src/omegi/generator/
--rw-r--r--   0 whisenlantern   (501) staff       (20)      299 2024-05-16 15:54:01.000000 omegi-instrumentation-python-0.0.6/src/omegi/generator/OmegiIdGenerator.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-16 07:10:31.000000 omegi-instrumentation-python-0.0.6/src/omegi/generator/__init__.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 17:28:37.576599 omegi-instrumentation-python-0.0.6/src/omegi/util/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     1856 2024-05-16 14:38:52.000000 omegi-instrumentation-python-0.0.6/src/omegi/util/OmegiDependencyInstrument.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2829 2024-05-16 17:28:14.000000 omegi-instrumentation-python-0.0.6/src/omegi/util/OmegiErrorSpanFormatter.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)      840 2024-05-14 07:24:09.000000 omegi-instrumentation-python-0.0.6/src/omegi/util/OmegiSamplerSpanFormatter.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)     1529 2024-05-14 08:52:40.000000 omegi-instrumentation-python-0.0.6/src/omegi/util/OmegiTracingSetup.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)      623 2024-05-14 06:53:00.000000 omegi-instrumentation-python-0.0.6/src/omegi/util/UtilFunction.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:04:48.000000 omegi-instrumentation-python-0.0.6/src/omegi/util/__init__.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 17:28:37.577095 omegi-instrumentation-python-0.0.6/src/omegi_instrumentation_python.egg-info/
--rw-r--r--   0 whisenlantern   (501) staff       (20)      807 2024-05-16 17:28:37.000000 omegi-instrumentation-python-0.0.6/src/omegi_instrumentation_python.egg-info/PKG-INFO
--rw-r--r--   0 whisenlantern   (501) staff       (20)      771 2024-05-16 17:28:37.000000 omegi-instrumentation-python-0.0.6/src/omegi_instrumentation_python.egg-info/SOURCES.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)        1 2024-05-16 17:28:37.000000 omegi-instrumentation-python-0.0.6/src/omegi_instrumentation_python.egg-info/dependency_links.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)     1151 2024-05-16 17:28:37.000000 omegi-instrumentation-python-0.0.6/src/omegi_instrumentation_python.egg-info/requires.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)        6 2024-05-16 17:28:37.000000 omegi-instrumentation-python-0.0.6/src/omegi_instrumentation_python.egg-info/top_level.txt
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 17:42:03.789565 omegi-instrumentation-python-0.0.7/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      807 2024-05-16 17:42:03.789433 omegi-instrumentation-python-0.0.7/PKG-INFO
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      405 2024-05-16 15:36:10.000000 omegi-instrumentation-python-0.0.7/README.md
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      103 2024-05-07 06:17:54.000000 omegi-instrumentation-python-0.0.7/pyproject.toml
+-rw-r--r--   0 whisenlantern   (501) staff       (20)       38 2024-05-16 17:42:03.789615 omegi-instrumentation-python-0.0.7/setup.cfg
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2436 2024-05-16 17:41:27.000000 omegi-instrumentation-python-0.0.7/setup.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 17:42:03.785719 omegi-instrumentation-python-0.0.7/src/
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 17:42:03.786240 omegi-instrumentation-python-0.0.7/src/omegi/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2906 2024-05-16 16:14:12.000000 omegi-instrumentation-python-0.0.7/src/omegi/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 17:42:03.786814 omegi-instrumentation-python-0.0.7/src/omegi/decorator/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2223 2024-05-14 06:38:33.000000 omegi-instrumentation-python-0.0.7/src/omegi/decorator/OmegiDecorator.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 00:41:28.000000 omegi-instrumentation-python-0.0.7/src/omegi/decorator/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 17:42:03.787179 omegi-instrumentation-python-0.0.7/src/omegi/exporter/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2133 2024-05-16 15:29:55.000000 omegi-instrumentation-python-0.0.7/src/omegi/exporter/OmegiSpanExporter.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 00:41:10.000000 omegi-instrumentation-python-0.0.7/src/omegi/exporter/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 17:42:03.787410 omegi-instrumentation-python-0.0.7/src/omegi/generator/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      299 2024-05-16 15:54:01.000000 omegi-instrumentation-python-0.0.7/src/omegi/generator/OmegiIdGenerator.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-16 07:10:31.000000 omegi-instrumentation-python-0.0.7/src/omegi/generator/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 17:42:03.788684 omegi-instrumentation-python-0.0.7/src/omegi/util/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     1856 2024-05-16 14:38:52.000000 omegi-instrumentation-python-0.0.7/src/omegi/util/OmegiDependencyInstrument.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2708 2024-05-16 17:41:47.000000 omegi-instrumentation-python-0.0.7/src/omegi/util/OmegiErrorSpanFormatter.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      840 2024-05-14 07:24:09.000000 omegi-instrumentation-python-0.0.7/src/omegi/util/OmegiSamplerSpanFormatter.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     1529 2024-05-14 08:52:40.000000 omegi-instrumentation-python-0.0.7/src/omegi/util/OmegiTracingSetup.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      623 2024-05-14 06:53:00.000000 omegi-instrumentation-python-0.0.7/src/omegi/util/UtilFunction.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:04:48.000000 omegi-instrumentation-python-0.0.7/src/omegi/util/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 17:42:03.789256 omegi-instrumentation-python-0.0.7/src/omegi_instrumentation_python.egg-info/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      807 2024-05-16 17:42:03.000000 omegi-instrumentation-python-0.0.7/src/omegi_instrumentation_python.egg-info/PKG-INFO
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      771 2024-05-16 17:42:03.000000 omegi-instrumentation-python-0.0.7/src/omegi_instrumentation_python.egg-info/SOURCES.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        1 2024-05-16 17:42:03.000000 omegi-instrumentation-python-0.0.7/src/omegi_instrumentation_python.egg-info/dependency_links.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     1151 2024-05-16 17:42:03.000000 omegi-instrumentation-python-0.0.7/src/omegi_instrumentation_python.egg-info/requires.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        6 2024-05-16 17:42:03.000000 omegi-instrumentation-python-0.0.7/src/omegi_instrumentation_python.egg-info/top_level.txt
```

### Comparing `omegi-instrumentation-python-0.0.6/PKG-INFO` & `omegi-instrumentation-python-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omegi-instrumentation-python
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python Instrumentation for Automatic Error Logging
 Home-page: https://github.com/TeamOmegi/Instrumentation-Python
 Author: omegi
 Author-email: canon1107@naver.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `omegi-instrumentation-python-0.0.6/setup.py` & `omegi-instrumentation-python-0.0.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="omegi-instrumentation-python",
-    version="0.0.6",
+    version="0.0.7",
     author="omegi",
     author_email="canon1107@naver.com",
     description="Python Instrumentation for Automatic Error Logging",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TeamOmegi/Instrumentation-Python",
     classifiers=[
```

### Comparing `omegi-instrumentation-python-0.0.6/src/omegi/__init__.py` & `omegi-instrumentation-python-0.0.7/src/omegi/__init__.py`

 * *Files identical despite different names*

### Comparing `omegi-instrumentation-python-0.0.6/src/omegi/decorator/OmegiDecorator.py` & `omegi-instrumentation-python-0.0.7/src/omegi/decorator/OmegiDecorator.py`

 * *Files identical despite different names*

### Comparing `omegi-instrumentation-python-0.0.6/src/omegi/exporter/OmegiSpanExporter.py` & `omegi-instrumentation-python-0.0.7/src/omegi/exporter/OmegiSpanExporter.py`

 * *Files identical despite different names*

### Comparing `omegi-instrumentation-python-0.0.6/src/omegi/util/OmegiDependencyInstrument.py` & `omegi-instrumentation-python-0.0.7/src/omegi/util/OmegiDependencyInstrument.py`

 * *Files identical despite different names*

### Comparing `omegi-instrumentation-python-0.0.6/src/omegi/util/OmegiErrorSpanFormatter.py` & `omegi-instrumentation-python-0.0.7/src/omegi/util/OmegiErrorSpanFormatter.py`

 * *Files 23% similar despite different names*

```diff
@@ -32,18 +32,16 @@
     data["serviceName"] = origin_spans[0].resource.attributes["service.name"]
     data["error"] = error
     data["spans"] = spans
     return data
 
 
 def _figure_internal_error(origin_spans: Sequence[Span]) -> bool:
-    if origin_spans[0].kind.name == SpanKind.CLIENT:
-        logging.info("Current Service is not Error Service")
+    if origin_spans[0].kind.name == 'CLIENT':
         return False
-    logging.info("Current Service is Error Service")
     return True
 
 
 def _extract_exception_flow(stack_trace):
     flow_steps = {}
     error_stack = []
     lines = stack_trace.strip().split('\n')
```

### Comparing `omegi-instrumentation-python-0.0.6/src/omegi/util/OmegiSamplerSpanFormatter.py` & `omegi-instrumentation-python-0.0.7/src/omegi/util/OmegiSamplerSpanFormatter.py`

 * *Files identical despite different names*

### Comparing `omegi-instrumentation-python-0.0.6/src/omegi/util/OmegiTracingSetup.py` & `omegi-instrumentation-python-0.0.7/src/omegi/util/OmegiTracingSetup.py`

 * *Files identical despite different names*

### Comparing `omegi-instrumentation-python-0.0.6/src/omegi/util/UtilFunction.py` & `omegi-instrumentation-python-0.0.7/src/omegi/util/UtilFunction.py`

 * *Files identical despite different names*

### Comparing `omegi-instrumentation-python-0.0.6/src/omegi_instrumentation_python.egg-info/PKG-INFO` & `omegi-instrumentation-python-0.0.7/src/omegi_instrumentation_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omegi-instrumentation-python
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python Instrumentation for Automatic Error Logging
 Home-page: https://github.com/TeamOmegi/Instrumentation-Python
 Author: omegi
 Author-email: canon1107@naver.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `omegi-instrumentation-python-0.0.6/src/omegi_instrumentation_python.egg-info/SOURCES.txt` & `omegi-instrumentation-python-0.0.7/src/omegi_instrumentation_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `omegi-instrumentation-python-0.0.6/src/omegi_instrumentation_python.egg-info/requires.txt` & `omegi-instrumentation-python-0.0.7/src/omegi_instrumentation_python.egg-info/requires.txt`

 * *Files identical despite different names*

