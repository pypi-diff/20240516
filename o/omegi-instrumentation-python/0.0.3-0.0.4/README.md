# Comparing `tmp/omegi-instrumentation-python-0.0.3.tar.gz` & `tmp/omegi-instrumentation-python-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omegi-instrumentation-python-0.0.3.tar", last modified: Thu May 16 15:54:58 2024, max compression
+gzip compressed data, was "omegi-instrumentation-python-0.0.4.tar", last modified: Thu May 16 16:15:29 2024, max compression
```

## Comparing `omegi-instrumentation-python-0.0.3.tar` & `omegi-instrumentation-python-0.0.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 15:54:58.929813 omegi-instrumentation-python-0.0.3/
--rw-r--r--   0 whisenlantern   (501) staff       (20)      807 2024-05-16 15:54:58.929681 omegi-instrumentation-python-0.0.3/PKG-INFO
--rw-r--r--   0 whisenlantern   (501) staff       (20)      405 2024-05-16 15:36:10.000000 omegi-instrumentation-python-0.0.3/README.md
--rw-r--r--   0 whisenlantern   (501) staff       (20)      103 2024-05-07 06:17:54.000000 omegi-instrumentation-python-0.0.3/pyproject.toml
--rw-r--r--   0 whisenlantern   (501) staff       (20)       38 2024-05-16 15:54:58.929859 omegi-instrumentation-python-0.0.3/setup.cfg
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2436 2024-05-16 15:54:49.000000 omegi-instrumentation-python-0.0.3/setup.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 15:54:58.925119 omegi-instrumentation-python-0.0.3/src/
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 15:54:58.925822 omegi-instrumentation-python-0.0.3/src/omegi/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2949 2024-05-16 15:54:25.000000 omegi-instrumentation-python-0.0.3/src/omegi/__init__.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 15:54:58.926389 omegi-instrumentation-python-0.0.3/src/omegi/decorator/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2223 2024-05-14 06:38:33.000000 omegi-instrumentation-python-0.0.3/src/omegi/decorator/OmegiDecorator.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 00:41:28.000000 omegi-instrumentation-python-0.0.3/src/omegi/decorator/__init__.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 15:54:58.926906 omegi-instrumentation-python-0.0.3/src/omegi/exporter/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2133 2024-05-16 15:29:55.000000 omegi-instrumentation-python-0.0.3/src/omegi/exporter/OmegiSpanExporter.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 00:41:10.000000 omegi-instrumentation-python-0.0.3/src/omegi/exporter/__init__.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 15:54:58.927209 omegi-instrumentation-python-0.0.3/src/omegi/generator/
--rw-r--r--   0 whisenlantern   (501) staff       (20)      299 2024-05-16 15:54:01.000000 omegi-instrumentation-python-0.0.3/src/omegi/generator/OmegiIdGenerator.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-16 07:10:31.000000 omegi-instrumentation-python-0.0.3/src/omegi/generator/__init__.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 15:54:58.928817 omegi-instrumentation-python-0.0.3/src/omegi/util/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     1856 2024-05-16 14:38:52.000000 omegi-instrumentation-python-0.0.3/src/omegi/util/OmegiDependencyInstrument.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2646 2024-05-16 15:48:09.000000 omegi-instrumentation-python-0.0.3/src/omegi/util/OmegiErrorSpanFormatter.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)      840 2024-05-14 07:24:09.000000 omegi-instrumentation-python-0.0.3/src/omegi/util/OmegiSamplerSpanFormatter.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)     1529 2024-05-14 08:52:40.000000 omegi-instrumentation-python-0.0.3/src/omegi/util/OmegiTracingSetup.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)      623 2024-05-14 06:53:00.000000 omegi-instrumentation-python-0.0.3/src/omegi/util/UtilFunction.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:04:48.000000 omegi-instrumentation-python-0.0.3/src/omegi/util/__init__.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 15:54:58.929472 omegi-instrumentation-python-0.0.3/src/omegi_instrumentation_python.egg-info/
--rw-r--r--   0 whisenlantern   (501) staff       (20)      807 2024-05-16 15:54:58.000000 omegi-instrumentation-python-0.0.3/src/omegi_instrumentation_python.egg-info/PKG-INFO
--rw-r--r--   0 whisenlantern   (501) staff       (20)      771 2024-05-16 15:54:58.000000 omegi-instrumentation-python-0.0.3/src/omegi_instrumentation_python.egg-info/SOURCES.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)        1 2024-05-16 15:54:58.000000 omegi-instrumentation-python-0.0.3/src/omegi_instrumentation_python.egg-info/dependency_links.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)     1151 2024-05-16 15:54:58.000000 omegi-instrumentation-python-0.0.3/src/omegi_instrumentation_python.egg-info/requires.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)        6 2024-05-16 15:54:58.000000 omegi-instrumentation-python-0.0.3/src/omegi_instrumentation_python.egg-info/top_level.txt
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 16:15:29.757596 omegi-instrumentation-python-0.0.4/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      807 2024-05-16 16:15:29.757472 omegi-instrumentation-python-0.0.4/PKG-INFO
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      405 2024-05-16 15:36:10.000000 omegi-instrumentation-python-0.0.4/README.md
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      103 2024-05-07 06:17:54.000000 omegi-instrumentation-python-0.0.4/pyproject.toml
+-rw-r--r--   0 whisenlantern   (501) staff       (20)       38 2024-05-16 16:15:29.757640 omegi-instrumentation-python-0.0.4/setup.cfg
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2436 2024-05-16 16:15:25.000000 omegi-instrumentation-python-0.0.4/setup.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 16:15:29.753922 omegi-instrumentation-python-0.0.4/src/
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 16:15:29.754379 omegi-instrumentation-python-0.0.4/src/omegi/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2906 2024-05-16 16:14:12.000000 omegi-instrumentation-python-0.0.4/src/omegi/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 16:15:29.754833 omegi-instrumentation-python-0.0.4/src/omegi/decorator/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2223 2024-05-14 06:38:33.000000 omegi-instrumentation-python-0.0.4/src/omegi/decorator/OmegiDecorator.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 00:41:28.000000 omegi-instrumentation-python-0.0.4/src/omegi/decorator/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 16:15:29.755163 omegi-instrumentation-python-0.0.4/src/omegi/exporter/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2133 2024-05-16 15:29:55.000000 omegi-instrumentation-python-0.0.4/src/omegi/exporter/OmegiSpanExporter.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 00:41:10.000000 omegi-instrumentation-python-0.0.4/src/omegi/exporter/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 16:15:29.755403 omegi-instrumentation-python-0.0.4/src/omegi/generator/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      299 2024-05-16 15:54:01.000000 omegi-instrumentation-python-0.0.4/src/omegi/generator/OmegiIdGenerator.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-16 07:10:31.000000 omegi-instrumentation-python-0.0.4/src/omegi/generator/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 16:15:29.756759 omegi-instrumentation-python-0.0.4/src/omegi/util/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     1856 2024-05-16 14:38:52.000000 omegi-instrumentation-python-0.0.4/src/omegi/util/OmegiDependencyInstrument.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2646 2024-05-16 15:48:09.000000 omegi-instrumentation-python-0.0.4/src/omegi/util/OmegiErrorSpanFormatter.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      840 2024-05-14 07:24:09.000000 omegi-instrumentation-python-0.0.4/src/omegi/util/OmegiSamplerSpanFormatter.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     1529 2024-05-14 08:52:40.000000 omegi-instrumentation-python-0.0.4/src/omegi/util/OmegiTracingSetup.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      623 2024-05-14 06:53:00.000000 omegi-instrumentation-python-0.0.4/src/omegi/util/UtilFunction.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:04:48.000000 omegi-instrumentation-python-0.0.4/src/omegi/util/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 16:15:29.757307 omegi-instrumentation-python-0.0.4/src/omegi_instrumentation_python.egg-info/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      807 2024-05-16 16:15:29.000000 omegi-instrumentation-python-0.0.4/src/omegi_instrumentation_python.egg-info/PKG-INFO
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      771 2024-05-16 16:15:29.000000 omegi-instrumentation-python-0.0.4/src/omegi_instrumentation_python.egg-info/SOURCES.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        1 2024-05-16 16:15:29.000000 omegi-instrumentation-python-0.0.4/src/omegi_instrumentation_python.egg-info/dependency_links.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     1151 2024-05-16 16:15:29.000000 omegi-instrumentation-python-0.0.4/src/omegi_instrumentation_python.egg-info/requires.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        6 2024-05-16 16:15:29.000000 omegi-instrumentation-python-0.0.4/src/omegi_instrumentation_python.egg-info/top_level.txt
```

### Comparing `omegi-instrumentation-python-0.0.3/PKG-INFO` & `omegi-instrumentation-python-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omegi-instrumentation-python
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python Instrumentation for Automatic Error Logging
 Home-page: https://github.com/TeamOmegi/Instrumentation-Python
 Author: omegi
 Author-email: canon1107@naver.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `omegi-instrumentation-python-0.0.3/setup.py` & `omegi-instrumentation-python-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="omegi-instrumentation-python",
-    version="0.0.3",
+    version="0.0.4",
     author="omegi",
     author_email="canon1107@naver.com",
     description="Python Instrumentation for Automatic Error Logging",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TeamOmegi/Instrumentation-Python",
     classifiers=[
```

### Comparing `omegi-instrumentation-python-0.0.3/src/omegi/__init__.py` & `omegi-instrumentation-python-0.0.4/src/omegi/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,16 +42,15 @@
         if self.project_root is None:
             logging.error("Please set Project root")
         # Setup Propagator, Custom Exporter, SpanProcessor
         propagator = TraceContextTextMapPropagator()
         propagate.set_global_textmap(propagator)
         span_processor = BatchSpanProcessor(self._set_exporter())
         trace.set_tracer_provider(TracerProvider(
-            resource=Resource.create({"service.name": os.getenv("OMEGI_SERVICE_NAME", 'test-server')}),
-            id_generator=HexIdGenerator()
+            resource=Resource.create({"service.name": os.getenv("OMEGI_SERVICE_NAME", 'test-server')})
         ))
         trace.get_tracer_provider().add_span_processor(span_processor)
         tracer = trace.get_tracer(__name__)
         # Setup Instrumentation
         if self.app is not None:
             self._start_depending_instrumentation(app=self.app)
         # Setup Tracing Functions
```

### Comparing `omegi-instrumentation-python-0.0.3/src/omegi/decorator/OmegiDecorator.py` & `omegi-instrumentation-python-0.0.4/src/omegi/decorator/OmegiDecorator.py`

 * *Files identical despite different names*

### Comparing `omegi-instrumentation-python-0.0.3/src/omegi/exporter/OmegiSpanExporter.py` & `omegi-instrumentation-python-0.0.4/src/omegi/exporter/OmegiSpanExporter.py`

 * *Files identical despite different names*

### Comparing `omegi-instrumentation-python-0.0.3/src/omegi/util/OmegiDependencyInstrument.py` & `omegi-instrumentation-python-0.0.4/src/omegi/util/OmegiDependencyInstrument.py`

 * *Files identical despite different names*

### Comparing `omegi-instrumentation-python-0.0.3/src/omegi/util/OmegiErrorSpanFormatter.py` & `omegi-instrumentation-python-0.0.4/src/omegi/util/OmegiErrorSpanFormatter.py`

 * *Files identical despite different names*

### Comparing `omegi-instrumentation-python-0.0.3/src/omegi/util/OmegiSamplerSpanFormatter.py` & `omegi-instrumentation-python-0.0.4/src/omegi/util/OmegiSamplerSpanFormatter.py`

 * *Files identical despite different names*

### Comparing `omegi-instrumentation-python-0.0.3/src/omegi/util/OmegiTracingSetup.py` & `omegi-instrumentation-python-0.0.4/src/omegi/util/OmegiTracingSetup.py`

 * *Files identical despite different names*

### Comparing `omegi-instrumentation-python-0.0.3/src/omegi/util/UtilFunction.py` & `omegi-instrumentation-python-0.0.4/src/omegi/util/UtilFunction.py`

 * *Files identical despite different names*

### Comparing `omegi-instrumentation-python-0.0.3/src/omegi_instrumentation_python.egg-info/PKG-INFO` & `omegi-instrumentation-python-0.0.4/src/omegi_instrumentation_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omegi-instrumentation-python
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python Instrumentation for Automatic Error Logging
 Home-page: https://github.com/TeamOmegi/Instrumentation-Python
 Author: omegi
 Author-email: canon1107@naver.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `omegi-instrumentation-python-0.0.3/src/omegi_instrumentation_python.egg-info/SOURCES.txt` & `omegi-instrumentation-python-0.0.4/src/omegi_instrumentation_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `omegi-instrumentation-python-0.0.3/src/omegi_instrumentation_python.egg-info/requires.txt` & `omegi-instrumentation-python-0.0.4/src/omegi_instrumentation_python.egg-info/requires.txt`

 * *Files identical despite different names*

