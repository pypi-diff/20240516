# Comparing `tmp/omegi-instrumentation-python-0.0.2.tar.gz` & `tmp/omegi-instrumentation-python-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omegi-instrumentation-python-0.0.2.tar", last modified: Thu May 16 15:37:06 2024, max compression
+gzip compressed data, was "omegi-instrumentation-python-0.0.3.tar", last modified: Thu May 16 15:54:58 2024, max compression
```

## Comparing `omegi-instrumentation-python-0.0.2.tar` & `omegi-instrumentation-python-0.0.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 15:37:06.116271 omegi-instrumentation-python-0.0.2/
--rw-r--r--   0 whisenlantern   (501) staff       (20)      807 2024-05-16 15:37:06.116040 omegi-instrumentation-python-0.0.2/PKG-INFO
--rw-r--r--   0 whisenlantern   (501) staff       (20)      405 2024-05-16 15:36:10.000000 omegi-instrumentation-python-0.0.2/README.md
--rw-r--r--   0 whisenlantern   (501) staff       (20)      103 2024-05-07 06:17:54.000000 omegi-instrumentation-python-0.0.2/pyproject.toml
--rw-r--r--   0 whisenlantern   (501) staff       (20)       38 2024-05-16 15:37:06.116450 omegi-instrumentation-python-0.0.2/setup.cfg
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2436 2024-05-16 15:36:10.000000 omegi-instrumentation-python-0.0.2/setup.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 15:37:06.111252 omegi-instrumentation-python-0.0.2/src/
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 15:37:06.111741 omegi-instrumentation-python-0.0.2/src/omegi/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2852 2024-05-16 15:29:55.000000 omegi-instrumentation-python-0.0.2/src/omegi/__init__.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 15:37:06.112522 omegi-instrumentation-python-0.0.2/src/omegi/decorator/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2223 2024-05-14 06:38:33.000000 omegi-instrumentation-python-0.0.2/src/omegi/decorator/OmegiDecorator.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 00:41:28.000000 omegi-instrumentation-python-0.0.2/src/omegi/decorator/__init__.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 15:37:06.112936 omegi-instrumentation-python-0.0.2/src/omegi/exporter/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2133 2024-05-16 15:29:55.000000 omegi-instrumentation-python-0.0.2/src/omegi/exporter/OmegiSpanExporter.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 00:41:10.000000 omegi-instrumentation-python-0.0.2/src/omegi/exporter/__init__.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 15:37:06.113231 omegi-instrumentation-python-0.0.2/src/omegi/generator/
--rw-r--r--   0 whisenlantern   (501) staff       (20)       95 2024-05-16 07:39:50.000000 omegi-instrumentation-python-0.0.2/src/omegi/generator/OmegiIdGenerator.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-16 07:10:31.000000 omegi-instrumentation-python-0.0.2/src/omegi/generator/__init__.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 15:37:06.114648 omegi-instrumentation-python-0.0.2/src/omegi/util/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     1856 2024-05-16 14:38:52.000000 omegi-instrumentation-python-0.0.2/src/omegi/util/OmegiDependencyInstrument.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2623 2024-05-16 14:35:48.000000 omegi-instrumentation-python-0.0.2/src/omegi/util/OmegiErrorSpanFormatter.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)      840 2024-05-14 07:24:09.000000 omegi-instrumentation-python-0.0.2/src/omegi/util/OmegiSamplerSpanFormatter.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)     1529 2024-05-14 08:52:40.000000 omegi-instrumentation-python-0.0.2/src/omegi/util/OmegiTracingSetup.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)      623 2024-05-14 06:53:00.000000 omegi-instrumentation-python-0.0.2/src/omegi/util/UtilFunction.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:04:48.000000 omegi-instrumentation-python-0.0.2/src/omegi/util/__init__.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 15:37:06.115491 omegi-instrumentation-python-0.0.2/src/omegi_instrumentation_python.egg-info/
--rw-r--r--   0 whisenlantern   (501) staff       (20)      807 2024-05-16 15:37:06.000000 omegi-instrumentation-python-0.0.2/src/omegi_instrumentation_python.egg-info/PKG-INFO
--rw-r--r--   0 whisenlantern   (501) staff       (20)      771 2024-05-16 15:37:06.000000 omegi-instrumentation-python-0.0.2/src/omegi_instrumentation_python.egg-info/SOURCES.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)        1 2024-05-16 15:37:06.000000 omegi-instrumentation-python-0.0.2/src/omegi_instrumentation_python.egg-info/dependency_links.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)     1151 2024-05-16 15:37:06.000000 omegi-instrumentation-python-0.0.2/src/omegi_instrumentation_python.egg-info/requires.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)        6 2024-05-16 15:37:06.000000 omegi-instrumentation-python-0.0.2/src/omegi_instrumentation_python.egg-info/top_level.txt
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 15:54:58.929813 omegi-instrumentation-python-0.0.3/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      807 2024-05-16 15:54:58.929681 omegi-instrumentation-python-0.0.3/PKG-INFO
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      405 2024-05-16 15:36:10.000000 omegi-instrumentation-python-0.0.3/README.md
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      103 2024-05-07 06:17:54.000000 omegi-instrumentation-python-0.0.3/pyproject.toml
+-rw-r--r--   0 whisenlantern   (501) staff       (20)       38 2024-05-16 15:54:58.929859 omegi-instrumentation-python-0.0.3/setup.cfg
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2436 2024-05-16 15:54:49.000000 omegi-instrumentation-python-0.0.3/setup.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 15:54:58.925119 omegi-instrumentation-python-0.0.3/src/
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 15:54:58.925822 omegi-instrumentation-python-0.0.3/src/omegi/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2949 2024-05-16 15:54:25.000000 omegi-instrumentation-python-0.0.3/src/omegi/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 15:54:58.926389 omegi-instrumentation-python-0.0.3/src/omegi/decorator/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2223 2024-05-14 06:38:33.000000 omegi-instrumentation-python-0.0.3/src/omegi/decorator/OmegiDecorator.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 00:41:28.000000 omegi-instrumentation-python-0.0.3/src/omegi/decorator/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 15:54:58.926906 omegi-instrumentation-python-0.0.3/src/omegi/exporter/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2133 2024-05-16 15:29:55.000000 omegi-instrumentation-python-0.0.3/src/omegi/exporter/OmegiSpanExporter.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 00:41:10.000000 omegi-instrumentation-python-0.0.3/src/omegi/exporter/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 15:54:58.927209 omegi-instrumentation-python-0.0.3/src/omegi/generator/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      299 2024-05-16 15:54:01.000000 omegi-instrumentation-python-0.0.3/src/omegi/generator/OmegiIdGenerator.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-16 07:10:31.000000 omegi-instrumentation-python-0.0.3/src/omegi/generator/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 15:54:58.928817 omegi-instrumentation-python-0.0.3/src/omegi/util/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     1856 2024-05-16 14:38:52.000000 omegi-instrumentation-python-0.0.3/src/omegi/util/OmegiDependencyInstrument.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2646 2024-05-16 15:48:09.000000 omegi-instrumentation-python-0.0.3/src/omegi/util/OmegiErrorSpanFormatter.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      840 2024-05-14 07:24:09.000000 omegi-instrumentation-python-0.0.3/src/omegi/util/OmegiSamplerSpanFormatter.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     1529 2024-05-14 08:52:40.000000 omegi-instrumentation-python-0.0.3/src/omegi/util/OmegiTracingSetup.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      623 2024-05-14 06:53:00.000000 omegi-instrumentation-python-0.0.3/src/omegi/util/UtilFunction.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-14 07:04:48.000000 omegi-instrumentation-python-0.0.3/src/omegi/util/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-16 15:54:58.929472 omegi-instrumentation-python-0.0.3/src/omegi_instrumentation_python.egg-info/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      807 2024-05-16 15:54:58.000000 omegi-instrumentation-python-0.0.3/src/omegi_instrumentation_python.egg-info/PKG-INFO
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      771 2024-05-16 15:54:58.000000 omegi-instrumentation-python-0.0.3/src/omegi_instrumentation_python.egg-info/SOURCES.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        1 2024-05-16 15:54:58.000000 omegi-instrumentation-python-0.0.3/src/omegi_instrumentation_python.egg-info/dependency_links.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     1151 2024-05-16 15:54:58.000000 omegi-instrumentation-python-0.0.3/src/omegi_instrumentation_python.egg-info/requires.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        6 2024-05-16 15:54:58.000000 omegi-instrumentation-python-0.0.3/src/omegi_instrumentation_python.egg-info/top_level.txt
```

### Comparing `omegi-instrumentation-python-0.0.2/PKG-INFO` & `omegi-instrumentation-python-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omegi-instrumentation-python
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python Instrumentation for Automatic Error Logging
 Home-page: https://github.com/TeamOmegi/Instrumentation-Python
 Author: omegi
 Author-email: canon1107@naver.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `omegi-instrumentation-python-0.0.2/setup.py` & `omegi-instrumentation-python-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="omegi-instrumentation-python",
-    version="0.0.2",
+    version="0.0.3",
     author="omegi",
     author_email="canon1107@naver.com",
     description="Python Instrumentation for Automatic Error Logging",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TeamOmegi/Instrumentation-Python",
     classifiers=[
```

### Comparing `omegi-instrumentation-python-0.0.2/src/omegi/__init__.py` & `omegi-instrumentation-python-0.0.3/src/omegi/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from opentelemetry.instrumentation.utils import unwrap
 from opentelemetry.sdk.resources import Resource
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import BatchSpanProcessor, ConsoleSpanExporter
 from opentelemetry.trace.propagation.tracecontext import TraceContextTextMapPropagator
 
 from .exporter.OmegiSpanExporter import OmegiKafkaSpanExporter
+from .generator.OmegiIdGenerator import HexIdGenerator
 from .util.OmegiDependencyInstrument import instrument_dependencies
 from .util.OmegiTracingSetup import wrap_functions
 
 
 class OmegiInstrumentor(BaseInstrumentor):
     def __init__(self, app=None):
         self.app = app
@@ -42,14 +43,15 @@
             logging.error("Please set Project root")
         # Setup Propagator, Custom Exporter, SpanProcessor
         propagator = TraceContextTextMapPropagator()
         propagate.set_global_textmap(propagator)
         span_processor = BatchSpanProcessor(self._set_exporter())
         trace.set_tracer_provider(TracerProvider(
             resource=Resource.create({"service.name": os.getenv("OMEGI_SERVICE_NAME", 'test-server')}),
+            id_generator=HexIdGenerator()
         ))
         trace.get_tracer_provider().add_span_processor(span_processor)
         tracer = trace.get_tracer(__name__)
         # Setup Instrumentation
         if self.app is not None:
             self._start_depending_instrumentation(app=self.app)
         # Setup Tracing Functions
```

### Comparing `omegi-instrumentation-python-0.0.2/src/omegi/decorator/OmegiDecorator.py` & `omegi-instrumentation-python-0.0.3/src/omegi/decorator/OmegiDecorator.py`

 * *Files identical despite different names*

### Comparing `omegi-instrumentation-python-0.0.2/src/omegi/exporter/OmegiSpanExporter.py` & `omegi-instrumentation-python-0.0.3/src/omegi/exporter/OmegiSpanExporter.py`

 * *Files identical despite different names*

### Comparing `omegi-instrumentation-python-0.0.2/src/omegi/util/OmegiDependencyInstrument.py` & `omegi-instrumentation-python-0.0.3/src/omegi/util/OmegiDependencyInstrument.py`

 * *Files identical despite different names*

### Comparing `omegi-instrumentation-python-0.0.2/src/omegi/util/OmegiErrorSpanFormatter.py` & `omegi-instrumentation-python-0.0.3/src/omegi/util/OmegiErrorSpanFormatter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Sequence
 
-from opentelemetry.trace import Span
+from opentelemetry.trace import Span, SpanKind
 
 from .UtilFunction import convert_nanoseconds_to_string
 
 
 def format_error_spans(origin_spans: Sequence[Span], token):
     data = {}
     error = {}
@@ -31,15 +31,15 @@
     data["serviceName"] = origin_spans[0].resource.attributes["service.name"]
     data["error"] = error
     data["spans"] = spans
     return data
 
 
 def _figure_internal_error(origin_spans: Sequence[Span]) -> bool:
-    if origin_spans[len(origin_spans) - 1].kind.name != "INTERNAL":
+    if origin_spans[len(origin_spans) - 1].kind.name != SpanKind.INTERNAL.value:
         return False
     return True
 
 
 def _extract_exception_flow(stack_trace):
     flow_steps = {}
     error_stack = []
```

### Comparing `omegi-instrumentation-python-0.0.2/src/omegi/util/OmegiSamplerSpanFormatter.py` & `omegi-instrumentation-python-0.0.3/src/omegi/util/OmegiSamplerSpanFormatter.py`

 * *Files identical despite different names*

### Comparing `omegi-instrumentation-python-0.0.2/src/omegi/util/OmegiTracingSetup.py` & `omegi-instrumentation-python-0.0.3/src/omegi/util/OmegiTracingSetup.py`

 * *Files identical despite different names*

### Comparing `omegi-instrumentation-python-0.0.2/src/omegi/util/UtilFunction.py` & `omegi-instrumentation-python-0.0.3/src/omegi/util/UtilFunction.py`

 * *Files identical despite different names*

### Comparing `omegi-instrumentation-python-0.0.2/src/omegi_instrumentation_python.egg-info/PKG-INFO` & `omegi-instrumentation-python-0.0.3/src/omegi_instrumentation_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omegi-instrumentation-python
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python Instrumentation for Automatic Error Logging
 Home-page: https://github.com/TeamOmegi/Instrumentation-Python
 Author: omegi
 Author-email: canon1107@naver.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `omegi-instrumentation-python-0.0.2/src/omegi_instrumentation_python.egg-info/SOURCES.txt` & `omegi-instrumentation-python-0.0.3/src/omegi_instrumentation_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `omegi-instrumentation-python-0.0.2/src/omegi_instrumentation_python.egg-info/requires.txt` & `omegi-instrumentation-python-0.0.3/src/omegi_instrumentation_python.egg-info/requires.txt`

 * *Files identical despite different names*

