# Comparing `tmp/dp-launching-app-0.0.3.tar.gz` & `tmp/dp-launching-app-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dp-launching-app-0.0.3.tar", last modified: Sat May 11 07:01:13 2024, max compression
+gzip compressed data, was "dp-launching-app-0.0.4.tar", last modified: Thu May 16 07:07:45 2024, max compression
```

## Comparing `dp-launching-app-0.0.3.tar` & `dp-launching-app-0.0.4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-11 07:01:13.671463 dp-launching-app-0.0.3/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)       94 2024-05-10 07:03:20.000000 dp-launching-app-0.0.3/MANIFEST.in
--rw-r--r--   0 xiongyanfei   (502) staff       (20)      156 2024-05-11 07:01:13.671305 dp-launching-app-0.0.3/PKG-INFO
--rw-r--r--   0 xiongyanfei   (502) staff       (20)        0 2024-05-10 07:03:20.000000 dp-launching-app-0.0.3/README.md
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-11 07:01:13.662600 dp-launching-app-0.0.3/dp/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)      154 2024-05-10 07:03:20.000000 dp-launching-app-0.0.3/dp/__init__.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-11 07:01:13.663016 dp-launching-app-0.0.3/dp/launching/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)       22 2024-05-10 07:03:20.000000 dp-launching-app-0.0.3/dp/launching/__init__.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-11 07:01:13.663453 dp-launching-app-0.0.3/dp/launching/cli/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)    12636 2024-05-10 07:03:20.000000 dp-launching-app-0.0.3/dp/launching/cli/__init__.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-11 07:01:13.664445 dp-launching-app-0.0.3/dp/launching/cli/api/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)        0 2024-05-10 07:03:20.000000 dp-launching-app-0.0.3/dp/launching/cli/api/__init__.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)    21712 2024-05-10 07:03:20.000000 dp-launching-app-0.0.3/dp/launching/cli/api/model.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     5386 2024-05-10 07:03:20.000000 dp-launching-app-0.0.3/dp/launching/cli/api/persistent_service.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-11 07:01:13.664992 dp-launching-app-0.0.3/dp/launching/cli/commands/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)        0 2024-05-10 07:03:20.000000 dp-launching-app-0.0.3/dp/launching/cli/commands/__init__.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     1315 2024-05-10 07:03:20.000000 dp-launching-app-0.0.3/dp/launching/cli/commands/launching.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-11 07:01:13.661115 dp-launching-app-0.0.3/dp/launching/cli/commands/scaffold/
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-11 07:01:13.665329 dp-launching-app-0.0.3/dp/launching/cli/commands/scaffold/basic/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     1858 2024-05-10 07:03:20.000000 dp-launching-app-0.0.3/dp/launching/cli/commands/scaffold/basic/basic.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-11 07:01:13.665556 dp-launching-app-0.0.3/dp/launching/cli/commands/scaffold/bohrium/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     2595 2024-05-10 07:03:20.000000 dp-launching-app-0.0.3/dp/launching/cli/commands/scaffold/bohrium/bohrium.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-11 07:01:13.665787 dp-launching-app-0.0.3/dp/launching/cli/commands/scaffold/dflow/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     2606 2024-05-10 07:03:20.000000 dp-launching-app-0.0.3/dp/launching/cli/commands/scaffold/dflow/dflow.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-11 07:01:13.666305 dp-launching-app-0.0.3/dp/launching/cli/utils/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)        0 2024-05-10 07:03:20.000000 dp-launching-app-0.0.3/dp/launching/cli/utils/__init__.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)      147 2024-05-10 07:03:20.000000 dp-launching-app-0.0.3/dp/launching/cli/utils/random.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-11 07:01:13.666638 dp-launching-app-0.0.3/dp/launching/report/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     2940 2024-05-10 07:03:20.000000 dp-launching-app-0.0.3/dp/launching/report/__init__.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-11 07:01:13.668757 dp-launching-app-0.0.3/dp/launching/typing/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)      175 2024-05-10 07:03:20.000000 dp-launching-app-0.0.3/dp/launching/typing/__init__.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-11 07:01:13.669628 dp-launching-app-0.0.3/dp/launching/typing/addon/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)        0 2024-05-10 07:03:20.000000 dp-launching-app-0.0.3/dp/launching/typing/addon/__init__.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)      867 2024-05-10 07:03:20.000000 dp-launching-app-0.0.3/dp/launching/typing/addon/sysmbol.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     6866 2024-05-10 07:03:20.000000 dp-launching-app-0.0.3/dp/launching/typing/addon/ui.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     7379 2024-05-11 02:54:01.000000 dp-launching-app-0.0.3/dp/launching/typing/basic.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)      749 2024-05-10 07:03:20.000000 dp-launching-app-0.0.3/dp/launching/typing/benchmark.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     1774 2024-05-10 07:03:20.000000 dp-launching-app-0.0.3/dp/launching/typing/bio.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     9731 2024-05-10 07:03:20.000000 dp-launching-app-0.0.3/dp/launching/typing/bohrium.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     4908 2024-05-10 07:03:20.000000 dp-launching-app-0.0.3/dp/launching/typing/dflow.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     6371 2024-05-10 07:03:20.000000 dp-launching-app-0.0.3/dp/launching/typing/io.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-11 07:01:13.671076 dp-launching-app-0.0.3/dp_launching_app.egg-info/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)      156 2024-05-11 07:01:13.000000 dp-launching-app-0.0.3/dp_launching_app.egg-info/PKG-INFO
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     1092 2024-05-11 07:01:13.000000 dp-launching-app-0.0.3/dp_launching_app.egg-info/SOURCES.txt
--rw-r--r--   0 xiongyanfei   (502) staff       (20)        1 2024-05-11 07:01:13.000000 dp-launching-app-0.0.3/dp_launching_app.egg-info/dependency_links.txt
--rw-r--r--   0 xiongyanfei   (502) staff       (20)       75 2024-05-11 07:01:13.000000 dp-launching-app-0.0.3/dp_launching_app.egg-info/entry_points.txt
--rw-r--r--   0 xiongyanfei   (502) staff       (20)      108 2024-05-11 07:01:13.000000 dp-launching-app-0.0.3/dp_launching_app.egg-info/requires.txt
--rw-r--r--   0 xiongyanfei   (502) staff       (20)        3 2024-05-11 07:01:13.000000 dp-launching-app-0.0.3/dp_launching_app.egg-info/top_level.txt
--rw-r--r--   0 xiongyanfei   (502) staff       (20)       38 2024-05-11 07:01:13.671499 dp-launching-app-0.0.3/setup.cfg
--rw-r--r--   0 xiongyanfei   (502) staff       (20)      714 2024-05-11 07:00:34.000000 dp-launching-app-0.0.3/setup.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-16 07:07:45.658682 dp-launching-app-0.0.4/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)       94 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/MANIFEST.in
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)      156 2024-05-16 07:07:45.658510 dp-launching-app-0.0.4/PKG-INFO
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)        0 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/README.md
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-16 07:07:45.649754 dp-launching-app-0.0.4/dp/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)      154 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/__init__.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-16 07:07:45.650177 dp-launching-app-0.0.4/dp/launching/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)       22 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/launching/__init__.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-16 07:07:45.650566 dp-launching-app-0.0.4/dp/launching/cli/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)    12682 2024-05-16 07:06:32.000000 dp-launching-app-0.0.4/dp/launching/cli/__init__.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-16 07:07:45.651572 dp-launching-app-0.0.4/dp/launching/cli/api/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)        0 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/launching/cli/api/__init__.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)    21712 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/launching/cli/api/model.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     5386 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/launching/cli/api/persistent_service.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-16 07:07:45.652098 dp-launching-app-0.0.4/dp/launching/cli/commands/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)        0 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/launching/cli/commands/__init__.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     1315 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/launching/cli/commands/launching.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-16 07:07:45.648379 dp-launching-app-0.0.4/dp/launching/cli/commands/scaffold/
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-16 07:07:45.652463 dp-launching-app-0.0.4/dp/launching/cli/commands/scaffold/basic/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     1858 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/launching/cli/commands/scaffold/basic/basic.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-16 07:07:45.652789 dp-launching-app-0.0.4/dp/launching/cli/commands/scaffold/bohrium/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     2595 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/launching/cli/commands/scaffold/bohrium/bohrium.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-16 07:07:45.653083 dp-launching-app-0.0.4/dp/launching/cli/commands/scaffold/dflow/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     2606 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/launching/cli/commands/scaffold/dflow/dflow.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-16 07:07:45.653660 dp-launching-app-0.0.4/dp/launching/cli/utils/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)        0 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/launching/cli/utils/__init__.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)      147 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/launching/cli/utils/random.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-16 07:07:45.653942 dp-launching-app-0.0.4/dp/launching/report/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     2940 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/launching/report/__init__.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-16 07:07:45.655905 dp-launching-app-0.0.4/dp/launching/typing/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)      175 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/launching/typing/__init__.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-16 07:07:45.656746 dp-launching-app-0.0.4/dp/launching/typing/addon/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)        0 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/launching/typing/addon/__init__.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)      867 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/launching/typing/addon/sysmbol.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     6866 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/launching/typing/addon/ui.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     7379 2024-05-11 02:54:01.000000 dp-launching-app-0.0.4/dp/launching/typing/basic.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)      749 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/launching/typing/benchmark.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     1774 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/launching/typing/bio.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     9731 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/launching/typing/bohrium.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     4908 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/launching/typing/dflow.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     6371 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/launching/typing/io.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-16 07:07:45.658292 dp-launching-app-0.0.4/dp_launching_app.egg-info/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)      156 2024-05-16 07:07:45.000000 dp-launching-app-0.0.4/dp_launching_app.egg-info/PKG-INFO
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     1092 2024-05-16 07:07:45.000000 dp-launching-app-0.0.4/dp_launching_app.egg-info/SOURCES.txt
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)        1 2024-05-16 07:07:45.000000 dp-launching-app-0.0.4/dp_launching_app.egg-info/dependency_links.txt
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)       75 2024-05-16 07:07:45.000000 dp-launching-app-0.0.4/dp_launching_app.egg-info/entry_points.txt
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)      108 2024-05-16 07:07:45.000000 dp-launching-app-0.0.4/dp_launching_app.egg-info/requires.txt
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)        3 2024-05-16 07:07:45.000000 dp-launching-app-0.0.4/dp_launching_app.egg-info/top_level.txt
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)       38 2024-05-16 07:07:45.658720 dp-launching-app-0.0.4/setup.cfg
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)      714 2024-05-16 07:06:59.000000 dp-launching-app-0.0.4/setup.py
```

### Comparing `dp-launching-app-0.0.3/dp/launching/cli/__init__.py` & `dp-launching-app-0.0.4/dp/launching/cli/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -337,10 +337,10 @@
             elif isinstance(value, BaseModel):
                 res.update({value.__name__: value})
             elif isinstance(value, SubParser):
                 value.model_class.description = value.description or ""
                 value.documentation = get_doc(value.model_class)
                 res.update({key+"_inputs": value.model_class})
                 # 添加outputOptions
-                if value.outputOptions:
+                if hasattr(self, "outputOptions") and self.outputOptions is not None:
                     res.update({key+"_outputs": value.outputOptions})
         return res
```

### Comparing `dp-launching-app-0.0.3/dp/launching/cli/api/model.py` & `dp-launching-app-0.0.4/dp/launching/cli/api/model.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.3/dp/launching/cli/api/persistent_service.py` & `dp-launching-app-0.0.4/dp/launching/cli/api/persistent_service.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.3/dp/launching/cli/commands/launching.py` & `dp-launching-app-0.0.4/dp/launching/cli/commands/launching.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.3/dp/launching/cli/commands/scaffold/basic/basic.py` & `dp-launching-app-0.0.4/dp/launching/cli/commands/scaffold/basic/basic.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.3/dp/launching/cli/commands/scaffold/bohrium/bohrium.py` & `dp-launching-app-0.0.4/dp/launching/cli/commands/scaffold/bohrium/bohrium.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.3/dp/launching/cli/commands/scaffold/dflow/dflow.py` & `dp-launching-app-0.0.4/dp/launching/cli/commands/scaffold/dflow/dflow.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.3/dp/launching/report/__init__.py` & `dp-launching-app-0.0.4/dp/launching/report/__init__.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.3/dp/launching/typing/addon/sysmbol.py` & `dp-launching-app-0.0.4/dp/launching/typing/addon/sysmbol.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.3/dp/launching/typing/addon/ui.py` & `dp-launching-app-0.0.4/dp/launching/typing/addon/ui.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.3/dp/launching/typing/basic.py` & `dp-launching-app-0.0.4/dp/launching/typing/basic.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.3/dp/launching/typing/benchmark.py` & `dp-launching-app-0.0.4/dp/launching/typing/benchmark.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.3/dp/launching/typing/bio.py` & `dp-launching-app-0.0.4/dp/launching/typing/bio.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.3/dp/launching/typing/bohrium.py` & `dp-launching-app-0.0.4/dp/launching/typing/bohrium.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.3/dp/launching/typing/dflow.py` & `dp-launching-app-0.0.4/dp/launching/typing/dflow.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.3/dp/launching/typing/io.py` & `dp-launching-app-0.0.4/dp/launching/typing/io.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.3/dp_launching_app.egg-info/SOURCES.txt` & `dp-launching-app-0.0.4/dp_launching_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.3/setup.py` & `dp-launching-app-0.0.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="dp-launching-app",
-    version="0.0.3",
+    version="0.0.4",
     author="",
     author_email="",
     description="",
     long_description="",
     long_description_content_type="text/plain",
     url="",
     entry_points={
```

