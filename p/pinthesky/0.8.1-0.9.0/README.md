# Comparing `tmp/pinthesky-0.8.1.tar.gz` & `tmp/pinthesky-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinthesky-0.8.1.tar", last modified: Thu Apr  4 23:13:12 2024, max compression
+gzip compressed data, was "pinthesky-0.9.0.tar", last modified: Wed May 15 23:03:36 2024, max compression
```

## Comparing `pinthesky-0.8.1.tar` & `pinthesky-0.9.0.tar`

### file list

```diff
@@ -1,39 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:13:12.372517 pinthesky-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-04 23:13:08.000000 pinthesky-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-04-04 23:13:12.372517 pinthesky-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8694 2024-04-04 23:13:08.000000 pinthesky-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:13:12.368517 pinthesky-0.8.1/pinthesky/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-04 23:13:08.000000 pinthesky-0.8.1/pinthesky/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-04-04 23:13:08.000000 pinthesky-0.8.1/pinthesky/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9345 2024-04-04 23:13:08.000000 pinthesky-0.8.1/pinthesky/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)    11676 2024-04-04 23:13:08.000000 pinthesky-0.8.1/pinthesky/cloudwatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-04 23:13:08.000000 pinthesky-0.8.1/pinthesky/combiner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-04-04 23:13:08.000000 pinthesky-0.8.1/pinthesky/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-04-04 23:13:08.000000 pinthesky-0.8.1/pinthesky/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-04-04 23:13:08.000000 pinthesky-0.8.1/pinthesky/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-04-04 23:13:08.000000 pinthesky-0.8.1/pinthesky/health.py
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-04 23:13:08.000000 pinthesky-0.8.1/pinthesky/input.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-04 23:13:08.000000 pinthesky-0.8.1/pinthesky/motion_detect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-04 23:13:08.000000 pinthesky-0.8.1/pinthesky/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-04-04 23:13:08.000000 pinthesky-0.8.1/pinthesky/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-04-04 23:13:08.000000 pinthesky-0.8.1/pinthesky/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:13:12.368517 pinthesky-0.8.1/pinthesky.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-04-04 23:13:12.000000 pinthesky-0.8.1/pinthesky.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-04 23:13:12.000000 pinthesky-0.8.1/pinthesky.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 23:13:12.000000 pinthesky-0.8.1/pinthesky.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-04 23:13:12.000000 pinthesky-0.8.1/pinthesky.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-04 23:13:12.000000 pinthesky-0.8.1/pinthesky.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-04 23:13:12.000000 pinthesky-0.8.1/pinthesky.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-04 23:13:12.372517 pinthesky-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-04 23:13:08.000000 pinthesky-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:13:12.368517 pinthesky-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5876 2024-04-04 23:13:08.000000 pinthesky-0.8.1/tests/test_camera.py
--rw-r--r--   0 runner    (1001) docker     (127)     8808 2024-04-04 23:13:08.000000 pinthesky-0.8.1/tests/test_cloudwatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-04 23:13:08.000000 pinthesky-0.8.1/tests/test_combiner.py
--rw-r--r--   0 runner    (1001) docker     (127)     5052 2024-04-04 23:13:08.000000 pinthesky-0.8.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-04 23:13:08.000000 pinthesky-0.8.1/tests/test_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-04 23:13:08.000000 pinthesky-0.8.1/tests/test_health.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-04 23:13:08.000000 pinthesky-0.8.1/tests/test_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-04 23:13:08.000000 pinthesky-0.8.1/tests/test_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-04-04 23:13:08.000000 pinthesky-0.8.1/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-04-04 23:13:08.000000 pinthesky-0.8.1/tests/test_upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:36.561320 pinthesky-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-15 23:03:31.000000 pinthesky-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10500 2024-05-15 23:03:36.561320 pinthesky-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9541 2024-05-15 23:03:31.000000 pinthesky-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:36.557320 pinthesky-0.9.0/pinthesky/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-15 23:03:31.000000 pinthesky-0.9.0/pinthesky/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12356 2024-05-15 23:03:31.000000 pinthesky-0.9.0/pinthesky/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12443 2024-05-15 23:03:31.000000 pinthesky-0.9.0/pinthesky/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12297 2024-05-15 23:03:31.000000 pinthesky-0.9.0/pinthesky/cloudwatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-15 23:03:31.000000 pinthesky-0.9.0/pinthesky/combiner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-05-15 23:03:31.000000 pinthesky-0.9.0/pinthesky/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5366 2024-05-15 23:03:31.000000 pinthesky-0.9.0/pinthesky/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-15 23:03:31.000000 pinthesky-0.9.0/pinthesky/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-05-15 23:03:31.000000 pinthesky-0.9.0/pinthesky/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-05-15 23:03:31.000000 pinthesky-0.9.0/pinthesky/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-05-15 23:03:31.000000 pinthesky-0.9.0/pinthesky/health.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-05-15 23:03:31.000000 pinthesky-0.9.0/pinthesky/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-15 23:03:31.000000 pinthesky-0.9.0/pinthesky/motion_detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-15 23:03:31.000000 pinthesky-0.9.0/pinthesky/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-05-15 23:03:31.000000 pinthesky-0.9.0/pinthesky/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-05-15 23:03:31.000000 pinthesky-0.9.0/pinthesky/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:36.561320 pinthesky-0.9.0/pinthesky.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10500 2024-05-15 23:03:36.000000 pinthesky-0.9.0/pinthesky.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-15 23:03:36.000000 pinthesky-0.9.0/pinthesky.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:03:36.000000 pinthesky-0.9.0/pinthesky.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-15 23:03:36.000000 pinthesky-0.9.0/pinthesky.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-15 23:03:36.000000 pinthesky-0.9.0/pinthesky.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 23:03:36.000000 pinthesky-0.9.0/pinthesky.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-15 23:03:36.561320 pinthesky-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-15 23:03:31.000000 pinthesky-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:03:36.561320 pinthesky-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5876 2024-05-15 23:03:31.000000 pinthesky-0.9.0/tests/test_camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-05-15 23:03:31.000000 pinthesky-0.9.0/tests/test_cloudwatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-15 23:03:31.000000 pinthesky-0.9.0/tests/test_combiner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5052 2024-05-15 23:03:31.000000 pinthesky-0.9.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7118 2024-05-15 23:03:31.000000 pinthesky-0.9.0/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-15 23:03:31.000000 pinthesky-0.9.0/tests/test_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-05-15 23:03:31.000000 pinthesky-0.9.0/tests/test_health.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-15 23:03:31.000000 pinthesky-0.9.0/tests/test_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-15 23:03:31.000000 pinthesky-0.9.0/tests/test_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-05-15 23:03:31.000000 pinthesky-0.9.0/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-05-15 23:03:31.000000 pinthesky-0.9.0/tests/test_upload.py
```

### Comparing `pinthesky-0.8.1/LICENSE` & `pinthesky-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pinthesky-0.8.1/PKG-INFO` & `pinthesky-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinthesky
-Version: 0.8.1
+Version: 0.9.0
 Summary: Simple Pi In The Sky device Integration
 Home-page: https://github.com/philcali/pits-device
 Author: Philip Cali
 Author-email: philip.cali@gmail.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -159,55 +159,73 @@
 `--cloudwatch-event-type emf`. The daemon will manage the `LogStream`
 associated to the `LogGroup`, by "{year}/{month}/{day}". It will
 delineate the stream by `thing_name`. To disable this behavior, use
 `--disable-cloudwatch-stream-split`.
 
 ```
   --cloudwatch          enable the cloudwatch upload, default false
+  --cloudwatch-region CLOUDWATCH_REGION
+                        the AWS region name override for CloudWatch
   --cloudwatch-thread   enable cloudwatch logs to upload in background, default false
   --cloudwatch-event-type CLOUDWATCH_EVENT_TYPE
                         event type to upload: logs,emf,all
   --cloudwatch-metric-namespace CLOUDWATCH_METRIC_NAMESPACE
                         metric namespace when using emf event type, default Pits/Device
   --cloudwatch-log-group CLOUDWATCH_LOG_GROUP
                         uploads to this cloudwatch log group
   --disable-cloudwatch-stream-split
                         disables splitting the log stream by thing name
 ```
 
+The `pinthesky` daemon supports live streaming through an optional
+integration through a custom data plane deployed through [pits-data](https://github.com/philcali/pits-data). Enabling this integration
+is done through `--dataplane` and the endpoint and AWS region are
+targeted with `--dataplane-endpoint` and `--dataplane-region`,
+respectively. Note that deploying a custom data plane is managed
+with the infrastructure instructions below.
+
+```
+  --dataplane           enable the dataplane integration
+  --dataplane-endpoint DATAPLANE_ENDPOINT
+                        endpoint for the dataplane
+  --dataplane-region DATAPLANE_REGION
+                        the AWS region name override for the Data Plane
+```
+
 __Note__: These can be configured correctly for you if you follow the guided `pitsctl` installation
 wizard.
 
 ## Usage
 
 The `pitsctl` entry point can handle three targets:
 
 - `install`: Installs or updates software and agents for running the camera control
 - `remove`: Removes all configuration, cloud resources, software and agents
 - `view`: Inpects the installation on the device
 
 ```
-Usage: pitsctl - v0.8.1: Install or manage pinthesky software
+Usage: pitsctl - v0.9.0: Install or manage pinthesky software
   -h,--help:    Prints out this help message
   -m,--host:    Client machine connection details
   -t,--text:    Enable a no color, text only view of the application
   -r,--root:    Assume root permission for management
   -l,--level:   Changes the logging verbosity for pitsctl
   -v,--version: Prints the version and exists
 ```
 
-## Control Plane and Infrastructure
+## Control/Data Plane and Infrastructure
 
 The [pits-infra][1] package can be used to deploy a complete and working 
 AWS cloud infrastructure to support the device configuration and integration.
 The infrastructure contains the following:
 
 - Storage configuration
 - Policy and device authorization
 - Control Plane deployment
+- Data Plane deployment
 - Console deployment
 - Console authorization through Cognito
 
 Follow the [re-use][2] section in the README to deploy it for at no charge
 or 50 cents a month if a custom domain is included.
 
 [1]: https://github.com/philcali/pits-infra
```

### Comparing `pinthesky-0.8.1/README.md` & `pinthesky-0.9.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -131,55 +131,73 @@
 `--cloudwatch-event-type emf`. The daemon will manage the `LogStream`
 associated to the `LogGroup`, by "{year}/{month}/{day}". It will
 delineate the stream by `thing_name`. To disable this behavior, use
 `--disable-cloudwatch-stream-split`.
 
 ```
   --cloudwatch          enable the cloudwatch upload, default false
+  --cloudwatch-region CLOUDWATCH_REGION
+                        the AWS region name override for CloudWatch
   --cloudwatch-thread   enable cloudwatch logs to upload in background, default false
   --cloudwatch-event-type CLOUDWATCH_EVENT_TYPE
                         event type to upload: logs,emf,all
   --cloudwatch-metric-namespace CLOUDWATCH_METRIC_NAMESPACE
                         metric namespace when using emf event type, default Pits/Device
   --cloudwatch-log-group CLOUDWATCH_LOG_GROUP
                         uploads to this cloudwatch log group
   --disable-cloudwatch-stream-split
                         disables splitting the log stream by thing name
 ```
 
+The `pinthesky` daemon supports live streaming through an optional
+integration through a custom data plane deployed through [pits-data](https://github.com/philcali/pits-data). Enabling this integration
+is done through `--dataplane` and the endpoint and AWS region are
+targeted with `--dataplane-endpoint` and `--dataplane-region`,
+respectively. Note that deploying a custom data plane is managed
+with the infrastructure instructions below.
+
+```
+  --dataplane           enable the dataplane integration
+  --dataplane-endpoint DATAPLANE_ENDPOINT
+                        endpoint for the dataplane
+  --dataplane-region DATAPLANE_REGION
+                        the AWS region name override for the Data Plane
+```
+
 __Note__: These can be configured correctly for you if you follow the guided `pitsctl` installation
 wizard.
 
 ## Usage
 
 The `pitsctl` entry point can handle three targets:
 
 - `install`: Installs or updates software and agents for running the camera control
 - `remove`: Removes all configuration, cloud resources, software and agents
 - `view`: Inpects the installation on the device
 
 ```
-Usage: pitsctl - v0.8.1: Install or manage pinthesky software
+Usage: pitsctl - v0.9.0: Install or manage pinthesky software
   -h,--help:    Prints out this help message
   -m,--host:    Client machine connection details
   -t,--text:    Enable a no color, text only view of the application
   -r,--root:    Assume root permission for management
   -l,--level:   Changes the logging verbosity for pitsctl
   -v,--version: Prints the version and exists
 ```
 
-## Control Plane and Infrastructure
+## Control/Data Plane and Infrastructure
 
 The [pits-infra][1] package can be used to deploy a complete and working 
 AWS cloud infrastructure to support the device configuration and integration.
 The infrastructure contains the following:
 
 - Storage configuration
 - Policy and device authorization
 - Control Plane deployment
+- Data Plane deployment
 - Console deployment
 - Console authorization through Cognito
 
 Follow the [re-use][2] section in the README to deploy it for at no charge
 or 50 cents a month if a custom domain is included.
 
 [1]: https://github.com/philcali/pits-infra
```

### Comparing `pinthesky-0.8.1/pinthesky/__init__.py` & `pinthesky-0.9.0/pinthesky/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 
-VERSION = "0.8.1"
+VERSION = "0.9.0"
 
 
 def set_stream_logger(name="pinthesky", level=logging.DEBUG, fmt_string=None):
     if fmt_string is None:
         fmt_string = "%(asctime)s %(name)s [%(levelname)s] %(message)s"
 
     logger = logging.getLogger(name)
```

### Comparing `pinthesky-0.8.1/pinthesky/__main__.py` & `pinthesky-0.9.0/pinthesky/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,197 +1,237 @@
 from datetime import timedelta
 
 from pinthesky import VERSION, input, output, upload, set_stream_logger
 from pinthesky.camera import CameraThread
 from pinthesky.cloudwatch import CloudWatchManager
 from pinthesky.combiner import VideoCombiner
+from pinthesky.connection import ConnectionManager, ConnectionHandler
 from pinthesky.config import ShadowConfig
 from pinthesky.events import EventThread
 from pinthesky.health import DeviceHealth
 from pinthesky.session import Session
 import argparse
 import os
 import sys
 import signal
 
 
 def create_parser():
     parser = argparse.ArgumentParser(
         description="Simple camera stream that captures motion video events")
     parser.add_argument(
-        "--log-level",
-        help="configured log level of the pinthesky app, default INFO",
-        required=False,
-        default='INFO')
-    parser.add_argument(
         "--version",
         help="displays the current version",
         action='store_true')
     parser.add_argument(
-        "--combine-dir",
-        help="the directory to combine video, defaults to motion_videos",
-        default="motion_videos")
+        "--log-level",
+        help="configured log level of the pinthesky app, default INFO",
+        required=False,
+        default='INFO')
     parser.add_argument(
+        "--health-interval",
+        help="seconds in which to emit health metrics, default: 3600",
+        default=3600,
+        type=int,
+        required=False)
+    camera = parser.add_argument_group(
+        title="Camera",
+        description="Configuration for camera options")
+    camera.add_argument(
         "--rotation",
         help="rotate the video, valid arguments [0, 90, 180, 270]",
         default=270,
         type=int)
-    parser.add_argument(
+    camera.add_argument(
         "--encoding-bitrate",
         help="the bitrate for the camera, default 17000000",
         default=17000000,
         type=int)
-    parser.add_argument(
+    camera.add_argument(
         "--encoding-profile",
         help="the camera encoding profile, default high",
         default="high")
-    parser.add_argument(
+    camera.add_argument(
         "--encoding-level",
         help="the encoding level, default 4",
         default="4")
-    parser.add_argument(
+    camera.add_argument(
         "--resolution",
         help="camera resolution, defaults 640x480",
         default="640x480")
-    parser.add_argument(
+    camera.add_argument(
         "--framerate",
         help="framerate of the camera, defaults to 20",
         type=int,
         default=20)
-    parser.add_argument(
+    camera.add_argument(
         "--buffer",
         help="buffer size in seconds, defaults to 15",
         type=int,
         default=15)
-    parser.add_argument(
+    camera.add_argument(
         "--buffer-size",
         help="buffer size in bytes, unset by default and uses buffer",
         type=int,
         required=False,
         default=None)
-    parser.add_argument(
+    camera.add_argument(
         "--sensitivity",
         help="sensitivity of the motion detection math, default 10",
         type=int,
         default=10)
-    parser.add_argument(
+    camera.add_argument(
+        "--recording-window",
+        help="the recording window for the camera relative to the host time," +
+        " ie: '08-18' for a ten hour window, defaults to always recordding",
+        required=False,
+        default=None)
+    events = parser.add_argument_group(
+        title="Events",
+        description="Configuration for reading and writing events")
+    events.add_argument(
         "--event-input",
         help="file representing external input, default input.json",
         default="input.json")
-    parser.add_argument(
+    events.add_argument(
         "--event-output",
         help="file representing external output, default output.json",
         default="output.json")
-    parser.add_argument(
+    events.add_argument(
         "--configure-input",
         help="file for configuration input, default config-input.json",
         default="config-input.json")
-    parser.add_argument(
+    events.add_argument(
         "--configure-output",
         help="file for configuration output, default config-output.json",
         default="config-output.json")
-    parser.add_argument(
+    iot = parser.add_argument_group(
+        title='AWS IoT',
+        description='Configuration for integrating with AWS IoT')
+    iot.add_argument(
         "--thing-name",
         help="the AWS IoT ThingName for use in upload",
         default=None,
         required=False)
-    parser.add_argument(
+    iot.add_argument(
         "--thing-cert",
         help="the AWS IoT certificate associated to the Thing",
         default=None,
         required=False)
-    parser.add_argument(
+    iot.add_argument(
         "--thing-key",
         help="the AWS IoT certificate pair associated to the Thing",
         default=None,
         required=False)
-    parser.add_argument(
+    iot.add_argument(
         "--ca-cert",
         help="the root CA certificate to authenticate the certificate",
         default=None,
         required=False)
-    parser.add_argument(
+    iot.add_argument(
         "--credentials-endpoint",
         help="the AWS IoT Credentials Provider endpoint",
         default=None,
         required=False)
-    parser.add_argument(
+    iot.add_argument(
         "--role-alias",
         help="the AWS IoT Role Alias to pull credentials",
         default=None,
         required=False)
-    parser.add_argument(
+    iot.add_argument(
+        "--shadow-update",
+        help="behavior for the camera shadow document: always, never, empty",
+        default="empty",
+        required=False)
+    storage = parser.add_argument_group(
+        title="Storage",
+        description="Configuration for remote storage")
+    storage.add_argument(
         "--bucket-name",
         help="the S3 bucket to upload motion detection files",
         default=None,
         required=False)
-    parser.add_argument(
+    storage.add_argument(
         "--bucket-prefix",
         help="the prefix to upload the motion files to, default motion_videos",
         default="motion_videos")
-    parser.add_argument(
-        "--recording-window",
-        help="the recording window for the camera relative to the host time," +
-        " ie: '08-18' for a ten hour window, defaults to always recordding",
-        required=False,
-        default=None)
-    parser.add_argument(
+    storage.add_argument(
         "--capture-dir",
         help="the directory to write temporary images, default capture_images",
         default="capture_images",
         required=False)
-    parser.add_argument(
+    storage.add_argument(
         "--bucket-image-prefix",
         help="the prefix to upload the latest images, default capture_images",
         default="capture_images",
         required=False)
-    parser.add_argument(
+    storage.add_argument(
+        "--combine-dir",
+        help="the directory to combine video, defaults to motion_videos",
+        default="motion_videos")
+    cloudwatch = parser.add_argument_group(
+        title="CloudWatch",
+        description="Configuration for CloudWatch logging")
+    cloudwatch.add_argument(
         "--cloudwatch",
         help="enable the cloudwatch upload, default false",
         required=False,
         default=os.getenv("CLOUDWATCH", "false") == "true",
         action='store_true')
-    parser.add_argument(
+    cloudwatch.add_argument(
+        "--cloudwatch-region",
+        help="the AWS region name override for CloudWatch",
+        default=os.getenv("AWS_DEFAULT_REGION", None),
+        required=False)
+    cloudwatch.add_argument(
         "--cloudwatch-thread",
         action='store_true',
         default=os.getenv("CLOUDWATCH_THREADED", "false") == "true",
         required=False,
         help="enable cloudwatch logs to upload in background, default false")
-    parser.add_argument(
+    cloudwatch.add_argument(
         "--cloudwatch-event-type",
         default="logs",
         required=False,
         help="event type to upload: logs,emf,all")
-    parser.add_argument(
+    cloudwatch.add_argument(
         "--cloudwatch-metric-namespace",
         required=False,
         default="Pits/Device",
         help="metric namespace when using emf event type, default Pits/Device")
-    parser.add_argument(
+    cloudwatch.add_argument(
         "--cloudwatch-log-group",
         help="uploads to this cloudwatch log group",
         default=None,
         required=False)
-    parser.add_argument(
+    cloudwatch.add_argument(
         "--disable-cloudwatch-stream-split",
         help="disables splitting the log stream by thing name",
         default=os.getenv("CLOUDWATCH_DELINEATE_STREAM", "true") == "false",
         required=False,
         action='store_true')
-    parser.add_argument(
-        "--shadow-update",
-        help="behavior for the camera shadow document: always, never, empty",
-        default="empty",
-        required=False)
-    parser.add_argument(
-        "--health-interval",
-        help="seconds in which to emit health metrics, default: 3600",
-        default=3600,
-        type=int,
-        required=False)
+    dataplane = parser.add_argument_group(
+        title="Data Plane",
+        description="Configuration for the data plane integration")
+    dataplane.add_argument(
+        "--dataplane",
+        help="enable the dataplane integration",
+        required=False,
+        default=os.getenv("DATAPLANE", "false") == "true",
+        action='store_true')
+    dataplane.add_argument(
+        "--dataplane-endpoint",
+        help="endpoint for the dataplane",
+        required=False,
+        default=None)
+    dataplane.add_argument(
+        "--dataplane-region",
+        help="the AWS region name override for the Data Plane",
+        required=False,
+        default=os.getenv("AWS_DEFAULT_REGION", None))
     return parser
 
 
 def main():
     parsed = create_parser().parse_args(sys.argv[1:])
     if parsed.version:
         print(VERSION)
@@ -208,14 +248,20 @@
     auth_session = Session(
         cacert_path=parsed.ca_cert,
         cert_path=parsed.thing_cert,
         key_path=parsed.thing_key,
         role_alias=parsed.role_alias,
         thing_name=parsed.thing_name,
         credentials_endpoint=parsed.credentials_endpoint)
+    connection_manager = ConnectionManager(
+        session=auth_session,
+        enabled=parsed.dataplane,
+        endpoint_url=parsed.dataplane_endpoint,
+        region_name=parsed.dataplane_region)
+    connection_handler = ConnectionHandler(manager=connection_manager)
     video_uploader = upload.S3Upload(
         events=event_thread,
         bucket_name=parsed.bucket_name,
         bucket_prefix=parsed.bucket_prefix,
         bucket_image_prefix=parsed.bucket_image_prefix,
         session=auth_session)
     camera_thread = CameraThread(
@@ -226,46 +272,51 @@
         rotation=parsed.rotation,
         framerate=parsed.framerate,
         encoding_bitrate=parsed.encoding_bitrate,
         encoding_level=parsed.encoding_level,
         encoding_profile=parsed.encoding_profile,
         recording_window=parsed.recording_window,
         capture_dir=parsed.capture_dir,
-        buffer_size=parsed.buffer_size)
+        buffer_size=parsed.buffer_size,
+        connection_manager=connection_manager)
     video_combiner = VideoCombiner(
         events=event_thread,
         combine_dir=parsed.combine_dir)
     event_input_handler = input.InputHandler(events=event_thread)
     cloudwatch_manager = CloudWatchManager(
         session=auth_session,
         log_level=parsed.log_level,
         delineate_stream=not parsed.disable_cloudwatch_stream_split,
         threaded=parsed.cloudwatch_thread,
         enabled=parsed.cloudwatch,
         log_group_name=parsed.cloudwatch_log_group,
         namespace=parsed.cloudwatch_metric_namespace,
-        event_type=parsed.cloudwatch_event_type)
+        event_type=parsed.cloudwatch_event_type,
+        region_name=parsed.cloudwatch_region)
     event_thread.on(camera_thread)
     event_thread.on(video_combiner)
     event_thread.on(video_uploader)
     event_thread.on(event_output)
     event_thread.on(event_input_handler)
     event_thread.on(auth_session)
     event_thread.on(device_health)
     event_thread.on(cloudwatch_manager)
+    event_thread.on(connection_manager)
+    event_thread.on(connection_handler)
     shadow_update = ShadowConfig(
         events=event_thread,
         configure_input=parsed.configure_input,
         configure_output=parsed.configure_output)
     event_thread.on(shadow_update)
     shadow_update.add_handler(camera_thread)
     shadow_update.add_handler(auth_session)
     shadow_update.add_handler(device_health)
     shadow_update.add_handler(cloudwatch_manager)
     shadow_update.add_handler(video_uploader)
+    shadow_update.add_handler(connection_manager)
     # Allow adaptation before shadow document kicks in
     cloudwatch_manager.adapt_logging()
 
     if not shadow_update.update_document(parsed):
         shadow_update.reset_from_document()
     notify_thread.notify_change(parsed.event_input)
     notify_thread.notify_change(parsed.configure_output, persist=True)
```

### Comparing `pinthesky-0.8.1/pinthesky/camera.py` & `pinthesky-0.9.0/pinthesky/camera.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,29 @@
 from datetime import datetime
+from collections import namedtuple
 from pinthesky.config import ConfigUpdate, ShadowConfigHandler
 from pinthesky.handler import Handler
 from pinthesky.health import DeviceHealth
+from pinthesky.conversion import VideoConversion, JSMPEGHeader
+from pinthesky.connection import ProcessBuffer, ConnectionThread
 import logging
 import time
 import threading
 
 
 logger = logging.getLogger(__name__)
 
 
+CameraConfig = namedtuple('CameraConfig', [
+    'rotation',
+    'framerate',
+    'resolution'
+])
+
+
 class CameraThread(threading.Thread, Handler, ShadowConfigHandler):
     """
     A thread that manages a picamera.PiCamera instance.
     """
     def __init__(
             self, events, sensitivity=10, resolution=(640, 480),
             framerate=20, rotation=270, buffer=15, recording_window=None,
@@ -21,35 +31,40 @@
             encoding_profile='high',
             encoding_level="4",
             camera_class=None,
             stream_class=None,
             motion_detection_class=None,
             capture_dir=None,
             device_health=None,
-            buffer_size=None):
+            buffer_size=None,
+            connection_manager=None):
         super().__init__(daemon=True)
         self.__camera_class = camera_class
         self.__stream_class = stream_class
         self.__motion_detection_class = motion_detection_class
         self.running = True
         self.flushing_stream = False
         self.flushing_ts = None
         self.flushing_buffer = None
         self.flushing_trigger = None
+        self.recording_thread = None
+        self.connection_manager = connection_manager
         self.buffer_size = buffer_size
         self.events = events
         self.buffer = buffer
         self.sensitivity = sensitivity
         self.encoding_bitrate = encoding_bitrate
         self.encoding_profile = encoding_profile
         self.encoding_level = encoding_level
+        self.camera_props = CameraConfig(
+            resolution=resolution,
+            rotation=rotation,
+            framerate=framerate
+        )
         self.camera = self.__new_camera()
-        self.camera.resolution = resolution
-        self.camera.framerate = framerate
-        self.camera.rotation = rotation
         self.historical_stream = self.__new_stream_buffer()
         self.recording_window = recording_window
         self.capture_dir = capture_dir
         self.device_health = device_health
         if self.device_health is None:
             self.device_health = DeviceHealth(events=events)
         self.configuration_lock = threading.Lock()
@@ -78,37 +93,77 @@
             kwargs['seconds'] = self.buffer // 2
         return self.__stream_class(self.camera, **kwargs)
 
     def __new_camera(self):
         if self.__camera_class is None:
             from picamera import PiCamera
             self.__camera_class = PiCamera
-        return self.__camera_class()
+        camera = self.__camera_class()
+        for prop, value in self.camera_props._asdict().items():
+            setattr(camera, prop, value)
+        return camera
 
-    def on_capture_image(self, event):
-        result = f'{self.capture_dir}/img-{event["timestamp"]}.jpg'
-        if 'file_name' in event:
-            result = f'{self.capture_dir}/{event["file_name"]}'
-        self.camera.capture(result, use_video_port=True)
-        logger.debug(f'Capture to {result}')
-        self.events.fire_event('capture_image_end', {
-            'image_file': result,
-            'start_time': event['timestamp']
-        })
+    def __update_fields_on(self, on_obj, cam_obj, fields):
+        self_types = {
+            "buffer": int,
+            "buffer_size": int,
+            "sensitivity": int,
+            "encoding_bitrate": int,
+            "rotation": int,
+            "framerate": int
+        }
+
+        def identity(x):
+            return x
+
+        for field in fields:
+            if field in cam_obj:
+                value = cam_obj[field]
+                value = self_types.get(field, identity)(value)
+                if field == "resolution":
+                    value = tuple(map(int, value.split("x")))
+                setattr(on_obj, field, value)
+                if field == "recording_window":
+                    self.__set_recording_window()
 
     def __flush_start(self, trigger, event):
         if not self.flushing_stream:
             logger.info(
                 f'Starting a flush on {trigger} video from {event["timestamp"]}')
             self.flushing_ts = event['timestamp']
             self.flushing_buffer = self.buffer
             if 'duration' in event:
                 self.flushing_buffer = event['duration']
             self.flushing_stream = True
             self.flushing_trigger = trigger
+            self.flushing_event = event
+
+    def on_capture_image(self, event):
+        result = f'{self.capture_dir}/img-{event["timestamp"]}.jpg'
+        if 'file_name' in event:
+            result = f'{self.capture_dir}/{event["file_name"]}'
+        self.camera.capture(result, use_video_port=True)
+        logger.debug(f'Capture to {result}')
+        self.events.fire_event('capture_image_end', {
+            'image_file': result,
+            'start_time': event['timestamp'],
+            **event,
+        })
+
+    def on_record(self, event):
+        with self.configuration_lock:
+            if event['session']['start']:
+                self.pause()
+                self.record(event)
+            elif event['session']['stop']:
+                self.pause()
+
+    def on_record_end(self, event):
+        with self.configuration_lock:
+            self.pause()
 
     def on_motion_start(self, event):
         self.__flush_start('motion', event)
 
     def on_capture_video(self, event):
         # Make sure to lock on other configuration changes before mutating camera state
         with self.configuration_lock:
@@ -126,101 +181,109 @@
             'recording_window': self.recording_window,
             'encoding_level': self.encoding_level,
             'encoding_profile': self.encoding_profile,
             'encoding_bitrate': self.encoding_bitrate
         })
 
     def on_file_change(self, event):
-        self_types = {
-            "buffer": int,
-            "buffer_size": int,
-            "sensitivity": int,
-            "encoding_bitrate": int,
-            "rotation": int,
-            "framerate": int
-        }
-
-        def identity(x):
-            return x
-
-        def set_fields_on(cam_obj, on_obj, fields):
-            for field in fields:
-                if field in cam_obj:
-                    value = cam_obj[field]
-                    value = self_types.get(field, identity)(value)
-                    if field == "resolution":
-                        value = tuple(map(int, value.split("x")))
-                    setattr(on_obj, field, value)
-                    if field == "recording_window":
-                        self.__set_recording_window()
-
         if "current" in event["content"]:
             cam_obj = event["content"]["current"]["state"]["desired"]["camera"]
             logger.info(f'Update camera fields in {cam_obj}')
             # Hold potentially dangerous mutations if the camera is flushing
             with self.configuration_lock:
+                # Pause any active recording on config update
                 previsouly_recording = self.pause()
+                # Update picamera fields using older resident properties
+                self.__update_fields_on(
+                    on_obj=self.camera,
+                    cam_obj=cam_obj,
+                    fields=["rotation", "resolution", "framerate"],
+                )
+                # Update resident properties for dynamic pauses
+                self.camera_props = CameraConfig(
+                    rotation=self.camera.rotation,
+                    framerate=self.camera.framerate,
+                    resolution=self.camera.resolution,
+                )
                 # Update wrapper fields
-                set_fields_on(on_obj=self, cam_obj=cam_obj, fields=[
+                self.__update_fields_on(on_obj=self, cam_obj=cam_obj, fields=[
                     "buffer",
                     "buffer_size",
                     "sensitivity",
                     "recording_window",
                     "encoding_bitrate",
                     "encoding_profile",
                     "encoding_level"
                 ])
-                # Update picamera fields
-                set_fields_on(on_obj=self.camera, cam_obj=cam_obj, fields=[
-                    "rotation", "resolution", "framerate"
-                ])
                 if previsouly_recording:
                     self.resume()
 
     def __flush_video(self):
         # Want to flush when it is safe to flush
         with self.configuration_lock:
             self.camera.split_recording(f'{self.flushing_ts}.after.h264')
             self.historical_stream.copy_to(f'{self.flushing_ts}.before.h264')
             self.historical_stream.clear()
             logger.debug("Flushed buffered contents")
             time.sleep(self.flushing_buffer)
             self.camera.split_recording(self.historical_stream)
             self.events.fire_event('flush_end', {
                 'start_time': self.flushing_ts,
-                'trigger': self.flushing_trigger
+                'trigger': self.flushing_trigger,
+                **self.flushing_event,
             })
             self.flushing_stream = False
 
+    def __enable_default_recording(self):
+        return (
+            self.recording_thread is None and
+            not self.flushing_stream and
+            self.recording_window
+        )
+
     def run(self):
         logger.info('Starting camera thread')
-        self.resume()
         while self.running:
             self.device_health.emit_health(force=False)
             # Configuration lock will prevent a race on "resume" from update
             with self.configuration_lock:
-                if not self.flushing_stream and self.recording_window:
+                if self.__enable_default_recording():
                     now = datetime.now()
                     if now.hour < self.start_hour or now.hour > self.end_hour:
                         self.pause()
                         time.sleep(1)
                         continue
                     else:
                         self.resume()
-            self.camera.wait_recording(1)
-            if self.flushing_stream:
-                self.__flush_video()
+            try:
+                self.camera.wait_recording(1)
+                if self.flushing_stream:
+                    self.__flush_video()
+            except Exception as e:
+                logger.warning(
+                    'Camera surfaced exception on failure:',
+                    exc_info=e
+                )
+                self.pause()
 
     def pause(self):
-        if self.camera.recording:
-            self.camera.stop_recording()
+        if self.camera.recording or self.recording_thread is not None:
+            # Have to tear down camera completely to reinstall encoders
+            try:
+                self.camera.close()
+            except Exception as e:
+                logger.warning(f'Failed to close, but killed the camera {e}')
+            if self.recording_thread is not None:
+                self.recording_thread.join()
+                self.recording_thread = None
             logger.info("Camera recording is now paused")
             self.events.fire_event('recording_change', {
                 'recording': False
             })
+            self.camera = self.__new_camera()
             return True
         return False
 
     def resume(self):
         if not self.camera.recording:
             self.historical_stream = self.__new_stream_buffer()
             self.camera.start_recording(
@@ -233,11 +296,32 @@
             logger.info("Camera is now recording")
             self.events.fire_event('recording_change', {
                 'recording': True
             })
             return True
         return False
 
+    def record(self, event):
+        if not self.camera.recording:
+            # Recording event was initated with a valid session connection
+            # Pump the magic header into the connection for streaming
+            JSMPEGHeader(self.connection_manager, event, self.camera).send()
+            conversion = VideoConversion(self.camera)
+            self.recording_thread = ConnectionThread(
+                buffer=ProcessBuffer(conversion.process),
+                manager=self.connection_manager,
+                events=self.events,
+                event_data=event,
+            )
+            self.camera.start_recording(conversion, 'yuv')
+            self.recording_thread.start()
+            logger.info("Camera is now live recording")
+            self.events.fire_event('recording_change', {
+                'recording': True
+            })
+            return True
+        return False
+
     def stop(self):
         self.running = False
-        self.camera.stop_recording()
+        self.pause()
         self.camera.close()
```

### Comparing `pinthesky-0.8.1/pinthesky/cloudwatch.py` & `pinthesky-0.9.0/pinthesky/cloudwatch.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,23 +23,25 @@
             session=None,
             log_group_name=None,
             log_level=logging.INFO,
             enabled=False,
             delineate_stream=True,
             threaded=False,
             namespace='Pits/Device',
-            event_type='logs'):
+            event_type='logs',
+            region_name=None):
         self.session = session
         self.log_group_name = log_group_name
         self.log_level = log_level
         self.enabled = enabled
         self.delineate_stream = delineate_stream
         self.namespace = namespace
         self.threaded = threaded
         self.event_type = event_type
+        self.region_name = region_name
         self.event_handler = None
         self.log_handler = None
         self.log_thread = None
         self.refresh_lock = threading.Lock()
 
     def adapt_logging(self):
         with self.refresh_lock:
@@ -53,15 +55,16 @@
             if self.log_thread is not None:
                 self.log_thread.stop()
                 self.log_thread = None
             log_stream = CloudWatchLoggingStream(
                 delineate_stream=self.delineate_stream,
                 enabled=self.enabled,
                 log_group_name=self.log_group_name,
-                session=self.session)
+                session=self.session,
+                region_name=self.region_name)
             # Create handler that writes logs to CW
             if self.log_handler is not None:
                 root.removeHandler(self.log_handler)
                 self.log_handler = None
             self.log_handler = logging.StreamHandler(stream=log_stream)
             self.log_handler.setFormatter(
                 logging.Formatter(
@@ -79,41 +82,51 @@
             if self.enabled and self.threaded:
                 # Replace stream to be backed by thread
                 self.log_thread = ThreadedStream(stream=log_stream)
                 self.log_handler.setStream(self.log_thread)
                 self.event_handler.setStream(self.log_thread)
                 self.log_thread.start()
             # Enable Logs, EMF, or both
+            logs_enabled = False
+            emf_enabled = False
             if self.enabled and self.event_type in ['logs', 'all']:
                 root.addHandler(self.log_handler)
+                logs_enabled = True
             if self.enabled and self.event_type in ['emf', 'all']:
                 root.addHandler(self.event_handler)
+                emf_enabled = True
+            if not logs_enabled:
+                self.log_handler = None
+            if not emf_enabled:
+                self.event_handler = None
 
     def update_document(self) -> ConfigUpdate:
         return ConfigUpdate('cloudwatch', {
             'threaded': self.threaded,
             'enabled': self.enabled,
             'delineate_stream': self.delineate_stream,
             'log_group_name': self.log_group_name,
             'metric_namespace': self.namespace,
             'log_level': logging.getLevelName(self.log_level),
             'event_type': self.event_type,
+            'region_name': self.region_name,
         })
 
     def on_file_change(self, event):
         if "current" in event["content"]:
             desired = event["content"]["current"]["state"]["desired"]
             cloudwatch = desired.get("cloudwatch", {})
             self.enabled = cloudwatch.get("enabled", self.enabled)
             self.threaded = cloudwatch.get("threaded", self.threaded)
             self.delineate_stream = cloudwatch.get("delineate_stream", self.delineate_stream)
             self.log_group_name = cloudwatch.get("log_group_name", self.log_group_name)
             self.namespace = cloudwatch.get("metric_namespace", self.namespace)
             self.event_type = cloudwatch.get("event_type", self.event_type)
             self.log_level = cloudwatch.get("log_level", self.log_level)
+            self.region_name = cloudwatch.get("region_name", self.region_name)
             self.adapt_logging()
 
     def stop(self):
         if self.log_thread is not None:
             self.log_thread.stop()
 
 
@@ -129,20 +142,22 @@
     logging.getLogger(__name__).addHandler(handler)
     """
     def __init__(
             self,
             session=None,
             log_group_name=None,
             enabled=False,
-            delineate_stream=True):
+            delineate_stream=True,
+            region_name=None):
         self.session = session
         self.log_group_name = log_group_name
         self.log_stream_name = None
         self.enabled = enabled
         self.delineate_stream = delineate_stream
+        self.region_name = region_name
 
     def _log_stream_name(self, now, cloudwatch):
         month = f'0{now.month}' if now.month < 10 else now.month
         day = f'0{now.day}' if now.day < 10 else now.day
         desired_stream = f'{now.year}/{month}/{day}'
         if self.delineate_stream and self.session.thing_name is not None:
             desired_stream += f'@{self.session.thing_name}'
@@ -166,15 +181,15 @@
         if not self.enabled or not credentials or not self.log_group_name:
             return
         now = ingest if ingest is not None else datetime.datetime.now()
         session = boto3.Session(
             credentials['accessKeyId'],
             credentials['secretAccessKey'],
             credentials['sessionToken'])
-        cloudwatch = session.client('logs')
+        cloudwatch = session.client('logs', region_name=self.region_name)
         log_stream_name = self._log_stream_name(now, cloudwatch)
         cloudwatch.put_log_events(
             logGroupName=self.log_group_name,
             logStreamName=log_stream_name,
             logEvents=[
                 {
                     'message': message.rstrip('\n'),
```

### Comparing `pinthesky-0.8.1/pinthesky/combiner.py` & `pinthesky-0.9.0/pinthesky/combiner.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,10 +31,10 @@
                 part_name = f'{event["start_time"]}.{n}.h264'
                 with open(part_name, 'rb') as i:
                     o.write(i.read())
                 os.remove(part_name)
         self.events.fire_event('combine_end', {
             'start_time': event['start_time'],
             'combine_video': file_name,
-            'trigger': event['trigger'],
+            **event,
         })
         logger.debug(f'Finish concatinating to {file_name}')
```

### Comparing `pinthesky-0.8.1/pinthesky/config.py` & `pinthesky-0.9.0/pinthesky/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,31 +56,41 @@
             with open(self.__configure_output, 'r') as f:
                 content = json.loads(f.read())
                 self.__events.fire_event('file_change', {
                     'file_name': self.__configure_output,
                     'content': content
                 })
 
+    def generate_document(self):
+        resulting_document = {}
+        for handler in self.__handlers:
+            rval = handler.update_document()
+            if rval is not None:
+                resulting_document[rval.name] = rval.body
+        return resulting_document
+
     def update_document(self, parser):
         if self.__should_update(parser.shadow_update):
-            resulting_document = {}
-            for handler in self.__handlers:
-                rval = handler.update_document()
-                if rval is not None:
-                    resulting_document[rval.name] = rval.body
+            resulting_document = self.generate_document()
             if len(resulting_document) == 0:
                 logger.info('There was no update, Skipping.')
                 return False
             logger.info(f'Updating config document with {resulting_document}')
             with open(self.__configure_input, 'w') as f:
                 f.write(json.dumps(resulting_document))
             logger.info(f'Successfully updated {self.__configure_input}')
             return True
         return False
 
+    def on_configuration(self, event):
+        self.__events.fire_event('configuration_end', {
+            'configuration': self.generate_document(),
+            **event,
+        })
+
     def on_file_change(self, event):
         if event['file_name'] == self.__configure_output:
             if os.path.getsize(self.__configure_input) > 0:
                 logger.info(f'Truncating {self.__configure_input}')
                 # TODO: probably want to lock on it
                 with open(self.__configure_input, 'w') as f:
                     f.write("")
```

### Comparing `pinthesky-0.8.1/pinthesky/events.py` & `pinthesky-0.9.0/pinthesky/events.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,19 @@
     'upload_end',
     'file_change',
     'capture_image',
     'capture_image_end',
     'capture_video',
     'recording_change',
     'health',
-    'health_end'
+    'health_end',
+    'configuration',
+    'configuration_end',
+    'record',
+    'record_end',
 ]
 
 
 class EventThread(threading.Thread):
     """
     This thread wraps a queue to flush events sequentially. A Handler could be
     added, or more general anonymous functions.
@@ -31,17 +35,22 @@
     def __init__(self):
         super().__init__(daemon=True)
         self.event_queue = queue.Queue()
         self.running = True
         self.handlers = {}
 
     def on(self, handler: Handler):
+        base_handler = Handler()
         for event_name in event_names:
             method_name = f'on_{event_name}'
             method = getattr(handler, method_name)
+            handler_method = getattr(base_handler, method_name)
+            if method.__func__ is handler_method.__func__:
+                logger.debug(f'Skipping {handler.__class__.__name__}:{method_name}')
+                continue
             self.on_event(
                 event_name=event_name,
                 handler=partial(method),
                 handler_name=handler.__class__.__name__)
 
     def on_event(self, event_name, handler, handler_name):
         if event_name not in self.handlers:
```

### Comparing `pinthesky-0.8.1/pinthesky/handler.py` & `pinthesky-0.9.0/pinthesky/handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,7 +85,31 @@
         - `disk_used`: disk used in bytes
         - `disk_total`: disk total in bytes
         - `mem_free`: memory free in KB
         - `mem_avail`: memory available in KB
         - `mem_total`: memory total in KB
         """
         pass
+
+    def on_configuration(self, event):
+        """
+        Signal to read configuration out of daemon memory.
+        """
+        pass
+
+    def on_configuration_end(self, event):
+        """
+        Event containing configuration data pulled from the device.
+        """
+        pass
+
+    def on_record(self, event):
+        """
+        Event containing configuration for a live recording.
+        """
+        pass
+
+    def on_record_end(self, event):
+        """
+        Event containing configuration for ending a live recording.
+        """
+        pass
```

### Comparing `pinthesky-0.8.1/pinthesky/health.py` & `pinthesky-0.9.0/pinthesky/health.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,33 +134,36 @@
 
     def on_flush_end(self, event):
         self.motion_captured += 1
 
     def on_recording_change(self, event):
         self.recording_status = event["recording"]
 
-    def __flush_metrics(self):
+    def __flush_metrics(self, parent_event={}):
         p_vs = sys.version_info
         context = {
             'version': VERSION,
             'python_version': f'{p_vs.major}.{p_vs.minor}.{p_vs.micro}',
             'motion_captured': self.motion_captured,
             'recording_status': self.recording_status,
         }
         for metric in self.metrics:
             context = dict(context, **metric.report())
-        self.events.fire_event('health_end', context)
+        self.events.fire_event('health_end', {
+            **parent_event,
+            **context,
+        })
         self.last_flush_time = datetime.utcnow()
         logger.debug('Emitted health metric data')
         return context
 
     def emit_health(self, force=False):
         with self.emit_health_lock:
             now = datetime.utcnow()
             if force or now - self.last_flush_time > self.flush_delta:
                 self.__flush_metrics()
                 return True
         return False
 
     def on_health(self, event):
         with self.emit_health_lock:
-            self.__flush_metrics()
+            self.__flush_metrics(event)
```

### Comparing `pinthesky-0.8.1/pinthesky/input.py` & `pinthesky-0.9.0/pinthesky/input.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         if file_name is not None and os.path.exists(file_name):
             with open(file_name, 'r') as f:
                 content = f.read()
                 if content == "":
                     logger.debug(f'The {file_name} was zeroed out. Skipping.')
                     return
                 js = json.loads(content)
+                logger.debug(f'Input data is {js}')
                 self.events.fire_event('file_change', {
                     'file_name': file_name,
                     'content': js
                 })
             if not self.persist_handles[file_name]:
                 with open(file_name, 'w') as f:
                     f.write("")
```

### Comparing `pinthesky-0.8.1/pinthesky/motion_detect.py` & `pinthesky-0.9.0/pinthesky/motion_detect.py`

 * *Files identical despite different names*

### Comparing `pinthesky-0.8.1/pinthesky/output.py` & `pinthesky-0.9.0/pinthesky/output.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,10 +28,13 @@
 
     def on_upload_end(self, event):
         self.__on_event(event)
 
     def on_health_end(self, event):
         self.__on_event(event)
 
+    def on_configuration_end(self, event):
+        self.__on_event(event)
+
     def reset(self):
         with open(self.output_file, 'w') as f:
             f.write("")
```

### Comparing `pinthesky-0.8.1/pinthesky/session.py` & `pinthesky-0.9.0/pinthesky/session.py`

 * *Files identical despite different names*

### Comparing `pinthesky-0.8.1/pinthesky/upload.py` & `pinthesky-0.9.0/pinthesky/upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
                         emf['UploadProcessed'] = 1
                         self.events.fire_event('upload_end', {
                             'start_time': source['start_time'],
                             'upload': {
                                 'bucket_name': self.bucket_name,
                                 'bucket_key': loc
                             },
-                            'source': source
+                            **source,
                         })
                     end_timestamp = floor(time.time())
                     emf['Time'] = end_timestamp - source['start_time']
                     logger.info(f'Uploaded to s3://{self.bucket_name}/{loc}', extra={
                         'emf': emf,
                     })
             except RuntimeError as e:
```

### Comparing `pinthesky-0.8.1/pinthesky.egg-info/PKG-INFO` & `pinthesky-0.9.0/pinthesky.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinthesky
-Version: 0.8.1
+Version: 0.9.0
 Summary: Simple Pi In The Sky device Integration
 Home-page: https://github.com/philcali/pits-device
 Author: Philip Cali
 Author-email: philip.cali@gmail.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -159,55 +159,73 @@
 `--cloudwatch-event-type emf`. The daemon will manage the `LogStream`
 associated to the `LogGroup`, by "{year}/{month}/{day}". It will
 delineate the stream by `thing_name`. To disable this behavior, use
 `--disable-cloudwatch-stream-split`.
 
 ```
   --cloudwatch          enable the cloudwatch upload, default false
+  --cloudwatch-region CLOUDWATCH_REGION
+                        the AWS region name override for CloudWatch
   --cloudwatch-thread   enable cloudwatch logs to upload in background, default false
   --cloudwatch-event-type CLOUDWATCH_EVENT_TYPE
                         event type to upload: logs,emf,all
   --cloudwatch-metric-namespace CLOUDWATCH_METRIC_NAMESPACE
                         metric namespace when using emf event type, default Pits/Device
   --cloudwatch-log-group CLOUDWATCH_LOG_GROUP
                         uploads to this cloudwatch log group
   --disable-cloudwatch-stream-split
                         disables splitting the log stream by thing name
 ```
 
+The `pinthesky` daemon supports live streaming through an optional
+integration through a custom data plane deployed through [pits-data](https://github.com/philcali/pits-data). Enabling this integration
+is done through `--dataplane` and the endpoint and AWS region are
+targeted with `--dataplane-endpoint` and `--dataplane-region`,
+respectively. Note that deploying a custom data plane is managed
+with the infrastructure instructions below.
+
+```
+  --dataplane           enable the dataplane integration
+  --dataplane-endpoint DATAPLANE_ENDPOINT
+                        endpoint for the dataplane
+  --dataplane-region DATAPLANE_REGION
+                        the AWS region name override for the Data Plane
+```
+
 __Note__: These can be configured correctly for you if you follow the guided `pitsctl` installation
 wizard.
 
 ## Usage
 
 The `pitsctl` entry point can handle three targets:
 
 - `install`: Installs or updates software and agents for running the camera control
 - `remove`: Removes all configuration, cloud resources, software and agents
 - `view`: Inpects the installation on the device
 
 ```
-Usage: pitsctl - v0.8.1: Install or manage pinthesky software
+Usage: pitsctl - v0.9.0: Install or manage pinthesky software
   -h,--help:    Prints out this help message
   -m,--host:    Client machine connection details
   -t,--text:    Enable a no color, text only view of the application
   -r,--root:    Assume root permission for management
   -l,--level:   Changes the logging verbosity for pitsctl
   -v,--version: Prints the version and exists
 ```
 
-## Control Plane and Infrastructure
+## Control/Data Plane and Infrastructure
 
 The [pits-infra][1] package can be used to deploy a complete and working 
 AWS cloud infrastructure to support the device configuration and integration.
 The infrastructure contains the following:
 
 - Storage configuration
 - Policy and device authorization
 - Control Plane deployment
+- Data Plane deployment
 - Console deployment
 - Console authorization through Cognito
 
 Follow the [re-use][2] section in the README to deploy it for at no charge
 or 50 cents a month if a custom domain is included.
 
 [1]: https://github.com/philcali/pits-infra
```

### Comparing `pinthesky-0.8.1/pinthesky.egg-info/SOURCES.txt` & `pinthesky-0.9.0/pinthesky.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 setup.py
 pinthesky/__init__.py
 pinthesky/__main__.py
 pinthesky/camera.py
 pinthesky/cloudwatch.py
 pinthesky/combiner.py
 pinthesky/config.py
+pinthesky/connection.py
+pinthesky/conversion.py
 pinthesky/events.py
 pinthesky/handler.py
 pinthesky/health.py
 pinthesky/input.py
 pinthesky/motion_detect.py
 pinthesky/output.py
 pinthesky/session.py
@@ -22,13 +24,14 @@
 pinthesky.egg-info/entry_points.txt
 pinthesky.egg-info/requires.txt
 pinthesky.egg-info/top_level.txt
 tests/test_camera.py
 tests/test_cloudwatch.py
 tests/test_combiner.py
 tests/test_config.py
+tests/test_connection.py
 tests/test_handler.py
 tests/test_health.py
 tests/test_input.py
 tests/test_output.py
 tests/test_session.py
 tests/test_upload.py
```

### Comparing `pinthesky-0.8.1/setup.cfg` & `pinthesky-0.9.0/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pinthesky
-version = 0.8.1
+version = 0.9.0
 author = philcali
 author_email = philcali@gmail.com
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/philcali/pits-device
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `pinthesky-0.8.1/setup.py` & `pinthesky-0.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="pinthesky",
-    version="0.8.1",
+    version="0.9.0",
     description="Simple Pi In The Sky device Integration",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Philip Cali",
     author_email="philip.cali@gmail.com",
     url="https://github.com/philcali/pits-device",
     license="Apache License 2.0",
```

### Comparing `pinthesky-0.8.1/tests/test_camera.py` & `pinthesky-0.9.0/tests/test_camera.py`

 * *Files identical despite different names*

### Comparing `pinthesky-0.8.1/tests/test_cloudwatch.py` & `pinthesky-0.9.0/tests/test_cloudwatch.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,16 @@
                         'cloudwatch': {
                             'enabled': True,
                             'threaded': True,
                             'log_group_name': None,
                             'metric_namespace': 'Pits/Devices',
                             'log_level': 'FARTS',
                             'delineate_stream': True,
-                            'event_type': 'all'
+                            'event_type': 'all',
+                            'region_name': 'us-east-2',
                         }
                     }
                 }
             }
         }
     })
     events.event_queue.join()
@@ -88,37 +89,41 @@
         'enabled': True,
         'threaded': True,
         'delineate_stream': True,
         'metric_namespace': 'Pits/Devices',
         'event_type': 'all',
         'log_level': 'INFO',
         'log_group_name': None,
+        'region_name': 'us-east-2',
     })
 
     events.fire_event('file_change', {
         'content': {
             'current': {
                 'state': {
                     'desired': {
                         'cloudwatch': {
                             'enabled': False,
                             'threaded': False,
                             'log_group_name': None,
                             'metric_namespace': 'Pits/Devices',
                             'log_level': 'FARTS',
                             'delineate_stream': True,
-                            'event_type': 'all'
+                            'event_type': 'all',
+                            'region_name': None,
                         }
                     }
                 }
             }
         }
     })
     events.event_queue.join()
     assert manager.log_thread is None
+    assert manager.log_handler is None
+    assert manager.event_handler is None
     assert len(root.handlers) == handler_length
 
 
 def test_cloudwatch_event_filter():
     filterer = logging.Filterer()
     filterer.addFilter(CloudWatchEventFilter())
```

### Comparing `pinthesky-0.8.1/tests/test_combiner.py` & `pinthesky-0.9.0/tests/test_combiner.py`

 * *Files identical despite different names*

### Comparing `pinthesky-0.8.1/tests/test_config.py` & `pinthesky-0.9.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pinthesky-0.8.1/tests/test_health.py` & `pinthesky-0.9.0/tests/test_health.py`

 * *Files identical despite different names*

### Comparing `pinthesky-0.8.1/tests/test_input.py` & `pinthesky-0.9.0/tests/test_input.py`

 * *Files identical despite different names*

### Comparing `pinthesky-0.8.1/tests/test_output.py` & `pinthesky-0.9.0/tests/test_output.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,13 +21,13 @@
     notify.start()
     for event_name in event_names:
         events.fire_event(event_name=event_name, context={
             "file_name": test_output
         })
         time.sleep(0.01)
     try:
-        assert client.calls['file_change'] == 3
+        assert client.calls['file_change'] == 4
         output.reset()
         with open(test_output, 'r') as f:
             assert f.read() == ""
     finally:
         os.remove(test_output)
```

### Comparing `pinthesky-0.8.1/tests/test_session.py` & `pinthesky-0.9.0/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `pinthesky-0.8.1/tests/test_upload.py` & `pinthesky-0.9.0/tests/test_upload.py`

 * *Files identical despite different names*

