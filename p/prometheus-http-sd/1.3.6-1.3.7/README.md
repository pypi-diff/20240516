# Comparing `tmp/prometheus_http_sd-1.3.6.tar.gz` & `tmp/prometheus_http_sd-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prometheus_http_sd-1.3.6.tar", max compression
+gzip compressed data, was "prometheus_http_sd-1.3.7.tar", max compression
```

## Comparing `prometheus_http_sd-1.3.6.tar` & `prometheus_http_sd-1.3.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2023-11-28 09:15:11.625856 prometheus_http_sd-1.3.6/LICENSE
--rw-r--r--   0        0        0    14321 2023-11-28 09:15:11.625856 prometheus_http_sd-1.3.6/README.md
--rw-r--r--   0        0        0        0 2023-11-28 09:15:11.629856 prometheus_http_sd-1.3.6/prometheus_http_sd/__init__.py
--rw-r--r--   0        0        0     3605 2023-11-28 09:15:11.629856 prometheus_http_sd-1.3.6/prometheus_http_sd/app.py
--rw-r--r--   0        0        0     4192 2023-11-28 09:15:11.629856 prometheus_http_sd-1.3.6/prometheus_http_sd/cli.py
--rw-r--r--   0        0        0      110 2023-11-28 09:15:11.629856 prometheus_http_sd-1.3.6/prometheus_http_sd/config.py
--rw-r--r--   0        0        0       45 2023-11-28 09:15:11.629856 prometheus_http_sd-1.3.6/prometheus_http_sd/const.py
--rw-r--r--   0        0        0    12848 2023-11-28 09:15:11.629856 prometheus_http_sd-1.3.6/prometheus_http_sd/decorator.py
--rw-r--r--   0        0        0        0 2023-11-28 09:15:11.629856 prometheus_http_sd-1.3.6/prometheus_http_sd/exceptions.py
--rw-r--r--   0        0        0     1165 2023-11-28 09:15:11.629856 prometheus_http_sd-1.3.6/prometheus_http_sd/mem_perf.py
--rw-r--r--   0        0        0     4944 2023-11-28 09:15:11.629856 prometheus_http_sd-1.3.6/prometheus_http_sd/sd.py
--rw-r--r--   0        0        0      147 2023-11-28 09:15:11.629856 prometheus_http_sd-1.3.6/prometheus_http_sd/targets.py
--rw-r--r--   0        0        0     1148 2023-11-28 09:15:11.629856 prometheus_http_sd-1.3.6/prometheus_http_sd/templates/admin.html
--rw-r--r--   0        0        0     2261 2023-11-28 09:15:11.629856 prometheus_http_sd-1.3.6/prometheus_http_sd/validate.py
--rw-r--r--   0        0        0       18 2023-11-28 09:15:11.629856 prometheus_http_sd-1.3.6/prometheus_http_sd/version.py
--rw-r--r--   0        0        0      703 2023-11-28 09:15:11.629856 prometheus_http_sd-1.3.6/pyproject.toml
--rw-r--r--   0        0        0    15192 1970-01-01 00:00:00.000000 prometheus_http_sd-1.3.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-01-05 04:18:35.405326 prometheus_http_sd-1.3.7/LICENSE
+-rw-r--r--   0        0        0    14321 2024-01-05 04:18:35.405326 prometheus_http_sd-1.3.7/README.md
+-rw-r--r--   0        0        0        0 2024-01-05 04:18:35.409326 prometheus_http_sd-1.3.7/prometheus_http_sd/__init__.py
+-rw-r--r--   0        0        0     3605 2024-01-05 04:18:35.409326 prometheus_http_sd-1.3.7/prometheus_http_sd/app.py
+-rw-r--r--   0        0        0     4192 2024-01-05 04:18:35.409326 prometheus_http_sd-1.3.7/prometheus_http_sd/cli.py
+-rw-r--r--   0        0        0      110 2024-01-05 04:18:35.409326 prometheus_http_sd-1.3.7/prometheus_http_sd/config.py
+-rw-r--r--   0        0        0       45 2024-01-05 04:18:35.409326 prometheus_http_sd-1.3.7/prometheus_http_sd/const.py
+-rw-r--r--   0        0        0    12848 2024-01-05 04:18:35.409326 prometheus_http_sd-1.3.7/prometheus_http_sd/decorator.py
+-rw-r--r--   0        0        0        0 2024-01-05 04:18:35.409326 prometheus_http_sd-1.3.7/prometheus_http_sd/exceptions.py
+-rw-r--r--   0        0        0     1165 2024-01-05 04:18:35.409326 prometheus_http_sd-1.3.7/prometheus_http_sd/mem_perf.py
+-rw-r--r--   0        0        0     4851 2024-01-05 04:18:35.409326 prometheus_http_sd-1.3.7/prometheus_http_sd/sd.py
+-rw-r--r--   0        0        0      147 2024-01-05 04:18:35.409326 prometheus_http_sd-1.3.7/prometheus_http_sd/targets.py
+-rw-r--r--   0        0        0     1148 2024-01-05 04:18:35.409326 prometheus_http_sd-1.3.7/prometheus_http_sd/templates/admin.html
+-rw-r--r--   0        0        0     2261 2024-01-05 04:18:35.409326 prometheus_http_sd-1.3.7/prometheus_http_sd/validate.py
+-rw-r--r--   0        0        0       18 2024-01-05 04:18:35.409326 prometheus_http_sd-1.3.7/prometheus_http_sd/version.py
+-rw-r--r--   0        0        0      703 2024-01-05 04:18:35.409326 prometheus_http_sd-1.3.7/pyproject.toml
+-rw-r--r--   0        0        0    15192 1970-01-01 00:00:00.000000 prometheus_http_sd-1.3.7/PKG-INFO
```

### Comparing `prometheus_http_sd-1.3.6/LICENSE` & `prometheus_http_sd-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.3.6/README.md` & `prometheus_http_sd-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.3.6/prometheus_http_sd/app.py` & `prometheus_http_sd-1.3.7/prometheus_http_sd/app.py`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.3.6/prometheus_http_sd/cli.py` & `prometheus_http_sd-1.3.7/prometheus_http_sd/cli.py`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.3.6/prometheus_http_sd/decorator.py` & `prometheus_http_sd-1.3.7/prometheus_http_sd/decorator.py`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.3.6/prometheus_http_sd/mem_perf.py` & `prometheus_http_sd-1.3.7/prometheus_http_sd/mem_perf.py`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.3.6/prometheus_http_sd/sd.py` & `prometheus_http_sd-1.3.7/prometheus_http_sd/sd.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,35 +37,32 @@
 generator_run_duration_seconds = Histogram(
     "httpsd_generator_run_duration_seconds",
     "The time cost that this generator run",
     ["generator"],
 )
 
 
-def should_ignore(file, full_path, ignore_dirs):
+def should_ignore(full_path, ignore_dirs):
     if ignore_dirs:
         for ignore in ignore_dirs:
             if full_path.startswith(ignore):
                 logger.warning(
                     f"{full_path} is ignored due to match ignore"
                     f" pattern {ignore}"
                 )
                 return True
 
-    should_ignore_underscore = any(
-        p.startswith("_") for p in os.path.normpath(full_path).split(os.sep)
+    should_ignore_this = any(
+        p.startswith("_") or p.startswith(".")
+        for p in os.path.normpath(full_path).split(os.sep)
     )
 
-    if should_ignore_underscore:
+    if should_ignore_this:
         return True
 
-    should_ignore_hidden = file.startswith(".")
-
-    if should_ignore_hidden:
-        return True
     return False
 
 
 def get_generator_list(
     root: str, path: str = "", ignore_dirs=None
 ) -> List[str]:
     """
@@ -82,15 +79,15 @@
     if not Path(root).exists():
         raise FileNotFoundError(f"{root} not exist!")
 
     for root, _, files in os.walk(root):
         for file in files:
             full_path = os.path.join(root, file)
 
-            ignore = should_ignore(file, full_path, ignore_dirs)
+            ignore = should_ignore(full_path, ignore_dirs)
             logger.info(f"{file=}, ignore={ignore}")
             if ignore:
                 continue
 
             generators.append(full_path)
 
     logger.debug(f"{generators=}")
```

### Comparing `prometheus_http_sd-1.3.6/prometheus_http_sd/templates/admin.html` & `prometheus_http_sd-1.3.7/prometheus_http_sd/templates/admin.html`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.3.6/prometheus_http_sd/validate.py` & `prometheus_http_sd-1.3.7/prometheus_http_sd/validate.py`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.3.6/pyproject.toml` & `prometheus_http_sd-1.3.7/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prometheus-http-sd"
-version = "1.3.6"
+version = "1.3.7"
 description = "Prometheus HTTP SD framework."
 authors = ["laixintao <laixintaoo@gmail.com>"]
 readme = 'README.md'
 homepage = "https://python-poetry.org://github.com/laixintao/prometheus-http-sd"
 
 
 [tool.poetry.dependencies]
@@ -16,15 +16,15 @@
 sentry-sdk = {extras = ["flask"], version = "^1.37.1"}
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 flake8 = "^4.0.1"
 
 [build-system]
-requires = ["poetry-core>=1.3.6"]
+requires = ["poetry-core>=1.3.7"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 79
 
 [tool.poetry.scripts]
 prometheus-http-sd = 'prometheus_http_sd.cli:main'
```

### Comparing `prometheus_http_sd-1.3.6/PKG-INFO` & `prometheus_http_sd-1.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prometheus-http-sd
-Version: 1.3.6
+Version: 1.3.7
 Summary: Prometheus HTTP SD framework.
 Home-page: https://python-poetry.org://github.com/laixintao/prometheus-http-sd
 Author: laixintao
 Author-email: laixintaoo@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

