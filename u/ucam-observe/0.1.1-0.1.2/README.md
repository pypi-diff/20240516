# Comparing `tmp/ucam_observe-0.1.1.tar.gz` & `tmp/ucam_observe-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ucam_observe-0.1.1.tar", max compression
+gzip compressed data, was "ucam_observe-0.1.2.tar", max compression
```

## Comparing `ucam_observe-0.1.1.tar` & `ucam_observe-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1925 2024-05-15 14:43:37.018812 ucam_observe-0.1.1/README.md
--rw-r--r--   0        0        0     1927 2024-05-13 16:36:11.958575 ucam_observe-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      205 2024-05-07 11:21:09.924321 ucam_observe-0.1.1/ucam_observe/__init__.py
--rw-r--r--   0        0        0      243 2024-05-02 18:28:36.651015 ucam_observe-0.1.1/ucam_observe/django.py
--rw-r--r--   0        0        0     1382 2024-05-15 14:43:37.018812 ucam_observe-0.1.1/ucam_observe/logging_config.py
--rw-r--r--   0        0        0     2682 1970-01-01 00:00:00.000000 ucam_observe-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2718 2024-05-15 16:08:39.433980 ucam_observe-0.1.2/README.md
+-rw-r--r--   0        0        0     1927 2024-05-15 15:58:01.609349 ucam_observe-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      205 2024-05-15 15:58:01.609349 ucam_observe-0.1.2/ucam_observe/__init__.py
+-rw-r--r--   0        0        0      243 2024-05-15 15:58:01.609349 ucam_observe-0.1.2/ucam_observe/django.py
+-rw-r--r--   0        0        0     2064 2024-05-15 15:58:01.609349 ucam_observe-0.1.2/ucam_observe/logging_config.py
+-rw-r--r--   0        0        0     3475 1970-01-01 00:00:00.000000 ucam_observe-0.1.2/PKG-INFO
```

### Comparing `ucam_observe-0.1.1/README.md` & `ucam_observe-0.1.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -39,14 +39,46 @@
 In the root of your project, create/amend a gunicorn.conf.py. Add the following code to the file.
 
 ```py
 from ucam_observe.gunicorn_conf import configure_logging
 configure_logging()
 ```
 
+### Environment Configuration
+
+#### Log Level
+
+Set the `LOG_LEVEL` environment variable to control the logging level (e.g., DEBUG, INFO, WARNING, ERROR, CRITICAL). This setting adjusts the verbosity of the log outputs:
+
+```bash
+export LOG_LEVEL=DEBUG
+```
+
+#### Console Logging
+
+Set the `CONSOLE_LOGGING` environment variable to control whether logs should be output in a console-friendly format. Set it to `True` to use console-friendly formatting:
+
+```bash
+export CONSOLE_LOGGING=True
+```
+
+### Example Docker Compose Configuration
+
+When using Docker Compose for local development, you can set the environment variables in your `docker-compose.yml` file:
+
+```yaml
+version: '3.8'
+services:
+  your_service:
+    build: .
+    environment:
+      - LOG_LEVEL=DEBUG
+      - CONSOLE_LOGGING=True
+```
+
 ## Developer quickstart
 
 Firstly, [install docker-compose](https://docs.docker.com/compose/install/).
 Install poethepoet
 ```bash
 pip install poethepoet
 ```
```

### Comparing `ucam_observe-0.1.1/pyproject.toml` & `ucam_observe-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ucam_observe"
-version = "0.1.1"
+version = "0.1.2"
 description = "Python library to aid consistent configuration of logging, metrics (future) and tracing (further in future). Packaging and wiring existing open tooling to work effortlessly on UIS DevOps managed cloud infrastructure."
 license = "MIT"
 readme = "README.md"
 authors = []
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `ucam_observe-0.1.1/ucam_observe/logging_config.py` & `ucam_observe-0.1.2/ucam_observe/logging_config.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,44 +5,61 @@
 
 
 def get_log_level():
     """Retrieve log level from environment variables."""
     return os.getenv("LOG_LEVEL", "INFO").upper()
 
 
+def get_console_logging_status():
+    """Retrieve console logging status from environment variables."""
+    return os.getenv("CONSOLE_LOGGING", "False").lower() in ("true", "1")
+
+
 def configure_logging():
     """Configure structured logging for both Python logging and structlog."""
-    log_level = get_log_level()
-
-    base_formatter = {
-        "()": "structlog.stdlib.ProcessorFormatter",
-        "processor": structlog.processors.JSONRenderer(),
-    }
 
     structlog.configure(
         processors=[
             structlog.stdlib.add_logger_name,
+            structlog.stdlib.filter_by_level,
             structlog.stdlib.add_log_level,
             structlog.processors.TimeStamper(fmt="iso"),
             structlog.stdlib.render_to_log_kwargs,
-            structlog.processors.JSONRenderer(),
+            structlog.stdlib.ProcessorFormatter.wrap_for_formatter,
         ],
-        context_class=dict,
         logger_factory=structlog.stdlib.LoggerFactory(),
-        wrapper_class=structlog.stdlib.BoundLogger,
         cache_logger_on_first_use=True,
     )
 
     dictConfig(
         {
             "version": 1,
-            "formatters": {"json": base_formatter},
-            "handlers": {"console": {"class": "logging.StreamHandler", "formatter": "json"}},
+            "disable_existing_loggers": True,
+            "formatters": {
+                "console": {
+                    "()": "structlog.stdlib.ProcessorFormatter",
+                    "processor": structlog.dev.ConsoleRenderer(colors=True),
+                },
+                "json": {
+                    "()": "structlog.stdlib.ProcessorFormatter",
+                    "processor": structlog.processors.JSONRenderer(),
+                },
+            },
+            "handlers": {
+                "console": {
+                    "class": "logging.StreamHandler",
+                    "formatter": "console",
+                },
+                "json": {
+                    "class": "logging.StreamHandler",
+                    "formatter": "json",
+                },
+            },
             "loggers": {
                 "": {
-                    "handlers": ["console"],
-                    "level": log_level,
+                    "handlers": ["console" if get_console_logging_status() else "json"],
+                    "level": get_log_level(),
                     "propagate": True,
                 },
             },
         }
     )
```

### Comparing `ucam_observe-0.1.1/PKG-INFO` & `ucam_observe-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ucam_observe
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python library to aid consistent configuration of logging, metrics (future) and tracing (further in future). Packaging and wiring existing open tooling to work effortlessly on UIS DevOps managed cloud infrastructure.
 License: MIT
 Requires-Python: >=3.9.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -55,14 +55,46 @@
 In the root of your project, create/amend a gunicorn.conf.py. Add the following code to the file.
 
 ```py
 from ucam_observe.gunicorn_conf import configure_logging
 configure_logging()
 ```
 
+### Environment Configuration
+
+#### Log Level
+
+Set the `LOG_LEVEL` environment variable to control the logging level (e.g., DEBUG, INFO, WARNING, ERROR, CRITICAL). This setting adjusts the verbosity of the log outputs:
+
+```bash
+export LOG_LEVEL=DEBUG
+```
+
+#### Console Logging
+
+Set the `CONSOLE_LOGGING` environment variable to control whether logs should be output in a console-friendly format. Set it to `True` to use console-friendly formatting:
+
+```bash
+export CONSOLE_LOGGING=True
+```
+
+### Example Docker Compose Configuration
+
+When using Docker Compose for local development, you can set the environment variables in your `docker-compose.yml` file:
+
+```yaml
+version: '3.8'
+services:
+  your_service:
+    build: .
+    environment:
+      - LOG_LEVEL=DEBUG
+      - CONSOLE_LOGGING=True
+```
+
 ## Developer quickstart
 
 Firstly, [install docker-compose](https://docs.docker.com/compose/install/).
 Install poethepoet
 ```bash
 pip install poethepoet
 ```
```

