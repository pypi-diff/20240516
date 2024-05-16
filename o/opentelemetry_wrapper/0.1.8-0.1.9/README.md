# Comparing `tmp/opentelemetry_wrapper-0.1.8.tar.gz` & `tmp/opentelemetry_wrapper-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentelemetry_wrapper-0.1.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "opentelemetry_wrapper-0.1.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `opentelemetry_wrapper-0.1.8.tar` & `opentelemetry_wrapper-0.1.9.tar`

### file list

```diff
@@ -1,37 +1,38 @@
--rw-r--r--   0        0        0     2311 2022-12-13 07:19:54.176205 opentelemetry_wrapper-0.1.8/.gitignore
--rw-r--r--   0        0        0     9229 2022-12-13 07:19:54.177203 opentelemetry_wrapper-0.1.8/LICENSE
--rw-r--r--   0        0        0     9233 2024-04-08 08:23:00.044355 opentelemetry_wrapper-0.1.8/README.md
--rw-r--r--   0        0        0     3868 2024-04-08 10:04:05.057403 opentelemetry_wrapper-0.1.8/TODO.md
--rw-r--r--   0        0        0       60 2022-12-13 07:19:54.179199 opentelemetry_wrapper-0.1.8/aaaa/bbbb.py
--rw-r--r--   0        0        0     3264 2024-04-08 01:44:30.035164 opentelemetry_wrapper-0.1.8/experiment_otel_logging.py
--rw-r--r--   0        0        0     2834 2024-04-08 10:31:54.524507 opentelemetry_wrapper-0.1.8/fastapi_main.py
--rw-r--r--   0        0        0     1181 2024-04-05 09:25:30.071466 opentelemetry_wrapper-0.1.8/log_weird_things.py
--rw-r--r--   0        0        0     2646 2024-04-05 08:52:10.474665 opentelemetry_wrapper-0.1.8/next_version_intended_usage.py
--rw-r--r--   0        0        0     2093 2024-04-08 10:34:21.599201 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/__init__.py
--rw-r--r--   0        0        0     3652 2023-06-05 02:58:25.364476 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/config/otel_exporter_otlp.py
--rw-r--r--   0        0        0     1260 2023-10-02 06:53:40.662583 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/config/otel_header_attributes.py
--rw-r--r--   0        0        0     2397 2024-04-08 10:00:58.967436 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/config/otel_headers.py
--rw-r--r--   0        0        0     1359 2022-12-13 07:19:54.183188 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/config/otel_log_level.py
--rw-r--r--   0        0        0     6154 2022-12-14 06:49:31.121402 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/config/otel_service_name.py
--rw-r--r--   0        0        0      507 2024-04-08 10:01:06.853687 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/config/otel_wrapper_prometheus_exporter.py
--rw-r--r--   0        0        0      270 2024-03-13 02:40:51.157859 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/dependencies/fastapi/fastapi_typedef.py
--rw-r--r--   0        0        0     1275 2024-04-08 10:12:38.034849 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/dependencies/fastapi/starlette_request_hook.py
--rw-r--r--   0        0        0     1310 2022-12-14 06:03:08.846216 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/dependencies/opentelemetry/instrument_dataclasses.py
--rw-r--r--   0        0        0     9850 2024-04-05 10:17:45.422050 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/dependencies/opentelemetry/instrument_decorator.py
--rw-r--r--   0        0        0     1908 2024-04-08 10:00:04.336638 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/dependencies/opentelemetry/instrument_fastapi.py
--rw-r--r--   0        0        0     6271 2024-04-08 01:55:33.344141 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/dependencies/opentelemetry/instrument_logging.py
--rw-r--r--   0        0        0      784 2024-03-13 09:44:08.327016 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/dependencies/opentelemetry/instrument_requests.py
--rw-r--r--   0        0        0     3534 2024-03-13 09:44:08.280147 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/dependencies/opentelemetry/instrument_sqlalchemy.py
--rw-r--r--   0        0        0     1811 2024-04-08 09:24:04.758627 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/dependencies/opentelemetry/instrument_system_metrics.py
--rw-r--r--   0        0        0     6805 2024-04-08 10:23:45.979425 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/dependencies/opentelemetry/otel_providers.py
--rw-r--r--   0        0        0      153 2022-12-14 03:26:52.894387 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/dependencies/opentelemetry/resource_detector.py
--rw-r--r--   0        0        0     1031 2024-04-08 10:17:28.804459 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/dependencies/sqlalchemy/engine_typedef.py
--rw-r--r--   0        0        0     5363 2024-04-08 10:25:31.283954 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/utils/extract_json_header.py
--rw-r--r--   0        0        0    15005 2024-04-05 10:18:28.473240 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/utils/introspect.py
--rw-r--r--   0        0        0     5184 2024-04-08 10:28:14.050060 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/utils/json_encoder.py
--rw-r--r--   0        0        0     6575 2024-03-13 07:02:29.960397 opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/utils/logging_json_formatter.py
--rw-r--r--   0        0        0     1069 2024-04-08 08:34:14.802204 opentelemetry_wrapper-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      445 2024-04-08 08:34:14.829047 opentelemetry_wrapper-0.1.8/requirements.txt
--rw-r--r--   0        0        0     1639 2024-04-04 06:59:50.663250 opentelemetry_wrapper-0.1.8/setup_otel_logging.py
--rw-r--r--   0        0        0     1016 2024-03-13 01:24:02.712219 opentelemetry_wrapper-0.1.8/sqlalchemy_example.py
--rw-r--r--   0        0        0    10162 1970-01-01 00:00:00.000000 opentelemetry_wrapper-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     2311 2022-12-13 07:19:54.176205 opentelemetry_wrapper-0.1.9/.gitignore
+-rw-r--r--   0        0        0     9229 2022-12-13 07:19:54.177203 opentelemetry_wrapper-0.1.9/LICENSE
+-rw-r--r--   0        0        0    10189 2024-04-09 09:46:37.626083 opentelemetry_wrapper-0.1.9/README.md
+-rw-r--r--   0        0        0     4185 2024-04-09 09:20:26.681641 opentelemetry_wrapper-0.1.9/TODO.md
+-rw-r--r--   0        0        0       60 2022-12-13 07:19:54.179199 opentelemetry_wrapper-0.1.9/aaaa/bbbb.py
+-rw-r--r--   0        0        0     3264 2024-04-09 06:18:58.614613 opentelemetry_wrapper-0.1.9/experiment_otel_logging.py
+-rw-r--r--   0        0        0     2946 2024-04-09 09:29:34.856470 opentelemetry_wrapper-0.1.9/fastapi_main.py
+-rw-r--r--   0        0        0     1183 2024-04-11 09:59:37.985198 opentelemetry_wrapper-0.1.9/log_weird_things.py
+-rw-r--r--   0        0        0     2646 2024-04-05 08:52:10.474665 opentelemetry_wrapper-0.1.9/next_version_intended_usage.py
+-rw-r--r--   0        0        0    32658 2024-04-09 06:37:57.635666 opentelemetry_wrapper-0.1.9/opentelemetry-prometheus-output-example.txt
+-rw-r--r--   0        0        0     1877 2024-04-12 10:02:42.290232 opentelemetry_wrapper-0.1.9/opentelemetry_wrapper/__init__.py
+-rw-r--r--   0        0        0     3652 2023-06-05 02:58:25.364476 opentelemetry_wrapper-0.1.9/opentelemetry_wrapper/config/otel_exporter_otlp.py
+-rw-r--r--   0        0        0     1260 2023-10-02 06:53:40.662583 opentelemetry_wrapper-0.1.9/opentelemetry_wrapper/config/otel_header_attributes.py
+-rw-r--r--   0        0        0     2574 2024-04-09 08:53:09.954024 opentelemetry_wrapper-0.1.9/opentelemetry_wrapper/config/otel_headers.py
+-rw-r--r--   0        0        0     1359 2022-12-13 07:19:54.183188 opentelemetry_wrapper-0.1.9/opentelemetry_wrapper/config/otel_log_level.py
+-rw-r--r--   0        0        0     6154 2022-12-14 06:49:31.121402 opentelemetry_wrapper-0.1.9/opentelemetry_wrapper/config/otel_service_name.py
+-rw-r--r--   0        0        0     1760 2024-04-09 08:40:51.396663 opentelemetry_wrapper-0.1.9/opentelemetry_wrapper/config/otel_wrapper_prometheus_exporter.py
+-rw-r--r--   0        0        0      270 2024-03-13 02:40:51.157859 opentelemetry_wrapper-0.1.9/opentelemetry_wrapper/dependencies/fastapi/fastapi_typedef.py
+-rw-r--r--   0        0        0     1322 2024-04-11 09:34:53.100509 opentelemetry_wrapper-0.1.9/opentelemetry_wrapper/dependencies/fastapi/starlette_request_hook.py
+-rw-r--r--   0        0        0     1310 2022-12-14 06:03:08.846216 opentelemetry_wrapper-0.1.9/opentelemetry_wrapper/dependencies/opentelemetry/instrument_dataclasses.py
+-rw-r--r--   0        0        0     9996 2024-04-11 08:52:19.658494 opentelemetry_wrapper-0.1.9/opentelemetry_wrapper/dependencies/opentelemetry/instrument_decorator.py
+-rw-r--r--   0        0        0     2076 2024-04-09 09:40:28.760664 opentelemetry_wrapper-0.1.9/opentelemetry_wrapper/dependencies/opentelemetry/instrument_fastapi.py
+-rw-r--r--   0        0        0     6271 2024-04-08 01:55:33.344141 opentelemetry_wrapper-0.1.9/opentelemetry_wrapper/dependencies/opentelemetry/instrument_logging.py
+-rw-r--r--   0        0        0     1654 2024-04-11 09:49:27.840818 opentelemetry_wrapper-0.1.9/opentelemetry_wrapper/dependencies/opentelemetry/instrument_requests.py
+-rw-r--r--   0        0        0     3534 2024-03-13 09:44:08.280147 opentelemetry_wrapper-0.1.9/opentelemetry_wrapper/dependencies/opentelemetry/instrument_sqlalchemy.py
+-rw-r--r--   0        0        0      543 2024-04-09 06:23:29.858208 opentelemetry_wrapper-0.1.9/opentelemetry_wrapper/dependencies/opentelemetry/instrument_system_metrics.py
+-rw-r--r--   0        0        0     7095 2024-04-09 09:29:26.670361 opentelemetry_wrapper-0.1.9/opentelemetry_wrapper/dependencies/opentelemetry/otel_providers.py
+-rw-r--r--   0        0        0      153 2022-12-14 03:26:52.894387 opentelemetry_wrapper-0.1.9/opentelemetry_wrapper/dependencies/opentelemetry/resource_detector.py
+-rw-r--r--   0        0        0     1031 2024-04-08 10:17:28.804459 opentelemetry_wrapper-0.1.9/opentelemetry_wrapper/dependencies/sqlalchemy/engine_typedef.py
+-rw-r--r--   0        0        0     5363 2024-04-08 10:25:31.283954 opentelemetry_wrapper-0.1.9/opentelemetry_wrapper/utils/extract_json_header.py
+-rw-r--r--   0        0        0    16641 2024-04-11 08:58:30.219641 opentelemetry_wrapper-0.1.9/opentelemetry_wrapper/utils/introspect.py
+-rw-r--r--   0        0        0     5184 2024-04-08 10:28:14.050060 opentelemetry_wrapper-0.1.9/opentelemetry_wrapper/utils/json_encoder.py
+-rw-r--r--   0        0        0     6575 2024-03-13 07:02:29.960397 opentelemetry_wrapper-0.1.9/opentelemetry_wrapper/utils/logging_json_formatter.py
+-rw-r--r--   0        0        0     1069 2024-04-08 08:34:14.802204 opentelemetry_wrapper-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      445 2024-04-08 08:34:14.829047 opentelemetry_wrapper-0.1.9/requirements.txt
+-rw-r--r--   0        0        0     1639 2024-04-04 06:59:50.663250 opentelemetry_wrapper-0.1.9/setup_otel_logging.py
+-rw-r--r--   0        0        0     1016 2024-03-13 01:24:02.712219 opentelemetry_wrapper-0.1.9/sqlalchemy_example.py
+-rw-r--r--   0        0        0    11116 1970-01-01 00:00:00.000000 opentelemetry_wrapper-0.1.9/PKG-INFO
```

### Comparing `opentelemetry_wrapper-0.1.8/.gitignore` & `opentelemetry_wrapper-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `opentelemetry_wrapper-0.1.8/LICENSE` & `opentelemetry_wrapper-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_wrapper-0.1.8/README.md` & `opentelemetry_wrapper-0.1.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 ### safe
 
 * **never crash the application**
     * fallback to non-`opentelemetry` if necessary
     * ignore input over raising an exception
     * possible exception: it may be better to fail at startup than to run with known bad config
         * https://opentelemetry.io/docs/specs/otel/error-handling/#basic-error-handling-principles
+    * make dangerous things impossible (by design) > difficult (guardrails) > unusual (defaults) > understood (docs)
+        * there should be a "best practice" somewhere in that statement
 * **hard to get wrong**
     * idempotent, even when you instrument the same thing in different ways from different places
     * "be conservative in what you send, be liberal in what you accept"
     * note: easy and simple mean different things
 
 ### unsurprising
 
@@ -44,25 +46,26 @@
 > 1. call `instrument_all()` to instrument `logging` and `requests`
 > 2. instrument your FastAPI app using `instrument_fastapi_app(FastAPI(...))`
 > 3. use `@instrument_decorate` on any function or class you want to monitor
 > 4. set `OTEL_WRAPPER_DISABLED=true` in your CICD tests, especially if you're using `pytest`
 
 ### env vars
 
-| Variable Name                   | Description                                                                                                                                       | Default (if not set)                                                                        |
-|---------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------|
-| `OTEL_EXPORTER_OTLP_ENDPOINT`   | Looks like `http://tempo.localhost:4317`.                                                                                                         | *NA* (traces are not exported to any OTLP endpoint)                                         |
-| `OTEL_EXPORTER_OTLP_HEADER`     | Looks like `Header-Name=header value`, where values can contain space ('\x20'). To insert multiple headers, delimit by any other whitespace char. | *NA* (no header sent to OTLP endpoint)                                                      |
-| `OTEL_EXPORTER_OTLP_INSECURE`   | Set to `true` to disable SSL for OTLP trace exports, or `false` to always verify.                                                                 | *NA* (follows OpenTelemetry default, which is secure for https and insecure for http)       |
-| `OTEL_EXPORTER_PROMETHEUS_PORT` | The port on which to expose methics for Prometheus. (E.g. `9464` to expose `http://localhost:9464/metrics`)                                       | *NA* (follows OpenTelemetry default, which is secure for https and insecure for http)       |
-| `OTEL_HEADER_ATTRIBUTES`        | List of HTTP headers to extract from incoming requests as span attributes, split by whitespace.                                                   | x-pf-number, x-client-id, x-preferred-username, x-resource-access                           |
-| `OTEL_LOG_LEVEL`                | Log level used by the logging instrumentor (case-insensitive).                                                                                    | `info`                                                                                      |
-| `OTEL_SERVICE_NAME`             | Sets the value of the `service.name` resource attribute.                                                                                          | f'{k8s namespace}/{k8s pod name}' or f'{username}@{hostname}.{domain}:<{filename of main}>' |
-| `OTEL_SERVICE_NAMESPACE`        | Sets the value of the `service.namespace` resource attribute.                                                                                     | f'{k8s namespace}' or None                                                                  |
-| `OTEL_WRAPPER_DISABLED`         | Set to `true` to disable tracing globally (e.g. when running pytest).                                                                             | `false` (tracing is enabled)                                                                |
+| Variable Name                       | Description                                                                                                                                                                                   | Default (if not set)                                                                        |
+|-------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------|
+| `OTEL_EXPORTER_OTLP_ENDPOINT`       | Looks like `http://tempo.localhost:4317`.                                                                                                                                                     | *NA* (traces are not exported to any OTLP endpoint)                                         |
+| `OTEL_EXPORTER_OTLP_HEADER`         | Looks like `Header-Name=header value`, where values can contain space ('\x20'). To insert multiple headers, delimit by any other whitespace char.                                             | *NA* (no header sent to OTLP endpoint)                                                      |
+| `OTEL_EXPORTER_OTLP_INSECURE`       | Set to `true` to disable SSL for OTLP trace exports, or `false` to always verify.                                                                                                             | *NA* (follows OpenTelemetry default, which is secure for https and insecure for http)       |
+| `OTEL_EXPORTER_PROMETHEUS_PORT`     | The port on which to expose metrics for Prometheus, running in parallel as a WSGI app. (E.g. `9464` to expose `http://localhost:9464/metrics`) WARNING: do not use the same port as your app. | *NA* (no Prometheus server)                                                                 |
+| `OTEL_EXPORTER_PROMETHEUS_ENDPOINT` | An endpoint on which to expose metrics for Prometheus via FastAPI. (E.g. `/metrics`, which will 307 redirect to `/metrics/`) WARNING: this can clash with your fastapi routes                 | *NA* (no Prometheus endpoint)                                                               |
+| `OTEL_HEADER_ATTRIBUTES`            | List of HTTP headers to extract from incoming requests as span attributes, split by whitespace.                                                                                               | x-pf-number, x-client-id, x-preferred-username, x-resource-access                           |
+| `OTEL_LOG_LEVEL`                    | Log level used by the logging instrumentor (case-insensitive).                                                                                                                                | `info`                                                                                      |
+| `OTEL_SERVICE_NAME`                 | Sets the value of the `service.name` resource attribute.                                                                                                                                      | f'{k8s namespace}/{k8s pod name}' or f'{username}@{hostname}.{domain}:<{filename of main}>' |
+| `OTEL_SERVICE_NAMESPACE`            | Sets the value of the `service.namespace` resource attribute.                                                                                                                                 | f'{k8s namespace}' or None                                                                  |
+| `OTEL_WRAPPER_DISABLED`             | Set to `true` to disable tracing globally (e.g. when running pytest).                                                                                                                         | `false` (tracing is enabled)                                                                |
 
 > **Note:** <br>
 > The `service.name` and `service.namespace` can also be set via `OTEL_RESOURCE_ATTRIBUTES`, but any settings there
 > will be overwritten by `OTEL_SERVICE_NAME` and `OTEL_SERVICE_NAMESPACE`. For more details, read the
 > original [OpenTelemetry docs](https://opentelemetry.io/docs)
 
 ### `@instrument_decorate` decorator for functions and classes
@@ -113,17 +116,16 @@
 instrument_logging()
 
 logging.warning('...')
 ```
 
 ### instrumenting fastapi
 
-* while the `instrument_fastapi()` function will auto-instrument any app that is created, if your import order is wrong
-  then your app may end up not being instrumented
-* as such, it is safer to explicitly call `instrument_fastapi_app`
+* Warning: using `opentelemetry.instrumentation.fastapi.FastAPIInstrumentor` does not work as intended
+* use `instrument_fastapi_app`, for example:
 
 ```python
 from fastapi import FastAPI
 from opentelemetry_wrapper import instrument_fastapi_app
 
 app = instrument_fastapi_app(FastAPI(...))
 ```
```

### Comparing `opentelemetry_wrapper-0.1.8/TODO.md` & `opentelemetry_wrapper-0.1.9/TODO.md`

 * *Files 9% similar despite different names*

```diff
@@ -35,30 +35,35 @@
     * `flit publish`
 * check that it can be downloaded/installed
     * `cd tmp`
     * `pip download opentelemetry_wrapper==X.Y.Z` <- replace with latest `__version__`
 
 ## todo
 
-* why is the fastapi instrumentor not outputting metrics? does it need to call observable metrics?
-  * consider doing whatever `prometheus-fastapi-instrumentator` is doing instead
+* an intelligent way to include multiple headers in `OTEL_EXPORTER_OTLP_HEADER`
+  * may need support for escapes
+* allow exposing prometheus via fastapi endpoint in an instrumented app
+    * probably create an asgi app and mount it to /metrics or something
+* consider RED metrics, e.g. whatever `prometheus-fastapi-instrumentator` is doing
 * documentation pls, including design decisions
 * rename `OTEL_EXPORTER_*` to `OTEL_COLLECTOR_*`
-  * and have separate metric, log, and trace collectors
-  * separate for http and grpc exporters too
+    * and have separate metric, log, and trace collectors
+    * separate for http and grpc exporters too
+    * maybe allow multiple urls (delimited by whitespace)?
 * env var to enable/disable console printing for logs, metrics (off by default), and traces
 * set `__tracebackhide__=True` (pytest) and `__traceback_hide__=True` (a few others like sentry) in the functions
 * update [introspect.py](./opentelemetry_wrapper/utils/introspect.py) for pep 626
     * The f_lineno attribute of frame objects will always contain the expected line number.
     * The co_lnotab attribute of code objects is deprecated and will be removed in 3.12.
     * Code that needs to convert from offset to line number should use the new co_lines() method instead.
 * `OTEL_HEADER_ATTRIBUTES` behaves too much like `OTEL_INSTRUMENTATION_HTTP_CAPTURE_HEADERS_SERVER_REQUEST`
-    * consider removing it?
+    * ~~consider removing it?~~
+    * update docs to explain the difference: decoding base64 and flattening json
 * `with ...` instrumentation for non-callable code (e.g. settings, semi-hardcoded config)
-  * see [next_version_intended_usage.py](./next_version_intended_usage.py)
+    * see [next_version_intended_usage.py](./next_version_intended_usage.py)
 * type-checking decorator, with warning on unmatched types
     * https://github.com/prechelt/typecheck-decorator/blob/master/README.md
     * https://stackoverflow.com/questions/36879932/python-type-checking-decorator
     * https://towardsdatascience.com/the-power-of-decorators-fef4dc97020e
     * https://typeguard.readthedocs.io/en/latest/userguide.html
     * or use `pydantic.TypeAdaptor` to manually check
 * correctly handle generators and context managers (and async versions of them)
@@ -70,11 +75,11 @@
         * reading frames to make a statistical guess how much time is spent in each function
     * https://psutil.readthedocs.io/en/latest/
     * Request Error Duration metrics can be calculated from spans
 * also add a prometheus endpoint for scraping?
 * builtin `tracemalloc` can be used locate the source file and line number of a function, if started early enough
     * check for the [`PYTHONTRACEMALLOC`](https://docs.python.org/3/using/cmdline.html#envvar-PYTHONTRACEMALLOC) var?
 * somehow mark functions/endpoints as do-not-instrument, for extremely spammy functions? or specify a sampling ratio?
-  * the nearest sampling ratio should overwrite, but idk how to do that
+    * the nearest sampling ratio should overwrite, but idk how to do that
 * add a (regex-based?) sanitizer to erase strings/patterns from log output
 * print config at startup? at least print the version?
     * or maybe print a json string with all the (non-sensitive) config?
```

### Comparing `opentelemetry_wrapper-0.1.8/experiment_otel_logging.py` & `opentelemetry_wrapper-0.1.9/experiment_otel_logging.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_wrapper-0.1.8/fastapi_main.py` & `opentelemetry_wrapper-0.1.9/fastapi_main.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,16 +63,20 @@
 def hello_hello() -> str:
     logging.info('called `hello-hello`')
     r = requests.get('http://localhost:8000/hello/hello')
     logging.info(f'`hello` returned {r.text}')
     return r.text
 
 
+# app.mount('/metrics', make_asgi_app())
+
 if __name__ == '__main__':
     os.environ['OTEL_EXPORTER_PROMETHEUS_PORT'] = '9464'
+    os.environ['OTEL_EXPORTER_PROMETHEUS_ENDPOINT'] = '/metrics'
+
     uvicorn.run(f'{inspect.getmodulename(__file__)}:app',
                 host='localhost',
                 port=8000,
                 # reload=True,
                 access_log=True,
                 workers=2,  # not valid with reload=True
                 # proxy_headers=True,  # github.com/encode/uvicorn/blob/master/uvicorn/middleware/proxy_headers.py
```

### Comparing `opentelemetry_wrapper-0.1.8/log_weird_things.py` & `opentelemetry_wrapper-0.1.9/log_weird_things.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 instrument_logging()
 
 # json-like
 logging.warning('')
 logging.warning(None)
 logging.warning([1, 2, 3])
-logging.warning({1: 11, None: None, 'a': 'A'})
+logging.warning({1: 11, None: None, 'a': {'A'}})
 logging.warning(float('nan'))
 logging.warning(float('inf'))
 logging.warning(float('-inf'))
 
 # not json-like
 logging.info(1.234 + 4j)  # a complex number
 logging.info(Decimal('0.11111111111111111111111111111111111111111111111111111111111111111111'))  # impossible precision
```

### Comparing `opentelemetry_wrapper-0.1.8/next_version_intended_usage.py` & `opentelemetry_wrapper-0.1.9/next_version_intended_usage.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/__init__.py` & `opentelemetry_wrapper-0.1.9/opentelemetry_wrapper/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,50 @@
 """
 a wrapper around `opentelemetry` and `opentelemetry-instrumentation-*` to make life a bit easier
 """
 
-__version__ = '0.1.8'
+__version__ = '0.1.9'
 
 from opentelemetry_wrapper.config.otel_headers import OTEL_WRAPPER_DISABLED
 from opentelemetry_wrapper.dependencies.opentelemetry.instrument_dataclasses import instrument_dataclasses
 from opentelemetry_wrapper.dependencies.opentelemetry.instrument_decorator import instrument_decorate
-from opentelemetry_wrapper.dependencies.opentelemetry.instrument_fastapi import instrument_fastapi
 from opentelemetry_wrapper.dependencies.opentelemetry.instrument_fastapi import instrument_fastapi_app
 from opentelemetry_wrapper.dependencies.opentelemetry.instrument_logging import instrument_logging
 from opentelemetry_wrapper.dependencies.opentelemetry.instrument_requests import instrument_requests
 from opentelemetry_wrapper.dependencies.opentelemetry.instrument_sqlalchemy import instrument_sqlalchemy
 from opentelemetry_wrapper.dependencies.opentelemetry.instrument_system_metrics import instrument_system_metrics
 
 
 @instrument_decorate
 def instrument_all(dataclasses: bool = True,
                    logging: bool = True,
-                   fastapi: bool = True,
                    requests: bool = True,
                    sqlalchemy: bool = False,  # too noisy for a default
                    log_json: bool = True,
                    system_metrics: bool = True
                    ):
     # no-op
     if OTEL_WRAPPER_DISABLED:
         return
 
     if dataclasses:
         instrument_dataclasses()
     if logging:
         instrument_logging(print_json=log_json)
-    if fastapi:
-        instrument_fastapi()
     if requests:
         instrument_requests()
     if sqlalchemy:
         instrument_sqlalchemy()
     if system_metrics:
         instrument_system_metrics()
 
 
 __all__ = (
     '__version__',
     'instrument_all',
     'instrument_decorate',
     'instrument_dataclasses',
     'instrument_logging',
-    'instrument_fastapi',
     'instrument_fastapi_app',
     'instrument_requests',
     'instrument_sqlalchemy',
 )
```

### Comparing `opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/config/otel_exporter_otlp.py` & `opentelemetry_wrapper-0.1.9/opentelemetry_wrapper/config/otel_exporter_otlp.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/config/otel_header_attributes.py` & `opentelemetry_wrapper-0.1.9/opentelemetry_wrapper/config/otel_header_attributes.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/config/otel_headers.py` & `opentelemetry_wrapper-0.1.9/opentelemetry_wrapper/config/otel_headers.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from opentelemetry_wrapper.config.otel_exporter_otlp import getenv_otel_exporter_otlp_insecure
 from opentelemetry_wrapper.config.otel_header_attributes import get_header_attributes
 from opentelemetry_wrapper.config.otel_log_level import get_log_level
 from opentelemetry_wrapper.config.otel_service_name import get_default_service_name
 from opentelemetry_wrapper.config.otel_service_name import get_k8s_namespace
 from opentelemetry_wrapper.config.otel_service_name import getenv_otel_service_name
 from opentelemetry_wrapper.config.otel_service_name import getenv_otel_service_namespace
+from opentelemetry_wrapper.config.otel_wrapper_prometheus_exporter import get_prometheus_endpoint
 from opentelemetry_wrapper.config.otel_wrapper_prometheus_exporter import get_prometheus_port
 
 # global flag to override opentelemetry and not do anything
 # because opentelemetry is too verbose in tests
 # naming / terminology based on:
 # https://opentelemetry.io/docs/reference/specification/sdk-environment-variables/#:~:text=OTEL_SDK_DISABLED
 OTEL_WRAPPER_DISABLED: bool = os.getenv('OTEL_WRAPPER_DISABLED', 'false').casefold().strip() == 'true'
@@ -35,7 +36,8 @@
 OTEL_EXPORTER_OTLP_INSECURE: Optional[bool] = getenv_otel_exporter_otlp_insecure()
 
 OTEL_LOG_LEVEL: int = get_log_level()
 
 OTEL_HEADER_ATTRIBUTES: List[str] = get_header_attributes()
 
 OTEL_EXPORTER_PROMETHEUS_PORT: Optional[int] = get_prometheus_port()
+OTEL_EXPORTER_PROMETHEUS_ENDPOINT: Optional[str] = get_prometheus_endpoint()
```

### Comparing `opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/config/otel_log_level.py` & `opentelemetry_wrapper-0.1.9/opentelemetry_wrapper/config/otel_log_level.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/config/otel_service_name.py` & `opentelemetry_wrapper-0.1.9/opentelemetry_wrapper/config/otel_service_name.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/dependencies/opentelemetry/instrument_dataclasses.py` & `opentelemetry_wrapper-0.1.9/opentelemetry_wrapper/dependencies/opentelemetry/instrument_dataclasses.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/dependencies/opentelemetry/instrument_decorator.py` & `opentelemetry_wrapper-0.1.9/opentelemetry_wrapper/dependencies/opentelemetry/instrument_decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from opentelemetry.trace import Status
 from opentelemetry.trace import StatusCode
 
 from opentelemetry_wrapper import __version__  # don't worry, this does not create an infinite import loop
 from opentelemetry_wrapper.config.otel_headers import OTEL_WRAPPER_DISABLED
 from opentelemetry_wrapper.dependencies.opentelemetry.otel_providers import get_tracer
 from opentelemetry_wrapper.utils.introspect import CodeInfo
+from opentelemetry_wrapper.utils.introspect import unwrap_function
 
 _TRACER = get_tracer(__name__, __version__)  # TODO: move this somewhere else
 
 InstrumentableThing = TypeVar('InstrumentableThing', Callable, Coroutine, type)
 
 _CACHE_INSTRUMENTED: Dict[InstrumentableThing, Optional[InstrumentableThing]] = dict()  # type: ignore[valid-type]
 _CACHE_GETATTRIBUTE: Dict[InstrumentableThing, InstrumentableThing] = dict()  # type: ignore[valid-type]
@@ -59,29 +60,30 @@
     # this requires slightly more complex logic than lru_cache provides
     if func in _CACHE_INSTRUMENTED:
         ret = _CACHE_INSTRUMENTED[func]
         if ret is not None:
             return ret
         return func
 
-    # if not provided, try to find the function name
-    code_info = CodeInfo(func)
-    func_name = func_name or code_info.name
-
     # avoid re-instrumenting functions with wrappers (e.g., lru_cache)
-    # note: this only works if the base function is instrumented
-    # todo: peel back one layer at a time and check if its instrumented
+    # by peeling back one layer at a time and checking if its instrumented
+    # note: this does not catch the edge case where you instrument a wrapped function first
+    # and instrument the base function later on
     # noinspection PyBroadException
     try:
-        # noinspection PyProtectedMember
-        if code_info._unwrapped_code_object in _CACHE_INSTRUMENTED:
-            return func
+        for _, code_object in unwrap_function(func):
+            if code_object in _CACHE_INSTRUMENTED:
+                return func
     except Exception:
         pass
 
+    # if not provided, try to find the function name
+    code_info = CodeInfo(func)
+    func_name = func_name or code_info.name
+
     # build span attributes for this class / function / method / builtin / etc
     span_attributes: Dict[str, Union[str, None, int]] = dict()
     if code_info.function_name:
         span_attributes[SpanAttributes.CODE_FUNCTION] = code_info.function_name
     if code_info.module_name:
         span_attributes[SpanAttributes.CODE_NAMESPACE] = code_info.module_name
     if code_info.path:
```

### Comparing `opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/dependencies/opentelemetry/instrument_logging.py` & `opentelemetry_wrapper-0.1.9/opentelemetry_wrapper/dependencies/opentelemetry/instrument_logging.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/dependencies/opentelemetry/instrument_sqlalchemy.py` & `opentelemetry_wrapper-0.1.9/opentelemetry_wrapper/dependencies/opentelemetry/instrument_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/dependencies/opentelemetry/otel_providers.py` & `opentelemetry_wrapper-0.1.9/opentelemetry_wrapper/dependencies/opentelemetry/otel_providers.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,17 +103,22 @@
     if OTEL_EXPORTER_OTLP_ENDPOINT:
         metric_readers.append(PeriodicExportingMetricReader(OTLPMetricExporter(endpoint=OTEL_EXPORTER_OTLP_ENDPOINT,
                                                                                headers=OTEL_EXPORTER_OTLP_HEADER,
                                                                                insecure=OTEL_EXPORTER_OTLP_INSECURE)))
 
     # https://opentelemetry.io/docs/languages/python/exporters/#prometheus-dependencies
     if OTEL_EXPORTER_PROMETHEUS_PORT is not None:
-        start_http_server(port=OTEL_EXPORTER_PROMETHEUS_PORT, addr="localhost")
-        metric_readers.append(PrometheusMetricReader())
+        # noinspection PyBroadException
+        try:
+            start_http_server(port=OTEL_EXPORTER_PROMETHEUS_PORT, addr="localhost")
+        except Exception:
+            logging.exception(f'failed to start prometheus server at port {OTEL_EXPORTER_PROMETHEUS_PORT}')
 
+    # always include prometheus metric reader since we might use the endpoint instead of the port
+    metric_readers.append(PrometheusMetricReader())
     mp = MeterProvider(resource=get_otel_resource(), metric_readers=metric_readers)
 
     # metrics.set_meter_provider(provider)
     # noinspection PyUnresolvedReferences,PyProtectedMember
     metrics._internal._set_meter_provider(mp, log=False)  # try to set, but don't warn otherwise
```

### Comparing `opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/dependencies/sqlalchemy/engine_typedef.py` & `opentelemetry_wrapper-0.1.9/opentelemetry_wrapper/dependencies/sqlalchemy/engine_typedef.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/utils/extract_json_header.py` & `opentelemetry_wrapper-0.1.9/opentelemetry_wrapper/utils/extract_json_header.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/utils/introspect.py` & `opentelemetry_wrapper-0.1.9/opentelemetry_wrapper/utils/introspect.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,144 @@
 import asyncio
 import importlib.util
 import inspect
 import sys
 from dataclasses import dataclass
 from dataclasses import field
+from functools import WRAPPER_ASSIGNMENTS
+from functools import WRAPPER_UPDATES
 from functools import cached_property
 from functools import lru_cache
 from functools import partial
 from functools import partialmethod
 from functools import singledispatchmethod
 from pathlib import Path
 from types import ModuleType
+from typing import Any
 from typing import Callable
 from typing import Coroutine
 from typing import Dict
+from typing import Generator
 from typing import List
 from typing import Optional
+from typing import Tuple
 from typing import Union
 
+CodeObjectType = Union[
+    Coroutine, Callable,
+    partial, partialmethod, singledispatchmethod, cached_property,
+    asyncio.Task,
+    type, property
+]
+
+
+def _is_function_type(_code_object: CodeObjectType) -> bool:
+    if callable(_code_object):
+        return True
+    if isinstance(_code_object, (Coroutine, Callable)):  # `def` and `async def`
+        return True
+    if isinstance(_code_object, (partial, partialmethod, singledispatchmethod, cached_property)):  # `functools`
+        return True
+    if isinstance(_code_object, asyncio.Task):
+        return True
+    return False
+
+
+def _unwrap_partial(_code_object: CodeObjectType) -> Tuple[Optional[str], CodeObjectType]:  # NOSONAR (complexity=32)
+    # class-based wrappers
+    for wrapper_class in (partial, partialmethod, singledispatchmethod, cached_property):
+        if isinstance(_code_object, wrapper_class):
+            return f'functools.{wrapper_class.__name__}', _code_object.func
+
+    # make best guess about the wrapper
+    _wrapped_code = getattr(_code_object, '__wrapped__', None)
+    if _is_function_type(_wrapped_code):
+
+        # probably single dispatch
+        if all(hasattr(_code_object, _attr) for _attr in {'register', 'dispatch', 'registry', '_clear_cache'}):
+            return 'functools.singledispatch', _wrapped_code
+
+        # could be lru_cache or cache (but that's a special_case of lru_cache anyway)
+        if all(hasattr(_code_object, _attr) for _attr in {'cache_info', 'cache_clear'}):
+            return 'functools.lru_cache', _wrapped_code
+
+        # update_wrapper was probably called, and since it's not internal to functools it's probably via wraps
+        if all(getattr(_wrapped_code, _a, None) == getattr(_code_object, _a, None) for _a in WRAPPER_ASSIGNMENTS):
+            for _u in WRAPPER_UPDATES:
+                # this must be a dict
+                if not isinstance(getattr(_code_object, _u, None), dict):
+                    break
+                # this should be a superset, since the keys probably won't be deleted
+                if not set(getattr(_code_object, _u).keys()).issuperset(getattr(_wrapped_code, _u, {}).keys()):
+                    break
+                # the values should also match, since devs are lazy to update things
+                for k, v in getattr(_wrapped_code, _u, {}).items():
+                    if getattr(_code_object, _u)[k] != v:
+                        break
+                else:
+                    break
+            else:
+                return 'functools.wraps', _wrapped_code
+
+    # failed to unwrap
+    return None, _code_object
+
+
+def _unwrap_async(_code_object: CodeObjectType) -> Tuple[Optional[str], CodeObjectType]:
+    # unwrap tasks
+    if isinstance(_code_object, asyncio.Task):
+        return 'asyncio.Task', _code_object.get_coro()
+
+    # attempt to detect asgiref.sync_to_async and asgiref.async_to_sync
+    _module = inspect.getmodule(_code_object)
+    if hasattr(_module, '__name__') and _module.__name__ == 'asgiref.sync':
+
+        # must check this first because it may also have an `awaitable` attribute
+        if hasattr(_code_object, 'func'):
+            if _is_function_type(_code_object.func):
+                return 'asgiref.sync.SynctoAsync', _code_object.func
+
+        if hasattr(_code_object, 'awaitable'):
+            if _is_function_type(_code_object.awaitable):
+                return 'asgiref.sync.AsyncToSync', _code_object.awaitable
+
+    # failed to unwrap
+    return None, _code_object
+
+
+def unwrap_function(code_object: CodeObjectType,
+                    *,
+                    unwrap_partial: bool = True,
+                    unwrap_async: bool = True,
+                    ) -> Generator[Tuple[str, CodeObjectType], Any, None]:
+    while True:
+
+        # handle wrappers from functools
+        if unwrap_partial:
+            _wrapper, code_object = _unwrap_partial(code_object)
+            if _wrapper is not None:
+                yield _wrapper, code_object
+                continue
+
+        # handle async
+        if unwrap_async:
+            _wrapper, code_object = _unwrap_async(code_object)
+            if _wrapper is not None:
+                yield _wrapper, code_object
+                continue
+
+        # unable to unwrap any further
+        return
+
 
 # noinspection PyBroadException
 @lru_cache(maxsize=None)
 @dataclass(unsafe_hash=True, frozen=True)
 class CodeInfo:
-    code_object: Union[Coroutine, Callable,
-    partial, partialmethod, singledispatchmethod, cached_property,
-    asyncio.Task,
-    type, property]
+    code_object: CodeObjectType
 
     unwrap_partial: bool = True
     unwrap_async: bool = True
 
     _maybe_unsafe__try_very_hard_to_find_class: bool = True
 
     __cached_cls: List[type] = field(default_factory=list, init=False, repr=False, hash=False, compare=False)
@@ -171,14 +279,16 @@
 
         return None
 
     @cached_property
     def cls(self) -> Optional[type]:
         try:
             # if we already are a class
+            # NOTE: this does not unwrap classes, only functions
+            # TODO: unwrap classes too
             if self.is_class:
                 return self._unwrapped_code_object
 
             # get class of method
             if inspect.ismethod(self._unwrapped_code_object) or \
                     (inspect.isbuiltin(self._unwrapped_code_object) and
                      hasattr(self._unwrapped_code_object, '__self__')):
@@ -300,83 +410,20 @@
         if isinstance(code_object, asyncio.Task):
             return True
 
         return False
 
     @cached_property
     def __unwrapped(self):
-        # todo: provide a way to get at all the layers, so that i can check whether any of them are instrumented
-        # this should probably be externalized and yield all the layers one at a time
         _code_object = self.code_object
         _prefixes = []
-
-        # unwrap recursively
-        while True:
-
-            # handle wrappers from functools
-            if self.unwrap_partial:
-
-                # class-based wrappers
-                if isinstance(_code_object, partial):
-                    _prefixes.append('partial')
-                    _code_object = _code_object.func
-                    continue
-                if isinstance(_code_object, partialmethod):
-                    _prefixes.append('partialmethod')
-                    _code_object = _code_object.func
-                    continue
-                if isinstance(_code_object, singledispatchmethod):
-                    _prefixes.append('singledispatchmethod')
-                    _code_object = _code_object.func
-                    continue
-                if isinstance(_code_object, cached_property):
-                    _prefixes.append('cached_property')
-                    _code_object = _code_object.func
-                    continue
-
-                # make best guess about the wrapper
-                if hasattr(_code_object, '__wrapped__'):
-                    if self.__is_supported_type(_code_object.__wrapped__):
-                        if all(hasattr(_code_object, _attr) for _attr in
-                               {'register', 'dispatch', 'registry', '_clear_cache'}):
-                            _prefixes.append('singledispatch')
-                        elif all(hasattr(_code_object, _attr) for _attr in {'cache_info', 'cache_clear'}):
-                            _prefixes.append('lru_cache')
-                        _code_object = _code_object.__wrapped__
-                        continue
-
-            # handle async
-            if self.unwrap_async:
-
-                # unwrap tasks
-                if isinstance(_code_object, asyncio.Task):
-                    _prefixes.append('Task')
-                    _code_object = _code_object.get_coro()
-                    continue
-
-                # attempt to detect asgiref.sync_to_async and asgiref.async_to_sync
-                _module = inspect.getmodule(_code_object)
-                if hasattr(_module, '__name__') and _module.__name__ == 'asgiref.sync':
-
-                    # must check this first because it may also have an `awaitable` attribute
-                    if hasattr(_code_object, 'func'):
-                        if self.__is_supported_type(_code_object.func):
-                            _prefixes.append('SynctoAsync')
-                            _code_object = _code_object.func
-                            continue
-
-                    if hasattr(_code_object, 'awaitable'):
-                        if self.__is_supported_type(_code_object.awaitable):
-                            _prefixes.append('AsyncToSync')
-                            _code_object = _code_object.awaitable
-                            continue
-
-            # unable to unwrap any further
-            break
-
+        for _wrapper, _code_object in unwrap_function(self.code_object,
+                                                      unwrap_partial=self.unwrap_partial,
+                                                      unwrap_async=self.unwrap_async):
+            _prefixes.append(_wrapper)
         return _prefixes, _code_object
 
     @property
     def __unwrapped_prefixes(self) -> List[str]:
         return self.__unwrapped[0]
 
     @property
```

### Comparing `opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/utils/json_encoder.py` & `opentelemetry_wrapper-0.1.9/opentelemetry_wrapper/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_wrapper-0.1.8/opentelemetry_wrapper/utils/logging_json_formatter.py` & `opentelemetry_wrapper-0.1.9/opentelemetry_wrapper/utils/logging_json_formatter.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_wrapper-0.1.8/pyproject.toml` & `opentelemetry_wrapper-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `opentelemetry_wrapper-0.1.8/setup_otel_logging.py` & `opentelemetry_wrapper-0.1.9/setup_otel_logging.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_wrapper-0.1.8/sqlalchemy_example.py` & `opentelemetry_wrapper-0.1.9/sqlalchemy_example.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_wrapper-0.1.8/PKG-INFO` & `opentelemetry_wrapper-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry_wrapper
-Version: 0.1.8
+Version: 0.1.9
 Summary: a wrapper around `opentelemetry` and `opentelemetry-instrumentation-*` to make life a bit easier
 Author-email: Avery Khoo <averykhoo@gmail.com>
 Requires-Python: >3.8.0
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: asgiref
 Requires-Dist: fastapi
@@ -35,14 +35,16 @@
 ### safe
 
 * **never crash the application**
     * fallback to non-`opentelemetry` if necessary
     * ignore input over raising an exception
     * possible exception: it may be better to fail at startup than to run with known bad config
         * https://opentelemetry.io/docs/specs/otel/error-handling/#basic-error-handling-principles
+    * make dangerous things impossible (by design) > difficult (guardrails) > unusual (defaults) > understood (docs)
+        * there should be a "best practice" somewhere in that statement
 * **hard to get wrong**
     * idempotent, even when you instrument the same thing in different ways from different places
     * "be conservative in what you send, be liberal in what you accept"
     * note: easy and simple mean different things
 
 ### unsurprising
 
@@ -72,25 +74,26 @@
 > 1. call `instrument_all()` to instrument `logging` and `requests`
 > 2. instrument your FastAPI app using `instrument_fastapi_app(FastAPI(...))`
 > 3. use `@instrument_decorate` on any function or class you want to monitor
 > 4. set `OTEL_WRAPPER_DISABLED=true` in your CICD tests, especially if you're using `pytest`
 
 ### env vars
 
-| Variable Name                   | Description                                                                                                                                       | Default (if not set)                                                                        |
-|---------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------|
-| `OTEL_EXPORTER_OTLP_ENDPOINT`   | Looks like `http://tempo.localhost:4317`.                                                                                                         | *NA* (traces are not exported to any OTLP endpoint)                                         |
-| `OTEL_EXPORTER_OTLP_HEADER`     | Looks like `Header-Name=header value`, where values can contain space ('\x20'). To insert multiple headers, delimit by any other whitespace char. | *NA* (no header sent to OTLP endpoint)                                                      |
-| `OTEL_EXPORTER_OTLP_INSECURE`   | Set to `true` to disable SSL for OTLP trace exports, or `false` to always verify.                                                                 | *NA* (follows OpenTelemetry default, which is secure for https and insecure for http)       |
-| `OTEL_EXPORTER_PROMETHEUS_PORT` | The port on which to expose methics for Prometheus. (E.g. `9464` to expose `http://localhost:9464/metrics`)                                       | *NA* (follows OpenTelemetry default, which is secure for https and insecure for http)       |
-| `OTEL_HEADER_ATTRIBUTES`        | List of HTTP headers to extract from incoming requests as span attributes, split by whitespace.                                                   | x-pf-number, x-client-id, x-preferred-username, x-resource-access                           |
-| `OTEL_LOG_LEVEL`                | Log level used by the logging instrumentor (case-insensitive).                                                                                    | `info`                                                                                      |
-| `OTEL_SERVICE_NAME`             | Sets the value of the `service.name` resource attribute.                                                                                          | f'{k8s namespace}/{k8s pod name}' or f'{username}@{hostname}.{domain}:<{filename of main}>' |
-| `OTEL_SERVICE_NAMESPACE`        | Sets the value of the `service.namespace` resource attribute.                                                                                     | f'{k8s namespace}' or None                                                                  |
-| `OTEL_WRAPPER_DISABLED`         | Set to `true` to disable tracing globally (e.g. when running pytest).                                                                             | `false` (tracing is enabled)                                                                |
+| Variable Name                       | Description                                                                                                                                                                                   | Default (if not set)                                                                        |
+|-------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------|
+| `OTEL_EXPORTER_OTLP_ENDPOINT`       | Looks like `http://tempo.localhost:4317`.                                                                                                                                                     | *NA* (traces are not exported to any OTLP endpoint)                                         |
+| `OTEL_EXPORTER_OTLP_HEADER`         | Looks like `Header-Name=header value`, where values can contain space ('\x20'). To insert multiple headers, delimit by any other whitespace char.                                             | *NA* (no header sent to OTLP endpoint)                                                      |
+| `OTEL_EXPORTER_OTLP_INSECURE`       | Set to `true` to disable SSL for OTLP trace exports, or `false` to always verify.                                                                                                             | *NA* (follows OpenTelemetry default, which is secure for https and insecure for http)       |
+| `OTEL_EXPORTER_PROMETHEUS_PORT`     | The port on which to expose metrics for Prometheus, running in parallel as a WSGI app. (E.g. `9464` to expose `http://localhost:9464/metrics`) WARNING: do not use the same port as your app. | *NA* (no Prometheus server)                                                                 |
+| `OTEL_EXPORTER_PROMETHEUS_ENDPOINT` | An endpoint on which to expose metrics for Prometheus via FastAPI. (E.g. `/metrics`, which will 307 redirect to `/metrics/`) WARNING: this can clash with your fastapi routes                 | *NA* (no Prometheus endpoint)                                                               |
+| `OTEL_HEADER_ATTRIBUTES`            | List of HTTP headers to extract from incoming requests as span attributes, split by whitespace.                                                                                               | x-pf-number, x-client-id, x-preferred-username, x-resource-access                           |
+| `OTEL_LOG_LEVEL`                    | Log level used by the logging instrumentor (case-insensitive).                                                                                                                                | `info`                                                                                      |
+| `OTEL_SERVICE_NAME`                 | Sets the value of the `service.name` resource attribute.                                                                                                                                      | f'{k8s namespace}/{k8s pod name}' or f'{username}@{hostname}.{domain}:<{filename of main}>' |
+| `OTEL_SERVICE_NAMESPACE`            | Sets the value of the `service.namespace` resource attribute.                                                                                                                                 | f'{k8s namespace}' or None                                                                  |
+| `OTEL_WRAPPER_DISABLED`             | Set to `true` to disable tracing globally (e.g. when running pytest).                                                                                                                         | `false` (tracing is enabled)                                                                |
 
 > **Note:** <br>
 > The `service.name` and `service.namespace` can also be set via `OTEL_RESOURCE_ATTRIBUTES`, but any settings there
 > will be overwritten by `OTEL_SERVICE_NAME` and `OTEL_SERVICE_NAMESPACE`. For more details, read the
 > original [OpenTelemetry docs](https://opentelemetry.io/docs)
 
 ### `@instrument_decorate` decorator for functions and classes
@@ -141,17 +144,16 @@
 instrument_logging()
 
 logging.warning('...')
 ```
 
 ### instrumenting fastapi
 
-* while the `instrument_fastapi()` function will auto-instrument any app that is created, if your import order is wrong
-  then your app may end up not being instrumented
-* as such, it is safer to explicitly call `instrument_fastapi_app`
+* Warning: using `opentelemetry.instrumentation.fastapi.FastAPIInstrumentor` does not work as intended
+* use `instrument_fastapi_app`, for example:
 
 ```python
 from fastapi import FastAPI
 from opentelemetry_wrapper import instrument_fastapi_app
 
 app = instrument_fastapi_app(FastAPI(...))
 ```
```

